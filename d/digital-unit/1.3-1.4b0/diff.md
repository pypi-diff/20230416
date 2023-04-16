# Comparing `tmp/digital_unit-1.3.tar.gz` & `tmp/digital_unit-1.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital_unit-1.3.tar", last modified: Sun Apr 16 06:36:10 2023, max compression
+gzip compressed data, was "digital_unit-1.4b0.tar", last modified: Sun Apr 16 12:32:36 2023, max compression
```

## Comparing `digital_unit-1.3.tar` & `digital_unit-1.4b0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 06:36:10.076434 digital_unit-1.3/
--rw-rw-rw-   0        0        0      238 2023-04-16 06:36:10.075446 digital_unit-1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 06:36:10.053434 digital_unit-1.3/digital_unit/
--rw-rw-rw-   0        0        0       30 2023-04-16 06:34:33.000000 digital_unit-1.3/digital_unit/__init__.py
--rw-rw-rw-   0        0        0     2782 2023-04-16 05:02:19.000000 digital_unit-1.3/digital_unit/lib.py
-drwxrwxrwx   0        0        0        0 2023-04-16 06:36:10.071434 digital_unit-1.3/digital_unit.egg-info/
--rw-rw-rw-   0        0        0      238 2023-04-16 06:36:09.000000 digital_unit-1.3/digital_unit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-04-16 06:36:09.000000 digital_unit-1.3/digital_unit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 06:36:09.000000 digital_unit-1.3/digital_unit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-16 06:36:09.000000 digital_unit-1.3/digital_unit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 06:36:10.076434 digital_unit-1.3/setup.cfg
--rw-rw-rw-   0        0        0      774 2023-04-16 06:35:48.000000 digital_unit-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:36.248702 digital_unit-1.4b0/
+-rw-rw-rw-   0        0        0      240 2023-04-16 12:32:36.245684 digital_unit-1.4b0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:36.217687 digital_unit-1.4b0/digital_unit/
+-rw-rw-rw-   0        0        0      146 2023-04-16 12:31:35.000000 digital_unit-1.4b0/digital_unit/__init__.py
+-rw-rw-rw-   0        0        0      313 2023-04-16 12:25:29.000000 digital_unit-1.4b0/digital_unit/sample.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:36.237706 digital_unit-1.4b0/digital_unit.egg-info/
+-rw-rw-rw-   0        0        0      240 2023-04-16 12:32:36.000000 digital_unit-1.4b0/digital_unit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-04-16 12:32:36.000000 digital_unit-1.4b0/digital_unit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 12:32:36.000000 digital_unit-1.4b0/digital_unit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-16 12:32:36.000000 digital_unit-1.4b0/digital_unit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 12:32:36.248702 digital_unit-1.4b0/setup.cfg
+-rw-rw-rw-   0        0        0      779 2023-04-16 12:32:22.000000 digital_unit-1.4b0/setup.py
```

### Comparing `digital_unit-1.3/setup.py` & `digital_unit-1.4b0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'digital_unit',         # How you named your package folder (MyLib)
   packages = ['digital_unit'],   # Chose the same as "name"
-  version = '1.3',      # Start with a small number and increase it with every change you make
+  version = '1.4.beta',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'number and units',   # Give a short description about your library
   author = 'st201109',                   # Type in your name
   author_email = 'st20110913@outlook.com',      # Type in your E-Mail
   
   keywords = ['SOME', 'MEANINGFULL', 'MATH'],   # Keywords that define your package best
```

