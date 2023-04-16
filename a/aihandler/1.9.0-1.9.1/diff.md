# Comparing `tmp/aihandler-1.9.0.tar.gz` & `tmp/aihandler-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aihandler-1.9.0.tar", last modified: Fri Apr 14 21:01:51 2023, max compression
+gzip compressed data, was "aihandler-1.9.1.tar", last modified: Sun Apr 16 05:11:29 2023, max compression
```

## Comparing `aihandler-1.9.0.tar` & `aihandler-1.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:01:51.278233 aihandler-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 21:01:41.000000 aihandler-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-14 21:01:51.278233 aihandler-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-14 21:01:41.000000 aihandler-1.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 21:01:51.278233 aihandler-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-14 21:01:41.000000 aihandler-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:01:51.274233 aihandler-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:01:51.278233 aihandler-1.9.0/src/aihandler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/controlnet_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/llmrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/offline_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/pyqt_offline_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/qtvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    50075 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/settings_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/socket_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-14 21:01:41.000000 aihandler-1.9.0/src/aihandler/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:01:51.278233 aihandler-1.9.0/src/aihandler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-14 21:01:51.000000 aihandler-1.9.0/src/aihandler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-14 21:01:51.000000 aihandler-1.9.0/src/aihandler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:01:51.000000 aihandler-1.9.0/src/aihandler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-14 21:01:51.000000 aihandler-1.9.0/src/aihandler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 21:01:51.000000 aihandler-1.9.0/src/aihandler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:11:29.350751 aihandler-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 05:11:18.000000 aihandler-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-16 05:11:29.350751 aihandler-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-04-16 05:11:18.000000 aihandler-1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 05:11:29.350751 aihandler-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-16 05:11:18.000000 aihandler-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:11:29.350751 aihandler-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:11:29.350751 aihandler-1.9.1/src/aihandler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 05:11:18.000000 aihandler-1.9.1/src/aihandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-04-16 05:11:18.000000 aihandler-1.9.1/src/aihandler/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-16 05:11:18.000000 aihandler-1.9.1/src/aihandler/controlnet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-04-16 05:11:18.000000 aihandler-1.9.1/src/aihandler/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-16 05:11:18.000000 aihandler-1.9.1/src/aihandler/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9663 2023-04-16 05:11:18.000000 aihandler-1.9.1/src/aihandler/llmrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-16 05:11:18.000000 aihandler-1.9.1/src/aihandler/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-04-16 05:11:18.000000 aihandler-1.9.1/src/aihandler/offline_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-04-16 05:11:18.000000 aihandler-1.9.1/src/aihandler/pyqt_offline_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-04-16 05:11:18.000000 aihandler-1.9.1/src/aihandler/qtvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53730 2023-04-16 05:11:18.000000 aihandler-1.9.1/src/aihandler/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-04-16 05:11:18.000000 aihandler-1.9.1/src/aihandler/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-16 05:11:18.000000 aihandler-1.9.1/src/aihandler/settings_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-16 05:11:18.000000 aihandler-1.9.1/src/aihandler/socket_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-04-16 05:11:18.000000 aihandler-1.9.1/src/aihandler/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 05:11:29.350751 aihandler-1.9.1/src/aihandler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-16 05:11:29.000000 aihandler-1.9.1/src/aihandler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-16 05:11:29.000000 aihandler-1.9.1/src/aihandler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 05:11:29.000000 aihandler-1.9.1/src/aihandler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-16 05:11:29.000000 aihandler-1.9.1/src/aihandler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-16 05:11:29.000000 aihandler-1.9.1/src/aihandler.egg-info/top_level.txt
```

### Comparing `aihandler-1.9.0/LICENSE` & `aihandler-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.0/PKG-INFO` & `aihandler-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aihandler
-Version: 1.9.0
+Version: 1.9.1
 Summary: AI Handler: An engine which wraps certain huggingface models
 Home-page: https://github.com/Capsize-Games/aihandler
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `aihandler-1.9.0/README.md` & `aihandler-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.0/setup.py` & `aihandler-1.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import os
 import sys
 import platform
 from setuptools import setup, find_packages
 
 
 install_requires = [
-    "torch==2.0.0",
-    "torchvision==0.15.1",
-    "torchaudio==2.0.1",
+    # "torch==2.0.0",
+    # "torchvision==0.15.1",
+    # "torchaudio==2.0.1",
+    # "bitsandbytes==0.38.0",
     "einops==0.6.0",
     "ninja==1.11.1",
     "JIT==0.2.7",
     "triton==2.0.0",
     "tqdm==4.65.0",
     "xformers==0.0.18",
-    "bitsandbytes==0.37.0",
     "omegaconf==2.3.0",
     "accelerate==0.18.0",
     "controlnet_aux==0.0.1",
     "huggingface-hub==0.13.3",
     "numpy==1.23.5",
     "Pillow==9.4.0",
     "pip==23.0.1",
@@ -40,20 +40,22 @@
     "setuptools==65.5.1",
     "sympy==1.11.1",
     "typing_extensions==4.5.0",
     "urllib3==1.26.15",
     "diffusers==0.15.0",
     "transformers==4.27.4",
     "compel==1.1.3",
+    "sympy==1.11.1",
+    "regex",
 ]
 
 
 setup(
     name="aihandler",
-    version="1.9.0",
+    version="1.9.1",
     author="Capsize LLC",
     description="AI Handler: An engine which wraps certain huggingface models",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="ai, chatbot, chat, ai",
     license="AGPL-3.0",
     author_email="contact@capsize.gg",
```

