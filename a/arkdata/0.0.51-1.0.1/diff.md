# Comparing `tmp/arkdata-0.0.51.tar.gz` & `tmp/arkdata-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkdata-0.0.51.tar", last modified: Wed Apr 12 17:24:45 2023, max compression
+gzip compressed data, was "arkdata-1.0.1.tar", last modified: Sat Apr 15 23:57:42 2023, max compression
```

## Comparing `arkdata-0.0.51.tar` & `arkdata-1.0.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 17:24:45.227339 arkdata-0.0.51/
--rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:13.000000 arkdata-0.0.51/LICENSE
--rw-rw-rw-   0        0        0      804 2023-04-12 17:24:45.227339 arkdata-0.0.51/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-03-25 16:35:13.000000 arkdata-0.0.51/README.md
--rw-rw-rw-   0        0        0      669 2023-04-11 00:23:50.000000 arkdata-0.0.51/pyproject.toml
--rw-rw-rw-   0        0        0     1315 2023-04-12 17:24:45.229340 arkdata-0.0.51/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-12 17:24:45.119030 arkdata-0.0.51/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 17:24:45.125553 arkdata-0.0.51/src/arkdata/
--rw-rw-rw-   0        0        0       54 2023-04-02 01:40:29.000000 arkdata-0.0.51/src/arkdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-12 17:24:45.138066 arkdata-0.0.51/src/arkdata/database/
--rw-rw-rw-   0        0        0      242 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/database/__init__.py
--rw-rw-rw-   0        0        0      860 2023-03-27 03:33:59.000000 arkdata-0.0.51/src/arkdata/database/configuration.py
--rw-rw-rw-   0        0        0     3371 2023-04-11 01:32:04.000000 arkdata-0.0.51/src/arkdata/database/cursor.py
--rw-rw-rw-   0        0        0     1470 2023-03-30 01:55:50.000000 arkdata-0.0.51/src/arkdata/database/database.py
--rw-rw-rw-   0        0        0     5190 2023-04-11 02:28:44.000000 arkdata-0.0.51/src/arkdata/database/table.py
--rw-rw-rw-   0        0        0        0 2023-03-27 03:33:59.000000 arkdata-0.0.51/src/arkdata/main.py
-drwxrwxrwx   0        0        0        0 2023-04-12 17:24:45.177305 arkdata-0.0.51/src/arkdata/models/
--rw-rw-rw-   0        0        0     2114 2023-04-04 00:26:27.000000 arkdata-0.0.51/src/arkdata/models/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-04-07 19:27:12.000000 arkdata-0.0.51/src/arkdata/models/account.py
--rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/ammunition.py
--rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/armour.py
--rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/artifact.py
--rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/attachment.py
--rw-rw-rw-   0        0        0     1397 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/cart_item.py
--rw-rw-rw-   0        0        0     1698 2023-04-12 17:24:05.000000 arkdata-0.0.51/src/arkdata/models/command.py
--rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/consumable.py
--rw-rw-rw-   0        0        0     1808 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/creature.py
--rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/dye.py
--rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/egg.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/farm.py
--rw-rw-rw-   0        0        0     1416 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/order_item.py
--rw-rw-rw-   0        0        0     2782 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/product.py
--rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/recipe.py
--rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/resource.py
--rw-rw-rw-   0        0        0     1629 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/saddle.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/seed.py
--rw-rw-rw-   0        0        0      810 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/server.py
--rw-rw-rw-   0        0        0     1757 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/sessions.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/skin.py
--rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/structure.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/tool.py
--rw-rw-rw-   0        0        0     1289 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/trophy.py
--rw-rw-rw-   0        0        0     1581 2023-04-11 01:12:51.000000 arkdata-0.0.51/src/arkdata/models/user.py
--rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-0.0.51/src/arkdata/models/weapon.py
-drwxrwxrwx   0        0        0        0 2023-04-12 17:24:45.226338 arkdata-0.0.51/src/arkdata/seeds/
--rw-rw-rw-   0        0        0        0 2023-03-30 03:59:09.000000 arkdata-0.0.51/src/arkdata/seeds/__init__.py
--rw-rw-rw-   0        0        0     2041 2023-04-07 19:25:52.000000 arkdata-0.0.51/src/arkdata/seeds/accounts.json
--rw-rw-rw-   0        0        0    16119 2023-03-30 06:36:40.000000 arkdata-0.0.51/src/arkdata/seeds/ammunitions.json
--rw-rw-rw-   0        0        0    36003 2023-03-30 03:50:59.000000 arkdata-0.0.51/src/arkdata/seeds/armours.json
--rw-rw-rw-   0        0        0    32929 2023-03-30 03:50:56.000000 arkdata-0.0.51/src/arkdata/seeds/artifacts.json
--rw-rw-rw-   0        0        0     3081 2023-03-30 03:50:48.000000 arkdata-0.0.51/src/arkdata/seeds/attachments.json
--rw-rw-rw-   0        0        0      651 2023-03-30 03:50:40.000000 arkdata-0.0.51/src/arkdata/seeds/commands.json
--rw-rw-rw-   0        0        0   100583 2023-03-30 03:50:36.000000 arkdata-0.0.51/src/arkdata/seeds/consumables.json
--rw-rw-rw-   0        0        0   589770 2023-03-30 03:50:20.000000 arkdata-0.0.51/src/arkdata/seeds/creatures.json
--rw-rw-rw-   0        0        0    11428 2023-03-30 03:50:14.000000 arkdata-0.0.51/src/arkdata/seeds/dyes.json
--rw-rw-rw-   0        0        0    57046 2023-03-30 03:50:12.000000 arkdata-0.0.51/src/arkdata/seeds/eggs.json
--rw-rw-rw-   0        0        0     3588 2023-03-30 03:50:09.000000 arkdata-0.0.51/src/arkdata/seeds/farms.json
--rw-rw-rw-   0        0        0   225349 2023-03-30 06:03:15.000000 arkdata-0.0.51/src/arkdata/seeds/products.json
--rw-rw-rw-   0        0        0     8457 2023-03-30 03:50:01.000000 arkdata-0.0.51/src/arkdata/seeds/recipes.json
--rw-rw-rw-   0        0        0    52865 2023-03-30 03:49:55.000000 arkdata-0.0.51/src/arkdata/seeds/resources.json
--rw-rw-rw-   0        0        0    57917 2023-03-30 07:19:16.000000 arkdata-0.0.51/src/arkdata/seeds/saddles.json
--rw-rw-rw-   0        0        0    16789 2023-03-30 03:47:57.000000 arkdata-0.0.51/src/arkdata/seeds/seeds.json
--rw-rw-rw-   0        0        0   180774 2023-03-30 03:44:21.000000 arkdata-0.0.51/src/arkdata/seeds/skins.json
--rw-rw-rw-   0        0        0   185254 2023-03-30 03:44:16.000000 arkdata-0.0.51/src/arkdata/seeds/structures.json
--rw-rw-rw-   0        0        0    12933 2023-03-30 03:44:10.000000 arkdata-0.0.51/src/arkdata/seeds/tools.json
--rw-rw-rw-   0        0        0    23142 2023-03-30 03:44:02.000000 arkdata-0.0.51/src/arkdata/seeds/trophies.json
--rw-rw-rw-   0        0        0     1251 2023-03-30 04:20:15.000000 arkdata-0.0.51/src/arkdata/seeds/users.json
--rw-rw-rw-   0        0        0    29591 2023-03-30 03:43:50.000000 arkdata-0.0.51/src/arkdata/seeds/weapons.json
-drwxrwxrwx   0        0        0        0 2023-04-12 17:24:45.130548 arkdata-0.0.51/src/arkdata.egg-info/
--rw-rw-rw-   0        0        0      804 2023-04-12 17:24:45.000000 arkdata-0.0.51/src/arkdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1948 2023-04-12 17:24:45.000000 arkdata-0.0.51/src/arkdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 17:24:45.000000 arkdata-0.0.51/src/arkdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      186 2023-04-12 17:24:45.000000 arkdata-0.0.51/src/arkdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-12 17:24:45.000000 arkdata-0.0.51/src/arkdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-15 23:57:42.343434 arkdata-1.0.1/
+-rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:13.000000 arkdata-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      650 2023-04-15 23:57:42.343434 arkdata-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-03-25 16:35:13.000000 arkdata-1.0.1/README.md
+-rw-rw-rw-   0        0        0      666 2023-04-15 23:52:45.000000 arkdata-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1241 2023-04-15 23:57:42.344437 arkdata-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 23:57:42.287231 arkdata-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-15 23:57:42.292230 arkdata-1.0.1/src/arkdata/
+-rw-rw-rw-   0        0        0       54 2023-04-02 01:40:29.000000 arkdata-1.0.1/src/arkdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-15 23:57:42.301230 arkdata-1.0.1/src/arkdata/database/
+-rw-rw-rw-   0        0        0      242 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/database/__init__.py
+-rw-rw-rw-   0        0        0      860 2023-03-27 03:33:59.000000 arkdata-1.0.1/src/arkdata/database/configuration.py
+-rw-rw-rw-   0        0        0     3371 2023-04-11 01:32:04.000000 arkdata-1.0.1/src/arkdata/database/cursor.py
+-rw-rw-rw-   0        0        0     1470 2023-03-30 01:55:50.000000 arkdata-1.0.1/src/arkdata/database/database.py
+-rw-rw-rw-   0        0        0     5190 2023-04-11 02:28:44.000000 arkdata-1.0.1/src/arkdata/database/table.py
+-rw-rw-rw-   0        0        0        0 2023-03-27 03:33:59.000000 arkdata-1.0.1/src/arkdata/main.py
+drwxrwxrwx   0        0        0        0 2023-04-15 23:57:42.323433 arkdata-1.0.1/src/arkdata/models/
+-rw-rw-rw-   0        0        0     2114 2023-04-04 00:26:27.000000 arkdata-1.0.1/src/arkdata/models/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-04-07 19:27:12.000000 arkdata-1.0.1/src/arkdata/models/account.py
+-rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/ammunition.py
+-rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/armour.py
+-rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/artifact.py
+-rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/attachment.py
+-rw-rw-rw-   0        0        0     1397 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/cart_item.py
+-rw-rw-rw-   0        0        0     1698 2023-04-12 17:31:52.000000 arkdata-1.0.1/src/arkdata/models/command.py
+-rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/consumable.py
+-rw-rw-rw-   0        0        0     1808 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/creature.py
+-rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/dye.py
+-rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/egg.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/farm.py
+-rw-rw-rw-   0        0        0     1416 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/order_item.py
+-rw-rw-rw-   0        0        0     2782 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/product.py
+-rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/recipe.py
+-rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/resource.py
+-rw-rw-rw-   0        0        0     1629 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/saddle.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/seed.py
+-rw-rw-rw-   0        0        0      810 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/server.py
+-rw-rw-rw-   0        0        0     1757 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/sessions.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/skin.py
+-rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/structure.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/tool.py
+-rw-rw-rw-   0        0        0     1289 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/trophy.py
+-rw-rw-rw-   0        0        0     1581 2023-04-11 01:12:51.000000 arkdata-1.0.1/src/arkdata/models/user.py
+-rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/weapon.py
+drwxrwxrwx   0        0        0        0 2023-04-15 23:57:42.342434 arkdata-1.0.1/src/arkdata/seeds/
+-rw-rw-rw-   0        0        0        0 2023-03-30 03:59:09.000000 arkdata-1.0.1/src/arkdata/seeds/__init__.py
+-rw-rw-rw-   0        0        0     2041 2023-04-07 19:25:52.000000 arkdata-1.0.1/src/arkdata/seeds/accounts.json
+-rw-rw-rw-   0        0        0    16119 2023-03-30 06:36:40.000000 arkdata-1.0.1/src/arkdata/seeds/ammunitions.json
+-rw-rw-rw-   0        0        0    36003 2023-03-30 03:50:59.000000 arkdata-1.0.1/src/arkdata/seeds/armours.json
+-rw-rw-rw-   0        0        0    32929 2023-03-30 03:50:56.000000 arkdata-1.0.1/src/arkdata/seeds/artifacts.json
+-rw-rw-rw-   0        0        0     3081 2023-03-30 03:50:48.000000 arkdata-1.0.1/src/arkdata/seeds/attachments.json
+-rw-rw-rw-   0        0        0      651 2023-03-30 03:50:40.000000 arkdata-1.0.1/src/arkdata/seeds/commands.json
+-rw-rw-rw-   0        0        0   100583 2023-03-30 03:50:36.000000 arkdata-1.0.1/src/arkdata/seeds/consumables.json
+-rw-rw-rw-   0        0        0   589770 2023-03-30 03:50:20.000000 arkdata-1.0.1/src/arkdata/seeds/creatures.json
+-rw-rw-rw-   0        0        0    11428 2023-03-30 03:50:14.000000 arkdata-1.0.1/src/arkdata/seeds/dyes.json
+-rw-rw-rw-   0        0        0    57046 2023-03-30 03:50:12.000000 arkdata-1.0.1/src/arkdata/seeds/eggs.json
+-rw-rw-rw-   0        0        0     3588 2023-03-30 03:50:09.000000 arkdata-1.0.1/src/arkdata/seeds/farms.json
+-rw-rw-rw-   0        0        0   225349 2023-03-30 06:03:15.000000 arkdata-1.0.1/src/arkdata/seeds/products.json
+-rw-rw-rw-   0        0        0     8457 2023-03-30 03:50:01.000000 arkdata-1.0.1/src/arkdata/seeds/recipes.json
+-rw-rw-rw-   0        0        0    52865 2023-03-30 03:49:55.000000 arkdata-1.0.1/src/arkdata/seeds/resources.json
+-rw-rw-rw-   0        0        0    57917 2023-03-30 07:19:16.000000 arkdata-1.0.1/src/arkdata/seeds/saddles.json
+-rw-rw-rw-   0        0        0    16789 2023-03-30 03:47:57.000000 arkdata-1.0.1/src/arkdata/seeds/seeds.json
+-rw-rw-rw-   0        0        0   180774 2023-03-30 03:44:21.000000 arkdata-1.0.1/src/arkdata/seeds/skins.json
+-rw-rw-rw-   0        0        0   185254 2023-03-30 03:44:16.000000 arkdata-1.0.1/src/arkdata/seeds/structures.json
+-rw-rw-rw-   0        0        0    12933 2023-03-30 03:44:10.000000 arkdata-1.0.1/src/arkdata/seeds/tools.json
+-rw-rw-rw-   0        0        0    23142 2023-03-30 03:44:02.000000 arkdata-1.0.1/src/arkdata/seeds/trophies.json
+-rw-rw-rw-   0        0        0     1251 2023-03-30 04:20:15.000000 arkdata-1.0.1/src/arkdata/seeds/users.json
+-rw-rw-rw-   0        0        0    29591 2023-03-30 03:43:50.000000 arkdata-1.0.1/src/arkdata/seeds/weapons.json
+drwxrwxrwx   0        0        0        0 2023-04-15 23:57:42.297231 arkdata-1.0.1/src/arkdata.egg-info/
+-rw-rw-rw-   0        0        0      650 2023-04-15 23:57:42.000000 arkdata-1.0.1/src/arkdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1948 2023-04-15 23:57:42.000000 arkdata-1.0.1/src/arkdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 23:57:42.000000 arkdata-1.0.1/src/arkdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      183 2023-04-15 23:57:42.000000 arkdata-1.0.1/src/arkdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-15 23:57:42.000000 arkdata-1.0.1/src/arkdata.egg-info/top_level.txt
```

### Comparing `arkdata-0.0.51/LICENSE` & `arkdata-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/PKG-INFO` & `arkdata-1.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: arkdata
-Version: 0.0.51
+Version: 1.0.1
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Data
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Data/issues
 Platform: win32
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # Ark-Data
```

### Comparing `arkdata-0.0.51/pyproject.toml` & `arkdata-1.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
     "setuptools>=42",
     "wheel",
