# Comparing `tmp/mls-api-1.2.0.tar.gz` & `tmp/mls-api-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mls-api-1.2.0.tar", last modified: Sun Apr 16 16:30:07 2023, max compression
+gzip compressed data, was "dist/mls-api-1.3.0.tar", last modified: Sun Apr 16 16:45:28 2023, max compression
```

## Comparing `mls-api-1.2.0.tar` & `mls-api-1.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 16:30:07.209050 mls-api-1.2.0/
--rw-r--r--   0 finn       (501) staff       (20)     5304 2023-04-16 16:30:07.209265 mls-api-1.2.0/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     2258 2023-04-16 06:16:08.000000 mls-api-1.2.0/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 16:30:07.205759 mls-api-1.2.0/mls_api/
--rw-r--r--   0 finn       (501) staff       (20)      343 2023-04-16 16:27:54.000000 mls-api-1.2.0/mls_api/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     1492 2023-04-16 06:08:58.000000 mls-api-1.2.0/mls_api/assists.py
--rw-r--r--   0 finn       (501) staff       (20)      655 2023-04-16 16:27:55.000000 mls-api-1.2.0/mls_api/auth.py
--rw-r--r--   0 finn       (501) staff       (20)     1500 2023-04-16 06:09:04.000000 mls-api-1.2.0/mls_api/fixtures.py
--rw-r--r--   0 finn       (501) staff       (20)     1510 2023-04-16 06:09:06.000000 mls-api-1.2.0/mls_api/historical.py
--rw-r--r--   0 finn       (501) staff       (20)     1298 2023-04-16 16:27:52.000000 mls-api-1.2.0/mls_api/latest_news.py
--rw-r--r--   0 finn       (501) staff       (20)     1492 2023-04-16 06:09:17.000000 mls-api-1.2.0/mls_api/offense.py
--rw-r--r--   0 finn       (501) staff       (20)     1716 2023-04-16 06:12:07.000000 mls-api-1.2.0/mls_api/players.py
--rw-r--r--   0 finn       (501) staff       (20)     1458 2023-04-16 06:09:21.000000 mls-api-1.2.0/mls_api/rtd.py
--rw-r--r--   0 finn       (501) staff       (20)    34581 2023-04-16 06:09:23.000000 mls-api-1.2.0/mls_api/six.py
--rw-r--r--   0 finn       (501) staff       (20)     1508 2023-04-16 06:09:26.000000 mls-api-1.2.0/mls_api/standings.py
--rw-r--r--   0 finn       (501) staff       (20)     1476 2023-04-16 06:09:28.000000 mls-api-1.2.0/mls_api/teams.py
--rw-r--r--   0 finn       (501) staff       (20)     1512 2023-04-16 06:09:30.000000 mls-api-1.2.0/mls_api/top_scorer.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-16 16:29:51.000000 mls-api-1.2.0/mls_api/version.py
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 16:30:07.208513 mls-api-1.2.0/mls_api.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     5304 2023-04-16 16:30:07.000000 mls-api-1.2.0/mls_api.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      479 2023-04-16 16:30:07.000000 mls-api-1.2.0/mls_api.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 16:30:07.000000 mls-api-1.2.0/mls_api.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 16:29:03.000000 mls-api-1.2.0/mls_api.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-16 16:30:07.000000 mls-api-1.2.0/mls_api.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)        8 2023-04-16 16:30:07.000000 mls-api-1.2.0/mls_api.egg-info/top_level.txt
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-16 16:30:07.209856 mls-api-1.2.0/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2476 2023-04-16 16:29:51.000000 mls-api-1.2.0/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 16:45:28.932271 mls-api-1.3.0/
+-rw-r--r--   0 finn       (501) staff       (20)     5304 2023-04-16 16:45:28.932489 mls-api-1.3.0/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     2258 2023-04-16 06:16:08.000000 mls-api-1.3.0/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 16:45:28.927440 mls-api-1.3.0/mls_api/
+-rw-r--r--   0 finn       (501) staff       (20)      343 2023-04-16 16:43:33.000000 mls-api-1.3.0/mls_api/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     1492 2023-04-16 06:08:58.000000 mls-api-1.3.0/mls_api/assists.py
+-rw-r--r--   0 finn       (501) staff       (20)      655 2023-04-16 16:44:55.000000 mls-api-1.3.0/mls_api/auth.py
+-rw-r--r--   0 finn       (501) staff       (20)     1500 2023-04-16 06:09:04.000000 mls-api-1.3.0/mls_api/fixtures.py
+-rw-r--r--   0 finn       (501) staff       (20)     1510 2023-04-16 06:09:06.000000 mls-api-1.3.0/mls_api/historical.py
+-rw-r--r--   0 finn       (501) staff       (20)     1496 2023-04-16 16:43:31.000000 mls-api-1.3.0/mls_api/latest_news.py
+-rw-r--r--   0 finn       (501) staff       (20)     1492 2023-04-16 06:09:17.000000 mls-api-1.3.0/mls_api/offense.py
+-rw-r--r--   0 finn       (501) staff       (20)     1716 2023-04-16 06:12:07.000000 mls-api-1.3.0/mls_api/players.py
+-rw-r--r--   0 finn       (501) staff       (20)     1458 2023-04-16 06:09:21.000000 mls-api-1.3.0/mls_api/rtd.py
+-rw-r--r--   0 finn       (501) staff       (20)    34581 2023-04-16 06:09:23.000000 mls-api-1.3.0/mls_api/six.py
+-rw-r--r--   0 finn       (501) staff       (20)     1508 2023-04-16 06:09:26.000000 mls-api-1.3.0/mls_api/standings.py
+-rw-r--r--   0 finn       (501) staff       (20)     1476 2023-04-16 06:09:28.000000 mls-api-1.3.0/mls_api/teams.py
+-rw-r--r--   0 finn       (501) staff       (20)     1512 2023-04-16 06:09:30.000000 mls-api-1.3.0/mls_api/top_scorer.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-16 16:45:12.000000 mls-api-1.3.0/mls_api/version.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 16:45:28.931856 mls-api-1.3.0/mls_api.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     5304 2023-04-16 16:45:28.000000 mls-api-1.3.0/mls_api.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      479 2023-04-16 16:45:28.000000 mls-api-1.3.0/mls_api.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 16:45:28.000000 mls-api-1.3.0/mls_api.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 16:29:03.000000 mls-api-1.3.0/mls_api.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-16 16:45:28.000000 mls-api-1.3.0/mls_api.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)        8 2023-04-16 16:45:28.000000 mls-api-1.3.0/mls_api.egg-info/top_level.txt
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-16 16:45:28.933262 mls-api-1.3.0/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2476 2023-04-16 16:45:12.000000 mls-api-1.3.0/setup.py
```

### Comparing `mls-api-1.2.0/PKG-INFO` & `mls-api-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mls-api
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python library for integrating with the MLS (Major League Soccer) API.
 Home-page: https://moatsystems.com/mls-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/moatsystems/mlsapi-python/issues
 Project-URL: Changes, https://github.com/moatsystems/mlsapi-python/blob/main/CHANGELOG.md
