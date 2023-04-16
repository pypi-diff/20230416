# Comparing `tmp/SynackAPI-0.4.4.tar.gz` & `tmp/SynackAPI-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SynackAPI-0.4.4.tar", last modified: Sun Apr 16 07:53:03 2023, max compression
+gzip compressed data, was "SynackAPI-0.4.6.tar", last modified: Sun Apr 16 15:28:07 2023, max compression
```

## Comparing `SynackAPI-0.4.4.tar` & `SynackAPI-0.4.6.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:53:03.137378 SynackAPI-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-16 07:53:03.137378 SynackAPI-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 07:53:03.137378 SynackAPI-0.4.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:53:03.125378 SynackAPI-0.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:53:03.129378 SynackAPI-0.4.4/src/SynackAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-16 07:53:03.000000 SynackAPI-0.4.4/src/SynackAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-16 07:53:03.000000 SynackAPI-0.4.4/src/SynackAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 07:53:03.000000 SynackAPI-0.4.4/src/SynackAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-16 07:53:03.000000 SynackAPI-0.4.4/src/SynackAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 07:53:03.000000 SynackAPI-0.4.4/src/SynackAPI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:53:03.129378 SynackAPI-0.4.4/src/synack/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:53:03.129378 SynackAPI-0.4.4/src/synack/db/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:53:03.129378 SynackAPI-0.4.4/src/synack/db/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/db/alembic/README
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/db/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/db/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/db/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:53:03.133378 SynackAPI-0.4.4/src/synack/db/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/db/alembic/versions/0c1ac7be711c_added_url_table_deleted_url_from_port_.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/db/alembic/versions/349c447c0d37_added_use_scratchspace_setting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/db/alembic/versions/355984ba030b_added_notification_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/db/alembic/versions/649443e08834_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/db/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/db/alembic/versions/deb7dd07212c_added_ip_port_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/db/alembic.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:53:03.133378 SynackAPI-0.4.4/src/synack/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/db/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      447 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/db/models/category.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1579 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/db/models/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/db/models/ip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/db/models/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/db/models/port.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1059 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/db/models/target.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/db/models/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:53:03.137378 SynackAPI-0.4.4/src/synack/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/plugins/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/plugins/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/plugins/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/plugins/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17777 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/plugins/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/plugins/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/plugins/hydra.py
--rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/plugins/missions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/plugins/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/plugins/scratchspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15083 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/plugins/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/plugins/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/plugins/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/src/synack/plugins/users.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:53:03.137378 SynackAPI-0.4.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/test/test_alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    42898 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/test/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/test/test_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/test/test_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/test/test_hydra.py
--rw-r--r--   0 runner    (1001) docker     (123)    16680 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/test/test_missions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/test/test_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/test/test_scratchspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/test/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    41866 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/test/test_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/test/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/test/test_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-16 07:53:02.000000 SynackAPI-0.4.4/test/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:28:07.728061 SynackAPI-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-16 15:28:07.724061 SynackAPI-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 15:28:07.728061 SynackAPI-0.4.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:28:07.704060 SynackAPI-0.4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:28:07.708060 SynackAPI-0.4.6/src/SynackAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-16 15:28:07.000000 SynackAPI-0.4.6/src/SynackAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-04-16 15:28:07.000000 SynackAPI-0.4.6/src/SynackAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 15:28:07.000000 SynackAPI-0.4.6/src/SynackAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-16 15:28:07.000000 SynackAPI-0.4.6/src/SynackAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 15:28:07.000000 SynackAPI-0.4.6/src/SynackAPI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:28:07.708060 SynackAPI-0.4.6/src/synack/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:28:07.708060 SynackAPI-0.4.6/src/synack/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:28:07.712061 SynackAPI-0.4.6/src/synack/db/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/db/alembic/README
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/db/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/db/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/db/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:28:07.712061 SynackAPI-0.4.6/src/synack/db/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/db/alembic/versions/0c1ac7be711c_added_url_table_deleted_url_from_port_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/db/alembic/versions/349c447c0d37_added_use_scratchspace_setting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/db/alembic/versions/355984ba030b_added_notification_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/db/alembic/versions/649443e08834_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/db/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/db/alembic/versions/deb7dd07212c_added_ip_port_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/db/alembic.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:28:07.716060 SynackAPI-0.4.6/src/synack/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/db/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      447 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/db/models/category.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1579 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/db/models/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/db/models/ip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      291 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/db/models/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/db/models/port.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1059 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/db/models/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/db/models/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:28:07.720061 SynackAPI-0.4.6/src/synack/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/plugins/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/plugins/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/plugins/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/plugins/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17777 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/plugins/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/plugins/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/plugins/hydra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9143 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/plugins/missions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/plugins/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/plugins/scratchspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15084 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/plugins/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/plugins/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/plugins/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/src/synack/plugins/users.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:28:07.724061 SynackAPI-0.4.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/test/test_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10463 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42898 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/test/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/test/test_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/test/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/test/test_hydra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16680 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/test/test_missions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/test/test_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/test/test_scratchspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/test/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41863 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/test/test_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/test/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/test/test_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-16 15:28:06.000000 SynackAPI-0.4.6/test/test_users.py
```

### Comparing `SynackAPI-0.4.4/LICENSE` & `SynackAPI-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/PKG-INFO` & `SynackAPI-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SynackAPI
-Version: 0.4.4
+Version: 0.4.6
 Summary: A package to interact with Synack's API
 Home-page: https://www.github.com/bamhm182/synackAPI
 Author: bamhm182
 Author-email: bamhm182@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SynackAPI-0.4.4/README.md` & `SynackAPI-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/setup.py` & `SynackAPI-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 setuptools.setup(
     name="SynackAPI",
-    version="0.4.4",
+    version="0.4.6",
     author="bamhm182",
     author_email="bamhm182@gmail.com",
     description="A package to interact with Synack's API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.github.com/bamhm182/synackAPI",
     classifiers=[
```

### Comparing `SynackAPI-0.4.4/src/SynackAPI.egg-info/PKG-INFO` & `SynackAPI-0.4.6/src/SynackAPI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SynackAPI
-Version: 0.4.4
+Version: 0.4.6
 Summary: A package to interact with Synack's API
 Home-page: https://www.github.com/bamhm182/synackAPI
 Author: bamhm182
 Author-email: bamhm182@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SynackAPI-0.4.4/src/SynackAPI.egg-info/SOURCES.txt` & `SynackAPI-0.4.6/src/SynackAPI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/_handler.py` & `SynackAPI-0.4.6/src/synack/_handler.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/_state.py` & `SynackAPI-0.4.6/src/synack/_state.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/db/alembic/env.py` & `SynackAPI-0.4.6/src/synack/db/alembic/env.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/db/alembic/versions/0c1ac7be711c_added_url_table_deleted_url_from_port_.py` & `SynackAPI-0.4.6/src/synack/db/alembic/versions/0c1ac7be711c_added_url_table_deleted_url_from_port_.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/db/alembic/versions/349c447c0d37_added_use_scratchspace_setting.py` & `SynackAPI-0.4.6/src/synack/db/alembic/versions/349c447c0d37_added_use_scratchspace_setting.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/db/alembic/versions/355984ba030b_added_notification_settings.py` & `SynackAPI-0.4.6/src/synack/db/alembic/versions/355984ba030b_added_notification_settings.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/db/alembic/versions/649443e08834_initial.py` & `SynackAPI-0.4.6/src/synack/db/alembic/versions/649443e08834_initial.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/db/alembic/versions/deb7dd07212c_added_ip_port_tables.py` & `SynackAPI-0.4.6/src/synack/db/alembic/versions/deb7dd07212c_added_ip_port_tables.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/db/alembic.ini` & `SynackAPI-0.4.6/src/synack/db/alembic.ini`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/db/models/config.py` & `SynackAPI-0.4.6/src/synack/db/models/config.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/db/models/port.py` & `SynackAPI-0.4.6/src/synack/db/models/port.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/db/models/target.py` & `SynackAPI-0.4.6/src/synack/db/models/target.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/plugins/alerts.py` & `SynackAPI-0.4.6/src/synack/plugins/alerts.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/plugins/api.py` & `SynackAPI-0.4.6/src/synack/plugins/api.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/plugins/auth.py` & `SynackAPI-0.4.6/src/synack/plugins/auth.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/plugins/db.py` & `SynackAPI-0.4.6/src/synack/plugins/db.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/plugins/debug.py` & `SynackAPI-0.4.6/src/synack/plugins/debug.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/plugins/hydra.py` & `SynackAPI-0.4.6/src/synack/plugins/hydra.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/plugins/missions.py` & `SynackAPI-0.4.6/src/synack/plugins/missions.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/plugins/notifications.py` & `SynackAPI-0.4.6/src/synack/plugins/notifications.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/plugins/scratchspace.py` & `SynackAPI-0.4.6/src/synack/plugins/scratchspace.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/plugins/targets.py` & `SynackAPI-0.4.6/src/synack/plugins/targets.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         res = self.api.request('GET', 'assessments')
         if res.status_code == 200:
             self.db.add_categories(res.json())
             return self.db.categories
 
     def get_assets(self, target=None, asset_type=None, host_type=None, active='true',
                    scope=['in', 'discovered'], sort='location', sort_dir='asc',
-                   page=1, perPage=500, organization_uid=None, **kwargs):
+                   page=1, perPage=5000, organization_uid=None, **kwargs):
         """Get the assets (scope) of a target"""
         if target is None:
             if len(kwargs) > 0:
                 target = self.db.find_targets(**kwargs)
             else:
                 curr = self.get_connected()
                 target = self.db.find_targets(slug=curr.get('slug'))
```

### Comparing `SynackAPI-0.4.4/src/synack/plugins/templates.py` & `SynackAPI-0.4.6/src/synack/plugins/templates.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/plugins/transactions.py` & `SynackAPI-0.4.6/src/synack/plugins/transactions.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/src/synack/plugins/users.py` & `SynackAPI-0.4.6/src/synack/plugins/users.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/test/test_alerts.py` & `SynackAPI-0.4.6/test/test_alerts.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/test/test_api.py` & `SynackAPI-0.4.6/test/test_api.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/test/test_auth.py` & `SynackAPI-0.4.6/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/test/test_db.py` & `SynackAPI-0.4.6/test/test_db.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/test/test_debug.py` & `SynackAPI-0.4.6/test/test_debug.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/test/test_handler.py` & `SynackAPI-0.4.6/test/test_handler.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/test/test_hydra.py` & `SynackAPI-0.4.6/test/test_hydra.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/test/test_missions.py` & `SynackAPI-0.4.6/test/test_missions.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/test/test_notifications.py` & `SynackAPI-0.4.6/test/test_notifications.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/test/test_scratchspace.py` & `SynackAPI-0.4.6/test/test_scratchspace.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/test/test_state.py` & `SynackAPI-0.4.6/test/test_state.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/test/test_targets.py` & `SynackAPI-0.4.6/test/test_targets.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,15 +224,15 @@
         self.targets.api.request.return_value.status_code = 200
         self.targets.api.request.return_value.text = 'rettext'
         self.targets.api.request.return_value.json.return_value = 'retjson'
         self.assertEqual('retjson', self.targets.get_assets())
         self.targets.api.request.assert_called_with('GET',
                                                     'asset/v2/assets?listingUid%5B%5D=327h8iw&scope%5B%5D=in' +
                                                     '&scope%5B%5D=discovered&sort%5B%5D=location&active=true' +
-                                                    '&sortDir=asc&page=1&perPage=500')
+                                                    '&sortDir=asc&page=1&perPage=5000')
 
     def test_get_assets_non_defaults(self):
         """Should return a list of assets given information to query"""
         self.targets.db.find_targets.return_value = [Target(codename='TURBULENTTORTOISE', slug='327h8iw')]
         self.targets.api.request.return_value.status_code = 200
         self.targets.api.request.return_value.text = 'rettext'
         self.targets.api.request.return_value.json.return_value = 'retjson'
@@ -240,21 +240,21 @@
                                                             asset_type='blah',
                                                             host_type='cidr',
                                                             active='false',
                                                             scope='secret',
                                                             sort='loc',
                                                             sort_dir='desc',
                                                             page=3,
-                                                            perPage=5000,
+                                                            perPage=50,
                                                             organization_uid='uiehqw'))
         self.targets.api.request.assert_called_with('GET',
                                                     'asset/v2/assets?listingUid%5B%5D=327h8iw' +
                                                     '&organizationUid%5B%5D=uiehqw&assetType%5B%5D=blah' +
                                                     '&hostType%5B%5D=cidr&scope%5B%5D=secret' +
-                                                    '&sort%5B%5D=loc&active=false&sortDir=desc&page=3&perPage=5000')
+                                                    '&sort%5B%5D=loc&active=false&sortDir=desc&page=3&perPage=50')
 
     def test_get_attachments_current(self):
         """Should return a list of attachments based on currently selected target"""
         attachments = [
             {
                 "listing_id": "12uib",
                 "url": "https://www.download.com/uh1g23ri",
```

### Comparing `SynackAPI-0.4.4/test/test_templates.py` & `SynackAPI-0.4.6/test/test_templates.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/test/test_transactions.py` & `SynackAPI-0.4.6/test/test_transactions.py`

 * *Files identical despite different names*

### Comparing `SynackAPI-0.4.4/test/test_users.py` & `SynackAPI-0.4.6/test/test_users.py`

 * *Files identical despite different names*

