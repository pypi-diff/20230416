# Comparing `tmp/simple-openai-0.0.1.tar.gz` & `tmp/simple-openai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-openai-0.0.1.tar", last modified: Sun Apr 16 14:35:06 2023, max compression
+gzip compressed data, was "simple-openai-0.0.2.tar", last modified: Sun Apr 16 14:42:40 2023, max compression
```

## Comparing `simple-openai-0.0.1.tar` & `simple-openai-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:35:06.867600 simple-openai-0.0.1/
--rw-r--r--   0 steve      (501) staff       (20)    11357 2023-04-15 11:09:16.000000 simple-openai-0.0.1/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)    13906 2023-04-16 14:35:06.867373 simple-openai-0.0.1/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)        9 2023-04-15 11:09:16.000000 simple-openai-0.0.1/README.md
--rw-r--r--   0 steve      (501) staff       (20)     1179 2023-04-16 14:35:01.000000 simple-openai-0.0.1/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-04-16 14:35:06.867641 simple-openai-0.0.1/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:35:06.864669 simple-openai-0.0.1/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:35:06.865893 simple-openai-0.0.1/src/simple_openai/
--rw-r--r--   0 steve      (501) staff       (20)      223 2023-04-16 13:49:41.000000 simple-openai-0.0.1/src/simple_openai/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     6571 2023-04-16 13:37:12.000000 simple-openai-0.0.1/src/simple_openai/async_simple_openai.py
--rw-r--r--   0 steve      (501) staff       (20)      184 2023-04-16 13:51:48.000000 simple-openai-0.0.1/src/simple_openai/constants.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:35:06.866743 simple-openai-0.0.1/src/simple_openai/models/
--rw-r--r--   0 steve      (501) staff       (20)      883 2023-04-15 16:43:05.000000 simple-openai-0.0.1/src/simple_openai/models/open_ai_models.py
--rw-r--r--   0 steve      (501) staff       (20)      672 2023-04-16 13:21:37.000000 simple-openai-0.0.1/src/simple_openai/responses.py
--rw-r--r--   0 steve      (501) staff       (20)     5924 2023-04-16 13:48:53.000000 simple-openai-0.0.1/src/simple_openai/simple_openai.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:35:06.866593 simple-openai-0.0.1/src/simple_openai.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    13906 2023-04-16 14:35:06.000000 simple-openai-0.0.1/src/simple_openai.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      506 2023-04-16 14:35:06.000000 simple-openai-0.0.1/src/simple_openai.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-04-16 14:35:06.000000 simple-openai-0.0.1/src/simple_openai.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)       89 2023-04-16 14:35:06.000000 simple-openai-0.0.1/src/simple_openai.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)       14 2023-04-16 14:35:06.000000 simple-openai-0.0.1/src/simple_openai.egg-info/top_level.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:35:06.867139 simple-openai-0.0.1/tests/
--rw-r--r--   0 steve      (501) staff       (20)     1579 2023-04-16 13:13:06.000000 simple-openai-0.0.1/tests/test_AsyncSimpleOpenai.py
--rw-r--r--   0 steve      (501) staff       (20)     1461 2023-04-16 13:51:21.000000 simple-openai-0.0.1/tests/test_SimpleOpenai.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:42:40.476346 simple-openai-0.0.2/
+-rw-r--r--   0 steve      (501) staff       (20)    11357 2023-04-15 11:09:16.000000 simple-openai-0.0.2/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)    14318 2023-04-16 14:42:40.475932 simple-openai-0.0.2/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      421 2023-04-16 14:41:39.000000 simple-openai-0.0.2/README.md
+-rw-r--r--   0 steve      (501) staff       (20)     1179 2023-04-16 14:42:15.000000 simple-openai-0.0.2/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-04-16 14:42:40.476414 simple-openai-0.0.2/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:42:40.471809 simple-openai-0.0.2/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:42:40.473628 simple-openai-0.0.2/src/simple_openai/
+-rw-r--r--   0 steve      (501) staff       (20)      223 2023-04-16 13:49:41.000000 simple-openai-0.0.2/src/simple_openai/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     6571 2023-04-16 13:37:12.000000 simple-openai-0.0.2/src/simple_openai/async_simple_openai.py
+-rw-r--r--   0 steve      (501) staff       (20)      184 2023-04-16 13:51:48.000000 simple-openai-0.0.2/src/simple_openai/constants.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:42:40.474717 simple-openai-0.0.2/src/simple_openai/models/
+-rw-r--r--   0 steve      (501) staff       (20)      883 2023-04-15 16:43:05.000000 simple-openai-0.0.2/src/simple_openai/models/open_ai_models.py
+-rw-r--r--   0 steve      (501) staff       (20)      672 2023-04-16 13:21:37.000000 simple-openai-0.0.2/src/simple_openai/responses.py
+-rw-r--r--   0 steve      (501) staff       (20)     5924 2023-04-16 13:48:53.000000 simple-openai-0.0.2/src/simple_openai/simple_openai.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:42:40.474577 simple-openai-0.0.2/src/simple_openai.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    14318 2023-04-16 14:42:40.000000 simple-openai-0.0.2/src/simple_openai.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      506 2023-04-16 14:42:40.000000 simple-openai-0.0.2/src/simple_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-04-16 14:42:40.000000 simple-openai-0.0.2/src/simple_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)       89 2023-04-16 14:42:40.000000 simple-openai-0.0.2/src/simple_openai.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       14 2023-04-16 14:42:40.000000 simple-openai-0.0.2/src/simple_openai.egg-info/top_level.txt
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-04-16 14:42:40.475413 simple-openai-0.0.2/tests/
+-rw-r--r--   0 steve      (501) staff       (20)     1579 2023-04-16 13:13:06.000000 simple-openai-0.0.2/tests/test_AsyncSimpleOpenai.py
+-rw-r--r--   0 steve      (501) staff       (20)     1461 2023-04-16 13:51:21.000000 simple-openai-0.0.2/tests/test_SimpleOpenai.py
```

### Comparing `simple-openai-0.0.1/LICENSE` & `simple-openai-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-openai-0.0.1/PKG-INFO` & `simple-openai-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-openai
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple OpenAI API wrapper
 Author-email: Stephen Schleising <stephen@schleising.net>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -218,8 +218,22 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# open-ai
