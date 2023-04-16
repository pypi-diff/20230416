# Comparing `tmp/image-reward-0.997.tar.gz` & `tmp/image-reward-0.998.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/image-reward-0.997.tar", last modified: Sun Apr 16 13:11:13 2023, max compression
+gzip compressed data, was "dist/image-reward-0.998.tar", last modified: Sun Apr 16 13:15:19 2023, max compression
```

## Comparing `image-reward-0.997.tar` & `image-reward-0.998.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:11:13.000000 image-reward-0.997/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:11:13.000000 image-reward-0.997/ImageReward/
--rw-r--r--   0 root         (0) root         (0)     5231 2023-04-16 05:25:28.000000 image-reward-0.997/ImageReward/ImageReward.py
--rw-r--r--   0 root         (0) root         (0)       42 2023-04-16 05:51:49.000000 image-reward-0.997/ImageReward/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:11:13.000000 image-reward-0.997/ImageReward/models/
--rw-r--r--   0 root         (0) root         (0)     2570 2023-04-16 05:25:28.000000 image-reward-0.997/ImageReward/models/AestheticScore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:11:13.000000 image-reward-0.997/ImageReward/models/BLIP/
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-16 05:53:10.000000 image-reward-0.997/ImageReward/models/BLIP/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3125 2023-04-16 05:25:28.000000 image-reward-0.997/ImageReward/models/BLIP/blip.py
--rw-r--r--   0 root         (0) root         (0)     1502 2023-04-16 05:25:28.000000 image-reward-0.997/ImageReward/models/BLIP/blip_pretrain.py
--rw-r--r--   0 root         (0) root         (0)    41498 2023-04-16 05:25:28.000000 image-reward-0.997/ImageReward/models/BLIP/med.py
--rw-r--r--   0 root         (0) root         (0)    14061 2023-04-16 05:25:28.000000 image-reward-0.997/ImageReward/models/BLIP/vit.py
--rw-r--r--   0 root         (0) root         (0)     2739 2023-04-16 05:25:28.000000 image-reward-0.997/ImageReward/models/BLIPScore.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-04-16 05:25:28.000000 image-reward-0.997/ImageReward/models/CLIPScore.py
--rw-r--r--   0 root         (0) root         (0)       99 2023-04-16 05:53:38.000000 image-reward-0.997/ImageReward/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5868 2023-04-16 05:25:28.000000 image-reward-0.997/ImageReward/utils.py
--rw-r--r--   0 root         (0) root         (0)    11351 2023-04-16 05:25:28.000000 image-reward-0.997/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4525 2023-04-16 13:11:13.000000 image-reward-0.997/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4180 2023-04-16 05:25:28.000000 image-reward-0.997/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:11:13.000000 image-reward-0.997/image_reward.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4525 2023-04-16 13:11:13.000000 image-reward-0.997/image_reward.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      580 2023-04-16 13:11:13.000000 image-reward-0.997/image_reward.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-16 13:11:13.000000 image-reward-0.997/image_reward.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-16 13:11:13.000000 image-reward-0.997/image_reward.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-16 13:11:13.000000 image-reward-0.997/image_reward.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 13:11:13.000000 image-reward-0.997/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-16 13:10:53.000000 image-reward-0.997/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:15:19.000000 image-reward-0.998/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:15:19.000000 image-reward-0.998/ImageReward/
+-rw-r--r--   0 root         (0) root         (0)     5231 2023-04-16 05:25:28.000000 image-reward-0.998/ImageReward/ImageReward.py
+-rw-r--r--   0 root         (0) root         (0)       42 2023-04-16 05:51:49.000000 image-reward-0.998/ImageReward/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:15:19.000000 image-reward-0.998/ImageReward/models/
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-04-16 05:25:28.000000 image-reward-0.998/ImageReward/models/AestheticScore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:15:19.000000 image-reward-0.998/ImageReward/models/BLIP/
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-16 05:53:10.000000 image-reward-0.998/ImageReward/models/BLIP/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3125 2023-04-16 05:25:28.000000 image-reward-0.998/ImageReward/models/BLIP/blip.py
+-rw-r--r--   0 root         (0) root         (0)     1502 2023-04-16 05:25:28.000000 image-reward-0.998/ImageReward/models/BLIP/blip_pretrain.py
+-rw-r--r--   0 root         (0) root         (0)    41498 2023-04-16 05:25:28.000000 image-reward-0.998/ImageReward/models/BLIP/med.py
+-rw-r--r--   0 root         (0) root         (0)    14061 2023-04-16 05:25:28.000000 image-reward-0.998/ImageReward/models/BLIP/vit.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2023-04-16 05:25:28.000000 image-reward-0.998/ImageReward/models/BLIPScore.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-04-16 05:25:28.000000 image-reward-0.998/ImageReward/models/CLIPScore.py
+-rw-r--r--   0 root         (0) root         (0)       99 2023-04-16 05:53:38.000000 image-reward-0.998/ImageReward/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5868 2023-04-16 05:25:28.000000 image-reward-0.998/ImageReward/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11351 2023-04-16 05:25:28.000000 image-reward-0.998/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4525 2023-04-16 13:15:19.000000 image-reward-0.998/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4180 2023-04-16 05:25:28.000000 image-reward-0.998/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 13:15:19.000000 image-reward-0.998/image_reward.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4525 2023-04-16 13:15:19.000000 image-reward-0.998/image_reward.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      580 2023-04-16 13:15:19.000000 image-reward-0.998/image_reward.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-04-16 13:15:19.000000 image-reward-0.998/image_reward.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2023-04-16 13:15:19.000000 image-reward-0.998/image_reward.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-16 13:15:19.000000 image-reward-0.998/image_reward.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 13:15:19.000000 image-reward-0.998/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-04-16 13:15:04.000000 image-reward-0.998/setup.py
```

### Comparing `image-reward-0.997/ImageReward/ImageReward.py` & `image-reward-0.998/ImageReward/ImageReward.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.997/ImageReward/models/AestheticScore.py` & `image-reward-0.998/ImageReward/models/AestheticScore.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.997/ImageReward/models/BLIP/blip.py` & `image-reward-0.998/ImageReward/models/BLIP/blip.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.997/ImageReward/models/BLIP/blip_pretrain.py` & `image-reward-0.998/ImageReward/models/BLIP/blip_pretrain.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.997/ImageReward/models/BLIP/med.py` & `image-reward-0.998/ImageReward/models/BLIP/med.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.997/ImageReward/models/BLIP/vit.py` & `image-reward-0.998/ImageReward/models/BLIP/vit.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.997/ImageReward/models/BLIPScore.py` & `image-reward-0.998/ImageReward/models/BLIPScore.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.997/ImageReward/models/CLIPScore.py` & `image-reward-0.998/ImageReward/models/CLIPScore.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.997/ImageReward/utils.py` & `image-reward-0.998/ImageReward/utils.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.997/LICENSE` & `image-reward-0.998/LICENSE`

 * *Files identical despite different names*

### Comparing `image-reward-0.997/PKG-INFO` & `image-reward-0.998/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-reward
-Version: 0.997
+Version: 0.998
 Summary: ImageReward
 Author: xujz18
 Author-email: <xjz22@mails.tsinghua.edu.cn>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `image-reward-0.997/README.md` & `image-reward-0.998/README.md`

 * *Files identical despite different names*

