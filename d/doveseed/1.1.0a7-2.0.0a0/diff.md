# Comparing `tmp/doveseed-1.1.0a7.tar.gz` & `tmp/doveseed-2.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doveseed-1.1.0a7.tar", max compression
+gzip compressed data, was "doveseed-2.0.0a0.tar", max compression
```

## Comparing `doveseed-1.1.0a7.tar` & `doveseed-2.0.0a0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1068 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/LICENSE
--rw-r--r--   0        0        0     6426 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/README.rst
--rw-r--r--   0        0        0       22 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/__init__.py
--rw-r--r--   0        0        0     3313 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/app.py
--rw-r--r--   0        0        0     2163 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/cli.py
--rw-r--r--   0        0        0      932 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/confirmation.py
--rw-r--r--   0        0        0      765 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/domain_types.py
--rw-r--r--   0        0        0     1128 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/email_notification.py
--rw-r--r--   0        0        0     3060 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/email_templating.py
--rw-r--r--   0        0        0     1289 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/feed.py
--rw-r--r--   0        0        0     1287 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/notifier.py
--rw-r--r--   0        0        0     2173 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/recaptcha.py
--rw-r--r--   0        0        0     3843 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/registration.py
--rw-r--r--   0        0        0     2047 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/smtp.py
--rw-r--r--   0        0        0     3976 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/storage.py
--rw-r--r--   0        0        0      121 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/doveseed/token_gen.py
--rw-r--r--   0        0        0     1059 2023-03-05 14:41:03.247859 doveseed-1.1.0a7/pyproject.toml
--rw-r--r--   0        0        0     7684 1970-01-01 00:00:00.000000 doveseed-1.1.0a7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-16 13:28:29.253062 doveseed-2.0.0a0/LICENSE
+-rw-r--r--   0        0        0     6379 2023-04-16 13:28:29.253062 doveseed-2.0.0a0/README.rst
+-rw-r--r--   0        0        0       24 2023-04-16 13:28:29.253062 doveseed-2.0.0a0/doveseed/__init__.py
+-rw-r--r--   0        0        0     5797 2023-04-16 13:28:29.253062 doveseed-2.0.0a0/doveseed/app.py
+-rw-r--r--   0        0        0     2163 2023-04-16 13:28:29.253062 doveseed-2.0.0a0/doveseed/cli.py
+-rw-r--r--   0        0        0      685 2023-04-16 13:28:29.253062 doveseed-2.0.0a0/doveseed/config.py
+-rw-r--r--   0        0        0      932 2023-04-16 13:28:29.253062 doveseed-2.0.0a0/doveseed/confirmation.py
+-rw-r--r--   0        0        0      765 2023-04-16 13:28:29.253062 doveseed-2.0.0a0/doveseed/domain_types.py
+-rw-r--r--   0        0        0     1128 2023-04-16 13:28:29.253062 doveseed-2.0.0a0/doveseed/email_notification.py
+-rw-r--r--   0        0        0     3060 2023-04-16 13:28:29.253062 doveseed-2.0.0a0/doveseed/email_templating.py
+-rw-r--r--   0        0        0     1289 2023-04-16 13:28:29.253062 doveseed-2.0.0a0/doveseed/feed.py
+-rw-r--r--   0        0        0     1287 2023-04-16 13:28:29.253062 doveseed-2.0.0a0/doveseed/notifier.py
+-rw-r--r--   0        0        0     2000 2023-04-16 13:28:29.253062 doveseed-2.0.0a0/doveseed/recaptcha.py
+-rw-r--r--   0        0        0     3843 2023-04-16 13:28:29.253062 doveseed-2.0.0a0/doveseed/registration.py
+-rw-r--r--   0        0        0     2047 2023-04-16 13:28:29.253062 doveseed-2.0.0a0/doveseed/smtp.py
+-rw-r--r--   0        0        0     3976 2023-04-16 13:28:29.253062 doveseed-2.0.0a0/doveseed/storage.py
+-rw-r--r--   0        0        0      121 2023-04-16 13:28:29.253062 doveseed-2.0.0a0/doveseed/token_gen.py
+-rw-r--r--   0        0        0     1172 2023-04-16 13:28:29.257062 doveseed-2.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0     7638 1970-01-01 00:00:00.000000 doveseed-2.0.0a0/PKG-INFO
```

### Comparing `doveseed-1.1.0a7/LICENSE` & `doveseed-2.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a7/README.rst` & `doveseed-2.0.0a0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -26,25 +26,23 @@
 
 Configuration
 ^^^^^^^^^^^^^
 
 Doveseed requires a configuration file in JSON format. Take a look at
 ``config.sample.json``. The format is as follows:
 
