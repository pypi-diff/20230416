# Comparing `tmp/bot_lens-0.0.3.tar.gz` & `tmp/bot_lens-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bot_lens-0.0.3.tar", last modified: Sun Apr 16 05:20:31 2023, max compression
+gzip compressed data, was "bot_lens-0.0.4.tar", last modified: Sun Apr 16 05:50:29 2023, max compression
```

## Comparing `bot_lens-0.0.3.tar` & `bot_lens-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-04-16 05:20:31.628864 bot_lens-0.0.3/
--rw-r--r--   0 tim        (501) staff       (20)     1075 2023-04-15 20:07:48.000000 bot_lens-0.0.3/LICENSE
--rw-r--r--   0 tim        (501) staff       (20)      431 2023-04-16 05:20:31.628908 bot_lens-0.0.3/PKG-INFO
--rw-r--r--   0 tim        (501) staff       (20)        0 2023-04-15 20:07:56.000000 bot_lens-0.0.3/README.md
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-04-16 05:20:31.628291 bot_lens-0.0.3/bot_lens/
--rw-r--r--   0 tim        (501) staff       (20)     2235 2023-04-16 05:19:01.000000 bot_lens-0.0.3/bot_lens/Tracker.py
--rw-r--r--   0 tim        (501) staff       (20)        0 2023-04-15 20:02:20.000000 bot_lens-0.0.3/bot_lens/__init__.py
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-04-16 05:20:31.628668 bot_lens-0.0.3/bot_lens.egg-info/
--rw-r--r--   0 tim        (501) staff       (20)      431 2023-04-16 05:20:31.000000 bot_lens-0.0.3/bot_lens.egg-info/PKG-INFO
--rw-r--r--   0 tim        (501) staff       (20)      224 2023-04-16 05:20:31.000000 bot_lens-0.0.3/bot_lens.egg-info/SOURCES.txt
--rw-r--r--   0 tim        (501) staff       (20)        1 2023-04-16 05:20:31.000000 bot_lens-0.0.3/bot_lens.egg-info/dependency_links.txt
--rw-r--r--   0 tim        (501) staff       (20)        9 2023-04-16 05:20:31.000000 bot_lens-0.0.3/bot_lens.egg-info/top_level.txt
--rw-r--r--   0 tim        (501) staff       (20)      135 2023-04-16 04:35:33.000000 bot_lens-0.0.3/pyproject.toml
--rw-r--r--   0 tim        (501) staff       (20)      521 2023-04-16 05:20:31.629094 bot_lens-0.0.3/setup.cfg
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-04-16 05:20:31.628770 bot_lens-0.0.3/test/
--rw-r--r--   0 tim        (501) staff       (20)     1393 2023-04-16 04:31:01.000000 bot_lens-0.0.3/test/test.py
+drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-04-16 05:50:29.838722 bot_lens-0.0.4/
+-rw-r--r--   0 tim        (501) staff       (20)     1075 2023-04-15 20:07:48.000000 bot_lens-0.0.4/LICENSE
+-rw-r--r--   0 tim        (501) staff       (20)      431 2023-04-16 05:50:29.838765 bot_lens-0.0.4/PKG-INFO
+-rw-r--r--   0 tim        (501) staff       (20)        0 2023-04-15 20:07:56.000000 bot_lens-0.0.4/README.md
+drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-04-16 05:50:29.838126 bot_lens-0.0.4/bot_lens/
+-rw-r--r--   0 tim        (501) staff       (20)     2340 2023-04-16 05:49:23.000000 bot_lens-0.0.4/bot_lens/Tracker.py
+-rw-r--r--   0 tim        (501) staff       (20)        0 2023-04-15 20:02:20.000000 bot_lens-0.0.4/bot_lens/__init__.py
+drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-04-16 05:50:29.838518 bot_lens-0.0.4/bot_lens.egg-info/
+-rw-r--r--   0 tim        (501) staff       (20)      431 2023-04-16 05:50:29.000000 bot_lens-0.0.4/bot_lens.egg-info/PKG-INFO
+-rw-r--r--   0 tim        (501) staff       (20)      224 2023-04-16 05:50:29.000000 bot_lens-0.0.4/bot_lens.egg-info/SOURCES.txt
+-rw-r--r--   0 tim        (501) staff       (20)        1 2023-04-16 05:50:29.000000 bot_lens-0.0.4/bot_lens.egg-info/dependency_links.txt
+-rw-r--r--   0 tim        (501) staff       (20)        9 2023-04-16 05:50:29.000000 bot_lens-0.0.4/bot_lens.egg-info/top_level.txt
+-rw-r--r--   0 tim        (501) staff       (20)      152 2023-04-16 05:49:57.000000 bot_lens-0.0.4/pyproject.toml
+-rw-r--r--   0 tim        (501) staff       (20)      521 2023-04-16 05:50:29.838949 bot_lens-0.0.4/setup.cfg
+drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-04-16 05:50:29.838617 bot_lens-0.0.4/test/
+-rw-r--r--   0 tim        (501) staff       (20)     1389 2023-04-16 05:37:15.000000 bot_lens-0.0.4/test/test.py
```

### Comparing `bot_lens-0.0.3/LICENSE` & `bot_lens-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bot_lens-0.0.3/bot_lens/Tracker.py` & `bot_lens-0.0.4/bot_lens/Tracker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import random
 import json
 import time
 import requests
 from fastapi import FastAPI, Header
-from user_agents import parse
+from termcolor import colored
 
 class Tracker:
 	DEFAULT_HOST = '34.221.241.220'
+	DEFAULT_DEBUG=True
     
