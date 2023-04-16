# Comparing `tmp/doveseed-2.0.0a3.tar.gz` & `tmp/doveseed-2.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doveseed-2.0.0a3.tar", max compression
+gzip compressed data, was "doveseed-2.0.0a4.tar", max compression
```

## Comparing `doveseed-2.0.0a3.tar` & `doveseed-2.0.0a4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1068 2023-04-16 14:18:23.163939 doveseed-2.0.0a3/LICENSE
--rw-r--r--   0        0        0     6437 2023-04-16 14:18:23.163939 doveseed-2.0.0a3/README.rst
--rw-r--r--   0        0        0       24 2023-04-16 14:18:23.163939 doveseed-2.0.0a3/doveseed/__init__.py
--rw-r--r--   0        0        0     5797 2023-04-16 14:18:23.163939 doveseed-2.0.0a3/doveseed/app.py
--rw-r--r--   0        0        0     2163 2023-04-16 14:18:23.163939 doveseed-2.0.0a3/doveseed/cli.py
--rw-r--r--   0        0        0      699 2023-04-16 14:18:23.163939 doveseed-2.0.0a3/doveseed/config.py
--rw-r--r--   0        0        0      932 2023-04-16 14:18:23.163939 doveseed-2.0.0a3/doveseed/confirmation.py
--rw-r--r--   0        0        0      765 2023-04-16 14:18:23.163939 doveseed-2.0.0a3/doveseed/domain_types.py
--rw-r--r--   0        0        0     1128 2023-04-16 14:18:23.163939 doveseed-2.0.0a3/doveseed/email_notification.py
--rw-r--r--   0        0        0     3060 2023-04-16 14:18:23.163939 doveseed-2.0.0a3/doveseed/email_templating.py
--rw-r--r--   0        0        0     1289 2023-04-16 14:18:23.163939 doveseed-2.0.0a3/doveseed/feed.py
--rw-r--r--   0        0        0     1287 2023-04-16 14:18:23.163939 doveseed-2.0.0a3/doveseed/notifier.py
--rw-r--r--   0        0        0     2000 2023-04-16 14:18:23.163939 doveseed-2.0.0a3/doveseed/recaptcha.py
--rw-r--r--   0        0        0     3843 2023-04-16 14:18:23.163939 doveseed-2.0.0a3/doveseed/registration.py
--rw-r--r--   0        0        0     2047 2023-04-16 14:18:23.163939 doveseed-2.0.0a3/doveseed/smtp.py
--rw-r--r--   0        0        0     3976 2023-04-16 14:18:23.163939 doveseed-2.0.0a3/doveseed/storage.py
--rw-r--r--   0        0        0      121 2023-04-16 14:18:23.163939 doveseed-2.0.0a3/doveseed/token_gen.py
--rw-r--r--   0        0        0     1172 2023-04-16 14:18:23.167939 doveseed-2.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     7696 1970-01-01 00:00:00.000000 doveseed-2.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-16 15:49:27.910298 doveseed-2.0.0a4/LICENSE
+-rw-r--r--   0        0        0     6437 2023-04-16 15:49:27.910298 doveseed-2.0.0a4/README.rst
+-rw-r--r--   0        0        0       24 2023-04-16 15:49:27.910298 doveseed-2.0.0a4/doveseed/__init__.py
+-rw-r--r--   0        0        0     5797 2023-04-16 15:49:27.910298 doveseed-2.0.0a4/doveseed/app.py
+-rw-r--r--   0        0        0     2163 2023-04-16 15:49:27.910298 doveseed-2.0.0a4/doveseed/cli.py
+-rw-r--r--   0        0        0      699 2023-04-16 15:49:27.910298 doveseed-2.0.0a4/doveseed/config.py
+-rw-r--r--   0        0        0      932 2023-04-16 15:49:27.910298 doveseed-2.0.0a4/doveseed/confirmation.py
+-rw-r--r--   0        0        0      765 2023-04-16 15:49:27.910298 doveseed-2.0.0a4/doveseed/domain_types.py
+-rw-r--r--   0        0        0     1128 2023-04-16 15:49:27.910298 doveseed-2.0.0a4/doveseed/email_notification.py
+-rw-r--r--   0        0        0     3060 2023-04-16 15:49:27.910298 doveseed-2.0.0a4/doveseed/email_templating.py
+-rw-r--r--   0        0        0     1289 2023-04-16 15:49:27.910298 doveseed-2.0.0a4/doveseed/feed.py
+-rw-r--r--   0        0        0     1287 2023-04-16 15:49:27.910298 doveseed-2.0.0a4/doveseed/notifier.py
+-rw-r--r--   0        0        0     2112 2023-04-16 15:49:27.914299 doveseed-2.0.0a4/doveseed/recaptcha.py
+-rw-r--r--   0        0        0     3843 2023-04-16 15:49:27.914299 doveseed-2.0.0a4/doveseed/registration.py
+-rw-r--r--   0        0        0     2047 2023-04-16 15:49:27.914299 doveseed-2.0.0a4/doveseed/smtp.py
+-rw-r--r--   0        0        0     3976 2023-04-16 15:49:27.914299 doveseed-2.0.0a4/doveseed/storage.py
+-rw-r--r--   0        0        0      121 2023-04-16 15:49:27.914299 doveseed-2.0.0a4/doveseed/token_gen.py
+-rw-r--r--   0        0        0     1248 2023-04-16 15:49:27.914299 doveseed-2.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0     7773 1970-01-01 00:00:00.000000 doveseed-2.0.0a4/PKG-INFO
```

### Comparing `doveseed-2.0.0a3/LICENSE` & `doveseed-2.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a3/README.rst` & `doveseed-2.0.0a4/README.rst`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a3/doveseed/app.py` & `doveseed-2.0.0a4/doveseed/app.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a3/doveseed/cli.py` & `doveseed-2.0.0a4/doveseed/cli.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a3/doveseed/config.py` & `doveseed-2.0.0a4/doveseed/config.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a3/doveseed/confirmation.py` & `doveseed-2.0.0a4/doveseed/confirmation.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a3/doveseed/domain_types.py` & `doveseed-2.0.0a4/doveseed/domain_types.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a3/doveseed/email_notification.py` & `doveseed-2.0.0a4/doveseed/email_notification.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a3/doveseed/email_templating.py` & `doveseed-2.0.0a4/doveseed/email_templating.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a3/doveseed/feed.py` & `doveseed-2.0.0a4/doveseed/feed.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a3/doveseed/notifier.py` & `doveseed-2.0.0a4/doveseed/notifier.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a3/doveseed/recaptcha.py` & `doveseed-2.0.0a4/doveseed/recaptcha.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 from typing import Optional
 import re
 import socket
 
 import aiohttp
 from fastapi import Request, status
 from fastapi.responses import PlainTextResponse
+from starlette.middleware.base import BaseHTTPMiddleware
 
 
 Logger = logging.getLogger(__name__)
 
 
-class ReCaptchaMiddleware:
-    def __init__(self, paths, config_path):
+class ReCaptchaMiddleware(BaseHTTPMiddleware):
+    def __init__(self, app, paths, config_path):
+        super().__init__(app)
         self.paths = re.compile(paths)
         with open(config_path, encoding="utf-8") as f:
             config = json.load(f)
         self.valid_hostnames = config["hostnames"]
         self._secret = config["secret"]
 
-    async def __call__(self, request: Request, call_next):
+    async def dispatch(self, request: Request, call_next):
         if self.paths.match(request.url.path) and request.method == "POST":
             data = await request.json()
             # pylint: disable=unsupported-membership-test,unsubscriptable-object
             if data is None or "captcha" not in data:
                 return PlainTextResponse(
                     status_code=status.HTTP_400_BAD_REQUEST, content="Missing captcha."
                 )
```

