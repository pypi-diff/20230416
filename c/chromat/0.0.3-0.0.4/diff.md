# Comparing `tmp/chromat-0.0.3.tar.gz` & `tmp/chromat-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromat-0.0.3.tar", max compression
+gzip compressed data, was "chromat-0.0.4.tar", max compression
```

## Comparing `chromat-0.0.3.tar` & `chromat-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       61 2023-04-08 22:20:34.106730 chromat-0.0.3/chromat/__init__.py
--rw-r--r--   0        0        0      244 2023-04-07 19:33:13.563276 chromat-0.0.3/chromat/app.py
--rw-r--r--   0        0        0     1273 2023-04-08 22:21:02.542212 chromat-0.0.3/chromat/printing.py
--rw-r--r--   0        0        0      818 2023-04-08 22:19:46.760887 chromat-0.0.3/chromat/swatches.py
--rw-r--r--   0        0        0     3958 2023-04-08 22:19:40.309035 chromat-0.0.3/chromat/utils.py
--rw-r--r--   0        0        0     1312 2023-04-09 00:46:50.451732 chromat-0.0.3/pyproject.toml
--rw-r--r--   0        0        0       93 2023-04-03 02:42:30.536779 chromat-0.0.3/README.md
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 chromat-0.0.3/setup.py
--rw-r--r--   0        0        0     1158 1970-01-01 00:00:00.000000 chromat-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-04-14 16:30:12.300399 chromat-0.0.4/chromat/__init__.py
+-rw-r--r--   0        0        0     2405 2023-04-16 01:32:09.534293 chromat-0.0.4/chromat/console.py
+-rw-r--r--   0        0        0      146 2023-04-13 19:57:48.808921 chromat-0.0.4/chromat/palettes.py
+-rw-r--r--   0        0        0    10281 2023-04-16 01:30:18.308501 chromat-0.0.4/chromat/swatches.py
+-rw-r--r--   0        0        0     3004 2023-04-16 01:29:19.967497 chromat-0.0.4/chromat/utils.py
+-rw-r--r--   0        0        0     1239 2023-04-16 01:37:00.848418 chromat-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-04-03 02:42:30.536779 chromat-0.0.4/README.md
+-rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 chromat-0.0.4/setup.py
+-rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 chromat-0.0.4/PKG-INFO
```

### Comparing `chromat-0.0.3/pyproject.toml` & `chromat-0.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chromat"
-version = "0.0.3"
+version = "0.0.4"
 description = "color palettes! under heavy construction!"
 license = "GPL-3.0-or-later"
 authors = ["hex benjamin <hex@hexbenjam.in>"]
 readme = "README.md"
 repository = "https://github.com/hexbenjamin/chromat"
 keywords = ["color", "palette"]
 classifiers = [
@@ -32,20 +32,18 @@
     ".flake8",
     ".gitignore",
     "testing.py",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-textual = "^0.18.0"
-colour = "^0.1.5"
+rich = "^13.3.4"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 flake8 = "^6.0.0"
 mypy = "^1.1.1"
 pytest = "^7.2.2"
-textual = {extras = ["dev"], version = "^0.18.0"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `chromat-0.0.3/setup.py` & `chromat-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['chromat']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['colour>=0.1.5,<0.2.0', 'textual>=0.18.0,<0.19.0']
+['rich>=13.3.4,<14.0.0']
 
 setup_kwargs = {
     'name': 'chromat',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'color palettes! under heavy construction!',
     'long_description': '\ufeff# chromat: algorithmic color palettes\ncoming soon!\n\nhttps://github.com/hexbenjamin/chromat',
     'author': 'hex benjamin',
     'author_email': 'hex@hexbenjam.in',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/hexbenjamin/chromat',
```

### Comparing `chromat-0.0.3/PKG-INFO` & `chromat-0.0.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromat
-Version: 0.0.3
+Version: 0.0.4
 Summary: color palettes! under heavy construction!
 Home-page: https://github.com/hexbenjamin/chromat
 License: GPL-3.0-or-later
 Keywords: color,palette
 Author: hex benjamin
 Author-email: hex@hexbenjam.in
 Requires-Python: >=3.10,<4.0
@@ -16,16 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Artistic Software
 Classifier: Topic :: Utilities
-Requires-Dist: colour (>=0.1.5,<0.2.0)
-Requires-Dist: textual (>=0.18.0,<0.19.0)
+Requires-Dist: rich (>=13.3.4,<14.0.0)
 Project-URL: Repository, https://github.com/hexbenjamin/chromat
 Description-Content-Type: text/markdown
 
 ﻿# chromat: algorithmic color palettes
 coming soon!
 
 https://github.com/hexbenjamin/chromat
```