### Comparing `image-reward-0.997/image_reward.egg-info/PKG-INFO` & `image-reward-0.998/image_reward.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-reward
-Version: 0.997
+Version: 0.998
 Summary: ImageReward
 Author: xujz18
 Author-email: <xjz22@mails.tsinghua.edu.cn>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `image-reward-0.997/image_reward.egg-info/SOURCES.txt` & `image-reward-0.998/image_reward.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `image-reward-0.997/setup.py` & `image-reward-0.998/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 long_description = (Path(__file__).parent / "README.md").read_text()
 DESCRIPTION = 'ImageReward'
 
 # 配置
 setup(
         name="image-reward", 
         py_modules = ["ImageReward"],
-        version="0.997",
+        version="0.998",
         author="xujz18",
         author_email="<xjz22@mails.tsinghua.edu.cn>",
         description=DESCRIPTION,
         long_description=long_description,
         long_description_content_type='text/markdown',
         packages=find_packages(exclude=["tests*"]),
         install_requires=[
             'timm==0.6.13',
             'transformers==4.27.4',
             'fairscale==0.4.13',
             'huggingface_hub==0.13.4',
         ],
         dependency_links = [
-            "https://github.com/openai/CLIP",
+            "clip @ git+https://github.com/openai/CLIP.git",
         ],
         classifiers=[
             "Programming Language :: Python :: 3",
             "License :: OSI Approved :: MIT License",
             "Operating System :: OS Independent",
         ],
 )
```

