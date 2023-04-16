# Comparing `tmp/oauthAPImojang-0.2.7.tar.gz` & `tmp/oauthAPImojang-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oauthAPImojang-0.2.7.tar", last modified: Sun Apr 16 20:49:12 2023, max compression
+gzip compressed data, was "oauthAPImojang-0.2.8.tar", last modified: Sun Apr 16 21:00:19 2023, max compression
```

## Comparing `oauthAPImojang-0.2.7.tar` & `oauthAPImojang-0.2.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 20:49:14.000000 oauthAPImojang-0.2.7/
--rw-rw-rw-   0        0        0       61 2023-04-16 20:49:14.000000 oauthAPImojang-0.2.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 20:49:14.000000 oauthAPImojang-0.2.7/oauthAPImojang/
--rw-rw-rw-   0        0        0      105 2023-04-16 20:02:36.000000 oauthAPImojang-0.2.7/oauthAPImojang/__init__.py
--rw-rw-rw-   0        0        0     6738 2023-04-16 20:47:36.000000 oauthAPImojang-0.2.7/oauthAPImojang/minecraftTHEapi.py
-drwxrwxrwx   0        0        0        0 2023-04-16 20:49:14.000000 oauthAPImojang-0.2.7/oauthAPImojang.egg-info/
--rw-rw-rw-   0        0        0       61 2023-04-16 20:49:14.000000 oauthAPImojang-0.2.7/oauthAPImojang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-04-16 20:49:14.000000 oauthAPImojang-0.2.7/oauthAPImojang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 20:49:14.000000 oauthAPImojang-0.2.7/oauthAPImojang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-16 20:49:14.000000 oauthAPImojang-0.2.7/oauthAPImojang.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-16 20:49:14.000000 oauthAPImojang-0.2.7/oauthAPImojang.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 20:49:14.000000 oauthAPImojang-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      223 2023-04-16 20:48:22.000000 oauthAPImojang-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:00:20.000000 oauthAPImojang-0.2.8/
+-rw-rw-rw-   0        0        0       61 2023-04-16 21:00:20.000000 oauthAPImojang-0.2.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 21:00:20.000000 oauthAPImojang-0.2.8/oauthAPImojang/
+-rw-rw-rw-   0        0        0      105 2023-04-16 20:02:36.000000 oauthAPImojang-0.2.8/oauthAPImojang/__init__.py
+-rw-rw-rw-   0        0        0    35164 2023-04-16 20:57:44.000000 oauthAPImojang-0.2.8/oauthAPImojang/minecraftTHEapi.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:00:20.000000 oauthAPImojang-0.2.8/oauthAPImojang.egg-info/
+-rw-rw-rw-   0        0        0       61 2023-04-16 21:00:20.000000 oauthAPImojang-0.2.8/oauthAPImojang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-04-16 21:00:20.000000 oauthAPImojang-0.2.8/oauthAPImojang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 21:00:20.000000 oauthAPImojang-0.2.8/oauthAPImojang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-16 21:00:20.000000 oauthAPImojang-0.2.8/oauthAPImojang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-16 21:00:20.000000 oauthAPImojang-0.2.8/oauthAPImojang.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 21:00:20.000000 oauthAPImojang-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      203 2023-04-16 20:59:18.000000 oauthAPImojang-0.2.8/setup.py
```

