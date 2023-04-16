# Comparing `tmp/bluepy3-1.2.1.tar.gz` & `tmp/bluepy3-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluepy3-1.2.1.tar", last modified: Mon Mar 27 14:27:24 2023, max compression
+gzip compressed data, was "bluepy3-1.2.2.tar", last modified: Sun Apr 16 07:53:41 2023, max compression
```

## Comparing `bluepy3-1.2.1.tar` & `bluepy3-1.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-03-27 14:27:24.944214 bluepy3-1.2.1/
--rw-r--r--   0 maurice    (501) staff       (20)     1084 2023-03-04 17:28:46.000000 bluepy3-1.2.1/LICENSE
--rw-r--r--   0 maurice    (501) staff       (20)     5344 2023-03-27 14:27:24.944295 bluepy3-1.2.1/PKG-INFO
--rw-r--r--   0 maurice    (501) staff       (20)     3458 2023-03-27 14:25:10.000000 bluepy3-1.2.1/README.md
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-03-27 14:27:24.943268 bluepy3-1.2.1/bluepy3/
--rw-r--r--   0 maurice    (501) staff       (20)     1571 2023-03-26 10:53:06.000000 bluepy3-1.2.1/bluepy3/Makefile
--rwxr-xr-x   0 maurice    (501) staff       (20)      135 2023-03-26 10:53:06.000000 bluepy3-1.2.1/bluepy3/__init__.py
--rwxr-xr-x   0 maurice    (501) staff       (20)     4720 2023-03-26 10:53:06.000000 bluepy3-1.2.1/bluepy3/blescan.py
--rw-r--r--   0 maurice    (501) staff       (20)    58458 2023-03-26 11:03:50.000000 bluepy3-1.2.1/bluepy3/bluepy3-helper.c
--rwxr-xr-x   0 maurice    (501) staff       (20)    36452 2023-03-26 10:54:03.000000 bluepy3-1.2.1/bluepy3/btle.py
--rw-r--r--   0 maurice    (501) staff       (20)     4167 2023-03-26 10:58:24.000000 bluepy3-1.2.1/bluepy3/config.5.47.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-03-26 10:58:24.000000 bluepy3-1.2.1/bluepy3/config.5.50.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-03-26 10:58:24.000000 bluepy3-1.2.1/bluepy3/config.5.60.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-03-26 10:58:24.000000 bluepy3-1.2.1/bluepy3/config.5.66.h
--rwxr-xr-x   0 maurice    (501) staff       (20)     9548 2023-03-26 10:53:06.000000 bluepy3-1.2.1/bluepy3/get_services.py
--rwxr-xr-x   0 maurice    (501) staff       (20)      690 2023-03-26 10:53:06.000000 bluepy3-1.2.1/bluepy3/scan_fuzz.py
--rwxr-xr-x   0 maurice    (501) staff       (20)      454 2023-03-26 10:53:06.000000 bluepy3-1.2.1/bluepy3/scanner.py
--rwxr-xr-x   0 maurice    (501) staff       (20)    16591 2023-03-26 10:53:06.000000 bluepy3-1.2.1/bluepy3/sensortag.py
--rwxr-xr-x   0 maurice    (501) staff       (20)    34320 2023-03-26 10:53:06.000000 bluepy3-1.2.1/bluepy3/thingy52.py
--rw-r--r--   0 maurice    (501) staff       (20)    37880 2023-03-26 10:53:06.000000 bluepy3-1.2.1/bluepy3/uuids.json
--rw-r--r--   0 maurice    (501) staff       (20)      125 2023-03-08 11:49:00.000000 bluepy3-1.2.1/bluepy3/version.h
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-03-27 14:27:24.944107 bluepy3-1.2.1/bluepy3.egg-info/
--rw-r--r--   0 maurice    (501) staff       (20)     5344 2023-03-27 14:27:24.000000 bluepy3-1.2.1/bluepy3.egg-info/PKG-INFO
--rw-r--r--   0 maurice    (501) staff       (20)      521 2023-03-27 14:27:24.000000 bluepy3-1.2.1/bluepy3.egg-info/SOURCES.txt
--rw-r--r--   0 maurice    (501) staff       (20)        1 2023-03-27 14:27:24.000000 bluepy3-1.2.1/bluepy3.egg-info/dependency_links.txt
--rw-r--r--   0 maurice    (501) staff       (20)      117 2023-03-27 14:27:24.000000 bluepy3-1.2.1/bluepy3.egg-info/entry_points.txt
--rw-r--r--   0 maurice    (501) staff       (20)        8 2023-03-27 14:27:24.000000 bluepy3-1.2.1/bluepy3.egg-info/top_level.txt
--rw-r--r--   0 maurice    (501) staff       (20)       94 2023-03-27 14:27:24.944621 bluepy3-1.2.1/setup.cfg
--rw-r--r--   0 maurice    (501) staff       (20)     3340 2023-03-27 14:26:49.000000 bluepy3-1.2.1/setup.py
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-04-16 07:53:41.987196 bluepy3-1.2.2/
+-rw-r--r--   0 maurice    (501) staff       (20)     1084 2023-03-04 17:28:46.000000 bluepy3-1.2.2/LICENSE
+-rw-r--r--   0 maurice    (501) staff       (20)     5340 2023-04-16 07:53:41.987288 bluepy3-1.2.2/PKG-INFO
+-rw-r--r--   0 maurice    (501) staff       (20)     3454 2023-04-10 10:16:14.000000 bluepy3-1.2.2/README.md
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-04-16 07:53:41.986204 bluepy3-1.2.2/bluepy3/
+-rw-r--r--   0 maurice    (501) staff       (20)     1571 2023-04-09 13:50:23.000000 bluepy3-1.2.2/bluepy3/Makefile
+-rwxr-xr-x   0 maurice    (501) staff       (20)      135 2023-03-26 10:53:06.000000 bluepy3-1.2.2/bluepy3/__init__.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)     4720 2023-03-26 10:53:06.000000 bluepy3-1.2.2/bluepy3/blescan.py
+-rw-r--r--   0 maurice    (501) staff       (20)    58458 2023-03-26 11:03:50.000000 bluepy3-1.2.2/bluepy3/bluepy3-helper.c
+-rwxr-xr-x   0 maurice    (501) staff       (20)    36451 2023-04-16 06:58:01.000000 bluepy3-1.2.2/bluepy3/btle.py
+-rw-r--r--   0 maurice    (501) staff       (20)     4167 2023-03-26 10:58:24.000000 bluepy3-1.2.2/bluepy3/config.5.47.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-03-26 10:58:24.000000 bluepy3-1.2.2/bluepy3/config.5.50.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-03-26 10:58:24.000000 bluepy3-1.2.2/bluepy3/config.5.60.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-03-26 10:58:24.000000 bluepy3-1.2.2/bluepy3/config.5.66.h
+-rwxr-xr-x   0 maurice    (501) staff       (20)     9548 2023-03-26 10:53:06.000000 bluepy3-1.2.2/bluepy3/get_services.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)      690 2023-03-26 10:53:06.000000 bluepy3-1.2.2/bluepy3/scan_fuzz.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)      454 2023-03-26 10:53:06.000000 bluepy3-1.2.2/bluepy3/scanner.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)    16591 2023-03-26 10:53:06.000000 bluepy3-1.2.2/bluepy3/sensortag.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)    34320 2023-03-26 10:53:06.000000 bluepy3-1.2.2/bluepy3/thingy52.py
+-rw-r--r--   0 maurice    (501) staff       (20)    37880 2023-03-26 10:53:06.000000 bluepy3-1.2.2/bluepy3/uuids.json
+-rw-r--r--   0 maurice    (501) staff       (20)      125 2023-03-08 11:49:00.000000 bluepy3-1.2.2/bluepy3/version.h
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-04-16 07:53:41.987089 bluepy3-1.2.2/bluepy3.egg-info/
+-rw-r--r--   0 maurice    (501) staff       (20)     5340 2023-04-16 07:53:41.000000 bluepy3-1.2.2/bluepy3.egg-info/PKG-INFO
+-rw-r--r--   0 maurice    (501) staff       (20)      521 2023-04-16 07:53:41.000000 bluepy3-1.2.2/bluepy3.egg-info/SOURCES.txt
+-rw-r--r--   0 maurice    (501) staff       (20)        1 2023-04-16 07:53:41.000000 bluepy3-1.2.2/bluepy3.egg-info/dependency_links.txt
+-rw-r--r--   0 maurice    (501) staff       (20)      117 2023-04-16 07:53:41.000000 bluepy3-1.2.2/bluepy3.egg-info/entry_points.txt
+-rw-r--r--   0 maurice    (501) staff       (20)        8 2023-04-16 07:53:41.000000 bluepy3-1.2.2/bluepy3.egg-info/top_level.txt
+-rw-r--r--   0 maurice    (501) staff       (20)       94 2023-04-16 07:53:41.987584 bluepy3-1.2.2/setup.cfg
+-rw-r--r--   0 maurice    (501) staff       (20)     3340 2023-04-16 07:53:13.000000 bluepy3-1.2.2/setup.py
```

### Comparing `bluepy3-1.2.1/LICENSE` & `bluepy3-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.1/PKG-INFO` & `bluepy3-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepy3
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python module for interfacing with BLE devices through Bluez
 Home-page: https://github.com/Mausy5043/bluepy3
 Download-URL: https://github.com/Mausy5043/bluepy3
 Author: mausy5043
 Keywords: Bluetooth,Bluetooth Smart,BLE,Bluetooth Low Energy,Raspberry Pi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,15 @@
 Classifier: Topic :: Home Automation
 Requires-Python: >=3.7
 License-File: LICENSE
 
 # bluepy3
 
 [![PyPI version](https://img.shields.io/pypi/v/bluepy3.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/bluepy3)
-[![Supported Python versions](https://img.shields.io/pypi/pyversions/bluepy3.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/bluepy3)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/bluepy3?logo=python&logoColor=FFE873)](https://pypi.org/project/bluepy3)
 [![PyPI downloads](https://img.shields.io/pypi/dm/bluepy3.svg)](https://pypistats.org/packages/bluepy3)
 [![Code style: Black](https://img.shields.io/badge/code%20style-Black-000000.svg)](https://github.com/psf/black)
 
 This is a Python3 library to allow communication with Bluetooth Low Energy devices on Linux.
 
 ###### Note: If you are reading this on [PyPi](https://pypi.org/project/bluepy3/) then note that the formatting below looks terrible. Visit the project's homepage to read the correctly formatted [README.md](https://github.com/Mausy5043/bluepy3#readme) file.
```

### Comparing `bluepy3-1.2.1/README.md` & `bluepy3-1.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # bluepy3
 
 [![PyPI version](https://img.shields.io/pypi/v/bluepy3.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/bluepy3)
-[![Supported Python versions](https://img.shields.io/pypi/pyversions/bluepy3.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/bluepy3)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/bluepy3?logo=python&logoColor=FFE873)](https://pypi.org/project/bluepy3)
 [![PyPI downloads](https://img.shields.io/pypi/dm/bluepy3.svg)](https://pypistats.org/packages/bluepy3)
 [![Code style: Black](https://img.shields.io/badge/code%20style-Black-000000.svg)](https://github.com/psf/black)
 
 This is a Python3 library to allow communication with Bluetooth Low Energy devices on Linux.
 
 ###### Note: If you are reading this on [PyPi](https://pypi.org/project/bluepy3/) then note that the formatting below looks terrible. Visit the project's homepage to read the correctly formatted [README.md](https://github.com/Mausy5043/bluepy3#readme) file.
```

### Comparing `bluepy3-1.2.1/bluepy3/Makefile` & `bluepy3-1.2.2/bluepy3/Makefile`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.1/bluepy3/blescan.py` & `bluepy3-1.2.2/bluepy3/blescan.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.1/bluepy3/bluepy3-helper.c` & `bluepy3-1.2.2/bluepy3/bluepy3-helper.c`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.1/bluepy3/btle.py` & `bluepy3-1.2.2/bluepy3/btle.py`

 * *Files 0% similar despite different names*

```diff
@@ -459,15 +459,15 @@
                 if self.delegate is not None:
                     self.delegate.handleNotification(hnd, data)
             if respType not in wantType:
                 continue
             return resp
 
     def _connect(self, addr, addrType=ADDR_TYPE_PUBLIC, iface=None, timeout=BTLE_TIMEOUT):
-        max_retries = 10
+        max_retries = 5
         if len(addr.split(":")) != 6:
             raise ValueError(f"*** -btle- Expected MAC address, got {repr(addr)}")
         if addrType not in (ADDR_TYPE_PUBLIC, ADDR_TYPE_RANDOM):
             raise ValueError(f"*** -btle- Expected address type public or random, got {addrType}")
         self.retries = max_retries
         while self.retries > 0:
             self._startHelper(iface)
```

### Comparing `bluepy3-1.2.1/bluepy3/config.5.47.h` & `bluepy3-1.2.2/bluepy3/config.5.47.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.1/bluepy3/config.5.50.h` & `bluepy3-1.2.2/bluepy3/config.5.50.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.1/bluepy3/config.5.60.h` & `bluepy3-1.2.2/bluepy3/config.5.60.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.1/bluepy3/config.5.66.h` & `bluepy3-1.2.2/bluepy3/config.5.66.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.1/bluepy3/get_services.py` & `bluepy3-1.2.2/bluepy3/get_services.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.1/bluepy3/scan_fuzz.py` & `bluepy3-1.2.2/bluepy3/scan_fuzz.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.1/bluepy3/sensortag.py` & `bluepy3-1.2.2/bluepy3/sensortag.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.1/bluepy3/thingy52.py` & `bluepy3-1.2.2/bluepy3/thingy52.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.1/bluepy3/uuids.json` & `bluepy3-1.2.2/bluepy3/uuids.json`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.1/bluepy3.egg-info/PKG-INFO` & `bluepy3-1.2.2/bluepy3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepy3
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python module for interfacing with BLE devices through Bluez
 Home-page: https://github.com/Mausy5043/bluepy3
 Download-URL: https://github.com/Mausy5043/bluepy3
 Author: mausy5043
 Keywords: Bluetooth,Bluetooth Smart,BLE,Bluetooth Low Energy,Raspberry Pi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -17,15 +17,15 @@
 Classifier: Topic :: Home Automation
 Requires-Python: >=3.7
 License-File: LICENSE
 
 # bluepy3
 
 [![PyPI version](https://img.shields.io/pypi/v/bluepy3.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/bluepy3)
-[![Supported Python versions](https://img.shields.io/pypi/pyversions/bluepy3.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/bluepy3)
+[![Supported Python versions](https://img.shields.io/pypi/pyversions/bluepy3?logo=python&logoColor=FFE873)](https://pypi.org/project/bluepy3)
 [![PyPI downloads](https://img.shields.io/pypi/dm/bluepy3.svg)](https://pypistats.org/packages/bluepy3)
 [![Code style: Black](https://img.shields.io/badge/code%20style-Black-000000.svg)](https://github.com/psf/black)
 
 This is a Python3 library to allow communication with Bluetooth Low Energy devices on Linux.
 
 ###### Note: If you are reading this on [PyPi](https://pypi.org/project/bluepy3/) then note that the formatting below looks terrible. Visit the project's homepage to read the correctly formatted [README.md](https://github.com/Mausy5043/bluepy3#readme) file.
```

### Comparing `bluepy3-1.2.1/bluepy3.egg-info/SOURCES.txt` & `bluepy3-1.2.2/bluepy3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluepy3-1.2.1/setup.py` & `bluepy3-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import shlex
 import subprocess
 import sys
 
 from setuptools import setup
 from setuptools.command.build_py import build_py
 
-VERSION = "1.2.1"
+VERSION = "1.2.2"
 MAKEFILE = "bluepy3/Makefile"
 VERSION_FILE = "bluepy3/version.h"
 BLUEZ_VERSION = "(unknown)"
 
 
 def pre_install():
     """Do the custom compiling of the bluepy3-helper executable from the makefile"""
```

