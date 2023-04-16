# Comparing `tmp/kosis-0.1.4.tar.gz` & `tmp/kosis-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kosis-0.1.4.tar", last modified: Sun Apr 16 03:23:20 2023, max compression
+gzip compressed data, was "kosis-0.1.5.tar", last modified: Sun Apr 16 03:36:40 2023, max compression
```

## Comparing `kosis-0.1.4.tar` & `kosis-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 euntaik   (1000) euntaik   (1000)        0 2023-04-16 03:23:20.381985 kosis-0.1.4/
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)     1080 2023-04-15 17:00:21.000000 kosis-0.1.4/LICENSE
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)     3692 2023-04-16 03:23:20.381985 kosis-0.1.4/PKG-INFO
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)     3224 2023-04-16 03:09:30.000000 kosis-0.1.4/README.md
-drwxr-xr-x   0 euntaik   (1000) euntaik   (1000)        0 2023-04-16 03:23:20.381985 kosis-0.1.4/kosis/
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)       24 2023-04-15 18:51:15.000000 kosis-0.1.4/kosis/__init__.py
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)     6630 2023-04-16 03:03:47.000000 kosis-0.1.4/kosis/kosis.py
-drwxr-xr-x   0 euntaik   (1000) euntaik   (1000)        0 2023-04-16 03:23:20.381985 kosis-0.1.4/kosis.egg-info/
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)     3692 2023-04-16 03:23:20.000000 kosis-0.1.4/kosis.egg-info/PKG-INFO
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)      229 2023-04-16 03:23:20.000000 kosis-0.1.4/kosis.egg-info/SOURCES.txt
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)        1 2023-04-16 03:23:20.000000 kosis-0.1.4/kosis.egg-info/dependency_links.txt
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)       14 2023-04-16 03:23:20.000000 kosis-0.1.4/kosis.egg-info/requires.txt
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)        6 2023-04-16 03:23:20.000000 kosis-0.1.4/kosis.egg-info/top_level.txt
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)      585 2023-04-16 03:15:41.000000 kosis-0.1.4/pyproject.toml
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)       38 2023-04-16 03:23:20.381985 kosis-0.1.4/setup.cfg
-drwxr-xr-x   0 euntaik   (1000) euntaik   (1000)        0 2023-04-16 03:23:20.381985 kosis-0.1.4/tests/
--rw-r--r--   0 euntaik   (1000) euntaik   (1000)      878 2023-04-16 03:20:35.000000 kosis-0.1.4/tests/test_kosis.py
+drwxr-xr-x   0 euntaik   (1000) euntaik   (1000)        0 2023-04-16 03:36:40.671987 kosis-0.1.5/
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)     1080 2023-04-15 17:00:21.000000 kosis-0.1.5/LICENSE
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)     3692 2023-04-16 03:36:40.671987 kosis-0.1.5/PKG-INFO
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)     3224 2023-04-16 03:09:30.000000 kosis-0.1.5/README.md
+drwxr-xr-x   0 euntaik   (1000) euntaik   (1000)        0 2023-04-16 03:36:40.661987 kosis-0.1.5/kosis/
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)       24 2023-04-15 18:51:15.000000 kosis-0.1.5/kosis/__init__.py
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)     6630 2023-04-16 03:03:47.000000 kosis-0.1.5/kosis/kosis.py
+drwxr-xr-x   0 euntaik   (1000) euntaik   (1000)        0 2023-04-16 03:36:40.671987 kosis-0.1.5/kosis.egg-info/
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)     3692 2023-04-16 03:36:40.000000 kosis-0.1.5/kosis.egg-info/PKG-INFO
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)      229 2023-04-16 03:36:40.000000 kosis-0.1.5/kosis.egg-info/SOURCES.txt
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)        1 2023-04-16 03:36:40.000000 kosis-0.1.5/kosis.egg-info/dependency_links.txt
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)       23 2023-04-16 03:36:40.000000 kosis-0.1.5/kosis.egg-info/requires.txt
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)        6 2023-04-16 03:36:40.000000 kosis-0.1.5/kosis.egg-info/top_level.txt
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)      599 2023-04-16 03:30:06.000000 kosis-0.1.5/pyproject.toml
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)       38 2023-04-16 03:36:40.671987 kosis-0.1.5/setup.cfg
+drwxr-xr-x   0 euntaik   (1000) euntaik   (1000)        0 2023-04-16 03:36:40.671987 kosis-0.1.5/tests/
+-rw-r--r--   0 euntaik   (1000) euntaik   (1000)      878 2023-04-16 03:20:35.000000 kosis-0.1.5/tests/test_kosis.py
```

### Comparing `kosis-0.1.4/LICENSE` & `kosis-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kosis-0.1.4/PKG-INFO` & `kosis-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kosis
-Version: 0.1.4
+Version: 0.1.5
 Summary: KOSIS API
 Author-email: Euntaik Lee <euntaik@gmail.com>
 Project-URL: Homepage, https://github.com/euntaik/kosis
 Project-URL: Bug Tracker, https://github.com/euntaik/kosis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kosis-0.1.4/README.md` & `kosis-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `kosis-0.1.4/kosis/kosis.py` & `kosis-0.1.5/kosis/kosis.py`

 * *Files identical despite different names*

### Comparing `kosis-0.1.4/kosis.egg-info/PKG-INFO` & `kosis-0.1.5/kosis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kosis
-Version: 0.1.4
+Version: 0.1.5
 Summary: KOSIS API
 Author-email: Euntaik Lee <euntaik@gmail.com>
 Project-URL: Homepage, https://github.com/euntaik/kosis
 Project-URL: Bug Tracker, https://github.com/euntaik/kosis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kosis-0.1.4/pyproject.toml` & `kosis-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kosis"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Euntaik Lee", email="euntaik@gmail.com" },
 ]
 description = "KOSIS API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "pandas",
   "plotly",
+  "requests",
 ]
 
 
 [project.urls]
 "Homepage" = "https://github.com/euntaik/kosis"
 "Bug Tracker" = "https://github.com/euntaik/kosis/issues"
```

### Comparing `kosis-0.1.4/tests/test_kosis.py` & `kosis-0.1.5/tests/test_kosis.py`

 * *Files identical despite different names*