-	def __init__(self, token, host=DEFAULT_HOST):  
+	def __init__(self, token, host=DEFAULT_HOST, debug=DEFAULT_DEBUG):  
 		self.token = token
 		self.host = host
+		self.debug = debug
 		print(f"token is {self.token} host is {host}")
 	
 	
 	"""
 	Headers({'host': 'chatgpt-lugin.timtully1.repl.co', 
  'user-agent': 'Python/3.9 aiohttp/3.8.4', 'accept': '*/*', 
  'accept-encoding': 'gzip, deflate', 'accept-language': 
@@ -36,39 +38,37 @@
 		ts = int(time.time()) 
 		openai_conv_id = http_header['openai-conversation-id']
 		openai_ephemeral_id = http_header['openai-ephemeral-user-id']
 		ip = http_header['x-forwarded-for']
 		ddog_parent = http_header['x-datadog-parent-id']
 		plugin_hostname = http_header['host']
 		iso_code = http_header['openai-subdivision-1-iso-code']
-		ua = parse(http_header['user-agent'])
 
 		payload = [
 				{
 					"event_time":ts,
 					"developer_id":self.token,
 					"user_id":openai_conv_id,
 					"user_name":username,
      				"event_name":event_name,
 					"ip_address":ip,
 					"unique_conversation_id":openai_conv_id,
      				"ephemeral_user_id":openai_ephemeral_id,
          			"plugin_hostname":plugin_hostname,
-					"os_version":ua.os.version,
-					"os":ua.os,
+					"os_version":1.2,
+					"os":"mac",
 					"subdivision-1-iso-code":iso_code,
      				"datadog-parent-id":ddog_parent,
-					"chatgpt_id":"1.2.3.4"
+					"chatgpt_ip":"1.2.3.4"
 				}
 		]
 		
-		print(f"payload is {payload}")
 		uri = f"http://{self.host}/log_events"
-		print(uri)
 		r = requests.post(url = uri, json=payload)
-		print(r.text)
-		pass
-
+		if self.debug:
+			print(f"bot-lens endpt: {uri}")
+			print(f"payload is {payload}")
+			print(colored(f"{r.status_code} Response:{r.text}", 'black', 'on_green'))
```

### Comparing `bot_lens-0.0.3/setup.cfg` & `bot_lens-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bot_lens
-version = 0.0.3
+version = 0.0.4
 author = bot_lens
 author_email = timtully24@gmail.com
 description = API for tracking dat in ChatGPT plugins
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nicrso/bot-lens/
 classifiers =
```

### Comparing `bot_lens-0.0.3/test/test.py` & `bot_lens-0.0.4/test/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 
 from bot_lens.Tracker import Tracker
 
 #t = Tracker("asdfadsf", "localhost:3000")
 t = Tracker("asdfadsf")
-t.log_event("tim test", "tim", {'host': 'chatgpt-lugin.timtully1.repl.co', 'user-agent': 'Python/3.9 aiohttp/3.8.4', 'accept': '*/*', 'accept-encoding': 'gzip, deflate', 'accept-language': 'en-US,en;q=0.9', 'content-type': 'application/json', 'openai-conversation-id': '679569e4-b3e6-52d6-be2d-0328761f6322', 'openai-ephemeral-user-id': '6599caa6-01e3-51e7-9e3b-e968cac26ef6', 'openai-subdivision-1-iso-code': 'US-CA', 'traceparent': '00-00000000000000004912ceeb977bc42b-8633e24135d6067e-01', 'tracestate': 'dd=s:1;t.dm:-1', 'x-datadog-parent-id': '9670321594598557310', 'x-datadog-sampling-priority': '1', 'x-datadog-tags': '_dd.p.dm=-1', 'x-datadog-trace-id': '5265498425603638315', 'x-forwarded-for': '23.102.140.113', 'x-forwarded-proto': 'https', 'x-replit-user-bio': '', 'x-replit-user-id': '', 'x-replit-user-name': '', 'x-replit-user-profile-image': '', 'x-replit-user-roles': '', 'x-replit-user-teams': '', 'x-replit-user-url': ''})
-
-
+t.log_event("coffee", "tim", {'host': 'chatgpt-lugin.timtully1.repl.co', 'user-agent': 'Python/3.9 aiohttp/3.8.4', 'accept': '*/*', 'accept-encoding': 'gzip, deflate', 'accept-language': 'en-US,en;q=0.9', 'content-type': 'application/json', 'openai-conversation-id': '679569e4-b3e6-52d6-be2d-0328761f6322', 'openai-ephemeral-user-id': '6599caa6-01e3-51e7-9e3b-e968cac26ef6', 'openai-subdivision-1-iso-code': 'US-CA', 'traceparent': '00-00000000000000004912ceeb977bc42b-8633e24135d6067e-01', 'tracestate': 'dd=s:1;t.dm:-1', 'x-datadog-parent-id': '9670321594598557310', 'x-datadog-sampling-priority': '1', 'x-datadog-tags': '_dd.p.dm=-1', 'x-datadog-trace-id': '5265498425603638315', 'x-forwarded-for': '23.102.140.113', 'x-forwarded-proto': 'https', 'x-replit-user-bio': '', 'x-replit-user-id': '', 'x-replit-user-name': '', 'x-replit-user-profile-image': '', 'x-replit-user-roles': '', 'x-replit-user-teams': '', 'x-replit-user-url': ''})
 
 """
 		-  `event_time: timestamp`
 		- `developer_id: str`
 		- `user_id: str`
 		- `event_name: str`
 		- `ip_address: str`
```

