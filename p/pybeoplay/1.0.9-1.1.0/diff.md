# Comparing `tmp/pybeoplay-1.0.9.tar.gz` & `tmp/pybeoplay-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybeoplay-1.0.9.tar", last modified: Sat Jan 14 23:14:06 2023, max compression
+gzip compressed data, was "pybeoplay-1.1.0.tar", last modified: Sun Apr 16 01:30:09 2023, max compression
```

## Comparing `pybeoplay-1.0.9.tar` & `pybeoplay-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-01-14 23:14:06.104637 pybeoplay-1.0.9/
--rw-rw-rw-   0        0        0     1074 2021-01-23 16:53:58.000000 pybeoplay-1.0.9/LICENSE
--rw-rw-rw-   0        0        0     1960 2023-01-14 23:14:06.105636 pybeoplay-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1296 2023-01-07 03:41:34.000000 pybeoplay-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-01-14 23:14:06.081638 pybeoplay-1.0.9/pybeoplay/
--rw-rw-rw-   0        0        0    27936 2023-01-14 23:12:07.000000 pybeoplay-1.0.9/pybeoplay/__init__.py
--rw-rw-rw-   0        0        0     1489 2023-01-03 05:52:49.000000 pybeoplay-1.0.9/pybeoplay/const.py
-drwxrwxrwx   0        0        0        0 2023-01-14 23:14:06.102664 pybeoplay-1.0.9/pybeoplay.egg-info/
--rw-rw-rw-   0        0        0     1960 2023-01-14 23:14:06.000000 pybeoplay-1.0.9/pybeoplay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-01-14 23:14:06.000000 pybeoplay-1.0.9/pybeoplay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-14 23:14:06.000000 pybeoplay-1.0.9/pybeoplay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-01-24 04:42:02.000000 pybeoplay-1.0.9/pybeoplay.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-01-14 23:14:06.000000 pybeoplay-1.0.9/pybeoplay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-01-14 23:14:06.108638 pybeoplay-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1285 2023-01-14 23:10:36.000000 pybeoplay-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:30:09.300606 pybeoplay-1.1.0/
+-rw-rw-rw-   0        0        0     1074 2021-01-23 16:53:58.000000 pybeoplay-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1960 2023-04-16 01:30:09.302135 pybeoplay-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1296 2023-01-07 03:41:34.000000 pybeoplay-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 01:30:09.267517 pybeoplay-1.1.0/pybeoplay/
+-rw-rw-rw-   0        0        0    29512 2023-04-15 21:34:07.000000 pybeoplay-1.1.0/pybeoplay/__init__.py
+-rw-rw-rw-   0        0        0     2315 2023-04-16 01:28:12.000000 pybeoplay-1.1.0/pybeoplay/const.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:30:09.295507 pybeoplay-1.1.0/pybeoplay.egg-info/
+-rw-rw-rw-   0        0        0     1960 2023-04-16 01:30:09.000000 pybeoplay-1.1.0/pybeoplay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-04-16 01:30:09.000000 pybeoplay-1.1.0/pybeoplay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 01:30:09.000000 pybeoplay-1.1.0/pybeoplay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-01-24 04:42:02.000000 pybeoplay-1.1.0/pybeoplay.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-04-16 01:30:09.000000 pybeoplay-1.1.0/pybeoplay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-16 01:30:09.305477 pybeoplay-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1285 2023-04-15 21:20:45.000000 pybeoplay-1.1.0/setup.py
```

### Comparing `pybeoplay-1.0.9/LICENSE` & `pybeoplay-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybeoplay-1.0.9/PKG-INFO` & `pybeoplay-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pybeoplay
-Version: 1.0.9
+Version: 1.1.0
 Summary: BeoPlay API for Python
 Home-page: https://github.com/giachello/pybeoplay
-Download-URL: https://github.com/giachello/pybeoplay/tarball/1.0.9
+Download-URL: https://github.com/giachello/pybeoplay/tarball/1.1.0
 Author: Giovanni Iachello
 Author-email: giovanni.iachello@gmail.com
 License: MIT License
 Keywords: beoplay,pybeoplay,B&O,Bang & Olufsen
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pybeoplay-1.0.9/README.md` & `pybeoplay-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pybeoplay-1.0.9/pybeoplay/__init__.py` & `pybeoplay-1.1.0/pybeoplay/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,14 +98,18 @@
         return self._softwareVersion
 
     @property
     def hardwareVersion(self):
         """Return the device serial number."""
         return self._hardwareVersion
 
