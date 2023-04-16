# Comparing `tmp/gpttui-0.1.0.tar.gz` & `tmp/gpttui-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpttui-0.1.0.tar", last modified: Tue Apr 11 01:50:29 2023, max compression
+gzip compressed data, was "gpttui-0.2.0.tar", last modified: Sun Apr 16 03:43:23 2023, max compression
```

## Comparing `gpttui-0.1.0.tar` & `gpttui-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      123 2023-04-07 23:28:42.202644 gpttui-0.1.0/.gitignore
--rw-r--r--   0        0        0      176 2023-04-11 01:50:25.100205 gpttui-0.1.0/Makefile
--rw-r--r--   0        0        0     2137 2023-04-11 01:50:25.100205 gpttui-0.1.0/README.md
--rw-r--r--   0        0        0      531 2023-04-11 01:50:25.100205 gpttui-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.1.0/src/gpttui/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.1.0/src/gpttui/database/__init__.py
--rw-r--r--   0        0        0     2937 2023-04-11 01:50:25.100205 gpttui-0.1.0/src/gpttui/database/base.py
--rw-r--r--   0        0        0     4103 2023-04-11 01:50:25.100205 gpttui-0.1.0/src/gpttui/database/sqlite.py
--rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.1.0/src/gpttui/models/__init__.py
--rw-r--r--   0        0        0     1851 2023-04-11 01:50:25.100205 gpttui-0.1.0/src/gpttui/models/base.py
--rw-r--r--   0        0        0     3191 2023-04-11 01:50:25.100205 gpttui-0.1.0/src/gpttui/models/openai.py
--rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.1.0/src/gpttui/tui/__init__.py
--rw-r--r--   0        0        0     5440 2023-04-11 01:50:25.103539 gpttui-0.1.0/src/gpttui/tui/app.py
--rw-r--r--   0        0        0     1643 2023-04-11 01:50:25.103539 gpttui-0.1.0/src/gpttui/tui/config.py
--rw-r--r--   0        0        0     2391 2023-04-11 01:50:25.103539 gpttui-0.1.0/src/gpttui/tui/front.py
--rw-r--r--   0        0        0      210 2023-04-11 01:50:25.103539 gpttui-0.1.0/src/gpttui/tui/main.py
--rwxr-xr-x   0        0        0      140 2023-04-11 01:50:25.103539 gpttui-0.1.0/test/main.sh
--rw-r--r--   0        0        0     1983 2023-04-11 01:50:25.103539 gpttui-0.1.0/test/test_db.py
--rw-r--r--   0        0        0     1582 2023-04-11 01:50:25.103539 gpttui-0.1.0/test/test_model.py
--rw-r--r--   0        0        0      431 1970-01-01 00:00:00.000000 gpttui-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      123 2023-04-07 23:28:42.202644 gpttui-0.2.0/.gitignore
+-rw-r--r--   0        0        0      176 2023-04-11 01:50:25.100205 gpttui-0.2.0/Makefile
+-rw-r--r--   0        0        0     2137 2023-04-11 01:50:25.100205 gpttui-0.2.0/README.md
+-rw-r--r--   0        0        0      531 2023-04-16 03:42:27.404389 gpttui-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.2.0/src/gpttui/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.2.0/src/gpttui/database/__init__.py
+-rw-r--r--   0        0        0     2937 2023-04-11 01:50:25.100205 gpttui-0.2.0/src/gpttui/database/base.py
+-rw-r--r--   0        0        0     4103 2023-04-11 01:50:25.100205 gpttui-0.2.0/src/gpttui/database/sqlite.py
+-rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.2.0/src/gpttui/models/__init__.py
+-rw-r--r--   0        0        0     1851 2023-04-11 01:50:25.100205 gpttui-0.2.0/src/gpttui/models/base.py
+-rw-r--r--   0        0        0     3410 2023-04-16 03:42:27.407722 gpttui-0.2.0/src/gpttui/models/openai.py
+-rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.2.0/src/gpttui/tui/__init__.py
+-rw-r--r--   0        0        0     6271 2023-04-16 03:42:27.407722 gpttui-0.2.0/src/gpttui/tui/app.py
+-rw-r--r--   0        0        0     2644 2023-04-16 03:42:27.407722 gpttui-0.2.0/src/gpttui/tui/config.py
+-rw-r--r--   0        0        0     2391 2023-04-11 01:50:25.103539 gpttui-0.2.0/src/gpttui/tui/front.py
+-rw-r--r--   0        0        0      210 2023-04-11 01:50:25.103539 gpttui-0.2.0/src/gpttui/tui/main.py
+-rwxr-xr-x   0        0        0      140 2023-04-11 01:50:25.103539 gpttui-0.2.0/test/main.sh
+-rw-r--r--   0        0        0     1983 2023-04-11 01:50:25.103539 gpttui-0.2.0/test/test_db.py
+-rw-r--r--   0        0        0     1582 2023-04-11 01:50:25.103539 gpttui-0.2.0/test/test_model.py
+-rw-r--r--   0        0        0      431 1970-01-01 00:00:00.000000 gpttui-0.2.0/PKG-INFO
```

### Comparing `gpttui-0.1.0/README.md` & `gpttui-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gpttui-0.1.0/pyproject.toml` & `gpttui-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gpttui"
-version = "0.1.0"
+version = "0.2.0"
 authors = [{name = "Juan Lara", email = "julara@unal.edu.co"}]
 description = "TUI to interact with gpt models."
 requires-python = ">3.8"
 dependencies = [
     "openai", "textual[dev]", "pydantic", "pyperclip"
 ]
