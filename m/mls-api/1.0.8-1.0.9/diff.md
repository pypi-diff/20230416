# Comparing `tmp/mls-api-1.0.8.tar.gz` & `tmp/mls-api-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mls-api-1.0.8.tar", last modified: Sun Apr 16 04:59:17 2023, max compression
+gzip compressed data, was "dist/mls-api-1.0.9.tar", last modified: Sun Apr 16 05:18:38 2023, max compression
```

## Comparing `mls-api-1.0.8.tar` & `mls-api-1.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 04:59:17.513277 mls-api-1.0.8/
--rw-r--r--   0 finn       (501) staff       (20)     5422 2023-04-16 04:59:17.513490 mls-api-1.0.8/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     2380 2023-04-16 04:58:30.000000 mls-api-1.0.8/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 04:59:17.509139 mls-api-1.0.8/mls_api/
--rw-r--r--   0 finn       (501) staff       (20)      336 2023-04-16 04:30:39.000000 mls-api-1.0.8/mls_api/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     2395 2023-04-16 04:49:43.000000 mls-api-1.0.8/mls_api/assists.py
--rw-r--r--   0 finn       (501) staff       (20)      381 2023-04-16 03:18:08.000000 mls-api-1.0.8/mls_api/auth.py
--rw-r--r--   0 finn       (501) staff       (20)     1020 2023-04-16 04:50:28.000000 mls-api-1.0.8/mls_api/fixtures.py
--rw-r--r--   0 finn       (501) staff       (20)     1792 2023-04-16 04:49:02.000000 mls-api-1.0.8/mls_api/historical.py
--rw-r--r--   0 finn       (501) staff       (20)      982 2023-04-16 04:51:14.000000 mls-api-1.0.8/mls_api/news.py
--rw-r--r--   0 finn       (501) staff       (20)     2527 2023-04-16 04:52:02.000000 mls-api-1.0.8/mls_api/offense.py
--rw-r--r--   0 finn       (501) staff       (20)     1881 2023-04-16 04:52:39.000000 mls-api-1.0.8/mls_api/players.py
--rw-r--r--   0 finn       (501) staff       (20)     1775 2023-04-16 04:53:09.000000 mls-api-1.0.8/mls_api/rtd.py
--rw-r--r--   0 finn       (501) staff       (20)    34581 2022-08-07 21:22:57.000000 mls-api-1.0.8/mls_api/six.py
--rw-r--r--   0 finn       (501) staff       (20)     1032 2023-04-16 04:53:34.000000 mls-api-1.0.8/mls_api/standings.py
--rw-r--r--   0 finn       (501) staff       (20)      984 2023-04-16 04:54:31.000000 mls-api-1.0.8/mls_api/teams.py
--rw-r--r--   0 finn       (501) staff       (20)     2438 2023-04-16 04:54:28.000000 mls-api-1.0.8/mls_api/top_scorer.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-16 04:58:44.000000 mls-api-1.0.8/mls_api/version.py
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 04:59:17.512818 mls-api-1.0.8/mls_api.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     5422 2023-04-16 04:59:17.000000 mls-api-1.0.8/mls_api.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      472 2023-04-16 04:59:17.000000 mls-api-1.0.8/mls_api.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 04:59:17.000000 mls-api-1.0.8/mls_api.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 04:59:03.000000 mls-api-1.0.8/mls_api.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-16 04:59:17.000000 mls-api-1.0.8/mls_api.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)        8 2023-04-16 04:59:17.000000 mls-api-1.0.8/mls_api.egg-info/top_level.txt
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-16 04:59:17.514315 mls-api-1.0.8/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2476 2023-04-16 04:58:44.000000 mls-api-1.0.8/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 05:18:38.834411 mls-api-1.0.9/
+-rw-r--r--   0 finn       (501) staff       (20)     5430 2023-04-16 05:18:38.834602 mls-api-1.0.9/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     2388 2023-04-16 05:17:06.000000 mls-api-1.0.9/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 05:18:38.831476 mls-api-1.0.9/mls_api/
+-rw-r--r--   0 finn       (501) staff       (20)      336 2023-04-16 04:30:39.000000 mls-api-1.0.9/mls_api/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     2395 2023-04-16 04:49:43.000000 mls-api-1.0.9/mls_api/assists.py
+-rw-r--r--   0 finn       (501) staff       (20)      381 2023-04-16 05:16:48.000000 mls-api-1.0.9/mls_api/auth.py
+-rw-r--r--   0 finn       (501) staff       (20)     1020 2023-04-16 04:50:28.000000 mls-api-1.0.9/mls_api/fixtures.py
+-rw-r--r--   0 finn       (501) staff       (20)     1792 2023-04-16 04:49:02.000000 mls-api-1.0.9/mls_api/historical.py
+-rw-r--r--   0 finn       (501) staff       (20)     1046 2023-04-16 05:17:17.000000 mls-api-1.0.9/mls_api/news.py
+-rw-r--r--   0 finn       (501) staff       (20)     2527 2023-04-16 04:52:02.000000 mls-api-1.0.9/mls_api/offense.py
+-rw-r--r--   0 finn       (501) staff       (20)     1881 2023-04-16 04:52:39.000000 mls-api-1.0.9/mls_api/players.py
+-rw-r--r--   0 finn       (501) staff       (20)     1775 2023-04-16 04:53:09.000000 mls-api-1.0.9/mls_api/rtd.py
+-rw-r--r--   0 finn       (501) staff       (20)    34581 2022-08-07 21:22:57.000000 mls-api-1.0.9/mls_api/six.py
+-rw-r--r--   0 finn       (501) staff       (20)     1032 2023-04-16 04:53:34.000000 mls-api-1.0.9/mls_api/standings.py
+-rw-r--r--   0 finn       (501) staff       (20)      984 2023-04-16 04:54:31.000000 mls-api-1.0.9/mls_api/teams.py
+-rw-r--r--   0 finn       (501) staff       (20)     2438 2023-04-16 04:54:28.000000 mls-api-1.0.9/mls_api/top_scorer.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-16 05:17:55.000000 mls-api-1.0.9/mls_api/version.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 05:18:38.834114 mls-api-1.0.9/mls_api.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     5430 2023-04-16 05:18:38.000000 mls-api-1.0.9/mls_api.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      472 2023-04-16 05:18:38.000000 mls-api-1.0.9/mls_api.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 05:18:38.000000 mls-api-1.0.9/mls_api.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 05:18:18.000000 mls-api-1.0.9/mls_api.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-16 05:18:38.000000 mls-api-1.0.9/mls_api.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)        8 2023-04-16 05:18:38.000000 mls-api-1.0.9/mls_api.egg-info/top_level.txt
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-16 05:18:38.835199 mls-api-1.0.9/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2476 2023-04-16 05:17:55.000000 mls-api-1.0.9/setup.py
```

### Comparing `mls-api-1.0.8/PKG-INFO` & `mls-api-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mls-api
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python library for integrating with the MLS (Major League Soccer) API.
 Home-page: https://moatsystems.com/mls-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/moatsystems/mlsapi-python/issues
 Project-URL: Changes, https://github.com/moatsystems/mlsapi-python/blob/main/CHANGELOG.md
