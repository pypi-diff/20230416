# Comparing `tmp/rubpy-5.3.0b0.tar.gz` & `tmp/rubpy-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-5.3.0b0.tar", last modified: Sat Jan 14 19:55:19 2023, max compression
+gzip compressed data, was "rubpy-6.0.0.tar", last modified: Sun Apr 16 00:16:26 2023, max compression
```

## Comparing `rubpy-5.3.0b0.tar` & `rubpy-6.0.0.tar`

### file list

```diff
@@ -1,32 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-01-14 19:55:19.710222 rubpy-5.3.0b0/
--rw-rw-rw-   0        0        0     3452 2023-01-14 19:55:19.710222 rubpy-5.3.0b0/PKG-INFO
--rw-rw-rw-   0        0        0     2246 2022-12-11 19:25:35.000000 rubpy-5.3.0b0/README.md
-drwxrwxrwx   0        0        0        0 2023-01-14 19:55:19.670249 rubpy-5.3.0b0/rubpy/
--rw-rw-rw-   0        0        0      161 2023-01-14 19:54:55.000000 rubpy-5.3.0b0/rubpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-14 19:55:19.697576 rubpy-5.3.0b0/rubpy/client/
--rw-rw-rw-   0        0        0       26 2023-01-14 18:52:14.000000 rubpy-5.3.0b0/rubpy/client/__init__.py
--rw-rw-rw-   0        0        0      522 2023-01-14 19:24:04.000000 rubpy-5.3.0b0/rubpy/client/client.py
-drwxrwxrwx   0        0        0        0 2023-01-14 19:55:19.700519 rubpy-5.3.0b0/rubpy/connections/
--rw-rw-rw-   0        0        0       62 2023-01-14 14:02:21.000000 rubpy-5.3.0b0/rubpy/connections/__init__.py
--rw-rw-rw-   0        0        0     3186 2023-01-14 19:50:58.000000 rubpy-5.3.0b0/rubpy/connections/_http.py
--rw-rw-rw-   0        0        0     2064 2023-01-14 18:53:50.000000 rubpy-5.3.0b0/rubpy/connections/_ws.py
-drwxrwxrwx   0        0        0        0 2023-01-14 19:55:19.702464 rubpy-5.3.0b0/rubpy/crypto/
--rw-rw-rw-   0        0        0       26 2023-01-14 14:06:16.000000 rubpy-5.3.0b0/rubpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     1711 2023-01-14 14:06:03.000000 rubpy-5.3.0b0/rubpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2023-01-14 19:55:19.702464 rubpy-5.3.0b0/rubpy/methods/
--rw-rw-rw-   0        0        0       65 2023-01-14 18:42:23.000000 rubpy-5.3.0b0/rubpy/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-14 19:55:19.705400 rubpy-5.3.0b0/rubpy/methods/advanced/
--rw-rw-rw-   0        0        0       61 2023-01-14 18:30:57.000000 rubpy-5.3.0b0/rubpy/methods/advanced/__init__.py
--rw-rw-rw-   0        0        0     2308 2023-01-14 18:20:56.000000 rubpy-5.3.0b0/rubpy/methods/advanced/make_data.py
--rw-rw-rw-   0        0        0     1307 2023-01-14 19:22:21.000000 rubpy-5.3.0b0/rubpy/methods/advanced/request.py
-drwxrwxrwx   0        0        0        0 2023-01-14 19:55:19.708803 rubpy-5.3.0b0/rubpy/methods/chats/
--rw-rw-rw-   0        0        0       24 2023-01-14 18:42:01.000000 rubpy-5.3.0b0/rubpy/methods/chats/__init__.py
--rw-rw-rw-   0        0        0      413 2023-01-14 19:12:16.000000 rubpy-5.3.0b0/rubpy/methods/chats/chats.py
-drwxrwxrwx   0        0        0        0 2023-01-14 19:55:19.694648 rubpy-5.3.0b0/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3452 2023-01-14 19:55:19.000000 rubpy-5.3.0b0/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-01-14 19:55:19.000000 rubpy-5.3.0b0/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-14 19:55:19.000000 rubpy-5.3.0b0/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-01-14 19:55:19.000000 rubpy-5.3.0b0/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-01-14 19:55:19.000000 rubpy-5.3.0b0/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-14 19:55:19.710222 rubpy-5.3.0b0/setup.cfg
--rw-rw-rw-   0        0        0     1494 2023-01-14 19:54:48.000000 rubpy-5.3.0b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 00:16:26.711695 rubpy-6.0.0/
+-rw-rw-rw-   0        0        0     3548 2023-04-16 00:16:26.711695 rubpy-6.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2455 2023-04-16 00:08:40.000000 rubpy-6.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 00:16:26.711695 rubpy-6.0.0/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3548 2023-04-16 00:16:26.000000 rubpy-6.0.0/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-04-16 00:16:26.000000 rubpy-6.0.0/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 00:16:26.000000 rubpy-6.0.0/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-16 00:16:26.000000 rubpy-6.0.0/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 00:16:26.000000 rubpy-6.0.0/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 00:16:26.711695 rubpy-6.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1568 2023-04-16 00:15:10.000000 rubpy-6.0.0/setup.py
```

### Comparing `rubpy-5.3.0b0/PKG-INFO` & `rubpy-6.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 5.3.0b0
+Version: 6.0.0
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
-Author-email: snipe4kill@yahoo.com
-Keywords: rubika,rubpy,rubikaio,chat,bot,robot,asyncio
+Author-email: contact@shayanheidari.info
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Topic :: Internet
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: ~=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: opencv-python
 
 <p align="center">
     <a href="github.address">
         <img src="https://upcdn.io/W142hJk/thumbnail/demo/4mrDXtYPJA.png.crop" alt="Rubpy" width="128">
     </a>
     <br>
     <b>Rubika API Framework for Python</b>
