# Comparing `tmp/hahomematic-2023.3.1.tar.gz` & `tmp/hahomematic-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hahomematic-2023.3.1.tar", last modified: Fri Mar 31 14:13:47 2023, max compression
+gzip compressed data, was "hahomematic-2023.4.0.tar", last modified: Sun Apr 16 10:20:03 2023, max compression
```

## Comparing `hahomematic-2023.3.1.tar` & `hahomematic-2023.4.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:13:47.268717 hahomematic-2023.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-03-31 14:13:47.268717 hahomematic-2023.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:13:47.264717 hahomematic-2023.3.1/hahomematic/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/backport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:13:47.264717 hahomematic-2023.3.1/hahomematic/caches/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/caches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/caches/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)    17167 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/caches/persistent.py
--rw-r--r--   0 runner    (1001) docker     (123)    24311 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/caches/visibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    49362 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/central_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    44779 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/hmcli.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/json_rpc_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:13:47.264717 hahomematic-2023.3.1/hahomematic/platforms/
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:13:47.268717 hahomematic-2023.3.1/hahomematic/platforms/custom/
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/custom/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/custom/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    23725 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/custom/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)    26740 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/custom/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    11295 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/custom/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/custom/light.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/custom/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/custom/siren.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/custom/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/custom/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    19910 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:13:47.268717 hahomematic-2023.3.1/hahomematic/platforms/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/generic/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/generic/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/generic/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/generic/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/generic/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/generic/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/generic/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/generic/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:13:47.268717 hahomematic-2023.3.1/hahomematic/platforms/hub/
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/hub/binary_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/hub/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/hub/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/hub/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/hub/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/hub/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/hub/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/hub/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/platforms/support.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:13:47.268717 hahomematic-2023.3.1/hahomematic/rega_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/rega_scripts/fetch_all_device_data.fn
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/rega_scripts/get_serial.fn
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/rega_scripts/set_system_variable.fn
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/xml_rpc_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/hahomematic/xml_rpc_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:13:47.264717 hahomematic-2023.3.1/hahomematic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-03-31 14:13:46.000000 hahomematic-2023.3.1/hahomematic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-03-31 14:13:47.000000 hahomematic-2023.3.1/hahomematic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 14:13:46.000000 hahomematic-2023.3.1/hahomematic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 14:13:44.000000 hahomematic-2023.3.1/hahomematic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-31 14:13:47.000000 hahomematic-2023.3.1/hahomematic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-31 14:13:47.000000 hahomematic-2023.3.1/hahomematic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-03-31 14:13:18.000000 hahomematic-2023.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-31 14:13:47.268717 hahomematic-2023.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:20:03.102901 hahomematic-2023.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-16 10:20:03.102901 hahomematic-2023.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:20:03.094901 hahomematic-2023.4.0/hahomematic/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/backport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:20:03.094901 hahomematic-2023.4.0/hahomematic/caches/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/caches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/caches/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17167 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/caches/persistent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24311 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/caches/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49209 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/central_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44779 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/hmcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/json_rpc_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:20:03.094901 hahomematic-2023.4.0/hahomematic/platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:20:03.098901 hahomematic-2023.4.0/hahomematic/platforms/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24881 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26740 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11295 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27456 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/siren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/custom/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19910 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:20:03.098901 hahomematic-2023.4.0/hahomematic/platforms/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/generic/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/generic/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/generic/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/generic/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/generic/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/generic/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/generic/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/generic/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:20:03.102901 hahomematic-2023.4.0/hahomematic/platforms/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/hub/binary_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/hub/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/hub/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/hub/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/hub/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/hub/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/hub/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/hub/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/platforms/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:20:03.102901 hahomematic-2023.4.0/hahomematic/rega_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/rega_scripts/fetch_all_device_data.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/rega_scripts/get_serial.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/rega_scripts/get_system_variables_ext_marker.fn
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/rega_scripts/set_system_variable.fn
+-rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/xml_rpc_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/hahomematic/xml_rpc_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 10:20:03.094901 hahomematic-2023.4.0/hahomematic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-16 10:20:02.000000 hahomematic-2023.4.0/hahomematic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-16 10:20:03.000000 hahomematic-2023.4.0/hahomematic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 10:20:02.000000 hahomematic-2023.4.0/hahomematic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 10:20:01.000000 hahomematic-2023.4.0/hahomematic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-16 10:20:02.000000 hahomematic-2023.4.0/hahomematic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 10:20:02.000000 hahomematic-2023.4.0/hahomematic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-04-16 10:19:23.000000 hahomematic-2023.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-16 10:20:03.102901 hahomematic-2023.4.0/setup.cfg
```

### Comparing `hahomematic-2023.3.1/LICENSE` & `hahomematic-2023.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/PKG-INFO` & `hahomematic-2023.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.3.1
+Version: 2023.4.0
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.3.1/README.md` & `hahomematic-2023.4.0/README.md`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/__init__.py` & `hahomematic-2023.4.0/hahomematic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/backport.py` & `hahomematic-2023.4.0/hahomematic/backport.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/caches/dynamic.py` & `hahomematic-2023.4.0/hahomematic/caches/dynamic.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/caches/persistent.py` & `hahomematic-2023.4.0/hahomematic/caches/persistent.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/caches/visibility.py` & `hahomematic-2023.4.0/hahomematic/caches/visibility.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/central_unit.py` & `hahomematic-2023.4.0/hahomematic/central_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1145,17 +1145,15 @@
         if not self.username:
             _LOGGER.warning("CHECK_CONFIG: Username must not be empty")
             return False
         if self.password is None:
             _LOGGER.warning("CHECK_CONFIG: Password is required")  # type: ignore[unreachable]
             return False
         if not check_password(self.password):
-            _LOGGER.warning("CHECK_CONFIG: password contains not allowed characters")
-            # Here we only log a warning to get some feedback
-            # no return False
+            return False
 
         try:
             check_or_create_directory(self.storage_folder)
         except BaseHomematicException:
             _LOGGER.warning("CHECK_CONFIG: directory % cannot be created", self.storage_folder)
             return False
         return True
```

