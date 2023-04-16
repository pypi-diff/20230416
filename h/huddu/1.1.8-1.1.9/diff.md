# Comparing `tmp/huddu-1.1.8.tar.gz` & `tmp/huddu-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huddu-1.1.8.tar", last modified: Thu Mar  9 16:24:08 2023, max compression
+gzip compressed data, was "huddu-1.1.9.tar", last modified: Thu Mar 16 19:35:09 2023, max compression
```

## Comparing `huddu-1.1.8.tar` & `huddu-1.1.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 joshuakock   (501) staff       (20)        0 2023-03-09 16:24:08.750336 huddu-1.1.8/
--rw-r--r--   0 joshuakock   (501) staff       (20)     1062 2022-11-21 17:07:28.000000 huddu-1.1.8/LICENSE
--rw-r--r--   0 joshuakock   (501) staff       (20)      292 2023-03-09 16:24:08.750229 huddu-1.1.8/PKG-INFO
-drwxr-xr-x   0 joshuakock   (501) staff       (20)        0 2023-03-09 16:24:08.749390 huddu-1.1.8/huddu/
--rw-r--r--   0 joshuakock   (501) staff       (20)     2577 2023-03-09 16:21:37.000000 huddu-1.1.8/huddu/Store.py
--rw-r--r--   0 joshuakock   (501) staff       (20)       51 2023-03-09 16:23:13.000000 huddu-1.1.8/huddu/__init__.py
--rw-r--r--   0 joshuakock   (501) staff       (20)       82 2023-03-09 16:23:04.000000 huddu-1.1.8/huddu/_exceptions.py
--rw-r--r--   0 joshuakock   (501) staff       (20)      790 2023-03-09 16:21:10.000000 huddu-1.1.8/huddu/_sessions.py
--rw-r--r--   0 joshuakock   (501) staff       (20)      226 2023-02-08 17:13:43.000000 huddu-1.1.8/huddu/utils.py
-drwxr-xr-x   0 joshuakock   (501) staff       (20)        0 2023-03-09 16:24:08.750059 huddu-1.1.8/huddu.egg-info/
--rw-r--r--   0 joshuakock   (501) staff       (20)      292 2023-03-09 16:24:08.000000 huddu-1.1.8/huddu.egg-info/PKG-INFO
--rw-r--r--   0 joshuakock   (501) staff       (20)      220 2023-03-09 16:24:08.000000 huddu-1.1.8/huddu.egg-info/SOURCES.txt
--rw-r--r--   0 joshuakock   (501) staff       (20)        1 2023-03-09 16:24:08.000000 huddu-1.1.8/huddu.egg-info/dependency_links.txt
--rw-r--r--   0 joshuakock   (501) staff       (20)        6 2023-03-09 16:24:08.000000 huddu-1.1.8/huddu.egg-info/top_level.txt
--rw-r--r--   0 joshuakock   (501) staff       (20)       38 2023-03-09 16:24:08.750367 huddu-1.1.8/setup.cfg
--rw-r--r--   0 joshuakock   (501) staff       (20)      317 2023-03-09 16:23:56.000000 huddu-1.1.8/setup.py
+drwxr-xr-x   0 joshuakock   (501) staff       (20)        0 2023-03-16 19:35:09.745146 huddu-1.1.9/
+-rw-r--r--   0 joshuakock   (501) staff       (20)     1062 2022-11-21 17:07:28.000000 huddu-1.1.9/LICENSE
+-rw-r--r--   0 joshuakock   (501) staff       (20)      292 2023-03-16 19:35:09.745048 huddu-1.1.9/PKG-INFO
+drwxr-xr-x   0 joshuakock   (501) staff       (20)        0 2023-03-16 19:35:09.744137 huddu-1.1.9/huddu/
+-rw-r--r--   0 joshuakock   (501) staff       (20)     2237 2023-03-16 19:34:37.000000 huddu-1.1.9/huddu/Queue.py
+-rw-r--r--   0 joshuakock   (501) staff       (20)     2577 2023-03-09 16:21:37.000000 huddu-1.1.9/huddu/Store.py
+-rw-r--r--   0 joshuakock   (501) staff       (20)       90 2023-03-16 19:12:40.000000 huddu-1.1.9/huddu/__init__.py
+-rw-r--r--   0 joshuakock   (501) staff       (20)      125 2023-03-16 15:50:40.000000 huddu-1.1.9/huddu/_exceptions.py
+-rw-r--r--   0 joshuakock   (501) staff       (20)      790 2023-03-16 19:27:23.000000 huddu-1.1.9/huddu/_sessions.py
+-rw-r--r--   0 joshuakock   (501) staff       (20)      226 2023-02-08 17:13:43.000000 huddu-1.1.9/huddu/utils.py
+drwxr-xr-x   0 joshuakock   (501) staff       (20)        0 2023-03-16 19:35:09.744784 huddu-1.1.9/huddu.egg-info/
+-rw-r--r--   0 joshuakock   (501) staff       (20)      292 2023-03-16 19:35:09.000000 huddu-1.1.9/huddu.egg-info/PKG-INFO
+-rw-r--r--   0 joshuakock   (501) staff       (20)      235 2023-03-16 19:35:09.000000 huddu-1.1.9/huddu.egg-info/SOURCES.txt
+-rw-r--r--   0 joshuakock   (501) staff       (20)        1 2023-03-16 19:35:09.000000 huddu-1.1.9/huddu.egg-info/dependency_links.txt
+-rw-r--r--   0 joshuakock   (501) staff       (20)        6 2023-03-16 19:35:09.000000 huddu-1.1.9/huddu.egg-info/top_level.txt
+-rw-r--r--   0 joshuakock   (501) staff       (20)       38 2023-03-16 19:35:09.745177 huddu-1.1.9/setup.cfg
+-rw-r--r--   0 joshuakock   (501) staff       (20)      317 2023-03-16 19:35:08.000000 huddu-1.1.9/setup.py
```

### Comparing `huddu-1.1.8/LICENSE` & `huddu-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `huddu-1.1.8/huddu/Store.py` & `huddu-1.1.9/huddu/Store.py`

 * *Files identical despite different names*

### Comparing `huddu-1.1.8/huddu/_sessions.py` & `huddu-1.1.9/huddu/_sessions.py`

 * *Files identical despite different names*

