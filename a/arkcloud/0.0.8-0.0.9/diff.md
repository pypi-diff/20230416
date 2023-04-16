# Comparing `tmp/arkcloud-0.0.8.tar.gz` & `tmp/arkcloud-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arkcloud-0.0.8.tar", last modified: Tue Sep  6 05:36:27 2022, max compression
+gzip compressed data, was "arkcloud-0.0.9.tar", last modified: Tue Sep  6 05:46:17 2022, max compression
```

## Comparing `arkcloud-0.0.8.tar` & `arkcloud-0.0.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2022-09-06 05:36:27.553955 arkcloud-0.0.8/
--rw-rw-rw-   0        0        0     1095 2022-08-06 20:49:26.000000 arkcloud-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1999 2022-09-06 05:36:27.553955 arkcloud-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1305 2022-08-06 05:59:32.000000 arkcloud-0.0.8/README.md
--rw-rw-rw-   0        0        0      534 2022-09-06 04:49:00.000000 arkcloud-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0     1136 2022-09-06 05:36:27.555955 arkcloud-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-09-06 05:36:27.503259 arkcloud-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-09-06 05:36:27.511258 arkcloud-0.0.8/src/arkcloud/
--rw-rw-rw-   0        0        0      104 2022-09-06 04:44:07.000000 arkcloud-0.0.8/src/arkcloud/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-06 05:36:27.527258 arkcloud-0.0.8/src/arkcloud/ai/
--rw-rw-rw-   0        0        0       33 2022-09-06 04:41:26.000000 arkcloud-0.0.8/src/arkcloud/ai/__init__.py
--rw-rw-rw-   0        0        0      358 2022-09-03 03:02:43.000000 arkcloud-0.0.8/src/arkcloud/ai/detect.py
--rw-rw-rw-   0        0        0     5192 2022-09-04 04:00:34.000000 arkcloud-0.0.8/src/arkcloud/ai/ocr.py
-drwxrwxrwx   0        0        0        0 2022-09-06 05:36:27.529893 arkcloud-0.0.8/src/arkcloud/ark/
--rw-rw-rw-   0        0        0       61 2022-09-06 04:57:40.000000 arkcloud-0.0.8/src/arkcloud/ark/__init__.py
--rw-rw-rw-   0        0        0     3920 2022-09-06 04:41:25.000000 arkcloud-0.0.8/src/arkcloud/ark/admin.py
--rw-rw-rw-   0        0        0      451 2022-09-06 05:09:47.000000 arkcloud-0.0.8/src/arkcloud/config.ini
-drwxrwxrwx   0        0        0        0 2022-09-06 05:36:27.530414 arkcloud-0.0.8/src/arkcloud/gamepad/
--rw-rw-rw-   0        0        0       53 2022-09-06 04:57:40.000000 arkcloud-0.0.8/src/arkcloud/gamepad/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-06 05:36:27.531955 arkcloud-0.0.8/src/arkcloud/gamepad/browser/
--rw-rw-rw-   0        0        0       58 2022-09-06 04:57:40.000000 arkcloud-0.0.8/src/arkcloud/gamepad/browser/__init__.py
--rw-rw-rw-   0        0        0     5253 2022-09-06 04:41:25.000000 arkcloud-0.0.8/src/arkcloud/gamepad/browser/xbox.py
-drwxrwxrwx   0        0        0        0 2022-09-06 05:36:27.537956 arkcloud-0.0.8/src/arkcloud/gamepad/components/
--rw-rw-rw-   0        0        0      409 2022-09-06 04:57:40.000000 arkcloud-0.0.8/src/arkcloud/gamepad/components/__init__.py
--rw-rw-rw-   0        0        0     1873 2022-09-06 04:41:25.000000 arkcloud-0.0.8/src/arkcloud/gamepad/components/base.py
--rw-rw-rw-   0        0        0      911 2022-09-06 04:41:25.000000 arkcloud-0.0.8/src/arkcloud/gamepad/components/buttons.py
--rw-rw-rw-   0        0        0      683 2022-09-06 04:41:25.000000 arkcloud-0.0.8/src/arkcloud/gamepad/components/directional_pad.py
--rw-rw-rw-   0        0        0     1193 2022-08-30 04:08:16.000000 arkcloud-0.0.8/src/arkcloud/gamepad/components/event.py
--rw-rw-rw-   0        0        0      843 2022-09-06 04:41:25.000000 arkcloud-0.0.8/src/arkcloud/gamepad/components/joystick.py
--rw-rw-rw-   0        0        0      567 2022-09-06 04:41:26.000000 arkcloud-0.0.8/src/arkcloud/gamepad/components/menu.py
--rw-rw-rw-   0        0        0      732 2022-09-06 04:41:26.000000 arkcloud-0.0.8/src/arkcloud/gamepad/components/shoulder.py
-drwxrwxrwx   0        0        0        0 2022-09-06 05:36:27.539955 arkcloud-0.0.8/src/arkcloud/gamepad/linux/
--rw-rw-rw-   0        0        0        0 2022-08-29 20:03:47.000000 arkcloud-0.0.8/src/arkcloud/gamepad/linux/__init__.py
--rw-rw-rw-   0        0        0     3997 2022-08-29 17:53:14.000000 arkcloud-0.0.8/src/arkcloud/gamepad/linux/example_1.py
-drwxrwxrwx   0        0        0        0 2022-09-06 05:36:27.541956 arkcloud-0.0.8/src/arkcloud/lib/
--rw-rw-rw-   0        0        0      420 2022-09-06 04:57:40.000000 arkcloud-0.0.8/src/arkcloud/lib/__init__.py
--rw-rw-rw-   0        0        0     2489 2022-09-06 05:33:45.000000 arkcloud-0.0.8/src/arkcloud/lib/configuration.py
--rw-rw-rw-   0        0        0     1599 2022-09-06 05:14:48.000000 arkcloud-0.0.8/src/arkcloud/lib/timer.py
-drwxrwxrwx   0        0        0        0 2022-09-06 05:36:27.542954 arkcloud-0.0.8/src/arkcloud/web/
--rw-rw-rw-   0        0        0      248 2022-09-06 04:57:40.000000 arkcloud-0.0.8/src/arkcloud/web/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-06 05:36:27.543956 arkcloud-0.0.8/src/arkcloud/web/driver/
--rw-rw-rw-   0        0        0       71 2022-09-06 04:41:25.000000 arkcloud-0.0.8/src/arkcloud/web/driver/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-06 05:36:27.546955 arkcloud-0.0.8/src/arkcloud/web/driver/chrome/
--rw-rw-rw-   0        0        0       54 2022-09-06 05:02:20.000000 arkcloud-0.0.8/src/arkcloud/web/driver/chrome/__init__.py
--rw-rw-rw-   0        0        0      761 2022-09-06 05:02:20.000000 arkcloud-0.0.8/src/arkcloud/web/driver/chrome/chrome.py
--rw-rw-rw-   0        0        0     5353 2022-09-06 04:57:40.000000 arkcloud-0.0.8/src/arkcloud/web/driver/chrome/options.py
--rw-rw-rw-   0        0        0     1596 2022-09-06 04:57:40.000000 arkcloud-0.0.8/src/arkcloud/web/driver/chrome/service.py
-drwxrwxrwx   0        0        0        0 2022-09-06 05:36:27.548956 arkcloud-0.0.8/src/arkcloud/web/driver/components/
--rw-rw-rw-   0        0        0       85 2022-09-06 05:02:41.000000 arkcloud-0.0.8/src/arkcloud/web/driver/components/__init__.py
--rw-rw-rw-   0        0        0    14561 2022-09-01 18:52:54.000000 arkcloud-0.0.8/src/arkcloud/web/driver/components/element.py
--rw-rw-rw-   0        0        0    11047 2022-09-06 04:57:40.000000 arkcloud-0.0.8/src/arkcloud/web/driver/driver.py
-drwxrwxrwx   0        0        0        0 2022-09-06 05:36:27.552955 arkcloud-0.0.8/src/arkcloud/web/websites/
--rw-rw-rw-   0        0        0      177 2022-09-06 04:57:40.000000 arkcloud-0.0.8/src/arkcloud/web/websites/__init__.py
--rw-rw-rw-   0        0        0    24516 2022-09-06 05:30:49.000000 arkcloud-0.0.8/src/arkcloud/web/websites/ark_website.py
--rw-rw-rw-   0        0        0     2085 2022-09-06 04:41:25.000000 arkcloud-0.0.8/src/arkcloud/web/websites/gamepad_website.py
--rw-rw-rw-   0        0        0     4138 2022-09-06 04:41:25.000000 arkcloud-0.0.8/src/arkcloud/web/websites/website.py
--rw-rw-rw-   0        0        0     3166 2022-09-06 04:57:40.000000 arkcloud-0.0.8/src/arkcloud/web/websites/xbox_controller_extension.py
-drwxrwxrwx   0        0        0        0 2022-09-06 05:36:27.525261 arkcloud-0.0.8/src/arkcloud.egg-info/
--rw-rw-rw-   0        0        0     1999 2022-09-06 05:36:27.000000 arkcloud-0.0.8/src/arkcloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1604 2022-09-06 05:36:27.000000 arkcloud-0.0.8/src/arkcloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-06 05:36:27.000000 arkcloud-0.0.8/src/arkcloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2022-09-06 05:36:27.000000 arkcloud-0.0.8/src/arkcloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-09-06 05:36:27.000000 arkcloud-0.0.8/src/arkcloud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-09-06 05:46:17.909643 arkcloud-0.0.9/
+-rw-rw-rw-   0        0        0     1095 2022-08-06 20:49:26.000000 arkcloud-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1999 2022-09-06 05:46:17.909643 arkcloud-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1305 2022-08-06 05:59:32.000000 arkcloud-0.0.9/README.md
+-rw-rw-rw-   0        0        0      534 2022-09-06 04:49:00.000000 arkcloud-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1136 2022-09-06 05:46:17.911232 arkcloud-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-09-06 05:46:17.736655 arkcloud-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-09-06 05:46:17.751653 arkcloud-0.0.9/src/arkcloud/
+-rw-rw-rw-   0        0        0      104 2022-09-06 04:44:07.000000 arkcloud-0.0.9/src/arkcloud/__init__.py
+drwxrwxrwx   0        0        0        0 2022-09-06 05:46:17.777654 arkcloud-0.0.9/src/arkcloud/ai/
+-rw-rw-rw-   0        0        0       33 2022-09-06 04:41:26.000000 arkcloud-0.0.9/src/arkcloud/ai/__init__.py
+-rw-rw-rw-   0        0        0      358 2022-09-03 03:02:43.000000 arkcloud-0.0.9/src/arkcloud/ai/detect.py
+-rw-rw-rw-   0        0        0     5192 2022-09-04 04:00:34.000000 arkcloud-0.0.9/src/arkcloud/ai/ocr.py
+drwxrwxrwx   0        0        0        0 2022-09-06 05:46:17.786653 arkcloud-0.0.9/src/arkcloud/ark/
+-rw-rw-rw-   0        0        0       61 2022-09-06 04:57:40.000000 arkcloud-0.0.9/src/arkcloud/ark/__init__.py
+-rw-rw-rw-   0        0        0     3920 2022-09-06 04:41:25.000000 arkcloud-0.0.9/src/arkcloud/ark/admin.py
+-rw-rw-rw-   0        0        0      451 2022-09-06 05:09:47.000000 arkcloud-0.0.9/src/arkcloud/config.ini
+drwxrwxrwx   0        0        0        0 2022-09-06 05:46:17.789655 arkcloud-0.0.9/src/arkcloud/gamepad/
+-rw-rw-rw-   0        0        0       53 2022-09-06 04:57:40.000000 arkcloud-0.0.9/src/arkcloud/gamepad/__init__.py
+drwxrwxrwx   0        0        0        0 2022-09-06 05:46:17.798653 arkcloud-0.0.9/src/arkcloud/gamepad/browser/
+-rw-rw-rw-   0        0        0       58 2022-09-06 04:57:40.000000 arkcloud-0.0.9/src/arkcloud/gamepad/browser/__init__.py
+-rw-rw-rw-   0        0        0     5253 2022-09-06 04:41:25.000000 arkcloud-0.0.9/src/arkcloud/gamepad/browser/xbox.py
+drwxrwxrwx   0        0        0        0 2022-09-06 05:46:17.833328 arkcloud-0.0.9/src/arkcloud/gamepad/components/
+-rw-rw-rw-   0        0        0      409 2022-09-06 04:57:40.000000 arkcloud-0.0.9/src/arkcloud/gamepad/components/__init__.py
+-rw-rw-rw-   0        0        0     1873 2022-09-06 04:41:25.000000 arkcloud-0.0.9/src/arkcloud/gamepad/components/base.py
+-rw-rw-rw-   0        0        0      911 2022-09-06 04:41:25.000000 arkcloud-0.0.9/src/arkcloud/gamepad/components/buttons.py
+-rw-rw-rw-   0        0        0      683 2022-09-06 04:41:25.000000 arkcloud-0.0.9/src/arkcloud/gamepad/components/directional_pad.py
+-rw-rw-rw-   0        0        0     1193 2022-08-30 04:08:16.000000 arkcloud-0.0.9/src/arkcloud/gamepad/components/event.py
+-rw-rw-rw-   0        0        0      843 2022-09-06 04:41:25.000000 arkcloud-0.0.9/src/arkcloud/gamepad/components/joystick.py
+-rw-rw-rw-   0        0        0      567 2022-09-06 04:41:26.000000 arkcloud-0.0.9/src/arkcloud/gamepad/components/menu.py
+-rw-rw-rw-   0        0        0      732 2022-09-06 04:41:26.000000 arkcloud-0.0.9/src/arkcloud/gamepad/components/shoulder.py
+drwxrwxrwx   0        0        0        0 2022-09-06 05:46:17.839329 arkcloud-0.0.9/src/arkcloud/gamepad/linux/
+-rw-rw-rw-   0        0        0        0 2022-08-29 20:03:47.000000 arkcloud-0.0.9/src/arkcloud/gamepad/linux/__init__.py
+-rw-rw-rw-   0        0        0     3997 2022-08-29 17:53:14.000000 arkcloud-0.0.9/src/arkcloud/gamepad/linux/example_1.py
+drwxrwxrwx   0        0        0        0 2022-09-06 05:46:17.852328 arkcloud-0.0.9/src/arkcloud/lib/
+-rw-rw-rw-   0        0        0      420 2022-09-06 04:57:40.000000 arkcloud-0.0.9/src/arkcloud/lib/__init__.py
+-rw-rw-rw-   0        0        0     2489 2022-09-06 05:33:45.000000 arkcloud-0.0.9/src/arkcloud/lib/configuration.py
+-rw-rw-rw-   0        0        0     1599 2022-09-06 05:14:48.000000 arkcloud-0.0.9/src/arkcloud/lib/timer.py
+drwxrwxrwx   0        0        0        0 2022-09-06 05:46:17.855328 arkcloud-0.0.9/src/arkcloud/web/
+-rw-rw-rw-   0        0        0      248 2022-09-06 04:57:40.000000 arkcloud-0.0.9/src/arkcloud/web/__init__.py
+drwxrwxrwx   0        0        0        0 2022-09-06 05:46:17.864328 arkcloud-0.0.9/src/arkcloud/web/driver/
+-rw-rw-rw-   0        0        0       71 2022-09-06 04:41:25.000000 arkcloud-0.0.9/src/arkcloud/web/driver/__init__.py
+drwxrwxrwx   0        0        0        0 2022-09-06 05:46:17.881329 arkcloud-0.0.9/src/arkcloud/web/driver/chrome/
+-rw-rw-rw-   0        0        0       54 2022-09-06 05:02:20.000000 arkcloud-0.0.9/src/arkcloud/web/driver/chrome/__init__.py
+-rw-rw-rw-   0        0        0      761 2022-09-06 05:02:20.000000 arkcloud-0.0.9/src/arkcloud/web/driver/chrome/chrome.py
+-rw-rw-rw-   0        0        0     5353 2022-09-06 04:57:40.000000 arkcloud-0.0.9/src/arkcloud/web/driver/chrome/options.py
+-rw-rw-rw-   0        0        0     1596 2022-09-06 04:57:40.000000 arkcloud-0.0.9/src/arkcloud/web/driver/chrome/service.py
+drwxrwxrwx   0        0        0        0 2022-09-06 05:46:17.890329 arkcloud-0.0.9/src/arkcloud/web/driver/components/
+-rw-rw-rw-   0        0        0       85 2022-09-06 05:02:41.000000 arkcloud-0.0.9/src/arkcloud/web/driver/components/__init__.py
+-rw-rw-rw-   0        0        0    14561 2022-09-01 18:52:54.000000 arkcloud-0.0.9/src/arkcloud/web/driver/components/element.py
+-rw-rw-rw-   0        0        0    11047 2022-09-06 04:57:40.000000 arkcloud-0.0.9/src/arkcloud/web/driver/driver.py
+drwxrwxrwx   0        0        0        0 2022-09-06 05:46:17.908576 arkcloud-0.0.9/src/arkcloud/web/websites/
+-rw-rw-rw-   0        0        0      177 2022-09-06 04:57:40.000000 arkcloud-0.0.9/src/arkcloud/web/websites/__init__.py
+-rw-rw-rw-   0        0        0    24884 2022-09-06 05:46:04.000000 arkcloud-0.0.9/src/arkcloud/web/websites/ark_website.py
+-rw-rw-rw-   0        0        0     2085 2022-09-06 04:41:25.000000 arkcloud-0.0.9/src/arkcloud/web/websites/gamepad_website.py
+-rw-rw-rw-   0        0        0     4138 2022-09-06 04:41:25.000000 arkcloud-0.0.9/src/arkcloud/web/websites/website.py
+-rw-rw-rw-   0        0        0     3166 2022-09-06 04:57:40.000000 arkcloud-0.0.9/src/arkcloud/web/websites/xbox_controller_extension.py
+drwxrwxrwx   0        0        0        0 2022-09-06 05:46:17.765653 arkcloud-0.0.9/src/arkcloud.egg-info/
+-rw-rw-rw-   0        0        0     1999 2022-09-06 05:46:17.000000 arkcloud-0.0.9/src/arkcloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1604 2022-09-06 05:46:17.000000 arkcloud-0.0.9/src/arkcloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-06 05:46:17.000000 arkcloud-0.0.9/src/arkcloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2022-09-06 05:46:17.000000 arkcloud-0.0.9/src/arkcloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2022-09-06 05:46:17.000000 arkcloud-0.0.9/src/arkcloud.egg-info/top_level.txt
```

### Comparing `arkcloud-0.0.8/LICENSE` & `arkcloud-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/PKG-INFO` & `arkcloud-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkcloud
-Version: 0.0.8
+Version: 0.0.9
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Cloud
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Cloud/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `arkcloud-0.0.8/README.md` & `arkcloud-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/pyproject.toml` & `arkcloud-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/setup.cfg` & `arkcloud-0.0.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 726b 636c 6f75 640d 0a76 6572   = arkcloud..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e38 0d0a 6175  sion = 0.0.8..au
+00000020: 7369 6f6e 203d 2030 2e30 2e39 0d0a 6175  sion = 0.0.9..au
 00000030: 7468 6f72 203d 204d 6175 7269 6369 6f0d  thor = Mauricio.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 6465 762e 6d61 7572 6963 696f 2e6c 6f6d  dev.mauricio.lom
 00000060: 656c 6940 676d 6169 6c2e 636f 6d0d 0a64  eli@gmail.com..d
 00000070: 6573 6372 6970 7469 6f6e 203d 2054 6869  escription = Thi
 00000080: 7320 6170 706c 6963 6174 696f 6e20 6163  s application ac
 00000090: 6365 7373 6573 2074 6865 2041 726b 2073  cesses the Ark s
```

