# Comparing `tmp/nonebot_plugin_treehelp-0.0.5.tar.gz` & `tmp/nonebot_plugin_treehelp-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_treehelp-0.0.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_treehelp-0.1.0.tar", max compression
```

## Comparing `nonebot_plugin_treehelp-0.0.5.tar` & `nonebot_plugin_treehelp-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-03-06 06:08:25.967871 nonebot_plugin_treehelp-0.0.5/LICENSE
--rw-r--r--   0        0        0     2031 2023-03-06 06:08:25.967871 nonebot_plugin_treehelp-0.0.5/README.md
--rw-r--r--   0        0        0     1683 2023-03-06 06:08:25.967871 nonebot_plugin_treehelp-0.0.5/nonebot_plugin_treehelp/__init__.py
--rw-r--r--   0        0        0     4988 2023-03-06 06:08:25.967871 nonebot_plugin_treehelp-0.0.5/nonebot_plugin_treehelp/data_source.py
--rw-r--r--   0        0        0     1312 2023-03-06 06:08:25.967871 nonebot_plugin_treehelp-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2852 1970-01-01 00:00:00.000000 nonebot_plugin_treehelp-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-16 11:21:40.890225 nonebot_plugin_treehelp-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2452 2023-04-16 11:21:40.890225 nonebot_plugin_treehelp-0.1.0/README.md
+-rw-r--r--   0        0        0     1495 2023-04-16 11:21:40.890225 nonebot_plugin_treehelp-0.1.0/nonebot_plugin_treehelp/__init__.py
+-rw-r--r--   0        0        0     4988 2023-04-16 11:21:40.890225 nonebot_plugin_treehelp-0.1.0/nonebot_plugin_treehelp/data_source.py
+-rw-r--r--   0        0        0     1312 2023-04-16 11:21:40.890225 nonebot_plugin_treehelp-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3273 1970-01-01 00:00:00.000000 nonebot_plugin_treehelp-0.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_treehelp-0.0.5/LICENSE` & `nonebot_plugin_treehelp-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_treehelp-0.0.5/README.md` & `nonebot_plugin_treehelp-0.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -43,18 +43,35 @@
 ├── 复杂功能 # 测试插件复杂子插件
 │   └── 二级功能 # 测试插件二级插件
 └── 简单功能 # 测试插件简单子插件
 ```
 
 ## 使用方式
 
-加载插件后发送 `/help` 或 `/help --help` 获取具体用法。
+加载插件后发送 `/help help` 或 `/help --help` 获取具体用法。
+
+## 插件适配
 
 插件与子插件写法可参考 [示例插件](./tests/plugins/tree/)。
 
+### 声明适配器
+
+通过设置 adapters 属性来指定支持的适配器。如果不设置或留空则默认支持全部适配器。如果插件不支持该适配器，则不会在帮助列表上显示。
+
+```python
+__plugin_meta__ = PluginMetadata(
+    name="OneBot",
+    description="测试 OneBot 适配器",
+    usage="/onebot",
+    extra={
+        "adapters": ["OneBot V11"],
+    },
+)
+```
+
 ## 配置项
 
 配置方式：直接在 `NoneBot` 全局配置文件中添加以下配置项即可。
 
 暂时还没有可配置的东西。
 
 ## 计划
```

#### html2text {}

```diff
@@ -5,13 +5,18 @@
 ## ç®ä»
 ä½¿ç¨æä»¶åæ°æ®è·åæä»¶ä¿¡æ¯ï¼å¹¶éè¿æä»¶ä¸å­æä»¶çç»ç»å½¢å¼ï¼æ¥åºåæä»¶çå¤ç§åè½ã
 æ å½¢å¸®å©æä»¶ï¼æéè¦çåè½å½ç¶æ¯æ¾ç¤ºæä»¶æ ï¼ åé `/
 help --tree`ï¼ä½ å°è·å¾å¦ä¸å¸®å©ï¼ ```text æä»¶ï¼ å¸®å© #
 è·åæä»¶å¸®å©ä¿¡æ¯ æµè¯ # ä¸ä¸ªæµè¯æä»¶ âââ å¤æåè½ #
 æµè¯æä»¶å¤æå­æä»¶ â âââ äºçº§åè½ #
 æµè¯æä»¶äºçº§æä»¶ âââ ç®ååè½ # æµè¯æä»¶ç®åå­æä»¶
