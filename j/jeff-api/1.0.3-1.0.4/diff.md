# Comparing `tmp/jeff_api-1.0.3.tar.gz` & `tmp/jeff_api-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeff_api-1.0.3.tar", last modified: Sun Apr 16 20:21:56 2023, max compression
+gzip compressed data, was "jeff_api-1.0.4.tar", last modified: Sun Apr 16 20:28:50 2023, max compression
```

## Comparing `jeff_api-1.0.3.tar` & `jeff_api-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 20:21:56.888711 jeff_api-1.0.3/
--rw-------   0 markcda   (1000) markcda   (1000)     1087 2023-01-15 14:50:00.000000 jeff_api-1.0.3/LICENSE
--rw-r--r--   0 markcda   (1000) markcda   (1000)     1134 2023-04-16 20:21:56.888711 jeff_api-1.0.3/PKG-INFO
--rw-r--r--   0 markcda   (1000) markcda   (1000)      623 2023-03-05 09:58:33.000000 jeff_api-1.0.3/README.md
--rw-------   0 markcda   (1000) markcda   (1000)      497 2023-04-16 20:20:27.000000 jeff_api-1.0.3/pyproject.toml
--rw-r--r--   0 markcda   (1000) markcda   (1000)       38 2023-04-16 20:21:56.888711 jeff_api-1.0.3/setup.cfg
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 20:21:56.878711 jeff_api-1.0.3/src/
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 20:21:56.882711 jeff_api-1.0.3/src/jeff_api/
--rw-r--r--   0 markcda   (1000) markcda   (1000)        0 2023-01-01 20:50:00.000000 jeff_api-1.0.3/src/jeff_api/__init__.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     7054 2023-04-16 20:21:08.000000 jeff_api-1.0.3/src/jeff_api/bridge.py
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 20:21:56.886711 jeff_api-1.0.3/src/jeff_api.egg-info/
--rw-------   0 markcda   (1000) markcda   (1000)     1134 2023-04-16 20:21:56.000000 jeff_api-1.0.3/src/jeff_api.egg-info/PKG-INFO
--rw-------   0 markcda   (1000) markcda   (1000)      224 2023-04-16 20:21:56.000000 jeff_api-1.0.3/src/jeff_api.egg-info/SOURCES.txt
--rw-------   0 markcda   (1000) markcda   (1000)        1 2023-04-16 20:21:56.000000 jeff_api-1.0.3/src/jeff_api.egg-info/dependency_links.txt
--rw-------   0 markcda   (1000) markcda   (1000)        9 2023-04-16 20:21:56.000000 jeff_api-1.0.3/src/jeff_api.egg-info/top_level.txt
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 20:28:50.547226 jeff_api-1.0.4/
+-rw-------   0 markcda   (1000) markcda   (1000)     1087 2023-01-15 14:50:00.000000 jeff_api-1.0.4/LICENSE
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     1134 2023-04-16 20:28:50.547226 jeff_api-1.0.4/PKG-INFO
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      623 2023-03-05 09:58:33.000000 jeff_api-1.0.4/README.md
+-rw-------   0 markcda   (1000) markcda   (1000)      497 2023-04-16 20:27:53.000000 jeff_api-1.0.4/pyproject.toml
+-rw-r--r--   0 markcda   (1000) markcda   (1000)       38 2023-04-16 20:28:50.547226 jeff_api-1.0.4/setup.cfg
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 20:28:50.539225 jeff_api-1.0.4/src/
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 20:28:50.543225 jeff_api-1.0.4/src/jeff_api/
+-rw-r--r--   0 markcda   (1000) markcda   (1000)        0 2023-01-01 20:50:00.000000 jeff_api-1.0.4/src/jeff_api/__init__.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     7095 2023-04-16 20:27:35.000000 jeff_api-1.0.4/src/jeff_api/bridge.py
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 20:28:50.545225 jeff_api-1.0.4/src/jeff_api.egg-info/
+-rw-------   0 markcda   (1000) markcda   (1000)     1134 2023-04-16 20:28:50.000000 jeff_api-1.0.4/src/jeff_api.egg-info/PKG-INFO
+-rw-------   0 markcda   (1000) markcda   (1000)      224 2023-04-16 20:28:50.000000 jeff_api-1.0.4/src/jeff_api.egg-info/SOURCES.txt
+-rw-------   0 markcda   (1000) markcda   (1000)        1 2023-04-16 20:28:50.000000 jeff_api-1.0.4/src/jeff_api.egg-info/dependency_links.txt
+-rw-------   0 markcda   (1000) markcda   (1000)        9 2023-04-16 20:28:50.000000 jeff_api-1.0.4/src/jeff_api.egg-info/top_level.txt
```

### Comparing `jeff_api-1.0.3/LICENSE` & `jeff_api-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jeff_api-1.0.3/PKG-INFO` & `jeff_api-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeff_api
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python library for intercommunicating with Jeff.
 Author-email: Mark CDA <aclo.create@gmail.com>
 Project-URL: Homepage, https://github.com/markcda/jeff
 Project-URL: Bug Tracker, https://github.com/markcda/jeff/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jeff_api-1.0.3/README.md` & `jeff_api-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `jeff_api-1.0.3/src/jeff_api/bridge.py` & `jeff_api-1.0.4/src/jeff_api/bridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,21 +146,22 @@
     jeff_host: Optional[str],
     jeff_port: int,
     self_host: Optional[str] = None,
     self_port: Optional[int] = None
   ):
     self.jeff_host = jeff_host
     self.jeff_port = jeff_port
-    self.self_host = self_host if self_host is not None else "0.0.0.0"
+    self.self_host = self_host
     self.self_port = self_port
     self.scn = None
     self.init_server()
 
   def init_server(self):
     if self.self_host is None and self.self_port is None: return
+    self.self_host = self.self_host if self.self_host is not None else "0.0.0.0"
     self.server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     self.server_socket.bind((self.self_host, self.self_port))
     self.server_socket.listen()
 
   def _encode_json(j: dict):
     return json.dumps(j).encode()
```

### Comparing `jeff_api-1.0.3/src/jeff_api.egg-info/PKG-INFO` & `jeff_api-1.0.4/src/jeff_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeff-api
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python library for intercommunicating with Jeff.
 Author-email: Mark CDA <aclo.create@gmail.com>
 Project-URL: Homepage, https://github.com/markcda/jeff
 Project-URL: Bug Tracker, https://github.com/markcda/jeff/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

