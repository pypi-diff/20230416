# Comparing `tmp/hond-1.0.1.tar.gz` & `tmp/hond-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hond-1.0.1.tar", last modified: Sat Apr 15 21:43:03 2023, max compression
+gzip compressed data, was "hond-1.0.2.tar", last modified: Sun Apr 16 02:53:19 2023, max compression
```

## Comparing `hond-1.0.1.tar` & `hond-1.0.2.tar`

### file list

```diff
@@ -1,61 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:43:03.843361 hond-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-15 21:42:31.000000 hond-1.0.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:43:03.835360 hond-1.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-15 21:42:31.000000 hond-1.0.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-15 21:42:31.000000 hond-1.0.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:43:03.835360 hond-1.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-15 21:42:31.000000 hond-1.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-15 21:42:31.000000 hond-1.0.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:43:03.835360 hond-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-15 21:42:31.000000 hond-1.0.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-15 21:42:31.000000 hond-1.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-15 21:42:31.000000 hond-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-15 21:42:31.000000 hond-1.0.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-15 21:42:31.000000 hond-1.0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-15 21:42:31.000000 hond-1.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-15 21:42:31.000000 hond-1.0.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-15 21:42:31.000000 hond-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-15 21:42:31.000000 hond-1.0.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-15 21:43:03.843361 hond-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-15 21:42:31.000000 hond-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:43:03.839361 hond-1.0.1/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-15 21:42:31.000000 hond-1.0.1/cache/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:43:03.839361 hond-1.0.1/chart/
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-04-15 21:42:31.000000 hond-1.0.1/chart/idog.drawio
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:43:03.839361 hond-1.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-15 21:42:31.000000 hond-1.0.1/examples/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-15 21:42:31.000000 hond-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-15 21:42:31.000000 hond-1.0.1/renovate.json
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-15 21:43:03.843361 hond-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-15 21:42:31.000000 hond-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:43:03.831360 hond-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:43:03.839361 hond-1.0.1/src/hond/
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-15 21:42:31.000000 hond-1.0.1/src/hond/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:43:03.839361 hond-1.0.1/src/hond/collect/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-15 21:42:31.000000 hond-1.0.1/src/hond/collect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-15 21:42:31.000000 hond-1.0.1/src/hond/collect/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-15 21:42:31.000000 hond-1.0.1/src/hond/collect/certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-15 21:42:31.000000 hond-1.0.1/src/hond/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-15 21:42:31.000000 hond-1.0.1/src/hond/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:43:03.839361 hond-1.0.1/src/hond/notify/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 21:42:31.000000 hond-1.0.1/src/hond/notify/.keep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:43:03.839361 hond-1.0.1/src/hond/store/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-15 21:42:31.000000 hond-1.0.1/src/hond/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-04-15 21:42:31.000000 hond-1.0.1/src/hond/store/elasticsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:43:03.839361 hond-1.0.1/src/hond/trigger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 21:42:31.000000 hond-1.0.1/src/hond/trigger/.keep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:43:03.839361 hond-1.0.1/src/hond/watch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 21:42:31.000000 hond-1.0.1/src/hond/watch/.keep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:43:03.839361 hond-1.0.1/src/hond.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-04-15 21:43:03.000000 hond-1.0.1/src/hond.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-15 21:43:03.000000 hond-1.0.1/src/hond.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 21:43:03.000000 hond-1.0.1/src/hond.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 21:43:03.000000 hond-1.0.1/src/hond.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-15 21:43:03.000000 hond-1.0.1/src/hond.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-15 21:43:03.000000 hond-1.0.1/src/hond.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:43:03.839361 hond-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-15 21:42:31.000000 hond-1.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 21:43:03.839361 hond-1.0.1/tests/datastore/
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-15 21:42:31.000000 hond-1.0.1/tests/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-15 21:42:31.000000 hond-1.0.1/tests/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-15 21:42:31.000000 hond-1.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:53:19.039316 hond-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-16 02:52:52.000000 hond-1.0.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:53:19.039316 hond-1.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-16 02:52:52.000000 hond-1.0.2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 02:52:52.000000 hond-1.0.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:53:19.039316 hond-1.0.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-16 02:52:52.000000 hond-1.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-16 02:52:52.000000 hond-1.0.2/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:53:19.039316 hond-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-16 02:52:52.000000 hond-1.0.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-16 02:52:52.000000 hond-1.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-16 02:52:52.000000 hond-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-16 02:52:52.000000 hond-1.0.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-16 02:52:52.000000 hond-1.0.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-04-16 02:52:52.000000 hond-1.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-16 02:52:52.000000 hond-1.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 02:52:52.000000 hond-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-16 02:52:52.000000 hond-1.0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-16 02:53:19.039316 hond-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-16 02:52:52.000000 hond-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:53:19.039316 hond-1.0.2/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-16 02:52:52.000000 hond-1.0.2/cache/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:53:19.039316 hond-1.0.2/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-04-16 02:52:52.000000 hond-1.0.2/chart/idog.drawio
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:53:19.039316 hond-1.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-16 02:52:52.000000 hond-1.0.2/examples/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-16 02:52:52.000000 hond-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-16 02:52:52.000000 hond-1.0.2/renovate.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-16 02:53:19.043316 hond-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-16 02:52:52.000000 hond-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:53:19.035316 hond-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:53:19.039316 hond-1.0.2/src/hond/
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-16 02:52:52.000000 hond-1.0.2/src/hond/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:53:19.039316 hond-1.0.2/src/hond/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 02:52:52.000000 hond-1.0.2/src/hond/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12528 2023-04-16 02:52:52.000000 hond-1.0.2/src/hond/driver/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-16 02:52:52.000000 hond-1.0.2/src/hond/hond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-16 02:52:52.000000 hond-1.0.2/src/hond/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-16 02:52:52.000000 hond-1.0.2/src/hond/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-16 02:52:52.000000 hond-1.0.2/src/hond/trigger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:53:19.039316 hond-1.0.2/src/hond.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-16 02:53:19.000000 hond-1.0.2/src/hond.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-04-16 02:53:19.000000 hond-1.0.2/src/hond.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 02:53:19.000000 hond-1.0.2/src/hond.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 02:53:18.000000 hond-1.0.2/src/hond.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-16 02:53:19.000000 hond-1.0.2/src/hond.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-16 02:53:19.000000 hond-1.0.2/src/hond.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:53:19.039316 hond-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 02:52:52.000000 hond-1.0.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:53:19.039316 hond-1.0.2/tests/datastore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 02:52:52.000000 hond-1.0.2/tests/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-16 02:52:52.000000 hond-1.0.2/tests/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-16 02:52:52.000000 hond-1.0.2/tox.ini
```

### Comparing `hond-1.0.1/.coveragerc` & `hond-1.0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `hond-1.0.1/.github/workflows/release.yml` & `hond-1.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `hond-1.0.1/.gitignore` & `hond-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hond-1.0.1/CODE_OF_CONDUCT.md` & `hond-1.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hond-1.0.1/CONTRIBUTING.rst` & `hond-1.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hond-1.0.1/LICENSE.txt` & `hond-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hond-1.0.1/Makefile` & `hond-1.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `hond-1.0.1/chart/idog.drawio` & `hond-1.0.2/chart/idog.drawio`

 * *Files identical despite different names*

