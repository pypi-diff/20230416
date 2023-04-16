# Comparing `tmp/nonebot_plugin_bilifan-0.0.2.tar.gz` & `tmp/nonebot_plugin_bilifan-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilifan-0.0.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_bilifan-0.1.0.tar", max compression
```

## Comparing `nonebot_plugin_bilifan-0.0.2.tar` & `nonebot_plugin_bilifan-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35823 2023-04-13 11:46:28.243648 nonebot_plugin_bilifan-0.0.2/LICENSE
--rw-r--r--   0        0        0     2457 2023-04-13 14:32:34.095783 nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/__init__.py
--rw-r--r--   0        0        0     4993 2023-04-13 14:32:49.994527 nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/login/__init__.py
--rw-r--r--   0        0        0     5453 2023-04-13 14:32:34.586527 nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/main.py
--rw-r--r--   0        0        0       54 2023-04-13 11:46:28.244641 nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/src/__init__.py
--rw-r--r--   0        0        0    17462 2023-04-13 14:33:29.648335 nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/src/api.py
--rw-r--r--   0        0        0    17061 2023-04-13 14:33:35.987716 nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/src/user.py
--rw-r--r--   0        0        0     2219 2023-04-13 11:46:28.245642 nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/users.yaml
--rw-r--r--   0        0        0     1098 2023-04-13 14:35:43.118435 nonebot_plugin_bilifan-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2029 2023-04-13 11:46:28.243648 nonebot_plugin_bilifan-0.0.2/README.md
--rw-r--r--   0        0        0     3010 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.0.2/setup.py
--rw-r--r--   0        0        0     3327 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-04-13 11:46:28.243648 nonebot_plugin_bilifan-0.1.0/LICENSE
+-rw-r--r--   0        0        0     5980 2023-04-16 08:59:13.519088 nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/__init__.py
+-rw-r--r--   0        0        0     4993 2023-04-13 14:32:49.994527 nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/login/__init__.py
+-rw-r--r--   0        0        0     4458 2023-04-16 08:49:13.391830 nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/main.py
+-rw-r--r--   0        0        0       54 2023-04-13 11:46:28.244641 nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/src/__init__.py
+-rw-r--r--   0        0        0    17462 2023-04-13 14:33:29.648335 nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/src/api.py
+-rw-r--r--   0        0        0    17061 2023-04-13 14:33:35.987716 nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/src/user.py
+-rw-r--r--   0        0        0     2217 2023-04-16 08:54:25.356364 nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/users.yaml
+-rw-r--r--   0        0        0     1099 2023-04-16 08:59:21.623283 nonebot_plugin_bilifan-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2043 2023-04-16 08:57:26.125573 nonebot_plugin_bilifan-0.1.0/README.md
+-rw-r--r--   0        0        0     3017 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.1.0/setup.py
+-rw-r--r--   0        0        0     3332 1970-01-01 00:00:00.000000 nonebot_plugin_bilifan-0.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilifan-0.0.2/LICENSE` & `nonebot_plugin_bilifan-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/login/__init__.py` & `nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/login/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/main.py` & `nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -46,38 +46,19 @@
             "WATCHINGLIVE": users['WATCHINGLIVE'],
             "WEARMEDAL": users['WEARMEDAL'],
             "SIGNINGROUP": users.get('SIGNINGROUP', 2),
         }
     except Exception as e:
         log.error(f"读取配置文件失败,请检查配置文件格式是否正确: {e}")
         exit(1)
-
+    return users
 
 @log.catch
 async def main(msg_path):
     await read_yaml(msg_path)
-    messageList = []
-    async with aiohttp.ClientSession() as session:
-        try:
-            log.warning("当前版本为: " + __VERSION__)
-            resp = await session.get(
-                "http://version.fansmedalhelper.1961584514352337.cn-hangzhou.fc.devsapp.net/"
-            )
-            data = await resp.json()
-            if data['version'] != __VERSION__:
-                log.warning("新版本为: " + data['version'] + ",请更新")
-                log.warning("更新内容: " + data['changelog'])
-                messageList.append(f"当前版本: {__VERSION__} ,最新版本: {data['version']}")
-                messageList.append(f"更新内容: {data['changelog']} ")
-            if data['notice']:
-                log.warning("公告: " + data['notice'])
-                messageList.append(f"公告: {data['notice']}")
-        except Exception as ex:
-            messageList.append(f"检查版本失败，{ex}")
-            log.warning(f"检查版本失败，{ex}")
     init_tasks = []
     start_tasks = []
     catch_msg = []
 
     for user in users['USERS']:
         if user['access_key']:
             bili_user = BiliUser(user['access_key'], user.get('white_uid', ''), user.get('banned_uid', ''), config)
