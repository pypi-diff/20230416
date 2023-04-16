# Comparing `tmp/file_memoizer-0.3.2.tar.gz` & `tmp/file_memoizer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_memoizer-0.3.2.tar", max compression
+gzip compressed data, was "file_memoizer-0.4.0.tar", max compression
```

## Comparing `file_memoizer-0.3.2.tar` & `file_memoizer-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      886 2023-03-13 03:40:05.971578 file_memoizer-0.3.2/LICENSE
--rw-r--r--   0        0        0     2484 2023-03-13 03:40:05.971578 file_memoizer-0.3.2/README.md
--rw-r--r--   0        0        0     2398 2023-03-13 03:40:25.539607 file_memoizer-0.3.2/file_memoizer/__init__.py
--rw-r--r--   0        0        0      603 2023-03-13 03:40:25.539607 file_memoizer-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3164 1970-01-01 00:00:00.000000 file_memoizer-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      886 2023-04-16 14:37:30.328073 file_memoizer-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2409 2023-04-16 14:37:30.328073 file_memoizer-0.4.0/README.md
+-rw-r--r--   0        0        0     1091 2023-04-16 14:37:53.344160 file_memoizer-0.4.0/file_memoizer/__init__.py
+-rw-r--r--   0        0        0      603 2023-04-16 14:37:53.340160 file_memoizer-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3089 1970-01-01 00:00:00.000000 file_memoizer-0.4.0/PKG-INFO
```

### Comparing `file_memoizer-0.3.2/LICENSE` & `file_memoizer-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `file_memoizer-0.3.2/README.md` & `file_memoizer-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # File Memoizer
 
 [![license](https://img.shields.io/github/license/lordjabez/file-memoizer?color=blue&label=License)](https://opensource.org/licenses/MIT)
 [![PyPi:version](https://img.shields.io/pypi/v/file-memoizer?color=blue&label=PyPI)](https://pypi.org/project/file-memoizer/)
 [![Tests](https://github.com/lordjabez/file-memoizer/actions/workflows/test.yml/badge.svg)](https://github.com/lordjabez/file-memoizer/actions/workflows/test.yml)
 [![Release](https://github.com/lordjabez/file-memoizer/actions/workflows/release.yml/badge.svg)](https://github.com/lordjabez/file-memoizer/actions/workflows/release.yml)
 
-This Python package makes it easy to store function results across executions using cache files.
-Underlying functionality is provided by [cachier](https://github.com/python-cachier/cachier), but
-this package adds a few conveniences, such as being able to ignore parameters that won't serialize.
+NOTICE: This package is deprecated and will no longer be updated, as the functionality it provides
+has now been inplemented directly in [cachier](https://github.com/python-cachier/cachier). Please
+use that package directly.
 
 
 ## Installation
 
 Installation is via `pip`:
 
 ```bash
@@ -71,11 +71,11 @@
 import requests
 
 class ExampleAPIClient():
 
     @file_memoizer.memoize()
     def get(self, url):
         return self.session.get(url)
-    
+
     def __init__(self):
         self.session = requests.Session()
 ```
```

### Comparing `file_memoizer-0.3.2/pyproject.toml` & `file_memoizer-0.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "file-memoizer"
 description = "Store function results across executions using cache files"
-version = "0.3.2"
+version = "0.4.0"
 license = "MIT-0"
 authors = ["Judson Neer <judson.neer@gmail.com>"]
 repository = "https://github.com/lordjabez/file-memoizer"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1 <3.12"
-cachier = "^2.0.0"
+cachier = "^2.1.1"
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.4"
 flake8 = "^6.0.0"
-pylint = "^2.17.0"
-pytest = "^7.2.2"
+pylint = "^2.17.2"
+pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 safety = "^2.3.5"
 toml = "^0.10.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `file_memoizer-0.3.2/PKG-INFO` & `file_memoizer-0.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: file-memoizer
-Version: 0.3.2
+Version: 0.4.0
 Summary: Store function results across executions using cache files
 Home-page: https://github.com/lordjabez/file-memoizer
 License: MIT-0
 Author: Judson Neer
 Author-email: judson.neer@gmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: cachier (>=2.0.0,<3.0.0)
+Requires-Dist: cachier (>=2.1.1,<3.0.0)
 Project-URL: Repository, https://github.com/lordjabez/file-memoizer
 Description-Content-Type: text/markdown
 
 # File Memoizer
 
 [![license](https://img.shields.io/github/license/lordjabez/file-memoizer?color=blue&label=License)](https://opensource.org/licenses/MIT)
 [![PyPi:version](https://img.shields.io/pypi/v/file-memoizer?color=blue&label=PyPI)](https://pypi.org/project/file-memoizer/)
 [![Tests](https://github.com/lordjabez/file-memoizer/actions/workflows/test.yml/badge.svg)](https://github.com/lordjabez/file-memoizer/actions/workflows/test.yml)
 [![Release](https://github.com/lordjabez/file-memoizer/actions/workflows/release.yml/badge.svg)](https://github.com/lordjabez/file-memoizer/actions/workflows/release.yml)
 
-This Python package makes it easy to store function results across executions using cache files.
-Underlying functionality is provided by [cachier](https://github.com/python-cachier/cachier), but
-this package adds a few conveniences, such as being able to ignore parameters that won't serialize.
+NOTICE: This package is deprecated and will no longer be updated, as the functionality it provides
+has now been inplemented directly in [cachier](https://github.com/python-cachier/cachier). Please
+use that package directly.
 
 
 ## Installation
 
 Installation is via `pip`:
 
 ```bash
@@ -89,12 +89,12 @@
 import requests
 
 class ExampleAPIClient():
 
     @file_memoizer.memoize()
     def get(self, url):
         return self.session.get(url)
-    
+
     def __init__(self):
         self.session = requests.Session()
 ```
```

