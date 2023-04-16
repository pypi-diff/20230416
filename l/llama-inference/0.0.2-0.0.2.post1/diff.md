# Comparing `tmp/llama_inference-0.0.2.tar.gz` & `tmp/llama_inference-0.0.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_inference-0.0.2.tar", last modified: Sun Apr 16 18:57:51 2023, max compression
+gzip compressed data, was "llama_inference-0.0.2.post1.tar", last modified: Sun Apr 16 21:02:24 2023, max compression
```

## Comparing `llama_inference-0.0.2.tar` & `llama_inference-0.0.2.post1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-16 18:57:51.084137 llama_inference-0.0.2/
--rw-r--r--   0 aniket     (501) staff       (20)     5218 2023-04-10 11:35:05.000000 llama_inference-0.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 aniket     (501) staff       (20)     3727 2023-04-10 11:35:05.000000 llama_inference-0.0.2/CONTRIBUTING.md
--rw-r--r--   0 aniket     (501) staff       (20)     1070 2023-04-10 11:47:38.000000 llama_inference-0.0.2/LICENSE
--rw-r--r--   0 aniket     (501) staff       (20)      783 2023-04-12 10:11:51.000000 llama_inference-0.0.2/MANIFEST.in
--rw-r--r--   0 aniket     (501) staff       (20)     1598 2023-04-16 18:57:51.084269 llama_inference-0.0.2/PKG-INFO
--rw-r--r--   0 aniket     (501) staff       (20)     1243 2023-04-16 18:57:12.000000 llama_inference-0.0.2/README.md
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-16 18:57:51.077019 llama_inference-0.0.2/assets/
--rw-r--r--   0 aniket     (501) staff       (20)   399922 2023-04-16 18:49:16.000000 llama_inference-0.0.2/assets/llama-inference-api-min.png
--rw-r--r--   0 aniket     (501) staff       (20)      512 2023-04-16 18:57:51.084691 llama_inference-0.0.2/setup.cfg
--rw-r--r--   0 aniket     (501) staff       (20)      148 2023-04-16 14:48:37.000000 llama_inference-0.0.2/setup.py
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-16 18:57:51.078541 llama_inference-0.0.2/src/
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-16 18:57:51.081222 llama_inference-0.0.2/src/llama_inference/
--rw-r--r--   0 aniket     (501) staff       (20)      118 2023-04-16 18:50:14.000000 llama_inference-0.0.2/src/llama_inference/__init__.py
--rw-r--r--   0 aniket     (501) staff       (20)     4967 2023-04-16 15:29:12.000000 llama_inference-0.0.2/src/llama_inference/model.py
--rw-r--r--   0 aniket     (501) staff       (20)      695 2023-04-16 18:50:14.000000 llama_inference-0.0.2/src/llama_inference/serve.py
-drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-16 18:57:51.083617 llama_inference-0.0.2/src/llama_inference.egg-info/
--rw-r--r--   0 aniket     (501) staff       (20)     1598 2023-04-16 18:57:51.000000 llama_inference-0.0.2/src/llama_inference.egg-info/PKG-INFO
--rw-r--r--   0 aniket     (501) staff       (20)      443 2023-04-16 18:57:51.000000 llama_inference-0.0.2/src/llama_inference.egg-info/SOURCES.txt
--rw-r--r--   0 aniket     (501) staff       (20)        1 2023-04-16 18:57:51.000000 llama_inference-0.0.2/src/llama_inference.egg-info/dependency_links.txt
--rw-r--r--   0 aniket     (501) staff       (20)       38 2023-04-16 18:57:51.000000 llama_inference-0.0.2/src/llama_inference.egg-info/requires.txt
--rw-r--r--   0 aniket     (501) staff       (20)       16 2023-04-16 18:57:51.000000 llama_inference-0.0.2/src/llama_inference.egg-info/top_level.txt
--rw-r--r--   0 aniket     (501) staff       (20)       38 2023-04-16 18:55:15.000000 llama_inference-0.0.2/src/requirements.txt
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-16 21:02:24.021332 llama_inference-0.0.2.post1/
+-rw-r--r--   0 aniket     (501) staff       (20)     5218 2023-04-10 11:35:05.000000 llama_inference-0.0.2.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 aniket     (501) staff       (20)     3727 2023-04-10 11:35:05.000000 llama_inference-0.0.2.post1/CONTRIBUTING.md
+-rw-r--r--   0 aniket     (501) staff       (20)     1070 2023-04-10 11:47:38.000000 llama_inference-0.0.2.post1/LICENSE
+-rw-r--r--   0 aniket     (501) staff       (20)      783 2023-04-16 21:01:31.000000 llama_inference-0.0.2.post1/MANIFEST.in
+-rw-r--r--   0 aniket     (501) staff       (20)     1604 2023-04-16 21:02:24.021457 llama_inference-0.0.2.post1/PKG-INFO
+-rw-r--r--   0 aniket     (501) staff       (20)     1243 2023-04-16 21:01:31.000000 llama_inference-0.0.2.post1/README.md
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-16 21:02:24.017386 llama_inference-0.0.2.post1/assets/
+-rw-r--r--   0 aniket     (501) staff       (20)   399922 2023-04-16 18:49:16.000000 llama_inference-0.0.2.post1/assets/llama-inference-api-min.png
+-rw-r--r--   0 aniket     (501) staff       (20)      512 2023-04-16 21:02:24.021903 llama_inference-0.0.2.post1/setup.cfg
+-rw-r--r--   0 aniket     (501) staff       (20)      148 2023-04-16 21:01:31.000000 llama_inference-0.0.2.post1/setup.py
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-16 21:02:24.019164 llama_inference-0.0.2.post1/src/
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-16 21:02:24.019899 llama_inference-0.0.2.post1/src/llama_inference/
+-rw-r--r--   0 aniket     (501) staff       (20)      123 2023-04-16 21:01:53.000000 llama_inference-0.0.2.post1/src/llama_inference/__init__.py
+-rw-r--r--   0 aniket     (501) staff       (20)     4968 2023-04-16 21:01:50.000000 llama_inference-0.0.2.post1/src/llama_inference/model.py
+-rw-r--r--   0 aniket     (501) staff       (20)      695 2023-04-16 21:01:31.000000 llama_inference-0.0.2.post1/src/llama_inference/serve.py
+drwxr-xr-x   0 aniket     (501) staff       (20)        0 2023-04-16 21:02:24.021127 llama_inference-0.0.2.post1/src/llama_inference.egg-info/
+-rw-r--r--   0 aniket     (501) staff       (20)     1604 2023-04-16 21:02:24.000000 llama_inference-0.0.2.post1/src/llama_inference.egg-info/PKG-INFO
+-rw-r--r--   0 aniket     (501) staff       (20)      443 2023-04-16 21:02:24.000000 llama_inference-0.0.2.post1/src/llama_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 aniket     (501) staff       (20)        1 2023-04-16 21:02:24.000000 llama_inference-0.0.2.post1/src/llama_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 aniket     (501) staff       (20)       38 2023-04-16 21:02:24.000000 llama_inference-0.0.2.post1/src/llama_inference.egg-info/requires.txt
+-rw-r--r--   0 aniket     (501) staff       (20)       16 2023-04-16 21:02:24.000000 llama_inference-0.0.2.post1/src/llama_inference.egg-info/top_level.txt
+-rw-r--r--   0 aniket     (501) staff       (20)       38 2023-04-16 21:01:31.000000 llama_inference-0.0.2.post1/src/requirements.txt
```

### Comparing `llama_inference-0.0.2/CODE_OF_CONDUCT.md` & `llama_inference-0.0.2.post1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.2/CONTRIBUTING.md` & `llama_inference-0.0.2.post1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.2/LICENSE` & `llama_inference-0.0.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.2/MANIFEST.in` & `llama_inference-0.0.2.post1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.2/PKG-INFO` & `llama_inference-0.0.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama_inference
-Version: 0.0.2
+Version: 0.0.2.post1
 Summary: Inference API for LLaMA
 Home-page: https://github.com/aniketmaurya/LLaMA-inference-api
 Author: Aniket Maurya
 Author-email: theaniketmaurya@gmail.com
 License: Apache License 2.0
 Keywords: LLM,LLaMA,GPT
 Requires-Python: >=3.8
