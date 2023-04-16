# Comparing `tmp/paper-streamfield-0.3.0.tar.gz` & `tmp/paper-streamfield-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-streamfield-0.3.0.tar", last modified: Thu Dec  1 09:29:00 2022, max compression
+gzip compressed data, was "paper-streamfield-0.4.0.tar", last modified: Sun Apr 16 17:54:41 2023, max compression
```

## Comparing `paper-streamfield-0.3.0.tar` & `paper-streamfield-0.4.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 09:29:00.562246 paper-streamfield-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      182 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2022-12-01 09:29:00.562246 paper-streamfield-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 09:29:00.546245 paper-streamfield-0.3.0/paper_streamfield.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2022-12-01 09:28:59.000000 paper-streamfield-0.3.0/paper_streamfield.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2022-12-01 09:28:59.000000 paper-streamfield-0.3.0/paper_streamfield.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-01 09:28:59.000000 paper-streamfield-0.3.0/paper_streamfield.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-01 09:28:59.000000 paper-streamfield-0.3.0/paper_streamfield.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       43 2022-12-01 09:28:59.000000 paper-streamfield-0.3.0/paper_streamfield.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2022-12-01 09:28:59.000000 paper-streamfield-0.3.0/paper_streamfield.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2022-12-01 09:29:00.562246 paper-streamfield-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 09:29:00.554246 paper-streamfield-0.3.0/streamfield/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 09:29:00.554246 paper-streamfield-0.3.0/streamfield/admin/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/admin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/admin/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 09:29:00.558246 paper-streamfield-0.3.0/streamfield/field/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/field/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/field/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/field/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 09:29:00.538245 paper-streamfield-0.3.0/streamfield/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 09:29:00.538245 paper-streamfield-0.3.0/streamfield/static/streamfield/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 09:29:00.558246 paper-streamfield-0.3.0/streamfield/static/streamfield/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 09:29:00.558246 paper-streamfield-0.3.0/streamfield/static/streamfield/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2022-12-01 09:28:59.000000 paper-streamfield-0.3.0/streamfield/static/streamfield/dist/assets/sortable.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2022-12-01 09:28:59.000000 paper-streamfield-0.3.0/streamfield/static/streamfield/dist/assets/spinner.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2022-12-01 09:28:59.000000 paper-streamfield-0.3.0/streamfield/static/streamfield/dist/widget.css
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2022-12-01 09:28:59.000000 paper-streamfield-0.3.0/streamfield/static/streamfield/dist/widget.js
--rw-r--r--   0 runner    (1001) docker     (123)    27174 2022-12-01 09:28:59.000000 paper-streamfield-0.3.0/streamfield/static/streamfield/dist/widget.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 09:29:00.538245 paper-streamfield-0.3.0/streamfield/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 09:29:00.562246 paper-streamfield-0.3.0/streamfield/templates/streamfield/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 09:29:00.562246 paper-streamfield-0.3.0/streamfield/templates/streamfield/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/templates/streamfield/admin/block.html
--rw-r--r--   0 runner    (1001) docker     (123)      733 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/templates/streamfield/admin/invalid_block.html
--rw-r--r--   0 runner    (1001) docker     (123)      534 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/templates/streamfield/admin/popup_response.html
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/templates/streamfield/admin/toolbar.html
--rw-r--r--   0 runner    (1001) docker     (123)      440 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/templates/streamfield/widget.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 09:29:00.562246 paper-streamfield-0.3.0/streamfield/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/templatetags/streamfield.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2022-12-01 09:28:36.000000 paper-streamfield-0.3.0/streamfield/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.487895 paper-streamfield-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-16 17:54:41.487895 paper-streamfield-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.479895 paper-streamfield-0.4.0/paper_streamfield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-04-16 17:54:41.000000 paper-streamfield-0.4.0/paper_streamfield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-16 17:54:41.000000 paper-streamfield-0.4.0/paper_streamfield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 17:54:41.000000 paper-streamfield-0.4.0/paper_streamfield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 17:54:41.000000 paper-streamfield-0.4.0/paper_streamfield.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-16 17:54:41.000000 paper-streamfield-0.4.0/paper_streamfield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-16 17:54:41.000000 paper-streamfield-0.4.0/paper_streamfield.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-16 17:54:41.487895 paper-streamfield-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.483895 paper-streamfield-0.4.0/streamfield/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.483895 paper-streamfield-0.4.0/streamfield/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/admin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/admin/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.483895 paper-streamfield-0.4.0/streamfield/field/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/field/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/field/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/field/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.479895 paper-streamfield-0.4.0/streamfield/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.479895 paper-streamfield-0.4.0/streamfield/static/streamfield/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.483895 paper-streamfield-0.4.0/streamfield/static/streamfield/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.483895 paper-streamfield-0.4.0/streamfield/static/streamfield/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-16 17:54:40.000000 paper-streamfield-0.4.0/streamfield/static/streamfield/dist/assets/sortable.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-16 17:54:40.000000 paper-streamfield-0.4.0/streamfield/static/streamfield/dist/assets/spinner.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-16 17:54:40.000000 paper-streamfield-0.4.0/streamfield/static/streamfield/dist/widget.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-04-16 17:54:40.000000 paper-streamfield-0.4.0/streamfield/static/streamfield/dist/widget.js
+-rw-r--r--   0 runner    (1001) docker     (123)    26424 2023-04-16 17:54:40.000000 paper-streamfield-0.4.0/streamfield/static/streamfield/dist/widget.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.479895 paper-streamfield-0.4.0/streamfield/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.483895 paper-streamfield-0.4.0/streamfield/templates/streamfield/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.487895 paper-streamfield-0.4.0/streamfield/templates/streamfield/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/templates/streamfield/admin/block.html
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/templates/streamfield/admin/invalid_block.html
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/templates/streamfield/admin/popup_response.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/templates/streamfield/admin/toolbar.html
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/templates/streamfield/widget.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:41.487895 paper-streamfield-0.4.0/streamfield/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/templatetags/streamfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-16 17:54:11.000000 paper-streamfield-0.4.0/streamfield/utils.py
```

### Comparing `paper-streamfield-0.3.0/CHANGELOG.md` & `paper-streamfield-0.4.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Change Log
 
+## [0.4.0](https://github.com/dldevinc/paper-streamfield/tree/v0.4.0) - 2023-04-16
+
+### ⚠ BREAKING CHANGES
+
+-   Minimum required `paper-admin` version is now `6.0.0`.
+
 ## [0.3.0](https://github.com/dldevinc/paper-streamfield/tree/v0.3.0) - 2022-11-30
 
 -   Support for `paper-admin` >= 5.0.
 -   Add Python 3.11 support (no code changes were needed, but now we test this release).
 
 ## [0.2.1](https://github.com/dldevinc/paper-streamfield/tree/v0.2.1) - 2022-10-05
```

### Comparing `paper-streamfield-0.3.0/CONTRIBUTING.md` & `paper-streamfield-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `paper-streamfield-0.3.0/LICENSE` & `paper-streamfield-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-streamfield-0.3.0/PKG-INFO` & `paper-streamfield-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-streamfield
-Version: 0.3.0
+Version: 0.4.0
 Summary: Implementation of the Wagtail's StreamField block picker for paper-admin.
 Home-page: https://github.com/dldevinc/paper-streamfield
 Author: Mihail Mishakin
 Author-email: x896321475@gmail.com
 Maintainer: Mihail Mishakin
 Maintainer-email: x896321475@gmail.com
 License: BSD license
@@ -13,14 +13,15 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -37,15 +38,15 @@
 [![Build Status](https://github.com/dldevinc/paper-streamfield/actions/workflows/tests.yml/badge.svg)](https://github.com/dldevinc/paper-streamfield)
 [![Software license](https://img.shields.io/pypi/l/paper-streamfield.svg)](https://pypi.org/project/paper-streamfield/)
 
 ## Compatibility
 
 -   `python` >= 3.8
 -   `django` >= 3.1
--   `paper-admin` >= 4.3
+-   `paper-admin` >= 6.0
 
 ## Installation
 
 Install the latest release with pip:
 
 ```shell
 pip install paper-streamfield
