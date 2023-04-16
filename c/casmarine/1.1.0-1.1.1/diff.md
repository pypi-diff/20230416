# Comparing `tmp/casmarine-1.1.0.tar.gz` & `tmp/casmarine-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casmarine-1.1.0.tar", last modified: Sat Apr 15 13:49:35 2023, max compression
+gzip compressed data, was "casmarine-1.1.1.tar", last modified: Sun Apr 16 09:42:45 2023, max compression
```

## Comparing `casmarine-1.1.0.tar` & `casmarine-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:49:35.639343 casmarine-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-15 13:49:19.000000 casmarine-1.1.0/LICENSE.
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-15 13:49:35.635343 casmarine-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:49:19.000000 casmarine-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:49:35.635343 casmarine-1.1.0/casmarine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 13:49:19.000000 casmarine-1.1.0/casmarine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-04-15 13:49:19.000000 casmarine-1.1.0/casmarine/cserial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-15 13:49:19.000000 casmarine-1.1.0/casmarine/csocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:49:35.635343 casmarine-1.1.0/casmarine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-15 13:49:35.000000 casmarine-1.1.0/casmarine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-15 13:49:35.000000 casmarine-1.1.0/casmarine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 13:49:35.000000 casmarine-1.1.0/casmarine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-15 13:49:35.000000 casmarine-1.1.0/casmarine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 13:49:35.000000 casmarine-1.1.0/casmarine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 13:49:35.639343 casmarine-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-15 13:49:19.000000 casmarine-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 13:49:35.635343 casmarine-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-15 13:49:19.000000 casmarine-1.1.0/tests/test_cserial.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-15 13:49:19.000000 casmarine-1.1.0/tests/test_csocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:42:45.911314 casmarine-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-16 09:42:34.000000 casmarine-1.1.1/LICENSE.
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-16 09:42:45.911314 casmarine-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:42:34.000000 casmarine-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:42:45.911314 casmarine-1.1.1/casmarine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:42:34.000000 casmarine-1.1.1/casmarine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9845 2023-04-16 09:42:34.000000 casmarine-1.1.1/casmarine/cserial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-04-16 09:42:34.000000 casmarine-1.1.1/casmarine/csocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:42:45.911314 casmarine-1.1.1/casmarine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-16 09:42:45.000000 casmarine-1.1.1/casmarine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-16 09:42:45.000000 casmarine-1.1.1/casmarine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 09:42:45.000000 casmarine-1.1.1/casmarine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-16 09:42:45.000000 casmarine-1.1.1/casmarine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-16 09:42:45.000000 casmarine-1.1.1/casmarine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 09:42:45.911314 casmarine-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-16 09:42:34.000000 casmarine-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:42:45.911314 casmarine-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-16 09:42:34.000000 casmarine-1.1.1/tests/test_cserial.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-16 09:42:34.000000 casmarine-1.1.1/tests/test_csocket.py
```

### Comparing `casmarine-1.1.0/LICENSE.` & `casmarine-1.1.1/LICENSE.`

 * *Files identical despite different names*

### Comparing `casmarine-1.1.0/PKG-INFO` & `casmarine-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casmarine
-Version: 1.1.0
+Version: 1.1.1
 Summary: Extendable communication library with support for various protocols for the use of CASMarine ROV team
 Home-page: https://github.com/CASMarine/Communication
 Author: Furkan Kırlangıç, Begüm İpek
 Author-email: kirlangicfurkan01@gmail.com
 Project-URL: Bug Tracker, https://github.com/CASMarine/Communication/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `casmarine-1.1.0/casmarine/cserial.py` & `casmarine-1.1.1/casmarine/cserial.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 
 
 class Protocol():
     CONST_DATA_SIZE = 8
 
     def __init__(self, baud=115200, port='/dev/ttyTHS1') -> None:
-        self.__ser = serial.Serial(port=port, baudrate=baud)
+        self.__ser = serial.Serial(port=port, baudrate=baud, timeout=0.1)
         self.__ack_size = 0
         self.__post_time_sleep = 15 / baud
         self.variables = [
                 _Data(Index.HeaderL, 'B', 0x11, rw=False),
                 _Data(Index.HeaderH, 'B', 0x55, rw=False),
                 _Data(Index.PackageSize, 'B'),
                 _Data(Index.Command, 'B'),
@@ -117,19 +117,18 @@
                 _Data(Index.Baudrate, 'I'),
                 _Data(Index.CRC, 'I'),
               ]
 
     def __write_bus(self, data):
         self.__ser.write(data)
 
-    def __read_bus(self, size):
-        data = self.__ser.read(size)
-        if (len(data) == size):
+    def __read_bus(self, byte_count):
+        data = self.__ser.read(byte_count)
+        if (len(data) == byte_count):
             return data
-        #return self.__ser.read(size=size)
         return None
     
     def get_ack_size(self) -> int:
         return self.__ack_size
 
     def __set_variables(self, idx_list=[], value_list=[]):
```

### Comparing `casmarine-1.1.0/casmarine/csocket.py` & `casmarine-1.1.1/casmarine/csocket.py`

 * *Files identical despite different names*

### Comparing `casmarine-1.1.0/casmarine.egg-info/PKG-INFO` & `casmarine-1.1.1/casmarine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casmarine
-Version: 1.1.0
+Version: 1.1.1
 Summary: Extendable communication library with support for various protocols for the use of CASMarine ROV team
 Home-page: https://github.com/CASMarine/Communication
 Author: Furkan Kırlangıç, Begüm İpek
 Author-email: kirlangicfurkan01@gmail.com
 Project-URL: Bug Tracker, https://github.com/CASMarine/Communication/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `casmarine-1.1.0/setup.py` & `casmarine-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="casmarine",
-    version="1.1.0",
+    version="1.1.1",
     author="Furkan Kırlangıç, Begüm İpek",
     author_email="kirlangicfurkan01@gmail.com",
     description="Extendable communication library with support for various protocols for the use of CASMarine ROV team",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CASMarine/Communication",
     project_urls={
```

