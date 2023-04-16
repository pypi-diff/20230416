# Comparing `tmp/llama_api_server-0.2.1.tar.gz` & `tmp/llama_api_server-0.2.2.tar.gz`

## Comparing `llama_api_server-0.2.1.tar` & `llama_api_server-0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/.gitattributes
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/Makefile
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/SECURITY.md
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/requirements.txt
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/version.txt
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/.github/dependabot.yml
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/.github/workflows/release.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/llama_api_server/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/llama_api_server/__main__.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/llama_api_server/app.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/llama_api_server/config.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/llama_api_server/model_pool.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/llama_api_server/utils.py
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/llama_api_server/models/llama_cpp.py
--rw-r--r--   0        0        0     2861 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/llama_api_server/models/pyllama.py
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/llama_api_server/models/pyllama_quant.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/LICENSE
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/README.md
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 llama_api_server-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/.gitattributes
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/Makefile
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/SECURITY.md
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/requirements.txt
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/version.txt
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/llama_api_server/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/llama_api_server/__main__.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/llama_api_server/app.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/llama_api_server/config.py
+-rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/llama_api_server/model_pool.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/llama_api_server/utils.py
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/llama_api_server/models/llama_cpp.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/llama_api_server/models/pyllama.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/llama_api_server/models/pyllama_quant.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3580 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/README.md
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 llama_api_server-0.2.2/PKG-INFO
```

### Comparing `llama_api_server-0.2.1/SECURITY.md` & `llama_api_server-0.2.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.1/requirements.txt` & `llama_api_server-0.2.2/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 fairscale==0.4.13
 filelock==3.11.0
 fire==0.5.0
 Flask==2.2.3
 hiq-python==1.1.11
 huggingface-hub==0.13.3
 idna==3.4
-importlib-metadata==6.1.0
+importlib-metadata==6.3.0
 itsdangerous==2.1.2
 Jinja2==3.1.2
 llamacpp==0.1.13
 markdown-it-py==2.2.0
 MarkupSafe==2.1.2
 mdurl==0.1.2
 mpmath==1.3.0
```

### Comparing `llama_api_server-0.2.1/.github/FUNDING.yml` & `llama_api_server-0.2.2/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.1/.github/ISSUE_TEMPLATE/bug_report.md` & `llama_api_server-0.2.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.1/.github/ISSUE_TEMPLATE/feature_request.md` & `llama_api_server-0.2.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.1/.github/workflows/release.yml` & `llama_api_server-0.2.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.1/llama_api_server/app.py` & `llama_api_server-0.2.2/llama_api_server/app.py`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.1/llama_api_server/model_pool.py` & `llama_api_server-0.2.2/llama_api_server/model_pool.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 import datetime
 from collections import defaultdict
 from functools import cache
 from threading import Lock
 from llama_api_server.models.llama_cpp import LlamaCppCompletion, LlamaCppEmbedding
-from llama_api_server.models.pyllama import PyLlamaCompletion
-from llama_api_server.models.pyllama_quant import PyLlamaQuantCompletion
+from llama_api_server.models.pyllama import PyLlama
+from llama_api_server.models.pyllama_quant import PyLlamaQuant
 from .config import get_config
 
 # Eventhrough python is not good at multi-threading, but must work is done by backend,
 # support multi thread with flask threaded mode may be a good idea.
 
 
 _pool = defaultdict(lambda: defaultdict(list))
 _pool_count = defaultdict(lambda: defaultdict(int))
 _lock = Lock()
 
 MODEL_TYPE_MAPPING = {
-    "embeddings": {"llama_cpp": LlamaCppEmbedding},
+    "embeddings": {
+        "llama_cpp": LlamaCppEmbedding,
+        "pyllama": PyLlama,
+        "pyllama_quant": PyLlamaQuant,
+    },
     "completions": {
         "llama_cpp": LlamaCppCompletion,
-        "pyllama": PyLlamaCompletion,
-        "pyllama_quant": PyLlamaQuantCompletion,
+        "pyllama": PyLlama,
+        "pyllama_quant": PyLlamaQuant,
     },
 }
 
 
 class _ModelInPool:
     def __init__(self, model, kind, name):
         self._model = model
```

