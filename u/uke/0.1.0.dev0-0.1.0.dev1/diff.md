# Comparing `tmp/uke-0.1.0.dev0.tar.gz` & `tmp/uke-0.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uke-0.1.0.dev0.tar", max compression
+gzip compressed data, was "uke-0.1.0.dev1.tar", max compression
```

## Comparing `uke-0.1.0.dev0.tar` & `uke-0.1.0.dev1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1092 2023-04-16 01:58:22.882152 uke-0.1.0.dev0/LICENSE
--rw-r--r--   0        0        0     1901 2023-04-16 08:30:32.348929 uke-0.1.0.dev0/pyproject.toml
--rw-r--r--   0        0        0      612 2023-04-16 02:37:56.217611 uke-0.1.0.dev0/README.md
--rw-r--r--   0        0        0       28 2023-04-16 08:07:23.871567 uke-0.1.0.dev0/src/uke/__init__.py
--rw-r--r--   0        0        0       46 2023-04-09 04:06:46.354065 uke-0.1.0.dev0/src/uke/__main__.py
--rw-r--r--   0        0        0     6858 2023-04-11 13:30:38.631395 uke-0.1.0.dev0/src/uke/chord.py
--rw-r--r--   0        0        0      442 2023-04-16 03:03:08.077669 uke-0.1.0.dev0/src/uke/cli.py
--rw-r--r--   0        0        0        0 2023-04-09 02:18:43.210195 uke-0.1.0.dev0/src/uke/strum.py
--rw-r--r--   0        0        0      208 2023-04-11 14:00:03.571385 uke-0.1.0.dev0/src/uke/tmpl/__init__.py
--rw-r--r--   0        0        0      265 2023-04-11 14:49:26.411383 uke-0.1.0.dev0/src/uke/tmpl/base.jinja2
--rw-r--r--   0        0        0        0 2023-03-26 04:32:43.071785 uke-0.1.0.dev0/src/uke/tmpl/chord.jinja2
--rw-r--r--   0        0        0     3447 2023-04-13 13:39:34.207421 uke-0.1.0.dev0/src/uke/tuner.py
--rw-r--r--   0        0        0      493 2023-04-16 08:03:39.756924 uke-0.1.0.dev0/tests/audio/standard_pitch.py
--rw-r--r--   0        0        0     1958 2023-04-13 14:05:02.074245 uke-0.1.0.dev0/tests/audio/test_notes.py
--rw-r--r--   0        0        0      738 2023-04-13 14:09:08.978063 uke-0.1.0.dev0/tests/audio/test_notes_mini.py
--rw-r--r--   0        0        0      197 2023-04-16 08:02:55.511018 uke-0.1.0.dev0/tests/audio/test_plot_sin.py
--rw-r--r--   0        0        0      474 2023-04-11 14:53:29.781387 uke-0.1.0.dev0/tests/jinja2/test_chord_svg.py
--rw-r--r--   0        0        0     2277 1970-01-01 00:00:00.000000 uke-0.1.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-16 01:58:22.882152 uke-0.1.0.dev1/LICENSE
+-rw-r--r--   0        0        0     1887 2023-04-16 12:34:06.132529 uke-0.1.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0      624 2023-04-16 10:24:21.013355 uke-0.1.0.dev1/README.md
+-rw-r--r--   0        0        0      493 2023-04-16 08:03:39.756924 uke-0.1.0.dev1/tests/audio/standard_pitch.py
+-rw-r--r--   0        0        0     1958 2023-04-13 14:05:02.074245 uke-0.1.0.dev1/tests/audio/test_notes.py
+-rw-r--r--   0        0        0      738 2023-04-13 14:09:08.978063 uke-0.1.0.dev1/tests/audio/test_notes_mini.py
+-rw-r--r--   0        0        0      197 2023-04-16 08:02:55.511018 uke-0.1.0.dev1/tests/audio/test_plot_sin.py
+-rw-r--r--   0        0        0      474 2023-04-11 14:53:29.781387 uke-0.1.0.dev1/tests/jinja2/test_chord_svg.py
+-rw-r--r--   0        0        0       28 2023-04-16 12:34:18.573576 uke-0.1.0.dev1/uke/__init__.py
+-rw-r--r--   0        0        0       46 2023-04-09 04:06:46.354065 uke-0.1.0.dev1/uke/__main__.py
+-rw-r--r--   0        0        0     6858 2023-04-11 13:30:38.631395 uke-0.1.0.dev1/uke/chord.py
+-rw-r--r--   0        0        0      479 2023-04-16 13:19:16.597359 uke-0.1.0.dev1/uke/cli.py
+-rw-r--r--   0        0        0        0 2023-04-09 02:18:43.210195 uke-0.1.0.dev1/uke/strum.py
+-rw-r--r--   0        0        0      208 2023-04-11 14:00:03.571385 uke-0.1.0.dev1/uke/tmpl/__init__.py
+-rw-r--r--   0        0        0      265 2023-04-11 14:49:26.411383 uke-0.1.0.dev1/uke/tmpl/base.jinja2
+-rw-r--r--   0        0        0        0 2023-03-26 04:32:43.071785 uke-0.1.0.dev1/uke/tmpl/chord.jinja2
+-rw-r--r--   0        0        0     3447 2023-04-13 13:39:34.207421 uke-0.1.0.dev1/uke/tuner.py
+-rw-r--r--   0        0        0     2289 1970-01-01 00:00:00.000000 uke-0.1.0.dev1/PKG-INFO
```

### Comparing `uke-0.1.0.dev0/LICENSE` & `uke-0.1.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `uke-0.1.0.dev0/pyproject.toml` & `uke-0.1.0.dev1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uke"
-version = "0.1.0.dev0"
+version = "0.1.0.dev1"
 description = "Creating Ukulele Chord and Strumming Patterns Diagrams in SVG with Python"
 authors = ["llxlr <i@xhlr.top>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/llxlr/uke"
 repository = "https://github.com/llxlr/uke"
 documentation = "https://github.com/llxlr/uke#readme"
@@ -22,15 +22,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Multimedia :: Sound/Audio",
     "Topic :: Multimedia :: Graphics",
 ]
 packages = [
-    { include = "uke", from = "src" }
+    { include = "uke" }
 ]
 include = [
     { path = "tests", format = "sdist" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.11"
```

