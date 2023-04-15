# Comparing `tmp/wield.pytest-0.9.2.tar.gz` & `tmp/wield.pytest-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wield.pytest-0.9.2.tar", last modified: Fri Apr 14 23:51:37 2023, max compression
+gzip compressed data, was "wield.pytest-0.9.5.tar", last modified: Sat Apr 15 23:54:51 2023, max compression
```

## Comparing `wield.pytest-0.9.2.tar` & `wield.pytest-0.9.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:37.401434 wield.pytest-0.9.2/
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:37.377434 wield.pytest-0.9.2/LICENSES/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)    10280 2021-10-12 20:00:25.000000 wield.pytest-0.9.2/LICENSES/Apache-2.0.txt
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     7048 2021-10-12 20:00:25.000000 wield.pytest-0.9.2/LICENSES/CC0-1.0.txt
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      483 2023-04-14 19:18:20.000000 wield.pytest-0.9.2/MANIFEST.in
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1034 2023-04-14 19:18:20.000000 wield.pytest-0.9.2/NOTICE
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1231 2023-04-14 23:51:37.405434 wield.pytest-0.9.2/PKG-INFO
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      345 2023-04-14 19:18:20.000000 wield.pytest-0.9.2/README.md
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      449 2023-04-14 19:18:20.000000 wield.pytest-0.9.2/pyproject.toml
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1123 2023-04-14 23:51:37.405434 wield.pytest-0.9.2/setup.cfg
--rwxr-xr-x   0 mcculler  (1000) mcculler  (1000)      746 2023-04-14 19:18:20.000000 wield.pytest-0.9.2/setup.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:37.373434 wield.pytest-0.9.2/src/
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:37.373434 wield.pytest-0.9.2/src/wield/
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:37.381434 wield.pytest-0.9.2/src/wield/pytest/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2671 2023-04-14 19:18:20.000000 wield.pytest-0.9.2/src/wield/pytest/__init__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      474 2023-04-14 23:28:28.000000 wield.pytest-0.9.2/src/wield/pytest/_version.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     9518 2023-04-14 19:18:20.000000 wield.pytest-0.9.2/src/wield/pytest/fixtures.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:37.381434 wield.pytest-0.9.2/src/wield/pytest/parse_collection/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      466 2023-04-14 19:18:20.000000 wield.pytest-0.9.2/src/wield/pytest/parse_collection/__init__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1030 2023-04-14 19:18:20.000000 wield.pytest-0.9.2/src/wield/pytest/parse_collection/__main__.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2473 2023-04-14 19:18:20.000000 wield.pytest-0.9.2/src/wield/pytest/parse_collection/parse.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:37.401434 wield.pytest-0.9.2/src/wield/pytest/parse_collection/test/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1306 2023-04-14 19:18:20.000000 wield.pytest-0.9.2/src/wield/pytest/parse_collection/test/test_pytest_parse_collection.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3838 2023-04-14 19:18:20.000000 wield.pytest-0.9.2/src/wield/pytest/plugin.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:37.401434 wield.pytest-0.9.2/src/wield/pytest/test/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      834 2023-04-14 19:18:20.000000 wield.pytest-0.9.2/src/wield/pytest/test/test_fixtures.py
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     4057 2023-04-14 19:18:20.000000 wield.pytest-0.9.2/src/wield/pytest/utilities.py
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:37.381434 wield.pytest-0.9.2/src/wield.pytest.egg-info/
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1231 2023-04-14 23:51:37.000000 wield.pytest-0.9.2/src/wield.pytest.egg-info/PKG-INFO
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)      719 2023-04-14 23:51:37.000000 wield.pytest-0.9.2/src/wield.pytest.egg-info/SOURCES.txt
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)        1 2023-04-14 23:51:37.000000 wield.pytest-0.9.2/src/wield.pytest.egg-info/dependency_links.txt
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)       29 2023-04-14 23:51:37.000000 wield.pytest-0.9.2/src/wield.pytest.egg-info/requires.txt
--rw-r--r--   0 mcculler  (1000) mcculler  (1000)        6 2023-04-14 23:51:37.000000 wield.pytest-0.9.2/src/wield.pytest.egg-info/top_level.txt
-drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-14 23:51:37.401434 wield.pytest-0.9.2/tools/
--rwxr-xr-x   0 mcculler  (1000) mcculler  (1000)     4118 2023-04-14 19:18:20.000000 wield.pytest-0.9.2/tools/check_versions.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:54:51.639134 wield.pytest-0.9.5/
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:54:51.631138 wield.pytest-0.9.5/LICENSES/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)    10280 2021-10-12 20:00:25.000000 wield.pytest-0.9.5/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     7048 2021-10-12 20:00:25.000000 wield.pytest-0.9.5/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      483 2023-04-14 19:18:20.000000 wield.pytest-0.9.5/MANIFEST.in
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1034 2023-04-14 19:18:20.000000 wield.pytest-0.9.5/NOTICE
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1231 2023-04-15 23:54:51.639134 wield.pytest-0.9.5/PKG-INFO
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      345 2023-04-14 19:18:20.000000 wield.pytest-0.9.5/README.md
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      449 2023-04-14 19:18:20.000000 wield.pytest-0.9.5/pyproject.toml
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1123 2023-04-15 23:54:51.639134 wield.pytest-0.9.5/setup.cfg
+-rwxr-xr-x   0 mcculler  (1000) mcculler  (1000)      746 2023-04-14 19:18:20.000000 wield.pytest-0.9.5/setup.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:54:51.623142 wield.pytest-0.9.5/src/
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:54:51.623142 wield.pytest-0.9.5/src/wield/
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:54:51.631138 wield.pytest-0.9.5/src/wield/pytest/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2671 2023-04-14 19:18:20.000000 wield.pytest-0.9.5/src/wield/pytest/__init__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      474 2023-04-15 23:45:37.000000 wield.pytest-0.9.5/src/wield/pytest/_version.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     9518 2023-04-14 19:18:20.000000 wield.pytest-0.9.5/src/wield/pytest/fixtures.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:54:51.639134 wield.pytest-0.9.5/src/wield/pytest/parse_collection/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      466 2023-04-14 19:18:20.000000 wield.pytest-0.9.5/src/wield/pytest/parse_collection/__init__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1030 2023-04-14 19:18:20.000000 wield.pytest-0.9.5/src/wield/pytest/parse_collection/__main__.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     2473 2023-04-14 19:18:20.000000 wield.pytest-0.9.5/src/wield/pytest/parse_collection/parse.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:54:51.639134 wield.pytest-0.9.5/src/wield/pytest/parse_collection/test/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1306 2023-04-14 19:18:20.000000 wield.pytest-0.9.5/src/wield/pytest/parse_collection/test/test_pytest_parse_collection.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     3838 2023-04-14 19:18:20.000000 wield.pytest-0.9.5/src/wield/pytest/plugin.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:54:51.639134 wield.pytest-0.9.5/src/wield/pytest/test/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      834 2023-04-14 19:18:20.000000 wield.pytest-0.9.5/src/wield/pytest/test/test_fixtures.py
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     4057 2023-04-14 19:18:20.000000 wield.pytest-0.9.5/src/wield/pytest/utilities.py
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:54:51.631138 wield.pytest-0.9.5/src/wield.pytest.egg-info/
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)     1231 2023-04-15 23:54:51.000000 wield.pytest-0.9.5/src/wield.pytest.egg-info/PKG-INFO
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)      719 2023-04-15 23:54:51.000000 wield.pytest-0.9.5/src/wield.pytest.egg-info/SOURCES.txt
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)        1 2023-04-15 23:54:51.000000 wield.pytest-0.9.5/src/wield.pytest.egg-info/dependency_links.txt
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)       29 2023-04-15 23:54:51.000000 wield.pytest-0.9.5/src/wield.pytest.egg-info/requires.txt
+-rw-r--r--   0 mcculler  (1000) mcculler  (1000)        6 2023-04-15 23:54:51.000000 wield.pytest-0.9.5/src/wield.pytest.egg-info/top_level.txt
+drwxr-xr-x   0 mcculler  (1000) mcculler  (1000)        0 2023-04-15 23:54:51.639134 wield.pytest-0.9.5/tools/
+-rwxr-xr-x   0 mcculler  (1000) mcculler  (1000)     4118 2023-04-14 19:18:20.000000 wield.pytest-0.9.5/tools/check_versions.py
```

### Comparing `wield.pytest-0.9.2/LICENSES/Apache-2.0.txt` & `wield.pytest-0.9.5/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `wield.pytest-0.9.2/LICENSES/CC0-1.0.txt` & `wield.pytest-0.9.5/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `wield.pytest-0.9.2/NOTICE` & `wield.pytest-0.9.5/NOTICE`

 * *Files identical despite different names*

### Comparing `wield.pytest-0.9.2/PKG-INFO` & `wield.pytest-0.9.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wield.pytest
-Version: 0.9.2
+Version: 0.9.5
 Summary: Toolkit for modeling interferometers, circuits, signals, and control systems
 Home-page: https://github.com/wieldphysics/wield-pytest
 Author: Lee McCuller
 Author-email: mcculler@caltech.edu
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/wieldphysics/wield-pytest/issues
 Project-URL: Source Code, https://github.com/wieldphysics/wield-pytest
