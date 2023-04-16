# Comparing `tmp/export_ease-0.0.1.tar.gz` & `tmp/export_ease-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "export_ease-0.0.1.tar", last modified: Sun Mar 12 04:11:30 2023, max compression
+gzip compressed data, was "export_ease-0.0.2.tar", last modified: Sun Apr 16 21:55:50 2023, max compression
```

## Comparing `export_ease-0.0.1.tar` & `export_ease-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-03-12 04:11:30.380797 export_ease-0.0.1/
--rw-r--r--   0 pauldilly   (501) staff       (20)     1067 2023-03-12 04:10:17.000000 export_ease-0.0.1/LICENSE
--rw-r--r--   0 pauldilly   (501) staff       (20)     4858 2023-03-12 04:11:30.380625 export_ease-0.0.1/PKG-INFO
--rw-r--r--   0 pauldilly   (501) staff       (20)     4332 2023-03-12 04:10:17.000000 export_ease-0.0.1/README.md
--rw-r--r--   0 pauldilly   (501) staff       (20)      608 2023-03-12 04:10:17.000000 export_ease-0.0.1/pyproject.toml
--rw-r--r--   0 pauldilly   (501) staff       (20)       38 2023-03-12 04:11:30.380844 export_ease-0.0.1/setup.cfg
-drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-03-12 04:11:30.378779 export_ease-0.0.1/src/
-drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-03-12 04:11:30.379604 export_ease-0.0.1/src/export_ease/
--rw-r--r--   0 pauldilly   (501) staff       (20)        1 2023-03-12 04:10:17.000000 export_ease-0.0.1/src/export_ease/__init__.py
--rw-r--r--   0 pauldilly   (501) staff       (20)     4480 2023-03-12 04:10:17.000000 export_ease-0.0.1/src/export_ease/comtrade.py
--rw-r--r--   0 pauldilly   (501) staff       (20)     6058 2023-03-12 04:10:17.000000 export_ease-0.0.1/src/export_ease/imf.py
-drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-03-12 04:11:30.380337 export_ease-0.0.1/src/export_ease.egg-info/
--rw-r--r--   0 pauldilly   (501) staff       (20)     4858 2023-03-12 04:11:30.000000 export_ease-0.0.1/src/export_ease.egg-info/PKG-INFO
--rw-r--r--   0 pauldilly   (501) staff       (20)      267 2023-03-12 04:11:30.000000 export_ease-0.0.1/src/export_ease.egg-info/SOURCES.txt
--rw-r--r--   0 pauldilly   (501) staff       (20)        1 2023-03-12 04:11:30.000000 export_ease-0.0.1/src/export_ease.egg-info/dependency_links.txt
--rw-r--r--   0 pauldilly   (501) staff       (20)       12 2023-03-12 04:11:30.000000 export_ease-0.0.1/src/export_ease.egg-info/top_level.txt
+drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 21:55:50.875713 export_ease-0.0.2/
+-rw-r--r--   0 pauldilly   (501) staff       (20)     1067 2023-04-16 21:36:49.000000 export_ease-0.0.2/LICENSE
+-rw-r--r--   0 pauldilly   (501) staff       (20)     4858 2023-04-16 21:55:50.875571 export_ease-0.0.2/PKG-INFO
+-rw-r--r--   0 pauldilly   (501) staff       (20)     4332 2023-04-16 21:36:49.000000 export_ease-0.0.2/README.md
+-rw-r--r--   0 pauldilly   (501) staff       (20)      608 2023-04-16 21:49:41.000000 export_ease-0.0.2/pyproject.toml
+-rw-r--r--   0 pauldilly   (501) staff       (20)       38 2023-04-16 21:55:50.875767 export_ease-0.0.2/setup.cfg
+drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 21:55:50.874031 export_ease-0.0.2/src/
+drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 21:55:50.874843 export_ease-0.0.2/src/export_ease/
+-rw-r--r--   0 pauldilly   (501) staff       (20)        1 2023-04-16 21:36:49.000000 export_ease-0.0.2/src/export_ease/__init__.py
+-rw-r--r--   0 pauldilly   (501) staff       (20)     2733 2023-04-16 21:43:25.000000 export_ease-0.0.2/src/export_ease/comtrade.py
+-rw-r--r--   0 pauldilly   (501) staff       (20)     3755 2023-04-16 21:48:39.000000 export_ease-0.0.2/src/export_ease/imf.py
+drwxr-xr-x   0 pauldilly   (501) staff       (20)        0 2023-04-16 21:55:50.875366 export_ease-0.0.2/src/export_ease.egg-info/
+-rw-r--r--   0 pauldilly   (501) staff       (20)     4858 2023-04-16 21:55:50.000000 export_ease-0.0.2/src/export_ease.egg-info/PKG-INFO
+-rw-r--r--   0 pauldilly   (501) staff       (20)      267 2023-04-16 21:55:50.000000 export_ease-0.0.2/src/export_ease.egg-info/SOURCES.txt
+-rw-r--r--   0 pauldilly   (501) staff       (20)        1 2023-04-16 21:55:50.000000 export_ease-0.0.2/src/export_ease.egg-info/dependency_links.txt
+-rw-r--r--   0 pauldilly   (501) staff       (20)       12 2023-04-16 21:55:50.000000 export_ease-0.0.2/src/export_ease.egg-info/top_level.txt
```

### Comparing `export_ease-0.0.1/LICENSE` & `export_ease-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `export_ease-0.0.1/PKG-INFO` & `export_ease-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: export_ease
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package that facilitates API calls to UN Comtrade and the International Monetary Fund to gather macroeconomic export data
 Author-email: Paul Dilly <paul.dilly@duke.edu>
 Project-URL: Homepage, https://github.com/pcd15/export_pkg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `export_ease-0.0.1/README.md` & `export_ease-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `export_ease-0.0.1/pyproject.toml` & `export_ease-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "export_ease"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Paul Dilly", email="paul.dilly@duke.edu" },
 ]
 description = "A package that facilitates API calls to UN Comtrade and the International Monetary Fund to gather macroeconomic export data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `export_ease-0.0.1/src/export_ease.egg-info/PKG-INFO` & `export_ease-0.0.2/src/export_ease.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: export-ease
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package that facilitates API calls to UN Comtrade and the International Monetary Fund to gather macroeconomic export data
 Author-email: Paul Dilly <paul.dilly@duke.edu>
 Project-URL: Homepage, https://github.com/pcd15/export_pkg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

