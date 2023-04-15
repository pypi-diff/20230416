# Comparing `tmp/openhasp_config_manager-0.4.8.tar.gz` & `tmp/openhasp_config_manager-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openhasp_config_manager-0.4.8.tar", max compression
+gzip compressed data, was "openhasp_config_manager-0.5.0.tar", max compression
```

## Comparing `openhasp_config_manager-0.4.8.tar` & `openhasp_config_manager-0.5.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0    34523 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/LICENSE
--rw-r--r--   0        0        0    13491 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/README.md
--rw-r--r--   0        0        0        0 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/__init__.py
--rw-r--r--   0        0        0    11950 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/__init__.py
--rw-r--r--   0        0        0      746 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/cmd.py
--rw-r--r--   0        0        0     3473 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/common.py
--rw-r--r--   0        0        0     1231 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/deploy.py
--rw-r--r--   0        0        0     1044 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/generate.py
--rw-r--r--   0        0        0     1152 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/listen.py
--rw-r--r--   0        0        0      972 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/logs.py
--rw-r--r--   0        0        0     1292 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/screenshot.py
--rw-r--r--   0        0        0     1023 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/shell.py
--rw-r--r--   0        0        0     1056 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/state.py
--rw-r--r--   0        0        0     1072 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/upload.py
--rw-r--r--   0        0        0     1265 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli/vars.py
--rw-r--r--   0        0        0      257 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/cli.py
--rw-r--r--   0        0        0      153 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/const.py
--rw-r--r--   0        0        0    16151 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/manager.py
--rw-r--r--   0        0        0        0 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/__init__.py
--rw-r--r--   0        0        0     1819 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/image_processor.py
--rw-r--r--   0        0        0        0 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/__init__.py
--rw-r--r--   0        0        0      229 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/component.py
--rw-r--r--   0        0        0      958 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/config.py
--rw-r--r--   0        0        0      164 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/debug_config.py
--rw-r--r--   0        0        0      362 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/device.py
--rw-r--r--   0        0        0      190 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/device_config.py
--rw-r--r--   0        0        0      224 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/gui_config.py
--rw-r--r--   0        0        0      178 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/hasp_config.py
--rw-r--r--   0        0        0      111 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/http_config.py
--rw-r--r--   0        0        0      154 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/mqtt_config.py
--rw-r--r--   0        0        0      193 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/openhasp_config_manager_config.py
--rw-r--r--   0        0        0       98 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/screen_config.py
--rw-r--r--   0        0        0       97 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/telnet_config.py
--rw-r--r--   0        0        0       85 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/website_config.py
--rw-r--r--   0        0        0       97 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/wifi_config.py
--rw-r--r--   0        0        0     4033 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/mqtt_client.py
--rw-r--r--   0        0        0    12037 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/openhasp.py
--rw-r--r--   0        0        0     4833 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/telnet_client.py
--rw-r--r--   0        0        0     8705 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/webservice_client.py
--rw-r--r--   0        0        0        0 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/processing/__init__.py
--rw-r--r--   0        0        0     6089 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/processing/device_processor.py
--rw-r--r--   0        0        0      369 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/processing/jsonl/__init__.py
--rw-r--r--   0        0        0     2198 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/processing/jsonl/jsonl.py
--rw-r--r--   0        0        0        0 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/processing/preprocessor/__init__.py
--rw-r--r--   0        0        0     2479 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/processing/preprocessor/jsonl_preprocessor.py
--rw-r--r--   0        0        0     5401 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/processing/template_rendering.py
--rw-r--r--   0        0        0     5464 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/processing/variables.py
--rw-r--r--   0        0        0        0 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/ui/__init__.py
--rw-r--r--   0        0        0     1427 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/ui/util.py
--rw-r--r--   0        0        0     6053 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/uploader.py
--rw-r--r--   0        0        0     1798 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/util.py
--rw-r--r--   0        0        0      565 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/validation/__init__.py
--rw-r--r--   0        0        0      649 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/validation/cmd.py
--rw-r--r--   0        0        0     1140 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/validation/device_validator.py
--rw-r--r--   0        0        0     2111 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/openhasp_config_manager/validation/jsonl.py
--rw-r--r--   0        0        0     1300 2023-04-15 14:39:17.579121 openhasp_config_manager-0.4.8/pyproject.toml
--rw-r--r--   0        0        0    14707 1970-01-01 00:00:00.000000 openhasp_config_manager-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/LICENSE
+-rw-r--r--   0        0        0    13491 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/__init__.py
+-rw-r--r--   0        0        0    11950 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/cli/__init__.py
+-rw-r--r--   0        0        0      746 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/cli/cmd.py
+-rw-r--r--   0        0        0     3473 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/cli/common.py
+-rw-r--r--   0        0        0     1231 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/cli/deploy.py
+-rw-r--r--   0        0        0     1044 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/cli/generate.py
+-rw-r--r--   0        0        0     1152 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/cli/listen.py
+-rw-r--r--   0        0        0      972 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/cli/logs.py
+-rw-r--r--   0        0        0     1292 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/cli/screenshot.py
+-rw-r--r--   0        0        0     1023 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/cli/shell.py
+-rw-r--r--   0        0        0     1056 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/cli/state.py
+-rw-r--r--   0        0        0     1072 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/cli/upload.py
+-rw-r--r--   0        0        0     1297 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/cli/vars.py
+-rw-r--r--   0        0        0      257 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/cli.py
+-rw-r--r--   0        0        0      153 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/const.py
+-rw-r--r--   0        0        0    19812 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/manager.py
+-rw-r--r--   0        0        0        0 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/__init__.py
+-rw-r--r--   0        0        0     1819 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/image_processor.py
+-rw-r--r--   0        0        0        0 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/model/__init__.py
+-rw-r--r--   0        0        0      886 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/model/component.py
+-rw-r--r--   0        0        0      958 2023-04-16 00:02:05.682420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/model/config.py
+-rw-r--r--   0        0        0      164 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/model/debug_config.py
+-rw-r--r--   0        0        0      510 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/model/device.py
+-rw-r--r--   0        0        0      190 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/model/device_config.py
+-rw-r--r--   0        0        0      224 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/model/gui_config.py
+-rw-r--r--   0        0        0      178 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/model/hasp_config.py
+-rw-r--r--   0        0        0      111 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/model/http_config.py
+-rw-r--r--   0        0        0      154 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/model/mqtt_config.py
+-rw-r--r--   0        0        0      193 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/model/openhasp_config_manager_config.py
+-rw-r--r--   0        0        0       98 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/model/screen_config.py
+-rw-r--r--   0        0        0       97 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/model/telnet_config.py
+-rw-r--r--   0        0        0       85 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/model/website_config.py
+-rw-r--r--   0        0        0       97 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/model/wifi_config.py
+-rw-r--r--   0        0        0     4033 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/mqtt_client.py
+-rw-r--r--   0        0        0    12043 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/openhasp.py
+-rw-r--r--   0        0        0     4833 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/telnet_client.py
+-rw-r--r--   0        0        0     8695 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/webservice_client.py
+-rw-r--r--   0        0        0        0 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/processing/__init__.py
+-rw-r--r--   0        0        0     6687 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/processing/device_processor.py
+-rw-r--r--   0        0        0      369 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/processing/jsonl/__init__.py
+-rw-r--r--   0        0        0     2198 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/processing/jsonl/jsonl.py
+-rw-r--r--   0        0        0        0 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/processing/preprocessor/__init__.py
+-rw-r--r--   0        0        0     2479 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/processing/preprocessor/jsonl_preprocessor.py
+-rw-r--r--   0        0        0     5401 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/processing/template_rendering.py
+-rw-r--r--   0        0        0     5955 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/processing/variables.py
+-rw-r--r--   0        0        0        0 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/ui/__init__.py
+-rw-r--r--   0        0        0     1427 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/ui/util.py
+-rw-r--r--   0        0        0     7917 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/uploader.py
+-rw-r--r--   0        0        0     1784 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/util.py
+-rw-r--r--   0        0        0      565 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/validation/__init__.py
+-rw-r--r--   0        0        0      649 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/validation/cmd.py
+-rw-r--r--   0        0        0     1140 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/validation/device_validator.py
+-rw-r--r--   0        0        0     2111 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/openhasp_config_manager/validation/jsonl.py
+-rw-r--r--   0        0        0     1300 2023-04-16 00:02:05.686420 openhasp_config_manager-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    14707 1970-01-01 00:00:00.000000 openhasp_config_manager-0.5.0/PKG-INFO
```

### Comparing `openhasp_config_manager-0.4.8/LICENSE` & `openhasp_config_manager-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/README.md` & `openhasp_config_manager-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/__init__.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/cmd.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/cli/cmd.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/common.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/cli/common.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/deploy.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/cli/deploy.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/generate.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/cli/generate.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/listen.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/cli/listen.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/logs.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/cli/logs.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/screenshot.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/cli/screenshot.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/shell.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/cli/shell.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/state.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/cli/state.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/upload.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/cli/upload.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/cli/vars.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/cli/vars.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,12 +23,13 @@
 
     return "\n".join(get_dict_contents(variables))
 
 
 async def c_vars(config_dir: Path, path: str):
     try:
         variable_manager = VariableManager(cfg_root=config_dir)
