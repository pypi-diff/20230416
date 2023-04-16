# Comparing `tmp/arkclient-0.0.8.tar.gz` & `tmp/arkclient-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkclient-0.0.8.tar", last modified: Mon Aug 15 02:19:51 2022, max compression
+gzip compressed data, was "arkclient-0.0.9.tar", last modified: Mon Aug 15 02:41:16 2022, max compression
```

## Comparing `arkclient-0.0.8.tar` & `arkclient-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2022-08-15 02:19:51.704439 arkclient-0.0.8/
--rw-rw-rw-   0        0        0     1095 2022-08-11 13:59:26.000000 arkclient-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      658 2022-08-15 02:19:51.704439 arkclient-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       12 2022-08-11 13:59:26.000000 arkclient-0.0.8/README.md
--rw-rw-rw-   0        0        0      535 2022-08-11 15:07:10.000000 arkclient-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      979 2022-08-15 02:19:51.709438 arkclient-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-15 02:19:51.676438 arkclient-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-08-15 02:19:51.682439 arkclient-0.0.8/src/arkclient/
--rw-rw-rw-   0        0        0        2 2022-08-14 21:51:42.000000 arkclient-0.0.8/src/arkclient/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-15 02:19:51.698439 arkclient-0.0.8/src/arkclient/client/
--rw-rw-rw-   0        0        0       93 2022-08-14 21:49:32.000000 arkclient-0.0.8/src/arkclient/client/__init__.py
--rw-rw-rw-   0        0        0     8976 2022-08-15 00:07:32.000000 arkclient-0.0.8/src/arkclient/client/game_bot_client.py
--rw-rw-rw-   0        0        0     1695 2022-07-24 04:02:31.000000 arkclient-0.0.8/src/arkclient/client/multi_client.py
--rw-rw-rw-   0        0        0      724 2022-07-24 02:33:53.000000 arkclient-0.0.8/src/arkclient/client/single_client.py
-drwxrwxrwx   0        0        0        0 2022-08-15 02:19:51.700437 arkclient-0.0.8/src/arkclient/format/
--rw-rw-rw-   0        0        0      122 2022-08-14 21:50:32.000000 arkclient-0.0.8/src/arkclient/format/__init__.py
--rw-rw-rw-   0        0        0     4436 2022-08-15 00:45:04.000000 arkclient-0.0.8/src/arkclient/format/header.py
--rw-rw-rw-   0        0        0     4948 2022-08-15 00:45:04.000000 arkclient-0.0.8/src/arkclient/format/stream.py
-drwxrwxrwx   0        0        0        0 2022-08-15 02:19:51.702437 arkclient-0.0.8/src/arkclient/lib/
--rw-rw-rw-   0        0        0       68 2022-08-14 21:50:32.000000 arkclient-0.0.8/src/arkclient/lib/__init__.py
--rw-rw-rw-   0        0        0     1967 2022-08-14 21:41:50.000000 arkclient-0.0.8/src/arkclient/lib/configuration.py
--rw-rw-rw-   0        0        0      508 2022-08-15 00:19:35.000000 arkclient-0.0.8/src/arkclient/main.py
-drwxrwxrwx   0        0        0        0 2022-08-15 02:19:51.703436 arkclient-0.0.8/src/arkclient/tools/
--rw-rw-rw-   0        0        0       94 2022-08-14 21:41:50.000000 arkclient-0.0.8/src/arkclient/tools/__init__.py
--rw-rw-rw-   0        0        0     1936 2022-08-14 21:41:50.000000 arkclient-0.0.8/src/arkclient/tools/configuration.py
-drwxrwxrwx   0        0        0        0 2022-08-15 02:19:51.694436 arkclient-0.0.8/src/arkclient.egg-info/
--rw-rw-rw-   0        0        0      658 2022-08-15 02:19:51.000000 arkclient-0.0.8/src/arkclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      651 2022-08-15 02:19:51.000000 arkclient-0.0.8/src/arkclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-15 02:19:51.000000 arkclient-0.0.8/src/arkclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2022-08-15 02:19:51.000000 arkclient-0.0.8/src/arkclient.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-08-15 02:19:51.000000 arkclient-0.0.8/src/arkclient.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-08-15 02:41:16.333227 arkclient-0.0.9/
+-rw-rw-rw-   0        0        0     1095 2022-08-11 13:59:26.000000 arkclient-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      658 2022-08-15 02:41:16.333227 arkclient-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2022-08-11 13:59:26.000000 arkclient-0.0.9/README.md
+-rw-rw-rw-   0        0        0      535 2022-08-11 15:07:10.000000 arkclient-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      979 2022-08-15 02:41:16.335229 arkclient-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-08-15 02:41:16.302226 arkclient-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-08-15 02:41:16.308227 arkclient-0.0.9/src/arkclient/
+-rw-rw-rw-   0        0        0        2 2022-08-14 21:51:42.000000 arkclient-0.0.9/src/arkclient/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-15 02:41:16.326229 arkclient-0.0.9/src/arkclient/client/
+-rw-rw-rw-   0        0        0       93 2022-08-14 21:49:32.000000 arkclient-0.0.9/src/arkclient/client/__init__.py
+-rw-rw-rw-   0        0        0     8976 2022-08-15 00:07:32.000000 arkclient-0.0.9/src/arkclient/client/game_bot_client.py
+-rw-rw-rw-   0        0        0     1695 2022-07-24 04:02:31.000000 arkclient-0.0.9/src/arkclient/client/multi_client.py
+-rw-rw-rw-   0        0        0      724 2022-07-24 02:33:53.000000 arkclient-0.0.9/src/arkclient/client/single_client.py
+drwxrwxrwx   0        0        0        0 2022-08-15 02:41:16.329226 arkclient-0.0.9/src/arkclient/format/
+-rw-rw-rw-   0        0        0      122 2022-08-14 21:50:32.000000 arkclient-0.0.9/src/arkclient/format/__init__.py
+-rw-rw-rw-   0        0        0     4436 2022-08-15 00:45:04.000000 arkclient-0.0.9/src/arkclient/format/header.py
+-rw-rw-rw-   0        0        0     4948 2022-08-15 00:45:04.000000 arkclient-0.0.9/src/arkclient/format/stream.py
+drwxrwxrwx   0        0        0        0 2022-08-15 02:41:16.330227 arkclient-0.0.9/src/arkclient/lib/
+-rw-rw-rw-   0        0        0       68 2022-08-14 21:50:32.000000 arkclient-0.0.9/src/arkclient/lib/__init__.py
+-rw-rw-rw-   0        0        0     1967 2022-08-14 21:41:50.000000 arkclient-0.0.9/src/arkclient/lib/configuration.py
+-rw-rw-rw-   0        0        0      508 2022-08-15 00:19:35.000000 arkclient-0.0.9/src/arkclient/main.py
+drwxrwxrwx   0        0        0        0 2022-08-15 02:41:16.333227 arkclient-0.0.9/src/arkclient/tools/
+-rw-rw-rw-   0        0        0       94 2022-08-14 21:41:50.000000 arkclient-0.0.9/src/arkclient/tools/__init__.py
+-rw-rw-rw-   0        0        0     1936 2022-08-14 21:41:50.000000 arkclient-0.0.9/src/arkclient/tools/configuration.py
+drwxrwxrwx   0        0        0        0 2022-08-15 02:41:16.322229 arkclient-0.0.9/src/arkclient.egg-info/
+-rw-rw-rw-   0        0        0      658 2022-08-15 02:41:16.000000 arkclient-0.0.9/src/arkclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      651 2022-08-15 02:41:16.000000 arkclient-0.0.9/src/arkclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-08-15 02:41:16.000000 arkclient-0.0.9/src/arkclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2022-08-15 02:41:16.000000 arkclient-0.0.9/src/arkclient.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-08-15 02:41:16.000000 arkclient-0.0.9/src/arkclient.egg-info/top_level.txt
```

### Comparing `arkclient-0.0.8/LICENSE` & `arkclient-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `arkclient-0.0.8/PKG-INFO` & `arkclient-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkclient
-Version: 0.0.8
+Version: 0.0.9
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Client
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Client/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `arkclient-0.0.8/pyproject.toml` & `arkclient-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arkclient-0.0.8/setup.cfg` & `arkclient-0.0.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 726b 636c 6965 6e74 0d0a 7665   = arkclient..ve
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

