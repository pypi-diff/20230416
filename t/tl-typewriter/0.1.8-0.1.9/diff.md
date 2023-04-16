# Comparing `tmp/tl_typewriter-0.1.8.tar.gz` & `tmp/tl_typewriter-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tl_typewriter-0.1.8.tar", last modified: Sun Apr 16 08:19:13 2023, max compression
+gzip compressed data, was "tl_typewriter-0.1.9.tar", last modified: Sun Apr 16 11:31:12 2023, max compression
```

## Comparing `tl_typewriter-0.1.8.tar` & `tl_typewriter-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 08:19:13.972407 tl_typewriter-0.1.8/
--rw-rw-rw-   0        0        0    11558 2023-04-16 06:54:47.000000 tl_typewriter-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      302 2023-04-16 08:19:13.972407 tl_typewriter-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-04-16 08:18:09.000000 tl_typewriter-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2023-04-16 08:19:13.972407 tl_typewriter-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      665 2023-04-16 08:18:36.000000 tl_typewriter-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:19:13.959232 tl_typewriter-0.1.8/tl_typewriter/
--rw-rw-rw-   0        0        0     1724 2023-04-16 08:09:50.000000 tl_typewriter-0.1.8/tl_typewriter/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 08:19:13.971404 tl_typewriter-0.1.8/tl_typewriter.egg-info/
--rw-rw-rw-   0        0        0      302 2023-04-16 08:19:13.000000 tl_typewriter-0.1.8/tl_typewriter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-04-16 08:19:13.000000 tl_typewriter-0.1.8/tl_typewriter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 08:19:13.000000 tl_typewriter-0.1.8/tl_typewriter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-04-16 08:19:13.000000 tl_typewriter-0.1.8/tl_typewriter.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-04-16 08:19:13.000000 tl_typewriter-0.1.8/tl_typewriter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-16 08:19:13.000000 tl_typewriter-0.1.8/tl_typewriter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 11:31:12.138488 tl_typewriter-0.1.9/
+-rw-rw-rw-   0        0        0    11558 2023-04-16 06:54:47.000000 tl_typewriter-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      302 2023-04-16 11:31:12.138488 tl_typewriter-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      594 2023-04-16 09:41:19.000000 tl_typewriter-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-16 11:31:12.139513 tl_typewriter-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      659 2023-04-16 11:23:50.000000 tl_typewriter-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 11:31:12.133018 tl_typewriter-0.1.9/tl_typewriter.egg-info/
+-rw-rw-rw-   0        0        0      302 2023-04-16 11:31:12.000000 tl_typewriter-0.1.9/tl_typewriter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-04-16 11:31:12.000000 tl_typewriter-0.1.9/tl_typewriter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 11:31:12.000000 tl_typewriter-0.1.9/tl_typewriter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-16 11:31:12.000000 tl_typewriter-0.1.9/tl_typewriter.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-04-16 11:31:12.000000 tl_typewriter-0.1.9/tl_typewriter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-16 11:31:12.000000 tl_typewriter-0.1.9/tl_typewriter.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 11:31:12.136467 tl_typewriter-0.1.9/typewriter/
+-rw-rw-rw-   0        0        0      127 2023-04-16 11:21:18.000000 tl_typewriter-0.1.9/typewriter/__main__.py
+-rw-rw-rw-   0        0        0     1763 2023-04-16 11:21:09.000000 tl_typewriter-0.1.9/typewriter/writer.py
```

### Comparing `tl_typewriter-0.1.8/LICENSE` & `tl_typewriter-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tl_typewriter-0.1.8/setup.py` & `tl_typewriter-0.1.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from pathlib import Path
 from setuptools import setup
 
 
 setup(
     name="tl_typewriter",
-    version='0.1.8',
+    version='0.1.9',
     description="pagination and bubble typewriter in translating manga",
     url="https://github.com/AbangTanYiHan/tl_typewriter",
     author="abangtan",
     license="Apache License 2.0",
     classifiers=[
         "Programming Language :: Python :: 3",
     ],
-    packages=['tl_typewriter'],
+    packages=['typewriter'],
     include_package_data=True,
     install_requires=[
         "fire",
         "keyboard",
         "loguru",
     ],
     entry_points={
         "console_scripts": [
-        'tl_typewriter = tl_typewriter.__main__:main'
+        'tl_typewriter = typewriter.__main__:main'
         ]
     },
 )
```

### Comparing `tl_typewriter-0.1.8/tl_typewriter/__main__.py` & `tl_typewriter-0.1.9/typewriter/writer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import keyboard
-import fire
 from pathlib import Path
 from loguru import logger
 
-def main(write_to='clipboard'):
+def run(write_to='file_path'):
+    logger.info(f"Writing to {write_to}")
     page = 0
     picture = 1
     box = 0
     text = 0
     bubble = 0
-    
-    if write_to == 'clipboard':
-        raise ValueError('write_to must be a path to a text file')
-    write_to = Path(write_to)
-    if write_to.suffix != '.txt':
-        raise ValueError('write_to must be a path to a text file')
-    logger.info('Using CPU')
-    logger.info('typewriter start')
-    while True:
-        event = keyboard.read_event()
-        logger.info('keyboard pressed')
-        if event.event_type == 'down':
-            result, page, picture, bubble, text, box = record_keystrokes(event, page, picture, bubble, text, box)
-            with write_to.open('a', encoding="utf-8") as f:
-                f.write(result)
+    if write_to == 'file_path':
+        raise ValueError('add file path')
+    else:
+        write_to = Path(write_to)
+        if write_to.suffix != '.txt':
+            raise ValueError('write_to must be a path to a text file')
+        logger.info(write_to)
+        logger.info('Using CPU')
+        logger.info('typewriter start')
+        while True:
+            event = keyboard.read_event()
+            logger.info('keyboard pressed')
+            if event.event_type == 'down':
+                result, page, picture, bubble, text, box = record_keystrokes(event, page, picture, bubble, text, box)
+                with write_to.open('a', encoding="utf-8") as f:
+                    f.write(result)
 
 def record_keystrokes(event, page, picture, bubble, text, box):
     result = ""
     if event.name == 'b':
         bubble += 1
         result = "b" + str(bubble)
         result = "P" + str(picture)  + result + ": "
@@ -46,10 +47,7 @@
         page += 1
         box = bubble = text = 0
         picture = 1
         result = "Page " + str(page) + "\n"
     else:
         result = ""
     return result, page, picture, bubble, text, box
-
-if __name__ == '__main__':
-    fire.Fire(main)
```

