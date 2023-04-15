# Comparing `tmp/python_web_io-0.1.1.tar.gz` & `tmp/python_web_io-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_web_io-0.1.1.tar", max compression
+gzip compressed data, was "python_web_io-0.1.2.tar", max compression
```

## Comparing `python_web_io-0.1.1.tar` & `python_web_io-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,11 @@
--rw-r--r--   0        0        0     1090 2023-04-15 12:44:31.002724 python_web_io-0.1.1/LICENSE
--rw-r--r--   0        0        0      578 2023-04-15 22:30:36.289547 python_web_io-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       25 2023-04-15 16:49:34.717762 python_web_io-0.1.1/python_web_io/.env
--rw-r--r--   0        0        0       26 2023-04-15 16:06:33.499148 python_web_io-0.1.1/python_web_io/.env.example
--rw-r--r--   0        0        0        0 2023-04-15 22:29:54.823024 python_web_io-0.1.1/python_web_io/__init__.py
--rw-r--r--   0        0        0       34 2023-04-15 22:30:14.398841 python_web_io-0.1.1/python_web_io/__main__.py
--rw-r--r--   0        0        0     1384 2023-04-15 22:30:16.527104 python_web_io-0.1.1/python_web_io/main.py
--rw-r--r--   0        0        0      108 2023-04-15 20:36:33.636176 python_web_io-0.1.1/python_web_io/python_web_io/__init__.py
--rw-r--r--   0        0        0      340 2023-04-15 20:46:31.293106 python_web_io-0.1.1/python_web_io/python_web_io/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      896 2023-04-15 20:46:44.667432 python_web_io-0.1.1/python_web_io/python_web_io/__pycache__/cache.cpython-310.pyc
--rw-r--r--   0        0        0     2469 2023-04-15 22:03:04.097038 python_web_io-0.1.1/python_web_io/python_web_io/__pycache__/override.cpython-310.pyc
--rw-r--r--   0        0        0     1975 2023-04-15 22:02:43.798452 python_web_io-0.1.1/python_web_io/python_web_io/__pycache__/server.cpython-310.pyc
--rw-r--r--   0        0        0      689 2023-04-15 20:46:43.293432 python_web_io-0.1.1/python_web_io/python_web_io/cache.py
--rw-r--r--   0        0        0     2265 2023-04-15 22:02:49.593645 python_web_io-0.1.1/python_web_io/python_web_io/override.py
--rw-r--r--   0        0        0     2757 2023-04-15 22:02:26.352098 python_web_io-0.1.1/python_web_io/python_web_io/server.py
--rw-r--r--   0        0        0      491 2023-04-15 21:42:54.685650 python_web_io-0.1.1/python_web_io/python_web_io/templates/500.html
--rw-r--r--   0        0        0      794 2023-04-15 21:36:26.425700 python_web_io-0.1.1/python_web_io/python_web_io/templates/base.html
--rw-r--r--   0        0        0      592 2023-04-15 20:07:32.561559 python_web_io-0.1.1/python_web_io/python_web_io/templates/index.html
--rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 python_web_io-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-04-15 12:44:31.002724 python_web_io-0.1.2/LICENSE
+-rw-r--r--   0        0        0      582 2023-04-15 22:51:39.217346 python_web_io-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      131 2023-04-15 22:36:41.655929 python_web_io-0.1.2/src/python_web_io/__init__.py
+-rw-r--r--   0        0        0      689 2023-04-15 20:46:43.293432 python_web_io-0.1.2/src/python_web_io/cache.py
+-rw-r--r--   0        0        0     1357 2023-04-15 22:35:01.193566 python_web_io-0.1.2/src/python_web_io/main.py
+-rw-r--r--   0        0        0     2265 2023-04-15 22:02:49.593645 python_web_io-0.1.2/src/python_web_io/override.py
+-rw-r--r--   0        0        0     2757 2023-04-15 22:02:26.352098 python_web_io-0.1.2/src/python_web_io/server.py
+-rw-r--r--   0        0        0      491 2023-04-15 21:42:54.685650 python_web_io-0.1.2/src/python_web_io/templates/500.html
+-rw-r--r--   0        0        0      794 2023-04-15 21:36:26.425700 python_web_io-0.1.2/src/python_web_io/templates/base.html
+-rw-r--r--   0        0        0      592 2023-04-15 20:07:32.561559 python_web_io-0.1.2/src/python_web_io/templates/index.html
+-rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 python_web_io-0.1.2/PKG-INFO
```

### Comparing `python_web_io-0.1.1/LICENSE` & `python_web_io-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_web_io-0.1.1/pyproject.toml` & `python_web_io-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "python-web-io"
-version = "0.1.1"
+version = "0.1.2"
 description = "Generate a webpage as a GUI for a Python script, and serve from anywhere."
 authors = ["Zachary Smith"]
-packages = [{include = "python_web_io"}]
+packages = [{include = "src/python_web_io"}]
 
 [tool.poetry.scripts]
 python_web_io = "python_web_io.main:start"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 flask = "^2.2.3"
```

### Comparing `python_web_io-0.1.1/python_web_io/main.py` & `python_web_io-0.1.2/src/python_web_io/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-import python_web_io
+from .cache import Cache
+from .server import app
 import argparse
 
 
 def main(filepath: str, title: str, icon: str, debug: bool):
     """
     Loads the contents of a script and executes it.
 
     Arguments:
         filepath (str): filepath to script / entrypoint.
     """
     with open(filepath, "r") as file:
         script = file.read()
 
     # save args to config / Cache
-    python_web_io.Cache.set("script", script)
-    python_web_io.Cache.set("title", title)
-    python_web_io.Cache.set("icon", icon)
+    Cache.set("script", script)
+    Cache.set("title", title)
+    Cache.set("icon", icon)
 
     # start the Flask server
-    python_web_io.app.run(debug=debug)
+    app.run(debug=debug)
 
 
 def start():
     parser = argparse.ArgumentParser(
         description="Generate a web UI to iteract with a Python script."
     )
     parser.add_argument("script", type=str, help="Script filepath (required).")
```

### Comparing `python_web_io-0.1.1/python_web_io/python_web_io/cache.py` & `python_web_io-0.1.2/src/python_web_io/cache.py`

 * *Files identical despite different names*

### Comparing `python_web_io-0.1.1/python_web_io/python_web_io/override.py` & `python_web_io-0.1.2/src/python_web_io/override.py`

 * *Files identical despite different names*

### Comparing `python_web_io-0.1.1/python_web_io/python_web_io/server.py` & `python_web_io-0.1.2/src/python_web_io/server.py`

 * *Files identical despite different names*

### Comparing `python_web_io-0.1.1/python_web_io/python_web_io/templates/base.html` & `python_web_io-0.1.2/src/python_web_io/templates/base.html`

 * *Files identical despite different names*

### Comparing `python_web_io-0.1.1/python_web_io/python_web_io/templates/index.html` & `python_web_io-0.1.2/src/python_web_io/templates/index.html`

 * *Files identical despite different names*

