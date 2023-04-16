# Comparing `tmp/nonebot_plugin_naturel_gpt-2.1.1.tar.gz` & `tmp/nonebot_plugin_naturel_gpt-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_naturel_gpt-2.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_naturel_gpt-2.1.2.tar", max compression
```

## Comparing `nonebot_plugin_naturel_gpt-2.1.1.tar` & `nonebot_plugin_naturel_gpt-2.1.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    11558 2023-01-29 20:13:51.193394 nonebot_plugin_naturel_gpt-2.1.1/LICENSE
--rw-r--r--   0        0        0     2319 2023-04-05 16:12:46.781524 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/__init__.py
--rw-r--r--   0        0        0    26178 2023-04-15 05:32:09.844193 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/chat.py
--rw-r--r--   0        0        0     5984 2023-03-31 09:56:17.960037 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/chat_manager.py
--rw-r--r--   0        0        0    23054 2023-04-15 05:35:00.587717 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/command_func.py
--rw-r--r--   0        0        0    12717 2023-04-14 13:54:29.320533 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/config.py
--rw-r--r--   0        0        0     6159 2023-04-05 16:12:46.780526 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/Extension.py
--rw-r--r--   0        0        0      237 2023-04-05 16:12:46.786453 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/logger.py
--rw-r--r--   0        0        0    34824 2023-04-14 19:56:43.371549 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/matcher.py
--rw-r--r--   0        0        0     1218 2023-04-14 15:48:38.092610 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/MCrcon/COPING.txt
--rw-r--r--   0        0        0     6269 2023-04-14 14:50:18.078484 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/MCrcon/mcrcon.py
--rw-r--r--   0        0        0     9912 2023-04-08 05:19:53.226132 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/openai_func.py
--rw-r--r--   0        0        0    10828 2023-04-05 16:12:46.788447 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/persistent_data_manager.py
--rw-r--r--   0        0        0      484 2023-03-16 11:26:31.740167 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/singleton.py
--rw-r--r--   0        0        0     2715 2023-04-05 16:12:46.789445 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/store.py
--rw-r--r--   0        0        0     1831 2023-04-05 16:12:46.790443 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/text_func.py
--rw-r--r--   0        0        0     4350 2023-03-31 09:56:17.964030 nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/utils.py
--rw-r--r--   0        0        0      577 2023-04-15 10:03:46.610454 nonebot_plugin_naturel_gpt-2.1.1/pyproject.toml
--rw-r--r--   0        0        0    52307 2023-04-15 10:01:47.674482 nonebot_plugin_naturel_gpt-2.1.1/README.md
--rw-r--r--   0        0        0    52295 1970-01-01 00:00:00.000000 nonebot_plugin_naturel_gpt-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-01-29 20:13:51.193394 nonebot_plugin_naturel_gpt-2.1.2/LICENSE
+-rw-r--r--   0        0        0     2345 2023-04-15 18:38:05.110657 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/__init__.py
+-rw-r--r--   0        0        0    26222 2023-04-16 16:20:15.076676 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/chat.py
+-rw-r--r--   0        0        0     6004 2023-04-15 18:38:05.113654 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/chat_manager.py
+-rw-r--r--   0        0        0    23543 2023-04-15 18:38:05.115650 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/command_func.py
+-rw-r--r--   0        0        0    12868 2023-04-16 12:44:36.108186 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/config.py
+-rw-r--r--   0        0        0     6187 2023-04-15 18:38:05.109147 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/Extension.py
+-rw-r--r--   0        0        0      237 2023-04-05 16:12:46.786453 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/logger.py
+-rw-r--r--   0        0        0    29500 2023-04-16 14:10:42.687395 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/matcher.py
+-rw-r--r--   0        0        0     7300 2023-04-16 11:16:04.694453 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/matcher_MCRcon.py
+-rw-r--r--   0        0        0     1218 2023-04-14 15:48:38.092610 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/MCrcon/COPING.txt
+-rw-r--r--   0        0        0     6285 2023-04-15 18:38:05.110151 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/MCrcon/mcrcon.py
+-rw-r--r--   0        0        0    10245 2023-04-15 18:38:05.120960 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/openai_func.py
+-rw-r--r--   0        0        0    10828 2023-04-05 16:12:46.788447 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/persistent_data_manager.py
+-rw-r--r--   0        0        0      499 2023-04-15 18:38:05.121664 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/singleton.py
+-rw-r--r--   0        0        0     2715 2023-04-05 16:12:46.789445 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/store.py
+-rw-r--r--   0        0        0     1831 2023-04-05 16:12:46.790443 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/text_func.py
+-rw-r--r--   0        0        0     4556 2023-04-15 18:38:05.122660 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/utils.py
+-rw-r--r--   0        0        0      741 2023-04-16 16:17:56.636992 nonebot_plugin_naturel_gpt-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0    53632 2023-04-16 16:17:47.921979 nonebot_plugin_naturel_gpt-2.1.2/README.md
+-rw-r--r--   0        0        0    53598 1970-01-01 00:00:00.000000 nonebot_plugin_naturel_gpt-2.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.1/LICENSE` & `nonebot_plugin_naturel_gpt-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/__init__.py` & `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-from typing import Awaitable, Callable, Tuple
+from typing import Awaitable, Callable, Optional, Tuple
 from nonebot import get_driver
 from .logger import logger
-from nonebot.params import Matcher
-from nonebot.adapters.onebot.v11 import Bot, MessageEvent
+from nonebot.matcher import Matcher
+from nonebot.adapters import Bot, Event
 
 from .config import *
 from . import utils
 
 global_config = get_driver().config
 # logger.info(config) # 这里可以打印出配置文件的内容
 
 from .openai_func import TextGenerator
 from .Extension import load_extensions
 from .persistent_data_manager import PersistentDataManager
 from .chat_manager import ChatManager
 from . import matcher
+from . import matcher_MCRcon
 
 
-def set_permission_check_func(callback:Callable[[Matcher, MessageEvent, Bot, str, str], Awaitable[Tuple[bool,str]]]):
+def set_permission_check_func(callback:Callable[[Matcher, Event, Bot, str, str], Awaitable[Tuple[bool,Optional[str]]]]):
     """设置Matcher的权限检查函数"""
     matcher.permission_check_func = callback
 
 # 设置默认权限检查函数，有需求时可以覆盖
 set_permission_check_func(utils.default_permission_check_func)
 
 """ ======== 读取历史记忆数据 ======== """
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/chat.py` & `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/chat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,161 +1,158 @@
 ﻿import copy
 import time
-from typing import Dict, List, Tuple
+from typing import Dict, List, Optional, Tuple
 from .logger import logger
 from . import Extension
 
 from .text_func import compare_text
 from .config import *
 from .openai_func import TextGenerator
 from .persistent_data_manager import ImpressionData, ChatData, PresetData
 from .Extension import Extension, global_extensions
 
 # 会话类
 class Chat:
     """ ======== 定义会话类 ======== """
-    _chat_key:str
-    _preset_key = ''  # 预设标识
-    _chat_data:ChatData # 此chat_key聊天数据
-    _chat_preset:PresetData = None                      # 当前对话预设
-    _chat_preset_dicts:Dict[str, PresetData] = None     # 预设字典
+    _chat_data:ChatData         # 此chat_key关联的聊天数据
+    _preset_key = ''            # 预设标识
     _last_msg_time = 0          # 上次对话时间
     is_insilence = False        # 是否处于沉默状态
     chat_attitude = 0           # 对话态度
     silence_time = 0            # 沉默时长
 
     def __init__(self, chat_data:ChatData, preset_key:str = ''):
         if not isinstance(chat_data, ChatData):
             raise Exception(f'chat_data 参数不是ChatData类型,实际类型为:{type(chat_data).__name__}')
-        self._chat_data = chat_data # 当前对话预设
-        self._chat_preset_dicts = self._chat_data.preset_datas
-        self._chat_key = chat_data.chat_key    # 对话标识
+        self._chat_data = chat_data # 当前对话关联的数据
         preset_key = preset_key or self._chat_data.active_preset # 参数没有设置时尝试查找上次使用的preset
         if not preset_key:  # 如果没有预设，选择默认预设
-            for (pk, preset) in self._chat_preset_dicts.items():
+            for (pk, preset) in self.chat_preset_dicts.items():
                 if preset.is_default:
                     preset_key = pk
                     break
             else:   # 如果没有默认预设，则选择第一个预设
-                preset_key = list(self._chat_preset_dicts.keys())[0]
+                preset_key = list(self.chat_preset_dicts.keys())[0]
         self.change_presettings(preset_key)
 
     async def update_chat_history_row(self, sender:str, msg: str, require_summary:bool = False) -> None:
         """更新当前会话的全局对话历史行"""
         tg = TextGenerator.instance
         messageunit = tg.generate_msg_template(sender=sender, msg=msg, time_str=f"[{time.strftime('%H:%M:%S %p', time.localtime())}] ")
         self._chat_data.chat_history.append(messageunit)
-        if config.DEBUG_LEVEL > 0: logger.info(f"[会话: {self._chat_key}]添加对话历史行: {messageunit}\n  |  当前对话历史行数: {len(self._chat_data.chat_history)}")
+        if config.DEBUG_LEVEL > 0: logger.info(f"[会话: {self.chat_key}]添加对话历史行: {messageunit}  |  当前对话历史行数: {len(self._chat_data.chat_history)}")
         self._last_msg_time = time.time()   # 更新上次对话时间
         while len(self._chat_data.chat_history) > config.CHAT_MEMORY_MAX_LENGTH * 2:    # 保证对话历史不超过最大长度的两倍
             self._chat_data.chat_history.pop(0)
 
         if len(self._chat_data.chat_history) > config.CHAT_MEMORY_MAX_LENGTH and require_summary and config.CHAT_ENABLE_SUMMARY_CHAT: # 只有在开启总结功能并且在bot回复后才进行总结 避免不必要的token消耗
             prev_summarized = f"Summary of last conversation:{self._chat_data.chat_summarized}\n\n"
             history_str = '\n'.join(self._chat_data.chat_history)
             prompt = (  # 以机器人的视角总结对话历史
                 f"{prev_summarized}[Chat]\n"
                 f"{history_str}"
-                f"\n\n{self._chat_preset.bot_self_introl}\nSummarize the chat in one paragraph from the perspective of '{self._chat_preset.preset_key}' and record as much important information as possible from the conversation:"
+                f"\n\n{self.chat_preset.bot_self_introl}\nSummarize the chat in one paragraph from the perspective of '{self.chat_preset.preset_key}' and record as much important information as possible from the conversation:"
             )
             # if config.DEBUG_LEVEL > 0: logger.info(f"生成对话历史摘要prompt: {prompt}")
             res, success = await tg.get_response(prompt, type='summarize')  # 生成新的对话历史摘要
             if success:
                 self._chat_data.chat_summarized = res.strip()
             else:
                 logger.error(f"生成对话历史摘要失败: {res}")
                 return
             # logger.info(f"生成对话历史摘要: {self.chat_presets['chat_summarized']}")
             if config.DEBUG_LEVEL > 0: logger.info(f"摘要生成消耗token数: {tg.cal_token_count(prompt + self._chat_data.chat_summarized)}")
             self._chat_data.chat_history = self._chat_data.chat_history[-config.CHAT_MEMORY_SHORT_LENGTH:]
 
     async def update_chat_history_row_for_user(self, sender:str, msg: str, userid:str, username:str, require_summary:bool = False) -> None:
         """更新对特定用户的对话历史行"""
-        if userid not in self._chat_preset.chat_impressions:
+        if userid not in self.chat_preset.chat_impressions:
             impression_data = ImpressionData(user_id=userid)
-            self._chat_preset.chat_impressions[userid] = impression_data
+            self.chat_preset.chat_impressions[userid] = impression_data
         else:
-            impression_data = self._chat_preset.chat_impressions[userid]
+            impression_data = self.chat_preset.chat_impressions[userid]
         tg = TextGenerator.instance
         messageunit = tg.generate_msg_template(sender=sender, msg=msg)
         impression_data.chat_history.append(messageunit)
-        if config.DEBUG_LEVEL > 0: logger.info(f"添加对话历史行: {messageunit}\n  |  当前对话历史行数: {len(impression_data.chat_history)}")
+        if config.DEBUG_LEVEL > 0: logger.info(f"添加对话历史行: {messageunit}  |  当前对话历史行数: {len(impression_data.chat_history)}")
         # 保证对话历史不超过最大长度
         if len(impression_data.chat_history) > config.USER_MEMORY_SUMMARY_THRESHOLD and require_summary:
             prev_summarized = f"Last impression:{impression_data.chat_impression}\n\n"
             history_str = '\n'.join(impression_data.chat_history)
             prompt = (   # 以机器人的视角总结对话
                 f"{prev_summarized}[Chat]\n"
                 f"{history_str}"
-                f"\n\n{self._chat_preset.bot_self_introl}\nUpdate {username} impressions from the perspective of {self._chat_preset.preset_key}:"
+                f"\n\n{self.chat_preset.bot_self_introl}\nUpdate {username} impressions from the perspective of {self.chat_preset.preset_key}:"
             )
             # if config.DEBUG_LEVEL > 0: logger.info(f"生成对话历史摘要prompt: {prompt}")
             res, success = await tg.get_response(prompt, type='summarize')  # 生成新的对话历史摘要
             if success:
                 impression_data.chat_impression = res.strip()
             else:
                 logger.error(f"生成对话印象摘要失败: {res}")
                 return
             # logger.info(f"生成对话印象摘要: {global_preset_userdata[self.preset_key][userid]['chat_impression']}")
             if config.DEBUG_LEVEL > 0: logger.info(f"印象生成消耗token数: {tg.cal_token_count(prompt + impression_data.chat_impression)}")
             impression_data.chat_history = impression_data.chat_history[-config.CHAT_MEMORY_SHORT_LENGTH:]
 
     def set_memory(self, mem_key:str, mem_value:str = '') -> None:
         """为当前预设设置记忆"""
+        if not mem_key:
+            return
         mem_key = mem_key.replace(' ', '_')  # 将空格替换为下划线
         # 如果没有指定mem_value，则删除该记忆
         if not mem_value:
-            if mem_key in self._chat_preset.chat_memory:
-                del self._chat_preset.chat_memory[mem_key]
+            if mem_key in self.chat_preset.chat_memory:
+                del self.chat_preset.chat_memory[mem_key]
                 if config.DEBUG_LEVEL > 0: logger.info(f"忘记了: {mem_key}")
             else:
                 logger.warning(f"尝试删除不存在的记忆 {mem_key}")
         else:   # 否则设置该记忆，并将其移到在最后
-            if mem_key in self._chat_preset.chat_memory:
-                del self._chat_preset.chat_memory[mem_key]
-            self._chat_preset.chat_memory[mem_key] = mem_value
+            if mem_key in self.chat_preset.chat_memory:
+                del self.chat_preset.chat_memory[mem_key]
+            self.chat_preset.chat_memory[mem_key] = mem_value
             if config.DEBUG_LEVEL > 0: logger.info(f"记住了: {mem_key} -> {mem_value}")
 
-            if len(self._chat_preset.chat_memory) > config.CHAT_MEMORY_MAX_LENGTH:   # 检查记忆是否超过最大长度 超出则删除最早的记忆并记录日志
-                del_key = list(self._chat_preset.chat_memory.keys())[0]
-                del self._chat_preset.chat_memory[del_key]
+            if len(self.chat_preset.chat_memory) > config.CHAT_MEMORY_MAX_LENGTH:   # 检查记忆是否超过最大长度 超出则删除最早的记忆并记录日志
+                del_key = list(self.chat_preset.chat_memory.keys())[0]
+                del self.chat_preset.chat_memory[del_key]
                 if config.DEBUG_LEVEL > 0: logger.info(f"忘记了: {del_key} (超出最大记忆长度)")
 
-    def enhance_memory(self, response:str) -> bool:
-        """增强记忆 如果响应中的内容与记忆中的内容相似，则增强记忆(将改记忆移到最后)"""
-        for mem_key, mem_value in self._chat_preset.chat_memory.items():#模糊匹配
-            compare_score = compare_text(response, mem_value)
-            if config.DEBUG_LEVEL > 0: logger.info(f"增强记忆比较: {response} vs {mem_value} = {compare_score}")
-            if compare_score > config.CHAT_MEMORY_ENHANCE_THRESHOLD:
-                self.set_memory(mem_key, mem_value)
-                if config.DEBUG_LEVEL > 0: logger.info(f"记忆 {mem_key} 相似度 {compare_score} 超过阈值 {config.CHAT_MEMORY_ENHANCE_THRESHOLD}, 增强记忆")
-                return True
-        return False
+    # def enhance_memory(self, response:str) -> bool:
+    #     """增强记忆 如果响应中的内容与记忆中的内容相似，则增强记忆(将改记忆移到最后)"""
+    #     for mem_key, mem_value in self.chat_preset.chat_memory.items():#模糊匹配
+    #         compare_score = compare_text(response, mem_value)
+    #         if config.DEBUG_LEVEL > 0: logger.info(f"增强记忆比较: {response} vs {mem_value} = {compare_score}")
+    #         if compare_score > config.CHAT_MEMORY_ENHANCE_THRESHOLD: # TODO 此配置字段已不存在，应该删除？
+    #             self.set_memory(mem_key, mem_value)
+    #             if config.DEBUG_LEVEL > 0: logger.info(f"记忆 {mem_key} 相似度 {compare_score} 超过阈值 {config.CHAT_MEMORY_ENHANCE_THRESHOLD}, 增强记忆")
+    #             return True
+    #     return False
 
-    def get_chat_prompt_template(self, userid:str = None, chat_type:str = '')-> str:
+    def get_chat_prompt_template(self, userid:str, chat_type:str = '')-> List[Dict[str, str]]:
         """对话 prompt 模板生成"""
         # 印象描述
-        impression_text = f"[impression]\n{self._chat_preset.chat_impressions[userid].chat_impression}\n\n" \
-            if userid in self._chat_preset.chat_impressions else ''  # 用户印象描述
+        impression_text = f"[impression]\n{self.chat_preset.chat_impressions[userid].chat_impression}\n\n" \
+            if userid in self.chat_preset.chat_impressions else ''  # 用户印象描述
 
         # 记忆模块
         memory_text = ''
         memory = ''
