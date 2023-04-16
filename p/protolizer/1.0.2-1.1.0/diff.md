# Comparing `tmp/protolizer-1.0.2.tar.gz` & `tmp/protolizer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protolizer-1.0.2.tar", last modified: Wed Aug 10 12:56:02 2022, max compression
+gzip compressed data, was "protolizer-1.1.0.tar", last modified: Sun Apr 16 09:28:29 2023, max compression
```

## Comparing `protolizer-1.0.2.tar` & `protolizer-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2022-08-10 12:56:02.702786 protolizer-1.0.2/
--rw-r--r--   0 hydra     (1000) hydra     (1000)     2072 2022-08-10 12:56:02.702786 protolizer-1.0.2/PKG-INFO
--rwxr-xr-x   0 hydra     (1000) hydra     (1000)     1658 2022-08-09 09:35:01.000000 protolizer-1.0.2/README.md
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2022-08-10 12:56:02.702786 protolizer-1.0.2/protolizer/
--rwxr-xr-x   0 hydra     (1000) hydra     (1000)      104 2022-08-09 07:15:52.000000 protolizer-1.0.2/protolizer/__init__.py
--rwxr-xr-x   0 hydra     (1000) hydra     (1000)      326 2022-08-09 09:42:57.000000 protolizer-1.0.2/protolizer/exceptions.py
--rwxr-xr-x   0 hydra     (1000) hydra     (1000)    17020 2022-08-10 12:53:12.000000 protolizer-1.0.2/protolizer/fields.py
--rwxr-xr-x   0 hydra     (1000) hydra     (1000)     4890 2022-08-09 07:22:07.000000 protolizer-1.0.2/protolizer/helpers.py
--rwxr-xr-x   0 hydra     (1000) hydra     (1000)     1494 2022-08-09 07:17:44.000000 protolizer-1.0.2/protolizer/meta.py
--rwxr-xr-x   0 hydra     (1000) hydra     (1000)    12633 2022-08-09 12:08:32.000000 protolizer-1.0.2/protolizer/serializer.py
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2022-08-10 12:56:02.702786 protolizer-1.0.2/protolizer.egg-info/
--rw-r--r--   0 hydra     (1000) hydra     (1000)     2072 2022-08-10 12:56:02.000000 protolizer-1.0.2/protolizer.egg-info/PKG-INFO
--rw-r--r--   0 hydra     (1000) hydra     (1000)      506 2022-08-10 12:56:02.000000 protolizer-1.0.2/protolizer.egg-info/SOURCES.txt
--rw-r--r--   0 hydra     (1000) hydra     (1000)        1 2022-08-10 12:56:02.000000 protolizer-1.0.2/protolizer.egg-info/dependency_links.txt
--rw-r--r--   0 hydra     (1000) hydra     (1000)       17 2022-08-10 12:56:02.000000 protolizer-1.0.2/protolizer.egg-info/top_level.txt
--rw-r--r--   0 hydra     (1000) hydra     (1000)       38 2022-08-10 12:56:02.702786 protolizer-1.0.2/setup.cfg
--rwxr-xr-x   0 hydra     (1000) hydra     (1000)      727 2022-08-10 12:53:12.000000 protolizer-1.0.2/setup.py
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2022-08-10 12:56:02.702786 protolizer-1.0.2/tests/
--rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-08-09 07:25:39.000000 protolizer-1.0.2/tests/__init__.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)      863 2022-08-09 09:49:42.000000 protolizer-1.0.2/tests/test_custom_response.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     6316 2022-08-10 12:53:12.000000 protolizer-1.0.2/tests/test_fields.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     1092 2022-08-09 11:48:19.000000 protolizer-1.0.2/tests/test_json_to_protobuf.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     1429 2022-08-09 12:07:09.000000 protolizer-1.0.2/tests/test_nested_fields.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)      847 2022-08-09 08:03:49.000000 protolizer-1.0.2/tests/test_pre_serialize_hook.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     1128 2022-08-09 12:43:51.000000 protolizer-1.0.2/tests/test_protobuf_to_json.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     1570 2022-08-09 09:28:25.000000 protolizer-1.0.2/tests/test_validation.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:28:29.257264 protolizer-1.1.0/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     2044 2023-04-16 09:28:29.257264 protolizer-1.1.0/PKG-INFO
+-rwxr-xr-x   0 hydra     (1000) hydra     (1000)     1658 2022-08-09 09:35:01.000000 protolizer-1.1.0/README.md
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:28:29.253931 protolizer-1.1.0/protolizer/
+-rwxr-xr-x   0 hydra     (1000) hydra     (1000)      104 2022-08-09 07:15:52.000000 protolizer-1.1.0/protolizer/__init__.py
+-rwxr-xr-x   0 hydra     (1000) hydra     (1000)      326 2022-08-09 09:42:57.000000 protolizer-1.1.0/protolizer/exceptions.py
+-rwxr-xr-x   0 hydra     (1000) hydra     (1000)    17020 2023-04-16 09:17:30.000000 protolizer-1.1.0/protolizer/fields.py
+-rwxr-xr-x   0 hydra     (1000) hydra     (1000)     4890 2022-08-09 07:22:07.000000 protolizer-1.1.0/protolizer/helpers.py
+-rwxr-xr-x   0 hydra     (1000) hydra     (1000)     1494 2022-08-09 07:17:44.000000 protolizer-1.1.0/protolizer/meta.py
+-rwxr-xr-x   0 hydra     (1000) hydra     (1000)    12849 2023-04-16 09:26:44.000000 protolizer-1.1.0/protolizer/serializer.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:28:29.257264 protolizer-1.1.0/protolizer.egg-info/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     2044 2023-04-16 09:28:29.000000 protolizer-1.1.0/protolizer.egg-info/PKG-INFO
+-rw-r--r--   0 hydra     (1000) hydra     (1000)      506 2023-04-16 09:28:29.000000 protolizer-1.1.0/protolizer.egg-info/SOURCES.txt
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        1 2023-04-16 09:28:29.000000 protolizer-1.1.0/protolizer.egg-info/dependency_links.txt
+-rw-r--r--   0 hydra     (1000) hydra     (1000)       17 2023-04-16 09:28:29.000000 protolizer-1.1.0/protolizer.egg-info/top_level.txt
+-rw-r--r--   0 hydra     (1000) hydra     (1000)       38 2023-04-16 09:28:29.257264 protolizer-1.1.0/setup.cfg
+-rwxr-xr-x   0 hydra     (1000) hydra     (1000)      699 2023-04-16 09:27:15.000000 protolizer-1.1.0/setup.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:28:29.257264 protolizer-1.1.0/tests/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-08-09 07:25:39.000000 protolizer-1.1.0/tests/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)      863 2022-08-09 09:49:42.000000 protolizer-1.1.0/tests/test_custom_response.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     6316 2023-04-16 09:27:00.000000 protolizer-1.1.0/tests/test_fields.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     1092 2023-04-16 09:17:27.000000 protolizer-1.1.0/tests/test_json_to_protobuf.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     1429 2023-04-16 09:17:27.000000 protolizer-1.1.0/tests/test_nested_fields.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)      847 2022-08-09 08:03:49.000000 protolizer-1.1.0/tests/test_pre_serialize_hook.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     1128 2022-08-09 12:43:51.000000 protolizer-1.1.0/tests/test_protobuf_to_json.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     1570 2022-08-09 09:28:25.000000 protolizer-1.1.0/tests/test_validation.py
```

### Comparing `protolizer-1.0.2/PKG-INFO` & `protolizer-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: protolizer
-Version: 1.0.2
+Version: 1.1.0
 Summary: A simple library to serialize and deserialize protobuf messages
 Home-page: https://github.com/its0x4d/protolizer
 Author: MosyDev
 Author-email: mostafa.uwsgi@gmail.com
