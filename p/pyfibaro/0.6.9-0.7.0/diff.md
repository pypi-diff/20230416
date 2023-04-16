# Comparing `tmp/pyfibaro-0.6.9.tar.gz` & `tmp/pyfibaro-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfibaro-0.6.9.tar", last modified: Fri Mar  3 17:56:20 2023, max compression
+gzip compressed data, was "pyfibaro-0.7.0.tar", last modified: Sun Apr 16 17:16:07 2023, max compression
```

## Comparing `pyfibaro-0.6.9.tar` & `pyfibaro-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 17:56:20.499692 pyfibaro-0.6.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-03 17:55:55.000000 pyfibaro-0.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-03-03 17:56:20.503692 pyfibaro-0.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-03-03 17:55:55.000000 pyfibaro-0.6.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 17:56:20.499692 pyfibaro-0.6.9/pyfibaro/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-03 17:55:55.000000 pyfibaro-0.6.9/pyfibaro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 17:56:20.499692 pyfibaro-0.6.9/pyfibaro/common/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-03 17:55:55.000000 pyfibaro-0.6.9/pyfibaro/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-03 17:55:55.000000 pyfibaro-0.6.9/pyfibaro/common/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-03-03 17:55:55.000000 pyfibaro-0.6.9/pyfibaro/common/rest_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-03-03 17:55:55.000000 pyfibaro-0.6.9/pyfibaro/fibaro_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16648 2023-03-03 17:55:55.000000 pyfibaro-0.6.9/pyfibaro/fibaro_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-03-03 17:55:55.000000 pyfibaro-0.6.9/pyfibaro/fibaro_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-03 17:55:55.000000 pyfibaro-0.6.9/pyfibaro/fibaro_login.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-03-03 17:55:55.000000 pyfibaro-0.6.9/pyfibaro/fibaro_room.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-03-03 17:55:55.000000 pyfibaro-0.6.9/pyfibaro/fibaro_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-03-03 17:55:55.000000 pyfibaro-0.6.9/pyfibaro/fibaro_state_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 17:56:20.499692 pyfibaro-0.6.9/pyfibaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-03-03 17:56:19.000000 pyfibaro-0.6.9/pyfibaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-03 17:56:20.000000 pyfibaro-0.6.9/pyfibaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 17:56:19.000000 pyfibaro-0.6.9/pyfibaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-03 17:56:20.000000 pyfibaro-0.6.9/pyfibaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-03 17:56:20.000000 pyfibaro-0.6.9/pyfibaro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-03 17:55:55.000000 pyfibaro-0.6.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-03-03 17:56:20.503692 pyfibaro-0.6.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:16:07.571606 pyfibaro-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-16 17:16:07.571606 pyfibaro-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:16:07.567606 pyfibaro-0.7.0/pyfibaro/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:16:07.567606 pyfibaro-0.7.0/pyfibaro/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/common/rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/fibaro_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17358 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/fibaro_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/fibaro_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/fibaro_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/fibaro_room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/fibaro_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyfibaro/fibaro_state_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:16:07.571606 pyfibaro-0.7.0/pyfibaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-16 17:16:06.000000 pyfibaro-0.7.0/pyfibaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-16 17:16:07.000000 pyfibaro-0.7.0/pyfibaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 17:16:06.000000 pyfibaro-0.7.0/pyfibaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-16 17:16:07.000000 pyfibaro-0.7.0/pyfibaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-16 17:16:07.000000 pyfibaro-0.7.0/pyfibaro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 17:15:39.000000 pyfibaro-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-16 17:16:07.571606 pyfibaro-0.7.0/setup.cfg
```

### Comparing `pyfibaro-0.6.9/LICENSE` & `pyfibaro-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.6.9/PKG-INFO` & `pyfibaro-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfibaro
-Version: 0.6.9
+Version: 0.7.0
 Summary: Simple API to access fibaro home center from any Python 3 script. Designed for Home Assistant (but not only)
 Home-page: https://github.com/rappenze/pyfibaro
 Author: Roman Appenzeller
 Author-email: 
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyfibaro-0.6.9/README.md` & `pyfibaro-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.6.9/pyfibaro/common/const.py` & `pyfibaro-0.7.0/pyfibaro/common/const.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.6.9/pyfibaro/common/rest_client.py` & `pyfibaro-0.7.0/pyfibaro/common/rest_client.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.6.9/pyfibaro/fibaro_client.py` & `pyfibaro-0.7.0/pyfibaro/fibaro_client.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.6.9/pyfibaro/fibaro_device.py` & `pyfibaro-0.7.0/pyfibaro/fibaro_device.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,14 +142,36 @@
 
     @property
     def has_armed(self) -> bool:
         """Returns true if the device has a unit property."""
         return "armed" in self.properties
 
     @property
+    def dead(self) -> bool:
+        """Returns the state if the device is reachable if supported,
+        otherwise False is returned.
+        """
+        return _to_bool(self.properties.get("dead", False))
+
+    @property
+    def has_dead(self) -> bool:
+        """Returns true if the device has a dead property."""
+        return "dead" in self.properties
+
+    @property
+    def dead_reason(self) -> str | None:
+        """Returns the dead reason or None if not supported."""
+        return self.properties.get("deadReason")
+
+    @property
+    def has_dead_reason(self) -> bool:
+        """Returns true if the device has a deadReason property."""
+        return "deadReason" in self.properties
+
+    @property
     def value(self) -> ValueModel:
         """Returns the value info."""
         return ValueModel(self.properties, "value")
 
     @property
     def value_2(self) -> ValueModel:
         """Returns the value info."""
```

### Comparing `pyfibaro-0.6.9/pyfibaro/fibaro_info.py` & `pyfibaro-0.7.0/pyfibaro/fibaro_info.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.6.9/pyfibaro/fibaro_room.py` & `pyfibaro-0.7.0/pyfibaro/fibaro_room.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.6.9/pyfibaro/fibaro_scene.py` & `pyfibaro-0.7.0/pyfibaro/fibaro_scene.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.6.9/pyfibaro/fibaro_state_handler.py` & `pyfibaro-0.7.0/pyfibaro/fibaro_state_handler.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.6.9/pyfibaro.egg-info/PKG-INFO` & `pyfibaro-0.7.0/pyfibaro.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfibaro
-Version: 0.6.9
+Version: 0.7.0
 Summary: Simple API to access fibaro home center from any Python 3 script. Designed for Home Assistant (but not only)
 Home-page: https://github.com/rappenze/pyfibaro
 Author: Roman Appenzeller
 Author-email: 
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyfibaro-0.6.9/setup.cfg` & `pyfibaro-0.7.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyfibaro
-version = 0.6.9
+version = 0.7.0
 description = Simple API to access fibaro home center from any Python 3 script. Designed for Home Assistant (but not only)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/rappenze/pyfibaro
 author = Roman Appenzeller
 author_email = 
 license = MIT
```

