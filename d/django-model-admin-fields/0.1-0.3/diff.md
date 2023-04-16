# Comparing `tmp/django_model_admin_fields-0.1.tar.gz` & `tmp/django_model_admin_fields-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_model_admin_fields-0.1.tar", last modified: Fri Oct 15 13:22:26 2021, max compression
+gzip compressed data, was "django_model_admin_fields-0.3.tar", last modified: Sun Apr 16 07:03:39 2023, max compression
```

## Comparing `django_model_admin_fields-0.1.tar` & `django_model_admin_fields-0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2021-10-15 13:22:26.385628 django_model_admin_fields-0.1/
--rw-rw-r--   0 bernd     (1000) bernd     (1000)    15891 2021-10-14 11:18:17.000000 django_model_admin_fields-0.1/LICENSE.md
--rw-rw-r--   0 bernd     (1000) bernd     (1000)     4562 2021-10-15 13:22:26.385628 django_model_admin_fields-0.1/PKG-INFO
--rw-rw-r--   0 bernd     (1000) bernd     (1000)     3645 2021-10-15 11:52:24.000000 django_model_admin_fields-0.1/README.md
--rw-rw-r--   0 bernd     (1000) bernd     (1000)      104 2021-10-14 10:42:04.000000 django_model_admin_fields-0.1/pyproject.toml
--rw-rw-r--   0 bernd     (1000) bernd     (1000)     1028 2021-10-15 13:22:26.389628 django_model_admin_fields-0.1/setup.cfg
-drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2021-10-15 13:22:26.385628 django_model_admin_fields-0.1/src/
-drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2021-10-15 13:22:26.385628 django_model_admin_fields-0.1/src/django_model_admin_fields/
--rw-r--r--   0 bernd     (1000) bernd     (1000)     4118 2021-10-15 13:11:00.000000 django_model_admin_fields-0.1/src/django_model_admin_fields/__init__.py
-drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2021-10-15 13:22:26.385628 django_model_admin_fields-0.1/src/django_model_admin_fields.egg-info/
--rw-rw-r--   0 bernd     (1000) bernd     (1000)     4562 2021-10-15 13:22:26.000000 django_model_admin_fields-0.1/src/django_model_admin_fields.egg-info/PKG-INFO
--rw-rw-r--   0 bernd     (1000) bernd     (1000)      351 2021-10-15 13:22:26.000000 django_model_admin_fields-0.1/src/django_model_admin_fields.egg-info/SOURCES.txt
--rw-rw-r--   0 bernd     (1000) bernd     (1000)        1 2021-10-15 13:22:26.000000 django_model_admin_fields-0.1/src/django_model_admin_fields.egg-info/dependency_links.txt
--rw-rw-r--   0 bernd     (1000) bernd     (1000)       55 2021-10-15 13:22:26.000000 django_model_admin_fields-0.1/src/django_model_admin_fields.egg-info/requires.txt
--rw-rw-r--   0 bernd     (1000) bernd     (1000)       26 2021-10-15 13:22:26.000000 django_model_admin_fields-0.1/src/django_model_admin_fields.egg-info/top_level.txt
+drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 07:03:39.104287 django_model_admin_fields-0.3/
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)    15891 2021-10-14 11:18:17.000000 django_model_admin_fields-0.3/LICENSE.md
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)     4486 2023-04-16 07:03:39.104287 django_model_admin_fields-0.3/PKG-INFO
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)     3653 2023-04-16 07:02:16.000000 django_model_admin_fields-0.3/README.md
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)      104 2021-10-14 10:42:04.000000 django_model_admin_fields-0.3/pyproject.toml
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)      974 2023-04-16 07:03:39.104287 django_model_admin_fields-0.3/setup.cfg
+drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 07:03:39.092287 django_model_admin_fields-0.3/src/
+drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 07:03:39.104287 django_model_admin_fields-0.3/src/django_model_admin_fields/
+-rw-r--r--   0 bernd     (1000) bernd     (1000)     4254 2023-04-16 06:52:29.000000 django_model_admin_fields-0.3/src/django_model_admin_fields/__init__.py
+drwxrwxr-x   0 bernd     (1000) bernd     (1000)        0 2023-04-16 07:03:39.104287 django_model_admin_fields-0.3/src/django_model_admin_fields.egg-info/
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)     4486 2023-04-16 07:03:39.000000 django_model_admin_fields-0.3/src/django_model_admin_fields.egg-info/PKG-INFO
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)      351 2023-04-16 07:03:39.000000 django_model_admin_fields-0.3/src/django_model_admin_fields.egg-info/SOURCES.txt
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)        1 2023-04-16 07:03:39.000000 django_model_admin_fields-0.3/src/django_model_admin_fields.egg-info/dependency_links.txt
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)       39 2023-04-16 07:03:39.000000 django_model_admin_fields-0.3/src/django_model_admin_fields.egg-info/requires.txt
+-rw-rw-r--   0 bernd     (1000) bernd     (1000)       26 2023-04-16 07:03:39.000000 django_model_admin_fields-0.3/src/django_model_admin_fields.egg-info/top_level.txt
```

### Comparing `django_model_admin_fields-0.1/LICENSE.md` & `django_model_admin_fields-0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_model_admin_fields-0.1/PKG-INFO` & `django_model_admin_fields-0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 Metadata-Version: 2.1
 Name: django_model_admin_fields
