# Comparing `tmp/pygeoweaver-0.6.1.tar.gz` & `tmp/pygeoweaver-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygeoweaver-0.6.1.tar", last modified: Sun Apr 16 20:54:54 2023, max compression
+gzip compressed data, was "pygeoweaver-0.6.2.tar", last modified: Sun Apr 16 21:25:08 2023, max compression
```

## Comparing `pygeoweaver-0.6.1.tar` & `pygeoweaver-0.6.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:54:54.369967 pygeoweaver-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-16 20:54:54.369967 pygeoweaver-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:54:54.369967 pygeoweaver-0.6.1/pygeoweaver/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/sc_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/sc_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/sc_history.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/sc_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/sc_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/sc_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/sc_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pygeoweaver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:54:54.369967 pygeoweaver-0.6.1/pygeoweaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-16 20:54:54.000000 pygeoweaver-0.6.1/pygeoweaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-16 20:54:54.000000 pygeoweaver-0.6.1/pygeoweaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 20:54:54.000000 pygeoweaver-0.6.1/pygeoweaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-16 20:54:54.000000 pygeoweaver-0.6.1/pygeoweaver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-16 20:54:54.369967 pygeoweaver-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:54:54.369967 pygeoweaver-0.6.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-16 20:54:45.000000 pygeoweaver-0.6.1/test/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:25:08.961156 pygeoweaver-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-16 21:25:08.961156 pygeoweaver-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:25:08.961156 pygeoweaver-0.6.2/pygeoweaver/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/sc_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/sc_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/sc_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/sc_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/sc_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/sc_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/sc_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pygeoweaver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:25:08.961156 pygeoweaver-0.6.2/pygeoweaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-16 21:25:08.000000 pygeoweaver-0.6.2/pygeoweaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-16 21:25:08.000000 pygeoweaver-0.6.2/pygeoweaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 21:25:08.000000 pygeoweaver-0.6.2/pygeoweaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-16 21:25:08.000000 pygeoweaver-0.6.2/pygeoweaver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-16 21:25:08.961156 pygeoweaver-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:25:08.961156 pygeoweaver-0.6.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-16 21:25:00.000000 pygeoweaver-0.6.2/test/test_all.py
```

### Comparing `pygeoweaver-0.6.1/LICENSE` & `pygeoweaver-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.1/PKG-INFO` & `pygeoweaver-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.6.1
+Version: 0.6.2
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pygeoweaver-0.6.1/README.md` & `pygeoweaver-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.1/pygeoweaver/__main__.py` & `pygeoweaver-0.6.2/pygeoweaver/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,30 @@
 from pygeoweaver import show_history
 from pygeoweaver import import_workflow
 from pygeoweaver import list_hosts, list_processes, list_workflows
 from pygeoweaver import start, stop
 
 def main():
     # start geoweaver
-    #start()
+    start()
     # stop geoweaver
     # stop()
     # list resources
     #list_hosts()
     #list_processes()
-    list_workflows()
+    # list_workflows()
     # show history
     #show_history("ll3u3W78eOEfklxhBJ")
     # detail host
     # detail_host("100001")
     # detail process
     # detail_process("7pxu8c")
     #detail_workflow("5jnhcrq33znbu2mue9v2")
     # import workflow
     #import_workflow("/Users/joe/Downloads/gr3ykr8dynu12vrwq11oy.zip")
     # export workflow
-    export_workflow("gr3ykr8dynu12vrwq11oy", "4", "/Users/joe/Downloads/test_pygeoweaver_export.zip")
+    # export_workflow("gr3ykr8dynu12vrwq11oy", "4", "/Users/joe/Downloads/test_pygeoweaver_export.zip")
     # run workflow
-    
+
 
 if __name__ == "__main__":
      main()
```

### Comparing `pygeoweaver-0.6.1/pygeoweaver/sc_detail.py` & `pygeoweaver-0.6.2/pygeoweaver/sc_detail.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.1/pygeoweaver/sc_export.py` & `pygeoweaver-0.6.2/pygeoweaver/sc_export.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.1/pygeoweaver/sc_import.py` & `pygeoweaver-0.6.2/pygeoweaver/sc_import.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.1/pygeoweaver/sc_list.py` & `pygeoweaver-0.6.2/pygeoweaver/sc_list.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.1/pygeoweaver/sc_run.py` & `pygeoweaver-0.6.2/pygeoweaver/sc_run.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.1/pygeoweaver/server.py` & `pygeoweaver-0.6.2/pygeoweaver/server.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.1/pygeoweaver/utils.py` & `pygeoweaver-0.6.2/pygeoweaver/utils.py`

 * *Files identical despite different names*

### Comparing `pygeoweaver-0.6.1/pygeoweaver.egg-info/PKG-INFO` & `pygeoweaver-0.6.2/pygeoweaver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygeoweaver
-Version: 0.6.1
+Version: 0.6.2
 Summary: This is a wrapper package of the Geoweaver app.
 Author-email: Geoweaver team <geoweaver.app@gmail.com>
 Project-URL: Homepage, https://github.com/ESIPFed/pygeoweaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `pygeoweaver-0.6.1/pyproject.toml` & `pygeoweaver-0.6.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygeoweaver"
-version = "0.6.1"
+version = "0.6.2"
 authors = [
   { name="Geoweaver team", email="geoweaver.app@gmail.com" },
 ]
 description = "This is a wrapper package of the Geoweaver app."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -18,15 +18,15 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ESIPFed/pygeoweaver"
 
 [tool.poetry]
 name = "pygeoweaver"
-version = "0.6.0"
+version = "0.6.2"
 description = "This is a wrapper package of the Geoweaver app."
 authors = ["Geoweaver team <geoweaver.app@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/ESIPFed/pygeoweaver"
 
 [tool.poetry.dependencies]
 python = ">=3.7"
```

### Comparing `pygeoweaver-0.6.1/test/test_all.py` & `pygeoweaver-0.6.2/test/test_all.py`

 * *Files identical despite different names*

