# Comparing `tmp/Liara-2.5.2.tar.gz` & `tmp/Liara-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Liara-2.5.2.tar", last modified: Sat Apr 15 11:41:51 2023, max compression
+gzip compressed data, was "Liara-2.5.3.tar", last modified: Sun Apr 16 11:43:25 2023, max compression
```

## Comparing `Liara-2.5.2.tar` & `Liara-2.5.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-15 11:41:51.566908 Liara-2.5.2/
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1332 2023-01-02 13:55:30.000000 Liara-2.5.2/LICENSE.txt
-drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-15 11:41:51.566908 Liara-2.5.2/Liara.egg-info/
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1395 2023-04-15 11:41:51.000000 Liara-2.5.2/Liara.egg-info/PKG-INFO
--rw-r--r--   0 anteru    (1000) anteru    (1000)      729 2023-04-15 11:41:51.000000 Liara-2.5.2/Liara.egg-info/SOURCES.txt
--rw-r--r--   0 anteru    (1000) anteru    (1000)        1 2023-04-15 11:41:51.000000 Liara-2.5.2/Liara.egg-info/dependency_links.txt
--rw-r--r--   0 anteru    (1000) anteru    (1000)       45 2023-04-15 11:41:51.000000 Liara-2.5.2/Liara.egg-info/entry_points.txt
--rw-r--r--   0 anteru    (1000) anteru    (1000)      376 2023-04-15 11:41:51.000000 Liara-2.5.2/Liara.egg-info/requires.txt
--rw-r--r--   0 anteru    (1000) anteru    (1000)        6 2023-04-15 11:41:51.000000 Liara-2.5.2/Liara.egg-info/top_level.txt
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1395 2023-04-15 11:41:51.566908 Liara-2.5.2/PKG-INFO
--rw-r--r--   0 anteru    (1000) anteru    (1000)      441 2023-01-01 11:59:39.000000 Liara-2.5.2/README.md
-drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-15 11:41:51.566908 Liara-2.5.2/liara/
--rwxr-xr-x   0 anteru    (1000) anteru    (1000)    29291 2023-04-15 11:41:10.000000 Liara-2.5.2/liara/__init__.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     4975 2023-01-01 11:59:39.000000 Liara-2.5.2/liara/actions.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     9328 2023-02-11 11:15:23.000000 Liara-2.5.2/liara/cache.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    10367 2023-04-15 11:41:10.000000 Liara-2.5.2/liara/cmdline.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     2675 2023-02-11 11:15:23.000000 Liara-2.5.2/liara/config.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     4540 2023-01-01 11:59:39.000000 Liara-2.5.2/liara/feeds.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    10536 2023-04-15 11:41:10.000000 Liara-2.5.2/liara/md.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    31982 2023-02-11 11:15:23.000000 Liara-2.5.2/liara/nodes.py
-drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-15 11:41:51.566908 Liara-2.5.2/liara/plugins/
--rw-r--r--   0 anteru    (1000) anteru    (1000)      132 2023-01-01 11:59:39.000000 Liara-2.5.2/liara/plugins/__init__.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)      889 2023-04-15 11:41:10.000000 Liara-2.5.2/liara/plugins/has_pending_document.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1326 2023-04-15 11:41:10.000000 Liara-2.5.2/liara/plugins/series_schedule.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     5349 2023-02-11 11:15:23.000000 Liara-2.5.2/liara/publish.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     8046 2023-02-11 11:15:23.000000 Liara-2.5.2/liara/query.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    11574 2023-01-01 11:59:39.000000 Liara-2.5.2/liara/quickstart.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     5236 2023-01-22 13:57:52.000000 Liara-2.5.2/liara/server.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1953 2023-02-11 11:15:23.000000 Liara-2.5.2/liara/signals.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    28210 2023-04-15 11:41:10.000000 Liara-2.5.2/liara/site.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)    11215 2023-01-01 11:59:39.000000 Liara-2.5.2/liara/template.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     4116 2023-01-01 11:59:39.000000 Liara-2.5.2/liara/util.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)      888 2023-01-01 11:59:39.000000 Liara-2.5.2/liara/yaml.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)      190 2023-01-01 11:59:39.000000 Liara-2.5.2/pyproject.toml
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1457 2023-04-15 11:41:51.566908 Liara-2.5.2/setup.cfg
--rw-r--r--   0 anteru    (1000) anteru    (1000)       38 2023-01-01 11:59:39.000000 Liara-2.5.2/setup.py
-drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-15 11:41:51.566908 Liara-2.5.2/test/
--rw-r--r--   0 anteru    (1000) anteru    (1000)      141 2023-01-01 11:59:39.000000 Liara-2.5.2/test/test_cache.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1118 2023-02-11 11:15:23.000000 Liara-2.5.2/test/test_md.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1363 2023-02-11 11:15:23.000000 Liara-2.5.2/test/test_nodes.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     2498 2023-02-11 11:15:23.000000 Liara-2.5.2/test/test_query.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     6064 2023-01-01 11:59:39.000000 Liara-2.5.2/test/test_site.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     2391 2023-01-01 11:59:39.000000 Liara-2.5.2/test/test_template.py
--rw-r--r--   0 anteru    (1000) anteru    (1000)     1031 2023-01-01 11:59:39.000000 Liara-2.5.2/test/test_util.py
+drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-16 11:43:25.966311 Liara-2.5.3/
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1332 2023-01-02 13:55:30.000000 Liara-2.5.3/LICENSE.txt
+drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-16 11:43:25.966311 Liara-2.5.3/Liara.egg-info/
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1395 2023-04-16 11:43:25.000000 Liara-2.5.3/Liara.egg-info/PKG-INFO
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      729 2023-04-16 11:43:25.000000 Liara-2.5.3/Liara.egg-info/SOURCES.txt
+-rw-r--r--   0 anteru    (1000) anteru    (1000)        1 2023-04-16 11:43:25.000000 Liara-2.5.3/Liara.egg-info/dependency_links.txt
+-rw-r--r--   0 anteru    (1000) anteru    (1000)       45 2023-04-16 11:43:25.000000 Liara-2.5.3/Liara.egg-info/entry_points.txt
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      376 2023-04-16 11:43:25.000000 Liara-2.5.3/Liara.egg-info/requires.txt
+-rw-r--r--   0 anteru    (1000) anteru    (1000)        6 2023-04-16 11:43:25.000000 Liara-2.5.3/Liara.egg-info/top_level.txt
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1395 2023-04-16 11:43:25.966311 Liara-2.5.3/PKG-INFO
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      441 2023-01-01 11:59:39.000000 Liara-2.5.3/README.md
+drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-16 11:43:25.966311 Liara-2.5.3/liara/
+-rwxr-xr-x   0 anteru    (1000) anteru    (1000)    29291 2023-04-16 11:43:18.000000 Liara-2.5.3/liara/__init__.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     4975 2023-01-01 11:59:39.000000 Liara-2.5.3/liara/actions.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     9328 2023-02-11 11:15:23.000000 Liara-2.5.3/liara/cache.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    10367 2023-04-15 11:41:10.000000 Liara-2.5.3/liara/cmdline.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     2675 2023-02-11 11:15:23.000000 Liara-2.5.3/liara/config.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     4540 2023-01-01 11:59:39.000000 Liara-2.5.3/liara/feeds.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    12347 2023-04-16 11:43:18.000000 Liara-2.5.3/liara/md.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    31982 2023-02-11 11:15:23.000000 Liara-2.5.3/liara/nodes.py
+drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-16 11:43:25.966311 Liara-2.5.3/liara/plugins/
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      132 2023-01-01 11:59:39.000000 Liara-2.5.3/liara/plugins/__init__.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      889 2023-04-15 11:41:10.000000 Liara-2.5.3/liara/plugins/has_pending_document.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1326 2023-04-15 11:41:10.000000 Liara-2.5.3/liara/plugins/series_schedule.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     5349 2023-02-11 11:15:23.000000 Liara-2.5.3/liara/publish.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     8046 2023-02-11 11:15:23.000000 Liara-2.5.3/liara/query.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    11574 2023-01-01 11:59:39.000000 Liara-2.5.3/liara/quickstart.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     5236 2023-01-22 13:57:52.000000 Liara-2.5.3/liara/server.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1953 2023-02-11 11:15:23.000000 Liara-2.5.3/liara/signals.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    28210 2023-04-15 11:41:10.000000 Liara-2.5.3/liara/site.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)    11215 2023-01-01 11:59:39.000000 Liara-2.5.3/liara/template.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     4116 2023-01-01 11:59:39.000000 Liara-2.5.3/liara/util.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      888 2023-01-01 11:59:39.000000 Liara-2.5.3/liara/yaml.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      190 2023-01-01 11:59:39.000000 Liara-2.5.3/pyproject.toml
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1457 2023-04-16 11:43:25.966311 Liara-2.5.3/setup.cfg
+-rw-r--r--   0 anteru    (1000) anteru    (1000)       38 2023-01-01 11:59:39.000000 Liara-2.5.3/setup.py
+drwxr-xr-x   0 anteru    (1000) anteru    (1000)        0 2023-04-16 11:43:25.966311 Liara-2.5.3/test/
+-rw-r--r--   0 anteru    (1000) anteru    (1000)      141 2023-01-01 11:59:39.000000 Liara-2.5.3/test/test_cache.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     3708 2023-04-16 11:43:18.000000 Liara-2.5.3/test/test_md.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1363 2023-02-11 11:15:23.000000 Liara-2.5.3/test/test_nodes.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     2498 2023-02-11 11:15:23.000000 Liara-2.5.3/test/test_query.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     6064 2023-01-01 11:59:39.000000 Liara-2.5.3/test/test_site.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     2391 2023-01-01 11:59:39.000000 Liara-2.5.3/test/test_template.py
+-rw-r--r--   0 anteru    (1000) anteru    (1000)     1031 2023-01-01 11:59:39.000000 Liara-2.5.3/test/test_util.py
```

### Comparing `Liara-2.5.2/LICENSE.txt` & `Liara-2.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/Liara.egg-info/PKG-INFO` & `Liara-2.5.3/Liara.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Liara
-Version: 2.5.2
+Version: 2.5.3
 Summary: Static page generator
 Home-page: http://shelter13.net/projects/Liara
 Author: Matthäus G. Chajdas
 Author-email: dev@anteru.net
 License: BSD 2-Clause License
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Liara-2.5.2/Liara.egg-info/SOURCES.txt` & `Liara-2.5.3/Liara.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/PKG-INFO` & `Liara-2.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Liara
-Version: 2.5.2
+Version: 2.5.3
 Summary: Static page generator
 Home-page: http://shelter13.net/projects/Liara
 Author: Matthäus G. Chajdas
 Author-email: dev@anteru.net
 License: BSD 2-Clause License
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Liara-2.5.2/liara/__init__.py` & `Liara-2.5.3/liara/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     _process_node_sync
 )
 
 from .cache import Cache, FilesystemCache, NullCache, Sqlite3Cache, RedisCache
 from .util import FilesystemWalker, flatten_dictionary
 from .yaml import load_yaml
 
