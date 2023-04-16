# Comparing `tmp/sabledocs-0.1.80.tar.gz` & `tmp/sabledocs-0.1.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabledocs-0.1.80.tar", last modified: Sat Apr 15 21:24:56 2023, max compression
+gzip compressed data, was "sabledocs-0.1.84.tar", last modified: Sun Apr 16 21:31:22 2023, max compression
```

## Comparing `sabledocs-0.1.80.tar` & `sabledocs-0.1.84.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-15 21:24:56.321535 sabledocs-0.1.80/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-04-15 21:24:43.000000 sabledocs-0.1.80/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-04-15 21:24:43.000000 sabledocs-0.1.80/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3722 2023-04-15 21:24:56.321535 sabledocs-0.1.80/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3186 2023-04-15 21:24:43.000000 sabledocs-0.1.80/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      776 2023-04-15 21:24:43.000000 sabledocs-0.1.80/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       73 2023-04-15 21:24:56.321535 sabledocs-0.1.80/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-15 21:24:56.317535 sabledocs-0.1.80/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-15 21:24:56.317535 sabledocs-0.1.80/src/sabledocs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-15 21:24:43.000000 sabledocs-0.1.80/src/sabledocs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2227 2023-04-15 21:24:43.000000 sabledocs-0.1.80/src/sabledocs/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13639 2023-04-15 21:24:43.000000 sabledocs-0.1.80/src/sabledocs/proto_descriptor_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2719 2023-04-15 21:24:43.000000 sabledocs-0.1.80/src/sabledocs/proto_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2269 2023-04-15 21:24:43.000000 sabledocs-0.1.80/src/sabledocs/sable_config.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-15 21:24:56.317535 sabledocs-0.1.80/src/sabledocs/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-15 21:24:56.321535 sabledocs-0.1.80/src/sabledocs/templates/_default/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1850 2023-04-15 21:24:43.000000 sabledocs-0.1.80/src/sabledocs/templates/_default/base.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-04-15 21:24:43.000000 sabledocs-0.1.80/src/sabledocs/templates/_default/enum.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      528 2023-04-15 21:24:43.000000 sabledocs-0.1.80/src/sabledocs/templates/_default/index.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-04-15 21:24:43.000000 sabledocs-0.1.80/src/sabledocs/templates/_default/message.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1889 2023-04-15 21:24:43.000000 sabledocs-0.1.80/src/sabledocs/templates/_default/package.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2023-04-15 21:24:43.000000 sabledocs-0.1.80/src/sabledocs/templates/_default/service.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-15 21:24:56.321535 sabledocs-0.1.80/src/sabledocs/templates/_default/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   257737 2023-04-15 21:24:43.000000 sabledocs-0.1.80/src/sabledocs/templates/_default/static/mystyles.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-04-15 21:24:43.000000 sabledocs-0.1.80/src/sabledocs/templates/_default/type_name.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-15 21:24:56.321535 sabledocs-0.1.80/src/sabledocs.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3722 2023-04-15 21:24:56.000000 sabledocs-0.1.80/src/sabledocs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      763 2023-04-15 21:24:56.000000 sabledocs-0.1.80/src/sabledocs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-15 21:24:56.000000 sabledocs-0.1.80/src/sabledocs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-04-15 21:24:56.000000 sabledocs-0.1.80/src/sabledocs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-04-15 21:24:56.000000 sabledocs-0.1.80/src/sabledocs.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 21:31:22.054477 sabledocs-0.1.84/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-04-16 21:31:06.000000 sabledocs-0.1.84/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-04-16 21:31:06.000000 sabledocs-0.1.84/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3817 2023-04-16 21:31:22.054477 sabledocs-0.1.84/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3281 2023-04-16 21:31:06.000000 sabledocs-0.1.84/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      776 2023-04-16 21:31:06.000000 sabledocs-0.1.84/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       73 2023-04-16 21:31:22.058477 sabledocs-0.1.84/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 21:31:22.050477 sabledocs-0.1.84/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 21:31:22.054477 sabledocs-0.1.84/src/sabledocs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-16 21:31:06.000000 sabledocs-0.1.84/src/sabledocs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2227 2023-04-16 21:31:06.000000 sabledocs-0.1.84/src/sabledocs/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13639 2023-04-16 21:31:06.000000 sabledocs-0.1.84/src/sabledocs/proto_descriptor_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2719 2023-04-16 21:31:06.000000 sabledocs-0.1.84/src/sabledocs/proto_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2269 2023-04-16 21:31:06.000000 sabledocs-0.1.84/src/sabledocs/sable_config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 21:31:22.050477 sabledocs-0.1.84/src/sabledocs/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 21:31:22.054477 sabledocs-0.1.84/src/sabledocs/templates/_default/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1850 2023-04-16 21:31:06.000000 sabledocs-0.1.84/src/sabledocs/templates/_default/base.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-04-16 21:31:06.000000 sabledocs-0.1.84/src/sabledocs/templates/_default/enum.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      528 2023-04-16 21:31:06.000000 sabledocs-0.1.84/src/sabledocs/templates/_default/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-04-16 21:31:06.000000 sabledocs-0.1.84/src/sabledocs/templates/_default/message.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1889 2023-04-16 21:31:06.000000 sabledocs-0.1.84/src/sabledocs/templates/_default/package.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2023-04-16 21:31:06.000000 sabledocs-0.1.84/src/sabledocs/templates/_default/service.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 21:31:22.054477 sabledocs-0.1.84/src/sabledocs/templates/_default/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   257737 2023-04-16 21:31:06.000000 sabledocs-0.1.84/src/sabledocs/templates/_default/static/mystyles.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-04-16 21:31:06.000000 sabledocs-0.1.84/src/sabledocs/templates/_default/type_name.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 21:31:22.054477 sabledocs-0.1.84/src/sabledocs.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3817 2023-04-16 21:31:22.000000 sabledocs-0.1.84/src/sabledocs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      763 2023-04-16 21:31:22.000000 sabledocs-0.1.84/src/sabledocs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-16 21:31:22.000000 sabledocs-0.1.84/src/sabledocs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-04-16 21:31:22.000000 sabledocs-0.1.84/src/sabledocs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-04-16 21:31:22.000000 sabledocs-0.1.84/src/sabledocs.egg-info/top_level.txt
```

### Comparing `sabledocs-0.1.80/LICENSE` & `sabledocs-0.1.84/LICENSE`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.80/PKG-INFO` & `sabledocs-0.1.84/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.1.80
+Version: 0.1.84
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sabledocs
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/markvincze/sabledocs/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/markvincze/sabledocs/tree/main)
+[![Latest Version][mdversion-button]][md-pypi]
+
+[md-pypi]: https://pypi.org/project/sabledocs/
 
 A simple static documentation generator for Protobuf and gRPC contracts.
 
 **Demo**: You can check out this [demo](https://markvincze.github.io/sabledocs/demo/) showing the generated documentation for the [Google Cloud Pub/Sub contracts](https://github.com/googleapis/googleapis/tree/master/google/pubsub/v1).
 
 ## How to use
```

