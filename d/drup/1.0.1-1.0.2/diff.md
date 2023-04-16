# Comparing `tmp/drup-1.0.1.tar.gz` & `tmp/drup-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drup-1.0.1.tar", last modified: Sun Apr 16 20:04:52 2023, max compression
+gzip compressed data, was "drup-1.0.2.tar", last modified: Sun Apr 16 20:27:55 2023, max compression
```

## Comparing `drup-1.0.1.tar` & `drup-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 mfredrik  (1000) mfredrik  (1000)        0 2023-04-16 20:04:52.622863 drup-1.0.1/
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)     1072 2023-04-16 13:21:59.000000 drup-1.0.1/LICENSE
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)       69 2023-04-16 18:45:20.000000 drup-1.0.1/MANIFEST.in
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)     4170 2023-04-16 20:04:52.622651 drup-1.0.1/PKG-INFO
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)     3450 2023-04-16 18:44:18.000000 drup-1.0.1/README.md
-drwxrwxr-x   0 mfredrik  (1000) mfredrik  (1000)        0 2023-04-16 20:04:52.618732 drup-1.0.1/drup.egg-info/
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)     4170 2023-04-16 20:04:52.000000 drup-1.0.1/drup.egg-info/PKG-INFO
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)      233 2023-04-16 20:04:52.000000 drup-1.0.1/drup.egg-info/SOURCES.txt
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)        1 2023-04-16 20:04:52.000000 drup-1.0.1/drup.egg-info/dependency_links.txt
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)        5 2023-04-16 20:04:52.000000 drup-1.0.1/drup.egg-info/top_level.txt
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)      777 2023-04-16 19:59:25.000000 drup-1.0.1/pyproject.toml
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)       38 2023-04-16 20:04:52.622924 drup-1.0.1/setup.cfg
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)     1138 2023-04-16 19:14:48.000000 drup-1.0.1/setup.py
-drwxrwxr-x   0 mfredrik  (1000) mfredrik  (1000)        0 2023-04-16 20:04:52.615637 drup-1.0.1/src/
-drwxrwxr-x   0 mfredrik  (1000) mfredrik  (1000)        0 2023-04-16 20:04:52.622196 drup-1.0.1/src/drup/
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)      405 2023-04-16 19:48:42.000000 drup-1.0.1/src/drup/__init__.py
--r-xr-xr-x   0 mfredrik  (1000) mfredrik  (1000)   649704 2023-04-16 20:04:52.000000 drup-1.0.1/src/drup/librupchecker.so
--rw-rw-r--   0 mfredrik  (1000) mfredrik  (1000)     1914 2023-04-16 18:42:28.000000 drup-1.0.1/src/drup/wrappers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 20:27:55.834829 drup-1.0.2/
+-rw-rw-r--   0 root         (0) root         (0)     1072 2023-04-16 13:21:59.000000 drup-1.0.2/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       69 2023-04-16 18:45:20.000000 drup-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4170 2023-04-16 20:27:55.834623 drup-1.0.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3450 2023-04-16 18:44:18.000000 drup-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 20:27:55.825711 drup-1.0.2/drup.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     4170 2023-04-16 20:27:55.000000 drup-1.0.2/drup.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      233 2023-04-16 20:27:55.000000 drup-1.0.2/drup.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-04-16 20:27:55.000000 drup-1.0.2/drup.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)        5 2023-04-16 20:27:55.000000 drup-1.0.2/drup.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      777 2023-04-16 20:27:25.000000 drup-1.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 20:27:55.834903 drup-1.0.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1139 2023-04-16 20:24:42.000000 drup-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 20:27:55.822121 drup-1.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 20:27:55.834129 drup-1.0.2/src/drup/
+-rw-rw-r--   0 root         (0) root         (0)      405 2023-04-16 20:27:28.000000 drup-1.0.2/src/drup/__init__.py
+-r-xr-xr-x   0 root         (0) root         (0)  2084792 2023-04-16 20:27:55.000000 drup-1.0.2/src/drup/librupchecker.so
+-rw-rw-r--   0 root         (0) root         (0)     1914 2023-04-16 18:42:28.000000 drup-1.0.2/src/drup/wrappers.py
```

### Comparing `drup-1.0.1/LICENSE` & `drup-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drup-1.0.1/PKG-INFO` & `drup-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drup
-Version: 1.0.1
+Version: 1.0.2
 Summary: Checks DRUP proofs against DIMACS source. Extracted from verified Why3 code.
 Author-email: Matt Fredrikson <mfredrik@cmu.edu>
 Project-URL: Homepage, https://github.com/cmu-transparency/verified_rup
 Project-URL: Bug Tracker, https://github.com/cmu-transparency/verified_rup/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: OCaml
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `drup-1.0.1/README.md` & `drup-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `drup-1.0.1/drup.egg-info/PKG-INFO` & `drup-1.0.2/drup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drup
-Version: 1.0.1
+Version: 1.0.2
 Summary: Checks DRUP proofs against DIMACS source. Extracted from verified Why3 code.
 Author-email: Matt Fredrikson <mfredrik@cmu.edu>
 Project-URL: Homepage, https://github.com/cmu-transparency/verified_rup
 Project-URL: Bug Tracker, https://github.com/cmu-transparency/verified_rup/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: OCaml
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `drup-1.0.1/pyproject.toml` & `drup-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "drup"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Matt Fredrikson", email="mfredrik@cmu.edu" },
 ]
 description = "Checks DRUP proofs against DIMACS source. Extracted from verified Why3 code."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `drup-1.0.1/setup.py` & `drup-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 class SDist(_sdist):
     def run(self) -> None:
         extract_checker()
         build_checker()
         shutil.copy("_build/default/src/librupchecker/checker.so", "src/drup/librupchecker.so")
         super().run()
         cmd = ["dune", "clean"]
-        subprocess.run(cmd, check=True, stdout=sys.stdout, stderr=sys.stderr)
+        subprocess.run(cmd, check=False, stdout=sys.stdout, stderr=sys.stderr)
         os.unlink("src/drup/librupchecker.so")
         os.unlink("src/librupchecker/rup.ml")
 
 setup(
     cmdclass={'sdist': SDist},
     packages=['drup'],
     package_dir={'drup': 'src/drup'},
```

### Comparing `drup-1.0.1/src/drup/wrappers.py` & `drup-1.0.2/src/drup/wrappers.py`

 * *Files identical despite different names*

