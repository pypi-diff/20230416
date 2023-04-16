# Comparing `tmp/merkl-0.4.tar.gz` & `tmp/merkl-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merkl-0.4.tar", last modified: Wed Dec  7 19:16:56 2022, max compression
+gzip compressed data, was "merkl-0.5.tar", last modified: Sun Apr 16 13:46:53 2023, max compression
```

## Comparing `merkl-0.4.tar` & `merkl-0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 marpett   (1000) marpett   (1000)        0 2022-12-07 19:16:56.834754 merkl-0.4/
--rw-rw-r--   0 marpett   (1000) marpett   (1000)       25 2022-12-04 09:24:58.000000 merkl-0.4/MANIFEST.in
--rw-rw-r--   0 marpett   (1000) marpett   (1000)    10432 2022-12-07 19:16:56.834754 merkl-0.4/PKG-INFO
--rw-r--r--   0 marpett   (1000) marpett   (1000)    10226 2022-12-04 09:30:44.000000 merkl-0.4/README.md
-drwxrwxr-x   0 marpett   (1000) marpett   (1000)        0 2022-12-07 19:16:56.794755 merkl-0.4/merkl/
--rw-r--r--   0 marpett   (1000) marpett   (1000)      308 2021-09-14 10:14:34.000000 merkl-0.4/merkl/__init__.py
--rw-r--r--   0 marpett   (1000) marpett   (1000)       62 2021-05-05 17:36:17.000000 merkl-0.4/merkl/__main__.py
--rw-r--r--   0 marpett   (1000) marpett   (1000)    10247 2021-10-08 07:41:32.000000 merkl-0.4/merkl/cache.py
-drwxrwxr-x   0 marpett   (1000) marpett   (1000)        0 2022-12-07 19:16:56.810754 merkl-0.4/merkl/cli/
--rw-r--r--   0 marpett   (1000) marpett   (1000)        0 2021-05-05 17:36:17.000000 merkl-0.4/merkl/cli/__init__.py
--rw-r--r--   0 marpett   (1000) marpett   (1000)      736 2021-09-30 07:17:11.000000 merkl-0.4/merkl/cli/cache.py
--rw-r--r--   0 marpett   (1000) marpett   (1000)     4616 2021-09-28 12:03:28.000000 merkl-0.4/merkl/cli/cli.py
--rw-r--r--   0 marpett   (1000) marpett   (1000)      935 2021-08-01 14:00:36.000000 merkl-0.4/merkl/cli/dot.py
--rw-r--r--   0 marpett   (1000) marpett   (1000)      262 2021-05-05 17:36:17.000000 merkl-0.4/merkl/cli/init.py
--rw-r--r--   0 marpett   (1000) marpett   (1000)      589 2021-09-29 09:06:22.000000 merkl-0.4/merkl/cli/migrate.py
--rw-r--r--   0 marpett   (1000) marpett   (1000)      895 2021-09-09 08:33:33.000000 merkl-0.4/merkl/cli/run.py
--rw-r--r--   0 marpett   (1000) marpett   (1000)     5066 2021-09-06 10:45:10.000000 merkl-0.4/merkl/dot.py
--rw-r--r--   0 marpett   (1000) marpett   (1000)      219 2021-05-12 09:30:22.000000 merkl-0.4/merkl/exceptions.py
--rw-r--r--   0 marpett   (1000) marpett   (1000)    19258 2022-03-03 10:33:11.000000 merkl-0.4/merkl/future.py
--rw-r--r--   0 marpett   (1000) marpett   (1000)     8549 2021-11-29 09:52:52.000000 merkl-0.4/merkl/io.py
--rw-r--r--   0 marpett   (1000) marpett   (1000)      401 2021-05-21 11:20:26.000000 merkl-0.4/merkl/logger.py
--rw-r--r--   0 marpett   (1000) marpett   (1000)    19814 2021-11-01 12:43:49.000000 merkl-0.4/merkl/task.py
-drwxrwxr-x   0 marpett   (1000) marpett   (1000)        0 2022-12-07 19:16:56.822754 merkl-0.4/merkl/tests/
--rw-r--r--   0 marpett   (1000) marpett   (1000)      444 2021-05-05 17:36:17.000000 merkl-0.4/merkl/tests/__init__.py
--rw-r--r--   0 marpett   (1000) marpett   (1000)    13072 2021-10-28 08:42:39.000000 merkl-0.4/merkl/tests/test_cache.py
--rw-r--r--   0 marpett   (1000) marpett   (1000)     5593 2021-10-14 10:35:16.000000 merkl-0.4/merkl/tests/test_io.py
--rw-r--r--   0 marpett   (1000) marpett   (1000)    21532 2022-03-03 10:35:19.000000 merkl-0.4/merkl/tests/test_task.py
--rw-r--r--   0 marpett   (1000) marpett   (1000)      336 2022-02-16 13:39:13.000000 merkl-0.4/merkl/util_tasks.py
--rw-r--r--   0 marpett   (1000) marpett   (1000)     9779 2021-11-01 12:43:47.000000 merkl-0.4/merkl/utils.py
-drwxrwxr-x   0 marpett   (1000) marpett   (1000)        0 2022-12-07 19:16:56.810754 merkl-0.4/merkl.egg-info/
--rw-r--r--   0 marpett   (1000) marpett   (1000)    10432 2022-12-07 19:16:56.000000 merkl-0.4/merkl.egg-info/PKG-INFO
--rw-r--r--   0 marpett   (1000) marpett   (1000)      629 2022-12-07 19:16:56.000000 merkl-0.4/merkl.egg-info/SOURCES.txt
--rw-r--r--   0 marpett   (1000) marpett   (1000)        1 2022-12-07 19:16:56.000000 merkl-0.4/merkl.egg-info/dependency_links.txt
--rw-r--r--   0 marpett   (1000) marpett   (1000)       37 2022-12-07 19:16:56.000000 merkl-0.4/merkl.egg-info/entry_points.txt
--rw-r--r--   0 marpett   (1000) marpett   (1000)       55 2022-12-07 19:16:56.000000 merkl-0.4/merkl.egg-info/requires.txt
--rw-r--r--   0 marpett   (1000) marpett   (1000)        6 2022-12-07 19:16:56.000000 merkl-0.4/merkl.egg-info/top_level.txt
--rw-r--r--   0 marpett   (1000) marpett   (1000)       55 2022-12-07 19:15:55.000000 merkl-0.4/requirements.txt
--rw-rw-r--   0 marpett   (1000) marpett   (1000)       38 2022-12-07 19:16:56.834754 merkl-0.4/setup.cfg
--rw-rw-r--   0 marpett   (1000) marpett   (1000)      854 2022-12-07 19:15:01.000000 merkl-0.4/setup.py
+drwxrwxr-x   0 martindbp  (1000) martindbp  (1000)        0 2023-04-16 13:46:53.574848 merkl-0.5/
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)       25 2023-04-16 13:44:17.000000 merkl-0.5/MANIFEST.in
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)    10432 2023-04-16 13:46:53.574848 merkl-0.5/PKG-INFO
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)    10226 2023-04-16 13:44:17.000000 merkl-0.5/README.md
+drwxrwxr-x   0 martindbp  (1000) martindbp  (1000)        0 2023-04-16 13:46:53.574848 merkl-0.5/merkl/
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)      308 2023-04-16 13:44:17.000000 merkl-0.5/merkl/__init__.py
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)       62 2023-04-16 13:44:17.000000 merkl-0.5/merkl/__main__.py
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)    10247 2023-04-16 13:44:17.000000 merkl-0.5/merkl/cache.py
+drwxrwxr-x   0 martindbp  (1000) martindbp  (1000)        0 2023-04-16 13:46:53.574848 merkl-0.5/merkl/cli/
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)        0 2023-04-16 13:44:17.000000 merkl-0.5/merkl/cli/__init__.py
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)      736 2023-04-16 13:44:17.000000 merkl-0.5/merkl/cli/cache.py
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)     4616 2023-04-16 13:44:17.000000 merkl-0.5/merkl/cli/cli.py
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)      935 2023-04-16 13:44:17.000000 merkl-0.5/merkl/cli/dot.py
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)      262 2023-04-16 13:44:17.000000 merkl-0.5/merkl/cli/init.py
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)      589 2023-04-16 13:44:17.000000 merkl-0.5/merkl/cli/migrate.py
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)      895 2023-04-16 13:44:17.000000 merkl-0.5/merkl/cli/run.py
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)     5066 2023-04-16 13:44:17.000000 merkl-0.5/merkl/dot.py
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)      219 2023-04-16 13:44:17.000000 merkl-0.5/merkl/exceptions.py
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)    19258 2023-04-16 13:44:17.000000 merkl-0.5/merkl/future.py
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)     8549 2023-04-16 13:44:17.000000 merkl-0.5/merkl/io.py
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)      401 2023-04-16 13:44:17.000000 merkl-0.5/merkl/logger.py
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)    19814 2023-04-16 13:44:17.000000 merkl-0.5/merkl/task.py
+drwxrwxr-x   0 martindbp  (1000) martindbp  (1000)        0 2023-04-16 13:46:53.574848 merkl-0.5/merkl/tests/
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)      444 2023-04-16 13:44:17.000000 merkl-0.5/merkl/tests/__init__.py
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)    13072 2023-04-16 13:44:17.000000 merkl-0.5/merkl/tests/test_cache.py
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)     5593 2023-04-16 13:44:17.000000 merkl-0.5/merkl/tests/test_io.py
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)    21532 2023-04-16 13:44:17.000000 merkl-0.5/merkl/tests/test_task.py
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)      336 2023-04-16 13:44:17.000000 merkl-0.5/merkl/util_tasks.py
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)     9779 2023-04-16 13:44:17.000000 merkl-0.5/merkl/utils.py
+drwxrwxr-x   0 martindbp  (1000) martindbp  (1000)        0 2023-04-16 13:46:53.574848 merkl-0.5/merkl.egg-info/
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)    10432 2023-04-16 13:46:53.000000 merkl-0.5/merkl.egg-info/PKG-INFO
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)      629 2023-04-16 13:46:53.000000 merkl-0.5/merkl.egg-info/SOURCES.txt
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)        1 2023-04-16 13:46:53.000000 merkl-0.5/merkl.egg-info/dependency_links.txt
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)       37 2023-04-16 13:46:53.000000 merkl-0.5/merkl.egg-info/entry_points.txt
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)       34 2023-04-16 13:46:53.000000 merkl-0.5/merkl.egg-info/requires.txt
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)        6 2023-04-16 13:46:53.000000 merkl-0.5/merkl.egg-info/top_level.txt
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)       34 2023-04-16 13:45:30.000000 merkl-0.5/requirements.txt
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)       38 2023-04-16 13:46:53.574848 merkl-0.5/setup.cfg
+-rw-rw-r--   0 martindbp  (1000) martindbp  (1000)      854 2023-04-16 13:46:45.000000 merkl-0.5/setup.py
```

### Comparing `merkl-0.4/PKG-INFO` & `merkl-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merkl
-Version: 0.4
+Version: 0.5
 Summary: MerkL
 Home-page: https://github.com/martindbp/merkl
 Author: Martin Pettersson
 Author-email: me@martindbp.com
 Description-Content-Type: text/markdown
 
 # MerkL - ML pipelines in pure Python with great caching
