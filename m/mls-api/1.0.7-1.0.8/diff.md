# Comparing `tmp/mls-api-1.0.7.tar.gz` & `tmp/mls-api-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mls-api-1.0.7.tar", last modified: Sun Apr 16 04:32:24 2023, max compression
+gzip compressed data, was "dist/mls-api-1.0.8.tar", last modified: Sun Apr 16 04:59:17 2023, max compression
```

## Comparing `mls-api-1.0.7.tar` & `mls-api-1.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 04:32:24.904910 mls-api-1.0.7/
--rw-r--r--   0 finn       (501) staff       (20)     7570 2023-04-16 04:32:24.905252 mls-api-1.0.7/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)     3932 2023-04-16 04:30:36.000000 mls-api-1.0.7/README.md
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 04:32:24.899907 mls-api-1.0.7/mls_api/
--rw-r--r--   0 finn       (501) staff       (20)      336 2023-04-16 04:30:39.000000 mls-api-1.0.7/mls_api/__init__.py
--rw-r--r--   0 finn       (501) staff       (20)     1956 2023-04-16 03:42:40.000000 mls-api-1.0.7/mls_api/assists.py
--rw-r--r--   0 finn       (501) staff       (20)      381 2023-04-16 03:18:08.000000 mls-api-1.0.7/mls_api/auth.py
--rw-r--r--   0 finn       (501) staff       (20)      926 2023-04-16 04:08:07.000000 mls-api-1.0.7/mls_api/fixtures.py
--rw-r--r--   0 finn       (501) staff       (20)     1353 2023-04-16 03:23:28.000000 mls-api-1.0.7/mls_api/historical.py
--rw-r--r--   0 finn       (501) staff       (20)      886 2023-04-16 04:26:45.000000 mls-api-1.0.7/mls_api/news.py
--rw-r--r--   0 finn       (501) staff       (20)     2088 2023-04-16 03:45:50.000000 mls-api-1.0.7/mls_api/offense.py
--rw-r--r--   0 finn       (501) staff       (20)     1442 2023-04-16 03:18:38.000000 mls-api-1.0.7/mls_api/players.py
--rw-r--r--   0 finn       (501) staff       (20)     1336 2023-04-16 03:30:18.000000 mls-api-1.0.7/mls_api/rtd.py
--rw-r--r--   0 finn       (501) staff       (20)    34581 2022-08-07 21:22:57.000000 mls-api-1.0.7/mls_api/six.py
--rw-r--r--   0 finn       (501) staff       (20)      936 2023-04-16 04:23:26.000000 mls-api-1.0.7/mls_api/standings.py
--rw-r--r--   0 finn       (501) staff       (20)      890 2023-04-16 04:04:21.000000 mls-api-1.0.7/mls_api/teams.py
--rw-r--r--   0 finn       (501) staff       (20)     1999 2023-04-16 03:54:25.000000 mls-api-1.0.7/mls_api/top_scorer.py
--rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-16 04:31:33.000000 mls-api-1.0.7/mls_api/version.py
-drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 04:32:24.904317 mls-api-1.0.7/mls_api.egg-info/
--rw-r--r--   0 finn       (501) staff       (20)     7570 2023-04-16 04:32:24.000000 mls-api-1.0.7/mls_api.egg-info/PKG-INFO
--rw-r--r--   0 finn       (501) staff       (20)      472 2023-04-16 04:32:24.000000 mls-api-1.0.7/mls_api.egg-info/SOURCES.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 04:32:24.000000 mls-api-1.0.7/mls_api.egg-info/dependency_links.txt
--rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 04:32:10.000000 mls-api-1.0.7/mls_api.egg-info/not-zip-safe
--rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-16 04:32:24.000000 mls-api-1.0.7/mls_api.egg-info/requires.txt
--rw-r--r--   0 finn       (501) staff       (20)        8 2023-04-16 04:32:24.000000 mls-api-1.0.7/mls_api.egg-info/top_level.txt
--rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-16 04:32:24.906507 mls-api-1.0.7/setup.cfg
--rw-r--r--   0 finn       (501) staff       (20)     2476 2023-04-16 04:31:26.000000 mls-api-1.0.7/setup.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 04:59:17.513277 mls-api-1.0.8/
+-rw-r--r--   0 finn       (501) staff       (20)     5422 2023-04-16 04:59:17.513490 mls-api-1.0.8/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)     2380 2023-04-16 04:58:30.000000 mls-api-1.0.8/README.md
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 04:59:17.509139 mls-api-1.0.8/mls_api/
+-rw-r--r--   0 finn       (501) staff       (20)      336 2023-04-16 04:30:39.000000 mls-api-1.0.8/mls_api/__init__.py
+-rw-r--r--   0 finn       (501) staff       (20)     2395 2023-04-16 04:49:43.000000 mls-api-1.0.8/mls_api/assists.py
+-rw-r--r--   0 finn       (501) staff       (20)      381 2023-04-16 03:18:08.000000 mls-api-1.0.8/mls_api/auth.py
+-rw-r--r--   0 finn       (501) staff       (20)     1020 2023-04-16 04:50:28.000000 mls-api-1.0.8/mls_api/fixtures.py
+-rw-r--r--   0 finn       (501) staff       (20)     1792 2023-04-16 04:49:02.000000 mls-api-1.0.8/mls_api/historical.py
+-rw-r--r--   0 finn       (501) staff       (20)      982 2023-04-16 04:51:14.000000 mls-api-1.0.8/mls_api/news.py
+-rw-r--r--   0 finn       (501) staff       (20)     2527 2023-04-16 04:52:02.000000 mls-api-1.0.8/mls_api/offense.py
+-rw-r--r--   0 finn       (501) staff       (20)     1881 2023-04-16 04:52:39.000000 mls-api-1.0.8/mls_api/players.py
+-rw-r--r--   0 finn       (501) staff       (20)     1775 2023-04-16 04:53:09.000000 mls-api-1.0.8/mls_api/rtd.py
+-rw-r--r--   0 finn       (501) staff       (20)    34581 2022-08-07 21:22:57.000000 mls-api-1.0.8/mls_api/six.py
+-rw-r--r--   0 finn       (501) staff       (20)     1032 2023-04-16 04:53:34.000000 mls-api-1.0.8/mls_api/standings.py
+-rw-r--r--   0 finn       (501) staff       (20)      984 2023-04-16 04:54:31.000000 mls-api-1.0.8/mls_api/teams.py
+-rw-r--r--   0 finn       (501) staff       (20)     2438 2023-04-16 04:54:28.000000 mls-api-1.0.8/mls_api/top_scorer.py
+-rw-r--r--   0 finn       (501) staff       (20)       17 2023-04-16 04:58:44.000000 mls-api-1.0.8/mls_api/version.py
+drwxr-xr-x   0 finn       (501) staff       (20)        0 2023-04-16 04:59:17.512818 mls-api-1.0.8/mls_api.egg-info/
+-rw-r--r--   0 finn       (501) staff       (20)     5422 2023-04-16 04:59:17.000000 mls-api-1.0.8/mls_api.egg-info/PKG-INFO
+-rw-r--r--   0 finn       (501) staff       (20)      472 2023-04-16 04:59:17.000000 mls-api-1.0.8/mls_api.egg-info/SOURCES.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 04:59:17.000000 mls-api-1.0.8/mls_api.egg-info/dependency_links.txt
+-rw-r--r--   0 finn       (501) staff       (20)        1 2023-04-16 04:59:03.000000 mls-api-1.0.8/mls_api.egg-info/not-zip-safe
+-rw-r--r--   0 finn       (501) staff       (20)        9 2023-04-16 04:59:17.000000 mls-api-1.0.8/mls_api.egg-info/requires.txt
+-rw-r--r--   0 finn       (501) staff       (20)        8 2023-04-16 04:59:17.000000 mls-api-1.0.8/mls_api.egg-info/top_level.txt
+-rw-r--r--   0 finn       (501) staff       (20)       38 2023-04-16 04:59:17.514315 mls-api-1.0.8/setup.cfg
+-rw-r--r--   0 finn       (501) staff       (20)     2476 2023-04-16 04:58:44.000000 mls-api-1.0.8/setup.py
```

### Comparing `mls-api-1.0.7/PKG-INFO` & `mls-api-1.0.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mls-api
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python library for integrating with the MLS (Major League Soccer) API.
 Home-page: https://moatsystems.com/mls-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/moatsystems/mlsapi-python/issues
 Project-URL: Changes, https://github.com/moatsystems/mlsapi-python/blob/main/CHANGELOG.md
