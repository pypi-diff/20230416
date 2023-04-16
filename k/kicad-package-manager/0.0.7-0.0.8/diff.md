# Comparing `tmp/kicad_package_manager-0.0.7.tar.gz` & `tmp/kicad_package_manager-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kicad_package_manager-0.0.7.tar", last modified: Sun Apr 16 01:52:38 2023, max compression
+gzip compressed data, was "kicad_package_manager-0.0.8.tar", last modified: Sun Apr 16 02:49:46 2023, max compression
```

## Comparing `kicad_package_manager-0.0.7.tar` & `kicad_package_manager-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:52:38.626365 kicad_package_manager-0.0.7/
--rwxrwxrwx   0 root         (0) root         (0)     3407 2023-04-16 01:52:38.624255 kicad_package_manager-0.0.7/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1938 2023-04-15 20:55:43.000000 kicad_package_manager-0.0.7/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:52:38.518590 kicad_package_manager-0.0.7/kicad_package_manager/
--rwxrwxrwx   0 root         (0) root         (0)       14 2023-04-16 00:09:47.000000 kicad_package_manager-0.0.7/kicad_package_manager/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      651 2023-04-15 08:32:16.000000 kicad_package_manager-0.0.7/kicad_package_manager/config.py
--rwxrwxrwx   0 root         (0) root         (0)      504 2023-04-16 01:05:16.000000 kicad_package_manager-0.0.7/kicad_package_manager/init.py
--rwxrwxrwx   0 root         (0) root         (0)     1862 2023-04-16 01:44:17.000000 kicad_package_manager-0.0.7/kicad_package_manager/install.py
--rwxrwxrwx   0 root         (0) root         (0)      959 2023-04-16 01:40:45.000000 kicad_package_manager-0.0.7/kicad_package_manager/kicad_project_tables.py
--rwxrwxrwx   0 root         (0) root         (0)      550 2023-04-16 01:05:45.000000 kicad_package_manager-0.0.7/kicad_package_manager/kpm.py
--rwxrwxrwx   0 root         (0) root         (0)      708 2023-04-16 01:52:09.000000 kicad_package_manager-0.0.7/kicad_package_manager/registry.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:52:38.608298 kicad_package_manager-0.0.7/kicad_package_manager.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3407 2023-04-16 01:52:38.000000 kicad_package_manager-0.0.7/kicad_package_manager.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      528 2023-04-16 01:52:38.000000 kicad_package_manager-0.0.7/kicad_package_manager.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-16 01:52:38.000000 kicad_package_manager-0.0.7/kicad_package_manager.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       56 2023-04-16 01:52:38.000000 kicad_package_manager-0.0.7/kicad_package_manager.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2023-04-16 01:52:38.000000 kicad_package_manager-0.0.7/kicad_package_manager.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-04-16 01:52:38.000000 kicad_package_manager-0.0.7/kicad_package_manager.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-16 01:52:38.627605 kicad_package_manager-0.0.7/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3832 2023-04-16 01:52:18.000000 kicad_package_manager-0.0.7/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 02:49:46.728020 kicad_package_manager-0.0.8/
+-rwxrwxrwx   0 root         (0) root         (0)     3543 2023-04-16 02:49:46.720894 kicad_package_manager-0.0.8/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2060 2023-04-16 01:54:19.000000 kicad_package_manager-0.0.8/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 02:49:46.430459 kicad_package_manager-0.0.8/kicad_package_manager/
+-rwxrwxrwx   0 root         (0) root         (0)       14 2023-04-16 02:15:17.000000 kicad_package_manager-0.0.8/kicad_package_manager/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      614 2023-04-16 02:15:17.000000 kicad_package_manager-0.0.8/kicad_package_manager/config.py
+-rwxrwxrwx   0 root         (0) root         (0)      479 2023-04-16 02:15:17.000000 kicad_package_manager-0.0.8/kicad_package_manager/init.py
+-rwxrwxrwx   0 root         (0) root         (0)     1815 2023-04-16 02:18:30.000000 kicad_package_manager-0.0.8/kicad_package_manager/install.py
+-rwxrwxrwx   0 root         (0) root         (0)     1105 2023-04-16 02:17:53.000000 kicad_package_manager-0.0.8/kicad_package_manager/kicad_project_tables.py
+-rwxrwxrwx   0 root         (0) root         (0)      842 2023-04-16 02:45:56.000000 kicad_package_manager-0.0.8/kicad_package_manager/kpm.py
+-rwxrwxrwx   0 root         (0) root         (0)      358 2023-04-16 02:49:10.000000 kicad_package_manager-0.0.8/kicad_package_manager/listt.py
+-rwxrwxrwx   0 root         (0) root         (0)      777 2023-04-16 02:48:10.000000 kicad_package_manager-0.0.8/kicad_package_manager/registry.py
+-rwxrwxrwx   0 root         (0) root         (0)      437 2023-04-16 02:46:21.000000 kicad_package_manager-0.0.8/kicad_package_manager/search.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 02:49:46.677664 kicad_package_manager-0.0.8/kicad_package_manager.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3543 2023-04-16 02:49:45.000000 kicad_package_manager-0.0.8/kicad_package_manager.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      591 2023-04-16 02:49:45.000000 kicad_package_manager-0.0.8/kicad_package_manager.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-16 02:49:45.000000 kicad_package_manager-0.0.8/kicad_package_manager.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       56 2023-04-16 02:49:45.000000 kicad_package_manager-0.0.8/kicad_package_manager.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-04-16 02:49:45.000000 kicad_package_manager-0.0.8/kicad_package_manager.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-04-16 02:49:45.000000 kicad_package_manager-0.0.8/kicad_package_manager.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-16 02:49:46.730759 kicad_package_manager-0.0.8/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3832 2023-04-16 02:49:26.000000 kicad_package_manager-0.0.8/setup.py
```

### Comparing `kicad_package_manager-0.0.7/PKG-INFO` & `kicad_package_manager-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kicad_package_manager
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package manager for KiCad projects
 Home-page: https://github.com/danroblewis/kicad-package-manager
 Author: Daniel Lewis
 Author-email: daniel.robert.lewis@gmail.com
 License: MIT
 Description: 
         # KiCad Package Manager
