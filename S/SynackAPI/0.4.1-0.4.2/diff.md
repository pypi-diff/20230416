# Comparing `tmp/SynackAPI-0.4.1.tar.gz` & `tmp/SynackAPI-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SynackAPI-0.4.1.tar", last modified: Wed Feb  8 15:47:34 2023, max compression
+gzip compressed data, was "SynackAPI-0.4.2.tar", last modified: Sun Apr 16 04:21:15 2023, max compression
```

## Comparing `SynackAPI-0.4.1.tar` & `SynackAPI-0.4.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:47:34.003970 SynackAPI-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-02-08 15:47:34.003970 SynackAPI-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 15:47:34.003970 SynackAPI-0.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:47:33.999970 SynackAPI-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:47:33.999970 SynackAPI-0.4.1/src/SynackAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-02-08 15:47:33.000000 SynackAPI-0.4.1/src/SynackAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-02-08 15:47:33.000000 SynackAPI-0.4.1/src/SynackAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 15:47:33.000000 SynackAPI-0.4.1/src/SynackAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-02-08 15:47:33.000000 SynackAPI-0.4.1/src/SynackAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-08 15:47:33.000000 SynackAPI-0.4.1/src/SynackAPI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:47:33.999970 SynackAPI-0.4.1/src/synack/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:47:33.999970 SynackAPI-0.4.1/src/synack/db/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:47:33.999970 SynackAPI-0.4.1/src/synack/db/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/db/alembic/README
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/db/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/db/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/db/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:47:33.999970 SynackAPI-0.4.1/src/synack/db/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/db/alembic/versions/0c1ac7be711c_added_url_table_deleted_url_from_port_.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/db/alembic/versions/349c447c0d37_added_use_scratchspace_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/db/alembic/versions/355984ba030b_added_notification_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/db/alembic/versions/649443e08834_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/db/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/db/alembic/versions/deb7dd07212c_added_ip_port_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/db/alembic.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:47:34.003970 SynackAPI-0.4.1/src/synack/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/db/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      447 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/db/models/category.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1579 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/db/models/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/db/models/ip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/db/models/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/db/models/port.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1059 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/db/models/target.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/db/models/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:47:34.003970 SynackAPI-0.4.1/src/synack/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/plugins/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/plugins/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/plugins/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/plugins/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17777 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/plugins/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/plugins/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/plugins/hydra.py
--rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/plugins/missions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/plugins/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/plugins/scratchspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    12304 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/plugins/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/plugins/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/plugins/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/src/synack/plugins/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 15:47:34.003970 SynackAPI-0.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/test/test_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    42898 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/test/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/test/test_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/test/test_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/test/test_hydra.py
--rw-r--r--   0 runner    (1001) docker     (123)    16680 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/test/test_missions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/test/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/test/test_scratchspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/test/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    36005 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/test/test_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/test/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/test/test_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-02-08 15:47:31.000000 SynackAPI-0.4.1/test/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:15.855337 SynackAPI-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-16 04:21:15.855337 SynackAPI-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 04:21:15.855337 SynackAPI-0.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:15.839337 SynackAPI-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:15.843337 SynackAPI-0.4.2/src/SynackAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-16 04:21:15.000000 SynackAPI-0.4.2/src/SynackAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-16 04:21:15.000000 SynackAPI-0.4.2/src/SynackAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 04:21:15.000000 SynackAPI-0.4.2/src/SynackAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-16 04:21:15.000000 SynackAPI-0.4.2/src/SynackAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 04:21:15.000000 SynackAPI-0.4.2/src/SynackAPI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:15.843337 SynackAPI-0.4.2/src/synack/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:15.843337 SynackAPI-0.4.2/src/synack/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:15.843337 SynackAPI-0.4.2/src/synack/db/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic/README
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:15.847337 SynackAPI-0.4.2/src/synack/db/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic/versions/0c1ac7be711c_added_url_table_deleted_url_from_port_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic/versions/349c447c0d37_added_use_scratchspace_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic/versions/355984ba030b_added_notification_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic/versions/649443e08834_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic/versions/deb7dd07212c_added_ip_port_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:15.847337 SynackAPI-0.4.2/src/synack/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      447 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/models/category.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1579 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/models/ip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/models/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/models/port.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1059 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/models/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/models/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:15.851338 SynackAPI-0.4.2/src/synack/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17777 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/hydra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/missions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/scratchspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14647 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:15.855337 SynackAPI-0.4.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42898 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_hydra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16680 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_missions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_scratchspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39427 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_users.py
```

### Comparing `SynackAPI-0.4.1/LICENSE` & `SynackAPI-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/PKG-INFO` & `SynackAPI-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SynackAPI
-Version: 0.4.1
+Version: 0.4.2
 Summary: A package to interact with Synack's API
 Home-page: https://www.github.com/bamhm182/synackAPI
 Author: bamhm182
 Author-email: bamhm182@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SynackAPI-0.4.1/README.md` & `SynackAPI-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/setup.py` & `SynackAPI-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 setuptools.setup(
     name="SynackAPI",
-    version="0.4.1",
+    version="0.4.2",
     author="bamhm182",
     author_email="bamhm182@gmail.com",
     description="A package to interact with Synack's API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.github.com/bamhm182/synackAPI",
     classifiers=[
```

### Comparing `SynackAPI-0.4.1/src/SynackAPI.egg-info/PKG-INFO` & `SynackAPI-0.4.2/src/SynackAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SynackAPI
-Version: 0.4.1
+Version: 0.4.2
 Summary: A package to interact with Synack's API
 Home-page: https://www.github.com/bamhm182/synackAPI
 Author: bamhm182
 Author-email: bamhm182@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SynackAPI-0.4.1/src/SynackAPI.egg-info/SOURCES.txt` & `SynackAPI-0.4.2/src/SynackAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/_handler.py` & `SynackAPI-0.4.2/src/synack/_handler.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/_state.py` & `SynackAPI-0.4.2/src/synack/_state.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/db/alembic/env.py` & `SynackAPI-0.4.2/src/synack/db/alembic/env.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/db/alembic/versions/0c1ac7be711c_added_url_table_deleted_url_from_port_.py` & `SynackAPI-0.4.2/src/synack/db/alembic/versions/0c1ac7be711c_added_url_table_deleted_url_from_port_.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/db/alembic/versions/349c447c0d37_added_use_scratchspace_setting.py` & `SynackAPI-0.4.2/src/synack/db/alembic/versions/349c447c0d37_added_use_scratchspace_setting.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/db/alembic/versions/355984ba030b_added_notification_settings.py` & `SynackAPI-0.4.2/src/synack/db/alembic/versions/355984ba030b_added_notification_settings.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/db/alembic/versions/649443e08834_initial.py` & `SynackAPI-0.4.2/src/synack/db/alembic/versions/649443e08834_initial.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/db/alembic/versions/deb7dd07212c_added_ip_port_tables.py` & `SynackAPI-0.4.2/src/synack/db/alembic/versions/deb7dd07212c_added_ip_port_tables.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/db/alembic.ini` & `SynackAPI-0.4.2/src/synack/db/alembic.ini`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/db/models/config.py` & `SynackAPI-0.4.2/src/synack/db/models/config.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/db/models/port.py` & `SynackAPI-0.4.2/src/synack/db/models/port.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/db/models/target.py` & `SynackAPI-0.4.2/src/synack/db/models/target.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/plugins/alerts.py` & `SynackAPI-0.4.2/src/synack/plugins/alerts.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,19 @@
             server = smtplib.SMTP(self.db.smtp_server, self.db.smtp_port)
 
         server.login(self.db.smtp_username, self.db.smtp_password)
         server.send_message(msg)
 
     def sanitize(self, message):
         message = re.sub(r'[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}.[0-9]{1,3}', '[IPv4]', message)
-        message = re.sub(r'(?:https?:\/\/)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}' +
+        message = re.sub(r'(?:h[tx]{1,2}ps?:\/\/)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{2,6}' +
                          r'\b(?:[-a-zA-Z0-9()@:%_\+.~#?&\\/=]*)', '[URL]', message)
-        message = re.sub(r'(?:https?:\/\/)?(?:www\\.)?[-a-zA-Z0-9@:%._\\+~#=]{1,256}' +
-                         r'\\.[a-zA-Z0-9()]{1,6}\\b(?:[-a-zA-Z0-9()@:%_\\+.~#?&\\/=]*)', '[URL]', message)
-        message = re.sub(r'[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b' +
+        message = re.sub(r'(?:h[xt]{1,2}ps?:\/\/)?(?:www\\.)?[-a-zA-Z0-9@:%._\\+~#=]{1,256}' +
+                         r'\\.[a-zA-Z0-9()]{2,6}\\b(?:[-a-zA-Z0-9()@:%_\\+.~#?&\\/=]*)', '[URL]', message)
+        message = re.sub(r'[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{2,6}\b' +
                          r'(?:[-a-zA-Z0-9()@:%_\+.~#?&\\/=]*)', '[URL]', message)
         message = re.sub(r'(?:^|(?<=\s))(([0-9a-fA-F]{1,4}:){7,7}[0-9a-fA-F]{1,4}|' +
                          r'([0-9a-fA-F]{1,4}:){1,7}:|([0-9a-fA-F]{1,4}:){1,6}:[0-9a-fA-F]{1,4}|' +
                          r'([0-9a-fA-F]{1,4}:){1,5}(:[0-9a-fA-F]{1,4}){1,2}|([0-9a-fA-F]{1,4}:){1,4}' +
                          r'(:[0-9a-fA-F]{1,4}){1,3}|([0-9a-fA-F]{1,4}:){1,3}(:[0-9a-fA-F]{1,4}){1,4}|' +
                          r'([0-9a-fA-F]{1,4}:){1,2}(:[0-9a-fA-F]{1,4}){1,5}|[0-9a-fA-F]{1,4}:' +
                          r'((:[0-9a-fA-F]{1,4}){1,6})|:((:[0-9a-fA-F]{1,4}){1,7}|:)|fe80:' +
```

### Comparing `SynackAPI-0.4.1/src/synack/plugins/api.py` & `SynackAPI-0.4.2/src/synack/plugins/api.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/plugins/auth.py` & `SynackAPI-0.4.2/src/synack/plugins/auth.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/plugins/db.py` & `SynackAPI-0.4.2/src/synack/plugins/db.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/plugins/debug.py` & `SynackAPI-0.4.2/src/synack/plugins/debug.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/plugins/hydra.py` & `SynackAPI-0.4.2/src/synack/plugins/hydra.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/plugins/missions.py` & `SynackAPI-0.4.2/src/synack/plugins/missions.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/plugins/notifications.py` & `SynackAPI-0.4.2/src/synack/plugins/notifications.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/plugins/scratchspace.py` & `SynackAPI-0.4.2/src/synack/plugins/scratchspace.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,23 @@
         if codename:
             f = self.db.scratchspace_dir
             f = f / codename
             f.mkdir(parents=True, exist_ok=True)
             f = f / filename
             return f
 
+    def set_assets_file(self, content, target=None, codename=None):
+        if target or codename:
+            if type(content) in [list, set]:
+                content = '\n'.join(content)
+            dest_file = self.build_filepath('assets.txt', target=target, codename=codename)
+            with open(dest_file, 'w') as fp:
+                fp.write(content)
+                return dest_file
+
     def set_burp_file(self, content, target=None, codename=None):
         if target or codename:
             if type(content) == dict:
                 content = json.dumps(content)
             dest_file = self.build_filepath('burp.txt', target=target, codename=codename)
             with open(dest_file, 'w') as fp:
                 fp.write(content)
@@ -51,13 +60,13 @@
                         with open(dest_file, 'wb') as fp:
                             fp.write(res.content)
                             downloads.append(dest_file)
         return downloads
 
     def set_hosts_file(self, content, target=None, codename=None):
         if target or codename:
-            if type(content) == list:
+            if type(content) in [list, set]:
                 content = '\n'.join(content)
             dest_file = self.build_filepath('hosts.txt', target=target, codename=codename)
             with open(dest_file, 'w') as fp:
                 fp.write(content)
                 return dest_file
```

### Comparing `SynackAPI-0.4.1/src/synack/plugins/targets.py` & `SynackAPI-0.4.2/src/synack/plugins/targets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """plugins/targets.py
 
 Functions related to handling and checking targets
 """
 
 import ipaddress
+import re
 
 from urllib.parse import urlparse
 from .base import Plugin
 
 
 class Targets(Plugin):
     def __init__(self, *args, **kwargs):
@@ -41,53 +42,49 @@
                     'target': slug,
                     'ip': ip
                 })
         return ret
 
     def build_scope_web_burp(self, scope):
         """Return a Burp Suite scope given retrieved web scope"""
