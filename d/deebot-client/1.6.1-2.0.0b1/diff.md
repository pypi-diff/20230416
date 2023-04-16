# Comparing `tmp/deebot-client-1.6.1.tar.gz` & `tmp/deebot-client-2.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deebot-client-1.6.1.tar", last modified: Thu Mar  2 17:21:33 2023, max compression
+gzip compressed data, was "deebot-client-2.0.0b1.tar", last modified: Sun Apr 16 10:11:05 2023, max compression
```

## Comparing `deebot-client-1.6.1.tar` & `deebot-client-2.0.0b1.tar`

### file list

```diff
@@ -1,92 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:21:33.704070 deebot-client-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-03-02 17:21:29.000000 deebot-client-1.6.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-03-02 17:21:33.704070 deebot-client-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-03-02 17:21:29.000000 deebot-client-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:21:33.700070 deebot-client-1.6.1/deebot_client/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:21:33.704070 deebot-client-1.6.1/deebot_client/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/advanced_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/carpet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/charge_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/clean_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/clean_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/clean_preference.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/continuous_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/life_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     9114 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/multimap_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/play_sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/pos.py
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/relocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/true_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/commands/water_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:21:33.704070 deebot-client-1.6.1/deebot_client/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/events/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/events/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/events/event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/events/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/events/water_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/logging_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:21:33.704070 deebot-client-1.6.1/deebot_client/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/messages/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/messages/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-03-02 17:21:29.000000 deebot-client-1.6.1/deebot_client/vacuum_bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:21:33.700070 deebot-client-1.6.1/deebot_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-03-02 17:21:33.000000 deebot-client-1.6.1/deebot_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-03-02 17:21:33.000000 deebot-client-1.6.1/deebot_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 17:21:33.000000 deebot-client-1.6.1/deebot_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-02 17:21:33.000000 deebot-client-1.6.1/deebot_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-02 17:21:33.000000 deebot-client-1.6.1/deebot_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-02 17:21:29.000000 deebot-client-1.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-02 17:21:33.708070 deebot-client-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-03-02 17:21:29.000000 deebot-client-1.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:21:33.696069 deebot-client-1.6.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:21:33.704070 deebot-client-1.6.1/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/commands/test_advanced_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/commands/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/commands/test_carpet.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/commands/test_charge.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/commands/test_charge_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/commands/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/commands/test_clean_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/commands/test_clean_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/commands/test_clean_preference.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/commands/test_continuous_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/commands/test_fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/commands/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/commands/test_mulitmap_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/commands/test_true_detect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:21:33.704070 deebot-client-1.6.1/tests/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/events/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/events/test_water_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 17:21:33.704070 deebot-client-1.6.1/tests/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/messages/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-02 17:21:29.000000 deebot-client-1.6.1/tests/messages/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:05.819820 deebot-client-2.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-16 10:11:05.823820 deebot-client-2.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:05.815820 deebot-client-2.0.0b1/deebot_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:05.819820 deebot-client-2.0.0b1/deebot_client/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/advanced_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/carpet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/clean_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/clean_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/clean_preference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/continuous_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/life_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/multimap_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/play_sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/pos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/relocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/true_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/commands/water_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:05.819820 deebot-client-2.0.0b1/deebot_client/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/events/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/events/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/events/event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/events/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/events/water_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/logging_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:05.819820 deebot-client-2.0.0b1/deebot_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/messages/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/messages/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8742 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/deebot_client/vacuum_bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:05.815820 deebot-client-2.0.0b1/deebot_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-16 10:11:05.000000 deebot-client-2.0.0b1/deebot_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-16 10:11:05.000000 deebot-client-2.0.0b1/deebot_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 10:11:05.000000 deebot-client-2.0.0b1/deebot_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-16 10:11:05.000000 deebot-client-2.0.0b1/deebot_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-16 10:11:05.000000 deebot-client-2.0.0b1/deebot_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-16 10:11:05.823820 deebot-client-2.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-16 10:11:01.000000 deebot-client-2.0.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:05.815820 deebot-client-2.0.0b1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:05.819820 deebot-client-2.0.0b1/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_advanced_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_carpet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_clean_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_clean_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_clean_preference.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_continuous_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_life_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_mulitmap_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_true_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/commands/test_water_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:05.819820 deebot-client-2.0.0b1/tests/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/events/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/events/test_water_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:11:05.819820 deebot-client-2.0.0b1/tests/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/messages/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/messages/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-16 10:11:00.000000 deebot-client-2.0.0b1/tests/messages/test_stats.py
```

### Comparing `deebot-client-1.6.1/LICENSE.txt` & `deebot-client-2.0.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deebot-client-1.6.1/PKG-INFO` & `deebot-client-2.0.0b1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deebot-client
-Version: 1.6.1
+Version: 2.0.0b1
 Summary: a library for controlling certain deebot vacuums
 Home-page: https://github.com/DeebotUniverse/client.py
 Author: DeebotUniverse
 Author-email: deebotuniverse@knatschig-as-hell.info
 License: GPL-3.0
 Keywords: home automation vacuum robot deebot ecovacs
 Classifier: Development Status :: 4 - Beta
@@ -37,20 +37,21 @@
 
 ```python
 import aiohttp
 import asyncio
 import logging
 import time
 
-from deebot_client import create_instances
+from deebot_client.api_client import ApiClient
+from deebot_client.authentication import Authenticator
 from deebot_client.commands import *
 from deebot_client.commands.clean import CleanAction
-from deebot_client.models import Configuration
-from deebot_client.mqtt_client import MqttClient
 from deebot_client.events import BatteryEvent
+from deebot_client.models import Configuration
+from deebot_client.mqtt_client import MqttClient, MqttConfiguration
 from deebot_client.util import md5
 from deebot_client.vacuum_bot import VacuumBot
 
 device_id = md5(str(time.time()))
 account_id = "your email or phonenumber (cn)"
 password_hash = md5("yourPassword")
 continent = "eu"
@@ -60,22 +61,24 @@
 async def main():
   async with aiohttp.ClientSession() as session:
     logging.basicConfig(level=logging.DEBUG)
     config = Configuration(session,
                            device_id=device_id, country=country, continent=continent,
                            )
 
-    (authenticator, api_client) = create_instances(config, account_id, password_hash)
+    authenticator = Authenticator(config, account_id, password_hash)
+    api_client = ApiClient(authenticator)
 
     devices_ = await api_client.get_devices()
 
-    bot = VacuumBot(devices_[0], api_client)
+    bot = VacuumBot(devices_[0], authenticator)
 
-    mqtt = MqttClient(config, authenticator)
-    await mqtt.initialize()
+    mqtt_config = MqttConfiguration(config=config)
+    mqtt = MqttClient(mqtt_config, authenticator)
+    await mqtt.connect()
     await mqtt.subscribe(bot)
 
     async def on_battery(event: BatteryEvent):
       # Do stuff on battery event
       if event.value == 100:
         # Battery full
         pass
```

### Comparing `deebot-client-1.6.1/README.md` & `deebot-client-2.0.0b1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,20 +19,21 @@
 
 ```python
 import aiohttp
 import asyncio
 import logging
 import time
 
-from deebot_client import create_instances
+from deebot_client.api_client import ApiClient
+from deebot_client.authentication import Authenticator
 from deebot_client.commands import *
 from deebot_client.commands.clean import CleanAction
-from deebot_client.models import Configuration
-from deebot_client.mqtt_client import MqttClient
 from deebot_client.events import BatteryEvent
+from deebot_client.models import Configuration
+from deebot_client.mqtt_client import MqttClient, MqttConfiguration
 from deebot_client.util import md5
 from deebot_client.vacuum_bot import VacuumBot
 
 device_id = md5(str(time.time()))
 account_id = "your email or phonenumber (cn)"
 password_hash = md5("yourPassword")
 continent = "eu"
@@ -42,22 +43,24 @@
 async def main():
   async with aiohttp.ClientSession() as session:
     logging.basicConfig(level=logging.DEBUG)
     config = Configuration(session,
                            device_id=device_id, country=country, continent=continent,
                            )
 
-    (authenticator, api_client) = create_instances(config, account_id, password_hash)
+    authenticator = Authenticator(config, account_id, password_hash)
+    api_client = ApiClient(authenticator)
 
     devices_ = await api_client.get_devices()
 
-    bot = VacuumBot(devices_[0], api_client)
+    bot = VacuumBot(devices_[0], authenticator)
 
-    mqtt = MqttClient(config, authenticator)
-    await mqtt.initialize()
+    mqtt_config = MqttConfiguration(config=config)
+    mqtt = MqttClient(mqtt_config, authenticator)
+    await mqtt.connect()
     await mqtt.subscribe(bot)
 
     async def on_battery(event: BatteryEvent):
       # Do stuff on battery event
       if event.value == 100:
         # Battery full
         pass
```

### Comparing `deebot-client-1.6.1/deebot_client/_api_client.py` & `deebot-client-2.0.0b1/tests/commands/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,86 @@
-"""Internal api client module."""
-import asyncio
+from collections.abc import Sequence
 from typing import Any
-from urllib.parse import urljoin
+from unittest.mock import AsyncMock, Mock, call
 
