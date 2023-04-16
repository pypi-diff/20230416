# Comparing `tmp/pinax-teams-2.0.0.tar.gz` & `tmp/pinax-teams-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pinax-teams-2.0.0.tar", last modified: Sun Jul 19 18:17:22 2020, max compression
+gzip compressed data, was "pinax-teams-3.0.0.tar", last modified: Sun Apr 16 15:09:36 2023, max compression
```

## Comparing `pinax-teams-2.0.0.tar` & `pinax-teams-3.0.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-19 18:17:22.752891 pinax-teams-2.0.0/
--rw-r--r--   0 katherinemichel   (501) staff       (20)      592 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/AUTHORS
--rw-r--r--   0 katherinemichel   (501) staff       (20)     1104 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/LICENSE
--rw-r--r--   0 katherinemichel   (501) staff       (20)       89 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/MANIFEST.in
--rw-r--r--   0 katherinemichel   (501) staff       (20)     2917 2020-07-19 18:17:22.752624 pinax-teams-2.0.0/PKG-INFO
--rw-r--r--   0 katherinemichel   (501) staff       (20)     8081 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/README.md
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-19 18:17:22.741436 pinax-teams-2.0.0/pinax/
--rw-r--r--   0 katherinemichel   (501) staff       (20)       84 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/__init__.py
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-19 18:17:22.746263 pinax-teams-2.0.0/pinax/teams/
--rw-r--r--   0 katherinemichel   (501) staff       (20)      141 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/__init__.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      924 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/admin.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      394 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/apps.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      928 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/conf.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)     1413 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/context_urls.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)     1552 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/decorators.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)     2861 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/forms.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)     1682 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/hooks.py
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-19 18:17:22.739324 pinax-teams-2.0.0/pinax/teams/locale/
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-19 18:17:22.739190 pinax-teams-2.0.0/pinax/teams/locale/en/
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-19 18:17:22.746691 pinax-teams-2.0.0/pinax/teams/locale/en/LC_MESSAGES/
--rw-r--r--   0 katherinemichel   (501) staff       (20)     1968 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-19 18:17:22.739399 pinax-teams-2.0.0/pinax/teams/locale/ja/
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-19 18:17:22.747566 pinax-teams-2.0.0/pinax/teams/locale/ja/LC_MESSAGES/
--rw-r--r--   0 katherinemichel   (501) staff       (20)     1738 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 katherinemichel   (501) staff       (20)     2391 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0 katherinemichel   (501) staff       (20)     2016 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/middleware.py
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-19 18:17:22.749344 pinax-teams-2.0.0/pinax/teams/migrations/
--rw-r--r--   0 katherinemichel   (501) staff       (20)     3635 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/migrations/0001_initial.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)     3269 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/migrations/0002_add_simple_models.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)     2663 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/migrations/0003_auto_20170416_1752.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)     1060 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/migrations/0004_auto_20170511_0856.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)        0 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/migrations/__init__.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)    12754 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/models.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      767 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/receivers.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      651 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/signals.py
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-19 18:17:22.749802 pinax-teams-2.0.0/pinax/teams/templatetags/
--rw-r--r--   0 katherinemichel   (501) staff       (20)        0 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/templatetags/__init__.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)     1091 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/templatetags/pinax_teams_tags.py
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-19 18:17:22.750634 pinax-teams-2.0.0/pinax/teams/tests/
--rw-r--r--   0 katherinemichel   (501) staff       (20)        0 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/tests/__init__.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)    14848 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/tests/tests.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      178 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/tests/urls.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)     1793 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/urls.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)     1720 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/utils.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)    12550 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/views.py
--rw-r--r--   0 katherinemichel   (501) staff       (20)      518 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/pinax/teams/wsgi_middleware.py
-drwxr-xr-x   0 katherinemichel   (501) staff       (20)        0 2020-07-19 18:17:22.752266 pinax-teams-2.0.0/pinax_teams.egg-info/
--rw-r--r--   0 katherinemichel   (501) staff       (20)     2917 2020-07-19 18:17:22.000000 pinax-teams-2.0.0/pinax_teams.egg-info/PKG-INFO
--rw-r--r--   0 katherinemichel   (501) staff       (20)     1162 2020-07-19 18:17:22.000000 pinax-teams-2.0.0/pinax_teams.egg-info/SOURCES.txt
--rw-r--r--   0 katherinemichel   (501) staff       (20)        1 2020-07-19 18:17:22.000000 pinax-teams-2.0.0/pinax_teams.egg-info/dependency_links.txt
--rw-r--r--   0 katherinemichel   (501) staff       (20)        1 2020-07-19 18:17:22.000000 pinax-teams-2.0.0/pinax_teams.egg-info/not-zip-safe
--rw-r--r--   0 katherinemichel   (501) staff       (20)      137 2020-07-19 18:17:22.000000 pinax-teams-2.0.0/pinax_teams.egg-info/requires.txt
--rw-r--r--   0 katherinemichel   (501) staff       (20)        6 2020-07-19 18:17:22.000000 pinax-teams-2.0.0/pinax_teams.egg-info/top_level.txt
--rw-r--r--   0 katherinemichel   (501) staff       (20)       38 2020-07-19 18:17:22.753229 pinax-teams-2.0.0/setup.cfg
--rw-r--r--   0 katherinemichel   (501) staff       (20)     3165 2020-07-19 18:16:40.000000 pinax-teams-2.0.0/setup.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-16 15:09:36.650141 pinax-teams-3.0.0/
+-rw-r--r--   0 chris      (502) staff       (20)      592 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/AUTHORS
+-rw-r--r--   0 chris      (502) staff       (20)     1104 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/LICENSE
+-rw-r--r--   0 chris      (502) staff       (20)       89 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/MANIFEST.in
+-rw-r--r--   0 chris      (502) staff       (20)     2663 2023-04-16 15:09:36.649806 pinax-teams-3.0.0/PKG-INFO
+-rw-r--r--   0 chris      (502) staff       (20)     8174 2023-04-15 00:28:42.000000 pinax-teams-3.0.0/README.md
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-16 15:09:36.629923 pinax-teams-3.0.0/pinax/
+-rw-r--r--   0 chris      (502) staff       (20)       84 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/__init__.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-16 15:09:36.640588 pinax-teams-3.0.0/pinax/teams/
+-rw-r--r--   0 chris      (502) staff       (20)      141 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/__init__.py
+-rw-r--r--   0 chris      (502) staff       (20)      923 2023-03-29 23:19:02.000000 pinax-teams-3.0.0/pinax/teams/admin.py
+-rw-r--r--   0 chris      (502) staff       (20)      325 2023-04-16 10:31:39.000000 pinax-teams-3.0.0/pinax/teams/apps.py
+-rw-r--r--   0 chris      (502) staff       (20)      928 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/conf.py
+-rw-r--r--   0 chris      (502) staff       (20)     1413 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/context_urls.py
+-rw-r--r--   0 chris      (502) staff       (20)     1552 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/decorators.py
+-rw-r--r--   0 chris      (502) staff       (20)     2860 2023-03-29 23:18:57.000000 pinax-teams-3.0.0/pinax/teams/forms.py
+-rw-r--r--   0 chris      (502) staff       (20)     1682 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/hooks.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-16 15:09:36.625472 pinax-teams-3.0.0/pinax/teams/locale/
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-16 15:09:36.625279 pinax-teams-3.0.0/pinax/teams/locale/en/
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-16 15:09:36.641167 pinax-teams-3.0.0/pinax/teams/locale/en/LC_MESSAGES/
+-rw-r--r--   0 chris      (502) staff       (20)     1968 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-16 15:09:36.625627 pinax-teams-3.0.0/pinax/teams/locale/ja/
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-16 15:09:36.642240 pinax-teams-3.0.0/pinax/teams/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 chris      (502) staff       (20)     1738 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 chris      (502) staff       (20)     2391 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0 chris      (502) staff       (20)     2016 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/middleware.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-16 15:09:36.644609 pinax-teams-3.0.0/pinax/teams/migrations/
+-rw-r--r--   0 chris      (502) staff       (20)     3635 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/migrations/0001_initial.py
+-rw-r--r--   0 chris      (502) staff       (20)     3269 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/migrations/0002_add_simple_models.py
+-rw-r--r--   0 chris      (502) staff       (20)     2663 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/migrations/0003_auto_20170416_1752.py
+-rw-r--r--   0 chris      (502) staff       (20)     1060 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/migrations/0004_auto_20170511_0856.py
+-rw-r--r--   0 chris      (502) staff       (20)        0 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/migrations/__init__.py
+-rw-r--r--   0 chris      (502) staff       (20)    12753 2023-03-29 23:18:52.000000 pinax-teams-3.0.0/pinax/teams/models.py
+-rw-r--r--   0 chris      (502) staff       (20)      767 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/receivers.py
+-rw-r--r--   0 chris      (502) staff       (20)      370 2023-03-29 23:20:08.000000 pinax-teams-3.0.0/pinax/teams/signals.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-16 15:09:36.645166 pinax-teams-3.0.0/pinax/teams/templatetags/
+-rw-r--r--   0 chris      (502) staff       (20)        0 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/templatetags/__init__.py
+-rw-r--r--   0 chris      (502) staff       (20)     1091 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/templatetags/pinax_teams_tags.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-16 15:09:36.646497 pinax-teams-3.0.0/pinax/teams/tests/
+-rw-r--r--   0 chris      (502) staff       (20)        0 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/tests/__init__.py
+-rw-r--r--   0 chris      (502) staff       (20)    14848 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/tests/tests.py
+-rw-r--r--   0 chris      (502) staff       (20)      185 2023-03-29 23:25:11.000000 pinax-teams-3.0.0/pinax/teams/tests/urls.py
+-rw-r--r--   0 chris      (502) staff       (20)     1860 2023-03-29 23:26:34.000000 pinax-teams-3.0.0/pinax/teams/urls.py
+-rw-r--r--   0 chris      (502) staff       (20)     1720 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/utils.py
+-rw-r--r--   0 chris      (502) staff       (20)    12550 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/views.py
+-rw-r--r--   0 chris      (502) staff       (20)      518 2022-12-05 18:56:49.000000 pinax-teams-3.0.0/pinax/teams/wsgi_middleware.py
+drwxr-xr-x   0 chris      (502) staff       (20)        0 2023-04-16 15:09:36.649242 pinax-teams-3.0.0/pinax_teams.egg-info/
+-rw-r--r--   0 chris      (502) staff       (20)     2663 2023-04-16 15:09:36.000000 pinax-teams-3.0.0/pinax_teams.egg-info/PKG-INFO
+-rw-r--r--   0 chris      (502) staff       (20)     1162 2023-04-16 15:09:36.000000 pinax-teams-3.0.0/pinax_teams.egg-info/SOURCES.txt
+-rw-r--r--   0 chris      (502) staff       (20)        1 2023-04-16 15:09:36.000000 pinax-teams-3.0.0/pinax_teams.egg-info/dependency_links.txt
+-rw-r--r--   0 chris      (502) staff       (20)        1 2023-02-17 18:45:45.000000 pinax-teams-3.0.0/pinax_teams.egg-info/not-zip-safe
+-rw-r--r--   0 chris      (502) staff       (20)      125 2023-04-16 15:09:36.000000 pinax-teams-3.0.0/pinax_teams.egg-info/requires.txt
+-rw-r--r--   0 chris      (502) staff       (20)        6 2023-04-16 15:09:36.000000 pinax-teams-3.0.0/pinax_teams.egg-info/top_level.txt
+-rw-r--r--   0 chris      (502) staff       (20)       38 2023-04-16 15:09:36.650233 pinax-teams-3.0.0/setup.cfg
+-rw-r--r--   0 chris      (502) staff       (20)     3234 2023-04-15 00:08:13.000000 pinax-teams-3.0.0/setup.py
```

### Comparing `pinax-teams-2.0.0/AUTHORS` & `pinax-teams-3.0.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `pinax-teams-2.0.0/LICENSE` & `pinax-teams-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pinax-teams-2.0.0/PKG-INFO` & `pinax-teams-3.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,94 @@
-Metadata-Version: 1.1
-Name: pinax-teams
-Version: 2.0.0
-Summary: An app for Django sites that supports open, by invitation, and by application teams
-Home-page: http://github.com/pinax/pinax-teams/
-Author: Pinax Team
-Author-email: team@pinaxproject.com
-License: MIT
-Description: 
-        .. image:: http://pinaxproject.com/pinax-design/patches/pinax-teams.svg
-            :target: https://pypi.python.org/pypi/pinax-teams/
-        
-        ===========
-        Pinax Teams
-        ===========
-        
-        .. image:: https://img.shields.io/pypi/v/pinax-teams.svg
-            :target: https://pypi.python.org/pypi/pinax-teams/
-        
-        \ 
-        
-        .. image:: https://img.shields.io/circleci/project/github/pinax/pinax-teams.svg
-            :target: https://circleci.com/gh/pinax/pinax-teams
-        .. image:: https://img.shields.io/codecov/c/github/pinax/pinax-teams.svg
-            :target: https://codecov.io/gh/pinax/pinax-teams
-        .. image:: https://img.shields.io/github/contributors/pinax/pinax-teams.svg
-            :target: https://github.com/pinax/pinax-teams/graphs/contributors
-        .. image:: https://img.shields.io/github/issues-pr/pinax/pinax-teams.svg
-            :target: https://github.com/pinax/pinax-teams/pulls
-        .. image:: https://img.shields.io/github/issues-pr-closed/pinax/pinax-teams.svg
-            :target: https://github.com/pinax/pinax-teams/pulls?q=is%3Apr+is%3Aclosed
-        
-        \ 
-        
-        .. image:: http://slack.pinaxproject.com/badge.svg
-            :target: http://slack.pinaxproject.com/
-        .. image:: https://img.shields.io/badge/license-MIT-blue.svg
-            :target: https://pypi.python.org/pypi/pinax-teams/
-        
-        \ 
-        
-        ``pinax-teams`` is an app for Django sites that supports open, by invitation, and by application teams.
-        
-        Supported Django and Python Versions
-        ------------------------------------
-        
-        +-----------------+-----+-----+-----+
-        | Django / Python | 3.6 | 3.7 | 3.8 |
-        +=================+=====+=====+=====+
-        |  2.2            |  *  |  *  |  *  |
-        +-----------------+-----+-----+-----+
-        |  3.0            |  *  |  *  |  *  |
-        +-----------------+-----+-----+-----+
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
+from setuptools import find_packages, setup
+
+VERSION = "3.0.0"
+LONG_DESCRIPTION = r"""
+.. image:: http://pinaxproject.com/pinax-design/patches/pinax-teams.svg
+    :target: https://pypi.python.org/pypi/pinax-teams/
+
+===========
+Pinax Teams
+===========
+
+.. image:: https://img.shields.io/pypi/v/pinax-teams.svg
+    :target: https://pypi.python.org/pypi/pinax-teams/
+
+\ 
+
+.. image:: https://img.shields.io/circleci/project/github/pinax/pinax-teams.svg
+    :target: https://circleci.com/gh/pinax/pinax-teams
+.. image:: https://img.shields.io/codecov/c/github/pinax/pinax-teams.svg
+    :target: https://codecov.io/gh/pinax/pinax-teams
+.. image:: https://img.shields.io/github/contributors/pinax/pinax-teams.svg
+    :target: https://github.com/pinax/pinax-teams/graphs/contributors
+.. image:: https://img.shields.io/github/issues-pr/pinax/pinax-teams.svg
+    :target: https://github.com/pinax/pinax-teams/pulls
+.. image:: https://img.shields.io/github/issues-pr-closed/pinax/pinax-teams.svg
+    :target: https://github.com/pinax/pinax-teams/pulls?q=is%3Apr+is%3Aclosed
+
+\ 
+
+.. image:: http://slack.pinaxproject.com/badge.svg
+    :target: http://slack.pinaxproject.com/
+.. image:: https://img.shields.io/badge/license-MIT-blue.svg
+    :target: https://pypi.python.org/pypi/pinax-teams/
+
+\ 
+
+``pinax-teams`` is an app for Django sites that supports open, by invitation, and by application teams.
+
+Supported Django and Python Versions
+------------------------------------
+
++-----------------+-----+-----+-----+-----+
+| Django / Python | 3.7 | 3.8 | 3.9 | 3.10|
++=================+=====+=====+=====+=====+
+|  3.2            |  *  |  *  |  *  |  *  |
++-----------------+-----+-----+-----+-----+
+|  4.1            |  -  |  -  |  -  |  *  |
++-----------------+-----+-----+-----+-----+
+"""
+
+setup(
+    author="Pinax Team",
+    author_email="team@pinaxproject.com",
+    description="An app for Django sites that supports open, by invitation, and by application teams",
+    name="pinax-teams",
+    long_description=LONG_DESCRIPTION,
+    version=VERSION,
+    url="http://github.com/pinax/pinax-teams/",
+    license="MIT",
+    packages=find_packages(),
+    package_data={
+        "teams": []
+    },
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Environment :: Web Environment",
+        "Framework :: Django",
+        "Framework :: Django :: 3.0",
+        "Framework :: Django :: 4.0",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+    ],
+    install_requires=[
+        "django>=3.2",
+        "django-reversion>=5.0.4",
+        "pinax-invitations>=8.0.0",
+        "python-slugify>=7.0.0",
+        "Pillow>=9.3.0",
+        "django-user-accounts>=3.2.0"
+    ],
+    tests_require=[
+        "django-test-plus>=1.0.22",
+        "pinax-templates>=3.0.0",
+    ],
+    test_suite="runtests.runtests",
+    zip_safe=False
+)
```

