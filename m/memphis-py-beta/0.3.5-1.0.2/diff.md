# Comparing `tmp/memphis-py-beta-0.3.5.tar.gz` & `tmp/memphis-py-beta-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/memphis-py-beta-0.3.5.tar", last modified: Sun Apr  2 15:23:16 2023, max compression
+gzip compressed data, was "dist/memphis-py-beta-1.0.2.tar", last modified: Sun Apr 16 13:50:15 2023, max compression
```

## Comparing `memphis-py-beta-0.3.5.tar` & `memphis-py-beta-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16583 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12646 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/memphis/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      820 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/memphis/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7816 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/memphis/consumer.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      628 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/memphis/exceptions.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      515 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/memphis/headers.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    30416 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/memphis/memphis.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2176 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/memphis/message.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12285 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/memphis/producer.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2190 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/memphis/station.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      827 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/memphis/types.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/memphis/utils.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/memphis_py_beta.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16583 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/memphis_py_beta.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      429 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/memphis_py_beta.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/memphis_py_beta.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       49 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/memphis_py_beta.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/memphis_py_beta.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       62 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/pyproject.toml
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       79 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1331 2023-04-02 15:23:16.000000 memphis-py-beta-0.3.5/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-16 13:50:15.000000 memphis-py-beta-1.0.2/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16297 2023-04-16 13:50:15.000000 memphis-py-beta-1.0.2/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    12392 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-16 13:50:15.000000 memphis-py-beta-1.0.2/memphis/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      820 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/memphis/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     8050 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/memphis/consumer.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      628 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/memphis/exceptions.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      515 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/memphis/headers.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    30732 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/memphis/memphis.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2176 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/memphis/message.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    13161 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/memphis/producer.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2190 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/memphis/station.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      827 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/memphis/types.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/memphis/utils.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-04-16 13:50:15.000000 memphis-py-beta-1.0.2/memphis_py_beta.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    16297 2023-04-16 13:50:15.000000 memphis-py-beta-1.0.2/memphis_py_beta.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      429 2023-04-16 13:50:15.000000 memphis-py-beta-1.0.2/memphis_py_beta.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-04-16 13:50:15.000000 memphis-py-beta-1.0.2/memphis_py_beta.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       49 2023-04-16 13:50:15.000000 memphis-py-beta-1.0.2/memphis_py_beta.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-04-16 13:50:15.000000 memphis-py-beta-1.0.2/memphis_py_beta.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       62 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/pyproject.toml
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       79 2023-04-16 13:50:15.000000 memphis-py-beta-1.0.2/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1331 2023-04-16 13:50:14.000000 memphis-py-beta-1.0.2/setup.py
```

### Comparing `memphis-py-beta-0.3.5/PKG-INFO` & `memphis-py-beta-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,53 @@
 Metadata-Version: 2.1
 Name: memphis-py-beta
-Version: 0.3.5
+Version: 1.0.2
 Summary: A powerful messaging platform for modern developers
 Home-page: https://github.com/memphisdev/memphis.py
 Author: Memphis.dev
 Author-email: team@memphis.dev
 License: Apache-2.0
-Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/0.3.5.tar.gz
+Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.2.tar.gz
 Description: <div align="center">
           
