# Comparing `tmp/aa-opcalendar-2.3.1.tar.gz` & `tmp/aa-opcalendar-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-opcalendar-2.3.1.tar", last modified: Wed Mar 22 16:21:15 2023, max compression
+gzip compressed data, was "aa-opcalendar-2.4.0.tar", last modified: Sun Apr 16 09:12:25 2023, max compression
```

## Comparing `aa-opcalendar-2.3.1.tar` & `aa-opcalendar-2.4.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 16:21:15.090292 aa-opcalendar-2.3.1/
--rwxr-xr-x   0 root         (0) root         (0)     1070 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/LICENSE
--rwxr-xr-x   0 root         (0) root         (0)      179 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10967 2023-03-22 16:21:15.090292 aa-opcalendar-2.3.1/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    10205 2022-05-22 08:49:24.000000 aa-opcalendar-2.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 16:21:15.086292 aa-opcalendar-2.3.1/aa_opcalendar.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10967 2023-03-22 16:21:15.000000 aa-opcalendar-2.3.1/aa_opcalendar.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2904 2023-03-22 16:21:15.000000 aa-opcalendar-2.3.1/aa_opcalendar.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-22 16:21:15.000000 aa-opcalendar-2.3.1/aa_opcalendar.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-03-22 16:21:15.000000 aa-opcalendar-2.3.1/aa_opcalendar.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-03-22 16:21:15.000000 aa-opcalendar-2.3.1/aa_opcalendar.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 16:21:15.086292 aa-opcalendar-2.3.1/eventcalendar/
--rwxr-xr-x   0 root         (0) root         (0)        0 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/eventcalendar/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      403 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/eventcalendar/asgi.py
--rwxr-xr-x   0 root         (0) root         (0)      453 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/eventcalendar/helper.py
--rwxr-xr-x   0 root         (0) root         (0)     3217 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/eventcalendar/settings.py
--rwxr-xr-x   0 root         (0) root         (0)      938 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/eventcalendar/urls.py
--rwxr-xr-x   0 root         (0) root         (0)      747 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/eventcalendar/views.py
--rwxr-xr-x   0 root         (0) root         (0)      403 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/eventcalendar/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 16:21:15.086292 aa-opcalendar-2.3.1/opcalendar/
--rwxr-xr-x   0 root         (0) root         (0)      104 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     3814 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/opcalendar/admin.py
--rwxr-xr-x   0 root         (0) root         (0)     3188 2022-05-22 08:49:24.000000 aa-opcalendar-2.3.1/opcalendar/app_settings.py
--rwxr-xr-x   0 root         (0) root         (0)      165 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/opcalendar/apps.py
--rwxr-xr-x   0 root         (0) root         (0)     1018 2023-03-22 16:13:00.000000 aa-opcalendar-2.3.1/opcalendar/auth_hooks.py
--rwxr-xr-x   0 root         (0) root         (0)    10322 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/calendar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 16:21:15.086292 aa-opcalendar-2.3.1/opcalendar/cogs/
--rwxr-xr-x   0 root         (0) root         (0)     6546 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/opcalendar/cogs/ops.py
--rwxr-xr-x   0 root         (0) root         (0)      553 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/opcalendar/decorators.py
--rwxr-xr-x   0 root         (0) root         (0)     3320 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/opcalendar/forms.py
--rwxr-xr-x   0 root         (0) root         (0)      772 2023-03-22 16:13:00.000000 aa-opcalendar-2.3.1/opcalendar/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 16:21:15.090292 aa-opcalendar-2.3.1/opcalendar/migrations/
--rwxr-xr-x   0 root         (0) root         (0)     7318 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0001_initial.py
--rwxr-xr-x   0 root         (0) root         (0)      769 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0002_auto_20201104_1054.py
--rwxr-xr-x   0 root         (0) root         (0)      827 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0003_eventhost.py
--rwxr-xr-x   0 root         (0) root         (0)      539 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0004_event_host.py
--rwxr-xr-x   0 root         (0) root         (0)      569 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0005_auto_20201104_1127.py
--rwxr-xr-x   0 root         (0) root         (0)     1946 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0006_auto_20201104_1201.py
--rwxr-xr-x   0 root         (0) root         (0)      403 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0007_eventhost_twitter.py
--rwxr-xr-x   0 root         (0) root         (0)      358 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0008_auto_20201105_0846.py
--rwxr-xr-x   0 root         (0) root         (0)      913 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0009_auto_20201105_0859.py
--rwxr-xr-x   0 root         (0) root         (0)      635 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0010_auto_20201105_1602.py
--rwxr-xr-x   0 root         (0) root         (0)     1568 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0011_eventimport.py
--rwxr-xr-x   0 root         (0) root         (0)      576 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0012_auto_20210112_0934.py
--rwxr-xr-x   0 root         (0) root         (0)      661 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0013_eventimport_creator.py
--rwxr-xr-x   0 root         (0) root         (0)     1957 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0014_auto_20210113_0836.py
--rwxr-xr-x   0 root         (0) root         (0)      671 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0015_eventimport_eve_character.py
--rwxr-xr-x   0 root         (0) root         (0)     4088 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0016_auto_20210119_1545.py
--rwxr-xr-x   0 root         (0) root         (0)     1295 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0017_auto_20210119_1626.py
--rwxr-xr-x   0 root         (0) root         (0)      684 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0018_auto_20210119_1701.py
--rwxr-xr-x   0 root         (0) root         (0)      708 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0019_auto_20210125_1005.py
--rwxr-xr-x   0 root         (0) root         (0)      459 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0020_auto_20210125_1007.py
--rwxr-xr-x   0 root         (0) root         (0)      404 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0021_eventhost_logo_url.py
--rwxr-xr-x   0 root         (0) root         (0)     2983 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0022_auto_20210222_1255.py
--rwxr-xr-x   0 root         (0) root         (0)    13049 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0023_auto_20210330_0632.py
--rwxr-xr-x   0 root         (0) root         (0)     2617 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0024_auto_20210429_1111.py
--rw-r--r--   0 root         (0) root         (0)      995 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0025_auto_20220115_1101.py
--rw-r--r--   0 root         (0) root         (0)      791 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/migrations/0026_alter_event_repeat_event.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/opcalendar/migrations/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    25244 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/models.py
--rwxr-xr-x   0 root         (0) root         (0)      374 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/opcalendar/providers.py
--rwxr-xr-x   0 root         (0) root         (0)    17736 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 16:21:15.082292 aa-opcalendar-2.3.1/opcalendar/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 16:21:15.090292 aa-opcalendar-2.3.1/opcalendar/static/opcalendar/
--rwxr-xr-x   0 root         (0) root         (0)     1204 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/opcalendar/static/opcalendar/calendar.png
--rwxr-xr-x   0 root         (0) root         (0)     2845 2022-05-22 08:49:24.000000 aa-opcalendar-2.3.1/opcalendar/static/opcalendar/style_dark.css
--rw-r--r--   0 root         (0) root         (0)     2861 2022-05-22 08:49:24.000000 aa-opcalendar-2.3.1/opcalendar/static/opcalendar/style_light.css
--rwxr-xr-x   0 root         (0) root         (0)     1379 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/opcalendar/static/opcalendar/terminate.png
--rwxr-xr-x   0 root         (0) root         (0)   947196 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/opcalendar/swagger.json
--rwxr-xr-x   0 root         (0) root         (0)    14478 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 16:21:15.082292 aa-opcalendar-2.3.1/opcalendar/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 16:21:15.090292 aa-opcalendar-2.3.1/opcalendar/templates/opcalendar/
--rwxr-xr-x   0 root         (0) root         (0)      448 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/opcalendar/templates/opcalendar/add_member.html
--rwxr-xr-x   0 root         (0) root         (0)     1194 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/opcalendar/templates/opcalendar/base.html
--rwxr-xr-x   0 root         (0) root         (0)     3745 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/opcalendar/templates/opcalendar/calendar.html
--rwxr-xr-x   0 root         (0) root         (0)     1751 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/opcalendar/templates/opcalendar/event-add.html
--rwxr-xr-x   0 root         (0) root         (0)    10057 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/opcalendar/templates/opcalendar/event-details.html
--rwxr-xr-x   0 root         (0) root         (0)     1219 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/opcalendar/templates/opcalendar/event-edit.html
--rwxr-xr-x   0 root         (0) root         (0)      384 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/opcalendar/templates/opcalendar/event_delete.html
--rwxr-xr-x   0 root         (0) root         (0)     4780 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/opcalendar/templates/opcalendar/ingame-event-details.html
--rwxr-xr-x   0 root         (0) root         (0)      400 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/opcalendar/templates/opcalendar/signup.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 16:21:15.090292 aa-opcalendar-2.3.1/opcalendar/tests/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 16:13:00.000000 aa-opcalendar-2.3.1/opcalendar/tests/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4316 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/tests/test_models.py
--rwxr-xr-x   0 root         (0) root         (0)    20000 2023-03-22 16:13:00.000000 aa-opcalendar-2.3.1/opcalendar/tests/test_tasks.py
--rwxr-xr-x   0 root         (0) root         (0)     2875 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/tests/testdata.py
--rwxr-xr-x   0 root         (0) root         (0)     1246 2023-03-22 16:13:00.000000 aa-opcalendar-2.3.1/opcalendar/urls.py
--rwxr-xr-x   0 root         (0) root         (0)    10257 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/utils.py
--rwxr-xr-x   0 root         (0) root         (0)    16275 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/opcalendar/views.py
--rwxr-xr-x   0 root         (0) root         (0)      187 2023-03-22 16:21:15.094292 aa-opcalendar-2.3.1/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1485 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-22 16:21:15.090292 aa-opcalendar-2.3.1/testauth/
--rwxr-xr-x   0 root         (0) root         (0)       46 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/testauth/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      611 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/testauth/celery.py
--rwxr-xr-x   0 root         (0) root         (0)     9946 2023-03-22 16:19:10.000000 aa-opcalendar-2.3.1/testauth/settings.py
--rwxr-xr-x   0 root         (0) root         (0)      120 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/testauth/urls.py
--rwxr-xr-x   0 root         (0) root         (0)      397 2022-05-22 08:26:00.000000 aa-opcalendar-2.3.1/testauth/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.591395 aa-opcalendar-2.4.0/
+-rwxr-xr-x   0 root         (0) root         (0)     1070 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/LICENSE
+-rwxr-xr-x   0 root         (0) root         (0)      179 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10967 2023-04-16 09:12:25.591395 aa-opcalendar-2.4.0/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    10205 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.567399 aa-opcalendar-2.4.0/aa_opcalendar.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10967 2023-04-16 09:12:25.000000 aa-opcalendar-2.4.0/aa_opcalendar.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2904 2023-04-16 09:12:25.000000 aa-opcalendar-2.4.0/aa_opcalendar.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 09:12:25.000000 aa-opcalendar-2.4.0/aa_opcalendar.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-04-16 09:12:25.000000 aa-opcalendar-2.4.0/aa_opcalendar.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-04-16 09:12:25.000000 aa-opcalendar-2.4.0/aa_opcalendar.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.567399 aa-opcalendar-2.4.0/eventcalendar/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/eventcalendar/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      403 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/eventcalendar/asgi.py
+-rwxr-xr-x   0 root         (0) root         (0)      453 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/eventcalendar/helper.py
+-rwxr-xr-x   0 root         (0) root         (0)     3217 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/eventcalendar/settings.py
+-rwxr-xr-x   0 root         (0) root         (0)      938 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/eventcalendar/urls.py
+-rwxr-xr-x   0 root         (0) root         (0)      747 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/eventcalendar/views.py
+-rwxr-xr-x   0 root         (0) root         (0)      403 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/eventcalendar/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.567399 aa-opcalendar-2.4.0/opcalendar/
+-rwxr-xr-x   0 root         (0) root         (0)      104 2023-04-16 09:09:21.000000 aa-opcalendar-2.4.0/opcalendar/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     3814 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/admin.py
+-rwxr-xr-x   0 root         (0) root         (0)     3188 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/app_settings.py
+-rwxr-xr-x   0 root         (0) root         (0)      165 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/apps.py
+-rwxr-xr-x   0 root         (0) root         (0)     1018 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/auth_hooks.py
+-rwxr-xr-x   0 root         (0) root         (0)    10322 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/calendar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.567399 aa-opcalendar-2.4.0/opcalendar/cogs/
+-rwxr-xr-x   0 root         (0) root         (0)     6898 2023-04-16 09:09:21.000000 aa-opcalendar-2.4.0/opcalendar/cogs/ops.py
+-rwxr-xr-x   0 root         (0) root         (0)      553 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/decorators.py
+-rwxr-xr-x   0 root         (0) root         (0)     3320 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/forms.py
+-rwxr-xr-x   0 root         (0) root         (0)      772 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.587395 aa-opcalendar-2.4.0/opcalendar/migrations/
+-rwxr-xr-x   0 root         (0) root         (0)     7318 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0001_initial.py
+-rwxr-xr-x   0 root         (0) root         (0)      769 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0002_auto_20201104_1054.py
+-rwxr-xr-x   0 root         (0) root         (0)      827 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0003_eventhost.py
+-rwxr-xr-x   0 root         (0) root         (0)      539 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0004_event_host.py
+-rwxr-xr-x   0 root         (0) root         (0)      569 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0005_auto_20201104_1127.py
+-rwxr-xr-x   0 root         (0) root         (0)     1946 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0006_auto_20201104_1201.py
+-rwxr-xr-x   0 root         (0) root         (0)      403 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0007_eventhost_twitter.py
+-rwxr-xr-x   0 root         (0) root         (0)      358 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0008_auto_20201105_0846.py
+-rwxr-xr-x   0 root         (0) root         (0)      913 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0009_auto_20201105_0859.py
+-rwxr-xr-x   0 root         (0) root         (0)      635 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0010_auto_20201105_1602.py
+-rwxr-xr-x   0 root         (0) root         (0)     1568 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0011_eventimport.py
+-rwxr-xr-x   0 root         (0) root         (0)      576 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0012_auto_20210112_0934.py
+-rwxr-xr-x   0 root         (0) root         (0)      661 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0013_eventimport_creator.py
+-rwxr-xr-x   0 root         (0) root         (0)     1957 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0014_auto_20210113_0836.py
+-rwxr-xr-x   0 root         (0) root         (0)      671 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0015_eventimport_eve_character.py
+-rwxr-xr-x   0 root         (0) root         (0)     4088 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0016_auto_20210119_1545.py
+-rwxr-xr-x   0 root         (0) root         (0)     1295 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0017_auto_20210119_1626.py
+-rwxr-xr-x   0 root         (0) root         (0)      684 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0018_auto_20210119_1701.py
+-rwxr-xr-x   0 root         (0) root         (0)      708 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0019_auto_20210125_1005.py
+-rwxr-xr-x   0 root         (0) root         (0)      459 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0020_auto_20210125_1007.py
+-rwxr-xr-x   0 root         (0) root         (0)      404 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0021_eventhost_logo_url.py
+-rwxr-xr-x   0 root         (0) root         (0)     2983 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0022_auto_20210222_1255.py
+-rwxr-xr-x   0 root         (0) root         (0)    13049 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0023_auto_20210330_0632.py
+-rwxr-xr-x   0 root         (0) root         (0)     2617 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0024_auto_20210429_1111.py
+-rw-r--r--   0 root         (0) root         (0)      995 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0025_auto_20220115_1101.py
+-rw-r--r--   0 root         (0) root         (0)      791 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0026_alter_event_repeat_event.py
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    25244 2023-04-16 09:07:24.000000 aa-opcalendar-2.4.0/opcalendar/models.py
+-rwxr-xr-x   0 root         (0) root         (0)      374 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/providers.py
+-rwxr-xr-x   0 root         (0) root         (0)    17736 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.567399 aa-opcalendar-2.4.0/opcalendar/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.591395 aa-opcalendar-2.4.0/opcalendar/static/opcalendar/
+-rwxr-xr-x   0 root         (0) root         (0)     1204 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/static/opcalendar/calendar.png
+-rwxr-xr-x   0 root         (0) root         (0)     2845 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/static/opcalendar/style_dark.css
+-rw-r--r--   0 root         (0) root         (0)     2861 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/static/opcalendar/style_light.css
+-rwxr-xr-x   0 root         (0) root         (0)     1379 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/static/opcalendar/terminate.png
+-rwxr-xr-x   0 root         (0) root         (0)   947196 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/swagger.json
+-rwxr-xr-x   0 root         (0) root         (0)    14478 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.567399 aa-opcalendar-2.4.0/opcalendar/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.591395 aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/
+-rwxr-xr-x   0 root         (0) root         (0)      448 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/add_member.html
+-rwxr-xr-x   0 root         (0) root         (0)     1194 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/base.html
+-rwxr-xr-x   0 root         (0) root         (0)     3745 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/calendar.html
+-rwxr-xr-x   0 root         (0) root         (0)     1751 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/event-add.html
+-rwxr-xr-x   0 root         (0) root         (0)    10057 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/event-details.html
+-rwxr-xr-x   0 root         (0) root         (0)     1219 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/event-edit.html
+-rwxr-xr-x   0 root         (0) root         (0)      384 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/event_delete.html
+-rwxr-xr-x   0 root         (0) root         (0)     4780 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/ingame-event-details.html
+-rwxr-xr-x   0 root         (0) root         (0)      400 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/signup.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.591395 aa-opcalendar-2.4.0/opcalendar/tests/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/tests/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4316 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/tests/test_models.py
+-rwxr-xr-x   0 root         (0) root         (0)    20000 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/tests/test_tasks.py
+-rwxr-xr-x   0 root         (0) root         (0)     2875 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/tests/testdata.py
+-rwxr-xr-x   0 root         (0) root         (0)     1246 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/urls.py
+-rwxr-xr-x   0 root         (0) root         (0)    10257 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    16275 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/views.py
+-rwxr-xr-x   0 root         (0) root         (0)      187 2023-04-16 09:12:25.591395 aa-opcalendar-2.4.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1485 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.591395 aa-opcalendar-2.4.0/testauth/
+-rwxr-xr-x   0 root         (0) root         (0)       46 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/testauth/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      611 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/testauth/celery.py
+-rwxr-xr-x   0 root         (0) root         (0)     9946 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/testauth/settings.py
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/testauth/urls.py
+-rwxr-xr-x   0 root         (0) root         (0)      397 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/testauth/wsgi.py
```

### Comparing `aa-opcalendar-2.3.1/LICENSE` & `aa-opcalendar-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/PKG-INFO` & `aa-opcalendar-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-opcalendar
-Version: 2.3.1
+Version: 2.4.0
 Summary: Event calendar plugin app for Alliance Auth
 Home-page: https://gitlab.com/paulipa/allianceauth-opcalendar
 Author: Ikarus Cesaille
 Author-email: contact@eve-linknet.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `aa-opcalendar-2.3.1/README.md` & `aa-opcalendar-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/aa_opcalendar.egg-info/PKG-INFO` & `aa-opcalendar-2.4.0/aa_opcalendar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-opcalendar
-Version: 2.3.1
+Version: 2.4.0
 Summary: Event calendar plugin app for Alliance Auth
 Home-page: https://gitlab.com/paulipa/allianceauth-opcalendar
 Author: Ikarus Cesaille
 Author-email: contact@eve-linknet.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `aa-opcalendar-2.3.1/aa_opcalendar.egg-info/SOURCES.txt` & `aa-opcalendar-2.4.0/aa_opcalendar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/eventcalendar/settings.py` & `aa-opcalendar-2.4.0/eventcalendar/settings.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/eventcalendar/urls.py` & `aa-opcalendar-2.4.0/eventcalendar/urls.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/eventcalendar/views.py` & `aa-opcalendar-2.4.0/eventcalendar/views.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/admin.py` & `aa-opcalendar-2.4.0/opcalendar/admin.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/app_settings.py` & `aa-opcalendar-2.4.0/opcalendar/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/auth_hooks.py` & `aa-opcalendar-2.4.0/opcalendar/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/calendar.py` & `aa-opcalendar-2.4.0/opcalendar/calendar.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/cogs/ops.py` & `aa-opcalendar-2.4.0/opcalendar/cogs/ops.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Cog Stuff
 from discord.ext import commands
 from discord.embeds import Embed
 from discord.colour import Color
