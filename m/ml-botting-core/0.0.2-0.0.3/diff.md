# Comparing `tmp/ml-botting-core-0.0.2.tar.gz` & `tmp/ml_botting_core-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-botting-core-0.0.2.tar", last modified: Sun Apr 16 16:28:22 2023, max compression
+gzip compressed data, was "ml_botting_core-0.0.3.tar", last modified: Sun Apr 16 17:43:09 2023, max compression
```

## Comparing `ml-botting-core-0.0.2.tar` & `ml_botting_core-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:28:22.657678 ml-botting-core-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-16 16:28:11.000000 ml-botting-core-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-16 16:28:22.657678 ml-botting-core-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-16 16:28:11.000000 ml-botting-core-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-16 16:28:11.000000 ml-botting-core-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-16 16:28:22.657678 ml-botting-core-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:28:22.657678 ml-botting-core-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:28:22.657678 ml-botting-core-0.0.2/src/ml-botting-core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:28:11.000000 ml-botting-core-0.0.2/src/ml-botting-core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:28:11.000000 ml-botting-core-0.0.2/src/ml-botting-core/temp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:28:22.657678 ml-botting-core-0.0.2/src/ml_botting_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-16 16:28:22.000000 ml-botting-core-0.0.2/src/ml_botting_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-16 16:28:22.000000 ml-botting-core-0.0.2/src/ml_botting_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:28:22.000000 ml-botting-core-0.0.2/src/ml_botting_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-16 16:28:22.000000 ml-botting-core-0.0.2/src/ml_botting_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:09.956010 ml_botting_core-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-16 17:42:58.000000 ml_botting_core-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-16 17:43:09.956010 ml_botting_core-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-16 17:42:58.000000 ml_botting_core-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-16 17:42:58.000000 ml_botting_core-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-16 17:43:09.956010 ml_botting_core-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:09.952010 ml_botting_core-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:09.956010 ml_botting_core-0.0.3/src/ml_botting_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:58.000000 ml_botting_core-0.0.3/src/ml_botting_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:09.956010 ml_botting_core-0.0.3/src/ml_botting_core/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:58.000000 ml_botting_core-0.0.3/src/ml_botting_core/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 17:42:58.000000 ml_botting_core-0.0.3/src/ml_botting_core/classification/universal_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:09.956010 ml_botting_core-0.0.3/src/ml_botting_core/regression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:58.000000 ml_botting_core-0.0.3/src/ml_botting_core/regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:58.000000 ml_botting_core-0.0.3/src/ml_botting_core/regression/universal_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-16 17:42:58.000000 ml_botting_core-0.0.3/src/ml_botting_core/universal_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:09.956010 ml_botting_core-0.0.3/src/ml_botting_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-16 17:43:09.000000 ml_botting_core-0.0.3/src/ml_botting_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-16 17:43:09.000000 ml_botting_core-0.0.3/src/ml_botting_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 17:43:09.000000 ml_botting_core-0.0.3/src/ml_botting_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-16 17:43:09.000000 ml_botting_core-0.0.3/src/ml_botting_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:09.956010 ml_botting_core-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:58.000000 ml_botting_core-0.0.3/tests/test_init.py
```

### Comparing `ml-botting-core-0.0.2/LICENSE` & `ml_botting_core-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-botting-core-0.0.2/setup.cfg` & `ml_botting_core-0.0.3/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
-name = ml-botting-core
-version = 0.0.2
+name = ml_botting_core
+version = 0.0.3
 author = Ryan Susman
 author_email = ryansusman@gmail.com
 description = Making ML more accessible to botting apps
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/darkmatter2222/ml-botting-core
 project_urls =
```

