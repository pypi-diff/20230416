# Comparing `tmp/arklibrary-1.0.1.tar.gz` & `tmp/arklibrary-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arklibrary-1.0.1.tar", last modified: Sat Apr 15 22:59:16 2023, max compression
+gzip compressed data, was "arklibrary-1.0.2.tar", last modified: Sun Apr 16 01:56:10 2023, max compression
```

## Comparing `arklibrary-1.0.1.tar` & `arklibrary-1.0.2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 22:59:16.771011 arklibrary-1.0.1/
--rw-rw-rw-   0        0        0     1095 2023-03-25 16:33:09.000000 arklibrary-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      713 2023-04-15 22:59:16.771011 arklibrary-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-03-25 16:33:09.000000 arklibrary-1.0.1/README.md
--rw-rw-rw-   0        0        0      609 2023-04-11 00:15:08.000000 arklibrary-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1129 2023-04-15 22:59:16.773014 arklibrary-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 22:59:16.717184 arklibrary-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 22:59:16.723185 arklibrary-1.0.1/src/arklibrary/
--rw-rw-rw-   0        0        0      336 2023-04-04 02:19:21.000000 arklibrary-1.0.1/src/arklibrary/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 22:59:16.738222 arklibrary-1.0.1/src/arklibrary/admin/
--rw-rw-rw-   0        0        0      121 2023-03-31 21:02:39.000000 arklibrary-1.0.1/src/arklibrary/admin/__init__.py
--rw-rw-rw-   0        0        0    21095 2023-04-04 03:30:02.000000 arklibrary-1.0.1/src/arklibrary/admin/admin.py
--rw-rw-rw-   0        0        0    10273 2023-03-31 21:01:19.000000 arklibrary-1.0.1/src/arklibrary/admin/bundle.py
--rw-rw-rw-   0        0        0     2115 2023-03-31 21:01:19.000000 arklibrary-1.0.1/src/arklibrary/admin/run_driver.py
-drwxrwxrwx   0        0        0        0 2023-04-15 22:59:16.755997 arklibrary-1.0.1/src/arklibrary/blueprints/
--rw-rw-rw-   0        0        0     1101 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/__init__.py
--rw-rw-rw-   0        0        0     3803 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/ammunitions.py
--rw-rw-rw-   0        0        0     9636 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/armours.py
--rw-rw-rw-   0        0        0     9294 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/artifacts.py
--rw-rw-rw-   0        0        0    11005 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/beacons.py
--rw-rw-rw-   0        0        0    17601 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/chibis.py
--rw-rw-rw-   0        0        0     7885 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/colors.py
--rw-rw-rw-   0        0        0     9916 2023-04-04 03:26:01.000000 arklibrary-1.0.1/src/arklibrary/blueprints/commands.py
--rw-rw-rw-   0        0        0    21773 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/consumables.py
--rw-rw-rw-   0        0        0    78373 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/creatures.py
--rw-rw-rw-   0        0        0     3028 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/dyes.py
--rw-rw-rw-   0        0        0    11739 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/eggs.py
--rw-rw-rw-   0        0        0      942 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/farming.py
--rw-rw-rw-   0        0        0     2368 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/recipes.py
--rw-rw-rw-   0        0        0    11037 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/resources.py
--rw-rw-rw-   0        0        0    13208 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/saddles.py
--rw-rw-rw-   0        0        0     2146 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/seeds.py
--rw-rw-rw-   0        0        0    33071 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/skins.py
--rw-rw-rw-   0        0        0    52735 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/structures.py
--rw-rw-rw-   0        0        0     3409 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/tools.py
--rw-rw-rw-   0        0        0     5723 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/trophies.py
--rw-rw-rw-   0        0        0     8052 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/blueprints/weapons.py
--rw-rw-rw-   0        0        0      313 2023-04-04 01:37:11.000000 arklibrary-1.0.1/src/arklibrary/config.ini
-drwxrwxrwx   0        0        0        0 2023-04-15 22:59:16.758997 arklibrary-1.0.1/src/arklibrary/data_structures/
--rw-rw-rw-   0        0        0       88 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/data_structures/__init__.py
--rw-rw-rw-   0        0        0      646 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/data_structures/encoder.py
--rw-rw-rw-   0        0        0     2327 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/data_structures/stream.py
--rw-rw-rw-   0        0        0     4224 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/data_structures/tri.py
-drwxrwxrwx   0        0        0        0 2023-04-15 22:59:16.759998 arklibrary-1.0.1/src/arklibrary/events/
--rw-rw-rw-   0        0        0        0 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/events/__init__.py
--rw-rw-rw-   0        0        0     5211 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/events/events.py
-drwxrwxrwx   0        0        0        0 2023-04-15 22:59:16.763999 arklibrary-1.0.1/src/arklibrary/lib/
--rw-rw-rw-   0        0        0      166 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/lib/__init__.py
--rw-rw-rw-   0        0        0     2662 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/lib/configuration.py
--rw-rw-rw-   0        0        0     4115 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/lib/console.py
--rw-rw-rw-   0        0        0     4152 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/lib/logger.py
--rw-rw-rw-   0        0        0     2495 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/lib/pathify.py
-drwxrwxrwx   0        0        0        0 2023-04-15 22:59:16.771011 arklibrary-1.0.1/src/arklibrary/tools/
--rw-rw-rw-   0        0        0      137 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/tools/__init__.py
--rw-rw-rw-   0        0        0     2831 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/tools/ark_generic_scraper.py
--rw-rw-rw-   0        0        0    14575 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/tools/ark_image_scraper.py
--rw-rw-rw-   0        0        0        0 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/tools/aws.py
--rw-rw-rw-   0        0        0     4478 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/tools/clipboard.py
--rw-rw-rw-   0        0        0      956 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/tools/config.py
--rw-rw-rw-   0        0        0     3794 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/tools/namecheap.py
--rw-rw-rw-   0        0        0     1196 2023-03-25 16:33:09.000000 arklibrary-1.0.1/src/arklibrary/tools/read.py
-drwxrwxrwx   0        0        0        0 2023-04-15 22:59:16.735222 arklibrary-1.0.1/src/arklibrary.egg-info/
--rw-rw-rw-   0        0        0      713 2023-04-15 22:59:16.000000 arklibrary-1.0.1/src/arklibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1894 2023-04-15 22:59:16.000000 arklibrary-1.0.1/src/arklibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 22:59:16.000000 arklibrary-1.0.1/src/arklibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      122 2023-04-15 22:59:16.000000 arklibrary-1.0.1/src/arklibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-15 22:59:16.000000 arklibrary-1.0.1/src/arklibrary.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 01:56:10.389614 arklibrary-1.0.2/
+-rw-rw-rw-   0        0        0     1095 2023-03-25 16:33:09.000000 arklibrary-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      662 2023-04-16 01:56:10.390614 arklibrary-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-03-25 16:33:09.000000 arklibrary-1.0.2/README.md
+-rw-rw-rw-   0        0        0      609 2023-04-11 00:15:08.000000 arklibrary-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1089 2023-04-16 01:56:10.395614 arklibrary-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 01:56:10.328926 arklibrary-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 01:56:10.335927 arklibrary-1.0.2/src/arklibrary/
+-rw-rw-rw-   0        0        0      336 2023-04-04 02:19:21.000000 arklibrary-1.0.2/src/arklibrary/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:56:10.354618 arklibrary-1.0.2/src/arklibrary/admin/
+-rw-rw-rw-   0        0        0      121 2023-03-31 21:02:39.000000 arklibrary-1.0.2/src/arklibrary/admin/__init__.py
+-rw-rw-rw-   0        0        0    21095 2023-04-04 03:30:02.000000 arklibrary-1.0.2/src/arklibrary/admin/admin.py
+-rw-rw-rw-   0        0        0    10273 2023-03-31 21:01:19.000000 arklibrary-1.0.2/src/arklibrary/admin/bundle.py
+-rw-rw-rw-   0        0        0     2115 2023-03-31 21:01:19.000000 arklibrary-1.0.2/src/arklibrary/admin/run_driver.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:56:10.372614 arklibrary-1.0.2/src/arklibrary/blueprints/
+-rw-rw-rw-   0        0        0     1101 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/__init__.py
+-rw-rw-rw-   0        0        0     3803 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/ammunitions.py
+-rw-rw-rw-   0        0        0     9636 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/armours.py
+-rw-rw-rw-   0        0        0     9294 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/artifacts.py
+-rw-rw-rw-   0        0        0    11005 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/beacons.py
+-rw-rw-rw-   0        0        0    17601 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/chibis.py
+-rw-rw-rw-   0        0        0     7885 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/colors.py
+-rw-rw-rw-   0        0        0     9916 2023-04-04 03:26:01.000000 arklibrary-1.0.2/src/arklibrary/blueprints/commands.py
+-rw-rw-rw-   0        0        0    21773 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/consumables.py
+-rw-rw-rw-   0        0        0    78373 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/creatures.py
+-rw-rw-rw-   0        0        0     3028 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/dyes.py
+-rw-rw-rw-   0        0        0    11739 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/eggs.py
+-rw-rw-rw-   0        0        0      942 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/farming.py
+-rw-rw-rw-   0        0        0     2368 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/recipes.py
+-rw-rw-rw-   0        0        0    11037 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/resources.py
+-rw-rw-rw-   0        0        0    13208 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/saddles.py
+-rw-rw-rw-   0        0        0     2146 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/seeds.py
+-rw-rw-rw-   0        0        0    33071 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/skins.py
+-rw-rw-rw-   0        0        0    52735 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/structures.py
+-rw-rw-rw-   0        0        0     3409 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/tools.py
+-rw-rw-rw-   0        0        0     5723 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/trophies.py
+-rw-rw-rw-   0        0        0     8052 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/blueprints/weapons.py
+-rw-rw-rw-   0        0        0      313 2023-04-04 01:37:11.000000 arklibrary-1.0.2/src/arklibrary/config.ini
+drwxrwxrwx   0        0        0        0 2023-04-16 01:56:10.376612 arklibrary-1.0.2/src/arklibrary/data_structures/
+-rw-rw-rw-   0        0        0       88 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/data_structures/__init__.py
+-rw-rw-rw-   0        0        0      646 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/data_structures/encoder.py
+-rw-rw-rw-   0        0        0     2327 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/data_structures/stream.py
+-rw-rw-rw-   0        0        0     4224 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/data_structures/tri.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:56:10.378613 arklibrary-1.0.2/src/arklibrary/events/
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/events/__init__.py
+-rw-rw-rw-   0        0        0     5211 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/events/events.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:56:10.382613 arklibrary-1.0.2/src/arklibrary/lib/
+-rw-rw-rw-   0        0        0      166 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/lib/__init__.py
+-rw-rw-rw-   0        0        0     2662 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/lib/configuration.py
+-rw-rw-rw-   0        0        0     4115 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/lib/console.py
+-rw-rw-rw-   0        0        0     4152 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/lib/logger.py
+-rw-rw-rw-   0        0        0     2495 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/lib/pathify.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:56:10.389614 arklibrary-1.0.2/src/arklibrary/tools/
+-rw-rw-rw-   0        0        0      137 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/tools/__init__.py
+-rw-rw-rw-   0        0        0     2831 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/tools/ark_generic_scraper.py
+-rw-rw-rw-   0        0        0    14575 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/tools/ark_image_scraper.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/tools/aws.py
+-rw-rw-rw-   0        0        0     4478 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/tools/clipboard.py
+-rw-rw-rw-   0        0        0      956 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/tools/config.py
+-rw-rw-rw-   0        0        0     3794 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/tools/namecheap.py
+-rw-rw-rw-   0        0        0     1196 2023-03-25 16:33:09.000000 arklibrary-1.0.2/src/arklibrary/tools/read.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:56:10.351615 arklibrary-1.0.2/src/arklibrary.egg-info/
+-rw-rw-rw-   0        0        0      662 2023-04-16 01:56:10.000000 arklibrary-1.0.2/src/arklibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1894 2023-04-16 01:56:10.000000 arklibrary-1.0.2/src/arklibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 01:56:10.000000 arklibrary-1.0.2/src/arklibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      122 2023-04-16 01:56:10.000000 arklibrary-1.0.2/src/arklibrary.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-16 01:56:10.000000 arklibrary-1.0.2/src/arklibrary.egg-info/top_level.txt
```

### Comparing `arklibrary-1.0.1/LICENSE` & `arklibrary-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/PKG-INFO` & `arklibrary-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: arklibrary
-Version: 1.0.1
+Version: 1.0.2
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Library
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Library/issues
 Platform: win32
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # Ark-Library
```

### Comparing `arklibrary-1.0.1/pyproject.toml` & `arklibrary-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/setup.cfg` & `arklibrary-1.0.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 726b 6c69 6272 6172 790d 0a76   = arklibrary..v
-00000020: 6572 7369 6f6e 203d 2031 2e30 2e31 0d0a  ersion = 1.0.1..
+00000020: 6572 7369 6f6e 203d 2031 2e30 2e32 0d0a  ersion = 1.0.2..
 00000030: 7072 6f64 7563 7469 6f6e 5f76 6572 7369  production_versi
