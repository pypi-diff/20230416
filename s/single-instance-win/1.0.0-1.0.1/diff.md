# Comparing `tmp/single-instance-win-1.0.0.tar.gz` & `tmp/single-instance-win-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "single-instance-win-1.0.0.tar", last modified: Sun Apr 16 07:17:55 2023, max compression
+gzip compressed data, was "single-instance-win-1.0.1.tar", last modified: Sun Apr 16 07:19:36 2023, max compression
```

## Comparing `single-instance-win-1.0.0.tar` & `single-instance-win-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 07:17:55.449329 single-instance-win-1.0.0/
--rw-rw-rw-   0        0        0     1052 2023-04-16 06:20:23.000000 single-instance-win-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       26 2019-08-27 18:29:08.000000 single-instance-win-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2867 2023-04-16 07:17:55.449329 single-instance-win-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2273 2023-04-16 07:11:39.000000 single-instance-win-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-16 07:17:55.449329 single-instance-win-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1954 2023-04-16 07:17:43.000000 single-instance-win-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:17:55.442245 single-instance-win-1.0.0/single-instance-win/
--rw-rw-rw-   0        0        0       20 2019-08-27 18:29:08.000000 single-instance-win-1.0.0/single-instance-win/__init__.py
--rw-rw-rw-   0        0        0      352 2019-08-27 18:29:08.000000 single-instance-win-1.0.0/single-instance-win/__version__.py
--rw-rw-rw-   0        0        0       26 2019-08-27 18:29:08.000000 single-instance-win-1.0.0/single-instance-win/core.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:17:55.447318 single-instance-win-1.0.0/single_instance_win.egg-info/
--rw-rw-rw-   0        0        0     2867 2023-04-16 07:17:55.000000 single-instance-win-1.0.0/single_instance_win.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-04-16 07:17:55.000000 single-instance-win-1.0.0/single_instance_win.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 07:17:55.000000 single-instance-win-1.0.0/single_instance_win.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-16 07:17:55.000000 single-instance-win-1.0.0/single_instance_win.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-04-16 07:17:55.000000 single-instance-win-1.0.0/single_instance_win.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 07:19:36.014312 single-instance-win-1.0.1/
+-rw-rw-rw-   0        0        0     1052 2023-04-16 06:20:23.000000 single-instance-win-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       26 2019-08-27 18:29:08.000000 single-instance-win-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2863 2023-04-16 07:19:36.014312 single-instance-win-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2269 2023-04-16 07:18:59.000000 single-instance-win-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-16 07:19:36.014312 single-instance-win-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1954 2023-04-16 07:19:33.000000 single-instance-win-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 07:19:36.007768 single-instance-win-1.0.1/single-instance-win/
+-rw-rw-rw-   0        0        0       20 2019-08-27 18:29:08.000000 single-instance-win-1.0.1/single-instance-win/__init__.py
+-rw-rw-rw-   0        0        0      352 2019-08-27 18:29:08.000000 single-instance-win-1.0.1/single-instance-win/__version__.py
+-rw-rw-rw-   0        0        0       26 2019-08-27 18:29:08.000000 single-instance-win-1.0.1/single-instance-win/core.py
+drwxrwxrwx   0        0        0        0 2023-04-16 07:19:36.013303 single-instance-win-1.0.1/single_instance_win.egg-info/
+-rw-rw-rw-   0        0        0     2863 2023-04-16 07:19:35.000000 single-instance-win-1.0.1/single_instance_win.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2023-04-16 07:19:35.000000 single-instance-win-1.0.1/single_instance_win.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 07:19:35.000000 single-instance-win-1.0.1/single_instance_win.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-16 07:19:35.000000 single-instance-win-1.0.1/single_instance_win.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-04-16 07:19:35.000000 single-instance-win-1.0.1/single_instance_win.egg-info/top_level.txt
```

### Comparing `single-instance-win-1.0.0/LICENSE` & `single-instance-win-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `single-instance-win-1.0.0/PKG-INFO` & `single-instance-win-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: single-instance-win
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python module for creating a single instance of an application on Windows.
 Home-page: https://github.com/YuckyFox/432
 Author: YuckyFox
 Author-email: mr.cr.fox@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -27,15 +27,15 @@
 Whether developing a new application or improving an existing one, this module is an essential tool for any developer working with Python on the Windows operating system.
 
 Installation
 -----
 
 ```If you want to use the SingleInstance module in your Python application, you can easily install it via pip:
 
-**pip install singleinstance**
+pip install singleinstance
 
 This will download and install the SingleInstance module and any dependencies it requires, making it available for use in your Python application.
 ```
 
 Usage
 -----
```

### Comparing `single-instance-win-1.0.0/README.md` & `single-instance-win-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Whether developing a new application or improving an existing one, this module is an essential tool for any developer working with Python on the Windows operating system.
 
 Installation
 -----
 
 ```If you want to use the SingleInstance module in your Python application, you can easily install it via pip:
 
-**pip install singleinstance**
+pip install singleinstance
 
 This will download and install the SingleInstance module and any dependencies it requires, making it available for use in your Python application.
 ```
 
 Usage
 -----
```

### Comparing `single-instance-win-1.0.0/setup.py` & `single-instance-win-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import io
 import os
 from shutil import rmtree
 from setuptools import find_packages, setup
 
 # Package meta-data.
 NAME = 'single-instance-win'
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'A Python module for creating a single instance of an application on Windows.'
 URL = 'https://github.com/YuckyFox/432'
 AUTHOR = 'YuckyFox'
 EMAIL = 'mr.cr.fox@gmail.com'
 REQUIRES_PYTHON = '>=3.6.0'
 
 # What packages are required for this module to be executed?
```

### Comparing `single-instance-win-1.0.0/single_instance_win.egg-info/PKG-INFO` & `single-instance-win-1.0.1/single_instance_win.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: single-instance-win
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python module for creating a single instance of an application on Windows.
 Home-page: https://github.com/YuckyFox/432
 Author: YuckyFox
 Author-email: mr.cr.fox@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -27,15 +27,15 @@
 Whether developing a new application or improving an existing one, this module is an essential tool for any developer working with Python on the Windows operating system.
 
 Installation
 -----
 
 ```If you want to use the SingleInstance module in your Python application, you can easily install it via pip:
 
-**pip install singleinstance**
+pip install singleinstance
 
 This will download and install the SingleInstance module and any dependencies it requires, making it available for use in your Python application.
 ```
 
 Usage
 -----
```

