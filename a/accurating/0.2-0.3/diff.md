# Comparing `tmp/accurating-0.2.tar.gz` & `tmp/accurating-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accurating-0.2.tar", max compression
+gzip compressed data, was "accurating-0.3.tar", max compression
```

## Comparing `accurating-0.2.tar` & `accurating-0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.2/LICENSE
--rw-r--r--   0        0        0      126 2023-04-16 18:26:44.687984 accurating-0.2/README.md
--rw-r--r--   0        0        0       25 2023-04-16 18:25:22.173292 accurating-0.2/accurating/__init__.py
--rw-r--r--   0        0        0       45 2023-04-16 18:25:22.173292 accurating-0.2/accurating/model.py
--rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.2/accurating/tests/__init__.py
--rw-r--r--   0        0        0       70 2023-04-16 18:27:03.123687 accurating-0.2/accurating/tests/model_test.py
--rw-r--r--   0        0        0      397 2023-04-16 18:39:09.569313 accurating-0.2/pyproject.toml
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 accurating-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.3/LICENSE
+-rw-r--r--   0        0        0      126 2023-04-16 18:26:44.687984 accurating-0.3/README.md
+-rw-r--r--   0        0        0       77 2023-04-16 19:43:19.355111 accurating-0.3/accurating/__init__.py
+-rw-r--r--   0        0        0     4613 2023-04-16 20:02:11.985128 accurating-0.3/accurating/model.py
+-rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.3/accurating/tests/__init__.py
+-rw-r--r--   0        0        0     3313 2023-04-16 20:07:51.802000 accurating-0.3/accurating/tests/model_test.py
+-rw-r--r--   0        0        0      460 2023-04-16 20:16:28.967228 accurating-0.3/pyproject.toml
+-rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 accurating-0.3/PKG-INFO
```

### Comparing `accurating-0.2/LICENSE` & `accurating-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `accurating-0.2/PKG-INFO` & `accurating-0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: accurating
-Version: 0.2
+Version: 0.3
 Summary: 
 Author: Lukasz Lew
 Author-email: lukasz.lew@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jax (>=0.4.8,<0.5.0)
+Requires-Dist: jaxlib (>=0.4.7,<0.5.0)
 Requires-Dist: pytest (>=6.2.5,<7.0.0)
 Description-Content-Type: text/markdown
 
 # AccuRating
 
 ## Development
```

