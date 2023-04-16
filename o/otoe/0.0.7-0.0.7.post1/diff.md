# Comparing `tmp/otoe-0.0.7.tar.gz` & `tmp/otoe-0.0.7.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otoe-0.0.7.tar", last modified: Sun Apr 16 20:48:19 2023, max compression
+gzip compressed data, was "otoe-0.0.7.post1.tar", last modified: Sun Apr 16 20:53:03 2023, max compression
```

## Comparing `otoe-0.0.7.tar` & `otoe-0.0.7.post1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:48:19.809100 otoe-0.0.7/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      960 2023-04-16 20:48:19.808844 otoe-0.0.7/PKG-INFO
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      637 2023-04-10 20:00:48.000000 otoe-0.0.7/README.md
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:48:19.806864 otoe-0.0.7/otoe/
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:48:19.806929 otoe-0.0.7/otoe/src/
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:48:19.806986 otoe-0.0.7/otoe/src/otoe_epicker/
-drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:48:19.808479 otoe-0.0.7/otoe/src/otoe_epicker/otoe.egg-info/
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      960 2023-04-16 20:48:19.000000 otoe-0.0.7/otoe/src/otoe_epicker/otoe.egg-info/PKG-INFO
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)      835 2023-04-16 20:48:19.000000 otoe-0.0.7/otoe/src/otoe_epicker/otoe.egg-info/SOURCES.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)        1 2023-04-16 20:48:19.000000 otoe-0.0.7/otoe/src/otoe_epicker/otoe.egg-info/dependency_links.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       44 2023-04-16 20:48:19.000000 otoe-0.0.7/otoe/src/otoe_epicker/otoe.egg-info/entry_points.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)        5 2023-04-16 20:48:19.000000 otoe-0.0.7/otoe/src/otoe_epicker/otoe.egg-info/top_level.txt
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)       38 2023-04-16 20:48:19.809172 otoe-0.0.7/setup.cfg
--rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1394 2023-04-16 20:47:52.000000 otoe-0.0.7/setup.py
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:53:03.792889 otoe-0.0.7.post1/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      966 2023-04-16 20:53:03.792756 otoe-0.0.7.post1/PKG-INFO
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      637 2023-04-10 20:00:48.000000 otoe-0.0.7.post1/README.md
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:53:03.791309 otoe-0.0.7.post1/otoe/
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:53:03.791369 otoe-0.0.7.post1/otoe/src/
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:53:03.791425 otoe-0.0.7.post1/otoe/src/otoe_epicker/
+drwxr-xr-x   0 yakovvarnaev   (501) staff       (20)        0 2023-04-16 20:53:03.792549 otoe-0.0.7.post1/otoe/src/otoe_epicker/otoe.egg-info/
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      966 2023-04-16 20:53:03.000000 otoe-0.0.7.post1/otoe/src/otoe_epicker/otoe.egg-info/PKG-INFO
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)      835 2023-04-16 20:53:03.000000 otoe-0.0.7.post1/otoe/src/otoe_epicker/otoe.egg-info/SOURCES.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        1 2023-04-16 20:53:03.000000 otoe-0.0.7.post1/otoe/src/otoe_epicker/otoe.egg-info/dependency_links.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       39 2023-04-16 20:53:03.000000 otoe-0.0.7.post1/otoe/src/otoe_epicker/otoe.egg-info/entry_points.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)        5 2023-04-16 20:53:03.000000 otoe-0.0.7.post1/otoe/src/otoe_epicker/otoe.egg-info/top_level.txt
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)       38 2023-04-16 20:53:03.792934 otoe-0.0.7.post1/setup.cfg
+-rw-r--r--   0 yakovvarnaev   (501) staff       (20)     1391 2023-04-16 20:51:08.000000 otoe-0.0.7.post1/setup.py
```

### Comparing `otoe-0.0.7/PKG-INFO` & `otoe-0.0.7.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoe
-Version: 0.0.7
+Version: 0.0.7.post1
 Summary: Sort of a UI for espanso configs.
 Author: Yakov Varnaev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `otoe-0.0.7/README.md` & `otoe-0.0.7.post1/README.md`

 * *Files identical despite different names*

### Comparing `otoe-0.0.7/otoe/src/otoe_epicker/otoe.egg-info/PKG-INFO` & `otoe-0.0.7.post1/otoe/src/otoe_epicker/otoe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otoe
-Version: 0.0.7
+Version: 0.0.7.post1
 Summary: Sort of a UI for espanso configs.
 Author: Yakov Varnaev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `otoe-0.0.7/otoe/src/otoe_epicker/otoe.egg-info/SOURCES.txt` & `otoe-0.0.7.post1/otoe/src/otoe_epicker/otoe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `otoe-0.0.7/setup.py` & `otoe-0.0.7.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 srcpath = str(Path(__file__).parent / 'src' / 'otoe_epicker')
 
 setuptools.setup(
     name="otoe",                     # This is the name of the package
-    version="0.0.7",                        # The initial release version
+    version="0.0.7_1",                        # The initial release version
     author="Yakov Varnaev",                     # Full name of the author
     description="Sort of a UI for espanso configs.",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
@@ -21,11 +21,11 @@
     ],                                      # Information to filter the project on PyPi website
     python_requires='>=3.7',                # Minimum version requirement of the package
     py_modules=["otoe"],             # Name of the python package
     package_dir={'': 'otoe/src/otoe_epicker'},     # Directory of the source code of the package
     install_requires=[],                     # Install other dependencies if any
     entry_points={
         'console_scripts': [
-            'otoe=otoe.obsidian:main',
+            'otoe=obsidian:main',
        ],
     }
 )
```