@@ -55,111 +55,58 @@
             # Authentication
             username = "your_username"
             password = "your_password"
             response_text = login(username, password)
             print("Login response:", response_text)
         
             # Get all historical data
-            response_text = get_all_hist()
+            response_text = mls_api.get_all_hist()
             print("All historical data response:", response_text)
         
-            # Get historical data by ID
-            hist_id = "the_uuid" # UUID
-            response_text = get_hist_by_id(hist_id)
-            print("Historical data by ID response:", response_text)
-        
             # Get all real-time data (RTD)
-            response_text = get_all_rtd()
+            response_text = mls_api.get_all_rtd()
             print("All real-time data response:", response_text)
         
-            # Get real-time data (RTD) by ID
-            rtd_id = "the_uuid" # UUID
-            response_text = get_rtd_by_id(rtd_id)
-            print("Real-time data by ID response:", response_text)
-        
             # Get a list of players with a custom limit and offset
             limit = 20
             offset = 10
-            response_text = get_all_players(limit, offset)
+            response_text = mls_api.get_all_players(limit, offset)
             print("Players response:", response_text)
         
-            # Get a specific player by ID
-            player_id = "the_uuid" # UUID
-            response_text = get_player_by_id(player_id)
-            print("Player by ID response:", response_text)
-        
             # Get all top scorers data