```

### Comparing `gpttui-0.1.0/src/gpttui/database/base.py` & `gpttui-0.2.0/src/gpttui/database/base.py`

 * *Files identical despite different names*

### Comparing `gpttui-0.1.0/src/gpttui/database/sqlite.py` & `gpttui-0.2.0/src/gpttui/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `gpttui-0.1.0/src/gpttui/models/base.py` & `gpttui-0.2.0/src/gpttui/models/base.py`

 * *Files identical despite different names*

### Comparing `gpttui-0.1.0/src/gpttui/models/openai.py` & `gpttui-0.2.0/src/gpttui/models/openai.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 This module contains the integration with OpenAI models.
 """
 import openai, os, time
+from openai.error import Timeout
 from gpttui.models.base import AbstractModel
 from gpttui.database.base import Messages, Message, MessageWithTime
 from typing import Any
 
 class OpenAIModel(AbstractModel):
     """
     This class allows loading and interacting with any openai model through its API.
     """
+    timeout = 0
+    max_retries = 3
 
     def setup(self, **kwargs: Any) -> "OpenAIModel":
         """
         Initializes the model and collects credentials for OpenAI.
 
         Parameters
         ----------
@@ -73,26 +76,29 @@
         last_msgs = self.last_messages()
         new_msg = MessageWithTime(
                 message=Message(role="user", content=message),
                 timestamp=int(time.time())
                 )
         self.database.add_message(msg=new_msg, session_name=self.session_name)
         last_msgs = self.last_messages()
-        response = None
-        while response is None:
+        response = ""
+        retries = 0
+        while not response and retries < self.max_retries:
             try:
                 response = str(
                         openai.ChatCompletion.create(
                             model = self.model_name,
                             messages = last_msgs.dict()["values"],
-                            request_timeout = 10
+                            request_timeout = self.timeout
                             )
                         .choices[0].message.content #type: ignore
                         )
-            except:
-                response = None
+            except Timeout:
+                retries += 1
+        if retries == 3:
+            raise Timeout("Maximum number of retries achieved.")
         new_msg = MessageWithTime(
                 message=Message(role="assistant", content=response),
                 timestamp=int(time.time())
                 )
         self.database.add_message(msg=new_msg, session_name=self.session_name)
         return response
```

### Comparing `gpttui-0.1.0/src/gpttui/tui/front.py` & `gpttui-0.2.0/src/gpttui/tui/front.py`

 * *Files identical despite different names*

### Comparing `gpttui-0.1.0/test/test_db.py` & `gpttui-0.2.0/test/test_db.py`

 * *Files identical despite different names*

### Comparing `gpttui-0.1.0/test/test_model.py` & `gpttui-0.2.0/test/test_model.py`

 * *Files identical despite different names*