```

### Comparing `paper-streamfield-0.3.0/README.md` & `paper-streamfield-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![Build Status](https://github.com/dldevinc/paper-streamfield/actions/workflows/tests.yml/badge.svg)](https://github.com/dldevinc/paper-streamfield)
 [![Software license](https://img.shields.io/pypi/l/paper-streamfield.svg)](https://pypi.org/project/paper-streamfield/)
 
 ## Compatibility
 
 -   `python` >= 3.8
 -   `django` >= 3.1
--   `paper-admin` >= 4.3
+-   `paper-admin` >= 6.0
 
 ## Installation
 
 Install the latest release with pip:
 
 ```shell
 pip install paper-streamfield
```

### Comparing `paper-streamfield-0.3.0/package.json` & `paper-streamfield-0.4.0/package.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.857487922705314%*

 * *Differences: {"'devDependencies'": "{'@babel/core': '^7.21.4', '@babel/preset-env': '^7.21.4', 'babel-loader': "*

 * *                      "'^9.1.2', 'css-minimizer-webpack-plugin': '^5.0.0', "*

 * *                      "'mini-css-extract-plugin': '^2.7.5', 'postcss': '^8.4.22', "*

 * *                      "'postcss-loader': '^7.2.4', 'sass': '^1.62.0', 'sass-loader': '^13.2.2', "*

 * *                      "'terser-webpack-plugin': '^5.3.7', 'webpack': '^5.79.0', 'webpack-cli': "*

 * *                      "'^5.0.1', 'babel-plugin-transform […]*

```diff
@@ -1,34 +1,34 @@
 {
     "author": "Mihail Mishakin",
     "description": "Implementation of the Wagtail's StreamField block picker for paper-admin.",
     "devDependencies": {
-        "@babel/core": "^7.20.5",
+        "@babel/core": "^7.21.4",
         "@babel/plugin-syntax-dynamic-import": "^7.8.3",
-        "@babel/plugin-transform-runtime": "^7.19.6",
-        "@babel/preset-env": "^7.20.2",
-        "autoprefixer": "^10.4.13",
-        "babel-loader": "^9.1.0",
-        "css-minimizer-webpack-plugin": "^4.2.2",
-        "fast-async": "^6.3.8",
+        "@babel/preset-env": "^7.21.4",
+        "babel-loader": "^9.1.2",
+        "babel-plugin-transform-imports": "^2.0.0",
+        "css-minimizer-webpack-plugin": "^5.0.0",
         "fast-css-loader": "^1.0.2",
         "fibers": "^5.0.3",
-        "mini-css-extract-plugin": "^2.7.1",
-        "pixrem": "^5.0.0",
-        "postcss": "^8.4.19",
-        "postcss-loader": "^7.0.2",
-        "sass": "^1.56.1",
-        "sass-loader": "^13.2.0",
-        "terser-webpack-plugin": "^5.3.6",
+        "mini-css-extract-plugin": "^2.7.5",
+        "postcss": "^8.4.22",
+        "postcss-loader": "^7.2.4",
+        "postcss-preset-env": "^8.3.1",
+        "sass": "^1.62.0",
+        "sass-loader": "^13.2.2",
+        "terser-webpack-plugin": "^5.3.7",
         "uuid": "^9.0.0",
-        "webpack": "^5.75.0",
-        "webpack-cli": "^4.10.0"
+        "webpack": "^5.79.0",
+        "webpack-cli": "^5.0.1",
+        "webpack-merge": "^5.8.0"
     },
     "license": "BSD license",
     "main": "streamfield/static/streamfield/index.js",
     "name": "paper-streamfield",
     "scripts": {
         "build": "webpack --mode production",
         "build:dev": "webpack --mode development"
     },
+    "type": "module",
     "version": "0.1.0"
 }
```

### Comparing `paper-streamfield-0.3.0/paper_streamfield.egg-info/PKG-INFO` & `paper-streamfield-0.4.0/paper_streamfield.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-streamfield
-Version: 0.3.0
+Version: 0.4.0
 Summary: Implementation of the Wagtail's StreamField block picker for paper-admin.
 Home-page: https://github.com/dldevinc/paper-streamfield
 Author: Mihail Mishakin
 Author-email: x896321475@gmail.com
 Maintainer: Mihail Mishakin
 Maintainer-email: x896321475@gmail.com
 License: BSD license
@@ -13,14 +13,15 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -37,15 +38,15 @@
 [![Build Status](https://github.com/dldevinc/paper-streamfield/actions/workflows/tests.yml/badge.svg)](https://github.com/dldevinc/paper-streamfield)
 [![Software license](https://img.shields.io/pypi/l/paper-streamfield.svg)](https://pypi.org/project/paper-streamfield/)
 
 ## Compatibility
 
 -   `python` >= 3.8
 -   `django` >= 3.1
--   `paper-admin` >= 4.3
+-   `paper-admin` >= 6.0
 
 ## Installation
 
 Install the latest release with pip:
 
 ```shell
 pip install paper-streamfield
```

### Comparing `paper-streamfield-0.3.0/paper_streamfield.egg-info/SOURCES.txt` & `paper-streamfield-0.4.0/paper_streamfield.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paper-streamfield-0.3.0/setup.cfg` & `paper-streamfield-0.4.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 	Development Status :: 3 - Alpha
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Framework :: Django :: 3.1
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
@@ -34,15 +35,15 @@
 
 [options]
 zip_safe = false
 python_requires = >= 3.8
 include_package_data = true
 install_requires = 
 	Django
-	paper-admin>=4.3
+	paper-admin>=6.0rc
 	jinja2-simple-tags
 packages = find_namespace:
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
```

### Comparing `paper-streamfield-0.3.0/streamfield/admin/views.py` & `paper-streamfield-0.4.0/streamfield/admin/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,37 +93,37 @@
             "pk": record["pk"],
             "instance": block,
             "title": str(block),
             "verbose_name": block._meta.verbose_name,
             "change_button": {
                 "show": has_change_permission or has_view_permission,
                 "title": _("Change block") if has_change_permission else _("View block"),
-                "icon": "fa-pencil" if has_change_permission else "fa-eye",
+                "icon": "bi-pencil-square" if has_change_permission else "bi-eye",
                 "url": reverse(
                     "admin:%s_%s_%s" % (info + ("change",)),
                     args=(block.pk,),
                 ),
             },
             "delete_button": {
                 "title": _("Delete block"),
-                "icon": "fa-trash"
+                "icon": "bi-trash"
             },
         }, request=self.request)
 
     def block_invalid(self, record: Dict[str, Any]) -> str:
         model = record.get("model", "undefined")
         pk = record.get("pk", "undefined")
         return render_to_string("streamfield/admin/invalid_block.html", {
             "uuid": record.get("uuid", ""),
             "model": model,
             "pk": pk,
             "title": _("Invalid block"),
             "delete_button": {
                 "title": _("Delete block"),
-                "icon": "fa-trash"
+                "icon": "bi-trash"
             },
         }, request=self.request)
 
 
 class RenderToolbarView(PermissionMixin, View):
     """
     Проверка прав на переданные модели для отрисовки кнопок StreamField.
```

### Comparing `paper-streamfield-0.3.0/streamfield/blocks.py` & `paper-streamfield-0.4.0/streamfield/blocks.py`

 * *Files identical despite different names*

### Comparing `paper-streamfield-0.3.0/streamfield/field/forms.py` & `paper-streamfield-0.4.0/streamfield/field/forms.py`

 * *Files identical despite different names*

### Comparing `paper-streamfield-0.3.0/streamfield/field/models.py` & `paper-streamfield-0.4.0/streamfield/field/models.py`

 * *Files identical despite different names*

### Comparing `paper-streamfield-0.3.0/streamfield/helpers.py` & `paper-streamfield-0.4.0/streamfield/helpers.py`

 * *Files identical despite different names*

### Comparing `paper-streamfield-0.3.0/streamfield/renderer.py` & `paper-streamfield-0.4.0/streamfield/renderer.py`

 * *Files identical despite different names*

### Comparing `paper-streamfield-0.3.0/streamfield/static/streamfield/dist/assets/sortable.svg` & `paper-streamfield-0.4.0/streamfield/static/streamfield/dist/assets/sortable.svg`

 * *Files identical despite different names*

### Comparing `paper-streamfield-0.3.0/streamfield/static/streamfield/dist/assets/spinner.svg` & `paper-streamfield-0.4.0/streamfield/static/streamfield/dist/assets/spinner.svg`

 * *Files identical despite different names*

### Comparing `paper-streamfield-0.3.0/streamfield/static/streamfield/dist/widget.css` & `paper-streamfield-0.4.0/streamfield/static/streamfield/dist/widget.css`

 * *Files identical despite different names*

### Comparing `paper-streamfield-0.3.0/streamfield/static/streamfield/dist/widget.js` & `paper-streamfield-0.4.0/streamfield/static/streamfield/dist/widget.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -26,19 +26,17 @@
         if (r[6] = 15 & r[6] | 64, r[8] = 63 & r[8] | 128, t) {
             s = s || 0;
             for (let e = 0; e < 16; ++e) t[s + e] = r[e];
             return t
         }
         return i(r)
     };
-    const d = window.paperAdmin.Sortable,
-        c = window.paperAdmin.Widget,
-        u = window.paperAdmin.popupUtils,
-        h = window.paperAdmin.modals;
-    class p {
+    const d = window.paperAdmin.popupUtils,
+        c = window.paperAdmin.modals;
+    class u {
         constructor(e) {
             this.field = e, this.control = this.field.querySelector(`.${this.CSS.control}`), this.blocks = this.field.querySelector(`.${this.CSS.blocks}`), this.toolbar = this.field.querySelector(`.${this.CSS.toolbar}`), this._sortable = this._initSortable(), this._addListeners(), this._updateBlockMap(), this.wrapPreloader(Promise.all([this.update(), this.updateToolbar()]))
         }
         get STATUS() {
             return this.constructor.STATUS
         }
         get CSS() {
@@ -84,29 +82,29 @@
                     return "string" == typeof r && t(r) ? o[r] = s : (e = !0, r = l(), o[r] = {
                         uuid: r
                     })
                 }));
             this._blockMap = o, s && (this.value = s)
         }
         _initSortable() {
-            return d.create(this.blocks, {
+            return Sortable.create(this.blocks, {
                 animation: 0,
                 draggable: `.${this.CSS.block}`,
                 filter: (e, t) => this.status === this.STATUS.LOADING || (!t || void 0),
                 handle: `.${this.CSS.sortableHandler}`,
                 ghostClass: "sortable-ghost",
                 onEnd: () => {
                     this.save()
                 }
             })
         }
         _addListeners() {
             this.field.addEventListener("click", (e => {
                 const t = e.target.closest(`.${this.CSS.deleteBlockButton}`);
-                t && (e.preventDefault(), t.disabled = !0, h.createModal({
+                t && (e.preventDefault(), t.disabled = !0, c.createModal({
                     modalClass: "paper-modal--warning fade",
                     title: gettext("Confirm deletion"),
                     body: gettext("Are you sure you want to <b>DELETE</b> selected block from this field?"),
                     buttons: [{
                         label: gettext("Cancel"),
                         buttonClass: "btn-light",
                         onClick: (e, t) => {
@@ -130,23 +128,23 @@
                 }));
                 const o = e.target.closest(`.${this.CSS.changeBlockButton}`);
                 if (o) {
                     e.preventDefault();
                     const t = $.Event("django:show-related", {
                         href: o.href
                     });
-                    $(o).trigger(t), t.isDefaultPrevented() || f(o)
+                    $(o).trigger(t), t.isDefaultPrevented() || h(o)
                 }
                 const s = e.target.closest(`.${this.CSS.dropdownItemButton}`);
                 if (s) {
                     e.preventDefault();
                     const t = $.Event("django:show-related", {
                         href: s.href
                     });
-                    $(s).trigger(t), t.isDefaultPrevented() || f(s)
+                    $(s).trigger(t), t.isDefaultPrevented() || h(s)
                 }
             }))
         }
         _appendBlock(e) {
             const o = e.uuid;
             if (!t(o)) throw new Error("Invalid UUID");
             const s = this.value;
@@ -178,15 +176,15 @@
                 body: JSON.stringify(e)
             }).then((e => {
                 if (!e.ok) throw `${e.status} ${e.statusText}`;
                 return e.json()
             })).then((e => {
                 this.blocks.innerHTML = e.blocks
             })).catch((e => {
-                e instanceof Error && console.error(e), h.showErrors(e)
+                e instanceof Error && console.error(e), c.showErrors(e)
             }))
         }
         renderToolbar(e) {
             const t = this.field.dataset.renderToolbarUrl;
             return fetch(t, {
                 method: "POST",
                 mode: "same-origin",
@@ -205,78 +203,73 @@
         updateToolbar() {
             return this.renderToolbar({
                 field_id: this.control.id,
                 models: this.allowedModels
             })
         }
     }
-    p.STATUS = {
+
+    function h(e) {
+        return d.showAdminPopup(e, /^(change|add|lookup)_/, !0)
+    }
+    var p;
+    u.STATUS = {
         LOADING: "loading",
         READY: "ready"
-    }, p.CSS = {
+    }, u.CSS = {
         field: "stream-field",
         control: "stream-field__control",
         blocks: "stream-field__blocks",
         block: "stream-field__block",
         toolbar: "stream-field__toolbar",
         sortableHandler: "stream-field__sortable-handler",
         changeBlockButton: "stream-field__change-btn",
         deleteBlockButton: "stream-field__delete-btn",
         dropdownItemButton: "stream-field__dropdown-item"
-    };
-    const m = new class extends c {
-        _init(e) {
-            e._streamField = new p(e, this)
-        }
-        _destroy(e) {
+    }, XClass.register("paper-streamfield", {
+        init: function(e) {
+            e._streamField = new u(e, this)
+        },
+        destroy: function(e) {
             e._streamField && (e._streamField.destroy(), delete e._streamField)
         }
-        getStreamFieldInstance(e) {
-            return e._streamField
-        }
-    };
-
-    function f(e) {
-        return u.showAdminPopup(e, /^(change|add|lookup)_/, !0)
-    }
-    var S;
-    "function" == typeof m.bind ? (m.bind(".stream-field"), m.attach()) : (m.initAll(".stream-field"), m.observe(".stream-field")), window.dismissAddStreamBlockPopup = function(e, t) {
-        const o = u.removePopupIndex(e.name),
+    }), window.dismissAddStreamBlockPopup = function(e, t) {
+        const o = d.removePopupIndex(e.name),
             s = /^(.+)--(.+)\.(.+)$/.exec(o);
         if (s) {
             const o = document.getElementById(s[1]).closest(".stream-field"),
-                r = o && m.getStreamFieldInstance(o);
+                r = o && o._streamField;
             r._appendBlock({
                 model: `${s[2]}.${s[3]}`,
                 pk: t,
                 uuid: l()
-            }), r.wrapPreloader(r.update()), u.removeRelatedWindow(e), e.close()
+            }), r.wrapPreloader(r.update()), d.removeRelatedWindow(e), e.close()
         }
     }, window.dismissChangeStreamBlockPopup = function(e) {
-        const t = "change_" + u.removePopupIndex(e.name),
+        const t = "change_" + d.removePopupIndex(e.name),
             o = document.getElementById(t),
             s = o && o.closest(".paper-widget"),
             r = s && s.firstElementChild;
-        (r && m.getStreamFieldInstance(r)).update(), u.removeRelatedWindow(e), e.close()
+        (r && r._streamField).update(), d.removeRelatedWindow(e), e.close()
     }, window.dismissDeleteStreamBlockPopup = function(e, t) {
-        const o = u.removePopupIndex(e.name),
+        const o = d.removePopupIndex(e.name),
             s = /^(.+)--(.+)\.(.+)$/.exec(o);
         if (s) {
             const t = document.getElementById(s[1]).closest(".stream-field"),
-                o = t && m.getStreamFieldInstance(t);
-            o.wrapPreloader(o.update()), u.removeRelatedWindow(e), e.close()
+                o = t && t._streamField;
+            o.wrapPreloader(o.update()), d.removeRelatedWindow(e), e.close()
         }
-    }, window.dismissRelatedLookupPopup = (S = window.dismissRelatedLookupPopup, (e, t) => {
-        const o = u.removePopupIndex(e.name),
+    }, window.dismissRelatedLookupPopup = (p = window.dismissRelatedLookupPopup, (e, t) => {
+        const o = d.removePopupIndex(e.name),
             s = /^(.+)--(.+)\.(.+)$/.exec(o);
         if (s) {
             const o = document.getElementById(s[1]).closest(".stream-field"),
-                r = o && m.getStreamFieldInstance(o);
+                r = o && o._streamField;
             r._appendBlock({
                 model: `${s[2]}.${s[3]}`,
                 pk: t,
                 uuid: l()
-            }), r.wrapPreloader(r.update()), u.removeRelatedWindow(e), e.close()
-        } else S(e, t)
+            }), r.wrapPreloader(r.update()), d.removeRelatedWindow(e), e.close()
+        } else p(e, t)
     })
 }();
 //# sourceMappingURL=widget.js.map
```

### Comparing `paper-streamfield-0.3.0/streamfield/static/streamfield/dist/widget.js.map` & `paper-streamfield-0.4.0/streamfield/static/streamfield/dist/widget.js.map`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9042894935752078%*

 * *Differences: {"'mappings'": "'yBAAA,4HCMA,MAJA,SAAkBA,GAChB,MAAuB,iBAATA,GAAqB,OAAWA,EAChD,ECHA,OACEC,WAFmC,oBAAXC,QAA0BA,OAAOD,YAAcC,OAAOD,WAAWE,KAAKD,SCGhG,IAAIE,EACJ,MAAMC,EAAQ,IAAIC,WAAW,IACd,SAASC,IAEtB,IAAKH,IAEHA,EAAoC,oBAAXF,QAA0BA,OAAOE,iBAAmBF,OAAOE,gBAAgBD,KAAKD,SAEpGE,GACH,MAAM,IAAII,MAAM,4GAIpB,OAAOJ,EAAgBC,EACzB,CCXA,MAAMI,EAAY,GAElB,IAAK,IAAIC,EAAI,EAAGA,EAAI,MAAOA,EACzBD,EAAUE,MAAMD,EAAI,KAAOE,SAAS,IAAIC,MAAM,IAGzC,SAASC,EAAgBC,EAAKC,EAAS,GAG5C,OAAQP,EAAUM,EAAIC,EAAS,IAAMP,EAAUM,EAAIC,EAAS,IAAMP,EAAUM,EA […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "widget.js",
-    "mappings": "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",
+    "mappings": "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",
     "names": [
         "uuid",
         "randomUUID",
         "crypto",
         "bind",
         "getRandomValues",
         "rnds8",
@@ -20,19 +20,17 @@
         "arr",
         "offset",
         "toLowerCase",
         "options",
         "buf",
         "rnds",
         "random",
-        "Sortable",
+        "popupUtils",
         "window",
         "paperAdmin",
-        "Widget",
-        "popupUtils",
         "modals",
         "StreamField",
         "constructor",
         "element",
         "this",
         "field",
         "control",
@@ -76,14 +74,15 @@
         "hasBadBlocks",
         "result",
         "processedValue",
         "map",
         "record",
         "uuid_validate",
         "uuid4",
+        "Sortable",
         "create",
         "animation",
         "draggable",
         "filter",
         "event",
         "target",
         "LOADING",
@@ -149,25 +148,21 @@
         "error",
         "showErrors",
         "renderToolbar",
         "renderToolbarUrl",
         "field_id",
         "id",
         "models",
-        "widget",
-        "_init",
-        "_streamField",
-        "_destroy",
-        "getStreamFieldInstance",
         "triggeringLink",
         "showAdminPopup",
         "originalFunc",
-        "attach",
-        "initAll",
-        "observe",
+        "XClass",
+        "register",
+        "init",
+        "_streamField",
         "dismissAddStreamBlockPopup",
         "win",
         "newId",
         "name",
         "removePopupIndex",
         "match",
         "exec",
@@ -199,11 +194,11 @@
     "sourcesContent": [
         "export default /^(?:[0-9a-f]{8}-[0-9a-f]{4}-[1-5][0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}|00000000-0000-0000-0000-000000000000)$/i;",
         "import REGEX from './regex.js';\n\nfunction validate(uuid) {\n  return typeof uuid === 'string' && REGEX.test(uuid);\n}\n\nexport default validate;",
         "const randomUUID = typeof crypto !== 'undefined' && crypto.randomUUID && crypto.randomUUID.bind(crypto);\nexport default {\n  randomUUID\n};",
         "// Unique ID creation requires a high quality random # generator. In the browser we therefore\n// require the crypto API and do not support built-in fallback to lower quality random number\n// generators (like Math.random()).\nlet getRandomValues;\nconst rnds8 = new Uint8Array(16);\nexport default function rng() {\n  // lazy load so that environments that need to polyfill have a chance to do so\n  if (!getRandomValues) {\n    // getRandomValues needs to be invoked in a context where \"this\" is a Crypto implementation.\n    getRandomValues = typeof crypto !== 'undefined' && crypto.getRandomValues && crypto.getRandomValues.bind(crypto);\n\n    if (!getRandomValues) {\n      throw new Error('crypto.getRandomValues() not supported. See https://github.com/uuidjs/uuid#getrandomvalues-not-supported');\n    }\n  }\n\n  return getRandomValues(rnds8);\n}",
         "import validate from './validate.js';\n/**\n * Convert array of 16 byte values to UUID string format of the form:\n * XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX\n */\n\nconst byteToHex = [];\n\nfor (let i = 0; i < 256; ++i) {\n  byteToHex.push((i + 0x100).toString(16).slice(1));\n}\n\nexport function unsafeStringify(arr, offset = 0) {\n  // Note: Be careful editing this code!  It's been tuned for performance\n  // and works in ways you may not expect. See https://github.com/uuidjs/uuid/pull/434\n  return (byteToHex[arr[offset + 0]] + byteToHex[arr[offset + 1]] + byteToHex[arr[offset + 2]] + byteToHex[arr[offset + 3]] + '-' + byteToHex[arr[offset + 4]] + byteToHex[arr[offset + 5]] + '-' + byteToHex[arr[offset + 6]] + byteToHex[arr[offset + 7]] + '-' + byteToHex[arr[offset + 8]] + byteToHex[arr[offset + 9]] + '-' + byteToHex[arr[offset + 10]] + byteToHex[arr[offset + 11]] + byteToHex[arr[offset + 12]] + byteToHex[arr[offset + 13]] + byteToHex[arr[offset + 14]] + byteToHex[arr[offset + 15]]).toLowerCase();\n}\n\nfunction stringify(arr, offset = 0) {\n  const uuid = unsafeStringify(arr, offset); // Consistency check for valid UUID.  If this throws, it's likely due to one\n  // of the following:\n  // - One or more input array values don't map to a hex octet (leading to\n  // \"undefined\" in the uuid)\n  // - Invalid input values for the RFC `version` or `variant` fields\n\n  if (!validate(uuid)) {\n    throw TypeError('Stringified UUID is invalid');\n  }\n\n  return uuid;\n}\n\nexport default stringify;",
         "import native from './native.js';\nimport rng from './rng.js';\nimport { unsafeStringify } from './stringify.js';\n\nfunction v4(options, buf, offset) {\n  if (native.randomUUID && !buf && !options) {\n    return native.randomUUID();\n  }\n\n  options = options || {};\n  const rnds = options.random || (options.rng || rng)(); // Per 4.4, set bits for version and `clock_seq_hi_and_reserved`\n\n  rnds[6] = rnds[6] & 0x0f | 0x40;\n  rnds[8] = rnds[8] & 0x3f | 0x80; // Copy bytes to buffer, if provided\n\n  if (buf) {\n    offset = offset || 0;\n\n    for (let i = 0; i < 16; ++i) {\n      buf[offset + i] = rnds[i];\n    }\n\n    return buf;\n  }\n\n  return unsafeStringify(rnds);\n}\n\nexport default v4;",
-        "/* global gettext */\nimport { v4 as uuid4, validate as uuid_validate } from \"uuid\";\n\nimport \"./widget.scss\";\n\nconst Sortable = window.paperAdmin.Sortable;\nconst Widget = window.paperAdmin.Widget;\nconst popupUtils = window.paperAdmin.popupUtils;\nconst modals = window.paperAdmin.modals;\n\nclass StreamField {\n    static STATUS = {\n        LOADING: \"loading\",\n        READY: \"ready\"\n    };\n\n    static CSS = {\n        field: \"stream-field\",\n        control: \"stream-field__control\",\n        blocks: \"stream-field__blocks\",\n        block: \"stream-field__block\",\n        toolbar: \"stream-field__toolbar\",\n        sortableHandler: \"stream-field__sortable-handler\",\n        changeBlockButton: \"stream-field__change-btn\",\n        deleteBlockButton: \"stream-field__delete-btn\",\n        dropdownItemButton: \"stream-field__dropdown-item\" // create or lookup block\n    };\n\n    constructor(element) {\n        this.field = element;\n        this.control = this.field.querySelector(`.${this.CSS.control}`);\n        this.blocks = this.field.querySelector(`.${this.CSS.blocks}`);\n        this.toolbar = this.field.querySelector(`.${this.CSS.toolbar}`);\n\n        this._sortable = this._initSortable();\n        this._addListeners();\n        this._updateBlockMap();\n\n        this.wrapPreloader(Promise.all([this.update(), this.updateToolbar()]));\n    }\n\n    get STATUS() {\n        return this.constructor.STATUS;\n    }\n\n    get CSS() {\n        return this.constructor.CSS;\n    }\n\n    /**\n     * @returns {Array}\n     */\n    get value() {\n        let data;\n        try {\n            data = JSON.parse(this.control.value);\n        } catch {\n            data = [];\n        }\n        return data;\n    }\n\n    /**\n     * @param {string|Array} data\n     */\n    set value(data) {\n        if (typeof data !== \"string\") {\n            data = JSON.stringify(data);\n        }\n        this.control.value = data;\n    }\n\n    /**\n     * @returns {string}\n     */\n    get status() {\n        return Object.values(this.STATUS).find(value => {\n            return this.field.classList.contains(`${this.CSS.field}--${value}`);\n        });\n    }\n\n    /**\n     * @param {string} status\n     */\n    set status(status) {\n        Object.values(this.STATUS).forEach(value => {\n            this.field.classList.toggle(`${this.CSS.field}--${value}`, status === value);\n        });\n    }\n\n    /**\n     * @returns {String[]}\n     */\n    get allowedModels() {\n        return JSON.parse(this.control.dataset.allowedModels);\n    }\n\n    /**\n     * @returns {HTMLElement[]}\n     */\n    getBlocks() {\n        return Array.from(this.blocks.querySelectorAll(`.${this.CSS.block}`));\n    }\n\n    /**\n     * @param {string} uuid\n     * @returns {Object}\n     */\n    getBlockByUUID(uuid) {\n        return this._blockMap[uuid];\n    }\n\n    destroy() {\n        if (this._sortable) {\n            this._sortable.destroy();\n        }\n\n        // TODO: remove event listeners\n    }\n\n    /**\n     * \u0421\u043e\u0437\u0434\u0430\u0451\u0442 \u043e\u0431\u044a\u0435\u043a\u0442 \u0434\u043b\u044f \u0431\u044b\u0441\u0442\u0440\u043e\u0433\u043e \u043f\u043e\u0438\u0441\u043a\u0430 \u0431\u043b\u043e\u043a\u043e\u0432 \u043f\u043e UUID.\n     *\n     * @returns {Object}\n     */\n    _updateBlockMap() {\n        let hasBadBlocks = false;\n        const result = {};\n\n        const processedValue = this.value.map(record => {\n            let uuid = record[\"uuid\"];\n            if (typeof uuid === \"string\" && uuid_validate(uuid)) {\n                return (result[uuid] = record);\n            } else {\n                hasBadBlocks = true;\n                uuid = uuid4();\n                return (result[uuid] = { uuid: uuid });\n            }\n        });\n\n        this._blockMap = result;\n        if (processedValue) {\n            this.value = processedValue;\n        }\n    }\n\n    /**\n     * @returns {*}\n     * @private\n     */\n    _initSortable() {\n        return Sortable.create(this.blocks, {\n            animation: 0,\n            draggable: `.${this.CSS.block}`,\n            filter: (event, target) => {\n                if (this.status === this.STATUS.LOADING) {\n                    return true;\n                }\n\n                if (!target) {\n                    return true;\n                }\n            },\n            handle: `.${this.CSS.sortableHandler}`,\n            ghostClass: \"sortable-ghost\",\n            onEnd: () => {\n                this.save();\n            }\n        });\n    }\n\n    _addListeners() {\n        this.field.addEventListener(\"click\", event => {\n            const deleteButton = event.target.closest(`.${this.CSS.deleteBlockButton}`);\n            if (deleteButton) {\n                event.preventDefault();\n                deleteButton.disabled = true;\n\n                modals.createModal({\n                    modalClass: \"paper-modal--warning fade\",\n                    title: gettext(\"Confirm deletion\"),\n                    body: gettext(\"Are you sure you want to <b>DELETE</b> selected block from this field?\"),\n                    buttons: [\n                        {\n                            label: gettext(\"Cancel\"),\n                            buttonClass: \"btn-light\",\n                            onClick: (event, popup) => {\n                                popup.destroy();\n                            }\n                        },\n                        {\n                            autofocus: true,\n                            label: gettext(\"Delete\"),\n                            buttonClass: \"btn-danger\",\n                            onClick: (event, popup) => {\n                                popup.destroy();\n\n                                const block = deleteButton.closest(`.${this.CSS.block}`);\n                                block.remove();\n\n                                this.save();\n                                this.wrapPreloader(this.update());\n                            }\n                        }\n                    ],\n                    onInit: function () {\n                        this.show();\n                    },\n                    onDestroy: function () {\n                        deleteButton.disabled = false;\n                    }\n                });\n            }\n\n            const changeButton = event.target.closest(`.${this.CSS.changeBlockButton}`);\n            if (changeButton) {\n                event.preventDefault();\n                const jQueryEvent = $.Event(\"django:show-related\", { href: changeButton.href });\n                $(changeButton).trigger(jQueryEvent);\n                if (!jQueryEvent.isDefaultPrevented()) {\n                    showStreamBlockPopup(changeButton);\n                }\n            }\n\n            const dropdownItem = event.target.closest(`.${this.CSS.dropdownItemButton}`);\n            if (dropdownItem) {\n                event.preventDefault();\n                const jQueryEvent = $.Event(\"django:show-related\", { href: dropdownItem.href });\n                $(dropdownItem).trigger(jQueryEvent);\n                if (!jQueryEvent.isDefaultPrevented()) {\n                    showStreamBlockPopup(dropdownItem);\n                }\n            }\n        });\n    }\n\n    /**\n     * @param {Object} block\n     * @private\n     */\n    _appendBlock(block) {\n        const uuid = block.uuid;\n        if (!uuid_validate(uuid)) {\n            throw new Error(\"Invalid UUID\");\n        }\n\n        const newValue = this.value;\n        newValue.push(block);\n        this.value = newValue;\n\n        this._blockMap[uuid] = block;\n    }\n\n    save() {\n        this.value = this.getBlocks().map(block => {\n            const uuid = block.dataset.uuid;\n            return this.getBlockByUUID(uuid);\n        });\n    }\n\n    update() {\n        return this.renderStream(this.value);\n    }\n\n    /**\n     * @param {Promise} promise\n     * @returns {Promise}\n     */\n    wrapPreloader(promise) {\n        this.status = this.STATUS.LOADING;\n        return promise.finally(() => {\n            this.status = this.STATUS.READY;\n        });\n    }\n\n    renderStream(data) {\n        const renderUrl = this.field.dataset.renderStreamUrl;\n        return fetch(renderUrl, {\n            method: \"POST\",\n            mode: \"same-origin\",\n            cache: \"no-store\",\n            headers: {\n                \"Content-Type\": \"application/json;charset=utf-8\"\n            },\n            body: JSON.stringify(data)\n        })\n            .then(response => {\n                if (!response.ok) {\n                    throw `${response.status} ${response.statusText}`;\n                }\n                return response.json();\n            })\n            .then(response => {\n                this.blocks.innerHTML = response.blocks;\n            })\n            .catch(reason => {\n                if (reason instanceof Error) {\n                    // JS-\u043e\u0448\u0438\u0431\u043a\u0438 \u0434\u0443\u0431\u043b\u0438\u0440\u0443\u0435\u043c \u0432 \u043a\u043e\u043d\u0441\u043e\u043b\u044c\n                    console.error(reason);\n                }\n                modals.showErrors(reason);\n            });\n    }\n\n    renderToolbar(data) {\n        const renderUrl = this.field.dataset.renderToolbarUrl;\n        return fetch(renderUrl, {\n            method: \"POST\",\n            mode: \"same-origin\",\n            cache: \"no-store\",\n            headers: {\n                \"Content-Type\": \"application/json;charset=utf-8\"\n            },\n            body: JSON.stringify(data)\n        })\n            .then(response => {\n                if (!response.ok) {\n                    throw `${response.status} ${response.statusText}`;\n                }\n                return response.json();\n            })\n            .then(response => {\n                this.toolbar.innerHTML = response.toolbar;\n            });\n    }\n\n    updateToolbar() {\n        return this.renderToolbar({\n            field_id: this.control.id,\n            models: this.allowedModels\n        });\n    }\n}\n\nclass StreamFieldWidget extends Widget {\n    _init(element) {\n        element._streamField = new StreamField(element, this);\n    }\n\n    _destroy(element) {\n        if (element._streamField) {\n            element._streamField.destroy();\n            delete element._streamField;\n        }\n    }\n\n    getStreamFieldInstance(element) {\n        return element._streamField;\n    }\n}\n\nconst widget = new StreamFieldWidget();\nif (typeof widget.bind === \"function\") {\n    // new-style widgets\n    widget.bind(\".stream-field\");\n    widget.attach();\n} else {\n    // old-style widgets\n    widget.initAll(\".stream-field\");\n    widget.observe(\".stream-field\");\n}\n\n\n/**\n * @param {HTMLElement} triggeringLink\n */\nfunction showStreamBlockPopup(triggeringLink) {\n    return popupUtils.showAdminPopup(triggeringLink, /^(change|add|lookup)_/, true);\n}\n\n/**\n * @param {Window} win\n * @param {String} newId\n */\nfunction dismissAddStreamBlockPopup(win, newId) {\n    const name = popupUtils.removePopupIndex(win.name);\n    const match = /^(.+)--(.+)\\.(.+)$/.exec(name);\n    if (match) {\n        const control = document.getElementById(match[1]);\n        const field = control.closest(\".stream-field\");\n        const streamField = field && widget.getStreamFieldInstance(field);\n\n        streamField._appendBlock({\n            model: `${match[2]}.${match[3]}`,\n            pk: newId,\n            uuid: uuid4()\n        });\n\n        streamField.wrapPreloader(streamField.update());\n\n        popupUtils.removeRelatedWindow(win);\n        win.close();\n    }\n}\n\n/**\n * @param {Window} win\n */\nfunction dismissChangeStreamBlockPopup(win) {\n    const name = \"change_\" + popupUtils.removePopupIndex(win.name);\n    const element = document.getElementById(name);\n    const fieldWrapper = element && element.closest(\".paper-widget\");\n    const field = fieldWrapper && fieldWrapper.firstElementChild;\n    const instance = field && widget.getStreamFieldInstance(field);\n\n    instance.update();\n\n    popupUtils.removeRelatedWindow(win);\n    win.close();\n}\n\n/**\n * @param {Window} win\n * @param {String} objId\n */\nfunction dismissDeleteStreamBlockPopup(win, objId) {\n    const name = popupUtils.removePopupIndex(win.name);\n    const match = /^(.+)--(.+)\\.(.+)$/.exec(name);\n    if (match) {\n        const control = document.getElementById(match[1]);\n        const field = control.closest(\".stream-field\");\n        const streamField = field && widget.getStreamFieldInstance(field);\n\n        streamField.wrapPreloader(streamField.update());\n\n        popupUtils.removeRelatedWindow(win);\n        win.close();\n    }\n}\n\n/**\n * \u041e\u0431\u0451\u0440\u0442\u043a\u0430 \u043d\u0430\u0434 Django-\u043e\u0431\u0440\u0430\u0431\u043e\u0442\u0447\u0438\u043a\u043e\u043c `window.dismissRelatedLookupPopup`.\n * @param {Function} originalFunc\n */\nfunction dismissLookupStreamBlockPopup(originalFunc) {\n    return (win, chosenId) => {\n        const name = popupUtils.removePopupIndex(win.name);\n        const match = /^(.+)--(.+)\\.(.+)$/.exec(name);\n        if (match) {\n            const control = document.getElementById(match[1]);\n            const field = control.closest(\".stream-field\");\n            const streamField = field && widget.getStreamFieldInstance(field);\n\n            streamField._appendBlock({\n                model: `${match[2]}.${match[3]}`,\n                pk: chosenId,\n                uuid: uuid4()\n            });\n\n            streamField.wrapPreloader(streamField.update());\n\n            popupUtils.removeRelatedWindow(win);\n            win.close();\n        } else {\n            originalFunc(win, chosenId);\n        }\n    };\n}\n\nwindow.dismissAddStreamBlockPopup = dismissAddStreamBlockPopup;\nwindow.dismissChangeStreamBlockPopup = dismissChangeStreamBlockPopup;\nwindow.dismissDeleteStreamBlockPopup = dismissDeleteStreamBlockPopup;\n\n// Wrap default `dismissRelatedLookupPopup`.\nwindow.dismissRelatedLookupPopup = dismissLookupStreamBlockPopup(window.dismissRelatedLookupPopup);\n"
+        "/* global gettext */\n/* global Sortable */\n/* global XClass */\nimport { v4 as uuid4, validate as uuid_validate } from \"uuid\";\n\nimport \"./widget.scss\";\n\nconst popupUtils = window.paperAdmin.popupUtils;\nconst modals = window.paperAdmin.modals;\n\nclass StreamField {\n    static STATUS = {\n        LOADING: \"loading\",\n        READY: \"ready\"\n    };\n\n    static CSS = {\n        field: \"stream-field\",\n        control: \"stream-field__control\",\n        blocks: \"stream-field__blocks\",\n        block: \"stream-field__block\",\n        toolbar: \"stream-field__toolbar\",\n        sortableHandler: \"stream-field__sortable-handler\",\n        changeBlockButton: \"stream-field__change-btn\",\n        deleteBlockButton: \"stream-field__delete-btn\",\n        dropdownItemButton: \"stream-field__dropdown-item\" // create or lookup block\n    };\n\n    constructor(element) {\n        this.field = element;\n        this.control = this.field.querySelector(`.${this.CSS.control}`);\n        this.blocks = this.field.querySelector(`.${this.CSS.blocks}`);\n        this.toolbar = this.field.querySelector(`.${this.CSS.toolbar}`);\n\n        this._sortable = this._initSortable();\n        this._addListeners();\n        this._updateBlockMap();\n\n        this.wrapPreloader(Promise.all([this.update(), this.updateToolbar()]));\n    }\n\n    get STATUS() {\n        return this.constructor.STATUS;\n    }\n\n    get CSS() {\n        return this.constructor.CSS;\n    }\n\n    /**\n     * @returns {Array}\n     */\n    get value() {\n        let data;\n        try {\n            data = JSON.parse(this.control.value);\n        } catch {\n            data = [];\n        }\n        return data;\n    }\n\n    /**\n     * @param {string|Array} data\n     */\n    set value(data) {\n        if (typeof data !== \"string\") {\n            data = JSON.stringify(data);\n        }\n        this.control.value = data;\n    }\n\n    /**\n     * @returns {string}\n     */\n    get status() {\n        return Object.values(this.STATUS).find(value => {\n            return this.field.classList.contains(`${this.CSS.field}--${value}`);\n        });\n    }\n\n    /**\n     * @param {string} status\n     */\n    set status(status) {\n        Object.values(this.STATUS).forEach(value => {\n            this.field.classList.toggle(`${this.CSS.field}--${value}`, status === value);\n        });\n    }\n\n    /**\n     * @returns {String[]}\n     */\n    get allowedModels() {\n        return JSON.parse(this.control.dataset.allowedModels);\n    }\n\n    /**\n     * @returns {HTMLElement[]}\n     */\n    getBlocks() {\n        return Array.from(this.blocks.querySelectorAll(`.${this.CSS.block}`));\n    }\n\n    /**\n     * @param {string} uuid\n     * @returns {Object}\n     */\n    getBlockByUUID(uuid) {\n        return this._blockMap[uuid];\n    }\n\n    destroy() {\n        if (this._sortable) {\n            this._sortable.destroy();\n        }\n\n        // TODO: remove event listeners\n    }\n\n    /**\n     * \u0421\u043e\u0437\u0434\u0430\u0451\u0442 \u043e\u0431\u044a\u0435\u043a\u0442 \u0434\u043b\u044f \u0431\u044b\u0441\u0442\u0440\u043e\u0433\u043e \u043f\u043e\u0438\u0441\u043a\u0430 \u0431\u043b\u043e\u043a\u043e\u0432 \u043f\u043e UUID.\n     *\n     * @returns {Object}\n     */\n    _updateBlockMap() {\n        let hasBadBlocks = false;\n        const result = {};\n\n        const processedValue = this.value.map(record => {\n            let uuid = record[\"uuid\"];\n            if (typeof uuid === \"string\" && uuid_validate(uuid)) {\n                return (result[uuid] = record);\n            } else {\n                hasBadBlocks = true;\n                uuid = uuid4();\n                return (result[uuid] = { uuid: uuid });\n            }\n        });\n\n        this._blockMap = result;\n        if (processedValue) {\n            this.value = processedValue;\n        }\n    }\n\n    /**\n     * @returns {*}\n     * @private\n     */\n    _initSortable() {\n        return Sortable.create(this.blocks, {\n            animation: 0,\n            draggable: `.${this.CSS.block}`,\n            filter: (event, target) => {\n                if (this.status === this.STATUS.LOADING) {\n                    return true;\n                }\n\n                if (!target) {\n                    return true;\n                }\n            },\n            handle: `.${this.CSS.sortableHandler}`,\n            ghostClass: \"sortable-ghost\",\n            onEnd: () => {\n                this.save();\n            }\n        });\n    }\n\n    _addListeners() {\n        this.field.addEventListener(\"click\", event => {\n            const deleteButton = event.target.closest(`.${this.CSS.deleteBlockButton}`);\n            if (deleteButton) {\n                event.preventDefault();\n                deleteButton.disabled = true;\n\n                modals.createModal({\n                    modalClass: \"paper-modal--warning fade\",\n                    title: gettext(\"Confirm deletion\"),\n                    body: gettext(\"Are you sure you want to <b>DELETE</b> selected block from this field?\"),\n                    buttons: [\n                        {\n                            label: gettext(\"Cancel\"),\n                            buttonClass: \"btn-light\",\n                            onClick: (event, popup) => {\n                                popup.destroy();\n                            }\n                        },\n                        {\n                            autofocus: true,\n                            label: gettext(\"Delete\"),\n                            buttonClass: \"btn-danger\",\n                            onClick: (event, popup) => {\n                                popup.destroy();\n\n                                const block = deleteButton.closest(`.${this.CSS.block}`);\n                                block.remove();\n\n                                this.save();\n                                this.wrapPreloader(this.update());\n                            }\n                        }\n                    ],\n                    onInit: function () {\n                        this.show();\n                    },\n                    onDestroy: function () {\n                        deleteButton.disabled = false;\n                    }\n                });\n            }\n\n            const changeButton = event.target.closest(`.${this.CSS.changeBlockButton}`);\n            if (changeButton) {\n                event.preventDefault();\n                const jQueryEvent = $.Event(\"django:show-related\", { href: changeButton.href });\n                $(changeButton).trigger(jQueryEvent);\n                if (!jQueryEvent.isDefaultPrevented()) {\n                    showStreamBlockPopup(changeButton);\n                }\n            }\n\n            const dropdownItem = event.target.closest(`.${this.CSS.dropdownItemButton}`);\n            if (dropdownItem) {\n                event.preventDefault();\n                const jQueryEvent = $.Event(\"django:show-related\", { href: dropdownItem.href });\n                $(dropdownItem).trigger(jQueryEvent);\n                if (!jQueryEvent.isDefaultPrevented()) {\n                    showStreamBlockPopup(dropdownItem);\n                }\n            }\n        });\n    }\n\n    /**\n     * @param {Object} block\n     * @private\n     */\n    _appendBlock(block) {\n        const uuid = block.uuid;\n        if (!uuid_validate(uuid)) {\n            throw new Error(\"Invalid UUID\");\n        }\n\n        const newValue = this.value;\n        newValue.push(block);\n        this.value = newValue;\n\n        this._blockMap[uuid] = block;\n    }\n\n    save() {\n        this.value = this.getBlocks().map(block => {\n            const uuid = block.dataset.uuid;\n            return this.getBlockByUUID(uuid);\n        });\n    }\n\n    update() {\n        return this.renderStream(this.value);\n    }\n\n    /**\n     * @param {Promise} promise\n     * @returns {Promise}\n     */\n    wrapPreloader(promise) {\n        this.status = this.STATUS.LOADING;\n        return promise.finally(() => {\n            this.status = this.STATUS.READY;\n        });\n    }\n\n    renderStream(data) {\n        const renderUrl = this.field.dataset.renderStreamUrl;\n        return fetch(renderUrl, {\n            method: \"POST\",\n            mode: \"same-origin\",\n            cache: \"no-store\",\n            headers: {\n                \"Content-Type\": \"application/json;charset=utf-8\"\n            },\n            body: JSON.stringify(data)\n        })\n            .then(response => {\n                if (!response.ok) {\n                    throw `${response.status} ${response.statusText}`;\n                }\n                return response.json();\n            })\n            .then(response => {\n                this.blocks.innerHTML = response.blocks;\n            })\n            .catch(reason => {\n                if (reason instanceof Error) {\n                    // JS-\u043e\u0448\u0438\u0431\u043a\u0438 \u0434\u0443\u0431\u043b\u0438\u0440\u0443\u0435\u043c \u0432 \u043a\u043e\u043d\u0441\u043e\u043b\u044c\n                    console.error(reason);\n                }\n                modals.showErrors(reason);\n            });\n    }\n\n    renderToolbar(data) {\n        const renderUrl = this.field.dataset.renderToolbarUrl;\n        return fetch(renderUrl, {\n            method: \"POST\",\n            mode: \"same-origin\",\n            cache: \"no-store\",\n            headers: {\n                \"Content-Type\": \"application/json;charset=utf-8\"\n            },\n            body: JSON.stringify(data)\n        })\n            .then(response => {\n                if (!response.ok) {\n                    throw `${response.status} ${response.statusText}`;\n                }\n                return response.json();\n            })\n            .then(response => {\n                this.toolbar.innerHTML = response.toolbar;\n            });\n    }\n\n    updateToolbar() {\n        return this.renderToolbar({\n            field_id: this.control.id,\n            models: this.allowedModels\n        });\n    }\n}\n\nXClass.register(\"paper-streamfield\", {\n    init: function (element) {\n        element._streamField = new StreamField(element, this);\n    },\n    destroy: function (element) {\n        if (element._streamField) {\n            element._streamField.destroy();\n            delete element._streamField;\n        }\n    }\n});\n\n/**\n * @param {HTMLElement} triggeringLink\n */\nfunction showStreamBlockPopup(triggeringLink) {\n    return popupUtils.showAdminPopup(triggeringLink, /^(change|add|lookup)_/, true);\n}\n\n/**\n * @param {Window} win\n * @param {String} newId\n */\nfunction dismissAddStreamBlockPopup(win, newId) {\n    const name = popupUtils.removePopupIndex(win.name);\n    const match = /^(.+)--(.+)\\.(.+)$/.exec(name);\n    if (match) {\n        const control = document.getElementById(match[1]);\n        const field = control.closest(\".stream-field\");\n        const streamField = field && field._streamField;\n\n        streamField._appendBlock({\n            model: `${match[2]}.${match[3]}`,\n            pk: newId,\n            uuid: uuid4()\n        });\n\n        streamField.wrapPreloader(streamField.update());\n\n        popupUtils.removeRelatedWindow(win);\n        win.close();\n    }\n}\n\n/**\n * @param {Window} win\n */\nfunction dismissChangeStreamBlockPopup(win) {\n    const name = \"change_\" + popupUtils.removePopupIndex(win.name);\n    const element = document.getElementById(name);\n    const fieldWrapper = element && element.closest(\".paper-widget\");\n    const field = fieldWrapper && fieldWrapper.firstElementChild;\n    const instance = field && field._streamField;\n\n    instance.update();\n\n    popupUtils.removeRelatedWindow(win);\n    win.close();\n}\n\n/**\n * @param {Window} win\n * @param {String} objId\n */\nfunction dismissDeleteStreamBlockPopup(win, objId) {\n    const name = popupUtils.removePopupIndex(win.name);\n    const match = /^(.+)--(.+)\\.(.+)$/.exec(name);\n    if (match) {\n        const control = document.getElementById(match[1]);\n        const field = control.closest(\".stream-field\");\n        const streamField = field && field._streamField;\n\n        streamField.wrapPreloader(streamField.update());\n\n        popupUtils.removeRelatedWindow(win);\n        win.close();\n    }\n}\n\n/**\n * \u041e\u0431\u0451\u0440\u0442\u043a\u0430 \u043d\u0430\u0434 Django-\u043e\u0431\u0440\u0430\u0431\u043e\u0442\u0447\u0438\u043a\u043e\u043c `window.dismissRelatedLookupPopup`.\n * @param {Function} originalFunc\n */\nfunction dismissLookupStreamBlockPopup(originalFunc) {\n    return (win, chosenId) => {\n        const name = popupUtils.removePopupIndex(win.name);\n        const match = /^(.+)--(.+)\\.(.+)$/.exec(name);\n        if (match) {\n            const control = document.getElementById(match[1]);\n            const field = control.closest(\".stream-field\");\n            const streamField = field && field._streamField;\n\n            streamField._appendBlock({\n                model: `${match[2]}.${match[3]}`,\n                pk: chosenId,\n                uuid: uuid4()\n            });\n\n            streamField.wrapPreloader(streamField.update());\n\n            popupUtils.removeRelatedWindow(win);\n            win.close();\n        } else {\n            originalFunc(win, chosenId);\n        }\n    };\n}\n\nwindow.dismissAddStreamBlockPopup = dismissAddStreamBlockPopup;\nwindow.dismissChangeStreamBlockPopup = dismissChangeStreamBlockPopup;\nwindow.dismissDeleteStreamBlockPopup = dismissDeleteStreamBlockPopup;\n\n// Wrap default `dismissRelatedLookupPopup`.\nwindow.dismissRelatedLookupPopup = dismissLookupStreamBlockPopup(window.dismissRelatedLookupPopup);\n"
     ],
     "version": 3
 }
```

### Comparing `paper-streamfield-0.3.0/streamfield/templates/streamfield/admin/block.html` & `paper-streamfield-0.4.0/streamfield/templates/streamfield/admin/block.html`

 * *Files 10% similar despite different names*

```diff
@@ -14,29 +14,29 @@
   <div class="stream-field__block-tools">
     {% block tools %}
       <div class="btn-square-group">
         {% if change_button.show %}
           <a href="{{ change_button.url }}"
              id="change_uuid_{{ uuid }}"
              class="stream-field__change-btn btn btn-square btn-sm btn-square--info"
-             data-toggle="tooltip"
+             data-xclass="bs-tooltip"
              data-placement="top"
              data-trigger="hover"
              data-html="true"
              title="{{ change_button.title }}">
-            <i class="fa {{ change_button.icon }}"></i>
+            <i class="{{ change_button.icon }}"></i>
           </a>
         {% endif %}
 
         <button type="button"
                 class="stream-field__delete-btn btn btn-square btn-sm btn-square--danger"
-                data-toggle="tooltip"
+                data-xclass="bs-tooltip"
                 data-placement="top"
                 data-trigger="hover"
                 data-html="true"
                 title="{{ delete_button.title }}">
-          <i class="fa {{ delete_button.icon }}"></i>
+          <i class="{{ delete_button.icon }}"></i>
         </button>
       </div>
     {% endblock %}
   </div>
 </div>
```

### Comparing `paper-streamfield-0.3.0/streamfield/templates/streamfield/admin/invalid_block.html` & `paper-streamfield-0.4.0/streamfield/templates/streamfield/admin/invalid_block.html`

 * *Files 1% similar despite different names*

```diff
@@ -16,11 +16,11 @@
     <button type="button"
             class="stream-field__delete-btn btn btn-square btn-sm btn-square--danger"
             data-toggle="tooltip"
             data-placement="top"
             data-trigger="hover"
             data-html="true"
             title="{{ delete_button.title }}">
-      <i class="fa {{ delete_button.icon }}"></i>
+      <i class="{{ delete_button.icon }}"></i>
     </button>
   </div>
 {% endblock %}
```

### Comparing `paper-streamfield-0.3.0/streamfield/templates/streamfield/admin/popup_response.html` & `paper-streamfield-0.4.0/streamfield/templates/streamfield/admin/popup_response.html`

 * *Files identical despite different names*

### Comparing `paper-streamfield-0.3.0/streamfield/templates/streamfield/admin/toolbar.html` & `paper-streamfield-0.4.0/streamfield/templates/streamfield/admin/toolbar.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load i18n %}
 
 <div class="stream-field__dropdown dropdown d-inline-block">
   <button class="btn-success btn dropdown-toggle" type="button" data-toggle="dropdown" aria-expanded="false">
-    <i class="fa fa-plus"></i>
+    <i class="bi-plus-lg"></i>
     {% trans "Create new block" %}
   </button>
   <ul class="stream-field__dropdown-menu dropdown-menu">
     {% for model in creatable_models %}
       <li role="presentation">
         <a class="stream-field__dropdown-item dropdown-item"
            href="{{ model.url }}"
@@ -17,15 +17,15 @@
       </li>
     {% endfor %}
   </ul>
 </div>
 
 <div class="stream-field__dropdown dropdown d-inline-block">
   <button class="btn-info btn dropdown-toggle" type="button" data-toggle="dropdown" aria-expanded="false">
-    <i class="fa fa-search"></i>
+    <i class="bi-search"></i>
     {% trans "Lookup block" %}
   </button>
   <ul class="stream-field__dropdown-menu dropdown-menu">
     {% for model in searchable_models %}
       <li role="presentation">
         <a class="stream-field__dropdown-item dropdown-item"
            href="{{ model.url }}"
```

### Comparing `paper-streamfield-0.3.0/streamfield/templatetags/streamfield.py` & `paper-streamfield-0.4.0/streamfield/templatetags/streamfield.py`

 * *Files identical despite different names*

