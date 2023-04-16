# Comparing `tmp/nonebot_plugin_naturel_gpt-2.1.2.tar.gz` & `tmp/nonebot_plugin_naturel_gpt-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_naturel_gpt-2.1.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_naturel_gpt-2.1.3.tar", max compression
```

## Comparing `nonebot_plugin_naturel_gpt-2.1.2.tar` & `nonebot_plugin_naturel_gpt-2.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11558 2023-01-29 20:13:51.193394 nonebot_plugin_naturel_gpt-2.1.2/LICENSE
--rw-r--r--   0        0        0     2345 2023-04-15 18:38:05.110657 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/__init__.py
--rw-r--r--   0        0        0    26222 2023-04-16 16:20:15.076676 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/chat.py
--rw-r--r--   0        0        0     6004 2023-04-15 18:38:05.113654 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/chat_manager.py
--rw-r--r--   0        0        0    23543 2023-04-15 18:38:05.115650 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/command_func.py
--rw-r--r--   0        0        0    12868 2023-04-16 12:44:36.108186 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/config.py
--rw-r--r--   0        0        0     6187 2023-04-15 18:38:05.109147 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/Extension.py
--rw-r--r--   0        0        0      237 2023-04-05 16:12:46.786453 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/logger.py
--rw-r--r--   0        0        0    29500 2023-04-16 14:10:42.687395 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/matcher.py
--rw-r--r--   0        0        0     7300 2023-04-16 11:16:04.694453 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/matcher_MCRcon.py
--rw-r--r--   0        0        0     1218 2023-04-14 15:48:38.092610 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/MCrcon/COPING.txt
--rw-r--r--   0        0        0     6285 2023-04-15 18:38:05.110151 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/MCrcon/mcrcon.py
--rw-r--r--   0        0        0    10245 2023-04-15 18:38:05.120960 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/openai_func.py
--rw-r--r--   0        0        0    10828 2023-04-05 16:12:46.788447 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/persistent_data_manager.py
--rw-r--r--   0        0        0      499 2023-04-15 18:38:05.121664 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/singleton.py
--rw-r--r--   0        0        0     2715 2023-04-05 16:12:46.789445 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/store.py
--rw-r--r--   0        0        0     1831 2023-04-05 16:12:46.790443 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/text_func.py
--rw-r--r--   0        0        0     4556 2023-04-15 18:38:05.122660 nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/utils.py
--rw-r--r--   0        0        0      741 2023-04-16 16:17:56.636992 nonebot_plugin_naturel_gpt-2.1.2/pyproject.toml
--rw-r--r--   0        0        0    53632 2023-04-16 16:17:47.921979 nonebot_plugin_naturel_gpt-2.1.2/README.md
--rw-r--r--   0        0        0    53598 1970-01-01 00:00:00.000000 nonebot_plugin_naturel_gpt-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11558 2023-01-29 20:13:51.193394 nonebot_plugin_naturel_gpt-2.1.3/LICENSE
+-rw-r--r--   0        0        0     2345 2023-04-15 18:38:05.110657 nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/__init__.py
+-rw-r--r--   0        0        0    26270 2023-04-16 17:09:02.439109 nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/chat.py
+-rw-r--r--   0        0        0     6004 2023-04-15 18:38:05.113654 nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/chat_manager.py
+-rw-r--r--   0        0        0    23543 2023-04-15 18:38:05.115650 nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/command_func.py
+-rw-r--r--   0        0        0    12868 2023-04-16 12:44:36.108186 nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/config.py
+-rw-r--r--   0        0        0     6187 2023-04-15 18:38:05.109147 nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/Extension.py
+-rw-r--r--   0        0        0      237 2023-04-05 16:12:46.786453 nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/logger.py
+-rw-r--r--   0        0        0    29616 2023-04-16 17:09:20.840400 nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/matcher.py
+-rw-r--r--   0        0        0     7300 2023-04-16 11:16:04.694453 nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/matcher_MCRcon.py
+-rw-r--r--   0        0        0     1218 2023-04-14 15:48:38.092610 nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/MCrcon/COPING.txt
+-rw-r--r--   0        0        0     6285 2023-04-15 18:38:05.110151 nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/MCrcon/mcrcon.py
+-rw-r--r--   0        0        0    10245 2023-04-15 18:38:05.120960 nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/openai_func.py
+-rw-r--r--   0        0        0    10828 2023-04-05 16:12:46.788447 nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/persistent_data_manager.py
+-rw-r--r--   0        0        0      499 2023-04-15 18:38:05.121664 nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/singleton.py
+-rw-r--r--   0        0        0     2715 2023-04-05 16:12:46.789445 nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/store.py
+-rw-r--r--   0        0        0     1831 2023-04-05 16:12:46.790443 nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/text_func.py
+-rw-r--r--   0        0        0     4556 2023-04-15 18:38:05.122660 nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/utils.py
+-rw-r--r--   0        0        0      741 2023-04-16 17:10:18.546353 nonebot_plugin_naturel_gpt-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0    53701 2023-04-16 17:10:44.890509 nonebot_plugin_naturel_gpt-2.1.3/README.md
+-rw-r--r--   0        0        0    53666 1970-01-01 00:00:00.000000 nonebot_plugin_naturel_gpt-2.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.2/LICENSE` & `nonebot_plugin_naturel_gpt-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/__init__.py` & `nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/chat.py` & `nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,21 +30,22 @@
                 if preset.is_default:
                     preset_key = pk
                     break
             else:   # 如果没有默认预设，则选择第一个预设
                 preset_key = list(self.chat_preset_dicts.keys())[0]
         self.change_presettings(preset_key)
 
