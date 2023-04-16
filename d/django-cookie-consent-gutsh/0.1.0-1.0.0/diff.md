# Comparing `tmp/django-cookie_consent_gutsh-0.1.0.tar.gz` & `tmp/django-cookie_consent_gutsh-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-cookie_consent_gutsh-0.1.0.tar", last modified: Sun Apr 16 10:55:31 2023, max compression
+gzip compressed data, was "django-cookie_consent_gutsh-1.0.0.tar", last modified: Sun Apr 16 11:05:54 2023, max compression
```

## Comparing `django-cookie_consent_gutsh-0.1.0.tar` & `django-cookie_consent_gutsh-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 10:55:31.489233 django-cookie_consent_gutsh-0.1.0/
--rw-r--r--   0 gutsh      (501) staff       (20)     1074 2023-04-15 14:55:37.000000 django-cookie_consent_gutsh-0.1.0/LICENSE
--rw-r--r--   0 gutsh      (501) staff       (20)      147 2023-04-14 11:24:09.000000 django-cookie_consent_gutsh-0.1.0/MANIFEST.in
--rw-r--r--   0 gutsh      (501) staff       (20)     1499 2023-04-16 10:55:31.489437 django-cookie_consent_gutsh-0.1.0/PKG-INFO
--rw-r--r--   0 gutsh      (501) staff       (20)      905 2023-04-16 10:53:45.000000 django-cookie_consent_gutsh-0.1.0/README.md
-drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 10:55:31.478237 django-cookie_consent_gutsh-0.1.0/cookie_consent/
--rw-r--r--   0 gutsh      (501) staff       (20)        0 2023-04-14 08:39:47.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/__init__.py
--rw-r--r--   0 gutsh      (501) staff       (20)      108 2023-04-15 13:09:46.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/admin.py
--rw-r--r--   0 gutsh      (501) staff       (20)      159 2023-04-14 08:39:47.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/apps.py
-drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 10:55:31.479420 django-cookie_consent_gutsh-0.1.0/cookie_consent/migrations/
--rw-r--r--   0 gutsh      (501) staff       (20)      732 2023-04-15 12:52:39.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/migrations/0001_initial.py
--rw-r--r--   0 gutsh      (501) staff       (20)        0 2023-04-14 08:39:47.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/migrations/__init__.py
--rw-r--r--   0 gutsh      (501) staff       (20)      327 2023-04-15 13:30:14.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/models.py
-drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 10:55:31.468588 django-cookie_consent_gutsh-0.1.0/cookie_consent/static/
-drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 10:55:31.468772 django-cookie_consent_gutsh-0.1.0/cookie_consent/static/cookie_consent/
-drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 10:55:31.482829 django-cookie_consent_gutsh-0.1.0/cookie_consent/static/cookie_consent/css/
--rw-r--r--   0 gutsh      (501) staff       (20)      149 2023-04-15 15:22:56.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/static/cookie_consent/css/README.md
--rw-r--r--   0 gutsh      (501) staff       (20)      462 2023-04-14 09:46:39.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/static/cookie_consent/css/index.css
--rw-r--r--   0 gutsh      (501) staff       (20)      245 2023-04-14 09:46:39.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/static/cookie_consent/css/index.css.map
-drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 10:55:31.469066 django-cookie_consent_gutsh-0.1.0/cookie_consent/templates/
-drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 10:55:31.469199 django-cookie_consent_gutsh-0.1.0/cookie_consent/templates/cookie_consent/
-drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 10:55:31.484656 django-cookie_consent_gutsh-0.1.0/cookie_consent/templates/cookie_consent/includes/
--rw-r--r--   0 gutsh      (501) staff       (20)      704 2023-04-15 13:27:04.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/templates/cookie_consent/includes/consent.html
--rw-r--r--   0 gutsh      (501) staff       (20)       60 2023-04-14 08:39:47.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/tests.py
--rw-r--r--   0 gutsh      (501) staff       (20)      180 2023-04-15 12:36:12.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/urls.py
--rw-r--r--   0 gutsh      (501) staff       (20)     1249 2023-04-15 13:29:26.000000 django-cookie_consent_gutsh-0.1.0/cookie_consent/views.py
-drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 10:55:31.488697 django-cookie_consent_gutsh-0.1.0/django_cookie_consent_gutsh.egg-info/
--rw-r--r--   0 gutsh      (501) staff       (20)     1499 2023-04-16 10:55:31.000000 django-cookie_consent_gutsh-0.1.0/django_cookie_consent_gutsh.egg-info/PKG-INFO
--rw-r--r--   0 gutsh      (501) staff       (20)      786 2023-04-16 10:55:31.000000 django-cookie_consent_gutsh-0.1.0/django_cookie_consent_gutsh.egg-info/SOURCES.txt
--rw-r--r--   0 gutsh      (501) staff       (20)        1 2023-04-16 10:55:31.000000 django-cookie_consent_gutsh-0.1.0/django_cookie_consent_gutsh.egg-info/dependency_links.txt
--rw-r--r--   0 gutsh      (501) staff       (20)       12 2023-04-16 10:55:31.000000 django-cookie_consent_gutsh-0.1.0/django_cookie_consent_gutsh.egg-info/requires.txt
--rw-r--r--   0 gutsh      (501) staff       (20)       15 2023-04-16 10:55:31.000000 django-cookie_consent_gutsh-0.1.0/django_cookie_consent_gutsh.egg-info/top_level.txt
--rw-r--r--   0 gutsh      (501) staff       (20)      547 2023-04-15 17:36:38.000000 django-cookie_consent_gutsh-0.1.0/pyproject.toml
--rw-r--r--   0 gutsh      (501) staff       (20)      937 2023-04-16 10:55:31.490196 django-cookie_consent_gutsh-0.1.0/setup.cfg
--rw-r--r--   0 gutsh      (501) staff       (20)       38 2023-04-14 11:20:52.000000 django-cookie_consent_gutsh-0.1.0/setup.py
+drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 11:05:54.459646 django-cookie_consent_gutsh-1.0.0/
+-rw-r--r--   0 gutsh      (501) staff       (20)     1074 2023-04-15 14:55:37.000000 django-cookie_consent_gutsh-1.0.0/LICENSE
+-rw-r--r--   0 gutsh      (501) staff       (20)      147 2023-04-14 11:24:09.000000 django-cookie_consent_gutsh-1.0.0/MANIFEST.in
+-rw-r--r--   0 gutsh      (501) staff       (20)     1707 2023-04-16 11:05:54.459852 django-cookie_consent_gutsh-1.0.0/PKG-INFO
+-rw-r--r--   0 gutsh      (501) staff       (20)     1113 2023-04-16 11:03:35.000000 django-cookie_consent_gutsh-1.0.0/README.md
+drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 11:05:54.449990 django-cookie_consent_gutsh-1.0.0/cookie_consent/
+-rw-r--r--   0 gutsh      (501) staff       (20)        0 2023-04-14 08:39:47.000000 django-cookie_consent_gutsh-1.0.0/cookie_consent/__init__.py
+-rw-r--r--   0 gutsh      (501) staff       (20)      108 2023-04-15 13:09:46.000000 django-cookie_consent_gutsh-1.0.0/cookie_consent/admin.py
+-rw-r--r--   0 gutsh      (501) staff       (20)      159 2023-04-14 08:39:47.000000 django-cookie_consent_gutsh-1.0.0/cookie_consent/apps.py
+drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 11:05:54.451789 django-cookie_consent_gutsh-1.0.0/cookie_consent/migrations/
+-rw-r--r--   0 gutsh      (501) staff       (20)      732 2023-04-15 12:52:39.000000 django-cookie_consent_gutsh-1.0.0/cookie_consent/migrations/0001_initial.py
+-rw-r--r--   0 gutsh      (501) staff       (20)        0 2023-04-14 08:39:47.000000 django-cookie_consent_gutsh-1.0.0/cookie_consent/migrations/__init__.py
+-rw-r--r--   0 gutsh      (501) staff       (20)      327 2023-04-15 13:30:14.000000 django-cookie_consent_gutsh-1.0.0/cookie_consent/models.py
+drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 11:05:54.441658 django-cookie_consent_gutsh-1.0.0/cookie_consent/static/
+drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 11:05:54.441785 django-cookie_consent_gutsh-1.0.0/cookie_consent/static/cookie_consent/
+drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 11:05:54.454843 django-cookie_consent_gutsh-1.0.0/cookie_consent/static/cookie_consent/css/
+-rw-r--r--   0 gutsh      (501) staff       (20)      149 2023-04-15 15:22:56.000000 django-cookie_consent_gutsh-1.0.0/cookie_consent/static/cookie_consent/css/README.md
+-rw-r--r--   0 gutsh      (501) staff       (20)      462 2023-04-14 09:46:39.000000 django-cookie_consent_gutsh-1.0.0/cookie_consent/static/cookie_consent/css/index.css
+-rw-r--r--   0 gutsh      (501) staff       (20)      245 2023-04-14 09:46:39.000000 django-cookie_consent_gutsh-1.0.0/cookie_consent/static/cookie_consent/css/index.css.map
+drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 11:05:54.442137 django-cookie_consent_gutsh-1.0.0/cookie_consent/templates/
+drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 11:05:54.442333 django-cookie_consent_gutsh-1.0.0/cookie_consent/templates/cookie_consent/
+drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 11:05:54.455403 django-cookie_consent_gutsh-1.0.0/cookie_consent/templates/cookie_consent/includes/
+-rw-r--r--   0 gutsh      (501) staff       (20)      704 2023-04-15 13:27:04.000000 django-cookie_consent_gutsh-1.0.0/cookie_consent/templates/cookie_consent/includes/consent.html
+-rw-r--r--   0 gutsh      (501) staff       (20)       60 2023-04-14 08:39:47.000000 django-cookie_consent_gutsh-1.0.0/cookie_consent/tests.py
+-rw-r--r--   0 gutsh      (501) staff       (20)      180 2023-04-15 12:36:12.000000 django-cookie_consent_gutsh-1.0.0/cookie_consent/urls.py
+-rw-r--r--   0 gutsh      (501) staff       (20)     1249 2023-04-15 13:29:26.000000 django-cookie_consent_gutsh-1.0.0/cookie_consent/views.py
+drwxr-xr-x   0 gutsh      (501) staff       (20)        0 2023-04-16 11:05:54.458980 django-cookie_consent_gutsh-1.0.0/django_cookie_consent_gutsh.egg-info/
+-rw-r--r--   0 gutsh      (501) staff       (20)     1707 2023-04-16 11:05:54.000000 django-cookie_consent_gutsh-1.0.0/django_cookie_consent_gutsh.egg-info/PKG-INFO
+-rw-r--r--   0 gutsh      (501) staff       (20)      786 2023-04-16 11:05:54.000000 django-cookie_consent_gutsh-1.0.0/django_cookie_consent_gutsh.egg-info/SOURCES.txt
+-rw-r--r--   0 gutsh      (501) staff       (20)        1 2023-04-16 11:05:54.000000 django-cookie_consent_gutsh-1.0.0/django_cookie_consent_gutsh.egg-info/dependency_links.txt
+-rw-r--r--   0 gutsh      (501) staff       (20)       12 2023-04-16 11:05:54.000000 django-cookie_consent_gutsh-1.0.0/django_cookie_consent_gutsh.egg-info/requires.txt
+-rw-r--r--   0 gutsh      (501) staff       (20)       15 2023-04-16 11:05:54.000000 django-cookie_consent_gutsh-1.0.0/django_cookie_consent_gutsh.egg-info/top_level.txt
+-rw-r--r--   0 gutsh      (501) staff       (20)      547 2023-04-16 11:03:56.000000 django-cookie_consent_gutsh-1.0.0/pyproject.toml
+-rw-r--r--   0 gutsh      (501) staff       (20)      937 2023-04-16 11:05:54.460769 django-cookie_consent_gutsh-1.0.0/setup.cfg
+-rw-r--r--   0 gutsh      (501) staff       (20)       38 2023-04-14 11:20:52.000000 django-cookie_consent_gutsh-1.0.0/setup.py
```

### Comparing `django-cookie_consent_gutsh-0.1.0/LICENSE` & `django-cookie_consent_gutsh-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-cookie_consent_gutsh-0.1.0/PKG-INFO` & `django-cookie_consent_gutsh-1.0.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: django-cookie_consent_gutsh
-Version: 0.1.0
-Summary: Cookie consent component for any Django web-site
-Home-page: https://www.barskiylab.com/
-Author: Artem Barskii
-Author-email: Artem Barskii <artemiy.barskiy@gmail.com>
-License: MIT  # Will be changed later perhaps
-Project-URL: Homepage, https://github.com/gutsh/django-cookie-consent
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Cookie consent
 
 Cookie consent is a Django app to show consent component for web-cookies.
 
 ## Quick start
 
 1. Add "cookie\_consent" to your `INSTALLED_APPS` setting like this:
