# Comparing `tmp/goastpy-0.1.0.tar.gz` & `tmp/goastpy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goastpy-0.1.0.tar", last modified: Sun Apr 16 12:42:36 2023, max compression
+gzip compressed data, was "goastpy-0.1.1.tar", last modified: Sun Apr 16 13:05:44 2023, max compression
```

## Comparing `goastpy-0.1.0.tar` & `goastpy-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,11 @@
-drwxr-xr-x   0 monolite   (502) staff       (20)        0 2023-04-16 12:42:36.153555 goastpy-0.1.0/
--rw-r--r--   0 monolite   (502) staff       (20)     1064 2023-04-16 11:48:27.000000 goastpy-0.1.0/LICENSE
--rw-r--r--   0 monolite   (502) staff       (20)      774 2023-04-16 12:42:36.153648 goastpy-0.1.0/PKG-INFO
--rw-r--r--   0 monolite   (502) staff       (20)       54 2023-04-16 11:48:27.000000 goastpy-0.1.0/README.md
-drwxr-xr-x   0 monolite   (502) staff       (20)        0 2023-04-16 12:42:36.152731 goastpy-0.1.0/goastpy/
--rw-r--r--   0 monolite   (502) staff       (20)       39 2023-04-16 12:27:23.000000 goastpy-0.1.0/goastpy/__init__.py
--rw-r--r--   0 monolite   (502) staff       (20)     2180 2023-04-16 12:29:36.000000 goastpy-0.1.0/goastpy/goastparser_wrapper.py
-drwxr-xr-x   0 monolite   (502) staff       (20)        0 2023-04-16 12:42:36.153433 goastpy-0.1.0/goastpy.egg-info/
--rw-r--r--   0 monolite   (502) staff       (20)      774 2023-04-16 12:42:36.000000 goastpy-0.1.0/goastpy.egg-info/PKG-INFO
--rw-r--r--   0 monolite   (502) staff       (20)      211 2023-04-16 12:42:36.000000 goastpy-0.1.0/goastpy.egg-info/SOURCES.txt
--rw-r--r--   0 monolite   (502) staff       (20)        1 2023-04-16 12:42:36.000000 goastpy-0.1.0/goastpy.egg-info/dependency_links.txt
--rw-r--r--   0 monolite   (502) staff       (20)        8 2023-04-16 12:42:36.000000 goastpy-0.1.0/goastpy.egg-info/top_level.txt
--rw-r--r--   0 monolite   (502) staff       (20)       79 2023-04-16 12:42:36.154068 goastpy-0.1.0/setup.cfg
--rw-r--r--   0 monolite   (502) staff       (20)      888 2023-04-16 12:39:05.000000 goastpy-0.1.0/setup.py
+drwxr-xr-x   0 monolite   (502) staff       (20)        0 2023-04-16 13:05:44.488643 goastpy-0.1.1/
+-rw-r--r--   0 monolite   (502) staff       (20)     1064 2023-04-16 11:48:27.000000 goastpy-0.1.1/LICENSE
+-rw-r--r--   0 monolite   (502) staff       (20)      774 2023-04-16 13:05:44.488742 goastpy-0.1.1/PKG-INFO
+-rw-r--r--   0 monolite   (502) staff       (20)       54 2023-04-16 11:48:27.000000 goastpy-0.1.1/README.md
+drwxr-xr-x   0 monolite   (502) staff       (20)        0 2023-04-16 13:05:44.488520 goastpy-0.1.1/goastpy.egg-info/
+-rw-r--r--   0 monolite   (502) staff       (20)      774 2023-04-16 13:05:44.000000 goastpy-0.1.1/goastpy.egg-info/PKG-INFO
+-rw-r--r--   0 monolite   (502) staff       (20)      160 2023-04-16 13:05:44.000000 goastpy-0.1.1/goastpy.egg-info/SOURCES.txt
+-rw-r--r--   0 monolite   (502) staff       (20)        1 2023-04-16 13:05:44.000000 goastpy-0.1.1/goastpy.egg-info/dependency_links.txt
+-rw-r--r--   0 monolite   (502) staff       (20)        1 2023-04-16 13:05:44.000000 goastpy-0.1.1/goastpy.egg-info/top_level.txt
+-rw-r--r--   0 monolite   (502) staff       (20)       79 2023-04-16 13:05:44.489035 goastpy-0.1.1/setup.cfg
+-rw-r--r--   0 monolite   (502) staff       (20)      903 2023-04-16 13:05:42.000000 goastpy-0.1.1/setup.py
```

### Comparing `goastpy-0.1.0/LICENSE` & `goastpy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `goastpy-0.1.0/PKG-INFO` & `goastpy-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goastpy
-Version: 0.1.0
+Version: 0.1.1
 Summary: a python wrapper for the built-in go parser using c-types
 Home-page: https://github.com/itayg25/goastpy
 Download-URL: https://github.com/itayg25/goastpy/archive/v_01.tar.gz
 Author: Itay Gersten
 Author-email: Itay.Gersten@gmail.com
 License: MIT
 Keywords: GO,GOLANG,PYTHON,AST,GOPYGO
```

### Comparing `goastpy-0.1.0/goastpy.egg-info/PKG-INFO` & `goastpy-0.1.1/goastpy.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goastpy
-Version: 0.1.0
+Version: 0.1.1
 Summary: a python wrapper for the built-in go parser using c-types
 Home-page: https://github.com/itayg25/goastpy
 Download-URL: https://github.com/itayg25/goastpy/archive/v_01.tar.gz
 Author: Itay Gersten
 Author-email: Itay.Gersten@gmail.com
 License: MIT
 Keywords: GO,GOLANG,PYTHON,AST,GOPYGO
```

### Comparing `goastpy-0.1.0/setup.py` & `goastpy-0.1.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from distutils.core import setup
+from setuptools import setup, find_packages
 
 setup(
     name='goastpy',
-    packages=['goastpy'],
-    version='0.1.0',
+    packages=find_packages(),
+    version='0.1.1',
     license='MIT',
     description='a python wrapper for the built-in go parser using c-types',
     author='Itay Gersten',
     author_email='Itay.Gersten@gmail.com',
     url='https://github.com/itayg25/goastpy',
     download_url='https://github.com/itayg25/goastpy/archive/v_01.tar.gz',
     keywords=['GO', 'GOLANG', 'PYTHON', 'AST', 'GOPYGO'],
```