-            all_topscorers = topscorer.get_all_topscorers()
+            all_topscorers = mls_api.get_all_topscorers()
             print("All Top Scorers:")
             print(all_topscorers)
         
-            # Get top scorers data by ID
-            topscorer_id = "the_uuid" # UUID
-            specific_topscorer = topscorer.get_topscorer_by_id(topscorer_id)
-            print(f"Top Scorer with ID {topscorer_id}:")
-            print(specific_topscorer)
-        
             # Get all offence data
-            all_offences = offence.get_all_offences()
+            all_offences = mls_api.get_all_offences()
             print("All Offences:")
             print(all_offences)
         
-            # Get offence data by ID
-            offence_id = "the_uuid" # UUID
-            specific_offence = offence.get_offence_by_id(offence_id)
-            print(f"Offence with ID {offence_id}:")
-            print(specific_offence)
-        
             # Get all assists data
-            all_assists = assists.get_all_assists()
+            all_assists = mls_api.get_all_assists()
             print("All Assists:")
             print(all_assists)
         
-            # Get assists data by ID
-            assist_id = "the_uuid" # UUID
-            specific_assist = assists.get_assist_by_id(assist_id)
-            print(f"Assist with ID {assist_id}:")
-            print(specific_assist)
-        
             # Get all teams data
-            all_teams = teams.get_all_teams()
+            all_teams = mls_api.get_all_teams()
             print("All teams:\n", all_teams)
         
-            # Get teams data by ID
-            team_id = "the_uuid" # UUID
-            team = teams.get_team_by_id(team_id)
-            print(f"Team with ID {team_id}:\n", team)
-        
             # Get all fixtures data
-            all_fixtures = fixtures.get_all_fixtures()
+            all_fixtures = mls_api.get_all_fixtures()
             print("All fixtures:\n", all_fixtures)
         
-            # Get fixtures data by ID
-            fixture_id = "the_uuid" # UUID
-            fixture = fixtures.get_fixture_by_id(fixture_id)
-            print(f"Fixture with ID {fixture_id}:\n", fixture)
-        
             # Get all standings data
-            all_standings = standings.get_all_standings()
+            all_standings = mls_api.get_all_standings()
             print(all_standings)
         
-            # Get a specific standing by ID
-            standing_id = "the_uuid" # UUID
-            specific_standing = standings.get_standing_by_id(standing_id)
-            print(specific_standing)
-        
             # Get all news data
-            all_news = news.get_all_news()
+            all_news = mls_api.get_all_news()
             print(all_news)
         
-            # Get a specific news item by ID
-            news_id = "the_uuid" # UUID
-            specific_news = news.get_news_by_id(news_id)
-            print(specific_news)
-        
         
         Setting up an MLS API Account
         -----------------------------
         
         Sign up for a self-service `user account`_.
         
         .. _user account: https://moatsystems.com/mls-api/