@@ -51,15 +51,15 @@
         
             import os, json
             import mls_api
         
             # Authentication
             username = "your_username"
             password = "your_password"
-            response_text = login(username, password)
+            response_text = mls_api.login(username, password)
             print("Login response:", response_text)
         
             # Get all historical data
             response_text = mls_api.get_all_hist()
             print("All historical data response:", response_text)
         
             # Get all real-time data (RTD)
```

### Comparing `mls-api-1.0.8/README.md` & `mls-api-1.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ```python
 import os, json
 import mls_api
 
 # Authentication
 username = "your_username"
 password = "your_password"
-response_text = login(username, password)
+response_text = mls_api.login(username, password)
 print("Login response:", response_text)
 
 # Get all historical data
 response_text = mls_api.get_all_hist()
 print("All historical data response:", response_text)
 
 # Get all real-time data (RTD)
```

### Comparing `mls-api-1.0.8/mls_api/assists.py` & `mls-api-1.0.9/mls_api/assists.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.8/mls_api/fixtures.py` & `mls-api-1.0.9/mls_api/fixtures.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.8/mls_api/historical.py` & `mls-api-1.0.9/mls_api/historical.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.8/mls_api/news.py` & `mls-api-1.0.9/mls_api/standings.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import os, json
 import requests
 
-BASE_URL = "https://mlssoccerapi.com/news"
+BASE_URL = "https://mlssoccerapi.com/standings"
 
 bearerToken = os.getenv('BEARER_TOKEN')
 
 headers = {
     'Content-Type': 'application/json',
     'Authorization': f'Bearer {bearerToken}'
 }
 
-def get_all_news():
+def get_all_standings():
     response = requests.get(BASE_URL, headers=headers)
     return response.text
 
-def get_news_by_id(news_id):
-    url = f"{BASE_URL}/{news_id}"
+def get_standing_by_id(standing_id):
+    url = f"{BASE_URL}/{standing_id}"
     response = requests.get(url, headers=headers)
     return response.text
 
-def update_news_by_id(news_id, data):
-    url = f"{BASE_URL}/{news_id}"
+def update_standing_by_id(standing_id, data):
+    url = f"{BASE_URL}/{standing_id}"
     payload = json.dumps(data)
     response = requests.put(url, headers=headers, data=payload)
     return response.text
 
-def delete_news_by_id(news_id):
-    url = f"{BASE_URL}/{news_id}"
+def delete_standing_by_id(standing_id):
+    url = f"{BASE_URL}/{standing_id}"
     response = requests.delete(url, headers=headers)
     return response.text
 
-def add_new_news(data):
+def add_new_standing(data):
     payload = json.dumps(data)
     response = requests.post(BASE_URL, headers=headers, data=payload)
     return response.text