@@ -71,31 +71,37 @@
     me = await bot.sendMessage('chat_id', 'text')
     print(me)
 
 app.run(my_bot)
 ```
 ### Accounts
 ``` python
-from rubpy import Client
+from rubpy import Client, Methods, Message
 
-app = Client('MY-AUTH')
+app = Client(
+    'MY-AUTH',
+    "my_guid"
+)
 
-@app.handler
-async def my_bot(bot, message):
+@app.MessageUpdates
+async def my_bot(bot: Methods, message: Message):
     await message.reply('``Hello`` __from__ **Rubpy**!')
 
 ```
 
 **Another example:**
 ``` python
-from rubpy import Client
+from rubpy import Client, Methods
 
-app = Client("my_account_auth")
+app = Client(
+    "my_account_auth",
+    "my_account_guid"
+)
 
-async def my_bot(bot):
+async def my_bot(bot: Methods):
     await bot.sendText('object_guid', '``Hello`` __from__ **Rubpy**!')
 
 app.run(my_bot)
 
 ```
 
 **Rubpy** is a modern, elegant and asynchronous framework. It enables you to easily interact with the main Rubika API through a user account (custom client) or a bot
@@ -110,9 +116,9 @@
 - **Fast**: Boosted up by pycryptodome, a high-performance cryptography library written in C.
 - **Async**: Fully asynchronous (also usable synchronously if wanted, for convenience).
 - **Powerful**: Full access to Rubika's API to execute any official client action and more.
 
 ### Installing
 
 ``` bash
-pip3 install rubpy==5.2.0
+pip3 install rubpy==5.2.2
 ```
```

#### html2text {}

```diff
@@ -1,40 +1,40 @@
-Metadata-Version: 2.1 Name: rubpy Version: 5.3.0b0 Summary: This is an
-unofficial library and fastest library for deploying robots on Rubika accounts.
-Home-page: https://github.com/shayanheidari01/rubika Author: Shayan Heidari
-Author-email: snipe4kill@yahoo.com Keywords:
-rubika,rubpy,rubikaio,chat,bot,robot,asyncio Classifier: Programming Language
-:: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Classifier: License :: OSI Approved ::
-GNU Lesser General Public License v3 (LGPLv3) Classifier: Topic :: Internet
-Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
-Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Topic ::
-Software Development :: Libraries :: Application Frameworks Requires-Python:
-~=3.7 Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: rubpy Version: 6.0.0 Summary: This is an unofficial
+library and fastest library for deploying robots on Rubika accounts. Home-page:
+https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
+contact@shayanheidari.info Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: License :: OSI Approved :: GNU Lesser
+General Public License v3 (LGPLv3) Classifier: Topic :: Internet Classifier:
+Topic :: Communications Classifier: Topic :: Communications :: Chat Classifier:
+Topic :: Software Development :: Libraries Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Topic :: Software
+Development :: Libraries :: Application Frameworks Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: opencv-python
                                    [Rubpy]
                        Rubika API Framework for Python
                Homepage â¢ Documentation â¢ Releases â¢ News
 ## Rubpy > Elegant, modern and asynchronous Rubika API framework in Python for
 users and bots ### Bots Examples ```python from rubpy import Bot app = Bot
 ('token') async def my_bot(bot): me = await bot.getMe() print(me) app.run
 (my_bot) ``` **OR** ```python from rubpy import Bot app = Bot('token') async
 def my_bot(bot): me = await bot.sendMessage('chat_id', 'text') print(me)
