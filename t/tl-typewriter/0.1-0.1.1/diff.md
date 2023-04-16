# Comparing `tmp/tl_typewriter-0.1.tar.gz` & `tmp/tl_typewriter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tl_typewriter-0.1.tar", last modified: Sun Apr 16 07:00:44 2023, max compression
+gzip compressed data, was "tl_typewriter-0.1.1.tar", last modified: Sun Apr 16 07:15:55 2023, max compression
```

## Comparing `tl_typewriter-0.1.tar` & `tl_typewriter-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 07:00:44.588213 tl_typewriter-0.1/
--rw-rw-rw-   0        0        0    11558 2023-04-16 06:54:47.000000 tl_typewriter-0.1/LICENSE
--rw-rw-rw-   0        0        0      313 2023-04-16 07:00:44.587206 tl_typewriter-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      309 2023-04-16 06:59:49.000000 tl_typewriter-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-16 07:00:44.588213 tl_typewriter-0.1/setup.cfg
--rw-rw-rw-   0        0        0      801 2023-04-16 07:00:42.000000 tl_typewriter-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:00:44.570228 tl_typewriter-0.1/tl_typewriter/
--rw-rw-rw-   0        0        0     1554 2023-04-16 06:56:19.000000 tl_typewriter-0.1/tl_typewriter/tl_typewriter.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:00:44.586115 tl_typewriter-0.1/tl_typewriter.egg-info/
--rw-rw-rw-   0        0        0      313 2023-04-16 07:00:44.000000 tl_typewriter-0.1/tl_typewriter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-04-16 07:00:44.000000 tl_typewriter-0.1/tl_typewriter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 07:00:44.000000 tl_typewriter-0.1/tl_typewriter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-16 07:00:44.000000 tl_typewriter-0.1/tl_typewriter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-04-16 07:00:44.000000 tl_typewriter-0.1/tl_typewriter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-16 07:00:44.000000 tl_typewriter-0.1/tl_typewriter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 07:15:55.192354 tl_typewriter-0.1.1/
+-rw-rw-rw-   0        0        0    11558 2023-04-16 06:54:47.000000 tl_typewriter-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      326 2023-04-16 07:15:55.191343 tl_typewriter-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2023-04-16 07:06:14.000000 tl_typewriter-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-16 07:15:55.192354 tl_typewriter-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      814 2023-04-16 07:15:24.000000 tl_typewriter-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 07:15:55.179326 tl_typewriter-0.1.1/tl_typewriter/
+-rw-rw-rw-   0        0        0     1554 2023-04-16 06:56:19.000000 tl_typewriter-0.1.1/tl_typewriter/tl_typewriter.py
+drwxrwxrwx   0        0        0        0 2023-04-16 07:15:55.190344 tl_typewriter-0.1.1/tl_typewriter.egg-info/
+-rw-rw-rw-   0        0        0      326 2023-04-16 07:15:55.000000 tl_typewriter-0.1.1/tl_typewriter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-04-16 07:15:55.000000 tl_typewriter-0.1.1/tl_typewriter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 07:15:55.000000 tl_typewriter-0.1.1/tl_typewriter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-16 07:15:55.000000 tl_typewriter-0.1.1/tl_typewriter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-04-16 07:15:55.000000 tl_typewriter-0.1.1/tl_typewriter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-16 07:15:55.000000 tl_typewriter-0.1.1/tl_typewriter.egg-info/top_level.txt
```

### Comparing `tl_typewriter-0.1/LICENSE` & `tl_typewriter-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tl_typewriter-0.1/setup.py` & `tl_typewriter-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from pathlib import Path
 from setuptools import setup
 
 long_description = (Path(__file__).parent / "README.md").read_text('utf-8').split('# Installation')[0]
 
 setup(
     name="tl_typewriter",
-    version='0.1',
+    version='0.1.1',
     description="pagination and bubble typewriter in translating manga",
     long_description=long_description,
-    url="https://github.com/AbangTanYiHan/tl",
+    url="https://github.com/AbangTanYiHan/tl_typewriter",
     author="abangtan",
     license="Apache License 2.0",
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
     packages=['tl_typewriter'],
     include_package_data=True,
```

### Comparing `tl_typewriter-0.1/tl_typewriter/tl_typewriter.py` & `tl_typewriter-0.1.1/tl_typewriter/tl_typewriter.py`

 * *Files identical despite different names*

