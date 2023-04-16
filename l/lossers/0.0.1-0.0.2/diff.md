# Comparing `tmp/lossers-0.0.1.tar.gz` & `tmp/lossers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lossers-0.0.1.tar", last modified: Sat Apr 15 11:01:59 2023, max compression
+gzip compressed data, was "lossers-0.0.2.tar", last modified: Sun Apr 16 02:50:07 2023, max compression
```

## Comparing `lossers-0.0.1.tar` & `lossers-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 11:01:59.468519 lossers-0.0.1/
--rw-rw-rw-   0        0        0     1087 2023-03-24 10:25:10.000000 lossers-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      543 2023-04-15 11:01:59.468519 lossers-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       75 2023-04-15 09:30:19.000000 lossers-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 11:01:59.448518 lossers-0.0.1/lossers/
--rw-rw-rw-   0        0        0        0 2023-04-15 09:04:19.000000 lossers-0.0.1/lossers/__init__.py
--rw-rw-rw-   0        0        0      436 2023-04-15 09:27:11.000000 lossers-0.0.1/lossers/clip.py
--rw-rw-rw-   0        0        0     2776 2023-04-15 09:13:24.000000 lossers-0.0.1/lossers/ssim.py
-drwxrwxrwx   0        0        0        0 2023-04-15 11:01:59.468519 lossers-0.0.1/lossers.egg-info/
--rw-rw-rw-   0        0        0      543 2023-04-15 11:01:59.000000 lossers-0.0.1/lossers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-04-15 11:01:59.000000 lossers-0.0.1/lossers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 11:01:59.000000 lossers-0.0.1/lossers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-15 11:01:59.000000 lossers-0.0.1/lossers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 11:01:59.468519 lossers-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      699 2023-04-15 09:10:58.000000 lossers-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 02:50:07.597660 lossers-0.0.2/
+-rw-rw-rw-   0        0        0     1087 2023-03-24 10:25:10.000000 lossers-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      543 2023-04-16 02:50:07.597660 lossers-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       75 2023-04-15 09:30:19.000000 lossers-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 02:50:07.577660 lossers-0.0.2/lossers/
+-rw-rw-rw-   0        0        0        0 2023-04-15 09:04:19.000000 lossers-0.0.2/lossers/__init__.py
+-rw-rw-rw-   0        0        0      436 2023-04-15 09:27:11.000000 lossers-0.0.2/lossers/clip.py
+drwxrwxrwx   0        0        0        0 2023-04-16 02:50:07.597660 lossers-0.0.2/lossers/lpips/
+-rw-rw-rw-   0        0        0       26 2023-04-16 02:21:05.000000 lossers-0.0.2/lossers/lpips/__init__.py
+-rw-rw-rw-   0        0        0     4211 2023-04-16 02:41:50.000000 lossers-0.0.2/lossers/lpips/lpips.py
+-rw-rw-rw-   0        0        0     3128 2023-04-16 01:02:20.000000 lossers-0.0.2/lossers/lpips/pretrained_model.py
+-rw-rw-rw-   0        0        0     2776 2023-04-15 09:13:24.000000 lossers-0.0.2/lossers/ssim.py
+drwxrwxrwx   0        0        0        0 2023-04-16 02:50:07.587665 lossers-0.0.2/lossers.egg-info/
+-rw-rw-rw-   0        0        0      543 2023-04-16 02:50:06.000000 lossers-0.0.2/lossers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2023-04-16 02:50:07.000000 lossers-0.0.2/lossers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 02:50:07.000000 lossers-0.0.2/lossers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-16 02:50:07.000000 lossers-0.0.2/lossers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 02:50:07.597660 lossers-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      699 2023-04-16 02:44:21.000000 lossers-0.0.2/setup.py
```

### Comparing `lossers-0.0.1/LICENSE` & `lossers-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lossers-0.0.1/PKG-INFO` & `lossers-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lossers
-Version: 0.0.1
+Version: 0.0.2
 Summary: ML Loss Function
 Home-page: https://github.com/JiauZhang/lossers
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: MIT
 Keywords: artificial intelligence,loss function,deep learning
 Classifier: Intended Audience :: Developers
```

### Comparing `lossers-0.0.1/lossers/ssim.py` & `lossers-0.0.2/lossers/ssim.py`

 * *Files identical despite different names*

### Comparing `lossers-0.0.1/lossers.egg-info/PKG-INFO` & `lossers-0.0.2/lossers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lossers
-Version: 0.0.1
+Version: 0.0.2
 Summary: ML Loss Function
 Home-page: https://github.com/JiauZhang/lossers
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: MIT
 Keywords: artificial intelligence,loss function,deep learning
 Classifier: Intended Audience :: Developers
```

### Comparing `lossers-0.0.1/setup.py` & `lossers-0.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'lossers',
   packages = find_packages(),
-  version = '0.0.1',
+  version = '0.0.2',
   license='MIT',
   description = 'ML Loss Function',
   author = 'JiauZhang',
   author_email = 'jiauzhang@163.com',
   url = 'https://github.com/JiauZhang/lossers',
   long_description_content_type = 'text/markdown',
   keywords = [
```