-License: GPLv3
+License: MIT
 Keywords: protobuf serialization deserialization
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
 # Protolizer Documentation
 
 ## Introduction
 Protolizer is a simple library to serialize and deserialize protobuf messages
```

### Comparing `protolizer-1.0.2/README.md` & `protolizer-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `protolizer-1.0.2/protolizer/fields.py` & `protolizer-1.1.0/protolizer/fields.py`

 * *Files identical despite different names*

### Comparing `protolizer-1.0.2/protolizer/helpers.py` & `protolizer-1.1.0/protolizer/helpers.py`

 * *Files identical despite different names*

### Comparing `protolizer-1.0.2/protolizer/meta.py` & `protolizer-1.1.0/protolizer/meta.py`

 * *Files identical despite different names*

### Comparing `protolizer-1.0.2/protolizer/serializer.py` & `protolizer-1.1.0/protolizer/serializer.py`

 * *Files 5% similar despite different names*

```diff
@@ -201,14 +201,18 @@
             return self.to_representation(self.initial_data)
         return []
 
     def to_internal_value(self, data):
         ret = []
         errors = []
         for item in data:
+            if self.child.context == 'self' and isinstance(self.parent.context, dict):
+                self.child.context = self.parent.context
+            else:
+                self.child.context = self.context
             try:
                 validated = self.child.run_validation(item)
             except ValidationError as exc:
                 errors.append(exc.detail)
             else:
                 ret.append(validated)
                 errors.append({})
```

