# Comparing `tmp/industrialucn-0.1.7.2.tar.gz` & `tmp/industrialucn-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\industrialucn-0.1.7.2.tar", last modified: Sat Oct  3 18:15:50 2020, max compression
+gzip compressed data, was "industrialucn-0.2.0.tar", last modified: Sun Apr 16 01:47:35 2023, max compression
```

## Comparing `industrialucn-0.1.7.2.tar` & `industrialucn-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2020-10-03 18:15:50.000000 industrialucn-0.1.7.2/
--rw-rw-rw-   0        0        0      920 2020-10-03 18:15:50.000000 industrialucn-0.1.7.2/PKG-INFO
--rw-rw-rw-   0        0        0      264 2020-10-03 17:51:49.000000 industrialucn-0.1.7.2/README.md
-drwxrwxrwx   0        0        0        0 2020-10-03 18:15:50.000000 industrialucn-0.1.7.2/industrialucn/
--rw-rw-rw-   0        0        0       40 2020-10-03 17:51:49.000000 industrialucn-0.1.7.2/industrialucn/__init__.py
--rw-rw-rw-   0        0        0     7390 2020-10-03 17:51:49.000000 industrialucn-0.1.7.2/industrialucn/econstraint.py
--rw-rw-rw-   0        0        0    10140 2020-10-03 17:51:49.000000 industrialucn-0.1.7.2/industrialucn/econstraint_test.py
-drwxrwxrwx   0        0        0        0 2020-10-03 18:15:50.000000 industrialucn-0.1.7.2/industrialucn/experimental/
--rw-rw-rw-   0        0        0       20 2020-10-03 14:17:52.000000 industrialucn-0.1.7.2/industrialucn/experimental/__init__.py
--rw-rw-rw-   0        0        0     3400 2020-10-03 14:17:52.000000 industrialucn-0.1.7.2/industrialucn/experimental/osrm.py
-drwxrwxrwx   0        0        0        0 2020-10-03 18:15:50.000000 industrialucn-0.1.7.2/industrialucn.egg-info/
--rw-rw-rw-   0        0        0      920 2020-10-03 18:15:49.000000 industrialucn-0.1.7.2/industrialucn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2020-10-03 18:15:49.000000 industrialucn-0.1.7.2/industrialucn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-10-03 18:15:49.000000 industrialucn-0.1.7.2/industrialucn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2020-10-03 18:15:49.000000 industrialucn-0.1.7.2/industrialucn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-10-03 18:15:50.000000 industrialucn-0.1.7.2/setup.cfg
--rw-rw-rw-   0        0        0      807 2020-10-03 18:15:35.000000 industrialucn-0.1.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:47:35.399767 industrialucn-0.2.0/
+-rw-rw-rw-   0        0        0    35823 2023-04-16 01:24:32.000000 industrialucn-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      850 2023-04-16 01:47:35.398685 industrialucn-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-04-16 01:24:32.000000 industrialucn-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 01:47:35.383177 industrialucn-0.2.0/industrialucn/
+-rw-rw-rw-   0        0        0       40 2023-04-16 01:24:32.000000 industrialucn-0.2.0/industrialucn/__init__.py
+-rw-rw-rw-   0        0        0     7390 2023-04-16 01:24:32.000000 industrialucn-0.2.0/industrialucn/econstraint.py
+-rw-rw-rw-   0        0        0    10140 2023-04-16 01:24:32.000000 industrialucn-0.2.0/industrialucn/econstraint_test.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:47:35.396764 industrialucn-0.2.0/industrialucn/experimental/
+-rw-rw-rw-   0        0        0       20 2023-04-16 01:24:32.000000 industrialucn-0.2.0/industrialucn/experimental/__init__.py
+-rw-rw-rw-   0        0        0     3400 2023-04-16 01:24:32.000000 industrialucn-0.2.0/industrialucn/experimental/osrm.py
+-rw-rw-rw-   0        0        0     5875 2023-04-16 01:43:39.000000 industrialucn-0.2.0/industrialucn/queueing.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:47:35.391569 industrialucn-0.2.0/industrialucn.egg-info/
+-rw-rw-rw-   0        0        0      850 2023-04-16 01:47:35.000000 industrialucn-0.2.0/industrialucn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2023-04-16 01:47:35.000000 industrialucn-0.2.0/industrialucn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 01:47:35.000000 industrialucn-0.2.0/industrialucn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-16 01:47:35.000000 industrialucn-0.2.0/industrialucn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 01:47:35.399767 industrialucn-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      804 2023-04-16 01:47:12.000000 industrialucn-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `industrialucn-0.1.7.2/PKG-INFO` & `industrialucn-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: industrialucn
-Version: 0.1.7.2
+Version: 0.2.0
 Summary: Generic tool for numerical experiments
 Home-page: https://industrial.ucn.cl
 Author: Hernan Caceres
-Author-email: idustrial@ucn.cl
-License: UNKNOWN
-Description: # IndustrialUCN
-        
-        IndustrialUCN is an open-source effort from the Industrial Engineering Community at Universidad CatÃ³lica del Norte, 
-        Chile ([industrial.ucn.cl](https://industrial.ucn.cl)). This package is intended for students
-        and researchers of our field.
-        
-Platform: UNKNOWN
+Author-email: hcaceres@ucn.cl
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# IndustrialUCN
+
+IndustrialUCN is an open-source effort from the Industrial Engineering Community at Universidad CatÃ³lica del Norte, 
+Chile ([industrial.ucn.cl](https://industrial.ucn.cl)). This package is intended for students
+and researchers of our field.
```

