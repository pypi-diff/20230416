# Comparing `tmp/SynackAPI-0.4.2.tar.gz` & `tmp/SynackAPI-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SynackAPI-0.4.2.tar", last modified: Sun Apr 16 04:21:15 2023, max compression
+gzip compressed data, was "SynackAPI-0.4.3.tar", last modified: Sun Apr 16 07:27:10 2023, max compression
```

## Comparing `SynackAPI-0.4.2.tar` & `SynackAPI-0.4.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:15.855337 SynackAPI-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-16 04:21:15.855337 SynackAPI-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 04:21:15.855337 SynackAPI-0.4.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:15.839337 SynackAPI-0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:15.843337 SynackAPI-0.4.2/src/SynackAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-16 04:21:15.000000 SynackAPI-0.4.2/src/SynackAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-16 04:21:15.000000 SynackAPI-0.4.2/src/SynackAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 04:21:15.000000 SynackAPI-0.4.2/src/SynackAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-16 04:21:15.000000 SynackAPI-0.4.2/src/SynackAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 04:21:15.000000 SynackAPI-0.4.2/src/SynackAPI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:15.843337 SynackAPI-0.4.2/src/synack/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:15.843337 SynackAPI-0.4.2/src/synack/db/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:15.843337 SynackAPI-0.4.2/src/synack/db/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic/README
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:15.847337 SynackAPI-0.4.2/src/synack/db/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic/versions/0c1ac7be711c_added_url_table_deleted_url_from_port_.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic/versions/349c447c0d37_added_use_scratchspace_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic/versions/355984ba030b_added_notification_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic/versions/649443e08834_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic/versions/deb7dd07212c_added_ip_port_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/alembic.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:15.847337 SynackAPI-0.4.2/src/synack/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      447 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/models/category.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1579 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/models/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/models/ip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/models/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/models/port.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1059 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/models/target.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/db/models/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:15.851338 SynackAPI-0.4.2/src/synack/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17777 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/hydra.py
--rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/missions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/scratchspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    14647 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/src/synack/plugins/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 04:21:15.855337 SynackAPI-0.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    42898 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_hydra.py
--rw-r--r--   0 runner    (1001) docker     (123)    16680 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_missions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_scratchspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    39427 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-16 04:21:14.000000 SynackAPI-0.4.2/test/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:27:10.520594 SynackAPI-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-16 07:27:10.520594 SynackAPI-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 07:27:10.520594 SynackAPI-0.4.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:27:10.508593 SynackAPI-0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:27:10.512593 SynackAPI-0.4.3/src/SynackAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-16 07:27:10.000000 SynackAPI-0.4.3/src/SynackAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-16 07:27:10.000000 SynackAPI-0.4.3/src/SynackAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 07:27:10.000000 SynackAPI-0.4.3/src/SynackAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-16 07:27:10.000000 SynackAPI-0.4.3/src/SynackAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 07:27:10.000000 SynackAPI-0.4.3/src/SynackAPI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:27:10.512593 SynackAPI-0.4.3/src/synack/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:27:10.512593 SynackAPI-0.4.3/src/synack/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:27:10.512593 SynackAPI-0.4.3/src/synack/db/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/db/alembic/README
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/db/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/db/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/db/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:27:10.516594 SynackAPI-0.4.3/src/synack/db/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/db/alembic/versions/0c1ac7be711c_added_url_table_deleted_url_from_port_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/db/alembic/versions/349c447c0d37_added_use_scratchspace_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/db/alembic/versions/355984ba030b_added_notification_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/db/alembic/versions/649443e08834_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/db/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/db/alembic/versions/deb7dd07212c_added_ip_port_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/db/alembic.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:27:10.516594 SynackAPI-0.4.3/src/synack/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/db/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      447 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/db/models/category.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1579 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/db/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/db/models/ip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/db/models/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/db/models/port.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1059 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/db/models/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/db/models/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:27:10.520594 SynackAPI-0.4.3/src/synack/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/plugins/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/plugins/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/plugins/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/plugins/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17777 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/plugins/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/plugins/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/plugins/hydra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/plugins/missions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/plugins/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/plugins/scratchspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14984 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/plugins/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/plugins/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/plugins/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/src/synack/plugins/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:27:10.520594 SynackAPI-0.4.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/test/test_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42898 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/test/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/test/test_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/test/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/test/test_hydra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16680 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/test/test_missions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/test/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/test/test_scratchspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/test/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41784 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/test/test_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/test/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/test/test_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-16 07:27:09.000000 SynackAPI-0.4.3/test/test_users.py
```

### Comparing `SynackAPI-0.4.2/LICENSE` & `SynackAPI-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/PKG-INFO` & `SynackAPI-0.4.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SynackAPI
-Version: 0.4.2
+Version: 0.4.3
 Summary: A package to interact with Synack's API
 Home-page: https://www.github.com/bamhm182/synackAPI
 Author: bamhm182
 Author-email: bamhm182@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SynackAPI-0.4.2/README.md` & `SynackAPI-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/setup.py` & `SynackAPI-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 setuptools.setup(
     name="SynackAPI",
-    version="0.4.2",
+    version="0.4.3",
     author="bamhm182",
     author_email="bamhm182@gmail.com",
     description="A package to interact with Synack's API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.github.com/bamhm182/synackAPI",
     classifiers=[
```

### Comparing `SynackAPI-0.4.2/src/SynackAPI.egg-info/PKG-INFO` & `SynackAPI-0.4.3/src/SynackAPI.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SynackAPI
-Version: 0.4.2
+Version: 0.4.3
 Summary: A package to interact with Synack's API
 Home-page: https://www.github.com/bamhm182/synackAPI
 Author: bamhm182
 Author-email: bamhm182@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SynackAPI-0.4.2/src/SynackAPI.egg-info/SOURCES.txt` & `SynackAPI-0.4.3/src/SynackAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/_handler.py` & `SynackAPI-0.4.3/src/synack/_handler.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/_state.py` & `SynackAPI-0.4.3/src/synack/_state.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/db/alembic/env.py` & `SynackAPI-0.4.3/src/synack/db/alembic/env.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/db/alembic/versions/0c1ac7be711c_added_url_table_deleted_url_from_port_.py` & `SynackAPI-0.4.3/src/synack/db/alembic/versions/0c1ac7be711c_added_url_table_deleted_url_from_port_.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/db/alembic/versions/349c447c0d37_added_use_scratchspace_setting.py` & `SynackAPI-0.4.3/src/synack/db/alembic/versions/349c447c0d37_added_use_scratchspace_setting.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/db/alembic/versions/355984ba030b_added_notification_settings.py` & `SynackAPI-0.4.3/src/synack/db/alembic/versions/355984ba030b_added_notification_settings.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/db/alembic/versions/649443e08834_initial.py` & `SynackAPI-0.4.3/src/synack/db/alembic/versions/649443e08834_initial.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/db/alembic/versions/deb7dd07212c_added_ip_port_tables.py` & `SynackAPI-0.4.3/src/synack/db/alembic/versions/deb7dd07212c_added_ip_port_tables.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/db/alembic.ini` & `SynackAPI-0.4.3/src/synack/db/alembic.ini`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/db/models/config.py` & `SynackAPI-0.4.3/src/synack/db/models/config.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/db/models/port.py` & `SynackAPI-0.4.3/src/synack/db/models/port.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/db/models/target.py` & `SynackAPI-0.4.3/src/synack/db/models/target.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/plugins/alerts.py` & `SynackAPI-0.4.3/src/synack/plugins/alerts.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/plugins/api.py` & `SynackAPI-0.4.3/src/synack/plugins/api.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/plugins/auth.py` & `SynackAPI-0.4.3/src/synack/plugins/auth.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/plugins/db.py` & `SynackAPI-0.4.3/src/synack/plugins/db.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/plugins/debug.py` & `SynackAPI-0.4.3/src/synack/plugins/debug.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/plugins/hydra.py` & `SynackAPI-0.4.3/src/synack/plugins/hydra.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/plugins/missions.py` & `SynackAPI-0.4.3/src/synack/plugins/missions.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/plugins/notifications.py` & `SynackAPI-0.4.3/src/synack/plugins/notifications.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/plugins/scratchspace.py` & `SynackAPI-0.4.3/src/synack/plugins/scratchspace.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/plugins/targets.py` & `SynackAPI-0.4.3/src/synack/plugins/targets.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,19 @@
                 return self.get_scope_host(target, add_to_db=add_to_db)
             elif categories[target.category].lower() in ['web application', 'mobile']:
                 return self.get_scope_web(target, add_to_db=add_to_db)
 
     def get_scope_host(self, target=None, add_to_db=False, **kwargs):
         """Get the scope of a Host target"""
         if target is None:
-            targets = self.db.find_targets(**kwargs)
+            if len(kwargs) > 0:
+                targets = self.db.find_targets(**kwargs)
+            else:
+                curr = self.get_connected()
+                targets = self.db.find_targets(slug=curr.get('slug'))
             if targets:
                 target = next(iter(targets), None)
 
         scope = set()
 
         if target:
             assets = self.get_assets(target=target, active='true', asset_type='host', host_type='cidr')
@@ -277,15 +281,19 @@
                     self.scratchspace.set_hosts_file(scope, target=target)
 
         return scope
 
     def get_scope_web(self, target=None, add_to_db=False, **kwargs):
         """Get the scope of a Web target"""
         if target is None:
-            targets = self.db.find_targets(**kwargs)
+            if len(kwargs) > 0:
+                targets = self.db.find_targets(**kwargs)
+            else:
+                curr = self.get_connected()
+                targets = self.db.find_targets(slug=curr.get('slug'))
             if targets:
                 target = next(iter(targets), None)
 
         scope = list()
 
         if target:
             assets = self.get_assets(target=target, active='true', asset_type='webapp')
@@ -303,15 +311,15 @@
                                 'rule': rule.get('rule')
                             })
 
             if len(scope) > 0:
                 if add_to_db:
                     self.db.add_urls(self.build_scope_web_db(scope))
                 if self.db.use_scratchspace:
-                    self.scratchspace.set_web_file(self.build_scope_web_burp(scope), target=target)
+                    self.scratchspace.set_burp_file(self.build_scope_web_burp(scope), target=target)
 
         return scope
 
     def get_submissions(self, target=None, status="accepted", **kwargs):
         """Get the details of previously submitted vulnerabilities from the analytics of a target."""
         if status not in ["accepted", "rejected", "in_queue"]:
             return []
```

### Comparing `SynackAPI-0.4.2/src/synack/plugins/templates.py` & `SynackAPI-0.4.3/src/synack/plugins/templates.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/plugins/transactions.py` & `SynackAPI-0.4.3/src/synack/plugins/transactions.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/src/synack/plugins/users.py` & `SynackAPI-0.4.3/src/synack/plugins/users.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/test/test_alerts.py` & `SynackAPI-0.4.3/test/test_alerts.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/test/test_api.py` & `SynackAPI-0.4.3/test/test_api.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/test/test_auth.py` & `SynackAPI-0.4.3/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/test/test_db.py` & `SynackAPI-0.4.3/test/test_db.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/test/test_debug.py` & `SynackAPI-0.4.3/test/test_debug.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/test/test_handler.py` & `SynackAPI-0.4.3/test/test_handler.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/test/test_hydra.py` & `SynackAPI-0.4.3/test/test_hydra.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/test/test_missions.py` & `SynackAPI-0.4.3/test/test_missions.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/test/test_notifications.py` & `SynackAPI-0.4.3/test/test_notifications.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/test/test_scratchspace.py` & `SynackAPI-0.4.3/test/test_scratchspace.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/test/test_state.py` & `SynackAPI-0.4.3/test/test_state.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/test/test_targets.py` & `SynackAPI-0.4.3/test/test_targets.py`

 * *Files 2% similar despite different names*

```diff
@@ -555,14 +555,36 @@
         self.targets.db.find_targets.return_value = [Target(slug='213h89h3', codename='SASSYSQUIRREL')]
         out = self.targets.get_scope_host(codename='SASSYSQUIRREL', add_to_db=True)
         self.assertEqual(ips, out)
         self.targets.db.find_targets.assert_called_with(codename='SASSYSQUIRREL')
         self.targets.build_scope_host_db.assert_called_with('213h89h3', ips)
         self.targets.db.add_ips.assert_called_with('host_db_return_value')
 
+    def test_get_scope_host_current(self):
+        """Should get the scope for the currenly connected Host if not specified"""
+        ips = {'1.1.1.1/32', '2.2.2.2/32'}
+        self.targets.get_connected = MagicMock()
+        self.targets.get_connected.return_value = {'slug': '213h89h3'}
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
+        self.targets.db.find_targets.return_value = [Target(slug='213h89h3', codename='SASSYSQUIRREL')]
+        out = self.targets.get_scope_host()
+        self.assertEqual(ips, out)
+        self.targets.get_connected.assert_called_with()
+        self.targets.db.find_targets.assert_called_with(slug='213h89h3')
+
     def test_get_scope_host_not_ip(self):
         """Should get the scope for a Host"""
         ips = {'1.1.1.1/32'}
         self.targets.get_assets = MagicMock()
         self.targets.get_assets.return_value = [
             {
                 'active': True,
@@ -641,14 +663,45 @@
         self.targets.db.find_targets.return_value = [tgt]
         out = self.targets.get_scope_web(codename='SASSYSQUIRREL', add_to_db=True)
         self.assertEqual(scope, out)
         self.targets.build_scope_web_burp.assert_called_with(scope)
         self.targets.db.find_targets.assert_called_with(codename='SASSYSQUIRREL')
         self.targets.db.add_urls.assert_called_with(self.targets.build_scope_web_db.return_value)
 
+    def test_get_scope_web_current(self):
+        """Should get the scope for the currently connected Web Application if not specified"""
+        self.targets.build_scope_web_burp = MagicMock()
+        scope = [{
+            'listing': 'uewqhuiewq',
+            'location': 'https://good.things.com',
+            'rule': '*.good.things.com/*',
+            'status': 'in'
+        }]
+        self.targets.get_connected = MagicMock()
+        self.targets.get_connected.return_value = {'slug': '93g8eg8'}
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
+        tgt = Target(slug='213h89h3', organization='93g8eh8', codename='SASSYSQUIRREL')
+        self.targets.db.find_targets.return_value = [tgt]
+        out = self.targets.get_scope_web()
+        self.assertEqual(scope, out)
+        self.targets.build_scope_web_burp.assert_called_with(scope)
+        self.targets.get_connected.assert_called_with()
+        self.targets.db.find_targets.assert_called_with(slug='93g8eg8')
+        self.targets.get_assets.assert_called_with(target=tgt, active='true', asset_type='webapp')
+
     def test_get_submissions(self):
         """Should return the accepted vulnerabilities for a target given a slug"""
         return_data = {
             "listing_id": "u2ire",
             "type": "categories",
             "value": [{
                 "categories": ["Authorization/Permissions", "Access/Privacy Control Violation"],
```

### Comparing `SynackAPI-0.4.2/test/test_templates.py` & `SynackAPI-0.4.3/test/test_templates.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/test/test_transactions.py` & `SynackAPI-0.4.3/test/test_transactions.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.2/test/test_users.py` & `SynackAPI-0.4.3/test/test_users.py`

 * *Files identical despite different names*

