# Comparing `tmp/mls-api-1.0.9.tar.gz` & `tmp/mls-api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mls-api-1.0.9.tar", last modified: Sun Apr 16 05:18:38 2023, max compression
+gzip compressed data, was "dist/mls-api-1.1.0.tar", last modified: Sun Apr 16 16:29:21 2023, max compression
```

## Comparing `mls-api-1.0.9.tar` & `mls-api-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 05:18:38.834411 mls-api-1.0.9/
--rw-r--r--   0 finn       (501) staff       (20)     5430 2023-04-16 05:18:38.834602 mls-api-1.0.9/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     2388 2023-04-16 05:17:06.000000 mls-api-1.0.9/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 05:18:38.831476 mls-api-1.0.9/mls_api/
--rw-r--r--   0 finn       (501) staff       (20)      336 2023-04-16 04:30:39.000000 mls-api-1.0.9/mls_api/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     2395 2023-04-16 04:49:43.000000 mls-api-1.0.9/mls_api/assists.py
--rw-r--r--   0 finn       (501) staff       (20)      381 2023-04-16 05:16:48.000000 mls-api-1.0.9/mls_api/auth.py
--rw-r--r--   0 finn       (501) staff       (20)     1020 2023-04-16 04:50:28.000000 mls-api-1.0.9/mls_api/fixtures.py
--rw-r--r--   0 finn       (501) staff       (20)     1792 2023-04-16 04:49:02.000000 mls-api-1.0.9/mls_api/historical.py
--rw-r--r--   0 finn       (501) staff       (20)     1046 2023-04-16 05:17:17.000000 mls-api-1.0.9/mls_api/news.py
--rw-r--r--   0 finn       (501) staff       (20)     2527 2023-04-16 04:52:02.000000 mls-api-1.0.9/mls_api/offense.py
--rw-r--r--   0 finn       (501) staff       (20)     1881 2023-04-16 04:52:39.000000 mls-api-1.0.9/mls_api/players.py
--rw-r--r--   0 finn       (501) staff       (20)     1775 2023-04-16 04:53:09.000000 mls-api-1.0.9/mls_api/rtd.py
--rw-r--r--   0 finn       (501) staff       (20)    34581 2022-08-07 21:22:57.000000 mls-api-1.0.9/mls_api/six.py
--rw-r--r--   0 finn       (501) staff       (20)     1032 2023-04-16 04:53:34.000000 mls-api-1.0.9/mls_api/standings.py
--rw-r--r--   0 finn       (501) staff       (20)      984 2023-04-16 04:54:31.000000 mls-api-1.0.9/mls_api/teams.py
--rw-r--r--   0 finn       (501) staff       (20)     2438 2023-04-16 04:54:28.000000 mls-api-1.0.9/mls_api/top_scorer.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-16 05:17:55.000000 mls-api-1.0.9/mls_api/version.py
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 05:18:38.834114 mls-api-1.0.9/mls_api.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     5430 2023-04-16 05:18:38.000000 mls-api-1.0.9/mls_api.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      472 2023-04-16 05:18:38.000000 mls-api-1.0.9/mls_api.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 05:18:38.000000 mls-api-1.0.9/mls_api.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 05:18:18.000000 mls-api-1.0.9/mls_api.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-16 05:18:38.000000 mls-api-1.0.9/mls_api.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)        8 2023-04-16 05:18:38.000000 mls-api-1.0.9/mls_api.egg-info/top_level.txt
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-16 05:18:38.835199 mls-api-1.0.9/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2476 2023-04-16 05:17:55.000000 mls-api-1.0.9/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 16:29:21.509856 mls-api-1.1.0/
+-rw-r--r--   0 finn       (501) staff       (20)     5304 2023-04-16 16:29:21.510048 mls-api-1.1.0/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     2258 2023-04-16 06:16:08.000000 mls-api-1.1.0/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 16:29:21.505750 mls-api-1.1.0/mls_api/
+-rw-r--r--   0 finn       (501) staff       (20)      343 2023-04-16 16:27:54.000000 mls-api-1.1.0/mls_api/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     1492 2023-04-16 06:08:58.000000 mls-api-1.1.0/mls_api/assists.py
+-rw-r--r--   0 finn       (501) staff       (20)      655 2023-04-16 16:27:55.000000 mls-api-1.1.0/mls_api/auth.py
+-rw-r--r--   0 finn       (501) staff       (20)     1500 2023-04-16 06:09:04.000000 mls-api-1.1.0/mls_api/fixtures.py
+-rw-r--r--   0 finn       (501) staff       (20)     1510 2023-04-16 06:09:06.000000 mls-api-1.1.0/mls_api/historical.py
+-rw-r--r--   0 finn       (501) staff       (20)     1298 2023-04-16 16:27:52.000000 mls-api-1.1.0/mls_api/latest_news.py
+-rw-r--r--   0 finn       (501) staff       (20)     1492 2023-04-16 06:09:17.000000 mls-api-1.1.0/mls_api/offense.py
+-rw-r--r--   0 finn       (501) staff       (20)     1716 2023-04-16 06:12:07.000000 mls-api-1.1.0/mls_api/players.py
+-rw-r--r--   0 finn       (501) staff       (20)     1458 2023-04-16 06:09:21.000000 mls-api-1.1.0/mls_api/rtd.py
+-rw-r--r--   0 finn       (501) staff       (20)    34581 2023-04-16 06:09:23.000000 mls-api-1.1.0/mls_api/six.py
+-rw-r--r--   0 finn       (501) staff       (20)     1508 2023-04-16 06:09:26.000000 mls-api-1.1.0/mls_api/standings.py
+-rw-r--r--   0 finn       (501) staff       (20)     1476 2023-04-16 06:09:28.000000 mls-api-1.1.0/mls_api/teams.py
+-rw-r--r--   0 finn       (501) staff       (20)     1512 2023-04-16 06:09:30.000000 mls-api-1.1.0/mls_api/top_scorer.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-16 06:30:02.000000 mls-api-1.1.0/mls_api/version.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 16:29:21.509287 mls-api-1.1.0/mls_api.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     5304 2023-04-16 16:29:21.000000 mls-api-1.1.0/mls_api.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      479 2023-04-16 16:29:21.000000 mls-api-1.1.0/mls_api.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 16:29:21.000000 mls-api-1.1.0/mls_api.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 16:29:03.000000 mls-api-1.1.0/mls_api.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-16 16:29:21.000000 mls-api-1.1.0/mls_api.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)        8 2023-04-16 16:29:21.000000 mls-api-1.1.0/mls_api.egg-info/top_level.txt
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-16 16:29:21.510562 mls-api-1.1.0/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2476 2023-04-16 06:30:02.000000 mls-api-1.1.0/setup.py
```

### Comparing `mls-api-1.0.9/README.md` & `mls-api-1.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -24,67 +24,68 @@
 ## or `sudo python setup.py install` to install the package for all users
 ```
 
 Usage Example
 -------------
 
 ```python
