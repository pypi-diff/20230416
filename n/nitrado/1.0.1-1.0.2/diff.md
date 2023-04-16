# Comparing `tmp/nitrado-1.0.1.tar.gz` & `tmp/nitrado-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitrado-1.0.1.tar", last modified: Sun Apr 16 09:35:14 2023, max compression
+gzip compressed data, was "nitrado-1.0.2.tar", last modified: Sun Apr 16 10:27:27 2023, max compression
```

## Comparing `nitrado-1.0.1.tar` & `nitrado-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 09:35:14.264843 nitrado-1.0.1/
--rw-rw-rw-   0        0        0     1093 2023-03-25 00:21:47.000000 nitrado-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     4401 2023-04-16 09:35:14.265847 nitrado-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3600 2023-03-25 00:21:47.000000 nitrado-1.0.1/README.md
--rw-rw-rw-   0        0        0      555 2023-04-16 01:48:34.000000 nitrado-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1135 2023-04-16 09:35:14.266848 nitrado-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-16 09:35:14.231401 nitrado-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-16 09:35:14.240427 nitrado-1.0.1/src/nitrado/
--rw-rw-rw-   0        0        0      236 2023-03-25 08:45:32.000000 nitrado-1.0.1/src/nitrado/__init__.py
--rw-rw-rw-   0        0        0       30 2023-03-25 08:45:32.000000 nitrado-1.0.1/src/nitrado/ark_server.py
-drwxrwxrwx   0        0        0        0 2023-04-16 09:35:14.259326 nitrado-1.0.1/src/nitrado/lib/
--rw-rw-rw-   0        0        0       91 2023-03-25 00:51:09.000000 nitrado-1.0.1/src/nitrado/lib/__init__.py
--rw-rw-rw-   0        0        0     1347 2023-04-16 03:40:10.000000 nitrado-1.0.1/src/nitrado/lib/errors.py
--rw-rw-rw-   0        0        0    21890 2023-04-16 09:32:56.000000 nitrado-1.0.1/src/nitrado/lib/game_server.py
--rw-rw-rw-   0        0        0     3919 2023-04-16 09:31:37.000000 nitrado-1.0.1/src/nitrado/lib/service.py
--rw-rw-rw-   0        0        0     2823 2023-04-16 05:06:33.000000 nitrado-1.0.1/src/nitrado/nitrado_api.py
--rw-rw-rw-   0        0        0        0 2023-03-25 00:21:47.000000 nitrado-1.0.1/src/nitrado/py.typed
-drwxrwxrwx   0        0        0        0 2023-04-16 09:35:14.260325 nitrado-1.0.1/src/nitrado/tools/
--rw-rw-rw-   0        0        0       43 2023-03-25 00:37:24.000000 nitrado-1.0.1/src/nitrado/tools/__init__.py
--rw-rw-rw-   0        0        0     1564 2023-04-16 05:08:15.000000 nitrado-1.0.1/src/nitrado/tools/client.py
-drwxrwxrwx   0        0        0        0 2023-04-16 09:35:14.255327 nitrado-1.0.1/src/nitrado.egg-info/
--rw-rw-rw-   0        0        0     4401 2023-04-16 09:35:14.000000 nitrado-1.0.1/src/nitrado.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      583 2023-04-16 09:35:14.000000 nitrado-1.0.1/src/nitrado.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 09:35:14.000000 nitrado-1.0.1/src/nitrado.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-04-16 09:35:14.000000 nitrado-1.0.1/src/nitrado.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-16 09:35:14.000000 nitrado-1.0.1/src/nitrado.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 09:35:14.264843 nitrado-1.0.1/tests/
--rw-rw-rw-   0        0        0     2251 2023-04-16 05:41:31.000000 nitrado-1.0.1/tests/test_connection.py
--rw-rw-rw-   0        0        0    19592 2023-04-16 09:33:34.000000 nitrado-1.0.1/tests/test_game_server.py
--rw-rw-rw-   0        0        0      106 2023-03-25 08:45:33.000000 nitrado-1.0.1/tests/test_nitrado_api.py
--rw-rw-rw-   0        0        0     2511 2023-03-25 08:45:33.000000 nitrado-1.0.1/tests/test_service.py
+drwxrwxrwx   0        0        0        0 2023-04-16 10:27:27.723296 nitrado-1.0.2/
+-rw-rw-rw-   0        0        0     1093 2023-03-25 00:21:47.000000 nitrado-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     3435 2023-04-16 10:27:27.724299 nitrado-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2634 2023-04-16 09:41:48.000000 nitrado-1.0.2/README.md
+-rw-rw-rw-   0        0        0      555 2023-04-16 01:48:34.000000 nitrado-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1135 2023-04-16 10:27:27.729295 nitrado-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-16 10:27:27.691856 nitrado-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 10:27:27.699283 nitrado-1.0.2/src/nitrado/
+-rw-rw-rw-   0        0        0      236 2023-03-25 08:45:32.000000 nitrado-1.0.2/src/nitrado/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-03-25 08:45:32.000000 nitrado-1.0.2/src/nitrado/ark_server.py
+drwxrwxrwx   0        0        0        0 2023-04-16 10:27:27.717295 nitrado-1.0.2/src/nitrado/lib/
+-rw-rw-rw-   0        0        0       91 2023-03-25 00:51:09.000000 nitrado-1.0.2/src/nitrado/lib/__init__.py
+-rw-rw-rw-   0        0        0     1347 2023-04-16 03:40:10.000000 nitrado-1.0.2/src/nitrado/lib/errors.py
+-rw-rw-rw-   0        0        0    21890 2023-04-16 09:32:56.000000 nitrado-1.0.2/src/nitrado/lib/game_server.py
+-rw-rw-rw-   0        0        0     3887 2023-04-16 10:26:22.000000 nitrado-1.0.2/src/nitrado/lib/service.py
+-rw-rw-rw-   0        0        0     2836 2023-04-16 10:18:35.000000 nitrado-1.0.2/src/nitrado/nitrado_api.py
+-rw-rw-rw-   0        0        0        0 2023-03-25 00:21:47.000000 nitrado-1.0.2/src/nitrado/py.typed
+drwxrwxrwx   0        0        0        0 2023-04-16 10:27:27.719295 nitrado-1.0.2/src/nitrado/tools/
+-rw-rw-rw-   0        0        0       43 2023-03-25 00:37:24.000000 nitrado-1.0.2/src/nitrado/tools/__init__.py
+-rw-rw-rw-   0        0        0     1564 2023-04-16 05:08:15.000000 nitrado-1.0.2/src/nitrado/tools/client.py
+drwxrwxrwx   0        0        0        0 2023-04-16 10:27:27.713300 nitrado-1.0.2/src/nitrado.egg-info/
+-rw-rw-rw-   0        0        0     3435 2023-04-16 10:27:27.000000 nitrado-1.0.2/src/nitrado.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2023-04-16 10:27:27.000000 nitrado-1.0.2/src/nitrado.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 10:27:27.000000 nitrado-1.0.2/src/nitrado.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       93 2023-04-16 10:27:27.000000 nitrado-1.0.2/src/nitrado.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-16 10:27:27.000000 nitrado-1.0.2/src/nitrado.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 10:27:27.722297 nitrado-1.0.2/tests/
+-rw-rw-rw-   0        0        0     2251 2023-04-16 05:41:31.000000 nitrado-1.0.2/tests/test_connection.py
+-rw-rw-rw-   0        0        0    19592 2023-04-16 09:33:34.000000 nitrado-1.0.2/tests/test_game_server.py
+-rw-rw-rw-   0        0        0      106 2023-03-25 08:45:33.000000 nitrado-1.0.2/tests/test_nitrado_api.py
+-rw-rw-rw-   0        0        0     2511 2023-03-25 08:45:33.000000 nitrado-1.0.2/tests/test_service.py
```

### Comparing `nitrado-1.0.1/LICENSE` & `nitrado-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.1/pyproject.toml` & `nitrado-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.1/setup.cfg` & `nitrado-1.0.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6974 7261 646f 0d0a 7665 7273   = nitrado..vers
-00000020: 696f 6e20 3d20 312e 302e 310d 0a74 6573  ion = 1.0.1..tes
+00000020: 696f 6e20 3d20 312e 302e 320d 0a74 6573  ion = 1.0.2..tes
 00000030: 745f 7665 7273 696f 6e20 3d20 312e 302e  t_version = 1.0.
