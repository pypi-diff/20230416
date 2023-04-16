# Comparing `tmp/pyfobal-0.1.0.tar.gz` & `tmp/pyfobal-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfobal-0.1.0.tar", last modified: Sun Apr 16 16:31:26 2023, max compression
+gzip compressed data, was "pyfobal-0.1.1.tar", last modified: Sun Apr 16 18:01:03 2023, max compression
```

## Comparing `pyfobal-0.1.0.tar` & `pyfobal-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:31:26.506355 pyfobal-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-16 16:31:26.506355 pyfobal-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:31:13.000000 pyfobal-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:31:26.506355 pyfobal-0.1.0/fobal_types/
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-16 16:31:13.000000 pyfobal-0.1.0/fobal_types/League.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:31:13.000000 pyfobal-0.1.0/fobal_types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:31:26.506355 pyfobal-0.1.0/pyfobal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-16 16:31:26.000000 pyfobal-0.1.0/pyfobal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-16 16:31:26.000000 pyfobal-0.1.0/pyfobal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:31:26.000000 pyfobal-0.1.0/pyfobal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-16 16:31:26.000000 pyfobal-0.1.0/pyfobal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 16:31:26.000000 pyfobal-0.1.0/pyfobal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 16:31:26.506355 pyfobal-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-16 16:31:13.000000 pyfobal-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:01:03.927321 pyfobal-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-16 18:01:03.927321 pyfobal-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:00:53.000000 pyfobal-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:01:03.927321 pyfobal-0.1.1/fobal_types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-16 18:00:53.000000 pyfobal-0.1.1/fobal_types/League.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:00:53.000000 pyfobal-0.1.1/fobal_types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:01:03.927321 pyfobal-0.1.1/pyfobal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-04-16 18:01:03.000000 pyfobal-0.1.1/pyfobal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-16 18:01:03.000000 pyfobal-0.1.1/pyfobal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 18:01:03.000000 pyfobal-0.1.1/pyfobal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-16 18:01:03.000000 pyfobal-0.1.1/pyfobal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 18:01:03.000000 pyfobal-0.1.1/pyfobal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 18:01:03.927321 pyfobal-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-16 18:00:53.000000 pyfobal-0.1.1/setup.py
```

### Comparing `pyfobal-0.1.0/fobal_types/League.py` & `pyfobal-0.1.1/fobal_types/League.py`

 * *Files identical despite different names*

### Comparing `pyfobal-0.1.0/setup.py` & `pyfobal-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="pyfobal",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[
         "requests",
     ],
     author="Karis Omotosho",
     author_email="karomo.sm@gmail.com",
     description="A Python SDK for the Fobal API",
```

