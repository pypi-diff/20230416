# Comparing `tmp/pygameHat-1.0.7.tar.gz` & `tmp/pygameHat-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygameHat-1.0.7.tar", last modified: Tue Apr 11 11:09:22 2023, max compression
+gzip compressed data, was "pygameHat-1.0.8.tar", last modified: Sun Apr 16 16:46:00 2023, max compression
```

## Comparing `pygameHat-1.0.7.tar` & `pygameHat-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 11:09:22.695850 pygameHat-1.0.7/
--rw-rw-rw-   0        0        0       78 2023-03-19 17:10:47.000000 pygameHat-1.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      544 2023-04-11 11:09:22.691784 pygameHat-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-11 11:09:22.595837 pygameHat-1.0.7/pygameHat/
--rw-rw-rw-   0        0        0    37874 2023-04-11 10:14:26.000000 pygameHat-1.0.7/pygameHat/__init__.py
--rw-rw-rw-   0        0        0       41 2023-03-19 17:43:54.000000 pygameHat-1.0.7/pygameHat/pygameHat.py
-drwxrwxrwx   0        0        0        0 2023-04-11 11:09:22.684804 pygameHat-1.0.7/pygameHat.egg-info/
--rw-rw-rw-   0        0        0      544 2023-04-11 11:09:21.000000 pygameHat-1.0.7/pygameHat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-04-11 11:09:21.000000 pygameHat-1.0.7/pygameHat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 11:09:21.000000 pygameHat-1.0.7/pygameHat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-11 11:09:21.000000 pygameHat-1.0.7/pygameHat.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-11 11:09:21.000000 pygameHat-1.0.7/pygameHat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-11 11:09:22.695850 pygameHat-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      726 2023-04-11 11:09:12.000000 pygameHat-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:46:00.219011 pygameHat-1.0.8/
+-rw-rw-rw-   0        0        0      549 2023-04-16 16:46:00.214986 pygameHat-1.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 16:46:00.206002 pygameHat-1.0.8/pygameHat.egg-info/
+-rw-rw-rw-   0        0        0      549 2023-04-16 16:46:00.000000 pygameHat-1.0.8/pygameHat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-04-16 16:46:00.000000 pygameHat-1.0.8/pygameHat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 16:46:00.000000 pygameHat-1.0.8/pygameHat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-16 16:46:00.000000 pygameHat-1.0.8/pygameHat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 16:46:00.000000 pygameHat-1.0.8/pygameHat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 16:46:00.219011 pygameHat-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      719 2023-04-16 16:39:34.000000 pygameHat-1.0.8/setup.py
```

### Comparing `pygameHat-1.0.7/PKG-INFO` & `pygameHat-1.0.8/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.1
 Name: pygameHat
-Version: 1.0.7
-Summary: Pygame game-making engine
+Version: 1.0.8
+Summary: pygame game-making engine
 Home-page: UNKNOWN
 Author: Wojciech Błajda
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
-Keywords: python,engine,pygame,game,maker
+Keywords: python,pygame,game,engine,maker,tool
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pygameHat-1.0.7/pygameHat.egg-info/PKG-INFO` & `pygameHat-1.0.8/pygameHat.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.1
 Name: pygameHat
-Version: 1.0.7
-Summary: Pygame game-making engine
+Version: 1.0.8
+Summary: pygame game-making engine
 Home-page: UNKNOWN
 Author: Wojciech Błajda
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
-Keywords: python,engine,pygame,game,maker
+Keywords: python,pygame,game,engine,maker,tool
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `pygameHat-1.0.7/setup.py` & `pygameHat-1.0.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.0.7'
-DESCRIPTION = 'Pygame game-making engine'
+VERSION = '1.0.8'
+DESCRIPTION = 'pygame game-making engine'
 
 # Setting up
 setup(
     name="pygameHat",
     version=VERSION,
     author="Wojciech Błajda",
-    #author_email="None",
+    #author_email="<mail@neuralnine.com>",
     description=DESCRIPTION,
-    packages=find_packages(),
     install_requires=['pygame'],
-    keywords=['python', 'engine', 'pygame', 'game', 'maker'],
+    keywords=['python', 'pygame', 'game', 'engine', 'maker', 'tool'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
-    ],
+    ]
 )
```

