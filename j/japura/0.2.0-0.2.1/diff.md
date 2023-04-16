# Comparing `tmp/japura-0.2.0.tar.gz` & `tmp/japura-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "japura-0.2.0.tar", last modified: Sun Apr 16 09:02:00 2023, max compression
+gzip compressed data, was "japura-0.2.1.tar", last modified: Sun Apr 16 16:38:34 2023, max compression
```

## Comparing `japura-0.2.0.tar` & `japura-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:00.064868 japura-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-16 09:01:48.000000 japura-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-16 09:02:00.064868 japura-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-16 09:01:48.000000 japura-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:00.064868 japura-0.2.0/japura/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-16 09:01:48.000000 japura-0.2.0/japura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-16 09:01:48.000000 japura-0.2.0/japura/efs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-16 09:01:48.000000 japura-0.2.0/japura/key.py
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-04-16 09:01:48.000000 japura-0.2.0/japura/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:00.064868 japura-0.2.0/japura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-16 09:02:00.000000 japura-0.2.0/japura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-16 09:02:00.000000 japura-0.2.0/japura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 09:02:00.000000 japura-0.2.0/japura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-16 09:02:00.000000 japura-0.2.0/japura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 09:02:00.000000 japura-0.2.0/japura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-16 09:01:48.000000 japura-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 09:02:00.064868 japura-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:02:00.064868 japura-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-16 09:01:48.000000 japura-0.2.0/tests/test_efs.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-16 09:01:48.000000 japura-0.2.0/tests/test_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-16 09:01:48.000000 japura-0.2.0/tests/test_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:38:34.189151 japura-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-16 16:38:20.000000 japura-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-16 16:38:34.185151 japura-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-16 16:38:20.000000 japura-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:38:34.185151 japura-0.2.1/japura/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-16 16:38:20.000000 japura-0.2.1/japura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-16 16:38:20.000000 japura-0.2.1/japura/efs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-16 16:38:20.000000 japura-0.2.1/japura/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-04-16 16:38:20.000000 japura-0.2.1/japura/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:38:34.185151 japura-0.2.1/japura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-16 16:38:34.000000 japura-0.2.1/japura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-16 16:38:34.000000 japura-0.2.1/japura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:38:34.000000 japura-0.2.1/japura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-16 16:38:34.000000 japura-0.2.1/japura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 16:38:34.000000 japura-0.2.1/japura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-16 16:38:20.000000 japura-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 16:38:34.189151 japura-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:38:34.185151 japura-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-16 16:38:20.000000 japura-0.2.1/tests/test_efs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-16 16:38:20.000000 japura-0.2.1/tests/test_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-16 16:38:20.000000 japura-0.2.1/tests/test_sql.py
```

### Comparing `japura-0.2.0/LICENSE` & `japura-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `japura-0.2.0/PKG-INFO` & `japura-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: japura
-Version: 0.2.0
+Version: 0.2.1
 Summary: The Python library for securing and managing web resources.
 Author-email: Joumaico Maulas <joumaico@gmx.com>
 License: MIT License
         
         Copyright (c) 2023 joumaico
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `japura-0.2.0/README.md` & `japura-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `japura-0.2.0/japura/efs.py` & `japura-0.2.1/japura/efs.py`

 * *Files identical despite different names*

### Comparing `japura-0.2.0/japura/key.py` & `japura-0.2.1/japura/key.py`

 * *Files identical despite different names*

### Comparing `japura-0.2.0/japura/sql.py` & `japura-0.2.1/japura/sql.py`

 * *Files identical despite different names*

### Comparing `japura-0.2.0/japura.egg-info/PKG-INFO` & `japura-0.2.1/japura.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: japura
-Version: 0.2.0
+Version: 0.2.1
 Summary: The Python library for securing and managing web resources.
 Author-email: Joumaico Maulas <joumaico@gmx.com>
 License: MIT License
         
         Copyright (c) 2023 joumaico
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `japura-0.2.0/pyproject.toml` & `japura-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,23 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 requires-python = ">=3.9"
 dependencies = [
-    "bcrypt>=4.0.1",
-    "cryptography>=40.0.1",
+    "bcrypt>=3.2.2",
+    "cryptography>=37.0.4",
     "pymysql>=1.0.3",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/joumaico/japura/"
 Documentation = "https://joumaico.github.io/japura/"
 
 [build-system]
-requires = ["setuptools>=67.4.0", "wheel"]
+requires = ["setuptools>=67.6.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.dynamic]
 version = {attr = "japura.__version__"}
```

### Comparing `japura-0.2.0/tests/test_key.py` & `japura-0.2.1/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `japura-0.2.0/tests/test_sql.py` & `japura-0.2.1/tests/test_sql.py`

 * *Files identical despite different names*

