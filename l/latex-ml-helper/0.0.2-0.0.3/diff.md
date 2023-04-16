# Comparing `tmp/latex_ml_helper-0.0.2.tar.gz` & `tmp/latex_ml_helper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latex_ml_helper-0.0.2.tar", last modified: Sun Apr 16 16:23:40 2023, max compression
+gzip compressed data, was "latex_ml_helper-0.0.3.tar", last modified: Sun Apr 16 18:14:27 2023, max compression
```

## Comparing `latex_ml_helper-0.0.2.tar` & `latex_ml_helper-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 16:23:40.357055 latex_ml_helper-0.0.2/
--rw-rw-rw-   0        0        0      657 2023-04-16 16:23:40.357055 latex_ml_helper-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 16:23:40.355055 latex_ml_helper-0.0.2/latex_ml_helper.egg-info/
--rw-rw-rw-   0        0        0      657 2023-04-16 16:23:40.000000 latex_ml_helper-0.0.2/latex_ml_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-04-16 16:23:40.000000 latex_ml_helper-0.0.2/latex_ml_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 16:23:40.000000 latex_ml_helper-0.0.2/latex_ml_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-16 16:23:40.000000 latex_ml_helper-0.0.2/latex_ml_helper.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 16:23:40.356055 latex_ml_helper-0.0.2/libraries/
--rw-rw-rw-   0        0        0       42 2023-04-16 16:21:20.000000 latex_ml_helper-0.0.2/libraries/__init__.py
--rw-rw-rw-   0        0        0       98 2023-04-16 16:00:15.000000 latex_ml_helper-0.0.2/libraries/definitions.py
--rw-rw-rw-   0        0        0       42 2023-04-16 16:23:40.357055 latex_ml_helper-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      906 2023-04-16 16:21:51.000000 latex_ml_helper-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 18:14:27.668154 latex_ml_helper-0.0.3/
+-rw-rw-rw-   0        0        0      657 2023-04-16 18:14:27.668154 latex_ml_helper-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 18:14:27.664154 latex_ml_helper-0.0.3/latex_ml_helper.egg-info/
+-rw-rw-rw-   0        0        0      657 2023-04-16 18:14:27.000000 latex_ml_helper-0.0.3/latex_ml_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-04-16 18:14:27.000000 latex_ml_helper-0.0.3/latex_ml_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 18:14:27.000000 latex_ml_helper-0.0.3/latex_ml_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-16 18:14:27.000000 latex_ml_helper-0.0.3/latex_ml_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-16 18:14:27.000000 latex_ml_helper-0.0.3/latex_ml_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 18:14:27.667154 latex_ml_helper-0.0.3/libraries/
+-rw-rw-rw-   0        0        0      184 2023-04-16 17:45:57.000000 latex_ml_helper-0.0.3/libraries/__init__.py
+-rw-rw-rw-   0        0        0      168 2023-04-16 17:40:17.000000 latex_ml_helper-0.0.3/libraries/copy.py
+-rw-rw-rw-   0        0        0     1951 2023-04-16 18:12:59.000000 latex_ml_helper-0.0.3/libraries/definitions.py
+-rw-rw-rw-   0        0        0     7677 2023-04-16 17:45:43.000000 latex_ml_helper-0.0.3/libraries/snippets.py
+-rw-rw-rw-   0        0        0       42 2023-04-16 18:14:27.669154 latex_ml_helper-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      917 2023-04-16 18:13:30.000000 latex_ml_helper-0.0.3/setup.py
```

### Comparing `latex_ml_helper-0.0.2/PKG-INFO` & `latex_ml_helper-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latex_ml_helper
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for getting latex equations for machine learning models
 Home-page: UNKNOWN
 Author: Ramal Salha
 Author-email: <ramal.salha@gmail.com>
 License: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
 Platform: UNKNOWN
```

### Comparing `latex_ml_helper-0.0.2/latex_ml_helper.egg-info/PKG-INFO` & `latex_ml_helper-0.0.3/latex_ml_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latex-ml-helper
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for getting latex equations for machine learning models
 Home-page: UNKNOWN
 Author: Ramal Salha
 Author-email: <ramal.salha@gmail.com>
 License: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
 Platform: UNKNOWN
```

### Comparing `latex_ml_helper-0.0.2/setup.py` & `latex_ml_helper-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Package for getting latex equations for machine learning models'
 
 # Setting up
 setup(
     name="latex_ml_helper",
     version=VERSION,
     author="Ramal Salha",
     author_email="<ramal.salha@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     packages=find_packages(),
-    install_requires=[],
+    install_requires=["pyperclip"],
     keywords=['python', 'video', 'stream', 'video stream', 'camera stream', 'sockets'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

