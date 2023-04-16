# Comparing `tmp/so_vits_svc_fork-3.8.1.tar.gz` & `tmp/so_vits_svc_fork-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork-3.8.1.tar", max compression
+gzip compressed data, was "so_vits_svc_fork-3.9.0.tar", max compression
```

## Comparing `so_vits_svc_fork-3.8.1.tar` & `so_vits_svc_fork-3.9.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    12463 2023-04-16 04:30:19.739066 so_vits_svc_fork-3.8.1/LICENSE
--rw-r--r--   0        0        0    18160 2023-04-16 04:30:19.739066 so_vits_svc_fork-3.8.1/README.md
--rw-r--r--   0        0        0     3092 2023-04-16 04:30:20.875066 so_vits_svc_fork-3.8.1/pyproject.toml
--rw-r--r--   0        0        0       70 2023-04-16 04:30:20.819066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    22740 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1352 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     2844 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2868 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2454 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7267 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    25663 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      864 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    24054 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     7485 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0     1341 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    16683 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     5854 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1419 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       76 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11618 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      340 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      318 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12477 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      419 2023-04-16 04:30:19.743066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4725 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     8954 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     4879 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5604 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4400 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1390 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1405 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5753 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14435 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8178 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     1671 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1421 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1482 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     2793 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4646 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4382 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     2948 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     1878 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      126 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    19861 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    13313 2023-04-16 04:30:19.747066 so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    20087 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.8.1/PKG-INFO
+-rw-r--r--   0        0        0    12463 2023-04-16 04:37:48.268783 so_vits_svc_fork-3.9.0/LICENSE
+-rw-r--r--   0        0        0    18160 2023-04-16 04:37:48.268783 so_vits_svc_fork-3.9.0/README.md
+-rw-r--r--   0        0        0     3092 2023-04-16 04:37:49.584802 so_vits_svc_fork-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-04-16 04:37:49.516801 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    22740 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1352 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     2844 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2868 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2454 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7267 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    25663 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      864 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    24054 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     7485 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0     1341 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    16683 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     5854 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1419 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       76 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11618 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      340 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      318 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12477 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      419 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4725 2023-04-16 04:37:48.272784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     8954 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     4879 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5604 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4400 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1390 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1405 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5753 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14435 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8178 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     1737 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1487 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1548 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     2793 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4646 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4382 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     2948 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     1878 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      126 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    20057 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    13313 2023-04-16 04:37:48.276784 so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    20087 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.9.0/PKG-INFO
```

### Comparing `so_vits_svc_fork-3.8.1/LICENSE` & `so_vits_svc_fork-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/README.md` & `so_vits_svc_fork-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/pyproject.toml` & `so_vits_svc_fork-3.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork"
-version = "3.8.1"
+version = "3.9.0"
 description = "A fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/so-vits-svc-fork"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
```

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/__main__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/dataset.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/gui.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/inference/core.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/inference/main.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/logger.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910714285714286%*

 * *Differences: {"'train'": "{'ckpt_name_by_step': False, 'accumulate_grad_batches': 1}"}*

```diff
@@ -60,22 +60,24 @@
             8,
             4
         ],
         "use_spectral_norm": false
     },
     "spk": {},
     "train": {
+        "accumulate_grad_batches": 1,
         "batch_size": 16,
         "betas": [
             0.8,
             0.99
         ],
         "bf16_run": false,
         "c_kl": 1.0,
         "c_mel": 45,
+        "ckpt_name_by_step": false,
         "epochs": 10000,
         "eps": 1e-09,
         "eval_interval": 200,
         "fft_sizes": [
             768,
             1366,
             342
```

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333333%*

 * *Differences: {"'train'": "{'ckpt_name_by_step': False, 'accumulate_grad_batches': 1}"}*

```diff
@@ -61,22 +61,24 @@
             2,
             2
         ],
         "use_spectral_norm": false
     },
     "spk": {},
     "train": {
+        "accumulate_grad_batches": 1,
         "batch_size": 16,
         "betas": [
             0.8,
             0.99
         ],
         "bf16_run": false,
         "c_kl": 1.0,
         "c_mel": 45,
+        "ckpt_name_by_step": false,
         "epochs": 10000,
         "eps": 1e-09,
         "eval_interval": 800,
         "fp16_run": false,
         "init_lr_ratio": 1,
         "keep_ckpts": 3,
         "learning_rate": 0.0001,
```

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9895833333333333%*

 * *Differences: {"'train'": "{'ckpt_name_by_step': False, 'accumulate_grad_batches': 1}"}*

```diff
@@ -63,22 +63,24 @@
             2,
             2
         ],
         "use_spectral_norm": false
     },
     "spk": {},
     "train": {
+        "accumulate_grad_batches": 1,
         "batch_size": 16,
         "betas": [
             0.8,
             0.99
         ],
         "bf16_run": false,
         "c_kl": 1.0,
         "c_mel": 45,
+        "ckpt_name_by_step": false,
         "epochs": 10000,
         "eps": 1e-09,
         "eval_interval": 200,
         "fp16_run": false,
         "init_lr_ratio": 1,
         "keep_ckpts": 3,
         "learning_rate": 0.0001,
```

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -501,22 +501,24 @@
             if self.current_epoch == 0 or batch_idx != 0:
                 return
             utils.save_checkpoint(
                 self.net_g,
                 self.optim_g,
                 self.learning_rate,
                 self.current_epoch + 1,  # prioritize prevention of undervaluation
-                Path(self.hparams.model_dir) / f"G_{self.total_batch_idx}.pth",
+                Path(self.hparams.model_dir)
+                / f"G_{self.total_batch_idx if self.hparams.train.get('ckpt_name_by_step', False) else self.current_epoch + 1}.pth",
             )
             utils.save_checkpoint(
                 self.net_d,
                 self.optim_d,
                 self.learning_rate,
                 self.current_epoch + 1,
-                Path(self.hparams.model_dir) / f"D_{self.total_batch_idx}.pth",
+                Path(self.hparams.model_dir)
+                / f"D_{self.total_batch_idx if self.hparams.train.get('ckpt_name_by_step', False) else self.current_epoch + 1}.pth",
             )
             keep_ckpts = self.hparams.train.get("keep_ckpts", 0)
             if keep_ckpts > 0:
                 utils.clean_checkpoints(
                     path_to_models=self.hparams.model_dir,
                     n_ckpts_to_keep=keep_ckpts,
                     sort_by_time=True,
```

### Comparing `so_vits_svc_fork-3.8.1/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork-3.9.0/src/so_vits_svc_fork/utils.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.8.1/PKG-INFO` & `so_vits_svc_fork-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: so-vits-svc-fork
-Version: 3.8.1
+Version: 3.9.0
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
-Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.8.1 Summary: A fork of
+Metadata-Version: 2.1 Name: so-vits-svc-fork Version: 3.9.0 Summary: A fork of
 so-vits-svc. Home-page: https://github.com/34j/so-vits-svc-fork License: MIT
 Author: 34j Author-email: 34j.95a2p@simplelogin.com Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