+        variable_manager.read()
         variables = variable_manager.get_vars(Path(config_dir, path))
         formatted = await _format_variables(variables)
         echo(formatted)
     except Exception as ex:
         error(str(ex))
```

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/manager.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/manager.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import shutil
 from pathlib import Path
 from typing import List, Set
 
 import orjson
 
 from openhasp_config_manager.const import COMMON_FOLDER_NAME, DEVICES_FOLDER_NAME, SYSTEM_SCRIPTS
-from openhasp_config_manager.openhasp_client.model.component import Component
+from openhasp_config_manager.openhasp_client.model.component import Component, TextComponent, RawComponent, \
+    ImageComponent, JsonlComponent, CmdComponent, FontComponent
 from openhasp_config_manager.openhasp_client.model.config import Config
 from openhasp_config_manager.openhasp_client.model.debug_config import DebugConfig
 from openhasp_config_manager.openhasp_client.model.device import Device
 from openhasp_config_manager.openhasp_client.model.device_config import DeviceConfig
 from openhasp_config_manager.openhasp_client.model.gui_config import GuiConfig
 from openhasp_config_manager.openhasp_client.model.hasp_config import HaspConfig
 from openhasp_config_manager.openhasp_client.model.http_config import HttpConfig
@@ -46,14 +47,15 @@
         """
         Analyze the configuration file tree and the contents of relevant files.
         The result will be a list of Device object instances, representing the structure
         and configuration found.
 
         :return: list of devices, which can be used in the ConfigManager.process() method
         """
+        self._variable_manager.read()
         return self._analyze(self.cfg_root, self._output_root)
 
     def _analyze(self, cfg_dir_root: Path, output_dir_root: Path) -> List[Device]:
         result: List[Device] = []
 
         common_components_path = Path(cfg_dir_root, COMMON_FOLDER_NAME)
         common_components = self._read_components(common_components_path, prefix="common")
@@ -71,18 +73,23 @@
             try:
                 config = self._read_config(device_path)
             except Exception as ex:
                 raise Exception(f"Error reading config '{device_path}': {ex}")
 
             device_components = self._analyze_device(config, device_path)
 
+            combined_components = common_components + device_components
+
             device = Device(
                 path=device_path,
                 name=device_path.name,
-                components=common_components + device_components,
+                jsonl=[c for c in combined_components if isinstance(c, JsonlComponent)],
+                cmd=[c for c in combined_components if isinstance(c, CmdComponent)],
+                images=[c for c in combined_components if isinstance(c, ImageComponent)],
+                fonts=[c for c in combined_components if isinstance(c, FontComponent)],
                 config=config,
                 output_dir=device_output_dir,
             )
 
             result.append(device)
 
         return result
@@ -111,28 +118,80 @@
         Recursively reads all components from the given path.
         :param path: the root path to read components from
         :param prefix: a prefix to add to the component name
         :return: list of components
         """
         result: List[Component] = []
 
-        for suffix in [".jsonl", ".cmd"]:
+        result.extend(self._read_jsonl_components(path, prefix))
+        result.extend(self._read_cmd_components(path, prefix))
+        result.extend(self._read_image_components(path, prefix))
+
+        return result
+
+    def _read_jsonl_components(self, path, prefix) -> List[Component]:
+        result = []
+        suffix = ".jsonl"
+        for file in path.rglob(f"*{suffix}"):
+            component = self._create_text_component_from_path(
+                device_cfg_dir_root=path,
+                path=Path(path, file.relative_to(path)).relative_to(path),
+                prefix=prefix
+            )
+            if component is not None:
+                jsonl_component = JsonlComponent(
+                    name=component.name,
+                    type=component.type,
+                    path=component.path,
+                    content=component.content,
+                )
+                result.append(jsonl_component)
+        return result
+
+    def _read_cmd_components(self, path, prefix) -> List[Component]:
+        result = []
+        suffix = ".cmd"
+        for file in path.rglob(f"*{suffix}"):
+            component = self._create_text_component_from_path(
+                device_cfg_dir_root=path,
+                path=Path(path, file.relative_to(path)).relative_to(path),
+                prefix=prefix
+            )
+            if component is not None:
+                cmd_component = CmdComponent(
+                    name=component.name,
+                    type=component.type,
+                    path=component.path,
+                    content=component.content,
+                )
+                result.append(cmd_component)
+        return result
+
+    def _read_image_components(self, path, prefix) -> List[Component]:
+        result = []
+        image_suffixes = [".png", ".bin"]
+        for suffix in image_suffixes:
             for file in path.rglob(f"*{suffix}"):
-                component = self._create_component_from_path(
+                component = self._create_raw_component_from_path(
                     device_cfg_dir_root=path,
                     path=Path(path, file.relative_to(path)).relative_to(path),
                     prefix=prefix
                 )
                 if component is not None:
-                    result.append(component)
-
+                    image_component = ImageComponent(
+                        name=component.name,
+                        type=component.type,
+                        path=component.path,
+                        content=component.content,
+                    )
+                    result.append(image_component)
         return result
 
     @staticmethod
-    def _create_component_from_path(device_cfg_dir_root: Path, path: Path, prefix: str) -> Component or None:
+    def _create_text_component_from_path(device_cfg_dir_root: Path, path: Path, prefix: str) -> Component or None:
         file = Path(device_cfg_dir_root, path)
 
         if not file.is_file():
             warn(f"Not a file, skipping: {file}")
             return None
 
         content = file.read_text()
@@ -140,15 +199,40 @@
         name_parts = []
         if len(prefix) > 0:
             name_parts.append(prefix)
         name_parts = name_parts + list(file.relative_to(device_cfg_dir_root).parts)
 
         name = "_".join(name_parts)
         suffix = file.suffix
-        component = Component(
+        component = TextComponent(
+            name=name,
+            type=suffix[1:],
+            path=file,
+            content=content,
+        )
+        return component
+
+    @staticmethod
+    def _create_raw_component_from_path(device_cfg_dir_root: Path, path: Path, prefix: str) -> Component or None:
+        file = Path(device_cfg_dir_root, path)
+
+        if not file.is_file():
+            warn(f"Not a file, skipping: {file}")
+            return None
+
+        content = file.read_bytes()
+
+        name_parts = []
+        if len(prefix) > 0:
+            name_parts.append(prefix)
+        name_parts = name_parts + list(file.relative_to(device_cfg_dir_root).parts)
+
+        name = "_".join(name_parts)
+        suffix = file.suffix
+        component = RawComponent(
             name=name,
             type=suffix[1:],
             path=file,
             content=content,
         )
         return component
 
@@ -284,19 +368,17 @@
 
         jsonl_validator = JsonlObjectValidator()
         cmd_file_validator = CmdFileValidator()
         device_validator = DeviceValidator(device.config, jsonl_validator, cmd_file_validator)
 
         # feed device specific data to the processor
         # Note: this also includes common components
-        for component in device.components:
-            if component.type == "jsonl":
-                device_processor.add_jsonl(component)
-            else:
-                device_processor.add_other(component)
+        components: List[Component] = device.jsonl + device.cmd + device.images + device.fonts
+        for component in components:
+            device_processor.add_component(component)
 
         # only include files which are referenced in a cmd file
         relevant_components = self.find_relevant_components(device)
 
         # let the processor manage each component
         for component in relevant_components:
             output_content = None
@@ -309,101 +391,112 @@
                 device_validator.validate(component, output_content)
             except Exception as ex:
                 raise Exception(f"Validation for {component.path} failed: {ex}")
 
             self._write_output(device, component, output_content)
 
     def find_relevant_components(self, device: Device) -> List[Component]:
-        cmd_components = list(filter(lambda x: x.type == "cmd", device.components))
-        jsonl_components = list(filter(lambda x: x.type == "jsonl", device.components))
+        result: List[Component] = []
+        cmd_components = device.cmd
+        jsonl_components = device.jsonl
+        image_components = device.images
 
         referenced_cmd_components = self._find_referenced_cmd_components(cmd_components)
 
         # find jsonl files referenced in CMD files
         referenced_jsonl_components = self._find_referenced_jsonl_components(cmd_components, jsonl_components)
 
         # compute component for jsonl file referenced in config.hasp.pages
         pages_jsonl_component_path = self._compute_component_path_of_pages_config_value(device.path, device.config)
         if pages_jsonl_component_path is not None:
-            pages_jsonl_component = self._create_component_from_path(
+            pages_jsonl_component = self._create_text_component_from_path(
                 device_cfg_dir_root=device.path,
                 path=pages_jsonl_component_path, prefix=""
             )
             referenced_jsonl_components.add(pages_jsonl_component)
 
-        return list(referenced_jsonl_components) + list(referenced_cmd_components)
+        result.extend(referenced_jsonl_components)
+        result.extend(referenced_cmd_components)
+        # TODO: filter these by actual usage
+        result.extend(image_components)
+        return result
 
-    def _find_referenced_cmd_components(self, components: List[Component]) -> Set[Component]:
+    def _find_referenced_cmd_components(self, cmd_components: List[CmdComponent]) -> Set[CmdComponent]:
         result = set()
 
-        system_components = list(filter(lambda x: x.name in SYSTEM_SCRIPTS, components))
-        cmd_components = [c for c in components if c.type == "cmd"] + system_components
+        system_components = list(filter(lambda x: x.name in SYSTEM_SCRIPTS, cmd_components))
+        cmd_components = cmd_components + system_components
 
         # TODO: this should also consider the hierarchy, if a cmd component is not a system component, and
         #  it is also not referenced anywhere, the component is not relevant
 
         for component in cmd_components:
             cmd_references = self._find_cmd_references_in_cmd_component(component)
             for match in cmd_references:
-                matching_components = list(filter(lambda x: x.name == match, components))
+                matching_components = list(filter(lambda x: x.name == match, cmd_components))
                 if len(matching_components) <= 0:
                     found_component_names = ','.join([c.name for c in cmd_components])
                     raise AssertionError(
                         f"Referenced CMD component not found: {match}, only found: {found_component_names}")
                 result.update(matching_components)
 
         # system components should always be included
         result.update(system_components)
 
         return result
 
     def _find_referenced_jsonl_components(
-            self,
-            cmd_components: List[Component],
-            jsonl_components: List[Component]
-    ) -> Set[Component]:
+        self,
+        cmd_components: List[CmdComponent],
+        jsonl_components: List[JsonlComponent]
+    ) -> Set[JsonlComponent]:
         referenced_jsonl_components = set()
         for component in cmd_components:
             jsonl_references = self._find_jsonl_references_in_cmd_component(component)
             for match in jsonl_references:
                 matching_components = list(filter(lambda x: x.name == match, jsonl_components))
                 if len(matching_components) <= 0:
                     found_component_names = ','.join([c.name for c in jsonl_components])
                     raise AssertionError(
                         f"Referenced JSONL component not found: {match}, only found: {found_component_names}")
                 referenced_jsonl_components.update(matching_components)
 
         return referenced_jsonl_components
 
     @staticmethod
-    def _find_cmd_references_in_cmd_component(component: Component) -> Set[str]:
+    def _find_cmd_references_in_cmd_component(component: TextComponent) -> Set[str]:
         result = set()
         pattern = re.compile("L:/(.*\.cmd)")
         for line in component.content.splitlines():
             matches = re.findall(pattern, line)
             result.update(matches)
         return result
 
     @staticmethod
-    def _find_jsonl_references_in_cmd_component(component: Component) -> Set[str]:
+    def _find_jsonl_references_in_cmd_component(component: TextComponent) -> Set[str]:
         result = set()
         pattern = re.compile("L:/(.*\.jsonl)")
         for line in component.content.splitlines():
             matches = re.findall(pattern, line)
             result.update(matches)
         return result
 
     @staticmethod
-    def _write_output(device: Device, component: Component, output_content: str):
+    def _write_output(device: Device, component: Component, output_content: str | bytes):
         device.output_dir.mkdir(parents=True, exist_ok=True)
 
         component_output_file = Path(
             device.output_dir,
             component.name
         )
 
-        component_output_file.write_text(output_content)
+        if isinstance(output_content, bytes):
+            component_output_file.write_bytes(output_content)
+        elif isinstance(output_content, str):
+            component_output_file.write_text(output_content)
+        else:
+            raise AssertionError(f"Unsupported output type: {type(output_content)}")
 
     @staticmethod
     def _clear_output(device: Device):
         if device.output_dir.exists():
             shutil.rmtree(device.output_dir)
```

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/image_processor.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/image_processor.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/model/config.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/model/config.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/mqtt_client.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/openhasp.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/openhasp.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
     def get_files(self) -> List[str]:
         """
         Retrieve a list of all file on the device
         :return: a list of all files on the device
         """
         return self._webservice_client.get_files()
 
