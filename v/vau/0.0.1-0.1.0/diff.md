# Comparing `tmp/vau-0.0.1.tar.gz` & `tmp/vau-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vau-0.0.1.tar", max compression
+gzip compressed data, was "vau-0.1.0.tar", max compression
```

## Comparing `vau-0.0.1.tar` & `vau-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,6 @@
--rw-r--r--   0        0        0      998 2023-04-16 00:51:39.829364 vau-0.0.1/LICENSE
--rw-r--r--   0        0        0     1411 2023-04-16 15:39:07.214360 vau-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-16 15:37:06.577752 vau-0.0.1/src/vau/__init__.py
--rw-r--r--   0        0        0      258 2023-04-16 14:27:45.474855 vau-0.0.1/src/vau/__main__.py
--rw-r--r--   0        0        0     2315 2023-04-16 15:34:02.470929 vau-0.0.1/src/vau/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-04-16 09:29:50.814334 vau-0.0.1/src/vau/commands/alias/__init__.py
--rw-r--r--   0        0        0      964 2023-04-16 14:27:45.582852 vau-0.0.1/src/vau/commands/alias/ls.py
--rw-r--r--   0        0        0      511 2023-04-16 15:31:33.563115 vau-0.0.1/src/vau/commands/alias/rm.py
--rw-r--r--   0        0        0      734 2023-04-16 14:27:45.582852 vau-0.0.1/src/vau/commands/alias/set.py
--rw-r--r--   0        0        0      493 2023-04-16 15:31:33.563115 vau-0.0.1/src/vau/commands/alias/use.py
--rw-r--r--   0        0        0      344 2023-04-16 15:33:54.179162 vau-0.0.1/src/vau/commands/approle/__init__.py
--rw-r--r--   0        0        0     3800 2023-04-16 15:32:12.026034 vau-0.0.1/src/vau/commands/approle/_format.py
--rw-r--r--   0        0        0      542 2023-04-16 15:33:21.548079 vau-0.0.1/src/vau/commands/approle/get.py
--rw-r--r--   0        0        0      651 2023-04-16 15:34:27.786217 vau-0.0.1/src/vau/commands/approle/ls.py
--rw-r--r--   0        0        0     3277 2023-04-16 15:33:16.956209 vau-0.0.1/src/vau/commands/approle/put.py
--rw-r--r--   0        0        0      418 2023-04-16 15:33:11.428364 vau-0.0.1/src/vau/commands/approle/rm.py
--rw-r--r--   0        0        0     1097 2023-04-16 14:27:45.574852 vau-0.0.1/src/vau/config.py
--rw-r--r--   0        0        0        0 2023-04-16 00:51:39.829364 vau-0.0.1/src/vau/py.typed
--rw-r--r--   0        0        0      772 1970-01-01 00:00:00.000000 vau-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      998 2023-04-16 00:51:39.829364 vau-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1244 2023-04-16 00:51:39.389376 vau-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        6 2023-04-16 00:51:39.829364 vau-0.1.0/readme.md
+-rw-r--r--   0        0        0       22 2023-04-16 00:51:39.829364 vau-0.1.0/src/vau/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 00:51:39.829364 vau-0.1.0/src/vau/py.typed
+-rw-r--r--   0        0        0      614 1970-01-01 00:00:00.000000 vau-0.1.0/PKG-INFO
```

### Comparing `vau-0.0.1/LICENSE` & `vau-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vau-0.0.1/pyproject.toml` & `vau-0.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,51 +1,41 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vau"
-version = "0.0.1"
+version = "0.1.0"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
+readme = "readme.md"
 packages = [{ include = "vau", from = "src" }]
 classifiers = []
 keywords = []
 
 [tool.poetry.urls]
 # "Bug Tracker" = ""
 # Documentation = ""
 # Homepage = ""
 # Repository = ""
 
 [tool.poetry.dependencies]
 python = "^3.6"
-typer = "^0.7.0"
-hvac = "^1.1.0"
-rich = "^13.3.4"
-"databind.json" = "^4.2.4"
-typer-builder = "^0.0.8"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 flake8 = "*"
 isort = "*"
 mypy = "*"
 pytest = "*"
 
-[tool.poetry.scripts]
-vau = "vau.__main__:main"
-
 [tool.slap]
 typed = true
 
-[tool.slap.release]
-branch = "main"
-
 [tool.slap.test]
 check = "slap check"
 mypy = "dmypy run src/"
 pytest = "pytest tests/ -vv"
 black = "black --check src/ tests/"
 isort = "isort --check-only src/ tests/"
 flake8 = "flake8 src/ tests/"
```

### Comparing `vau-0.0.1/PKG-INFO` & `vau-0.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: vau
-Version: 0.0.1
+Version: 0.1.0
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: databind.json (>=4.2.4,<5.0.0)
-Requires-Dist: hvac (>=1.1.0,<2.0.0)
-Requires-Dist: rich (>=13.3.4,<14.0.0)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
-Requires-Dist: typer-builder (>=0.0.8,<0.0.9)
+Description-Content-Type: text/markdown
+
+# vau
+
```

