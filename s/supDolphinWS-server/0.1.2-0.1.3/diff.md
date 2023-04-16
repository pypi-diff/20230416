# Comparing `tmp/supDolphinWS-server-0.1.2.tar.gz` & `tmp/supDolphinWS-server-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "supDolphinWS-server-0.1.2.tar", last modified: Mon Mar 27 14:54:10 2023, max compression
+gzip compressed data, was "supDolphinWS-server-0.1.3.tar", last modified: Sun Apr 16 10:21:08 2023, max compression
```

## Comparing `supDolphinWS-server-0.1.2.tar` & `supDolphinWS-server-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 14:54:10.932992 supDolphinWS-server-0.1.2/
--rw-rw-rw-   0        0        0     1083 2023-03-09 06:55:01.000000 supDolphinWS-server-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1090 2023-03-27 14:54:10.933992 supDolphinWS-server-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      506 2023-03-09 08:50:19.000000 supDolphinWS-server-0.1.2/README.md
--rw-rw-rw-   0        0        0       88 2022-10-14 08:59:04.000000 supDolphinWS-server-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0      787 2023-03-27 14:54:10.933992 supDolphinWS-server-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-27 14:54:10.922085 supDolphinWS-server-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-03-27 14:54:10.925044 supDolphinWS-server-0.1.2/src/supDolphinWS/
--rw-rw-rw-   0        0        0        0 2023-03-09 08:41:58.000000 supDolphinWS-server-0.1.2/src/supDolphinWS/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 14:54:10.929044 supDolphinWS-server-0.1.2/src/supDolphinWS/server/
--rw-rw-rw-   0        0        0        0 2023-03-09 06:00:58.000000 supDolphinWS-server-0.1.2/src/supDolphinWS/server/__init__.py
--rw-rw-rw-   0        0        0      892 2023-03-09 07:01:56.000000 supDolphinWS-server-0.1.2/src/supDolphinWS/server/__main__.py
--rw-rw-rw-   0        0        0     1665 2023-03-09 06:55:45.000000 supDolphinWS-server-0.1.2/src/supDolphinWS/server/api.py
--rw-rw-rw-   0        0        0     2703 2023-03-27 14:53:44.000000 supDolphinWS-server-0.1.2/src/supDolphinWS/server/dolphin.py
--rw-rw-rw-   0        0        0      335 2023-03-09 06:55:48.000000 supDolphinWS-server-0.1.2/src/supDolphinWS/server/err.py
--rw-rw-rw-   0        0        0     1352 2023-03-09 07:03:53.000000 supDolphinWS-server-0.1.2/src/supDolphinWS/server/server.py
--rw-rw-rw-   0        0        0      341 2023-03-09 06:55:57.000000 supDolphinWS-server-0.1.2/src/supDolphinWS/server/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-27 14:54:10.932992 supDolphinWS-server-0.1.2/src/supDolphinWS_server.egg-info/
--rw-rw-rw-   0        0        0     1090 2023-03-27 14:54:10.000000 supDolphinWS-server-0.1.2/src/supDolphinWS_server.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      541 2023-03-27 14:54:10.000000 supDolphinWS-server-0.1.2/src/supDolphinWS_server.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 14:54:10.000000 supDolphinWS-server-0.1.2/src/supDolphinWS_server.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-03-27 14:54:10.000000 supDolphinWS-server-0.1.2/src/supDolphinWS_server.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-27 14:54:10.000000 supDolphinWS-server-0.1.2/src/supDolphinWS_server.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 10:21:08.989020 supDolphinWS-server-0.1.3/
+-rw-rw-rw-   0        0        0     1410 2023-04-16 09:43:35.000000 supDolphinWS-server-0.1.3/3RD-PARTY-LICENSE.txt
+-rw-rw-rw-   0        0        0     1083 2023-03-09 06:55:01.000000 supDolphinWS-server-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1090 2023-04-16 10:21:08.989020 supDolphinWS-server-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      506 2023-03-09 08:50:19.000000 supDolphinWS-server-0.1.3/README.md
+-rw-rw-rw-   0        0        0       88 2022-10-14 08:59:04.000000 supDolphinWS-server-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      787 2023-04-16 10:21:08.989020 supDolphinWS-server-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 10:21:08.977003 supDolphinWS-server-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 10:21:08.981001 supDolphinWS-server-0.1.3/src/supDolphinWS/
+-rw-rw-rw-   0        0        0        0 2023-03-09 08:41:58.000000 supDolphinWS-server-0.1.3/src/supDolphinWS/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 10:21:08.985020 supDolphinWS-server-0.1.3/src/supDolphinWS/server/
+-rw-rw-rw-   0        0        0        0 2023-03-09 06:00:58.000000 supDolphinWS-server-0.1.3/src/supDolphinWS/server/__init__.py
+-rw-rw-rw-   0        0        0      892 2023-03-09 07:01:56.000000 supDolphinWS-server-0.1.3/src/supDolphinWS/server/__main__.py
+-rw-rw-rw-   0        0        0     1665 2023-03-09 06:55:45.000000 supDolphinWS-server-0.1.3/src/supDolphinWS/server/api.py
+-rw-rw-rw-   0        0        0     3119 2023-04-16 09:48:33.000000 supDolphinWS-server-0.1.3/src/supDolphinWS/server/dolphin.py
+-rw-rw-rw-   0        0        0      335 2023-03-09 06:55:48.000000 supDolphinWS-server-0.1.3/src/supDolphinWS/server/err.py
+-rw-rw-rw-   0        0        0     3470 2023-04-16 09:51:23.000000 supDolphinWS-server-0.1.3/src/supDolphinWS/server/memory_windows.py
+-rw-rw-rw-   0        0        0     1352 2023-03-09 07:03:53.000000 supDolphinWS-server-0.1.3/src/supDolphinWS/server/server.py
+-rw-rw-rw-   0        0        0      341 2023-03-09 06:55:57.000000 supDolphinWS-server-0.1.3/src/supDolphinWS/server/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-16 10:21:08.988021 supDolphinWS-server-0.1.3/src/supDolphinWS_server.egg-info/
+-rw-rw-rw-   0        0        0     1090 2023-04-16 10:21:08.000000 supDolphinWS-server-0.1.3/src/supDolphinWS_server.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      605 2023-04-16 10:21:08.000000 supDolphinWS-server-0.1.3/src/supDolphinWS_server.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 10:21:08.000000 supDolphinWS-server-0.1.3/src/supDolphinWS_server.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-16 10:21:08.000000 supDolphinWS-server-0.1.3/src/supDolphinWS_server.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-16 10:21:08.000000 supDolphinWS-server-0.1.3/src/supDolphinWS_server.egg-info/top_level.txt
```

### Comparing `supDolphinWS-server-0.1.2/LICENSE` & `supDolphinWS-server-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `supDolphinWS-server-0.1.2/PKG-INFO` & `supDolphinWS-server-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supDolphinWS-server
-Version: 0.1.2
+Version: 0.1.3
 Summary: A WebSocket server for accessing memory of emulated games in Dolphin
 Home-page: https://github.com/sup39/supDolphinWS-server
 Author: sup39
 Author-email: sms@sup39.dev
 License: MIT
 Project-URL: Bug Tracker, https://github.com/sup39/supDolphinWS-server/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `supDolphinWS-server-0.1.2/src/supDolphinWS/server/__main__.py` & `supDolphinWS-server-0.1.3/src/supDolphinWS/server/__main__.py`

 * *Files identical despite different names*

### Comparing `supDolphinWS-server-0.1.2/src/supDolphinWS/server/api.py` & `supDolphinWS-server-0.1.3/src/supDolphinWS/server/api.py`

 * *Files identical despite different names*

### Comparing `supDolphinWS-server-0.1.2/src/supDolphinWS/server/dolphin.py` & `supDolphinWS-server-0.1.3/src/supDolphinWS/server/dolphin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,47 @@
 # SPDX-License-Identifier: MIT
 # Copyright (c) 2023 sup39
 import os
 import psutil
 import struct
 from multiprocessing.shared_memory import SharedMemory
 
