# Comparing `tmp/StableDiffusionAPI-0.0.4.tar.gz` & `tmp/StableDiffusionAPI-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StableDiffusionAPI-0.0.4.tar", last modified: Wed Apr 12 15:49:51 2023, max compression
+gzip compressed data, was "StableDiffusionAPI-0.0.5.tar", last modified: Sat Apr 15 23:00:01 2023, max compression
```

## Comparing `StableDiffusionAPI-0.0.4.tar` & `StableDiffusionAPI-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 15:49:51.508899 StableDiffusionAPI-0.0.4/
--rw-rw-rw-   0        0        0     2185 2023-04-10 10:15:54.000000 StableDiffusionAPI-0.0.4/LICENSE
--rw-rw-rw-   0        0        0        0 2023-04-10 23:23:24.000000 StableDiffusionAPI-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      923 2023-04-12 15:49:51.508899 StableDiffusionAPI-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-04-12 07:52:41.000000 StableDiffusionAPI-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-12 15:49:51.503900 StableDiffusionAPI-0.0.4/StableDiffusionAPI/
--rw-rw-rw-   0        0        0       96 2023-04-12 13:09:21.000000 StableDiffusionAPI-0.0.4/StableDiffusionAPI/SetKey.py
--rw-rw-rw-   0        0        0     5105 2023-04-12 15:43:25.000000 StableDiffusionAPI-0.0.4/StableDiffusionAPI/Text2Img.py
--rw-rw-rw-   0        0        0      144 2023-04-12 07:53:33.000000 StableDiffusionAPI-0.0.4/StableDiffusionAPI/__init__.py
--rw-rw-rw-   0        0        0       30 2023-04-12 07:45:34.000000 StableDiffusionAPI-0.0.4/StableDiffusionAPI/__main__.py
--rw-rw-rw-   0        0        0      115 2023-04-12 07:46:13.000000 StableDiffusionAPI-0.0.4/StableDiffusionAPI/key.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:49:51.507900 StableDiffusionAPI-0.0.4/StableDiffusionAPI.egg-info/
--rw-rw-rw-   0        0        0      923 2023-04-12 15:49:51.000000 StableDiffusionAPI-0.0.4/StableDiffusionAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-04-12 15:49:51.000000 StableDiffusionAPI-0.0.4/StableDiffusionAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 15:49:51.000000 StableDiffusionAPI-0.0.4/StableDiffusionAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-04-12 15:49:51.000000 StableDiffusionAPI-0.0.4/StableDiffusionAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      790 2023-04-12 15:49:14.000000 StableDiffusionAPI-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 15:49:51.509899 StableDiffusionAPI-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-15 23:00:01.863444 StableDiffusionAPI-0.0.5/
+-rw-rw-rw-   0        0        0     2185 2023-04-10 10:15:54.000000 StableDiffusionAPI-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-04-10 23:23:24.000000 StableDiffusionAPI-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1135 2023-04-15 23:00:01.862444 StableDiffusionAPI-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2023-04-15 22:46:25.000000 StableDiffusionAPI-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-15 23:00:01.857445 StableDiffusionAPI-0.0.5/StableDiffusionAPI/
+-rw-rw-rw-   0        0        0     9015 2023-04-15 22:41:17.000000 StableDiffusionAPI-0.0.5/StableDiffusionAPI/Community.py
+-rw-rw-rw-   0        0        0       96 2023-04-12 13:09:21.000000 StableDiffusionAPI-0.0.5/StableDiffusionAPI/SetKey.py
+-rw-rw-rw-   0        0        0     5105 2023-04-12 15:43:25.000000 StableDiffusionAPI-0.0.5/StableDiffusionAPI/Text2Img.py
+-rw-rw-rw-   0        0        0      146 2023-04-15 16:14:44.000000 StableDiffusionAPI-0.0.5/StableDiffusionAPI/__init__.py
+-rw-rw-rw-   0        0        0       30 2023-04-12 07:45:34.000000 StableDiffusionAPI-0.0.5/StableDiffusionAPI/__main__.py
+-rw-rw-rw-   0        0        0      115 2023-04-12 07:46:13.000000 StableDiffusionAPI-0.0.5/StableDiffusionAPI/key.py
+drwxrwxrwx   0        0        0        0 2023-04-15 23:00:01.862444 StableDiffusionAPI-0.0.5/StableDiffusionAPI.egg-info/
+-rw-rw-rw-   0        0        0     1135 2023-04-15 23:00:01.000000 StableDiffusionAPI-0.0.5/StableDiffusionAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-04-15 23:00:01.000000 StableDiffusionAPI-0.0.5/StableDiffusionAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-15 23:00:01.000000 StableDiffusionAPI-0.0.5/StableDiffusionAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-04-15 23:00:01.000000 StableDiffusionAPI-0.0.5/StableDiffusionAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      790 2023-04-15 22:59:32.000000 StableDiffusionAPI-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-15 23:00:01.863444 StableDiffusionAPI-0.0.5/setup.cfg
```

### Comparing `StableDiffusionAPI-0.0.4/LICENSE` & `StableDiffusionAPI-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `StableDiffusionAPI-0.0.4/PKG-INFO` & `StableDiffusionAPI-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StableDiffusionAPI
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to interface with the StableDiffusionAPI.com API
 Author-email: Jonathan Caraveo <jon@ziawe.com>
 Project-URL: Homepage, https://StableDiffusionAPI.com
 Project-URL: GitHub, https://github.com/caraveo/SDAPI/
 Project-URL: Bug Tracker, https://github.com/Caraveo/SDAPI/issues
 Project-URL: Guide, https://www.sparkandwave.com/stablediffusionapi/
 Classifier: Programming Language :: Python :: 3
@@ -17,9 +17,17 @@
 # StableDiffuionAPI
 ```
 import StableDiffusionAPI
 
 StableDiffusionAPI.Key("StableDiffusionAPI_KEY")
 StableDiffusionAPI.Text2Img("Tractor", 512, 512, "Tractor.png")
 ```
+
+# StableDiffuionAPI.Community
+```
+StableDiffusionAPI.Community as Community
+
+Community.Text2Img("dreamlike", "Cat", "dreamlike-cat.png")
+Community.Text2Img("midjourney", "Cat", "midjourney-cat.png")
+```
 # Requires API Key
 [StableDiffusionAPI.com](https://stablediffusionapi.com/)
```

