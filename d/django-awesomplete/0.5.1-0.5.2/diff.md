# Comparing `tmp/django-awesomplete-0.5.1.tar.gz` & `tmp/django-awesomplete-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-awesomplete-0.5.1.tar", last modified: Mon Jan  9 07:26:32 2023, max compression
+gzip compressed data, was "django-awesomplete-0.5.2.tar", last modified: Sun Apr 16 19:15:43 2023, max compression
```

## Comparing `django-awesomplete-0.5.1.tar` & `django-awesomplete-0.5.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 07:26:32.038138 django-awesomplete-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-01-09 07:26:22.000000 django-awesomplete-0.5.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-01-09 07:26:22.000000 django-awesomplete-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-01-09 07:26:22.000000 django-awesomplete-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-01-09 07:26:32.038138 django-awesomplete-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-01-09 07:26:22.000000 django-awesomplete-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 07:26:32.034138 django-awesomplete-0.5.1/awesomplete/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-09 07:26:22.000000 django-awesomplete-0.5.1/awesomplete/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 07:26:32.026138 django-awesomplete-0.5.1/awesomplete/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 07:26:32.026138 django-awesomplete-0.5.1/awesomplete/static/awesomplete/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 07:26:32.034138 django-awesomplete-0.5.1/awesomplete/static/awesomplete/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-01-09 07:26:22.000000 django-awesomplete-0.5.1/awesomplete/static/awesomplete/css/awesomplete.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 07:26:32.034138 django-awesomplete-0.5.1/awesomplete/static/awesomplete/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 07:26:32.034138 django-awesomplete-0.5.1/awesomplete/static/awesomplete/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-01-09 07:26:22.000000 django-awesomplete-0.5.1/awesomplete/static/awesomplete/js/vendor/awesomplete.js
--rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-01-09 07:26:22.000000 django-awesomplete-0.5.1/awesomplete/static/awesomplete/js/vendor/awesomplete.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    24637 2023-01-09 07:26:22.000000 django-awesomplete-0.5.1/awesomplete/static/awesomplete/js/vendor/awesomplete.min.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-01-09 07:26:22.000000 django-awesomplete-0.5.1/awesomplete/static/awesomplete/js/widget.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 07:26:32.030138 django-awesomplete-0.5.1/awesomplete/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 07:26:32.034138 django-awesomplete-0.5.1/awesomplete/templates/awesomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-01-09 07:26:22.000000 django-awesomplete-0.5.1/awesomplete/templates/awesomplete/widget_wrapper.html
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-01-09 07:26:22.000000 django-awesomplete-0.5.1/awesomplete/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 07:26:32.038138 django-awesomplete-0.5.1/django_awesomplete.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-01-09 07:26:31.000000 django-awesomplete-0.5.1/django_awesomplete.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-01-09 07:26:31.000000 django-awesomplete-0.5.1/django_awesomplete.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 07:26:31.000000 django-awesomplete-0.5.1/django_awesomplete.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 07:26:31.000000 django-awesomplete-0.5.1/django_awesomplete.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-09 07:26:31.000000 django-awesomplete-0.5.1/django_awesomplete.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-09 07:26:31.000000 django-awesomplete-0.5.1/django_awesomplete.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-01-09 07:26:32.042138 django-awesomplete-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-09 07:26:22.000000 django-awesomplete-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:15:43.122819 django-awesomplete-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-04-16 19:15:37.000000 django-awesomplete-0.5.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-16 19:15:37.000000 django-awesomplete-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-16 19:15:37.000000 django-awesomplete-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-04-16 19:15:43.122819 django-awesomplete-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-04-16 19:15:37.000000 django-awesomplete-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:15:43.118819 django-awesomplete-0.5.2/awesomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-16 19:15:37.000000 django-awesomplete-0.5.2/awesomplete/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:15:43.118819 django-awesomplete-0.5.2/awesomplete/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:15:43.118819 django-awesomplete-0.5.2/awesomplete/static/awesomplete/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:15:43.118819 django-awesomplete-0.5.2/awesomplete/static/awesomplete/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-16 19:15:37.000000 django-awesomplete-0.5.2/awesomplete/static/awesomplete/css/awesomplete.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:15:43.118819 django-awesomplete-0.5.2/awesomplete/static/awesomplete/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:15:43.118819 django-awesomplete-0.5.2/awesomplete/static/awesomplete/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-04-16 19:15:37.000000 django-awesomplete-0.5.2/awesomplete/static/awesomplete/js/vendor/awesomplete.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7599 2023-04-16 19:15:37.000000 django-awesomplete-0.5.2/awesomplete/static/awesomplete/js/vendor/awesomplete.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24637 2023-04-16 19:15:37.000000 django-awesomplete-0.5.2/awesomplete/static/awesomplete/js/vendor/awesomplete.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-04-16 19:15:37.000000 django-awesomplete-0.5.2/awesomplete/static/awesomplete/js/widget.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:15:43.118819 django-awesomplete-0.5.2/awesomplete/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:15:43.118819 django-awesomplete-0.5.2/awesomplete/templates/awesomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-16 19:15:37.000000 django-awesomplete-0.5.2/awesomplete/templates/awesomplete/widget_wrapper.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-16 19:15:37.000000 django-awesomplete-0.5.2/awesomplete/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:15:43.122819 django-awesomplete-0.5.2/django_awesomplete.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-04-16 19:15:43.000000 django-awesomplete-0.5.2/django_awesomplete.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-16 19:15:43.000000 django-awesomplete-0.5.2/django_awesomplete.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 19:15:43.000000 django-awesomplete-0.5.2/django_awesomplete.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 19:15:43.000000 django-awesomplete-0.5.2/django_awesomplete.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-16 19:15:43.000000 django-awesomplete-0.5.2/django_awesomplete.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 19:15:43.000000 django-awesomplete-0.5.2/django_awesomplete.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-16 19:15:43.122819 django-awesomplete-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-16 19:15:37.000000 django-awesomplete-0.5.2/setup.py
```

### Comparing `django-awesomplete-0.5.1/CHANGELOG.md` & `django-awesomplete-0.5.2/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Change Log
 
