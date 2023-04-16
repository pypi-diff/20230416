# Comparing `tmp/image-reward-0.95.tar.gz` & `tmp/image-reward-0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/image-reward-0.95.tar", last modified: Sun Apr 16 07:16:11 2023, max compression
+gzip compressed data, was "dist/image-reward-0.96.tar", last modified: Sun Apr 16 07:24:46 2023, max compression
```

## Comparing `image-reward-0.95.tar` & `image-reward-0.96.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 07:16:11.000000 image-reward-0.95/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 07:16:10.000000 image-reward-0.95/ImageReward/
--rw-r--r--   0 root         (0) root         (0)     5231 2023-04-16 05:25:28.000000 image-reward-0.95/ImageReward/ImageReward.py
--rw-r--r--   0 root         (0) root         (0)       42 2023-04-16 05:51:49.000000 image-reward-0.95/ImageReward/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 07:16:10.000000 image-reward-0.95/ImageReward/models/
--rw-r--r--   0 root         (0) root         (0)     2570 2023-04-16 05:25:28.000000 image-reward-0.95/ImageReward/models/AestheticScore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 07:16:11.000000 image-reward-0.95/ImageReward/models/BLIP/
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-16 05:53:10.000000 image-reward-0.95/ImageReward/models/BLIP/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3125 2023-04-16 05:25:28.000000 image-reward-0.95/ImageReward/models/BLIP/blip.py
--rw-r--r--   0 root         (0) root         (0)     1502 2023-04-16 05:25:28.000000 image-reward-0.95/ImageReward/models/BLIP/blip_pretrain.py
--rw-r--r--   0 root         (0) root         (0)    41498 2023-04-16 05:25:28.000000 image-reward-0.95/ImageReward/models/BLIP/med.py
--rw-r--r--   0 root         (0) root         (0)    14061 2023-04-16 05:25:28.000000 image-reward-0.95/ImageReward/models/BLIP/vit.py
--rw-r--r--   0 root         (0) root         (0)     2739 2023-04-16 05:25:28.000000 image-reward-0.95/ImageReward/models/BLIPScore.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-04-16 05:25:28.000000 image-reward-0.95/ImageReward/models/CLIPScore.py
--rw-r--r--   0 root         (0) root         (0)       99 2023-04-16 05:53:38.000000 image-reward-0.95/ImageReward/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5868 2023-04-16 05:25:28.000000 image-reward-0.95/ImageReward/utils.py
--rw-r--r--   0 root         (0) root         (0)    11351 2023-04-16 05:25:28.000000 image-reward-0.95/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4524 2023-04-16 07:16:11.000000 image-reward-0.95/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4180 2023-04-16 05:25:28.000000 image-reward-0.95/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 07:16:11.000000 image-reward-0.95/image_reward.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4524 2023-04-16 07:16:10.000000 image-reward-0.95/image_reward.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      580 2023-04-16 07:16:10.000000 image-reward-0.95/image_reward.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 07:16:10.000000 image-reward-0.95/image_reward.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-16 07:16:10.000000 image-reward-0.95/image_reward.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-16 07:16:10.000000 image-reward-0.95/image_reward.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 07:16:11.000000 image-reward-0.95/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      967 2023-04-16 07:15:10.000000 image-reward-0.95/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 07:24:46.000000 image-reward-0.96/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 07:24:46.000000 image-reward-0.96/ImageReward/
+-rw-r--r--   0 root         (0) root         (0)     5231 2023-04-16 05:25:28.000000 image-reward-0.96/ImageReward/ImageReward.py
+-rw-r--r--   0 root         (0) root         (0)       42 2023-04-16 05:51:49.000000 image-reward-0.96/ImageReward/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 07:24:46.000000 image-reward-0.96/ImageReward/models/
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-04-16 05:25:28.000000 image-reward-0.96/ImageReward/models/AestheticScore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 07:24:46.000000 image-reward-0.96/ImageReward/models/BLIP/
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-16 05:53:10.000000 image-reward-0.96/ImageReward/models/BLIP/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3125 2023-04-16 05:25:28.000000 image-reward-0.96/ImageReward/models/BLIP/blip.py
+-rw-r--r--   0 root         (0) root         (0)     1502 2023-04-16 05:25:28.000000 image-reward-0.96/ImageReward/models/BLIP/blip_pretrain.py
+-rw-r--r--   0 root         (0) root         (0)    41498 2023-04-16 05:25:28.000000 image-reward-0.96/ImageReward/models/BLIP/med.py
+-rw-r--r--   0 root         (0) root         (0)    14061 2023-04-16 05:25:28.000000 image-reward-0.96/ImageReward/models/BLIP/vit.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2023-04-16 05:25:28.000000 image-reward-0.96/ImageReward/models/BLIPScore.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-04-16 05:25:28.000000 image-reward-0.96/ImageReward/models/CLIPScore.py
+-rw-r--r--   0 root         (0) root         (0)       99 2023-04-16 05:53:38.000000 image-reward-0.96/ImageReward/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5868 2023-04-16 05:25:28.000000 image-reward-0.96/ImageReward/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11351 2023-04-16 05:25:28.000000 image-reward-0.96/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4524 2023-04-16 07:24:46.000000 image-reward-0.96/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4180 2023-04-16 05:25:28.000000 image-reward-0.96/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 07:24:46.000000 image-reward-0.96/image_reward.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4524 2023-04-16 07:24:45.000000 image-reward-0.96/image_reward.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      580 2023-04-16 07:24:45.000000 image-reward-0.96/image_reward.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 07:24:45.000000 image-reward-0.96/image_reward.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2023-04-16 07:24:45.000000 image-reward-0.96/image_reward.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-16 07:24:45.000000 image-reward-0.96/image_reward.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 07:24:46.000000 image-reward-0.96/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      967 2023-04-16 07:23:22.000000 image-reward-0.96/setup.py
```

### Comparing `image-reward-0.95/ImageReward/ImageReward.py` & `image-reward-0.96/ImageReward/ImageReward.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.95/ImageReward/models/AestheticScore.py` & `image-reward-0.96/ImageReward/models/AestheticScore.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.95/ImageReward/models/BLIP/blip.py` & `image-reward-0.96/ImageReward/models/BLIP/blip.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.95/ImageReward/models/BLIP/blip_pretrain.py` & `image-reward-0.96/ImageReward/models/BLIP/blip_pretrain.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.95/ImageReward/models/BLIP/med.py` & `image-reward-0.96/ImageReward/models/BLIP/med.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.95/ImageReward/models/BLIP/vit.py` & `image-reward-0.96/ImageReward/models/BLIP/vit.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.95/ImageReward/models/BLIPScore.py` & `image-reward-0.96/ImageReward/models/BLIPScore.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.95/ImageReward/models/CLIPScore.py` & `image-reward-0.96/ImageReward/models/CLIPScore.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.95/ImageReward/utils.py` & `image-reward-0.96/ImageReward/utils.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.95/LICENSE` & `image-reward-0.96/LICENSE`

 * *Files identical despite different names*

### Comparing `image-reward-0.95/PKG-INFO` & `image-reward-0.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-reward
-Version: 0.95
+Version: 0.96
 Summary: ImageReward
 Author: xujz18
 Author-email: <xjz22@mails.tsinghua.edu.cn>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `image-reward-0.95/README.md` & `image-reward-0.96/README.md`

 * *Files identical despite different names*

### Comparing `image-reward-0.95/image_reward.egg-info/PKG-INFO` & `image-reward-0.96/image_reward.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-reward
-Version: 0.95
+Version: 0.96
 Summary: ImageReward
 Author: xujz18
 Author-email: <xjz22@mails.tsinghua.edu.cn>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `image-reward-0.95/image_reward.egg-info/SOURCES.txt` & `image-reward-0.96/image_reward.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `image-reward-0.95/setup.py` & `image-reward-0.96/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = (Path(__file__).parent / "README.md").read_text()
 DESCRIPTION = 'ImageReward'
 
 # 配置
 setup(
         name="image-reward", 
         py_modules = ["ImageReward"],
-        version="0.95",
+        version="0.96",
         author="xujz18",
         author_email="<xjz22@mails.tsinghua.edu.cn>",
         description=DESCRIPTION,
         long_description=long_description,
         long_description_content_type='text/markdown',
         packages=find_packages(exclude=["tests*"]),
         install_requires=[
```

