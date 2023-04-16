# Comparing `tmp/meta-person-3.4.16.tar.gz` & `tmp/meta-person-3.4.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/meta-person-3.4.16.tar", last modified: Sun Apr 16 07:34:28 2023, max compression
+gzip compressed data, was "dist/meta-person-3.4.17.tar", last modified: Sun Apr 16 08:07:29 2023, max compression
```

## Comparing `meta-person-3.4.16.tar` & `meta-person-3.4.17.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-16 07:34:28.000000 meta-person-3.4.16/
--rw-rw-r--   0 cash      (1000) cash      (1000)      281 2023-04-16 07:34:28.000000 meta-person-3.4.16/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)       35 2021-11-29 11:46:57.000000 meta-person-3.4.16/README.md
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-16 07:34:28.000000 meta-person-3.4.16/meta_person.egg-info/
--rw-rw-r--   0 cash      (1000) cash      (1000)      281 2023-04-16 07:34:28.000000 meta-person-3.4.16/meta_person.egg-info/PKG-INFO
--rw-rw-r--   0 cash      (1000) cash      (1000)      670 2023-04-16 07:34:28.000000 meta-person-3.4.16/meta_person.egg-info/SOURCES.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-04-16 07:34:28.000000 meta-person-3.4.16/meta_person.egg-info/dependency_links.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)       57 2023-04-16 07:34:28.000000 meta-person-3.4.16/meta_person.egg-info/requires.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)       11 2023-04-16 07:34:28.000000 meta-person-3.4.16/meta_person.egg-info/top_level.txt
--rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-04-16 07:34:28.000000 meta-person-3.4.16/meta_person.egg-info/zip-safe
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-16 07:34:28.000000 meta-person-3.4.16/metaperson/
--rw-rw-r--   0 cash      (1000) cash      (1000)       79 2023-04-16 07:19:12.000000 meta-person-3.4.16/metaperson/__init__.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-16 07:34:28.000000 meta-person-3.4.16/metaperson/app/
--rw-rw-r--   0 cash      (1000) cash      (1000)      183 2023-04-16 07:19:24.000000 meta-person-3.4.16/metaperson/app/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1798 2021-12-10 18:12:55.000000 meta-person-3.4.16/metaperson/app/onnx_to_trt.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     3565 2023-04-11 04:05:00.000000 meta-person-3.4.16/metaperson/app/person_detection_trt.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     3355 2023-04-10 07:31:05.000000 meta-person-3.4.16/metaperson/app/person_recognition_trt.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     4239 2023-04-11 05:47:00.000000 meta-person-3.4.16/metaperson/app/person_reid_trt.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-16 07:34:28.000000 meta-person-3.4.16/metaperson/model_zoo/
--rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-04-16 07:22:22.000000 meta-person-3.4.16/metaperson/model_zoo/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)      951 2021-12-04 09:05:10.000000 meta-person-3.4.16/metaperson/model_zoo/basetrack.py
--rw-rw-r--   0 cash      (1000) cash      (1000)    11898 2023-04-10 08:22:12.000000 meta-person-3.4.16/metaperson/model_zoo/byte_tracker.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     9500 2023-04-10 08:08:30.000000 meta-person-3.4.16/metaperson/model_zoo/kalman_filter.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     6134 2023-04-10 08:12:10.000000 meta-person-3.4.16/metaperson/model_zoo/matching.py
-drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-16 07:34:28.000000 meta-person-3.4.16/metaperson/utils/
--rw-rw-r--   0 cash      (1000) cash      (1000)       40 2023-04-16 07:18:35.000000 meta-person-3.4.16/metaperson/utils/__init__.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     3509 2023-04-16 07:30:41.000000 meta-person-3.4.16/metaperson/utils/boxes.py
--rw-rw-r--   0 cash      (1000) cash      (1000)     1371 2021-12-11 03:52:50.000000 meta-person-3.4.16/metaperson/utils/trt.py
--rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-04-16 07:34:28.000000 meta-person-3.4.16/setup.cfg
--rw-rw-r--   0 cash      (1000) cash      (1000)      699 2023-04-16 07:32:54.000000 meta-person-3.4.16/setup.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-16 08:07:29.000000 meta-person-3.4.17/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      281 2023-04-16 08:07:29.000000 meta-person-3.4.17/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)       35 2021-11-29 11:46:57.000000 meta-person-3.4.17/README.md
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-16 08:07:29.000000 meta-person-3.4.17/meta_person.egg-info/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      281 2023-04-16 08:07:29.000000 meta-person-3.4.17/meta_person.egg-info/PKG-INFO
+-rw-rw-r--   0 cash      (1000) cash      (1000)      670 2023-04-16 08:07:29.000000 meta-person-3.4.17/meta_person.egg-info/SOURCES.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-04-16 08:07:29.000000 meta-person-3.4.17/meta_person.egg-info/dependency_links.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)       57 2023-04-16 08:07:29.000000 meta-person-3.4.17/meta_person.egg-info/requires.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)       11 2023-04-16 08:07:29.000000 meta-person-3.4.17/meta_person.egg-info/top_level.txt
+-rw-rw-r--   0 cash      (1000) cash      (1000)        1 2023-04-16 07:34:28.000000 meta-person-3.4.17/meta_person.egg-info/zip-safe
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-16 08:07:29.000000 meta-person-3.4.17/metaperson/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       79 2023-04-16 07:19:12.000000 meta-person-3.4.17/metaperson/__init__.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-16 08:07:29.000000 meta-person-3.4.17/metaperson/app/
+-rw-rw-r--   0 cash      (1000) cash      (1000)      183 2023-04-16 07:19:24.000000 meta-person-3.4.17/metaperson/app/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1798 2021-12-10 18:12:55.000000 meta-person-3.4.17/metaperson/app/onnx_to_trt.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     3565 2023-04-11 04:05:00.000000 meta-person-3.4.17/metaperson/app/person_detection_trt.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     3355 2023-04-10 07:31:05.000000 meta-person-3.4.17/metaperson/app/person_recognition_trt.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     4239 2023-04-11 05:47:00.000000 meta-person-3.4.17/metaperson/app/person_reid_trt.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-16 08:07:29.000000 meta-person-3.4.17/metaperson/model_zoo/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-04-16 07:22:22.000000 meta-person-3.4.17/metaperson/model_zoo/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)      951 2021-12-04 09:05:10.000000 meta-person-3.4.17/metaperson/model_zoo/basetrack.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)    11898 2023-04-10 08:22:12.000000 meta-person-3.4.17/metaperson/model_zoo/byte_tracker.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     9500 2023-04-10 08:08:30.000000 meta-person-3.4.17/metaperson/model_zoo/kalman_filter.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     6134 2023-04-10 08:12:10.000000 meta-person-3.4.17/metaperson/model_zoo/matching.py
+drwxrwxr-x   0 cash      (1000) cash      (1000)        0 2023-04-16 08:07:29.000000 meta-person-3.4.17/metaperson/utils/
+-rw-rw-r--   0 cash      (1000) cash      (1000)       40 2023-04-16 07:18:35.000000 meta-person-3.4.17/metaperson/utils/__init__.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     3509 2023-04-16 07:30:41.000000 meta-person-3.4.17/metaperson/utils/boxes.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)     1371 2021-12-11 03:52:50.000000 meta-person-3.4.17/metaperson/utils/trt.py
+-rw-rw-r--   0 cash      (1000) cash      (1000)       38 2023-04-16 08:07:29.000000 meta-person-3.4.17/setup.cfg
+-rw-rw-r--   0 cash      (1000) cash      (1000)      699 2023-04-16 08:07:24.000000 meta-person-3.4.17/setup.py
```

### Comparing `meta-person-3.4.16/meta_person.egg-info/SOURCES.txt` & `meta-person-3.4.17/meta_person.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meta-person-3.4.16/metaperson/app/onnx_to_trt.py` & `meta-person-3.4.17/metaperson/app/onnx_to_trt.py`

 * *Files identical despite different names*

### Comparing `meta-person-3.4.16/metaperson/app/person_detection_trt.py` & `meta-person-3.4.17/metaperson/app/person_detection_trt.py`

 * *Files identical despite different names*

### Comparing `meta-person-3.4.16/metaperson/app/person_recognition_trt.py` & `meta-person-3.4.17/metaperson/app/person_recognition_trt.py`

 * *Files identical despite different names*

### Comparing `meta-person-3.4.16/metaperson/app/person_reid_trt.py` & `meta-person-3.4.17/metaperson/app/person_reid_trt.py`

 * *Files identical despite different names*

### Comparing `meta-person-3.4.16/metaperson/model_zoo/basetrack.py` & `meta-person-3.4.17/metaperson/model_zoo/basetrack.py`

 * *Files identical despite different names*

### Comparing `meta-person-3.4.16/metaperson/model_zoo/byte_tracker.py` & `meta-person-3.4.17/metaperson/model_zoo/byte_tracker.py`

 * *Files identical despite different names*

### Comparing `meta-person-3.4.16/metaperson/model_zoo/kalman_filter.py` & `meta-person-3.4.17/metaperson/model_zoo/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `meta-person-3.4.16/metaperson/model_zoo/matching.py` & `meta-person-3.4.17/metaperson/model_zoo/matching.py`

 * *Files identical despite different names*

### Comparing `meta-person-3.4.16/metaperson/utils/boxes.py` & `meta-person-3.4.17/metaperson/utils/boxes.py`

 * *Files identical despite different names*

### Comparing `meta-person-3.4.16/metaperson/utils/trt.py` & `meta-person-3.4.17/metaperson/utils/trt.py`

 * *Files identical despite different names*

### Comparing `meta-person-3.4.16/setup.py` & `meta-person-3.4.17/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     'tensorrt',
     'numpy',
     'pycuda',
     'scipy',
     'lap',
 ]
 
-__version__ = 'V3.04.16'
+__version__ = 'V3.04.17'
 
 setup(
     name='meta-person',
     version=__version__,
     author='CachCheng',
     author_email='tkggpdc2007@163.com',
     url='https://github.com/CachCheng/cvtrack',
```

