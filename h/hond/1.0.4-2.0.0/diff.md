# Comparing `tmp/hond-1.0.4.tar.gz` & `tmp/hond-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hond-1.0.4.tar", last modified: Sun Apr 16 02:58:56 2023, max compression
+gzip compressed data, was "hond-2.0.0.tar", last modified: Sun Apr 16 14:11:18 2023, max compression
```

## Comparing `hond-1.0.4.tar` & `hond-2.0.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.323442 hond-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-16 02:58:22.000000 hond-1.0.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.315442 hond-1.0.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-16 02:58:22.000000 hond-1.0.4/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 02:58:22.000000 hond-1.0.4/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.315442 hond-1.0.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-16 02:58:22.000000 hond-1.0.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-16 02:58:22.000000 hond-1.0.4/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.315442 hond-1.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-16 02:58:22.000000 hond-1.0.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-16 02:58:22.000000 hond-1.0.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-16 02:58:22.000000 hond-1.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-16 02:58:22.000000 hond-1.0.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-16 02:58:22.000000 hond-1.0.4/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-16 02:58:22.000000 hond-1.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-16 02:58:22.000000 hond-1.0.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 02:58:22.000000 hond-1.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-16 02:58:22.000000 hond-1.0.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-16 02:58:56.323442 hond-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-16 02:58:22.000000 hond-1.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.319442 hond-1.0.4/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-16 02:58:22.000000 hond-1.0.4/cache/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.319442 hond-1.0.4/chart/
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-04-16 02:58:22.000000 hond-1.0.4/chart/idog.drawio
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.319442 hond-1.0.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-16 02:58:22.000000 hond-1.0.4/examples/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-16 02:58:22.000000 hond-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 02:58:22.000000 hond-1.0.4/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-16 02:58:56.323442 hond-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-16 02:58:22.000000 hond-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.311442 hond-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.319442 hond-1.0.4/src/hond/
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-16 02:58:22.000000 hond-1.0.4/src/hond/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.323442 hond-1.0.4/src/hond/driver/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 02:58:22.000000 hond-1.0.4/src/hond/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-04-16 02:58:22.000000 hond-1.0.4/src/hond/driver/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-16 02:58:22.000000 hond-1.0.4/src/hond/hond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-16 02:58:22.000000 hond-1.0.4/src/hond/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-16 02:58:22.000000 hond-1.0.4/src/hond/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-16 02:58:22.000000 hond-1.0.4/src/hond/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.323442 hond-1.0.4/src/hond.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-16 02:58:56.000000 hond-1.0.4/src/hond.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-16 02:58:56.000000 hond-1.0.4/src/hond.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 02:58:56.000000 hond-1.0.4/src/hond.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 02:58:55.000000 hond-1.0.4/src/hond.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-16 02:58:56.000000 hond-1.0.4/src/hond.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-16 02:58:56.000000 hond-1.0.4/src/hond.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.323442 hond-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 02:58:22.000000 hond-1.0.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.323442 hond-1.0.4/tests/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 02:58:22.000000 hond-1.0.4/tests/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-16 02:58:22.000000 hond-1.0.4/tests/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-16 02:58:22.000000 hond-1.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:11:18.607175 hond-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-16 14:10:47.000000 hond-2.0.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:11:18.599175 hond-2.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-16 14:10:47.000000 hond-2.0.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 14:10:47.000000 hond-2.0.0/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:11:18.599175 hond-2.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-16 14:10:47.000000 hond-2.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-16 14:10:47.000000 hond-2.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:11:18.599175 hond-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-16 14:10:47.000000 hond-2.0.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-16 14:10:47.000000 hond-2.0.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-16 14:10:47.000000 hond-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-16 14:10:47.000000 hond-2.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-16 14:10:47.000000 hond-2.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-16 14:10:47.000000 hond-2.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-16 14:10:47.000000 hond-2.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 14:10:47.000000 hond-2.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-16 14:10:47.000000 hond-2.0.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-16 14:11:18.607175 hond-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-16 14:10:47.000000 hond-2.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:11:18.599175 hond-2.0.0/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-16 14:10:47.000000 hond-2.0.0/cache/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:11:18.599175 hond-2.0.0/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-04-16 14:10:47.000000 hond-2.0.0/chart/idog.drawio
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:11:18.599175 hond-2.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-16 14:10:47.000000 hond-2.0.0/examples/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-16 14:10:47.000000 hond-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 14:10:47.000000 hond-2.0.0/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-16 14:11:18.607175 hond-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-16 14:10:47.000000 hond-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:11:18.599175 hond-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:11:18.599175 hond-2.0.0/src/hond/
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-16 14:10:47.000000 hond-2.0.0/src/hond/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:11:18.603175 hond-2.0.0/src/hond/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 14:10:47.000000 hond-2.0.0/src/hond/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13341 2023-04-16 14:10:47.000000 hond-2.0.0/src/hond/driver/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-16 14:10:47.000000 hond-2.0.0/src/hond/hond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-16 14:10:47.000000 hond-2.0.0/src/hond/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-16 14:10:47.000000 hond-2.0.0/src/hond/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-16 14:10:47.000000 hond-2.0.0/src/hond/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:11:18.603175 hond-2.0.0/src/hond.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-16 14:11:18.000000 hond-2.0.0/src/hond.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-16 14:11:18.000000 hond-2.0.0/src/hond.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 14:11:18.000000 hond-2.0.0/src/hond.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 14:11:18.000000 hond-2.0.0/src/hond.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-16 14:11:18.000000 hond-2.0.0/src/hond.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-16 14:11:18.000000 hond-2.0.0/src/hond.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:11:18.603175 hond-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 14:10:47.000000 hond-2.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:11:18.607175 hond-2.0.0/tests/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 14:10:47.000000 hond-2.0.0/tests/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-16 14:10:47.000000 hond-2.0.0/tests/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-16 14:10:47.000000 hond-2.0.0/tox.ini
```

### Comparing `hond-1.0.4/.coveragerc` & `hond-2.0.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `hond-1.0.4/.github/workflows/release.yml` & `hond-2.0.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hond-1.0.4/.gitignore` & `hond-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hond-1.0.4/CODE_OF_CONDUCT.md` & `hond-2.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hond-1.0.4/CONTRIBUTING.rst` & `hond-2.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hond-1.0.4/LICENSE.txt` & `hond-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hond-1.0.4/Makefile` & `hond-2.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `hond-1.0.4/PKG-INFO` & `hond-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hond
-Version: 1.0.4
+Version: 2.0.0
 Summary: Metrics Ingestion and Alerting Reimagined.
 Home-page: https://github.com/uptimedog/hond/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/uptimedog/hond/
 Project-URL: Source, https://github.com/uptimedog/hond/
