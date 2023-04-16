# Comparing `tmp/plesicdb-2.0.0.tar.gz` & `tmp/plesicdb-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plesicdb-2.0.0.tar", last modified: Sun Apr 16 13:12:22 2023, max compression
+gzip compressed data, was "plesicdb-2.0.1.tar", last modified: Sun Apr 16 13:21:03 2023, max compression
```

## Comparing `plesicdb-2.0.0.tar` & `plesicdb-2.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 13:12:22.385693 plesicdb-2.0.0/
--rw-rw-rw-   0        0        0     1442 2023-04-16 13:12:22.377385 plesicdb-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      926 2023-04-16 13:10:34.000000 plesicdb-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 13:12:22.366033 plesicdb-2.0.0/plesicdb/
--rw-rw-rw-   0        0        0      146 2023-04-16 13:12:00.000000 plesicdb-2.0.0/plesicdb/__about__.py
--rw-rw-rw-   0        0        0      940 2023-04-16 12:57:20.000000 plesicdb-2.0.0/plesicdb/__init__.py
--rw-rw-rw-   0        0        0    25279 2023-04-16 12:30:05.000000 plesicdb-2.0.0/plesicdb/core.py
--rw-rw-rw-   0        0        0     9415 2023-04-16 12:52:17.000000 plesicdb-2.0.0/plesicdb/fields.py
--rw-rw-rw-   0        0        0     1632 2023-04-16 12:32:24.000000 plesicdb-2.0.0/plesicdb/functions.py
--rw-rw-rw-   0        0        0     2551 2023-04-16 12:54:10.000000 plesicdb-2.0.0/plesicdb/helpers.py
--rw-rw-rw-   0        0        0     1015 2023-04-15 17:26:40.000000 plesicdb-2.0.0/plesicdb/lock.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:12:22.375388 plesicdb-2.0.0/plesicdb.egg-info/
--rw-rw-rw-   0        0        0     1442 2023-04-16 13:12:21.000000 plesicdb-2.0.0/plesicdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-04-16 13:12:21.000000 plesicdb-2.0.0/plesicdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 13:12:21.000000 plesicdb-2.0.0/plesicdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-16 13:12:21.000000 plesicdb-2.0.0/plesicdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 13:12:22.386705 plesicdb-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      791 2023-04-16 13:11:13.000000 plesicdb-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:21:03.570035 plesicdb-2.0.1/
+-rw-rw-rw-   0        0        0     1457 2023-04-16 13:21:03.561866 plesicdb-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      941 2023-04-16 13:19:48.000000 plesicdb-2.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 13:21:03.543962 plesicdb-2.0.1/plesicdb/
+-rw-rw-rw-   0        0        0      146 2023-04-16 13:20:34.000000 plesicdb-2.0.1/plesicdb/__about__.py
+-rw-rw-rw-   0        0        0      940 2023-04-16 12:57:20.000000 plesicdb-2.0.1/plesicdb/__init__.py
+-rw-rw-rw-   0        0        0    25279 2023-04-16 12:30:05.000000 plesicdb-2.0.1/plesicdb/core.py
+-rw-rw-rw-   0        0        0     9415 2023-04-16 12:52:17.000000 plesicdb-2.0.1/plesicdb/fields.py
+-rw-rw-rw-   0        0        0     1632 2023-04-16 12:32:24.000000 plesicdb-2.0.1/plesicdb/functions.py
+-rw-rw-rw-   0        0        0     2551 2023-04-16 12:54:10.000000 plesicdb-2.0.1/plesicdb/helpers.py
+-rw-rw-rw-   0        0        0     1015 2023-04-15 17:26:40.000000 plesicdb-2.0.1/plesicdb/lock.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:21:03.559855 plesicdb-2.0.1/plesicdb.egg-info/
+-rw-rw-rw-   0        0        0     1457 2023-04-16 13:21:03.000000 plesicdb-2.0.1/plesicdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-04-16 13:21:03.000000 plesicdb-2.0.1/plesicdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 13:21:03.000000 plesicdb-2.0.1/plesicdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-16 13:21:03.000000 plesicdb-2.0.1/plesicdb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 13:21:03.571023 plesicdb-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      791 2023-04-16 13:20:27.000000 plesicdb-2.0.1/setup.py
```

### Comparing `plesicdb-2.0.0/PKG-INFO` & `plesicdb-2.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plesicdb
-Version: 2.0.0
+Version: 2.0.1
 Summary: Plesicdb is a simple model based file database
 Home-page: https://github.com/hakiKhuva/plesicdb
 Author: Harkishan Khuva
 Author-email: harkishankhuva02@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -39,15 +39,15 @@
 from plesicdb import connect
 
 user_model = {
     "id": UUIDField("id"),
     "name": StringField("name")
 }
 
