# Comparing `tmp/nonebot_plugin_eventmonitor-0.1.5.tar.gz` & `tmp/nonebot_plugin_eventmonitor-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_eventmonitor-0.1.5.tar", last modified: Sun Apr  9 06:13:09 2023, max compression
+gzip compressed data, was "nonebot_plugin_eventmonitor-0.1.6.tar", last modified: Sun Apr 16 07:21:47 2023, max compression
```

## Comparing `nonebot_plugin_eventmonitor-0.1.5.tar` & `nonebot_plugin_eventmonitor-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 06:13:09.467748 nonebot_plugin_eventmonitor-0.1.5/
--rw-rw-rw-   0        0        0    35149 2023-01-29 04:13:58.000000 nonebot_plugin_eventmonitor-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     1293 2023-04-09 06:13:09.467748 nonebot_plugin_eventmonitor-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      662 2023-04-09 06:12:53.000000 nonebot_plugin_eventmonitor-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 06:13:09.420829 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor/
--rw-rw-rw-   0        0        0     4627 2023-04-09 06:00:28.000000 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor/__init__.py
--rw-rw-rw-   0        0        0     1882 2023-04-09 05:58:13.000000 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor/admin.py
--rw-rw-rw-   0        0        0     1086 2023-04-09 05:58:40.000000 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor/honour.py
--rw-rw-rw-   0        0        0     1995 2023-04-09 05:58:48.000000 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor/stamp.py
--rw-rw-rw-   0        0        0      386 2023-04-09 05:58:55.000000 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-09 06:13:09.467748 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor.egg-info/
--rw-rw-rw-   0        0        0     1293 2023-04-09 06:13:08.000000 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      469 2023-04-09 06:13:09.000000 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 06:13:08.000000 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-09 06:13:08.000000 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-04-09 06:13:08.000000 nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 06:13:09.467748 nonebot_plugin_eventmonitor-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      993 2023-04-09 06:11:30.000000 nonebot_plugin_eventmonitor-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 07:21:47.476523 nonebot_plugin_eventmonitor-0.1.6/
+-rw-rw-rw-   0        0        0    35149 2023-01-29 04:13:58.000000 nonebot_plugin_eventmonitor-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     1320 2023-04-16 07:21:47.460916 nonebot_plugin_eventmonitor-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      689 2023-04-16 07:19:49.000000 nonebot_plugin_eventmonitor-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 07:21:47.414026 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor/
+-rw-rw-rw-   0        0        0     4627 2023-04-09 06:00:28.000000 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor/__init__.py
+-rw-rw-rw-   0        0        0     1882 2023-04-09 05:58:13.000000 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor/admin.py
+-rw-rw-rw-   0        0        0     1086 2023-04-16 07:03:41.000000 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor/honour.py
+-rw-rw-rw-   0        0        0     1995 2023-04-09 05:58:48.000000 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor/stamp.py
+-rw-rw-rw-   0        0        0      386 2023-04-16 07:04:11.000000 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-16 07:21:47.460916 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor.egg-info/
+-rw-rw-rw-   0        0        0     1320 2023-04-16 07:21:46.000000 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-04-16 07:21:47.000000 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 07:21:46.000000 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-16 07:21:46.000000 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-04-16 07:21:46.000000 nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 07:21:47.476523 nonebot_plugin_eventmonitor-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      993 2023-04-16 07:11:29.000000 nonebot_plugin_eventmonitor-0.1.6/setup.py
```

### Comparing `nonebot_plugin_eventmonitor-0.1.5/LICENSE` & `nonebot_plugin_eventmonitor-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_eventmonitor-0.1.5/PKG-INFO` & `nonebot_plugin_eventmonitor-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_eventmonitor
-Version: 0.1.5
+Version: 0.1.6
 Summary: 监控群事件的插件，支持戳一戳，成员变动，群荣誉，运气王变化等提示
 Home-page: https://github.com/Reversedeer/nonebot_plugin_eventmonitor
 Author: schwarzwald
 Project-URL: Bug Tracker, https://github.com/Reversedeer/nonebot_plugin_eventmonitor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <details>
     <summary><h2>更新日志</h2></summary>
 
-- v0.1.5
+- v0.1.6
 
