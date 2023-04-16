# Comparing `tmp/db_simple-0.1.tar.gz` & `tmp/db_simple-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db_simple-0.1.tar", last modified: Sun Apr 16 05:50:11 2023, max compression
+gzip compressed data, was "db_simple-0.3.tar", last modified: Sun Apr 16 06:05:31 2023, max compression
```

## Comparing `db_simple-0.1.tar` & `db_simple-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-16 05:50:11.093392 db_simple-0.1/
--rw-rw----   0 root         (0) everybody  (9997)     1906 2023-04-16 05:50:11.089392 db_simple-0.1/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     1412 2023-04-16 05:46:55.000000 db_simple-0.1/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-16 05:50:11.081392 db_simple-0.1/db_simple.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     1906 2023-04-16 05:50:10.000000 db_simple-0.1/db_simple.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      186 2023-04-16 05:50:10.000000 db_simple-0.1/db_simple.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-16 05:50:10.000000 db_simple-0.1/db_simple.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       46 2023-04-16 05:50:10.000000 db_simple-0.1/db_simple.egg-info/entry_points.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-16 05:50:10.000000 db_simple-0.1/db_simple.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-16 05:50:11.097392 db_simple-0.1/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)      778 2023-04-16 05:48:45.000000 db_simple-0.1/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-16 06:05:31.513392 db_simple-0.3/
+-rw-rw----   0 root         (0) everybody  (9997)     1906 2023-04-16 06:05:31.505391 db_simple-0.3/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     1412 2023-04-16 05:46:55.000000 db_simple-0.3/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-04-16 06:05:31.497392 db_simple-0.3/db_simple.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     1906 2023-04-16 06:05:31.000000 db_simple-0.3/db_simple.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      186 2023-04-16 06:05:31.000000 db_simple-0.3/db_simple.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-16 06:05:31.000000 db_simple-0.3/db_simple.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       46 2023-04-16 06:05:31.000000 db_simple-0.3/db_simple.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-04-16 06:05:31.000000 db_simple-0.3/db_simple.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-04-16 06:05:31.513392 db_simple-0.3/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      778 2023-04-16 06:02:51.000000 db_simple-0.3/setup.py
```

### Comparing `db_simple-0.1/PKG-INFO` & `db_simple-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db_simple
-Version: 0.1
+Version: 0.3
 Summary: Данный модуль , заменяет другие database если вам не удобно их использовать!
 Home-page: UNKNOWN
 Author: Danyamutit23
 Author-email: duaneskalanak@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `db_simple-0.1/README.md` & `db_simple-0.3/README.md`

 * *Files identical despite different names*

### Comparing `db_simple-0.1/db_simple.egg-info/PKG-INFO` & `db_simple-0.3/db_simple.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db-simple
-Version: 0.1
+Version: 0.3
 Summary: Данный модуль , заменяет другие database если вам не удобно их использовать!
 Home-page: UNKNOWN
 Author: Danyamutit23
 Author-email: duaneskalanak@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `db_simple-0.1/setup.py` & `db_simple-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="db_simple",
-    version="0.1",
+    version="0.3",
     author="Danyamutit23",
     author_email="duaneskalanak@gmail.com",
     description="Данный модуль , заменяет другие database если вам не удобно их использовать!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
```

