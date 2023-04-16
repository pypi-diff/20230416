# Comparing `tmp/image-reward-0.993.tar.gz` & `tmp/image-reward-0.994.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-reward-0.993.tar", last modified: Sun Apr 16 12:22:24 2023, max compression
+gzip compressed data, was "dist/image-reward-0.994.tar", last modified: Sun Apr 16 12:28:23 2023, max compression
```

## Comparing `image-reward-0.993.tar` & `image-reward-0.994.tar`

### file list

```diff
@@ -1,16 +1,27 @@
-drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-16 12:22:24.187197 image-reward-0.993/
-drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-16 12:22:24.187197 image-reward-0.993/ImageReward/
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     5231 2023-04-13 01:54:47.000000 image-reward-0.993/ImageReward/ImageReward.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       20 2023-04-16 12:21:03.000000 image-reward-0.993/ImageReward/__init__.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     5868 2023-04-13 01:55:02.000000 image-reward-0.993/ImageReward/utils.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)    11351 2023-04-13 01:21:59.000000 image-reward-0.993/LICENSE
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     1969 2023-04-16 12:22:24.187197 image-reward-0.993/PKG-INFO
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     3944 2023-04-13 01:33:39.000000 image-reward-0.993/README.md
-drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-16 12:22:24.187197 image-reward-0.993/image_reward.egg-info/
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     1969 2023-04-16 12:22:24.000000 image-reward-0.993/image_reward.egg-info/PKG-INFO
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)      277 2023-04-16 12:22:24.000000 image-reward-0.993/image_reward.egg-info/SOURCES.txt
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)        1 2023-04-16 12:22:24.000000 image-reward-0.993/image_reward.egg-info/dependency_links.txt
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       97 2023-04-16 12:22:24.000000 image-reward-0.993/image_reward.egg-info/requires.txt
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       12 2023-04-16 12:22:24.000000 image-reward-0.993/image_reward.egg-info/top_level.txt
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       38 2023-04-16 12:22:24.187197 image-reward-0.993/setup.cfg
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)      973 2023-04-16 12:22:12.000000 image-reward-0.993/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:28:23.000000 image-reward-0.994/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:28:23.000000 image-reward-0.994/ImageReward/
+-rw-r--r--   0 root         (0) root         (0)     5231 2023-04-16 05:25:28.000000 image-reward-0.994/ImageReward/ImageReward.py
+-rw-r--r--   0 root         (0) root         (0)       42 2023-04-16 05:51:49.000000 image-reward-0.994/ImageReward/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:28:23.000000 image-reward-0.994/ImageReward/models/
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-04-16 05:25:28.000000 image-reward-0.994/ImageReward/models/AestheticScore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:28:23.000000 image-reward-0.994/ImageReward/models/BLIP/
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-16 05:53:10.000000 image-reward-0.994/ImageReward/models/BLIP/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3125 2023-04-16 05:25:28.000000 image-reward-0.994/ImageReward/models/BLIP/blip.py
+-rw-r--r--   0 root         (0) root         (0)     1502 2023-04-16 05:25:28.000000 image-reward-0.994/ImageReward/models/BLIP/blip_pretrain.py
+-rw-r--r--   0 root         (0) root         (0)    41498 2023-04-16 05:25:28.000000 image-reward-0.994/ImageReward/models/BLIP/med.py
+-rw-r--r--   0 root         (0) root         (0)    14061 2023-04-16 05:25:28.000000 image-reward-0.994/ImageReward/models/BLIP/vit.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2023-04-16 05:25:28.000000 image-reward-0.994/ImageReward/models/BLIPScore.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-04-16 05:25:28.000000 image-reward-0.994/ImageReward/models/CLIPScore.py
+-rw-r--r--   0 root         (0) root         (0)       99 2023-04-16 05:53:38.000000 image-reward-0.994/ImageReward/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5868 2023-04-16 05:25:28.000000 image-reward-0.994/ImageReward/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11351 2023-04-16 05:25:28.000000 image-reward-0.994/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4525 2023-04-16 12:28:23.000000 image-reward-0.994/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4180 2023-04-16 05:25:28.000000 image-reward-0.994/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 12:28:23.000000 image-reward-0.994/image_reward.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4525 2023-04-16 12:28:23.000000 image-reward-0.994/image_reward.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      580 2023-04-16 12:28:23.000000 image-reward-0.994/image_reward.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 12:28:23.000000 image-reward-0.994/image_reward.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2023-04-16 12:28:23.000000 image-reward-0.994/image_reward.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-16 12:28:23.000000 image-reward-0.994/image_reward.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 12:28:23.000000 image-reward-0.994/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      968 2023-04-16 12:28:13.000000 image-reward-0.994/setup.py
```

### Comparing `image-reward-0.993/ImageReward/ImageReward.py` & `image-reward-0.994/ImageReward/ImageReward.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.993/ImageReward/utils.py` & `image-reward-0.994/ImageReward/utils.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.993/LICENSE` & `image-reward-0.994/LICENSE`

 * *Files identical despite different names*

### Comparing `image-reward-0.993/README.md` & `image-reward-0.994/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,27 @@
 
 <p align="center">
    🤗 <a href="https://huggingface.co/THUDM/ImageReward" target="_blank">HF Repo</a> • 🐦 <a href="https://twitter.com/thukeg" target="_blank">Twitter</a> • 📃 <a href="https://arxiv.org/abs/2304.05977" target="_blank">Paper</a> <br>
 </p>
 
 **ImageReward: Learning and Evaluating Human Preferences for Text-to-Image Generation**
 
-ImageReward is the first general-purpose text-to-image human preference RM which is trained on in total 137k pairs of
-expert comparisons, based on text prompts and corresponding model outputs from DiffusionDB. We demonstrate that
-ImageReward outperforms existing text-image scoring methods, such as CLIP, Aesthetic, and BLIP, in terms of
-understanding human preference in text-to-image synthesis through extensive analysis and experiments.
+ImageReward is the first general-purpose text-to-image human preference RM, which is trained on in total **137k pairs of expert comparisons**. 
+
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
 
 <p align="center">
     <img src="figures/ImageReward.png" width="700px">
 </p>
 
 ## Quick Start
 
@@ -103,8 +112,8 @@
       title={ImageReward: Learning and Evaluating Human Preferences for Text-to-Image Generation}, 
       author={Jiazheng Xu and Xiao Liu and Yuchen Wu and Yuxuan Tong and Qinkai Li and Ming Ding and Jie Tang and Yuxiao Dong},
       year={2023},
       eprint={2304.05977},
       archivePrefix={arXiv},
       primaryClass={cs.CV}
 }
-```
+```
```

### Comparing `image-reward-0.993/setup.py` & `image-reward-0.994/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 import os
 import pkg_resources
 from pathlib import Path
 
-long_description = (Path(__file__).parent / "README-pypi.md").read_text()
+long_description = (Path(__file__).parent / "README.md").read_text()
 DESCRIPTION = 'ImageReward'
 
 # 配置
 setup(
         name="image-reward", 
         py_modules = ["ImageReward"],
-        version="0.993",
+        version="0.994",
         author="xujz18",
         author_email="<xjz22@mails.tsinghua.edu.cn>",
         description=DESCRIPTION,
         long_description=long_description,
         long_description_content_type='text/markdown',
         packages=find_packages(exclude=["tests*"]),
         install_requires=[
```

