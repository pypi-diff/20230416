# Comparing `tmp/pylint_json2checkstyle-0.0.8.tar.gz` & `tmp/pylint_json2checkstyle-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/calvarez/dev/projects/perso/pylint-json2checkstyle/dist/tmp171dux2k/pylint_json2checkstyle-0.0.8.tar", last modified: Sat May 21 20:31:48 2022, max compression
+gzip compressed data, was "/Users/calvarez/dev/projects/perso/pylint-json2checkstyle/dist/tmpap4daq4z/pylint_json2checkstyle-0.0.9.tar", last modified: Sat May 21 21:56:47 2022, max compression
```

## Comparing `pylint_json2checkstyle-0.0.8.tar` & `pylint_json2checkstyle-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 calvarez   (501) staff       (20)        0 2022-05-21 20:31:48.000000 pylint_json2checkstyle-0.0.8/
--rw-r--r--   0 calvarez   (501) staff       (20)     1748 2022-05-21 20:31:48.000000 pylint_json2checkstyle-0.0.8/PKG-INFO
--rw-r--r--   0 calvarez   (501) staff       (20)     1058 2022-05-21 13:51:26.000000 pylint_json2checkstyle-0.0.8/LICENSE
--rw-r--r--   0 calvarez   (501) staff       (20)       88 2022-05-21 17:24:45.000000 pylint_json2checkstyle-0.0.8/pyproject.toml
-drwxr-xr-x   0 calvarez   (501) staff       (20)        0 2022-05-21 20:31:48.000000 pylint_json2checkstyle-0.0.8/pylint_json2checkstyle/
--rw-r--r--   0 calvarez   (501) staff       (20)     4606 2022-05-21 19:59:16.000000 pylint_json2checkstyle-0.0.8/pylint_json2checkstyle/checkstyle_reporter.py
--rw-r--r--   0 calvarez   (501) staff       (20)        0 2022-05-21 13:51:26.000000 pylint_json2checkstyle-0.0.8/pylint_json2checkstyle/__init__.py
--rw-r--r--   0 calvarez   (501) staff       (20)     1122 2022-05-21 17:06:54.000000 pylint_json2checkstyle-0.0.8/README.md
--rw-r--r--   0 calvarez   (501) staff       (20)       82 2022-05-21 18:04:37.000000 pylint_json2checkstyle-0.0.8/setup.py
-drwxr-xr-x   0 calvarez   (501) staff       (20)        0 2022-05-21 20:31:48.000000 pylint_json2checkstyle-0.0.8/pylint_json2checkstyle.egg-info/
--rw-r--r--   0 calvarez   (501) staff       (20)     1748 2022-05-21 20:31:48.000000 pylint_json2checkstyle-0.0.8/pylint_json2checkstyle.egg-info/PKG-INFO
--rw-r--r--   0 calvarez   (501) staff       (20)      410 2022-05-21 20:31:48.000000 pylint_json2checkstyle-0.0.8/pylint_json2checkstyle.egg-info/SOURCES.txt
--rw-r--r--   0 calvarez   (501) staff       (20)       92 2022-05-21 20:31:48.000000 pylint_json2checkstyle-0.0.8/pylint_json2checkstyle.egg-info/entry_points.txt
--rw-r--r--   0 calvarez   (501) staff       (20)        7 2022-05-21 20:31:48.000000 pylint_json2checkstyle-0.0.8/pylint_json2checkstyle.egg-info/requires.txt
--rw-r--r--   0 calvarez   (501) staff       (20)       23 2022-05-21 20:31:48.000000 pylint_json2checkstyle-0.0.8/pylint_json2checkstyle.egg-info/top_level.txt
--rw-r--r--   0 calvarez   (501) staff       (20)        1 2022-05-21 20:31:48.000000 pylint_json2checkstyle-0.0.8/pylint_json2checkstyle.egg-info/dependency_links.txt
--rw-r--r--   0 calvarez   (501) staff       (20)      854 2022-05-21 20:31:48.000000 pylint_json2checkstyle-0.0.8/setup.cfg
+drwxr-xr-x   0 calvarez   (501) staff       (20)        0 2022-05-21 21:56:47.000000 pylint_json2checkstyle-0.0.9/
+-rw-r--r--   0 calvarez   (501) staff       (20)     1871 2022-05-21 21:56:47.000000 pylint_json2checkstyle-0.0.9/PKG-INFO
+-rw-r--r--   0 calvarez   (501) staff       (20)     1058 2022-05-21 13:51:26.000000 pylint_json2checkstyle-0.0.9/LICENSE
+-rw-r--r--   0 calvarez   (501) staff       (20)       88 2022-05-21 17:24:45.000000 pylint_json2checkstyle-0.0.9/pyproject.toml
+drwxr-xr-x   0 calvarez   (501) staff       (20)        0 2022-05-21 21:56:47.000000 pylint_json2checkstyle-0.0.9/pylint_json2checkstyle/
+-rw-r--r--   0 calvarez   (501) staff       (20)     4606 2022-05-21 19:59:16.000000 pylint_json2checkstyle-0.0.9/pylint_json2checkstyle/checkstyle_reporter.py
+-rw-r--r--   0 calvarez   (501) staff       (20)        0 2022-05-21 13:51:26.000000 pylint_json2checkstyle-0.0.9/pylint_json2checkstyle/__init__.py
+-rw-r--r--   0 calvarez   (501) staff       (20)     1122 2022-05-21 17:06:54.000000 pylint_json2checkstyle-0.0.9/README.md
+-rw-r--r--   0 calvarez   (501) staff       (20)       82 2022-05-21 18:04:37.000000 pylint_json2checkstyle-0.0.9/setup.py
+drwxr-xr-x   0 calvarez   (501) staff       (20)        0 2022-05-21 21:56:47.000000 pylint_json2checkstyle-0.0.9/pylint_json2checkstyle.egg-info/
+-rw-r--r--   0 calvarez   (501) staff       (20)     1871 2022-05-21 21:56:47.000000 pylint_json2checkstyle-0.0.9/pylint_json2checkstyle.egg-info/PKG-INFO
+-rw-r--r--   0 calvarez   (501) staff       (20)      410 2022-05-21 21:56:47.000000 pylint_json2checkstyle-0.0.9/pylint_json2checkstyle.egg-info/SOURCES.txt
+-rw-r--r--   0 calvarez   (501) staff       (20)       92 2022-05-21 21:56:47.000000 pylint_json2checkstyle-0.0.9/pylint_json2checkstyle.egg-info/entry_points.txt
+-rw-r--r--   0 calvarez   (501) staff       (20)        7 2022-05-21 21:56:47.000000 pylint_json2checkstyle-0.0.9/pylint_json2checkstyle.egg-info/requires.txt
+-rw-r--r--   0 calvarez   (501) staff       (20)       23 2022-05-21 21:56:47.000000 pylint_json2checkstyle-0.0.9/pylint_json2checkstyle.egg-info/top_level.txt
+-rw-r--r--   0 calvarez   (501) staff       (20)        1 2022-05-21 21:56:47.000000 pylint_json2checkstyle-0.0.9/pylint_json2checkstyle.egg-info/dependency_links.txt
+-rw-r--r--   0 calvarez   (501) staff       (20)      944 2022-05-21 21:56:47.000000 pylint_json2checkstyle-0.0.9/setup.cfg
```

### Comparing `pylint_json2checkstyle-0.0.8/PKG-INFO` & `pylint_json2checkstyle-0.0.9/pylint_json2checkstyle.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
-Name: pylint_json2checkstyle
-Version: 0.0.8
+Name: pylint-json2checkstyle
+Version: 0.0.9
 Summary: A Pylint plugin and command line tool to produce Pylint reports in checkstyle format.
 Home-page: https://github.com/caarmen/pylint-json2checkstyle
 Author: Carmen Alvarez
 Author-email: carmen@rmen.ca
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/caarmen/pylint-json2checkstyle/issues
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pylint-json2checkstyle
 
 A Pylint plugin and command line tool to produce Pylint reports in checkstyle format.
