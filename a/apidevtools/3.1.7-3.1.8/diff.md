# Comparing `tmp/apidevtools-3.1.7.tar.gz` & `tmp/apidevtools-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidevtools-3.1.7.tar", last modified: Wed Apr  5 14:46:21 2023, max compression
+gzip compressed data, was "apidevtools-3.1.8.tar", last modified: Sun Apr 16 13:51:36 2023, max compression
```

## Comparing `apidevtools-3.1.7.tar` & `apidevtools-3.1.8.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 14:46:21.836152 apidevtools-3.1.7/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.1.7/LICENSE.txt
--rw-rw-rw-   0        0        0     3400 2023-04-05 14:46:21.836152 apidevtools-3.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      971 2023-03-21 22:01:37.000000 apidevtools-3.1.7/README.md
--rw-rw-rw-   0        0        0     1774 2023-04-05 14:46:06.000000 apidevtools-3.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-05 14:46:21.836152 apidevtools-3.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-05 14:46:21.774152 apidevtools-3.1.7/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.1.7/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:46:21.776152 apidevtools-3.1.7/src/apidevtools/
--rw-rw-rw-   0        0        0       71 2023-03-26 16:10:22.000000 apidevtools-3.1.7/src/apidevtools/__init__.py
--rw-rw-rw-   0        0        0      914 2023-02-27 15:21:15.000000 apidevtools-3.1.7/src/apidevtools/logman.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:46:21.796154 apidevtools-3.1.7/src/apidevtools/media/
--rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.1.7/src/apidevtools/media/__init__.py
--rw-rw-rw-   0        0        0     3846 2023-03-14 23:04:59.000000 apidevtools-3.1.7/src/apidevtools/media/imgproc.py
--rw-rw-rw-   0        0        0     1104 2023-03-14 23:15:32.000000 apidevtools-3.1.7/src/apidevtools/media/telegraph.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:46:21.799166 apidevtools-3.1.7/src/apidevtools/security/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/security/__init__.py
--rw-rw-rw-   0        0        0      697 2023-03-27 23:36:30.000000 apidevtools-3.1.7/src/apidevtools/security/encryptor.py
--rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.1.7/src/apidevtools/security/hasher.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:46:21.803152 apidevtools-3.1.7/src/apidevtools/simpleorm/
--rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.1.7/src/apidevtools/simpleorm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:46:21.808152 apidevtools-3.1.7/src/apidevtools/simpleorm/connectors/
--rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.1.7/src/apidevtools/simpleorm/connectors/__init__.py
--rw-rw-rw-   0        0        0     3357 2023-03-21 23:35:42.000000 apidevtools-3.1.7/src/apidevtools/simpleorm/connectors/_connector.py
--rw-rw-rw-   0        0        0     4793 2023-03-21 23:30:17.000000 apidevtools-3.1.7/src/apidevtools/simpleorm/connectors/mysql.py
--rw-rw-rw-   0        0        0     4446 2023-03-21 23:26:07.000000 apidevtools-3.1.7/src/apidevtools/simpleorm/connectors/postgresql.py
--rw-rw-rw-   0        0        0     3287 2023-03-21 21:53:42.000000 apidevtools-3.1.7/src/apidevtools/simpleorm/connectors/sqlite.py
--rw-rw-rw-   0        0        0     5532 2023-04-05 14:28:09.000000 apidevtools-3.1.7/src/apidevtools/simpleorm/orm.py
--rw-rw-rw-   0        0        0     1792 2023-03-29 11:40:43.000000 apidevtools-3.1.7/src/apidevtools/simpleorm/redis.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:46:21.811154 apidevtools-3.1.7/src/apidevtools/simpleorm/types/
--rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.1.7/src/apidevtools/simpleorm/types/__init__.py
--rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.1.7/src/apidevtools/simpleorm/types/records.py
--rw-rw-rw-   0        0        0      772 2023-03-28 00:36:31.000000 apidevtools-3.1.7/src/apidevtools/simpleorm/types/schema.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:46:21.819155 apidevtools-3.1.7/src/apidevtools/template/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/template/__init__.py
--rw-rw-rw-   0        0        0      746 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/template/create.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:46:21.768152 apidevtools-3.1.7/src/apidevtools/template/template/
-drwxrwxrwx   0        0        0        0 2023-04-05 14:46:21.820152 apidevtools-3.1.7/src/apidevtools/template/template/api/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/template/template/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:46:21.822152 apidevtools-3.1.7/src/apidevtools/template/template/api/build/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/template/template/api/build/__init__.py
--rw-rw-rw-   0        0        0      306 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/template/template/api/build/compose.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:46:21.824152 apidevtools-3.1.7/src/apidevtools/template/template/api/src/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/template/template/api/src/__init__.py
--rw-rw-rw-   0        0        0     1105 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/template/template/api/src/app.py
--rw-rw-rw-   0        0        0     1210 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/template/template/api/src/const.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:46:21.828152 apidevtools-3.1.7/src/apidevtools/template/template/api/src/crud/
--rw-rw-rw-   0        0        0       63 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/template/template/api/src/crud/__init__.py
--rw-rw-rw-   0        0        0     1334 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/template/template/api/src/crud/auth.py
--rw-rw-rw-   0        0        0     1212 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/template/template/api/src/crud/item.py
--rw-rw-rw-   0        0        0     1601 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/template/template/api/src/crud/user.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:46:21.832153 apidevtools-3.1.7/src/apidevtools/template/template/api/src/routers/
--rw-rw-rw-   0        0        0      123 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/template/template/api/src/routers/__init__.py
--rw-rw-rw-   0        0        0      835 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/template/template/api/src/routers/auth.py
--rw-rw-rw-   0        0        0     1726 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/template/template/api/src/routers/item.py
--rw-rw-rw-   0        0        0     2300 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/template/template/api/src/routers/user.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:46:21.835155 apidevtools-3.1.7/src/apidevtools/template/template/api/src/schemas/
--rw-rw-rw-   0        0        0       42 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/template/template/api/src/schemas/__init__.py
--rw-rw-rw-   0        0        0      387 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/template/template/api/src/schemas/item.py
--rw-rw-rw-   0        0        0      547 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/template/template/api/src/schemas/user.py
--rw-rw-rw-   0        0        0    26020 2023-02-26 16:41:50.000000 apidevtools-3.1.7/src/apidevtools/template/template.zip
--rw-rw-rw-   0        0        0     1006 2023-04-05 13:54:15.000000 apidevtools-3.1.7/src/apidevtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:46:21.793155 apidevtools-3.1.7/src/apidevtools.egg-info/
--rw-rw-rw-   0        0        0     3400 2023-04-05 14:46:21.000000 apidevtools-3.1.7/src/apidevtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2079 2023-04-05 14:46:21.000000 apidevtools-3.1.7/src/apidevtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 14:46:21.000000 apidevtools-3.1.7/src/apidevtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-04-05 14:46:21.000000 apidevtools-3.1.7/src/apidevtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-05 14:46:21.000000 apidevtools-3.1.7/src/apidevtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.265046 apidevtools-3.1.8/
+-rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     3400 2023-04-16 13:51:36.264047 apidevtools-3.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2023-03-21 22:01:37.000000 apidevtools-3.1.8/README.md
+-rw-rw-rw-   0        0        0     1774 2023-04-16 13:51:17.000000 apidevtools-3.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 13:51:36.265046 apidevtools-3.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.027391 apidevtools-3.1.8/src/
+-rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.1.8/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.045471 apidevtools-3.1.8/src/apidevtools/
+-rw-rw-rw-   0        0        0       71 2023-03-26 16:10:22.000000 apidevtools-3.1.8/src/apidevtools/__init__.py
+-rw-rw-rw-   0        0        0      914 2023-02-27 15:21:15.000000 apidevtools-3.1.8/src/apidevtools/logman.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.076920 apidevtools-3.1.8/src/apidevtools/media/
+-rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.1.8/src/apidevtools/media/__init__.py
+-rw-rw-rw-   0        0        0     3846 2023-03-14 23:04:59.000000 apidevtools-3.1.8/src/apidevtools/media/imgproc.py
+-rw-rw-rw-   0        0        0     1104 2023-03-14 23:15:32.000000 apidevtools-3.1.8/src/apidevtools/media/telegraph.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.093249 apidevtools-3.1.8/src/apidevtools/security/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/security/__init__.py
+-rw-rw-rw-   0        0        0      697 2023-04-05 15:55:54.000000 apidevtools-3.1.8/src/apidevtools/security/encryptor.py
+-rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.1.8/src/apidevtools/security/hasher.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.113512 apidevtools-3.1.8/src/apidevtools/simpleorm/
+-rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.148867 apidevtools-3.1.8/src/apidevtools/simpleorm/connectors/
+-rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/connectors/__init__.py
+-rw-rw-rw-   0        0        0     3357 2023-03-21 23:35:42.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/connectors/_connector.py
+-rw-rw-rw-   0        0        0     4793 2023-03-21 23:30:17.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/connectors/mysql.py
+-rw-rw-rw-   0        0        0     4446 2023-03-21 23:26:07.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/connectors/postgresql.py
+-rw-rw-rw-   0        0        0     3287 2023-03-21 21:53:42.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/connectors/sqlite.py
+-rw-rw-rw-   0        0        0     5532 2023-04-05 14:28:09.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/orm.py
+-rw-rw-rw-   0        0        0     1792 2023-03-29 11:40:43.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/redis.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.165867 apidevtools-3.1.8/src/apidevtools/simpleorm/types/
+-rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/types/__init__.py
+-rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/types/records.py
+-rw-rw-rw-   0        0        0      772 2023-03-28 00:36:31.000000 apidevtools-3.1.8/src/apidevtools/simpleorm/types/schema.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.178870 apidevtools-3.1.8/src/apidevtools/template/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/__init__.py
+-rw-rw-rw-   0        0        0      746 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/create.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.021390 apidevtools-3.1.8/src/apidevtools/template/template/
+drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.179870 apidevtools-3.1.8/src/apidevtools/template/template/api/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.185870 apidevtools-3.1.8/src/apidevtools/template/template/api/build/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/build/__init__.py
+-rw-rw-rw-   0        0        0      306 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/build/compose.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.200941 apidevtools-3.1.8/src/apidevtools/template/template/api/src/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/__init__.py
+-rw-rw-rw-   0        0        0     1105 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/app.py
+-rw-rw-rw-   0        0        0     1210 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/const.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.223940 apidevtools-3.1.8/src/apidevtools/template/template/api/src/crud/
+-rw-rw-rw-   0        0        0       63 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/crud/__init__.py
+-rw-rw-rw-   0        0        0     1334 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/crud/auth.py
+-rw-rw-rw-   0        0        0     1212 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/crud/item.py
+-rw-rw-rw-   0        0        0     1601 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/crud/user.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.248050 apidevtools-3.1.8/src/apidevtools/template/template/api/src/routers/
+-rw-rw-rw-   0        0        0      123 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/routers/__init__.py
+-rw-rw-rw-   0        0        0      835 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/routers/auth.py
+-rw-rw-rw-   0        0        0     1726 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/routers/item.py
+-rw-rw-rw-   0        0        0     2300 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/routers/user.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.263046 apidevtools-3.1.8/src/apidevtools/template/template/api/src/schemas/
+-rw-rw-rw-   0        0        0       42 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/schemas/__init__.py
+-rw-rw-rw-   0        0        0      387 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/schemas/item.py
+-rw-rw-rw-   0        0        0      547 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template/api/src/schemas/user.py
+-rw-rw-rw-   0        0        0    26020 2023-02-26 16:41:50.000000 apidevtools-3.1.8/src/apidevtools/template/template.zip
+-rw-rw-rw-   0        0        0     1154 2023-04-05 15:54:39.000000 apidevtools-3.1.8/src/apidevtools/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:51:36.063699 apidevtools-3.1.8/src/apidevtools.egg-info/
+-rw-rw-rw-   0        0        0     3400 2023-04-16 13:51:35.000000 apidevtools-3.1.8/src/apidevtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2079 2023-04-16 13:51:36.000000 apidevtools-3.1.8/src/apidevtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 13:51:35.000000 apidevtools-3.1.8/src/apidevtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-04-16 13:51:35.000000 apidevtools-3.1.8/src/apidevtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-16 13:51:36.000000 apidevtools-3.1.8/src/apidevtools.egg-info/top_level.txt
```

### Comparing `apidevtools-3.1.7/LICENSE.txt` & `apidevtools-3.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/PKG-INFO` & `apidevtools-3.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.1.7
+Version: 3.1.8
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.1.7/README.md` & `apidevtools-3.1.8/README.md`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/pyproject.toml` & `apidevtools-3.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apidevtools"
-version = "3.1.7"
+version = "3.1.8"
 authors = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 maintainers = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 description = "All in one tools for API development."
```

