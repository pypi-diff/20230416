# Comparing `tmp/arkdata-1.0.1.tar.gz` & `tmp/arkdata-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkdata-1.0.1.tar", last modified: Sat Apr 15 23:57:42 2023, max compression
+gzip compressed data, was "arkdata-1.0.2.tar", last modified: Sun Apr 16 02:15:01 2023, max compression
```

## Comparing `arkdata-1.0.1.tar` & `arkdata-1.0.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 23:57:42.343434 arkdata-1.0.1/
--rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:13.000000 arkdata-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      650 2023-04-15 23:57:42.343434 arkdata-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       12 2023-03-25 16:35:13.000000 arkdata-1.0.1/README.md
--rw-rw-rw-   0        0        0      666 2023-04-15 23:52:45.000000 arkdata-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1241 2023-04-15 23:57:42.344437 arkdata-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 23:57:42.287231 arkdata-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 23:57:42.292230 arkdata-1.0.1/src/arkdata/
--rw-rw-rw-   0        0        0       54 2023-04-02 01:40:29.000000 arkdata-1.0.1/src/arkdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 23:57:42.301230 arkdata-1.0.1/src/arkdata/database/
--rw-rw-rw-   0        0        0      242 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/database/__init__.py
--rw-rw-rw-   0        0        0      860 2023-03-27 03:33:59.000000 arkdata-1.0.1/src/arkdata/database/configuration.py
--rw-rw-rw-   0        0        0     3371 2023-04-11 01:32:04.000000 arkdata-1.0.1/src/arkdata/database/cursor.py
--rw-rw-rw-   0        0        0     1470 2023-03-30 01:55:50.000000 arkdata-1.0.1/src/arkdata/database/database.py
--rw-rw-rw-   0        0        0     5190 2023-04-11 02:28:44.000000 arkdata-1.0.1/src/arkdata/database/table.py
--rw-rw-rw-   0        0        0        0 2023-03-27 03:33:59.000000 arkdata-1.0.1/src/arkdata/main.py
-drwxrwxrwx   0        0        0        0 2023-04-15 23:57:42.323433 arkdata-1.0.1/src/arkdata/models/
--rw-rw-rw-   0        0        0     2114 2023-04-04 00:26:27.000000 arkdata-1.0.1/src/arkdata/models/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-04-07 19:27:12.000000 arkdata-1.0.1/src/arkdata/models/account.py
--rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/ammunition.py
--rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/armour.py
--rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/artifact.py
--rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/attachment.py
--rw-rw-rw-   0        0        0     1397 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/cart_item.py
--rw-rw-rw-   0        0        0     1698 2023-04-12 17:31:52.000000 arkdata-1.0.1/src/arkdata/models/command.py
--rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/consumable.py
--rw-rw-rw-   0        0        0     1808 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/creature.py
--rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/dye.py
--rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/egg.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/farm.py
--rw-rw-rw-   0        0        0     1416 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/order_item.py
--rw-rw-rw-   0        0        0     2782 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/product.py
--rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/recipe.py
--rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/resource.py
--rw-rw-rw-   0        0        0     1629 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/saddle.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/seed.py
--rw-rw-rw-   0        0        0      810 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/server.py
--rw-rw-rw-   0        0        0     1757 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/sessions.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/skin.py
--rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/structure.py
--rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/tool.py
--rw-rw-rw-   0        0        0     1289 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/trophy.py
--rw-rw-rw-   0        0        0     1581 2023-04-11 01:12:51.000000 arkdata-1.0.1/src/arkdata/models/user.py
--rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.1/src/arkdata/models/weapon.py
-drwxrwxrwx   0        0        0        0 2023-04-15 23:57:42.342434 arkdata-1.0.1/src/arkdata/seeds/
--rw-rw-rw-   0        0        0        0 2023-03-30 03:59:09.000000 arkdata-1.0.1/src/arkdata/seeds/__init__.py
--rw-rw-rw-   0        0        0     2041 2023-04-07 19:25:52.000000 arkdata-1.0.1/src/arkdata/seeds/accounts.json
--rw-rw-rw-   0        0        0    16119 2023-03-30 06:36:40.000000 arkdata-1.0.1/src/arkdata/seeds/ammunitions.json
--rw-rw-rw-   0        0        0    36003 2023-03-30 03:50:59.000000 arkdata-1.0.1/src/arkdata/seeds/armours.json
--rw-rw-rw-   0        0        0    32929 2023-03-30 03:50:56.000000 arkdata-1.0.1/src/arkdata/seeds/artifacts.json
--rw-rw-rw-   0        0        0     3081 2023-03-30 03:50:48.000000 arkdata-1.0.1/src/arkdata/seeds/attachments.json
--rw-rw-rw-   0        0        0      651 2023-03-30 03:50:40.000000 arkdata-1.0.1/src/arkdata/seeds/commands.json
--rw-rw-rw-   0        0        0   100583 2023-03-30 03:50:36.000000 arkdata-1.0.1/src/arkdata/seeds/consumables.json
--rw-rw-rw-   0        0        0   589770 2023-03-30 03:50:20.000000 arkdata-1.0.1/src/arkdata/seeds/creatures.json
--rw-rw-rw-   0        0        0    11428 2023-03-30 03:50:14.000000 arkdata-1.0.1/src/arkdata/seeds/dyes.json
--rw-rw-rw-   0        0        0    57046 2023-03-30 03:50:12.000000 arkdata-1.0.1/src/arkdata/seeds/eggs.json
--rw-rw-rw-   0        0        0     3588 2023-03-30 03:50:09.000000 arkdata-1.0.1/src/arkdata/seeds/farms.json
--rw-rw-rw-   0        0        0   225349 2023-03-30 06:03:15.000000 arkdata-1.0.1/src/arkdata/seeds/products.json
--rw-rw-rw-   0        0        0     8457 2023-03-30 03:50:01.000000 arkdata-1.0.1/src/arkdata/seeds/recipes.json
--rw-rw-rw-   0        0        0    52865 2023-03-30 03:49:55.000000 arkdata-1.0.1/src/arkdata/seeds/resources.json
--rw-rw-rw-   0        0        0    57917 2023-03-30 07:19:16.000000 arkdata-1.0.1/src/arkdata/seeds/saddles.json
--rw-rw-rw-   0        0        0    16789 2023-03-30 03:47:57.000000 arkdata-1.0.1/src/arkdata/seeds/seeds.json
--rw-rw-rw-   0        0        0   180774 2023-03-30 03:44:21.000000 arkdata-1.0.1/src/arkdata/seeds/skins.json
--rw-rw-rw-   0        0        0   185254 2023-03-30 03:44:16.000000 arkdata-1.0.1/src/arkdata/seeds/structures.json
--rw-rw-rw-   0        0        0    12933 2023-03-30 03:44:10.000000 arkdata-1.0.1/src/arkdata/seeds/tools.json
--rw-rw-rw-   0        0        0    23142 2023-03-30 03:44:02.000000 arkdata-1.0.1/src/arkdata/seeds/trophies.json
--rw-rw-rw-   0        0        0     1251 2023-03-30 04:20:15.000000 arkdata-1.0.1/src/arkdata/seeds/users.json
--rw-rw-rw-   0        0        0    29591 2023-03-30 03:43:50.000000 arkdata-1.0.1/src/arkdata/seeds/weapons.json
-drwxrwxrwx   0        0        0        0 2023-04-15 23:57:42.297231 arkdata-1.0.1/src/arkdata.egg-info/
--rw-rw-rw-   0        0        0      650 2023-04-15 23:57:42.000000 arkdata-1.0.1/src/arkdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1948 2023-04-15 23:57:42.000000 arkdata-1.0.1/src/arkdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 23:57:42.000000 arkdata-1.0.1/src/arkdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      183 2023-04-15 23:57:42.000000 arkdata-1.0.1/src/arkdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-15 23:57:42.000000 arkdata-1.0.1/src/arkdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 02:15:01.554152 arkdata-1.0.2/
+-rw-rw-rw-   0        0        0     1095 2023-03-25 16:35:13.000000 arkdata-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      650 2023-04-16 02:15:01.555154 arkdata-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2023-03-25 16:35:13.000000 arkdata-1.0.2/README.md
+-rw-rw-rw-   0        0        0      642 2023-04-16 02:13:53.000000 arkdata-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1223 2023-04-16 02:15:01.556153 arkdata-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 02:15:01.495014 arkdata-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 02:15:01.501219 arkdata-1.0.2/src/arkdata/
+-rw-rw-rw-   0        0        0       54 2023-04-02 01:40:29.000000 arkdata-1.0.2/src/arkdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 02:15:01.510218 arkdata-1.0.2/src/arkdata/database/
+-rw-rw-rw-   0        0        0      242 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/database/__init__.py
+-rw-rw-rw-   0        0        0      860 2023-03-27 03:33:59.000000 arkdata-1.0.2/src/arkdata/database/configuration.py
+-rw-rw-rw-   0        0        0     3371 2023-04-11 01:32:04.000000 arkdata-1.0.2/src/arkdata/database/cursor.py
+-rw-rw-rw-   0        0        0     1470 2023-03-30 01:55:50.000000 arkdata-1.0.2/src/arkdata/database/database.py
+-rw-rw-rw-   0        0        0     5190 2023-04-11 02:28:44.000000 arkdata-1.0.2/src/arkdata/database/table.py
+-rw-rw-rw-   0        0        0        0 2023-03-27 03:33:59.000000 arkdata-1.0.2/src/arkdata/main.py
+drwxrwxrwx   0        0        0        0 2023-04-16 02:15:01.533156 arkdata-1.0.2/src/arkdata/models/
+-rw-rw-rw-   0        0        0     2114 2023-04-04 00:26:27.000000 arkdata-1.0.2/src/arkdata/models/__init__.py
+-rw-rw-rw-   0        0        0     1198 2023-04-07 19:27:12.000000 arkdata-1.0.2/src/arkdata/models/account.py
+-rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/ammunition.py
+-rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/armour.py
+-rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/artifact.py
+-rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/attachment.py
+-rw-rw-rw-   0        0        0     1397 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/cart_item.py
+-rw-rw-rw-   0        0        0     1698 2023-04-12 17:31:52.000000 arkdata-1.0.2/src/arkdata/models/command.py
+-rw-rw-rw-   0        0        0     1296 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/consumable.py
+-rw-rw-rw-   0        0        0     1808 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/creature.py
+-rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/dye.py
+-rw-rw-rw-   0        0        0     1282 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/egg.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/farm.py
+-rw-rw-rw-   0        0        0     1416 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/order_item.py
+-rw-rw-rw-   0        0        0     2782 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/product.py
+-rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/recipe.py
+-rw-rw-rw-   0        0        0     1292 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/resource.py
+-rw-rw-rw-   0        0        0     1629 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/saddle.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/seed.py
+-rw-rw-rw-   0        0        0      810 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/server.py
+-rw-rw-rw-   0        0        0     1757 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/sessions.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/skin.py
+-rw-rw-rw-   0        0        0     1294 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/structure.py
+-rw-rw-rw-   0        0        0     1284 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/tool.py
+-rw-rw-rw-   0        0        0     1289 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/trophy.py
+-rw-rw-rw-   0        0        0     1581 2023-04-11 01:12:51.000000 arkdata-1.0.2/src/arkdata/models/user.py
+-rw-rw-rw-   0        0        0     1288 2023-04-04 00:17:39.000000 arkdata-1.0.2/src/arkdata/models/weapon.py
+drwxrwxrwx   0        0        0        0 2023-04-16 02:15:01.554152 arkdata-1.0.2/src/arkdata/seeds/
+-rw-rw-rw-   0        0        0        0 2023-03-30 03:59:09.000000 arkdata-1.0.2/src/arkdata/seeds/__init__.py
+-rw-rw-rw-   0        0        0     2041 2023-04-07 19:25:52.000000 arkdata-1.0.2/src/arkdata/seeds/accounts.json
+-rw-rw-rw-   0        0        0    16119 2023-03-30 06:36:40.000000 arkdata-1.0.2/src/arkdata/seeds/ammunitions.json
+-rw-rw-rw-   0        0        0    36003 2023-03-30 03:50:59.000000 arkdata-1.0.2/src/arkdata/seeds/armours.json
+-rw-rw-rw-   0        0        0    32929 2023-03-30 03:50:56.000000 arkdata-1.0.2/src/arkdata/seeds/artifacts.json
+-rw-rw-rw-   0        0        0     3081 2023-03-30 03:50:48.000000 arkdata-1.0.2/src/arkdata/seeds/attachments.json
+-rw-rw-rw-   0        0        0      651 2023-03-30 03:50:40.000000 arkdata-1.0.2/src/arkdata/seeds/commands.json
+-rw-rw-rw-   0        0        0   100583 2023-03-30 03:50:36.000000 arkdata-1.0.2/src/arkdata/seeds/consumables.json
+-rw-rw-rw-   0        0        0   589770 2023-03-30 03:50:20.000000 arkdata-1.0.2/src/arkdata/seeds/creatures.json
+-rw-rw-rw-   0        0        0    11428 2023-03-30 03:50:14.000000 arkdata-1.0.2/src/arkdata/seeds/dyes.json
+-rw-rw-rw-   0        0        0    57046 2023-03-30 03:50:12.000000 arkdata-1.0.2/src/arkdata/seeds/eggs.json
+-rw-rw-rw-   0        0        0     3588 2023-03-30 03:50:09.000000 arkdata-1.0.2/src/arkdata/seeds/farms.json
+-rw-rw-rw-   0        0        0   225349 2023-03-30 06:03:15.000000 arkdata-1.0.2/src/arkdata/seeds/products.json
+-rw-rw-rw-   0        0        0     8457 2023-03-30 03:50:01.000000 arkdata-1.0.2/src/arkdata/seeds/recipes.json
+-rw-rw-rw-   0        0        0    52865 2023-03-30 03:49:55.000000 arkdata-1.0.2/src/arkdata/seeds/resources.json
+-rw-rw-rw-   0        0        0    57917 2023-03-30 07:19:16.000000 arkdata-1.0.2/src/arkdata/seeds/saddles.json
+-rw-rw-rw-   0        0        0    16789 2023-03-30 03:47:57.000000 arkdata-1.0.2/src/arkdata/seeds/seeds.json
+-rw-rw-rw-   0        0        0   180774 2023-03-30 03:44:21.000000 arkdata-1.0.2/src/arkdata/seeds/skins.json
+-rw-rw-rw-   0        0        0   185254 2023-03-30 03:44:16.000000 arkdata-1.0.2/src/arkdata/seeds/structures.json
+-rw-rw-rw-   0        0        0    12933 2023-03-30 03:44:10.000000 arkdata-1.0.2/src/arkdata/seeds/tools.json
+-rw-rw-rw-   0        0        0    23142 2023-03-30 03:44:02.000000 arkdata-1.0.2/src/arkdata/seeds/trophies.json
+-rw-rw-rw-   0        0        0     1251 2023-03-30 04:20:15.000000 arkdata-1.0.2/src/arkdata/seeds/users.json
+-rw-rw-rw-   0        0        0    29591 2023-03-30 03:43:50.000000 arkdata-1.0.2/src/arkdata/seeds/weapons.json
+drwxrwxrwx   0        0        0        0 2023-04-16 02:15:01.506217 arkdata-1.0.2/src/arkdata.egg-info/
+-rw-rw-rw-   0        0        0      650 2023-04-16 02:15:01.000000 arkdata-1.0.2/src/arkdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1948 2023-04-16 02:15:01.000000 arkdata-1.0.2/src/arkdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 02:15:01.000000 arkdata-1.0.2/src/arkdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      167 2023-04-16 02:15:01.000000 arkdata-1.0.2/src/arkdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-16 02:15:01.000000 arkdata-1.0.2/src/arkdata.egg-info/top_level.txt
```

### Comparing `arkdata-1.0.1/LICENSE` & `arkdata-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/PKG-INFO` & `arkdata-1.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkdata
-Version: 1.0.1
+Version: 1.0.2
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Data
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Data/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `arkdata-1.0.1/pyproject.toml` & `arkdata-1.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [build-system]
 requires = [
     "setuptools>=42",
     "wheel",
-    "arklibrary==1.*",
     "python-dotenv>=1.0.0",
     "SQLAlchemy>=2.0.9",
     "sqlalchemy_utils>=0.40.0",
     "flask>=2.2.3"
 ]
 build-backend = "setuptools.build_meta"
```

