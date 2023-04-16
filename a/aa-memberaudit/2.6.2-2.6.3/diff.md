# Comparing `tmp/aa_memberaudit-2.6.2.tar.gz` & `tmp/aa_memberaudit-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_memberaudit-2.6.2.tar", last modified: Tue Apr 11 14:29:41 2023, max compression
+gzip compressed data, was "aa_memberaudit-2.6.3.tar", last modified: Sun Apr 16 16:38:10 2023, max compression
```

## Comparing `aa_memberaudit-2.6.2.tar` & `aa_memberaudit-2.6.3.tar`

### file list

```diff
@@ -1,276 +1,278 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.104345 aa_memberaudit-2.6.2/
--rw-rw-rw-   0 root         (0) root         (0)    25118 2023-04-11 13:51:51.000000 aa_memberaudit-2.6.2/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1070 2020-12-07 16:50:18.000000 aa_memberaudit-2.6.2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-03-27 13:03:22.000000 aa_memberaudit-2.6.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6841 2023-04-11 14:29:41.104345 aa_memberaudit-2.6.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5719 2023-03-23 15:22:24.000000 aa_memberaudit-2.6.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.048345 aa_memberaudit-2.6.2/aa_memberaudit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6841 2023-04-11 14:29:41.000000 aa_memberaudit-2.6.2/aa_memberaudit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11052 2023-04-11 14:29:41.000000 aa_memberaudit-2.6.2/aa_memberaudit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 14:29:41.000000 aa_memberaudit-2.6.2/aa_memberaudit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-11 14:29:40.000000 aa_memberaudit-2.6.2/aa_memberaudit.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      117 2023-04-11 14:29:41.000000 aa_memberaudit-2.6.2/aa_memberaudit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-11 14:29:41.000000 aa_memberaudit-2.6.2/aa_memberaudit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.052345 aa_memberaudit-2.6.2/memberaudit/
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-04-11 13:51:51.000000 aa_memberaudit-2.6.2/memberaudit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21864 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.2/memberaudit/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     4486 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.2/memberaudit/app_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.2/memberaudit/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     1223 2021-05-04 15:11:43.000000 aa_memberaudit-2.6.2/memberaudit/auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1242 2023-03-22 20:38:17.000000 aa_memberaudit-2.6.2/memberaudit/checks.py
--rw-rw-rw-   0 root         (0) root         (0)     1354 2023-03-22 22:31:11.000000 aa_memberaudit-2.6.2/memberaudit/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.052345 aa_memberaudit-2.6.2/memberaudit/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 14:29:19.000000 aa_memberaudit-2.6.2/memberaudit/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11673 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.2/memberaudit/core/data_exporters.py
--rw-rw-rw-   0 root         (0) root         (0)    19049 2023-03-27 10:15:12.000000 aa_memberaudit-2.6.2/memberaudit/core/eft_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     5305 2023-03-27 10:15:12.000000 aa_memberaudit-2.6.2/memberaudit/core/fittings.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2022-09-03 21:36:22.000000 aa_memberaudit-2.6.2/memberaudit/core/skill_plans.py
--rw-rw-rw-   0 root         (0) root         (0)     5342 2022-09-02 18:40:08.000000 aa_memberaudit-2.6.2/memberaudit/core/skills.py
--rw-rw-rw-   0 root         (0) root         (0)     3150 2022-07-14 11:30:46.000000 aa_memberaudit-2.6.2/memberaudit/core/xml_converter.py
--rw-rw-rw-   0 root         (0) root         (0)     2336 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.2/memberaudit/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     3636 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.2/memberaudit/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     2257 2023-02-24 17:52:57.000000 aa_memberaudit-2.6.2/memberaudit/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.040345 aa_memberaudit-2.6.2/memberaudit/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.036345 aa_memberaudit-2.6.2/memberaudit/locale/de/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.056345 aa_memberaudit-2.6.2/memberaudit/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    20772 2021-01-05 20:12:03.000000 aa_memberaudit-2.6.2/memberaudit/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.036345 aa_memberaudit-2.6.2/memberaudit/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.056345 aa_memberaudit-2.6.2/memberaudit/locale/en/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    20766 2021-01-05 20:12:03.000000 aa_memberaudit-2.6.2/memberaudit/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.036345 aa_memberaudit-2.6.2/memberaudit/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.056345 aa_memberaudit-2.6.2/memberaudit/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    20766 2021-01-05 20:12:03.000000 aa_memberaudit-2.6.2/memberaudit/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.040345 aa_memberaudit-2.6.2/memberaudit/locale/ko/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.056345 aa_memberaudit-2.6.2/memberaudit/locale/ko/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    20759 2021-01-05 20:12:03.000000 aa_memberaudit-2.6.2/memberaudit/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.040345 aa_memberaudit-2.6.2/memberaudit/locale/ru/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.056345 aa_memberaudit-2.6.2/memberaudit/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    20910 2021-01-05 20:12:03.000000 aa_memberaudit-2.6.2/memberaudit/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.040345 aa_memberaudit-2.6.2/memberaudit/locale/zh_Hans/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.056345 aa_memberaudit-2.6.2/memberaudit/locale/zh_Hans/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    20759 2021-01-05 20:12:03.000000 aa_memberaudit-2.6.2/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.040345 aa_memberaudit-2.6.2/memberaudit/management/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.056345 aa_memberaudit-2.6.2/memberaudit/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      102 2020-11-24 21:31:34.000000 aa_memberaudit-2.6.2/memberaudit/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1424 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.2/memberaudit/management/commands/memberaudit_data_export.py
--rw-rw-rw-   0 root         (0) root         (0)     1357 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/management/commands/memberaudit_load_eve.py
--rw-rw-rw-   0 root         (0) root         (0)     3832 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.2/memberaudit/management/commands/memberaudit_reset_characters.py
--rw-rw-rw-   0 root         (0) root         (0)      723 2021-05-04 15:11:43.000000 aa_memberaudit-2.6.2/memberaudit/management/commands/memberaudit_stats.py
--rw-rw-rw-   0 root         (0) root         (0)     1914 2021-05-04 15:11:43.000000 aa_memberaudit-2.6.2/memberaudit/management/commands/memberaudit_update_characters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.056345 aa_memberaudit-2.6.2/memberaudit/managers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 14:29:19.000000 aa_memberaudit-2.6.2/memberaudit/managers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13007 2023-02-24 14:11:29.000000 aa_memberaudit-2.6.2/memberaudit/managers/character.py
--rw-rw-rw-   0 root         (0) root         (0)    21180 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.2/memberaudit/managers/general.py
--rw-rw-rw-   0 root         (0) root         (0)    48369 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.2/memberaudit/managers/sections.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.060345 aa_memberaudit-2.6.2/memberaudit/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    65995 2023-02-24 17:11:11.000000 aa_memberaudit-2.6.2/memberaudit/migrations/0001_initial_new.py
--rw-rw-rw-   0 root         (0) root         (0)     3444 2023-02-24 17:11:11.000000 aa_memberaudit-2.6.2/memberaudit/migrations/0002_add_mining_ledger.py
--rw-rw-rw-   0 root         (0) root         (0)     1478 2023-02-24 17:11:11.000000 aa_memberaudit-2.6.2/memberaudit/migrations/0003_add_notify_permission.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-02-24 17:11:11.000000 aa_memberaudit-2.6.2/memberaudit/migrations/0004_character_is_disabled.py
--rw-rw-rw-   0 root         (0) root         (0)     3819 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.2/memberaudit/migrations/0005_add_fw_stats.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 14:29:19.000000 aa_memberaudit-2.6.2/memberaudit/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.060345 aa_memberaudit-2.6.2/memberaudit/models/
--rw-rw-rw-   0 root         (0) root         (0)     1033 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.2/memberaudit/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    53140 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.2/memberaudit/models/character.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2021-01-17 22:43:01.000000 aa_memberaudit-2.6.2/memberaudit/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    14223 2022-10-21 17:48:21.000000 aa_memberaudit-2.6.2/memberaudit/models/general.py
--rw-rw-rw-   0 root         (0) root         (0)    39924 2023-03-22 22:31:11.000000 aa_memberaudit-2.6.2/memberaudit/models/sections.py
--rw-rw-rw-   0 root         (0) root         (0)      246 2022-06-17 10:57:57.000000 aa_memberaudit-2.6.2/memberaudit/providers.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2022-03-05 14:47:06.000000 aa_memberaudit-2.6.2/memberaudit/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.040345 aa_memberaudit-2.6.2/memberaudit/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.040345 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.064345 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/
--rw-rw-rw-   0 root         (0) root         (0)      191 2023-02-24 14:11:29.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/admin.css
--rw-rw-rw-   0 root         (0) root         (0)      174 2022-02-09 21:55:36.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/character_finder.css
--rw-rw-rw-   0 root         (0) root         (0)     5638 2022-10-13 18:45:54.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/character_viewer.css
--rw-rw-rw-   0 root         (0) root         (0)     2540 2021-01-29 15:59:17.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/character_viewer.min.css
--rw-rw-rw-   0 root         (0) root         (0)       94 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/data_export.css
--rw-rw-rw-   0 root         (0) root         (0)     1538 2021-05-04 21:32:43.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/global.css
--rw-rw-rw-   0 root         (0) root         (0)      646 2021-01-29 15:59:17.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/global.min.css
--rw-rw-rw-   0 root         (0) root         (0)     4331 2020-11-03 21:09:40.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/launcher.css
--rw-rw-rw-   0 root         (0) root         (0)     2765 2021-01-29 15:59:17.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/launcher.min.css
--rw-rw-rw-   0 root         (0) root         (0)     1363 2021-02-16 17:03:36.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/memberaudit.css
--rw-rw-rw-   0 root         (0) root         (0)      617 2021-02-16 17:03:36.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/memberaudit.min.css
--rw-rw-rw-   0 root         (0) root         (0)      611 2021-02-17 10:40:00.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/reports.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.068345 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/
--rw-rw-rw-   0 root         (0) root         (0)    43262 2020-10-26 16:42:17.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif
--rw-rw-rw-   0 root         (0) root         (0)    43381 2020-10-26 16:42:17.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif
--rw-rw-rw-   0 root         (0) root         (0)     1862 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/charisma.png
--rw-rw-rw-   0 root         (0) root         (0)      694 2020-11-03 21:09:40.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/eve-prism.png
--rw-rw-rw-   0 root         (0) root         (0)      220 2020-11-03 21:09:40.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/evelogo.png
--rw-rw-rw-   0 root         (0) root         (0)      595 2020-11-03 21:09:40.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/evesearch.png
--rw-rw-rw-   0 root         (0) root         (0)     1966 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/intelligence.png
--rw-rw-rw-   0 root         (0) root         (0)     1809 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/memory.png
--rw-rw-rw-   0 root         (0) root         (0)     1803 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/perception.png
--rw-rw-rw-   0 root         (0) root         (0)     1782 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/willpower.png
--rw-rw-rw-   0 root         (0) root         (0)      259 2020-10-22 17:18:29.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/zkillboard.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.040345 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/vendor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.040345 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/vendor/datatables/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.068345 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/vendor/datatables/plugins/
--rw-rw-rw-   0 root         (0) root         (0)     5573 2020-10-22 17:18:29.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js
--rw-rw-rw-   0 root         (0) root         (0)     3908 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js
--rw-rw-rw-   0 root         (0) root         (0)     2529 2022-04-01 19:48:30.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js
--rw-rw-rw-   0 root         (0) root         (0)      384 2020-10-22 17:18:29.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.bootstrap.min.css
--rw-rw-rw-   0 root         (0) root         (0)      384 2020-10-22 17:18:29.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.dataTables.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.068345 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/vendor/moment/
--rw-rw-rw-   0 root         (0) root         (0)    69950 2020-10-28 14:46:25.000000 aa_memberaudit-2.6.2/memberaudit/static/memberaudit/vendor/moment/moment.min.js
--rw-rw-rw-   0 root         (0) root         (0)   881821 2023-02-16 19:01:05.000000 aa_memberaudit-2.6.2/memberaudit/swagger.json
--rw-rw-rw-   0 root         (0) root         (0)    39964 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.2/memberaudit/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.040345 aa_memberaudit-2.6.2/memberaudit/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.040345 aa_memberaudit-2.6.2/memberaudit/templates/admin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.040345 aa_memberaudit-2.6.2/memberaudit/templates/admin/memberaudit/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.068345 aa_memberaudit-2.6.2/memberaudit/templates/admin/memberaudit/character/
--rw-rw-rw-   0 root         (0) root         (0)      640 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.068345 aa_memberaudit-2.6.2/memberaudit/templates/admin/memberaudit/skillset/
--rw-rw-rw-   0 root         (0) root         (0)      488 2022-09-02 18:40:08.000000 aa_memberaudit-2.6.2/memberaudit/templates/admin/memberaudit/skillset/change_list.html
--rw-rw-rw-   0 root         (0) root         (0)      830 2022-09-03 16:21:19.000000 aa_memberaudit-2.6.2/memberaudit/templates/admin/memberaudit/skillset/import_skills.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.068345 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/
--rw-rw-rw-   0 root         (0) root         (0)      367 2020-12-07 00:53:01.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/base.html
--rw-rw-rw-   0 root         (0) root         (0)     4679 2022-04-01 19:48:30.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/character_finder.html
--rw-rw-rw-   0 root         (0) root         (0)    27476 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/character_viewer.html
--rw-rw-rw-   0 root         (0) root         (0)     2669 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/data_export.html
--rw-rw-rw-   0 root         (0) root         (0)     8152 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/launcher.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.040345 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/modals/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.072345 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/modals/character_viewer/
--rw-rw-rw-   0 root         (0) root         (0)     1238 2021-01-29 15:52:00.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html
--rw-rw-rw-   0 root         (0) root         (0)     4307 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html
--rw-rw-rw-   0 root         (0) root         (0)     1713 2021-02-18 07:41:27.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1246 2020-11-01 21:48:51.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/modals/character_viewer/contract.html
--rw-rw-rw-   0 root         (0) root         (0)     8003 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html
--rw-rw-rw-   0 root         (0) root         (0)      640 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html
--rw-rw-rw-   0 root         (0) root         (0)     1375 2022-02-09 21:55:36.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/modals/character_viewer/mail.html
--rw-rw-rw-   0 root         (0) root         (0)      364 2022-02-09 21:55:36.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/modals/character_viewer/mail_content.html
--rw-rw-rw-   0 root         (0) root         (0)     3880 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.072345 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.072345 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/
--rw-rw-rw-   0 root         (0) root         (0)     9001 2022-07-22 18:45:02.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/overview.html
--rw-rw-rw-   0 root         (0) root         (0)     1359 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html
--rw-rw-rw-   0 root         (0) root         (0)      561 2021-02-18 10:40:48.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.076345 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/
--rw-rw-rw-   0 root         (0) root         (0)     1218 2021-01-29 15:52:00.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html
--rw-rw-rw-   0 root         (0) root         (0)      520 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html
--rw-rw-rw-   0 root         (0) root         (0)     2604 2021-02-23 15:40:36.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html
--rw-rw-rw-   0 root         (0) root         (0)      279 2022-02-08 21:33:10.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_bio.html
--rw-rw-rw-   0 root         (0) root         (0)      808 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html
--rw-rw-rw-   0 root         (0) root         (0)      919 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html
--rw-rw-rw-   0 root         (0) root         (0)      543 2020-11-09 19:29:14.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html
--rw-rw-rw-   0 root         (0) root         (0)      894 2020-12-14 23:31:49.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html
--rw-rw-rw-   0 root         (0) root         (0)     2768 2023-03-22 22:31:11.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html
--rw-rw-rw-   0 root         (0) root         (0)      505 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html
--rw-rw-rw-   0 root         (0) root         (0)      678 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html
--rw-rw-rw-   0 root         (0) root         (0)      148 2020-11-09 19:29:14.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/last_updated.html
--rw-rw-rw-   0 root         (0) root         (0)      572 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html
--rw-rw-rw-   0 root         (0) root         (0)     2841 2022-02-09 21:55:36.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html
--rw-rw-rw-   0 root         (0) root         (0)      741 2022-10-13 17:41:55.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html
--rw-rw-rw-   0 root         (0) root         (0)      626 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html
--rw-rw-rw-   0 root         (0) root         (0)      822 2021-02-16 14:35:06.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html
--rw-rw-rw-   0 root         (0) root         (0)      554 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html
--rw-rw-rw-   0 root         (0) root         (0)      889 2021-01-25 17:36:44.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html
--rw-rw-rw-   0 root         (0) root         (0)      898 2021-01-25 17:36:44.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html
--rw-rw-rw-   0 root         (0) root         (0)     3440 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html
--rw-rw-rw-   0 root         (0) root         (0)     2674 2022-01-23 15:08:18.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/menu.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.076345 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/reports/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.080345 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/reports/tabs/
--rw-rw-rw-   0 root         (0) root         (0)      796 2021-02-16 15:13:05.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html
--rw-rw-rw-   0 root         (0) root         (0)      742 2022-04-01 19:28:56.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html
--rw-rw-rw-   0 root         (0) root         (0)      887 2021-02-17 10:40:00.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html
--rw-rw-rw-   0 root         (0) root         (0)      691 2021-02-16 15:13:05.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html
--rw-rw-rw-   0 root         (0) root         (0)      675 2020-11-09 19:29:14.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/solar_system.html
--rw-rw-rw-   0 root         (0) root         (0)     9420 2022-04-01 19:56:47.000000 aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/reports.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.080345 aa_memberaudit-2.6.2/memberaudit/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 14:29:19.000000 aa_memberaudit-2.6.2/memberaudit/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      330 2021-01-05 22:10:38.000000 aa_memberaudit-2.6.2/memberaudit/templatetags/memberaudit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.084345 aa_memberaudit-2.6.2/memberaudit/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 14:29:19.000000 aa_memberaudit-2.6.2/memberaudit/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.084345 aa_memberaudit-2.6.2/memberaudit/tests/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 14:29:19.000000 aa_memberaudit-2.6.2/memberaudit/tests/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6340 2022-07-14 11:30:46.000000 aa_memberaudit-2.6.2/memberaudit/tests/core/test_core_xml_converter.py
--rw-rw-rw-   0 root         (0) root         (0)    12708 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.2/memberaudit/tests/core/test_data_exporters.py
--rw-rw-rw-   0 root         (0) root         (0)    20438 2023-03-27 10:15:12.000000 aa_memberaudit-2.6.2/memberaudit/tests/core/test_eft_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4627 2023-03-27 10:15:12.000000 aa_memberaudit-2.6.2/memberaudit/tests/core/test_fittings.py
--rw-rw-rw-   0 root         (0) root         (0)     4082 2022-09-03 21:36:22.000000 aa_memberaudit-2.6.2/memberaudit/tests/core/test_skill_plans.py
--rw-rw-rw-   0 root         (0) root         (0)     2431 2022-09-02 18:40:08.000000 aa_memberaudit-2.6.2/memberaudit/tests/core/test_skills.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.084345 aa_memberaudit-2.6.2/memberaudit/tests/managers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 14:29:19.000000 aa_memberaudit-2.6.2/memberaudit/tests/managers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18357 2023-02-24 14:11:29.000000 aa_memberaudit-2.6.2/memberaudit/tests/managers/test_character.py
--rw-rw-rw-   0 root         (0) root         (0)    39823 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.2/memberaudit/tests/managers/test_general.py
--rw-rw-rw-   0 root         (0) root         (0)     3382 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.2/memberaudit/tests/managers/test_sections.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.088345 aa_memberaudit-2.6.2/memberaudit/tests/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 14:29:19.000000 aa_memberaudit-2.6.2/memberaudit/tests/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    34701 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.2/memberaudit/tests/models/test_character_1.py
--rw-rw-rw-   0 root         (0) root         (0)    35834 2023-02-16 19:01:05.000000 aa_memberaudit-2.6.2/memberaudit/tests/models/test_character_2.py
--rw-rw-rw-   0 root         (0) root         (0)    40698 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.2/memberaudit/tests/models/test_character_3.py
--rw-rw-rw-   0 root         (0) root         (0)    28275 2023-03-22 21:45:48.000000 aa_memberaudit-2.6.2/memberaudit/tests/models/test_character_4.py
--rw-rw-rw-   0 root         (0) root         (0)    10448 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.2/memberaudit/tests/models/test_general.py
--rw-rw-rw-   0 root         (0) root         (0)     1590 2023-03-22 22:31:11.000000 aa_memberaudit-2.6.2/memberaudit/tests/models/test_sections.py
--rw-rw-rw-   0 root         (0) root         (0)     1048 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.2/memberaudit/tests/models/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    11633 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.2/memberaudit/tests/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     1807 2023-02-24 17:52:57.000000 aa_memberaudit-2.6.2/memberaudit/tests/test_auth_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1314 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.2/memberaudit/tests/test_checks.py
--rw-rw-rw-   0 root         (0) root         (0)     3425 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.2/memberaudit/tests/test_commands.py
--rw-rw-rw-   0 root         (0) root         (0)     4062 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.2/memberaudit/tests/test_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)      889 2022-08-07 14:05:02.000000 aa_memberaudit-2.6.2/memberaudit/tests/test_factories.py
--rw-rw-rw-   0 root         (0) root         (0)     3516 2022-09-03 16:21:19.000000 aa_memberaudit-2.6.2/memberaudit/tests/test_forms.py
--rw-rw-rw-   0 root         (0) root         (0)     3813 2023-02-24 17:52:57.000000 aa_memberaudit-2.6.2/memberaudit/tests/test_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    12216 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.2/memberaudit/tests/test_integration.py
--rw-rw-rw-   0 root         (0) root         (0)     1215 2022-03-05 14:47:06.000000 aa_memberaudit-2.6.2/memberaudit/tests/test_signals.py
--rw-rw-rw-   0 root         (0) root         (0)    36109 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.2/memberaudit/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)      958 2021-05-04 15:11:43.000000 aa_memberaudit-2.6.2/memberaudit/tests/test_templatetags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.096345 aa_memberaudit-2.6.2/memberaudit/tests/testdata/
--rw-rw-rw-   0 root         (0) root         (0)      267 2020-10-22 17:18:30.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4277 2022-10-12 21:43:27.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/create_eveuniverse.py
--rw-rw-rw-   0 root         (0) root         (0)     4350 2022-02-10 22:57:31.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/entities.json
--rw-rw-rw-   0 root         (0) root         (0)     4703 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/esi_client_stub.py
--rw-rw-rw-   0 root         (0) root         (0)    40192 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/esi_testdata.json
--rw-rw-rw-   0 root         (0) root         (0)  1159197 2022-10-12 21:43:27.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/eveuniverse.json
--rw-rw-rw-   0 root         (0) root         (0)    11769 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/factories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.100345 aa_memberaudit-2.6.2/memberaudit/tests/testdata/fittings/
--rw-rw-rw-   0 root         (0) root         (0)      799 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/fittings/fitting_archon.txt
--rw-rw-rw-   0 root         (0) root         (0)      889 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/fittings/fitting_archon_max.txt
--rw-rw-rw-   0 root         (0) root         (0)      231 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/fittings/fitting_empty.txt
--rw-rw-rw-   0 root         (0) root         (0)      503 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/fittings/fitting_eve_celestis_no_high_slots.txt
--rw-rw-rw-   0 root         (0) root         (0)      193 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/fittings/fitting_eve_tristan_3.txt
--rw-rw-rw-   0 root         (0) root         (0)      377 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/fittings/fitting_eve_tristian.txt
--rw-rw-rw-   0 root         (0) root         (0)      293 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/fittings/fitting_eve_tristian_2.txt
--rw-rw-rw-   0 root         (0) root         (0)       96 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/fittings/fitting_eve_tristian_empty.txt
--rw-rw-rw-   0 root         (0) root         (0)      583 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/fittings/fitting_svipul.txt
--rw-rw-rw-   0 root         (0) root         (0)      432 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/fittings/fitting_svipul_2.txt
--rw-rw-rw-   0 root         (0) root         (0)      700 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/fittings/fitting_tengu.txt
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/fittings/fitting_tristan.txt
--rw-rw-rw-   0 root         (0) root         (0)      332 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/fittings/fitting_tristan_missing_rigs.txt
--rw-rw-rw-   0 root         (0) root         (0)      410 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/fittings/fitting_tristan_no_title.txt
--rw-rw-rw-   0 root         (0) root         (0)      460 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/fittings/fitting_tristan_unknown_types.txt
--rw-rw-rw-   0 root         (0) root         (0)     3908 2022-01-20 23:34:01.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/generate_character.py
--rw-rw-rw-   0 root         (0) root         (0)     3859 2022-01-20 23:34:01.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/generate_doctrines.py
--rw-rw-rw-   0 root         (0) root         (0)     3671 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/load_entities.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2020-10-22 17:18:30.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/load_eveuniverse.py
--rw-rw-rw-   0 root         (0) root         (0)     1188 2022-02-10 21:29:55.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/load_locations.py
--rw-rw-rw-   0 root         (0) root         (0)     1097 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/pilot_esi_error_handling.py
--rw-rw-rw-   0 root         (0) root         (0)      825 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/tests/testdata/profiler_toolbox.py
--rw-rw-rw-   0 root         (0) root         (0)     3494 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.2/memberaudit/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.100345 aa_memberaudit-2.6.2/memberaudit/tests/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 14:29:19.000000 aa_memberaudit-2.6.2/memberaudit/tests/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7809 2022-09-03 16:21:19.000000 aa_memberaudit-2.6.2/memberaudit/tests/views/test_admin.py
--rw-rw-rw-   0 root         (0) root         (0)     7079 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.2/memberaudit/tests/views/test_character_finder.py
--rw-rw-rw-   0 root         (0) root         (0)    32680 2023-03-22 21:45:48.000000 aa_memberaudit-2.6.2/memberaudit/tests/views/test_character_viewer_1.py
--rw-rw-rw-   0 root         (0) root         (0)    22475 2022-10-13 12:47:37.000000 aa_memberaudit-2.6.2/memberaudit/tests/views/test_character_viewer_2.py
--rw-rw-rw-   0 root         (0) root         (0)    14577 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.2/memberaudit/tests/views/test_characters.py
--rw-rw-rw-   0 root         (0) root         (0)     4091 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.2/memberaudit/tests/views/test_data_export.py
--rw-rw-rw-   0 root         (0) root         (0)    16230 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.2/memberaudit/tests/views/test_reports.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.100345 aa_memberaudit-2.6.2/memberaudit/tools/
--rw-rw-rw-   0 root         (0) root         (0)     3051 2022-10-21 18:07:26.000000 aa_memberaudit-2.6.2/memberaudit/tools/drop_tables.sql
--rw-rw-rw-   0 root         (0) root         (0)      329 2020-12-16 22:00:54.000000 aa_memberaudit-2.6.2/memberaudit/tools/total_size.sql
--rw-rw-rw-   0 root         (0) root         (0)     7031 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.2/memberaudit/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-11 14:29:41.104345 aa_memberaudit-2.6.2/memberaudit/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-11 14:29:19.000000 aa_memberaudit-2.6.2/memberaudit/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1478 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.2/memberaudit/views/_common.py
--rw-rw-rw-   0 root         (0) root         (0)     4636 2022-09-03 16:21:19.000000 aa_memberaudit-2.6.2/memberaudit/views/admin.py
--rw-rw-rw-   0 root         (0) root         (0)    12471 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.2/memberaudit/views/character_finder.py
--rw-rw-rw-   0 root         (0) root         (0)    25425 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.2/memberaudit/views/character_viewer_1.py
--rw-rw-rw-   0 root         (0) root         (0)    22486 2023-02-24 17:11:11.000000 aa_memberaudit-2.6.2/memberaudit/views/character_viewer_2.py
--rw-rw-rw-   0 root         (0) root         (0)     7845 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.2/memberaudit/views/characters.py
--rw-rw-rw-   0 root         (0) root         (0)     2186 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.2/memberaudit/views/data_export.py
--rw-rw-rw-   0 root         (0) root         (0)    13074 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.2/memberaudit/views/reports.py
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-03-27 10:15:12.000000 aa_memberaudit-2.6.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1748 2023-04-11 14:29:41.108345 aa_memberaudit-2.6.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.703024 aa_memberaudit-2.6.3/
+-rw-rw-rw-   0 root         (0) root         (0)    25180 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2020-12-07 16:50:18.000000 aa_memberaudit-2.6.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-03-27 13:03:22.000000 aa_memberaudit-2.6.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6841 2023-04-16 16:38:10.703024 aa_memberaudit-2.6.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5719 2023-03-23 15:22:24.000000 aa_memberaudit-2.6.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.527024 aa_memberaudit-2.6.3/aa_memberaudit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6841 2023-04-16 16:38:10.000000 aa_memberaudit-2.6.3/aa_memberaudit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11185 2023-04-16 16:38:10.000000 aa_memberaudit-2.6.3/aa_memberaudit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 16:38:10.000000 aa_memberaudit-2.6.3/aa_memberaudit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 16:38:10.000000 aa_memberaudit-2.6.3/aa_memberaudit.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      117 2023-04-16 16:38:10.000000 aa_memberaudit-2.6.3/aa_memberaudit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-16 16:38:10.000000 aa_memberaudit-2.6.3/aa_memberaudit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.543024 aa_memberaudit-2.6.3/memberaudit/
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22972 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4486 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     1223 2021-05-04 15:11:43.000000 aa_memberaudit-2.6.3/memberaudit/auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2023-03-22 20:38:17.000000 aa_memberaudit-2.6.3/memberaudit/checks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1354 2023-03-22 22:31:11.000000 aa_memberaudit-2.6.3/memberaudit/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.547024 aa_memberaudit-2.6.3/memberaudit/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:37:37.000000 aa_memberaudit-2.6.3/memberaudit/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11673 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.3/memberaudit/core/data_exporters.py
+-rw-rw-rw-   0 root         (0) root         (0)    19049 2023-03-27 10:15:12.000000 aa_memberaudit-2.6.3/memberaudit/core/eft_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     5305 2023-03-27 10:15:12.000000 aa_memberaudit-2.6.3/memberaudit/core/fittings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2022-09-03 21:36:22.000000 aa_memberaudit-2.6.3/memberaudit/core/skill_plans.py
+-rw-rw-rw-   0 root         (0) root         (0)     5342 2022-09-02 18:40:08.000000 aa_memberaudit-2.6.3/memberaudit/core/skills.py
+-rw-rw-rw-   0 root         (0) root         (0)     3150 2022-07-14 11:30:46.000000 aa_memberaudit-2.6.3/memberaudit/core/xml_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2336 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     3636 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.3/memberaudit/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     2257 2023-02-24 17:52:57.000000 aa_memberaudit-2.6.3/memberaudit/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.503024 aa_memberaudit-2.6.3/memberaudit/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.503024 aa_memberaudit-2.6.3/memberaudit/locale/de/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.551024 aa_memberaudit-2.6.3/memberaudit/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    40294 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.503024 aa_memberaudit-2.6.3/memberaudit/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.551024 aa_memberaudit-2.6.3/memberaudit/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    40291 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.503024 aa_memberaudit-2.6.3/memberaudit/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.551024 aa_memberaudit-2.6.3/memberaudit/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    40291 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.503024 aa_memberaudit-2.6.3/memberaudit/locale/ko/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.551024 aa_memberaudit-2.6.3/memberaudit/locale/ko/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    40284 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.503024 aa_memberaudit-2.6.3/memberaudit/locale/ru/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.551024 aa_memberaudit-2.6.3/memberaudit/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    40433 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.503024 aa_memberaudit-2.6.3/memberaudit/locale/zh_Hans/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.551024 aa_memberaudit-2.6.3/memberaudit/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    40284 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.503024 aa_memberaudit-2.6.3/memberaudit/management/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.559024 aa_memberaudit-2.6.3/memberaudit/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      102 2020-11-24 21:31:34.000000 aa_memberaudit-2.6.3/memberaudit/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.3/memberaudit/management/commands/memberaudit_data_export.py
+-rw-rw-rw-   0 root         (0) root         (0)     1357 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/management/commands/memberaudit_load_eve.py
+-rw-rw-rw-   0 root         (0) root         (0)     3832 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/management/commands/memberaudit_reset_characters.py
+-rw-rw-rw-   0 root         (0) root         (0)      723 2021-05-04 15:11:43.000000 aa_memberaudit-2.6.3/memberaudit/management/commands/memberaudit_stats.py
+-rw-rw-rw-   0 root         (0) root         (0)     1914 2021-05-04 15:11:43.000000 aa_memberaudit-2.6.3/memberaudit/management/commands/memberaudit_update_characters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.563024 aa_memberaudit-2.6.3/memberaudit/managers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:37:37.000000 aa_memberaudit-2.6.3/memberaudit/managers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13007 2023-02-24 14:11:29.000000 aa_memberaudit-2.6.3/memberaudit/managers/character.py
+-rw-rw-rw-   0 root         (0) root         (0)    21180 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/managers/general.py
+-rw-rw-rw-   0 root         (0) root         (0)    48369 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.3/memberaudit/managers/sections.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.567024 aa_memberaudit-2.6.3/memberaudit/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    65995 2023-02-24 17:11:11.000000 aa_memberaudit-2.6.3/memberaudit/migrations/0001_initial_new.py
+-rw-rw-rw-   0 root         (0) root         (0)     3444 2023-02-24 17:11:11.000000 aa_memberaudit-2.6.3/memberaudit/migrations/0002_add_mining_ledger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2023-02-24 17:11:11.000000 aa_memberaudit-2.6.3/memberaudit/migrations/0003_add_notify_permission.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-02-24 17:11:11.000000 aa_memberaudit-2.6.3/memberaudit/migrations/0004_character_is_disabled.py
+-rw-rw-rw-   0 root         (0) root         (0)     3819 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.3/memberaudit/migrations/0005_add_fw_stats.py
+-rw-rw-rw-   0 root         (0) root         (0)     5969 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/migrations/0006_add_localizations.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:37:37.000000 aa_memberaudit-2.6.3/memberaudit/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.567024 aa_memberaudit-2.6.3/memberaudit/models/
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.3/memberaudit/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    53374 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/models/character.py
+-rw-rw-rw-   0 root         (0) root         (0)      108 2021-01-17 22:43:01.000000 aa_memberaudit-2.6.3/memberaudit/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    14766 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/models/general.py
+-rw-rw-rw-   0 root         (0) root         (0)    39924 2023-03-22 22:31:11.000000 aa_memberaudit-2.6.3/memberaudit/models/sections.py
+-rw-rw-rw-   0 root         (0) root         (0)      246 2022-06-17 10:57:57.000000 aa_memberaudit-2.6.3/memberaudit/providers.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2022-03-05 14:47:06.000000 aa_memberaudit-2.6.3/memberaudit/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.503024 aa_memberaudit-2.6.3/memberaudit/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.507024 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.591024 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-02-24 14:11:29.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/admin.css
+-rw-rw-rw-   0 root         (0) root         (0)      174 2022-02-09 21:55:36.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/character_finder.css
+-rw-rw-rw-   0 root         (0) root         (0)     5638 2022-10-13 18:45:54.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/character_viewer.css
+-rw-rw-rw-   0 root         (0) root         (0)     2540 2021-01-29 15:59:17.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/character_viewer.min.css
+-rw-rw-rw-   0 root         (0) root         (0)       94 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/data_export.css
+-rw-rw-rw-   0 root         (0) root         (0)     1538 2021-05-04 21:32:43.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/global.css
+-rw-rw-rw-   0 root         (0) root         (0)      646 2021-01-29 15:59:17.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/global.min.css
+-rw-rw-rw-   0 root         (0) root         (0)     4331 2020-11-03 21:09:40.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/launcher.css
+-rw-rw-rw-   0 root         (0) root         (0)     2765 2021-01-29 15:59:17.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/launcher.min.css
+-rw-rw-rw-   0 root         (0) root         (0)     1363 2021-02-16 17:03:36.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/memberaudit.css
+-rw-rw-rw-   0 root         (0) root         (0)      617 2021-02-16 17:03:36.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/memberaudit.min.css
+-rw-rw-rw-   0 root         (0) root         (0)      611 2021-02-17 10:40:00.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/reports.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.607024 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/
+-rw-rw-rw-   0 root         (0) root         (0)    43262 2020-10-26 16:42:17.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif
+-rw-rw-rw-   0 root         (0) root         (0)    43381 2020-10-26 16:42:17.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif
+-rw-rw-rw-   0 root         (0) root         (0)     1862 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/charisma.png
+-rw-rw-rw-   0 root         (0) root         (0)      694 2020-11-03 21:09:40.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/eve-prism.png
+-rw-rw-rw-   0 root         (0) root         (0)      220 2020-11-03 21:09:40.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/evelogo.png
+-rw-rw-rw-   0 root         (0) root         (0)      595 2020-11-03 21:09:40.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/evesearch.png
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/intelligence.png
+-rw-rw-rw-   0 root         (0) root         (0)     1809 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/memory.png
+-rw-rw-rw-   0 root         (0) root         (0)     1803 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/perception.png
+-rw-rw-rw-   0 root         (0) root         (0)     1782 2021-02-23 10:36:55.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/willpower.png
+-rw-rw-rw-   0 root         (0) root         (0)      259 2020-10-22 17:18:29.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/zkillboard.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.507024 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.507024 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/datatables/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.615024 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/datatables/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)     5573 2020-10-22 17:18:29.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     3908 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js
+-rw-rw-rw-   0 root         (0) root         (0)     2529 2022-04-01 19:48:30.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js
+-rw-rw-rw-   0 root         (0) root         (0)      384 2020-10-22 17:18:29.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.bootstrap.min.css
+-rw-rw-rw-   0 root         (0) root         (0)      384 2020-10-22 17:18:29.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.dataTables.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.615024 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/moment/
+-rw-rw-rw-   0 root         (0) root         (0)    69950 2020-10-28 14:46:25.000000 aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/moment/moment.min.js
+-rw-rw-rw-   0 root         (0) root         (0)   881821 2023-02-16 19:01:05.000000 aa_memberaudit-2.6.3/memberaudit/swagger.json
+-rw-rw-rw-   0 root         (0) root         (0)    39964 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.507024 aa_memberaudit-2.6.3/memberaudit/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.507024 aa_memberaudit-2.6.3/memberaudit/templates/admin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.507024 aa_memberaudit-2.6.3/memberaudit/templates/admin/memberaudit/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.619024 aa_memberaudit-2.6.3/memberaudit/templates/admin/memberaudit/character/
+-rw-rw-rw-   0 root         (0) root         (0)      687 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.619024 aa_memberaudit-2.6.3/memberaudit/templates/admin/memberaudit/skillset/
+-rw-rw-rw-   0 root         (0) root         (0)      488 2022-09-02 18:40:08.000000 aa_memberaudit-2.6.3/memberaudit/templates/admin/memberaudit/skillset/change_list.html
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/admin/memberaudit/skillset/import_skills.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.623024 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/
+-rw-rw-rw-   0 root         (0) root         (0)      367 2020-12-07 00:53:01.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/base.html
+-rw-rw-rw-   0 root         (0) root         (0)     4711 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/character_finder.html
+-rw-rw-rw-   0 root         (0) root         (0)    27476 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/character_viewer.html
+-rw-rw-rw-   0 root         (0) root         (0)     2909 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/data_export.html
+-rw-rw-rw-   0 root         (0) root         (0)     8515 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/launcher.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.507024 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.631024 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/
+-rw-rw-rw-   0 root         (0) root         (0)     1238 2021-01-29 15:52:00.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html
+-rw-rw-rw-   0 root         (0) root         (0)     4307 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2021-02-18 07:41:27.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     1246 2020-11-01 21:48:51.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/contract.html
+-rw-rw-rw-   0 root         (0) root         (0)     8075 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html
+-rw-rw-rw-   0 root         (0) root         (0)      658 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2022-02-09 21:55:36.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/mail.html
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/mail_content.html
+-rw-rw-rw-   0 root         (0) root         (0)     3880 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.635024 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.635024 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/
+-rw-rw-rw-   0 root         (0) root         (0)     9001 2022-07-22 18:45:02.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/overview.html
+-rw-rw-rw-   0 root         (0) root         (0)     1451 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.647024 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/
+-rw-rw-rw-   0 root         (0) root         (0)     1218 2021-01-29 15:52:00.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html
+-rw-rw-rw-   0 root         (0) root         (0)     2604 2021-02-23 15:40:36.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_bio.html
+-rw-rw-rw-   0 root         (0) root         (0)      808 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html
+-rw-rw-rw-   0 root         (0) root         (0)      919 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html
+-rw-rw-rw-   0 root         (0) root         (0)      543 2020-11-09 19:29:14.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html
+-rw-rw-rw-   0 root         (0) root         (0)      894 2020-12-14 23:31:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html
+-rw-rw-rw-   0 root         (0) root         (0)      488 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html
+-rw-rw-rw-   0 root         (0) root         (0)     2786 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html
+-rw-rw-rw-   0 root         (0) root         (0)      523 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html
+-rw-rw-rw-   0 root         (0) root         (0)      678 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html
+-rw-rw-rw-   0 root         (0) root         (0)      148 2020-11-09 19:29:14.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/last_updated.html
+-rw-rw-rw-   0 root         (0) root         (0)      572 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2022-02-09 21:55:36.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html
+-rw-rw-rw-   0 root         (0) root         (0)      741 2022-10-13 17:41:55.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html
+-rw-rw-rw-   0 root         (0) root         (0)      626 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html
+-rw-rw-rw-   0 root         (0) root         (0)      554 2020-11-14 02:21:27.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html
+-rw-rw-rw-   0 root         (0) root         (0)      907 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html
+-rw-rw-rw-   0 root         (0) root         (0)      916 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html
+-rw-rw-rw-   0 root         (0) root         (0)     3440 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html
+-rw-rw-rw-   0 root         (0) root         (0)     2674 2022-01-23 15:08:18.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/menu.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.651024 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.651024 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/tabs/
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/tabs/_compliance_color_code.html
+-rw-rw-rw-   0 root         (0) root         (0)      684 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html
+-rw-rw-rw-   0 root         (0) root         (0)      775 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html
+-rw-rw-rw-   0 root         (0) root         (0)      691 2021-02-16 15:13:05.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html
+-rw-rw-rw-   0 root         (0) root         (0)      709 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/solar_system.html
+-rw-rw-rw-   0 root         (0) root         (0)     9420 2022-04-01 19:56:47.000000 aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/reports.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.651024 aa_memberaudit-2.6.3/memberaudit/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:37:37.000000 aa_memberaudit-2.6.3/memberaudit/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      330 2021-01-05 22:10:38.000000 aa_memberaudit-2.6.3/memberaudit/templatetags/memberaudit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.659024 aa_memberaudit-2.6.3/memberaudit/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:37:37.000000 aa_memberaudit-2.6.3/memberaudit/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.659024 aa_memberaudit-2.6.3/memberaudit/tests/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:37:37.000000 aa_memberaudit-2.6.3/memberaudit/tests/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6340 2022-07-14 11:30:46.000000 aa_memberaudit-2.6.3/memberaudit/tests/core/test_core_xml_converter.py
+-rw-rw-rw-   0 root         (0) root         (0)    12708 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.3/memberaudit/tests/core/test_data_exporters.py
+-rw-rw-rw-   0 root         (0) root         (0)    20438 2023-03-27 10:15:12.000000 aa_memberaudit-2.6.3/memberaudit/tests/core/test_eft_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4627 2023-03-27 10:15:12.000000 aa_memberaudit-2.6.3/memberaudit/tests/core/test_fittings.py
+-rw-rw-rw-   0 root         (0) root         (0)     4082 2022-09-03 21:36:22.000000 aa_memberaudit-2.6.3/memberaudit/tests/core/test_skill_plans.py
+-rw-rw-rw-   0 root         (0) root         (0)     2431 2022-09-02 18:40:08.000000 aa_memberaudit-2.6.3/memberaudit/tests/core/test_skills.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.663024 aa_memberaudit-2.6.3/memberaudit/tests/managers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:37:37.000000 aa_memberaudit-2.6.3/memberaudit/tests/managers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18357 2023-02-24 14:11:29.000000 aa_memberaudit-2.6.3/memberaudit/tests/managers/test_character.py
+-rw-rw-rw-   0 root         (0) root         (0)    39823 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/tests/managers/test_general.py
+-rw-rw-rw-   0 root         (0) root         (0)     3382 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/tests/managers/test_sections.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.667024 aa_memberaudit-2.6.3/memberaudit/tests/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:37:37.000000 aa_memberaudit-2.6.3/memberaudit/tests/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    34701 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/tests/models/test_character_1.py
+-rw-rw-rw-   0 root         (0) root         (0)    35834 2023-02-16 19:01:05.000000 aa_memberaudit-2.6.3/memberaudit/tests/models/test_character_2.py
+-rw-rw-rw-   0 root         (0) root         (0)    40698 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/tests/models/test_character_3.py
+-rw-rw-rw-   0 root         (0) root         (0)    28275 2023-03-22 21:45:48.000000 aa_memberaudit-2.6.3/memberaudit/tests/models/test_character_4.py
+-rw-rw-rw-   0 root         (0) root         (0)    10448 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/tests/models/test_general.py
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2023-03-22 22:31:11.000000 aa_memberaudit-2.6.3/memberaudit/tests/models/test_sections.py
+-rw-rw-rw-   0 root         (0) root         (0)     1048 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/tests/models/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    11633 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1807 2023-02-24 17:52:57.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_auth_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_checks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3425 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     4062 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)      889 2022-08-07 14:05:02.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_factories.py
+-rw-rw-rw-   0 root         (0) root         (0)     3516 2022-09-03 16:21:19.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     3813 2023-02-24 17:52:57.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    12216 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_integration.py
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2022-03-05 14:47:06.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_signals.py
+-rw-rw-rw-   0 root         (0) root         (0)    36109 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)      958 2021-05-04 15:11:43.000000 aa_memberaudit-2.6.3/memberaudit/tests/test_templatetags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.679024 aa_memberaudit-2.6.3/memberaudit/tests/testdata/
+-rw-rw-rw-   0 root         (0) root         (0)      267 2020-10-22 17:18:30.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4277 2022-10-12 21:43:27.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/create_eveuniverse.py
+-rw-rw-rw-   0 root         (0) root         (0)     4350 2022-02-10 22:57:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/entities.json
+-rw-rw-rw-   0 root         (0) root         (0)     4703 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/esi_client_stub.py
+-rw-rw-rw-   0 root         (0) root         (0)    40192 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/esi_testdata.json
+-rw-rw-rw-   0 root         (0) root         (0)  1159197 2022-10-12 21:43:27.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/eveuniverse.json
+-rw-rw-rw-   0 root         (0) root         (0)    11769 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.691024 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/
+-rw-rw-rw-   0 root         (0) root         (0)      799 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_archon.txt
+-rw-rw-rw-   0 root         (0) root         (0)      889 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_archon_max.txt
+-rw-rw-rw-   0 root         (0) root         (0)      231 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_empty.txt
+-rw-rw-rw-   0 root         (0) root         (0)      503 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_eve_celestis_no_high_slots.txt
+-rw-rw-rw-   0 root         (0) root         (0)      193 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_eve_tristan_3.txt
+-rw-rw-rw-   0 root         (0) root         (0)      377 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_eve_tristian.txt
+-rw-rw-rw-   0 root         (0) root         (0)      293 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_eve_tristian_2.txt
+-rw-rw-rw-   0 root         (0) root         (0)       96 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_eve_tristian_empty.txt
+-rw-rw-rw-   0 root         (0) root         (0)      583 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_svipul.txt
+-rw-rw-rw-   0 root         (0) root         (0)      432 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_svipul_2.txt
+-rw-rw-rw-   0 root         (0) root         (0)      700 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_tengu.txt
+-rw-rw-rw-   0 root         (0) root         (0)      459 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_tristan.txt
+-rw-rw-rw-   0 root         (0) root         (0)      332 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_tristan_missing_rigs.txt
+-rw-rw-rw-   0 root         (0) root         (0)      410 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_tristan_no_title.txt
+-rw-rw-rw-   0 root         (0) root         (0)      460 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_tristan_unknown_types.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3908 2022-01-20 23:34:01.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/generate_character.py
+-rw-rw-rw-   0 root         (0) root         (0)     3859 2022-01-20 23:34:01.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/generate_doctrines.py
+-rw-rw-rw-   0 root         (0) root         (0)     3671 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/load_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      412 2020-10-22 17:18:30.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/load_eveuniverse.py
+-rw-rw-rw-   0 root         (0) root         (0)     1188 2022-02-10 21:29:55.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/load_locations.py
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/pilot_esi_error_handling.py
+-rw-rw-rw-   0 root         (0) root         (0)      825 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/tests/testdata/profiler_toolbox.py
+-rw-rw-rw-   0 root         (0) root         (0)     3494 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.699024 aa_memberaudit-2.6.3/memberaudit/tests/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:37:37.000000 aa_memberaudit-2.6.3/memberaudit/tests/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7809 2022-09-03 16:21:19.000000 aa_memberaudit-2.6.3/memberaudit/tests/views/test_admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     7079 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/tests/views/test_character_finder.py
+-rw-rw-rw-   0 root         (0) root         (0)    32680 2023-03-22 21:45:48.000000 aa_memberaudit-2.6.3/memberaudit/tests/views/test_character_viewer_1.py
+-rw-rw-rw-   0 root         (0) root         (0)    22475 2022-10-13 12:47:37.000000 aa_memberaudit-2.6.3/memberaudit/tests/views/test_character_viewer_2.py
+-rw-rw-rw-   0 root         (0) root         (0)    14577 2023-03-22 16:51:39.000000 aa_memberaudit-2.6.3/memberaudit/tests/views/test_characters.py
+-rw-rw-rw-   0 root         (0) root         (0)     4091 2022-11-27 20:20:23.000000 aa_memberaudit-2.6.3/memberaudit/tests/views/test_data_export.py
+-rw-rw-rw-   0 root         (0) root         (0)    16230 2022-08-07 14:41:41.000000 aa_memberaudit-2.6.3/memberaudit/tests/views/test_reports.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.699024 aa_memberaudit-2.6.3/memberaudit/tools/
+-rw-rw-rw-   0 root         (0) root         (0)     3051 2022-10-21 18:07:26.000000 aa_memberaudit-2.6.3/memberaudit/tools/drop_tables.sql
+-rw-rw-rw-   0 root         (0) root         (0)      329 2020-12-16 22:00:54.000000 aa_memberaudit-2.6.3/memberaudit/tools/total_size.sql
+-rw-rw-rw-   0 root         (0) root         (0)     7031 2023-03-22 20:57:15.000000 aa_memberaudit-2.6.3/memberaudit/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:38:10.703024 aa_memberaudit-2.6.3/memberaudit/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:37:37.000000 aa_memberaudit-2.6.3/memberaudit/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2022-04-01 19:33:31.000000 aa_memberaudit-2.6.3/memberaudit/views/_common.py
+-rw-rw-rw-   0 root         (0) root         (0)     4636 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/views/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)    12529 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/views/character_finder.py
+-rw-rw-rw-   0 root         (0) root         (0)    25505 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/views/character_viewer_1.py
+-rw-rw-rw-   0 root         (0) root         (0)    22528 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/views/character_viewer_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     7909 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/views/characters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2231 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/views/data_export.py
+-rw-rw-rw-   0 root         (0) root         (0)    13100 2023-04-16 16:03:49.000000 aa_memberaudit-2.6.3/memberaudit/views/reports.py
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-03-27 10:15:12.000000 aa_memberaudit-2.6.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1748 2023-04-16 16:38:10.707024 aa_memberaudit-2.6.3/setup.cfg
```

### Comparing `aa_memberaudit-2.6.2/CHANGELOG.md` & `aa_memberaudit-2.6.3/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/).
 
 ## [Unreleased] - yyyy-mm-dd
 
