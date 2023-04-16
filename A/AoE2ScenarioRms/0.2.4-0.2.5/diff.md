# Comparing `tmp/AoE2ScenarioRms-0.2.4.tar.gz` & `tmp/AoE2ScenarioRms-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AoE2ScenarioRms-0.2.4.tar", last modified: Sun Apr 16 14:03:52 2023, max compression
+gzip compressed data, was "AoE2ScenarioRms-0.2.5.tar", last modified: Sun Apr 16 14:10:29 2023, max compression
```

## Comparing `AoE2ScenarioRms-0.2.4.tar` & `AoE2ScenarioRms-0.2.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.186286 AoE2ScenarioRms-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.182286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.182286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/core/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/core/aoe2_scenario_rms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.182286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/debug/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/debug/apply_all_visible.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/debug/apply_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/debug/apply_no_clutter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/debug/apply_state_as_black.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/debug/apply_xs_print.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.182286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/enums/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/enums/grouping_method.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.182286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/enums/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/enums/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/enums/internal/xs_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/enums/tile_level.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.182286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/errors/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/errors/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.182286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/flags/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/flags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/flags/object_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/flags/object_marks.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/flags/terrain_mark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.186286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.186286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/create_object/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/create_object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/create_object/create_object_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/create_object/create_object_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/rms_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/rms_feature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.186286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/grid_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/grid_map_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/locator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/scenario_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/tile_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/unit_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/xs_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/xs_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:03:52.182286 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-16 14:03:52.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-16 14:03:52.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 14:03:52.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-16 14:03:52.000000 AoE2ScenarioRms-0.2.4/AoE2ScenarioRms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-16 14:03:52.186286 AoE2ScenarioRms-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-16 14:03:43.000000 AoE2ScenarioRms-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 14:03:52.186286 AoE2ScenarioRms-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:10:29.104815 AoE2ScenarioRms-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:10:29.092815 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:10:29.092815 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/core/aoe2_scenario_rms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:10:29.096815 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/debug/apply_all_visible.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/debug/apply_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/debug/apply_no_clutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/debug/apply_state_as_black.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/debug/apply_xs_print.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:10:29.096815 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/enums/grouping_method.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:10:29.096815 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/enums/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/enums/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/enums/internal/xs_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/enums/tile_level.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:10:29.100815 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/errors/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/errors/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:10:29.100815 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/flags/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/flags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/flags/object_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/flags/object_marks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/flags/terrain_mark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:10:29.100815 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/rms/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/rms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:10:29.100815 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/rms/create_object/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/rms/create_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/rms/create_object/create_object_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/rms/create_object/create_object_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/rms/rms_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/rms/rms_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:10:29.104815 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/util/grid_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/util/grid_map_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8817 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/util/locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/util/scenario_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/util/tile_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/util/unit_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/util/xs_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/util/xs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 14:10:29.092815 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-16 14:10:29.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-16 14:10:29.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 14:10:29.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-16 14:10:29.000000 AoE2ScenarioRms-0.2.5/AoE2ScenarioRms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-16 14:10:29.104815 AoE2ScenarioRms-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-16 14:10:17.000000 AoE2ScenarioRms-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 14:10:29.104815 AoE2ScenarioRms-0.2.5/setup.cfg
```

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/core/aoe2_scenario_rms.py` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/core/aoe2_scenario_rms.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/debug/apply_all_visible.py` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/debug/apply_all_visible.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/debug/apply_state_as_black.py` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/debug/apply_state_as_black.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/debug/apply_xs_print.py` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/debug/apply_xs_print.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/enums/internal/xs_key.py` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/enums/internal/xs_key.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/flags/object_clear.py` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/flags/object_clear.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/flags/terrain_mark.py` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/flags/terrain_mark.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/create_object/create_object_config.py` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/rms/create_object/create_object_config.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/create_object/create_object_feature.py` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/rms/create_object/create_object_feature.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/rms/rms_feature.py` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/rms/rms_feature.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/data.py` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/util/data.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/grid_map.py` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/util/grid_map.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/grid_map_factory.py` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/util/grid_map_factory.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/locator.py` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/util/locator.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/scenario_util.py` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/util/scenario_util.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/tile_util.py` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/util/tile_util.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/unit_util.py` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/util/unit_util.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/xs_container.py` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/util/xs_container.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms/util/xs_util.py` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms/util/xs_util.py`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms.egg-info/PKG-INFO` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AoE2ScenarioRms
-Version: 0.2.4
+Version: 0.2.5
 Summary: A library built on top of the AoE2ScenarioParser.
 Author-email: Kerwin Sneijders <ksneijders-dev@hotmail.com>
 Project-URL: Homepage, https://github.com/KSneijders/AoE2ScenarioRms
 Project-URL: Bug Tracker, https://github.com/KSneijders/AoE2ScenarioRms/issues
 Project-URL: Examples, https://github.com/KSneijders/AoE2ScenarioRms/tree/main/examples
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `AoE2ScenarioRms-0.2.4/AoE2ScenarioRms.egg-info/SOURCES.txt` & `AoE2ScenarioRms-0.2.5/AoE2ScenarioRms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/LICENSE` & `AoE2ScenarioRms-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/PKG-INFO` & `AoE2ScenarioRms-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AoE2ScenarioRms
-Version: 0.2.4
+Version: 0.2.5
 Summary: A library built on top of the AoE2ScenarioParser.
 Author-email: Kerwin Sneijders <ksneijders-dev@hotmail.com>
 Project-URL: Homepage, https://github.com/KSneijders/AoE2ScenarioRms
 Project-URL: Bug Tracker, https://github.com/KSneijders/AoE2ScenarioRms/issues
 Project-URL: Examples, https://github.com/KSneijders/AoE2ScenarioRms/tree/main/examples
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `AoE2ScenarioRms-0.2.4/README.md` & `AoE2ScenarioRms-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `AoE2ScenarioRms-0.2.4/pyproject.toml` & `AoE2ScenarioRms-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "AoE2ScenarioRms"
-version = "0.2.4"  # << Also change `AoE2ScenarioRms/version.py`
+version = "0.2.5"  # << Also change `AoE2ScenarioRms/version.py`
 authors = [
     { name = "Kerwin Sneijders", email = "ksneijders-dev@hotmail.com" },
 ]
 description = """A library built on top of the AoE2ScenarioParser.
     Allows you to add triggers and XS to your AoE2:DE scenarios
     which will add logic to allow for random resource placements each play-through
 """
```

