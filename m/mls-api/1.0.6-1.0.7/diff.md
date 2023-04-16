# Comparing `tmp/mls-api-1.0.6.tar.gz` & `tmp/mls-api-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mls-api-1.0.6.tar", last modified: Sat Apr 15 21:54:33 2023, max compression
+gzip compressed data, was "dist/mls-api-1.0.7.tar", last modified: Sun Apr 16 04:32:24 2023, max compression
```

## Comparing `mls-api-1.0.6.tar` & `mls-api-1.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-15 21:54:33.860905 mls-api-1.0.6/
--rw-r--r--   0 finn       (501) staff       (20)     6929 2023-04-15 21:54:33.861118 mls-api-1.0.6/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     3467 2023-04-15 21:50:10.000000 mls-api-1.0.6/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-15 21:54:33.857178 mls-api-1.0.6/mls_api/
--rw-r--r--   0 finn       (501) staff       (20)      413 2022-09-10 10:52:58.000000 mls-api-1.0.6/mls_api/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     1492 2022-09-10 10:20:53.000000 mls-api-1.0.6/mls_api/assists_api.py
--rw-r--r--   0 finn       (501) staff       (20)     1500 2022-09-10 10:20:53.000000 mls-api-1.0.6/mls_api/fixtures_api.py
--rw-r--r--   0 finn       (501) staff       (20)     1510 2022-09-10 10:20:53.000000 mls-api-1.0.6/mls_api/historical_data_api.py
--rw-r--r--   0 finn       (501) staff       (20)     1496 2022-09-10 10:20:53.000000 mls-api-1.0.6/mls_api/latest_news_api.py
--rw-r--r--   0 finn       (501) staff       (20)      655 2022-09-10 10:20:53.000000 mls-api-1.0.6/mls_api/login.py
--rw-r--r--   0 finn       (501) staff       (20)     1492 2022-09-10 10:20:53.000000 mls-api-1.0.6/mls_api/offence_api.py
--rw-r--r--   0 finn       (501) staff       (20)     1786 2023-04-15 21:48:26.000000 mls-api-1.0.6/mls_api/players_api.py
--rw-r--r--   0 finn       (501) staff       (20)     1458 2022-09-10 10:20:53.000000 mls-api-1.0.6/mls_api/real_time_data__live_scores_api.py
--rw-r--r--   0 finn       (501) staff       (20)    34581 2022-08-07 21:22:57.000000 mls-api-1.0.6/mls_api/six.py
--rw-r--r--   0 finn       (501) staff       (20)     1508 2022-09-10 10:20:53.000000 mls-api-1.0.6/mls_api/standings_api.py
--rw-r--r--   0 finn       (501) staff       (20)     1476 2022-09-10 10:20:53.000000 mls-api-1.0.6/mls_api/teams_api.py
--rw-r--r--   0 finn       (501) staff       (20)     1512 2022-09-10 10:20:53.000000 mls-api-1.0.6/mls_api/top_scorer_api.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-15 21:52:31.000000 mls-api-1.0.6/mls_api/version.py
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-15 21:54:33.860380 mls-api-1.0.6/mls_api.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     6929 2023-04-15 21:54:33.000000 mls-api-1.0.6/mls_api.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      549 2023-04-15 21:54:33.000000 mls-api-1.0.6/mls_api.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-15 21:54:33.000000 mls-api-1.0.6/mls_api.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-15 21:54:16.000000 mls-api-1.0.6/mls_api.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-15 21:54:33.000000 mls-api-1.0.6/mls_api.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)        8 2023-04-15 21:54:33.000000 mls-api-1.0.6/mls_api.egg-info/top_level.txt
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-15 21:54:33.861641 mls-api-1.0.6/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2476 2023-04-15 21:52:31.000000 mls-api-1.0.6/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 04:32:24.904910 mls-api-1.0.7/
+-rw-r--r--   0 finn       (501) staff       (20)     7570 2023-04-16 04:32:24.905252 mls-api-1.0.7/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     3932 2023-04-16 04:30:36.000000 mls-api-1.0.7/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 04:32:24.899907 mls-api-1.0.7/mls_api/
+-rw-r--r--   0 finn       (501) staff       (20)      336 2023-04-16 04:30:39.000000 mls-api-1.0.7/mls_api/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     1956 2023-04-16 03:42:40.000000 mls-api-1.0.7/mls_api/assists.py
+-rw-r--r--   0 finn       (501) staff       (20)      381 2023-04-16 03:18:08.000000 mls-api-1.0.7/mls_api/auth.py
+-rw-r--r--   0 finn       (501) staff       (20)      926 2023-04-16 04:08:07.000000 mls-api-1.0.7/mls_api/fixtures.py
+-rw-r--r--   0 finn       (501) staff       (20)     1353 2023-04-16 03:23:28.000000 mls-api-1.0.7/mls_api/historical.py
+-rw-r--r--   0 finn       (501) staff       (20)      886 2023-04-16 04:26:45.000000 mls-api-1.0.7/mls_api/news.py
+-rw-r--r--   0 finn       (501) staff       (20)     2088 2023-04-16 03:45:50.000000 mls-api-1.0.7/mls_api/offense.py
+-rw-r--r--   0 finn       (501) staff       (20)     1442 2023-04-16 03:18:38.000000 mls-api-1.0.7/mls_api/players.py
+-rw-r--r--   0 finn       (501) staff       (20)     1336 2023-04-16 03:30:18.000000 mls-api-1.0.7/mls_api/rtd.py
+-rw-r--r--   0 finn       (501) staff       (20)    34581 2022-08-07 21:22:57.000000 mls-api-1.0.7/mls_api/six.py
+-rw-r--r--   0 finn       (501) staff       (20)      936 2023-04-16 04:23:26.000000 mls-api-1.0.7/mls_api/standings.py
+-rw-r--r--   0 finn       (501) staff       (20)      890 2023-04-16 04:04:21.000000 mls-api-1.0.7/mls_api/teams.py
+-rw-r--r--   0 finn       (501) staff       (20)     1999 2023-04-16 03:54:25.000000 mls-api-1.0.7/mls_api/top_scorer.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-16 04:31:33.000000 mls-api-1.0.7/mls_api/version.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 04:32:24.904317 mls-api-1.0.7/mls_api.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     7570 2023-04-16 04:32:24.000000 mls-api-1.0.7/mls_api.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      472 2023-04-16 04:32:24.000000 mls-api-1.0.7/mls_api.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 04:32:24.000000 mls-api-1.0.7/mls_api.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 04:32:10.000000 mls-api-1.0.7/mls_api.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-16 04:32:24.000000 mls-api-1.0.7/mls_api.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)        8 2023-04-16 04:32:24.000000 mls-api-1.0.7/mls_api.egg-info/top_level.txt
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-16 04:32:24.906507 mls-api-1.0.7/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2476 2023-04-16 04:31:26.000000 mls-api-1.0.7/setup.py
```

### Comparing `mls-api-1.0.6/mls_api/latest_news_api.py` & `mls-api-1.0.7/mls_api/offense.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,59 @@
 import requests
 import json
