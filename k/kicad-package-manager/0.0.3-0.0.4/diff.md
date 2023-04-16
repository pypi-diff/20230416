# Comparing `tmp/kicad_package_manager-0.0.3.tar.gz` & `tmp/kicad_package_manager-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kicad_package_manager-0.0.3.tar", last modified: Sun Apr 16 01:18:12 2023, max compression
+gzip compressed data, was "kicad_package_manager-0.0.4.tar", last modified: Sun Apr 16 01:32:36 2023, max compression
```

## Comparing `kicad_package_manager-0.0.3.tar` & `kicad_package_manager-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:18:12.831648 kicad_package_manager-0.0.3/
--rwxrwxrwx   0 root         (0) root         (0)     3407 2023-04-16 01:18:12.829596 kicad_package_manager-0.0.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1938 2023-04-15 20:55:43.000000 kicad_package_manager-0.0.3/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:18:12.711640 kicad_package_manager-0.0.3/kicad_package_manager/
--rwxrwxrwx   0 root         (0) root         (0)       14 2023-04-16 00:09:47.000000 kicad_package_manager-0.0.3/kicad_package_manager/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      651 2023-04-15 08:32:16.000000 kicad_package_manager-0.0.3/kicad_package_manager/config.py
--rwxrwxrwx   0 root         (0) root         (0)      504 2023-04-16 01:05:16.000000 kicad_package_manager-0.0.3/kicad_package_manager/init.py
--rwxrwxrwx   0 root         (0) root         (0)     1899 2023-04-16 01:05:32.000000 kicad_package_manager-0.0.3/kicad_package_manager/install.py
--rwxrwxrwx   0 root         (0) root         (0)      950 2023-04-15 09:19:50.000000 kicad_package_manager-0.0.3/kicad_package_manager/kicad_project_tables.py
--rwxrwxrwx   0 root         (0) root         (0)      550 2023-04-16 01:05:45.000000 kicad_package_manager-0.0.3/kicad_package_manager/kpm.py
--rwxrwxrwx   0 root         (0) root         (0)     1768 2023-04-16 01:16:56.000000 kicad_package_manager-0.0.3/kicad_package_manager/registry.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:18:12.811969 kicad_package_manager-0.0.3/kicad_package_manager.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3407 2023-04-16 01:18:12.000000 kicad_package_manager-0.0.3/kicad_package_manager.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      528 2023-04-16 01:18:12.000000 kicad_package_manager-0.0.3/kicad_package_manager.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-16 01:18:12.000000 kicad_package_manager-0.0.3/kicad_package_manager.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       56 2023-04-16 01:18:12.000000 kicad_package_manager-0.0.3/kicad_package_manager.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2023-04-16 01:18:12.000000 kicad_package_manager-0.0.3/kicad_package_manager.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       22 2023-04-16 01:18:12.000000 kicad_package_manager-0.0.3/kicad_package_manager.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-16 01:18:12.832533 kicad_package_manager-0.0.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     3832 2023-04-16 01:17:25.000000 kicad_package_manager-0.0.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:32:36.388634 kicad_package_manager-0.0.4/
+-rwxrwxrwx   0 root         (0) root         (0)     3407 2023-04-16 01:32:36.386517 kicad_package_manager-0.0.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1938 2023-04-15 20:55:43.000000 kicad_package_manager-0.0.4/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:32:36.282760 kicad_package_manager-0.0.4/kicad_package_manager/
+-rwxrwxrwx   0 root         (0) root         (0)       14 2023-04-16 00:09:47.000000 kicad_package_manager-0.0.4/kicad_package_manager/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      651 2023-04-15 08:32:16.000000 kicad_package_manager-0.0.4/kicad_package_manager/config.py
+-rwxrwxrwx   0 root         (0) root         (0)      504 2023-04-16 01:05:16.000000 kicad_package_manager-0.0.4/kicad_package_manager/init.py
+-rwxrwxrwx   0 root         (0) root         (0)     1862 2023-04-16 01:30:03.000000 kicad_package_manager-0.0.4/kicad_package_manager/install.py
+-rwxrwxrwx   0 root         (0) root         (0)      950 2023-04-15 09:19:50.000000 kicad_package_manager-0.0.4/kicad_package_manager/kicad_project_tables.py
+-rwxrwxrwx   0 root         (0) root         (0)      550 2023-04-16 01:05:45.000000 kicad_package_manager-0.0.4/kicad_package_manager/kpm.py
+-rwxrwxrwx   0 root         (0) root         (0)     1750 2023-04-16 01:30:17.000000 kicad_package_manager-0.0.4/kicad_package_manager/registry.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-16 01:32:36.370358 kicad_package_manager-0.0.4/kicad_package_manager.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     3407 2023-04-16 01:32:35.000000 kicad_package_manager-0.0.4/kicad_package_manager.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      528 2023-04-16 01:32:36.000000 kicad_package_manager-0.0.4/kicad_package_manager.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2023-04-16 01:32:35.000000 kicad_package_manager-0.0.4/kicad_package_manager.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       56 2023-04-16 01:32:35.000000 kicad_package_manager-0.0.4/kicad_package_manager.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2023-04-16 01:32:35.000000 kicad_package_manager-0.0.4/kicad_package_manager.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       22 2023-04-16 01:32:35.000000 kicad_package_manager-0.0.4/kicad_package_manager.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2023-04-16 01:32:36.389572 kicad_package_manager-0.0.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     3832 2023-04-16 01:32:28.000000 kicad_package_manager-0.0.4/setup.py
```

### Comparing `kicad_package_manager-0.0.3/PKG-INFO` & `kicad_package_manager-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kicad_package_manager
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package manager for KiCad projects
 Home-page: https://github.com/danroblewis/kicad-package-manager
 Author: Daniel Lewis
 Author-email: daniel.robert.lewis@gmail.com
 License: MIT
 Description: 
         # KiCad Package Manager