+from discord.commands import Option
 
 # AA Contexts
 from aadiscordbot.app_settings import get_site_url
 from allianceauth.services.modules.discord.models import DiscordUser
 
 # OPCALENDAR
 import operator
@@ -14,186 +15,222 @@
 from itertools import chain
 from app_utils.urls import static_file_absolute_url
 from datetime import datetime
 import os
 
 import logging
 
+from django.conf import settings
 from opcalendar.app_settings import (
     OPCALENDAR_DISCORD_OPS_DISPLAY_EXTERNAL,
 )
 
 logger = logging.getLogger(__name__)
 
 # i dont want to do this, but the below object get wont work without it, investigate.
 os.environ["DJANGO_ALLOW_ASYNC_UNSAFE"] = "true"
 
 
 class Ops(commands.Cog):
     """
-    A Collection of Authentication Tools for Alliance Auth
+    Return upcoming events as a discord DM
     """
 
     def __init__(self, bot):
         self.bot = bot
 
+    hosts = EventHost.objects.all().values_list("community", flat=True)
+
     @commands.command(pass_context=True)
     async def ops(self, ctx):
         """
         Sends a direct message about the upcoming events visible for the user
         """
         await ctx.trigger_typing()
 
         # Get authod ID
-        id = ctx.message.author.id
-
-        url = get_site_url()
-
-        today = datetime.today()
+        author_id = ctx.message.author.id
 
         user_argument = ctx.message.content[5:]
 