+# simple-openai
+
+This is a simple wrapper around the OpenAI API.  It's not meant to be a full-featured library, but rather a simple way to get started with the API.
+
+The library provides both synchronous and asynchronous methods for interacting with the API.
+
+## Installation
+
+```bash
+pip install simple-openai
+```
+
+## Documentation
+
+The documentation is available on [GitHub](https://schleising.github.io/simple-openai/)
```

### Comparing `simple-openai-0.0.1/pyproject.toml` & `simple-openai-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simple-openai"
-version = "0.0.1"
+version = "0.0.2"
 description = "Simple OpenAI API wrapper"
 readme = "README.md"
 authors = [{ name = "Stephen Schleising", email = "stephen@schleising.net" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

### Comparing `simple-openai-0.0.1/src/simple_openai/async_simple_openai.py` & `simple-openai-0.0.2/src/simple_openai/async_simple_openai.py`

 * *Files identical despite different names*

### Comparing `simple-openai-0.0.1/src/simple_openai/models/open_ai_models.py` & `simple-openai-0.0.2/src/simple_openai/models/open_ai_models.py`

 * *Files identical despite different names*

### Comparing `simple-openai-0.0.1/src/simple_openai/responses.py` & `simple-openai-0.0.2/src/simple_openai/responses.py`

 * *Files identical despite different names*

### Comparing `simple-openai-0.0.1/src/simple_openai/simple_openai.py` & `simple-openai-0.0.2/src/simple_openai/simple_openai.py`

 * *Files identical despite different names*

### Comparing `simple-openai-0.0.1/src/simple_openai.egg-info/PKG-INFO` & `simple-openai-0.0.2/src/simple_openai.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-openai
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple OpenAI API wrapper
 Author-email: Stephen Schleising <stephen@schleising.net>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -218,8 +218,22 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# open-ai
+# simple-openai
+
+This is a simple wrapper around the OpenAI API.  It's not meant to be a full-featured library, but rather a simple way to get started with the API.
+
+The library provides both synchronous and asynchronous methods for interacting with the API.
+
+## Installation
+
+```bash
+pip install simple-openai
+```
+
+## Documentation
+
+The documentation is available on [GitHub](https://schleising.github.io/simple-openai/)
```

### Comparing `simple-openai-0.0.1/tests/test_AsyncSimpleOpenai.py` & `simple-openai-0.0.2/tests/test_AsyncSimpleOpenai.py`

 * *Files identical despite different names*

### Comparing `simple-openai-0.0.1/tests/test_SimpleOpenai.py` & `simple-openai-0.0.2/tests/test_SimpleOpenai.py`

 * *Files identical despite different names*

