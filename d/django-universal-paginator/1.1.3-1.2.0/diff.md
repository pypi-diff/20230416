# Comparing `tmp/django_universal_paginator-1.1.3.tar.gz` & `tmp/django_universal_paginator-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_universal_paginator-1.1.3.tar", last modified: Sat Apr  8 06:57:36 2023, max compression
+gzip compressed data, was "django_universal_paginator-1.2.0.tar", last modified: Sun Apr 16 06:41:13 2023, max compression
```

## Comparing `django_universal_paginator-1.1.3.tar` & `django_universal_paginator-1.2.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-08 06:57:36.050760 django_universal_paginator-1.1.3/
--rw-r--r--   0 mirec     (1000) mirec     (1000)       97 2022-12-18 17:51:41.000000 django_universal_paginator-1.1.3/.editorconfig
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-08 06:57:36.044760 django_universal_paginator-1.1.3/.github/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-08 06:57:36.047760 django_universal_paginator-1.1.3/.github/workflows/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1027 2022-12-18 18:41:54.000000 django_universal_paginator-1.1.3/.github/workflows/python-package.yml
--rw-r--r--   0 mirec     (1000) mirec     (1000)      142 2022-12-18 18:41:54.000000 django_universal_paginator-1.1.3/.gitignore
--rw-r--r--   0 mirec     (1000) mirec     (1000)      197 2022-12-18 17:51:41.000000 django_universal_paginator-1.1.3/.pre-commit-config.yaml
--rw-r--r--   0 mirec     (1000) mirec     (1000)    17720 2022-12-18 17:51:41.000000 django_universal_paginator-1.1.3/.pylintrc
--rw-r--r--   0 mirec     (1000) mirec     (1000)       45 2022-12-18 17:51:41.000000 django_universal_paginator-1.1.3/AUTHORS
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2340 2023-04-08 06:57:21.000000 django_universal_paginator-1.1.3/CHANGELOG.md
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1073 2022-12-18 17:51:41.000000 django_universal_paginator-1.1.3/LICENSE
--rw-r--r--   0 mirec     (1000) mirec     (1000)       92 2022-12-18 18:41:54.000000 django_universal_paginator-1.1.3/MANIFEST.in
--rw-r--r--   0 mirec     (1000) mirec     (1000)     5196 2023-04-08 06:57:36.050760 django_universal_paginator-1.1.3/PKG-INFO
--rw-r--r--   0 mirec     (1000) mirec     (1000)     4439 2022-12-26 12:18:20.000000 django_universal_paginator-1.1.3/README.rst
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-08 06:57:36.047760 django_universal_paginator-1.1.3/django_universal_paginator/
--rw-r--r--   0 mirec     (1000) mirec     (1000)       24 2022-12-18 18:48:06.000000 django_universal_paginator-1.1.3/django_universal_paginator/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)       96 2023-02-11 17:12:19.000000 django_universal_paginator-1.1.3/django_universal_paginator/constants.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      664 2023-02-11 17:23:37.000000 django_universal_paginator-1.1.3/django_universal_paginator/converter.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     4487 2023-04-08 06:57:16.000000 django_universal_paginator-1.1.3/django_universal_paginator/cursor.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      291 2022-12-18 18:48:06.000000 django_universal_paginator-1.1.3/django_universal_paginator/settings.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-08 06:57:36.045760 django_universal_paginator-1.1.3/django_universal_paginator/templates/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-08 06:57:36.047760 django_universal_paginator-1.1.3/django_universal_paginator/templates/paginator/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      738 2022-12-18 18:48:06.000000 django_universal_paginator-1.1.3/django_universal_paginator/templates/paginator/paginator.html
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-08 06:57:36.048760 django_universal_paginator-1.1.3/django_universal_paginator/templatetags/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-18 18:48:06.000000 django_universal_paginator-1.1.3/django_universal_paginator/templatetags/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     3440 2022-12-18 18:48:06.000000 django_universal_paginator-1.1.3/django_universal_paginator/templatetags/paginator_tags.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)    13848 2023-02-11 17:12:19.000000 django_universal_paginator-1.1.3/django_universal_paginator/utils.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-08 06:57:36.047760 django_universal_paginator-1.1.3/django_universal_paginator.egg-info/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     5196 2023-04-08 06:57:35.000000 django_universal_paginator-1.1.3/django_universal_paginator.egg-info/PKG-INFO
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1685 2023-04-08 06:57:36.000000 django_universal_paginator-1.1.3/django_universal_paginator.egg-info/SOURCES.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2023-04-08 06:57:35.000000 django_universal_paginator-1.1.3/django_universal_paginator.egg-info/dependency_links.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)       73 2023-04-08 06:57:35.000000 django_universal_paginator-1.1.3/django_universal_paginator.egg-info/requires.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)       27 2023-04-08 06:57:35.000000 django_universal_paginator-1.1.3/django_universal_paginator.egg-info/top_level.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1258 2023-04-08 06:57:21.000000 django_universal_paginator-1.1.3/pyproject.toml
--rw-r--r--   0 mirec     (1000) mirec     (1000)      395 2022-12-18 17:51:41.000000 django_universal_paginator-1.1.3/run_tests.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-08 06:57:36.048760 django_universal_paginator-1.1.3/sample_project/
--rwxr-xr-x   0 mirec     (1000) mirec     (1000)      749 2022-12-18 17:51:41.000000 django_universal_paginator-1.1.3/sample_project/manage.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-08 06:57:36.045760 django_universal_paginator-1.1.3/sample_project/static/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-08 06:57:36.048760 django_universal_paginator-1.1.3/sample_project/static/css/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1560 2022-12-18 17:51:41.000000 django_universal_paginator-1.1.3/sample_project/static/css/style.css
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-08 06:57:36.048760 django_universal_paginator-1.1.3/sample_project/templates/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      594 2022-12-18 18:41:54.000000 django_universal_paginator-1.1.3/sample_project/templates/base.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      375 2022-12-18 17:51:41.000000 django_universal_paginator-1.1.3/sample_project/templates/custom_template.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      534 2022-12-18 17:51:41.000000 django_universal_paginator-1.1.3/sample_project/templates/default.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      487 2022-12-18 18:41:54.000000 django_universal_paginator-1.1.3/sample_project/templates/home.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      313 2022-12-18 17:51:41.000000 django_universal_paginator-1.1.3/sample_project/templates/large.html
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-08 06:57:36.048760 django_universal_paginator-1.1.3/sample_project/templates/paginator/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      438 2022-12-18 17:51:41.000000 django_universal_paginator-1.1.3/sample_project/templates/paginator/custom.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      630 2022-12-18 17:51:41.000000 django_universal_paginator-1.1.3/sample_project/templates/paginator/paginator.html
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-08 06:57:36.049760 django_universal_paginator-1.1.3/sample_project/web/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-18 17:51:41.000000 django_universal_paginator-1.1.3/sample_project/web/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      145 2022-12-18 18:41:54.000000 django_universal_paginator-1.1.3/sample_project/web/apps.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-08 06:57:36.049760 django_universal_paginator-1.1.3/sample_project/web/migrations/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      890 2022-12-18 18:41:54.000000 django_universal_paginator-1.1.3/sample_project/web/migrations/0001_initial.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-18 18:41:54.000000 django_universal_paginator-1.1.3/sample_project/web/migrations/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      198 2022-12-18 18:41:54.000000 django_universal_paginator-1.1.3/sample_project/web/models.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1757 2022-12-18 18:41:54.000000 django_universal_paginator-1.1.3/sample_project/web/settings.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)       90 2022-12-18 18:41:54.000000 django_universal_paginator-1.1.3/sample_project/web/settings_local.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      689 2022-12-18 18:41:54.000000 django_universal_paginator-1.1.3/sample_project/web/urls.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      950 2022-12-18 18:41:54.000000 django_universal_paginator-1.1.3/sample_project/web/views.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      384 2022-12-18 17:51:41.000000 django_universal_paginator-1.1.3/sample_project/web/wsgi.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-04-08 06:57:36.050760 django_universal_paginator-1.1.3/setup.cfg
--rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2022-12-18 17:51:41.000000 django_universal_paginator-1.1.3/setup.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-08 06:57:36.050760 django_universal_paginator-1.1.3/tests/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-18 17:51:41.000000 django_universal_paginator-1.1.3/tests/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      762 2022-12-18 17:51:41.000000 django_universal_paginator-1.1.3/tests/models.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      813 2022-12-18 18:41:54.000000 django_universal_paginator-1.1.3/tests/settings.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-08 06:57:36.045760 django_universal_paginator-1.1.3/tests/templates/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-08 06:57:36.050760 django_universal_paginator-1.1.3/tests/templates/django/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      112 2022-12-18 17:51:41.000000 django_universal_paginator-1.1.3/tests/templates/django/example.html
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-08 06:57:36.050760 django_universal_paginator-1.1.3/tests/templates/jinja/
--rw-r--r--   0 mirec     (1000) mirec     (1000)       19 2022-12-18 17:51:41.000000 django_universal_paginator-1.1.3/tests/templates/jinja/example.jinja
--rw-r--r--   0 mirec     (1000) mirec     (1000)    17926 2023-02-11 17:27:57.000000 django_universal_paginator-1.1.3/tests/tests.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      522 2022-12-18 18:41:54.000000 django_universal_paginator-1.1.3/tests/urls.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      577 2022-12-18 18:41:54.000000 django_universal_paginator-1.1.3/tests/views.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      442 2022-12-18 18:41:54.000000 django_universal_paginator-1.1.3/tox.ini
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.292059 django_universal_paginator-1.2.0/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       97 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/.editorconfig
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.288059 django_universal_paginator-1.2.0/.github/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.290059 django_universal_paginator-1.2.0/.github/workflows/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1027 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/.github/workflows/python-package.yml
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      142 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/.gitignore
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      197 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 mirec     (1000) mirec     (1000)    17720 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/.pylintrc
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       45 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/AUTHORS
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2444 2023-04-16 06:41:05.000000 django_universal_paginator-1.2.0/CHANGELOG.md
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1073 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/LICENSE
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       92 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/MANIFEST.in
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     5196 2023-04-16 06:41:13.292059 django_universal_paginator-1.2.0/PKG-INFO
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     4439 2022-12-26 12:18:20.000000 django_universal_paginator-1.2.0/README.rst
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.290059 django_universal_paginator-1.2.0/django_universal_paginator/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       24 2022-12-18 18:48:06.000000 django_universal_paginator-1.2.0/django_universal_paginator/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       96 2023-02-11 17:12:19.000000 django_universal_paginator-1.2.0/django_universal_paginator/constants.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      664 2023-02-11 17:23:37.000000 django_universal_paginator-1.2.0/django_universal_paginator/converter.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     4628 2023-04-16 06:40:59.000000 django_universal_paginator-1.2.0/django_universal_paginator/cursor.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      291 2022-12-18 18:48:06.000000 django_universal_paginator-1.2.0/django_universal_paginator/settings.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.288059 django_universal_paginator-1.2.0/django_universal_paginator/templates/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.290059 django_universal_paginator-1.2.0/django_universal_paginator/templates/paginator/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      738 2022-12-18 18:48:06.000000 django_universal_paginator-1.2.0/django_universal_paginator/templates/paginator/paginator.html
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.290059 django_universal_paginator-1.2.0/django_universal_paginator/templatetags/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-18 18:48:06.000000 django_universal_paginator-1.2.0/django_universal_paginator/templatetags/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     3440 2022-12-18 18:48:06.000000 django_universal_paginator-1.2.0/django_universal_paginator/templatetags/paginator_tags.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)    13899 2023-04-16 06:40:59.000000 django_universal_paginator-1.2.0/django_universal_paginator/utils.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.290059 django_universal_paginator-1.2.0/django_universal_paginator.egg-info/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     5196 2023-04-16 06:41:13.000000 django_universal_paginator-1.2.0/django_universal_paginator.egg-info/PKG-INFO
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1685 2023-04-16 06:41:13.000000 django_universal_paginator-1.2.0/django_universal_paginator.egg-info/SOURCES.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2023-04-16 06:41:13.000000 django_universal_paginator-1.2.0/django_universal_paginator.egg-info/dependency_links.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       73 2023-04-16 06:41:13.000000 django_universal_paginator-1.2.0/django_universal_paginator.egg-info/requires.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       27 2023-04-16 06:41:13.000000 django_universal_paginator-1.2.0/django_universal_paginator.egg-info/top_level.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1258 2023-04-16 06:41:05.000000 django_universal_paginator-1.2.0/pyproject.toml
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      395 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/run_tests.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.290059 django_universal_paginator-1.2.0/sample_project/
+-rwxr-xr-x   0 mirec     (1000) mirec     (1000)      749 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/sample_project/manage.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.289059 django_universal_paginator-1.2.0/sample_project/static/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.290059 django_universal_paginator-1.2.0/sample_project/static/css/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1560 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/sample_project/static/css/style.css
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.291059 django_universal_paginator-1.2.0/sample_project/templates/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      594 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/sample_project/templates/base.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      375 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/sample_project/templates/custom_template.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      592 2023-04-16 06:40:59.000000 django_universal_paginator-1.2.0/sample_project/templates/default.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      575 2023-04-16 06:40:59.000000 django_universal_paginator-1.2.0/sample_project/templates/home.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      313 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/sample_project/templates/large.html
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.291059 django_universal_paginator-1.2.0/sample_project/templates/paginator/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      438 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/sample_project/templates/paginator/custom.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      630 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/sample_project/templates/paginator/paginator.html
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.291059 django_universal_paginator-1.2.0/sample_project/web/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/sample_project/web/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      145 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/sample_project/web/apps.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.291059 django_universal_paginator-1.2.0/sample_project/web/migrations/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      890 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/sample_project/web/migrations/0001_initial.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/sample_project/web/migrations/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      198 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/sample_project/web/models.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1757 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/sample_project/web/settings.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       90 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/sample_project/web/settings_local.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      785 2023-04-16 06:40:59.000000 django_universal_paginator-1.2.0/sample_project/web/urls.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1157 2023-04-16 06:40:59.000000 django_universal_paginator-1.2.0/sample_project/web/views.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      384 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/sample_project/web/wsgi.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-04-16 06:41:13.292059 django_universal_paginator-1.2.0/setup.cfg
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/setup.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.291059 django_universal_paginator-1.2.0/tests/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/tests/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      762 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/tests/models.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      813 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/tests/settings.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.289059 django_universal_paginator-1.2.0/tests/templates/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.291059 django_universal_paginator-1.2.0/tests/templates/django/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      112 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/tests/templates/django/example.html
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-04-16 06:41:13.291059 django_universal_paginator-1.2.0/tests/templates/jinja/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       19 2022-12-18 17:51:41.000000 django_universal_paginator-1.2.0/tests/templates/jinja/example.jinja
+-rw-r--r--   0 mirec     (1000) mirec     (1000)    18167 2023-04-16 06:40:59.000000 django_universal_paginator-1.2.0/tests/tests.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      522 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/tests/urls.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      577 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/tests/views.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      442 2022-12-18 18:41:54.000000 django_universal_paginator-1.2.0/tox.ini
```

### Comparing `django_universal_paginator-1.1.3/.github/workflows/python-package.yml` & `django_universal_paginator-1.2.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.1.3/.pylintrc` & `django_universal_paginator-1.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.1.3/CHANGELOG.md` & `django_universal_paginator-1.2.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## 1.2.0 (2023-04-16)
+
+### Feat
+
+- Added example with values_list
+- Added pagination using values_list
+
 ## 1.1.3 (2023-04-08)
 
 ### Fix
 
 - Don't throw exception on unknown page
 
 ## 1.1.2 (2023-02-11)
