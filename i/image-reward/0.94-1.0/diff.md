# Comparing `tmp/image-reward-0.94.tar.gz` & `tmp/image-reward-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-reward-0.94.tar", last modified: Wed Apr 12 13:38:56 2023, max compression
+gzip compressed data, was "dist/image-reward-1.0.tar", last modified: Sun Apr 16 13:25:39 2023, max compression
```

## Comparing `image-reward-0.94.tar` & `image-reward-1.0.tar`

### file list

```diff
@@ -1,15 +1,27 @@
-drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-12 13:38:56.484947 image-reward-0.94/
-drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-12 13:38:56.484947 image-reward-0.94/ImageReward/
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     5231 2023-04-08 13:28:23.000000 image-reward-0.94/ImageReward/ImageReward.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       20 2023-04-08 13:29:13.000000 image-reward-0.94/ImageReward/__init__.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     5868 2023-04-12 12:22:50.000000 image-reward-0.94/ImageReward/utils.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     1946 2023-04-12 13:38:56.484947 image-reward-0.94/PKG-INFO
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     3492 2023-04-12 13:21:16.000000 image-reward-0.94/README.md
-drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-12 13:38:56.484947 image-reward-0.94/image_reward.egg-info/
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     1946 2023-04-12 13:38:56.000000 image-reward-0.94/image_reward.egg-info/PKG-INFO
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)      269 2023-04-12 13:38:56.000000 image-reward-0.94/image_reward.egg-info/SOURCES.txt
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)        1 2023-04-12 13:38:56.000000 image-reward-0.94/image_reward.egg-info/dependency_links.txt
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       52 2023-04-12 13:38:56.000000 image-reward-0.94/image_reward.egg-info/requires.txt
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       12 2023-04-12 13:38:56.000000 image-reward-0.94/image_reward.egg-info/top_level.txt
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       38 2023-04-12 13:38:56.488947 image-reward-0.94/setup.cfg
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)      972 2023-04-12 13:31:46.000000 image-reward-0.94/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:25:39.000000 image-reward-1.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:25:39.000000 image-reward-1.0/ImageReward/
+-rw-r--r--   0 root         (0) root         (0)     5231 2023-04-16 05:25:28.000000 image-reward-1.0/ImageReward/ImageReward.py
+-rw-r--r--   0 root         (0) root         (0)       42 2023-04-16 05:51:49.000000 image-reward-1.0/ImageReward/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:25:39.000000 image-reward-1.0/ImageReward/models/
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-04-16 05:25:28.000000 image-reward-1.0/ImageReward/models/AestheticScore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:25:39.000000 image-reward-1.0/ImageReward/models/BLIP/
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-16 05:53:10.000000 image-reward-1.0/ImageReward/models/BLIP/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3125 2023-04-16 05:25:28.000000 image-reward-1.0/ImageReward/models/BLIP/blip.py
+-rw-r--r--   0 root         (0) root         (0)     1502 2023-04-16 05:25:28.000000 image-reward-1.0/ImageReward/models/BLIP/blip_pretrain.py
+-rw-r--r--   0 root         (0) root         (0)    41498 2023-04-16 05:25:28.000000 image-reward-1.0/ImageReward/models/BLIP/med.py
+-rw-r--r--   0 root         (0) root         (0)    14061 2023-04-16 05:25:28.000000 image-reward-1.0/ImageReward/models/BLIP/vit.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2023-04-16 05:25:28.000000 image-reward-1.0/ImageReward/models/BLIPScore.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-04-16 05:25:28.000000 image-reward-1.0/ImageReward/models/CLIPScore.py
+-rw-r--r--   0 root         (0) root         (0)       99 2023-04-16 05:53:38.000000 image-reward-1.0/ImageReward/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5868 2023-04-16 05:25:28.000000 image-reward-1.0/ImageReward/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11351 2023-04-16 05:25:28.000000 image-reward-1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4489 2023-04-16 13:25:39.000000 image-reward-1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4180 2023-04-16 05:25:28.000000 image-reward-1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:25:39.000000 image-reward-1.0/image_reward.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4489 2023-04-16 13:25:39.000000 image-reward-1.0/image_reward.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      580 2023-04-16 13:25:39.000000 image-reward-1.0/image_reward.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-04-16 13:25:39.000000 image-reward-1.0/image_reward.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2023-04-16 13:25:39.000000 image-reward-1.0/image_reward.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-16 13:25:39.000000 image-reward-1.0/image_reward.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 13:25:39.000000 image-reward-1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      980 2023-04-16 13:25:12.000000 image-reward-1.0/setup.py
```

### Comparing `image-reward-0.94/ImageReward/ImageReward.py` & `image-reward-1.0/ImageReward/ImageReward.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 @File       :   ImageReward.py
-@Time       :   2023/02/28 19:53:00
+@Time       :   2023/01/28 19:53:00
 @Auther     :   Jiazheng Xu
 @Contact    :   xjz22@mails.tsinghua.edu.cn
 @Description:   ImageReward Reward model.
 * Based on CLIP code base and improved-aesthetic-predictor code base
 * https://github.com/openai/CLIP
 * https://github.com/christophschuhmann/improved-aesthetic-predictor
 '''
```

### Comparing `image-reward-0.94/ImageReward/utils.py` & `image-reward-1.0/ImageReward/utils.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.94/README.md` & `image-reward-1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,42 @@
 # ImageReward
 
 <p align="center">
-   🤗 <a href="https://huggingface.co/THUDM/ImageReward" target="_blank">HF Repo</a> • 🐦 <a href="https://twitter.com/thukeg" target="_blank">Twitter</a> • 📃 <a href="" target="_blank">Paper (Coming soon)</a> <br>
+   🤗 <a href="https://huggingface.co/THUDM/ImageReward" target="_blank">HF Repo</a> • 🐦 <a href="https://twitter.com/thukeg" target="_blank">Twitter</a> • 📃 <a href="https://arxiv.org/abs/2304.05977" target="_blank">Paper</a> <br>
 </p>
 
 **ImageReward: Learning and Evaluating Human Preferences for Text-to-Image Generation**
 
-ImageReward is the first general-purpose text-to-image human preference RM which is trained on in total 137k pairs of
-expert comparisons, based on text prompts and corresponding model outputs from DiffusionDB. We demonstrate that
-ImageReward outperforms existing text-image scoring methods, such as CLIP, Aesthetic, and BLIP, in terms of
-understanding human preference in text-to-image synthesis through extensive analysis and experiments.
+ImageReward is the first general-purpose text-to-image human preference RM, which is trained on in total **137k pairs of expert comparisons**. 
 
-![ImageReward](figures/ImageReward.png)
+It outperforms existing text-image scoring methods, such as CLIP (by 38.6%), Aesthetic (by 39.6%), and BLIP (by 31.6%), in terms of understanding human preference in text-to-image synthesis. Try `image-reward` package in only 3 lines of code!
+
+```python
+# pip install image-reward
+import ImageReward as RM
+model = RM.load("ImageReward-v1.0")
+
+rewards = model.score("<prompt>", ["<img1_path>", "<img2_path>", ...])
+```
+
+If you find `ImageReward`'s open-source effort useful, please 🌟 us to encourage our following developement!
+
+<p align="center">
+    <img src="figures/ImageReward.png" width="700px">
+</p>
 
 ## Quick Start
 
 ### Install Dependency
 
 We have integrated the whole repository to a single python package `image-reward`. Following the commands below to prepare the environment:
 
 ```shell
 # Clone the ImageReward repository (containing data for testing)
-git clone https://github.com/THUDM/ImageReward-.git
+git clone https://github.com/THUDM/ImageReward.git
 cd ImageReward
 
 # Install the integrated package `image-reward`
 pip install image-reward
 ```
 
 ### Example Use
@@ -72,15 +83,17 @@
           2.webp: 0.27
           3.webp: -1.41
           4.webp: -2.03
 ```
 
 ## Reproduce Experiments in Table 2
 
-![ImageReward](figures/Table_2_in_paper.png)
+<p align="center">
+    <img src="figures/Table_2_in_paper.png" width="700px">
+</p>
 
 Run the following script to automatically download data, baseline models, and run experiments:
 
 ```bash
 bash ./scripts/test.sh
 ```
 
@@ -90,8 +103,17 @@
 * Generated outputs for each prompt (originally from [DiffusionDB](https://github.com/poloclub/diffusiondb)) can be downloaded from [Huggingface](https://huggingface.co/THUDM/ImageReward/blob/main/test_images.zip) or [Tsinghua Cloud](https://cloud.tsinghua.edu.cn/f/9bd245027652422499f4/?dl=1). It should be decompressed to `data/test_images`.
 
 ## Reproduce Experiments in Table 4
 TODO
 
 ## Citation
 
-TODO
+```
+@misc{xu2023imagereward,
+      title={ImageReward: Learning and Evaluating Human Preferences for Text-to-Image Generation}, 
+      author={Jiazheng Xu and Xiao Liu and Yuchen Wu and Yuxuan Tong and Qinkai Li and Ming Ding and Jie Tang and Yuxiao Dong},
+      year={2023},
+      eprint={2304.05977},
+      archivePrefix={arXiv},
+      primaryClass={cs.CV}
+}
+```
```