```

### Comparing `mls-api-1.0.7/README.md` & `mls-api-1.0.8/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -34,110 +34,57 @@
 # Authentication
 username = "your_username"
 password = "your_password"
 response_text = login(username, password)
 print("Login response:", response_text)
 
 # Get all historical data
-response_text = get_all_hist()
+response_text = mls_api.get_all_hist()
 print("All historical data response:", response_text)
 
-# Get historical data by ID
-hist_id = "the_uuid" # UUID
-response_text = get_hist_by_id(hist_id)
-print("Historical data by ID response:", response_text)
-
 # Get all real-time data (RTD)
-response_text = get_all_rtd()
+response_text = mls_api.get_all_rtd()
 print("All real-time data response:", response_text)
 
-# Get real-time data (RTD) by ID
-rtd_id = "the_uuid" # UUID
-response_text = get_rtd_by_id(rtd_id)
-print("Real-time data by ID response:", response_text)
-
 # Get a list of players with a custom limit and offset
 limit = 20
 offset = 10
-response_text = get_all_players(limit, offset)
+response_text = mls_api.get_all_players(limit, offset)
 print("Players response:", response_text)
 
-# Get a specific player by ID
-player_id = "the_uuid" # UUID
-response_text = get_player_by_id(player_id)
-print("Player by ID response:", response_text)
-
 # Get all top scorers data
-all_topscorers = topscorer.get_all_topscorers()
+all_topscorers = mls_api.get_all_topscorers()
 print("All Top Scorers:")
 print(all_topscorers)
 
-# Get top scorers data by ID
-topscorer_id = "the_uuid" # UUID
-specific_topscorer = topscorer.get_topscorer_by_id(topscorer_id)
-print(f"Top Scorer with ID {topscorer_id}:")
-print(specific_topscorer)
-
 # Get all offence data
-all_offences = offence.get_all_offences()
+all_offences = mls_api.get_all_offences()
 print("All Offences:")
 print(all_offences)
 
-# Get offence data by ID
-offence_id = "the_uuid" # UUID
-specific_offence = offence.get_offence_by_id(offence_id)
-print(f"Offence with ID {offence_id}:")
-print(specific_offence)
-
 # Get all assists data
-all_assists = assists.get_all_assists()
+all_assists = mls_api.get_all_assists()
 print("All Assists:")
 print(all_assists)
 
-# Get assists data by ID
-assist_id = "the_uuid" # UUID
-specific_assist = assists.get_assist_by_id(assist_id)
-print(f"Assist with ID {assist_id}:")
-print(specific_assist)
-
 # Get all teams data
-all_teams = teams.get_all_teams()
+all_teams = mls_api.get_all_teams()
 print("All teams:\n", all_teams)
 
-# Get teams data by ID
-team_id = "the_uuid" # UUID
-team = teams.get_team_by_id(team_id)
-print(f"Team with ID {team_id}:\n", team)
-
 # Get all fixtures data
-all_fixtures = fixtures.get_all_fixtures()
+all_fixtures = mls_api.get_all_fixtures()
 print("All fixtures:\n", all_fixtures)
 
-# Get fixtures data by ID
-fixture_id = "the_uuid" # UUID
-fixture = fixtures.get_fixture_by_id(fixture_id)
-print(f"Fixture with ID {fixture_id}:\n", fixture)
-
 # Get all standings data
-all_standings = standings.get_all_standings()
+all_standings = mls_api.get_all_standings()
 print(all_standings)
 
-# Get a specific standing by ID
-standing_id = "the_uuid" # UUID
-specific_standing = standings.get_standing_by_id(standing_id)
-print(specific_standing)
-
 # Get all news data
-all_news = news.get_all_news()
+all_news = mls_api.get_all_news()
 print(all_news)
-
-# Get a specific news item by ID
-news_id = "the_uuid" # UUID
-specific_news = news.get_news_by_id(news_id)
-print(specific_news)
 ```
 
 ## Setting up an MLS API Account
 
 Sign up for a self-service [user account](https://moatsystems.com/mls-api/).
```

