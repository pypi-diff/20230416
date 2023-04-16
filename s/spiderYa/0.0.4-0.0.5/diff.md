# Comparing `tmp/spiderYa-0.0.4.tar.gz` & `tmp/spiderYa-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spiderYa-0.0.4.tar", last modified: Sun Apr 16 13:02:42 2023, max compression
+gzip compressed data, was "dist/spiderYa-0.0.5.tar", last modified: Sun Apr 16 13:12:13 2023, max compression
```

## Comparing `spiderYa-0.0.4.tar` & `spiderYa-0.0.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-16 13:02:42.000000 spiderYa-0.0.4/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1068 2023-04-16 08:59:14.000000 spiderYa-0.0.4/LICENSE
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      570 2023-04-16 13:02:42.000000 spiderYa-0.0.4/PKG-INFO
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      170 2023-04-16 08:58:58.000000 spiderYa-0.0.4/README.md
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       78 2023-04-16 13:02:42.000000 spiderYa-0.0.4/setup.cfg
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1403 2023-04-16 13:02:36.000000 spiderYa-0.0.4/setup.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-16 13:02:42.000000 spiderYa-0.0.4/spider/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     8196 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/SPIDER.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-16 13:02:42.000000 spiderYa-0.0.4/spider/SpatialDE/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      802 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/SpatialDE/__init__.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-16 13:02:42.000000 spiderYa-0.0.4/spider/SpatialDE/_internal/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        1 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/SpatialDE/_internal/__init__.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1156 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/SpatialDE/_internal/distance_cache.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11731 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/SpatialDE/_internal/gpflow_helpers.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3326 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/SpatialDE/_internal/kernels.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11116 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/SpatialDE/_internal/models.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1150 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/SpatialDE/_internal/optimizer.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     9297 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/SpatialDE/_internal/score_test.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     5569 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/SpatialDE/_internal/sm_kernel.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11625 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/SpatialDE/_internal/svca.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1762 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/SpatialDE/_internal/tf_dataset.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3700 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/SpatialDE/_internal/util.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2067 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/SpatialDE/_internal/util_mixture.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    14715 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/SpatialDE/aeh.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     8305 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/SpatialDE/de_test.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    16006 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/SpatialDE/dp_hmrf.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    13415 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/SpatialDE/gaussian_process.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3323 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/SpatialDE/io.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     6818 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/SpatialDE/svca.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       43 2023-04-16 08:57:16.000000 spiderYa-0.0.4/spider/__init__.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2866 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/clustering.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     9892 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/enrichment.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-16 13:02:42.000000 spiderYa-0.0.4/spider/lrdb/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/lrdb/__init__.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    13867 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/preprocess.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    26029 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/svi.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      996 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/trajectory.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2716 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/util.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       21 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/version.py
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    12002 2023-04-16 08:56:05.000000 spiderYa-0.0.4/spider/visualization.py
-drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-16 13:02:42.000000 spiderYa-0.0.4/spiderYa.egg-info/
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      570 2023-04-16 13:02:42.000000 spiderYa-0.0.4/spiderYa.egg-info/PKG-INFO
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1083 2023-04-16 13:02:42.000000 spiderYa-0.0.4/spiderYa.egg-info/SOURCES.txt
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        1 2023-04-16 13:02:42.000000 spiderYa-0.0.4/spiderYa.egg-info/dependency_links.txt
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      442 2023-04-16 13:02:42.000000 spiderYa-0.0.4/spiderYa.egg-info/requires.txt
--rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        7 2023-04-16 13:02:42.000000 spiderYa-0.0.4/spiderYa.egg-info/top_level.txt
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-16 13:12:13.000000 spiderYa-0.0.5/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1068 2023-04-16 08:59:14.000000 spiderYa-0.0.5/LICENSE
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      570 2023-04-16 13:12:13.000000 spiderYa-0.0.5/PKG-INFO
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      170 2023-04-16 08:58:58.000000 spiderYa-0.0.5/README.md
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       78 2023-04-16 13:12:13.000000 spiderYa-0.0.5/setup.cfg
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1403 2023-04-16 13:12:06.000000 spiderYa-0.0.5/setup.py
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-16 13:12:13.000000 spiderYa-0.0.5/spider/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     8196 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/SPIDER.py
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-16 13:12:13.000000 spiderYa-0.0.5/spider/SpatialDE/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      802 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/SpatialDE/__init__.py
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-16 13:12:13.000000 spiderYa-0.0.5/spider/SpatialDE/_internal/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        1 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/SpatialDE/_internal/__init__.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1156 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/SpatialDE/_internal/distance_cache.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11731 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/SpatialDE/_internal/gpflow_helpers.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3326 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/SpatialDE/_internal/kernels.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11116 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/SpatialDE/_internal/models.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1150 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/SpatialDE/_internal/optimizer.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     9297 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/SpatialDE/_internal/score_test.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     5569 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/SpatialDE/_internal/sm_kernel.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    11625 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/SpatialDE/_internal/svca.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1762 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/SpatialDE/_internal/tf_dataset.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3700 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/SpatialDE/_internal/util.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2067 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/SpatialDE/_internal/util_mixture.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    14715 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/SpatialDE/aeh.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     8305 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/SpatialDE/de_test.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    16006 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/SpatialDE/dp_hmrf.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    13415 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/SpatialDE/gaussian_process.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     3323 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/SpatialDE/io.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     6818 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/SpatialDE/svca.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       43 2023-04-16 08:57:16.000000 spiderYa-0.0.5/spider/__init__.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2866 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/clustering.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     9892 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/enrichment.py
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-16 13:12:13.000000 spiderYa-0.0.5/spider/lrdb/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/lrdb/__init__.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    13867 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/preprocess.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    26029 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/svi.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      996 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/trajectory.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     2716 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/util.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)       21 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/version.py
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)    12002 2023-04-16 08:56:05.000000 spiderYa-0.0.5/spider/visualization.py
+drwxrwxr-x   0 xuezhengyang  (1069) xuezhengyang  (1069)        0 2023-04-16 13:12:13.000000 spiderYa-0.0.5/spiderYa.egg-info/
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      570 2023-04-16 13:12:13.000000 spiderYa-0.0.5/spiderYa.egg-info/PKG-INFO
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)     1083 2023-04-16 13:12:13.000000 spiderYa-0.0.5/spiderYa.egg-info/SOURCES.txt
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        1 2023-04-16 13:12:13.000000 spiderYa-0.0.5/spiderYa.egg-info/dependency_links.txt
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)      442 2023-04-16 13:12:13.000000 spiderYa-0.0.5/spiderYa.egg-info/requires.txt
+-rw-rw-r--   0 xuezhengyang  (1069) xuezhengyang  (1069)        7 2023-04-16 13:12:13.000000 spiderYa-0.0.5/spiderYa.egg-info/top_level.txt
```

### Comparing `spiderYa-0.0.4/LICENSE` & `spiderYa-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/PKG-INFO` & `spiderYa-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiderYa
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Example Author
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spiderYa-0.0.4/setup.py` & `spiderYa-0.0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="spiderYa",
-    version="0.0.4",
+    version="0.0.5",
     author="Example Author",
     author_email="author@example.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     
     install_requires=[
-        'anndata==0.8.0',
-        'cellrank==1.5.2',
-        'fa2==0.3.5',
-        'gseapy==1.0.3',
-        'h5py==3.7.0',
-        'igraph==0.9.11',
-        'leidenalg==0.8.10',
-        'louvain==0.7.1',
-        'matplotlib==3.6.3',
-        'matplotlib-venn==0.11.7',
-        'networkx==2.8.8',
-        'numba==0.56.4',
-        'numpy==1.23.5',
-        'pandas==1.5.2',
-        'plotly==5.10.0',
-        'pygco==0.0.16',
-        'scanpy==1.9.1',
-        'scgco==1.1.2',
-        'scikit-learn==1.2.0',
-        'scipy==1.10.0',
-        'scvelo==0.2.5',
-        'seaborn==0.12.2',
-        'sklearn==0.0',
-        'somde==0.1.8',
-        'somoclu==1.7.5.1',
-        'spaotsc==0.2',
-        'spatialde==1.1.3',
-        'stlearn==0.4.8',
-        'umap-learn==0.5.3'
+        'anndata>=0.8.0',
+        'cellrank>=1.5.2',
+        'fa2>=0.3.5',
+        'gseapy>=1.0.3',
+        'h5py>=3.7.0',
+        'igraph>=0.9.11',
+        'leidenalg>=0.8.10',
+        'louvain>=0.7.1',
+        'matplotlib>=3.6.3',
+        'matplotlib-venn>=0.11.7',
+        'networkx>=2.8.8',
+        'numba>=0.56.4',
+        'numpy>=1.23.5',
+        'pandas>=1.5.2',
+        'plotly>=5.10.0',
+        'pygco>=0.0.16',
+        'scanpy>=1.9.1',
+        'scgco>=1.1.2',
+        'scikit-learn>=1.2.0',
+        'scipy>=1.10.0',
+        'scvelo>=0.2.5',
+        'seaborn>=0.12.2',
+        'sklearn>=0.0',
+        'somde>=0.1.8',
+        'somoclu>=1.7.5.1',
+        'spaotsc>=0.2',
+        'spatialde>=1.1.3',
+        'stlearn>=0.4.8',
+        'umap-learn>=0.5.3'
     ],
 )