```

### Comparing `django_universal_paginator-1.1.3/LICENSE` & `django_universal_paginator-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.1.3/PKG-INFO` & `django_universal_paginator-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_universal_paginator
-Version: 1.1.3
+Version: 1.2.0
 Summary: Simple pagination for django
 Author-email: Miroslav Bendík <miroslav.bendik@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/mireq/django-universal-paginator
 Project-URL: documentation, https://github.com/mireq/django-universal-paginator
 Project-URL: repository, https://github.com/mireq/django-universal-paginator
 Project-URL: changelog, https://github.com/mireq/django-universal-paginator/blob/master/CHANGELOG.md
```

### Comparing `django_universal_paginator-1.1.3/README.rst` & `django_universal_paginator-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.1.3/django_universal_paginator/converter.py` & `django_universal_paginator-1.2.0/django_universal_paginator/converter.py`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.1.3/django_universal_paginator/cursor.py` & `django_universal_paginator-1.2.0/django_universal_paginator/cursor.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,20 +39,26 @@
 
 class IteratorWrapper(object):
 	def __init__(self, iterator_class, paginator, page, *args, **kwargs):
 		self.iterator = iterator_class(*args, **kwargs)
 		self.paginator = paginator
 		self.page = page
 
+	def _get_sentinel(self, obj):
+		if isinstance(obj, dict):
+			return obj[constants.SENTINEL_NAME]
+		else:
+			return getattr(obj, constants.SENTINEL_NAME)
+
 	@cached_property
 	def _result_cache(self):
 		cache = list(self.iterator)
 		start_key = self.paginator.get_start_order_key(self.page.number)
 
-		if self.page.number is not None and cache and getattr(cache[0], constants.SENTINEL_NAME):
+		if self.page.number is not None and cache and self._get_sentinel(cache[0]):
 			if start_key.direction == constants.KEY_BACK:
 				self.page.next_page_item = cache.pop(0)
 			else:
 				self.page.prev_page_item = cache.pop(0)
 
 		# last item handling (used to check previous page existence)
 		if len(cache) > self.paginator.per_page:
```