-from aiohttp import ClientResponseError
-
-from .const import REALM
-from .logging_filter import get_logger
-from .models import Configuration, Credentials
-
-_LOGGER = get_logger(__name__)
-
-
-def _get_portal_url(config: Configuration, path: str) -> str:
-    subdomain = f"portal-{config.continent}" if config.country != "cn" else "portal"
-    return urljoin(f"https://{subdomain}.ecouser.net/api/", path)
-
-
-class _InternalApiClient:
-    """Internal api client.
-
-    Only required for AuthClient and ApiClient. For all other usecases use APIClient instead.
-    """
-
-    def __init__(self, config: Configuration):
-        self._config = config
-
-    async def post(
-        self,
-        path: str,
-        json: dict[str, Any],
-        *,
-        query_params: dict[str, Any] | None = None,
-        headers: dict[str, Any] | None = None,
-        credentials: Credentials | None = None,
-    ) -> dict[str, Any]:
-        """Perform a post request."""
-        url = _get_portal_url(self._config, path)
-
-        logger_msg = f"calling api: url={url}, params={query_params}, json={json}"
-        _LOGGER.debug(logger_msg)
-
-        if credentials is not None:
-            json.update(
-                {
-                    "auth": {
-                        "with": "users",
-                        "userid": credentials.user_id,
-                        "realm": REALM,
-                        "token": credentials.token,
-                        "resource": self._config.device_id,
-                    }
-                }
-            )
-
-        try:
-            async with self._config.session.post(
-                url,
-                json=json,
-                params=query_params,
-                headers=headers,
-                timeout=60,
-                ssl=self._config.verify_ssl,
-            ) as res:
-                res.raise_for_status()
-                if res.status == 200:
-                    response_data: dict[str, Any] = await res.json()
-                    _LOGGER.debug("Success: %s, response=%s", logger_msg, response_data)
-                    return response_data
-
-                _LOGGER.warning("Error calling API (%d): %s", res.status, path)
-                _LOGGER.debug("Error: %s, status=%s", logger_msg, res.status)
-        except asyncio.TimeoutError:
-            command = ""
-            if "cmdName" in json:
-                command = f"({json['cmdName']})"
-            _LOGGER.warning("Timeout reached on api path: %s%s", path, command)
-            _LOGGER.debug("Timeout on %s", logger_msg)
-        except ClientResponseError as err:
-            if err.status == 502:
-                _LOGGER.info(
-                    "Error calling API (502): Unfortunately the ecovacs api is unreliable. URL was: %s",
-                    url,
-                )
-            else:
-                _LOGGER.warning("Error calling API (%d): %s", err.status, url)
-            _LOGGER.debug("Error: %s, status=%s", logger_msg, err.status)
-
-        return {}
+from deebot_client.authentication import Authenticator
+from deebot_client.command import Command
+from deebot_client.commands import SetCommand
+from deebot_client.events import Event
+from deebot_client.events.event_bus import EventBus
+from deebot_client.models import Credentials, DeviceInfo
+
+from ..helpers import get_message_json, get_request_json
+
+
+async def assert_command(
+    command: Command,
+    json_api_response: dict[str, Any],
+    expected_events: Event | None | Sequence[Event],
+) -> None:
+    event_bus = Mock(spec_set=EventBus)
+    authenticator = Mock(spec_set=Authenticator)
+    authenticator.authenticate = AsyncMock(
+        return_value=Credentials("token", "user_id", 9999)
+    )
+    authenticator.post_authenticated = AsyncMock(return_value=json_api_response)
+    device_info = DeviceInfo(
+        {
+            "company": "company",
+            "did": "did",
+            "name": "name",
+            "nick": "nick",
+            "resource": "resource",
+            "deviceName": "device_name",
+            "status": 1,
+            "class": "get_class",
+        }
+    )
+
+    await command.execute(authenticator, device_info, event_bus)
+
+    # verify
+    authenticator.post_authenticated.assert_called()
+    if expected_events:
+        if isinstance(expected_events, Sequence):
+            event_bus.notify.assert_has_calls([call(x) for x in expected_events])
+            assert event_bus.notify.call_count == len(expected_events)
+        else:
+            event_bus.notify.assert_called_once_with(expected_events)
+    else:
+        event_bus.notify.assert_not_called()
+
+
+async def assert_set_command(
+    command: SetCommand,
+    args: dict | list | None,
+    expected_get_command_event: Event,
+) -> None:
+    assert command.name != "invalid"
+    assert command._args == args
+
+    json = get_request_json({"code": 0, "msg": "ok"})
+    await assert_command(command, json, None)
+
+    event_bus = Mock(spec_set=EventBus)
+
+    # Failed to set
+    json = {
+        "header": {
+            "pri": 1,
+            "tzm": 480,
+            "ts": "1304623069888",
+            "ver": "0.0.1",
+            "fwVer": "1.8.2",
+            "hwVer": "0.1.1",
+        },
+        "body": {
+            "code": 500,
+            "msg": "fail",
+        },
+    }
+    command.handle_mqtt_p2p(event_bus, json)
+    event_bus.notify.assert_not_called()
+
+    # Success
+    command.handle_mqtt_p2p(event_bus, get_message_json(None))
+    event_bus.notify.assert_called_once_with(expected_get_command_event)
```

### Comparing `deebot-client-1.6.1/deebot_client/authentication.py` & `deebot-client-2.0.0b1/deebot_client/authentication.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Authentication module."""
 import asyncio
 import time
 from collections.abc import Callable, Mapping
 from typing import Any
+from urllib.parse import urljoin
 
-from aiohttp import hdrs
+from aiohttp import ClientResponseError, hdrs
 
-from ._api_client import _InternalApiClient
 from .const import REALM
-from .exceptions import AuthenticationError, InvalidAuthenticationError
+from .exceptions import ApiError, AuthenticationError, InvalidAuthenticationError
 from .logging_filter import get_logger
 from .models import Configuration, Credentials
 from .util import md5
 
 _LOGGER = get_logger(__name__)
 
 _CLIENT_KEY = "1520391301804"
@@ -30,28 +30,32 @@
 _META = {
     "lang": "EN",
     "appCode": "global_e",
     "appVersion": "1.6.3",
     "channel": "google_play",
     "deviceType": "1",
 }
+MAX_RETRIES = 3
+
+
+def _get_portal_url(config: Configuration, path: str) -> str:
+    subdomain = f"portal-{config.continent}" if config.country != "cn" else "portal"
+    return urljoin(f"https://{subdomain}.ecouser.net/api/", path)
 
 
 class _AuthClient:
     """Ecovacs auth client."""
 
     def __init__(
         self,
         config: Configuration,
-        internal_api_client: _InternalApiClient,
         account_id: str,
         password_hash: str,
     ):
         self._config = config
-        self._api_client = internal_api_client
         self._account_id = account_id
         self._password_hash = password_hash
         self._tld = "com" if self._config.country != "cn" else "cn"
 
         self._meta: dict[str, str] = {
             **_META,
             "country": self._config.country,
@@ -186,43 +190,124 @@
             "country": self._config.country.upper()
             if self._config.country != "cn"
             else "Chinese",
             "todo": "loginByItToken",
         }
 
         for i in range(3):
-            resp = await self._api_client.post(_PATH_USERS_USER, data)
+            resp = await self.post(_PATH_USERS_USER, data)
             if resp["result"] == "ok":
                 return resp
             if resp["result"] == "fail" and resp["error"] == "set token error.":
                 # If it is a set token error try again
                 _LOGGER.warning("loginByItToken set token error, attempt %d/3", i + 2)
                 continue
 
             _LOGGER.error("call to %s failed with %s", _PATH_USERS_USER, resp)
             raise AuthenticationError(
                 f"failure {resp['error']} ({resp['errno']}) for call {_PATH_USERS_USER}"
             )
 
         raise AuthenticationError("failed to login with token")
 
+    async def post(
+        self,
+        path: str,
+        json: dict[str, Any],
+        *,
+        query_params: dict[str, Any] | None = None,
+        headers: dict[str, Any] | None = None,
+        credentials: Credentials | None = None,
+    ) -> dict[str, Any]:
+        """Perform a post request."""
+        url = _get_portal_url(self._config, path)
+        logger_requst_params = f"url={url}, params={query_params}, json={json}"
+
+        if credentials is not None:
+            json.update(
+                {
+                    "auth": {
+                        "with": "users",
+                        "userid": credentials.user_id,
+                        "realm": REALM,
+                        "token": credentials.token,
+                        "resource": self._config.device_id,
+                    }
+                }
+            )
+
+        for i in range(MAX_RETRIES):
+            _LOGGER.debug(
+                "Calling api(%d/%d): %s",
+                i + 1,
+                MAX_RETRIES,
+                logger_requst_params,
+            )
+
+            try:
+                async with self._config.session.post(
+                    url,
+                    json=json,
+                    params=query_params,
+                    headers=headers,
+                    timeout=60,
+                    ssl=self._config.verify_ssl,
+                ) as res:
+                    if res.status == 200:
+                        response_data: dict[str, Any] = await res.json()
+                        _LOGGER.debug(
+                            "Success calling api %s, response=%s",
+                            logger_requst_params,
+                            response_data,
+                        )
+                        return response_data
+
+                    _LOGGER.debug(
+                        "Error calling api %s, response=%s", logger_requst_params, res
+                    )
+                    raise ClientResponseError(
+                        res.request_info,
+                        res.history,
+                        status=res.status,
+                        message=str(res.reason),
+                        headers=res.headers,
+                    )
+            except asyncio.TimeoutError as ex:
+                _LOGGER.warning(
+                    "Timeout reached on api path: %s%s", path, json.get("cmdName", "")
+                )
+                raise ApiError("Timeout reached") from ex
+            except ClientResponseError as ex:
+                _LOGGER.debug("Error: %s", logger_requst_params, exc_info=True)
+                if ex.status == 502:
+                    seconds_to_sleep = 10
+                    _LOGGER.info(
+                        "Retry calling API due 502: Unfortunately the ecovacs api is unreliable. Retrying in %d seconds",
+                        seconds_to_sleep,
+                    )
+
+                    await asyncio.sleep(seconds_to_sleep)
+                    continue
+
+                raise ApiError from ex
+
+        raise ApiError("Unknown error occurred")
+
 
 class Authenticator:
     """Authenticator."""
 
     def __init__(
         self,
         config: Configuration,
-        ecovacs_api_client: _InternalApiClient,
         account_id: str,
         password_hash: str,
     ):
         self._auth_client = _AuthClient(
             config,
-            ecovacs_api_client,
             account_id,
             password_hash,
         )
 
         self._lock = asyncio.Lock()
         self._on_credentials_changed: set[Callable[[Credentials], None]] = set()
         self._credentials: Credentials | None = None
@@ -279,7 +364,24 @@
                 await self.authenticate(True)
             except Exception:  # pylint: disable=broad-except
                 _LOGGER.error(
                     "An exception occurred during refreshing token", exc_info=True
                 )
 
         asyncio.create_task(refresh())
+
+    async def post_authenticated(
+        self,
+        path: str,
+        json: dict[str, Any],
+        *,
+        query_params: dict[str, Any] | None = None,
+        headers: dict[str, Any] | None = None,
+    ) -> dict[str, Any]:
+        """Perform an authenticated post request."""
+        return await self._auth_client.post(
+            path,
+            json,
+            query_params=query_params,
+            headers=headers,
+            credentials=await self.authenticate(),
+        )
```

### Comparing `deebot-client-1.6.1/deebot_client/commands/__init__.py` & `deebot-client-2.0.0b1/deebot_client/commands/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Commands module."""
 from typing import Dict, Type
 
+from ..command import Command
 from .advanced_mode import GetAdvancedMode, SetAdvancedMode
 from .battery import GetBattery
 from .carpet import GetCarpetAutoFanBoost, SetCarpetAutoFanBoost
 from .charge import Charge
 from .charge_state import GetChargeState
 from .clean import Clean, CleanArea, GetCleanInfo
 from .clean_count import GetCleanCount, SetCleanCount
 from .clean_logs import GetCleanLogs
 from .clean_preference import GetCleanPreference, SetCleanPreference
