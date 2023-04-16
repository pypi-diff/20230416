# Comparing `tmp/aihandler-1.9.2.tar.gz` & `tmp/aihandler-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aihandler-1.9.2.tar", last modified: Sun Apr 16 17:52:55 2023, max compression
+gzip compressed data, was "aihandler-1.9.3.tar", last modified: Sun Apr 16 18:38:07 2023, max compression
```

## Comparing `aihandler-1.9.2.tar` & `aihandler-1.9.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:52:55.789569 aihandler-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 17:52:44.000000 aihandler-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-16 17:52:55.789569 aihandler-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-16 17:52:44.000000 aihandler-1.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 17:52:55.789569 aihandler-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-16 17:52:44.000000 aihandler-1.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:52:55.781569 aihandler-1.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:52:55.789569 aihandler-1.9.2/src/aihandler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:52:44.000000 aihandler-1.9.2/src/aihandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-16 17:52:44.000000 aihandler-1.9.2/src/aihandler/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-16 17:52:44.000000 aihandler-1.9.2/src/aihandler/controlnet_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-04-16 17:52:44.000000 aihandler-1.9.2/src/aihandler/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-16 17:52:44.000000 aihandler-1.9.2/src/aihandler/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-04-16 17:52:44.000000 aihandler-1.9.2/src/aihandler/llmrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-16 17:52:44.000000 aihandler-1.9.2/src/aihandler/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-16 17:52:44.000000 aihandler-1.9.2/src/aihandler/offline_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-04-16 17:52:44.000000 aihandler-1.9.2/src/aihandler/pyqt_offline_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-04-16 17:52:44.000000 aihandler-1.9.2/src/aihandler/qtvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    53718 2023-04-16 17:52:44.000000 aihandler-1.9.2/src/aihandler/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-04-16 17:52:44.000000 aihandler-1.9.2/src/aihandler/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-16 17:52:44.000000 aihandler-1.9.2/src/aihandler/settings_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-16 17:52:44.000000 aihandler-1.9.2/src/aihandler/socket_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-16 17:52:44.000000 aihandler-1.9.2/src/aihandler/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:52:55.789569 aihandler-1.9.2/src/aihandler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-16 17:52:55.000000 aihandler-1.9.2/src/aihandler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-16 17:52:55.000000 aihandler-1.9.2/src/aihandler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 17:52:55.000000 aihandler-1.9.2/src/aihandler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-16 17:52:55.000000 aihandler-1.9.2/src/aihandler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-16 17:52:55.000000 aihandler-1.9.2/src/aihandler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:38:07.687915 aihandler-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 18:37:56.000000 aihandler-1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-16 18:38:07.687915 aihandler-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-04-16 18:37:56.000000 aihandler-1.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 18:38:07.687915 aihandler-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-16 18:37:56.000000 aihandler-1.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:38:07.683915 aihandler-1.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:38:07.687915 aihandler-1.9.3/src/aihandler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:37:56.000000 aihandler-1.9.3/src/aihandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-16 18:37:56.000000 aihandler-1.9.3/src/aihandler/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-16 18:37:56.000000 aihandler-1.9.3/src/aihandler/controlnet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-04-16 18:37:56.000000 aihandler-1.9.3/src/aihandler/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-16 18:37:56.000000 aihandler-1.9.3/src/aihandler/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-04-16 18:37:56.000000 aihandler-1.9.3/src/aihandler/llmrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-16 18:37:56.000000 aihandler-1.9.3/src/aihandler/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-16 18:37:56.000000 aihandler-1.9.3/src/aihandler/offline_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-04-16 18:37:56.000000 aihandler-1.9.3/src/aihandler/pyqt_offline_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-04-16 18:37:56.000000 aihandler-1.9.3/src/aihandler/qtvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53718 2023-04-16 18:37:56.000000 aihandler-1.9.3/src/aihandler/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-04-16 18:37:56.000000 aihandler-1.9.3/src/aihandler/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-16 18:37:56.000000 aihandler-1.9.3/src/aihandler/settings_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-16 18:37:56.000000 aihandler-1.9.3/src/aihandler/socket_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-16 18:37:56.000000 aihandler-1.9.3/src/aihandler/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:38:07.687915 aihandler-1.9.3/src/aihandler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-16 18:38:07.000000 aihandler-1.9.3/src/aihandler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-16 18:38:07.000000 aihandler-1.9.3/src/aihandler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 18:38:07.000000 aihandler-1.9.3/src/aihandler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-16 18:38:07.000000 aihandler-1.9.3/src/aihandler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-16 18:38:07.000000 aihandler-1.9.3/src/aihandler.egg-info/top_level.txt
```

### Comparing `aihandler-1.9.2/LICENSE` & `aihandler-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.2/PKG-INFO` & `aihandler-1.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aihandler
-Version: 1.9.2
+Version: 1.9.3
 Summary: AI Handler: An engine which wraps certain huggingface models
 Home-page: https://github.com/Capsize-Games/aihandler
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `aihandler-1.9.2/README.md` & `aihandler-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.2/setup.py` & `aihandler-1.9.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,25 +37,25 @@
     "tqdm==4.65.0",
     "charset-normalizer==3.1.0",
     "opencv-python==4.7.0.72",
     "setuptools==65.5.1",
     "sympy==1.11.1",
     "typing_extensions==4.5.0",
     "urllib3==1.26.15",
-    "diffusers==0.15.0",
+    # "diffusers==0.15.0",
     "transformers==4.28.1",
     "compel==1.1.3",
     "sympy==1.11.1",
     "regex",
 ]
 
 
 setup(
     name="aihandler",
-    version="1.9.2",
+    version="1.9.3",
     author="Capsize LLC",
     description="AI Handler: An engine which wraps certain huggingface models",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="ai, chatbot, chat, ai",
     license="AGPL-3.0",
     author_email="contact@capsize.gg",
```

