# Comparing `tmp/revChatGPT-4.2.2.tar.gz` & `tmp/revChatGPT-4.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-4.2.2.tar", last modified: Sat Apr 15 14:30:15 2023, max compression
+gzip compressed data, was "revChatGPT-4.2.3.tar", last modified: Sun Apr 16 15:13:25 2023, max compression
```

## Comparing `revChatGPT-4.2.2.tar` & `revChatGPT-4.2.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:30:15.696614 revChatGPT-4.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-15 14:29:46.000000 revChatGPT-4.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-04-15 14:30:15.696614 revChatGPT-4.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-04-15 14:30:15.000000 revChatGPT-4.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-15 14:30:15.696614 revChatGPT-4.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-15 14:29:46.000000 revChatGPT-4.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:30:15.692614 revChatGPT-4.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:30:15.696614 revChatGPT-4.2.2/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    47274 2023-04-15 14:29:46.000000 revChatGPT-4.2.2/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23198 2023-04-15 14:29:46.000000 revChatGPT-4.2.2/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-15 14:29:46.000000 revChatGPT-4.2.2/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-15 14:29:46.000000 revChatGPT-4.2.2/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:30:15.696614 revChatGPT-4.2.2/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-15 14:29:46.000000 revChatGPT-4.2.2/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-15 14:29:46.000000 revChatGPT-4.2.2/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-15 14:29:46.000000 revChatGPT-4.2.2/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 14:30:15.696614 revChatGPT-4.2.2/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-04-15 14:30:15.000000 revChatGPT-4.2.2/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-15 14:30:15.000000 revChatGPT-4.2.2/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 14:30:15.000000 revChatGPT-4.2.2/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-15 14:30:15.000000 revChatGPT-4.2.2/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-15 14:30:15.000000 revChatGPT-4.2.2/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:13:25.220344 revChatGPT-4.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-16 15:12:53.000000 revChatGPT-4.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-04-16 15:13:25.220344 revChatGPT-4.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-04-16 15:13:25.000000 revChatGPT-4.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-16 15:13:25.224344 revChatGPT-4.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-16 15:12:53.000000 revChatGPT-4.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:13:25.220344 revChatGPT-4.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:13:25.220344 revChatGPT-4.2.3/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    47267 2023-04-16 15:12:53.000000 revChatGPT-4.2.3/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23198 2023-04-16 15:12:53.000000 revChatGPT-4.2.3/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-16 15:12:53.000000 revChatGPT-4.2.3/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-04-16 15:12:53.000000 revChatGPT-4.2.3/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:13:25.220344 revChatGPT-4.2.3/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-16 15:12:53.000000 revChatGPT-4.2.3/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-04-16 15:12:53.000000 revChatGPT-4.2.3/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-16 15:12:53.000000 revChatGPT-4.2.3/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:13:25.220344 revChatGPT-4.2.3/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-04-16 15:13:25.000000 revChatGPT-4.2.3/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-16 15:13:25.000000 revChatGPT-4.2.3/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 15:13:25.000000 revChatGPT-4.2.3/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-16 15:13:25.000000 revChatGPT-4.2.3/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-16 15:13:25.000000 revChatGPT-4.2.3/src/revChatGPT.egg-info/top_level.txt
```

### Comparing `revChatGPT-4.2.2/LICENSE` & `revChatGPT-4.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.2/PKG-INFO` & `revChatGPT-4.2.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 4.2.2
+Version: 4.2.3
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -46,22 +46,20 @@
 
 ### Suport Python Version
 
 - Minimum - Python3.9
 - Recommend - Python3.11+
 
 <details>
-
-<summary>
+  
+  <summary>
 
 # V1 Standard ChatGPT
 
