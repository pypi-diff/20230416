# Comparing `tmp/kenu-1.2.4.tar.gz` & `tmp/kenu-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kenu-1.2.4.tar", last modified: Sun Apr 16 14:09:06 2023, max compression
+gzip compressed data, was "kenu-1.2.5.tar", last modified: Sun Apr 16 14:11:21 2023, max compression
```

## Comparing `kenu-1.2.4.tar` & `kenu-1.2.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 14:09:06.345119 kenu-1.2.4/
--rw-rw-rw-   0        0        0      122 2023-04-16 14:09:06.343124 kenu-1.2.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 14:09:06.306222 kenu-1.2.4/kenu/
--rw-rw-rw-   0        0        0     5025 2023-03-24 18:10:30.000000 kenu-1.2.4/kenu/__init__.py
--rw-rw-rw-   0        0        0     8177 2023-03-31 17:35:51.000000 kenu-1.2.4/kenu/__main__.py
--rw-rw-rw-   0        0        0     4027 2023-04-16 14:03:32.000000 kenu-1.2.4/kenu/connect.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:09:06.340130 kenu-1.2.4/kenu.egg-info/
--rw-rw-rw-   0        0        0      122 2023-04-16 14:09:06.000000 kenu-1.2.4/kenu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-04-16 14:09:06.000000 kenu-1.2.4/kenu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 14:09:06.000000 kenu-1.2.4/kenu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-16 14:09:06.000000 kenu-1.2.4/kenu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-04-16 14:09:06.000000 kenu-1.2.4/kenu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-16 14:09:06.000000 kenu-1.2.4/kenu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 14:09:06.345119 kenu-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0      418 2023-04-16 14:08:31.000000 kenu-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:11:21.491537 kenu-1.2.5/
+-rw-rw-rw-   0        0        0      122 2023-04-16 14:11:21.489542 kenu-1.2.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 14:11:21.457627 kenu-1.2.5/kenu/
+-rw-rw-rw-   0        0        0     5025 2023-03-24 18:10:30.000000 kenu-1.2.5/kenu/__init__.py
+-rw-rw-rw-   0        0        0     8177 2023-03-31 17:35:51.000000 kenu-1.2.5/kenu/__main__.py
+-rw-rw-rw-   0        0        0     4027 2023-04-16 14:03:32.000000 kenu-1.2.5/kenu/connect.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:11:21.487547 kenu-1.2.5/kenu.egg-info/
+-rw-rw-rw-   0        0        0      122 2023-04-16 14:11:21.000000 kenu-1.2.5/kenu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-04-16 14:11:21.000000 kenu-1.2.5/kenu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 14:11:21.000000 kenu-1.2.5/kenu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-04-16 14:11:21.000000 kenu-1.2.5/kenu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-04-16 14:11:21.000000 kenu-1.2.5/kenu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-16 14:11:21.000000 kenu-1.2.5/kenu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 14:11:21.492536 kenu-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      423 2023-04-16 14:11:13.000000 kenu-1.2.5/setup.py
```

### Comparing `kenu-1.2.4/kenu/__init__.py` & `kenu-1.2.5/kenu/__init__.py`

 * *Files identical despite different names*

### Comparing `kenu-1.2.4/kenu/__main__.py` & `kenu-1.2.5/kenu/__main__.py`

 * *Files identical despite different names*

### Comparing `kenu-1.2.4/kenu/connect.py` & `kenu-1.2.5/kenu/connect.py`

 * *Files identical despite different names*