```

### Comparing `mls-api-1.2.0/README.md` & `mls-api-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mls-api-1.2.0/mls_api/assists.py` & `mls-api-1.3.0/mls_api/assists.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.2.0/mls_api/auth.py` & `mls-api-1.3.0/mls_api/auth.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.2.0/mls_api/fixtures.py` & `mls-api-1.3.0/mls_api/fixtures.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.2.0/mls_api/historical.py` & `mls-api-1.3.0/mls_api/historical.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.2.0/mls_api/latest_news.py` & `mls-api-1.3.0/mls_api/teams.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,48 @@
 import requests
 import json
+import os
 
-def get_latest_news(bearer_token, id=None):
-    url = 'https://mlssoccerapi.com/news/'
+def get_teams(id=None):
+    bearerToken = os.getenv('BEARER_TOKEN')
+    url = 'https://mlssoccerapi.com/teams/'
     headers = {
         'Content-Type': 'application/json', 
-        'Authorization': f'Bearer {bearer_token}'
+        'Authorization': f'Bearer {bearerToken}'
     }
     if id != None: 
         url += id
     response = requests.get(url=url, headers=headers)
     return response.json()
 
-def update_latest_news(bearer_token, id, payload):
-    url = f'https://mlssoccerapi.com/news/{id}'
+def update_teams(id, payload):
+    bearerToken = os.getenv('BEARER_TOKEN') 
+    url = f'https://mlssoccerapi.com/teams/{id}'
     headers = {
         'Content-Type': 'application/json', 
-        'Authorization': f'Bearer {bearer_token}'
+        'Authorization': f'Bearer {bearerToken}'
     }