-        if not user_argument:
-            host = "all hosts"
+        embed = _get_events(author_id, user_argument)
 
-        else:
-            host = user_argument
+        await ctx.author.send(embed=embed)
 
-        # Get user if discord service is active
-        try:
-            discord_user = DiscordUser.objects.get(uid=id)
+        confirm = _confirm_ops_in_channel()
 
-            user = discord_user.user
+        return await ctx.reply(embed=confirm)
 
-            discord_active = True
+    @commands.slash_command(name="ops", guild_ids=[int(settings.DISCORD_GUILD_ID)])
+    async def ops_slash(
+        self,
+        ctx,
+        host: Option(
+            str,
+            choices=hosts,
+            required=False,
+        ),
+    ):
+        """
+        Get upcoming events as DM. Can be filtered by hosts (optional)
+        """
 
-        except Exception:
-            logger.error("Discord service is not active for user")
+        # Get attributes
+        author_id = ctx.author.id
 
-            embed = Embed(title="Command failed")
-            embed.colour = Color.red()
-            embed.set_thumbnail(
-                url=static_file_absolute_url("opcalendar/terminate.png")
-            )
-            embed.description = "Activate the [discord service]({}/services) to access this command.".format(
-                url
-            )
-            discord_active = False
+        user_argument = host
 
