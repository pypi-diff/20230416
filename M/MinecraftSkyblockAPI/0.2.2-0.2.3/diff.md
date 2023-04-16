# Comparing `tmp/MinecraftSkyblockAPI-0.2.2.tar.gz` & `tmp/MinecraftSkyblockAPI-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MinecraftSkyblockAPI-0.2.2.tar", last modified: Sun Apr 16 19:54:39 2023, max compression
+gzip compressed data, was "MinecraftSkyblockAPI-0.2.3.tar", last modified: Sun Apr 16 20:04:12 2023, max compression
```

## Comparing `MinecraftSkyblockAPI-0.2.2.tar` & `MinecraftSkyblockAPI-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 19:54:40.000000 MinecraftSkyblockAPI-0.2.2/
-drwxrwxrwx   0        0        0        0 2023-04-16 19:54:40.000000 MinecraftSkyblockAPI-0.2.2/MinecraftSkyblockAPI.egg-info/
--rw-rw-rw-   0        0        0       91 2023-04-16 19:54:40.000000 MinecraftSkyblockAPI-0.2.2/MinecraftSkyblockAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-04-16 19:54:40.000000 MinecraftSkyblockAPI-0.2.2/MinecraftSkyblockAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 19:54:40.000000 MinecraftSkyblockAPI-0.2.2/MinecraftSkyblockAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-16 19:54:40.000000 MinecraftSkyblockAPI-0.2.2/MinecraftSkyblockAPI.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-04-16 19:54:40.000000 MinecraftSkyblockAPI-0.2.2/MinecraftSkyblockAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-04-16 19:54:40.000000 MinecraftSkyblockAPI-0.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 19:54:40.000000 MinecraftSkyblockAPI-0.2.2/minecraft-utilities-api/
--rw-rw-rw-   0        0        0        0 2023-04-16 18:29:22.000000 MinecraftSkyblockAPI-0.2.2/minecraft-utilities-api/__init__.py
--rw-rw-rw-   0        0        0     9527 2023-04-16 19:38:04.000000 MinecraftSkyblockAPI-0.2.2/minecraft-utilities-api/minecraft-api.py
--rw-rw-rw-   0        0        0       42 2023-04-16 19:54:40.000000 MinecraftSkyblockAPI-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      274 2023-04-16 19:54:36.000000 MinecraftSkyblockAPI-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 20:04:12.000000 MinecraftSkyblockAPI-0.2.3/
+drwxrwxrwx   0        0        0        0 2023-04-16 20:04:12.000000 MinecraftSkyblockAPI-0.2.3/MinecraftSkyblockAPI/
+-rw-rw-rw-   0        0        0      105 2023-04-16 20:02:36.000000 MinecraftSkyblockAPI-0.2.3/MinecraftSkyblockAPI/__init__.py
+-rw-rw-rw-   0        0        0     9527 2023-04-16 19:38:04.000000 MinecraftSkyblockAPI-0.2.3/MinecraftSkyblockAPI/minecraftTHEapi.py
+drwxrwxrwx   0        0        0        0 2023-04-16 20:04:12.000000 MinecraftSkyblockAPI-0.2.3/MinecraftSkyblockAPI.egg-info/
+-rw-rw-rw-   0        0        0       91 2023-04-16 20:04:12.000000 MinecraftSkyblockAPI-0.2.3/MinecraftSkyblockAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2023-04-16 20:04:12.000000 MinecraftSkyblockAPI-0.2.3/MinecraftSkyblockAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 20:04:12.000000 MinecraftSkyblockAPI-0.2.3/MinecraftSkyblockAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-16 20:04:12.000000 MinecraftSkyblockAPI-0.2.3/MinecraftSkyblockAPI.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-16 20:04:12.000000 MinecraftSkyblockAPI-0.2.3/MinecraftSkyblockAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-04-16 20:04:12.000000 MinecraftSkyblockAPI-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-16 20:04:12.000000 MinecraftSkyblockAPI-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      271 2023-04-16 20:03:42.000000 MinecraftSkyblockAPI-0.2.3/setup.py
```

### Comparing `MinecraftSkyblockAPI-0.2.2/minecraft-utilities-api/minecraft-api.py` & `MinecraftSkyblockAPI-0.2.3/MinecraftSkyblockAPI/minecraftTHEapi.py`

 * *Files identical despite different names*

