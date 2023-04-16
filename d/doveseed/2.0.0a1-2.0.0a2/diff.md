# Comparing `tmp/doveseed-2.0.0a1.tar.gz` & `tmp/doveseed-2.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doveseed-2.0.0a1.tar", max compression
+gzip compressed data, was "doveseed-2.0.0a2.tar", max compression
```

## Comparing `doveseed-2.0.0a1.tar` & `doveseed-2.0.0a2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1068 2023-04-16 13:49:07.941987 doveseed-2.0.0a1/LICENSE
--rw-r--r--   0        0        0     6379 2023-04-16 13:49:07.941987 doveseed-2.0.0a1/README.rst
--rw-r--r--   0        0        0       24 2023-04-16 13:49:07.941987 doveseed-2.0.0a1/doveseed/__init__.py
--rw-r--r--   0        0        0     5797 2023-04-16 13:49:07.941987 doveseed-2.0.0a1/doveseed/app.py
--rw-r--r--   0        0        0     2163 2023-04-16 13:49:07.941987 doveseed-2.0.0a1/doveseed/cli.py
--rw-r--r--   0        0        0      685 2023-04-16 13:49:07.941987 doveseed-2.0.0a1/doveseed/config.py
--rw-r--r--   0        0        0      932 2023-04-16 13:49:07.941987 doveseed-2.0.0a1/doveseed/confirmation.py
--rw-r--r--   0        0        0      765 2023-04-16 13:49:07.941987 doveseed-2.0.0a1/doveseed/domain_types.py
--rw-r--r--   0        0        0     1128 2023-04-16 13:49:07.941987 doveseed-2.0.0a1/doveseed/email_notification.py
--rw-r--r--   0        0        0     3060 2023-04-16 13:49:07.941987 doveseed-2.0.0a1/doveseed/email_templating.py
--rw-r--r--   0        0        0     1289 2023-04-16 13:49:07.941987 doveseed-2.0.0a1/doveseed/feed.py
--rw-r--r--   0        0        0     1287 2023-04-16 13:49:07.941987 doveseed-2.0.0a1/doveseed/notifier.py
--rw-r--r--   0        0        0     2000 2023-04-16 13:49:07.941987 doveseed-2.0.0a1/doveseed/recaptcha.py
--rw-r--r--   0        0        0     3843 2023-04-16 13:49:07.941987 doveseed-2.0.0a1/doveseed/registration.py
--rw-r--r--   0        0        0     2047 2023-04-16 13:49:07.941987 doveseed-2.0.0a1/doveseed/smtp.py
--rw-r--r--   0        0        0     3976 2023-04-16 13:49:07.941987 doveseed-2.0.0a1/doveseed/storage.py
--rw-r--r--   0        0        0      121 2023-04-16 13:49:07.941987 doveseed-2.0.0a1/doveseed/token_gen.py
--rw-r--r--   0        0        0     1172 2023-04-16 13:49:07.945987 doveseed-2.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     7638 1970-01-01 00:00:00.000000 doveseed-2.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-16 14:05:55.606673 doveseed-2.0.0a2/LICENSE
+-rw-r--r--   0        0        0     6379 2023-04-16 14:05:55.606673 doveseed-2.0.0a2/README.rst
+-rw-r--r--   0        0        0       24 2023-04-16 14:05:55.606673 doveseed-2.0.0a2/doveseed/__init__.py
+-rw-r--r--   0        0        0     5797 2023-04-16 14:05:55.606673 doveseed-2.0.0a2/doveseed/app.py
+-rw-r--r--   0        0        0     2163 2023-04-16 14:05:55.606673 doveseed-2.0.0a2/doveseed/cli.py
+-rw-r--r--   0        0        0      685 2023-04-16 14:05:55.606673 doveseed-2.0.0a2/doveseed/config.py
+-rw-r--r--   0        0        0      932 2023-04-16 14:05:55.606673 doveseed-2.0.0a2/doveseed/confirmation.py
+-rw-r--r--   0        0        0      765 2023-04-16 14:05:55.606673 doveseed-2.0.0a2/doveseed/domain_types.py
+-rw-r--r--   0        0        0     1128 2023-04-16 14:05:55.606673 doveseed-2.0.0a2/doveseed/email_notification.py
+-rw-r--r--   0        0        0     3060 2023-04-16 14:05:55.606673 doveseed-2.0.0a2/doveseed/email_templating.py
+-rw-r--r--   0        0        0     1289 2023-04-16 14:05:55.606673 doveseed-2.0.0a2/doveseed/feed.py
+-rw-r--r--   0        0        0     1287 2023-04-16 14:05:55.606673 doveseed-2.0.0a2/doveseed/notifier.py
+-rw-r--r--   0        0        0     2000 2023-04-16 14:05:55.606673 doveseed-2.0.0a2/doveseed/recaptcha.py
+-rw-r--r--   0        0        0     3843 2023-04-16 14:05:55.606673 doveseed-2.0.0a2/doveseed/registration.py
+-rw-r--r--   0        0        0     2047 2023-04-16 14:05:55.606673 doveseed-2.0.0a2/doveseed/smtp.py
+-rw-r--r--   0        0        0     3976 2023-04-16 14:05:55.606673 doveseed-2.0.0a2/doveseed/storage.py
+-rw-r--r--   0        0        0      121 2023-04-16 14:05:55.606673 doveseed-2.0.0a2/doveseed/token_gen.py
+-rw-r--r--   0        0        0     1172 2023-04-16 14:05:55.606673 doveseed-2.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     7638 1970-01-01 00:00:00.000000 doveseed-2.0.0a2/PKG-INFO
```

### Comparing `doveseed-2.0.0a1/LICENSE` & `doveseed-2.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a1/README.rst` & `doveseed-2.0.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a1/doveseed/app.py` & `doveseed-2.0.0a2/doveseed/app.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a1/doveseed/cli.py` & `doveseed-2.0.0a2/doveseed/cli.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a1/doveseed/config.py` & `doveseed-2.0.0a2/doveseed/config.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a1/doveseed/confirmation.py` & `doveseed-2.0.0a2/doveseed/confirmation.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a1/doveseed/domain_types.py` & `doveseed-2.0.0a2/doveseed/domain_types.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a1/doveseed/email_notification.py` & `doveseed-2.0.0a2/doveseed/email_notification.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a1/doveseed/email_templating.py` & `doveseed-2.0.0a2/doveseed/email_templating.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a1/doveseed/feed.py` & `doveseed-2.0.0a2/doveseed/feed.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a1/doveseed/notifier.py` & `doveseed-2.0.0a2/doveseed/notifier.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a1/doveseed/recaptcha.py` & `doveseed-2.0.0a2/doveseed/recaptcha.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a1/doveseed/registration.py` & `doveseed-2.0.0a2/doveseed/registration.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a1/doveseed/smtp.py` & `doveseed-2.0.0a2/doveseed/smtp.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a1/doveseed/storage.py` & `doveseed-2.0.0a2/doveseed/storage.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a1/pyproject.toml` & `doveseed-2.0.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ]
 description = "Doveseed is a backend service for email subscriptions to RSS feeds."
 keywords = ["email", "rss", "subscriptions"]
 license = "MIT"
 name = "doveseed"
 readme = "README.rst"
 repository = "https://github.com/jgosmann/doveseed/"
-version = "2.0.0a1" # Also update in doveseed/__init__.py
+version = "2.0.0a2" # Also update in doveseed/__init__.py
 
 [tool.poetry.dependencies]
 aiohttp = {version = "^3.8.4", optional = true}
 fastapi = "^0.95.0"
 jinja2 = "^3.1.2"
 python = "^3.9.0"
 tinydb = "^4.7.0"
```

### Comparing `doveseed-2.0.0a1/PKG-INFO` & `doveseed-2.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doveseed
-Version: 2.0.0a1
+Version: 2.0.0a2
 Summary: Doveseed is a backend service for email subscriptions to RSS feeds.
 Home-page: https://github.com/jgosmann/doveseed/
 License: MIT
 Keywords: email,rss,subscriptions
 Author: Jan Gosmann
 Author-email: jan@hyper-world.de
 Requires-Python: >=3.9.0,<4.0.0
```

