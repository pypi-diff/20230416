# Comparing `tmp/aqualogic-3.3.tar.gz` & `tmp/aqualogic-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqualogic-3.3.tar", last modified: Tue Jul  6 23:19:55 2021, max compression
+gzip compressed data, was "aqualogic-3.4.tar", last modified: Sun Apr 16 14:17:42 2023, max compression
```

## Comparing `aqualogic-3.3.tar` & `aqualogic-3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 swilson    (501) staff       (20)        0 2021-07-06 23:19:55.392618 aqualogic-3.3/
--rw-r--r--   0 swilson    (501) staff       (20)       53 2021-07-06 23:16:31.000000 aqualogic-3.3/MANIFEST.in
--rw-r--r--   0 swilson    (501) staff       (20)     1024 2021-07-06 23:19:55.392848 aqualogic-3.3/PKG-INFO
--rw-r--r--   0 swilson    (501) staff       (20)     1356 2021-07-06 19:24:57.000000 aqualogic-3.3/README.md
-drwxr-xr-x   0 swilson    (501) staff       (20)        0 2021-07-06 23:19:55.390728 aqualogic-3.3/aqualogic/
--rw-r--r--   0 swilson    (501) staff       (20)        0 2021-07-06 20:20:04.000000 aqualogic-3.3/aqualogic/__init__.py
--rw-r--r--   0 swilson    (501) staff       (20)     1359 2021-07-06 20:23:19.000000 aqualogic-3.3/aqualogic/cli.py
--rw-r--r--   0 swilson    (501) staff       (20)    22205 2021-07-06 22:54:27.000000 aqualogic-3.3/aqualogic/core.py
--rw-r--r--   0 swilson    (501) staff       (20)      791 2021-07-06 17:30:20.000000 aqualogic-3.3/aqualogic/keys.py
--rw-r--r--   0 swilson    (501) staff       (20)      852 2021-07-06 17:28:46.000000 aqualogic-3.3/aqualogic/states.py
--rw-r--r--   0 swilson    (501) staff       (20)     1399 2021-07-06 19:08:13.000000 aqualogic-3.3/aqualogic/web.html
--rw-r--r--   0 swilson    (501) staff       (20)     2529 2021-07-06 23:10:13.000000 aqualogic-3.3/aqualogic/web.py
-drwxr-xr-x   0 swilson    (501) staff       (20)        0 2021-07-06 23:19:55.392254 aqualogic-3.3/aqualogic.egg-info/
--rw-r--r--   0 swilson    (501) staff       (20)     1024 2021-07-06 23:19:55.000000 aqualogic-3.3/aqualogic.egg-info/PKG-INFO
--rw-r--r--   0 swilson    (501) staff       (20)      335 2021-07-06 23:19:55.000000 aqualogic-3.3/aqualogic.egg-info/SOURCES.txt
--rw-r--r--   0 swilson    (501) staff       (20)        1 2021-07-06 23:19:55.000000 aqualogic-3.3/aqualogic.egg-info/dependency_links.txt
--rw-r--r--   0 swilson    (501) staff       (20)       20 2021-07-06 23:19:55.000000 aqualogic-3.3/aqualogic.egg-info/requires.txt
--rw-r--r--   0 swilson    (501) staff       (20)       10 2021-07-06 23:19:55.000000 aqualogic-3.3/aqualogic.egg-info/top_level.txt
--rw-r--r--   0 swilson    (501) staff       (20)       79 2021-07-06 23:19:55.393609 aqualogic-3.3/setup.cfg
--rwxr-xr-x   0 swilson    (501) staff       (20)     1406 2021-07-06 23:19:13.000000 aqualogic-3.3/setup.py
+drwxr-xr-x   0 swilson    (501) staff       (20)        0 2023-04-16 14:17:42.276963 aqualogic-3.4/
+-rw-r--r--   0 swilson    (501) staff       (20)     1068 2023-04-16 13:49:50.000000 aqualogic-3.4/LICENSE.txt
+-rw-r--r--   0 swilson    (501) staff       (20)       26 2023-04-16 14:13:12.000000 aqualogic-3.4/MANIFEST.in
+-rw-r--r--   0 swilson    (501) staff       (20)     1020 2023-04-16 14:17:42.277010 aqualogic-3.4/PKG-INFO
+-rw-r--r--   0 swilson    (501) staff       (20)     1356 2023-04-16 13:49:50.000000 aqualogic-3.4/README.md
+drwxr-xr-x   0 swilson    (501) staff       (20)        0 2023-04-16 14:17:42.276216 aqualogic-3.4/aqualogic/
+-rw-r--r--   0 swilson    (501) staff       (20)        0 2023-04-16 13:49:50.000000 aqualogic-3.4/aqualogic/__init__.py
+-rw-r--r--   0 swilson    (501) staff       (20)     1359 2023-04-16 13:49:50.000000 aqualogic-3.4/aqualogic/cli.py
+-rw-r--r--   0 swilson    (501) staff       (20)    22205 2023-04-16 13:49:50.000000 aqualogic-3.4/aqualogic/core.py
+-rw-r--r--   0 swilson    (501) staff       (20)      791 2023-04-16 13:49:50.000000 aqualogic-3.4/aqualogic/keys.py
+-rw-r--r--   0 swilson    (501) staff       (20)      852 2023-04-16 13:49:50.000000 aqualogic-3.4/aqualogic/states.py
+-rw-r--r--   0 swilson    (501) staff       (20)     2475 2023-04-16 14:13:12.000000 aqualogic-3.4/aqualogic/web.py
+drwxr-xr-x   0 swilson    (501) staff       (20)        0 2023-04-16 14:17:42.276875 aqualogic-3.4/aqualogic.egg-info/
+-rw-r--r--   0 swilson    (501) staff       (20)     1020 2023-04-16 14:17:42.000000 aqualogic-3.4/aqualogic.egg-info/PKG-INFO
+-rw-r--r--   0 swilson    (501) staff       (20)      328 2023-04-16 14:17:42.000000 aqualogic-3.4/aqualogic.egg-info/SOURCES.txt
+-rw-r--r--   0 swilson    (501) staff       (20)        1 2023-04-16 14:17:42.000000 aqualogic-3.4/aqualogic.egg-info/dependency_links.txt
+-rw-r--r--   0 swilson    (501) staff       (20)       28 2023-04-16 14:17:42.000000 aqualogic-3.4/aqualogic.egg-info/requires.txt
+-rw-r--r--   0 swilson    (501) staff       (20)       10 2023-04-16 14:17:42.000000 aqualogic-3.4/aqualogic.egg-info/top_level.txt
+-rw-r--r--   0 swilson    (501) staff       (20)       79 2023-04-16 14:17:42.277220 aqualogic-3.4/setup.cfg
+-rwxr-xr-x   0 swilson    (501) staff       (20)     1381 2023-04-16 14:16:47.000000 aqualogic-3.4/setup.py
```

### Comparing `aqualogic-3.3/PKG-INFO` & `aqualogic-3.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: aqualogic
-Version: 3.3
+Version: 3.4
 Summary: Library for interfacing with a Hayward/Goldline AquaLogic/ProLogic pool controller.
 Home-page: https://github.com/swilson/aqualogic
 Author: Sean Wilson
 Author-email: sean.wilson@live.ca
 License: MIT
