# Comparing `tmp/image-reward-1.0.tar.gz` & `tmp/image-reward-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/image-reward-1.0.tar", last modified: Sun Apr 16 13:25:39 2023, max compression
+gzip compressed data, was "dist/image-reward-1.1.tar", last modified: Sun Apr 16 14:37:53 2023, max compression
```

## Comparing `image-reward-1.0.tar` & `image-reward-1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:25:39.000000 image-reward-1.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:25:39.000000 image-reward-1.0/ImageReward/
--rw-r--r--   0 root         (0) root         (0)     5231 2023-04-16 05:25:28.000000 image-reward-1.0/ImageReward/ImageReward.py
--rw-r--r--   0 root         (0) root         (0)       42 2023-04-16 05:51:49.000000 image-reward-1.0/ImageReward/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:25:39.000000 image-reward-1.0/ImageReward/models/
--rw-r--r--   0 root         (0) root         (0)     2570 2023-04-16 05:25:28.000000 image-reward-1.0/ImageReward/models/AestheticScore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:25:39.000000 image-reward-1.0/ImageReward/models/BLIP/
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-16 05:53:10.000000 image-reward-1.0/ImageReward/models/BLIP/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3125 2023-04-16 05:25:28.000000 image-reward-1.0/ImageReward/models/BLIP/blip.py
--rw-r--r--   0 root         (0) root         (0)     1502 2023-04-16 05:25:28.000000 image-reward-1.0/ImageReward/models/BLIP/blip_pretrain.py
--rw-r--r--   0 root         (0) root         (0)    41498 2023-04-16 05:25:28.000000 image-reward-1.0/ImageReward/models/BLIP/med.py
--rw-r--r--   0 root         (0) root         (0)    14061 2023-04-16 05:25:28.000000 image-reward-1.0/ImageReward/models/BLIP/vit.py
--rw-r--r--   0 root         (0) root         (0)     2739 2023-04-16 05:25:28.000000 image-reward-1.0/ImageReward/models/BLIPScore.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-04-16 05:25:28.000000 image-reward-1.0/ImageReward/models/CLIPScore.py
--rw-r--r--   0 root         (0) root         (0)       99 2023-04-16 05:53:38.000000 image-reward-1.0/ImageReward/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5868 2023-04-16 05:25:28.000000 image-reward-1.0/ImageReward/utils.py
--rw-r--r--   0 root         (0) root         (0)    11351 2023-04-16 05:25:28.000000 image-reward-1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4489 2023-04-16 13:25:39.000000 image-reward-1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4180 2023-04-16 05:25:28.000000 image-reward-1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:25:39.000000 image-reward-1.0/image_reward.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4489 2023-04-16 13:25:39.000000 image-reward-1.0/image_reward.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      580 2023-04-16 13:25:39.000000 image-reward-1.0/image_reward.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-04-16 13:25:39.000000 image-reward-1.0/image_reward.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-16 13:25:39.000000 image-reward-1.0/image_reward.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-16 13:25:39.000000 image-reward-1.0/image_reward.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 13:25:39.000000 image-reward-1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      980 2023-04-16 13:25:12.000000 image-reward-1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 14:37:53.000000 image-reward-1.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 14:37:53.000000 image-reward-1.1/ImageReward/
+-rw-r--r--   0 root         (0) root         (0)     5437 2023-04-16 14:33:13.000000 image-reward-1.1/ImageReward/ImageReward.py
+-rw-r--r--   0 root         (0) root         (0)       42 2023-04-16 13:56:03.000000 image-reward-1.1/ImageReward/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 14:37:53.000000 image-reward-1.1/ImageReward/models/
+-rw-r--r--   0 root         (0) root         (0)     2614 2023-04-16 14:34:13.000000 image-reward-1.1/ImageReward/models/AestheticScore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 14:37:53.000000 image-reward-1.1/ImageReward/models/BLIP/
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-16 13:56:03.000000 image-reward-1.1/ImageReward/models/BLIP/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3125 2023-04-16 13:56:03.000000 image-reward-1.1/ImageReward/models/BLIP/blip.py
+-rw-r--r--   0 root         (0) root         (0)     1502 2023-04-16 13:56:03.000000 image-reward-1.1/ImageReward/models/BLIP/blip_pretrain.py
+-rw-r--r--   0 root         (0) root         (0)    41498 2023-04-16 13:56:03.000000 image-reward-1.1/ImageReward/models/BLIP/med.py
+-rw-r--r--   0 root         (0) root         (0)    14061 2023-04-16 13:56:03.000000 image-reward-1.1/ImageReward/models/BLIP/vit.py
+-rw-r--r--   0 root         (0) root         (0)     2783 2023-04-16 14:34:23.000000 image-reward-1.1/ImageReward/models/BLIPScore.py
+-rw-r--r--   0 root         (0) root         (0)     2165 2023-04-16 14:35:17.000000 image-reward-1.1/ImageReward/models/CLIPScore.py
+-rw-r--r--   0 root         (0) root         (0)       99 2023-04-16 13:56:03.000000 image-reward-1.1/ImageReward/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5868 2023-04-16 13:56:03.000000 image-reward-1.1/ImageReward/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11351 2023-04-16 13:56:03.000000 image-reward-1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4481 2023-04-16 14:37:53.000000 image-reward-1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4172 2023-04-16 13:56:03.000000 image-reward-1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 14:37:53.000000 image-reward-1.1/image_reward.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4481 2023-04-16 14:37:52.000000 image-reward-1.1/image_reward.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      580 2023-04-16 14:37:53.000000 image-reward-1.1/image_reward.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-04-16 14:37:52.000000 image-reward-1.1/image_reward.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2023-04-16 14:37:52.000000 image-reward-1.1/image_reward.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-16 14:37:52.000000 image-reward-1.1/image_reward.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 14:37:53.000000 image-reward-1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      980 2023-04-16 14:37:22.000000 image-reward-1.1/setup.py
```

### Comparing `image-reward-1.0/ImageReward/ImageReward.py` & `image-reward-1.1/ImageReward/ImageReward.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,14 +78,18 @@
         
         self.mean = 0.16717362830052426
         self.std = 1.0333394966054072
 
 
     def score(self, prompt, image_path):
         
