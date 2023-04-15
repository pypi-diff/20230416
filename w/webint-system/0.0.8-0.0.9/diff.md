# Comparing `tmp/webint_system-0.0.8.tar.gz` & `tmp/webint_system-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webint_system-0.0.8.tar", max compression
+gzip compressed data, was "webint_system-0.0.9.tar", max compression
```

## Comparing `webint_system-0.0.8.tar` & `webint_system-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1119 2023-03-10 04:17:57.443160 webint_system-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3429 2023-03-10 04:17:32.954820 webint_system-0.0.8/webint_system/__init__.py
--rw-r--r--   0        0        0      143 2023-02-19 22:52:12.932021 webint_system-0.0.8/webint_system/templates/__init__.py
--rw-r--r--   0        0        0     6313 2023-03-08 02:50:37.340106 webint_system-0.0.8/webint_system/templates/index.html
--rw-r--r--   0        0        0      149 2023-02-19 22:46:12.283338 webint_system-0.0.8/webint_system/templates/template.html
--rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 webint_system-0.0.8/setup.py
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 webint_system-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1119 2023-03-12 06:59:33.717673 webint_system-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5002 2023-03-12 06:58:41.128938 webint_system-0.0.9/webint_system/__init__.py
+-rw-r--r--   0        0        0      143 2023-02-19 22:52:12.932021 webint_system-0.0.9/webint_system/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-11 01:38:23.631030 webint_system-0.0.9/webint_system/templates/addresses/__init__.py
+-rw-r--r--   0        0        0      538 2023-03-11 05:11:06.963716 webint_system-0.0.9/webint_system/templates/addresses/domains.html
+-rw-r--r--   0        0        0     6315 2023-03-11 01:36:04.165235 webint_system-0.0.9/webint_system/templates/index.html
+-rw-r--r--   0        0        0      149 2023-02-19 22:46:12.283338 webint_system-0.0.9/webint_system/templates/template.html
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 webint_system-0.0.9/setup.py
+-rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 webint_system-0.0.9/PKG-INFO
```

### Comparing `webint_system-0.0.8/pyproject.toml` & `webint_system-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "webint-system"
-version = "0.0.8"
+version = "0.0.9"
 description = "manage the system"
 keywords = ["webint"]
 homepage = "https://ragt.ag/code/projects/webint-system"
 repository = "https://ragt.ag/code/projects/webint-system.git"
 documentation = "https://ragt.ag/code/projects/webint-system/api"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "BSD-2-Clause"
```

### Comparing `webint_system-0.0.8/webint_system/__init__.py` & `webint_system-0.0.9/webint_system/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 app = web.application(__name__, prefix="system")
 
 code_dir = pathlib.Path.home() / "code"
 meta_dir = code_dir / "meta"
 working_dir = code_dir / "working"
 
 
+def get_ip():
+    return subprocess.check_output(["hostname", "-I"]).split()[0].decode()
+
+
 def update_system(package):
     print(
         subprocess.run(
             ["/home/gaea/runinenv", "/home/gaea/app", "pip", "install", "-U", package],
             capture_output=True,
         )
     )
@@ -66,25 +70,24 @@
 class System:
     """The system that runs your website."""
 
     def get(self):
         """"""
         if not web.tx.user.is_owner:
             return "owner only"
