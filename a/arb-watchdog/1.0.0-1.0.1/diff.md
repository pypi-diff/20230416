# Comparing `tmp/arb_watchdog-1.0.0.tar.gz` & `tmp/arb_watchdog-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arb_watchdog-1.0.0.tar", last modified: Sun Apr  2 11:07:31 2023, max compression
+gzip compressed data, was "arb_watchdog-1.0.1.tar", last modified: Sun Apr 16 08:57:16 2023, max compression
```

## Comparing `arb_watchdog-1.0.0.tar` & `arb_watchdog-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 jack       (501) staff       (20)        0 2023-04-02 11:07:31.817201 arb_watchdog-1.0.0/
--rw-r--r--   0 jack       (501) staff       (20)     3818 2023-04-02 11:07:31.817007 arb_watchdog-1.0.0/PKG-INFO
--rw-r--r--   0 jack       (501) staff       (20)     3513 2023-04-02 11:05:45.000000 arb_watchdog-1.0.0/README.md
-drwxr-xr-x   0 jack       (501) staff       (20)        0 2023-04-02 11:07:31.816254 arb_watchdog-1.0.0/arb_watchdog.egg-info/
--rw-r--r--   0 jack       (501) staff       (20)     3818 2023-04-02 11:07:31.000000 arb_watchdog-1.0.0/arb_watchdog.egg-info/PKG-INFO
--rw-r--r--   0 jack       (501) staff       (20)      259 2023-04-02 11:07:31.000000 arb_watchdog-1.0.0/arb_watchdog.egg-info/SOURCES.txt
--rw-r--r--   0 jack       (501) staff       (20)        1 2023-04-02 11:07:31.000000 arb_watchdog-1.0.0/arb_watchdog.egg-info/dependency_links.txt
--rw-r--r--   0 jack       (501) staff       (20)      108 2023-04-02 11:07:31.000000 arb_watchdog-1.0.0/arb_watchdog.egg-info/entry_points.txt
--rw-r--r--   0 jack       (501) staff       (20)       40 2023-04-02 11:07:31.000000 arb_watchdog-1.0.0/arb_watchdog.egg-info/requires.txt
--rw-r--r--   0 jack       (501) staff       (20)        1 2023-04-02 11:07:31.000000 arb_watchdog-1.0.0/arb_watchdog.egg-info/top_level.txt
--rw-r--r--   0 jack       (501) staff       (20)       38 2023-04-02 11:07:31.817258 arb_watchdog-1.0.0/setup.cfg
--rw-r--r--   0 jack       (501) staff       (20)      726 2023-04-02 10:32:24.000000 arb_watchdog-1.0.0/setup.py
-drwxr-xr-x   0 jack       (501) staff       (20)        0 2023-04-02 11:07:31.816381 arb_watchdog-1.0.0/tests/
--rw-r--r--   0 jack       (501) staff       (20)     4125 2023-04-02 10:28:39.000000 arb_watchdog-1.0.0/tests/test_watchdog.py
+drwxr-xr-x   0 acid3croco   (501) staff       (20)        0 2023-04-16 08:57:16.856426 arb_watchdog-1.0.1/
+-rw-r--r--   0 acid3croco   (501) staff       (20)     3818 2023-04-16 08:57:16.856095 arb_watchdog-1.0.1/PKG-INFO
+-rw-r--r--   0 acid3croco   (501) staff       (20)     3513 2023-04-13 14:43:15.000000 arb_watchdog-1.0.1/README.md
+drwxr-xr-x   0 acid3croco   (501) staff       (20)        0 2023-04-16 08:57:16.852707 arb_watchdog-1.0.1/arb_watchdog/
+-rw-r--r--   0 acid3croco   (501) staff       (20)        0 2023-04-16 08:53:26.000000 arb_watchdog-1.0.1/arb_watchdog/__init__.py
+-rw-r--r--   0 acid3croco   (501) staff       (20)     3103 2023-04-13 14:43:15.000000 arb_watchdog-1.0.1/arb_watchdog/cli.py
+-rw-r--r--   0 acid3croco   (501) staff       (20)     2071 2023-04-13 14:43:15.000000 arb_watchdog-1.0.1/arb_watchdog/config.py
+-rw-r--r--   0 acid3croco   (501) staff       (20)      691 2023-04-13 14:43:15.000000 arb_watchdog-1.0.1/arb_watchdog/process_data.py
+-rw-r--r--   0 acid3croco   (501) staff       (20)     4115 2023-04-13 14:43:15.000000 arb_watchdog-1.0.1/arb_watchdog/process_watcher.py
+drwxr-xr-x   0 acid3croco   (501) staff       (20)        0 2023-04-16 08:57:16.855553 arb_watchdog-1.0.1/arb_watchdog.egg-info/
+-rw-r--r--   0 acid3croco   (501) staff       (20)     3818 2023-04-16 08:57:16.000000 arb_watchdog-1.0.1/arb_watchdog.egg-info/PKG-INFO
+-rw-r--r--   0 acid3croco   (501) staff       (20)      365 2023-04-16 08:57:16.000000 arb_watchdog-1.0.1/arb_watchdog.egg-info/SOURCES.txt
+-rw-r--r--   0 acid3croco   (501) staff       (20)        1 2023-04-16 08:57:16.000000 arb_watchdog-1.0.1/arb_watchdog.egg-info/dependency_links.txt
+-rw-r--r--   0 acid3croco   (501) staff       (20)      108 2023-04-16 08:57:16.000000 arb_watchdog-1.0.1/arb_watchdog.egg-info/entry_points.txt
+-rw-r--r--   0 acid3croco   (501) staff       (20)       40 2023-04-16 08:57:16.000000 arb_watchdog-1.0.1/arb_watchdog.egg-info/requires.txt
+-rw-r--r--   0 acid3croco   (501) staff       (20)       13 2023-04-16 08:57:16.000000 arb_watchdog-1.0.1/arb_watchdog.egg-info/top_level.txt
+-rw-r--r--   0 acid3croco   (501) staff       (20)       38 2023-04-16 08:57:16.856518 arb_watchdog-1.0.1/setup.cfg
+-rw-r--r--   0 acid3croco   (501) staff       (20)      726 2023-04-16 08:57:04.000000 arb_watchdog-1.0.1/setup.py
```

### Comparing `arb_watchdog-1.0.0/PKG-INFO` & `arb_watchdog-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arb_watchdog
-Version: 1.0.0
+Version: 1.0.1
 Summary: A process monitoring and alerting tool that keeps an up-to-date status of processes in Redis
 Home-page: https://github.com/Acid3croco/arb-trops-services
 Author: arb
 Author-email: arb.trops@gmail.com
 Description-Content-Type: text/markdown
 
 # arb_watchdog
```

### Comparing `arb_watchdog-1.0.0/README.md` & `arb_watchdog-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `arb_watchdog-1.0.0/arb_watchdog.egg-info/PKG-INFO` & `arb_watchdog-1.0.1/arb_watchdog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arb-watchdog
-Version: 1.0.0
+Version: 1.0.1
 Summary: A process monitoring and alerting tool that keeps an up-to-date status of processes in Redis
 Home-page: https://github.com/Acid3croco/arb-trops-services
 Author: arb
 Author-email: arb.trops@gmail.com
 Description-Content-Type: text/markdown
 
 # arb_watchdog
```

### Comparing `arb_watchdog-1.0.0/setup.py` & `arb_watchdog-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='arb_watchdog',
-    version='1.0.0',
+    version='1.0.1',
     author='arb',
     author_email='arb.trops@gmail.com',
     description=
     'A process monitoring and alerting tool that keeps an up-to-date status of processes in Redis',
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