-00000040: 6f6e 203d 2031 2e30 2e31 0d0a 7465 7374  on = 1.0.1..test
-00000050: 5f76 6572 7369 6f6e 203d 2031 2e30 2e32  _version = 1.0.2
+00000040: 6f6e 203d 2031 2e30 2e32 0d0a 7465 7374  on = 1.0.2..test
+00000050: 5f76 6572 7369 6f6e 203d 2031 2e30 2e33  _version = 1.0.3
 00000060: 0d0a 6175 7468 6f72 203d 204d 6175 7269  ..author = Mauri
 00000070: 6369 6f0d 0a61 7574 686f 725f 656d 6169  cio..author_emai
 00000080: 6c20 3d20 6465 762e 6d61 7572 6963 696f  l = dev.mauricio
 00000090: 2e6c 6f6d 656c 6940 676d 6169 6c2e 636f  .lomeli@gmail.co
 000000a0: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 000000b0: 2054 6869 7320 6170 706c 6963 6174 696f   This applicatio
 000000c0: 6e20 6163 6365 7373 6573 2074 6865 2041  n accesses the A
@@ -26,46 +26,44 @@
 00000190: 6875 622e 636f 6d2f 4761 6d65 5365 7276  hub.com/GameServ
 000001a0: 6572 4775 7275 732f 4172 6b2d 4c69 6272  erGurus/Ark-Libr
 000001b0: 6172 792f 6973 7375 6573 0d0a 706c 6174  ary/issues..plat
 000001c0: 666f 726d 7320 3d20 7769 6e33 320d 0a63  forms = win32..c
 000001d0: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
 000001e0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
 000001f0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000200: 3a20 332e 380d 0a09 5072 6f67 7261 6d6d  : 3.8...Programm
