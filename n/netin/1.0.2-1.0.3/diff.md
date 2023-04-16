# Comparing `tmp/netin-1.0.2.tar.gz` & `tmp/netin-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netin-1.0.2.tar", last modified: Sun Apr 16 07:00:51 2023, max compression
+gzip compressed data, was "netin-1.0.3.tar", last modified: Sun Apr 16 07:06:05 2023, max compression
```

## Comparing `netin-1.0.2.tar` & `netin-1.0.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:00:51.232683 netin-1.0.2/
--rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.2/LICENSE
--rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.2/MANIFEST.in
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3648 2023-04-16 07:00:51.232683 netin-1.0.2/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2397 2023-04-16 06:45:05.000000 netin-1.0.2/README.rst
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:00:51.228683 netin-1.0.2/examples/
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:00:51.228683 netin-1.0.2/examples/directed/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.2/examples/directed/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.2/examples/directed/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.2/examples/directed/dpah.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:00:51.228683 netin-1.0.2/examples/undirected/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.2/examples/undirected/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.2/examples/undirected/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.2/examples/undirected/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.2/examples/undirected/patch.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:00:51.228683 netin-1.0.2/netin/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      351 2023-04-16 07:00:43.000000 netin-1.0.2/netin/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:00:51.228683 netin-1.0.2/netin/algorithms/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-06 13:44:46.000000 netin-1.0.2/netin/algorithms/__init__.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:00:51.228683 netin-1.0.2/netin/generators/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-14 21:19:23.000000 netin-1.0.2/netin/generators/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4078 2023-04-15 01:01:03.000000 netin-1.0.2/netin/generators/dh.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     9214 2023-04-15 22:08:19.000000 netin-1.0.2/netin/generators/directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2385 2023-04-14 21:16:14.000000 netin-1.0.2/netin/generators/dpa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3448 2023-04-15 21:55:31.000000 netin-1.0.2/netin/generators/dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    13362 2023-04-15 21:45:47.000000 netin-1.0.2/netin/generators/graph.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6332 2023-04-15 18:01:34.000000 netin-1.0.2/netin/generators/h.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1948 2023-04-14 21:16:41.000000 netin-1.0.2/netin/generators/pa.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4388 2023-04-15 21:51:05.000000 netin-1.0.2/netin/generators/pah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3587 2023-04-14 21:16:55.000000 netin-1.0.2/netin/generators/patc.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3951 2023-04-15 22:08:18.000000 netin-1.0.2/netin/generators/patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     6339 2023-04-14 23:53:00.000000 netin-1.0.2/netin/generators/tc.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:00:51.232683 netin-1.0.2/netin/generators/tests/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.2/netin/generators/tests/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.2/netin/generators/tests/test_directed.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.2/netin/generators/tests/test_dpah.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.2/netin/generators/tests/test_patch.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.2/netin/generators/tests/test_undirected.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     7000 2023-04-15 22:08:18.000000 netin-1.0.2/netin/generators/undirected.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:00:51.232683 netin-1.0.2/netin/stats/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      288 2023-04-15 18:06:03.000000 netin-1.0.2/netin/stats/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1854 2023-04-15 19:33:04.000000 netin-1.0.2/netin/stats/distributions.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     2753 2023-04-15 22:08:18.000000 netin-1.0.2/netin/stats/ranking.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:00:51.232683 netin-1.0.2/netin/utils/
--rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.2/netin/utils/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1075 2023-04-15 18:01:34.000000 netin-1.0.2/netin/utils/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1221 2023-04-13 15:18:30.000000 netin-1.0.2/netin/utils/validator.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:00:51.232683 netin-1.0.2/netin/viz/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      426 2023-04-15 18:04:47.000000 netin-1.0.2/netin/viz/__init__.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)      421 2023-04-15 19:20:18.000000 netin-1.0.2/netin/viz/constants.py
--rw-r--r--   0 espinl    (1001) espinl    (1001)    14275 2023-04-15 22:08:18.000000 netin-1.0.2/netin/viz/handlers.py
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:00:51.228683 netin-1.0.2/netin.egg-info/
--rw-r--r--   0 espinl    (1001) espinl    (1001)     3648 2023-04-16 07:00:51.000000 netin-1.0.2/netin.egg-info/PKG-INFO
--rw-r--r--   0 espinl    (1001) espinl    (1001)     1237 2023-04-16 07:00:51.000000 netin-1.0.2/netin.egg-info/SOURCES.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.2/netin.egg-info/dependency_links.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.2/netin.egg-info/not-zip-safe
--rw-r--r--   0 espinl    (1001) espinl    (1001)      390 2023-04-16 07:00:51.000000 netin-1.0.2/netin.egg-info/requires.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-16 07:00:51.000000 netin-1.0.2/netin.egg-info/top_level.txt
-drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:00:51.232683 netin-1.0.2/requirements/
--rw-r--r--   0 espinl    (1001) espinl    (1001)      168 2023-04-15 14:37:32.000000 netin-1.0.2/requirements/default.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.2/requirements/test.txt
--rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-16 07:00:51.232683 netin-1.0.2/setup.cfg
--rw-r--r--   0 espinl    (1001) espinl    (1001)     4228 2023-04-16 07:00:24.000000 netin-1.0.2/setup.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.160397 netin-1.0.3/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    20843 2023-04-06 14:10:28.000000 netin-1.0.3/LICENSE
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      457 2023-04-16 06:40:57.000000 netin-1.0.3/MANIFEST.in
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3648 2023-04-16 07:06:05.160397 netin-1.0.3/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2397 2023-04-16 06:45:05.000000 netin-1.0.3/README.rst
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.156397 netin-1.0.3/examples/
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.156397 netin-1.0.3/examples/directed/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      311 2023-04-15 01:00:38.000000 netin-1.0.3/examples/directed/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      258 2023-04-07 18:39:19.000000 netin-1.0.3/examples/directed/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      315 2023-04-15 01:15:07.000000 netin-1.0.3/examples/directed/dpah.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.156397 netin-1.0.3/examples/undirected/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      196 2023-04-07 14:05:50.000000 netin-1.0.3/examples/undirected/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      251 2023-04-14 23:44:49.000000 netin-1.0.3/examples/undirected/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      220 2023-04-14 23:45:47.000000 netin-1.0.3/examples/undirected/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      274 2023-04-07 22:28:52.000000 netin-1.0.3/examples/undirected/patch.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.156397 netin-1.0.3/netin/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      351 2023-04-16 07:06:00.000000 netin-1.0.3/netin/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.156397 netin-1.0.3/netin/algorithms/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-06 13:44:46.000000 netin-1.0.3/netin/algorithms/__init__.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.156397 netin-1.0.3/netin/generators/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      320 2023-04-14 21:19:23.000000 netin-1.0.3/netin/generators/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4078 2023-04-15 01:01:03.000000 netin-1.0.3/netin/generators/dh.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     9214 2023-04-15 22:08:19.000000 netin-1.0.3/netin/generators/directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2385 2023-04-14 21:16:14.000000 netin-1.0.3/netin/generators/dpa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3448 2023-04-15 21:55:31.000000 netin-1.0.3/netin/generators/dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    13362 2023-04-15 21:45:47.000000 netin-1.0.3/netin/generators/graph.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6332 2023-04-15 18:01:34.000000 netin-1.0.3/netin/generators/h.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1948 2023-04-14 21:16:41.000000 netin-1.0.3/netin/generators/pa.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4363 2023-04-16 07:05:49.000000 netin-1.0.3/netin/generators/pah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3587 2023-04-14 21:16:55.000000 netin-1.0.3/netin/generators/patc.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3951 2023-04-15 22:08:18.000000 netin-1.0.3/netin/generators/patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     6339 2023-04-14 23:53:00.000000 netin-1.0.3/netin/generators/tc.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.156397 netin-1.0.3/netin/generators/tests/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-15 10:40:52.000000 netin-1.0.3/netin/generators/tests/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3106 2023-04-14 21:24:51.000000 netin-1.0.3/netin/generators/tests/test_directed.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4122 2023-04-15 01:17:44.000000 netin-1.0.3/netin/generators/tests/test_dpah.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3241 2023-04-15 01:19:15.000000 netin-1.0.3/netin/generators/tests/test_patch.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3895 2023-04-15 01:22:06.000000 netin-1.0.3/netin/generators/tests/test_undirected.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     7000 2023-04-15 22:08:18.000000 netin-1.0.3/netin/generators/undirected.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.156397 netin-1.0.3/netin/stats/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      288 2023-04-15 18:06:03.000000 netin-1.0.3/netin/stats/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1854 2023-04-15 19:33:04.000000 netin-1.0.3/netin/stats/distributions.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     2753 2023-04-15 22:08:18.000000 netin-1.0.3/netin/stats/ranking.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.156397 netin-1.0.3/netin/utils/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        0 2023-04-14 21:38:11.000000 netin-1.0.3/netin/utils/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1075 2023-04-15 18:01:34.000000 netin-1.0.3/netin/utils/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1221 2023-04-13 15:18:30.000000 netin-1.0.3/netin/utils/validator.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.160397 netin-1.0.3/netin/viz/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      426 2023-04-15 18:04:47.000000 netin-1.0.3/netin/viz/__init__.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      421 2023-04-15 19:20:18.000000 netin-1.0.3/netin/viz/constants.py
+-rw-r--r--   0 espinl    (1001) espinl    (1001)    14275 2023-04-15 22:08:18.000000 netin-1.0.3/netin/viz/handlers.py
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.156397 netin-1.0.3/netin.egg-info/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     3648 2023-04-16 07:06:05.000000 netin-1.0.3/netin.egg-info/PKG-INFO
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     1237 2023-04-16 07:06:05.000000 netin-1.0.3/netin.egg-info/SOURCES.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:06:05.000000 netin-1.0.3/netin.egg-info/dependency_links.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        1 2023-04-16 07:00:51.000000 netin-1.0.3/netin.egg-info/not-zip-safe
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      418 2023-04-16 07:06:05.000000 netin-1.0.3/netin.egg-info/requires.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)        6 2023-04-16 07:06:05.000000 netin-1.0.3/netin.egg-info/top_level.txt
+drwxr-xr-x   0 espinl    (1001) espinl    (1001)        0 2023-04-16 07:06:05.160397 netin-1.0.3/requirements/
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      182 2023-04-16 07:05:49.000000 netin-1.0.3/requirements/default.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)       32 2023-04-15 10:35:15.000000 netin-1.0.3/requirements/test.txt
+-rw-r--r--   0 espinl    (1001) espinl    (1001)      104 2023-04-16 07:06:05.160397 netin-1.0.3/setup.cfg
+-rw-r--r--   0 espinl    (1001) espinl    (1001)     4228 2023-04-16 07:00:24.000000 netin-1.0.3/setup.py
```

### Comparing `netin-1.0.2/LICENSE` & `netin-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/PKG-INFO` & `netin-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python package to study inequalities in social networks
 Home-page: https://www.networkinequality.com
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.2/README.rst` & `netin-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin/generators/dh.py` & `netin-1.0.3/netin/generators/dh.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin/generators/directed.py` & `netin-1.0.3/netin/generators/directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin/generators/dpa.py` & `netin-1.0.3/netin/generators/dpa.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin/generators/dpah.py` & `netin-1.0.3/netin/generators/dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin/generators/graph.py` & `netin-1.0.3/netin/generators/graph.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin/generators/h.py` & `netin-1.0.3/netin/generators/h.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin/generators/pa.py` & `netin-1.0.3/netin/generators/pa.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin/generators/pah.py` & `netin-1.0.3/netin/generators/pah.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from typing import Union, Set
 
 import numpy as np
