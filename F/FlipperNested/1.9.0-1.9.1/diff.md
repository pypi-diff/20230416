# Comparing `tmp/FlipperNested-1.9.0.tar.gz` & `tmp/FlipperNested-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlipperNested-1.9.0.tar", last modified: Thu Apr 13 18:37:40 2023, max compression
+gzip compressed data, was "FlipperNested-1.9.1.tar", last modified: Sun Apr 16 19:06:49 2023, max compression
```

## Comparing `FlipperNested-1.9.0.tar` & `FlipperNested-1.9.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:37:40.087426 FlipperNested-1.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:37:40.083426 FlipperNested-1.9.0/FlipperNested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/FlipperNested/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/FlipperNested/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/FlipperNested/bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/FlipperNested/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/FlipperNested/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:37:40.083426 FlipperNested-1.9.0/FlipperNested/proto/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/FlipperNested/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/FlipperNested/proto/flipper_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/FlipperNested/proto/storage_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:37:40.083426 FlipperNested-1.9.0/FlipperNested.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-13 18:37:40.000000 FlipperNested-1.9.0/FlipperNested.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-13 18:37:40.000000 FlipperNested-1.9.0/FlipperNested.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:37:40.000000 FlipperNested-1.9.0/FlipperNested.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-13 18:37:40.000000 FlipperNested-1.9.0/FlipperNested.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-13 18:37:40.000000 FlipperNested-1.9.0/FlipperNested.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-13 18:37:40.000000 FlipperNested-1.9.0/FlipperNested.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:37:40.087426 FlipperNested-1.9.0/NestedSolver/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/bucketsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/bucketsort.h
--rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/crapto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/crapto1.h
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/crypto1.c
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/library.c
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/library.h
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/parity.h
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/progress.c
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/progress.h
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/NestedSolver/python.c
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-13 18:37:40.087426 FlipperNested-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 18:37:40.087426 FlipperNested-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:37:40.087426 FlipperNested-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/tests/test_calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-13 18:37:30.000000 FlipperNested-1.9.0/tests/test_parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:06:49.841029 FlipperNested-1.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:06:49.837029 FlipperNested-1.9.1/FlipperNested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/FlipperNested/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/FlipperNested/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/FlipperNested/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/FlipperNested/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/FlipperNested/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:06:49.837029 FlipperNested-1.9.1/FlipperNested/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/FlipperNested/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/FlipperNested/proto/flipper_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/FlipperNested/proto/storage_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:06:49.837029 FlipperNested-1.9.1/FlipperNested.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-16 19:06:49.000000 FlipperNested-1.9.1/FlipperNested.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-16 19:06:49.000000 FlipperNested-1.9.1/FlipperNested.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 19:06:49.000000 FlipperNested-1.9.1/FlipperNested.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-16 19:06:49.000000 FlipperNested-1.9.1/FlipperNested.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-16 19:06:49.000000 FlipperNested-1.9.1/FlipperNested.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-16 19:06:49.000000 FlipperNested-1.9.1/FlipperNested.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:06:49.841029 FlipperNested-1.9.1/NestedSolver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/bucketsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/bucketsort.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/crapto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/crapto1.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/crypto1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/library.c
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/library.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/parity.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/progress.c
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/progress.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/NestedSolver/python.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-16 19:06:49.841029 FlipperNested-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 19:06:49.841029 FlipperNested-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:06:49.841029 FlipperNested-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/tests/test_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-16 19:06:40.000000 FlipperNested-1.9.1/tests/test_parse.py
```

### Comparing `FlipperNested-1.9.0/FlipperNested/bridge.py` & `FlipperNested-1.9.1/FlipperNested/bridge.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.0/FlipperNested/cli.py` & `FlipperNested-1.9.1/FlipperNested/cli.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.0/FlipperNested/main.py` & `FlipperNested-1.9.1/FlipperNested/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         version_string = lines.pop(0)
         if "Version" not in version_string:
             print("No version info in", self.filename)
             return False
         file_version = int(version_string.split(": ")[1])
         if file_version != self.VERSION:
             print("[!!!] Invalid version for", self.filename)
-            print("[!] You should update " + "app" if file_version < self.VERSION else "recovery script")
+            print("[!] You should update " + ("app" if file_version < self.VERSION else "recovery script"))
             return False
         if "Nested: Delay" in contents:
             print("[!] Nested attack with delay was used, will try more PRNG values (will take more time)")
             result = re.search(r"Nested: Delay [0-9]*, distance ([0-9]*)", contents.strip())
             print("[?] Please select depth of check")
             print("[1] Fast: +-25 values")
             print("[2] Normal: +-50 values")
```

### Comparing `FlipperNested-1.9.0/FlipperNested/proto/flipper_pb2.py` & `FlipperNested-1.9.1/FlipperNested/proto/flipper_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.0/FlipperNested/proto/storage_pb2.py` & `FlipperNested-1.9.1/FlipperNested/proto/storage_pb2.py`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.0/FlipperNested.egg-info/PKG-INFO` & `FlipperNested-1.9.1/FlipperNested.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 1.9.0
+Version: 1.9.1
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `FlipperNested-1.9.0/FlipperNested.egg-info/SOURCES.txt` & `FlipperNested-1.9.1/FlipperNested.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.0/LICENSE.md` & `FlipperNested-1.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.0/NestedSolver/bucketsort.c` & `FlipperNested-1.9.1/NestedSolver/bucketsort.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.0/NestedSolver/bucketsort.h` & `FlipperNested-1.9.1/NestedSolver/bucketsort.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.0/NestedSolver/crapto1.c` & `FlipperNested-1.9.1/NestedSolver/crapto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.0/NestedSolver/crapto1.h` & `FlipperNested-1.9.1/NestedSolver/crapto1.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.0/NestedSolver/crypto1.c` & `FlipperNested-1.9.1/NestedSolver/crypto1.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.0/NestedSolver/library.c` & `FlipperNested-1.9.1/NestedSolver/library.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.0/NestedSolver/library.h` & `FlipperNested-1.9.1/NestedSolver/library.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.0/NestedSolver/parity.h` & `FlipperNested-1.9.1/NestedSolver/parity.h`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.0/NestedSolver/progress.c` & `FlipperNested-1.9.1/NestedSolver/progress.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.0/NestedSolver/python.c` & `FlipperNested-1.9.1/NestedSolver/python.c`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.0/PKG-INFO` & `FlipperNested-1.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlipperNested
-Version: 1.9.0
+Version: 1.9.1
 Summary: Recover keys from collected nonces
 Home-page: https://github.com/AloneLiberty/FlipperNestedRecovery
 Author: AloneLiberty
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `FlipperNested-1.9.0/README.md` & `FlipperNested-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `FlipperNested-1.9.0/setup.py` & `FlipperNested-1.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                           libraries=libraries)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="FlipperNested",
-    version="1.9.0",
+    version="1.9.1",
     author="AloneLiberty",
     description="Recover keys from collected nonces",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AloneLiberty/FlipperNestedRecovery",
     entry_points={'console_scripts': ['FlipperNested = FlipperNested.cli:main']},
     install_requires=['protobuf>4', 'pyserial'],
```

### Comparing `FlipperNested-1.9.0/tests/test_calculate.py` & `FlipperNested-1.9.1/tests/test_calculate.py`

 * *Files identical despite different names*