-``` ## ä½¿ç¨æ¹å¼ å è½½æä»¶ååé `/help` æ `/help --help`
-è·åå·ä½ç¨æ³ã æä»¶ä¸å­æä»¶åæ³å¯åè [ç¤ºä¾æä»¶](./tests/
-plugins/tree/)ã ## éç½®é¡¹ éç½®æ¹å¼ï¼ç´æ¥å¨ `NoneBot`
+``` ## ä½¿ç¨æ¹å¼ å è½½æä»¶ååé `/help help` æ `/help --help`
+è·åå·ä½ç¨æ³ã ## æä»¶éé æä»¶ä¸å­æä»¶åæ³å¯åè
+[ç¤ºä¾æä»¶](./tests/plugins/tree/)ã ### å£°æééå¨ éè¿è®¾ç½®
+adapters
+å±æ§æ¥æå®æ¯æçééå¨ãå¦æä¸è®¾ç½®æçç©ºåé»è®¤æ¯æå¨é¨ééå¨ãå¦ææä»¶ä¸æ¯æè¯¥ééå¨ï¼åä¸ä¼å¨å¸®å©åè¡¨ä¸æ¾ç¤ºã
+```python __plugin_meta__ = PluginMetadata( name="OneBot", description="æµè¯
+OneBot ééå¨", usage="/onebot", extra={ "adapters": ["OneBot V11"], }, )
+``` ## éç½®é¡¹ éç½®æ¹å¼ï¼ç´æ¥å¨ `NoneBot`
 å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã
 ææ¶è¿æ²¡æå¯éç½®çä¸è¥¿ã ## è®¡å - [ ] æ¯æè¾åºæä»¶çæ¬ -
 [x] æ¯æè¾åºæä»¶æ  - [ ] æ¯æè¾åºæä»¶åçå½ä»¤åç§°
```

### Comparing `nonebot_plugin_treehelp-0.0.5/nonebot_plugin_treehelp/__init__.py` & `nonebot_plugin_treehelp-0.1.0/nonebot_plugin_treehelp/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,42 +11,37 @@
 
 from .data_source import get_plugin_help, get_plugin_list
 
 __plugin_meta__ = PluginMetadata(
     name="帮助",
     description="获取插件帮助信息",
     usage="""获取插件列表
-/help -l
-/help --list
+/help
 获取插件树
 /help -t
 /help --tree
 获取某个插件的帮助
 /help 插件名
 获取某个插件的树
 /help --tree 插件名
 """,
 )
 
 parser = ArgumentParser("帮助", description="获取插件帮助信息")
 parser.add_argument("plugin_name", nargs="?", type=str, help="插件名", metavar="插件名")
-parser.add_argument("-l", "--list", action="store_true", help="获取插件列表")
 parser.add_argument("-t", "--tree", action="store_true", help="获取插件树")
 help_cmd = on_shell_command("help", aliases={"帮助"}, parser=parser)
 
 
 @help_cmd.handle()
 async def help_handle(bot: Bot, args: Namespace = ShellCommandArgs()):
     plugin_name = args.plugin_name
 
     if plugin_name is None:
-        if args.list or args.tree:
-            await help_cmd.finish(get_plugin_list(bot, args.tree))
-        else:
-            plugin_name = "帮助"
+        await help_cmd.finish(get_plugin_list(bot, args.tree))
 
     plugin_help = get_plugin_help(bot, plugin_name, args.tree)
     if plugin_help:
         await help_cmd.finish(plugin_help)
     else:
         await help_cmd.finish(f"未找到插件 {plugin_name}")
