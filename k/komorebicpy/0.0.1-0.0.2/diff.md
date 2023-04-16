# Comparing `tmp/komorebicpy-0.0.1.tar.gz` & `tmp/komorebicpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "komorebicpy-0.0.1.tar", max compression
+gzip compressed data, was "komorebicpy-0.0.2.tar", max compression
```

## Comparing `komorebicpy-0.0.1.tar` & `komorebicpy-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0      171 2023-04-15 09:20:18.037779 komorebicpy-0.0.1/komorebic/__init__.py
--rw-r--r--   0        0        0     2538 2023-04-15 08:07:32.588269 komorebicpy-0.0.1/komorebic/async_client.py
--rw-r--r--   0        0        0      634 2023-04-15 13:23:59.926062 komorebicpy-0.0.1/komorebic/base.py
--rw-r--r--   0        0        0     3632 2023-04-15 13:29:26.796023 komorebicpy-0.0.1/komorebic/client.py
--rw-r--r--   0        0        0     3348 2023-04-15 09:27:28.137731 komorebicpy-0.0.1/komorebic/event_manager.py
--rw-r--r--   0        0        0     1358 2023-04-15 08:15:14.958236 komorebicpy-0.0.1/komorebic/events.py
--rw-r--r--   0        0        0     2378 2023-04-15 15:12:36.915295 komorebicpy-0.0.1/komorebic/komorebic_detect_workspaces.py
--rw-r--r--   0        0        0        2 2023-04-13 13:31:11.226377 komorebicpy-0.0.1/komorebic/sync_client.py
--rw-r--r--   0        0        0     2334 2023-04-14 19:27:00.935683 komorebicpy-0.0.1/komorebic/utils.py
--rw-r--r--   0        0        0      547 2023-04-16 05:53:23.027774 komorebicpy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-16 05:53:51.897768 komorebicpy-0.0.1/README.md
--rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 komorebicpy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      171 2023-04-15 09:20:18.037779 komorebicpy-0.0.2/komorebic/__init__.py
+-rw-r--r--   0        0        0     2538 2023-04-15 08:07:32.588269 komorebicpy-0.0.2/komorebic/async_client.py
+-rw-r--r--   0        0        0      757 2023-04-16 08:10:07.696146 komorebicpy-0.0.2/komorebic/base.py
+-rw-r--r--   0        0        0     3632 2023-04-15 13:29:26.796023 komorebicpy-0.0.2/komorebic/client.py
+-rw-r--r--   0        0        0     3348 2023-04-15 09:27:28.137731 komorebicpy-0.0.2/komorebic/event_manager.py
+-rw-r--r--   0        0        0     1358 2023-04-15 08:15:14.958236 komorebicpy-0.0.2/komorebic/events.py
+-rw-r--r--   0        0        0        2 2023-04-13 13:31:11.226377 komorebicpy-0.0.2/komorebic/sync_client.py
+-rw-r--r--   0        0        0     2334 2023-04-14 19:27:00.935683 komorebicpy-0.0.2/komorebic/utils.py
+-rw-r--r--   0        0        0      547 2023-04-16 08:10:28.206143 komorebicpy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-16 05:53:51.897768 komorebicpy-0.0.2/README.md
+-rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 komorebicpy-0.0.2/PKG-INFO
```

### Comparing `komorebicpy-0.0.1/komorebic/async_client.py` & `komorebicpy-0.0.2/komorebic/async_client.py`

 * *Files identical despite different names*

### Comparing `komorebicpy-0.0.1/komorebic/base.py` & `komorebicpy-0.0.2/komorebic/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 from loguru import logger
 
 
 class ClientBase:
     def __init__(self, exe: str):
         self.exe = exe
 
-    async def run(self, *cmd):
+    async def run(self, *cmd) -> str:
         cmd = [str(param) for param in cmd]
         logger.debug(cmd)
 
         return await self._run(self.exe, *cmd)
 
-    async def _run(self, exe, *cmd):
+    async def _run(self, exe, *cmd) -> str:
         proc = await aio.create_subprocess_exec(
             exe, *cmd, stdout=aio.subprocess.PIPE, stderr=aio.subprocess.PIPE
         )
-        stdout, stderr = await proc.communicate()
+        # sometime when komorebi somehow becomes unresponsive, raises TimeoutError
+        stdout, stderr = await aio.wait_for(proc.communicate(), timeout=2)
+
         stdout, stderr = stdout.decode(), stderr.decode()
         if stderr:
             logger.error(stderr)
 
         return stdout
```

### Comparing `komorebicpy-0.0.1/komorebic/client.py` & `komorebicpy-0.0.2/komorebic/client.py`

 * *Files identical despite different names*

### Comparing `komorebicpy-0.0.1/komorebic/event_manager.py` & `komorebicpy-0.0.2/komorebic/event_manager.py`

 * *Files identical despite different names*

### Comparing `komorebicpy-0.0.1/komorebic/events.py` & `komorebicpy-0.0.2/komorebic/events.py`

 * *Files identical despite different names*

### Comparing `komorebicpy-0.0.1/komorebic/utils.py` & `komorebicpy-0.0.2/komorebic/utils.py`

 * *Files identical despite different names*

### Comparing `komorebicpy-0.0.1/pyproject.toml` & `komorebicpy-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "komorebicpy"
 packages = [
     { include="komorebic", from="." }
 ]
-version = "0.0.1"
+version = "0.0.2"
 description = "Python wrapper around komorebic.exe"
 authors = ["Dmitrij Vinokour <dmitrij.vinokour@cojodi.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `komorebicpy-0.0.1/PKG-INFO` & `komorebicpy-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: komorebicpy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper around komorebic.exe
 License: MIT
 Author: Dmitrij Vinokour
 Author-email: dmitrij.vinokour@cojodi.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