-    def get_file_content(self, file_name: str) -> str or None:
+    def get_file_content(self, file_name: str) -> bytes or None:
         return self._webservice_client.get_file_content(file_name)
 
     def delete_file(self, file_name: str):
         """
         Delete a file on the device
         :param file_name: the name of the file
         """
@@ -319,22 +319,22 @@
         """
         Set the GUI configuration
         :param config: the configuration to set
         :return:
         """
         self._webservice_client.set_gui_config(config)
 
-    def upload_files(self, files: Dict[str, str]):
+    def upload_files(self, files: Dict[str, bytes]):
         """
         Upload a collection of files
         :param files: "target file name"->"file content" mapping
         """
         self._webservice_client.upload_files(files)
 
-    def upload_file(self, name: str, content: str):
+    def upload_file(self, name: str, content: bytes):
         """
         Upload a single file
         :param name: the target name of the file on the device
         :param content: the file content
         """
         info(f"Uploading '{name}'...")
         self._webservice_client.upload_file(name, content)
```

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/telnet_client.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/telnet_client.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/openhasp_client/webservice_client.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/openhasp_client/webservice_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,23 +179,23 @@
 
         self._do_request(
             method=POST,
             url=self._base_url + "config",
             data=data,
         )
 
-    def upload_files(self, files: Dict[str, str]):
+    def upload_files(self, files: Dict[str, bytes]):
         """
         Upload a collection of files
         :param files: "target file name"->"file content" mapping
         """
         for name, content in files.items():
             self.upload_file(name, content)
 
-    def upload_file(self, name: str, content: str):
+    def upload_file(self, name: str, content: bytes):
         """
         Upload a single file
         :param name: the target name of the file on the device
         :param content: the file content
         """
         self._do_request(
             method=POST,
@@ -216,21 +216,21 @@
         )
         response_data = orjson.loads(response.decode('utf-8'))
 
         files = list(filter(lambda x: x["type"] == "file", response_data))
         file_names = list(map(lambda x: x["name"], files))
         return file_names
 
-    def get_file_content(self, file_name: str) -> str or None:
+    def get_file_content(self, file_name: str) -> bytes or None:
         try:
             response = self._do_request(
                 method=GET,
                 url=self._base_url + file_name,
             )
-            response_data = response.decode('utf-8')
+            response_data = response
             return response_data
         except Exception as ex:
             return None
 
     def delete_file(self, file_name: str):
         """
         Delete a file on the device
```

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/processing/device_processor.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/processing/device_processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from typing import List, Dict, Any
 
 import orjson
 
