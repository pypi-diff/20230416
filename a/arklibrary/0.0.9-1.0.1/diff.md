# Comparing `tmp/arklibrary-0.0.9.tar.gz` & `tmp/arklibrary-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arklibrary-0.0.9.tar", last modified: Sun Aug 21 00:22:06 2022, max compression
+gzip compressed data, was "arklibrary-1.0.1.tar", last modified: Sat Apr 15 22:59:16 2023, max compression
```

## Comparing `arklibrary-0.0.9.tar` & `arklibrary-1.0.1.tar`

### file list

```diff
@@ -1,63 +1,67 @@
-drwxrwxrwx   0        0        0        0 2022-08-21 00:22:06.676860 arklibrary-0.0.9/
--rw-rw-rw-   0        0        0     1095 2022-08-11 13:59:26.000000 arklibrary-0.0.9/LICENSE
--rw-rw-rw-   0        0        0      662 2022-08-21 00:22:06.677859 arklibrary-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       13 2022-08-17 05:16:41.000000 arklibrary-0.0.9/README.md
--rw-rw-rw-   0        0        0      536 2022-08-17 05:16:41.000000 arklibrary-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0      995 2022-08-21 00:22:06.682860 arklibrary-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-08-21 00:22:06.626860 arklibrary-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2022-08-21 00:22:06.633859 arklibrary-0.0.9/src/arklibrary/
--rw-rw-rw-   0        0        0      130 2022-08-20 20:36:56.000000 arklibrary-0.0.9/src/arklibrary/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-21 00:22:06.646865 arklibrary-0.0.9/src/arklibrary/admin/
--rw-rw-rw-   0        0        0      303 2022-08-20 22:13:21.000000 arklibrary-0.0.9/src/arklibrary/admin/__init__.py
--rw-rw-rw-   0        0        0     1800 2022-08-20 22:37:07.000000 arklibrary-0.0.9/src/arklibrary/admin/admin.py
--rw-rw-rw-   0        0        0    10216 2022-08-20 22:38:20.000000 arklibrary-0.0.9/src/arklibrary/admin/bundle.py
--rw-rw-rw-   0        0        0    20084 2022-08-20 22:38:20.000000 arklibrary-0.0.9/src/arklibrary/admin/commands.py
--rw-rw-rw-   0        0        0     2123 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/admin/run_driver.py
-drwxrwxrwx   0        0        0        0 2022-08-21 00:22:06.664860 arklibrary-0.0.9/src/arklibrary/blueprints/
--rw-rw-rw-   0        0        0     1101 2022-08-20 22:13:21.000000 arklibrary-0.0.9/src/arklibrary/blueprints/__init__.py
--rw-rw-rw-   0        0        0     3803 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/ammunitions.py
--rw-rw-rw-   0        0        0     9636 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/armours.py
--rw-rw-rw-   0        0        0     9294 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/artifacts.py
--rw-rw-rw-   0        0        0    11005 2021-10-13 20:30:55.000000 arklibrary-0.0.9/src/arklibrary/blueprints/beacons.py
--rw-rw-rw-   0        0        0    17601 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/chibis.py
--rw-rw-rw-   0        0        0     7885 2021-10-13 20:02:05.000000 arklibrary-0.0.9/src/arklibrary/blueprints/colors.py
--rw-rw-rw-   0        0        0     9913 2021-09-24 02:50:11.000000 arklibrary-0.0.9/src/arklibrary/blueprints/commands.py
--rw-rw-rw-   0        0        0    21773 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/consumables.py
--rw-rw-rw-   0        0        0    78373 2022-08-20 22:11:17.000000 arklibrary-0.0.9/src/arklibrary/blueprints/creatures.py
--rw-rw-rw-   0        0        0     3028 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/dyes.py
--rw-rw-rw-   0        0        0    11739 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/eggs.py
--rw-rw-rw-   0        0        0      942 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/farming.py
--rw-rw-rw-   0        0        0     2368 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/recipes.py
--rw-rw-rw-   0        0        0    11037 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/resources.py
--rw-rw-rw-   0        0        0    13208 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/saddles.py
--rw-rw-rw-   0        0        0     2146 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/seeds.py
--rw-rw-rw-   0        0        0    33071 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/skins.py
--rw-rw-rw-   0        0        0    52735 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/structures.py
--rw-rw-rw-   0        0        0     3409 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/tools.py
--rw-rw-rw-   0        0        0     5723 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/trophies.py
--rw-rw-rw-   0        0        0     8052 2022-08-20 22:05:40.000000 arklibrary-0.0.9/src/arklibrary/blueprints/weapons.py
--rw-rw-rw-   0        0        0      227 2022-08-15 04:49:50.000000 arklibrary-0.0.9/src/arklibrary/config.ini
-drwxrwxrwx   0        0        0        0 2022-08-21 00:22:06.668862 arklibrary-0.0.9/src/arklibrary/data_structures/
--rw-rw-rw-   0        0        0       88 2022-08-20 20:52:25.000000 arklibrary-0.0.9/src/arklibrary/data_structures/__init__.py
--rw-rw-rw-   0        0        0      602 2022-08-20 23:21:23.000000 arklibrary-0.0.9/src/arklibrary/data_structures/encoder.py
--rw-rw-rw-   0        0        0     2306 2022-08-21 00:21:58.000000 arklibrary-0.0.9/src/arklibrary/data_structures/stream.py
--rw-rw-rw-   0        0        0     4224 2022-08-20 22:39:42.000000 arklibrary-0.0.9/src/arklibrary/data_structures/tri.py
-drwxrwxrwx   0        0        0        0 2022-08-21 00:22:06.669859 arklibrary-0.0.9/src/arklibrary/events/
--rw-rw-rw-   0        0        0        0 2022-08-20 18:00:52.000000 arklibrary-0.0.9/src/arklibrary/events/__init__.py
--rw-rw-rw-   0        0        0     5211 2021-10-17 07:56:36.000000 arklibrary-0.0.9/src/arklibrary/events/events.py
-drwxrwxrwx   0        0        0        0 2022-08-21 00:22:06.671861 arklibrary-0.0.9/src/arklibrary/lib/
--rw-rw-rw-   0        0        0       69 2022-08-17 05:16:41.000000 arklibrary-0.0.9/src/arklibrary/lib/__init__.py
--rw-rw-rw-   0        0        0     2278 2022-08-20 22:39:42.000000 arklibrary-0.0.9/src/arklibrary/lib/configuration.py
-drwxrwxrwx   0        0        0        0 2022-08-21 00:22:06.676860 arklibrary-0.0.9/src/arklibrary/tools/
--rw-rw-rw-   0        0        0        2 2021-10-15 20:23:29.000000 arklibrary-0.0.9/src/arklibrary/tools/__init__.py
--rw-rw-rw-   0        0        0     2831 2021-10-05 00:32:43.000000 arklibrary-0.0.9/src/arklibrary/tools/ark_generic_scraper.py
--rw-rw-rw-   0        0        0    14575 2021-10-13 20:49:49.000000 arklibrary-0.0.9/src/arklibrary/tools/ark_image_scraper.py
--rw-rw-rw-   0        0        0     4478 2021-09-24 02:58:55.000000 arklibrary-0.0.9/src/arklibrary/tools/clipboard.py
--rw-rw-rw-   0        0        0      956 2022-08-20 22:39:42.000000 arklibrary-0.0.9/src/arklibrary/tools/config.py
--rw-rw-rw-   0        0        0     1196 2021-09-24 02:57:41.000000 arklibrary-0.0.9/src/arklibrary/tools/read.py
-drwxrwxrwx   0        0        0        0 2022-08-21 00:22:06.642859 arklibrary-0.0.9/src/arklibrary.egg-info/
--rw-rw-rw-   0        0        0      662 2022-08-21 00:22:06.000000 arklibrary-0.0.9/src/arklibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1776 2022-08-21 00:22:06.000000 arklibrary-0.0.9/src/arklibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-21 00:22:06.000000 arklibrary-0.0.9/src/arklibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       82 2022-08-21 00:22:06.000000 arklibrary-0.0.9/src/arklibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-08-21 00:22:06.000000 arklibrary-0.0.9/src/arklibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 22:59:16.771011 arklibrary-1.0.1/
+-rw-rw-rw-   0        0        0     1095 2023-03-25 16:33:09.000000 arklibrary-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      713 2023-04-15 22:59:16.771011 arklibrary-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-03-25 16:33:09.000000 arklibrary-1.0.1/README.md
+-rw-rw-rw-   0        0        0      609 2023-04-11 00:15:08.000000 arklibrary-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1129 2023-04-15 22:59:16.773014 arklibrary-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 22:59:16.717184 arklibrary-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 22:59:16.723185 arklibrary-1.0.1/src/arklibrary/
+-rw-rw-rw-   0        0        0      336 2023-04-04 02:19:21.000000 arklibrary-1.0.1/src/arklibrary/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 22:59:16.738222 arklibrary-1.0.1/src/arklibrary/admin/
+-rw-rw-rw-   0        0        0      121 2023-03-31 21:02:39.000000 arklibrary-1.0.1/src/arklibrary/admin/__init__.py
+-rw-rw-rw-   0        0        0    21095 2023-04-04 03:30:02.000000 arklibrary-1.0.1/src/arklibrary/admin/admin.py
+-rw-rw-rw-   0        0        0    10273 2023-03-31 21:01:19.000000 arklibrary-1.0.1/src/arklibrary/admin/bundle.py
+-rw-rw-rw-   0        0        0     2115 2023-03-31 21:01:19.000000 arklibrary-1.0.1/src/arklibrary/admin/run_driver.py
+drwxrwxrwx   0        0        0        0 2023-04-15 22:59:16.755997 arklibrary-1.0.1/src/arklibrary/blueprints/
+-rw-rw-rw-   0        0        0     1101 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/__init__.py
+-rw-rw-rw-   0        0        0     3803 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/ammunitions.py
+-rw-rw-rw-   0        0        0     9636 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/armours.py
+-rw-rw-rw-   0        0        0     9294 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/artifacts.py
+-rw-rw-rw-   0        0        0    11005 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/beacons.py
+-rw-rw-rw-   0        0        0    17601 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/chibis.py
+-rw-rw-rw-   0        0        0     7885 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/colors.py
+-rw-rw-rw-   0        0        0     9916 2023-04-04 03:26:01.000000 arklibrary-1.0.1/src/arklibrary/blueprints/commands.py
+-rw-rw-rw-   0        0        0    21773 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/consumables.py
+-rw-rw-rw-   0        0        0    78373 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/creatures.py
+-rw-rw-rw-   0        0        0     3028 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/dyes.py
+-rw-rw-rw-   0        0        0    11739 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/eggs.py
+-rw-rw-rw-   0        0        0      942 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/farming.py
+-rw-rw-rw-   0        0        0     2368 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/recipes.py
+-rw-rw-rw-   0        0        0    11037 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/resources.py
+-rw-rw-rw-   0        0        0    13208 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/saddles.py
+-rw-rw-rw-   0        0        0     2146 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/seeds.py
+-rw-rw-rw-   0        0        0    33071 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/skins.py
+-rw-rw-rw-   0        0        0    52735 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/structures.py
+-rw-rw-rw-   0        0        0     3409 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/tools.py
+-rw-rw-rw-   0        0        0     5723 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/trophies.py
+-rw-rw-rw-   0        0        0     8052 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/weapons.py
+-rw-rw-rw-   0        0        0      313 2023-04-04 01:37:11.000000 arklibrary-1.0.1/src/arklibrary/config.ini
+drwxrwxrwx   0        0        0        0 2023-04-15 22:59:16.758997 arklibrary-1.0.1/src/arklibrary/data_structures/
+-rw-rw-rw-   0        0        0       88 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/data_structures/__init__.py
+-rw-rw-rw-   0        0        0      646 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/data_structures/encoder.py
+-rw-rw-rw-   0        0        0     2327 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/data_structures/stream.py
+-rw-rw-rw-   0        0        0     4224 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/data_structures/tri.py
+drwxrwxrwx   0        0        0        0 2023-04-15 22:59:16.759998 arklibrary-1.0.1/src/arklibrary/events/
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/events/__init__.py
+-rw-rw-rw-   0        0        0     5211 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/events/events.py
+drwxrwxrwx   0        0        0        0 2023-04-15 22:59:16.763999 arklibrary-1.0.1/src/arklibrary/lib/
+-rw-rw-rw-   0        0        0      166 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/lib/__init__.py
+-rw-rw-rw-   0        0        0     2662 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/lib/configuration.py
+-rw-rw-rw-   0        0        0     4115 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/lib/console.py
+-rw-rw-rw-   0        0        0     4152 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/lib/logger.py
+-rw-rw-rw-   0        0        0     2495 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/lib/pathify.py
+drwxrwxrwx   0        0        0        0 2023-04-15 22:59:16.771011 arklibrary-1.0.1/src/arklibrary/tools/
+-rw-rw-rw-   0        0        0      137 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/tools/__init__.py
+-rw-rw-rw-   0        0        0     2831 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/tools/ark_generic_scraper.py
+-rw-rw-rw-   0        0        0    14575 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/tools/ark_image_scraper.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/tools/aws.py
+-rw-rw-rw-   0        0        0     4478 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/tools/clipboard.py
+-rw-rw-rw-   0        0        0      956 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/tools/config.py
+-rw-rw-rw-   0        0        0     3794 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/tools/namecheap.py
+-rw-rw-rw-   0        0        0     1196 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/tools/read.py
+drwxrwxrwx   0        0        0        0 2023-04-15 22:59:16.735222 arklibrary-1.0.1/src/arklibrary.egg-info/
+-rw-rw-rw-   0        0        0      713 2023-04-15 22:59:16.000000 arklibrary-1.0.1/src/arklibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1894 2023-04-15 22:59:16.000000 arklibrary-1.0.1/src/arklibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 22:59:16.000000 arklibrary-1.0.1/src/arklibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-04-15 22:59:16.000000 arklibrary-1.0.1/src/arklibrary.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-15 22:59:16.000000 arklibrary-1.0.1/src/arklibrary.egg-info/top_level.txt
```

### Comparing `arklibrary-0.0.9/LICENSE` & `arklibrary-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/PKG-INFO` & `arklibrary-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: arklibrary
-Version: 0.0.9
+Version: 1.0.1
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Library
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Library/issues
 Platform: win32
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # Ark-Library
```

### Comparing `arklibrary-0.0.9/pyproject.toml` & `arklibrary-1.0.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 [build-system]
 requires = [
     "setuptools>=42",
-    "wheel"
+    "wheel",
+    "requests>=2.28.2",
+    "xmltodict>=0.13.0",
+    "numpy>=1.24.2"
 ]
 build-backend = "setuptools.build_meta"
 
 
 [too.pytest.ini_options]
 addopts = "--cov=arklibrary"
 testpaths = [
```

### Comparing `arklibrary-0.0.9/setup.cfg` & `arklibrary-1.0.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,71 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 726b 6c69 6272 6172 790d 0a76   = arklibrary..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e39 0d0a  ersion = 0.0.9..
-00000030: 6175 7468 6f72 203d 204d 6175 7269 6369  author = Maurici
-00000040: 6f0d 0a61 7574 686f 725f 656d 6169 6c20  o..author_email 
-00000050: 3d20 6465 762e 6d61 7572 6963 696f 2e6c  = dev.mauricio.l
-00000060: 6f6d 656c 6940 676d 6169 6c2e 636f 6d0d  omeli@gmail.com.
-00000070: 0a64 6573 6372 6970 7469 6f6e 203d 2054  .description = T
-00000080: 6869 7320 6170 706c 6963 6174 696f 6e20  his application 
-00000090: 6163 6365 7373 6573 2074 6865 2041 726b  accesses the Ark
-000000a0: 2073 7973 7465 6d2e 0d0a 6c6f 6e67 5f64   system...long_d
-000000b0: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
-000000c0: 653a 2052 4541 444d 452e 6d64 0d0a 6c6f  e: README.md..lo
-000000d0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
-000000e0: 6f6e 7465 6e74 5f74 7970 6520 3d20 7465  ontent_type = te
-000000f0: 7874 2f6d 6172 6b64 6f77 6e0d 0a75 726c  xt/markdown..url
-00000100: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-00000110: 622e 636f 6d2f 4761 6d65 5365 7276 6572  b.com/GameServer
-00000120: 4775 7275 732f 4172 6b2d 4c69 6272 6172  Gurus/Ark-Librar
-00000130: 790d 0a70 726f 6a65 6374 5f75 726c 7320  y..project_urls 
-00000140: 3d20 0d0a 0942 7567 2054 7261 636b 6572  = ...Bug Tracker
-00000150: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-00000160: 622e 636f 6d2f 4761 6d65 5365 7276 6572  b.com/GameServer
-00000170: 4775 7275 732f 4172 6b2d 4c69 6272 6172  Gurus/Ark-Librar
-00000180: 792f 6973 7375 6573 0d0a 706c 6174 666f  y/issues..platfo
-00000190: 726d 7320 3d20 7769 6e33 320d 0a63 6c61  rms = win32..cla
-000001a0: 7373 6966 6965 7273 203d 200d 0a09 5072  ssifiers = ...Pr
-000001b0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001c0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000001d0: 332e 390d 0a09 5072 6f67 7261 6d6d 696e  3.9...Programmin
-000001e0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000001f0: 7468 6f6e 203a 3a20 332e 3130 0d0a 090d  thon :: 3.10....
-00000200: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
-00000210: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-00000220: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
-00000230: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-00000240: 5320 496e 6465 7065 6e64 656e 740d 0a0d  S Independent...
-00000250: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
-00000260: 6167 655f 6469 7220 3d20 0d0a 093d 2073  age_dir = ...= s
-00000270: 7263 0d0a 7061 636b 6167 6573 203d 2066  rc..packages = f
-00000280: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
-00000290: 7569 7265 7320 3d20 3e3d 332e 390d 0a69  uires = >=3.9..i
-000002a0: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
-000002b0: 3d20 0d0a 0972 6571 7565 7374 730d 0a0d  = ...requests...
-000002c0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-000002d0: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-000002e0: 3d20 7372 630d 0a0d 0a5b 6f70 7469 6f6e  = src....[option
-000002f0: 732e 6578 7472 6173 5f72 6571 7569 7265  s.extras_require
-00000300: 5d0d 0a74 6573 7469 6e67 203d 200d 0a09  ]..testing = ...
-00000310: 7079 7465 7374 3e3d 362e 300d 0a09 7079  pytest>=6.0...py
-00000320: 7465 7374 2d63 6f76 3e3d 322e 300d 0a09  test-cov>=2.0...
-00000330: 6d79 7079 3e3d 302e 3937 310d 0a09 666c  mypy>=0.971...fl
-00000340: 616b 6538 3e3d 332e 390d 0a09 746f 783e  ake8>=3.9...tox>
-00000350: 3d33 2e32 340d 0a0d 0a5b 6f70 7469 6f6e  =3.24....[option
-00000360: 732e 7061 636b 6167 655f 6461 7461 5d0d  s.package_data].
-00000370: 0a61 726b 6c69 6272 6172 7920 3d20 7079  .arklibrary = py
-00000380: 2e74 7970 6564 2c20 636f 6e66 6967 2e69  .typed, config.i
-00000390: 6e69 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a  ni....[flake8]..
-000003a0: 6d61 782d 6c69 6e65 2d6c 656e 6774 6820  max-line-length 
-000003b0: 3d20 3136 300d 0a0d 0a5b 6567 675f 696e  = 160....[egg_in
-000003c0: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-000003d0: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-000003e0: 0a0d 0a                                  ...
+00000020: 6572 7369 6f6e 203d 2031 2e30 2e31 0d0a  ersion = 1.0.1..
+00000030: 7072 6f64 7563 7469 6f6e 5f76 6572 7369  production_versi
+00000040: 6f6e 203d 2031 2e30 2e31 0d0a 7465 7374  on = 1.0.1..test
+00000050: 5f76 6572 7369 6f6e 203d 2031 2e30 2e32  _version = 1.0.2
+00000060: 0d0a 6175 7468 6f72 203d 204d 6175 7269  ..author = Mauri
+00000070: 6369 6f0d 0a61 7574 686f 725f 656d 6169  cio..author_emai
+00000080: 6c20 3d20 6465 762e 6d61 7572 6963 696f  l = dev.mauricio
+00000090: 2e6c 6f6d 656c 6940 676d 6169 6c2e 636f  .lomeli@gmail.co
+000000a0: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
+000000b0: 2054 6869 7320 6170 706c 6963 6174 696f   This applicatio
+000000c0: 6e20 6163 6365 7373 6573 2074 6865 2041  n accesses the A
+000000d0: 726b 2073 7973 7465 6d2e 0d0a 6c6f 6e67  rk system...long
+000000e0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
+000000f0: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
+00000100: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+00000110: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
+00000120: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
+00000130: 726c 203d 2068 7474 7073 3a2f 2f67 6974  rl = https://git
+00000140: 6875 622e 636f 6d2f 4761 6d65 5365 7276  hub.com/GameServ
+00000150: 6572 4775 7275 732f 4172 6b2d 4c69 6272  erGurus/Ark-Libr
+00000160: 6172 790d 0a70 726f 6a65 6374 5f75 726c  ary..project_url
+00000170: 7320 3d20 0d0a 0942 7567 2054 7261 636b  s = ...Bug Track
+00000180: 6572 203d 2068 7474 7073 3a2f 2f67 6974  er = https://git
+00000190: 6875 622e 636f 6d2f 4761 6d65 5365 7276  hub.com/GameServ
+000001a0: 6572 4775 7275 732f 4172 6b2d 4c69 6272  erGurus/Ark-Libr
+000001b0: 6172 792f 6973 7375 6573 0d0a 706c 6174  ary/issues..plat
+000001c0: 666f 726d 7320 3d20 7769 6e33 320d 0a63  forms = win32..c
+000001d0: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
+000001e0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000001f0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000200: 3a20 332e 380d 0a09 5072 6f67 7261 6d6d  : 3.8...Programm
+00000210: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000220: 5079 7468 6f6e 203a 3a20 332e 390d 0a09  Python :: 3.9...
+00000230: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000240: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000250: 3a20 332e 3130 0d0a 090d 0a09 4c69 6365  : 3.10......Lice
+00000260: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000270: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+00000280: 7365 0d0a 094f 7065 7261 7469 6e67 2053  se...Operating S
+00000290: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
+000002a0: 7065 6e64 656e 740d 0a0d 0a5b 6f70 7469  pendent....[opti
+000002b0: 6f6e 735d 0d0a 7061 636b 6167 655f 6469  ons]..package_di
+000002c0: 7220 3d20 0d0a 093d 2073 7263 0d0a 7061  r = ...= src..pa
+000002d0: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
+000002e0: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
+000002f0: 3d20 3e3d 332e 380d 0a69 6e73 7461 6c6c  = >=3.8..install
+00000300: 5f72 6571 7569 7265 7320 3d20 0d0a 0972  _requires = ...r
+00000310: 6571 7565 7374 733e 3d32 2e32 382e 320d  equests>=2.28.2.
+00000320: 0a09 786d 6c74 6f64 6963 743e 3d30 2e31  ..xmltodict>=0.1
+00000330: 332e 300d 0a09 6e75 6d70 793e 3d31 2e32  3.0...numpy>=1.2
+00000340: 342e 320d 0a0d 0a5b 6f70 7469 6f6e 732e  4.2....[options.
+00000350: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
+00000360: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
+00000370: 6f70 7469 6f6e 732e 6578 7472 6173 5f72  options.extras_r
+00000380: 6571 7569 7265 5d0d 0a74 6573 7469 6e67  equire]..testing
+00000390: 203d 200d 0a09 7079 7465 7374 3e3d 362e   = ...pytest>=6.
+000003a0: 300d 0a09 7079 7465 7374 2d63 6f76 3e3d  0...pytest-cov>=
+000003b0: 322e 300d 0a09 6d79 7079 3e3d 302e 3937  2.0...mypy>=0.97
+000003c0: 310d 0a09 666c 616b 6538 3e3d 332e 390d  1...flake8>=3.9.
+000003d0: 0a09 746f 783e 3d33 2e32 340d 0a0d 0a5b  ..tox>=3.24....[
+000003e0: 6f70 7469 6f6e 732e 7061 636b 6167 655f  options.package_
+000003f0: 6461 7461 5d0d 0a61 726b 6c69 6272 6172  data]..arklibrar
+00000400: 7920 3d20 7079 2e74 7970 6564 2c20 636f  y = py.typed, co
+00000410: 6e66 6967 2e69 6e69 0d0a 0d0a 5b66 6c61  nfig.ini....[fla
+00000420: 6b65 385d 0d0a 6d61 782d 6c69 6e65 2d6c  ke8]..max-line-l
+00000430: 656e 6774 6820 3d20 3136 300d 0a0d 0a5b  ength = 160....[
+00000440: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+00000450: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+00000460: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `arklibrary-0.0.9/src/arklibrary/admin/bundle.py` & `arklibrary-1.0.1/src/arklibrary/admin/bundle.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,194 +1,198 @@
-from arklibrary.admin.commands import Commands
-from arklibrary.blueprints import *
+from arklibrary.blueprints import Weapons, Structures, Tools, Resources
+from arklibrary.blueprints import Armour, Dinos, Saddles, Ammunition
+from arklibrary.admin import Admin
 import math
 
 
-class Bundle(Commands):
+class Bundle:
+    def __init__(self, admin: Admin):
+        self.admin = admin
+
     def execute(self):
-        self.execute()
+        self.admin.execute()
 
     def flak_armour(self, player_id, quality=0):
         boots = Armour.FLAK_BOOTS
         leggings = Armour.FLAK_LEGGINGS
         chest = Armour.FLAK_CHESTPIECE
         gauntlets = Armour.FLAK_GAUNTLETS
         helmet = Armour.FLAK_HELMET
         wings = Armour.GLIDER_SUIT
-        self.give_items_to_player(player_id, [boots, leggings, chest, gauntlets, helmet, wings], quality=quality)
+        self.admin.give_items_to_player(player_id, [boots, leggings, chest, gauntlets, helmet, wings], quality=quality)
 
     def hazard_armour(self, player_id, quality=0):
         boots = Armour.HAZARD_SUIT_BOOTS
         leggings = Armour.HAZARD_SUIT_PANTS
         chest = Armour.HAZARD_SUIT_SHIRT
         gauntlets = Armour.HAZARD_SUIT_GLOVES
         helmet = Armour.HAZARD_SUIT_HAT
         wings = Armour.GLIDER_SUIT
-        self.give_items_to_player(player_id, [boots, leggings, chest, gauntlets, helmet, wings], quality=quality)
+        self.admin.give_items_to_player(player_id, [boots, leggings, chest, gauntlets, helmet, wings], quality=quality)
 
     def desert_armour(self, player_id, quality=0):
         boots = Armour.DESERT_CLOTH_BOOTS
         leggings = Armour.DESERT_CLOTH_PANTS
         chest = Armour.DESERT_CLOTH_SHIRT
         gauntlets = Armour.DESERT_CLOTH_GLOVES
         helmet = Armour.DESERT_GOGGLES_AND_HAT
         wings = Armour.GLIDER_SUIT
-        self.give_items_to_player(player_id, [boots, leggings, chest, gauntlets, helmet, wings], quality=quality)
+        self.admin.give_items_to_player(player_id, [boots, leggings, chest, gauntlets, helmet, wings], quality=quality)
 
     def fur_armour(self, player_id, quality=0):
         boots = Armour.FUR_BOOTS
         leggings = Armour.FUR_LEGGINGS
         chest = Armour.FUR_CHESTPIECE
         gauntlets = Armour.FUR_GAUNTLETS
         helmet = Armour.FUR_CAP
         wings = Armour.GLIDER_SUIT
-        self.give_items_to_player(player_id, [boots, leggings, chest, gauntlets, helmet, wings], quality=quality)
+        self.admin.give_items_to_player(player_id, [boots, leggings, chest, gauntlets, helmet, wings], quality=quality)
 
     def tek_armour(self, player_id, quality=0):
         boots = Armour.TEK_BOOTS
         leggings = Armour.TEK_LEGGINGS
         chest = Armour.TEK_CHESTPIECE
         gauntlets = Armour.TEK_GAUNTLETS
         helmet = Armour.TEK_HELMET
-        self.give_items_to_player(player_id, [boots, leggings, chest, gauntlets, helmet], quality=quality)
+        self.admin.give_items_to_player(player_id, [boots, leggings, chest, gauntlets, helmet], quality=quality)
 
     def dino_starter(self, player_id, level=150):
-        self.teleport_to_playerid(player_id)
-        self.spawn_exact_dino(Dinos.PTERANODON, base_level=level)
-        self.give_items_to_player(player_id, Saddles.PTERANODON_SADDLE)
+        self.admin.teleport_to_playerid(player_id)
+        self.admin.spawn_exact_dino(Dinos.PTERANODON, base_level=level)
+        self.admin.give_items_to_player(player_id, Saddles.PTERANODON_SADDLE)
 
     def rocket_set(self, player_id):
         rockets = Ammunition.ROCKET_PROPELLED_GRENADE
         launcher = Weapons.ROCKET_LAUNCHER
-        self.give_items_to_player(player_id, [rockets], quantity=10)
-        self.give_items_to_player(player_id, [launcher])
+        self.admin.give_items_to_player(player_id, [rockets], quantity=10)
+        self.admin.give_items_to_player(player_id, [launcher])
 
     def shotgun_set(self, player_id, quality=0):
         shotgun = Weapons.PUMP_ACTION_SHOTGUN
         ammo = Ammunition.SIMPLE_SHOTGUN_AMMO
-        self.give_items_to_player(player_id, [ammo], quantity=100)
-        self.give_items_to_player(player_id, [shotgun], quality=quality)
+        self.admin.give_items_to_player(player_id, [ammo], quantity=100)
+        self.admin.give_items_to_player(player_id, [shotgun], quality=quality)
 
     def soaker_set(self, player_id, level=150, quality=0):
-        self.teleport_to_playerid(player_id)
-        self.spawn_exact_dino(Dinos.TEK_STEGOSAURUS, base_level=level)
-        self.give_items_to_player(player_id, Saddles.STEGO_SADDLE, quality=quality)
+        self.admin.teleport_to_playerid(player_id)
+        self.admin.spawn_exact_dino(Dinos.TEK_STEGOSAURUS, base_level=level)
+        self.admin.give_items_to_player(player_id, Saddles.STEGO_SADDLE, quality=quality)
 
     def sniper_set(self, player_id, quality=0):
         sniper = Weapons.FABRICATED_SNIPER_RIFLE
         ammo = Ammunition.ADVANCED_SNIPER_BULLET
-        self.give_items_to_player(player_id, [ammo], quantity=100)
-        self.give_items_to_player(player_id, [sniper], quality=quality)
+        self.admin.give_items_to_player(player_id, [ammo], quantity=100)
+        self.admin.give_items_to_player(player_id, [sniper], quality=quality)
 
     def compound_set(self, player_id, quality=0):
         bow = Weapons.COMPOUND_BOW
         ammo = Ammunition.METAL_ARROW
         flame = Ammunition.FLAME_ARROW
-        self.give_items_to_player(player_id, [ammo, flame], quantity=100)
-        self.give_items_to_player(player_id, [bow], quality=quality)
+        self.admin.give_items_to_player(player_id, [ammo, flame], quantity=100)
+        self.admin.give_items_to_player(player_id, [bow], quality=quality)
 
     def rifle_set(self, player_id, quality=0):
         rifle = Weapons.LONGNECK_RIFLE
         ammo = Ammunition.SIMPLE_RIFLE_AMMO
         tranq = Ammunition.SHOCKING_TRANQUILIZER_DART
-        self.give_items_to_player(player_id, [ammo, tranq], quantity=100)
-        self.give_items_to_player(player_id, [rifle], quality=quality)
+        self.admin.give_items_to_player(player_id, [ammo, tranq], quantity=100)
+        self.admin.give_items_to_player(player_id, [rifle], quality=quality)
 
     def hiking_set(self, player_id, quality=0):
         bow = Weapons.CROSSBOW
         grap = Ammunition.GRAPPLING_HOOK
         pick = Weapons.CLIMBING_PICK
         para = Armour.PARACHUTE
         glow = Weapons.GLOW_STICK
-        self.give_items_to_player(player_id, [pick], quantity=3)
-        self.give_items_to_player(player_id, [glow], quantity=5)
-        self.give_items_to_player(player_id, [grap, para], quantity=50)
-        self.give_items_to_player(player_id, [bow], quality=quality)
+        self.admin.give_items_to_player(player_id, [pick], quantity=3)
+        self.admin.give_items_to_player(player_id, [glow], quantity=5)
+        self.admin.give_items_to_player(player_id, [grap, para], quantity=50)
+        self.admin.give_items_to_player(player_id, [bow], quality=quality)
 
     def trap_set(self, player_id, quality=0):
         bow = Weapons.HARPOON_LAUNCHER
         net = Ammunition.NET_PROJECTILE
         trap = Weapons.BEAR_TRAP
         bear = Weapons.LARGE_BEAR_TRAP
         narc = Weapons.TRIPWIRE_NARCOTIC_TRAP
         bomb = Weapons.IMPROVISED_EXPLOSIVE_DEVICE
-        self.give_items_to_player(player_id, [trap, bear, narc, bomb], quantity=3)
-        self.give_items_to_player(player_id, [net], quantity=10)
-        self.give_items_to_player(player_id, [bow], quality=quality)
+        self.admin.give_items_to_player(player_id, [trap, bear, narc, bomb], quantity=3)
+        self.admin.give_items_to_player(player_id, [net], quantity=10)
+        self.admin.give_items_to_player(player_id, [bow], quality=quality)
 
     def c4_set(self, player_id):
         detonator = Weapons.C4_REMOTE_DETONATOR
         ammo = Ammunition.C4_CHARGE
-        self.give_items_to_player(player_id, [ammo], quantity=20)
-        self.give_items_to_player(player_id, [detonator])
+        self.admin.give_items_to_player(player_id, [ammo], quantity=20)
+        self.admin.give_items_to_player(player_id, [detonator])
 
     def flame_arrow_set(self, player_id, quality=0):
         crossbow = Weapons.CROSSBOW
         ammo = Ammunition.FLAME_ARROW
-        self.give_items_to_player(player_id, [ammo], quantity=100)
-        self.give_items_to_player(player_id, [crossbow], quality=quality)
+        self.admin.give_items_to_player(player_id, [ammo], quantity=100)
+        self.admin.give_items_to_player(player_id, [crossbow], quality=quality)
 
     def electrical_set(self, player_id, quantity=1):
         generator = Structures.ELECTRICAL_GENERATOR
         outlet = Structures.ELECTRICAL_OUTLET
         wires = [Structures.STRAIGHT_ELECTRICAL_CABLE,
                  Structures.VERTICAL_ELECTRICAL_CABLE,
                  Structures.ELECTRICAL_CABLE_INTERSECTION,
                  Structures.INCLINED_ELECTRICAL_CABLE]
         gas = Resources.GASOLINE
-        self.give_items_to_player(player_id, [gas] * quantity, quantity=50)
-        self.give_items_to_player(player_id, [generator], quantity=quantity)
-        self.give_items_to_player(player_id, wires + [outlet], quantity=quantity * 5)
+        self.admin.give_items_to_player(player_id, [gas] * quantity, quantity=50)
+        self.admin.give_items_to_player(player_id, [generator], quantity=quantity)
+        self.admin.give_items_to_player(player_id, wires + [outlet], quantity=quantity * 5)
 
     def crafting_set(self, player_id, quality=4, tek=False):
         smithy = Structures.SMITHY
         fabricator = Structures.FABRICATOR
         indiforge = Structures.INDUSTRIAL_FORGE
         chembench = Structures.CHEMISTRY_BENCH
         replicator = Structures.TEK_REPLICATOR
         gas = Resources.GASOLINE
-        self.give_items_to_player(player_id, [smithy, fabricator, indiforge, chembench][:quality])
-        self.give_item_to_player(player_id, gas, quantity=50)
+        self.admin.give_items_to_player(player_id, [smithy, fabricator, indiforge, chembench][:quality])
+        self.admin.give_item_to_player(player_id, gas, quantity=50)
         if tek:
-            self.give_items_to_player(player_id, replicator)
+            self.admin.give_items_to_player(player_id, replicator)
 
     def storage_set(self, player_id, quantity=1):
         wood = Structures.STORAGE_BOX
         vault = Structures.VAULT
         fridge = Structures.REFRIGERATOR
         cryofridge = Structures.CRYOFRIDGE
-        self.give_items_to_player(player_id, [wood, vault, fridge, cryofridge], quantity=quantity)
+        self.admin.give_items_to_player(player_id, [wood, vault, fridge, cryofridge], quantity=quantity)
 
     def defense_set(self, player_id, quantity, quality=1):
         auto = Structures.AUTO_TURRET
         heavy = Structures.HEAVY_AUTO_TURRET
         ammo = Ammunition.ADVANCED_RIFLE_BULLET
         battery = Tools.BATTERY
         if quality == 1:
-            self.give_items_to_player(player_id, [heavy, battery], quantity=quantity)
+            self.admin.give_items_to_player(player_id, [heavy, battery], quantity=quantity)
         else:
-            self.give_items_to_player(player_id, [auto, battery], quantity=quantity)
-        self.give_items_to_player(player_id, [ammo], quantity=200)
+            self.admin.give_items_to_player(player_id, [auto, battery], quantity=quantity)
+        self.admin.give_items_to_player(player_id, [ammo], quantity=200)
 
     def base_set(self, player_id, quantity=10):
         foundation = Structures.METAL_FOUNDATION
         wall = Structures.METAL_WALL
         ceiling = Structures.METAL_CEILING
         pillar = Structures.METAL_PILLAR
         doors = [Structures.METAL_DOUBLE_DOORFRAME, Structures.METAL_DOUBLE_DOOR]
-        self.give_items_to_player(player_id, doors, quantity=math.ceil(quantity / 10))
-        self.give_items_to_player(player_id, [pillar, foundation, wall, ceiling], quantity=quantity)
+        self.admin.give_items_to_player(player_id, doors, quantity=math.ceil(quantity / 10))
+        self.admin.give_items_to_player(player_id, [pillar, foundation, wall, ceiling], quantity=quantity)
 
     def fob_set(self, player_id, quantity=1):
         self.base_set(player_id, quantity=10 * quantity)
         self.electrical_set(player_id, quantity=quantity)
         self.defense_set(player_id, quantity=quantity * 3)
-        self.give_items_to_player(player_id, [Structures.GIANT_METAL_HATCHFRAME], quantity=quantity * 2)
-        self.give_items_to_player(player_id, [Structures.SIMPLE_BED], quantity=quantity * 4)
-        self.give_items_to_player(player_id, [Structures.VAULT], quantity=quantity)
+        self.admin.give_items_to_player(player_id, [Structures.GIANT_METAL_HATCHFRAME], quantity=quantity * 2)
+        self.admin.give_items_to_player(player_id, [Structures.SIMPLE_BED], quantity=quantity * 4)
+        self.admin.give_items_to_player(player_id, [Structures.VAULT], quantity=quantity)
 
     def resource_set(self, player_id, stacks=1, omit=[]):
         resources = [(Resources.METAL, 500),
                      (Resources.OBSIDIAN, 50),
                      (Resources.POLYMER, 50),
                      (Resources.HIDE, 300),
                      (Resources.OIL, 50),
@@ -203,19 +207,8 @@
                      (Resources.THATCH, 1000),
                      (Resources.FLINT, 1000),
                      (Resources.CHARCOAL, 500)]
         for resc in resources:
             blueprint, count = resc
             if blueprint not in omit:
                 for i in range(stacks):
-                    self.give_item_to_player(player_id, blueprint, quantity=count)
-
-    def __eq__(self, other):
-        return self.__dict__ == other.__dict__
-
-    def __repr__(self):
-        items = []
-        for k, v in self.__dict__.items():
-            if k and k[0] != "_":
-                items.append(f"\033[34m{k}\033[90m=\033[0m{repr(v)}\033[0m")
-        args = ', '.join(items)
-        return f'<\033[96m{type(self).__name__}\033[0m({args})>\033[0m'
+                    self.admin.give_item_to_player(player_id, blueprint, quantity=count)
```

### Comparing `arklibrary-0.0.9/src/arklibrary/admin/commands.py` & `arklibrary-1.0.1/src/arklibrary/admin/admin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,486 +1,492 @@
-from arklibrary.blueprints import *
+from arklibrary.blueprints import Spectator, PlayerManagement, CreativeMode, ServerManagement
+from arklibrary.blueprints import ItemManagement, DinoManagement, Teleportation, Map, TribeManagement
+from pathlib import Path
+import json
 
 
-class Commands:
-    def __init__(self):
+class Admin:
+    def __init__(self, driver: 'Driver' = None, password='password', player_id=None):
         # ctrl-x to clear console
         # ctrl-c to copy console
+        self.__password = password
+        self.__my_player_id = player_id
+        self.driver = driver
         self.command_list = []
+        self.cache = {'default': player_id}
 
-    def command(self, code):
-        #Command(map=self.map_name, admin_player_id=self.player_id, code=code)
-        pass
-
-    def player_coords(self, player_id='default'):
-        #self.copy_coords()
-        # this next line should be a listener running in the background
-        #clip = self.driver.app.get_from_clipboard()
-        #self.cache[player_id] = [float(c) for c in clip.split()]
-        # end of listener running in the background
-        pass
-
-    # def return_player(self, player_id='default'):
-    #     # wait until the listener on player_coords has finished copying
-    #     if player_id != 'default' and player_id in self.cache:
-    #         self.teleport_exact(self.cache[player_id])
-    #         self.teleport_player_id_to_me(player_id)
-    #     self.teleport_exact(self.cache['default'])
-
-    def execute(self):
-        # all_new = Command.all_new(self.player_id, self.map_name)
-        # if len(all_new) > 0:
-        #     command_list = [com.code for com in all_new]
-        #     self.driver.write_console(*command_list)
-        #     for command in all_new:
-        #         command.make_executed()
-        pass
+    def execute(self, *commands):
+        if len(self.command_list) > 0:
+            self.driver.write_console(*self.command_list, *commands)
+            self.command_list.clear()
+
+    def enable_admin(self):
+        self.enable_cheats(self.__password)
+        self.gcm()
+        self.enemy_ignores_me()
+        self.execute()
+        return self
+
+    def enable_cheats(self, password):
+        self.command_list.append(CreativeMode.ENABLE_CHEATS.format(password))
+        return self
 
     def gcm(self):
-        self.command(CreativeMode.GIVE_CREATIVE_MODE)
+        self.command_list.append(CreativeMode.GIVE_CREATIVE_MODE)
+        return self
+
+    def god_mode(self):
+        self.command_list.append(PlayerManagement.GOD)
+        return self
+
+    def clear_tutorials(self):
+        self.command_list.append(PlayerManagement.CLEAR_TUTORIALS)
+        return self
+
+    def leave_me_alone(self):
+        self.command_list.append(PlayerManagement.LEAVE_ME_ALONE)
+        return self
+
+    def enemy_ignores_me(self, condition=True):
+        """ Enemy creatures ignore me """
+        condition = "true" if condition else "false"
+        self.command_list.append(PlayerManagement.ENEMY_INVISIBLE.format(condition))
+        return self
 
+    def ghost(self):
+        """ Allows to go through walls """
+        self.command_list.append(PlayerManagement.GHOST)
+        self.enemy_ignores_me()
         return self
 
     def enable_spectator(self):
         """ Once you enter the spectator state your body will disapear and your inventory items
         will be erased as well. If you leave the game and rejoin it will carry on where you left
         off, thus using the command "stopspectating" is highly recommended. The latter will
         show the respawn map. """
-        self.command(Spectator.ENABLE_SPECTATOR)
+        self.command_list.append(Spectator.ENABLE_SPECTATOR)
         return self
 
     def stop_spectating(self):
         """ Stops spectating """
-        self.command(Spectator.STOP_SPECTATING)
+        self.command_list.append(Spectator.STOP_SPECTATING)
         return self
 
-    def clear_player_inventory(self, player_id, inventory=True, slot_items=False, equipment=False):
-        """ Clears player's inventory, equipped items, and/or slot items.
-            Ex. cheat ClearPlayerInventory <playerID> <inventory?> <slotitems?> <equippeditems?>
-                cheat ClearPlayerInventory 4213211323 1 1 1 1
-        """
-        # TODO: Need to fix numbers (e.g. clear_player_inventory(id, True, False, False) -> clear_player_inventory id 1 1 1
-        # Should be returning 1 0 0 at the end instead of 1 1 1
-        inventory = "1" if inventory else "0"
-        slot_items = "1" if inventory else "0"
-        equipment = "1" if inventory else "0"
-
-        self.command(PlayerManagement.CLEAR_PLAYER_INVENTORY.format(player_id, inventory, slot_items, equipment))
-
     def message_server(self, message):
         """ Writes to chat as a server message to all players"""
-        self.command(ServerManagement.SERVER_CHAT.format(message))
+        self.command_list.append(ServerManagement.SERVER_CHAT.format(message))
+        return self
 
+    def broadcast(self, message):
+        """ Sends a message to the whole server using the banner """
+        self.command_list.append(ServerManagement.BROADCAST.format(str(message)))
         return self
 
-    def rename_player(self, current_name, new_name):
-        self.command(PlayerManagement.RENAME_PLAYER.format(current_name, new_name))
+    def give_item_to_player(self, player_id, blueprint_path, quantity=1, quality=0, force_blueprint=False):
+        """ Adds the specified item (or its blueprint) to the player's inventory in the specified quantity
+            Ex. cheat GiveItemToPlayer 696509819 "Blueprint'/Game/PrimalEarth/CoreBlueprints/Weapons/PrimalItemAmmo_AdvancedRifleBullet.PrimalItemAmmo_AdvancedRifleBullet'" 200 1 0
+        """
+        force_blueprint = 1 if force_blueprint else 0
+        self.command_list.append(ItemManagement.GIVE_ITEM_TO_PLAYER.format(
+            player_id, blueprint_path, quantity, quality, force_blueprint))
+        return self
 
+    def give_items_to_player(self, player_id, blueprint_paths, quantity=1, quality=0, force_blueprint=False):
+        """ Adds the specified item (or its blueprint) to the player's inventory in the specified quantity
+            Ex. cheat GiveItemToPlayer 696509819 "Blueprint'/Game/PrimalEarth/CoreBlueprints/Weapons/PrimalItemAmmo_AdvancedRifleBullet.PrimalItemAmmo_AdvancedRifleBullet'" 200 1 0
+            NOTE: Quantity above the stack limit isn't given
+        """
+        force_blueprint = 1 if force_blueprint else 0
+        for path in blueprint_paths:
+            self.command_list.append(ItemManagement.GIVE_ITEM_TO_PLAYER.format(
+                player_id, path, quantity, quality, force_blueprint))
         return self
 
-    def rename_tribe(self, current_name, new_name):
-        self.command(TribeManagement.RENAME_TRIBE.format(current_name, new_name))
+    def spawn_exact_dino(self, dino_blueprint_path="", saddle_blueprint_path="", saddle_quality=0,
+                         base_level=150, extra_levels=0, base_stats="0,0,0,0,0,0,1,1",
+                         added_stats="0,0,0,0,0,0,0,0", dino_name="", cloned=0, neutered=0,
+                         tamed_on="", uploaded_from="", imprinter_name="", imprinter_player_id=0,
+                         imprint_quality=0, colors="0,0,0,0,0,0", dino_id=0, exp=0,
+                         spawn_distance=0, y_offset=0, z_offset=0):
+        """
+        DinoBlueprintPath:	    String,	Blueprint path
+        SaddleBlueprintPath:	String,	Blueprint path
+        To spawn the creature without saddle pass an empty string ("")
+
+        SaddleQuality:	        float,	Quality of the equipped saddle
+        BaseLevel:	       Integer[32],	Level of the spawned Dino.
+        If the level is not the sum of BaseStats + 1, the creature stats may be broken.
+
+        ExtraLevels:	   Integer[32],	Sum of the domesticated levels
+        If the value is not the sum of AddedStats, the creature stats may be broken.
+
+        BaseStats:	            String,	Comma separated string with the base levels
+        The order is health, stamina, oxygen, food, weight, melee damage, movement speed, crafting skill
+        The set levels will only be visible after putting the creature in and out of a crypod.
+        Syntax example: "0,0,0,0,0,0,0,0"
+
+        AddedStats:	            String,	Comma separated string with the domesticated levels
+        The order is health, stamina, oxygen, food, weight, melee damage, movement speed, crafting skill
+        The set levels will only be visible after putting the creature in and out of a crypod.
+        Syntax example: "0,0,0,0,0,0,0,0"
+
+        DinoName:	            String
+        Cloned:	            Integer[8]
+        Neutered:	        Integer[8]
+        TamedOn:	        String
+        UploadedFrom:	        String
+        ImprinterName:	        String,	If left empty, there will be no imprint
+        ImprinterPlayerID:	Integer[32]
+        ImprintQuality:	        float
+
+        Colors:     	        String,	Comma separated string with the color ids
+        Syntax example: "0,0,0,0,0,0"
+        The colors will appear if the creature was put in and out of a cryopod.
+        If an empty string ("") is passed, the colors will be randomly taken from the natural occuring colors of that species.
+
+        DinoID:	           Integer[64],	If 0 is passed, the game will roll the id.
+        Exp:	           Integer[64]
+        spawnDistance:	        float
+        YOffset:	            float
+        ZOffset:	            float
+        """
+        format = DinoManagement.SPAWN_EXACT_DINO
+        self.command_list.append(format.format(dino_blueprint_path, saddle_blueprint_path, saddle_quality, base_level,
+                                   extra_levels, base_stats, added_stats, dino_name, cloned, neutered,
+                                   tamed_on,
+                                   uploaded_from, imprinter_name, imprinter_player_id, imprint_quality,
+                                   colors,
+                                   dino_id, exp, spawn_distance, y_offset, z_offset))
+        return self
 
+    def spawn_dino(self, blueprint_path, tamed=False, level=0):
+        """
+        Spawns a dino
+        :param name_part:	String	significant part of a creature's Entity ID (without _C)
+        :param tamed: 	    Boolean	true or 1: tamed, false or 0: wild
+        :param level: 	    float	Give creature a specific level, set to 0 for random
+
+        Ex. spawn_dino("dodo", True, 150)
+        """
+        tamed = "true" if tamed else "false"
+        if 'bionics' in blueprint_path:
+            name = blueprint_path.split("/")[-1].split('.')[0]
+        else:
+            name = blueprint_path.split("/")[4]
+        self.command_list.append(DinoManagement.SDF.format(name, tamed, level))
         return self
 
-    def show_admin_manager(self):
-        """ shows a list of all the players with their player id's """
-        self.command(ServerManagement.SHOW_MY_ADMIN_MANAGER)
+    def remove_cryosickness(self):
+        self.command_list.append(DinoManagement.CLEAR_CRYO_SICKNESS)
+        return self
 
+    def set_target_dino_color(self, color_region: int, color_id: int):
+        """
+        Change a dino's color
+        :param color_region:    Integer[32]	Color Region
+        :param color_id:        Integer[32]	Color ID.
+        """
+        self.command_list.append(DinoManagement.SET_TARGET_DINO_COLOR.format(color_region, color_id))
         return self
 
-    def ban_player(self, player_id):
-        """ Bans a player """
-        self.command(ServerManagement.BAN_PLAYER.format(player_id))
+    def copy_coords(self):
+        """ Copies your current coordinates and rotation to clipboard in the form x,y,z Yaw pitch """
+        self.command_list.append(Map.COPY_COORDS_TO_CLIPBOARD)
+        return self
 
+    def teleport_exact(self, x, y, z, yaw, pitch):
+        """ Pitch is looking down or up (-80.00 ... 87.00), and 0.00 is leveled"""
+        """ Yaw is rotation left to right (-80.00 north... 0.00 east.. 80.00 south... 179.99 west)"""
+        self.command_list.append(Teleportation.SPI.format(int(x), int(y), int(z), float(yaw), float(pitch)))
         return self
 
-    def unban_player(self, player_id):
-        """ Unbans player """
-        self.command(ServerManagement.UNBAN_PLAYER.format(player_id))
+    def teleport_gps_coords(self, lattitude, longitude, altitude):
+        """ Moves player to GPS coordinates """
+        self.command_list.append(Teleportation.TP_COORDS.format(lattitude, longitude, altitude))
+        return self
 
+    def teleport_player_id_to_me(self, player_id):
+        """
+        Teleport player by player id to me
+        :param id: int, player's id
+        """
+        self.command_list.append(Teleportation.TELEPORT_PLAYER_ID_TO_ME.format(player_id))
         return self
 
-    def disable_spectator(self):
-        self.command(Spectator.STOP_SPECTATING)
+    def teleport_to_playerid(self, player_id):
+        """ Teleport to another player by their id """
 
+        self.command_list.append(Teleportation.TELEPORT_TO_PLAYER.format(player_id))
         return self
 
-    def teleport(self, command):
-        self.command(Teleportation.TP.format(command))
+    def paste_teleport(self):
+        """ After copying coordinates pastes and teleport here """
+        copied = self.driver.app.get_from_clipboard()
+        x, y, z, yaw, pitch = copied.split()
+        self.command_list.append(Teleportation.SPI.format(int(x), int(y), int(z), float(yaw), float(pitch)))
+        return self
 
+    def spawn_beacon(self, blueprint_path):
+        self.command_list.append(Map.SUMMON.format(blueprint_path))
         return self
 
     def teleport_green_obelisk(self):
         """ Teleport myself to green obelisk """
 
-        self.command(Teleportation.TP.format("green"))
+        self.command_list.append(Teleportation.TP.format("green"))
         return self
 
     def teleport_blue_obelisk(self):
         """ Teleport myself to blue obelisk """
 
-        self.command(Teleportation.TP.format("blue"))
+        self.command_list.append(Teleportation.TP.format("blue"))
         return self
 
     def teleport_red_obelisk(self):
         """ Teleport myself to red obelisk """
 
-        self.command(Teleportation.TP.format("red"))
+        self.command_list.append(Teleportation.TP.format("red"))
         return self
 
-    def teleport_king_titan_terminal(self):
-        """ Teleport me to King Titan Terminal in Extinction"""
+    def teleport_xyz(self, x, y, z):
+        """ Moves player to x,y,z game coordinates """
+        self.command_list.append(Teleportation.SET_PLAYER_POS.format(x, y, z))
+        return self
 
-        self.command(Teleportation.TP.format("king"))
+    def teleport_target_xyz(self, x, y, z):
+        """ Moves player or dino to game coordinates """
+        self.command_list.append(Teleportation.MOVE_TARGET_TO.format(x, y, z))
         return self
 
-    def teleport_desert_titan_terminal(self):
-        """ Teleport me to Desert Titan Terminal in Extinction"""
+    def save_current_coordinates(self, map, name):
+        """ Stores the coordinates into file with a name
+        :param name: str, name for the coordinates
+        """
+        data = {"center": {}, "gen1": {}, "gen2": {}, "island": {},
+                "scortched": {}, "ragnarok": {}, "extinction": {}, "aberration": {}}
+        if map not in data:
+            raise NotImplementedError("'{}' isn't part of the map list: {}".format(map, data.keys()))
+        self.copy_coords()
+        coords = [float(val) for val in self.driver.get_from_clipboard().split()]
+        file_path = Path.cwd() / Path('../logs/saved_coordinates.json')
+        if file_path.exists():
+            with open(file_path, 'r') as r:
+                data = json.load(r)
+
+        cc = {"x": coords[0], "y": coords[1], "z": coords[2], "yaw": coords[3], "pitch": coords[4]}
+        data[map][name] = cc
+        with open(file_path, "w") as w:
+            json.dump(data, w)
 
-        self.command(Teleportation.TP.format("red"))
+    def give_tek_engrams_to(self, player_id, engram=None):
+        self.command_list.append(f"cheat GiveTekEngramsTo {player_id} tek")
         return self
 
-    def teleport_forest_titan_terminal(self):
-        """ Teleport me to Forest Titan Terminal in Extinction"""
+    def hide_admin_icon(self, condition=True):
+        """ Hides admin icon when writing into chat """
+        condition = "true" if condition else "false"
+        self.command_list.append("cheat SetAdminIcon {}".format(condition))
+        return self
 
-        self.command(Teleportation.TP.format("green"))
+    def tranquilize_target(self):
+        """ Tranquilize target in crosshairs """
+        self.command_list.append("cheat SetMyTargetSleeping 1")
         return self
 
-    def teleport_ice_titan_terminal(self):
-        """ Teleport me to Ice Titan Terminal in Extinction"""
+    def wake_up_target(self):
+        """ Removes tranquilizing effects of target in crosshairs """
+        self.command_list.append("cheat SetMyTargetSleeping 0")
+        return self
+
+    def add_hexagons(self, amount):
+        """ Give myself a number of hexagons """
+        self.command_list.append("cheat AddHexagons {}".format(amount))
+        return self
 
-        self.command(Teleportation.TP.format("blue"))
+    def tame(self):
+        """ Tames the targeted dino in my crosshairs """
+        self.command_list.append("cheat DoTame")
         return self
 
-    def teleport_to_playerid(self, player_id):
-        """ Teleport to another player by their id """
 
-        self.command(Teleportation.TELEPORT_TO_PLAYER.format(player_id))
+    def clear_player_inventory(self, player_id, inventory=True, slot_items=False, equipment=False):
+        """ Clears player's inventory, equipped items, and/or slot items.
+            Ex. cheat ClearPlayerInventory <playerID> <inventory?> <slotitems?> <equippeditems?>
+                cheat ClearPlayerInventory 4213211323 1 1 1 1
+        """
+        # TODO: Need to fix numbers (e.g. clear_player_inventory(id, True, False, False) -> clear_player_inventory id 1 1 1
+        # Should be returning 1 0 0 at the end instead of 1 1 1
+        inventory = "1" if inventory else "0"
+        slot_items = "1" if inventory else "0"
+        equipment = "1" if inventory else "0"
+
+        self.command_list.append(PlayerManagement.CLEAR_PLAYER_INVENTORY.format(player_id, inventory, slot_items, equipment))
+
+    def rename_player(self, current_name, new_name):
+        self.command_list.append(PlayerManagement.RENAME_PLAYER.format(current_name, new_name))
         return self
 
-    def teleport_to_player_name(self, name):
-        """ Teleport to another player by their name """
+    def rename_tribe(self, current_name, new_name):
+        self.command_list.append(TribeManagement.RENAME_TRIBE.format(current_name, new_name))
+        return self
 
-        self.command(Teleportation.TELEPORT_TO_PLAYER_NAME.format(name))
+    def show_admin_manager(self):
+        """ shows a list of all the players with their player id's """
+        self.command_list.append(ServerManagement.SHOW_MY_ADMIN_MANAGER)
         return self
 
-    def teleport_player_id_to_me(self, player_id):
-        """
-        Teleport player by player id to me
-        :param id: int, player's id
-        """
-        self.command(Teleportation.TELEPORT_PLAYER_ID_TO_ME.format(player_id))
+    def ban_player(self, player_id):
+        """ Bans a player """
+        self.command_list.append(ServerManagement.BAN_PLAYER.format(player_id))
         return self
 
-    def teleport_player_name_to_me(self, name):
-        """
-        Teleport player by name to me.
-        :param name: str, player's ingame name
-        """
-        self.command(Teleportation.TELEPORT_PLAYER_NAME_TO_ME.format(name))
+    def unban_player(self, player_id):
+        """ Unbans player """
+        self.command_list.append(ServerManagement.UNBAN_PLAYER.format(player_id))
         return self
 
-    def teleport_gps_coords(self, lattitude, longitude, altitude):
-        """ Moves player to GPS coordinates """
-        self.command(Teleportation.TP_COORDS.format(lattitude, longitude, altitude))
+    def disable_spectator(self):
+        self.command_list.append(Spectator.STOP_SPECTATING)
         return self
 
-    def teleport_xyz(self, x, y, z):
-        """ Moves player to x,y,z game coordinates """
-        self.command(Teleportation.SET_PLAYER_POS.format(x, y, z))
+    def teleport(self, command):
+        self.command_list.append(Teleportation.TP.format(command))
         return self
 
-    def teleport_target_xyz(self, x, y, z):
-        """ Moves player or dino to game coordinates """
-        self.command(Teleportation.MOVE_TARGET_TO.format(x, y, z))
+    def teleport_king_titan_terminal(self):
+        """ Teleport me to King Titan Terminal in Extinction"""
+
+        self.command_list.append(Teleportation.TP.format("king"))
+        return self
+
+    def teleport_desert_titan_terminal(self):
+        """ Teleport me to Desert Titan Terminal in Extinction"""
+        self.command_list.append(Teleportation.TP.format("red"))
+        return self
+
+    def teleport_forest_titan_terminal(self):
+        """ Teleport me to Forest Titan Terminal in Extinction"""
+        self.command_list.append(Teleportation.TP.format("green"))
+        return self
+
+    def teleport_ice_titan_terminal(self):
+        """ Teleport me to Ice Titan Terminal in Extinction"""
+        self.command_list.append(Teleportation.TP.format("blue"))
+        return self
+
+    def teleport_to_player_name(self, name):
+        """ Teleport to another player by their name """
+        self.command_list.append(Teleportation.TELEPORT_TO_PLAYER_NAME.format(name))
+        return self
+
+    def teleport_player_name_to_me(self, name):
+        """
+        Teleport player by name to me.
+        :param name: str, player's ingame name
+        """
+        self.command_list.append(Teleportation.TELEPORT_PLAYER_NAME_TO_ME.format(name))
         return self
 
     def kill_target(self):
         """ Kills exactly whoever is in my crosshairs """
-        self.command(DinoManagement.DESTROY_MY_TARGET)
+        self.command_list.append(DinoManagement.DESTROY_MY_TARGET)
         return self
 
     def destroy_tribes_dinos(self):
         """ Kills all dinos in my crosshairs in its tribe """
-        self.command(DinoManagement.DESTROY_TRIBE_DINOS)
+        self.command_list.append(DinoManagement.DESTROY_TRIBE_DINOS)
         return self
 
     def destroy_tribes_dinos_by_id(self, tribe_id):
         """ Kills all tribe's dinos """
-        self.command(TribeManagement.DESTROY_TRIBE_ID.format(tribe_id))
+        self.command_list.append(TribeManagement.DESTROY_TRIBE_ID.format(tribe_id))
         return self
 
     def destroy_players_by_tribeid(self, tribe_id):
         """ Destroys all players in a tribe by tribe id """
-        self.command(TribeManagement.DESTROY_TRIBE_ID_PLAYERS.format(tribe_id))
+        self.command_list.append(TribeManagement.DESTROY_TRIBE_ID_PLAYERS.format(tribe_id))
         return self
 
     def destroy_tribe_by_id(self, tribe_id):
         """ Destroy a tribe by their id """
-        self.command(TribeManagement.DESTROY_TRIBE_ID.format(tribe_id))
+        self.command_list.append(TribeManagement.DESTROY_TRIBE_ID.format(tribe_id))
         return self
 
     def destroy_structures_by_tribeid(self, tribe_id):
         """ Destroys all structures in a tribe by tribe id """
-        self.command(TribeManagement.DESTROY_TRIBE_ID_STRUCTURES.format(tribe_id))
+        self.command_list.append(TribeManagement.DESTROY_TRIBE_ID_STRUCTURES.format(tribe_id))
         return self
 
     def destroy_tribe_structures(self):
         """ destroys target tribe's structures """
-        self.command(TribeManagement.DESTROY_TRIBE_STRUCTURES)
+        self.command_list.append(TribeManagement.DESTROY_TRIBE_STRUCTURES)
         return self
 
     def destroy_wild_dinos(self):
         """ Destroys all untamed dinos to help with respawns """
-        self.command(DinoManagement.DESTROY_WILD_DINOS)
+        self.command_list.append(DinoManagement.DESTROY_WILD_DINOS)
         return self
 
     def force_player_to_join_target_tribe(self, player_id):
         """ Force a player to join a tribe i'm targeting with my crosshairs"""
-        self.command(TribeManagement.FORCE_PLAYER_TO_JOIN_TARGET_TRIBE.format(player_id))
+        self.command_list.append(TribeManagement.FORCE_PLAYER_TO_JOIN_TARGET_TRIBE.format(player_id))
         return self
 
     def force_myself_into_target_tribe(self):
         """ Force myself into a tribe I'm targeting with my crosshairs """
-        self.command(TribeManagement.FORCE_JOIN_TRIBE)
+        self.command_list.append(TribeManagement.FORCE_JOIN_TRIBE)
         return self
 
     def force_myself_tribe_admin(self):
         """ Force myself as tribe admin """
-        self.command(TribeManagement.FORCE_TRIBE_ADMIN)
+        self.command_list.append(TribeManagement.FORCE_TRIBE_ADMIN)
         return self
 
     def force_myself_tribe_owner(self):
         """ Force myself as tribe owner """
-        self.command(TribeManagement.FORCE_TRIBE_FOUNDER)
+        self.command_list.append(TribeManagement.FORCE_TRIBE_FOUNDER)
         return self
 
     def give_experience_to_player(self, player_id, amount, from_tribe_share=False, prevent_sharing_with_tribe=True):
         """ Give a player experience points """
         from_tribe_share = 1 if from_tribe_share else 0
-        self.command(
+        self.command_list.append(
             PlayerManagement.GIVE_EXP_TO_PLAYER.format(player_id, amount, from_tribe_share,
                                                        prevent_sharing_with_tribe))
         return self
 
     def add_experience_on_mounted_dino(self, amount, from_tribe_share=False, prevent_sharing_with_tribe=True):
         """ Give experience to a dino you're mounted on """
         from_tribe_share = 1 if from_tribe_share else 0
         prevent_sharing_with_tribe = 1 if prevent_sharing_with_tribe else 0
-        self.command(
+        self.command_list.append(
             PlayerManagement.ADD_EXPERIENCE.format(amount, from_tribe_share, prevent_sharing_with_tribe))
         return self
 
-    def enemy_ignores_me(self, condition=True):
-        """ Enemy creatures ignore me """
-        condition = "true" if condition else "false"
-        self.command(PlayerManagement.ENEMY_INVISIBLE.format(condition))
-        return self
-
-    def ghost(self):
-        """ Allows to go through walls """
-        self.command(PlayerManagement.GHOST)
-        self.enemy_ignores_me()
-        return self
-
-    def give_item_to_player(self, player_id, blueprint_path, quantity=1, quality=0, force_blueprint=False):
-        """ Adds the specified item (or its blueprint) to the player's inventory in the specified quantity
-            Ex. cheat GiveItemToPlayer 696509819 "Blueprint'/Game/PrimalEarth/CoreBlueprints/Weapons/PrimalItemAmmo_AdvancedRifleBullet.PrimalItemAmmo_AdvancedRifleBullet'" 200 1 0
-        """
-        force_blueprint = 1 if force_blueprint else 0
-        self.command(ItemManagement.GIVE_ITEM_TO_PLAYER.format(
-            player_id, blueprint_path, quantity, quality, force_blueprint))
-        return self
-
-    def give_items_to_player(self, player_id, blueprint_paths, quantity=1, quality=0, force_blueprint=False):
-        """ Adds the specified item (or its blueprint) to the player's inventory in the specified quantity
-            Ex. cheat GiveItemToPlayer 696509819 "Blueprint'/Game/PrimalEarth/CoreBlueprints/Weapons/PrimalItemAmmo_AdvancedRifleBullet.PrimalItemAmmo_AdvancedRifleBullet'" 200 1 0
-            NOTE: Quantity above the stack limit isn't given
-        """
-        force_blueprint = 1 if force_blueprint else 0
-        for path in blueprint_paths:
-            self.command(ItemManagement.GIVE_ITEM_TO_PLAYER.format(
-                player_id, path, quantity, quality, force_blueprint))
-        return self
-
-    def hide_admin_icon(self, condition=True):
-        """ Hides admin icon when writing into chat """
-        condition = "true" if condition else "false"
-        self.command("cheat SetAdminIcon {}".format(condition))
-        return self
-
-    def tranquilize_target(self):
-        """ Tranquilize target in crosshairs """
-        self.command("cheat SetMyTargetSleeping 1")
-        return self
-
-    def wake_up_target(self):
-        """ Removes tranquilizing effects of target in crosshairs """
-        self.command("cheat SetMyTargetSleeping 0")
-        return self
-
-    def add_hexagons(self, amount):
-        """ Give myself a number of hexagons """
-        self.command("cheat AddHexagons {}".format(amount))
-        return self
-
-    def tame(self):
-        """ Tames the targeted dino in my crosshairs """
-        self.command("cheat DoTame")
-        return self
-
-    def spawn_dino(self, blueprint_path, tamed=False, level=0):
-        """
-        Spawns a dino
-        :param name_part:	String	significant part of a creature's Entity ID (without _C)
-        :param tamed: 	    Boolean	true or 1: tamed, false or 0: wild
-        :param level: 	    float	Give creature a specific level, set to 0 for random
-
-        Ex. spawn_dino("dodo", True, 150)
-        """
-        tamed = "true" if tamed else "false"
-        if 'bionics' in blueprint_path:
-            name = blueprint_path.split("/")[-1].split('.')[0]
-        else:
-            name = blueprint_path.split("/")[4]
-        self.command(DinoManagement.SDF.format(name, tamed, level))
-        return self
-
-    def spawn_dinos(self, *blueprint_paths, level=0, tamed=True):
-        """
-        Spawns a dino
-        :param name_part:	String	significant part of a creature's Entity ID (without _C)
-        :param tamed: 	    Boolean	true or 1: tamed, false or 0: wild
-        :param level: 	    float	Give creature a specific level, set to 0 for random
-
-        Ex. spawn_dino("dodo", True, 150)
-        """
-        tamed = "true" if tamed else "false"
-        for path in blueprint_paths:
-            if 'bionics' in path.lower():
-                name = path.split("/")[-1].split('.')[0]
-            else:
-                name = path.split("/")[4]
-            self.command(DinoManagement.SDF.format(name, tamed, level))
-        return self
-
-    def remove_cryosickness(self):
-        self.command(DinoManagement.CLEAR_CRYO_SICKNESS)
-        return self
-
-    def spawn_exact_dino(self, dino_blueprint_path="", saddle_blueprint_path="", saddle_quality=0,
-                         base_level=150, extra_levels=0, base_stats="0,0,0,0,0,0,1,1",
-                         added_stats="0,0,0,0,0,0,0,0", dino_name="", cloned=0, neutered=0,
-                         tamed_on="", uploaded_from="", imprinter_name="", imprinter_player_id=0,
-                         imprint_quality=0, colors="0,0,0,0,0,0", dino_id=0, exp=0,
-                         spawn_distance=0, y_offset=0, z_offset=0):
-        """
-        DinoBlueprintPath:	    String,	Blueprint path
-        SaddleBlueprintPath:	String,	Blueprint path
-        To spawn the creature without saddle pass an empty string ("")
-
-        SaddleQuality:	        float,	Quality of the equipped saddle
-        BaseLevel:	       Integer[32],	Level of the spawned Dino.
-        If the level is not the sum of BaseStats + 1, the creature stats may be broken.
-
-        ExtraLevels:	   Integer[32],	Sum of the domesticated levels
-        If the value is not the sum of AddedStats, the creature stats may be broken.
-
-        BaseStats:	            String,	Comma separated string with the base levels
-        The order is health, stamina, oxygen, food, weight, melee damage, movement speed, crafting skill
-        The set levels will only be visible after putting the creature in and out of a crypod.
-        Syntax example: "0,0,0,0,0,0,0,0"
-
-        AddedStats:	            String,	Comma separated string with the domesticated levels
-        The order is health, stamina, oxygen, food, weight, melee damage, movement speed, crafting skill
-        The set levels will only be visible after putting the creature in and out of a crypod.
-        Syntax example: "0,0,0,0,0,0,0,0"
-
-        DinoName:	            String
-        Cloned:	            Integer[8]
-        Neutered:	        Integer[8]
-        TamedOn:	        String
-        UploadedFrom:	        String
-        ImprinterName:	        String,	If left empty, there will be no imprint
-        ImprinterPlayerID:	Integer[32]
-        ImprintQuality:	        float
-
-        Colors:     	        String,	Comma separated string with the color ids
-        Syntax example: "0,0,0,0,0,0"
-        The colors will appear if the creature was put in and out of a cryopod.
-        If an empty string ("") is passed, the colors will be randomly taken from the natural occuring colors of that species.
-
-        DinoID:	           Integer[64],	If 0 is passed, the game will roll the id.
-        Exp:	           Integer[64]
-        spawnDistance:	        float
-        YOffset:	            float
-        ZOffset:	            float
-        """
-        format = DinoManagement.SPAWN_EXACT_DINO
-        self.command(format.format(dino_blueprint_path, saddle_blueprint_path, saddle_quality, base_level,
-                                   extra_levels, base_stats, added_stats, dino_name, cloned, neutered,
-                                   tamed_on,
-                                   uploaded_from, imprinter_name, imprinter_player_id, imprint_quality,
-                                   colors,
-                                   dino_id, exp, spawn_distance, y_offset, z_offset))
-        return self
-
-    def set_target_dino_color(self, color_region: int, color_id: int):
-        """
-        Change a dino's color
-        :param color_region:    Integer[32]	Color Region
-        :param color_id:        Integer[32]	Color ID.
-        """
-        self.command(DinoManagement.SET_TARGET_DINO_COLOR.format(color_region, color_id))
+    def set_time_of_day(self, hour: int = 8, minute: int = 0, seconds: int = 0):
+        self.command_list.append(Map.SET_TIME_OF_DAY.format(hour, minute, seconds))
         return self
 
-    def copy_coords(self):
-        """ Copies your current coordinates and rotation to clipboard in the form x,y,z Yaw pitch """
-        self.command(Map.COPY_COORDS_TO_CLIPBOARD)
-        return self
+    def morning(self):
+        return self.set_time_of_day(hour=4, minute=30)
 
-    def teleport_exact(self, x, y, z, yaw, pitch):
-        """ Pitch is looking down or up (-80.00 ... 87.00), and 0.00 is leveled"""
-        """ Yaw is rotation left to right (-80.00 north... 0.00 east.. 80.00 south... 179.99 west)"""
-        self.command(Teleportation.SPI.format(int(x), int(y), int(z), float(yaw), float(pitch)))
-        return self
+    def daylight(self):
+        return self.set_time_of_day(hour=10)
 
-    def paste_teleport(self):
-        """ After copying coordinates pastes and teleport here """
-        copied = self.driver.app.get_from_clipboard()
-        x, y, z, yaw, pitch = copied.split()
-        self.command(Teleportation.SPI.format(int(x), int(y), int(z), float(yaw), float(pitch)))
-        return self
+    def dusk(self):
+        return self.set_time_of_day(hour=21)
 
-    def get_tribe_id_player_list(self, tribe_id):
-        """ Get a list of player id's from a tribe """
-        self.command(TribeManagement.GET_TRIBE_ID_PLAYER_LIST.format(tribe_id))
-        return self
+    def night(self):
+        return self.set_time_of_day(hour=24)
 
-    def spawn_beacon(self, blueprint_path):
-        self.command(Map.SUMMON.format(blueprint_path))
+    def __enter__(self):
         return self
 
-    def spawn_beaver_dam(self):
-        self.command(ItemManagement.SPAWN.format("BeaverDam_C"))
-        return self
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.execute()
 
-    def broadcast(self, message):
-        """ Sends a message to the whole server using the banner """
-        self.command(ServerManagement.BROADCAST.format(str(message)))
-        return self
+    def restart_application(self):
+        self.driver.app.close()
+        return Admin(password=self.__password)
 
-    def give_engram_to(self, player_id, engram=None):
-        self.command(f"cheat GiveTekEngramsTo {player_id} tek")
-        return self
 
-    def __eq__(self, other):
-        return self.__dict__ == other.__dict__
 
-    def __repr__(self):
-        items = []
-        for k, v in self.__dict__.items():
-            if k and k[0] != "_":
-                items.append(f"\033[34m{k}\033[90m=\033[0m{repr(v)}\033[0m")
-        args = ', '.join(items)
-        return f'<\033[96m{type(self).__name__}\033[0m({args})>\033[0m'
```

### Comparing `arklibrary-0.0.9/src/arklibrary/admin/run_driver.py` & `arklibrary-1.0.1/src/arklibrary/admin/run_driver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from arklibrary.admin import Admin, Bundle
+from arklibrary.admin import Admin
 from time import sleep
 
 
 def game_driver_config():
     with open("config.json", 'r') as r:
         return json.load(r)["gamedriver"]
```

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/__init__.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/__init__.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/ammunitions.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/ammunitions.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/armours.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/armours.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/artifacts.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/artifacts.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/beacons.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/beacons.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/chibis.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/chibis.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/colors.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/colors.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/commands.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     SET_ADMIN_ICON = "cheat SetAdminIcon {}"
     SHOW_IN_GAME_MENU = "cheat ShowInGameMenu"
     SHOW_DEBUG = "ShowDebug {}"
 
 
 class Map:
     SET_DAY = "cheat SetDay {}"
-    SET_TIME_OF_DAY = "cheat SetTimeOfDay {} {}"
+    SET_TIME_OF_DAY = "cheat SetTimeOfDay {}:{}:{}"
     GET_ALL_STATE = "cheat GetAllState {}"
     DESTROY_FOLIAGE = "cheat DestroyFoliage {}"
     OPEN_MAP = "cheat OpenMap {}"
     SUMMON = "cheat Summon {}"
     COPY_COORDS_TO_CLIPBOARD = "ccc"
     CE = "cheat {}"
     DCM_SET = "DCMSET {} {}"
```

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/consumables.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/consumables.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/creatures.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/creatures.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/dyes.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/dyes.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/eggs.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/eggs.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/farming.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/farming.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/recipes.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/recipes.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/resources.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/resources.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/saddles.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/saddles.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/seeds.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/seeds.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/skins.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/skins.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/structures.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/structures.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/tools.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/tools.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/trophies.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/trophies.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/blueprints/weapons.py` & `arklibrary-1.0.1/src/arklibrary/blueprints/weapons.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/data_structures/stream.py` & `arklibrary-1.0.1/src/arklibrary/data_structures/stream.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             Stream   =   0036   |   {body_length: 19, body_type: 'json'}   |    {'data': 'my data'}
             Stream   =   0038   |   {body_length: 19, body_type: 'pickle'} |    \x8\a43\x92\x213\x1
             Stream   =   0035   |   {body_length: 19, body_type: 'str'}   |     this is my data str
     """
     SIZE = 4  # is 4 decimal digits long (e.g. 4 bytes)
 
     @classmethod
-    def new(cls, stream: bytes):
+    def new(cls, stream: bytes) -> 'Stream':
         return pickle.loads(stream)
 
     def __init__(self, **kwargs):
         attrs = defaultdict(lambda: None)
         attrs.update(kwargs)
         self.from_address = attrs['from_address']
         self.to_address = attrs['to_address']
@@ -39,15 +39,15 @@
 
     def items(self):
         return self.__dict__.items()
 
     def __getitem__(self, item):
         return self.__dict__[item]
 
-    def encode(self):
+    def encode(self) -> bytes:
         return pickle.dumps(self)
 
     def __getstate__(self):
         state = self.__dict__.copy()
         state['body'] = encode(self.body)
         return state
```

### Comparing `arklibrary-0.0.9/src/arklibrary/data_structures/tri.py` & `arklibrary-1.0.1/src/arklibrary/data_structures/tri.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/events/events.py` & `arklibrary-1.0.1/src/arklibrary/events/events.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/lib/configuration.py` & `arklibrary-1.0.1/src/arklibrary/lib/configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from abc import abstractmethod
 from pathlib import Path
 import configparser
+from collections import defaultdict
 
 
 class Configuration:
-    def __init__(self, path: Path or str):
-        self.path = Path(path)
-        if not self.path.exists():
-            raise FileNotFoundError(path)
-        self.data = None
+    def __init__(self, path):
+        self.path = path and Path(path) or None
+        self.data = defaultdict(lambda: None)
 
     @abstractmethod
     def __getitem__(self, item):
         pass
 
     @abstractmethod
     def __contains__(self, item):
@@ -30,32 +29,42 @@
     def items(self):
         pass
 
     @abstractmethod
     def keys(self):
         pass
 
+    def exists(self):
+        return self.path is not None and self.path.exists()
+
 
 class Ini(Configuration):
-    def __init__(self, path=None):
-        if path is None:
-            path = Path(__file__).parent.parent / Path('config.ini')
+    def __init__(self, path: str or Path = None):
         super().__init__(path)
-        config = configparser.ConfigParser()
-        config.read(self.path)
-        self.data = self.__to_dict(config)
+        if self.path and self.path.exists():
+            config = configparser.ConfigParser()
+            config.read(self.path)
+            self.data = self.__to_dict(config)
 
     @classmethod
     def __to_dict(cls, data: dict, result=None):
         if result is None:
             result = {}
         for key, value in data.items():
             if isinstance(value, configparser.SectionProxy):
                 result[key] = cls.__to_dict(dict(value))
             else:
+                if isinstance(value, str):
+                    value = value.lower()
+                    if value == 'false':
+                        value = False
+                    elif value == 'true':
+                        value = True
+                    elif value.isnumeric():
+                        value = int(value)
                 result[key] = value
         return result
 
     @classmethod
     def __to_array(cls, data: list):
         result = []
         for item in data:
```

### Comparing `arklibrary-0.0.9/src/arklibrary/tools/ark_generic_scraper.py` & `arklibrary-1.0.1/src/arklibrary/tools/ark_generic_scraper.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/tools/ark_image_scraper.py` & `arklibrary-1.0.1/src/arklibrary/tools/ark_image_scraper.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/tools/clipboard.py` & `arklibrary-1.0.1/src/arklibrary/tools/clipboard.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/tools/config.py` & `arklibrary-1.0.1/src/arklibrary/tools/config.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary/tools/read.py` & `arklibrary-1.0.1/src/arklibrary/tools/read.py`

 * *Files identical despite different names*

### Comparing `arklibrary-0.0.9/src/arklibrary.egg-info/PKG-INFO` & `arklibrary-1.0.1/src/arklibrary.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: arklibrary
-Version: 0.0.9
+Version: 1.0.1
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Library
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Library/issues
 Platform: win32
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # Ark-Library
```

### Comparing `arklibrary-0.0.9/src/arklibrary.egg-info/SOURCES.txt` & `arklibrary-1.0.1/src/arklibrary.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 src/arklibrary.egg-info/SOURCES.txt
 src/arklibrary.egg-info/dependency_links.txt
 src/arklibrary.egg-info/requires.txt
 src/arklibrary.egg-info/top_level.txt
 src/arklibrary/admin/__init__.py
 src/arklibrary/admin/admin.py
 src/arklibrary/admin/bundle.py
-src/arklibrary/admin/commands.py
 src/arklibrary/admin/run_driver.py
 src/arklibrary/blueprints/__init__.py
 src/arklibrary/blueprints/ammunitions.py
 src/arklibrary/blueprints/armours.py
 src/arklibrary/blueprints/artifacts.py
 src/arklibrary/blueprints/beacons.py
 src/arklibrary/blueprints/chibis.py
@@ -40,13 +39,18 @@
 src/arklibrary/data_structures/encoder.py
 src/arklibrary/data_structures/stream.py
 src/arklibrary/data_structures/tri.py
 src/arklibrary/events/__init__.py
 src/arklibrary/events/events.py
 src/arklibrary/lib/__init__.py
 src/arklibrary/lib/configuration.py
+src/arklibrary/lib/console.py
+src/arklibrary/lib/logger.py
+src/arklibrary/lib/pathify.py
 src/arklibrary/tools/__init__.py
 src/arklibrary/tools/ark_generic_scraper.py
 src/arklibrary/tools/ark_image_scraper.py
+src/arklibrary/tools/aws.py
 src/arklibrary/tools/clipboard.py
 src/arklibrary/tools/config.py
+src/arklibrary/tools/namecheap.py
 src/arklibrary/tools/read.py
```

