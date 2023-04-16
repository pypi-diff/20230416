# Comparing `tmp/netin-1.0.3.tar.gz` & `tmp/netin-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netin-1.0.3.tar", last modified: Sun Apr 16 07:06:05 2023, max compression
+gzip compressed data, was "netin-1.0.4.tar", last modified: Sun Apr 16 07:36:19 2023, max compression
```

## Comparing `netin-1.0.3.tar` & `netin-1.0.4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.160397 netin-1.0.3/
--rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.3/LICENSE
--rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.3/MANIFEST.in
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3648 2023-04-16 07:06:05.160397 netin-1.0.3/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2397 2023-04-16 06:45:05.000000 netin-1.0.3/README.rst
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.156397 netin-1.0.3/examples/
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.156397 netin-1.0.3/examples/directed/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.3/examples/directed/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.3/examples/directed/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.3/examples/directed/dpah.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.156397 netin-1.0.3/examples/undirected/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.3/examples/undirected/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.3/examples/undirected/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.3/examples/undirected/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.3/examples/undirected/patch.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.156397 netin-1.0.3/netin/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      351 2023-04-16 07:06:00.000000 netin-1.0.3/netin/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.156397 netin-1.0.3/netin/algorithms/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-06 13:44:46.000000 netin-1.0.3/netin/algorithms/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.156397 netin-1.0.3/netin/generators/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-14 21:19:23.000000 netin-1.0.3/netin/generators/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4078 2023-04-15 01:01:03.000000 netin-1.0.3/netin/generators/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     9214 2023-04-15 22:08:19.000000 netin-1.0.3/netin/generators/directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2385 2023-04-14 21:16:14.000000 netin-1.0.3/netin/generators/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3448 2023-04-15 21:55:31.000000 netin-1.0.3/netin/generators/dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    13362 2023-04-15 21:45:47.000000 netin-1.0.3/netin/generators/graph.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6332 2023-04-15 18:01:34.000000 netin-1.0.3/netin/generators/h.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1948 2023-04-14 21:16:41.000000 netin-1.0.3/netin/generators/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4363 2023-04-16 07:05:49.000000 netin-1.0.3/netin/generators/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3587 2023-04-14 21:16:55.000000 netin-1.0.3/netin/generators/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3951 2023-04-15 22:08:18.000000 netin-1.0.3/netin/generators/patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6339 2023-04-14 23:53:00.000000 netin-1.0.3/netin/generators/tc.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.156397 netin-1.0.3/netin/generators/tests/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.3/netin/generators/tests/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.3/netin/generators/tests/test_directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.3/netin/generators/tests/test_dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.3/netin/generators/tests/test_patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.3/netin/generators/tests/test_undirected.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     7000 2023-04-15 22:08:18.000000 netin-1.0.3/netin/generators/undirected.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.156397 netin-1.0.3/netin/stats/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      288 2023-04-15 18:06:03.000000 netin-1.0.3/netin/stats/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1854 2023-04-15 19:33:04.000000 netin-1.0.3/netin/stats/distributions.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2753 2023-04-15 22:08:18.000000 netin-1.0.3/netin/stats/ranking.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.156397 netin-1.0.3/netin/utils/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.3/netin/utils/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1075 2023-04-15 18:01:34.000000 netin-1.0.3/netin/utils/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1221 2023-04-13 15:18:30.000000 netin-1.0.3/netin/utils/validator.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.160397 netin-1.0.3/netin/viz/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      426 2023-04-15 18:04:47.000000 netin-1.0.3/netin/viz/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      421 2023-04-15 19:20:18.000000 netin-1.0.3/netin/viz/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    14275 2023-04-15 22:08:18.000000 netin-1.0.3/netin/viz/handlers.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.156397 netin-1.0.3/netin.egg-info/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3648 2023-04-16 07:06:05.000000 netin-1.0.3/netin.egg-info/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1237 2023-04-16 07:06:05.000000 netin-1.0.3/netin.egg-info/SOURCES.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:06:05.000000 netin-1.0.3/netin.egg-info/dependency_links.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.3/netin.egg-info/not-zip-safe
--rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-16 07:06:05.000000 netin-1.0.3/netin.egg-info/requires.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-16 07:06:05.000000 netin-1.0.3/netin.egg-info/top_level.txt
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.160397 netin-1.0.3/requirements/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.3/requirements/default.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.3/requirements/test.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-16 07:06:05.160397 netin-1.0.3/setup.cfg
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4228 2023-04-16 07:00:24.000000 netin-1.0.3/setup.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:36:19.978709 netin-1.0.4/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.4/LICENSE
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.4/MANIFEST.in
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3631 2023-04-16 07:36:19.978709 netin-1.0.4/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2365 2023-04-16 07:25:54.000000 netin-1.0.4/README.rst
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:36:19.974709 netin-1.0.4/examples/
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:36:19.978709 netin-1.0.4/examples/directed/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.4/examples/directed/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.4/examples/directed/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.4/examples/directed/dpah.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:36:19.978709 netin-1.0.4/examples/undirected/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.4/examples/undirected/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.4/examples/undirected/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.4/examples/undirected/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.4/examples/undirected/patch.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:36:19.978709 netin-1.0.4/netin/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      351 2023-04-16 07:36:15.000000 netin-1.0.4/netin/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:36:19.978709 netin-1.0.4/netin/algorithms/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-06 13:44:46.000000 netin-1.0.4/netin/algorithms/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:36:19.978709 netin-1.0.4/netin/generators/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-14 21:19:23.000000 netin-1.0.4/netin/generators/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4078 2023-04-15 01:01:03.000000 netin-1.0.4/netin/generators/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     9214 2023-04-15 22:08:19.000000 netin-1.0.4/netin/generators/directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2385 2023-04-14 21:16:14.000000 netin-1.0.4/netin/generators/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3448 2023-04-15 21:55:31.000000 netin-1.0.4/netin/generators/dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    13362 2023-04-15 21:45:47.000000 netin-1.0.4/netin/generators/graph.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6332 2023-04-15 18:01:34.000000 netin-1.0.4/netin/generators/h.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1948 2023-04-14 21:16:41.000000 netin-1.0.4/netin/generators/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4363 2023-04-16 07:05:49.000000 netin-1.0.4/netin/generators/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3587 2023-04-14 21:16:55.000000 netin-1.0.4/netin/generators/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3951 2023-04-15 22:08:18.000000 netin-1.0.4/netin/generators/patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6339 2023-04-14 23:53:00.000000 netin-1.0.4/netin/generators/tc.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:36:19.978709 netin-1.0.4/netin/generators/tests/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.4/netin/generators/tests/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.4/netin/generators/tests/test_directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.4/netin/generators/tests/test_dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.4/netin/generators/tests/test_patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.4/netin/generators/tests/test_undirected.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     7000 2023-04-15 22:08:18.000000 netin-1.0.4/netin/generators/undirected.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:36:19.978709 netin-1.0.4/netin/stats/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      288 2023-04-15 18:06:03.000000 netin-1.0.4/netin/stats/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1854 2023-04-15 19:33:04.000000 netin-1.0.4/netin/stats/distributions.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2753 2023-04-15 22:08:18.000000 netin-1.0.4/netin/stats/ranking.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:36:19.978709 netin-1.0.4/netin/utils/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.4/netin/utils/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1075 2023-04-15 18:01:34.000000 netin-1.0.4/netin/utils/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1221 2023-04-13 15:18:30.000000 netin-1.0.4/netin/utils/validator.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:36:19.978709 netin-1.0.4/netin/viz/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      426 2023-04-15 18:04:47.000000 netin-1.0.4/netin/viz/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      421 2023-04-15 19:20:18.000000 netin-1.0.4/netin/viz/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    14275 2023-04-15 22:08:18.000000 netin-1.0.4/netin/viz/handlers.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:36:19.978709 netin-1.0.4/netin.egg-info/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3631 2023-04-16 07:36:19.000000 netin-1.0.4/netin.egg-info/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1237 2023-04-16 07:36:19.000000 netin-1.0.4/netin.egg-info/SOURCES.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:36:19.000000 netin-1.0.4/netin.egg-info/dependency_links.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.4/netin.egg-info/not-zip-safe
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-16 07:36:19.000000 netin-1.0.4/netin.egg-info/requires.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-16 07:36:19.000000 netin-1.0.4/netin.egg-info/top_level.txt
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:36:19.978709 netin-1.0.4/requirements/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.4/requirements/default.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.4/requirements/test.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-16 07:36:19.978709 netin-1.0.4/setup.cfg
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4243 2023-04-16 07:22:10.000000 netin-1.0.4/setup.py
```

### Comparing `netin-1.0.3/LICENSE` & `netin-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/PKG-INFO` & `netin-1.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python package to study inequalities in social networks
-Home-page: https://www.networkinequality.com
+Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
 Platform: Linux
 Platform: Mac OSX
