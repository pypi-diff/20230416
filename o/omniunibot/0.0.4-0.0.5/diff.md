# Comparing `tmp/omniunibot-0.0.4.tar.gz` & `tmp/omniunibot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniunibot-0.0.4.tar", last modified: Mon Mar 27 08:26:52 2023, max compression
+gzip compressed data, was "omniunibot-0.0.5.tar", last modified: Sun Apr 16 09:13:31 2023, max compression
```

## Comparing `omniunibot-0.0.4.tar` & `omniunibot-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 08:26:52.791409 omniunibot-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-27 08:26:40.000000 omniunibot-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-03-27 08:26:52.791409 omniunibot-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-03-27 08:26:40.000000 omniunibot-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 08:26:52.787409 omniunibot-0.0.4/omniunibot/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-27 08:26:40.000000 omniunibot-0.0.4/omniunibot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-27 08:26:40.000000 omniunibot-0.0.4/omniunibot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-27 08:26:40.000000 omniunibot-0.0.4/omniunibot/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-03-27 08:26:40.000000 omniunibot-0.0.4/omniunibot/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-03-27 08:26:40.000000 omniunibot-0.0.4/omniunibot/server.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 08:26:40.000000 omniunibot-0.0.4/omniunibot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 08:26:52.791409 omniunibot-0.0.4/omniunibot/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 08:26:40.000000 omniunibot-0.0.4/omniunibot/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-27 08:26:40.000000 omniunibot-0.0.4/omniunibot/wrapper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-03-27 08:26:40.000000 omniunibot-0.0.4/omniunibot/wrapper/dingtalk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-03-27 08:26:40.000000 omniunibot-0.0.4/omniunibot/wrapper/feishu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-03-27 08:26:40.000000 omniunibot-0.0.4/omniunibot/wrapper/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-03-27 08:26:40.000000 omniunibot-0.0.4/omniunibot/wrapper/wecom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 08:26:52.791409 omniunibot-0.0.4/omniunibot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-03-27 08:26:52.000000 omniunibot-0.0.4/omniunibot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-27 08:26:52.000000 omniunibot-0.0.4/omniunibot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 08:26:52.000000 omniunibot-0.0.4/omniunibot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 08:26:52.000000 omniunibot-0.0.4/omniunibot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-27 08:26:52.000000 omniunibot-0.0.4/omniunibot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-27 08:26:52.000000 omniunibot-0.0.4/omniunibot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 08:26:52.795409 omniunibot-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-03-27 08:26:40.000000 omniunibot-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:13:31.303208 omniunibot-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-16 09:13:19.000000 omniunibot-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-16 09:13:31.303208 omniunibot-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-04-16 09:13:19.000000 omniunibot-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:13:31.303208 omniunibot-0.0.5/omniunibot/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:13:31.303208 omniunibot-0.0.5/omniunibot/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/wrapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/wrapper/dingtalk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/wrapper/feishu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/wrapper/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/wrapper/wecom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:13:31.303208 omniunibot-0.0.5/omniunibot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-16 09:13:31.000000 omniunibot-0.0.5/omniunibot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-16 09:13:31.000000 omniunibot-0.0.5/omniunibot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 09:13:31.000000 omniunibot-0.0.5/omniunibot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 09:13:31.000000 omniunibot-0.0.5/omniunibot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-16 09:13:31.000000 omniunibot-0.0.5/omniunibot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-16 09:13:31.000000 omniunibot-0.0.5/omniunibot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 09:13:31.303208 omniunibot-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-16 09:13:19.000000 omniunibot-0.0.5/setup.py
```

### Comparing `omniunibot-0.0.4/LICENSE` & `omniunibot-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.4/PKG-INFO` & `omniunibot-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniunibot
-Version: 0.0.4
+Version: 0.0.5
 Summary: A universal multiplatform message bot
 Home-page: https://github.com/yttty/omniunibot
 Author: yttty
 Author-email: yttty@noreply.com
 License: MIT
 Keywords: bots
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `omniunibot-0.0.4/README.md` & `omniunibot-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.4/omniunibot/__main__.py` & `omniunibot-0.0.5/omniunibot/__main__.py`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.4/omniunibot/client.py` & `omniunibot-0.0.5/omniunibot/client.py`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.4/omniunibot/server.py` & `omniunibot-0.0.5/omniunibot/server.py`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.4/omniunibot/wrapper/base.py` & `omniunibot-0.0.5/omniunibot/wrapper/base.py`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.4/omniunibot/wrapper/dingtalk.py` & `omniunibot-0.0.5/omniunibot/wrapper/dingtalk.py`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.4/omniunibot/wrapper/feishu.py` & `omniunibot-0.0.5/omniunibot/wrapper/feishu.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import base64
 import time
 import hashlib
 import hmac
 import requests
 import traceback
 from loguru import logger
+from typing import List, Optional
 
 from .base import BaseBot
 
 
 class FeishuBot(BaseBot):
     """
     https://open.feishu.cn/document/ukTMukTMukTM/ucTM5YjL3ETO24yNxkjN
@@ -46,23 +47,46 @@
         )
         return response['code']
 
     def _onSuccessResponse(self, response=None) -> int:
         logger.info("Successully sent message to Feishu.")
         return 0
 
-    def generatePayload(self, text: str):
+    def generatePayload(self,
+                        text: str,
+                        title: Optional[str] = None):
+        """Generate payload to send, using message type `post`, see the document for details
+
+        Args:
+            text (str): _description_
+            title (Optional[str], optional): _description_. Defaults to None.
+            at_uid (Optional[List[str]], optional): uids to at. Defaults to None.
+        """
         timestamp, sign = self._sign()
+        post_zh_cn = {
+            "content": [
+                [
+                    {
+                        "tag": "text",
+                        "text": text
+                    }
+                ]
+            ]
+        }
+        if title:
+            post_zh_cn["title"] = title
         payload = {
             "timestamp": timestamp,
             "sign": sign,
-            "msg_type": "text",
+            "msg_type": "post",
             "content": {
-                "text": text
-            },
+                "post": {
+                        "zh_cn": post_zh_cn
+                }
+            }
         }
         return payload
 
     def sendQuickMessage(self, msg: str):
         logger.info(f"Get text message: {msg}")
         try:
             r = requests.post(self.webhook,
```

### Comparing `omniunibot-0.0.4/omniunibot/wrapper/slack.py` & `omniunibot-0.0.5/omniunibot/wrapper/slack.py`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.4/omniunibot/wrapper/wecom.py` & `omniunibot-0.0.5/omniunibot/wrapper/wecom.py`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.4/omniunibot.egg-info/PKG-INFO` & `omniunibot-0.0.5/omniunibot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniunibot
-Version: 0.0.4
+Version: 0.0.5
 Summary: A universal multiplatform message bot
 Home-page: https://github.com/yttty/omniunibot
 Author: yttty
 Author-email: yttty@noreply.com
 License: MIT
 Keywords: bots
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `omniunibot-0.0.4/omniunibot.egg-info/SOURCES.txt` & `omniunibot-0.0.5/omniunibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.4/setup.py` & `omniunibot-0.0.5/setup.py`

 * *Files identical despite different names*