-from .common import CommandWithHandling, CommandWithMqttP2PHandling, SetCommand
+from .common import CommandHandlingMqttP2P, SetCommand
 from .continuous_cleaning import GetContinuousCleaning, SetContinuousCleaning
 from .error import GetError
 from .fan_speed import FanSpeedLevel, GetFanSpeed, SetFanSpeed
 from .life_span import GetLifeSpan, ResetLifeSpan
 from .map import (
     GetCachedMapInfo,
     GetMajorMap,
@@ -30,15 +31,15 @@
 from .stats import GetStats, GetTotalStats
 from .true_detect import GetTrueDetect, SetTrueDetect
 from .volume import GetVolume, SetVolume
 from .water_info import GetWaterInfo, SetWaterInfo
 
 # fmt: off
 # ordered by file asc
-_COMMANDS: list[type[CommandWithHandling]] = [
+_COMMANDS: list[type[Command]] = [
     GetAdvancedMode,
     SetAdvancedMode,
 
     GetBattery,
 
     GetCarpetAutoFanBoost,
     SetCarpetAutoFanBoost,
@@ -96,16 +97,16 @@
     SetVolume,
 
     GetWaterInfo,
     SetWaterInfo,
 ]
 # fmt: on
 
-COMMANDS_WITH_HANDLING: dict[str, type[CommandWithHandling]] = {
-    cmd.name: cmd for cmd in _COMMANDS
+COMMANDS_WITH_HANDLING: dict[str, type[Command]] = {
+    cmd.name: cmd for cmd in _COMMANDS  # type: ignore[misc]
 }
 
-COMMANDS_WITH_MQTT_P2P_HANDLING: dict[str, type[CommandWithMqttP2PHandling]] = {
+COMMANDS_WITH_MQTT_P2P_HANDLING: dict[str, type[CommandHandlingMqttP2P]] = {
     cmd_name: cmd
     for (cmd_name, cmd) in COMMANDS_WITH_HANDLING.items()
-    if issubclass(cmd, CommandWithMqttP2PHandling)
+    if issubclass(cmd, CommandHandlingMqttP2P)
 }
```

### Comparing `deebot-client-1.6.1/deebot_client/commands/charge.py` & `deebot-client-2.0.0b1/deebot_client/commands/charge.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Charge commands."""
 from typing import Any
 
 from ..events import StatusEvent
 from ..logging_filter import get_logger
 from ..message import HandlingResult
 from ..models import VacuumState
-from .common import EventBus, _ExecuteCommand
+from .common import EventBus, ExecuteCommand
 from .const import CODE
 
 _LOGGER = get_logger(__name__)
 
 
-class Charge(_ExecuteCommand):
+class Charge(ExecuteCommand):
     """Charge command."""
 
     name = "charge"
 
     def __init__(self) -> None:
         super().__init__({"act": "go"})
```

### Comparing `deebot-client-1.6.1/deebot_client/commands/charge_state.py` & `deebot-client-2.0.0b1/deebot_client/commands/charge_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Charge state commands."""
 from typing import Any
 
 from ..events import StatusEvent
-from ..message import HandlingResult
+from ..message import HandlingResult, MessageBodyDataDict
 from ..models import VacuumState
-from .common import EventBus, _NoArgsCommand
+from .common import EventBus, NoArgsCommand
 from .const import CODE
 
 
-class GetChargeState(_NoArgsCommand):
+class GetChargeState(NoArgsCommand, MessageBodyDataDict):
     """Get charge state command."""
 
     name = "getChargeState"
 
     @classmethod
     def _handle_body_data_dict(
         cls, event_bus: EventBus, data: dict[str, Any]
```

### Comparing `deebot-client-1.6.1/deebot_client/commands/clean_count.py` & `deebot-client-2.0.0b1/deebot_client/commands/clean_count.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Clean count command module."""
 
 from collections.abc import Mapping
 from typing import Any
 
 from ..events import CleanCountEvent
-from ..message import HandlingResult
-from .common import EventBus, SetCommand, _NoArgsCommand
+from ..message import HandlingResult, MessageBodyDataDict
+from .common import EventBus, NoArgsCommand, SetCommand
 
 
-class GetCleanCount(_NoArgsCommand):
+class GetCleanCount(NoArgsCommand, MessageBodyDataDict):
     """Get clean count command."""
 
     name = "getCleanCount"
 
     @classmethod
     def _handle_body_data_dict(
         cls, event_bus: EventBus, data: dict[str, Any]
```

### Comparing `deebot-client-1.6.1/deebot_client/commands/clean_logs.py` & `deebot-client-2.0.0b1/deebot_client/commands/clean_logs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,58 @@
 """clean log commands."""
 from typing import Any
 
+from ..authentication import Authenticator
+from ..command import Command, CommandResult
+from ..const import PATH_API_LG_LOG, REQUEST_HEADERS
 from ..events import CleanJobStatus, CleanLogEntry, CleanLogEvent
-from ..exceptions import DeebotError
+from ..events.event_bus import EventBus
 from ..logging_filter import get_logger
-from ..message import HandlingResult
-from .common import CommandResult, CommandWithHandling, EventBus
+from ..models import DeviceInfo
 
 _LOGGER = get_logger(__name__)
 
 
-class GetCleanLogs(CommandWithHandling):
+class GetCleanLogs(Command):
     """Get clean logs command."""
 
     name = "GetCleanLogs"
 
     def __init__(self, count: int = 0) -> None:
         super().__init__({"count": count})
 
-    def _handle_requested(
+    async def _execute_api_request(
+        self, authenticator: Authenticator, device_info: DeviceInfo
+    ) -> dict[str, Any]:
+        json = {
+            "td": self.name,
+            "did": device_info.did,
+            "resource": device_info.resource,
+        }
+
+        credentials = await authenticator.authenticate()
+        query_params = {
+            "td": json["td"],
+            "u": credentials.user_id,
+            "cv": "1.67.3",
+            "t": "a",
+            "av": "1.3.1",
+        }
+
+        return await authenticator.post_authenticated(
+            PATH_API_LG_LOG,
+            json,
+            query_params=query_params,
+            headers=REQUEST_HEADERS,
+        )
+
+    def _handle_response(
         self, event_bus: EventBus, response: dict[str, Any]
     ) -> CommandResult:
-        """Handle response from a manual requested command.
+        """Handle response from a command.
 
         :return: A message response
         """
         if response["ret"] == "ok":
             resp_logs: list[dict] | None = response.get("logs")
 
             # Ecovacs API is changing their API, this request may not work properly
@@ -48,11 +75,7 @@
                     except Exception:  # pylint: disable=broad-except
                         _LOGGER.warning("Skipping log entry: %s", log, exc_info=True)
 
                 event_bus.notify(CleanLogEvent(logs))
                 return CommandResult.success()
 
         return CommandResult.analyse()
-
-    @classmethod
-    def _handle_body(cls, event_bus: EventBus, body: dict[str, Any]) -> HandlingResult:
-        raise DeebotError("Should never be called!")
```

### Comparing `deebot-client-1.6.1/deebot_client/commands/custom.py` & `deebot-client-2.0.0b1/deebot_client/commands/custom.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 """Custom command module."""
 from typing import Any
 
+from ..command import Command, CommandResult, EventBus
 from ..events import CustomCommandEvent
 from ..logging_filter import get_logger
 from ..message import HandlingState
-from .common import CommandResult, EventBus
 
 _LOGGER = get_logger(__name__)
 
 
-class CustomCommand:
+class CustomCommand(Command):
     """Custom command, used when user wants to execute a command, which is not part of this library."""
 
+    name = "CustomCommand"
+
     def __init__(self, name: str, args: dict | list | None = None) -> None:
         self._name = name
-        if args is None:
-            args = {}
-        self._args = args
-
-    @property
-    def name(self) -> str:
-        """Command name."""
-        return self._name
-
-    @property
-    def args(self) -> dict[str, Any] | list:
-        """Command additional arguments."""
-        return self._args
+        super().__init__(args)
 
-    def handle_requested(
-        self, events: EventBus, response: dict[str, Any]
+    def _handle_response(
+        self, event_bus: EventBus, response: dict[str, Any]
     ) -> CommandResult:
-        """Handle response from a manual requested command.
+        """Handle response from a command.
 
         :return: A message response
         """
         if response.get("ret") == "ok":
             data = response.get("resp", response)
-            events.notify(CustomCommandEvent(self.name, data))
+            event_bus.notify(CustomCommandEvent(self._name, data))
             return CommandResult.success()
 
-        _LOGGER.warning('Command "%s" was not successfully: %s', self.name, response)
+        _LOGGER.warning('Command "%s" was not successfully: %s', self._name, response)
         return CommandResult(HandlingState.FAILED)
+
+    def __eq__(self, obj: object) -> bool:
+        if super().__eq__(obj) and isinstance(obj, CustomCommand):
+            return self._name == obj._name
+
+        return False
+
+    def __hash__(self) -> int:
+        return super().__hash__() + hash(self._name)
+
+
+class CustomPayloadCommand(CustomCommand):
+    """Custom command, where args is the raw payload."""
+
+    def _get_payload(self) -> dict[str, Any] | list:
+        return self._args
```

### Comparing `deebot-client-1.6.1/deebot_client/commands/error.py` & `deebot-client-2.0.0b1/deebot_client/commands/error.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Error commands."""
 from typing import Any
 
 from ..events import ErrorEvent, StatusEvent
-from ..message import HandlingResult
+from ..message import HandlingResult, MessageBodyDataDict
 from ..models import VacuumState
-from .common import EventBus, _NoArgsCommand
+from .common import EventBus, NoArgsCommand
 
 
-class GetError(_NoArgsCommand):
+class GetError(NoArgsCommand, MessageBodyDataDict):
     """Get error command."""
 
     name = "getError"
 
     @classmethod
     def _handle_body_data_dict(
         cls, event_bus: EventBus, data: dict[str, Any]
```

### Comparing `deebot-client-1.6.1/deebot_client/commands/fan_speed.py` & `deebot-client-2.0.0b1/deebot_client/commands/fan_speed.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """(fan) speed commands."""
 from collections.abc import Mapping
 from typing import Any
 
 from ..events import FanSpeedEvent
-from ..message import HandlingResult
+from ..message import HandlingResult, MessageBodyDataDict
 from ..util import DisplayNameIntEnum
-from .common import EventBus, SetCommand, _NoArgsCommand
+from .common import EventBus, NoArgsCommand, SetCommand
 
 
 class FanSpeedLevel(DisplayNameIntEnum):
     """Enum class for all possible fan speed levels."""
 
     # Values should be sort from low to high on their meanings
     QUIET = 1000
     NORMAL = 0
     MAX = 1
     MAX_PLUS = 2, "max+"
 
 
-class GetFanSpeed(_NoArgsCommand):
+class GetFanSpeed(NoArgsCommand, MessageBodyDataDict):
     """Get fan speed command."""
 
     name = "getSpeed"
 
     @classmethod
     def _handle_body_data_dict(
         cls, event_bus: EventBus, data: dict[str, Any]
```

### Comparing `deebot-client-1.6.1/deebot_client/commands/life_span.py` & `deebot-client-2.0.0b1/deebot_client/commands/life_span.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Life span commands."""
 from typing import Any
 
 from ..events import LifeSpan, LifeSpanEvent
-from ..message import HandlingResult, HandlingState
+from ..message import HandlingResult, HandlingState, MessageBodyDataList
 from .common import (
-    CommandWithHandling,
-    CommandWithMqttP2PHandling,
+    CommandHandlingMqttP2P,
+    CommandWithMessageHandling,
     EventBus,
-    _ExecuteCommand,
+    ExecuteCommand,
 )
 
 
-class GetLifeSpan(CommandWithHandling):
+class GetLifeSpan(CommandWithMessageHandling, MessageBodyDataList):
     """Get life span command."""
 
     name = "getLifeSpan"
 
     def __init__(self) -> None:
         args = [life_span.value for life_span in LifeSpan]
         super().__init__(args)
@@ -36,15 +36,15 @@
 
             percent = round((left / total) * 100, 2)
             event_bus.notify(LifeSpanEvent(component_type, percent, left))
 
         return HandlingResult.success()
 
 
-class ResetLifeSpan(_ExecuteCommand, CommandWithMqttP2PHandling):
+class ResetLifeSpan(ExecuteCommand, CommandHandlingMqttP2P):
     """Reset life span command."""
 
     name = "resetLifeSpan"
 
     def __init__(
         self, type: str | LifeSpan  # pylint: disable=redefined-builtin
     ) -> None:
```

### Comparing `deebot-client-1.6.1/deebot_client/commands/map.py` & `deebot-client-2.0.0b1/deebot_client/commands/map.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,59 +7,63 @@
     MapSetEvent,
     MapSetType,
     MapSubsetEvent,
     MapTraceEvent,
     MinorMapEvent,
 )
 from ..events.event_bus import EventBus
-from ..message import HandlingResult, HandlingState
-from . import CommandWithHandling
-from .common import CommandResult
+from ..events.map import CachedMapInfoEvent
+from ..message import HandlingResult, HandlingState, MessageBodyDataDict
+from .common import CommandResult, CommandWithMessageHandling
 
 
-class GetCachedMapInfo(CommandWithHandling):
+class GetCachedMapInfo(CommandWithMessageHandling, MessageBodyDataDict):
     """Get cached map info command."""
 
     name = "getCachedMapInfo"
 
     @classmethod
     def _handle_body_data_dict(
         cls, event_bus: EventBus, data: dict[str, Any]
     ) -> HandlingResult:
         """Handle message->body->data and notify the correct event subscribers.
 
         :return: A message response
         """
         for map_status in data["info"]:
             if map_status["using"] == 1:
+                event_bus.notify(
+                    CachedMapInfoEvent(name=map_status.get("name", ""), active=True)
+                )
+
                 return HandlingResult(
                     HandlingState.SUCCESS, {"map_id": map_status["mid"]}
                 )
 
         return HandlingResult.analyse()
 
-    def _handle_requested(
+    def _handle_response(
         self, event_bus: EventBus, response: dict[str, Any]
     ) -> CommandResult:
-        """Handle response from a manual requested command.
+        """Handle response from a command.
 
         :return: A message response
         """
-        result = super()._handle_requested(event_bus, response)
+        result = super()._handle_response(event_bus, response)
         if result.state == HandlingState.SUCCESS and result.args:
             return CommandResult(
                 result.state,
                 result.args,
                 [GetMapSet(result.args["map_id"], entry) for entry in MapSetType],
             )
 
         return result
 
 
-class GetMajorMap(CommandWithHandling):
+class GetMajorMap(CommandWithMessageHandling, MessageBodyDataDict):
     """Get major map command."""
 
     name = "getMajorMap"
 
     @classmethod
     def _handle_body_data_dict(
         cls, event_bus: EventBus, data: dict[str, Any]
@@ -72,30 +76,30 @@
         map_id = data["mid"]
 
         return HandlingResult(
             HandlingState.SUCCESS,
             {"map_id": map_id, "values": values},
         )
 
-    def _handle_requested(
+    def _handle_response(
         self, event_bus: EventBus, response: dict[str, Any]
     ) -> CommandResult:
-        """Handle response from a manual requested command.
+        """Handle response from a command.
 
         :return: A message response
         """
-        result = super()._handle_requested(event_bus, response)
+        result = super()._handle_response(event_bus, response)
         if result.state == HandlingState.SUCCESS and result.args:
             event_bus.notify(MajorMapEvent(True, **result.args))
             return CommandResult.success()
 
         return result
 
 
-class GetMapSet(CommandWithHandling):
+class GetMapSet(CommandWithMessageHandling, MessageBodyDataDict):
     """Get map set command."""
 
     _ARGS_ID = "id"
     _ARGS_SET_ID = "set_id"
     _ARGS_TYPE = "type"
     _ARGS_SUBSETS = "subsets"
 
@@ -128,22 +132,22 @@
             cls._ARGS_TYPE: data["type"],
             cls._ARGS_SUBSETS: subsets,
         }
 
         event_bus.notify(MapSetEvent(MapSetType(data["type"]), subsets))
         return HandlingResult(HandlingState.SUCCESS, args)
 
-    def _handle_requested(
+    def _handle_response(
         self, event_bus: EventBus, response: dict[str, Any]
     ) -> CommandResult:
-        """Handle response from a manual requested command.
+        """Handle response from a command.
 
         :return: A message response
         """
-        result = super()._handle_requested(event_bus, response)
+        result = super()._handle_response(event_bus, response)
         if result.state == HandlingState.SUCCESS and result.args:
             commands: list[Command] = []
             for subset in result.args[self._ARGS_SUBSETS]:
                 commands.append(
                     GetMapSubSet(
                         mid=result.args[self._ARGS_ID],
                         msid=result.args[self._ARGS_SET_ID],
@@ -152,15 +156,15 @@
                     )
                 )
             return CommandResult(result.state, result.args, commands)
 
         return result
 
 
-class GetMapSubSet(CommandWithHandling):
+class GetMapSubSet(CommandWithMessageHandling, MessageBodyDataDict):
     """Get map subset command."""
 
     _ROOM_NUM_TO_NAME = {
         "0": "Default",
         "1": "Living Room",
         "2": "Dining Room",
         "3": "Bedroom",
@@ -231,15 +235,15 @@
             )
 
             return HandlingResult.success()
 
         return HandlingResult.analyse()
 
 
-class GetMapTrace(CommandWithHandling):
+class GetMapTrace(CommandWithMessageHandling, MessageBodyDataDict):
     """Get map trace command."""
 
     _TRACE_POINT_COUNT = 200
 
     name = "getMapTrace"
 
     def __init__(self, trace_start: int = 0) -> None:
@@ -263,31 +267,31 @@
             return HandlingResult.analyse()
 
         event_bus.notify(
             MapTraceEvent(start=start, total=total, data=data["traceValue"])
         )
         return HandlingResult(HandlingState.SUCCESS, {"start": start, "total": total})
 
-    def _handle_requested(
+    def _handle_response(
         self, event_bus: EventBus, response: dict[str, Any]
     ) -> CommandResult:
-        """Handle response from a manual requested command.
+        """Handle response from a command.
 
         :return: A message response
         """
-        result = super()._handle_requested(event_bus, response)
+        result = super()._handle_response(event_bus, response)
         if result.state == HandlingState.SUCCESS and result.args:
             start = result.args["start"] + self._TRACE_POINT_COUNT
             if start < result.args["total"]:
                 return CommandResult(result.state, result.args, [GetMapTrace(start)])
 
         return result
 
 
-class GetMinorMap(CommandWithHandling):
+class GetMinorMap(CommandWithMessageHandling, MessageBodyDataDict):
     """Get minor map command."""
 
     name = "getMinorMap"
 
     def __init__(self, *, map_id: str, piece_index: int) -> None:
         super().__init__({"mid": map_id, "type": "ol", "pieceIndex": piece_index})
```

### Comparing `deebot-client-1.6.1/deebot_client/commands/pos.py` & `deebot-client-2.0.0b1/deebot_client/commands/pos.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Position command module."""
 
 from typing import Any
 
 from ..events import Position, PositionsEvent, PositionType
-from ..message import HandlingResult
-from .common import CommandWithHandling, EventBus
+from ..message import HandlingResult, MessageBodyDataDict
+from .common import CommandWithMessageHandling, EventBus
 
 
-class GetPos(CommandWithHandling):
+class GetPos(CommandWithMessageHandling, MessageBodyDataDict):
     """Get volume command."""
 
     name = "getPos"
 
     def __init__(self) -> None:
         super().__init__(["chargePos", "deebotPos"])
```

### Comparing `deebot-client-1.6.1/deebot_client/commands/stats.py` & `deebot-client-2.0.0b1/deebot_client/commands/stats.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Stats commands."""
 from typing import Any
 
 from ..events import StatsEvent, TotalStatsEvent
-from ..message import HandlingResult
-from .common import EventBus, _NoArgsCommand
+from ..message import HandlingResult, MessageBodyDataDict
+from .common import EventBus, NoArgsCommand
 
 
-class GetStats(_NoArgsCommand):
+class GetStats(NoArgsCommand, MessageBodyDataDict):
     """Get stats command."""
 
     name = "getStats"
 
     @classmethod
     def _handle_body_data_dict(
         cls, event_bus: EventBus, data: dict[str, Any]
@@ -24,15 +24,15 @@
             time=data.get("time"),
             type=data.get("type"),
         )
         event_bus.notify(stats_event)
         return HandlingResult.success()
 
 
-class GetTotalStats(_NoArgsCommand):
+class GetTotalStats(NoArgsCommand, MessageBodyDataDict):
     """Get stats command."""
 
     name = "getTotalStats"
 
     @classmethod
     def _handle_body_data_dict(
         cls, event_bus: EventBus, data: dict[str, Any]
```

### Comparing `deebot-client-1.6.1/deebot_client/commands/volume.py` & `deebot-client-2.0.0b1/deebot_client/commands/volume.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Volume command module."""
 
 from collections.abc import Mapping
 from typing import Any
 
 from ..events import VolumeEvent
-from ..message import HandlingResult
-from .common import EventBus, SetCommand, _NoArgsCommand
+from ..message import HandlingResult, MessageBodyDataDict
+from .common import EventBus, NoArgsCommand, SetCommand
 
 
-class GetVolume(_NoArgsCommand):
+class GetVolume(NoArgsCommand, MessageBodyDataDict):
     """Get volume command."""
 
     name = "getVolume"
 
     @classmethod
     def _handle_body_data_dict(
         cls, event_bus: EventBus, data: dict[str, Any]
```

### Comparing `deebot-client-1.6.1/deebot_client/commands/water_info.py` & `deebot-client-2.0.0b1/deebot_client/commands/water_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """Water info commands."""
 from collections.abc import Mapping
 from typing import Any
 
 from ..events import WaterAmount, WaterInfoEvent
-from ..message import HandlingResult
-from .common import EventBus, SetCommand, _NoArgsCommand
+from ..message import HandlingResult, MessageBodyDataDict
+from .common import EventBus, NoArgsCommand, SetCommand
 
 
-class GetWaterInfo(_NoArgsCommand):
+class GetWaterInfo(NoArgsCommand, MessageBodyDataDict):
     """Get water info command."""
 
     name = "getWaterInfo"
 
     @classmethod
     def _handle_body_data_dict(
         cls, event_bus: EventBus, data: dict[str, Any]
     ) -> HandlingResult:
         """Handle message->body->data and notify the correct event subscribers.
 
         :return: A message response
         """
-        # todo enable can be missing pylint: disable=fixme
-        mop_attached = bool(data.get("enable"))
+        mop_attached = data.get("enable", None)
+        if mop_attached is not None:
+            mop_attached = bool(mop_attached)
 
         event_bus.notify(WaterInfoEvent(mop_attached, WaterAmount(int(data["amount"]))))
         return HandlingResult.success()
 
 
 class SetWaterInfo(SetCommand):
     """Set water info command."""
```

### Comparing `deebot-client-1.6.1/deebot_client/events/__init__.py` & `deebot-client-2.0.0b1/deebot_client/events/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot-client-1.6.1/deebot_client/events/const.py` & `deebot-client-2.0.0b1/deebot_client/events/const.py`

 * *Files 12% similar despite different names*

```diff
@@ -47,24 +47,26 @@
     StatusEvent,
     TotalStatsEvent,
     TrueDetectEvent,
     VolumeEvent,
     WaterInfoEvent,
 )
 from .map import (
+    CachedMapInfoEvent,
     MajorMapEvent,
     MapSetEvent,
     MapSubsetEvent,
     MapTraceEvent,
     MinorMapEvent,
 )
 
 EVENT_DTO_REFRESH_COMMANDS: Mapping[type[Event], list[Command]] = {
     AdvancedModeEvent: [GetAdvancedMode()],
     BatteryEvent: [GetBattery()],
+    CachedMapInfoEvent: [GetCachedMapInfo()],
     CarpetAutoFanBoostEvent: [GetCarpetAutoFanBoost()],
     CleanLogEvent: [GetCleanLogs()],
     CleanCountEvent: [GetCleanCount()],
     CleanPreferenceEvent: [GetCleanPreference()],
     ContinuousCleaningEvent: [GetContinuousCleaning()],
     CustomCommandEvent: [],
     ErrorEvent: [GetError()],
```

### Comparing `deebot-client-1.6.1/deebot_client/events/event_bus.py` & `deebot-client-2.0.0b1/deebot_client/events/event_bus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Event emitter module."""
 import asyncio
 import threading
 from collections.abc import Callable, Coroutine
-from typing import Any, Final, Generic, TypeVar
+from typing import TYPE_CHECKING, Any, Final, Generic, TypeVar
 
-from ..command import Command
 from ..logging_filter import get_logger
 from ..models import VacuumState
 from . import Event, StatusEvent
 
+if TYPE_CHECKING:
+    from ..command import Command
+
 _LOGGER = get_logger(__name__)
 
 T = TypeVar("T", bound=Event)
 
 
 class EventListener(Generic[T]):
     """Object that allows event consumers to easily unsubscribe from event bus."""
@@ -50,15 +52,18 @@
         """Return semaphore."""
         return self._semaphore
 
 
 class EventBus:
     """A very simple event bus system."""
 
-    def __init__(self, execute_command: Callable[[Command], Coroutine[Any, Any, None]]):
+    def __init__(
+        self,
+        execute_command: Callable[["Command"], Coroutine[Any, Any, None]],
+    ):
         self._event_processing_dict: dict[type[Event], _EventProcessingData] = {}
         self._lock = threading.Lock()
         self._execute_command: Final = execute_command
 
     def has_subscribers(self, event: type[T]) -> bool:
         """Return True, if emitter has subscribers."""
         return (
@@ -152,7 +157,17 @@
             event_processing_data = self._event_processing_dict.get(event_class, None)
 
             if event_processing_data is None:
                 event_processing_data = _EventProcessingData()
                 self._event_processing_dict[event_class] = event_processing_data
 
             return event_processing_data
+
+    def get_last_event(
+        self,
+        event_type: type[T],
+    ) -> T | None:
+        """Get last event of type T, if available."""
+        if event_processing := self._event_processing_dict.get(event_type, None):
+            return event_processing.last_event
+
+        return None
```

### Comparing `deebot-client-1.6.1/deebot_client/events/map.py` & `deebot-client-2.0.0b1/deebot_client/events/map.py`

 * *Files 9% similar despite different names*

```diff
@@ -83,7 +83,15 @@
 class MapSubsetEvent(Event):
     """Map subset event."""
 
     id: int
     type: MapSetType
     coordinates: str
     name: str | None = None
+
+
+@dataclass(frozen=True)
+class CachedMapInfoEvent(Event):
+    """Cached map info event."""
+
+    name: str
+    active: bool
```

### Comparing `deebot-client-1.6.1/deebot_client/logging_filter.py` & `deebot-client-2.0.0b1/deebot_client/logging_filter.py`

 * *Files identical despite different names*

### Comparing `deebot-client-1.6.1/deebot_client/map.py` & `deebot-client-2.0.0b1/deebot_client/map.py`

 * *Files identical despite different names*

### Comparing `deebot-client-1.6.1/deebot_client/message.py` & `deebot-client-2.0.0b1/deebot_client/message.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Base messages."""
 import functools
-from abc import ABC
+from abc import ABC, abstractmethod
 from collections.abc import Callable
 from dataclasses import dataclass
 from enum import IntEnum, auto
 from typing import Any, final
 
 from .events.event_bus import EventBus
 from .logging_filter import get_logger
@@ -61,75 +61,127 @@
 
     return wrapper
 
 
 class Message(ABC):
     """Message with handling code."""
 
-    # will be overwritten in subclasses
-    name = "__invalid__"
+    @property  # type: ignore[misc]
+    @classmethod
+    @abstractmethod
+    def name(cls) -> str:
+        """Command name."""
 
     @classmethod
-    def _handle_body_data_list(cls, event_bus: EventBus, data: list) -> HandlingResult:
-        """Handle message->body->data and notify the correct event subscribers.
+    @abstractmethod
+    def _handle_body(cls, event_bus: EventBus, body: dict[str, Any]) -> HandlingResult:
+        """Handle message->body and notify the correct event subscribers.
 
         :return: A message response
         """
-        raise NotImplementedError
 
     @classmethod
-    def _handle_body_data_dict(
-        cls, event_bus: EventBus, data: dict[str, Any]
-    ) -> HandlingResult:
-        """Handle message->body->data and notify the correct event subscribers.
+    @_handle_error_or_analyse
+    @final
+    def __handle_body(cls, event_bus: EventBus, body: dict[str, Any]) -> HandlingResult:
+        return cls._handle_body(event_bus, body)
+
+    @classmethod
+    @_handle_error_or_analyse
+    @final
+    def handle(cls, event_bus: EventBus, message: dict[str, Any]) -> HandlingResult:
+        """Handle message and notify the correct event subscribers.
 
         :return: A message response
         """
-        raise NotImplementedError
+        data_body = message.get("body", message)
+        return cls.__handle_body(event_bus, data_body)
+
+
+class MessageBodyData(Message):
+    """Message with handling body->data code."""
 
     @classmethod
+    @abstractmethod
     def _handle_body_data(
         cls, event_bus: EventBus, data: dict[str, Any] | list
     ) -> HandlingResult:
         """Handle message->body->data and notify the correct event subscribers.
 
         :return: A message response
         """
-        if isinstance(data, dict):
-            return cls._handle_body_data_dict(event_bus, data)
-
-        if isinstance(data, list):
-            return cls._handle_body_data_list(event_bus, data)
 
     @classmethod
-    @_handle_error_or_analyse
     @final
     def __handle_body_data(
         cls, event_bus: EventBus, data: dict[str, Any] | list
     ) -> HandlingResult:
-        return cls._handle_body_data(event_bus, data)
+        try:
+            response = cls._handle_body_data(event_bus, data)
+            if response.state == HandlingState.ANALYSE:
+                _LOGGER.debug("Could not handle %s message: %s", cls.name, data)
+                return HandlingResult(HandlingState.ANALYSE_LOGGED, response.args)
+            return response
+        except Exception:  # pylint: disable=broad-except
+            _LOGGER.warning("Could not parse %s: %s", cls.name, data, exc_info=True)
+            return HandlingResult(HandlingState.ERROR)
 
     @classmethod
     def _handle_body(cls, event_bus: EventBus, body: dict[str, Any]) -> HandlingResult:
         """Handle message->body and notify the correct event subscribers.
 
         :return: A message response
         """
         data = body.get("data", body)
         return cls.__handle_body_data(event_bus, data)
 
+
+class MessageBodyDataDict(MessageBodyData):
+    """Message with handling body->data->dict code."""
+
     @classmethod
-    @_handle_error_or_analyse
-    @final
-    def __handle_body(cls, event_bus: EventBus, body: dict[str, Any]) -> HandlingResult:
-        return cls._handle_body(event_bus, body)
+    @abstractmethod
+    def _handle_body_data_dict(
+        cls, event_bus: EventBus, data: dict[str, Any]
+    ) -> HandlingResult:
+        """Handle message->body->data and notify the correct event subscribers.
+
+        :return: A message response
+        """
 
     @classmethod
-    @_handle_error_or_analyse
-    @final
-    def handle(cls, event_bus: EventBus, message: dict[str, Any]) -> HandlingResult:
-        """Handle message and notify the correct event subscribers.
+    def _handle_body_data(
+        cls, event_bus: EventBus, data: dict[str, Any] | list
+    ) -> HandlingResult:
+        """Handle message->body->data and notify the correct event subscribers.
 
         :return: A message response
         """
-        data_body = message.get("body", message)
-        return cls.__handle_body(event_bus, data_body)
+        if isinstance(data, dict):
+            return cls._handle_body_data_dict(event_bus, data)
+
+        return super()._handle_body_data(event_bus, data)
+
+
+class MessageBodyDataList(MessageBodyData):
+    """Message with handling body->data->list code."""
+
+    @classmethod
+    @abstractmethod
+    def _handle_body_data_list(cls, event_bus: EventBus, data: list) -> HandlingResult:
+        """Handle message->body->data and notify the correct event subscribers.
+
+        :return: A message response
+        """
+
+    @classmethod
+    def _handle_body_data(
+        cls, event_bus: EventBus, data: dict[str, Any] | list
+    ) -> HandlingResult:
+        """Handle message->body->data and notify the correct event subscribers.
+
+        :return: A message response
+        """
+        if isinstance(data, list):
+            return cls._handle_body_data_list(event_bus, data)
+
+        return super()._handle_body_data(event_bus, data)
```

### Comparing `deebot-client-1.6.1/deebot_client/messages/battery.py` & `deebot-client-2.0.0b1/deebot_client/messages/battery.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Battery messages."""
 from typing import Any
 
 from ..events import BatteryEvent
 from ..events.event_bus import EventBus
-from ..message import HandlingResult, Message
+from ..message import HandlingResult, MessageBodyDataDict
 
 
-class OnBattery(Message):
+class OnBattery(MessageBodyDataDict):
     """On battery message."""
 
     name = "onBattery"
 
     @classmethod
     def _handle_body_data_dict(
         cls, event_bus: EventBus, data: dict[str, Any]
```

### Comparing `deebot-client-1.6.1/deebot_client/messages/stats.py` & `deebot-client-2.0.0b1/deebot_client/messages/stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Stats messages."""
 from typing import Any
 
 from ..events import CleanJobStatus, ReportStatsEvent
 from ..events.event_bus import EventBus
-from ..message import HandlingResult, Message
+from ..message import HandlingResult, MessageBodyDataDict
 
 
-class ReportStats(Message):
+class ReportStats(MessageBodyDataDict):
     """Report stats message."""
 
     name = "reportStats"
 
     @classmethod
     def _handle_body_data_dict(
         cls, event_bus: EventBus, data: dict[str, Any]
```

### Comparing `deebot-client-1.6.1/deebot_client/models.py` & `deebot-client-2.0.0b1/deebot_client/models.py`

 * *Files identical despite different names*

### Comparing `deebot-client-1.6.1/deebot_client/mqtt_client.py` & `deebot-client-2.0.0b1/deebot_client/mqtt_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """MQTT module."""
+import asyncio
 import json
 import ssl
 from collections.abc import MutableMapping
+from dataclasses import _MISSING_TYPE, InitVar, dataclass, field, fields
 from datetime import datetime
 
 from cachetools import TTLCache
 from gmqtt import Client, Subscription
 from gmqtt.mqtt.constants import MQTTv311
 
 from .authentication import Authenticator
-from .commands import COMMANDS_WITH_MQTT_P2P_HANDLING, CommandWithMqttP2PHandling
-from .exceptions import NotInitializedError
+from .commands import COMMANDS_WITH_MQTT_P2P_HANDLING, CommandHandlingMqttP2P
 from .logging_filter import get_logger
 from .models import Configuration, Credentials, DeviceInfo
 from .vacuum_bot import VacuumBot
 
 _LOGGER = get_logger(__name__)
 
 
@@ -32,29 +33,64 @@
         ),
         Subscription(
             f"iot/p2p/+/{device_info.did}/{device_info.get_class}/{device_info.resource}/+/+/+/p/+/j"
         ),
     ]
 
 
+def _default_ssl_context() -> ssl.SSLContext:
+    ssl_ctx = ssl.create_default_context()
+    ssl_ctx.check_hostname = False
+    ssl_ctx.verify_mode = ssl.CERT_NONE
+    return ssl_ctx
+
+
+@dataclass(frozen=True)
+class MqttConfiguration:
+    """Mqtt configuration."""
+
+    config: InitVar[Configuration]
+    port: int = 443
+    hostname: str = "mq.ecouser.net"
+    ssl_context: ssl.SSLContext | bool = field(default_factory=_default_ssl_context)
+    device_id: str = field(init=False)
+
+    def __post_init__(self, config: Configuration) -> None:
+        for _field in fields(self):
+            # If there is a default and the value of the field is none we can assign a value
+            if (
+                not isinstance(_field.default, _MISSING_TYPE)
+                and getattr(self, _field.name) is None
+            ):
+                object.__setattr__(self, _field.name, _field.default)
+
+        object.__setattr__(self, "device_id", config.device_id)
+
+        if (
+            self.hostname == MqttConfiguration.hostname
+            and config.country.lower() != "cn"
+        ):
+            object.__setattr__(self, "hostname", f"mq-{config.continent}.ecouser.net")
+
+
 class MqttClient:
     """MQTT client."""
 
-    def __init__(self, config: Configuration, authenticator: Authenticator):
+    def __init__(
+        self,
+        config: MqttConfiguration,
+        authenticator: Authenticator,
+    ):
         self._config = config
         self._authenticator = authenticator
-        self._subscribers: MutableMapping[str, VacuumBot] = {}
-        self._port = 443
-        self._hostname = f"mq-{config.continent}.ecouser.net"
-        if config.country.lower() == "cn":
-            self._hostname = "mq.ecouser.net"
+        self._subscribers: MutableMapping[str, SubscriberInfo] = {}
 
         self._client: Client | None = None
         self._received_p2p_commands: MutableMapping[
-            str, CommandWithMqttP2PHandling
+            str, CommandHandlingMqttP2P
         ] = TTLCache(maxsize=60 * 60, ttl=60)
         self._last_message_received_at: datetime | None = None
 
         # pylint: disable=unused-argument
         async def __on_message(
             client: Client, topic: str, payload: bytes, qos: int, properties: dict
         ) -> None:
@@ -72,69 +108,85 @@
         self._on_message = __on_message
 
         def on_credentials_changed(credentials: Credentials) -> None:
             if self._client:
                 self._client.set_auth_credentials(
                     credentials.user_id, credentials.token
                 )
+                asyncio.create_task(self.connect())
 
         authenticator.subscribe(on_credentials_changed)
 
     @property
     def last_message_received_at(self) -> datetime | None:
         """Return the datetime of the last received message or None."""
         return self._last_message_received_at
 
-    async def initialize(self) -> None:
-        """Initialize MQTT."""
+    async def connect(self) -> None:
+        """Connect to the mqtt broker."""
         if self._client:
             await self.disconnect()
 
         credentials = await self._authenticator.authenticate()
         client_id = f"{credentials.user_id}@ecouser/{self._config.device_id}"
         self._client = Client(client_id)
         self._client.on_message = self._on_message
         self._client.set_auth_credentials(credentials.user_id, credentials.token)
 
-        ssl_ctx = ssl.create_default_context()
-        ssl_ctx.check_hostname = False
-        ssl_ctx.verify_mode = ssl.CERT_NONE
+        # pylint: disable=unused-argument
+        def on_connect(client: Client, flags: int, code: int, properties: dict) -> None:
+            if self._subscribers:
+                _LOGGER.debug("Subscribe again to all previous subscriptions")
+                for _, info in self._subscribers.items():
+                    client.subscribe(info.subscriptions)
+
+        self._client.on_connect = on_connect
+
         await self._client.connect(
-            self._hostname, self._port, ssl=ssl_ctx, version=MQTTv311
+            self._config.hostname,
+            self._config.port,
+            ssl=self._config.ssl_context,
+            version=MQTTv311,
         )
 
     async def subscribe(self, vacuum_bot: VacuumBot) -> None:
         """Subscribe for messages for given vacuum."""
-        if self._client is None:
-            raise NotInitializedError
+        if self._client is None or not self._client.is_connected:
+            await self.connect()
+            assert self._client is not None
 
         device_info = vacuum_bot.device_info
-        self._client.subscribe(_get_subscriptions(device_info))
-        self._subscribers[device_info.did] = vacuum_bot
+        sub_info = self._subscribers.setdefault(
+            device_info.did,
+            SubscriberInfo(
+                bot=vacuum_bot, subscriptions=_get_subscriptions(device_info)
+            ),
+        )
+
+        self._client.subscribe(sub_info.subscriptions)
 
     def unsubscribe(self, vacuum_bot: VacuumBot) -> None:
         """Unsubscribe given vacuum."""
         device_info = vacuum_bot.device_info
 
-        if self._subscribers.pop(device_info.did, None) and self._client:
-            for subscription in _get_subscriptions(device_info):
+        if (info := self._subscribers.pop(device_info.did, None)) and self._client:
+            for subscription in info.subscriptions:
                 self._client.unsubscribe(subscription.topic)
 
     async def disconnect(self) -> None:
         """Disconnect from MQTT."""
         if self._client:
             await self._client.disconnect()
-        self._subscribers.clear()
 
     async def _handle_atr(self, topic_split: list[str], payload: bytes) -> None:
         try:
-            bot = self._subscribers.get(topic_split[3])
-            if bot:
+            sub_info = self._subscribers.get(topic_split[3])
+            if sub_info:
                 data = json.loads(payload)
-                await bot.handle_message(topic_split[2], data)
+                await sub_info.bot.handle_message(topic_split[2], data)
         except Exception:  # pylint: disable=broad-except
             _LOGGER.error(
                 "An exception occurred during handling atr message", exc_info=True
             )
 
     def _handle_p2p(self, topic_split: list[str], payload: bytes) -> None:
         try:
@@ -166,15 +218,23 @@
                     _LOGGER.debug(
                         "Response to command came in probably to late. requestId=%s, commandName=%s",
                         request_id,
                         command_name,
                     )
                     return
 
-                bot = self._subscribers.get(topic_split[3])
-                if bot:
+                sub_info = self._subscribers.get(topic_split[3])
+                if sub_info:
                     data = json.loads(payload)
-                    command.handle_mqtt_p2p(bot.events, data)
+                    command.handle_mqtt_p2p(sub_info.bot.events, data)
         except Exception:  # pylint: disable=broad-except
             _LOGGER.error(
                 "An exception occurred during handling p2p message", exc_info=True
             )
+
+
+@dataclass(frozen=True)
+class SubscriberInfo:
+    """Subscriber information."""
+
+    bot: VacuumBot
+    subscriptions: list[Subscription]
```

### Comparing `deebot-client-1.6.1/deebot_client/util.py` & `deebot-client-2.0.0b1/deebot_client/util.py`

 * *Files identical despite different names*

### Comparing `deebot-client-1.6.1/deebot_client/vacuum_bot.py` & `deebot-client-2.0.0b1/deebot_client/vacuum_bot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 """Vacuum bot module."""
 import asyncio
 import inspect
 import re
 from typing import Any, Final
 
-from .api_client import ApiClient
+from .authentication import Authenticator
 from .command import Command
-from .commands import COMMANDS_WITH_HANDLING, Clean, CommandWithHandling
-from .commands.clean import CleanAction
-from .commands.custom import CustomCommand
+from .commands import COMMANDS_WITH_HANDLING
 from .events import (
     CleanLogEvent,
+    CustomCommandEvent,
     LifeSpanEvent,
     PositionsEvent,
     PositionType,
     StatsEvent,
     StatusEvent,
     TotalStatsEvent,
 )
 from .events.event_bus import EventBus
 from .logging_filter import get_logger
 from .map import Map
-from .message import HandlingState
+from .message import Message
 from .messages import MESSAGES
 from .models import DeviceInfo, VacuumState
 
 _LOGGER = get_logger(__name__)
 
 _COMMAND_REPLACE_PATTERN = "^((on)|(off)|(report))"
 _COMMAND_REPLACE_REPLACEMENT = "get"
@@ -33,18 +32,18 @@
 
 class VacuumBot:
     """Vacuum bot representation."""
 
     def __init__(
         self,
         device_info: DeviceInfo,
-        api_client: ApiClient,
+        authenticator: Authenticator,
     ):
         self.device_info: Final[DeviceInfo] = device_info
-        self._api_client = api_client
+        self._authenticator = authenticator
 
         self._semaphore = asyncio.Semaphore(3)
         self._status: StatusEvent = StatusEvent(device_info.status == 1, None)
 
         self.fw_version: str | None = None
         self.events: Final[EventBus] = EventBus(self.execute_command)
 
@@ -86,49 +85,23 @@
         self.events.subscribe(StatusEvent, on_status)
 
         async def on_stats(_: StatsEvent) -> None:
             self.events.request_refresh(LifeSpanEvent)
 
         self.events.subscribe(StatsEvent, on_stats)
 
-    async def execute_command(self, command: Command | CustomCommand) -> None:
-        """Execute given command and handle response."""
-        if (
-            command == Clean(CleanAction.RESUME)
-            and self._status.state != VacuumState.PAUSED
-        ):
-            command = Clean(CleanAction.START)
-        elif (
-            command == Clean(CleanAction.START)
-            and self._status.state == VacuumState.PAUSED
-        ):
-            command = Clean(CleanAction.RESUME)
+        async def on_custom_command(event: CustomCommandEvent) -> None:
+            await self.handle_message(event.name, event.response)
 
-        async with self._semaphore:
-            response = await self._api_client.send_command(command, self.device_info)
-
-        _LOGGER.debug("Handle command %s: %s", command.name, response)
-        if isinstance(command, (CommandWithHandling, CustomCommand)):
-            result = command.handle_requested(self.events, response)
-            if isinstance(command, CustomCommand):
-                # Custom command can be send for implemented commands too.
-                # We handle the response explicit to fire event if necessary
-                await self.handle_message(command.name, response)
-
-            if result.state == HandlingState.SUCCESS and result.requested_commands:
-                # Execute command which are requested by the handler
-                tasks = []
-                for requested_command in result.requested_commands:
-                    tasks.append(
-                        asyncio.create_task(self.execute_command(requested_command))
-                    )
+        self.events.subscribe(CustomCommandEvent, on_custom_command)
 
-                await asyncio.gather(*tasks)
-        else:
-            _LOGGER.warning("Unsupported command! Command %s", command.name)
+    async def execute_command(self, command: Command) -> None:
+        """Execute given command."""
+        async with self._semaphore:
+            await command.execute(self._authenticator, self.device_info, self.events)
 
     def set_available(self, available: bool) -> None:
         """Set available."""
         status = StatusEvent(available, self._status.state)
         self.events.notify(status)
 
     async def handle_message(
@@ -146,26 +119,31 @@
             self.fw_version = fw_version
 
         message_type = MESSAGES.get(message_name, None)
         if message_type:
             message_type.handle(self.events, message_data)
             return
 
-        _LOGGER.debug("Falling back to old handling way for %s", message_name)
         # Handle message starting with "on","off","report" the same as "get" commands
-        message_name = re.sub(
+        converted_name = re.sub(
             _COMMAND_REPLACE_PATTERN,
             _COMMAND_REPLACE_REPLACEMENT,
             message_name,
         )
 
         # T8 series and newer
-        if message_name.endswith("_V2"):
-            message_name = message_name[:-3]
+        if converted_name.endswith("_V2"):
+            converted_name = converted_name[:-3]
 
         found_command = MESSAGES.get(
-            message_name, COMMANDS_WITH_HANDLING.get(message_name, None)
+            converted_name, COMMANDS_WITH_HANDLING.get(converted_name, None)
         )
         if found_command:
-            found_command.handle(self.events, message_data)
+            if issubclass(found_command, Message):
+                _LOGGER.debug("Falling back to old handling way for %s", message_name)
+                found_command.handle(self.events, message_data)
+            else:
+                _LOGGER.debug(
+                    'Command "%s" doesn\'t support message handling', converted_name
+                )
         else:
             _LOGGER.debug('Unknown message "%s" with %s', message_name, message_data)
```

### Comparing `deebot-client-1.6.1/deebot_client.egg-info/PKG-INFO` & `deebot-client-2.0.0b1/deebot_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deebot-client
-Version: 1.6.1
+Version: 2.0.0b1
 Summary: a library for controlling certain deebot vacuums
 Home-page: https://github.com/DeebotUniverse/client.py
 Author: DeebotUniverse
 Author-email: deebotuniverse@knatschig-as-hell.info
 License: GPL-3.0
 Keywords: home automation vacuum robot deebot ecovacs
 Classifier: Development Status :: 4 - Beta
@@ -37,20 +37,21 @@
 
 ```python
 import aiohttp
 import asyncio
 import logging
 import time
 
-from deebot_client import create_instances
+from deebot_client.api_client import ApiClient
+from deebot_client.authentication import Authenticator
 from deebot_client.commands import *
 from deebot_client.commands.clean import CleanAction
-from deebot_client.models import Configuration
-from deebot_client.mqtt_client import MqttClient
 from deebot_client.events import BatteryEvent
+from deebot_client.models import Configuration
+from deebot_client.mqtt_client import MqttClient, MqttConfiguration
 from deebot_client.util import md5
 from deebot_client.vacuum_bot import VacuumBot
 
 device_id = md5(str(time.time()))
 account_id = "your email or phonenumber (cn)"
 password_hash = md5("yourPassword")
 continent = "eu"
@@ -60,22 +61,24 @@
 async def main():
   async with aiohttp.ClientSession() as session:
     logging.basicConfig(level=logging.DEBUG)
     config = Configuration(session,
                            device_id=device_id, country=country, continent=continent,
                            )
 
-    (authenticator, api_client) = create_instances(config, account_id, password_hash)
+    authenticator = Authenticator(config, account_id, password_hash)
+    api_client = ApiClient(authenticator)
 
     devices_ = await api_client.get_devices()
 
-    bot = VacuumBot(devices_[0], api_client)
+    bot = VacuumBot(devices_[0], authenticator)
 
-    mqtt = MqttClient(config, authenticator)
-    await mqtt.initialize()
+    mqtt_config = MqttConfiguration(config=config)
+    mqtt = MqttClient(mqtt_config, authenticator)
+    await mqtt.connect()
     await mqtt.subscribe(bot)
 
     async def on_battery(event: BatteryEvent):
       # Do stuff on battery event
       if event.value == 100:
         # Battery full
         pass
```

### Comparing `deebot-client-1.6.1/deebot_client.egg-info/SOURCES.txt` & `deebot-client-2.0.0b1/deebot_client.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 deebot_client/__init__.py
-deebot_client/_api_client.py
 deebot_client/api_client.py
 deebot_client/authentication.py
 deebot_client/command.py
 deebot_client/const.py
 deebot_client/exceptions.py
 deebot_client/logging_filter.py
 deebot_client/map.py
@@ -65,17 +64,21 @@
 tests/commands/test_charge.py
 tests/commands/test_charge_state.py
 tests/commands/test_clean.py
 tests/commands/test_clean_count.py
 tests/commands/test_clean_log.py
 tests/commands/test_clean_preference.py
 tests/commands/test_continuous_cleaning.py
+tests/commands/test_custom.py
 tests/commands/test_fan_speed.py
+tests/commands/test_life_span.py
 tests/commands/test_map.py
 tests/commands/test_mulitmap_state.py
 tests/commands/test_true_detect.py
+tests/commands/test_water_info.py
 tests/events/__init__.py
 tests/events/test_events.py
 tests/events/test_water_info.py
 tests/messages/__init__.py
 tests/messages/test_battery.py
+tests/messages/test_messages.py
 tests/messages/test_stats.py
```

### Comparing `deebot-client-1.6.1/setup.py` & `deebot-client-2.0.0b1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = file.read()
 
 with open("requirements.txt", encoding="utf-8") as file:
     install_requires = list(val.strip() for val in file)
 
 setup(
     name="deebot-client",
-    version="1.6.1",
+    version="2.0.0b1",
     url="https://github.com/DeebotUniverse/client.py",
     description="a library for controlling certain deebot vacuums",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DeebotUniverse",
     author_email="deebotuniverse@knatschig-as-hell.info",
     license="GPL-3.0",
```

### Comparing `deebot-client-1.6.1/tests/commands/test_advanced_mode.py` & `deebot-client-2.0.0b1/tests/commands/test_advanced_mode.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import pytest
 
 from deebot_client.commands import GetAdvancedMode, SetAdvancedMode
 from deebot_client.events import AdvancedModeEvent
-from tests.commands import assert_command_requested, assert_set_command
+from tests.commands import assert_command, assert_set_command
 from tests.helpers import get_request_json
 
 
 @pytest.mark.parametrize("value", [False, True])
-def test_get_advanced_mode_requested(value: bool) -> None:
+async def test_GetAdvancedMode(value: bool) -> None:
     json = get_request_json({"enable": 1 if value else 0})
-    assert_command_requested(GetAdvancedMode(), json, AdvancedModeEvent(value))
+    await assert_command(GetAdvancedMode(), json, AdvancedModeEvent(value))
 
 
 @pytest.mark.parametrize("value", [False, True])
-def test_set_advanced_mode(value: bool) -> None:
+async def test_SetAdvancedMode(value: bool) -> None:
     args = {"enable": 1 if value else 0}
-    assert_set_command(SetAdvancedMode(value), args, AdvancedModeEvent(value))
+    await assert_set_command(SetAdvancedMode(value), args, AdvancedModeEvent(value))
```

### Comparing `deebot-client-1.6.1/tests/commands/test_carpet.py` & `deebot-client-2.0.0b1/tests/commands/test_carpet.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import pytest
 
 from deebot_client.commands import GetCarpetAutoFanBoost, SetCarpetAutoFanBoost
 from deebot_client.events import CarpetAutoFanBoostEvent
-from tests.commands import assert_command_requested, assert_set_command
+from tests.commands import assert_command, assert_set_command
 from tests.helpers import get_request_json
 
 
 @pytest.mark.parametrize("value", [False, True])
-def test_get_carpet_auto_fan_boost_requested(value: bool) -> None:
+async def test_GetCarpetAutoFanBoost(value: bool) -> None:
     json = get_request_json({"enable": 1 if value else 0})
-    assert_command_requested(
-        GetCarpetAutoFanBoost(), json, CarpetAutoFanBoostEvent(value)
-    )
+    await assert_command(GetCarpetAutoFanBoost(), json, CarpetAutoFanBoostEvent(value))
 
 
 @pytest.mark.parametrize("value", [False, True])
-def test_set_carpet_auto_fan_boost(value: bool) -> None:
+async def test_SetCarpetAutoFanBoost(value: bool) -> None:
     args = {"enable": 1 if value else 0}
-    assert_set_command(
+    await assert_set_command(
         SetCarpetAutoFanBoost(value), args, CarpetAutoFanBoostEvent(value)
     )
```

### Comparing `deebot-client-1.6.1/tests/commands/test_charge.py` & `deebot-client-2.0.0b1/tests/commands/test_clean.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from typing import Any
 
 import pytest
 
-from deebot_client.commands import Charge
+from deebot_client.commands import GetCleanInfo
 from deebot_client.events import StatusEvent
 from deebot_client.models import VacuumState
-from tests.commands import assert_command_requested
+from tests.commands import assert_command
 from tests.helpers import get_request_json
 
 
-def prepare_json_docked_test() -> dict[str, Any]:
-    json = get_request_json(None)
-    json["resp"]["body"]["code"] = 30007
-    return json
-
-
 @pytest.mark.parametrize(
     "json, expected",
     [
-        (get_request_json(None), StatusEvent(True, VacuumState.RETURNING)),
-        (prepare_json_docked_test(), StatusEvent(True, VacuumState.DOCKED)),
+        (
+            get_request_json({"trigger": "none", "state": "idle"}),
+            StatusEvent(True, VacuumState.IDLE),
+        ),
     ],
 )
-def test_charge(json: dict[str, Any], expected: StatusEvent) -> None:
-    assert_command_requested(Charge(), json, expected)
+async def test_GetCleanInfo(json: dict[str, Any], expected: StatusEvent) -> None:
+    await assert_command(GetCleanInfo(), json, expected)
```

### Comparing `deebot-client-1.6.1/tests/commands/test_clean_count.py` & `deebot-client-2.0.0b1/tests/commands/test_clean_count.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import pytest
 
 from deebot_client.commands import GetCleanCount, SetCleanCount
 from deebot_client.events import CleanCountEvent
-from tests.commands import assert_command_requested, assert_set_command
+from tests.commands import assert_command, assert_set_command
 from tests.helpers import get_request_json
 
 
-def test_GetFanSpeed_requested() -> None:
+async def test_GetCleanCount() -> None:
     json = get_request_json({"count": 2})
-    assert_command_requested(GetCleanCount(), json, CleanCountEvent(2))
+    await assert_command(GetCleanCount(), json, CleanCountEvent(2))
 
 
 @pytest.mark.parametrize("count", [1, 2, 3])
-def test_set_multimap_state(count: int) -> None:
+async def test_SetCleanCount(count: int) -> None:
     args = {"count": count}
-    assert_set_command(SetCleanCount(count), args, CleanCountEvent(count))
+    await assert_set_command(SetCleanCount(count), args, CleanCountEvent(count))
```

### Comparing `deebot-client-1.6.1/tests/commands/test_clean_log.py` & `deebot-client-2.0.0b1/tests/commands/test_clean_log.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 from typing import Any
-from unittest.mock import Mock
 
 import pytest
 from testfixtures import LogCapture
 
 from deebot_client.commands import GetCleanLogs
-from deebot_client.commands.common import CommandResult
 from deebot_client.events import CleanJobStatus, CleanLogEntry, CleanLogEvent
-from deebot_client.events.event_bus import EventBus
-from deebot_client.message import HandlingState
-from tests.commands import assert_command_requested
+from tests.commands import assert_command
 
 
-def test_GetCleanLogs() -> None:
+async def test_GetCleanLogs() -> None:
     json = {
         "ret": "ok",
         "logs": [
             {
                 "ts": 1656265100,
                 "last": 139,
                 "area": 2,
@@ -105,51 +101,52 @@
                 stop_reason=CleanJobStatus.FINISHED_WITH_WARNINGS,
                 duration=73,
             ),
         ]
     )
 
     with LogCapture() as log:
-        assert_command_requested(GetCleanLogs(), json, expected)
+        await assert_command(GetCleanLogs(), json, expected)
 
         log.check_present(
             (
                 "deebot_client.commands.clean_logs",
                 "WARNING",
                 "Skipping log entry: {'ts': 1655564616, 'invalid': 'event'}",
             )
         )
 
 
 @pytest.mark.parametrize(
     "json",
     [{"ret": "ok"}, {"ret": "fail"}],
 )
-def test_GetCleanLogs_analyse_logged(json: dict[str, Any]) -> None:
+async def test_GetCleanLogs_analyse_logged(json: dict[str, Any]) -> None:
     with LogCapture() as log:
-        assert_command_requested(
+        await assert_command(
             GetCleanLogs(),
             json,
             None,
-            CommandResult(HandlingState.ANALYSE_LOGGED),
         )
         log.check_present(
             (
-                "deebot_client.commands.common",
+                "deebot_client.command",
                 "DEBUG",
-                f"Could not handle command: GetCleanLogs with {json}",
+                f"ANALYSE: Could not handle command: GetCleanLogs with {json}",
             )
         )
 
 
-def test_GetCleanLogs_handle_fails() -> None:
+async def test_GetCleanLogs_handle_fails() -> None:
     with LogCapture() as log:
-        result = GetCleanLogs.handle(Mock(spec_set=EventBus), {})
-
-        assert result.state == HandlingState.ERROR
+        await assert_command(
+            GetCleanLogs(),
+            {},
+            None,
+        )
         log.check_present(
             (
-                "deebot_client.message",
+                "deebot_client.command",
                 "WARNING",
-                f"Could not parse {GetCleanLogs.name}: {{}}",
+                f"Could not parse response for {GetCleanLogs.name}: {{}}",
             )
         )
```

### Comparing `deebot-client-1.6.1/tests/commands/test_clean_preference.py` & `deebot-client-2.0.0b1/tests/commands/test_clean_preference.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import pytest
 
 from deebot_client.commands import GetCleanPreference, SetCleanPreference
 from deebot_client.events import CleanPreferenceEvent
-from tests.commands import assert_command_requested, assert_set_command
+from tests.commands import assert_command, assert_set_command
 from tests.helpers import get_request_json
 
 
 @pytest.mark.parametrize("value", [False, True])
-def test_get_clean_preference(value: bool) -> None:
+async def test_GetCleanPreference(value: bool) -> None:
     json = get_request_json({"enable": 1 if value else 0})
-    assert_command_requested(GetCleanPreference(), json, CleanPreferenceEvent(value))
+    await assert_command(GetCleanPreference(), json, CleanPreferenceEvent(value))
 
 
 @pytest.mark.parametrize("value", [False, True])
-def test_set_clean_preference(value: bool) -> None:
+async def test_SetCleanPreference(value: bool) -> None:
     args = {"enable": 1 if value else 0}
-    assert_set_command(SetCleanPreference(value), args, CleanPreferenceEvent(value))
+    await assert_set_command(
+        SetCleanPreference(value), args, CleanPreferenceEvent(value)
+    )
```

### Comparing `deebot-client-1.6.1/tests/commands/test_continuous_cleaning.py` & `deebot-client-2.0.0b1/tests/commands/test_continuous_cleaning.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import pytest
 
 from deebot_client.commands import GetContinuousCleaning, SetContinuousCleaning
 from deebot_client.events import ContinuousCleaningEvent
-from tests.commands import assert_command_requested, assert_set_command
+from tests.commands import assert_command, assert_set_command
 from tests.helpers import get_request_json
 
 
 @pytest.mark.parametrize("value", [False, True])
-def test_get_continuous_cleaning_requested(value: bool) -> None:
+async def test_GetContinuousCleaning(value: bool) -> None:
     json = get_request_json({"enable": 1 if value else 0})
-    assert_command_requested(
-        GetContinuousCleaning(), json, ContinuousCleaningEvent(value)
-    )
+    await assert_command(GetContinuousCleaning(), json, ContinuousCleaningEvent(value))
 
 
 @pytest.mark.parametrize("value", [False, True])
-def test_set_continuous_cleaning(value: bool) -> None:
+async def test_SetContinuousCleaning(value: bool) -> None:
     args = {"enable": 1 if value else 0}
-    assert_set_command(
+    await assert_set_command(
         SetContinuousCleaning(value), args, ContinuousCleaningEvent(value)
     )
```

### Comparing `deebot-client-1.6.1/tests/commands/test_fan_speed.py` & `deebot-client-2.0.0b1/tests/commands/test_fan_speed.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import pytest
 
 from deebot_client.commands import FanSpeedLevel, GetFanSpeed, SetFanSpeed
 from deebot_client.events import FanSpeedEvent
-from tests.commands import assert_command_requested
+from tests.commands import assert_command
 from tests.helpers import get_request_json, verify_DisplayNameEnum_unique
 
 
 def test_FanSpeedLevel_unique() -> None:
     verify_DisplayNameEnum_unique(FanSpeedLevel)
 
 
-def test_GetFanSpeed_requested() -> None:
+async def test_GetFanSpeed() -> None:
     json = get_request_json({"speed": 2})
-    assert_command_requested(GetFanSpeed(), json, FanSpeedEvent("max+"))
+    await assert_command(GetFanSpeed(), json, FanSpeedEvent("max+"))
 
 
 @pytest.mark.parametrize(
     "value, expected", [("quiet", 1000), ("max+", 2), (0, 0), (FanSpeedLevel.MAX, 1)]
 )
 def test_SetFanSpeed(value: str | int | FanSpeedLevel, expected: int) -> None:
     command = SetFanSpeed(value)
     assert command.name == "setSpeed"
-    assert command.args == {"speed": expected}
+    assert command._args == {"speed": expected}
```

### Comparing `deebot-client-1.6.1/tests/commands/test_map.py` & `deebot-client-2.0.0b1/tests/commands/test_map.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from deebot_client.commands import (
     GetCachedMapInfo,
     GetMajorMap,
     GetMapSet,
     GetMapSubSet,
     GetMapTrace,
 )
-from deebot_client.commands.common import CommandResult
 from deebot_client.events import (
     MajorMapEvent,
     MapSetEvent,
     MapSetType,
     MapSubsetEvent,
     MapTraceEvent,
 )
-from deebot_client.message import HandlingState
-from tests.commands import assert_command_requested
+from deebot_client.events.map import CachedMapInfoEvent
+from tests.commands import assert_command
 from tests.helpers import get_request_json
 
 
-def test_getMapSubSet_requested_customName() -> None:
+async def test_getMapSubSet_customName() -> None:
     type = MapSetType.ROOMS
     value = "XQAABAB5AgAAABaOQok5MfkIKbGTBxaUTX13SjXBAI1/Q3A9Kkx2gYZ1QdgwfwOSlU3hbRjNJYgr2Pr3WgFez3Gcoj3R2JmzAuc436F885ZKt5NF2AE1UPAF4qq67tK6TSA64PPfmZQ0lqwInQmqKG5/KO59RyFBbV1NKnDIGNBGVCWpH62WLlMu8N4zotA8dYMQ/UBMwr/gddQO5HU01OQM2YvF"
     name = "Levin"
     json = get_request_json(
         {
             "type": type.value,
             "subtype": "15",
@@ -38,100 +37,102 @@
             "compress": 1,
             "center": "-6775,-9225",
             "mssid": "8",
             "value": value,
             "mid": "98100521",
         }
     )
-    assert_command_requested(
+    await assert_command(
         GetMapSubSet(mid="98100521", mssid="8", msid="1"),
         json,
         MapSubsetEvent(8, type, value, name),
     )
 
 
-def test_getMapSubSet_requested_living_room() -> None:
+async def test_getMapSubSet_living_room() -> None:
     type = MapSetType.ROOMS
     value = "-1400,-1600;-1400,-1350;-950,-1100;-900,-150;-550,100;200,950;500,950;650,800;800,950;1850,950;1950,800;1950,-200;2050,-300;2300,-300;2550,-650;2700,-650;2700,-1600;2400,-1750;2700,-1900;2700,-2950;2450,-2950;2300,-3100;2400,-3200;2650,-3200;2700,-3500;2300,-3500;2200,-3250;2050,-3550;1200,-3550;1200,-3300;1050,-3200;950,-3300;950,-3550;600,-3550;550,-2850;850,-2800;950,-2700;850,-2600;950,-2400;900,-2350;800,-2300;550,-2500;550,-2350;400,-2250;200,-2650;-800,-2650;-950,-2550;-950,-2150;-650,-2000;-450,-2000;-400,-1950;-450,-1850;-750,-1800;-950,-1900;-1350,-1900;-1400,-1600"
     json = get_request_json(
         {
             "type": type.value,
             "mssid": "7",
             "value": value,
             "subtype": "1",
             "connections": "12",
             "mid": "199390082",
         }
     )
-    assert_command_requested(
+    await assert_command(
         GetMapSubSet(mid="199390082", mssid="7", msid="1"),
         json,
         MapSubsetEvent(7, type, value, "Living Room"),
     )
 
 
-def test_getCachedMapInfo_requested() -> None:
+async def test_getCachedMapInfo() -> None:
     expected_mid = "199390082"
+    expected_name = "Erdgeschoss"
     json = get_request_json(
         {
             "enable": 1,
             "info": [
                 {
                     "mid": expected_mid,
                     "index": 0,
                     "status": 1,
                     "using": 1,
                     "built": 1,
-                    "name": "Erdgeschoss",
+                    "name": expected_name,
                 },
                 {
                     "mid": "722607162",
                     "index": 3,
                     "status": 0,
                     "using": 0,
                     "built": 0,
                     "name": "",
                 },
             ],
         }
     )
-    assert_command_requested(
+    await assert_command(
         GetCachedMapInfo(),
         json,
-        None,
-        CommandResult(
-            HandlingState.SUCCESS,
-            {"map_id": expected_mid},
-            [GetMapSet(expected_mid, entry) for entry in MapSetType],
-        ),
+        CachedMapInfoEvent(expected_name, True),
+        # todo check requested command be called
+        # CommandResult(
+        #    HandlingState.SUCCESS,
+        #    {"map_id": expected_mid},
+        #    [GetMapSet(expected_mid, entry) for entry in MapSetType],
+        # ),
     )
 
 
-def test_getMajorMap_requested() -> None:
+async def test_getMajorMap() -> None:
     expected_mid = "199390082"
     value = "1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,3378526980,2963288214,2739565817,729228561,2452519304,1295764014,1295764014,1295764014,2753376360,329080101,952462272,3648890579,412193448,1540631558,1295764014,1295764014,1561391782,1081327924,1096350476,2860639280,37066625,86907282,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014,1295764014"
     json = get_request_json(
         {
             "mid": expected_mid,
             "pieceWidth": 100,
             "pieceHeight": 100,
             "cellWidth": 8,
             "cellHeight": 8,
             "pixel": 50,
             "value": value,
         }
     )
-    assert_command_requested(
+    await assert_command(
         GetMajorMap(), json, MajorMapEvent(True, expected_mid, value.split(","))
     )
 
 
-def test_getMapSet_requested() -> None:
+async def test_getMapSet() -> None:
     mid = "199390082"
-    msid = "8"
+    # msid = "8"
     json = get_request_json(
         {
             "type": "ar",
             "count": 7,
             "mid": mid,
             "msid": "8",
             "subsets": [
@@ -142,43 +143,45 @@
                 {"mssid": "10"},
                 {"mssid": "11"},
                 {"mssid": "13"},
             ],
         }
     )
     subsets = [7, 12, 17, 14, 10, 11, 13]
-    assert_command_requested(
+    await assert_command(
         GetMapSet(mid),
         json,
         MapSetEvent(MapSetType.ROOMS, subsets),
-        CommandResult(
-            HandlingState.SUCCESS,
-            {"id": "199390082", "set_id": "8", "type": "ar", "subsets": subsets},
-            [
-                GetMapSubSet(mid=mid, msid=msid, type=MapSetType.ROOMS, mssid=s)
-                for s in subsets
-            ],
-        ),
+        # todo check requested command be called
+        # CommandResult(
+        #    HandlingState.SUCCESS,
+        #    {"id": "199390082", "set_id": "8", "type": "ar", "subsets": subsets},
+        #    [
+        #        GetMapSubSet(mid=mid, msid=msid, type=MapSetType.ROOMS, mssid=s)
+        #        for s in subsets
+        #    ],
+        # ),
     )
 
 
-def test_getMapTrace_requested() -> None:
+async def test_getMapTrace() -> None:
     start = 0
-    total = 2545
+    total = 160
     trace_value = "REMOVED"
     json = get_request_json(
         {
             "tid": "173207",
-            "totalCount": 2545,
+            "totalCount": total,
             "traceStart": start,
             "pointCount": 200,
             "traceValue": trace_value,
         }
     )
-    assert_command_requested(
+    await assert_command(
         GetMapTrace(start),
         json,
         MapTraceEvent(start=start, total=total, data=trace_value),
-        CommandResult(
-            HandlingState.SUCCESS, {"start": start, "total": total}, [GetMapTrace(200)]
-        ),
+        # todo check requested command be called
+        # CommandResult(
+        #    HandlingState.SUCCESS, {"start": start, "total": total}, [GetMapTrace(200)]
+        # ),
     )
```

### Comparing `deebot-client-1.6.1/tests/commands/test_true_detect.py` & `deebot-client-2.0.0b1/tests/commands/test_true_detect.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import pytest
 
 from deebot_client.commands import GetTrueDetect, SetTrueDetect
 from deebot_client.events import TrueDetectEvent
-from tests.commands import assert_command_requested, assert_set_command
+from tests.commands import assert_command, assert_set_command
 from tests.helpers import get_request_json
 
 
 @pytest.mark.parametrize("value", [False, True])
-def test_get_true_detect(value: bool) -> None:
+async def test_GetTrueDetect(value: bool) -> None:
     json = get_request_json({"enable": 1 if value else 0})
-    assert_command_requested(GetTrueDetect(), json, TrueDetectEvent(value))
+    await assert_command(GetTrueDetect(), json, TrueDetectEvent(value))
 
 
 @pytest.mark.parametrize("value", [False, True])
-def test_set_true_detect(value: bool) -> None:
+async def test_SetTrueDetect(value: bool) -> None:
     args = {"enable": 1 if value else 0}
-    assert_set_command(SetTrueDetect(value), args, TrueDetectEvent(value))
+    await assert_set_command(SetTrueDetect(value), args, TrueDetectEvent(value))
```

### Comparing `deebot-client-1.6.1/tests/messages/test_battery.py` & `deebot-client-2.0.0b1/tests/messages/test_battery.py`

 * *Files identical despite different names*

### Comparing `deebot-client-1.6.1/tests/messages/test_stats.py` & `deebot-client-2.0.0b1/tests/messages/test_stats.py`

 * *Files identical despite different names*