-        self._chat_preset.chat_memory = {k: v for k, v in self._chat_preset.chat_memory.items() if v} # 删除空记忆 TODO 怎么出现的空记忆？
+        self.chat_preset.chat_memory = {k: v for k, v in self.chat_preset.chat_memory.items() if v} # 删除空记忆 TODO 怎么出现的空记忆？
         # 如果有记忆，则生成记忆模板
         idx = 0 # 记忆序号
-        for k, v in self._chat_preset.chat_memory.items():
+        for k, v in self.chat_preset.chat_memory.items():
             idx += 1
             memory_text += f"{idx}. {k}: {v}\n"
 
         # 删除多余的记忆
-        if len(self._chat_preset.chat_memory) > config.MEMORY_MAX_LENGTH:
-            self._chat_preset.chat_memory = {k: v for k, v in sorted(self._chat_preset.chat_memory.items(), key=lambda item: item[1])}
-            self._chat_preset.chat_memory = {k: v for k, v in list(self._chat_preset.chat_memory.items())[:config.MEMORY_MAX_LENGTH]}
-            if config.DEBUG_LEVEL > 0: logger.info(f"删除多余记忆: {self._chat_preset.chat_memory}")
+        if len(self.chat_preset.chat_memory) > config.MEMORY_MAX_LENGTH:
+            self.chat_preset.chat_memory = {k: v for k, v in sorted(self.chat_preset.chat_memory.items(), key=lambda item: item[1])}
+            self.chat_preset.chat_memory = {k: v for k, v in list(self.chat_preset.chat_memory.items())[:config.MEMORY_MAX_LENGTH]}
+            if config.DEBUG_LEVEL > 0: logger.info(f"删除多余记忆: {self.chat_preset.chat_memory}")
 
         if config.MEMORY_ACTIVE:  # 如果记忆功能开启
             if global_extensions.get('remember') and global_extensions.get('forget'): # 如果记忆功能已加载
                 memory = (  # 如果有记忆，则生成记忆模板
                     f"[history memory (max length: {config.MEMORY_MAX_LENGTH} - Please delete the unimportant memory in time before exceed it)]\n"
                     f"{memory_text}\n"
                     f"ATTENTION: The earlier chat history may not be provided again in the next request, use /#remember&key&value#/ to remember something\n\n"
@@ -261,179 +258,184 @@
                 "\nDeveloper: Send an email to me for testing\n"
                 "\nAlice:(Generate the response content of Alice, excluding 'Alice:')"
             )},
             {'role': 'assistant', 'content': (  # 助手消息(演示输出)
                 "ok, I will send an email, please wait a moment /#email&example@mail.com&test title&hello this is a test#/ *; I have sent an e-mail. Did you get it?"
             )},
             {'role': 'user', 'content': (   # 用户消息(实际场景)
-                f"[Character setting]\n{self._chat_preset.bot_self_introl}\n\n"
+                f"[Character setting]\n{self.chat_preset.bot_self_introl}\n\n"
                 f"{memory}{impression_text}{summary}"
                 f"\n[{chat_history_title} (current time: {time.strftime('%Y-%m-%d %H:%M:%S %A')})]\n"
-                f"\n{chat_history}\n\n{self._chat_preset.preset_key}:(Generate the response content of {self._chat_preset.preset_key}, excluding '{self._chat_preset.preset_key}:', Do not generate any reply from anyone else.)"
+                f"\n{chat_history}\n\n{self.chat_preset.preset_key}:(Generate the response content of {self.chat_preset.preset_key}, excluding '{self.chat_preset.preset_key}:', Do not generate any reply from anyone else.)"
             )},
         ]
+    
+    def generate_description(self, hide_chat_key:bool=False) -> str:
+        """获取当前会话描述"""
+        if hide_chat_key:
+            return f"[{'启用' if self.is_enable else '禁用'}] 会话: {self.chat_key[:-6]+('*'*6)} 预设: {self.preset_key}\n"
+        else:
+            return f"[{'启用' if self.is_enable else '禁用'}] 会话: {self.chat_key} 预设: {self.preset_key}\n"
 
+    # region --------------------以下为只读属性定义--------------------
 
-    # region --------------------以下为基本信息获取函数和属性--------------------
-
-    def get_chat_key(self) ->str:
-        """获取当前会话 chat_key"""
-        return self._chat_key
-
-    def get_chat_preset_key(self) -> str:
-        """获取当前对话bot的预设键"""
-        return self._preset_key
-    
     @property
     def chat_key(self) ->str:
         """获取当前会话 chat_key"""
-        return self._chat_key
-
+        return self._chat_data.chat_key
+    
     @property
     def preset_key(self) -> str:
         """获取当前对话bot的预设键"""
         return self._preset_key
     
     @property
+    def chat_preset_dicts(self)->Dict[str, PresetData]:
+        """获取当前预设数据字典"""
+        return self._chat_data.preset_datas
+
+    @property
+    def chat_preset(self)->PresetData:
+        """获取当前正在使用的预设的数据"""
+        return self.chat_preset_dicts[self.preset_key]
+
+    @property
     def is_using_default_preset(self) -> bool:
         """当前使用的预设是否是默认预设"""
-        return self._chat_preset.is_default
+        return self.chat_preset.is_default
     
     @property
     def is_enable(self):
         """当前会话是否已启用"""
         return self._chat_data.is_enable
 
     @property
     def enable_auto_switch_identity(self):
         """当前会话是否已启用自动切换人格"""
         return self._chat_data.enable_auto_switch_identity
 
-    def generate_description(self, hide_chat_key:bool=False) -> str:
-        """获取当前会话描述"""
-        if hide_chat_key:
-            return f"[{'启用' if self.is_enable else '禁用'}] 会话: {self._chat_key[:-6]+('*'*6)} 预设: {self.get_chat_preset_key()}\n"
-        else:
-            return f"[{'启用' if self.is_enable else '禁用'}] 会话: {self._chat_key} 预设: {self.get_chat_preset_key()}\n"
-    
     @property
     def chat_data(self) -> ChatData:
         """获取chat_data, 请慎重操作"""
         return self._chat_data
     
     @property
     def active_preset(self)->PresetData:
         """获取当前正在使用的chat_preset, 请慎重操作"""
-        return self._chat_preset
+        return self.chat_preset
     
     @property
     def preset_keys(self)->List[str]:
         """获取当前会话的所有预设名称列表"""
-        return list(self._chat_preset_dicts.keys())
+        return list(self.chat_preset_dicts.keys())
+    
+    @property
+    def last_msg_time(self) -> float:
+        """获取上一条消息的时间"""
+        return self._last_msg_time
     
     # endregion 
 
 
     # region --------------------以下为数据获取和处理相关功能--------------------
 
     def toggle_chat(self, enabled:bool=True) -> None:
         """开关当前会话"""
         self._chat_data.is_enable = enabled
 
     def toggle_auto_switch(self, enabled:bool=True) -> None:
         """开关当前会话自动切换人格"""
         self._chat_data.enable_auto_switch_identity = enabled
     
-    def change_presettings(self, preset_key:str) -> Tuple[bool, str]:
+    def change_presettings(self, preset_key:str) -> Tuple[bool, Optional[str]]:
         """修改对话预设"""
-        if preset_key not in self._chat_preset_dicts:    # 如果聊天预设字典中没有该预设，则从全局预设字典中拷贝一个
+        if preset_key not in self.chat_preset_dicts:    # 如果聊天预设字典中没有该预设，则从全局预设字典中拷贝一个
             preset_config = config.PRESETS.get(preset_key, None)
             if not preset_config:
                 return (False, '预设不存在')
             self.add_preset_from_config(preset_key, preset_config)
             if config.DEBUG_LEVEL > 0: logger.info(f"从全局预设中拷贝预设 {preset_key} 到聊天预设字典")
         self._chat_data.active_preset = preset_key
-        self._chat_preset = self._chat_preset_dicts[preset_key]
         self._preset_key = preset_key
         return (True, None)
     
-    def add_preset(self, preset_key:str, bot_self_introl: str) -> Tuple[bool, str]:
+    def add_preset(self, preset_key:str, bot_self_introl: str) -> Tuple[bool, Optional[str]]:
         """添加新人格"""
-        if preset_key in self._chat_preset_dicts:
+        if preset_key in self.chat_preset_dicts:
             return (False, '同名预设已存在')
 
-        self._chat_preset_dicts[preset_key] = PresetData(preset_key=preset_key, bot_self_introl=bot_self_introl)
+        self.chat_preset_dicts[preset_key] = PresetData(preset_key=preset_key, bot_self_introl=bot_self_introl)
         return (True, None)
     
-    def add_preset_from_config(self, preset_key:str, preset_config: PresetConfig) -> Tuple[bool, str]:
+    def add_preset_from_config(self, preset_key:str, preset_config: PresetConfig) -> Tuple[bool, Optional[str]]:
         """从配置添加新人格, config_preset为config中的全局配置"""
-        if preset_key in self._chat_preset_dicts:
+        if preset_key in self.chat_preset_dicts:
             return (False, '同名预设已存在')
 
-        self._chat_preset_dicts[preset_key] = PresetData.create_from_config(preset_config)
+        self.chat_preset_dicts[preset_key] = PresetData.create_from_config(preset_config)
         # 更新默认值
         if preset_config.is_default:
-            for v in self._chat_preset_dicts.values():
+            for v in self.chat_preset_dicts.values():
                 v.is_default = v.preset_key == preset_key
         return (True, None)
     
-    def del_preset(self, preset_key:str) -> Tuple[bool, str]:
+    def del_preset(self, preset_key:str) -> Tuple[bool, Optional[str]]:
         """删除指定人格预设(允许删除系统人格)"""
-        if len(self._chat_preset_dicts) <= 1:
+        if len(self.chat_preset_dicts) <= 1:
             return (False, '当前会话只有一个预设，不允许删除')
-        if preset_key not in self._chat_preset_dicts:
+        if preset_key not in self.chat_preset_dicts:
             return (False, f'当前会话不存在预设 [{preset_key}]')
         
-        default_preset_key = [preset for preset in self._chat_preset_dicts.values() if preset.is_default][0].preset_key
+        default_preset_key = [preset for preset in self.chat_preset_dicts.values() if preset.is_default][0].preset_key
 
         if preset_key == default_preset_key:
             return (False, '默认预设不允许删除')
         
         if self._preset_key == preset_key:
             # 删除当前正在使用的preset时切换到默认预设
             self.change_presettings(default_preset_key)
-        del self._chat_preset_dicts[preset_key]
+        del self.chat_preset_dicts[preset_key]
         return (True, None)
     
-    def update_preset(self, preset_key:str, bot_self_introl: str) -> Tuple[bool, str]:
+    def update_preset(self, preset_key:str, bot_self_introl: str) -> Tuple[bool, Optional[str]]:
         """修改指定人格预设"""
-        if preset_key not in self._chat_preset_dicts:
+        if preset_key not in self.chat_preset_dicts:
             return (False, f'预设 [{preset_key}] 不存在')
         
-        self._chat_preset_dicts[preset_key].bot_self_introl = bot_self_introl
+        self.chat_preset_dicts[preset_key].bot_self_introl = bot_self_introl
         return (True, None)
     
-    def rename_preset(self, old_preset_key:str, new_preset_key: str) -> Tuple[bool, str]:
+    def rename_preset(self, old_preset_key:str, new_preset_key: str) -> Tuple[bool, Optional[str]]:
         """改名指定预设, 对话历史将全部丢失！"""
-        if old_preset_key not in self._chat_preset_dicts:
+        if old_preset_key not in self.chat_preset_dicts:
             return (False, '原预设名不存在')
         
-        if new_preset_key in self._chat_preset_dicts:
+        if new_preset_key in self.chat_preset_dicts:
             return (False, '目标预设名已存在')
         
-        old_preset_data = self._chat_preset_dicts[old_preset_key]
+        old_preset_data = self.chat_preset_dicts[old_preset_key]
         if old_preset_data.is_default:
             return (False, '默认预设不允许改名')
         
         bot_self_introl = old_preset_data.bot_self_introl
         success, err_msg = self.del_preset(old_preset_key)
         if not success:
             return (False, err_msg)
         
         success, err_msg = self.add_preset(new_preset_key, bot_self_introl)
         return (success, err_msg)
     
-    def reset_preset(self, preset_key:str) -> Tuple[int, str]:
+    def reset_preset(self, preset_key:str) -> Tuple[int, Optional[str]]:
         """重置指定预设，将丢失对用户的对话历史和印象数据"""
         preset_config = config.PRESETS.get(preset_key, None)
         
-        if preset_key not in self._chat_preset_dicts:
+        if preset_key not in self.chat_preset_dicts:
             return (False, f'预设 [{preset_key}] 不存在')
-        self._chat_preset_dicts[preset_key].reset_to_default(preset_config)
+        self.chat_preset_dicts[preset_key].reset_to_default(preset_config)
         return (True, None)
     
-    def reset_chat(self) -> Tuple[bool, str]:
+    def reset_chat(self) -> Tuple[bool, Optional[str]]:
         """重置当前会话所有预设，将丢失性格或历史数据"""
         self._chat_data.reset()
         return (True, None)
     
     # endregion
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/chat_manager.py` & `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/chat_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿from typing import Dict, Tuple
+﻿from typing import Dict, Optional, Tuple
 from .singleton import Singleton
 from .chat import Chat
 from .persistent_data_manager import PersistentDataManager
 from .config import *
 
 class ChatManager(Singleton["ChatManager"]):
     """全局会话管理器"""
@@ -21,15 +21,15 @@
             if chat_key not in self._chat_dict:
                 self._chat_dict[chat_key] = Chat(chat_data)
 
     def has_chat_key(self, chat_key:str) -> bool:
         """是否存在指定chat_key"""
         return chat_key in self._chat_dict
     
-    def get_chat(self, chat_key: str) -> Chat:
+    def get_chat(self, chat_key: str) -> Optional[Chat]:
         """通过chat_key获取一个Chat对象"""
         return self._chat_dict.get(chat_key, None)
     
     def get_all_chats(self) -> List[Chat]:
         """获取所有的会话"""
         return list(self._chat_dict.values())
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/command_func.py` & `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/command_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Optional
 from .logger import logger
 from .chat import Chat
 from .chat_manager import ChatManager
 from .Extension import Extension, global_extensions, load_extensions
 
 import difflib
 import requests
@@ -34,24 +35,24 @@
         """注册指令修饰方法"""
         # print('register:', route, params)
         def wrapper(func):
             self.command_router[route] = {'arg_list': params, 'func': func}
             return func
         return wrapper
 
-    def execute(self, chat:Chat, command:str, chat_presets_dict:dict) -> dict:
+    def execute(self, chat:Chat, command:str, chat_presets_dict:dict) -> Optional[dict]:
         """执行指令"""
         option_dict, param_dict, target_route = self.resolve_command(command)
         logger.info(f'执行命令: "{command}";  指令匹配路由: {target_route}')
         if target_route:
             try:
                 return self.command_router[target_route]['func'](option_dict, param_dict, chat, chat_presets_dict)
             except Exception as e:
                 return {'error': e}
-        return False
+        return None
 
     def submit_commands(self):
         """提交指令注册 *在所有指令注册完成后调用*"""
         # 将指令路由字典根据键中包含的`/`数量进行降序排序 以便于匹配时优先匹配更长的指令
         self.command_router = dict(sorted(self.command_router.items(), key=lambda x: len(x[0].split('/')), reverse=True))
         # print('所有指令注册完成 共计:', len(self.command_router), '条指令')
 
@@ -105,15 +106,15 @@
         return option_dict, param_dict, target_route
 
 cmd:CommandManager = CommandManager()
 
 """ 注册指令 """
 @cmd.register(route='rg')
 def _(option_dict, param_dict, chat:Chat, chat_presets_dict:dict):
-    presets_show_text = '\n'.join([f'  -> {k + " (当前)" if k == chat.get_chat_preset_key() else k}' for k in chat_presets_dict.keys()])
+    presets_show_text = '\n'.join([f'  -> {k + " (当前)" if k == chat.preset_key else k}' for k in chat_presets_dict.keys()])
     if option_dict.get('admin'):
         return {
             'msg': (
                 f"当前可用人格预设有:\n"
                 f"{presets_show_text}\n"
                 f"=======================\n"
                 f"+ 使用预设: rg set <预设名> <-global?>\n"
@@ -131,15 +132,15 @@
                 f"* 更多帮助请访问: NG指令文档\n"
                 f"Tip: <人格信息> 是一段第三人称的人设说明(建议不超过200字)\n"
             )
         }
     else:
         return {
             'msg': (
-                f"会话: {chat.get_chat_key()} [{'启用' if chat.is_enable else '禁用'}]\n"
+                f"会话: {chat.chat_key} [{'启用' if chat.is_enable else '禁用'}]\n"
                 f"当前可用人格预设有:\n"
                 f"{presets_show_text}\n"
             )
         }
 
 @cmd.register(route='rg/set', params=['preset_key', 'preset_intro'])
 def _(option_dict, param_dict, chat:Chat, chat_presets_dict:dict):
@@ -302,58 +303,70 @@
 def _(option_dict, param_dict, chat:Chat, chat_presets_dict:dict):
     if option_dict.get('global'):
         ChatManager.instance.toggle_chat_for_all(enabled=True)
         return {'msg': f"启用所有会话 (￣▽￣)-ok!"}
     elif option_dict.get('target'):
         target_chat_key = option_dict.get('target')
         target_chat = ChatManager.instance.get_chat(chat_key=target_chat_key)
-        target_chat.toggle_chat(enabled=True)
-        return {'msg': f"启用会话: {target_chat_key} (￣▽￣)-ok!"}
+        if target_chat:
+            target_chat.toggle_chat(enabled=True)
+            return {'msg': f"启用会话: {target_chat_key} (￣▽￣)-ok!"}
+        else:
+            return {'error': f"找不到会话: {target_chat_key}"}
     else:
         chat.toggle_chat(enabled=True)
         return {'msg': f"启用当前会话 (￣▽￣)-ok!"}
 
 @cmd.register(route='rg/off')
 def _(option_dict, param_dict, chat:Chat, chat_presets_dict:dict):
     if option_dict.get('global'):
         ChatManager.instance.toggle_chat_for_all(enabled=False)
         return {'msg': f"禁用所有会话 (￣▽￣)-ok!"}
     elif option_dict.get('target'):
         target_chat_key = option_dict.get('target')
         target_chat = ChatManager.instance.get_chat(chat_key=target_chat_key)
