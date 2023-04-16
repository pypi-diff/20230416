# Comparing `tmp/pyproject-generator-0.0.2.tar.gz` & `tmp/pyproject-generator-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-generator-0.0.2.tar", last modified: Thu Apr 13 21:01:57 2023, max compression
+gzip compressed data, was "pyproject-generator-0.0.3.tar", last modified: Sun Apr 16 17:45:19 2023, max compression
```

## Comparing `pyproject-generator-0.0.2.tar` & `pyproject-generator-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-13 21:01:57.879990 pyproject-generator-0.0.2/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      518 2023-04-13 21:01:57.880227 pyproject-generator-0.0.2/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-12 22:11:58.000000 pyproject-generator-0.0.2/README.md
--rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-12 22:11:58.000000 pyproject-generator-0.0.2/pyproject.toml
--rw-r--r--   0 cangyuanli   (501) staff       (20)      824 2023-04-13 21:01:57.881625 pyproject-generator-0.0.2/setup.cfg
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-13 21:01:57.864064 pyproject-generator-0.0.2/src/
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-13 21:01:57.868564 pyproject-generator-0.0.2/src/pyproject/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-13 20:46:07.000000 pyproject-generator-0.0.2/src/pyproject/__init__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-13 21:01:49.000000 pyproject-generator-0.0.2/src/pyproject/__version__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)      799 2023-04-13 20:45:19.000000 pyproject-generator-0.0.2/src/pyproject/cli.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     4650 2023-04-13 20:29:53.000000 pyproject-generator-0.0.2/src/pyproject/project_builder.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-13 21:01:57.875109 pyproject-generator-0.0.2/src/pyproject/templates/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1477 2023-04-13 18:28:38.000000 pyproject-generator-0.0.2/src/pyproject/templates/gitignore.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.0.2/src/pyproject/templates/pyproject.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      416 2023-04-13 18:52:00.000000 pyproject-generator-0.0.2/src/pyproject/templates/readme.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      632 2023-04-13 17:35:50.000000 pyproject-generator-0.0.2/src/pyproject/templates/setup.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.0.2/src/pyproject/templates/tests.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.0.2/src/pyproject/templates/tox.template
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-13 21:01:57.879034 pyproject-generator-0.0.2/src/pyproject_generator.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      518 2023-04-13 21:01:57.000000 pyproject-generator-0.0.2/src/pyproject_generator.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)      646 2023-04-13 21:01:57.000000 pyproject-generator-0.0.2/src/pyproject_generator.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-13 21:01:57.000000 pyproject-generator-0.0.2/src/pyproject_generator.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-13 21:01:57.000000 pyproject-generator-0.0.2/src/pyproject_generator.egg-info/entry_points.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-13 21:01:57.000000 pyproject-generator-0.0.2/src/pyproject_generator.egg-info/top_level.txt
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-13 21:01:57.879607 pyproject-generator-0.0.2/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-12 22:11:58.000000 pyproject-generator-0.0.2/tests/test_pyproject.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-16 17:45:19.609700 pyproject-generator-0.0.3/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1159 2023-04-16 17:45:19.609886 pyproject-generator-0.0.3/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      640 2023-04-13 21:07:05.000000 pyproject-generator-0.0.3/README.md
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      232 2023-04-12 22:11:58.000000 pyproject-generator-0.0.3/pyproject.toml
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      834 2023-04-16 17:45:19.611256 pyproject-generator-0.0.3/setup.cfg
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-16 17:45:19.570465 pyproject-generator-0.0.3/src/
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-16 17:45:19.580610 pyproject-generator-0.0.3/src/pyproject/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       37 2023-04-13 20:46:07.000000 pyproject-generator-0.0.3/src/pyproject/__init__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-04-16 17:45:10.000000 pyproject-generator-0.0.3/src/pyproject/__version__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2361 2023-04-15 15:52:22.000000 pyproject-generator-0.0.3/src/pyproject/cli.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-16 17:45:19.581602 pyproject-generator-0.0.3/src/pyproject/config/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-16 17:42:35.000000 pyproject-generator-0.0.3/src/pyproject/config/config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     7346 2023-04-16 17:44:32.000000 pyproject-generator-0.0.3/src/pyproject/project_builder.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-16 17:45:19.597284 pyproject-generator-0.0.3/src/pyproject/templates/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1477 2023-04-13 18:28:38.000000 pyproject-generator-0.0.3/src/pyproject/templates/gitignore.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      231 2023-04-12 23:53:39.000000 pyproject-generator-0.0.3/src/pyproject/templates/pyproject.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      398 2023-04-14 17:01:55.000000 pyproject-generator-0.0.3/src/pyproject/templates/readme.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      578 2023-04-14 17:03:04.000000 pyproject-generator-0.0.3/src/pyproject/templates/setup.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.0.3/src/pyproject/templates/tests.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.0.3/src/pyproject/templates/tox.template
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-16 17:45:19.608485 pyproject-generator-0.0.3/src/pyproject_generator.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1159 2023-04-16 17:45:19.000000 pyproject-generator-0.0.3/src/pyproject_generator.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      679 2023-04-16 17:45:19.000000 pyproject-generator-0.0.3/src/pyproject_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-04-16 17:45:19.000000 pyproject-generator-0.0.3/src/pyproject_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-04-16 17:45:19.000000 pyproject-generator-0.0.3/src/pyproject_generator.egg-info/entry_points.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-04-16 17:45:19.000000 pyproject-generator-0.0.3/src/pyproject_generator.egg-info/top_level.txt
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-04-16 17:45:19.609307 pyproject-generator-0.0.3/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-12 22:11:58.000000 pyproject-generator-0.0.3/tests/test_pyproject.py
```

### Comparing `pyproject-generator-0.0.2/setup.cfg` & `pyproject-generator-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 [options.packages.find]
 where = src
 
 [options.package_data]
 pyproject = 
 	py.typed
 	templates/*
+	config/*
 
 [options.entry_points]
 console_scripts = 
 	pyproject = pyproject.cli:main
 
 [egg_info]
 tag_build =
```

### Comparing `pyproject-generator-0.0.2/src/pyproject/templates/gitignore.template` & `pyproject-generator-0.0.3/src/pyproject/templates/gitignore.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.2/src/pyproject/templates/setup.template` & `pyproject-generator-0.0.3/src/pyproject/templates/setup.template`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = $PACKAGE
 version = 0.0.0
-author = Cangyuan Li
-author_email = everest229@gmail.com
+author = $AUTHOR
+author_email = $EMAIL
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/CangyuanLi/$PACKAGE
+url = $GITHUB_URL/$PACKAGE
 project_urls =
-    Bug Tracker = https://github.com/CangyuanLi/$PACKAGE/issues
+    Bug Tracker = $GITHUB_URL/$PACKAGE/issues
 classifiers =
     Programming Language :: Python :: 3
     License :: OSI Approved :: MIT License
     Operating System :: OS Independent
 
 [options]
 package_dir =
```

### Comparing `pyproject-generator-0.0.2/src/pyproject/templates/tests.template` & `pyproject-generator-0.0.3/src/pyproject/templates/tests.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.0.2/src/pyproject_generator.egg-info/SOURCES.txt` & `pyproject-generator-0.0.3/src/pyproject_generator.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 README.md
 pyproject.toml
 setup.cfg
 src/pyproject/__init__.py
 src/pyproject/__version__.py
 src/pyproject/cli.py
 src/pyproject/project_builder.py
+src/pyproject/config/config.json
 src/pyproject/templates/gitignore.template
 src/pyproject/templates/pyproject.template
 src/pyproject/templates/readme.template
 src/pyproject/templates/setup.template
 src/pyproject/templates/tests.template
 src/pyproject/templates/tox.template
 src/pyproject_generator.egg-info/PKG-INFO
```