-            await ctx.reply(embed=embed)
+        embed = _get_events(author_id, user_argument)
 
-        if discord_active:
-            # Get normal events
-            # Filter by groups and states
-            events = (
-                Event.objects.filter(
-                    Q(event_visibility__restricted_to_group__in=user.groups.all())
-                    | Q(event_visibility__restricted_to_group__isnull=True),
-                )
-                .filter(
-                    Q(event_visibility__restricted_to_state=user.profile.state)
-                    | Q(event_visibility__restricted_to_state__isnull=True),
-                )
-                .filter(start_time__gte=today)
-            )
-            if user_argument:
-                events = events.filter(host__community=host)
+        await ctx.author.send(embed=embed)
 
-            # Get ingame events
-            # Filter by groups and states
-            ingame_events = (
-                IngameEvents.objects.annotate(
-                    start_time=F("event_start_date"),
-                    end_time=F("event_end_date"),
-                )
-                .filter(
-                    Q(
-                        owner__event_visibility__restricted_to_group__in=user.groups.all()
-                    )
-                    | Q(owner__event_visibility__restricted_to_group__isnull=True),
-                )
-                .filter(
-                    Q(owner__event_visibility__restricted_to_state=user.profile.state)
-                    | Q(owner__event_visibility__restricted_to_state__isnull=True),
-                )
-                .filter(start_time__gte=today)
-            )
+        confirm = _confirm_ops_in_channel()
 