+## [2.6.3] - 2023-04-16
+
+### Changed
+
+- Added more locations
+
 ## [2.6.2] - 2023-04-11
 
 ### Fixed
 
 - Template files are missing from the distribution package
 
 ## [2.6.1] - 2023-04-08 [YANKED]
```

### Comparing `aa_memberaudit-2.6.2/LICENSE` & `aa_memberaudit-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/PKG-INFO` & `aa_memberaudit-2.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa_memberaudit
-Version: 2.6.2
+Version: 2.6.3
 Summary: An Alliance Auth app that provides full access to Eve characters and related reports for auditing, vetting and monitoring.
 Home-page: https://gitlab.com/ErikKalkoken/aa-memberaudit
 Author: Erik Kalkoken
 Author-email: kalkoken87@gmail.com
 License: MIT
 Keywords: allianceauth,eveonline,memberaudit
 Classifier: Environment :: Web Environment
```

### Comparing `aa_memberaudit-2.6.2/README.md` & `aa_memberaudit-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/aa_memberaudit.egg-info/PKG-INFO` & `aa_memberaudit-2.6.3/aa_memberaudit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-memberaudit
-Version: 2.6.2
+Version: 2.6.3
 Summary: An Alliance Auth app that provides full access to Eve characters and related reports for auditing, vetting and monitoring.
 Home-page: https://gitlab.com/ErikKalkoken/aa-memberaudit
 Author: Erik Kalkoken
 Author-email: kalkoken87@gmail.com
 License: MIT
 Keywords: allianceauth,eveonline,memberaudit
 Classifier: Environment :: Web Environment
