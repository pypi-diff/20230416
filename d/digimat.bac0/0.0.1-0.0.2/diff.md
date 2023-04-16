# Comparing `tmp/digimat.bac0-0.0.1.tar.gz` & `tmp/digimat.bac0-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digimat.bac0-0.0.1.tar", last modified: Sat Apr 15 22:20:19 2023, max compression
+gzip compressed data, was "digimat.bac0-0.0.2.tar", last modified: Sun Apr 16 10:30:59 2023, max compression
```

## Comparing `digimat.bac0-0.0.1.tar` & `digimat.bac0-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-15 22:20:19.718017 digimat.bac0-0.0.1/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-15 22:20:19.717782 digimat.bac0-0.0.1/PKG-INFO
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       38 2023-04-15 22:20:19.718103 digimat.bac0-0.0.1/setup.cfg
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      958 2023-04-14 15:42:53.000000 digimat.bac0-0.0.1/setup.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-15 22:20:19.714317 digimat.bac0-0.0.1/src/
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-15 22:20:19.714854 digimat.bac0-0.0.1/src/digimat/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       57 2014-09-24 08:13:04.000000 digimat.bac0-0.0.1/src/digimat/__init__.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-15 22:20:19.717417 digimat.bac0-0.0.1/src/digimat/bac0/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       25 2023-04-15 20:24:12.000000 digimat.bac0-0.0.1/src/digimat/bac0/__init__.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     4630 2023-04-15 22:18:00.000000 digimat.bac0-0.0.1/src/digimat/bac0/bacnet.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-15 22:20:19.716930 digimat.bac0-0.0.1/src/digimat.bac0.egg-info/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-15 22:20:19.000000 digimat.bac0-0.0.1/src/digimat.bac0.egg-info/PKG-INFO
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      375 2023-04-15 22:20:19.000000 digimat.bac0-0.0.1/src/digimat.bac0.egg-info/SOURCES.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-15 22:20:19.000000 digimat.bac0-0.0.1/src/digimat.bac0.egg-info/dependency_links.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-15 22:20:19.000000 digimat.bac0-0.0.1/src/digimat.bac0.egg-info/namespace_packages.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-15 16:54:48.000000 digimat.bac0-0.0.1/src/digimat.bac0.egg-info/not-zip-safe
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       28 2023-04-15 22:20:19.000000 digimat.bac0-0.0.1/src/digimat.bac0.egg-info/requires.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-15 22:20:19.000000 digimat.bac0-0.0.1/src/digimat.bac0.egg-info/top_level.txt
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-16 10:30:59.400419 digimat.bac0-0.0.2/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-16 10:30:59.400153 digimat.bac0-0.0.2/PKG-INFO
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       38 2023-04-16 10:30:59.400515 digimat.bac0-0.0.2/setup.cfg
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      958 2023-04-16 09:32:27.000000 digimat.bac0-0.0.2/setup.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-16 10:30:59.397030 digimat.bac0-0.0.2/src/
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-16 10:30:59.397562 digimat.bac0-0.0.2/src/digimat/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       57 2014-09-24 08:13:04.000000 digimat.bac0-0.0.2/src/digimat/__init__.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-16 10:30:59.399812 digimat.bac0-0.0.2/src/digimat/bac0/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       25 2023-04-15 20:24:12.000000 digimat.bac0-0.0.2/src/digimat/bac0/__init__.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     8245 2023-04-16 10:27:22.000000 digimat.bac0-0.0.2/src/digimat/bac0/bacnet.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-04-16 10:30:59.399323 digimat.bac0-0.0.2/src/digimat.bac0.egg-info/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      281 2023-04-16 10:30:59.000000 digimat.bac0-0.0.2/src/digimat.bac0.egg-info/PKG-INFO
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      375 2023-04-16 10:30:59.000000 digimat.bac0-0.0.2/src/digimat.bac0.egg-info/SOURCES.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-16 10:30:59.000000 digimat.bac0-0.0.2/src/digimat.bac0.egg-info/dependency_links.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-16 10:30:59.000000 digimat.bac0-0.0.2/src/digimat.bac0.egg-info/namespace_packages.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-04-15 16:54:48.000000 digimat.bac0-0.0.2/src/digimat.bac0.egg-info/not-zip-safe
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       28 2023-04-16 10:30:59.000000 digimat.bac0-0.0.2/src/digimat.bac0.egg-info/requires.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-04-16 10:30:59.000000 digimat.bac0-0.0.2/src/digimat.bac0.egg-info/top_level.txt
```

### Comparing `digimat.bac0-0.0.1/setup.py` & `digimat.bac0-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='digimat.bac0',
-    version='0.0.1',
+    version='0.0.2',
     description='Digimat BACnet BAC0 Wrapper',
     namespace_packages=['digimat'],
     author='Frederic Hess',
     author_email='fhess@st-sa.ch',
     url='http://www.digimat.ch',
     license='PSF',
     packages=find_packages('src'),
