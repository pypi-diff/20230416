# Comparing `tmp/aa_discord_announcements-1.0.0.tar.gz` & `tmp/aa_discord_announcements-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_discord_announcements-1.0.0.tar", last modified: Thu Apr 13 15:56:46 2023, max compression
+gzip compressed data, was "aa_discord_announcements-1.1.0.tar", last modified: Sun Apr 16 16:09:35 2023, max compression
```

## Comparing `aa_discord_announcements-1.0.0.tar` & `aa_discord_announcements-1.1.0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.657008 aa_discord_announcements-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-04-13 15:56:46.657008 aa_discord_announcements-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.649008 aa_discord_announcements-1.0.0/aa_discord_announcements/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/app_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.649008 aa_discord_announcements-1.0.0/aa_discord_announcements/helper/
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/helper/announcement_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/helper/discord_webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.641008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.641008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/it_IT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/static/aa_discord_announcements/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/static/aa_discord_announcements/css/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.css
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/static/aa_discord_announcements/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/bundles/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-css.html
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-js.html
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.645008 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/copy-paste-text.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.653008 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.657008 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.657008 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/header/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/header/page-header.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.657008 aa_discord_announcements-1.0.0/aa_discord_announcements/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.657008 aa_discord_announcements-1.0.0/aa_discord_announcements/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_ajax_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_installed_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_templatetags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/aa_discord_announcements/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 15:56:46.649008 aa_discord_announcements-1.0.0/aa_discord_announcements.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-04-13 15:56:46.000000 aa_discord_announcements-1.0.0/aa_discord_announcements.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-13 15:56:46.000000 aa_discord_announcements-1.0.0/aa_discord_announcements.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:56:46.000000 aa_discord_announcements-1.0.0/aa_discord_announcements.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 15:56:46.000000 aa_discord_announcements-1.0.0/aa_discord_announcements.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-13 15:56:46.000000 aa_discord_announcements-1.0.0/aa_discord_announcements.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 15:56:46.000000 aa_discord_announcements-1.0.0/aa_discord_announcements.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 15:56:25.000000 aa_discord_announcements-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-13 15:56:46.657008 aa_discord_announcements-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/helper/announcement_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/helper/discord_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     6492 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/it_IT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/it_IT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/static/aa_discord_announcements/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/aa_discord_announcements/static/aa_discord_announcements/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.css
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/aa_discord_announcements/static/aa_discord_announcements/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/bundles/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-css.html
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-js.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.029473 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/copy-paste-text.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/header/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/header/page-header.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/aa_discord_announcements/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/aa_discord_announcements/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_ajax_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_installed_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_templatetags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/aa_discord_announcements/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:35.033473 aa_discord_announcements-1.1.0/aa_discord_announcements.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-16 16:09:35.000000 aa_discord_announcements-1.1.0/aa_discord_announcements.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-04-16 16:09:35.000000 aa_discord_announcements-1.1.0/aa_discord_announcements.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:09:35.000000 aa_discord_announcements-1.1.0/aa_discord_announcements.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:09:34.000000 aa_discord_announcements-1.1.0/aa_discord_announcements.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-16 16:09:35.000000 aa_discord_announcements-1.1.0/aa_discord_announcements.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-16 16:09:35.000000 aa_discord_announcements-1.1.0/aa_discord_announcements.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 16:09:13.000000 aa_discord_announcements-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-16 16:09:35.037473 aa_discord_announcements-1.1.0/setup.cfg
```

### Comparing `aa_discord_announcements-1.0.0/CHANGELOG.md` & `aa_discord_announcements-1.1.0/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
 
 ## [In Development] - Unreleased
 
 
+## [1.1.0] - 2023-04-16
+
+### Added
+
+- Russian translation
+
+
 ## [1.0.0] - 2023-04-13
 
 ### Added
 
 - German translation
```

### Comparing `aa_discord_announcements-1.0.0/LICENSE` & `aa_discord_announcements-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/PKG-INFO` & `aa_discord_announcements-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa_discord_announcements
-Version: 1.0.0
+Version: 1.1.0
 Summary: Discord Announcements via Alliance Auth. Write announcements and manage who can write announcements on your corporation or alliance Discord through Alliance Auth.
 Home-page: https://github.com/ppfeufer/aa-discord-announcements
 Author: Peter Pfeufer
 Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
