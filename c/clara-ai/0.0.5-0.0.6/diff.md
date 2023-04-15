# Comparing `tmp/clara_ai-0.0.5.tar.gz` & `tmp/clara_ai-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clara_ai-0.0.5.tar", max compression
+gzip compressed data, was "clara_ai-0.0.6.tar", max compression
```

## Comparing `clara_ai-0.0.5.tar` & `clara_ai-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1534 2023-04-15 21:29:03.406781 clara_ai-0.0.5/LICENSE
--rw-r--r--   0        0        0     3036 2023-04-15 21:29:03.410781 clara_ai-0.0.5/README.md
--rw-r--r--   0        0        0     2283 2023-04-15 21:29:03.410781 clara_ai-0.0.5/clara/chat.py
--rw-r--r--   0        0        0     6035 2023-04-15 21:29:03.410781 clara_ai-0.0.5/clara/cli.py
--rw-r--r--   0        0        0      369 2023-04-15 21:29:03.410781 clara_ai-0.0.5/clara/config.py
--rw-r--r--   0        0        0       54 2023-04-15 21:29:03.410781 clara_ai-0.0.5/clara/console.py
--rw-r--r--   0        0        0     3593 2023-04-15 21:29:03.410781 clara_ai-0.0.5/clara/consts.py
--rw-r--r--   0        0        0     5351 2023-04-15 21:29:03.410781 clara_ai-0.0.5/clara/index.py
--rw-r--r--   0        0        0      703 2023-04-15 21:29:03.410781 clara_ai-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3808 1970-01-01 00:00:00.000000 clara_ai-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1534 2023-04-15 22:28:20.086655 clara_ai-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3116 2023-04-15 22:28:20.086655 clara_ai-0.0.6/README.md
+-rw-r--r--   0        0        0     2283 2023-04-15 22:28:20.086655 clara_ai-0.0.6/clara/chat.py
+-rw-r--r--   0        0        0     6035 2023-04-15 22:28:20.086655 clara_ai-0.0.6/clara/cli.py
+-rw-r--r--   0        0        0      460 2023-04-15 22:28:20.086655 clara_ai-0.0.6/clara/config.py
+-rw-r--r--   0        0        0       54 2023-04-15 22:28:20.086655 clara_ai-0.0.6/clara/console.py
+-rw-r--r--   0        0        0     3593 2023-04-15 22:28:20.086655 clara_ai-0.0.6/clara/consts.py
+-rw-r--r--   0        0        0     5205 2023-04-15 22:28:20.086655 clara_ai-0.0.6/clara/index.py
+-rw-r--r--   0        0        0      703 2023-04-15 22:28:20.090655 clara_ai-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3888 1970-01-01 00:00:00.000000 clara_ai-0.0.6/PKG-INFO
```

### Comparing `clara_ai-0.0.5/LICENSE` & `clara_ai-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clara_ai-0.0.5/README.md` & `clara_ai-0.0.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -79,19 +79,23 @@
 /help    -- show this message
 ```
 
 ## Configuration
 
 Run `poetry run clara config` to know from where the program is going to read the configuration. Usually this path is going to be `/.config/clara/clara.yaml`.
 
-For now, there is only one parameter to change. This is a sample configuration:
+For now, there is only a couple of parameters. This is a sample configuration with the default values:
 
 ```
 llm:
   model: gpt-3.5-turbo
+index:
+  # similarity or mmr
+  search: similarity
+  k: 5
 ```
 
 Change the model for `gpt-4` if you have access to it.
 
 ## Cache
 
 Vector DB and chat history are stored in a cache directory, per code directory. Use `poetry run clara config` to know the path to this directory.
```

### Comparing `clara_ai-0.0.5/clara/chat.py` & `clara_ai-0.0.6/clara/chat.py`

 * *Files identical despite different names*

### Comparing `clara_ai-0.0.5/clara/cli.py` & `clara_ai-0.0.6/clara/cli.py`

 * *Files identical despite different names*

