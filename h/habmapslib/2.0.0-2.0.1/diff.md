# Comparing `tmp/habmapslib-2.0.0.tar.gz` & `tmp/habmapslib-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "habmapslib-2.0.0.tar", last modified: Sat Apr 15 18:14:44 2023, max compression
+gzip compressed data, was "habmapslib-2.0.1.tar", last modified: Sun Apr 16 09:51:32 2023, max compression
```

## Comparing `habmapslib-2.0.0.tar` & `habmapslib-2.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-04-15 18:14:44.584937 habmapslib-2.0.0/
--rw-r--r--   0 alvaroperis   (501) staff       (20)     1072 2023-04-13 16:43:51.000000 habmapslib-2.0.0/LICENSE.txt
--rw-r--r--   0 alvaroperis   (501) staff       (20)     8969 2023-04-15 18:14:44.573326 habmapslib-2.0.0/PKG-INFO
--rw-r--r--   0 alvaroperis   (501) staff       (20)     8025 2023-04-15 18:14:42.000000 habmapslib-2.0.0/README.md
-drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-04-15 18:14:44.563024 habmapslib-2.0.0/habmapslib/
--rw-r--r--   0 alvaroperis   (501) staff       (20)      694 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/Appender.py
--rw-r--r--   0 alvaroperis   (501) staff       (20)      489 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/ConfHandler.py
--rw-r--r--   0 alvaroperis   (501) staff       (20)     2116 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/GPSAppender.py
--rw-r--r--   0 alvaroperis   (501) staff       (20)     2154 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/HMTail.py
--rw-r--r--   0 alvaroperis   (501) staff       (20)     3557 2023-04-15 18:10:37.000000 habmapslib-2.0.0/habmapslib/HabMapsMessage.py
--rw-r--r--   0 alvaroperis   (501) staff       (20)     1694 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/InitChecks.py
--rw-r--r--   0 alvaroperis   (501) staff       (20)     2660 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/MapTracker.py
--rw-r--r--   0 alvaroperis   (501) staff       (20)     3830 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/Parser.py
--rw-r--r--   0 alvaroperis   (501) staff       (20)      105 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/__init__.py
--rw-r--r--   0 alvaroperis   (501) staff       (20)        0 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/__main__.py
--rw-r--r--   0 alvaroperis   (501) staff       (20)     1107 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/cli.py
--rw-r--r--   0 alvaroperis   (501) staff       (20)      862 2023-04-13 16:43:51.000000 habmapslib-2.0.0/habmapslib/confyaml.py
-drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-04-15 18:14:44.571431 habmapslib-2.0.0/habmapslib.egg-info/
--rw-r--r--   0 alvaroperis   (501) staff       (20)     8969 2023-04-15 18:14:43.000000 habmapslib-2.0.0/habmapslib.egg-info/PKG-INFO
--rw-r--r--   0 alvaroperis   (501) staff       (20)      482 2023-04-15 18:14:43.000000 habmapslib-2.0.0/habmapslib.egg-info/SOURCES.txt
--rw-r--r--   0 alvaroperis   (501) staff       (20)        1 2023-04-15 18:14:43.000000 habmapslib-2.0.0/habmapslib.egg-info/dependency_links.txt
--rw-r--r--   0 alvaroperis   (501) staff       (20)       43 2023-04-15 18:14:43.000000 habmapslib-2.0.0/habmapslib.egg-info/requires.txt
--rw-r--r--   0 alvaroperis   (501) staff       (20)       11 2023-04-15 18:14:43.000000 habmapslib-2.0.0/habmapslib.egg-info/top_level.txt
--rw-r--r--   0 alvaroperis   (501) staff       (20)       38 2023-04-15 18:14:44.591460 habmapslib-2.0.0/setup.cfg
--rw-r--r--   0 alvaroperis   (501) staff       (20)     1325 2023-04-15 18:14:36.000000 habmapslib-2.0.0/setup.py
+drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-04-16 09:51:32.431993 habmapslib-2.0.1/
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     1072 2023-04-13 16:43:51.000000 habmapslib-2.0.1/LICENSE.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     8969 2023-04-16 09:51:32.431129 habmapslib-2.0.1/PKG-INFO
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     8025 2023-04-16 09:51:30.000000 habmapslib-2.0.1/README.md
+drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-04-16 09:51:32.424971 habmapslib-2.0.1/habmapslib/
+-rw-r--r--   0 alvaroperis   (501) staff       (20)      694 2023-04-13 16:43:51.000000 habmapslib-2.0.1/habmapslib/Appender.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)      489 2023-04-13 16:43:51.000000 habmapslib-2.0.1/habmapslib/ConfHandler.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     2116 2023-04-13 16:43:51.000000 habmapslib-2.0.1/habmapslib/GPSAppender.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     2154 2023-04-13 16:43:51.000000 habmapslib-2.0.1/habmapslib/HMTail.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     3563 2023-04-16 09:10:36.000000 habmapslib-2.0.1/habmapslib/HabMapsMessage.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     1694 2023-04-13 16:43:51.000000 habmapslib-2.0.1/habmapslib/InitChecks.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     2727 2023-04-16 09:28:20.000000 habmapslib-2.0.1/habmapslib/MapTracker.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     3816 2023-04-16 09:21:52.000000 habmapslib-2.0.1/habmapslib/Parser.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)      105 2023-04-13 16:43:51.000000 habmapslib-2.0.1/habmapslib/__init__.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)        0 2023-04-13 16:43:51.000000 habmapslib-2.0.1/habmapslib/__main__.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     1107 2023-04-13 16:43:51.000000 habmapslib-2.0.1/habmapslib/cli.py
+-rw-r--r--   0 alvaroperis   (501) staff       (20)      866 2023-04-16 09:08:20.000000 habmapslib-2.0.1/habmapslib/confyaml.py
+drwxr-xr-x   0 alvaroperis   (501) staff       (20)        0 2023-04-16 09:51:32.430341 habmapslib-2.0.1/habmapslib.egg-info/
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     8969 2023-04-16 09:51:31.000000 habmapslib-2.0.1/habmapslib.egg-info/PKG-INFO
+-rw-r--r--   0 alvaroperis   (501) staff       (20)      482 2023-04-16 09:51:32.000000 habmapslib-2.0.1/habmapslib.egg-info/SOURCES.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)        1 2023-04-16 09:51:31.000000 habmapslib-2.0.1/habmapslib.egg-info/dependency_links.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)       43 2023-04-16 09:51:31.000000 habmapslib-2.0.1/habmapslib.egg-info/requires.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)       11 2023-04-16 09:51:31.000000 habmapslib-2.0.1/habmapslib.egg-info/top_level.txt
+-rw-r--r--   0 alvaroperis   (501) staff       (20)       38 2023-04-16 09:51:32.432707 habmapslib-2.0.1/setup.cfg
+-rw-r--r--   0 alvaroperis   (501) staff       (20)     1325 2023-04-16 09:51:21.000000 habmapslib-2.0.1/setup.py
```

### Comparing `habmapslib-2.0.0/LICENSE.txt` & `habmapslib-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `habmapslib-2.0.0/PKG-INFO` & `habmapslib-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habmapslib
-Version: 2.0.0
+Version: 2.0.1
 Summary: Librería para el acceso a habmaps
 Home-page: https://github.com/alpeza/habmapsgateway
 Author: Alpeza
 Author-email: 
 Project-URL: Bug Reports, https://github.com/alpeza/habmapsgateway/issues
 Project-URL: Funding, https://github.com/alpeza/habmapsgateway/issues
 Project-URL: Say Thanks!, https://github.com/alpeza/habmapsgateway/issues
```

