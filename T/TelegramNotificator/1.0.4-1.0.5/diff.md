# Comparing `tmp/TelegramNotificator-1.0.4.tar.gz` & `tmp/TelegramNotificator-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TelegramNotificator-1.0.4.tar", last modified: Sat Apr 15 02:59:21 2023, max compression
+gzip compressed data, was "TelegramNotificator-1.0.5.tar", last modified: Sun Apr 16 21:56:25 2023, max compression
```

## Comparing `TelegramNotificator-1.0.4.tar` & `TelegramNotificator-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 02:59:21.442502 TelegramNotificator-1.0.4/
--rw-rw-rw-   0        0        0     1063 2023-04-15 02:05:41.000000 TelegramNotificator-1.0.4/LICENCE
--rw-rw-rw-   0        0        0      723 2023-04-15 02:59:21.439497 TelegramNotificator-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      659 2023-04-15 02:50:22.000000 TelegramNotificator-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 02:59:21.382216 TelegramNotificator-1.0.4/TelegramNotificator.egg-info/
--rw-rw-rw-   0        0        0      723 2023-04-15 02:59:21.000000 TelegramNotificator-1.0.4/TelegramNotificator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      318 2023-04-15 02:59:21.000000 TelegramNotificator-1.0.4/TelegramNotificator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 02:59:21.000000 TelegramNotificator-1.0.4/TelegramNotificator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-15 02:59:21.000000 TelegramNotificator-1.0.4/TelegramNotificator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-04-15 02:59:21.000000 TelegramNotificator-1.0.4/TelegramNotificator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 02:59:21.442502 TelegramNotificator-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      933 2023-04-15 02:58:56.000000 TelegramNotificator-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-15 02:59:21.385215 TelegramNotificator-1.0.4/telegram_notificator/
--rw-rw-rw-   0        0        0      523 2023-04-15 02:58:12.000000 TelegramNotificator-1.0.4/telegram_notificator/__init__.py
--rw-rw-rw-   0        0        0      524 2023-04-15 02:58:43.000000 TelegramNotificator-1.0.4/telegram_notificator/telegram_notificator.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:56:25.980579 TelegramNotificator-1.0.5/
+-rw-rw-rw-   0        0        0     1063 2023-04-15 02:05:41.000000 TelegramNotificator-1.0.5/LICENCE
+-rw-rw-rw-   0        0        0      786 2023-04-16 21:56:25.980579 TelegramNotificator-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      654 2023-04-15 03:09:06.000000 TelegramNotificator-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 21:56:25.913580 TelegramNotificator-1.0.5/TelegramNotificator.egg-info/
+-rw-rw-rw-   0        0        0      786 2023-04-16 21:56:25.000000 TelegramNotificator-1.0.5/TelegramNotificator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-04-16 21:56:25.000000 TelegramNotificator-1.0.5/TelegramNotificator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 21:56:25.000000 TelegramNotificator-1.0.5/TelegramNotificator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-16 21:56:25.000000 TelegramNotificator-1.0.5/TelegramNotificator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-04-16 21:56:25.000000 TelegramNotificator-1.0.5/TelegramNotificator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 21:56:25.981580 TelegramNotificator-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      996 2023-04-16 21:56:22.000000 TelegramNotificator-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:56:25.947580 TelegramNotificator-1.0.5/telegram_notificator/
+-rw-rw-rw-   0        0        0      523 2023-04-15 02:58:12.000000 TelegramNotificator-1.0.5/telegram_notificator/__init__.py
+-rw-rw-rw-   0        0        0      524 2023-04-15 02:58:43.000000 TelegramNotificator-1.0.5/telegram_notificator/telegram_notificator.py
```

### Comparing `TelegramNotificator-1.0.4/LICENCE` & `TelegramNotificator-1.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `TelegramNotificator-1.0.4/PKG-INFO` & `TelegramNotificator-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: TelegramNotificator
-Version: 1.0.4
+Version: 1.0.5
 Summary: A basic telegram notifications sender.
+Home-page: https://github.com/errais2000/telegram_notificator
 Author: Cryptoroid
 Author-email: 
 License: MIT
 Keywords: telegram,message,notification,alert,send message,telegram message,telegram bot
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TelegramNotificator-1.0.4/TelegramNotificator.egg-info/PKG-INFO` & `TelegramNotificator-1.0.5/TelegramNotificator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: TelegramNotificator
-Version: 1.0.4
+Version: 1.0.5
 Summary: A basic telegram notifications sender.
+Home-page: https://github.com/errais2000/telegram_notificator
 Author: Cryptoroid
 Author-email: 
 License: MIT
 Keywords: telegram,message,notification,alert,send message,telegram message,telegram bot
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TelegramNotificator-1.0.4/setup.py` & `TelegramNotificator-1.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 
 
 # Setting up
 setup(
     name="TelegramNotificator",
-    version='1.0.4',
+    version='1.0.5',
     author="Cryptoroid",
     author_email="",
     license='MIT',
     description='A basic telegram notifications sender.',
     long_description_content_type="text/markdown",
     long_description='Send telegram notifications or alerts from your python programs.',
+    url='https://github.com/errais2000/telegram_notificator',
     packages=find_packages(),
     install_requires=['requests'],
     keywords=['telegram', 'message', 'notification', 'alert', 'send message', 'telegram message', 'telegram bot'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

### Comparing `TelegramNotificator-1.0.4/telegram_notificator/__init__.py` & `TelegramNotificator-1.0.5/telegram_notificator/__init__.py`

 * *Files identical despite different names*

### Comparing `TelegramNotificator-1.0.4/telegram_notificator/telegram_notificator.py` & `TelegramNotificator-1.0.5/telegram_notificator/telegram_notificator.py`

 * *Files identical despite different names*