```

### Comparing `aa_memberaudit-2.6.2/aa_memberaudit.egg-info/SOURCES.txt` & `aa_memberaudit-2.6.3/aa_memberaudit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 memberaudit/managers/general.py
 memberaudit/managers/sections.py
 memberaudit/migrations/0001_initial_new.py
 memberaudit/migrations/0002_add_mining_ledger.py
 memberaudit/migrations/0003_add_notify_permission.py
 memberaudit/migrations/0004_character_is_disabled.py
 memberaudit/migrations/0005_add_fw_stats.py
+memberaudit/migrations/0006_add_localizations.py
 memberaudit/migrations/__init__.py
 memberaudit/models/__init__.py
 memberaudit/models/character.py
 memberaudit/models/constants.py
 memberaudit/models/general.py
 memberaudit/models/sections.py
 memberaudit/static/memberaudit/css/admin.css
@@ -130,14 +131,15 @@
 memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html
 memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html
 memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html
 memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html
 memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html
 memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html
 memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html
+memberaudit/templates/memberaudit/partials/reports/tabs/_compliance_color_code.html
 memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html
 memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html
 memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html
 memberaudit/templatetags/__init__.py
 memberaudit/templatetags/memberaudit.py
 memberaudit/tests/__init__.py
 memberaudit/tests/test_admin.py
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/admin.py` & `aa_memberaudit-2.6.3/memberaudit/admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             )
             obj.delete()
 
     @admin.display(ordering="group__name")
     def _group_name(self, obj) -> str:
         return obj.group.name
 
