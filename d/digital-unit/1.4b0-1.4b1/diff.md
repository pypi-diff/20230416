# Comparing `tmp/digital_unit-1.4b0.tar.gz` & `tmp/digital_unit-1.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digital_unit-1.4b0.tar", last modified: Sun Apr 16 12:32:36 2023, max compression
+gzip compressed data, was "digital_unit-1.4b1.tar", last modified: Sun Apr 16 13:28:42 2023, max compression
```

## Comparing `digital_unit-1.4b0.tar` & `digital_unit-1.4b1.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 12:32:36.248702 digital_unit-1.4b0/
--rw-rw-rw-   0        0        0      240 2023-04-16 12:32:36.245684 digital_unit-1.4b0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 12:32:36.217687 digital_unit-1.4b0/digital_unit/
--rw-rw-rw-   0        0        0      146 2023-04-16 12:31:35.000000 digital_unit-1.4b0/digital_unit/__init__.py
--rw-rw-rw-   0        0        0      313 2023-04-16 12:25:29.000000 digital_unit-1.4b0/digital_unit/sample.py
-drwxrwxrwx   0        0        0        0 2023-04-16 12:32:36.237706 digital_unit-1.4b0/digital_unit.egg-info/
--rw-rw-rw-   0        0        0      240 2023-04-16 12:32:36.000000 digital_unit-1.4b0/digital_unit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-04-16 12:32:36.000000 digital_unit-1.4b0/digital_unit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 12:32:36.000000 digital_unit-1.4b0/digital_unit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-16 12:32:36.000000 digital_unit-1.4b0/digital_unit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 12:32:36.248702 digital_unit-1.4b0/setup.cfg
--rw-rw-rw-   0        0        0      779 2023-04-16 12:32:22.000000 digital_unit-1.4b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:28:42.198014 digital_unit-1.4b1/
+-rw-rw-rw-   0        0        0      240 2023-04-16 13:28:42.197025 digital_unit-1.4b1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 13:28:42.176018 digital_unit-1.4b1/digital_unit/
+-rw-rw-rw-   0        0        0      826 2023-04-16 12:38:40.000000 digital_unit-1.4b1/digital_unit/Area.py
+-rw-rw-rw-   0        0        0      796 2023-04-16 12:38:36.000000 digital_unit-1.4b1/digital_unit/Lenth.py
+-rw-rw-rw-   0        0        0      134 2023-04-16 13:27:44.000000 digital_unit-1.4b1/digital_unit/__init__.py
+-rw-rw-rw-   0        0        0      976 2023-04-16 12:22:16.000000 digital_unit-1.4b1/digital_unit/root.py
+-rw-rw-rw-   0        0        0      305 2023-04-16 13:27:53.000000 digital_unit-1.4b1/digital_unit/sample.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:28:42.193013 digital_unit-1.4b1/digital_unit.egg-info/
+-rw-rw-rw-   0        0        0      240 2023-04-16 13:28:42.000000 digital_unit-1.4b1/digital_unit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-04-16 13:28:42.000000 digital_unit-1.4b1/digital_unit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 13:28:42.000000 digital_unit-1.4b1/digital_unit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-04-16 13:28:42.000000 digital_unit-1.4b1/digital_unit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 13:28:42.198014 digital_unit-1.4b1/setup.cfg
+-rw-rw-rw-   0        0        0      776 2023-04-16 13:24:25.000000 digital_unit-1.4b1/setup.py
```

### Comparing `digital_unit-1.4b0/setup.py` & `digital_unit-1.4b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'digital_unit',         # How you named your package folder (MyLib)
   packages = ['digital_unit'],   # Chose the same as "name"
-  version = '1.4.beta',      # Start with a small number and increase it with every change you make
+  version = '1.4b1',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'number and units',   # Give a short description about your library
   author = 'st201109',                   # Type in your name
   author_email = 'st20110913@outlook.com',      # Type in your E-Mail
   
   keywords = ['SOME', 'MEANINGFULL', 'MATH'],   # Keywords that define your package best
```