### Comparing `sabledocs-0.1.80/README.md` & `sabledocs-0.1.84/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # sabledocs
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/markvincze/sabledocs/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/markvincze/sabledocs/tree/main)
+[![Latest Version][mdversion-button]][md-pypi]
+
+[md-pypi]: https://pypi.org/project/sabledocs/
 
 A simple static documentation generator for Protobuf and gRPC contracts.
 
 **Demo**: You can check out this [demo](https://markvincze.github.io/sabledocs/demo/) showing the generated documentation for the [Google Cloud Pub/Sub contracts](https://github.com/googleapis/googleapis/tree/master/google/pubsub/v1).
 
 ## How to use
```

### Comparing `sabledocs-0.1.80/pyproject.toml` & `sabledocs-0.1.84/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.80/src/sabledocs/__main__.py` & `sabledocs-0.1.84/src/sabledocs/__main__.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.80/src/sabledocs/proto_descriptor_parser.py` & `sabledocs-0.1.84/src/sabledocs/proto_descriptor_parser.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.80/src/sabledocs/proto_model.py` & `sabledocs-0.1.84/src/sabledocs/proto_model.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.80/src/sabledocs/sable_config.py` & `sabledocs-0.1.84/src/sabledocs/sable_config.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.80/src/sabledocs/templates/_default/base.html` & `sabledocs-0.1.84/src/sabledocs/templates/_default/base.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.80/src/sabledocs/templates/_default/enum.html` & `sabledocs-0.1.84/src/sabledocs/templates/_default/enum.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.80/src/sabledocs/templates/_default/index.html` & `sabledocs-0.1.84/src/sabledocs/templates/_default/index.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.80/src/sabledocs/templates/_default/message.html` & `sabledocs-0.1.84/src/sabledocs/templates/_default/message.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.80/src/sabledocs/templates/_default/package.html` & `sabledocs-0.1.84/src/sabledocs/templates/_default/package.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.80/src/sabledocs/templates/_default/service.html` & `sabledocs-0.1.84/src/sabledocs/templates/_default/service.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.80/src/sabledocs/templates/_default/static/mystyles.css` & `sabledocs-0.1.84/src/sabledocs/templates/_default/static/mystyles.css`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.80/src/sabledocs/templates/_default/type_name.html` & `sabledocs-0.1.84/src/sabledocs/templates/_default/type_name.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.1.80/src/sabledocs.egg-info/PKG-INFO` & `sabledocs-0.1.84/src/sabledocs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.1.80
+Version: 0.1.84
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sabledocs
 
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/markvincze/sabledocs/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/markvincze/sabledocs/tree/main)
+[![Latest Version][mdversion-button]][md-pypi]
+
+[md-pypi]: https://pypi.org/project/sabledocs/
 
 A simple static documentation generator for Protobuf and gRPC contracts.
 
 **Demo**: You can check out this [demo](https://markvincze.github.io/sabledocs/demo/) showing the generated documentation for the [Google Cloud Pub/Sub contracts](https://github.com/googleapis/googleapis/tree/master/google/pubsub/v1).
 
 ## How to use
```

### Comparing `sabledocs-0.1.80/src/sabledocs.egg-info/SOURCES.txt` & `sabledocs-0.1.84/src/sabledocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