-    async def update_chat_history_row(self, sender:str, msg: str, require_summary:bool = False) -> None:
+    async def update_chat_history_row(self, sender:str, msg: str, require_summary:bool = False, record_time=False) -> None:
         """更新当前会话的全局对话历史行"""
         tg = TextGenerator.instance
         messageunit = tg.generate_msg_template(sender=sender, msg=msg, time_str=f"[{time.strftime('%H:%M:%S %p', time.localtime())}] ")
         self._chat_data.chat_history.append(messageunit)
         if config.DEBUG_LEVEL > 0: logger.info(f"[会话: {self.chat_key}]添加对话历史行: {messageunit}  |  当前对话历史行数: {len(self._chat_data.chat_history)}")
-        self._last_msg_time = time.time()   # 更新上次对话时间
+        if record_time:
+            self._last_msg_time = time.time()   # 更新上次对话时间
         while len(self._chat_data.chat_history) > config.CHAT_MEMORY_MAX_LENGTH * 2:    # 保证对话历史不超过最大长度的两倍
             self._chat_data.chat_history.pop(0)
 
         if len(self._chat_data.chat_history) > config.CHAT_MEMORY_MAX_LENGTH and require_summary and config.CHAT_ENABLE_SUMMARY_CHAT: # 只有在开启总结功能并且在bot回复后才进行总结 避免不必要的token消耗
             prev_summarized = f"Summary of last conversation:{self._chat_data.chat_summarized}\n\n"
             history_str = '\n'.join(self._chat_data.chat_history)
             prompt = (  # 以机器人的视角总结对话历史
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/chat_manager.py` & `nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/chat_manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/command_func.py` & `nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/command_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/config.py` & `nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/Extension.py` & `nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/Extension.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/matcher.py` & `nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,19 +267,19 @@
         (config.REPLY_ON_NAME_MENTION and (chat.preset_key.lower() in trigger_text.lower())) or \
         (config.REPLY_ON_AT and is_tome)
     ):
         # 更新全局对话历史记录
         # chat.update_chat_history_row(sender=sender_name, msg=trigger_text, require_summary=True)
         await chat.update_chat_history_row(sender=sender_name,
                                     msg=f"@{chat.preset_key} {trigger_text}" if is_tome and chat_type=='group' else trigger_text,
-                                    require_summary=False)
+                                    require_summary=False, record_time=True)    # 只有在需要回复时才记录时间，用于节流
         logger.info("符合 bot 发言条件，进行回复...")
     else:
         if config.CHAT_ENABLE_RECORD_ORTHER:
-            await chat.update_chat_history_row(sender=sender_name, msg=trigger_text, require_summary=False)
+            await chat.update_chat_history_row(sender=sender_name, msg=trigger_text, require_summary=False, record_time=False)
             if config.DEBUG_LEVEL > 1: logger.info("不是 bot 相关的信息，记录但不进行回复")
         else:
             if config.DEBUG_LEVEL > 1: logger.info("不是 bot 相关的信息，不进行回复")
         return
     
     wake_up = False # 进入对话流程，重置唤醒状态
 
