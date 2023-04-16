# Comparing `tmp/to-cloud-run-1.0.tar.gz` & `tmp/to-cloud-run-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "to-cloud-run-1.0.tar", last modified: Sun Apr 16 15:14:30 2023, max compression
+gzip compressed data, was "to-cloud-run-1.1.tar", last modified: Sun Apr 16 15:20:25 2023, max compression
```

## Comparing `to-cloud-run-1.0.tar` & `to-cloud-run-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-04-16 15:14:30.044721 to-cloud-run-1.0/
--rw-rw-r--   0 root         (0) root         (0)     2289 2023-04-16 15:14:30.044458 to-cloud-run-1.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2121 2023-04-16 15:14:18.000000 to-cloud-run-1.0/README.md
--rw-rw-r--   0 root         (0) root         (0)       38 2023-04-16 15:14:30.044782 to-cloud-run-1.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      510 2023-04-16 15:14:18.000000 to-cloud-run-1.0/setup.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-04-16 15:14:30.044209 to-cloud-run-1.0/to_cloud_run.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     2289 2023-04-16 15:14:29.000000 to-cloud-run-1.0/to_cloud_run.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      252 2023-04-16 15:14:29.000000 to-cloud-run-1.0/to_cloud_run.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-04-16 15:14:29.000000 to-cloud-run-1.0/to_cloud_run.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       52 2023-04-16 15:14:29.000000 to-cloud-run-1.0/to_cloud_run.egg-info/entry_points.txt
--rw-rw-r--   0 root         (0) root         (0)      103 2023-04-16 15:14:29.000000 to-cloud-run-1.0/to_cloud_run.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       13 2023-04-16 15:14:29.000000 to-cloud-run-1.0/to_cloud_run.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)     2936 2023-04-16 15:14:18.000000 to-cloud-run-1.0/to_cloud_run.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-04-16 15:20:25.721536 to-cloud-run-1.1/
+-rw-rw-r--   0 root         (0) root         (0)     2289 2023-04-16 15:20:25.721269 to-cloud-run-1.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2121 2023-04-16 15:20:19.000000 to-cloud-run-1.1/README.md
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-04-16 15:20:25.721601 to-cloud-run-1.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      510 2023-04-16 15:20:19.000000 to-cloud-run-1.1/setup.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-04-16 15:20:25.721019 to-cloud-run-1.1/to_cloud_run.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     2289 2023-04-16 15:20:24.000000 to-cloud-run-1.1/to_cloud_run.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      252 2023-04-16 15:20:24.000000 to-cloud-run-1.1/to_cloud_run.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-04-16 15:20:24.000000 to-cloud-run-1.1/to_cloud_run.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       52 2023-04-16 15:20:24.000000 to-cloud-run-1.1/to_cloud_run.egg-info/entry_points.txt
+-rw-rw-r--   0 root         (0) root         (0)      103 2023-04-16 15:20:24.000000 to-cloud-run-1.1/to_cloud_run.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       13 2023-04-16 15:20:24.000000 to-cloud-run-1.1/to_cloud_run.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)     2936 2023-04-16 15:20:18.000000 to-cloud-run-1.1/to_cloud_run.py
```

### Comparing `to-cloud-run-1.0/PKG-INFO` & `to-cloud-run-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-cloud-run
-Version: 1.0
+Version: 1.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # to-pip
```

### Comparing `to-cloud-run-1.0/README.md` & `to-cloud-run-1.1/README.md`

 * *Files identical despite different names*

### Comparing `to-cloud-run-1.0/to_cloud_run.egg-info/PKG-INFO` & `to-cloud-run-1.1/to_cloud_run.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: to-cloud-run
-Version: 1.0
+Version: 1.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # to-pip
```

### Comparing `to-cloud-run-1.0/to_cloud_run.py` & `to-cloud-run-1.1/to_cloud_run.py`

 * *Files identical despite different names*

