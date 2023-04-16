# Comparing `tmp/rssfixer-0.0.2.tar.gz` & `tmp/rssfixer-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rssfixer-0.0.2.tar", last modified: Sun Apr 16 12:15:42 2023, max compression
+gzip compressed data, was "rssfixer-0.0.3.tar", last modified: Sun Apr 16 13:37:38 2023, max compression
```

## Comparing `rssfixer-0.0.2.tar` & `rssfixer-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-16 12:15:42.140343 rssfixer-0.0.2/
--rw-r--r--   0 reuteras   (501) staff       (20)     1058 2023-04-16 10:16:56.000000 rssfixer-0.0.2/LICENSE
--rw-r--r--   0 reuteras   (501) staff       (20)      529 2023-04-16 12:15:42.140220 rssfixer-0.0.2/PKG-INFO
--rw-r--r--   0 reuteras   (501) staff       (20)       11 2023-04-16 11:28:48.000000 rssfixer-0.0.2/README.md
--rw-r--r--   0 reuteras   (501) staff       (20)      774 2023-04-16 12:15:19.000000 rssfixer-0.0.2/pyproject.toml
--rw-r--r--   0 reuteras   (501) staff       (20)       38 2023-04-16 12:15:42.140386 rssfixer-0.0.2/setup.cfg
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-16 12:15:42.138023 rssfixer-0.0.2/src/
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-16 12:15:42.138919 rssfixer-0.0.2/src/rssfixer/
--rw-r--r--   0 reuteras   (501) staff       (20)       60 2023-04-16 12:15:09.000000 rssfixer-0.0.2/src/rssfixer/__init__.py
--rw-r--r--   0 reuteras   (501) staff       (20)     2825 2023-04-16 11:26:17.000000 rssfixer-0.0.2/src/rssfixer/rss.py
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-16 12:15:42.140051 rssfixer-0.0.2/src/rssfixer.egg-info/
--rw-r--r--   0 reuteras   (501) staff       (20)      529 2023-04-16 12:15:42.000000 rssfixer-0.0.2/src/rssfixer.egg-info/PKG-INFO
--rw-r--r--   0 reuteras   (501) staff       (20)      295 2023-04-16 12:15:42.000000 rssfixer-0.0.2/src/rssfixer.egg-info/SOURCES.txt
--rw-r--r--   0 reuteras   (501) staff       (20)        1 2023-04-16 12:15:42.000000 rssfixer-0.0.2/src/rssfixer.egg-info/dependency_links.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       43 2023-04-16 12:15:42.000000 rssfixer-0.0.2/src/rssfixer.egg-info/entry_points.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       58 2023-04-16 12:15:42.000000 rssfixer-0.0.2/src/rssfixer.egg-info/requires.txt
--rw-r--r--   0 reuteras   (501) staff       (20)        9 2023-04-16 12:15:42.000000 rssfixer-0.0.2/src/rssfixer.egg-info/top_level.txt
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-16 13:37:38.570423 rssfixer-0.0.3/
+-rw-r--r--   0 reuteras   (501) staff       (20)     1058 2023-04-16 10:16:56.000000 rssfixer-0.0.3/LICENSE
+-rw-r--r--   0 reuteras   (501) staff       (20)     1595 2023-04-16 13:37:38.570291 rssfixer-0.0.3/PKG-INFO
+-rw-r--r--   0 reuteras   (501) staff       (20)     1052 2023-04-16 13:36:03.000000 rssfixer-0.0.3/README.md
+-rw-r--r--   0 reuteras   (501) staff       (20)      799 2023-04-16 13:26:05.000000 rssfixer-0.0.3/pyproject.toml
+-rw-r--r--   0 reuteras   (501) staff       (20)       38 2023-04-16 13:37:38.570472 rssfixer-0.0.3/setup.cfg
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-16 13:37:38.568440 rssfixer-0.0.3/src/
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-16 13:37:38.569112 rssfixer-0.0.3/src/rssfixer/
+-rw-r--r--   0 reuteras   (501) staff       (20)       60 2023-04-16 12:15:09.000000 rssfixer-0.0.3/src/rssfixer/__init__.py
+-rw-r--r--   0 reuteras   (501) staff       (20)     2825 2023-04-16 11:26:17.000000 rssfixer-0.0.3/src/rssfixer/rss.py
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-16 13:37:38.570105 rssfixer-0.0.3/src/rssfixer.egg-info/
+-rw-r--r--   0 reuteras   (501) staff       (20)     1595 2023-04-16 13:37:38.000000 rssfixer-0.0.3/src/rssfixer.egg-info/PKG-INFO
+-rw-r--r--   0 reuteras   (501) staff       (20)      295 2023-04-16 13:37:38.000000 rssfixer-0.0.3/src/rssfixer.egg-info/SOURCES.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)        1 2023-04-16 13:37:38.000000 rssfixer-0.0.3/src/rssfixer.egg-info/dependency_links.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)       43 2023-04-16 13:37:38.000000 rssfixer-0.0.3/src/rssfixer.egg-info/entry_points.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)       58 2023-04-16 13:37:38.000000 rssfixer-0.0.3/src/rssfixer.egg-info/requires.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)        9 2023-04-16 13:37:38.000000 rssfixer-0.0.3/src/rssfixer.egg-info/top_level.txt
```

### Comparing `rssfixer-0.0.2/LICENSE` & `rssfixer-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rssfixer-0.0.2/pyproject.toml` & `rssfixer-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "rssfixer"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Peter Reuterås", email="peter@reuteras.net" },
 ]
-description = "A small example package"
+description = "Generate RSS feed for Wordpress blog without it."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `rssfixer-0.0.2/src/rssfixer/rss.py` & `rssfixer-0.0.3/src/rssfixer/rss.py`

 * *Files identical despite different names*

