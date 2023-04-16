# Comparing `tmp/doveseed-2.0.0a5.tar.gz` & `tmp/doveseed-2.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doveseed-2.0.0a5.tar", max compression
+gzip compressed data, was "doveseed-2.0.0a6.tar", max compression
```

## Comparing `doveseed-2.0.0a5.tar` & `doveseed-2.0.0a6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1068 2023-04-16 16:22:34.660948 doveseed-2.0.0a5/LICENSE
--rw-r--r--   0        0        0     6454 2023-04-16 16:22:34.660948 doveseed-2.0.0a5/README.rst
--rw-r--r--   0        0        0       24 2023-04-16 16:22:34.660948 doveseed-2.0.0a5/doveseed/__init__.py
--rw-r--r--   0        0        0     5797 2023-04-16 16:22:34.660948 doveseed-2.0.0a5/doveseed/app.py
--rw-r--r--   0        0        0     2163 2023-04-16 16:22:34.660948 doveseed-2.0.0a5/doveseed/cli.py
--rw-r--r--   0        0        0      704 2023-04-16 16:22:34.660948 doveseed-2.0.0a5/doveseed/config.py
--rw-r--r--   0        0        0      932 2023-04-16 16:22:34.660948 doveseed-2.0.0a5/doveseed/confirmation.py
--rw-r--r--   0        0        0      765 2023-04-16 16:22:34.660948 doveseed-2.0.0a5/doveseed/domain_types.py
--rw-r--r--   0        0        0     1128 2023-04-16 16:22:34.660948 doveseed-2.0.0a5/doveseed/email_notification.py
--rw-r--r--   0        0        0     3060 2023-04-16 16:22:34.660948 doveseed-2.0.0a5/doveseed/email_templating.py
--rw-r--r--   0        0        0     1289 2023-04-16 16:22:34.660948 doveseed-2.0.0a5/doveseed/feed.py
--rw-r--r--   0        0        0     1287 2023-04-16 16:22:34.660948 doveseed-2.0.0a5/doveseed/notifier.py
--rw-r--r--   0        0        0     2112 2023-04-16 16:22:34.660948 doveseed-2.0.0a5/doveseed/recaptcha.py
--rw-r--r--   0        0        0     3843 2023-04-16 16:22:34.660948 doveseed-2.0.0a5/doveseed/registration.py
--rw-r--r--   0        0        0     2047 2023-04-16 16:22:34.660948 doveseed-2.0.0a5/doveseed/smtp.py
--rw-r--r--   0        0        0     3976 2023-04-16 16:22:34.660948 doveseed-2.0.0a5/doveseed/storage.py
--rw-r--r--   0        0        0      121 2023-04-16 16:22:34.660948 doveseed-2.0.0a5/doveseed/token_gen.py
--rw-r--r--   0        0        0     1248 2023-04-16 16:22:34.660948 doveseed-2.0.0a5/pyproject.toml
--rw-r--r--   0        0        0     7790 1970-01-01 00:00:00.000000 doveseed-2.0.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-16 16:37:15.829382 doveseed-2.0.0a6/LICENSE
+-rw-r--r--   0        0        0     6467 2023-04-16 16:37:15.829382 doveseed-2.0.0a6/README.rst
+-rw-r--r--   0        0        0       24 2023-04-16 16:37:15.829382 doveseed-2.0.0a6/doveseed/__init__.py
+-rw-r--r--   0        0        0     5797 2023-04-16 16:37:15.829382 doveseed-2.0.0a6/doveseed/app.py
+-rw-r--r--   0        0        0     2163 2023-04-16 16:37:15.829382 doveseed-2.0.0a6/doveseed/cli.py
+-rw-r--r--   0        0        0      703 2023-04-16 16:37:15.829382 doveseed-2.0.0a6/doveseed/config.py
+-rw-r--r--   0        0        0      932 2023-04-16 16:37:15.829382 doveseed-2.0.0a6/doveseed/confirmation.py
+-rw-r--r--   0        0        0      765 2023-04-16 16:37:15.829382 doveseed-2.0.0a6/doveseed/domain_types.py
+-rw-r--r--   0        0        0     1128 2023-04-16 16:37:15.829382 doveseed-2.0.0a6/doveseed/email_notification.py
+-rw-r--r--   0        0        0     3060 2023-04-16 16:37:15.829382 doveseed-2.0.0a6/doveseed/email_templating.py
+-rw-r--r--   0        0        0     1289 2023-04-16 16:37:15.829382 doveseed-2.0.0a6/doveseed/feed.py
+-rw-r--r--   0        0        0     1287 2023-04-16 16:37:15.829382 doveseed-2.0.0a6/doveseed/notifier.py
+-rw-r--r--   0        0        0     2112 2023-04-16 16:37:15.829382 doveseed-2.0.0a6/doveseed/recaptcha.py
+-rw-r--r--   0        0        0     3843 2023-04-16 16:37:15.829382 doveseed-2.0.0a6/doveseed/registration.py
+-rw-r--r--   0        0        0     2047 2023-04-16 16:37:15.829382 doveseed-2.0.0a6/doveseed/smtp.py
+-rw-r--r--   0        0        0     3976 2023-04-16 16:37:15.829382 doveseed-2.0.0a6/doveseed/storage.py
+-rw-r--r--   0        0        0      121 2023-04-16 16:37:15.829382 doveseed-2.0.0a6/doveseed/token_gen.py
+-rw-r--r--   0        0        0     1248 2023-04-16 16:37:15.829382 doveseed-2.0.0a6/pyproject.toml
+-rw-r--r--   0        0        0     7803 1970-01-01 00:00:00.000000 doveseed-2.0.0a6/PKG-INFO
```

### Comparing `doveseed-2.0.0a5/LICENSE` & `doveseed-2.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a5/README.rst` & `doveseed-2.0.0a6/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 ``config.sample.json``. The format is as follows:
 
 * ``db``: JSON file in which Doveseed persists its data.
 * ``rss``: URL to the RSS feed for which new notifications are to be send.
 * ``smtp``
 
   * ``host``: SMTP host used to send notification emails.
