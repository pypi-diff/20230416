# Comparing `tmp/nonebot_adapter_kaiheila-0.2.5.tar.gz` & `tmp/nonebot_adapter_kaiheila-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_kaiheila-0.2.5.tar", max compression
+gzip compressed data, was "nonebot_adapter_kaiheila-0.2.6.tar", max compression
```

## Comparing `nonebot_adapter_kaiheila-0.2.5.tar` & `nonebot_adapter_kaiheila-0.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1065 2023-04-06 02:30:47.028934 nonebot_adapter_kaiheila-0.2.5/LICENSE
--rw-r--r--   0        0        0      296 2023-04-06 02:30:47.028934 nonebot_adapter_kaiheila-0.2.5/README.md
--rw-r--r--   0        0        0      359 2023-04-06 02:30:47.028934 nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/__init__.py
--rw-r--r--   0        0        0    15919 2023-04-06 02:30:47.028934 nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/adapter.py
--rw-r--r--   0        0        0       66 2023-04-06 02:30:47.028934 nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/api/__init__.py
--rw-r--r--   0        0        0       27 2023-04-06 02:30:47.028934 nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/api/client.py
--rw-r--r--   0        0        0    13445 2023-04-06 02:30:47.028934 nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/api/client.pyi
--rw-r--r--   0        0        0     4153 2023-04-06 02:30:47.028934 nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/api/handle.py
--rw-r--r--   0        0        0    12975 2023-04-06 02:30:47.028934 nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/api/model.py
--rw-r--r--   0        0        0    12338 2023-04-06 02:30:47.028934 nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/bot.py
--rw-r--r--   0        0        0      833 2023-04-06 02:30:47.028934 nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/config.py
--rw-r--r--   0        0        0    28176 2023-04-06 02:30:47.028934 nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/event.py
--rw-r--r--   0        0        0     3504 2023-04-06 02:30:47.028934 nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/exception.py
--rw-r--r--   0        0        0    12822 2023-04-06 02:30:47.028934 nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/message.py
--rw-r--r--   0        0        0      494 2023-04-06 02:30:47.028934 nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/permission.py
--rw-r--r--   0        0        0     2437 2023-04-06 02:30:47.028934 nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/utils.py
--rw-r--r--   0        0        0      709 2023-04-06 02:30:47.032934 nonebot_adapter_kaiheila-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1090 1970-01-01 00:00:00.000000 nonebot_adapter_kaiheila-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/LICENSE
+-rw-r--r--   0        0        0      296 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/README.md
+-rw-r--r--   0        0        0      359 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/__init__.py
+-rw-r--r--   0        0        0    15919 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/adapter.py
+-rw-r--r--   0        0        0       66 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/api/__init__.py
+-rw-r--r--   0        0        0       27 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/api/client.py
+-rw-r--r--   0        0        0    13445 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/api/client.pyi
+-rw-r--r--   0        0        0     4153 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/api/handle.py
+-rw-r--r--   0        0        0    12976 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/api/model.py
+-rw-r--r--   0        0        0    12338 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/bot.py
+-rw-r--r--   0        0        0      833 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/config.py
+-rw-r--r--   0        0        0    28176 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/event.py
+-rw-r--r--   0        0        0     3504 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/exception.py
+-rw-r--r--   0        0        0    12822 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/message.py
+-rw-r--r--   0        0        0      494 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/permission.py
+-rw-r--r--   0        0        0     2437 2023-04-16 05:35:36.030823 nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/utils.py
+-rw-r--r--   0        0        0      749 2023-04-16 05:35:36.034823 nonebot_adapter_kaiheila-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1090 1970-01-01 00:00:00.000000 nonebot_adapter_kaiheila-0.2.6/PKG-INFO
```

### Comparing `nonebot_adapter_kaiheila-0.2.5/LICENSE` & `nonebot_adapter_kaiheila-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/adapter.py` & `nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/api/client.pyi` & `nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/api/client.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/api/handle.py` & `nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/api/handle.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/api/model.py` & `nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/api/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     https://developer.kaiheila.cn/doc/objects
     """
     id_: Optional[str] = Field(None, alias="id")
     """用户的 id"""
     username: Optional[str] = None
     """用户的名称"""
-    nikname: Optional[str] = None
+    nickname: Optional[str] = None
     """用户在当前服务器的昵称"""
     identify_num: Optional[str] = None
     """用户名的认证数字，用户名正常为：user_name#identify_num"""
     online: Optional[bool] = None
     """当前是否在线"""
     bot: Optional[bool] = None
     """是否为机器人"""
```

### Comparing `nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/bot.py` & `nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/config.py` & `nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/event.py` & `nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/event.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/exception.py` & `nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/message.py` & `nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.5/nonebot/adapters/kaiheila/utils.py` & `nonebot_adapter_kaiheila-0.2.6/nonebot/adapters/kaiheila/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_kaiheila-0.2.5/pyproject.toml` & `nonebot_adapter_kaiheila-0.2.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "nonebot-adapter-kaiheila"
-version = "0.2.5"
+version = "0.2.6"
 description = "kaiheila adapter for nonebot2"
-authors = ["Tian-que <1605206150@qq.com>"]
+authors = ["Tian-que <1605206150@qq.com>", "ssttkkl <huang.wen.long@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Tian-que/nonebot-adapter-kaiheila"
 keywords = ["bot", "khl", "kaiheila", "khlbot"]
 
 packages = [
   { include = "nonebot" }
```

### Comparing `nonebot_adapter_kaiheila-0.2.5/PKG-INFO` & `nonebot_adapter_kaiheila-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-kaiheila
-Version: 0.2.5
+Version: 0.2.6
 Summary: kaiheila adapter for nonebot2
 Home-page: https://github.com/Tian-que/nonebot-adapter-kaiheila
 License: MIT
 Keywords: bot,khl,kaiheila,khlbot
 Author: Tian-que
 Author-email: 1605206150@qq.com
 Requires-Python: >=3.9,<4.0
```

