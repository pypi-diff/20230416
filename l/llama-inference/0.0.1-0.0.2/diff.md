# Comparing `tmp/llama_inference-0.0.1.tar.gz` & `tmp/llama_inference-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_inference-0.0.1.tar", last modified: Wed Apr 12 10:17:03 2023, max compression
+gzip compressed data, was "llama_inference-0.0.2.tar", last modified: Sun Apr 16 18:57:51 2023, max compression
```

## Comparing `llama_inference-0.0.1.tar` & `llama_inference-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-12 10:17:03.734829 llama_inference-0.0.1/
--rw-r--r--   0 aniket     (501) staff       (20)     5218 2023-04-10 11:35:05.000000 llama_inference-0.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 aniket     (501) staff       (20)     3727 2023-04-10 11:35:05.000000 llama_inference-0.0.1/CONTRIBUTING.md
--rw-r--r--   0 aniket     (501) staff       (20)     1070 2023-04-10 11:47:38.000000 llama_inference-0.0.1/LICENSE
--rw-r--r--   0 aniket     (501) staff       (20)      783 2023-04-12 10:11:51.000000 llama_inference-0.0.1/MANIFEST.in
--rw-r--r--   0 aniket     (501) staff       (20)      778 2023-04-12 10:17:03.734897 llama_inference-0.0.1/PKG-INFO
--rw-r--r--   0 aniket     (501) staff       (20)      560 2023-04-12 09:22:21.000000 llama_inference-0.0.1/README.md
--rw-r--r--   0 aniket     (501) staff       (20)      374 2023-04-12 10:17:03.735165 llama_inference-0.0.1/setup.cfg
--rw-r--r--   0 aniket     (501) staff       (20)      148 2023-04-12 10:08:35.000000 llama_inference-0.0.1/setup.py
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-12 10:17:03.733489 llama_inference-0.0.1/src/
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-12 10:17:03.733939 llama_inference-0.0.1/src/llama_inference/
--rw-r--r--   0 aniket     (501) staff       (20)       88 2023-04-12 10:06:07.000000 llama_inference-0.0.1/src/llama_inference/__init__.py
--rw-r--r--   0 aniket     (501) staff       (20)      695 2023-04-12 10:06:07.000000 llama_inference-0.0.1/src/llama_inference/app.py
--rw-r--r--   0 aniket     (501) staff       (20)     4465 2023-04-12 10:06:07.000000 llama_inference-0.0.1/src/llama_inference/model.py
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-12 10:17:03.734686 llama_inference-0.0.1/src/llama_inference.egg-info/
--rw-r--r--   0 aniket     (501) staff       (20)      778 2023-04-12 10:17:03.000000 llama_inference-0.0.1/src/llama_inference.egg-info/PKG-INFO
--rw-r--r--   0 aniket     (501) staff       (20)      406 2023-04-12 10:17:03.000000 llama_inference-0.0.1/src/llama_inference.egg-info/SOURCES.txt
--rw-r--r--   0 aniket     (501) staff       (20)        1 2023-04-12 10:17:03.000000 llama_inference-0.0.1/src/llama_inference.egg-info/dependency_links.txt
--rw-r--r--   0 aniket     (501) staff       (20)       21 2023-04-12 10:17:03.000000 llama_inference-0.0.1/src/llama_inference.egg-info/requires.txt
--rw-r--r--   0 aniket     (501) staff       (20)       16 2023-04-12 10:17:03.000000 llama_inference-0.0.1/src/llama_inference.egg-info/top_level.txt
--rw-r--r--   0 aniket     (501) staff       (20)       21 2023-04-12 10:06:07.000000 llama_inference-0.0.1/src/requirements.txt
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-16 18:57:51.084137 llama_inference-0.0.2/
+-rw-r--r--   0 aniket     (501) staff       (20)     5218 2023-04-10 11:35:05.000000 llama_inference-0.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 aniket     (501) staff       (20)     3727 2023-04-10 11:35:05.000000 llama_inference-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0 aniket     (501) staff       (20)     1070 2023-04-10 11:47:38.000000 llama_inference-0.0.2/LICENSE
+-rw-r--r--   0 aniket     (501) staff       (20)      783 2023-04-12 10:11:51.000000 llama_inference-0.0.2/MANIFEST.in
+-rw-r--r--   0 aniket     (501) staff       (20)     1598 2023-04-16 18:57:51.084269 llama_inference-0.0.2/PKG-INFO
+-rw-r--r--   0 aniket     (501) staff       (20)     1243 2023-04-16 18:57:12.000000 llama_inference-0.0.2/README.md
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-16 18:57:51.077019 llama_inference-0.0.2/assets/
+-rw-r--r--   0 aniket     (501) staff       (20)   399922 2023-04-16 18:49:16.000000 llama_inference-0.0.2/assets/llama-inference-api-min.png
+-rw-r--r--   0 aniket     (501) staff       (20)      512 2023-04-16 18:57:51.084691 llama_inference-0.0.2/setup.cfg
+-rw-r--r--   0 aniket     (501) staff       (20)      148 2023-04-16 14:48:37.000000 llama_inference-0.0.2/setup.py
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-16 18:57:51.078541 llama_inference-0.0.2/src/
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-16 18:57:51.081222 llama_inference-0.0.2/src/llama_inference/
+-rw-r--r--   0 aniket     (501) staff       (20)      118 2023-04-16 18:50:14.000000 llama_inference-0.0.2/src/llama_inference/__init__.py
+-rw-r--r--   0 aniket     (501) staff       (20)     4967 2023-04-16 15:29:12.000000 llama_inference-0.0.2/src/llama_inference/model.py
+-rw-r--r--   0 aniket     (501) staff       (20)      695 2023-04-16 18:50:14.000000 llama_inference-0.0.2/src/llama_inference/serve.py
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-16 18:57:51.083617 llama_inference-0.0.2/src/llama_inference.egg-info/
+-rw-r--r--   0 aniket     (501) staff       (20)     1598 2023-04-16 18:57:51.000000 llama_inference-0.0.2/src/llama_inference.egg-info/PKG-INFO
+-rw-r--r--   0 aniket     (501) staff       (20)      443 2023-04-16 18:57:51.000000 llama_inference-0.0.2/src/llama_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 aniket     (501) staff       (20)        1 2023-04-16 18:57:51.000000 llama_inference-0.0.2/src/llama_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 aniket     (501) staff       (20)       38 2023-04-16 18:57:51.000000 llama_inference-0.0.2/src/llama_inference.egg-info/requires.txt
+-rw-r--r--   0 aniket     (501) staff       (20)       16 2023-04-16 18:57:51.000000 llama_inference-0.0.2/src/llama_inference.egg-info/top_level.txt
+-rw-r--r--   0 aniket     (501) staff       (20)       38 2023-04-16 18:55:15.000000 llama_inference-0.0.2/src/requirements.txt
```

### Comparing `llama_inference-0.0.1/CODE_OF_CONDUCT.md` & `llama_inference-0.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.1/CONTRIBUTING.md` & `llama_inference-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.1/LICENSE` & `llama_inference-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.1/MANIFEST.in` & `llama_inference-0.0.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.1/src/llama_inference/app.py` & `llama_inference-0.0.2/src/llama_inference/serve.py`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.1/src/llama_inference/model.py` & `llama_inference-0.0.2/src/llama_inference/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import sys
 import time
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Union
 
 import lightning as L
 import torch
 from dotenv import load_dotenv
 from lit_llama import LLaMA, Tokenizer
 from lit_llama.utils import EmptyInitOnDevice
 
@@ -67,22 +67,23 @@
 
     return idx
 
 
 class LLaMAInference:
     def __init__(
         self,
-        accelerator: str = "auto",
-        checkpoint_path: Optional[Path] = None,
-        tokenizer_path: Optional[Path] = None,
         model_size: str = "7B",
         dtype: Optional[str] = None,
         quantize: Optional[str] = None,
+        checkpoint_path: Optional[Path] = None,
+        tokenizer_path: Optional[Path] = None,
+        accelerator: str = "auto",
+        devices: int = 1,
     ) -> None:
-        self.fabric = fabric = L.Fabric(accelerator=accelerator, devices=1)
+        self.fabric = fabric = L.Fabric(accelerator=accelerator, devices=devices)
 
         if not checkpoint_path and WEIGHTS_PATH:
             checkpoint_path = f"{WEIGHTS_PATH}/{model_size}/state_dict.pth"
             tokenizer_path = f"{WEIGHTS_PATH}/tokenizer.model"
 
         if dtype is not None:
             dt = getattr(torch, dtype, None)
@@ -98,18 +99,21 @@
             model = LLaMA.from_name(model_size)
             checkpoint = torch.load(checkpoint_path)
             model.load_state_dict(checkpoint)
             print(
                 f"Time to load model: {time.time() - t0:.02f} seconds.", file=sys.stderr
             )
 
-        model.eval()
+        self.eval()
         self.model = fabric.setup_module(model)
         self.tokenizer = Tokenizer(tokenizer_path)
 
+    def eval(self):
+        self.model.eval()
+
     def __call__(
         self,
         prompt: str,
         max_new_tokens: int = 50,
         top_k: int = 200,
         temperature: float = 0.8,
     ) -> str:
@@ -131,7 +135,17 @@
             encoded_prompt,
             max_new_tokens,
             self.model.config.block_size,  # type: ignore[union-attr,arg-type]
             temperature=temperature,
             top_k=top_k,
         )[0]
         return self.tokenizer.decode(y)
+
+    def load_state_dict_from_path(self, checkpoint_path: Union[Path, str]):
+        checkpoints = torch.load(checkpoint_path)
+        self.model.load_state_dict(checkpoints, strict=False)
+
+    def load_lora_weights(self, checkpoint_path: str):
+        self.load_state_dict_from_path(checkpoint_path)
+
+    def load_adapters_weights(self, checkpoint_path: str):
+        self.load_state_dict_from_path(checkpoint_path)
```

