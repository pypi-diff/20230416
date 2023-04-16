# Comparing `tmp/jupyterlab_code_formatter-1.6.0.tar.gz` & `tmp/jupyterlab_code_formatter-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterlab_code_formatter-1.6.0.tar", last modified: Sun Mar 26 14:05:55 2023, max compression
+gzip compressed data, was "jupyterlab_code_formatter-1.6.1.tar", last modified: Sun Apr 16 18:07:31 2023, max compression
```

## Comparing `jupyterlab_code_formatter-1.6.0.tar` & `jupyterlab_code_formatter-1.6.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-26 14:05:55.207172 jupyterlab_code_formatter-1.6.0/
--rw-rw-r--   0 root         (0) root         (0)     1052 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      447 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3429 2023-03-26 14:05:55.207172 jupyterlab_code_formatter-1.6.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     2668 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.0/README.md
--rw-rw-r--   0 root         (0) root         (0)      211 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.0/install.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-26 14:05:55.199171 jupyterlab_code_formatter-1.6.0/jupyter-config/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-26 14:05:55.203172 jupyterlab_code_formatter-1.6.0/jupyter-config/jupyter_notebook_config.d/
--rw-rw-r--   0 root         (0) root         (0)      102 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.0/jupyter-config/jupyter_notebook_config.d/jupyterlab_code_formatter.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-26 14:05:55.203172 jupyterlab_code_formatter-1.6.0/jupyter-config/jupyter_server_config.d/
--rw-rw-r--   0 root         (0) root         (0)      100 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.0/jupyter-config/jupyter_server_config.d/jupyterlab_code_formatter.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-26 14:05:55.203172 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/
--rw-rw-r--   0 root         (0) root         (0)      819 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      459 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/_version.py
--rw-rw-r--   0 root         (0) root         (0)    12749 2023-03-26 13:28:58.000000 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/formatters.py
--rw-rw-r--   0 root         (0) root         (0)     4510 2023-03-26 13:28:58.000000 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/handlers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-26 14:05:55.207172 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/labextension/
--rw-rw-r--   0 root         (0) root         (0)     2734 2023-03-26 14:05:54.000000 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/labextension/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-26 14:05:55.203172 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/labextension/schemas/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-26 14:05:55.203172 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/labextension/schemas/@ryantam626/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-26 14:05:55.207172 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/labextension/schemas/@ryantam626/jupyterlab_code_formatter/
--rw-rw-r--   0 root         (0) root         (0)     2618 2023-03-26 14:05:54.000000 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/labextension/schemas/@ryantam626/jupyterlab_code_formatter/package.json.orig
--rw-rw-r--   0 root         (0) root         (0)    13640 2023-03-26 14:05:54.000000 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/labextension/schemas/@ryantam626/jupyterlab_code_formatter/settings.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-26 14:05:55.207172 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/labextension/static/
--rw-r--r--   0 root         (0) root         (0)     8139 2023-03-26 14:05:54.000000 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/labextension/static/160.3ef5c980b8cf8340ee46.js
--rw-r--r--   0 root         (0) root         (0)     6650 2023-03-26 14:05:54.000000 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/labextension/static/remoteEntry.d9a0f67ce40945c257d4.js
--rw-r--r--   0 root         (0) root         (0)      118 2023-03-26 14:05:54.000000 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/labextension/static/style.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-26 14:05:55.207172 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3429 2023-03-26 14:05:55.000000 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1219 2023-03-26 14:05:55.000000 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-26 14:05:55.000000 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-18 17:20:18.000000 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       16 2023-03-26 14:05:55.000000 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-03-26 14:05:55.000000 jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)     2618 2023-03-26 13:30:25.000000 jupyterlab_code_formatter-1.6.0/package.json
--rw-rw-r--   0 root         (0) root         (0)      145 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-26 14:05:55.207172 jupyterlab_code_formatter-1.6.0/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2725 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-26 14:05:55.207172 jupyterlab_code_formatter-1.6.0/src/
--rw-rw-r--   0 root         (0) root         (0)     1184 2023-03-26 13:28:58.000000 jupyterlab_code_formatter-1.6.0/src/client.ts
--rw-rw-r--   0 root         (0) root         (0)     1350 2023-03-26 14:02:50.000000 jupyterlab_code_formatter-1.6.0/src/constants.ts
--rw-rw-r--   0 root         (0) root         (0)     7391 2023-03-26 13:28:58.000000 jupyterlab_code_formatter-1.6.0/src/formatter.ts
--rw-rw-r--   0 root         (0) root         (0)     7789 2023-03-26 13:28:58.000000 jupyterlab_code_formatter-1.6.0/src/index.ts
--rw-rw-r--   0 root         (0) root         (0)      534 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.0/tsconfig.json
--rw-rw-r--   0 root         (0) root         (0)     3817 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.0/tslint.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.853280 jupyterlab_code_formatter-1.6.1/
+-rw-rw-r--   0 root         (0) root         (0)     1052 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      447 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-04-16 18:07:31.853280 jupyterlab_code_formatter-1.6.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     2668 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/README.md
+-rw-rw-r--   0 root         (0) root         (0)      211 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/install.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.845280 jupyterlab_code_formatter-1.6.1/jupyter-config/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.849280 jupyterlab_code_formatter-1.6.1/jupyter-config/jupyter_notebook_config.d/
+-rw-rw-r--   0 root         (0) root         (0)      102 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/jupyter-config/jupyter_notebook_config.d/jupyterlab_code_formatter.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.849280 jupyterlab_code_formatter-1.6.1/jupyter-config/jupyter_server_config.d/
+-rw-rw-r--   0 root         (0) root         (0)      100 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/jupyter-config/jupyter_server_config.d/jupyterlab_code_formatter.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.849280 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/
+-rw-rw-r--   0 root         (0) root         (0)      819 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      459 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/_version.py
+-rw-rw-r--   0 root         (0) root         (0)    12749 2023-03-26 13:28:58.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/formatters.py
+-rw-rw-r--   0 root         (0) root         (0)     4316 2023-04-16 16:44:42.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/handlers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.853280 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/
+-rw-rw-r--   0 root         (0) root         (0)     2734 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.845280 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/schemas/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.845280 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/schemas/@ryantam626/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.853280 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/schemas/@ryantam626/jupyterlab_code_formatter/
+-rw-rw-r--   0 root         (0) root         (0)     2618 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/schemas/@ryantam626/jupyterlab_code_formatter/package.json.orig
+-rw-rw-r--   0 root         (0) root         (0)    13640 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/schemas/@ryantam626/jupyterlab_code_formatter/settings.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.853280 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/static/
+-rw-r--r--   0 root         (0) root         (0)     8139 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/static/160.ee2bfa087021ad817bae.js
+-rw-r--r--   0 root         (0) root         (0)     6650 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/static/remoteEntry.d347e3dfbeaa4b572523.js
+-rw-r--r--   0 root         (0) root         (0)      118 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/static/style.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.853280 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1219 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-18 17:20:18.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-16 18:07:31.000000 jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     2618 2023-04-16 17:56:10.000000 jupyterlab_code_formatter-1.6.1/package.json
+-rw-rw-r--   0 root         (0) root         (0)      145 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 18:07:31.853280 jupyterlab_code_formatter-1.6.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2725 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:07:31.853280 jupyterlab_code_formatter-1.6.1/src/
+-rw-rw-r--   0 root         (0) root         (0)     1184 2023-03-26 13:28:58.000000 jupyterlab_code_formatter-1.6.1/src/client.ts
+-rw-rw-r--   0 root         (0) root         (0)     1350 2023-04-16 17:56:10.000000 jupyterlab_code_formatter-1.6.1/src/constants.ts
+-rw-rw-r--   0 root         (0) root         (0)     7391 2023-03-26 13:28:58.000000 jupyterlab_code_formatter-1.6.1/src/formatter.ts
+-rw-rw-r--   0 root         (0) root         (0)     7789 2023-03-26 13:28:58.000000 jupyterlab_code_formatter-1.6.1/src/index.ts
+-rw-rw-r--   0 root         (0) root         (0)      534 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/tsconfig.json
+-rw-rw-r--   0 root         (0) root         (0)     3817 2022-12-26 12:18:32.000000 jupyterlab_code_formatter-1.6.1/tslint.json
```

### Comparing `jupyterlab_code_formatter-1.6.0/LICENSE` & `jupyterlab_code_formatter-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-1.6.0/PKG-INFO` & `jupyterlab_code_formatter-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab_code_formatter
-Version: 1.6.0
+Version: 1.6.1
 Summary: Code formatter for JupyterLab
 Home-page: https://github.com/ryantam626/jupyterlab_code_formatter
 Author: Ryan Tam
 License: MIT
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupyterlab_code_formatter Version: 1.6.0 Summary:
+Metadata-Version: 2.1 Name: jupyterlab_code_formatter Version: 1.6.1 Summary:
 Code formatter for JupyterLab Home-page: https://github.com/ryantam626/
 jupyterlab_code_formatter Author: Ryan Tam License: MIT Keywords:
 Jupyter,JupyterLab,JupyterLab3 Platform: Linux Platform: Mac OS X Platform:
 Windows Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `jupyterlab_code_formatter-1.6.0/README.md` & `jupyterlab_code_formatter-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/__init__.py` & `jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/formatters.py` & `jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/formatters.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/handlers.py` & `jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/handlers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 
-import pkg_resources
+from importlib.metadata import version
 from jupyter_server.base.handlers import APIHandler
 from jupyter_server.serverapp import ServerWebApplication
 from jupyter_server.utils import url_path_join
 
 from .formatters import SERVER_FORMATTERS
 
 
@@ -44,17 +44,15 @@
                 VersionAPIHandler,
             )
         ],
     )
 
 
 def check_plugin_version(handler: APIHandler):
-    server_extension_version = pkg_resources.get_distribution(
-        "jupyterlab_code_formatter"
-    ).version
+    server_extension_version = version("jupyterlab_code_formatter")
     lab_extension_version = handler.request.headers.get("Plugin-Version")
     version_matches = server_extension_version == lab_extension_version
     if not version_matches:
         handler.set_status(
             422,
             f"Mismatched versions of server extension ({server_extension_version}) "
             f"and lab extension ({lab_extension_version}). "
@@ -121,16 +119,8 @@
                         formatted_code.append({"error": str(e)})
                 self.finish(json.dumps({"code": formatted_code}))
 
 
 class VersionAPIHandler(APIHandler):
     def get(self) -> None:
         """Show what version is this server plugin on."""
-        self.finish(
-            json.dumps(
-                {
-                    "version": pkg_resources.get_distribution(
-                        "jupyterlab_code_formatter"
-                    ).version
-                }
-            )
-        )
+        self.finish(json.dumps({"version": version("jupyterlab_code_formatter")}))
```

