# Comparing `tmp/st_text_annotator-0.1.1.tar.gz` & `tmp/st_text_annotator-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_text_annotator-0.1.1.tar", last modified: Fri Apr 14 22:43:09 2023, max compression
+gzip compressed data, was "st_text_annotator-0.1.6.tar", max compression
```

## Comparing `st_text_annotator-0.1.1.tar` & `st_text_annotator-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,28 @@
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2023-04-14 22:43:09.255078 st_text_annotator-0.1.1/
--rw-r--r--   0 robin      (501) staff       (20)     1075 2023-04-14 18:30:17.000000 st_text_annotator-0.1.1/LICENSE
--rw-r--r--   0 robin      (501) staff       (20)       53 2023-04-14 21:49:12.000000 st_text_annotator-0.1.1/MANIFEST.in
--rw-r--r--   0 robin      (501) staff       (20)     1630 2023-04-14 22:43:09.253256 st_text_annotator-0.1.1/PKG-INFO
--rw-r--r--   0 robin      (501) staff       (20)      971 2023-04-14 22:26:10.000000 st_text_annotator-0.1.1/README.md
--rw-r--r--   0 robin      (501) staff       (20)      646 2023-04-14 22:40:24.000000 st_text_annotator-0.1.1/pyproject.toml
--rw-r--r--   0 robin      (501) staff       (20)       38 2023-04-14 22:43:09.255560 st_text_annotator-0.1.1/setup.cfg
--rw-r--r--   0 robin      (501) staff       (20)      851 2023-04-14 22:42:20.000000 st_text_annotator-0.1.1/setup.py
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2023-04-14 22:43:09.245087 st_text_annotator-0.1.1/src/
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2023-04-14 22:43:09.248497 st_text_annotator-0.1.1/src/st_text_annotator/
--rw-r--r--   0 robin      (501) staff       (20)     5238 2023-04-14 22:21:01.000000 st_text_annotator-0.1.1/src/st_text_annotator/__init__.py
-drwxr-xr-x   0 robin      (501) staff       (20)        0 2023-04-14 22:43:09.252436 st_text_annotator-0.1.1/src/st_text_annotator.egg-info/
--rw-r--r--   0 robin      (501) staff       (20)     1630 2023-04-14 22:43:09.000000 st_text_annotator-0.1.1/src/st_text_annotator.egg-info/PKG-INFO
--rw-r--r--   0 robin      (501) staff       (20)      311 2023-04-14 22:43:09.000000 st_text_annotator-0.1.1/src/st_text_annotator.egg-info/SOURCES.txt
--rw-r--r--   0 robin      (501) staff       (20)        1 2023-04-14 22:43:09.000000 st_text_annotator-0.1.1/src/st_text_annotator.egg-info/dependency_links.txt
--rw-r--r--   0 robin      (501) staff       (20)       17 2023-04-14 22:43:09.000000 st_text_annotator-0.1.1/src/st_text_annotator.egg-info/requires.txt
--rw-r--r--   0 robin      (501) staff       (20)       18 2023-04-14 22:43:09.000000 st_text_annotator-0.1.1/src/st_text_annotator.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1075 2023-04-14 18:30:17.965925 st_text_annotator-0.1.6/LICENSE
+-rw-r--r--   0        0        0      971 2023-04-14 22:26:10.101353 st_text_annotator-0.1.6/README.md
+-rw-r--r--   0        0        0      702 2023-04-16 14:19:25.824988 st_text_annotator-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2309 2023-04-15 21:13:21.432502 st_text_annotator-0.1.6/src/st_text_annotator/__init__.py
+-rw-r--r--   0        0        0      180 2023-04-14 17:24:02.791373 st_text_annotator-0.1.6/src/st_text_annotator/frontend/.env
+-rw-r--r--   0        0        0       67 2023-04-14 17:24:02.792164 st_text_annotator-0.1.6/src/st_text_annotator/frontend/.prettierrc
+-rw-r--r--   0        0        0      961 2023-04-14 22:08:31.587769 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0   197459 2023-04-14 22:08:17.378178 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/bootstrap.min.css
+-rw-r--r--   0        0        0     2097 2023-04-14 22:08:31.587571 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/index.html
+-rw-r--r--   0        0        0      685 2023-04-14 22:08:31.587640 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/precache-manifest.e1f4d7e39016325d19b80487326d9754.js
+-rw-r--r--   0        0        0     1183 2023-04-14 22:08:31.587724 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/service-worker.js
+-rw-r--r--   0        0        0   594301 2023-04-14 22:08:31.594107 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js
+-rw-r--r--   0        0        0     1803 2023-04-14 22:08:31.593423 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0  1813945 2023-04-14 22:08:31.593928 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/2.0d16c425.chunk.js.map
+-rw-r--r--   0        0        0    11817 2023-04-14 22:08:31.593385 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/main.c60fd880.chunk.js
+-rw-r--r--   0        0        0      149 2023-04-14 22:08:31.594561 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/main.c60fd880.chunk.js.LICENSE.txt
+-rw-r--r--   0        0        0    22907 2023-04-14 22:08:31.593496 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/main.c60fd880.chunk.js.map
+-rw-r--r--   0        0        0     1594 2023-04-14 22:08:31.593462 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/runtime-main.d5954658.js
+-rw-r--r--   0        0        0     8307 2023-04-14 22:08:31.594489 st_text_annotator-0.1.6/src/st_text_annotator/frontend/build/static/js/runtime-main.d5954658.js.map
+-rw-r--r--   0        0        0      846 2023-04-14 21:50:22.684911 st_text_annotator-0.1.6/src/st_text_annotator/frontend/package.json
+-rw-r--r--   0        0        0   197459 2023-04-14 17:24:02.785648 st_text_annotator-0.1.6/src/st_text_annotator/frontend/public/bootstrap.min.css
+-rw-r--r--   0        0        0      894 2023-04-14 17:24:02.786098 st_text_annotator-0.1.6/src/st_text_annotator/frontend/public/index.html
+-rw-r--r--   0        0        0     7490 2023-04-14 21:49:47.302144 st_text_annotator-0.1.6/src/st_text_annotator/frontend/src/Annotation.tsx
+-rw-r--r--   0        0        0     7490 2023-04-15 21:14:06.072822 st_text_annotator-0.1.6/src/st_text_annotator/frontend/src/AnnotationNew.tsx
+-rw-r--r--   0        0        0      219 2023-04-15 21:23:26.959735 st_text_annotator-0.1.6/src/st_text_annotator/frontend/src/index.tsx
+-rw-r--r--   0        0        0       40 2023-04-14 17:24:02.814143 st_text_annotator-0.1.6/src/st_text_annotator/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      459 2023-04-14 17:24:02.792820 st_text_annotator-0.1.6/src/st_text_annotator/frontend/tsconfig.json
+-rw-r--r--   0        0        0     1521 1970-01-01 00:00:00.000000 st_text_annotator-0.1.6/PKG-INFO
```

### Comparing `st_text_annotator-0.1.1/LICENSE` & `st_text_annotator-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `st_text_annotator-0.1.1/PKG-INFO` & `st_text_annotator-0.1.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
-Name: st_text_annotator
-Version: 0.1.1
+Name: st-text-annotator
+Version: 0.1.6
 Summary: Component for annotating text for NLP resolution
-Home-page: https://github.com/rmarquet21/steamlit-text-annotator
+License: MIT
 Author: Robin Marquet
-Author-email: Robin Marquet <robin.marquet3@gmail.com>
-Project-URL: Homepage, https://github.com/rmarquet21/streamlit-text-annotator
-Project-URL: Bug Tracker, https://github.com/rmarquet21/streamlit-text-annotator/issues
-Classifier: Programming Language :: Python :: 3
+Author-email: robin.marquet@epitech.eu
+Requires-Python: >=3.8,<3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: streamlit (>=1.21.0,<2.0.0)
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 <h1> streamlit-annotation </h1>
 
 - [Install](#install)
 - [Quick Use](#quick-use)
 - [Development](#development)
   - [Install](#install-1)
@@ -74,7 +74,8 @@
 
 Robin Marquet
 
 # Contributors
 
 - [Robin Marquet](robin.marquet3@gmail.com)
 
+
```

### Comparing `st_text_annotator-0.1.1/README.md` & `st_text_annotator-0.1.6/README.md`

 * *Files identical despite different names*