-    "arklibrary>=0.0.62",
+    "arklibrary==1.*",
     "python-dotenv>=1.0.0",
     "SQLAlchemy>=2.0.9",
     "sqlalchemy_utils>=0.40.0",
     "flask>=2.2.3"
 ]
 build-backend = "setuptools.build_meta"
```

### Comparing `arkdata-0.0.51/setup.cfg` & `arkdata-1.0.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,83 +1,78 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 726b 6461 7461 0d0a 7665 7273   = arkdata..vers
-00000020: 696f 6e20 3d20 302e 302e 3531 0d0a 6175  ion = 0.0.51..au
-00000030: 7468 6f72 203d 204d 6175 7269 6369 6f0d  thor = Mauricio.
-00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
-00000050: 6465 762e 6d61 7572 6963 696f 2e6c 6f6d  dev.mauricio.lom
-00000060: 656c 6940 676d 6169 6c2e 636f 6d0d 0a64  eli@gmail.com..d
-00000070: 6573 6372 6970 7469 6f6e 203d 2054 6869  escription = Thi
-00000080: 7320 6170 706c 6963 6174 696f 6e20 6163  s application ac
-00000090: 6365 7373 6573 2074 6865 2041 726b 2073  cesses the Ark s
-000000a0: 7973 7465 6d2e 0d0a 6c6f 6e67 5f64 6573  ystem...long_des
-000000b0: 6372 6970 7469 6f6e 203d 2066 696c 653a  cription = file:
-000000c0: 2052 4541 444d 452e 6d64 0d0a 6c6f 6e67   README.md..long
-000000d0: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
-000000e0: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
-000000f0: 2f6d 6172 6b64 6f77 6e0d 0a75 726c 203d  /markdown..url =
-00000100: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000110: 636f 6d2f 4761 6d65 5365 7276 6572 4775  com/GameServerGu
-00000120: 7275 732f 4172 6b2d 4461 7461 0d0a 7072  rus/Ark-Data..pr
-00000130: 6f6a 6563 745f 7572 6c73 203d 200d 0a09  oject_urls = ...
-00000140: 4275 6720 5472 6163 6b65 7220 3d20 6874  Bug Tracker = ht
-00000150: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000160: 2f47 616d 6553 6572 7665 7247 7572 7573  /GameServerGurus
-00000170: 2f41 726b 2d44 6174 612f 6973 7375 6573  /Ark-Data/issues
-00000180: 0d0a 706c 6174 666f 726d 7320 3d20 7769  ..platforms = wi
-00000190: 6e33 320d 0a63 6c61 7373 6966 6965 7273  n32..classifiers
-000001a0: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
-000001b0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000001c0: 7468 6f6e 203a 3a20 332e 360d 0a09 5072  thon :: 3.6...Pr
-000001d0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001e0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000001f0: 332e 370d 0a09 5072 6f67 7261 6d6d 696e  3.7...Programmin
-00000200: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000210: 7468 6f6e 203a 3a20 332e 380d 0a09 5072  thon :: 3.8...Pr
-00000220: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000230: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000240: 332e 390d 0a09 5072 6f67 7261 6d6d 696e  3.9...Programmin
-00000250: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000260: 7468 6f6e 203a 3a20 332e 3130 0d0a 090d  thon :: 3.10....
-00000270: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
-00000280: 2041 7070 726f 7665 6420 3a3a 204d 4954   Approved :: MIT
-00000290: 204c 6963 656e 7365 0d0a 094f 7065 7261   License...Opera
-000002a0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-000002b0: 5320 496e 6465 7065 6e64 656e 740d 0a0d  S Independent...
-000002c0: 0a5b 6f70 7469 6f6e 735d 0d0a 7061 636b  .[options]..pack
-000002d0: 6167 655f 6469 7220 3d20 0d0a 093d 2073  age_dir = ...= s
-000002e0: 7263 0d0a 7061 636b 6167 6573 203d 2066  rc..packages = f
-000002f0: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
-00000300: 7569 7265 7320 3d20 3e3d 332e 360d 0a69  uires = >=3.6..i
-00000310: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
-00000320: 3d20 0d0a 0972 6571 7565 7374 733e 3d32  = ...requests>=2
-00000330: 2e32 382e 310d 0a09 6172 6b6c 6962 7261  .28.1...arklibra
-00000340: 7279 3e3d 302e 302e 3632 0d0a 0970 7974  ry>=0.0.62...pyt
-00000350: 686f 6e2d 646f 7465 6e76 3e3d 312e 302e  hon-dotenv>=1.0.
-00000360: 300d 0a09 5351 4c41 6c63 6865 6d79 3e3d  0...SQLAlchemy>=
-00000370: 322e 302e 390d 0a09 7371 6c61 6c63 6865  2.0.9...sqlalche
-00000380: 6d79 5f75 7469 6c73 3e3d 302e 3430 2e30  my_utils>=0.40.0
-00000390: 0d0a 0966 6c61 736b 3e3d 322e 322e 330d  ...flask>=2.2.3.
-000003a0: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
-000003b0: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
-000003c0: 6520 3d20 7372 630d 0a0d 0a5b 6f70 7469  e = src....[opti
-000003d0: 6f6e 732e 6578 7472 6173 5f72 6571 7569  ons.extras_requi
-000003e0: 7265 5d0d 0a74 6573 7469 6e67 203d 200d  re]..testing = .
-000003f0: 0a09 7079 7465 7374 3e3d 362e 300d 0a09  ..pytest>=6.0...
-00000400: 7079 7465 7374 2d63 6f76 3e3d 322e 300d  pytest-cov>=2.0.
-00000410: 0a09 6d79 7079 3e3d 302e 3937 310d 0a09  ..mypy>=0.971...
-00000420: 666c 616b 6538 3e3d 332e 390d 0a09 746f  flake8>=3.9...to
-00000430: 783e 3d33 2e32 340d 0a0d 0a5b 6f70 7469  x>=3.24....[opti
-00000440: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
-00000450: 5d0d 0a61 726b 6461 7461 203d 200d 0a09  ]..arkdata = ...
-00000460: 7079 2e74 7970 6564 0d0a 0963 6f6e 6669  py.typed...confi
-00000470: 672e 696e 690d 0a61 726b 6461 7461 2e73  g.ini..arkdata.s
-00000480: 6565 6473 203d 200d 0a09 2a2e 6a73 6f6e  eeds = ...*.json
-00000490: 0d0a 6172 6b64 6174 612e 7365 6564 732e  ..arkdata.seeds.
-000004a0: 6461 7461 203d 200d 0a09 2a2e 6a73 6f6e  data = ...*.json
-000004b0: 0d0a 6172 6b64 6174 612e 7365 6564 732e  ..arkdata.seeds.
-000004c0: 7461 626c 6573 203d 200d 0a09 2a2e 6a73  tables = ...*.js
-000004d0: 6f6e 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a  on....[flake8]..
-000004e0: 6d61 782d 6c69 6e65 2d6c 656e 6774 6820  max-line-length 
-000004f0: 3d20 3136 300d 0a0d 0a5b 6567 675f 696e  = 160....[egg_in
-00000500: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-00000510: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-00000520: 0a0d 0a                                  ...
+00000020: 696f 6e20 3d20 312e 302e 310d 0a74 6573  ion = 1.0.1..tes
+00000030: 745f 7665 7273 696f 6e20 3d20 312e 302e  t_version = 1.0.
+00000040: 310d 0a70 726f 6475 6374 696f 6e5f 7665  1..production_ve
+00000050: 7273 696f 6e20 3d20 312e 302e 310d 0a61  rsion = 1.0.1..a
+00000060: 7574 686f 7220 3d20 4d61 7572 6963 696f  uthor = Mauricio
+00000070: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
+00000080: 2064 6576 2e6d 6175 7269 6369 6f2e 6c6f   dev.mauricio.lo
+00000090: 6d65 6c69 4067 6d61 696c 2e63 6f6d 0d0a  meli@gmail.com..
+000000a0: 6465 7363 7269 7074 696f 6e20 3d20 5468  description = Th
+000000b0: 6973 2061 7070 6c69 6361 7469 6f6e 2061  is application a
+000000c0: 6363 6573 7365 7320 7468 6520 4172 6b20  ccesses the Ark 
+000000d0: 7379 7374 656d 2e0d 0a6c 6f6e 675f 6465  system...long_de
+000000e0: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
+000000f0: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
+00000100: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
+00000110: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
+00000120: 742f 6d61 726b 646f 776e 0d0a 7572 6c20  t/markdown..url 
+00000130: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+00000140: 2e63 6f6d 2f47 616d 6553 6572 7665 7247  .com/GameServerG
+00000150: 7572 7573 2f41 726b 2d44 6174 610d 0a70  urus/Ark-Data..p
+00000160: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
+00000170: 0942 7567 2054 7261 636b 6572 203d 2068  .Bug Tracker = h
+00000180: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000190: 6d2f 4761 6d65 5365 7276 6572 4775 7275  m/GameServerGuru
+000001a0: 732f 4172 6b2d 4461 7461 2f69 7373 7565  s/Ark-Data/issue
+000001b0: 730d 0a70 6c61 7466 6f72 6d73 203d 2077  s..platforms = w
+000001c0: 696e 3332 0d0a 636c 6173 7369 6669 6572  in32..classifier
+000001d0: 7320 3d20 0d0a 0950 726f 6772 616d 6d69  s = ...Programmi
+000001e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001f0: 7974 686f 6e20 3a3a 2033 2e39 0d0a 0950  ython :: 3.9...P
+00000200: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000210: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000220: 2033 2e31 300d 0a09 0d0a 094c 6963 656e   3.10......Licen
+00000230: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
+00000240: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
+00000250: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
+00000260: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
+00000270: 656e 6465 6e74 0d0a 0d0a 5b6f 7074 696f  endent....[optio
+00000280: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
+00000290: 203d 200d 0a09 3d20 7372 630d 0a70 6163   = ...= src..pac
+000002a0: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
+000002b0: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
+000002c0: 203e 3d33 2e39 0d0a 696e 7374 616c 6c5f   >=3.9..install_
+000002d0: 7265 7175 6972 6573 203d 200d 0a09 7265  requires = ...re
+000002e0: 7175 6573 7473 3e3d 322e 3238 2e31 0d0a  quests>=2.28.1..
+000002f0: 0961 726b 6c69 6272 6172 793d 3d31 2e2a  .arklibrary==1.*
+00000300: 0d0a 0970 7974 686f 6e2d 646f 7465 6e76  ...python-dotenv
+00000310: 3e3d 312e 302e 300d 0a09 5351 4c41 6c63  >=1.0.0...SQLAlc
+00000320: 6865 6d79 3e3d 322e 302e 390d 0a09 7371  hemy>=2.0.9...sq
+00000330: 6c61 6c63 6865 6d79 5f75 7469 6c73 3e3d  lalchemy_utils>=
+00000340: 302e 3430 2e30 0d0a 0966 6c61 736b 3e3d  0.40.0...flask>=
+00000350: 322e 322e 330d 0a0d 0a5b 6f70 7469 6f6e  2.2.3....[option
+00000360: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+00000370: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
+00000380: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
+00000390: 5f72 6571 7569 7265 5d0d 0a74 6573 7469  _require]..testi
+000003a0: 6e67 203d 200d 0a09 7079 7465 7374 3e3d  ng = ...pytest>=
+000003b0: 362e 300d 0a09 7079 7465 7374 2d63 6f76  6.0...pytest-cov
+000003c0: 3e3d 322e 300d 0a09 6d79 7079 3e3d 302e  >=2.0...mypy>=0.
+000003d0: 3937 310d 0a09 666c 616b 6538 3e3d 332e  971...flake8>=3.
+000003e0: 390d 0a09 746f 783e 3d33 2e32 340d 0a0d  9...tox>=3.24...
+000003f0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
+00000400: 655f 6461 7461 5d0d 0a61 726b 6461 7461  e_data]..arkdata
+00000410: 203d 200d 0a09 7079 2e74 7970 6564 0d0a   = ...py.typed..
+00000420: 0963 6f6e 6669 672e 696e 690d 0a61 726b  .config.ini..ark
+00000430: 6461 7461 2e73 6565 6473 203d 200d 0a09  data.seeds = ...
+00000440: 2a2e 6a73 6f6e 0d0a 6172 6b64 6174 612e  *.json..arkdata.
+00000450: 7365 6564 732e 6461 7461 203d 200d 0a09  seeds.data = ...
+00000460: 2a2e 6a73 6f6e 0d0a 6172 6b64 6174 612e  *.json..arkdata.
+00000470: 7365 6564 732e 7461 626c 6573 203d 200d  seeds.tables = .
+00000480: 0a09 2a2e 6a73 6f6e 0d0a 0d0a 5b66 6c61  ..*.json....[fla
+00000490: 6b65 385d 0d0a 6d61 782d 6c69 6e65 2d6c  ke8]..max-line-l
+000004a0: 656e 6774 6820 3d20 3136 300d 0a0d 0a5b  ength = 160....[
+000004b0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+000004c0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+000004d0: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `arkdata-0.0.51/src/arkdata/database/configuration.py` & `arkdata-1.0.1/src/arkdata/database/configuration.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/database/cursor.py` & `arkdata-1.0.1/src/arkdata/database/cursor.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/database/database.py` & `arkdata-1.0.1/src/arkdata/database/database.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/database/table.py` & `arkdata-1.0.1/src/arkdata/database/table.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/__init__.py` & `arkdata-1.0.1/src/arkdata/models/__init__.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/account.py` & `arkdata-1.0.1/src/arkdata/models/account.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/ammunition.py` & `arkdata-1.0.1/src/arkdata/models/ammunition.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/armour.py` & `arkdata-1.0.1/src/arkdata/models/armour.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/artifact.py` & `arkdata-1.0.1/src/arkdata/models/artifact.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/attachment.py` & `arkdata-1.0.1/src/arkdata/models/attachment.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/cart_item.py` & `arkdata-1.0.1/src/arkdata/models/cart_item.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/command.py` & `arkdata-1.0.1/src/arkdata/models/command.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/consumable.py` & `arkdata-1.0.1/src/arkdata/models/consumable.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/creature.py` & `arkdata-1.0.1/src/arkdata/models/creature.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/dye.py` & `arkdata-1.0.1/src/arkdata/models/dye.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/egg.py` & `arkdata-1.0.1/src/arkdata/models/egg.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/farm.py` & `arkdata-1.0.1/src/arkdata/models/farm.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/order_item.py` & `arkdata-1.0.1/src/arkdata/models/order_item.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/product.py` & `arkdata-1.0.1/src/arkdata/models/product.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/recipe.py` & `arkdata-1.0.1/src/arkdata/models/recipe.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/resource.py` & `arkdata-1.0.1/src/arkdata/models/resource.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/saddle.py` & `arkdata-1.0.1/src/arkdata/models/saddle.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/seed.py` & `arkdata-1.0.1/src/arkdata/models/seed.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/server.py` & `arkdata-1.0.1/src/arkdata/models/server.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/sessions.py` & `arkdata-1.0.1/src/arkdata/models/sessions.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/skin.py` & `arkdata-1.0.1/src/arkdata/models/skin.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/structure.py` & `arkdata-1.0.1/src/arkdata/models/structure.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/tool.py` & `arkdata-1.0.1/src/arkdata/models/tool.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/trophy.py` & `arkdata-1.0.1/src/arkdata/models/trophy.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/user.py` & `arkdata-1.0.1/src/arkdata/models/user.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/models/weapon.py` & `arkdata-1.0.1/src/arkdata/models/weapon.py`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/accounts.json` & `arkdata-1.0.1/src/arkdata/seeds/accounts.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/ammunitions.json` & `arkdata-1.0.1/src/arkdata/seeds/ammunitions.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/armours.json` & `arkdata-1.0.1/src/arkdata/seeds/armours.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/artifacts.json` & `arkdata-1.0.1/src/arkdata/seeds/artifacts.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/attachments.json` & `arkdata-1.0.1/src/arkdata/seeds/attachments.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/commands.json` & `arkdata-1.0.1/src/arkdata/seeds/commands.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/consumables.json` & `arkdata-1.0.1/src/arkdata/seeds/consumables.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/creatures.json` & `arkdata-1.0.1/src/arkdata/seeds/creatures.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/dyes.json` & `arkdata-1.0.1/src/arkdata/seeds/dyes.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/eggs.json` & `arkdata-1.0.1/src/arkdata/seeds/eggs.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/farms.json` & `arkdata-1.0.1/src/arkdata/seeds/farms.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/products.json` & `arkdata-1.0.1/src/arkdata/seeds/products.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/recipes.json` & `arkdata-1.0.1/src/arkdata/seeds/recipes.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/resources.json` & `arkdata-1.0.1/src/arkdata/seeds/resources.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/saddles.json` & `arkdata-1.0.1/src/arkdata/seeds/saddles.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/seeds.json` & `arkdata-1.0.1/src/arkdata/seeds/seeds.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/skins.json` & `arkdata-1.0.1/src/arkdata/seeds/skins.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/structures.json` & `arkdata-1.0.1/src/arkdata/seeds/structures.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/tools.json` & `arkdata-1.0.1/src/arkdata/seeds/tools.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/trophies.json` & `arkdata-1.0.1/src/arkdata/seeds/trophies.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/users.json` & `arkdata-1.0.1/src/arkdata/seeds/users.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata/seeds/weapons.json` & `arkdata-1.0.1/src/arkdata/seeds/weapons.json`

 * *Files identical despite different names*

### Comparing `arkdata-0.0.51/src/arkdata.egg-info/PKG-INFO` & `arkdata-1.0.1/src/arkdata.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: arkdata
-Version: 0.0.51
+Version: 1.0.1
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Data
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Data/issues
 Platform: win32
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 # Ark-Data
```

### Comparing `arkdata-0.0.51/src/arkdata.egg-info/SOURCES.txt` & `arkdata-1.0.1/src/arkdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

