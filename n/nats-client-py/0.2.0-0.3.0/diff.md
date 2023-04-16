# Comparing `tmp/nats-client-py-0.2.0.tar.gz` & `tmp/nats-client-py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nats-client-py-0.2.0.tar", last modified: Sun Apr 16 11:19:29 2023, max compression
+gzip compressed data, was "nats-client-py-0.3.0.tar", last modified: Sun Apr 16 15:32:41 2023, max compression
```

## Comparing `nats-client-py-0.2.0.tar` & `nats-client-py-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 11:19:29.579470 nats-client-py-0.2.0/
--rw-rw-rw-   0        0        0       61 2023-04-16 11:19:29.578470 nats-client-py-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3762 2023-04-16 10:42:42.000000 nats-client-py-0.2.0/client.py
-drwxrwxrwx   0        0        0        0 2023-04-16 11:19:29.578470 nats-client-py-0.2.0/nats_client_py.egg-info/
--rw-rw-rw-   0        0        0       61 2023-04-16 11:19:29.000000 nats-client-py-0.2.0/nats_client_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-04-16 11:19:29.000000 nats-client-py-0.2.0/nats_client_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 11:19:29.000000 nats-client-py-0.2.0/nats_client_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-04-16 11:19:29.000000 nats-client-py-0.2.0/nats_client_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 11:19:29.579470 nats-client-py-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      208 2023-04-16 11:17:55.000000 nats-client-py-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:32:41.603184 nats-client-py-0.3.0/
+-rw-rw-rw-   0        0        0       61 2023-04-16 15:32:41.602223 nats-client-py-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4673 2023-04-16 15:26:53.000000 nats-client-py-0.3.0/client.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:32:41.602223 nats-client-py-0.3.0/nats_client_py.egg-info/
+-rw-rw-rw-   0        0        0       61 2023-04-16 15:32:41.000000 nats-client-py-0.3.0/nats_client_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-04-16 15:32:41.000000 nats-client-py-0.3.0/nats_client_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 15:32:41.000000 nats-client-py-0.3.0/nats_client_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-04-16 15:32:41.000000 nats-client-py-0.3.0/nats_client_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 15:32:41.603184 nats-client-py-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      208 2023-04-16 15:31:57.000000 nats-client-py-0.3.0/setup.py
```

### Comparing `nats-client-py-0.2.0/client.py` & `nats-client-py-0.3.0/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,20 +3,26 @@
 import asyncio
 import json
 import typing
 
 import nats
 from nats.aio.client import Client, Msg
 
-from utils.action import ActionSchema
-
 nats_server = nats
 nats_client = None
 
 
+class ActionSchema:
+    def __init__(self, name, handle, queue: bool = True, validate=None):
+        self.name = name
+        self.handle = handle
+        self.queue = queue
+        self.validate = validate
+
+
 def prefix_topic(service_name, service_version, action_name):
     return "v{version}.{name}.{action_name}".format(
         version=service_version,
         name=service_name,
         action_name=action_name,
     )
 
@@ -119,7 +125,35 @@
         return msg_handle
 
     def _context(self):
         return {
             "broker": self.nc,
             "emit": self.emit(),
         }
+
+
+class CreateService:
+    version: str = '1'
+    name: str
+    workers: int = 1
+    actions: list[ActionSchema]
+
+    def __init__(self, version, name, workers):
+        self.actions = []
+        self.version = version
+        self.name = name
+        self.workers = workers
+
+    def add(self, **kwargs):
+        actions = kwargs.get('actions')
+        if isinstance(actions, list):
+            self.actions.extend(actions)
+        else:
+            self.actions.append(actions)
+
+    async def register(self, broker: NatsBroker):
+        await broker.create_service(
+            name=self.name,
+            version=self.version,
+            workers=self.workers,
+            actions=self.actions,
+        )
```

