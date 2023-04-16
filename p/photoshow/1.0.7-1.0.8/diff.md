# Comparing `tmp/photoshow-1.0.7.tar.gz` & `tmp/photoshow-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Git\photoshow\dist\tmpu5po3p1q\photoshow-1.0.7.tar", last modified: Wed Oct 19 14:04:06 2022, max compression
+gzip compressed data, was "C:\Git\photoshow\dist\.tmp-gk_kal1b\photoshow-1.0.8.tar", last modified: Sun Apr 16 05:22:26 2023, max compression
```

## Comparing `photoshow-1.0.7.tar` & `photoshow-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-10-19 14:04:06.000000 photoshow-1.0.7/
--rw-rw-rw-   0        0        0     1085 2022-06-09 10:31:48.000000 photoshow-1.0.7/LICENCE.txt
--rw-rw-rw-   0        0        0     2368 2022-10-19 14:04:06.000000 photoshow-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1505 2022-08-25 15:06:44.000000 photoshow-1.0.7/README.rst
--rw-rw-rw-   0        0        0      142 2022-08-24 14:01:27.000000 photoshow-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-10-19 14:04:06.000000 photoshow-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1449 2022-10-19 13:38:48.000000 photoshow-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-19 14:04:06.000000 photoshow-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2022-10-19 14:04:06.000000 photoshow-1.0.7/src/photoshow/
--rw-rw-rw-   0        0        0      240 2022-09-30 14:54:37.000000 photoshow-1.0.7/src/photoshow/__init__.py
--rw-rw-rw-   0        0        0      639 2022-09-30 14:54:37.000000 photoshow-1.0.7/src/photoshow/__main__.py
--rw-rw-rw-   0        0        0    11707 2022-09-30 14:56:39.000000 photoshow-1.0.7/src/photoshow/_photoshow.py
-drwxrwxrwx   0        0        0        0 2022-10-19 14:04:06.000000 photoshow-1.0.7/src/photoshow.egg-info/
--rw-rw-rw-   0        0        0     2368 2022-10-19 14:04:05.000000 photoshow-1.0.7/src/photoshow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2022-10-19 14:04:05.000000 photoshow-1.0.7/src/photoshow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-19 14:04:05.000000 photoshow-1.0.7/src/photoshow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2022-10-19 14:04:05.000000 photoshow-1.0.7/src/photoshow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-10-19 14:04:05.000000 photoshow-1.0.7/src/photoshow.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 05:22:25.000000 photoshow-1.0.8/
+-rw-rw-rw-   0        0        0     1085 2022-06-09 10:31:48.000000 photoshow-1.0.8/LICENCE.txt
+-rw-rw-rw-   0        0        0     2368 2023-04-16 05:22:25.000000 photoshow-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1505 2022-08-25 15:06:44.000000 photoshow-1.0.8/README.rst
+-rw-rw-rw-   0        0        0      142 2022-08-24 14:01:27.000000 photoshow-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 05:22:25.000000 photoshow-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1449 2022-10-19 13:38:48.000000 photoshow-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 05:22:25.000000 photoshow-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 05:22:25.000000 photoshow-1.0.8/src/photoshow/
+-rw-rw-rw-   0        0        0      240 2023-04-16 05:05:53.000000 photoshow-1.0.8/src/photoshow/__init__.py
+-rw-rw-rw-   0        0        0      732 2023-04-16 05:19:03.000000 photoshow-1.0.8/src/photoshow/__main__.py
+-rw-rw-rw-   0        0        0    12014 2023-04-16 05:16:45.000000 photoshow-1.0.8/src/photoshow/_photoshow.py
+drwxrwxrwx   0        0        0        0 2023-04-16 05:22:25.000000 photoshow-1.0.8/src/photoshow.egg-info/
+-rw-rw-rw-   0        0        0     2368 2023-04-16 05:22:25.000000 photoshow-1.0.8/src/photoshow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-04-16 05:22:25.000000 photoshow-1.0.8/src/photoshow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 05:22:25.000000 photoshow-1.0.8/src/photoshow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-04-16 05:22:25.000000 photoshow-1.0.8/src/photoshow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-16 05:22:25.000000 photoshow-1.0.8/src/photoshow.egg-info/top_level.txt
```

### Comparing `photoshow-1.0.7/LICENCE.txt` & `photoshow-1.0.8/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `photoshow-1.0.7/PKG-INFO` & `photoshow-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photoshow
-Version: 1.0.7
+Version: 1.0.8
 Summary: Full screen photo slideshow
 Home-page: https://github.com/rikfair/photoshow
 Author: rikfair
 Author-email: mail4rik-pypi@yahoo.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rikfair/photoshow/issues
 Project-URL: Documentation, https://photoshow.readthedocs.io/
```