-import os, json
 import mls_api
+from dotenv import load_dotenv
+import os
 
-# Authentication
-username = "your_username"
-password = "your_password"
-response_text = mls_api.login(username, password)
-print("Login response:", response_text)
-
-# Get all historical data
-response_text = mls_api.get_all_hist()
-print("All historical data response:", response_text)
-
-# Get all real-time data (RTD)
-response_text = mls_api.get_all_rtd()
-print("All real-time data response:", response_text)
-
-# Get a list of players with a custom limit and offset
-limit = 20
-offset = 10
-response_text = mls_api.get_all_players(limit, offset)
-print("Players response:", response_text)
-
-# Get all top scorers data
-all_topscorers = mls_api.get_all_topscorers()
-print("All Top Scorers:")
-print(all_topscorers)
-
-# Get all offence data
-all_offences = mls_api.get_all_offences()
-print("All Offences:")
-print(all_offences)
-
-# Get all assists data
-all_assists = mls_api.get_all_assists()
-print("All Assists:")
-print(all_assists)
-
-# Get all teams data
-all_teams = mls_api.get_all_teams()
-print("All teams:\n", all_teams)
-
-# Get all fixtures data
-all_fixtures = mls_api.get_all_fixtures()
-print("All fixtures:\n", all_fixtures)
-
-# Get all standings data
-all_standings = mls_api.get_all_standings()
-print(all_standings)
-
-# Get all news data
-all_news = mls_api.get_all_news()
-print(all_news)
+## Loads environment variables from .env
+load_dotenv('.env')
+
+username = os.getenv('_USERNAME')
+password = os.getenv('_PASSWORD')
+
+## Authentication
+mls_api.login(username, password)
+
+## Retrieve MLS Real-Time Data
+mls_rtd = mls_api.get_rtd()
+print(mls_rtd)
+
+## Retrieve MLS Historical Data
+mls_historical = mls_api.get_historical_data()
+print(mls_historical)
+
+## Retrieve MLS Players Data
+limit = 10
+offset = 5
+mls_players = mls_api.get_players(limit=limit, offset=offset)
+print(mls_players)
+
+## Retrieve MLS Assist Data
+mls_assists = mls_api.get_assists()
+print(mls_assists)
+
+## Retrieve MLS Offence Data
+mls_offence = mls_api.get_offence()
+print(mls_offence)
+
+## Retrieve MLS Top Scorers Data
+mls_top_scorer = mls_api.get_top_scorer()
+print(mls_top_scorer)
+
+## Retrieve MLS Teams Data
+mls_teams = mls_api.get_teams()
+print(mls_teams)
+
+## Retrieve MLS Fixtures Data
+mls_fixtures = mls_api.get_fixtures()
+print(mls_fixtures)
+
+## Retrieve MLS Standings Data
+mls_standings = mls_api.get_standings()
+print(mls_standings)
+
+## Retrieve MLS Latest News Data
+mls_latest_news = mls_api.get_latest_news()
+print(mls_latest_news)
 ```
 
 ## Setting up an MLS API Account
 
 Sign up for a self-service [user account](https://moatsystems.com/mls-api/).
```

