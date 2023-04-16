# Comparing `tmp/cagen-0.2.0a4.tar.gz` & `tmp/cagen-0.2.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cagen-0.2.0a4.tar", last modified: Sun Apr 16 21:03:17 2023, max compression
+gzip compressed data, was "cagen-0.2.0a5.tar", last modified: Sun Apr 16 21:08:23 2023, max compression
```

## Comparing `cagen-0.2.0a4.tar` & `cagen-0.2.0a5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-16 21:03:17.959013 cagen-0.2.0a4/
--rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0a4/MANIFEST.in
--rw-r--r--   0 xan       (1000) xan       (1000)     4049 2023-04-16 21:03:17.959013 cagen-0.2.0a4/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)     3314 2023-04-16 10:42:06.000000 cagen-0.2.0a4/README.md
--rw-r--r--   0 xan       (1000) xan       (1000)     1160 2023-04-16 21:03:06.000000 cagen-0.2.0a4/pyproject.toml
--rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-04-16 21:03:17.959013 cagen-0.2.0a4/setup.cfg
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-16 21:03:17.955679 cagen-0.2.0a4/src/
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-16 21:03:17.955679 cagen-0.2.0a4/src/cagen/
--rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0a4/src/cagen/__init__.py
--rw-r--r--   0 xan       (1000) xan       (1000)     4773 2023-04-16 21:02:18.000000 cagen-0.2.0a4/src/cagen/cmd.py
--rw-r--r--   0 xan       (1000) xan       (1000)     8288 2023-04-16 21:01:28.000000 cagen-0.2.0a4/src/cagen/libcagen.py
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-16 21:03:17.959013 cagen-0.2.0a4/src/cagen/templates/
--rw-r--r--   0 xan       (1000) xan       (1000)      381 2023-02-09 11:33:44.000000 cagen-0.2.0a4/src/cagen/templates/list.md.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0a4/src/cagen/templates/list.md.tmpl.license
--rw-r--r--   0 xan       (1000) xan       (1000)     1754 2023-01-21 12:38:41.000000 cagen-0.2.0a4/src/cagen/templates/schema.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0a4/src/cagen/templates/schema.tmpl.license
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-16 21:03:17.959013 cagen-0.2.0a4/src/cagen.egg-info/
--rw-r--r--   0 xan       (1000) xan       (1000)     4049 2023-04-16 21:03:17.000000 cagen-0.2.0a4/src/cagen.egg-info/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-04-16 21:03:17.000000 cagen-0.2.0a4/src/cagen.egg-info/SOURCES.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-04-16 21:03:17.000000 cagen-0.2.0a4/src/cagen.egg-info/dependency_links.txt
--rw-r--r--   0 xan       (1000) xan       (1000)      114 2023-04-16 21:03:17.000000 cagen-0.2.0a4/src/cagen.egg-info/entry_points.txt
--rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-04-16 21:03:17.000000 cagen-0.2.0a4/src/cagen.egg-info/requires.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-04-16 21:03:17.000000 cagen-0.2.0a4/src/cagen.egg-info/top_level.txt
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-16 21:08:23.351849 cagen-0.2.0a5/
+-rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0a5/MANIFEST.in
+-rw-r--r--   0 xan       (1000) xan       (1000)     4049 2023-04-16 21:08:23.351849 cagen-0.2.0a5/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)     3314 2023-04-16 10:42:06.000000 cagen-0.2.0a5/README.md
+-rw-r--r--   0 xan       (1000) xan       (1000)     1160 2023-04-16 21:08:18.000000 cagen-0.2.0a5/pyproject.toml
+-rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-04-16 21:08:23.351849 cagen-0.2.0a5/setup.cfg
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-16 21:08:23.348516 cagen-0.2.0a5/src/
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-16 21:08:23.348516 cagen-0.2.0a5/src/cagen/
+-rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0a5/src/cagen/__init__.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     4773 2023-04-16 21:02:18.000000 cagen-0.2.0a5/src/cagen/cmd.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     8287 2023-04-16 21:07:57.000000 cagen-0.2.0a5/src/cagen/libcagen.py
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-16 21:08:23.351849 cagen-0.2.0a5/src/cagen/templates/
+-rw-r--r--   0 xan       (1000) xan       (1000)      381 2023-02-09 11:33:44.000000 cagen-0.2.0a5/src/cagen/templates/list.md.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0a5/src/cagen/templates/list.md.tmpl.license
+-rw-r--r--   0 xan       (1000) xan       (1000)     1754 2023-01-21 12:38:41.000000 cagen-0.2.0a5/src/cagen/templates/schema.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0a5/src/cagen/templates/schema.tmpl.license
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-16 21:08:23.351849 cagen-0.2.0a5/src/cagen.egg-info/
+-rw-r--r--   0 xan       (1000) xan       (1000)     4049 2023-04-16 21:08:23.000000 cagen-0.2.0a5/src/cagen.egg-info/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-04-16 21:08:23.000000 cagen-0.2.0a5/src/cagen.egg-info/SOURCES.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-04-16 21:08:23.000000 cagen-0.2.0a5/src/cagen.egg-info/dependency_links.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)      114 2023-04-16 21:08:23.000000 cagen-0.2.0a5/src/cagen.egg-info/entry_points.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-04-16 21:08:23.000000 cagen-0.2.0a5/src/cagen.egg-info/requires.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-04-16 21:08:23.000000 cagen-0.2.0a5/src/cagen.egg-info/top_level.txt
```

### Comparing `cagen-0.2.0a4/PKG-INFO` & `cagen-0.2.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0a4
+Version: 0.2.0a5
 Summary: A static site generator for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `cagen-0.2.0a4/README.md` & `cagen-0.2.0a5/README.md`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0a4/pyproject.toml` & `cagen-0.2.0a5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [project.scripts]
 cagen = "cagen.cmd:cagen_cli"
 cagen-list = "cagen.cmd:cagen_list"
 cagen-make = "cagen.cmd:cagen_make"
 
 [project]
 name = "cagen"
-version = "0.2.0.alpha-4"
+version = "0.2.0.alpha-5"
 authors = [{'name'="Xavier B."}]
 description = "A static site generator for cmpalgorithms project"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
```

### Comparing `cagen-0.2.0a4/src/cagen/cmd.py` & `cagen-0.2.0a5/src/cagen/cmd.py`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0a4/src/cagen/libcagen.py` & `cagen-0.2.0a5/src/cagen/libcagen.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 It is used in [cagen](https://git.sr.ht/~somenxavierb/cagen/tree/main/item/src/cagen/cagen.py) CLI front-end.
 """
 
 
 ## Python Library imports
 from dataclasses import dataclass
-from typing import Optionali, List
+from typing import Optional, List
 from pprint import pprint
 import os.path
 import itertools
 import types
 
 # External imports
 import frontmatter
```

### Comparing `cagen-0.2.0a4/src/cagen/templates/schema.tmpl` & `cagen-0.2.0a5/src/cagen/templates/schema.tmpl`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0a4/src/cagen.egg-info/PKG-INFO` & `cagen-0.2.0a5/src/cagen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0a4
+Version: 0.2.0a5
 Summary: A static site generator for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