### Comparing `aihandler-1.9.0/src/aihandler/base_runner.py` & `aihandler-1.9.1/src/aihandler/base_runner.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.0/src/aihandler/controlnet_utils.py` & `aihandler-1.9.1/src/aihandler/controlnet_utils.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.0/src/aihandler/database.py` & `aihandler-1.9.1/src/aihandler/database.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.0/src/aihandler/llmrunner.py` & `aihandler-1.9.1/src/aihandler/llmrunner.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.0/src/aihandler/logger.py` & `aihandler-1.9.1/src/aihandler/logger.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.0/src/aihandler/offline_client.py` & `aihandler-1.9.1/src/aihandler/offline_client.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.0/src/aihandler/pyqt_offline_client.py` & `aihandler-1.9.1/src/aihandler/pyqt_offline_client.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.0/src/aihandler/qtvar.py` & `aihandler-1.9.1/src/aihandler/qtvar.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.0/src/aihandler/runner.py` & `aihandler-1.9.1/src/aihandler/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,17 +39,30 @@
     prompt: str = ""
     negative_prompt: str = ""
     guidance_scale: float = 7.5
     image_guidance_scale: float = 1.5
     num_inference_steps: int = 20
     height: int = 512
     width: int = 512
+    steps: int = 20
+    ddim_eta: float = 0.5
     C: int = 4
     f: int = 8
-    batch_size = 1
+    batch_size: int = 1
+    n_samples: int = 1
+    pos_x: int = 0
+    pos_y: int = 0
+    outpaint_box_rect = None
+    hf_token: str = ""
+    enable_model_cpu_offload: bool = False
+    use_attention_slicing: bool = False
+    use_tf32: bool = False
+    use_cudnn_benchmark: bool = False
+    use_enable_vae_slicing: bool = False
+    use_xformers: bool = False
     reload_model: bool = False
     action: str = ""
     options: dict = {}
     model = None
     do_cancel = False
     schedulers: dict = {
         "Euler": "EulerDiscreteScheduler",
@@ -478,23 +491,24 @@
             "DPM++ multistep": "dpm++",
             "DPM++ singlestep": "dpmss++",
             "DPM2 k": "dpm2k",
             "DPM2 a k": "dpm2ak",
             "DEIS": "deis",
         }
         from diffusers.pipelines.stable_diffusion.convert_from_ckpt import \
-            load_pipeline_from_original_stable_diffusion_ckpt
+            download_from_original_stable_diffusion_ckpt
         logger.debug(f"Loading ckpt file, is safetensors {self.is_safetensors}")
         try:
