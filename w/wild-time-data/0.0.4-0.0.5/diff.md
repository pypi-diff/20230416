# Comparing `tmp/wild_time_data-0.0.4.tar.gz` & `tmp/wild_time_data-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wild_time_data-0.0.4.tar", last modified: Mon Apr  3 16:40:48 2023, max compression
+gzip compressed data, was "wild_time_data-0.0.5.tar", last modified: Sun Apr 16 07:31:51 2023, max compression
```

## Comparing `wild_time_data-0.0.4.tar` & `wild_time_data-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:40:48.479678 wild_time_data-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:40:48.475678 wild_time_data-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:40:48.479678 wild_time_data-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-03 16:40:35.000000 wild_time_data-0.0.4/.github/workflows/pypi_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-03 16:40:35.000000 wild_time_data-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-03 16:40:35.000000 wild_time_data-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-03 16:40:48.479678 wild_time_data-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-03 16:40:35.000000 wild_time_data-0.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-03 16:40:35.000000 wild_time_data-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-03 16:40:35.000000 wild_time_data-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 16:40:48.479678 wild_time_data-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:40:48.479678 wild_time_data-0.0.4/wild_time_data/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-03 16:40:35.000000 wild_time_data-0.0.4/wild_time_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-03 16:40:35.000000 wild_time_data-0.0.4/wild_time_data/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-04-03 16:40:35.000000 wild_time_data-0.0.4/wild_time_data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-03 16:40:35.000000 wild_time_data-0.0.4/wild_time_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 16:40:48.479678 wild_time_data-0.0.4/wild_time_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-03 16:40:48.000000 wild_time_data-0.0.4/wild_time_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-03 16:40:48.000000 wild_time_data-0.0.4/wild_time_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 16:40:48.000000 wild_time_data-0.0.4/wild_time_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-03 16:40:48.000000 wild_time_data-0.0.4/wild_time_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-03 16:40:48.000000 wild_time_data-0.0.4/wild_time_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)   255896 2023-04-03 16:40:35.000000 wild_time_data-0.0.4/yearbook.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:31:51.996630 wild_time_data-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:31:51.992629 wild_time_data-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:31:51.992629 wild_time_data-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/.github/workflows/pypi_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-16 07:31:51.992629 wild_time_data-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 07:31:51.996630 wild_time_data-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:31:51.992629 wild_time_data-0.0.5/wild_time_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/wild_time_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/wild_time_data/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/wild_time_data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/wild_time_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 07:31:51.992629 wild_time_data-0.0.5/wild_time_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-16 07:31:51.000000 wild_time_data-0.0.5/wild_time_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-16 07:31:51.000000 wild_time_data-0.0.5/wild_time_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 07:31:51.000000 wild_time_data-0.0.5/wild_time_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-16 07:31:51.000000 wild_time_data-0.0.5/wild_time_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-16 07:31:51.000000 wild_time_data-0.0.5/wild_time_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   255896 2023-04-16 07:31:42.000000 wild_time_data-0.0.5/yearbook.png
```

### Comparing `wild_time_data-0.0.4/.github/workflows/pypi_publish.yml` & `wild_time_data-0.0.5/.github/workflows/pypi_publish.yml`

 * *Files identical despite different names*

### Comparing `wild_time_data-0.0.4/.gitignore` & `wild_time_data-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `wild_time_data-0.0.4/LICENSE` & `wild_time_data-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wild_time_data-0.0.4/PKG-INFO` & `wild_time_data-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wild_time_data
-Version: 0.0.4
+Version: 0.0.5
 Summary: WILDS distribution shift data
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wild_time_data-0.0.4/README.rst` & `wild_time_data-0.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `wild_time_data-0.0.4/pyproject.toml` & `wild_time_data-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wild_time_data-0.0.4/wild_time_data/core.py` & `wild_time_data-0.0.5/wild_time_data/core.py`

 * *Files identical despite different names*

### Comparing `wild_time_data-0.0.4/wild_time_data/datasets.py` & `wild_time_data-0.0.5/wild_time_data/datasets.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy as np
 import torch
 from PIL import Image
 from torch.utils.data import Dataset
 from torchvision import transforms
 from wilds import get_dataset
 
-from wild_time_data.utils import embed_drug, embed_protein, maybe_download
+from wild_time_data.utils import maybe_download
 
 
 class WildTimeDataset(Dataset, ABC):
     def __init__(self, time_step, split, data_dir):
         super().__init__()
         if time_step not in self.time_steps:
             raise ValueError(f"Unknown time `{time_step}. Choose a time_step in {self.time_steps}")
