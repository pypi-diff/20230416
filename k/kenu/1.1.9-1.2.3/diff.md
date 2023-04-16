# Comparing `tmp/kenu-1.1.9.tar.gz` & `tmp/kenu-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kenu-1.1.9.tar", last modified: Sun Apr 16 14:04:12 2023, max compression
+gzip compressed data, was "kenu-1.2.3.tar", last modified: Sun Apr 16 14:05:55 2023, max compression
```

## Comparing `kenu-1.1.9.tar` & `kenu-1.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 14:04:12.181970 kenu-1.1.9/
--rw-rw-rw-   0        0        0      122 2023-04-16 14:04:12.179974 kenu-1.1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 14:04:12.124123 kenu-1.1.9/kenu/
--rw-rw-rw-   0        0        0     5025 2023-03-24 18:10:30.000000 kenu-1.1.9/kenu/__init__.py
--rw-rw-rw-   0        0        0     8177 2023-03-31 17:35:51.000000 kenu-1.1.9/kenu/__main__.py
--rw-rw-rw-   0        0        0     4027 2023-04-16 14:03:32.000000 kenu-1.1.9/kenu/connect.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:04:12.177014 kenu-1.1.9/kenu.egg-info/
--rw-rw-rw-   0        0        0      122 2023-04-16 14:04:11.000000 kenu-1.1.9/kenu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-04-16 14:04:11.000000 kenu-1.1.9/kenu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 14:04:11.000000 kenu-1.1.9/kenu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-16 14:04:11.000000 kenu-1.1.9/kenu.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       19 2023-04-16 14:04:11.000000 kenu-1.1.9/kenu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-04-16 14:04:11.000000 kenu-1.1.9/kenu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 14:04:12.182973 kenu-1.1.9/setup.cfg
--rw-rw-rw-   0        0        0      385 2023-04-16 14:04:07.000000 kenu-1.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:05:55.227976 kenu-1.2.3/
+-rw-rw-rw-   0        0        0      122 2023-04-16 14:05:55.225970 kenu-1.2.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 14:05:55.193060 kenu-1.2.3/kenu/
+-rw-rw-rw-   0        0        0     5025 2023-03-24 18:10:30.000000 kenu-1.2.3/kenu/__init__.py
+-rw-rw-rw-   0        0        0     8177 2023-03-31 17:35:51.000000 kenu-1.2.3/kenu/__main__.py
+-rw-rw-rw-   0        0        0     4027 2023-04-16 14:03:32.000000 kenu-1.2.3/kenu/connect.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:05:55.221980 kenu-1.2.3/kenu.egg-info/
+-rw-rw-rw-   0        0        0      122 2023-04-16 14:05:54.000000 kenu-1.2.3/kenu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-04-16 14:05:55.000000 kenu-1.2.3/kenu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 14:05:54.000000 kenu-1.2.3/kenu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-04-16 14:05:54.000000 kenu-1.2.3/kenu.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       19 2023-04-16 14:05:54.000000 kenu-1.2.3/kenu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-16 14:05:54.000000 kenu-1.2.3/kenu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 14:05:55.228964 kenu-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      386 2023-04-16 14:05:41.000000 kenu-1.2.3/setup.py
```

### Comparing `kenu-1.1.9/kenu/__init__.py` & `kenu-1.2.3/kenu/__init__.py`

 * *Files identical despite different names*

### Comparing `kenu-1.1.9/kenu/__main__.py` & `kenu-1.2.3/kenu/__main__.py`

 * *Files identical despite different names*

### Comparing `kenu-1.1.9/kenu/connect.py` & `kenu-1.2.3/kenu/connect.py`

 * *Files identical despite different names*