+from sympy import symbols
+from sympy import Eq
+from sympy import solve
 
 from netin.utils import constants as const
 from netin.generators.h import Homophily
 from .pa import PA
 
 
 class PAH(PA, Homophily):
@@ -92,18 +95,14 @@
         Homophily.info_params(self)
 
     def info_computed(self):
         PA.info_computed(self)
         Homophily.info_computed(self)
 
     def infer_homophily_values(self) -> (float, float):
-        from sympy import symbols
-        from sympy import Eq
-        from sympy import solve
-
         f_m = self.calculate_fraction_of_minority()
         f_M = 1 - f_m
 
         e = self.count_edges_types()
         e_MM = e['MM']
         e_mm = e['mm']
         M = e['MM'] + e['mm'] + e['Mm'] + e['mM']
```

### Comparing `netin-1.0.2/netin/generators/patc.py` & `netin-1.0.3/netin/generators/patc.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin/generators/patch.py` & `netin-1.0.3/netin/generators/patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin/generators/tc.py` & `netin-1.0.3/netin/generators/tc.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin/generators/tests/test_directed.py` & `netin-1.0.3/netin/generators/tests/test_directed.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin/generators/tests/test_dpah.py` & `netin-1.0.3/netin/generators/tests/test_dpah.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin/generators/tests/test_patch.py` & `netin-1.0.3/netin/generators/tests/test_patch.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin/generators/tests/test_undirected.py` & `netin-1.0.3/netin/generators/tests/test_undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin/generators/undirected.py` & `netin-1.0.3/netin/generators/undirected.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin/stats/distributions.py` & `netin-1.0.3/netin/stats/distributions.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin/stats/ranking.py` & `netin-1.0.3/netin/stats/ranking.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin/utils/constants.py` & `netin-1.0.3/netin/utils/constants.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin/utils/validator.py` & `netin-1.0.3/netin/utils/validator.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin/viz/handlers.py` & `netin-1.0.3/netin/viz/handlers.py`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/netin.egg-info/PKG-INFO` & `netin-1.0.3/netin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netin
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python package to study inequalities in social networks
 Home-page: https://www.networkinequality.com
 Author: Lisette Espín-Noboa
 Author-email: espin@csh.ac.at
 Maintainer: NetIn Developers
 Maintainer-email: netin@googlegroups.com
 Keywords: Networks,Inequalities,Social Networks,Ranking,InferenceGraph Theory,Mathematics,network,undirected,discrete mathematics,math
```

### Comparing `netin-1.0.2/netin.egg-info/SOURCES.txt` & `netin-1.0.3/netin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netin-1.0.2/setup.py` & `netin-1.0.3/setup.py`

 * *Files identical despite different names*