-from openhasp_config_manager.openhasp_client.model.component import Component
+from openhasp_config_manager.openhasp_client.model.component import Component, JsonlComponent, CmdComponent, \
+    TextComponent, RawComponent
 from openhasp_config_manager.openhasp_client.model.config import Config
 from openhasp_config_manager.openhasp_client.model.device import Device
 from openhasp_config_manager.processing.jsonl import JsonlObjectProcessor
 from openhasp_config_manager.processing.preprocessor.jsonl_preprocessor import JsonlPreProcessor
 from openhasp_config_manager.processing.template_rendering import render_dict_recursive, _render_template
 from openhasp_config_manager.processing.variables import VariableManager
 from openhasp_config_manager.util import merge_dict_recursive
@@ -19,37 +20,48 @@
     present within the configuration files.
     """
 
     def __init__(self, device: Device, jsonl_object_processors: List[JsonlObjectProcessor],
                  variable_manager: VariableManager):
         self._device = device
 
-        self._jsonl_components: List[Component] = []
+        self._jsonl_components: List[JsonlComponent] = []
         self._others: List[Component] = []
 
         self._jsonl_preprocessor = JsonlPreProcessor()
         self._jsonl_object_processors = jsonl_object_processors
         self._variable_manager = variable_manager
 
-    def add_other(self, component: Component):
+    def add_component(self, component: Component):
+        if isinstance(component, JsonlComponent):
+            self._add_jsonl(component)
+        else:
+            self._add_other(component)
+
+    def _add_other(self, component: Component):
         self._others.append(component)
 
-    def add_jsonl(self, component: Component):
+    def _add_jsonl(self, component: JsonlComponent):
         self._jsonl_components.append(component)
 
     def normalize(self, device: Device, component: Component) -> str:
-        if component.type == "jsonl":
+        if isinstance(component, JsonlComponent):
             template_vars: Dict[str, any] = self._compute_jsonl_template_variables(device, component)
             return self._normalize_jsonl(self._device.config, component, template_vars)
-        elif component.type == "cmd":
+        elif isinstance(component, CmdComponent):
             template_vars: Dict[str, any] = {}
             return self._normalize_cmd(self._device.config, component, template_vars)
-        else:
+        elif isinstance(component, TextComponent):
+            # no changes necessary
+            return component.content
+        elif isinstance(component, RawComponent):
             # no changes necessary
             return component.content
+        elif isinstance(component, Component):
+            raise NotImplementedError(f"Unknown component type: {component.type}")
 
     def _normalize_jsonl(self, config: Config, component: Component, template_vars: Dict[str, any]) -> str:
         normalized_objects: List[str] = []
 
         objects = self._jsonl_preprocessor.split_jsonl_objects(component.content)
         for ob in objects:
             preprocessed = self._jsonl_preprocessor.cleanup_object_for_json_parsing(ob)
@@ -72,15 +84,15 @@
 
         processed = normalized_object
         for processor in self._jsonl_object_processors:
             processed = processor.process(processed, config)
 
         return json.dumps(processed, indent=None)
 
-    def _normalize_cmd(self, _device_config, component, template_vars: Dict[str, any]) -> str:
+    def _normalize_cmd(self, _device_config, component: CmdComponent, template_vars: Dict[str, any]) -> str:
         return _render_template(component.content, template_vars)
 
     def _compute_jsonl_template_variables(self, device: Device, component: Component) -> Dict[str, Any]:
         """
         Computes a map of "variable" -> "evaluated value in the given path context" for the given component.
 
         :param component: the component to use as a context for evaluating template variables
