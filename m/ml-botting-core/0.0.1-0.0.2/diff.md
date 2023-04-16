# Comparing `tmp/ml-botting-core-0.0.1.tar.gz` & `tmp/ml-botting-core-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-botting-core-0.0.1.tar", last modified: Sun Apr 16 15:56:31 2023, max compression
+gzip compressed data, was "ml-botting-core-0.0.2.tar", last modified: Sun Apr 16 16:28:22 2023, max compression
```

## Comparing `ml-botting-core-0.0.1.tar` & `ml-botting-core-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 15:56:31.019355 ml-botting-core-0.0.1/
--rw-rw-rw-   0        0        0     1092 2023-04-16 15:23:47.000000 ml-botting-core-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      592 2023-04-16 15:56:31.020355 ml-botting-core-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       36 2023-04-16 15:23:47.000000 ml-botting-core-0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2023-04-16 15:28:39.000000 ml-botting-core-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      695 2023-04-16 15:56:31.020355 ml-botting-core-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-16 15:56:31.011355 ml-botting-core-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 15:56:31.016355 ml-botting-core-0.0.1/src/ml-botting-core/
--rw-rw-rw-   0        0        0        0 2023-04-16 15:26:05.000000 ml-botting-core-0.0.1/src/ml-botting-core/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-16 15:26:18.000000 ml-botting-core-0.0.1/src/ml-botting-core/temp.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:56:31.019355 ml-botting-core-0.0.1/src/ml_botting_core.egg-info/
--rw-rw-rw-   0        0        0      592 2023-04-16 15:56:30.000000 ml-botting-core-0.0.1/src/ml_botting_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-04-16 15:56:31.000000 ml-botting-core-0.0.1/src/ml_botting_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 15:56:31.000000 ml-botting-core-0.0.1/src/ml_botting_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-16 15:56:31.000000 ml-botting-core-0.0.1/src/ml_botting_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:28:22.657678 ml-botting-core-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-16 16:28:11.000000 ml-botting-core-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-16 16:28:22.657678 ml-botting-core-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-16 16:28:11.000000 ml-botting-core-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-16 16:28:11.000000 ml-botting-core-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-16 16:28:22.657678 ml-botting-core-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:28:22.657678 ml-botting-core-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:28:22.657678 ml-botting-core-0.0.2/src/ml-botting-core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:28:11.000000 ml-botting-core-0.0.2/src/ml-botting-core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 16:28:11.000000 ml-botting-core-0.0.2/src/ml-botting-core/temp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:28:22.657678 ml-botting-core-0.0.2/src/ml_botting_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-16 16:28:22.000000 ml-botting-core-0.0.2/src/ml_botting_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-16 16:28:22.000000 ml-botting-core-0.0.2/src/ml_botting_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:28:22.000000 ml-botting-core-0.0.2/src/ml_botting_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-16 16:28:22.000000 ml-botting-core-0.0.2/src/ml_botting_core.egg-info/top_level.txt
```

### Comparing `ml-botting-core-0.0.1/LICENSE` & `ml-botting-core-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Ryan V. Susman
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Ryan V. Susman
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `ml-botting-core-0.0.1/PKG-INFO` & `ml-botting-core-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1
-Name: ml-botting-core
-Version: 0.0.1
-Summary: Making ML more accessible to botting apps
-Home-page: https://github.com/darkmatter2222/ml-botting-core
-Author: Ryan Susman
-Author-email: ryansusman@gmail.com
-Project-URL: Bug Tracker, https://github.com/darkmatter2222/ml-botting-core/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ml-botting-core
-ml-botting-core
+Metadata-Version: 2.1
+Name: ml-botting-core
+Version: 0.0.2
+Summary: Making ML more accessible to botting apps
+Home-page: https://github.com/darkmatter2222/ml-botting-core
+Author: Ryan Susman
+Author-email: ryansusman@gmail.com
+Project-URL: Bug Tracker, https://github.com/darkmatter2222/ml-botting-core/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ml-botting-core
+ml-botting-core
```

### Comparing `ml-botting-core-0.0.1/src/ml_botting_core.egg-info/PKG-INFO` & `ml-botting-core-0.0.2/src/ml_botting_core.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1
-Name: ml-botting-core
-Version: 0.0.1
-Summary: Making ML more accessible to botting apps
-Home-page: https://github.com/darkmatter2222/ml-botting-core
-Author: Ryan Susman
-Author-email: ryansusman@gmail.com
-Project-URL: Bug Tracker, https://github.com/darkmatter2222/ml-botting-core/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ml-botting-core
-ml-botting-core
+Metadata-Version: 2.1
+Name: ml-botting-core
+Version: 0.0.2
+Summary: Making ML more accessible to botting apps
+Home-page: https://github.com/darkmatter2222/ml-botting-core
+Author: Ryan Susman
+Author-email: ryansusman@gmail.com
+Project-URL: Bug Tracker, https://github.com/darkmatter2222/ml-botting-core/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ml-botting-core
+ml-botting-core
```