### Comparing `django_universal_paginator-1.1.3/django_universal_paginator/templates/paginator/paginator.html` & `django_universal_paginator-1.2.0/django_universal_paginator/templates/paginator/paginator.html`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.1.3/django_universal_paginator/templatetags/paginator_tags.py` & `django_universal_paginator-1.2.0/django_universal_paginator/templatetags/paginator_tags.py`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.1.3/django_universal_paginator/utils.py` & `django_universal_paginator-1.2.0/django_universal_paginator/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,14 +265,16 @@
 		raise Http404(_('Invalid page (%(page_number)s): %(message)s') % {'page_number': page_number, 'message': str(e)})
 
 
 def get_model_attribute(obj, attribute):
 	"""
 	Get model attribute by traversing attributes by django path like review__book
 	"""
+	if isinstance(obj, dict):
+		return obj[attribute]
 	for lookup in attribute.split(LOOKUP_SEP):
 		obj = getattr(obj, lookup)
 	return obj
 
 
 def get_order_key(obj, order_by):
 	"""
```

### Comparing `django_universal_paginator-1.1.3/django_universal_paginator.egg-info/PKG-INFO` & `django_universal_paginator-1.2.0/django_universal_paginator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-universal-paginator
-Version: 1.1.3
+Version: 1.2.0
 Summary: Simple pagination for django
 Author-email: Miroslav Bendík <miroslav.bendik@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/mireq/django-universal-paginator
 Project-URL: documentation, https://github.com/mireq/django-universal-paginator
 Project-URL: repository, https://github.com/mireq/django-universal-paginator
 Project-URL: changelog, https://github.com/mireq/django-universal-paginator/blob/master/CHANGELOG.md
```

### Comparing `django_universal_paginator-1.1.3/django_universal_paginator.egg-info/SOURCES.txt` & `django_universal_paginator-1.2.0/django_universal_paginator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.1.3/pyproject.toml` & `django_universal_paginator-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -39,9 +39,9 @@
 [tool.setuptools]
 packages = ["django_universal_paginator", "django_universal_paginator.templates.paginator", "django_universal_paginator.templatetags"]
 
 [tool.setuptools_scm]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.1.3"
+version = "1.2.0"
 tag_format = "$version"
```

### Comparing `django_universal_paginator-1.1.3/sample_project/manage.py` & `django_universal_paginator-1.2.0/sample_project/manage.py`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.1.3/sample_project/static/css/style.css` & `django_universal_paginator-1.2.0/sample_project/static/css/style.css`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.1.3/sample_project/templates/base.html` & `django_universal_paginator-1.2.0/sample_project/templates/base.html`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.1.3/sample_project/templates/paginator/paginator.html` & `django_universal_paginator-1.2.0/sample_project/templates/paginator/paginator.html`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.1.3/sample_project/web/migrations/0001_initial.py` & `django_universal_paginator-1.2.0/sample_project/web/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.1.3/sample_project/web/settings.py` & `django_universal_paginator-1.2.0/sample_project/web/settings.py`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.1.3/sample_project/web/views.py` & `django_universal_paginator-1.2.0/sample_project/web/views.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,12 +21,18 @@
 
 
 class CursorListView(CursorPaginateMixin, SampleListView):
 	def get_queryset(self):
 		return Random.objects.order_by('pk')
 
 
+class CursorValuesListView(CursorListView):
+	def get_queryset(self):
+		return super().get_queryset().values('pk', 'name')
+
+
 home_view = TemplateView.as_view(template_name='home.html')
 default_paginator_view = SampleListView.as_view(template_name='default.html')
 large_paginator_view = SampleListView.as_view(template_name='large.html')
 custom_template_paginator_view = SampleListView.as_view(template_name='custom_template.html')
 cursor_list_view = CursorListView.as_view(template_name='large.html')
+cursor_values_list_view = CursorValuesListView.as_view(template_name='large.html')
```

### Comparing `django_universal_paginator-1.1.3/tests/models.py` & `django_universal_paginator-1.2.0/tests/models.py`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.1.3/tests/settings.py` & `django_universal_paginator-1.2.0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.1.3/tests/tests.py` & `django_universal_paginator-1.2.0/tests/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,15 +297,23 @@
 		books = Book.objects.order_by('pk').none()
 		__, page, qs, __ = paginate_cursor_queryset(books, None, 2)
 		self.assertFalse(page.has_previous())
 		self.assertFalse(page.has_next())
 		self.assertBookPage([], qs)
 
 	def test_paginate(self):
+		self.runPaginationTest(False)
+
+	def test_paginate_values(self):
+		self.runPaginationTest(True)
+
+	def runPaginationTest(self, use_values: bool = False):
 		books = Book.objects.order_by('pk')
+		if use_values:
+			books = books.values('pk')
 		paginator, page, qs, __ = paginate_cursor_queryset(books, None, 2)
 		# not needed
 		self.assertEqual(0, paginator.count)
 		self.assertEqual(0, paginator.num_pages)
 		self.assertFalse(page.has_previous())
 		self.assertTrue(page.has_next())
 
@@ -353,15 +361,15 @@
 
 		books = Book.objects.order_by('pk')
 
 		__, __, qs, __ = v.paginate_queryset(books, page_size=2)
 		self.assertBookPage([1, 2], qs)
 
 	def assertBookPage(self, ids, qs):
-		returned_pages = [obj.pk for obj in qs]
+		returned_pages = [obj['pk'] if isinstance(obj, dict) else obj.pk for obj in qs]
 		self.assertEqual(ids, returned_pages)
 
 
 class TestTemplates(TestCase):
 	@classmethod
 	def setUpTestData(cls):
 		book_list = [
```

### Comparing `django_universal_paginator-1.1.3/tests/urls.py` & `django_universal_paginator-1.2.0/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_universal_paginator-1.1.3/tests/views.py` & `django_universal_paginator-1.2.0/tests/views.py`

 * *Files identical despite different names*