### Comparing `clara_ai-0.0.5/clara/consts.py` & `clara_ai-0.0.6/clara/consts.py`

 * *Files identical despite different names*

### Comparing `clara_ai-0.0.5/clara/index.py` & `clara_ai-0.0.6/clara/index.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from langchain.schema import Document
 
 from .consts import (
     WILDCARDS,
     BASE_PERSIST_PATH,
     PROMPT_PREFIX,
 )
+from .config import config
 from .chat import create_chat
 from .console import console
 
 
 @dataclass
 class QueryResult:
     question: str
@@ -99,15 +100,17 @@
 
         documents = []
         for file_path in get_files_by_wildcards(self.path, WILDCARDS):
             console.log(f"Loading [blue underline]{file_path}", "…")
             loader = TextLoader(file_path, encoding="utf-8")
             documents.extend(loader.load_and_split())
 
-        text_splitter = CharacterTextSplitter(chunk_size=1000, chunk_overlap=100)
+        text_splitter = CharacterTextSplitter.from_tiktoken_encoder(
+            chunk_size=1000, chunk_overlap=100
+        )
         return text_splitter.split_documents(documents)
 
     def ingest(self):
         if not self.in_memory:
             if os.path.exists(self.persist_path):
                 vectorstore = Chroma(
                     persist_directory=self.persist_path,
@@ -132,26 +135,22 @@
             self.index.vectorstore.persist()
 
     def clean(self):
         if not self.in_memory:
             shutil.rmtree(self.persist_path)
 
     def init_chat(self):
-        # model = self.get_model()
-        # self.chat = ConversationalRetrievalChain.from_llm(
-        #     model,
-        #     retriever=self.index.vectorstore.as_retriever(),
-        #     return_source_documents=True,
-        #     condense_question_prompt=CONDENSE_QUESTION_PROMPT,
-        # )
-
-        self.chat = create_chat(self.index.vectorstore.as_retriever())
+        self.chat = create_chat(
+            self.index.vectorstore.as_retriever(
+                search_type=config["index"]["search_type"],
+                search_kwargs={"k": config["index"]["k"]},
+            )
+        )
 
     def query_with_sources(self, query: str) -> QueryResult:
-        # return QueryResult(**self.index.query_with_sources(query))
         if self.chat is None:
             self.init_chat()
         response = self.chat(
             {"question": query, "chat_history": self.chat_history.history}
             # {"question": query, "chat_history": ""}
         )
         # console.log(response)
```

### Comparing `clara_ai-0.0.5/pyproject.toml` & `clara_ai-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clara-ai"
-version = "0.0.5"
+version = "0.0.6"
 description = "CLARA: Code Language Assistant & Repository Analyzer"
 authors = ["Cristóbal Carnero Liñán <cristobal@seednapse.ai>"]
 readme = "README.md"
 packages = [{include = "clara"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `clara_ai-0.0.5/PKG-INFO` & `clara_ai-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clara-ai
-Version: 0.0.5
+Version: 0.0.6
 Summary: CLARA: Code Language Assistant & Repository Analyzer
 Author: Cristóbal Carnero Liñán
 Author-email: cristobal@seednapse.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -100,19 +100,23 @@
 /help    -- show this message
 ```
 
 ## Configuration
 
 Run `poetry run clara config` to know from where the program is going to read the configuration. Usually this path is going to be `/.config/clara/clara.yaml`.
 
-For now, there is only one parameter to change. This is a sample configuration:
+For now, there is only a couple of parameters. This is a sample configuration with the default values:
 
 ```
 llm:
   model: gpt-3.5-turbo
+index:
+  # similarity or mmr
+  search: similarity
+  k: 5
 ```
 
 Change the model for `gpt-4` if you have access to it.
 
 ## Cache
 
 Vector DB and chat history are stored in a cache directory, per code directory. Use `poetry run clara config` to know the path to this directory.
```

