# Comparing `tmp/acb-0.1.0.tar.gz` & `tmp/acb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acb-0.1.0.tar", last modified: Sun Apr 16 02:43:37 2023, max compression
+gzip compressed data, was "acb-0.1.1.tar", last modified: Sun Apr 16 03:44:11 2023, max compression
```

## Comparing `acb-0.1.0.tar` & `acb-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      410 2023-04-16 02:10:02.113982 acb-0.1.0/README.md
--rw-r--r--   0        0        0      150 2023-04-16 02:10:02.109301 acb-0.1.0/acb/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 01:26:47.448746 acb-0.1.0/acb/actions/__init__.py
--rw-r--r--   0        0        0     1368 2023-04-16 01:26:47.449716 acb-0.1.0/acb/actions/configure.py
--rw-r--r--   0        0        0     2263 2023-04-16 01:26:47.450059 acb-0.1.0/acb/actions/encode.py
--rw-r--r--   0        0        0     1268 2023-04-16 01:26:47.450605 acb-0.1.0/acb/actions/hash.py
--rw-r--r--   0        0        0        0 2023-04-16 01:26:47.448746 acb-0.1.0/acb/adapters/__init__.py
--rw-r--r--   0        0        0     1036 2023-04-16 02:43:37.996126 acb-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 acb-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      410 2023-04-16 02:10:02.113982 acb-0.1.1/README.md
+-rw-r--r--   0        0        0      150 2023-04-16 02:10:02.109301 acb-0.1.1/acb/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 01:26:47.448746 acb-0.1.1/acb/actions/__init__.py
+-rw-r--r--   0        0        0     1368 2023-04-16 01:26:47.449716 acb-0.1.1/acb/actions/configure.py
+-rw-r--r--   0        0        0     2263 2023-04-16 01:26:47.450059 acb-0.1.1/acb/actions/encode.py
+-rw-r--r--   0        0        0     1268 2023-04-16 01:26:47.450605 acb-0.1.1/acb/actions/hash.py
+-rw-r--r--   0        0        0        0 2023-04-16 01:26:47.448746 acb-0.1.1/acb/adapters/__init__.py
+-rw-r--r--   0        0        0     1197 2023-04-16 03:44:11.004073 acb-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 acb-0.1.1/PKG-INFO
```

### Comparing `acb-0.1.0/acb/actions/configure.py` & `acb-0.1.1/acb/actions/configure.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.0/acb/actions/encode.py` & `acb-0.1.1/acb/actions/encode.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.0/acb/actions/hash.py` & `acb-0.1.1/acb/actions/hash.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.0/pyproject.toml` & `acb-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 [tool.deptry]
 
 [tool.refurb]
 
 [project]
 name = "acb"
-version = "0.1.0"
+version = "0.1.1"
 description = "Asynchronus Code Base"
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 dependencies = [
     "pydantic>=1.10.7",
     "itsdangerous>=2.1.2",
@@ -53,12 +53,17 @@
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 
 [project.license]
 text = "BSD-3-Clause"
 
+[project.urls]
+Homepage = "https://github.com/lesleslie/acb"
+Documentation = "https://github.com/lesleslie/acb"
+Repository = "https://github.com/lesleslie/acb"
+
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