### Comparing `photoshow-1.0.7/README.rst` & `photoshow-1.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `photoshow-1.0.7/setup.py` & `photoshow-1.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `photoshow-1.0.7/src/photoshow/__main__.py` & `photoshow-1.0.8/src/photoshow/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # -----------------------------------------------
 
 import sys
 
 import photoshow
 
 # -----------------------------------------------
+# pylint: disable=broad-exception-raised
+# -----------------------------------------------
 
 
 if __name__ == '__main__':
     if len(sys.argv) != 2:
         raise Exception('Path or parameter file argument expected')
 
     print('Presenting photoshow')
```

### Comparing `photoshow-1.0.7/src/photoshow/_photoshow.py` & `photoshow-1.0.8/src/photoshow/_photoshow.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 import time
 import tkinter as tk
 
 import piexif
 from PIL import ImageTk, Image, ImageDraw, ImageFont, ImageFilter
 
 # -----------------------------------------------
+# pylint: disable=broad-exception-raised
+# -----------------------------------------------
 
 _CAPTIONS = 'captions'
 _DELAY = 'delay'
 _DELAY_TIME = 'delay_time'
 _DELAY_UNIT = 'delay_unit'
 _FONT_BIG = 'font_big'
 _FONT_PATH = 'font_path'
@@ -205,30 +207,33 @@
     if _PATH not in kwargs:
         raise Exception('No path provided')
     if not os.path.isdir(kwargs[_PATH]):
         raise Exception(f"Path is not a directory: {kwargs[_PATH]}")
 
     # Check for font if provided
 
+    captions = bool(kwargs.get(_CAPTIONS))
     font_path = kwargs.get(_FONT_PATH, '')
-    if font_path and not os.path.isfile(font_path):
-        raise Exception(f"Font not found: {font_path}")
-    if not font_path:
-        font_path = 'arial.ttf'
+    if captions:
+        if font_path and not os.path.isfile(font_path):
+            raise Exception(f"Font not found: {font_path}")
+        if not font_path:
+            # Sets arial as default. Only works on Windows. Linux needs font_path setting.
+            font_path = 'arial.ttf'
 
     # Return provided parameter or default values
 
     delay_time = int(kwargs.get(_DELAY_TIME, 15))
     delay_unit = kwargs.get(_DELAY_UNIT, 'S')
 
     return {
         _CAPTIONS: kwargs.get(_CAPTIONS.lower(), False),
         _DELAY: delay_time * {'M': 60}.get(delay_unit, 1),
-        _FONT_BIG: ImageFont.truetype(font_path, 40),
-        _FONT_SMALL: ImageFont.truetype(font_path, 16),
+        _FONT_BIG: ImageFont.truetype(font_path, 40) if captions else None,
+        _FONT_SMALL: ImageFont.truetype(font_path, 16) if captions else None,
         _MAX_PHOTOS: kwargs.get(_MAX_PHOTOS, 0),
         _PATH: kwargs[_PATH],
         _RANDOM: kwargs.get(_RANDOM, True),
         _REPEAT: kwargs.get(_REPEAT, True),
         _IGNORE: [_format_path(os.path.join(path, i)) for i in kwargs.get(_IGNORE, [])],
         _NEXT_PHOTO: False,
         _RUN: True
```

### Comparing `photoshow-1.0.7/src/photoshow.egg-info/PKG-INFO` & `photoshow-1.0.8/src/photoshow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photoshow
-Version: 1.0.7
+Version: 1.0.8
 Summary: Full screen photo slideshow
 Home-page: https://github.com/rikfair/photoshow
 Author: rikfair
 Author-email: mail4rik-pypi@yahoo.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/rikfair/photoshow/issues
 Project-URL: Documentation, https://photoshow.readthedocs.io/
```