### Comparing `hond-1.0.1/examples/basic.py` & `hond-1.0.2/examples/basic.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.1/setup.py` & `hond-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.1/src/hond/__init__.py` & `hond-1.0.2/src/hond/__init__.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.1/src/hond/collect/__init__.py` & `hond-1.0.2/src/hond/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.1/src/hond/collect/application.py` & `hond-1.0.2/tests/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,13 +15,7 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-
-
-class Application:
-    """Collect Application Metrics"""
-
-    pass
```

### Comparing `hond-1.0.1/src/hond/collect/certificate.py` & `hond-1.0.2/tests/datastore/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,13 +15,7 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-
-
-class Certificate:
-    """Collect Certificate Metrics"""
-
-    pass
```

### Comparing `hond-1.0.1/src/hond/logger.py` & `hond-1.0.2/src/hond/logger.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.1/src/hond/metric.py` & `hond-1.0.2/src/hond/metric.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.1/src/hond/store/__init__.py` & `hond-1.0.2/src/hond/hond.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,7 +15,23 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+
+from hond.logger import Logger
+
+
+class Hond:
+    """Hond Class"""
+
+    def __init__(self, driver):
+        self.logger = Logger().get_logger(__name__)
+        self.driver = driver
+
+    def insert(metric):
+        return self.driver.insert(metric)
+
+    def evaluate(trigger):
+        return self.driver.evaluate(trigger)
```

### Comparing `hond-1.0.1/src/hond/store/elasticsearch.py` & `hond-1.0.2/src/hond/driver/elasticsearch.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,119 +15,75 @@
 import time
 
 from hond.logger import Logger
 from elasticsearch import Elasticsearch
 
 
 class ElasticSearch:
-    """ElasticSearch Class
-
-    Attributes:
-        logger: An instance of Logger class
-        client: An instance of elasticsearch client
+    """
+    ElasticSearch Driver Class
     """
 
-    def __init__(self, connection):
+    def __init__(self, connection, index_name):
         """Inits elasticsearch"""
         self.logger = Logger().get_logger(__name__)
         self.client = Elasticsearch(connection)
-        self.before_hook = None
-        self.after_hook = None
+        self.index_name = index_name
 
     def get_client(self):
         """
         Get elasticsearch client
 
         Returns:
             a dict of client info
         """
         return self.client.info()
 
-    def add_before_hook(self, callback):
-        """Add before hook
-
-        Args:
-            callback: the before callback function
-        """
-        self.before_hook = callback
-
-    def add_after_hook(self, callback):
-        """Add after hook
-
-        Args:
-            callback: the after callback function
+    def migrate(self, shards=1, replicas=1):
         """
-        self.after_hook = callback
-
-    def migrate(self, index_name, shards=1, replicas=1):
-        """Create metric index
-
-        Args:
-            index_name: the elasticsearch index
-            shards: the number of shards
-            replicas: the number of replicas
+        Create metric index
         """
         doc = {
             "settings": {"number_of_shards": shards, "number_of_replicas": replicas},
             "mappings": {
                 "properties": {
                     "id": {"type": "text"},
                     "name": {"type": "text"},
                     "value": {"type": "float"},
                     "timestamp": {"type": "long"},
                     "meta": {"type": "object"},
                 }
             },
         }
 
-        response = self.client.index(index=index_name, document=doc)
+        response = self.client.index(index=self.index_name, document=doc)
 
         return response
 
-    def insert(self, metric, index_name):
-        """Insert metrics into elastic search
-
-        Args:
-            index_name: the elasticsearch index
-            metric: the metric data to insert
+    def insert(self, metric):
+        """
+        Insert metrics into elastic search
         """
-        self.logger.debug("Trigger before hook for metric: {}", str(metric))
-
-        if self.before_hook is not None:
-            self.before_hook(metric)
-
         doc = {
             "id": metric.id,
             "name": metric.name,
             "value": metric.value,
             "timestamp": metric.timestamp,
             "meta": metric.meta,
         }
 
         self.logger.debug("Insert metric into elasticsearch: {}", str(metric))
 
-        response = self.client.index(index=index_name, document=doc)
-
-        self.logger.debug("Trigger after hook for metric: {}", str(metric))
-
-        if self.after_hook is not None:
-            self.after_hook(metric)
+        response = self.client.index(index=self.index_name, document=doc)
 
         return response
 
-    def is_absent(self, index_name, metric_name, for_in_sec=60):
-        """Check if the metric is absent for x seconds
-
-        Args:
-            index_name: The elasticsearch index
-            metric_name: The metric name
-            for_in_sec: The time interval in seconds
-
-        Returns:
-            Whether the condition is true or false
+    def is_absent(self, metric_name, for_in_sec=60):
+        """
+        Check if the metric is absent for x seconds
         """
         query = {
             "query": {
                 "bool": {
                     "must": [
                         {"match_phrase": {"name": {"query": metric_name}}},
                         {
@@ -136,32 +92,24 @@
                             }
                         },
                     ]
                 }
             }
         }
 
-        response = self.client.search(index=index_name, body=query)
+        response = self.search(query)
 
         return (
             response["hits"]["total"]["value"] == 0
             and len(response["hits"]["hits"]) == 0
         )
 
-    def equal(self, index_name, metric_name, benchmark, for_in_sec=60):
-        """Check if the metric is equal to the benchmark for x seconds
-
-        Args:
-            index_name: The elasticsearch index
-            metric_name: The metric name
-            benchmark: The benchmark value
-            for_in_sec: The time interval in seconds
-
-        Returns:
-            Whether the condition is true or false
+    def equal(self, metric_name, benchmark, for_in_sec=60):
+        """
+        Check if the metric is equal to the benchmark for x seconds
         """
         query1 = {
             "query": {
                 "bool": {
                     "must": [
                         {"match_phrase": {"name": {"query": metric_name}}},
                         {
@@ -170,15 +118,15 @@
                             }
                         },
                     ]
                 }
             }
         }
 
