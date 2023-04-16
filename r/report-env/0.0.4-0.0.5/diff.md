# Comparing `tmp/report-env-0.0.4.tar.gz` & `tmp/report-env-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "report-env-0.0.4.tar", last modified: Sun Apr 16 08:01:53 2023, max compression
+gzip compressed data, was "report-env-0.0.5.tar", last modified: Sun Apr 16 08:18:22 2023, max compression
```

## Comparing `report-env-0.0.4.tar` & `report-env-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 08:01:53.023997 report-env-0.0.4/
--rw-r--r--   0 swyx       (501) staff       (20)     1090 2023-04-16 07:33:25.000000 report-env-0.0.4/LICENSE
--rw-r--r--   0 swyx       (501) staff       (20)      117 2023-04-16 07:45:18.000000 report-env-0.0.4/MANIFEST.in
--rw-r--r--   0 swyx       (501) staff       (20)      853 2023-04-16 08:01:53.023862 report-env-0.0.4/PKG-INFO
--rw-r--r--   0 swyx       (501) staff       (20)      364 2023-04-16 07:45:32.000000 report-env-0.0.4/README.md
--rw-r--r--   0 swyx       (501) staff       (20)      532 2023-04-16 08:01:45.000000 report-env-0.0.4/pyproject.toml
--rw-r--r--   0 swyx       (501) staff       (20)       38 2023-04-16 08:01:53.024034 report-env-0.0.4/setup.cfg
-drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 08:01:53.021432 report-env-0.0.4/src/
-drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 08:01:53.023059 report-env-0.0.4/src/report-env/
--rw-r--r--   0 swyx       (501) staff       (20)        0 2023-04-16 07:33:10.000000 report-env-0.0.4/src/report-env/__init__.py
--rw-r--r--   0 swyx       (501) staff       (20)       62 2023-04-16 07:46:10.000000 report-env-0.0.4/src/report-env/__main__.py
--rw-r--r--   0 swyx       (501) staff       (20)      690 2023-04-16 07:46:21.000000 report-env-0.0.4/src/report-env/main.py
-drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 08:01:53.023696 report-env-0.0.4/src/report_env.egg-info/
--rw-r--r--   0 swyx       (501) staff       (20)      853 2023-04-16 08:01:53.000000 report-env-0.0.4/src/report_env.egg-info/PKG-INFO
--rw-r--r--   0 swyx       (501) staff       (20)      273 2023-04-16 08:01:53.000000 report-env-0.0.4/src/report_env.egg-info/SOURCES.txt
--rw-r--r--   0 swyx       (501) staff       (20)        1 2023-04-16 08:01:53.000000 report-env-0.0.4/src/report_env.egg-info/dependency_links.txt
--rw-r--r--   0 swyx       (501) staff       (20)       11 2023-04-16 08:01:53.000000 report-env-0.0.4/src/report_env.egg-info/top_level.txt
+drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 08:18:22.620761 report-env-0.0.5/
+-rw-r--r--   0 swyx       (501) staff       (20)     1090 2023-04-16 07:33:25.000000 report-env-0.0.5/LICENSE
+-rw-r--r--   0 swyx       (501) staff       (20)      117 2023-04-16 07:45:18.000000 report-env-0.0.5/MANIFEST.in
+-rw-r--r--   0 swyx       (501) staff       (20)      827 2023-04-16 08:18:22.620639 report-env-0.0.5/PKG-INFO
+-rw-r--r--   0 swyx       (501) staff       (20)      501 2023-04-16 08:11:25.000000 report-env-0.0.5/README.md
+drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 08:18:22.619746 report-env-0.0.5/report-env/
+-rw-r--r--   0 swyx       (501) staff       (20)        0 2023-04-16 07:33:10.000000 report-env-0.0.5/report-env/__init__.py
+-rw-r--r--   0 swyx       (501) staff       (20)       62 2023-04-16 07:46:10.000000 report-env-0.0.5/report-env/__main__.py
+-rw-r--r--   0 swyx       (501) staff       (20)      688 2023-04-16 08:18:07.000000 report-env-0.0.5/report-env/main.py
+drwxr-xr-x   0 swyx       (501) staff       (20)        0 2023-04-16 08:18:22.620460 report-env-0.0.5/report_env.egg-info/
+-rw-r--r--   0 swyx       (501) staff       (20)      827 2023-04-16 08:18:22.000000 report-env-0.0.5/report_env.egg-info/PKG-INFO
+-rw-r--r--   0 swyx       (501) staff       (20)      309 2023-04-16 08:18:22.000000 report-env-0.0.5/report_env.egg-info/SOURCES.txt
+-rw-r--r--   0 swyx       (501) staff       (20)        1 2023-04-16 08:18:22.000000 report-env-0.0.5/report_env.egg-info/dependency_links.txt
+-rw-r--r--   0 swyx       (501) staff       (20)       52 2023-04-16 08:18:22.000000 report-env-0.0.5/report_env.egg-info/entry_points.txt
+-rw-r--r--   0 swyx       (501) staff       (20)        1 2023-04-16 08:18:22.000000 report-env-0.0.5/report_env.egg-info/not-zip-safe
+-rw-r--r--   0 swyx       (501) staff       (20)       11 2023-04-16 08:18:22.000000 report-env-0.0.5/report_env.egg-info/top_level.txt
+-rw-r--r--   0 swyx       (501) staff       (20)       38 2023-04-16 08:18:22.620802 report-env-0.0.5/setup.cfg
+-rw-r--r--   0 swyx       (501) staff       (20)     2033 2023-04-16 08:17:09.000000 report-env-0.0.5/setup.py
```

### Comparing `report-env-0.0.4/LICENSE` & `report-env-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `report-env-0.0.4/PKG-INFO` & `report-env-0.0.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: report-env
-Version: 0.0.4
-Summary: A small example package
-Author-email: swyx <swyx@dontemailme.com>
-Project-URL: Homepage, https://github.com/sw-yx/report-env
-Project-URL: Bug Tracker, https://github.com/sw-yx/report-env/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Version: 0.0.5
+Home-page: https://github.com/sw-yx/report-env
+Author: swyx
+Author-email: swyx@dontemailme.com
+License: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Example Package
 
 This is a simple example package. You can use
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
 to write your content.
 
 ## Distributing
 
+- failed to use poetry to bundle - got `/Users/swyx/Desktop/Work/env-info/report_env does not contain any element` error and couldnt fix
 - `python3 -m build`
 - `python3 -m twine upload dist/*`
 
 
 ## thanks
 
 - https://packaging.python.org/en/latest/tutorials/packaging-projects/
```

### Comparing `report-env-0.0.4/src/report-env/main.py` & `report-env-0.0.5/report-env/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import sys
 from textwrap import dedent
 
 
-__version__ = "0.0.0.1"
+__version__ = "0.0.5"
 
 
 def main():
     if "--version" in sys.argv[1:]:
         print(__version__)
         exit(0)
     elif "--help" in sys.argv[1:]:
```

### Comparing `report-env-0.0.4/src/report_env.egg-info/PKG-INFO` & `report-env-0.0.5/report_env.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: report-env
-Version: 0.0.4
-Summary: A small example package
-Author-email: swyx <swyx@dontemailme.com>
-Project-URL: Homepage, https://github.com/sw-yx/report-env
-Project-URL: Bug Tracker, https://github.com/sw-yx/report-env/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Version: 0.0.5
+Home-page: https://github.com/sw-yx/report-env
+Author: swyx
+Author-email: swyx@dontemailme.com
+License: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Example Package
 
 This is a simple example package. You can use
 [Github-flavored Markdown](https://guides.github.com/features/mastering-markdown/)
 to write your content.
 
 ## Distributing
 
+- failed to use poetry to bundle - got `/Users/swyx/Desktop/Work/env-info/report_env does not contain any element` error and couldnt fix
 - `python3 -m build`
 - `python3 -m twine upload dist/*`
 
 
 ## thanks
 
 - https://packaging.python.org/en/latest/tutorials/packaging-projects/
```

