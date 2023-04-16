# Comparing `tmp/Erutils-1.3.1.tar.gz` & `tmp/erutils-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Erutils-1.3.1.tar", last modified: Sat Apr 15 14:15:12 2023, max compression
+gzip compressed data, was "erutils-1.3.2.tar", last modified: Sun Apr 16 07:20:45 2023, max compression
```

## Comparing `Erutils-1.3.1.tar` & `erutils-1.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-04-15 14:15:12.733213 Erutils-1.3.1/
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-04-15 14:15:12.729213 Erutils-1.3.1/Erutils/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      601 2023-04-15 14:09:00.000000 Erutils-1.3.1/Erutils/__init__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      160 2023-04-15 14:06:10.000000 Erutils-1.3.1/Erutils/__main__.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       67 2023-04-15 14:06:10.000000 Erutils-1.3.1/Erutils/config.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    32172 2023-04-15 14:06:10.000000 Erutils-1.3.1/Erutils/lightning.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3379 2023-04-15 14:06:10.000000 Erutils-1.3.1/Erutils/loggers.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    47142 2023-04-15 14:06:10.000000 Erutils-1.3.1/Erutils/nn.py
--rw-rw-r--   0 erfan     (1000) erfan     (1000)    12973 2023-04-15 14:07:54.000000 Erutils-1.3.1/Erutils/utils.py
-drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-04-15 14:15:12.729213 Erutils-1.3.1/Erutils.egg-info/
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3023 2023-04-15 14:15:12.000000 Erutils-1.3.1/Erutils.egg-info/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      316 2023-04-15 14:15:12.000000 Erutils-1.3.1/Erutils.egg-info/SOURCES.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-04-15 14:15:12.000000 Erutils-1.3.1/Erutils.egg-info/dependency_links.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      120 2023-04-15 14:15:12.000000 Erutils-1.3.1/Erutils.egg-info/requires.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-04-15 14:15:12.000000 Erutils-1.3.1/Erutils.egg-info/top_level.txt
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     3023 2023-04-15 14:15:12.729213 Erutils-1.3.1/PKG-INFO
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     2287 2023-04-15 14:06:10.000000 Erutils-1.3.1/README.md
--rw-rw-r--   0 erfan     (1000) erfan     (1000)      576 2023-04-15 14:06:10.000000 Erutils-1.3.1/pyproject.toml
--rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-04-15 14:15:12.733213 Erutils-1.3.1/setup.cfg
--rw-rw-r--   0 erfan     (1000) erfan     (1000)     1272 2023-04-15 14:15:02.000000 Erutils-1.3.1/setup.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-04-16 07:20:45.074921 erutils-1.3.2/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3023 2023-04-16 07:20:45.074921 erutils-1.3.2/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2287 2023-04-16 07:20:29.000000 erutils-1.3.2/README.md
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-04-16 07:20:45.070922 erutils-1.3.2/erutils/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      601 2023-04-15 14:09:00.000000 erutils-1.3.2/erutils/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      160 2023-04-15 14:06:10.000000 erutils-1.3.2/erutils/__main__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       67 2023-04-15 14:06:10.000000 erutils-1.3.2/erutils/config.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    32172 2023-04-15 14:06:10.000000 erutils-1.3.2/erutils/lightning.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3379 2023-04-15 14:06:10.000000 erutils-1.3.2/erutils/loggers.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    47142 2023-04-15 14:06:10.000000 erutils-1.3.2/erutils/nn.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    12973 2023-04-15 14:07:54.000000 erutils-1.3.2/erutils/utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2023-04-16 07:20:45.074921 erutils-1.3.2/erutils.egg-info/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3023 2023-04-16 07:20:45.000000 erutils-1.3.2/erutils.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      316 2023-04-16 07:20:45.000000 erutils-1.3.2/erutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2023-04-16 07:20:45.000000 erutils-1.3.2/erutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      120 2023-04-16 07:20:45.000000 erutils-1.3.2/erutils.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        8 2023-04-16 07:20:45.000000 erutils-1.3.2/erutils.egg-info/top_level.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      576 2023-04-15 14:06:10.000000 erutils-1.3.2/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2023-04-16 07:20:45.074921 erutils-1.3.2/setup.cfg
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1272 2023-04-16 07:20:29.000000 erutils-1.3.2/setup.py
```

### Comparing `Erutils-1.3.1/Erutils/__init__.py` & `erutils-1.3.2/erutils/__init__.py`

 * *Files identical despite different names*

### Comparing `Erutils-1.3.1/Erutils/lightning.py` & `erutils-1.3.2/erutils/lightning.py`

 * *Files identical despite different names*

### Comparing `Erutils-1.3.1/Erutils/loggers.py` & `erutils-1.3.2/erutils/loggers.py`

 * *Files identical despite different names*

### Comparing `Erutils-1.3.1/Erutils/nn.py` & `erutils-1.3.2/erutils/nn.py`

 * *Files identical despite different names*

### Comparing `Erutils-1.3.1/Erutils/utils.py` & `erutils-1.3.2/erutils/utils.py`

 * *Files identical despite different names*

### Comparing `Erutils-1.3.1/Erutils.egg-info/PKG-INFO` & `erutils-1.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Erutils
-Version: 1.3.1
+Name: erutils
+Version: 1.3.2
 Summary: UNKNOWN
 Home-page: https://github.com/erfanzar/
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@yahoo.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -25,34 +25,34 @@
 personal projects. While this package is mainly for my personal use, others may find it useful as well.
 
 # Installation
 
 You can install Erutils using pip:
 
 ```shell
-pip install Erutils
+pip install erutils
 ````
 
 Open [erfan zare Github](https://github.com/erfanzar/)
 
 Open [Package Github](https://github.com/erfanzar/Erutils)
 
 ## 🚀 APIs and Usages
 
 ```python
