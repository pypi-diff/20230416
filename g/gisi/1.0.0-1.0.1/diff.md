# Comparing `tmp/gisi-1.0.0.tar.gz` & `tmp/gisi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gisi-1.0.0.tar", last modified: Sun Apr 16 19:31:53 2023, max compression
+gzip compressed data, was "gisi-1.0.1.tar", last modified: Sun Apr 16 19:37:04 2023, max compression
```

## Comparing `gisi-1.0.0.tar` & `gisi-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 19:31:53.530076 gisi-1.0.0/
--rw-rw-rw-   0        0        0     1092 2023-04-16 19:22:53.000000 gisi-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      407 2023-04-16 19:31:53.531079 gisi-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      119 2023-04-16 19:23:44.000000 gisi-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 19:31:53.488833 gisi-1.0.0/gisi/
--rw-rw-rw-   0        0        0        0 2023-04-16 19:27:20.000000 gisi-1.0.0/gisi/__init__.py
--rw-rw-rw-   0        0        0      116 2023-04-16 19:11:18.000000 gisi-1.0.0/gisi/bd.py
--rw-rw-rw-   0        0        0      363 2023-04-16 19:07:30.000000 gisi-1.0.0/gisi/dd.py
--rw-rw-rw-   0        0        0      566 2023-04-16 19:13:42.000000 gisi-1.0.0/gisi/gek.py
--rw-rw-rw-   0        0        0     1588 2023-04-16 19:16:46.000000 gisi-1.0.0/gisi/gisi.py
-drwxrwxrwx   0        0        0        0 2023-04-16 19:31:53.521072 gisi-1.0.0/gisi.egg-info/
--rw-rw-rw-   0        0        0      407 2023-04-16 19:31:53.000000 gisi-1.0.0/gisi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-04-16 19:31:53.000000 gisi-1.0.0/gisi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 19:31:53.000000 gisi-1.0.0/gisi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-16 19:31:53.000000 gisi-1.0.0/gisi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 19:31:53.538550 gisi-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      512 2023-04-16 19:27:17.000000 gisi-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 19:37:04.155969 gisi-1.0.1/
+-rw-rw-rw-   0        0        0     1092 2023-04-16 19:22:53.000000 gisi-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      407 2023-04-16 19:37:04.155969 gisi-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      119 2023-04-16 19:23:44.000000 gisi-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 19:37:04.118262 gisi-1.0.1/gisi/
+-rw-rw-rw-   0        0        0        0 2023-04-16 19:27:20.000000 gisi-1.0.1/gisi/__init__.py
+-rw-rw-rw-   0        0        0      116 2023-04-16 19:11:18.000000 gisi-1.0.1/gisi/bd.py
+-rw-rw-rw-   0        0        0      363 2023-04-16 19:07:30.000000 gisi-1.0.1/gisi/dd.py
+-rw-rw-rw-   0        0        0      566 2023-04-16 19:13:42.000000 gisi-1.0.1/gisi/gek.py
+-rw-rw-rw-   0        0        0     1603 2023-04-16 19:35:59.000000 gisi-1.0.1/gisi/gisi.py
+drwxrwxrwx   0        0        0        0 2023-04-16 19:37:04.152248 gisi-1.0.1/gisi.egg-info/
+-rw-rw-rw-   0        0        0      407 2023-04-16 19:37:03.000000 gisi-1.0.1/gisi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-04-16 19:37:03.000000 gisi-1.0.1/gisi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 19:37:03.000000 gisi-1.0.1/gisi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-16 19:37:03.000000 gisi-1.0.1/gisi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 19:37:04.160753 gisi-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      512 2023-04-16 19:36:17.000000 gisi-1.0.1/setup.py
```

### Comparing `gisi-1.0.0/LICENSE` & `gisi-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gisi-1.0.0/gisi/gek.py` & `gisi-1.0.1/gisi/gek.py`

 * *Files identical despite different names*

### Comparing `gisi-1.0.0/gisi/gisi.py` & `gisi-1.0.1/gisi/gisi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from gek import gek
-from bd import bd
-from dd import dd
+from gisi.gek import gek
+from gisi.bd import bd
+from gisi.dd import dd
 import sqlite3
 import shutil
 import os
 
 
 def gisi():
     try:
```

