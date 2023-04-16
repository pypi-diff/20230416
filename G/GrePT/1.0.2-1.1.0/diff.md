# Comparing `tmp/GrePT-1.0.2.tar.gz` & `tmp/GrePT-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GrePT-1.0.2.tar", last modified: Wed Mar 22 13:54:20 2023, max compression
+gzip compressed data, was "GrePT-1.1.0.tar", last modified: Sun Apr 16 10:09:12 2023, max compression
```

## Comparing `GrePT-1.0.2.tar` & `GrePT-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 jbarry    (1000) jbarry    (1000)        0 2023-03-22 13:54:20.829051 GrePT-1.0.2/
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)     1067 2023-03-22 12:52:59.000000 GrePT-1.0.2/LICENSE.md
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)       40 2023-03-22 13:38:22.000000 GrePT-1.0.2/MANIFEST.in
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)     1237 2023-03-22 13:54:20.829051 GrePT-1.0.2/PKG-INFO
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)      938 2023-03-22 13:46:39.000000 GrePT-1.0.2/README.md
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)      923 2023-03-22 13:52:44.000000 GrePT-1.0.2/pyproject.toml
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)       38 2023-03-22 13:54:20.829051 GrePT-1.0.2/setup.cfg
-drwxr-xr-x   0 jbarry    (1000) jbarry    (1000)        0 2023-03-22 13:54:20.818218 GrePT-1.0.2/src/
-drwxr-xr-x   0 jbarry    (1000) jbarry    (1000)        0 2023-03-22 13:54:20.818218 GrePT-1.0.2/src/GrePT.egg-info/
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)     1237 2023-03-22 13:54:20.000000 GrePT-1.0.2/src/GrePT.egg-info/PKG-INFO
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)      336 2023-03-22 13:54:20.000000 GrePT-1.0.2/src/GrePT.egg-info/SOURCES.txt
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)        1 2023-03-22 13:54:20.000000 GrePT-1.0.2/src/GrePT.egg-info/dependency_links.txt
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)       46 2023-03-22 13:54:20.000000 GrePT-1.0.2/src/GrePT.egg-info/entry_points.txt
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)       32 2023-03-22 13:54:20.000000 GrePT-1.0.2/src/GrePT.egg-info/requires.txt
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)        6 2023-03-22 13:54:20.000000 GrePT-1.0.2/src/GrePT.egg-info/top_level.txt
-drwxr-xr-x   0 jbarry    (1000) jbarry    (1000)        0 2023-03-22 13:54:20.829051 GrePT-1.0.2/src/grept/
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)       21 2023-03-22 13:52:44.000000 GrePT-1.0.2/src/grept/__init__.py
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)     5672 2023-03-22 13:07:33.000000 GrePT-1.0.2/src/grept/__main__.py
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)     3201 2023-03-22 13:28:40.000000 GrePT-1.0.2/src/grept/completions.py
--rw-r--r--   0 jbarry    (1000) jbarry    (1000)      121 2023-03-22 13:13:07.000000 GrePT-1.0.2/src/grept/config.py
+drwxr-xr-x   0 jbarry    (1000) jbarry    (1000)        0 2023-04-16 10:09:12.843706 GrePT-1.1.0/
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)     1067 2023-03-22 12:52:59.000000 GrePT-1.1.0/LICENSE.md
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)       40 2023-03-22 13:38:22.000000 GrePT-1.1.0/MANIFEST.in
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)     1237 2023-04-16 10:09:12.843706 GrePT-1.1.0/PKG-INFO
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)      938 2023-04-06 12:22:25.000000 GrePT-1.1.0/README.md
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)      982 2023-04-16 10:06:25.000000 GrePT-1.1.0/pyproject.toml
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)       38 2023-04-16 10:09:12.843706 GrePT-1.1.0/setup.cfg
+drwxr-xr-x   0 jbarry    (1000) jbarry    (1000)        0 2023-04-16 10:09:12.833706 GrePT-1.1.0/src/
+drwxr-xr-x   0 jbarry    (1000) jbarry    (1000)        0 2023-04-16 10:09:12.843706 GrePT-1.1.0/src/GrePT.egg-info/
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)     1237 2023-04-16 10:09:12.000000 GrePT-1.1.0/src/GrePT.egg-info/PKG-INFO
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)      359 2023-04-16 10:09:12.000000 GrePT-1.1.0/src/GrePT.egg-info/SOURCES.txt
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)        1 2023-04-16 10:09:12.000000 GrePT-1.1.0/src/GrePT.egg-info/dependency_links.txt
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)       46 2023-04-16 10:09:12.000000 GrePT-1.1.0/src/GrePT.egg-info/entry_points.txt
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)       32 2023-04-16 10:09:12.000000 GrePT-1.1.0/src/GrePT.egg-info/requires.txt
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)        6 2023-04-16 10:09:12.000000 GrePT-1.1.0/src/GrePT.egg-info/top_level.txt
+drwxr-xr-x   0 jbarry    (1000) jbarry    (1000)        0 2023-04-16 10:09:12.843706 GrePT-1.1.0/src/grept/
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)       21 2023-04-16 10:06:25.000000 GrePT-1.1.0/src/grept/__init__.py
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)     6174 2023-04-16 10:06:25.000000 GrePT-1.1.0/src/grept/__main__.py
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)     3409 2023-04-07 14:24:03.000000 GrePT-1.1.0/src/grept/completions.py
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)      121 2023-04-07 17:22:47.000000 GrePT-1.1.0/src/grept/config.py
+-rw-r--r--   0 jbarry    (1000) jbarry    (1000)     1058 2023-04-07 14:03:27.000000 GrePT-1.1.0/src/grept/tokenizer.py
```

### Comparing `GrePT-1.0.2/LICENSE.md` & `GrePT-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `GrePT-1.0.2/PKG-INFO` & `GrePT-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GrePT
-Version: 1.0.2
+Version: 1.1.0
 Summary: Talk to your code
 Author-email: Jack Barry <jack.barry@live.com>
 Project-URL: Homepage, https://github.com/jackbarry24/GrePT
 Keywords: GPT,OpenAI,GPT-3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `GrePT-1.0.2/README.md` & `GrePT-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `GrePT-1.0.2/pyproject.toml` & `GrePT-1.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=59.6.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "GrePT"
-version = "1.0.2"
+version = "1.1.0"
 description = "Talk to your code"
 readme = "README.md"
 authors = [{name = "Jack Barry", email = "jack.barry@live.com"}]
 license = { file = "LICENSE" }
 classifiers = []
 keywords = ["GPT", "OpenAI", "GPT-3"]
 dependencies = [
@@ -20,15 +20,15 @@
 [project.urls]
 Homepage = "https://github.com/jackbarry24/GrePT"
 
 [project.scripts]
 grept = "grept.__main__:main"
 
 [tool.bumpver]
-current_version = "1.0.2"
+current_version = "1.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
@@ -37,7 +37,10 @@
     'version = "{version}"',
 ]
 
 "src/grept/__init__.py" = [
     '__version__ = "{version}"',
 ]
 
+"src/grept/__main__.py" = [
+    'VERSION = "{version}"',
+]
```

