# Comparing `tmp/pyawskit-0.1.61.tar.gz` & `tmp/pyawskit-0.1.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyawskit-0.1.61.tar", last modified: Sun Apr 16 13:56:00 2023, max compression
+gzip compressed data, was "pyawskit-0.1.62.tar", last modified: Sun Apr 16 14:02:43 2023, max compression
```

## Comparing `pyawskit-0.1.61.tar` & `pyawskit-0.1.62.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 13:56:00.683488 pyawskit-0.1.61/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-16 13:55:50.000000 pyawskit-0.1.61/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)     1401 2023-04-16 13:56:00.683488 pyawskit-0.1.61/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      415 2023-04-16 13:55:50.000000 pyawskit-0.1.61/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 13:56:00.683488 pyawskit-0.1.61/pyawskit/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2016-11-03 02:32:24.000000 pyawskit-0.1.61/pyawskit/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3635 2020-11-21 23:57:10.000000 pyawskit-0.1.61/pyawskit/aws.py
--rw-r--r--   0 mark      (1000) mark      (1000)     7604 2023-03-08 22:51:40.000000 pyawskit-0.1.61/pyawskit/common.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1058 2021-09-08 16:57:25.000000 pyawskit-0.1.61/pyawskit/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)    14050 2023-04-16 13:55:36.000000 pyawskit-0.1.61/pyawskit/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2847 2022-07-01 11:36:28.000000 pyawskit-0.1.61/pyawskit/os_utils.py
--rw-r--r--   0 mark      (1000) mark      (1000)      211 2023-04-16 13:55:50.000000 pyawskit-0.1.61/pyawskit/static.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3356 2022-07-01 11:39:13.000000 pyawskit-0.1.61/pyawskit/utils.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 13:56:00.683488 pyawskit-0.1.61/pyawskit.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1401 2023-04-16 13:56:00.000000 pyawskit-0.1.61/pyawskit.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      382 2023-04-16 13:56:00.000000 pyawskit-0.1.61/pyawskit.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-16 13:56:00.000000 pyawskit-0.1.61/pyawskit.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       48 2023-04-16 13:56:00.000000 pyawskit-0.1.61/pyawskit.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       80 2023-04-16 13:56:00.000000 pyawskit-0.1.61/pyawskit.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-04-16 13:56:00.000000 pyawskit-0.1.61/pyawskit.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-16 13:56:00.684488 pyawskit-0.1.61/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1730 2023-04-16 13:55:50.000000 pyawskit-0.1.61/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 14:02:43.643594 pyawskit-0.1.62/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-16 14:02:30.000000 pyawskit-0.1.62/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1401 2023-04-16 14:02:43.643594 pyawskit-0.1.62/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      415 2023-04-16 14:02:30.000000 pyawskit-0.1.62/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 14:02:43.642594 pyawskit-0.1.62/pyawskit/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2016-11-03 02:32:24.000000 pyawskit-0.1.62/pyawskit/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3635 2020-11-21 23:57:10.000000 pyawskit-0.1.62/pyawskit/aws.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     7604 2023-03-08 22:51:40.000000 pyawskit-0.1.62/pyawskit/common.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1519 2023-04-16 14:02:10.000000 pyawskit-0.1.62/pyawskit/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)    14050 2023-04-16 13:55:36.000000 pyawskit-0.1.62/pyawskit/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2847 2022-07-01 11:36:28.000000 pyawskit-0.1.62/pyawskit/os_utils.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      211 2023-04-16 14:02:30.000000 pyawskit-0.1.62/pyawskit/static.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3356 2022-07-01 11:39:13.000000 pyawskit-0.1.62/pyawskit/utils.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 14:02:43.643594 pyawskit-0.1.62/pyawskit.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1401 2023-04-16 14:02:43.000000 pyawskit-0.1.62/pyawskit.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      382 2023-04-16 14:02:43.000000 pyawskit-0.1.62/pyawskit.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-16 14:02:43.000000 pyawskit-0.1.62/pyawskit.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       48 2023-04-16 14:02:43.000000 pyawskit-0.1.62/pyawskit.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       80 2023-04-16 14:02:43.000000 pyawskit-0.1.62/pyawskit.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-04-16 14:02:43.000000 pyawskit-0.1.62/pyawskit.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-16 14:02:43.643594 pyawskit-0.1.62/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1730 2023-04-16 14:02:30.000000 pyawskit-0.1.62/setup.py
```

### Comparing `pyawskit-0.1.61/LICENSE` & `pyawskit-0.1.62/LICENSE`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.61/PKG-INFO` & `pyawskit-0.1.62/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyawskit
-Version: 0.1.61
+Version: 0.1.62
 Summary: pyawskit is a collection of utilities to help interact with aws
 Home-page: https://veltzer.github.io/pyawskit
 Download-URL: https://github.com/veltzer/pyawskit
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pyawskit
 
 author: Mark Veltzer
 
-version: 0.1.61
+version: 0.1.62
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pyawskit-0.1.61/pyawskit/aws.py` & `pyawskit-0.1.62/pyawskit/aws.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.61/pyawskit/common.py` & `pyawskit-0.1.62/pyawskit/common.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.61/pyawskit/main.py` & `pyawskit-0.1.62/pyawskit/main.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.61/pyawskit/os_utils.py` & `pyawskit-0.1.62/pyawskit/os_utils.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.61/pyawskit/utils.py` & `pyawskit-0.1.62/pyawskit/utils.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.61/pyawskit.egg-info/PKG-INFO` & `pyawskit-0.1.62/pyawskit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyawskit
-Version: 0.1.61
+Version: 0.1.62
 Summary: pyawskit is a collection of utilities to help interact with aws
 Home-page: https://veltzer.github.io/pyawskit
 Download-URL: https://github.com/veltzer/pyawskit
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
@@ -35,10 +35,10 @@
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
 
 project website: https://veltzer.github.io/pyawskit
 
 author: Mark Veltzer
 
-version: 0.1.61
+version: 0.1.62
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pyawskit-0.1.61/setup.py` & `pyawskit-0.1.62/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pyawskit",
-    version="0.1.61",
+    version="0.1.62",
     packages=[
         "pyawskit",
     ],
     # from here all is optional
     description="pyawskit is a collection of utilities to help interact with aws",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
```