-            hosts = EventHost.objects.all()
+        return await ctx.respond(embed=confirm)
 
-            if not OPCALENDAR_DISCORD_OPS_DISPLAY_EXTERNAL:
-                hosts = hosts.filter(external=False)
 
-            hosts = _hosts(hosts)
+def _hosts(hosts):
+    hosts = [x.community for x in hosts]
+
+    if hosts:
+        return ", ".join(hosts)
+    else:
+        return None
 
-            if user_argument:
-                ingame_events = ingame_events.filter(host__community=host)
 
-            # Combine events, limit to 10 events
-            all_events = sorted(
-                chain(events, ingame_events),
-                key=operator.attrgetter("start_time"),
-            )[:10]
+def _get_events(author, user_argument):
+    url = get_site_url()
 
-            embed = Embed(title="Scheduled Opcalendar Events")
+    today = datetime.today()
 
-            embed.set_thumbnail(url=static_file_absolute_url("opcalendar/calendar.png"))
+    if not user_argument:
+        host = "all hosts"
 
-            embed.colour = Color.blue()
+    else:
+        host = user_argument
 
-            embed.description = "List view of the next 10 upcoming operations for {}. A calendar view is located in [here]({}/opcalendar).\n\nFiltering: To filter events for a specific host add the name after the command ie. `!ops my coalition`\n\nAvailable hosts: *{}*".format(
-                host, url, hosts
-            )
+    # Get user if discord service is active
+    try:
+        discord_user = DiscordUser.objects.get(uid=author)
+
+        user = discord_user.user
+
+        discord_active = True
+
+    except Exception:
+        logger.error("Discord service is not active for user")
+
+        embed = Embed(title="Command failed")
+        embed.colour = Color.red()
+        embed.set_thumbnail(url=static_file_absolute_url("opcalendar/terminate.png"))
+        embed.description = "Activate the [discord service]({}/services) to access this command.".format(
+            url
+        )
+        discord_active = False
+
+        return embed
+
+    if discord_active:
+        # Get normal events
+        # Filter by groups and states
+        events = (
+            Event.objects.filter(
+                Q(event_visibility__restricted_to_group__in=user.groups.all())
+                | Q(event_visibility__restricted_to_group__isnull=True),
+            )
+            .filter(
+                Q(event_visibility__restricted_to_state=user.profile.state)
+                | Q(event_visibility__restricted_to_state__isnull=True),
+            )
+            .filter(start_time__gte=today)
+        )
+        if user_argument:
+            events = events.filter(host__community=host)
+
+        # Get ingame events
+        # Filter by groups and states
+        ingame_events = (
+            IngameEvents.objects.annotate(
+                start_time=F("event_start_date"),
+                end_time=F("event_end_date"),
+            )
+            .filter(
+                Q(owner__event_visibility__restricted_to_group__in=user.groups.all())
+                | Q(owner__event_visibility__restricted_to_group__isnull=True),
+            )
+            .filter(
+                Q(owner__event_visibility__restricted_to_state=user.profile.state)
+                | Q(owner__event_visibility__restricted_to_state__isnull=True),
+            )
+            .filter(start_time__gte=today)
+        )
+
+        hosts = EventHost.objects.all()
+
+        if not OPCALENDAR_DISCORD_OPS_DISPLAY_EXTERNAL:
+            hosts = hosts.filter(external=False)
+
+        hosts = _hosts(hosts)
+
+        if user_argument:
+            ingame_events = ingame_events.filter(host__community=host)
+
+        # Combine events, limit to 10 events
+        all_events = sorted(
+            chain(events, ingame_events),
+            key=operator.attrgetter("start_time"),
+        )[:10]
+
+        embed = Embed(title="Scheduled Opcalendar Events")
+
+        embed.set_thumbnail(url=static_file_absolute_url("opcalendar/calendar.png"))
+
+        embed.colour = Color.blue()
+
+        embed.description = "List view of the next 10 upcoming operations for {}. A calendar view is located in [here]({}/opcalendar).\n\nFiltering: To filter events for a specific host add the name after the command ie. `/ops my coalition`\n\nAvailable hosts: *{}*".format(
+            host, url, hosts
+        )
+
+        # Format all events and ingame events
+        for event in all_events:
+            if type(event) == Event:
+                embed.add_field(
+                    name="Event: {0} {1}".format(
+                        event.title, event.operation_type.ticker
+                    ),
+                    value="Host: {0}\nFC: {1}\nDoctrine: {2}\nLocation: {3}\nTime: {4}\n[Details]({5}/opcalendar/event/{6}/details/)\n".format(
+                        event.host,
+                        event.fc,
+                        event.doctrine,
+                        event.formup_system,
+                        event.start_time,
+                        url,
+                        event.id,
+                    ),
+                    inline=False,
+                )
+            if type(event) == IngameEvents:
+                embed.add_field(
+                    name="Ingame Event: {0}".format(event.title),
+                    value="Host: {0}\n Time:{1}\n[Details]({2}/opcalendar/ingame/event/{3}/details/)".format(
+                        event.owner_name,
+                        event.start_time,
+                        url,
+                        event.event_id,
+                    ),
+                    inline=False,
+                )
 