-00000040: 320d 0a70 726f 6475 6374 696f 6e5f 7665  2..production_ve
-00000050: 7273 696f 6e20 3d20 312e 302e 310d 0a61  rsion = 1.0.1..a
+00000040: 330d 0a70 726f 6475 6374 696f 6e5f 7665  3..production_ve
+00000050: 7273 696f 6e20 3d20 312e 302e 320d 0a61  rsion = 1.0.2..a
 00000060: 7574 686f 7220 3d20 4d61 7572 6963 696f  uthor = Mauricio
 00000070: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000080: 2064 6576 2e6d 6175 7269 6369 6f2e 6c6f   dev.mauricio.lo
 00000090: 6d65 6c69 4067 6d61 696c 2e63 6f6d 0d0a  meli@gmail.com..
 000000a0: 6465 7363 7269 7074 696f 6e20 3d20 5468  description = Th
 000000b0: 6973 2061 7070 6c69 6361 7469 6f6e 2061  is application a
 000000c0: 6363 6573 7365 7320 7468 6520 4e69 7472  ccesses the Nitr
```

### Comparing `nitrado-1.0.1/src/nitrado/lib/errors.py` & `nitrado-1.0.2/src/nitrado/lib/errors.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.1/src/nitrado/lib/game_server.py` & `nitrado-1.0.2/src/nitrado/lib/game_server.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.1/src/nitrado/lib/service.py` & `nitrado-1.0.2/src/nitrado/lib/service.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,29 +26,29 @@
         self.delete_date = None
         self.suspending_in = None
         self.deleting_in = None
         for k, v in data.items():
             self.__dict__[k] = v
 
     def log_page(self, page: int) -> dict:
+        assert page > 0, "Page number must be greater than 0"
         path = f'/services/{self.id}/logs'
         response = self.__client.get(path=path, data={'page': page})
         data: dict = response.json()['data']
         return data
 
-    def logs(self, page: int = None) -> dict:
-        if page:
-            return self.log_page(page)['logs']
-        data = self.log_page(1)
-        logs = data['logs']
-        current_page_num = 2
-        while current_page_num <= data['page_count']:
-            data = self.log_page(current_page_num)
-            logs += data['data']['logs']
-            current_page_num += 1
+    def logs(self) -> list:
+        first = self.log_page(1)
+        logs = first['logs']
+        page = 2
+        last_page = first['page_count']
+        while page <= last_page:
+            data = self.log_page(page)
+            logs += data['logs']
+            page += 1
         return logs
 
     def notifications(self) -> list:
         path = f'/services/{self.id}/notifications'
         response = self.__client.get(path=path)
         data: dict = response.json()['data']
         return data['notifications']
@@ -73,15 +73,15 @@
                   'hour': hour, 'day': day, 'month': month, 'weekday': weekday}
         response = self.__client.put(path=path, params=params)
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def delete_task(self, task_id) -> bool:
         path = f'/services/{self.id}/tasks/{task_id}'
-        self.__client.delete(path=path)
+        response = self.__client.delete(path=path)
         data: dict = response.json()
         return response.ok and data['status'] == 'success'
 
     def __contains__(self, item):
         return item in self.__data
 
     def __getitem__(self, item):
```

### Comparing `nitrado-1.0.1/src/nitrado/nitrado_api.py` & `nitrado-1.0.2/src/nitrado/nitrado_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,23 +51,23 @@
         response = self.client.get(path=f'/services/{service_id}/gameservers')
         data: dict = response.json()['data']
         return GameServer(self.client, data['gameserver'])
 
     def find_service_by_id(self, service_id: str) -> Service:
         response = self.client.get(path=f'/services/{service_id}')
         data: dict = response.json()['data']
-        return Service(self.client, data['services'])
+        return Service(self.client, data['service'])
 
-    def health_check(self) -> str:
+    def health_check(self) -> bool:
         response = self.client.get('/ping')
-        data: dict = response.json()['data']
-        return data['message']
+        data: dict = response.json()
+        return response.ok and data['status'] == 'success'
 
-    def maintenance_status(self) -> str:
+    def maintenance_status(self) -> dict:
         response = self.client.get('/maintenance')
         data: dict = response.json()['data']
         return data['maintenance']
 
     def version(self) -> str:
         response = self.client.get('/version')
-        data: dict = response.json()['data']
+        data: dict = response.json()
         return data['message']
```

### Comparing `nitrado-1.0.1/src/nitrado/tools/client.py` & `nitrado-1.0.2/src/nitrado/tools/client.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.1/src/nitrado.egg-info/SOURCES.txt` & `nitrado-1.0.2/src/nitrado.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.1/tests/test_connection.py` & `nitrado-1.0.2/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.1/tests/test_game_server.py` & `nitrado-1.0.2/tests/test_game_server.py`

 * *Files identical despite different names*

### Comparing `nitrado-1.0.1/tests/test_service.py` & `nitrado-1.0.2/tests/test_service.py`

 * *Files identical despite different names*

