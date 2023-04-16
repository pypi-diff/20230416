# Comparing `tmp/hond-1.0.3.tar.gz` & `tmp/hond-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hond-1.0.3.tar", last modified: Sun Apr 16 02:56:26 2023, max compression
+gzip compressed data, was "hond-1.0.4.tar", last modified: Sun Apr 16 02:58:56 2023, max compression
```

## Comparing `hond-1.0.3.tar` & `hond-1.0.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:56:26.253260 hond-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-16 02:56:00.000000 hond-1.0.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:56:26.249260 hond-1.0.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-16 02:56:00.000000 hond-1.0.3/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 02:56:00.000000 hond-1.0.3/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:56:26.249260 hond-1.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-16 02:56:00.000000 hond-1.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-16 02:56:00.000000 hond-1.0.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:56:26.249260 hond-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-16 02:56:00.000000 hond-1.0.3/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-16 02:56:00.000000 hond-1.0.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-16 02:56:00.000000 hond-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-16 02:56:00.000000 hond-1.0.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-16 02:56:00.000000 hond-1.0.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-16 02:56:00.000000 hond-1.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-16 02:56:00.000000 hond-1.0.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 02:56:00.000000 hond-1.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-16 02:56:00.000000 hond-1.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-16 02:56:26.253260 hond-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-16 02:56:00.000000 hond-1.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:56:26.249260 hond-1.0.3/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-16 02:56:00.000000 hond-1.0.3/cache/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:56:26.249260 hond-1.0.3/chart/
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-04-16 02:56:00.000000 hond-1.0.3/chart/idog.drawio
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:56:26.249260 hond-1.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-16 02:56:00.000000 hond-1.0.3/examples/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-16 02:56:00.000000 hond-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 02:56:00.000000 hond-1.0.3/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-16 02:56:26.253260 hond-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-16 02:56:00.000000 hond-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:56:26.245260 hond-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:56:26.249260 hond-1.0.3/src/hond/
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-16 02:56:00.000000 hond-1.0.3/src/hond/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:56:26.249260 hond-1.0.3/src/hond/driver/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 02:56:00.000000 hond-1.0.3/src/hond/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12538 2023-04-16 02:56:00.000000 hond-1.0.3/src/hond/driver/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-16 02:56:00.000000 hond-1.0.3/src/hond/hond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-16 02:56:00.000000 hond-1.0.3/src/hond/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-16 02:56:00.000000 hond-1.0.3/src/hond/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-16 02:56:00.000000 hond-1.0.3/src/hond/trigger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:56:26.249260 hond-1.0.3/src/hond.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-16 02:56:26.000000 hond-1.0.3/src/hond.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-16 02:56:26.000000 hond-1.0.3/src/hond.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 02:56:26.000000 hond-1.0.3/src/hond.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 02:56:25.000000 hond-1.0.3/src/hond.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-16 02:56:26.000000 hond-1.0.3/src/hond.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-16 02:56:26.000000 hond-1.0.3/src/hond.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:56:26.249260 hond-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 02:56:00.000000 hond-1.0.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:56:26.253260 hond-1.0.3/tests/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 02:56:00.000000 hond-1.0.3/tests/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-16 02:56:00.000000 hond-1.0.3/tests/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-16 02:56:00.000000 hond-1.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.323442 hond-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-16 02:58:22.000000 hond-1.0.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.315442 hond-1.0.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-16 02:58:22.000000 hond-1.0.4/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 02:58:22.000000 hond-1.0.4/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.315442 hond-1.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-16 02:58:22.000000 hond-1.0.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-16 02:58:22.000000 hond-1.0.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.315442 hond-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-16 02:58:22.000000 hond-1.0.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-16 02:58:22.000000 hond-1.0.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-16 02:58:22.000000 hond-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-16 02:58:22.000000 hond-1.0.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-16 02:58:22.000000 hond-1.0.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-16 02:58:22.000000 hond-1.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-16 02:58:22.000000 hond-1.0.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 02:58:22.000000 hond-1.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-16 02:58:22.000000 hond-1.0.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-16 02:58:56.323442 hond-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-16 02:58:22.000000 hond-1.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.319442 hond-1.0.4/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-16 02:58:22.000000 hond-1.0.4/cache/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.319442 hond-1.0.4/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-04-16 02:58:22.000000 hond-1.0.4/chart/idog.drawio
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.319442 hond-1.0.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-16 02:58:22.000000 hond-1.0.4/examples/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-16 02:58:22.000000 hond-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 02:58:22.000000 hond-1.0.4/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-16 02:58:56.323442 hond-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-16 02:58:22.000000 hond-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.311442 hond-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.319442 hond-1.0.4/src/hond/
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-16 02:58:22.000000 hond-1.0.4/src/hond/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.323442 hond-1.0.4/src/hond/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 02:58:22.000000 hond-1.0.4/src/hond/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13068 2023-04-16 02:58:22.000000 hond-1.0.4/src/hond/driver/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-16 02:58:22.000000 hond-1.0.4/src/hond/hond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-16 02:58:22.000000 hond-1.0.4/src/hond/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-16 02:58:22.000000 hond-1.0.4/src/hond/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-16 02:58:22.000000 hond-1.0.4/src/hond/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.323442 hond-1.0.4/src/hond.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-16 02:58:56.000000 hond-1.0.4/src/hond.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-16 02:58:56.000000 hond-1.0.4/src/hond.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 02:58:56.000000 hond-1.0.4/src/hond.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 02:58:55.000000 hond-1.0.4/src/hond.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-16 02:58:56.000000 hond-1.0.4/src/hond.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-16 02:58:56.000000 hond-1.0.4/src/hond.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.323442 hond-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 02:58:22.000000 hond-1.0.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:58:56.323442 hond-1.0.4/tests/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 02:58:22.000000 hond-1.0.4/tests/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-16 02:58:22.000000 hond-1.0.4/tests/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-16 02:58:22.000000 hond-1.0.4/tox.ini
```

### Comparing `hond-1.0.3/.coveragerc` & `hond-1.0.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/.github/workflows/release.yml` & `hond-1.0.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/.gitignore` & `hond-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/CODE_OF_CONDUCT.md` & `hond-1.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/CONTRIBUTING.rst` & `hond-1.0.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/LICENSE.txt` & `hond-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/Makefile` & `hond-1.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/PKG-INFO` & `hond-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hond
-Version: 1.0.3
+Version: 1.0.4
 Summary: Metrics Ingestion and Alerting Reimagined.
 Home-page: https://github.com/uptimedog/hond/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/uptimedog/hond/
 Project-URL: Source, https://github.com/uptimedog/hond/