```

### Comparing `hond-1.0.4/chart/idog.drawio` & `hond-2.0.0/chart/idog.drawio`

 * *Files identical despite different names*

### Comparing `hond-1.0.4/setup.cfg` & `hond-2.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `hond-1.0.4/setup.py` & `hond-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.4/src/hond/__init__.py` & `hond-2.0.0/src/hond/__init__.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.4/src/hond/driver/__init__.py` & `hond-2.0.0/src/hond/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.4/src/hond/driver/elasticsearch.py` & `hond-2.0.0/src/hond/driver/elasticsearch.py`

 * *Files 3% similar despite different names*

```diff
@@ -349,15 +349,15 @@
 
     def search(self, query):
         """
         Query elasticsearch index
         """
         return self.client.search(index=self.index_name, body=query)
 
-    def evaluate(expression):
+    def evaluate(self, expression):
         """
         Evaluate a trigger value
 
         Examples:
             m{customers.123.456.789.cpu>=20}[30s]
             m{customers.123.456.789.cpu<20}[30s]
             m{customers.123.456.789.cpu==nul}[30s]
@@ -365,43 +365,51 @@
 
         TODO: switch to safer way other than eval but right now triggers is not a user input
         """
         result = []
         expressions = re.split(" and | or ", expression)
 
         for exp in expressions:
-            pattern = r"^(m)\{(.*)\}(\[(.*)\])?$"
+            pattern = r"^(m)\{(.*)\}(\[(.*)s\])?$"
             match = re.match(pattern, exp)
             if match:
                 items = re.split(">=|<=|==|>|<", match.group(2))
 
                 if items[1] == "nul":
                     metric_name = items[0]
-                    for_in_sec = int(match.group(4))
+
+                    try:
+                        for_in_sec = int(match.group(4))
+                    except Exception:
+                        raise Exception("Invalid expression: {}".format(exp))
 
                     value = self.is_absent(metric_name, for_in_sec)
                 else:
                     metric_name = items[0]
-                    benchmark = float(items[1])
-                    for_in_sec = int(match.group(4))
+
+                    try:
+                        benchmark = float(items[1])
+                        for_in_sec = int(match.group(4))
+                    except Exception:
+                        raise Exception("Invalid expression: {}".format(exp))
 
                     if "==" in match.group(2):
-                        value = self.equal(self, metric_name, benchmark, for_in_sec)
+                        value = self.equal(metric_name, benchmark, for_in_sec)
                     elif ">=" in match.group(2):
                         value = self.above_equal(
-                            self, metric_name, benchmark, for_in_sec
+                            metric_name, benchmark, for_in_sec
                         )
                     elif "<=" in match.group(2):
                         value = self.below_equal(
-                            self, metric_name, benchmark, for_in_sec
+                            metric_name, benchmark, for_in_sec
                         )
                     elif ">" in match.group(2):
-                        value = self.above(self, metric_name, benchmark, for_in_sec)
+                        value = self.above(metric_name, benchmark, for_in_sec)
                     elif "<" in match.group(2):
-                        value = self.below(self, metric_name, benchmark, for_in_sec)
+                        value = self.below(metric_name, benchmark, for_in_sec)
 
                 if value:
                     result.append("True")
                 else:
                     result.append("False")
             else:
                 raise Exception("Invalid expression: {}".format(exp))
```