-import os
 
-def get_latest_news(id=None):
-    bearerToken = os.getenv('BEARER_TOKEN')
-    url = 'https://mlssoccerapi.com/news/'
-    headers = {
-        'Content-Type': 'application/json', 
-        'Authorization': f'Bearer {bearerToken}'
-    }
-    if id != None: 
-        url += id
-    response = requests.get(url=url, headers=headers)
-    return response.json()
-
-def update_latest_news(id, payload):
-    bearerToken = os.getenv('BEARER_TOKEN') 
-    url = f'https://mlssoccerapi.com/news/{id}'
-    headers = {
-        'Content-Type': 'application/json', 
-        'Authorization': f'Bearer {bearerToken}'
-    }
-    response = requests.put(url=url, headers=headers, data=payload)
-    return response.json()
-
-def delete_latest_news(id): 
-    bearerToken = os.getenv('BEARER_TOKEN')
-    url = f'https://mlssoccerapi.com/news/{id}'
-    headers = {
-        'Content-Type': 'application/json', 
-        'Authorization': f'Bearer {bearerToken}'
-    }
+def get_all_offence():
+    url = "https://mlssoccerapi.com/offence"
+    payload = {}
+    headers = {'Content-Type': 'application/json'}
+    response = requests.request("GET", url, headers=headers, data=payload)
+    return response.text
+
+
+def get_offence_by_id(offence_id):
+    url = f"https://mlssoccerapi.com/offence/{offence_id}"
+    payload = {}
+    headers = {'Content-Type': 'application/json'}
+    response = requests.request("GET", url, headers=headers, data=payload)
+    return response.text
+
+
+def update_offence_by_id(offence_id, league_name, standing, player_name, team_name, yellow_cards, red_cards, tag):
+    url = f"https://mlssoccerapi.com/offence/{offence_id}"
     payload = json.dumps({
-        'id': id
+        "id": offence_id,
+        "league_name": league_name,
+        "standing": standing,
+        "player_name": player_name,
+        "team_name": team_name,
+        "yellow_cards": yellow_cards,
+        "red_cards": red_cards,
+        "tag": tag
     })
-    response = requests.delete(url=url, headers=headers, data=payload)
-    return response.json()
+    headers = {'Content-Type': 'application/json'}
+    response = requests.request("PUT", url, headers=headers, data=payload)
+    return response.text
+
 