```

### Comparing `nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/src/api.py` & `nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/src/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/src/user.py` & `nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/src/user.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilifan-0.0.2/nonebot_plugin_bilifan/users.yaml` & `nonebot_plugin_bilifan-0.1.0/nonebot_plugin_bilifan/users.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
       white_uid: 0
       banned_uid: 0
     # 注意对齐
     # 多用户以上格式添加
     # 井号后为注释 井号前后必须有空格！井号前后必须有空格！井号前后必须有空格！
     # 冒号后面也要有空格！冒号前面也要有空格！冒号前面也要有空格！
     # 英文冒号,英文逗号！英文逗号！英文逗号！
-CRON: # 0 0 * * *
+CRON: 0 0 * * *
 # 这里是 cron 表达式, 第一个参数是分钟, 第二个参数是小时
 # 例如每天凌晨0点0分执行一次为 0 0 * * *
 # 如果不填,则不使用内置定时器,填写正确后要保持该进程一直运行
 
 #########以下为自定义配置#########
 ASYNC: 1 # 异步执行,默认异步执行,设置为0则同步执行,开启异步后,将不支持设置点赞CD时间
```

### Comparing `nonebot_plugin_bilifan-0.0.2/pyproject.toml` & `nonebot_plugin_bilifan-0.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_bilifan"
-version = "0.0.2"
+version = "0.1.0"
 description = "刷bili粉丝牌子的机器人插件"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["bilibili", "nonebot2", "plugin"]
@@ -20,15 +20,15 @@
     "LICENSE","README.md"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = "^2.0.0rc4"
 nonebot-adapter-onebot = ">=2.1.5"
-nonebot_plugin_apscheduler = "^0.2.0"
+nonebot_plugin_apscheduler = ">=0.2.0"
 
 pillow = "^9.3.0"
 aiohttp = "^3.8.3"
 aiohttp-socks = "^0.8.0"
 pyyaml = "^6.0"
 qrcode = "^7.4.2"
```

### Comparing `nonebot_plugin_bilifan-0.0.2/README.md` & `nonebot_plugin_bilifan-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,21 +30,23 @@
 
 启动一次插件，在bot路径下，"data/bilifan"文件夹内，按需求修改"users.yaml"文件
 
 ## 指令
 
  - b站登录 - 返回b站二维码，扫码登录，绑定qq号
  - 开始刷牌子 - 开始执行命令
+ - 自动刷牌子 - 添加或取消定时任务
+
 
 </details>
 
 ## 🙈 其他
 
-+ 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr
 + 如果本插件对你有帮助，不要忘了点个Star~
 + 本项目仅供学习使用，请勿用于商业用途
