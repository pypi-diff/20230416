# Comparing `tmp/python_web_io-0.1.7.tar.gz` & `tmp/python_web_io-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_web_io-0.1.7.tar", max compression
+gzip compressed data, was "python_web_io-0.1.8.tar", max compression
```

## Comparing `python_web_io-0.1.7.tar` & `python_web_io-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      576 2023-04-16 00:58:45.108370 python_web_io-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       45 2023-04-16 00:58:22.446645 python_web_io-0.1.7/python_web_io/__main__.py
--rw-r--r--   0        0        0      689 2023-04-15 20:46:43.293432 python_web_io-0.1.7/python_web_io/cache.py
--rw-r--r--   0        0        0     1385 2023-04-16 00:58:18.317553 python_web_io-0.1.7/python_web_io/main.py
--rw-r--r--   0        0        0     2265 2023-04-15 22:02:49.593645 python_web_io-0.1.7/python_web_io/override.py
--rw-r--r--   0        0        0     2783 2023-04-16 00:58:26.859300 python_web_io-0.1.7/python_web_io/server.py
--rw-r--r--   0        0        0      491 2023-04-15 21:42:54.685650 python_web_io-0.1.7/python_web_io/templates/500.html
--rw-r--r--   0        0        0      794 2023-04-15 21:36:26.425700 python_web_io-0.1.7/python_web_io/templates/base.html
--rw-r--r--   0        0        0      592 2023-04-15 20:07:32.561559 python_web_io-0.1.7/python_web_io/templates/index.html
--rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 python_web_io-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      550 2023-04-16 01:04:25.875413 python_web_io-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-04-16 00:58:22.446645 python_web_io-0.1.8/python_web_io/__main__.py
+-rw-r--r--   0        0        0      689 2023-04-15 20:46:43.293432 python_web_io-0.1.8/python_web_io/cache.py
+-rw-r--r--   0        0        0     1385 2023-04-16 00:58:18.317553 python_web_io-0.1.8/python_web_io/main.py
+-rw-r--r--   0        0        0     2265 2023-04-15 22:02:49.593645 python_web_io-0.1.8/python_web_io/override.py
+-rw-r--r--   0        0        0     2736 2023-04-16 01:03:41.446254 python_web_io-0.1.8/python_web_io/server.py
+-rw-r--r--   0        0        0      491 2023-04-15 21:42:54.685650 python_web_io-0.1.8/python_web_io/templates/500.html
+-rw-r--r--   0        0        0      794 2023-04-15 21:36:26.425700 python_web_io-0.1.8/python_web_io/templates/base.html
+-rw-r--r--   0        0        0      592 2023-04-15 20:07:32.561559 python_web_io-0.1.8/python_web_io/templates/index.html
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 python_web_io-0.1.8/PKG-INFO
```

### Comparing `python_web_io-0.1.7/pyproject.toml` & `python_web_io-0.1.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [tool.poetry]
 name = "python-web-io"
-version = "0.1.7"
+version = "0.1.8"
 description = "Generate a webpage as a GUI for a Python script, and serve from anywhere."
 authors = ["Zachary Smith"]
 packages = [{include = "python_web_io"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 flask = "^2.2.3"
-python-dotenv = "^1.0.0"
 flask-session = "^0.4.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pre-commit = "^3.2.2"
 
 [build-system]
```

### Comparing `python_web_io-0.1.7/python_web_io/cache.py` & `python_web_io-0.1.8/python_web_io/cache.py`

 * *Files identical despite different names*

### Comparing `python_web_io-0.1.7/python_web_io/main.py` & `python_web_io-0.1.8/python_web_io/main.py`

 * *Files identical despite different names*

### Comparing `python_web_io-0.1.7/python_web_io/override.py` & `python_web_io-0.1.8/python_web_io/override.py`

 * *Files identical despite different names*

### Comparing `python_web_io-0.1.7/python_web_io/server.py` & `python_web_io-0.1.8/python_web_io/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import os
 import builtins
 
-from dotenv import load_dotenv
 from flask import Flask, session, request, render_template
 from python_web_io.override import (
     input,
     print,
     Exec,
 )  # input, print are listed as unused, but exist to override builtin calls made from Exec() of the user script
 from python_web_io.cache import Cache
 
 app = Flask(__name__)
 
-load_dotenv()
 FLASK_SECRET_KEY = os.environ["FLASK_SECRET_KEY"]
 app.secret_key = bytes(FLASK_SECRET_KEY, "utf-8")
 
 
 @app.errorhandler(500)
 def internal_error(error):
     """
```

### Comparing `python_web_io-0.1.7/python_web_io/templates/base.html` & `python_web_io-0.1.8/python_web_io/templates/base.html`

 * *Files identical despite different names*

### Comparing `python_web_io-0.1.7/python_web_io/templates/index.html` & `python_web_io-0.1.8/python_web_io/templates/index.html`

 * *Files identical despite different names*