@@ -61,28 +61,49 @@
 
 class Drug(WildTimeDataset):
     time_steps = [i for i in range(2013, 2021)]
     input_dim = [(63, 100), (26, 1000)]
     num_classes = 1
     drive_id = "12SmQXA6f1fPd9__WAY8lravVAlDsFP7p"
     file_name = "drug.pkl"
+    mapping_amino = {key: value for value, key in enumerate("?ABCDEFGHIKLMNOPQRSTUVWXYZ")}
+    mapping_smiles = {
+        key: value
+        for value, key in enumerate(
+            "#%()+-.0123456789=?ABCDEFGHIKLMNOPRSTUVWYZ[]_abcdefghilmnorstuy"
+        )
+    }
+
+    @classmethod
+    def _transform_protein(cls, x):
+        tensor = torch.zeros((26, 1000))
+        for i, c in enumerate(x):
+            tensor[Drug.mapping_amino[c], i] = 1
+        return tensor
+
+    @classmethod
+    def _transform_drug(cls, x):
+        tensor = torch.zeros((63, 100))
+        for i, c in enumerate(x):
+            tensor[Drug.mapping_smiles[c], i] = 1
+        return tensor
 
     def __getitem__(self, index):
         return (
-            embed_drug(self._dataset.iloc[index].Drug_Enc),
-            embed_protein(self._dataset.iloc[index].Target_Enc),
-        ), self._dataset.iloc[index].Y
+            Drug._transform_drug(self._dataset.iloc[index].Drug_Enc),
+            Drug._transform_protein(self._dataset.iloc[index].Target_Enc),
+        ), torch.FloatTensor(self._dataset.iloc[index].Y)[0]
 
     def __len__(self):
         return len(self._dataset)
 
 
 class FMoW(WildTimeImageDataset):
-    time_steps = [i for i in range(16)]
-    input_dim = (3, 32, 32)
+    time_steps = list(range(16))
+    input_dim = (3, 224, 224)
     num_classes = 62
     drive_id = "1s_xtf2M5EC7vIFhNv_OulxZkNvrVwIm3"
     file_name = "fmow.pkl"
 
     def __init__(self, time_step, split, data_dir):
         super().__init__(time_step, split, data_dir)
         self._transform = transforms.Compose(
@@ -90,17 +111,17 @@
                 transforms.ToTensor(),
                 transforms.Normalize([0.485, 0.456, 0.406], [0.229, 0.224, 0.225]),
             ]
         )
         self._root = get_dataset(dataset="fmow", root_dir=data_dir, download=True).root
 
     def __getitem__(self, idx):
-        idx = self._dataset["image_idxs"][idx]
-        img = Image.open(self._root / "images" / f"rgb_img_{idx}.png").convert("RGB")
-        image = self._transform(img)
+        image_idx = self._dataset["image_idxs"][idx]
+        image = Image.open(self._root / "images" / f"rgb_img_{image_idx}.png").convert("RGB")
+        image = self._transform(image)
         label = torch.LongTensor([self._dataset["labels"][idx]])[0]
         return image, label
 
 
 class HuffPost(WildTimeTextDataset):
     time_steps = [i for i in range(2012, 2019)]
     input_dim = 44
@@ -117,12 +138,19 @@
     input_dim = (1, 32, 32)
     num_classes = 2
     drive_id = "1mPpxoX2y2oijOvW1ymiHEYd7oMu2vVRb"
     file_name = "yearbook.pkl"
 
     def __init__(self, time_step, split, data_dir):
         super().__init__(time_step, split, data_dir)
-        self._images = torch.FloatTensor(np.array([img.transpose(2, 0, 1)[0].reshape(*self.input_dim) for img in self._dataset["images"]]))
+        self._images = torch.FloatTensor(
+            np.array(
+                [
+                    img.transpose(2, 0, 1)[0].reshape(*self.input_dim)
+                    for img in self._dataset["images"]
+                ]
+            )
+        )
         self._labels = torch.LongTensor(self._dataset["labels"])
 
     def __getitem__(self, idx):
         return self._images[idx], self._labels[idx]
```

### Comparing `wild_time_data-0.0.4/wild_time_data.egg-info/PKG-INFO` & `wild_time_data-0.0.5/wild_time_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wild-time-data
-Version: 0.0.4
+Version: 0.0.5
 Summary: WILDS distribution shift data
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wild_time_data-0.0.4/yearbook.png` & `wild_time_data-0.0.5/yearbook.png`

 * *Files identical despite different names*

