# Comparing `tmp/pylint-blank-line-plugin-0.1.3.tar.gz` & `tmp/pylint_blank_line_plugin-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylint-blank-line-plugin-0.1.3.tar", max compression
+gzip compressed data, was "pylint_blank_line_plugin-0.1.4.tar", max compression
```

## Comparing `pylint-blank-line-plugin-0.1.3.tar` & `pylint_blank_line_plugin-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1077 2021-09-09 02:28:52.723185 pylint-blank-line-plugin-0.1.3/LICENSE
--rw-r--r--   0        0        0      238 2021-09-11 10:45:21.637364 pylint-blank-line-plugin-0.1.3/README.md
--rw-r--r--   0        0        0       57 2021-09-11 10:45:27.361151 pylint-blank-line-plugin-0.1.3/pylint_blank_line_plugin/__init__.py
--rw-r--r--   0        0        0      140 2021-09-11 10:45:21.637364 pylint-blank-line-plugin-0.1.3/pylint_blank_line_plugin/blank_line.py
--rw-r--r--   0        0        0     4808 2021-09-11 11:13:18.640490 pylint-blank-line-plugin-0.1.3/pylint_blank_line_plugin/checker.py
--rw-r--r--   0        0        0      889 2021-09-11 11:14:44.872803 pylint-blank-line-plugin-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      991 2021-09-11 11:15:58.567818 pylint-blank-line-plugin-0.1.3/setup.py
--rw-r--r--   0        0        0     1152 2021-09-11 11:15:58.567994 pylint-blank-line-plugin-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-14 01:49:10.978642 pylint_blank_line_plugin-0.1.4/LICENSE
+-rw-r--r--   0        0        0      252 2023-04-16 15:04:48.601379 pylint_blank_line_plugin-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-16 14:45:11.396804 pylint_blank_line_plugin-0.1.4/pylint_blank_line_plugin/__init__.py
+-rw-r--r--   0        0        0      192 2023-04-16 14:46:50.003847 pylint_blank_line_plugin-0.1.4/pylint_blank_line_plugin/blank_line.py
+-rw-r--r--   0        0        0     4782 2023-04-16 15:03:46.453423 pylint_blank_line_plugin-0.1.4/pylint_blank_line_plugin/checker.py
+-rw-r--r--   0        0        0     1230 2023-04-16 15:04:25.474847 pylint_blank_line_plugin-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1268 1970-01-01 00:00:00.000000 pylint_blank_line_plugin-0.1.4/PKG-INFO
```

### Comparing `pylint-blank-line-plugin-0.1.3/LICENSE` & `pylint_blank_line_plugin-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pylint-blank-line-plugin-0.1.3/pyproject.toml` & `pylint_blank_line_plugin-0.1.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylint-blank-line-plugin"
-version = "0.1.3"
+version = "0.1.4"
 description = "Plugin for pylint which checks blank line before and after return, yield, raise, break, continue statements  "
 authors = ["Konstantin Shestakov <winmasta@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/winmasta"
 repository = "https://github.com/winmasta"
 keywords = ["pylint", "blank", "line", "lint"]
@@ -16,13 +16,32 @@
     "Topic :: Software Development :: Quality Assurance",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pylint = "*"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.test]
+optional = true
+
+[tool.poetry.group.test.dependencies]
+black = "*"
 pytest = "*"
+ruff = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pylint.basic]
+good-names = ["f", "i"]
+
+[tool.pylint."messages control"]
+disable = ["missing-docstring"]
+
+[tool.pylint.format]
+max-line-length = 119
+
+[tool.ruff]
+line-length = 119
+select = ["ALL"]
+ignore = ["D100", "D101", "D102", "D103", "D104", "D203", "D212"]
```

### Comparing `pylint-blank-line-plugin-0.1.3/PKG-INFO` & `pylint_blank_line_plugin-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: pylint-blank-line-plugin
-Version: 0.1.3
+Version: 0.1.4
 Summary: Plugin for pylint which checks blank line before and after return, yield, raise, break, continue statements  
 Home-page: https://github.com/winmasta
 License: MIT
 Keywords: pylint,blank,line,lint
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
 
@@ -25,10 +27,10 @@
 Install:
 ```bash
 pip install pylint-blank-line-plugin
 ```
 
 Usage:
 ```bash
-pylint --load-plugins blank_line FILES_TO_CHECK
+pylint --load-plugins pylint_blank_line_plugin FILES_TO_CHECK
 ```
```

