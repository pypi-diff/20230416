# Comparing `tmp/butler-connect-0.4.3.tar.gz` & `tmp/butler-connect-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butler-connect-0.4.3.tar", last modified: Sat Apr 15 11:38:00 2023, max compression
+gzip compressed data, was "butler-connect-0.4.4.tar", last modified: Sun Apr 16 09:47:12 2023, max compression
```

## Comparing `butler-connect-0.4.3.tar` & `butler-connect-0.4.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 11:38:00.551450 butler-connect-0.4.3/
--rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.4.3/LICENSE
--rw-rw-rw-   0        0        0     1957 2023-04-15 11:38:00.549786 butler-connect-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-04-15 11:37:42.000000 butler-connect-0.4.3/README.md
--rw-rw-rw-   0        0        0      738 2023-04-15 11:33:00.000000 butler-connect-0.4.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 11:38:00.551450 butler-connect-0.4.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-15 11:38:00.515910 butler-connect-0.4.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-15 11:38:00.519926 butler-connect-0.4.3/src/butlerConnect/
--rw-rw-rw-   0        0        0       43 2022-12-30 14:11:10.000000 butler-connect-0.4.3/src/butlerConnect/__init__.py
--rw-rw-rw-   0        0        0    16460 2023-04-15 11:32:35.000000 butler-connect-0.4.3/src/butlerConnect/pikaButler.py
-drwxrwxrwx   0        0        0        0 2023-04-15 11:38:00.526701 butler-connect-0.4.3/src/butlerDescription/
--rw-rw-rw-   0        0        0      108 2022-12-30 15:11:11.000000 butler-connect-0.4.3/src/butlerDescription/__init__.py
--rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.4.3/src/butlerDescription/component.py
--rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.4.3/src/butlerDescription/control.py
--rw-rw-rw-   0        0        0     1570 2023-01-18 19:27:38.000000 butler-connect-0.4.3/src/butlerDescription/signal.py
-drwxrwxrwx   0        0        0        0 2023-04-15 11:38:00.548695 butler-connect-0.4.3/src/butler_connect.egg-info/
--rw-rw-rw-   0        0        0     1957 2023-04-15 11:38:00.000000 butler-connect-0.4.3/src/butler_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2023-04-15 11:38:00.000000 butler-connect-0.4.3/src/butler_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 11:38:00.000000 butler-connect-0.4.3/src/butler_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2023-04-15 11:38:00.000000 butler-connect-0.4.3/src/butler_connect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-04-15 11:38:00.000000 butler-connect-0.4.3/src/butler_connect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 09:47:12.723688 butler-connect-0.4.4/
+-rw-rw-rw-   0        0        0     1091 2022-12-30 14:19:14.000000 butler-connect-0.4.4/LICENSE
+-rw-rw-rw-   0        0        0     2022 2023-04-16 09:47:12.722680 butler-connect-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-04-16 09:43:57.000000 butler-connect-0.4.4/README.md
+-rw-rw-rw-   0        0        0      738 2023-04-16 09:42:49.000000 butler-connect-0.4.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 09:47:12.723688 butler-connect-0.4.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 09:47:12.687683 butler-connect-0.4.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 09:47:12.697689 butler-connect-0.4.4/src/butlerConnect/
+-rw-rw-rw-   0        0        0       43 2022-12-30 14:11:10.000000 butler-connect-0.4.4/src/butlerConnect/__init__.py
+-rw-rw-rw-   0        0        0    17118 2023-04-16 09:42:21.000000 butler-connect-0.4.4/src/butlerConnect/pikaButler.py
+drwxrwxrwx   0        0        0        0 2023-04-16 09:47:12.701679 butler-connect-0.4.4/src/butlerDescription/
+-rw-rw-rw-   0        0        0      108 2022-12-30 15:11:11.000000 butler-connect-0.4.4/src/butlerDescription/__init__.py
+-rw-rw-rw-   0        0        0      180 2023-04-11 15:45:51.000000 butler-connect-0.4.4/src/butlerDescription/component.py
+-rw-rw-rw-   0        0        0     1525 2022-12-30 14:09:45.000000 butler-connect-0.4.4/src/butlerDescription/control.py
+-rw-rw-rw-   0        0        0     1570 2023-01-18 19:27:38.000000 butler-connect-0.4.4/src/butlerDescription/signal.py
+drwxrwxrwx   0        0        0        0 2023-04-16 09:47:12.720692 butler-connect-0.4.4/src/butler_connect.egg-info/
+-rw-rw-rw-   0        0        0     2022 2023-04-16 09:47:12.000000 butler-connect-0.4.4/src/butler_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2023-04-16 09:47:12.000000 butler-connect-0.4.4/src/butler_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 09:47:12.000000 butler-connect-0.4.4/src/butler_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-04-16 09:47:12.000000 butler-connect-0.4.4/src/butler_connect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-04-16 09:47:12.000000 butler-connect-0.4.4/src/butler_connect.egg-info/top_level.txt
```

### Comparing `butler-connect-0.4.3/LICENSE` & `butler-connect-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `butler-connect-0.4.3/PKG-INFO` & `butler-connect-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.4.3
+Version: 0.4.4
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,7 +36,10 @@
 Access libraries and data definitions for the Buttler project.
 For more information ask Oliver Birkholz.
 
 0.4.0:
 - Adding vhost Support
 0.4.3: 
 - Adding sending automatic heartbeats in publisher-function
+0.4.4:
+- update sending automatic heartbeats
+- handling error
```