@@ -46,67 +46,75 @@
 
 Discord Announcements via [Alliance Auth](https://gitlab.com/allianceauth/allianceauth)
 
 Write announcements and manage who can write announcements on your corporation or
 alliance Discord through Alliance Auth.
 
 
-## Contents
-
-- [Installation](#installation)
-- [Change Log](https://github.com/ppfeufer/aa-discord-announcements/blob/master/CHANGELOG.md)
-- [Code of Conduct](https://github.com/ppfeufer/aa-discord-announcements/blob/master/CODE_OF_CONDUCT.md)
-- [Contribute](https://github.com/ppfeufer/aa-discord-announcements/blob/master/CONTRIBUTING.md)
+<!-- TOC -->
+* [AA Discord Announcements](#aa-discord-announcements)
+  * [Installation](#installation)
+    * [⚠️ Important ⚠️](#-important-)
+    * [Step 1: Install the App](#step-1-install-the-app)
+    * [Step 2: Update Your AA Settings](#step-2-update-your-aa-settings)
+    * [Step 3: Finalizing the Installation](#step-3-finalizing-the-installation)
+    * [Step 4: Setting up Permission](#step-4-setting-up-permission)
+    * [Step 5: Setting up the App](#step-5-setting-up-the-app)
+<!-- TOC -->
 
 
 ## Installation
 
 ### ⚠️ Important ⚠️
 
 This app is a plugin for Alliance Auth. If you don't have Alliance Auth running already,
 please install it first before proceeding.
-(see the official
+(See the official
 [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html)
 for details)
 
 **⚠️ You also want to make sure that you have the
 [Discord service](https://allianceauth.readthedocs.io/en/latest/features/services/discord.html)
 installed, configured and activated before installing this app. ⚠️**
 
-### Step 1 - Install the app
 
-Make sure you are in the virtual environment (venv) of your Alliance Auth installation.
+### Step 1: Install the App
+
+Make sure you're in the virtual environment (venv) of your Alliance Auth installation.
 Then install the latest version:
 
-```bash
+```shell
 pip install aa-discord-announcements
 ```
 
-### Step 2 - Update your AA settings
+
+### Step 2: Update Your AA Settings
 
 Configure your AA settings (`local.py`) as follows:
 
-- Add `'aa_discord_announcements',` to `INSTALLED_APPS`
+- Add `"aa_discord_announcements",` to `INSTALLED_APPS`
 
 
-### Step 3 - Finalize the installation
+### Step 3: Finalizing the Installation
 
 Copy static files and run migrations
 
-```bash
+```shell
 python manage.py collectstatic
 python manage.py migrate
 ```
 
 Restart your supervisor services for AA
 
-### Step 4 - Setup permission
 
-Now you can setup permissions in Alliance Auth for your users.
+### Step 4: Setting up Permission
+
+Now you can set up permissions in Alliance Auth for your users.
 Add `aa_discord_announcements | general | Can access this app` to the states and/or
 groups you would like to have access.
 
-### Step 5 - Setup the app
+
+### Step 5: Setting up the App
 
 In your admin backend you'll find a new section called `Discord Announcements`.
 This is where you set all your stuff up, like the webhooks you want to ping and who
 can ping them. It's pretty straight forward, so you shouldn't have any issues. Go nuts!
```

### Comparing `aa_discord_announcements-1.0.0/README.md` & `aa_discord_announcements-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -15,67 +15,75 @@
 
 Discord Announcements via [Alliance Auth](https://gitlab.com/allianceauth/allianceauth)
 
 Write announcements and manage who can write announcements on your corporation or
 alliance Discord through Alliance Auth.
 
 
-## Contents
-
-- [Installation](#installation)
-- [Change Log](https://github.com/ppfeufer/aa-discord-announcements/blob/master/CHANGELOG.md)
-- [Code of Conduct](https://github.com/ppfeufer/aa-discord-announcements/blob/master/CODE_OF_CONDUCT.md)
-- [Contribute](https://github.com/ppfeufer/aa-discord-announcements/blob/master/CONTRIBUTING.md)
+<!-- TOC -->
+* [AA Discord Announcements](#aa-discord-announcements)
+  * [Installation](#installation)
+    * [⚠️ Important ⚠️](#-important-)
+    * [Step 1: Install the App](#step-1-install-the-app)
+    * [Step 2: Update Your AA Settings](#step-2-update-your-aa-settings)
+    * [Step 3: Finalizing the Installation](#step-3-finalizing-the-installation)
+    * [Step 4: Setting up Permission](#step-4-setting-up-permission)
+    * [Step 5: Setting up the App](#step-5-setting-up-the-app)
+<!-- TOC -->
 
 
 ## Installation
 
 ### ⚠️ Important ⚠️
 
 This app is a plugin for Alliance Auth. If you don't have Alliance Auth running already,
 please install it first before proceeding.
-(see the official
+(See the official
 [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html)
 for details)
 
 **⚠️ You also want to make sure that you have the
 [Discord service](https://allianceauth.readthedocs.io/en/latest/features/services/discord.html)
 installed, configured and activated before installing this app. ⚠️**
 
-### Step 1 - Install the app
 
-Make sure you are in the virtual environment (venv) of your Alliance Auth installation.
+### Step 1: Install the App
+
+Make sure you're in the virtual environment (venv) of your Alliance Auth installation.
 Then install the latest version:
 
-```bash
+```shell
 pip install aa-discord-announcements
 ```
 
-### Step 2 - Update your AA settings
+
+### Step 2: Update Your AA Settings
 
 Configure your AA settings (`local.py`) as follows:
 
-- Add `'aa_discord_announcements',` to `INSTALLED_APPS`
+- Add `"aa_discord_announcements",` to `INSTALLED_APPS`
 
 
-### Step 3 - Finalize the installation
+### Step 3: Finalizing the Installation
 
 Copy static files and run migrations
 
-```bash
+```shell
 python manage.py collectstatic
 python manage.py migrate
 ```
 
 Restart your supervisor services for AA
 
-### Step 4 - Setup permission
 
-Now you can setup permissions in Alliance Auth for your users.
+### Step 4: Setting up Permission
+
+Now you can set up permissions in Alliance Auth for your users.
 Add `aa_discord_announcements | general | Can access this app` to the states and/or
 groups you would like to have access.
 
-### Step 5 - Setup the app
+
+### Step 5: Setting up the App
 
 In your admin backend you'll find a new section called `Discord Announcements`.
 This is where you set all your stuff up, like the webhooks you want to ping and who
 can ping them. It's pretty straight forward, so you shouldn't have any issues. Go nuts!
```

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/admin.py` & `aa_discord_announcements-1.1.0/aa_discord_announcements/admin.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/auth_hooks.py` & `aa_discord_announcements-1.1.0/aa_discord_announcements/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/forms.py` & `aa_discord_announcements-1.1.0/aa_discord_announcements/forms.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/helper/announcement_context.py` & `aa_discord_announcements-1.1.0/aa_discord_announcements/helper/announcement_context.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/helper/discord_webhook.py` & `aa_discord_announcements-1.1.0/aa_discord_announcements/helper/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo` & `aa_discord_announcements-1.1.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.po` & `aa_discord_announcements-1.1.0/aa_discord_announcements/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/locale/es/LC_MESSAGES/django.po` & `aa_discord_announcements-1.1.0/aa_discord_announcements/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po` & `aa_discord_announcements-1.1.0/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po` & `aa_discord_announcements-1.1.0/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po` & `aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po` & `aa_discord_announcements-1.1.0/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po` & `aa_discord_announcements-1.1.0/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-04-11 23:21+0200\n"
-"PO-Revision-Date: 2023-04-11 21:42+0000\n"
-"Last-Translator: \"H. Peter Pfeufer\" <info@ppfeufer.de>\n"
-"Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-discord-announcements/ru/>\n"
-"Language: ru\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || ("
-"n%100>=11 && n%100<=14)? 2 : 3);\n"
-"X-Generator: Weblate 4.16.4\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: forms.py:20
 msgid "This field is mandatory"
-msgstr "Обязательное поле"
+msgstr ""
 
 #: forms.py:41
 msgid "Discord Markdown"
 msgstr ""
 
 #: forms.py:48
 #, python-brace-format
```

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/migrations/0001_initial.py` & `aa_discord_announcements-1.1.0/aa_discord_announcements/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/models.py` & `aa_discord_announcements-1.1.0/aa_discord_announcements/models.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js` & `aa_discord_announcements-1.1.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js` & `aa_discord_announcements-1.1.0/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/index.html` & `aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/index.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html` & `aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html` & `aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html` & `aa_discord_announcements-1.1.0/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py` & `aa_discord_announcements-1.1.0/aa_discord_announcements/templatetags/aa_discord_announcements_versioned_static.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_access.py` & `aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_ajax_calls.py` & `aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_ajax_calls.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_auth_hooks.py` & `aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_installed_modules.py` & `aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_installed_modules.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_models.py` & `aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/tests/test_templatetags.py` & `aa_discord_announcements-1.1.0/aa_discord_announcements/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/tests/utils.py` & `aa_discord_announcements-1.1.0/aa_discord_announcements/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/urls.py` & `aa_discord_announcements-1.1.0/aa_discord_announcements/urls.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements/views.py` & `aa_discord_announcements-1.1.0/aa_discord_announcements/views.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements.egg-info/PKG-INFO` & `aa_discord_announcements-1.1.0/aa_discord_announcements.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-discord-announcements
-Version: 1.0.0
+Version: 1.1.0
 Summary: Discord Announcements via Alliance Auth. Write announcements and manage who can write announcements on your corporation or alliance Discord through Alliance Auth.
 Home-page: https://github.com/ppfeufer/aa-discord-announcements
 Author: Peter Pfeufer
 Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
@@ -46,67 +46,75 @@
 
 Discord Announcements via [Alliance Auth](https://gitlab.com/allianceauth/allianceauth)
 
 Write announcements and manage who can write announcements on your corporation or
 alliance Discord through Alliance Auth.
 
 
-## Contents
-
-- [Installation](#installation)
-- [Change Log](https://github.com/ppfeufer/aa-discord-announcements/blob/master/CHANGELOG.md)
-- [Code of Conduct](https://github.com/ppfeufer/aa-discord-announcements/blob/master/CODE_OF_CONDUCT.md)
-- [Contribute](https://github.com/ppfeufer/aa-discord-announcements/blob/master/CONTRIBUTING.md)
+<!-- TOC -->
+* [AA Discord Announcements](#aa-discord-announcements)
+  * [Installation](#installation)
+    * [⚠️ Important ⚠️](#-important-)
+    * [Step 1: Install the App](#step-1-install-the-app)
+    * [Step 2: Update Your AA Settings](#step-2-update-your-aa-settings)
+    * [Step 3: Finalizing the Installation](#step-3-finalizing-the-installation)
+    * [Step 4: Setting up Permission](#step-4-setting-up-permission)
+    * [Step 5: Setting up the App](#step-5-setting-up-the-app)
+<!-- TOC -->
 
 
 ## Installation
 
 ### ⚠️ Important ⚠️
 
 This app is a plugin for Alliance Auth. If you don't have Alliance Auth running already,
 please install it first before proceeding.
-(see the official
+(See the official
 [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html)
 for details)
 
 **⚠️ You also want to make sure that you have the
 [Discord service](https://allianceauth.readthedocs.io/en/latest/features/services/discord.html)
 installed, configured and activated before installing this app. ⚠️**
 
-### Step 1 - Install the app
 
-Make sure you are in the virtual environment (venv) of your Alliance Auth installation.
+### Step 1: Install the App
+
+Make sure you're in the virtual environment (venv) of your Alliance Auth installation.
 Then install the latest version:
 
-```bash
+```shell
 pip install aa-discord-announcements
 ```
 
-### Step 2 - Update your AA settings
+
+### Step 2: Update Your AA Settings
 
 Configure your AA settings (`local.py`) as follows:
 
-- Add `'aa_discord_announcements',` to `INSTALLED_APPS`
+- Add `"aa_discord_announcements",` to `INSTALLED_APPS`
 
 
-### Step 3 - Finalize the installation
+### Step 3: Finalizing the Installation
 
 Copy static files and run migrations
 
-```bash
+```shell
 python manage.py collectstatic
 python manage.py migrate
 ```
 
 Restart your supervisor services for AA
 
-### Step 4 - Setup permission
 
-Now you can setup permissions in Alliance Auth for your users.
+### Step 4: Setting up Permission
+
+Now you can set up permissions in Alliance Auth for your users.
 Add `aa_discord_announcements | general | Can access this app` to the states and/or
 groups you would like to have access.
 
-### Step 5 - Setup the app
+
+### Step 5: Setting up the App
 
 In your admin backend you'll find a new section called `Discord Announcements`.
 This is where you set all your stuff up, like the webhooks you want to ping and who
 can ping them. It's pretty straight forward, so you shouldn't have any issues. Go nuts!
```

### Comparing `aa_discord_announcements-1.0.0/aa_discord_announcements.egg-info/SOURCES.txt` & `aa_discord_announcements-1.1.0/aa_discord_announcements.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-1.0.0/setup.cfg` & `aa_discord_announcements-1.1.0/setup.cfg`

 * *Files identical despite different names*

