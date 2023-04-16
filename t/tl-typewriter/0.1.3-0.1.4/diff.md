# Comparing `tmp/tl_typewriter-0.1.3.tar.gz` & `tmp/tl_typewriter-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tl_typewriter-0.1.3.tar", last modified: Sun Apr 16 07:37:39 2023, max compression
+gzip compressed data, was "tl_typewriter-0.1.4.tar", last modified: Sun Apr 16 07:40:57 2023, max compression
```

## Comparing `tl_typewriter-0.1.3.tar` & `tl_typewriter-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 07:37:39.498596 tl_typewriter-0.1.3/
--rw-rw-rw-   0        0        0    11558 2023-04-16 06:54:47.000000 tl_typewriter-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      302 2023-04-16 07:37:39.498596 tl_typewriter-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      478 2023-04-16 07:18:45.000000 tl_typewriter-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-16 07:37:39.498596 tl_typewriter-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      670 2023-04-16 07:37:24.000000 tl_typewriter-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:37:39.486603 tl_typewriter-0.1.3/tl_typewriter/
--rw-rw-rw-   0        0        0     1724 2023-04-16 07:36:48.000000 tl_typewriter-0.1.3/tl_typewriter/tl_typewriter.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:37:39.497596 tl_typewriter-0.1.3/tl_typewriter.egg-info/
--rw-rw-rw-   0        0        0      302 2023-04-16 07:37:39.000000 tl_typewriter-0.1.3/tl_typewriter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-04-16 07:37:39.000000 tl_typewriter-0.1.3/tl_typewriter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 07:37:39.000000 tl_typewriter-0.1.3/tl_typewriter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-16 07:37:39.000000 tl_typewriter-0.1.3/tl_typewriter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-04-16 07:37:39.000000 tl_typewriter-0.1.3/tl_typewriter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-16 07:37:39.000000 tl_typewriter-0.1.3/tl_typewriter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 07:40:57.897557 tl_typewriter-0.1.4/
+-rw-rw-rw-   0        0        0    11558 2023-04-16 06:54:47.000000 tl_typewriter-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      302 2023-04-16 07:40:57.897557 tl_typewriter-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2023-04-16 07:18:45.000000 tl_typewriter-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-16 07:40:57.897557 tl_typewriter-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      670 2023-04-16 07:40:52.000000 tl_typewriter-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 07:40:57.885024 tl_typewriter-0.1.4/tl_typewriter/
+-rw-rw-rw-   0        0        0     1724 2023-04-16 07:36:48.000000 tl_typewriter-0.1.4/tl_typewriter/tl_typewriter.py
+drwxrwxrwx   0        0        0        0 2023-04-16 07:40:57.896562 tl_typewriter-0.1.4/tl_typewriter.egg-info/
+-rw-rw-rw-   0        0        0      302 2023-04-16 07:40:57.000000 tl_typewriter-0.1.4/tl_typewriter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-04-16 07:40:57.000000 tl_typewriter-0.1.4/tl_typewriter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 07:40:57.000000 tl_typewriter-0.1.4/tl_typewriter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-16 07:40:57.000000 tl_typewriter-0.1.4/tl_typewriter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-04-16 07:40:57.000000 tl_typewriter-0.1.4/tl_typewriter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-16 07:40:57.000000 tl_typewriter-0.1.4/tl_typewriter.egg-info/top_level.txt
```

### Comparing `tl_typewriter-0.1.3/LICENSE` & `tl_typewriter-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tl_typewriter-0.1.3/setup.py` & `tl_typewriter-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 from setuptools import setup
 
 
 setup(
     name="tl_typewriter",
-    version='0.1.3',
+    version='0.1.4',
     description="pagination and bubble typewriter in translating manga",
     url="https://github.com/AbangTanYiHan/tl_typewriter",
     author="abangtan",
     license="Apache License 2.0",
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
```

### Comparing `tl_typewriter-0.1.3/tl_typewriter/tl_typewriter.py` & `tl_typewriter-0.1.4/tl_typewriter/tl_typewriter.py`

 * *Files identical despite different names*