```

### Comparing `nonebot_plugin_treehelp-0.0.5/nonebot_plugin_treehelp/data_source.py` & `nonebot_plugin_treehelp-0.1.0/nonebot_plugin_treehelp/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_treehelp-0.0.5/pyproject.toml` & `nonebot_plugin_treehelp-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-treehelp"
-version = "0.0.5"
+version = "0.1.0"
 description = "适用于 Nonebot2 的树形帮助插件"
 authors = ["hemengyang <hmy0119@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/he0119/nonebot-plugin-treehelp"
 repository = "https://github.com/he0119/nonebot-plugin-treehelp"
 documentation = "https://github.com/he0119/nonebot-plugin-treehelp#readme"
```

### Comparing `nonebot_plugin_treehelp-0.0.5/PKG-INFO` & `nonebot_plugin_treehelp-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-treehelp
-Version: 0.0.5
+Version: 0.1.0
 Summary: 适用于 Nonebot2 的树形帮助插件
 Home-page: https://github.com/he0119/nonebot-plugin-treehelp
 License: MIT
 Author: hemengyang
 Author-email: hmy0119@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -63,18 +63,35 @@
 ├── 复杂功能 # 测试插件复杂子插件
 │   └── 二级功能 # 测试插件二级插件
 └── 简单功能 # 测试插件简单子插件
 ```
 
 ## 使用方式
 
-加载插件后发送 `/help` 或 `/help --help` 获取具体用法。
+加载插件后发送 `/help help` 或 `/help --help` 获取具体用法。
+
+## 插件适配
 
 插件与子插件写法可参考 [示例插件](./tests/plugins/tree/)。
 
+### 声明适配器
+
+通过设置 adapters 属性来指定支持的适配器。如果不设置或留空则默认支持全部适配器。如果插件不支持该适配器，则不会在帮助列表上显示。
+
+```python
+__plugin_meta__ = PluginMetadata(
+    name="OneBot",
+    description="测试 OneBot 适配器",
+    usage="/onebot",
+    extra={
+        "adapters": ["OneBot V11"],
+    },
+)
+```
+
 ## 配置项
 
 配置方式：直接在 `NoneBot` 全局配置文件中添加以下配置项即可。
 
 暂时还没有可配置的东西。
 
 ## 计划
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-treehelp Version: 0.0.5 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-treehelp Version: 0.1.0 Summary:
 éç¨äº Nonebot2 çæ å½¢å¸®å©æä»¶ Home-page: https://github.com/he0119/
 nonebot-plugin-treehelp License: MIT Author: hemengyang Author-email:
 hmy0119@gmail.com Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: nonebot2
@@ -16,13 +16,18 @@
 ## ç®ä»
 ä½¿ç¨æä»¶åæ°æ®è·åæä»¶ä¿¡æ¯ï¼å¹¶éè¿æä»¶ä¸å­æä»¶çç»ç»å½¢å¼ï¼æ¥åºåæä»¶çå¤ç§åè½ã
 æ å½¢å¸®å©æä»¶ï¼æéè¦çåè½å½ç¶æ¯æ¾ç¤ºæä»¶æ ï¼ åé `/
 help --tree`ï¼ä½ å°è·å¾å¦ä¸å¸®å©ï¼ ```text æä»¶ï¼ å¸®å© #
 è·åæä»¶å¸®å©ä¿¡æ¯ æµè¯ # ä¸ä¸ªæµè¯æä»¶ âââ å¤æåè½ #
 æµè¯æä»¶å¤æå­æä»¶ â âââ äºçº§åè½ #
 æµè¯æä»¶äºçº§æä»¶ âââ ç®ååè½ # æµè¯æä»¶ç®åå­æä»¶
-``` ## ä½¿ç¨æ¹å¼ å è½½æä»¶ååé `/help` æ `/help --help`
-è·åå·ä½ç¨æ³ã æä»¶ä¸å­æä»¶åæ³å¯åè [ç¤ºä¾æä»¶](./tests/
-plugins/tree/)ã ## éç½®é¡¹ éç½®æ¹å¼ï¼ç´æ¥å¨ `NoneBot`
+``` ## ä½¿ç¨æ¹å¼ å è½½æä»¶ååé `/help help` æ `/help --help`
+è·åå·ä½ç¨æ³ã ## æä»¶éé æä»¶ä¸å­æä»¶åæ³å¯åè
+[ç¤ºä¾æä»¶](./tests/plugins/tree/)ã ### å£°æééå¨ éè¿è®¾ç½®
+adapters
+å±æ§æ¥æå®æ¯æçééå¨ãå¦æä¸è®¾ç½®æçç©ºåé»è®¤æ¯æå¨é¨ééå¨ãå¦ææä»¶ä¸æ¯æè¯¥ééå¨ï¼åä¸ä¼å¨å¸®å©åè¡¨ä¸æ¾ç¤ºã
+```python __plugin_meta__ = PluginMetadata( name="OneBot", description="æµè¯
+OneBot ééå¨", usage="/onebot", extra={ "adapters": ["OneBot V11"], }, )
+``` ## éç½®é¡¹ éç½®æ¹å¼ï¼ç´æ¥å¨ `NoneBot`
 å¨å±éç½®æä»¶ä¸­æ·»å ä»¥ä¸éç½®é¡¹å³å¯ã
 ææ¶è¿æ²¡æå¯éç½®çä¸è¥¿ã ## è®¡å - [ ] æ¯æè¾åºæä»¶çæ¬ -
 [x] æ¯æè¾åºæä»¶æ  - [ ] æ¯æè¾åºæä»¶åçå½ä»¤åç§°
```

