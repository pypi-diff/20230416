# Comparing `tmp/lcu-connector-1.0.1.tar.gz` & `tmp/lcu-connector-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcu-connector-1.0.1.tar", last modified: Sat Apr 15 05:24:21 2023, max compression
+gzip compressed data, was "lcu-connector-1.0.2.tar", last modified: Sun Apr 16 09:05:37 2023, max compression
```

## Comparing `lcu-connector-1.0.1.tar` & `lcu-connector-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 05:24:21.563248 lcu-connector-1.0.1/
--rw-rw-rw-   0        0        0     1091 2023-04-15 04:30:40.000000 lcu-connector-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2821 2023-04-15 05:24:21.562269 lcu-connector-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1976 2023-04-15 04:30:40.000000 lcu-connector-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 05:24:21.559307 lcu-connector-1.0.1/lcu_connector/
--rw-rw-rw-   0        0        0       34 2023-04-15 04:30:40.000000 lcu-connector-1.0.1/lcu_connector/__init__.py
--rw-rw-rw-   0        0        0     4121 2023-04-15 04:30:40.000000 lcu-connector-1.0.1/lcu_connector/connection.py
--rw-rw-rw-   0        0        0     3938 2023-04-15 05:06:52.000000 lcu-connector-1.0.1/lcu_connector/connector.py
--rw-rw-rw-   0        0        0      830 2023-04-15 04:30:40.000000 lcu-connector-1.0.1/lcu_connector/exceptions.py
--rw-rw-rw-   0        0        0     4544 2023-04-15 05:19:53.000000 lcu-connector-1.0.1/lcu_connector/riot.py
-drwxrwxrwx   0        0        0        0 2023-04-15 05:24:21.562269 lcu-connector-1.0.1/lcu_connector.egg-info/
--rw-rw-rw-   0        0        0     2821 2023-04-15 05:24:21.000000 lcu-connector-1.0.1/lcu_connector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-04-15 05:24:21.000000 lcu-connector-1.0.1/lcu_connector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       45 2023-04-15 05:24:21.000000 lcu-connector-1.0.1/lcu_connector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-15 05:24:21.000000 lcu-connector-1.0.1/lcu_connector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-15 05:24:21.000000 lcu-connector-1.0.1/lcu_connector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1145 2023-04-15 04:30:40.000000 lcu-connector-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-15 05:24:21.563248 lcu-connector-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1341 2023-04-15 05:20:56.000000 lcu-connector-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 09:05:37.433278 lcu-connector-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-04-15 14:11:25.000000 lcu-connector-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2821 2023-04-16 09:05:37.432270 lcu-connector-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1976 2023-04-15 14:11:25.000000 lcu-connector-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 09:05:37.427383 lcu-connector-1.0.2/lcu_connector/
+-rw-rw-rw-   0        0        0       34 2023-04-15 14:11:25.000000 lcu-connector-1.0.2/lcu_connector/__init__.py
+-rw-rw-rw-   0        0        0     4121 2023-04-15 14:11:25.000000 lcu-connector-1.0.2/lcu_connector/connection.py
+-rw-rw-rw-   0        0        0     3940 2023-04-16 02:51:26.000000 lcu-connector-1.0.2/lcu_connector/connector.py
+-rw-rw-rw-   0        0        0      830 2023-04-15 14:11:25.000000 lcu-connector-1.0.2/lcu_connector/exceptions.py
+-rw-rw-rw-   0        0        0     4545 2023-04-16 02:49:35.000000 lcu-connector-1.0.2/lcu_connector/riot.py
+drwxrwxrwx   0        0        0        0 2023-04-16 09:05:37.431292 lcu-connector-1.0.2/lcu_connector.egg-info/
+-rw-rw-rw-   0        0        0     2821 2023-04-16 09:05:37.000000 lcu-connector-1.0.2/lcu_connector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-04-16 09:05:37.000000 lcu-connector-1.0.2/lcu_connector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       45 2023-04-16 09:05:37.000000 lcu-connector-1.0.2/lcu_connector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-16 09:05:37.000000 lcu-connector-1.0.2/lcu_connector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-16 09:05:37.000000 lcu-connector-1.0.2/lcu_connector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      955 2023-04-16 09:05:09.000000 lcu-connector-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-16 09:05:37.433278 lcu-connector-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1343 2023-04-16 09:02:23.000000 lcu-connector-1.0.2/setup.py
```

### Comparing `lcu-connector-1.0.1/LICENSE` & `lcu-connector-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lcu-connector-1.0.1/PKG-INFO` & `lcu-connector-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcu-connector
-Version: 1.0.1
+Version: 1.0.2
 Summary: Easy-to-use wrapper for the League Client API.
 Author: Gabriel Viana
 Author-email: ssiriusbeck@gmail.com
 Project-URL: Source, https://github.com/pySiriusDev/lcu-connector
 Project-URL: Download, https://github.com/pySiriusDev/lcu-connector/releases
 Project-URL: Instagram, https://instagram.com/biellviana
 Project-URL: Twitter, https://twitter.com/_siriusbeck
