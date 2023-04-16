# Comparing `tmp/digital_unit-1.0.tar.gz` & `tmp/digital_unit-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital_unit-1.0.tar", last modified: Sun Apr 16 06:05:17 2023, max compression
+gzip compressed data, was "digital_unit-1.1.tar", last modified: Sun Apr 16 06:22:46 2023, max compression
```

## Comparing `digital_unit-1.0.tar` & `digital_unit-1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 06:05:17.089779 digital_unit-1.0/
--rw-rw-rw-   0        0        0      238 2023-04-16 06:05:17.087773 digital_unit-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 06:05:17.069774 digital_unit-1.0/digital_unit/
--rw-rw-rw-   0        0        0      115 2023-04-16 05:25:20.000000 digital_unit-1.0/digital_unit/__init__.py
--rw-rw-rw-   0        0        0     2782 2023-04-16 05:02:19.000000 digital_unit-1.0/digital_unit/digital_unit.py
-drwxrwxrwx   0        0        0        0 2023-04-16 06:05:17.084774 digital_unit-1.0/digital_unit.egg-info/
--rw-rw-rw-   0        0        0      238 2023-04-16 06:05:16.000000 digital_unit-1.0/digital_unit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-04-16 06:05:16.000000 digital_unit-1.0/digital_unit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 06:05:16.000000 digital_unit-1.0/digital_unit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-16 06:05:16.000000 digital_unit-1.0/digital_unit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 06:05:17.089779 digital_unit-1.0/setup.cfg
--rw-rw-rw-   0        0        0      774 2023-04-16 06:05:11.000000 digital_unit-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 06:22:46.852226 digital_unit-1.1/
+-rw-rw-rw-   0        0        0      238 2023-04-16 06:22:46.851228 digital_unit-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 06:22:46.829227 digital_unit-1.1/digital_unit/
+-rw-rw-rw-   0        0        0      106 2023-04-16 06:16:09.000000 digital_unit-1.1/digital_unit/__init__.py
+-rw-rw-rw-   0        0        0     2782 2023-04-16 05:02:19.000000 digital_unit-1.1/digital_unit/lib.py
+drwxrwxrwx   0        0        0        0 2023-04-16 06:22:46.846227 digital_unit-1.1/digital_unit.egg-info/
+-rw-rw-rw-   0        0        0      238 2023-04-16 06:22:46.000000 digital_unit-1.1/digital_unit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-04-16 06:22:46.000000 digital_unit-1.1/digital_unit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 06:22:46.000000 digital_unit-1.1/digital_unit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-16 06:22:46.000000 digital_unit-1.1/digital_unit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 06:22:46.857360 digital_unit-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      774 2023-04-16 06:22:39.000000 digital_unit-1.1/setup.py
```

### Comparing `digital_unit-1.0/digital_unit/digital_unit.py` & `digital_unit-1.1/digital_unit/lib.py`

 * *Files identical despite different names*

### Comparing `digital_unit-1.0/setup.py` & `digital_unit-1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'digital_unit',         # How you named your package folder (MyLib)
   packages = ['digital_unit'],   # Chose the same as "name"
-  version = '1.0',      # Start with a small number and increase it with every change you make
+  version = '1.1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'number and units',   # Give a short description about your library
   author = 'st201109',                   # Type in your name
   author_email = 'st20110913@outlook.com',      # Type in your E-Mail
   
   keywords = ['SOME', 'MEANINGFULL', 'MATH'],   # Keywords that define your package best
```

