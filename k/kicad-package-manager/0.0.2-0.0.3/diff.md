# Comparing `tmp/kicad_package_manager-0.0.2.tar.gz` & `tmp/kicad_package_manager-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kicad_package_manager-0.0.2.tar", last modified: Sun Apr 16 01:08:58 2023, max compression
+gzip compressed data, was "kicad_package_manager-0.0.3.tar", last modified: Sun Apr 16 01:18:12 2023, max compression
```

## Comparing `kicad_package_manager-0.0.2.tar` & `kicad_package_manager-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:08:58.551513 kicad_package_manager-0.0.2/
--rwxrwxrwx   0 root         (0) root         (0)     3407 2023-04-16 01:08:58.549021 kicad_package_manager-0.0.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1938 2023-04-15 20:55:43.000000 kicad_package_manager-0.0.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:08:58.436166 kicad_package_manager-0.0.2/kicad_package_manager/
--rwxrwxrwx   0 root         (0) root         (0)       14 2023-04-16 00:09:47.000000 kicad_package_manager-0.0.2/kicad_package_manager/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      651 2023-04-15 08:32:16.000000 kicad_package_manager-0.0.2/kicad_package_manager/config.py
--rwxrwxrwx   0 root         (0) root         (0)      504 2023-04-16 01:05:16.000000 kicad_package_manager-0.0.2/kicad_package_manager/init.py
--rwxrwxrwx   0 root         (0) root         (0)     1899 2023-04-16 01:05:32.000000 kicad_package_manager-0.0.2/kicad_package_manager/install.py
--rwxrwxrwx   0 root         (0) root         (0)      950 2023-04-15 09:19:50.000000 kicad_package_manager-0.0.2/kicad_package_manager/kicad_project_tables.py
--rwxrwxrwx   0 root         (0) root         (0)      550 2023-04-16 01:05:45.000000 kicad_package_manager-0.0.2/kicad_package_manager/kpm.py
--rwxrwxrwx   0 root         (0) root         (0)      694 2023-04-15 08:58:24.000000 kicad_package_manager-0.0.2/kicad_package_manager/registry.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:08:58.532704 kicad_package_manager-0.0.2/kicad_package_manager.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3407 2023-04-16 01:08:58.000000 kicad_package_manager-0.0.2/kicad_package_manager.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      528 2023-04-16 01:08:58.000000 kicad_package_manager-0.0.2/kicad_package_manager.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-16 01:08:58.000000 kicad_package_manager-0.0.2/kicad_package_manager.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       56 2023-04-16 01:08:58.000000 kicad_package_manager-0.0.2/kicad_package_manager.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2023-04-16 01:08:58.000000 kicad_package_manager-0.0.2/kicad_package_manager.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-04-16 01:08:58.000000 kicad_package_manager-0.0.2/kicad_package_manager.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-16 01:08:58.552138 kicad_package_manager-0.0.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3832 2023-04-16 01:08:09.000000 kicad_package_manager-0.0.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:18:12.831648 kicad_package_manager-0.0.3/
+-rwxrwxrwx   0 root         (0) root         (0)     3407 2023-04-16 01:18:12.829596 kicad_package_manager-0.0.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1938 2023-04-15 20:55:43.000000 kicad_package_manager-0.0.3/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:18:12.711640 kicad_package_manager-0.0.3/kicad_package_manager/
+-rwxrwxrwx   0 root         (0) root         (0)       14 2023-04-16 00:09:47.000000 kicad_package_manager-0.0.3/kicad_package_manager/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      651 2023-04-15 08:32:16.000000 kicad_package_manager-0.0.3/kicad_package_manager/config.py
+-rwxrwxrwx   0 root         (0) root         (0)      504 2023-04-16 01:05:16.000000 kicad_package_manager-0.0.3/kicad_package_manager/init.py
+-rwxrwxrwx   0 root         (0) root         (0)     1899 2023-04-16 01:05:32.000000 kicad_package_manager-0.0.3/kicad_package_manager/install.py
+-rwxrwxrwx   0 root         (0) root         (0)      950 2023-04-15 09:19:50.000000 kicad_package_manager-0.0.3/kicad_package_manager/kicad_project_tables.py
+-rwxrwxrwx   0 root         (0) root         (0)      550 2023-04-16 01:05:45.000000 kicad_package_manager-0.0.3/kicad_package_manager/kpm.py
+-rwxrwxrwx   0 root         (0) root         (0)     1768 2023-04-16 01:16:56.000000 kicad_package_manager-0.0.3/kicad_package_manager/registry.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:18:12.811969 kicad_package_manager-0.0.3/kicad_package_manager.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3407 2023-04-16 01:18:12.000000 kicad_package_manager-0.0.3/kicad_package_manager.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      528 2023-04-16 01:18:12.000000 kicad_package_manager-0.0.3/kicad_package_manager.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-16 01:18:12.000000 kicad_package_manager-0.0.3/kicad_package_manager.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       56 2023-04-16 01:18:12.000000 kicad_package_manager-0.0.3/kicad_package_manager.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-04-16 01:18:12.000000 kicad_package_manager-0.0.3/kicad_package_manager.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-04-16 01:18:12.000000 kicad_package_manager-0.0.3/kicad_package_manager.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-16 01:18:12.832533 kicad_package_manager-0.0.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3832 2023-04-16 01:17:25.000000 kicad_package_manager-0.0.3/setup.py
```

### Comparing `kicad_package_manager-0.0.2/PKG-INFO` & `kicad_package_manager-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kicad_package_manager
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package manager for KiCad projects
 Home-page: https://github.com/danroblewis/kicad-package-manager
 Author: Daniel Lewis
 Author-email: daniel.robert.lewis@gmail.com
 License: MIT
 Description: 
         # KiCad Package Manager
```

### Comparing `kicad_package_manager-0.0.2/README.md` & `kicad_package_manager-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.2/kicad_package_manager/config.py` & `kicad_package_manager-0.0.3/kicad_package_manager/config.py`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.2/kicad_package_manager/install.py` & `kicad_package_manager-0.0.3/kicad_package_manager/install.py`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.2/kicad_package_manager/kicad_project_tables.py` & `kicad_package_manager-0.0.3/kicad_package_manager/kicad_project_tables.py`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.2/kicad_package_manager/kpm.py` & `kicad_package_manager-0.0.3/kicad_package_manager/kpm.py`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.2/kicad_package_manager.egg-info/PKG-INFO` & `kicad_package_manager-0.0.3/kicad_package_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kicad-package-manager
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package manager for KiCad projects
 Home-page: https://github.com/danroblewis/kicad-package-manager
 Author: Daniel Lewis
 Author-email: daniel.robert.lewis@gmail.com
 License: MIT
 Description: 
         # KiCad Package Manager
```

### Comparing `kicad_package_manager-0.0.2/kicad_package_manager.egg-info/SOURCES.txt` & `kicad_package_manager-0.0.3/kicad_package_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.2/setup.py` & `kicad_package_manager-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'kicad_package_manager'
 DESCRIPTION = 'A package manager for KiCad projects'
 URL = 'https://github.com/danroblewis/kicad-package-manager'
 EMAIL = 'daniel.robert.lewis@gmail.com'
 AUTHOR = 'Daniel Lewis'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'sexpdata'
 ]
```

