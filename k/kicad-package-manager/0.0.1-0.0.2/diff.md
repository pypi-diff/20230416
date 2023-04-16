# Comparing `tmp/kicad-package-manager-0.0.1.tar.gz` & `tmp/kicad_package_manager-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kicad-package-manager-0.0.1.tar", last modified: Sun Apr 16 00:33:09 2023, max compression
+gzip compressed data, was "kicad_package_manager-0.0.2.tar", last modified: Sun Apr 16 01:08:58 2023, max compression
```

## Comparing `kicad-package-manager-0.0.1.tar` & `kicad_package_manager-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 00:33:09.020765 kicad-package-manager-0.0.1/
--rwxrwxrwx   0 root         (0) root         (0)     3407 2023-04-16 00:33:09.017767 kicad-package-manager-0.0.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1938 2023-04-15 20:55:43.000000 kicad-package-manager-0.0.1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 00:33:08.903903 kicad-package-manager-0.0.1/kicad_package_manager.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3407 2023-04-16 00:33:08.000000 kicad-package-manager-0.0.1/kicad_package_manager.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      314 2023-04-16 00:33:08.000000 kicad-package-manager-0.0.1/kicad_package_manager.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-16 00:33:08.000000 kicad-package-manager-0.0.1/kicad_package_manager.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)        4 2023-04-16 00:33:08.000000 kicad-package-manager-0.0.1/kicad_package_manager.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)      626 2023-04-16 00:11:44.000000 kicad-package-manager-0.0.1/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-16 00:33:09.021773 kicad-package-manager-0.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3828 2023-04-16 00:32:29.000000 kicad-package-manager-0.0.1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 00:33:08.999810 kicad-package-manager-0.0.1/src/
--rwxrwxrwx   0 root         (0) root         (0)       14 2023-04-16 00:09:47.000000 kicad-package-manager-0.0.1/src/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      651 2023-04-15 08:32:16.000000 kicad-package-manager-0.0.1/src/config.py
--rwxrwxrwx   0 root         (0) root         (0)      497 2023-04-15 08:30:57.000000 kicad-package-manager-0.0.1/src/init.py
--rwxrwxrwx   0 root         (0) root         (0)     1884 2023-04-15 09:39:06.000000 kicad-package-manager-0.0.1/src/install.py
--rwxrwxrwx   0 root         (0) root         (0)      950 2023-04-15 09:19:50.000000 kicad-package-manager-0.0.1/src/kicad_project_tables.py
--rwxrwxrwx   0 root         (0) root         (0)      694 2023-04-15 08:58:24.000000 kicad-package-manager-0.0.1/src/registry.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:08:58.551513 kicad_package_manager-0.0.2/
+-rwxrwxrwx   0 root         (0) root         (0)     3407 2023-04-16 01:08:58.549021 kicad_package_manager-0.0.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1938 2023-04-15 20:55:43.000000 kicad_package_manager-0.0.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:08:58.436166 kicad_package_manager-0.0.2/kicad_package_manager/
+-rwxrwxrwx   0 root         (0) root         (0)       14 2023-04-16 00:09:47.000000 kicad_package_manager-0.0.2/kicad_package_manager/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      651 2023-04-15 08:32:16.000000 kicad_package_manager-0.0.2/kicad_package_manager/config.py
+-rwxrwxrwx   0 root         (0) root         (0)      504 2023-04-16 01:05:16.000000 kicad_package_manager-0.0.2/kicad_package_manager/init.py
+-rwxrwxrwx   0 root         (0) root         (0)     1899 2023-04-16 01:05:32.000000 kicad_package_manager-0.0.2/kicad_package_manager/install.py
+-rwxrwxrwx   0 root         (0) root         (0)      950 2023-04-15 09:19:50.000000 kicad_package_manager-0.0.2/kicad_package_manager/kicad_project_tables.py
+-rwxrwxrwx   0 root         (0) root         (0)      550 2023-04-16 01:05:45.000000 kicad_package_manager-0.0.2/kicad_package_manager/kpm.py
+-rwxrwxrwx   0 root         (0) root         (0)      694 2023-04-15 08:58:24.000000 kicad_package_manager-0.0.2/kicad_package_manager/registry.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:08:58.532704 kicad_package_manager-0.0.2/kicad_package_manager.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3407 2023-04-16 01:08:58.000000 kicad_package_manager-0.0.2/kicad_package_manager.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      528 2023-04-16 01:08:58.000000 kicad_package_manager-0.0.2/kicad_package_manager.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-16 01:08:58.000000 kicad_package_manager-0.0.2/kicad_package_manager.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       56 2023-04-16 01:08:58.000000 kicad_package_manager-0.0.2/kicad_package_manager.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-04-16 01:08:58.000000 kicad_package_manager-0.0.2/kicad_package_manager.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-04-16 01:08:58.000000 kicad_package_manager-0.0.2/kicad_package_manager.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-16 01:08:58.552138 kicad_package_manager-0.0.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3832 2023-04-16 01:08:09.000000 kicad_package_manager-0.0.2/setup.py
```

### Comparing `kicad-package-manager-0.0.1/PKG-INFO` & `kicad_package_manager-0.0.2/kicad_package_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kicad-package-manager
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package manager for KiCad projects
 Home-page: https://github.com/danroblewis/kicad-package-manager
 Author: Daniel Lewis
 Author-email: daniel.robert.lewis@gmail.com
 License: MIT
 Description: 
         # KiCad Package Manager
