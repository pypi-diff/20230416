# Comparing `tmp/vhdx_2_zvol-0.3.tar.gz` & `tmp/vhdx_2_zvol-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vhdx_2_zvol-0.3.tar", last modified: Fri Apr 14 01:01:50 2023, max compression
+gzip compressed data, was "vhdx_2_zvol-0.4.tar", last modified: Sun Apr 16 18:28:07 2023, max compression
```

## Comparing `vhdx_2_zvol-0.3.tar` & `vhdx_2_zvol-0.4.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:01:50.612283 vhdx_2_zvol-0.3/
--rw-r--r--   0 root         (0) root         (0)      209 2023-04-14 01:01:50.612283 vhdx_2_zvol-0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-14 01:01:50.612283 vhdx_2_zvol-0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      280 2023-04-14 01:01:33.000000 vhdx_2_zvol-0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 01:01:50.612283 vhdx_2_zvol-0.3/vhdx_2_zvol.egg-info/
--rw-r--r--   0 root         (0) root         (0)      209 2023-04-14 01:01:50.000000 vhdx_2_zvol-0.3/vhdx_2_zvol.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      186 2023-04-14 01:01:50.000000 vhdx_2_zvol-0.3/vhdx_2_zvol.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 01:01:50.000000 vhdx_2_zvol-0.3/vhdx_2_zvol.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-04-14 01:01:50.000000 vhdx_2_zvol-0.3/vhdx_2_zvol.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 01:01:50.000000 vhdx_2_zvol-0.3/vhdx_2_zvol.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:28:07.807582 vhdx_2_zvol-0.4/
+-rw-r--r--   0 root         (0) root         (0)      209 2023-04-16 18:28:07.807582 vhdx_2_zvol-0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 18:28:07.807582 vhdx_2_zvol-0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      280 2023-04-16 18:28:02.000000 vhdx_2_zvol-0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:28:07.807582 vhdx_2_zvol-0.4/vhdx_2_zvol/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-13 00:22:43.000000 vhdx_2_zvol-0.4/vhdx_2_zvol/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7631 2023-04-14 00:22:46.000000 vhdx_2_zvol-0.4/vhdx_2_zvol/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:28:07.807582 vhdx_2_zvol-0.4/vhdx_2_zvol.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      209 2023-04-16 18:28:07.000000 vhdx_2_zvol-0.4/vhdx_2_zvol.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      230 2023-04-16 18:28:07.000000 vhdx_2_zvol-0.4/vhdx_2_zvol.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 18:28:07.000000 vhdx_2_zvol-0.4/vhdx_2_zvol.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-04-16 18:28:07.000000 vhdx_2_zvol-0.4/vhdx_2_zvol.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-16 18:28:07.000000 vhdx_2_zvol-0.4/vhdx_2_zvol.egg-info/top_level.txt
```