### Comparing `arkcloud-0.0.8/src/arkcloud/ai/ocr.py` & `arkcloud-0.0.9/src/arkcloud/ai/ocr.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud/ark/admin.py` & `arkcloud-0.0.9/src/arkcloud/ark/admin.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud/gamepad/browser/xbox.py` & `arkcloud-0.0.9/src/arkcloud/gamepad/browser/xbox.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud/gamepad/components/base.py` & `arkcloud-0.0.9/src/arkcloud/gamepad/components/base.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud/gamepad/components/buttons.py` & `arkcloud-0.0.9/src/arkcloud/gamepad/components/buttons.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud/gamepad/components/directional_pad.py` & `arkcloud-0.0.9/src/arkcloud/gamepad/components/directional_pad.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud/gamepad/components/event.py` & `arkcloud-0.0.9/src/arkcloud/gamepad/components/event.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud/gamepad/components/joystick.py` & `arkcloud-0.0.9/src/arkcloud/gamepad/components/joystick.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud/gamepad/components/menu.py` & `arkcloud-0.0.9/src/arkcloud/gamepad/components/menu.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud/gamepad/components/shoulder.py` & `arkcloud-0.0.9/src/arkcloud/gamepad/components/shoulder.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud/gamepad/linux/example_1.py` & `arkcloud-0.0.9/src/arkcloud/gamepad/linux/example_1.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud/lib/configuration.py` & `arkcloud-0.0.9/src/arkcloud/lib/configuration.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud/lib/timer.py` & `arkcloud-0.0.9/src/arkcloud/lib/timer.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud/web/driver/chrome/chrome.py` & `arkcloud-0.0.9/src/arkcloud/web/driver/chrome/chrome.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud/web/driver/chrome/options.py` & `arkcloud-0.0.9/src/arkcloud/web/driver/chrome/options.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud/web/driver/chrome/service.py` & `arkcloud-0.0.9/src/arkcloud/web/driver/chrome/service.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud/web/driver/components/element.py` & `arkcloud-0.0.9/src/arkcloud/web/driver/components/element.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud/web/driver/driver.py` & `arkcloud-0.0.9/src/arkcloud/web/driver/driver.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud/web/websites/ark_website.py` & `arkcloud-0.0.9/src/arkcloud/web/websites/ark_website.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,53 +266,64 @@
         print("Attempting to respawn")
         self.send_buttons(*(['left'] * 5), spread=0.2)
         self.send_buttons(*(['down'] * 20), spread=0.2)
         self.send_buttons(*(['RIGHT'] * 5), spread=0.2)
         self.send_buttons(*(['down'] * 20), spread=0.2)
         self.send_buttons('left', spread=0.2)
         self.send_buttons('a')