@@ -58,37 +58,36 @@
 Simple examples
 ---------------
 
 Create an undirected network with preferential attachment and homophily.
 
 .. code:: pycon
 
-    >>> from netin as PAH
+    >>> from netin import PAH
     >>> G = PAH(n=200, k=2, f_m=0.2, h_MM=0.1, h_mm=0.9, seed=42)
     >>> G.generate()
+    >>> G.info()
 
 
 Create a directed network with preferential attachment and homophily.
 
 .. code:: pycon
 
     >>> from netin import DPAH
-    >>> G = DPAH(n=200, f_m=0.2, d=0.1, h_MM=0.1, h_mm=0.6, plo_M=2.0, plo_m=2.0, seed=42)
+    >>> G = DPAH(n=200, f_m=0.2, d=0.02, h_MM=0.1, h_mm=0.6, plo_M=2.0, plo_m=2.0, seed=42)
     >>> G.generate()
+    >>> G.info()
 
 Install
 -------
 
 Install the latest version of NetIn::
 
     $ pip install netin
 
-Install with all optional dependencies::
-
-    $ pip install netin[all]
 
 Install from source::
 
         $ git clone
         $ cd NetworkInequalities
         $ pip install -e .
```

### Comparing `netin-1.0.3/README.rst` & `netin-1.0.4/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -26,37 +26,36 @@
 Simple examples
 ---------------
 
 Create an undirected network with preferential attachment and homophily.
 
 .. code:: pycon
 
