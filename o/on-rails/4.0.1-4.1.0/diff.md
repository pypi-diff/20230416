# Comparing `tmp/on_rails-4.0.1.tar.gz` & `tmp/on_rails-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "on_rails-4.0.1.tar", max compression
+gzip compressed data, was "on_rails-4.1.0.tar", max compression
```

## Comparing `on_rails-4.0.1.tar` & `on_rails-4.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    35149 2023-04-12 20:37:44.960427 on_rails-4.0.1/LICENSE
--rw-r--r--   0        0        0    14186 2023-04-12 20:37:44.960427 on_rails-4.0.1/README.md
--rw-r--r--   0        0        0    48606 2023-04-12 20:37:44.960427 on_rails-4.0.1/on_rails/Result.py
--rw-r--r--   0        0        0     2866 2023-04-12 20:37:44.960427 on_rails-4.0.1/on_rails/ResultDetail.py
--rw-r--r--   0        0        0     1802 2023-04-12 20:37:44.960427 on_rails-4.0.1/on_rails/ResultDetails/ErrorDetail.py
--rw-r--r--   0        0        0      808 2023-04-12 20:37:44.960427 on_rails-4.0.1/on_rails/ResultDetails/Errors/BadRequestError.py
--rw-r--r--   0        0        0      819 2023-04-12 20:37:44.960427 on_rails-4.0.1/on_rails/ResultDetails/Errors/ConflictError.py
--rw-r--r--   0        0        0      840 2023-04-12 20:37:44.960427 on_rails-4.0.1/on_rails/ResultDetails/Errors/ExceptionError.py
--rw-r--r--   0        0        0      728 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/Errors/ForbiddenError.py
--rw-r--r--   0        0        0      726 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/Errors/InternalError.py
--rw-r--r--   0        0        0     1227 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/Errors/NotFoundError.py
--rw-r--r--   0        0        0      880 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/Errors/UnauthorizedError.py
--rw-r--r--   0        0        0      753 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/Errors/ValidationError.py
--rw-r--r--   0        0        0      474 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/Errors/__init__.py
--rw-r--r--   0        0        0      573 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/Success/CreatedDetail.py
--rw-r--r--   0        0        0      629 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/Success/NotModifiedDetail.py
--rw-r--r--   0        0        0      831 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/Success/PartialContentDetail.py
--rw-r--r--   0        0        0      188 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/Success/__init__.py
--rw-r--r--   0        0        0     1034 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/SuccessDetail.py
--rw-r--r--   0        0        0      100 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/ResultDetails/__init__.py
--rw-r--r--   0        0        0      135 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/__init__.py
--rw-r--r--   0        0        0     4867 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/_utility.py
--rw-r--r--   0        0        0     2085 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/decorator.py
--rw-r--r--   0        0        0     8011 2023-04-12 20:37:44.964428 on_rails-4.0.1/on_rails/test_helpers.py
--rw-r--r--   0        0        0      722 2023-04-12 20:37:44.964428 on_rails-4.0.1/pyproject.toml
--rw-r--r--   0        0        0    14813 1970-01-01 00:00:00.000000 on_rails-4.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-16 00:24:39.375441 on_rails-4.1.0/LICENSE
+-rw-r--r--   0        0        0    14186 2023-04-16 00:24:39.375441 on_rails-4.1.0/README.md
+-rw-r--r--   0        0        0    48606 2023-04-16 00:24:39.375441 on_rails-4.1.0/on_rails/Result.py
+-rw-r--r--   0        0        0     2866 2023-04-16 00:24:39.375441 on_rails-4.1.0/on_rails/ResultDetail.py
+-rw-r--r--   0        0        0     1802 2023-04-16 00:24:39.375441 on_rails-4.1.0/on_rails/ResultDetails/ErrorDetail.py
+-rw-r--r--   0        0        0      808 2023-04-16 00:24:39.375441 on_rails-4.1.0/on_rails/ResultDetails/Errors/BadRequestError.py
+-rw-r--r--   0        0        0      819 2023-04-16 00:24:39.375441 on_rails-4.1.0/on_rails/ResultDetails/Errors/ConflictError.py
+-rw-r--r--   0        0        0      840 2023-04-16 00:24:39.375441 on_rails-4.1.0/on_rails/ResultDetails/Errors/ExceptionError.py
+-rw-r--r--   0        0        0      728 2023-04-16 00:24:39.375441 on_rails-4.1.0/on_rails/ResultDetails/Errors/ForbiddenError.py
+-rw-r--r--   0        0        0      726 2023-04-16 00:24:39.375441 on_rails-4.1.0/on_rails/ResultDetails/Errors/InternalError.py
+-rw-r--r--   0        0        0     1227 2023-04-16 00:24:39.375441 on_rails-4.1.0/on_rails/ResultDetails/Errors/NotFoundError.py
+-rw-r--r--   0        0        0      880 2023-04-16 00:24:39.375441 on_rails-4.1.0/on_rails/ResultDetails/Errors/UnauthorizedError.py
+-rw-r--r--   0        0        0      753 2023-04-16 00:24:39.375441 on_rails-4.1.0/on_rails/ResultDetails/Errors/ValidationError.py
+-rw-r--r--   0        0        0      474 2023-04-16 00:24:39.379441 on_rails-4.1.0/on_rails/ResultDetails/Errors/__init__.py
+-rw-r--r--   0        0        0      573 2023-04-16 00:24:39.379441 on_rails-4.1.0/on_rails/ResultDetails/Success/CreatedDetail.py
+-rw-r--r--   0        0        0      629 2023-04-16 00:24:39.379441 on_rails-4.1.0/on_rails/ResultDetails/Success/NotModifiedDetail.py
+-rw-r--r--   0        0        0      831 2023-04-16 00:24:39.379441 on_rails-4.1.0/on_rails/ResultDetails/Success/PartialContentDetail.py
+-rw-r--r--   0        0        0      188 2023-04-16 00:24:39.379441 on_rails-4.1.0/on_rails/ResultDetails/Success/__init__.py
+-rw-r--r--   0        0        0     1034 2023-04-16 00:24:39.379441 on_rails-4.1.0/on_rails/ResultDetails/SuccessDetail.py
+-rw-r--r--   0        0        0      100 2023-04-16 00:24:39.379441 on_rails-4.1.0/on_rails/ResultDetails/__init__.py
+-rw-r--r--   0        0        0      135 2023-04-16 00:24:39.379441 on_rails-4.1.0/on_rails/__init__.py
+-rw-r--r--   0        0        0     4867 2023-04-16 00:24:39.379441 on_rails-4.1.0/on_rails/_utility.py
+-rw-r--r--   0        0        0     2085 2023-04-16 00:24:39.379441 on_rails-4.1.0/on_rails/decorator.py
+-rw-r--r--   0        0        0     8011 2023-04-16 00:24:39.379441 on_rails-4.1.0/on_rails/test_helpers.py
+-rw-r--r--   0        0        0      721 2023-04-16 00:24:39.379441 on_rails-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0    14912 1970-01-01 00:00:00.000000 on_rails-4.1.0/PKG-INFO
```

### Comparing `on_rails-4.0.1/LICENSE` & `on_rails-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.1/README.md` & `on_rails-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.1/on_rails/Result.py` & `on_rails-4.1.0/on_rails/Result.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.1/on_rails/ResultDetail.py` & `on_rails-4.1.0/on_rails/ResultDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.1/on_rails/ResultDetails/ErrorDetail.py` & `on_rails-4.1.0/on_rails/ResultDetails/ErrorDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.1/on_rails/ResultDetails/Errors/BadRequestError.py` & `on_rails-4.1.0/on_rails/ResultDetails/Errors/BadRequestError.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.1/on_rails/ResultDetails/Errors/ConflictError.py` & `on_rails-4.1.0/on_rails/ResultDetails/Errors/ConflictError.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.1/on_rails/ResultDetails/Errors/ExceptionError.py` & `on_rails-4.1.0/on_rails/ResultDetails/Errors/ExceptionError.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.1/on_rails/ResultDetails/Errors/ForbiddenError.py` & `on_rails-4.1.0/on_rails/ResultDetails/Errors/ForbiddenError.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.1/on_rails/ResultDetails/Errors/InternalError.py` & `on_rails-4.1.0/on_rails/ResultDetails/Errors/InternalError.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.1/on_rails/ResultDetails/Errors/NotFoundError.py` & `on_rails-4.1.0/on_rails/ResultDetails/Errors/NotFoundError.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.1/on_rails/ResultDetails/Errors/UnauthorizedError.py` & `on_rails-4.1.0/on_rails/ResultDetails/Errors/UnauthorizedError.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.1/on_rails/ResultDetails/Errors/ValidationError.py` & `on_rails-4.1.0/on_rails/ResultDetails/Errors/ValidationError.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.1/on_rails/ResultDetails/Success/CreatedDetail.py` & `on_rails-4.1.0/on_rails/ResultDetails/Success/CreatedDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.1/on_rails/ResultDetails/Success/NotModifiedDetail.py` & `on_rails-4.1.0/on_rails/ResultDetails/Success/NotModifiedDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.1/on_rails/ResultDetails/Success/PartialContentDetail.py` & `on_rails-4.1.0/on_rails/ResultDetails/Success/PartialContentDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.1/on_rails/ResultDetails/SuccessDetail.py` & `on_rails-4.1.0/on_rails/ResultDetails/SuccessDetail.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.1/on_rails/_utility.py` & `on_rails-4.1.0/on_rails/_utility.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.1/on_rails/decorator.py` & `on_rails-4.1.0/on_rails/decorator.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.1/on_rails/test_helpers.py` & `on_rails-4.1.0/on_rails/test_helpers.py`

 * *Files identical despite different names*

### Comparing `on_rails-4.0.1/pyproject.toml` & `on_rails-4.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # https://python-poetry.org/docs/pyproject/
 [tool.poetry]
 name = "on_rails"
-version = "4.0.1"
+version = "4.1.0"
 description = "Simple and powerful Railway Oriented library for python"
 authors = ["Payadel <payadelteam@gmail.com>"]
 readme = "README.md"
 license = "GPLV3"
 repository = "https://github.com/Payadel/on_rails"
 keywords = ["railway oriented","functional programming", "error handling"]
 packages = [{ include = "on_rails" }]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.0"
 pytest = "^7.2.2"
 pylint = "^2.17.0"
 isort = "^5.12.0"
```

### Comparing `on_rails-4.0.1/PKG-INFO` & `on_rails-4.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: on-rails
-Version: 4.0.1
+Version: 4.1.0
 Summary: Simple and powerful Railway Oriented library for python
 Home-page: https://github.com/Payadel/on_rails
 License: GPLV3
 Keywords: railway oriented,functional programming,error handling
 Author: Payadel
 Author-email: payadelteam@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/Payadel/on_rails
 Description-Content-Type: text/markdown
 
 <div align="center">
   <h1>on_rails</h1>
```

