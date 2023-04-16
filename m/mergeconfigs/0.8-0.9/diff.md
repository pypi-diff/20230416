# Comparing `tmp/mergeconfigs-0.8.tar.gz` & `tmp/mergeconfigs-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergeconfigs-0.8.tar", last modified: Mon Jan 23 15:03:14 2023, max compression
+gzip compressed data, was "mergeconfigs-0.9.tar", last modified: Sun Mar 19 10:05:28 2023, max compression
```

## Comparing `mergeconfigs-0.8.tar` & `mergeconfigs-0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwx------   0 x41       (1000) x41       (1000)        0 2023-01-23 15:03:14.309364 mergeconfigs-0.8/
--rw-------   0 x41       (1000) x41       (1000)     1070 2023-01-19 09:21:22.000000 mergeconfigs-0.8/LICENSE.txt
--rw-------   0 x41       (1000) x41       (1000)     5233 2023-01-23 15:03:14.309364 mergeconfigs-0.8/PKG-INFO
--rw-------   0 x41       (1000) x41       (1000)     4827 2023-01-23 15:01:22.000000 mergeconfigs-0.8/README.md
-drwx------   0 x41       (1000) x41       (1000)        0 2023-01-23 15:03:14.309364 mergeconfigs-0.8/mergeconfigs/
--rw-------   0 x41       (1000) x41       (1000)       61 2023-01-19 09:00:44.000000 mergeconfigs-0.8/mergeconfigs/__main__.py
--rw-------   0 x41       (1000) x41       (1000)      670 2023-01-19 15:25:30.000000 mergeconfigs-0.8/mergeconfigs/cli.py
--rw-------   0 x41       (1000) x41       (1000)     3559 2023-01-23 15:00:35.000000 mergeconfigs-0.8/mergeconfigs/config_builder.py
-drwx------   0 x41       (1000) x41       (1000)        0 2023-01-23 15:03:14.309364 mergeconfigs-0.8/mergeconfigs.egg-info/
--rw-------   0 x41       (1000) x41       (1000)     5233 2023-01-23 15:03:14.000000 mergeconfigs-0.8/mergeconfigs.egg-info/PKG-INFO
--rw-------   0 x41       (1000) x41       (1000)      300 2023-01-23 15:03:14.000000 mergeconfigs-0.8/mergeconfigs.egg-info/SOURCES.txt
--rw-------   0 x41       (1000) x41       (1000)        1 2023-01-23 15:03:14.000000 mergeconfigs-0.8/mergeconfigs.egg-info/dependency_links.txt
--rw-------   0 x41       (1000) x41       (1000)       18 2023-01-23 15:03:14.000000 mergeconfigs-0.8/mergeconfigs.egg-info/requires.txt
--rw-------   0 x41       (1000) x41       (1000)       13 2023-01-23 15:03:14.000000 mergeconfigs-0.8/mergeconfigs.egg-info/top_level.txt
--rw-------   0 x41       (1000) x41       (1000)       85 2023-01-19 09:19:37.000000 mergeconfigs-0.8/pyproject.toml
--rw-------   0 x41       (1000) x41       (1000)       38 2023-01-23 15:03:14.309364 mergeconfigs-0.8/setup.cfg
--rw-------   0 x41       (1000) x41       (1000)      708 2023-01-23 15:01:44.000000 mergeconfigs-0.8/setup.py
+drwx------   0 x41       (1000) x41       (1000)        0 2023-03-19 10:05:27.996784 mergeconfigs-0.9/
+-rw-------   0 x41       (1000) x41       (1000)     1070 2023-01-19 09:21:22.000000 mergeconfigs-0.9/LICENSE.txt
+-rw-------   0 x41       (1000) x41       (1000)     5233 2023-03-19 10:05:27.996784 mergeconfigs-0.9/PKG-INFO
+-rw-------   0 x41       (1000) x41       (1000)     4827 2023-01-23 15:01:22.000000 mergeconfigs-0.9/README.md
+drwx------   0 x41       (1000) x41       (1000)        0 2023-03-19 10:05:27.992784 mergeconfigs-0.9/mergeconfigs/
+-rw-------   0 x41       (1000) x41       (1000)       61 2023-01-19 09:00:44.000000 mergeconfigs-0.9/mergeconfigs/__main__.py
+-rw-------   0 x41       (1000) x41       (1000)      670 2023-01-19 15:25:30.000000 mergeconfigs-0.9/mergeconfigs/cli.py
+-rw-------   0 x41       (1000) x41       (1000)     3622 2023-03-19 10:00:48.000000 mergeconfigs-0.9/mergeconfigs/config_builder.py
+drwx------   0 x41       (1000) x41       (1000)        0 2023-03-19 10:05:27.996784 mergeconfigs-0.9/mergeconfigs.egg-info/
+-rw-------   0 x41       (1000) x41       (1000)     5233 2023-03-19 10:05:27.000000 mergeconfigs-0.9/mergeconfigs.egg-info/PKG-INFO
+-rw-------   0 x41       (1000) x41       (1000)      300 2023-03-19 10:05:27.000000 mergeconfigs-0.9/mergeconfigs.egg-info/SOURCES.txt
+-rw-------   0 x41       (1000) x41       (1000)        1 2023-03-19 10:05:27.000000 mergeconfigs-0.9/mergeconfigs.egg-info/dependency_links.txt
+-rw-------   0 x41       (1000) x41       (1000)       18 2023-03-19 10:05:27.000000 mergeconfigs-0.9/mergeconfigs.egg-info/requires.txt
+-rw-------   0 x41       (1000) x41       (1000)       13 2023-03-19 10:05:27.000000 mergeconfigs-0.9/mergeconfigs.egg-info/top_level.txt
+-rw-------   0 x41       (1000) x41       (1000)       85 2023-01-19 09:19:37.000000 mergeconfigs-0.9/pyproject.toml
+-rw-------   0 x41       (1000) x41       (1000)       38 2023-03-19 10:05:27.996784 mergeconfigs-0.9/setup.cfg
+-rw-------   0 x41       (1000) x41       (1000)      707 2023-03-19 10:01:02.000000 mergeconfigs-0.9/setup.py
```

### Comparing `mergeconfigs-0.8/LICENSE.txt` & `mergeconfigs-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mergeconfigs-0.8/PKG-INFO` & `mergeconfigs-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mergeconfigs
-Version: 0.8
+Version: 0.9
 Summary: Help developers with config files
 Home-page: https://github.com/x41lakazam/mergeconfigs
 Author: Eyal Chocron
 Author-email: x41lakazam@gmail.com
 Maintainer: Eyal Chocron
 Maintainer-email: x41lakazam@gmail.com
 Keywords: config,yaml,inheritance,templates