-    >>> from netin as PAH
+    >>> from netin import PAH
     >>> G = PAH(n=200, k=2, f_m=0.2, h_MM=0.1, h_mm=0.9, seed=42)
     >>> G.generate()
+    >>> G.info()
 
 
 Create a directed network with preferential attachment and homophily.
 
 .. code:: pycon
 
     >>> from netin import DPAH
-    >>> G = DPAH(n=200, f_m=0.2, d=0.1, h_MM=0.1, h_mm=0.6, plo_M=2.0, plo_m=2.0, seed=42)
+    >>> G = DPAH(n=200, f_m=0.2, d=0.02, h_MM=0.1, h_mm=0.6, plo_M=2.0, plo_m=2.0, seed=42)
     >>> G.generate()
+    >>> G.info()
 
 Install
 -------
 
 Install the latest version of NetIn::
 
     $ pip install netin
 
-Install with all optional dependencies::
-
-    $ pip install netin[all]
 
 Install from source::
 
         $ git clone
         $ cd NetworkInequalities
         $ pip install -e .
```

### Comparing `netin-1.0.3/netin/generators/dh.py` & `netin-1.0.4/netin/generators/dh.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin/generators/directed.py` & `netin-1.0.4/netin/generators/directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin/generators/dpa.py` & `netin-1.0.4/netin/generators/dpa.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin/generators/dpah.py` & `netin-1.0.4/netin/generators/dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin/generators/graph.py` & `netin-1.0.4/netin/generators/graph.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin/generators/h.py` & `netin-1.0.4/netin/generators/h.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin/generators/pa.py` & `netin-1.0.4/netin/generators/pa.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin/generators/pah.py` & `netin-1.0.4/netin/generators/pah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin/generators/patc.py` & `netin-1.0.4/netin/generators/patc.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin/generators/patch.py` & `netin-1.0.4/netin/generators/patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin/generators/tc.py` & `netin-1.0.4/netin/generators/tc.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin/generators/tests/test_directed.py` & `netin-1.0.4/netin/generators/tests/test_directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin/generators/tests/test_dpah.py` & `netin-1.0.4/netin/generators/tests/test_dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin/generators/tests/test_patch.py` & `netin-1.0.4/netin/generators/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin/generators/tests/test_undirected.py` & `netin-1.0.4/netin/generators/tests/test_undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin/generators/undirected.py` & `netin-1.0.4/netin/generators/undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin/stats/distributions.py` & `netin-1.0.4/netin/stats/distributions.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin/stats/ranking.py` & `netin-1.0.4/netin/stats/ranking.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin/utils/constants.py` & `netin-1.0.4/netin/utils/constants.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin/utils/validator.py` & `netin-1.0.4/netin/utils/validator.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin/viz/handlers.py` & `netin-1.0.4/netin/viz/handlers.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/netin.egg-info/PKG-INFO` & `netin-1.0.4/netin.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python package to study inequalities in social networks
-Home-page: https://www.networkinequality.com
+Home-page: https://github.com/CSHVienna/NetworkInequalities
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
 Platform: Linux
 Platform: Mac OSX
