# Comparing `tmp/py3status-reddit-1.0.0.tar.gz` & `tmp/py3status_reddit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3status-reddit-1.0.0.tar", last modified: Mon May 17 13:47:59 2021, max compression
+gzip compressed data, was "py3status_reddit-1.0.1.tar", max compression
```

## Comparing `py3status-reddit-1.0.0.tar` & `py3status_reddit-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      609 2021-05-17 13:34:08.310317 py3status-reddit-1.0.0/README.md
--rw-r--r--   0        0        0      628 2021-05-17 13:34:08.310317 py3status-reddit-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       68 2021-05-17 13:34:08.310317 py3status-reddit-1.0.0/src/py3status_reddit/__init__.py
--rw-r--r--   0        0        0     3890 2021-05-17 13:34:08.310317 py3status-reddit-1.0.0/src/py3status_reddit/reddit.py
--rw-r--r--   0        0        0     1086 2021-05-17 13:34:08.310317 py3status-reddit-1.0.0/src/py3status_reddit/webserver.py
--rw-r--r--   0        0        0     1493 2021-05-17 13:47:59.747195 py3status-reddit-1.0.0/setup.py
--rw-r--r--   0        0        0     1145 2021-05-17 13:47:59.747455 py3status-reddit-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      609 2023-01-17 11:17:54.263097 py3status_reddit-1.0.1/README.md
+-rw-r--r--   0        0        0      628 2023-04-16 16:48:03.388774 py3status_reddit-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-01-17 11:17:54.263097 py3status_reddit-1.0.1/src/py3status_reddit/__init__.py
+-rw-r--r--   0        0        0       18 2023-04-16 16:55:00.489000 py3status_reddit-1.0.1/src/py3status_reddit/__version__.py
+-rw-r--r--   0        0        0     3889 2023-04-16 16:47:36.420151 py3status_reddit-1.0.1/src/py3status_reddit/reddit.py
+-rw-r--r--   0        0        0     1086 2023-01-17 11:17:54.263097 py3status_reddit-1.0.1/src/py3status_reddit/webserver.py
+-rw-r--r--   0        0        0     1247 1970-01-01 00:00:00.000000 py3status_reddit-1.0.1/PKG-INFO
```

### Comparing `py3status-reddit-1.0.0/README.md` & `py3status_reddit-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `py3status-reddit-1.0.0/pyproject.toml` & `py3status_reddit-1.0.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py3status-reddit"
-version = "1.0.0"
+version = "1.0.1"
 description = "py3status module showing reddit unread messages"
 authors = ["Alessandro -oggei- Ogier <alessandro.ogier@gmail.com>"]
 readme = "README.md"
 include = ["fancy_count.png"]
 
 [tool.poetry.dependencies]
 python = "^3.6.2"
```

### Comparing `py3status-reddit-1.0.0/src/py3status_reddit/reddit.py` & `py3status_reddit-1.0.1/src/py3status_reddit/reddit.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
             if query["state"] == [str(state)]:
                 refresh_token = self._reddit.auth.authorize(query["code"][0])
                 self._token.write(refresh_token)
 
         elif self._count > 0:
             self.py3.command_run(  # pylint: disable=no-member
-                "xdg-open https://www.reddit.com/message/unread"
+                "xdg-open https://www.reddit.com/message/inbox"
             )
 
 
 # Run module in test mode.
 if __name__ == "__main__":
     from py3status.module_test import module_test
```

### Comparing `py3status-reddit-1.0.0/src/py3status_reddit/webserver.py` & `py3status_reddit-1.0.1/src/py3status_reddit/webserver.py`

 * *Files identical despite different names*

### Comparing `py3status-reddit-1.0.0/PKG-INFO` & `py3status_reddit-1.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: py3status-reddit
-Version: 1.0.0
+Version: 1.0.1
 Summary: py3status module showing reddit unread messages
 Author: Alessandro -oggei- Ogier
 Author-email: alessandro.ogier@gmail.com
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: praw (>=7.2.0,<8.0.0)
 Requires-Dist: xdg (>=5.0.2,<6.0.0)
 Description-Content-Type: text/markdown
 
 # py3status-reddit
 
 A py3status module showing reddit unread messages.
```