-* ``cors``: Maybe omitted to disable CORS headers. If given, will be passed to
-  ``CORS`` constructor of `flask-cors <https://flask-cors.readthedocs.io/en/latest/>`_.
 * ``db``: JSON file in which Doveseed persists its data.
 * ``rss``: URL to the RSS feed for which new notifications are to be send.
 * ``smtp``
 
   * ``host``: SMTP host used to send notification emails.
   * ``user``: SMTP logon user name.
   * ``password``: SMTP logon password.
-  * ``ssl_mode``: Activate/deactivate SSL/TLS, valid values `"no-ssl"`, `"start-tls"`, `"tls"` (default `"start-tls"`).
-  * ``check_hostname``: Whether to verify the hostname when using TLS (default `true`).
+  * ``ssl_mode``: Activate/deactivate SSL/TLS, valid values ``"no-ssl"``, ``"start-tls"``, ``"tls"`` (default ``"start-tls"``).
+  * ``check_hostname``: Whether to verify the hostname when using TLS (default ``true``).
 
 * ``template_vars``: Defines template variables to replace in the email templates.
 
   * ``display_name``: Name for the website to use in emails.
   * ``host``: Hostname of the website.
   * ``sender``: Email address that is sending the notifications.
   * ``confirm_url_format``: Template for the URL that is used for confirmation
@@ -83,52 +81,56 @@
 * and ``*.html``: for the HTML version of the email.
 
 
 
 REST service
 ^^^^^^^^^^^^
 
-The REST service runs as a Python WSGI app. Any WSGI app server could be used.
+The REST service runs as a Python `ASGI app
+<https://asgi.readthedocs.io/en/latest/>`_. See the FastAPI documentation for
+`deployment options <https://fastapi.tiangolo.com/deployment/>`_.
 
-Passenger
-~~~~~~~~~
-
-Sample ``passenger_wsgi.py`` file::
-
-    import logging
-    logging.basicConfig(filename="/path/to/log", level=logging.WARN)
-
-    from doveseed.app import create_app
-    application = create_app()
 
 
 CORS
 ~~~~
 
-To set appropriate CORS headers use the
-`flask-cors <https://flask-cors.readthedocs.io/en/latest/>`_ package.
-Activate it by adding the following lines to the file where you instantiate
-the app, for example your ``passenger_wsgi.py`` file::
-
-    from flask_cors import CORS
-    CORS(application, origins=["https://my-domain.tld"])
+To set appropriate CORS headers use the `FastAPI CORSMiddleware
+<https://fastapi.tiangolo.com/tutorial/cors/>`_. Activate it by adding the
+following lines to the file where you instantiate the app::
+
+    from doveseed.app import app
+    from fastapi.middleware.cors import CORSMiddleware
+
+    app.add_middleware(
+        CORSMiddleware,
+        allow_origins=["http://example.com"],
+        allow_methods=["GET", "POST"],
+        allow_headers=["Authorization"],
+    )
 
 
 ReCaptcha
 ~~~~~~~~~
 
-To activate `ReCaptcha (v2) <https://www.google.com/recaptcha/>`_ verification of
-requests, add the follwing lines to the file where you instantiate the app,
-for example your ``passenger_wsgi.py`` file::
+You activate `ReCaptcha (v2) <https://www.google.com/recaptcha/>`_ verification of
+requests with Doveseed.
 
+First, you need to install the required optional dependencies::
+
+    pip install 'doveseed[recaptcha]'
+
+Then, add the follwing lines to the file where you instantiate the app::
+
+    from doveseed.app import app
     from doveseed.recaptcha import ReCaptchaMiddleware
-    application.wsgi_app = ReCaptchaMiddleware(
-        application.wsgi_app, '^/(un)?subscribe/.*', 'recaptcha.json')
 
