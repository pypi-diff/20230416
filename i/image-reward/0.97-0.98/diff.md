# Comparing `tmp/image-reward-0.97.tar.gz` & `tmp/image-reward-0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/image-reward-0.97.tar", last modified: Sun Apr 16 07:30:20 2023, max compression
+gzip compressed data, was "dist/image-reward-0.98.tar", last modified: Sun Apr 16 07:33:08 2023, max compression
```

## Comparing `image-reward-0.97.tar` & `image-reward-0.98.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 07:30:20.000000 image-reward-0.97/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 07:30:20.000000 image-reward-0.97/ImageReward/
--rw-r--r--   0 root         (0) root         (0)     5231 2023-04-16 05:25:28.000000 image-reward-0.97/ImageReward/ImageReward.py
--rw-r--r--   0 root         (0) root         (0)       42 2023-04-16 05:51:49.000000 image-reward-0.97/ImageReward/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 07:30:20.000000 image-reward-0.97/ImageReward/models/
--rw-r--r--   0 root         (0) root         (0)     2570 2023-04-16 05:25:28.000000 image-reward-0.97/ImageReward/models/AestheticScore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 07:30:20.000000 image-reward-0.97/ImageReward/models/BLIP/
--rw-r--r--   0 root         (0) root         (0)       28 2023-04-16 05:53:10.000000 image-reward-0.97/ImageReward/models/BLIP/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3125 2023-04-16 05:25:28.000000 image-reward-0.97/ImageReward/models/BLIP/blip.py
--rw-r--r--   0 root         (0) root         (0)     1502 2023-04-16 05:25:28.000000 image-reward-0.97/ImageReward/models/BLIP/blip_pretrain.py
--rw-r--r--   0 root         (0) root         (0)    41498 2023-04-16 05:25:28.000000 image-reward-0.97/ImageReward/models/BLIP/med.py
--rw-r--r--   0 root         (0) root         (0)    14061 2023-04-16 05:25:28.000000 image-reward-0.97/ImageReward/models/BLIP/vit.py
--rw-r--r--   0 root         (0) root         (0)     2739 2023-04-16 05:25:28.000000 image-reward-0.97/ImageReward/models/BLIPScore.py
--rw-r--r--   0 root         (0) root         (0)     2121 2023-04-16 05:25:28.000000 image-reward-0.97/ImageReward/models/CLIPScore.py
--rw-r--r--   0 root         (0) root         (0)       99 2023-04-16 05:53:38.000000 image-reward-0.97/ImageReward/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5868 2023-04-16 05:25:28.000000 image-reward-0.97/ImageReward/utils.py
--rw-r--r--   0 root         (0) root         (0)    11351 2023-04-16 05:25:28.000000 image-reward-0.97/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3639 2023-04-16 07:30:20.000000 image-reward-0.97/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4180 2023-04-16 05:25:28.000000 image-reward-0.97/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 07:30:20.000000 image-reward-0.97/image_reward.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3639 2023-04-16 07:30:20.000000 image-reward-0.97/image_reward.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      580 2023-04-16 07:30:20.000000 image-reward-0.97/image_reward.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 07:30:20.000000 image-reward-0.97/image_reward.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-16 07:30:20.000000 image-reward-0.97/image_reward.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-04-16 07:30:20.000000 image-reward-0.97/image_reward.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 07:30:20.000000 image-reward-0.97/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      972 2023-04-16 07:29:44.000000 image-reward-0.97/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 07:33:08.000000 image-reward-0.98/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 07:33:08.000000 image-reward-0.98/ImageReward/
+-rw-r--r--   0 root         (0) root         (0)     5231 2023-04-16 05:25:28.000000 image-reward-0.98/ImageReward/ImageReward.py
+-rw-r--r--   0 root         (0) root         (0)       42 2023-04-16 05:51:49.000000 image-reward-0.98/ImageReward/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 07:33:08.000000 image-reward-0.98/ImageReward/models/
+-rw-r--r--   0 root         (0) root         (0)     2570 2023-04-16 05:25:28.000000 image-reward-0.98/ImageReward/models/AestheticScore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 07:33:08.000000 image-reward-0.98/ImageReward/models/BLIP/
+-rw-r--r--   0 root         (0) root         (0)       28 2023-04-16 05:53:10.000000 image-reward-0.98/ImageReward/models/BLIP/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3125 2023-04-16 05:25:28.000000 image-reward-0.98/ImageReward/models/BLIP/blip.py
+-rw-r--r--   0 root         (0) root         (0)     1502 2023-04-16 05:25:28.000000 image-reward-0.98/ImageReward/models/BLIP/blip_pretrain.py
+-rw-r--r--   0 root         (0) root         (0)    41498 2023-04-16 05:25:28.000000 image-reward-0.98/ImageReward/models/BLIP/med.py
+-rw-r--r--   0 root         (0) root         (0)    14061 2023-04-16 05:25:28.000000 image-reward-0.98/ImageReward/models/BLIP/vit.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2023-04-16 05:25:28.000000 image-reward-0.98/ImageReward/models/BLIPScore.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2023-04-16 05:25:28.000000 image-reward-0.98/ImageReward/models/CLIPScore.py
+-rw-r--r--   0 root         (0) root         (0)       99 2023-04-16 05:53:38.000000 image-reward-0.98/ImageReward/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5868 2023-04-16 05:25:28.000000 image-reward-0.98/ImageReward/utils.py
+-rw-r--r--   0 root         (0) root         (0)    11351 2023-04-16 05:25:28.000000 image-reward-0.98/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3639 2023-04-16 07:33:08.000000 image-reward-0.98/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4180 2023-04-16 05:25:28.000000 image-reward-0.98/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 07:33:08.000000 image-reward-0.98/image_reward.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3639 2023-04-16 07:33:08.000000 image-reward-0.98/image_reward.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      580 2023-04-16 07:33:08.000000 image-reward-0.98/image_reward.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 07:33:08.000000 image-reward-0.98/image_reward.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2023-04-16 07:33:08.000000 image-reward-0.98/image_reward.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-04-16 07:33:08.000000 image-reward-0.98/image_reward.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 07:33:08.000000 image-reward-0.98/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      974 2023-04-16 07:32:48.000000 image-reward-0.98/setup.py
```

### Comparing `image-reward-0.97/ImageReward/ImageReward.py` & `image-reward-0.98/ImageReward/ImageReward.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.97/ImageReward/models/AestheticScore.py` & `image-reward-0.98/ImageReward/models/AestheticScore.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.97/ImageReward/models/BLIP/blip.py` & `image-reward-0.98/ImageReward/models/BLIP/blip.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.97/ImageReward/models/BLIP/blip_pretrain.py` & `image-reward-0.98/ImageReward/models/BLIP/blip_pretrain.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.97/ImageReward/models/BLIP/med.py` & `image-reward-0.98/ImageReward/models/BLIP/med.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.97/ImageReward/models/BLIP/vit.py` & `image-reward-0.98/ImageReward/models/BLIP/vit.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.97/ImageReward/models/BLIPScore.py` & `image-reward-0.98/ImageReward/models/BLIPScore.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.97/ImageReward/models/CLIPScore.py` & `image-reward-0.98/ImageReward/models/CLIPScore.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.97/ImageReward/utils.py` & `image-reward-0.98/ImageReward/utils.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.97/LICENSE` & `image-reward-0.98/LICENSE`

 * *Files identical despite different names*

### Comparing `image-reward-0.97/PKG-INFO` & `image-reward-0.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-reward
-Version: 0.97
+Version: 0.98
 Summary: ImageReward
 Author: xujz18
 Author-email: <xjz22@mails.tsinghua.edu.cn>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `image-reward-0.97/README.md` & `image-reward-0.98/README.md`

 * *Files identical despite different names*

### Comparing `image-reward-0.97/image_reward.egg-info/PKG-INFO` & `image-reward-0.98/image_reward.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-reward
-Version: 0.97
+Version: 0.98
 Summary: ImageReward
 Author: xujz18
 Author-email: <xjz22@mails.tsinghua.edu.cn>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `image-reward-0.97/image_reward.egg-info/SOURCES.txt` & `image-reward-0.98/image_reward.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `image-reward-0.97/setup.py` & `image-reward-0.98/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 long_description = (Path(__file__).parent / "README-pypi.md").read_text()
 DESCRIPTION = 'ImageReward'
 
 # 配置
 setup(
         name="image-reward", 
-        py_modules = ["ImageReward"],
-        version="0.97",
+        # py_modules = ["ImageReward"],
+        version="0.98",
         author="xujz18",
         author_email="<xjz22@mails.tsinghua.edu.cn>",
         description=DESCRIPTION,
         long_description=long_description,
         long_description_content_type='text/markdown',
         packages=find_packages(exclude=["tests*"]),
         install_requires=[
```