+  - 修复bug
+  
+- v0.1.5
   - 优化配置文件 [#issue6](https://github.com/Reversedeer/nonebot_plugin_eventmonitor/issues/6)
   - 删除冗余代码
   - 修复获取superusers数值bug
-  
+
 - v0.1.3
   - 修复配置文件bug
 - v0.1.2
   - 增加了戳一戳的文案
 
   - 修改一些bug
 - v0.1.1
```

### Comparing `nonebot_plugin_eventmonitor-0.1.5/README.md` & `nonebot_plugin_eventmonitor-0.1.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 <details>
     <summary><h2>更新日志</h2></summary>
 
-- v0.1.5
+- v0.1.6
 
+  - 修复bug
+  
+- v0.1.5
   - 优化配置文件 [#issue6](https://github.com/Reversedeer/nonebot_plugin_eventmonitor/issues/6)
   - 删除冗余代码
   - 修复获取superusers数值bug
-  
+
 - v0.1.3
   - 修复配置文件bug
 - v0.1.2
   - 增加了戳一戳的文案
 
   - 修改一些bug
 - v0.1.1
```

### Comparing `nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor/__init__.py` & `nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor/admin.py` & `nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor/admin.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor/honour.py` & `nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor/honour.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 async def monitor_rongyu(honor_type, user_id, bot_qq):  
     rely = ""
 
     if honor_type == "emotion":
         if user_id == bot_qq:
             pass
-        elif user_id != superusers:
+        elif user_id in superusers:
             rely = f"[CQ:at,qq={user_id}]恭喜主人荣获快乐源泉🤣标识喵~"
         else:
             rely = f"恭喜[CQ:at,qq={user_id}]荣获快乐源泉🤣标识喵~"
     elif honor_type == "performer":
         if user_id == bot_qq:
             pass
-        elif user_id != superusers:
+        elif user_id in superusers:
             rely = f"[CQ:at,qq={user_id}]恭喜主人荣获群聊之火🔥标识喵~"
         else:
             rely = f"恭喜[CQ:at,qq={user_id}]荣获群聊之火🔥标识喵~"
 
     elif honor_type == "talkative":
         if user_id == bot_qq:
             rely = "你们又不行了，本喵喜提龙王🐲~"
-        elif user_id != superusers:
+        elif user_id in superusers:
             rely = f"[CQ:at,qq={user_id}]恭喜主人荣获龙王🐲标识喵~"
         else:
             rely = f"恭喜[CQ:at,qq={user_id}]荣获龙王🐲标识喵~"
 
     return rely
```

### Comparing `nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor/stamp.py` & `nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor/stamp.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_eventmonitor-0.1.5/nonebot_plugin_eventmonitor.egg-info/PKG-INFO` & `nonebot_plugin_eventmonitor-0.1.6/nonebot_plugin_eventmonitor.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-eventmonitor
-Version: 0.1.5
+Version: 0.1.6
 Summary: 监控群事件的插件，支持戳一戳，成员变动，群荣誉，运气王变化等提示
 Home-page: https://github.com/Reversedeer/nonebot_plugin_eventmonitor
 Author: schwarzwald
 Project-URL: Bug Tracker, https://github.com/Reversedeer/nonebot_plugin_eventmonitor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <details>
     <summary><h2>更新日志</h2></summary>
 
-- v0.1.5
+- v0.1.6
 
+  - 修复bug
+  
+- v0.1.5
   - 优化配置文件 [#issue6](https://github.com/Reversedeer/nonebot_plugin_eventmonitor/issues/6)
   - 删除冗余代码
   - 修复获取superusers数值bug
-  
+
 - v0.1.3
   - 修复配置文件bug
 - v0.1.2
   - 增加了戳一戳的文案
 
   - 修改一些bug
 - v0.1.1
```

### Comparing `nonebot_plugin_eventmonitor-0.1.5/setup.py` & `nonebot_plugin_eventmonitor-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nonebot_plugin_eventmonitor",
-    version="0.1.5",
+    version="0.1.6",
     author="schwarzwald",
     description="监控群事件的插件，支持戳一戳，成员变动，群荣誉，运气王变化等提示",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Reversedeer/nonebot_plugin_eventmonitor",
     project_urls={
         "Bug Tracker": "https://github.com/Reversedeer/nonebot_plugin_eventmonitor/issues",
```

