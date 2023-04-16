# Comparing `tmp/report-env-0.0.3.tar.gz` & `tmp/report-env-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "report-env-0.0.3.tar", last modified: Sun Apr 16 07:56:28 2023, max compression
+gzip compressed data, was "report-env-0.0.4.tar", last modified: Sun Apr 16 08:01:53 2023, max compression
```

## Comparing `report-env-0.0.3.tar` & `report-env-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 07:56:28.716658 report-env-0.0.3/
--rw-r--r--   0 swyx       (501) staff       (20)     1090 2023-04-16 07:33:25.000000 report-env-0.0.3/LICENSE
--rw-r--r--   0 swyx       (501) staff       (20)      117 2023-04-16 07:45:18.000000 report-env-0.0.3/MANIFEST.in
--rw-r--r--   0 swyx       (501) staff       (20)      853 2023-04-16 07:56:28.716494 report-env-0.0.3/PKG-INFO
--rw-r--r--   0 swyx       (501) staff       (20)      364 2023-04-16 07:45:32.000000 report-env-0.0.3/README.md
--rw-r--r--   0 swyx       (501) staff       (20)      532 2023-04-16 07:56:22.000000 report-env-0.0.3/pyproject.toml
--rw-r--r--   0 swyx       (501) staff       (20)       38 2023-04-16 07:56:28.716708 report-env-0.0.3/setup.cfg
-drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 07:56:28.713763 report-env-0.0.3/src/
-drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 07:56:28.715389 report-env-0.0.3/src/report-env/
--rw-r--r--   0 swyx       (501) staff       (20)        0 2023-04-16 07:33:10.000000 report-env-0.0.3/src/report-env/__init__.py
--rw-r--r--   0 swyx       (501) staff       (20)       62 2023-04-16 07:46:10.000000 report-env-0.0.3/src/report-env/__main__.py
--rw-r--r--   0 swyx       (501) staff       (20)      690 2023-04-16 07:46:21.000000 report-env-0.0.3/src/report-env/main.py
-drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 07:56:28.716293 report-env-0.0.3/src/report_env.egg-info/
--rw-r--r--   0 swyx       (501) staff       (20)      853 2023-04-16 07:56:28.000000 report-env-0.0.3/src/report_env.egg-info/PKG-INFO
--rw-r--r--   0 swyx       (501) staff       (20)      314 2023-04-16 07:56:28.000000 report-env-0.0.3/src/report_env.egg-info/SOURCES.txt
--rw-r--r--   0 swyx       (501) staff       (20)        1 2023-04-16 07:56:28.000000 report-env-0.0.3/src/report_env.egg-info/dependency_links.txt
--rw-r--r--   0 swyx       (501) staff       (20)       56 2023-04-16 07:56:28.000000 report-env-0.0.3/src/report_env.egg-info/entry_points.txt
--rw-r--r--   0 swyx       (501) staff       (20)       11 2023-04-16 07:56:28.000000 report-env-0.0.3/src/report_env.egg-info/top_level.txt
+drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 08:01:53.023997 report-env-0.0.4/
+-rw-r--r--   0 swyx       (501) staff       (20)     1090 2023-04-16 07:33:25.000000 report-env-0.0.4/LICENSE
+-rw-r--r--   0 swyx       (501) staff       (20)      117 2023-04-16 07:45:18.000000 report-env-0.0.4/MANIFEST.in
+-rw-r--r--   0 swyx       (501) staff       (20)      853 2023-04-16 08:01:53.023862 report-env-0.0.4/PKG-INFO
+-rw-r--r--   0 swyx       (501) staff       (20)      364 2023-04-16 07:45:32.000000 report-env-0.0.4/README.md
+-rw-r--r--   0 swyx       (501) staff       (20)      532 2023-04-16 08:01:45.000000 report-env-0.0.4/pyproject.toml
+-rw-r--r--   0 swyx       (501) staff       (20)       38 2023-04-16 08:01:53.024034 report-env-0.0.4/setup.cfg
+drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 08:01:53.021432 report-env-0.0.4/src/
+drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 08:01:53.023059 report-env-0.0.4/src/report-env/
+-rw-r--r--   0 swyx       (501) staff       (20)        0 2023-04-16 07:33:10.000000 report-env-0.0.4/src/report-env/__init__.py
+-rw-r--r--   0 swyx       (501) staff       (20)       62 2023-04-16 07:46:10.000000 report-env-0.0.4/src/report-env/__main__.py
+-rw-r--r--   0 swyx       (501) staff       (20)      690 2023-04-16 07:46:21.000000 report-env-0.0.4/src/report-env/main.py
+drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 08:01:53.023696 report-env-0.0.4/src/report_env.egg-info/
+-rw-r--r--   0 swyx       (501) staff       (20)      853 2023-04-16 08:01:53.000000 report-env-0.0.4/src/report_env.egg-info/PKG-INFO
+-rw-r--r--   0 swyx       (501) staff       (20)      273 2023-04-16 08:01:53.000000 report-env-0.0.4/src/report_env.egg-info/SOURCES.txt
+-rw-r--r--   0 swyx       (501) staff       (20)        1 2023-04-16 08:01:53.000000 report-env-0.0.4/src/report_env.egg-info/dependency_links.txt
+-rw-r--r--   0 swyx       (501) staff       (20)       11 2023-04-16 08:01:53.000000 report-env-0.0.4/src/report_env.egg-info/top_level.txt
```

### Comparing `report-env-0.0.3/LICENSE` & `report-env-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `report-env-0.0.3/PKG-INFO` & `report-env-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: report-env
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Author-email: swyx <swyx@dontemailme.com>
 Project-URL: Homepage, https://github.com/sw-yx/report-env
 Project-URL: Bug Tracker, https://github.com/sw-yx/report-env/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `report-env-0.0.3/src/report-env/main.py` & `report-env-0.0.4/src/report-env/main.py`

 * *Files identical despite different names*

### Comparing `report-env-0.0.3/src/report_env.egg-info/PKG-INFO` & `report-env-0.0.4/src/report_env.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: report-env
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Author-email: swyx <swyx@dontemailme.com>
 Project-URL: Homepage, https://github.com/sw-yx/report-env
 Project-URL: Bug Tracker, https://github.com/sw-yx/report-env/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