-        print("Finished respawning")
-        return True
+        self._driver.pause(2)
+        if self.is_respawning():
+            return self.respawn()
+        else:
+            print("Finished respawning")
+            return True
 
     def create_character(self):
         if not self.is_character_creation():
             print("Could not detect character creation")
             return False
         self.send_buttons(*(['b'] * 6), spread=0.2)
         print("Attempting to create character")
         self.send_buttons(*(['LEFT'] * 6), spread=0.2)
         self.send_buttons(*(['UP'] * 20), spread=0.2)
         self.send_buttons(*(['DOWN'] * 20), spread=0.2)
         self.send_buttons(*(['RIGHT'] * 6), spread=0.2)
         self.send_buttons('a', spread=1)
+        self._driver.pause(2)
         if self.is_character_creation():
             self.send_buttons(*(['LEFT'] * 6), spread=0.2)
             self.send_buttons(*(['UP'] * 20), spread=0.2)
             self.send_buttons(*(['DOWN'] * 20), spread=0.2)
             self.send_buttons(*(['RIGHT'] * 6), spread=0.2)
             self.send_buttons('UP', 'UP', 'a', 'a', spread=1)
-        print("Finished creating character")
-        return True
+            self._driver.pause(2)
+        if self.is_character_creation():
+            return self.create_character()
+        else:
+            print("Finished creating character")
+            return True
 
     def menu_reset(self, timeout=2):
         print("Trying to go to main menu")
         self.send_buttons('b', 'b', spread=1)
         self.send_buttons('START')
         countdown(2, 'Waiting for menu to appear')
         if self.is_options_menu():
             self.send_buttons('UP', hold=5)
             self.send_buttons('DOWN', 'DOWN', 'DOWN', spread=2)
             self.send_buttons('a')
