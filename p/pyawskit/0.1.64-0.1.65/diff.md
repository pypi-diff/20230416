# Comparing `tmp/pyawskit-0.1.64.tar.gz` & `tmp/pyawskit-0.1.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyawskit-0.1.64.tar", last modified: Sun Apr 16 17:14:14 2023, max compression
+gzip compressed data, was "pyawskit-0.1.65.tar", last modified: Sun Apr 16 18:11:51 2023, max compression
```

## Comparing `pyawskit-0.1.64.tar` & `pyawskit-0.1.65.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 17:14:14.971262 pyawskit-0.1.64/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-16 17:14:02.000000 pyawskit-0.1.64/LICENSE
--rw-r--r--   0 mark      (1000) mark      (1000)     1401 2023-04-16 17:14:14.971262 pyawskit-0.1.64/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      415 2023-04-16 17:14:02.000000 pyawskit-0.1.64/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 17:14:14.971262 pyawskit-0.1.64/pyawskit/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2016-11-03 02:32:24.000000 pyawskit-0.1.64/pyawskit/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3635 2020-11-21 23:57:10.000000 pyawskit-0.1.64/pyawskit/aws.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3371 2023-04-16 17:06:41.000000 pyawskit-0.1.64/pyawskit/aws_codeartifact_npm_env_config_code.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1859 2023-04-16 17:13:39.000000 pyawskit-0.1.64/pyawskit/aws_codeartifact_pip_env_config_code.py
--rw-r--r--   0 mark      (1000) mark      (1000)      722 2023-04-16 17:05:38.000000 pyawskit-0.1.64/pyawskit/aws_ecr_login_code.py
--rw-r--r--   0 mark      (1000) mark      (1000)     7604 2023-03-08 22:51:40.000000 pyawskit-0.1.64/pyawskit/common.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2286 2023-04-16 17:13:26.000000 pyawskit-0.1.64/pyawskit/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)    14917 2023-04-16 17:01:13.000000 pyawskit-0.1.64/pyawskit/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2847 2022-07-01 11:36:28.000000 pyawskit-0.1.64/pyawskit/os_utils.py
--rw-r--r--   0 mark      (1000) mark      (1000)      211 2023-04-16 17:14:02.000000 pyawskit-0.1.64/pyawskit/static.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3356 2022-07-01 11:39:13.000000 pyawskit-0.1.64/pyawskit/utils.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 17:14:14.971262 pyawskit-0.1.64/pyawskit.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1401 2023-04-16 17:14:14.000000 pyawskit-0.1.64/pyawskit.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      511 2023-04-16 17:14:14.000000 pyawskit-0.1.64/pyawskit.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-16 17:14:14.000000 pyawskit-0.1.64/pyawskit.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       48 2023-04-16 17:14:14.000000 pyawskit-0.1.64/pyawskit.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       80 2023-04-16 17:14:14.000000 pyawskit-0.1.64/pyawskit.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-04-16 17:14:14.000000 pyawskit-0.1.64/pyawskit.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-16 17:14:14.971262 pyawskit-0.1.64/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1730 2023-04-16 17:14:02.000000 pyawskit-0.1.64/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 18:11:51.738028 pyawskit-0.1.65/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1069 2023-04-16 18:11:34.000000 pyawskit-0.1.65/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     1401 2023-04-16 18:11:51.738028 pyawskit-0.1.65/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      415 2023-04-16 18:11:34.000000 pyawskit-0.1.65/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 18:11:51.738028 pyawskit-0.1.65/pyawskit/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2016-11-03 02:32:24.000000 pyawskit-0.1.65/pyawskit/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3635 2020-11-21 23:57:10.000000 pyawskit-0.1.65/pyawskit/aws.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3371 2023-04-16 17:06:41.000000 pyawskit-0.1.65/pyawskit/aws_codeartifact_npm_env_config_code.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1859 2023-04-16 17:13:39.000000 pyawskit-0.1.65/pyawskit/aws_codeartifact_pip_env_config_code.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      722 2023-04-16 17:05:38.000000 pyawskit-0.1.65/pyawskit/aws_ecr_login_code.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     7604 2023-03-08 22:51:40.000000 pyawskit-0.1.65/pyawskit/common.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2286 2023-04-16 17:13:26.000000 pyawskit-0.1.65/pyawskit/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)    14917 2023-04-16 17:01:13.000000 pyawskit-0.1.65/pyawskit/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2847 2022-07-01 11:36:28.000000 pyawskit-0.1.65/pyawskit/os_utils.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      211 2023-04-16 18:11:34.000000 pyawskit-0.1.65/pyawskit/static.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3356 2022-07-01 11:39:13.000000 pyawskit-0.1.65/pyawskit/utils.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-04-16 18:11:51.738028 pyawskit-0.1.65/pyawskit.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1401 2023-04-16 18:11:51.000000 pyawskit-0.1.65/pyawskit.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      511 2023-04-16 18:11:51.000000 pyawskit-0.1.65/pyawskit.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-04-16 18:11:51.000000 pyawskit-0.1.65/pyawskit.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       48 2023-04-16 18:11:51.000000 pyawskit-0.1.65/pyawskit.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       89 2023-04-16 18:11:51.000000 pyawskit-0.1.65/pyawskit.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        9 2023-04-16 18:11:51.000000 pyawskit-0.1.65/pyawskit.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2023-04-16 18:11:51.739028 pyawskit-0.1.65/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1750 2023-04-16 18:11:34.000000 pyawskit-0.1.65/setup.py
```

### Comparing `pyawskit-0.1.64/LICENSE` & `pyawskit-0.1.65/LICENSE`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.64/PKG-INFO` & `pyawskit-0.1.65/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyawskit
-Version: 0.1.64
+Version: 0.1.65
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
 
-version: 0.1.64
+version: 0.1.65
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pyawskit-0.1.64/pyawskit/aws.py` & `pyawskit-0.1.65/pyawskit/aws.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.64/pyawskit/aws_codeartifact_npm_env_config_code.py` & `pyawskit-0.1.65/pyawskit/aws_codeartifact_npm_env_config_code.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.64/pyawskit/aws_codeartifact_pip_env_config_code.py` & `pyawskit-0.1.65/pyawskit/aws_codeartifact_pip_env_config_code.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.64/pyawskit/aws_ecr_login_code.py` & `pyawskit-0.1.65/pyawskit/aws_ecr_login_code.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.64/pyawskit/common.py` & `pyawskit-0.1.65/pyawskit/common.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.64/pyawskit/configs.py` & `pyawskit-0.1.65/pyawskit/configs.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.64/pyawskit/main.py` & `pyawskit-0.1.65/pyawskit/main.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.64/pyawskit/os_utils.py` & `pyawskit-0.1.65/pyawskit/os_utils.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.64/pyawskit/utils.py` & `pyawskit-0.1.65/pyawskit/utils.py`

 * *Files identical despite different names*

### Comparing `pyawskit-0.1.64/pyawskit.egg-info/PKG-INFO` & `pyawskit-0.1.65/pyawskit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyawskit
-Version: 0.1.64
+Version: 0.1.65
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
 
-version: 0.1.64
+version: 0.1.65
 
 	Mark Veltzer <mark.veltzer@gmail.com>, Copyright © 2016, 2017, 2018, 2019, 2020, 2021, 2022, 2023
```

### Comparing `pyawskit-0.1.64/setup.py` & `pyawskit-0.1.65/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pyawskit",
-    version="0.1.64",
+    version="0.1.65",
     packages=[
         "pyawskit",
     ],
     # from here all is optional
     description="pyawskit is a collection of utilities to help interact with aws",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
@@ -42,14 +42,15 @@
         "tqdm",
         "requests",
         "boto3",
         "pymount",
         "ujson",
         "sultan",
         "pytconf",
+        "pyapikey",
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

