# Comparing `tmp/pylaunches-1.3.0.tar.gz` & `tmp/pylaunches-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylaunches-1.3.0.tar", last modified: Tue Jan 25 19:17:37 2022, max compression
+gzip compressed data, was "pylaunches-1.4.0.tar", last modified: Sun Apr 16 20:02:32 2023, max compression
```

## Comparing `pylaunches-1.3.0.tar` & `pylaunches-1.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 19:17:37.968495 pylaunches-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-01-25 19:17:28.000000 pylaunches-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-01-25 19:17:37.968495 pylaunches-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-01-25 19:17:28.000000 pylaunches-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 19:17:37.964495 pylaunches-1.3.0/pylaunches/
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-01-25 19:17:28.000000 pylaunches-1.3.0/pylaunches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2045 2022-01-25 19:17:28.000000 pylaunches-1.3.0/pylaunches/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      999 2022-01-25 19:17:28.000000 pylaunches-1.3.0/pylaunches/common.py
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-01-25 19:17:28.000000 pylaunches-1.3.0/pylaunches/const.py
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-01-25 19:17:28.000000 pylaunches-1.3.0/pylaunches/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 19:17:37.968495 pylaunches-1.3.0/pylaunches/objects/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-25 19:17:28.000000 pylaunches-1.3.0/pylaunches/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-01-25 19:17:28.000000 pylaunches-1.3.0/pylaunches/objects/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     1450 2022-01-25 19:17:28.000000 pylaunches-1.3.0/pylaunches/objects/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     7274 2022-01-25 19:17:28.000000 pylaunches-1.3.0/pylaunches/objects/launch.py
--rw-r--r--   0 runner    (1001) docker     (121)     3507 2022-01-25 19:17:28.000000 pylaunches-1.3.0/pylaunches/objects/starship.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-25 19:17:37.964495 pylaunches-1.3.0/pylaunches.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-01-25 19:17:37.000000 pylaunches-1.3.0/pylaunches.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-01-25 19:17:37.000000 pylaunches-1.3.0/pylaunches.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-25 19:17:37.000000 pylaunches-1.3.0/pylaunches.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-25 19:17:37.000000 pylaunches-1.3.0/pylaunches.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-01-25 19:17:37.000000 pylaunches-1.3.0/pylaunches.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-01-25 19:17:37.968495 pylaunches-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-01-25 19:17:36.000000 pylaunches-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:02:32.661250 pylaunches-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-16 20:02:25.000000 pylaunches-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-16 20:02:32.661250 pylaunches-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-16 20:02:25.000000 pylaunches-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:02:32.661250 pylaunches-1.4.0/pylaunches/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-16 20:02:25.000000 pylaunches-1.4.0/pylaunches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-04-16 20:02:25.000000 pylaunches-1.4.0/pylaunches/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-16 20:02:25.000000 pylaunches-1.4.0/pylaunches/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-16 20:02:25.000000 pylaunches-1.4.0/pylaunches/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-16 20:02:25.000000 pylaunches-1.4.0/pylaunches/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:02:32.661250 pylaunches-1.4.0/pylaunches/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 20:02:25.000000 pylaunches-1.4.0/pylaunches/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-16 20:02:25.000000 pylaunches-1.4.0/pylaunches/objects/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-04-16 20:02:25.000000 pylaunches-1.4.0/pylaunches/objects/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-04-16 20:02:25.000000 pylaunches-1.4.0/pylaunches/objects/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-16 20:02:25.000000 pylaunches-1.4.0/pylaunches/objects/starship.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 20:02:32.661250 pylaunches-1.4.0/pylaunches.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-16 20:02:32.000000 pylaunches-1.4.0/pylaunches.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-16 20:02:32.000000 pylaunches-1.4.0/pylaunches.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 20:02:32.000000 pylaunches-1.4.0/pylaunches.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-16 20:02:32.000000 pylaunches-1.4.0/pylaunches.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-16 20:02:32.000000 pylaunches-1.4.0/pylaunches.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-16 20:02:32.661250 pylaunches-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-16 20:02:32.000000 pylaunches-1.4.0/setup.py
```

### Comparing `pylaunches-1.3.0/LICENSE` & `pylaunches-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylaunches-1.3.0/PKG-INFO` & `pylaunches-1.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: pylaunches
-Version: 1.3.0
-Summary: UNKNOWN
+Version: 1.4.0
 Home-page: https://github.com/ludeeus/pylaunches
 Author: Joakim Sorensen
 Author-email: hi@ludeeus.dev
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyLaunches
@@ -46,8 +43,7 @@
 asyncio.get_event_loop().run_until_complete(example())
 
 ```
 
 This package is using the [Launch Library 2 API][launchlibrary] to get the information.
 
 [launchlibrary]: https://thespacedevs.com/llapi
-
```