-        ip_address = subprocess.check_output(["hostname", "-I"]).split()[0].decode()
         try:
             with open("/home/gaea/app/run/onion") as fp:
                 onion = fp.read()
         except FileNotFoundError:
             onion = None
         domains = []
         webint_metadata = importlib.metadata.metadata("webint")
         webint_versions = get_versions("webint")
         return app.view.index(
-            ip_address,
+            get_ip(),
             onion,
             domains,
             web.tx.app.cfg,
             web.tx.app,
             web.get_apps(),
             webint_metadata,
             webint_versions,
@@ -96,14 +99,64 @@
     """System addresses."""
 
     def post(self):
         """"""
         return "addresses have been updated"
 
 
+@app.control("addresses/domains")
+class Domains:
+    """System addresses."""
+
+    def get(self):
+        """"""
+        form = web.form("domain")
+        records = {}
+        for record in ("A", "CNAME", "MX", "NS"):
+            try:
+                records[record] = web.dns.resolve(form.domain, record)
+            except (web.dns.NoAnswer, web.dns.NXDOMAIN):
+                pass
+        return app.view.addresses.domains(get_ip(), form.domain, records)
+
+    def post(self):
+        form = web.form("domain")
+        web.enqueue(add_domain, form.domain)
+        return "adding domain"
+
+
+def add_domain(domain):
+    ip = get_ip()
+    with open("onion") as fp:
+        onion = fp.read()
+
+    domain_path = pathlib.Path("domains")
+    with domain_path.open() as fp:
+        domains = {domain: True for domain in fp.readlines()}
+    domains[domain] = False
+
+    nginx_conf_path = pathlib.Path("/etc/nginx/nginx.conf")
+    with nginx_conf_path.open("w") as fp:
+        fp.write(web.host.templates.nginx(ip, onion, domains))
+    subprocess.call(["sudo", "service", "nginx", "restart"])
+
+    web.generate_cert(domain)
+    subprocess.call(["cp", f"certs/{domain}/domain.key", "/etc/ssl/private"])
+    subprocess.call(["cp", f"certs/{domain}/domain.crt", "/etc/ssl/certs"])
+
+    domains[domain] = True
+    with nginx_conf_path.open("w") as fp:
+        fp.write(web.host.templates.nginx(ip, onion, domains))
+    subprocess.call(["sudo", "service", "nginx", "restart"])
+
+    with domain_path.open("w") as fp:
+        for domain in domains:
+            print(domain, file=fp)
+
+
 @app.control("settings")
 class Settings:
     """System settings."""
 
     def post(self):
         """"""
         form = web.form("key", "value")
```

### Comparing `webint_system-0.0.8/webint_system/templates/index.html` & `webint_system-0.0.9/webint_system/templates/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 $def with (ip_address, onion, domains, settings, main_app, apps, webint_metadata, webint_versions)
 $# , understory_version, applications)
 $var title: System
 
 <h2>Addresses</h2>
-<p><strong>IP:</strong> $ip_address</p>
-<p><strong>Onion:</strong> $onion</p>
+<p>$ip_address</p>
+$if onion:
+    <p style=font-family:monospace>$(onion[:28])&shy;$(onion[28:]).onion</p>
 <form method=post action=/addresses/tor/miner>
 <button>Mine</button>
 </form>
-<p><strong>Domains:</strong> $", ".join(domains)</p>
-<form method=post action=/addresses/domains>
+<p>$", ".join(domains)</p>
+<form method=get action=/addresses/domains>
 <input name=domain> <button>Lookup</button>
 </form>
 
 <h2>Settings</h2>
 <ul>
 $for key, value in settings.items():
     <li><strong>$key:</strong> <code>$value</code></li>
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
 $def with (ip_address, onion, domains, settings, main_app, apps,
 webint_metadata, webint_versions) $# , understory_version, applications) $var
 title: System
 ***** Addresses *****
-IP: $ip_address
-Onion: $onion
+$ip_address
+$if onion:
+$(onion[:28])­$(onion[28:]).onion
 Mine
-Domains: $", ".join(domains)
+$", ".join(domains)
 [domain              ] Lookup
 ***** Settings *****
     * $for key, value in settings.items():
     * $key: $value
 [key                 ] [value               ] Add
 ***** Software *****
 Primary application: $main_app.name
```

### Comparing `webint_system-0.0.8/setup.py` & `webint_system-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['webint_system', 'webint_system.templates']
+['webint_system',
+ 'webint_system.templates',
+ 'webint_system.templates.addresses']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['bgq>=0.0',
  'gmpg>=0.0',
@@ -15,15 +17,15 @@
  'webint>=0.0']
 
 entry_points = \
 {'webapps': ['system = webint_system:app']}
 
 setup_kwargs = {
     'name': 'webint-system',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'manage the system',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ragt.ag/code/projects/webint-system',
```

### Comparing `webint_system-0.0.8/PKG-INFO` & `webint_system-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webint-system
-Version: 0.0.8
+Version: 0.0.9
 Summary: manage the system
 Home-page: https://ragt.ag/code/projects/webint-system
 License: BSD-2-Clause
 Keywords: webint
 Author: Angelo Gladding
 Author-email: angelo@ragt.ag
 Requires-Python: >=3.10,<3.11
```