-            pipeline = load_pipeline_from_original_stable_diffusion_ckpt(
+            pipeline = download_from_original_stable_diffusion_ckpt(
                 checkpoint_path=self.model,
                 original_config_file={"v1": "v1.yaml", "v2": "v2.yaml"},
                 scheduler_type=schedulers[self.scheduler_name],
                 device=self.device,
                 from_safetensors=self.is_safetensors,
+                load_safety_checker=self.do_nsfw_filter,
             )
             if self.is_controlnet:
                 pipeline = self.load_controlnet_from_ckpt(pipeline)
         except Exception as e:
             print("Something went wrong loading the model file", e)
             self.error_handler("Unable to load ckpt file")
             raise e
@@ -735,15 +749,29 @@
         self.image_guidance_scale = float(options.get(f"{action}_image_scale", self.image_guidance_scale))
         self.strength = float(options.get(f"{action}_strength") or 1)
         self.num_inference_steps = int(options.get(f"{action}_steps", self.num_inference_steps))
         self.height = int(options.get(f"{action}_height", self.height))
         self.width = int(options.get(f"{action}_width", self.width))
         self.C = int(options.get(f"{action}_C", self.C))
         self.f = int(options.get(f"{action}_f", self.f))
+        self.steps = int(options.get(f"{action}_steps", self.steps))
+        self.ddim_eta = float(options.get(f"{action}_ddim_eta", self.ddim_eta))
         self.batch_size = int(options.get(f"{action}_n_samples", self.batch_size))
+        self.n_samples = int(options.get(f"{action}_n_samples", self.n_samples))
+        self.pos_x = int(options.get(f"{action}_pos_x", self.pos_x))
+        self.pos_y = int(options.get(f"{action}_pos_y", self.pos_y))
+        self.outpaint_box_rect = options.get(f"{action}_outpaint_box_rect", self.outpaint_box_rect)
+        self.hf_token = ""
+        self.enable_model_cpu_offload = False
+        self.use_attention_slicing = self.use_attention_slicing
+        self.use_tf32 = self.use_tf32
+        self.use_cudnn_benchmark = self.use_cudnn_benchmark
+        self.use_enable_vae_slicing = self.use_enable_vae_slicing
+        self.use_xformers = self.use_xformers
+
         do_nsfw_filter = bool(options.get(f"do_nsfw_filter", self.do_nsfw_filter))
         self.do_nsfw_filter = do_nsfw_filter
         self.action = action
         self.options = options
 
         # memory settings
         self.use_last_channels = options.get("use_last_channels", True) == True
@@ -784,33 +812,35 @@
 
     def do_sample(self, **kwargs):
         logger.info(f"Sampling {self.action}")
         self.set_message(f"Generating image...")
         # move everything but this action to the cpu
         # self.move_models_to_cpu(self.action)
         #if not self.is_ckpt_model and not self.is_safetensors:
+        logger.info(f"Load safety checker")
         self.load_safety_checker(self.action)
 
         if not self.use_enable_sequential_cpu_offload:
             logger.debug("Moving to cuda")
             self.pipe.to("cuda") if self.cuda_is_available else None
         else:
             logger.debug("Enabling sequential cpu offload")
             self.pipe.enable_sequential_cpu_offload()
         try:
             if self.is_controlnet:
+                logger.info(f"Setting up controlnet")
                 #generator = torch.manual_seed(self.seed)
                 kwargs["image"] = self._preprocess_for_controlnet(kwargs.get("image"), process_type=self.controlnet_type)
                 #kwargs["generator"] = generator
 
-            if self.is_controlnet:
                 if kwargs.get("strength"):
                     kwargs["controlnet_conditioning_scale"] = kwargs["strength"]
                     del kwargs["strength"]
 
+            logger.info(f"Generating image")
             output = self.call_pipe(**kwargs)
         except Exception as e:
             logger.warning("something went wrong")
             print(e)
             logger.error(e)
             if "`flshattF` is not supported because" in str(e):
                 # try again
@@ -828,21 +858,75 @@
             nsfw_content_detected = None
             if self.action_has_safety_checker:
                 nsfw_content_detected = output.nsfw_content_detected
             return image, nsfw_content_detected
 
     active_extensions = []
 
+    def enhance_video(self, video_frames):
+        """
+        Iterate over each video frame and call img2img on it using the same options that were passed
+        and replace each frame with the enhanced version.
+        :param video_frames: list of numpy arrays
+        :return: video_frames: list of numpy arrays
+        """
+        new_video_frames = []
+        for img in video_frames:
+            pil_image = Image.fromarray(img)
+            pil_image = pil_image.resize((self.width, self.height), Image.LANCZOS)
+            image, nsfw_detected = self.generator_sample({
+                "action": "img2img",
+                "options": {
+                    "image": pil_image,
+                    "mask": pil_image,
+                    "img2img_prompt": self.prompt,
+                    "img2img_negative_prompt": self.negative_prompt,
+                    "img2img_steps": self.steps,
+                    "img2img_ddim_eta": self.ddim_eta,
+                    "img2img_n_iter": 1,
+                    "img2img_width": self.width,
+                    "img2img_height": self.height,
+                    "img2img_n_samples": 20,
+                    "img2img_strength": 0.5,
+                    "img2img_scale": 7.5,
+                    "img2img_seed": self.seed,
+                    "img2img_model": "Stable diffusion V2",
+                    "img2img_scheduler": self.scheduler_name,
+                    "img2img_model_path": "stabilityai/stable-diffusion-2-1-base",
+                    "img2img_model_branch": "fp16",
+                    "width": self.width,
+                    "height": self.height,
+                    "do_nsfw_filter": self.do_nsfw_filter,
+                    "model_base_path": self.model_base_path,
+                    "pos_x": self.pos_x,
+                    "pos_y": self.pos_y,
+                    "outpaint_box_rect": self.outpaint_box_rect,
+                    "hf_token": self.hf_token,
+                    "enable_model_cpu_offload": self.enable_model_cpu_offload,
+                    "use_attention_slicing": self.use_attention_slicing,
+                    "use_tf32": self.use_tf32,
+                    "use_cudnn_benchmark": self.use_cudnn_benchmark,
+                    "use_enable_vae_slicing": self.use_enable_vae_slicing,
+                    "use_xformers": self.use_xformers,
+                }
+            }, image_var=None, use_callback=False)
+            if image:
+                # convert to numpy array and add to new_video_frames
+                new_video_frames.append(np.array(image))
+        return new_video_frames if len(new_video_frames) > 0 else video_frames
+
     def handle_txt2vid_output(self, output):
         pil_image = None
         if output:
             from diffusers.utils import export_to_video
             video_frames = output.frames
             os.makedirs(os.path.dirname(self.txt2vid_file), exist_ok=True)
+            self.enhance_video(video_frames)
             export_to_video(video_frames, self.txt2vid_file)
+
             pil_image = Image.fromarray(video_frames[0])
         else:
             print("failed to get output from txt2vid")
         return pil_image, None
 
     def call_pipe_extension(self, **kwargs):
         """
@@ -856,18 +940,23 @@
 
     def call_pipe(self, **kwargs):
         """
         Generate an image using the pipe
         :param kwargs:
         :return:
         """
+        logger.info("Initialize compel")
         compel_proc = Compel(tokenizer=self.pipe.tokenizer, text_encoder=self.pipe.text_encoder)
+        logger.info("Initialize compel prompt")
         prompt_embeds = compel_proc(self.prompt)
+        logger.info("Initialize compel negative prompt")
         negative_prompt_embeds = compel_proc(self.negative_prompt) if self.negative_prompt else None
 
+        logger.info(f"is_txt2vid: {self.is_txt2vid}")
+
         if self.is_txt2vid:
             return self.pipe(
                 prompt_embeds=prompt_embeds,
                 negative_prompt_embeds=negative_prompt_embeds,
                 guidance_scale=self.guidance_scale,
                 num_inference_steps=self.num_inference_steps,
                 num_frames=self.batch_size,
@@ -1139,15 +1228,15 @@
         composite.putalpha(mask)
 
         # blend the composite image with the original image
         blended_image = Image.composite(composite, upscaled_image, mask)
 
         return blended_image
 
-    def _generate(self, data: dict, image_var: ImageVar = None):
+    def _generate(self, data: dict, image_var: ImageVar = None, use_callback: bool = True):
         logger.info("_generate called")
         self._prepare_options(data)
         self._prepare_scheduler()
         self._prepare_model()
         self._initialize()
         self._change_scheduler()
 
@@ -1158,15 +1247,18 @@
         self._apply_memory_efficient_settings()
         if self.is_txt2vid:
             total_to_generate = 1
         else:
             total_to_generate = self.batch_size
         for n in range(total_to_generate):
             image, nsfw_content_detected = self._sample_diffusers_model(data)
-            self.image_handler(image, data, nsfw_content_detected)
+            if use_callback:
+                self.image_handler(image, data, nsfw_content_detected)
+            else:
+                return image, nsfw_content_detected
             self.seed = self.seed + 1
             if self.do_cancel:
                 self.do_cancel = False
                 break
 
     def image_handler(self, image, data, nsfw_content_detected):
         if image:
@@ -1210,38 +1302,30 @@
         image = Image.fromarray(image)
         return image
 
     def generator_sample(
         self,
         data: dict,
         image_var: callable,
-        error_var: callable = None
+        error_var: callable = None,
+        use_callback: bool = True,
     ):
-        # check if model in data is cached
-        # if not, download it
-        # if it is, load it
         self.data = data
         self.set_message("Generating image...")
-        if data["action"] == "outpaint" and self.initialized and self.outpaint is None:
-            self.initialized = False
-        elif data["action"] == "img2img" and self.initialized and self.img2img is None:
-            self.initialized = False
-        elif data["action"] == "controlnet" and self.initialized and self.controlnet is None:
-            self.initialized = False
-        elif data["action"] == "depth" and self.initialized and self.depth2img is None:
-            self.initialized = False
-        elif data["action"] == "superresolution" and self.initialized and self.superresolution is None:
-            self.initialized = False
-        elif data["action"] == "txt2img" and self.initialized and self.txt2img is None:
-            self.initialized = False
-        elif data["action"] == "txt2vid" and self.initialized and self.txt2vid is None:
+
+        action = "depth2img" if data["action"] == "depth" else data["action"]
+        try:
+            self.initialized =  self.__dict__[action] is not None
+        except KeyError:
             self.initialized = False
+
         error = None
+        print(data)
         try:
-            self._generate(data, image_var=image_var)
+            self._generate(data, image_var=image_var, use_callback=use_callback)
         except OSError as e:
             err = e.args[0]
             logger.error(err)
             error = "model_not_found"
             err_obj = e
             traceback.print_exc() if self.is_dev_env else logger.error(err_obj)
         except TypeError as e:
```

### Comparing `aihandler-1.9.0/src/aihandler/settings.py` & `aihandler-1.9.1/src/aihandler/settings.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.0/src/aihandler/settings_manager.py` & `aihandler-1.9.1/src/aihandler/settings_manager.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.0/src/aihandler/socket_server.py` & `aihandler-1.9.1/src/aihandler/socket_server.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.0/src/aihandler/util.py` & `aihandler-1.9.1/src/aihandler/util.py`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.0/src/aihandler.egg-info/PKG-INFO` & `aihandler-1.9.1/src/aihandler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aihandler
-Version: 1.9.0
+Version: 1.9.1
 Summary: AI Handler: An engine which wraps certain huggingface models
 Home-page: https://github.com/Capsize-Games/aihandler
 Author: Capsize LLC
 Author-email: contact@capsize.gg
 License: AGPL-3.0
 Keywords: ai,chatbot,chat,ai
 Requires-Python: >=3.10.0
```

### Comparing `aihandler-1.9.0/src/aihandler.egg-info/SOURCES.txt` & `aihandler-1.9.1/src/aihandler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aihandler-1.9.0/src/aihandler.egg-info/requires.txt` & `aihandler-1.9.1/src/aihandler.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-torch==2.0.0
-torchvision==0.15.1
-torchaudio==2.0.1
 einops==0.6.0
 ninja==1.11.1
 JIT==0.2.7
 triton==2.0.0
 tqdm==4.65.0
 xformers==0.0.18
-bitsandbytes==0.37.0
 omegaconf==2.3.0
 accelerate==0.18.0
 controlnet_aux==0.0.1
 huggingface-hub==0.13.3
 numpy==1.23.5
 Pillow==9.4.0
 pip==23.0.1
@@ -33,7 +29,9 @@
 setuptools==65.5.1
 sympy==1.11.1
 typing_extensions==4.5.0
 urllib3==1.26.15
 diffusers==0.15.0
 transformers==4.27.4
 compel==1.1.3
+sympy==1.11.1
+regex
```

