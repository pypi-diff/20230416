# Comparing `tmp/apidevtools-3.1.8.tar.gz` & `tmp/apidevtools-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidevtools-3.1.8.tar", last modified: Sun Apr 16 13:51:36 2023, max compression
+gzip compressed data, was "apidevtools-3.1.9.tar", last modified: Sun Apr 16 14:10:18 2023, max compression
```

## Comparing `apidevtools-3.1.8.tar` & `apidevtools-3.1.9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.265046 apidevtools-3.1.8/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0     3400 2023-04-16 13:51:36.264047 apidevtools-3.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      971 2023-03-21 22:01:37.000000 apidevtools-3.1.8/README.md
--rw-rw-rw-   0        0        0     1774 2023-04-16 13:51:17.000000 apidevtools-3.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 13:51:36.265046 apidevtools-3.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.027391 apidevtools-3.1.8/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.1.8/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.045471 apidevtools-3.1.8/src/apidevtools/
--rw-rw-rw-   0        0        0       71 2023-03-26 16:10:22.000000 apidevtools-3.1.8/src/apidevtools/__init__.py
--rw-rw-rw-   0        0        0      914 2023-02-27 15:21:15.000000 apidevtools-3.1.8/src/apidevtools/logman.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.076920 apidevtools-3.1.8/src/apidevtools/media/
--rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.1.8/src/apidevtools/media/__init__.py
--rw-rw-rw-   0        0        0     3846 2023-03-14 23:04:59.000000 apidevtools-3.1.8/src/apidevtools/media/imgproc.py
--rw-rw-rw-   0        0        0     1104 2023-03-14 23:15:32.000000 apidevtools-3.1.8/src/apidevtools/media/telegraph.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.093249 apidevtools-3.1.8/src/apidevtools/security/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/security/__init__.py
--rw-rw-rw-   0        0        0      697 2023-04-05 15:55:54.000000 apidevtools-3.1.8/src/apidevtools/security/encryptor.py
--rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.1.8/src/apidevtools/security/hasher.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.113512 apidevtools-3.1.8/src/apidevtools/simpleorm/
--rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.148867 apidevtools-3.1.8/src/apidevtools/simpleorm/connectors/
--rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/connectors/__init__.py
--rw-rw-rw-   0        0        0     3357 2023-03-21 23:35:42.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/connectors/_connector.py
--rw-rw-rw-   0        0        0     4793 2023-03-21 23:30:17.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/connectors/mysql.py
--rw-rw-rw-   0        0        0     4446 2023-03-21 23:26:07.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/connectors/postgresql.py
--rw-rw-rw-   0        0        0     3287 2023-03-21 21:53:42.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/connectors/sqlite.py
--rw-rw-rw-   0        0        0     5532 2023-04-05 14:28:09.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/orm.py
--rw-rw-rw-   0        0        0     1792 2023-03-29 11:40:43.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/redis.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.165867 apidevtools-3.1.8/src/apidevtools/simpleorm/types/
--rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/types/__init__.py
--rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/types/records.py
--rw-rw-rw-   0        0        0      772 2023-03-28 00:36:31.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/types/schema.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.178870 apidevtools-3.1.8/src/apidevtools/template/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/__init__.py
--rw-rw-rw-   0        0        0      746 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/create.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.021390 apidevtools-3.1.8/src/apidevtools/template/template/
-drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.179870 apidevtools-3.1.8/src/apidevtools/template/template/api/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.185870 apidevtools-3.1.8/src/apidevtools/template/template/api/build/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/build/__init__.py
--rw-rw-rw-   0        0        0      306 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/build/compose.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.200941 apidevtools-3.1.8/src/apidevtools/template/template/api/src/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/__init__.py
--rw-rw-rw-   0        0        0     1105 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/app.py
--rw-rw-rw-   0        0        0     1210 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/const.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.223940 apidevtools-3.1.8/src/apidevtools/template/template/api/src/crud/
--rw-rw-rw-   0        0        0       63 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/crud/__init__.py
--rw-rw-rw-   0        0        0     1334 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/crud/auth.py
--rw-rw-rw-   0        0        0     1212 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/crud/item.py
--rw-rw-rw-   0        0        0     1601 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/crud/user.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.248050 apidevtools-3.1.8/src/apidevtools/template/template/api/src/routers/
--rw-rw-rw-   0        0        0      123 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/routers/__init__.py
--rw-rw-rw-   0        0        0      835 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/routers/auth.py
--rw-rw-rw-   0        0        0     1726 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/routers/item.py
--rw-rw-rw-   0        0        0     2300 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/routers/user.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.263046 apidevtools-3.1.8/src/apidevtools/template/template/api/src/schemas/
--rw-rw-rw-   0        0        0       42 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/schemas/__init__.py
--rw-rw-rw-   0        0        0      387 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/schemas/item.py
--rw-rw-rw-   0        0        0      547 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/schemas/user.py
--rw-rw-rw-   0        0        0    26020 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template.zip
--rw-rw-rw-   0        0        0     1154 2023-04-05 15:54:39.000000 apidevtools-3.1.8/src/apidevtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.063699 apidevtools-3.1.8/src/apidevtools.egg-info/
--rw-rw-rw-   0        0        0     3400 2023-04-16 13:51:35.000000 apidevtools-3.1.8/src/apidevtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2079 2023-04-16 13:51:36.000000 apidevtools-3.1.8/src/apidevtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 13:51:35.000000 apidevtools-3.1.8/src/apidevtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-16 13:51:35.000000 apidevtools-3.1.8/src/apidevtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-16 13:51:36.000000 apidevtools-3.1.8/src/apidevtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 14:10:18.542511 apidevtools-3.1.9/
+-rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     3400 2023-04-16 14:10:18.541512 apidevtools-3.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2023-03-21 22:01:37.000000 apidevtools-3.1.9/README.md
+-rw-rw-rw-   0        0        0     1774 2023-04-16 14:09:59.000000 apidevtools-3.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 14:10:18.542511 apidevtools-3.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 14:10:18.495512 apidevtools-3.1.9/src/
+-rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.1.9/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:10:18.498516 apidevtools-3.1.9/src/apidevtools/
+-rw-rw-rw-   0        0        0       71 2023-03-26 16:10:22.000000 apidevtools-3.1.9/src/apidevtools/__init__.py
+-rw-rw-rw-   0        0        0      914 2023-02-27 15:21:15.000000 apidevtools-3.1.9/src/apidevtools/logman.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:10:18.512512 apidevtools-3.1.9/src/apidevtools/media/
+-rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.1.9/src/apidevtools/media/__init__.py
+-rw-rw-rw-   0        0        0     3846 2023-03-14 23:04:59.000000 apidevtools-3.1.9/src/apidevtools/media/imgproc.py
+-rw-rw-rw-   0        0        0     1104 2023-03-14 23:15:32.000000 apidevtools-3.1.9/src/apidevtools/media/telegraph.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:10:18.515512 apidevtools-3.1.9/src/apidevtools/security/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/security/__init__.py
+-rw-rw-rw-   0        0        0      697 2023-04-05 15:55:54.000000 apidevtools-3.1.9/src/apidevtools/security/encryptor.py
+-rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.1.9/src/apidevtools/security/hasher.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:10:18.517514 apidevtools-3.1.9/src/apidevtools/simpleorm/
+-rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.1.9/src/apidevtools/simpleorm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:10:18.522512 apidevtools-3.1.9/src/apidevtools/simpleorm/connectors/
+-rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.1.9/src/apidevtools/simpleorm/connectors/__init__.py
+-rw-rw-rw-   0        0        0     3357 2023-03-21 23:35:42.000000 apidevtools-3.1.9/src/apidevtools/simpleorm/connectors/_connector.py
+-rw-rw-rw-   0        0        0     4793 2023-03-21 23:30:17.000000 apidevtools-3.1.9/src/apidevtools/simpleorm/connectors/mysql.py
+-rw-rw-rw-   0        0        0     4446 2023-03-21 23:26:07.000000 apidevtools-3.1.9/src/apidevtools/simpleorm/connectors/postgresql.py
+-rw-rw-rw-   0        0        0     3287 2023-03-21 21:53:42.000000 apidevtools-3.1.9/src/apidevtools/simpleorm/connectors/sqlite.py
+-rw-rw-rw-   0        0        0     5896 2023-04-16 14:09:49.000000 apidevtools-3.1.9/src/apidevtools/simpleorm/orm.py
+-rw-rw-rw-   0        0        0     1792 2023-03-29 11:40:43.000000 apidevtools-3.1.9/src/apidevtools/simpleorm/redis.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:10:18.524512 apidevtools-3.1.9/src/apidevtools/simpleorm/types/
+-rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.1.9/src/apidevtools/simpleorm/types/__init__.py
+-rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.1.9/src/apidevtools/simpleorm/types/records.py
+-rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.1.9/src/apidevtools/simpleorm/types/schema.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:10:18.526512 apidevtools-3.1.9/src/apidevtools/template/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/template/__init__.py
+-rw-rw-rw-   0        0        0      746 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/template/create.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:10:18.490512 apidevtools-3.1.9/src/apidevtools/template/template/
+drwxrwxrwx   0        0        0        0 2023-04-16 14:10:18.527512 apidevtools-3.1.9/src/apidevtools/template/template/api/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/template/template/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:10:18.529512 apidevtools-3.1.9/src/apidevtools/template/template/api/build/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/template/template/api/build/__init__.py
+-rw-rw-rw-   0        0        0      306 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/template/template/api/build/compose.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:10:18.531512 apidevtools-3.1.9/src/apidevtools/template/template/api/src/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/template/template/api/src/__init__.py
+-rw-rw-rw-   0        0        0     1105 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/template/template/api/src/app.py
+-rw-rw-rw-   0        0        0     1210 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/template/template/api/src/const.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:10:18.534512 apidevtools-3.1.9/src/apidevtools/template/template/api/src/crud/
+-rw-rw-rw-   0        0        0       63 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/template/template/api/src/crud/__init__.py
+-rw-rw-rw-   0        0        0     1334 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/template/template/api/src/crud/auth.py
+-rw-rw-rw-   0        0        0     1212 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/template/template/api/src/crud/item.py
+-rw-rw-rw-   0        0        0     1601 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/template/template/api/src/crud/user.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:10:18.538512 apidevtools-3.1.9/src/apidevtools/template/template/api/src/routers/
+-rw-rw-rw-   0        0        0      123 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/template/template/api/src/routers/__init__.py
+-rw-rw-rw-   0        0        0      835 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/template/template/api/src/routers/auth.py
+-rw-rw-rw-   0        0        0     1726 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/template/template/api/src/routers/item.py
+-rw-rw-rw-   0        0        0     2300 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/template/template/api/src/routers/user.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:10:18.540512 apidevtools-3.1.9/src/apidevtools/template/template/api/src/schemas/
+-rw-rw-rw-   0        0        0       42 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/template/template/api/src/schemas/__init__.py
+-rw-rw-rw-   0        0        0      387 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/template/template/api/src/schemas/item.py
+-rw-rw-rw-   0        0        0      547 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/template/template/api/src/schemas/user.py
+-rw-rw-rw-   0        0        0    26020 2023-02-26 16:41:50.000000 apidevtools-3.1.9/src/apidevtools/template/template.zip
+-rw-rw-rw-   0        0        0     1154 2023-04-05 15:54:39.000000 apidevtools-3.1.9/src/apidevtools/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:10:18.509512 apidevtools-3.1.9/src/apidevtools.egg-info/
+-rw-rw-rw-   0        0        0     3400 2023-04-16 14:10:18.000000 apidevtools-3.1.9/src/apidevtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2079 2023-04-16 14:10:18.000000 apidevtools-3.1.9/src/apidevtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 14:10:18.000000 apidevtools-3.1.9/src/apidevtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-16 14:10:18.000000 apidevtools-3.1.9/src/apidevtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-16 14:10:18.000000 apidevtools-3.1.9/src/apidevtools.egg-info/top_level.txt
```

### Comparing `apidevtools-3.1.8/LICENSE.txt` & `apidevtools-3.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/PKG-INFO` & `apidevtools-3.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.1.8
+Version: 3.1.9
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.1.8/README.md` & `apidevtools-3.1.9/README.md`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/pyproject.toml` & `apidevtools-3.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apidevtools"
-version = "3.1.8"
+version = "3.1.9"
 authors = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 maintainers = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 description = "All in one tools for API development."
```