### Comparing `aihandler-1.9.2/src/aihandler/base_runner.py` & `aihandler-1.9.3/src/aihandler/base_runner.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.2/src/aihandler/controlnet_utils.py` & `aihandler-1.9.3/src/aihandler/controlnet_utils.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.2/src/aihandler/database.py` & `aihandler-1.9.3/src/aihandler/database.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.2/src/aihandler/llmrunner.py` & `aihandler-1.9.3/src/aihandler/llmrunner.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.2/src/aihandler/logger.py` & `aihandler-1.9.3/src/aihandler/logger.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.2/src/aihandler/offline_client.py` & `aihandler-1.9.3/src/aihandler/offline_client.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.2/src/aihandler/pyqt_offline_client.py` & `aihandler-1.9.3/src/aihandler/pyqt_offline_client.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.2/src/aihandler/qtvar.py` & `aihandler-1.9.3/src/aihandler/qtvar.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.2/src/aihandler/runner.py` & `aihandler-1.9.3/src/aihandler/runner.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.2/src/aihandler/settings.py` & `aihandler-1.9.3/src/aihandler/settings.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.2/src/aihandler/settings_manager.py` & `aihandler-1.9.3/src/aihandler/settings_manager.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.2/src/aihandler/socket_server.py` & `aihandler-1.9.3/src/aihandler/socket_server.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.2/src/aihandler/util.py` & `aihandler-1.9.3/src/aihandler/util.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.2/src/aihandler.egg-info/PKG-INFO` & `aihandler-1.9.3/src/aihandler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aihandler
-Version: 1.9.2
+Version: 1.9.3
 Summary: AI Handler: An engine which wraps certain huggingface models
 Home-page: https://github.com/Capsize-Games/aihandler
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `aihandler-1.9.2/src/aihandler.egg-info/SOURCES.txt` & `aihandler-1.9.3/src/aihandler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.2/src/aihandler.egg-info/requires.txt` & `aihandler-1.9.3/src/aihandler.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -26,12 +26,11 @@
 tqdm==4.65.0
 charset-normalizer==3.1.0
 opencv-python==4.7.0.72
 setuptools==65.5.1
 sympy==1.11.1
 typing_extensions==4.5.0
 urllib3==1.26.15
-diffusers==0.15.0
 transformers==4.28.1
 compel==1.1.3
 sympy==1.11.1
 regex
```

