# Comparing `tmp/jeff_api-0.2.9.tar.gz` & `tmp/jeff_api-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeff_api-0.2.9.tar", last modified: Mon Apr  3 05:02:32 2023, max compression
+gzip compressed data, was "jeff_api-1.0.0.tar", last modified: Sun Apr 16 20:06:56 2023, max compression
```

## Comparing `jeff_api-0.2.9.tar` & `jeff_api-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-03 05:02:32.046251 jeff_api-0.2.9/
--rw-------   0 markcda   (1000) markcda   (1000)     1087 2023-01-15 14:50:00.000000 jeff_api-0.2.9/LICENSE
--rw-r--r--   0 markcda   (1000) markcda   (1000)     1134 2023-04-03 05:02:32.044251 jeff_api-0.2.9/PKG-INFO
--rw-r--r--   0 markcda   (1000) markcda   (1000)      623 2023-03-05 09:58:33.000000 jeff_api-0.2.9/README.md
--rw-r--r--   0 markcda   (1000) markcda   (1000)      497 2023-04-03 05:00:35.000000 jeff_api-0.2.9/pyproject.toml
--rw-r--r--   0 markcda   (1000) markcda   (1000)       38 2023-04-03 05:02:32.046251 jeff_api-0.2.9/setup.cfg
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-03 05:02:32.034251 jeff_api-0.2.9/src/
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-03 05:02:32.040251 jeff_api-0.2.9/src/jeff_api/
--rw-r--r--   0 markcda   (1000) markcda   (1000)        0 2023-01-01 20:50:00.000000 jeff_api-0.2.9/src/jeff_api/__init__.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     2116 2023-03-13 03:54:13.000000 jeff_api-0.2.9/src/jeff_api/client.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     3702 2023-04-01 15:33:54.000000 jeff_api-0.2.9/src/jeff_api/scenario.py
--rw-r--r--   0 markcda   (1000) markcda   (1000)     1035 2023-04-03 05:00:35.000000 jeff_api-0.2.9/src/jeff_api/server.py
-drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-03 05:02:32.044251 jeff_api-0.2.9/src/jeff_api.egg-info/
--rw-r--r--   0 markcda   (1000) markcda   (1000)     1134 2023-04-03 05:02:31.000000 jeff_api-0.2.9/src/jeff_api.egg-info/PKG-INFO
--rw-r--r--   0 markcda   (1000) markcda   (1000)      272 2023-04-03 05:02:32.000000 jeff_api-0.2.9/src/jeff_api.egg-info/SOURCES.txt
--rw-r--r--   0 markcda   (1000) markcda   (1000)        1 2023-04-03 05:02:32.000000 jeff_api-0.2.9/src/jeff_api.egg-info/dependency_links.txt
--rw-r--r--   0 markcda   (1000) markcda   (1000)        9 2023-04-03 05:02:32.000000 jeff_api-0.2.9/src/jeff_api.egg-info/top_level.txt
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 20:06:56.031158 jeff_api-1.0.0/
+-rw-------   0 markcda   (1000) markcda   (1000)     1087 2023-01-15 14:50:00.000000 jeff_api-1.0.0/LICENSE
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     1134 2023-04-16 20:06:56.031158 jeff_api-1.0.0/PKG-INFO
+-rw-r--r--   0 markcda   (1000) markcda   (1000)      623 2023-03-05 09:58:33.000000 jeff_api-1.0.0/README.md
+-rw-------   0 markcda   (1000) markcda   (1000)      497 2023-04-16 07:36:22.000000 jeff_api-1.0.0/pyproject.toml
+-rw-r--r--   0 markcda   (1000) markcda   (1000)       38 2023-04-16 20:06:56.031158 jeff_api-1.0.0/setup.cfg
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 20:06:56.017158 jeff_api-1.0.0/src/
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 20:06:56.027158 jeff_api-1.0.0/src/jeff_api/
+-rw-r--r--   0 markcda   (1000) markcda   (1000)        0 2023-01-01 20:50:00.000000 jeff_api-1.0.0/src/jeff_api/__init__.py
+-rw-r--r--   0 markcda   (1000) markcda   (1000)     6901 2023-04-16 07:44:02.000000 jeff_api-1.0.0/src/jeff_api/bridge.py
+drwxr-xr-x   0 markcda   (1000) markcda   (1000)        0 2023-04-16 20:06:56.029158 jeff_api-1.0.0/src/jeff_api.egg-info/
+-rw-------   0 markcda   (1000) markcda   (1000)     1134 2023-04-16 20:06:55.000000 jeff_api-1.0.0/src/jeff_api.egg-info/PKG-INFO
+-rw-------   0 markcda   (1000) markcda   (1000)      224 2023-04-16 20:06:56.000000 jeff_api-1.0.0/src/jeff_api.egg-info/SOURCES.txt
+-rw-------   0 markcda   (1000) markcda   (1000)        1 2023-04-16 20:06:55.000000 jeff_api-1.0.0/src/jeff_api.egg-info/dependency_links.txt
+-rw-------   0 markcda   (1000) markcda   (1000)        9 2023-04-16 20:06:55.000000 jeff_api-1.0.0/src/jeff_api.egg-info/top_level.txt
```

### Comparing `jeff_api-0.2.9/LICENSE` & `jeff_api-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jeff_api-0.2.9/PKG-INFO` & `jeff_api-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeff_api
-Version: 0.2.9
+Version: 1.0.0
 Summary: A Python library for intercommunicating with Jeff.
 Author-email: Mark CDA <aclo.create@gmail.com>
 Project-URL: Homepage, https://github.com/markcda/jeff
 Project-URL: Bug Tracker, https://github.com/markcda/jeff/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jeff_api-0.2.9/README.md` & `jeff_api-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `jeff_api-0.2.9/src/jeff_api.egg-info/PKG-INFO` & `jeff_api-1.0.0/src/jeff_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jeff-api
-Version: 0.2.9
+Version: 1.0.0
 Summary: A Python library for intercommunicating with Jeff.
 Author-email: Mark CDA <aclo.create@gmail.com>
 Project-URL: Homepage, https://github.com/markcda/jeff
 Project-URL: Bug Tracker, https://github.com/markcda/jeff/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