-app.run(my_bot) ``` ### Accounts ``` python from rubpy import Client app =
-Client('MY-AUTH') @app.handler async def my_bot(bot, message): await
-message.reply('``Hello`` __from__ **Rubpy**!') ``` **Another example:** ```
-python from rubpy import Client app = Client("my_account_auth") async def
-my_bot(bot): await bot.sendText('object_guid', '``Hello`` __from__ **Rubpy**!')
-app.run(my_bot) ``` **Rubpy** is a modern, elegant and asynchronous framework.
-It enables you to easily interact with the main Rubika API through a user
-account (custom client) or a bot identity (bot API alternative) using Python.
-### Key Features - **Ready**: Install Rubpy with pip and start building your
-applications right away. - **Easy**: Makes the Rubika API simple and intuitive,
-while still allowing advanced usages. - **Elegant**: Low-level details are
-abstracted and re-presented in a more convenient way. - **Fast**: Boosted up by
-pycryptodome, a high-performance cryptography library written in C. -
-**Async**: Fully asynchronous (also usable synchronously if wanted, for
-convenience). - **Powerful**: Full access to Rubika's API to execute any
-official client action and more. ### Installing ``` bash pip3 install
-rubpy==5.2.0 ```
+app.run(my_bot) ``` ### Accounts ``` python from rubpy import Client, Methods,
+Message app = Client( 'MY-AUTH', "my_guid" ) @app.MessageUpdates async def
+my_bot(bot: Methods, message: Message): await message.reply('``Hello`` __from__
+**Rubpy**!') ``` **Another example:** ``` python from rubpy import Client,
+Methods app = Client( "my_account_auth", "my_account_guid" ) async def my_bot
+(bot: Methods): await bot.sendText('object_guid', '``Hello`` __from__
+**Rubpy**!') app.run(my_bot) ``` **Rubpy** is a modern, elegant and
+asynchronous framework. It enables you to easily interact with the main Rubika
+API through a user account (custom client) or a bot identity (bot API
+alternative) using Python. ### Key Features - **Ready**: Install Rubpy with pip
+and start building your applications right away. - **Easy**: Makes the Rubika
+API simple and intuitive, while still allowing advanced usages. - **Elegant**:
+Low-level details are abstracted and re-presented in a more convenient way. -
+**Fast**: Boosted up by pycryptodome, a high-performance cryptography library
+written in C. - **Async**: Fully asynchronous (also usable synchronously if
+wanted, for convenience). - **Powerful**: Full access to Rubika's API to
+execute any official client action and more. ### Installing ``` bash pip3
+install rubpy==5.2.2 ```
```

### Comparing `rubpy-5.3.0b0/rubpy.egg-info/PKG-INFO` & `rubpy-6.0.0/rubpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 5.3.0b0
+Version: 6.0.0
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
-Author-email: snipe4kill@yahoo.com
-Keywords: rubika,rubpy,rubikaio,chat,bot,robot,asyncio
+Author-email: contact@shayanheidari.info
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Topic :: Internet
 Classifier: Topic :: Communications
 Classifier: Topic :: Communications :: Chat
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Python: ~=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: opencv-python
 
 <p align="center">
     <a href="github.address">
         <img src="https://upcdn.io/W142hJk/thumbnail/demo/4mrDXtYPJA.png.crop" alt="Rubpy" width="128">
     </a>
     <br>
     <b>Rubika API Framework for Python</b>
@@ -71,31 +71,37 @@
     me = await bot.sendMessage('chat_id', 'text')
     print(me)
 
 app.run(my_bot)
 ```
 ### Accounts
 ``` python
-from rubpy import Client
+from rubpy import Client, Methods, Message
 
-app = Client('MY-AUTH')
+app = Client(
+    'MY-AUTH',
+    "my_guid"
+)
 
-@app.handler
-async def my_bot(bot, message):
+@app.MessageUpdates
+async def my_bot(bot: Methods, message: Message):
     await message.reply('``Hello`` __from__ **Rubpy**!')
 
 ```
 
 **Another example:**
 ``` python
-from rubpy import Client
+from rubpy import Client, Methods
 
-app = Client("my_account_auth")
+app = Client(
+    "my_account_auth",
+    "my_account_guid"
+)
 
-async def my_bot(bot):
+async def my_bot(bot: Methods):
     await bot.sendText('object_guid', '``Hello`` __from__ **Rubpy**!')
 
 app.run(my_bot)
 
 ```
 
 **Rubpy** is a modern, elegant and asynchronous framework. It enables you to easily interact with the main Rubika API through a user account (custom client) or a bot
@@ -110,9 +116,9 @@
 - **Fast**: Boosted up by pycryptodome, a high-performance cryptography library written in C.
 - **Async**: Fully asynchronous (also usable synchronously if wanted, for convenience).
 - **Powerful**: Full access to Rubika's API to execute any official client action and more.
 
 ### Installing
 
 ``` bash
-pip3 install rubpy==5.2.0
+pip3 install rubpy==5.2.2
 ```
```

#### html2text {}

```diff
@@ -1,40 +1,40 @@
-Metadata-Version: 2.1 Name: rubpy Version: 5.3.0b0 Summary: This is an
-unofficial library and fastest library for deploying robots on Rubika accounts.
-Home-page: https://github.com/shayanheidari01/rubika Author: Shayan Heidari
-Author-email: snipe4kill@yahoo.com Keywords:
-rubika,rubpy,rubikaio,chat,bot,robot,asyncio Classifier: Programming Language
-:: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Classifier: License :: OSI Approved ::
-GNU Lesser General Public License v3 (LGPLv3) Classifier: Topic :: Internet
-Classifier: Topic :: Communications Classifier: Topic :: Communications :: Chat
-Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
-Software Development :: Libraries :: Python Modules Classifier: Topic ::
-Software Development :: Libraries :: Application Frameworks Requires-Python:
-~=3.7 Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: rubpy Version: 6.0.0 Summary: This is an unofficial
+library and fastest library for deploying robots on Rubika accounts. Home-page:
+https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
+contact@shayanheidari.info Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3.12 Classifier: License :: OSI Approved :: GNU Lesser
+General Public License v3 (LGPLv3) Classifier: Topic :: Internet Classifier:
+Topic :: Communications Classifier: Topic :: Communications :: Chat Classifier:
+Topic :: Software Development :: Libraries Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Topic :: Software
+Development :: Libraries :: Application Frameworks Requires-Python: >=3.7
+Description-Content-Type: text/markdown Provides-Extra: opencv-python
                                    [Rubpy]
                        Rubika API Framework for Python
                Homepage â¢ Documentation â¢ Releases â¢ News
 ## Rubpy > Elegant, modern and asynchronous Rubika API framework in Python for
 users and bots ### Bots Examples ```python from rubpy import Bot app = Bot
 ('token') async def my_bot(bot): me = await bot.getMe() print(me) app.run
 (my_bot) ``` **OR** ```python from rubpy import Bot app = Bot('token') async
 def my_bot(bot): me = await bot.sendMessage('chat_id', 'text') print(me)
-app.run(my_bot) ``` ### Accounts ``` python from rubpy import Client app =
-Client('MY-AUTH') @app.handler async def my_bot(bot, message): await
-message.reply('``Hello`` __from__ **Rubpy**!') ``` **Another example:** ```
-python from rubpy import Client app = Client("my_account_auth") async def
-my_bot(bot): await bot.sendText('object_guid', '``Hello`` __from__ **Rubpy**!')
-app.run(my_bot) ``` **Rubpy** is a modern, elegant and asynchronous framework.
-It enables you to easily interact with the main Rubika API through a user
-account (custom client) or a bot identity (bot API alternative) using Python.
-### Key Features - **Ready**: Install Rubpy with pip and start building your
-applications right away. - **Easy**: Makes the Rubika API simple and intuitive,
-while still allowing advanced usages. - **Elegant**: Low-level details are
-abstracted and re-presented in a more convenient way. - **Fast**: Boosted up by
-pycryptodome, a high-performance cryptography library written in C. -
-**Async**: Fully asynchronous (also usable synchronously if wanted, for
-convenience). - **Powerful**: Full access to Rubika's API to execute any
-official client action and more. ### Installing ``` bash pip3 install
-rubpy==5.2.0 ```
+app.run(my_bot) ``` ### Accounts ``` python from rubpy import Client, Methods,
+Message app = Client( 'MY-AUTH', "my_guid" ) @app.MessageUpdates async def
+my_bot(bot: Methods, message: Message): await message.reply('``Hello`` __from__
+**Rubpy**!') ``` **Another example:** ``` python from rubpy import Client,
+Methods app = Client( "my_account_auth", "my_account_guid" ) async def my_bot
+(bot: Methods): await bot.sendText('object_guid', '``Hello`` __from__
+**Rubpy**!') app.run(my_bot) ``` **Rubpy** is a modern, elegant and
+asynchronous framework. It enables you to easily interact with the main Rubika
+API through a user account (custom client) or a bot identity (bot API
+alternative) using Python. ### Key Features - **Ready**: Install Rubpy with pip
+and start building your applications right away. - **Easy**: Makes the Rubika
+API simple and intuitive, while still allowing advanced usages. - **Elegant**:
+Low-level details are abstracted and re-presented in a more convenient way. -
+**Fast**: Boosted up by pycryptodome, a high-performance cryptography library
+written in C. - **Async**: Fully asynchronous (also usable synchronously if
+wanted, for convenience). - **Powerful**: Full access to Rubika's API to
+execute any official client action and more. ### Installing ``` bash pip3
+install rubpy==5.2.2 ```
```