### Comparing `doveseed-2.0.0a3/doveseed/registration.py` & `doveseed-2.0.0a4/doveseed/registration.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a3/doveseed/smtp.py` & `doveseed-2.0.0a4/doveseed/smtp.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a3/doveseed/storage.py` & `doveseed-2.0.0a4/doveseed/storage.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a3/pyproject.toml` & `doveseed-2.0.0a4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -10,27 +10,28 @@
 ]
 description = "Doveseed is a backend service for email subscriptions to RSS feeds."
 keywords = ["email", "rss", "subscriptions"]
 license = "MIT"
 name = "doveseed"
 readme = "README.rst"
 repository = "https://github.com/jgosmann/doveseed/"
-version = "2.0.0a3" # Also update in doveseed/__init__.py
+version = "2.0.0a4" # Also update in doveseed/__init__.py
 
 [tool.poetry.dependencies]
 aiohttp = {version = "^3.8.4", optional = true}
 fastapi = "^0.95.0"
 jinja2 = "^3.1.2"
 python = "^3.9.0"
+starlette = {version = "0.26.1", optional = true}
 tinydb = "^4.7.0"
 typing_extensions = "^4.3.0"
 
 [tool.poetry.extras]
-all = ['aiohttp']
-recaptcha = ["aiohttp"]
+all = ["aiohttp", "starlette"]
+recaptcha = ["aiohttp", "starlette"]
 
 [tool.poetry.group.dev.dependencies]
 black = "22.8.0"
 httpx = "^0.24.0"
 mypy = "^0.981.0"
 pylint = "^2.15.3"
 pytest = "^7.1.3"
```

### Comparing `doveseed-2.0.0a3/PKG-INFO` & `doveseed-2.0.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doveseed
-Version: 2.0.0a3
+Version: 2.0.0a4
 Summary: Doveseed is a backend service for email subscriptions to RSS feeds.
 Home-page: https://github.com/jgosmann/doveseed/
 License: MIT
 Keywords: email,rss,subscriptions
 Author: Jan Gosmann
 Author-email: jan@hyper-world.de
 Requires-Python: >=3.9.0,<4.0.0
@@ -20,14 +20,15 @@
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Provides-Extra: all
 Provides-Extra: recaptcha
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0) ; extra == "all" or extra == "recaptcha"
 Requires-Dist: fastapi (>=0.95.0,<0.96.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: starlette (==0.26.1) ; extra == "all" or extra == "recaptcha"
 Requires-Dist: tinydb (>=4.7.0,<5.0.0)
 Requires-Dist: typing_extensions (>=4.3.0,<5.0.0)
 Project-URL: Repository, https://github.com/jgosmann/doveseed/
 Description-Content-Type: text/x-rst
 
 .. image:: https://github.com/jgosmann/doveseed/actions/workflows/ci.yml/badge.svg
   :target: https://github.com/jgosmann/doveseed/actions/workflows/ci.yml
```