+00000200: 3a20 332e 390d 0a09 5072 6f67 7261 6d6d  : 3.9...Programm
 00000210: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000220: 5079 7468 6f6e 203a 3a20 332e 390d 0a09  Python :: 3.9...
-00000230: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000240: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000250: 3a20 332e 3130 0d0a 090d 0a09 4c69 6365  : 3.10......Lice
-00000260: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-00000270: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
-00000280: 7365 0d0a 094f 7065 7261 7469 6e67 2053  se...Operating S
-00000290: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
-000002a0: 7065 6e64 656e 740d 0a0d 0a5b 6f70 7469  pendent....[opti
-000002b0: 6f6e 735d 0d0a 7061 636b 6167 655f 6469  ons]..package_di
-000002c0: 7220 3d20 0d0a 093d 2073 7263 0d0a 7061  r = ...= src..pa
-000002d0: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
-000002e0: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
-000002f0: 3d20 3e3d 332e 380d 0a69 6e73 7461 6c6c  = >=3.8..install
-00000300: 5f72 6571 7569 7265 7320 3d20 0d0a 0972  _requires = ...r
-00000310: 6571 7565 7374 733e 3d32 2e32 382e 320d  equests>=2.28.2.
-00000320: 0a09 786d 6c74 6f64 6963 743e 3d30 2e31  ..xmltodict>=0.1
-00000330: 332e 300d 0a09 6e75 6d70 793e 3d31 2e32  3.0...numpy>=1.2
-00000340: 342e 320d 0a0d 0a5b 6f70 7469 6f6e 732e  4.2....[options.
-00000350: 7061 636b 6167 6573 2e66 696e 645d 0d0a  packages.find]..
-00000360: 7768 6572 6520 3d20 7372 630d 0a0d 0a5b  where = src....[
-00000370: 6f70 7469 6f6e 732e 6578 7472 6173 5f72  options.extras_r
-00000380: 6571 7569 7265 5d0d 0a74 6573 7469 6e67  equire]..testing
-00000390: 203d 200d 0a09 7079 7465 7374 3e3d 362e   = ...pytest>=6.
-000003a0: 300d 0a09 7079 7465 7374 2d63 6f76 3e3d  0...pytest-cov>=
-000003b0: 322e 300d 0a09 6d79 7079 3e3d 302e 3937  2.0...mypy>=0.97
-000003c0: 310d 0a09 666c 616b 6538 3e3d 332e 390d  1...flake8>=3.9.
-000003d0: 0a09 746f 783e 3d33 2e32 340d 0a0d 0a5b  ..tox>=3.24....[
-000003e0: 6f70 7469 6f6e 732e 7061 636b 6167 655f  options.package_
-000003f0: 6461 7461 5d0d 0a61 726b 6c69 6272 6172  data]..arklibrar
-00000400: 7920 3d20 7079 2e74 7970 6564 2c20 636f  y = py.typed, co
-00000410: 6e66 6967 2e69 6e69 0d0a 0d0a 5b66 6c61  nfig.ini....[fla
-00000420: 6b65 385d 0d0a 6d61 782d 6c69 6e65 2d6c  ke8]..max-line-l
-00000430: 656e 6774 6820 3d20 3136 300d 0a0d 0a5b  ength = 160....[
-00000440: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-00000450: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-00000460: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000220: 5079 7468 6f6e 203a 3a20 332e 3130 0d0a  Python :: 3.10..
+00000230: 090d 0a09 4c69 6365 6e73 6520 3a3a 204f  ....License :: O
+00000240: 5349 2041 7070 726f 7665 6420 3a3a 204d  SI Approved :: M
+00000250: 4954 204c 6963 656e 7365 0d0a 094f 7065  IT License...Ope
+00000260: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000270: 204f 5320 496e 6465 7065 6e64 656e 740d   OS Independent.
+00000280: 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a 7061  ...[options]..pa
+00000290: 636b 6167 655f 6469 7220 3d20 0d0a 093d  ckage_dir = ...=
+000002a0: 2073 7263 0d0a 7061 636b 6167 6573 203d   src..packages =
+000002b0: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
+000002c0: 6571 7569 7265 7320 3d20 3e3d 332e 390d  equires = >=3.9.
+000002d0: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
+000002e0: 7320 3d20 0d0a 0972 6571 7565 7374 733e  s = ...requests>
+000002f0: 3d32 2e32 382e 320d 0a09 786d 6c74 6f64  =2.28.2...xmltod
+00000300: 6963 743e 3d30 2e31 332e 300d 0a09 6e75  ict>=0.13.0...nu
+00000310: 6d70 793e 3d31 2e32 342e 320d 0a0d 0a5b  mpy>=1.24.2....[
+00000320: 6f70 7469 6f6e 732e 7061 636b 6167 6573  options.packages
+00000330: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
+00000340: 7372 630d 0a0d 0a5b 6f70 7469 6f6e 732e  src....[options.
+00000350: 6578 7472 6173 5f72 6571 7569 7265 5d0d  extras_require].
+00000360: 0a74 6573 7469 6e67 203d 200d 0a09 7079  .testing = ...py
+00000370: 7465 7374 3e3d 362e 300d 0a09 7079 7465  test>=6.0...pyte
+00000380: 7374 2d63 6f76 3e3d 322e 300d 0a09 6d79  st-cov>=2.0...my
+00000390: 7079 3e3d 302e 3937 310d 0a09 666c 616b  py>=0.971...flak
+000003a0: 6538 3e3d 332e 390d 0a09 746f 783e 3d33  e8>=3.9...tox>=3
+000003b0: 2e32 340d 0a0d 0a5b 6f70 7469 6f6e 732e  .24....[options.
+000003c0: 7061 636b 6167 655f 6461 7461 5d0d 0a61  package_data]..a
+000003d0: 726b 6c69 6272 6172 7920 3d20 7079 2e74  rklibrary = py.t
+000003e0: 7970 6564 2c20 636f 6e66 6967 2e69 6e69  yped, config.ini
+000003f0: 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a 6d61  ....[flake8]..ma
+00000400: 782d 6c69 6e65 2d6c 656e 6774 6820 3d20  x-line-length = 
+00000410: 3136 300d 0a0d 0a5b 6567 675f 696e 666f  160....[egg_info
+00000420: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000430: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000440: 0a                                       .
```

### Comparing `arklibrary-1.0.1/src/arklibrary/admin/admin.py` & `arklibrary-1.0.2/src/arklibrary/admin/admin.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/admin/bundle.py` & `arklibrary-1.0.2/src/arklibrary/admin/bundle.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/admin/run_driver.py` & `arklibrary-1.0.2/src/arklibrary/admin/run_driver.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/__init__.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/__init__.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/ammunitions.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/ammunitions.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/armours.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/armours.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/artifacts.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/artifacts.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/beacons.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/beacons.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/chibis.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/chibis.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/colors.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/colors.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/commands.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/commands.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/consumables.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/consumables.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/creatures.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/creatures.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/dyes.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/dyes.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/eggs.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/eggs.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/farming.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/farming.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/recipes.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/recipes.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/resources.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/resources.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/saddles.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/saddles.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/seeds.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/seeds.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/skins.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/skins.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/structures.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/structures.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/tools.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/tools.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/trophies.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/trophies.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/blueprints/weapons.py` & `arklibrary-1.0.2/src/arklibrary/blueprints/weapons.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/data_structures/encoder.py` & `arklibrary-1.0.2/src/arklibrary/data_structures/encoder.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/data_structures/stream.py` & `arklibrary-1.0.2/src/arklibrary/data_structures/stream.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/data_structures/tri.py` & `arklibrary-1.0.2/src/arklibrary/data_structures/tri.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/events/events.py` & `arklibrary-1.0.2/src/arklibrary/events/events.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/lib/configuration.py` & `arklibrary-1.0.2/src/arklibrary/lib/configuration.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/lib/console.py` & `arklibrary-1.0.2/src/arklibrary/lib/console.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/lib/logger.py` & `arklibrary-1.0.2/src/arklibrary/lib/logger.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/lib/pathify.py` & `arklibrary-1.0.2/src/arklibrary/lib/pathify.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/tools/ark_generic_scraper.py` & `arklibrary-1.0.2/src/arklibrary/tools/ark_generic_scraper.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/tools/ark_image_scraper.py` & `arklibrary-1.0.2/src/arklibrary/tools/ark_image_scraper.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/tools/clipboard.py` & `arklibrary-1.0.2/src/arklibrary/tools/clipboard.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/tools/config.py` & `arklibrary-1.0.2/src/arklibrary/tools/config.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/tools/namecheap.py` & `arklibrary-1.0.2/src/arklibrary/tools/namecheap.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary/tools/read.py` & `arklibrary-1.0.2/src/arklibrary/tools/read.py`

 * *Files identical despite different names*

### Comparing `arklibrary-1.0.1/src/arklibrary.egg-info/PKG-INFO` & `arklibrary-1.0.2/src/arklibrary.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: arklibrary
-Version: 1.0.1
+Version: 1.0.2
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Library
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Library/issues
 Platform: win32
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # Ark-Library
```

### Comparing `arklibrary-1.0.1/src/arklibrary.egg-info/SOURCES.txt` & `arklibrary-1.0.2/src/arklibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