-Description: A python library to interface with Hayward/Goldline AquaLogic/ProLogic pool controllers. Note that the Goldline protocol uses RS-485 so a hardware interface that can provide the library with reader and writer file objects is required. The simplest solution for this is an RS-485 to Ethernet adapter connected via a socket.
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
+License-File: LICENSE.txt
+
+A python library to interface with Hayward/Goldline AquaLogic/ProLogic pool controllers. Note that the Goldline protocol uses RS-485 so a hardware interface that can provide the library with reader and writer file objects is required. The simplest solution for this is an RS-485 to Ethernet adapter connected via a socket.
```

### Comparing `aqualogic-3.3/README.md` & `aqualogic-3.4/README.md`

 * *Files identical despite different names*

### Comparing `aqualogic-3.3/aqualogic/cli.py` & `aqualogic-3.4/aqualogic/cli.py`

 * *Files identical despite different names*

### Comparing `aqualogic-3.3/aqualogic/core.py` & `aqualogic-3.4/aqualogic/core.py`

 * *Files identical despite different names*

### Comparing `aqualogic-3.3/aqualogic/keys.py` & `aqualogic-3.4/aqualogic/keys.py`

 * *Files identical despite different names*

### Comparing `aqualogic-3.3/aqualogic/states.py` & `aqualogic-3.4/aqualogic/states.py`

 * *Files identical despite different names*

### Comparing `aqualogic-3.3/aqualogic/web.py` & `aqualogic-3.4/aqualogic/web.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 import aiohttp
 import socketserver
 import socket
 import asyncio
 import websockets
 import threading
 import logging
