# Comparing `tmp/georise-0.0.1.tar.gz` & `tmp/georise-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "georise-0.0.1.tar", last modified: Sat Apr 15 19:00:02 2023, max compression
+gzip compressed data, was "georise-0.0.2.tar", last modified: Sun Apr 16 21:04:26 2023, max compression
```

## Comparing `georise-0.0.1.tar` & `georise-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 quothbonney  (1000) quothbonney  (1000)        0 2023-04-15 19:00:02.780758 georise-0.0.1/
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)      710 2023-04-15 19:00:02.780758 georise-0.0.1/PKG-INFO
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)       10 2023-04-15 18:56:19.000000 georise-0.0.1/README.md
-drwxrwxr-x   0 quothbonney  (1000) quothbonney  (1000)        0 2023-04-15 19:00:02.780758 georise-0.0.1/georise/
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)        0 2023-04-13 06:22:06.000000 georise-0.0.1/georise/__init__.py
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)       63 2023-04-12 23:48:00.000000 georise-0.0.1/georise/constants.py
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)     5147 2023-04-11 20:01:17.000000 georise-0.0.1/georise/glview.py
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)      956 2023-04-13 04:57:45.000000 georise-0.0.1/georise/overlay.py
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)     2558 2023-04-15 17:46:15.000000 georise-0.0.1/georise/provider.py
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)     2960 2023-04-15 17:46:17.000000 georise-0.0.1/georise/raster.py
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)     4556 2023-04-15 17:54:39.000000 georise-0.0.1/georise/scene.py
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)     3376 2023-04-15 05:09:08.000000 georise-0.0.1/georise/transform.py
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)      822 2023-04-08 19:16:20.000000 georise-0.0.1/georise/util.py
-drwxrwxr-x   0 quothbonney  (1000) quothbonney  (1000)        0 2023-04-15 19:00:02.780758 georise-0.0.1/georise.egg-info/
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)      710 2023-04-15 19:00:02.000000 georise-0.0.1/georise.egg-info/PKG-INFO
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)      428 2023-04-15 19:00:02.000000 georise-0.0.1/georise.egg-info/SOURCES.txt
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)        1 2023-04-15 19:00:02.000000 georise-0.0.1/georise.egg-info/dependency_links.txt
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)      191 2023-04-15 19:00:02.000000 georise-0.0.1/georise.egg-info/requires.txt
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)       14 2023-04-15 19:00:02.000000 georise-0.0.1/georise.egg-info/top_level.txt
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)       38 2023-04-15 19:00:02.780758 georise-0.0.1/setup.cfg
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)     1126 2023-04-15 18:59:59.000000 georise-0.0.1/setup.py
-drwxrwxr-x   0 quothbonney  (1000) quothbonney  (1000)        0 2023-04-15 19:00:02.780758 georise-0.0.1/tests/
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)        0 2023-04-15 15:05:59.000000 georise-0.0.1/tests/__init__.py
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)     1837 2023-04-15 17:31:59.000000 georise-0.0.1/tests/test_provider.py
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)     1915 2023-04-15 15:10:23.000000 georise-0.0.1/tests/test_raster.py
--rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)     2203 2023-04-15 15:11:20.000000 georise-0.0.1/tests/test_transform.py
+drwxrwxr-x   0 quothbonney  (1000) quothbonney  (1000)        0 2023-04-16 21:04:26.990199 georise-0.0.2/
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)      710 2023-04-16 21:04:26.990199 georise-0.0.2/PKG-INFO
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)       10 2023-04-15 18:56:19.000000 georise-0.0.2/README.md
+drwxrwxr-x   0 quothbonney  (1000) quothbonney  (1000)        0 2023-04-16 21:04:26.990199 georise-0.0.2/georise/
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)        0 2023-04-13 06:22:06.000000 georise-0.0.2/georise/__init__.py
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)       63 2023-04-12 23:48:00.000000 georise-0.0.2/georise/constants.py
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)     5147 2023-04-11 20:01:17.000000 georise-0.0.2/georise/glview.py
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)      956 2023-04-13 04:57:45.000000 georise-0.0.2/georise/overlay.py
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)     2558 2023-04-15 17:46:15.000000 georise-0.0.2/georise/provider.py
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)     2960 2023-04-15 17:46:17.000000 georise-0.0.2/georise/raster.py
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)     4556 2023-04-15 17:54:39.000000 georise-0.0.2/georise/scene.py
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)     3376 2023-04-15 05:09:08.000000 georise-0.0.2/georise/transform.py
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)      822 2023-04-08 19:16:20.000000 georise-0.0.2/georise/util.py
+drwxrwxr-x   0 quothbonney  (1000) quothbonney  (1000)        0 2023-04-16 21:04:26.990199 georise-0.0.2/georise.egg-info/
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)      710 2023-04-16 21:04:26.000000 georise-0.0.2/georise.egg-info/PKG-INFO
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)      428 2023-04-16 21:04:26.000000 georise-0.0.2/georise.egg-info/SOURCES.txt
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)        1 2023-04-16 21:04:26.000000 georise-0.0.2/georise.egg-info/dependency_links.txt
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)      131 2023-04-16 21:04:26.000000 georise-0.0.2/georise.egg-info/requires.txt
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)       14 2023-04-16 21:04:26.000000 georise-0.0.2/georise.egg-info/top_level.txt
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)       38 2023-04-16 21:04:26.990199 georise-0.0.2/setup.cfg
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)     1022 2023-04-16 21:02:51.000000 georise-0.0.2/setup.py
+drwxrwxr-x   0 quothbonney  (1000) quothbonney  (1000)        0 2023-04-16 21:04:26.990199 georise-0.0.2/tests/
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)        0 2023-04-15 15:05:59.000000 georise-0.0.2/tests/__init__.py
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)     1837 2023-04-15 17:31:59.000000 georise-0.0.2/tests/test_provider.py
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)     1915 2023-04-15 15:10:23.000000 georise-0.0.2/tests/test_raster.py
+-rw-rw-r--   0 quothbonney  (1000) quothbonney  (1000)     2203 2023-04-15 15:11:20.000000 georise-0.0.2/tests/test_transform.py
```

### Comparing `georise-0.0.1/PKG-INFO` & `georise-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: georise
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python Library Built on GDAL for Visualization of Geospatial Maps
 Home-page: https://github.com/quothbonney/georise
 Author: Jack David Carson
 Author-email: jackdavidcarson@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `georise-0.0.1/georise/glview.py` & `georise-0.0.2/georise/glview.py`

 * *Files identical despite different names*