-    response = requests.put(url=url, headers=headers, json=payload)
+    response = requests.put(url=url, headers=headers, data=payload)
     return response.json()
 
-def delete_latest_news(bearer_token, id): 
-    url = f'https://mlssoccerapi.com/news/{id}'
+def delete_teams(id): 
+    bearerToken = os.getenv('BEARER_TOKEN')
+    url = f'https://mlssoccerapi.com/teams/{id}'
     headers = {
         'Content-Type': 'application/json', 
-        'Authorization': f'Bearer {bearer_token}'
+        'Authorization': f'Bearer {bearerToken}'
     }
-    response = requests.delete(url=url, headers=headers)
+    payload = json.dumps({
+        'id': id
+    })
+    response = requests.delete(url=url, headers=headers, data=payload)
     return response.json()
 
-def add_latest_news(bearer_token, payload):
-    url = 'https://mlssoccerapi.com/news/'
+def add_teams(payload):
+    bearerToken = os.getenv('BEARER_TOKEN')
+    url = 'https://mlssoccerapi.com/teams/'
     headers = {
         'Content-Type': 'application/json', 
-        'Authorization': f'Bearer {bearer_token}'
+        'Authorization': f'Bearer {bearerToken}'
     }
-    response = requests.post(url=url, headers=headers, json=payload)
-    return response.json()
+    response = requests.post(url=url, headers=headers, data=payload)
+    return response.json()
```

### Comparing `mls-api-1.2.0/mls_api/offense.py` & `mls-api-1.3.0/mls_api/offense.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.2.0/mls_api/players.py` & `mls-api-1.3.0/mls_api/players.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.2.0/mls_api/rtd.py` & `mls-api-1.3.0/mls_api/rtd.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.2.0/mls_api/six.py` & `mls-api-1.3.0/mls_api/six.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.2.0/mls_api/standings.py` & `mls-api-1.3.0/mls_api/standings.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.2.0/mls_api/teams.py` & `mls-api-1.3.0/mls_api/latest_news.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 import requests
 import json
 import os
 
-def get_teams(id=None):
+def get_latest_news(id=None):
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = 'https://mlssoccerapi.com/teams/'
+    url = 'https://mlssoccerapi.com/news/'
     headers = {
         'Content-Type': 'application/json', 
         'Authorization': f'Bearer {bearerToken}'
     }
     if id != None: 
         url += id
     response = requests.get(url=url, headers=headers)
     return response.json()
 
-def update_teams(id, payload):
+def update_latest_news(id, payload):
     bearerToken = os.getenv('BEARER_TOKEN') 
-    url = f'https://mlssoccerapi.com/teams/{id}'
+    url = f'https://mlssoccerapi.com/news/{id}'
     headers = {
         'Content-Type': 'application/json', 
         'Authorization': f'Bearer {bearerToken}'
     }
     response = requests.put(url=url, headers=headers, data=payload)
     return response.json()
 
-def delete_teams(id): 
+def delete_latest_news(id): 
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = f'https://mlssoccerapi.com/teams/{id}'
+    url = f'https://mlssoccerapi.com/news/{id}'
     headers = {
         'Content-Type': 'application/json', 
         'Authorization': f'Bearer {bearerToken}'
     }
     payload = json.dumps({
         'id': id
     })
     response = requests.delete(url=url, headers=headers, data=payload)
     return response.json()
 
-def add_teams(payload):
+def add_latest_news(payload):
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = 'https://mlssoccerapi.com/teams/'
+    url = 'https://mlssoccerapi.com/news/'
     headers = {
         'Content-Type': 'application/json', 
         'Authorization': f'Bearer {bearerToken}'
     }
     response = requests.post(url=url, headers=headers, data=payload)
     return response.json()
```

### Comparing `mls-api-1.2.0/mls_api/top_scorer.py` & `mls-api-1.3.0/mls_api/top_scorer.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.2.0/mls_api.egg-info/PKG-INFO` & `mls-api-1.3.0/mls_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mls-api
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python library for integrating with the MLS (Major League Soccer) API.
 Home-page: https://moatsystems.com/mls-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/moatsystems/mlsapi-python/issues
 Project-URL: Changes, https://github.com/moatsystems/mlsapi-python/blob/main/CHANGELOG.md
```

### Comparing `mls-api-1.2.0/setup.py` & `mls-api-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "mls-api"
-VERSION = "1.2.0"
+VERSION = "1.3.0"
 REQUIRES = ["requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

