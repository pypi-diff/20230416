# Comparing `tmp/leopards-0.9.1.tar.gz` & `tmp/leopards-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/leopards-0.9.1.tar", last modified: Tue Nov 15 13:58:57 2022, max compression
+gzip compressed data, was "dist/leopards-0.9.2.tar", last modified: Tue Nov 15 14:00:37 2022, max compression
```

## Comparing `leopards-0.9.1.tar` & `leopards-0.9.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-11-15 13:58:57.000000 leopards-0.9.1/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1075 2022-11-15 10:39:53.000000 leopards-0.9.1/LICENSE
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6342 2022-11-15 13:58:57.000000 leopards-0.9.1/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4430 2022-11-15 13:56:46.000000 leopards-0.9.1/README.md
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-11-15 13:58:57.000000 leopards-0.9.1/leopards/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1749 2022-11-15 10:39:53.000000 leopards-0.9.1/leopards/Q.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1619 2022-11-15 10:39:53.000000 leopards-0.9.1/leopards/Query.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       20 2022-11-15 10:39:53.000000 leopards-0.9.1/leopards/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4593 2022-11-15 10:39:53.000000 leopards-0.9.1/leopards/test.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    13306 2022-11-15 10:39:53.000000 leopards-0.9.1/leopards/test_file.py
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-11-15 13:58:57.000000 leopards-0.9.1/leopards.egg-info/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6342 2022-11-15 13:58:57.000000 leopards-0.9.1/leopards.egg-info/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      277 2022-11-15 13:58:57.000000 leopards-0.9.1/leopards.egg-info/SOURCES.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2022-11-15 13:58:57.000000 leopards-0.9.1/leopards.egg-info/dependency_links.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2022-11-15 13:50:44.000000 leopards-0.9.1/leopards.egg-info/not-zip-safe
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        9 2022-11-15 13:58:57.000000 leopards-0.9.1/leopards.egg-info/top_level.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2022-11-15 13:58:57.000000 leopards-0.9.1/setup.cfg
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1296 2022-11-15 13:58:38.000000 leopards-0.9.1/setup.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-11-15 14:00:37.000000 leopards-0.9.2/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1075 2022-11-15 10:39:53.000000 leopards-0.9.2/LICENSE
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6354 2022-11-15 14:00:37.000000 leopards-0.9.2/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4442 2022-11-15 13:59:55.000000 leopards-0.9.2/README.md
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-11-15 14:00:37.000000 leopards-0.9.2/leopards/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1749 2022-11-15 10:39:53.000000 leopards-0.9.2/leopards/Q.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1619 2022-11-15 10:39:53.000000 leopards-0.9.2/leopards/Query.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       20 2022-11-15 10:39:53.000000 leopards-0.9.2/leopards/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4593 2022-11-15 10:39:53.000000 leopards-0.9.2/leopards/test.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)    13306 2022-11-15 10:39:53.000000 leopards-0.9.2/leopards/test_file.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2022-11-15 14:00:37.000000 leopards-0.9.2/leopards.egg-info/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6354 2022-11-15 14:00:37.000000 leopards-0.9.2/leopards.egg-info/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      277 2022-11-15 14:00:37.000000 leopards-0.9.2/leopards.egg-info/SOURCES.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2022-11-15 14:00:37.000000 leopards-0.9.2/leopards.egg-info/dependency_links.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2022-11-15 13:50:44.000000 leopards-0.9.2/leopards.egg-info/not-zip-safe
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        9 2022-11-15 14:00:37.000000 leopards-0.9.2/leopards.egg-info/top_level.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2022-11-15 14:00:37.000000 leopards-0.9.2/setup.cfg
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1296 2022-11-15 14:00:34.000000 leopards-0.9.2/setup.py
```

### Comparing `leopards-0.9.1/LICENSE` & `leopards-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `leopards-0.9.1/PKG-INFO` & `leopards-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leopards
-Version: 0.9.1
+Version: 0.9.2
 Summary: Allows filtering  iterable of dictionary by another dictionary. Much faster than pandas
 Home-page: https://github.com/mkalioby/leopards/
 Author: Mohamed El-Kalioby
 Author-email: mkalioby@mkalioby.com
 License: MIT
 Download-URL: https://github.com/mkalioby/leopards/
 Description: # Leopards
@@ -115,25 +115,25 @@
         [{'name': 'John', 'age': '16'}, {'name': 'Mike', 'age': '19'}]
         ```
         
         ## Comparison with Pandas
         
         This is done on Python 3.8 running on Ubuntu 22.04 on i7 11th generation and 32 GB of RAM.
         