-            # Format all events and ingame events
-            for event in all_events:
-                if type(event) == Event:
-                    embed.add_field(
-                        name="Event: {0} {1}".format(
-                            event.title, event.operation_type.ticker
-                        ),
-                        value="Host: {0}\nFC: {1}\nDoctrine: {2}\nLocation: {3}\nTime: {4}\n[Details]({5}/opcalendar/event/{6}/details/)\n".format(
-                            event.host,
-                            event.fc,
-                            event.doctrine,
-                            event.formup_system,
-                            event.start_time,
-                            url,
-                            event.id,
-                        ),
-                        inline=False,
-                    )
-                if type(event) == IngameEvents:
-                    embed.add_field(
-                        name="Ingame Event: {0}".format(event.title),
-                        value="Host: {0}\n Time:{1}\n[Details]({2}/opcalendar/ingame/event/{3}/details/)".format(
-                            event.owner_name,
-                            event.start_time,
-                            url,
-                            event.event_id,
-                        ),
-                        inline=False,
-                    )
-
-            await ctx.author.send(embed=embed)
-
-            embed = Embed(title="Events sent")
-            embed.colour = Color.green()
-            embed.description = (
-                "I have sent you a direct message about upcoming events."
-            )
-            discord_active = False
+        discord_active = False
 