```

### Comparing `kicad-package-manager-0.0.1/README.md` & `kicad_package_manager-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `kicad-package-manager-0.0.1/kicad_package_manager.egg-info/PKG-INFO` & `kicad_package_manager-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: kicad-package-manager
-Version: 0.0.1
+Name: kicad_package_manager
+Version: 0.0.2
 Summary: A package manager for KiCad projects
 Home-page: https://github.com/danroblewis/kicad-package-manager
 Author: Daniel Lewis
 Author-email: daniel.robert.lewis@gmail.com
 License: MIT
 Description: 
         # KiCad Package Manager
```

### Comparing `kicad-package-manager-0.0.1/setup.py` & `kicad_package_manager-0.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,25 +8,26 @@
 import os
 import sys
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
 # Package meta-data.
-NAME = 'kicad-package-manager'
+NAME = 'kicad_package_manager'
 DESCRIPTION = 'A package manager for KiCad projects'
 URL = 'https://github.com/danroblewis/kicad-package-manager'
 EMAIL = 'daniel.robert.lewis@gmail.com'
 AUTHOR = 'Daniel Lewis'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
-    # 'requests', 'maya', 'records',
+    'requests',
+    'sexpdata'
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
@@ -103,17 +104,17 @@
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
     # If your package is a single module, use this instead of 'packages':
     # py_modules=['mypackage'],
 
-    # entry_points={
-    #     'console_scripts': ['mycli=mymodule:cli'],
-    # },
+    entry_points={
+        'console_scripts': ['kpm=kicad_package_manager.kpm:main'],
+    },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
     license='MIT',
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
```

### Comparing `kicad-package-manager-0.0.1/src/config.py` & `kicad_package_manager-0.0.2/kicad_package_manager/config.py`

 * *Files identical despite different names*

### Comparing `kicad-package-manager-0.0.1/src/install.py` & `kicad_package_manager-0.0.2/kicad_package_manager/install.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
-import config
+from . import config
 import requests
-from registry import get_release_for
+from .registry import get_release_for
 import os
 import io
 import zipfile
-import kicad_project_tables
+from . import kicad_project_tables
 import glob
 import shutil
 
 
 def run_command(args):
 	package_ref = args.package_ref
```

### Comparing `kicad-package-manager-0.0.1/src/kicad_project_tables.py` & `kicad_package_manager-0.0.2/kicad_package_manager/kicad_project_tables.py`

 * *Files identical despite different names*

### Comparing `kicad-package-manager-0.0.1/src/registry.py` & `kicad_package_manager-0.0.2/kicad_package_manager/registry.py`

 * *Files identical despite different names*

