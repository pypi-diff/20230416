# Comparing `tmp/griptape_tools-0.5.3.tar.gz` & `tmp/griptape_tools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "griptape_tools-0.5.3.tar", max compression
+gzip compressed data, was "griptape_tools-0.6.0.tar", max compression
```

## Comparing `griptape_tools-0.5.3.tar` & `griptape_tools-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.5.3/LICENSE
--rw-r--r--   0        0        0     1402 2023-04-13 17:49:58.210759 griptape_tools-0.5.3/README.md
--rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.5.3/griptape/__init__.py
--rw-r--r--   0        0        0      352 2023-04-13 16:07:18.435628 griptape_tools-0.5.3/griptape/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.3/griptape/tools/aws_cli/__init__.py
--rw-r--r--   0        0        0      159 2023-04-13 16:14:30.544316 griptape_tools-0.5.3/griptape/tools/aws_cli/manifest.yml
--rw-r--r--   0        0        0       78 2023-04-13 21:55:09.487715 griptape_tools-0.5.3/griptape/tools/aws_cli/requirements.txt
--rw-r--r--   0        0        0     1516 2023-04-13 16:56:09.699727 griptape_tools-0.5.3/griptape/tools/aws_cli/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.3/griptape/tools/calculator/__init__.py
--rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.5.3/griptape/tools/calculator/manifest.yml
--rw-r--r--   0        0        0       21 2023-04-13 21:55:09.483314 griptape_tools-0.5.3/griptape/tools/calculator/requirements.txt
--rw-r--r--   0        0        0      725 2023-04-13 16:45:31.204704 griptape_tools-0.5.3/griptape/tools/calculator/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.3/griptape/tools/email_client/__init__.py
--rw-r--r--   0        0        0      153 2023-04-12 21:25:06.766972 griptape_tools-0.5.3/griptape/tools/email_client/manifest.yml
--rw-r--r--   0        0        0       21 2023-04-13 21:55:09.481296 griptape_tools-0.5.3/griptape/tools/email_client/requirements.txt
--rw-r--r--   0        0        0     2409 2023-04-14 19:59:52.372885 griptape_tools-0.5.3/griptape/tools/email_client/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.5.3/griptape/tools/sql_client/__init__.py
--rw-r--r--   0        0        0      154 2023-04-12 19:53:04.579660 griptape_tools-0.5.3/griptape/tools/sql_client/manifest.yml
--rw-r--r--   0        0        0       33 2023-04-13 21:55:09.486224 griptape_tools-0.5.3/griptape/tools/sql_client/requirements.txt
--rw-r--r--   0        0        0     1328 2023-04-13 16:45:31.207393 griptape_tools-0.5.3/griptape/tools/sql_client/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.5.3/griptape/tools/web_scraper/__init__.py
--rw-r--r--   0        0        0      195 2023-04-11 21:24:23.634297 griptape_tools-0.5.3/griptape/tools/web_scraper/manifest.yml
--rw-r--r--   0        0        0       53 2023-04-13 21:55:09.484886 griptape_tools-0.5.3/griptape/tools/web_scraper/requirements.txt
--rw-r--r--   0        0        0     4758 2023-04-16 15:54:43.085400 griptape_tools-0.5.3/griptape/tools/web_scraper/tool.py
--rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.5.3/griptape/tools/web_search/__init__.py
--rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.5.3/griptape/tools/web_search/manifest.yml
--rw-r--r--   0        0        0       29 2023-04-13 21:55:09.489187 griptape_tools-0.5.3/griptape/tools/web_search/requirements.txt
--rw-r--r--   0        0        0     2332 2023-04-12 19:48:33.963528 griptape_tools-0.5.3/griptape/tools/web_search/tool.py
--rw-r--r--   0        0        0      526 2023-04-16 15:58:58.633882 griptape_tools-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 griptape_tools-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-04-06 19:20:02.762584 griptape_tools-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1402 2023-04-13 17:49:58.210759 griptape_tools-0.6.0/README.md
+-rw-r--r--   0        0        0       65 2023-04-07 15:46:22.422848 griptape_tools-0.6.0/griptape/__init__.py
+-rw-r--r--   0        0        0      352 2023-04-13 16:07:18.435628 griptape_tools-0.6.0/griptape/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.6.0/griptape/tools/aws_cli/__init__.py
+-rw-r--r--   0        0        0      159 2023-04-13 16:14:30.544316 griptape_tools-0.6.0/griptape/tools/aws_cli/manifest.yml
+-rw-r--r--   0        0        0       78 2023-04-16 19:48:12.571528 griptape_tools-0.6.0/griptape/tools/aws_cli/requirements.txt
+-rw-r--r--   0        0        0     1447 2023-04-16 19:44:48.773728 griptape_tools-0.6.0/griptape/tools/aws_cli/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.6.0/griptape/tools/calculator/__init__.py
+-rw-r--r--   0        0        0      169 2023-04-06 19:20:02.784946 griptape_tools-0.6.0/griptape/tools/calculator/manifest.yml
+-rw-r--r--   0        0        0       21 2023-04-16 19:48:12.566517 griptape_tools-0.6.0/griptape/tools/calculator/requirements.txt
+-rw-r--r--   0        0        0      652 2023-04-16 19:44:48.772145 griptape_tools-0.6.0/griptape/tools/calculator/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.6.0/griptape/tools/email_client/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-12 21:25:06.766972 griptape_tools-0.6.0/griptape/tools/email_client/manifest.yml
+-rw-r--r--   0        0        0       21 2023-04-16 19:48:12.564602 griptape_tools-0.6.0/griptape/tools/email_client/requirements.txt
+-rw-r--r--   0        0        0     2318 2023-04-16 19:44:48.775301 griptape_tools-0.6.0/griptape/tools/email_client/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.783032 griptape_tools-0.6.0/griptape/tools/sql_client/__init__.py
+-rw-r--r--   0        0        0      154 2023-04-12 19:53:04.579660 griptape_tools-0.6.0/griptape/tools/sql_client/manifest.yml
+-rw-r--r--   0        0        0       33 2023-04-16 19:48:12.570157 griptape_tools-0.6.0/griptape/tools/sql_client/requirements.txt
+-rw-r--r--   0        0        0     1259 2023-04-16 19:44:48.779356 griptape_tools-0.6.0/griptape/tools/sql_client/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.6.0/griptape/tools/web_scraper/__init__.py
+-rw-r--r--   0        0        0      195 2023-04-11 21:24:23.634297 griptape_tools-0.6.0/griptape/tools/web_scraper/manifest.yml
+-rw-r--r--   0        0        0       53 2023-04-16 19:48:12.568056 griptape_tools-0.6.0/griptape/tools/web_scraper/requirements.txt
+-rw-r--r--   0        0        0     4420 2023-04-16 19:44:48.778162 griptape_tools-0.6.0/griptape/tools/web_scraper/tool.py
+-rw-r--r--   0        0        0        0 2023-04-06 19:20:02.786470 griptape_tools-0.6.0/griptape/tools/web_search/__init__.py
+-rw-r--r--   0        0        0      172 2023-04-08 22:17:19.115836 griptape_tools-0.6.0/griptape/tools/web_search/manifest.yml
+-rw-r--r--   0        0        0       29 2023-04-16 19:48:12.561911 griptape_tools-0.6.0/griptape/tools/web_search/requirements.txt
+-rw-r--r--   0        0        0     2272 2023-04-16 19:44:48.776769 griptape_tools-0.6.0/griptape/tools/web_search/tool.py
+-rw-r--r--   0        0        0      526 2023-04-16 19:50:14.950453 griptape_tools-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2061 1970-01-01 00:00:00.000000 griptape_tools-0.6.0/PKG-INFO
```

### Comparing `griptape_tools-0.5.3/LICENSE` & `griptape_tools-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.3/README.md` & `griptape_tools-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `griptape_tools-0.5.3/griptape/tools/aws_cli/tool.py` & `griptape_tools-0.6.0/griptape/tools/aws_cli/tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from typing import Optional
-from schema import Schema, Literal
+from schema import Schema
 from griptape.core import BaseTool, action, utils
 from attr import define, field
 
 
 @define
 class AwsCli(BaseTool):
     aws_access_key_id: Optional[str] = field(default=None, kw_only=True, metadata={"env": "AWS_ACCESS_KEY_ID"})
@@ -17,20 +17,18 @@
         return {
             "policy": json.dumps(utils.minify_json(self.env_value("AWS_CLI_POLICY"))).strip('"')
         }
 
     @action(config={
         "name": "execute",
         "description": "Can be used to execute AWS CLI v2 commands limited by this policy: {{ policy }}",
-        "value_schema": Schema({
-            Literal(
-                "value",
-                description="AWS CLI v2 command"
-            ): str
-        })
+        "schema": Schema(
+            str,
+            description="AWS CLI v2 command"
+        )
     })
     def execute(self, value: bytes) -> str:
         result = utils.CommandRunner().run(f"AWS_PAGER='' {value.decode()} --output json")
 
         if result == "":
             return "[]"
         else:
```

