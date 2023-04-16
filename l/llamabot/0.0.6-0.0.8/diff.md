# Comparing `tmp/llamabot-0.0.6.tar.gz` & `tmp/llamabot-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamabot-0.0.6.tar", last modified: Tue Apr 11 12:47:44 2023, max compression
+gzip compressed data, was "llamabot-0.0.8.tar", last modified: Sun Apr 16 18:23:47 2023, max compression
```

## Comparing `llamabot-0.0.6.tar` & `llamabot-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-11 12:47:44.620686 llamabot-0.0.6/
--rw-r--r--   0 ericmjl    (501) staff       (20)      124 2023-04-03 18:38:54.000000 llamabot-0.0.6/MANIFEST.in
--rw-r--r--   0 ericmjl    (501) staff       (20)       95 2023-04-11 12:47:44.620551 llamabot-0.0.6/PKG-INFO
--rw-r--r--   0 ericmjl    (501) staff       (20)     5647 2023-04-04 15:17:20.000000 llamabot-0.0.6/README.md
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-11 12:47:44.619249 llamabot-0.0.6/llamabot/
--rw-r--r--   0 ericmjl    (501) staff       (20)      284 2023-04-10 22:45:50.000000 llamabot-0.0.6/llamabot/__init__.py
--rw-r--r--   0 ericmjl    (501) staff       (20)     5720 2023-04-11 12:47:19.000000 llamabot-0.0.6/llamabot/bot.py
--rw-r--r--   0 ericmjl    (501) staff       (20)      652 2023-04-03 18:38:54.000000 llamabot-0.0.6/llamabot/cli.py
--rw-r--r--   0 ericmjl    (501) staff       (20)       35 2023-04-03 18:38:54.000000 llamabot-0.0.6/llamabot/preprocessing.py
--rw-r--r--   0 ericmjl    (501) staff       (20)      182 2023-04-03 18:38:54.000000 llamabot-0.0.6/llamabot/schemas.py
--rw-r--r--   0 ericmjl    (501) staff       (20)       30 2023-04-03 18:38:54.000000 llamabot-0.0.6/llamabot/utils.py
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-11 12:47:44.619998 llamabot-0.0.6/llamabot.egg-info/
--rw-r--r--   0 ericmjl    (501) staff       (20)       95 2023-04-11 12:47:44.000000 llamabot-0.0.6/llamabot.egg-info/PKG-INFO
--rw-r--r--   0 ericmjl    (501) staff       (20)      409 2023-04-11 12:47:44.000000 llamabot-0.0.6/llamabot.egg-info/SOURCES.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)        1 2023-04-11 12:47:44.000000 llamabot-0.0.6/llamabot.egg-info/dependency_links.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)       46 2023-04-11 12:47:44.000000 llamabot-0.0.6/llamabot.egg-info/entry_points.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)       90 2023-04-11 12:47:44.000000 llamabot-0.0.6/llamabot.egg-info/requires.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)        9 2023-04-11 12:47:44.000000 llamabot-0.0.6/llamabot.egg-info/top_level.txt
--rw-r--r--   0 ericmjl    (501) staff       (20)     1529 2023-04-11 12:47:41.000000 llamabot-0.0.6/pyproject.toml
--rw-r--r--   0 ericmjl    (501) staff       (20)       38 2023-04-11 12:47:44.620725 llamabot-0.0.6/setup.cfg
-drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-11 12:47:44.620379 llamabot-0.0.6/tests/
--rw-r--r--   0 ericmjl    (501) staff       (20)       26 2023-04-03 18:38:54.000000 llamabot-0.0.6/tests/test___init__.py
--rw-r--r--   0 ericmjl    (501) staff       (20)       30 2023-04-03 18:38:54.000000 llamabot-0.0.6/tests/test_cli.py
--rw-r--r--   0 ericmjl    (501) staff       (20)       52 2023-04-03 18:38:54.000000 llamabot-0.0.6/tests/test_models.py
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-16 18:23:47.719910 llamabot-0.0.8/
+-rw-r--r--   0 ericmjl    (501) staff       (20)      124 2023-04-03 18:38:54.000000 llamabot-0.0.8/MANIFEST.in
+-rw-r--r--   0 ericmjl    (501) staff       (20)       95 2023-04-16 18:23:47.719761 llamabot-0.0.8/PKG-INFO
+-rw-r--r--   0 ericmjl    (501) staff       (20)     6237 2023-04-11 12:50:37.000000 llamabot-0.0.8/README.md
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-16 18:23:47.718025 llamabot-0.0.8/llamabot/
+-rw-r--r--   0 ericmjl    (501) staff       (20)      284 2023-04-11 12:47:57.000000 llamabot-0.0.8/llamabot/__init__.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)     7436 2023-04-16 18:23:26.000000 llamabot-0.0.8/llamabot/bot.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)      652 2023-04-03 18:38:54.000000 llamabot-0.0.8/llamabot/cli.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)       35 2023-04-03 18:38:54.000000 llamabot-0.0.8/llamabot/preprocessing.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)      182 2023-04-03 18:38:54.000000 llamabot-0.0.8/llamabot/schemas.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)       30 2023-04-03 18:38:54.000000 llamabot-0.0.8/llamabot/utils.py
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-16 18:23:47.719138 llamabot-0.0.8/llamabot.egg-info/
+-rw-r--r--   0 ericmjl    (501) staff       (20)       95 2023-04-16 18:23:47.000000 llamabot-0.0.8/llamabot.egg-info/PKG-INFO
+-rw-r--r--   0 ericmjl    (501) staff       (20)      409 2023-04-16 18:23:47.000000 llamabot-0.0.8/llamabot.egg-info/SOURCES.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)        1 2023-04-16 18:23:47.000000 llamabot-0.0.8/llamabot.egg-info/dependency_links.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)       46 2023-04-16 18:23:47.000000 llamabot-0.0.8/llamabot.egg-info/entry_points.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)      102 2023-04-16 18:23:47.000000 llamabot-0.0.8/llamabot.egg-info/requires.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)        9 2023-04-16 18:23:47.000000 llamabot-0.0.8/llamabot.egg-info/top_level.txt
+-rw-r--r--   0 ericmjl    (501) staff       (20)     1549 2023-04-16 18:23:44.000000 llamabot-0.0.8/pyproject.toml
+-rw-r--r--   0 ericmjl    (501) staff       (20)       38 2023-04-16 18:23:47.719958 llamabot-0.0.8/setup.cfg
+drwxr-xr-x   0 ericmjl    (501) staff       (20)        0 2023-04-16 18:23:47.719562 llamabot-0.0.8/tests/
+-rw-r--r--   0 ericmjl    (501) staff       (20)       26 2023-04-03 18:38:54.000000 llamabot-0.0.8/tests/test___init__.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)       30 2023-04-03 18:38:54.000000 llamabot-0.0.8/tests/test_cli.py
+-rw-r--r--   0 ericmjl    (501) staff       (20)       52 2023-04-03 18:38:54.000000 llamabot-0.0.8/tests/test_models.py
```

### Comparing `llamabot-0.0.6/README.md` & `llamabot-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -70,14 +70,35 @@
 
 ```python
 feynman("Is there a simpler way to rephrase the text?")
 ```
 
 And your bot will work with the chat history to respond.
 