++ [爱发电](https://afdian.net/a/agnes_digital)
 + [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_bilifan/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
         
 
 ## 🌐 感谢
 
 - [新 B 站粉丝牌助手](https://github.com/XiaoMiku01/fansMedalHelper) - 源代码来自于他
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
   # nonebot_plugin_bilifan _â¨èªå¨bç«ç²ä¸çâ¨_ [GitHub_stars] [GitHub
                issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
 ## éç½® å¯å¨ä¸æ¬¡æä»¶ï¼å¨botè·¯å¾ä¸ï¼"data/
 bilifan"æä»¶å¤¹åï¼æéæ±ä¿®æ¹"users.yaml"æä»¶ ## æä»¤ - bç«ç»å½
 - è¿åbç«äºç»´ç ï¼æ«ç ç»å½ï¼ç»å®qqå· - å¼å§å·çå­ -
-å¼å§æ§è¡å½ä»¤  ## ð å¶ä» +
-æ¬äººææ¯å¾å·®ï¼å¦ææ¨æåç°BUGæèæ´å¥½çå»ºè®®ï¼æ¬¢è¿æIssue
-& Pr + å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ +
-æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é + [GPL-3.0 License]
-(https://github.com/Agnes4m/nonebot_plugin_bilifan/blob/main/LICENSE) Â©
-[@Agnes4m](https://github.com/Agnes4m) ## ð æè°¢ - [æ° B
-ç«ç²ä¸çå©æ](https://github.com/XiaoMiku01/fansMedalHelper) -
-æºä»£ç æ¥èªäºä»
+å¼å§æ§è¡å½ä»¤ - èªå¨å·çå­ - æ·»å æåæ¶å®æ¶ä»»å¡  ## ð
+å¶ä» + å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ +
+æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é + [ç±åçµ](https://
+afdian.net/a/agnes_digital) + [GPL-3.0 License](https://github.com/Agnes4m/
+nonebot_plugin_bilifan/blob/main/LICENSE) Â©[@Agnes4m](https://github.com/
+Agnes4m) ## ð æè°¢ - [æ° B ç«ç²ä¸çå©æ](https://github.com/
+XiaoMiku01/fansMedalHelper) - æºä»£ç æ¥èªäºä»
```

### Comparing `nonebot_plugin_bilifan-0.0.2/setup.py` & `nonebot_plugin_bilifan-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp-socks>=0.8.0,<0.9.0',
  'aiohttp>=3.8.3,<4.0.0',
  'nonebot-adapter-onebot>=2.1.5',
  'nonebot2>=2.0.0rc4,<3.0.0',
- 'nonebot_plugin_apscheduler>=0.2.0,<0.3.0',
+ 'nonebot_plugin_apscheduler>=0.2.0',
  'pillow>=9.3.0,<10.0.0',
  'pyyaml>=6.0,<7.0',
  'qrcode>=7.4.2,<8.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-bilifan',
-    'version': '0.0.2',
+    'version': '0.1.0',
     'description': '刷bili粉丝牌子的机器人插件',
-    'long_description': '<div align="center">\n  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_bilifan\n_✨自动b站粉丝牌✨_\n\n<a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_bilifan" alt="stars">\n</a>\n<a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_bilifan" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_bilifan">\n        <img src="https://img.shields.io/pypi/v/nonebot_plugin_bilifan.svg" alt="pypi">\n</a>\n    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc4-red.svg" alt="NoneBot">\n</div>\n\n\n## 配置\n\n启动一次插件，在bot路径下，"data/bilifan"文件夹内，按需求修改"users.yaml"文件\n\n## 指令\n\n - b站登录 - 返回b站二维码，扫码登录，绑定qq号\n - 开始刷牌子 - 开始执行命令\n\n</details>\n\n## 🙈 其他\n\n+ 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr\n+ 如果本插件对你有帮助，不要忘了点个Star~\n+ 本项目仅供学习使用，请勿用于商业用途\n+ [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_bilifan/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)\n        \n\n## 🌐 感谢\n\n- [新 B 站粉丝牌助手](https://github.com/XiaoMiku01/fansMedalHelper) - 源代码来自于他\n',
+    'long_description': '<div align="center">\n  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_bilifan\n_✨自动b站粉丝牌✨_\n\n<a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_bilifan" alt="stars">\n</a>\n<a href="https://github.com/Agnes4m/nonebot_plugin_bilifan/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_bilifan" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_bilifan">\n        <img src="https://img.shields.io/pypi/v/nonebot_plugin_bilifan.svg" alt="pypi">\n</a>\n    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc4-red.svg" alt="NoneBot">\n</div>\n\n\n## 配置\n\n启动一次插件，在bot路径下，"data/bilifan"文件夹内，按需求修改"users.yaml"文件\n\n## 指令\n\n - b站登录 - 返回b站二维码，扫码登录，绑定qq号\n - 开始刷牌子 - 开始执行命令\n - 自动刷牌子 - 添加或取消定时任务\n\n\n</details>\n\n## 🙈 其他\n\n+ 如果本插件对你有帮助，不要忘了点个Star~\n+ 本项目仅供学习使用，请勿用于商业用途\n+ [爱发电](https://afdian.net/a/agnes_digital)\n+ [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_bilifan/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)\n        \n\n## 🌐 感谢\n\n- [新 B 站粉丝牌助手](https://github.com/XiaoMiku01/fansMedalHelper) - 源代码来自于他\n',
     'author': 'Agnes_Digital',
     'author_email': 'Z735803792@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Agnes4m/nonebot_plugin_l4d2_server',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,32 +1,33 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['nonebot_plugin_bilifan', 'nonebot_plugin_bilifan.login',
 'nonebot_plugin_bilifan.src'] package_data = \ {'': ['*']} install_requires = \
 ['aiohttp-socks>=0.8.0,<0.9.0', 'aiohttp>=3.8.3,<4.0.0', 'nonebot-adapter-
 onebot>=2.1.5', 'nonebot2>=2.0.0rc4,<3.0.0',
-'nonebot_plugin_apscheduler>=0.2.0,<0.3.0', 'pillow>=9.3.0,<10.0.0',
+'nonebot_plugin_apscheduler>=0.2.0', 'pillow>=9.3.0,<10.0.0',
 'pyyaml>=6.0,<7.0', 'qrcode>=7.4.2,<8.0.0'] setup_kwargs = { 'name': 'nonebot-
-plugin-bilifan', 'version': '0.0.2', 'description':
+plugin-bilifan', 'version': '0.1.0', 'description':
 'å·biliç²ä¸çå­çæºå¨äººæä»¶', 'long_description': '
                            \n [AgnesDigitalLogo]\n
                                       \n
                               [NoneBotPluginText]
                                       \n
 \n\n
     \n\n# nonebot_plugin_bilifan\n_â¨èªå¨bç«ç²ä¸çâ¨_\n\n\n_[GitHub
 stars]\n\n\n_[GitHub_issues]\n\n\n_[QQ_Chat_Group]\n\n\n_[pypi]\n\n [python]\n
                                   [NoneBot]\n
 \n\n\n## éç½®\n\nå¯å¨ä¸æ¬¡æä»¶ï¼å¨botè·¯å¾ä¸ï¼"data/
 bilifan"æä»¶å¤¹åï¼æéæ±ä¿®æ¹"users.yaml"æä»¶\n\n## æä»¤\n\n -
 bç«ç»å½ - è¿åbç«äºç»´ç ï¼æ«ç ç»å½ï¼ç»å®qqå·\n -
-å¼å§å·çå­ - å¼å§æ§è¡å½ä»¤\n\n\n\n## ð å¶ä»\n\n+
-æ¬äººææ¯å¾å·®ï¼å¦ææ¨æåç°BUGæèæ´å¥½çå»ºè®®ï¼æ¬¢è¿æIssue
-& Pr\n+ å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~\n+
-æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é\n+ [GPL-3.0 License]
-(https://github.com/Agnes4m/nonebot_plugin_bilifan/blob/main/LICENSE) Â©
-[@Agnes4m](https://github.com/Agnes4m)\n \n\n## ð æè°¢\n\n- [æ° B
-ç«ç²ä¸çå©æ](https://github.com/XiaoMiku01/fansMedalHelper) -
-æºä»£ç æ¥èªäºä»\n', 'author': 'Agnes_Digital', 'author_email':
-'Z735803792@163.com', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
-'https://github.com/Agnes4m/nonebot_plugin_l4d2_server', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
+å¼å§å·çå­ - å¼å§æ§è¡å½ä»¤\n - èªå¨å·çå­ -
+æ·»å æåæ¶å®æ¶ä»»å¡\n\n\n\n\n## ð å¶ä»\n\n+
+å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~\n+
+æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é\n+ [ç±åçµ](https://
+afdian.net/a/agnes_digital)\n+ [GPL-3.0 License](https://github.com/Agnes4m/
+nonebot_plugin_bilifan/blob/main/LICENSE) Â©[@Agnes4m](https://github.com/
+Agnes4m)\n \n\n## ð æè°¢\n\n- [æ° B ç«ç²ä¸çå©æ](https://
+github.com/XiaoMiku01/fansMedalHelper) - æºä»£ç æ¥èªäºä»\n', 'author':
+'Agnes_Digital', 'author_email': 'Z735803792@163.com', 'maintainer': 'None',
+'maintainer_email': 'None', 'url': 'https://github.com/Agnes4m/
+nonebot_plugin_l4d2_server', 'packages': packages, 'package_data':
+package_data, 'install_requires': install_requires, 'python_requires':
+'>=3.9,<4.0', } setup(**setup_kwargs)
```

### Comparing `nonebot_plugin_bilifan-0.0.2/PKG-INFO` & `nonebot_plugin_bilifan-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilifan
-Version: 0.0.2
+Version: 0.1.0
 Summary: 刷bili粉丝牌子的机器人插件
 Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 License: GPLv3
 Keywords: bilibili,nonebot2,plugin
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: aiohttp-socks (>=0.8.0,<0.9.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.1.5)
 Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
-Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
+Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0)
 Requires-Dist: pillow (>=9.3.0,<10.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: qrcode (>=7.4.2,<8.0.0)
 Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_l4d2_server
 Description-Content-Type: text/markdown
 
 <div align="center">
@@ -62,22 +62,24 @@
 
 启动一次插件，在bot路径下，"data/bilifan"文件夹内，按需求修改"users.yaml"文件
 
 ## 指令
 
  - b站登录 - 返回b站二维码，扫码登录，绑定qq号
  - 开始刷牌子 - 开始执行命令
+ - 自动刷牌子 - 添加或取消定时任务
+
 
 </details>
 
 ## 🙈 其他
 
-+ 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr
 + 如果本插件对你有帮助，不要忘了点个Star~
 + 本项目仅供学习使用，请勿用于商业用途
++ [爱发电](https://afdian.net/a/agnes_digital)
 + [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_bilifan/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
         
 
 ## 🌐 感谢
 
 - [新 B 站粉丝牌助手](https://github.com/XiaoMiku01/fansMedalHelper) - 源代码来自于他
```

#### html2text {}

```diff
@@ -1,33 +1,32 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilifan Version: 0.0.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilifan Version: 0.1.0 Summary:
 å·biliç²ä¸çå­çæºå¨äººæä»¶ Home-page: https://github.com/Agnes4m/
 nonebot_plugin_l4d2_server License: GPLv3 Keywords: bilibili,nonebot2,plugin
 Author: Agnes_Digital Author-email: Z735803792@163.com Requires-Python:
 >=3.9,<4.0 Classifier: License :: OSI Approved :: GNU General Public License v3
 (GPLv3) Classifier: License :: Other/Proprietary License Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.9 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
 Requires-Dist: aiohttp-socks (>=0.8.0,<0.9.0) Requires-Dist: nonebot-adapter-
 onebot (>=2.1.5) Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0) Requires-Dist:
-nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist: pillow
-(>=9.3.0,<10.0.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: qrcode
-(>=7.4.2,<8.0.0) Project-URL: Repository, https://github.com/Agnes4m/
-nonebot_plugin_l4d2_server Description-Content-Type: text/markdown
+nonebot_plugin_apscheduler (>=0.2.0) Requires-Dist: pillow (>=9.3.0,<10.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: qrcode (>=7.4.2,<8.0.0)
+Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_l4d2_server
+Description-Content-Type: text/markdown
                               [AgnesDigitalLogo]
                               [NoneBotPluginText]
   # nonebot_plugin_bilifan _â¨èªå¨bç«ç²ä¸çâ¨_ [GitHub_stars] [GitHub
                issues] [QQ_Chat_Group] [pypi] [python] [NoneBot]
 ## éç½® å¯å¨ä¸æ¬¡æä»¶ï¼å¨botè·¯å¾ä¸ï¼"data/
 bilifan"æä»¶å¤¹åï¼æéæ±ä¿®æ¹"users.yaml"æä»¶ ## æä»¤ - bç«ç»å½
 - è¿åbç«äºç»´ç ï¼æ«ç ç»å½ï¼ç»å®qqå· - å¼å§å·çå­ -
-å¼å§æ§è¡å½ä»¤  ## ð å¶ä» +
-æ¬äººææ¯å¾å·®ï¼å¦ææ¨æåç°BUGæèæ´å¥½çå»ºè®®ï¼æ¬¢è¿æIssue
-& Pr + å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ +
-æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é + [GPL-3.0 License]
-(https://github.com/Agnes4m/nonebot_plugin_bilifan/blob/main/LICENSE) Â©
-[@Agnes4m](https://github.com/Agnes4m) ## ð æè°¢ - [æ° B
-ç«ç²ä¸çå©æ](https://github.com/XiaoMiku01/fansMedalHelper) -
-æºä»£ç æ¥èªäºä»
+å¼å§æ§è¡å½ä»¤ - èªå¨å·çå­ - æ·»å æåæ¶å®æ¶ä»»å¡  ## ð
+å¶ä» + å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ +
+æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é + [ç±åçµ](https://
+afdian.net/a/agnes_digital) + [GPL-3.0 License](https://github.com/Agnes4m/
+nonebot_plugin_bilifan/blob/main/LICENSE) Â©[@Agnes4m](https://github.com/
+Agnes4m) ## ð æè°¢ - [æ° B ç«ç²ä¸çå©æ](https://github.com/
+XiaoMiku01/fansMedalHelper) - æºä»£ç æ¥èªäºä»
```