```

### Comparing `hond-1.0.3/chart/idog.drawio` & `hond-1.0.4/chart/idog.drawio`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/examples/basic.py` & `hond-1.0.4/examples/basic.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/setup.cfg` & `hond-1.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/setup.py` & `hond-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/src/hond/__init__.py` & `hond-1.0.4/src/hond/__init__.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/src/hond/driver/__init__.py` & `hond-1.0.4/src/hond/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/src/hond/driver/elasticsearch.py` & `hond-1.0.4/src/hond/driver/elasticsearch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-# Copyright 2020 Clivern
+# MIT License
 #
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
+# Copyright (c) 2021 Clivern
 #
-#     https://www.apache.org/licenses/LICENSE-2.0
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
 #
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
 
 import re
 import time
 
 from hond.logger import Logger
 from elasticsearch import Elasticsearch
```

### Comparing `hond-1.0.3/src/hond/hond.py` & `hond-1.0.4/src/hond/hond.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/src/hond/logger.py` & `hond-1.0.4/src/hond/logger.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/src/hond/metric.py` & `hond-1.0.4/src/hond/metric.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/src/hond/trigger.py` & `hond-1.0.4/src/hond/trigger.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/src/hond.egg-info/PKG-INFO` & `hond-1.0.4/src/hond.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hond
-Version: 1.0.3
+Version: 1.0.4
 Summary: Metrics Ingestion and Alerting Reimagined.
 Home-page: https://github.com/uptimedog/hond/
 Author: Clivern
 Author-email: hello@clivern.com
 License: MIT
 Project-URL: Documentation, https://github.com/uptimedog/hond/
 Project-URL: Source, https://github.com/uptimedog/hond/
```

### Comparing `hond-1.0.3/src/hond.egg-info/SOURCES.txt` & `hond-1.0.4/src/hond.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/tests/__init__.py` & `hond-1.0.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/tests/datastore/__init__.py` & `hond-1.0.4/tests/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/tests/test_metric.py` & `hond-1.0.4/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.3/tox.ini` & `hond-1.0.4/tox.ini`

 * *Files identical despite different names*