@@ -58,37 +58,36 @@
 Simple examples
 ---------------
 
 Create an undirected network with preferential attachment and homophily.
 
 .. code:: pycon
 
-    >>> from netin as PAH
+    >>> from netin import PAH
     >>> G = PAH(n=200, k=2, f_m=0.2, h_MM=0.1, h_mm=0.9, seed=42)
     >>> G.generate()
+    >>> G.info()
 
 
 Create a directed network with preferential attachment and homophily.
 
 .. code:: pycon
 
     >>> from netin import DPAH
-    >>> G = DPAH(n=200, f_m=0.2, d=0.1, h_MM=0.1, h_mm=0.6, plo_M=2.0, plo_m=2.0, seed=42)
+    >>> G = DPAH(n=200, f_m=0.2, d=0.02, h_MM=0.1, h_mm=0.6, plo_M=2.0, plo_m=2.0, seed=42)
     >>> G.generate()
+    >>> G.info()
 
 Install
 -------
 
 Install the latest version of NetIn::
 
     $ pip install netin
 
-Install with all optional dependencies::
-
-    $ pip install netin[all]
 
 Install from source::
 
         $ git clone
         $ cd NetworkInequalities
         $ pip install -e .
```

### Comparing `netin-1.0.3/netin.egg-info/SOURCES.txt` & `netin-1.0.4/netin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netin-1.0.3/setup.py` & `netin-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 authors = {
     "Karimi": ("Fariba Karimi", "karimi@csh.ac.at"),
     "Espín-Noboa": ("Lisette Espín-Noboa", "espin@csh.ac.at"),
     "Bachmann": ("Jan Bachmann", "bachmann@csh.ac.at"),
 }
 maintainer = "NetIn Developers"
 maintainer_email = "netin@googlegroups.com"
-url = "https://www.networkinequality.com"
+url = "https://github.com/CSHVienna/NetworkInequalities"
 platforms = ["Linux", "Mac OSX", "Windows", "Unix"]
 keywords = [
     "Networks",
     "Inequalities",
     "Social Networks",
     "Ranking",
     "Inference"
```

