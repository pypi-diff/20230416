# Comparing `tmp/hyperparse-0.0.2.tar.gz` & `tmp/hyperparse-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperparse-0.0.2.tar", last modified: Fri Apr 14 07:05:45 2023, max compression
+gzip compressed data, was "hyperparse-0.0.3.tar", last modified: Sun Apr 16 17:17:27 2023, max compression
```

## Comparing `hyperparse-0.0.2.tar` & `hyperparse-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-sr-x   0 zhfu     (32413) info_fil (10015)        0 2023-04-14 07:05:45.419588 hyperparse-0.0.2/
--rw-r--r--   0 zhfu     (32413) info_fil (10015)     2016 2023-04-14 07:05:45.417588 hyperparse-0.0.2/PKG-INFO
--rw-r--r--   0 zhfu     (32413) info_fil (10015)     1725 2023-04-14 07:04:57.000000 hyperparse-0.0.2/README.md
-drwxr-sr-x   0 zhfu     (32413) info_fil (10015)        0 2023-04-14 07:05:45.386588 hyperparse-0.0.2/hyperparse/
--rw-r--r--   0 zhfu     (32413) info_fil (10015)       78 2023-04-13 11:22:30.000000 hyperparse-0.0.2/hyperparse/__init__.py
--rw-r--r--   0 zhfu     (32413) info_fil (10015)     2510 2023-04-13 20:00:07.000000 hyperparse-0.0.2/hyperparse/hyperparse.py
--rw-r--r--   0 zhfu     (32413) info_fil (10015)       21 2023-04-13 15:01:26.000000 hyperparse-0.0.2/hyperparse/version.py
-drwxr-sr-x   0 zhfu     (32413) info_fil (10015)        0 2023-04-14 07:05:45.409588 hyperparse-0.0.2/hyperparse.egg-info/
--rw-r--r--   0 zhfu     (32413) info_fil (10015)     2016 2023-04-14 07:05:45.000000 hyperparse-0.0.2/hyperparse.egg-info/PKG-INFO
--rw-r--r--   0 zhfu     (32413) info_fil (10015)      237 2023-04-14 07:05:45.000000 hyperparse-0.0.2/hyperparse.egg-info/SOURCES.txt
--rw-r--r--   0 zhfu     (32413) info_fil (10015)        1 2023-04-14 07:05:45.000000 hyperparse-0.0.2/hyperparse.egg-info/dependency_links.txt
--rw-r--r--   0 zhfu     (32413) info_fil (10015)       11 2023-04-14 07:05:45.000000 hyperparse-0.0.2/hyperparse.egg-info/top_level.txt
--rw-r--r--   0 zhfu     (32413) info_fil (10015)       38 2023-04-14 07:05:45.419588 hyperparse-0.0.2/setup.cfg
--rw-r--r--   0 zhfu     (32413) info_fil (10015)      737 2023-04-13 11:26:41.000000 hyperparse-0.0.2/setup.py
-drwxr-sr-x   0 zhfu     (32413) info_fil (10015)        0 2023-04-14 07:05:45.413588 hyperparse-0.0.2/test/
--rw-r--r--   0 zhfu     (32413) info_fil (10015)     2111 2023-04-13 19:08:23.000000 hyperparse-0.0.2/test/test.py
+drwx--S---   0 zhfu     (32413) info_fil (10015)        0 2023-04-16 17:17:27.118532 hyperparse-0.0.3/
+-rw-------   0 zhfu     (32413) info_fil (10015)     2016 2023-04-16 17:17:27.116532 hyperparse-0.0.3/PKG-INFO
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)     1725 2023-04-14 07:04:57.000000 hyperparse-0.0.3/README.md
+drwx--S---   0 zhfu     (32413) info_fil (10015)        0 2023-04-16 17:17:27.079532 hyperparse-0.0.3/hyperparse/
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)       78 2023-04-13 11:22:30.000000 hyperparse-0.0.3/hyperparse/__init__.py
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)     2570 2023-04-15 20:09:42.000000 hyperparse-0.0.3/hyperparse/hyperparse.py
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)       22 2023-04-16 17:17:18.000000 hyperparse-0.0.3/hyperparse/version.py
+drwx--S---   0 zhfu     (32413) info_fil (10015)        0 2023-04-16 17:17:27.104532 hyperparse-0.0.3/hyperparse.egg-info/
+-rw-------   0 zhfu     (32413) info_fil (10015)     2016 2023-04-16 17:17:26.000000 hyperparse-0.0.3/hyperparse.egg-info/PKG-INFO
+-rw-------   0 zhfu     (32413) info_fil (10015)      237 2023-04-16 17:17:27.000000 hyperparse-0.0.3/hyperparse.egg-info/SOURCES.txt
+-rw-------   0 zhfu     (32413) info_fil (10015)        1 2023-04-16 17:17:26.000000 hyperparse-0.0.3/hyperparse.egg-info/dependency_links.txt
+-rw-------   0 zhfu     (32413) info_fil (10015)       11 2023-04-16 17:17:26.000000 hyperparse-0.0.3/hyperparse.egg-info/top_level.txt
+-rw-------   0 zhfu     (32413) info_fil (10015)       38 2023-04-16 17:17:27.119532 hyperparse-0.0.3/setup.cfg
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)      737 2023-04-13 11:26:41.000000 hyperparse-0.0.3/setup.py
+drwx--S---   0 zhfu     (32413) info_fil (10015)        0 2023-04-16 17:17:27.110532 hyperparse-0.0.3/test/
+-rw-r--r--   0 zhfu     (32413) info_fil (10015)     2111 2023-04-13 19:08:23.000000 hyperparse-0.0.3/test/test.py
```

### Comparing `hyperparse-0.0.2/PKG-INFO` & `hyperparse-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperparse
-Version: 0.0.2
+Version: 0.0.3
 Summary: Parse shell env variables to python dict
 Home-page: https://github.com/fuzihaofzh/hyperparse
 Author: 
 Author-email: 
 Keywords: Shell env
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
```

### Comparing `hyperparse-0.0.2/README.md` & `hyperparse-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hyperparse-0.0.2/hyperparse/hyperparse.py` & `hyperparse-0.0.3/hyperparse/hyperparse.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import re
 import os
 import inspect
 import argparse
 import ctypes
 import sys
 