```

### Comparing `merkl-0.4/README.md` & `merkl-0.5/README.md`

 * *Files identical despite different names*

### Comparing `merkl-0.4/merkl/cache.py` & `merkl-0.5/merkl/cache.py`

 * *Files identical despite different names*

### Comparing `merkl-0.4/merkl/cli/cache.py` & `merkl-0.5/merkl/cli/cache.py`

 * *Files identical despite different names*

### Comparing `merkl-0.4/merkl/cli/cli.py` & `merkl-0.5/merkl/cli/cli.py`

 * *Files identical despite different names*

### Comparing `merkl-0.4/merkl/cli/dot.py` & `merkl-0.5/merkl/cli/dot.py`

 * *Files identical despite different names*

### Comparing `merkl-0.4/merkl/cli/migrate.py` & `merkl-0.5/merkl/cli/migrate.py`

 * *Files identical despite different names*

### Comparing `merkl-0.4/merkl/cli/run.py` & `merkl-0.5/merkl/cli/run.py`

 * *Files identical despite different names*

### Comparing `merkl-0.4/merkl/dot.py` & `merkl-0.5/merkl/dot.py`

 * *Files identical despite different names*

### Comparing `merkl-0.4/merkl/future.py` & `merkl-0.5/merkl/future.py`

 * *Files identical despite different names*

### Comparing `merkl-0.4/merkl/io.py` & `merkl-0.5/merkl/io.py`

 * *Files identical despite different names*

### Comparing `merkl-0.4/merkl/task.py` & `merkl-0.5/merkl/task.py`

 * *Files identical despite different names*

### Comparing `merkl-0.4/merkl/tests/test_cache.py` & `merkl-0.5/merkl/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `merkl-0.4/merkl/tests/test_io.py` & `merkl-0.5/merkl/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `merkl-0.4/merkl/tests/test_task.py` & `merkl-0.5/merkl/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `merkl-0.4/merkl/utils.py` & `merkl-0.5/merkl/utils.py`

 * *Files identical despite different names*

### Comparing `merkl-0.4/merkl.egg-info/PKG-INFO` & `merkl-0.5/merkl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merkl
-Version: 0.4
+Version: 0.5
 Summary: MerkL
 Home-page: https://github.com/martindbp/merkl
 Author: Martin Pettersson
 Author-email: me@martindbp.com
 Description-Content-Type: text/markdown
 
 # MerkL - ML pipelines in pure Python with great caching
```

### Comparing `merkl-0.4/merkl.egg-info/SOURCES.txt` & `merkl-0.5/merkl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `merkl-0.4/setup.py` & `merkl-0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 except:
     reqs = [str(ir.requirement) for ir in reqs]
 
 setup(
     name="merkl",
     packages=find_packages(),
     entry_points={"console_scripts": ['merkl = merkl:main']},
-    version="0.4",
+    version="0.5",
     description="MerkL",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Martin Pettersson",
     author_email="me@martindbp.com",
     url="https://github.com/martindbp/merkl",
     install_requires=reqs
```