@@ -39,8 +23,11 @@
   ```
   {% block cookie_consent %}
     <link rel="stylesheet" href="{% static 'cookie_consent/css/index.css' %}">
     {% include 'cookie_consent/includes/consent.html' %}
     <script type="module" src="/assets/js/toolkit/cookie_consent.js"></script>
   {% endblock %}
   ```
+
+  Don't forget to serve that script and css files! You can find them in distribution, css is already fine (as long as you run `collectstatic` command), and javascript is available under `assets/js/tookit`.
+
 5. Start the development server and visit necessary pages.
```

#### html2text {}

```diff
@@ -1,18 +1,13 @@
-Metadata-Version: 2.1 Name: django-cookie_consent_gutsh Version: 0.1.0 Summary:
-Cookie consent component for any Django web-site Home-page: https://
-www.barskiylab.com/ Author: Artem Barskii Author-email: Artem Barskii
-barskiy@gmail.com> License: MIT # Will be changed later perhaps Project-URL:
-Homepage, https://github.com/gutsh/django-cookie-consent Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
-Description-Content-Type: text/markdown License-File: LICENSE # Cookie consent
-Cookie consent is a Django app to show consent component for web-cookies. ##
-Quick start 1. Add "cookie\_consent" to your `INSTALLED_APPS` setting like
-this: ``` INSTALLED_APPS = [ "cookie_consent", ..., ] ``` 2. Include the
-cookie\_consent URLconf in your project urls.py like this: ``` path
+# Cookie consent Cookie consent is a Django app to show consent component for
+web-cookies. ## Quick start 1. Add "cookie\_consent" to your `INSTALLED_APPS`
+setting like this: ``` INSTALLED_APPS = [ "cookie_consent", ..., ] ``` 2.
+Include the cookie\_consent URLconf in your project urls.py like this: ``` path
 ("cookie_consent/", include("cookie_consent.urls")), ``` 3. Run `python
 manage.py migrate` to create the models. 4. Include consent template in your
 web-site templates. For example, I've included that text in my base template:
 ``` {% block cookie_consent %}
  {% include 'cookie_consent/includes/consent.html' %}