### Comparing `apidevtools-3.1.7/src/apidevtools/logman.py` & `apidevtools-3.1.8/src/apidevtools/logman.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/media/imgproc.py` & `apidevtools-3.1.8/src/apidevtools/media/imgproc.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/media/telegraph.py` & `apidevtools-3.1.8/src/apidevtools/media/telegraph.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/security/encryptor.py` & `apidevtools-3.1.8/src/apidevtools/security/encryptor.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/security/hasher.py` & `apidevtools-3.1.8/src/apidevtools/security/hasher.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/simpleorm/connectors/_connector.py` & `apidevtools-3.1.8/src/apidevtools/simpleorm/connectors/_connector.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/simpleorm/connectors/mysql.py` & `apidevtools-3.1.8/src/apidevtools/simpleorm/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/simpleorm/connectors/postgresql.py` & `apidevtools-3.1.8/src/apidevtools/simpleorm/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/simpleorm/connectors/sqlite.py` & `apidevtools-3.1.8/src/apidevtools/simpleorm/connectors/sqlite.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/simpleorm/orm.py` & `apidevtools-3.1.8/src/apidevtools/simpleorm/orm.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/simpleorm/redis.py` & `apidevtools-3.1.8/src/apidevtools/simpleorm/redis.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/simpleorm/types/records.py` & `apidevtools-3.1.8/src/apidevtools/simpleorm/types/records.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/simpleorm/types/schema.py` & `apidevtools-3.1.8/src/apidevtools/simpleorm/types/schema.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/template/create.py` & `apidevtools-3.1.8/src/apidevtools/template/create.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/template/template/api/src/app.py` & `apidevtools-3.1.8/src/apidevtools/template/template/api/src/app.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/template/template/api/src/const.py` & `apidevtools-3.1.8/src/apidevtools/template/template/api/src/const.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/template/template/api/src/crud/auth.py` & `apidevtools-3.1.8/src/apidevtools/template/template/api/src/crud/auth.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/template/template/api/src/crud/item.py` & `apidevtools-3.1.8/src/apidevtools/template/template/api/src/crud/item.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/template/template/api/src/crud/user.py` & `apidevtools-3.1.8/src/apidevtools/template/template/api/src/crud/user.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/template/template/api/src/routers/auth.py` & `apidevtools-3.1.8/src/apidevtools/template/template/api/src/routers/auth.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/template/template/api/src/routers/item.py` & `apidevtools-3.1.8/src/apidevtools/template/template/api/src/routers/item.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/template/template/api/src/routers/user.py` & `apidevtools-3.1.8/src/apidevtools/template/template/api/src/routers/user.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/template/template/api/src/schemas/user.py` & `apidevtools-3.1.8/src/apidevtools/template/template/api/src/schemas/user.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/template/template.zip` & `apidevtools-3.1.8/src/apidevtools/template/template.zip`

 * *Files identical despite different names*

### Comparing `apidevtools-3.1.7/src/apidevtools/utils.py` & `apidevtools-3.1.8/src/apidevtools/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,16 +3,22 @@
 import datetime
 
 
 INF: int = 2147483647
 LIMIT: int = 100
 
 
-def utcnow() -> datetime.datetime:
-    return datetime.datetime.utcnow()
+def now_tz_aware() -> datetime.datetime:
+    return datetime.datetime.now(datetime.timezone.utc)
+
+
+def now_tz_naive() -> datetime.datetime:
+    dt = datetime.datetime.now()
+    dt.replace(tzinfo=None)
+    return dt
 
 
 def evaluate(value: bytes, convert: bool = True) -> Any:
     """
     normal ast.literal_eval with a fix of known error together wit adaptation to the apidevtools package
     :param value:
     :param convert:
```

### Comparing `apidevtools-3.1.7/src/apidevtools.egg-info/PKG-INFO` & `apidevtools-3.1.8/src/apidevtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.1.7
+Version: 3.1.8
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.1.7/src/apidevtools.egg-info/SOURCES.txt` & `apidevtools-3.1.8/src/apidevtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