### Comparing `GrePT-1.0.2/src/GrePT.egg-info/PKG-INFO` & `GrePT-1.1.0/src/GrePT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GrePT
-Version: 1.0.2
+Version: 1.1.0
 Summary: Talk to your code
 Author-email: Jack Barry <jack.barry@live.com>
 Project-URL: Homepage, https://github.com/jackbarry24/GrePT
 Keywords: GPT,OpenAI,GPT-3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `GrePT-1.0.2/src/grept/__main__.py` & `GrePT-1.1.0/src/grept/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 import argparse
 from termcolor import colored, cprint
 from grept import completions
 import sys
 
+VERSION = "1.1.0"
+
 def _clear():
     os.system("cls" if os.name == "nt" else "clear")
 
 def _crawl(paths: list[str], level: int, suffix: list[str], ignore: list[str]) -> set[str]:
     """Crawl through a list of files and folders
 
     Args:
@@ -69,15 +71,15 @@
 
     Args:
         messages (list[dict]): message history
         fname (str): file to query
         query (str, optional): query to ask. Defaults to None.
     """   
     file_messages = completions._generate_file_messages(file_set)
-    print("Type 'exit' or 'quit' to exit and 'clear' to clear chat history") 
+    print("'exit' or 'quit' to exit, 'clear' to clear chat history, 'refresh' to reload files") 
     # if the user uses -i and -q, the -q query will be asked first in interactive mode
     if query:
         response, messages = completions.answer(file_messages, messages, query, tokens)
         print("> " + query)
         print(colored("> " + response, "light_blue"))
 
     while True:
@@ -86,45 +88,57 @@
             if query.lower() in ["exit", "quit"]:
                 break
             if query.lower() == "clear":
                 messages = []
                 _clear()
                 print(colored("> Chat history cleared", "green"))
                 continue
+            if query.lower() == "refresh":
+                messages = []
+                file_messages = completions._generate_file_messages(file_set)
+                for file in file_set:
+                    print(colored(f"Parsing file {file} ...", "green"))
+                continue
             if query == "":
                 continue
             response, messages = completions.answer(file_messages, messages, query, tokens)
             response = response.replace("\n", "\n> ")
         except KeyboardInterrupt:
             print()
             return
 
 def main():
     parser = argparse.ArgumentParser(description="Ask questions about your code")
 
-    parser.add_argument("files", nargs="+", help="list of files and folders to crawl through")
+    parser.add_argument("files", nargs="*", default=["./"], help="list of files and folders to crawl through")
 
     mode_group = parser.add_argument_group()
     mode_group.add_argument("-q", "--query", type=str, help="input a query in the command")
     mode_group.add_argument("-i", "--interactive", action="store_true", help="start interactive mode")
     
     parser.add_argument("-l", "--level", type=int, default=1, help="set the level of recursion for crawling (default: 1)")
     parser.add_argument("-x", "--suffix", nargs="+", help="filter files by suffix")
     parser.add_argument("-t", "--tokens", type=int, default=250, help="set the maximum number of tokens (default: 250)")
 
+    parser.add_argument("-v", "--version", action="store_true", help="dump version to stdout")
+    
     args = parser.parse_args()
 
+    if args.version:
+        print(VERSION)
+        sys.exit(0)
+
     if args.level < 1: 
         print(colored("Error: level must be greater than 0", "red"), file=sys.stderr)
         sys.exit(1)
 
     if not args.files:
         print(colored("Error: no files specified", "red"), file=sys.stderr)
         sys.exit(1)
-    
+
     if not args.query and not args.interactive:
         print(colored("Error: no query specified", "red"), file=sys.stderr)
         sys.exit(1)
 
     ignore = []
     try:
         with open(".greptignore", "r") as f:
@@ -146,8 +160,8 @@
         file_messages = completions._generate_file_messages(file_set)
         response, messages = completions.answer(file_messages, [], args.query, args.tokens)
 
             
 if __name__ == "__main__":
     main()
 
-       
+
```