### Comparing `apidevtools-3.1.8/src/apidevtools/logman.py` & `apidevtools-3.1.9/src/apidevtools/logman.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/media/imgproc.py` & `apidevtools-3.1.9/src/apidevtools/media/imgproc.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/media/telegraph.py` & `apidevtools-3.1.9/src/apidevtools/media/telegraph.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/security/encryptor.py` & `apidevtools-3.1.9/src/apidevtools/security/encryptor.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/security/hasher.py` & `apidevtools-3.1.9/src/apidevtools/security/hasher.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/simpleorm/connectors/_connector.py` & `apidevtools-3.1.9/src/apidevtools/simpleorm/connectors/_connector.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/simpleorm/connectors/mysql.py` & `apidevtools-3.1.9/src/apidevtools/simpleorm/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/simpleorm/connectors/postgresql.py` & `apidevtools-3.1.9/src/apidevtools/simpleorm/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/simpleorm/connectors/sqlite.py` & `apidevtools-3.1.9/src/apidevtools/simpleorm/connectors/sqlite.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/simpleorm/orm.py` & `apidevtools-3.1.9/src/apidevtools/simpleorm/orm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from loguru._logger import Logger
 from typing import Any
 import loguru
+import inspect as _inspect
 
 from ..utils import INF, is_dict as _is_dict
 from .types import RecordType, Record, Schema, Records, Relation, Instance
 from .connectors._connector import Connector
 
 
 class ORM:
