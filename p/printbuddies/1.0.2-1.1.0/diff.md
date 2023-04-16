# Comparing `tmp/printbuddies-1.0.2.tar.gz` & `tmp/printbuddies-1.1.0.tar.gz`

## Comparing `printbuddies-1.0.2.tar` & `printbuddies-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 printbuddies-1.0.2/CHANGELOG.md
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 printbuddies-1.0.2/docs/index.html
--rw-r--r--   0        0        0    34260 2020-02-02 00:00:00.000000 printbuddies-1.0.2/docs/printbuddies.html
--rw-r--r--   0        0        0    28001 2020-02-02 00:00:00.000000 printbuddies-1.0.2/docs/search.js
--rw-r--r--   0        0        0   153632 2020-02-02 00:00:00.000000 printbuddies-1.0.2/docs/printbuddies/printbuddies.html
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 printbuddies-1.0.2/src/printbuddies/__init__.py
--rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 printbuddies-1.0.2/src/printbuddies/printbuddies.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 printbuddies-1.0.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 printbuddies-1.0.2/LICENSE.txt
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 printbuddies-1.0.2/README.md
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 printbuddies-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 printbuddies-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 printbuddies-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 printbuddies-1.1.0/docs/index.html
+-rw-r--r--   0        0        0    34260 2020-02-02 00:00:00.000000 printbuddies-1.1.0/docs/printbuddies.html
+-rw-r--r--   0        0        0    28001 2020-02-02 00:00:00.000000 printbuddies-1.1.0/docs/search.js
+-rw-r--r--   0        0        0   153632 2020-02-02 00:00:00.000000 printbuddies-1.1.0/docs/printbuddies/printbuddies.html
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 printbuddies-1.1.0/src/printbuddies/__init__.py
+-rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 printbuddies-1.1.0/src/printbuddies/printbuddies.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 printbuddies-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 printbuddies-1.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 printbuddies-1.1.0/README.md
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 printbuddies-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 printbuddies-1.1.0/PKG-INFO
```

### Comparing `printbuddies-1.0.2/docs/printbuddies.html` & `printbuddies-1.1.0/docs/printbuddies.html`

 * *Files identical despite different names*

### Comparing `printbuddies-1.0.2/docs/search.js` & `printbuddies-1.1.0/docs/search.js`

 * *Files identical despite different names*

### Comparing `printbuddies-1.0.2/docs/printbuddies/printbuddies.html` & `printbuddies-1.1.0/docs/printbuddies/printbuddies.html`

 * *Files identical despite different names*

### Comparing `printbuddies-1.0.2/src/printbuddies/printbuddies.py` & `printbuddies-1.1.0/src/printbuddies/printbuddies.py`

 * *Files identical despite different names*

### Comparing `printbuddies-1.0.2/LICENSE.txt` & `printbuddies-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `printbuddies-1.0.2/README.md` & `printbuddies-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `printbuddies-1.0.2/pyproject.toml` & `printbuddies-1.1.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "printbuddies"
 authors = [{name="Matt Manes"}]
 description = "Handful of utilities to do printing tricks to the terminal."
-version = "1.0.2"
-requires-python = ">=3.6"
+version = "1.1.0"
+requires-python = ">=3.9"
 dependencies = ["noiftimer", "pytest"]
 readme = "README.md"
 keywords = [
     "terminal",
     "print",
     "printing",
     "progressbar"
```

### Comparing `printbuddies-1.0.2/PKG-INFO` & `printbuddies-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: printbuddies
-Version: 1.0.2
+Version: 1.1.0
 Summary: Handful of utilities to do printing tricks to the terminal.
 Project-URL: Homepage, https://github.com/matt-manes/printbuddies
 Project-URL: Documentation, https://github.com/matt-manes/printbuddies/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/printbuddies/tree/main/src/printbuddies
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: print,printing,progressbar,terminal
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Requires-Dist: noiftimer
 Requires-Dist: pytest
 Description-Content-Type: text/markdown
 
 # printbuddies
 
 A few utilities to do terminal printing tricks. <br>
```

