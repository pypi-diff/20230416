# Comparing `tmp/wield.declarative-1.5.0.tar.gz` & `tmp/wield.declarative-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wield.declarative-1.5.0.tar", last modified: Fri Apr 14 23:51:08 2023, max compression
+gzip compressed data, was "wield.declarative-1.5.1.tar", last modified: Sat Apr 15 23:36:49 2023, max compression
```

## Comparing `wield.declarative-1.5.0.tar` & `wield.declarative-1.5.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:08.209801 wield.declarative-1.5.0/
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:08.201801 wield.declarative-1.5.0/LICENSES/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    10280 2021-10-19 15:23:31.000000 wield.declarative-1.5.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     7048 2021-10-19 15:23:31.000000 wield.declarative-1.5.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      483 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/MANIFEST.in
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1034 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/NOTICE
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     8109 2023-04-14 23:51:08.209801 wield.declarative-1.5.0/PKG-INFO
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     7240 2021-10-20 15:14:41.000000 wield.declarative-1.5.0/README.md
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      449 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/pyproject.toml
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1101 2023-04-14 23:51:08.209801 wield.declarative-1.5.0/setup.cfg
--rwxr-xr-x   0 mcculler  (1000) mcculler  (1000)      746 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/setup.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:08.201801 wield.declarative-1.5.0/src/
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:08.201801 wield.declarative-1.5.0/src/wield/
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:08.205801 wield.declarative-1.5.0/src/wield/declarative/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1521 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/__init__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      475 2023-04-14 23:28:28.000000 wield.declarative-1.5.0/src/wield/declarative/_version.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:08.205801 wield.declarative-1.5.0/src/wield/declarative/argparse/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      523 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/argparse/__init__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     4405 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/argparse/annotations.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     7716 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/argparse/oo_argparse.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:08.209801 wield.declarative-1.5.0/src/wield/declarative/callbacks/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      820 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/callbacks/__init__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     8119 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/callbacks/callbacks.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     4719 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/callbacks/relay.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    18816 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/callbacks/state_booleans.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2996 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/callbacks/validators.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     4062 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/metaclass.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2364 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/overridable_object.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:08.209801 wield.declarative-1.5.0/src/wield/declarative/properties/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      976 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/properties/__init__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3567 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/properties/bases.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    15770 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/properties/memoized.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     7804 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/properties/memoized_adv.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     9447 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/properties/memoized_adv_group.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2145 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/properties/utilities.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      850 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/run.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:08.209801 wield.declarative-1.5.0/src/wield/declarative/utilities/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      510 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/utilities/__init__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3133 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/utilities/representations.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      804 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/utilities/super_base.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      663 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/src/wield/declarative/utilities/unique.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:08.205801 wield.declarative-1.5.0/src/wield.declarative.egg-info/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     8109 2023-04-14 23:51:08.000000 wield.declarative-1.5.0/src/wield.declarative.egg-info/PKG-INFO
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1357 2023-04-14 23:51:08.000000 wield.declarative-1.5.0/src/wield.declarative.egg-info/SOURCES.txt
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)        1 2023-04-14 23:51:08.000000 wield.declarative-1.5.0/src/wield.declarative.egg-info/dependency_links.txt
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)       22 2023-04-14 23:51:08.000000 wield.declarative-1.5.0/src/wield.declarative.egg-info/requires.txt
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)        6 2023-04-14 23:51:08.000000 wield.declarative-1.5.0/src/wield.declarative.egg-info/top_level.txt
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:08.209801 wield.declarative-1.5.0/test/
--rwxr-xr-x   0 mcculler  (1000) mcculler  (1000)     1619 2023-04-14 19:17:47.000000 wield.declarative-1.5.0/test/test_properties.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:36:49.285269 wield.declarative-1.5.1/
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:36:49.261281 wield.declarative-1.5.1/LICENSES/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    10280 2021-10-19 15:23:31.000000 wield.declarative-1.5.1/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     7048 2021-10-19 15:23:31.000000 wield.declarative-1.5.1/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      483 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/MANIFEST.in
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1034 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/NOTICE
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     8109 2023-04-15 23:36:49.285269 wield.declarative-1.5.1/PKG-INFO
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     7240 2021-10-20 15:14:41.000000 wield.declarative-1.5.1/README.md
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      449 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/pyproject.toml
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1085 2023-04-15 23:36:49.285269 wield.declarative-1.5.1/setup.cfg
+-rwxr-xr-x   0 mcculler  (1000) mcculler  (1000)      746 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/setup.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:36:49.257283 wield.declarative-1.5.1/src/
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:36:49.257283 wield.declarative-1.5.1/src/wield/
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:36:49.265279 wield.declarative-1.5.1/src/wield/declarative/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1521 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/__init__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      475 2023-04-15 23:29:40.000000 wield.declarative-1.5.1/src/wield/declarative/_version.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:36:49.269277 wield.declarative-1.5.1/src/wield/declarative/argparse/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      523 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/argparse/__init__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     4405 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/argparse/annotations.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     7716 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/argparse/oo_argparse.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:36:49.273275 wield.declarative-1.5.1/src/wield/declarative/callbacks/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      820 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/callbacks/__init__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     8119 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/callbacks/callbacks.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     4719 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/callbacks/relay.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    18816 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/callbacks/state_booleans.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2996 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/callbacks/validators.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     4062 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/metaclass.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2364 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/overridable_object.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:36:49.281271 wield.declarative-1.5.1/src/wield/declarative/properties/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      976 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/properties/__init__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3567 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/properties/bases.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    15770 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/properties/memoized.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     7804 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/properties/memoized_adv.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     9447 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/properties/memoized_adv_group.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2145 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/properties/utilities.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      850 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/run.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:36:49.285269 wield.declarative-1.5.1/src/wield/declarative/utilities/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      510 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/utilities/__init__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3133 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/utilities/representations.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      804 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/utilities/super_base.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      663 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/src/wield/declarative/utilities/unique.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:36:49.261281 wield.declarative-1.5.1/src/wield.declarative.egg-info/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     8109 2023-04-15 23:36:49.000000 wield.declarative-1.5.1/src/wield.declarative.egg-info/PKG-INFO
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1357 2023-04-15 23:36:49.000000 wield.declarative-1.5.1/src/wield.declarative.egg-info/SOURCES.txt
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)        1 2023-04-15 23:36:49.000000 wield.declarative-1.5.1/src/wield.declarative.egg-info/dependency_links.txt
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)        6 2023-04-15 23:36:49.000000 wield.declarative-1.5.1/src/wield.declarative.egg-info/requires.txt
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)        6 2023-04-15 23:36:49.000000 wield.declarative-1.5.1/src/wield.declarative.egg-info/top_level.txt
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:36:49.285269 wield.declarative-1.5.1/test/
+-rwxr-xr-x   0 mcculler  (1000) mcculler  (1000)     1619 2023-04-14 19:17:47.000000 wield.declarative-1.5.1/test/test_properties.py
```

### Comparing `wield.declarative-1.5.0/LICENSES/Apache-2.0.txt` & `wield.declarative-1.5.1/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/LICENSES/CC0-1.0.txt` & `wield.declarative-1.5.1/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/NOTICE` & `wield.declarative-1.5.1/NOTICE`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/PKG-INFO` & `wield.declarative-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wield.declarative
-Version: 1.5.0
+Version: 1.5.1
 Summary: Base classes and methods for declarative object instantiation
 Home-page: https://github.com/wieldphysics/wield-declarative
 Author: Lee McCuller
 Author-email: mcculler@caltech.edu
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/wieldphysics/wield-declarative/issues
 Project-URL: Source Code, https://github.com/wieldphysics/wield-declarative
```

