# Comparing `tmp/hond-2.0.1.tar.gz` & `tmp/hond-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hond-2.0.1.tar", last modified: Sun Apr 16 15:19:57 2023, max compression
+gzip compressed data, was "hond-2.0.2.tar", last modified: Sun Apr 16 21:09:53 2023, max compression
```

## Comparing `hond-2.0.1.tar` & `hond-2.0.2.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:19:57.171876 hond-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-16 15:19:30.000000 hond-2.0.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:19:57.167876 hond-2.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-16 15:19:30.000000 hond-2.0.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 15:19:30.000000 hond-2.0.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:19:57.167876 hond-2.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-16 15:19:30.000000 hond-2.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-16 15:19:30.000000 hond-2.0.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:19:57.171876 hond-2.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-16 15:19:30.000000 hond-2.0.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-16 15:19:30.000000 hond-2.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-16 15:19:30.000000 hond-2.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-16 15:19:30.000000 hond-2.0.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-16 15:19:30.000000 hond-2.0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-16 15:19:30.000000 hond-2.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-16 15:19:30.000000 hond-2.0.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 15:19:30.000000 hond-2.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-16 15:19:30.000000 hond-2.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-16 15:19:57.171876 hond-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-16 15:19:30.000000 hond-2.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:19:57.171876 hond-2.0.1/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-16 15:19:30.000000 hond-2.0.1/cache/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:19:57.171876 hond-2.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-16 15:19:30.000000 hond-2.0.1/examples/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-16 15:19:30.000000 hond-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 15:19:30.000000 hond-2.0.1/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-16 15:19:57.171876 hond-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-16 15:19:30.000000 hond-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:19:57.167876 hond-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:19:57.171876 hond-2.0.1/src/hond/
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-16 15:19:30.000000 hond-2.0.1/src/hond/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:19:57.171876 hond-2.0.1/src/hond/driver/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 15:19:30.000000 hond-2.0.1/src/hond/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13341 2023-04-16 15:19:30.000000 hond-2.0.1/src/hond/driver/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-16 15:19:30.000000 hond-2.0.1/src/hond/hond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-16 15:19:30.000000 hond-2.0.1/src/hond/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-16 15:19:30.000000 hond-2.0.1/src/hond/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-16 15:19:30.000000 hond-2.0.1/src/hond/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:19:57.171876 hond-2.0.1/src/hond.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-16 15:19:57.000000 hond-2.0.1/src/hond.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-16 15:19:57.000000 hond-2.0.1/src/hond.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 15:19:57.000000 hond-2.0.1/src/hond.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 15:19:56.000000 hond-2.0.1/src/hond.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-16 15:19:57.000000 hond-2.0.1/src/hond.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-16 15:19:57.000000 hond-2.0.1/src/hond.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:19:57.171876 hond-2.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 15:19:30.000000 hond-2.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:19:57.171876 hond-2.0.1/tests/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 15:19:30.000000 hond-2.0.1/tests/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-16 15:19:30.000000 hond-2.0.1/tests/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-16 15:19:30.000000 hond-2.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:09:53.293479 hond-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-16 21:09:22.000000 hond-2.0.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:09:53.289479 hond-2.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-16 21:09:22.000000 hond-2.0.2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 21:09:22.000000 hond-2.0.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:09:53.289479 hond-2.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-16 21:09:22.000000 hond-2.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-16 21:09:22.000000 hond-2.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:09:53.289479 hond-2.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-16 21:09:22.000000 hond-2.0.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-16 21:09:22.000000 hond-2.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-16 21:09:22.000000 hond-2.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-16 21:09:22.000000 hond-2.0.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-16 21:09:22.000000 hond-2.0.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-16 21:09:22.000000 hond-2.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-16 21:09:22.000000 hond-2.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 21:09:22.000000 hond-2.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-16 21:09:22.000000 hond-2.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-16 21:09:53.293479 hond-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-04-16 21:09:22.000000 hond-2.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:09:53.289479 hond-2.0.2/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-16 21:09:22.000000 hond-2.0.2/cache/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:09:53.289479 hond-2.0.2/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)    74544 2023-04-16 21:09:22.000000 hond-2.0.2/chart/chart.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:09:53.289479 hond-2.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-16 21:09:22.000000 hond-2.0.2/examples/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-16 21:09:22.000000 hond-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 21:09:22.000000 hond-2.0.2/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-16 21:09:53.293479 hond-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-16 21:09:22.000000 hond-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:09:53.285479 hond-2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:09:53.289479 hond-2.0.2/src/hond/
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-16 21:09:22.000000 hond-2.0.2/src/hond/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:09:53.293479 hond-2.0.2/src/hond/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 21:09:22.000000 hond-2.0.2/src/hond/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13341 2023-04-16 21:09:22.000000 hond-2.0.2/src/hond/driver/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-16 21:09:22.000000 hond-2.0.2/src/hond/hond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-16 21:09:22.000000 hond-2.0.2/src/hond/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-16 21:09:22.000000 hond-2.0.2/src/hond/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-16 21:09:22.000000 hond-2.0.2/src/hond/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:09:53.293479 hond-2.0.2/src/hond.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-16 21:09:53.000000 hond-2.0.2/src/hond.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-16 21:09:53.000000 hond-2.0.2/src/hond.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 21:09:53.000000 hond-2.0.2/src/hond.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 21:09:52.000000 hond-2.0.2/src/hond.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-16 21:09:53.000000 hond-2.0.2/src/hond.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-16 21:09:53.000000 hond-2.0.2/src/hond.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:09:53.293479 hond-2.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 21:09:22.000000 hond-2.0.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:09:53.293479 hond-2.0.2/tests/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 21:09:22.000000 hond-2.0.2/tests/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-16 21:09:22.000000 hond-2.0.2/tests/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-16 21:09:22.000000 hond-2.0.2/tox.ini
```

### Comparing `hond-2.0.1/.coveragerc` & `hond-2.0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `hond-2.0.1/.github/workflows/release.yml` & `hond-2.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hond-2.0.1/.gitignore` & `hond-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hond-2.0.1/CODE_OF_CONDUCT.md` & `hond-2.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hond-2.0.1/CONTRIBUTING.rst` & `hond-2.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hond-2.0.1/LICENSE.txt` & `hond-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hond-2.0.1/Makefile` & `hond-2.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `hond-2.0.1/PKG-INFO` & `hond-2.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hond
-Version: 2.0.1
+Version: 2.0.2
 Summary: Metrics Ingestion and Alerting Reimagined.
 Home-page: https://github.com/uptimedog/hond/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/uptimedog/hond/
 Project-URL: Source, https://github.com/uptimedog/hond/