### Comparing `mls-api-1.0.9/mls_api/historical.py` & `mls-api-1.1.0/mls_api/assists.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,48 @@
-import os, json
 import requests
+import json
+import os
 
-def get_all_hist():
+def get_assists(id=None):
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = "https://mlssoccerapi.com/hist"
-    payload = {}
-    headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {bearerToken}'}
-    response = requests.request("GET", url, headers=headers, data=payload)
-    return response.text
+    url = 'https://mlssoccerapi.com/assists/'
+    headers = {
+        'Content-Type': 'application/json', 
+        'Authorization': f'Bearer {bearerToken}'
+    }
+    if id != None: 
+        url += id
+    response = requests.get(url=url, headers=headers)
+    return response.json()
 
-def get_hist_by_id(hist_id):
-    bearerToken = os.getenv('BEARER_TOKEN')
-    url = f"https://mlssoccerapi.com/hist/{hist_id}"
-    payload = {}
-    headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {bearerToken}'}
-    response = requests.request("GET", url, headers=headers, data=payload)
-    return response.text
-
-def update_hist_by_id(hist_id, data):
-    bearerToken = os.getenv('BEARER_TOKEN')
-    url = f"https://mlssoccerapi.com/hist/{hist_id}"
-    payload = json.dumps(data)
-    headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {bearerToken}'}
-    response = requests.request("PUT", url, headers=headers, data=payload)
-    return response.text
+def update_assists(id, payload):
+    bearerToken = os.getenv('BEARER_TOKEN') 
+    url = f'https://mlssoccerapi.com/assists/{id}'
+    headers = {
+        'Content-Type': 'application/json', 
+        'Authorization': f'Bearer {bearerToken}'
+    }
+    response = requests.put(url=url, headers=headers, data=payload)
+    return response.json()
 