-        | Comparison                                                  | Pandas   | QyPy    |
-        |-------------------------------------------------------------|----------|---------|
-        | Package Size     <br/> (Lower is better)                    | 29.8 MB  | 7.5 KB  |
-        | import Time (Worst) <br/> (Lower is better)                 | 146 ms   | 1.05 ms |
-        | load 10k CSV lines<br/> (Lower is better) <sup>[1]</sup>    | 0.295s   | 0.138s  |
-        | get first matched record<br/> (Lower is better)             | 0.310s   | 0.017s  |
-        | print all filtered records (10/10k) <br/> (Lower is better) | 0.310s   | 0.137s  | 
-        | filter by integers <br/>(Lower is better)                   | 0.316s   | 0.138s  |
+        | Comparison                                                  | Pandas   | Leopards |
+        |-------------------------------------------------------------|----------|----------|
+        | Package Size     <br/> (Lower is better)                    | 29.8 MB  | 7.5 KB   |
+        | import Time (Worst) <br/> (Lower is better)                 | 146 ms   | 1.05 ms  |
+        | load 10k CSV lines<br/> (Lower is better) <sup>[1]</sup>    | 0.295s   | 0.138s   |
+        | get first matched record<br/> (Lower is better)             | 0.310s   | 0.017s   |
+        | print all filtered records (10/10k) <br/> (Lower is better) | 0.310s   | 0.137s   | 
+        | filter by integers <br/>(Lower is better)                   | 0.316s   | 0.138s   |
         
         <sup>[1]</sup> This was loading the whole csv in memory which was for sake of fair comparison. 
