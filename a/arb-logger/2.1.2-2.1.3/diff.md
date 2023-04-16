# Comparing `tmp/arb_logger-2.1.2.tar.gz` & `tmp/arb_logger-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arb_logger-2.1.2.tar", last modified: Wed Apr 12 13:09:19 2023, max compression
+gzip compressed data, was "arb_logger-2.1.3.tar", last modified: Sun Apr 16 08:55:05 2023, max compression
```

## Comparing `arb_logger-2.1.2.tar` & `arb_logger-2.1.3.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 jack       (501) staff       (20)        0 2023-04-12 13:09:19.924234 arb_logger-2.1.2/
--rw-r--r--   0 jack       (501) staff       (20)     3997 2023-04-12 13:09:19.924085 arb_logger-2.1.2/PKG-INFO
--rw-r--r--   0 jack       (501) staff       (20)     3748 2023-04-02 10:52:02.000000 arb_logger-2.1.2/README.md
-drwxr-xr-x   0 jack       (501) staff       (20)        0 2023-04-12 13:09:19.923538 arb_logger-2.1.2/arb_logger.egg-info/
--rw-r--r--   0 jack       (501) staff       (20)     3997 2023-04-12 13:09:19.000000 arb_logger-2.1.2/arb_logger.egg-info/PKG-INFO
--rw-r--r--   0 jack       (501) staff       (20)      245 2023-04-12 13:09:19.000000 arb_logger-2.1.2/arb_logger.egg-info/SOURCES.txt
--rw-r--r--   0 jack       (501) staff       (20)        1 2023-04-12 13:09:19.000000 arb_logger-2.1.2/arb_logger.egg-info/dependency_links.txt
--rw-r--r--   0 jack       (501) staff       (20)       58 2023-04-12 13:09:19.000000 arb_logger-2.1.2/arb_logger.egg-info/entry_points.txt
--rw-r--r--   0 jack       (501) staff       (20)       23 2023-04-12 13:09:19.000000 arb_logger-2.1.2/arb_logger.egg-info/requires.txt
--rw-r--r--   0 jack       (501) staff       (20)        1 2023-04-12 13:09:19.000000 arb_logger-2.1.2/arb_logger.egg-info/top_level.txt
--rw-r--r--   0 jack       (501) staff       (20)       38 2023-04-12 13:09:19.924290 arb_logger-2.1.2/setup.cfg
--rw-r--r--   0 jack       (501) staff       (20)      577 2023-04-12 13:08:32.000000 arb_logger-2.1.2/setup.py
-drwxr-xr-x   0 jack       (501) staff       (20)        0 2023-04-12 13:09:19.923675 arb_logger-2.1.2/tests/
--rw-r--r--   0 jack       (501) staff       (20)     5190 2023-04-01 10:33:30.000000 arb_logger-2.1.2/tests/test_logger.py
+drwxr-xr-x   0 acid3croco   (501) staff       (20)        0 2023-04-16 08:55:05.692069 arb_logger-2.1.3/
+-rw-r--r--   0 acid3croco   (501) staff       (20)     3997 2023-04-16 08:55:05.691510 arb_logger-2.1.3/PKG-INFO
+-rw-r--r--   0 acid3croco   (501) staff       (20)     3748 2023-04-13 14:43:15.000000 arb_logger-2.1.3/README.md
+drwxr-xr-x   0 acid3croco   (501) staff       (20)        0 2023-04-16 08:55:05.688125 arb_logger-2.1.3/arb_logger/
+-rw-r--r--   0 acid3croco   (501) staff       (20)        0 2023-04-16 08:53:23.000000 arb_logger-2.1.3/arb_logger/__init__.py
+-rw-r--r--   0 acid3croco   (501) staff       (20)     2040 2023-04-13 14:43:15.000000 arb_logger-2.1.3/arb_logger/alert_message.py
+-rw-r--r--   0 acid3croco   (501) staff       (20)     2694 2023-04-13 14:43:15.000000 arb_logger-2.1.3/arb_logger/arb_alerts.py
+-rw-r--r--   0 acid3croco   (501) staff       (20)     4853 2023-04-13 14:43:15.000000 arb_logger-2.1.3/arb_logger/logger.py
+drwxr-xr-x   0 acid3croco   (501) staff       (20)        0 2023-04-16 08:55:05.690816 arb_logger-2.1.3/arb_logger.egg-info/
+-rw-r--r--   0 acid3croco   (501) staff       (20)     3997 2023-04-16 08:55:05.000000 arb_logger-2.1.3/arb_logger.egg-info/PKG-INFO
+-rw-r--r--   0 acid3croco   (501) staff       (20)      321 2023-04-16 08:55:05.000000 arb_logger-2.1.3/arb_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 acid3croco   (501) staff       (20)        1 2023-04-16 08:55:05.000000 arb_logger-2.1.3/arb_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 acid3croco   (501) staff       (20)       58 2023-04-16 08:55:05.000000 arb_logger-2.1.3/arb_logger.egg-info/entry_points.txt
+-rw-r--r--   0 acid3croco   (501) staff       (20)       23 2023-04-16 08:55:05.000000 arb_logger-2.1.3/arb_logger.egg-info/requires.txt
+-rw-r--r--   0 acid3croco   (501) staff       (20)       11 2023-04-16 08:55:05.000000 arb_logger-2.1.3/arb_logger.egg-info/top_level.txt
+-rw-r--r--   0 acid3croco   (501) staff       (20)       38 2023-04-16 08:55:05.692242 arb_logger-2.1.3/setup.cfg
+-rw-r--r--   0 acid3croco   (501) staff       (20)      577 2023-04-16 08:53:35.000000 arb_logger-2.1.3/setup.py
```

### Comparing `arb_logger-2.1.2/PKG-INFO` & `arb_logger-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arb_logger
-Version: 2.1.2
+Version: 2.1.3
 Summary: A custom logger with Redis integration
 Home-page: https://github.com/Acid3croco/arb-trops-services
 Author: arb
 Author-email: arb.trops@gmail.com
 Description-Content-Type: text/markdown
 
 # arb_logger
```

### Comparing `arb_logger-2.1.2/README.md` & `arb_logger-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `arb_logger-2.1.2/arb_logger.egg-info/PKG-INFO` & `arb_logger-2.1.3/arb_logger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arb-logger
-Version: 2.1.2
+Version: 2.1.3
 Summary: A custom logger with Redis integration
 Home-page: https://github.com/Acid3croco/arb-trops-services
 Author: arb
 Author-email: arb.trops@gmail.com
 Description-Content-Type: text/markdown
 
 # arb_logger
```

### Comparing `arb_logger-2.1.2/setup.py` & `arb_logger-2.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     name='arb_logger',
     author='arb',
     author_email='arb.trops@gmail.com',
     description="A custom logger with Redis integration",
     url="https://github.com/Acid3croco/arb-trops-services",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    version='2.1.2',
+    version='2.1.3',
     packages=find_packages(),
     install_requires=['coloredlogs', 'redis', 'pync'],
     entry_points={
         'console_scripts': [
             'arb_alerts = arb_logger.arb_alerts:main',
         ]
     },
```