+### QueryBot
+
+The final bot provided is a QueryBot.
+This bot lets you query a collection of documents.
+To use it, you have two options:
+
+1. Pass in a list of paths to text files, or
+2. Pass in a pre-computed `GPTSimpleIndex` from LlamaIndex.
+
+As an illustrative example:
+
+```python
+from llamabot import QueryBot
+from pathlib import Path
+
+blog_index = Path("/path/to/index.json")
+bot = QueryBot(system_message="You are a Q&A bot.", saved_index_path=blog_index)
+result = bot("Do you have any advice for me on career development?", similarity_top_k=5)
+display(Markdown(result.response))
+```
+
 ## Contributing
 
 ### New features
 
 New features are welcome!
 These are early and exciting days for users of large language models.
 Our development goals are to keep the project as simple as possible.
```

### Comparing `llamabot-0.0.6/llamabot/cli.py` & `llamabot-0.0.8/llamabot/cli.py`

 * *Files identical despite different names*

### Comparing `llamabot-0.0.6/pyproject.toml` & `llamabot-0.0.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -57,19 +57,20 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 namespaces = false
 
 [project]
 name = "llamabot"
-version = "0.0.6"
+version = "0.0.8"
 dependencies = [
     "openai",
     "langchain",
-    "typer"
+    "typer",
+    "llama_index",
 ]
 
 [project.optional-dependencies]
 tests = [
     "pytest"
 ]
 docs = [
```

