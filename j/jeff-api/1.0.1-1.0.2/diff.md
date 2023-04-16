# Comparing `tmp/jeff_api-1.0.1.tar.gz` & `tmp/jeff_api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeff_api-1.0.1.tar", last modified: Sun Apr 16 20:13:50 2023, max compression
+gzip compressed data, was "jeff_api-1.0.2.tar", last modified: Sun Apr 16 20:16:55 2023, max compression
```

## Comparing `jeff_api-1.0.1.tar` & `jeff_api-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 20:13:50.873737 jeff_api-1.0.1/
--rw-------   0 markcda   (1000) markcda   (1000)     1087 2023-01-15 14:50:00.000000 jeff_api-1.0.1/LICENSE
--rw-r--r--   0 markcda   (1000) markcda   (1000)     1134 2023-04-16 20:13:50.871737 jeff_api-1.0.1/PKG-INFO
--rw-r--r--   0 markcda   (1000) markcda   (1000)      623 2023-03-05 09:58:33.000000 jeff_api-1.0.1/README.md
--rw-------   0 markcda   (1000) markcda   (1000)      497 2023-04-16 20:13:21.000000 jeff_api-1.0.1/pyproject.toml
--rw-r--r--   0 markcda   (1000) markcda   (1000)       38 2023-04-16 20:13:50.873737 jeff_api-1.0.1/setup.cfg
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 20:13:50.865737 jeff_api-1.0.1/src/
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 20:13:50.867737 jeff_api-1.0.1/src/jeff_api/
--rw-r--r--   0 markcda   (1000) markcda   (1000)        0 2023-01-01 20:50:00.000000 jeff_api-1.0.1/src/jeff_api/__init__.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     6921 2023-04-16 20:12:40.000000 jeff_api-1.0.1/src/jeff_api/bridge.py
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 20:13:50.871737 jeff_api-1.0.1/src/jeff_api.egg-info/
--rw-------   0 markcda   (1000) markcda   (1000)     1134 2023-04-16 20:13:50.000000 jeff_api-1.0.1/src/jeff_api.egg-info/PKG-INFO
--rw-------   0 markcda   (1000) markcda   (1000)      224 2023-04-16 20:13:50.000000 jeff_api-1.0.1/src/jeff_api.egg-info/SOURCES.txt
--rw-------   0 markcda   (1000) markcda   (1000)        1 2023-04-16 20:13:50.000000 jeff_api-1.0.1/src/jeff_api.egg-info/dependency_links.txt
--rw-------   0 markcda   (1000) markcda   (1000)        9 2023-04-16 20:13:50.000000 jeff_api-1.0.1/src/jeff_api.egg-info/top_level.txt
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 20:16:55.472870 jeff_api-1.0.2/
+-rw-------   0 markcda   (1000) markcda   (1000)     1087 2023-01-15 14:50:00.000000 jeff_api-1.0.2/LICENSE
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     1134 2023-04-16 20:16:55.470870 jeff_api-1.0.2/PKG-INFO
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      623 2023-03-05 09:58:33.000000 jeff_api-1.0.2/README.md
+-rw-------   0 markcda   (1000) markcda   (1000)      497 2023-04-16 20:16:22.000000 jeff_api-1.0.2/pyproject.toml
+-rw-r--r--   0 markcda   (1000) markcda   (1000)       38 2023-04-16 20:16:55.472870 jeff_api-1.0.2/setup.cfg
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 20:16:55.460870 jeff_api-1.0.2/src/
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 20:16:55.466870 jeff_api-1.0.2/src/jeff_api/
+-rw-r--r--   0 markcda   (1000) markcda   (1000)        0 2023-01-01 20:50:00.000000 jeff_api-1.0.2/src/jeff_api/__init__.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     6941 2023-04-16 20:16:14.000000 jeff_api-1.0.2/src/jeff_api/bridge.py
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 20:16:55.470870 jeff_api-1.0.2/src/jeff_api.egg-info/
+-rw-------   0 markcda   (1000) markcda   (1000)     1134 2023-04-16 20:16:55.000000 jeff_api-1.0.2/src/jeff_api.egg-info/PKG-INFO
+-rw-------   0 markcda   (1000) markcda   (1000)      224 2023-04-16 20:16:55.000000 jeff_api-1.0.2/src/jeff_api.egg-info/SOURCES.txt
+-rw-------   0 markcda   (1000) markcda   (1000)        1 2023-04-16 20:16:55.000000 jeff_api-1.0.2/src/jeff_api.egg-info/dependency_links.txt
+-rw-------   0 markcda   (1000) markcda   (1000)        9 2023-04-16 20:16:55.000000 jeff_api-1.0.2/src/jeff_api.egg-info/top_level.txt
```

### Comparing `jeff_api-1.0.1/LICENSE` & `jeff_api-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jeff_api-1.0.1/PKG-INFO` & `jeff_api-1.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeff_api
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python library for intercommunicating with Jeff.
 Author-email: Mark CDA <aclo.create@gmail.com>
 Project-URL: Homepage, https://github.com/markcda/jeff
 Project-URL: Bug Tracker, https://github.com/markcda/jeff/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jeff_api-1.0.1/README.md` & `jeff_api-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `jeff_api-1.0.1/src/jeff_api/bridge.py` & `jeff_api-1.0.2/src/jeff_api/bridge.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,14 +142,15 @@
   "TBD"
 
   def __init__(self, jeff_host: Optional[str], jeff_port: int, self_host: Optional[str], self_port: int):
     self.jeff_host = jeff_host
     self.jeff_port = jeff_port
     self.self_host = self_host if self_host is not None else "0.0.0.0"
     self.self_port = self_port
+    self.scn = None
     self.init_server()
 
   def init_server(self):
     self.server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     self.server_socket.bind((self.self_host, self.self_port))
     self.server_socket.listen()
```

### Comparing `jeff_api-1.0.1/src/jeff_api.egg-info/PKG-INFO` & `jeff_api-1.0.2/src/jeff_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeff-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python library for intercommunicating with Jeff.
 Author-email: Mark CDA <aclo.create@gmail.com>
 Project-URL: Homepage, https://github.com/markcda/jeff
 Project-URL: Bug Tracker, https://github.com/markcda/jeff/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