-import Erutils
-from Erutils.loggers import *
+import erutils
+from erutils.loggers import *
 # Loggers contain Logging stuff
-from Erutils.nn import *
+from erutils.nn import *
 # NN contain Nural networks built in Pytorch
-# you can easily import Erutils.nn and use many prebuilt neurons in the project 
+# you can easily import erutils.nn and use many prebuilt neurons in the project 
 # if you thing any refrence should be added tell me in discussion 
-from Erutils.lightning import *
+from erutils.lightning import *
 # Lightning Contain Some CV Packages
-from Erutils.utils import *
+from erutils.utils import *
 # Utils Contain Some Utils like reading files downloading and etc ...
 ```
 
 # Neural Networks
 
 Erutils includes a diverse collection of over 80 pre-built neural networks that cover a wide range of applications, such
 as natural language processing, computer vision, and more. Some of the neural networks included are:
```

### Comparing `Erutils-1.3.1/PKG-INFO` & `erutils-1.3.2/erutils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Erutils
-Version: 1.3.1
+Name: erutils
+Version: 1.3.2
 Summary: UNKNOWN
 Home-page: https://github.com/erfanzar/
 Author: Erfan Zare Chavoshi
 Author-email: erfanzare82@yahoo.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -25,34 +25,34 @@
 personal projects. While this package is mainly for my personal use, others may find it useful as well.
 
 # Installation
 
 You can install Erutils using pip:
 
 ```shell
-pip install Erutils
+pip install erutils
 ````
 
 Open [erfan zare Github](https://github.com/erfanzar/)
 
 Open [Package Github](https://github.com/erfanzar/Erutils)
 
 ## 🚀 APIs and Usages
 
 ```python
-import Erutils
-from Erutils.loggers import *
+import erutils
+from erutils.loggers import *
 # Loggers contain Logging stuff
-from Erutils.nn import *
+from erutils.nn import *
 # NN contain Nural networks built in Pytorch
-# you can easily import Erutils.nn and use many prebuilt neurons in the project 
+# you can easily import erutils.nn and use many prebuilt neurons in the project 
 # if you thing any refrence should be added tell me in discussion 
-from Erutils.lightning import *
+from erutils.lightning import *
 # Lightning Contain Some CV Packages
-from Erutils.utils import *
+from erutils.utils import *
 # Utils Contain Some Utils like reading files downloading and etc ...
 ```
 
 # Neural Networks
 
 Erutils includes a diverse collection of over 80 pre-built neural networks that cover a wide range of applications, such
 as natural language processing, computer vision, and more. Some of the neural networks included are:
```

### Comparing `Erutils-1.3.1/README.md` & `erutils-1.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 personal projects. While this package is mainly for my personal use, others may find it useful as well.
 
 # Installation
 
 You can install Erutils using pip:
 
 ```shell
-pip install Erutils
+pip install erutils
 ````
 
 Open [erfan zare Github](https://github.com/erfanzar/)
 
 Open [Package Github](https://github.com/erfanzar/Erutils)
 
 ## 🚀 APIs and Usages
 
 ```python
-import Erutils
-from Erutils.loggers import *
+import erutils
+from erutils.loggers import *
 # Loggers contain Logging stuff
-from Erutils.nn import *
+from erutils.nn import *
 # NN contain Nural networks built in Pytorch
-# you can easily import Erutils.nn and use many prebuilt neurons in the project 
+# you can easily import erutils.nn and use many prebuilt neurons in the project 
 # if you thing any refrence should be added tell me in discussion 
-from Erutils.lightning import *
+from erutils.lightning import *
 # Lightning Contain Some CV Packages
-from Erutils.utils import *
+from erutils.utils import *
 # Utils Contain Some Utils like reading files downloading and etc ...
 ```
 
 # Neural Networks
 
 Erutils includes a diverse collection of over 80 pre-built neural networks that cover a wide range of applications, such
 as natural language processing, computer vision, and more. Some of the neural networks included are:
```

### Comparing `Erutils-1.3.1/pyproject.toml` & `erutils-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Erutils-1.3.1/setup.py` & `erutils-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
-    name="Erutils",
-    version='1.3.1',
+    name="erutils",
+    version='1.3.2',
     author="Erfan Zare Chavoshi",
     author_email="erfanzare82@yahoo.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/erfanzar/",
     packages=setuptools.find_packages(),
     install_requires=[
```

