# Comparing `tmp/simple_flask_restful-0.1.0.tar.gz` & `tmp/simple_flask_restful-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_flask_restful-0.1.0.tar", last modified: Sun Apr 16 05:18:01 2023, max compression
+gzip compressed data, was "simple_flask_restful-0.2.0.tar", last modified: Sun Apr 16 21:18:08 2023, max compression
```

## Comparing `simple_flask_restful-0.1.0.tar` & `simple_flask_restful-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-04-16 05:18:01.291990 simple_flask_restful-0.1.0/
--rw-r--r--   0 wwang2     (501) staff       (20)     1069 2023-04-16 02:39:40.000000 simple_flask_restful-0.1.0/LICENSE
--rw-r--r--   0 wwang2     (501) staff       (20)     4422 2023-04-16 05:18:01.291866 simple_flask_restful-0.1.0/PKG-INFO
--rw-r--r--   0 wwang2     (501) staff       (20)     3913 2023-04-16 02:53:09.000000 simple_flask_restful-0.1.0/README.md
--rw-r--r--   0 wwang2     (501) staff       (20)       38 2023-04-16 05:18:01.292031 simple_flask_restful-0.1.0/setup.cfg
--rw-r--r--   0 wwang2     (501) staff       (20)      856 2023-04-16 00:49:24.000000 simple_flask_restful-0.1.0/setup.py
-drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-04-16 05:18:01.288786 simple_flask_restful-0.1.0/src/
-drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-04-16 05:18:01.290725 simple_flask_restful-0.1.0/src/simple_flask_restful/
--rw-r--r--   0 wwang2     (501) staff       (20)      126 2023-04-15 07:43:03.000000 simple_flask_restful-0.1.0/src/simple_flask_restful/__init__.py
--rw-r--r--   0 wwang2     (501) staff       (20)      733 2023-04-13 00:01:43.000000 simple_flask_restful-0.1.0/src/simple_flask_restful/decorator_method.py
--rw-r--r--   0 wwang2     (501) staff       (20)     1912 2023-04-15 09:37:19.000000 simple_flask_restful-0.1.0/src/simple_flask_restful/reqparse.py
--rw-r--r--   0 wwang2     (501) staff       (20)      296 2023-04-15 05:22:11.000000 simple_flask_restful-0.1.0/src/simple_flask_restful/restful_exceptions.py
--rw-r--r--   0 wwang2     (501) staff       (20)     2370 2023-04-13 10:56:46.000000 simple_flask_restful-0.1.0/src/simple_flask_restful/simple_restful.py
-drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-04-16 05:18:01.291672 simple_flask_restful-0.1.0/src/simple_flask_restful.egg-info/
--rw-r--r--   0 wwang2     (501) staff       (20)     4422 2023-04-16 05:18:01.000000 simple_flask_restful-0.1.0/src/simple_flask_restful.egg-info/PKG-INFO
--rw-r--r--   0 wwang2     (501) staff       (20)      474 2023-04-16 05:18:01.000000 simple_flask_restful-0.1.0/src/simple_flask_restful.egg-info/SOURCES.txt
--rw-r--r--   0 wwang2     (501) staff       (20)        1 2023-04-16 05:18:01.000000 simple_flask_restful-0.1.0/src/simple_flask_restful.egg-info/dependency_links.txt
--rw-r--r--   0 wwang2     (501) staff       (20)       27 2023-04-16 05:18:01.000000 simple_flask_restful-0.1.0/src/simple_flask_restful.egg-info/requires.txt
--rw-r--r--   0 wwang2     (501) staff       (20)       21 2023-04-16 05:18:01.000000 simple_flask_restful-0.1.0/src/simple_flask_restful.egg-info/top_level.txt
+drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-04-16 21:18:08.654151 simple_flask_restful-0.2.0/
+-rw-r--r--   0 wwang2     (501) staff       (20)     1069 2023-04-16 02:39:40.000000 simple_flask_restful-0.2.0/LICENSE
+-rw-r--r--   0 wwang2     (501) staff       (20)     4423 2023-04-16 21:18:08.654025 simple_flask_restful-0.2.0/PKG-INFO
+-rw-r--r--   0 wwang2     (501) staff       (20)     3913 2023-04-16 02:53:09.000000 simple_flask_restful-0.2.0/README.md
+-rw-r--r--   0 wwang2     (501) staff       (20)       38 2023-04-16 21:18:08.654196 simple_flask_restful-0.2.0/setup.cfg
+-rw-r--r--   0 wwang2     (501) staff       (20)      858 2023-04-16 21:12:42.000000 simple_flask_restful-0.2.0/setup.py
+drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-04-16 21:18:08.651895 simple_flask_restful-0.2.0/src/
+drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-04-16 21:18:08.653104 simple_flask_restful-0.2.0/src/simple_flask_restful/
+-rw-r--r--   0 wwang2     (501) staff       (20)      358 2023-04-16 21:04:02.000000 simple_flask_restful-0.2.0/src/simple_flask_restful/__init__.py
+-rw-r--r--   0 wwang2     (501) staff       (20)      733 2023-04-13 00:01:43.000000 simple_flask_restful-0.2.0/src/simple_flask_restful/decorator_method.py
+-rw-r--r--   0 wwang2     (501) staff       (20)     1912 2023-04-15 09:37:19.000000 simple_flask_restful-0.2.0/src/simple_flask_restful/reqparse.py
+-rw-r--r--   0 wwang2     (501) staff       (20)      296 2023-04-15 05:22:11.000000 simple_flask_restful-0.2.0/src/simple_flask_restful/restful_exceptions.py
+-rw-r--r--   0 wwang2     (501) staff       (20)     2370 2023-04-13 10:56:46.000000 simple_flask_restful-0.2.0/src/simple_flask_restful/simple_restful.py
+drwxr-xr-x   0 wwang2     (501) staff       (20)        0 2023-04-16 21:18:08.653824 simple_flask_restful-0.2.0/src/simple_flask_restful.egg-info/
+-rw-r--r--   0 wwang2     (501) staff       (20)     4423 2023-04-16 21:18:08.000000 simple_flask_restful-0.2.0/src/simple_flask_restful.egg-info/PKG-INFO
+-rw-r--r--   0 wwang2     (501) staff       (20)      474 2023-04-16 21:18:08.000000 simple_flask_restful-0.2.0/src/simple_flask_restful.egg-info/SOURCES.txt
+-rw-r--r--   0 wwang2     (501) staff       (20)        1 2023-04-16 21:18:08.000000 simple_flask_restful-0.2.0/src/simple_flask_restful.egg-info/dependency_links.txt
+-rw-r--r--   0 wwang2     (501) staff       (20)       27 2023-04-16 21:18:08.000000 simple_flask_restful-0.2.0/src/simple_flask_restful.egg-info/requires.txt
+-rw-r--r--   0 wwang2     (501) staff       (20)       21 2023-04-16 21:18:08.000000 simple_flask_restful-0.2.0/src/simple_flask_restful.egg-info/top_level.txt
```

### Comparing `simple_flask_restful-0.1.0/LICENSE` & `simple_flask_restful-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_flask_restful-0.1.0/PKG-INFO` & `simple_flask_restful-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: simple_flask_restful
-Version: 0.1.0
-Summary: wrap up flask for restul interface
+Version: 0.2.0
+Summary: wrap up flask for restful interface
 Home-page: https://github.com/AutomationLover/simple_flask_restful
 Author: William Wang
 Author-email: williamwangatsydney@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # simple_flask_restful
 
 `simple_flask_restful` is a lightweight Python package that provides a simpler interface to create RESTful APIs using Flask.