-    @admin.display(description="Restricted to states")
+    @admin.display(description=_("Restricted to states"))
     def _states(self, obj):
         states = [state.name for state in obj.group.authgroup.states.all()]
         return sorted(states) if states else "-"
 
     def has_change_permission(self, request, obj=None):
         return False
 
@@ -127,15 +127,15 @@
     def has_delete_permission(self, request, obj=None):
         return False
 
 
 class CharacterUpdateStatusListFilter(admin.SimpleListFilter):
     """Custom filter for update status with counts."""
 
-    title = "update status"
+    title = _("update status")
     parameter_name = "update_status"
 
     def lookups(self, request, model_admin):
         qs = model_admin.get_queryset(request)
         counts = []
         for status in Character.UpdateStatus:
             counts.append((status, qs.filter(update_status=status.value).count()))
@@ -153,15 +153,15 @@
                 return queryset.filter(update_status=value)
         return queryset
 
 
 class CharacterStateListFilter(admin.SimpleListFilter):
     """Custom state filter to include filtering of characters without main."""
 
-    title = "state"
+    title = _("state")
     parameter_name = "state"
     _NO_MAIN_KEY = "_NO_MAIN"
 
     def __init__(self, *args, **kwargs) -> None:
         self._states = State.objects.order_by("-priority").values_list(
             "name", flat=True
         )
@@ -207,15 +207,15 @@
 
     list_display = (
         "_character_pic",
         "_character",
         "_main",
         "_state",
         "_organization",
-        "created_at",
+        "_created_at",
         "_enabled",
         "_last_update_at",
         "_update_status",
         "_missing_sections",
     )
     list_display_links = (
         "_character_pic",
@@ -255,75 +255,82 @@
         """Remove the default delete action from the drop-down."""
         actions = super().get_actions(request)
         if "delete_selected" in actions:
             del actions["delete_selected"]
         return actions
 
     @admin.display(description="")
-    def _character_pic(self, obj):
+    def _character_pic(self, obj: Character):
         character = obj.eve_character
         return format_html(
             '<img src="{}" class="img-circle">', character.portrait_url(size=32)
         )
 
-    @admin.display(ordering="eve_character__character_name")
-    def _character(self, obj) -> str:
+    @admin.display(ordering="eve_character__character_name", description=_("character"))
+    def _character(self, obj: Character) -> str:
         return str(obj.eve_character)
 
-    @admin.display(ordering="is_disabled", boolean=True)
-    def _enabled(self, obj) -> bool:
+    @admin.display(ordering="is_disabled", boolean=True, description=_("enabled"))
+    def _enabled(self, obj: Character) -> bool:
         return not obj.is_disabled
 
     @admin.display(
-        ordering="eve_character__character_ownership__user__profile__main_character"
+        ordering="eve_character__character_ownership__user__profile__main_character",
+        description=_("main"),
     )
-    def _main(self, obj) -> str:
+    def _main(self, obj: Character) -> str:
         try:
             name = obj.main_character.character_name
         except AttributeError:
             return None
         return str(name)
 
     @admin.display(
-        ordering="eve_character__character_ownership__user__profile__state__name"
+        ordering="eve_character__character_ownership__user__profile__state__name",
+        description=_("state"),
     )
-    def _state(self, obj) -> str:
+    def _state(self, obj: Character) -> str:
         try:
             return str(obj.user.profile.state)
         except AttributeError:
             return None
 
     @admin.display(
-        ordering="eve_character__character_ownership__user__profile__main_character__corporation_name"
+        ordering="eve_character__character_ownership__user__profile__main_character__corporation_name",
+        description=_("organization"),
     )
-    def _organization(self, obj) -> str:
+    def _organization(self, obj: Character) -> str:
         try:
             return "{}{}".format(
                 obj.main_character.corporation_name,
                 f" [{obj.main_character.alliance_ticker}]"
                 if obj.main_character.alliance_ticker
                 else "",
             )
         except AttributeError:
             return None
 
-    @admin.display(ordering="update_status")
-    def _update_status(self, obj):
+    @admin.display(ordering="update_status", description=_("update status"))
+    def _update_status(self, obj: Character):
         css_class_map = {
             Character.UpdateStatus.INCOMPLETE: "text-warning",
             Character.UpdateStatus.ERROR: "text-danger",
             Character.UpdateStatus.DISABLED: "text-muted",
         }
         label = Character.UpdateStatus(obj.update_status).label.title()
         if css_class := css_class_map.get(obj.update_status):
             return format_html('<span class="{}">{}</span>', css_class, label)
         return label
 
-    @admin.display(ordering="last_update_at")
-    def _last_update_at(self, obj):
+    @admin.display(ordering="created_at", description=_("created"))
+    def _created_at(self, obj: Character):
+        return obj.created_at
+
+    @admin.display(ordering="last_update_at", description=_("last update"))
+    def _last_update_at(self, obj: Character):
         return obj.last_update_at
 
     def _missing_sections(self, obj):
         existing = {x.section for x in obj.update_status_set.all()}
         all_sections = set(Character.UpdateSection.values)
         missing = all_sections.difference(existing)
         if missing:
@@ -338,118 +345,137 @@
         "update_assets",
         "update_location",
         "update_online_status",
         "enable_characters",
         "disable_characters",
     ]
 
-    @admin.display(description="Delete selected characters")
+    @admin.display(description=_("Delete selected characters"))
     def delete_characters(self, request, queryset):
         if "apply" in request.POST:
             for obj in queryset:
                 tasks.delete_character.apply_async(
                     kwargs={"character_pk": obj.pk},
                     priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
                 )
             self.message_user(
                 request,
-                f"Started deleting {queryset.count()} character(s). "
-                "This can take a minute.",
+                _(
+                    "Started deleting %d character(s). "
+                    "This can take a minute." % queryset.count()
+                ),
             )
             return redirect(request.get_full_path())
         return render(
             request,
             "admin/memberaudit/character/confirm_character_deletion.html",
             {
-                "title": "Are you sure you want to delete these characters?",
+                "title": _("Are you sure you want to delete these characters?"),
                 "queryset": queryset.all(),
             },
         )
 