### Comparing `mls-api-1.0.7/mls_api/fixtures.py` & `mls-api-1.0.8/mls_api/fixtures.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import os, json
 import requests
-import json
 
 BASE_URL = "https://mlssoccerapi.com/fixtures"
 
+bearerToken = os.getenv('BEARER_TOKEN')
+
 headers = {
-    'Content-Type': 'application/json'
+    'Content-Type': 'application/json',
+    'Authorization': f'Bearer {bearerToken}'
 }
 
 def get_all_fixtures():
     response = requests.get(BASE_URL, headers=headers)
     return response.text
 
 def get_fixture_by_id(fixture_id):
```

### Comparing `mls-api-1.0.7/mls_api/historical.py` & `mls-api-1.0.8/mls_api/news.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,36 @@
+import os, json
 import requests
-import json
 
-def get_all_hist():
-    url = "https://mlssoccerapi.com/hist"
-    payload = {}
-    headers = {'Content-Type': 'application/json'}
-    response = requests.request("GET", url, headers=headers, data=payload)
+BASE_URL = "https://mlssoccerapi.com/news"
+
+bearerToken = os.getenv('BEARER_TOKEN')
+
+headers = {
+    'Content-Type': 'application/json',
+    'Authorization': f'Bearer {bearerToken}'
+}
+
+def get_all_news():
+    response = requests.get(BASE_URL, headers=headers)
     return response.text
 
-def get_hist_by_id(hist_id):
-    url = f"https://mlssoccerapi.com/hist/{hist_id}"
-    payload = {}
-    headers = {'Content-Type': 'application/json'}
-    response = requests.request("GET", url, headers=headers, data=payload)
+def get_news_by_id(news_id):
+    url = f"{BASE_URL}/{news_id}"
+    response = requests.get(url, headers=headers)
     return response.text
 
-def update_hist_by_id(hist_id, data):
-    url = f"https://mlssoccerapi.com/hist/{hist_id}"
+def update_news_by_id(news_id, data):
+    url = f"{BASE_URL}/{news_id}"
     payload = json.dumps(data)
-    headers = {'Content-Type': 'application/json'}
-    response = requests.request("PUT", url, headers=headers, data=payload)
+    response = requests.put(url, headers=headers, data=payload)
     return response.text
 
-def delete_hist_by_id(hist_id):
-    url = f"https://mlssoccerapi.com/hist/{hist_id}"
-    payload = json.dumps({"id": hist_id})
-    headers = {'Content-Type': 'application/json'}
-    response = requests.request("DELETE", url, headers=headers, data=payload)
+def delete_news_by_id(news_id):
+    url = f"{BASE_URL}/{news_id}"
+    response = requests.delete(url, headers=headers)
     return response.text
 
-def add_new_hist(data):
-    url = "https://mlssoccerapi.com/hist"
+def add_new_news(data):
     payload = json.dumps(data)
-    headers = {'Content-Type': 'application/json'}
-    response = requests.request("POST", url, headers=headers, data=payload)
+    response = requests.post(BASE_URL, headers=headers, data=payload)
     return response.text
```

### Comparing `mls-api-1.0.7/mls_api/news.py` & `mls-api-1.0.8/mls_api/teams.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,36 @@
+import os, json
 import requests
-import json
 
-BASE_URL = "https://mlssoccerapi.com/news"
+BASE_URL = "https://mlssoccerapi.com/teams"
+
+bearerToken = os.getenv('BEARER_TOKEN')
 
 headers = {
-  'Content-Type': 'application/json'
+    'Content-Type': 'application/json',
+    'Authorization': f'Bearer {bearerToken}'
 }
 
-def get_all_news():
+def get_all_teams():
     response = requests.get(BASE_URL, headers=headers)
     return response.text
 
-def get_news_by_id(news_id):
-    url = f"{BASE_URL}/{news_id}"
+def get_team_by_id(team_id):
+    url = f"{BASE_URL}/{team_id}"
     response = requests.get(url, headers=headers)
     return response.text
 
-def update_news_by_id(news_id, data):
-    url = f"{BASE_URL}/{news_id}"
+def update_team_by_id(team_id, data):
+    url = f"{BASE_URL}/{team_id}"
     payload = json.dumps(data)
     response = requests.put(url, headers=headers, data=payload)
     return response.text
 
