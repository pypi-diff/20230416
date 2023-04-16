# Comparing `tmp/tl_typewriter-0.1.1.tar.gz` & `tmp/tl_typewriter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tl_typewriter-0.1.1.tar", last modified: Sun Apr 16 07:15:55 2023, max compression
+gzip compressed data, was "tl_typewriter-0.1.2.tar", last modified: Sun Apr 16 07:33:26 2023, max compression
```

## Comparing `tl_typewriter-0.1.1.tar` & `tl_typewriter-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 07:15:55.192354 tl_typewriter-0.1.1/
--rw-rw-rw-   0        0        0    11558 2023-04-16 06:54:47.000000 tl_typewriter-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      326 2023-04-16 07:15:55.191343 tl_typewriter-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      478 2023-04-16 07:06:14.000000 tl_typewriter-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-16 07:15:55.192354 tl_typewriter-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      814 2023-04-16 07:15:24.000000 tl_typewriter-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:15:55.179326 tl_typewriter-0.1.1/tl_typewriter/
--rw-rw-rw-   0        0        0     1554 2023-04-16 06:56:19.000000 tl_typewriter-0.1.1/tl_typewriter/tl_typewriter.py
-drwxrwxrwx   0        0        0        0 2023-04-16 07:15:55.190344 tl_typewriter-0.1.1/tl_typewriter.egg-info/
--rw-rw-rw-   0        0        0      326 2023-04-16 07:15:55.000000 tl_typewriter-0.1.1/tl_typewriter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-04-16 07:15:55.000000 tl_typewriter-0.1.1/tl_typewriter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 07:15:55.000000 tl_typewriter-0.1.1/tl_typewriter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-16 07:15:55.000000 tl_typewriter-0.1.1/tl_typewriter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-04-16 07:15:55.000000 tl_typewriter-0.1.1/tl_typewriter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-16 07:15:55.000000 tl_typewriter-0.1.1/tl_typewriter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 07:33:26.307843 tl_typewriter-0.1.2/
+-rw-rw-rw-   0        0        0    11558 2023-04-16 06:54:47.000000 tl_typewriter-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      302 2023-04-16 07:33:26.306836 tl_typewriter-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2023-04-16 07:18:45.000000 tl_typewriter-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-16 07:33:26.307843 tl_typewriter-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      670 2023-04-16 07:32:45.000000 tl_typewriter-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 07:33:26.294744 tl_typewriter-0.1.2/tl_typewriter/
+-rw-rw-rw-   0        0        0     1728 2023-04-16 07:32:28.000000 tl_typewriter-0.1.2/tl_typewriter/tl_typewriter.py
+drwxrwxrwx   0        0        0        0 2023-04-16 07:33:26.305725 tl_typewriter-0.1.2/tl_typewriter.egg-info/
+-rw-rw-rw-   0        0        0      302 2023-04-16 07:33:26.000000 tl_typewriter-0.1.2/tl_typewriter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-04-16 07:33:26.000000 tl_typewriter-0.1.2/tl_typewriter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 07:33:26.000000 tl_typewriter-0.1.2/tl_typewriter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-16 07:33:26.000000 tl_typewriter-0.1.2/tl_typewriter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-04-16 07:33:26.000000 tl_typewriter-0.1.2/tl_typewriter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-16 07:33:26.000000 tl_typewriter-0.1.2/tl_typewriter.egg-info/top_level.txt
```

### Comparing `tl_typewriter-0.1.1/LICENSE` & `tl_typewriter-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tl_typewriter-0.1.1/setup.py` & `tl_typewriter-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from pathlib import Path
 from setuptools import setup
 
-long_description = (Path(__file__).parent / "README.md").read_text('utf-8').split('# Installation')[0]
 
 setup(
     name="tl_typewriter",
-    version='0.1.1',
+    version='0.1.2',
     description="pagination and bubble typewriter in translating manga",
-    long_description=long_description,
     url="https://github.com/AbangTanYiHan/tl_typewriter",
     author="abangtan",
     license="Apache License 2.0",
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
     packages=['tl_typewriter'],
```

### Comparing `tl_typewriter-0.1.1/tl_typewriter/tl_typewriter.py` & `tl_typewriter-0.1.2/tl_typewriter/tl_typewriter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import keyboard
 import fire
 from pathlib import Path
 from loguru import logger
 
 
 
-def main(write_to='tl.txt'):
+def main(write_to='clipboard'):
     page = 0
     picture = 1
     box = 0
     text = 0
     bubble = 0
-    file = Path(write_to)
-    if file.suffix != '.txt':
-        raise ValueError('write_to must be either "clipboard" or a path to a text file')
+    
+    if write_to == 'clipboard':
+        raise ValueError('write_to must be a path to a text file')
+    write_to = Path(write_to)
+    if write_to.suffix != '.txt':
+        raise ValueError('write_to must be a path to a text file')
+    logger.info('Using CPU')
+    logger.info('typewriter start')
     while True:
-        logger.info('Using CPU')
+        logger.info('keyboard pressed')
         event = keyboard.read_event()
         if event.event_type == 'down':
             result, page, picture, bubble, text, box = record_keystrokes(event, page, picture, bubble, text, box)
-            with file.open('a', encoding="utf-8") as f:
+            with write_to.open('a', encoding="utf-8") as f:
                 f.write(result)
 
 def record_keystrokes(event, page, picture, bubble, text, box):
     result = ""
     if event.name == 'b':
         bubble += 1
         result = "b" + str(bubble)
```