-    @admin.display(description="Update selected characters from EVE server")
+    @admin.display(description=_("Update selected characters from EVE server"))
     def update_characters(self, request, queryset):
         for obj in queryset:
             tasks.update_character.apply_async(
                 kwargs={"character_pk": obj.pk, "force_update": True},
                 priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
             )
-            self.message_user(request, f"Started updating character: {obj}. ")
+            self.message_user(request, _("Started updating character: %s. " % obj))
 
-    @admin.display(description="Update assets for selected characters from EVE server")
+    @admin.display(
+        description=_("Update assets for selected characters from EVE server")
+    )
     def update_assets(self, request, queryset):
         for obj in queryset:
             tasks.update_character_assets.apply_async(
                 kwargs={"character_pk": obj.pk, "force_update": True},
                 priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
             )
             self.message_user(
-                request, f"Started updating assets for character: {obj}. "
+                request, _("Started updating assets for character: %s." % obj)
             )
 
     @admin.display(
         description=(
-            f"Update {Character.UpdateSection.display_name(Character.UpdateSection.LOCATION)} "
-            "for selected characters from EVE server"
+            _(
+                "Update %s for selected characters from EVE server"
+                % {
+                    Character.UpdateSection.display_name(
+                        Character.UpdateSection.LOCATION
+                    )
+                }
+            )
         )
     )
     def update_location(self, request, queryset):
         section = Character.UpdateSection.LOCATION
         for obj in queryset:
             tasks.update_character_section.apply_async(
                 kwargs={"character_pk": obj.pk, "section": section},
                 priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
             )
             self.message_user(
                 request,
-                f"Started updating {Character.UpdateSection.display_name(section)} for character: {obj}. ",
+                _(
+                    "Started updating %s for character: %s. "
+                    % (Character.UpdateSection.display_name(section), obj)
+                ),
             )
 
     @admin.display(
         description=(
-            "Update "
-            f"{Character.UpdateSection.display_name(Character.UpdateSection.ONLINE_STATUS)} "
-            "for selected characters from EVE server"
+            _(
+                "Update %s for selected characters from EVE server"
+                % Character.UpdateSection.display_name(
+                    Character.UpdateSection.ONLINE_STATUS
+                )
+            )
         )
     )
     def update_online_status(self, request, queryset):
         section = Character.UpdateSection.ONLINE_STATUS
         for obj in queryset:
             tasks.update_character_section.apply_async(
                 kwargs={"character_pk": obj.pk, "section": section},
                 priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
             )
             self.message_user(
                 request,
-                f"Started updating {Character.UpdateSection.display_name(section)} for character: {obj}. ",
+                _(
+                    "Started updating %s for character: %s."
+                    % (Character.UpdateSection.display_name(section), obj)
+                ),
             )
 
-    @admin.display(description=("Enable selected characters"))
+    @admin.display(description=_("Enable selected characters"))
     def enable_characters(self, request, queryset):
         pks = list(queryset.values_list("pk", flat=True))
         queryset.filter(pk__in=pks).update(is_disabled=False)
-        self.message_user(request, f"Enabled {len(pks)} characters.")
+        self.message_user(request, _("Enabled %d characters." % len(pks)))
 
-    @admin.display(description=("Disable selected characters"))
+    @admin.display(description=_("Disable selected characters"))
     def disable_characters(self, request, queryset):
         pks = list(queryset.values_list("pk", flat=True))
         queryset.filter(pk__in=pks).update(is_disabled=True)
-        self.message_user(request, f"Disabled {len(pks)} characters.")
+        self.message_user(request, _("Disabled %d characters." % len(pks)))
 
     inlines = (SyncStatusAdminInline,)
 
     def has_add_permission(self, request):
         return False
 
     def has_change_permission(self, request, obj=None):
         return False
 
 
 @admin.register(Location)
 class LocationAdmin(admin.ModelAdmin):
-    list_display = ("id", "_name", "_type", "_group", "_solar_system", "updated_at")
+    list_display = ("id", "_name", "_type", "_group", "_solar_system", "_updated_at")
     list_filter = (
         ("eve_type__eve_group__eve_category", admin.RelatedOnlyFieldListFilter),
         ("eve_type__eve_group", admin.RelatedOnlyFieldListFilter),
     )
     search_fields = [
         "id",
         "name",
@@ -460,30 +486,34 @@
         "eve_type__eve_group",
         "eve_type",
         "eve_solar_system__eve_constellation__eve_region",
         "eve_solar_system",
     )
     ordering = ["id"]
 
-    @admin.display(ordering="name")
+    @admin.display(ordering="name", description=_("name"))
     def _name(self, obj):
         return obj.name_plus
 
-    @admin.display(ordering="eve_solar_system__name")
+    @admin.display(ordering="eve_solar_system__name", description=_("solar system"))
     def _solar_system(self, obj):
         return obj.eve_solar_system.name if obj.eve_solar_system else None
 
-    @admin.display(ordering="eve_type__name")
+    @admin.display(ordering="eve_type__name", description=_("type"))
     def _type(self, obj):
         return obj.eve_type.name if obj.eve_type else None
 
-    @admin.display(ordering="eve_type__eve_group__name")
+    @admin.display(ordering="eve_type__eve_group__name", description=_("group"))
     def _group(self, obj):
         return obj.eve_type.eve_group.name if obj.eve_type else None
 
+    @admin.display(ordering="updated_at", description=_("updated at"))
+    def _updated_at(self, obj):
+        return obj.name_plus
+
     def has_add_permission(self, request):
         return False
 
     def has_change_permission(self, request, obj=None):
         return False
 
 
@@ -533,15 +563,15 @@
                         row
                         and row.get("DELETE") is False
                         and not row.get("required_level")
                         and not row.get("recommended_level")
                     ):
                         eve_type = row.get("eve_type")
                         raise ValidationError(
-                            f"Skill '{eve_type.name}' must have a level."
+                            _("Skill '%s' must have a level.", eve_type.name)
                         )
 
 
 class SkillSetSkillAdminInline(MinValidatedInlineMixIn, admin.TabularInline):
     model = SkillSetSkill
     verbose_name = "skill"
     verbose_name_plural = "skills"
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/app_settings.py` & `aa_memberaudit-2.6.3/memberaudit/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/auth_hooks.py` & `aa_memberaudit-2.6.3/memberaudit/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/checks.py` & `aa_memberaudit-2.6.3/memberaudit/checks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/constants.py` & `aa_memberaudit-2.6.3/memberaudit/constants.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/core/data_exporters.py` & `aa_memberaudit-2.6.3/memberaudit/core/data_exporters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/core/eft_parser.py` & `aa_memberaudit-2.6.3/memberaudit/core/eft_parser.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/core/fittings.py` & `aa_memberaudit-2.6.3/memberaudit/core/fittings.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/core/skill_plans.py` & `aa_memberaudit-2.6.3/memberaudit/core/skill_plans.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/core/skills.py` & `aa_memberaudit-2.6.3/memberaudit/core/skills.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/core/xml_converter.py` & `aa_memberaudit-2.6.3/memberaudit/core/xml_converter.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/decorators.py` & `aa_memberaudit-2.6.3/memberaudit/decorators.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/forms.py` & `aa_memberaudit-2.6.3/memberaudit/forms.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/helpers.py` & `aa_memberaudit-2.6.3/memberaudit/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/management/commands/memberaudit_data_export.py` & `aa_memberaudit-2.6.3/memberaudit/management/commands/memberaudit_data_export.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/management/commands/memberaudit_load_eve.py` & `aa_memberaudit-2.6.3/memberaudit/management/commands/memberaudit_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/management/commands/memberaudit_reset_characters.py` & `aa_memberaudit-2.6.3/memberaudit/management/commands/memberaudit_reset_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/management/commands/memberaudit_stats.py` & `aa_memberaudit-2.6.3/memberaudit/management/commands/memberaudit_stats.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/management/commands/memberaudit_update_characters.py` & `aa_memberaudit-2.6.3/memberaudit/management/commands/memberaudit_update_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/managers/character.py` & `aa_memberaudit-2.6.3/memberaudit/managers/character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/managers/general.py` & `aa_memberaudit-2.6.3/memberaudit/managers/general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/managers/sections.py` & `aa_memberaudit-2.6.3/memberaudit/managers/sections.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/migrations/0001_initial_new.py` & `aa_memberaudit-2.6.3/memberaudit/migrations/0001_initial_new.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/migrations/0002_add_mining_ledger.py` & `aa_memberaudit-2.6.3/memberaudit/migrations/0002_add_mining_ledger.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/migrations/0003_add_notify_permission.py` & `aa_memberaudit-2.6.3/memberaudit/migrations/0003_add_notify_permission.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/migrations/0004_character_is_disabled.py` & `aa_memberaudit-2.6.3/memberaudit/migrations/0004_character_is_disabled.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/migrations/0005_add_fw_stats.py` & `aa_memberaudit-2.6.3/memberaudit/migrations/0005_add_fw_stats.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/models/__init__.py` & `aa_memberaudit-2.6.3/memberaudit/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/models/character.py` & `aa_memberaudit-2.6.3/memberaudit/models/character.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,26 +142,36 @@
         IN_PROGRESS = "in_progress", _("in progress")
         INCOMPLETE = "incomplete", _("incomplete")
         ERROR = "error", _("error")
         DISABLED = "disabled", _("disabled")
 
     id = models.AutoField(primary_key=True)
     eve_character = models.OneToOneField(
-        EveCharacter, related_name="memberaudit_character", on_delete=models.CASCADE
+        EveCharacter,
+        related_name="memberaudit_character",
+        on_delete=models.CASCADE,
+        verbose_name=_("eve character"),
     )
 
-    created_at = models.DateTimeField(auto_now_add=True, db_index=True)
+    created_at = models.DateTimeField(
+        auto_now_add=True, db_index=True, verbose_name=_("created at")
+    )
     is_shared = models.BooleanField(
         default=False,
+        verbose_name=_("is shared"),
         help_text="Shared characters can be viewed by recruiters",
     )
     is_disabled = models.BooleanField(
-        default=False, help_text="Disabled characters are no longer updated from ESI."
+        default=False,
+        verbose_name=_("is disabled"),
+        help_text="Disabled characters are no longer updated from ESI.",
+    )
+    mailing_lists = models.ManyToManyField(
+        "MailEntity", related_name="characters", verbose_name=_("mailing lists")
     )
-    mailing_lists = models.ManyToManyField("MailEntity", related_name="characters")
 
     objects = CharacterManager()
 
     class Meta:
         default_permissions = ()
 
     def __str__(self) -> str:
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/models/general.py` & `aa_memberaudit-2.6.3/memberaudit/models/general.py`

 * *Files 4% similar despite different names*

```diff
@@ -252,28 +252,34 @@
 
     objects = EveSkillTypeManger()
 
 
 class SkillSetGroup(models.Model):
     """A group of SkillSets, e.g. for defining a doctrine"""
 
-    name = models.CharField(max_length=NAMES_MAX_LENGTH, unique=True)
-    description = models.TextField(blank=True)
-    skill_sets = models.ManyToManyField("SkillSet", related_name="groups")
+    name = models.CharField(
+        max_length=NAMES_MAX_LENGTH, unique=True, verbose_name=_("name")
+    )
+    description = models.TextField(blank=True, verbose_name=_("description"))
+    skill_sets = models.ManyToManyField(
+        "SkillSet", related_name="groups", verbose_name=_("skill sets")
+    )
     is_doctrine = models.BooleanField(
         default=False,
         db_index=True,
+        verbose_name=_("is doctrine"),
         help_text=(
-            "This enables a skill set group to show up correctly in doctrine reports"
+            _("This enables a skill set group to show up correctly in doctrine reports")
         ),
     )
     is_active = models.BooleanField(
         default=True,
         db_index=True,
-        help_text="Whether this skill set group is in active use",
+        verbose_name=_("is active"),
+        help_text=_("Whether this skill set group is in active use"),
     )
 
     def __str__(self) -> str:
         return str(self.name)
 
     @property
     def name_plus(self) -> str:
@@ -281,32 +287,38 @@
 
 
 class SkillSet(models.Model):
     """A set of required and recommended skills needed to perform
     a particular task like flying a doctrine ships.
     """
 