-        Nevertheless,  QyPy can work with DictReader as an iterable which executes in 0.014s, for it handles line by line.
+        Nevertheless,  Leopards can work with DictReader as an iterable which executes in 0.014s, for it handles line by line.
         
         Thanks for [Asma Tahir](https://github.com/tahirasma) for Pandas stats.
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `leopards-0.9.1/README.md` & `leopards-0.9.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -106,20 +106,20 @@
 [{'name': 'John', 'age': '16'}, {'name': 'Mike', 'age': '19'}]
 ```
 
 ## Comparison with Pandas
 
 This is done on Python 3.8 running on Ubuntu 22.04 on i7 11th generation and 32 GB of RAM.
 
-| Comparison                                                  | Pandas   | QyPy    |
-|-------------------------------------------------------------|----------|---------|
-| Package Size     <br/> (Lower is better)                    | 29.8 MB  | 7.5 KB  |
-| import Time (Worst) <br/> (Lower is better)                 | 146 ms   | 1.05 ms |
-| load 10k CSV lines<br/> (Lower is better) <sup>[1]</sup>    | 0.295s   | 0.138s  |
-| get first matched record<br/> (Lower is better)             | 0.310s   | 0.017s  |
-| print all filtered records (10/10k) <br/> (Lower is better) | 0.310s   | 0.137s  | 
-| filter by integers <br/>(Lower is better)                   | 0.316s   | 0.138s  |
+| Comparison                                                  | Pandas   | Leopards |
+|-------------------------------------------------------------|----------|----------|
+| Package Size     <br/> (Lower is better)                    | 29.8 MB  | 7.5 KB   |
+| import Time (Worst) <br/> (Lower is better)                 | 146 ms   | 1.05 ms  |
+| load 10k CSV lines<br/> (Lower is better) <sup>[1]</sup>    | 0.295s   | 0.138s   |
+| get first matched record<br/> (Lower is better)             | 0.310s   | 0.017s   |
+| print all filtered records (10/10k) <br/> (Lower is better) | 0.310s   | 0.137s   | 
+| filter by integers <br/>(Lower is better)                   | 0.316s   | 0.138s   |
 
 <sup>[1]</sup> This was loading the whole csv in memory which was for sake of fair comparison. 
-Nevertheless,  QyPy can work with DictReader as an iterable which executes in 0.014s, for it handles line by line.
+Nevertheless,  Leopards can work with DictReader as an iterable which executes in 0.014s, for it handles line by line.
 
 Thanks for [Asma Tahir](https://github.com/tahirasma) for Pandas stats.
```

### Comparing `leopards-0.9.1/leopards/Q.py` & `leopards-0.9.2/leopards/Q.py`

 * *Files identical despite different names*

### Comparing `leopards-0.9.1/leopards/Query.py` & `leopards-0.9.2/leopards/Query.py`

 * *Files identical despite different names*

### Comparing `leopards-0.9.1/leopards/test.py` & `leopards-0.9.2/leopards/test.py`

 * *Files identical despite different names*

### Comparing `leopards-0.9.1/leopards/test_file.py` & `leopards-0.9.2/leopards/test_file.py`

 * *Files identical despite different names*

### Comparing `leopards-0.9.1/leopards.egg-info/PKG-INFO` & `leopards-0.9.2/leopards.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leopards
-Version: 0.9.1
+Version: 0.9.2
 Summary: Allows filtering  iterable of dictionary by another dictionary. Much faster than pandas
 Home-page: https://github.com/mkalioby/leopards/
 Author: Mohamed El-Kalioby
 Author-email: mkalioby@mkalioby.com
 License: MIT
 Download-URL: https://github.com/mkalioby/leopards/
 Description: # Leopards
@@ -115,25 +115,25 @@
         [{'name': 'John', 'age': '16'}, {'name': 'Mike', 'age': '19'}]
         ```
         
         ## Comparison with Pandas
         
         This is done on Python 3.8 running on Ubuntu 22.04 on i7 11th generation and 32 GB of RAM.
         
-        | Comparison                                                  | Pandas   | QyPy    |
-        |-------------------------------------------------------------|----------|---------|
-        | Package Size     <br/> (Lower is better)                    | 29.8 MB  | 7.5 KB  |
-        | import Time (Worst) <br/> (Lower is better)                 | 146 ms   | 1.05 ms |
-        | load 10k CSV lines<br/> (Lower is better) <sup>[1]</sup>    | 0.295s   | 0.138s  |
-        | get first matched record<br/> (Lower is better)             | 0.310s   | 0.017s  |
-        | print all filtered records (10/10k) <br/> (Lower is better) | 0.310s   | 0.137s  | 
-        | filter by integers <br/>(Lower is better)                   | 0.316s   | 0.138s  |
+        | Comparison                                                  | Pandas   | Leopards |
+        |-------------------------------------------------------------|----------|----------|
+        | Package Size     <br/> (Lower is better)                    | 29.8 MB  | 7.5 KB   |
+        | import Time (Worst) <br/> (Lower is better)                 | 146 ms   | 1.05 ms  |
+        | load 10k CSV lines<br/> (Lower is better) <sup>[1]</sup>    | 0.295s   | 0.138s   |
+        | get first matched record<br/> (Lower is better)             | 0.310s   | 0.017s   |
+        | print all filtered records (10/10k) <br/> (Lower is better) | 0.310s   | 0.137s   | 
+        | filter by integers <br/>(Lower is better)                   | 0.316s   | 0.138s   |
         
         <sup>[1]</sup> This was loading the whole csv in memory which was for sake of fair comparison. 
-        Nevertheless,  QyPy can work with DictReader as an iterable which executes in 0.014s, for it handles line by line.
+        Nevertheless,  Leopards can work with DictReader as an iterable which executes in 0.014s, for it handles line by line.
         
         Thanks for [Asma Tahir](https://github.com/tahirasma) for Pandas stats.
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `leopards-0.9.1/setup.py` & `leopards-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='leopards',
-    version='0.9.1',
+    version='0.9.2',
     description='Allows filtering  iterable of dictionary by another dictionary. Much faster than pandas',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     #long_description="Filters List of Dictionaries by a query dictionary",
     author='Mohamed El-Kalioby',
     author_email = 'mkalioby@mkalioby.com',
     url = 'https://github.com/mkalioby/leopards/',
```

