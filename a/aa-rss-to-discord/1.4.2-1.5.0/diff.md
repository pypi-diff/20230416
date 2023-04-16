# Comparing `tmp/aa_rss_to_discord-1.4.2.tar.gz` & `tmp/aa_rss_to_discord-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_rss_to_discord-1.4.2.tar", last modified: Thu Apr 13 20:35:22 2023, max compression
+gzip compressed data, was "aa_rss_to_discord-1.5.0.tar", last modified: Sun Apr 16 17:42:07 2023, max compression
```

## Comparing `aa_rss_to_discord-1.4.2.tar` & `aa_rss_to_discord-1.5.0.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/auth_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/discordbot/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/discordbot/cogs/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/discordbot/cogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/discordbot/cogs/rss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/it_IT/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/it_IT/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ko_KR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ko_KR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ko_KR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.053346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/migrations/0002_enable_disable_rss_feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/aa_rss_to_discord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-04-13 20:35:22.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-13 20:35:22.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:35:22.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 20:35:21.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-13 20:35:22.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-13 20:35:22.000000 aa_rss_to_discord-1.4.2/aa_rss_to_discord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-13 20:35:04.000000 aa_rss_to_discord-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-13 20:35:22.057346 aa_rss_to_discord-1.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/auth_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.787154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/discordbot/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/discordbot/cogs/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/discordbot/cogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/discordbot/cogs/rss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.795154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.791154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.791154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.791154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.791154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/it_IT/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/it_IT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/it_IT/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.791154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.791154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ko_KR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ko_KR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ko_KR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.791154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.795154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/migrations/0002_enable_disable_rss_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:07.799154 aa_rss_to_discord-1.5.0/aa_rss_to_discord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-04-16 17:42:07.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-16 17:42:07.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 17:42:07.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 17:42:07.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-16 17:42:07.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 17:42:07.000000 aa_rss_to_discord-1.5.0/aa_rss_to_discord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 17:41:49.000000 aa_rss_to_discord-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-16 17:42:07.803154 aa_rss_to_discord-1.5.0/setup.cfg
```

### Comparing `aa_rss_to_discord-1.4.2/CHANGELOG.md` & `aa_rss_to_discord-1.5.0/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -5,14 +5,21 @@
 The format is based on [Keep a Changelog](http://keepachangelog.com/)
 and this project adheres to [Semantic Versioning](http://semver.org/)
 
 
 ## [In Development] - Unreleased
 
 
+## [1.5.0] - 2023-04-16
+
+### Added
+
+- Russian translation
+
+
 ## [1.4.2] - 2023-04-13
 
 ### Added
 
 - German translation
 
 
@@ -105,21 +112,21 @@
 ## [1.1.0] - 2021-09-03
 
 ### Added
 
 - Commands for the Discord bot to manage RSS/Atom feeds. The following commands have
   been added:
 
-  | Command | Options | What it does |
-  |:---|:---|:---|
-  | `!rss_add <rss_url> <rss_name>` | - `rss_url` - The URL of the RSS/Atom feed<br>- `rss_name` - A Name for the RSS/Atom Feed | Adding a RSS/Atom fedd to the current channel |
-  | `!rss_delete <rss_feed_id>` | `rss_feed_id` - The ID of the RSS/Atom feed you want to remove |  Remove a RSS/Atom feed from the current Discord channel |
-  | `!rss_disable <rss_feed_id>` | `rss_feed_id` - The ID of the RSS/Atom feed you want to disable |  Disable an enabled RSS/Atom feed for the current Discord channel |
-  | `!rss_enable <rss_feed_id>` | `rss_feed_id` - The ID of the RSS/Atom feed you want to enable |  Enable a disabled RSS/Atom feed for the current Discord channel |
-  | `!rss_list` | None |  List all RSS/Atom feeds for the current Discord channel |
+  | Command                           | Options                                                                                                                      | What it does                                                     |
+  |:----------------------------------|:-----------------------------------------------------------------------------------------------------------------------------|:-----------------------------------------------------------------|
+  | `!rss_add <rss_url> <rss_name>`   | - `rss_url` - The URL of the RSS/Atom <br/><br/><br/><br/><br/><br/><br/>feed<br>- `rss_name` - A Name for the RSS/Atom Feed | Adding a RSS/Atom feed to the current channel                    |
+  | `!rss_delete <rss_feed_id>`       | `rss_feed_id` - The ID of the RSS/Atom feed you want to remove                                                               | Remove a RSS/Atom feed from the current Discord channel          |
+  | `!rss_disable <rss_feed_id>`      | `rss_feed_id` - The ID of the RSS/Atom feed you want to disable                                                              | Disable an enabled RSS/Atom feed for the current Discord channel |
+  | `!rss_enable <rss_feed_id>`       | `rss_feed_id` - The ID of the RSS/Atom feed you want to enable                                                               | Enable a disabled RSS/Atom feed for the current Discord channel  |
+  | `!rss_list`                       | None                                                                                                                         | List all RSS/Atom feeds for the <br/>current Discord channel     |
 
 
 ## [1.0.0] - 2021-09-03
 
 ### Changed
 
 - Moved from Beta to Stable
@@ -143,15 +150,15 @@
 
 ### Added
 
 - Switch to enable/disable RSS feeds in admin interface
 
 ### Changed
 
-- Cleaned up filter in admin interface
+- Cleaned up the filter in admin interface
 
 
 ## [0.1.0-beta.4] - 2021-05-05
 
 ### Fixed
 
 - Using Django application registry instead of directly accessing `INSTALLED_APPS`
```

### Comparing `aa_rss_to_discord-1.4.2/LICENSE` & `aa_rss_to_discord-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.4.2/PKG-INFO` & `aa_rss_to_discord-1.5.0/aa_rss_to_discord.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aa_rss_to_discord
-Version: 1.4.2
+Name: aa-rss-to-discord
+Version: 1.5.0
 Summary: Alliance Auth module to post news from RSS feeds to your Discord
 Home-page: https://github.com/ppfeufer/aa-rss-to-discord
 Author: Peter Pfeufer
 Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
@@ -42,57 +42,60 @@
 [![codecov](https://codecov.io/gh/ppfeufer/aa-rss-to-discord/branch/master/graph/badge.svg?token=LVEQ6W55ZB)](https://codecov.io/gh/ppfeufer/aa-rss-to-discord)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/ppfeufer/aa-rss-to-discord/blob/master/CODE_OF_CONDUCT.md)
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/N4N8CL1BY)
 
 A simple app to post selected RSS feeds to your Discord.
 
+---
 
-## Contents
-
-- [Installation](#installation)
-  - [Step 0.5 - Install AA-Discordbot](#step-05---install-aa-discordbot)
-  - [Step 1 - Install the Package](#step-1---install-the-package)
-  - [Step 2 - Configure Alliance Auth](#step-2---configure-alliance-auth)
-  - [Step 3 - Finalize the Installation](#step-3---finalize-the-installation)
-  - [Step 4 - Configure your RSS Feeds](#step-4---configure-your-rss-feeds)
-- [Discord Bot Commands](#discord-bot-commands)
-- [Updating](#updating)
+<!-- TOC -->
+* [Alliance Auth RSS to Discord](#alliance-auth-rss-to-discord)
+  * [Installation](#installation)
+    * [Step 0.5: Install AA-Discordbot](#step-05-install-aa-discordbot)
+    * [Step 1: Install the Package](#step-1-install-the-package)
+    * [Step 2: Configure Alliance Auth](#step-2-configure-alliance-auth)
+    * [Step 3: Finalizing the Installation](#step-3-finalizing-the-installation)
+    * [Step 4: Configure your RSS Feeds](#step-4-configure-your-rss-feeds)
+  * [Discord Bot Commands](#discord-bot-commands)
+  * [Updating](#updating)
+<!-- TOC -->
 
+---
 
 ## Installation
 
 **Important**: Please make sure you meet all preconditions before you proceed:
 
 - Alliance Auth RSS to Discord is a plugin for Alliance Auth. If you don't have Alliance Auth running
   already, please install it first before proceeding. (see the official
   [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html) for details)
 - Alliance Auth RSS to Discord needs [AA-Discordbot](https://github.com/pvyParts/allianceauth-discordbot)
   to interact with your Discord server. Make sure it is installed and configured
   **before** installing this app.
 
 
-### Step 0.5 - Install AA-Discordbot
+### Step 0.5: Install AA-Discordbot
 
 In order for this app to work, you need to install and configure
 [AA-Discordbot](https://github.com/pvyParts/allianceauth-discordbot) first. Read the
 instructions how to do so in the README of AA-Discordbot.
 
 
-### Step 1 - Install the Package
+### Step 1: Install the Package
 
-Make sure you are in the virtual environment (venv) of your Alliance Auth
-installation Then install the latest releast directly from PyPi.
+Make sure you're in the virtual environment (venv) of your Alliance Auth
+installation Then install the latest release directly from PyPi.
 
 ```shell
 pip install aa-rss-to-discord
 ```
 
 
-### Step 2 - Configure Alliance Auth
+### Step 2: Configure Alliance Auth
 
 This is fairly simple, just add the following to the `INSTALLED_APPS` of your `local.py`
 
 Configure your AA settings (`local.py`) as follows:
 
 - Add `"aa_rss_to_discord",` to `INSTALLED_APPS`
 - Add the scheduled task
@@ -100,52 +103,53 @@
   CELERYBEAT_SCHEDULE["aa_rss_to_discord_fetch_rss"] = {
       "task": "aa_rss_to_discord.tasks.fetch_rss",
       "schedule": crontab(minute="*/5"),
   }
   ```
 
 
-### Step 3 - Finalize the Installation
+### Step 3: Finalizing the Installation
 
 Run migrations to finalize the installation
 
 ```shell
 python manage.py migrate
 ```
 
-Finally restart your supervisor services for AA.
+Finally, restart your supervisor services for AA.
 
 
-### Step 4 - Configure your RSS Feeds
+### Step 4: Configure your RSS Feeds
 
-First you need to set up the Discord Server and Channels. For this you go in your
+First, you need to set up the Discord Server and Channels. For this, you go in your
 admin backend to the Discordbot settings and enter the needed information there.
 
 When done, you can set up your RSS feeds. This can be done in the setting of this
 app, still in your admin backend. Create a new RSS Feed entry, enter the name, url
 and select the Discord channel it should be posted to. Once done, save it.
 
 
 ## Discord Bot Commands
 
 The following commands are available for the Discord bot to manage RSS/Atom feeds:
 
-| Command | Options | What it does |
-|:---|:---|:---|
-| `!rss_add <rss_url> <rss_name>` | - `rss_url` - The URL of the RSS/Atom feed<br>- `rss_name` - A Name for the RSS/Atom Feed | Adding a RSS/Atom fedd to the current channel |
-| `!rss_delete <rss_feed_id>` | `rss_feed_id` - The ID of the RSS/Atom feed you want to remove |  Remove a RSS/Atom feed from the current Discord channel |
-| `!rss_disable <rss_feed_id>` | `rss_feed_id` - The ID of the RSS/Atom feed you want to disable |  Disable an enabled RSS/Atom feed for the current Discord channel |
-| `!rss_enable <rss_feed_id>` | `rss_feed_id` - The ID of the RSS/Atom feed you want to enable |  Enable a disabled RSS/Atom feed for the current Discord channel |
-| `!rss_list` | None |  List all RSS/Atom feeds for the current Discord channel |
+| Command                         | Options                                                                                   | What it does                                                     |
+|:--------------------------------|:------------------------------------------------------------------------------------------|:-----------------------------------------------------------------|
+| `!rss_add <rss_url> <rss_name>` | - `rss_url` - The URL of the RSS/Atom feed<br>- `rss_name` - A Name for the RSS/Atom Feed | Adding a RSS/Atom feed to the current channel                    |
+| `!rss_delete <rss_feed_id>`     | `rss_feed_id` - The ID of the RSS/Atom feed you want to remove                            | Remove a RSS/Atom feed from the current Discord channel          |
+| `!rss_disable <rss_feed_id>`    | `rss_feed_id` - The ID of the RSS/Atom feed you want to disable                           | Disable an enabled RSS/Atom feed for the current Discord channel |
+| `!rss_enable <rss_feed_id>`     | `rss_feed_id` - The ID of the RSS/Atom feed you want to enable                            | Enable a disabled RSS/Atom feed for the current Discord channel  |
+| `!rss_list`                     | None                                                                                      | List all RSS/Atom feeds for the current Discord channel          |
+
 
 ## Updating
 
 To update your existing installation of Alliance Auth RSS to Discord, first enable your
 virtual environment (venv) of your Alliance Auth installation.
 
 ```bash
 pip install -U aa-rss-to-discord
 
 python manage.py migrate
 ```
 
-Finally restart your supervisor services for AA.
+Finally, restart your supervisor services for AA.
```

### Comparing `aa_rss_to_discord-1.4.2/README.md` & `aa_rss_to_discord-1.5.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -11,57 +11,60 @@
 [![codecov](https://codecov.io/gh/ppfeufer/aa-rss-to-discord/branch/master/graph/badge.svg?token=LVEQ6W55ZB)](https://codecov.io/gh/ppfeufer/aa-rss-to-discord)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/ppfeufer/aa-rss-to-discord/blob/master/CODE_OF_CONDUCT.md)
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/N4N8CL1BY)
 
 A simple app to post selected RSS feeds to your Discord.
 
+---
 
-## Contents
-
-- [Installation](#installation)
-  - [Step 0.5 - Install AA-Discordbot](#step-05---install-aa-discordbot)
-  - [Step 1 - Install the Package](#step-1---install-the-package)
-  - [Step 2 - Configure Alliance Auth](#step-2---configure-alliance-auth)
-  - [Step 3 - Finalize the Installation](#step-3---finalize-the-installation)
-  - [Step 4 - Configure your RSS Feeds](#step-4---configure-your-rss-feeds)
-- [Discord Bot Commands](#discord-bot-commands)
-- [Updating](#updating)
+<!-- TOC -->
+* [Alliance Auth RSS to Discord](#alliance-auth-rss-to-discord)
+  * [Installation](#installation)
+    * [Step 0.5: Install AA-Discordbot](#step-05-install-aa-discordbot)
+    * [Step 1: Install the Package](#step-1-install-the-package)
+    * [Step 2: Configure Alliance Auth](#step-2-configure-alliance-auth)
+    * [Step 3: Finalizing the Installation](#step-3-finalizing-the-installation)
+    * [Step 4: Configure your RSS Feeds](#step-4-configure-your-rss-feeds)
+  * [Discord Bot Commands](#discord-bot-commands)
+  * [Updating](#updating)
+<!-- TOC -->
 
+---
 
 ## Installation
 
 **Important**: Please make sure you meet all preconditions before you proceed:
 
 - Alliance Auth RSS to Discord is a plugin for Alliance Auth. If you don't have Alliance Auth running
   already, please install it first before proceeding. (see the official
   [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html) for details)
 - Alliance Auth RSS to Discord needs [AA-Discordbot](https://github.com/pvyParts/allianceauth-discordbot)
   to interact with your Discord server. Make sure it is installed and configured
   **before** installing this app.
 
 
-### Step 0.5 - Install AA-Discordbot
+### Step 0.5: Install AA-Discordbot
 
 In order for this app to work, you need to install and configure
 [AA-Discordbot](https://github.com/pvyParts/allianceauth-discordbot) first. Read the
 instructions how to do so in the README of AA-Discordbot.
 
 
-### Step 1 - Install the Package
+### Step 1: Install the Package
 
-Make sure you are in the virtual environment (venv) of your Alliance Auth
-installation Then install the latest releast directly from PyPi.
+Make sure you're in the virtual environment (venv) of your Alliance Auth
+installation Then install the latest release directly from PyPi.
 
 ```shell
 pip install aa-rss-to-discord
 ```
 
 
-### Step 2 - Configure Alliance Auth
+### Step 2: Configure Alliance Auth
 
 This is fairly simple, just add the following to the `INSTALLED_APPS` of your `local.py`
 
 Configure your AA settings (`local.py`) as follows:
 
 - Add `"aa_rss_to_discord",` to `INSTALLED_APPS`
 - Add the scheduled task
@@ -69,52 +72,53 @@
   CELERYBEAT_SCHEDULE["aa_rss_to_discord_fetch_rss"] = {
       "task": "aa_rss_to_discord.tasks.fetch_rss",
       "schedule": crontab(minute="*/5"),
   }
   ```
 
 
-### Step 3 - Finalize the Installation
+### Step 3: Finalizing the Installation
 
 Run migrations to finalize the installation
 
 ```shell
 python manage.py migrate
 ```
 
-Finally restart your supervisor services for AA.
+Finally, restart your supervisor services for AA.
 
 
-### Step 4 - Configure your RSS Feeds
+### Step 4: Configure your RSS Feeds
 
-First you need to set up the Discord Server and Channels. For this you go in your
+First, you need to set up the Discord Server and Channels. For this, you go in your
 admin backend to the Discordbot settings and enter the needed information there.
 
 When done, you can set up your RSS feeds. This can be done in the setting of this
 app, still in your admin backend. Create a new RSS Feed entry, enter the name, url
 and select the Discord channel it should be posted to. Once done, save it.
 
 
 ## Discord Bot Commands
 
 The following commands are available for the Discord bot to manage RSS/Atom feeds:
 
-| Command | Options | What it does |
-|:---|:---|:---|
-| `!rss_add <rss_url> <rss_name>` | - `rss_url` - The URL of the RSS/Atom feed<br>- `rss_name` - A Name for the RSS/Atom Feed | Adding a RSS/Atom fedd to the current channel |
-| `!rss_delete <rss_feed_id>` | `rss_feed_id` - The ID of the RSS/Atom feed you want to remove |  Remove a RSS/Atom feed from the current Discord channel |
-| `!rss_disable <rss_feed_id>` | `rss_feed_id` - The ID of the RSS/Atom feed you want to disable |  Disable an enabled RSS/Atom feed for the current Discord channel |
-| `!rss_enable <rss_feed_id>` | `rss_feed_id` - The ID of the RSS/Atom feed you want to enable |  Enable a disabled RSS/Atom feed for the current Discord channel |
-| `!rss_list` | None |  List all RSS/Atom feeds for the current Discord channel |
+| Command                         | Options                                                                                   | What it does                                                     |
+|:--------------------------------|:------------------------------------------------------------------------------------------|:-----------------------------------------------------------------|
+| `!rss_add <rss_url> <rss_name>` | - `rss_url` - The URL of the RSS/Atom feed<br>- `rss_name` - A Name for the RSS/Atom Feed | Adding a RSS/Atom feed to the current channel                    |
+| `!rss_delete <rss_feed_id>`     | `rss_feed_id` - The ID of the RSS/Atom feed you want to remove                            | Remove a RSS/Atom feed from the current Discord channel          |
+| `!rss_disable <rss_feed_id>`    | `rss_feed_id` - The ID of the RSS/Atom feed you want to disable                           | Disable an enabled RSS/Atom feed for the current Discord channel |
+| `!rss_enable <rss_feed_id>`     | `rss_feed_id` - The ID of the RSS/Atom feed you want to enable                            | Enable a disabled RSS/Atom feed for the current Discord channel  |
+| `!rss_list`                     | None                                                                                      | List all RSS/Atom feeds for the current Discord channel          |
+
 
 ## Updating
 
 To update your existing installation of Alliance Auth RSS to Discord, first enable your
 virtual environment (venv) of your Alliance Auth installation.
 
 ```bash
 pip install -U aa-rss-to-discord
 
 python manage.py migrate
 ```
 
-Finally restart your supervisor services for AA.
+Finally, restart your supervisor services for AA.
```

### Comparing `aa_rss_to_discord-1.4.2/aa_rss_to_discord/discordbot/cogs/rss.py` & `aa_rss_to_discord-1.5.0/aa_rss_to_discord/discordbot/cogs/rss.py`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/de/LC_MESSAGES/django.mo` & `aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/de/LC_MESSAGES/django.po` & `aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/es/LC_MESSAGES/django.po` & `aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/fr_FR/LC_MESSAGES/django.po` & `aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/it_IT/LC_MESSAGES/django.po` & `aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ja/LC_MESSAGES/django.po` & `aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ko_KR/LC_MESSAGES/django.po` & `aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.4.2/aa_rss_to_discord/locale/ru/LC_MESSAGES/django.po` & `aa_rss_to_discord-1.5.0/aa_rss_to_discord/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 20% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
-"n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
-"(n%100>=11 && n%100<=14)? 2 : 3);\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
 
 #: models.py:41
 msgid "RSS Feed"
 msgstr ""
 
 #: models.py:42
 msgid "RSS Feeds"
```

### Comparing `aa_rss_to_discord-1.4.2/aa_rss_to_discord/migrations/0001_initial.py` & `aa_rss_to_discord-1.5.0/aa_rss_to_discord/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.4.2/aa_rss_to_discord/models.py` & `aa_rss_to_discord-1.5.0/aa_rss_to_discord/models.py`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.4.2/aa_rss_to_discord/tasks.py` & `aa_rss_to_discord-1.5.0/aa_rss_to_discord/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-1.4.2/aa_rss_to_discord.egg-info/PKG-INFO` & `aa_rss_to_discord-1.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aa-rss-to-discord
-Version: 1.4.2
+Name: aa_rss_to_discord
+Version: 1.5.0
 Summary: Alliance Auth module to post news from RSS feeds to your Discord
 Home-page: https://github.com/ppfeufer/aa-rss-to-discord
 Author: Peter Pfeufer
 Author-email: develop@ppfeufer.de
 Maintainer: Peter Pfeufer
 Maintainer-email: develop@ppfeufer.de
 License: GPL-3.0
@@ -42,57 +42,60 @@
 [![codecov](https://codecov.io/gh/ppfeufer/aa-rss-to-discord/branch/master/graph/badge.svg?token=LVEQ6W55ZB)](https://codecov.io/gh/ppfeufer/aa-rss-to-discord)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](https://github.com/ppfeufer/aa-rss-to-discord/blob/master/CODE_OF_CONDUCT.md)
 
 [![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/N4N8CL1BY)
 
 A simple app to post selected RSS feeds to your Discord.
 
+---
 
-## Contents
-
-- [Installation](#installation)
-  - [Step 0.5 - Install AA-Discordbot](#step-05---install-aa-discordbot)
-  - [Step 1 - Install the Package](#step-1---install-the-package)
-  - [Step 2 - Configure Alliance Auth](#step-2---configure-alliance-auth)
-  - [Step 3 - Finalize the Installation](#step-3---finalize-the-installation)
-  - [Step 4 - Configure your RSS Feeds](#step-4---configure-your-rss-feeds)
-- [Discord Bot Commands](#discord-bot-commands)
-- [Updating](#updating)
+<!-- TOC -->
+* [Alliance Auth RSS to Discord](#alliance-auth-rss-to-discord)
+  * [Installation](#installation)
+    * [Step 0.5: Install AA-Discordbot](#step-05-install-aa-discordbot)
+    * [Step 1: Install the Package](#step-1-install-the-package)
+    * [Step 2: Configure Alliance Auth](#step-2-configure-alliance-auth)
+    * [Step 3: Finalizing the Installation](#step-3-finalizing-the-installation)
+    * [Step 4: Configure your RSS Feeds](#step-4-configure-your-rss-feeds)
+  * [Discord Bot Commands](#discord-bot-commands)
+  * [Updating](#updating)
+<!-- TOC -->
 
+---
 
 ## Installation
 
 **Important**: Please make sure you meet all preconditions before you proceed:
 
 - Alliance Auth RSS to Discord is a plugin for Alliance Auth. If you don't have Alliance Auth running
   already, please install it first before proceeding. (see the official
   [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html) for details)
 - Alliance Auth RSS to Discord needs [AA-Discordbot](https://github.com/pvyParts/allianceauth-discordbot)
   to interact with your Discord server. Make sure it is installed and configured
   **before** installing this app.
 
 
-### Step 0.5 - Install AA-Discordbot
+### Step 0.5: Install AA-Discordbot
 
 In order for this app to work, you need to install and configure
 [AA-Discordbot](https://github.com/pvyParts/allianceauth-discordbot) first. Read the
 instructions how to do so in the README of AA-Discordbot.
 
 
-### Step 1 - Install the Package
+### Step 1: Install the Package
 
-Make sure you are in the virtual environment (venv) of your Alliance Auth
-installation Then install the latest releast directly from PyPi.
+Make sure you're in the virtual environment (venv) of your Alliance Auth
+installation Then install the latest release directly from PyPi.
 
 ```shell
 pip install aa-rss-to-discord
 ```
 
 
-### Step 2 - Configure Alliance Auth
+### Step 2: Configure Alliance Auth
 
 This is fairly simple, just add the following to the `INSTALLED_APPS` of your `local.py`
 
 Configure your AA settings (`local.py`) as follows:
 
 - Add `"aa_rss_to_discord",` to `INSTALLED_APPS`
 - Add the scheduled task
@@ -100,52 +103,53 @@
   CELERYBEAT_SCHEDULE["aa_rss_to_discord_fetch_rss"] = {
       "task": "aa_rss_to_discord.tasks.fetch_rss",
       "schedule": crontab(minute="*/5"),
   }
   ```
 
 
-### Step 3 - Finalize the Installation
+### Step 3: Finalizing the Installation
 
 Run migrations to finalize the installation
 
 ```shell
 python manage.py migrate
 ```
 
-Finally restart your supervisor services for AA.
+Finally, restart your supervisor services for AA.
 
 
-### Step 4 - Configure your RSS Feeds
+### Step 4: Configure your RSS Feeds
 
-First you need to set up the Discord Server and Channels. For this you go in your
+First, you need to set up the Discord Server and Channels. For this, you go in your
 admin backend to the Discordbot settings and enter the needed information there.
 
 When done, you can set up your RSS feeds. This can be done in the setting of this
 app, still in your admin backend. Create a new RSS Feed entry, enter the name, url
 and select the Discord channel it should be posted to. Once done, save it.
 
 
 ## Discord Bot Commands
 
 The following commands are available for the Discord bot to manage RSS/Atom feeds:
 
-| Command | Options | What it does |
-|:---|:---|:---|
-| `!rss_add <rss_url> <rss_name>` | - `rss_url` - The URL of the RSS/Atom feed<br>- `rss_name` - A Name for the RSS/Atom Feed | Adding a RSS/Atom fedd to the current channel |
-| `!rss_delete <rss_feed_id>` | `rss_feed_id` - The ID of the RSS/Atom feed you want to remove |  Remove a RSS/Atom feed from the current Discord channel |
-| `!rss_disable <rss_feed_id>` | `rss_feed_id` - The ID of the RSS/Atom feed you want to disable |  Disable an enabled RSS/Atom feed for the current Discord channel |
-| `!rss_enable <rss_feed_id>` | `rss_feed_id` - The ID of the RSS/Atom feed you want to enable |  Enable a disabled RSS/Atom feed for the current Discord channel |
-| `!rss_list` | None |  List all RSS/Atom feeds for the current Discord channel |
+| Command                         | Options                                                                                   | What it does                                                     |
+|:--------------------------------|:------------------------------------------------------------------------------------------|:-----------------------------------------------------------------|
+| `!rss_add <rss_url> <rss_name>` | - `rss_url` - The URL of the RSS/Atom feed<br>- `rss_name` - A Name for the RSS/Atom Feed | Adding a RSS/Atom feed to the current channel                    |
+| `!rss_delete <rss_feed_id>`     | `rss_feed_id` - The ID of the RSS/Atom feed you want to remove                            | Remove a RSS/Atom feed from the current Discord channel          |
+| `!rss_disable <rss_feed_id>`    | `rss_feed_id` - The ID of the RSS/Atom feed you want to disable                           | Disable an enabled RSS/Atom feed for the current Discord channel |
+| `!rss_enable <rss_feed_id>`     | `rss_feed_id` - The ID of the RSS/Atom feed you want to enable                            | Enable a disabled RSS/Atom feed for the current Discord channel  |
+| `!rss_list`                     | None                                                                                      | List all RSS/Atom feeds for the current Discord channel          |
+
 
 ## Updating
 
 To update your existing installation of Alliance Auth RSS to Discord, first enable your
 virtual environment (venv) of your Alliance Auth installation.
 
 ```bash
 pip install -U aa-rss-to-discord
 
 python manage.py migrate
 ```
 
-Finally restart your supervisor services for AA.
+Finally, restart your supervisor services for AA.
```

### Comparing `aa_rss_to_discord-1.4.2/aa_rss_to_discord.egg-info/SOURCES.txt` & `aa_rss_to_discord-1.5.0/aa_rss_to_discord.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -23,12 +23,13 @@
 aa_rss_to_discord/locale/de/LC_MESSAGES/django.mo
 aa_rss_to_discord/locale/de/LC_MESSAGES/django.po
 aa_rss_to_discord/locale/es/LC_MESSAGES/django.po
 aa_rss_to_discord/locale/fr_FR/LC_MESSAGES/django.po
 aa_rss_to_discord/locale/it_IT/LC_MESSAGES/django.po
 aa_rss_to_discord/locale/ja/LC_MESSAGES/django.po
 aa_rss_to_discord/locale/ko_KR/LC_MESSAGES/django.po
+aa_rss_to_discord/locale/ru/LC_MESSAGES/django.mo
 aa_rss_to_discord/locale/ru/LC_MESSAGES/django.po
 aa_rss_to_discord/locale/zh_Hans/LC_MESSAGES/django.po
 aa_rss_to_discord/migrations/0001_initial.py
 aa_rss_to_discord/migrations/0002_enable_disable_rss_feeds.py
 aa_rss_to_discord/migrations/__init__.py
```

### Comparing `aa_rss_to_discord-1.4.2/setup.cfg` & `aa_rss_to_discord-1.5.0/setup.cfg`

 * *Files identical despite different names*

