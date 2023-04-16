# Comparing `tmp/image-reward-0.992.tar.gz` & `tmp/image-reward-0.993.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-reward-0.992.tar", last modified: Sun Apr 16 12:17:19 2023, max compression
+gzip compressed data, was "image-reward-0.993.tar", last modified: Sun Apr 16 12:22:24 2023, max compression
```

## Comparing `image-reward-0.992.tar` & `image-reward-0.993.tar`

### file list

```diff
@@ -1,27 +1,16 @@
-drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-16 12:17:19.348533 image-reward-0.992/
-drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-16 12:17:19.348533 image-reward-0.992/ImageReward/
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     5231 2023-04-13 01:54:47.000000 image-reward-0.992/ImageReward/ImageReward.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       44 2023-04-16 12:16:33.000000 image-reward-0.992/ImageReward/__init__.py
-drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-16 12:17:19.348533 image-reward-0.992/ImageReward/models/
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     2570 2023-04-13 01:54:51.000000 image-reward-0.992/ImageReward/models/AestheticScore.py
-drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-16 12:17:19.348533 image-reward-0.992/ImageReward/models/BLIP/
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       30 2023-04-16 12:16:21.000000 image-reward-0.992/ImageReward/models/BLIP/__init__.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     3125 2023-04-13 02:31:10.000000 image-reward-0.992/ImageReward/models/BLIP/blip.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     1502 2023-04-13 02:31:05.000000 image-reward-0.992/ImageReward/models/BLIP/blip_pretrain.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)    41498 2023-04-13 02:30:44.000000 image-reward-0.992/ImageReward/models/BLIP/med.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)    14061 2023-04-13 02:30:55.000000 image-reward-0.992/ImageReward/models/BLIP/vit.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     2739 2023-04-13 01:54:50.000000 image-reward-0.992/ImageReward/models/BLIPScore.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     2121 2023-04-13 01:54:49.000000 image-reward-0.992/ImageReward/models/CLIPScore.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)      107 2023-04-16 12:16:25.000000 image-reward-0.992/ImageReward/models/__init__.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     5868 2023-04-13 01:55:02.000000 image-reward-0.992/ImageReward/utils.py
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)    11351 2023-04-13 01:21:59.000000 image-reward-0.992/LICENSE
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     1969 2023-04-16 12:17:19.348533 image-reward-0.992/PKG-INFO
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     3944 2023-04-13 01:33:39.000000 image-reward-0.992/README.md
-drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-16 12:17:19.348533 image-reward-0.992/image_reward.egg-info/
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     1969 2023-04-16 12:17:19.000000 image-reward-0.992/image_reward.egg-info/PKG-INFO
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)      580 2023-04-16 12:17:19.000000 image-reward-0.992/image_reward.egg-info/SOURCES.txt
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)        1 2023-04-16 12:17:19.000000 image-reward-0.992/image_reward.egg-info/dependency_links.txt
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       97 2023-04-16 12:17:19.000000 image-reward-0.992/image_reward.egg-info/requires.txt
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       12 2023-04-16 12:17:19.000000 image-reward-0.992/image_reward.egg-info/top_level.txt
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       38 2023-04-16 12:17:19.348533 image-reward-0.992/setup.cfg
--rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)      973 2023-04-16 12:17:03.000000 image-reward-0.992/setup.py
+drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-16 12:22:24.187197 image-reward-0.993/
+drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-16 12:22:24.187197 image-reward-0.993/ImageReward/
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     5231 2023-04-13 01:54:47.000000 image-reward-0.993/ImageReward/ImageReward.py
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       20 2023-04-16 12:21:03.000000 image-reward-0.993/ImageReward/__init__.py
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     5868 2023-04-13 01:55:02.000000 image-reward-0.993/ImageReward/utils.py
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)    11351 2023-04-13 01:21:59.000000 image-reward-0.993/LICENSE
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     1969 2023-04-16 12:22:24.187197 image-reward-0.993/PKG-INFO
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     3944 2023-04-13 01:33:39.000000 image-reward-0.993/README.md
+drwxrwxr-x   0 jiazhengx  (1003) jiazhengx  (1003)        0 2023-04-16 12:22:24.187197 image-reward-0.993/image_reward.egg-info/
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)     1969 2023-04-16 12:22:24.000000 image-reward-0.993/image_reward.egg-info/PKG-INFO
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)      277 2023-04-16 12:22:24.000000 image-reward-0.993/image_reward.egg-info/SOURCES.txt
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)        1 2023-04-16 12:22:24.000000 image-reward-0.993/image_reward.egg-info/dependency_links.txt
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       97 2023-04-16 12:22:24.000000 image-reward-0.993/image_reward.egg-info/requires.txt
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       12 2023-04-16 12:22:24.000000 image-reward-0.993/image_reward.egg-info/top_level.txt
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)       38 2023-04-16 12:22:24.187197 image-reward-0.993/setup.cfg
+-rw-rw-r--   0 jiazhengx  (1003) jiazhengx  (1003)      973 2023-04-16 12:22:12.000000 image-reward-0.993/setup.py
```

### Comparing `image-reward-0.992/ImageReward/ImageReward.py` & `image-reward-0.993/ImageReward/ImageReward.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.992/ImageReward/utils.py` & `image-reward-0.993/ImageReward/utils.py`

 * *Files identical despite different names*

### Comparing `image-reward-0.992/LICENSE` & `image-reward-0.993/LICENSE`

 * *Files identical despite different names*

### Comparing `image-reward-0.992/PKG-INFO` & `image-reward-0.993/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-reward
-Version: 0.992
+Version: 0.993
 Summary: ImageReward
 Author: xujz18
 Author-email: <xjz22@mails.tsinghua.edu.cn>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `image-reward-0.992/README.md` & `image-reward-0.993/README.md`

 * *Files identical despite different names*

### Comparing `image-reward-0.992/image_reward.egg-info/PKG-INFO` & `image-reward-0.993/image_reward.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image-reward
-Version: 0.992
+Version: 0.993
 Summary: ImageReward
 Author: xujz18
 Author-email: <xjz22@mails.tsinghua.edu.cn>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `image-reward-0.992/setup.py` & `image-reward-0.993/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = (Path(__file__).parent / "README-pypi.md").read_text()
 DESCRIPTION = 'ImageReward'
 
 # 配置
 setup(
         name="image-reward", 
         py_modules = ["ImageReward"],
-        version="0.992",
+        version="0.993",
         author="xujz18",
         author_email="<xjz22@mails.tsinghua.edu.cn>",
         description=DESCRIPTION,
         long_description=long_description,
         long_description_content_type='text/markdown',
         packages=find_packages(exclude=["tests*"]),
         install_requires=[
```