-Also, create the ``recaptcha.json`` with the required ReCaptcha configuration::
+    app.add_middleware = ReCaptchaMiddleware('^/(un)?subscribe/.*', 'recaptcha.json')
+
+Also, create the ``recaptcha.json`` with the required ReCaptcha configuration:
 
 * ``hostnames``: List of hostnames to accept ReCaptchas from.
 * ``secret``: The shared key between your site and reCAPTCHA.
 
 
 **Ensure that the configuration files have appropriate permissions, i.e. only
 readable by you and Doveseed.**
```

### Comparing `doveseed-1.1.0a7/doveseed/cli.py` & `doveseed-2.0.0a0/doveseed/cli.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a7/doveseed/confirmation.py` & `doveseed-2.0.0a0/doveseed/confirmation.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a7/doveseed/domain_types.py` & `doveseed-2.0.0a0/doveseed/domain_types.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a7/doveseed/email_notification.py` & `doveseed-2.0.0a0/doveseed/email_notification.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a7/doveseed/email_templating.py` & `doveseed-2.0.0a0/doveseed/email_templating.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a7/doveseed/feed.py` & `doveseed-2.0.0a0/doveseed/feed.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a7/doveseed/notifier.py` & `doveseed-2.0.0a0/doveseed/notifier.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a7/doveseed/recaptcha.py` & `doveseed-2.0.0a0/doveseed/recaptcha.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,58 +1,53 @@
-import http
 import json
 import logging
 from typing import Optional
-import urllib.request
-from urllib.parse import urlencode
 import re
+import socket
 
-from werkzeug.wrappers import Request, Response
+import aiohttp
+from fastapi import Request, status
+from fastapi.responses import PlainTextResponse
 
 
 Logger = logging.getLogger(__name__)
 
 
 class ReCaptchaMiddleware:
-    def __init__(self, app, paths, config_path):
-        self.app = app
+    def __init__(self, paths, config_path):
         self.paths = re.compile(paths)
         with open(config_path, encoding="utf-8") as f:
             config = json.load(f)
         self.valid_hostnames = config["hostnames"]
         self._secret = config["secret"]
 
-    def __call__(self, environ, start_response):
-        request = Request(environ)
-        if self.paths.match(request.path) and request.method == "POST":
-            data = request.get_json()
+    async def __call__(self, request: Request, call_next):
+        if self.paths.match(request.url.path) and request.method == "POST":
+            data = await request.json()
             # pylint: disable=unsupported-membership-test,unsubscriptable-object
             if data is None or "captcha" not in data:
-                return self._to_response(
-                    environ,
-                    start_response,
-                    ("Missing captcha.", http.HTTPStatus.BAD_REQUEST),
+                return PlainTextResponse(
+                    status_code=status.HTTP_400_BAD_REQUEST, content="Missing captcha."
                 )
-            if not self.verify_captcha(data["captcha"], request.remote_addr):
-                return self._to_response(
-                    environ,
-                    start_response,
-                    ("Invalid captcha.", http.HTTPStatus.UNAUTHORIZED),
+            if not await self.verify_captcha(
+                data["captcha"],
+                socket.gethostbyname(request.client.host) if request.client else None,
+            ):
+                return PlainTextResponse(
+                    status_code=status.HTTP_401_UNAUTHORIZED, content="Invalid captcha."
                 )
-        return self.app(environ, start_response)
+        return await call_next(request)
 
-    def verify_captcha(self, captcha: str, remote_ip: Optional[str]):
-        verification_request = urllib.request.Request(
-            "https://www.google.com/recaptcha/api/siteverify",
-            method="POST",
-            data=urlencode(
-                {"secret": self._secret, "response": captcha, "remoteip": remote_ip}
-            ).encode("ascii"),
-        )
-        with urllib.request.urlopen(verification_request) as f:
-            result = json.loads(f.read())
+    async def verify_captcha(self, captcha: str, remote_ip: Optional[str]):
+        async with aiohttp.ClientSession() as session:
+            async with session.post(
+                "https://www.google.com/recaptcha/api/siteverify",
+                data={
+                    "secret": self._secret,
+                    "response": captcha,
+                    "remoteip": remote_ip,
+                },
+            ) as response:
+                result = await response.json()
         if len(result.get("error-codes", [])) > 0:
             Logger.warning(result["error-codes"])
         return result["success"] and result["hostname"] in self.valid_hostnames
-
-    def _to_response(self, environ, start_response, response):
-        return Response(*response)(environ, start_response)
```

### Comparing `doveseed-1.1.0a7/doveseed/registration.py` & `doveseed-2.0.0a0/doveseed/registration.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a7/doveseed/smtp.py` & `doveseed-2.0.0a0/doveseed/smtp.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a7/doveseed/storage.py` & `doveseed-2.0.0a0/doveseed/storage.py`

 * *Files identical despite different names*

### Comparing `doveseed-1.1.0a7/pyproject.toml` & `doveseed-2.0.0a0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 [tool.poetry]
 authors = ["Jan Gosmann <jan@hyper-world.de>"]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Framework :: Flask",
   "Intended Audience :: Developers",
-  "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3 :: Only",
   "Topic :: Communications :: Email",
   "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
 ]
 description = "Doveseed is a backend service for email subscriptions to RSS feeds."
 keywords = ["email", "rss", "subscriptions"]
 license = "MIT"
 name = "doveseed"
 readme = "README.rst"
 repository = "https://github.com/jgosmann/doveseed/"
-version = "1.1.0a7"
+version = "2.0.0a0" # Also update in doveseed/__init__.py
 
 [tool.poetry.dependencies]
-Werkzeug = "^2.2.2"
-flask = "^2.2.2"
-flask_cors = "^3.0"
+aiohttp = {version = "^3.8.4", optional = true}
+fastapi = "^0.95.0"
 jinja2 = "^3.1.2"
-python = "^3.7.2"
+python = "^3.9.0"
 tinydb = "^4.7.0"
 typing_extensions = "^4.3.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.extras]
+all = ['aiohttp']
+recaptcha = ["aiohttp"]
+
+[tool.poetry.group.dev.dependencies]
 black = "22.8.0"
+httpx = "^0.24.0"
 mypy = "^0.981.0"
 pylint = "^2.15.3"
 pytest = "^7.1.3"
 pytest-cov = "^4.0.0"
 pytest-emoji = "^0.2.0"
 pytest-mypy = "^0.10.0"
+uvicorn = "^0.21.1"
 
 [build-system]
 build-backend = "poetry.masonry.api"
 requires = ["poetry>=0.12"]
```

### Comparing `doveseed-1.1.0a7/PKG-INFO` & `doveseed-2.0.0a0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: doveseed
-Version: 1.1.0a7
+Version: 2.0.0a0
 Summary: Doveseed is a backend service for email subscriptions to RSS feeds.
 Home-page: https://github.com/jgosmann/doveseed/
 License: MIT
 Keywords: email,rss,subscriptions
 Author: Jan Gosmann
 Author-email: jan@hyper-world.de
-Requires-Python: >=3.7.2,<4.0.0
+Requires-Python: >=3.9.0,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
-Requires-Dist: Werkzeug (>=2.2.2,<3.0.0)
-Requires-Dist: flask (>=2.2.2,<3.0.0)
-Requires-Dist: flask_cors (>=3.0,<4.0)
+Provides-Extra: all
+Provides-Extra: recaptcha
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0) ; extra == "all" or extra == "recaptcha"
+Requires-Dist: fastapi (>=0.95.0,<0.96.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: tinydb (>=4.7.0,<5.0.0)
 Requires-Dist: typing_extensions (>=4.3.0,<5.0.0)
 Project-URL: Repository, https://github.com/jgosmann/doveseed/
 Description-Content-Type: text/x-rst
 
 .. image:: https://github.com/jgosmann/doveseed/actions/workflows/ci.yml/badge.svg
@@ -57,25 +57,23 @@
 
 Configuration
 ^^^^^^^^^^^^^
 
 Doveseed requires a configuration file in JSON format. Take a look at
 ``config.sample.json``. The format is as follows:
 
-* ``cors``: Maybe omitted to disable CORS headers. If given, will be passed to
-  ``CORS`` constructor of `flask-cors <https://flask-cors.readthedocs.io/en/latest/>`_.
 * ``db``: JSON file in which Doveseed persists its data.
 * ``rss``: URL to the RSS feed for which new notifications are to be send.
 * ``smtp``
 
   * ``host``: SMTP host used to send notification emails.
   * ``user``: SMTP logon user name.
   * ``password``: SMTP logon password.
-  * ``ssl_mode``: Activate/deactivate SSL/TLS, valid values `"no-ssl"`, `"start-tls"`, `"tls"` (default `"start-tls"`).
-  * ``check_hostname``: Whether to verify the hostname when using TLS (default `true`).
+  * ``ssl_mode``: Activate/deactivate SSL/TLS, valid values ``"no-ssl"``, ``"start-tls"``, ``"tls"`` (default ``"start-tls"``).
+  * ``check_hostname``: Whether to verify the hostname when using TLS (default ``true``).
 
 * ``template_vars``: Defines template variables to replace in the email templates.
 
   * ``display_name``: Name for the website to use in emails.
   * ``host``: Hostname of the website.
   * ``sender``: Email address that is sending the notifications.
   * ``confirm_url_format``: Template for the URL that is used for confirmation
@@ -114,52 +112,56 @@
 * and ``*.html``: for the HTML version of the email.
 
 
 
 REST service
 ^^^^^^^^^^^^
 
-The REST service runs as a Python WSGI app. Any WSGI app server could be used.
+The REST service runs as a Python `ASGI app
+<https://asgi.readthedocs.io/en/latest/>`_. See the FastAPI documentation for
+`deployment options <https://fastapi.tiangolo.com/deployment/>`_.
 
-Passenger
-~~~~~~~~~
-
-Sample ``passenger_wsgi.py`` file::
-
-    import logging
-    logging.basicConfig(filename="/path/to/log", level=logging.WARN)
-
-    from doveseed.app import create_app
-    application = create_app()
 
 
 CORS
 ~~~~
 
-To set appropriate CORS headers use the
-`flask-cors <https://flask-cors.readthedocs.io/en/latest/>`_ package.
-Activate it by adding the following lines to the file where you instantiate
-the app, for example your ``passenger_wsgi.py`` file::
-
-    from flask_cors import CORS
-    CORS(application, origins=["https://my-domain.tld"])
+To set appropriate CORS headers use the `FastAPI CORSMiddleware
+<https://fastapi.tiangolo.com/tutorial/cors/>`_. Activate it by adding the
+following lines to the file where you instantiate the app::
+
+    from doveseed.app import app
+    from fastapi.middleware.cors import CORSMiddleware
+
+    app.add_middleware(
+        CORSMiddleware,
+        allow_origins=["http://example.com"],
+        allow_methods=["GET", "POST"],
+        allow_headers=["Authorization"],
+    )
 
 
 ReCaptcha
 ~~~~~~~~~
 
-To activate `ReCaptcha (v2) <https://www.google.com/recaptcha/>`_ verification of
-requests, add the follwing lines to the file where you instantiate the app,
-for example your ``passenger_wsgi.py`` file::
+You activate `ReCaptcha (v2) <https://www.google.com/recaptcha/>`_ verification of
+requests with Doveseed.
 
+First, you need to install the required optional dependencies::
+
+    pip install 'doveseed[recaptcha]'
+
+Then, add the follwing lines to the file where you instantiate the app::
+
+    from doveseed.app import app
     from doveseed.recaptcha import ReCaptchaMiddleware
-    application.wsgi_app = ReCaptchaMiddleware(
-        application.wsgi_app, '^/(un)?subscribe/.*', 'recaptcha.json')
 
-Also, create the ``recaptcha.json`` with the required ReCaptcha configuration::
+    app.add_middleware = ReCaptchaMiddleware('^/(un)?subscribe/.*', 'recaptcha.json')
+
+Also, create the ``recaptcha.json`` with the required ReCaptcha configuration:
 
 * ``hostnames``: List of hostnames to accept ReCaptchas from.
 * ``secret``: The shared key between your site and reCAPTCHA.
 
 
 **Ensure that the configuration files have appropriate permissions, i.e. only
 readable by you and Doveseed.**
```

