# Comparing `tmp/kicad_package_manager-0.0.5.tar.gz` & `tmp/kicad_package_manager-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kicad_package_manager-0.0.5.tar", last modified: Sun Apr 16 01:41:45 2023, max compression
+gzip compressed data, was "kicad_package_manager-0.0.6.tar", last modified: Sun Apr 16 01:44:40 2023, max compression
```

## Comparing `kicad_package_manager-0.0.5.tar` & `kicad_package_manager-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:41:45.448172 kicad_package_manager-0.0.5/
--rwxrwxrwx   0 root         (0) root         (0)     3407 2023-04-16 01:41:45.445838 kicad_package_manager-0.0.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1938 2023-04-15 20:55:43.000000 kicad_package_manager-0.0.5/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:41:45.334321 kicad_package_manager-0.0.5/kicad_package_manager/
--rwxrwxrwx   0 root         (0) root         (0)       14 2023-04-16 00:09:47.000000 kicad_package_manager-0.0.5/kicad_package_manager/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      651 2023-04-15 08:32:16.000000 kicad_package_manager-0.0.5/kicad_package_manager/config.py
--rwxrwxrwx   0 root         (0) root         (0)      504 2023-04-16 01:05:16.000000 kicad_package_manager-0.0.5/kicad_package_manager/init.py
--rwxrwxrwx   0 root         (0) root         (0)     1899 2023-04-16 01:34:38.000000 kicad_package_manager-0.0.5/kicad_package_manager/install.py
--rwxrwxrwx   0 root         (0) root         (0)      959 2023-04-16 01:40:45.000000 kicad_package_manager-0.0.5/kicad_package_manager/kicad_project_tables.py
--rwxrwxrwx   0 root         (0) root         (0)      550 2023-04-16 01:05:45.000000 kicad_package_manager-0.0.5/kicad_package_manager/kpm.py
--rwxrwxrwx   0 root         (0) root         (0)     1750 2023-04-16 01:30:17.000000 kicad_package_manager-0.0.5/kicad_package_manager/registry.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:41:45.429935 kicad_package_manager-0.0.5/kicad_package_manager.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3407 2023-04-16 01:41:45.000000 kicad_package_manager-0.0.5/kicad_package_manager.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      528 2023-04-16 01:41:45.000000 kicad_package_manager-0.0.5/kicad_package_manager.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-16 01:41:45.000000 kicad_package_manager-0.0.5/kicad_package_manager.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       56 2023-04-16 01:41:45.000000 kicad_package_manager-0.0.5/kicad_package_manager.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2023-04-16 01:41:45.000000 kicad_package_manager-0.0.5/kicad_package_manager.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-04-16 01:41:45.000000 kicad_package_manager-0.0.5/kicad_package_manager.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-16 01:41:45.448884 kicad_package_manager-0.0.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3832 2023-04-16 01:41:24.000000 kicad_package_manager-0.0.5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:44:40.156315 kicad_package_manager-0.0.6/
+-rwxrwxrwx   0 root         (0) root         (0)     3407 2023-04-16 01:44:40.152876 kicad_package_manager-0.0.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1938 2023-04-15 20:55:43.000000 kicad_package_manager-0.0.6/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:44:39.977726 kicad_package_manager-0.0.6/kicad_package_manager/
+-rwxrwxrwx   0 root         (0) root         (0)       14 2023-04-16 00:09:47.000000 kicad_package_manager-0.0.6/kicad_package_manager/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      651 2023-04-15 08:32:16.000000 kicad_package_manager-0.0.6/kicad_package_manager/config.py
+-rwxrwxrwx   0 root         (0) root         (0)      504 2023-04-16 01:05:16.000000 kicad_package_manager-0.0.6/kicad_package_manager/init.py
+-rwxrwxrwx   0 root         (0) root         (0)     1862 2023-04-16 01:44:17.000000 kicad_package_manager-0.0.6/kicad_package_manager/install.py
+-rwxrwxrwx   0 root         (0) root         (0)      959 2023-04-16 01:40:45.000000 kicad_package_manager-0.0.6/kicad_package_manager/kicad_project_tables.py
+-rwxrwxrwx   0 root         (0) root         (0)      550 2023-04-16 01:05:45.000000 kicad_package_manager-0.0.6/kicad_package_manager/kpm.py
+-rwxrwxrwx   0 root         (0) root         (0)     1750 2023-04-16 01:30:17.000000 kicad_package_manager-0.0.6/kicad_package_manager/registry.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:44:40.129820 kicad_package_manager-0.0.6/kicad_package_manager.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3407 2023-04-16 01:44:39.000000 kicad_package_manager-0.0.6/kicad_package_manager.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      528 2023-04-16 01:44:39.000000 kicad_package_manager-0.0.6/kicad_package_manager.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-16 01:44:39.000000 kicad_package_manager-0.0.6/kicad_package_manager.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       56 2023-04-16 01:44:39.000000 kicad_package_manager-0.0.6/kicad_package_manager.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-04-16 01:44:39.000000 kicad_package_manager-0.0.6/kicad_package_manager.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-04-16 01:44:39.000000 kicad_package_manager-0.0.6/kicad_package_manager.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-16 01:44:40.158982 kicad_package_manager-0.0.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3832 2023-04-16 01:44:23.000000 kicad_package_manager-0.0.6/setup.py
```

### Comparing `kicad_package_manager-0.0.5/PKG-INFO` & `kicad_package_manager-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kicad_package_manager
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package manager for KiCad projects
 Home-page: https://github.com/danroblewis/kicad-package-manager
 Author: Daniel Lewis
 Author-email: daniel.robert.lewis@gmail.com
 License: MIT
 Description: 
         # KiCad Package Manager
