# Comparing `tmp/arkserver-0.0.8.tar.gz` & `tmp/arkserver-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkserver-0.0.8.tar", last modified: Mon Aug 15 02:11:21 2022, max compression
+gzip compressed data, was "arkserver-0.0.9.tar", last modified: Mon Aug 15 02:13:48 2022, max compression
```

## Comparing `arkserver-0.0.8.tar` & `arkserver-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2022-08-15 02:11:21.092945 arkserver-0.0.8/
--rw-rw-rw-   0        0        0     1095 2022-08-06 20:49:26.000000 arkserver-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1951 2022-08-15 02:11:21.092945 arkserver-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1305 2022-08-06 05:59:32.000000 arkserver-0.0.8/README.md
--rw-rw-rw-   0        0        0      535 2022-08-11 15:03:37.000000 arkserver-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      979 2022-08-15 02:11:21.094946 arkserver-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-15 02:11:21.061946 arkserver-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-08-15 02:11:21.069945 arkserver-0.0.8/src/arkserver/
--rw-rw-rw-   0        0        0        0 2022-08-11 14:36:59.000000 arkserver-0.0.8/src/arkserver/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-15 02:11:21.086945 arkserver-0.0.8/src/arkserver/format/
--rw-rw-rw-   0        0        0      122 2022-08-14 23:42:19.000000 arkserver-0.0.8/src/arkserver/format/__init__.py
--rw-rw-rw-   0        0        0     4436 2022-08-15 00:44:42.000000 arkserver-0.0.8/src/arkserver/format/header.py
--rw-rw-rw-   0        0        0     4948 2022-08-15 00:44:42.000000 arkserver-0.0.8/src/arkserver/format/stream.py
-drwxrwxrwx   0        0        0        0 2022-08-15 02:11:21.088945 arkserver-0.0.8/src/arkserver/lib/
--rw-rw-rw-   0        0        0       72 2022-08-11 14:37:49.000000 arkserver-0.0.8/src/arkserver/lib/__init__.py
--rw-rw-rw-   0        0        0     2141 2022-08-15 00:26:39.000000 arkserver-0.0.8/src/arkserver/lib/configuration.py
--rw-rw-rw-   0        0        0      687 2022-08-15 00:20:47.000000 arkserver-0.0.8/src/arkserver/main.py
-drwxrwxrwx   0        0        0        0 2022-08-15 02:11:21.091945 arkserver-0.0.8/src/arkserver/server/
--rw-rw-rw-   0        0        0       97 2022-08-14 21:18:37.000000 arkserver-0.0.8/src/arkserver/server/__init__.py
--rw-rw-rw-   0        0        0     8020 2022-08-15 00:34:24.000000 arkserver-0.0.8/src/arkserver/server/game_bot_server.py
--rw-rw-rw-   0        0        0     2427 2022-08-14 21:18:37.000000 arkserver-0.0.8/src/arkserver/server/multi_server.py
--rw-rw-rw-   0        0        0     1150 2022-07-24 02:33:53.000000 arkserver-0.0.8/src/arkserver/server/single_server.py
--rw-rw-rw-   0        0        0      359 2022-08-14 21:39:15.000000 arkserver-0.0.8/src/arkserver/service.py
-drwxrwxrwx   0        0        0        0 2022-08-15 02:11:21.083945 arkserver-0.0.8/src/arkserver.egg-info/
--rw-rw-rw-   0        0        0     1951 2022-08-15 02:11:21.000000 arkserver-0.0.8/src/arkserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      607 2022-08-15 02:11:21.000000 arkserver-0.0.8/src/arkserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-15 02:11:21.000000 arkserver-0.0.8/src/arkserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2022-08-15 02:11:21.000000 arkserver-0.0.8/src/arkserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-08-15 02:11:21.000000 arkserver-0.0.8/src/arkserver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-08-15 02:13:48.372843 arkserver-0.0.9/
+-rw-rw-rw-   0        0        0     1095 2022-08-06 20:49:26.000000 arkserver-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1951 2022-08-15 02:13:48.372843 arkserver-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1305 2022-08-06 05:59:32.000000 arkserver-0.0.9/README.md
+-rw-rw-rw-   0        0        0      535 2022-08-11 15:03:37.000000 arkserver-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      979 2022-08-15 02:13:48.373843 arkserver-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-08-15 02:13:48.345009 arkserver-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-08-15 02:13:48.352843 arkserver-0.0.9/src/arkserver/
+-rw-rw-rw-   0        0        0        0 2022-08-11 14:36:59.000000 arkserver-0.0.9/src/arkserver/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-15 02:13:48.366842 arkserver-0.0.9/src/arkserver/format/
+-rw-rw-rw-   0        0        0      122 2022-08-14 23:42:19.000000 arkserver-0.0.9/src/arkserver/format/__init__.py
+-rw-rw-rw-   0        0        0     4436 2022-08-15 00:44:42.000000 arkserver-0.0.9/src/arkserver/format/header.py
+-rw-rw-rw-   0        0        0     4948 2022-08-15 00:44:42.000000 arkserver-0.0.9/src/arkserver/format/stream.py
+drwxrwxrwx   0        0        0        0 2022-08-15 02:13:48.367845 arkserver-0.0.9/src/arkserver/lib/
+-rw-rw-rw-   0        0        0       68 2022-08-15 02:13:17.000000 arkserver-0.0.9/src/arkserver/lib/__init__.py
+-rw-rw-rw-   0        0        0     2141 2022-08-15 00:26:39.000000 arkserver-0.0.9/src/arkserver/lib/configuration.py
+-rw-rw-rw-   0        0        0      687 2022-08-15 00:20:47.000000 arkserver-0.0.9/src/arkserver/main.py
+drwxrwxrwx   0        0        0        0 2022-08-15 02:13:48.371841 arkserver-0.0.9/src/arkserver/server/
+-rw-rw-rw-   0        0        0       93 2022-08-15 02:13:17.000000 arkserver-0.0.9/src/arkserver/server/__init__.py
+-rw-rw-rw-   0        0        0     8012 2022-08-15 02:13:17.000000 arkserver-0.0.9/src/arkserver/server/game_bot_server.py
+-rw-rw-rw-   0        0        0     2427 2022-08-14 21:18:37.000000 arkserver-0.0.9/src/arkserver/server/multi_server.py
+-rw-rw-rw-   0        0        0     1150 2022-07-24 02:33:53.000000 arkserver-0.0.9/src/arkserver/server/single_server.py
+-rw-rw-rw-   0        0        0      359 2022-08-14 21:39:15.000000 arkserver-0.0.9/src/arkserver/service.py
+drwxrwxrwx   0        0        0        0 2022-08-15 02:13:48.363841 arkserver-0.0.9/src/arkserver.egg-info/
+-rw-rw-rw-   0        0        0     1951 2022-08-15 02:13:48.000000 arkserver-0.0.9/src/arkserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2022-08-15 02:13:48.000000 arkserver-0.0.9/src/arkserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-08-15 02:13:48.000000 arkserver-0.0.9/src/arkserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2022-08-15 02:13:48.000000 arkserver-0.0.9/src/arkserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-08-15 02:13:48.000000 arkserver-0.0.9/src/arkserver.egg-info/top_level.txt
```

### Comparing `arkserver-0.0.8/LICENSE` & `arkserver-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `arkserver-0.0.8/PKG-INFO` & `arkserver-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkserver
-Version: 0.0.8
+Version: 0.0.9
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Server
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Server/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `arkserver-0.0.8/README.md` & `arkserver-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `arkserver-0.0.8/pyproject.toml` & `arkserver-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arkserver-0.0.8/setup.cfg` & `arkserver-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 726b 7365 7276 6572 0d0a 7665   = arkserver..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 380d 0a61  rsion = 0.0.8..a
+00000020: 7273 696f 6e20 3d20 302e 302e 390d 0a61  rsion = 0.0.9..a
 00000030: 7574 686f 7220 3d20 4d61 7572 6963 696f  uthor = Mauricio
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2064 6576 2e6d 6175 7269 6369 6f2e 6c6f   dev.mauricio.lo
 00000060: 6d65 6c69 4067 6d61 696c 2e63 6f6d 0d0a  meli@gmail.com..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 5468  description = Th
 00000080: 6973 2061 7070 6c69 6361 7469 6f6e 2061  is application a
 00000090: 6363 6573 7365 7320 7468 6520 4172 6b20  ccesses the Ark
```

