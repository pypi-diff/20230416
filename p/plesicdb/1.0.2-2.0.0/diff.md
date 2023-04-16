# Comparing `tmp/PlesicDB-1.0.2.tar.gz` & `tmp/plesicdb-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlesicDB-1.0.2.tar", last modified: Wed Oct 13 13:57:03 2021, max compression
+gzip compressed data, was "plesicdb-2.0.0.tar", last modified: Sun Apr 16 13:12:22 2023, max compression
```

## Comparing `PlesicDB-1.0.2.tar` & `plesicdb-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 harkishankhuva  (1000) harkishankhuva  (1000)        0 2021-10-13 13:57:03.957171 PlesicDB-1.0.2/
--rw-rw-r--   0 harkishankhuva  (1000) harkishankhuva  (1000)     1436 2021-10-13 13:57:03.953171 PlesicDB-1.0.2/PKG-INFO
-drwxrwxr-x   0 harkishankhuva  (1000) harkishankhuva  (1000)        0 2021-10-13 13:57:03.949171 PlesicDB-1.0.2/PlesicDB.egg-info/
--rw-rw-r--   0 harkishankhuva  (1000) harkishankhuva  (1000)     1436 2021-10-13 13:57:03.000000 PlesicDB-1.0.2/PlesicDB.egg-info/PKG-INFO
--rw-rw-r--   0 harkishankhuva  (1000) harkishankhuva  (1000)      293 2021-10-13 13:57:03.000000 PlesicDB-1.0.2/PlesicDB.egg-info/SOURCES.txt
--rw-rw-r--   0 harkishankhuva  (1000) harkishankhuva  (1000)        1 2021-10-13 13:57:03.000000 PlesicDB-1.0.2/PlesicDB.egg-info/dependency_links.txt
--rw-rw-r--   0 harkishankhuva  (1000) harkishankhuva  (1000)        9 2021-10-13 13:57:03.000000 PlesicDB-1.0.2/PlesicDB.egg-info/top_level.txt
--rw-rw-r--   0 harkishankhuva  (1000) harkishankhuva  (1000)      820 2021-10-13 13:43:13.000000 PlesicDB-1.0.2/README.md
-drwxrwxr-x   0 harkishankhuva  (1000) harkishankhuva  (1000)        0 2021-10-13 13:57:03.953171 PlesicDB-1.0.2/plesicdb/
--rw-rw-r--   0 harkishankhuva  (1000) harkishankhuva  (1000)      143 2021-10-13 13:51:25.000000 PlesicDB-1.0.2/plesicdb/__about__.py
--rw-rw-r--   0 harkishankhuva  (1000) harkishankhuva  (1000)      923 2021-10-13 13:43:13.000000 PlesicDB-1.0.2/plesicdb/__init__.py
--rw-rw-r--   0 harkishankhuva  (1000) harkishankhuva  (1000)     9022 2021-10-13 13:43:13.000000 PlesicDB-1.0.2/plesicdb/_base.py
--rw-rw-r--   0 harkishankhuva  (1000) harkishankhuva  (1000)    17276 2021-10-13 13:45:55.000000 PlesicDB-1.0.2/plesicdb/_collection.py
--rw-rw-r--   0 harkishankhuva  (1000) harkishankhuva  (1000)     7948 2021-10-13 13:43:13.000000 PlesicDB-1.0.2/plesicdb/_database.py
--rw-rw-r--   0 harkishankhuva  (1000) harkishankhuva  (1000)      136 2021-10-13 13:43:13.000000 PlesicDB-1.0.2/plesicdb/_helpers.py
--rw-rw-r--   0 harkishankhuva  (1000) harkishankhuva  (1000)     1632 2021-10-13 13:43:13.000000 PlesicDB-1.0.2/plesicdb/_utils.py
--rw-rw-r--   0 harkishankhuva  (1000) harkishankhuva  (1000)       38 2021-10-13 13:57:03.957171 PlesicDB-1.0.2/setup.cfg
--rw-rw-r--   0 harkishankhuva  (1000) harkishankhuva  (1000)     1380 2021-10-13 13:51:10.000000 PlesicDB-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:12:22.385693 plesicdb-2.0.0/
+-rw-rw-rw-   0        0        0     1442 2023-04-16 13:12:22.377385 plesicdb-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      926 2023-04-16 13:10:34.000000 plesicdb-2.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 13:12:22.366033 plesicdb-2.0.0/plesicdb/
+-rw-rw-rw-   0        0        0      146 2023-04-16 13:12:00.000000 plesicdb-2.0.0/plesicdb/__about__.py
+-rw-rw-rw-   0        0        0      940 2023-04-16 12:57:20.000000 plesicdb-2.0.0/plesicdb/__init__.py
+-rw-rw-rw-   0        0        0    25279 2023-04-16 12:30:05.000000 plesicdb-2.0.0/plesicdb/core.py
+-rw-rw-rw-   0        0        0     9415 2023-04-16 12:52:17.000000 plesicdb-2.0.0/plesicdb/fields.py
+-rw-rw-rw-   0        0        0     1632 2023-04-16 12:32:24.000000 plesicdb-2.0.0/plesicdb/functions.py
+-rw-rw-rw-   0        0        0     2551 2023-04-16 12:54:10.000000 plesicdb-2.0.0/plesicdb/helpers.py
+-rw-rw-rw-   0        0        0     1015 2023-04-15 17:26:40.000000 plesicdb-2.0.0/plesicdb/lock.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:12:22.375388 plesicdb-2.0.0/plesicdb.egg-info/
+-rw-rw-rw-   0        0        0     1442 2023-04-16 13:12:21.000000 plesicdb-2.0.0/plesicdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-04-16 13:12:21.000000 plesicdb-2.0.0/plesicdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 13:12:21.000000 plesicdb-2.0.0/plesicdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-16 13:12:21.000000 plesicdb-2.0.0/plesicdb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 13:12:22.386705 plesicdb-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      791 2023-04-16 13:11:13.000000 plesicdb-2.0.0/setup.py
```

