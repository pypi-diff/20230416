# Comparing `tmp/cagen-0.2.0a1.tar.gz` & `tmp/cagen-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cagen-0.2.0a1.tar", last modified: Sat Apr 15 18:22:11 2023, max compression
+gzip compressed data, was "cagen-0.2.0a2.tar", last modified: Sun Apr 16 17:35:10 2023, max compression
```

## Comparing `cagen-0.2.0a1.tar` & `cagen-0.2.0a2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-15 18:22:11.005245 cagen-0.2.0a1/
--rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0a1/MANIFEST.in
--rw-r--r--   0 xan       (1000) xan       (1000)     3943 2023-04-15 18:22:11.005245 cagen-0.2.0a1/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)     3208 2023-04-15 08:10:27.000000 cagen-0.2.0a1/README.md
--rw-r--r--   0 xan       (1000) xan       (1000)     1160 2023-04-15 08:11:23.000000 cagen-0.2.0a1/pyproject.toml
--rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-04-15 18:22:11.005245 cagen-0.2.0a1/setup.cfg
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-15 18:22:11.001911 cagen-0.2.0a1/src/
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-15 18:22:11.005245 cagen-0.2.0a1/src/cagen/
--rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0a1/src/cagen/__init__.py
--rw-r--r--   0 xan       (1000) xan       (1000)     4757 2023-03-28 18:54:37.000000 cagen-0.2.0a1/src/cagen/cmd.py
--rw-r--r--   0 xan       (1000) xan       (1000)     8233 2023-03-28 18:54:45.000000 cagen-0.2.0a1/src/cagen/libcagen.py
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-15 18:22:11.005245 cagen-0.2.0a1/src/cagen/templates/
--rw-r--r--   0 xan       (1000) xan       (1000)      381 2023-02-09 11:33:44.000000 cagen-0.2.0a1/src/cagen/templates/list.md.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0a1/src/cagen/templates/list.md.tmpl.license
--rw-r--r--   0 xan       (1000) xan       (1000)     1754 2023-01-21 12:38:41.000000 cagen-0.2.0a1/src/cagen/templates/schema.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0a1/src/cagen/templates/schema.tmpl.license
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-15 18:22:11.005245 cagen-0.2.0a1/src/cagen.egg-info/
--rw-r--r--   0 xan       (1000) xan       (1000)     3943 2023-04-15 18:22:10.000000 cagen-0.2.0a1/src/cagen.egg-info/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-04-15 18:22:11.000000 cagen-0.2.0a1/src/cagen.egg-info/SOURCES.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-04-15 18:22:10.000000 cagen-0.2.0a1/src/cagen.egg-info/dependency_links.txt
--rw-r--r--   0 xan       (1000) xan       (1000)      114 2023-04-15 18:22:10.000000 cagen-0.2.0a1/src/cagen.egg-info/entry_points.txt
--rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-04-15 18:22:10.000000 cagen-0.2.0a1/src/cagen.egg-info/requires.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-04-15 18:22:10.000000 cagen-0.2.0a1/src/cagen.egg-info/top_level.txt
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-16 17:35:10.033770 cagen-0.2.0a2/
+-rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0a2/MANIFEST.in
+-rw-r--r--   0 xan       (1000) xan       (1000)     4049 2023-04-16 17:35:10.030436 cagen-0.2.0a2/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)     3314 2023-04-16 10:42:06.000000 cagen-0.2.0a2/README.md
+-rw-r--r--   0 xan       (1000) xan       (1000)     1160 2023-04-16 17:35:05.000000 cagen-0.2.0a2/pyproject.toml
+-rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-04-16 17:35:10.033770 cagen-0.2.0a2/setup.cfg
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-16 17:35:10.030436 cagen-0.2.0a2/src/
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-16 17:35:10.030436 cagen-0.2.0a2/src/cagen/
+-rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0a2/src/cagen/__init__.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     4757 2023-03-28 18:54:37.000000 cagen-0.2.0a2/src/cagen/cmd.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     8275 2023-04-16 17:34:47.000000 cagen-0.2.0a2/src/cagen/libcagen.py
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-16 17:35:10.030436 cagen-0.2.0a2/src/cagen/templates/
+-rw-r--r--   0 xan       (1000) xan       (1000)      381 2023-02-09 11:33:44.000000 cagen-0.2.0a2/src/cagen/templates/list.md.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0a2/src/cagen/templates/list.md.tmpl.license
+-rw-r--r--   0 xan       (1000) xan       (1000)     1754 2023-01-21 12:38:41.000000 cagen-0.2.0a2/src/cagen/templates/schema.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0a2/src/cagen/templates/schema.tmpl.license
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-04-16 17:35:10.030436 cagen-0.2.0a2/src/cagen.egg-info/
+-rw-r--r--   0 xan       (1000) xan       (1000)     4049 2023-04-16 17:35:10.000000 cagen-0.2.0a2/src/cagen.egg-info/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-04-16 17:35:10.000000 cagen-0.2.0a2/src/cagen.egg-info/SOURCES.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-04-16 17:35:10.000000 cagen-0.2.0a2/src/cagen.egg-info/dependency_links.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)      114 2023-04-16 17:35:10.000000 cagen-0.2.0a2/src/cagen.egg-info/entry_points.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-04-16 17:35:10.000000 cagen-0.2.0a2/src/cagen.egg-info/requires.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-04-16 17:35:10.000000 cagen-0.2.0a2/src/cagen.egg-info/top_level.txt
```

### Comparing `cagen-0.2.0a1/PKG-INFO` & `cagen-0.2.0a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: A static site generator for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -40,15 +40,15 @@
 The reason to use "external" templating system instead of built-in pandoc template system is because pandoc templates [are not capable of make conditions with values](https://pandoc.org/MANUAL.html#conditionals) (something like `$if(author=='me') Print full name here $endif$`).
 
 The program just converts markdown files to HTML ones by default in the same directory. Unlike many other static site generators, there is no predefined structure by default: no `assets` directory neither `site` directory. By default, all generated files are in the same directory than the source files. Obviously, you can modify it if you want.
 
 We provide:
 
 - a [library](src/cagen/libcagen.py)
-- a command line program (called `cagen`) for convert documents
+- a [command line program](src/cagen/cmd.py) (called `cagen`) for convert documents
 - a script called `cagen-make` to generate a Makefile to convert automatically all markdown files to HTML ones.
 
 The software is implemented in [python](https://www.python.org/) because it's easy to program (I'm very language-neutral). If you want some really fast static site generator, be free to fork the project and program with any compiled language.
 
 ## Installation
 
 You can install via [pip](https://pypi.org/project/cagen/):
@@ -84,13 +84,13 @@
 ```
 
 It automatically convert all markdown files to HTML5 ones using `templates/schema.tmpl` Mako template. You can modify it editing `Makefile`.
 
 ## Other resources
 
 - You can see the [list of tasks](tasks/index.md) (completed and pending).
-- The [API documentation](src/cagen/docs/index.html) is available.
+- The [API documentation](https://repo.or.cz/cagen.git/tree/HEAD:/src/cagen/docs) is available (automatically generated with [pdoc](https://pdoc.dev/)).
 
 ## Contribute
 
 If you want to make a suggestion, a question, reporting a bug, or even send patches, then you can send me an email to the concatenation, in some order, of the words in the set {"@", "posteo.net", "somenxavier"}. Sorry for the riddle, spam is strong in the web nowadays.
```

### Comparing `cagen-0.2.0a1/README.md` & `cagen-0.2.0a2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 The reason to use "external" templating system instead of built-in pandoc template system is because pandoc templates [are not capable of make conditions with values](https://pandoc.org/MANUAL.html#conditionals) (something like `$if(author=='me') Print full name here $endif$`).
 
 The program just converts markdown files to HTML ones by default in the same directory. Unlike many other static site generators, there is no predefined structure by default: no `assets` directory neither `site` directory. By default, all generated files are in the same directory than the source files. Obviously, you can modify it if you want.
 
 We provide:
 
 - a [library](src/cagen/libcagen.py)
-- a command line program (called `cagen`) for convert documents
+- a [command line program](src/cagen/cmd.py) (called `cagen`) for convert documents
 - a script called `cagen-make` to generate a Makefile to convert automatically all markdown files to HTML ones.
 
 The software is implemented in [python](https://www.python.org/) because it's easy to program (I'm very language-neutral). If you want some really fast static site generator, be free to fork the project and program with any compiled language.
 
 ## Installation
 
 You can install via [pip](https://pypi.org/project/cagen/):
@@ -65,13 +65,13 @@
 ```
 
 It automatically convert all markdown files to HTML5 ones using `templates/schema.tmpl` Mako template. You can modify it editing `Makefile`.
 
 ## Other resources
 
 - You can see the [list of tasks](tasks/index.md) (completed and pending).
-- The [API documentation](src/cagen/docs/index.html) is available.
+- The [API documentation](https://repo.or.cz/cagen.git/tree/HEAD:/src/cagen/docs) is available (automatically generated with [pdoc](https://pdoc.dev/)).
 
 ## Contribute
 
 If you want to make a suggestion, a question, reporting a bug, or even send patches, then you can send me an email to the concatenation, in some order, of the words in the set {"@", "posteo.net", "somenxavier"}. Sorry for the riddle, spam is strong in the web nowadays.
```

### Comparing `cagen-0.2.0a1/pyproject.toml` & `cagen-0.2.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [project.scripts]
 cagen = "cagen.cmd:cagen_cli"
 cagen-list = "cagen.cmd:cagen_list"
 cagen-make = "cagen.cmd:cagen_make"
 
 [project]
 name = "cagen"
-version = "0.2.0.alpha-1"
+version = "0.2.0.alpha-2"
 authors = [{'name'="Xavier B."}]
 description = "A static site generator for cmpalgorithms project"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
```

### Comparing `cagen-0.2.0a1/src/cagen/cmd.py` & `cagen-0.2.0a2/src/cagen/cmd.py`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0a1/src/cagen/libcagen.py` & `cagen-0.2.0a2/src/cagen/libcagen.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,16 @@
     ```
 
     If the cast is not possible, it cast the variable as `str` and not returning any error (just printed message).
     """
 
     eassignments = {}
     for variable in assignments:
-        if variable in evals:
-            try:
-                eassignments[variable] = eval("{}".format(assignments[variable]))
-            except:
-                eassignments[variable] = assignments[variable]
-                print("{} cannot be evaluated. Stored as str".format(variable))
+        if evals:
+            if variable in evals:
+                try:
+                    eassignments[variable] = eval("{}".format(assignments[variable]))
+                except:
+                    eassignments[variable] = assignments[variable]
+                    print("{} cannot be evaluated. Stored as str".format(variable))
 
     return eassignments
```

### Comparing `cagen-0.2.0a1/src/cagen/templates/schema.tmpl` & `cagen-0.2.0a2/src/cagen/templates/schema.tmpl`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0a1/src/cagen.egg-info/PKG-INFO` & `cagen-0.2.0a2/src/cagen.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: A static site generator for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -40,15 +40,15 @@
 The reason to use "external" templating system instead of built-in pandoc template system is because pandoc templates [are not capable of make conditions with values](https://pandoc.org/MANUAL.html#conditionals) (something like `$if(author=='me') Print full name here $endif$`).
 
 The program just converts markdown files to HTML ones by default in the same directory. Unlike many other static site generators, there is no predefined structure by default: no `assets` directory neither `site` directory. By default, all generated files are in the same directory than the source files. Obviously, you can modify it if you want.
 
 We provide:
 
 - a [library](src/cagen/libcagen.py)
-- a command line program (called `cagen`) for convert documents
+- a [command line program](src/cagen/cmd.py) (called `cagen`) for convert documents
 - a script called `cagen-make` to generate a Makefile to convert automatically all markdown files to HTML ones.
 
 The software is implemented in [python](https://www.python.org/) because it's easy to program (I'm very language-neutral). If you want some really fast static site generator, be free to fork the project and program with any compiled language.
 
 ## Installation
 
 You can install via [pip](https://pypi.org/project/cagen/):
@@ -84,13 +84,13 @@
 ```
 
 It automatically convert all markdown files to HTML5 ones using `templates/schema.tmpl` Mako template. You can modify it editing `Makefile`.
 
 ## Other resources
 
 - You can see the [list of tasks](tasks/index.md) (completed and pending).
-- The [API documentation](src/cagen/docs/index.html) is available.
+- The [API documentation](https://repo.or.cz/cagen.git/tree/HEAD:/src/cagen/docs) is available (automatically generated with [pdoc](https://pdoc.dev/)).
 
 ## Contribute
 
 If you want to make a suggestion, a question, reporting a bug, or even send patches, then you can send me an email to the concatenation, in some order, of the words in the set {"@", "posteo.net", "somenxavier"}. Sorry for the riddle, spam is strong in the web nowadays.
```

