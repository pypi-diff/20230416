# Comparing `tmp/tl_typewriter-0.1.7.tar.gz` & `tmp/tl_typewriter-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tl_typewriter-0.1.7.tar", last modified: Sun Apr 16 08:17:18 2023, max compression
+gzip compressed data, was "tl_typewriter-0.1.8.tar", last modified: Sun Apr 16 08:19:13 2023, max compression
```

## Comparing `tl_typewriter-0.1.7.tar` & `tl_typewriter-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 08:17:18.692026 tl_typewriter-0.1.7/
--rw-rw-rw-   0        0        0    11558 2023-04-16 06:54:47.000000 tl_typewriter-0.1.7/LICENSE
--rw-rw-rw-   0        0        0      302 2023-04-16 08:17:18.691017 tl_typewriter-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      478 2023-04-16 07:18:45.000000 tl_typewriter-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2023-04-16 08:17:18.692026 tl_typewriter-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      665 2023-04-16 08:10:20.000000 tl_typewriter-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:17:18.681856 tl_typewriter-0.1.7/tl_typewriter/
--rw-rw-rw-   0        0        0     1724 2023-04-16 08:09:50.000000 tl_typewriter-0.1.7/tl_typewriter/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:17:18.690011 tl_typewriter-0.1.7/tl_typewriter.egg-info/
--rw-rw-rw-   0        0        0      302 2023-04-16 08:17:18.000000 tl_typewriter-0.1.7/tl_typewriter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-04-16 08:17:18.000000 tl_typewriter-0.1.7/tl_typewriter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 08:17:18.000000 tl_typewriter-0.1.7/tl_typewriter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-04-16 08:17:18.000000 tl_typewriter-0.1.7/tl_typewriter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-04-16 08:17:18.000000 tl_typewriter-0.1.7/tl_typewriter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-16 08:17:18.000000 tl_typewriter-0.1.7/tl_typewriter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 08:19:13.972407 tl_typewriter-0.1.8/
+-rw-rw-rw-   0        0        0    11558 2023-04-16 06:54:47.000000 tl_typewriter-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0      302 2023-04-16 08:19:13.972407 tl_typewriter-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-04-16 08:18:09.000000 tl_typewriter-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-16 08:19:13.972407 tl_typewriter-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      665 2023-04-16 08:18:36.000000 tl_typewriter-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 08:19:13.959232 tl_typewriter-0.1.8/tl_typewriter/
+-rw-rw-rw-   0        0        0     1724 2023-04-16 08:09:50.000000 tl_typewriter-0.1.8/tl_typewriter/__main__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 08:19:13.971404 tl_typewriter-0.1.8/tl_typewriter.egg-info/
+-rw-rw-rw-   0        0        0      302 2023-04-16 08:19:13.000000 tl_typewriter-0.1.8/tl_typewriter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-04-16 08:19:13.000000 tl_typewriter-0.1.8/tl_typewriter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 08:19:13.000000 tl_typewriter-0.1.8/tl_typewriter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-04-16 08:19:13.000000 tl_typewriter-0.1.8/tl_typewriter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-04-16 08:19:13.000000 tl_typewriter-0.1.8/tl_typewriter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-16 08:19:13.000000 tl_typewriter-0.1.8/tl_typewriter.egg-info/top_level.txt
```

### Comparing `tl_typewriter-0.1.7/LICENSE` & `tl_typewriter-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tl_typewriter-0.1.7/setup.py` & `tl_typewriter-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from setuptools import setup
 
 
 setup(
     name="tl_typewriter",
-    version='0.1.7',
+    version='0.1.8',
     description="pagination and bubble typewriter in translating manga",
     url="https://github.com/AbangTanYiHan/tl_typewriter",
     author="abangtan",
     license="Apache License 2.0",
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
```

### Comparing `tl_typewriter-0.1.7/tl_typewriter/__main__.py` & `tl_typewriter-0.1.8/tl_typewriter/__main__.py`

 * *Files identical despite different names*