-        ret = {'target': {'scope': {'advanced_mode': 'true', 'exclude': [], 'include': []}}}
+        ret = {'target': {'scope': {'advanced_mode': 'true', 'exclude': list(), 'include': list()}}}
+
         for asset in scope:
-            state = 'include' if asset['status'] == 'in' else 'exclude'
-            raw = urlparse(asset['raw_url'])
-            for item in asset['rules']:
-                item = item['rule'].strip('.*')
-                url = urlparse(item)
-                if len(url.netloc) == 0:
-                    url = urlparse(raw.scheme + '://' + item)
-                ret['target']['scope'][state].append({
-                    'enabled': True if url.hostname else False,
-                    'scheme': url.scheme if url.scheme else 'any',
-                    'host': url.hostname,
-                    'file': url.path
-                })
+            state = 'include' if asset.get('status') == 'in' else 'exclude'
+            raw = urlparse(asset.get('location', ''))
+            item = asset.get('rule', '').strip('.*')
+            url = urlparse(item)
+            if len(url.netloc) == 0:
+                url = urlparse(raw.scheme + '://' + item)
+            ret['target']['scope'][state].append({
+                'enabled': True if url.hostname else False,
+                'scheme': url.scheme if url.scheme else 'any',
+                'host': url.hostname,
+                'file': url.path
+            })
         return ret
 
     def build_scope_web_db(self, scope):
         """Return a Web Scope that can be ingested into the Database"""