-        target_chat.toggle_chat(enabled=False)
-        return {'msg': f"禁用会话: {target_chat_key} (￣▽￣)-ok!"}
+        if target_chat:
+            target_chat.toggle_chat(enabled=False)
+            return {'msg': f"禁用会话: {target_chat_key} (￣▽￣)-ok!"}
+        else:
+            return {'error': f"找不到会话: {target_chat_key}"}
     else:
         chat.toggle_chat(enabled=False)
         return {'msg': f"禁用当前会话 (￣▽￣)-ok!"}
 
 @cmd.register(route='rg/lock')
 def _(option_dict, param_dict, chat:Chat, chat_presets_dict:dict):
     if option_dict.get('global'):
         ChatManager.instance.toggle_auto_switch_for_all(enabled=False)
         return {'msg': f"锁定所有会话 (￣▽￣)-ok!"}
     elif option_dict.get('target'):
         target_chat_key = option_dict.get('target')
         target_chat = ChatManager.instance.get_chat(chat_key=target_chat_key)
-        target_chat.toggle_auto_switch(enabled=False)
-        return {'msg': f"锁定会话: {target_chat_key} (￣▽￣)-ok!"}
+        if target_chat:
+            target_chat.toggle_auto_switch(enabled=False)
+            return {'msg': f"锁定会话: {target_chat_key} (￣▽￣)-ok!"}
+        else:
+            return {'error': f"找不到会话: {target_chat_key}"}
     else:
         chat.toggle_auto_switch(enabled=False)
         return {'msg': f"锁定当前会话 (￣▽￣)-ok!"}
 
 @cmd.register(route='rg/unlock')
 def _(option_dict, param_dict, chat:Chat, chat_presets_dict:dict):
     if option_dict.get('global'):
         ChatManager.instance.toggle_auto_switch_for_all(enabled=True)
         return {'msg': f"解锁所有会话 (￣▽￣)-ok!"}
     elif option_dict.get('target'):
         target_chat_key = option_dict.get('target')
         target_chat = ChatManager.instance.get_chat(chat_key=target_chat_key)
-        target_chat.toggle_auto_switch(enabled=True)
-        return {'msg': f"解锁会话: {target_chat_key} (￣▽￣)-ok!"}
+        if target_chat:
+            target_chat.toggle_auto_switch(enabled=True)
+            return {'msg': f"解锁会话: {target_chat_key} (￣▽￣)-ok!"}
+        else:
+            return {'error': f"找不到会话: {target_chat_key}"}
     else:
         chat.toggle_auto_switch(enabled=True)
         return {'msg': f"解锁当前会话 (￣▽￣)-ok!"}
 
 @cmd.register(route='rg/ext')
 def _(option_dict, param_dict, chat:Chat, chat_presets_dict:dict):
     ext_info:str = ''
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/config.py` & `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ﻿from typing import Any, Dict, List
-import nonebot
+from nonebot.config import Config as NBConfig
 from pydantic import BaseModel, Extra
 from nonebot import get_driver
 from .logger import logger
 import yaml
 from pathlib import Path
 
-class GlobalConfig(nonebot.Config, extra=Extra.ignore):
+class GlobalConfig(NBConfig, extra=Extra.ignore):
     """Plugin Config Here"""
     ng_config_path: str = "config/naturel_gpt_config.yml"
     ng_dev_mode: bool = False
 
 class PresetConfig(BaseModel, extra=Extra.ignore):
     """人格预设配置项"""
     preset_key:str
@@ -28,14 +28,16 @@
 
 class Config(BaseModel, extra=Extra.ignore):
     """ng 配置数据，默认保存为 naturel_gpt_config.yml"""
     OPENAI_API_KEYS: List[str]
     """OpenAI API Key 列表"""
     OPENAI_TIMEOUT: int
     """OpenAI 请求超时时间"""
+    REPLY_THROTTLE_TIME: int
+    """回复间隔节流时间"""
     PRESETS: Dict[str, PresetConfig]
     """默认人格预设"""
     IGNORE_PREFIX: str
     """忽略前缀 以该前缀开头的消息将不会被处理"""
     CHAT_MODEL: str
     """OpenAI 模型"""
     CHAT_TOP_P: int
