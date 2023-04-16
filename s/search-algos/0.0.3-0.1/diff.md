# Comparing `tmp/search-algos-0.0.3.tar.gz` & `tmp/search-algos-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "search-algos-0.0.3.tar", last modified: Sun Apr 16 15:55:00 2023, max compression
+gzip compressed data, was "search-algos-0.1.tar", last modified: Sat Apr 15 19:10:30 2023, max compression
```

## Comparing `search-algos-0.0.3.tar` & `search-algos-0.1.tar`

### file list

```diff
@@ -1,19 +1,12 @@
-drwxr-xr-x   0 arpanadhikari   (501) staff       (20)        0 2023-04-16 15:55:00.647602 search-algos-0.0.3/
--rw-r--r--   0 arpanadhikari   (501) staff       (20)     1387 2023-04-16 15:55:00.647165 search-algos-0.0.3/PKG-INFO
--rw-r--r--   0 arpanadhikari   (501) staff       (20)     1119 2023-04-16 07:34:32.000000 search-algos-0.0.3/README.md
-drwxr-xr-x   0 arpanadhikari   (501) staff       (20)        0 2023-04-16 15:55:00.628757 search-algos-0.0.3/search_algos/
--rw-r--r--   0 arpanadhikari   (501) staff       (20)      459 2023-04-16 07:22:03.000000 search-algos-0.0.3/search_algos/__init__.py
--rw-r--r--   0 arpanadhikari   (501) staff       (20)      290 2023-04-16 07:15:47.000000 search-algos-0.0.3/search_algos/binary_search.py
--rw-r--r--   0 arpanadhikari   (501) staff       (20)      266 2023-04-16 15:54:26.000000 search-algos-0.0.3/search_algos/exponential_search.py
--rw-r--r--   0 arpanadhikari   (501) staff       (20)      634 2023-04-16 07:20:54.000000 search-algos-0.0.3/search_algos/fibonacci_search.py
--rw-r--r--   0 arpanadhikari   (501) staff       (20)      384 2023-04-16 07:17:18.000000 search-algos-0.0.3/search_algos/interpolation_search.py
--rw-r--r--   0 arpanadhikari   (501) staff       (20)      386 2023-04-16 07:18:22.000000 search-algos-0.0.3/search_algos/jump_search.py
--rw-r--r--   0 arpanadhikari   (501) staff       (20)      121 2023-04-15 19:09:12.000000 search-algos-0.0.3/search_algos/linear_search.py
--rw-r--r--   0 arpanadhikari   (501) staff       (20)      503 2023-04-16 07:21:43.000000 search-algos-0.0.3/search_algos/ternary_search.py
-drwxr-xr-x   0 arpanadhikari   (501) staff       (20)        0 2023-04-16 15:55:00.645573 search-algos-0.0.3/search_algos.egg-info/
--rw-r--r--   0 arpanadhikari   (501) staff       (20)     1387 2023-04-16 15:54:59.000000 search-algos-0.0.3/search_algos.egg-info/PKG-INFO
--rw-r--r--   0 arpanadhikari   (501) staff       (20)      411 2023-04-16 15:55:00.000000 search-algos-0.0.3/search_algos.egg-info/SOURCES.txt
--rw-r--r--   0 arpanadhikari   (501) staff       (20)        1 2023-04-16 15:54:59.000000 search-algos-0.0.3/search_algos.egg-info/dependency_links.txt
--rw-r--r--   0 arpanadhikari   (501) staff       (20)       13 2023-04-16 15:55:00.000000 search-algos-0.0.3/search_algos.egg-info/top_level.txt
--rw-r--r--   0 arpanadhikari   (501) staff       (20)       38 2023-04-16 15:55:00.651786 search-algos-0.0.3/setup.cfg
--rw-r--r--   0 arpanadhikari   (501) staff       (20)      442 2023-04-16 15:54:51.000000 search-algos-0.0.3/setup.py
+drwxr-xr-x   0 arpanadhikari   (501) staff       (20)        0 2023-04-15 19:10:30.796857 search-algos-0.1/
+-rw-r--r--   0 arpanadhikari   (501) staff       (20)      233 2023-04-15 19:10:30.793833 search-algos-0.1/PKG-INFO
+drwxr-xr-x   0 arpanadhikari   (501) staff       (20)        0 2023-04-15 19:10:30.764984 search-algos-0.1/algos/
+-rw-r--r--   0 arpanadhikari   (501) staff       (20)       69 2023-04-15 19:09:48.000000 search-algos-0.1/algos/__init__.py
+-rw-r--r--   0 arpanadhikari   (501) staff       (20)      121 2023-04-15 19:09:12.000000 search-algos-0.1/algos/linear_search.py
+drwxr-xr-x   0 arpanadhikari   (501) staff       (20)        0 2023-04-15 19:10:30.785784 search-algos-0.1/search_algos.egg-info/
+-rw-r--r--   0 arpanadhikari   (501) staff       (20)      233 2023-04-15 19:10:29.000000 search-algos-0.1/search_algos.egg-info/PKG-INFO
+-rw-r--r--   0 arpanadhikari   (501) staff       (20)      193 2023-04-15 19:10:30.000000 search-algos-0.1/search_algos.egg-info/SOURCES.txt
+-rw-r--r--   0 arpanadhikari   (501) staff       (20)        1 2023-04-15 19:10:30.000000 search-algos-0.1/search_algos.egg-info/dependency_links.txt
+-rw-r--r--   0 arpanadhikari   (501) staff       (20)        6 2023-04-15 19:10:30.000000 search-algos-0.1/search_algos.egg-info/top_level.txt
+-rw-r--r--   0 arpanadhikari   (501) staff       (20)       38 2023-04-15 19:10:30.801192 search-algos-0.1/setup.cfg
+-rw-r--r--   0 arpanadhikari   (501) staff       (20)      283 2023-04-15 19:06:27.000000 search-algos-0.1/setup.py
```

