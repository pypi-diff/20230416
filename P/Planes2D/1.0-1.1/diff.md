# Comparing `tmp/Planes2D-1.0.tar.gz` & `tmp/Planes2D-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Planes2D-1.0.tar", last modified: Sun Apr 16 16:36:15 2023, max compression
+gzip compressed data, was "Planes2D-1.1.tar", last modified: Sun Apr 16 16:47:43 2023, max compression
```

## Comparing `Planes2D-1.0.tar` & `Planes2D-1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 16:36:15.688002 Planes2D-1.0/
--rw-rw-rw-   0        0        0      120 2023-04-16 16:36:15.687004 Planes2D-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 16:36:15.659079 Planes2D-1.0/Planes2D/
--rw-rw-rw-   0        0        0     3099 2023-04-16 13:34:41.000000 Planes2D-1.0/Planes2D/Planes2D.py
--rw-rw-rw-   0        0        0       55 2023-04-16 16:33:47.000000 Planes2D-1.0/Planes2D/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 16:36:15.685009 Planes2D-1.0/Planes2D.egg-info/
--rw-rw-rw-   0        0        0      120 2023-04-16 16:36:15.000000 Planes2D-1.0/Planes2D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-04-16 16:36:15.000000 Planes2D-1.0/Planes2D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 16:36:15.000000 Planes2D-1.0/Planes2D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-16 16:36:15.000000 Planes2D-1.0/Planes2D.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 16:36:15.688002 Planes2D-1.0/setup.cfg
--rw-rw-rw-   0        0        0      262 2023-04-16 16:34:35.000000 Planes2D-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:47:43.263249 Planes2D-1.1/
+-rw-rw-rw-   0        0        0      134 2023-04-16 16:47:43.261252 Planes2D-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 16:47:43.246293 Planes2D-1.1/Planes2D/
+-rw-rw-rw-   0        0        0     3099 2023-04-16 13:34:41.000000 Planes2D-1.1/Planes2D/Planes2D.py
+-rw-rw-rw-   0        0        0       55 2023-04-16 16:33:47.000000 Planes2D-1.1/Planes2D/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 16:47:43.259257 Planes2D-1.1/Planes2D.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-04-16 16:47:43.000000 Planes2D-1.1/Planes2D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-04-16 16:47:43.000000 Planes2D-1.1/Planes2D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 16:47:43.000000 Planes2D-1.1/Planes2D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-16 16:47:43.000000 Planes2D-1.1/Planes2D.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 16:47:43.264246 Planes2D-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      228 2023-04-16 16:47:16.000000 Planes2D-1.1/setup.py
```

### Comparing `Planes2D-1.0/Planes2D/Planes2D.py` & `Planes2D-1.1/Planes2D/Planes2D.py`

 * *Files identical despite different names*