### Comparing `habmapslib-2.0.0/README.md` & `habmapslib-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `habmapslib-2.0.0/habmapslib/Appender.py` & `habmapslib-2.0.1/habmapslib/Appender.py`

 * *Files identical despite different names*

### Comparing `habmapslib-2.0.0/habmapslib/GPSAppender.py` & `habmapslib-2.0.1/habmapslib/GPSAppender.py`

 * *Files identical despite different names*

### Comparing `habmapslib-2.0.0/habmapslib/HMTail.py` & `habmapslib-2.0.1/habmapslib/HMTail.py`

 * *Files identical despite different names*

### Comparing `habmapslib-2.0.0/habmapslib/HabMapsMessage.py` & `habmapslib-2.0.1/habmapslib/HabMapsMessage.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,21 +59,21 @@
         valid = True
 
         if self._track['hab']['pos']['lat'] == -1.0 or self._track['hab']['pos']['lon'] == -1.0:
             logging.error(
                 'Please set a valid hab pos with setHabPosition([<float : lat>, <float : lon>])')
             valid = False
 
-        if self._track['hab']['id'] == '':
-            logging.error('Please set a habid with setHabId(<string : id>)')
+        if self._track['hab']['hid'] == '':
+            logging.error('Please set a habid with setHabId(<string : hid>)')
             valid = False
 
