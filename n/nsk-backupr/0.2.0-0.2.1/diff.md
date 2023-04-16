# Comparing `tmp/nsk_backupr-0.2.0.tar.gz` & `tmp/nsk_backupr-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsk_backupr-0.2.0.tar", max compression
+gzip compressed data, was "nsk_backupr-0.2.1.tar", max compression
```

## Comparing `nsk_backupr-0.2.0.tar` & `nsk_backupr-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2023-04-08 19:28:12.037129 nsk_backupr-0.2.0/LICENSE
--rw-r--r--   0        0        0      341 2023-04-09 06:01:26.289658 nsk_backupr-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-08 19:28:12.037129 nsk_backupr-0.2.0/backupr/__init__.py
--rw-r--r--   0        0        0     1077 2023-04-11 04:28:23.044836 nsk_backupr-0.2.0/backupr/cli.py
--rw-r--r--   0        0        0     5971 2023-04-16 14:59:06.822141 nsk_backupr-0.2.0/backupr/config.py
--rw-r--r--   0        0        0      687 2023-04-11 04:28:23.044836 nsk_backupr-0.2.0/backupr/di.py
--rw-r--r--   0        0        0     2652 2023-04-16 01:59:04.406086 nsk_backupr-0.2.0/backupr/encrypter.py
--rw-r--r--   0        0        0     6363 2023-04-16 01:59:04.406086 nsk_backupr-0.2.0/backupr/engine.py
--rw-r--r--   0        0        0     1830 2023-04-08 19:28:12.037129 nsk_backupr-0.2.0/backupr/storage_provider/__init__.py
--rw-r--r--   0        0        0     2815 2023-04-11 00:35:47.611849 nsk_backupr-0.2.0/backupr/storage_provider/b2_provider.py
--rw-r--r--   0        0        0     1028 2023-04-08 19:28:12.037129 nsk_backupr-0.2.0/backupr/storage_provider/local_provider.py
--rw-r--r--   0        0        0     2265 2023-04-11 04:28:23.044836 nsk_backupr-0.2.0/backupr/tar_builder.py
--rw-r--r--   0        0        0      358 2023-04-16 02:13:19.092756 nsk_backupr-0.2.0/backupr/util.py
--rw-r--r--   0        0        0     1010 2023-04-16 19:48:31.626554 nsk_backupr-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 nsk_backupr-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-08 19:28:12.037129 nsk_backupr-0.2.1/LICENSE
+-rw-r--r--   0        0        0      341 2023-04-09 06:01:26.289658 nsk_backupr-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-08 19:28:12.037129 nsk_backupr-0.2.1/backupr/__init__.py
+-rw-r--r--   0        0        0     1077 2023-04-11 04:28:23.044836 nsk_backupr-0.2.1/backupr/cli.py
+-rw-r--r--   0        0        0     5971 2023-04-16 14:59:06.822141 nsk_backupr-0.2.1/backupr/config.py
+-rw-r--r--   0        0        0      687 2023-04-11 04:28:23.044836 nsk_backupr-0.2.1/backupr/di.py
+-rw-r--r--   0        0        0     2652 2023-04-16 01:59:04.406086 nsk_backupr-0.2.1/backupr/encrypter.py
+-rw-r--r--   0        0        0     6363 2023-04-16 01:59:04.406086 nsk_backupr-0.2.1/backupr/engine.py
+-rw-r--r--   0        0        0     1830 2023-04-08 19:28:12.037129 nsk_backupr-0.2.1/backupr/storage_provider/__init__.py
+-rw-r--r--   0        0        0     2815 2023-04-11 00:35:47.611849 nsk_backupr-0.2.1/backupr/storage_provider/b2_provider.py
+-rw-r--r--   0        0        0     1028 2023-04-08 19:28:12.037129 nsk_backupr-0.2.1/backupr/storage_provider/local_provider.py
+-rw-r--r--   0        0        0     2265 2023-04-11 04:28:23.044836 nsk_backupr-0.2.1/backupr/tar_builder.py
+-rw-r--r--   0        0        0      358 2023-04-16 02:13:19.092756 nsk_backupr-0.2.1/backupr/util.py
+-rw-r--r--   0        0        0     1010 2023-04-16 19:52:18.468321 nsk_backupr-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 nsk_backupr-0.2.1/PKG-INFO
```

### Comparing `nsk_backupr-0.2.0/LICENSE` & `nsk_backupr-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nsk_backupr-0.2.0/backupr/cli.py` & `nsk_backupr-0.2.1/backupr/cli.py`

 * *Files identical despite different names*

### Comparing `nsk_backupr-0.2.0/backupr/config.py` & `nsk_backupr-0.2.1/backupr/config.py`

 * *Files identical despite different names*

### Comparing `nsk_backupr-0.2.0/backupr/di.py` & `nsk_backupr-0.2.1/backupr/di.py`

 * *Files identical despite different names*

### Comparing `nsk_backupr-0.2.0/backupr/encrypter.py` & `nsk_backupr-0.2.1/backupr/encrypter.py`

 * *Files identical despite different names*

### Comparing `nsk_backupr-0.2.0/backupr/engine.py` & `nsk_backupr-0.2.1/backupr/engine.py`

 * *Files identical despite different names*

### Comparing `nsk_backupr-0.2.0/backupr/storage_provider/__init__.py` & `nsk_backupr-0.2.1/backupr/storage_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `nsk_backupr-0.2.0/backupr/storage_provider/b2_provider.py` & `nsk_backupr-0.2.1/backupr/storage_provider/b2_provider.py`

 * *Files identical despite different names*

### Comparing `nsk_backupr-0.2.0/backupr/storage_provider/local_provider.py` & `nsk_backupr-0.2.1/backupr/storage_provider/local_provider.py`

 * *Files identical despite different names*

### Comparing `nsk_backupr-0.2.0/backupr/tar_builder.py` & `nsk_backupr-0.2.1/backupr/tar_builder.py`

 * *Files identical despite different names*

### Comparing `nsk_backupr-0.2.0/pyproject.toml` & `nsk_backupr-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nsk-backupr"
-version = "0.2.0"
+version = "0.2.1"
 description = "A backup runner designed to tar up a root directory, optionally encrypt it, and upload to remote storage."
 authors = ["Erik Nelson <erik@nsk.io>"]
 readme = "README.md"
 packages = [
   { include = "backupr" }
 ]
```

### Comparing `nsk_backupr-0.2.0/PKG-INFO` & `nsk_backupr-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsk-backupr
-Version: 0.2.0
+Version: 0.2.1
 Summary: A backup runner designed to tar up a root directory, optionally encrypt it, and upload to remote storage.
 Author: Erik Nelson
 Author-email: erik@nsk.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

