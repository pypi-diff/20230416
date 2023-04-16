# Comparing `tmp/griptape_tools-0.5.2.tar.gz` & `tmp/griptape_tools-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_tools-0.5.2.tar", max compression
+gzip compressed data, was "griptape_tools-0.5.3.tar", max compression
```

## Comparing `griptape_tools-0.5.2.tar` & `griptape_tools-0.5.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.5.2/LICENSE
--rw-r--r--   0        0        0     1402 2023-04-13 17:49:58.210759 griptape_tools-0.5.2/README.md
--rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.5.2/griptape/__init__.py
--rw-r--r--   0        0        0      352 2023-04-13 16:07:18.435628 griptape_tools-0.5.2/griptape/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.2/griptape/tools/aws_cli/__init__.py
--rw-r--r--   0        0        0      159 2023-04-13 16:14:30.544316 griptape_tools-0.5.2/griptape/tools/aws_cli/manifest.yml
--rw-r--r--   0        0        0       78 2023-04-13 21:55:09.487715 griptape_tools-0.5.2/griptape/tools/aws_cli/requirements.txt
--rw-r--r--   0        0        0     1516 2023-04-13 16:56:09.699727 griptape_tools-0.5.2/griptape/tools/aws_cli/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.2/griptape/tools/calculator/__init__.py
--rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.5.2/griptape/tools/calculator/manifest.yml
--rw-r--r--   0        0        0       21 2023-04-13 21:55:09.483314 griptape_tools-0.5.2/griptape/tools/calculator/requirements.txt
--rw-r--r--   0        0        0      725 2023-04-13 16:45:31.204704 griptape_tools-0.5.2/griptape/tools/calculator/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.2/griptape/tools/email_client/__init__.py
--rw-r--r--   0        0        0      153 2023-04-12 21:25:06.766972 griptape_tools-0.5.2/griptape/tools/email_client/manifest.yml
--rw-r--r--   0        0        0       21 2023-04-13 21:55:09.481296 griptape_tools-0.5.2/griptape/tools/email_client/requirements.txt
--rw-r--r--   0        0        0     2409 2023-04-14 19:59:52.372885 griptape_tools-0.5.2/griptape/tools/email_client/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.2/griptape/tools/sql_client/__init__.py
--rw-r--r--   0        0        0      154 2023-04-12 19:53:04.579660 griptape_tools-0.5.2/griptape/tools/sql_client/manifest.yml
--rw-r--r--   0        0        0       33 2023-04-13 21:55:09.486224 griptape_tools-0.5.2/griptape/tools/sql_client/requirements.txt
--rw-r--r--   0        0        0     1328 2023-04-13 16:45:31.207393 griptape_tools-0.5.2/griptape/tools/sql_client/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.5.2/griptape/tools/web_scraper/__init__.py
--rw-r--r--   0        0        0      195 2023-04-11 21:24:23.634297 griptape_tools-0.5.2/griptape/tools/web_scraper/manifest.yml
--rw-r--r--   0        0        0       53 2023-04-13 21:55:09.484886 griptape_tools-0.5.2/griptape/tools/web_scraper/requirements.txt
--rw-r--r--   0        0        0     4506 2023-04-13 15:55:25.582021 griptape_tools-0.5.2/griptape/tools/web_scraper/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.5.2/griptape/tools/web_search/__init__.py
--rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.5.2/griptape/tools/web_search/manifest.yml
--rw-r--r--   0        0        0       29 2023-04-13 21:55:09.489187 griptape_tools-0.5.2/griptape/tools/web_search/requirements.txt
--rw-r--r--   0        0        0     2332 2023-04-12 19:48:33.963528 griptape_tools-0.5.2/griptape/tools/web_search/tool.py
--rw-r--r--   0        0        0      526 2023-04-14 20:00:46.071902 griptape_tools-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 griptape_tools-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.5.3/LICENSE
+-rw-r--r--   0        0        0     1402 2023-04-13 17:49:58.210759 griptape_tools-0.5.3/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.5.3/griptape/__init__.py
+-rw-r--r--   0        0        0      352 2023-04-13 16:07:18.435628 griptape_tools-0.5.3/griptape/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.3/griptape/tools/aws_cli/__init__.py
+-rw-r--r--   0        0        0      159 2023-04-13 16:14:30.544316 griptape_tools-0.5.3/griptape/tools/aws_cli/manifest.yml
+-rw-r--r--   0        0        0       78 2023-04-13 21:55:09.487715 griptape_tools-0.5.3/griptape/tools/aws_cli/requirements.txt
+-rw-r--r--   0        0        0     1516 2023-04-13 16:56:09.699727 griptape_tools-0.5.3/griptape/tools/aws_cli/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.3/griptape/tools/calculator/__init__.py
+-rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.5.3/griptape/tools/calculator/manifest.yml
+-rw-r--r--   0        0        0       21 2023-04-13 21:55:09.483314 griptape_tools-0.5.3/griptape/tools/calculator/requirements.txt
+-rw-r--r--   0        0        0      725 2023-04-13 16:45:31.204704 griptape_tools-0.5.3/griptape/tools/calculator/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.3/griptape/tools/email_client/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-12 21:25:06.766972 griptape_tools-0.5.3/griptape/tools/email_client/manifest.yml
+-rw-r--r--   0        0        0       21 2023-04-13 21:55:09.481296 griptape_tools-0.5.3/griptape/tools/email_client/requirements.txt
+-rw-r--r--   0        0        0     2409 2023-04-14 19:59:52.372885 griptape_tools-0.5.3/griptape/tools/email_client/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.3/griptape/tools/sql_client/__init__.py
+-rw-r--r--   0        0        0      154 2023-04-12 19:53:04.579660 griptape_tools-0.5.3/griptape/tools/sql_client/manifest.yml
+-rw-r--r--   0        0        0       33 2023-04-13 21:55:09.486224 griptape_tools-0.5.3/griptape/tools/sql_client/requirements.txt
+-rw-r--r--   0        0        0     1328 2023-04-13 16:45:31.207393 griptape_tools-0.5.3/griptape/tools/sql_client/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.5.3/griptape/tools/web_scraper/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-11 21:24:23.634297 griptape_tools-0.5.3/griptape/tools/web_scraper/manifest.yml
+-rw-r--r--   0        0        0       53 2023-04-13 21:55:09.484886 griptape_tools-0.5.3/griptape/tools/web_scraper/requirements.txt
+-rw-r--r--   0        0        0     4758 2023-04-16 15:54:43.085400 griptape_tools-0.5.3/griptape/tools/web_scraper/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.5.3/griptape/tools/web_search/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.5.3/griptape/tools/web_search/manifest.yml
+-rw-r--r--   0        0        0       29 2023-04-13 21:55:09.489187 griptape_tools-0.5.3/griptape/tools/web_search/requirements.txt
+-rw-r--r--   0        0        0     2332 2023-04-12 19:48:33.963528 griptape_tools-0.5.3/griptape/tools/web_search/tool.py
+-rw-r--r--   0        0        0      526 2023-04-16 15:58:58.633882 griptape_tools-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 griptape_tools-0.5.3/PKG-INFO
```

### Comparing `griptape_tools-0.5.2/LICENSE` & `griptape_tools-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.2/README.md` & `griptape_tools-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.2/griptape/tools/aws_cli/tool.py` & `griptape_tools-0.5.3/griptape/tools/aws_cli/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.2/griptape/tools/calculator/tool.py` & `griptape_tools-0.5.3/griptape/tools/calculator/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.2/griptape/tools/email_client/tool.py` & `griptape_tools-0.5.3/griptape/tools/email_client/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.2/griptape/tools/sql_client/tool.py` & `griptape_tools-0.5.3/griptape/tools/sql_client/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.2/griptape/tools/web_scraper/tool.py` & `griptape_tools-0.5.3/griptape/tools/web_scraper/tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from __future__ import annotations
+import ast
+import logging
 from typing import TYPE_CHECKING, Optional
 import json
 from typing import Union
 from attr import define, field
 from schema import Schema, Literal
 from griptape.core import BaseTool, action
 