```

### Comparing `llama_inference-0.0.2/README.md` & `llama_inference-0.0.2.post1/README.md`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.2/assets/llama-inference-api-min.png` & `llama_inference-0.0.2.post1/assets/llama-inference-api-min.png`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.2/setup.cfg` & `llama_inference-0.0.2.post1/setup.cfg`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.2/src/llama_inference/model.py` & `llama_inference-0.0.2.post1/src/llama_inference/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
             model = LLaMA.from_name(model_size)
             checkpoint = torch.load(checkpoint_path)
             model.load_state_dict(checkpoint)
             print(
                 f"Time to load model: {time.time() - t0:.02f} seconds.", file=sys.stderr
             )
 
-        self.eval()
+        model.eval()
         self.model = fabric.setup_module(model)
         self.tokenizer = Tokenizer(tokenizer_path)
 
     def eval(self):
         self.model.eval()
 
     def __call__(
```

### Comparing `llama_inference-0.0.2/src/llama_inference/serve.py` & `llama_inference-0.0.2.post1/src/llama_inference/serve.py`

 * *Files identical despite different names*

### Comparing `llama_inference-0.0.2/src/llama_inference.egg-info/PKG-INFO` & `llama_inference-0.0.2.post1/src/llama_inference.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-inference
-Version: 0.0.2
+Version: 0.0.2.post1
 Summary: Inference API for LLaMA
 Home-page: https://github.com/aniketmaurya/LLaMA-inference-api
 Author: Aniket Maurya
 Author-email: theaniketmaurya@gmail.com
 License: Apache License 2.0
 Keywords: LLM,LLaMA,GPT
 Requires-Python: >=3.8
```