-        response1 = self.client.search(index=index_name, body=query1)
+        response1 = self.search(query1)
 
         # If no hits have been found
         if response1["hits"]["total"]["value"] == 0:
             return False
 
         query2 = {
             "query": {
@@ -192,31 +140,23 @@
                             }
                         },
                     ]
                 }
             }
         }
 
-        response2 = self.client.search(index=index_name, body=query2)
+        response2 = self.search(query2)
 
         return (
             response1["hits"]["total"]["value"] == response2["hits"]["total"]["value"]
         )
 
-    def above(self, index_name, metric_name, benchmark, for_in_sec=60):
-        """Check if the metric is above the benchmark for x seconds
-
-        Args:
-            index_name: The elasticsearch index
-            metric_name: The metric name
-            benchmark: The benchmark value
-            for_in_sec: The time interval in seconds
-
-        Returns:
-            Whether the condition is true or false
+    def above(self, metric_name, benchmark, for_in_sec=60):
+        """
+        Check if the metric is above the benchmark for x seconds
         """
         query1 = {
             "query": {
                 "bool": {
                     "must": [
                         {"match_phrase": {"name": {"query": metric_name}}},
                         {
@@ -225,15 +165,15 @@
                             }
                         },
                     ]
                 }
             }
         }
 
-        response1 = self.client.search(index=index_name, body=query1)
+        response1 = self.search(query1)
 
         # If no hits have been found
         if response1["hits"]["total"]["value"] == 0:
             return False
 
         query2 = {
             "query": {
@@ -247,31 +187,70 @@
                             }
                         },
                     ]
                 }
             }
         }
 
-        response2 = self.client.search(index=index_name, body=query2)
+        response2 = self.search(query2)
 
         return (
             response1["hits"]["total"]["value"] == response2["hits"]["total"]["value"]
         )
 
-    def below(self, index_name, metric_name, benchmark, for_in_sec=60):
-        """Check if the metric is below the benchmark for x seconds
+    def below(self, metric_name, benchmark, for_in_sec=60):
+        """
+        Check if the metric is below the benchmark for x seconds
+        """
+        query1 = {
+            "query": {
+                "bool": {
+                    "must": [
+                        {"match_phrase": {"name": {"query": metric_name}}},
+                        {
+                            "range": {
+                                "timestamp": {"gte": int(time.time()) - for_in_sec}
+                            }
+                        },
+                    ]
+                }
+            }
+        }
 
-        Args:
-            index_name: The elasticsearch index
-            metric_name: The metric name
-            benchmark: The benchmark value
-            for_in_sec: The time interval in seconds
+        response1 = self.search(query1)
 
-        Returns:
-            Whether the condition is true or false
+        # If no hits have been found
+        if response1["hits"]["total"]["value"] == 0:
+            return False
+
+        query2 = {
+            "query": {
+                "bool": {
+                    "must": [
+                        {"match_phrase": {"name": {"query": metric_name}}},
+                        {"range": {"value": {"lt": benchmark}}},
+                        {
+                            "range": {
+                                "timestamp": {"gte": int(time.time()) - for_in_sec}
+                            }
+                        },
+                    ]
+                }
+            }
+        }
+
+        response2 = self.search(query2)
+
+        return (
+            response1["hits"]["total"]["value"] == response2["hits"]["total"]["value"]
+        )
+
+    def above_equal(self, metric_name, benchmark, for_in_sec=60):
+        """
+        Check if the metric is above or equal the benchmark for x seconds
         """
         query1 = {
             "query": {
                 "bool": {
                     "must": [
                         {"match_phrase": {"name": {"query": metric_name}}},
                         {
@@ -280,45 +259,147 @@
                             }
                         },
                     ]
                 }
             }
         }
 