+        sorting = dict()
+
+        for item in scope:
+            if item.get('status') == 'in':
+                slug = item.get('listing')
+                sorting[slug] = sorting.get(slug, list())
+                sorting[slug].append({'url': item.get('location')})
+
         ret = list()
-        for asset in scope:
-            if asset.get('status') == 'in':
-                for owner in asset.get('owners'):
-                    ret.append({
-                        "target": owner.get('owner_uid'),
-                        "urls": [{
-                            "url": asset.get('raw_url')
-                        }]
-                    })
-        return ret
 
-    def build_scope_web_urls(self, scope):
-        """Return a list of the raw urls gived a retrieved web scope"""
-        ret = {"in": list(), "out": list()}
-        for asset in scope:
-            if asset.get('status') == 'in':
-                ret["in"].append(asset["raw_url"])
-            else:
-                ret["out"].append(asset["raw_url"])
+        for slug, urls in sorting.items():
+            ret.append({
+                'target': slug,
+                'urls': urls
+            })
+
         return ret
 
     def build_slug_from_codename(self, codename):
         """Return a slug for a target given its codename"""
         slug = None
         targets = self.db.find_targets(codename=codename)
         if not targets:
@@ -100,14 +97,57 @@
     def get_assessments(self):
         """Check which assessments have been completed"""
         res = self.api.request('GET', 'assessments')
         if res.status_code == 200:
             self.db.add_categories(res.json())
             return self.db.categories
 