### Comparing `butler-connect-0.4.3/pyproject.toml` & `butler-connect-0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "butler-connect"
-version = "0.4.3"
+version = "0.4.4"
 description = "Access libraries (with pika) and data definitions for the Buttler project."
 readme = "README.md"
 authors = [{ name = "Oliver Birkholz", email = "info@aibutler.de" }]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `butler-connect-0.4.3/src/butlerConnect/pikaButler.py` & `butler-connect-0.4.4/src/butlerConnect/pikaButler.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,35 +249,45 @@
         self.que = queue.Queue()
         self.connection = None
         self.channel = None
     def run(self):
         LOG.info(f'Create pika Publish-Connection with: {self.connectionParameter}')
         self.connection = pika.BlockingConnection(self.connectionParameter)
         self.channel:pika.adapters.blocking_connection.BlockingChannel = self.connection.channel()
+        self.channel.confirm_delivery()
         
         while self.isRunning :
             try:
-                item = self.que.get(block=True,timeout=default_heartbeat/2)
+                item = self.que.get(block=True,timeout=default_heartbeat/4)
             except:
                 item = {}      
             if item != {}:
                 try:
                     for topic in item.keys():
                         d = item[topic]
                         msg = d.get('msg')
                         routing_key = d.get('routing_key',None)
                         if routing_key == None: routing_key = ''
                         LOG.info(f'publish data {topic}@{msg}')
-                        self.channel.basic_publish(exchange=topic,
+                        try:
+                            self.channel.basic_publish(exchange=topic,
                                 routing_key=routing_key,
-                                body=msg)
+                                body=msg,properties=pika.BasicProperties(content_type='text/plain',
+                                                          delivery_mode=pika.DeliveryMode.Transient),
+                          mandatory=True)
+                        except (pika.exceptions.UnroutableError, pika.exceptions.ChannelClosedByBroker) as e:
+                            print(f'Error on publish {topic}=>{msg} with routing_key={routing_key}')
+                            print(e)
+                            self.que.put(item)
                 except Exception as e:
                     self.que.put(item)
                     raise e
-                self.que.task_done()
+            else:
+                # do a pika heartbeat
+                self.connection.process_data_events(time_limit=0.1) 
 
             
     def publish(self,topic,msg,routing_key=None):
         LOG.info(f'publish {topic}=>{msg} with routing_key={routing_key}')
         self.que.put_nowait({topic:{'msg':msg,'routing_key':routing_key}})
     def stop(self):
         super().stop()
```

### Comparing `butler-connect-0.4.3/src/butlerDescription/control.py` & `butler-connect-0.4.4/src/butlerDescription/control.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.4.3/src/butlerDescription/signal.py` & `butler-connect-0.4.4/src/butlerDescription/signal.py`

 * *Files identical despite different names*

### Comparing `butler-connect-0.4.3/src/butler_connect.egg-info/PKG-INFO` & `butler-connect-0.4.4/src/butler_connect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butler-connect
-Version: 0.4.3
+Version: 0.4.4
 Summary: Access libraries (with pika) and data definitions for the Buttler project.
 Author-email: Oliver Birkholz <info@aibutler.de>
 License: MIT License
         
         Copyright (c) 2023 Oliver Birkholz
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,7 +36,10 @@
 Access libraries and data definitions for the Buttler project.
 For more information ask Oliver Birkholz.
 
 0.4.0:
 - Adding vhost Support
 0.4.3: 
 - Adding sending automatic heartbeats in publisher-function
+0.4.4:
+- update sending automatic heartbeats
+- handling error
```

