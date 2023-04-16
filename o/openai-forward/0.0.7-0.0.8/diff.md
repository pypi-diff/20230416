# Comparing `tmp/openai_forward-0.0.7.tar.gz` & `tmp/openai_forward-0.0.8.tar.gz`

## Comparing `openai_forward-0.0.7.tar` & `openai_forward-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openai_forward-0.0.7/openai_forward/__init__.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 openai_forward-0.0.7/openai_forward/__main__.py
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 openai_forward-0.0.7/openai_forward/_base.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 openai_forward-0.0.7/openai_forward/app.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 openai_forward-0.0.7/openai_forward/config.py
--rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 openai_forward-0.0.7/openai_forward/openai.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.0.7/openai_forward/routers/__init__.py
--rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 openai_forward-0.0.7/openai_forward/routers/openai_v1.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 openai_forward-0.0.7/openai_forward/routers/schemas.py
--rw-r--r--   0        0        0    84661 2020-02-02 00:00:00.000000 openai_forward-0.0.7/openai_forward/web/index.js
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 openai_forward-0.0.7/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.0.7/LICENSE
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 openai_forward-0.0.7/README.md
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 openai_forward-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 openai_forward-0.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 openai_forward-0.0.8/openai_forward/__init__.py
+-rwxr-xr-x   0        0        0      626 2020-02-02 00:00:00.000000 openai_forward-0.0.8/openai_forward/__main__.py
+-rwxr-xr-x   0        0        0     5713 2020-02-02 00:00:00.000000 openai_forward-0.0.8/openai_forward/_base.py
+-rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 openai_forward-0.0.8/openai_forward/app.py
+-rwxr-xr-x   0        0        0     1167 2020-02-02 00:00:00.000000 openai_forward-0.0.8/openai_forward/config.py
+-rwxr-xr-x   0        0        0      490 2020-02-02 00:00:00.000000 openai_forward-0.0.8/openai_forward/openai.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.0.8/openai_forward/routers/__init__.py
+-rwxr-xr-x   0        0        0      490 2020-02-02 00:00:00.000000 openai_forward-0.0.8/openai_forward/routers/openai_v1.py
+-rwxr-xr-x   0        0        0     2316 2020-02-02 00:00:00.000000 openai_forward-0.0.8/openai_forward/routers/schemas.py
+-rwxr-xr-x   0        0        0    40662 2020-02-02 00:00:00.000000 openai_forward-0.0.8/openai_forward/web/index.js
+-rwxr-xr-x   0        0        0     1876 2020-02-02 00:00:00.000000 openai_forward-0.0.8/.gitignore
+-rwxr-xr-x   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.0.8/LICENSE
+-rwxr-xr-x   0        0        0     3079 2020-02-02 00:00:00.000000 openai_forward-0.0.8/README.md
+-rwxr-xr-x   0        0        0     1553 2020-02-02 00:00:00.000000 openai_forward-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4260 2020-02-02 00:00:00.000000 openai_forward-0.0.8/PKG-INFO
```

### Comparing `openai_forward-0.0.7/openai_forward/config.py` & `openai_forward-0.0.8/openai_forward/config.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.0.7/openai_forward/routers/schemas.py` & `openai_forward-0.0.8/openai_forward/routers/schemas.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.0.7/.gitignore` & `openai_forward-0.0.8/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 .idea/
 .vscode/
 third-party/
+run.sh
+ssl/
+chat.yaml
+chat_*.yaml
 
 tests/
 Log/
 dist/
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
```

### Comparing `openai_forward-0.0.7/LICENSE` & `openai_forward-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_forward-0.0.7/pyproject.toml` & `openai_forward-0.0.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -6,51 +6,57 @@
 name = "openai_forward"
 description = ""
 authors = [
     { name = "kunyuan", email = "beidongjiedeguang@gmail.com" },
 ]
 requires-python = ">=3.6"
 readme = "README.md"
-keywords = ["openai", "chatgpt", "forward", "chatbot",]
+keywords = ["openai", "chatgpt", "api forward", "chatbot", "streaming-api", "fastapi", "openai-proxy"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3"
 ]
 
 dependencies = [
     "loguru",
-    "sparrow-python",
+    "sparrow-python>=0.1.1",
     "fastapi",
     "uvicorn",
     "orjson",
     "python-dotenv",
+    "httpx",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/beidongjiedeguang/openai-forward"
-Documentation = "https://github.com/beidongjiedeguang/openai-forward#openai-forwarding-agent"
+Documentation = "https://github.com/beidongjiedeguang/openai-forward#openai-forward"
 Issues = "https://github.com/beidongjiedeguang/openai-forward/issues"
 Source = "https://github.com/beidongjiedeguang/openai-forward"
 
 [project.optional-dependencies]
+ssl = [
+    "certbot"
+]
 chatgpt = [
     "revChatGPT",
 ]
 bard = [
     "GoogleBard",
 ]
 edge = [
     "EdgeGPT",
 ]
 
 [project.scripts]
 openai_forward = "openai_forward.__main__:main"
+openai-forward = "openai_forward.__main__:main"
+aifwd = "openai_forward.__main__:main"
 
 [tool.hatch.version]
 path = "openai_forward/__init__.py"
 
 [tool.isort]
 profile = "black"
```