```

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/processing/jsonl/jsonl.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/processing/jsonl/jsonl.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/processing/preprocessor/jsonl_preprocessor.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/processing/preprocessor/jsonl_preprocessor.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/processing/template_rendering.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/processing/template_rendering.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/processing/variables.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/processing/variables.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,20 +12,36 @@
     Used to manage variable definitions found in YAML files inside the configuration
     directory.
     """
 
     def __init__(self, cfg_root: Path):
         self._cfg_root: Path = Path(cfg_root)
         self._path_vars: Dict[str, Dict] = {}
-        self._path_vars = self._read(cfg_root)
+
+    def read(self):
+        """
+        Reads all variable definitions from the configuration directory.
+        """
+        self._path_vars = self._read(self._cfg_root)
 
     def add_var(self, key: str, value: any, path: Path = None):
+        """
+        Registers a variable to a path
+        :param key: the variable key
+        :param value: the variable value
+        :param path: the path this variable should apply to
+        """
         self.add_vars({key: value}, path)
 
     def add_vars(self, vars: Dict[str, Any], path: Path = None):
+        """
+        Registers a set of variables to a path
+        :param vars: the variables
+        :param path: the path the variables should apply to
+        """
         if path is None:
             path = self._cfg_root
 
         relative_path = Path(self._cfg_root, path.relative_to(self._cfg_root))
         if relative_path.is_file():
             relative_path = relative_path.parent
         relative_path_str = str(relative_path)
```

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/ui/util.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/ui/util.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/uploader.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/uploader.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,52 +35,99 @@
         existing_files = self._api_client.get_files()
 
         result = False
 
         for file in device.output_dir.iterdir():
             info(f"Preparing '{file.name}' for upload...")
 
