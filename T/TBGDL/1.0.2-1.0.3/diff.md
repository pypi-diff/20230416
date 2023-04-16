# Comparing `tmp/TBGDL-1.0.2.tar.gz` & `tmp/TBGDL-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TBGDL-1.0.2.tar", last modified: Fri Feb 24 20:22:49 2023, max compression
+gzip compressed data, was "TBGDL-1.0.3.tar", last modified: Sun Apr 16 09:51:57 2023, max compression
```

## Comparing `TBGDL-1.0.2.tar` & `TBGDL-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 20:22:49.780861 TBGDL-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-24 20:22:39.000000 TBGDL-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-02-24 20:22:49.780861 TBGDL-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-02-24 20:22:39.000000 TBGDL-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 20:22:49.780861 TBGDL-1.0.2/TBGDL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-02-24 20:22:49.000000 TBGDL-1.0.2/TBGDL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-24 20:22:49.000000 TBGDL-1.0.2/TBGDL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 20:22:49.000000 TBGDL-1.0.2/TBGDL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-24 20:22:49.000000 TBGDL-1.0.2/TBGDL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-24 20:22:49.000000 TBGDL-1.0.2/TBGDL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 20:22:49.780861 TBGDL-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-02-24 20:22:39.000000 TBGDL-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 20:22:49.780861 TBGDL-1.0.2/tbgdl/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-02-24 20:22:39.000000 TBGDL-1.0.2/tbgdl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:57.648882 TBGDL-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-16 09:51:43.000000 TBGDL-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-16 09:51:57.648882 TBGDL-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-16 09:51:43.000000 TBGDL-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:57.648882 TBGDL-1.0.3/TBGDL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-16 09:51:57.000000 TBGDL-1.0.3/TBGDL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-16 09:51:57.000000 TBGDL-1.0.3/TBGDL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 09:51:57.000000 TBGDL-1.0.3/TBGDL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-16 09:51:57.000000 TBGDL-1.0.3/TBGDL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 09:51:57.000000 TBGDL-1.0.3/TBGDL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 09:51:57.648882 TBGDL-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-16 09:51:43.000000 TBGDL-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:51:57.648882 TBGDL-1.0.3/tbgdl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-16 09:51:43.000000 TBGDL-1.0.3/tbgdl/__init__.py
```

### Comparing `TBGDL-1.0.2/LICENSE` & `TBGDL-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `TBGDL-1.0.2/PKG-INFO` & `TBGDL-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: TBGDL
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python library for creating text-based games.
 Home-page: https://github.com/Marko2155/TBGDL
 Author: Marko Camandioti
 Author-email: camandiotimarko@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/Marko2155/TBGDL#readme
 Project-URL: Source, https://github.com/Marko2155/TBGDL
 Project-URL: Tracker, https://github.com/Marko2155/TBGDL/issues
 Keywords: pygame,textadventure,text,game
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![TBGDL Logo](/docs/img/logo.png)
 # TBGDL
 A Python library for creating text-based games.
 
 # Features
 tbgdl_print(text, color) - Like print but also adds the ability to color the text. Makes cool ASCII art too!
 
 tbgdl_clear() - Clears the screen.
```

### Comparing `TBGDL-1.0.2/README.md` & `TBGDL-1.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+![TBGDL Logo](/docs/img/logo.png)
 # TBGDL
 A Python library for creating text-based games.
 
 # Features
 tbgdl_print(text, color) - Like print but also adds the ability to color the text. Makes cool ASCII art too!
 
 tbgdl_clear() - Clears the screen.
```

### Comparing `TBGDL-1.0.2/TBGDL.egg-info/PKG-INFO` & `TBGDL-1.0.3/TBGDL.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: TBGDL
-Version: 1.0.2
+Version: 1.0.3
 Summary: A Python library for creating text-based games.
 Home-page: https://github.com/Marko2155/TBGDL
 Author: Marko Camandioti
 Author-email: camandiotimarko@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/Marko2155/TBGDL#readme
 Project-URL: Source, https://github.com/Marko2155/TBGDL
 Project-URL: Tracker, https://github.com/Marko2155/TBGDL/issues
 Keywords: pygame,textadventure,text,game
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+![TBGDL Logo](/docs/img/logo.png)
 # TBGDL
 A Python library for creating text-based games.
 
 # Features
 tbgdl_print(text, color) - Like print but also adds the ability to color the text. Makes cool ASCII art too!
 
 tbgdl_clear() - Clears the screen.
```

### Comparing `TBGDL-1.0.2/setup.py` & `TBGDL-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='TBGDL',
     long_description_content_type='text/markdown',
     long_description=long_description,
     keywords="pygame, textadventure, text, game",
-    version='1.0.2',
+    version='1.0.3',
     packages=['tbgdl'],
     install_requires=[
         "colorama",
         "simpleaudio",
         "numpy",
         "musicalbeeps"
     ],
```

### Comparing `TBGDL-1.0.2/tbgdl/__init__.py` & `TBGDL-1.0.3/tbgdl/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -38,7 +38,11 @@
 def tbgdl_load_scene(scene):
     return scene
 
 def tbgdl_playsound(note, sound):
         player = musicalbeeps.Player(volume = 0.3, mute_output = False)
         player.play_note(note, sound)
 
+def tbgdl_AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA():
+    tbgdl_print("COVER YOUR EARS!", red)
+    player = musicalbeeps.Player(volume = 1, mute_output = False)
+    player.play_note("F3#", 100.0)
```

