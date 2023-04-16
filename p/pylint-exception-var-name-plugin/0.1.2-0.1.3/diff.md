# Comparing `tmp/pylint-exception-var-name-plugin-0.1.2.tar.gz` & `tmp/pylint_exception_var_name_plugin-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylint-exception-var-name-plugin-0.1.2.tar", max compression
+gzip compressed data, was "pylint_exception_var_name_plugin-0.1.3.tar", max compression
```

## Comparing `pylint-exception-var-name-plugin-0.1.2.tar` & `pylint_exception_var_name_plugin-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1077 2021-09-02 12:15:39.574359 pylint-exception-var-name-plugin-0.1.2/LICENSE
--rw-r--r--   0        0        0      490 2021-09-11 10:05:51.950766 pylint-exception-var-name-plugin-0.1.2/README.md
--rw-r--r--   0        0        0       73 2021-09-11 10:05:51.950766 pylint-exception-var-name-plugin-0.1.2/pylint_exception_var_name_plugin/__init__.py
--rw-r--r--   0        0        0      931 2021-09-11 10:05:51.950766 pylint-exception-var-name-plugin-0.1.2/pylint_exception_var_name_plugin/checker.py
--rw-r--r--   0        0        0      162 2021-09-11 10:05:51.950766 pylint-exception-var-name-plugin-0.1.2/pylint_exception_var_name_plugin/exception_var_name.py
--rw-r--r--   0        0        0      884 2021-09-11 10:05:51.950766 pylint-exception-var-name-plugin-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1236 2021-09-11 10:06:45.711126 pylint-exception-var-name-plugin-0.1.2/setup.py
--rw-r--r--   0        0        0     1380 2021-09-11 10:06:45.711345 pylint-exception-var-name-plugin-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-14 03:35:46.889746 pylint_exception_var_name_plugin-0.1.3/LICENSE
+-rw-r--r--   0        0        0      381 2023-04-16 14:16:49.285101 pylint_exception_var_name_plugin-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-16 14:18:13.792799 pylint_exception_var_name_plugin-0.1.3/pylint_exception_var_name_plugin/__init__.py
+-rw-r--r--   0        0        0      938 2023-04-16 14:23:25.047637 pylint_exception_var_name_plugin-0.1.3/pylint_exception_var_name_plugin/checker.py
+-rw-r--r--   0        0        0      214 2023-04-16 14:24:26.486732 pylint_exception_var_name_plugin-0.1.3/pylint_exception_var_name_plugin/exception_var_name.py
+-rw-r--r--   0        0        0     1058 2023-04-16 14:23:58.595508 pylint_exception_var_name_plugin-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 pylint_exception_var_name_plugin-0.1.3/PKG-INFO
```

### Comparing `pylint-exception-var-name-plugin-0.1.2/LICENSE` & `pylint_exception_var_name_plugin-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pylint-exception-var-name-plugin-0.1.2/pyproject.toml` & `pylint_exception_var_name_plugin-0.1.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylint-exception-var-name-plugin"
-version = "0.1.2"
+version = "0.1.3"
 description = "Plugin for pylint which allows to define and check variable name for exception"
 authors = ["Konstantin Shestakov <winmasta@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/winmasta"
 repository = "https://github.com/winmasta"
 keywords = ["pylint", "exception", "lint"]
@@ -17,13 +17,22 @@
 ]
 include = ["LICENSE"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pylint = "*"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.test]
+optional = true
+
+[tool.poetry.group.test.dependencies]
 pytest = "*"
+ruff = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.ruff]
+line-length = 120
+select = ["ALL"]
+ignore = ["D100", "D101", "D102", "D103", "D104", "D203", "D212"]
```

### Comparing `pylint-exception-var-name-plugin-0.1.2/PKG-INFO` & `pylint_exception_var_name_plugin-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: pylint-exception-var-name-plugin
-Version: 0.1.2
+Version: 0.1.3
 Summary: Plugin for pylint which allows to define and check variable name for exception
 Home-page: https://github.com/winmasta
 License: MIT
 Keywords: pylint,exception,lint
 Author: Konstantin Shestakov
 Author-email: winmasta@yandex.ru
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta 
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Dist: pylint
 Project-URL: Repository, https://github.com/winmasta
 Description-Content-Type: text/markdown
 
@@ -25,18 +27,16 @@
 Install:
 ```bash
 pip install pylint-exception-var-name-plugin
 ```
 
 Usage:
 ```bash
-pylint --load-plugins exception_var_name FILES_TO_CHECK
+pylint --load-plugins pylint_exception_var_name_plugin FILES_TO_CHECK
 ```
 
-`ALLOWED_VAR_NAME` default is `e`. Can be set in command line:
-```bash
-pylint --load-plugins exception_var_name ALLOWED_VAR_NAME FILES_TO_CHECK
-```
-or in pylint config file (`pylintrc`)
+Add to `pylintrc` file to set `ALLOWED_VAR_NAME`:
 ```bash
+[VARIABLES]
 exception-var-name=ALLOWED_VAR_NAME
 ```
+
```