### Comparing `arkdata-1.0.1/setup.cfg` & `arkdata-1.0.2/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 726b 6461 7461 0d0a 7665 7273   = arkdata..vers
-00000020: 696f 6e20 3d20 312e 302e 310d 0a74 6573  ion = 1.0.1..tes
+00000020: 696f 6e20 3d20 312e 302e 320d 0a74 6573  ion = 1.0.2..tes
 00000030: 745f 7665 7273 696f 6e20 3d20 312e 302e  t_version = 1.0.
-00000040: 310d 0a70 726f 6475 6374 696f 6e5f 7665  1..production_ve
-00000050: 7273 696f 6e20 3d20 312e 302e 310d 0a61  rsion = 1.0.1..a
+00000040: 320d 0a70 726f 6475 6374 696f 6e5f 7665  2..production_ve
+00000050: 7273 696f 6e20 3d20 312e 302e 320d 0a61  rsion = 1.0.2..a
 00000060: 7574 686f 7220 3d20 4d61 7572 6963 696f  uthor = Mauricio
 00000070: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000080: 2064 6576 2e6d 6175 7269 6369 6f2e 6c6f   dev.mauricio.lo
 00000090: 6d65 6c69 4067 6d61 696c 2e63 6f6d 0d0a  meli@gmail.com..
 000000a0: 6465 7363 7269 7074 696f 6e20 3d20 5468  description = Th
 000000b0: 6973 2061 7070 6c69 6361 7469 6f6e 2061  is application a
 000000c0: 6363 6573 7365 7320 7468 6520 4172 6b20  ccesses the Ark 