@@ -54,15 +56,15 @@
                     "query",
                     description="Search query"
                 ): str
             }
         })
     })
     def search_page(self, value: bytes) -> str:
-        params = json.loads(value.decode())
+        params = ast.literal_eval(value.decode())
         index = self._to_vector_index(self._load_page(params["url"]).get("text"))
 
         return str(index.query(params["query"])).strip()
 
     @action(config={
         "name": "get_authors",
         "description": "Can be used to get a list of web page authors",
@@ -123,14 +125,18 @@
         config = use_config()
         page = trafilatura.fetch_url(url)
 
         # This disables signal, so that trafilatura can work on any thread:
         # More info: https://trafilatura.readthedocs.io/en/latest/usage-python.html#disabling-signal
         config.set("DEFAULT", "EXTRACTION_TIMEOUT", "0")
 
+        # Disable error logging in trafilatura as it sometimes logs errors from lxml, even though
+        # the end result of page parsing is successful.
+        logging.getLogger("trafilatura").setLevel(logging.FATAL)
+
         if page is None:
             return "error: can't access URL"
         else:
             return json.loads(
                 trafilatura.extract(
                     page,
                     include_links=self.env_value("INCLUDE_LINKS"),
```

### Comparing `griptape_tools-0.5.2/griptape/tools/web_search/tool.py` & `griptape_tools-0.5.3/griptape/tools/web_search/tool.py`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.2/pyproject.toml` & `griptape_tools-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "griptape-tools"
-version = "0.5.2"
+version = "0.5.3"
 description = "Tools for the griptape-core package."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape-tools"
 
 packages = [
```

### Comparing `griptape_tools-0.5.2/PKG-INFO` & `griptape_tools-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: griptape-tools
-Version: 0.5.2
+Version: 0.5.3
 Summary: Tools for the griptape-core package.
 Home-page: https://github.com/griptape-ai/griptape-tools
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