### Comparing `StableDiffusionAPI-0.0.4/StableDiffusionAPI/Text2Img.py` & `StableDiffusionAPI-0.0.5/StableDiffusionAPI/Text2Img.py`

 * *Files identical despite different names*

### Comparing `StableDiffusionAPI-0.0.4/StableDiffusionAPI.egg-info/PKG-INFO` & `StableDiffusionAPI-0.0.5/StableDiffusionAPI.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StableDiffusionAPI
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package to interface with the StableDiffusionAPI.com API
 Author-email: Jonathan Caraveo <jon@ziawe.com>
 Project-URL: Homepage, https://StableDiffusionAPI.com
 Project-URL: GitHub, https://github.com/caraveo/SDAPI/
 Project-URL: Bug Tracker, https://github.com/Caraveo/SDAPI/issues
 Project-URL: Guide, https://www.sparkandwave.com/stablediffusionapi/
 Classifier: Programming Language :: Python :: 3
@@ -17,9 +17,17 @@
 # StableDiffuionAPI
 ```
 import StableDiffusionAPI
 
 StableDiffusionAPI.Key("StableDiffusionAPI_KEY")
 StableDiffusionAPI.Text2Img("Tractor", 512, 512, "Tractor.png")
 ```
+
+# StableDiffuionAPI.Community
+```
+StableDiffusionAPI.Community as Community
+
+Community.Text2Img("dreamlike", "Cat", "dreamlike-cat.png")
+Community.Text2Img("midjourney", "Cat", "midjourney-cat.png")
+```
 # Requires API Key
 [StableDiffusionAPI.com](https://stablediffusionapi.com/)
```

### Comparing `StableDiffusionAPI-0.0.4/pyproject.toml` & `StableDiffusionAPI-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 requires = ["setuptools>=61.0"]
 install_requires = ['random', 'json', 'time', 'urllib3', 'http.client']
 build-backend = "setuptools.build_meta"
 [project]
 name = "StableDiffusionAPI"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Jonathan Caraveo", email="jon@ziawe.com" },
 ]
 description = "A package to interface with the StableDiffusionAPI.com API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