-users = connect("users", user_model)
+users = connect("users", list(user_model.values()))
 
 users.insert({
     "name" : "Harkishan Khuva"
 })
 ```
 
 **NOTE :** The first field of any Model must be either `UUIDField` or an `IntegerField`.
```

### Comparing `plesicdb-2.0.0/README.md` & `plesicdb-2.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from plesicdb import connect
 
 user_model = {
     "id": UUIDField("id"),
     "name": StringField("name")
 }
 
-users = connect("users", user_model)
+users = connect("users", list(user_model.values()))
 
 users.insert({
     "name" : "Harkishan Khuva"
 })
 ```
 
 **NOTE :** The first field of any Model must be either `UUIDField` or an `IntegerField`.
```

### Comparing `plesicdb-2.0.0/plesicdb/__init__.py` & `plesicdb-2.0.1/plesicdb/__init__.py`

 * *Files identical despite different names*

### Comparing `plesicdb-2.0.0/plesicdb/core.py` & `plesicdb-2.0.1/plesicdb/core.py`

 * *Files identical despite different names*

### Comparing `plesicdb-2.0.0/plesicdb/fields.py` & `plesicdb-2.0.1/plesicdb/fields.py`

 * *Files identical despite different names*

### Comparing `plesicdb-2.0.0/plesicdb/functions.py` & `plesicdb-2.0.1/plesicdb/functions.py`

 * *Files identical despite different names*

### Comparing `plesicdb-2.0.0/plesicdb/helpers.py` & `plesicdb-2.0.1/plesicdb/helpers.py`

 * *Files identical despite different names*

### Comparing `plesicdb-2.0.0/plesicdb/lock.py` & `plesicdb-2.0.1/plesicdb/lock.py`

 * *Files identical despite different names*

### Comparing `plesicdb-2.0.0/plesicdb.egg-info/PKG-INFO` & `plesicdb-2.0.1/plesicdb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plesicdb
-Version: 2.0.0
+Version: 2.0.1
 Summary: Plesicdb is a simple model based file database
 Home-page: https://github.com/hakiKhuva/plesicdb
 Author: Harkishan Khuva
 Author-email: harkishankhuva02@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -39,15 +39,15 @@
 from plesicdb import connect
 
 user_model = {
     "id": UUIDField("id"),
     "name": StringField("name")
 }
 
-users = connect("users", user_model)
+users = connect("users", list(user_model.values()))
 
 users.insert({
     "name" : "Harkishan Khuva"
 })
 ```
 
 **NOTE :** The first field of any Model must be either `UUIDField` or an `IntegerField`.
```

### Comparing `plesicdb-2.0.0/setup.py` & `plesicdb-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 long_description = ""
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="plesicdb",
-    version="2.0.0",
+    version="2.0.1",
     author="Harkishan Khuva",
     author_email="harkishankhuva02@gmail.com",
     description="Plesicdb is a simple model based file database",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hakiKhuva/plesicdb",
     classifiers=[
```

