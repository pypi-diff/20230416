# Comparing `tmp/django_model_privacy_mixin-0.3.tar.gz` & `tmp/django_model_privacy_mixin-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_model_privacy_mixin-0.3.tar", last modified: Sat Apr 15 03:04:01 2023, max compression
+gzip compressed data, was "django_model_privacy_mixin-0.4.tar", last modified: Sun Apr 16 07:02:43 2023, max compression
```

## Comparing `django_model_privacy_mixin-0.3.tar` & `django_model_privacy_mixin-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-15 03:04:01.527549 django_model_privacy_mixin-0.3/
--rw-rw-r--   0 bernd     (1000) bernd     (1000)    15891 2021-10-14 11:18:17.000000 django_model_privacy_mixin-0.3/LICENSE.md
--rw-rw-r--   0 bernd     (1000) bernd     (1000)    14485 2023-04-15 03:04:01.527549 django_model_privacy_mixin-0.3/PKG-INFO
--rw-rw-r--   0 bernd     (1000) bernd     (1000)    13691 2023-03-13 10:24:23.000000 django_model_privacy_mixin-0.3/README.md
--rw-rw-r--   0 bernd     (1000) bernd     (1000)      104 2021-10-14 10:42:04.000000 django_model_privacy_mixin-0.3/pyproject.toml
--rw-rw-r--   0 bernd     (1000) bernd     (1000)      935 2023-04-15 03:04:01.527549 django_model_privacy_mixin-0.3/setup.cfg
-drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-15 03:04:01.523549 django_model_privacy_mixin-0.3/src/
-drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-15 03:04:01.523549 django_model_privacy_mixin-0.3/src/django_model_privacy_mixin/
--rw-r--r--   0 bernd     (1000) bernd     (1000)    12480 2023-04-15 02:57:57.000000 django_model_privacy_mixin-0.3/src/django_model_privacy_mixin/__init__.py
-drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-15 03:04:01.527549 django_model_privacy_mixin-0.3/src/django_model_privacy_mixin.egg-info/
--rw-rw-r--   0 bernd     (1000) bernd     (1000)    14485 2023-04-15 03:04:01.000000 django_model_privacy_mixin-0.3/src/django_model_privacy_mixin.egg-info/PKG-INFO
--rw-rw-r--   0 bernd     (1000) bernd     (1000)      357 2023-04-15 03:04:01.000000 django_model_privacy_mixin-0.3/src/django_model_privacy_mixin.egg-info/SOURCES.txt
--rw-rw-r--   0 bernd     (1000) bernd     (1000)        1 2023-04-15 03:04:01.000000 django_model_privacy_mixin-0.3/src/django_model_privacy_mixin.egg-info/dependency_links.txt
--rw-rw-r--   0 bernd     (1000) bernd     (1000)       39 2023-04-15 03:04:01.000000 django_model_privacy_mixin-0.3/src/django_model_privacy_mixin.egg-info/requires.txt
--rw-rw-r--   0 bernd     (1000) bernd     (1000)       27 2023-04-15 03:04:01.000000 django_model_privacy_mixin-0.3/src/django_model_privacy_mixin.egg-info/top_level.txt
+drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 07:02:43.416422 django_model_privacy_mixin-0.4/
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)    15891 2021-10-14 11:18:17.000000 django_model_privacy_mixin-0.4/LICENSE.md
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)    14485 2023-04-16 07:02:43.416422 django_model_privacy_mixin-0.4/PKG-INFO
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)    13691 2023-03-13 10:24:23.000000 django_model_privacy_mixin-0.4/README.md
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)      104 2021-10-14 10:42:04.000000 django_model_privacy_mixin-0.4/pyproject.toml
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)      935 2023-04-16 07:02:43.416422 django_model_privacy_mixin-0.4/setup.cfg
+drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 07:02:43.416422 django_model_privacy_mixin-0.4/src/
+drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 07:02:43.416422 django_model_privacy_mixin-0.4/src/django_model_privacy_mixin/
+-rw-r--r--   0 bernd     (1000) bernd     (1000)    12481 2023-04-16 06:39:47.000000 django_model_privacy_mixin-0.4/src/django_model_privacy_mixin/__init__.py
+drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 07:02:43.416422 django_model_privacy_mixin-0.4/src/django_model_privacy_mixin.egg-info/
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)    14485 2023-04-16 07:02:43.000000 django_model_privacy_mixin-0.4/src/django_model_privacy_mixin.egg-info/PKG-INFO
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)      357 2023-04-16 07:02:43.000000 django_model_privacy_mixin-0.4/src/django_model_privacy_mixin.egg-info/SOURCES.txt
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)        1 2023-04-16 07:02:43.000000 django_model_privacy_mixin-0.4/src/django_model_privacy_mixin.egg-info/dependency_links.txt
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)       39 2023-04-16 07:02:43.000000 django_model_privacy_mixin-0.4/src/django_model_privacy_mixin.egg-info/requires.txt
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)       27 2023-04-16 07:02:43.000000 django_model_privacy_mixin-0.4/src/django_model_privacy_mixin.egg-info/top_level.txt
```

### Comparing `django_model_privacy_mixin-0.3/LICENSE.md` & `django_model_privacy_mixin-0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_model_privacy_mixin-0.3/PKG-INFO` & `django_model_privacy_mixin-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_model_privacy_mixin
-Version: 0.3
+Version: 0.4
 Summary: Django Model MixIn providing flexible field privacy control
 Home-page: https://github.com/bernd-wechner/django-model-privacy-mixin
 Author: Bernd Wechner
 Author-email: bwechner@yahoo.com
 Project-URL: Bug Tracker, https://github.com/bernd-wechner/django-model-privacy-mixin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Freely Distributable
