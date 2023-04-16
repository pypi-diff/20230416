# Comparing `tmp/blag-1.4.1.tar.gz` & `tmp/blag-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blag-1.4.1.tar", last modified: Thu Sep 29 18:50:25 2022, max compression
+gzip compressed data, was "blag-1.5.0.tar", last modified: Sun Apr 16 09:01:18 2023, max compression
```

## Comparing `blag-1.4.1.tar` & `blag-1.5.0.tar`

### file list

```diff
@@ -1,27 +1,34 @@
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2022-09-29 18:50:25.087885 blag-1.4.1/
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1072 2021-02-01 20:16:23.000000 blag-1.4.1/LICENSE
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1916 2022-09-29 18:50:25.087885 blag-1.4.1/PKG-INFO
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1383 2022-07-01 08:26:42.000000 blag-1.4.1/README.md
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2022-09-29 18:50:25.087885 blag-1.4.1/blag/
--rw-r--r--   0 venthur   (1000) venthur   (1000)       60 2022-09-01 16:56:08.000000 blag-1.4.1/blag/__init__.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)    12876 2022-09-04 10:57:00.000000 blag-1.4.1/blag/blag.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     2624 2022-09-01 16:56:08.000000 blag-1.4.1/blag/devserver.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     3577 2022-09-01 16:56:08.000000 blag-1.4.1/blag/markdown.py
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1636 2022-09-01 16:56:08.000000 blag-1.4.1/blag/quickstart.py
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2022-09-29 18:50:25.087885 blag-1.4.1/blag/templates/
--rw-r--r--   0 venthur   (1000) venthur   (1000)      373 2022-08-06 19:36:01.000000 blag-1.4.1/blag/templates/archive.html
--rw-r--r--   0 venthur   (1000) venthur   (1000)      559 2022-08-06 19:36:01.000000 blag-1.4.1/blag/templates/article.html
--rw-r--r--   0 venthur   (1000) venthur   (1000)      867 2022-08-06 19:36:01.000000 blag-1.4.1/blag/templates/base.html
--rw-r--r--   0 venthur   (1000) venthur   (1000)      120 2021-02-06 13:22:35.000000 blag-1.4.1/blag/templates/page.html
--rw-r--r--   0 venthur   (1000) venthur   (1000)      371 2022-08-06 19:36:01.000000 blag-1.4.1/blag/templates/tag.html
--rw-r--r--   0 venthur   (1000) venthur   (1000)      245 2021-02-09 20:55:37.000000 blag-1.4.1/blag/templates/tags.html
--rw-r--r--   0 venthur   (1000) venthur   (1000)       22 2022-09-29 18:43:55.000000 blag-1.4.1/blag/version.py
-drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2022-09-29 18:50:25.087885 blag-1.4.1/blag.egg-info/
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1916 2022-09-29 18:50:25.000000 blag-1.4.1/blag.egg-info/PKG-INFO
--rw-r--r--   0 venthur   (1000) venthur   (1000)      461 2022-09-29 18:50:25.000000 blag-1.4.1/blag.egg-info/SOURCES.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)        1 2022-09-29 18:50:25.000000 blag-1.4.1/blag.egg-info/dependency_links.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)       40 2022-09-29 18:50:25.000000 blag-1.4.1/blag.egg-info/entry_points.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)       39 2022-09-29 18:50:25.000000 blag-1.4.1/blag.egg-info/requires.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)        5 2022-09-29 18:50:25.000000 blag-1.4.1/blag.egg-info/top_level.txt
--rw-r--r--   0 venthur   (1000) venthur   (1000)      279 2022-09-29 18:50:25.091885 blag-1.4.1/setup.cfg
--rw-r--r--   0 venthur   (1000) venthur   (1000)     1116 2022-08-06 19:20:59.000000 blag-1.4.1/setup.py
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-04-16 09:01:18.473932 blag-1.5.0/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1072 2021-02-01 20:16:23.000000 blag-1.5.0/LICENSE
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     3124 2023-04-16 09:01:18.473932 blag-1.5.0/PKG-INFO
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1383 2022-07-01 08:26:42.000000 blag-1.5.0/README.md
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-04-16 09:01:18.473932 blag-1.5.0/blag/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       60 2022-09-01 16:56:08.000000 blag-1.5.0/blag/__init__.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)    12876 2022-09-04 10:57:00.000000 blag-1.5.0/blag/blag.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     2624 2022-09-01 16:56:08.000000 blag-1.5.0/blag/devserver.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     3577 2022-09-01 16:56:08.000000 blag-1.5.0/blag/markdown.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1636 2022-09-01 16:56:08.000000 blag-1.5.0/blag/quickstart.py
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-04-16 09:01:18.473932 blag-1.5.0/blag/templates/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      373 2022-08-06 19:36:01.000000 blag-1.5.0/blag/templates/archive.html
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      559 2022-08-06 19:36:01.000000 blag-1.5.0/blag/templates/article.html
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      867 2022-08-06 19:36:01.000000 blag-1.5.0/blag/templates/base.html
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      120 2021-02-06 13:22:35.000000 blag-1.5.0/blag/templates/page.html
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      371 2022-08-06 19:36:01.000000 blag-1.5.0/blag/templates/tag.html
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      245 2021-02-09 20:55:37.000000 blag-1.5.0/blag/templates/tags.html
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       22 2023-04-16 08:58:00.000000 blag-1.5.0/blag/version.py
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-04-16 09:01:18.473932 blag-1.5.0/blag.egg-info/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     3124 2023-04-16 09:01:18.000000 blag-1.5.0/blag.egg-info/PKG-INFO
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      594 2023-04-16 09:01:18.000000 blag-1.5.0/blag.egg-info/SOURCES.txt
+-rw-r--r--   0 venthur   (1000) venthur   (1000)        1 2023-04-16 09:01:18.000000 blag-1.5.0/blag.egg-info/dependency_links.txt
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       40 2023-04-16 09:01:18.000000 blag-1.5.0/blag.egg-info/entry_points.txt
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      116 2023-04-16 09:01:18.000000 blag-1.5.0/blag.egg-info/requires.txt
+-rw-r--r--   0 venthur   (1000) venthur   (1000)        5 2023-04-16 09:01:18.000000 blag-1.5.0/blag.egg-info/top_level.txt
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1351 2023-04-16 08:58:00.000000 blag-1.5.0/pyproject.toml
+-rw-r--r--   0 venthur   (1000) venthur   (1000)       38 2023-04-16 09:01:18.473932 blag-1.5.0/setup.cfg
+drwxr-xr-x   0 venthur   (1000) venthur   (1000)        0 2023-04-16 09:01:18.473932 blag-1.5.0/tests/
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     8868 2022-09-01 16:56:08.000000 blag-1.5.0/tests/test_blag.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1833 2022-09-01 16:56:08.000000 blag-1.5.0/tests/test_devserver.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     2994 2022-09-01 16:56:08.000000 blag-1.5.0/tests/test_markdown.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      891 2022-09-01 16:56:08.000000 blag-1.5.0/tests/test_quickstart.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)     1967 2022-09-01 16:56:08.000000 blag-1.5.0/tests/test_templates.py
+-rw-r--r--   0 venthur   (1000) venthur   (1000)      167 2022-09-01 16:56:08.000000 blag-1.5.0/tests/test_version.py
```

### Comparing `blag-1.4.1/LICENSE` & `blag-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blag-1.4.1/PKG-INFO` & `blag-1.5.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: blag
-Version: 1.4.1
-Summary: blog-aware, static site generator
-Home-page: https://github.com/venthur/blag
-Author: Bastian Venthur
-Author-email: mail@venthur.de
-License: MIT
-Project-URL: Documentation, https://blag.readthedocs.io/
-Project-URL: Source, https://github.com/venthur/blag
-Project-URL: Changelog, https://github.com/venthur/blag/blob/master/CHANGELOG.md
-Keywords: markdown blag blog static site generator cli
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # blag
 
 blag is a blog-aware, static site generator, written in [Python][].
 
 * an example "deployment" can be found [here][venthur.de]
 * online [documentation][] is available on https://readthedocs.org.
```

### Comparing `blag-1.4.1/blag/blag.py` & `blag-1.5.0/blag/blag.py`

 * *Files identical despite different names*

### Comparing `blag-1.4.1/blag/devserver.py` & `blag-1.5.0/blag/devserver.py`

 * *Files identical despite different names*

### Comparing `blag-1.4.1/blag/markdown.py` & `blag-1.5.0/blag/markdown.py`

 * *Files identical despite different names*

### Comparing `blag-1.4.1/blag/quickstart.py` & `blag-1.5.0/blag/quickstart.py`

 * *Files identical despite different names*

### Comparing `blag-1.4.1/blag/templates/article.html` & `blag-1.5.0/blag/templates/article.html`

 * *Files identical despite different names*

### Comparing `blag-1.4.1/blag/templates/base.html` & `blag-1.5.0/blag/templates/base.html`

 * *Files identical despite different names*

