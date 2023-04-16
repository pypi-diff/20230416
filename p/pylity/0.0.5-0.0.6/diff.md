# Comparing `tmp/pylity-0.0.5.tar.gz` & `tmp/pylity-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylity-0.0.5.tar", max compression
+gzip compressed data, was "pylity-0.0.6.tar", max compression
```

## Comparing `pylity-0.0.5.tar` & `pylity-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-04-15 16:46:34.425188 pylity-0.0.5/LICENSE
--rw-r--r--   0        0        0     4740 2023-04-15 16:46:34.425188 pylity-0.0.5/README.md
--rw-r--r--   0        0        0      882 2023-04-15 16:46:34.425188 pylity-0.0.5/pylity/Async.py
--rw-r--r--   0        0        0     1035 2023-04-15 16:46:34.429188 pylity-0.0.5/pylity/Collection.py
--rw-r--r--   0        0        0     4509 2023-04-15 16:46:34.429188 pylity-0.0.5/pylity/Function.py
--rw-r--r--   0        0        0     4819 2023-04-15 16:46:34.429188 pylity-0.0.5/pylity/Path.py
--rw-r--r--   0        0        0      473 2023-04-15 16:46:34.429188 pylity-0.0.5/pylity/String.py
--rw-r--r--   0        0        0      116 2023-04-15 16:46:34.429188 pylity-0.0.5/pylity/__init__.py
--rw-r--r--   0        0        0      713 2023-04-15 16:46:34.429188 pylity-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     5375 1970-01-01 00:00:00.000000 pylity-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-16 00:42:11.912757 pylity-0.0.6/LICENSE
+-rw-r--r--   0        0        0     5113 2023-04-16 00:42:11.912757 pylity-0.0.6/README.md
+-rw-r--r--   0        0        0      882 2023-04-16 00:42:11.912757 pylity-0.0.6/pylity/Async.py
+-rw-r--r--   0        0        0     1035 2023-04-16 00:42:11.912757 pylity-0.0.6/pylity/Collection.py
+-rw-r--r--   0        0        0     4509 2023-04-16 00:42:11.912757 pylity-0.0.6/pylity/Function.py
+-rw-r--r--   0        0        0     4819 2023-04-16 00:42:11.912757 pylity-0.0.6/pylity/Path.py
+-rw-r--r--   0        0        0      473 2023-04-16 00:42:11.912757 pylity-0.0.6/pylity/String.py
+-rw-r--r--   0        0        0      116 2023-04-16 00:42:11.912757 pylity-0.0.6/pylity/__init__.py
+-rw-r--r--   0        0        0      712 2023-04-16 00:42:11.912757 pylity-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5847 1970-01-01 00:00:00.000000 pylity-0.0.6/PKG-INFO
```

### Comparing `pylity-0.0.5/LICENSE` & `pylity-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pylity-0.0.5/README.md` & `pylity-0.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 </div>
 
 <div align="center">
 <br />
 
 [![code with love by Payadel](https://img.shields.io/badge/%3C%2F%3E%20with%20%E2%99%A5%20by-Payadel-ff1414.svg?style=flat-square)](https://github.com/Payadel)
 
+[![Build Status](https://img.shields.io/github/actions/workflow/status/Payadel/pylity/build.yaml?branch=dev)](https://github.com/Payadel/pylity/actions/workflows/build.yaml?query=branch%3Adev)
+[![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen.svg)](coverage.md)
+[![PyPI](https://img.shields.io/pypi/v/on_rails.svg)](https://pypi.org/project/on_rails/)
+
 ![GitHub](https://img.shields.io/github/license/Payadel/pylity)
 [![Pull Requests welcome](https://img.shields.io/badge/PRs-welcome-ff69b4.svg?style=flat-square)](https://github.com/Payadel/pylity/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22)
 
 </div>
 
 
 ## About
```

#### html2text {}

```diff
@@ -2,16 +2,21 @@
 
                               Getting_Started_Â»
 
               Report_a_Bug Â· Request_a_Feature . Ask_a_Question
 
           [![code with love by Payadel](https://img.shields.io/badge/
 %3C%2F%3E%20with%20%E2%99%A5%20by-Payadel-ff1414.svg?style=flat-square)](https:
-//github.com/Payadel) ![GitHub](https://img.shields.io/github/license/Payadel/
-  pylity) [![Pull Requests welcome](https://img.shields.io/badge/PRs-welcome-
+ //github.com/Payadel) [![Build Status](https://img.shields.io/github/actions/
+  workflow/status/Payadel/pylity/build.yaml?branch=dev)](https://github.com/
+ Payadel/pylity/actions/workflows/build.yaml?query=branch%3Adev) [![Coverage]
+(https://img.shields.io/badge/coverage-100%25-brightgreen.svg)](coverage.md) [!
+ [PyPI](https://img.shields.io/pypi/v/on_rails.svg)](https://pypi.org/project/
+ on_rails/) ![GitHub](https://img.shields.io/github/license/Payadel/pylity) [!
+       [Pull Requests welcome](https://img.shields.io/badge/PRs-welcome-
        ff69b4.svg?style=flat-square)](https://github.com/Payadel/pylity/
            issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22)
 ## About The `pylity` package is a set of utility and common functions for
 Python. **pylity** means `Python Utility`. When we work on different projects,
 there are usually functions that are **common** between the projects. Functions
 that we generally call Utility or helpers or something like that. Functions
 that are **independent** and can be used in different places. Well, instead of
```

### Comparing `pylity-0.0.5/pylity/Async.py` & `pylity-0.0.6/pylity/Async.py`

 * *Files identical despite different names*

### Comparing `pylity-0.0.5/pylity/Collection.py` & `pylity-0.0.6/pylity/Collection.py`

 * *Files identical despite different names*

### Comparing `pylity-0.0.5/pylity/Function.py` & `pylity-0.0.6/pylity/Function.py`

 * *Files identical despite different names*

### Comparing `pylity-0.0.5/pylity/Path.py` & `pylity-0.0.6/pylity/Path.py`

 * *Files identical despite different names*

### Comparing `pylity-0.0.5/pyproject.toml` & `pylity-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # https://python-poetry.org/docs/pyproject/
 [tool.poetry]
 name = "pylity"
-version = "0.0.5"
+version = "0.0.6"
 description = "A collection of utility functions for Python. pylity means Python Utility "
 authors = ["Payadel <payadelteam@gmail.com>"]
 license = "GPLV3"
 readme = "README.md"
 repository = "https://github.com/Payadel/pylity"
 keywords = ['utility', 'helpers']
 packages = [{ include = "pylity" }]
 
 [tool.poetry.dependencies]
-python = "^3.10"
-on-rails = "4.0.1"
+python = "^3.8"
+on-rails = "4.1.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.0"
 pytest = "^7.2.2"
 pylint = "^2.17.0"
 isort = "^5.12.0"
```

### Comparing `pylity-0.0.5/PKG-INFO` & `pylity-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: pylity
-Version: 0.0.5
+Version: 0.0.6
 Summary: A collection of utility functions for Python. pylity means Python Utility 
 Home-page: https://github.com/Payadel/pylity
 License: GPLV3
 Keywords: utility,helpers
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
-Requires-Dist: on-rails (==4.0.1)
+Requires-Dist: on-rails (==4.1.0)
 Project-URL: Repository, https://github.com/Payadel/pylity
 Description-Content-Type: text/markdown
 
 <div align="center">
   <h1>pylity</h1>
   <br />
   <a href="#getting-started"><strong>Getting Started »</strong></a>
@@ -30,14 +32,18 @@
 </div>
 
 <div align="center">
 <br />
 
 [![code with love by Payadel](https://img.shields.io/badge/%3C%2F%3E%20with%20%E2%99%A5%20by-Payadel-ff1414.svg?style=flat-square)](https://github.com/Payadel)
 
+[![Build Status](https://img.shields.io/github/actions/workflow/status/Payadel/pylity/build.yaml?branch=dev)](https://github.com/Payadel/pylity/actions/workflows/build.yaml?query=branch%3Adev)
+[![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen.svg)](coverage.md)
+[![PyPI](https://img.shields.io/pypi/v/on_rails.svg)](https://pypi.org/project/on_rails/)
+
 ![GitHub](https://img.shields.io/github/license/Payadel/pylity)
 [![Pull Requests welcome](https://img.shields.io/badge/PRs-welcome-ff69b4.svg?style=flat-square)](https://github.com/Payadel/pylity/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22)
 
 </div>
 
 
 ## About
```

#### html2text {}

```diff
@@ -1,26 +1,32 @@
-Metadata-Version: 2.1 Name: pylity Version: 0.0.5 Summary: A collection of
+Metadata-Version: 2.1 Name: pylity Version: 0.0.6 Summary: A collection of
 utility functions for Python. pylity means Python Utility Home-page: https://
 github.com/Payadel/pylity License: GPLV3 Keywords: utility,helpers Author:
-Payadel Author-email: payadelteam@gmail.com Requires-Python: >=3.10,<4.0
+Payadel Author-email: payadelteam@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: on-rails
-(==4.0.1) Project-URL: Repository, https://github.com/Payadel/pylity
-Description-Content-Type: text/markdown
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: on-rails (==4.1.0) Project-URL: Repository, https://github.com/
+Payadel/pylity Description-Content-Type: text/markdown
                              ****** pylity ******
 
                               Getting_Started_Â»
 
               Report_a_Bug Â· Request_a_Feature . Ask_a_Question
 
           [![code with love by Payadel](https://img.shields.io/badge/
 %3C%2F%3E%20with%20%E2%99%A5%20by-Payadel-ff1414.svg?style=flat-square)](https:
-//github.com/Payadel) ![GitHub](https://img.shields.io/github/license/Payadel/
-  pylity) [![Pull Requests welcome](https://img.shields.io/badge/PRs-welcome-
+ //github.com/Payadel) [![Build Status](https://img.shields.io/github/actions/
+  workflow/status/Payadel/pylity/build.yaml?branch=dev)](https://github.com/
+ Payadel/pylity/actions/workflows/build.yaml?query=branch%3Adev) [![Coverage]
+(https://img.shields.io/badge/coverage-100%25-brightgreen.svg)](coverage.md) [!
+ [PyPI](https://img.shields.io/pypi/v/on_rails.svg)](https://pypi.org/project/
+ on_rails/) ![GitHub](https://img.shields.io/github/license/Payadel/pylity) [!
+       [Pull Requests welcome](https://img.shields.io/badge/PRs-welcome-
        ff69b4.svg?style=flat-square)](https://github.com/Payadel/pylity/
            issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22)
 ## About The `pylity` package is a set of utility and common functions for
 Python. **pylity** means `Python Utility`. When we work on different projects,
 there are usually functions that are **common** between the projects. Functions
 that we generally call Utility or helpers or something like that. Functions
 that are **independent** and can be used in different places. Well, instead of
```

