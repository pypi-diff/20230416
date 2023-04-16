# Comparing `tmp/karpyncho-reload-urls-0.1.0.tar.gz` & `tmp/karpyncho-reload-urls-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karpyncho-reload-urls-0.1.0.tar", last modified: Tue Apr  4 21:17:29 2023, max compression
+gzip compressed data, was "karpyncho-reload-urls-0.1.1.tar", last modified: Sun Apr 16 01:46:01 2023, max compression
```

## Comparing `karpyncho-reload-urls-0.1.0.tar` & `karpyncho-reload-urls-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:17:29.217270 karpyncho-reload-urls-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-04 21:17:18.000000 karpyncho-reload-urls-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-04 21:17:18.000000 karpyncho-reload-urls-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-04 21:17:18.000000 karpyncho-reload-urls-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-04 21:17:29.217270 karpyncho-reload-urls-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-04 21:17:18.000000 karpyncho-reload-urls-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-04 21:17:18.000000 karpyncho-reload-urls-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-04 21:17:18.000000 karpyncho-reload-urls-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 21:17:29.217270 karpyncho-reload-urls-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:17:29.213271 karpyncho-reload-urls-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:17:29.213271 karpyncho-reload-urls-0.1.0/src/karpyncho/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 21:17:18.000000 karpyncho-reload-urls-0.1.0/src/karpyncho/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:17:29.213271 karpyncho-reload-urls-0.1.0/src/karpyncho/reload_urls/
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-04 21:17:18.000000 karpyncho-reload-urls-0.1.0/src/karpyncho/reload_urls/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:17:29.213271 karpyncho-reload-urls-0.1.0/src/karpyncho_reload_urls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-04 21:17:29.000000 karpyncho-reload-urls-0.1.0/src/karpyncho_reload_urls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-04 21:17:29.000000 karpyncho-reload-urls-0.1.0/src/karpyncho_reload_urls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 21:17:29.000000 karpyncho-reload-urls-0.1.0/src/karpyncho_reload_urls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-04 21:17:29.000000 karpyncho-reload-urls-0.1.0/src/karpyncho_reload_urls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-04 21:17:29.000000 karpyncho-reload-urls-0.1.0/src/karpyncho_reload_urls.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-04 21:17:18.000000 karpyncho-reload-urls-0.1.0/src/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 21:17:29.217270 karpyncho-reload-urls-0.1.0/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 21:17:18.000000 karpyncho-reload-urls-0.1.0/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-04 21:17:18.000000 karpyncho-reload-urls-0.1.0/src/tests/another_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-04 21:17:18.000000 karpyncho-reload-urls-0.1.0/src/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-04 21:17:18.000000 karpyncho-reload-urls-0.1.0/src/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-04 21:17:18.000000 karpyncho-reload-urls-0.1.0/src/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:46:01.912649 karpyncho-reload-urls-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-16 01:45:50.000000 karpyncho-reload-urls-0.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-16 01:45:50.000000 karpyncho-reload-urls-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-16 01:45:50.000000 karpyncho-reload-urls-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-16 01:46:01.912649 karpyncho-reload-urls-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-16 01:45:50.000000 karpyncho-reload-urls-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-04-16 01:45:50.000000 karpyncho-reload-urls-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-16 01:45:50.000000 karpyncho-reload-urls-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 01:46:01.912649 karpyncho-reload-urls-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:46:01.912649 karpyncho-reload-urls-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:46:01.908649 karpyncho-reload-urls-0.1.1/src/karpyncho/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:46:01.912649 karpyncho-reload-urls-0.1.1/src/karpyncho/reload_urls/
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-04-16 01:45:50.000000 karpyncho-reload-urls-0.1.1/src/karpyncho/reload_urls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:46:01.912649 karpyncho-reload-urls-0.1.1/src/karpyncho_reload_urls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-16 01:46:01.000000 karpyncho-reload-urls-0.1.1/src/karpyncho_reload_urls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-16 01:46:01.000000 karpyncho-reload-urls-0.1.1/src/karpyncho_reload_urls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 01:46:01.000000 karpyncho-reload-urls-0.1.1/src/karpyncho_reload_urls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-16 01:46:01.000000 karpyncho-reload-urls-0.1.1/src/karpyncho_reload_urls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-16 01:46:01.000000 karpyncho-reload-urls-0.1.1/src/karpyncho_reload_urls.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-04-16 01:45:50.000000 karpyncho-reload-urls-0.1.1/src/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 01:46:01.912649 karpyncho-reload-urls-0.1.1/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 01:45:50.000000 karpyncho-reload-urls-0.1.1/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-16 01:45:50.000000 karpyncho-reload-urls-0.1.1/src/tests/another_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-16 01:45:50.000000 karpyncho-reload-urls-0.1.1/src/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-16 01:45:50.000000 karpyncho-reload-urls-0.1.1/src/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-16 01:45:50.000000 karpyncho-reload-urls-0.1.1/src/tests/urls.py
```

### Comparing `karpyncho-reload-urls-0.1.0/LICENSE` & `karpyncho-reload-urls-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `karpyncho-reload-urls-0.1.0/PKG-INFO` & `karpyncho-reload-urls-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: karpyncho-reload-urls
-Version: 0.1.0
-Summary: A contex manaager to reload urls routing in unittests changing a django setting.
+Version: 0.1.1
+Summary: A context manaager to reload urls routing in unittests changing a django setting.
 Author-email: Sebastian Quiles <qsebas@gmail.com>
 Project-URL: homepage, https://github.com/karpyncho/reload-urls
 Project-URL: repository, https://github.com/karpyncho/reload-urls
 Project-URL: changelog, https://github.com/karpyncho/reload-urls/blob/main/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `karpyncho-reload-urls-0.1.0/README.md` & `karpyncho-reload-urls-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `karpyncho-reload-urls-0.1.0/pyproject.toml` & `karpyncho-reload-urls-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["wheel", "setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "karpyncho-reload-urls"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     {name = "Sebastian Quiles", email = "qsebas@gmail.com"},
 ]
-description = "A contex manaager to reload urls routing in unittests changing a django setting."
+description = "A context manaager to reload urls routing in unittests changing a django setting."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
```

