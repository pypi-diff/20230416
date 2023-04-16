# Comparing `tmp/SEKKAYBOT-0.22.264.tar.gz` & `tmp/SEKKAYBOT-0.22.265.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SEKKAYBOT-0.22.264.tar", last modified: Sun Apr 16 11:06:31 2023, max compression
+gzip compressed data, was "SEKKAYBOT-0.22.265.tar", last modified: Sun Apr 16 13:32:25 2023, max compression
```

## Comparing `SEKKAYBOT-0.22.264.tar` & `SEKKAYBOT-0.22.265.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 11:06:31.325916 SEKKAYBOT-0.22.264/
--rw-rw-rw-   0        0        0      281 2023-04-16 11:06:31.325916 SEKKAYBOT-0.22.264/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-16 11:06:31.262193 SEKKAYBOT-0.22.264/SEKKAYBOT/
--rw-rw-rw-   0        0        0    54302 2022-12-22 13:43:58.000000 SEKKAYBOT-0.22.264/SEKKAYBOT/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-16 11:06:31.309773 SEKKAYBOT-0.22.264/SEKKAYBOT.egg-info/
--rw-rw-rw-   0        0        0      281 2023-04-16 11:06:31.000000 SEKKAYBOT-0.22.264/SEKKAYBOT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-04-16 11:06:31.000000 SEKKAYBOT-0.22.264/SEKKAYBOT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 11:06:31.000000 SEKKAYBOT-0.22.264/SEKKAYBOT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       93 2023-04-16 11:06:31.000000 SEKKAYBOT-0.22.264/SEKKAYBOT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-16 11:06:31.000000 SEKKAYBOT-0.22.264/SEKKAYBOT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 11:06:31.341640 SEKKAYBOT-0.22.264/setup.cfg
--rw-rw-rw-   0        0        0      593 2023-04-16 11:05:54.000000 SEKKAYBOT-0.22.264/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:32:25.574616 SEKKAYBOT-0.22.265/
+-rw-rw-rw-   0        0        0      281 2023-04-16 13:32:25.543371 SEKKAYBOT-0.22.265/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-16 13:32:25.399602 SEKKAYBOT-0.22.265/SEKKAYBOT/
+-rw-rw-rw-   0        0        0    54303 2023-04-16 11:21:47.000000 SEKKAYBOT-0.22.265/SEKKAYBOT/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 13:32:25.527023 SEKKAYBOT-0.22.265/SEKKAYBOT.egg-info/
+-rw-rw-rw-   0        0        0      281 2023-04-16 13:32:25.000000 SEKKAYBOT-0.22.265/SEKKAYBOT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-04-16 13:32:25.000000 SEKKAYBOT-0.22.265/SEKKAYBOT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 13:32:25.000000 SEKKAYBOT-0.22.265/SEKKAYBOT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-04-16 13:32:25.000000 SEKKAYBOT-0.22.265/SEKKAYBOT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-16 13:32:25.000000 SEKKAYBOT-0.22.265/SEKKAYBOT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 13:32:25.574616 SEKKAYBOT-0.22.265/setup.cfg
+-rw-rw-rw-   0        0        0      594 2023-04-16 13:06:13.000000 SEKKAYBOT-0.22.265/setup.py
```

### Comparing `SEKKAYBOT-0.22.264/SEKKAYBOT/__init__.py` & `SEKKAYBOT-0.22.265/SEKKAYBOT/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     os.system('python -m pip install --upgrade pip')#upgrade pip
     for module in (
         'crayons',
         'PirxcyPinger',
         'fortnitepy==3.6.8',
         'BenBotAsync',
         'FortniteAPIAsync',
-        'sanic==21.6.2',
+        'sanic==22.12.0',
         'aiohttp',
         'requests',
         'aioconsole'
     ):
         subprocess.check_call([sys.executable, "-m", "pip", "install", module])
 
     os.system('clear')
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 colorama import Fore, Back, Style, init init(autoreset=True) from functools
 import partial from datetime import timedelta import crayons try: import
 PirxcyPinger except: pass import fortnitepy import BenBotAsync import
 FortniteAPIAsync import sanic import aiohttp import uvloop import requests
 except ModuleNotFoundError as e: print(f'Error: {e}\nAttempting to install
 packages now (this may take a while).') os.system('python -m pip install --
 upgrade pip')#upgrade pip for module in ( 'crayons', 'PirxcyPinger',
-'fortnitepy==3.6.8', 'BenBotAsync', 'FortniteAPIAsync', 'sanic==21.6.2',
+'fortnitepy==3.6.8', 'BenBotAsync', 'FortniteAPIAsync', 'sanic==22.12.0',
 'aiohttp', 'requests', 'aioconsole' ): subprocess.check_call([sys.executable,
 "-m", "pip", "install", module]) os.system('clear') print('Installed packages,
 restarting script.') python = sys.executable os.execl(python, python,
 *sys.argv) os.system('clear') print(crayons.cyan(f'\nSekkayBOT made by Sekkay &
 Cousin. USE CODE DEXE !'))#ez fix by Mathyslol print(crayons.cyan(f'Discord
 server: discord.gg/tvJtRF25s2 - For support, questions, etc.')) sanic_app =
 sanic.Sanic(__name__) server = None @sanic_app.middleware('response') async def
```

### Comparing `SEKKAYBOT-0.22.264/setup.py` & `SEKKAYBOT-0.22.265/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
     
 setuptools.setup(
     name="SEKKAYBOT",
-    version="0.22.264",
+    version="0.22.265",
     author="Sekkay",
     description="Lobby bot.",
     url="https://www.youtube.com",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
@@ -14,12 +14,12 @@
     ],
     install_requires=[
         'crayons',
         'fortnitepy==3.6.8',
         'BenBotAsync',
         'FortniteAPIAsync',
         'uvloop',
-        'sanic==21.6.2',
+        'sanic==22.12.0',
         'colorama',
         'aiohttp'
     ],
 )
```

