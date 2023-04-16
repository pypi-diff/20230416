# Comparing `tmp/AoE2ScenarioRms-0.2.0.tar.gz` & `tmp/AoE2ScenarioRms-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Kerwin Sneijders\Documents\Python\AoE2ScenarioRms\dist\.tmp-whpu97up\AoE2ScenarioRms-0.2.0.tar", last modified: Sun Apr 16 13:16:14 2023, max compression
+gzip compressed data, was "AoE2ScenarioRms-0.2.4.tar", last modified: Sun Apr 16 14:03:52 2023, max compression
```

## Comparing `AoE2ScenarioRms-0.2.0.tar` & `AoE2ScenarioRms-0.2.4.tar`

### file list

```diff
@@ -1,60 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 13:16:14.737705 AoE2ScenarioRms-0.2.0/
-drwxrwxrwx   0        0        0        0 2023-04-16 13:16:14.663708 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/
--rw-rw-rw-   0        0        0       34 2023-02-22 22:58:44.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/__init__.py
--rw-rw-rw-   0        0        0     1819 2023-04-16 13:05:47.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/app.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:16:14.674706 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/core/
--rw-rw-rw-   0        0        0       47 2023-02-22 22:56:39.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/core/__init__.py
--rw-rw-rw-   0        0        0     3155 2023-03-04 00:19:45.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/core/aoe2_scenario_rms.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:16:14.684706 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/debug/
--rw-rw-rw-   0        0        0      228 2023-04-16 12:07:30.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/debug/__init__.py
--rw-rw-rw-   0        0        0      987 2023-02-26 22:18:32.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/debug/apply_all_visible.py
--rw-rw-rw-   0        0        0      314 2023-02-26 22:18:32.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/debug/apply_debug.py
--rw-rw-rw-   0        0        0      515 2023-02-26 22:18:32.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/debug/apply_no_clutter.py
--rw-rw-rw-   0        0        0     1827 2023-04-16 12:08:04.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/debug/apply_state_as_black.py
--rw-rw-rw-   0        0        0      681 2023-02-26 22:18:32.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/debug/apply_xs_print.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:16:14.690705 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/enums/
--rw-rw-rw-   0        0        0      113 2023-02-23 23:24:33.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/enums/__init__.py
--rw-rw-rw-   0        0        0      378 2023-02-26 22:22:13.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/enums/grouping_method.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:16:14.693705 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/enums/internal/
--rw-rw-rw-   0        0        0        0 2023-02-22 20:34:16.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/enums/internal/__init__.py
--rw-rw-rw-   0        0        0     1439 2023-02-26 22:18:32.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/enums/internal/xs_key.py
--rw-rw-rw-   0        0        0      340 2023-02-26 22:22:59.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/enums/tile_level.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:16:14.698709 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/errors/
--rw-rw-rw-   0        0        0      222 2023-02-25 15:30:06.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/errors/__init__.py
--rw-rw-rw-   0        0        0      340 2023-02-25 15:30:05.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/errors/exceptions.py
--rw-rw-rw-   0        0        0      275 2023-02-20 00:36:32.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/errors/warnings.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:16:14.706705 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/flags/
--rw-rw-rw-   0        0        0      116 2023-02-25 13:08:12.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/flags/__init__.py
--rw-rw-rw-   0        0        0     1656 2023-02-26 22:35:11.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/flags/object_clear.py
--rw-rw-rw-   0        0        0      375 2023-04-16 12:01:49.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/flags/object_marks.py
--rw-rw-rw-   0        0        0      967 2023-04-16 13:05:47.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/flags/terrain_mark.py
--rw-rw-rw-   0        0        0      536 2023-02-23 01:07:40.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/local_config.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:16:14.711710 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/rms/
--rw-rw-rw-   0        0        0      206 2023-02-22 22:38:43.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/rms/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:16:14.717709 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/rms/create_object/
--rw-rw-rw-   0        0        0        0 2023-02-22 20:34:16.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/rms/create_object/__init__.py
--rw-rw-rw-   0        0        0     7621 2023-04-16 12:42:40.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/rms/create_object/create_object_config.py
--rw-rw-rw-   0        0        0     6502 2023-02-26 23:27:54.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/rms/create_object/create_object_feature.py
--rw-rw-rw-   0        0        0      156 2023-02-26 22:46:30.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/rms/rms_config.py
--rw-rw-rw-   0        0        0      827 2023-02-26 22:46:30.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/rms/rms_feature.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:16:14.734705 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/util/
--rw-rw-rw-   0        0        0      297 2023-02-26 22:07:17.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/util/__init__.py
--rw-rw-rw-   0        0        0     4327 2023-02-26 22:55:54.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/util/data.py
--rw-rw-rw-   0        0        0     4768 2023-04-16 11:32:10.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/util/grid_map.py
--rw-rw-rw-   0        0        0     4850 2023-04-16 12:07:30.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/util/grid_map_factory.py
--rw-rw-rw-   0        0        0     8817 2023-04-16 10:28:19.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/util/locator.py
--rw-rw-rw-   0        0        0     2539 2023-02-27 01:33:09.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/util/scenario_util.py
--rw-rw-rw-   0        0        0     2009 2023-03-04 01:17:30.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/util/tile_util.py
--rw-rw-rw-   0        0        0      754 2023-02-27 01:38:25.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/util/unit_util.py
--rw-rw-rw-   0        0        0     2864 2023-03-04 00:18:25.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/util/xs_container.py
--rw-rw-rw-   0        0        0     1243 2023-02-27 01:41:50.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/util/xs_util.py
-drwxrwxrwx   0        0        0        0 2023-04-16 13:16:14.671704 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms.egg-info/
--rw-rw-rw-   0        0        0     2993 2023-04-16 13:16:14.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1645 2023-04-16 13:16:14.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 13:16:14.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-16 13:16:14.000000 AoE2ScenarioRms-0.2.0/AoE2ScenarioRms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1067 2023-02-25 18:29:35.000000 AoE2ScenarioRms-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     2993 2023-04-16 13:16:14.736706 AoE2ScenarioRms-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2332 2023-04-16 12:12:40.000000 AoE2ScenarioRms-0.2.0/README.md
--rw-rw-rw-   0        0        0      870 2023-04-16 13:05:02.000000 AoE2ScenarioRms-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 13:16:14.737705 AoE2ScenarioRms-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.186286 AoE2ScenarioRms-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.182286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.182286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/core/aoe2_scenario_rms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.182286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/debug/apply_all_visible.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/debug/apply_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/debug/apply_no_clutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/debug/apply_state_as_black.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/debug/apply_xs_print.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.182286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/enums/grouping_method.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.182286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/enums/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/enums/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/enums/internal/xs_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/enums/tile_level.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.182286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/errors/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/errors/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.182286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/flags/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/flags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/flags/object_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/flags/object_marks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/flags/terrain_mark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.186286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.186286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/create_object/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/create_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/create_object/create_object_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/create_object/create_object_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/rms_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/rms_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.186286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/grid_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/grid_map_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/scenario_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/tile_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/unit_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/xs_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/xs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.182286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-16 14:03:52.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-16 14:03:52.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 14:03:52.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-16 14:03:52.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-16 14:03:52.186286 AoE2ScenarioRms-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 14:03:52.186286 AoE2ScenarioRms-0.2.4/setup.cfg
```

### Comparing `AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/core/aoe2_scenario_rms.py` & `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/core/aoe2_scenario_rms.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from pathlib import Path
-from typing import List
-
-from AoE2ScenarioParser.scenarios.aoe2_de_scenario import AoE2DEScenario
-
-from AoE2ScenarioRms.enums import XsKey
-from AoE2ScenarioRms.errors import InvalidAoE2ScenarioRmsState
-from AoE2ScenarioRms.rms import CreateObjectConfig, CreateObjectFeature
-from AoE2ScenarioRms.util import GridMap, XsContainer, XsUtil
-
-
-class AoE2ScenarioRms:
-
-    def __init__(self, scenario: AoE2DEScenario):
-        """
-        Core class of this AoE2ScenarioParser plugin (?). Manages the 'overarching' functionality of adding RMS features to
-        the given scenario
-
-        Args:
-            scenario: The scenario to edit with this plugin (?)
-        """
-        self.scenario: AoE2DEScenario = scenario
-        self.xs_container: XsContainer = XsContainer()
-        self._debug_applied = False
-
-        scenario.xs_manager.initialise_xs_trigger()
-        scenario.xs_manager.add_script(xs_file_path=str((Path(__file__).parent.parent / 'xs' / 'random.xs').resolve()))
-
-        self._register_scenario_write_to_file_event()
-
-    def create_objects(self, configs: List[CreateObjectConfig], grid_map: GridMap) -> None:
-        """
-        Add a set of <create object> configs to your scenario. This represents the ``create_object`` blocks in the
-        ``<OBJECTS_GENERATION>`` section of an RMS script.
-
-        Args:
-            configs: The configs for this create object block
-            grid_map: The grid map marking the area where this block should (not) be applied
-        """
-        self._verify_no_debug()
-
-        create_objects = CreateObjectFeature(self.scenario)
-        self.xs_container += create_objects.solve(configs, grid_map)
-
-    def _verify_no_debug(self) -> None:
-        """
-        Verify if no debug classes have been applied to this scenario
-
-        Raises:
-            InvalidAoE2ScenarioRmsState: When debug functions have previously been applied to this scenario
-        """
-        if self._debug_applied:
-            raise InvalidAoE2ScenarioRmsState(
-                "Debug applied before RMS functionality is called. "
-                "Please ONLY apply debug just before `scenario.write_to_file(...)`."
-            )
-
-    def _register_scenario_write_to_file_event(self) -> None:
-        """
-        Overwrites the ``write_to_file`` function of the scenario to add custom functionality like adding the necessary
-        XS scripts to the scenario.
-        """
-        original_write_to_file = self.scenario.write_to_file
-
-        def write_to_file_wrapper(filename: str, skip_reconstruction: bool = False):
-            variable_count = str(len(self.xs_container.get(XsKey.RESOURCE_VARIABLE_DECLARATION)))
-            self.xs_container.append(XsKey.RESOURCE_VARIABLE_COUNT, variable_count)
-
-            xs_string = self.xs_container.resolve(XsUtil.file('main.xs'))
-            self.scenario.xs_manager.add_script(xs_string=xs_string)
-
-            original_write_to_file(filename, skip_reconstruction)
-
-        self.scenario.write_to_file = write_to_file_wrapper
-        self._debug_all_visible_enabled = True
+from pathlib import Path
+from typing import List
+
+from AoE2ScenarioParser.scenarios.aoe2_de_scenario import AoE2DEScenario
+
+from AoE2ScenarioRms.enums import XsKey
+from AoE2ScenarioRms.errors import InvalidAoE2ScenarioRmsState
+from AoE2ScenarioRms.rms import CreateObjectConfig, CreateObjectFeature
+from AoE2ScenarioRms.util import GridMap, XsContainer, XsUtil
+
+
+class AoE2ScenarioRms:
+
+    def __init__(self, scenario: AoE2DEScenario):
+        """
+        Core class of this AoE2ScenarioParser plugin (?). Manages the 'overarching' functionality of adding RMS features to
+        the given scenario
+
+        Args:
+            scenario: The scenario to edit with this plugin (?)
+        """
+        self.scenario: AoE2DEScenario = scenario
+        self.xs_container: XsContainer = XsContainer()
+        self._debug_applied = False
+
+        scenario.xs_manager.initialise_xs_trigger()
+        scenario.xs_manager.add_script(xs_file_path=str((Path(__file__).parent.parent / 'xs' / 'random.xs').resolve()))
+
+        self._register_scenario_write_to_file_event()
+
+    def create_objects(self, configs: List[CreateObjectConfig], grid_map: GridMap) -> None:
+        """
+        Add a set of <create object> configs to your scenario. This represents the ``create_object`` blocks in the
+        ``<OBJECTS_GENERATION>`` section of an RMS script.
+
+        Args:
+            configs: The configs for this create object block
+            grid_map: The grid map marking the area where this block should (not) be applied
+        """
+        self._verify_no_debug()
+
+        create_objects = CreateObjectFeature(self.scenario)
+        self.xs_container += create_objects.solve(configs, grid_map)
+
+    def _verify_no_debug(self) -> None:
+        """
+        Verify if no debug classes have been applied to this scenario
+
+        Raises:
+            InvalidAoE2ScenarioRmsState: When debug functions have previously been applied to this scenario
+        """
+        if self._debug_applied:
+            raise InvalidAoE2ScenarioRmsState(
+                "Debug applied before RMS functionality is called. "
+                "Please ONLY apply debug just before `scenario.write_to_file(...)`."
+            )
+
+    def _register_scenario_write_to_file_event(self) -> None:
+        """
+        Overwrites the ``write_to_file`` function of the scenario to add custom functionality like adding the necessary
+        XS scripts to the scenario.
+        """
+        original_write_to_file = self.scenario.write_to_file
+
+        def write_to_file_wrapper(filename: str, skip_reconstruction: bool = False):
+            variable_count = str(len(self.xs_container.get(XsKey.RESOURCE_VARIABLE_DECLARATION)))
+            self.xs_container.append(XsKey.RESOURCE_VARIABLE_COUNT, variable_count)
+
+            xs_string = self.xs_container.resolve(XsUtil.file('main.xs'))
+            self.scenario.xs_manager.add_script(xs_string=xs_string)
+
+            original_write_to_file(filename, skip_reconstruction)
+
+        self.scenario.write_to_file = write_to_file_wrapper
+        self._debug_all_visible_enabled = True
```

### Comparing `AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/debug/apply_state_as_black.py` & `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/debug/apply_state_as_black.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-from typing import TYPE_CHECKING
-
-from AoE2ScenarioParser.datasets.terrains import TerrainId
-from AoE2ScenarioParser.helper.helper import xy_to_i
-
-from AoE2ScenarioRms.debug.apply_debug import ApplyDebug
-from AoE2ScenarioRms.util import GridMap
-
-if TYPE_CHECKING:
-    from AoE2ScenarioRms import AoE2ScenarioRms
-
-
-class ApplyStateAsBlack(ApplyDebug):
-    """
-
-    Change all terrain tiles that are <state> (in the gridmap) to ``TerrainId.BLACK``
-
-    """
-
-    def __init__(self, rms: 'AoE2ScenarioRms', grid_map: 'GridMap', as_layer: bool = False) -> None:
-        super().__init__(rms)
-
-        mm = rms.scenario.map_manager
-        map_size = mm.map_size
-
-        for y in range(map_size):
-            for x in range(map_size):
-                if self.tile_should_be_black(grid_map, x, y):
-                    if as_layer:
-                        mm.terrain[xy_to_i(x, y, map_size)].layer = TerrainId.BLACK
-                    else:
-                        mm.terrain[xy_to_i(x, y, map_size)].terrain_id = TerrainId.BLACK
-
-    def tile_should_be_black(self, grid_map: 'GridMap', x: int, y: int) -> bool:
-        raise NotImplementedError("The function 'tile_should_be_black' was not implemented for this class")
-
-
-class ApplyBlockedAsBlack(ApplyStateAsBlack):
-    """
-
-    Change all terrain tiles that are blocked (in the gridmap) to ``TerrainId.BLACK``
-
-    """
-
-    def tile_should_be_black(self, grid_map: 'GridMap', x: int, y: int) -> bool:
-        return grid_map.is_blocked(x, y)
-
-
-class ApplyAvailableAsBlack(ApplyStateAsBlack):
-    """
-
-    Change all terrain tiles that are available (in the gridmap) to ``TerrainId.BLACK``
-
-    """
-
-    def tile_should_be_black(self, grid_map: 'GridMap', x: int, y: int) -> bool:
-        return grid_map.is_available(x, y)
+from typing import TYPE_CHECKING
+
+from AoE2ScenarioParser.datasets.terrains import TerrainId
+from AoE2ScenarioParser.helper.helper import xy_to_i
+
+from AoE2ScenarioRms.debug.apply_debug import ApplyDebug
+from AoE2ScenarioRms.util import GridMap
+
+if TYPE_CHECKING:
+    from AoE2ScenarioRms import AoE2ScenarioRms
+
+
+class ApplyStateAsBlack(ApplyDebug):
+    """
+
+    Change all terrain tiles that are <state> (in the gridmap) to ``TerrainId.BLACK``
+
+    """
+
+    def __init__(self, rms: 'AoE2ScenarioRms', grid_map: 'GridMap', as_layer: bool = False) -> None:
+        super().__init__(rms)
+
+        mm = rms.scenario.map_manager
+        map_size = mm.map_size
+
+        for y in range(map_size):
+            for x in range(map_size):
+                if self.tile_should_be_black(grid_map, x, y):
+                    if as_layer:
+                        mm.terrain[xy_to_i(x, y, map_size)].layer = TerrainId.BLACK
+                    else:
+                        mm.terrain[xy_to_i(x, y, map_size)].terrain_id = TerrainId.BLACK
+
+    def tile_should_be_black(self, grid_map: 'GridMap', x: int, y: int) -> bool:
+        raise NotImplementedError("The function 'tile_should_be_black' was not implemented for this class")
+
+
+class ApplyBlockedAsBlack(ApplyStateAsBlack):
+    """
+
+    Change all terrain tiles that are blocked (in the gridmap) to ``TerrainId.BLACK``
+
+    """
+
+    def tile_should_be_black(self, grid_map: 'GridMap', x: int, y: int) -> bool:
+        return grid_map.is_blocked(x, y)
+
+
+class ApplyAvailableAsBlack(ApplyStateAsBlack):
+    """
+
+    Change all terrain tiles that are available (in the gridmap) to ``TerrainId.BLACK``
+
+    """
+
+    def tile_should_be_black(self, grid_map: 'GridMap', x: int, y: int) -> bool:
+        return grid_map.is_available(x, y)
```

### Comparing `AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/enums/internal/xs_key.py` & `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/enums/internal/xs_key.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from __future__ import annotations
-
-from enum import Enum, auto
-
-
-class XsKey(Enum):
-    """
-    Enum used to identify the different sections of an XS script that can be replaced.
-    Only really useful in conjunction with ``XsContainer``
-    """
-    RESOURCE_VARIABLE_DECLARATION = auto()
-    RESOURCE_VARIABLE_COUNT = auto()
-    RESOURCE_COUNT_DECLARATION = auto()
-    RESOURCE_MAX_SPAWN_DECLARATION = auto()
-    RESOURCE_MAX_SPAWN_IS_PER_PLAYER_DECLARATION = auto()
-    RESOURCE_LOCATION_INJECTION = auto()
-    RESOURCE_GROUP_NAMES_DECLARATION = auto()
-
-    CONFIG_DECLARATION = auto()
-
-    AFTER_RESOURCE_SPAWN_EVENT = auto()
-
-    XS_ON_INIT_FILE = auto()
-    XS_ON_INIT_RULE = auto()
-
-    XS_ON_SUCCESSFUL_SPAWN = auto()
-
-    @staticmethod
-    def join_string(key: XsKey):
-        return _xs_join_strings[key]
-
-
-_xs_join_strings = {
-    XsKey.RESOURCE_VARIABLE_COUNT: '',
-
-    XsKey.RESOURCE_VARIABLE_DECLARATION: '\n',
-    XsKey.XS_ON_INIT_FILE: '\n',
-
-    XsKey.RESOURCE_GROUP_NAMES_DECLARATION: '\n\t',
-    XsKey.RESOURCE_COUNT_DECLARATION: '\n\t',
-    XsKey.RESOURCE_MAX_SPAWN_DECLARATION: '\n\t',
-    XsKey.RESOURCE_MAX_SPAWN_IS_PER_PLAYER_DECLARATION: '\n\t',
-    XsKey.RESOURCE_LOCATION_INJECTION: '\n\t',
-    XsKey.CONFIG_DECLARATION: '\n\t',
-    XsKey.XS_ON_INIT_RULE: '\n\t',
-
-    XsKey.AFTER_RESOURCE_SPAWN_EVENT: '\n\t\t',
-
-    XsKey.XS_ON_SUCCESSFUL_SPAWN: '\n\t\t\t',
-}
+from __future__ import annotations
+
+from enum import Enum, auto
+
+
+class XsKey(Enum):
+    """
+    Enum used to identify the different sections of an XS script that can be replaced.
+    Only really useful in conjunction with ``XsContainer``
+    """
+    RESOURCE_VARIABLE_DECLARATION = auto()
+    RESOURCE_VARIABLE_COUNT = auto()
+    RESOURCE_COUNT_DECLARATION = auto()
+    RESOURCE_MAX_SPAWN_DECLARATION = auto()
+    RESOURCE_MAX_SPAWN_IS_PER_PLAYER_DECLARATION = auto()
+    RESOURCE_LOCATION_INJECTION = auto()
+    RESOURCE_GROUP_NAMES_DECLARATION = auto()
+
+    CONFIG_DECLARATION = auto()
+
+    AFTER_RESOURCE_SPAWN_EVENT = auto()
+
+    XS_ON_INIT_FILE = auto()
+    XS_ON_INIT_RULE = auto()
+
+    XS_ON_SUCCESSFUL_SPAWN = auto()
+
+    @staticmethod
+    def join_string(key: XsKey):
+        return _xs_join_strings[key]
+
+
+_xs_join_strings = {
+    XsKey.RESOURCE_VARIABLE_COUNT: '',
+
+    XsKey.RESOURCE_VARIABLE_DECLARATION: '\n',
+    XsKey.XS_ON_INIT_FILE: '\n',
+
+    XsKey.RESOURCE_GROUP_NAMES_DECLARATION: '\n\t',
+    XsKey.RESOURCE_COUNT_DECLARATION: '\n\t',
+    XsKey.RESOURCE_MAX_SPAWN_DECLARATION: '\n\t',
+    XsKey.RESOURCE_MAX_SPAWN_IS_PER_PLAYER_DECLARATION: '\n\t',
+    XsKey.RESOURCE_LOCATION_INJECTION: '\n\t',
+    XsKey.CONFIG_DECLARATION: '\n\t',
+    XsKey.XS_ON_INIT_RULE: '\n\t',
+
+    XsKey.AFTER_RESOURCE_SPAWN_EVENT: '\n\t\t',
+
+    XsKey.XS_ON_SUCCESSFUL_SPAWN: '\n\t\t\t',
+}
```

### Comparing `AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/flags/object_clear.py` & `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/flags/object_clear.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/flags/terrain_mark.py` & `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/flags/terrain_mark.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/rms/create_object/create_object_config.py` & `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/create_object/create_object_config.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,190 +1,190 @@
-from __future__ import annotations
-
-import math
-import random
-from typing import Generator
-
-from AoE2ScenarioParser.helper.printers import warn
-
-from AoE2ScenarioRms.errors import InvalidCreateObjectError, ImproperCreateObjectWarning
-from AoE2ScenarioRms.enums import GroupingMethod
-from AoE2ScenarioRms.rms.rms_config import RmsConfig
-from AoE2ScenarioRms.util import XsUtil
-
-
-class CreateObjectConfig(RmsConfig):
-    """
-    An object that holds the configuration of a single object group
-
-    *An effort was made to make these keys to be somewhat the same to RMS `<create_object>` options.*
-
-    ----
-
-    Usual configuration.
-
-    ----
-
-    **name**:
-        **[REQUIRED]** The name for this config, needs to be unique
-
-    **const**:
-        **[REQUIRED]** The unit to spawn. If a list is given this will be randomized per group so is **NOT** useful
-        for spawning equal & fair resources.
-
-    **grouping**:
-        The spread method. Use: ``GroupingMethod.TIGHT`` for spawning like gold, or: ``GroupingMethod.LOOSE`` for
-        spawning like deer. Defaults to: ``GroupingMethod.TIGHT``
-
-    **number_of_objects**:
-        The size of a single group (Amount of objects per group).
-        Accepts an ``int`` or a ``tuple[int, int]`` indicating a range ([1, 3] can spawn 1, 2 or 3 objects in a group).
-        This value randomized per group so is **NOT** useful for spawning equal & fair resources. Defaults to 1
-
-    **group_placement_radius**:
-        **[NOT IMPLEMENTED]** The number of tiles out from the central tile that objects belonging to the same group
-        may spawn. Defaults to 3
-
-    **number_of_groups**:
-        The maximum amount of groups to spawn. Can be a float when using `scale_to_player_number`. When left unchanged
-        the maximum amount of spawns will be the maximum of groups that fits in the map. Defaults to infinity
-
-    **loose_grouping_distance**:
-        The distance at which resources should spawn from each other in the same group. Ignored when ``grouping`` is
-        not set to ``GroupingMethod.LOOSE``. Defaults to 3
-
-    **min_distance_group_placement**:
-        The minimum distance in tiles to groups of OTHER create object config
-
-    **temp_min_distance_group_placement**:
-        The minimum distance in tiles to groups of THIS create object config
-
-    **min_distance_to_map_edge**:
-        **[NOT IMPLEMENTED]** The minimum distance in tiles that groups will stay away from the map edge
-
-    **scale_to_player_number**:
-        If the number of groups should be affected by the player number. When set to True, the number_of_groups value
-        is multiplied with the number of players
-        With this enabled and ... (Examples)::
-           ... 'number_of_groups' to 3 with 2 players will result in 6 spawns
-           ... 'number_of_groups' to 0.5 with 6 players will result in 3 spawns
-           ... 'number_of_groups' to 0.4 with 1, 2 or 3 player(s) will all result in a single spawn
-
-    ----
-
-    MetaData
-
-    ----
-
-    These configuration settings are necessary for the spawning of the objects or the processes around it
-
-    **object_size**:
-        The size of the object, a unit is 1x1 so this can be left blank as 1 is the default, a house is 2x2 so set this
-        to 2. Farm is 3x3 so set this to 3 etc. -- If this isn't properly configured the grid map might not be taken
-        into account properly.
-
-    ----
-
-    Parser related configurations
-
-    ----
-
-    These configuration settings affect how the groups are generated **IN THE SCENARIO**. This means these settings will
-    affect the triggers and XS generated. *Leave as-is if you don't know what they do*
-
-    **_max_potential_group_count**:
-        [PARSER GENERATION] The total amount of groups to **generate** on a map
-
-    **_debug_place_all**:
-        [DEBUG] Force all groups to be placed directly in the map. Not recommended with a high
-        ``_max_potential_group_count``
-    """
-
-    unique_names = set()
-
-    def __init__(
-            self,
-            name: str,
-            const: int | list[int],
-            grouping: GroupingMethod = GroupingMethod.TIGHT,
-            number_of_objects: int | tuple[int, int] = 1,
-            group_placement_radius: int = 3,
-            number_of_groups: float = 999_999_999,  # Cannot be math.inf as `str(...)` is used within xs
-            loose_grouping_distance: int = None,
-            min_distance_group_placement: int = 4,
-            temp_min_distance_group_placement: int = 20,
-            min_distance_to_map_edge: int = 0,
-            scale_to_player_number: bool = False,
-
-            # ----- Meta Data -----
-            object_size=1,
-
-            # ----- Debug & Parser -----
-            _max_potential_group_count: int = 250,
-            _debug_place_all: bool = False
-    ):
-        super().__init__()
-
-        name = self._validate_name_unique(name)\
-            .lower()
-
-        if scale_to_player_number and number_of_groups > 100_000:
-            raise InvalidCreateObjectError(
-                f"[{name}]: cannot use scale with player number when number of groups is above 100k"
-            )
-
-        if not isinstance(number_of_objects, int) and not isinstance(number_of_objects, tuple):
-            raise TypeError(f"[{name}]: number_of_objects has to be either int or tuple[int, int], "
-                            f"not: {type(number_of_objects)}.")
-
-        if grouping is not GroupingMethod.LOOSE and loose_grouping_distance is not None:
-            warn(f"[{name}]: Setting 'loose_grouping_distance' without GroupingMethod.LOOSE has no effect",
-                 ImproperCreateObjectWarning)
-
-        if loose_grouping_distance is None:
-            loose_grouping_distance = 3
-
-        self.name: str = name
-        self.const: int = const
-        self.grouping: GroupingMethod = grouping
-        self.number_of_objects: int | tuple[int, int] = number_of_objects
-        self.group_placement_radius: int = group_placement_radius  # Todo: Implement
-        self.number_of_groups: float = number_of_groups
-        self.loose_grouping_distance: int = loose_grouping_distance
-        self.min_distance_group_placement: int = min_distance_group_placement
-        self.temp_min_distance_group_placement: int = temp_min_distance_group_placement
-        self.min_distance_to_map_edge: int = min_distance_to_map_edge  # Todo: Implement
-        self.scale_to_player_number: bool = scale_to_player_number
-
-        self.object_size = object_size
-
-        self.max_potential_group_count: int = _max_potential_group_count
-        self.debug_place_all: bool = _debug_place_all
-
-        self.index = next(_counter)
-
-    @staticmethod
-    def _validate_name_unique(name: str) -> str:
-        xs_name = XsUtil.constant(name)
-
-        if xs_name in CreateObjectConfig.unique_names:
-            raise InvalidCreateObjectError(
-                f"[{name}]: group with name '{name}' ('{xs_name}') already exists. Make sure all names are unique and "
-                f"aren't differentiated through just casing or spaces."
-            )
-        CreateObjectConfig.unique_names.add(xs_name)
-
-        return xs_name
-
-    def get_random_const(self) -> int:
-        if isinstance(self.const, list):
-            return random.choice(self.const)
-        else:
-            return self.const
-
-
-def _create_counter_generator() -> Generator[int]:
-    for i in range(999_999_999):
-        yield i
-
-
-_counter = _create_counter_generator()
+from __future__ import annotations
+
+import math
+import random
+from typing import Generator
+
+from AoE2ScenarioParser.helper.printers import warn
+
+from AoE2ScenarioRms.errors import InvalidCreateObjectError, ImproperCreateObjectWarning
+from AoE2ScenarioRms.enums import GroupingMethod
+from AoE2ScenarioRms.rms.rms_config import RmsConfig
+from AoE2ScenarioRms.util import XsUtil
+
+
+class CreateObjectConfig(RmsConfig):
+    """
+    An object that holds the configuration of a single object group
+
+    *An effort was made to make these keys to be somewhat the same to RMS `<create_object>` options.*
+
+    ----
+
+    Usual configuration.
+
+    ----
+
+    **name**:
+        **[REQUIRED]** The name for this config, needs to be unique
+
+    **const**:
+        **[REQUIRED]** The unit to spawn. If a list is given this will be randomized per group so is **NOT** useful
+        for spawning equal & fair resources.
+
+    **grouping**:
+        The spread method. Use: ``GroupingMethod.TIGHT`` for spawning like gold, or: ``GroupingMethod.LOOSE`` for
+        spawning like deer. Defaults to: ``GroupingMethod.TIGHT``
+
+    **number_of_objects**:
+        The size of a single group (Amount of objects per group).
+        Accepts an ``int`` or a ``tuple[int, int]`` indicating a range ([1, 3] can spawn 1, 2 or 3 objects in a group).
+        This value randomized per group so is **NOT** useful for spawning equal & fair resources. Defaults to 1
+
+    **group_placement_radius**:
+        **[NOT IMPLEMENTED]** The number of tiles out from the central tile that objects belonging to the same group
+        may spawn. Defaults to 3
+
+    **number_of_groups**:
+        The maximum amount of groups to spawn. Can be a float when using `scale_to_player_number`. When left unchanged
+        the maximum amount of spawns will be the maximum of groups that fits in the map. Defaults to infinity
+
+    **loose_grouping_distance**:
+        The distance at which resources should spawn from each other in the same group. Ignored when ``grouping`` is
+        not set to ``GroupingMethod.LOOSE``. Defaults to 3
+
+    **min_distance_group_placement**:
+        The minimum distance in tiles to groups of OTHER create object config
+
+    **temp_min_distance_group_placement**:
+        The minimum distance in tiles to groups of THIS create object config
+
+    **min_distance_to_map_edge**:
+        **[NOT IMPLEMENTED]** The minimum distance in tiles that groups will stay away from the map edge
+
+    **scale_to_player_number**:
+        If the number of groups should be affected by the player number. When set to True, the number_of_groups value
+        is multiplied with the number of players
+        With this enabled and ... (Examples)::
+           ... 'number_of_groups' to 3 with 2 players will result in 6 spawns
+           ... 'number_of_groups' to 0.5 with 6 players will result in 3 spawns
+           ... 'number_of_groups' to 0.4 with 1, 2 or 3 player(s) will all result in a single spawn
+
+    ----
+
+    MetaData
+
+    ----
+
+    These configuration settings are necessary for the spawning of the objects or the processes around it
+
+    **object_size**:
+        The size of the object, a unit is 1x1 so this can be left blank as 1 is the default, a house is 2x2 so set this
+        to 2. Farm is 3x3 so set this to 3 etc. -- If this isn't properly configured the grid map might not be taken
+        into account properly.
+
+    ----
+
+    Parser related configurations
+
+    ----
+
+    These configuration settings affect how the groups are generated **IN THE SCENARIO**. This means these settings will
+    affect the triggers and XS generated. *Leave as-is if you don't know what they do*
+
+    **_max_potential_group_count**:
+        [PARSER GENERATION] The total amount of groups to **generate** on a map
+
+    **_debug_place_all**:
+        [DEBUG] Force all groups to be placed directly in the map. Not recommended with a high
+        ``_max_potential_group_count``
+    """
+
+    unique_names = set()
+
+    def __init__(
+            self,
+            name: str,
+            const: int | list[int],
+            grouping: GroupingMethod = GroupingMethod.TIGHT,
+            number_of_objects: int | tuple[int, int] = 1,
+            group_placement_radius: int = 3,
+            number_of_groups: float = 999_999_999,  # Cannot be math.inf as `str(...)` is used within xs
+            loose_grouping_distance: int = None,
+            min_distance_group_placement: int = 4,
+            temp_min_distance_group_placement: int = 20,
+            min_distance_to_map_edge: int = 0,
+            scale_to_player_number: bool = False,
+
+            # ----- Meta Data -----
+            object_size=1,
+
+            # ----- Debug & Parser -----
+            _max_potential_group_count: int = 250,
+            _debug_place_all: bool = False
+    ):
+        super().__init__()
+
+        name = self._validate_name_unique(name)\
+            .lower()
+
+        if scale_to_player_number and number_of_groups > 100_000:
+            raise InvalidCreateObjectError(
+                f"[{name}]: cannot use scale with player number when number of groups is above 100k"
+            )
+
+        if not isinstance(number_of_objects, int) and not isinstance(number_of_objects, tuple):
+            raise TypeError(f"[{name}]: number_of_objects has to be either int or tuple[int, int], "
+                            f"not: {type(number_of_objects)}.")
+
+        if grouping is not GroupingMethod.LOOSE and loose_grouping_distance is not None:
+            warn(f"[{name}]: Setting 'loose_grouping_distance' without GroupingMethod.LOOSE has no effect",
+                 ImproperCreateObjectWarning)
+
+        if loose_grouping_distance is None:
+            loose_grouping_distance = 3
+
+        self.name: str = name
+        self.const: int = const
+        self.grouping: GroupingMethod = grouping
+        self.number_of_objects: int | tuple[int, int] = number_of_objects
+        self.group_placement_radius: int = group_placement_radius  # Todo: Implement
+        self.number_of_groups: float = number_of_groups
+        self.loose_grouping_distance: int = loose_grouping_distance
+        self.min_distance_group_placement: int = min_distance_group_placement
+        self.temp_min_distance_group_placement: int = temp_min_distance_group_placement
+        self.min_distance_to_map_edge: int = min_distance_to_map_edge  # Todo: Implement
+        self.scale_to_player_number: bool = scale_to_player_number
+
+        self.object_size = object_size
+
+        self.max_potential_group_count: int = _max_potential_group_count
+        self.debug_place_all: bool = _debug_place_all
+
+        self.index = next(_counter)
+
+    @staticmethod
+    def _validate_name_unique(name: str) -> str:
+        xs_name = XsUtil.constant(name)
+
+        if xs_name in CreateObjectConfig.unique_names:
+            raise InvalidCreateObjectError(
+                f"[{name}]: group with name '{name}' ('{xs_name}') already exists. Make sure all names are unique and "
+                f"aren't differentiated through just casing or spaces."
+            )
+        CreateObjectConfig.unique_names.add(xs_name)
+
+        return xs_name
+
+    def get_random_const(self) -> int:
+        if isinstance(self.const, list):
+            return random.choice(self.const)
+        else:
+            return self.const
+
+
+def _create_counter_generator() -> Generator[int]:
+    for i in range(999_999_999):
+        yield i
+
+
+_counter = _create_counter_generator()
```

### Comparing `AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/rms/create_object/create_object_feature.py` & `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/create_object/create_object_feature.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING, List
-
-from AoE2ScenarioParser.datasets.other import OtherInfo
-from AoE2ScenarioParser.datasets.players import PlayerId
-from AoE2ScenarioParser.scenarios.aoe2_de_scenario import AoE2DEScenario
-
-from AoE2ScenarioRms.enums import XsKey
-from AoE2ScenarioRms.errors import InvalidCreateObjectError
-from AoE2ScenarioRms.rms.create_object.create_object_config import CreateObjectConfig
-from AoE2ScenarioRms.rms.rms_feature import RmsFeature
-from AoE2ScenarioRms.util import XsUtil, XsContainer, Locator
-
-if TYPE_CHECKING:
-    from AoE2ScenarioRms.util import GridMap
-
-
-class CreateObjectFeature(RmsFeature):
-    unique_names = set()
-
-    def __init__(self, scenario: AoE2DEScenario) -> None:
-        """
-        Class that manages the functionality behind implementing the create_object clause
-
-        Args:
-            scenario: The scenario to apply the configs to
-        """
-        container = XsContainer()
-
-        super().__init__(scenario, container)
-
-    def init(self, config: CreateObjectConfig) -> None:
-        """
-        Initialize the 'create object' configurations. Setting XS initializers like variable and array definitions
-
-        Args:
-            config: The configs to be added
-        """
-        name = self._name(config)
-
-        self._validate_name_unique(name)
-
-        self.xs_container.append(
-            XsKey.RESOURCE_VARIABLE_DECLARATION,
-            f"int {name} = {config.index};"
-        )
-
-        self.xs_container.append(
-            XsKey.RESOURCE_GROUP_NAMES_DECLARATION,
-            f"xsArraySetString(__RESOURCE_GROUP_NAMES, {name}, \"{config.name}\");"
-        )
-
-        self.xs_container.append(
-            XsKey.RESOURCE_COUNT_DECLARATION,
-            f"xsArraySetInt(__RESOURCE_SPAWN_COUNTS, {name}, {config.max_potential_group_count});"
-        )
-
-        self.xs_container.append(
-            XsKey.RESOURCE_MAX_SPAWN_DECLARATION,
-            f"xsArraySetFloat(__RESOURCE_MAX_SPAWN_COUNTS, {name}, {config.number_of_groups});"
-        )
-
-        bool_ = XsUtil.bool(config.scale_to_player_number)
-        self.xs_container.append(
-            XsKey.RESOURCE_MAX_SPAWN_IS_PER_PLAYER_DECLARATION,
-            f"xsArraySetBool(__RESOURCE_MAX_SPAWN_COUNTS_IS_PER_PLAYER, {name}, {bool_});"
-        )
-
-        self.xs_container.append(
-            XsKey.RESOURCE_LOCATION_INJECTION,
-            f"rArray = xsArrayGetInt(__ARRAY_RESOURCE_LOCATIONS, {name});"
-        )
-
-        self.xs_container.extend(
-            XsKey.CONFIG_DECLARATION,
-            [
-                f"cArray = xsArrayGetInt(__ARRAY_RESOURCE_CONFIGS, {name});",
-                f"xsArraySetInt(cArray, 0, {config.temp_min_distance_group_placement});",
-                f"xsArraySetInt(cArray, 1, {config.min_distance_group_placement});",
-            ]
-        )
-
-    def build(self, config: CreateObjectConfig, grid_map: 'GridMap') -> None:
-        """
-        Write the functional logic (triggers) for placing the objects. Also write the functional and conditional logic
-        for XS for the given configs.
-
-        Args:
-            config: The config to implement
-            grid_map: The GridMap to take into account when generating potential locations for groups
-        """
-        tm, um = self.scenario.trigger_manager, self.scenario.unit_manager
-        name = self._name(config)
-
-        groups = Locator.create_groups(config, grid_map)
-
-        for index, group in enumerate(groups):
-            spawn_group = tm.add_trigger(f"Spawn {config.name} {index}/{len(groups)}")
-            group_const = config.get_random_const()
-
-            function = f"bool __should_spawn_{config.name}_{index}() {{" \
-                f"return (xsArrayGetBool(xsArrayGetInt(__ARRAY_RESOURCE_PLACED_INDICES, {name}), {index}));" \
-                f"}}"
-            spawn_group.new_condition.script_call(xs_function=function.strip().replace('  ', ''))
-
-            for iindex, tile in enumerate(group):
-                spawn_group.new_effect.create_object(group_const, PlayerId.GAIA, tile.x, tile.y)
-
-                if config.debug_place_all:
-                    um.add_unit(PlayerId.GAIA, group_const, tile.x + .5, tile.y + .5)
-                    player = PlayerId.GAIA if iindex == 0 else PlayerId.ONE
-                    const = OtherInfo.FLAG_M.ID if iindex == 0 else OtherInfo.FLAG_C.ID
-                    um.add_unit(player, const, tile.x + .5, tile.y + .5)
-
-            self.xs_container.append(
-                XsKey.RESOURCE_LOCATION_INJECTION,
-                f"xsArraySetVector(rArray, {index}, vector({group[0].x}, {group[0].y}, -1));\t// {index}"
-            )
-        self.xs_container.append(
-            XsKey.RESOURCE_LOCATION_INJECTION,
-            f"ShuffleVectorArray(rArray, xsArrayGetInt(__ARRAY_RESOURCE_INDICES, {name}));"
-        )
-
-    def solve(self, configs: List[CreateObjectConfig], grid_map: 'GridMap') -> XsContainer:
-        """
-        Execute the init and build steps in one go for each config given.
-
-        Args:
-            configs: The configs to implement
-            grid_map: The GridMap to take into account when generating potential locations for groups of configs
-
-        Returns:
-            The XsContainer with all generated XS
-        """
-        for config_entry in configs:
-            self.init(config_entry)
-            self.build(config_entry, grid_map)
-        return self.xs_container
-
-    @staticmethod
-    def _validate_name_unique(name: str) -> None:
-        """
-        Validate if the given name is unique compared to other names used
-
-        Args:
-            name: The name to validate
-
-        Raises:
-            InvalidCreateObjectError: If the given name has already been registered before in the scenario
-        """
-        if name in CreateObjectConfig.unique_names:
-            raise InvalidCreateObjectError(
-                f"A CreateObjectFeature with the name '{name}' was already initialized. "
-                f"Make sure the names are unique and are not accidentally registered more than once.\n"
-                f"Also make sure that names aren't differentiated through just casing or spaces."
-            )
-        CreateObjectConfig.unique_names.add(name)
-
-    @staticmethod
-    def _name(create: CreateObjectConfig) -> str:
-        return f"____{XsUtil.constant(create.name)}"
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, List
+
+from AoE2ScenarioParser.datasets.other import OtherInfo
+from AoE2ScenarioParser.datasets.players import PlayerId
+from AoE2ScenarioParser.scenarios.aoe2_de_scenario import AoE2DEScenario
+
+from AoE2ScenarioRms.enums import XsKey
+from AoE2ScenarioRms.errors import InvalidCreateObjectError
+from AoE2ScenarioRms.rms.create_object.create_object_config import CreateObjectConfig
+from AoE2ScenarioRms.rms.rms_feature import RmsFeature
+from AoE2ScenarioRms.util import XsUtil, XsContainer, Locator
+
+if TYPE_CHECKING:
+    from AoE2ScenarioRms.util import GridMap
+
+
+class CreateObjectFeature(RmsFeature):
+    unique_names = set()
+
+    def __init__(self, scenario: AoE2DEScenario) -> None:
+        """
+        Class that manages the functionality behind implementing the create_object clause
+
+        Args:
+            scenario: The scenario to apply the configs to
+        """
+        container = XsContainer()
+
+        super().__init__(scenario, container)
+
+    def init(self, config: CreateObjectConfig) -> None:
+        """
+        Initialize the 'create object' configurations. Setting XS initializers like variable and array definitions
+
+        Args:
+            config: The configs to be added
+        """
+        name = self._name(config)
+
+        self._validate_name_unique(name)
+
+        self.xs_container.append(
+            XsKey.RESOURCE_VARIABLE_DECLARATION,
+            f"int {name} = {config.index};"
+        )
+
+        self.xs_container.append(
+            XsKey.RESOURCE_GROUP_NAMES_DECLARATION,
+            f"xsArraySetString(__RESOURCE_GROUP_NAMES, {name}, \"{config.name}\");"
+        )
+
+        self.xs_container.append(
+            XsKey.RESOURCE_COUNT_DECLARATION,
+            f"xsArraySetInt(__RESOURCE_SPAWN_COUNTS, {name}, {config.max_potential_group_count});"
+        )
+
+        self.xs_container.append(
+            XsKey.RESOURCE_MAX_SPAWN_DECLARATION,
+            f"xsArraySetFloat(__RESOURCE_MAX_SPAWN_COUNTS, {name}, {config.number_of_groups});"
+        )
+
+        bool_ = XsUtil.bool(config.scale_to_player_number)
+        self.xs_container.append(
+            XsKey.RESOURCE_MAX_SPAWN_IS_PER_PLAYER_DECLARATION,
+            f"xsArraySetBool(__RESOURCE_MAX_SPAWN_COUNTS_IS_PER_PLAYER, {name}, {bool_});"
+        )
+
+        self.xs_container.append(
+            XsKey.RESOURCE_LOCATION_INJECTION,
+            f"rArray = xsArrayGetInt(__ARRAY_RESOURCE_LOCATIONS, {name});"
+        )
+
+        self.xs_container.extend(
+            XsKey.CONFIG_DECLARATION,
+            [
+                f"cArray = xsArrayGetInt(__ARRAY_RESOURCE_CONFIGS, {name});",
+                f"xsArraySetInt(cArray, 0, {config.temp_min_distance_group_placement});",
+                f"xsArraySetInt(cArray, 1, {config.min_distance_group_placement});",
+            ]
+        )
+
+    def build(self, config: CreateObjectConfig, grid_map: 'GridMap') -> None:
+        """
+        Write the functional logic (triggers) for placing the objects. Also write the functional and conditional logic
+        for XS for the given configs.
+
+        Args:
+            config: The config to implement
+            grid_map: The GridMap to take into account when generating potential locations for groups
+        """
+        tm, um = self.scenario.trigger_manager, self.scenario.unit_manager
+        name = self._name(config)
+
+        groups = Locator.create_groups(config, grid_map)
+
+        for index, group in enumerate(groups):
+            spawn_group = tm.add_trigger(f"Spawn {config.name} {index}/{len(groups)}")
+            group_const = config.get_random_const()
+
+            function = f"bool __should_spawn_{config.name}_{index}() {{" \
+                f"return (xsArrayGetBool(xsArrayGetInt(__ARRAY_RESOURCE_PLACED_INDICES, {name}), {index}));" \
+                f"}}"
+            spawn_group.new_condition.script_call(xs_function=function.strip().replace('  ', ''))
+
+            for iindex, tile in enumerate(group):
+                spawn_group.new_effect.create_object(group_const, PlayerId.GAIA, tile.x, tile.y)
+
+                if config.debug_place_all:
+                    um.add_unit(PlayerId.GAIA, group_const, tile.x + .5, tile.y + .5)
+                    player = PlayerId.GAIA if iindex == 0 else PlayerId.ONE
+                    const = OtherInfo.FLAG_M.ID if iindex == 0 else OtherInfo.FLAG_C.ID
+                    um.add_unit(player, const, tile.x + .5, tile.y + .5)
+
+            self.xs_container.append(
+                XsKey.RESOURCE_LOCATION_INJECTION,
+                f"xsArraySetVector(rArray, {index}, vector({group[0].x}, {group[0].y}, -1));\t// {index}"
+            )
+        self.xs_container.append(
+            XsKey.RESOURCE_LOCATION_INJECTION,
+            f"ShuffleVectorArray(rArray, xsArrayGetInt(__ARRAY_RESOURCE_INDICES, {name}));"
+        )
+
+    def solve(self, configs: List[CreateObjectConfig], grid_map: 'GridMap') -> XsContainer:
+        """
+        Execute the init and build steps in one go for each config given.
+
+        Args:
+            configs: The configs to implement
+            grid_map: The GridMap to take into account when generating potential locations for groups of configs
+
+        Returns:
+            The XsContainer with all generated XS
+        """
+        for config_entry in configs:
+            self.init(config_entry)
+            self.build(config_entry, grid_map)
+        return self.xs_container
+
+    @staticmethod
+    def _validate_name_unique(name: str) -> None:
+        """
+        Validate if the given name is unique compared to other names used
+
+        Args:
+            name: The name to validate
+
+        Raises:
+            InvalidCreateObjectError: If the given name has already been registered before in the scenario
+        """
+        if name in CreateObjectConfig.unique_names:
+            raise InvalidCreateObjectError(
+                f"A CreateObjectFeature with the name '{name}' was already initialized. "
+                f"Make sure the names are unique and are not accidentally registered more than once.\n"
+                f"Also make sure that names aren't differentiated through just casing or spaces."
+            )
+        CreateObjectConfig.unique_names.add(name)
+
+    @staticmethod
+    def _name(create: CreateObjectConfig) -> str:
+        return f"____{XsUtil.constant(create.name)}"
```

### Comparing `AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/rms/rms_feature.py` & `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/rms_feature.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/util/data.py` & `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/data.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-from typing import List
-
-from AoE2ScenarioParser.datasets.other import OtherInfo
-from AoE2ScenarioParser.datasets.terrains import TerrainId
-from AoE2ScenarioParser.datasets.units import UnitInfo
-
-from AoE2ScenarioRms.flags.object_clear import ObjectClear
-from AoE2ScenarioRms.flags.terrain_mark import TerrainMark
-
-
-class Data:
-    """
-    Static class that holds functions that return specific data, mainly IDs used for removal of objects or marking of a
-    scenario.
-    """
-    @staticmethod
-    def trees() -> List[int]:
-        """
-        Returns:
-            A list of all tree object IDs
-        """
-        return [o.ID for o in OtherInfo.trees()]
-
-    @staticmethod
-    def cliffs() -> List[int]:
-        """
-        Returns:
-            A list of all cliff IDs
-        """
-        return [
-            264, 265, 266, 267, 268, 269, 270, 271, 272,
-            1339, 1340, 1341, 1342, 1344, 1346
-        ]
-
-    @staticmethod
-    def get_terrain_ids_by_terrain_marks(marks: TerrainMark) -> List[TerrainId]:
-        """
-        Args:
-            marks: The marks to take into account
-
-        Returns:
-            A list of Terrain Ids based on the marks given
-        """
-        ids: List[TerrainId] = []
-
-        if TerrainMark.WATER in marks:
-            ids.extend(TerrainId.water_terrains())
-        if TerrainMark.BEACH in marks:
-            ids.extend(TerrainId.beach_terrains())
-        if TerrainMark.LAND in marks:
-            water_beach = TerrainId.water_terrains() + TerrainId.beach_terrains()
-            ids.extend(terrain for terrain in TerrainId if terrain not in water_beach)
-
-        return ids
-
-    @staticmethod
-    def get_object_consts_by_clear_options(clear: ObjectClear) -> List[int]:
-        """
-        Args:
-            clear: The ``ObjectClear`` configuration used for removing objects from a scenario
-
-        Returns:
-            A list of IDs of object consts used for the removal of objects
-        """
-        consts: List[int] = []
-
-        if ObjectClear.BOARS in clear:
-            consts.extend([
-                UnitInfo.JAVELINA.ID,
-                UnitInfo.WILD_BOAR.ID,
-                UnitInfo.ELEPHANT.ID,
-                UnitInfo.RHINOCEROS.ID
-            ])
-
-        if ObjectClear.SHEEP in clear:
-            consts.extend([
-                UnitInfo.SHEEP.ID,
-                UnitInfo.GOAT.ID,
-                UnitInfo.TURKEY.ID,
-                UnitInfo.GOOSE.ID,
-                UnitInfo.PIG.ID,
-                UnitInfo.COW_A.ID,
-                UnitInfo.COW_B.ID,
-                UnitInfo.COW_C.ID,
-                UnitInfo.COW_D.ID,
-                UnitInfo.LLAMA.ID
-            ])
-
-        if ObjectClear.DEER in clear:
-            consts.extend([
-                UnitInfo.DEER.ID,
-                UnitInfo.IBEX.ID,
-                UnitInfo.ZEBRA.ID
-            ])
-
-        if ObjectClear.WOLFS in clear:
-            consts.extend([
-                UnitInfo.WOLF.ID,
-                UnitInfo.JAGUAR.ID,
-                UnitInfo.LION.ID,
-                UnitInfo.SNOW_LEOPARD.ID,
-                UnitInfo.CROCODILE.ID,
-            ])
-
-        if ObjectClear.RELICS in clear:
-            consts.append(OtherInfo.RELIC.ID)
-
-        if ObjectClear.GOLDS in clear:
-            consts.append(OtherInfo.GOLD_MINE.ID)
-
-        if ObjectClear.STONES in clear:
-            consts.append(OtherInfo.STONE_MINE.ID)
-
-        if ObjectClear.BUSHES in clear:
-            consts.extend([
-                OtherInfo.FORAGE_BUSH.ID,
-                OtherInfo.FRUIT_BUSH.ID
-            ])
-
-        if ObjectClear.CLIFFS in clear:
-            consts.extend(Data.cliffs())
-
-        if ObjectClear.DEEP_FISH in clear:
-            consts.extend([
-                OtherInfo.FISH_TUNA.ID,
-                OtherInfo.FISH_PERCH.ID,
-                OtherInfo.FISH_DORADO.ID,
-                OtherInfo.FISH_SALMON.ID,
-                OtherInfo.FISH_SNAPPER.ID,
-                OtherInfo.GREAT_FISH_MARLIN.ID,
-                OtherInfo.DOLPHIN.ID,
-            ])
-
-        if ObjectClear.SHORE_FISH in clear:
-            consts.extend([
-                OtherInfo.SHORE_FISH.ID,
-                OtherInfo.BOX_TURTLES.ID,
-            ])
-
-        return consts
+from typing import List
+
+from AoE2ScenarioParser.datasets.other import OtherInfo
+from AoE2ScenarioParser.datasets.terrains import TerrainId
+from AoE2ScenarioParser.datasets.units import UnitInfo
+
+from AoE2ScenarioRms.flags.object_clear import ObjectClear
+from AoE2ScenarioRms.flags.terrain_mark import TerrainMark
+
+
+class Data:
+    """
+    Static class that holds functions that return specific data, mainly IDs used for removal of objects or marking of a
+    scenario.
+    """
+    @staticmethod
+    def trees() -> List[int]:
+        """
+        Returns:
+            A list of all tree object IDs
+        """
+        return [o.ID for o in OtherInfo.trees()]
+
+    @staticmethod
+    def cliffs() -> List[int]:
+        """
+        Returns:
+            A list of all cliff IDs
+        """
+        return [
+            264, 265, 266, 267, 268, 269, 270, 271, 272,
+            1339, 1340, 1341, 1342, 1344, 1346
+        ]
+
+    @staticmethod
+    def get_terrain_ids_by_terrain_marks(marks: TerrainMark) -> List[TerrainId]:
+        """
+        Args:
+            marks: The marks to take into account
+
+        Returns:
+            A list of Terrain Ids based on the marks given
+        """
+        ids: List[TerrainId] = []
+
+        if TerrainMark.WATER in marks:
+            ids.extend(TerrainId.water_terrains())
+        if TerrainMark.BEACH in marks:
+            ids.extend(TerrainId.beach_terrains())
+        if TerrainMark.LAND in marks:
+            water_beach = TerrainId.water_terrains() + TerrainId.beach_terrains()
+            ids.extend(terrain for terrain in TerrainId if terrain not in water_beach)
+
+        return ids
+
+    @staticmethod
+    def get_object_consts_by_clear_options(clear: ObjectClear) -> List[int]:
+        """
+        Args:
+            clear: The ``ObjectClear`` configuration used for removing objects from a scenario
+
+        Returns:
+            A list of IDs of object consts used for the removal of objects
+        """
+        consts: List[int] = []
+
+        if ObjectClear.BOARS in clear:
+            consts.extend([
+                UnitInfo.JAVELINA.ID,
+                UnitInfo.WILD_BOAR.ID,
+                UnitInfo.ELEPHANT.ID,
+                UnitInfo.RHINOCEROS.ID
+            ])
+
+        if ObjectClear.SHEEP in clear:
+            consts.extend([
+                UnitInfo.SHEEP.ID,
+                UnitInfo.GOAT.ID,
+                UnitInfo.TURKEY.ID,
+                UnitInfo.GOOSE.ID,
+                UnitInfo.PIG.ID,
+                UnitInfo.COW_A.ID,
+                UnitInfo.COW_B.ID,
+                UnitInfo.COW_C.ID,
+                UnitInfo.COW_D.ID,
+                UnitInfo.LLAMA.ID
+            ])
+
+        if ObjectClear.DEER in clear:
+            consts.extend([
+                UnitInfo.DEER.ID,
+                UnitInfo.IBEX.ID,
+                UnitInfo.ZEBRA.ID
+            ])
+
+        if ObjectClear.WOLFS in clear:
+            consts.extend([
+                UnitInfo.WOLF.ID,
+                UnitInfo.JAGUAR.ID,
+                UnitInfo.LION.ID,
+                UnitInfo.SNOW_LEOPARD.ID,
+                UnitInfo.CROCODILE.ID,
+            ])
+
+        if ObjectClear.RELICS in clear:
+            consts.append(OtherInfo.RELIC.ID)
+
+        if ObjectClear.GOLDS in clear:
+            consts.append(OtherInfo.GOLD_MINE.ID)
+
+        if ObjectClear.STONES in clear:
+            consts.append(OtherInfo.STONE_MINE.ID)
+
+        if ObjectClear.BUSHES in clear:
+            consts.extend([
+                OtherInfo.FORAGE_BUSH.ID,
+                OtherInfo.FRUIT_BUSH.ID
+            ])
+
+        if ObjectClear.CLIFFS in clear:
+            consts.extend(Data.cliffs())
+
+        if ObjectClear.DEEP_FISH in clear:
+            consts.extend([
+                OtherInfo.FISH_TUNA.ID,
+                OtherInfo.FISH_PERCH.ID,
+                OtherInfo.FISH_DORADO.ID,
+                OtherInfo.FISH_SALMON.ID,
+                OtherInfo.FISH_SNAPPER.ID,
+                OtherInfo.GREAT_FISH_MARLIN.ID,
+                OtherInfo.DOLPHIN.ID,
+            ])
+
+        if ObjectClear.SHORE_FISH in clear:
+            consts.extend([
+                OtherInfo.SHORE_FISH.ID,
+                OtherInfo.BOX_TURTLES.ID,
+            ])
+
+        return consts
```

### Comparing `AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/util/grid_map.py` & `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/grid_map.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/util/locator.py` & `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/locator.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/util/scenario_util.py` & `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/scenario_util.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-import math
-from typing import List
-
-from AoE2ScenarioParser.datasets.players import PlayerId
-from AoE2ScenarioParser.datasets.terrains import TerrainId
-from AoE2ScenarioParser.helper.helper import xy_to_i
-from AoE2ScenarioParser.objects.data_objects.unit import Unit
-from AoE2ScenarioParser.scenarios.aoe2_de_scenario import AoE2DEScenario
-
-from AoE2ScenarioRms.flags import ObjectClear
-from AoE2ScenarioRms.util.data import Data
-
-
-class ScenarioUtil:
-    @staticmethod
-    def clear(
-            scenario: AoE2DEScenario,
-            clear: ObjectClear = None,
-            consts: List[int] = None,
-            units: List[Unit] = None
-    ) -> None:
-        """
-        Clear objects from a scenario to make place for randomized objects
-
-        Args:
-            scenario: The scenario to clear objects from
-            clear: The flag indicating what to clear and what to leave
-            consts: A list of object consts to clear on top of the clear flag
-            units: A list of unit objects to clear on top of the flag and consts
-        """
-        um, mm = scenario.unit_manager, scenario.map_manager
-
-        if clear is None:
-            clear = ObjectClear.RESOURCE_OBJECTS + ObjectClear.ANIMAL_OBJECTS
-
-        consts = consts if consts is not None else []
-        units = units if units is not None else []
-
-        # Clear all player related objects
-        if ObjectClear.PLAYERS in clear:
-            for i in PlayerId.all(exclude_gaia=True):
-                um.units[i] = []
-
-        # Mark resources
-        resource_consts = Data.get_object_consts_by_clear_options(clear)
-        objects_to_remove = set(obj for obj in um.units[PlayerId.GAIA] if obj.unit_const in resource_consts)
-
-        # Mark straggler trees
-        if ObjectClear.STRAGGLERS in clear:
-            tree_consts = Data.trees()
-            for u in um.units[PlayerId.GAIA]:
-                underlying_terrain = mm.terrain[xy_to_i(math.floor(u.x), math.floor(u.y), mm.map_size)].terrain_id
-                if u.unit_const in tree_consts and underlying_terrain not in TerrainId.tree_terrains():
-                    objects_to_remove.add(u)
-
-        # Mark given consts
-        if len(consts):
-            objects_to_remove.update(set(um.filter_units_by_const(consts)))
-
-        # Clear all marked objects
-        for unit in objects_to_remove:
-            um.remove_unit(unit=unit)
-
-        # Clear all given objects
-        for unit in units:
-            um.remove_unit(unit=unit)
+import math
+from typing import List
+
+from AoE2ScenarioParser.datasets.players import PlayerId
+from AoE2ScenarioParser.datasets.terrains import TerrainId
+from AoE2ScenarioParser.helper.helper import xy_to_i
+from AoE2ScenarioParser.objects.data_objects.unit import Unit
+from AoE2ScenarioParser.scenarios.aoe2_de_scenario import AoE2DEScenario
+
+from AoE2ScenarioRms.flags import ObjectClear
+from AoE2ScenarioRms.util.data import Data
+
+
+class ScenarioUtil:
+    @staticmethod
+    def clear(
+            scenario: AoE2DEScenario,
+            clear: ObjectClear = None,
+            consts: List[int] = None,
+            units: List[Unit] = None
+    ) -> None:
+        """
+        Clear objects from a scenario to make place for randomized objects
+
+        Args:
+            scenario: The scenario to clear objects from
+            clear: The flag indicating what to clear and what to leave
+            consts: A list of object consts to clear on top of the clear flag
+            units: A list of unit objects to clear on top of the flag and consts
+        """
+        um, mm = scenario.unit_manager, scenario.map_manager
+
+        if clear is None:
+            clear = ObjectClear.RESOURCE_OBJECTS + ObjectClear.ANIMAL_OBJECTS
+
+        consts = consts if consts is not None else []
+        units = units if units is not None else []
+
+        # Clear all player related objects
+        if ObjectClear.PLAYERS in clear:
+            for i in PlayerId.all(exclude_gaia=True):
+                um.units[i] = []
+
+        # Mark resources
+        resource_consts = Data.get_object_consts_by_clear_options(clear)
+        objects_to_remove = set(obj for obj in um.units[PlayerId.GAIA] if obj.unit_const in resource_consts)
+
+        # Mark straggler trees
+        if ObjectClear.STRAGGLERS in clear:
+            tree_consts = Data.trees()
+            for u in um.units[PlayerId.GAIA]:
+                underlying_terrain = mm.terrain[xy_to_i(math.floor(u.x), math.floor(u.y), mm.map_size)].terrain_id
+                if u.unit_const in tree_consts and underlying_terrain not in TerrainId.tree_terrains():
+                    objects_to_remove.add(u)
+
+        # Mark given consts
+        if len(consts):
+            objects_to_remove.update(set(um.filter_units_by_const(consts)))
+
+        # Clear all marked objects
+        for unit in objects_to_remove:
+            um.remove_unit(unit=unit)
+
+        # Clear all given objects
+        for unit in units:
+            um.remove_unit(unit=unit)
```

### Comparing `AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/util/tile_util.py` & `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/tile_util.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/util/xs_container.py` & `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/xs_container.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.0/AoE2ScenarioRms/util/xs_util.py` & `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/xs_util.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-from pathlib import Path
-from typing import Any
-
-
-class XsUtil:
-    """
-
-    Class for managing common Xs shortcuts and functionality.
-
-    """
-    @staticmethod
-    def bool(val: Any) -> str:
-        """
-        Transform a value into an XS boolean
-
-        Args:
-            val: The value to check
-
-        Returns:
-            'true' if val is truthy, 'false' otherwise
-        """
-        return 'true' if val else 'false'
-
-    @staticmethod
-    def file(path: str) -> str:
-        """
-        Read a file from the XS folder within this repo and return its contents
-
-        Args:
-            path: The path of the XS file within the XS folder
-
-        Returns:
-            The content of the file as string
-        """
-        with (Path(__file__).parent.parent / 'xs' / path).open() as file:
-            return file.read()
-
-    @staticmethod
-    def constant(name: str) -> str:
-        """
-        Change a given name to an XS constant name
-
-        Args:
-            name: The name to update
-
-        Returns:
-            The updated string as an XS constant
-        """
-        xs_name = ' '.join(filter(lambda e: e, name.split(' ')))
-        return xs_name.upper().replace(' ', '_')
+from pathlib import Path
+from typing import Any
+
+
+class XsUtil:
+    """
+
+    Class for managing common Xs shortcuts and functionality.
+
+    """
+    @staticmethod
+    def bool(val: Any) -> str:
+        """
+        Transform a value into an XS boolean
+
+        Args:
+            val: The value to check
+
+        Returns:
+            'true' if val is truthy, 'false' otherwise
+        """
+        return 'true' if val else 'false'
+
+    @staticmethod
+    def file(path: str) -> str:
+        """
+        Read a file from the XS folder within this repo and return its contents
+
+        Args:
+            path: The path of the XS file within the XS folder
+
+        Returns:
+            The content of the file as string
+        """
+        with (Path(__file__).parent.parent / 'xs' / path).open() as file:
+            return file.read()
+
+    @staticmethod
+    def constant(name: str) -> str:
+        """
+        Change a given name to an XS constant name
+
+        Args:
+            name: The name to update
+
+        Returns:
+            The updated string as an XS constant
+        """
+        xs_name = ' '.join(filter(lambda e: e, name.split(' ')))
+        return xs_name.upper().replace(' ', '_')
```

### Comparing `AoE2ScenarioRms-0.2.0/AoE2ScenarioRms.egg-info/PKG-INFO` & `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-Metadata-Version: 2.1
-Name: AoE2ScenarioRms
-Version: 0.2.0
-Summary: A library built on top of the AoE2ScenarioParser.
-Author-email: Kerwin Sneijders <ksneijders-dev@hotmail.com>
-Project-URL: Homepage, https://github.com/KSneijders/AoE2ScenarioRms
-Project-URL: Bug Tracker, https://github.com/KSneijders/AoE2ScenarioRms/issues
-Project-URL: Examples, https://github.com/KSneijders/AoE2ScenarioRms/tree/main/examples
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# AoE2ScenarioRms
-
-A library built on top of the [AoE2ScenarioParser].
-Allows you to add `triggers` and `XS` to your AoE2:DE scenarios which will add logic to allow for random resource
-placements each play-through.
-
-> Keep in mind this project is still heavily a **WORK-IN-PROGRESS**
-
-[AoE2ScenarioParser]: https://github.com/KSneijders/AoE2ScenarioParser
-
-## Example
-
-Please check out the example [here](https://github.com/KSneijders/AoE2ScenarioRms/tree/main/examples). 
-(no real docs atm)
-
-This project is still a work-in-progress.
-So everything can still change without notice (most likely will).  
-If you'd like to try anyway, for now just clone this repository to the root of your source folder and import from there.
-
-Make sure `AoE2ScenarioParser` is installed: [link](https://github.com/KSneijders/AoE2ScenarioParser).
-
-## Rough todo:
-
-1. ~~Change tile selection to `random.choice(all_possible_tiles)` instead of looking for completely random tiles
-   Potentially conditionally? Or with parameter? As big surfaces are faster with completely random tiles~~
-2. ~~Move XS logic to own class(es)~~
-3. ~~Move Debug logic to own class~~
-4. ~~Change `asr.write()` as triggers are always added directly, so why isn't the script?~~
-5. ~~Add docs, docstrings and tests~~
-6. ~~Allow XS to log the amount that spawned succesfully, so you can limit the amount of spawns for performance~~
-7. More (?)
-
-## Potential Ideas:
-
-1. Player areas :monkaS:
-2. Scale with map size (hardcoded on parser level as map_size cannot be changed dynamically)
-3. ~~Support larger objects (currently only 1x1 is supported)~~
-4. Automatically figure out what to remove based on CreateObjectConfig configs
-5. Add ability to mock the XS spawning process to estimate the amount of necessary successful spawn attempts
-6. Ability to bind ID to list of create objects and be able to differentiate distance to each group 
-7. (Somehow) remove spawn order bias. Currently, the earlier the spawns the more chance they have to succeed because 
-   the map isn't filled up yet.
-8. More (?)
-
----
-
-**Suggestions are always welcome!**
-
-# Authors
-
-- Kerwin Sneijders (Main Author)
-
-# License
-
-MIT License: Please see the [LICENSE file].
-
-[license file]: https://github.com/KSneijders/AoE2ScenarioRms/blob/main/LICENSE
+Metadata-Version: 2.1
+Name: AoE2ScenarioRms
+Version: 0.2.4
+Summary: A library built on top of the AoE2ScenarioParser.
+Author-email: Kerwin Sneijders <ksneijders-dev@hotmail.com>
+Project-URL: Homepage, https://github.com/KSneijders/AoE2ScenarioRms
+Project-URL: Bug Tracker, https://github.com/KSneijders/AoE2ScenarioRms/issues
+Project-URL: Examples, https://github.com/KSneijders/AoE2ScenarioRms/tree/main/examples
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# AoE2ScenarioRms
+
+A library built on top of the [AoE2ScenarioParser].
+Allows you to add `triggers` and `XS` to your AoE2:DE scenarios which will add logic to allow for random resource
+placements each play-through.
+
+> Keep in mind this project is still heavily a **WORK-IN-PROGRESS**
+
+[AoE2ScenarioParser]: https://github.com/KSneijders/AoE2ScenarioParser
+
+## Example
+
+Please check out the example [here](https://github.com/KSneijders/AoE2ScenarioRms/tree/main/examples). 
+(no real docs atm)
+
+This project is still a work-in-progress.
+So everything can still change without notice (most likely will).  
+If you'd like to try anyway, for now just clone this repository to the root of your source folder and import from there.
+
+Make sure `AoE2ScenarioParser` is installed: [link](https://github.com/KSneijders/AoE2ScenarioParser).
+
+## Rough todo:
+
+1. ~~Change tile selection to `random.choice(all_possible_tiles)` instead of looking for completely random tiles
+   Potentially conditionally? Or with parameter? As big surfaces are faster with completely random tiles~~
+2. ~~Move XS logic to own class(es)~~
+3. ~~Move Debug logic to own class~~
+4. ~~Change `asr.write()` as triggers are always added directly, so why isn't the script?~~
+5. ~~Add docs, docstrings and tests~~
+6. ~~Allow XS to log the amount that spawned succesfully, so you can limit the amount of spawns for performance~~
+7. More (?)
+
+## Potential Ideas:
+
+1. Player areas :monkaS:
+2. Scale with map size (hardcoded on parser level as map_size cannot be changed dynamically)
+3. ~~Support larger objects (currently only 1x1 is supported)~~
+4. Automatically figure out what to remove based on CreateObjectConfig configs
+5. Add ability to mock the XS spawning process to estimate the amount of necessary successful spawn attempts
+6. Ability to bind ID to list of create objects and be able to differentiate distance to each group 
+7. (Somehow) remove spawn order bias. Currently, the earlier the spawns the more chance they have to succeed because 
+   the map isn't filled up yet.
+8. More (?)
+
+---
+
+**Suggestions are always welcome!**
+
+# Authors
+
+- Kerwin Sneijders (Main Author)
+
+# License
+
+MIT License: Please see the [LICENSE file].
+
+[license file]: https://github.com/KSneijders/AoE2ScenarioRms/blob/main/LICENSE
```

### Comparing `AoE2ScenarioRms-0.2.0/AoE2ScenarioRms.egg-info/SOURCES.txt` & `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 AoE2ScenarioRms/__init__.py
-AoE2ScenarioRms/app.py
-AoE2ScenarioRms/local_config.py
+AoE2ScenarioRms/version.py
 AoE2ScenarioRms.egg-info/PKG-INFO
 AoE2ScenarioRms.egg-info/SOURCES.txt
 AoE2ScenarioRms.egg-info/dependency_links.txt
 AoE2ScenarioRms.egg-info/top_level.txt
 AoE2ScenarioRms/core/__init__.py
 AoE2ScenarioRms/core/aoe2_scenario_rms.py
 AoE2ScenarioRms/debug/__init__.py
```

### Comparing `AoE2ScenarioRms-0.2.0/LICENSE` & `AoE2ScenarioRms-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.0/PKG-INFO` & `AoE2ScenarioRms-0.2.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-Metadata-Version: 2.1
-Name: AoE2ScenarioRms
-Version: 0.2.0
-Summary: A library built on top of the AoE2ScenarioParser.
-Author-email: Kerwin Sneijders <ksneijders-dev@hotmail.com>
-Project-URL: Homepage, https://github.com/KSneijders/AoE2ScenarioRms
-Project-URL: Bug Tracker, https://github.com/KSneijders/AoE2ScenarioRms/issues
-Project-URL: Examples, https://github.com/KSneijders/AoE2ScenarioRms/tree/main/examples
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# AoE2ScenarioRms
-
-A library built on top of the [AoE2ScenarioParser].
-Allows you to add `triggers` and `XS` to your AoE2:DE scenarios which will add logic to allow for random resource
-placements each play-through.
-
-> Keep in mind this project is still heavily a **WORK-IN-PROGRESS**
-
-[AoE2ScenarioParser]: https://github.com/KSneijders/AoE2ScenarioParser
-
-## Example
-
-Please check out the example [here](https://github.com/KSneijders/AoE2ScenarioRms/tree/main/examples). 
-(no real docs atm)
-
-This project is still a work-in-progress.
-So everything can still change without notice (most likely will).  
-If you'd like to try anyway, for now just clone this repository to the root of your source folder and import from there.
-
-Make sure `AoE2ScenarioParser` is installed: [link](https://github.com/KSneijders/AoE2ScenarioParser).
-
-## Rough todo:
-
-1. ~~Change tile selection to `random.choice(all_possible_tiles)` instead of looking for completely random tiles
-   Potentially conditionally? Or with parameter? As big surfaces are faster with completely random tiles~~
-2. ~~Move XS logic to own class(es)~~
-3. ~~Move Debug logic to own class~~
-4. ~~Change `asr.write()` as triggers are always added directly, so why isn't the script?~~
-5. ~~Add docs, docstrings and tests~~
-6. ~~Allow XS to log the amount that spawned succesfully, so you can limit the amount of spawns for performance~~
-7. More (?)
-
-## Potential Ideas:
-
-1. Player areas :monkaS:
-2. Scale with map size (hardcoded on parser level as map_size cannot be changed dynamically)
-3. ~~Support larger objects (currently only 1x1 is supported)~~
-4. Automatically figure out what to remove based on CreateObjectConfig configs
-5. Add ability to mock the XS spawning process to estimate the amount of necessary successful spawn attempts
-6. Ability to bind ID to list of create objects and be able to differentiate distance to each group 
-7. (Somehow) remove spawn order bias. Currently, the earlier the spawns the more chance they have to succeed because 
-   the map isn't filled up yet.
-8. More (?)
-
----
-
-**Suggestions are always welcome!**
-
-# Authors
-
-- Kerwin Sneijders (Main Author)
-
-# License
-
-MIT License: Please see the [LICENSE file].
-
-[license file]: https://github.com/KSneijders/AoE2ScenarioRms/blob/main/LICENSE
+Metadata-Version: 2.1
+Name: AoE2ScenarioRms
+Version: 0.2.4
+Summary: A library built on top of the AoE2ScenarioParser.
+Author-email: Kerwin Sneijders <ksneijders-dev@hotmail.com>
+Project-URL: Homepage, https://github.com/KSneijders/AoE2ScenarioRms
+Project-URL: Bug Tracker, https://github.com/KSneijders/AoE2ScenarioRms/issues
+Project-URL: Examples, https://github.com/KSneijders/AoE2ScenarioRms/tree/main/examples
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# AoE2ScenarioRms
+
+A library built on top of the [AoE2ScenarioParser].
+Allows you to add `triggers` and `XS` to your AoE2:DE scenarios which will add logic to allow for random resource
+placements each play-through.
+
+> Keep in mind this project is still heavily a **WORK-IN-PROGRESS**
+
+[AoE2ScenarioParser]: https://github.com/KSneijders/AoE2ScenarioParser
+
+## Example
+
+Please check out the example [here](https://github.com/KSneijders/AoE2ScenarioRms/tree/main/examples). 
+(no real docs atm)
+
+This project is still a work-in-progress.
+So everything can still change without notice (most likely will).  
+If you'd like to try anyway, for now just clone this repository to the root of your source folder and import from there.
+
+Make sure `AoE2ScenarioParser` is installed: [link](https://github.com/KSneijders/AoE2ScenarioParser).
+
+## Rough todo:
+
+1. ~~Change tile selection to `random.choice(all_possible_tiles)` instead of looking for completely random tiles
+   Potentially conditionally? Or with parameter? As big surfaces are faster with completely random tiles~~
+2. ~~Move XS logic to own class(es)~~
+3. ~~Move Debug logic to own class~~
+4. ~~Change `asr.write()` as triggers are always added directly, so why isn't the script?~~
+5. ~~Add docs, docstrings and tests~~
+6. ~~Allow XS to log the amount that spawned succesfully, so you can limit the amount of spawns for performance~~
+7. More (?)
+
+## Potential Ideas:
+
+1. Player areas :monkaS:
+2. Scale with map size (hardcoded on parser level as map_size cannot be changed dynamically)
+3. ~~Support larger objects (currently only 1x1 is supported)~~
+4. Automatically figure out what to remove based on CreateObjectConfig configs
+5. Add ability to mock the XS spawning process to estimate the amount of necessary successful spawn attempts
+6. Ability to bind ID to list of create objects and be able to differentiate distance to each group 
+7. (Somehow) remove spawn order bias. Currently, the earlier the spawns the more chance they have to succeed because 
+   the map isn't filled up yet.
+8. More (?)
+
+---
+
+**Suggestions are always welcome!**
+
+# Authors
+
+- Kerwin Sneijders (Main Author)
+
+# License
+
+MIT License: Please see the [LICENSE file].
+
+[license file]: https://github.com/KSneijders/AoE2ScenarioRms/blob/main/LICENSE
```

### Comparing `AoE2ScenarioRms-0.2.0/README.md` & `AoE2ScenarioRms-0.2.4/README.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-# AoE2ScenarioRms
-
-A library built on top of the [AoE2ScenarioParser].
-Allows you to add `triggers` and `XS` to your AoE2:DE scenarios which will add logic to allow for random resource
-placements each play-through.
-
-> Keep in mind this project is still heavily a **WORK-IN-PROGRESS**
-
-[AoE2ScenarioParser]: https://github.com/KSneijders/AoE2ScenarioParser
-
-## Example
-
-Please check out the example [here](https://github.com/KSneijders/AoE2ScenarioRms/tree/main/examples). 
-(no real docs atm)
-
-This project is still a work-in-progress.
-So everything can still change without notice (most likely will).  
-If you'd like to try anyway, for now just clone this repository to the root of your source folder and import from there.
-
-Make sure `AoE2ScenarioParser` is installed: [link](https://github.com/KSneijders/AoE2ScenarioParser).
-
-## Rough todo:
-
-1. ~~Change tile selection to `random.choice(all_possible_tiles)` instead of looking for completely random tiles
-   Potentially conditionally? Or with parameter? As big surfaces are faster with completely random tiles~~
-2. ~~Move XS logic to own class(es)~~
-3. ~~Move Debug logic to own class~~
-4. ~~Change `asr.write()` as triggers are always added directly, so why isn't the script?~~
-5. ~~Add docs, docstrings and tests~~
-6. ~~Allow XS to log the amount that spawned succesfully, so you can limit the amount of spawns for performance~~
-7. More (?)
-
-## Potential Ideas:
-
-1. Player areas :monkaS:
-2. Scale with map size (hardcoded on parser level as map_size cannot be changed dynamically)
-3. ~~Support larger objects (currently only 1x1 is supported)~~
-4. Automatically figure out what to remove based on CreateObjectConfig configs
-5. Add ability to mock the XS spawning process to estimate the amount of necessary successful spawn attempts
-6. Ability to bind ID to list of create objects and be able to differentiate distance to each group 
-7. (Somehow) remove spawn order bias. Currently, the earlier the spawns the more chance they have to succeed because 
-   the map isn't filled up yet.
-8. More (?)
-
----
-
-**Suggestions are always welcome!**
-
-# Authors
-
-- Kerwin Sneijders (Main Author)
-
-# License
-
-MIT License: Please see the [LICENSE file].
-
-[license file]: https://github.com/KSneijders/AoE2ScenarioRms/blob/main/LICENSE
+# AoE2ScenarioRms
+
+A library built on top of the [AoE2ScenarioParser].
+Allows you to add `triggers` and `XS` to your AoE2:DE scenarios which will add logic to allow for random resource
+placements each play-through.
+
+> Keep in mind this project is still heavily a **WORK-IN-PROGRESS**
+
+[AoE2ScenarioParser]: https://github.com/KSneijders/AoE2ScenarioParser
+
+## Example
+
+Please check out the example [here](https://github.com/KSneijders/AoE2ScenarioRms/tree/main/examples). 
+(no real docs atm)
+
+This project is still a work-in-progress.
+So everything can still change without notice (most likely will).  
+If you'd like to try anyway, for now just clone this repository to the root of your source folder and import from there.
+
+Make sure `AoE2ScenarioParser` is installed: [link](https://github.com/KSneijders/AoE2ScenarioParser).
+
+## Rough todo:
+
+1. ~~Change tile selection to `random.choice(all_possible_tiles)` instead of looking for completely random tiles
+   Potentially conditionally? Or with parameter? As big surfaces are faster with completely random tiles~~
+2. ~~Move XS logic to own class(es)~~
+3. ~~Move Debug logic to own class~~
+4. ~~Change `asr.write()` as triggers are always added directly, so why isn't the script?~~
+5. ~~Add docs, docstrings and tests~~
+6. ~~Allow XS to log the amount that spawned succesfully, so you can limit the amount of spawns for performance~~
+7. More (?)
+
+## Potential Ideas:
+
+1. Player areas :monkaS:
+2. Scale with map size (hardcoded on parser level as map_size cannot be changed dynamically)
+3. ~~Support larger objects (currently only 1x1 is supported)~~
+4. Automatically figure out what to remove based on CreateObjectConfig configs
+5. Add ability to mock the XS spawning process to estimate the amount of necessary successful spawn attempts
+6. Ability to bind ID to list of create objects and be able to differentiate distance to each group 
+7. (Somehow) remove spawn order bias. Currently, the earlier the spawns the more chance they have to succeed because 
+   the map isn't filled up yet.
+8. More (?)
+
+---
+
+**Suggestions are always welcome!**
+
+# Authors
+
+- Kerwin Sneijders (Main Author)
+
+# License
+
+MIT License: Please see the [LICENSE file].
+
+[license file]: https://github.com/KSneijders/AoE2ScenarioRms/blob/main/LICENSE
```

### Comparing `AoE2ScenarioRms-0.2.0/pyproject.toml` & `AoE2ScenarioRms-0.2.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AoE2ScenarioRms"
-version = "0.2.0"
+version = "0.2.4"  # << Also change `AoE2ScenarioRms/version.py`
 authors = [
     { name = "Kerwin Sneijders", email = "ksneijders-dev@hotmail.com" },
 ]
 description = """A library built on top of the AoE2ScenarioParser.
     Allows you to add triggers and XS to your AoE2:DE scenarios
     which will add logic to allow for random resource placements each play-through
 """
```