### Comparing `griptape_tools-0.5.3/griptape/tools/calculator/tool.py` & `griptape_tools-0.6.0/griptape/tools/calculator/tool.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from schema import Schema, Literal
 from griptape.core import BaseTool, action, utils
+from schema import Schema
 
 
 class Calculator(BaseTool):
     @action(config={
         "name": "calculate",
         "description": "Can be used for making simple calculations in Python",
-        "value_schema": Schema({
-            Literal(
-                "value",
-                description="Arithmetic expression parsable in pure Python. Single line only. Don't use any "
-                            "imports or external libraries"
-            ): str
-        })
+        "schema": Schema(
+            str,
+            description="Arithmetic expression parsable in pure Python. Single line only. Don't use any "
+                        "imports or external libraries"
+        )
     })
     def calculate(self, value: bytes) -> str:
         try:
             return utils.PythonRunner().run(value.decode())
         except Exception as e:
             return f"error calculating: {e}"
```

### Comparing `griptape_tools-0.5.3/griptape/tools/email_client/tool.py` & `griptape_tools-0.6.0/griptape/tools/email_client/tool.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,29 +15,27 @@
     password: Optional[str] = field(default=None, kw_only=True, metadata={"env": "SMTP_PASSWORD"})
     from_email: Optional[str] = field(default=None, kw_only=True, metadata={"env": "FROM_EMAIL"})
     use_ssl: bool = field(default=True, kw_only=True, metadata={"env": "SMTP_USE_SSL"})
 
     @action(config={
         "name": "send",
         "description": "Can be used to send emails",
-        "value_schema": Schema({
-            "value": {
-                Literal(
-                    "to",
-                    description="Recipient's email address"
-                ): str,
-                Literal(
-                    "subject",
-                    description="Email subject"
-                ): str,
-                Literal(
-                    "body",
-                    description="Email body"
-                ): str
-            }
+        "schema": Schema({
+            Literal(
+                "to",
+                description="Recipient's email address"
+            ): str,
+            Literal(
+                "subject",
+                description="Email subject"
+            ): str,
+            Literal(
+                "body",
+                description="Email body"
+            ): str
         })
     })
     def send(self, value: bytes) -> str:
         server: Optional[smtplib.SMTP] = None
         params = ast.literal_eval(value.decode())
         host = self.env_value("SMTP_HOST")
         port = int(self.env_value("SMTP_PORT"))
```

### Comparing `griptape_tools-0.5.3/griptape/tools/sql_client/tool.py` & `griptape_tools-0.6.0/griptape/tools/sql_client/tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional
-from schema import Schema, Literal
-from griptape.core import BaseTool, action
 from attr import define, field
+from griptape.core import BaseTool, action
+from schema import Schema
 
 
 @define
 class SqlClient(BaseTool):
     engine_url: Optional[str] = field(default=None, kw_only=True, metadata={"env": "ENGINE_URL"})
     engine_name: str = field(kw_only=True)
 
@@ -14,20 +14,18 @@
         return {
             "engine": self.engine_name
         }
 
     @action(config={
         "name": "query",
         "description": "Can be used to execute SQL queries in {{ engine }}",
-        "value_schema": Schema({
-            Literal(
-                "value",
-                description="SQL query to execute. For example, SELECT, CREATE, INSERT, DROP, DELETE, etc."
-            ): str
-        })
+        "schema": Schema(
+            str,
+            description="SQL query to execute. For example, SELECT, CREATE, INSERT, DROP, DELETE, etc."
+        )
     })
     def query(self, value: bytes) -> str:
         from sqlalchemy import create_engine, text
 
         engine = create_engine(self.env_value("ENGINE_URL"))
 
         try:
```

### Comparing `griptape_tools-0.5.3/griptape/tools/web_scraper/tool.py` & `griptape_tools-0.6.0/griptape/tools/web_scraper/tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,99 +16,87 @@
 class WebScraper(BaseTool):
     openai_api_key: Optional[str] = field(default=None, kw_only=True, metadata={"env": "OPENAI_API_KEY"})
     include_links: bool = field(default=True, kw_only=True, metadata={"env": "INCLUDE_LINKS"})
 
     @action(config={
         "name": "get_title",
         "description": "Can be used to get the title of a web page",
-        "value_schema": Schema({
-            Literal(
-                "value",
-                description="Valid HTTP URL"
-            ): str
-        })
+        "schema": Schema(
+            str,
+            description="Valid HTTP URL"
+        )
     })
     def get_title(self, value: bytes) -> str:
         return self._load_page(value.decode()).get("title")
 
     @action(config={
         "name": "get_full_page",
         "description": "Can be used to get all text content of a web page",
-        "value_schema": Schema({
-            Literal(
-                "value",
-                description="Valid HTTP URL"
-            ): str
-        })
+        "schema": Schema(
+            str,
+            description="Valid HTTP URL"
+        )
     })
     def get_full_page(self, value: bytes) -> str:
         return self._load_page(value.decode()).get("text")
 
     @action(config={
         "name": "search_page",
         "description": "Can be used to search a specific web page",
-        "value_schema": Schema({
-            "value": {
-                Literal(
-                    "url",
-                    description="Valid HTTP URL"
-                ): str,
-                Literal(
-                    "query",
-                    description="Search query"
-                ): str
-            }
+        "schema": Schema({
+            Literal(
+                "url",
+                description="Valid HTTP URL"
+            ): str,
+            Literal(
+                "query",
+                description="Search query"
+            ): str
         })
     })
     def search_page(self, value: bytes) -> str:
         params = ast.literal_eval(value.decode())
         index = self._to_vector_index(self._load_page(params["url"]).get("text"))
 
-        return str(index.query(params["query"])).strip()
+        return str(index.query(f"search the following text for '{params['query']}'")).strip()
 
     @action(config={
         "name": "get_authors",
         "description": "Can be used to get a list of web page authors",
-        "value_schema": Schema({
-            Literal(
-                "value",
-                description="Valid HTTP URL"
-            ): str
-        })
+        "schema": Schema(
+            str,
+            description="Valid HTTP URL"
+        )
     })
     def get_authors(self, value: bytes) -> list[str]:
         return [
             self._load_page(value.decode()).get("author")
         ]
 
     @action(config={
         "name": "get_keywords",
         "description": "Can be used to generate a list of keywords for a web page",
-        "value_schema": Schema({
-            Literal(
-                "value",
-                description="Valid HTTP URL"
-            ): str
-        })
+        "schema": Schema(
+            str,
+            description="Valid HTTP URL"
+        )
     })
     def get_keywords(self, value: bytes) -> list[str]:
         index = self._to_vector_index(self._load_page(value.decode()).get("text"))
         keywords = str(index.query("Generate a comma-separated list of keywords for the following text"))
 
         return [w.strip() for w in keywords.split(",")]
 
     @action(config={
         "name": "summarize_page",
         "description": "Can be used to generate a web page summary",
-        "value_schema": Schema({
-            Literal(
-                "value",
-                description="Valid HTTP URL"
-            ): str
-        })
+        "schema": Schema(
+            str,
+            description="Valid HTTP URL"
+        )
     })
     def summarize_page(self, value: bytes) -> str:
         index = self._to_vector_index(self._load_page(value.decode()).get("text"))
 
         return str(index.query("Generate a summary")).strip()
 
     def _to_vector_index(self, text: str) -> GPTSimpleVectorIndex:
```

### Comparing `griptape_tools-0.5.3/griptape/tools/web_search/tool.py` & `griptape_tools-0.6.0/griptape/tools/web_search/tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,20 +11,18 @@
     google_api_key: Optional[str] = field(default=None, kw_only=True, metadata={"env": "GOOGLE_API_KEY"})
     google_api_search_id: Optional[str] = field(default=None, kw_only=True, metadata={"env": "GOOGLE_API_SEARCH_ID"})
     google_api_country: str = field(default="us", kw_only=True, metadata={"env": "GOOGLE_API_COUNTRY"})
 
     @action(config={
         "name": "search",
         "description": "Can be used for searching the web",
-        "value_schema": Schema({
-            Literal(
-                "value",
-                description="Search engine request that returns a list of pages with titles, descriptions, and URLs"
-            ): str
-        })
+        "schema": Schema(
+            str,
+            description="Search engine request that returns a list of pages with titles, descriptions, and URLs"
+        )
     })
     def search(self, value: bytes) -> dict:
         try:
             return {
                 "results": self._search_google(value.decode())
             }
         except Exception as e:
```

### Comparing `griptape_tools-0.5.3/pyproject.toml` & `griptape_tools-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "griptape-tools"
-version = "0.5.3"
+version = "0.6.0"
 description = "Tools for the griptape-core package."
 authors = ["Griptape <hello@griptape.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/griptape-ai/griptape-tools"
 
 packages = [
     {include = "griptape"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-griptape-core = ">=0.7.2"
+griptape-core = ">=0.8.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-mock = "*"
 
 [build-system]
```

### Comparing `griptape_tools-0.5.3/PKG-INFO` & `griptape_tools-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: griptape-tools
-Version: 0.5.3
+Version: 0.6.0
 Summary: Tools for the griptape-core package.
 Home-page: https://github.com/griptape-ai/griptape-tools
 License: Apache 2.0
 Author: Griptape
 Author-email: hello@griptape.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: griptape-core (>=0.7.2)
+Requires-Dist: griptape-core (>=0.8.0)
 Project-URL: Repository, https://github.com/griptape-ai/griptape-tools
 Description-Content-Type: text/markdown
 
 # Griptape Tools
 
 [![Tests](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml/badge.svg)](https://github.com/griptape-ai/griptape-tools/actions/workflows/tests.yml)
 [![Docs](https://readthedocs.org/projects/griptape/badge/)](https://griptape.readthedocs.io)
```