```

### Comparing `django_model_privacy_mixin-0.3/README.md` & `django_model_privacy_mixin-0.4/README.md`

 * *Files identical despite different names*

### Comparing `django_model_privacy_mixin-0.3/setup.cfg` & `django_model_privacy_mixin-0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_model_privacy_mixin
-version = 0.3
+version = 0.4
 author = Bernd Wechner
 author_email = bwechner@yahoo.com
 description = Django Model MixIn providing flexible field privacy control
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/bernd-wechner/django-model-privacy-mixin
 project_urls =
```

### Comparing `django_model_privacy_mixin-0.3/src/django_model_privacy_mixin/__init__.py` & `django_model_privacy_mixin-0.4/src/django_model_privacy_mixin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''
 Created on 8 Mar.,2018
 
 @author: Bernd Wechner
 @status: Beta - works and is in use on a dedicated project.
 
-In your Dango settings.py make sure to cilude 'crequest.middleware.CrequestMiddleware' in the MIDDDLEWARE list.
+In your Dango settings.py make sure to include 'crequest.middleware.CrequestMiddleware' in the MIDDDLEWARE list.
 
 Provides one class PrivacyMixIn which adds Privacy support for model fields in a Django model.
 '''
 
 from django.core.exceptions import PermissionDenied
 from django.forms.models import fields_for_model
 from django.utils.safestring import mark_safe
```

### Comparing `django_model_privacy_mixin-0.3/src/django_model_privacy_mixin.egg-info/PKG-INFO` & `django_model_privacy_mixin-0.4/src/django_model_privacy_mixin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-model-privacy-mixin
-Version: 0.3
+Version: 0.4
 Summary: Django Model MixIn providing flexible field privacy control
 Home-page: https://github.com/bernd-wechner/django-model-privacy-mixin
 Author: Bernd Wechner
 Author-email: bwechner@yahoo.com
 Project-URL: Bug Tracker, https://github.com/bernd-wechner/django-model-privacy-mixin/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Freely Distributable
```