+        if (type(image_path).__name__=='list'):
+            _, rewards = self.inference_rank(prompt, image_path)
+            return rewards
+            
         # text encode
         text_input = self.blip.tokenizer(prompt, padding='max_length', truncation=True, max_length=35, return_tensors="pt").to(self.device)
         
         # image encode
         pil_image = Image.open(image_path)
         image = self.preprocess(pil_image).unsqueeze(0).to(self.device)
         image_embeds = self.blip.visual_encoder(image)
@@ -99,15 +103,15 @@
                                                 return_dict = True,
                                             )
         
         txt_features = text_output.last_hidden_state[:,0,:].float() # (feature_dim)
         rewards = self.mlp(txt_features)
         rewards = (rewards - self.mean) / self.std
         
-        return rewards.cpu().numpy().item()
+        return rewards.detach().cpu().numpy().item()
 
 
     def inference_rank(self, prompt, generations_list):
         
         text_input = self.blip.tokenizer(prompt, padding='max_length', truncation=True, max_length=35, return_tensors="pt").to(self.device)
         
         txt_set = []
@@ -127,12 +131,13 @@
                                                     return_dict = True,
                                                 )
             txt_set.append(text_output.last_hidden_state[:,0,:])
             
         txt_features = torch.cat(txt_set, 0).float() # [image_num, feature_dim]
         rewards = self.mlp(txt_features) # [image_num, 1]
         rewards = (rewards - self.mean) / self.std
+        rewards = torch.squeeze(rewards)
         _, rank = torch.sort(rewards, dim=0, descending=True)
         _, indices = torch.sort(rank, dim=0)
-        indices = torch.squeeze(indices) + 1
+        indices = indices + 1
         
