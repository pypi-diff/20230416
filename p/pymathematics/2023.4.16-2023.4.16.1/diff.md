# Comparing `tmp/pymathematics-2023.4.16.tar.gz` & `tmp/pymathematics-2023.4.16.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymathematics-2023.4.16.tar", last modified: Sun Apr 16 06:14:23 2023, max compression
+gzip compressed data, was "pymathematics-2023.4.16.1.tar", last modified: Sun Apr 16 06:29:55 2023, max compression
```

## Comparing `pymathematics-2023.4.16.tar` & `pymathematics-2023.4.16.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-16 06:14:23.471387 pymathematics-2023.4.16/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.16/LICENSE
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-16 06:14:23.463088 pymathematics-2023.4.16/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       28 2023-04-16 06:01:41.000000 pymathematics-2023.4.16/README.md
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-16 06:14:23.228056 pymathematics-2023.4.16/pymathematics/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      112 2023-04-16 06:00:49.000000 pymathematics-2023.4.16/pymathematics/info.py
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     7971 2023-04-16 05:59:31.000000 pymathematics-2023.4.16/pymathematics/main.py
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-16 06:14:23.414087 pymathematics-2023.4.16/pymathematics.egg-info/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-16 06:14:21.000000 pymathematics-2023.4.16/pymathematics.egg-info/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      218 2023-04-16 06:14:21.000000 pymathematics-2023.4.16/pymathematics.egg-info/SOURCES.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-16 06:14:21.000000 pymathematics-2023.4.16/pymathematics.egg-info/dependency_links.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-16 06:14:21.000000 pymathematics-2023.4.16/pymathematics.egg-info/top_level.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-16 06:14:23.473411 pymathematics-2023.4.16/setup.cfg
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      690 2023-04-15 19:34:46.000000 pymathematics-2023.4.16/setup.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-16 06:29:55.952398 pymathematics-2023.4.16.1/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.16.1/LICENSE
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      509 2023-04-16 06:29:55.924712 pymathematics-2023.4.16.1/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       30 2023-04-16 06:28:23.000000 pymathematics-2023.4.16.1/README.md
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-16 06:29:55.669618 pymathematics-2023.4.16.1/pymathematics/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     7996 2023-04-16 06:28:36.000000 pymathematics-2023.4.16.1/pymathematics/__init__.py
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      112 2023-04-16 06:00:49.000000 pymathematics-2023.4.16.1/pymathematics/info.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-16 06:29:55.869623 pymathematics-2023.4.16.1/pymathematics.egg-info/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      509 2023-04-16 06:29:55.000000 pymathematics-2023.4.16.1/pymathematics.egg-info/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      222 2023-04-16 06:29:55.000000 pymathematics-2023.4.16.1/pymathematics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-16 06:29:55.000000 pymathematics-2023.4.16.1/pymathematics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-16 06:29:55.000000 pymathematics-2023.4.16.1/pymathematics.egg-info/top_level.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-16 06:29:55.955387 pymathematics-2023.4.16.1/setup.cfg
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      692 2023-04-16 06:23:12.000000 pymathematics-2023.4.16.1/setup.py
```

### Comparing `pymathematics-2023.4.16/LICENSE` & `pymathematics-2023.4.16.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymathematics-2023.4.16/pymathematics/main.py` & `pymathematics-2023.4.16.1/pymathematics/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-import info
+from .info import (
+    author,version,homepage
+)
 
-author = info.author
-version = info.version
-homepage = info.homepage
+author = author
+version = version
+homepage = homepage
 
 class constants:
     pi = 3.1415926535897932384626433832795
     exp = 2.7182818284590452353602874713527
 
 def factorial(number: int) -> int:
     if number == 0:
```

### Comparing `pymathematics-2023.4.16/setup.py` & `pymathematics-2023.4.16.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name = "pymathematics",
-    version = "2023.04.16",
+    version = "2023.04.16.1",
     description = "package for mathematics",
     long_description = "for more info, check the github repository",
     author = "Sahil Rajwar",
     maintainer = "its_Sahil",
     author_email = "justsahilrajwar2004@gmail.com",
     packages = ["pymathematics"],
     license = "MIT",
```

