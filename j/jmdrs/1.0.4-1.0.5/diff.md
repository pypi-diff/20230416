# Comparing `tmp/jmdrs-1.0.4.tar.gz` & `tmp/jmdrs-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmdrs-1.0.4.tar", last modified: Sun Apr 16 03:23:01 2023, max compression
+gzip compressed data, was "jmdrs-1.0.5.tar", last modified: Sun Apr 16 03:27:11 2023, max compression
```

## Comparing `jmdrs-1.0.4.tar` & `jmdrs-1.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 03:23:01.067528 jmdrs-1.0.4/
--rw-r--r--   0 root         (0) root         (0)       99 2023-04-16 03:23:01.067528 jmdrs-1.0.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 03:23:01.067528 jmdrs-1.0.4/jmdrs.egg-info/
--rw-r--r--   0 root         (0) root         (0)       99 2023-04-16 03:23:00.000000 jmdrs-1.0.4/jmdrs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      152 2023-04-16 03:23:00.000000 jmdrs-1.0.4/jmdrs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 03:23:00.000000 jmdrs-1.0.4/jmdrs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 03:23:00.000000 jmdrs-1.0.4/jmdrs.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 03:23:00.000000 jmdrs-1.0.4/jmdrs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 03:23:01.067528 jmdrs-1.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      658 2023-04-16 03:22:47.000000 jmdrs-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 03:27:11.979177 jmdrs-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-04-16 03:27:11.979177 jmdrs-1.0.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 03:27:11.979177 jmdrs-1.0.5/jmdrs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-04-16 03:27:11.000000 jmdrs-1.0.5/jmdrs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      152 2023-04-16 03:27:11.000000 jmdrs-1.0.5/jmdrs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 03:27:11.000000 jmdrs-1.0.5/jmdrs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 03:27:11.000000 jmdrs-1.0.5/jmdrs.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 03:27:11.000000 jmdrs-1.0.5/jmdrs.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 03:27:11.979177 jmdrs-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      637 2023-04-16 03:26:57.000000 jmdrs-1.0.5/setup.py
```

