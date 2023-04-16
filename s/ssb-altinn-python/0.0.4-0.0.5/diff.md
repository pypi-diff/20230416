# Comparing `tmp/ssb_altinn_python-0.0.4.tar.gz` & `tmp/ssb_altinn_python-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_altinn_python-0.0.4.tar", max compression
+gzip compressed data, was "ssb_altinn_python-0.0.5.tar", max compression
```

## Comparing `ssb_altinn_python-0.0.4.tar` & `ssb_altinn_python-0.0.5.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-04-05 22:12:36.710211 ssb_altinn_python-0.0.4/LICENSE
--rw-r--r--   0        0        0     2808 2023-04-05 22:12:36.710211 ssb_altinn_python-0.0.4/README.md
--rw-r--r--   0        0        0     1932 2023-04-05 22:12:49.542281 ssb_altinn_python-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       25 2023-04-05 22:12:36.714211 ssb_altinn_python-0.0.4/src/altinn/__init__.py
--rw-r--r--   0        0        0      110 2023-04-05 22:12:49.542281 ssb_altinn_python-0.0.4/src/altinn/__main__.py
--rw-r--r--   0        0        0     1217 2023-04-05 22:12:49.542281 ssb_altinn_python-0.0.4/src/altinn/main.py
--rw-r--r--   0        0        0        0 2023-04-05 22:12:36.714211 ssb_altinn_python-0.0.4/src/altinn/py.typed
--rw-r--r--   0        0        0     3671 1970-01-01 00:00:00.000000 ssb_altinn_python-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-04-16 19:33:04.808758 ssb_altinn_python-0.0.5/LICENSE
+-rw-r--r--   0        0        0     2844 2023-04-16 19:33:17.780731 ssb_altinn_python-0.0.5/README.md
+-rw-r--r--   0        0        0     1954 2023-04-16 19:33:17.784731 ssb_altinn_python-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       78 2023-04-16 19:33:17.784731 ssb_altinn_python-0.0.5/src/altinn/__init__.py
+-rw-r--r--   0        0        0      116 2023-04-16 19:33:17.784731 ssb_altinn_python-0.0.5/src/altinn/__main__.py
+-rw-r--r--   0        0        0     1988 2023-04-16 19:33:17.784731 ssb_altinn_python-0.0.5/src/altinn/file.py
+-rw-r--r--   0        0        0      419 2023-04-16 19:33:17.784731 ssb_altinn_python-0.0.5/src/altinn/flatten.py
+-rw-r--r--   0        0        0       35 2023-04-16 19:33:17.784731 ssb_altinn_python-0.0.5/src/altinn/parser.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:33:04.808758 ssb_altinn_python-0.0.5/src/altinn/py.typed
+-rw-r--r--   0        0        0       56 2023-04-16 19:33:17.784731 ssb_altinn_python-0.0.5/src/altinn/utils.py
+-rw-r--r--   0        0        0     3750 1970-01-01 00:00:00.000000 ssb_altinn_python-0.0.5/PKG-INFO
```

### Comparing `ssb_altinn_python-0.0.4/LICENSE` & `ssb_altinn_python-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_altinn_python-0.0.4/README.md` & `ssb_altinn_python-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,26 +22,28 @@
 [black]: https://github.com/psf/black
 
 ## Features
 
 This is work-in-progress Python-package for dealing with xml-data from Altinn3.
 
 ```python
-from altinn import __main__
+from altinn import FileInfo
 
-x = __main__.XmlFile(
+x = FileInfo(
     "gs://ssb-prod-dapla-felles-data-delt/altinn3/form_dc551844cd74.xml"
 )
 
 x.filename()
-
+# Returns the filename: form_dc551844cd74
 ```
 
 ## Requirements
 
+s
+
 - TODO
 
 ## Installation
 
 You can install _SSB Altinn Python_ via [pip] from [PyPI]:
 
 ```console
```

### Comparing `ssb_altinn_python-0.0.4/pyproject.toml` & `ssb_altinn_python-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-altinn-python"
-version = "0.0.4"
+version = "0.0.5"
 description = "SSB Altinn Python"
 authors = ["Øyvind Bruer-Skarsbø <obr@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/skars82/ssb-altinn-python"
 repository = "https://github.com/skars82/ssb-altinn-python"
 documentation = "https://ssb-altinn-python.readthedocs.io"
@@ -19,14 +19,15 @@
 Changelog = "https://github.com/skars82/ssb-altinn-python/releases"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = ">=8.0.1"
 pytest = "^7.2.2"
 dapla-toolbelt = "^1.6.2"
+defusedxml = "^0.7.1"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
```

### Comparing `ssb_altinn_python-0.0.4/PKG-INFO` & `ssb_altinn_python-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: ssb-altinn-python
-Version: 0.0.4
+Version: 0.0.5
 Summary: SSB Altinn Python
 Home-page: https://github.com/skars82/ssb-altinn-python
 License: MIT
 Author: Øyvind Bruer-Skarsbø
 Author-email: obr@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.1)
 Requires-Dist: dapla-toolbelt (>=1.6.2,<2.0.0)
+Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: pytest (>=7.2.2,<8.0.0)
 Project-URL: Changelog, https://github.com/skars82/ssb-altinn-python/releases
 Project-URL: Documentation, https://ssb-altinn-python.readthedocs.io
 Project-URL: Repository, https://github.com/skars82/ssb-altinn-python
 Description-Content-Type: text/markdown
 
 # SSB Altinn Python
@@ -44,26 +45,28 @@
 [black]: https://github.com/psf/black
 
 ## Features
 
 This is work-in-progress Python-package for dealing with xml-data from Altinn3.
 
 ```python
-from altinn import __main__
+from altinn import FileInfo
 
-x = __main__.XmlFile(
+x = FileInfo(
     "gs://ssb-prod-dapla-felles-data-delt/altinn3/form_dc551844cd74.xml"
 )
 
 x.filename()
-
+# Returns the filename: form_dc551844cd74
 ```
 
 ## Requirements
 
+s
+
 - TODO
 
 ## Installation
 
 You can install _SSB Altinn Python_ via [pip] from [PyPI]:
 
 ```console
```