-        return indices.cpu().numpy().tolist(), rewards.cpu().numpy().tolist()
+        return indices.detach().cpu().numpy().tolist(), rewards.detach().cpu().numpy().tolist()
```

### Comparing `image-reward-1.0/ImageReward/models/AestheticScore.py` & `image-reward-1.1/ImageReward/models/AestheticScore.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,12 +68,13 @@
             pil_image = Image.open(img_path)
             image = self.preprocess(pil_image).unsqueeze(0).to(self.device)
             image_features = F.normalize(self.clip_model.encode_image(image))
             img_set.append(image_features)
             
         img_features = torch.cat(img_set, 0).float() # [image_num, feature_dim]
         rewards = self.mlp(img_features)
+        rewards = torch.squeeze(rewards)
         _, rank = torch.sort(rewards, dim=0, descending=True)
         _, indices = torch.sort(rank, dim=0)
-        indices = torch.squeeze(indices) + 1
+        indices = indices + 1
         
-        return indices.cpu().numpy().tolist(), rewards.cpu().numpy().tolist()
+        return indices.detach().cpu().numpy().tolist(), rewards.detach().cpu().numpy().tolist()
```

### Comparing `image-reward-1.0/ImageReward/models/BLIP/blip.py` & `image-reward-1.1/ImageReward/models/BLIP/blip.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.0/ImageReward/models/BLIP/blip_pretrain.py` & `image-reward-1.1/ImageReward/models/BLIP/blip_pretrain.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.0/ImageReward/models/BLIP/med.py` & `image-reward-1.1/ImageReward/models/BLIP/med.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.0/ImageReward/models/BLIP/vit.py` & `image-reward-1.1/ImageReward/models/BLIP/vit.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.0/ImageReward/models/BLIPScore.py` & `image-reward-1.1/ImageReward/models/BLIPScore.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,12 +64,13 @@
             image_features = F.normalize(self.blip.vision_proj(image_embeds[:,0,:]), dim=-1)    
             img_set.append(image_features)
             txt_set.append(txt_feature)
             
         txt_features = torch.cat(txt_set, 0).float() # [image_num, feature_dim]
         img_features = torch.cat(img_set, 0).float() # [image_num, feature_dim]
         rewards = torch.sum(torch.mul(txt_features, img_features), dim=1, keepdim=True)
+        rewards = torch.squeeze(rewards)
         _, rank = torch.sort(rewards, dim=0, descending=True)
         _, indices = torch.sort(rank, dim=0)
-        indices = torch.squeeze(indices) + 1
+        indices = indices + 1
         
-        return indices.cpu().numpy().tolist(), rewards.cpu().numpy().tolist()
+        return indices.detach().cpu().numpy().tolist(), rewards.detach().cpu().numpy().tolist()
```

### Comparing `image-reward-1.0/ImageReward/models/CLIPScore.py` & `image-reward-1.1/ImageReward/models/CLIPScore.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,12 +45,13 @@
             image_features = F.normalize(self.clip_model.encode_image(image))
             img_set.append(image_features)
             txt_set.append(txt_feature)
             
         txt_features = torch.cat(txt_set, 0).float() # [image_num, feature_dim]
         img_features = torch.cat(img_set, 0).float() # [image_num, feature_dim]
         rewards = torch.sum(torch.mul(txt_features, img_features), dim=1, keepdim=True)
+        rewards = torch.squeeze(rewards)
         _, rank = torch.sort(rewards, dim=0, descending=True)
         _, indices = torch.sort(rank, dim=0)
-        indices = torch.squeeze(indices) + 1
+        indices = indices + 1
         
