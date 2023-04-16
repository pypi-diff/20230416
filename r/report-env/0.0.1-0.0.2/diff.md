# Comparing `tmp/report-env-0.0.1.tar.gz` & `tmp/report-env-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "report-env-0.0.1.tar", last modified: Sun Apr 16 07:40:14 2023, max compression
+gzip compressed data, was "report-env-0.0.2.tar", last modified: Sun Apr 16 07:50:21 2023, max compression
```

## Comparing `report-env-0.0.1.tar` & `report-env-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 07:40:14.794445 report-env-0.0.1/
--rw-r--r--   0 swyx       (501) staff       (20)     1090 2023-04-16 07:33:25.000000 report-env-0.0.1/LICENSE
--rw-r--r--   0 swyx       (501) staff       (20)      734 2023-04-16 07:40:14.794260 report-env-0.0.1/PKG-INFO
--rw-r--r--   0 swyx       (501) staff       (20)      244 2023-04-16 07:39:14.000000 report-env-0.0.1/README.md
--rw-r--r--   0 swyx       (501) staff       (20)      474 2023-04-16 07:39:43.000000 report-env-0.0.1/pyproject.toml
--rw-r--r--   0 swyx       (501) staff       (20)       38 2023-04-16 07:40:14.794494 report-env-0.0.1/setup.cfg
-drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 07:40:14.791079 report-env-0.0.1/src/
-drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 07:40:14.792425 report-env-0.0.1/src/report-env/
--rw-r--r--   0 swyx       (501) staff       (20)        0 2023-04-16 07:33:10.000000 report-env-0.0.1/src/report-env/__init__.py
--rw-r--r--   0 swyx       (501) staff       (20)       42 2023-04-16 07:33:18.000000 report-env-0.0.1/src/report-env/example.py
-drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 07:40:14.794002 report-env-0.0.1/src/report_env.egg-info/
--rw-r--r--   0 swyx       (501) staff       (20)      734 2023-04-16 07:40:14.000000 report-env-0.0.1/src/report_env.egg-info/PKG-INFO
--rw-r--r--   0 swyx       (501) staff       (20)      237 2023-04-16 07:40:14.000000 report-env-0.0.1/src/report_env.egg-info/SOURCES.txt
--rw-r--r--   0 swyx       (501) staff       (20)        1 2023-04-16 07:40:14.000000 report-env-0.0.1/src/report_env.egg-info/dependency_links.txt
--rw-r--r--   0 swyx       (501) staff       (20)       11 2023-04-16 07:40:14.000000 report-env-0.0.1/src/report_env.egg-info/top_level.txt
+drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 07:50:21.507456 report-env-0.0.2/
+-rw-r--r--   0 swyx       (501) staff       (20)     1090 2023-04-16 07:33:25.000000 report-env-0.0.2/LICENSE
+-rw-r--r--   0 swyx       (501) staff       (20)      117 2023-04-16 07:45:18.000000 report-env-0.0.2/MANIFEST.in
+-rw-r--r--   0 swyx       (501) staff       (20)      853 2023-04-16 07:50:21.507321 report-env-0.0.2/PKG-INFO
+-rw-r--r--   0 swyx       (501) staff       (20)      364 2023-04-16 07:45:32.000000 report-env-0.0.2/README.md
+-rw-r--r--   0 swyx       (501) staff       (20)      474 2023-04-16 07:50:01.000000 report-env-0.0.2/pyproject.toml
+-rw-r--r--   0 swyx       (501) staff       (20)       38 2023-04-16 07:50:21.507497 report-env-0.0.2/setup.cfg
+drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 07:50:21.505045 report-env-0.0.2/src/
+drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 07:50:21.506508 report-env-0.0.2/src/report-env/
+-rw-r--r--   0 swyx       (501) staff       (20)        0 2023-04-16 07:33:10.000000 report-env-0.0.2/src/report-env/__init__.py
+-rw-r--r--   0 swyx       (501) staff       (20)       62 2023-04-16 07:46:10.000000 report-env-0.0.2/src/report-env/__main__.py
+-rw-r--r--   0 swyx       (501) staff       (20)      690 2023-04-16 07:46:21.000000 report-env-0.0.2/src/report-env/main.py
+drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 07:50:21.507156 report-env-0.0.2/src/report_env.egg-info/
+-rw-r--r--   0 swyx       (501) staff       (20)      853 2023-04-16 07:50:21.000000 report-env-0.0.2/src/report_env.egg-info/PKG-INFO
+-rw-r--r--   0 swyx       (501) staff       (20)      273 2023-04-16 07:50:21.000000 report-env-0.0.2/src/report_env.egg-info/SOURCES.txt
+-rw-r--r--   0 swyx       (501) staff       (20)        1 2023-04-16 07:50:21.000000 report-env-0.0.2/src/report_env.egg-info/dependency_links.txt
+-rw-r--r--   0 swyx       (501) staff       (20)       11 2023-04-16 07:50:21.000000 report-env-0.0.2/src/report_env.egg-info/top_level.txt
```

### Comparing `report-env-0.0.1/LICENSE` & `report-env-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `report-env-0.0.1/PKG-INFO` & `report-env-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: report-env
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Author-email: swyx <swyx@dontemailme.com>
 Project-URL: Homepage, https://github.com/sw-yx/report-env
 Project-URL: Bug Tracker, https://github.com/sw-yx/report-env/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,7 +18,13 @@
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
 to write your content.
 
 ## Distributing
 
 - `python3 -m build`
 - `python3 -m twine upload dist/*`
+
+
+## thanks
+
+- https://packaging.python.org/en/latest/tutorials/packaging-projects/
+- https://github.com/cs01/pycowsay
```

### Comparing `report-env-0.0.1/src/report_env.egg-info/PKG-INFO` & `report-env-0.0.2/src/report_env.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: report-env
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Author-email: swyx <swyx@dontemailme.com>
 Project-URL: Homepage, https://github.com/sw-yx/report-env
 Project-URL: Bug Tracker, https://github.com/sw-yx/report-env/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,7 +18,13 @@
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
 to write your content.
 
 ## Distributing
 
 - `python3 -m build`
 - `python3 -m twine upload dist/*`
+
+
+## thanks
+
+- https://packaging.python.org/en/latest/tutorials/packaging-projects/
+- https://github.com/cs01/pycowsay
```