### Comparing `karpyncho-reload-urls-0.1.0/src/karpyncho/reload_urls/__init__.py` & `karpyncho-reload-urls-0.1.1/src/karpyncho/reload_urls/__init__.py`

 * *Files identical despite different names*

### Comparing `karpyncho-reload-urls-0.1.0/src/karpyncho_reload_urls.egg-info/PKG-INFO` & `karpyncho-reload-urls-0.1.1/src/karpyncho_reload_urls.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: karpyncho-reload-urls
-Version: 0.1.0
-Summary: A contex manaager to reload urls routing in unittests changing a django setting.
+Version: 0.1.1
+Summary: A context manaager to reload urls routing in unittests changing a django setting.
 Author-email: Sebastian Quiles <qsebas@gmail.com>
 Project-URL: homepage, https://github.com/karpyncho/reload-urls
 Project-URL: repository, https://github.com/karpyncho/reload-urls
 Project-URL: changelog, https://github.com/karpyncho/reload-urls/blob/main/CHANGELOG.md
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `karpyncho-reload-urls-0.1.0/src/manage.py` & `karpyncho-reload-urls-0.1.1/src/manage.py`

 * *Files identical despite different names*

### Comparing `karpyncho-reload-urls-0.1.0/src/tests/settings.py` & `karpyncho-reload-urls-0.1.1/src/tests/settings.py`

 * *Files identical despite different names*

### Comparing `karpyncho-reload-urls-0.1.0/src/tests/test_init.py` & `karpyncho-reload-urls-0.1.1/src/tests/test_init.py`

 * *Files identical despite different names*

