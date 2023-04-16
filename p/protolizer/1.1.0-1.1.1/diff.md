# Comparing `tmp/protolizer-1.1.0.tar.gz` & `tmp/protolizer-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protolizer-1.1.0.tar", last modified: Sun Apr 16 09:28:29 2023, max compression
+gzip compressed data, was "protolizer-1.1.1.tar", last modified: Sun Apr 16 09:47:57 2023, max compression
```

## Comparing `protolizer-1.1.0.tar` & `protolizer-1.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:28:29.257264 protolizer-1.1.0/
--rw-r--r--   0 hydra     (1000) hydra     (1000)     2044 2023-04-16 09:28:29.257264 protolizer-1.1.0/PKG-INFO
--rwxr-xr-x   0 hydra     (1000) hydra     (1000)     1658 2022-08-09 09:35:01.000000 protolizer-1.1.0/README.md
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:28:29.253931 protolizer-1.1.0/protolizer/
--rwxr-xr-x   0 hydra     (1000) hydra     (1000)      104 2022-08-09 07:15:52.000000 protolizer-1.1.0/protolizer/__init__.py
--rwxr-xr-x   0 hydra     (1000) hydra     (1000)      326 2022-08-09 09:42:57.000000 protolizer-1.1.0/protolizer/exceptions.py
--rwxr-xr-x   0 hydra     (1000) hydra     (1000)    17020 2023-04-16 09:17:30.000000 protolizer-1.1.0/protolizer/fields.py
--rwxr-xr-x   0 hydra     (1000) hydra     (1000)     4890 2022-08-09 07:22:07.000000 protolizer-1.1.0/protolizer/helpers.py
--rwxr-xr-x   0 hydra     (1000) hydra     (1000)     1494 2022-08-09 07:17:44.000000 protolizer-1.1.0/protolizer/meta.py
--rwxr-xr-x   0 hydra     (1000) hydra     (1000)    12849 2023-04-16 09:26:44.000000 protolizer-1.1.0/protolizer/serializer.py
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:28:29.257264 protolizer-1.1.0/protolizer.egg-info/
--rw-r--r--   0 hydra     (1000) hydra     (1000)     2044 2023-04-16 09:28:29.000000 protolizer-1.1.0/protolizer.egg-info/PKG-INFO
--rw-r--r--   0 hydra     (1000) hydra     (1000)      506 2023-04-16 09:28:29.000000 protolizer-1.1.0/protolizer.egg-info/SOURCES.txt
--rw-r--r--   0 hydra     (1000) hydra     (1000)        1 2023-04-16 09:28:29.000000 protolizer-1.1.0/protolizer.egg-info/dependency_links.txt
--rw-r--r--   0 hydra     (1000) hydra     (1000)       17 2023-04-16 09:28:29.000000 protolizer-1.1.0/protolizer.egg-info/top_level.txt
--rw-r--r--   0 hydra     (1000) hydra     (1000)       38 2023-04-16 09:28:29.257264 protolizer-1.1.0/setup.cfg
--rwxr-xr-x   0 hydra     (1000) hydra     (1000)      699 2023-04-16 09:27:15.000000 protolizer-1.1.0/setup.py
-drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:28:29.257264 protolizer-1.1.0/tests/
--rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-08-09 07:25:39.000000 protolizer-1.1.0/tests/__init__.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)      863 2022-08-09 09:49:42.000000 protolizer-1.1.0/tests/test_custom_response.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     6316 2023-04-16 09:27:00.000000 protolizer-1.1.0/tests/test_fields.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     1092 2023-04-16 09:17:27.000000 protolizer-1.1.0/tests/test_json_to_protobuf.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     1429 2023-04-16 09:17:27.000000 protolizer-1.1.0/tests/test_nested_fields.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)      847 2022-08-09 08:03:49.000000 protolizer-1.1.0/tests/test_pre_serialize_hook.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     1128 2022-08-09 12:43:51.000000 protolizer-1.1.0/tests/test_protobuf_to_json.py
--rw-r--r--   0 hydra     (1000) hydra     (1000)     1570 2022-08-09 09:28:25.000000 protolizer-1.1.0/tests/test_validation.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:47:57.224280 protolizer-1.1.1/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     2044 2023-04-16 09:47:57.224280 protolizer-1.1.1/PKG-INFO
+-rwxr-xr-x   0 hydra     (1000) hydra     (1000)     1658 2022-08-09 09:35:01.000000 protolizer-1.1.1/README.md
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:47:57.220947 protolizer-1.1.1/protolizer/
+-rwxr-xr-x   0 hydra     (1000) hydra     (1000)      104 2022-08-09 07:15:52.000000 protolizer-1.1.1/protolizer/__init__.py
+-rwxr-xr-x   0 hydra     (1000) hydra     (1000)      326 2022-08-09 09:42:57.000000 protolizer-1.1.1/protolizer/exceptions.py
+-rwxr-xr-x   0 hydra     (1000) hydra     (1000)    17020 2023-04-16 09:17:30.000000 protolizer-1.1.1/protolizer/fields.py
+-rwxr-xr-x   0 hydra     (1000) hydra     (1000)     4890 2022-08-09 07:22:07.000000 protolizer-1.1.1/protolizer/helpers.py
+-rwxr-xr-x   0 hydra     (1000) hydra     (1000)     1494 2022-08-09 07:17:44.000000 protolizer-1.1.1/protolizer/meta.py
+-rwxr-xr-x   0 hydra     (1000) hydra     (1000)    13049 2023-04-16 09:47:21.000000 protolizer-1.1.1/protolizer/serializer.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:47:57.224280 protolizer-1.1.1/protolizer.egg-info/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     2044 2023-04-16 09:47:57.000000 protolizer-1.1.1/protolizer.egg-info/PKG-INFO
+-rw-r--r--   0 hydra     (1000) hydra     (1000)      506 2023-04-16 09:47:57.000000 protolizer-1.1.1/protolizer.egg-info/SOURCES.txt
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        1 2023-04-16 09:47:57.000000 protolizer-1.1.1/protolizer.egg-info/dependency_links.txt
+-rw-r--r--   0 hydra     (1000) hydra     (1000)       17 2023-04-16 09:47:57.000000 protolizer-1.1.1/protolizer.egg-info/top_level.txt
+-rw-r--r--   0 hydra     (1000) hydra     (1000)       38 2023-04-16 09:47:57.224280 protolizer-1.1.1/setup.cfg
+-rwxr-xr-x   0 hydra     (1000) hydra     (1000)      699 2023-04-16 09:47:48.000000 protolizer-1.1.1/setup.py
+drwxr-xr-x   0 hydra     (1000) hydra     (1000)        0 2023-04-16 09:47:57.224280 protolizer-1.1.1/tests/
+-rw-r--r--   0 hydra     (1000) hydra     (1000)        0 2022-08-09 07:25:39.000000 protolizer-1.1.1/tests/__init__.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)      863 2022-08-09 09:49:42.000000 protolizer-1.1.1/tests/test_custom_response.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     6316 2023-04-16 09:27:00.000000 protolizer-1.1.1/tests/test_fields.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     1092 2023-04-16 09:17:27.000000 protolizer-1.1.1/tests/test_json_to_protobuf.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     1429 2023-04-16 09:17:27.000000 protolizer-1.1.1/tests/test_nested_fields.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)      847 2022-08-09 08:03:49.000000 protolizer-1.1.1/tests/test_pre_serialize_hook.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     1128 2022-08-09 12:43:51.000000 protolizer-1.1.1/tests/test_protobuf_to_json.py
+-rw-r--r--   0 hydra     (1000) hydra     (1000)     1570 2022-08-09 09:28:25.000000 protolizer-1.1.1/tests/test_validation.py
```

### Comparing `protolizer-1.1.0/PKG-INFO` & `protolizer-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protolizer
-Version: 1.1.0
+Version: 1.1.1
 Summary: A simple library to serialize and deserialize protobuf messages
 Home-page: https://github.com/its0x4d/protolizer
 Author: MosyDev
 Author-email: mostafa.uwsgi@gmail.com
 License: MIT
 Keywords: protobuf serialization deserialization
 Platform: UNKNOWN