```

### Comparing `kicad_package_manager-0.0.3/README.md` & `kicad_package_manager-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.3/kicad_package_manager/config.py` & `kicad_package_manager-0.0.4/kicad_package_manager/config.py`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.3/kicad_package_manager/install.py` & `kicad_package_manager-0.0.4/kicad_package_manager/install.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,25 +9,23 @@
 import glob
 import shutil
 
 
 def run_command(args):
 	package_ref = args.package_ref
 
-	found_packages = {}
-
 	if package_ref == '.':
 		c = config.parse_config()
-		deps = explore_deps(c.name, c.version)
+		deps = {}
+		for depname, depversion in c.dependencies.items():
+			explore_deps(depname, depversion, deps)
 		install_deps(deps)
 
 
 def explore_deps(name, version, found_packages={}):
-	print('explore_deps', name, version)
-
 	if name in found_packages:
 		if found_packages[name] != version:
 			raise Exception(f"incompatible version for {name}: {version}, committed version is {found_packages[name]['version']}")
 		else:
 			return found_packages
 
 	release = get_release_for(name, version)
@@ -48,18 +46,15 @@
 	install_libraries()
 
 
 def install_package(name, version, zip_url):
 	package_dir = f"./kpm_modules/{name}@{version}/"
 	os.makedirs(package_dir, exist_ok=True)
 	res = requests.get(zip_url)
-	print(zip_url)
-	print(res)
 	r = zipfile.ZipFile(io.BytesIO(res.content)).extractall(package_dir)
-	print(r)
 
 
 def install_libraries():
 	# link symbol files
 	symfiles = glob.glob("**/*.kicad_sym", recursive=True)
 	kicad_project_tables.write_sym_lib_table(symfiles)
```

### Comparing `kicad_package_manager-0.0.3/kicad_package_manager/kicad_project_tables.py` & `kicad_package_manager-0.0.4/kicad_package_manager/kicad_project_tables.py`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.3/kicad_package_manager/kpm.py` & `kicad_package_manager-0.0.4/kicad_package_manager/kpm.py`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.3/kicad_package_manager/registry.py` & `kicad_package_manager-0.0.4/kicad_package_manager/registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 def get_release_for(package_name, version):
 	if package_name not in temporary_registry:
 		raise Exception(f"no package exists by name {package_name}")
 
 	releases = temporary_registry[package_name]['releases']
 	found = None
 	for release in releases:
-		print(release)
 		if release['version'] == version:
 			return release
 
 
 def get_zip_url_for(package_name, version):
 	release = get_release_for(package_name, version)
 	return release['artifact_url']
```

### Comparing `kicad_package_manager-0.0.3/kicad_package_manager.egg-info/PKG-INFO` & `kicad_package_manager-0.0.4/kicad_package_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kicad-package-manager
-Version: 0.0.3
+Version: 0.0.4
 Summary: A package manager for KiCad projects
 Home-page: https://github.com/danroblewis/kicad-package-manager
 Author: Daniel Lewis
 Author-email: daniel.robert.lewis@gmail.com
 License: MIT
 Description: 
         # KiCad Package Manager
```

### Comparing `kicad_package_manager-0.0.3/kicad_package_manager.egg-info/SOURCES.txt` & `kicad_package_manager-0.0.4/kicad_package_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kicad_package_manager-0.0.3/setup.py` & `kicad_package_manager-0.0.4/setup.py`

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
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'sexpdata'
 ]
```

