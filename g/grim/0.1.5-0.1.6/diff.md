# Comparing `tmp/grim-0.1.5.tar.gz` & `tmp/grim-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grim-0.1.5.tar", last modified: Sat Apr  1 14:50:37 2023, max compression
+gzip compressed data, was "grim-0.1.6.tar", last modified: Sun Apr 16 16:53:54 2023, max compression
```

## Comparing `grim-0.1.5.tar` & `grim-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 14:50:37.692766 grim-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-01 14:50:11.000000 grim-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-01 14:50:37.692766 grim-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-04-01 14:50:11.000000 grim-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 14:50:37.688766 grim-0.1.5/grim/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-01 14:50:11.000000 grim-0.1.5/grim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-04-01 14:50:11.000000 grim-0.1.5/grim/mean_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 14:50:37.692766 grim-0.1.5/grim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-04-01 14:50:37.000000 grim-0.1.5/grim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-01 14:50:37.000000 grim-0.1.5/grim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 14:50:37.000000 grim-0.1.5/grim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-01 14:50:37.000000 grim-0.1.5/grim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 14:50:37.692766 grim-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-01 14:50:11.000000 grim-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:53:54.945343 grim-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-16 16:53:33.000000 grim-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-16 16:53:54.941343 grim-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-16 16:53:33.000000 grim-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:53:54.941343 grim-0.1.6/grim/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-16 16:53:33.000000 grim-0.1.6/grim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-04-16 16:53:33.000000 grim-0.1.6/grim/mean_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:53:54.941343 grim-0.1.6/grim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-04-16 16:53:54.000000 grim-0.1.6/grim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-16 16:53:54.000000 grim-0.1.6/grim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:53:54.000000 grim-0.1.6/grim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-16 16:53:54.000000 grim-0.1.6/grim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 16:53:54.945343 grim-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-16 16:53:33.000000 grim-0.1.6/setup.py
```

### Comparing `grim-0.1.5/LICENSE` & `grim-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `grim-0.1.5/PKG-INFO` & `grim-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grim
-Version: 0.1.5
+Version: 0.1.6
 Summary: An implementation of the GRIM test, in Python
 Home-page: https://github.com/phoughton/grim_test
 Author: Peter Houghton
 Author-email: pete@investigatingsoftware.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,15 +36,15 @@
 ### How do I install it?
 
 On the command line:
 ```bash
 pip install grim
 ```
 
-In a google Colab/iPython notebook:
+In a google Colab/iPython/Jupyter notebook:
 ```bash
 !pip install grim
 ```
 
 ### Example: Is this _mean_, _n_ and rounding type consistent?
 ```python
 from grim import mean_tester
```

### Comparing `grim-0.1.5/README.md` & `grim-0.1.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ### How do I install it?
 
 On the command line:
 ```bash
 pip install grim
 ```
 
-In a google Colab/iPython notebook:
+In a google Colab/iPython/Jupyter notebook:
 ```bash
 !pip install grim
 ```
 
 ### Example: Is this _mean_, _n_ and rounding type consistent?
 ```python
 from grim import mean_tester
```

### Comparing `grim-0.1.5/grim.egg-info/PKG-INFO` & `grim-0.1.6/grim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grim
-Version: 0.1.5
+Version: 0.1.6
 Summary: An implementation of the GRIM test, in Python
 Home-page: https://github.com/phoughton/grim_test
 Author: Peter Houghton
 Author-email: pete@investigatingsoftware.co.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,15 +36,15 @@
 ### How do I install it?
 
 On the command line:
 ```bash
 pip install grim
 ```
 
-In a google Colab/iPython notebook:
+In a google Colab/iPython/Jupyter notebook:
 ```bash
 !pip install grim
 ```
 
 ### Example: Is this _mean_, _n_ and rounding type consistent?
 ```python
 from grim import mean_tester
```

### Comparing `grim-0.1.5/setup.py` & `grim-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="grim",
-    version="0.1.5",
+    version="0.1.6",
     author="Peter Houghton",
     author_email="pete@investigatingsoftware.co.uk",
     description="An implementation of the GRIM test, in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/phoughton/grim_test",
     packages=setuptools.find_packages(),
```