### Comparing `hond-1.0.4/src/hond/hond.py` & `hond-2.0.0/src/hond/hond.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,12 +26,12 @@
 class Hond:
     """Hond Class"""
 
     def __init__(self, driver):
         self.logger = Logger().get_logger(__name__)
         self.driver = driver
 
-    def insert(metric):
+    def insert(self, metric):
         return self.driver.insert(metric)
 
-    def evaluate(trigger):
-        return self.driver.evaluate(trigger)
+    def evaluate(self, trigger):
+        return self.driver.evaluate(trigger.value)
```

### Comparing `hond-1.0.4/src/hond/logger.py` & `hond-2.0.0/src/hond/logger.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.4/src/hond/metric.py` & `hond-2.0.0/src/hond/metric.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.4/src/hond/trigger.py` & `hond-2.0.0/src/hond/trigger.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.4/src/hond.egg-info/PKG-INFO` & `hond-2.0.0/src/hond.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hond
-Version: 1.0.4
+Version: 2.0.0
 Summary: Metrics Ingestion and Alerting Reimagined.
 Home-page: https://github.com/uptimedog/hond/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/uptimedog/hond/
 Project-URL: Source, https://github.com/uptimedog/hond/
```

### Comparing `hond-1.0.4/src/hond.egg-info/SOURCES.txt` & `hond-2.0.0/src/hond.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hond-1.0.4/tests/__init__.py` & `hond-2.0.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.4/tests/datastore/__init__.py` & `hond-2.0.0/tests/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.4/tests/test_metric.py` & `hond-2.0.0/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.4/tox.ini` & `hond-2.0.0/tox.ini`

 * *Files identical despite different names*