-def delete_news_by_id(news_id):
-    url = f"{BASE_URL}/{news_id}"
+def delete_team_by_id(team_id):
+    url = f"{BASE_URL}/{team_id}"
     response = requests.delete(url, headers=headers)
     return response.text
 
-def add_new_news(data):
+def add_new_team(data):
     payload = json.dumps(data)
     response = requests.post(BASE_URL, headers=headers, data=payload)
     return response.text
```

### Comparing `mls-api-1.0.7/mls_api/offense.py` & `mls-api-1.0.8/mls_api/offense.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,64 @@
+import os, json
 import requests
-import json
 
 def get_all_offence():
+    bearerToken = os.getenv('BEARER_TOKEN')
     url = "https://mlssoccerapi.com/offence"
     payload = {}
-    headers = {'Content-Type': 'application/json'}
+    headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {bearerToken}'}
     response = requests.request("GET", url, headers=headers, data=payload)
     return response.text
 
 
 def get_offence_by_id(offence_id):
+    bearerToken = os.getenv('BEARER_TOKEN')
     url = f"https://mlssoccerapi.com/offence/{offence_id}"
     payload = {}
-    headers = {'Content-Type': 'application/json'}
+    headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {bearerToken}'}
     response = requests.request("GET", url, headers=headers, data=payload)
     return response.text
 
 
 def update_offence_by_id(offence_id, league_name, standing, player_name, team_name, yellow_cards, red_cards, tag):
+    bearerToken = os.getenv('BEARER_TOKEN')
     url = f"https://mlssoccerapi.com/offence/{offence_id}"
     payload = json.dumps({
         "id": offence_id,
         "league_name": league_name,
         "standing": standing,
         "player_name": player_name,
         "team_name": team_name,
         "yellow_cards": yellow_cards,
         "red_cards": red_cards,
         "tag": tag
     })
-    headers = {'Content-Type': 'application/json'}
+    headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {bearerToken}'}
     response = requests.request("PUT", url, headers=headers, data=payload)
     return response.text
 
 
 def delete_offence_by_id(offence_id):
+    bearerToken = os.getenv('BEARER_TOKEN')
     url = f"https://mlssoccerapi.com/offence/{offence_id}"
     payload = json.dumps({"id": offence_id})
-    headers = {'Content-Type': 'application/json'}
+    headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {bearerToken}'}
     response = requests.request("DELETE", url, headers=headers, data=payload)
     return response.text
 
 
 def add_new_offence(offence_id, league_name, standing, player_name, team_name, yellow_cards, red_cards, tag):
+    bearerToken = os.getenv('BEARER_TOKEN')
     url = "https://mlssoccerapi.com/offence"
     payload = json.dumps({
         "id": offence_id,
         "league_name": league_name,
         "standing": standing,
         "player_name": player_name,
         "team_name": team_name,
         "yellow_cards": yellow_cards,
         "red_cards": red_cards,
         "tag": tag
     })
-    headers = {'Content-Type': 'application/json'}
+    headers = {'Content-Type': 'application/json', 'Authorization': f'Bearer {bearerToken}'}
     response = requests.request("POST", url, headers=headers, data=payload)
     return response.text
```

### Comparing `mls-api-1.0.7/mls_api/six.py` & `mls-api-1.0.8/mls_api/six.py`

 * *Files identical despite different names*

### Comparing `mls-api-1.0.7/mls_api.egg-info/PKG-INFO` & `mls-api-1.0.8/mls_api.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mls-api
-Version: 1.0.7
+Version: 1.0.8
 Summary: Python library for integrating with the MLS (Major League Soccer) API.
 Home-page: https://moatsystems.com/mls-api/
 Author: Moat Systems Limited
 Author-email: support@moatsystems.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/moatsystems/mlsapi-python/issues
 Project-URL: Changes, https://github.com/moatsystems/mlsapi-python/blob/main/CHANGELOG.md
@@ -55,111 +55,58 @@
             # Authentication
             username = "your_username"
             password = "your_password"
             response_text = login(username, password)
             print("Login response:", response_text)
         
             # Get all historical data
-            response_text = get_all_hist()
+            response_text = mls_api.get_all_hist()
             print("All historical data response:", response_text)
         
