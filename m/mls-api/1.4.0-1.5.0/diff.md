# Comparing `tmp/mls-api-1.4.0.tar.gz` & `tmp/mls-api-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mls-api-1.4.0.tar", last modified: Sun Apr 16 16:59:01 2023, max compression
+gzip compressed data, was "dist/mls-api-1.5.0.tar", last modified: Sun Apr 16 17:09:40 2023, max compression
```

## Comparing `mls-api-1.4.0.tar` & `mls-api-1.5.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 16:59:01.003046 mls-api-1.4.0/
--rw-r--r--   0 finn       (501) staff       (20)     5304 2023-04-16 16:59:01.003295 mls-api-1.4.0/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     2258 2023-04-16 06:16:08.000000 mls-api-1.4.0/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 16:59:00.998145 mls-api-1.4.0/mls_api/
--rw-r--r--   0 finn       (501) staff       (20)      343 2023-04-16 16:43:33.000000 mls-api-1.4.0/mls_api/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     1492 2023-04-16 16:55:53.000000 mls-api-1.4.0/mls_api/assists.py
--rw-r--r--   0 finn       (501) staff       (20)      655 2023-04-16 16:56:36.000000 mls-api-1.4.0/mls_api/auth.py
--rw-r--r--   0 finn       (501) staff       (20)     1500 2023-04-16 16:56:03.000000 mls-api-1.4.0/mls_api/fixtures.py
--rw-r--r--   0 finn       (501) staff       (20)     1510 2023-04-16 16:56:14.000000 mls-api-1.4.0/mls_api/historical.py
--rw-r--r--   0 finn       (501) staff       (20)     1496 2023-04-16 16:56:25.000000 mls-api-1.4.0/mls_api/latest_news.py
--rw-r--r--   0 finn       (501) staff       (20)     1492 2023-04-16 16:56:48.000000 mls-api-1.4.0/mls_api/offense.py
--rw-r--r--   0 finn       (501) staff       (20)     1492 2023-04-16 16:57:01.000000 mls-api-1.4.0/mls_api/players.py
--rw-r--r--   0 finn       (501) staff       (20)     1458 2023-04-16 16:57:12.000000 mls-api-1.4.0/mls_api/rtd.py
--rw-r--r--   0 finn       (501) staff       (20)    34581 2023-04-16 06:09:23.000000 mls-api-1.4.0/mls_api/six.py
--rw-r--r--   0 finn       (501) staff       (20)     1508 2023-04-16 16:57:23.000000 mls-api-1.4.0/mls_api/standings.py
--rw-r--r--   0 finn       (501) staff       (20)     1476 2023-04-16 16:57:34.000000 mls-api-1.4.0/mls_api/teams.py
--rw-r--r--   0 finn       (501) staff       (20)     1512 2023-04-16 16:57:46.000000 mls-api-1.4.0/mls_api/top_scorer.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-16 16:58:20.000000 mls-api-1.4.0/mls_api/version.py
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 16:59:01.002505 mls-api-1.4.0/mls_api.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     5304 2023-04-16 16:59:00.000000 mls-api-1.4.0/mls_api.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      479 2023-04-16 16:59:00.000000 mls-api-1.4.0/mls_api.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 16:59:00.000000 mls-api-1.4.0/mls_api.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 16:58:40.000000 mls-api-1.4.0/mls_api.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-16 16:59:00.000000 mls-api-1.4.0/mls_api.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)        8 2023-04-16 16:59:00.000000 mls-api-1.4.0/mls_api.egg-info/top_level.txt
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-16 16:59:01.004117 mls-api-1.4.0/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2476 2023-04-16 16:58:20.000000 mls-api-1.4.0/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 17:09:40.149324 mls-api-1.5.0/
+-rw-r--r--   0 finn       (501) staff       (20)     5304 2023-04-16 17:09:40.149554 mls-api-1.5.0/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     2258 2023-04-16 06:16:08.000000 mls-api-1.5.0/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 17:09:40.145877 mls-api-1.5.0/mls_api/
+-rw-r--r--   0 finn       (501) staff       (20)      343 2023-04-16 16:43:33.000000 mls-api-1.5.0/mls_api/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     1492 2023-04-16 16:55:53.000000 mls-api-1.5.0/mls_api/assists.py
+-rw-r--r--   0 finn       (501) staff       (20)      655 2023-04-16 16:56:36.000000 mls-api-1.5.0/mls_api/auth.py
+-rw-r--r--   0 finn       (501) staff       (20)     1500 2023-04-16 16:56:03.000000 mls-api-1.5.0/mls_api/fixtures.py
+-rw-r--r--   0 finn       (501) staff       (20)     1510 2023-04-16 16:56:14.000000 mls-api-1.5.0/mls_api/historical.py
+-rw-r--r--   0 finn       (501) staff       (20)     1496 2023-04-16 16:56:25.000000 mls-api-1.5.0/mls_api/latest_news.py
+-rw-r--r--   0 finn       (501) staff       (20)     1492 2023-04-16 16:56:48.000000 mls-api-1.5.0/mls_api/offense.py
+-rw-r--r--   0 finn       (501) staff       (20)     1691 2023-04-16 17:08:48.000000 mls-api-1.5.0/mls_api/players.py
+-rw-r--r--   0 finn       (501) staff       (20)     1458 2023-04-16 16:57:12.000000 mls-api-1.5.0/mls_api/rtd.py
+-rw-r--r--   0 finn       (501) staff       (20)    34581 2023-04-16 06:09:23.000000 mls-api-1.5.0/mls_api/six.py
+-rw-r--r--   0 finn       (501) staff       (20)     1508 2023-04-16 16:57:23.000000 mls-api-1.5.0/mls_api/standings.py
+-rw-r--r--   0 finn       (501) staff       (20)     1476 2023-04-16 16:57:34.000000 mls-api-1.5.0/mls_api/teams.py
+-rw-r--r--   0 finn       (501) staff       (20)     1512 2023-04-16 16:57:46.000000 mls-api-1.5.0/mls_api/top_scorer.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-16 17:09:02.000000 mls-api-1.5.0/mls_api/version.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 17:09:40.148885 mls-api-1.5.0/mls_api.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     5304 2023-04-16 17:09:40.000000 mls-api-1.5.0/mls_api.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      479 2023-04-16 17:09:40.000000 mls-api-1.5.0/mls_api.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 17:09:40.000000 mls-api-1.5.0/mls_api.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 17:09:20.000000 mls-api-1.5.0/mls_api.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-16 17:09:40.000000 mls-api-1.5.0/mls_api.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)        8 2023-04-16 17:09:40.000000 mls-api-1.5.0/mls_api.egg-info/top_level.txt
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-16 17:09:40.150051 mls-api-1.5.0/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2476 2023-04-16 17:09:02.000000 mls-api-1.5.0/setup.py
```

### Comparing `mls-api-1.4.0/PKG-INFO` & `mls-api-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mls-api
-Version: 1.4.0
+Version: 1.5.0
 Summary: Python library for integrating with the MLS (Major League Soccer) API.
 Home-page: https://moatsystems.com/mls-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/moatsystems/mlsapi-python/issues
 Project-URL: Changes, https://github.com/moatsystems/mlsapi-python/blob/main/CHANGELOG.md
