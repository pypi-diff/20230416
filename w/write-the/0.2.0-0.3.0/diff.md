# Comparing `tmp/write_the-0.2.0.tar.gz` & `tmp/write_the-0.3.0.tar.gz`

## Comparing `write_the-0.2.0.tar` & `write_the-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,33 @@
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 write_the-0.2.0/test.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 write_the-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/__main__.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/cli/__init__.py
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/cli/utils.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/cst/__init__.py
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/cst/docstring_adder.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/cst/docstring_remover.py
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/cst/function_and_class_collector.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/cst/node_extractor.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/cst/node_remover.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/cst/utils.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/docs/__init__.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/docs/chain.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 write_the-0.2.0/write_the/docs/write.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 write_the-0.2.0/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 write_the-0.2.0/README.md
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 write_the-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 write_the-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 write_the-0.3.0/mkdocs.yml
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 write_the-0.3.0/test.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 write_the-0.3.0/docs/index.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 write_the-0.3.0/docs/reference/cli.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 write_the-0.3.0/docs/reference/cst.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 write_the-0.3.0/docs/reference/docs.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 write_the-0.3.0/docs/reference/mkdocs.md
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.3.0/docs/reference/utils.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 write_the-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/__main__.py
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/utils.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/cli/__init__.py
+-rw-r--r--   0        0        0     2325 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/cli/main.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/cst/__init__.py
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/cst/docstring_adder.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/cst/docstring_remover.py
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/cst/function_and_class_collector.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/cst/node_extractor.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/cst/node_remover.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/cst/utils.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/docs/__init__.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/docs/chain.py
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/docs/write.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/mkdocs/__init__.py
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/mkdocs/write.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 write_the-0.3.0/write_the/tests/__init__.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 write_the-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 write_the-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 write_the-0.3.0/README.md
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 write_the-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 write_the-0.3.0/PKG-INFO
```

### Comparing `write_the-0.2.0/write_the/cli/utils.py` & `write_the-0.3.0/write_the/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.2.0/write_the/cst/docstring_adder.py` & `write_the-0.3.0/write_the/cst/docstring_adder.py`

 * *Files identical despite different names*

### Comparing `write_the-0.2.0/write_the/cst/docstring_remover.py` & `write_the-0.3.0/write_the/cst/docstring_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.2.0/write_the/cst/function_and_class_collector.py` & `write_the-0.3.0/write_the/cst/function_and_class_collector.py`

 * *Files identical despite different names*

### Comparing `write_the-0.2.0/write_the/cst/node_extractor.py` & `write_the-0.3.0/write_the/cst/node_extractor.py`

 * *Files identical despite different names*

### Comparing `write_the-0.2.0/write_the/cst/node_remover.py` & `write_the-0.3.0/write_the/cst/node_remover.py`

 * *Files identical despite different names*

### Comparing `write_the-0.2.0/write_the/cst/utils.py` & `write_the-0.3.0/write_the/cst/utils.py`

 * *Files identical despite different names*

### Comparing `write_the-0.2.0/write_the/docs/chain.py` & `write_the-0.3.0/write_the/docs/chain.py`

 * *Files identical despite different names*

### Comparing `write_the-0.2.0/write_the/docs/write.py` & `write_the-0.3.0/write_the/docs/write.py`

 * *Files identical despite different names*

### Comparing `write_the-0.2.0/LICENSE.txt` & `write_the-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `write_the-0.2.0/README.md` & `write_the-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `write_the-0.2.0/pyproject.toml` & `write_the-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,16 @@
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "typer[all]",
   "langchain",
   "black",
   "libcst",
+  "mkdocstrings[python]",
+  "mkdocs-material"
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/wytamma/write-the#readme"
 Issues = "https://github.com/wytamma/write-the/issues"
 Source = "https://github.com/wytamma/write-the"
```

### Comparing `write_the-0.2.0/PKG-INFO` & `write_the-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: write-the
-Version: 0.2.0
+Version: 0.3.0
 Summary: AI-powered Code Generation and Refactoring Tool
 Project-URL: Documentation, https://github.com/wytamma/write-the#readme
 Project-URL: Issues, https://github.com/wytamma/write-the/issues
 Project-URL: Source, https://github.com/wytamma/write-the
 Author-email: wytamma <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -15,14 +15,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Requires-Dist: black
 Requires-Dist: langchain
 Requires-Dist: libcst
+Requires-Dist: mkdocs-material
+Requires-Dist: mkdocstrings[python]
 Requires-Dist: typer[all]
 Description-Content-Type: text/markdown
 
 # Write-The: AI-powered Code Generation and Refactoring Tool
 
 [![PyPI - Version](https://img.shields.io/pypi/v/write-the.svg)](https://pypi.org/project/write-the)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/write-the.svg)](https://pypi.org/project/write-the)
```