@@ -50,14 +50,16 @@
         kpm init
         
         kpm install https://github.com/danroblewis/kicad-eurorack-tools.git
         
         kpm install .
         ```
         
+        To add a new package to the package index, [submit a pull request](https://github.com/danroblewis/kicad-package-index)
+        
         
         ### kpm.json
         ```json
         {
         	"name": "cool-project",
         	"version": "0.0.1",
         	"author": "danroblewis",
```

### Comparing `kicad_package_manager-0.0.7/README.md` & `kicad_package_manager-0.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 kpm init
 
 kpm install https://github.com/danroblewis/kicad-eurorack-tools.git
 
 kpm install .
 ```
 
+To add a new package to the package index, [submit a pull request](https://github.com/danroblewis/kicad-package-index)
+
 
 ### kpm.json
 ```json
 {
 	"name": "cool-project",
 	"version": "0.0.1",
 	"author": "danroblewis",
```

### Comparing `kicad_package_manager-0.0.7/kicad_package_manager/config.py` & `kicad_package_manager-0.0.8/kicad_package_manager/config.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import json
-
-
-class Config:
-	defaults = {
-		"name": "",
-		"version": "0.0.0",
-		"author": "",
-		"homepage": "",
-		"commands": {},
-		"dependencies": {},
-	}
-
-	def __init__(self, j={}):
-		self.j = j
-	
-	def __getattr__(self, name):
-		if name in self.j:
-			return self.j[name]
-		elif name in self.defaults:
-			return self.defaults[name]
-		else:
-			raise Exception(f"unknown config value '{name}'")
-
-	def toJSON(self):
-		d = {}
-		for k in self.defaults:
-			d[k] = self.__getattr__(k)
-		return json.dumps(d, indent=4)
-
-
-def parse_config(filepath="./kpm.json"):
-	with open(filepath) as f:
-		return Config(json.load(f))
-
-
-
+import json
+
+
+class Config:
+	defaults = {
+		"name": "",
+		"version": "0.0.0",
+		"author": "",
+		"homepage": "",
+		"commands": {},
+		"dependencies": {},
+	}
+
+	def __init__(self, j={}):
+		self.j = j
+	
+	def __getattr__(self, name):
+		if name in self.j:
+			return self.j[name]
+		elif name in self.defaults:
+			return self.defaults[name]
+		else:
+			raise Exception(f"unknown config value '{name}'")
+
+	def toJSON(self):
+		d = {}
+		for k in self.defaults:
+			d[k] = self.__getattr__(k)
+		return json.dumps(d, indent=4)
+
+
+def parse_config(filepath="./kpm.json"):
+	with open(filepath) as f:
+		return Config(json.load(f))
+
+
+
```

### Comparing `kicad_package_manager-0.0.7/kicad_package_manager/install.py` & `kicad_package_manager-0.0.8/kicad_package_manager/install.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-import json
-from . import config
-import requests
-from .registry import get_release_for
-import os
-import io
-import zipfile
-from . import kicad_project_tables
-import glob
-import shutil
-
-
-def run_command(args):
-	package_ref = args.package_ref
-
-	if package_ref == '.':
-		c = config.parse_config()
-		deps = {}
-		for depname, depversion in c.dependencies.items():
-			explore_deps(depname, depversion, deps)
-		install_deps(deps)
-
-
-def explore_deps(name, version, found_packages={}):
-	if name in found_packages:
-		if found_packages[name] != version:
-			raise Exception(f"incompatible version for {name}: {version}, committed version is {found_packages[name]['version']}")
-		else:
-			return found_packages
-
-	release = get_release_for(name, version)
-	found_packages[name] = release
-
-	if 'dependencies' in release:
-		for depname, depversion in release['dependencies'].items():
-			explore_deps(depname, depversion, found_packages)
-
-	return found_packages
-
-
-def install_deps(deps):
-	shutil.rmtree("./kpm_modules", ignore_errors=True)
-	for package_name, release in deps.items():
-		print(f"installing {package_name}")
-		install_package(package_name, release['version'], release['artifact_url'])
-	install_libraries()
-
-
-def install_package(name, version, zip_url):
-	package_dir = f"./kpm_modules/{name}@{version}/"
-	os.makedirs(package_dir, exist_ok=True)
-	res = requests.get(zip_url)
-	r = zipfile.ZipFile(io.BytesIO(res.content)).extractall(package_dir)
-
-
-def install_libraries():
-	# link symbol files
-	symfiles = glob.glob("**/*.kicad_sym", recursive=True)
-	kicad_project_tables.write_sym_lib_table(symfiles)
-
-	# link footprint files
-	footfiles = glob.glob("**/*.kicad_mod", recursive=True)
-	kicad_project_tables.write_fp_lib_table(footfiles)
-
-	# install 3d models
-	# install spice models
-	# install plugins
-
+import json
+from . import config
+import requests
+from .registry import get_release_for
+import os
+import io
+import zipfile
+from . import kicad_project_tables
+import glob
+import shutil
+
+
+def run_command(args):
+	package_ref = args.package_ref
+
+	if package_ref == '.':
+		c = config.parse_config()
+		deps = {}
+		for depname, depversion in c.dependencies.items():
+			explore_deps(depname, depversion, deps)
+		install_deps(deps)
+
+
+def explore_deps(name, version, found_packages={}):
+	if name in found_packages:
+		if found_packages[name] != version:
+			raise Exception(f"incompatible version for {name}: {version}, committed version is {found_packages[name]['version']}")
+		else:
+			return found_packages
+
+	release = get_release_for(name, version)
+	found_packages[name] = release
+
+	if 'dependencies' in release:
+		for depname, depversion in release['dependencies'].items():
+			explore_deps(depname, depversion, found_packages)
+
+	return found_packages
+
+
+def install_deps(deps):
+	shutil.rmtree("./kpm_modules", ignore_errors=True)
+	for package_name, release in deps.items():
+		print(f"installing {package_name}")
+		install_package(package_name, release['version'], release['artifact_url'])
+	install_libraries()
+
+
+def install_package(name, version, zip_url):
+	package_dir = f"./kpm_modules/{name}@{version}/"
+	os.makedirs(package_dir, exist_ok=True)
+	res = requests.get(zip_url)
+	r = zipfile.ZipFile(io.BytesIO(res.content)).extractall(package_dir)
+
+
+def install_libraries():
+	# link symbol files
+	symfiles = glob.glob("kpm_modules/**/*.kicad_sym", recursive=True)
+	kicad_project_tables.write_sym_lib_table(symfiles)
+
+	# link footprint files
+	footfiles = glob.glob("kpm_modules/**/*.pretty", recursive=True)
+	kicad_project_tables.write_fp_lib_table(footfiles)
+
+	# install 3d models
+	# install spice models
+	# install plugins
+
```

### Comparing `kicad_package_manager-0.0.7/kicad_package_manager.egg-info/PKG-INFO` & `kicad_package_manager-0.0.8/kicad_package_manager.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kicad-package-manager
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package manager for KiCad projects
 Home-page: https://github.com/danroblewis/kicad-package-manager
 Author: Daniel Lewis
 Author-email: daniel.robert.lewis@gmail.com
 License: MIT
 Description: 
         # KiCad Package Manager
@@ -50,14 +50,16 @@
         kpm init
         
         kpm install https://github.com/danroblewis/kicad-eurorack-tools.git
         
         kpm install .
         ```
         
+        To add a new package to the package index, [submit a pull request](https://github.com/danroblewis/kicad-package-index)
+        
         
         ### kpm.json
         ```json
         {
         	"name": "cool-project",
         	"version": "0.0.1",
         	"author": "danroblewis",
```

### Comparing `kicad_package_manager-0.0.7/setup.py` & `kicad_package_manager-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'kicad_package_manager'
 DESCRIPTION = 'A package manager for KiCad projects'
 URL = 'https://github.com/danroblewis/kicad-package-manager'
 EMAIL = 'daniel.robert.lewis@gmail.com'
 AUTHOR = 'Daniel Lewis'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'sexpdata'
 ]
```

