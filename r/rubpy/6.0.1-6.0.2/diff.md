# Comparing `tmp/rubpy-6.0.1.tar.gz` & `tmp/rubpy-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-6.0.1.tar", last modified: Sun Apr 16 00:20:24 2023, max compression
+gzip compressed data, was "rubpy-6.0.2.tar", last modified: Sun Apr 16 01:07:56 2023, max compression
```

## Comparing `rubpy-6.0.1.tar` & `rubpy-6.0.2.tar`

### file list

```diff
@@ -1,11 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 00:20:24.989141 rubpy-6.0.1/
--rw-rw-rw-   0        0        0     3548 2023-04-16 00:20:24.989141 rubpy-6.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2455 2023-04-16 00:08:40.000000 rubpy-6.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 00:20:24.989141 rubpy-6.0.1/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3548 2023-04-16 00:20:24.000000 rubpy-6.0.1/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      162 2023-04-16 00:20:24.000000 rubpy-6.0.1/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 00:20:24.000000 rubpy-6.0.1/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-16 00:20:24.000000 rubpy-6.0.1/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 00:20:24.000000 rubpy-6.0.1/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 00:20:24.989141 rubpy-6.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1436 2023-04-16 00:20:04.000000 rubpy-6.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:07:56.227053 rubpy-6.0.2/
+-rw-rw-rw-   0        0        0     3595 2023-04-16 01:07:56.227053 rubpy-6.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2455 2023-04-16 00:08:40.000000 rubpy-6.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 01:07:56.133322 rubpy-6.0.2/rubpy/
+-rw-rw-rw-   0        0        0      193 2023-04-16 01:07:40.000000 rubpy-6.0.2/rubpy/__init__.py
+-rw-rw-rw-   0        0        0    11974 2023-04-16 00:00:51.000000 rubpy-6.0.2/rubpy/client.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:07:56.148977 rubpy-6.0.2/rubpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.0.2/rubpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 rubpy-6.0.2/rubpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:07:56.164566 rubpy-6.0.2/rubpy/gadgets/
+-rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.0.2/rubpy/gadgets/__init__.py
+-rw-rw-rw-   0        0        0      909 2022-09-12 11:03:20.000000 rubpy-6.0.2/rubpy/gadgets/classino.py
+-rw-rw-rw-   0        0        0     2122 2022-09-12 11:03:20.000000 rubpy-6.0.2/rubpy/gadgets/exceptions.py
+-rw-rw-rw-   0        0        0    12549 2022-09-12 11:03:20.000000 rubpy-6.0.2/rubpy/gadgets/methods.py
+-rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.0.2/rubpy/gadgets/thumbnail.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:07:56.164566 rubpy-6.0.2/rubpy/network/
+-rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.0.2/rubpy/network/__init__.py
+-rw-rw-rw-   0        0        0    10591 2023-04-15 19:45:40.000000 rubpy-6.0.2/rubpy/network/connection.py
+-rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.0.2/rubpy/network/proxies.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:07:56.195840 rubpy-6.0.2/rubpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.0.2/rubpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 rubpy-6.0.2/rubpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.0.2/rubpy/sessions/stringSession.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:07:56.227053 rubpy-6.0.2/rubpy/structs/
+-rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.0.2/rubpy/structs/__init__.py
+-rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.0.2/rubpy/structs/handlers.py
+-rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.0.2/rubpy/structs/models.py
+-rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.0.2/rubpy/structs/results.py
+-rw-rw-rw-   0        0        0    15142 2022-09-12 11:03:20.000000 rubpy-6.0.2/rubpy/structs/struct.py
+drwxrwxrwx   0        0        0        0 2023-04-16 01:07:56.148977 rubpy-6.0.2/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3595 2023-04-16 01:07:55.000000 rubpy-6.0.2/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      671 2023-04-16 01:07:56.000000 rubpy-6.0.2/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 01:07:55.000000 rubpy-6.0.2/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-04-16 01:07:55.000000 rubpy-6.0.2/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-16 01:07:55.000000 rubpy-6.0.2/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 01:07:56.227053 rubpy-6.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1535 2023-04-16 01:07:20.000000 rubpy-6.0.2/setup.py
```

### Comparing `rubpy-6.0.1/PKG-INFO` & `rubpy-6.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.0.1
+Version: 6.0.2
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
+Keywords: rubika,rubpy,chat,bot,robot,asyncio
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
-Requires-Python: >=3.7
+Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: opencv-python
 
 <p align="center">
     <a href="github.address">
         <img src="https://upcdn.io/W142hJk/thumbnail/demo/4mrDXtYPJA.png.crop" alt="Rubpy" width="128">
     </a>
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.0.1 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.0.2 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
-contact@shayanheidari.info Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Classifier: License :: OSI Approved :: GNU Lesser
-General Public License v3 (LGPLv3) Classifier: Topic :: Internet Classifier:
-Topic :: Communications Classifier: Topic :: Communications :: Chat Classifier:
-Topic :: Software Development :: Libraries Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Topic :: Software
-Development :: Libraries :: Application Frameworks Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: opencv-python
+contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3
+(LGPLv3) Classifier: Topic :: Internet Classifier: Topic :: Communications
+Classifier: Topic :: Communications :: Chat Classifier: Topic :: Software
+Development :: Libraries Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Classifier: Topic :: Software Development :: Libraries ::
+Application Frameworks Requires-Python: ~=3.7 Description-Content-Type: text/
+markdown Provides-Extra: opencv-python
                                    [Rubpy]
                        Rubika API Framework for Python
                Homepage â¢ Documentation â¢ Releases â¢ News
 ## Rubpy > Elegant, modern and asynchronous Rubika API framework in Python for
 users and bots ### Bots Examples ```python from rubpy import Bot app = Bot
 ('token') async def my_bot(bot): me = await bot.getMe() print(me) app.run
 (my_bot) ``` **OR** ```python from rubpy import Bot app = Bot('token') async
