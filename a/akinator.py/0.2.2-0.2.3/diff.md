# Comparing `tmp/akinator.py-0.2.2.tar.gz` & `tmp/akinator.py-0.2.3.tar.gz`

## Comparing `akinator.py-0.2.2.tar` & `akinator.py-0.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      878 1970-01-01 00:00:00.000000 akinator.py-0.2.2/Cargo.toml
--rw-r--r--   0     1001      123     4639 2023-04-14 23:36:17.000000 akinator.py-0.2.2/.github/workflows/ci.yml
--rw-r--r--   0     1001      123       88 2023-04-14 23:36:17.000000 akinator.py-0.2.2/.gitignore
--rw-r--r--   0     1001      123      213 2023-04-14 23:36:17.000000 akinator.py-0.2.2/.readthedocs.yml
--rw-r--r--   0     1001      123      190 2023-04-14 23:36:17.000000 akinator.py-0.2.2/.vscode/settings.json
--rw-r--r--   0     1001      123     1076 2023-04-14 23:36:17.000000 akinator.py-0.2.2/LICENSE
--rw-r--r--   0     1001      123      695 2023-04-14 23:36:17.000000 akinator.py-0.2.2/README.md
--rw-r--r--   0     1001      123     4220 2023-04-14 23:36:17.000000 akinator.py-0.2.2/akinator.pyi
--rw-r--r--   0     1001      123      146 2023-04-14 23:36:17.000000 akinator.py-0.2.2/docs/akinator.rst
--rw-r--r--   0     1001      123     2498 2023-04-14 23:36:17.000000 akinator.py-0.2.2/docs/conf.py
--rw-r--r--   0     1001      123     4170 2023-04-14 23:36:17.000000 akinator.py-0.2.2/docs/examples.rst
--rw-r--r--   0     1001      123      475 2023-04-14 23:36:17.000000 akinator.py-0.2.2/docs/index.rst
--rw-r--r--   0     1001      123      591 2023-04-14 23:36:17.000000 akinator.py-0.2.2/pyproject.toml
--rw-r--r--   0     1001      123    10034 2023-04-14 23:36:17.000000 akinator.py-0.2.2/src/async_akinator.rs
--rw-r--r--   0     1001      123     8646 2023-04-14 23:36:17.000000 akinator.py-0.2.2/src/blocking_akinator.rs
--rw-r--r--   0     1001      123     6575 2023-04-14 23:36:17.000000 akinator.py-0.2.2/src/enums.rs
--rw-r--r--   0     1001      123     3947 2023-04-14 23:36:17.000000 akinator.py-0.2.2/src/error.rs
--rw-r--r--   0     1001      123     1044 2023-04-14 23:36:17.000000 akinator.py-0.2.2/src/lib.rs
--rw-r--r--   0     1001      123     1996 2023-04-14 23:36:17.000000 akinator.py-0.2.2/src/models.rs
--rw-r--r--   0     1001      123     1612 2023-04-14 23:36:17.000000 akinator.py-0.2.2/tests/test_async.py
--rw-r--r--   0     1001      123     1543 2023-04-14 23:36:17.000000 akinator.py-0.2.2/tests/test_sync.py
--rw-r--r--   0     1001      123       10 2023-04-14 23:36:38.000000 akinator.py-0.2.2/wheelhouse/akinator.py-0.2.2.tar.gz
--rw-r--r--   0     1001      123    29148 2023-04-14 23:36:37.000000 akinator.py-0.2.2/Cargo.lock
--rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 akinator.py-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      878 1970-01-01 00:00:00.000000 akinator.py-0.2.3/Cargo.toml
+-rw-r--r--   0     1001      123     4639 2023-04-15 22:17:44.000000 akinator.py-0.2.3/.github/workflows/ci.yml
+-rw-r--r--   0     1001      123       88 2023-04-15 22:17:44.000000 akinator.py-0.2.3/.gitignore
+-rw-r--r--   0     1001      123      213 2023-04-15 22:17:44.000000 akinator.py-0.2.3/.readthedocs.yml
+-rw-r--r--   0     1001      123      190 2023-04-15 22:17:44.000000 akinator.py-0.2.3/.vscode/settings.json
+-rw-r--r--   0     1001      123     1076 2023-04-15 22:17:44.000000 akinator.py-0.2.3/LICENSE
+-rw-r--r--   0     1001      123      695 2023-04-15 22:17:44.000000 akinator.py-0.2.3/README.md
+-rw-r--r--   0     1001      123     4220 2023-04-15 22:17:44.000000 akinator.py-0.2.3/akinator.pyi
+-rw-r--r--   0     1001      123      146 2023-04-15 22:17:44.000000 akinator.py-0.2.3/docs/akinator.rst
+-rw-r--r--   0     1001      123     2498 2023-04-15 22:17:44.000000 akinator.py-0.2.3/docs/conf.py
+-rw-r--r--   0     1001      123     4170 2023-04-15 22:17:44.000000 akinator.py-0.2.3/docs/examples.rst
+-rw-r--r--   0     1001      123      475 2023-04-15 22:17:44.000000 akinator.py-0.2.3/docs/index.rst
+-rw-r--r--   0     1001      123      591 2023-04-15 22:17:44.000000 akinator.py-0.2.3/pyproject.toml
+-rw-r--r--   0     1001      123    10034 2023-04-15 22:17:44.000000 akinator.py-0.2.3/src/async_akinator.rs
+-rw-r--r--   0     1001      123     8646 2023-04-15 22:17:44.000000 akinator.py-0.2.3/src/blocking_akinator.rs
+-rw-r--r--   0     1001      123     6575 2023-04-15 22:17:44.000000 akinator.py-0.2.3/src/enums.rs
+-rw-r--r--   0     1001      123     3947 2023-04-15 22:17:44.000000 akinator.py-0.2.3/src/error.rs
+-rw-r--r--   0     1001      123     1044 2023-04-15 22:17:44.000000 akinator.py-0.2.3/src/lib.rs
+-rw-r--r--   0     1001      123     1996 2023-04-15 22:17:44.000000 akinator.py-0.2.3/src/models.rs
+-rw-r--r--   0     1001      123     1612 2023-04-15 22:17:44.000000 akinator.py-0.2.3/tests/test_async.py
+-rw-r--r--   0     1001      123     1543 2023-04-15 22:17:44.000000 akinator.py-0.2.3/tests/test_sync.py
+-rw-r--r--   0     1001      123       10 2023-04-15 22:18:07.000000 akinator.py-0.2.3/wheelhouse/akinator.py-0.2.3.tar.gz
+-rw-r--r--   0     1001      123    29149 2023-04-15 22:18:05.000000 akinator.py-0.2.3/Cargo.lock
+-rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 akinator.py-0.2.3/PKG-INFO
```

### Comparing `akinator.py-0.2.2/Cargo.toml` & `akinator.py-0.2.3/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 name = "akinator-py"
 authors = ["Tom-the-Bomb"]
