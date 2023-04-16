# Comparing `tmp/python_web_io-0.1.3.tar.gz` & `tmp/python_web_io-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_web_io-0.1.3.tar", max compression
+gzip compressed data, was "python_web_io-0.1.4.tar", max compression
```

## Comparing `python_web_io-0.1.3.tar` & `python_web_io-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rwxr-xr-x   0        0        0     1090 2023-04-15 12:44:31.002724 python_web_io-0.1.3/LICENSE
--rwxr-xr-x   0        0        0      578 2023-04-16 00:29:25.482057 python_web_io-0.1.3/pyproject.toml
--rwxr-xr-x   0        0        0       26 2023-04-15 16:06:33.499148 python_web_io-0.1.3/python_web_io/.env.example
--rwxr-xr-x   0        0        0     1434 2023-04-16 00:22:13.372429 python_web_io-0.1.3/python_web_io/main.py
--rwxr-xr-x   0        0        0      175 2023-04-16 00:22:09.613091 python_web_io-0.1.3/python_web_io/python_web_io_internals/__init__.py
--rwxr-xr-x   0        0        0      689 2023-04-15 20:46:43.293432 python_web_io-0.1.3/python_web_io/python_web_io_internals/cache.py
--rwxr-xr-x   0        0        0     2265 2023-04-15 22:02:49.593645 python_web_io-0.1.3/python_web_io/python_web_io_internals/override.py
--rwxr-xr-x   0        0        0     2757 2023-04-15 22:02:26.352098 python_web_io-0.1.3/python_web_io/python_web_io_internals/server.py
--rwxr-xr-x   0        0        0      491 2023-04-15 21:42:54.685650 python_web_io-0.1.3/python_web_io/python_web_io_internals/templates/500.html
--rwxr-xr-x   0        0        0      794 2023-04-15 21:36:26.425700 python_web_io-0.1.3/python_web_io/python_web_io_internals/templates/base.html
--rwxr-xr-x   0        0        0      592 2023-04-15 20:07:32.561559 python_web_io-0.1.3/python_web_io/python_web_io_internals/templates/index.html
--rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 python_web_io-0.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1090 2023-04-15 12:44:31.002724 python_web_io-0.1.4/LICENSE
+-rwxr-xr-x   0        0        0      578 2023-04-16 00:32:18.197342 python_web_io-0.1.4/pyproject.toml
+-rwxr-xr-x   0        0        0       26 2023-04-15 16:06:33.499148 python_web_io-0.1.4/python_web_io/.env.example
+-rwxr-xr-x   0        0        0       50 2023-04-16 00:32:01.158397 python_web_io-0.1.4/python_web_io/__main__.py
+-rwxr-xr-x   0        0        0      223 2023-04-16 00:31:46.924427 python_web_io-0.1.4/python_web_io/python_web_io_internals/__init__.py
+-rwxr-xr-x   0        0        0      689 2023-04-15 20:46:43.293432 python_web_io-0.1.4/python_web_io/python_web_io_internals/cache.py
+-rwxr-xr-x   0        0        0     1434 2023-04-16 00:31:21.807165 python_web_io-0.1.4/python_web_io/python_web_io_internals/main.py
+-rwxr-xr-x   0        0        0     2265 2023-04-15 22:02:49.593645 python_web_io-0.1.4/python_web_io/python_web_io_internals/override.py
+-rwxr-xr-x   0        0        0     2757 2023-04-15 22:02:26.352098 python_web_io-0.1.4/python_web_io/python_web_io_internals/server.py
+-rwxr-xr-x   0        0        0      491 2023-04-15 21:42:54.685650 python_web_io-0.1.4/python_web_io/python_web_io_internals/templates/500.html
+-rwxr-xr-x   0        0        0      794 2023-04-15 21:36:26.425700 python_web_io-0.1.4/python_web_io/python_web_io_internals/templates/base.html
+-rwxr-xr-x   0        0        0      592 2023-04-15 20:07:32.561559 python_web_io-0.1.4/python_web_io/python_web_io_internals/templates/index.html
+-rw-r--r--   0        0        0      471 1970-01-01 00:00:00.000000 python_web_io-0.1.4/PKG-INFO
```

### Comparing `python_web_io-0.1.3/LICENSE` & `python_web_io-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python_web_io-0.1.3/pyproject.toml` & `python_web_io-0.1.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-web-io"
-version = "0.1.3"
+version = "0.1.4"
 description = "Generate a webpage as a GUI for a Python script, and serve from anywhere."
 authors = ["Zachary Smith"]
 packages = [{include = "python_web_io"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 flask = "^2.2.3"
```

### Comparing `python_web_io-0.1.3/python_web_io/main.py` & `python_web_io-0.1.4/python_web_io/python_web_io_internals/main.py`

 * *Files identical despite different names*

### Comparing `python_web_io-0.1.3/python_web_io/python_web_io_internals/cache.py` & `python_web_io-0.1.4/python_web_io/python_web_io_internals/cache.py`

 * *Files identical despite different names*

### Comparing `python_web_io-0.1.3/python_web_io/python_web_io_internals/override.py` & `python_web_io-0.1.4/python_web_io/python_web_io_internals/override.py`

 * *Files identical despite different names*

### Comparing `python_web_io-0.1.3/python_web_io/python_web_io_internals/server.py` & `python_web_io-0.1.4/python_web_io/python_web_io_internals/server.py`

 * *Files identical despite different names*

### Comparing `python_web_io-0.1.3/python_web_io/python_web_io_internals/templates/base.html` & `python_web_io-0.1.4/python_web_io/python_web_io_internals/templates/base.html`

 * *Files identical despite different names*

### Comparing `python_web_io-0.1.3/python_web_io/python_web_io_internals/templates/index.html` & `python_web_io-0.1.4/python_web_io/python_web_io_internals/templates/index.html`

 * *Files identical despite different names*