-def delete_hist_by_id(hist_id):
+def delete_assists(id): 
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = f"https://mlssoccerapi.com/hist/{hist_id}"
-    payload = json.dumps({"id": hist_id})
-    headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {bearerToken}'}
-    response = requests.request("DELETE", url, headers=headers, data=payload)
-    return response.text
+    url = f'https://mlssoccerapi.com/assists/{id}'
+    headers = {
+        'Content-Type': 'application/json', 
+        'Authorization': f'Bearer {bearerToken}'
+    }
+    payload = json.dumps({
+        'id': id
+    })
+    response = requests.delete(url=url, headers=headers, data=payload)
+    return response.json()
 
-def add_new_hist(data):
+def add_assists(payload):
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = "https://mlssoccerapi.com/hist"
-    payload = json.dumps(data)
-    headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {bearerToken}'}
-    response = requests.request("POST", url, headers=headers, data=payload)
-    return response.text
+    url = 'https://mlssoccerapi.com/assists/'
+    headers = {
+        'Content-Type': 'application/json', 
+        'Authorization': f'Bearer {bearerToken}'
+    }
+    response = requests.post(url=url, headers=headers, data=payload)
+    return response.json()
```

### Comparing `mls-api-1.0.9/mls_api/players.py` & `mls-api-1.1.0/mls_api/players.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,56 @@
-import os, json
 import requests
+import json
+import os
 
-def get_all_players(limit=10, offset=0):
+def get_players(id=None, limit=None, offset=None):
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = f"https://mlssoccerapi.com/players?limit={limit}&offset={offset}"
-    payload = {}
-    headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {bearerToken}'}
-    response = requests.request("GET", url, headers=headers, data=payload)
-    return response.text
+    url = 'https://mlssoccerapi.com/players/'
+    headers = {
+        'Content-Type': 'application/json', 
+        'Authorization': f'Bearer {bearerToken}'
+    }
 
-def get_player_by_id(player_id):
-    bearerToken = os.getenv('BEARER_TOKEN')
-    url = f"https://mlssoccerapi.com/players/{player_id}"
-    payload = {}
-    headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {bearerToken}'}
-    response = requests.request("GET", url, headers=headers, data=payload)
-    return response.text
+    # Add query parameters if provided
+    params = {}
+    if limit is not None:
+        params['limit'] = limit
+    if offset is not None:
+        params['offset'] = offset
 
-def update_player_by_id(player_id, data):
-    bearerToken = os.getenv('BEARER_TOKEN')
-    url = f"https://mlssoccerapi.com/players/{player_id}"
-    payload = json.dumps(data)
-    headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {bearerToken}'}
-    response = requests.request("PUT", url, headers=headers, data=payload)
-    return response.text
+    if id != None: 
+        url += id
+    response = requests.get(url=url, headers=headers, params=params)
+    return response.json()
+
+def update_players(id, payload):
+    bearerToken = os.getenv('BEARER_TOKEN') 
+    url = f'https://mlssoccerapi.com/players/{id}'
+    headers = {
+        'Content-Type': 'application/json', 
+        'Authorization': f'Bearer {bearerToken}'
+    }
+    response = requests.put(url=url, headers=headers, data=payload)
+    return response.json()
 
-def delete_player_by_id(player_id):
+def delete_players(id): 
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = f"https://mlssoccerapi.com/players/{player_id}"
-    payload = json.dumps({"id": player_id})
-    headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {bearerToken}'}
-    response = requests.request("DELETE", url, headers=headers, data=payload)
-    return response.text
+    url = f'https://mlssoccerapi.com/players/{id}'
+    headers = {
+        'Content-Type': 'application/json', 
+        'Authorization': f'Bearer {bearerToken}'
+    }
+    payload = json.dumps({
+        'id': id
+    })
+    response = requests.delete(url=url, headers=headers, data=payload)
+    return response.json()
 