```

### Comparing `mls-api-1.0.8/mls_api/offense.py` & `mls-api-1.0.9/mls_api/offense.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.8/mls_api/players.py` & `mls-api-1.0.9/mls_api/players.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.8/mls_api/rtd.py` & `mls-api-1.0.9/mls_api/rtd.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.8/mls_api/six.py` & `mls-api-1.0.9/mls_api/six.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.8/mls_api/standings.py` & `mls-api-1.0.9/mls_api/teams.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import os, json
 import requests
 
-BASE_URL = "https://mlssoccerapi.com/standings"
+BASE_URL = "https://mlssoccerapi.com/teams"
 
 bearerToken = os.getenv('BEARER_TOKEN')
 
 headers = {
     'Content-Type': 'application/json',
     'Authorization': f'Bearer {bearerToken}'
 }
 
-def get_all_standings():
+def get_all_teams():
     response = requests.get(BASE_URL, headers=headers)
     return response.text
 
-def get_standing_by_id(standing_id):
-    url = f"{BASE_URL}/{standing_id}"
+def get_team_by_id(team_id):
+    url = f"{BASE_URL}/{team_id}"
     response = requests.get(url, headers=headers)
     return response.text
 
-def update_standing_by_id(standing_id, data):
-    url = f"{BASE_URL}/{standing_id}"
+def update_team_by_id(team_id, data):
+    url = f"{BASE_URL}/{team_id}"
     payload = json.dumps(data)
     response = requests.put(url, headers=headers, data=payload)
     return response.text
 
-def delete_standing_by_id(standing_id):
-    url = f"{BASE_URL}/{standing_id}"
+def delete_team_by_id(team_id):
+    url = f"{BASE_URL}/{team_id}"
     response = requests.delete(url, headers=headers)
     return response.text
 
-def add_new_standing(data):
+def add_new_team(data):
     payload = json.dumps(data)
     response = requests.post(BASE_URL, headers=headers, data=payload)
     return response.text
```

### Comparing `mls-api-1.0.8/mls_api/teams.py` & `mls-api-1.0.9/mls_api/news.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,33 @@
-import os, json
+import json
 import requests
 
-BASE_URL = "https://mlssoccerapi.com/teams"
-
-bearerToken = os.getenv('BEARER_TOKEN')
+BASE_URL = "https://mlssoccerapi.com/news"
 
 headers = {
-    'Content-Type': 'application/json',
-    'Authorization': f'Bearer {bearerToken}'
+    'Content-Type': 'application/json'
 }
 
-def get_all_teams():
-    response = requests.get(BASE_URL, headers=headers)
+def get_all_news(auth_header):
+    response = requests.get(BASE_URL, headers={**headers, **auth_header})
     return response.text
 
-def get_team_by_id(team_id):
-    url = f"{BASE_URL}/{team_id}"
-    response = requests.get(url, headers=headers)
+def get_news_by_id(news_id, auth_header):
+    url = f"{BASE_URL}/{news_id}"
+    response = requests.get(url, headers={**headers, **auth_header})
     return response.text
 
-def update_team_by_id(team_id, data):
-    url = f"{BASE_URL}/{team_id}"
+def update_news_by_id(news_id, data, auth_header):
+    url = f"{BASE_URL}/{news_id}"
     payload = json.dumps(data)
-    response = requests.put(url, headers=headers, data=payload)
+    response = requests.put(url, headers={**headers, **auth_header}, data=payload)
     return response.text
 
-def delete_team_by_id(team_id):
-    url = f"{BASE_URL}/{team_id}"
-    response = requests.delete(url, headers=headers)
+def delete_news_by_id(news_id, auth_header):
+    url = f"{BASE_URL}/{news_id}"
+    response = requests.delete(url, headers={**headers, **auth_header})
     return response.text
 
-def add_new_team(data):
+def add_new_news(data, auth_header):
     payload = json.dumps(data)
-    response = requests.post(BASE_URL, headers=headers, data=payload)
+    response = requests.post(BASE_URL, headers={**headers, **auth_header}, data=payload)
     return response.text
```

### Comparing `mls-api-1.0.8/mls_api/top_scorer.py` & `mls-api-1.0.9/mls_api/top_scorer.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.8/mls_api.egg-info/PKG-INFO` & `mls-api-1.0.9/mls_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mls-api
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python library for integrating with the MLS (Major League Soccer) API.
 Home-page: https://moatsystems.com/mls-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/moatsystems/mlsapi-python/issues
 Project-URL: Changes, https://github.com/moatsystems/mlsapi-python/blob/main/CHANGELOG.md
@@ -51,15 +51,15 @@
         
             import os, json
             import mls_api
         
             # Authentication
             username = "your_username"
             password = "your_password"
-            response_text = login(username, password)
+            response_text = mls_api.login(username, password)
             print("Login response:", response_text)
         
             # Get all historical data
             response_text = mls_api.get_all_hist()
             print("All historical data response:", response_text)
         
             # Get all real-time data (RTD)
```

### Comparing `mls-api-1.0.8/setup.py` & `mls-api-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "mls-api"
-VERSION = "1.0.8"
+VERSION = "1.0.9"
 REQUIRES = ["requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

