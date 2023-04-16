# Comparing `tmp/mini_python-0.1.4.tar.gz` & `tmp/mini_python-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mini_python-0.1.4.tar", max compression
+gzip compressed data, was "mini_python-0.1.5.tar", max compression
```

## Comparing `mini_python-0.1.4.tar` & `mini_python-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-04-16 15:51:46.561202 mini_python-0.1.4/LICENSE
--rw-r--r--   0        0        0       52 2023-04-16 15:51:46.561202 mini_python-0.1.4/README.md
--rw-r--r--   0        0        0     6148 2023-04-16 15:51:46.561202 mini_python-0.1.4/mini_python/.DS_Store
--rw-r--r--   0        0        0       22 2023-04-16 15:51:46.561202 mini_python-0.1.4/mini_python/__init__.py
--rw-r--r--   0        0        0     2311 2023-04-16 15:51:46.561202 mini_python-0.1.4/mini_python/app.py
--rw-r--r--   0        0        0       96 2023-04-16 15:51:46.561202 mini_python-0.1.4/mini_python/static/css/style.css
--rw-r--r--   0        0        0     2112 2023-04-16 15:51:46.561202 mini_python-0.1.4/mini_python/templates/base.html
--rw-r--r--   0        0        0      730 2023-04-16 15:51:46.561202 mini_python-0.1.4/mini_python/templates/create.html
--rw-r--r--   0        0        0     1037 2023-04-16 15:51:46.561202 mini_python-0.1.4/mini_python/templates/edit.html
--rw-r--r--   0        0        0      500 2023-04-16 15:51:46.561202 mini_python-0.1.4/mini_python/templates/index.html
--rw-r--r--   0        0        0      228 2023-04-16 15:51:46.561202 mini_python-0.1.4/mini_python/templates/post.html
--rw-r--r--   0        0        0      588 2023-04-16 15:51:46.561202 mini_python-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 mini_python-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-16 15:58:46.721152 mini_python-0.1.5/LICENSE
+-rw-r--r--   0        0        0       52 2023-04-16 15:58:46.721152 mini_python-0.1.5/README.md
+-rw-r--r--   0        0        0     6148 2023-04-16 15:58:46.721152 mini_python-0.1.5/mini_python/.DS_Store
+-rw-r--r--   0        0        0       22 2023-04-16 15:58:46.721152 mini_python-0.1.5/mini_python/__init__.py
+-rw-r--r--   0        0        0     2311 2023-04-16 15:58:46.721152 mini_python-0.1.5/mini_python/app.py
+-rw-r--r--   0        0        0       96 2023-04-16 15:58:46.721152 mini_python-0.1.5/mini_python/static/css/style.css
+-rw-r--r--   0        0        0     2112 2023-04-16 15:58:46.721152 mini_python-0.1.5/mini_python/templates/base.html
+-rw-r--r--   0        0        0      730 2023-04-16 15:58:46.721152 mini_python-0.1.5/mini_python/templates/create.html
+-rw-r--r--   0        0        0     1037 2023-04-16 15:58:46.721152 mini_python-0.1.5/mini_python/templates/edit.html
+-rw-r--r--   0        0        0      500 2023-04-16 15:58:46.721152 mini_python-0.1.5/mini_python/templates/index.html
+-rw-r--r--   0        0        0      228 2023-04-16 15:58:46.721152 mini_python-0.1.5/mini_python/templates/post.html
+-rw-r--r--   0        0        0      588 2023-04-16 15:58:46.721152 mini_python-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 mini_python-0.1.5/PKG-INFO
```

### Comparing `mini_python-0.1.4/LICENSE` & `mini_python-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mini_python-0.1.4/mini_python/.DS_Store` & `mini_python-0.1.5/mini_python/.DS_Store`

 * *Files identical despite different names*

### Comparing `mini_python-0.1.4/mini_python/app.py` & `mini_python-0.1.5/mini_python/app.py`

 * *Files identical despite different names*

### Comparing `mini_python-0.1.4/mini_python/templates/base.html` & `mini_python-0.1.5/mini_python/templates/base.html`

 * *Files identical despite different names*

### Comparing `mini_python-0.1.4/mini_python/templates/create.html` & `mini_python-0.1.5/mini_python/templates/create.html`

 * *Files identical despite different names*

### Comparing `mini_python-0.1.4/mini_python/templates/edit.html` & `mini_python-0.1.5/mini_python/templates/edit.html`

 * *Files identical despite different names*

### Comparing `mini_python-0.1.4/pyproject.toml` & `mini_python-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mini-python"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Naveen Thurimerla <nawinto99@gmail.com>"]
 readme = "README.md"
 packages = [{include = "mini_python"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `mini_python-0.1.4/PKG-INFO` & `mini_python-0.1.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini-python
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Naveen Thurimerla
 Author-email: nawinto99@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