### Comparing `pinax-teams-2.0.0/README.md` & `pinax-teams-3.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -60,26 +60,25 @@
 #### Dependencies
 
 * django-appconf
 * django-reversion
 * django-user-accounts
 * pillow
 * pinax-invitations
-* six
 * python-slugify
 
 See [`setup.py`](https://github.com/pinax/pinax-teams/blob/master/setup.py) for specific required versions of these packages.
 
 
 #### Supported Django and Python Versions
 
-Django / Python | 3.6 | 3.7 | 3.8
+Django / Python | 3.7 | 3.8 | 3.9| 3.10
 --------------- | --- | --- | ---
-2.2  |  *  |  *  |  *
-3.0  |  *  |  *  |  *
+3.2  |  *  |  *  |  * |  *
+4.1  |  -  |  -  |  - |  *
 
 
 ## Documentation
 
 ### Installation
 
 To install pinax-teams:
@@ -196,20 +195,25 @@
 #### `_membership.html`
 
 ### Views
 
 
 ## Change Log
 
+### 3.0.0
+
+* Drop Django 2 and <3.2 and Python 2.*, <3.6 support
+* Add Django 4.0, and Python 3.7, 3.8 and 3.9 support
+
+
 ### 2.0.0
 
 * Drop Django 1.11, 2.0, and 2.1, and Python 2,7, 3.4, and 3.5 support
 * Add Django 2.2 and 3.0, and Python 3.6, 3.7, and 3.8 support
 * Update packaging configs
-* Direct users to community resources
 
 ### 1.0.6
 
 * Switch to using python-slugify from unicode-slugify
 
 ### 1.0.5
```

### Comparing `pinax-teams-2.0.0/pinax/teams/admin.py` & `pinax-teams-3.0.0/pinax/teams/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.contrib import admin
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from reversion.admin import VersionAdmin
 
 from .hooks import hookset
 from .models import Membership, Team
```

### Comparing `pinax-teams-2.0.0/pinax/teams/conf.py` & `pinax-teams-3.0.0/pinax/teams/conf.py`

 * *Files identical despite different names*

### Comparing `pinax-teams-2.0.0/pinax/teams/context_urls.py` & `pinax-teams-3.0.0/pinax/teams/context_urls.py`

 * *Files identical despite different names*

### Comparing `pinax-teams-2.0.0/pinax/teams/decorators.py` & `pinax-teams-3.0.0/pinax/teams/decorators.py`

 * *Files identical despite different names*

### Comparing `pinax-teams-2.0.0/pinax/teams/forms.py` & `pinax-teams-3.0.0/pinax/teams/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django import forms
 from django.contrib.auth import get_user_model
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from account.forms import SignupForm
 
 from .conf import settings
 from .hooks import hookset
 from .models import Membership, Team, create_slug
```

### Comparing `pinax-teams-2.0.0/pinax/teams/hooks.py` & `pinax-teams-3.0.0/pinax/teams/hooks.py`

 * *Files identical despite different names*

### Comparing `pinax-teams-2.0.0/pinax/teams/locale/en/LC_MESSAGES/django.po` & `pinax-teams-3.0.0/pinax/teams/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pinax-teams-2.0.0/pinax/teams/locale/ja/LC_MESSAGES/django.mo` & `pinax-teams-3.0.0/pinax/teams/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `pinax-teams-2.0.0/pinax/teams/locale/ja/LC_MESSAGES/django.po` & `pinax-teams-3.0.0/pinax/teams/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pinax-teams-2.0.0/pinax/teams/middleware.py` & `pinax-teams-3.0.0/pinax/teams/middleware.py`

 * *Files identical despite different names*

### Comparing `pinax-teams-2.0.0/pinax/teams/migrations/0001_initial.py` & `pinax-teams-3.0.0/pinax/teams/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pinax-teams-2.0.0/pinax/teams/migrations/0002_add_simple_models.py` & `pinax-teams-3.0.0/pinax/teams/migrations/0002_add_simple_models.py`

 * *Files identical despite different names*

### Comparing `pinax-teams-2.0.0/pinax/teams/migrations/0003_auto_20170416_1752.py` & `pinax-teams-3.0.0/pinax/teams/migrations/0003_auto_20170416_1752.py`

 * *Files identical despite different names*

### Comparing `pinax-teams-2.0.0/pinax/teams/migrations/0004_auto_20170511_0856.py` & `pinax-teams-3.0.0/pinax/teams/migrations/0004_auto_20170511_0856.py`

 * *Files identical despite different names*

### Comparing `pinax-teams-2.0.0/pinax/teams/models.py` & `pinax-teams-3.0.0/pinax/teams/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import uuid
 
 from django.conf import settings
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import models
 from django.urls import reverse
 from django.utils import timezone
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from pinax.invitations.models import JoinInvitation
 from reversion import revisions as reversion
 from slugify import slugify
 
 from . import signals
 from .hooks import hookset
```

### Comparing `pinax-teams-2.0.0/pinax/teams/receivers.py` & `pinax-teams-3.0.0/pinax/teams/receivers.py`

 * *Files identical despite different names*

### Comparing `pinax-teams-2.0.0/pinax/teams/templatetags/pinax_teams_tags.py` & `pinax-teams-3.0.0/pinax/teams/templatetags/pinax_teams_tags.py`

 * *Files identical despite different names*

### Comparing `pinax-teams-2.0.0/pinax/teams/tests/tests.py` & `pinax-teams-3.0.0/pinax/teams/tests/tests.py`

 * *Files identical despite different names*

### Comparing `pinax-teams-2.0.0/pinax/teams/urls.py` & `pinax-teams-3.0.0/pinax/teams/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from django.conf.urls import url
+from django.urls import re_path
 
 from . import views
 
 app_name = "pinax_teams"
 
 
 urlpatterns = [
     # overall
-    url(r"^$", views.TeamListView.as_view(), name="team_list"),
-    url(r"^:create/$", views.TeamCreateView.as_view(), name="team_create"),
+    re_path(r"^$", views.TeamListView.as_view(), name="team_list"),
+    re_path(r"^:create/$", views.TeamCreateView.as_view(), name="team_create"),
 
     # team specific
-    url(r"^(?P<slug>[\w\-]+)/$", views.team_detail, name="team_detail"),
-    url(r"^(?P<slug>[\w\-]+)/join/$", views.team_join, name="team_join"),
-    url(r"^(?P<slug>[\w\-]+)/leave/$", views.team_leave, name="team_leave"),
-    url(r"^(?P<slug>[\w\-]+)/apply/$", views.team_apply, name="team_apply"),
-    url(r"^(?P<slug>[\w\-]+)/edit/$", views.team_update, name="team_edit"),
-    url(r"^(?P<slug>[\w\-]+)/manage/$", views.TeamManageView.as_view(), name="team_manage"),
+    re_path(r"^(?P<slug>[\w\-]+)/$", views.team_detail, name="team_detail"),
+    re_path(r"^(?P<slug>[\w\-]+)/join/$", views.team_join, name="team_join"),
+    re_path(r"^(?P<slug>[\w\-]+)/leave/$", views.team_leave, name="team_leave"),
+    re_path(r"^(?P<slug>[\w\-]+)/apply/$", views.team_apply, name="team_apply"),
+    re_path(r"^(?P<slug>[\w\-]+)/edit/$", views.team_update, name="team_edit"),
+    re_path(r"^(?P<slug>[\w\-]+)/manage/$", views.TeamManageView.as_view(), name="team_manage"),
 
     # membership specific
-    url(r"^(?P<slug>[\w\-]+)/ac/users-to-invite/$", views.autocomplete_users, name="team_autocomplete_users"),  # noqa
-    url(r"^(?P<slug>[\w\-]+)/invite-user/$", views.TeamInviteView.as_view(), name="team_invite"),
-    url(r"^(?P<slug>[\w\-]+)/members/(?P<pk>\d+)/revoke-invite/$", views.team_member_revoke_invite, name="team_member_revoke_invite"),  # noqa
-    url(r"^(?P<slug>[\w\-]+)/members/(?P<pk>\d+)/resend-invite/$", views.team_member_resend_invite, name="team_member_resend_invite"),  # noqa
-    url(r"^(?P<slug>[\w\-]+)/members/(?P<pk>\d+)/promote/$", views.team_member_promote, name="team_member_promote"),  # noqa
-    url(r"^(?P<slug>[\w\-]+)/members/(?P<pk>\d+)/demote/$", views.team_member_demote, name="team_member_demote"),  # noqa
-    url(r"^(?P<slug>[\w\-]+)/members/(?P<pk>\d+)/remove/$", views.team_member_remove, name="team_member_remove"),  # noqa
+    re_path(r"^(?P<slug>[\w\-]+)/ac/users-to-invite/$", views.autocomplete_users, name="team_autocomplete_users"),  # noqa
+    re_path(r"^(?P<slug>[\w\-]+)/invite-user/$", views.TeamInviteView.as_view(), name="team_invite"),
+    re_path(r"^(?P<slug>[\w\-]+)/members/(?P<pk>\d+)/revoke-invite/$", views.team_member_revoke_invite, name="team_member_revoke_invite"),  # noqa
+    re_path(r"^(?P<slug>[\w\-]+)/members/(?P<pk>\d+)/resend-invite/$", views.team_member_resend_invite, name="team_member_resend_invite"),  # noqa
+    re_path(r"^(?P<slug>[\w\-]+)/members/(?P<pk>\d+)/promote/$", views.team_member_promote, name="team_member_promote"),  # noqa
+    re_path(r"^(?P<slug>[\w\-]+)/members/(?P<pk>\d+)/demote/$", views.team_member_demote, name="team_member_demote"),  # noqa
+    re_path(r"^(?P<slug>[\w\-]+)/members/(?P<pk>\d+)/remove/$", views.team_member_remove, name="team_member_remove"),  # noqa
 
-    url(r"^accept/(?P<pk>\d+)/$", views.team_accept, name="team_accept"),
-    url(r"^reject/(?P<pk>\d+)/$", views.team_reject, name="team_reject"),
+    re_path(r"^accept/(?P<pk>\d+)/$", views.team_accept, name="team_accept"),
+    re_path(r"^reject/(?P<pk>\d+)/$", views.team_reject, name="team_reject"),
 ]
```

### Comparing `pinax-teams-2.0.0/pinax/teams/utils.py` & `pinax-teams-3.0.0/pinax/teams/utils.py`

 * *Files identical despite different names*

### Comparing `pinax-teams-2.0.0/pinax/teams/views.py` & `pinax-teams-3.0.0/pinax/teams/views.py`

 * *Files identical despite different names*

### Comparing `pinax-teams-2.0.0/pinax/teams/wsgi_middleware.py` & `pinax-teams-3.0.0/pinax/teams/wsgi_middleware.py`

 * *Files identical despite different names*

### Comparing `pinax-teams-2.0.0/pinax_teams.egg-info/PKG-INFO` & `pinax-teams-3.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,70 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pinax-teams
-Version: 2.0.0
+Version: 3.0.0
 Summary: An app for Django sites that supports open, by invitation, and by application teams
 Home-page: http://github.com/pinax/pinax-teams/
 Author: Pinax Team
 Author-email: team@pinaxproject.com
 License: MIT
-Description: 
-        .. image:: http://pinaxproject.com/pinax-design/patches/pinax-teams.svg
-            :target: https://pypi.python.org/pypi/pinax-teams/
-        
-        ===========
-        Pinax Teams
-        ===========
-        
-        .. image:: https://img.shields.io/pypi/v/pinax-teams.svg
-            :target: https://pypi.python.org/pypi/pinax-teams/
-        
-        \ 
-        
-        .. image:: https://img.shields.io/circleci/project/github/pinax/pinax-teams.svg
-            :target: https://circleci.com/gh/pinax/pinax-teams
-        .. image:: https://img.shields.io/codecov/c/github/pinax/pinax-teams.svg
-            :target: https://codecov.io/gh/pinax/pinax-teams
-        .. image:: https://img.shields.io/github/contributors/pinax/pinax-teams.svg
-            :target: https://github.com/pinax/pinax-teams/graphs/contributors
-        .. image:: https://img.shields.io/github/issues-pr/pinax/pinax-teams.svg
-            :target: https://github.com/pinax/pinax-teams/pulls
-        .. image:: https://img.shields.io/github/issues-pr-closed/pinax/pinax-teams.svg
-            :target: https://github.com/pinax/pinax-teams/pulls?q=is%3Apr+is%3Aclosed
-        
-        \ 
-        
-        .. image:: http://slack.pinaxproject.com/badge.svg
-            :target: http://slack.pinaxproject.com/
-        .. image:: https://img.shields.io/badge/license-MIT-blue.svg
-            :target: https://pypi.python.org/pypi/pinax-teams/
-        
-        \ 
-        
-        ``pinax-teams`` is an app for Django sites that supports open, by invitation, and by application teams.
-        
-        Supported Django and Python Versions
-        ------------------------------------
-        
-        +-----------------+-----+-----+-----+
-        | Django / Python | 3.6 | 3.7 | 3.8 |
-        +=================+=====+=====+=====+
-        |  2.2            |  *  |  *  |  *  |
-        +-----------------+-----+-----+-----+
-        |  3.0            |  *  |  *  |  *  |
-        +-----------------+-----+-----+-----+
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+License-File: LICENSE
+License-File: AUTHORS
+
+
+.. image:: http://pinaxproject.com/pinax-design/patches/pinax-teams.svg
+    :target: https://pypi.python.org/pypi/pinax-teams/
+
+===========
+Pinax Teams
+===========
+
+.. image:: https://img.shields.io/pypi/v/pinax-teams.svg
+    :target: https://pypi.python.org/pypi/pinax-teams/
+
+\ 
+
+.. image:: https://img.shields.io/circleci/project/github/pinax/pinax-teams.svg
+    :target: https://circleci.com/gh/pinax/pinax-teams
+.. image:: https://img.shields.io/codecov/c/github/pinax/pinax-teams.svg
+    :target: https://codecov.io/gh/pinax/pinax-teams
+.. image:: https://img.shields.io/github/contributors/pinax/pinax-teams.svg
+    :target: https://github.com/pinax/pinax-teams/graphs/contributors
+.. image:: https://img.shields.io/github/issues-pr/pinax/pinax-teams.svg
+    :target: https://github.com/pinax/pinax-teams/pulls
+.. image:: https://img.shields.io/github/issues-pr-closed/pinax/pinax-teams.svg
+    :target: https://github.com/pinax/pinax-teams/pulls?q=is%3Apr+is%3Aclosed
+
+\ 
+
+.. image:: http://slack.pinaxproject.com/badge.svg
+    :target: http://slack.pinaxproject.com/
+.. image:: https://img.shields.io/badge/license-MIT-blue.svg
+    :target: https://pypi.python.org/pypi/pinax-teams/
+
+\ 
+
+``pinax-teams`` is an app for Django sites that supports open, by invitation, and by application teams.
+
+Supported Django and Python Versions
+------------------------------------
+
++-----------------+-----+-----+-----+-----+
+| Django / Python | 3.7 | 3.8 | 3.9 | 3.10|
++=================+=====+=====+=====+=====+
+|  3.2            |  *  |  *  |  *  |  *  |
++-----------------+-----+-----+-----+-----+
+|  4.1            |  -  |  -  |  -  |  *  |
++-----------------+-----+-----+-----+-----+
```

### Comparing `pinax-teams-2.0.0/pinax_teams.egg-info/SOURCES.txt` & `pinax-teams-3.0.0/pinax_teams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

