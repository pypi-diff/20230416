# Comparing `tmp/randgenlib-1.0.2.tar.gz` & `tmp/randgenlib-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "randgenlib-1.0.2.tar", last modified: Fri Apr 14 21:50:17 2023, max compression
+gzip compressed data, was "randgenlib-1.0.3.tar", last modified: Sun Apr 16 12:24:33 2023, max compression
```

## Comparing `randgenlib-1.0.2.tar` & `randgenlib-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:50:17.749609 randgenlib-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      347 2023-04-14 21:50:17.749609 randgenlib-1.0.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:50:17.749609 randgenlib-1.0.2/randgenlib/
--rw-r--r--   0 root         (0) root         (0)    82161 2023-04-14 21:50:17.000000 randgenlib-1.0.2/randgenlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 21:50:17.749609 randgenlib-1.0.2/randgenlib.egg-info/
--rw-r--r--   0 root         (0) root         (0)      347 2023-04-14 21:50:17.000000 randgenlib-1.0.2/randgenlib.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      167 2023-04-14 21:50:17.000000 randgenlib-1.0.2/randgenlib.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 21:50:17.000000 randgenlib-1.0.2/randgenlib.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-14 21:50:17.000000 randgenlib-1.0.2/randgenlib.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 21:50:17.749609 randgenlib-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      560 2023-04-14 21:50:16.000000 randgenlib-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:24:33.485101 randgenlib-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      325 2023-04-16 12:24:33.485101 randgenlib-1.0.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:24:33.485101 randgenlib-1.0.3/randgenlib/
+-rw-r--r--   0 root         (0) root         (0)   148961 2023-04-16 12:24:32.000000 randgenlib-1.0.3/randgenlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:24:33.485101 randgenlib-1.0.3/randgenlib.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      325 2023-04-16 12:24:33.000000 randgenlib-1.0.3/randgenlib.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      167 2023-04-16 12:24:33.000000 randgenlib-1.0.3/randgenlib.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 12:24:33.000000 randgenlib-1.0.3/randgenlib.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-16 12:24:33.000000 randgenlib-1.0.3/randgenlib.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 12:24:33.485101 randgenlib-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      538 2023-04-16 12:24:32.000000 randgenlib-1.0.3/setup.py
```

