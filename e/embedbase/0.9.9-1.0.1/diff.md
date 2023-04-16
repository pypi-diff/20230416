# Comparing `tmp/embedbase-0.9.9.tar.gz` & `tmp/embedbase-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-0.9.9.tar", last modified: Mon Apr  3 16:22:07 2023, max compression
+gzip compressed data, was "embedbase-1.0.1.tar", last modified: Sun Apr 16 15:20:19 2023, max compression
```

## Comparing `embedbase-0.9.9.tar` & `embedbase-1.0.1.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:22:07.405027 embedbase-0.9.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-03 16:21:56.000000 embedbase-0.9.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-03 16:21:56.000000 embedbase-0.9.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-04-03 16:22:07.405027 embedbase-0.9.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-03 16:21:56.000000 embedbase-0.9.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:22:07.401028 embedbase-0.9.9/embedbase/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:22:07.405027 embedbase-0.9.9/embedbase/database/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/database/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/database/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/database/pinecone_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/database/postgres_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/database/supabase_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/database/weaviate_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:22:07.405027 embedbase-0.9.9/embedbase/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/embedding/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/embedding/cohere.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/embedding/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/firebase_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/strings.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/supabase_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-03 16:21:56.000000 embedbase-0.9.9/embedbase/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:22:07.401028 embedbase-0.9.9/embedbase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-04-03 16:22:07.000000 embedbase-0.9.9/embedbase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-03 16:22:07.000000 embedbase-0.9.9/embedbase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 16:22:07.000000 embedbase-0.9.9/embedbase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-03 16:22:07.000000 embedbase-0.9.9/embedbase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-03 16:22:07.000000 embedbase-0.9.9/embedbase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-03 16:21:56.000000 embedbase-0.9.9/optional-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-03 16:21:56.000000 embedbase-0.9.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 16:22:07.405027 embedbase-0.9.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-03 16:21:56.000000 embedbase-0.9.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:22:07.405027 embedbase-0.9.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 16:21:56.000000 embedbase-0.9.9/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:22:07.405027 embedbase-0.9.9/tests/database/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 16:21:56.000000 embedbase-0.9.9/tests/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-04-03 16:21:56.000000 embedbase-0.9.9/tests/database/test_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:22:07.405027 embedbase-0.9.9/tests/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 16:21:56.000000 embedbase-0.9.9/tests/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-03 16:21:56.000000 embedbase-0.9.9/tests/embedding/test_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-03 16:21:56.000000 embedbase-0.9.9/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    16985 2023-04-03 16:21:56.000000 embedbase-0.9.9/tests/test_end_to_end.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 16:21:56.000000 embedbase-0.9.9/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:20:19.915730 embedbase-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-16 15:20:05.000000 embedbase-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-16 15:20:05.000000 embedbase-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-04-16 15:20:19.915730 embedbase-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-04-16 15:20:05.000000 embedbase-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:20:19.911730 embedbase-1.0.1/embedbase/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:20:19.911730 embedbase-1.0.1/embedbase/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/database/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/database/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/database/memory_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/database/pinecone_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7938 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/database/postgres_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/database/supabase_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/database/weaviate_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:20:19.915730 embedbase-1.0.1/embedbase/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/embedding/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/embedding/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/embedding/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/firebase_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/strings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/supabase_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-16 15:20:05.000000 embedbase-1.0.1/embedbase/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:20:19.911730 embedbase-1.0.1/embedbase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-04-16 15:20:19.000000 embedbase-1.0.1/embedbase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-16 15:20:19.000000 embedbase-1.0.1/embedbase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 15:20:19.000000 embedbase-1.0.1/embedbase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-16 15:20:19.000000 embedbase-1.0.1/embedbase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-16 15:20:19.000000 embedbase-1.0.1/embedbase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-16 15:20:05.000000 embedbase-1.0.1/optional-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-16 15:20:05.000000 embedbase-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 15:20:19.915730 embedbase-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-16 15:20:05.000000 embedbase-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:20:19.915730 embedbase-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 15:20:05.000000 embedbase-1.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:20:19.915730 embedbase-1.0.1/tests/database/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 15:20:05.000000 embedbase-1.0.1/tests/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-04-16 15:20:05.000000 embedbase-1.0.1/tests/database/test_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:20:19.915730 embedbase-1.0.1/tests/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 15:20:05.000000 embedbase-1.0.1/tests/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-16 15:20:05.000000 embedbase-1.0.1/tests/embedding/test_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-16 15:20:05.000000 embedbase-1.0.1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16985 2023-04-16 15:20:05.000000 embedbase-1.0.1/tests/test_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 15:20:05.000000 embedbase-1.0.1/tests/test_utils.py
```

### Comparing `embedbase-0.9.9/LICENSE` & `embedbase-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-0.9.9/PKG-INFO` & `embedbase-1.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,68 +1,80 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 0.9.9
-Summary: An API to easily connect your data to ChatGPT
+Version: 1.0.1
+Summary: API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings
 Home-page: https://github.com/different-ai/embedbase
 Author: Different AI
 Author-email: louis@embedbase.xyz
 License: MIT
 Description: <br />
         
         
         <p align="center">
         <img width="150" alt="embedbasevector" src="https://user-images.githubusercontent.com/11430621/223136025-14572cac-f2aa-455c-936b-a48cb35a0c57.png">
           <h1 align="center">Embedbase</h1>
         
         
