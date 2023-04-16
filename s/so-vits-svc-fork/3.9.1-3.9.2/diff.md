# Comparing `tmp/so_vits_svc_fork-3.9.1.tar.gz` & `tmp/so_vits_svc_fork-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork-3.9.1.tar", max compression
+gzip compressed data, was "so_vits_svc_fork-3.9.2.tar", max compression
```

## Comparing `so_vits_svc_fork-3.9.1.tar` & `so_vits_svc_fork-3.9.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    12463 2023-04-16 05:32:37.384638 so_vits_svc_fork-3.9.1/LICENSE
--rw-r--r--   0        0        0    18160 2023-04-16 05:32:37.384638 so_vits_svc_fork-3.9.1/README.md
--rw-r--r--   0        0        0     3092 2023-04-16 05:32:38.364642 so_vits_svc_fork-3.9.1/pyproject.toml
--rw-r--r--   0        0        0       70 2023-04-16 05:32:38.316642 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    22740 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1393 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     2844 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2868 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2454 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7267 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    25663 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      864 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    24054 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     7485 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0     1341 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    16683 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     4620 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1419 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       76 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11618 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      340 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      318 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12477 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      419 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4725 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     8954 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     4879 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5604 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4400 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1390 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1405 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5753 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14435 2023-04-16 05:32:37.388638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8178 2023-04-16 05:32:37.392638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2023-04-16 05:32:37.392638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     1737 2023-04-16 05:32:37.392638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1487 2023-04-16 05:32:37.392638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1548 2023-04-16 05:32:37.392638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     2793 2023-04-16 05:32:37.392638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4646 2023-04-16 05:32:37.392638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4382 2023-04-16 05:32:37.392638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     2948 2023-04-16 05:32:37.392638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     1878 2023-04-16 05:32:37.392638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      126 2023-04-16 05:32:37.392638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2023-04-16 05:32:37.392638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    20095 2023-04-16 05:32:37.392638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    13313 2023-04-16 05:32:37.392638 so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    20087 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.9.1/PKG-INFO
+-rw-r--r--   0        0        0    12463 2023-04-16 09:02:51.966997 so_vits_svc_fork-3.9.2/LICENSE
+-rw-r--r--   0        0        0    18160 2023-04-16 09:02:51.966997 so_vits_svc_fork-3.9.2/README.md
+-rw-r--r--   0        0        0     3092 2023-04-16 09:02:53.070997 so_vits_svc_fork-3.9.2/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-04-16 09:02:53.022997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    22740 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1393 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     2844 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2868 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2454 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7267 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    25663 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      864 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    24054 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     7485 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0     1341 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    16683 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     4620 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1419 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       76 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11618 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      340 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      318 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12477 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      419 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4725 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     8954 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     4879 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5604 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4400 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1390 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1405 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5753 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14435 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8178 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     1737 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1487 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1548 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     2793 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4646 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4382 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     2948 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     1878 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      126 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    20145 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    13313 2023-04-16 09:02:51.970997 so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    20087 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.9.2/PKG-INFO
```

### Comparing `so_vits_svc_fork-3.9.1/LICENSE` & `so_vits_svc_fork-3.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/README.md` & `so_vits_svc_fork-3.9.2/README.md`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/pyproject.toml` & `so_vits_svc_fork-3.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork"
-version = "3.9.1"
+version = "3.9.2"
 description = "A fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/so-vits-svc-fork"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
```

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/__main__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/gui.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/inference/core.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/inference/main.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/logger.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,14 +366,15 @@
         ) = self.net_g(c, f0, uv, spec, g=g, c_lengths=lengths, spec_lengths=lengths)
         y_mel = commons.slice_segments(
             mel,
             ids_slice,
             self.hparams.train.segment_size // self.hparams.data.hop_length,
         )
         y_hat_mel = mel_spectrogram_torch(y_hat.squeeze(1), self.hparams)
+        y_mel = y_mel[..., : y_hat_mel.shape[-1]]
         y = commons.slice_segments(
             y,
             ids_slice * self.hparams.data.hop_length,
             self.hparams.train.segment_size,
         )
         y = y[..., : y_hat.shape[-1]]
```

### Comparing `so_vits_svc_fork-3.9.1/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork-3.9.2/src/so_vits_svc_fork/utils.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.1/PKG-INFO` & `so_vits_svc_fork-3.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: so-vits-svc-fork
-Version: 3.9.1
+Version: 3.9.2
 Summary: A fork of so-vits-svc.
 Home-page: https://github.com/34j/so-vits-svc-fork
 License: MIT
 Author: 34j
 Author-email: 34j.95a2p@simplelogin.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.9.1 Summary: A fork of
+Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.9.2 Summary: A fork of
 so-vits-svc. Home-page: https://github.com/34j/so-vits-svc-fork License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

