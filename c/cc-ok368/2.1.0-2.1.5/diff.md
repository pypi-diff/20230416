# Comparing `tmp/cc-ok368-2.1.0.tar.gz` & `tmp/cc-ok368-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc-ok368-2.1.0.tar", last modified: Thu Feb 23 03:28:45 2023, max compression
+gzip compressed data, was "cc-ok368-2.1.5.tar", last modified: Sun Apr 16 14:47:18 2023, max compression
```

## Comparing `cc-ok368-2.1.0.tar` & `cc-ok368-2.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 namle      (501) staff       (20)        0 2023-02-23 03:28:45.793673 cc-ok368-2.1.0/
--rw-r--r--   0 namle      (501) staff       (20)      264 2023-02-23 03:28:45.793763 cc-ok368-2.1.0/PKG-INFO
--rw-r--r--   0 namle      (501) staff       (20)      111 2023-02-07 10:25:57.000000 cc-ok368-2.1.0/README.md
-drwxr-xr-x   0 namle      (501) staff       (20)        0 2023-02-23 03:28:45.791657 cc-ok368-2.1.0/cc_ok368.egg-info/
--rw-r--r--   0 namle      (501) staff       (20)      264 2023-02-23 03:28:45.000000 cc-ok368-2.1.0/cc_ok368.egg-info/PKG-INFO
--rw-r--r--   0 namle      (501) staff       (20)      243 2023-02-23 03:28:45.000000 cc-ok368-2.1.0/cc_ok368.egg-info/SOURCES.txt
--rw-r--r--   0 namle      (501) staff       (20)        1 2023-02-23 03:28:45.000000 cc-ok368-2.1.0/cc_ok368.egg-info/dependency_links.txt
--rw-r--r--   0 namle      (501) staff       (20)        6 2023-02-23 03:28:45.000000 cc-ok368-2.1.0/cc_ok368.egg-info/top_level.txt
-drwxr-xr-x   0 namle      (501) staff       (20)        0 2023-02-23 03:28:45.793050 cc-ok368-2.1.0/ok368/
--rw-r--r--   0 namle      (501) staff       (20)      112 2023-02-23 03:26:25.000000 cc-ok368-2.1.0/ok368/__init__.py
--rw-r--r--   0 namle      (501) staff       (20)     5629 2023-02-07 10:38:10.000000 cc-ok368-2.1.0/ok368/client.py
--rw-r--r--   0 namle      (501) staff       (20)      148 2023-02-07 10:38:13.000000 cc-ok368-2.1.0/ok368/exceptions.py
--rw-r--r--   0 namle      (501) staff       (20)      168 2023-01-08 16:32:17.000000 cc-ok368-2.1.0/ok368/settings.py
--rw-r--r--   0 namle      (501) staff       (20)       94 2023-02-07 10:25:57.000000 cc-ok368-2.1.0/pyproject.toml
--rw-r--r--   0 namle      (501) staff       (20)      298 2023-02-23 03:28:45.794066 cc-ok368-2.1.0/setup.cfg
--rw-r--r--   0 namle      (501) staff       (20)       53 2023-02-07 10:25:57.000000 cc-ok368-2.1.0/setup.py
+drwxr-xr-x   0 namle      (501) staff       (20)        0 2023-04-16 14:47:18.619800 cc-ok368-2.1.5/
+-rw-r--r--   0 namle      (501) staff       (20)      264 2023-04-16 14:47:18.619884 cc-ok368-2.1.5/PKG-INFO
+-rw-r--r--   0 namle      (501) staff       (20)      111 2023-02-07 10:25:57.000000 cc-ok368-2.1.5/README.md
+drwxr-xr-x   0 namle      (501) staff       (20)        0 2023-04-16 14:47:18.616943 cc-ok368-2.1.5/cc_ok368.egg-info/
+-rw-r--r--   0 namle      (501) staff       (20)      264 2023-04-16 14:47:18.000000 cc-ok368-2.1.5/cc_ok368.egg-info/PKG-INFO
+-rw-r--r--   0 namle      (501) staff       (20)      243 2023-04-16 14:47:18.000000 cc-ok368-2.1.5/cc_ok368.egg-info/SOURCES.txt
+-rw-r--r--   0 namle      (501) staff       (20)        1 2023-04-16 14:47:18.000000 cc-ok368-2.1.5/cc_ok368.egg-info/dependency_links.txt
+-rw-r--r--   0 namle      (501) staff       (20)        6 2023-04-16 14:47:18.000000 cc-ok368-2.1.5/cc_ok368.egg-info/top_level.txt
+drwxr-xr-x   0 namle      (501) staff       (20)        0 2023-04-16 14:47:18.619475 cc-ok368-2.1.5/ok368/
+-rw-r--r--   0 namle      (501) staff       (20)      112 2023-02-23 03:26:25.000000 cc-ok368-2.1.5/ok368/__init__.py
+-rw-r--r--   0 namle      (501) staff       (20)     5629 2023-04-01 04:18:22.000000 cc-ok368-2.1.5/ok368/client.py
+-rw-r--r--   0 namle      (501) staff       (20)      148 2023-02-07 10:38:13.000000 cc-ok368-2.1.5/ok368/exceptions.py
+-rw-r--r--   0 namle      (501) staff       (20)      168 2023-01-08 16:32:17.000000 cc-ok368-2.1.5/ok368/settings.py
+-rw-r--r--   0 namle      (501) staff       (20)       94 2023-02-07 10:25:57.000000 cc-ok368-2.1.5/pyproject.toml
+-rw-r--r--   0 namle      (501) staff       (20)      298 2023-04-16 14:47:18.620518 cc-ok368-2.1.5/setup.cfg
+-rw-r--r--   0 namle      (501) staff       (20)       53 2023-02-07 10:25:57.000000 cc-ok368-2.1.5/setup.py
```

### Comparing `cc-ok368-2.1.0/ok368/client.py` & `cc-ok368-2.1.5/ok368/client.py`

 * *Files identical despite different names*