### Comparing `georise-0.0.1/georise/overlay.py` & `georise-0.0.2/georise/overlay.py`

 * *Files identical despite different names*

### Comparing `georise-0.0.1/georise/provider.py` & `georise-0.0.2/georise/provider.py`

 * *Files identical despite different names*

### Comparing `georise-0.0.1/georise/raster.py` & `georise-0.0.2/georise/raster.py`

 * *Files identical despite different names*

### Comparing `georise-0.0.1/georise/scene.py` & `georise-0.0.2/georise/scene.py`

 * *Files identical despite different names*

### Comparing `georise-0.0.1/georise/transform.py` & `georise-0.0.2/georise/transform.py`

 * *Files identical despite different names*

### Comparing `georise-0.0.1/georise/util.py` & `georise-0.0.2/georise/util.py`

 * *Files identical despite different names*

### Comparing `georise-0.0.1/georise.egg-info/PKG-INFO` & `georise-0.0.2/georise.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: georise
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python Library Built on GDAL for Visualization of Geospatial Maps
 Home-page: https://github.com/quothbonney/georise
 Author: Jack David Carson
 Author-email: jackdavidcarson@gmail.com
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `georise-0.0.1/setup.py` & `georise-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="georise",
-    version="0.0.1",
+    version="0.0.2",
     author='Jack David Carson',
     author_email='jackdavidcarson@gmail.com',
     description='A Python Library Built on GDAL for Visualization of Geospatial Maps',
     url='https://github.com/quothbonney/georise',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
@@ -19,19 +19,15 @@
         'Programming Language :: Python :: 3.9',
     ],
     install_requires=[
         'geopy==2.3.0',
         'matplotlib==3.4.3',
         'numpy==1.24.2',
         'numpy==1.17.4',
-        'osgeo==0.0.1',
-        'PyQt5==5.15.9',
-        'PyQt5_sip==12.11.1',
         'pyqtgraph==0.13.1',
-        'pytest==7.3.0',
         'rasterio==1.3.6',
         'setuptools==44.0.0',
         'setuptools==45.2.0'
     ],
     python_requires='>=3.6',
 )
```

### Comparing `georise-0.0.1/tests/test_provider.py` & `georise-0.0.2/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `georise-0.0.1/tests/test_raster.py` & `georise-0.0.2/tests/test_raster.py`

 * *Files identical despite different names*

### Comparing `georise-0.0.1/tests/test_transform.py` & `georise-0.0.2/tests/test_transform.py`

 * *Files identical despite different names*