```

### Comparing `mergeconfigs-0.8/README.md` & `mergeconfigs-0.9/README.md`

 * *Files identical despite different names*

### Comparing `mergeconfigs-0.8/mergeconfigs/cli.py` & `mergeconfigs-0.9/mergeconfigs/cli.py`

 * *Files identical despite different names*

### Comparing `mergeconfigs-0.8/mergeconfigs/config_builder.py` & `mergeconfigs-0.9/mergeconfigs/config_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,18 @@
     return val
 
 
 def _resolve_yaml(file: Path, workdir=Path("."), env=".", ctx=None, callers=None):
     callers = callers or []
     ctx = ctx or {}
 
-    file_content = yaml.load(open(file.absolute()), Loader=Loader) or {}
+    if file.is_file():
+        file_content = yaml.load(open(file.absolute()), Loader=Loader) or {}
+    else:
+        file_content = {}
     # Store the content of the current file under "this" namespace
     inner_ctx = {"this": file_content}
     ctx = ctx | inner_ctx
 
     file_vars = file_content.copy()
     ctx[file.stem] = file_vars
```

### Comparing `mergeconfigs-0.8/mergeconfigs.egg-info/PKG-INFO` & `mergeconfigs-0.9/mergeconfigs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mergeconfigs
-Version: 0.8
+Version: 0.9
 Summary: Help developers with config files
 Home-page: https://github.com/x41lakazam/mergeconfigs
 Author: Eyal Chocron
 Author-email: x41lakazam@gmail.com
 Maintainer: Eyal Chocron
 Maintainer-email: x41lakazam@gmail.com
 Keywords: config,yaml,inheritance,templates
```

### Comparing `mergeconfigs-0.8/setup.py` & `mergeconfigs-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 except:
     long_description = ""
 
 
 setup(
     name='mergeconfigs',
     python_requires=">=3.7",
-    version='0.8',
+    version='0.9',
     description='Help developers with config files',
     long_description=long_description,
-    long_description_content_type="text/markdown", 
+    long_description_content_type="text/markdown",
     url="https://github.com/x41lakazam/mergeconfigs",
     author='Eyal Chocron',
     maintainer="Eyal Chocron",
     author_email='x41lakazam@gmail.com',
     maintainer_email='x41lakazam@gmail.com',
     keywords=["config", "yaml", "inheritance", "templates"],
     packages=['mergeconfigs'],
```

