# Comparing `tmp/Turk_game-1.0.0.tar.gz` & `tmp/Turk_game-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Turk_game-1.0.0.tar", last modified: Sat Apr 15 11:14:12 2023, max compression
+gzip compressed data, was "Turk_game-1.0.1.tar", last modified: Sun Apr 16 11:19:40 2023, max compression
```

## Comparing `Turk_game-1.0.0.tar` & `Turk_game-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 11:14:12.000000 Turk_game-1.0.0/
--rw-rw-rw-   0        0        0     1066 2019-06-03 23:39:34.000000 Turk_game-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      239 2023-04-15 11:14:14.000000 Turk_game-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2033 2019-06-03 23:39:34.000000 Turk_game-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 11:14:12.000000 Turk_game-1.0.0/Turk_game.egg-info/
--rw-rw-rw-   0        0        0      239 2023-04-15 11:14:12.000000 Turk_game-1.0.0/Turk_game.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-04-15 11:14:12.000000 Turk_game-1.0.0/Turk_game.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 11:14:12.000000 Turk_game-1.0.0/Turk_game.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 11:14:12.000000 Turk_game-1.0.0/Turk_game.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2662 2023-04-15 11:12:20.000000 Turk_game-1.0.0/Turk_game.py
--rw-rw-rw-   0        0        0       10 2023-04-11 06:37:16.000000 Turk_game-1.0.0/__init__.py
--rw-rw-rw-   0        0        0      170 2023-04-11 11:55:54.000000 Turk_game-1.0.0/a.py
--rw-rw-rw-   0        0        0       42 2023-04-15 11:14:14.000000 Turk_game-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      354 2023-04-15 11:13:56.000000 Turk_game-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 11:19:40.000000 Turk_game-1.0.1/
+-rw-rw-rw-   0        0        0     1066 2019-06-03 23:39:34.000000 Turk_game-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      278 2023-04-16 11:19:42.000000 Turk_game-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2033 2019-06-03 23:39:34.000000 Turk_game-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 11:19:40.000000 Turk_game-1.0.1/Turk_game.egg-info/
+-rw-rw-rw-   0        0        0      278 2023-04-16 11:19:40.000000 Turk_game-1.0.1/Turk_game.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-04-16 11:19:40.000000 Turk_game-1.0.1/Turk_game.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 11:19:40.000000 Turk_game-1.0.1/Turk_game.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 11:19:40.000000 Turk_game-1.0.1/Turk_game.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2553 2023-04-16 11:14:42.000000 Turk_game-1.0.1/Turk_game.py
+-rw-rw-rw-   0        0        0       10 2023-04-11 06:37:16.000000 Turk_game-1.0.1/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-04-16 11:19:42.000000 Turk_game-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      425 2023-04-16 11:19:32.000000 Turk_game-1.0.1/setup.py
```

### Comparing `Turk_game-1.0.0/LICENSE` & `Turk_game-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Turk_game-1.0.0/README.md` & `Turk_game-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `Turk_game-1.0.0/Turk_game.py` & `Turk_game-1.0.1/Turk_game.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,12 @@
 import pygame as pg
 import threading as th
 import sys, os
 
 
-def clear():
-    os.system('cls')
-
-clear()
-print("""Turk_game kullandıgınız icin tesekkurler""")
-
-
 def carpma_listesi(nesne,diger):
     x = nesne.collidelist(diger)
     if x != -1:
         return 1
     else:
         return 0
```

