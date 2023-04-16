# Comparing `tmp/pytest_maybe_context-0.tar.gz` & `tmp/pytest_maybe_context-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_maybe_context-0.tar", max compression
+gzip compressed data, was "pytest_maybe_context-0.1.tar", max compression
```

## Comparing `pytest_maybe_context-0.tar` & `pytest_maybe_context-0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      929 2023-04-16 10:13:37.023112 pytest_maybe_context-0/pyproject.toml
--rw-r--r--   0        0        0      115 2023-04-16 09:33:28.807866 pytest_maybe_context-0/pytest_maybe_context/__init__.py
--rw-r--r--   0        0        0     1153 2023-04-15 18:16:49.009554 pytest_maybe_context-0/pytest_maybe_context/main.py
--rw-r--r--   0        0        0        0 2023-04-09 12:19:40.764656 pytest_maybe_context-0/pytest_maybe_context/py.typed
--rw-r--r--   0        0        0      611 2023-04-16 10:19:48.618216 pytest_maybe_context-0/readme.md
--rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 pytest_maybe_context-0/PKG-INFO
+-rw-r--r--   0        0        0      993 2023-04-16 12:39:18.960503 pytest_maybe_context-0.1/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-04-16 09:33:28.807866 pytest_maybe_context-0.1/pytest_maybe_context/__init__.py
+-rw-r--r--   0        0        0     1153 2023-04-15 18:16:49.009554 pytest_maybe_context-0.1/pytest_maybe_context/main.py
+-rw-r--r--   0        0        0        0 2023-04-09 12:19:40.764656 pytest_maybe_context-0.1/pytest_maybe_context/py.typed
+-rw-r--r--   0        0        0      611 2023-04-16 10:19:48.618216 pytest_maybe_context-0.1/readme.md
+-rw-r--r--   0        0        0     1245 1970-01-01 00:00:00.000000 pytest_maybe_context-0.1/PKG-INFO
```

### Comparing `pytest_maybe_context-0/pyproject.toml` & `pytest_maybe_context-0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = 'pytest-maybe-context'
-version = '0'
+version = '0.1'
 description = "Simplify tests with warning and exception cases."
 readme = 'readme.md'
 authors = ["wrwrwr <code@wr.waw.pl>"]
 license = 'MIT'
 keywords = ['pytest', 'plugin']
 packages = [{include = 'pytest_maybe_context'}]
+repository = "https://github.com/wrwrwr/pytest-maybe-context"
 
 [tool.poetry.dependencies]
 python = '^3.10'
 pytest = '^7'
 
 [tool.poetry.group.dev.dependencies]
 flake8 = '*'
```

### Comparing `pytest_maybe_context-0/pytest_maybe_context/main.py` & `pytest_maybe_context-0.1/pytest_maybe_context/main.py`

 * *Files identical despite different names*

### Comparing `pytest_maybe_context-0/readme.md` & `pytest_maybe_context-0.1/readme.md`

 * *Files identical despite different names*

### Comparing `pytest_maybe_context-0/PKG-INFO` & `pytest_maybe_context-0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: pytest-maybe-context
-Version: 0
+Version: 0.1
 Summary: Simplify tests with warning and exception cases.
+Home-page: https://github.com/wrwrwr/pytest-maybe-context
 License: MIT
 Keywords: pytest,plugin
 Author: wrwrwr
 Author-email: code@wr.waw.pl
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pytest (>=7,<8)
+Project-URL: Repository, https://github.com/wrwrwr/pytest-maybe-context
 Description-Content-Type: text/markdown
 
 # pytest-maybe-context
 
 Makes it a bit easier to write warning and exception checks along other cases.
 
 ```python
```