-  * ``port``: SMTP port used to send notification emails (defaul: ``25``).
+  * ``port``: SMTP port used to send notification emails (defaul: ``0`` = auto-select).
   * ``user``: SMTP logon user name.
   * ``password``: SMTP logon password.
   * ``ssl_mode``: Activate/deactivate SSL/TLS, valid values ``"no-ssl"``, ``"start-tls"``, ``"tls"`` (default ``"start-tls"``).
   * ``check_hostname``: Whether to verify the hostname when using TLS (default ``true``).
 
 * ``template_vars``: Defines template variables to replace in the email templates.
```

### Comparing `doveseed-2.0.0a5/doveseed/app.py` & `doveseed-2.0.0a6/doveseed/app.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a5/doveseed/cli.py` & `doveseed-2.0.0a6/doveseed/cli.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a5/doveseed/config.py` & `doveseed-2.0.0a6/doveseed/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 @dataclass(frozen=True)
 class SmtpConfig:
     host: str
     user: str
     password: str
-    port: int = 25
+    port: int = 0
     ssl_mode: Union[
         Literal["no-ssl"], Literal["start-tls"], Literal["tls"]
     ] = "start-tls"
     check_hostname: bool = True
 
 
 @dataclass(frozen=True)
```

### Comparing `doveseed-2.0.0a5/doveseed/confirmation.py` & `doveseed-2.0.0a6/doveseed/confirmation.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a5/doveseed/domain_types.py` & `doveseed-2.0.0a6/doveseed/domain_types.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a5/doveseed/email_notification.py` & `doveseed-2.0.0a6/doveseed/email_notification.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a5/doveseed/email_templating.py` & `doveseed-2.0.0a6/doveseed/email_templating.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a5/doveseed/feed.py` & `doveseed-2.0.0a6/doveseed/feed.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a5/doveseed/notifier.py` & `doveseed-2.0.0a6/doveseed/notifier.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a5/doveseed/recaptcha.py` & `doveseed-2.0.0a6/doveseed/recaptcha.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a5/doveseed/registration.py` & `doveseed-2.0.0a6/doveseed/registration.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a5/doveseed/smtp.py` & `doveseed-2.0.0a6/doveseed/smtp.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a5/doveseed/storage.py` & `doveseed-2.0.0a6/doveseed/storage.py`

 * *Files identical despite different names*

### Comparing `doveseed-2.0.0a5/pyproject.toml` & `doveseed-2.0.0a6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 ]
 description = "Doveseed is a backend service for email subscriptions to RSS feeds."
 keywords = ["email", "rss", "subscriptions"]
 license = "MIT"
 name = "doveseed"
 readme = "README.rst"
 repository = "https://github.com/jgosmann/doveseed/"
-version = "2.0.0a5" # Also update in doveseed/__init__.py
+version = "2.0.0a6" # Also update in doveseed/__init__.py
 
 [tool.poetry.dependencies]
 aiohttp = {version = "^3.8.4", optional = true}
 fastapi = "^0.95.0"
 jinja2 = "^3.1.2"
 python = "^3.9.0"
 starlette = {version = "0.26.1", optional = true}
```

### Comparing `doveseed-2.0.0a5/PKG-INFO` & `doveseed-2.0.0a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doveseed
-Version: 2.0.0a5
+Version: 2.0.0a6
 Summary: Doveseed is a backend service for email subscriptions to RSS feeds.
 Home-page: https://github.com/jgosmann/doveseed/
 License: MIT
 Keywords: email,rss,subscriptions
 Author: Jan Gosmann
 Author-email: jan@hyper-world.de
 Requires-Python: >=3.9.0,<4.0.0
@@ -63,15 +63,15 @@
 ``config.sample.json``. The format is as follows:
 
 * ``db``: JSON file in which Doveseed persists its data.
 * ``rss``: URL to the RSS feed for which new notifications are to be send.
 * ``smtp``
 
   * ``host``: SMTP host used to send notification emails.
-  * ``port``: SMTP port used to send notification emails (defaul: ``25``).
+  * ``port``: SMTP port used to send notification emails (defaul: ``0`` = auto-select).
   * ``user``: SMTP logon user name.
   * ``password``: SMTP logon password.
   * ``ssl_mode``: Activate/deactivate SSL/TLS, valid values ``"no-ssl"``, ``"start-tls"``, ``"tls"`` (default ``"start-tls"``).
   * ``check_hostname``: Whether to verify the hostname when using TLS (default ``true``).
 
 * ``template_vars``: Defines template variables to replace in the email templates.
```