### Comparing `wield.declarative-1.5.0/README.md` & `wield.declarative-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/setup.cfg` & `wield.declarative-1.5.1/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wield.declarative
-version = 1.5.0
+version = 1.5.1
 license = Apache-2.0
 license_files = LICENSES/*, NOTICE
 author = Lee McCuller
 author_email = mcculler@caltech.edu
 description = Base classes and methods for declarative object instantiation
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -17,17 +17,18 @@
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Topic :: Scientific/Engineering :: Physics
 
 [options]
-setup_requires = 'setuptools>=45.0.0'
+setup_requires = 
+	setuptools>=45.0.0
 install_requires = 
-	setuptools_scm>=6.0.0
+	numpy
 package_dir = 
 	=src
 packages = find_namespace:
 
 [options.packages.find]
 where = src
```

### Comparing `wield.declarative-1.5.0/setup.py` & `wield.declarative-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/__init__.py` & `wield.declarative-1.5.1/src/wield/declarative/__init__.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/argparse/__init__.py` & `wield.declarative-1.5.1/src/wield/declarative/argparse/__init__.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/argparse/annotations.py` & `wield.declarative-1.5.1/src/wield/declarative/argparse/annotations.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/argparse/oo_argparse.py` & `wield.declarative-1.5.1/src/wield/declarative/argparse/oo_argparse.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/callbacks/__init__.py` & `wield.declarative-1.5.1/src/wield/declarative/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/callbacks/callbacks.py` & `wield.declarative-1.5.1/src/wield/declarative/callbacks/callbacks.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/callbacks/relay.py` & `wield.declarative-1.5.1/src/wield/declarative/callbacks/relay.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/callbacks/state_booleans.py` & `wield.declarative-1.5.1/src/wield/declarative/callbacks/state_booleans.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/callbacks/validators.py` & `wield.declarative-1.5.1/src/wield/declarative/callbacks/validators.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/metaclass.py` & `wield.declarative-1.5.1/src/wield/declarative/metaclass.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/overridable_object.py` & `wield.declarative-1.5.1/src/wield/declarative/overridable_object.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/properties/__init__.py` & `wield.declarative-1.5.1/src/wield/declarative/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/properties/bases.py` & `wield.declarative-1.5.1/src/wield/declarative/properties/bases.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/properties/memoized.py` & `wield.declarative-1.5.1/src/wield/declarative/properties/memoized.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/properties/memoized_adv.py` & `wield.declarative-1.5.1/src/wield/declarative/properties/memoized_adv.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/properties/memoized_adv_group.py` & `wield.declarative-1.5.1/src/wield/declarative/properties/memoized_adv_group.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/properties/utilities.py` & `wield.declarative-1.5.1/src/wield/declarative/properties/utilities.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/run.py` & `wield.declarative-1.5.1/src/wield/declarative/run.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/utilities/representations.py` & `wield.declarative-1.5.1/src/wield/declarative/utilities/representations.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/utilities/super_base.py` & `wield.declarative-1.5.1/src/wield/declarative/utilities/super_base.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield/declarative/utilities/unique.py` & `wield.declarative-1.5.1/src/wield/declarative/utilities/unique.py`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/src/wield.declarative.egg-info/PKG-INFO` & `wield.declarative-1.5.1/src/wield.declarative.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wield.declarative
-Version: 1.5.0
+Version: 1.5.1
 Summary: Base classes and methods for declarative object instantiation
 Home-page: https://github.com/wieldphysics/wield-declarative
 Author: Lee McCuller
 Author-email: mcculler@caltech.edu
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/wieldphysics/wield-declarative/issues
 Project-URL: Source Code, https://github.com/wieldphysics/wield-declarative
```

### Comparing `wield.declarative-1.5.0/src/wield.declarative.egg-info/SOURCES.txt` & `wield.declarative-1.5.1/src/wield.declarative.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wield.declarative-1.5.0/test/test_properties.py` & `wield.declarative-1.5.1/test/test_properties.py`

 * *Files identical despite different names*

