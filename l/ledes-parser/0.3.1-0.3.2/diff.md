# Comparing `tmp/ledes-parser-0.3.1.tar.gz` & `tmp/ledes-parser-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ledes-parser-0.3.1.tar", last modified: Sun Apr 16 03:20:34 2023, max compression
+gzip compressed data, was "ledes-parser-0.3.2.tar", last modified: Sun Apr 16 03:33:25 2023, max compression
```

## Comparing `ledes-parser-0.3.1.tar` & `ledes-parser-0.3.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:20:34.389090 ledes-parser-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-16 03:20:19.000000 ledes-parser-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-16 03:20:34.389090 ledes-parser-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-16 03:20:19.000000 ledes-parser-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:20:34.389090 ledes-parser-0.3.1/ledes_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-16 03:20:19.000000 ledes-parser-0.3.1/ledes_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-16 03:20:19.000000 ledes-parser-0.3.1/ledes_parser/base_ledes_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-16 03:20:19.000000 ledes-parser-0.3.1/ledes_parser/ledes_1998BI_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-16 03:20:19.000000 ledes-parser-0.3.1/ledes_parser/ledes_1998B_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-16 03:20:19.000000 ledes-parser-0.3.1/ledes_parser/ledes_1998_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-16 03:20:19.000000 ledes-parser-0.3.1/ledes_parser/ledes_dynamic_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:20:34.389090 ledes-parser-0.3.1/ledes_parser/typings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 03:20:19.000000 ledes-parser-0.3.1/ledes_parser/typings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-16 03:20:19.000000 ledes-parser-0.3.1/ledes_parser/typings/invoice_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:20:34.389090 ledes-parser-0.3.1/ledes_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-16 03:20:34.000000 ledes-parser-0.3.1/ledes_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-16 03:20:34.000000 ledes-parser-0.3.1/ledes_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 03:20:34.000000 ledes-parser-0.3.1/ledes_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-16 03:20:34.000000 ledes-parser-0.3.1/ledes_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 03:20:34.389090 ledes-parser-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-16 03:20:19.000000 ledes-parser-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:20:34.389090 ledes-parser-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 03:20:19.000000 ledes-parser-0.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-16 03:20:19.000000 ledes-parser-0.3.1/tests/test_ledes_1998_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-16 03:20:19.000000 ledes-parser-0.3.1/tests/test_parse_leads_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:33:25.089482 ledes-parser-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-16 03:33:08.000000 ledes-parser-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-16 03:33:25.089482 ledes-parser-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-16 03:33:08.000000 ledes-parser-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:33:25.085482 ledes-parser-0.3.2/ledes_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-16 03:33:08.000000 ledes-parser-0.3.2/ledes_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-16 03:33:08.000000 ledes-parser-0.3.2/ledes_parser/base_ledes_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-16 03:33:08.000000 ledes-parser-0.3.2/ledes_parser/ledes_1998BI_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-16 03:33:08.000000 ledes-parser-0.3.2/ledes_parser/ledes_1998B_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-16 03:33:08.000000 ledes-parser-0.3.2/ledes_parser/ledes_1998_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-16 03:33:08.000000 ledes-parser-0.3.2/ledes_parser/ledes_dynamic_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:33:25.085482 ledes-parser-0.3.2/ledes_parser/typings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 03:33:08.000000 ledes-parser-0.3.2/ledes_parser/typings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-16 03:33:08.000000 ledes-parser-0.3.2/ledes_parser/typings/invoice_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:33:25.085482 ledes-parser-0.3.2/ledes_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-16 03:33:25.000000 ledes-parser-0.3.2/ledes_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-16 03:33:25.000000 ledes-parser-0.3.2/ledes_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 03:33:25.000000 ledes-parser-0.3.2/ledes_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-16 03:33:25.000000 ledes-parser-0.3.2/ledes_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 03:33:25.089482 ledes-parser-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-16 03:33:08.000000 ledes-parser-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 03:33:25.089482 ledes-parser-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 03:33:08.000000 ledes-parser-0.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-16 03:33:08.000000 ledes-parser-0.3.2/tests/test_ledes_1998_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-16 03:33:08.000000 ledes-parser-0.3.2/tests/test_parse_leads_file.py
```

### Comparing `ledes-parser-0.3.1/LICENSE` & `ledes-parser-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ledes-parser-0.3.1/ledes_parser/ledes_1998_parser.py` & `ledes-parser-0.3.2/ledes_parser/ledes_1998_parser.py`

 * *Files identical despite different names*

### Comparing `ledes-parser-0.3.1/ledes_parser/ledes_dynamic_parser.py` & `ledes-parser-0.3.2/ledes_parser/ledes_dynamic_parser.py`

 * *Files identical despite different names*

### Comparing `ledes-parser-0.3.1/ledes_parser.egg-info/SOURCES.txt` & `ledes-parser-0.3.2/ledes_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ledes-parser-0.3.1/setup.py` & `ledes-parser-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 def read_version():
-    return '0.3.1'
+    return '0.3.2'
     # with open("./VERSION", "r") as version_file:
     #     return version_file.read().strip()
 
 setup(
     name='ledes-parser',
     version=read_version(),
     packages=find_packages(),
```

### Comparing `ledes-parser-0.3.1/tests/test_ledes_1998_parser.py` & `ledes-parser-0.3.2/tests/test_ledes_1998_parser.py`

 * *Files identical despite different names*