-            # Get historical data by ID
-            hist_id = "the_uuid" # UUID
-            response_text = get_hist_by_id(hist_id)
-            print("Historical data by ID response:", response_text)
-        
             # Get all real-time data (RTD)
-            response_text = get_all_rtd()
+            response_text = mls_api.get_all_rtd()
             print("All real-time data response:", response_text)
         
-            # Get real-time data (RTD) by ID
-            rtd_id = "the_uuid" # UUID
-            response_text = get_rtd_by_id(rtd_id)
-            print("Real-time data by ID response:", response_text)
-        
             # Get a list of players with a custom limit and offset
             limit = 20
             offset = 10
-            response_text = get_all_players(limit, offset)
+            response_text = mls_api.get_all_players(limit, offset)
             print("Players response:", response_text)
         
-            # Get a specific player by ID
-            player_id = "the_uuid" # UUID
-            response_text = get_player_by_id(player_id)
-            print("Player by ID response:", response_text)
-        
             # Get all top scorers data
-            all_topscorers = topscorer.get_all_topscorers()
+            all_topscorers = mls_api.get_all_topscorers()
             print("All Top Scorers:")
             print(all_topscorers)
         
-            # Get top scorers data by ID
-            topscorer_id = "the_uuid" # UUID
-            specific_topscorer = topscorer.get_topscorer_by_id(topscorer_id)
-            print(f"Top Scorer with ID {topscorer_id}:")
-            print(specific_topscorer)
-        
             # Get all offence data
-            all_offences = offence.get_all_offences()
+            all_offences = mls_api.get_all_offences()
             print("All Offences:")
             print(all_offences)
         
-            # Get offence data by ID
-            offence_id = "the_uuid" # UUID
-            specific_offence = offence.get_offence_by_id(offence_id)
-            print(f"Offence with ID {offence_id}:")
-            print(specific_offence)
-        
             # Get all assists data
-            all_assists = assists.get_all_assists()
+            all_assists = mls_api.get_all_assists()
             print("All Assists:")
             print(all_assists)
         
-            # Get assists data by ID
-            assist_id = "the_uuid" # UUID
-            specific_assist = assists.get_assist_by_id(assist_id)
-            print(f"Assist with ID {assist_id}:")
-            print(specific_assist)
-        
             # Get all teams data
-            all_teams = teams.get_all_teams()
+            all_teams = mls_api.get_all_teams()
             print("All teams:\n", all_teams)
         
-            # Get teams data by ID
-            team_id = "the_uuid" # UUID
-            team = teams.get_team_by_id(team_id)
-            print(f"Team with ID {team_id}:\n", team)
-        
             # Get all fixtures data
-            all_fixtures = fixtures.get_all_fixtures()
+            all_fixtures = mls_api.get_all_fixtures()
             print("All fixtures:\n", all_fixtures)
         
-            # Get fixtures data by ID
-            fixture_id = "the_uuid" # UUID
-            fixture = fixtures.get_fixture_by_id(fixture_id)
-            print(f"Fixture with ID {fixture_id}:\n", fixture)
-        
             # Get all standings data
-            all_standings = standings.get_all_standings()
+            all_standings = mls_api.get_all_standings()
             print(all_standings)
         
-            # Get a specific standing by ID
-            standing_id = "the_uuid" # UUID
-            specific_standing = standings.get_standing_by_id(standing_id)
-            print(specific_standing)
-        
             # Get all news data
-            all_news = news.get_all_news()
+            all_news = mls_api.get_all_news()
             print(all_news)
         
-            # Get a specific news item by ID
-            news_id = "the_uuid" # UUID
-            specific_news = news.get_news_by_id(news_id)
-            print(specific_news)
-        
         
         Setting up an MLS API Account
         -----------------------------
         
         Sign up for a self-service `user account`_.
         
         .. _user account: https://moatsystems.com/mls-api/
```

### Comparing `mls-api-1.0.7/setup.py` & `mls-api-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages  # noqa: H301
 from distutils.core import Extension
 
 NAME = "mls-api"
-VERSION = "1.0.7"
+VERSION = "1.0.8"
 REQUIRES = ["requests"]
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'LONG_DESCRIPTION.rst')) as f:
     long_description = f.read()
```

