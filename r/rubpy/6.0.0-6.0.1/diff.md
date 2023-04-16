# Comparing `tmp/rubpy-6.0.0.tar.gz` & `tmp/rubpy-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-6.0.0.tar", last modified: Sun Apr 16 00:16:26 2023, max compression
+gzip compressed data, was "rubpy-6.0.1.tar", last modified: Sun Apr 16 00:20:24 2023, max compression
```

## Comparing `rubpy-6.0.0.tar` & `rubpy-6.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 00:16:26.711695 rubpy-6.0.0/
--rw-rw-rw-   0        0        0     3548 2023-04-16 00:16:26.711695 rubpy-6.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2455 2023-04-16 00:08:40.000000 rubpy-6.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 00:16:26.711695 rubpy-6.0.0/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3548 2023-04-16 00:16:26.000000 rubpy-6.0.0/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-04-16 00:16:26.000000 rubpy-6.0.0/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 00:16:26.000000 rubpy-6.0.0/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-16 00:16:26.000000 rubpy-6.0.0/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 00:16:26.000000 rubpy-6.0.0/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 00:16:26.711695 rubpy-6.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1568 2023-04-16 00:15:10.000000 rubpy-6.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 00:20:24.989141 rubpy-6.0.1/
+-rw-rw-rw-   0        0        0     3548 2023-04-16 00:20:24.989141 rubpy-6.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2455 2023-04-16 00:08:40.000000 rubpy-6.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 00:20:24.989141 rubpy-6.0.1/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3548 2023-04-16 00:20:24.000000 rubpy-6.0.1/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-04-16 00:20:24.000000 rubpy-6.0.1/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 00:20:24.000000 rubpy-6.0.1/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-16 00:20:24.000000 rubpy-6.0.1/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 00:20:24.000000 rubpy-6.0.1/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 00:20:24.989141 rubpy-6.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1436 2023-04-16 00:20:04.000000 rubpy-6.0.1/setup.py
```

### Comparing `rubpy-6.0.0/PKG-INFO` & `rubpy-6.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.0.0
+Version: 6.0.1
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.0.0 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.0.1 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: License :: OSI Approved :: GNU Lesser
```

### Comparing `rubpy-6.0.0/README.md` & `rubpy-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.0/rubpy.egg-info/PKG-INFO` & `rubpy-6.0.1/rubpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.0.0
+Version: 6.0.1
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.0.0 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.0.1 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: License :: OSI Approved :: GNU Lesser
```

### Comparing `rubpy-6.0.0/setup.py` & `rubpy-6.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-import re
 from setuptools import find_packages, setup
 
-with open('rubpy/__init__.py', 'r') as f:
-    version = re.search(r'__version__\s*=\s*\'(\S+)\'', f.read()).group(1)
-
 with open("README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
     name='rubpy',
-    version=version,
+    version='6.0.1',
     author='Shayan Heidari',
     url='https://github.com/shayanheidari01/rubika',
     author_email = 'contact@shayanheidari.info',
     description='This is an unofficial library and fastest library for deploying robots on Rubika accounts.',
     python_requires='>=3.7',
     long_description=readme,
     long_description_content_type = 'text/markdown',
```