-def add_latest_news(payload):
-    bearerToken = os.getenv('BEARER_TOKEN')
-    url = 'https://mlssoccerapi.com/news/'
-    headers = {
-        'Content-Type': 'application/json', 
-        'Authorization': f'Bearer {bearerToken}'
-    }
-    response = requests.post(url=url, headers=headers, data=payload)
-    return response.json()
+def delete_offence_by_id(offence_id):
+    url = f"https://mlssoccerapi.com/offence/{offence_id}"
+    payload = json.dumps({"id": offence_id})
+    headers = {'Content-Type': 'application/json'}
+    response = requests.request("DELETE", url, headers=headers, data=payload)
+    return response.text
+
+
+def add_new_offence(offence_id, league_name, standing, player_name, team_name, yellow_cards, red_cards, tag):
+    url = "https://mlssoccerapi.com/offence"
+    payload = json.dumps({
+        "id": offence_id,
+        "league_name": league_name,
+        "standing": standing,
+        "player_name": player_name,
+        "team_name": team_name,
+        "yellow_cards": yellow_cards,
+        "red_cards": red_cards,
+        "tag": tag
+    })
+    headers = {'Content-Type': 'application/json'}
+    response = requests.request("POST", url, headers=headers, data=payload)
+    return response.text
```

### Comparing `mls-api-1.0.6/mls_api/six.py` & `mls-api-1.0.7/mls_api/six.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.6/mls_api/top_scorer_api.py` & `mls-api-1.0.7/mls_api/top_scorer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,48 +1,57 @@
 import requests
 import json
-import os
 
-def get_top_scorer(id=None):
-    bearerToken = os.getenv('BEARER_TOKEN')
-    url = 'https://mlssoccerapi.com/topscorer/'
-    headers = {
-        'Content-Type': 'application/json', 
-        'Authorization': f'Bearer {bearerToken}'
-    }
-    if id != None: 
-        url += id
-    response = requests.get(url=url, headers=headers)
-    return response.json()
-
-def update_top_scorer(id, payload):
-    bearerToken = os.getenv('BEARER_TOKEN') 
-    url = f'https://mlssoccerapi.com/topscorer/{id}'
-    headers = {
-        'Content-Type': 'application/json', 
-        'Authorization': f'Bearer {bearerToken}'
-    }
-    response = requests.put(url=url, headers=headers, data=payload)
-    return response.json()
-
-def delete_top_scorer(id): 
-    bearerToken = os.getenv('BEARER_TOKEN')
-    url = f'https://mlssoccerapi.com/topscorer/{id}'
-    headers = {
-        'Content-Type': 'application/json', 
-        'Authorization': f'Bearer {bearerToken}'
-    }
+def get_all_topscorers():
+    url = "https://mlssoccerapi.com/topscorer"
+    payload = {}
+    headers = {'Content-Type': 'application/json'}
+    response = requests.request("GET", url, headers=headers, data=payload)
+    return response.text
+
+
+def get_topscorer_by_id(topscorer_id):
+    url = f"https://mlssoccerapi.com/topscorer/{topscorer_id}"
+    payload = {}
+    headers = {'Content-Type': 'application/json'}
+    response = requests.request("GET", url, headers=headers, data=payload)
+    return response.text
+
+
+def update_topscorer_by_id(topscorer_id, league_name, standing, player_name, team_name, goals, tag):
+    url = f"https://mlssoccerapi.com/topscorer/{topscorer_id}"
     payload = json.dumps({
-        'id': id
+        "id": topscorer_id,
+        "league_name": league_name,
+        "standing": standing,
+        "player_name": player_name,
+        "team_name": team_name,
+        "goals": goals,
+        "tag": tag
     })
-    response = requests.delete(url=url, headers=headers, data=payload)
-    return response.json()
+    headers = {'Content-Type': 'application/json'}
+    response = requests.request("PUT", url, headers=headers, data=payload)
+    return response.text
+
 
-def add_top_scorer(payload):
-    bearerToken = os.getenv('BEARER_TOKEN')
-    url = 'https://mlssoccerapi.com/topscorer/'
-    headers = {
-        'Content-Type': 'application/json', 
-        'Authorization': f'Bearer {bearerToken}'
-    }
-    response = requests.post(url=url, headers=headers, data=payload)
-    return response.json()
+def delete_topscorer_by_id(topscorer_id):
+    url = f"https://mlssoccerapi.com/topscorer/{topscorer_id}"
+    payload = json.dumps({"id": topscorer_id})
+    headers = {'Content-Type': 'application/json'}
+    response = requests.request("DELETE", url, headers=headers, data=payload)
+    return response.text
+
+
+def add_new_topscorer(topscorer_id, league_name, standing, player_name, team_name, goals, tag):
+    url = "https://mlssoccerapi.com/topscorer"
+    payload = json.dumps({
+        "id": topscorer_id,
+        "league_name": league_name,
+        "standing": standing,
+        "player_name": player_name,
+        "team_name": team_name,
+        "goals": goals,
+        "tag": tag
+    })
+    headers = {'Content-Type': 'application/json'}
+    response = requests.request("POST", url, headers=headers, data=payload)
+    return response.text
```

### Comparing `mls-api-1.0.6/setup.py` & `mls-api-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "mls-api"
-VERSION = "1.0.6"
+VERSION = "1.0.7"
 REQUIRES = ["requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