+    def get_assets(self, target=None, asset_type=None, host_type=None, active='true',
+                   scope=['in', 'discovered'], sort='location', sort_dir='asc',
+                   page=None, organization_uid=None, **kwargs):
+        """Get the assets (scope) of a target"""
+        if target is None:
+            if len(kwargs) > 0:
+                target = self.db.find_targets(**kwargs)
+            else:
+                curr = self.get_connected()
+                target = self.db.find_targets(slug=curr.get('slug'))
+
+        if type(scope) == str:
+            scope = [scope]
+
+        if target:
+            if type(target) is list and len(target) > 0:
+                target = target[0]
+            queries = list()
+
+            queries.append(f'listingUid%5B%5D={target.slug}')
+            if organization_uid is not None:
+                queries.append(f'organizationUid%5B%5D={organization_uid}')
+            if asset_type is not None:
+                queries.append(f'assetType%5B%5D={asset_type}')
+            if host_type is not None:
+                queries.append(f'hostType%5B%5D={host_type}')
+            for item in scope:
+                queries.append(f'scope%5B%5D={item}')
+            if sort is not None:
+                queries.append(f'sort%5B%5D={sort}')
+            if active is not None:
+                queries.append(f'active={active}')
+            if sort_dir is not None:
+                queries.append(f'sortDir={sort_dir}')
+            if page is not None:
+                queries.append(f'page={page}')
+
+            res = self.api.request('GET', f'asset/v2/assets?{"&".join(queries)}')
+            if res.status_code == 200:
+                if self.db.use_scratchspace:
+                    self.scratchspace.set_assets_file(res.text, target=target)
+                return res.json()
+
     def get_attachments(self, target=None, **kwargs):
         """Get the attachments of a target."""
         if target is None:
             if len(kwargs) == 0:
                 kwargs = {'codename': self.get_connected().get('codename')}
             target = self.db.find_targets(**kwargs)
             if target:
@@ -207,45 +247,73 @@
                 return self.get_scope_host(target, add_to_db=add_to_db)
             elif categories[target.category].lower() in ['web application', 'mobile']:
                 return self.get_scope_web(target, add_to_db=add_to_db)
 
     def get_scope_host(self, target=None, add_to_db=False, **kwargs):
         """Get the scope of a Host target"""
         if target is None:
-            target = self.db.find_targets(**kwargs)
-            if target:
-                target = target[0]
+            targets = self.db.find_targets(**kwargs)
+            if targets:
+                target = next(iter(targets), None)
+
+        scope = set()
+
         if target:
-            res = self.api.request('GET', f'targets/{target.slug}/cidrs?page=all')
-            if res.status_code == 200:
-                scope = res.json()['cidrs']
+            assets = self.get_assets(target=target, active='true', asset_type='host', host_type='cidr')
+            for asset in assets:
+                if asset.get('active'):
+                    try:
+                        ipaddress.IPv4Network(asset.get('location'))
+                        scope.add(asset.get('location'))
+                    except ipaddress.AddressValueError:
+                        # Not actually an IP
+                        pass
+
+            scope.discard(None)
+
+            if len(scope) > 0:
                 if add_to_db:
                     self.db.add_ips(self.build_scope_host_db(target.slug, scope))
                 if self.db.use_scratchspace:
                     self.scratchspace.set_hosts_file(scope, target=target)
-                return scope
+
+        return scope
 
     def get_scope_web(self, target=None, add_to_db=False, **kwargs):
-        """Get the web scpope of a Web or Mobile target"""
+        """Get the scope of a Web target"""
         if target is None:
-            target = self.db.find_targets(**kwargs)
-            if target:
-                target = target[0]
-        res = self.api.request('GET', f'asset/v1/organizations/{target.organization}' +
-                                      f'/owners/listings/{target.slug}/webapps')
-        if res.status_code == 200:
-            scope = list()
-            for asset in res.json():
-                if target.slug in [o['owner_uid'] for o in asset['owners']]:
-                    scope.append(asset)
-            if add_to_db:
-                self.db.add_urls(self.build_scope_web_db(scope))
-            if self.db.use_scratchspace:
-                self.scratchspace.set_burp_file(self.build_scope_web_burp(scope), target=target)
-            return scope
+            targets = self.db.find_targets(**kwargs)
+            if targets:
+                target = next(iter(targets), None)
+
+        scope = list()
+
+        if target:
+            assets = self.get_assets(target=target, active='true', asset_type='webapp')
+            for asset in assets:
+                if asset.get('active'):
+                    location = next(iter(re.split(r' \(', asset.get('location', ''))))
+                    for listing in asset.get('listings', []):
+                        status = listing.get('scope')
+                        listing = listing.get('listingUid')
+                        for rule in asset.get('scopeRules', []):
+                            scope.append({
+                                'status': status,
+                                'listing': listing,
+                                'location': location,
+                                'rule': rule.get('rule')
+                            })
+
+            if len(scope) > 0:
+                if add_to_db:
+                    self.db.add_urls(self.build_scope_web_db(scope))
+                if self.db.use_scratchspace:
+                    self.scratchspace.set_web_file(self.build_scope_web_burp(scope), target=target)
+
+        return scope
 
     def get_submissions(self, target=None, status="accepted", **kwargs):
         """Get the details of previously submitted vulnerabilities from the analytics of a target."""
         if status not in ["accepted", "rejected", "in_queue"]:
             return []
         if target is None:
             if len(kwargs) == 0:
```

### Comparing `SynackAPI-0.4.1/src/synack/plugins/templates.py` & `SynackAPI-0.4.2/src/synack/plugins/templates.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/plugins/transactions.py` & `SynackAPI-0.4.2/src/synack/plugins/transactions.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/src/synack/plugins/users.py` & `SynackAPI-0.4.2/src/synack/plugins/users.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/test/test_alerts.py` & `SynackAPI-0.4.2/test/test_alerts.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,19 +66,21 @@
 
     def test_sanitize_overzealous(self):
         """Should not overly sanitize things that are fine"""
         self.assertEqual(self.alerts.sanitize('This is fine'), 'This is fine')
         self.assertEqual(self.alerts.sanitize('This is fine!'), 'This is fine!')
         self.assertEqual(self.alerts.sanitize('This is: fine'), 'This is: fine')
         self.assertEqual(self.alerts.sanitize('This is fine?'), 'This is fine?')
+        self.assertEqual(self.alerts.sanitize('24.0'), '24.0')
 
     def test_sanitize_urls(self):
         """Should sanitize URLs"""
         self.assertEqual(self.alerts.sanitize('test.cc'), '[URL]')
         self.assertEqual(self.alerts.sanitize('http://1.2.ewufg.4.test.cc'), '[URL]')
+        self.assertEqual(self.alerts.sanitize('hxxp://1.2.ewufg.4.test.cc'), '[URL]')
         self.assertEqual(self.alerts.sanitize('http://1.2.ewufg.4.test.cc:8081'), '[URL]')
         self.assertEqual(self.alerts.sanitize('http://1.2.ewufg.4.test.cc:8081/tacos/are/number/1'), '[URL]')
         self.assertEqual(self.alerts.sanitize('URL: https://www.test.com/1/2/3/air'), 'URL: [URL]')
         self.assertEqual(self.alerts.sanitize('This is a URL: bob.com'), 'This is a URL: [URL]')
 
     def test_slack(self):
         """Should POST a message to slack"""
```

### Comparing `SynackAPI-0.4.1/test/test_api.py` & `SynackAPI-0.4.2/test/test_api.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/test/test_auth.py` & `SynackAPI-0.4.2/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/test/test_db.py` & `SynackAPI-0.4.2/test/test_db.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/test/test_debug.py` & `SynackAPI-0.4.2/test/test_debug.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/test/test_handler.py` & `SynackAPI-0.4.2/test/test_handler.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/test/test_hydra.py` & `SynackAPI-0.4.2/test/test_hydra.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/test/test_missions.py` & `SynackAPI-0.4.2/test/test_missions.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/test/test_notifications.py` & `SynackAPI-0.4.2/test/test_notifications.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/test/test_scratchspace.py` & `SynackAPI-0.4.2/test/test_scratchspace.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,14 +29,36 @@
     def test_build_filepath_target(self):
         """Should build the appropriate scratchspace filepath given a filepath"""
         self.scratchspace.db.scratchspace_dir = pathlib.Path('/tmp')
         target = synack.db.models.Target(codename='TIREDTURKEY')
         ret = self.scratchspace.build_filepath('test.txt', target=target)
         self.assertEqual(pathlib.Path('/tmp/TIREDTURKEY/test.txt'), ret)
 
+    def test_set_asset_file(self):
+        """Shoudl create an asset file within the correct directory"""
+        self.scratchspace.build_filepath = MagicMock()
+        self.scratchspace.build_filepath.return_value = '/tmp/TIREDTURKEY/assets.txt'
+        m = mock_open()
+        with patch('builtins.open', m, create=True):
+            ret = self.scratchspace.set_assets_file('Test', codename='TIREDTURKEY')
+            self.assertEqual('/tmp/TIREDTURKEY/assets.txt', ret)
+            m.return_value.write.assert_called_with('Test')
+            m.assert_called_with('/tmp/TIREDTURKEY/assets.txt', 'w')
+
+    def test_set_asset_file_list(self):
+        """Shoudl create an asset file within the correct directory"""
+        self.scratchspace.build_filepath = MagicMock()
+        self.scratchspace.build_filepath.return_value = '/tmp/TIREDTURKEY/assets.txt'
+        m = mock_open()
+        with patch('builtins.open', m, create=True):
+            ret = self.scratchspace.set_assets_file(['one', 'two', 'three'], codename='TIREDTURKEY')
+            self.assertEqual('/tmp/TIREDTURKEY/assets.txt', ret)
+            m.return_value.write.assert_called_with('one\ntwo\nthree')
+            m.assert_called_with('/tmp/TIREDTURKEY/assets.txt', 'w')
+
     def test_set_burp_file(self):
         """Should create a burp file within the correct directory"""
         self.scratchspace.build_filepath = MagicMock()
         self.scratchspace.build_filepath.return_value = '/tmp/TIREDTURKEY/burp.txt'
         m = mock_open()
         with patch('builtins.open', m, create=True):
             ret = self.scratchspace.set_burp_file('Test', codename='TIREDTURKEY')
