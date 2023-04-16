# Comparing `tmp/cryptographyComplements-0.2.6.tar.gz` & `tmp/cryptographyComplements-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptographyComplements-0.2.6.tar", last modified: Mon Apr 10 21:59:08 2023, max compression
+gzip compressed data, was "cryptographyComplements-0.2.7.tar", last modified: Sun Apr 16 13:33:31 2023, max compression
```

## Comparing `cryptographyComplements-0.2.6.tar` & `cryptographyComplements-0.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 21:59:08.067495 cryptographyComplements-0.2.6/
--rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.2.6/LICENSE
--rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.2.6/MANIFEST.in
--rw-rw-rw-   0        0        0      579 2023-04-10 21:59:08.066147 cryptographyComplements-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-04-10 21:25:57.000000 cryptographyComplements-0.2.6/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 21:59:08.055642 cryptographyComplements-0.2.6/cryptographyComplements/
--rw-rw-rw-   0        0        0      203 2023-04-10 21:55:26.000000 cryptographyComplements-0.2.6/cryptographyComplements/__init__.py
--rw-rw-rw-   0        0        0     2963 2023-04-10 21:52:48.000000 cryptographyComplements-0.2.6/cryptographyComplements/cryptosystems.py
--rw-rw-rw-   0        0        0    10286 2023-04-10 21:53:29.000000 cryptographyComplements-0.2.6/cryptographyComplements/mathFunctions.py
--rw-rw-rw-   0        0        0     2575 2023-04-10 21:54:35.000000 cryptographyComplements-0.2.6/cryptographyComplements/primalityTests.py
--rw-rw-rw-   0        0        0     2332 2023-04-10 21:55:09.000000 cryptographyComplements-0.2.6/cryptographyComplements/tools.py
-drwxrwxrwx   0        0        0        0 2023-04-10 21:59:08.065085 cryptographyComplements-0.2.6/cryptographyComplements.egg-info/
--rw-rw-rw-   0        0        0      285 2023-04-10 21:59:07.000000 cryptographyComplements-0.2.6/cryptographyComplements.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 21:59:08.067495 cryptographyComplements-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      742 2023-04-10 21:59:02.000000 cryptographyComplements-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:33:31.305603 cryptographyComplements-0.2.7/
+-rw-rw-rw-   0        0        0    35823 2023-03-09 20:16:46.000000 cryptographyComplements-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0      186 2023-03-10 20:09:27.000000 cryptographyComplements-0.2.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      579 2023-04-16 13:33:31.305101 cryptographyComplements-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-04-10 21:25:57.000000 cryptographyComplements-0.2.7/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:33:31.302051 cryptographyComplements-0.2.7/cryptographyComplements/
+-rw-rw-rw-   0        0        0      203 2023-04-10 21:55:26.000000 cryptographyComplements-0.2.7/cryptographyComplements/__init__.py
+-rw-rw-rw-   0        0        0     2963 2023-04-10 21:52:48.000000 cryptographyComplements-0.2.7/cryptographyComplements/cryptosystems.py
+-rw-rw-rw-   0        0        0    10286 2023-04-10 21:53:29.000000 cryptographyComplements-0.2.7/cryptographyComplements/mathFunctions.py
+-rw-rw-rw-   0        0        0     2575 2023-04-10 21:54:35.000000 cryptographyComplements-0.2.7/cryptographyComplements/primalityTests.py
+-rw-rw-rw-   0        0        0     3166 2023-04-16 13:32:27.000000 cryptographyComplements-0.2.7/cryptographyComplements/tools.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:33:31.304060 cryptographyComplements-0.2.7/cryptographyComplements.egg-info/
+-rw-rw-rw-   0        0        0      285 2023-04-16 13:33:31.000000 cryptographyComplements-0.2.7/cryptographyComplements.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 13:33:31.306785 cryptographyComplements-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      742 2023-04-16 13:33:11.000000 cryptographyComplements-0.2.7/setup.py
```

### Comparing `cryptographyComplements-0.2.6/LICENSE` & `cryptographyComplements-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.2.6/PKG-INFO` & `cryptographyComplements-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptographyComplements
-Version: 0.2.6
+Version: 0.2.7
 Summary: A Python library, in development, that allows the user to use cryptography, and related, functions.
 Author: Forzo
 License: GPL-3.0
 Project-URL: Source, https://github.com/Forzooo/cryptographyComplements
 Project-URL: Documentation, https://cryptographycomplements.readthedocs.io/
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
```

### Comparing `cryptographyComplements-0.2.6/cryptographyComplements/cryptosystems.py` & `cryptographyComplements-0.2.7/cryptographyComplements/cryptosystems.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.2.6/cryptographyComplements/mathFunctions.py` & `cryptographyComplements-0.2.7/cryptographyComplements/mathFunctions.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.2.6/cryptographyComplements/primalityTests.py` & `cryptographyComplements-0.2.7/cryptographyComplements/primalityTests.py`

 * *Files identical despite different names*

### Comparing `cryptographyComplements-0.2.6/setup.py` & `cryptographyComplements-0.2.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cryptographyComplements',
-    version='0.2.6',
+    version='0.2.7',
     description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description='A Python library, in development, that allows the user to use cryptography, and related, functions.',
     long_description_content_type='text/markdown',
     author='Forzo',
     packages=find_packages(),
     license="GPL-3.0",
     project_urls={
```