-global var_list
+global var_list, str_list
 var_list = {}
+str_list = {}
 
 def parse_value(value):
     if value.isdigit():
         return int(value)
     elif "." in value and value.replace(".", "", 1).isdigit():
         return float(value)
     elif value.lower() == "none":
@@ -39,15 +40,15 @@
 
 #s = "a=1,b,c=[1,2,3],d=4,e=3.2,f=itud,g=False"
 def parse_env(name):
     env_vars = os.environ
     value = env_vars[name]
     result = parse_string(value)
     var_list[name] = result
-    var_list[name + "_str"] = value
+    str_list[name] = value
 
 """for key, value in env_vars.items():
     result = parse_string(value)
     if key not in globals():
         globals()[key] = result
         globals()[key + "_str"] = value"""
 
@@ -59,26 +60,29 @@
         elif f"--{name}" in sys.argv:
             parse_arg(name)
         else:
             return {}
     return var_list[name]
 
 def get_hyper_str(name):
-    if name not in var_list:
+    if name not in str_list:
         get_hyper(name)
-    return var_list[name + "_str"]
+    if name not in str_list:
+        return None
+    else:
+        return str_list[name]
 
 def parse_arg(name):
     parser = argparse.ArgumentParser()
     parser.add_argument(f"--{name}", type=str, default="")
     args, unknown_args = parser.parse_known_args()
     value = getattr(args, name)
     result = parse_string(value)
     var_list[name] = result
-    var_list[name + "_str"] = value
+    str_list[name] = value
     sys.argv = [sys.argv[0]] + unknown_args
 
 def reset_hyper(hyper, pargs=None):
     if type(hyper) is str:
         hyper = get_hyper(hyper)
     if pargs is None:
         frame = inspect.currentframe().f_back
```

### Comparing `hyperparse-0.0.2/hyperparse.egg-info/PKG-INFO` & `hyperparse-0.0.3/hyperparse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperparse
-Version: 0.0.2
+Version: 0.0.3
 Summary: Parse shell env variables to python dict
 Home-page: https://github.com/fuzihaofzh/hyperparse
 Author: 
 Author-email: 
 Keywords: Shell env
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
```

### Comparing `hyperparse-0.0.2/setup.py` & `hyperparse-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `hyperparse-0.0.2/test/test.py` & `hyperparse-0.0.3/test/test.py`

 * *Files identical despite different names*

