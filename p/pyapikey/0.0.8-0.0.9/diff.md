# Comparing `tmp/pyapikey-0.0.8.tar.gz` & `tmp/pyapikey-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyapikey-0.0.8.tar", last modified: Sun Apr 16 18:18:27 2023, max compression
+gzip compressed data, was "pyapikey-0.0.9.tar", last modified: Sun Apr 16 18:26:54 2023, max compression
```

## Comparing `pyapikey-0.0.8.tar` & `pyapikey-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 18:18:27.058752 pyapikey-0.0.8/
--rw-r--r--   0 mark      (1000) mark      (1000)     1069 2023-04-16 18:18:15.000000 pyapikey-0.0.8/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)     1325 2023-04-16 18:18:27.058752 pyapikey-0.0.8/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      390 2023-04-16 18:18:15.000000 pyapikey-0.0.8/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 18:18:27.057752 pyapikey-0.0.8/pyapikey/
--rw-r--r--   0 mark      (1000) mark      (1000)       46 2020-10-02 10:21:11.000000 pyapikey-0.0.8/pyapikey/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1382 2023-04-16 18:17:51.000000 pyapikey-0.0.8/pyapikey/core.py
--rw-r--r--   0 mark      (1000) mark      (1000)      172 2023-04-16 18:18:15.000000 pyapikey-0.0.8/pyapikey/static.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 18:18:27.058752 pyapikey-0.0.8/pyapikey.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1325 2023-04-16 18:18:26.000000 pyapikey-0.0.8/pyapikey.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      222 2023-04-16 18:18:27.000000 pyapikey-0.0.8/pyapikey.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-16 18:18:26.000000 pyapikey-0.0.8/pyapikey.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-04-16 18:18:26.000000 pyapikey-0.0.8/pyapikey.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-16 18:18:27.058752 pyapikey-0.0.8/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1351 2023-04-16 18:18:15.000000 pyapikey-0.0.8/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 18:26:54.028745 pyapikey-0.0.9/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1069 2023-04-16 18:26:31.000000 pyapikey-0.0.9/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1325 2023-04-16 18:26:54.029745 pyapikey-0.0.9/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      390 2023-04-16 18:26:31.000000 pyapikey-0.0.9/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 18:26:54.028745 pyapikey-0.0.9/pyapikey/
+-rw-r--r--   0 mark      (1000) mark      (1000)       46 2020-10-02 10:21:11.000000 pyapikey-0.0.9/pyapikey/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1452 2023-04-16 18:26:22.000000 pyapikey-0.0.9/pyapikey/core.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      172 2023-04-16 18:26:31.000000 pyapikey-0.0.9/pyapikey/static.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 18:26:54.028745 pyapikey-0.0.9/pyapikey.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1325 2023-04-16 18:26:53.000000 pyapikey-0.0.9/pyapikey.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      222 2023-04-16 18:26:53.000000 pyapikey-0.0.9/pyapikey.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-16 18:26:53.000000 pyapikey-0.0.9/pyapikey.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-04-16 18:26:53.000000 pyapikey-0.0.9/pyapikey.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-16 18:26:54.029745 pyapikey-0.0.9/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1351 2023-04-16 18:26:31.000000 pyapikey-0.0.9/setup.py
```

### Comparing `pyapikey-0.0.8/LICENSE` & `pyapikey-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyapikey-0.0.8/PKG-INFO` & `pyapikey-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyapikey
-Version: 0.0.8
+Version: 0.0.9
 Summary: access api keys from code
 Home-page: https://veltzer.github.io/pyapikey
 Download-URL: https://github.com/veltzer/pyapikey
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pyapikey
 
 author: Mark Veltzer
 
-version: 0.0.8
+version: 0.0.9
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2020, 2021, 2022, 2023
```

### Comparing `pyapikey-0.0.8/pyapikey/core.py` & `pyapikey-0.0.9/pyapikey/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,10 +41,12 @@
         self.data[key] = value
 
     def has(self, key: str) -> bool:
         return key in self.data
 
     def save(self):
         filename = os.path.expanduser("~/.config/pyapikey.temp.json")
-        os.makedirs(os.path.dirname(filename))
-        with open(filename, 'w') as file_handle:
+        dirname = os.path.dirname(filename)
+        if not os.path.isdir(dirname):
+            os.makedirs(dirname)
+        with open(filename, "wt") as file_handle:
             json.dump(fp=file_handle, obj=self.data, default=default, indent=4)
```

### Comparing `pyapikey-0.0.8/pyapikey.egg-info/PKG-INFO` & `pyapikey-0.0.9/pyapikey.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyapikey
-Version: 0.0.8
+Version: 0.0.9
 Summary: access api keys from code
 Home-page: https://veltzer.github.io/pyapikey
 Download-URL: https://github.com/veltzer/pyapikey
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pyapikey
 
 author: Mark Veltzer
 
-version: 0.0.8
+version: 0.0.9
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2020, 2021, 2022, 2023
```

### Comparing `pyapikey-0.0.8/setup.py` & `pyapikey-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pyapikey",
-    version="0.0.8",
+    version="0.0.9",
     packages=[
         "pyapikey",
     ],
     # from here all is optional
     description="access api keys from code",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
```