### Comparing `hahomematic-2023.3.1/hahomematic/client.py` & `hahomematic-2023.4.0/hahomematic/client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/const.py` & `hahomematic-2023.4.0/hahomematic/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/decorators.py` & `hahomematic-2023.4.0/hahomematic/decorators.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/exceptions.py` & `hahomematic-2023.4.0/hahomematic/exceptions.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/exporter.py` & `hahomematic-2023.4.0/hahomematic/exporter.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/hmcli.py` & `hahomematic-2023.4.0/hahomematic/hmcli.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/json_rpc_client.py` & `hahomematic-2023.4.0/hahomematic/json_rpc_client.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/__init__.py` & `hahomematic-2023.4.0/hahomematic/platforms/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/custom/__init__.py` & `hahomematic-2023.4.0/hahomematic/platforms/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/custom/climate.py` & `hahomematic-2023.4.0/hahomematic/platforms/custom/climate.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/custom/const.py` & `hahomematic-2023.4.0/hahomematic/platforms/custom/const.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/custom/cover.py` & `hahomematic-2023.4.0/hahomematic/platforms/custom/cover.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,17 +327,17 @@
     ) -> str | None:
         """Return the combined parameter."""
         if level is None and tilt_level is None:
             return None
         levels: list[str] = []
         # the resulting hex value is based on the doubled position
         if level is not None:
-            levels.append(str(hex(int(level * 100 * 2))))
+            levels.append(format(int(level * 100 * 2), "#04x"))
         if tilt_level is not None:
-            levels.append(str(hex(int(tilt_level * 100 * 2))))
+            levels.append(format(int(tilt_level * 100 * 2), "#04x"))
 
         if levels:
             return ",".join(levels)
         return None
 
 
 class CeIpBlind(CeBlind):
