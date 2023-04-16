# Comparing `tmp/ml_infrastructure-1.4.3.tar.gz` & `tmp/ml_infrastructure-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_infrastructure-1.4.3.tar", last modified: Sun Apr 16 14:43:18 2023, max compression
+gzip compressed data, was "ml_infrastructure-1.5.1.tar", last modified: Sun Apr 16 14:46:08 2023, max compression
```

## Comparing `ml_infrastructure-1.4.3.tar` & `ml_infrastructure-1.5.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-04-16 14:43:18.622128 ml_infrastructure-1.4.3/
--rw-rw-r--   0 maple     (1000) maple     (1000)     1067 2023-04-16 13:21:50.000000 ml_infrastructure-1.4.3/LICENSE.rst
--rw-rw-r--   0 maple     (1000) maple     (1000)      581 2023-04-16 14:43:18.622128 ml_infrastructure-1.4.3/PKG-INFO
--rw-rw-r--   0 maple     (1000) maple     (1000)        0 2023-02-25 18:05:38.000000 ml_infrastructure-1.4.3/README.rst
-drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-04-16 14:43:18.622128 ml_infrastructure-1.4.3/ml_infrastructure/
--rw-rw-r--   0 maple     (1000) maple     (1000)      168 2023-02-25 17:41:53.000000 ml_infrastructure-1.4.3/ml_infrastructure/__init__.py
--rw-rw-r--   0 maple     (1000) maple     (1000)     9224 2023-04-15 23:10:23.000000 ml_infrastructure-1.4.3/ml_infrastructure/app.py
--rw-rw-r--   0 maple     (1000) maple     (1000)      180 2022-11-28 03:17:28.000000 ml_infrastructure-1.4.3/ml_infrastructure/data_manager.py
--rw-rw-r--   0 maple     (1000) maple     (1000)     4402 2023-04-16 13:23:13.000000 ml_infrastructure-1.4.3/ml_infrastructure/evaluator.py
--rw-rw-r--   0 maple     (1000) maple     (1000)     3532 2022-11-28 03:17:28.000000 ml_infrastructure-1.4.3/ml_infrastructure/example.py
--rw-rw-r--   0 maple     (1000) maple     (1000)     3924 2023-04-16 14:21:11.000000 ml_infrastructure-1.4.3/ml_infrastructure/manager.py
--rw-rw-r--   0 maple     (1000) maple     (1000)     3300 2023-04-16 13:27:14.000000 ml_infrastructure-1.4.3/ml_infrastructure/model.py
-drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-04-16 14:43:18.622128 ml_infrastructure-1.4.3/ml_infrastructure/templates/
--rw-rw-r--   0 maple     (1000) maple     (1000)      508 2022-11-28 03:17:28.000000 ml_infrastructure-1.4.3/ml_infrastructure/templates/control.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      316 2023-04-15 15:08:42.000000 ml_infrastructure-1.4.3/ml_infrastructure/templates/eval.html
--rw-rw-r--   0 maple     (1000) maple     (1000)     1530 2023-04-16 14:31:42.000000 ml_infrastructure-1.4.3/ml_infrastructure/templates/header.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      138 2023-04-15 15:08:42.000000 ml_infrastructure-1.4.3/ml_infrastructure/templates/index.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      309 2023-04-15 15:08:42.000000 ml_infrastructure-1.4.3/ml_infrastructure/templates/loss.html
--rw-rw-r--   0 maple     (1000) maple     (1000)     1706 2023-04-16 14:31:42.000000 ml_infrastructure-1.4.3/ml_infrastructure/templates/stopForm.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      181 2022-11-28 03:17:28.000000 ml_infrastructure-1.4.3/ml_infrastructure/templates/trainingEval.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      452 2023-02-25 17:15:04.000000 ml_infrastructure-1.4.3/ml_infrastructure/templates/trainingLoss.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      189 2022-11-28 03:17:28.000000 ml_infrastructure-1.4.3/ml_infrastructure/templates/validationEval.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      446 2023-02-25 16:35:50.000000 ml_infrastructure-1.4.3/ml_infrastructure/templates/validationLoss.html
--rw-rw-r--   0 maple     (1000) maple     (1000)     1899 2022-12-13 04:56:19.000000 ml_infrastructure-1.4.3/ml_infrastructure/trainer.py
-drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-04-16 14:43:18.622128 ml_infrastructure-1.4.3/ml_infrastructure.egg-info/
--rw-rw-r--   0 maple     (1000) maple     (1000)      581 2023-04-16 14:43:18.000000 ml_infrastructure-1.4.3/ml_infrastructure.egg-info/PKG-INFO
--rw-rw-r--   0 maple     (1000) maple     (1000)      905 2023-04-16 14:43:18.000000 ml_infrastructure-1.4.3/ml_infrastructure.egg-info/SOURCES.txt
--rw-rw-r--   0 maple     (1000) maple     (1000)        1 2023-04-16 14:43:18.000000 ml_infrastructure-1.4.3/ml_infrastructure.egg-info/dependency_links.txt
--rw-rw-r--   0 maple     (1000) maple     (1000)       46 2023-04-16 14:43:18.000000 ml_infrastructure-1.4.3/ml_infrastructure.egg-info/requires.txt
--rw-rw-r--   0 maple     (1000) maple     (1000)       18 2023-04-16 14:43:18.000000 ml_infrastructure-1.4.3/ml_infrastructure.egg-info/top_level.txt
--rw-rw-r--   0 maple     (1000) maple     (1000)      107 2023-04-16 14:43:18.626129 ml_infrastructure-1.4.3/setup.cfg
--rw-rw-r--   0 maple     (1000) maple     (1000)      987 2023-04-15 23:10:44.000000 ml_infrastructure-1.4.3/setup.py
+drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-04-16 14:46:08.319739 ml_infrastructure-1.5.1/
+-rw-rw-r--   0 maple     (1000) maple     (1000)     1067 2023-04-16 13:21:50.000000 ml_infrastructure-1.5.1/LICENSE.rst
+-rw-rw-r--   0 maple     (1000) maple     (1000)      581 2023-04-16 14:46:08.319739 ml_infrastructure-1.5.1/PKG-INFO
+-rw-rw-r--   0 maple     (1000) maple     (1000)        0 2023-02-25 18:05:38.000000 ml_infrastructure-1.5.1/README.rst
+drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-04-16 14:46:08.315739 ml_infrastructure-1.5.1/ml_infrastructure/
+-rw-rw-r--   0 maple     (1000) maple     (1000)      168 2023-02-25 17:41:53.000000 ml_infrastructure-1.5.1/ml_infrastructure/__init__.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)     9224 2023-04-15 23:10:23.000000 ml_infrastructure-1.5.1/ml_infrastructure/app.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)      180 2022-11-28 03:17:28.000000 ml_infrastructure-1.5.1/ml_infrastructure/data_manager.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)     4402 2023-04-16 13:23:13.000000 ml_infrastructure-1.5.1/ml_infrastructure/evaluator.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)     3532 2022-11-28 03:17:28.000000 ml_infrastructure-1.5.1/ml_infrastructure/example.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)     3924 2023-04-16 14:21:11.000000 ml_infrastructure-1.5.1/ml_infrastructure/manager.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)     3300 2023-04-16 13:27:14.000000 ml_infrastructure-1.5.1/ml_infrastructure/model.py
+drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-04-16 14:46:08.319739 ml_infrastructure-1.5.1/ml_infrastructure/templates/
+-rw-rw-r--   0 maple     (1000) maple     (1000)      508 2022-11-28 03:17:28.000000 ml_infrastructure-1.5.1/ml_infrastructure/templates/control.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      316 2023-04-15 15:08:42.000000 ml_infrastructure-1.5.1/ml_infrastructure/templates/eval.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)     1530 2023-04-16 14:31:42.000000 ml_infrastructure-1.5.1/ml_infrastructure/templates/header.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      138 2023-04-15 15:08:42.000000 ml_infrastructure-1.5.1/ml_infrastructure/templates/index.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      309 2023-04-15 15:08:42.000000 ml_infrastructure-1.5.1/ml_infrastructure/templates/loss.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)     1706 2023-04-16 14:31:42.000000 ml_infrastructure-1.5.1/ml_infrastructure/templates/stopForm.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      181 2022-11-28 03:17:28.000000 ml_infrastructure-1.5.1/ml_infrastructure/templates/trainingEval.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      452 2023-02-25 17:15:04.000000 ml_infrastructure-1.5.1/ml_infrastructure/templates/trainingLoss.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      189 2022-11-28 03:17:28.000000 ml_infrastructure-1.5.1/ml_infrastructure/templates/validationEval.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      446 2023-02-25 16:35:50.000000 ml_infrastructure-1.5.1/ml_infrastructure/templates/validationLoss.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)     1899 2022-12-13 04:56:19.000000 ml_infrastructure-1.5.1/ml_infrastructure/trainer.py
+drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-04-16 14:46:08.315739 ml_infrastructure-1.5.1/ml_infrastructure.egg-info/
+-rw-rw-r--   0 maple     (1000) maple     (1000)      581 2023-04-16 14:46:08.000000 ml_infrastructure-1.5.1/ml_infrastructure.egg-info/PKG-INFO
+-rw-rw-r--   0 maple     (1000) maple     (1000)      905 2023-04-16 14:46:08.000000 ml_infrastructure-1.5.1/ml_infrastructure.egg-info/SOURCES.txt
+-rw-rw-r--   0 maple     (1000) maple     (1000)        1 2023-04-16 14:46:08.000000 ml_infrastructure-1.5.1/ml_infrastructure.egg-info/dependency_links.txt
+-rw-rw-r--   0 maple     (1000) maple     (1000)       46 2023-04-16 14:46:08.000000 ml_infrastructure-1.5.1/ml_infrastructure.egg-info/requires.txt
+-rw-rw-r--   0 maple     (1000) maple     (1000)       18 2023-04-16 14:46:08.000000 ml_infrastructure-1.5.1/ml_infrastructure.egg-info/top_level.txt
+-rw-rw-r--   0 maple     (1000) maple     (1000)      107 2023-04-16 14:46:08.319739 ml_infrastructure-1.5.1/setup.cfg
+-rw-rw-r--   0 maple     (1000) maple     (1000)      987 2023-04-16 14:45:48.000000 ml_infrastructure-1.5.1/setup.py
```

### Comparing `ml_infrastructure-1.4.3/LICENSE.rst` & `ml_infrastructure-1.5.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.4.3/PKG-INFO` & `ml_infrastructure-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_infrastructure
-Version: 1.4.3
+Version: 1.5.1
 Summary: Software infrastructure to for machine learning
 Author: Ada L
 Author-email: the.nostra.tymus@gmail.com
 License: MIT
 Keywords: machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ml_infrastructure-1.4.3/ml_infrastructure/app.py` & `ml_infrastructure-1.5.1/ml_infrastructure/app.py`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.4.3/ml_infrastructure/evaluator.py` & `ml_infrastructure-1.5.1/ml_infrastructure/evaluator.py`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.4.3/ml_infrastructure/example.py` & `ml_infrastructure-1.5.1/ml_infrastructure/example.py`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.4.3/ml_infrastructure/manager.py` & `ml_infrastructure-1.5.1/ml_infrastructure/manager.py`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.4.3/ml_infrastructure/model.py` & `ml_infrastructure-1.5.1/ml_infrastructure/model.py`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.4.3/ml_infrastructure/templates/header.html` & `ml_infrastructure-1.5.1/ml_infrastructure/templates/header.html`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.4.3/ml_infrastructure/templates/stopForm.html` & `ml_infrastructure-1.5.1/ml_infrastructure/templates/stopForm.html`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.4.3/ml_infrastructure/trainer.py` & `ml_infrastructure-1.5.1/ml_infrastructure/trainer.py`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.4.3/ml_infrastructure.egg-info/PKG-INFO` & `ml_infrastructure-1.5.1/ml_infrastructure.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-infrastructure
-Version: 1.4.3
+Version: 1.5.1
 Summary: Software infrastructure to for machine learning
 Author: Ada L
 Author-email: the.nostra.tymus@gmail.com
 License: MIT
 Keywords: machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ml_infrastructure-1.4.3/ml_infrastructure.egg-info/SOURCES.txt` & `ml_infrastructure-1.5.1/ml_infrastructure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.4.3/setup.py` & `ml_infrastructure-1.5.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = '1.4.3'
+VERSION = '1.5.1'
 DESCRIPTION = 'Software infrastructure to for machine learning'
 LONG_DESCRIPTION = 'Software infrastructure for machine learning projects that makes it easier to manage experiments and log progress'
 
 setup(
     name="ml_infrastructure",
     version=VERSION,
     description=DESCRIPTION,
```