-Version: 0.1
+Version: 0.3
 Summary: Django abstract model that adds admin fields (created_on/by, laste_edited_on/by) to an existing model
 Home-page: https://github.com/bernd-wechner/django-model-admin-fields
 Author: Bernd Wechner
 Author-email: bwechner@yahoo.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/bernd-wechner/django-model-admin-fields/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Freely Distributable
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: System Administrators
-Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Django Model Admin Fields
 
-[Django](https://www.djangoproject.com/) is one of the most popular Python web frameworks today. Importantly it provides an [ORM](https://en.wikipedia.org/wiki/Object%E2%80%93relational_mapping) permitting us to define models as Python classes that Django maps to a databse representations for us. 
+[Django](https://www.djangoproject.com/) is one of the most popular Python web frameworks today. Importantly, it provides an [ORM](https://en.wikipedia.org/wiki/Object%E2%80%93relational_mapping) permitting us to define models as Python classes that Django maps to a database representations for us. 
 
-A very common, nearly ubiquitous desire/need I have is to keep some record against all database objects as to who created them, when and who last edited them and when. Very basic tracking fields. Given the ubiquity of the need it was best implemented as an abstrack model that my models derive from.
+A very common, nearly ubiquitous desire/need I have is to keep some record against all database objects as to who created them, when and who last edited them and when. Very basic tracking fields. Given the ubiquity of the need it was best implemented as an abstract model that my models derive from.
 
 The basic Django example of model:
 
 ```python
 from django.db import models
 
 class Person(models.Model):
@@ -63,29 +60,27 @@
     last_edited_on = models.DateTimeField('Time of Last Edit', editable=False, null=True)
     last_edited_on_tz = TimeZoneField('Time of Last Edit, Timezone', 
                                       default=settings.TIME_ZONE, editable=False)
 ```
 
 (a more precise description of course is in `__init__.py`)
 
-Importantly it also overrides the mmodel `save()` method to set those six fields before calling `super().save()` (i.e. the default save method) and thus these fields are automatically managed.
+Importantly it also overrides the model's `save()` method to set those six fields before calling `super().save()` (i.e. the default save method) and thus these fields are automatically managed.
 
 The [currently active](https://docs.djangoproject.com/en/3.2/topics/i18n/timezones/#selecting-the-current-time-zone) Django timezone is saved as well to support sensible human interpretation of the saved times (as Django's [DateTimeField](https://docs.djangoproject.com/en/3.2/ref/models/fields/#datetimefield)) is not timezone aware.
 
-To make use of that easier two properties are also added to the model: `created_on_local` and `last_edited_on_local` which are timezone aware versions of the naive `created_one` and `last_edited_on` fields.
+To make use of that easier, two properties are also added to the model: `created_on_local` and `last_edited_on_local` which are timezone aware versions of the naive `created_one` and `last_edited_on` fields.
 
 To illustrate use of the Person example above:
 
 ```Python
 person = Person()
 person.first_name = "John"
 person.last_name = "Smith"
 person.save
 
 print(f"{person.first_name} {person.last_name}")
 print(f"was created by {person.created_by} on {person.created_on_local}.")
 ```
 
-Of course to make use of local times, you need to activate the timezone that the creating user is in. To that you need to know it first. The Javascript library [jstz](https://github.com/iansinnott/jstz) is useful in that regard for detecting the users timezone and there's a great guide on [setting timezones](https://docs.djangoproject.com/en/3.2/topics/i18n/timezones/#selecting-the-current-time-zone) in Django inthe django documentation proper.
-
-
+Of course to make use of local times, you need to activate the timezone that the creating user is in. To do that you need to know it first. The JavaScript library [jstz](https://github.com/iansinnott/jstz) is useful in that regard for detecting the users timezone and there's a great guide on [setting timezones](https://docs.djangoproject.com/en/3.2/topics/i18n/timezones/#selecting-the-current-time-zone) in Django in the Django documentation proper.
```

### Comparing `django_model_admin_fields-0.1/README.md` & `django_model_admin_fields-0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Django Model Admin Fields
 
-[Django](https://www.djangoproject.com/) is one of the most popular Python web frameworks today. Importantly it provides an [ORM](https://en.wikipedia.org/wiki/Object%E2%80%93relational_mapping) permitting us to define models as Python classes that Django maps to a databse representations for us. 
+[Django](https://www.djangoproject.com/) is one of the most popular Python web frameworks today. Importantly, it provides an [ORM](https://en.wikipedia.org/wiki/Object%E2%80%93relational_mapping) permitting us to define models as Python classes that Django maps to a database representations for us. 
 
-A very common, nearly ubiquitous desire/need I have is to keep some record against all database objects as to who created them, when and who last edited them and when. Very basic tracking fields. Given the ubiquity of the need it was best implemented as an abstrack model that my models derive from.
+A very common, nearly ubiquitous desire/need I have is to keep some record against all database objects as to who created them, when and who last edited them and when. Very basic tracking fields. Given the ubiquity of the need it was best implemented as an abstract model that my models derive from.
 
 The basic Django example of model:
 
 ```python
 from django.db import models
 
 class Person(models.Model):
@@ -41,27 +41,27 @@
     last_edited_on = models.DateTimeField('Time of Last Edit', editable=False, null=True)
     last_edited_on_tz = TimeZoneField('Time of Last Edit, Timezone', 
                                       default=settings.TIME_ZONE, editable=False)
 ```
 
 (a more precise description of course is in `__init__.py`)
 
-Importantly it also overrides the mmodel `save()` method to set those six fields before calling `super().save()` (i.e. the default save method) and thus these fields are automatically managed.
+Importantly it also overrides the model's `save()` method to set those six fields before calling `super().save()` (i.e. the default save method) and thus these fields are automatically managed.
 
 The [currently active](https://docs.djangoproject.com/en/3.2/topics/i18n/timezones/#selecting-the-current-time-zone) Django timezone is saved as well to support sensible human interpretation of the saved times (as Django's [DateTimeField](https://docs.djangoproject.com/en/3.2/ref/models/fields/#datetimefield)) is not timezone aware.
 
-To make use of that easier two properties are also added to the model: `created_on_local` and `last_edited_on_local` which are timezone aware versions of the naive `created_one` and `last_edited_on` fields.
+To make use of that easier, two properties are also added to the model: `created_on_local` and `last_edited_on_local` which are timezone aware versions of the naive `created_one` and `last_edited_on` fields.
 
 To illustrate use of the Person example above:
 
 ```Python
 person = Person()
 person.first_name = "John"
 person.last_name = "Smith"
 person.save
 
 print(f"{person.first_name} {person.last_name}")
 print(f"was created by {person.created_by} on {person.created_on_local}.")
 ```
 
-Of course to make use of local times, you need to activate the timezone that the creating user is in. To that you need to know it first. The Javascript library [jstz](https://github.com/iansinnott/jstz) is useful in that regard for detecting the users timezone and there's a great guide on [setting timezones](https://docs.djangoproject.com/en/3.2/topics/i18n/timezones/#selecting-the-current-time-zone) in Django inthe django documentation proper.
+Of course to make use of local times, you need to activate the timezone that the creating user is in. To do that you need to know it first. The JavaScript library [jstz](https://github.com/iansinnott/jstz) is useful in that regard for detecting the users timezone and there's a great guide on [setting timezones](https://docs.djangoproject.com/en/3.2/topics/i18n/timezones/#selecting-the-current-time-zone) in Django in the Django documentation proper.
```

### Comparing `django_model_admin_fields-0.1/setup.cfg` & `django_model_admin_fields-0.3/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 [metadata]
 name = django_model_admin_fields
-version = 0.1
+version = 0.3
 author = Bernd Wechner
 author_email = bwechner@yahoo.com
 description = Django abstract model that adds admin fields (created_on/by, laste_edited_on/by) to an existing model
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/bernd-wechner/django-model-admin-fields
 project_urls = 
 	Bug Tracker = https://github.com/bernd-wechner/django-model-admin-fields/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Freely Distributable
 	Operating System :: OS Independent
 	Development Status :: 4 - Beta
-	Framework :: Django :: 3.2
+	Framework :: Django :: 4.0
 	Intended Audience :: System Administrators
-	Operating System :: OS Independent
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 install_requires = 
-	django-currentuser >= 0.5.3
-	django-timezone-field >= 4.2.1
+	django-crequest
+	django-bitfield >= 2.0.1
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 
 [options.packages.find]
 where = src
```

### Comparing `django_model_admin_fields-0.1/src/django_model_admin_fields/__init__.py` & `django_model_admin_fields-0.3/src/django_model_admin_fields/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 '''
 Created on 8 Mar.,2018
 
 @author: Bernd Wechner
-@status: Beta - works and is in use on a dedicated project. 
+@status: Beta - works and is in use on a dedicated project.
+
+In your Dango settings.py make sure to include 'crequest.middleware.CrequestMiddleware' in the MIDDDLEWARE list.
 
 Provides a class, AdminModel which is an abstract Django model that a model can derive from to inherit
 some admin fields and a save override that keeps them up to date. Intended for recording some user and time
 info against every record saved.
 
 Specifically it adds to any model that derives from it 6 new fields:
 
     created_by
     created_on
     created_on_tz
-    
+
     last_edited_by
     last_edited_on
     last_edited_on_tz
 
 That is, the name of the user who created the object and who last saved (edited) it,
-and the time it was created and last saved (edited). Timezone fields are maintained 
+and the time it was created and last saved (edited). Timezone fields are maintained
 as well as a convenience for timezone aware sites.
 
 The timezone saved is the one active in Django at the time. Django has solid support
-for presenting times that make sense to users across the globe, by activating the 
+for presenting times that make sense to users across the globe, by activating the
 timezone a given user is in (provided the site asks for that and activates the
-timezone appropriately). 
+timezone appropriately).
 '''
 import pytz
 
-from django_currentuser.middleware import get_current_user
 from timezone_field import TimeZoneField
 
 from django.db import models
 from django.utils import timezone
 from django.contrib.auth.models import User
 from django.conf import settings
 from django.utils.timezone import get_current_timezone
 
+from crequest.middleware import CrequestMiddleware
+
 UTC = pytz.timezone('UTC')
 
 
 def safe_tz(tz):
     '''A one-line that converts TZ string to a TimeZone object if needed'''
     return pytz.timezone(tz) if isinstance(tz, str) else tz
 
@@ -66,15 +69,16 @@
     __bypass_admin__ = False
 
     def update_admin_fields(self):
         '''
         Update the CoGs admin fields on an object (whenever it is saved).
         '''
         now = timezone.now()
-        usr = get_current_user()
+        rqt = CrequestMiddleware.get_request()
+        usr = rqt.user
 
         if hasattr(self, "last_edited_by"):
             self.last_edited_by = usr
 
         if hasattr(self, "last_edited_on"):
             self.last_edited_on = now
```

### Comparing `django_model_admin_fields-0.1/src/django_model_admin_fields.egg-info/PKG-INFO` & `django_model_admin_fields-0.3/src/django_model_admin_fields.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 Metadata-Version: 2.1
 Name: django-model-admin-fields
-Version: 0.1
+Version: 0.3
 Summary: Django abstract model that adds admin fields (created_on/by, laste_edited_on/by) to an existing model
 Home-page: https://github.com/bernd-wechner/django-model-admin-fields
 Author: Bernd Wechner
 Author-email: bwechner@yahoo.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/bernd-wechner/django-model-admin-fields/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Freely Distributable
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: System Administrators
-Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Django Model Admin Fields
 
-[Django](https://www.djangoproject.com/) is one of the most popular Python web frameworks today. Importantly it provides an [ORM](https://en.wikipedia.org/wiki/Object%E2%80%93relational_mapping) permitting us to define models as Python classes that Django maps to a databse representations for us. 
+[Django](https://www.djangoproject.com/) is one of the most popular Python web frameworks today. Importantly, it provides an [ORM](https://en.wikipedia.org/wiki/Object%E2%80%93relational_mapping) permitting us to define models as Python classes that Django maps to a database representations for us. 
 
-A very common, nearly ubiquitous desire/need I have is to keep some record against all database objects as to who created them, when and who last edited them and when. Very basic tracking fields. Given the ubiquity of the need it was best implemented as an abstrack model that my models derive from.
+A very common, nearly ubiquitous desire/need I have is to keep some record against all database objects as to who created them, when and who last edited them and when. Very basic tracking fields. Given the ubiquity of the need it was best implemented as an abstract model that my models derive from.
 
 The basic Django example of model:
 
 ```python
 from django.db import models
 
 class Person(models.Model):
@@ -63,29 +60,27 @@
     last_edited_on = models.DateTimeField('Time of Last Edit', editable=False, null=True)
     last_edited_on_tz = TimeZoneField('Time of Last Edit, Timezone', 
                                       default=settings.TIME_ZONE, editable=False)
 ```
 
 (a more precise description of course is in `__init__.py`)
 
-Importantly it also overrides the mmodel `save()` method to set those six fields before calling `super().save()` (i.e. the default save method) and thus these fields are automatically managed.
+Importantly it also overrides the model's `save()` method to set those six fields before calling `super().save()` (i.e. the default save method) and thus these fields are automatically managed.
 
 The [currently active](https://docs.djangoproject.com/en/3.2/topics/i18n/timezones/#selecting-the-current-time-zone) Django timezone is saved as well to support sensible human interpretation of the saved times (as Django's [DateTimeField](https://docs.djangoproject.com/en/3.2/ref/models/fields/#datetimefield)) is not timezone aware.
 
-To make use of that easier two properties are also added to the model: `created_on_local` and `last_edited_on_local` which are timezone aware versions of the naive `created_one` and `last_edited_on` fields.
+To make use of that easier, two properties are also added to the model: `created_on_local` and `last_edited_on_local` which are timezone aware versions of the naive `created_one` and `last_edited_on` fields.
 
 To illustrate use of the Person example above:
 
 ```Python
 person = Person()
 person.first_name = "John"
 person.last_name = "Smith"
 person.save
 
 print(f"{person.first_name} {person.last_name}")
 print(f"was created by {person.created_by} on {person.created_on_local}.")
 ```
 
-Of course to make use of local times, you need to activate the timezone that the creating user is in. To that you need to know it first. The Javascript library [jstz](https://github.com/iansinnott/jstz) is useful in that regard for detecting the users timezone and there's a great guide on [setting timezones](https://docs.djangoproject.com/en/3.2/topics/i18n/timezones/#selecting-the-current-time-zone) in Django inthe django documentation proper.
-
-
+Of course to make use of local times, you need to activate the timezone that the creating user is in. To do that you need to know it first. The JavaScript library [jstz](https://github.com/iansinnott/jstz) is useful in that regard for detecting the users timezone and there's a great guide on [setting timezones](https://docs.djangoproject.com/en/3.2/topics/i18n/timezones/#selecting-the-current-time-zone) in Django in the Django documentation proper.
```