@@ -70,14 +71,16 @@
             *, rel_depth: int = 0, del_depth: int = INF
     ) -> Records:
         instance, tablename = await self.__parse_parameters(instance, tablename)
         query, args = await self.connector._constructor__select_instances(instance, tablename)
         records = await self.select(query, args, record_t)
         if del_depth and _is_dict(record_t):
             self.logger.warning(f'`record_t` is not `Schema` ({record_t}) but `del_depth` is set to {del_depth}')
+        if rel_depth and _is_dict(record_t):
+            self.logger.warning(f'`record_t` is not `Schema` ({record_t}) but `rel_depth` is set to {rel_depth}')
         for index, record in enumerate(await records.all()) if not _is_dict(record_t) and del_depth else ():
             for relation in record.relations():
                 instances = await (await self.delete(
                     relation.where, relation.rel_schema_t, relation.rel_schema_t.__tablename__, del_depth=del_depth - 1
                 )).all()
                 if rel_depth:
                     records = await self.__attach_instances(records, record, relation, instances, index)
@@ -98,15 +101,19 @@
 
     async def __parse_parameters(
             self,
             instance: Instance, tablename: str
     ) -> tuple[dict[str, Any], str]:
         if isinstance(instance, Schema):
             tablename = instance.__tablename__
+            noupdate = instance.__noupdate__
             instance = dict(await instance.into_db())
