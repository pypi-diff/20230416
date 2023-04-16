# Comparing `tmp/otoe-0.0.5.tar.gz` & `tmp/otoe-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otoe-0.0.5.tar", last modified: Sun Apr 16 20:40:27 2023, max compression
+gzip compressed data, was "otoe-0.0.6.tar", last modified: Sun Apr 16 20:44:09 2023, max compression
```

## Comparing `otoe-0.0.5.tar` & `otoe-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:40:27.302410 otoe-0.0.5/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      960 2023-04-16 20:40:27.302284 otoe-0.0.5/PKG-INFO
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      637 2023-04-10 20:00:48.000000 otoe-0.0.5/README.md
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:40:27.301141 otoe-0.0.5/otoe/
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:40:27.301197 otoe-0.0.5/otoe/src/
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:40:27.302110 otoe-0.0.5/otoe/src/otoe.egg-info/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      960 2023-04-16 20:40:27.000000 otoe-0.0.5/otoe/src/otoe.egg-info/PKG-INFO
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      206 2023-04-16 20:40:27.000000 otoe-0.0.5/otoe/src/otoe.egg-info/SOURCES.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)        1 2023-04-16 20:40:27.000000 otoe-0.0.5/otoe/src/otoe.egg-info/dependency_links.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       52 2023-04-16 20:40:27.000000 otoe-0.0.5/otoe/src/otoe.egg-info/entry_points.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)        5 2023-04-16 20:40:27.000000 otoe-0.0.5/otoe/src/otoe.egg-info/top_level.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       38 2023-04-16 20:40:27.302451 otoe-0.0.5/setup.cfg
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1389 2023-04-16 20:40:18.000000 otoe-0.0.5/setup.py
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:44:09.494371 otoe-0.0.6/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      960 2023-04-16 20:44:09.494241 otoe-0.0.6/PKG-INFO
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      637 2023-04-10 20:00:48.000000 otoe-0.0.6/README.md
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:44:09.492810 otoe-0.0.6/otoe/
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:44:09.492876 otoe-0.0.6/otoe/src/
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:44:09.492930 otoe-0.0.6/otoe/src/otoe_epicker/
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:44:09.494024 otoe-0.0.6/otoe/src/otoe_epicker/otoe.egg-info/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      960 2023-04-16 20:44:09.000000 otoe-0.0.6/otoe/src/otoe_epicker/otoe.egg-info/PKG-INFO
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      835 2023-04-16 20:44:09.000000 otoe-0.0.6/otoe/src/otoe_epicker/otoe.egg-info/SOURCES.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        1 2023-04-16 20:44:09.000000 otoe-0.0.6/otoe/src/otoe_epicker/otoe.egg-info/dependency_links.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       52 2023-04-16 20:44:09.000000 otoe-0.0.6/otoe/src/otoe_epicker/otoe.egg-info/entry_points.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        5 2023-04-16 20:44:09.000000 otoe-0.0.6/otoe/src/otoe_epicker/otoe.egg-info/top_level.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       38 2023-04-16 20:44:09.494410 otoe-0.0.6/setup.cfg
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1402 2023-04-16 20:44:00.000000 otoe-0.0.6/setup.py
```

### Comparing `otoe-0.0.5/PKG-INFO` & `otoe-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoe
-Version: 0.0.5
+Version: 0.0.6
 Summary: Sort of a UI for espanso configs.
 Author: Yakov Varnaev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `otoe-0.0.5/README.md` & `otoe-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `otoe-0.0.5/otoe/src/otoe.egg-info/PKG-INFO` & `otoe-0.0.6/otoe/src/otoe_epicker/otoe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoe
-Version: 0.0.5
+Version: 0.0.6
 Summary: Sort of a UI for espanso configs.
 Author: Yakov Varnaev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `otoe-0.0.5/setup.py` & `otoe-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 srcpath = str(Path(__file__).parent / 'src' / 'otoe_epicker')
 
 setuptools.setup(
     name="otoe",                     # This is the name of the package
-    version="0.0.5",                        # The initial release version
+    version="0.0.6",                        # The initial release version
     author="Yakov Varnaev",                     # Full name of the author
     description="Sort of a UI for espanso configs.",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.7',                # Minimum version requirement of the package
     py_modules=["otoe"],             # Name of the python package
-    package_dir={'': 'otoe/src'},     # Directory of the source code of the package
+    package_dir={'': 'otoe/src/otoe_epicker'},     # Directory of the source code of the package
     install_requires=[],                     # Install other dependencies if any
     entry_points={
         'console_scripts': [
             'otoe=otoe_epicker.obsidian:main',
        ],
     }
 )
```