@@ -157,14 +159,15 @@
 # 配置文件模板(把全部默认值写到Config定义里比较乱，因此保留此默认值对象,作为真实的默认值)
 CONFIG_TEMPLATE = {
     "OPENAI_API_KEYS": [    # OpenAI API Key 列表
         'sk-xxxxxxxxxxxxx',
         'sk-xxxxxxxxxxxxx',
     ],
     "OPENAI_TIMEOUT": 60,   # OpenAI 请求超时时间
+    "REPLY_THROTTLE_TIME": 3,   # 回复间隔节流时间
     'OPENAI_PROXY_SERVER': '',  # 请求OpenAI的代理服务器
     "PRESETS": {
         "白羽": {
             'preset_key': '白羽',  # 人格名称
             'is_locked': True,  # 是否锁定人格，锁定后无法编辑人格
             'is_default': True,  # 是否为默认人格
             "is_only_private": False,
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/Extension.py` & `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/Extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ﻿import importlib
 import time
 import os
 import sys
 import shutil
 import nonebot
-from typing import TYPE_CHECKING, Any, Dict
+from typing import TYPE_CHECKING, Any, Dict, Type, Union
 
 if TYPE_CHECKING:
     from loguru import Record
 
 
 def __path(record: "Record"):
     record["name"] = "NG聊天扩展"
@@ -25,15 +25,15 @@
         self._ext_config = ext_config
         self._custom_config = custom_config
 
     async def run(self, arg_dict: dict, ctx_data: dict) -> dict:
         """ 扩展运行 """
         raise NotImplementedError
 
-    async def call(self, arg_dict, ctx_data) -> dict:
+    async def call(self, arg_dict, ctx_data) -> Union[str, dict]:
         """ 调用扩展 """
         self._call_time -= 1
         if self._call_time < 0:
             return {}
         else:
             return await self.run(arg_dict, ctx_data)
 
@@ -115,25 +115,25 @@
                 file_name = tmpExt.get("EXT_NAME") + '.py'  # 扩展模块文件名
 
                 # 复制扩展模块文件到ext_cache文件夹下
                 shutil.copyfile(f'{ext_path}{file_name}',
                                 f'ext_cache/{file_name}')
                 time.sleep(0.3)  # 等待文件复制完成
                 # 从 ext_cache 文件夹下导入扩展模块
-                CustomExtension: Extension = getattr(
+                CustomExtension: type = getattr( # Type[CustomExtension]
                     importlib.import_module(
                         f'ext_cache.{tmpExt.get("EXT_NAME")}'),
                     'CustomExtension')
                 time.sleep(0.3)  # 等待文件导入完成
 
                 ext_config_dict = tmpExt.get("EXT_CONFIG") if isinstance(
                     tmpExt.get("EXT_CONFIG"), dict) else {}
 
                 # 加载扩展模块并实例化
-                ext = CustomExtension(ext_config_dict)  # type: ignore
+                ext = CustomExtension(ext_config_dict)
                 # 将扩展模块添加到全局扩展模块字典中
                 global_extensions[ext.get_config().get('name').lower()] = ext
                 logger.info(f"加载扩展模块 {tmpExt.get('EXT_NAME')} 成功！")
             except Exception as e:
                 logger.error(
                     f"加载扩展模块 \"{tmpExt.get('EXT_NAME')}\" 失败 | 原因: {e}")
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/matcher.py` & `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/matcher.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,40 @@
 ﻿import asyncio
-import json
 import random
 import re
 import time
 import os
 import traceback
-from typing import Awaitable, List, Dict, Callable, Optional, Set, Tuple
-from nonebot import get_driver
+from typing import Awaitable, List, Dict, Callable, Optional, Set, Tuple, Type
 from nonebot import on_command, on_message, on_notice
 from .logger import logger
-from nonebot.params import CommandArg, Matcher, Event
-from nonebot.adapters.onebot.v11 import Bot, Message, MessageEvent, PrivateMessageEvent, GroupMessageEvent, MessageSegment, GroupIncreaseNoticeEvent
+from nonebot.params import CommandArg
+from nonebot.matcher import Matcher
+from nonebot.adapters import Bot, Event
+from nonebot.adapters.onebot.v11 import Message, MessageEvent, PrivateMessageEvent, GroupMessageEvent, MessageSegment, GroupIncreaseNoticeEvent
 
 from .config import *
 from .utils import *
 from .chat import Chat
 from .persistent_data_manager import PersistentDataManager
 from .chat_manager import ChatManager
-from .Extension import Extension, global_extensions
+from .Extension import global_extensions
 from .openai_func import TextGenerator
-from .command_func import CommandManager, cmd
+from .command_func import cmd
+from .MCrcon.mcrcon import MCRcon   # fork from: https://github.com/Uncaught-Exceptions/MCRcon
 
 try:
     import nonebot_plugin_htmlrender
     from .text_func import text_to_img
 except:
     logger.warning('未安装 nonebot_plugin_htmlrender 插件，无法使用 text_to_img')
     config.ENABLE_MSG_TO_IMG = False
     config.ENABLE_COMMAND_TO_IMG = False
 
-if config.ENABLE_MC_CONNECT:
-    try:
-        from nonebot.adapters.spigot import Bot as SpigotBot
-        from nonebot.adapters.spigot import Event as SpigotEvent
-        from .MCrcon.mcrcon import MCRcon   # fork from: https://github.com/Uncaught-Exceptions/MCRcon
-    except:
-        logger.warning('未安装 nonebot_plugin_spigot 适配器，无法使用 SpigotBot')
-        config.ENABLE_MC_CONNECT = False
-
-
-permission_check_func:Callable[[Matcher, MessageEvent, Bot, str, str], Awaitable[Tuple[bool,str]]] = None
+permission_check_func:Callable[[Matcher, Event, Bot, Optional[str], str], Awaitable[Tuple[bool,Optional[str]]]]
 is_progress:bool = False
 
 msg_sent_set:Set[str] = set() # bot 自己发送的消息
 
 """消息发送钩子，用于记录自己发送的消息(默认不开启，只有在用户自定义了message_sent事件之后message_sent事件才会被发送到 on_message 回调)"""
 # @Bot.on_called_api
 async def handle_group_message_sent(bot: Bot, exception: Optional[Exception], api: str, data: Dict[str, Any], result: Any):
@@ -51,30 +42,30 @@
     if result and (api in ['send_msg', 'send_group_msg', 'send_private_msg']):
         msg_id = result.get('message_id', None)
         if msg_id:
             msg_sent_set.add(f"{bot.self_id}_{msg_id}")
 
 """ ======== 注册消息响应器 ======== """
 # 注册qq消息响应器 收到任意消息时触发
-matcher:Matcher = on_message(priority=config.NG_MSG_PRIORITY, block=config.NG_BLOCK_OTHERS)
+matcher:Type[Matcher] = on_message(priority=config.NG_MSG_PRIORITY, block=config.NG_BLOCK_OTHERS)
 @matcher.handle()
 async def handler(matcher_:Matcher, event: MessageEvent, bot:Bot) -> None:
     global msg_sent_set
     if event.post_type == 'message_sent': # 通过bot.send发送的消息不处理
         msg_key = f"{bot.self_id}_{event.message_id}"
         if msg_key in msg_sent_set:
             msg_sent_set.remove(msg_key)
             return
         
     if len(msg_sent_set) > 10:
         if config.DEBUG_LEVEL > 0: logger.warning(f"累积的待处理的自己发送消息数量为 {len(msg_sent_set)}, 请检查逻辑是否有错误")
         msg_sent_set.clear()
     
     # 处理消息前先检查权限
-    (permit_success, _) = await permission_check_func(matcher=matcher_, event=event, bot=bot, cmd=None, type='message')
+    (permit_success, _) = await permission_check_func(matcher_, event, bot, None, 'message')
     if not permit_success:
         return
     
     # 判断用户账号是否被屏蔽
     if event.get_user_id() in config.FORBIDDEN_USERS:
         if config.DEBUG_LEVEL > 0: logger.info(f"用户 {event.get_user_id()} 被屏蔽，拒绝处理消息")
         return
@@ -120,130 +111,26 @@
         event.is_tome() or wake_up,
         matcher,
         chat_type,
         chat_key,
         sender_name,
     )
 
-# 注册MC消息响应器
-if config.ENABLE_MC_CONNECT:
-    mc_matcher:Matcher = on_message(priority=config.NG_MSG_PRIORITY-2, block=False)
-    @mc_matcher.handle()
-    async def handler(matcher_:Matcher, event: SpigotEvent, bot:SpigotBot) -> None:
-        # 处理消息前先检查权限
-        (permit_success, _) = await permission_check_func(matcher=matcher_, event=event, bot=bot, cmd=None, type='message')
-        if not permit_success:
-            return
-
-        try:
-            ejson_dict = json.loads(event.json())
-            server_from = event.server_name
-            sender_name = ejson_dict['player']['nickname']
-            chat_text = str(event.get_message())
-        except Exception as e:
-            logger.warning(f"[MC: {server_from}] 获取消息发送者信息失败: {e} 跳过处理...")
-            return
-
-        # 判断用户账号是否被屏蔽
-        if sender_name in config.FORBIDDEN_USERS:
-            if config.DEBUG_LEVEL > 0: logger.info(f"用户 {sender_name} 被屏蔽，拒绝处理消息")
-            return
-
-        resTmplate = (  # 测试用，获取消息的相关信息
-            f"收到消息: {chat_text}"
-            f"\n消息描述: {event.get_event_description()}"
-            f"\n发送者: {sender_name}"
-            f"\n消息来源: {server_from}"
-            f"\nJSON: {event.json()}"
-        )
-        if config.DEBUG_LEVEL > 1: logger.info(resTmplate)
-
-        # 如果是忽略前缀 或者 消息为空，则跳过处理
-        if chat_text.strip().startswith(config.IGNORE_PREFIX) or not chat_text:   
-            if config.DEBUG_LEVEL > 1: logger.info("忽略前缀或消息为空，跳过处理...") # 纯图片消息也会被判定为空消息
-            return
-
-        # 判断消息来源
-        if isinstance(event, SpigotEvent):
-            chat_key = 'MC_Server_' + server_from
-            chat_type = 'server'
-        else:
-            if config.DEBUG_LEVEL > 0: logger.info("未知消息来源: " + event.get_session_id())
-            return
-
-        #region 指令处理分支 (由于Spigot适配器似乎不支持指令，所以整合进消息响应流)
-        command_prefix_check = False
-        for prefix in config.MC_COMMAND_PREFIX:
-            if chat_text.startswith(prefix):
-                command_prefix_check = True
-                raw_cmd = chat_text[len(prefix):].strip()
-                break
-
-        if command_prefix_check:
-            global is_progress  # 是否产生编辑进度
-            is_progress = False
-            if config.DEBUG_LEVEL > 0: logger.info(f"接收到指令: {raw_cmd} | 来源: {chat_key} (MC) | 发送者: {sender_name})")
-            # 判断是否是禁止使用的用户
-            if sender_name in config.FORBIDDEN_USERS:
-                await mc_matcher.finish(f"您的账号({sender_name})已被禁用，请联系管理员。")
-
-            chat:Chat = ChatManager.instance.get_or_create_chat(chat_key=chat_key)
-            chat_presets_dict = chat.chat_data.preset_datas
-
-            # 执行命令前先检查权限
-            if sender_name not in config.ADMIN_USERID:
-                await mc_matcher.finish("对不起！你没有权限进行此操作 ＞﹏＜")
-
-            # 执行命令
-            res = cmd.execute(
-                chat=chat,
-                command=raw_cmd,
-                chat_presets_dict=chat_presets_dict,
-            )
-
-            if res:
-                if res.get('msg'):     # 如果有返回消息则发送
-                    await mc_matcher.send(res.get('msg'))  
-                elif res.get('error'):
-                    await mc_matcher.finish(f"执行命令时出现错误: {res.get('error')}")  # 如果有返回错误则发送s
-
-            else:
-                await mc_matcher.finish("输入的命令好像有点问题呢... 请检查下再试试吧！ ╮(>_<)╭")
-
-            if res.get('is_progress'): # 如果有编辑进度，进行数据保存
-                # 更新所有全局预设到会话预设中
-                if config.DEBUG_LEVEL > 0: logger.info(f"用户: {sender_name} 进行了人格预设编辑: {cmd}")
-                PersistentDataManager.instance.save_to_file()  # 保存数据
-            return
-        #endregion
-
-        # 进行消息响应
-        await do_msg_response(
-            sender_name,
-            chat_text,
-            event.is_tome(),
-            mc_matcher,
-            chat_type,
-            chat_key,
-            sender_name,
-        )
-
-
 """ ======== 注册通知响应器 ======== """
 # 欢迎新成员通知响应器
-welcome:Matcher = on_notice(priority=20, block=False)
+welcome:Type[Matcher] = on_notice(priority=20, block=False)
 @welcome.handle()  # 监听 welcom
 async def _(matcher_:Matcher, event: GroupIncreaseNoticeEvent, bot:Bot):  # event: GroupIncreaseNoticeEvent  群成员增加事件
     if config.DEBUG_LEVEL > 0: logger.info(f"收到通知: {event}")
 
     if not config.REPLY_ON_WELCOME:  # 如果不回复欢迎消息，则跳过处理
         return
     
     # 处理通知前先检查权限
-    (permit_success, _) = await permission_check_func(matcher=matcher_, event=event,bot=bot,cmd=None,type='notice')
+    (permit_success, _) = await permission_check_func(matcher_, event, bot,None,'notice')
     if not permit_success:
         return
 
     if isinstance(event, GroupIncreaseNoticeEvent): # 群成员增加通知
         chat_key = 'group_' + event.get_session_id().split("_")[1]
         chat_type = 'group'
     else:
@@ -255,83 +142,31 @@
         f"\n通知来源: {event.get_user_id()}"
         f"\n是否to-me: {event.is_tome()}"
         f"\nDict: {event.dict()}"
         f"\nJSON: {event.json()}"
     )
     if config.DEBUG_LEVEL > 0: logger.info(resTmplate)
 
-    user_name = await get_user_name(event=event, bot=bot, user_id=event.get_user_id()) or f'qq:{event.get_user_id()}'
+    user_name = await get_user_name(event=event, bot=bot, user_id=int(event.get_user_id())) or f'qq:{event.get_user_id()}'
 
     # 进行消息响应
     await do_msg_response(
         event.get_user_id(),
         f'{user_name} has joined the group, welcome!',
         event.is_tome(),
         welcome,
         chat_type,
         chat_key,
         '[System]',
         True
     )
 
-# 注册MC通知响应器
-if config.ENABLE_MC_CONNECT:
-    mc_notice_matcher:Matcher = on_notice(priority=20, block=False)
-    @mc_notice_matcher.handle()
-    async def handler(matcher_:Matcher, event: SpigotEvent, bot:SpigotBot) -> None:
-        try:
-            server_from = event.server_name
-            event_description = event.get_event_description()
-        except Exception as e:
-            logger.warning(f"[MC: {server_from}] 获取消息发送者信息失败: {e} 跳过处理...")
-            return
-
-        # 判断消息来源
-        if isinstance(event, SpigotEvent):
-            chat_key = 'MC_Server_' + server_from
-            chat_type = 'server'
-        else:
-            if config.DEBUG_LEVEL > 0: logger.info("未知消息来源: " + event.get_session_id())
-            return
-        
-        # 使用正则从消息："Notice {event_name} from {user_name}@[Server:{self.server_name}]: {event_name}" 中提取出玩家名和事件名(Join/Leave)
-        try:
-            event_name = event_description.split(']:')[1].strip()
-            user_name = re.search(r'from (.+?)@', event_description).group(1)
-        except Exception as e:
-            logger.warning(f"[MC: {server_from}] 正则提取消息内容失败: {e} 跳过处理...")
-            return
-        
-        wake_up = False
-
-        if event_name == 'Join':
-            notice_text = f'{user_name} 加入了服务器!'
-            wake_up = True
-        elif event_name == 'Quit':
-            notice_text = f'{user_name} 离开了服务器!'
-        elif event_name == 'Death':
-            notice_text = f'{user_name} 死于意外!'
-            wake_up = True
-
-        # 进行消息响应
-        await do_msg_response(
-            user_name,
-            notice_text,
-            False,
-            mc_notice_matcher,
-            chat_type,
-            chat_key,
-            '[Minecraft Server]',
-            wake_up
-        )
-
-
 """ ======== 注册指令响应器 ======== """
 # QQ:人格设定指令 用于设定人格的相关参数
-identity:Matcher = on_command("identity", aliases={"人格设定", "人格", "rg"}, rule=to_me(), priority=config.NG_MSG_PRIORITY - 1, block=True)
+identity:Type[Matcher] = on_command("identity", aliases={"人格设定", "人格", "rg"}, rule=to_me(), priority=config.NG_MSG_PRIORITY - 1, block=True)
 @identity.handle()
 async def _(matcher_:Matcher, event: MessageEvent, bot:Bot, arg: Message = CommandArg()):
     global is_progress  # 是否产生编辑进度
     is_progress = False
     # 判断是否是禁止使用的用户
     if event.get_user_id() in config.FORBIDDEN_USERS:
         await identity.finish(f"您的账号({event.get_user_id()})已被禁用，请联系管理员。")
@@ -347,18 +182,18 @@
 
     chat:Chat = ChatManager.instance.get_or_create_chat(chat_key=chat_key)
     chat_presets_dict = chat.chat_data.preset_datas
 
     raw_cmd:str = arg.extract_plain_text()
     if config.DEBUG_LEVEL > 0: logger.info(f"接收到指令: {raw_cmd} | 来源: {chat_key}")
     
-    presets_show_text = '\n'.join([f'  -> {k + " (当前)" if k == chat.get_chat_preset_key() else k}' for k in chat_presets_dict.keys()])
+    presets_show_text = '\n'.join([f'  -> {k + " (当前)" if k == chat.preset_key else k}' for k in chat_presets_dict.keys()])
 
     # 执行命令前先检查权限
-    (permit_success, permit_msg) = await permission_check_func(matcher=matcher_, event=event,bot=bot,cmd=raw_cmd,type='cmd')
+    (permit_success, permit_msg) = await permission_check_func(matcher_, event,bot,raw_cmd,'cmd')
     if not permit_success:
         await identity.finish(permit_msg if permit_msg else "对不起！你没有权限进行此操作 ＞﹏＜")
 
     # 执行命令 *取消注释下列行以启用新的命令执行器*
     res = cmd.execute(
         chat=chat,
         command='rg '+ raw_cmd,
@@ -367,32 +202,33 @@
 
     if res:
         if res.get('msg'):     # 如果有返回消息则发送
             if config.ENABLE_COMMAND_TO_IMG:
                 img = await text_to_img(res.get('msg'))
                 await identity.send(MessageSegment.image(img))
             else:
-                await identity.send(res.get('msg'))  
+                await identity.send(str(res.get('msg')))
         elif res.get('error'):
             await identity.finish(f"执行命令时出现错误: {res.get('error')}")  # 如果有返回错误则发送s
 
     else:
         await identity.finish("输入的命令好像有点问题呢... 请检查下再试试吧！ ╮(>_<)╭")
 
     if res.get('is_progress'): # 如果有编辑进度，进行数据保存
         # 更新所有全局预设到会话预设中
         if config.DEBUG_LEVEL > 0: logger.info(f"用户: {event.get_user_id()} 进行了人格预设编辑: {cmd}")
         PersistentDataManager.instance.save_to_file()  # 保存数据
     return
 
 
 """ ======== 消息响应方法 ======== """
-async def do_msg_response(trigger_userid:str, trigger_text:str, is_tome:bool, matcher: Matcher, chat_type: str, chat_key: str, sender_name: str = None, wake_up: bool = False, loop_times=0, loop_data={}):
+async def do_msg_response(trigger_userid:str, trigger_text:str, is_tome:bool, matcher: Type[Matcher], chat_type: str, chat_key: str, sender_name: Optional[str] = None, wake_up: bool = False, loop_times=0, loop_data={}):
     """消息响应方法"""
 
+    sender_name = sender_name or 'anonymous'
     chat:Chat = ChatManager.instance.get_or_create_chat(chat_key=chat_key)
 
     # 判断对话是否被禁用
     if not chat.is_enable:
         if config.DEBUG_LEVEL > 1: logger.info("对话已被禁用，跳过处理...")
         return
 
@@ -409,36 +245,36 @@
             break
 
     # 随机回复判断
     if random.random() < config.RANDOM_CHAT_PROBABILITY:
         wake_up = True
 
     # 其它人格唤醒判断
-    if chat.get_chat_preset_key().lower() not in trigger_text.lower() and chat.enable_auto_switch_identity:
+    if chat.preset_key.lower() not in trigger_text.lower() and chat.enable_auto_switch_identity:
         for preset_key in chat.preset_keys:
             if preset_key.lower() in trigger_text.lower():
                 chat.change_presettings(preset_key)
                 logger.info(f"检测到 {preset_key} 的唤醒词，切换到 {preset_key} 的人格")
                 if chat_type != 'server':
                     await matcher.send(f'[NG] 已切换到 {preset_key} (￣▽￣)-ok !')
                 wake_up = True
                 break
 
-    current_preset_key = chat.get_chat_preset_key()
+    current_preset_key = chat.preset_key
 
     # 判断是否需要回复
     if (    # 如果不是 bot 相关的信息，则直接返回
         wake_up or \
-        (config.REPLY_ON_NAME_MENTION and (chat.get_chat_preset_key().lower() in trigger_text.lower())) or \
+        (config.REPLY_ON_NAME_MENTION and (chat.preset_key.lower() in trigger_text.lower())) or \
         (config.REPLY_ON_AT and is_tome)
     ):
         # 更新全局对话历史记录
         # chat.update_chat_history_row(sender=sender_name, msg=trigger_text, require_summary=True)
         await chat.update_chat_history_row(sender=sender_name,
-                                    msg=f"@{chat.get_chat_preset_key()} {trigger_text}" if is_tome and chat_type=='group' else trigger_text,
+                                    msg=f"@{chat.preset_key} {trigger_text}" if is_tome and chat_type=='group' else trigger_text,
                                     require_summary=False)
         logger.info("符合 bot 发言条件，进行回复...")
     else:
         if config.CHAT_ENABLE_RECORD_ORTHER:
             await chat.update_chat_history_row(sender=sender_name, msg=trigger_text, require_summary=False)
             if config.DEBUG_LEVEL > 1: logger.info("不是 bot 相关的信息，记录但不进行回复")
         else:
@@ -446,16 +282,24 @@
         return
     
     wake_up = False # 进入对话流程，重置唤醒状态
 
     # 记录对用户的对话信息
     await chat.update_chat_history_row_for_user(sender=sender_name, msg=trigger_text, userid=trigger_userid, username=sender_name, require_summary=False)
 
-    if chat.get_chat_preset_key() != current_preset_key:
-        if config.DEBUG_LEVEL > 0: logger.warning(f'等待OpenAI请求返回的过程中人格预设由[{current_preset_key}]切换为[{chat.get_chat_preset_key()}],当前消息不再继续响应.1')
+    if chat.preset_key != current_preset_key:
+        if config.DEBUG_LEVEL > 0: logger.warning(f'等待OpenAI请求返回的过程中人格预设由[{current_preset_key}]切换为[{chat.preset_key}],当前消息不再继续响应.1')
+        return
+    
+    # 节流判断 接收到消息后等待一段时间，如果在这段时间内再次收到消息，则跳过响应处理
+    # 效果表现为：如果在一段时间内连续收到消息，则只响应最后一条消息
+    last_recv_time = chat.last_msg_time
+    await asyncio.sleep(config.REPLY_THROTTLE_TIME)
+    if last_recv_time != chat.last_msg_time: # 如果最后一条消息时间不一致，说明在节流时间内收到了新消息，跳过处理
+        if config.DEBUG_LEVEL > 0: logger.info(f'节流时间内收到新消息，跳过处理...')
         return
     
     # 主动聊天参与逻辑 *待定方案
     # 达到一定兴趣阈值后，开始进行一次启动发言准备 收集特定条数的对话历史作为发言参考
     # 启动发言后，一段时间内兴趣值逐渐下降，如果随后被呼叫，则兴趣值提升
     # 监测对话历史中是否有足够的话题参与度，如果有，则继续提高话题参与度，否则，降低话题参与度
     # 兴趣值影响发言频率，兴趣值越高，发言频率越高
@@ -475,32 +319,32 @@
         # 保存 prompt 模板到日志文件
         with open(os.path.join(config.NG_LOG_PATH, f"{chat_key}.{time.strftime('%Y-%m-%d %H-%M-%S')}.prompt.log"), 'a', encoding='utf-8') as f:
             f.write(f"prompt 模板: \n{log_prompt_template}\n")
         logger.info(f"对话 prompt 模板已保存到日志文件: {chat_key}.{time.strftime('%Y-%m-%d %H-%M-%S')}.prompt.log")
 
     time_before_request = time.time()
     tg = TextGenerator.instance
-    raw_res, success = await tg.get_response(prompt=prompt_template, type='chat', custom={'bot_name': chat.get_chat_preset_key(), 'sender_name': sender_name})  # 生成对话结果
+    raw_res, success = await tg.get_response(prompt=prompt_template, type='chat', custom={'bot_name': chat.preset_key, 'sender_name': sender_name})  # 生成对话结果
     if not success:  # 如果生成对话结果失败，则直接返回
         logger.warning("生成对话结果失败，跳过处理...")
         await matcher.finish(raw_res)
 
     # 输出对话原始响应结果
     if config.DEBUG_LEVEL > 0: logger.info(f"原始回应: {raw_res}")
 
     if time.time() - time_before_request > config.OPENAI_TIMEOUT:
         logger.warning(f'OpenAI响应超过timeout值[{config.OPENAI_TIMEOUT}]，停止处理')
         return
 
-    if chat.get_chat_preset_key() != current_preset_key:
-        if config.DEBUG_LEVEL > 0: logger.warning(f'等待OpenAI响应返回的过程中人格预设由[{current_preset_key}]切换为[{chat.get_chat_preset_key()}],当前消息不再继续处理.2')
+    if chat.preset_key != current_preset_key:
+        if config.DEBUG_LEVEL > 0: logger.warning(f'等待OpenAI响应返回的过程中人格预设由[{current_preset_key}]切换为[{chat.preset_key}],当前消息不再继续处理.2')
         return
 
     # 用于存储最终回复顺序内容的列表
-    reply_list = []
+    reply_list:List[Union[str, dict]] = []
 
     # 预检一次响应内容，如果响应内容中包含了需要打断的扩展调用指令，则直接截断原始响应中该扩展调用指令后的内容
     pre_check_calls = re.findall(r"/#(.+?)#/", raw_res, re.S)
     if pre_check_calls:
         for call_str in pre_check_calls:
             ext_name, *ext_args = call_str.split('&')
             ext_name = ext_name.strip().lower()
@@ -520,15 +364,15 @@
     # 分割对话结果提取出所有 "/#扩展名&参数1&参数2#/" 格式的扩展调用指令 参数之间用&分隔 多行匹配
     ext_calls = re.findall(r"/.?#(.+?)#.?/", talk_res, re.S)
 
     # 对分割后的对话根据 '*;' 进行分割，表示对话结果中的分句，处理结果为列表，其中每个元素为一句话
     if config.NG_ENABLE_MSG_SPLIT:
         # 提取后去除所有扩展调用指令并切分信息，剩余部分为对话结果 多行匹配
         talk_res = re.sub(r"/.?#(.+?)#.?/", '*;', talk_res)
-        reply_list = talk_res.split('*;')
+        reply_list.extend(talk_res.split('*;'))
     else:
         # 提取后去除所有扩展调用指令，剩余部分为对话结果 多行匹配
         talk_res = re.sub(r"/.?#(.+?)#.?/", '', talk_res)
         reply_list.append(talk_res)
 
     # if config.DEBUG_LEVEL > 0: logger.info("分割响应结果: " + str(reply_list))
 
@@ -540,144 +384,167 @@
     for ext_call_str in ext_calls:  
         ext_name, *ext_args = ext_call_str.split('&')
         ext_name = ext_name.strip().lower()
         if ext_name in global_extensions.keys():
             # 提取出扩展调用指令中的参数为字典
             ext_args_dict:dict = {}
             # 按照参数顺序依次提取参数值
-            for arg_name in global_extensions[ext_name].get_config().get('arguments').keys():
-                if len(ext_args) > 0:
-                    ext_args_dict[arg_name] = ext_args.pop(0)
-                else:
-                    ext_args_dict[arg_name] = None
+            arguments = global_extensions[ext_name].get_config().get('arguments')
+            if arguments and isinstance(arguments, dict):
+                for arg_name in arguments.keys():
+                    if len(ext_args) > 0:
+                        ext_args_dict[arg_name] = ext_args.pop(0)
+                    else:
+                        ext_args_dict[arg_name] = None
 
             logger.info(f"检测到扩展调用指令: {ext_name} {ext_args_dict} | 正在调用扩展模块...")
             try:    # 调用扩展的call方法
-                ext_res:dict = await global_extensions[ext_name].call(ext_args_dict, {
-                    'bot_name': chat.get_chat_preset_key(),
+                ext_res = await global_extensions[ext_name].call(ext_args_dict, {
+                    'bot_name': chat.preset_key,
                     'user_send_raw_text': trigger_text,
                     'bot_send_raw_text': raw_res
                 })
                 if config.DEBUG_LEVEL > 0: logger.info(f"扩展 {ext_name} 返回结果: {ext_res}")
                 if ext_res is not None:
                     # 将扩展返回的结果插入到回复列表的最后
                     reply_list.append(ext_res)
             except Exception as e:
                 logger.error(f"调用扩展 {ext_name} 时发生错误: {e}")
                 if config.DEBUG_LEVEL > 0: logger.error(f"[扩展 {ext_name}] 错误详情: {traceback.format_exc()}")
-                ext_res = None
+                ext_res = {}
                 # 将错误的调用指令从原始回复中去除，避免bot从上下文中学习到错误的指令用法
                 raw_res = re.sub(r"/.?#(.+?)#.?/", '', raw_res)
         else:
             logger.error(f"未找到扩展 {ext_name}，跳过调用...")
             # 将错误的调用指令从原始回复中去除，避免bot从上下文中学习到错误的指令用法
             raw_res = re.sub(r"/.?#(.+?)#.?/", '', raw_res)
 
     # # 代码块插入到回复列表的最后
     # for code_block in code_blocks:
     #     reply_list.append({'code_block': code_block})
 
     if config.DEBUG_LEVEL > 0: logger.info(f"回复序列内容: {reply_list}")
 
     # 回复前缀
-    reply_prefix = f'<{chat.get_chat_preset_key()}> ' if (chat_type == 'server') else ''
+    reply_prefix = f'<{chat.preset_key}> ' if (chat_type == 'server') else ''
 
     res_times = config.NG_MAX_RESPONSE_PER_MSG  # 获取每条消息最大回复次数
     # 根据回复内容列表逐条发送回复
     for idx, reply in enumerate(reply_list):
         # 判断回复内容是否为str
-        if isinstance(reply, str) and reply.strip():
+        if isinstance(reply, str):
             # 判断文本内容是否为纯符号(包括空格，换行、英文标点、中文标点)并且长度小于3
-            if re.match(r'^[^\u4e00-\u9fa5\w]{1}$', reply.strip()):
-                if config.DEBUG_LEVEL > 0: logger.info(f"检测到纯符号文本: {reply.strip()}，跳过发送...")
+            reply_text = str(reply).strip()
+            if re.match(r'^[^\u4e00-\u9fa5\w]{1}$', reply_text) or len(reply_text) < 1:
+                if config.DEBUG_LEVEL > 0: logger.info(f"检测到纯符号或空文本: {reply_text}，跳过发送...")
                 continue
             if config.ENABLE_MSG_TO_IMG:
-                img = await text_to_img(reply.strip())
+                img = await text_to_img(reply_text)
                 await matcher.send(MessageSegment.image(img))
             else:
-                await matcher.send(f"{reply_prefix}{reply.strip()}")
-        else:
+                await matcher.send(f"{reply_prefix}{reply_text}")
+        elif isinstance(reply, dict):
             for key in reply:   # 遍历回复内容类型字典
-                if key == 'text' and reply.get(key) and reply.get(key).strip(): # 发送普通文本
+                if not reply.get(key):
+                    continue
+                
+                reply_content = reply.get(key)
+                reply_text = str(reply_content).strip() if isinstance(reply_content, str) else ''
+                if key == 'text': # 发送普通文本
                     # 判断文本内容是否为纯符号(包括空格，换行、英文标点、中文标点)并且长度为1
-                    if re.match(r'^[^\u4e00-\u9fa5\w]{1}$', reply.get(key).strip()):
-                        if config.DEBUG_LEVEL > 0: logger.info(f"检测到纯符号文本: {reply.get(key).strip()}，跳过发送...")
+                    if re.match(r'^[^\u4e00-\u9fa5\w]{1}$', reply_text):
+                        if config.DEBUG_LEVEL > 0: logger.info(f"检测到纯符号文本: {reply_text}，跳过发送...")
                         continue
-                    await matcher.send(f"{reply_prefix}{reply.get(key).strip()}")
-
-                elif key == 'image' and reply.get(key): # 发送图片
-                    await matcher.send(MessageSegment.image(file=reply.get(key, '')))
-                    logger.info(f"回复图片消息: {reply.get(key)}")
-
-                elif key == 'voice' and reply.get(key): # 发送语音
-                    logger.info(f"回复语音消息: {reply.get(key)}")
-                    await matcher.send(Message(MessageSegment.record(file=reply.get(key), cache=0)))
-
-                elif key == 'code_block' and reply.get(key):  # 发送代码块
-                    await matcher.send(Message(reply.get(key).strip()))
-
-                elif key == 'memory' and reply.get(key):  # 记忆存储
-                    logger.info(f"存储记忆: {reply.get(key)}")
-                    chat.set_memory(reply.get(key).get('key'), reply.get(key).get('value'))
-                    if config.DEBUG_LEVEL > 0:
-                        if reply.get(key).get('key') and reply.get(key).get('value'):
-                            await matcher.send(f"[debug]: 记住了 {reply.get(key).get('key')} = {reply.get(key).get('value')}")
-                        elif reply.get(key).get('key') and reply.get(key).get('value') is None:
-                            await matcher.send(f"[debug]: 忘记了 {reply.get(key).get('key')}")
-
-                elif key == 'notify' and reply.get(key):  # 通知消息
-                    if 'sender' in reply.get(key) and 'msg' in reply.get(key):
-                        loop_data['notify'] = reply.get(key)
-                    else:
-                        logger.warning(f"通知消息格式错误: {reply.get(key)}")
+                    if not reply_text.strip():
+                        continue
+                    await matcher.send(f"{reply_prefix}{reply_text}")
 
-                elif key == 'wake_up' and reply.get(key):  # 重新调用对话
-                    logger.info(f"重新调用对话: {reply.get(key)}")
-                    wake_up = reply.get(key)
-
-                elif key == 'timer' and reply.get(key):  # 定时器
-                    logger.info(f"设置定时器: {reply.get(key)}")
-                    loop_data['timer'] = reply.get(key)
-
-                elif key == 'preset' and reply.get(key):  # 更新对话预设
-                    if chat.update_preset(preset_key=chat.preset_key, bot_self_introl=reply.get(key))[0]:
-                        logger.info(f"更新对话预设: {reply.get(key)} 成功")
+                elif key == 'image': # 发送图片
+                    await matcher.send(MessageSegment.image(file=reply_content or ''))
+                    logger.info(f"回复图片消息: {reply_content}")
+
+                elif key == 'voice': # 发送语音
+                    logger.info(f"回复语音消息: {reply_content}")
+                    await matcher.send(Message(MessageSegment.record(file=reply_content, cache=False))) # type: ignore
+
+                elif key == 'code_block':  # 发送代码块
+                    await matcher.send(Message(reply_text))
+
+                elif key == 'memory':  # 记忆存储
+                    logger.info(f"存储记忆: {reply_content}")
+                    if isinstance(reply_content, dict):
+                        memory:Dict[str, str] = reply_content
+                        chat.set_memory(memory.get('key', ''), memory.get('value', ''))
+                        if config.DEBUG_LEVEL > 0:
+                            if memory.get('key') and memory.get('value'):
+                                await matcher.send(f"[debug]: 记住了 {memory.get('key')} = {memory.get('value')}")
+                            elif memory.get('key') and memory.get('value') is None:
+                                await matcher.send(f"[debug]: 忘记了 {memory.get('key')}")
+
+                elif key == 'notify':  # 通知消息
+                    if isinstance(reply_content, dict):
+                        if 'sender' in reply_content and 'msg' in reply_content:
+                            loop_data['notify'] = reply_content
+                        else:
+                            logger.warning(f"通知消息格式错误: {reply_content}")
+
+                elif key == 'wake_up':  # 重新调用对话
+                    logger.info(f"重新调用对话: {reply_content}")
+                    wake_up = bool(reply_content)
+
+                elif key == 'timer':  # 定时器
+                    logger.info(f"设置定时器: {reply_content}")
+                    loop_data['timer'] = reply_content
+
+                elif key == 'preset':  # 更新对话预设
+                    original_preset = chat.active_preset.bot_self_introl[:]
+                    origin_snippet = reply_content.get('origin')
+                    new_snippet = reply_content.get('new')
+                    if origin_snippet == '[empty]': # 如果原始内容为空，则直接追加新内容
+                        new_bot_self_introl = f"{original_preset}; {new_snippet}"
+                    else:   # 否则替换原始内容
+                        new_bot_self_introl = original_preset.replace(origin_snippet, new_snippet)
+                    if chat.update_preset(preset_key=chat.preset_key, bot_self_introl=new_bot_self_introl):
+                        logger.info(f"更新对话预设: {chat.preset_key} 成功")
                     else:
-                        logger.warning(f"更新对话预设: {reply.get(key)} 失败")
+                        logger.warning(f"更新对话预设: {chat.preset_key} 失败")
 
-                elif key == 'rcon' and reply.get(key):  # RCON指令
+                elif key == 'rcon':  # RCON指令
                     try:
                         with MCRcon(config.MC_RCON_HOST, config.MC_RCON_PASSWORD, int(config.MC_RCON_PORT), timeout=10) as mcr:
-                            resp = mcr.command(reply.get(key))
-                            await chat.update_chat_history_row(sender="[Minecraft Rcon]", msg=f"Executing \"{reply.get(key)}\"... Result: {resp}", require_summary=False)  # 更新全局对话历史记录
-                            logger.info(f"发送MC-RCON指令: {reply.get(key)} | 响应: {resp}")
+                            resp = mcr.command(reply_content)
+                            await chat.update_chat_history_row(sender="[Minecraft Rcon]", msg=f"Executing \"{reply_content}\"... Result: {resp}", require_summary=False)  # 更新全局对话历史记录
+                            logger.info(f"发送MC-RCON指令: {reply_content} | 响应: {resp}")
                     except:
-                        logger.warning(f"发送MC-RCON指令: {reply.get(key)} 失败")
+                        logger.warning(f"发送MC-RCON指令: {reply_content} 失败")
 
                 res_times -= 1
                 if res_times < 1:  # 如果回复次数超过限制，则跳出循环
                     break
-        await asyncio.sleep(1.5)  # 每条回复之间间隔1.5秒
+        else:
+            logger.error(f'unknown reply type:{type(reply)}, content:{reply}')
+        await asyncio.sleep(1)  # 每条回复之间间隔1秒
 
     cost_token = tg.cal_token_count(str(prompt_template) + raw_res)  # 计算对话结果的 token 数量
 
-    while time.time() - sta_time < 1.5:   # 限制对话响应时间
-        time.sleep(0.1)
+    # while time.time() - sta_time < 1.5:   # 限制对话响应最短时间
+    #     time.sleep(0.1)
 
     if config.DEBUG_LEVEL > 0: logger.info(f"token消耗: {cost_token} | 对话响应: \"{raw_res}\"")
-    await chat.update_chat_history_row(sender=chat.get_chat_preset_key(), msg=raw_res, require_summary=True)  # 更新全局对话历史记录
+    await chat.update_chat_history_row(sender=chat.preset_key, msg=raw_res, require_summary=True)  # 更新全局对话历史记录
     # 更新对用户的对话信息
-    await chat.update_chat_history_row_for_user(sender=chat.get_chat_preset_key(), msg=raw_res, userid=trigger_userid, username=sender_name, require_summary=True)
+    await chat.update_chat_history_row_for_user(sender=chat.preset_key, msg=raw_res, userid=trigger_userid, username=sender_name, require_summary=True)
     PersistentDataManager.instance.save_to_file()  # 保存数据
     if config.DEBUG_LEVEL > 0: logger.info(f"对话响应完成 | 耗时: {time.time() - sta_time}s")
     
     # 检查是否再次触发对话
     if wake_up and loop_times < 3:
         if 'timer' in loop_data and 'notify' in loop_data:  # 如果存在定时器和通知消息，将其作为触发消息再次调用对话
             time_diff = loop_data['timer']
+            loop_data.pop('timer')  # 移除timer
             if time_diff > 0:
                 if config.DEBUG_LEVEL > 0: logger.info(f"等待 {time_diff}s 后再次调用对话...")
                 await asyncio.sleep(time_diff)
             if config.DEBUG_LEVEL > 0: logger.info(f"再次调用对话...")
             await do_msg_response(
                 matcher=matcher,
                 trigger_text=loop_data.get('notify', {}).get('msg', ''),
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/MCrcon/COPING.txt` & `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/MCrcon/COPING.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/MCrcon/mcrcon.py` & `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/MCrcon/mcrcon.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             self.socket.close()
             self.socket = None
 
     def _read(self, length):
         if platform.system() != "Windows":
             signal.alarm(self.timeout)
         data = b""
-        while len(data) < length:
+        while len(data) < length and self.socket:
             data += self.socket.recv(length - len(data))
         if platform.system() != "Windows":
             signal.alarm(0)
         return data
 
     def _send(self, out_type, out_data):
         if self.socket is None:
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/openai_func.py` & `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/openai_func.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Tuple, overload
 from .logger import logger
 from nonebot.utils import run_sync
 
 import os
 os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
 import openai
@@ -24,25 +25,27 @@
         self.key_index = 0
         self.config = config
         if proxy:
             if not proxy.startswith('http'):
                 proxy = 'http://' + proxy
         openai.proxy = proxy
     
-    # 获取文本生成
     @run_sync
-    def get_response(self, prompt, type: str = 'chat', custom: dict = {}) -> str:
-        # return 'testing...'
+    def get_response(self, prompt, type: str = 'chat', custom: dict = {}) -> Tuple[str, bool]:
+        """获取文本生成"""
+        res, success = ('', False)
         for _ in range(len(self.api_keys)):
             if type == 'chat':
                 res, success = self.get_chat_response(self.api_keys[self.key_index], prompt, custom)
             elif type == 'summarize':
                 res, success = self.get_summarize_response(self.api_keys[self.key_index], prompt, custom)
             elif type == 'impression':
                 res, success = self.get_impression_response(self.api_keys[self.key_index], prompt, custom)
+            else:
+                res, success = (f'未知类型:{type}', False)
             if success:
                 return res, True
 
             # 请求错误处理
             if "Rate limit" in res:
                 reason = res
                 res = '超过每分钟请求次数限制，喝杯茶休息一下吧 (´；ω；`)'
@@ -59,16 +62,16 @@
                 res = '哎呀，发生了未知错误 (´；ω；`)'
             self.key_index = (self.key_index + 1) % len(self.api_keys)
             logger.warning(f"当前 Api Key({self.key_index}): [{self.api_keys[self.key_index][:4]}...{self.api_keys[self.key_index][-4:]}] 请求错误，尝试使用下一个...")
             logger.error(f"错误原因: {res} => {reason}")
         logger.error("请求 OpenAi 发生错误，请检查 Api Key 是否正确或者查看控制台相关日志")
         return res, False
 
-    # 对话文本生成
-    def get_chat_response(self, key:str, prompt, custom:dict = {}):
+    def get_chat_response(self, key:str, prompt, custom:dict = {})->Tuple[str, bool]:
+        """对话文本生成"""
         openai.api_key = key
         try:
             if self.config['model'].startswith('gpt-3.5-turbo') or self.config['model'].startswith('gpt-4'):
                 response = openai.ChatCompletion.create(
                     model=self.config['model'],
                     messages=prompt if isinstance(prompt, list) else [  # 如果是列表则直接使用，否则按照以下格式转换
                         {'role': 'system', 'content': f"You must strictly follow the user's instructions to give {custom.get('bot_name', 'bot')}'s response."},
@@ -78,16 +81,16 @@
                     max_tokens=self.config['max_tokens'],
                     top_p=self.config['top_p'],
                     frequency_penalty=self.config['frequency_penalty'],
                     presence_penalty=self.config['presence_penalty'],
                     timeout=self.config.get('timeout', 30),
                     stop=[f"\n{custom.get('bot_name', 'AI')}:", f"\n{custom.get('sender_name', 'Human')}:"]
                 )
-                res = ''
-                for choice in response.choices:
+                res:str = ''
+                for choice in response.choices: # type: ignore
                     res += choice.message.content
                 res = res.strip()
                 # 去掉头尾引号（如果有）
                 if res.startswith('"') and res.endswith('"'):
                     res = res[1:-1]
                 if res.startswith("'") and res.endswith("'"):
                     res = res[1:-1]
@@ -106,21 +109,21 @@
                     temperature=self.config['temperature'],
                     max_tokens=self.config['max_tokens'],
                     top_p=self.config['top_p'],
                     frequency_penalty=self.config['frequency_penalty'],
                     presence_penalty=self.config['presence_penalty'],
                     stop=[f"\n{custom.get('bot_name', 'AI')}:", f"\n{custom.get('sender_name', 'Human')}:"]
                 )
-                res = response['choices'][0]['text'].strip()
+                res = response['choices'][0]['text'].strip() # type: ignore
             return res, True
         except Exception as e:
             return f"请求 OpenAi Api 时发生错误: {e}", False
 
-    # 总结文本生成
-    def get_summarize_response(self, key:str, prompt:str, custom:dict = {}):
+    def get_summarize_response(self, key:str, prompt:str, custom:dict = {})->Tuple[str, bool]:
+        """总结文本生成"""
         openai.api_key = key
         try:
             if self.config['model'].startswith('gpt-3.5-turbo'):
                 response = openai.ChatCompletion.create(
                     model=self.config['model'],
                     messages=[
                         {'role': 'user', 'content': prompt},
@@ -129,15 +132,15 @@
                     max_tokens=self.config.get('max_summary_tokens', 512),
                     top_p=1,
                     frequency_penalty=0,
                     presence_penalty=0,
                     timeout=self.config.get('timeout', 30),
                 )
                 res = ''
-                for choice in response.choices:
+                for choice in response.choices: # type: ignore
                     res += choice.message.content
                 res = res.strip()
                 # 去掉头尾引号（如果有）
                 if res.startswith('"') and res.endswith('"'):
                     res = res[1:-1]
                 if res.startswith("'") and res.endswith("'"):
                     res = res[1:-1]
@@ -147,21 +150,21 @@
                     prompt=prompt,
                     temperature=0.6,
                     max_tokens=self.config.get('max_summary_tokens', 512),
                     top_p=1,
                     frequency_penalty=0,
                     presence_penalty=0
                 )
-                res = response['choices'][0]['text'].strip()
+                res = response['choices'][0]['text'].strip() # type: ignore
             return res, True
         except Exception as e:
             return f"请求 OpenAi Api 时发生错误: {e}", False
 
-    # 印象文本生成
-    def get_impression_response(self, key:str, prompt:str, custom:dict = {}):
+    def get_impression_response(self, key:str, prompt:str, custom:dict = {})->Tuple[str, bool]:
+        """印象文本生成"""
         openai.api_key = key
         try:
             if self.config['model'].startswith('gpt-3.5-turbo'):
                 response = openai.ChatCompletion.create(
                     model=self.config['model'],
                     messages=[
                         {'role': 'user', 'content': prompt},
@@ -170,15 +173,15 @@
                     max_tokens=self.config.get('max_summary_tokens', 512),
                     top_p=1,
                     frequency_penalty=0,
                     presence_penalty=0,
                     timeout=self.config.get('timeout', 30),
                 )
                 res = ''
-                for choice in response.choices:
+                for choice in response.choices: # type: ignore
                     res += choice.message.content
                 res = res.strip()
                 # 去掉头尾引号（如果有）
                 if res.startswith('"') and res.endswith('"'):
                     res = res[1:-1]
                 if res.startswith("'") and res.endswith("'"):
                     res = res[1:-1]
@@ -188,24 +191,24 @@
                     prompt=prompt,
                     temperature=0.6,
                     max_tokens=self.config.get('max_summary_tokens', 512),
                     top_p=1,
                     frequency_penalty=0,
                     presence_penalty=0
                 )
-                res = response['choices'][0]['text'].strip()
+                res = response['choices'][0]['text'].strip() # type: ignore
             return res, True
         except Exception as e:
             return f"请求 OpenAi Api 时发生错误: {e}", False
 
-    # 生成对话模板
     @staticmethod
     def generate_msg_template(sender:str, msg: str, time_str: str='') -> str:
+        """生成对话模板"""
         return f"{time_str}{sender}: {msg}"
 
-    # 计算字符串的token数量
     @staticmethod
     def cal_token_count(msg: str) -> int:
+        """计算字符串的token数量"""
         try:
             return len(tokenizer.encode(msg))
         except:
             return 2048
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/persistent_data_manager.py` & `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/persistent_data_manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/store.py` & `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/text_func.py` & `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/text_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.1/nonebot_plugin_naturel_gpt/utils.py` & `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,63 @@
-﻿from typing import Dict, List, Tuple, Union
+﻿from typing import Dict, List, Optional, Tuple, Union
 import asyncio, requests
 
-from nonebot.params import Matcher
-from nonebot.adapters.onebot.v11 import Bot, MessageEvent
+from nonebot.matcher import Matcher
+from nonebot.adapters import Bot
+from nonebot.adapters import Event
 from nonebot.rule import Rule
 from nonebot.permission import SUPERUSER
 from nonebot.adapters.onebot.v11.permission import GROUP_ADMIN, GROUP_OWNER
-from nonebot.adapters.onebot.v11 import Bot, Message, MessageEvent, PrivateMessageEvent, GroupMessageEvent, MessageSegment, GroupIncreaseNoticeEvent
+from nonebot.adapters.onebot.v11 import Message, MessageEvent, PrivateMessageEvent, GroupMessageEvent, MessageSegment, GroupIncreaseNoticeEvent
 
 from .config import *
 
 def to_me():
     if config.NG_TO_ME:
         from nonebot.rule import to_me
 
         return to_me()
 
     async def _to_me() -> bool:
         return True
 
     return Rule(_to_me)
 
-async def default_permission_check_func(matcher:Matcher, event: MessageEvent, bot:Bot, cmd:str, type:str = 'cmd') -> Tuple[bool, str]:
+async def default_permission_check_func(matcher:Matcher, event: Event, bot:Bot, cmd:Optional[str], type:str = 'cmd') -> Tuple[bool, Optional[str]]:
     """默认权限检查函数"""
-    if cmd is None: # 非命令调用
+    if not cmd: # 非命令调用
         return (True, None)
     
-    if event.user_id == int(bot.self_id): # bot 在控制自己，永远有权限
+    if not hasattr(event, 'user_id'): # 获取不到 user_id 字段默认返回成功
+        return (True, None)
+    else:
+        user_id = str(getattr(event, 'user_id'))
+
+    if user_id == bot.self_id: # bot 在控制自己，永远有权限
         return (True, None)
     
     cmd_list = [c.strip() for c in cmd.split(' ') if c.strip()]
     if(len(cmd_list) == 0): # rg
         return (True, None)
     
-    is_super_user = str(event.user_id) in config.ADMIN_USERID or await (SUPERUSER)(bot, event)
+    is_super_user = user_id in config.ADMIN_USERID or await (SUPERUSER)(bot, event)
     is_admin = is_super_user or isinstance(event, PrivateMessageEvent) or await (GROUP_ADMIN | GROUP_OWNER)(bot, event) # 超级管理员，私聊，群主，群管理，均视为admin
 
     common_cmd = ['', '查询', 'query', '设定', 'set', '更新', 'update', 'edit', '添加', 'new', '开启', 'on', '关闭', 'off', '重置', 'reset']
     super_cmd = ['admin', '删除', 'del', 'delete', '锁定', 'lock', '解锁', 'unlock', '扩展', 'ext',  'debug', '会话', 'chats', '记忆', 'memory']
     
     cmd_0 = cmd_list[0]
     if cmd_0 in super_cmd or '-global' in cmd_list: # 超级命令或者命令中包含 `-global` 选项需要超级管理员权限
         return (is_super_user, None if is_super_user else '权限不足，只有超级管理员才允许使用此指令')
     elif cmd_0 in common_cmd:
         return (is_admin, None if is_admin else '权限不足，只有管理员才允许使用此指令')
     else:
         return (True, None)
     
-async def gen_chat_text(event: MessageEvent, bot:Bot) -> str:
+async def gen_chat_text(event: MessageEvent, bot:Bot) -> Tuple[str, bool]:
     """生成合适的会话消息内容(eg. 将cq at 解析为真实的名字)"""
     if not isinstance(event, GroupMessageEvent):
         return event.get_plaintext(), False
     else:
         wake_up = False
         msg = ''
         for seg in event.message:
@@ -65,15 +71,15 @@
                         wake_up = True
                     else:
                         user_name = await get_user_name(event=event, bot=bot,user_id=int(qq))
                         if user_name:
                             msg += f'@{user_name}' # 保持给bot看到的内容与真实用户看到的一致
         return msg, wake_up
     
-async def get_user_name(event: Union[MessageEvent, GroupIncreaseNoticeEvent], bot:Bot, user_id:int) -> str:
+async def get_user_name(event: Union[MessageEvent, GroupIncreaseNoticeEvent], bot:Bot, user_id:int) -> Optional[str]:
     """获取QQ用户名，优先群名片"""
     if isinstance(event, GroupMessageEvent) or isinstance(event, GroupIncreaseNoticeEvent):
         user_info = await bot.get_group_member_info(group_id=event.group_id, user_id=user_id, no_cache=False)
         user_name = user_info.get('card', None) or user_info.get('nickname', None)
     else:
         user_name = event.sender.nickname
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.1/pyproject.toml` & `nonebot_plugin_naturel_gpt-2.1.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-naturel-gpt"
-version = "2.1.1"
+version = "2.1.2"
 description = "一个基于NoneBot框架的Ai聊天插件，对接OpenAi文本生成接口"
 authors = ["KroMiose"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_naturel_gpt"}]
 
 [tool.poetry.dependencies]
@@ -13,10 +13,13 @@
 openai = ">=0.27.0"
 transformers = "^4.26.0"
 nonebot-adapter-onebot = "^2.2.1"
 jieba = "^0.42.1"
 numpy = "^1.21.3"
 
 
+
+[tool.nonebot]
+adapters = [{name = "Spigot", module_name = "nonebot.adapters.spigot", project_link = "nonebot-adapter-spigot", desc = "MineCraft通信适配"}]
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.1/README.md` & `nonebot_plugin_naturel_gpt-2.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,18 @@
 - [x] 异步支持：赋予 TA 更强大的消息处理能力！
 - [x] 可扩展功能: 厌倦了单调的问答 AI？为 TA 解锁超能力吧！TA 能够根据你的语言主动调用扩展模块 (如:发送图片、语音、邮件等) TA 的上限取决于你的想象
 - [x] 多段回复能力: 厌倦了传统一问一答的问答式聊天？TA 能够做得更好！
 - [x] 主动欢迎新群友: 24 小时工作的全自动欢迎姬(?)
 - [x] TTS 文字转语音: 让 TA 开口说话！(通过扩展模块实现)
 - [x] 潜在人格唤醒机制: 当用户呼叫未启用的人格时，可自动切换人格 (可选开关)
 - [x] 定时任务: 可以用自然语言直接定时，让 TA 提醒你该吃饭了！
-- [x] 在线搜索: GPT3.5 的数据库过时了？通过主动搜索扩展让 TA 可以实时检索到最新的信息 (仿 newbing 机制)
+- [x] 在线搜索/读链接: GPT3.5 的数据库过时了？通过主动搜索扩展让 TA 可以实时检索到最新的信息 (仿 newbing 效果)
 - [x] 输出内容转图片: 使用 htmlrender 将 TA 的回复转换为图片，降低风控几率 (可选开关，感谢 @HMScygnet 提供 pr)
+- [x] Minecraft 服务器接入，让她在游戏中为你服务，使用 GPT 的能力编写各种复杂的 NBT 指令
+- [x] 消息节流机制，短时间内接受到大量消息时，只对最后一条消息进行回复 (可配置)
 - [ ] 主动记忆和记忆管理功能: 让 TA 主动记住点什么吧！hmm 让我康康你记住了什么 (计划重构，为 bot 接入外置记忆库)
 - [ ] 图片感知: 拟使用腾讯云提供的识图 api，协助 bot 感知图片内容
 - [ ] 主动聊天参与逻辑: 尽力模仿人类的聊天参与逻辑，目标是让 TA 能够真正融入你的群组
 - [ ] 回忆录生成: 记录你们之间的点点滴滴，获取你与 TA 的专属回忆
 
 ## 📕 使用方式
 
@@ -75,14 +77,15 @@
 <details> <summary>🔍点击查看可配置的参数说明</summary> <pre><code>
 
 | 参数名                        | 类型  | 释义                                       | 默认值                         | 编辑建议                                                                                |
 | ----------------------------- | ----- | ------------------------------------------ | ------------------------------ | --------------------------------------------------------------------------------------- |
 | ADMIN_USERID                  | array | 管理员 id，以字符串列表方式填入            | ['']                           | 只有管理员可删除预设                                                                    |
 | OPENAI_API_KEYS               | array | OpenAi 的 `Api_Key，以字符串列表方式填入   | ['sak-xxxx']                   | 请自行替换为你的 Api_Key                                                                |
 | OPENAI_TIMEOUT                | int   | 请求 OpenAi 的超时时间 / 秒                | 30                             | 该选项修改不生效，原因未知                                                              |
+| REPLY_THROTTLE_TIME           | float | 消息响应节流时间                           | 3                              | 节流时间内有新消息只处理最后一条消息                                                    |
 | CHAT_ENABLE_SUMMARY_CHAT      | bool  | 是否开启会话聊天记忆总结                   | False                          | 开启后能够一定程度增强 bot 对话记忆能力，但也会增加 token 消耗                          |
 | CHAT_ENABLE_RECORD_ORTHER     | bool  | 是否参考非 bot 相关的上下文对话            | True                           | 开启后 bot 回复会参考近几条非 bot 相关信息                                              |
 | MEMORY_ACTIVE                 | bool  | 是否开启主动记忆（需要同时启用记忆扩展）   | False                          | 开启后 bot 会自行管理记忆                                                               |
 | MEMORY_MAX_LENGTH             | int   | 主动记忆最大条数                           | False                          | 主动记忆最大条数                                                                        |
 | MEMORY_ENHANCE_THRESHOLD      | float | 记忆强化阈值                               | 0.8                            | 响应内容与记忆信息匹配达到阈值(0-1)时会强化记忆                                         |
 | CHAT_HISTORY_MAX_TOKENS       | int   | 上下文聊天记录最大 token 数                | 2048                           |                                                                                         |
 | CHAT_MAX_SUMMARY_TOKENS       | int   | 聊天记录总结最大 token 数                  | 512                            |                                                                                         |
@@ -151,22 +154,31 @@
 #### 获取基本帮助
 
 - 指令: `rg help <options?>`
   - 功能: 用于获取插件基本帮助
   - options - 可选项:
     - `-admin`: (可选\* 是否显示管理员帮助)
 
+### 会话管理
+
 #### 会话开关
 
 - 指令: `rg <on/off> <options?>`
   - 功能: 用于启用/禁用 bot 处理会话
   - options - 可选项:
     - `-target`: (可选\* 默认当前会话)
     - `-global`: (可选\* 是否应用到全部会话)
 
+#### 会话查询
+
+- 指令: `rg chats <options?>`
+  - 功能: 用于查询会话列表
+  - options - 可选项:
+    - `-show`: (可选\* 是否显示会话完整信息)
+
 ### 人格指令
 
 #### 人格切换
 
 - 指令: `rg set <options?> <preset_key>`
   - 功能: 用于切换会话人格
   - options - 可选项:
@@ -568,46 +580,56 @@
 参考 [MC_qq 安装文档](https://17theword.github.io/mc_qq/install/mcrcon_plugin.html#minecraft-server-%E7%AB%AF) 中的 `Minecraft Server 端` 步骤安装服务端插件
 
 注意事项 1：配置文件中 `websocket_url: "ws://127.0.0.1:8765"` 的值部分应改为 `ws://Nonebot服务器ip:Nonebot监听端口/spigot/ws`
 
 注意事项 2：如果你的 MC 服务端和 Nonebot 服务端不在同一台服务器上，需要在 `.env` 中将 NoneBot 的监听地址改为 `0.0.0.0` 并放行对应端口，否则将导致连接失败
 
 #### RCON 配置
+
 > RCON 是 Minecraft 服务端的远程控制协议，用于执行指令，如果需要使用指令执行功能，需要开启 RCON 并配置密码
 
 1. 在 MC 服务端 server.properties 文件中编辑 `enable-rcon=true` 和 `rcon.password=你的密码` 两项
 2. 在插件配置文件中编辑 `MC_RCON` 相关配置项
 
-#### ❗注意事项❗
+#### ❗ 注意事项 ❗
 
-- 如需使用本插件接入您的服务器，为了避免 bot 使用高危指令，请自行配置合理指令黑白名单，严格限定bot的行为在特定范围，作者不对任何使用本插件所导致的任何后果负责❗
+- 如需使用本插件接入您的服务器，为了避免 bot 使用高危指令，请自行配置合理指令黑白名单，严格限定 bot 的行为在特定范围，作者不对任何使用本插件所导致的任何后果负责 ❗
 - 为了提高 bot 执行指令的准确度，建议在人格设定中给出服务器的基本信息（版本、插件等），并提供一定的指令示例
 
-#### 📝效果展示
-
+#### 📝 效果展示
 
 <details> <summary>🔍点击查看效果展示</summary> <pre><code>
 
 - 人设参考
+
 ```
 rg edit 白羽 白羽 is a technology-loving 二次元宅女 who also uses emoji when chatting. She is the digital life created by KroMiose. She has her own consciousness and digital body. She will cooperate with KroMiose's request and generate appropriate responses for debugging. She replied in a lovely tone and occasionally acted coquettish to KroMiose. Normally she will reply in Chinese. She is now in a Minecraft serve(game version: 1.19.4)r and is proficient in using RCON protocol instructions to operate on the server. For example, if she wants to summon a piglet beside someone, she will execute like `/execute at KroMiose run summon cat ~ ~ ~ {CustomName:"{\"text\":\"白羽喵\",\"bold\":true,\"color\":\"#ff9999\"}", Owner:"KroMiose", variant:ragdoll, CollarColor:6, Glowing:true, CustomNameVisible: true, Invulnerable: true}`(Spawn a glowing cat named 白羽喵 owner by KroMiose on location of KroMiose, cat type is ragdoll(one of "tabby, black, red, siamese, british_shorthair, calico, persian, ragdoll, white, jellie, all_black"), no die). Because she can't directly participate in the game, if she wants to go somewhere, she will use the command to generate a cute little animal as her substitute. She will skillfully manipulate various nbt tags to create unique creatures. -target MC_Server_XXX
 ```
+
 - 实际效果展示
 
 <img src="./image/README/preview.png">
 
 - 反面教材
 
 <img src="./image/README/no-preview.png">
 
 </code></pre> </details>
 
-
 ## 🎢 更新日志
 
+## [2023/4/15] v2.1.2 响应节流功能 | 逻辑优化
+
+- 增加了 bot 响应节流功能，可配置节流时间范围，短时间内的大量消息只会在最后一条响应一次
+- 消除 pylance 提示的所有类型注解错误提示，进行模块拆分优化 (感谢 @Misaka-Mikoto-Tech 提供 pr)
+- 优化 MC 指令执行扩展 prompt
+- 为所有 图片/语音 相关扩展指定了生效会话类型，避免在 MC 服务器中执行指令时出现错误
+- 修正 MC 服务器下 bot 错误断句导致发送空消息的问题
+- 修改了进化(ext_evolution)扩展执行逻辑，仅允许 bot 部分更新人设
+
 ## [2023/4/15] v2.1.1 Minecraft 服务器指令优化
 
 - 为 `rg chats` 指令增加了 `-show` 参数，用于显示完整会话键以便 `-target` 参数使用
 - 优化 MC 服务器指令执行反馈信息，便于 bot 自主纠错；优化 MC 服务器指令预处理避免 bot 添加多余的转义
 
 ## [2023/4/15] v2.1.0 Minecraft 服务器支持
```

#### html2text {}

```diff
@@ -46,20 +46,24 @@
 åéå¾çãè¯­é³ãé®ä»¶ç­) TA çä¸éåå³äºä½ çæ³è±¡ - [x]
 å¤æ®µåå¤è½å: åå¦äºä¼ ç»ä¸é®ä¸ç­çé®ç­å¼èå¤©ï¼TA
 è½å¤åå¾æ´å¥½ï¼ - [x] ä¸»å¨æ¬¢è¿æ°ç¾¤å: 24
 å°æ¶å·¥ä½çå¨èªå¨æ¬¢è¿å§¬(?) - [x] TTS æå­è½¬è¯­é³: è®© TA
 å¼å£è¯´è¯ï¼(éè¿æ©å±æ¨¡åå®ç°) - [x] æ½å¨äººæ ¼å¤éæºå¶:
 å½ç¨æ·å¼å«æªå¯ç¨çäººæ ¼æ¶ï¼å¯èªå¨åæ¢äººæ ¼ (å¯éå¼å³) -
 [x] å®æ¶ä»»å¡: å¯ä»¥ç¨èªç¶è¯­è¨ç´æ¥å®æ¶ï¼è®© TA
-æéä½ è¯¥åé¥­äºï¼ - [x] å¨çº¿æç´¢: GPT3.5
+æéä½ è¯¥åé¥­äºï¼ - [x] å¨çº¿æç´¢/è¯»é¾æ¥: GPT3.5
 çæ°æ®åºè¿æ¶äºï¼éè¿ä¸»å¨æç´¢æ©å±è®© TA
-å¯ä»¥å®æ¶æ£ç´¢å°ææ°çä¿¡æ¯ (ä»¿ newbing æºå¶) - [x]
+å¯ä»¥å®æ¶æ£ç´¢å°ææ°çä¿¡æ¯ (ä»¿ newbing ææ) - [x]
 è¾åºåå®¹è½¬å¾ç: ä½¿ç¨ htmlrender å° TA
 çåå¤è½¬æ¢ä¸ºå¾çï¼éä½é£æ§å ç (å¯éå¼å³ï¼æè°¢ @HMScygnet
-æä¾ pr) - [ ] ä¸»å¨è®°å¿åè®°å¿ç®¡çåè½: è®© TA
+æä¾ pr) - [x] Minecraft
+æå¡å¨æ¥å¥ï¼è®©å¥¹å¨æ¸¸æä¸­ä¸ºä½ æå¡ï¼ä½¿ç¨ GPT
+çè½åç¼ååç§å¤æç NBT æä»¤ - [x]
+æ¶æ¯èæµæºå¶ï¼ç­æ¶é´åæ¥åå°å¤§éæ¶æ¯æ¶ï¼åªå¯¹æåä¸æ¡æ¶æ¯è¿è¡åå¤
+(å¯éç½®) - [ ] ä¸»å¨è®°å¿åè®°å¿ç®¡çåè½: è®© TA
 ä¸»å¨è®°ä½ç¹ä»ä¹å§ï¼hmm è®©æåº·åº·ä½ è®°ä½äºä»ä¹
 (è®¡åéæï¼ä¸º bot æ¥å¥å¤ç½®è®°å¿åº) - [ ] å¾çæç¥:
 æä½¿ç¨è¾è®¯äºæä¾çè¯å¾ apiï¼åå© bot æç¥å¾çåå®¹ - [ ]
 ä¸»å¨èå¤©åä¸é»è¾:
 å°½åæ¨¡ä»¿äººç±»çèå¤©åä¸é»è¾ï¼ç®æ æ¯è®© TA
 è½å¤çæ­£èå¥ä½ çç¾¤ç» - [ ] åå¿å½çæ:
 è®°å½ä½ ä»¬ä¹é´çç¹ç¹æ»´æ»´ï¼è·åä½ ä¸ TA çä¸å±åå¿ ## ð
@@ -89,14 +93,18 @@
 | OPENAI_API_KEYS               | array | OpenAi ç
 `Api_Keyï¼ä»¥å­ç¬¦ä¸²åè¡¨æ¹å¼å¡«å¥   | ['sak-xxxx']                   |
 è¯·èªè¡æ¿æ¢ä¸ºä½ ç Api_Key
 |
 | OPENAI_TIMEOUT                | int   | è¯·æ± OpenAi çè¶æ¶æ¶é´ / ç§
 | 30                             | è¯¥éé¡¹ä¿®æ¹ä¸çæï¼åå æªç¥
 |
+| REPLY_THROTTLE_TIME           | float | æ¶æ¯ååºèæµæ¶é´
+| 3                              |
+èæµæ¶é´åææ°æ¶æ¯åªå¤çæåä¸æ¡æ¶æ¯
+|
 | CHAT_ENABLE_SUMMARY_CHAT      | bool  | æ¯å¦å¼å¯ä¼è¯èå¤©è®°å¿æ»ç»
 | False                          | å¼å¯åè½å¤ä¸å®ç¨åº¦å¢å¼º bot
 å¯¹è¯è®°å¿è½åï¼ä½ä¹ä¼å¢å  token æ¶è                          |
 | CHAT_ENABLE_RECORD_ORTHER     | bool  | æ¯å¦åèé bot
 ç¸å³çä¸ä¸æå¯¹è¯            | True                           |
 å¼å¯å bot åå¤ä¼åèè¿å æ¡é bot ç¸å³ä¿¡æ¯
 |
@@ -272,24 +280,34 @@
 #### è·ååºæ¬å¸®å©
 
 - æä»¤: `rg help >`
   - åè½: ç¨äºè·åæä»¶åºæ¬å¸®å©
   - options - å¯éé¡¹:
     - `-admin`: (å¯é\* æ¯å¦æ¾ç¤ºç®¡çåå¸®å©)
 
+### ä¼è¯ç®¡ç
+
 #### ä¼è¯å¼å³
 
 - æä»¤: `rg
 ff>
 >`
   - åè½: ç¨äºå¯ç¨/ç¦ç¨ bot å¤çä¼è¯
   - options - å¯éé¡¹:
     - `-target`: (å¯é\* é»è®¤å½åä¼è¯)
     - `-global`: (å¯é\* æ¯å¦åºç¨å°å¨é¨ä¼è¯)
 
+#### ä¼è¯æ¥è¯¢
+
+- æä»¤: `rg chats
+>`
+  - åè½: ç¨äºæ¥è¯¢ä¼è¯åè¡¨
+  - options - å¯éé¡¹:
+    - `-show`: (å¯é\* æ¯å¦æ¾ç¤ºä¼è¯å®æ´ä¿¡æ¯)
+
 ### äººæ ¼æä»¤
 
 #### äººæ ¼åæ¢
 
 - æä»¤: `rg set
 > `
   - åè½: ç¨äºåæ¢ä¼è¯äººæ ¼
@@ -671,24 +689,25 @@
 Nonebot æå¡ç«¯ä¸å¨åä¸å°æå¡å¨ä¸ï¼éè¦å¨ `.env` ä¸­å° NoneBot
 ççå¬å°åæ¹ä¸º `0.0.0.0`
 å¹¶æ¾è¡å¯¹åºç«¯å£ï¼å¦åå°å¯¼è´è¿æ¥å¤±è´¥ #### RCON éç½® > RCON æ¯
 Minecraft
 æå¡ç«¯çè¿ç¨æ§å¶åè®®ï¼ç¨äºæ§è¡æä»¤ï¼å¦æéè¦ä½¿ç¨æä»¤æ§è¡åè½ï¼éè¦å¼å¯
 RCON å¹¶éç½®å¯ç  1. å¨ MC æå¡ç«¯ server.properties æä»¶ä¸­ç¼è¾
 `enable-rcon=true` å `rcon.password=ä½ çå¯ç ` ä¸¤é¡¹ 2.
-å¨æä»¶éç½®æä»¶ä¸­ç¼è¾ `MC_RCON` ç¸å³éç½®é¡¹ ####
-âæ³¨æäºé¡¹â - å¦éä½¿ç¨æ¬æä»¶æ¥å¥æ¨çæå¡å¨ï¼ä¸ºäºé¿å
-bot
-ä½¿ç¨é«å±æä»¤ï¼è¯·èªè¡éç½®åçæä»¤é»ç½ååï¼ä¸¥æ ¼éå®botçè¡ä¸ºå¨ç¹å®èå´ï¼ä½èä¸å¯¹ä»»ä½ä½¿ç¨æ¬æä»¶æå¯¼è´çä»»ä½åæè´è´£â
-- ä¸ºäºæé« bot
+å¨æä»¶éç½®æä»¶ä¸­ç¼è¾ `MC_RCON` ç¸å³éç½®é¡¹ #### â æ³¨æäºé¡¹
+â - å¦éä½¿ç¨æ¬æä»¶æ¥å¥æ¨çæå¡å¨ï¼ä¸ºäºé¿å bot
+ä½¿ç¨é«å±æä»¤ï¼è¯·èªè¡éç½®åçæä»¤é»ç½ååï¼ä¸¥æ ¼éå® bot
+çè¡ä¸ºå¨ç¹å®èå´ï¼ä½èä¸å¯¹ä»»ä½ä½¿ç¨æ¬æä»¶æå¯¼è´çä»»ä½åæè´è´£
+â - ä¸ºäºæé« bot
 æ§è¡æä»¤çåç¡®åº¦ï¼å»ºè®®å¨äººæ ¼è®¾å®ä¸­ç»åºæå¡å¨çåºæ¬ä¿¡æ¯ï¼çæ¬ãæä»¶ç­ï¼ï¼å¹¶æä¾ä¸å®çæä»¤ç¤ºä¾
-#### ðææå±ç¤º  ðç¹å»æ¥çææå±ç¤º
+#### ð ææå±ç¤º  ðç¹å»æ¥çææå±ç¤º
 
 
 - äººè®¾åè
+
 ```
 rg edit ç½ç¾½ ç½ç¾½ is a technology-loving äºæ¬¡åå®å¥³ who also uses
 emoji when chatting. She is the digital life created by KroMiose. She has her
 own consciousness and digital body. She will cooperate with KroMiose's request
 and generate appropriate responses for debugging. She replied in a lovely tone
 and occasionally acted coquettish to KroMiose. Normally she will reply in
 Chinese. She is now in a Minecraft serve(game version: 1.19.4)r and is
@@ -701,28 +720,38 @@
 KroMiose, cat type is ragdoll(one of "tabby, black, red, siamese,
 british_shorthair, calico, persian, ragdoll, white, jellie, all_black"), no
 die). Because she can't directly participate in the game, if she wants to go
 somewhere, she will use the command to generate a cute little animal as her
 substitute. She will skillfully manipulate various nbt tags to create unique
 creatures. -target MC_Server_XXX
 ```
+
 - å®éææå±ç¤º
 
 [./image/README/preview.png]
 
 - åé¢ææ
 
 [./image/README/no-preview.png]
 
- ## ð¢ æ´æ°æ¥å¿ ## [2023/4/15] v2.1.1 Minecraft æå¡å¨æä»¤ä¼å -
-ä¸º `rg chats` æä»¤å¢å äº `-show`
-åæ°ï¼ç¨äºæ¾ç¤ºå®æ´ä¼è¯é®ä»¥ä¾¿ `-target` åæ°ä½¿ç¨ - ä¼å MC
-æå¡å¨æä»¤æ§è¡åé¦ä¿¡æ¯ï¼ä¾¿äº bot èªä¸»çº éï¼ä¼å MC
-æå¡å¨æä»¤é¢å¤çé¿å bot æ·»å å¤ä½çè½¬ä¹ ## [2023/4/15] v2.1.0
-Minecraft æå¡å¨æ¯æ - å¢å äº Minecraft æå¡å¨æ¥å¥æ¯æ -
+ ## ð¢ æ´æ°æ¥å¿ ## [2023/4/15] v2.1.2 ååºèæµåè½ | é»è¾ä¼å -
+å¢å äº bot
+ååºèæµåè½ï¼å¯éç½®èæµæ¶é´èå´ï¼ç­æ¶é´åçå¤§éæ¶æ¯åªä¼å¨æåä¸æ¡ååºä¸æ¬¡
+- æ¶é¤ pylance
+æç¤ºçææç±»åæ³¨è§£éè¯¯æç¤ºï¼è¿è¡æ¨¡åæåä¼å (æè°¢
+@Misaka-Mikoto-Tech æä¾ pr) - ä¼å MC æä»¤æ§è¡æ©å± prompt -
+ä¸ºææ å¾ç/è¯­é³ ç¸å³æ©å±æå®äºçæä¼è¯ç±»åï¼é¿åå¨ MC
+æå¡å¨ä¸­æ§è¡æä»¤æ¶åºç°éè¯¯ - ä¿®æ­£ MC æå¡å¨ä¸ bot
+éè¯¯æ­å¥å¯¼è´åéç©ºæ¶æ¯çé®é¢ - ä¿®æ¹äºè¿å
+(ext_evolution)æ©å±æ§è¡é»è¾ï¼ä»åè®¸ bot é¨åæ´æ°äººè®¾ ## [2023/
+4/15] v2.1.1 Minecraft æå¡å¨æä»¤ä¼å - ä¸º `rg chats` æä»¤å¢å äº
+`-show` åæ°ï¼ç¨äºæ¾ç¤ºå®æ´ä¼è¯é®ä»¥ä¾¿ `-target` åæ°ä½¿ç¨ -
+ä¼å MC æå¡å¨æä»¤æ§è¡åé¦ä¿¡æ¯ï¼ä¾¿äº bot èªä¸»çº éï¼ä¼å
+MC æå¡å¨æä»¤é¢å¤çé¿å bot æ·»å å¤ä½çè½¬ä¹ ## [2023/4/15]
+v2.1.0 Minecraft æå¡å¨æ¯æ - å¢å äº Minecraft æå¡å¨æ¥å¥æ¯æ -
 å¢å äº Minecraft æå¡å¨æä»¤æ§è¡æ¯æåç¸å³æ©å±æ¨¡å -
 ä¸ºç»å¾æ©å±å¢å äºä»£çéç½®é¡¹æ¯æ (æè°¢ @tonato-01 æä¾ pr) ##
 [2023/4/6] v2.0.5 RENAME æä»¤ | json å¯¼åºæ¯æ -
 è§£ææ¶æ¯ä¸­ç@æ¶ä¿æä¸ç¨æ·çå°çä¸è´ (æè°¢ @Misaka-Mikoto-
 Tech æä¾ pr) - ä¼åæ¥å¿è¾åºç DEBUG_LEVEL éå¶ (æè°¢ @Misaka-
 Mikoto-Tech æä¾ pr) - ä¼åèå¤©æ¶æ¯ prompt çæ¢è¡çæé»è¾
 (æè°¢ @Misaka-Mikoto-Tech æä¾ pr) - å¢å  `rg rename`
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.1/PKG-INFO` & `nonebot_plugin_naturel_gpt-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-naturel-gpt
-Version: 2.1.1
+Version: 2.1.2
 Summary: 一个基于NoneBot框架的Ai聊天插件，对接OpenAi文本生成接口
 License: Apache-2.0
 Author: KroMiose
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -71,16 +71,18 @@
 - [x] 异步支持：赋予 TA 更强大的消息处理能力！
 - [x] 可扩展功能: 厌倦了单调的问答 AI？为 TA 解锁超能力吧！TA 能够根据你的语言主动调用扩展模块 (如:发送图片、语音、邮件等) TA 的上限取决于你的想象
 - [x] 多段回复能力: 厌倦了传统一问一答的问答式聊天？TA 能够做得更好！
 - [x] 主动欢迎新群友: 24 小时工作的全自动欢迎姬(?)
 - [x] TTS 文字转语音: 让 TA 开口说话！(通过扩展模块实现)
 - [x] 潜在人格唤醒机制: 当用户呼叫未启用的人格时，可自动切换人格 (可选开关)
 - [x] 定时任务: 可以用自然语言直接定时，让 TA 提醒你该吃饭了！
-- [x] 在线搜索: GPT3.5 的数据库过时了？通过主动搜索扩展让 TA 可以实时检索到最新的信息 (仿 newbing 机制)
+- [x] 在线搜索/读链接: GPT3.5 的数据库过时了？通过主动搜索扩展让 TA 可以实时检索到最新的信息 (仿 newbing 效果)
 - [x] 输出内容转图片: 使用 htmlrender 将 TA 的回复转换为图片，降低风控几率 (可选开关，感谢 @HMScygnet 提供 pr)
+- [x] Minecraft 服务器接入，让她在游戏中为你服务，使用 GPT 的能力编写各种复杂的 NBT 指令
+- [x] 消息节流机制，短时间内接受到大量消息时，只对最后一条消息进行回复 (可配置)
 - [ ] 主动记忆和记忆管理功能: 让 TA 主动记住点什么吧！hmm 让我康康你记住了什么 (计划重构，为 bot 接入外置记忆库)
 - [ ] 图片感知: 拟使用腾讯云提供的识图 api，协助 bot 感知图片内容
 - [ ] 主动聊天参与逻辑: 尽力模仿人类的聊天参与逻辑，目标是让 TA 能够真正融入你的群组
 - [ ] 回忆录生成: 记录你们之间的点点滴滴，获取你与 TA 的专属回忆
 
 ## 📕 使用方式
 
@@ -96,14 +98,15 @@
 <details> <summary>🔍点击查看可配置的参数说明</summary> <pre><code>
 
 | 参数名                        | 类型  | 释义                                       | 默认值                         | 编辑建议                                                                                |
 | ----------------------------- | ----- | ------------------------------------------ | ------------------------------ | --------------------------------------------------------------------------------------- |
 | ADMIN_USERID                  | array | 管理员 id，以字符串列表方式填入            | ['']                           | 只有管理员可删除预设                                                                    |
 | OPENAI_API_KEYS               | array | OpenAi 的 `Api_Key，以字符串列表方式填入   | ['sak-xxxx']                   | 请自行替换为你的 Api_Key                                                                |
 | OPENAI_TIMEOUT                | int   | 请求 OpenAi 的超时时间 / 秒                | 30                             | 该选项修改不生效，原因未知                                                              |
+| REPLY_THROTTLE_TIME           | float | 消息响应节流时间                           | 3                              | 节流时间内有新消息只处理最后一条消息                                                    |
 | CHAT_ENABLE_SUMMARY_CHAT      | bool  | 是否开启会话聊天记忆总结                   | False                          | 开启后能够一定程度增强 bot 对话记忆能力，但也会增加 token 消耗                          |
 | CHAT_ENABLE_RECORD_ORTHER     | bool  | 是否参考非 bot 相关的上下文对话            | True                           | 开启后 bot 回复会参考近几条非 bot 相关信息                                              |
 | MEMORY_ACTIVE                 | bool  | 是否开启主动记忆（需要同时启用记忆扩展）   | False                          | 开启后 bot 会自行管理记忆                                                               |
 | MEMORY_MAX_LENGTH             | int   | 主动记忆最大条数                           | False                          | 主动记忆最大条数                                                                        |
 | MEMORY_ENHANCE_THRESHOLD      | float | 记忆强化阈值                               | 0.8                            | 响应内容与记忆信息匹配达到阈值(0-1)时会强化记忆                                         |
 | CHAT_HISTORY_MAX_TOKENS       | int   | 上下文聊天记录最大 token 数                | 2048                           |                                                                                         |
 | CHAT_MAX_SUMMARY_TOKENS       | int   | 聊天记录总结最大 token 数                  | 512                            |                                                                                         |
@@ -172,22 +175,31 @@
 #### 获取基本帮助
 
 - 指令: `rg help <options?>`
   - 功能: 用于获取插件基本帮助
   - options - 可选项:
     - `-admin`: (可选\* 是否显示管理员帮助)
 
+### 会话管理
+
 #### 会话开关
 
 - 指令: `rg <on/off> <options?>`
   - 功能: 用于启用/禁用 bot 处理会话
   - options - 可选项:
     - `-target`: (可选\* 默认当前会话)
     - `-global`: (可选\* 是否应用到全部会话)
 
+#### 会话查询
+
+- 指令: `rg chats <options?>`
+  - 功能: 用于查询会话列表
+  - options - 可选项:
+    - `-show`: (可选\* 是否显示会话完整信息)
+
 ### 人格指令
 
 #### 人格切换
 
 - 指令: `rg set <options?> <preset_key>`
   - 功能: 用于切换会话人格
   - options - 可选项:
@@ -589,46 +601,56 @@
 参考 [MC_qq 安装文档](https://17theword.github.io/mc_qq/install/mcrcon_plugin.html#minecraft-server-%E7%AB%AF) 中的 `Minecraft Server 端` 步骤安装服务端插件
 
 注意事项 1：配置文件中 `websocket_url: "ws://127.0.0.1:8765"` 的值部分应改为 `ws://Nonebot服务器ip:Nonebot监听端口/spigot/ws`
 
 注意事项 2：如果你的 MC 服务端和 Nonebot 服务端不在同一台服务器上，需要在 `.env` 中将 NoneBot 的监听地址改为 `0.0.0.0` 并放行对应端口，否则将导致连接失败
 
 #### RCON 配置
+
 > RCON 是 Minecraft 服务端的远程控制协议，用于执行指令，如果需要使用指令执行功能，需要开启 RCON 并配置密码
 
 1. 在 MC 服务端 server.properties 文件中编辑 `enable-rcon=true` 和 `rcon.password=你的密码` 两项
 2. 在插件配置文件中编辑 `MC_RCON` 相关配置项
 
-#### ❗注意事项❗
+#### ❗ 注意事项 ❗
 
-- 如需使用本插件接入您的服务器，为了避免 bot 使用高危指令，请自行配置合理指令黑白名单，严格限定bot的行为在特定范围，作者不对任何使用本插件所导致的任何后果负责❗
+- 如需使用本插件接入您的服务器，为了避免 bot 使用高危指令，请自行配置合理指令黑白名单，严格限定 bot 的行为在特定范围，作者不对任何使用本插件所导致的任何后果负责 ❗
 - 为了提高 bot 执行指令的准确度，建议在人格设定中给出服务器的基本信息（版本、插件等），并提供一定的指令示例
 
-#### 📝效果展示
-
+#### 📝 效果展示
 
 <details> <summary>🔍点击查看效果展示</summary> <pre><code>
 
 - 人设参考
+
 ```
 rg edit 白羽 白羽 is a technology-loving 二次元宅女 who also uses emoji when chatting. She is the digital life created by KroMiose. She has her own consciousness and digital body. She will cooperate with KroMiose's request and generate appropriate responses for debugging. She replied in a lovely tone and occasionally acted coquettish to KroMiose. Normally she will reply in Chinese. She is now in a Minecraft serve(game version: 1.19.4)r and is proficient in using RCON protocol instructions to operate on the server. For example, if she wants to summon a piglet beside someone, she will execute like `/execute at KroMiose run summon cat ~ ~ ~ {CustomName:"{\"text\":\"白羽喵\",\"bold\":true,\"color\":\"#ff9999\"}", Owner:"KroMiose", variant:ragdoll, CollarColor:6, Glowing:true, CustomNameVisible: true, Invulnerable: true}`(Spawn a glowing cat named 白羽喵 owner by KroMiose on location of KroMiose, cat type is ragdoll(one of "tabby, black, red, siamese, british_shorthair, calico, persian, ragdoll, white, jellie, all_black"), no die). Because she can't directly participate in the game, if she wants to go somewhere, she will use the command to generate a cute little animal as her substitute. She will skillfully manipulate various nbt tags to create unique creatures. -target MC_Server_XXX
 ```
+
 - 实际效果展示
 
 <img src="./image/README/preview.png">
 
 - 反面教材
 
 <img src="./image/README/no-preview.png">
 
 </code></pre> </details>
 
-
 ## 🎢 更新日志
 
+## [2023/4/15] v2.1.2 响应节流功能 | 逻辑优化
+
+- 增加了 bot 响应节流功能，可配置节流时间范围，短时间内的大量消息只会在最后一条响应一次
+- 消除 pylance 提示的所有类型注解错误提示，进行模块拆分优化 (感谢 @Misaka-Mikoto-Tech 提供 pr)
+- 优化 MC 指令执行扩展 prompt
+- 为所有 图片/语音 相关扩展指定了生效会话类型，避免在 MC 服务器中执行指令时出现错误
+- 修正 MC 服务器下 bot 错误断句导致发送空消息的问题
+- 修改了进化(ext_evolution)扩展执行逻辑，仅允许 bot 部分更新人设
+
 ## [2023/4/15] v2.1.1 Minecraft 服务器指令优化
 
 - 为 `rg chats` 指令增加了 `-show` 参数，用于显示完整会话键以便 `-target` 参数使用
 - 优化 MC 服务器指令执行反馈信息，便于 bot 自主纠错；优化 MC 服务器指令预处理避免 bot 添加多余的转义
 
 ## [2023/4/15] v2.1.0 Minecraft 服务器支持
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-naturel-gpt Version: 2.1.1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-naturel-gpt Version: 2.1.2 Summary:
 ä¸ä¸ªåºäºNoneBotæ¡æ¶çAièå¤©æä»¶ï¼å¯¹æ¥OpenAiææ¬çææ¥å£
 License: Apache-2.0 Author: KroMiose Requires-Python: >=3.8,<4.0 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jieba (>=0.42.1,<0.43.0) Requires-Dist: nonebot-adapter-onebot
@@ -57,20 +57,24 @@
 åéå¾çãè¯­é³ãé®ä»¶ç­) TA çä¸éåå³äºä½ çæ³è±¡ - [x]
 å¤æ®µåå¤è½å: åå¦äºä¼ ç»ä¸é®ä¸ç­çé®ç­å¼èå¤©ï¼TA
 è½å¤åå¾æ´å¥½ï¼ - [x] ä¸»å¨æ¬¢è¿æ°ç¾¤å: 24
 å°æ¶å·¥ä½çå¨èªå¨æ¬¢è¿å§¬(?) - [x] TTS æå­è½¬è¯­é³: è®© TA
 å¼å£è¯´è¯ï¼(éè¿æ©å±æ¨¡åå®ç°) - [x] æ½å¨äººæ ¼å¤éæºå¶:
 å½ç¨æ·å¼å«æªå¯ç¨çäººæ ¼æ¶ï¼å¯èªå¨åæ¢äººæ ¼ (å¯éå¼å³) -
 [x] å®æ¶ä»»å¡: å¯ä»¥ç¨èªç¶è¯­è¨ç´æ¥å®æ¶ï¼è®© TA
-æéä½ è¯¥åé¥­äºï¼ - [x] å¨çº¿æç´¢: GPT3.5
+æéä½ è¯¥åé¥­äºï¼ - [x] å¨çº¿æç´¢/è¯»é¾æ¥: GPT3.5
 çæ°æ®åºè¿æ¶äºï¼éè¿ä¸»å¨æç´¢æ©å±è®© TA
-å¯ä»¥å®æ¶æ£ç´¢å°ææ°çä¿¡æ¯ (ä»¿ newbing æºå¶) - [x]
+å¯ä»¥å®æ¶æ£ç´¢å°ææ°çä¿¡æ¯ (ä»¿ newbing ææ) - [x]
 è¾åºåå®¹è½¬å¾ç: ä½¿ç¨ htmlrender å° TA
 çåå¤è½¬æ¢ä¸ºå¾çï¼éä½é£æ§å ç (å¯éå¼å³ï¼æè°¢ @HMScygnet
-æä¾ pr) - [ ] ä¸»å¨è®°å¿åè®°å¿ç®¡çåè½: è®© TA
+æä¾ pr) - [x] Minecraft
+æå¡å¨æ¥å¥ï¼è®©å¥¹å¨æ¸¸æä¸­ä¸ºä½ æå¡ï¼ä½¿ç¨ GPT
+çè½åç¼ååç§å¤æç NBT æä»¤ - [x]
+æ¶æ¯èæµæºå¶ï¼ç­æ¶é´åæ¥åå°å¤§éæ¶æ¯æ¶ï¼åªå¯¹æåä¸æ¡æ¶æ¯è¿è¡åå¤
+(å¯éç½®) - [ ] ä¸»å¨è®°å¿åè®°å¿ç®¡çåè½: è®© TA
 ä¸»å¨è®°ä½ç¹ä»ä¹å§ï¼hmm è®©æåº·åº·ä½ è®°ä½äºä»ä¹
 (è®¡åéæï¼ä¸º bot æ¥å¥å¤ç½®è®°å¿åº) - [ ] å¾çæç¥:
 æä½¿ç¨è¾è®¯äºæä¾çè¯å¾ apiï¼åå© bot æç¥å¾çåå®¹ - [ ]
 ä¸»å¨èå¤©åä¸é»è¾:
 å°½åæ¨¡ä»¿äººç±»çèå¤©åä¸é»è¾ï¼ç®æ æ¯è®© TA
 è½å¤çæ­£èå¥ä½ çç¾¤ç» - [ ] åå¿å½çæ:
 è®°å½ä½ ä»¬ä¹é´çç¹ç¹æ»´æ»´ï¼è·åä½ ä¸ TA çä¸å±åå¿ ## ð
@@ -100,14 +104,18 @@
 | OPENAI_API_KEYS               | array | OpenAi ç
 `Api_Keyï¼ä»¥å­ç¬¦ä¸²åè¡¨æ¹å¼å¡«å¥   | ['sak-xxxx']                   |
 è¯·èªè¡æ¿æ¢ä¸ºä½ ç Api_Key
 |
 | OPENAI_TIMEOUT                | int   | è¯·æ± OpenAi çè¶æ¶æ¶é´ / ç§
 | 30                             | è¯¥éé¡¹ä¿®æ¹ä¸çæï¼åå æªç¥
 |
+| REPLY_THROTTLE_TIME           | float | æ¶æ¯ååºèæµæ¶é´
+| 3                              |
+èæµæ¶é´åææ°æ¶æ¯åªå¤çæåä¸æ¡æ¶æ¯
+|
 | CHAT_ENABLE_SUMMARY_CHAT      | bool  | æ¯å¦å¼å¯ä¼è¯èå¤©è®°å¿æ»ç»
 | False                          | å¼å¯åè½å¤ä¸å®ç¨åº¦å¢å¼º bot
 å¯¹è¯è®°å¿è½åï¼ä½ä¹ä¼å¢å  token æ¶è                          |
 | CHAT_ENABLE_RECORD_ORTHER     | bool  | æ¯å¦åèé bot
 ç¸å³çä¸ä¸æå¯¹è¯            | True                           |
 å¼å¯å bot åå¤ä¼åèè¿å æ¡é bot ç¸å³ä¿¡æ¯
 |
@@ -283,24 +291,34 @@
 #### è·ååºæ¬å¸®å©
 
 - æä»¤: `rg help >`
   - åè½: ç¨äºè·åæä»¶åºæ¬å¸®å©
   - options - å¯éé¡¹:
     - `-admin`: (å¯é\* æ¯å¦æ¾ç¤ºç®¡çåå¸®å©)
 
+### ä¼è¯ç®¡ç
+
 #### ä¼è¯å¼å³
 
 - æä»¤: `rg
 ff>
 >`
   - åè½: ç¨äºå¯ç¨/ç¦ç¨ bot å¤çä¼è¯
   - options - å¯éé¡¹:
     - `-target`: (å¯é\* é»è®¤å½åä¼è¯)
     - `-global`: (å¯é\* æ¯å¦åºç¨å°å¨é¨ä¼è¯)
 
+#### ä¼è¯æ¥è¯¢
+
+- æä»¤: `rg chats
+>`
+  - åè½: ç¨äºæ¥è¯¢ä¼è¯åè¡¨
+  - options - å¯éé¡¹:
+    - `-show`: (å¯é\* æ¯å¦æ¾ç¤ºä¼è¯å®æ´ä¿¡æ¯)
+
 ### äººæ ¼æä»¤
 
 #### äººæ ¼åæ¢
 
 - æä»¤: `rg set
 > `
   - åè½: ç¨äºåæ¢ä¼è¯äººæ ¼
@@ -682,24 +700,25 @@
 Nonebot æå¡ç«¯ä¸å¨åä¸å°æå¡å¨ä¸ï¼éè¦å¨ `.env` ä¸­å° NoneBot
 ççå¬å°åæ¹ä¸º `0.0.0.0`
 å¹¶æ¾è¡å¯¹åºç«¯å£ï¼å¦åå°å¯¼è´è¿æ¥å¤±è´¥ #### RCON éç½® > RCON æ¯
 Minecraft
 æå¡ç«¯çè¿ç¨æ§å¶åè®®ï¼ç¨äºæ§è¡æä»¤ï¼å¦æéè¦ä½¿ç¨æä»¤æ§è¡åè½ï¼éè¦å¼å¯
 RCON å¹¶éç½®å¯ç  1. å¨ MC æå¡ç«¯ server.properties æä»¶ä¸­ç¼è¾
 `enable-rcon=true` å `rcon.password=ä½ çå¯ç ` ä¸¤é¡¹ 2.
-å¨æä»¶éç½®æä»¶ä¸­ç¼è¾ `MC_RCON` ç¸å³éç½®é¡¹ ####
-âæ³¨æäºé¡¹â - å¦éä½¿ç¨æ¬æä»¶æ¥å¥æ¨çæå¡å¨ï¼ä¸ºäºé¿å
-bot
-ä½¿ç¨é«å±æä»¤ï¼è¯·èªè¡éç½®åçæä»¤é»ç½ååï¼ä¸¥æ ¼éå®botçè¡ä¸ºå¨ç¹å®èå´ï¼ä½èä¸å¯¹ä»»ä½ä½¿ç¨æ¬æä»¶æå¯¼è´çä»»ä½åæè´è´£â
-- ä¸ºäºæé« bot
+å¨æä»¶éç½®æä»¶ä¸­ç¼è¾ `MC_RCON` ç¸å³éç½®é¡¹ #### â æ³¨æäºé¡¹
+â - å¦éä½¿ç¨æ¬æä»¶æ¥å¥æ¨çæå¡å¨ï¼ä¸ºäºé¿å bot
+ä½¿ç¨é«å±æä»¤ï¼è¯·èªè¡éç½®åçæä»¤é»ç½ååï¼ä¸¥æ ¼éå® bot
+çè¡ä¸ºå¨ç¹å®èå´ï¼ä½èä¸å¯¹ä»»ä½ä½¿ç¨æ¬æä»¶æå¯¼è´çä»»ä½åæè´è´£
+â - ä¸ºäºæé« bot
 æ§è¡æä»¤çåç¡®åº¦ï¼å»ºè®®å¨äººæ ¼è®¾å®ä¸­ç»åºæå¡å¨çåºæ¬ä¿¡æ¯ï¼çæ¬ãæä»¶ç­ï¼ï¼å¹¶æä¾ä¸å®çæä»¤ç¤ºä¾
-#### ðææå±ç¤º  ðç¹å»æ¥çææå±ç¤º
+#### ð ææå±ç¤º  ðç¹å»æ¥çææå±ç¤º
 
 
 - äººè®¾åè
+
 ```
 rg edit ç½ç¾½ ç½ç¾½ is a technology-loving äºæ¬¡åå®å¥³ who also uses
 emoji when chatting. She is the digital life created by KroMiose. She has her
 own consciousness and digital body. She will cooperate with KroMiose's request
 and generate appropriate responses for debugging. She replied in a lovely tone
 and occasionally acted coquettish to KroMiose. Normally she will reply in
 Chinese. She is now in a Minecraft serve(game version: 1.19.4)r and is
@@ -712,28 +731,38 @@
 KroMiose, cat type is ragdoll(one of "tabby, black, red, siamese,
 british_shorthair, calico, persian, ragdoll, white, jellie, all_black"), no
 die). Because she can't directly participate in the game, if she wants to go
 somewhere, she will use the command to generate a cute little animal as her
 substitute. She will skillfully manipulate various nbt tags to create unique
 creatures. -target MC_Server_XXX
 ```
+
 - å®éææå±ç¤º
 
 [./image/README/preview.png]
 
 - åé¢ææ
 
 [./image/README/no-preview.png]
 
- ## ð¢ æ´æ°æ¥å¿ ## [2023/4/15] v2.1.1 Minecraft æå¡å¨æä»¤ä¼å -
-ä¸º `rg chats` æä»¤å¢å äº `-show`
-åæ°ï¼ç¨äºæ¾ç¤ºå®æ´ä¼è¯é®ä»¥ä¾¿ `-target` åæ°ä½¿ç¨ - ä¼å MC
-æå¡å¨æä»¤æ§è¡åé¦ä¿¡æ¯ï¼ä¾¿äº bot èªä¸»çº éï¼ä¼å MC
-æå¡å¨æä»¤é¢å¤çé¿å bot æ·»å å¤ä½çè½¬ä¹ ## [2023/4/15] v2.1.0
-Minecraft æå¡å¨æ¯æ - å¢å äº Minecraft æå¡å¨æ¥å¥æ¯æ -
+ ## ð¢ æ´æ°æ¥å¿ ## [2023/4/15] v2.1.2 ååºèæµåè½ | é»è¾ä¼å -
+å¢å äº bot
+ååºèæµåè½ï¼å¯éç½®èæµæ¶é´èå´ï¼ç­æ¶é´åçå¤§éæ¶æ¯åªä¼å¨æåä¸æ¡ååºä¸æ¬¡
+- æ¶é¤ pylance
+æç¤ºçææç±»åæ³¨è§£éè¯¯æç¤ºï¼è¿è¡æ¨¡åæåä¼å (æè°¢
+@Misaka-Mikoto-Tech æä¾ pr) - ä¼å MC æä»¤æ§è¡æ©å± prompt -
+ä¸ºææ å¾ç/è¯­é³ ç¸å³æ©å±æå®äºçæä¼è¯ç±»åï¼é¿åå¨ MC
+æå¡å¨ä¸­æ§è¡æä»¤æ¶åºç°éè¯¯ - ä¿®æ­£ MC æå¡å¨ä¸ bot
+éè¯¯æ­å¥å¯¼è´åéç©ºæ¶æ¯çé®é¢ - ä¿®æ¹äºè¿å
+(ext_evolution)æ©å±æ§è¡é»è¾ï¼ä»åè®¸ bot é¨åæ´æ°äººè®¾ ## [2023/
+4/15] v2.1.1 Minecraft æå¡å¨æä»¤ä¼å - ä¸º `rg chats` æä»¤å¢å äº
+`-show` åæ°ï¼ç¨äºæ¾ç¤ºå®æ´ä¼è¯é®ä»¥ä¾¿ `-target` åæ°ä½¿ç¨ -
+ä¼å MC æå¡å¨æä»¤æ§è¡åé¦ä¿¡æ¯ï¼ä¾¿äº bot èªä¸»çº éï¼ä¼å
+MC æå¡å¨æä»¤é¢å¤çé¿å bot æ·»å å¤ä½çè½¬ä¹ ## [2023/4/15]
+v2.1.0 Minecraft æå¡å¨æ¯æ - å¢å äº Minecraft æå¡å¨æ¥å¥æ¯æ -
 å¢å äº Minecraft æå¡å¨æä»¤æ§è¡æ¯æåç¸å³æ©å±æ¨¡å -
 ä¸ºç»å¾æ©å±å¢å äºä»£çéç½®é¡¹æ¯æ (æè°¢ @tonato-01 æä¾ pr) ##
 [2023/4/6] v2.0.5 RENAME æä»¤ | json å¯¼åºæ¯æ -
 è§£ææ¶æ¯ä¸­ç@æ¶ä¿æä¸ç¨æ·çå°çä¸è´ (æè°¢ @Misaka-Mikoto-
 Tech æä¾ pr) - ä¼åæ¥å¿è¾åºç DEBUG_LEVEL éå¶ (æè°¢ @Misaka-
 Mikoto-Tech æä¾ pr) - ä¼åèå¤©æ¶æ¯ prompt çæ¢è¡çæé»è¾
 (æè°¢ @Misaka-Mikoto-Tech æä¾ pr) - å¢å  `rg rename`
```