- {% endblock %} ``` 5. Start the development server and visit necessary pages.
+ {% endblock %} ``` Don't forget to serve that script and css files! You can
+find them in distribution, css is already fine (as long as you run
+`collectstatic` command), and javascript is available under `assets/js/tookit`.
+5. Start the development server and visit necessary pages.
```

### Comparing `django-cookie_consent_gutsh-0.1.0/cookie_consent/migrations/0001_initial.py` & `django-cookie_consent_gutsh-1.0.0/cookie_consent/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-cookie_consent_gutsh-0.1.0/cookie_consent/templates/cookie_consent/includes/consent.html` & `django-cookie_consent_gutsh-1.0.0/cookie_consent/templates/cookie_consent/includes/consent.html`

 * *Files identical despite different names*

### Comparing `django-cookie_consent_gutsh-0.1.0/cookie_consent/views.py` & `django-cookie_consent_gutsh-1.0.0/cookie_consent/views.py`

 * *Files identical despite different names*

### Comparing `django-cookie_consent_gutsh-0.1.0/django_cookie_consent_gutsh.egg-info/PKG-INFO` & `django-cookie_consent_gutsh-1.0.0/django_cookie_consent_gutsh.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cookie-consent-gutsh
-Version: 0.1.0
+Version: 1.0.0
 Summary: Cookie consent component for any Django web-site
 Home-page: https://www.barskiylab.com/
 Author: Artem Barskii
 Author-email: Artem Barskii <artemiy.barskiy@gmail.com>
 License: MIT  # Will be changed later perhaps
 Project-URL: Homepage, https://github.com/gutsh/django-cookie-consent
 Classifier: Programming Language :: Python :: 3
