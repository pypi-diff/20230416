# Comparing `tmp/randgenlib-1.0.3.tar.gz` & `tmp/randgenlib-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "randgenlib-1.0.3.tar", last modified: Sun Apr 16 12:24:33 2023, max compression
+gzip compressed data, was "randgenlib-1.0.4.tar", last modified: Sun Apr 16 12:44:55 2023, max compression
```

## Comparing `randgenlib-1.0.3.tar` & `randgenlib-1.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:24:33.485101 randgenlib-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      325 2023-04-16 12:24:33.485101 randgenlib-1.0.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:24:33.485101 randgenlib-1.0.3/randgenlib/
--rw-r--r--   0 root         (0) root         (0)   148961 2023-04-16 12:24:32.000000 randgenlib-1.0.3/randgenlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:24:33.485101 randgenlib-1.0.3/randgenlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      325 2023-04-16 12:24:33.000000 randgenlib-1.0.3/randgenlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      167 2023-04-16 12:24:33.000000 randgenlib-1.0.3/randgenlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 12:24:33.000000 randgenlib-1.0.3/randgenlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-16 12:24:33.000000 randgenlib-1.0.3/randgenlib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 12:24:33.485101 randgenlib-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      538 2023-04-16 12:24:32.000000 randgenlib-1.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:44:55.961778 randgenlib-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)      339 2023-04-16 12:44:55.961778 randgenlib-1.0.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:44:55.961778 randgenlib-1.0.4/randgenlib/
+-rw-r--r--   0 root         (0) root         (0)    82161 2023-04-16 12:44:55.000000 randgenlib-1.0.4/randgenlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:44:55.961778 randgenlib-1.0.4/randgenlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      339 2023-04-16 12:44:55.000000 randgenlib-1.0.4/randgenlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      167 2023-04-16 12:44:55.000000 randgenlib-1.0.4/randgenlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 12:44:55.000000 randgenlib-1.0.4/randgenlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-16 12:44:55.000000 randgenlib-1.0.4/randgenlib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 12:44:55.961778 randgenlib-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      552 2023-04-16 12:44:54.000000 randgenlib-1.0.4/setup.py
```

### Comparing `randgenlib-1.0.3/setup.py` & `randgenlib-1.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.3'
-DESCRIPTION = "Random gen lib"
-LONG_DESCRIPTION = "Random gen lib"
+VERSION = '1.0.4'
+DESCRIPTION = "Random generation lib"
+LONG_DESCRIPTION = "Random generation lib"
 
 # Setting up
 setup(
     name="randgenlib",
     version=VERSION,
     author="GigaAlex",
     author_email="nick.faltermeier@gmx.de",
```