### Comparing `llama_api_server-0.2.1/llama_api_server/models/llama_cpp.py` & `llama_api_server-0.2.2/llama_api_server/models/llama_cpp.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,16 @@
         temp = args["temperature"]
         echo = args["echo"]
         max_tokens = args["max_tokens"]
         suffix = args["suffix"]
         repeat_penalty = 1.3
 
         prompt = args["prompt"]
+        if isinstanceof(prompt, list):
+            prompt = prompt[0]
         prompt_tokens = self.model.str_to_token(prompt, True).tolist()
         n_past = _eval_token(
             self.model, prompt_tokens[:-1], 0, self.n_batch, self.n_thread
         )
 
         result = prompt if echo else ""
         token = prompt_tokens[-1]
@@ -89,36 +91,33 @@
         model_path = params["path"]
         self.model = _create_llama_model(model_path, True)
         self.n_batch = params.get("n_batch", None) or 2
         self.n_thread = params.get("n_thread", None) or 4
 
     def embeddings(self, args):
         inputs = args["input"]
-        if inputs is str:
+        if isinstance(inputs, str):
             inputs = [inputs]
-            is_array = False
-        else:
-            is_array = True
         embeds = []
 
         for i in inputs:
             prompt_tokens = self.model.str_to_token(i, True)
             n_past = _eval_token(
                 self.model, prompt_tokens, 0, self.n_batch, self.n_thread
             )
 
             embed = unpack_cfloat_array(self.model.get_embeddings())
             embeds.append(embed)
 
-        if not is_array:
+        if len(embeds) == 1:
             embeds = embeds[0]
 
         c_prompt_tokens = len(prompt_tokens)
         return {
             "object": "list",
-            "data": [{"object": "embedding", "embedding": embed, "index": 0}],
+            "data": [{"object": "embedding", "embedding": embeds, "index": 0}],
             "model": args["model"],
             "usage": {
                 "prompt_tokens": c_prompt_tokens,
                 "total_tokens": c_prompt_tokens,
             },
         }
```

### Comparing `llama_api_server-0.2.1/llama_api_server/models/pyllama.py` & `llama_api_server-0.2.2/llama_api_server/models/pyllama.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import json
 from pathlib import Path
 from llama_api_server.utils import get_uuid, get_timestamp
 
 
-class PyLlamaCompletion:
+class PyLlama:
     def __init__(self, params):
         try:
             import llama
             import torch
         except ImportError:
             raise ImportError(
                 'To run model with pyllama, please run "python -m pip install pyllama transformers" first'
@@ -35,23 +35,25 @@
             max_seq_len=max_seq_len, max_batch_size=max_batch_size, **params
         )
         tokenizer = llama.Tokenizer(model_path=tokenizer_path)
         model_args.vocab_size = tokenizer.n_words
         if device.startswith("cuda"):
             torch.set_default_tensor_type(torch.cuda.HalfTensor)
         else:
-            os.environ['KV_CAHCHE_IN_GPU'] = "0"
+            os.environ["KV_CAHCHE_IN_GPU"] = "0"
             torch.set_default_tensor_type(torch.FloatTensor)
         model = llama.Transformer(model_args)
         torch.set_default_tensor_type(torch.FloatTensor)
         model.load_state_dict(checkpoint, strict=False)
         self.model = llama.LLaMA(model, tokenizer)
 
     def completions(self, args):
         prompt = args["prompt"]
+        if isinstanceof(prompt, list):
+            prompt = prompt[0]
         top_p = args["top_p"]
         suffix = args["suffix"]
         echo = args["echo"]
         temp = args["temperature"]
         max_tokens = args["max_tokens"]
         result = self.model.generate(
             [prompt], max_gen_len=max_tokens, temperature=temp, top_p=top_p
@@ -74,8 +76,36 @@
             "usage": {
                 "prompt_tokens": c_prompt_tokens,
                 "completion_tokens": n_past - c_prompt_tokens,
                 "total_tokens": n_past,
             },
         }
 
+    def embeddings(self, args):
+        import torch
 