+            self._driver.pause(2)
             self.send_buttons('b', spread=1)
         if self.resolve_disconnections() or not self.is_intro_menu():
             print("Was unable to resolve or get to the intro menu, trying again...")
             self.send_buttons('START')
             self.send_buttons('UP', hold=5)
             self.send_buttons('DOWN', 'DOWN', spread=2)
             self.send_buttons('a')
+            self._driver.pause(2)
             self.send_buttons('b', spread=1)
             self.menu_reset(timeout=timeout)
         print("Menu reset has finished")
 
     def dashboard_reset(self, timeout=2):
         if self._driver.url() == 'https://www.xbox.com/en-US/play' or self._driver.url() != "https://www.xbox.com/en-US/play/launch/ark-ultimate-survivor-edition/9N5JRWWGMS1R":
             print("Dashboard reset has finished")
```

### Comparing `arkcloud-0.0.8/src/arkcloud/web/websites/gamepad_website.py` & `arkcloud-0.0.9/src/arkcloud/web/websites/gamepad_website.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud/web/websites/website.py` & `arkcloud-0.0.9/src/arkcloud/web/websites/website.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud/web/websites/xbox_controller_extension.py` & `arkcloud-0.0.9/src/arkcloud/web/websites/xbox_controller_extension.py`

 * *Files identical despite different names*

### Comparing `arkcloud-0.0.8/src/arkcloud.egg-info/PKG-INFO` & `arkcloud-0.0.9/src/arkcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arkcloud
-Version: 0.0.8
+Version: 0.0.9
 Summary: This application accesses the Ark system.
 Home-page: https://github.com/GameServerGurus/Ark-Cloud
 Author: Mauricio
 Author-email: dev.mauricio.lomeli@gmail.com
 Project-URL: Bug Tracker, https://github.com/GameServerGurus/Ark-Cloud/issues
 Platform: win32
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `arkcloud-0.0.8/src/arkcloud.egg-info/SOURCES.txt` & `arkcloud-0.0.9/src/arkcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