```

### Comparing `digimat.bac0-0.0.1/src/digimat/bac0/bacnet.py` & `digimat.bac0-0.0.2/src/digimat/bac0/bacnet.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,52 +4,152 @@
 # import time
 import logging
 import logging.handlers
 
 from prettytable import PrettyTable
 
 
+class BACBag(object):
+    def __init__(self, device, key=None):
+        self._device=device
+        self._points=[]
+        self._pointsByName={}
+        if key:
+            self.add(key)
+
+    def __repr__(self):
+        return '<%s[%s](%d points)>' % (self.__class__.__name__, self.device.name,
+            len(self._points))
+
+    @property
+    def logger(self):
+        return self._device.logger
+
+    @property
+    def device(self):
+        return self._device
+
+    def points(self):
+        return self._points
+
+    def point(self, name):
+        try:
+            return self._pointsByName[name]
+        except:
+            pass
+        try:
+            return self._points[int(name)]
+        except:
+            pass
+
+    def __getitem__(self, key):
+        return self.point(key)
+
+    def count(self):
+        return len(self._points)
+
+    def __len__(self):
+        return self.count()
+
+    def add(self, key):
+        if key:
+            if type(key)==list:
+                points=key
+            else:
+                points=self.device.points(key)
+            if points:
+                for point in points:
+                    if not self.point(point.properties.name):
+                        self._points.append(point)
+                        self._pointsByName[point.properties.name]=point
+
+    def dump(self):
+        if self._points:
+            t=PrettyTable()
+            t.field_names=['#', 'name', 'type', 'value', 'unit', 'description']
+            t.align['#']='l'
+            t.align['name']='l'
+            t.align['type']='l'
+            t.align['value']='r'
+            t.align['unit']='l'
+            t.align['description']='l'
+            for n in range(len(self._points)):
+                point=self._points[n]
+                t.add_row([n, point.properties.name, point.properties.type, point.value, point.units, point.properties.description])
+            print(t)
+
+
 class BACDevice(object):
-    def __init__(self, bacnet, ip, did):
-        self._bacnet=bacnet
+    def __init__(self, parent, ip, did):
+        self._parent=parent
         self._did=did
         self._ip=ip
         self.logger.info('Creating device %s:%d' % (ip, did))
-        self._device=BAC0.device(ip, did, bacnet.bac0)
+        self._device=BAC0.device(ip, did, parent.bac0)
 
-    @property
-    def bacnet(self):
-        return self._bacnet
+    def __repr__(self):
+        return '<%s:%d(%s:%s, %s, %d points)>' % (self.__class__.__name__, self._did,
+            self.vendorName, self.modelName, self.systemStatus,
+            len(self._device.points))
 
     @property
     def logger(self):
-        return self.bacnet.logger
+        return self._parent.logger
 
     @property
     def bac0(self):
-        return self.bacnet.bac0
+        return self._parent.bac0
 
     @property
     def properties(self):
         return self._device.bacnet_properties
 
     @property
     def name(self):
         return self.properties['objectName']
 
     @property