-          ![Memphis light logo](https://github.com/memphisdev/memphis-broker/blob/master/logo-white.png?raw=true#gh-dark-mode-only)
+          ![github memphis banner](https://user-images.githubusercontent.com/70286779/229371212-8531c1e1-1a9d-4bbe-9285-b4dbb8601bfa.jpeg)
           
         </div>
         
         <div align="center">
-          
-          ![Memphis light logo](https://github.com/memphisdev/memphis-broker/blob/master/logo-black.png?raw=true#gh-light-mode-only)
-          
-        </div>
         
-        <div align="center">
-        <h4>Simple as RabbitMQ, Robust as Apache Kafka, and Perfect for microservices.</h4>
+          <h4>
         
-        <img width="750" alt="Memphis UI" src="https://user-images.githubusercontent.com/70286779/204081372-186aae7b-a387-4253-83d1-b07dff69b3d0.png"><br>
+        **[Memphis](https://memphis.dev)** is a next-generation alternative to traditional message brokers.
         
+          </h4>
           
           <a href="https://landscape.cncf.io/?selected=memphis"><img width="200" alt="CNCF Silver Member" src="https://github.com/cncf/artwork/raw/master/other/cncf-member/silver/white/cncf-member-silver-white.svg#gh-dark-mode-only"></a>
           
         </div>
         
         <div align="center">
           
           <img width="200" alt="CNCF Silver Member" src="https://github.com/cncf/artwork/raw/master/other/cncf-member/silver/color/cncf-member-silver-color.svg#gh-light-mode-only">
           
         </div>
          
          <p align="center">
-          <a href="https://sandbox.memphis.dev/" target="_blank">Sandbox</a> - <a href="https://memphis.dev/docs/">Docs</a> - <a href="https://twitter.com/Memphis_Dev">Twitter</a> - <a href="https://www.youtube.com/channel/UCVdMDLCSxXOqtgrBaRUHKKg">YouTube</a>
+          <a href="https://memphis.dev/docs/">Docs</a> - <a href="https://twitter.com/Memphis_Dev">Twitter</a> - <a href="https://www.youtube.com/channel/UCVdMDLCSxXOqtgrBaRUHKKg">YouTube</a>
         </p>
         
         <p align="center">
         <a href="https://discord.gg/WZpysvAeTf"><img src="https://img.shields.io/discord/963333392844328961?color=6557ff&label=discord" alt="Discord"></a>
-        <a href="https://github.com/memphisdev/memphis-broker/issues?q=is%3Aissue+is%3Aclosed"><img src="https://img.shields.io/github/issues-closed/memphisdev/memphis-broker?color=6557ff"></a> 
-        <a href="https://github.com/memphisdev/memphis-broker/blob/master/CODE_OF_CONDUCT.md"><img src="https://img.shields.io/badge/Code%20of%20Conduct-v1.0-ff69b4.svg?color=ffc633" alt="Code Of Conduct"></a> 
-        <a href="https://docs.memphis.dev/memphis/release-notes/releases/v0.4.2-beta"><img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/memphisdev/memphis-broker?color=61dfc6"></a>
-        <img src="https://img.shields.io/github/last-commit/memphisdev/memphis-broker?color=61dfc6&label=last%20commit">
+        <a href="https://github.com/memphisdev/memphis/issues?q=is%3Aissue+is%3Aclosed"><img src="https://img.shields.io/github/issues-closed/memphisdev/memphis?color=6557ff"></a> 
+          <img src="https://img.shields.io/npm/dw/memphis-dev?color=ffc633&label=installations">
+        <a href="https://github.com/memphisdev/memphis/blob/master/CODE_OF_CONDUCT.md"><img src="https://img.shields.io/badge/Code%20of%20Conduct-v1.0-ff69b4.svg?color=ffc633" alt="Code Of Conduct"></a> 
+        <a href="https://docs.memphis.dev/memphis/release-notes/releases/v0.4.2-beta"><img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/memphisdev/memphis?color=61dfc6"></a>
+        <img src="https://img.shields.io/github/last-commit/memphisdev/memphis?color=61dfc6&label=last%20commit">
         </p>
         
-        **[Memphis](https://memphis.dev)** is a next-generation alternative to traditional message brokers.<br><br>
         A simple, robust, and durable cloud-native message broker wrapped with<br>
         an entire ecosystem that enables cost-effective, fast, and reliable development of modern queue-based use cases.<br><br>
         Memphis enables the building of modern queue-based applications that require<br>
         large volumes of streamed and enriched data, modern protocols, zero ops, rapid development,<br>
         extreme cost reduction, and a significantly lower amount of dev time for data-oriented developers and data engineers.
         
         ## Installation
@@ -107,15 +103,15 @@
         To disconnect from Memphis, call `close()` on the memphis object.
         
         ```python
         await memphis.close()
         ```
         
         ### Creating a Station
-        
+        **Unexist stations will be created automatically through the SDK on the first producer/consumer connection with default values.**<br><br>
         _If a station already exists nothing happens, the new configuration will not be applied_
         
         ```python
         station = memphis.station(
           name="<station-name>",
           schema_name="<schema-name>",
           retention_type=Retention.MAX_MESSAGE_AGE_SECONDS, # MAX_MESSAGE_AGE_SECONDS/MESSAGES/BYTES. Defaults to MAX_MESSAGE_AGE_SECONDS
```

### Comparing `memphis-py-beta-0.3.5/README.md` & `memphis-py-beta-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,44 @@
 <div align="center">
   
-  ![Memphis light logo](https://github.com/memphisdev/memphis-broker/blob/master/logo-white.png?raw=true#gh-dark-mode-only)
+  ![github memphis banner](https://user-images.githubusercontent.com/70286779/229371212-8531c1e1-1a9d-4bbe-9285-b4dbb8601bfa.jpeg)
   
 </div>
 
 <div align="center">
-  
-  ![Memphis light logo](https://github.com/memphisdev/memphis-broker/blob/master/logo-black.png?raw=true#gh-light-mode-only)
-  
-</div>
 
-<div align="center">
-<h4>Simple as RabbitMQ, Robust as Apache Kafka, and Perfect for microservices.</h4>
+  <h4>
 
-<img width="750" alt="Memphis UI" src="https://user-images.githubusercontent.com/70286779/204081372-186aae7b-a387-4253-83d1-b07dff69b3d0.png"><br>
+**[Memphis](https://memphis.dev)** is a next-generation alternative to traditional message brokers.
 
+  </h4>
   
   <a href="https://landscape.cncf.io/?selected=memphis"><img width="200" alt="CNCF Silver Member" src="https://github.com/cncf/artwork/raw/master/other/cncf-member/silver/white/cncf-member-silver-white.svg#gh-dark-mode-only"></a>
   
 </div>
 
 <div align="center">
   
   <img width="200" alt="CNCF Silver Member" src="https://github.com/cncf/artwork/raw/master/other/cncf-member/silver/color/cncf-member-silver-color.svg#gh-light-mode-only">
   
 </div>
  
  <p align="center">
-  <a href="https://sandbox.memphis.dev/" target="_blank">Sandbox</a> - <a href="https://memphis.dev/docs/">Docs</a> - <a href="https://twitter.com/Memphis_Dev">Twitter</a> - <a href="https://www.youtube.com/channel/UCVdMDLCSxXOqtgrBaRUHKKg">YouTube</a>
+  <a href="https://memphis.dev/docs/">Docs</a> - <a href="https://twitter.com/Memphis_Dev">Twitter</a> - <a href="https://www.youtube.com/channel/UCVdMDLCSxXOqtgrBaRUHKKg">YouTube</a>
 </p>
 
 <p align="center">
 <a href="https://discord.gg/WZpysvAeTf"><img src="https://img.shields.io/discord/963333392844328961?color=6557ff&label=discord" alt="Discord"></a>
-<a href="https://github.com/memphisdev/memphis-broker/issues?q=is%3Aissue+is%3Aclosed"><img src="https://img.shields.io/github/issues-closed/memphisdev/memphis-broker?color=6557ff"></a> 
-<a href="https://github.com/memphisdev/memphis-broker/blob/master/CODE_OF_CONDUCT.md"><img src="https://img.shields.io/badge/Code%20of%20Conduct-v1.0-ff69b4.svg?color=ffc633" alt="Code Of Conduct"></a> 
-<a href="https://docs.memphis.dev/memphis/release-notes/releases/v0.4.2-beta"><img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/memphisdev/memphis-broker?color=61dfc6"></a>
-<img src="https://img.shields.io/github/last-commit/memphisdev/memphis-broker?color=61dfc6&label=last%20commit">
+<a href="https://github.com/memphisdev/memphis/issues?q=is%3Aissue+is%3Aclosed"><img src="https://img.shields.io/github/issues-closed/memphisdev/memphis?color=6557ff"></a> 
+  <img src="https://img.shields.io/npm/dw/memphis-dev?color=ffc633&label=installations">
+<a href="https://github.com/memphisdev/memphis/blob/master/CODE_OF_CONDUCT.md"><img src="https://img.shields.io/badge/Code%20of%20Conduct-v1.0-ff69b4.svg?color=ffc633" alt="Code Of Conduct"></a> 
+<a href="https://docs.memphis.dev/memphis/release-notes/releases/v0.4.2-beta"><img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/memphisdev/memphis?color=61dfc6"></a>
+<img src="https://img.shields.io/github/last-commit/memphisdev/memphis?color=61dfc6&label=last%20commit">
 </p>
 
-**[Memphis](https://memphis.dev)** is a next-generation alternative to traditional message brokers.<br><br>
 A simple, robust, and durable cloud-native message broker wrapped with<br>
 an entire ecosystem that enables cost-effective, fast, and reliable development of modern queue-based use cases.<br><br>
 Memphis enables the building of modern queue-based applications that require<br>
 large volumes of streamed and enriched data, modern protocols, zero ops, rapid development,<br>
 extreme cost reduction, and a significantly lower amount of dev time for data-oriented developers and data engineers.
 
 ## Installation
@@ -98,15 +94,15 @@
 To disconnect from Memphis, call `close()` on the memphis object.
 
 ```python
 await memphis.close()
 ```
 
 ### Creating a Station
-
+**Unexist stations will be created automatically through the SDK on the first producer/consumer connection with default values.**<br><br>
 _If a station already exists nothing happens, the new configuration will not be applied_
 
 ```python
 station = memphis.station(
   name="<station-name>",
   schema_name="<schema-name>",
   retention_type=Retention.MAX_MESSAGE_AGE_SECONDS, # MAX_MESSAGE_AGE_SECONDS/MESSAGES/BYTES. Defaults to MAX_MESSAGE_AGE_SECONDS
```

### Comparing `memphis-py-beta-0.3.5/memphis/__init__.py` & `memphis-py-beta-1.0.2/memphis/__init__.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-0.3.5/memphis/consumer.py` & `memphis-py-beta-1.0.2/memphis/consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from memphis.exceptions import MemphisError
 from memphis.utils import default_error_handler, get_internal_name
 from memphis.message import Message
 
 
 class Consumer:
+    MAX_BATCH_SIZE = 5000
     def __init__(
         self,
         connection,
         station_name: str,
         consumer_name,
         consumer_group,
         pull_interval_ms: int,
@@ -104,22 +105,25 @@
                 if self.dls_callback_func != None:
                     await self.dls_callback_func(
                         [Message(msg, self.connection, self.consumer_group)],
                         None,
                         self.context,
                     )
         except Exception as e:
-            await self.dls_callback_func([], MemphisError(str(e)), self.context)
-            return
+            if self.dls_callback_func != None:
+                await self.dls_callback_func([], MemphisError(str(e)), self.context)
+                return
 
     async def fetch(self, batch_size: int = 10):
         """Fetch a batch of messages."""
         messages = []
         if self.connection.is_connection_active:
             try:
+                if batch_size > self.MAX_BATCH_SIZE:
+                    raise MemphisError(f"Batch size can not be greater than {self.MAX_BATCH_SIZE}")
                 self.batch_size = batch_size
                 if len(self.dls_messages) > 0:
                     if len(self.dls_messages) <= batch_size:
                         messages = self.dls_messages
                         self.dls_messages = []
                         self.dls_current_index = 0
                     else:
```

### Comparing `memphis-py-beta-0.3.5/memphis/exceptions.py` & `memphis-py-beta-1.0.2/memphis/exceptions.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-0.3.5/memphis/headers.py` & `memphis-py-beta-1.0.2/memphis/headers.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-0.3.5/memphis/memphis.py` & `memphis-py-beta-1.0.2/memphis/memphis.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from memphis.producer import Producer
 from memphis.station import Station
 from memphis.types import Retention, Storage
 from memphis.utils import get_internal_name, random_bytes
 
 
 class Memphis:
+    MAX_BATCH_SIZE = 5000
     def __init__(self):
         self.is_connection_active = False
         self.schema_updates_data = {}
         self.schema_updates_subs = {}
         self.producers_per_station = {}
         self.schema_tasks = {}
         self.proto_msgs = {}
@@ -495,14 +496,16 @@
             last_messages: consume the last N messages, defaults to -1 (all messages in the station).
         Returns:
             object: consumer
         """
         try:
             if not self.is_connection_active:
                 raise MemphisError("Connection is dead")
+            if batch_size > self.MAX_BATCH_SIZE:
+                raise MemphisError(f"Batch size can not be greater than {self.MAX_BATCH_SIZE}")
             real_name = consumer_name.lower()
             if generate_random_suffix:
                 consumer_name = self.__generateRandomSuffix(consumer_name)
             cg = consumer_name if not consumer_group else consumer_group
 
             if start_consume_from_sequence <= 0:
                 raise MemphisError(
@@ -635,14 +638,16 @@
         Returns:
             list: Message
         """
         try:
             consumer = None
             if not self.is_connection_active:
                 raise MemphisError("Cant fetch messages without being connected!")
+            if batch_size > self.MAX_BATCH_SIZE:
+                raise MemphisError(f"Batch size can not be greater than {self.MAX_BATCH_SIZE}")
             internal_station_name = get_internal_name(station_name)
             consumer_map_key = internal_station_name + "_" + consumer_name.lower()
             if consumer_map_key in self.consumers_map:
                 consumer = self.consumers_map[consumer_map_key]
             else:
                 consumer = await self.consumer(
                     station_name=station_name,
```

### Comparing `memphis-py-beta-0.3.5/memphis/message.py` & `memphis-py-beta-1.0.2/memphis/message.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-0.3.5/memphis/producer.py` & `memphis-py-beta-1.0.2/memphis/producer.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,14 +37,25 @@
                 return message
             elif schema_type == "json":
                 message = self.validate_json_schema(message)
                 return message
             elif schema_type == "graphql":
                 message = self.validate_graphql(message)
                 return message
+            elif hasattr(message, "SerializeToString"):
+                msgToSend = message.SerializeToString()
+                return msgToSend
+        elif isinstance(message, str):
+            message = message.encode("utf-8")
+            return message
+        elif isinstance(message, graphql.language.ast.DocumentNode):
+            msg = message
+            message = str(msg.loc.source.body)
+            message = message.encode("utf-8")
+            return message
         elif not isinstance(message, bytearray) and not isinstance(message, dict):
             raise MemphisSchemaError("Unsupported message type")
         else:
             if isinstance(message, dict):
                 message = bytearray(json.dumps(message).encode("utf-8"))
             return message
 
@@ -177,71 +188,75 @@
                     message,
                     timeout=ack_wait_sec,
                     headers=headers,
                 )
         except Exception as e:
             if hasattr(e, "status_code") and e.status_code == "503":
                 raise MemphisError(
-                    "Produce operation has failed, please check whether Station/Producer are still exist"
+                    "Produce operation has failed, please check whether Station/Producer still exist"
                 )
             else:
                 if "Schema validation has failed" in str(
                     e
                 ) or "Unsupported message type" in str(e):
-                    msgToSend = ""
-                    if hasattr(message, "SerializeToString"):
-                        msgToSend = message.SerializeToString().decode("utf-8")
-                    elif isinstance(message, bytearray):
-                        msgToSend = str(message, "utf-8")
-                    else:
-                        msgToSend = str(message)
-                    if self.connection.station_schemaverse_to_dls[
-                        self.internal_station_name
-                    ]:
-                        memphis_headers = {
-                            "$memphis_producedBy": self.producer_name,
-                            "$memphis_connectionId": self.connection.connection_id,
-                        }
-
-                        if headers != {}:
-                            headers = headers.headers
-                            headers.update(memphis_headers)
+                    if self.connection.schema_updates_data[self.internal_station_name] != {}:
+                        msgToSend = ""
+                        if hasattr(message, "SerializeToString"):
+                            msgToSend = message.SerializeToString().decode("utf-8")
+                        elif isinstance(message, bytearray):
+                            msgToSend = str(message, "utf-8")
                         else:
-                            headers = memphis_headers
-
-                        msgToSendEncoded = msgToSend.encode("utf-8")
-                        msgHex = msgToSendEncoded.hex()
-                        buf = {
-                            "station_name": self.internal_station_name,
-                            "producer": {
-                                "name": self.producer_name,
-                                "connection_id": self.connection.connection_id,
-                            },
-                            "message": {
-                                "data": msgHex,
-                                "headers": headers,
-                            },
-                            "validation_error": str(e),
-                        }
-                        buf = json.dumps(buf).encode("utf-8")
-                        await self.connection.broker_manager.publish("$memphis_schemaverse_dls", buf)
-                        if self.connection.cluster_configurations.get(
-                            "send_notification"
-                        ):
-                            await self.connection.send_notification(
-                                "Schema validation has failed",
-                                "Station: "
-                                + self.station_name
-                                + "\nProducer: "
-                                + self.producer_name
-                                + "\nError:"
-                                + str(e),
-                                msgToSend,
-                                schemaVFailAlertType,
-                            )
+                            msgToSend = str(message)
+                        if self.connection.station_schemaverse_to_dls[
+                            self.internal_station_name
+                        ]:
+                            unix_time = int(time.time())
+
+                            memphis_headers = {
+                                "$memphis_producedBy": self.producer_name,
+                                "$memphis_connectionId": self.connection.connection_id,
+                            }
+
+                            if headers != {}:
+                                headers = headers.headers
+                                headers.update(memphis_headers)
+                            else:
+                                headers = memphis_headers
+
+                            msgToSendEncoded = msgToSend.encode("utf-8")
+                            msgHex = msgToSendEncoded.hex()
+                            buf = {
+                                "station_name": self.internal_station_name,
+                                "producer": {
+                                    "name": self.producer_name,
+                                    "connection_id": self.connection.connection_id,
+                                },
+                                "creation_unix": unix_time,
+                                "message": {
+                                    "data": msgHex,
+                                    "headers": headers,
+                                },
+                                "validation_error": str(e),
+                            }
+                            buf = json.dumps(buf).encode("utf-8")
+                            await self.connection.broker_manager.publish("$memphis_schemaverse_dls", buf)
+                            if self.connection.cluster_configurations.get(
+                                "send_notification"
+                            ):
+                                await self.connection.send_notification(
+                                    "Schema validation has failed",
+                                    "Station: "
+                                    + self.station_name
+                                    + "\nProducer: "
+                                    + self.producer_name
+                                    + "\nError:"
+                                    + str(e),
+                                    msgToSend,
+                                    schemaVFailAlertType,
+                                )
                 raise MemphisError(str(e)) from e
 
     async def destroy(self):
         """Destroy the producer."""
         try:
             destroyProducerReq = {
                 "name": self.producer_name,
```

### Comparing `memphis-py-beta-0.3.5/memphis/station.py` & `memphis-py-beta-1.0.2/memphis/station.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-0.3.5/memphis/types.py` & `memphis-py-beta-1.0.2/memphis/types.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-0.3.5/memphis/utils.py` & `memphis-py-beta-1.0.2/memphis/utils.py`

 * *Files identical despite different names*

### Comparing `memphis-py-beta-0.3.5/memphis_py_beta.egg-info/PKG-INFO` & `memphis-py-beta-1.0.2/memphis_py_beta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,57 +1,53 @@
 Metadata-Version: 2.1
 Name: memphis-py-beta
-Version: 0.3.5
+Version: 1.0.2
 Summary: A powerful messaging platform for modern developers
 Home-page: https://github.com/memphisdev/memphis.py
 Author: Memphis.dev
 Author-email: team@memphis.dev
 License: Apache-2.0
-Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/0.3.5.tar.gz
+Download-URL: https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.2.tar.gz
 Description: <div align="center">
           
-          ![Memphis light logo](https://github.com/memphisdev/memphis-broker/blob/master/logo-white.png?raw=true#gh-dark-mode-only)
+          ![github memphis banner](https://user-images.githubusercontent.com/70286779/229371212-8531c1e1-1a9d-4bbe-9285-b4dbb8601bfa.jpeg)
           
         </div>
         
         <div align="center">
-          
-          ![Memphis light logo](https://github.com/memphisdev/memphis-broker/blob/master/logo-black.png?raw=true#gh-light-mode-only)
-          
-        </div>
         
-        <div align="center">
-        <h4>Simple as RabbitMQ, Robust as Apache Kafka, and Perfect for microservices.</h4>
+          <h4>
         
-        <img width="750" alt="Memphis UI" src="https://user-images.githubusercontent.com/70286779/204081372-186aae7b-a387-4253-83d1-b07dff69b3d0.png"><br>
+        **[Memphis](https://memphis.dev)** is a next-generation alternative to traditional message brokers.
         
+          </h4>
           
           <a href="https://landscape.cncf.io/?selected=memphis"><img width="200" alt="CNCF Silver Member" src="https://github.com/cncf/artwork/raw/master/other/cncf-member/silver/white/cncf-member-silver-white.svg#gh-dark-mode-only"></a>
           
         </div>
         
         <div align="center">
           
           <img width="200" alt="CNCF Silver Member" src="https://github.com/cncf/artwork/raw/master/other/cncf-member/silver/color/cncf-member-silver-color.svg#gh-light-mode-only">
           
         </div>
          
          <p align="center">
-          <a href="https://sandbox.memphis.dev/" target="_blank">Sandbox</a> - <a href="https://memphis.dev/docs/">Docs</a> - <a href="https://twitter.com/Memphis_Dev">Twitter</a> - <a href="https://www.youtube.com/channel/UCVdMDLCSxXOqtgrBaRUHKKg">YouTube</a>
+          <a href="https://memphis.dev/docs/">Docs</a> - <a href="https://twitter.com/Memphis_Dev">Twitter</a> - <a href="https://www.youtube.com/channel/UCVdMDLCSxXOqtgrBaRUHKKg">YouTube</a>
         </p>
         
         <p align="center">
         <a href="https://discord.gg/WZpysvAeTf"><img src="https://img.shields.io/discord/963333392844328961?color=6557ff&label=discord" alt="Discord"></a>
-        <a href="https://github.com/memphisdev/memphis-broker/issues?q=is%3Aissue+is%3Aclosed"><img src="https://img.shields.io/github/issues-closed/memphisdev/memphis-broker?color=6557ff"></a> 
-        <a href="https://github.com/memphisdev/memphis-broker/blob/master/CODE_OF_CONDUCT.md"><img src="https://img.shields.io/badge/Code%20of%20Conduct-v1.0-ff69b4.svg?color=ffc633" alt="Code Of Conduct"></a> 
-        <a href="https://docs.memphis.dev/memphis/release-notes/releases/v0.4.2-beta"><img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/memphisdev/memphis-broker?color=61dfc6"></a>
-        <img src="https://img.shields.io/github/last-commit/memphisdev/memphis-broker?color=61dfc6&label=last%20commit">
+        <a href="https://github.com/memphisdev/memphis/issues?q=is%3Aissue+is%3Aclosed"><img src="https://img.shields.io/github/issues-closed/memphisdev/memphis?color=6557ff"></a> 
+          <img src="https://img.shields.io/npm/dw/memphis-dev?color=ffc633&label=installations">
+        <a href="https://github.com/memphisdev/memphis/blob/master/CODE_OF_CONDUCT.md"><img src="https://img.shields.io/badge/Code%20of%20Conduct-v1.0-ff69b4.svg?color=ffc633" alt="Code Of Conduct"></a> 
+        <a href="https://docs.memphis.dev/memphis/release-notes/releases/v0.4.2-beta"><img alt="GitHub release (latest by date)" src="https://img.shields.io/github/v/release/memphisdev/memphis?color=61dfc6"></a>
+        <img src="https://img.shields.io/github/last-commit/memphisdev/memphis?color=61dfc6&label=last%20commit">
         </p>
         
-        **[Memphis](https://memphis.dev)** is a next-generation alternative to traditional message brokers.<br><br>
         A simple, robust, and durable cloud-native message broker wrapped with<br>
         an entire ecosystem that enables cost-effective, fast, and reliable development of modern queue-based use cases.<br><br>
         Memphis enables the building of modern queue-based applications that require<br>
         large volumes of streamed and enriched data, modern protocols, zero ops, rapid development,<br>
         extreme cost reduction, and a significantly lower amount of dev time for data-oriented developers and data engineers.
         
         ## Installation
@@ -107,15 +103,15 @@
         To disconnect from Memphis, call `close()` on the memphis object.
         
         ```python
         await memphis.close()
         ```
         
         ### Creating a Station
-        
+        **Unexist stations will be created automatically through the SDK on the first producer/consumer connection with default values.**<br><br>
         _If a station already exists nothing happens, the new configuration will not be applied_
         
         ```python
         station = memphis.station(
           name="<station-name>",
           schema_name="<schema-name>",
           retention_type=Retention.MAX_MESSAGE_AGE_SECONDS, # MAX_MESSAGE_AGE_SECONDS/MESSAGES/BYTES. Defaults to MAX_MESSAGE_AGE_SECONDS
```

### Comparing `memphis-py-beta-0.3.5/setup.py` & `memphis-py-beta-1.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="memphis-py-beta",
     packages=["memphis"],
-    version="0.3.5",
+    version="1.0.2",
     license="Apache-2.0",
     description="A powerful messaging platform for modern developers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     readme="README.md",
     author="Memphis.dev",
     author_email="team@memphis.dev",
     url="https://github.com/memphisdev/memphis.py",
-    download_url="https://github.com/memphisdev/memphis.py/archive/refs/tags/0.3.5.tar.gz",
+    download_url="https://github.com/memphisdev/memphis.py/archive/refs/tags/1.0.2.tar.gz",
     keywords=["message broker", "devtool", "streaming", "data"],
     install_requires=["asyncio", "nats-py", "protobuf", "jsonschema", "graphql-core"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development",
         "License :: OSI Approved :: GNU General Public License (GPL)",
```