-import os
 
 from .keys import Keys
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class WebServer():
     def __init__(self, panel):
-        self._loop = asyncio.new_event_loop()
         self._panel = panel
-        self._msg_queue = asyncio.Queue(loop=self._loop)
+        self._msg_queue = asyncio.Queue()
 
     def _run_thread(self):
         asyncio.set_event_loop(self._loop)
         try:
             self._loop.run_forever()
         except KeyboardInterrupt:
             pass
 
     def start(self, port):
+        self._loop = asyncio.get_event_loop()
+
         # Set up the HTTP server
         app = web.Application()
         
         app.router.add_get('/', self._root_handler)
         app.router.add_get('/ws', self._websocket_handler)
 
         runner = web.AppRunner(app)
@@ -44,15 +44,15 @@
         t = threading.Thread(target=self._run_thread)
         t.start();
 
     def text_updated(self, text):
         self._loop.call_soon_threadsafe(self._msg_queue.put_nowait, text)
 
     async def _root_handler(self, request):
-        s = open(os.path.join(os.path.dirname(__file__), 'web.html'), 'r')
+        s = open('aqualogic/web.html', 'r')
         return web.Response(text=s.read(), content_type='text/html')
 
     async def _websocket_handler(self, request):
         # Websocket handler for providing the live data
         ws = aiohttp.web.WebSocketResponse()
         await ws.prepare(request)
         _LOGGER.info('Websocket connection ready')
@@ -74,12 +74,11 @@
             try:
                 key = Keys[msg.data]
                 self._panel.send_key(key)
             except KeyError:
                 _LOGGER.info('Invalid key name {}'.format(msg.data))
 
     async def _producer_handler(self, ws):
-        while True:
+        while not ws.closed:
             text = await self._msg_queue.get()
-            if ws.closed:
-                break
             await ws.send_str(text)
+            self._msg_queue.task_done()
```

### Comparing `aqualogic-3.3/aqualogic.egg-info/PKG-INFO` & `aqualogic-3.4/aqualogic.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: aqualogic
-Version: 3.3
+Version: 3.4
 Summary: Library for interfacing with a Hayward/Goldline AquaLogic/ProLogic pool controller.
 Home-page: https://github.com/swilson/aqualogic
 Author: Sean Wilson
 Author-email: sean.wilson@live.ca
 License: MIT
-Description: A python library to interface with Hayward/Goldline AquaLogic/ProLogic pool controllers. Note that the Goldline protocol uses RS-485 so a hardware interface that can provide the library with reader and writer file objects is required. The simplest solution for this is an RS-485 to Ethernet adapter connected via a socket.
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
+License-File: LICENSE.txt
+
+A python library to interface with Hayward/Goldline AquaLogic/ProLogic pool controllers. Note that the Goldline protocol uses RS-485 so a hardware interface that can provide the library with reader and writer file objects is required. The simplest solution for this is an RS-485 to Ethernet adapter connected via a socket.
```

### Comparing `aqualogic-3.3/setup.py` & `aqualogic-3.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 setup(
   name = 'aqualogic',
   packages = ['aqualogic'], # this must be the same as the name above
-  version = '3.3',
+  version = '3.4',
   description = 'Library for interfacing with a Hayward/Goldline AquaLogic/ProLogic pool controller.',
   long_description = 'A python library to interface with Hayward/Goldline AquaLogic/ProLogic pool controllers. Note that the Goldline protocol uses RS-485 so a hardware interface that can provide the library with reader and writer file objects is required. The simplest solution for this is an RS-485 to Ethernet adapter connected via a socket.',
   author = 'Sean Wilson',
   author_email = 'sean.wilson@live.ca',
   url = 'https://github.com/swilson/aqualogic',
   license='MIT',
   classifiers=[
@@ -24,12 +24,10 @@
 
       'Programming Language :: Python :: 3',
       'Programming Language :: Python :: 3.2',
       'Programming Language :: Python :: 3.3',
       'Programming Language :: Python :: 3.4',
   ],
   install_requires=[
-    'pyserial',
-    'websockets',
-  ],
-  include_package_data = True
+    'pyserial',"aiohttp","websockets"
+  ]  
 )
```