-version = "0.2.2"
+version = "0.2.3"
 edition = "2021"
 license = "MIT"
 readme = "README.md"
 description = "Python bindings for akinator-rs"
 documentation = "https://akinatorpy.readthedocs.io/en/latest/"
 repository = "https://github.com/Tom-the-Bomb/akinator.py"
 homepage = "https://github.com/Tom-the-Bomb/akinator.py"
```

### Comparing `akinator.py-0.2.2/.github/workflows/ci.yml` & `akinator.py-0.2.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.2/LICENSE` & `akinator.py-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.2/README.md` & `akinator.py-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.2/akinator.pyi` & `akinator.py-0.2.3/akinator.pyi`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.2/docs/conf.py` & `akinator.py-0.2.3/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'akinator.py'
 copyright = '2022, Tom-the-Bomb'
 author = 'Tom-the-Bomb'
 
 # The full version, including alpha/beta/rc tags
-release = '0.2.2'
+release = '0.2.3'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `akinator.py-0.2.2/docs/examples.rst` & `akinator.py-0.2.3/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.2/src/async_akinator.rs` & `akinator.py-0.2.3/src/async_akinator.rs`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.2/src/blocking_akinator.rs` & `akinator.py-0.2.3/src/blocking_akinator.rs`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.2/src/enums.rs` & `akinator.py-0.2.3/src/enums.rs`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.2/src/error.rs` & `akinator.py-0.2.3/src/error.rs`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.2/src/lib.rs` & `akinator.py-0.2.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.2/src/models.rs` & `akinator.py-0.2.3/src/models.rs`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.2/tests/test_async.py` & `akinator.py-0.2.3/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.2/tests/test_sync.py` & `akinator.py-0.2.3/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `akinator.py-0.2.2/Cargo.lock` & `akinator.py-0.2.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "akinator-py"
-version = "0.2.2"
+version = "0.2.3"
 dependencies = [
  "akinator-rs",
  "lazy_static",
  "pyo3",
  "pyo3-asyncio",
  "tokio",
 ]
 
 [[package]]
 name = "akinator-rs"
-version = "0.1.9"
-source = "git+https://github.com/Tom-the-Bomb/akinator-rs#9bfb1ae51a1a654a43f463f64283ce01ee18cd4c"
+version = "0.1.10"
+source = "git+https://github.com/Tom-the-Bomb/akinator-rs#254f546eef15c0b593725496ff51c5a15ab8ecaf"
 dependencies = [
  "lazy_static",
  "regex",
  "reqwest",
  "serde",
  "serde_json",
  "thiserror",
```

### Comparing `akinator.py-0.2.2/PKG-INFO` & `akinator.py-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: akinator.py
-Version: 0.2.2
+Version: 0.2.3
 Requires-Dist: sphinx; extra == 'docs'
 Requires-Dist: furo; extra == 'docs'
 Requires-Dist: sphinxext-opengraph; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
 Provides-Extra: docs
 License-File: LICENSE
 Summary: Python bindings for akinator-rs
 Keywords: akinator,python,async,game,pyo3
 Home-Page: https://github.com/Tom-the-Bomb/akinator.py
 Author: Tom-the-Bomb
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: documentation, https://akinatorpy.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/Tom-the-Bomb/akinator.py
+Project-URL: documentation, https://akinatorpy.readthedocs.io/en/latest/
 Project-URL: homepage, https://github.com/Tom-the-Bomb/akinator.py
 
 # Akinator-py
 Python bindings for ``akinator-rs``, a wrapper around the undocumented akinator API, made using [pyo3](https://pyo3.rs)
 
 designed for easy implementation of an akinator game in code, providing a simple and easy to use API.
```

