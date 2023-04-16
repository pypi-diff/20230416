# Comparing `tmp/pdm_dotenv-0.1.0.tar.gz` & `tmp/pdm_dotenv-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_dotenv-0.1.0.tar", last modified: Sun Apr 16 01:58:19 2023, max compression
+gzip compressed data, was "pdm_dotenv-0.2.0.tar", last modified: Sun Apr 16 12:30:44 2023, max compression
```

## Comparing `pdm_dotenv-0.1.0.tar` & `pdm_dotenv-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1060 2023-04-16 01:58:09.479113 pdm_dotenv-0.1.0/LICENSE
--rw-r--r--   0        0        0      902 2023-04-16 01:58:09.479113 pdm_dotenv-0.1.0/README.md
--rw-r--r--   0        0        0     3271 2023-04-16 01:58:19.107824 pdm_dotenv-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      689 2023-04-16 01:58:09.483113 pdm_dotenv-0.1.0/src/pdm_dotenv/__init__.py
--rw-r--r--   0        0        0      135 2023-04-16 01:58:09.483113 pdm_dotenv-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0       80 2023-04-16 01:58:09.483113 pdm_dotenv-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1120 2023-04-16 01:58:09.483113 pdm_dotenv-0.1.0/tests/test_core.py
--rw-r--r--   0        0        0     1411 1970-01-01 00:00:00.000000 pdm_dotenv-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-04-16 12:30:33.817109 pdm_dotenv-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1076 2023-04-16 12:30:33.817109 pdm_dotenv-0.2.0/README.md
+-rw-r--r--   0        0        0     3294 2023-04-16 12:30:44.129120 pdm_dotenv-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      689 2023-04-16 12:30:33.817109 pdm_dotenv-0.2.0/src/pdm_dotenv/__init__.py
+-rw-r--r--   0        0        0      135 2023-04-16 12:30:33.817109 pdm_dotenv-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       80 2023-04-16 12:30:33.817109 pdm_dotenv-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     1120 2023-04-16 12:30:33.817109 pdm_dotenv-0.2.0/tests/test_core.py
+-rw-r--r--   0        0        0     1584 1970-01-01 00:00:00.000000 pdm_dotenv-0.2.0/PKG-INFO
```

### Comparing `pdm_dotenv-0.1.0/LICENSE` & `pdm_dotenv-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_dotenv-0.1.0/README.md` & `pdm_dotenv-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -14,7 +14,15 @@
 pdm-dotenv requires Python >=3.10
 
 ## Installation
 
 ```shell
 pdm self add pdm-dotenv
 ```
+
+## Configuration
+
+If you want to use something other than `.env`, such as `.dev.env`, you can set `dotenv.path`, e.g.:
+
+```shell
+pdm config --local dotenv.path .dev.env
+```
```

### Comparing `pdm_dotenv-0.1.0/pyproject.toml` & `pdm_dotenv-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 [project]
 name = "pdm-dotenv"
 description = "A pdm plugin that automatically loads .env files"
 authors = [
     { name = "Zane Dufour", email = "zane@znd4.me" },
 ]
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 dependencies = [
     "pdm>=2.5.2",
     "python-dotenv>=1.0.0",
 ]
 dynamic = []
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
 ]
-version = "0.1.0"
+version = "0.2.0"
 
 [project.license]
 text = "MIT"
 
 [project.entry-points.pdm]
 dotenv = "pdm_dotenv:plugin"
 
@@ -72,14 +72,16 @@
 [tool.pdm.scripts.doc]
 shell = "cd docs && mkdocs serve"
 help = "Start the dev server for doc preview"
 
 [tool.black]
 line-length = 100
 target-version = [
+    "py38",
+    "py39",
     "py310",
     "py311",
 ]
 
 [tool.ruff]
 line-length = 100
 select = [
```

### Comparing `pdm_dotenv-0.1.0/src/pdm_dotenv/__init__.py` & `pdm_dotenv-0.2.0/src/pdm_dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm_dotenv-0.1.0/tests/test_core.py` & `pdm_dotenv-0.2.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pdm_dotenv-0.1.0/PKG-INFO` & `pdm_dotenv-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pdm-dotenv
-Version: 0.1.0
+Version: 0.2.0
 Summary: A pdm plugin that automatically loads .env files
 Author-Email: Zane Dufour <zane@znd4.me>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Project-URL: Repository, https://github.com/zdog234/pdm-dotenv
 Project-URL: Homepage, https://github.com/zdog234/pdm-dotenv
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Requires-Dist: pdm>=2.5.2
 Requires-Dist: python-dotenv>=1.0.0
 Description-Content-Type: text/markdown
 
 # pdm-dotenv
 
 [![Tests](https://github.com/zdog234/pdm-dotenv/workflows/Tests/badge.svg)](https://github.com/zdog234/pdm-dotenv/actions?query=workflow%3Aci)
@@ -29,7 +29,15 @@
 pdm-dotenv requires Python >=3.10
 
 ## Installation
 
 ```shell
 pdm self add pdm-dotenv
 ```
+
+## Configuration
+
+If you want to use something other than `.env`, such as `.dev.env`, you can set `dotenv.path`, e.g.:
+
+```shell
+pdm config --local dotenv.path .dev.env
+```
```