```

### Comparing `spiderYa-0.0.4/spider/SPIDER.py` & `spiderYa-0.0.5/spider/SPIDER.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/SpatialDE/__init__.py` & `spiderYa-0.0.5/spider/SpatialDE/__init__.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/SpatialDE/_internal/distance_cache.py` & `spiderYa-0.0.5/spider/SpatialDE/_internal/distance_cache.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/SpatialDE/_internal/gpflow_helpers.py` & `spiderYa-0.0.5/spider/SpatialDE/_internal/gpflow_helpers.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/SpatialDE/_internal/kernels.py` & `spiderYa-0.0.5/spider/SpatialDE/_internal/kernels.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/SpatialDE/_internal/models.py` & `spiderYa-0.0.5/spider/SpatialDE/_internal/models.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/SpatialDE/_internal/optimizer.py` & `spiderYa-0.0.5/spider/SpatialDE/_internal/optimizer.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/SpatialDE/_internal/score_test.py` & `spiderYa-0.0.5/spider/SpatialDE/_internal/score_test.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/SpatialDE/_internal/sm_kernel.py` & `spiderYa-0.0.5/spider/SpatialDE/_internal/sm_kernel.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/SpatialDE/_internal/svca.py` & `spiderYa-0.0.5/spider/SpatialDE/_internal/svca.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/SpatialDE/_internal/tf_dataset.py` & `spiderYa-0.0.5/spider/SpatialDE/_internal/tf_dataset.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/SpatialDE/_internal/util.py` & `spiderYa-0.0.5/spider/SpatialDE/_internal/util.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/SpatialDE/_internal/util_mixture.py` & `spiderYa-0.0.5/spider/SpatialDE/_internal/util_mixture.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/SpatialDE/aeh.py` & `spiderYa-0.0.5/spider/SpatialDE/aeh.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/SpatialDE/de_test.py` & `spiderYa-0.0.5/spider/SpatialDE/de_test.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/SpatialDE/dp_hmrf.py` & `spiderYa-0.0.5/spider/SpatialDE/dp_hmrf.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/SpatialDE/gaussian_process.py` & `spiderYa-0.0.5/spider/SpatialDE/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/SpatialDE/io.py` & `spiderYa-0.0.5/spider/SpatialDE/io.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/SpatialDE/svca.py` & `spiderYa-0.0.5/spider/SpatialDE/svca.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/clustering.py` & `spiderYa-0.0.5/spider/clustering.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/enrichment.py` & `spiderYa-0.0.5/spider/enrichment.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/preprocess.py` & `spiderYa-0.0.5/spider/preprocess.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/svi.py` & `spiderYa-0.0.5/spider/svi.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/trajectory.py` & `spiderYa-0.0.5/spider/trajectory.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/util.py` & `spiderYa-0.0.5/spider/util.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spider/visualization.py` & `spiderYa-0.0.5/spider/visualization.py`

 * *Files identical despite different names*

### Comparing `spiderYa-0.0.4/spiderYa.egg-info/PKG-INFO` & `spiderYa-0.0.5/spiderYa.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spiderYa
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: Example Author
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spiderYa-0.0.4/spiderYa.egg-info/SOURCES.txt` & `spiderYa-0.0.5/spiderYa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

