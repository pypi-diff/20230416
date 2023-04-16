# Comparing `tmp/latex_ml_helper-0.0.1.tar.gz` & `tmp/latex_ml_helper-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latex_ml_helper-0.0.1.tar", last modified: Sun Apr 16 16:08:05 2023, max compression
+gzip compressed data, was "latex_ml_helper-0.0.2.tar", last modified: Sun Apr 16 16:23:40 2023, max compression
```

## Comparing `latex_ml_helper-0.0.1.tar` & `latex_ml_helper-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 16:08:05.617689 latex_ml_helper-0.0.1/
--rw-rw-rw-   0        0        0      657 2023-04-16 16:08:05.617689 latex_ml_helper-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 16:08:05.615690 latex_ml_helper-0.0.1/latex_ml_helper.egg-info/
--rw-rw-rw-   0        0        0      657 2023-04-16 16:08:05.000000 latex_ml_helper-0.0.1/latex_ml_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-04-16 16:08:05.000000 latex_ml_helper-0.0.1/latex_ml_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 16:08:05.000000 latex_ml_helper-0.0.1/latex_ml_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-16 16:08:05.000000 latex_ml_helper-0.0.1/latex_ml_helper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 16:08:05.616690 latex_ml_helper-0.0.1/libraries/
--rw-rw-rw-   0        0        0       25 2023-04-16 16:00:47.000000 latex_ml_helper-0.0.1/libraries/__init__.py
--rw-rw-rw-   0        0        0       98 2023-04-16 16:00:15.000000 latex_ml_helper-0.0.1/libraries/definitions.py
--rw-rw-rw-   0        0        0       42 2023-04-16 16:08:05.617689 latex_ml_helper-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      906 2023-04-16 16:04:15.000000 latex_ml_helper-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:23:40.357055 latex_ml_helper-0.0.2/
+-rw-rw-rw-   0        0        0      657 2023-04-16 16:23:40.357055 latex_ml_helper-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 16:23:40.355055 latex_ml_helper-0.0.2/latex_ml_helper.egg-info/
+-rw-rw-rw-   0        0        0      657 2023-04-16 16:23:40.000000 latex_ml_helper-0.0.2/latex_ml_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-04-16 16:23:40.000000 latex_ml_helper-0.0.2/latex_ml_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 16:23:40.000000 latex_ml_helper-0.0.2/latex_ml_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-16 16:23:40.000000 latex_ml_helper-0.0.2/latex_ml_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 16:23:40.356055 latex_ml_helper-0.0.2/libraries/
+-rw-rw-rw-   0        0        0       42 2023-04-16 16:21:20.000000 latex_ml_helper-0.0.2/libraries/__init__.py
+-rw-rw-rw-   0        0        0       98 2023-04-16 16:00:15.000000 latex_ml_helper-0.0.2/libraries/definitions.py
+-rw-rw-rw-   0        0        0       42 2023-04-16 16:23:40.357055 latex_ml_helper-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      906 2023-04-16 16:21:51.000000 latex_ml_helper-0.0.2/setup.py
```

### Comparing `latex_ml_helper-0.0.1/PKG-INFO` & `latex_ml_helper-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latex_ml_helper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for getting latex equations for machine learning models
 Home-page: UNKNOWN
 Author: Ramal Salha
 Author-email: <ramal.salha@gmail.com>
 License: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
 Platform: UNKNOWN
```

### Comparing `latex_ml_helper-0.0.1/latex_ml_helper.egg-info/PKG-INFO` & `latex_ml_helper-0.0.2/latex_ml_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latex-ml-helper
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for getting latex equations for machine learning models
 Home-page: UNKNOWN
 Author: Ramal Salha
 Author-email: <ramal.salha@gmail.com>
 License: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
 Platform: UNKNOWN
```

### Comparing `latex_ml_helper-0.0.1/setup.py` & `latex_ml_helper-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Package for getting latex equations for machine learning models'
 
 # Setting up
 setup(
     name="latex_ml_helper",
     version=VERSION,
     author="Ramal Salha",
```