-        return indices.cpu().numpy().tolist(), rewards.cpu().numpy().tolist()
+        return indices.detach().cpu().numpy().tolist(), rewards.detach().cpu().numpy().tolist()
```

### Comparing `image-reward-1.0/ImageReward/utils.py` & `image-reward-1.1/ImageReward/utils.py`

 * *Files identical despite different names*

### Comparing `image-reward-1.0/LICENSE` & `image-reward-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `image-reward-1.0/PKG-INFO` & `image-reward-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-reward
-Version: 1.0
+Version: 1.1
 Summary: ImageReward
 Home-page: https://github.com/THUDM/ImageReward
 Author: Jiazheng Xu, et al.
 Author-email: <xjz22@mails.tsinghua.edu.cn>
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
@@ -60,22 +60,22 @@
 ```
 
 Use the following code to get the human preference scores from ImageReward:
 
 ```python
 import os
 import torch
-import ImageReward as reward
+import ImageReward as RM
 
 if __name__ == "__main__":
     prompt = "a painting of an ocean with clouds and birds, day time, low depth field effect"
     img_prefix = "assets/images"
     generations = [f"{pic_id}.webp" for pic_id in range(1, 5)]
     img_list = [os.path.join(img_prefix, img) for img in generations]
-    model = reward.load("ImageReward-v1.0")
+    model = RM.load("ImageReward-v1.0")
     with torch.no_grad():
         ranking, rewards = model.inference_rank(prompt, img_list)
         # Print the result
         print("\nPreference predictions:\n")
         print(f"ranking = {ranking}")
         print(f"rewards = {rewards}")
         for index in range(len(img_list)):
```

### Comparing `image-reward-1.0/README.md` & `image-reward-1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -48,22 +48,22 @@
 ```
 
 Use the following code to get the human preference scores from ImageReward:
 
 ```python
 import os
 import torch
-import ImageReward as reward
+import ImageReward as RM
 
 if __name__ == "__main__":
     prompt = "a painting of an ocean with clouds and birds, day time, low depth field effect"
     img_prefix = "assets/images"
     generations = [f"{pic_id}.webp" for pic_id in range(1, 5)]
     img_list = [os.path.join(img_prefix, img) for img in generations]
-    model = reward.load("ImageReward-v1.0")
+    model = RM.load("ImageReward-v1.0")
     with torch.no_grad():
         ranking, rewards = model.inference_rank(prompt, img_list)
         # Print the result
         print("\nPreference predictions:\n")
         print(f"ranking = {ranking}")
         print(f"rewards = {rewards}")
         for index in range(len(img_list)):
```

### Comparing `image-reward-1.0/image_reward.egg-info/PKG-INFO` & `image-reward-1.1/image_reward.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-reward
-Version: 1.0
+Version: 1.1
 Summary: ImageReward
 Home-page: https://github.com/THUDM/ImageReward
 Author: Jiazheng Xu, et al.
 Author-email: <xjz22@mails.tsinghua.edu.cn>
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
@@ -60,22 +60,22 @@
 ```
 
 Use the following code to get the human preference scores from ImageReward:
 
 ```python
 import os
 import torch
-import ImageReward as reward
+import ImageReward as RM
 
 if __name__ == "__main__":
     prompt = "a painting of an ocean with clouds and birds, day time, low depth field effect"
     img_prefix = "assets/images"
     generations = [f"{pic_id}.webp" for pic_id in range(1, 5)]
     img_list = [os.path.join(img_prefix, img) for img in generations]
-    model = reward.load("ImageReward-v1.0")
+    model = RM.load("ImageReward-v1.0")
     with torch.no_grad():
         ranking, rewards = model.inference_rank(prompt, img_list)
         # Print the result
         print("\nPreference predictions:\n")
         print(f"ranking = {ranking}")
         print(f"rewards = {rewards}")
         for index in range(len(img_list)):
```

### Comparing `image-reward-1.0/image_reward.egg-info/SOURCES.txt` & `image-reward-1.1/image_reward.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `image-reward-1.0/setup.py` & `image-reward-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = (Path(__file__).parent / "README.md").read_text()
 DESCRIPTION = 'ImageReward'
 
 # 配置
 setup(
         name="image-reward", 
         py_modules = ["ImageReward"],
-        version="1.0",
+        version="1.1",
         author="Jiazheng Xu, et al.",
         author_email="<xjz22@mails.tsinghua.edu.cn>",
         url="https://github.com/THUDM/ImageReward",
         description=DESCRIPTION,
         long_description=long_description,
         long_description_content_type='text/markdown',
         packages=find_packages(exclude=["tests*"]),
```

