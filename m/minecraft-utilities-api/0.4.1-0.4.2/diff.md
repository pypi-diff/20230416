# Comparing `tmp/minecraft-utilities-api-0.4.1.tar.gz` & `tmp/minecraft-utilities-api-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraft-utilities-api-0.4.1.tar", last modified: Sun Apr 16 19:45:19 2023, max compression
+gzip compressed data, was "minecraft-utilities-api-0.4.2.tar", last modified: Sun Apr 16 19:48:26 2023, max compression
```

## Comparing `minecraft-utilities-api-0.4.1.tar` & `minecraft-utilities-api-0.4.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 19:45:20.000000 minecraft-utilities-api-0.4.1/
--rw-rw-rw-   0        0        0       94 2023-04-16 19:45:20.000000 minecraft-utilities-api-0.4.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 19:45:20.000000 minecraft-utilities-api-0.4.1/minecraft-utilities-api/
--rw-rw-rw-   0        0        0        0 2023-04-16 18:29:22.000000 minecraft-utilities-api-0.4.1/minecraft-utilities-api/__init__.py
--rw-rw-rw-   0        0        0     9527 2023-04-16 19:38:04.000000 minecraft-utilities-api-0.4.1/minecraft-utilities-api/minecraft-api.py
-drwxrwxrwx   0        0        0        0 2023-04-16 19:45:20.000000 minecraft-utilities-api-0.4.1/minecraft_utilities_api.egg-info/
--rw-rw-rw-   0        0        0       94 2023-04-16 19:45:20.000000 minecraft-utilities-api-0.4.1/minecraft_utilities_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-04-16 19:45:20.000000 minecraft-utilities-api-0.4.1/minecraft_utilities_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 19:45:20.000000 minecraft-utilities-api-0.4.1/minecraft_utilities_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-16 19:45:20.000000 minecraft-utilities-api-0.4.1/minecraft_utilities_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-16 19:45:20.000000 minecraft-utilities-api-0.4.1/minecraft_utilities_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 19:45:20.000000 minecraft-utilities-api-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0      298 2023-04-16 19:45:04.000000 minecraft-utilities-api-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 19:48:26.000000 minecraft-utilities-api-0.4.2/
+-rw-rw-rw-   0        0        0       94 2023-04-16 19:48:28.000000 minecraft-utilities-api-0.4.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 19:48:26.000000 minecraft-utilities-api-0.4.2/minecraft-utilities-api/
+-rw-rw-rw-   0        0        0        0 2023-04-16 18:29:22.000000 minecraft-utilities-api-0.4.2/minecraft-utilities-api/__init__.py
+-rw-rw-rw-   0        0        0     9527 2023-04-16 19:38:04.000000 minecraft-utilities-api-0.4.2/minecraft-utilities-api/minecraft-api.py
+drwxrwxrwx   0        0        0        0 2023-04-16 19:48:26.000000 minecraft-utilities-api-0.4.2/minecraft_utilities_api.egg-info/
+-rw-rw-rw-   0        0        0       94 2023-04-16 19:48:26.000000 minecraft-utilities-api-0.4.2/minecraft_utilities_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2023-04-16 19:48:26.000000 minecraft-utilities-api-0.4.2/minecraft_utilities_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 19:48:26.000000 minecraft-utilities-api-0.4.2/minecraft_utilities_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-16 19:48:26.000000 minecraft-utilities-api-0.4.2/minecraft_utilities_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-04-16 19:48:26.000000 minecraft-utilities-api-0.4.2/minecraft_utilities_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 19:48:28.000000 minecraft-utilities-api-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      277 2023-04-16 19:48:10.000000 minecraft-utilities-api-0.4.2/setup.py
```

### Comparing `minecraft-utilities-api-0.4.1/minecraft-utilities-api/minecraft-api.py` & `minecraft-utilities-api-0.4.2/minecraft-utilities-api/minecraft-api.py`

 * *Files identical despite different names*