### Comparing `arkserver-0.0.8/src/arkserver/format/header.py` & `arkserver-0.0.9/src/arkserver/format/header.py`

 * *Files identical despite different names*

### Comparing `arkserver-0.0.8/src/arkserver/format/stream.py` & `arkserver-0.0.9/src/arkserver/format/stream.py`

 * *Files identical despite different names*

### Comparing `arkserver-0.0.8/src/arkserver/lib/configuration.py` & `arkserver-0.0.9/src/arkserver/lib/configuration.py`

 * *Files identical despite different names*

### Comparing `arkserver-0.0.8/src/arkserver/main.py` & `arkserver-0.0.9/src/arkserver/main.py`

 * *Files identical despite different names*

### Comparing `arkserver-0.0.8/src/arkserver/server/game_bot_server.py` & `arkserver-0.0.9/src/arkserver/server/game_bot_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from src.arkserver.lib import Ini
-from src.arkserver.format.stream import Stream
+from arkserver.lib import Ini
+from arkserver.format.stream import Stream
 import socket
 import selectors
 import types
 from pathlib import Path
 
 
 class GameBotServer:
```

### Comparing `arkserver-0.0.8/src/arkserver/server/multi_server.py` & `arkserver-0.0.9/src/arkserver/server/multi_server.py`

 * *Files identical despite different names*

### Comparing `arkserver-0.0.8/src/arkserver/server/single_server.py` & `arkserver-0.0.9/src/arkserver/server/single_server.py`

 * *Files identical despite different names*

### Comparing `arkserver-0.0.8/src/arkserver.egg-info/PKG-INFO` & `arkserver-0.0.9/src/arkserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkserver
-Version: 0.0.8
+Version: 0.0.9
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Server
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Server/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `arkserver-0.0.8/src/arkserver.egg-info/SOURCES.txt` & `arkserver-0.0.9/src/arkserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

