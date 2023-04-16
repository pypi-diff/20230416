# Comparing `tmp/pygeoweaver-0.6.0.tar.gz` & `tmp/pygeoweaver-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeoweaver-0.6.0.tar", last modified: Sun Apr 16 20:14:20 2023, max compression
+gzip compressed data, was "pygeoweaver-0.6.1.tar", last modified: Sun Apr 16 20:54:54 2023, max compression
```

## Comparing `pygeoweaver-0.6.0.tar` & `pygeoweaver-0.6.1.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:14:20.855888 pygeoweaver-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-16 20:14:08.000000 pygeoweaver-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-16 20:14:20.855888 pygeoweaver-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-16 20:14:08.000000 pygeoweaver-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:14:20.855888 pygeoweaver-0.6.0/pygeoweaver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 20:14:08.000000 pygeoweaver-0.6.0/pygeoweaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-16 20:14:08.000000 pygeoweaver-0.6.0/pygeoweaver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-16 20:14:08.000000 pygeoweaver-0.6.0/pygeoweaver/sc_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-16 20:14:08.000000 pygeoweaver-0.6.0/pygeoweaver/sc_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-16 20:14:08.000000 pygeoweaver-0.6.0/pygeoweaver/sc_history.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-16 20:14:08.000000 pygeoweaver-0.6.0/pygeoweaver/sc_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-16 20:14:08.000000 pygeoweaver-0.6.0/pygeoweaver/sc_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-16 20:14:08.000000 pygeoweaver-0.6.0/pygeoweaver/sc_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-16 20:14:08.000000 pygeoweaver-0.6.0/pygeoweaver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-16 20:14:08.000000 pygeoweaver-0.6.0/pygeoweaver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:14:20.855888 pygeoweaver-0.6.0/pygeoweaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-16 20:14:20.000000 pygeoweaver-0.6.0/pygeoweaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-16 20:14:20.000000 pygeoweaver-0.6.0/pygeoweaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 20:14:20.000000 pygeoweaver-0.6.0/pygeoweaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 20:14:20.000000 pygeoweaver-0.6.0/pygeoweaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-16 20:14:08.000000 pygeoweaver-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-16 20:14:20.855888 pygeoweaver-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:14:20.855888 pygeoweaver-0.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 20:14:08.000000 pygeoweaver-0.6.0/test/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:54:54.369967 pygeoweaver-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-16 20:54:54.369967 pygeoweaver-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:54:54.369967 pygeoweaver-0.6.1/pygeoweaver/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/sc_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/sc_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/sc_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/sc_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/sc_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/sc_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/sc_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:54:54.369967 pygeoweaver-0.6.1/pygeoweaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-16 20:54:54.000000 pygeoweaver-0.6.1/pygeoweaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-16 20:54:54.000000 pygeoweaver-0.6.1/pygeoweaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 20:54:54.000000 pygeoweaver-0.6.1/pygeoweaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-16 20:54:54.000000 pygeoweaver-0.6.1/pygeoweaver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-16 20:54:54.369967 pygeoweaver-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:54:54.369967 pygeoweaver-0.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/test/test_all.py
```

### Comparing `pygeoweaver-0.6.0/LICENSE` & `pygeoweaver-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.0/PKG-INFO` & `pygeoweaver-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.6.0
+Version: 0.6.1
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pygeoweaver-0.6.0/README.md` & `pygeoweaver-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.0/pygeoweaver/__main__.py` & `pygeoweaver-0.6.1/pygeoweaver/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 The main function of pygeoweaver
 To run in CLI mode. 
 """
-from pygeoweaver.sc_detail import detail_host, detail_process, detail_workflow
-from pygeoweaver.sc_export import export_workflow
-from pygeoweaver.sc_history import show_history
-from pygeoweaver.sc_import import import_workflow
-from pygeoweaver.sc_list import list_hosts, list_processes, list_workflows
-from pygeoweaver.server import start, stop
+from pygeoweaver import detail_host, detail_process, detail_workflow
+from pygeoweaver import export_workflow
+from pygeoweaver import show_history
+from pygeoweaver import import_workflow
+from pygeoweaver import list_hosts, list_processes, list_workflows
+from pygeoweaver import start, stop
 
 def main():
     # start geoweaver
     #start()
     # stop geoweaver
     # stop()
     # list resources
@@ -25,11 +25,12 @@
     # detail process
     # detail_process("7pxu8c")
     #detail_workflow("5jnhcrq33znbu2mue9v2")
     # import workflow
     #import_workflow("/Users/joe/Downloads/gr3ykr8dynu12vrwq11oy.zip")
     # export workflow
     export_workflow("gr3ykr8dynu12vrwq11oy", "4", "/Users/joe/Downloads/test_pygeoweaver_export.zip")
-
+    # run workflow
+    
 
 if __name__ == "__main__":
      main()
```

### Comparing `pygeoweaver-0.6.0/pygeoweaver/sc_detail.py` & `pygeoweaver-0.6.1/pygeoweaver/sc_detail.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.0/pygeoweaver/sc_export.py` & `pygeoweaver-0.6.1/pygeoweaver/sc_export.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.0/pygeoweaver/sc_import.py` & `pygeoweaver-0.6.1/pygeoweaver/sc_import.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.0/pygeoweaver/sc_list.py` & `pygeoweaver-0.6.1/pygeoweaver/sc_list.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.0/pygeoweaver/sc_run.py` & `pygeoweaver-0.6.1/pygeoweaver/sc_run.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.0/pygeoweaver/server.py` & `pygeoweaver-0.6.1/pygeoweaver/server.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.0/pygeoweaver/utils.py` & `pygeoweaver-0.6.1/pygeoweaver/utils.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.0/pygeoweaver.egg-info/PKG-INFO` & `pygeoweaver-0.6.1/pygeoweaver.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.6.0
+Version: 0.6.1
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pygeoweaver-0.6.0/pyproject.toml` & `pygeoweaver-0.6.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygeoweaver"
-version = "0.6.0"
+version = "0.6.1"
 authors = [
   { name="Geoweaver team", email="geoweaver.app@gmail.com" },
 ]
 description = "This is a wrapper package of the Geoweaver app."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -27,9 +27,10 @@
 authors = ["Geoweaver team <geoweaver.app@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/ESIPFed/pygeoweaver"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 setuptools = ">=61.0"
+requests = "2.28.2"
 
 [tool.poetry.scripts]
```