+if os.name == 'nt':
+  from .memory_windows import try_get_memory as try_get_memory_direct
+else:
+  try_get_memory_direct = None
+
 MEM1_START = 0x80000000
 MEM1_END   = 0x81800000
 MEM2_START = 0x90000000
 MEM2_END   = 0x94000000
 MEM2_OFFSET = 0x4040000
 
 dolphinProcNames = \
   {'Dolphin.exe', 'DolphinQt2.exe', 'DolphinWx.exe'} if os.name == 'nt' \
   else {'dolphin-emu', 'dolphin-emu-qt2', 'dolphin-emu-wx'}
 
 def try_get_memory(pid):
-  try: return SharedMemory('dolphin-emu.'+str(pid))
-  except FileNotFoundError: return None
+  # newer Dolphin => SharedMemory
+  try:
+    return SharedMemory('dolphin-emu.'+str(pid))
+  except FileNotFoundError: pass
+  # old Dolphin (on windows) => direct memory access via win32 api
+  if try_get_memory_direct:
+    try:
+      return try_get_memory_direct(pid)
+    except:
+      import traceback
+      print(traceback.format_exc())
 
 def find_memory(exclude_pid={}):
   try: return next(
     (p.pid, m)
     for p in psutil.process_iter(['pid', 'name'])
-    if p.pid not in exclude_pid and p.name() in dolphinProcNames
+    if p.pid not in exclude_pid and p.name() in dolphinProcNames and p.status() == 'running'
     for m in [try_get_memory(p.pid)]
     if m is not None
   )
   except StopIteration: return None
 
 class Dolphin():
   def __init__(self):
```

### Comparing `supDolphinWS-server-0.1.2/src/supDolphinWS/server/server.py` & `supDolphinWS-server-0.1.3/src/supDolphinWS/server/server.py`

 * *Files identical despite different names*

### Comparing `supDolphinWS-server-0.1.2/src/supDolphinWS_server.egg-info/PKG-INFO` & `supDolphinWS-server-0.1.3/src/supDolphinWS_server.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: supDolphinWS-server
-Version: 0.1.2
+Version: 0.1.3
 Summary: A WebSocket server for accessing memory of emulated games in Dolphin
 Home-page: https://github.com/sup39/supDolphinWS-server
 Author: sup39
 Author-email: sms@sup39.dev
 License: MIT
 Project-URL: Bug Tracker, https://github.com/sup39/supDolphinWS-server/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `supDolphinWS-server-0.1.2/src/supDolphinWS_server.egg-info/SOURCES.txt` & `supDolphinWS-server-0.1.3/src/supDolphinWS_server.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+3RD-PARTY-LICENSE.txt
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/supDolphinWS/__init__.py
 src/supDolphinWS/server/__init__.py
 src/supDolphinWS/server/__main__.py
 src/supDolphinWS/server/api.py
 src/supDolphinWS/server/dolphin.py
 src/supDolphinWS/server/err.py
+src/supDolphinWS/server/memory_windows.py
 src/supDolphinWS/server/server.py
 src/supDolphinWS/server/utils.py
 src/supDolphinWS_server.egg-info/PKG-INFO
 src/supDolphinWS_server.egg-info/SOURCES.txt
 src/supDolphinWS_server.egg-info/dependency_links.txt
 src/supDolphinWS_server.egg-info/requires.txt
 src/supDolphinWS_server.egg-info/top_level.txt
```