-    name = models.CharField(max_length=NAMES_MAX_LENGTH, unique=True)
-    description = models.TextField(blank=True)
+    name = models.CharField(
+        max_length=NAMES_MAX_LENGTH, unique=True, verbose_name=_("name")
+    )
+    description = models.TextField(blank=True, verbose_name=_("description"))
     ship_type = models.ForeignKey(
         EveShipType,
         on_delete=models.SET_DEFAULT,
         default=None,
         null=True,
         blank=True,
         related_name="+",
+        verbose_name=_("ship type"),
         help_text=(
-            "Ship type is used for visual presentation only. "
-            "All skill requirements must be explicitly defined."
+            _(
+                "Ship type is used for visual presentation only. "
+                "All skill requirements must be explicitly defined."
+            )
         ),
     )
     is_visible = models.BooleanField(
         default=True,
         db_index=True,
-        help_text=(
+        verbose_name=_("is visible"),
+        help_text=_(
             "Non visible skill sets are not shown to users "
             "on their character sheet and used for audit purposes only."
         ),
     )
 
     objects = SkillSetManager()
 
@@ -314,31 +326,39 @@
         return str(self.name)
 
 
 class SkillSetSkill(models.Model):
     """A specific skill within a skill set."""
 
     skill_set = models.ForeignKey(
-        SkillSet, on_delete=models.CASCADE, related_name="skills"
+        SkillSet,
+        on_delete=models.CASCADE,
+        related_name="skills",
+        verbose_name=_("skills"),
     )
     eve_type = models.ForeignKey(
-        EveSkillType, on_delete=models.CASCADE, verbose_name="skill", related_name="+"
+        EveSkillType,
+        on_delete=models.CASCADE,
+        verbose_name=_("skill"),
+        related_name="+",
     )
 
     required_level = models.PositiveIntegerField(
         default=None,
         null=True,
         blank=True,
         validators=[MinValueValidator(1), MaxValueValidator(5)],
+        verbose_name=_("required level"),
     )
     recommended_level = models.PositiveIntegerField(
         default=None,
         null=True,
         blank=True,
         validators=[MinValueValidator(1), MaxValueValidator(5)],
+        verbose_name=_("recommended level"),
     )
 
     class Meta:
         constraints = [
             models.UniqueConstraint(
                 fields=["skill_set", "eve_type"],
                 name="functional_pk_skillsetskill",
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/models/sections.py` & `aa_memberaudit-2.6.3/memberaudit/models/sections.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/character_viewer.css` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/character_viewer.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/character_viewer.min.css` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/character_viewer.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/global.css` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/global.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/global.min.css` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/global.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/launcher.css` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/launcher.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/launcher.min.css` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/launcher.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/memberaudit.css` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/memberaudit.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/memberaudit.min.css` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/memberaudit.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/css/reports.css` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/css/reports.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/charisma.png` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/charisma.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/eve-prism.png` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/eve-prism.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/evesearch.png` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/evesearch.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/intelligence.png` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/intelligence.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/memory.png` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/memory.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/perception.png` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/perception.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/images/willpower.png` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/images/willpower.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/static/memberaudit/vendor/moment/moment.min.js` & `aa_memberaudit-2.6.3/memberaudit/static/memberaudit/vendor/moment/moment.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/swagger.json` & `aa_memberaudit-2.6.3/memberaudit/swagger.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tasks.py` & `aa_memberaudit-2.6.3/memberaudit/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html` & `aa_memberaudit-2.6.3/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,20 @@
- {% extends 'admin/base_site.html' %}
+{% extends 'admin/base_site.html' %}
+{% load i18n %}
 
- {% block content %}
- <form action="" method="post">
+{% block content %}
+<form action="" method="post">
     {% csrf_token %}
     <div>
         <ul>
         {% for character in queryset %}
             <input type="hidden" name="_selected_action" value="{{ character.pk }}" />
             <li>{{ character.name }} </li>
         {% endfor %}
         </ul>
         <br>
         <input type="hidden" name="action" value="delete_characters" />
-        <input type="submit" name="apply" value="Delete" style="background-color: rgb(201, 48, 44)"/>
-        <a href="./"><input type="button" name="Cancel" value="Cancel"></a>
+        <input type="submit" name="apply" value="{% translate 'Delete' %}" style="background-color: rgb(201, 48, 44)"/>
+        <a href="./"><input type="button" name="Cancel" value="{% translate 'Cancel' %}"></a>
     </div>
- </form>
- {% endblock %}
+</form>
+{% endblock %}
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
- {% extends 'admin/base_site.html' %} {% block content %}
+{% extends 'admin/base_site.html' %} {% load i18n %} {% block content %}
 {% csrf_token %}
     * {% for character in queryset %}
     * {{ character.name }}
     * {% endfor %}
 
- [Delete] [Unknown_INPUT_type]
+ [{% translate 'Delete' %}] [Unknown_INPUT_type]
 {% endblock %}
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/admin/memberaudit/skillset/import_skills.html` & `aa_memberaudit-2.6.3/memberaudit/templates/admin/memberaudit/skillset/import_skills.html`

 * *Files 7% similar despite different names*

```diff
@@ -14,11 +14,11 @@
     <form action="" method="post">
         {% csrf_token %}
         {{ form.as_p }}
         <br>
         <br>
         <input type="submit" value="Submit">
         <a href="{% url 'admin:memberaudit_skillset_changelist' %}">
-            <input type="button" name="Cancel" value="Cancel">
+            <input type="button" name="Cancel" value="{% translate 'Cancel' %}">
         </a>
     </form>
 {% endblock %}
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/character_finder.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/character_finder.html`

 * *Files 9% similar despite different names*

```diff
@@ -24,16 +24,16 @@
                         </tr>
                     </thead>
 
                     <tbody></tbody>
                 </table>
             </div>
             <p class="text-muted">
-                <i class="fas fa-crown"></i> Main character&nbsp;•&nbsp;
-                <i class="far fa-eye"></i> Currently shared with recruiters
+                <i class="fas fa-crown"></i> {% translate 'Main character' %}&nbsp;•&nbsp;
+                <i class="far fa-eye"></i> {% translate 'Currently shared with others' %}
             </p>
         </div>
     </div>
 {% endblock details %}
 
 {% block extra_javascript %}
     {% include 'bundles/datatables-js.html' %}
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/character_viewer.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/character_viewer.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/data_export.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/data_export.html`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,18 @@
     <div class="panel panel-default">
         <div class="panel-heading" style="display:flex;">
             <h3 class="panel-title">{% translate 'Topics' %}</h3>
         </div>
         <div class="panel-body">
             <table id="tbl_data_exports" class="table table-striped">
                 <thead>
-                    <th>Name</th>
-                    <th>Description</th>
-                    <th>Rows</th>
-                    <th>Export file age</th>
+                    <th>{% translate 'Name' %}</th>
+                    <th>{% translate 'Description' %}</th>
+                    <th>{% translate 'Rows' %}</th>
+                    <th>{% translate 'Export file age' %}</th>
                     <th></th>
                 </thead>
                 <tbody>
                     {% for topic in topics %}
                         <tr>
                             <td>{{ topic.title }}</td>
                             <td>{{ topic.description }}</td>
@@ -38,15 +38,19 @@
                                 {% endif %}
                             </td>
                         </tr>
                     {% endfor %}
                 </tbody>
             </table>
             <p class="text-muted">
-                Export files contain the complete data of all <strong>{{ character_count|intcomma }}</strong> characters known to Member Audit. They are in CSV format and zipped. Existing export files can updated after {{ minutes_until_next_update }} minutes.
+                {% blocktranslate with amount_of_characters=character_count|intcomma %}
+                    Export files contain the complete data of all <strong>{{ amount_of_characters }}</strong>
+                    characters known to Member Audit. They are in CSV format and zipped.
+                    Existing export files can updated after {{ minutes_until_next_update }} minutes.
+                {% endblocktranslate %}
             </p>
         </div>
     </div>
 {% endblock details %}
 
 {% block extra_css %}
     <link rel="stylesheet" href="{% static 'memberaudit/css/global.css' %}" type="text/css">
```

#### html2text {}

```diff
@@ -5,14 +5,16 @@
                                                                                            %} Download {% else
 {           {                 {                   {                                        %} Download {% endif
 {           {                 {                   {                                        %} {% if
 topic.title topic.description topic.rows|intcomma topic.last_updated_at|timesince|default: topic.update_allowed
 }}          }}                }}                  "no file" }}                             %} Update_now {%
                                                                                            else %} Update_now
                                                                                            {% endif %}
-Export files contain the complete data of all {{ character_count|intcomma }}
-characters known to Member Audit. They are in CSV format and zipped. Existing
-export files can updated after {{ minutes_until_next_update }} minutes.
+{% blocktranslate with amount_of_characters=character_count|intcomma %} Export
+files contain the complete data of all {{ amount_of_characters }} characters
+known to Member Audit. They are in CSV format and zipped. Existing export files
+can updated after {{ minutes_until_next_update }} minutes. {% endblocktranslate
+%}
 {% endblock details %} {% block extra_css %}
 
 
  {% endblock %} {% block extra_script %} {% endblock %}
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/launcher.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/launcher.html`

 * *Files 7% similar despite different names*

```diff
@@ -35,18 +35,18 @@
                         <!-- Registered Characters -->
                         {% for auth_character in auth_characters|dictsort:"character_name" %}
                             <li class="cards_item">
                                 <div class="card">
                                     <div class="card-header">
                                         {{ auth_character.character_name }}
                                         {% if auth_character.character_id == main_character_id %}
-                                            &nbsp;<i class="fas fa-crown" title="Main character"></i>
+                                            &nbsp;<i class="fas fa-crown" title="{% translate 'Main character' %}"></i>
                                         {% endif %}
                                         {% if auth_character.character.is_shared %}
-                                            &nbsp;<i class="far fa-eye" title="Currently shared with recruiters"></i>
+                                            &nbsp;<i class="far fa-eye" title="{% translate 'Main Currently shared with recruiters' %}"></i>
                                         {% endif %}
                                     </div>
 
                                     <div class="card-body card__content">
                                         <p>
                                             <a href="{% url 'memberaudit:character_viewer' auth_character.character.pk %}">
                                                 <span class="aa-memberaudit-launcher-character-image">
@@ -85,26 +85,28 @@
                                         {% if perms.memberaudit.share_characters %}
                                             {% if auth_character.character.is_shared %}
                                                 <a class="btn btn-primary btn-sm" href="{% url 'memberaudit:unshare_character' auth_character.character.pk %}"
                                                     role="button" title="{% translate 'Disable access to this character for recruiters.' %}">
                                                     <i class="far fa-eye-slash"></i>
                                                 </a>
                                             {% else %}
+                                                {% blocktranslate asvar confirm_share_message %}Are you sure you want to allow others to see this character?{% endblocktranslate %}
                                                 <a class="btn btn-warning btn-sm" href="{% url 'memberaudit:share_character' auth_character.character.pk %}"
                                                     role="button"
-                                                    onclick="return confirm('Are you sure you want to SHARE this character?')"
-                                                    title="{% translate 'Enable access to this character for recruiters.' %}">
+                                                    onclick="return confirm('{{ confirm_share_message }}')"
+                                                    title="{% translate 'Allow others to see this character.' %}">
                                                     <i class="far fa-eye"></i>
                                                 </a>
                                             {% endif %}
                                         {% endif %}
 
+                                        {% blocktranslate asvar confirm_remove_message %}Are you sure you want to remove this character?{% endblocktranslate %}
                                         <a class="btn btn-danger btn-sm" href="{% url 'memberaudit:remove_character' auth_character.character.pk %}"
                                             role="button" title="{% translate 'Remove this character.' %}"
-                                            onclick="return confirm('Are you sure you want to REMOVE this character?')">
+                                            onclick="return confirm('{{ confirm_remove_message }}')">
                                             <i class="far fa-trash-alt"></i>
                                         </a>
                                     </div>
                                 </div>
                             </li>
                         {% endfor %}
                     {% endif %}
@@ -117,16 +119,16 @@
                     <i class="fas fa-exclamation-triangle"></i>
                     {% translate 'Unregistered character(s):' %}&nbsp;&nbsp;</strong>
                     {{ unregistered_chars|join:", " }}
                 </p>
             {% endif %}
 
             <p class="text-muted">
-                <i class="fas fa-crown"></i> Main character&nbsp;•&nbsp;
-                <i class="far fa-eye"></i> Currently shared with recruiters
+                <i class="fas fa-crown"></i> {% translate 'Main character' %}&nbsp;•&nbsp;
+                <i class="far fa-eye"></i> {% translate 'Currently shared with others' %}
             </p>
         </div>
     </div>
 
 {% endblock details %}
 
 {% block extra_javascript %}
```

#### html2text {}

```diff
@@ -15,20 +15,24 @@
       {% include 'memberaudit/partials/solar_system.html' with
       character=auth_character.character only %}
       {% if auth_character.character.wallet_balance %} {
       { auth_character.character.wallet_balance.total|intword|default_if_none:
       "-" }} ISK
       {% else %} {% translate "(no data yet)" %} {% endif %}
        {% if perms.memberaudit.share_characters %} {% if
-      auth_character.character.is_shared %}  {% else %}  {% endif %} {% endif
-      %}
+      auth_character.character.is_shared %}  {% else %} {% blocktranslate asvar
+      confirm_share_message %}Are you sure you want to allow others to see this
+      character?{% endblocktranslate %}  {% endif %} {% endif %} {%
+      blocktranslate asvar confirm_remove_message %}Are you sure you want to
+      remove this character?{% endblocktranslate %}
     * {% endfor %} {% endif %}
 {% if unregistered_chars|length > 0 %}
  {% translate 'Unregistered character(s):' %}  
  {{ unregistered_chars|join:", " }}
 {% endif %}
- Main character â¢   Currently shared with recruiters
+ {% translate 'Main character' %} â¢   {% translate 'Currently shared with
+others' %}
 {% endblock details %} {% block extra_javascript %} {% endblock %} {% block
 extra_css %}
 
 
  {% endblock %} {% block extra_script %} {% endblock %}
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/modals/character_viewer/contract.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/contract.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html`

 * *Files 6% similar despite different names*

```diff
@@ -65,18 +65,18 @@
                             <p>{{ contract.reward|floatformat:2|intcomma }} {% translate 'ISK' %}</p>
                         {% endif %}
                         {% if has_items_included %}
                             {% include "memberaudit/modals/character_viewer/contract_items.html" with table_name="tab_contract_items_included" %}
                         {% endif %}
                     {% endif %}
                 {% elif contract.contract_type == contract.TYPE_AUCTION %}
-                    <dt>Starting Bid:</dt> <dd>{{ contract.price|floatformat:2|intcomma }}</dd>
-                    <dt>Buyout Price:</dt> <dd>{{ contract.buyout|floatformat:2|intcomma }}</dd>
-                    <dt>Current Bid:</dt> <dd>{{ current_bid|floatformat:2|intcomma }} ({{ bids_count }} {% translate 'so far' %})</dd>
-                    <dt>Time Left:</dt> <dd>{{ contract.date_expired|timeuntil }}</dd>
+                    <dt>{% translate 'Starting Bid:' %}</dt> <dd>{{ contract.price|floatformat:2|intcomma }}</dd>
+                    <dt>{% translate 'Buyout Price:' %}</dt> <dd>{{ contract.buyout|floatformat:2|intcomma }}</dd>
+                    <dt>{% translate 'Current Bid:' %}</dt> <dd>{{ current_bid|floatformat:2|intcomma }} ({{ bids_count }} {% translate 'so far' %})</dd>
+                    <dt>{% translate 'Time Left:' %}</dt> <dd>{{ contract.date_expired|timeuntil }}</dd>
 
                     <hr>
 
                     <h4 class="text-success">{% translate 'Buyer will get' %}</h4>
                     {% if has_items_included %}
                         {% include "memberaudit/modals/character_viewer/contract_items.html" with table_name="tab_contract_items_included" %}
                     {% endif %}
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html`

 * *Files 8% similar despite different names*

```diff
@@ -16,13 +16,13 @@
 
     <tfoot>
         <tr>
             <th></th>
             <th></th>
             <th></th>
             <th></th>
-            <th>Grand Total:</th>
+            <th>{% translate 'Grand Total:' %}</th>
             <th></th>
         </tr>
     </tfoot>
 
 </table>
```

#### html2text {}

```diff
@@ -1,4 +1,6 @@
 {% load i18n %}
-{% translate {% translate {% translate {% translate  {% translate {% translate
-'Name' %}    'Qty' %}     'Type' %}    'Category' %} 'Price' %}   'Total' %}
-                                                     Grand Total:
+{% translate {% translate {% translate {% translate  {% translate  {% translate
+'Name' %}    'Qty' %}     'Type' %}    'Category' %} 'Price' %}    'Total' %}
+                                                     {% translate
+                                                     'Grand Total:
+                                                     ' %}
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/modals/character_viewer/mail.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/mail.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/overview.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/overview.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 {% load i18n %}
 {% load static %}
 {% load evelinks %}
 
 <!-- Sidebar panel-->
 <div class="panel panel-default">
-    <div class="panel-heading">Characters</div>
+    <div class="panel-heading">{% translate 'Characters' %}</div>
     <div class="panel-body">
         <ul class="sidebar_characters">
             {% for character in all_characters %}
                 {% if character.memberaudit_character_pk and character.has_access%}
                     <li class="sidebar_character character-{{ character.memberaudit_character_pk }}{% if auth_character.character_name == character.character_name %} active{% endif %}">
                         <a href="{% url 'memberaudit:character_viewer' character.memberaudit_character_pk %}">
                             {% include "memberaudit/partials/character_viewer/sidebar_character.html" %}
                         </a>
                     </li>
                 {% else %}
                     <li class="sidebar_character_disabled">
                         {% include "memberaudit/partials/character_viewer/sidebar_character.html" %}&nbsp;
-                        <i class="fas fa-exclamation-triangle text-muted" title="Unregistered character"></i>
+                        <i class="fas fa-exclamation-triangle text-muted" title="{% translate 'Unregistered character' %}"></i>
                     </li>
                 {% endif %}
             {% empty %}
-                <li class="sidebar_character_disabled"><span class="text-muted">(orphan)</span></li>
+                <li class="sidebar_character_disabled">
+                    <span class="text-muted">{% translate '(orphan)' %}</span>
+                </li>
             {% endfor %}
         </ul>
     </div>
 </div>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% load i18n %} {% load static %} {% load evelinks %}
-Characters
+{% translate 'Characters' %}
     * {% for character in all_characters %} {% if
       character.memberaudit_character_pk and character.has_access%}
     * {%_include_"memberaudit/partials/character_viewer/sidebar_character.html"
       %}
     * {% else %}
     * {% include "memberaudit/partials/character_viewer/sidebar_character.html"
       %} 
     * {% endif %} {% empty %}
-    * (orphan)
+    * {% translate '(orphan)' %}
     * {% endfor %}
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 {% load i18n %}
 {% load evelinks %}
 
-<img height="20" width="20" src="{{ character.character_id|character_portrait_url:32 }}"/>
-<span
-    {% if not character.memberaudit_character_pk %}class="text-muted"{% endif%}>{{ character.character_name }}
+<span class="nowrap">
+    <img height="20" width="20" src="{{ character.character_id|character_portrait_url:32 }}"/>
+    <span {% if not character.memberaudit_character_pk %}class="text-muted"{% endif%}>
+        {{ character.character_name }}
 
-    {% if character.character_id == main_character_id %}
-        &nbsp;<i class="fas fa-crown" title="{% translate 'Main character' %}"></i>
-    {% endif %}
+        {% if character.character_id == main_character_id %}
+            &nbsp;<i class="fas fa-crown" title="{% translate 'Main character' %}"></i>
+        {% endif %}
 
-    {% if character.is_shared %}
-        &nbsp;<i class="far fa-eye" title="{% translate 'Currently shared with recruiters' %}"></i>
-    {% endif %}
+        {% if character.is_shared %}
+            &nbsp;<i class="far fa-eye" title="{% translate 'Currently shared with recruiters' %}"></i>
+        {% endif %}
+    </span>
 </span>
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-{% load i18n %}
 {% load static %}
+{% load i18n %}
+{% load humanize %}
 
-<div role="tabpanel" class="tab-pane" id="attributes">
-
-     <div id="div_character_attributes">
+<div role="tabpanel" class="tab-pane" id="history">
+    <div id="div_corporation_history">
         {% if NIGHT_MODE %}
             <img src="{% static 'memberaudit/images/Spinner-1s-64px-dark.gif' %}"/>
         {% else %}
             <img src="{% static 'memberaudit/images/Spinner-1s-64px-light.gif' %}"/>
         {% endif %}
     </div>
     <br>
-    {% include 'memberaudit/partials/character_viewer/tabs/last_updated.html' with update_section=last_updates.attributes %}
+    {% include 'memberaudit/partials/character_viewer/tabs/last_updated.html' with update_section=last_updates.corporation_history %}
 </div>
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                     <dt>{% translate "Faction" %}</dt>
                     <dd>
                         {% if fw_stats.faction %}
                             <a href="{{ fw_stats.faction.profile_url }}" target="_blank">
                                 {{ fw_stats.faction }}
                             </a>
                         {% else %}
-                            Not enlisted
+                            {% translate "Not enlisted" %}
                         {% endif %}
                     </dd>
                     <dt>{% translate "Enlisted on" %}</dt>
                     <dd>{{ fw_stats.enlisted_on|default:"-" }}</dd>
                     <dt>{% translate "Current rank" %}</dt>
                     <dd>{{ fw_stats.current_rank_name|default:"-" }}</dd>
                     <dt>{% translate "Highest rank" %}</dt>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
 {% load humanize %} {% load i18n %}
 {% if faction_logo_url %}
 [{{_faction_logo_url_}}]
 {% endif %}
 *** {% translate "Status" %} ***
   {% translate "Faction" %}
-      {% if fw_stats.faction %} {{_fw_stats.faction_}} {% else %} Not enlisted
-      {% endif %}
+      {% if fw_stats.faction %} {{_fw_stats.faction_}} {% else %} {% translate
+      "Not enlisted" %} {% endif %}
   {% translate "Enlisted on" %}
       {{ fw_stats.enlisted_on|default:"-" }}
   {% translate "Current rank" %}
       {{ fw_stats.current_rank_name|default:"-" }}
   {% translate "Highest rank" %}
       {{ fw_stats.highest_rank_name|default:"-" }}
 *** {% translate "Kills" %} ***
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 {% load humanize %}
 
 <div role="tabpanel" class="tab-pane" id="skill_sets">
     <div class="table-responsive">
         <table class="table table-striped table-width-fix" id="tab_skill_sets">
             <thead>
                 <tr>
-                    <th>Skill Set Group</th>
+                    <th>{% translate 'Skill Set Group' %}</th>
                     <th>{% translate 'Skill Set' %}</th>
                     <th>{% translate 'Has all required?' %}</th>
                     <th>{% translate 'Missing Required Skills' %}</th>
                     <th>{% translate 'Missing Recommended Skills' %}</th>
                     <th></th>
                 </tr>
             </thead>
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 {% load i18n %} {% load humanize %}
-                               {% translate  {% translate      {% translate
-Skill Set Group {% translate   'Has all      'Missing Required 'Missing
-                'Skill Set' %} required?' %} Skills' %}        Recommended
-                                                               Skills' %}
+{% translate                                  {% translate      {% translate
+'Skill Set   {% translate   {% translate 'Has 'Missing Required 'Missing
+Group' %}    'Skill Set' %} all required?' %} Skills' %}        Recommended
+                                                                Skills' %}
 {% include 'memberaudit/partials/character_viewer/tabs/last_updated.html' with
 update_section=last_updates.skill_sets %}
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% load i18n %}
 
 <div role="tabpanel" class="tab-pane" id="wallet_journal">
-    <h4>Transactions</h4>
+    <h4>{% translate 'Transactions' %}</h4>
     <div class="table-responsive">
         <table class="table table-striped table-width-fix" id="tab_wallet_journal">
             <thead>
                 <tr>
                     <th>{% translate 'Date' %}</th>
                     <th>{% translate 'Type' %}</th>
                     <th>{% translate 'First party' %}</th>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
 {% load i18n %}
-*** Transactions ***
+*** {% translate 'Transactions' %} ***
 {%        {%        {%        {%                                  {% translate
 translate translate translate translate {% translate {% translate 'Description'
 'Date' %} 'Type' %} 'First    'Second   'Amount' %}  'Balance' %} %}
                     party' %} party' %}
 {% include 'memberaudit/partials/character_viewer/tabs/last_updated.html' with
 update_section=last_updates.wallet_journal %}
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% load i18n %}
 
 <div role="tabpanel" class="tab-pane" id="wallet_transactions">
-    <h4>Market Transactions</h4>
+    <h4>{% translate 'Market Transactions' %}</h4>
     <div class="table-responsive">
         <table class="table table-striped table-width-fix" id="tab_wallet_transactions">
             <thead>
                 <tr>
                     <th>{% translate 'Date' %}</th>
                     <th>{% translate 'Quantity' %}</th>
                     <th>{% translate 'Type' %}</th>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
 {% load i18n %}
-*** Market Transactions ***
+*** {% translate 'Market Transactions' %} ***
 {%        {%         {%        {%
 translate translate  translate translate {% translate {% translate {% translate
 'Date' %} 'Quantity' 'Type' %} 'Unit     'Total' %}   'Client' %}  'Where' %}
           %}                   Price' %}
 {% include 'memberaudit/partials/character_viewer/tabs/last_updated.html' with
 update_section=last_updates.wallet_transactions %}
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/menu.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/menu.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <!-- Skill Sets -->
 <div role="tabpanel" class="tab-pane" id="skill_sets">
     <div class="table-responsive">
         <table class="table table-striped table-width-fix" id="tab_skill_sets">
             <thead>
                 <tr>
-                    <th>Skill Set Group</th>
+                    <th>{% translate 'Skill Set Group' %}</th>
                     <th>{% translate 'Main' %}</th>
                     <th>{% translate 'State' %}</th>
                     <th>{% translate 'Organization' %}</th>
                     <th>{% translate 'Character' %}</th>
                     <th>{% translate 'Required Skills?' %}</th>
                     <th>{% translate 'Is Main?' %}</th>
                 </tr>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
 {% load i18n %}
-                                              {%          {%        {%
-Skill Set {%        {%         {% translate   translate   translate translate
-Group     translate translate  'Organization' 'Character' 'Required 'Is Main?'
-          'Main' %} 'State' %} %}             %}          Skills?'  %}
-                                                          %}
+{%                                             {%          {%        {%
+translate  {%        {%         {% translate   translate   translate translate
+'Skill Set translate translate  'Organization' 'Character' 'Required 'Is Main?'
+Group' %}  'Main' %} 'State' %} %}             %}          Skills?'  %}
+                                                           %}
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html`

 * *Files 17% similar despite different names*

```diff
@@ -13,9 +13,9 @@
                     <th>{% translate 'Total Chars' %}</th>
                 </tr>
             </thead>
 
             <tbody></tbody>
         </table>
     </div>
-    <p class="text-muted">Color code: <span class="text-success">fully compliant</span> | <span class="text-warning">partly compliant</span> | <span class="text-danger">not compliant</span></p>
+    {% include 'memberaudit/partials/reports/tabs/_compliance_color_code.html' %}
 </div>
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
 {% load i18n %}
 {%        {% translate {% translate   {% translate  {% translate {% translate
 translate 'State' %}   'Organization' 'Registered?' 'Compliant?' 'Total
 'User' %}              %}             %}            %}           Chars' %}
-Color code: fully compliant | partly compliant | not compliant
+{% include 'memberaudit/partials/reports/tabs/_compliance_color_code.html' %}
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/templates/memberaudit/reports.html` & `aa_memberaudit-2.6.3/memberaudit/templates/memberaudit/reports.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/core/test_core_xml_converter.py` & `aa_memberaudit-2.6.3/memberaudit/tests/core/test_core_xml_converter.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/core/test_data_exporters.py` & `aa_memberaudit-2.6.3/memberaudit/tests/core/test_data_exporters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/core/test_eft_parser.py` & `aa_memberaudit-2.6.3/memberaudit/tests/core/test_eft_parser.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/core/test_fittings.py` & `aa_memberaudit-2.6.3/memberaudit/tests/core/test_fittings.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/core/test_skill_plans.py` & `aa_memberaudit-2.6.3/memberaudit/tests/core/test_skill_plans.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/core/test_skills.py` & `aa_memberaudit-2.6.3/memberaudit/tests/core/test_skills.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/managers/test_character.py` & `aa_memberaudit-2.6.3/memberaudit/tests/managers/test_character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/managers/test_general.py` & `aa_memberaudit-2.6.3/memberaudit/tests/managers/test_general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/managers/test_sections.py` & `aa_memberaudit-2.6.3/memberaudit/tests/managers/test_sections.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/models/test_character_1.py` & `aa_memberaudit-2.6.3/memberaudit/tests/models/test_character_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/models/test_character_2.py` & `aa_memberaudit-2.6.3/memberaudit/tests/models/test_character_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/models/test_character_3.py` & `aa_memberaudit-2.6.3/memberaudit/tests/models/test_character_3.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/models/test_character_4.py` & `aa_memberaudit-2.6.3/memberaudit/tests/models/test_character_4.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/models/test_general.py` & `aa_memberaudit-2.6.3/memberaudit/tests/models/test_general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/models/test_sections.py` & `aa_memberaudit-2.6.3/memberaudit/tests/models/test_sections.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/models/utils.py` & `aa_memberaudit-2.6.3/memberaudit/tests/models/utils.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/test_admin.py` & `aa_memberaudit-2.6.3/memberaudit/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/test_auth_hooks.py` & `aa_memberaudit-2.6.3/memberaudit/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/test_checks.py` & `aa_memberaudit-2.6.3/memberaudit/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/test_commands.py` & `aa_memberaudit-2.6.3/memberaudit/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/test_decorators.py` & `aa_memberaudit-2.6.3/memberaudit/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/test_factories.py` & `aa_memberaudit-2.6.3/memberaudit/tests/test_factories.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/test_forms.py` & `aa_memberaudit-2.6.3/memberaudit/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/test_helpers.py` & `aa_memberaudit-2.6.3/memberaudit/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/test_integration.py` & `aa_memberaudit-2.6.3/memberaudit/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/test_signals.py` & `aa_memberaudit-2.6.3/memberaudit/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/test_tasks.py` & `aa_memberaudit-2.6.3/memberaudit/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/test_templatetags.py` & `aa_memberaudit-2.6.3/memberaudit/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/testdata/create_eveuniverse.py` & `aa_memberaudit-2.6.3/memberaudit/tests/testdata/create_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/testdata/entities.json` & `aa_memberaudit-2.6.3/memberaudit/tests/testdata/entities.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/testdata/esi_client_stub.py` & `aa_memberaudit-2.6.3/memberaudit/tests/testdata/esi_client_stub.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/testdata/esi_testdata.json` & `aa_memberaudit-2.6.3/memberaudit/tests/testdata/esi_testdata.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/testdata/eveuniverse.json` & `aa_memberaudit-2.6.3/memberaudit/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/testdata/factories.py` & `aa_memberaudit-2.6.3/memberaudit/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/testdata/fittings/fitting_archon.txt` & `aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_archon.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/testdata/fittings/fitting_archon_max.txt` & `aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_archon_max.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/testdata/fittings/fitting_svipul.txt` & `aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_svipul.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/testdata/fittings/fitting_tengu.txt` & `aa_memberaudit-2.6.3/memberaudit/tests/testdata/fittings/fitting_tengu.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/testdata/generate_character.py` & `aa_memberaudit-2.6.3/memberaudit/tests/testdata/generate_character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/testdata/generate_doctrines.py` & `aa_memberaudit-2.6.3/memberaudit/tests/testdata/generate_doctrines.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/testdata/load_entities.py` & `aa_memberaudit-2.6.3/memberaudit/tests/testdata/load_entities.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/testdata/load_locations.py` & `aa_memberaudit-2.6.3/memberaudit/tests/testdata/load_locations.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/testdata/pilot_esi_error_handling.py` & `aa_memberaudit-2.6.3/memberaudit/tests/testdata/pilot_esi_error_handling.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/testdata/profiler_toolbox.py` & `aa_memberaudit-2.6.3/memberaudit/tests/testdata/profiler_toolbox.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/utils.py` & `aa_memberaudit-2.6.3/memberaudit/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/views/test_admin.py` & `aa_memberaudit-2.6.3/memberaudit/tests/views/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/views/test_character_finder.py` & `aa_memberaudit-2.6.3/memberaudit/tests/views/test_character_finder.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/views/test_character_viewer_1.py` & `aa_memberaudit-2.6.3/memberaudit/tests/views/test_character_viewer_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/views/test_character_viewer_2.py` & `aa_memberaudit-2.6.3/memberaudit/tests/views/test_character_viewer_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/views/test_characters.py` & `aa_memberaudit-2.6.3/memberaudit/tests/views/test_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/views/test_data_export.py` & `aa_memberaudit-2.6.3/memberaudit/tests/views/test_data_export.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tests/views/test_reports.py` & `aa_memberaudit-2.6.3/memberaudit/tests/views/test_reports.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/tools/drop_tables.sql` & `aa_memberaudit-2.6.3/memberaudit/tools/drop_tables.sql`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/urls.py` & `aa_memberaudit-2.6.3/memberaudit/urls.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/views/_common.py` & `aa_memberaudit-2.6.3/memberaudit/views/_common.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.6.2/memberaudit/views/admin.py` & `aa_memberaudit-2.6.3/memberaudit/views/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django.contrib import messages
 from django.contrib.admin.views.decorators import staff_member_required
 from django.contrib.auth.decorators import login_required
 from django.shortcuts import redirect, render
 from django.utils.html import format_html
+from django.utils.translation import gettext_lazy as _
 
 from allianceauth import NAME as site_header
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
 
 from .. import __title__, tasks
 from ..forms import ImportFittingForm, ImportSkillPlanForm
@@ -29,48 +30,45 @@
             )
             if (
                 not form.cleaned_data["can_overwrite"]
                 and SkillSet.objects.filter(name=skill_set_name).exists()
             ):
                 messages.warning(
                     request,
-                    format_html(
-                        "A skill set with the name "
-                        f"<b>{fitting.name}</b> already exists."
-                    ),
+                    _("A skill set with the name %s already exists." % fitting.name),
                 )
             else:
                 params = {"fitting": fitting, "user": request.user}
                 if form.cleaned_data["skill_set_group"]:
                     params["skill_set_group"] = form.cleaned_data["skill_set_group"]
                 if form.cleaned_data["skill_set_name"]:
                     params["skill_set_name"] = form.cleaned_data["skill_set_name"]
                 obj, created = SkillSet.objects.update_or_create_from_fitting(**params)
                 logger.info(
                     "Skill Set created from fitting with name: %s", fitting.name
                 )
                 tasks.update_characters_skill_checks.delay(force_update=True)
                 if created:
-                    msg = f"Skill Set <b>{obj.name}</b> has been created"
+                    msg = _("Skill Set <b>%s</b> has been created") % obj.name
                 else:
-                    msg = f"Skill Set <b>{obj.name}</b> has been updated"
+                    msg = _("Skill Set <b>%s</b> has been updated") % obj.name
                 if form.cleaned_data["_errors"]:
                     errors = form.cleaned_data["_errors"]
                     msg += f" with issues:<br>- {'<br>- '.join(errors)}"
                     messages.warning(request, format_html(msg))
                 else:
                     messages.info(request, format_html(f"{msg}."))
             return redirect("admin:memberaudit_skillset_changelist")
     else:
         form = ImportFittingForm()
     return render(
         request,
         "admin/memberaudit/skillset/import_skills.html",
         {
-            "title": "Create skill set from fitting",
+            "title": _("Create skill set from fitting"),
             "form": form,
             "cl": {"opts": SkillSet._meta},
             "site_header": site_header,
         },
     )
 
 
@@ -84,29 +82,29 @@
             params = {"skill_plan": skill_plan, "user": request.user}
             if form.cleaned_data["skill_set_group"]:
                 params["skill_set_group"] = form.cleaned_data["skill_set_group"]
             obj, created = SkillSet.objects.update_or_create_from_skill_plan(**params)
             logger.info("%s: Skill Set created from skill plan", skill_plan.name)
             tasks.update_characters_skill_checks.delay(force_update=True)
             if created:
-                msg = f"Skill Set <b>{obj.name}</b> has been created"
+                msg = _("Skill Set <b>%s</b> has been created") % obj.name
             else:
-                msg = f"Skill Set <b>{obj.name}</b> has been updated"
+                msg = _("Skill Set <b>%s</b> has been updated") % obj.name
             if form.cleaned_data["_errors"]:
                 errors = form.cleaned_data["_errors"]
-                msg += f" with issues:<br>- {'<br>- '.join(errors)}"
+                msg += f" {_('with issues')}:<br>- {'<br>- '.join(errors)}"
                 messages.warning(request, format_html(msg))
             else:
                 messages.info(request, format_html(f"{msg}."))
             return redirect("admin:memberaudit_skillset_changelist")
     else:
         form = ImportSkillPlanForm()
     return render(
         request,
         "admin/memberaudit/skillset/import_skills.html",
         {
-            "title": "Create skill set from skill plan",
+            "title": _("Create skill set from skill plan"),
             "form": form,
             "cl": {"opts": SkillSet._meta},
             "site_header": site_header,
         },
     )
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/views/character_finder.py` & `aa_memberaudit-2.6.3/memberaudit/views/character_finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from django.core.exceptions import ObjectDoesNotExist
 from django.db.models import Case, F, Q, Value, When
 from django.http import HttpResponse, JsonResponse
 from django.shortcuts import render
 from django.urls import reverse
 from django.utils.html import format_html, format_html_join
 from django.utils.safestring import mark_safe
+from django.utils.translation import gettext_lazy as _
 
 from allianceauth.eveonline.models import EveCharacter
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
 from app_utils.views import (
     bootstrap_icon_plus_name_html,
     fontawesome_link_button_html,
@@ -26,15 +27,15 @@
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 @login_required
 @permission_required("memberaudit.finder_access")
 def character_finder(request) -> HttpResponse:
     context = {
-        "page_title": "Character Finder",
+        "page_title": _("Character Finder"),
     }
     return render(
         request,
         "memberaudit/character_finder.html",
         add_common_context(request, context),
     )
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/views/character_viewer_1.py` & `aa_memberaudit-2.6.3/memberaudit/views/character_viewer_1.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from django.db.models import Count, F, Max, Q, Sum
 from django.http import HttpResponse, HttpResponseNotFound, JsonResponse
 from django.shortcuts import render
 from django.urls import reverse
 from django.utils.html import format_html
 from django.utils.timesince import timeuntil
 from django.utils.timezone import now
+from django.utils.translation import gettext_lazy as _
 from eveuniverse.models import EveType
 
 from allianceauth.eveonline.models import EveCharacter
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.helpers import humanize_number
 from app_utils.logging import LoggerAddTag
 from app_utils.views import (
@@ -173,19 +174,20 @@
             for obj in character.update_status_set.filter(is_success=True).values(
                 "section", "finished_at"
             )
         }
     except ObjectDoesNotExist:
         last_updates = None
 
-    page_title = "Character Sheet"
+    page_title = _("Character Sheet")
     if not character.user_is_owner(request.user):
         page_title = format_html(
-            '{}&nbsp;<i class="far fa-eye" title="You do not own this character"></i>',
+            '{}&nbsp;<i class="far fa-eye" title="{}"></i>',
             page_title,
+            _("You do not own this character"),
         )
 
     context = {
         "page_title": page_title,
         "character": character,
         "auth_character": character.eve_character,
         "character_details": character_details,
@@ -206,15 +208,15 @@
         request,
         "memberaudit/character_viewer.html",
         add_common_context(request, context),
     )
 
 
 def _identify_user_characters(request, character):
-    """Identify all characters owned by this user for siderbar."""
+    """Identify all characters owned by this user for sidebar."""
     if not character.user:
         eve_characters_of_user = EveCharacter.objects.none()
     else:
         eve_characters_of_user = EveCharacter.objects.select_related(
             "character_ownership__memberaudit_character"
         ).filter(character_ownership__user=character.user)
     all_characters = (
@@ -327,16 +329,16 @@
                 "actions": actions_html,
                 "region": region,
                 "solar_system": solar_system,
                 "is_ship": is_ship,
             }
         )
     for row in data:
-        sumstr = humanize_number(location_totals[row["location"]])
-        row["location"] = row["location"] + f" ({sumstr} ISK)"
+        sum_str = humanize_number(location_totals[row["location"]])
+        row["location"] = row["location"] + f" ({sum_str} ISK)"
     return JsonResponse({"data": data})
 
 
 @login_required
 @permission_required("memberaudit.basic_access")
 @fetch_character_if_allowed()
 def character_asset_container(
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/views/character_viewer_2.py` & `aa_memberaudit-2.6.3/memberaudit/views/character_viewer_2.py`

 * *Files identical despite different names*

```diff
@@ -192,15 +192,17 @@
     try:
         mail = (
             character.mails.select_related("sender")
             .prefetch_related("recipients")
             .get(pk=mail_pk)
         )
     except CharacterMail.DoesNotExist:
-        error_msg = f"Mail with pk {mail_pk} not found for character {character}"
+        error_msg = gettext_lazy(
+            "Mail with pk %s not found for character %s" % (mail_pk, character)
+        )
         logger.warning(error_msg)
         return HttpResponseNotFound(error_msg)
     recipients = sorted(
         [
             {
                 "name": obj.name_plus,
                 "link": link_html(obj.external_url(), obj.name_plus),
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/views/characters.py` & `aa_memberaudit-2.6.3/memberaudit/views/characters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from django.contrib import messages
 from django.contrib.auth.decorators import login_required, permission_required
 from django.contrib.auth.models import Permission
 from django.db import transaction
 from django.http import HttpResponse, HttpResponseForbidden, HttpResponseNotFound
 from django.shortcuts import get_object_or_404, redirect, render
 from django.utils.html import format_html
+from django.utils.translation import gettext_lazy as _
 from esi.decorators import token_required
 
 from allianceauth.eveonline.models import EveCharacter
 from allianceauth.notifications import notify
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.django import users_with_permission
 from app_utils.logging import LoggerAddTag
@@ -68,15 +69,15 @@
 
     try:
         main_character_id = request.user.profile.main_character.character_id
     except AttributeError:
         main_character_id = None
 
     context = {
-        "page_title": "My Characters",
+        "page_title": _("My Characters"),
         "auth_characters": auth_characters,
         "has_auth_characters": has_auth_characters,
         "unregistered_chars": unregistered_chars,
         "has_registered_characters": len(auth_characters) > 0,
         "main_character_id": main_character_id,
     }
 
@@ -98,27 +99,30 @@
 
 @login_required
 @permission_required("memberaudit.basic_access")
 @token_required(scopes=Character.get_esi_scopes())
 def add_character(request, token) -> HttpResponse:
     eve_character = get_object_or_404(EveCharacter, character_id=token.character_id)
     with transaction.atomic():
-        character, _ = Character.objects.update_or_create(
+        character, created = Character.objects.update_or_create(
             eve_character=eve_character, defaults={"is_disabled": False}
         )
     tasks.update_character.apply_async(
         kwargs={"character_pk": character.pk},
         priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY,
     )
     messages.success(
         request,
         format_html(
-            "<strong>{}</strong> has been registered. "
-            "Note that it can take a minute until all character data is visible.",
+            "<strong>{}</strong> {}",
             eve_character,
+            _(
+                "has been registered. "
+                "Note that it can take a minute until all character data is visible."
+            ),
         ),
     )
     if ComplianceGroupDesignation.objects.exists():
         tasks.update_compliance_groups_for_user.apply_async(
             args=[request.user.pk], priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY
         )
     return redirect("memberaudit:launcher")
@@ -137,26 +141,23 @@
         character_name = character.eve_character.character_name
 
         # Notify that character has been dropped
         permission_to_notify = Permission.objects.select_related("content_type").get(
             content_type__app_label=Character._meta.app_label,
             codename="notified_on_character_removal",
         )
-        title = f"{__title__}: Character has been removed!"
-        message = f"{request.user} has removed character '{character_name}'"
+        title = _("%s: Character has been removed!" % __title__)
+        message = _("%s has removed character '%s'" % (request.user, character_name))
         for to_notify in users_with_permission(permission_to_notify):
             if character.user_has_scope(to_notify):
                 notify(user=to_notify, title=title, message=message, level="INFO")
 
         character.delete()
         messages.success(
-            request,
-            format_html(
-                "Removed character <strong>{}</strong> as requested.", character_name
-            ),
+            request, _("Removed character %s as requested.") % character_name
         )
         if ComplianceGroupDesignation.objects.exists():
             tasks.update_compliance_groups_for_user.apply_async(
                 args=[request.user.pk], priority=MEMBERAUDIT_TASKS_NORMAL_PRIORITY
             )
     else:
         return HttpResponseForbidden(
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/views/data_export.py` & `aa_memberaudit-2.6.3/memberaudit/views/data_export.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django.contrib import messages
 from django.contrib.auth.decorators import login_required, permission_required
 from django.http import FileResponse, Http404
 from django.shortcuts import redirect, render
 from django.utils.html import format_html
+from django.utils.translation import gettext_lazy as _
 
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
 
 from .. import __title__, tasks
 from ..app_settings import MEMBERAUDIT_DATA_EXPORT_MIN_UPDATE_AGE
 from ..core import data_exporters
@@ -17,15 +18,15 @@
 
 
 @login_required
 @permission_required("memberaudit.exports_access")
 def data_export(request):
     topics = data_exporters.topics_and_export_files()
     context = {
-        "page_title": "Data Export",
+        "page_title": _("Data Export"),
         "topics": topics,
         "character_count": Character.objects.count(),
         "minutes_until_next_update": MEMBERAUDIT_DATA_EXPORT_MIN_UPDATE_AGE,
     }
     return render(
         request, "memberaudit/data_export.html", add_common_context(request, context)
     )
@@ -46,15 +47,15 @@
 @login_required
 @permission_required("memberaudit.exports_access")
 def data_export_run_update(request, topic: str):
     tasks.export_data_for_topic.delay(topic=topic, user_pk=request.user.pk)
     format_html
     messages.info(
         request,
-        format_html(
-            "Data export for topic <strong>{}</strong> has been started. "
+        _(
+            "Data export for topic <strong>%s</strong> has been started. "
             "This can take a couple of minutes. "
             "You will get a notification once it is completed.",
-            topic,
-        ),
+        )
+        % topic,
     )
     return redirect("memberaudit:data_export")
```

### Comparing `aa_memberaudit-2.6.2/memberaudit/views/reports.py` & `aa_memberaudit-2.6.3/memberaudit/views/reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from django.contrib.auth.decorators import login_required, permission_required
 from django.core.exceptions import ObjectDoesNotExist
 from django.db.models import Count, Exists, OuterRef, Q
 from django.http import HttpResponse, JsonResponse
 from django.shortcuts import render
 from django.urls import reverse
 from django.utils.html import format_html
+from django.utils.translation import gettext_lazy as _
 from eveuniverse.core import eveimageserver
 from eveuniverse.models import EveType
 
 from allianceauth.authentication.models import get_guest_state_pk
 from allianceauth.eveonline.models import EveCharacter
 from allianceauth.services.hooks import get_extension_logger
 from app_utils.logging import LoggerAddTag
@@ -31,21 +32,17 @@
         f" [{main_character.alliance_ticker}]" if main_character.alliance_name else "",
     )
 
 
 @login_required
 @permission_required("memberaudit.reports_access")
 def reports(request) -> HttpResponse:
-    context = {
-        "page_title": "Reports",
-    }
+    context = {"page_title": _("Reports")}
     return render(
-        request,
-        "memberaudit/reports.html",
-        add_common_context(request, context),
+        request, "memberaudit/reports.html", add_common_context(request, context)
     )
 
 
 @login_required
 @permission_required("memberaudit.reports_access")
 def user_compliance_report_data(request) -> JsonResponse:
     users_and_character_counts = (
```

### Comparing `aa_memberaudit-2.6.2/setup.cfg` & `aa_memberaudit-2.6.3/setup.cfg`

 * *Files identical despite different names*