-        <h3 align="center">An API to easily connect your data to ChatGPT</h3>
+        <h3 align="center">The end to end platform to help you ship embeddings-powered apps.</h3>
         
           <p align="center">
             <br />
             <a href="https://discord.gg/pMNeuGrDky"><img alt="Discord" src="https://img.shields.io/discord/1066022656845025310?color=black&style=for-the-badge"></a>
             <a href="https://badge.fury.io/py/embedbase"><img alt="PyPI" src="https://img.shields.io/pypi/v/embedbase?color=black&style=for-the-badge"></a>
-            <p>Open-source sdk & api to easily connect data to ChatGPT</p>
-            <p>Used by <a href="https://github.com/louis030195/obsidian-ava">AVA</a> and serving 100k request a day</p>
-            <a href="https://app.embedbase.xyz/signup">Try the sandbox playground now</a>
-            ·
-            <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=enhancement">Request Feature</a>
-            ·
-            <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=bug">Report Bug</a>
+            <p align="center">Open-source API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings</p>
+            <p align="center">Used by <a href="https://github.com/louis030195/obsidian-ava">AVA</a> and serving 100k request a day</p>
+            <div align="center">
+              <a href="https://app.embedbase.xyz/signup">Try Embedbase Cloud now</a>
+              ·
+              <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=enhancement">Request Feature</a>
+              ·
+              <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=bug">Report Bug</a>
+            </div>
             <br />
           </p>
         </p>
         
         Check out the [docs](https://docs.embedbase.xyz) for more info.
         
         
         ## Table of Contents
         
         - [Getting started](#getting-started)
         - [Javascript SDK](#sdk)
         - [Docs and support](#docs-and-support)
         - [Contributing](#contributing)
         
+        ## The 3 ways to use Embedbase
+        
+        - [Embedbase Cloud](#managed-instance): **Build embeddings-powered apps in minutes** | `npm i embedbase-js`
+        - [Embedbase.py](#getting-started): **Choose your own db, embeddings models, and get started with a simple** | `pip install embedbase`
+        - Embedbase self-hosted: **Get Embedbase Cloud on your infra** | `docker-compose up`
+        
         ## Examples
         
         Please refer to [examples in the documentation](https://docs.embedbase.xyz/).
         
         ## What are people building
         
-        - [AVA uses Embedbase to help their users find related notes](https://github.com/louis030195/obsidian-ava)
-        - [Solpilot uses Embedbase to put smart contract integration on autopilot](https://solpilot.xyz/chat)
-        - [ChatGPT-powered search for markdown documentation](https://github.com/different-ai/chat-gpt-powered-nextra)
+        - [Creating a recommendation engine: AVA uses Embedbase to help their users find related notes](https://github.com/louis030195/obsidian-ava)
+        - [Creating chat with your data experiences: Solpilot uses Embedbase to put smart contract integration on autopilot](https://solpilot.xyz/chat)
+        - [Creating a talk with your docs experience: ChatGPT-powered search for markdown documentation](https://github.com/different-ai/chat-gpt-powered-nextra)
         
         ## Getting started
         
+        Let's install Python dependencies:
+        
         ```bash
-        # start local postgres
-        docker-compose up
+        pip install embedbase uvicorn
         ```
         
+        And write a basic boilerplate code in `main.py`:
+        
         ```py
+        import uvicorn
         from embedbase import get_app
         
         from embedbase.database.postgres_db import Postgres
         from embedbase.embedding.openai import OpenAI
          
         async def custom_middleware(request, call_next):
             # customise as you prefer :)
@@ -75,18 +87,29 @@
          
         app = (
             get_app()
             .use_middleware(custom_middleware)
             .use_embedder(OpenAI("<your key>"))
             .use_db(Postgres())
         ).run()
+        
+        if __name__ == "__main__":
+            uvicorn.run("main:app")
         ```
         
+        Let's use Postgres as a database, you can start it with Docker:
+        
+        ```bash
+        docker run -d -p 8080:8080 -p 5432:5432 -e POSTGRES_DB=embedbase -e POSTGRES_PASSWORD=localdb ankane/pgvector
         ```
-        uvicorn main:app
+        
+        Now start embedbase using the boilerplate code we just wrote in `main.py`:
+        
+        ```bash
+        python3 main.py
         ```
         
         🔥 Embedbase now runs! [Time to ship your product](#sdk)
         
         
         ### Managed Instance
```

#### html2text {}

```diff
@@ -1,54 +1,69 @@
-Metadata-Version: 2.1 Name: embedbase Version: 0.9.9 Summary: An API to easily
-connect your data to ChatGPT Home-page: https://github.com/different-ai/
-embedbase Author: Different AI Author-email: louis@embedbase.xyz License: MIT
-Description:
+Metadata-Version: 2.1 Name: embedbase Version: 1.0.1 Summary: API, SDK &
+dashboard to easily create, store, and retrieve machine learning embeddings
+Home-page: https://github.com/different-ai/embedbase Author: Different AI
+Author-email: louis@embedbase.xyz License: MIT Description:
                                [embedbasevector]
                             ****** Embedbase ******
-            **** An API to easily connect your data to ChatGPT ****
+  **** The end to end platform to help you ship embeddings-powered apps. ****
 
                                [Discord] [PyPI]
-Open-source sdk & api to easily connect data to ChatGPT
-Used by AVA and serving 100k request a day
-Try_the_sandbox_playground_now Â· Request_Feature Â· Report_Bug
+Open-source API, SDK & dashboard to easily create, store, and retrieve machine
+                              learning embeddings
+                  Used by AVA and serving 100k request a day
+           Try_Embedbase_Cloud_now Â· Request_Feature Â· Report_Bug
+
 Check out the [docs](https://docs.embedbase.xyz) for more info. ## Table of
 Contents - [Getting started](#getting-started) - [Javascript SDK](#sdk) - [Docs
-and support](#docs-and-support) - [Contributing](#contributing) ## Examples
-Please refer to [examples in the documentation](https://docs.embedbase.xyz/).
-## What are people building - [AVA uses Embedbase to help their users find
-related notes](https://github.com/louis030195/obsidian-ava) - [Solpilot uses
-Embedbase to put smart contract integration on autopilot](https://solpilot.xyz/
-chat) - [ChatGPT-powered search for markdown documentation](https://github.com/
-different-ai/chat-gpt-powered-nextra) ## Getting started ```bash # start local
-postgres docker-compose up ``` ```py from embedbase import get_app from
+and support](#docs-and-support) - [Contributing](#contributing) ## The 3 ways
+to use Embedbase - [Embedbase Cloud](#managed-instance): **Build embeddings-
+powered apps in minutes** | `npm i embedbase-js` - [Embedbase.py](#getting-
+started): **Choose your own db, embeddings models, and get started with a
+simple** | `pip install embedbase` - Embedbase self-hosted: **Get Embedbase
+Cloud on your infra** | `docker-compose up` ## Examples Please refer to
+[examples in the documentation](https://docs.embedbase.xyz/). ## What are
+people building - [Creating a recommendation engine: AVA uses Embedbase to help
+their users find related notes](https://github.com/louis030195/obsidian-ava) -
+[Creating chat with your data experiences: Solpilot uses Embedbase to put smart
+contract integration on autopilot](https://solpilot.xyz/chat) - [Creating a
+talk with your docs experience: ChatGPT-powered search for markdown
+documentation](https://github.com/different-ai/chat-gpt-powered-nextra) ##
+Getting started Let's install Python dependencies: ```bash pip install
+embedbase uvicorn ``` And write a basic boilerplate code in `main.py`: ```py
+import uvicorn from embedbase import get_app from
 embedbase.database.postgres_db import Postgres from embedbase.embedding.openai
 import OpenAI async def custom_middleware(request, call_next): # customise as
 you prefer :) start_time = time.time() response = await call_next(request)
 process_time = time.time() - start_time response.headers["X-Process-Time"] =
 str(process_time) return response app = ( get_app() .use_middleware
-(custom_middleware) .use_embedder(OpenAI("")) .use_db(Postgres()) ).run() ```
-``` uvicorn main:app ``` ð¥ Embedbase now runs! [Time to ship your product]
-(#sdk) ### Managed Instance The fastest way to get started with Embedbase is
-signing up for free to [Embedbase Cloud](https://app.embedbase.xyz/). !
-[Dashboard Screenshot](https://user-images.githubusercontent.com/11430621/
-227351386-f540fac0-c5fa-485a-bcc9-f23368fe3f63.png) ## How to use ### SDK `npm
-i embedbase-js` ```js import { createClient } from 'embedbase-js' const
-question = 'What can I do with Embedbase API?' const embedbase = createClient
-( 'https://api.embedbase.xyz', 'api-key') const context = await embedbase
-.dataset('embedbase-docs') .createContext('What can I do with Embedbase API?',
-{ limit: 3 }); console.log(context) [ "Embedbase API allows to store
-unstructured data...", "Embedbase API has 3 main functions a) provides a plug
-and play solution to store embeddings b) makes it easy to connect to get the
-right data into llms c)..", "Embedabase API is self-hostable...", ] // refer to
-https://github.com/openai/openai-node for the exact api openai.createCompletion
-( `Write a response to question: ${question} based on the follwing context $
-{context.toString()}` ) // answer: // You can use the Embedbase API to store
-unstructured data and then use the data to connect it to LLMs ``` ### Inserting
-data ```ts const URL = 'http://localhost:8000' const VAULT_ID = 'people' // if
-using the hosted version const API_KEY = '
+(custom_middleware) .use_embedder(OpenAI("")) .use_db(Postgres()) ).run() if
+__name__ == "__main__": uvicorn.run("main:app") ``` Let's use Postgres as a
+database, you can start it with Docker: ```bash docker run -d -p 8080:8080 -
+p 5432:5432 -e POSTGRES_DB=embedbase -e POSTGRES_PASSWORD=localdb ankane/
+pgvector ``` Now start embedbase using the boilerplate code we just wrote in
+`main.py`: ```bash python3 main.py ``` ð¥ Embedbase now runs! [Time to ship
+your product](#sdk) ### Managed Instance The fastest way to get started with
+Embedbase is signing up for free to [Embedbase Cloud](https://
+app.embedbase.xyz/). ![Dashboard Screenshot](https://user-
+images.githubusercontent.com/11430621/227351386-f540fac0-c5fa-485a-bcc9-
+f23368fe3f63.png) ## How to use ### SDK `npm i embedbase-js` ```js import
+{ createClient } from 'embedbase-js' const question = 'What can I do with
+Embedbase API?' const embedbase = createClient( 'https://api.embedbase.xyz',
+'api-key') const context = await embedbase .dataset('embedbase-docs')
+.createContext('What can I do with Embedbase API?', { limit: 3 }); console.log
+(context) [ "Embedbase API allows to store unstructured data...", "Embedbase
+API has 3 main functions a) provides a plug and play solution to store
+embeddings b) makes it easy to connect to get the right data into llms c)..",
+"Embedabase API is self-hostable...", ] // refer to https://github.com/openai/
+openai-node for the exact api openai.createCompletion( `Write a response to
+question: ${question} based on the follwing context ${context.toString()}` ) /
+/ answer: // You can use the Embedbase API to store unstructured data and then
+use the data to connect it to LLMs ``` ### Inserting data ```ts const URL =
+'http://localhost:8000' const VAULT_ID = 'people' // if using the hosted
+version const API_KEY = '
 app.embedbase.xyz/signup>' fetch(`${URL}/v1/${VAULT_ID}`, { method: 'POST',
 headers: { 'Content-Type': 'application/json', // if using the hosted version,
 uncomment // 'Authorization': `Bearer ${API_KEY}` }, body: JSON.stringify(
 { documents: [{ data: 'Elon is sipping a tea on Mars', }], }), }); ``` ###
 Searching ```ts fetch(`${URL}/v1/${VAULT_ID}/search`, { method: 'POST',
 headers: { 'Content-Type': 'application/json', // 'Authorization': `Bearer $
 {API_KEY}` }, body: JSON.stringify({ query: 'Something about a red planet', }),
```

### Comparing `embedbase-0.9.9/README.md` & `embedbase-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,59 +2,71 @@
 
 
 <p align="center">
 <img width="150" alt="embedbasevector" src="https://user-images.githubusercontent.com/11430621/223136025-14572cac-f2aa-455c-936b-a48cb35a0c57.png">
   <h1 align="center">Embedbase</h1>
 
 
-<h3 align="center">An API to easily connect your data to ChatGPT</h3>
+<h3 align="center">The end to end platform to help you ship embeddings-powered apps.</h3>
 
   <p align="center">
     <br />
     <a href="https://discord.gg/pMNeuGrDky"><img alt="Discord" src="https://img.shields.io/discord/1066022656845025310?color=black&style=for-the-badge"></a>
     <a href="https://badge.fury.io/py/embedbase"><img alt="PyPI" src="https://img.shields.io/pypi/v/embedbase?color=black&style=for-the-badge"></a>
-    <p>Open-source sdk & api to easily connect data to ChatGPT</p>
-    <p>Used by <a href="https://github.com/louis030195/obsidian-ava">AVA</a> and serving 100k request a day</p>
-    <a href="https://app.embedbase.xyz/signup">Try the sandbox playground now</a>
-    ·
-    <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=enhancement">Request Feature</a>
-    ·
-    <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=bug">Report Bug</a>
+    <p align="center">Open-source API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings</p>
+    <p align="center">Used by <a href="https://github.com/louis030195/obsidian-ava">AVA</a> and serving 100k request a day</p>
+    <div align="center">
+      <a href="https://app.embedbase.xyz/signup">Try Embedbase Cloud now</a>
+      ·
+      <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=enhancement">Request Feature</a>
+      ·
+      <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=bug">Report Bug</a>
+    </div>
     <br />
   </p>
 </p>
 
 Check out the [docs](https://docs.embedbase.xyz) for more info.
 
 
 ## Table of Contents
 
 - [Getting started](#getting-started)
 - [Javascript SDK](#sdk)
 - [Docs and support](#docs-and-support)
 - [Contributing](#contributing)
 
+## The 3 ways to use Embedbase
+
+- [Embedbase Cloud](#managed-instance): **Build embeddings-powered apps in minutes** | `npm i embedbase-js`
+- [Embedbase.py](#getting-started): **Choose your own db, embeddings models, and get started with a simple** | `pip install embedbase`
+- Embedbase self-hosted: **Get Embedbase Cloud on your infra** | `docker-compose up`
+
 ## Examples
 
 Please refer to [examples in the documentation](https://docs.embedbase.xyz/).
 
 ## What are people building
 
-- [AVA uses Embedbase to help their users find related notes](https://github.com/louis030195/obsidian-ava)
-- [Solpilot uses Embedbase to put smart contract integration on autopilot](https://solpilot.xyz/chat)
-- [ChatGPT-powered search for markdown documentation](https://github.com/different-ai/chat-gpt-powered-nextra)
+- [Creating a recommendation engine: AVA uses Embedbase to help their users find related notes](https://github.com/louis030195/obsidian-ava)
+- [Creating chat with your data experiences: Solpilot uses Embedbase to put smart contract integration on autopilot](https://solpilot.xyz/chat)
+- [Creating a talk with your docs experience: ChatGPT-powered search for markdown documentation](https://github.com/different-ai/chat-gpt-powered-nextra)
 
 ## Getting started
 
+Let's install Python dependencies:
+
 ```bash
-# start local postgres
-docker-compose up
+pip install embedbase uvicorn
 ```
 
+And write a basic boilerplate code in `main.py`:
+
 ```py
+import uvicorn
 from embedbase import get_app
 
 from embedbase.database.postgres_db import Postgres
 from embedbase.embedding.openai import OpenAI
  
 async def custom_middleware(request, call_next):
     # customise as you prefer :)
@@ -67,18 +79,29 @@
  
 app = (
     get_app()
     .use_middleware(custom_middleware)
     .use_embedder(OpenAI("<your key>"))
     .use_db(Postgres())
 ).run()
+
+if __name__ == "__main__":
+    uvicorn.run("main:app")
 ```
 
+Let's use Postgres as a database, you can start it with Docker:
+
+```bash
+docker run -d -p 8080:8080 -p 5432:5432 -e POSTGRES_DB=embedbase -e POSTGRES_PASSWORD=localdb ankane/pgvector
 ```
-uvicorn main:app
+
+Now start embedbase using the boilerplate code we just wrote in `main.py`:
+
+```bash
+python3 main.py
 ```
 
 🔥 Embedbase now runs! [Time to ship your product](#sdk)
 
 
 ### Managed Instance
```

### Comparing `embedbase-0.9.9/embedbase/api.py` & `embedbase-1.0.1/embedbase/api.py`

 * *Files identical despite different names*

### Comparing `embedbase-0.9.9/embedbase/app.py` & `embedbase-1.0.1/embedbase/app.py`

 * *Files identical despite different names*

### Comparing `embedbase-0.9.9/embedbase/database/base.py` & `embedbase-1.0.1/embedbase/database/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-0.9.9/embedbase/database/db_utils.py` & `embedbase-1.0.1/embedbase/database/db_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-0.9.9/embedbase/database/postgres_db.py` & `embedbase-1.0.1/embedbase/database/postgres_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-0.9.9/embedbase/database/supabase_db.py` & `embedbase-1.0.1/embedbase/database/supabase_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-0.9.9/embedbase/embedding/base.py` & `embedbase-1.0.1/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-0.9.9/embedbase/embedding/cohere.py` & `embedbase-1.0.1/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-0.9.9/embedbase/embedding/openai.py` & `embedbase-1.0.1/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-0.9.9/embedbase/firebase_auth.py` & `embedbase-1.0.1/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-0.9.9/embedbase/logging_utils.py` & `embedbase-1.0.1/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-0.9.9/embedbase/models.py` & `embedbase-1.0.1/embedbase/models.py`

 * *Files identical despite different names*

### Comparing `embedbase-0.9.9/embedbase/settings.py` & `embedbase-1.0.1/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-0.9.9/embedbase/strings.py` & `embedbase-1.0.1/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-0.9.9/embedbase/utils.py` & `embedbase-1.0.1/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-0.9.9/embedbase.egg-info/PKG-INFO` & `embedbase-1.0.1/embedbase.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,68 +1,80 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 0.9.9
-Summary: An API to easily connect your data to ChatGPT
+Version: 1.0.1
+Summary: API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings
 Home-page: https://github.com/different-ai/embedbase
 Author: Different AI
 Author-email: louis@embedbase.xyz
 License: MIT
 Description: <br />
         
         
         <p align="center">
         <img width="150" alt="embedbasevector" src="https://user-images.githubusercontent.com/11430621/223136025-14572cac-f2aa-455c-936b-a48cb35a0c57.png">
           <h1 align="center">Embedbase</h1>
         
         
-        <h3 align="center">An API to easily connect your data to ChatGPT</h3>
+        <h3 align="center">The end to end platform to help you ship embeddings-powered apps.</h3>
         
           <p align="center">
             <br />
             <a href="https://discord.gg/pMNeuGrDky"><img alt="Discord" src="https://img.shields.io/discord/1066022656845025310?color=black&style=for-the-badge"></a>
             <a href="https://badge.fury.io/py/embedbase"><img alt="PyPI" src="https://img.shields.io/pypi/v/embedbase?color=black&style=for-the-badge"></a>
-            <p>Open-source sdk & api to easily connect data to ChatGPT</p>
-            <p>Used by <a href="https://github.com/louis030195/obsidian-ava">AVA</a> and serving 100k request a day</p>
-            <a href="https://app.embedbase.xyz/signup">Try the sandbox playground now</a>
-            ·
-            <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=enhancement">Request Feature</a>
-            ·
-            <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=bug">Report Bug</a>
+            <p align="center">Open-source API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings</p>
+            <p align="center">Used by <a href="https://github.com/louis030195/obsidian-ava">AVA</a> and serving 100k request a day</p>
+            <div align="center">
+              <a href="https://app.embedbase.xyz/signup">Try Embedbase Cloud now</a>
+              ·
+              <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=enhancement">Request Feature</a>
+              ·
+              <a href="https://github.com/different-ai/embedbase/issues/new?assignees=&labels=bug">Report Bug</a>
+            </div>
             <br />
           </p>
         </p>
         
         Check out the [docs](https://docs.embedbase.xyz) for more info.
         
         
         ## Table of Contents
         
         - [Getting started](#getting-started)
         - [Javascript SDK](#sdk)
         - [Docs and support](#docs-and-support)
         - [Contributing](#contributing)
         
+        ## The 3 ways to use Embedbase
+        
+        - [Embedbase Cloud](#managed-instance): **Build embeddings-powered apps in minutes** | `npm i embedbase-js`
+        - [Embedbase.py](#getting-started): **Choose your own db, embeddings models, and get started with a simple** | `pip install embedbase`
+        - Embedbase self-hosted: **Get Embedbase Cloud on your infra** | `docker-compose up`
+        
         ## Examples
         
         Please refer to [examples in the documentation](https://docs.embedbase.xyz/).
         
         ## What are people building
         
-        - [AVA uses Embedbase to help their users find related notes](https://github.com/louis030195/obsidian-ava)
-        - [Solpilot uses Embedbase to put smart contract integration on autopilot](https://solpilot.xyz/chat)
-        - [ChatGPT-powered search for markdown documentation](https://github.com/different-ai/chat-gpt-powered-nextra)
+        - [Creating a recommendation engine: AVA uses Embedbase to help their users find related notes](https://github.com/louis030195/obsidian-ava)
+        - [Creating chat with your data experiences: Solpilot uses Embedbase to put smart contract integration on autopilot](https://solpilot.xyz/chat)
+        - [Creating a talk with your docs experience: ChatGPT-powered search for markdown documentation](https://github.com/different-ai/chat-gpt-powered-nextra)
         
         ## Getting started
         
+        Let's install Python dependencies:
+        
         ```bash
-        # start local postgres
-        docker-compose up
+        pip install embedbase uvicorn
         ```
         
+        And write a basic boilerplate code in `main.py`:
+        
         ```py
+        import uvicorn
         from embedbase import get_app
         
         from embedbase.database.postgres_db import Postgres
         from embedbase.embedding.openai import OpenAI
          
         async def custom_middleware(request, call_next):
             # customise as you prefer :)
@@ -75,18 +87,29 @@
          
         app = (
             get_app()
             .use_middleware(custom_middleware)
             .use_embedder(OpenAI("<your key>"))
             .use_db(Postgres())
         ).run()
+        
+        if __name__ == "__main__":
+            uvicorn.run("main:app")
         ```
         
+        Let's use Postgres as a database, you can start it with Docker:
+        
+        ```bash
+        docker run -d -p 8080:8080 -p 5432:5432 -e POSTGRES_DB=embedbase -e POSTGRES_PASSWORD=localdb ankane/pgvector
         ```
-        uvicorn main:app
+        
+        Now start embedbase using the boilerplate code we just wrote in `main.py`:
+        
+        ```bash
+        python3 main.py
         ```
         
         🔥 Embedbase now runs! [Time to ship your product](#sdk)
         
         
         ### Managed Instance
```

#### html2text {}

```diff
@@ -1,54 +1,69 @@
-Metadata-Version: 2.1 Name: embedbase Version: 0.9.9 Summary: An API to easily
-connect your data to ChatGPT Home-page: https://github.com/different-ai/
-embedbase Author: Different AI Author-email: louis@embedbase.xyz License: MIT
-Description:
+Metadata-Version: 2.1 Name: embedbase Version: 1.0.1 Summary: API, SDK &
+dashboard to easily create, store, and retrieve machine learning embeddings
+Home-page: https://github.com/different-ai/embedbase Author: Different AI
+Author-email: louis@embedbase.xyz License: MIT Description:
                                [embedbasevector]
                             ****** Embedbase ******
-            **** An API to easily connect your data to ChatGPT ****
+  **** The end to end platform to help you ship embeddings-powered apps. ****
 
                                [Discord] [PyPI]
-Open-source sdk & api to easily connect data to ChatGPT
-Used by AVA and serving 100k request a day
-Try_the_sandbox_playground_now Â· Request_Feature Â· Report_Bug
+Open-source API, SDK & dashboard to easily create, store, and retrieve machine
+                              learning embeddings
+                  Used by AVA and serving 100k request a day
+           Try_Embedbase_Cloud_now Â· Request_Feature Â· Report_Bug
+
 Check out the [docs](https://docs.embedbase.xyz) for more info. ## Table of
 Contents - [Getting started](#getting-started) - [Javascript SDK](#sdk) - [Docs
-and support](#docs-and-support) - [Contributing](#contributing) ## Examples
-Please refer to [examples in the documentation](https://docs.embedbase.xyz/).
-## What are people building - [AVA uses Embedbase to help their users find
-related notes](https://github.com/louis030195/obsidian-ava) - [Solpilot uses
-Embedbase to put smart contract integration on autopilot](https://solpilot.xyz/
-chat) - [ChatGPT-powered search for markdown documentation](https://github.com/
-different-ai/chat-gpt-powered-nextra) ## Getting started ```bash # start local
-postgres docker-compose up ``` ```py from embedbase import get_app from
+and support](#docs-and-support) - [Contributing](#contributing) ## The 3 ways
+to use Embedbase - [Embedbase Cloud](#managed-instance): **Build embeddings-
+powered apps in minutes** | `npm i embedbase-js` - [Embedbase.py](#getting-
+started): **Choose your own db, embeddings models, and get started with a
+simple** | `pip install embedbase` - Embedbase self-hosted: **Get Embedbase
+Cloud on your infra** | `docker-compose up` ## Examples Please refer to
+[examples in the documentation](https://docs.embedbase.xyz/). ## What are
+people building - [Creating a recommendation engine: AVA uses Embedbase to help
+their users find related notes](https://github.com/louis030195/obsidian-ava) -
+[Creating chat with your data experiences: Solpilot uses Embedbase to put smart
+contract integration on autopilot](https://solpilot.xyz/chat) - [Creating a
+talk with your docs experience: ChatGPT-powered search for markdown
+documentation](https://github.com/different-ai/chat-gpt-powered-nextra) ##
+Getting started Let's install Python dependencies: ```bash pip install
+embedbase uvicorn ``` And write a basic boilerplate code in `main.py`: ```py
+import uvicorn from embedbase import get_app from
 embedbase.database.postgres_db import Postgres from embedbase.embedding.openai
 import OpenAI async def custom_middleware(request, call_next): # customise as
 you prefer :) start_time = time.time() response = await call_next(request)
 process_time = time.time() - start_time response.headers["X-Process-Time"] =
 str(process_time) return response app = ( get_app() .use_middleware
-(custom_middleware) .use_embedder(OpenAI("")) .use_db(Postgres()) ).run() ```
-``` uvicorn main:app ``` ð¥ Embedbase now runs! [Time to ship your product]
-(#sdk) ### Managed Instance The fastest way to get started with Embedbase is
-signing up for free to [Embedbase Cloud](https://app.embedbase.xyz/). !
-[Dashboard Screenshot](https://user-images.githubusercontent.com/11430621/
-227351386-f540fac0-c5fa-485a-bcc9-f23368fe3f63.png) ## How to use ### SDK `npm
-i embedbase-js` ```js import { createClient } from 'embedbase-js' const
-question = 'What can I do with Embedbase API?' const embedbase = createClient
-( 'https://api.embedbase.xyz', 'api-key') const context = await embedbase
-.dataset('embedbase-docs') .createContext('What can I do with Embedbase API?',
-{ limit: 3 }); console.log(context) [ "Embedbase API allows to store
-unstructured data...", "Embedbase API has 3 main functions a) provides a plug
-and play solution to store embeddings b) makes it easy to connect to get the
-right data into llms c)..", "Embedabase API is self-hostable...", ] // refer to
-https://github.com/openai/openai-node for the exact api openai.createCompletion
-( `Write a response to question: ${question} based on the follwing context $
-{context.toString()}` ) // answer: // You can use the Embedbase API to store
-unstructured data and then use the data to connect it to LLMs ``` ### Inserting
-data ```ts const URL = 'http://localhost:8000' const VAULT_ID = 'people' // if
-using the hosted version const API_KEY = '
+(custom_middleware) .use_embedder(OpenAI("")) .use_db(Postgres()) ).run() if
+__name__ == "__main__": uvicorn.run("main:app") ``` Let's use Postgres as a
+database, you can start it with Docker: ```bash docker run -d -p 8080:8080 -
+p 5432:5432 -e POSTGRES_DB=embedbase -e POSTGRES_PASSWORD=localdb ankane/
+pgvector ``` Now start embedbase using the boilerplate code we just wrote in
+`main.py`: ```bash python3 main.py ``` ð¥ Embedbase now runs! [Time to ship
+your product](#sdk) ### Managed Instance The fastest way to get started with
+Embedbase is signing up for free to [Embedbase Cloud](https://
+app.embedbase.xyz/). ![Dashboard Screenshot](https://user-
+images.githubusercontent.com/11430621/227351386-f540fac0-c5fa-485a-bcc9-
+f23368fe3f63.png) ## How to use ### SDK `npm i embedbase-js` ```js import
+{ createClient } from 'embedbase-js' const question = 'What can I do with
+Embedbase API?' const embedbase = createClient( 'https://api.embedbase.xyz',
+'api-key') const context = await embedbase .dataset('embedbase-docs')
+.createContext('What can I do with Embedbase API?', { limit: 3 }); console.log
+(context) [ "Embedbase API allows to store unstructured data...", "Embedbase
+API has 3 main functions a) provides a plug and play solution to store
+embeddings b) makes it easy to connect to get the right data into llms c)..",
+"Embedabase API is self-hostable...", ] // refer to https://github.com/openai/
+openai-node for the exact api openai.createCompletion( `Write a response to
+question: ${question} based on the follwing context ${context.toString()}` ) /
+/ answer: // You can use the Embedbase API to store unstructured data and then
+use the data to connect it to LLMs ``` ### Inserting data ```ts const URL =
+'http://localhost:8000' const VAULT_ID = 'people' // if using the hosted
+version const API_KEY = '
 app.embedbase.xyz/signup>' fetch(`${URL}/v1/${VAULT_ID}`, { method: 'POST',
 headers: { 'Content-Type': 'application/json', // if using the hosted version,
 uncomment // 'Authorization': `Bearer ${API_KEY}` }, body: JSON.stringify(
 { documents: [{ data: 'Elon is sipping a tea on Mars', }], }), }); ``` ###
 Searching ```ts fetch(`${URL}/v1/${VAULT_ID}/search`, { method: 'POST',
 headers: { 'Content-Type': 'application/json', // 'Authorization': `Bearer $
 {API_KEY}` }, body: JSON.stringify({ query: 'Something about a red planet', }),
```

### Comparing `embedbase-0.9.9/embedbase.egg-info/SOURCES.txt` & `embedbase-1.0.1/embedbase.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 embedbase.egg-info/SOURCES.txt
 embedbase.egg-info/dependency_links.txt
 embedbase.egg-info/requires.txt
 embedbase.egg-info/top_level.txt
 embedbase/database/__init__.py
 embedbase/database/base.py
 embedbase/database/db_utils.py
+embedbase/database/memory_db.py
 embedbase/database/pinecone_db.py
 embedbase/database/postgres_db.py
 embedbase/database/supabase_db.py
 embedbase/database/weaviate_db.py
 embedbase/embedding/__init__.py
 embedbase/embedding/base.py
 embedbase/embedding/cohere.py
```

### Comparing `embedbase-0.9.9/setup.py` & `embedbase-1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     ]
 
 setup(
     # TODO: entrypoint?
     name="embedbase",
     packages=find_packages(),
     include_package_data=True,
-    version="0.9.9",
-    description="An API to easily connect your data to ChatGPT",
+    version="1.0.1",
+    description="API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     python_requires=">=3.8",
     author="Different AI",
     author_email="louis@embedbase.xyz",
     url="https://github.com/different-ai/embedbase",
     license="MIT",
```

### Comparing `embedbase-0.9.9/tests/database/test_db.py` & `embedbase-1.0.1/tests/database/test_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 Tests at the database abstraction level.
 """
 
 import hashlib
 from typing import List
 
+import numpy as np
 import pandas as pd
 import pytest
-import numpy as np
+
 from embedbase.database import VectorDatabase
 from embedbase.database.db_utils import batch_select
+from embedbase.database.memory_db import MemoryDatabase
 from embedbase.database.postgres_db import Postgres
-from embedbase.settings import get_settings_from_file
 from embedbase.database.supabase_db import Supabase
+from embedbase.settings import get_settings_from_file
 from tests.test_utils import unit_testing_dataset
 
 vector_databases: List[VectorDatabase] = []
 
 
 # before running any test initialize the databases
 @pytest.fixture(scope="session", autouse=True)
@@ -26,14 +28,15 @@
     vector_databases.append(Postgres())
     vector_databases.append(
         Supabase(
             url=settings.supabase_url,
             key=settings.supabase_key,
         )
     )
+    vector_databases.append(MemoryDatabase())
 
 
 @pytest.mark.asyncio
 async def test_search():
     d = [
         "Bob is a human",
         "The quick brown fox jumps over the lazy dog",
```

### Comparing `embedbase-0.9.9/tests/embedding/test_embeddings.py` & `embedbase-1.0.1/tests/embedding/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `embedbase-0.9.9/tests/test_auth.py` & `embedbase-1.0.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-0.9.9/tests/test_end_to_end.py` & `embedbase-1.0.1/tests/test_end_to_end.py`

 * *Files identical despite different names*