### Comparing `arkclient-0.0.8/src/arkclient/client/game_bot_client.py` & `arkclient-0.0.9/src/arkclient/client/game_bot_client.py`

 * *Files identical despite different names*

### Comparing `arkclient-0.0.8/src/arkclient/client/multi_client.py` & `arkclient-0.0.9/src/arkclient/client/multi_client.py`

 * *Files identical despite different names*

### Comparing `arkclient-0.0.8/src/arkclient/client/single_client.py` & `arkclient-0.0.9/src/arkclient/client/single_client.py`

 * *Files identical despite different names*

### Comparing `arkclient-0.0.8/src/arkclient/format/header.py` & `arkclient-0.0.9/src/arkclient/format/header.py`

 * *Files identical despite different names*

### Comparing `arkclient-0.0.8/src/arkclient/format/stream.py` & `arkclient-0.0.9/src/arkclient/format/stream.py`

 * *Files identical despite different names*

### Comparing `arkclient-0.0.8/src/arkclient/lib/configuration.py` & `arkclient-0.0.9/src/arkclient/lib/configuration.py`

 * *Files identical despite different names*

### Comparing `arkclient-0.0.8/src/arkclient/tools/configuration.py` & `arkclient-0.0.9/src/arkclient/tools/configuration.py`

 * *Files identical despite different names*

### Comparing `arkclient-0.0.8/src/arkclient.egg-info/PKG-INFO` & `arkclient-0.0.9/src/arkclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkclient
-Version: 0.0.8
+Version: 0.0.9
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Client
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Client/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `arkclient-0.0.8/src/arkclient.egg-info/SOURCES.txt` & `arkclient-0.0.9/src/arkclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