+## [0.5.2](https://github.com/dldevinc/django-awesomplete/tree/v0.5.2) - 2023-02-24
+
+### Features
+
+-   Test against Django 4.2.
+-   Add Wagtail compatibility.
+
 ## [0.5.1](https://github.com/dldevinc/django-awesomplete/tree/v0.5.1) - 2023-01-09
 
 ### Features
 
-- Add Python 3.11 support (no code changes were needed, but now we test this release).
+-   Add Python 3.11 support (no code changes were needed, but now we test this release).
 
 ## [0.5.0](https://github.com/dldevinc/django-awesomplete/tree/v0.5.0) - 2022-08-15
 
 ### Features
 
 -   Added support for Django 4.1.
```

### Comparing `django-awesomplete-0.5.1/LICENSE` & `django-awesomplete-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-awesomplete-0.5.1/PKG-INFO` & `django-awesomplete-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-awesomplete
-Version: 0.5.1
+Version: 0.5.2
 Summary: A django app that provides suggestions while you type into the field.
 Home-page: https://github.com/dldevinc/django-awesomplete
 Author: Mihail Mishakin
 Author-email: x896321475@gmail.com
 Maintainer: Mihail Mishakin
 Maintainer-email: x896321475@gmail.com
 License: BSD license
@@ -18,14 +18,15 @@
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `django-awesomplete-0.5.1/README.md` & `django-awesomplete-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `django-awesomplete-0.5.1/awesomplete/static/awesomplete/css/awesomplete.css` & `django-awesomplete-0.5.2/awesomplete/static/awesomplete/css/awesomplete.css`

 * *Files identical despite different names*

### Comparing `django-awesomplete-0.5.1/awesomplete/static/awesomplete/js/vendor/awesomplete.js` & `django-awesomplete-0.5.2/awesomplete/static/awesomplete/js/vendor/awesomplete.js`

 * *Files identical despite different names*

### Comparing `django-awesomplete-0.5.1/awesomplete/static/awesomplete/js/vendor/awesomplete.min.js` & `django-awesomplete-0.5.2/awesomplete/static/awesomplete/js/vendor/awesomplete.min.js`

 * *Files identical despite different names*

### Comparing `django-awesomplete-0.5.1/awesomplete/static/awesomplete/js/vendor/awesomplete.min.js.map` & `django-awesomplete-0.5.2/awesomplete/static/awesomplete/js/vendor/awesomplete.min.js.map`

 * *Files identical despite different names*

### Comparing `django-awesomplete-0.5.1/awesomplete/static/awesomplete/js/widget.js` & `django-awesomplete-0.5.2/awesomplete/static/awesomplete/js/widget.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -140,8 +140,8 @@
     $(document)
         .ready(function() {
             initWidgets($(document.body));
         })
         .on("formset:added", function(event, $row, formsetName) {
             initWidgets($row, formsetName);
         });
-})(django.jQuery);
+})((window.django && window.django.jQuery) || jQuery);
```

### Comparing `django-awesomplete-0.5.1/awesomplete/widgets.py` & `django-awesomplete-0.5.2/awesomplete/widgets.py`

 * *Files identical despite different names*

### Comparing `django-awesomplete-0.5.1/django_awesomplete.egg-info/PKG-INFO` & `django-awesomplete-0.5.2/django_awesomplete.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-awesomplete
-Version: 0.5.1
+Version: 0.5.2
 Summary: A django app that provides suggestions while you type into the field.
 Home-page: https://github.com/dldevinc/django-awesomplete
 Author: Mihail Mishakin
 Author-email: x896321475@gmail.com
 Maintainer: Mihail Mishakin
 Maintainer-email: x896321475@gmail.com
 License: BSD license
@@ -18,14 +18,15 @@
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `django-awesomplete-0.5.1/django_awesomplete.egg-info/SOURCES.txt` & `django-awesomplete-0.5.2/django_awesomplete.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-awesomplete-0.5.1/setup.cfg` & `django-awesomplete-0.5.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 	Framework :: Django :: 2.1
 	Framework :: Django :: 2.2
 	Framework :: Django :: 3.0
 	Framework :: Django :: 3.1
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
```