### Comparing `industrialucn-0.1.7.2/industrialucn/econstraint.py` & `industrialucn-0.2.0/industrialucn/econstraint.py`

 * *Files identical despite different names*

### Comparing `industrialucn-0.1.7.2/industrialucn/econstraint_test.py` & `industrialucn-0.2.0/industrialucn/econstraint_test.py`

 * *Files identical despite different names*

### Comparing `industrialucn-0.1.7.2/industrialucn/experimental/osrm.py` & `industrialucn-0.2.0/industrialucn/experimental/osrm.py`

 * *Files identical despite different names*

### Comparing `industrialucn-0.1.7.2/industrialucn.egg-info/PKG-INFO` & `industrialucn-0.2.0/industrialucn.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: industrialucn
-Version: 0.1.7.2
+Version: 0.2.0
 Summary: Generic tool for numerical experiments
 Home-page: https://industrial.ucn.cl
 Author: Hernan Caceres
-Author-email: idustrial@ucn.cl
-License: UNKNOWN
-Description: # IndustrialUCN
-        
-        IndustrialUCN is an open-source effort from the Industrial Engineering Community at Universidad CatÃ³lica del Norte, 
-        Chile ([industrial.ucn.cl](https://industrial.ucn.cl)). This package is intended for students
-        and researchers of our field.
-        
-Platform: UNKNOWN
+Author-email: hcaceres@ucn.cl
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# IndustrialUCN
+
+IndustrialUCN is an open-source effort from the Industrial Engineering Community at Universidad CatÃ³lica del Norte, 
+Chile ([industrial.ucn.cl](https://industrial.ucn.cl)). This package is intended for students
+and researchers of our field.
```

### Comparing `industrialucn-0.1.7.2/setup.py` & `industrialucn-0.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="industrialucn",
-    version="0.1.7.2",
+    version="0.2.0",
     author="Hernan Caceres",
-    author_email="idustrial@ucn.cl",
+    author_email="hcaceres@ucn.cl",
     description="Generic tool for numerical experiments",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://industrial.ucn.cl",
     packages=setuptools.find_packages(),
     classifiers=[
         "Development Status :: 3 - Alpha",
```

