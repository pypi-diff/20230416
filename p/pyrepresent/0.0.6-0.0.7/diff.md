# Comparing `tmp/pyrepresent-0.0.6.tar.gz` & `tmp/pyrepresent-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrepresent-0.0.6.tar", last modified: Sat Apr 15 12:29:33 2023, max compression
+gzip compressed data, was "pyrepresent-0.0.7.tar", last modified: Sun Apr 16 14:51:53 2023, max compression
```

## Comparing `pyrepresent-0.0.6.tar` & `pyrepresent-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 12:29:33.668529 pyrepresent-0.0.6/
--rw-rw-rw-   0        0        0      115 2023-04-15 12:29:33.000000 pyrepresent-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     5268 2023-04-15 12:29:33.667530 pyrepresent-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4389 2023-03-21 18:58:55.000000 pyrepresent-0.0.6/README.md
--rw-rw-rw-   0        0        0    12965 2023-03-21 19:21:52.000000 pyrepresent-0.0.6/build.py
--rw-rw-rw-   0        0        0      715 2023-04-15 12:29:29.000000 pyrepresent-0.0.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-15 12:29:33.662564 pyrepresent-0.0.6/pyrepresent.egg-info/
--rw-rw-rw-   0        0        0     5268 2023-04-15 12:29:33.000000 pyrepresent-0.0.6/pyrepresent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-04-15 12:29:33.000000 pyrepresent-0.0.6/pyrepresent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 12:29:33.000000 pyrepresent-0.0.6/pyrepresent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-15 12:29:33.000000 pyrepresent-0.0.6/pyrepresent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-15 12:29:33.000000 pyrepresent-0.0.6/pyrepresent.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-15 12:29:33.667530 pyrepresent-0.0.6/represent/
--rw-rw-rw-   0        0        0       85 2023-03-09 09:17:11.000000 pyrepresent-0.0.6/represent/__init__.py
--rw-rw-rw-   0        0        0     5875 2023-03-09 09:10:13.000000 pyrepresent-0.0.6/represent/base.py
--rw-rw-rw-   0        0        0      202 2023-03-09 09:18:08.000000 pyrepresent-0.0.6/represent/document.py
--rw-rw-rw-   0        0        0     2121 2023-04-05 09:22:18.000000 pyrepresent-0.0.6/represent/indentation.py
--rw-rw-rw-   0        0        0    11524 2023-04-15 12:28:39.000000 pyrepresent-0.0.6/represent/object.py
--rw-rw-rw-   0        0        0    19611 2023-04-09 18:51:47.000000 pyrepresent-0.0.6/represent/structures.py
--rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.0.6/requirements-dev.txt
--rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.0.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 12:29:33.668529 pyrepresent-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-04-15 12:29:26.000000 pyrepresent-0.0.6/setup.py
--rw-rw-rw-   0        0        0      669 2023-03-28 10:53:06.000000 pyrepresent-0.0.6/test.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:51:53.114583 pyrepresent-0.0.7/
+-rw-rw-rw-   0        0        0      115 2023-04-16 14:51:52.000000 pyrepresent-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     5268 2023-04-16 14:51:53.114583 pyrepresent-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4389 2023-03-21 18:58:55.000000 pyrepresent-0.0.7/README.md
+-rw-rw-rw-   0        0        0    12965 2023-03-21 19:21:52.000000 pyrepresent-0.0.7/build.py
+-rw-rw-rw-   0        0        0      715 2023-04-16 14:51:48.000000 pyrepresent-0.0.7/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-16 14:51:53.088067 pyrepresent-0.0.7/pyrepresent.egg-info/
+-rw-rw-rw-   0        0        0     5268 2023-04-16 14:51:52.000000 pyrepresent-0.0.7/pyrepresent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-04-16 14:51:53.000000 pyrepresent-0.0.7/pyrepresent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 14:51:52.000000 pyrepresent-0.0.7/pyrepresent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-16 14:51:52.000000 pyrepresent-0.0.7/pyrepresent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-16 14:51:52.000000 pyrepresent-0.0.7/pyrepresent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 14:51:53.113581 pyrepresent-0.0.7/represent/
+-rw-rw-rw-   0        0        0       85 2023-03-09 09:17:11.000000 pyrepresent-0.0.7/represent/__init__.py
+-rw-rw-rw-   0        0        0     5875 2023-03-09 09:10:13.000000 pyrepresent-0.0.7/represent/base.py
+-rw-rw-rw-   0        0        0      202 2023-03-09 09:18:08.000000 pyrepresent-0.0.7/represent/document.py
+-rw-rw-rw-   0        0        0     2121 2023-04-05 09:22:18.000000 pyrepresent-0.0.7/represent/indentation.py
+-rw-rw-rw-   0        0        0    11534 2023-04-16 14:51:13.000000 pyrepresent-0.0.7/represent/object.py
+-rw-rw-rw-   0        0        0    19611 2023-04-09 18:51:47.000000 pyrepresent-0.0.7/represent/structures.py
+-rw-rw-rw-   0        0        0       30 2023-03-28 10:51:56.000000 pyrepresent-0.0.7/requirements-dev.txt
+-rw-rw-rw-   0        0        0       21 2023-03-28 10:51:53.000000 pyrepresent-0.0.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 14:51:53.114583 pyrepresent-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-04-16 14:51:47.000000 pyrepresent-0.0.7/setup.py
+-rw-rw-rw-   0        0        0      669 2023-03-28 10:53:06.000000 pyrepresent-0.0.7/test.py
```

### Comparing `pyrepresent-0.0.6/PKG-INFO` & `pyrepresent-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.0.6
+Version: 0.0.7
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.0.6/README.md` & `pyrepresent-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.0.6/build.py` & `pyrepresent-0.0.7/build.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.0.6/pyproject.toml` & `pyrepresent-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'pyrepresent'
-version = '0.0.6'
+version = '0.0.7'
 description = 'A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `pyrepresent-0.0.6/pyrepresent.egg-info/PKG-INFO` & `pyrepresent-0.0.7/pyrepresent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrepresent
-Version: 0.0.6
+Version: 0.0.7
 Summary: A module for object and model representations as strings, with vast configurations, colors, hidden and protected values, assignment operations, memory addresses and more.
 Home-page: https://github.com/Shahaf-F-S/represent
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrepresent-0.0.6/represent/base.py` & `pyrepresent-0.0.7/represent/base.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.0.6/represent/indentation.py` & `pyrepresent-0.0.7/represent/indentation.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.0.6/represent/object.py` & `pyrepresent-0.0.7/represent/object.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
 
     if (data_id := id(data)) in ids:
         return ids[data_id]
 
     else:
         ids[data_id] = (
             data if (
-                (data.__class__.__name__ in dir(builtins)) or
+                (data.__class__.__name__ in dir(builtins) + dir(dt)) or
                 (data is None)
             )
             else (
                 (
                     repr(CircularReferenceStructure(data))
                     if legalize else (
                         StringWrapper(repr(CircularReferenceStructure(data)))
```

### Comparing `pyrepresent-0.0.6/represent/structures.py` & `pyrepresent-0.0.7/represent/structures.py`

 * *Files identical despite different names*

### Comparing `pyrepresent-0.0.6/setup.py` & `pyrepresent-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='pyrepresent',
-        version='0.0.6',
+        version='0.0.7',
         description=(
             "A module for object and model representations as strings, "
             "with vast configurations, colors, hidden and protected values, "
             "assignment operations, memory addresses and more."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `pyrepresent-0.0.6/test.py` & `pyrepresent-0.0.7/test.py`

 * *Files identical despite different names*