-            content = file.read_text()
-
-            if len(content) <= 0:
-                warn(f"File is empty, skipping upload: {file}")
-                continue
-
-            # check if the checksum of the file has changed on the device
-            file_content_on_device = ""
-            if file.name in existing_files:
-                file_content_on_device = self._api_client.get_file_content(file.name)
-                device_file_content_checksum = util.calculate_checksum(file_content_on_device)
+            if file.suffix in [".cmd", ".jsonl"]:
+                result &= self._upload_text_file(device, print_diff, file, existing_files)
             else:
-                device_file_content_checksum = None
+                result &= self._upload_binary_file(device, print_diff, file, existing_files)
 
-            new_checksum = self._check_if_checksum_will_change(
-                file=file,
-                original_checksum=device_file_content_checksum,
-                new_content=content
-            )
+        return result
 
-            if new_checksum is not None:
-                result = True
-                if print_diff:
-                    diff_output = self._calculate_diff(
-                        file_name=file.name,
-                        string1=file_content_on_device,
-                        string2=content
-                    )
-                    print_diff_to_console(diff_output)
-                try:
-                    self._api_client.upload_file(file.name, content)
-                    checksum_file = self._get_checksum_file(file)
-                    checksum_file.parent.mkdir(parents=True, exist_ok=True)
-                    checksum_file.write_text(new_checksum)
-                except Exception as ex:
-                    raise Exception(f"Error uploading file '{file.name}' to '{device.name}': {ex}")
-            else:
-                info(f"Skipping {file} because it hasn't changed.")
+    def _upload_text_file(self, device, print_diff, file, existing_files) -> bool:
+        result = False
+
+        content = file.read_text()
+        if len(content) <= 0:
+            warn(f"File is empty, skipping upload: {file}")
+            return result
+
+        # check if the checksum of the file has changed on the device
+        file_content_on_device = ""
+        if file.name in existing_files:
+            file_content_on_device = self._api_client.get_file_content(file.name).decode("utf-8")
+            device_file_content_checksum = util.calculate_checksum(file_content_on_device.encode("utf-8"))
+        else:
+            device_file_content_checksum = None
+
+        new_checksum = self._check_if_checksum_will_change(
+            file=file,
+            original_checksum=device_file_content_checksum,
+            new_content=content.encode("utf-8")
+        )
+
+        if new_checksum is not None:
+            result = True
+            if print_diff:
+                diff_output = self._calculate_diff(
+                    file_name=file.name,
+                    string1=file_content_on_device,
+                    string2=content
+                )
+                print_diff_to_console(diff_output)
+            try:
+                self._api_client.upload_file(file.name, content.encode("utf-8"))
+                checksum_file = self._get_checksum_file(file)
+                checksum_file.parent.mkdir(parents=True, exist_ok=True)
+                checksum_file.write_text(new_checksum)
+            except Exception as ex:
+                raise Exception(f"Error uploading file '{file.name}' to '{device.name}': {ex}")
+        else:
+            info(f"Skipping {file} because it hasn't changed.")
+
+        return result
+
+    def _upload_binary_file(self, device, print_diff, file, existing_files) -> bool:
+        result = False
+
+        content = file.read_bytes()
+        if len(content) <= 0:
+            warn(f"File is empty, skipping upload: {file}")
+            return result
+
+        # check if the checksum of the file has changed on the device
+        file_content_on_device = b""
+        if file.name in existing_files:
+            file_content_on_device: bytes = self._api_client.get_file_content(file.name)
+            device_file_content_checksum = util.calculate_checksum(file_content_on_device)
+        else:
+            device_file_content_checksum = None
+
+        new_checksum = self._check_if_checksum_will_change(
+            file=file,
+            original_checksum=device_file_content_checksum,
+            new_content=content
+        )
+
+        if new_checksum is not None:
+            result = True
+            if print_diff:
+                info(f"Binary file '{file.name}' has changed ({device_file_content_checksum} -> {new_checksum})")
+            try:
+                self._api_client.upload_file(file.name, content)
+                checksum_file = self._get_checksum_file(file)
+                checksum_file.parent.mkdir(parents=True, exist_ok=True)
+                checksum_file.write_text(new_checksum)
+            except Exception as ex:
+                raise Exception(f"Error uploading file '{file.name}' to '{device.name}': {ex}")
+        else:
+            info(f"Skipping {file} because it hasn't changed.")
 
         return result
 
     def cleanup_device(self, device: Device) -> bool:
         """
         Delete files from the device, which are not present in the currently generated output
         :param device: the target device
@@ -97,15 +144,15 @@
         for f in files_on_device:
             if f not in file_names:
                 result = True
                 info(f"Deleting file '{f}' from device '{device.name}'")
                 self._api_client.delete_file(f)
         return result
 
-    def _check_if_checksum_will_change(self, file: Path, original_checksum: str, new_content: str) -> str | None:
+    def _check_if_checksum_will_change(self, file: Path, original_checksum: str, new_content: bytes) -> str | None:
         """
         Checks if the checksum for the given file has changed since it was last uploaded.
         :param file: the path of the file to check
         :param original_checksum: expected checksum of the original content
         :param new_content: the content of the new file
         :return: new checksum if the checksum changed, None otherwise
         """
```

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/util.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict
 
 
-def calculate_checksum(content: str) -> str:
+def calculate_checksum(content: bytes) -> str:
     import hashlib
-    hash_value = hashlib.md5(content.encode('utf-8')).hexdigest()
+    hash_value = hashlib.md5(content).hexdigest()
     return hash_value
 
 
 def contains_nested_dict_key(d: dict, key: str) -> bool:
     """
     Recursively checks if any key in a nested dictionary structure is equal to the given string.
     :param d: the dictionary to check
```

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/validation/__init__.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/validation/cmd.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/validation/cmd.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/validation/device_validator.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/validation/device_validator.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/openhasp_config_manager/validation/jsonl.py` & `openhasp_config_manager-0.5.0/openhasp_config_manager/validation/jsonl.py`

 * *Files identical despite different names*

### Comparing `openhasp_config_manager-0.4.8/pyproject.toml` & `openhasp_config_manager-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openhasp-config-manager"
-version = "0.4.8"
+version = "0.5.0"
 description = "A tool to manage all of your openHASP device configs in a centralized place."
 
 license = "AGPL-3.0-or-later"
 
 authors = [
     "Markus Ressel <mail@markusressel.de>",
 ]
```

### Comparing `openhasp_config_manager-0.4.8/PKG-INFO` & `openhasp_config_manager-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openhasp-config-manager
-Version: 0.4.8
+Version: 0.5.0
 Summary: A tool to manage all of your openHASP device configs in a centralized place.
 Home-page: https://github.com/markusressel/openhasp-config-manager
 License: AGPL-3.0-or-later
 Keywords: openhasp,config,management
 Author: Markus Ressel
 Author-email: mail@markusressel.de
 Requires-Python: >=3.10,<4.0
```