```

### Comparing `mls-api-1.4.0/README.md` & `mls-api-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mls-api-1.4.0/mls_api/assists.py` & `mls-api-1.5.0/mls_api/assists.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.4.0/mls_api/auth.py` & `mls-api-1.5.0/mls_api/auth.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.4.0/mls_api/fixtures.py` & `mls-api-1.5.0/mls_api/fixtures.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.4.0/mls_api/historical.py` & `mls-api-1.5.0/mls_api/historical.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.4.0/mls_api/latest_news.py` & `mls-api-1.5.0/mls_api/latest_news.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.4.0/mls_api/offense.py` & `mls-api-1.5.0/mls_api/offense.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.4.0/mls_api/players.py` & `mls-api-1.5.0/mls_api/top_scorer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import requests
 import json
 import os
 
-def get_players(id=None):
+def get_top_scorer(id=None):
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = 'https://mlssoccerapi.com/players/'
+    url = 'https://mlssoccerapi.com/topscorer/'
     headers = {
         'Content-Type': 'application/json', 
         'Authorization': f'Bearer {bearerToken}'
     }
     if id != None: 
         url += id
     response = requests.get(url=url, headers=headers)
     return response.json()
 
-def update_players(id, payload):
+def update_top_scorer(id, payload):
     bearerToken = os.getenv('BEARER_TOKEN') 