+            if _inspect.stack()[1][3] == 'update':
+                for key in noupdate:
+                    instance.pop(key)
         if not tablename:
             raise AttributeError('Specify "tablename" if "instance" is a "dict", otherwise pass "Schema" object')
         db_columns = await self.connector.columns(tablename)
         instance_columns = set(instance.keys())
         columns = instance_columns.intersection(db_columns)
         for key in instance_columns.difference(db_columns):
             if key not in columns:
```

### Comparing `apidevtools-3.1.8/src/apidevtools/simpleorm/redis.py` & `apidevtools-3.1.9/src/apidevtools/simpleorm/redis.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/simpleorm/types/records.py` & `apidevtools-3.1.9/src/apidevtools/simpleorm/types/records.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/simpleorm/types/schema.py` & `apidevtools-3.1.9/src/apidevtools/simpleorm/types/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
         self.ext_schema_t: type['Schema'] = ext_schema_t
         self.propname: str = propname
         self.rel_schema_t: type['Schema'] = rel_schema_t
         self.where: dict[str, Any] = where
 
 
 class Schema(BaseModel, ABC):
+    __noupdate__ = []
+
     @property
     @_abstractmethod
     def __tablename__(self) -> str:
         ...
 
     def relations(self) -> list[Relation]:
         return []
```

### Comparing `apidevtools-3.1.8/src/apidevtools/template/create.py` & `apidevtools-3.1.9/src/apidevtools/template/create.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/template/template/api/src/app.py` & `apidevtools-3.1.9/src/apidevtools/template/template/api/src/app.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/template/template/api/src/const.py` & `apidevtools-3.1.9/src/apidevtools/template/template/api/src/const.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/template/template/api/src/crud/auth.py` & `apidevtools-3.1.9/src/apidevtools/template/template/api/src/crud/auth.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/template/template/api/src/crud/item.py` & `apidevtools-3.1.9/src/apidevtools/template/template/api/src/crud/item.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/template/template/api/src/crud/user.py` & `apidevtools-3.1.9/src/apidevtools/template/template/api/src/crud/user.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/template/template/api/src/routers/auth.py` & `apidevtools-3.1.9/src/apidevtools/template/template/api/src/routers/auth.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/template/template/api/src/routers/item.py` & `apidevtools-3.1.9/src/apidevtools/template/template/api/src/routers/item.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/template/template/api/src/routers/user.py` & `apidevtools-3.1.9/src/apidevtools/template/template/api/src/routers/user.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/template/template/api/src/schemas/user.py` & `apidevtools-3.1.9/src/apidevtools/template/template/api/src/schemas/user.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/template/template.zip` & `apidevtools-3.1.9/src/apidevtools/template/template.zip`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools/utils.py` & `apidevtools-3.1.9/src/apidevtools/utils.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.8/src/apidevtools.egg-info/PKG-INFO` & `apidevtools-3.1.9/src/apidevtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.1.8
+Version: 3.1.9
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.1.8/src/apidevtools.egg-info/SOURCES.txt` & `apidevtools-3.1.9/src/apidevtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

