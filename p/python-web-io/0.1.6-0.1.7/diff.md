# Comparing `tmp/python_web_io-0.1.6.tar.gz` & `tmp/python_web_io-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_web_io-0.1.6.tar", max compression
+gzip compressed data, was "python_web_io-0.1.7.tar", max compression
```

## Comparing `python_web_io-0.1.6.tar` & `python_web_io-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,10 @@
--rw-r--r--   0        0        0      576 2023-04-16 00:48:38.469977 python_web_io-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-16 00:44:09.593767 python_web_io-0.1.6/python_web_io/__init__.py
--rw-r--r--   0        0        0       50 2023-04-16 00:32:01.158397 python_web_io-0.1.6/python_web_io/__main__.py
--rw-r--r--   0        0        0      223 2023-04-16 00:31:46.924427 python_web_io-0.1.6/python_web_io/python_web_io_internals/__init__.py
--rw-r--r--   0        0        0      484 2023-04-16 00:34:25.921541 python_web_io-0.1.6/python_web_io/python_web_io_internals/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      896 2023-04-15 20:46:44.667432 python_web_io-0.1.6/python_web_io/python_web_io_internals/__pycache__/cache.cpython-310.pyc
--rw-r--r--   0        0        0     1491 2023-04-16 00:34:26.131568 python_web_io-0.1.6/python_web_io/python_web_io_internals/__pycache__/main.cpython-310.pyc
--rw-r--r--   0        0        0     2469 2023-04-15 22:03:04.097038 python_web_io-0.1.6/python_web_io/python_web_io_internals/__pycache__/override.cpython-310.pyc
--rw-r--r--   0        0        0     1975 2023-04-15 22:02:43.798452 python_web_io-0.1.6/python_web_io/python_web_io_internals/__pycache__/server.cpython-310.pyc
--rw-r--r--   0        0        0      689 2023-04-15 20:46:43.293432 python_web_io-0.1.6/python_web_io/python_web_io_internals/cache.py
--rw-r--r--   0        0        0     1434 2023-04-16 00:31:21.807165 python_web_io-0.1.6/python_web_io/python_web_io_internals/main.py
--rw-r--r--   0        0        0     2265 2023-04-15 22:02:49.593645 python_web_io-0.1.6/python_web_io/python_web_io_internals/override.py
--rw-r--r--   0        0        0     2757 2023-04-15 22:02:26.352098 python_web_io-0.1.6/python_web_io/python_web_io_internals/server.py
--rw-r--r--   0        0        0      491 2023-04-15 21:42:54.685650 python_web_io-0.1.6/python_web_io/python_web_io_internals/templates/500.html
--rw-r--r--   0        0        0      794 2023-04-15 21:36:26.425700 python_web_io-0.1.6/python_web_io/python_web_io_internals/templates/base.html
--rw-r--r--   0        0        0      592 2023-04-15 20:07:32.561559 python_web_io-0.1.6/python_web_io/python_web_io_internals/templates/index.html
--rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 python_web_io-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      576 2023-04-16 00:58:45.108370 python_web_io-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-04-16 00:58:22.446645 python_web_io-0.1.7/python_web_io/__main__.py
+-rw-r--r--   0        0        0      689 2023-04-15 20:46:43.293432 python_web_io-0.1.7/python_web_io/cache.py
+-rw-r--r--   0        0        0     1385 2023-04-16 00:58:18.317553 python_web_io-0.1.7/python_web_io/main.py
+-rw-r--r--   0        0        0     2265 2023-04-15 22:02:49.593645 python_web_io-0.1.7/python_web_io/override.py
+-rw-r--r--   0        0        0     2783 2023-04-16 00:58:26.859300 python_web_io-0.1.7/python_web_io/server.py
+-rw-r--r--   0        0        0      491 2023-04-15 21:42:54.685650 python_web_io-0.1.7/python_web_io/templates/500.html
+-rw-r--r--   0        0        0      794 2023-04-15 21:36:26.425700 python_web_io-0.1.7/python_web_io/templates/base.html
+-rw-r--r--   0        0        0      592 2023-04-15 20:07:32.561559 python_web_io-0.1.7/python_web_io/templates/index.html
+-rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 python_web_io-0.1.7/PKG-INFO
```

### Comparing `python_web_io-0.1.6/pyproject.toml` & `python_web_io-0.1.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-web-io"
-version = "0.1.6"
+version = "0.1.7"
 description = "Generate a webpage as a GUI for a Python script, and serve from anywhere."
 authors = ["Zachary Smith"]
 packages = [{include = "python_web_io"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 flask = "^2.2.3"
```

### Comparing `python_web_io-0.1.6/python_web_io/python_web_io_internals/cache.py` & `python_web_io-0.1.7/python_web_io/cache.py`

 * *Files identical despite different names*

### Comparing `python_web_io-0.1.6/python_web_io/python_web_io_internals/main.py` & `python_web_io-0.1.7/python_web_io/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-import python_web_io_internals
 import argparse
 
+from python_web_io.cache import Cache
+from python_web_io.server import app
+
 
 def main(filepath: str, title: str, icon: str, debug: bool):
     """
     Loads the contents of a script and executes it.
 
     Arguments:
         filepath (str): filepath to script / entrypoint.
     """
     with open(filepath, "r") as file:
         script = file.read()
 
     # save args to config / Cache
-    python_web_io_internals.Cache.set("script", script)
-    python_web_io_internals.Cache.set("title", title)
-    python_web_io_internals.Cache.set("icon", icon)
+    Cache.set("script", script)
+    Cache.set("title", title)
+    Cache.set("icon", icon)
 
     # start the Flask server
-    python_web_io_internals.app.run(debug=debug)
+    app.run(debug=debug)
 
 
 def start():
     parser = argparse.ArgumentParser(
         description="Generate a web UI to iteract with a Python script."
     )
     parser.add_argument("script", type=str, help="Script filepath (required).")
```

### Comparing `python_web_io-0.1.6/python_web_io/python_web_io_internals/override.py` & `python_web_io-0.1.7/python_web_io/override.py`

 * *Files identical despite different names*

### Comparing `python_web_io-0.1.6/python_web_io/python_web_io_internals/server.py` & `python_web_io-0.1.7/python_web_io/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import builtins
 
 from dotenv import load_dotenv
 from flask import Flask, session, request, render_template
-from .override import (
+from python_web_io.override import (
     input,
     print,
     Exec,
 )  # input, print are listed as unused, but exist to override builtin calls made from Exec() of the user script
-from .cache import Cache
+from python_web_io.cache import Cache
 
 app = Flask(__name__)
 
 load_dotenv()
 FLASK_SECRET_KEY = os.environ["FLASK_SECRET_KEY"]
 app.secret_key = bytes(FLASK_SECRET_KEY, "utf-8")
```

### Comparing `python_web_io-0.1.6/python_web_io/python_web_io_internals/templates/base.html` & `python_web_io-0.1.7/python_web_io/templates/base.html`

 * *Files identical despite different names*

### Comparing `python_web_io-0.1.6/python_web_io/python_web_io_internals/templates/index.html` & `python_web_io-0.1.7/python_web_io/templates/index.html`

 * *Files identical despite different names*