-This uses a reversed `chat.openai.com`'s API with a [cloudflare bypass server](https://github.com/acheong08/ChatGPT-Proxy-V4) to make programmatic ChatGPT usage free. This specific library is meant for personal use due to severe rate limits on OpenAI's side. It has not been optimized for use with mutliple accounts.
-
-You can check out [this project](https://github.com/acheong08/ChatGPT-to-API) for well supported multi account cycling. It is compatible with the official API. Use [OpenAI's documentation](https://platform.openai.com/docs/guides/chat) as reference on usage. It carries conversations between accounts to ensure rate limits are not hit given a high number of accounts.
+Due to recent tightening of OpenAI's security, the default endpoint has been swapped over to one provided by @pengzhile. It is not open source and privacy is not guarenteed. Use it at your own risk. I am working on an open source implementation with the latest changes but that could take a while.
 
 </summary>
 
 ## Rate limits
 - Proxy server: 5 requests / 10 seconds
 - OpenAI: 50 requests / hour for each account
 
@@ -72,26 +70,24 @@
 
 ### Authentication method: (Choose 1)
 
 #### - Email/Password
 
 > _Currently broken for free users. Do `export PUID="..."` if you have a plus account. The PUID is a cookie named `_puid`_
 > Not supported for Google/Microsoft accounts.
-
 ```json
 {
   "email": "email",
   "password": "your password"
 }
 ```
 
 #### - Access token
 
 > Please this!
-
 https://chat.openai.com/api/auth/session
 
 ```json
 {
   "access_token": "<access_token>"
 }
 ```
@@ -119,38 +115,33 @@
 ### Command line
 
 `python3 -m revChatGPT.V1`
 
 ```
         ChatGPT - A command-line interface to OpenAI's ChatGPT (https://chat.openai.com/chat)
         Repo: github.com/acheong08/ChatGPT
-
 Type '!help' to show a full list of commands
-
 Logging in...
-
 You:
 (Press Esc followed by Enter to finish)
 ```
 
 The command line interface supports multi-line inputs and allows navigation using arrow keys. Besides, you can also edit history inputs by arrow keys when the prompt is empty. It also completes your input if it finds matched previous prompts. To finish input, press `Esc` and then `Enter` as solely `Enter` itself is used for creating new line in multi-line mode.
 
 Set the environment variable `NO_COLOR` to `true` to disable color output.
 
 ### Developer API
 
 #### Basic example (streamed):
 
 ```python
 from revChatGPT.V1 import Chatbot
-
 chatbot = Chatbot(config={
   "access_token": "<your access_token>"
 })
-
 print("Chatbot: ")
 prev_text = ""
 for data in chatbot.ask(
     "Hello world",
 ):
     message = data["message"][len(prev_text) :]
     print(message, end="", flush=True)
@@ -158,39 +149,33 @@
 print()
 ```
 
 #### Basic example (single result):
 
 ```python
 from revChatGPT.V1 import Chatbot
-
 chatbot = Chatbot(config={
   "access_token": "<your access_token>"
 })
-
 prompt = "how many beaches does portugal have?"
 response = ""
-
 for data in chatbot.ask(
   prompt
 ):
     response = data["message"]
-
 print(response)
 ```
 
 #### All API methods
 
 Refer to the [wiki](https://github.com/acheong08/ChatGPT/wiki/) for advanced developer usage.
 
 </details>
 
-<details>
-
-<summary>
+<summary>  
 
 # V3 Official Chat API
 
 > Recently released by OpenAI
 >
 > - Paid
```

### Comparing `revChatGPT-4.2.2/README.md` & `revChatGPT-4.2.3/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: revChatGPT
+Version: 4.2.3
+Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
+Home-page: https://github.com/acheong08/ChatGPT
+Author: Antonio Cheong
+Author-email: acheong@student.dalat.org
+License: GNU General Public License v2.0
+Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
+Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Natural Language :: English
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ChatGPT <img src="https://github.com/acheong08/ChatGPT/blob/main/logo.png?raw=true" width="15%"></img>
 
 English - [中文](./README_zh.md)
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
@@ -24,22 +46,20 @@
 
 ### Suport Python Version
 
 - Minimum - Python3.9
 - Recommend - Python3.11+
 
 <details>
-
-<summary>
+  
+  <summary>
 
 # V1 Standard ChatGPT
 
-This uses a reversed `chat.openai.com`'s API with a [cloudflare bypass server](https://github.com/acheong08/ChatGPT-Proxy-V4) to make programmatic ChatGPT usage free. This specific library is meant for personal use due to severe rate limits on OpenAI's side. It has not been optimized for use with mutliple accounts.
-
-You can check out [this project](https://github.com/acheong08/ChatGPT-to-API) for well supported multi account cycling. It is compatible with the official API. Use [OpenAI's documentation](https://platform.openai.com/docs/guides/chat) as reference on usage. It carries conversations between accounts to ensure rate limits are not hit given a high number of accounts.
+Due to recent tightening of OpenAI's security, the default endpoint has been swapped over to one provided by @pengzhile. It is not open source and privacy is not guarenteed. Use it at your own risk. I am working on an open source implementation with the latest changes but that could take a while.
 
 </summary>
 
 ## Rate limits
 - Proxy server: 5 requests / 10 seconds
 - OpenAI: 50 requests / hour for each account
 
@@ -50,26 +70,24 @@
 
 ### Authentication method: (Choose 1)
 
 #### - Email/Password
 
 > _Currently broken for free users. Do `export PUID="..."` if you have a plus account. The PUID is a cookie named `_puid`_
 > Not supported for Google/Microsoft accounts.
-
 ```json
 {
   "email": "email",
   "password": "your password"
 }
 ```
 
 #### - Access token
 
 > Please this!
-
 https://chat.openai.com/api/auth/session
 
 ```json
 {
   "access_token": "<access_token>"
 }
 ```
@@ -97,38 +115,33 @@
 ### Command line
 
 `python3 -m revChatGPT.V1`
 
 ```
         ChatGPT - A command-line interface to OpenAI's ChatGPT (https://chat.openai.com/chat)
         Repo: github.com/acheong08/ChatGPT
-
 Type '!help' to show a full list of commands
-
 Logging in...
-
 You:
 (Press Esc followed by Enter to finish)
 ```
 
 The command line interface supports multi-line inputs and allows navigation using arrow keys. Besides, you can also edit history inputs by arrow keys when the prompt is empty. It also completes your input if it finds matched previous prompts. To finish input, press `Esc` and then `Enter` as solely `Enter` itself is used for creating new line in multi-line mode.
 
 Set the environment variable `NO_COLOR` to `true` to disable color output.
 
 ### Developer API
 
 #### Basic example (streamed):
 
 ```python
 from revChatGPT.V1 import Chatbot
-
 chatbot = Chatbot(config={
   "access_token": "<your access_token>"
 })
-
 print("Chatbot: ")
 prev_text = ""
 for data in chatbot.ask(
     "Hello world",
 ):
     message = data["message"][len(prev_text) :]
     print(message, end="", flush=True)
@@ -136,39 +149,33 @@
 print()
 ```
 
 #### Basic example (single result):
 
 ```python
 from revChatGPT.V1 import Chatbot
-
 chatbot = Chatbot(config={
   "access_token": "<your access_token>"
 })
-
 prompt = "how many beaches does portugal have?"
 response = ""
-
 for data in chatbot.ask(
   prompt
 ):
     response = data["message"]
-
 print(response)
 ```
 
 #### All API methods
 
 Refer to the [wiki](https://github.com/acheong08/ChatGPT/wiki/) for advanced developer usage.
 
 </details>
 
-<details>
-
-<summary>
+<summary>  
 
 # V3 Official Chat API
 
 > Recently released by OpenAI
 >
 > - Paid
```

### Comparing `revChatGPT-4.2.2/setup.py` & `revChatGPT-4.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="4.2.2",
+    version="4.2.3",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-4.2.2/src/revChatGPT/V1.py` & `revChatGPT-4.2.3/src/revChatGPT/V1.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             return out
 
         return wrapper
 
     return decorator
 
 
-BASE_URL = environ.get("CHATGPT_BASE_URL") or "https://bypass.churchless.tech/api/"
+BASE_URL = environ.get("CHATGPT_BASE_URL") or "https://chat.gateway.do/api/"
 
 bcolors = t.colors()
 
 
 class Chatbot:
     """
     Chatbot class for ChatGPT
```

### Comparing `revChatGPT-4.2.2/src/revChatGPT/V3.py` & `revChatGPT-4.2.3/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.2/src/revChatGPT/__init__.py` & `revChatGPT-4.2.3/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.2/src/revChatGPT/__main__.py` & `revChatGPT-4.2.3/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.2/src/revChatGPT/config/enable_internet.json` & `revChatGPT-4.2.3/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.2/src/revChatGPT/typings.py` & `revChatGPT-4.2.3/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.2/src/revChatGPT/utils.py` & `revChatGPT-4.2.3/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-4.2.2/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-4.2.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: revChatGPT
-Version: 4.2.2
-Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
-Home-page: https://github.com/acheong08/ChatGPT
-Author: Antonio Cheong
-Author-email: acheong@student.dalat.org
-License: GNU General Public License v2.0
-Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
-Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Natural Language :: English
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ChatGPT <img src="https://github.com/acheong08/ChatGPT/blob/main/logo.png?raw=true" width="15%"></img>
 
 English - [中文](./README_zh.md)
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
@@ -46,22 +24,20 @@
 
 ### Suport Python Version
 
 - Minimum - Python3.9
 - Recommend - Python3.11+
 
 <details>
-
-<summary>
+  
+  <summary>
 
 # V1 Standard ChatGPT
 
-This uses a reversed `chat.openai.com`'s API with a [cloudflare bypass server](https://github.com/acheong08/ChatGPT-Proxy-V4) to make programmatic ChatGPT usage free. This specific library is meant for personal use due to severe rate limits on OpenAI's side. It has not been optimized for use with mutliple accounts.
-
-You can check out [this project](https://github.com/acheong08/ChatGPT-to-API) for well supported multi account cycling. It is compatible with the official API. Use [OpenAI's documentation](https://platform.openai.com/docs/guides/chat) as reference on usage. It carries conversations between accounts to ensure rate limits are not hit given a high number of accounts.
+Due to recent tightening of OpenAI's security, the default endpoint has been swapped over to one provided by @pengzhile. It is not open source and privacy is not guarenteed. Use it at your own risk. I am working on an open source implementation with the latest changes but that could take a while.
 
 </summary>
 
 ## Rate limits
 - Proxy server: 5 requests / 10 seconds
 - OpenAI: 50 requests / hour for each account
 
@@ -72,26 +48,24 @@
 
 ### Authentication method: (Choose 1)
 
 #### - Email/Password
 
 > _Currently broken for free users. Do `export PUID="..."` if you have a plus account. The PUID is a cookie named `_puid`_
 > Not supported for Google/Microsoft accounts.
-
 ```json
 {
   "email": "email",
   "password": "your password"
 }
 ```
 
 #### - Access token
 
 > Please this!
-
 https://chat.openai.com/api/auth/session
 
 ```json
 {
   "access_token": "<access_token>"
 }
 ```
@@ -119,38 +93,33 @@
 ### Command line
 
 `python3 -m revChatGPT.V1`
 
 ```
         ChatGPT - A command-line interface to OpenAI's ChatGPT (https://chat.openai.com/chat)
         Repo: github.com/acheong08/ChatGPT
-
 Type '!help' to show a full list of commands
-
 Logging in...
-
 You:
 (Press Esc followed by Enter to finish)
 ```
 
 The command line interface supports multi-line inputs and allows navigation using arrow keys. Besides, you can also edit history inputs by arrow keys when the prompt is empty. It also completes your input if it finds matched previous prompts. To finish input, press `Esc` and then `Enter` as solely `Enter` itself is used for creating new line in multi-line mode.
 
 Set the environment variable `NO_COLOR` to `true` to disable color output.
 
 ### Developer API
 
 #### Basic example (streamed):
 
 ```python
 from revChatGPT.V1 import Chatbot
-
 chatbot = Chatbot(config={
   "access_token": "<your access_token>"
 })
-
 print("Chatbot: ")
 prev_text = ""
 for data in chatbot.ask(
     "Hello world",
 ):
     message = data["message"][len(prev_text) :]
     print(message, end="", flush=True)
@@ -158,39 +127,33 @@
 print()
 ```
 
 #### Basic example (single result):
 
 ```python
 from revChatGPT.V1 import Chatbot
-
 chatbot = Chatbot(config={
   "access_token": "<your access_token>"
 })
-
 prompt = "how many beaches does portugal have?"
 response = ""
-
 for data in chatbot.ask(
   prompt
 ):
     response = data["message"]
-
 print(response)
 ```
 
 #### All API methods
 
 Refer to the [wiki](https://github.com/acheong08/ChatGPT/wiki/) for advanced developer usage.
 
 </details>
 
-<details>
-
-<summary>
+<summary>  
 
 # V3 Official Chat API
 
 > Recently released by OpenAI
 >
 > - Paid
```