```

### Comparing `simple_flask_restful-0.1.0/README.md` & `simple_flask_restful-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `simple_flask_restful-0.1.0/setup.py` & `simple_flask_restful-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from setuptools import (
     setup,
     find_packages
 )
 
+
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='simple_flask_restful',
-    version='0.1.0',
+    version='0.2.0',
     author='William Wang',
     author_email='williamwangatsydney@gmail.com',
-    description='wrap up flask for restul interface',
+    description='wrap up flask for restful interface',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/AutomationLover/simple_flask_restful',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.9',
+    python_requires='>=3.7',
     install_requires=requirements
 )
```

### Comparing `simple_flask_restful-0.1.0/src/simple_flask_restful/decorator_method.py` & `simple_flask_restful-0.2.0/src/simple_flask_restful/decorator_method.py`

 * *Files identical despite different names*

### Comparing `simple_flask_restful-0.1.0/src/simple_flask_restful/reqparse.py` & `simple_flask_restful-0.2.0/src/simple_flask_restful/reqparse.py`

 * *Files identical despite different names*

### Comparing `simple_flask_restful-0.1.0/src/simple_flask_restful/simple_restful.py` & `simple_flask_restful-0.2.0/src/simple_flask_restful/simple_restful.py`

 * *Files identical despite different names*

### Comparing `simple_flask_restful-0.1.0/src/simple_flask_restful.egg-info/PKG-INFO` & `simple_flask_restful-0.2.0/src/simple_flask_restful.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: simple-flask-restful
-Version: 0.1.0
-Summary: wrap up flask for restul interface
+Version: 0.2.0
+Summary: wrap up flask for restful interface
 Home-page: https://github.com/AutomationLover/simple_flask_restful
 Author: William Wang
 Author-email: williamwangatsydney@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # simple_flask_restful
 
 `simple_flask_restful` is a lightweight Python package that provides a simpler interface to create RESTful APIs using Flask.
```