@@ -41,38 +41,37 @@
 00000280: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
 00000290: 203d 200d 0a09 3d20 7372 630d 0a70 6163   = ...= src..pac
 000002a0: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
 000002b0: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
 000002c0: 203e 3d33 2e39 0d0a 696e 7374 616c 6c5f   >=3.9..install_
 000002d0: 7265 7175 6972 6573 203d 200d 0a09 7265  requires = ...re
 000002e0: 7175 6573 7473 3e3d 322e 3238 2e31 0d0a  quests>=2.28.1..
-000002f0: 0961 726b 6c69 6272 6172 793d 3d31 2e2a  .arklibrary==1.*
-00000300: 0d0a 0970 7974 686f 6e2d 646f 7465 6e76  ...python-dotenv
-00000310: 3e3d 312e 302e 300d 0a09 5351 4c41 6c63  >=1.0.0...SQLAlc
-00000320: 6865 6d79 3e3d 322e 302e 390d 0a09 7371  hemy>=2.0.9...sq
-00000330: 6c61 6c63 6865 6d79 5f75 7469 6c73 3e3d  lalchemy_utils>=
-00000340: 302e 3430 2e30 0d0a 0966 6c61 736b 3e3d  0.40.0...flask>=
-00000350: 322e 322e 330d 0a0d 0a5b 6f70 7469 6f6e  2.2.3....[option
-00000360: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
-00000370: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
-00000380: 0a5b 6f70 7469 6f6e 732e 6578 7472 6173  .[options.extras
-00000390: 5f72 6571 7569 7265 5d0d 0a74 6573 7469  _require]..testi
-000003a0: 6e67 203d 200d 0a09 7079 7465 7374 3e3d  ng = ...pytest>=
-000003b0: 362e 300d 0a09 7079 7465 7374 2d63 6f76  6.0...pytest-cov
-000003c0: 3e3d 322e 300d 0a09 6d79 7079 3e3d 302e  >=2.0...mypy>=0.
-000003d0: 3937 310d 0a09 666c 616b 6538 3e3d 332e  971...flake8>=3.
-000003e0: 390d 0a09 746f 783e 3d33 2e32 340d 0a0d  9...tox>=3.24...
-000003f0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-00000400: 655f 6461 7461 5d0d 0a61 726b 6461 7461  e_data]..arkdata
-00000410: 203d 200d 0a09 7079 2e74 7970 6564 0d0a   = ...py.typed..
-00000420: 0963 6f6e 6669 672e 696e 690d 0a61 726b  .config.ini..ark
-00000430: 6461 7461 2e73 6565 6473 203d 200d 0a09  data.seeds = ...
-00000440: 2a2e 6a73 6f6e 0d0a 6172 6b64 6174 612e  *.json..arkdata.
-00000450: 7365 6564 732e 6461 7461 203d 200d 0a09  seeds.data = ...
-00000460: 2a2e 6a73 6f6e 0d0a 6172 6b64 6174 612e  *.json..arkdata.
-00000470: 7365 6564 732e 7461 626c 6573 203d 200d  seeds.tables = .
-00000480: 0a09 2a2e 6a73 6f6e 0d0a 0d0a 5b66 6c61  ..*.json....[fla
-00000490: 6b65 385d 0d0a 6d61 782d 6c69 6e65 2d6c  ke8]..max-line-l
-000004a0: 656e 6774 6820 3d20 3136 300d 0a0d 0a5b  ength = 160....[
-000004b0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-000004c0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-000004d0: 6520 3d20 300d 0a0d 0a                   e = 0....
+000002f0: 0970 7974 686f 6e2d 646f 7465 6e76 3e3d  .python-dotenv>=
+00000300: 312e 302e 300d 0a09 5351 4c41 6c63 6865  1.0.0...SQLAlche
+00000310: 6d79 3e3d 322e 302e 390d 0a09 7371 6c61  my>=2.0.9...sqla
+00000320: 6c63 6865 6d79 5f75 7469 6c73 3e3d 302e  lchemy_utils>=0.
+00000330: 3430 2e30 0d0a 0966 6c61 736b 3e3d 322e  40.0...flask>=2.
+00000340: 322e 330d 0a0d 0a5b 6f70 7469 6f6e 732e  2.3....[options.
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
+000003f0: 6461 7461 5d0d 0a61 726b 6461 7461 203d  data]..arkdata =
+00000400: 200d 0a09 7079 2e74 7970 6564 0d0a 0963   ...py.typed...c
+00000410: 6f6e 6669 672e 696e 690d 0a61 726b 6461  onfig.ini..arkda
+00000420: 7461 2e73 6565 6473 203d 200d 0a09 2a2e  ta.seeds = ...*.
+00000430: 6a73 6f6e 0d0a 6172 6b64 6174 612e 7365  json..arkdata.se
+00000440: 6564 732e 6461 7461 203d 200d 0a09 2a2e  eds.data = ...*.
+00000450: 6a73 6f6e 0d0a 6172 6b64 6174 612e 7365  json..arkdata.se
+00000460: 6564 732e 7461 626c 6573 203d 200d 0a09  eds.tables = ...
+00000470: 2a2e 6a73 6f6e 0d0a 0d0a 5b66 6c61 6b65  *.json....[flake
+00000480: 385d 0d0a 6d61 782d 6c69 6e65 2d6c 656e  8]..max-line-len
+00000490: 6774 6820 3d20 3136 300d 0a0d 0a5b 6567  gth = 160....[eg
+000004a0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+000004b0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+000004c0: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `arkdata-1.0.1/src/arkdata/database/configuration.py` & `arkdata-1.0.2/src/arkdata/database/configuration.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/database/cursor.py` & `arkdata-1.0.2/src/arkdata/database/cursor.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/database/database.py` & `arkdata-1.0.2/src/arkdata/database/database.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/database/table.py` & `arkdata-1.0.2/src/arkdata/database/table.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/__init__.py` & `arkdata-1.0.2/src/arkdata/models/__init__.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/account.py` & `arkdata-1.0.2/src/arkdata/models/account.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/ammunition.py` & `arkdata-1.0.2/src/arkdata/models/ammunition.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/armour.py` & `arkdata-1.0.2/src/arkdata/models/armour.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/artifact.py` & `arkdata-1.0.2/src/arkdata/models/artifact.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/attachment.py` & `arkdata-1.0.2/src/arkdata/models/attachment.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/cart_item.py` & `arkdata-1.0.2/src/arkdata/models/cart_item.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/command.py` & `arkdata-1.0.2/src/arkdata/models/command.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/consumable.py` & `arkdata-1.0.2/src/arkdata/models/consumable.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/creature.py` & `arkdata-1.0.2/src/arkdata/models/creature.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/dye.py` & `arkdata-1.0.2/src/arkdata/models/dye.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/egg.py` & `arkdata-1.0.2/src/arkdata/models/egg.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/farm.py` & `arkdata-1.0.2/src/arkdata/models/farm.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/order_item.py` & `arkdata-1.0.2/src/arkdata/models/order_item.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/product.py` & `arkdata-1.0.2/src/arkdata/models/product.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/recipe.py` & `arkdata-1.0.2/src/arkdata/models/recipe.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/resource.py` & `arkdata-1.0.2/src/arkdata/models/resource.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/saddle.py` & `arkdata-1.0.2/src/arkdata/models/saddle.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/seed.py` & `arkdata-1.0.2/src/arkdata/models/seed.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/server.py` & `arkdata-1.0.2/src/arkdata/models/server.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/sessions.py` & `arkdata-1.0.2/src/arkdata/models/sessions.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/skin.py` & `arkdata-1.0.2/src/arkdata/models/skin.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/structure.py` & `arkdata-1.0.2/src/arkdata/models/structure.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/tool.py` & `arkdata-1.0.2/src/arkdata/models/tool.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/trophy.py` & `arkdata-1.0.2/src/arkdata/models/trophy.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/user.py` & `arkdata-1.0.2/src/arkdata/models/user.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/models/weapon.py` & `arkdata-1.0.2/src/arkdata/models/weapon.py`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/accounts.json` & `arkdata-1.0.2/src/arkdata/seeds/accounts.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/ammunitions.json` & `arkdata-1.0.2/src/arkdata/seeds/ammunitions.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/armours.json` & `arkdata-1.0.2/src/arkdata/seeds/armours.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/artifacts.json` & `arkdata-1.0.2/src/arkdata/seeds/artifacts.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/attachments.json` & `arkdata-1.0.2/src/arkdata/seeds/attachments.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/commands.json` & `arkdata-1.0.2/src/arkdata/seeds/commands.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/consumables.json` & `arkdata-1.0.2/src/arkdata/seeds/consumables.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/creatures.json` & `arkdata-1.0.2/src/arkdata/seeds/creatures.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/dyes.json` & `arkdata-1.0.2/src/arkdata/seeds/dyes.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/eggs.json` & `arkdata-1.0.2/src/arkdata/seeds/eggs.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/farms.json` & `arkdata-1.0.2/src/arkdata/seeds/farms.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/products.json` & `arkdata-1.0.2/src/arkdata/seeds/products.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/recipes.json` & `arkdata-1.0.2/src/arkdata/seeds/recipes.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/resources.json` & `arkdata-1.0.2/src/arkdata/seeds/resources.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/saddles.json` & `arkdata-1.0.2/src/arkdata/seeds/saddles.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/seeds.json` & `arkdata-1.0.2/src/arkdata/seeds/seeds.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/skins.json` & `arkdata-1.0.2/src/arkdata/seeds/skins.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/structures.json` & `arkdata-1.0.2/src/arkdata/seeds/structures.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/tools.json` & `arkdata-1.0.2/src/arkdata/seeds/tools.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/trophies.json` & `arkdata-1.0.2/src/arkdata/seeds/trophies.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/users.json` & `arkdata-1.0.2/src/arkdata/seeds/users.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata/seeds/weapons.json` & `arkdata-1.0.2/src/arkdata/seeds/weapons.json`

 * *Files identical despite different names*

### Comparing `arkdata-1.0.1/src/arkdata.egg-info/PKG-INFO` & `arkdata-1.0.2/src/arkdata.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkdata
-Version: 1.0.1
+Version: 1.0.2
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Data
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Data/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `arkdata-1.0.1/src/arkdata.egg-info/SOURCES.txt` & `arkdata-1.0.2/src/arkdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