```

### Comparing `pylint_json2checkstyle-0.0.8/LICENSE` & `pylint_json2checkstyle-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pylint_json2checkstyle-0.0.8/pylint_json2checkstyle/checkstyle_reporter.py` & `pylint_json2checkstyle-0.0.9/pylint_json2checkstyle/checkstyle_reporter.py`

 * *Files identical despite different names*

### Comparing `pylint_json2checkstyle-0.0.8/README.md` & `pylint_json2checkstyle-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pylint_json2checkstyle-0.0.8/pylint_json2checkstyle.egg-info/PKG-INFO` & `pylint_json2checkstyle-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
-Name: pylint-json2checkstyle
-Version: 0.0.8
+Name: pylint_json2checkstyle
+Version: 0.0.9
 Summary: A Pylint plugin and command line tool to produce Pylint reports in checkstyle format.
 Home-page: https://github.com/caarmen/pylint-json2checkstyle
 Author: Carmen Alvarez
 Author-email: carmen@rmen.ca
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/caarmen/pylint-json2checkstyle/issues
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pylint-json2checkstyle
 
 A Pylint plugin and command line tool to produce Pylint reports in checkstyle format.
```

### Comparing `pylint_json2checkstyle-0.0.8/setup.cfg` & `pylint_json2checkstyle-0.0.9/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [metadata]
 name = pylint_json2checkstyle
-version = 0.0.8
+version = 0.0.9
 author = Carmen Alvarez
 author_email = carmen@rmen.ca
 description = A Pylint plugin and command line tool to produce Pylint reports in checkstyle format.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/caarmen/pylint-json2checkstyle
 project_urls = 
 	Bug Tracker = https://github.com/caarmen/pylint-json2checkstyle/issues
 classifiers = 
-	Programming Language :: Python :: 3
+	Development Status :: 3 - Alpha
+	Environment :: Console
+	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
+	Programming Language :: Python :: 3
 
 [options]
 packages = pylint_json2checkstyle
 python_requires = >=3.6
 install_requires = 
 	pylint
```