```

### Comparing `protolizer-1.1.0/README.md` & `protolizer-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `protolizer-1.1.0/protolizer/fields.py` & `protolizer-1.1.1/protolizer/fields.py`

 * *Files identical despite different names*

### Comparing `protolizer-1.1.0/protolizer/helpers.py` & `protolizer-1.1.1/protolizer/helpers.py`

 * *Files identical despite different names*

### Comparing `protolizer-1.1.0/protolizer/meta.py` & `protolizer-1.1.1/protolizer/meta.py`

 * *Files identical despite different names*

### Comparing `protolizer-1.1.0/protolizer/serializer.py` & `protolizer-1.1.1/protolizer/serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,14 +323,18 @@
 
     def to_internal_value(self, data):
         ret = dict()
         errors = dict()
         fields = self._readable_fields
 
         for field in fields:
+            if self.context == 'self' and isinstance(self.parent.context, dict):
+                field.context = self.parent.context
+            else:
+                field.context = self.context
             validate_method = getattr(self, 'validate_' + field.field_name, None)
             primitive_value = field.get_value(data, self)
             try:
                 validated_value = field.run_validation(primitive_value)
                 if validate_method:
                     validated_value = validate_method(primitive_value)
             except ValidationError as e:
```

### Comparing `protolizer-1.1.0/protolizer.egg-info/PKG-INFO` & `protolizer-1.1.1/protolizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protolizer
-Version: 1.1.0
+Version: 1.1.1
 Summary: A simple library to serialize and deserialize protobuf messages
 Home-page: https://github.com/its0x4d/protolizer
 Author: MosyDev
 Author-email: mostafa.uwsgi@gmail.com
 License: MIT
 Keywords: protobuf serialization deserialization
 Platform: UNKNOWN
```

### Comparing `protolizer-1.1.0/setup.py` & `protolizer-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="protolizer",
-    version="1.1.0",
+    version="1.1.1",
     author='MosyDev',
     author_email='mostafa.uwsgi@gmail.com',
     description='A simple library to serialize and deserialize protobuf messages',
     url='https://github.com/its0x4d/protolizer',
     packages=setuptools.find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `protolizer-1.1.0/tests/test_custom_response.py` & `protolizer-1.1.1/tests/test_custom_response.py`

 * *Files identical despite different names*

### Comparing `protolizer-1.1.0/tests/test_fields.py` & `protolizer-1.1.1/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `protolizer-1.1.0/tests/test_json_to_protobuf.py` & `protolizer-1.1.1/tests/test_json_to_protobuf.py`

 * *Files identical despite different names*

### Comparing `protolizer-1.1.0/tests/test_nested_fields.py` & `protolizer-1.1.1/tests/test_nested_fields.py`

 * *Files identical despite different names*

### Comparing `protolizer-1.1.0/tests/test_pre_serialize_hook.py` & `protolizer-1.1.1/tests/test_pre_serialize_hook.py`

 * *Files identical despite different names*

### Comparing `protolizer-1.1.0/tests/test_protobuf_to_json.py` & `protolizer-1.1.1/tests/test_protobuf_to_json.py`

 * *Files identical despite different names*

### Comparing `protolizer-1.1.0/tests/test_validation.py` & `protolizer-1.1.1/tests/test_validation.py`

 * *Files identical despite different names*

