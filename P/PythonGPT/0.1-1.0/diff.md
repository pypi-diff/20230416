# Comparing `tmp/PythonGPT-0.1.tar.gz` & `tmp/PythonGPT-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonGPT-0.1.tar", last modified: Sun Apr 16 09:31:20 2023, max compression
+gzip compressed data, was "PythonGPT-1.0.tar", last modified: Sun Apr 16 10:07:41 2023, max compression
```

## Comparing `PythonGPT-0.1.tar` & `PythonGPT-1.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2023-04-16 09:31:20.058151 PythonGPT-0.1/
--rw-rw-r--   0 anon      (1000) anon      (1000)      274 2023-04-16 09:31:20.058151 PythonGPT-0.1/PKG-INFO
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2023-04-16 09:31:20.054151 PythonGPT-0.1/PythonGPT/
--rw-rw-r--   0 anon      (1000) anon      (1000)     2649 2023-04-16 09:28:03.000000 PythonGPT-0.1/PythonGPT/__init__.py
-drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2023-04-16 09:31:20.054151 PythonGPT-0.1/PythonGPT.egg-info/
--rw-rw-r--   0 anon      (1000) anon      (1000)      274 2023-04-16 09:31:19.000000 PythonGPT-0.1/PythonGPT.egg-info/PKG-INFO
--rw-rw-r--   0 anon      (1000) anon      (1000)      194 2023-04-16 09:31:20.000000 PythonGPT-0.1/PythonGPT.egg-info/SOURCES.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)        1 2023-04-16 09:31:19.000000 PythonGPT-0.1/PythonGPT.egg-info/dependency_links.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)        7 2023-04-16 09:31:19.000000 PythonGPT-0.1/PythonGPT.egg-info/requires.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)       10 2023-04-16 09:31:19.000000 PythonGPT-0.1/PythonGPT.egg-info/top_level.txt
--rw-rw-r--   0 anon      (1000) anon      (1000)       38 2023-04-16 09:31:20.058151 PythonGPT-0.1/setup.cfg
--rw-rw-r--   0 anon      (1000) anon      (1000)      340 2023-04-16 09:31:09.000000 PythonGPT-0.1/setup.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2023-04-16 10:07:41.157816 PythonGPT-1.0/
+-rw-rw-r--   0 anon      (1000) anon      (1000)    35149 2023-04-16 09:34:55.000000 PythonGPT-1.0/LICENSE
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1311 2023-04-16 10:07:41.157816 PythonGPT-1.0/PKG-INFO
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2023-04-16 10:07:41.157816 PythonGPT-1.0/PythonGPT/
+-rw-rw-r--   0 anon      (1000) anon      (1000)     2649 2023-04-16 09:28:03.000000 PythonGPT-1.0/PythonGPT/__init__.py
+drwxrwxr-x   0 anon      (1000) anon      (1000)        0 2023-04-16 10:07:41.157816 PythonGPT-1.0/PythonGPT.egg-info/
+-rw-rw-r--   0 anon      (1000) anon      (1000)     1311 2023-04-16 10:07:41.000000 PythonGPT-1.0/PythonGPT.egg-info/PKG-INFO
+-rw-rw-r--   0 anon      (1000) anon      (1000)      212 2023-04-16 10:07:41.000000 PythonGPT-1.0/PythonGPT.egg-info/SOURCES.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)        1 2023-04-16 10:07:41.000000 PythonGPT-1.0/PythonGPT.egg-info/dependency_links.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)        7 2023-04-16 10:07:41.000000 PythonGPT-1.0/PythonGPT.egg-info/requires.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)       10 2023-04-16 10:07:41.000000 PythonGPT-1.0/PythonGPT.egg-info/top_level.txt
+-rw-rw-r--   0 anon      (1000) anon      (1000)      981 2023-04-16 09:59:59.000000 PythonGPT-1.0/README.md
+-rw-rw-r--   0 anon      (1000) anon      (1000)       38 2023-04-16 10:07:41.157816 PythonGPT-1.0/setup.cfg
+-rw-rw-r--   0 anon      (1000) anon      (1000)      546 2023-04-16 10:07:33.000000 PythonGPT-1.0/setup.py
```

### Comparing `PythonGPT-0.1/PythonGPT/__init__.py` & `PythonGPT-1.0/PythonGPT/__init__.py`

 * *Files identical despite different names*