-        response1 = self.client.search(index=index_name, body=query1)
+        response1 = self.search(query1)
 
         # If no hits have been found
         if response1["hits"]["total"]["value"] == 0:
             return False
 
         query2 = {
             "query": {
                 "bool": {
                     "must": [
                         {"match_phrase": {"name": {"query": metric_name}}},
-                        {"range": {"value": {"lt": benchmark}}},
+                        {"range": {"value": {"gte": benchmark}}},
                         {
                             "range": {
                                 "timestamp": {"gte": int(time.time()) - for_in_sec}
                             }
                         },
                     ]
                 }
             }
         }
 
-        response2 = self.client.search(index=index_name, body=query2)
+        response2 = self.search(query2)
 
         return (
             response1["hits"]["total"]["value"] == response2["hits"]["total"]["value"]
         )
 
-    def search(self, index_name, query):
-        """Query elasticsearch index
+    def below_equal(self, metric_name, benchmark, for_in_sec=60):
+        """
+        Check if the metric is below or equal the benchmark for x seconds
+        """
+        query1 = {
+            "query": {
+                "bool": {
+                    "must": [
+                        {"match_phrase": {"name": {"query": metric_name}}},
+                        {
+                            "range": {
+                                "timestamp": {"gte": int(time.time()) - for_in_sec}
+                            }
+                        },
+                    ]
+                }
+            }
+        }
 
-        Args:
-            index_name: The elasticsearch index
+        response1 = self.search(query1)
 
-        Returns:
-            The result
+        # If no hits have been found
+        if response1["hits"]["total"]["value"] == 0:
+            return False
+
+        query2 = {
+            "query": {
+                "bool": {
+                    "must": [
+                        {"match_phrase": {"name": {"query": metric_name}}},
+                        {"range": {"value": {"lte": benchmark}}},
+                        {
+                            "range": {
+                                "timestamp": {"gte": int(time.time()) - for_in_sec}
+                            }
+                        },
+                    ]
+                }
+            }
+        }
+
+        response2 = self.search(query2)
+
+        return (
+            response1["hits"]["total"]["value"] == response2["hits"]["total"]["value"]
+        )
+
+    def search(self, query):
+        """
+        Query elasticsearch index
+        """
+        return self.client.search(index=self.index_name, body=query)
+
+    def evaluate(expression):
         """
-        return self.client.search(index=index_name, body=query)
+        Evaluate a trigger value
+
+        Examples:
+            m{customers.123.456.789.cpu>=20}[30s]
+            m{customers.123.456.789.cpu<20}[30s]
+            m{customers.123.456.789.cpu==nul}[30s]
+            m{customers.123.456.789.cpu==nul}[30s] and m{customers.123.456.789.mem==nul}[30s]
+
+        TODO: switch to safer way other than eval but right now triggers is not a user input
+        """
+        result = []
+        expressions = re.split(" and | or ", expression)
+
+        for exp in expressions:
+            pattern = r"^(m)\{(.*)\}(\[(.*)\])?$"
+            match = re.match(pattern, exp)
+            if match:
+                items = re.split(">=|<=|==|>|<", match.group(2))
+
+                if items[1] == "nul":
+                    metric_name = items[0]
+                    for_in_sec = int(match.group(4))
+
+                    value = self.is_absent(metric_name, for_in_sec)
+                else:
+                    metric_name = items[0]
+                    benchmark = float(items[1])
+                    for_in_sec = int(match.group(4))
+
+                    if "==" in match.group(2):
+                        value = self.equal(self, metric_name, benchmark, for_in_sec)
+                    elif ">=" in match.group(2):
+                        value = self.above_equal(
+                            self, metric_name, benchmark, for_in_sec
+                        )
+                    elif "<=" in match.group(2):
+                        value = self.below_equal(
+                            self, metric_name, benchmark, for_in_sec
+                        )
+                    elif ">" in match.group(2):
+                        value = self.above(self, metric_name, benchmark, for_in_sec)
+                    elif "<" in match.group(2):
+                        value = self.below(self, metric_name, benchmark, for_in_sec)
+
+                if value:
+                    result.append("True")
+                else:
+                    result.append("False")
+            else:
+                raise Exception("Invalid expression: {}".format(exp))
+
+        out = expression
+
+        for i in range(len(expressions)):
+            out = out.replace(expressions[i], result[i])
+
+        return eval(out)
```

### Comparing `hond-1.0.1/tests/test_metric.py` & `hond-1.0.2/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `hond-1.0.1/tox.ini` & `hond-1.0.2/tox.ini`

 * *Files identical despite different names*