```

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/custom/definition.py` & `hahomematic-2023.4.0/hahomematic/platforms/custom/definition.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/custom/entity.py` & `hahomematic-2023.4.0/hahomematic/platforms/custom/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/custom/light.py` & `hahomematic-2023.4.0/hahomematic/platforms/custom/light.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/custom/lock.py` & `hahomematic-2023.4.0/hahomematic/platforms/custom/lock.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/custom/siren.py` & `hahomematic-2023.4.0/hahomematic/platforms/custom/siren.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/custom/support.py` & `hahomematic-2023.4.0/hahomematic/platforms/custom/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/custom/switch.py` & `hahomematic-2023.4.0/hahomematic/platforms/custom/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/device.py` & `hahomematic-2023.4.0/hahomematic/platforms/device.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/entity.py` & `hahomematic-2023.4.0/hahomematic/platforms/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/event.py` & `hahomematic-2023.4.0/hahomematic/platforms/event.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/generic/__init__.py` & `hahomematic-2023.4.0/hahomematic/platforms/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/generic/action.py` & `hahomematic-2023.4.0/hahomematic/platforms/generic/action.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/generic/binary_sensor.py` & `hahomematic-2023.4.0/hahomematic/platforms/generic/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/generic/button.py` & `hahomematic-2023.4.0/hahomematic/platforms/generic/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/generic/entity.py` & `hahomematic-2023.4.0/hahomematic/platforms/generic/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/generic/number.py` & `hahomematic-2023.4.0/hahomematic/platforms/generic/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/generic/select.py` & `hahomematic-2023.4.0/hahomematic/platforms/generic/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/generic/sensor.py` & `hahomematic-2023.4.0/hahomematic/platforms/generic/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/generic/switch.py` & `hahomematic-2023.4.0/hahomematic/platforms/generic/switch.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/hub/__init__.py` & `hahomematic-2023.4.0/hahomematic/platforms/hub/__init__.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/hub/binary_sensor.py` & `hahomematic-2023.4.0/hahomematic/platforms/hub/binary_sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/hub/button.py` & `hahomematic-2023.4.0/hahomematic/platforms/hub/button.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/hub/entity.py` & `hahomematic-2023.4.0/hahomematic/platforms/hub/entity.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/hub/number.py` & `hahomematic-2023.4.0/hahomematic/platforms/hub/number.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/hub/select.py` & `hahomematic-2023.4.0/hahomematic/platforms/hub/select.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/hub/sensor.py` & `hahomematic-2023.4.0/hahomematic/platforms/hub/sensor.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/hub/text.py` & `hahomematic-2023.4.0/hahomematic/platforms/hub/text.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/platforms/support.py` & `hahomematic-2023.4.0/hahomematic/platforms/support.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/rega_scripts/fetch_all_device_data.fn` & `hahomematic-2023.4.0/hahomematic/rega_scripts/fetch_all_device_data.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/rega_scripts/get_serial.fn` & `hahomematic-2023.4.0/hahomematic/rega_scripts/get_serial.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/rega_scripts/get_system_variables_ext_marker.fn` & `hahomematic-2023.4.0/hahomematic/rega_scripts/get_system_variables_ext_marker.fn`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/support.py` & `hahomematic-2023.4.0/hahomematic/support.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,22 @@
     return lower_value in ["y", "yes", "t", "true", "on", "1"]
 
 
 def check_password(password: str | None) -> bool:
     """Check password."""
     if password is None:
         return False
-    return re.fullmatch(CCU_PASSWORD_PATTERN, password) is not None
+    if re.fullmatch(CCU_PASSWORD_PATTERN, password) is None:
+        _LOGGER.warning(
+            "CHECK_CONFIG: password contains not allowed characters. "
+            "Use only allowed characters. See password regex: %s",
+            CCU_PASSWORD_PATTERN,
+        )
+        return False
+    return True
 
 
 def get_tls_context(verify_tls: bool) -> ssl.SSLContext:
     """Return tls verified/unverified ssl/tls context."""
     if verify_tls:
         ssl_context = ssl.create_default_context()
     else:
```

### Comparing `hahomematic-2023.3.1/hahomematic/xml_rpc_proxy.py` & `hahomematic-2023.4.0/hahomematic/xml_rpc_proxy.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic/xml_rpc_server.py` & `hahomematic-2023.4.0/hahomematic/xml_rpc_server.py`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/hahomematic.egg-info/PKG-INFO` & `hahomematic-2023.4.0/hahomematic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hahomematic
-Version: 2023.3.1
+Version: 2023.4.0
 Summary: Homematic interface for Home Assistant running on Python 3.
 Home-page: https://github.com/danielperna84/hahomematic
 Author-email: Daniel Perna <danielperna84@gmail.com>, SukramJ <sukramj@icloud.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/danielperna84/hahomematic
 Project-URL: Bug Reports, https://github.com/danielperna84/hahomematic/issues
 Project-URL: Docs: Dev, https://github.com/danielperna84/hahomematic
```

### Comparing `hahomematic-2023.3.1/hahomematic.egg-info/SOURCES.txt` & `hahomematic-2023.4.0/hahomematic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hahomematic-2023.3.1/pyproject.toml` & `hahomematic-2023.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "hahomematic"
-version     = "2023.3.1"
+version     = "2023.4.0"
 license     = {text = "MIT License"}
 description = "Homematic interface for Home Assistant running on Python 3."
 readme      = "README.md"
 authors     = [
     {name = "Daniel Perna", email = "danielperna84@gmail.com"},
     {name = "SukramJ", email = "sukramj@icloud.com"},
 ]
```