### Comparing `jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/labextension/package.json` & `jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96796875%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.d347e3dfbeaa4b572523.js'}}",*

 * * "'version'": "'1.6.1'"}*

```diff
@@ -27,15 +27,15 @@
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/ryantam626/jupyterlab_code_formatter",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.d9a0f67ce40945c257d4.js"
+            "load": "static/remoteEntry.d347e3dfbeaa4b572523.js"
         },
         "discovery": {
             "kernel": [
                 {
                     "base": {
                         "name": "jupyterlab_code_formatter"
                     },
@@ -80,9 +80,9 @@
         "lint": "tslint src/*.ts",
         "prepare": "jlpm run clean && jlpm run build:prod",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lib/index.d.ts",
-    "version": "1.6.0"
+    "version": "1.6.1"
 }
```

### Comparing `jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/labextension/schemas/@ryantam626/jupyterlab_code_formatter/package.json.orig` & `jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/schemas/@ryantam626/jupyterlab_code_formatter/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'1.6.1'"}*

```diff
@@ -76,9 +76,9 @@
         "lint": "tslint src/*.ts",
         "prepare": "jlpm run clean && jlpm run build:prod",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lib/index.d.ts",
-    "version": "1.6.0"
+    "version": "1.6.1"
 }
```

### Comparing `jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/labextension/schemas/@ryantam626/jupyterlab_code_formatter/settings.json` & `jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/schemas/@ryantam626/jupyterlab_code_formatter/settings.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/labextension/static/160.3ef5c980b8cf8340ee46.js` & `jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/static/160.ee2bfa087021ad817bae.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -9,15 +9,15 @@
                 a = r(884),
                 n = r(194),
                 i = r(448),
                 c = r(209),
                 l = r(848),
                 d = r(613);
             ! function(e) {
-                e.SHORT_PLUGIN_NAME = "jupyterlab_code_formatter", e.FORMAT_COMMAND = `${e.SHORT_PLUGIN_NAME}:format`, e.FORMAT_ALL_COMMAND = `${e.SHORT_PLUGIN_NAME}:format_all`, e.ICON_FORMAT_ALL_SVG = '<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" focusable="false" width="1em" height="1em" style="-ms-transform: rotate(360deg); -webkit-transform: rotate(360deg); transform: rotate(360deg);" preserveAspectRatio="xMidYMid meet" viewBox="0 0 1792 1792"><path class="jp-icon3" d="M1473 929q7-118-33-226.5t-113-189t-177-131T929 325q-116-7-225.5 32t-192 110.5t-135 175T317 863q-7 118 33 226.5t113 189t177.5 131T862 1467q155 9 293-59t224-195.5t94-283.5zM1792 0l-349 348q120 117 180.5 272t50.5 321q-11 183-102 339t-241 255.5T999 1660L0 1792l347-347q-120-116-180.5-271.5T116 852q11-184 102-340t241.5-255.5T792 132q167-22 500-66t500-66z" fill="#626262"/></svg>', e.ICON_FORMAT_ALL = "fa fa-superpowers", e.LONG_PLUGIN_NAME = `@ryantam626/${e.SHORT_PLUGIN_NAME}`, e.SETTINGS_SECTION = `${e.LONG_PLUGIN_NAME}:settings`, e.COMMAND_SECTION_NAME = "Jupyterlab Code Formatter", e.PLUGIN_VERSION = "1.6.0"
+                e.SHORT_PLUGIN_NAME = "jupyterlab_code_formatter", e.FORMAT_COMMAND = `${e.SHORT_PLUGIN_NAME}:format`, e.FORMAT_ALL_COMMAND = `${e.SHORT_PLUGIN_NAME}:format_all`, e.ICON_FORMAT_ALL_SVG = '<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" focusable="false" width="1em" height="1em" style="-ms-transform: rotate(360deg); -webkit-transform: rotate(360deg); transform: rotate(360deg);" preserveAspectRatio="xMidYMid meet" viewBox="0 0 1792 1792"><path class="jp-icon3" d="M1473 929q7-118-33-226.5t-113-189t-177-131T929 325q-116-7-225.5 32t-192 110.5t-135 175T317 863q-7 118 33 226.5t113 189t177.5 131T862 1467q155 9 293-59t224-195.5t94-283.5zM1792 0l-349 348q120 117 180.5 272t50.5 321q-11 183-102 339t-241 255.5T999 1660L0 1792l347-347q-120-116-180.5-271.5T116 852q11-184 102-340t241.5-255.5T792 132q167-22 500-66t500-66z" fill="#626262"/></svg>', e.ICON_FORMAT_ALL = "fa fa-superpowers", e.LONG_PLUGIN_NAME = `@ryantam626/${e.SHORT_PLUGIN_NAME}`, e.SETTINGS_SECTION = `${e.LONG_PLUGIN_NAME}:settings`, e.COMMAND_SECTION_NAME = "Jupyterlab Code Formatter", e.PLUGIN_VERSION = "1.6.1"
             }(o || (o = {}));
             class h {
                 constructor(e) {
                     this.client = e
                 }
                 formatCode(e, t, r, o, s) {
                     return this.client.request("format" + (s ? "?cached" : ""), "POST", JSON.stringify({
```

### Comparing `jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter/labextension/static/remoteEntry.d9a0f67ce40945c257d4.js` & `jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter/labextension/static/remoteEntry.d347e3dfbeaa4b572523.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@ryantam626/jupyterlab_code_formatter"] = (() => {
     "use strict";
-    var e, r, t, n, o, a, i, u, l, f, s, d, p, c, h, v = {
+    var e, r, t, n, o, a, i, u, l, f, s, p, d, c, h, v = {
             983: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(160).then((() => () => t(160))),
                         "./extension": () => t.e(160).then((() => () => t(160)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
@@ -20,102 +20,102 @@
                     };
                 t.d(r, {
                     get: () => o,
                     init: () => a
                 })
             }
         },
-        b = {};
+        y = {};
 
-    function y(e) {
-        if (b[e]) return b[e].exports;
-        var r = b[e] = {
+    function m(e) {
+        if (y[e]) return y[e].exports;
+        var r = y[e] = {
             exports: {}
         };
-        return v[e](r, r.exports, y), r.exports
+        return v[e](r, r.exports, m), r.exports
     }
-    return y.m = v, y.d = (e, r) => {
-        for (var t in r) y.o(r, t) && !y.o(e, t) && Object.defineProperty(e, t, {
+    return m.m = v, m.d = (e, r) => {
+        for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + ".3ef5c980b8cf8340ee46.js", y.g = function() {
+    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + ".ee2bfa087021ad817bae.js", m.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), y.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@ryantam626/jupyterlab_code_formatter:", y.l = (t, n, o) => {
+    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@ryantam626/jupyterlab_code_formatter:", m.l = (t, n, o) => {
         if (e[t]) e[t].push(n);
         else {
             var a, i;
             if (void 0 !== o)
                 for (var u = document.getElementsByTagName("script"), l = 0; l < u.length; l++) {
                     var f = u[l];
                     if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + o) {
                         a = f;
                         break
                     }
                 }
-            a || (i = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, y.nc && a.setAttribute("nonce", y.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
+            a || (i = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, m.nc && a.setAttribute("nonce", m.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
             var s = (r, n) => {
-                    a.onerror = a.onload = null, clearTimeout(d);
+                    a.onerror = a.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                d = setTimeout(s.bind(null, void 0, {
+                p = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
             a.onerror = s.bind(null, a.onerror), a.onload = s.bind(null, a.onload), i && document.head.appendChild(a)
         }
-    }, y.r = e => {
+    }, m.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
-        y.S = {};
+        m.S = {};
         var e = {},
             r = {};
-        y.I = (t, n) => {
+        m.I = (t, n) => {
             n || (n = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
                 if (n.push(o), e[t]) return e[t];
-                y.o(y.S, t) || (y.S[t] = {});
-                var a = y.S[t],
+                m.o(m.S, t) || (m.S[t] = {});
+                var a = m.S[t],
                     i = "@ryantam626/jupyterlab_code_formatter",
                     u = [];
                 switch (t) {
                     case "default":
                         ((e, r, t) => {
                             var n = a[e] = a[e] || {},
                                 o = n[r];
                             (!o || !o.loaded && i > o.from) && (n[r] = {
-                                get: () => y.e(160).then((() => () => y(160))),
+                                get: () => m.e(160).then((() => () => m(160))),
                                 from: i
                             })
-                        })("@ryantam626/jupyterlab_code_formatter", "1.6.0")
+                        })("@ryantam626/jupyterlab_code_formatter", "1.6.1")
                 }
                 return e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        y.g.importScripts && (e = y.g.location + "");
-        var r = y.g.document;
+        m.g.importScripts && (e = m.g.location + "");
+        var r = m.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             t.length && (e = t[t.length - 1].src)
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), y.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), m.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -152,113 +152,113 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, u = 1, l = !0;; u++, i++) {
-                var f, s, d = u < e.length ? (typeof e[u])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == d ? u > n && !o : "" == d != o);
+                var f, s, p = u < e.length ? (typeof e[u])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !l || ("u" == p ? u > n && !o : "" == p != o);
                 if ("u" == s) {
-                    if (!l || "u" != d) return !1
+                    if (!l || "u" != p) return !1
                 } else if (l)
-                    if (d == s)
+                    if (p == s)
                         if (u <= n) {
                             if (f != e[u]) return !1
                         } else {
                             if (o ? f > e[u] : f < e[u]) return !1;
                             f != e[u] && (l = !1)
                         }
-                else if ("s" != d && "n" != d) {
+                else if ("s" != p && "n" != p) {
                     if (o || u <= n) return !1;
                     l = !1, u--
                 } else {
-                    if (u <= n || s < d != o) return !1;
+                    if (u <= n || s < p != o) return !1;
                     l = !1
-                } else "s" != d && "n" != d && (l = !1, u--)
+                } else "s" != p && "n" != p && (l = !1, u--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var d = [],
+            c = d.pop.bind(d);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
+            d.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? a(h, r) : !c())
         }
         return !!c()
     }, i = (e, r) => {
-        var t = y.S[e];
-        if (!t || !y.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = m.S[e];
+        if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, l = (e, r, t) => "Unsatisfied version " + r + " of shared singleton module " + e + " (required " + o(t) + ")", f = (e, r, t, n) => {
         var o = u(e, t);
         return a(n, o) || "undefined" != typeof console && console.warn && console.warn(l(t, o, n)), s(e[t][o])
-    }, s = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
-        var a = y.I(r);
-        return a && a.then ? a.then(e.bind(e, r, y.S[r], t, n, o)) : e(r, y.S[r], t, n)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), p = {}, c = {
-        679: () => d("default", "@jupyterlab/notebook", [1, 3, 6, 2]),
-        884: () => d("default", "@jupyterlab/apputils", [1, 3, 6, 2]),
-        194: () => d("default", "@jupyterlab/settingregistry", [1, 3, 6, 2]),
-        448: () => d("default", "@jupyterlab/mainmenu", [1, 3, 6, 2]),
-        209: () => d("default", "@jupyterlab/fileeditor", [1, 3, 6, 2]),
-        848: () => d("default", "@jupyterlab/coreutils", [1, 5, 6, 2]),
-        613: () => d("default", "@jupyterlab/services", [1, 6, 6, 2]),
-        923: () => d("default", "@lumino/disposable", [1, 1, 10, 0]),
-        215: () => d("default", "@jupyterlab/ui-components", [1, 3, 6, 2])
+    }, s = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, o) {
+        var a = m.I(r);
+        return a && a.then ? a.then(e.bind(e, r, m.S[r], t, n, o)) : e(r, m.S[r], t, n)
+    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), d = {}, c = {
+        679: () => p("default", "@jupyterlab/notebook", [1, 3, 6, 2]),
+        884: () => p("default", "@jupyterlab/apputils", [1, 3, 6, 2]),
+        194: () => p("default", "@jupyterlab/settingregistry", [1, 3, 6, 2]),
+        448: () => p("default", "@jupyterlab/mainmenu", [1, 3, 6, 2]),
+        209: () => p("default", "@jupyterlab/fileeditor", [1, 3, 6, 2]),
+        848: () => p("default", "@jupyterlab/coreutils", [1, 5, 6, 2]),
+        613: () => p("default", "@jupyterlab/services", [1, 6, 6, 2]),
+        923: () => p("default", "@lumino/disposable", [1, 1, 10, 0]),
+        215: () => p("default", "@jupyterlab/ui-components", [1, 3, 6, 2])
     }, h = {
         160: [679, 884, 194, 448, 209, 848, 613, 923, 215]
-    }, y.f.consumes = (e, r) => {
-        y.o(h, e) && h[e].forEach((e => {
-            if (y.o(p, e)) return r.push(p[e]);
+    }, m.f.consumes = (e, r) => {
+        m.o(h, e) && h[e].forEach((e => {
+            if (m.o(d, e)) return r.push(d[e]);
             var t = r => {
-                    p[e] = 0, v[e] = t => {
-                        delete b[e], t.exports = r()
+                    d[e] = 0, v[e] = t => {
+                        delete y[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete p[e], v[e] = t => {
-                        throw delete b[e], r
+                    delete d[e], v[e] = t => {
+                        throw delete y[e], r
                     }
                 };
             try {
                 var o = c[e]();
-                o.then ? r.push(p[e] = o.then(t).catch(n)) : t(o)
+                o.then ? r.push(d[e] = o.then(t).catch(n)) : t(o)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             408: 0
         };
-        y.f.j = (r, t) => {
-            var n = y.o(e, r) ? e[r] : void 0;
+        m.f.j = (r, t) => {
+            var n = m.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else {
                     var o = new Promise(((t, o) => {
                         n = e[r] = [t, o]
                     }));
                     t.push(n[2] = o);
-                    var a = y.p + y.u(r),
+                    var a = m.p + m.u(r),
                         i = new Error;
-                    y.l(a, (t => {
-                        if (y.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                    m.l(a, (t => {
+                        if (m.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
                             var o = t && ("load" === t.type ? "missing" : t.type),
                                 a = t && t.target && t.target.src;
                             i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
                         }
                     }), "chunk-" + r)
                 }
         };
         var r = (r, t) => {
-                for (var n, o, [a, i, u] = t, l = 0, f = []; l < a.length; l++) o = a[l], y.o(e, o) && e[o] && f.push(e[o][0]), e[o] = 0;
-                for (n in i) y.o(i, n) && (y.m[n] = i[n]);
-                for (u && u(y), r && r(t); f.length;) f.shift()()
+                for (var n, o, [a, i, u] = t, l = 0, f = []; l < a.length; l++) o = a[l], m.o(e, o) && e[o] && f.push(e[o][0]), e[o] = 0;
+                for (n in i) m.o(i, n) && (m.m[n] = i[n]);
+                for (u && u(m), r && r(t); f.length;) f.shift()()
             },
             t = self.webpackChunk_ryantam626_jupyterlab_code_formatter = self.webpackChunk_ryantam626_jupyterlab_code_formatter || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), y(983)
+    })(), m(983)
 })();
```

### Comparing `jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter.egg-info/PKG-INFO` & `jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-code-formatter
-Version: 1.6.0
+Version: 1.6.1
 Summary: Code formatter for JupyterLab
 Home-page: https://github.com/ryantam626/jupyterlab_code_formatter
 Author: Ryan Tam
 License: MIT
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupyterlab-code-formatter Version: 1.6.0 Summary:
+Metadata-Version: 2.1 Name: jupyterlab-code-formatter Version: 1.6.1 Summary:
 Code formatter for JupyterLab Home-page: https://github.com/ryantam626/
 jupyterlab_code_formatter Author: Ryan Tam License: MIT Keywords:
 Jupyter,JupyterLab,JupyterLab3 Platform: Linux Platform: Mac OS X Platform:
 Windows Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `jupyterlab_code_formatter-1.6.0/jupyterlab_code_formatter.egg-info/SOURCES.txt` & `jupyterlab_code_formatter-1.6.1/jupyterlab_code_formatter.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 jupyterlab_code_formatter.egg-info/dependency_links.txt
 jupyterlab_code_formatter.egg-info/not-zip-safe
 jupyterlab_code_formatter.egg-info/requires.txt
 jupyterlab_code_formatter.egg-info/top_level.txt
 jupyterlab_code_formatter/labextension/package.json
 jupyterlab_code_formatter/labextension/schemas/@ryantam626/jupyterlab_code_formatter/package.json.orig
 jupyterlab_code_formatter/labextension/schemas/@ryantam626/jupyterlab_code_formatter/settings.json
-jupyterlab_code_formatter/labextension/static/160.3ef5c980b8cf8340ee46.js
-jupyterlab_code_formatter/labextension/static/remoteEntry.d9a0f67ce40945c257d4.js
+jupyterlab_code_formatter/labextension/static/160.ee2bfa087021ad817bae.js
+jupyterlab_code_formatter/labextension/static/remoteEntry.d347e3dfbeaa4b572523.js
 jupyterlab_code_formatter/labextension/static/style.js
 src/client.ts
 src/constants.ts
 src/formatter.ts
 src/index.ts
```

### Comparing `jupyterlab_code_formatter-1.6.0/package.json` & `jupyterlab_code_formatter-1.6.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'1.6.1'"}*

```diff
@@ -76,9 +76,9 @@
         "lint": "tslint src/*.ts",
         "prepare": "jlpm run clean && jlpm run build:prod",
         "watch": "run-p watch:src watch:labextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:src": "tsc -w"
     },
     "types": "lib/index.d.ts",
-    "version": "1.6.0"
+    "version": "1.6.1"
 }
```

### Comparing `jupyterlab_code_formatter-1.6.0/setup.py` & `jupyterlab_code_formatter-1.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-1.6.0/src/client.ts` & `jupyterlab_code_formatter-1.6.1/src/client.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-1.6.0/src/constants.ts` & `jupyterlab_code_formatter-1.6.1/src/constants.ts`

 * *Files 9% similar despite different names*

```diff
@@ -6,9 +6,9 @@
   export const ICON_FORMAT_ALL_SVG =
     '<svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" focusable="false" width="1em" height="1em" style="-ms-transform: rotate(360deg); -webkit-transform: rotate(360deg); transform: rotate(360deg);" preserveAspectRatio="xMidYMid meet" viewBox="0 0 1792 1792"><path class="jp-icon3" d="M1473 929q7-118-33-226.5t-113-189t-177-131T929 325q-116-7-225.5 32t-192 110.5t-135 175T317 863q-7 118 33 226.5t113 189t177.5 131T862 1467q155 9 293-59t224-195.5t94-283.5zM1792 0l-349 348q120 117 180.5 272t50.5 321q-11 183-102 339t-241 255.5T999 1660L0 1792l347-347q-120-116-180.5-271.5T116 852q11-184 102-340t241.5-255.5T792 132q167-22 500-66t500-66z" fill="#626262"/></svg>';
   export const ICON_FORMAT_ALL = 'fa fa-superpowers';
   export const LONG_PLUGIN_NAME = `@ryantam626/${SHORT_PLUGIN_NAME}`;
   export const SETTINGS_SECTION = `${LONG_PLUGIN_NAME}:settings`;
   export const COMMAND_SECTION_NAME = 'Jupyterlab Code Formatter';
   // TODO: Use package.json info
-  export const PLUGIN_VERSION = '1.6.0';
+  export const PLUGIN_VERSION = '1.6.1';
 }
```

### Comparing `jupyterlab_code_formatter-1.6.0/src/formatter.ts` & `jupyterlab_code_formatter-1.6.1/src/formatter.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-1.6.0/src/index.ts` & `jupyterlab_code_formatter-1.6.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-1.6.0/tsconfig.json` & `jupyterlab_code_formatter-1.6.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_code_formatter-1.6.0/tslint.json` & `jupyterlab_code_formatter-1.6.1/tslint.json`

 * *Files identical despite different names*