+    @property
+    def remote_commands(self):
+        """Get the list of available remote commands"""
+        return BEOPLAY_REMOTE_COMMANDS
 
     ###############################################################
     # ASYNC BASED NETWORK CALLS
     ###############################################################
 
     async def async_getReq(self, path):
         """Non blocking GET call to the speaker, with a given path."""
@@ -392,14 +396,39 @@
         if instantplay:
             await self.async_postReq(
                 "POST", BEOPLAY_URL_PLAYQUEUE + BEOPLAY_URL_PLAYQUEUE_INSTANT, queueItem
             )
         else:
             await self.async_postReq("POST", BEOPLAY_URL_PLAYQUEUE, queueItem)
 
+    async def async_remote_command(self, command : str, toBeReleased :bool = False):
+        """
+        Send a remote command to the device. Command needs to be one of:  
+
+        Cursor/Select, Cursor/Up, Cursor/Down, Cursor/Left, Cursor/Right, Cursor/Exit, Cursor/Back, Cursor/PageUp, Cursor/PageDown, Cursor/Clear, 
+        Stream/Play, Stream/Stop, Stream/Pause, Stream/Wind, Stream/Rewind, Stream/Forward, Stream/Backward, 
+        List/StepUp, List/StepDown, List/PreviousElement, List/Shuffle, List/Repeat, 
+        Menu/Root, Menu/Option, Menu/Setup, Menu/Contents, Menu/Favorites, Menu/ElectronicProgramGuide, Menu/VideoOnDemand, Menu/Text, Menu/HbbTV,Menu/HomeControl, 
+        Device/Information, Device/Eject, Device/TogglePower, Device/Languages, Device/Subtitles, Device/OneWayJoin, Device/Mots, 
+        Record/Record, 
+        Generic/Blue, Generic/Red, Generic/Green, Generic/Yellow.
+        
+        toBeReleased: true if this is a button press that is held. Needs to be completed by calling async_remote_release.
+
+        """
+        if (command not in BEOPLAY_REMOTE_COMMANDS):
+            return
+        await self.async_postReq("POST", BEOPLAY_REMOTE_PREFIX + command, {"toBeReleased": toBeReleased})
+
+    async def async_remote_release(self, command : str):
+        if (command not in BEOPLAY_REMOTE_COMMANDS):
+            return
+        await self.async_postReq("POST", BEOPLAY_REMOTE_PREFIX + command + BEOPLAY_URL_RELEASE, {})
+
+
     ###############################################################
     # REQUESTS (BLOCKING) NETWORK CALLS
     ###############################################################
 
     def _getReq(self, path):
         try:
             if self._connfail:
@@ -421,29 +450,29 @@
             if self._connfail:
                 LOG.debug("Connfail: %i", self._connfail)
                 self._connfail -= 1
                 return False
             if type == "PUT":
                 r = requests.put(
                     BASE_URL.format(self._host, path),
-                    data=json.dumps(data),
+                    json=data,
                     timeout=TIMEOUT,
                 )
-            if type == "POST":
+            elif type == "POST":
                 if data is None or data == "":
                     r = requests.post(
                         BASE_URL.format(self._host, path), timeout=TIMEOUT
                     )
                 else:
                     r = requests.post(
                         BASE_URL.format(self._host, path),
-                        data=json.dumps(data),
+                        json=data,
                         timeout=TIMEOUT,
                     )
-            if type == "DELETE":
+            elif type == "DELETE":
                 r = requests.delete(BASE_URL.format(self._host, path), timeout=TIMEOUT)
             if r:
                 LOG.debug("Response: %s", r.content)
                 if r.status_code == 200:
                     return True
             return False
         except requests.exceptions.RequestException as err:
```

### Comparing `pybeoplay-1.0.9/pybeoplay.egg-info/PKG-INFO` & `pybeoplay-1.1.0/pybeoplay.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pybeoplay
-Version: 1.0.9
+Version: 1.1.0
 Summary: BeoPlay API for Python
 Home-page: https://github.com/giachello/pybeoplay
-Download-URL: https://github.com/giachello/pybeoplay/tarball/1.0.9
+Download-URL: https://github.com/giachello/pybeoplay/tarball/1.1.0
 Author: Giovanni Iachello
 Author-email: giovanni.iachello@gmail.com
 License: MIT License
 Keywords: beoplay,pybeoplay,B&O,Bang & Olufsen
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pybeoplay-1.0.9/setup.py` & `pybeoplay-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 PACKAGE_NAME = 'pybeoplay'
 HERE = os.path.abspath(os.path.dirname(__file__))
-VERSION = '1.0.9'
+VERSION = '1.1.0'
 
 PACKAGES = find_packages(exclude=['tests', 'tests.*', 'dist', 'ccu', 'build'])
 
 REQUIRES = []
 
 long_description = readme()
```

