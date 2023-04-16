# Comparing `tmp/ttlo-1.0.0.tar.gz` & `tmp/ttlo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttlo-1.0.0.tar", last modified: Sun Apr 16 20:19:17 2023, max compression
+gzip compressed data, was "ttlo-1.0.1.tar", last modified: Sun Apr 16 20:21:17 2023, max compression
```

## Comparing `ttlo-1.0.0.tar` & `ttlo-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 20:19:17.106640 ttlo-1.0.0/
--rw-rw-rw-   0        0        0     1092 2023-04-16 20:14:07.000000 ttlo-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      287 2023-04-16 20:19:17.106640 ttlo-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-16 20:19:17.111614 ttlo-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      382 2023-04-16 20:14:36.000000 ttlo-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 20:19:17.078828 ttlo-1.0.0/ttlo/
--rw-rw-rw-   0        0        0        0 2023-04-16 20:10:05.000000 ttlo-1.0.0/ttlo/__init__.py
--rw-rw-rw-   0        0        0      263 2023-04-16 20:12:47.000000 ttlo-1.0.0/ttlo/b.py
--rw-rw-rw-   0        0        0      139 2023-04-16 20:19:14.000000 ttlo-1.0.0/ttlo/ttlo.py
-drwxrwxrwx   0        0        0        0 2023-04-16 20:19:17.102618 ttlo-1.0.0/ttlo.egg-info/
--rw-rw-rw-   0        0        0      287 2023-04-16 20:19:16.000000 ttlo-1.0.0/ttlo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-04-16 20:19:16.000000 ttlo-1.0.0/ttlo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 20:19:16.000000 ttlo-1.0.0/ttlo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-16 20:19:16.000000 ttlo-1.0.0/ttlo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 20:21:17.672735 ttlo-1.0.1/
+-rw-rw-rw-   0        0        0     1092 2023-04-16 20:14:07.000000 ttlo-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      287 2023-04-16 20:21:17.673732 ttlo-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-16 20:21:17.680897 ttlo-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      382 2023-04-16 20:21:14.000000 ttlo-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 20:21:17.621006 ttlo-1.0.1/ttlo/
+-rw-rw-rw-   0        0        0       35 2023-04-16 20:21:04.000000 ttlo-1.0.1/ttlo/__init__.py
+-rw-rw-rw-   0        0        0      263 2023-04-16 20:12:47.000000 ttlo-1.0.1/ttlo/b.py
+-rw-rw-rw-   0        0        0      139 2023-04-16 20:19:14.000000 ttlo-1.0.1/ttlo/ttlo.py
+drwxrwxrwx   0        0        0        0 2023-04-16 20:21:17.666666 ttlo-1.0.1/ttlo.egg-info/
+-rw-rw-rw-   0        0        0      287 2023-04-16 20:21:17.000000 ttlo-1.0.1/ttlo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-04-16 20:21:17.000000 ttlo-1.0.1/ttlo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 20:21:17.000000 ttlo-1.0.1/ttlo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-04-16 20:21:17.000000 ttlo-1.0.1/ttlo.egg-info/top_level.txt
```

### Comparing `ttlo-1.0.0/LICENSE` & `ttlo-1.0.1/LICENSE`

 * *Files identical despite different names*