### Comparing `GrePT-1.0.2/src/grept/completions.py` & `GrePT-1.1.0/src/grept/completions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 import openai
 import os
 from termcolor import colored, cprint
 import time
-# import PyPDF2
-# import tiktoken
-from grept import config
-
+from grept import config, tokenizer
 
 
 def _generate_file_messages(file_set: set[str]) -> list[dict]:
     """Generates dictionary of file messages
 
     Args:
         file_set (set[str]): list of files to query
 
     Returns:
         list[dict]: formatted file messages
     """    
+
+    TOKSPLIT_BUF = 10
     file_messages = []
     for fname in file_set:
         try:
             with open(fname, "r") as f:
                 try:
                     lines = f.readlines()
                 except:
                     print(colored(f"> Error: Could not read file: {fname}", "red"))
                     continue
         except:
             continue
         code = "".join([line for line in lines if line.strip() != ""])
-        code_prompt = "File Name: " + fname + "\n" + code
-        code_message = {"role": "system", "content": code_prompt}
-        file_messages.append(code_message)
+        code_chunks = tokenizer.toksplit(code, config.MAX_INPUT_TOKENS[config.COMPLETIONS_MODEL] - TOKSPLIT_BUF)
+        for index, chunk in enumerate(code_chunks):
+            code_prompt = f"File Name: {fname}, Chunk: {index+1}/{len(code_chunks)}\n{chunk}"
+            code_message = {"role": "system", "content": code_prompt}
+            file_messages.append(code_message)
     return file_messages
 
 
 def answer(file_messages: list[str], messages: list[dict], query: str, tokens: int) -> tuple[str, list[dict]]:
     """Generates response from file set, message history, and query
 
     Args:
```

