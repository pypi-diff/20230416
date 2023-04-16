# Comparing `tmp/sloslsoododldl-sosoajajk-1.tar.gz` & `tmp/sloslsoododldl-sosoajajk-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sloslsoododldl-sosoajajk-1.tar", last modified: Sun Apr 16 07:55:31 2023, max compression
+gzip compressed data, was "sloslsoododldl-sosoajajk-2.tar", last modified: Sun Apr 16 07:56:57 2023, max compression
```

## Comparing `sloslsoododldl-sosoajajk-1.tar` & `sloslsoododldl-sosoajajk-2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 07:55:31.623436 sloslsoododldl-sosoajajk-1/
--rw-rw-rw-   0        0        0     1052 2023-04-16 06:20:23.000000 sloslsoododldl-sosoajajk-1/LICENSE
--rw-rw-rw-   0        0        0       26 2019-08-27 18:29:08.000000 sloslsoododldl-sosoajajk-1/MANIFEST.in
--rw-rw-rw-   0        0        0     3145 2023-04-16 07:55:31.623436 sloslsoododldl-sosoajajk-1/PKG-INFO
--rw-rw-rw-   0        0        0     2282 2023-04-16 07:45:49.000000 sloslsoododldl-sosoajajk-1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-16 07:55:31.624757 sloslsoododldl-sosoajajk-1/setup.cfg
--rw-rw-rw-   0        0        0     2208 2023-04-16 07:53:30.000000 sloslsoododldl-sosoajajk-1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:55:31.617430 sloslsoododldl-sosoajajk-1/sloslsoododldl-sosoajajk/
--rw-rw-rw-   0        0        0       20 2019-08-27 18:29:08.000000 sloslsoododldl-sosoajajk-1/sloslsoododldl-sosoajajk/__init__.py
--rw-rw-rw-   0        0        0       26 2019-08-27 18:29:08.000000 sloslsoododldl-sosoajajk-1/sloslsoododldl-sosoajajk/core.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:55:31.622435 sloslsoododldl-sosoajajk-1/sloslsoododldl_sosoajajk.egg-info/
--rw-rw-rw-   0        0        0     3145 2023-04-16 07:55:31.000000 sloslsoododldl-sosoajajk-1/sloslsoododldl_sosoajajk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-04-16 07:55:31.000000 sloslsoododldl-sosoajajk-1/sloslsoododldl_sosoajajk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 07:55:31.000000 sloslsoododldl-sosoajajk-1/sloslsoododldl_sosoajajk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-16 07:55:31.000000 sloslsoododldl-sosoajajk-1/sloslsoododldl_sosoajajk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-04-16 07:55:31.000000 sloslsoododldl-sosoajajk-1/sloslsoododldl_sosoajajk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 07:56:57.760291 sloslsoododldl-sosoajajk-2/
+-rw-rw-rw-   0        0        0     1052 2023-04-16 06:20:23.000000 sloslsoododldl-sosoajajk-2/LICENSE
+-rw-rw-rw-   0        0        0       26 2019-08-27 18:29:08.000000 sloslsoododldl-sosoajajk-2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3145 2023-04-16 07:56:57.760291 sloslsoododldl-sosoajajk-2/PKG-INFO
+-rw-rw-rw-   0        0        0     2282 2023-04-16 07:45:49.000000 sloslsoododldl-sosoajajk-2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-16 07:56:57.761293 sloslsoododldl-sosoajajk-2/setup.cfg
+-rw-rw-rw-   0        0        0     2208 2023-04-16 07:56:39.000000 sloslsoododldl-sosoajajk-2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 07:56:57.754282 sloslsoododldl-sosoajajk-2/sloslsoododldl-sosoajajk/
+-rw-rw-rw-   0        0        0       20 2019-08-27 18:29:08.000000 sloslsoododldl-sosoajajk-2/sloslsoododldl-sosoajajk/__init__.py
+-rw-rw-rw-   0        0        0      787 2023-04-16 07:56:21.000000 sloslsoododldl-sosoajajk-2/sloslsoododldl-sosoajajk/core.py
+drwxrwxrwx   0        0        0        0 2023-04-16 07:56:57.759290 sloslsoododldl-sosoajajk-2/sloslsoododldl_sosoajajk.egg-info/
+-rw-rw-rw-   0        0        0     3145 2023-04-16 07:56:57.000000 sloslsoododldl-sosoajajk-2/sloslsoododldl_sosoajajk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2023-04-16 07:56:57.000000 sloslsoododldl-sosoajajk-2/sloslsoododldl_sosoajajk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 07:56:57.000000 sloslsoododldl-sosoajajk-2/sloslsoododldl_sosoajajk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-16 07:56:57.000000 sloslsoododldl-sosoajajk-2/sloslsoododldl_sosoajajk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-04-16 07:56:57.000000 sloslsoododldl-sosoajajk-2/sloslsoododldl_sosoajajk.egg-info/top_level.txt
```

### Comparing `sloslsoododldl-sosoajajk-1/LICENSE` & `sloslsoododldl-sosoajajk-2/LICENSE`

 * *Files identical despite different names*

### Comparing `sloslsoododldl-sosoajajk-1/PKG-INFO` & `sloslsoododldl-sosoajajk-2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sloslsoododldl-sosoajajk
-Version: 1
+Version: 2
 Summary: A Python module for creating a single instance of an application on Windows.
 Home-page: https://github.com/YuckyFox/432
 Author: YuckyFox
 Author-email: mr.cr.fox@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `sloslsoododldl-sosoajajk-1/README.md` & `sloslsoododldl-sosoajajk-2/README.md`

 * *Files identical despite different names*

### Comparing `sloslsoododldl-sosoajajk-1/setup.py` & `sloslsoododldl-sosoajajk-2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import io
 import os
 from shutil import rmtree
 from setuptools import find_packages, setup
 
 # Package meta-data.
 NAME = 'sloslsoododldl-sosoajajk'
-VERSION = '1'
+VERSION = '2'
 DESCRIPTION = 'A Python module for creating a single instance of an application on Windows.'
 URL = 'https://github.com/YuckyFox/432'
 AUTHOR = 'YuckyFox'
 EMAIL = 'mr.cr.fox@gmail.com'
 REQUIRES_PYTHON = '>=3.7.0'
 
 # What packages are required for this module to be executed?
```

### Comparing `sloslsoododldl-sosoajajk-1/sloslsoododldl_sosoajajk.egg-info/PKG-INFO` & `sloslsoododldl-sosoajajk-2/sloslsoododldl_sosoajajk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sloslsoododldl-sosoajajk
-Version: 1
+Version: 2
 Summary: A Python module for creating a single instance of an application on Windows.
 Home-page: https://github.com/YuckyFox/432
 Author: YuckyFox
 Author-email: mr.cr.fox@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

