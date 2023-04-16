# Comparing `tmp/drup-1.0.0.tar.gz` & `tmp/drup-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drup-1.0.0.tar", last modified: Sun Apr 16 19:10:02 2023, max compression
+gzip compressed data, was "drup-1.0.1.tar", last modified: Sun Apr 16 20:04:52 2023, max compression
```

## Comparing `drup-1.0.0.tar` & `drup-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 mfredrik  (1000) mfredrik  (1000)        0 2023-04-16 19:10:02.177174 drup-1.0.0/
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)     1072 2023-04-16 13:21:59.000000 drup-1.0.0/LICENSE
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)       69 2023-04-16 18:45:20.000000 drup-1.0.0/MANIFEST.in
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)     4170 2023-04-16 19:10:02.176897 drup-1.0.0/PKG-INFO
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)     3450 2023-04-16 18:44:18.000000 drup-1.0.0/README.md
-drwxrwxr-x   0 mfredrik  (1000) mfredrik  (1000)        0 2023-04-16 19:10:02.172538 drup-1.0.0/drup.egg-info/
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)     4170 2023-04-16 19:10:02.000000 drup-1.0.0/drup.egg-info/PKG-INFO
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)      233 2023-04-16 19:10:02.000000 drup-1.0.0/drup.egg-info/SOURCES.txt
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)        1 2023-04-16 19:10:02.000000 drup-1.0.0/drup.egg-info/dependency_links.txt
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)        5 2023-04-16 19:10:02.000000 drup-1.0.0/drup.egg-info/top_level.txt
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)      777 2023-04-16 18:40:22.000000 drup-1.0.0/pyproject.toml
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)       38 2023-04-16 19:10:02.177266 drup-1.0.0/setup.cfg
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)     1138 2023-04-16 19:09:46.000000 drup-1.0.0/setup.py
-drwxrwxr-x   0 mfredrik  (1000) mfredrik  (1000)        0 2023-04-16 19:10:02.168415 drup-1.0.0/src/
-drwxrwxr-x   0 mfredrik  (1000) mfredrik  (1000)        0 2023-04-16 19:10:02.176394 drup-1.0.0/src/drup/
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)      405 2023-04-16 18:43:43.000000 drup-1.0.0/src/drup/__init__.py
--r-xr-xr-x   0 mfredrik  (1000) mfredrik  (1000)   649704 2023-04-16 19:10:02.000000 drup-1.0.0/src/drup/librupchecker.so
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)     1914 2023-04-16 18:42:28.000000 drup-1.0.0/src/drup/wrappers.py
+drwxrwxr-x   0 mfredrik  (1000) mfredrik  (1000)        0 2023-04-16 20:04:52.622863 drup-1.0.1/
+-rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)     1072 2023-04-16 13:21:59.000000 drup-1.0.1/LICENSE
+-rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)       69 2023-04-16 18:45:20.000000 drup-1.0.1/MANIFEST.in
+-rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)     4170 2023-04-16 20:04:52.622651 drup-1.0.1/PKG-INFO
+-rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)     3450 2023-04-16 18:44:18.000000 drup-1.0.1/README.md
+drwxrwxr-x   0 mfredrik  (1000) mfredrik  (1000)        0 2023-04-16 20:04:52.618732 drup-1.0.1/drup.egg-info/
+-rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)     4170 2023-04-16 20:04:52.000000 drup-1.0.1/drup.egg-info/PKG-INFO
+-rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)      233 2023-04-16 20:04:52.000000 drup-1.0.1/drup.egg-info/SOURCES.txt
+-rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)        1 2023-04-16 20:04:52.000000 drup-1.0.1/drup.egg-info/dependency_links.txt
+-rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)        5 2023-04-16 20:04:52.000000 drup-1.0.1/drup.egg-info/top_level.txt
+-rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)      777 2023-04-16 19:59:25.000000 drup-1.0.1/pyproject.toml
+-rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)       38 2023-04-16 20:04:52.622924 drup-1.0.1/setup.cfg
+-rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)     1138 2023-04-16 19:14:48.000000 drup-1.0.1/setup.py
+drwxrwxr-x   0 mfredrik  (1000) mfredrik  (1000)        0 2023-04-16 20:04:52.615637 drup-1.0.1/src/
+drwxrwxr-x   0 mfredrik  (1000) mfredrik  (1000)        0 2023-04-16 20:04:52.622196 drup-1.0.1/src/drup/
+-rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)      405 2023-04-16 19:48:42.000000 drup-1.0.1/src/drup/__init__.py
+-r-xr-xr-x   0 mfredrik  (1000) mfredrik  (1000)   649704 2023-04-16 20:04:52.000000 drup-1.0.1/src/drup/librupchecker.so
+-rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)     1914 2023-04-16 18:42:28.000000 drup-1.0.1/src/drup/wrappers.py
```

### Comparing `drup-1.0.0/LICENSE` & `drup-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drup-1.0.0/PKG-INFO` & `drup-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: drup
-Version: 1.0.0
+Version: 1.0.1
 Summary: Checks DRUP proofs against DIMACS source. Extracted from verified Why3 code.
 Author-email: Matt Fredrikson <mfredrik@cmu.edu>
 Project-URL: Homepage, https://github.com/cmu-transparency/verified_rup
 Project-URL: Bug Tracker, https://github.com/cmu-transparency/verified_rup/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: OCaml
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Verified DRUP Proof Checker
 
 As the title suggests, a verified implementation of a checker for propositional unsatisfiability proofs in the  [DRUP format](https://satcompetition.github.io/2022/certificates.html) that is produced by several solvers.
 The core of the checker is written in [Why3](https://why3.lri.fr/), which is extracted to OCaml, compiled natively, and exported as a C library with Python bindings.
```

### Comparing `drup-1.0.0/README.md` & `drup-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `drup-1.0.0/drup.egg-info/PKG-INFO` & `drup-1.0.1/drup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: drup
-Version: 1.0.0
+Version: 1.0.1
 Summary: Checks DRUP proofs against DIMACS source. Extracted from verified Why3 code.
 Author-email: Matt Fredrikson <mfredrik@cmu.edu>
 Project-URL: Homepage, https://github.com/cmu-transparency/verified_rup
 Project-URL: Bug Tracker, https://github.com/cmu-transparency/verified_rup/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: OCaml
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Verified DRUP Proof Checker
 
 As the title suggests, a verified implementation of a checker for propositional unsatisfiability proofs in the  [DRUP format](https://satcompetition.github.io/2022/certificates.html) that is produced by several solvers.
 The core of the checker is written in [Why3](https://why3.lri.fr/), which is extracted to OCaml, compiled natively, and exported as a C library with Python bindings.
```

### Comparing `drup-1.0.0/pyproject.toml` & `drup-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "drup"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Matt Fredrikson", email="mfredrik@cmu.edu" },
 ]
 description = "Checks DRUP proofs against DIMACS source. Extracted from verified Why3 code."
 readme = "README.md"
-requires-python = ">=3.6"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: OCaml",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
     "Topic :: Scientific/Engineering :: Mathematics"
```

### Comparing `drup-1.0.0/setup.py` & `drup-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `drup-1.0.0/src/drup/librupchecker.so` & `drup-1.0.1/src/drup/librupchecker.so`

 * *Files identical despite different names*

### Comparing `drup-1.0.0/src/drup/wrappers.py` & `drup-1.0.1/src/drup/wrappers.py`

 * *Files identical despite different names*

