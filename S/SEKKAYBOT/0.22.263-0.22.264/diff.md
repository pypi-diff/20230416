# Comparing `tmp/SEKKAYBOT-0.22.263.tar.gz` & `tmp/SEKKAYBOT-0.22.264.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SEKKAYBOT-0.22.263.tar", last modified: Thu Dec 22 13:44:51 2022, max compression
+gzip compressed data, was "SEKKAYBOT-0.22.264.tar", last modified: Sun Apr 16 11:06:31 2023, max compression
```

## Comparing `SEKKAYBOT-0.22.263.tar` & `SEKKAYBOT-0.22.264.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2022-12-22 13:44:51.036783 SEKKAYBOT-0.22.263/
--rw-rw-rw-   0        0        0      281 2022-12-22 13:44:51.021030 SEKKAYBOT-0.22.263/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-12-22 13:44:50.910122 SEKKAYBOT-0.22.263/SEKKAYBOT/
--rw-rw-rw-   0        0        0    54302 2022-12-22 13:43:58.000000 SEKKAYBOT-0.22.263/SEKKAYBOT/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-22 13:44:51.021030 SEKKAYBOT-0.22.263/SEKKAYBOT.egg-info/
--rw-rw-rw-   0        0        0      281 2022-12-22 13:44:50.000000 SEKKAYBOT-0.22.263/SEKKAYBOT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2022-12-22 13:44:50.000000 SEKKAYBOT-0.22.263/SEKKAYBOT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-22 13:44:50.000000 SEKKAYBOT-0.22.263/SEKKAYBOT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2022-12-22 13:44:50.000000 SEKKAYBOT-0.22.263/SEKKAYBOT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-12-22 13:44:50.000000 SEKKAYBOT-0.22.263/SEKKAYBOT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-22 13:44:51.036783 SEKKAYBOT-0.22.263/setup.cfg
--rw-rw-rw-   0        0        0      593 2022-12-22 13:44:18.000000 SEKKAYBOT-0.22.263/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 11:06:31.325916 SEKKAYBOT-0.22.264/
+-rw-rw-rw-   0        0        0      281 2023-04-16 11:06:31.325916 SEKKAYBOT-0.22.264/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 11:06:31.262193 SEKKAYBOT-0.22.264/SEKKAYBOT/
+-rw-rw-rw-   0        0        0    54302 2022-12-22 13:43:58.000000 SEKKAYBOT-0.22.264/SEKKAYBOT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 11:06:31.309773 SEKKAYBOT-0.22.264/SEKKAYBOT.egg-info/
+-rw-rw-rw-   0        0        0      281 2023-04-16 11:06:31.000000 SEKKAYBOT-0.22.264/SEKKAYBOT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-04-16 11:06:31.000000 SEKKAYBOT-0.22.264/SEKKAYBOT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 11:06:31.000000 SEKKAYBOT-0.22.264/SEKKAYBOT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-04-16 11:06:31.000000 SEKKAYBOT-0.22.264/SEKKAYBOT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-16 11:06:31.000000 SEKKAYBOT-0.22.264/SEKKAYBOT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 11:06:31.341640 SEKKAYBOT-0.22.264/setup.cfg
+-rw-rw-rw-   0        0        0      593 2023-04-16 11:05:54.000000 SEKKAYBOT-0.22.264/setup.py
```

### Comparing `SEKKAYBOT-0.22.263/SEKKAYBOT/__init__.py` & `SEKKAYBOT-0.22.264/SEKKAYBOT/__init__.py`

 * *Files identical despite different names*

### Comparing `SEKKAYBOT-0.22.263/setup.py` & `SEKKAYBOT-0.22.264/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
     
 setuptools.setup(
     name="SEKKAYBOT",
-    version="0.22.263",
+    version="0.22.264",
     author="Sekkay",
     description="Lobby bot.",
     url="https://www.youtube.com",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