-__version__ = '2.5.2'
+__version__ = '2.5.3'
 __all__ = [
     'actions',
     'cache',
     'cmdline',
     'config',
     'feeds',
     'md',
```

### Comparing `Liara-2.5.2/liara/actions.py` & `Liara-2.5.3/liara/actions.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/liara/cache.py` & `Liara-2.5.3/liara/cache.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/liara/cmdline.py` & `Liara-2.5.3/liara/cmdline.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/liara/config.py` & `Liara-2.5.3/liara/config.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/liara/feeds.py` & `Liara-2.5.3/liara/feeds.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/liara/nodes.py` & `Liara-2.5.3/liara/nodes.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/liara/plugins/has_pending_document.py` & `Liara-2.5.3/liara/plugins/has_pending_document.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/liara/plugins/series_schedule.py` & `Liara-2.5.3/liara/plugins/series_schedule.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/liara/publish.py` & `Liara-2.5.3/liara/publish.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/liara/query.py` & `Liara-2.5.3/liara/query.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/liara/quickstart.py` & `Liara-2.5.3/liara/quickstart.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/liara/server.py` & `Liara-2.5.3/liara/server.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/liara/signals.py` & `Liara-2.5.3/liara/signals.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/liara/site.py` & `Liara-2.5.3/liara/site.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/liara/template.py` & `Liara-2.5.3/liara/template.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/liara/util.py` & `Liara-2.5.3/liara/util.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/liara/yaml.py` & `Liara-2.5.3/liara/yaml.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/setup.cfg` & `Liara-2.5.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/test/test_nodes.py` & `Liara-2.5.3/test/test_nodes.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/test/test_query.py` & `Liara-2.5.3/test/test_query.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/test/test_site.py` & `Liara-2.5.3/test/test_site.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/test/test_template.py` & `Liara-2.5.3/test/test_template.py`

 * *Files identical despite different names*

### Comparing `Liara-2.5.2/test/test_util.py` & `Liara-2.5.3/test/test_util.py`

 * *Files identical despite different names*