```

### Comparing `wield.pytest-0.9.2/setup.cfg` & `wield.pytest-0.9.5/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wield.pytest
-version = 0.9.2
+version = 0.9.5
 license = Apache-2.0
 license_files = LICENSES/*, NOTICE
 author = Lee McCuller
 author_email = mcculler@caltech.edu
 description = Toolkit for modeling interferometers, circuits, signals, and control systems
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -17,15 +17,16 @@
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
 	pytest
 package_dir = 
 	=src
 packages = find_namespace:
 
 [options.extras_require]
```

### Comparing `wield.pytest-0.9.2/setup.py` & `wield.pytest-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `wield.pytest-0.9.2/src/wield/pytest/__init__.py` & `wield.pytest-0.9.5/src/wield/pytest/__init__.py`

 * *Files identical despite different names*

### Comparing `wield.pytest-0.9.2/src/wield/pytest/fixtures.py` & `wield.pytest-0.9.5/src/wield/pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `wield.pytest-0.9.2/src/wield/pytest/parse_collection/__main__.py` & `wield.pytest-0.9.5/src/wield/pytest/parse_collection/__main__.py`

 * *Files identical despite different names*

### Comparing `wield.pytest-0.9.2/src/wield/pytest/parse_collection/parse.py` & `wield.pytest-0.9.5/src/wield/pytest/parse_collection/parse.py`

 * *Files identical despite different names*

### Comparing `wield.pytest-0.9.2/src/wield/pytest/parse_collection/test/test_pytest_parse_collection.py` & `wield.pytest-0.9.5/src/wield/pytest/parse_collection/test/test_pytest_parse_collection.py`

 * *Files identical despite different names*

### Comparing `wield.pytest-0.9.2/src/wield/pytest/plugin.py` & `wield.pytest-0.9.5/src/wield/pytest/plugin.py`

 * *Files identical despite different names*

### Comparing `wield.pytest-0.9.2/src/wield/pytest/test/test_fixtures.py` & `wield.pytest-0.9.5/src/wield/pytest/test/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `wield.pytest-0.9.2/src/wield/pytest/utilities.py` & `wield.pytest-0.9.5/src/wield/pytest/utilities.py`

 * *Files identical despite different names*

### Comparing `wield.pytest-0.9.2/src/wield.pytest.egg-info/PKG-INFO` & `wield.pytest-0.9.5/src/wield.pytest.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wield.pytest
-Version: 0.9.2
+Version: 0.9.5
 Summary: Toolkit for modeling interferometers, circuits, signals, and control systems
 Home-page: https://github.com/wieldphysics/wield-pytest
 Author: Lee McCuller
 Author-email: mcculler@caltech.edu
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/wieldphysics/wield-pytest/issues
 Project-URL: Source Code, https://github.com/wieldphysics/wield-pytest
```

### Comparing `wield.pytest-0.9.2/src/wield.pytest.egg-info/SOURCES.txt` & `wield.pytest-0.9.5/src/wield.pytest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wield.pytest-0.9.2/tools/check_versions.py` & `wield.pytest-0.9.5/tools/check_versions.py`

 * *Files identical despite different names*