@@ -526,15 +526,15 @@
 
     cost_token = tg.cal_token_count(str(prompt_template) + raw_res)  # 计算对话结果的 token 数量
 
     # while time.time() - sta_time < 1.5:   # 限制对话响应最短时间
     #     time.sleep(0.1)
 
     if config.DEBUG_LEVEL > 0: logger.info(f"token消耗: {cost_token} | 对话响应: \"{raw_res}\"")
-    await chat.update_chat_history_row(sender=chat.preset_key, msg=raw_res, require_summary=True)  # 更新全局对话历史记录
+    await chat.update_chat_history_row(sender=chat.preset_key, msg=raw_res, require_summary=True, record_time=False)  # 更新全局对话历史记录
     # 更新对用户的对话信息
     await chat.update_chat_history_row_for_user(sender=chat.preset_key, msg=raw_res, userid=trigger_userid, username=sender_name, require_summary=True)
     PersistentDataManager.instance.save_to_file()  # 保存数据
     if config.DEBUG_LEVEL > 0: logger.info(f"对话响应完成 | 耗时: {time.time() - sta_time}s")
     
     # 检查是否再次触发对话
     if wake_up and loop_times < 3:
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/matcher_MCRcon.py` & `nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/matcher_MCRcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/MCrcon/COPING.txt` & `nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/MCrcon/COPING.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/MCrcon/mcrcon.py` & `nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/MCrcon/mcrcon.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/openai_func.py` & `nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/openai_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/persistent_data_manager.py` & `nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/persistent_data_manager.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/store.py` & `nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/text_func.py` & `nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/text_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.2/nonebot_plugin_naturel_gpt/utils.py` & `nonebot_plugin_naturel_gpt-2.1.3/nonebot_plugin_naturel_gpt/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_naturel_gpt-2.1.2/pyproject.toml` & `nonebot_plugin_naturel_gpt-2.1.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-naturel-gpt"
-version = "2.1.2"
+version = "2.1.3"
 description = "一个基于NoneBot框架的Ai聊天插件，对接OpenAi文本生成接口"
 authors = ["KroMiose"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_naturel_gpt"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.2/README.md` & `nonebot_plugin_naturel_gpt-2.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -613,22 +613,23 @@
 
 <img src="./image/README/no-preview.png">
 
 </code></pre> </details>
 
 ## 🎢 更新日志
 
-## [2023/4/15] v2.1.2 响应节流功能 | 逻辑优化
+## [2023/4/17] v2.1.3 响应节流功能 | 逻辑优化
 
 - 增加了 bot 响应节流功能，可配置节流时间范围，短时间内的大量消息只会在最后一条响应一次
 - 消除 pylance 提示的所有类型注解错误提示，进行模块拆分优化 (感谢 @Misaka-Mikoto-Tech 提供 pr)
 - 优化 MC 指令执行扩展 prompt
 - 为所有 图片/语音 相关扩展指定了生效会话类型，避免在 MC 服务器中执行指令时出现错误
 - 修正 MC 服务器下 bot 错误断句导致发送空消息的问题
 - 修改了进化(ext_evolution)扩展执行逻辑，仅允许 bot 部分更新人设
+- 修正节流逻辑错误，避免 bot 无法响应消息的问题
 
 ## [2023/4/15] v2.1.1 Minecraft 服务器指令优化
 
 - 为 `rg chats` 指令增加了 `-show` 参数，用于显示完整会话键以便 `-target` 参数使用
 - 优化 MC 服务器指令执行反馈信息，便于 bot 自主纠错；优化 MC 服务器指令预处理避免 bot 添加多余的转义
 
 ## [2023/4/15] v2.1.0 Minecraft 服务器支持
```

#### html2text {}

```diff
@@ -729,26 +729,27 @@
 
 [./image/README/preview.png]
 
 - åé¢ææ
 
 [./image/README/no-preview.png]
 
- ## ð¢ æ´æ°æ¥å¿ ## [2023/4/15] v2.1.2 ååºèæµåè½ | é»è¾ä¼å -
+ ## ð¢ æ´æ°æ¥å¿ ## [2023/4/17] v2.1.3 ååºèæµåè½ | é»è¾ä¼å -
 å¢å äº bot
 ååºèæµåè½ï¼å¯éç½®èæµæ¶é´èå´ï¼ç­æ¶é´åçå¤§éæ¶æ¯åªä¼å¨æåä¸æ¡ååºä¸æ¬¡
 - æ¶é¤ pylance
 æç¤ºçææç±»åæ³¨è§£éè¯¯æç¤ºï¼è¿è¡æ¨¡åæåä¼å (æè°¢
 @Misaka-Mikoto-Tech æä¾ pr) - ä¼å MC æä»¤æ§è¡æ©å± prompt -
 ä¸ºææ å¾ç/è¯­é³ ç¸å³æ©å±æå®äºçæä¼è¯ç±»åï¼é¿åå¨ MC
 æå¡å¨ä¸­æ§è¡æä»¤æ¶åºç°éè¯¯ - ä¿®æ­£ MC æå¡å¨ä¸ bot
 éè¯¯æ­å¥å¯¼è´åéç©ºæ¶æ¯çé®é¢ - ä¿®æ¹äºè¿å
-(ext_evolution)æ©å±æ§è¡é»è¾ï¼ä»åè®¸ bot é¨åæ´æ°äººè®¾ ## [2023/
-4/15] v2.1.1 Minecraft æå¡å¨æä»¤ä¼å - ä¸º `rg chats` æä»¤å¢å äº
-`-show` åæ°ï¼ç¨äºæ¾ç¤ºå®æ´ä¼è¯é®ä»¥ä¾¿ `-target` åæ°ä½¿ç¨ -
+(ext_evolution)æ©å±æ§è¡é»è¾ï¼ä»åè®¸ bot é¨åæ´æ°äººè®¾ -
+ä¿®æ­£èæµé»è¾éè¯¯ï¼é¿å bot æ æ³ååºæ¶æ¯çé®é¢ ## [2023/4/
+15] v2.1.1 Minecraft æå¡å¨æä»¤ä¼å - ä¸º `rg chats` æä»¤å¢å äº `-
+show` åæ°ï¼ç¨äºæ¾ç¤ºå®æ´ä¼è¯é®ä»¥ä¾¿ `-target` åæ°ä½¿ç¨ -
 ä¼å MC æå¡å¨æä»¤æ§è¡åé¦ä¿¡æ¯ï¼ä¾¿äº bot èªä¸»çº éï¼ä¼å
 MC æå¡å¨æä»¤é¢å¤çé¿å bot æ·»å å¤ä½çè½¬ä¹ ## [2023/4/15]
 v2.1.0 Minecraft æå¡å¨æ¯æ - å¢å äº Minecraft æå¡å¨æ¥å¥æ¯æ -
 å¢å äº Minecraft æå¡å¨æä»¤æ§è¡æ¯æåç¸å³æ©å±æ¨¡å -
 ä¸ºç»å¾æ©å±å¢å äºä»£çéç½®é¡¹æ¯æ (æè°¢ @tonato-01 æä¾ pr) ##
 [2023/4/6] v2.0.5 RENAME æä»¤ | json å¯¼åºæ¯æ -
 è§£ææ¶æ¯ä¸­ç@æ¶ä¿æä¸ç¨æ·çå°çä¸è´ (æè°¢ @Misaka-Mikoto-
```

### Comparing `nonebot_plugin_naturel_gpt-2.1.2/PKG-INFO` & `nonebot_plugin_naturel_gpt-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-naturel-gpt
-Version: 2.1.2
+Version: 2.1.3
 Summary: 一个基于NoneBot框架的Ai聊天插件，对接OpenAi文本生成接口
 License: Apache-2.0
 Author: KroMiose
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -634,22 +634,23 @@
 
 <img src="./image/README/no-preview.png">
 
 </code></pre> </details>
 
 ## 🎢 更新日志
 
-## [2023/4/15] v2.1.2 响应节流功能 | 逻辑优化
+## [2023/4/17] v2.1.3 响应节流功能 | 逻辑优化
 
 - 增加了 bot 响应节流功能，可配置节流时间范围，短时间内的大量消息只会在最后一条响应一次
 - 消除 pylance 提示的所有类型注解错误提示，进行模块拆分优化 (感谢 @Misaka-Mikoto-Tech 提供 pr)
 - 优化 MC 指令执行扩展 prompt
 - 为所有 图片/语音 相关扩展指定了生效会话类型，避免在 MC 服务器中执行指令时出现错误
 - 修正 MC 服务器下 bot 错误断句导致发送空消息的问题
 - 修改了进化(ext_evolution)扩展执行逻辑，仅允许 bot 部分更新人设
+- 修正节流逻辑错误，避免 bot 无法响应消息的问题
 
 ## [2023/4/15] v2.1.1 Minecraft 服务器指令优化
 
 - 为 `rg chats` 指令增加了 `-show` 参数，用于显示完整会话键以便 `-target` 参数使用
 - 优化 MC 服务器指令执行反馈信息，便于 bot 自主纠错；优化 MC 服务器指令预处理避免 bot 添加多余的转义
 
 ## [2023/4/15] v2.1.0 Minecraft 服务器支持
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-naturel-gpt Version: 2.1.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-naturel-gpt Version: 2.1.3 Summary:
 ä¸ä¸ªåºäºNoneBotæ¡æ¶çAièå¤©æä»¶ï¼å¯¹æ¥OpenAiææ¬çææ¥å£
 License: Apache-2.0 Author: KroMiose Requires-Python: >=3.8,<4.0 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jieba (>=0.42.1,<0.43.0) Requires-Dist: nonebot-adapter-onebot
@@ -740,26 +740,27 @@
 
 [./image/README/preview.png]
 
 - åé¢ææ
 
 [./image/README/no-preview.png]
 
- ## ð¢ æ´æ°æ¥å¿ ## [2023/4/15] v2.1.2 ååºèæµåè½ | é»è¾ä¼å -
+ ## ð¢ æ´æ°æ¥å¿ ## [2023/4/17] v2.1.3 ååºèæµåè½ | é»è¾ä¼å -
 å¢å äº bot
 ååºèæµåè½ï¼å¯éç½®èæµæ¶é´èå´ï¼ç­æ¶é´åçå¤§éæ¶æ¯åªä¼å¨æåä¸æ¡ååºä¸æ¬¡
 - æ¶é¤ pylance
 æç¤ºçææç±»åæ³¨è§£éè¯¯æç¤ºï¼è¿è¡æ¨¡åæåä¼å (æè°¢
 @Misaka-Mikoto-Tech æä¾ pr) - ä¼å MC æä»¤æ§è¡æ©å± prompt -
 ä¸ºææ å¾ç/è¯­é³ ç¸å³æ©å±æå®äºçæä¼è¯ç±»åï¼é¿åå¨ MC
 æå¡å¨ä¸­æ§è¡æä»¤æ¶åºç°éè¯¯ - ä¿®æ­£ MC æå¡å¨ä¸ bot
 éè¯¯æ­å¥å¯¼è´åéç©ºæ¶æ¯çé®é¢ - ä¿®æ¹äºè¿å
-(ext_evolution)æ©å±æ§è¡é»è¾ï¼ä»åè®¸ bot é¨åæ´æ°äººè®¾ ## [2023/
-4/15] v2.1.1 Minecraft æå¡å¨æä»¤ä¼å - ä¸º `rg chats` æä»¤å¢å äº
-`-show` åæ°ï¼ç¨äºæ¾ç¤ºå®æ´ä¼è¯é®ä»¥ä¾¿ `-target` åæ°ä½¿ç¨ -
+(ext_evolution)æ©å±æ§è¡é»è¾ï¼ä»åè®¸ bot é¨åæ´æ°äººè®¾ -
+ä¿®æ­£èæµé»è¾éè¯¯ï¼é¿å bot æ æ³ååºæ¶æ¯çé®é¢ ## [2023/4/
+15] v2.1.1 Minecraft æå¡å¨æä»¤ä¼å - ä¸º `rg chats` æä»¤å¢å äº `-
+show` åæ°ï¼ç¨äºæ¾ç¤ºå®æ´ä¼è¯é®ä»¥ä¾¿ `-target` åæ°ä½¿ç¨ -
 ä¼å MC æå¡å¨æä»¤æ§è¡åé¦ä¿¡æ¯ï¼ä¾¿äº bot èªä¸»çº éï¼ä¼å
 MC æå¡å¨æä»¤é¢å¤çé¿å bot æ·»å å¤ä½çè½¬ä¹ ## [2023/4/15]
 v2.1.0 Minecraft æå¡å¨æ¯æ - å¢å äº Minecraft æå¡å¨æ¥å¥æ¯æ -
 å¢å äº Minecraft æå¡å¨æä»¤æ§è¡æ¯æåç¸å³æ©å±æ¨¡å -
 ä¸ºç»å¾æ©å±å¢å äºä»£çéç½®é¡¹æ¯æ (æè°¢ @tonato-01 æä¾ pr) ##
 [2023/4/6] v2.0.5 RENAME æä»¤ | json å¯¼åºæ¯æ -
 è§£ææ¶æ¯ä¸­ç@æ¶ä¿æä¸ç¨æ·çå°çä¸è´ (æè°¢ @Misaka-Mikoto-
```