-            await ctx.reply(embed=embed)
+        return embed
 
 
-def _hosts(hosts):
-    hosts = [x.community for x in hosts]
+def _confirm_ops_in_channel():
+    embed = Embed(title="Events sent as DM!")
+    embed.colour = Color.green()
 
-    if hosts:
-        return ", ".join(hosts)
-    else:
-        return None
+    return embed
 
 
 def setup(bot):
     bot.add_cog(Ops(bot))
```

### Comparing `aa-opcalendar-2.3.1/opcalendar/decorators.py` & `aa-opcalendar-2.4.0/opcalendar/decorators.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/forms.py` & `aa-opcalendar-2.4.0/opcalendar/forms.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/helpers.py` & `aa-opcalendar-2.4.0/opcalendar/helpers.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0001_initial.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0002_auto_20201104_1054.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0002_auto_20201104_1054.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0003_eventhost.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0003_eventhost.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0004_event_host.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0004_event_host.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0005_auto_20201104_1127.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0005_auto_20201104_1127.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0006_auto_20201104_1201.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0006_auto_20201104_1201.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0009_auto_20201105_0859.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0009_auto_20201105_0859.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0010_auto_20201105_1602.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0010_auto_20201105_1602.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0011_eventimport.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0011_eventimport.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0012_auto_20210112_0934.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0012_auto_20210112_0934.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0013_eventimport_creator.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0013_eventimport_creator.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0014_auto_20210113_0836.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0014_auto_20210113_0836.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0015_eventimport_eve_character.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0015_eventimport_eve_character.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0016_auto_20210119_1545.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0016_auto_20210119_1545.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0017_auto_20210119_1626.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0017_auto_20210119_1626.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0018_auto_20210119_1701.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0018_auto_20210119_1701.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0019_auto_20210125_1005.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0019_auto_20210125_1005.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0022_auto_20210222_1255.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0022_auto_20210222_1255.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0023_auto_20210330_0632.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0023_auto_20210330_0632.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0024_auto_20210429_1111.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0024_auto_20210429_1111.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0025_auto_20220115_1101.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0025_auto_20220115_1101.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/migrations/0026_alter_event_repeat_event.py` & `aa-opcalendar-2.4.0/opcalendar/migrations/0026_alter_event_repeat_event.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/models.py` & `aa-opcalendar-2.4.0/opcalendar/models.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/signals.py` & `aa-opcalendar-2.4.0/opcalendar/signals.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/static/opcalendar/calendar.png` & `aa-opcalendar-2.4.0/opcalendar/static/opcalendar/calendar.png`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/static/opcalendar/style_dark.css` & `aa-opcalendar-2.4.0/opcalendar/static/opcalendar/style_dark.css`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/static/opcalendar/style_light.css` & `aa-opcalendar-2.4.0/opcalendar/static/opcalendar/style_light.css`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/static/opcalendar/terminate.png` & `aa-opcalendar-2.4.0/opcalendar/static/opcalendar/terminate.png`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/swagger.json` & `aa-opcalendar-2.4.0/opcalendar/swagger.json`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/tasks.py` & `aa-opcalendar-2.4.0/opcalendar/tasks.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/templates/opcalendar/base.html` & `aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/base.html`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/templates/opcalendar/calendar.html` & `aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/calendar.html`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/templates/opcalendar/event-add.html` & `aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/event-add.html`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/templates/opcalendar/event-details.html` & `aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/event-details.html`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/templates/opcalendar/event-edit.html` & `aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/event-edit.html`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/templates/opcalendar/ingame-event-details.html` & `aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/ingame-event-details.html`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/tests/test_models.py` & `aa-opcalendar-2.4.0/opcalendar/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/tests/test_tasks.py` & `aa-opcalendar-2.4.0/opcalendar/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/tests/testdata.py` & `aa-opcalendar-2.4.0/opcalendar/tests/testdata.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/urls.py` & `aa-opcalendar-2.4.0/opcalendar/urls.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/utils.py` & `aa-opcalendar-2.4.0/opcalendar/utils.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/opcalendar/views.py` & `aa-opcalendar-2.4.0/opcalendar/views.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/setup.py` & `aa-opcalendar-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/testauth/celery.py` & `aa-opcalendar-2.4.0/testauth/celery.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.3.1/testauth/settings.py` & `aa-opcalendar-2.4.0/testauth/settings.py`

 * *Files identical despite different names*

