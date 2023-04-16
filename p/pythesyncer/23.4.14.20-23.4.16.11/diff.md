# Comparing `tmp/pythesyncer-23.4.14.20.tar.gz` & `tmp/pythesyncer-23.4.16.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pythesyncer-23.4.14.20.tar", last modified: Fri Apr 14 12:25:41 2023, max compression
+gzip compressed data, was "dist/pythesyncer-23.4.16.11.tar", last modified: Sun Apr 16 03:04:45 2023, max compression
```

## Comparing `pythesyncer-23.4.14.20.tar` & `pythesyncer-23.4.16.11.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-04-14 12:25:41.449374 pythesyncer-23.4.14.20/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      434 2023-04-14 12:25:41.449374 pythesyncer-23.4.14.20/PKG-INFO
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)       76 2023-04-14 11:29:59.000000 pythesyncer-23.4.14.20/README.md
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-04-14 12:25:41.449374 pythesyncer-23.4.14.20/pythesyncer/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     2618 2023-04-14 12:20:57.000000 pythesyncer-23.4.14.20/pythesyncer/__init__.py
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)     1241 2023-04-14 11:47:39.000000 pythesyncer-23.4.14.20/pythesyncer/auth.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-04-14 12:25:41.449374 pythesyncer-23.4.14.20/pythesyncer.egg-info/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      434 2023-04-14 12:25:41.000000 pythesyncer-23.4.14.20/pythesyncer.egg-info/PKG-INFO
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      274 2023-04-14 12:25:41.000000 pythesyncer-23.4.14.20/pythesyncer.egg-info/SOURCES.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        1 2023-04-14 12:25:41.000000 pythesyncer-23.4.14.20/pythesyncer.egg-info/dependency_links.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       55 2023-04-14 12:25:41.000000 pythesyncer-23.4.14.20/pythesyncer.egg-info/entry_points.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       20 2023-04-14 12:25:41.000000 pythesyncer-23.4.14.20/pythesyncer.egg-info/requires.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       12 2023-04-14 12:25:41.000000 pythesyncer-23.4.14.20/pythesyncer.egg-info/top_level.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       38 2023-04-14 12:25:41.449374 pythesyncer-23.4.14.20/setup.cfg
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      864 2023-04-14 11:58:13.000000 pythesyncer-23.4.14.20/setup.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-04-16 03:04:45.070639 pythesyncer-23.4.16.11/
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)      434 2023-04-16 03:04:45.070639 pythesyncer-23.4.16.11/PKG-INFO
+-rw-r--r--   0 tp03      (1000) tp03      (1000)       76 2023-04-14 11:29:59.000000 pythesyncer-23.4.16.11/README.md
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-04-16 03:04:45.070639 pythesyncer-23.4.16.11/pythesyncer/
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     3448 2023-04-16 03:03:05.000000 pythesyncer-23.4.16.11/pythesyncer/__init__.py
+-rw-r--r--   0 tp03      (1000) tp03      (1000)     1469 2023-04-16 02:52:44.000000 pythesyncer-23.4.16.11/pythesyncer/auth.py
+drwxrwxr-x   0 tp03      (1000) tp03      (1000)        0 2023-04-16 03:04:45.070639 pythesyncer-23.4.16.11/pythesyncer.egg-info/
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)      434 2023-04-16 03:04:44.000000 pythesyncer-23.4.16.11/pythesyncer.egg-info/PKG-INFO
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)      274 2023-04-16 03:04:45.000000 pythesyncer-23.4.16.11/pythesyncer.egg-info/SOURCES.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)        1 2023-04-16 03:04:44.000000 pythesyncer-23.4.16.11/pythesyncer.egg-info/dependency_links.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       55 2023-04-16 03:04:44.000000 pythesyncer-23.4.16.11/pythesyncer.egg-info/entry_points.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       20 2023-04-16 03:04:44.000000 pythesyncer-23.4.16.11/pythesyncer.egg-info/requires.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       12 2023-04-16 03:04:44.000000 pythesyncer-23.4.16.11/pythesyncer.egg-info/top_level.txt
+-rw-rw-r--   0 tp03      (1000) tp03      (1000)       38 2023-04-16 03:04:45.070639 pythesyncer-23.4.16.11/setup.cfg
+-rw-r--r--   0 tp03      (1000) tp03      (1000)      864 2023-04-14 11:58:13.000000 pythesyncer-23.4.16.11/setup.py
```

### Comparing `pythesyncer-23.4.14.20/pythesyncer/__init__.py` & `pythesyncer-23.4.16.11/pythesyncer/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # --------------------------------------------
 import asyncio
 import os
 import sys
 import threading
 from enum import Enum
-
+import aiohttp
 import boto3
 import codefast as cf
 import fire
 from boto3.s3.transfer import TransferConfig
 from codefast.asyncio import asyncformer
 from rich import print
 
 from .auth import auth
 
 # —--------------------------------------------
+KEY = 'pythesyncer'
+REDIS_API = auth.redis_api
 
 
 class ProgressPercentage(object):
 
     def __init__(self, filename):
         self._filename = filename
         self._size = float(os.path.getsize(filename))
@@ -60,37 +62,55 @@
     if action == Action.up:
         await sync_up(obj)
     elif action == Action.down:
         await sync_down(obj)
 
 
 async def sync_up(obj):
+    file_name=cf.io.basename(obj)
     if os.path.isfile(obj):
         cf.info('Uploading file: {}'.format(obj))
         await asyncformer(upload_file, obj)
 
     elif os.path.isdir(obj):
         cf.info('Uploading dir: {}'.format(obj))
+        zipname = cf.random_string(7)
+        zipfile = zipname+'.7z'
         os.system(
-            '7z a -t7z -m0=lzma2 -mx=9 -mfb=64 -md=32m -ms=on archive.7z {}'.
-            format(obj))
-        await asyncformer(upload_file, 'archive.7z')
-        os.remove('archive.7z')
-        cf.info("Upload done: {}".format(obj))
+            '7z a -t7z -m0=lzma2 -mx=9 -mfb=64 -md=32m -ms=on {} {}'.
+            format(zipfile, obj))
+        await asyncformer(upload_file, zipfile)
+        os.remove(zipfile)
+        cf.info("Upload done: {}".format(zipfile))
+        file_name = zipfile
+
+    async with aiohttp.ClientSession() as session:
+        async with session.post(REDIS_API, json={'key': KEY, 'value': file_name}) as resp:
+            if resp.status != 200:
+                cf.error('Failed to get redis key: {}'.format(KEY))
 
 
 async def sync_down(obj):
+    if not obj:
+        async with aiohttp.ClientSession() as session:
+            async with session.post(REDIS_API, json={'key': KEY}) as resp:
+                if resp.status != 200:
+                    cf.error('Failed to get redis key: {}'.format(KEY))
+                js = await resp.json()
+                obj = js['value']
     remote_file = os.path.join(auth.host_api, obj)
     await asyncformer(cf.net.download, remote_file, obj)
 
 
-def entry(action: str, obj: str):
+def entry(action: str, obj: str = None):
     if action not in [a.value for a in Action]:
         print('Action must be one of {}'.format([a.value for a in Action]))
         return
     action = Action(action)
-    loop = asyncio.get_event_loop()
-    loop.run_until_complete(sync(action, obj))
+    if action == Action.up and not obj:
+        print('Uploading object must be specified')
+        return
+    asyncio.run(sync(action, obj))
 
 
 def main():
     fire.Fire(entry)
```

### Comparing `pythesyncer-23.4.14.20/setup.py` & `pythesyncer-23.4.16.11/setup.py`

 * *Files identical despite different names*