```

### Comparing `kicad_package_manager-0.0.5/README.md` & `kicad_package_manager-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.5/kicad_package_manager/config.py` & `kicad_package_manager-0.0.6/kicad_package_manager/config.py`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.5/kicad_package_manager/install.py` & `kicad_package_manager-0.0.6/kicad_package_manager/install.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,19 +52,17 @@
 	res = requests.get(zip_url)
 	r = zipfile.ZipFile(io.BytesIO(res.content)).extractall(package_dir)
 
 
 def install_libraries():
 	# link symbol files
 	symfiles = glob.glob("**/*.kicad_sym", recursive=True)
-	print(symfiles)
 	kicad_project_tables.write_sym_lib_table(symfiles)
 
 	# link footprint files
 	footfiles = glob.glob("**/*.kicad_mod", recursive=True)
-	print(footfiles)
 	kicad_project_tables.write_fp_lib_table(footfiles)
 
 	# install 3d models
 	# install spice models
 	# install plugins
```

### Comparing `kicad_package_manager-0.0.5/kicad_package_manager/kicad_project_tables.py` & `kicad_package_manager-0.0.6/kicad_package_manager/kicad_project_tables.py`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.5/kicad_package_manager/kpm.py` & `kicad_package_manager-0.0.6/kicad_package_manager/kpm.py`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.5/kicad_package_manager/registry.py` & `kicad_package_manager-0.0.6/kicad_package_manager/registry.py`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.5/kicad_package_manager.egg-info/PKG-INFO` & `kicad_package_manager-0.0.6/kicad_package_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kicad-package-manager
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package manager for KiCad projects
 Home-page: https://github.com/danroblewis/kicad-package-manager
 Author: Daniel Lewis
 Author-email: daniel.robert.lewis@gmail.com
 License: MIT
 Description: 
         # KiCad Package Manager
```

### Comparing `kicad_package_manager-0.0.5/kicad_package_manager.egg-info/SOURCES.txt` & `kicad_package_manager-0.0.6/kicad_package_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.5/setup.py` & `kicad_package_manager-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'kicad_package_manager'
 DESCRIPTION = 'A package manager for KiCad projects'
 URL = 'https://github.com/danroblewis/kicad-package-manager'
 EMAIL = 'daniel.robert.lewis@gmail.com'
 AUTHOR = 'Daniel Lewis'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'sexpdata'
 ]
```