-        if self._track['basestation']['id'] == '':
+        if self._track['basestation']['bid'] == '':
             logging.error(
-                'Please set a habid with setBasestationId(<string : id>)')
+                'Please set a habid with setBasestationId(<string : bid>)')
             valid = False
 
         if self._track['ftime'] == '':
             self._setTS()
 
         return valid
 
@@ -97,11 +97,11 @@
         if len(bspos) == 3 and float(bspos[2]) != 0.0:
             self.addSignal('BStationHeight', float(bspos[2]))
 
     def addSignal(self, key, value):
         self._track['hab']['payload'][key] = value
 
     def setHabId(self, id):
-        self._track['hab']['id'] = id.replace(" ", "-")
+        self._track['hab']['hid'] = id.replace(" ", "-")
 
     def setBasestationId(self, id):
-        self._track['basestation']['id'] = id.replace(" ", "-")
+        self._track['basestation']['bid'] = id.replace(" ", "-")
```

### Comparing `habmapslib-2.0.0/habmapslib/InitChecks.py` & `habmapslib-2.0.1/habmapslib/InitChecks.py`

 * *Files identical despite different names*

### Comparing `habmapslib-2.0.0/habmapslib/MapTracker.py` & `habmapslib-2.0.1/habmapslib/MapTracker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,74 +1,82 @@
 import paho.mqtt.client as mqtt
-import sched, time, threading,os
-import json,logging, traceback
+import sched
+import time
+import threading
+import os
+import json
+import logging
+import traceback
 from datetime import datetime, timedelta
 LOGLEVEL = os.environ.get('HABLIB_LOGLEVEL', 'INFO').upper()
-FORMATTER = os.environ.get('HABLIB_FORMAT', '[%(asctime)s] p%(process)s {%(pathname)s:%(lineno)d} %(levelname)s - %(message)s')
+FORMATTER = os.environ.get(
+    'HABLIB_FORMAT', '[%(asctime)s] p%(process)s {%(pathname)s:%(lineno)d} %(levelname)s - %(message)s')
 LOGFILE = os.environ.get('HABLIB_LOGFILE', '/tmp/hablibclient.log')
-logging.basicConfig(level=LOGLEVEL, format=FORMATTER, handlers=[logging.FileHandler(LOGFILE),logging.StreamHandler()])
+logging.basicConfig(level=LOGLEVEL, format=FORMATTER, handlers=[
+                    logging.FileHandler(LOGFILE), logging.StreamHandler()])
+
 
 class MapTracker(object):
     """Cliente de MQTT para maptracker"""