-def add_new_player(data):
+def add_players(payload):
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = "https://mlssoccerapi.com/players"
-    payload = json.dumps(data)
-    headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {bearerToken}'}
-    response = requests.request("POST", url, headers=headers, data=payload)
-    return response.text
+    url = 'https://mlssoccerapi.com/players/'
+    headers = {
+        'Content-Type': 'application/json', 
+        'Authorization': f'Bearer {bearerToken}'
+    }
+    response = requests.post(url=url, headers=headers, data=payload)
+    return response.json()
```

### Comparing `mls-api-1.0.9/mls_api/rtd.py` & `mls-api-1.1.0/mls_api/historical.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,48 @@
-import os, json
 import requests
+import json
+import os
 
-def get_all_rtd():
+def get_historical_data(id=None):
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = "https://mlssoccerapi.com/rtd"
-    payload = {}
-    headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {bearerToken}'}
-    response = requests.request("GET", url, headers=headers, data=payload)
-    return response.text
+    url = 'https://mlssoccerapi.com/hist'
+    headers = {
+        'Content-Type': 'application/json', 
+        'Authorization': f'Bearer {bearerToken}'
+    }
+    if id != None: 
+        url += id
+    response = requests.get(url=url, headers=headers)
+    return response.json()
 
-def get_rtd_by_id(rtd_id):
-    bearerToken = os.getenv('BEARER_TOKEN')
-    url = f"https://mlssoccerapi.com/rtd/{rtd_id}"
-    payload = {}
-    headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {bearerToken}'}
-    response = requests.request("GET", url, headers=headers, data=payload)
-    return response.text
-
-def update_rtd_by_id(rtd_id, data):
-    bearerToken = os.getenv('BEARER_TOKEN')
-    url = f"https://mlssoccerapi.com/rtd/{rtd_id}"
-    payload = json.dumps(data)
-    headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {bearerToken}'}
-    response = requests.request("PUT", url, headers=headers, data=payload)
-    return response.text
+def update_historical_data(id, payload):
+    bearerToken = os.getenv('BEARER_TOKEN') 
+    url = f'https://mlssoccerapi.com/hist/{id}'
+    headers = {
+        'Content-Type': 'application/json', 
+        'Authorization': f'Bearer {bearerToken}'
+    }
+    response = requests.put(url=url, headers=headers, data=payload)
+    return response.json()
 
-def delete_rtd_by_id(rtd_id):
+def delete_historical_data(id): 
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = f"https://mlssoccerapi.com/rtd/{rtd_id}"
-    payload = json.dumps({"id": rtd_id})
-    headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {bearerToken}'}
-    response = requests.request("DELETE", url, headers=headers, data=payload)
-    return response.text
+    url = f'https://mlssoccerapi.com/hist/{id}'
+    headers = {
+        'Content-Type': 'application/json', 
+        'Authorization': f'Bearer {bearerToken}'
+    }
+    payload = json.dumps({
+        'id': id
+    })
+    response = requests.delete(url=url, headers=headers, data=payload)
+    return response.json()
 
-def add_new_rtd(data):
+def add_historical_data(payload):
     bearerToken = os.getenv('BEARER_TOKEN')
-    url = "https://mlssoccerapi.com/rtd"
-    payload = json.dumps(data)
-    headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {bearerToken}'}
-    response = requests.request("POST", url, headers=headers, data=payload)
-    return response.text
+    url = 'https://mlssoccerapi.com/hist'
+    headers = {
+        'Content-Type': 'application/json', 
+        'Authorization': f'Bearer {bearerToken}'
+    }
+    response = requests.post(url=url, headers=headers, data=payload)
+    return response.json()
```

### Comparing `mls-api-1.0.9/mls_api/six.py` & `mls-api-1.1.0/mls_api/six.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.9/setup.py` & `mls-api-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "mls-api"
-VERSION = "1.0.9"
+VERSION = "1.1.0"
 REQUIRES = ["requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