```

### Comparing `SynackAPI-0.4.1/test/test_state.py` & `SynackAPI-0.4.2/test/test_state.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/test/test_targets.py` & `SynackAPI-0.4.2/test/test_targets.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,27 +69,30 @@
         ]
         self.assertEqual(expected, self.targets.build_scope_host_db(slug, scope))
 
     def test_build_scope_web_burp(self):
         """Should build a Burp Suite Scope given a Synack API Scope"""
         scope = [
             {
-                'raw_url': 'https://good.stuff.com',
+                'listing': 'uqwheiuqwhe',
+                'location': 'https://good.stuff.com',
                 'status': 'in',
-                'rules': [
-                    {'rule': '*.stuff.com/*'},
-                    {'rule': 'https://super.stuff.com/'},
-                ]
+                'rule': '*.stuff.com/*',
             },
             {
-                'raw_url': 'http://evil.stuff.com',
+                'listing': 'uqwheiuqwhe',
+                'location': 'https://good.stuff.com',
+                'status': 'in',
+                'rule': 'https://super.stuff.com/'
+            },
+            {
+                'listing': 'uqwheiuqwhe',
+                'location': 'http://evil.stuff.com',
                 'status': 'out',
-                'rules': [
-                    {'rule': '*.evil.stuff.com/login/*'},
-                ]
+                'rule': '*.evil.stuff.com/login/*'
             }
         ]
         expected = {
             'target': {
                 'scope': {
                     'advanced_mode': 'true',
                     'exclude': [
@@ -119,58 +122,48 @@
         }
         self.assertEqual(expected, self.targets.build_scope_web_burp(scope))
 
     def test_build_scope_web_db(self):
         """Should build a web scope that can be ingested into the Database"""
         scope = [
             {
-                'raw_url': 'https://good.stuff.com',
-                'owners': [{'owner_uid': '12345'}, {'owner_uid': '67890'}],
-                'status': 'in'
+                'listing': 'uqwheiuq',
+                'location': 'https://good.stuff.com',
+                'status': 'in',
+                'rule': '*.good.stuff.com/*'
+            },
+            {
+                'listing': 'uqwheiuq',
+                'location': 'https://bad.stuff.com',
+                'status': 'out',
+                'rule': '*.bad.stuff.com/*'
             },
             {
-                'raw_url': 'https://bad.stuff.com',
-                'owners': [{'owner_uid': 'abcde'}],
-                'status': 'out'
+                'listing': '21ye78r3hwe',
+                'location': 'https://good.things.com',
+                'status': 'in',
+                'rule': '*.good.things.com/*'
             }
         ]
         expected = [
             {
-                'target': '12345',
+                'target': 'uqwheiuq',
                 'urls': [{
                     'url': 'https://good.stuff.com'
                 }]
             },
             {
-                'target': '67890',
+                'target': '21ye78r3hwe',
                 'urls': [{
-                    'url': 'https://good.stuff.com'
+                    'url': 'https://good.things.com'
                 }]
             }
         ]
         self.assertEqual(expected, self.targets.build_scope_web_db(scope))
 
-    def test_build_scope_web_urls(self):
-        """Should build dictionaries of Web Application URLs given a Synack API Scope"""
-        scope = [
-            {
-                'raw_url': 'https://good.stuff.com',
-                'status': 'in'
-            },
-            {
-                'raw_url': 'https://bad.stuff.com',
-                'status': 'out'
-            }
-        ]
-        expected = {
-            'in': ['https://good.stuff.com'],
-            'out': ['https://bad.stuff.com']
-        }
-        self.assertEqual(expected, self.targets.build_scope_web_urls(scope))
-
     def test_build_slug_from_codename(self):
         """Should return a slug for a given codename"""
         ret_targets = [Target(slug="qwerty")]
         self.targets.db.find_targets.return_value = ret_targets
         self.assertEqual("qwerty",
                          self.targets.build_slug_from_codename("qwerty"))
         self.targets.db.find_targets.assert_called_with(codename="qwerty")
@@ -219,14 +212,49 @@
         cat1 = synack.db.models.Category()
         self.targets.api.request.return_value.status_code = 200
         self.targets.api.request.return_value.json.return_value = assessments
         self.targets.db.categories = [cat1]
         self.assertEqual([cat1], self.targets.get_assessments())
         self.targets.db.add_categories.assert_called_with(assessments)
 
+    def test_get_assets(self):
+        """Should return a list of assets for a currently connected target"""
+        self.targets.get_connected = MagicMock()
+        self.targets.get_connected.return_value = {'codename': 'TURBULENTTORTOISE', 'slug': '327h8iw'}
+        self.targets.db.find_targets.return_value = [Target(slug='327h8iw')]
+        self.targets.api.request.return_value.status_code = 200
+        self.targets.api.request.return_value.text = 'rettext'
+        self.targets.api.request.return_value.json.return_value = 'retjson'
+        self.assertEqual('retjson', self.targets.get_assets())
+        self.targets.api.request.assert_called_with('GET',
+                                                    'asset/v2/assets?listingUid%5B%5D=327h8iw&scope%5B%5D=in' +
+                                                    '&scope%5B%5D=discovered&sort%5B%5D=location&active=true' +
+                                                    '&sortDir=asc')
+
+    def test_get_assets_non_defaults(self):
+        """Should return a list of assets given information to query"""
+        self.targets.db.find_targets.return_value = [Target(codename='TURBULENTTORTOISE', slug='327h8iw')]
+        self.targets.api.request.return_value.status_code = 200
+        self.targets.api.request.return_value.text = 'rettext'
+        self.targets.api.request.return_value.json.return_value = 'retjson'
+        self.assertEqual('retjson', self.targets.get_assets(codename='TURBULENTTORTOISE',
+                                                            asset_type='blah',
+                                                            host_type='applecidr',
+                                                            active='false',
+                                                            scope='secret',
+                                                            sort='vulnerable',
+                                                            sort_dir='desc',
+                                                            page=3,
+                                                            organization_uid='uiehqw'))
+        self.targets.api.request.assert_called_with('GET',
+                                                    'asset/v2/assets?listingUid%5B%5D=327h8iw' +
+                                                    '&organizationUid%5B%5D=uiehqw&assetType%5B%5D=blah' +
+                                                    '&hostType%5B%5D=applecidr&scope%5B%5D=secret' +
+                                                    '&sort%5B%5D=vulnerable&active=false&sortDir=desc&page=3')
+
     def test_get_attachments_current(self):
         """Should return a list of attachments based on currently selected target"""
         attachments = [
             {
                 "listing_id": "12uib",
                 "url": "https://www.download.com/uh1g23ri",
                 "filename": "file1.txt",
@@ -487,93 +515,138 @@
         out = self.targets.get_scope(slug='1392g78yr', add_to_db=True)
         self.targets.db.find_targets.assert_called_with(slug='1392g78yr')
         self.targets.get_scope_web.assert_called_with(tgt, add_to_db=True)
         self.assertEquals(out, 'WebScope')
 
     def test_get_scope_host(self):
         """Should get the scope for a Host"""
-        ips = ['1.1.1.1/32', '2.2.2.2/32']
-        self.targets.api.request.return_value.status_code = 200
-        self.targets.api.request.return_value.json.return_value = {
-            'cidrs': ips
-        }
+        ips = {'1.1.1.1/32', '2.2.2.2/32'}
+        self.targets.get_assets = MagicMock()
+        self.targets.get_assets.return_value = [
+            {
+                'active': True,
+                'location': '1.1.1.1/32'
+            },
+            {
+                'active': True,
+                'location': '2.2.2.2/32'
+            }
+        ]
         self.targets.db.find_targets.return_value = [Target(slug='213h89h3', codename='SASSYSQUIRREL')]
         out = self.targets.get_scope_host(codename='SASSYSQUIRREL')
         self.assertEqual(ips, out)
         self.targets.db.find_targets.assert_called_with(codename='SASSYSQUIRREL')
-        self.targets.api.request.assert_called_with('GET', 'targets/213h89h3/cidrs?page=all')
-        self.targets.api.request.return_value.json.assert_called()
 
     def test_get_scope_host_add_to_db(self):
         """Should get the scope for a Host"""
-        ips = ['1.1.1.1/32', '2.2.2.2/32']
-        self.targets.api.request.return_value.status_code = 200
-        self.targets.api.request.return_value.json.return_value = {
-            'cidrs': ips
-        }
+        ips = {'1.1.1.1/32', '2.2.2.2/32'}
+        self.targets.get_assets = MagicMock()
+        self.targets.get_assets.return_value = [
+            {
+                'active': True,
+                'location': '1.1.1.1/32'
+            },
+            {
+                'active': True,
+                'location': '2.2.2.2/32'
+            }
+        ]
+        self.targets.build_scope_host_db = MagicMock()
+        self.targets.build_scope_host_db.return_value = 'host_db_return_value'
         self.targets.db.find_targets.return_value = [Target(slug='213h89h3', codename='SASSYSQUIRREL')]
         out = self.targets.get_scope_host(codename='SASSYSQUIRREL', add_to_db=True)
         self.assertEqual(ips, out)
         self.targets.db.find_targets.assert_called_with(codename='SASSYSQUIRREL')
-        self.targets.api.request.assert_called_with('GET', 'targets/213h89h3/cidrs?page=all')
-        self.targets.api.request.return_value.json.assert_called()
-        self.targets.db.add_ips.assert_called_with([{'target': '213h89h3', 'ip': '1.1.1.1'},
-                                                    {'target': '213h89h3', 'ip': '2.2.2.2'}])
+        self.targets.build_scope_host_db.assert_called_with('213h89h3', ips)
+        self.targets.db.add_ips.assert_called_with('host_db_return_value')
+
+    def test_get_scope_host_not_ip(self):
+        """Should get the scope for a Host"""
+        ips = {'1.1.1.1/32'}
+        self.targets.get_assets = MagicMock()
+        self.targets.get_assets.return_value = [
+            {
+                'active': True,
+                'location': '1.1.1.1/32'
+            },
+            {
+                'active': True,
+                'location': '8675309'
+            }
+        ]
+        self.targets.db.find_targets.return_value = [Target(slug='213h89h3', codename='SASSYSQUIRREL')]
+        out = self.targets.get_scope_host(codename='SASSYSQUIRREL')
+        self.assertEqual(ips, out)
+        self.targets.db.find_targets.assert_called_with(codename='SASSYSQUIRREL')
 
     def test_get_scope_no_provided(self):
         """Should get the scope for the currently connected target if none is specified"""
         self.targets.get_connected = MagicMock()
         self.targets.get_connected.return_value = {'slug': 'test'}
         self.targets.db.find_targets.return_value = None
         self.targets.get_scope()
         self.targets.get_connected.assert_called_with()
         self.targets.db.find_targets.assert_called_with(slug='test')
 
     def test_get_scope_web(self):
         """Should get the scope for a Web Application"""
-        self.targets.api.request.return_value.status_code = 200
         self.targets.build_scope_web_burp = MagicMock()
-        web_results = [{
-            'web_results': 'yup these them!',
-            'owners': [{
-                'owner_uid': '213h89h3'
-            }],
+        scope = [{
+            'listing': 'uewqhuiewq',
+            'location': 'https://good.things.com',
+            'rule': '*.good.things.com/*',
+            'status': 'in'
         }]
-        self.targets.api.request.return_value.json.return_value = web_results
+        self.targets.get_assets = MagicMock()
+        self.targets.get_assets.return_value = [
+            {
+                'active': True,
+                'listings': [{'listingUid': 'uewqhuiewq', 'scope': 'in'}],
+                'location': 'https://good.things.com (https://good.things.com)',
+                'scopeRules': [
+                    {'rule': '*.good.things.com/*'}
+                ]
+            }
+        ]
         tgt = Target(slug='213h89h3', organization='93g8eh8', codename='SASSYSQUIRREL')
         self.targets.db.find_targets.return_value = [tgt]
         out = self.targets.get_scope_web(codename='SASSYSQUIRREL')
-        self.assertEqual(web_results, out)
-        self.targets.build_scope_web_burp.assert_called_with(web_results)
+        self.assertEqual(scope, out)
+        self.targets.build_scope_web_burp.assert_called_with(scope)
         self.targets.db.find_targets.assert_called_with(codename='SASSYSQUIRREL')
-        self.targets.api.request.assert_called_with('GET',
-                                                    'asset/v1/organizations/93g8eh8/owners/listings/213h89h3/webapps')
-        self.targets.api.request.return_value.json.assert_called()
+        self.targets.get_assets.assert_called_with(target=tgt, active='true', asset_type='webapp')
 
     def test_get_scope_web_add_to_db(self):
-        """Should get the scope for a Web Application"""
-        self.targets.api.request.return_value.status_code = 200
+        """Should get the scope for a Web Application and add it to the database"""
         self.targets.build_scope_web_burp = MagicMock()
         self.targets.build_scope_web_db = MagicMock()
-        web_results = [{
-            'web_results': 'yup these them!',
-            'owners': [{
-                'owner_uid': '213h89h3'
-            }],
+        self.targets.get_assets = MagicMock()
+        scope = [{
+            'listing': 'uewqhuiewq',
+            'location': 'https://good.things.com',
+            'rule': '*.good.things.com/*',
+            'status': 'in'
         }]
-        self.targets.api.request.return_value.json.return_value = web_results
+        self.targets.get_assets = MagicMock()
+        self.targets.get_assets.return_value = [
+            {
+                'active': True,
+                'listings': [{'listingUid': 'uewqhuiewq', 'scope': 'in'}],
+                'location': 'https://good.things.com (https://good.things.com)',
+                'scopeRules': [
+                    {'rule': '*.good.things.com/*'}
+                ]
+            }
+        ]
         tgt = Target(slug='213h89h3', organization='93g8eh8', codename='SASSYSQUIRREL')
         self.targets.db.find_targets.return_value = [tgt]
         out = self.targets.get_scope_web(codename='SASSYSQUIRREL', add_to_db=True)
-        self.assertEqual(web_results, out)
-        self.targets.build_scope_web_burp.assert_called_with(web_results)
+        self.assertEqual(scope, out)
+        self.targets.build_scope_web_burp.assert_called_with(scope)
         self.targets.db.find_targets.assert_called_with(codename='SASSYSQUIRREL')
-        self.targets.api.request.assert_called_with('GET',
-                                                    'asset/v1/organizations/93g8eh8/owners/listings/213h89h3/webapps')
-        self.targets.api.request.return_value.json.assert_called()
         self.targets.db.add_urls.assert_called_with(self.targets.build_scope_web_db.return_value)
 
     def test_get_submissions(self):
         """Should return the accepted vulnerabilities for a target given a slug"""
         return_data = {
             "listing_id": "u2ire",
             "type": "categories",
```

### Comparing `SynackAPI-0.4.1/test/test_templates.py` & `SynackAPI-0.4.2/test/test_templates.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/test/test_transactions.py` & `SynackAPI-0.4.2/test/test_transactions.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.1/test/test_users.py` & `SynackAPI-0.4.2/test/test_users.py`

 * *Files identical despite different names*