+        inputs = args["input"]
+        if isinstance(inputs, str):
+            inputs = [inputs]
+
+        input_ids = self.tokenizer.encode(inputs, return_tensors="pt").to(self.dev)
+
+        with torch.no_grad():
+            hidden_states = self.model(
+                input_ids, output_hidden_states=True
+            ).hidden_states
+            # [0] for embedding layers
+            embeds = torch.squeeze(torch.mean(hidden_states[0], 1), 1).tolist()
+
+        if len(embeds) == 1:
+            embeds = embeds[0]
+
+        c_prompt_tokens = sum([len(i) for i in input_ids])
+        return {
+            "object": "list",
+            "data": [{"object": "embedding", "embedding": embeds, "index": 0}],
+            "model": args["model"],
+            "usage": {
+                "prompt_tokens": c_prompt_tokens,
+                "total_tokens": c_prompt_tokens,
+            },
+        }
```

### Comparing `llama_api_server-0.2.1/llama_api_server/models/pyllama_quant.py` & `llama_api_server-0.2.2/llama_api_server/models/pyllama_quant.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from pathlib import Path
 from llama_api_server.utils import get_uuid, get_timestamp
 
 
-class PyLlamaQuantCompletion:
+class PyLlamaQuant:
     def __init__(self, params):
         try:
             import llama
             import torch
             from llama.hf import LLaMATokenizer
             from llama.hf.utils import get_llama
             from llama.llama_quant import load_quant
@@ -27,14 +27,16 @@
         self.model.to(self.dev)
         self.tokenizer = LLaMATokenizer.from_pretrained(model_name)
 
     def completions(self, args):
         import torch
 
         prompt = args["prompt"]
+        if isinstanceof(prompt, list):
+            prompt = prompt[0]
         top_p = args["top_p"]
         suffix = args["suffix"]
         echo = args["echo"]
         temp = args["temperature"]
         max_tokens = args["max_tokens"]
 
         input_ids = self.tokenizer.encode(prompt, return_tensors="pt").to(self.dev)
@@ -67,7 +69,37 @@
             ],
             "usage": {
                 "prompt_tokens": c_prompt_tokens,
                 "completion_tokens": c_completion_tokens,
                 "total_tokens": c_prompt_tokens + c_completion_tokens,
             },
         }