-    url = f'https://mlssoccerapi.com/players/{id}'
+    url = f'https://mlssoccerapi.com/topscorer/{id}'
     headers = {
         'Content-Type': 'application/json', 
         'Authorization': f'Bearer {bearerToken}'
     }
     response = requests.put(url=url, headers=headers, data=payload)
     return response.json()
 
-def delete_players(id): 
+def delete_top_scorer(id): 
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = f'https://mlssoccerapi.com/players/{id}'
+    url = f'https://mlssoccerapi.com/topscorer/{id}'
     headers = {
         'Content-Type': 'application/json', 
         'Authorization': f'Bearer {bearerToken}'
     }
     payload = json.dumps({
         'id': id
     })
     response = requests.delete(url=url, headers=headers, data=payload)
     return response.json()
 
-def add_players(payload):
+def add_top_scorer(payload):
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = 'https://mlssoccerapi.com/players/'
+    url = 'https://mlssoccerapi.com/topscorer/'
     headers = {
         'Content-Type': 'application/json', 
         'Authorization': f'Bearer {bearerToken}'
     }
     response = requests.post(url=url, headers=headers, data=payload)
     return response.json()
```

### Comparing `mls-api-1.4.0/mls_api/rtd.py` & `mls-api-1.5.0/mls_api/rtd.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.4.0/mls_api/six.py` & `mls-api-1.5.0/mls_api/six.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.4.0/mls_api/standings.py` & `mls-api-1.5.0/mls_api/standings.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.4.0/mls_api/teams.py` & `mls-api-1.5.0/mls_api/teams.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.4.0/mls_api/top_scorer.py` & `mls-api-1.5.0/mls_api/players.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,55 @@
 import requests
 import json
 import os
 
-def get_top_scorer(id=None):
+def get_players(id=None, offset=None, limit=None):
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = 'https://mlssoccerapi.com/topscorer/'
+    url = 'https://mlssoccerapi.com/players/'
     headers = {
-        'Content-Type': 'application/json', 
+        'Content-Type': 'application/json',
         'Authorization': f'Bearer {bearerToken}'
     }
-    if id != None: 
-        url += id
-    response = requests.get(url=url, headers=headers)
+    
+    params = {}
+    if offset is not None:
+        params['offset'] = offset
+    if limit is not None:
+        params['limit'] = limit
+    if id is not None:
+        url += str(id)
+    
+    response = requests.get(url=url, headers=headers, params=params)
     return response.json()
 
-def update_top_scorer(id, payload):
+def update_players(id, payload):
     bearerToken = os.getenv('BEARER_TOKEN') 
-    url = f'https://mlssoccerapi.com/topscorer/{id}'
+    url = f'https://mlssoccerapi.com/players/{id}'
     headers = {
         'Content-Type': 'application/json', 
         'Authorization': f'Bearer {bearerToken}'
     }
     response = requests.put(url=url, headers=headers, data=payload)
     return response.json()
 
-def delete_top_scorer(id): 
+def delete_players(id): 
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = f'https://mlssoccerapi.com/topscorer/{id}'
+    url = f'https://mlssoccerapi.com/players/{id}'
     headers = {
         'Content-Type': 'application/json', 
         'Authorization': f'Bearer {bearerToken}'
     }
     payload = json.dumps({
         'id': id
     })
     response = requests.delete(url=url, headers=headers, data=payload)
     return response.json()
 
-def add_top_scorer(payload):
+def add_players(payload):
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = 'https://mlssoccerapi.com/topscorer/'
+    url = 'https://mlssoccerapi.com/players/'
     headers = {
         'Content-Type': 'application/json', 
         'Authorization': f'Bearer {bearerToken}'
     }
     response = requests.post(url=url, headers=headers, data=payload)
     return response.json()
```

### Comparing `mls-api-1.4.0/mls_api.egg-info/PKG-INFO` & `mls-api-1.5.0/mls_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mls-api
-Version: 1.4.0
+Version: 1.5.0
 Summary: Python library for integrating with the MLS (Major League Soccer) API.
 Home-page: https://moatsystems.com/mls-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/moatsystems/mlsapi-python/issues
 Project-URL: Changes, https://github.com/moatsystems/mlsapi-python/blob/main/CHANGELOG.md
```

### Comparing `mls-api-1.4.0/setup.py` & `mls-api-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "mls-api"
-VERSION = "1.4.0"
+VERSION = "1.5.0"
 REQUIRES = ["requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