@@ -24,17 +24,22 @@
     :target: https://pypi.org/project/Hond/
 .. image:: https://github.com/Uptimedog/Hond/actions/workflows/ci.yml/badge.svg
     :alt: Build Status
     :target: https://github.com/Uptimedog/Hond/actions/workflows/ci.yml
 
 |
 
-========
+.. image:: https://raw.githubusercontent.com/Uptimedog/Hond/main/chart/chart.png
+   :width: 100%
+
+|
+
+=====
 Hond
-========
+=====
 
     Metrics Ingestion and Alerting Reimagined.
 
 
 Note
 ====
```

### Comparing `hond-2.0.1/examples/basic.py` & `hond-2.0.2/examples/basic.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.1/setup.cfg` & `hond-2.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `hond-2.0.1/setup.py` & `hond-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.1/src/hond/__init__.py` & `hond-2.0.2/src/hond/__init__.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.1/src/hond/driver/__init__.py` & `hond-2.0.2/src/hond/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.1/src/hond/driver/elasticsearch.py` & `hond-2.0.2/src/hond/driver/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.1/src/hond/hond.py` & `hond-2.0.2/src/hond/hond.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.1/src/hond/logger.py` & `hond-2.0.2/src/hond/logger.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.1/src/hond/metric.py` & `hond-2.0.2/src/hond/metric.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.1/src/hond/trigger.py` & `hond-2.0.2/src/hond/trigger.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.1/src/hond.egg-info/PKG-INFO` & `hond-2.0.2/src/hond.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hond
-Version: 2.0.1
+Version: 2.0.2
 Summary: Metrics Ingestion and Alerting Reimagined.
 Home-page: https://github.com/uptimedog/hond/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/uptimedog/hond/
 Project-URL: Source, https://github.com/uptimedog/hond/
@@ -24,17 +24,22 @@
     :target: https://pypi.org/project/Hond/
 .. image:: https://github.com/Uptimedog/Hond/actions/workflows/ci.yml/badge.svg
     :alt: Build Status
     :target: https://github.com/Uptimedog/Hond/actions/workflows/ci.yml
 
 |
 
-========
+.. image:: https://raw.githubusercontent.com/Uptimedog/Hond/main/chart/chart.png
+   :width: 100%
+
+|
+
+=====
 Hond
-========
+=====
 
     Metrics Ingestion and Alerting Reimagined.
 
 
 Note
 ====
```

### Comparing `hond-2.0.1/src/hond.egg-info/SOURCES.txt` & `hond-2.0.2/src/hond.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 .github/CODEOWNERS
 .github/FUNDING.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/ci.yml
 .github/workflows/release.yml
 cache/.gitignore
+chart/chart.png
 examples/basic.py
 src/hond/__init__.py
 src/hond/hond.py
 src/hond/logger.py
 src/hond/metric.py
 src/hond/trigger.py
 src/hond.egg-info/PKG-INFO
```

### Comparing `hond-2.0.1/tests/__init__.py` & `hond-2.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.1/tests/datastore/__init__.py` & `hond-2.0.2/tests/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.1/tests/test_metric.py` & `hond-2.0.2/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `hond-2.0.1/tox.ini` & `hond-2.0.2/tox.ini`

 * *Files identical despite different names*