### Comparing `uke-0.1.0.dev0/src/uke/chord.py` & `uke-0.1.0.dev1/uke/chord.py`

 * *Files identical despite different names*

### Comparing `uke-0.1.0.dev0/src/uke/tuner.py` & `uke-0.1.0.dev1/uke/tuner.py`

 * *Files identical despite different names*

### Comparing `uke-0.1.0.dev0/tests/audio/test_notes.py` & `uke-0.1.0.dev1/tests/audio/test_notes.py`

 * *Files identical despite different names*

### Comparing `uke-0.1.0.dev0/tests/audio/test_notes_mini.py` & `uke-0.1.0.dev1/tests/audio/test_notes_mini.py`

 * *Files identical despite different names*

### Comparing `uke-0.1.0.dev0/PKG-INFO` & `uke-0.1.0.dev1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uke
-Version: 0.1.0.dev0
+Version: 0.1.0.dev1
 Summary: Creating Ukulele Chord and Strumming Patterns Diagrams in SVG with Python
 Home-page: https://github.com/llxlr/uke
 License: MIT
 Keywords: music,ukulele,uke,uku,chord,audio,svg,strumming patterns
 Author: llxlr
 Author-email: i@xhlr.top
 Requires-Python: >=3.7,<3.11
@@ -37,15 +37,15 @@
 Project-URL: Repository, https://github.com/llxlr/uke
 Description-Content-Type: text/markdown
 
 # uke
 
 [![PyPI - Version](https://img.shields.io/pypi/v/uke.svg)](https://pypi.org/project/uke)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/uke.svg)](https://pypi.org/project/uke)
-[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
+[![Poetry project](https://img.shields.io/badge/%F0%9F%A6%84-Poetry-60A5FA.svg)](https://github.com/python-poetry/poetry)
 
 -----
 
 **Table of Contents**
 
 - [Installation](#installation)
 - [License](#license)
```