@@ -39,8 +39,11 @@
   ```
   {% block cookie_consent %}
     <link rel="stylesheet" href="{% static 'cookie_consent/css/index.css' %}">
     {% include 'cookie_consent/includes/consent.html' %}
     <script type="module" src="/assets/js/toolkit/cookie_consent.js"></script>
   {% endblock %}
   ```
+
+  Don't forget to serve that script and css files! You can find them in distribution, css is already fine (as long as you run `collectstatic` command), and javascript is available under `assets/js/tookit`.
+
 5. Start the development server and visit necessary pages.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-cookie-consent-gutsh Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: django-cookie-consent-gutsh Version: 1.0.0 Summary:
 Cookie consent component for any Django web-site Home-page: https://
 www.barskiylab.com/ Author: Artem Barskii Author-email: Artem Barskii
 barskiy@gmail.com> License: MIT # Will be changed later perhaps Project-URL:
 Homepage, https://github.com/gutsh/django-cookie-consent Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE # Cookie consent
@@ -11,8 +11,11 @@
 this: ``` INSTALLED_APPS = [ "cookie_consent", ..., ] ``` 2. Include the
 cookie\_consent URLconf in your project urls.py like this: ``` path
 ("cookie_consent/", include("cookie_consent.urls")), ``` 3. Run `python
 manage.py migrate` to create the models. 4. Include consent template in your
 web-site templates. For example, I've included that text in my base template:
 ``` {% block cookie_consent %}
  {% include 'cookie_consent/includes/consent.html' %}
- {% endblock %} ``` 5. Start the development server and visit necessary pages.
+ {% endblock %} ``` Don't forget to serve that script and css files! You can
+find them in distribution, css is already fine (as long as you run
+`collectstatic` command), and javascript is available under `assets/js/tookit`.
+5. Start the development server and visit necessary pages.
```

### Comparing `django-cookie_consent_gutsh-0.1.0/django_cookie_consent_gutsh.egg-info/SOURCES.txt` & `django-cookie_consent_gutsh-1.0.0/django_cookie_consent_gutsh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-cookie_consent_gutsh-0.1.0/pyproject.toml` & `django-cookie_consent_gutsh-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "django-cookie_consent_gutsh"
-version = "0.1.0"
+version = "1.0.0"
 authors = [
     { name="Artem Barskii", email="artemiy.barskiy@gmail.com" },
 ]
 description = "Cookie consent component for any Django web-site"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `django-cookie_consent_gutsh-0.1.0/setup.cfg` & `django-cookie_consent_gutsh-1.0.0/setup.cfg`

 * *Files identical despite different names*

