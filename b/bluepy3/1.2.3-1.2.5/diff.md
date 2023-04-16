# Comparing `tmp/bluepy3-1.2.3.tar.gz` & `tmp/bluepy3-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluepy3-1.2.3.tar", last modified: Sun Apr 16 14:03:40 2023, max compression
+gzip compressed data, was "bluepy3-1.2.5.tar", last modified: Sun Apr 16 14:05:43 2023, max compression
```

## Comparing `bluepy3-1.2.3.tar` & `bluepy3-1.2.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-04-16 14:03:40.452681 bluepy3-1.2.3/
--rw-r--r--   0 maurice    (501) staff       (20)     1084 2023-03-04 17:28:46.000000 bluepy3-1.2.3/LICENSE
--rw-r--r--   0 maurice    (501) staff       (20)     5340 2023-04-16 14:03:40.452761 bluepy3-1.2.3/PKG-INFO
--rw-r--r--   0 maurice    (501) staff       (20)     3454 2023-04-10 10:16:14.000000 bluepy3-1.2.3/README.md
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-04-16 14:03:40.451662 bluepy3-1.2.3/bluepy3/
--rw-r--r--   0 maurice    (501) staff       (20)     1571 2023-04-09 13:50:23.000000 bluepy3-1.2.3/bluepy3/Makefile
--rwxr-xr-x   0 maurice    (501) staff       (20)      135 2023-03-26 10:53:06.000000 bluepy3-1.2.3/bluepy3/__init__.py
--rwxr-xr-x   0 maurice    (501) staff       (20)     4758 2023-04-16 14:01:33.000000 bluepy3-1.2.3/bluepy3/blescan.py
--rw-r--r--   0 maurice    (501) staff       (20)    58458 2023-03-26 11:03:50.000000 bluepy3-1.2.3/bluepy3/bluepy3-helper.c
--rwxr-xr-x   0 maurice    (501) staff       (20)    37221 2023-04-16 14:00:43.000000 bluepy3-1.2.3/bluepy3/btle.py
--rw-r--r--   0 maurice    (501) staff       (20)     4167 2023-03-26 10:58:24.000000 bluepy3-1.2.3/bluepy3/config.5.47.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-03-26 10:58:24.000000 bluepy3-1.2.3/bluepy3/config.5.50.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-03-26 10:58:24.000000 bluepy3-1.2.3/bluepy3/config.5.60.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-03-26 10:58:24.000000 bluepy3-1.2.3/bluepy3/config.5.66.h
--rwxr-xr-x   0 maurice    (501) staff       (20)     9750 2023-04-16 13:52:52.000000 bluepy3-1.2.3/bluepy3/get_services.py
--rwxr-xr-x   0 maurice    (501) staff       (20)      690 2023-03-26 10:53:06.000000 bluepy3-1.2.3/bluepy3/scan_fuzz.py
--rwxr-xr-x   0 maurice    (501) staff       (20)      454 2023-03-26 10:53:06.000000 bluepy3-1.2.3/bluepy3/scanner.py
--rwxr-xr-x   0 maurice    (501) staff       (20)    16627 2023-04-16 13:52:52.000000 bluepy3-1.2.3/bluepy3/sensortag.py
--rwxr-xr-x   0 maurice    (501) staff       (20)    34902 2023-04-16 13:52:53.000000 bluepy3-1.2.3/bluepy3/thingy52.py
--rw-r--r--   0 maurice    (501) staff       (20)    37880 2023-03-26 10:53:06.000000 bluepy3-1.2.3/bluepy3/uuids.json
--rw-r--r--   0 maurice    (501) staff       (20)      125 2023-03-08 11:49:00.000000 bluepy3-1.2.3/bluepy3/version.h
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-04-16 14:03:40.452564 bluepy3-1.2.3/bluepy3.egg-info/
--rw-r--r--   0 maurice    (501) staff       (20)     5340 2023-04-16 14:03:40.000000 bluepy3-1.2.3/bluepy3.egg-info/PKG-INFO
--rw-r--r--   0 maurice    (501) staff       (20)      521 2023-04-16 14:03:40.000000 bluepy3-1.2.3/bluepy3.egg-info/SOURCES.txt
--rw-r--r--   0 maurice    (501) staff       (20)        1 2023-04-16 14:03:40.000000 bluepy3-1.2.3/bluepy3.egg-info/dependency_links.txt
--rw-r--r--   0 maurice    (501) staff       (20)      117 2023-04-16 14:03:40.000000 bluepy3-1.2.3/bluepy3.egg-info/entry_points.txt
--rw-r--r--   0 maurice    (501) staff       (20)        8 2023-04-16 14:03:40.000000 bluepy3-1.2.3/bluepy3.egg-info/top_level.txt
--rw-r--r--   0 maurice    (501) staff       (20)       94 2023-04-16 14:03:40.453060 bluepy3-1.2.3/setup.cfg
--rw-r--r--   0 maurice    (501) staff       (20)     3340 2023-04-16 14:03:03.000000 bluepy3-1.2.3/setup.py
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-04-16 14:05:43.105247 bluepy3-1.2.5/
+-rw-r--r--   0 maurice    (501) staff       (20)     1084 2023-03-04 17:28:46.000000 bluepy3-1.2.5/LICENSE
+-rw-r--r--   0 maurice    (501) staff       (20)     5340 2023-04-16 14:05:43.105334 bluepy3-1.2.5/PKG-INFO
+-rw-r--r--   0 maurice    (501) staff       (20)     3454 2023-04-10 10:16:14.000000 bluepy3-1.2.5/README.md
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-04-16 14:05:43.104224 bluepy3-1.2.5/bluepy3/
+-rw-r--r--   0 maurice    (501) staff       (20)     1571 2023-04-09 13:50:23.000000 bluepy3-1.2.5/bluepy3/Makefile
+-rwxr-xr-x   0 maurice    (501) staff       (20)      135 2023-03-26 10:53:06.000000 bluepy3-1.2.5/bluepy3/__init__.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)     4758 2023-04-16 14:01:33.000000 bluepy3-1.2.5/bluepy3/blescan.py
+-rw-r--r--   0 maurice    (501) staff       (20)    58458 2023-03-26 11:03:50.000000 bluepy3-1.2.5/bluepy3/bluepy3-helper.c
+-rwxr-xr-x   0 maurice    (501) staff       (20)    37227 2023-04-16 14:04:38.000000 bluepy3-1.2.5/bluepy3/btle.py
+-rw-r--r--   0 maurice    (501) staff       (20)     4167 2023-03-26 10:58:24.000000 bluepy3-1.2.5/bluepy3/config.5.47.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-03-26 10:58:24.000000 bluepy3-1.2.5/bluepy3/config.5.50.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-03-26 10:58:24.000000 bluepy3-1.2.5/bluepy3/config.5.60.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-03-26 10:58:24.000000 bluepy3-1.2.5/bluepy3/config.5.66.h
+-rwxr-xr-x   0 maurice    (501) staff       (20)     9750 2023-04-16 13:52:52.000000 bluepy3-1.2.5/bluepy3/get_services.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)      690 2023-03-26 10:53:06.000000 bluepy3-1.2.5/bluepy3/scan_fuzz.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)      454 2023-03-26 10:53:06.000000 bluepy3-1.2.5/bluepy3/scanner.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)    16627 2023-04-16 13:52:52.000000 bluepy3-1.2.5/bluepy3/sensortag.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)    34902 2023-04-16 13:52:53.000000 bluepy3-1.2.5/bluepy3/thingy52.py
+-rw-r--r--   0 maurice    (501) staff       (20)    37880 2023-03-26 10:53:06.000000 bluepy3-1.2.5/bluepy3/uuids.json
+-rw-r--r--   0 maurice    (501) staff       (20)      125 2023-03-08 11:49:00.000000 bluepy3-1.2.5/bluepy3/version.h
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-04-16 14:05:43.105129 bluepy3-1.2.5/bluepy3.egg-info/
+-rw-r--r--   0 maurice    (501) staff       (20)     5340 2023-04-16 14:05:43.000000 bluepy3-1.2.5/bluepy3.egg-info/PKG-INFO
+-rw-r--r--   0 maurice    (501) staff       (20)      521 2023-04-16 14:05:43.000000 bluepy3-1.2.5/bluepy3.egg-info/SOURCES.txt
+-rw-r--r--   0 maurice    (501) staff       (20)        1 2023-04-16 14:05:43.000000 bluepy3-1.2.5/bluepy3.egg-info/dependency_links.txt
+-rw-r--r--   0 maurice    (501) staff       (20)      117 2023-04-16 14:05:43.000000 bluepy3-1.2.5/bluepy3.egg-info/entry_points.txt
+-rw-r--r--   0 maurice    (501) staff       (20)        8 2023-04-16 14:05:43.000000 bluepy3-1.2.5/bluepy3.egg-info/top_level.txt
+-rw-r--r--   0 maurice    (501) staff       (20)       94 2023-04-16 14:05:43.105614 bluepy3-1.2.5/setup.cfg
+-rw-r--r--   0 maurice    (501) staff       (20)     3340 2023-04-16 14:05:29.000000 bluepy3-1.2.5/setup.py
```

### Comparing `bluepy3-1.2.3/LICENSE` & `bluepy3-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.3/PKG-INFO` & `bluepy3-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepy3
-Version: 1.2.3
+Version: 1.2.5
 Summary: Python module for interfacing with BLE devices through Bluez
 Home-page: https://github.com/Mausy5043/bluepy3
 Download-URL: https://github.com/Mausy5043/bluepy3
 Author: mausy5043
 Keywords: Bluetooth,Bluetooth Smart,BLE,Bluetooth Low Energy,Raspberry Pi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bluepy3-1.2.3/README.md` & `bluepy3-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.3/bluepy3/Makefile` & `bluepy3-1.2.5/bluepy3/Makefile`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.3/bluepy3/blescan.py` & `bluepy3-1.2.5/bluepy3/blescan.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.3/bluepy3/bluepy3-helper.c` & `bluepy3-1.2.5/bluepy3/bluepy3-helper.c`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.3/bluepy3/btle.py` & `bluepy3-1.2.5/bluepy3/btle.py`

 * *Files 0% similar despite different names*

```diff
@@ -680,15 +680,15 @@
         if len(address.split(":")) != 6:
             raise ValueError(f"*** -btle- Expected MAC address, got {repr(address)}")
         if address_type not in (ADDR_TYPE_PUBLIC, ADDR_TYPE_RANDOM):
             raise ValueError(
                 f"*** -btle- Expected address type public or random, got {address_type}"
             )
         if isinstance(address, ScanEntry):