+
+    def embeddings(self, args):
+        import torch
+
+        inputs = args["input"]
+        if isinstance(inputs, str):
+            inputs = [inputs]
+
+        input_ids = self.tokenizer.encode(inputs, return_tensors="pt").to(self.dev)
+
+        with torch.no_grad():
+            hidden_states = self.model(
+                input_ids, output_hidden_states=True
+            ).hidden_states
+            # [0] for embedding layers
+            embeds = torch.squeeze(torch.mean(hidden_states[0], 1), 1).tolist()
+
+        if len(embeds) == 1:
+            embeds = embeds[0]
+
+        c_prompt_tokens = sum([len(i) for i in input_ids])
+        return {
+            "object": "list",
+            "data": [{"object": "embedding", "embedding": embeds, "index": 0}],
+            "model": args["model"],
+            "usage": {
+                "prompt_tokens": c_prompt_tokens,
+                "total_tokens": c_prompt_tokens,
+            },
+        }
```

### Comparing `llama_api_server-0.2.1/.gitignore` & `llama_api_server-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.1/LICENSE` & `llama_api_server-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_api_server-0.2.1/README.md` & `llama_api_server-0.2.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 🎭🦙 llama-api-server
 =======
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Release](https://github.com/iaalm/llama-api-server/actions/workflows/release.yml/badge.svg)](https://github.com/iaalm/llama-api-server/actions/workflows/release.yml)
+[![PyPI version](https://badge.fury.io/py/llama-api-server.svg)](https://badge.fury.io/py/llama-api-server)
 
 This project is under active deployment. Breaking changes could be made any time.
 
 Llama as a Service! This project try to build a REST-ful API server compatible to OpenAI API using open source backends like llama.
 
 # 🚀Get started
 
@@ -16,14 +17,15 @@
 If you you don't have quantized llama.cpp, you need to follow [instruction](https://github.com/ggerganov/llama.cpp#usage) to prepare model.
 
 ### pyllama
 If you you don't have quantize pyllama, you need to follow [instruction](https://github.com/juncongmoo/pyllama#-quantize-llama-to-run-in-a-4gb-gpu) to prepare model.
 
 
 ## Install
+Use following script to download package from [PyPI](https://pypi.org/project/llama-api-server) and generates model config file `config.yml` and security token file `tokens.txt`.
 ```
 pip install llama-api-server
 
 # to run wth pyllama
 pip install llama-api-server[pyllama]
 
 echo > config.yml << EOF
@@ -39,17 +41,22 @@
         path: /absolute/path/to/your/pyllama-7B4b.pt
     text-davinci-003:
       type: pyllama
       params:
         ckpt_dir: /absolute/path/to/your/7B/
         tokenizer_path: /absolute/path/to/your/tokenizer.model
       # keep to 1 instance to speed up loading of model
+  embeddings:
+    text-embedding-davinci-002:
+      type: pyllama_quant
+      params:
+        path: /absolute/path/to/your/pyllama-7B4b.pt
       min_instance: 1
       max_instance: 1
-  embeddings:
+      idle_timeout: 3600
     text-embedding-ada-002:
       type: llama_cpp
       params:
         path: /absolute/path/to/your/7B/ggml-model-q4_0.bin
 EOF
 
 echo "SOME_TOKEN" > tokens.txt
```

### Comparing `llama_api_server-0.2.1/pyproject.toml` & `llama_api_server-0.2.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "llama_api_server"
-version = "0.2.1"
-description = ""
+version = "0.2.2"
+description = "A OpenAI API compatible REST server for llama."
 authors = [
     {name = "iaalm", email= "iaalmsimon@gmail.com"}
 ]
 license = {text = "MIT"}
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `llama_api_server-0.2.1/PKG-INFO` & `llama_api_server-0.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: llama_api_server
-Version: 0.2.1
+Version: 0.2.2
+Summary: A OpenAI API compatible REST server for llama.
 Project-URL: homepage, https://github.com/iaalm/llama-api-server
 Project-URL: repository, https://github.com/iaalm/llama-api-server
 Author-email: iaalm <iaalmsimon@gmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -25,14 +26,15 @@
 Description-Content-Type: text/markdown
 
 🎭🦙 llama-api-server
 =======
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Release](https://github.com/iaalm/llama-api-server/actions/workflows/release.yml/badge.svg)](https://github.com/iaalm/llama-api-server/actions/workflows/release.yml)
+[![PyPI version](https://badge.fury.io/py/llama-api-server.svg)](https://badge.fury.io/py/llama-api-server)
 
 This project is under active deployment. Breaking changes could be made any time.
 
 Llama as a Service! This project try to build a REST-ful API server compatible to OpenAI API using open source backends like llama.
 
 # 🚀Get started
 
@@ -42,14 +44,15 @@
 If you you don't have quantized llama.cpp, you need to follow [instruction](https://github.com/ggerganov/llama.cpp#usage) to prepare model.
 
 ### pyllama
 If you you don't have quantize pyllama, you need to follow [instruction](https://github.com/juncongmoo/pyllama#-quantize-llama-to-run-in-a-4gb-gpu) to prepare model.
 
 
 ## Install
+Use following script to download package from [PyPI](https://pypi.org/project/llama-api-server) and generates model config file `config.yml` and security token file `tokens.txt`.
 ```
 pip install llama-api-server
 
 # to run wth pyllama
 pip install llama-api-server[pyllama]
 
 echo > config.yml << EOF
@@ -65,17 +68,22 @@
         path: /absolute/path/to/your/pyllama-7B4b.pt
     text-davinci-003:
       type: pyllama
       params:
         ckpt_dir: /absolute/path/to/your/7B/
         tokenizer_path: /absolute/path/to/your/tokenizer.model
       # keep to 1 instance to speed up loading of model
+  embeddings:
+    text-embedding-davinci-002:
+      type: pyllama_quant
+      params:
+        path: /absolute/path/to/your/pyllama-7B4b.pt
       min_instance: 1
       max_instance: 1
-  embeddings:
+      idle_timeout: 3600
     text-embedding-ada-002:
       type: llama_cpp
       params:
         path: /absolute/path/to/your/7B/ggml-model-q4_0.bin
 EOF
 
 echo "SOME_TOKEN" > tokens.txt
```