```

### Comparing `rubpy-6.0.1/README.md` & `rubpy-6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rubpy-6.0.1/rubpy.egg-info/PKG-INFO` & `rubpy-6.0.2/rubpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.0.1
+Version: 6.0.2
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
+Keywords: rubika,rubpy,chat,bot,robot,asyncio
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
-Requires-Python: >=3.7
+Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: opencv-python
 
 <p align="center">
     <a href="github.address">
         <img src="https://upcdn.io/W142hJk/thumbnail/demo/4mrDXtYPJA.png.crop" alt="Rubpy" width="128">
     </a>
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.0.1 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.0.2 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
-contact@shayanheidari.info Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Classifier: License :: OSI Approved :: GNU Lesser
-General Public License v3 (LGPLv3) Classifier: Topic :: Internet Classifier:
-Topic :: Communications Classifier: Topic :: Communications :: Chat Classifier:
-Topic :: Software Development :: Libraries Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Classifier: Topic :: Software
-Development :: Libraries :: Application Frameworks Requires-Python: >=3.7
-Description-Content-Type: text/markdown Provides-Extra: opencv-python
+contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3
+(LGPLv3) Classifier: Topic :: Internet Classifier: Topic :: Communications
+Classifier: Topic :: Communications :: Chat Classifier: Topic :: Software
+Development :: Libraries Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Classifier: Topic :: Software Development :: Libraries ::
+Application Frameworks Requires-Python: ~=3.7 Description-Content-Type: text/
+markdown Provides-Extra: opencv-python
                                    [Rubpy]
                        Rubika API Framework for Python
                Homepage â¢ Documentation â¢ Releases â¢ News
 ## Rubpy > Elegant, modern and asynchronous Rubika API framework in Python for
 users and bots ### Bots Examples ```python from rubpy import Bot app = Bot
 ('token') async def my_bot(bot): me = await bot.getMe() print(me) app.run
 (my_bot) ``` **OR** ```python from rubpy import Bot app = Bot('token') async
```

### Comparing `rubpy-6.0.1/setup.py` & `rubpy-6.0.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from setuptools import find_packages, setup
+from setuptools import setup, find_packages
+
+requirements = ['aiohttp', 'pycryptodome']
 
 with open("README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
-    name='rubpy',
-    version='6.0.1',
+    name = 'rubpy',
+    version = '6.0.2',
     author='Shayan Heidari',
-    url='https://github.com/shayanheidari01/rubika',
     author_email = 'contact@shayanheidari.info',
-    description='This is an unofficial library and fastest library for deploying robots on Rubika accounts.',
-    python_requires='>=3.7',
-    long_description=readme,
+    description = 'This is an unofficial library and fastest library for deploying robots on Rubika accounts.',
+    keywords = ['rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
+    long_description = readme,
+    python_requires="~=3.7",
     long_description_content_type = 'text/markdown',
-    packages=find_packages(exclude=['rubpy*']),
-    install_requires=['aiohttp', 'pycryptodome'],
+    url = 'https://github.com/shayanheidari01/rubika',
+    packages = find_packages(),
+    install_requires = requirements,
     extras_require={
         'opencv-python': ['opencv-python']
     },
     classifiers=[
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