### Comparing `protolizer-1.0.2/protolizer.egg-info/PKG-INFO` & `protolizer-1.1.0/protolizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: protolizer
-Version: 1.0.2
+Version: 1.1.0
 Summary: A simple library to serialize and deserialize protobuf messages
 Home-page: https://github.com/its0x4d/protolizer
 Author: MosyDev
 Author-email: mostafa.uwsgi@gmail.com
-License: GPLv3
+License: MIT
 Keywords: protobuf serialization deserialization
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 
 # Protolizer Documentation
 
 ## Introduction
 Protolizer is a simple library to serialize and deserialize protobuf messages
```

### Comparing `protolizer-1.0.2/setup.py` & `protolizer-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="protolizer",
-    version="1.0.2",
+    version="1.1.0",
     author='MosyDev',
     author_email='mostafa.uwsgi@gmail.com',
     description='A simple library to serialize and deserialize protobuf messages',
     url='https://github.com/its0x4d/protolizer',
     packages=setuptools.find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
-    license='GPLv3',
+    license='MIT',
     classifiers=[
-        'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
     ],
     keywords='protobuf serialization deserialization',
 )
```

### Comparing `protolizer-1.0.2/tests/test_custom_response.py` & `protolizer-1.1.0/tests/test_custom_response.py`

 * *Files identical despite different names*

### Comparing `protolizer-1.0.2/tests/test_fields.py` & `protolizer-1.1.0/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `protolizer-1.0.2/tests/test_json_to_protobuf.py` & `protolizer-1.1.0/tests/test_json_to_protobuf.py`

 * *Files identical despite different names*

### Comparing `protolizer-1.0.2/tests/test_nested_fields.py` & `protolizer-1.1.0/tests/test_nested_fields.py`

 * *Files identical despite different names*

### Comparing `protolizer-1.0.2/tests/test_pre_serialize_hook.py` & `protolizer-1.1.0/tests/test_pre_serialize_hook.py`

 * *Files identical despite different names*

### Comparing `protolizer-1.0.2/tests/test_protobuf_to_json.py` & `protolizer-1.1.0/tests/test_protobuf_to_json.py`

 * *Files identical despite different names*

### Comparing `protolizer-1.0.2/tests/test_validation.py` & `protolizer-1.1.0/tests/test_validation.py`

 * *Files identical despite different names*