+    def did(self):
+        return self._did
+
+    @property
+    def ip(self):
+        return self._ip
+
+    @property
+    def systemStatus(self):
+        return self.properties['systemStatus']
+
+    @property
+    def vendorName(self):
+        return self.properties['vendorName']
+
+    @property
+    def vendorIdentifier(self):
+        return self.properties['vendorIdentifier']
+
+    @property
+    def modelName(self):
+        return self.properties['modelName']
+
+    @property
     def description(self):
         return self.properties['description']
 
+    def count(self, key=None, objectType=None, outOfService=False):
+        return len(self.points(key, objectType, outOfService))
+
     @functools.cache
-    def points(self, key=None, objectType=None):
+    def points(self, key=None, objectType=None, outOfService=False):
         items=[]
         if key:
             key=key.lower()
         for point in self._device.points:
+            if not outOfService and point.bacnet_properties['outOfService']:
+                continue
             if objectType and objectType!=point.properties.type:
                 continue
             if key:
                 if key not in point.properties.name.lower() and \
                         key not in point.properties.description.lower():
                     continue
             items.append(point)
@@ -75,33 +175,36 @@
 
     def __getitem__(self, key):
         try:
             return self.points(key)[0]
         except:
             pass
 
-    def dump(self, points=None):
+    def dump(self, points=None, outOfService=False):
         if type(points) is not list:
-            points=self.points(points)
+            points=self.points(points, outOfService=outOfService)
         if points:
             t=PrettyTable()
             t.field_names=['name', 'type', 'value', 'unit', 'description']
             t.align['name']='l'
             t.align['type']='l'
-            t.align['value']='l'
+            t.align['value']='r'
             t.align['unit']='l'
             t.align['description']='l'
             for point in points:
                 t.add_row([point.properties.name, point.properties.type, point.value, point.units, point.properties.description])
             print(t)
 
+    def bag(self, key=None):
+        return BACBag(self, key)
+
 
 class BAC(object):
     def __init__(self, network, ipRouter=None, logServer='localhost', logLevel=logging.DEBUG):
-        logger=logging.getLogger("BACNET(%s)" % network)
+        logger=logging.getLogger("BAC(%s)" % network)
         logger.setLevel(logLevel)
         socketHandler = logging.handlers.SocketHandler(logServer, logging.handlers.DEFAULT_TCP_LOGGING_PORT)
         logger.addHandler(socketHandler)
         self._logger=logger
 
         self._network=network
         self._bac0=None
@@ -117,14 +220,17 @@
             self.logger.info('Using BAC0 v%s' % BAC0.version)
             self.logger.info('BAC0:%s' % self._bac0)
 
         self._devices={}
 
         # self.open()
 
+    def __repr__(self):
+        return '<%s:%s(%d devices)>' % (self.__class__.__name__, self._network, len(self._devices))
+
     @property
     def logger(self):
         return self._logger
 
     @property
     def bac0(self):
         return self._bac0
@@ -135,19 +241,19 @@
 
     def close(self):
         if self._bac0:
             self._bac0.disconnect()
 
     def device(self, did):
         try:
-            return self._devices[did]
+            return self._devices[int(did)]
         except:
             pass
 
-    def devices(self):
+    def devices(self, key=None):
         return self._devices.values()
 
     def whois(self, autoDeclare=False):
         if self._bac0:
             items=self._bac0.whois()
             if items and autoDeclare:
                 for item in items:
@@ -163,15 +269,26 @@
             self._devices[did]=device
             return device
 
     def __getitem__(self, key):
         return self.device(key)
 
     def dump(self):
-        pass
-
-    def table(self):
-        pass
+        devices=self.devices()
+        if devices:
+            t=PrettyTable()
+            t.field_names=['name', 'id', 'ip', 'vendor', 'model', ' status', 'description', 'points']
+            t.align['*']='l'
+            t.align['name']='l'
+            t.align['vendor']='l'
+            t.align['model']='l'
+            t.align['description']='l'
+            for device in devices:
+                t.add_row([device.name, device.did, device.ip,
+                           device.vendorName, device.modelName, device.systemStatus,
+                           device.description,
+                           device.count()])
+            print(t)
 
 
 if __name__=='__main__':
     pass
```