-    def __init__(self, id="default-station-id",
+
+    def __init__(self, bid="default-station-id",
                  mqtt_url="localhost",
                  mqtt_port=1883,
                  publish="hablistener",
                  alive=60,
                  user='habmaps',
                  password='root'):
         super(MapTracker, self).__init__()
         logging.info("Starting new MapTracker Client ...")
         self.client = mqtt.Client()
-        self.client.username_pw_set(username=user,password=password)
+        self.client.username_pw_set(username=user, password=password)
 
         self.mqtt_url = mqtt_url
         self.mqtt_port = mqtt_port
         self.topic = publish
-        self.id = id
+        self.bid = bid
         self.alive = alive
 
         self.s = sched.scheduler(time.time, time.sleep)
 
         self.alive_flag = False
 
-
     def sendAliveMessage(self):
         msg = {
             "type": "health",
             "ftime": datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
-            "id": self.id
+            "bid": self.bid
         }
         logging.debug(msg)
-        self.sendMessage(msg);
-
+        self.sendMessage(msg)
 
     def _runIamAlive(self):
         logging.info("Sending Alive Message ...")
         self.sendAliveMessage()
         self.s.enter(self.alive, 1, self._runIamAlive)
+
     def _runAlive(self):
         logging.info("Starting health signal ...")
         self.s.enter(self.alive, 1, self._runIamAlive)
         self.s.run()
 
     def startAlive(self):
         threading.Timer(1, self._runAlive).start()
 
     def sendMessage(self, message):
         logging.info("Sending message ...")
         logging.debug(json.dumps(message))
         try:
-            self.client.connect(self.mqtt_url,self.mqtt_port,60)
-            self.client.publish(self.topic, json.dumps(message));
-            self.client.disconnect();
+            self.client.connect(self.mqtt_url, self.mqtt_port, 60)
+            self.client.publish(self.topic, json.dumps(message))
+            self.client.disconnect()
             return {"isOK": True, "reason": ""}
         except Exception as e:
             logging.error(e)
             logging.error(traceback.format_exc())
             return {"isOK": False, "reason": str(e)}
 
-    def sendHabMessage(self,hm):
-        hm.setBasestationId(self.id)
+    def sendHabMessage(self, hm):
+        hm.setBasestationId(self.bid)
         if hm.isValidMessage() == False:
             raise ValueError("Please inform all required data")
         return self.sendMessage(hm.getMessage())
```

### Comparing `habmapslib-2.0.0/habmapslib/Parser.py` & `habmapslib-2.0.1/habmapslib/Parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,73 +1,79 @@
-import logging, os
+import traceback
+import logging
+import os
 from datetime import datetime
 from . import HMTail
 from . import HabMapsMessage
 from . import MapTracker
 from . import GPSAppender
 LOGLEVEL = os.environ.get('HABLIB_LOGLEVEL', 'INFO').upper()
-FORMATTER = os.environ.get('HABLIB_FORMAT', '%(asctime)s - %(name)s - %(levelname)s - %(message)s')
+FORMATTER = os.environ.get(
+    'HABLIB_FORMAT', '%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 LOGFILE = os.environ.get('HABLIB_LOGFILE', '/tmp/hablibclient.log')
-logging.basicConfig(level=LOGLEVEL, format=FORMATTER, handlers=[logging.FileHandler(LOGFILE), logging.StreamHandler()])
-import traceback
+logging.basicConfig(level=LOGLEVEL, format=FORMATTER, handlers=[
+                    logging.FileHandler(LOGFILE), logging.StreamHandler()])
+
 
 class Parser(object):
     """docstring for Parser."""
 
     def __init__(self, confHandler):
         super(Parser, self).__init__()
         self.ch = confHandler.getConfig()
-        self.mt = MapTracker.MapTracker(id=self.ch['basestation']['id'],
+        self.mt = MapTracker.MapTracker(bid=self.ch['basestation']['bid'],
                                         mqtt_url=self.ch['mqtt']['url'],
                                         mqtt_port=int(self.ch['mqtt']['port']),
                                         user=self.ch['mqtt']['user'],
                                         publish=self.ch['mqtt']['topic'],
                                         alive=int(self.ch['mqtt']['alive']),
                                         password=self.ch['mqtt']['password']
                                         )
         self.gps_appender = GPSAppender.GPSAppender(self.ch)
-        #self.mt.startAlive()
+        # self.mt.startAlive()
 
     def parseline(self, line, definition):
         """ Core de parseo, aqui realiza la serialización a json de la traza retornando un HabMapsMessage"""
         trace = line.split('|')
         definitions = definition.split('|')
         i = 0
         hm = HabMapsMessage.HabMapsMessage()
 
         if len(trace) != len(definitions):
-            logging.error("Invalid frame: " + str(len(trace)) + " != " + str(len(definitions)))
+            logging.error("Invalid frame: " + str(len(trace)) +
+                          " != " + str(len(definitions)))
             logging.error(line)
             return None
 
         for el in definitions:
             if el != '':
                 if el == '$time':
                     date_composed = datetime.now().strftime("%Y-%m-%d") + " " + trace[i][0:2] + ":" + trace[i][
-                                                                                                      2:4] + ":" + \
-                                    trace[i][4:6]
+                        2:4] + ":" + \
+                        trace[i][4:6]
                     hm.setTimeStamp(date_composed)
                 elif el == '$pos':
                     pos = trace[i].split(',')
                     hm.setHabPosition([float(pos[0]), float(pos[1])])
-                elif el == '$id':
+                elif el == '$hid':
                     hm.setHabId(trace[i])
                 # Parseo de señales
                 else:
                     try:
                         hm.addSignal(el, float(trace[i]))
                     except Exception as e:
                         logging.info("Not a float signal")
                         hm.addSignal(el, trace[i])
             i += 1
         return hm
 
     def _print_line(self, txt):
         """ Call back, funcion que se llama por cada linea que se lee"""
-        logging.debug(datetime.now().strftime("%Y-%m-%d %H:%M:%S") + "  --> New line in file:")
+        logging.debug(datetime.now().strftime(
+            "%Y-%m-%d %H:%M:%S") + "  --> New line in file:")
         logging.debug(txt)
         # 1.- Parseamos la traza que nos llega de lora
         try:
             hm = self.parseline(txt, self.ch['frame']['format'])
             if hm:
                 # 2.- Obtenemos la ultima traza de gps
                 pos_gps = self.gps_appender.getValueAsArray()
@@ -75,13 +81,12 @@
                 # 3.- Transmitimos el mensaje
                 self.mt.sendHabMessage(hm)
         except Exception as e:
             logging.error("Something went wrong ...")
             logging.error(e)
             logging.error(traceback.format_exc())
 
-
     def run(self):
         """ Función que lanza el parser """
         t = HMTail.Tail(self.ch['frame']['file'])
         t.register_callback(self._print_line)
-        t.follow(s=float(self.ch['frame']['refresh']))
+        t.follow(s=float(self.ch['frame']['refresh']))
```

### Comparing `habmapslib-2.0.0/habmapslib/cli.py` & `habmapslib-2.0.1/habmapslib/cli.py`

 * *Files identical despite different names*

### Comparing `habmapslib-2.0.0/habmapslib/confyaml.py` & `habmapslib-2.0.1/habmapslib/confyaml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-conf='''basestation:
+conf = '''basestation:
   id: "id-de-mi-estacion"
   appenders:
     gpsappender:
       file: '/Users/alvaroperis/ArchLab/habmapsgateway/demotraces/gps.appender'
       regexselect: '\[.*\]\|(.*)\|(.*),(.*)\|.*\|'
       mapping:
         - "height"
@@ -16,13 +16,13 @@
   password: "root"
   alive: 60
 frame:
   # Definición de la trama donde
   # $time : Es la hora expresada en HHMMSS
   # $pos : Es la posición gps del hab expresada en lat,lon
   # $id  : Es el identificador del hab
-  format: "$time|AlturaGPS|$pos|VelocidadHorizontalGPS|Temperatura|Presion|AlturaBarometrica|$id|"
+  format: "$time|AlturaGPS|$pos|VelocidadHorizontalGPS|Temperatura|Presion|AlturaBarometrica|$hid|"
   # Fichero donde se van insertando las trazas de LoRa
   file: "/Users/alvaroperis/ArchLab/habmapsgateway/demotraces/out.log"
   # Cada cuantos segundos se mira el fichero de envio
   refresh: 1
-'''
+'''
```

### Comparing `habmapslib-2.0.0/habmapslib.egg-info/PKG-INFO` & `habmapslib-2.0.1/habmapslib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: habmapslib
-Version: 2.0.0
+Version: 2.0.1
 Summary: Librería para el acceso a habmaps
 Home-page: https://github.com/alpeza/habmapsgateway
 Author: Alpeza
 Author-email: 
 Project-URL: Bug Reports, https://github.com/alpeza/habmapsgateway/issues
 Project-URL: Funding, https://github.com/alpeza/habmapsgateway/issues
 Project-URL: Say Thanks!, https://github.com/alpeza/habmapsgateway/issues
```

### Comparing `habmapslib-2.0.0/setup.py` & `habmapslib-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="habmapslib",
     include_package_data=True,
-    version="2.0.0",
+    version="2.0.1",
     author="Alpeza",
     author_email="",
     description="Librería para el acceso a habmaps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/alpeza/habmapsgateway",
     packages=setuptools.find_packages(),
```