-            return self._setOOB(address.addr, address.addrType, oob_data, address.iface)
+            return self._setRemoteOOB(address.addr, address.addrType, oob_data, address.iface)
         elif address is not None:
             return self._setRemoteOOB(address, address_type, oob_data, iface)
 
     def getLocalOOB(self, iface=None):
         cmd = ""
         if self._helper is None:
             self._startHelper(iface)
```

### Comparing `bluepy3-1.2.3/bluepy3/config.5.47.h` & `bluepy3-1.2.5/bluepy3/config.5.47.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.3/bluepy3/config.5.50.h` & `bluepy3-1.2.5/bluepy3/config.5.50.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.3/bluepy3/config.5.60.h` & `bluepy3-1.2.5/bluepy3/config.5.60.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.3/bluepy3/config.5.66.h` & `bluepy3-1.2.5/bluepy3/config.5.66.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.3/bluepy3/get_services.py` & `bluepy3-1.2.5/bluepy3/get_services.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.3/bluepy3/scan_fuzz.py` & `bluepy3-1.2.5/bluepy3/scan_fuzz.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.3/bluepy3/sensortag.py` & `bluepy3-1.2.5/bluepy3/sensortag.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.3/bluepy3/thingy52.py` & `bluepy3-1.2.5/bluepy3/thingy52.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.3/bluepy3/uuids.json` & `bluepy3-1.2.5/bluepy3/uuids.json`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.3/bluepy3.egg-info/PKG-INFO` & `bluepy3-1.2.5/bluepy3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepy3
-Version: 1.2.3
+Version: 1.2.5
 Summary: Python module for interfacing with BLE devices through Bluez
 Home-page: https://github.com/Mausy5043/bluepy3
 Download-URL: https://github.com/Mausy5043/bluepy3
 Author: mausy5043
 Keywords: Bluetooth,Bluetooth Smart,BLE,Bluetooth Low Energy,Raspberry Pi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bluepy3-1.2.3/bluepy3.egg-info/SOURCES.txt` & `bluepy3-1.2.5/bluepy3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.3/setup.py` & `bluepy3-1.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import shlex
 import subprocess
 import sys
 
 from setuptools import setup
 from setuptools.command.build_py import build_py
 
-VERSION = "1.2.3"
+VERSION = "1.2.5"
 MAKEFILE = "bluepy3/Makefile"
 VERSION_FILE = "bluepy3/version.h"
 BLUEZ_VERSION = "(unknown)"
 
 
 def pre_install():
     """Do the custom compiling of the bluepy3-helper executable from the makefile"""
```