### Comparing `pylaunches-1.3.0/README.md` & `pylaunches-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pylaunches-1.3.0/pylaunches/common.py` & `pylaunches-1.4.0/pylaunches/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 """Common attributes and functions."""
 from asyncio import CancelledError, TimeoutError
-from typing import Optional
+from typing import Mapping, Optional
 
 from aiohttp import ClientSession, ClientTimeout
 
 from pylaunches.const import HEADERS
 from pylaunches.exceptions import PyLaunchesException
 
 
 async def call_api(
     session: ClientSession,
     endpoint: str,
     token: Optional[str],
+    params: Optional[Mapping[str, str]],
 ) -> dict or None:
     """Call the API."""
     headers = HEADERS
     if token is not None:
         headers["Token"] = token
     try:
         response = await session.get(
-            endpoint,
-            headers=headers,
-            timeout=ClientTimeout(total=20),
+            endpoint, headers=headers, timeout=ClientTimeout(total=20), params=params
         )
         if response.status != 200:
             raise PyLaunchesException(f"Unexpected statuscode {response.status}")
         return await response.json()
     except (CancelledError, PyLaunchesException) as exception:
         raise PyLaunchesException(exception)
     except TimeoutError:
```

### Comparing `pylaunches-1.3.0/pylaunches/objects/event.py` & `pylaunches-1.4.0/pylaunches/objects/event.py`

 * *Files identical despite different names*

### Comparing `pylaunches-1.3.0/pylaunches/objects/launch.py` & `pylaunches-1.4.0/pylaunches/objects/launch.py`

 * *Files identical despite different names*

### Comparing `pylaunches-1.3.0/pylaunches/objects/starship.py` & `pylaunches-1.4.0/pylaunches/objects/starship.py`

 * *Files identical despite different names*

### Comparing `pylaunches-1.3.0/pylaunches.egg-info/PKG-INFO` & `pylaunches-1.4.0/pylaunches.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: pylaunches
-Version: 1.3.0
-Summary: UNKNOWN
+Version: 1.4.0
 Home-page: https://github.com/ludeeus/pylaunches
 Author: Joakim Sorensen
 Author-email: hi@ludeeus.dev
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PyLaunches
@@ -46,8 +43,7 @@
 asyncio.get_event_loop().run_until_complete(example())
 
 ```
 
 This package is using the [Launch Library 2 API][launchlibrary] to get the information.
 
 [launchlibrary]: https://thespacedevs.com/llapi
-
```

### Comparing `pylaunches-1.3.0/setup.py` & `pylaunches-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     DESCRIPTION = fh.read()
 
 setuptools.setup(
     name="pylaunches",
-    version="1.3.0",
+    version="1.4.0",
     author="Joakim Sorensen",
     author_email="hi@ludeeus.dev",
     description="",
     long_description=DESCRIPTION,
     install_requires=["aiohttp", "pytest-runner"],
     long_description_content_type="text/markdown",
     url="https://github.com/ludeeus/pylaunches",
```