```

### Comparing `lcu-connector-1.0.1/README.md` & `lcu-connector-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lcu-connector-1.0.1/lcu_connector/connection.py` & `lcu-connector-1.0.2/lcu_connector/connection.py`

 * *Files identical despite different names*

### Comparing `lcu-connector-1.0.1/lcu_connector/connector.py` & `lcu-connector-1.0.2/lcu_connector/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from base64 import b64encode
 from typing import Dict, Optional
 
 from .connection import Connection
-from .riot import LeaguClient
+from .riot import LeagueClient
 
 
 class BaseConnector():
     """Base class that stores the attributes for the `Connector`.
 
     Attributes:
         __pid (str): The private ID of the connector.
@@ -121,15 +121,15 @@
         self.__setup_attr()
         if start:
             self.start()
 
     def __setup_attr(self) -> None:
         """Set up attributes for the `Connector` instance.
         """
-        client = LeaguClient()
+        client = LeagueClient()
         lockfile = client.lockfile
 
         self.pid = lockfile.pid
         self.url = f'{lockfile.protocol}://127.0.0.1:{lockfile.port}'
         self.auth = b64encode(f'riot:{lockfile.password}'.encode('ascii')).decode('ascii')
         self.headers = {
             "host": f'127.0.0.1:{lockfile.port}',
```

### Comparing `lcu-connector-1.0.1/lcu_connector/exceptions.py` & `lcu-connector-1.0.2/lcu_connector/exceptions.py`

 * *Files identical despite different names*

### Comparing `lcu-connector-1.0.1/lcu_connector/riot.py` & `lcu-connector-1.0.2/lcu_connector/riot.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,27 +40,27 @@
             self.name = data[0]
             self.pid = data[1]
             self.port = data[2]
             self.password = data[3]
             self.protocol = data[4]
 
 
-class LeaguClient:
+class LeagueClient:
     """Class representing a League of Legends client.
 
     Attributes:
         __process_name (str): The name of the League client executable file.
         __process (psutil.Process): The process object representing the League client.
         __lockfile (Lockfile): The lockfile object representing the League client's lockfile.
     """
 
     def __init__(self) -> None:
         """Initializes a new client object and validates the League client process and lockfile.
         """
-        self.__process_name = 'LeagueClient.exe' + ('.app' if not WINDOWS else '')
+        self.__process_name = 'LeagueClient' + ('.app' if not WINDOWS else '.exe')
         self.__process = self.__get_process()
         self.__lockfile = self.__get_lockfile()
 
     def __get_process(self) -> Process:
         """Return the League Client process.
 
         Returns:
```

### Comparing `lcu-connector-1.0.1/lcu_connector.egg-info/PKG-INFO` & `lcu-connector-1.0.2/lcu_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcu-connector
-Version: 1.0.1
+Version: 1.0.2
 Summary: Easy-to-use wrapper for the League Client API.
 Author: Gabriel Viana
 Author-email: ssiriusbeck@gmail.com
 Project-URL: Source, https://github.com/pySiriusDev/lcu-connector
 Project-URL: Download, https://github.com/pySiriusDev/lcu-connector/releases
 Project-URL: Instagram, https://instagram.com/biellviana
 Project-URL: Twitter, https://twitter.com/_siriusbeck
```

### Comparing `lcu-connector-1.0.1/pyproject.toml` & `lcu-connector-1.0.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -14,26 +14,20 @@
 requests = "^2.28.2"
 psutil = "^5.9.4"
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.2"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
-sphinx = "^6.1.3"
-pydata-sphinx-theme = "^0.13.3"
-sphinx-autodoc-typehints = "^1.22"
-sphinx-design = "^0.4.1"
-sphinx-togglebutton = "^0.3.2"
-sphinx-copybutton = "^0.5.1"
-sphinx-sitemap = "^2.5.0"
-sphinx-autoapi = "^2.1.0"
-myst-parser = "^1.0.0"
-sphinx-autobuild = "^2021.3.14"
 twine = "^4.0.2"
+markdown-refdocs = "^1.4.1"
+wheel = "^0.40.0"
+setuptools = "^67.6.1"
 
 [tool.poetry.scripts]
 tests = "scripts:run_tests"
 docs = "scripts:build_docs"
+build = "scripts:build"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lcu-connector-1.0.1/setup.py` & `lcu-connector-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     readme = fh.read()
 
 setup(
     name="lcu-connector",
-    version="1.0.1",
+    version="1.0.2",
     author="Gabriel Viana",
     author_email='ssiriusbeck@gmail.com',
     description="Easy-to-use wrapper for the League Client API.",
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=["lcu_connector"],
     classifiers=[
@@ -38,8 +38,8 @@
         'league of legends',
         'league of legends api',
         'lcu-driver',
         'lcu driver',
         'lcu-connector',
         'lcu connector'
     ]
-)
+)
```

