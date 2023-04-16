# Comparing `tmp/monai-weekly-1.2.dev2315.tar.gz` & `tmp/monai-weekly-1.2.dev2316.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monai-weekly-1.2.dev2315.tar", last modified: Sun Apr  9 02:19:26 2023, max compression
+gzip compressed data, was "monai-weekly-1.2.dev2316.tar", last modified: Sun Apr 16 02:21:48 2023, max compression
```

## Comparing `monai-weekly-1.2.dev2315.tar` & `monai-weekly-1.2.dev2316.tar`

### file list

```diff
@@ -1,1131 +1,1133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:26.006656 monai-weekly-1.2.dev2315/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-04-09 02:19:26.006656 monai-weekly-1.2.dev2315/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:26.010656 monai-weekly-1.2.dev2315/monai/
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-09 02:17:16.000000 monai-weekly-1.2.dev2315/monai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.286658 monai-weekly-1.2.dev2315/monai/_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/_extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.286658 monai-weekly-1.2.dev2315/monai/_extensions/gmm/
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/_extensions/gmm/gmm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/_extensions/gmm/gmm.h
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/_extensions/gmm/gmm_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/_extensions/gmm/gmm_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/_extensions/gmm/gmm_cuda_linalg.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/_extensions/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-09 02:19:26.010656 monai-weekly-1.2.dev2315/monai/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.290658 monai-weekly-1.2.dev2315/monai/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.294658 monai-weekly-1.2.dev2315/monai/apps/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/auto3dseg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36120 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/auto3dseg/auto_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    23180 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/auto3dseg/bundle_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    13587 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/auto3dseg/data_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/auto3dseg/ensemble_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17563 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/auto3dseg/hpo_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/auto3dseg/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/auto3dseg/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34560 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.294658 monai-weekly-1.2.dev2315/monai/apps/deepedit/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/deepedit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/deepedit/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    37435 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/deepedit/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.298658 monai-weekly-1.2.dev2315/monai/apps/deepgrow/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/deepgrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/deepgrow/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/deepgrow/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    42011 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/deepgrow/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.298658 monai-weekly-1.2.dev2315/monai/apps/detection/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/detection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.302658 monai-weekly-1.2.dev2315/monai/apps/detection/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/detection/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26617 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/detection/metrics/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/detection/metrics/matching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.302658 monai-weekly-1.2.dev2315/monai/apps/detection/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/detection/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51663 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/detection/networks/retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/detection/networks/retinanet_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.306658 monai-weekly-1.2.dev2315/monai/apps/detection/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/detection/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24519 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/detection/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/detection/transforms/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    68979 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/detection/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.310658 monai-weekly-1.2.dev2315/monai/apps/detection/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/detection/utils/ATSS_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/detection/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18681 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/detection/utils/anchor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/detection/utils/box_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/detection/utils/box_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/detection/utils/detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/detection/utils/hard_negative_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/detection/utils/predict_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.314658 monai-weekly-1.2.dev2315/monai/apps/mmars/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/mmars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/mmars/mmars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/mmars/model_desc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.314658 monai-weekly-1.2.dev2315/monai/apps/nnunet/
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/nnunet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/nnunet/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38587 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/nnunet/nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/nnunet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.314658 monai-weekly-1.2.dev2315/monai/apps/nuclick/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/nuclick/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/nuclick/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.318658 monai-weekly-1.2.dev2315/monai/apps/pathology/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/pathology/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.318658 monai-weekly-1.2.dev2315/monai/apps/pathology/engines/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/pathology/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/pathology/engines/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.318658 monai-weekly-1.2.dev2315/monai/apps/pathology/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/pathology/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/pathology/handlers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.318658 monai-weekly-1.2.dev2315/monai/apps/pathology/inferers/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/pathology/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/pathology/inferers/inferer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.322658 monai-weekly-1.2.dev2315/monai/apps/pathology/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/pathology/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/pathology/losses/hovernet_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.322658 monai-weekly-1.2.dev2315/monai/apps/pathology/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/pathology/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/pathology/metrics/lesion_froc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.322658 monai-weekly-1.2.dev2315/monai/apps/pathology/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/pathology/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.326658 monai-weekly-1.2.dev2315/monai/apps/pathology/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/pathology/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36850 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/pathology/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    25716 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/pathology/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.326658 monai-weekly-1.2.dev2315/monai/apps/pathology/transforms/stain/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/pathology/transforms/stain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/pathology/transforms/stain/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/pathology/transforms/stain/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/pathology/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.330658 monai-weekly-1.2.dev2315/monai/apps/reconstruction/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/reconstruction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/reconstruction/complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/reconstruction/fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/reconstruction/mri_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.330658 monai-weekly-1.2.dev2315/monai/apps/reconstruction/networks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/reconstruction/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.330658 monai-weekly-1.2.dev2315/monai/apps/reconstruction/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/reconstruction/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/reconstruction/networks/blocks/varnetblock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.334658 monai-weekly-1.2.dev2315/monai/apps/reconstruction/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/reconstruction/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/reconstruction/networks/nets/complex_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/reconstruction/networks/nets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/reconstruction/networks/nets/varnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.334658 monai-weekly-1.2.dev2315/monai/apps/reconstruction/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/reconstruction/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/reconstruction/transforms/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    15844 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/reconstruction/transforms/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.338658 monai-weekly-1.2.dev2315/monai/apps/tcia/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/tcia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/tcia/label_desc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/tcia/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/apps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.342658 monai-weekly-1.2.dev2315/monai/auto3dseg/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/auto3dseg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/auto3dseg/algo_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)    41223 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/auto3dseg/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/auto3dseg/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/auto3dseg/seg_summarizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12193 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/auto3dseg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.346658 monai-weekly-1.2.dev2315/monai/bundle/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/bundle/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16035 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/bundle/config_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/bundle/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/bundle/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/bundle/reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    61643 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/bundle/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/bundle/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/bundle/workflows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.350658 monai-weekly-1.2.dev2315/monai/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/config/deviceconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/config/type_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.370658 monai-weekly-1.2.dev2315/monai/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50102 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    68927 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    60619 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    39872 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/image_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/meta_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    27125 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/test_time_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    64795 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/video_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18631 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/wsi_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    38749 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/data/wsi_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.378658 monai-weekly-1.2.dev2315/monai/engines/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24568 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/engines/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/engines/multi_gpu_supervised_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    21347 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/engines/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/engines/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/engines/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.378658 monai-weekly-1.2.dev2315/monai/fl/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/fl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.378658 monai-weekly-1.2.dev2315/monai/fl/client/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/fl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/fl/client/client_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)    32635 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/fl/client/monai_algo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.382658 monai-weekly-1.2.dev2315/monai/fl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/fl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/fl/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/fl/utils/exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/fl/utils/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.410658 monai-weekly-1.2.dev2315/monai/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/clearml_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/earlystop_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/ignite_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/logfile_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/lr_schedule_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/metrics_reloaded_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/mlflow_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/nvtx_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/probability_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/smartcache_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/stats_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    23325 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/tensorboard_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/handlers/validation_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.414657 monai-weekly-1.2.dev2315/monai/inferers/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/inferers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27881 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/inferers/inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/inferers/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/inferers/splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20044 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/inferers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.426658 monai-weekly-1.2.dev2315/monai/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/losses/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/losses/deform.py
--rw-r--r--   0 runner    (1001) docker     (123)    46326 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/losses/dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/losses/ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/losses/focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/losses/giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/losses/image_dissimilarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/losses/multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/losses/spatial_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/losses/ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/losses/tversky.py
--rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/losses/unified_focal_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.442658 monai-weekly-1.2.dev2315/monai/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/metrics/active_learning_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    15101 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/metrics/confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/metrics/cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/metrics/f_beta_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/metrics/froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/metrics/generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/metrics/hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/metrics/loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/metrics/meandice.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/metrics/meaniou.py
--rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/metrics/panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)    18235 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/metrics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/metrics/rocauc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12166 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/metrics/surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/metrics/surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/metrics/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.442658 monai-weekly-1.2.dev2315/monai/networks/
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.462657 monai-weekly-1.2.dev2315/monai/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/acti_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/backbone_fpn_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/crf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/denseblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/dints_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/feature_pyramid_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/fft_utils_t.py
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/selfattention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/squeeze_and_excitation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/blocks/warp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.470657 monai-weekly-1.2.dev2315/monai/networks/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/layers/convutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/layers/drop_path.py
--rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/layers/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/layers/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/layers/gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    28470 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/layers/simplelayers.py
--rw-r--r--   0 runner    (1001) docker     (123)    25576 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/layers/spatial_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/layers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/layers/weight_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.498657 monai-weekly-1.2.dev2315/monai/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21533 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/ahnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/dints.py
--rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/dynunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    40643 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/highresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/milmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/netadapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17189 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/regunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/segresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/senet.py
--rw-r--r--   0 runner    (1001) docker     (123)    42000 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/torchvision_fc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/transchex.py
--rw-r--r--   0 runner    (1001) docker     (123)    13722 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/nets/vnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    40024 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/networks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.502657 monai-weekly-1.2.dev2315/monai/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21948 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/optimizers/lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/optimizers/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/optimizers/novograd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/optimizers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.514657 monai-weekly-1.2.dev2315/monai/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)    15216 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/adaptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    40532 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/compose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.522657 monai-weekly-1.2.dev2315/monai/transforms/croppad/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/croppad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68728 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/croppad/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/croppad/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    54071 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/croppad/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/croppad/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.522657 monai-weekly-1.2.dev2315/monai/transforms/intensity/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/intensity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    98613 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/intensity/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    76501 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/intensity/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/inverse_batch_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.526657 monai-weekly-1.2.dev2315/monai/transforms/io/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25430 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/io/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/io/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.526657 monai-weekly-1.2.dev2315/monai/transforms/lazy/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/lazy/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/lazy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.530657 monai-weekly-1.2.dev2315/monai/transforms/meta_utility/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/meta_utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/meta_utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/nvtx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.534657 monai-weekly-1.2.dev2315/monai/transforms/post/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/post/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    39905 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/post/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.534657 monai-weekly-1.2.dev2315/monai/transforms/signal/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16378 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/signal/array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.538657 monai-weekly-1.2.dev2315/monai/transforms/smooth_field/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/smooth_field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/smooth_field/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/smooth_field/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.542657 monai-weekly-1.2.dev2315/monai/transforms/spatial/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/spatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   168560 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/spatial/array.py
--rw-r--r--   0 runner    (1001) docker     (123)   107151 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/spatial/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    31494 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/spatial/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.542657 monai-weekly-1.2.dev2315/monai/transforms/utility/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70325 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/utility/array.py
--rw-r--r--   0 runner    (1001) docker     (123)    75816 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/utility/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (123)    71153 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    31081 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/utils_create_transform_ims.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/transforms/utils_pytorch_numpy_unification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.554657 monai-weekly-1.2.dev2315/monai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/utils/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/utils/deprecate_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    16215 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/utils/jupyter_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24927 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/utils/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/utils/nvtx.py
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/utils/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/utils/state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (123)    21127 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/utils/type_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.562657 monai-weekly-1.2.dev2315/monai/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16156 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/visualize/class_activation_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/visualize/gradient_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/visualize/img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/visualize/occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/visualize/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/monai/visualize/visualizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:25.562657 monai-weekly-1.2.dev2315/monai_weekly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-04-09 02:19:25.000000 monai-weekly-1.2.dev2315/monai_weekly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33801 2023-04-09 02:19:25.000000 monai-weekly-1.2.dev2315/monai_weekly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 02:19:25.000000 monai-weekly-1.2.dev2315/monai_weekly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 02:19:25.000000 monai-weekly-1.2.dev2315/monai_weekly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-09 02:19:25.000000 monai-weekly-1.2.dev2315/monai_weekly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-09 02:19:25.000000 monai-weekly-1.2.dev2315/monai_weekly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-04-09 02:19:26.010656 monai-weekly-1.2.dev2315/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 02:19:26.006656 monai-weekly-1.2.dev2315/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_acn_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_activationsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_adaptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_add_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_add_coordinate_channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_add_coordinate_channelsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_add_extreme_points_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_add_extreme_points_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_adn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_affine_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_affined.py
--rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_ahnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_anchor_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_apply.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_apply_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_arraydataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_as_channel_first.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_as_channel_firstd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_as_channel_last.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_as_channel_lastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_as_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_as_discreted.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_atss_box_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_attentionunet.py
--rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_auto3dseg.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_auto3dseg_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_auto3dseg_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_avg_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_basic_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_basic_unetplusplus.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_bending_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_bilateral_approx_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_bilateral_approx_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)    15034 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_bilateral_precise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_blend_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_border_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_border_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_bounding_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_bounding_rectd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_box_coder.py
--rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_box_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_bundle_ckpt_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_bundle_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_bundle_get_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_bundle_init_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_bundle_onnx_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_bundle_trt_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_bundle_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_bundle_verify_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_bundle_verify_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_bundle_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_cachedataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_cachedataset_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_cachedataset_persistent_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_cachentransdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_call_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_cast_to_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_cast_to_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_center_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_center_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_center_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_center_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_channel_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_check_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_check_missing_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_classes_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_complex_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_component_locator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_compose_get_number_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_compute_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_compute_f_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_compute_froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_compute_generalized_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_compute_ho_ver_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_compute_ho_ver_maps_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_compute_meandice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_compute_meaniou.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_compute_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_compute_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_compute_roc_auc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_compute_variance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_concat_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_config_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_contrastive_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_convert_data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_convert_to_multi_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_convert_to_multi_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_convert_to_onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_convert_to_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_convert_to_trt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_copy_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_copy_model_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_correct_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_create_cross_validation_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_create_grid_and_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_crf_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_crf_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_crop_foreground.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_crop_foregroundd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_cross_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_csv_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_csv_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_cumulative.py
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_cumulative_average.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_cumulative_average_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_cv2_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_data_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_data_statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_dataset_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_dataset_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_decathlondataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_decollate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_deepedit_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_deepedit_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_deepgrow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_deepgrow_interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_deepgrow_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_delete_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_denseblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_densenet.py
--rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_detect_envelope.py
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_detection_coco_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_detector_boxselector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_detector_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_dev_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_dice_ce_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_dints_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_dints_mixop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_dints_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_divisible_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_divisible_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_download_and_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_downsample_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_drop_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_ds_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_dvf2ddf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_dynunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_dynunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_ensemble_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_ensure_channel_first.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_ensure_channel_firstd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_ensure_tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_ensure_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_ensure_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_enum_bound_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_eval_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_evenly_divisible_all_gather_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_factorized_increase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_factorized_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_fastmri_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_fft_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_fg_bg_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_fg_bg_to_indicesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_file_basename.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_fill_holes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_fill_holesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_fl_exchange_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_fl_monai_algo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_fl_monai_algo_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_fl_monai_algo_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_flatten_sub_keysd.py
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_flexible_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_folder_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_foreground_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_foreground_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_fourier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_fpn_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_from_engine_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_fullyconnectednet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_gaussian_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generalized_dice_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generalized_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generalized_wasserstein_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generate_distance_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generate_distance_mapd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generate_instance_border.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generate_instance_borderd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generate_instance_centroid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generate_instance_centroidd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generate_instance_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generate_instance_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generate_instance_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generate_instance_typed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generate_label_classes_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generate_param_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generate_pos_neg_label_crop_centers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generate_spatial_bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generate_succinct_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generate_succinct_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generate_watershed_markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generate_watershed_markersd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generate_watershed_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generate_watershed_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_get_equivalent_dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_get_extreme_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_get_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_get_package_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_get_unique_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_giou_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_global_mutual_information_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_globalnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_gmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_grid_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_grid_pull.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_grid_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_grid_splitd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_checkpoint_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_classification_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_classification_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_clearml_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_clearml_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_confusion_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_confusion_matrix_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_decollate_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_early_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_logfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_mean_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_metric_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_metrics_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_metrics_saver_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_mlflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_nvtx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_panoptic_quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_parameter_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_prob_map_producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_regression_metrics_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_rocauc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_rocauc_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_smartcache.py
--rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_tb_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_tb_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_handler_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_hardnegsampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_hausdorff_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_header_correct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_highresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_hilbert_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_histogram_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_histogram_normalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_hovernet_instance_map_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_hovernet_instance_map_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_hovernet_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_hovernet_nuclear_type_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_hovernet_nuclear_type_post_processingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_identityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_image_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_image_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_img2tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_init_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_integration_autorunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_integration_bundle_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_integration_classification_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_integration_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_integration_fast_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_integration_gpu_customization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_integration_lazy_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_integration_nnunetv2_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_integration_segmentation_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_integration_sliding_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_integration_stn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_integration_unet_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_integration_workers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_integration_workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_integration_workflows_gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_intensity_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_intensity_statsd.py
--rw-r--r--   0 runner    (1001) docker     (123)    18873 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_inverse_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_inverse_collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_invert.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_invertd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_is_supported_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_iterable_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_itk_torch_bridge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_itk_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_keep_largest_connected_component.py
--rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_keep_largest_connected_componentd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_kspace_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_label_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_label_filterd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_label_quality_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_label_to_contour.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_label_to_contourd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_label_to_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_label_to_maskd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_lesion_froc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_list_data_collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_list_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_lltm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10439 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_lmdbdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_lmdbdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_load_decathlon_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_load_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_load_imaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_load_spacing_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_loader_semaphore.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_local_normalized_cross_correlation_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_localnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_localnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_look_up_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_loss_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_lr_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_make_nifti.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_map_binary_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_map_classes_to_indices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_map_label_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_map_label_valued.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_map_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_mask_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_mask_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_masked_dice_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_masked_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_masked_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_matshow3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_mean_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_mean_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_median_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_median_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_median_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_mednistdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_meta_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)    23433 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_metatensor_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_metrics_reloaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_milmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_mmar_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_module_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_monai_env_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_monai_utils_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_mri_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_multi_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_net_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_network_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_nifti_endianness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_nifti_header_revise.py
--rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_nifti_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_normalize_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_npzdictitemdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_nrrd_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_nuclick_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_numpy_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_nvtx_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_nvtx_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_occlusion_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_one_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_optim_novograd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_optional_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_ori_ras_lps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_orientationd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_p3d_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_pad_collation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_pad_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_parallel_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_parallel_execution_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_partition_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_partition_dataset_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_patch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_patch_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8412 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_patchembedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_pathology_he_stain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_pathology_he_stain_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_pathology_prob_nms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_persistentdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_persistentdataset_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_phl_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_phl_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_pil_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_plot_2d_or_3d_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_png_rw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_polyval.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_prepare_batch_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_prepare_batch_default_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_prepare_batch_extra_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_prepare_batch_hovernet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_preset_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_print_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_print_transform_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_probnms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_probnmsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_pytorch_version_after.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_query_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_adjust_contrast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_adjust_contrastd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_affine_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_affined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_axis_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_axis_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_bias_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_bias_fieldd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_coarse_dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_coarse_dropoutd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_coarse_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_coarse_shuffled.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_crop_by_label_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_crop_by_label_classesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_crop_by_pos_neg_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_crop_by_pos_neg_labeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_cucim_dict_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_cucim_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_deform_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_elastic_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_elastic_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_elasticd_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_elasticd_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_flip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_flipd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_gaussian_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_gaussian_sharpen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_gaussian_sharpend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_gaussian_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_gaussian_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_gibbs_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_gibbs_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_grid_distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_grid_distortiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_grid_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_grid_patchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_histogram_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_histogram_shiftd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_k_space_spike_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_k_space_spike_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_lambdad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_rician_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_rician_noised.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_scale_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_scale_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_spatial_crop_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_spatial_crop_samplesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_weighted_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_weighted_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rand_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_randidentity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_random_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_randomizable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_randomizable_transform_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_randtorchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rankfilter_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_recon_net_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_reference_based_normalize_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_reference_based_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_reference_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_reg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_regunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_regunet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_remove_repeated_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_remove_repeated_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_remove_small_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_repeat_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_repeat_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_replace_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_require_pkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_resample_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_resample_datalist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_resample_to_match.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_resample_to_matchd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_resampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_resize.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_resize_with_pad_or_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_resize_with_pad_or_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_resized.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7362 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_retinanet.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_retinanet_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_retinanet_predict_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rotate90.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rotate90d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_rotated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_safe_dtype_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_saliency_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_sample_slices.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_save_classificationd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_save_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_save_imaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_save_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_savitzky_golay_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_savitzky_golay_smooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_savitzky_golay_smoothd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_scale_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_scale_intensity_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_scale_intensity_range_percentiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_scale_intensity_range_percentilesd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_scale_intensity_ranged.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_scale_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_se_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_se_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_seg_loss_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_segresnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_segresnet_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_segresnet_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_select_cross_validation_folds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_select_itemsd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_selfattention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_senet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_separable_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_set_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_set_visible_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_shuffle_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_signal_continuouswavelet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_signal_fillempty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_signal_rand_add_gaussiannoise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_signal_rand_add_sine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_signal_rand_add_sine_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_signal_rand_add_squarepulse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_signal_rand_add_squarepulse_partial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_signal_rand_drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_signal_rand_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_signal_rand_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_signal_remove_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_simple_aspp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_simulatedelay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_simulatedelayd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_skip_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_slice_inferer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_sliding_patch_wsi_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11790 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_sliding_window_hovernet_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_sliding_window_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_sliding_window_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_smartcachedataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_smooth_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_sobel_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_sobel_gradientd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_some_of.py
--rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_spacing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_spacingd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_spatial_combine_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_spatial_crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_spatial_cropd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_spatial_pad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_spatial_padd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_spatial_resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_spatial_resampled.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_split_channel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_split_channeld.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_splitdim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_splitdimd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_squeezedim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_squeezedimd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_ssim_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_ssim_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_state_cacher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_std_shift_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_std_shift_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_str2bool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_str2list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_subpixel_upsample.py
--rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_surface_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_surface_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_swin_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_synthetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_tciadataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_testtimeaugmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_thread_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_threadcontainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_threshold_intensity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_threshold_intensityd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_timedcall_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_to_contiguous.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_to_cupy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_to_cupyd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_to_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_to_deviced.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_to_from_meta_tensord.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_to_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_to_numpyd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_to_onehot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_to_pil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_to_pild.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_to_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_to_tensord.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_torchscript_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_torchvision_fc_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_torchvisiond.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_traceable_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_train_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_trainable_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (123)    21368 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_trainable_joint_bilateral.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_transchex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_transformerblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_transposed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_tversky_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_unetr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_unetr_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_unified_focal_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_upsample_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_utils_pytorch_numpy_unification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_varautoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_varnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_version_leq.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_video_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_vis_cam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_vis_gradbased.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_vis_gradcam.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_vitautoenc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_vnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_vote_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_vote_ensembled.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_warp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_watershed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_watershedd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_weight_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_weighted_random_sampler_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_with_allow_missing_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_write_metrics_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)    19695 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_wsireader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_zipdataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_zoom_affine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-09 02:17:10.000000 monai-weekly-1.2.dev2315/tests/test_zoomd.py
--rw-r--r--   0 runner    (1001) docker     (123)    81097 2023-04-09 02:17:11.000000 monai-weekly-1.2.dev2315/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.476853 monai-weekly-1.2.dev2316/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-04-16 02:21:48.476853 monai-weekly-1.2.dev2316/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.476853 monai-weekly-1.2.dev2316/monai/
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-04-16 02:19:48.000000 monai-weekly-1.2.dev2316/monai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.044857 monai-weekly-1.2.dev2316/monai/_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/_extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.044857 monai-weekly-1.2.dev2316/monai/_extensions/gmm/
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/_extensions/gmm/gmm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/_extensions/gmm/gmm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/_extensions/gmm/gmm_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/_extensions/gmm/gmm_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/_extensions/gmm/gmm_cuda_linalg.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/_extensions/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-16 02:21:48.476853 monai-weekly-1.2.dev2316/monai/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.044857 monai-weekly-1.2.dev2316/monai/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.048857 monai-weekly-1.2.dev2316/monai/apps/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/auto3dseg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36754 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/auto3dseg/auto_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25498 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/auto3dseg/bundle_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/auto3dseg/data_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22475 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/auto3dseg/ensemble_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17523 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/auto3dseg/hpo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/auto3dseg/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/auto3dseg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34560 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.048857 monai-weekly-1.2.dev2316/monai/apps/deepedit/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/deepedit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/deepedit/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37435 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/deepedit/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.052857 monai-weekly-1.2.dev2316/monai/apps/deepgrow/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/deepgrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/deepgrow/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/deepgrow/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42011 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/deepgrow/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.052857 monai-weekly-1.2.dev2316/monai/apps/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.052857 monai-weekly-1.2.dev2316/monai/apps/detection/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26617 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/metrics/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/metrics/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.056857 monai-weekly-1.2.dev2316/monai/apps/detection/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51663 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/networks/retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17604 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/networks/retinanet_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.056857 monai-weekly-1.2.dev2316/monai/apps/detection/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24519 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/transforms/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68979 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.060857 monai-weekly-1.2.dev2316/monai/apps/detection/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/utils/ATSS_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18681 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/utils/anchor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/utils/box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/utils/box_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/utils/detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13890 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/utils/hard_negative_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/detection/utils/predict_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.060857 monai-weekly-1.2.dev2316/monai/apps/mmars/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/mmars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13115 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/mmars/mmars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/mmars/model_desc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.064857 monai-weekly-1.2.dev2316/monai/apps/nnunet/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/nnunet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/nnunet/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38587 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/nnunet/nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/nnunet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.064857 monai-weekly-1.2.dev2316/monai/apps/nuclick/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/nuclick/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/nuclick/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.064857 monai-weekly-1.2.dev2316/monai/apps/pathology/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.064857 monai-weekly-1.2.dev2316/monai/apps/pathology/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/engines/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.064857 monai-weekly-1.2.dev2316/monai/apps/pathology/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/handlers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.064857 monai-weekly-1.2.dev2316/monai/apps/pathology/inferers/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/inferers/inferer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.068857 monai-weekly-1.2.dev2316/monai/apps/pathology/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7293 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/losses/hovernet_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.068857 monai-weekly-1.2.dev2316/monai/apps/pathology/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/metrics/lesion_froc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.068857 monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.068857 monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37322 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25992 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.068857 monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/stain/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/stain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/stain/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/stain/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/pathology/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.072857 monai-weekly-1.2.dev2316/monai/apps/reconstruction/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/mri_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.072857 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.072857 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/blocks/varnetblock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.072857 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/complex_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/varnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.076856 monai-weekly-1.2.dev2316/monai/apps/reconstruction/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/transforms/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15844 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/reconstruction/transforms/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.076856 monai-weekly-1.2.dev2316/monai/apps/tcia/
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/tcia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/tcia/label_desc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/tcia/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13505 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/apps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.080856 monai-weekly-1.2.dev2316/monai/auto3dseg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/auto3dseg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/auto3dseg/algo_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41223 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/auto3dseg/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/auto3dseg/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/auto3dseg/seg_summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12193 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/auto3dseg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.080856 monai-weekly-1.2.dev2316/monai/bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/bundle/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16035 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/bundle/config_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22410 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/bundle/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/bundle/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/bundle/reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63733 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/bundle/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/bundle/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/bundle/workflows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.084856 monai-weekly-1.2.dev2316/monai/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/config/deviceconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/config/type_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.092856 monai-weekly-1.2.dev2316/monai/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50102 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68927 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60619 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39872 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/image_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/meta_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27321 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/test_time_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8840 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64795 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9059 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/video_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18631 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/wsi_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49442 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/data/wsi_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.096856 monai-weekly-1.2.dev2316/monai/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24568 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/engines/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/engines/multi_gpu_supervised_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21347 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/engines/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/engines/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15250 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/engines/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.096856 monai-weekly-1.2.dev2316/monai/fl/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/fl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.096856 monai-weekly-1.2.dev2316/monai/fl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/fl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/fl/client/client_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32635 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/fl/client/monai_algo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.096856 monai-weekly-1.2.dev2316/monai/fl/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/fl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/fl/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/fl/utils/exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/fl/utils/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.112856 monai-weekly-1.2.dev2316/monai/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16071 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/clearml_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/earlystop_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/ignite_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/logfile_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/lr_schedule_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/metrics_reloaded_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16326 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/mlflow_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/nvtx_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/probability_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/smartcache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14251 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/stats_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23325 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/tensorboard_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/handlers/validation_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.116856 monai-weekly-1.2.dev2316/monai/inferers/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/inferers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32038 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/inferers/inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/inferers/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/inferers/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20036 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/inferers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.124856 monai-weekly-1.2.dev2316/monai/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/deform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46326 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15492 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/image_dissimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/spatial_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/tversky.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/losses/unified_focal_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.136856 monai-weekly-1.2.dev2316/monai/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/active_learning_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15101 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/f_beta_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8262 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/meandice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13679 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18235 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14415 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/metrics/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.136856 monai-weekly-1.2.dev2316/monai/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.152856 monai-weekly-1.2.dev2316/monai/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/acti_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/backbone_fpn_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/crf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/dints_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/feature_pyramid_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/fft_utils_t.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7987 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/squeeze_and_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/text_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6656 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/blocks/warp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.156856 monai-weekly-1.2.dev2316/monai/networks/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/layers/convutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/layers/drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/layers/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17992 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/layers/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/layers/gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28470 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/layers/simplelayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25576 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/layers/spatial_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/layers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/layers/weight_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.172855 monai-weekly-1.2.dev2316/monai/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21533 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9202 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10950 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44771 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/dints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18210 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40643 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14147 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/netadapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17189 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/regunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16785 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15667 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19289 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42000 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/torchvision_fc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16626 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/transchex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13722 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/nets/vnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46286 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/networks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.176855 monai-weekly-1.2.dev2316/monai/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21952 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/optimizers/lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/optimizers/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/optimizers/novograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/optimizers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.184856 monai-weekly-1.2.dev2316/monai/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)    15248 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40532 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/compose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.188856 monai-weekly-1.2.dev2316/monai/transforms/croppad/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/croppad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67678 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/croppad/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/croppad/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54071 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/croppad/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/croppad/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.188856 monai-weekly-1.2.dev2316/monai/transforms/intensity/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/intensity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98613 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/intensity/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76501 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/intensity/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17160 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/inverse_batch_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.188856 monai-weekly-1.2.dev2316/monai/transforms/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25430 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/io/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/io/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.192855 monai-weekly-1.2.dev2316/monai/transforms/lazy/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/lazy/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/lazy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.192855 monai-weekly-1.2.dev2316/monai/transforms/meta_utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/meta_utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/meta_utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/nvtx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.196855 monai-weekly-1.2.dev2316/monai/transforms/post/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/post/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39905 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/post/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.196855 monai-weekly-1.2.dev2316/monai/transforms/signal/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16378 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/signal/array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.196855 monai-weekly-1.2.dev2316/monai/transforms/smooth_field/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/smooth_field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/smooth_field/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/smooth_field/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.200855 monai-weekly-1.2.dev2316/monai/transforms/spatial/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/spatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   168618 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/spatial/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107151 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/spatial/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31494 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/spatial/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18234 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.204855 monai-weekly-1.2.dev2316/monai/transforms/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70325 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/utility/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75816 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/utility/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72516 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31081 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/utils_create_transform_ims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/transforms/utils_pytorch_numpy_unification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.216855 monai-weekly-1.2.dev2316/monai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/deprecate_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16807 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15637 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/jupyter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27512 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23631 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/utils/type_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.220855 monai-weekly-1.2.dev2316/monai/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16156 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/visualize/class_activation_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/visualize/gradient_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9200 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/visualize/img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/visualize/occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/visualize/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/monai/visualize/visualizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.220855 monai-weekly-1.2.dev2316/monai_weekly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-04-16 02:21:47.000000 monai-weekly-1.2.dev2316/monai_weekly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33869 2023-04-16 02:21:48.000000 monai-weekly-1.2.dev2316/monai_weekly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 02:21:47.000000 monai-weekly-1.2.dev2316/monai_weekly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 02:21:47.000000 monai-weekly-1.2.dev2316/monai_weekly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-16 02:21:47.000000 monai-weekly-1.2.dev2316/monai_weekly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 02:21:47.000000 monai-weekly-1.2.dev2316/monai_weekly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-04-16 02:21:48.476853 monai-weekly-1.2.dev2316/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 02:21:48.476853 monai-weekly-1.2.dev2316/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_acn_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_activationsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_adaptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_add_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_add_coordinate_channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_add_coordinate_channelsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_add_extreme_points_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_add_extreme_points_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_adn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9979 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_affine_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_affined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ahnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_anchor_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_apply.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_apply_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_arraydataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_as_channel_first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_as_channel_firstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_as_channel_last.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_as_channel_lastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_as_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_as_discreted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_atss_box_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_attentionunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21578 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_auto3dseg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_auto3dseg_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_auto3dseg_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_avg_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_basic_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_basic_unetplusplus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bending_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bilateral_approx_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13773 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bilateral_approx_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15064 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bilateral_precise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_blend_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_border_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_border_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bounding_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bounding_rectd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_box_coder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17289 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_box_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bundle_ckpt_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bundle_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bundle_get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bundle_init_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bundle_onnx_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bundle_trt_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bundle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bundle_verify_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bundle_verify_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_bundle_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cachedataset_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cachedataset_persistent_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cachentransdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_call_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cast_to_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cast_to_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_center_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_center_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_center_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_center_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_channel_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_check_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_check_missing_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_classes_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_complex_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_component_locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11371 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compose_get_number_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_f_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_generalized_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_ho_ver_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_ho_ver_maps_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_meandice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_meaniou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_roc_auc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_compute_variance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_concat_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_config_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14667 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_contrastive_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_convert_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_convert_to_multi_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_convert_to_multi_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_convert_to_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_convert_to_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_convert_to_trt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_copy_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6761 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_copy_model_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_correct_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_create_cross_validation_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_create_grid_and_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_crf_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_crf_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_crop_foreground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_crop_foregroundd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cross_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11089 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_csv_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_csv_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cumulative.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cumulative_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cumulative_average_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_cv2_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_data_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_data_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dataset_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dataset_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_decathlondataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_decollate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_deepedit_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_deepedit_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_deepgrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_deepgrow_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_deepgrow_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_delete_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_denseblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_densenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_detect_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_detection_coco_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_detector_boxselector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_detector_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dev_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dice_ce_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dints_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dints_mixop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dints_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_divisible_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_divisible_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_download_and_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_downsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_drop_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ds_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dvf2ddf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dynunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_dynunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13331 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ensemble_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ensure_channel_first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ensure_channel_firstd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ensure_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ensure_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ensure_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_enum_bound_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_eval_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_evenly_divisible_all_gather_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_factorized_increase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_factorized_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fastmri_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fft_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fg_bg_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fg_bg_to_indicesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_file_basename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fill_holes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fill_holesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fl_exchange_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fl_monai_algo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fl_monai_algo_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fl_monai_algo_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_flatten_sub_keysd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_flexible_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12045 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_folder_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_foreground_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_foreground_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fpn_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_from_engine_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_fullyconnectednet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_gaussian_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generalized_dice_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generalized_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generalized_wasserstein_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_distance_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_distance_mapd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_instance_border.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_instance_borderd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_instance_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_instance_centroidd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_instance_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_instance_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_instance_typed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_label_classes_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_param_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_pos_neg_label_crop_centers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_spatial_bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_succinct_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_succinct_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_watershed_markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_watershed_markersd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_watershed_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generate_watershed_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_get_equivalent_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_get_extreme_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_get_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_get_package_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_get_unique_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_giou_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_global_mutual_information_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_globalnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_gmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8683 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_grid_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_grid_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_grid_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_grid_splitd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_checkpoint_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_classification_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_classification_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_clearml_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_clearml_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_confusion_matrix_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_decollate_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_early_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3879 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_logfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_mean_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_metric_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5833 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_metrics_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_metrics_saver_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_mlflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_nvtx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_panoptic_quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_parameter_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_prob_map_producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_regression_metrics_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_rocauc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_rocauc_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_smartcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_tb_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_tb_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_handler_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_hardnegsampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_hausdorff_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_header_correct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_highresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_hilbert_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_histogram_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_histogram_normalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_hovernet_instance_map_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_hovernet_instance_map_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_hovernet_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_hovernet_nuclear_type_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_hovernet_nuclear_type_post_processingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_identityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_image_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_image_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_img2tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_init_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_autorunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_bundle_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_classification_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_fast_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_gpu_customization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8693 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_lazy_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_nnunetv2_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13199 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_segmentation_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_sliding_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_stn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_unet_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_workers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_integration_workflows_gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_intensity_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_intensity_statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18873 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_inverse_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_inverse_collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_invert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_invertd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_is_supported_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_iterable_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_itk_torch_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_itk_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14754 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_keep_largest_connected_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12548 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_keep_largest_connected_componentd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_kspace_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_label_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_label_filterd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_label_quality_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_label_to_contour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_label_to_contourd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_label_to_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_label_to_maskd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_lesion_froc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_list_data_collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_list_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_lltm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10439 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_lmdbdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_lmdbdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_load_decathlon_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_load_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_load_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_load_spacing_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_loader_semaphore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_local_normalized_cross_correlation_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_localnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_localnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_look_up_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_loss_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_lr_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_make_nifti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_map_binary_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_map_classes_to_indices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_map_label_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_map_label_valued.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_map_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_mask_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_mask_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_masked_dice_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_masked_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_masked_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_matshow3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_mean_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_mean_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_median_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_median_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_median_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_mednistdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7458 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_meta_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23490 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_metatensor_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_metrics_reloaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_milmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_mmar_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_monai_env_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_monai_utils_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_mri_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_multi_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_net_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_network_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_nifti_endianness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_nifti_header_revise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_nifti_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_normalize_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_npzdictitemdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_nrrd_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_nuclick_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_numpy_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_nvtx_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_nvtx_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_occlusion_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_one_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_optim_novograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_optional_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ori_ras_lps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_orientationd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_p3d_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_pad_collation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_pad_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_parallel_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_parallel_execution_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_partition_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_partition_dataset_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_patch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_patch_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_patchembedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_pathology_he_stain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_pathology_he_stain_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_pathology_prob_nms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_persistentdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_persistentdataset_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_phl_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_phl_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_pil_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_plot_2d_or_3d_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_png_rw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_polyval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_prepare_batch_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_prepare_batch_default_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_prepare_batch_extra_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_prepare_batch_hovernet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_preset_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_print_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_print_transform_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_probnms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_probnmsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_pytorch_version_after.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_query_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_adjust_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_adjust_contrastd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_affine_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_affined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_axis_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_axis_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_bias_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_bias_fieldd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_coarse_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_coarse_dropoutd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_coarse_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_coarse_shuffled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_crop_by_label_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_crop_by_label_classesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_crop_by_pos_neg_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_crop_by_pos_neg_labeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_cucim_dict_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_cucim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_deform_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4596 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_elastic_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_elastic_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_elasticd_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_elasticd_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_flip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_flipd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_gaussian_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_gaussian_sharpen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_gaussian_sharpend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_gaussian_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_gaussian_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_gibbs_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_gibbs_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_grid_distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_grid_distortiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_grid_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_grid_patchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_histogram_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_histogram_shiftd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_k_space_spike_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_k_space_spike_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_lambdad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_rician_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_rician_noised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_scale_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_scale_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_spatial_crop_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_spatial_crop_samplesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_weighted_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_weighted_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rand_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_randidentity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_random_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_randomizable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_randomizable_transform_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_randtorchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rankfilter_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_recon_net_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_reference_based_normalize_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_reference_based_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_reference_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_reg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_regunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_regunet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_remove_repeated_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_remove_repeated_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_remove_small_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_repeat_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_repeat_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_replace_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_require_pkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resample_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resample_datalist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resample_to_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resample_to_matchd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resize_with_pad_or_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resize_with_pad_or_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_retinanet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_retinanet_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_retinanet_predict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rotate90.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rotate90d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_rotated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_safe_dtype_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_saliency_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_sample_slices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_save_classificationd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_save_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_save_imaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_save_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_savitzky_golay_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_savitzky_golay_smooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_savitzky_golay_smoothd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_scale_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_scale_intensity_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_scale_intensity_range_percentiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_scale_intensity_range_percentilesd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_scale_intensity_ranged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_scale_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_se_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_se_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_seg_loss_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_segresnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_segresnet_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_segresnet_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_select_cross_validation_folds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_select_itemsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_selfattention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_senet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_separable_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_set_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_set_visible_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_shuffle_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_continuouswavelet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_fillempty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_rand_add_gaussiannoise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_rand_add_sine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_rand_add_sine_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_rand_add_squarepulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_rand_add_squarepulse_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_rand_drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_rand_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_rand_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_signal_remove_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_simple_aspp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_simulatedelay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_simulatedelayd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_skip_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_slice_inferer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10903 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_sliding_patch_wsi_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_sliding_window_hovernet_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_sliding_window_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8162 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_sliding_window_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_smartcachedataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_smooth_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_sobel_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_sobel_gradientd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_some_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_spacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_spacingd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_spatial_combine_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_spatial_crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_spatial_cropd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_spatial_pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_spatial_padd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9792 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_spatial_resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_spatial_resampled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_split_channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_split_channeld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_splitdim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_splitdimd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_squeezedim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_squeezedimd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ssim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_ssim_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_state_cacher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_std_shift_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_std_shift_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_str2bool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_str2list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_subpixel_upsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18990 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_surface_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_surface_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_swin_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_synthetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_tciadataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6739 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_testtimeaugmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_text_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_thread_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_threadcontainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_threshold_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_threshold_intensityd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_timedcall_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_contiguous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_cupy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_cupyd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_deviced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_from_meta_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_numpyd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_onehot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_pild.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_to_tensord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_torchscript_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_torchvision_fc_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_torchvisiond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_traceable_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_train_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16832 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_trainable_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_trainable_joint_bilateral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_transchex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_transformerblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_transposed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_tversky_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_unetr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_unetr_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_unified_focal_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_upsample_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_utils_pytorch_numpy_unification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_varautoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_varnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_version_leq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_video_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_vis_cam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_vis_gradbased.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_vis_gradcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_vitautoenc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_vnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_vote_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_vote_ensembled.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_warp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_watershed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_watershedd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_weight_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_weighted_random_sampler_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_with_allow_missing_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_write_metrics_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25914 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_wsireader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_zipdataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_zoom_affine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/tests/test_zoomd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81097 2023-04-16 02:19:41.000000 monai-weekly-1.2.dev2316/versioneer.py
```

### Comparing `monai-weekly-1.2.dev2315/LICENSE` & `monai-weekly-1.2.dev2316/LICENSE`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/PKG-INFO` & `monai-weekly-1.2.dev2316/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.2.dev2315
+Version: 1.2.dev2316
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
```

### Comparing `monai-weekly-1.2.dev2315/README.md` & `monai-weekly-1.2.dev2316/README.md`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/__init__.py` & `monai-weekly-1.2.dev2316/monai/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,8 +74,8 @@
     "metrics",
     "networks",
     "optimizers",
     "transforms",
     "utils",
     "visualize",
 ]
-__commit_id__ = "e4b313d59b2702cd2a441d7a557650ced78dc6c8"
+__commit_id__ = "b356fecdb265ee9af4ce91a0c8238731994b5095"
```

### Comparing `monai-weekly-1.2.dev2315/monai/_extensions/__init__.py` & `monai-weekly-1.2.dev2316/monai/_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/_extensions/gmm/gmm.cpp` & `monai-weekly-1.2.dev2316/monai/_extensions/gmm/gmm.cpp`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/_extensions/gmm/gmm.h` & `monai-weekly-1.2.dev2316/monai/_extensions/gmm/gmm.h`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/_extensions/gmm/gmm_cpu.cpp` & `monai-weekly-1.2.dev2316/monai/_extensions/gmm/gmm_cpu.cpp`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/_extensions/gmm/gmm_cuda.cu` & `monai-weekly-1.2.dev2316/monai/_extensions/gmm/gmm_cuda.cu`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/_extensions/gmm/gmm_cuda_linalg.cuh` & `monai-weekly-1.2.dev2316/monai/_extensions/gmm/gmm_cuda_linalg.cuh`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/_extensions/loader.py` & `monai-weekly-1.2.dev2316/monai/_extensions/loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/auto3dseg/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/tcia/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,13 +7,9 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from .auto_runner import AutoRunner
-from .bundle_gen import BundleAlgo, BundleGen
-from .data_analyzer import DataAnalyzer
-from .ensemble_builder import AlgoEnsemble, AlgoEnsembleBestByFold, AlgoEnsembleBestN, AlgoEnsembleBuilder
-from .hpo_gen import NNIGen, OptunaGen
-from .utils import export_bundle_algo_history, import_bundle_algo_history
+from .label_desc import TCIA_LABEL_DICT
+from .utils import download_tcia_series_instance, get_tcia_metadata, get_tcia_ref_uid, match_tcia_ref_uid_in_study
```

### Comparing `monai-weekly-1.2.dev2315/monai/apps/auto3dseg/__main__.py` & `monai-weekly-1.2.dev2316/monai/apps/auto3dseg/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,25 +10,26 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 from monai.apps.auto3dseg.auto_runner import AutoRunner
 from monai.apps.auto3dseg.bundle_gen import BundleAlgo, BundleGen
 from monai.apps.auto3dseg.data_analyzer import DataAnalyzer
-from monai.apps.auto3dseg.ensemble_builder import AlgoEnsembleBuilder
+from monai.apps.auto3dseg.ensemble_builder import AlgoEnsembleBuilder, EnsembleRunner
 from monai.apps.auto3dseg.hpo_gen import NNIGen, OptunaGen
 
 if __name__ == "__main__":
     from monai.utils import optional_import
 
     fire, _ = optional_import("fire")
     fire.Fire(
         {
             "DataAnalyzer": DataAnalyzer,
             "BundleGen": BundleGen,
             "BundleAlgo": BundleAlgo,
             "AlgoEnsembleBuilder": AlgoEnsembleBuilder,
+            "EnsembleRunner": EnsembleRunner,
             "AutoRunner": AutoRunner,
             "NNIGen": NNIGen,
             "OptunaGen": OptunaGen,
         }
     )
```

### Comparing `monai-weekly-1.2.dev2315/monai/apps/auto3dseg/auto_runner.py` & `monai-weekly-1.2.dev2316/monai/apps/auto3dseg/auto_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,33 +15,25 @@
 import shutil
 import subprocess
 import warnings
 from copy import deepcopy
 from time import sleep
 from typing import Any, cast
 
-import numpy as np
 import torch
 
 from monai.apps.auto3dseg.bundle_gen import BundleGen
 from monai.apps.auto3dseg.data_analyzer import DataAnalyzer
-from monai.apps.auto3dseg.ensemble_builder import (
-    AlgoEnsemble,
-    AlgoEnsembleBestByFold,
-    AlgoEnsembleBestN,
-    AlgoEnsembleBuilder,
-)
+from monai.apps.auto3dseg.ensemble_builder import EnsembleRunner
 from monai.apps.auto3dseg.hpo_gen import NNIGen
 from monai.apps.auto3dseg.utils import export_bundle_algo_history, import_bundle_algo_history
 from monai.apps.utils import get_logger
 from monai.auto3dseg.utils import algo_to_pickle
 from monai.bundle import ConfigParser
-from monai.transforms import SaveImage
-from monai.utils.enums import AlgoEnsembleKeys
-from monai.utils.module import look_up_option, optional_import
+from monai.utils import AlgoKeys, has_option, look_up_option, optional_import
 
 logger = get_logger(module_name=__name__)
 
 nni, has_nni = optional_import("nni")
 
 
 class AutoRunner:
@@ -228,14 +220,15 @@
         os.makedirs(work_dir, exist_ok=True)
 
         self.work_dir = os.path.abspath(work_dir)
         self.data_src_cfg = dict()
         self.data_src_cfg_name = os.path.join(self.work_dir, "input.yaml")
         self.algos = algos
         self.templates_path_or_url = templates_path_or_url
+        self.kwargs = deepcopy(kwargs)
 
         if input is None and os.path.isfile(self.data_src_cfg_name):
             input = self.data_src_cfg_name
             logger.info(f"Input config is not provided, using the default {input}")
 
         if isinstance(input, dict):
             self.data_src_cfg = input
@@ -281,24 +274,19 @@
         # determine if we need to analyze, algo_gen or train from cache, unless manually provided
         self.analyze = not self.cache["analyze"] if analyze is None else analyze
         self.algo_gen = not self.cache["algo_gen"] if algo_gen is None else algo_gen
         self.train = train
         self.ensemble = ensemble  # last step, no need to check
 
         self.set_training_params()
+        self.set_device_info()
         self.set_prediction_params()
         self.set_analyze_params()
-
-        self.save_image = self.set_image_save_transform(kwargs)
-
-        self.ensemble_method: AlgoEnsemble
-        self.ensemble_method_name: str | None = None
-
+        self.set_ensemble_method()
         self.set_num_fold(num_fold=num_fold)
-        self.set_ensemble_method("AlgoEnsembleBestByFold")
 
         self.gpu_customization = False
         self.gpu_customization_specs: dict[str, Any] = {}
 
         # hpo
         if hpo_backend.lower() != "nni":
             raise NotImplementedError("HPOGen backend only supports NNI")
@@ -457,26 +445,19 @@
 
     def set_num_fold(self, num_fold: int = 5) -> None:
         """
         Set the number of cross validation folds for all algos.
 
         Args:
             num_fold: a positive integer to define the number of folds.
-
-        Notes:
-            If the ensemble method is ``AlgoEnsembleBestByFold``, this function automatically updates the ``n_fold``
-            parameter in the ``ensemble_method`` to avoid inconsistency between the training and the ensemble.
         """
 
         if num_fold <= 0:
             raise ValueError(f"num_fold is expected to be an integer greater than zero. Now it gets {num_fold}")
-
         self.num_fold = num_fold
-        if self.ensemble_method_name == "AlgoEnsembleBestByFold":
-            self.ensemble_method.n_fold = self.num_fold  # type: ignore
 
     def set_training_params(self, params: dict[str, Any] | None = None) -> None:
         """
         Set the training params for all algos.
 
         Args:
             params: a dict that defines the overriding key-value pairs during training. The overriding method
@@ -484,14 +465,103 @@
 
         Examples:
             For BundleAlgo objects, the training parameter to shorten the training time to a few epochs can be
                 {"num_iterations": 8, "num_iterations_per_validation": 4}
 
         """
         self.train_params = deepcopy(params) if params is not None else {}
+        if "CUDA_VISIBLE_DEVICES" in self.train_params:
+            warnings.warn(
+                "CUDA_VISIBLE_DEVICES is deprecated from 'set_training_params'. Use 'set_device_info' intead.",
+                DeprecationWarning,
+            )
+
+    def set_device_info(
+        self,
+        cuda_visible_devices: list[int] | str | None = None,
+        num_nodes: int | None = None,
+        mn_start_method: str | None = None,
+        cmd_prefix: str | None = None,
+    ) -> None:
+        """
+        Set the device related info
+
+        Args:
+            cuda_visible_device: define GPU ids for data analyzer, training, and ensembling.
+                List of GPU ids [0,1,2,3] or a string "0,1,2,3".
+                Default using env "CUDA_VISIBLE_DEVICES" or all devices available.
+            num_nodes: number of nodes for training and ensembling.
+                Default using env "NUM_NODES" or 1 if "NUM_NODES" is unset.
+            mn_start_method: multi-node start method. Autorunner will use the method to start multi-node processes.
+                Default using env "MN_START_METHOD" or 'bcprun' if "MN_START_METHOD" is unset.
+            cmd_prefix: command line prefix for subprocess running in BundleAlgo and EnsembleRunner.
+                Default using env "CMD_PREFIX" or None, examples are:
+
+                    - single GPU/CPU or multinode bcprun: "python " or "/opt/conda/bin/python3.8 ",
+                    - single node multi-GPU running "torchrun --nnodes=1 --nproc_per_node=2 "
+
+                If user define this prefix, please make sure --nproc_per_node matches cuda_visible_device or
+                os.env['CUDA_VISIBLE_DEVICES]. Also always set --nnodes=1. Set num_nodes for multi-node.
+        """
+        self.device_setting: dict[str, Any] = {}
+        if cuda_visible_devices is None:
+            cuda_visible_devices = os.environ.get("CUDA_VISIBLE_DEVICES")
+        if cuda_visible_devices is None:  # still None after reading the environ
+            self.device_setting["CUDA_VISIBLE_DEVICES"] = ",".join([str(x) for x in range(torch.cuda.device_count())])
+            self.device_setting["n_devices"] = torch.cuda.device_count()
+        elif isinstance(cuda_visible_devices, str):
+            self.device_setting["CUDA_VISIBLE_DEVICES"] = cuda_visible_devices
+            self.device_setting["n_devices"] = len(cuda_visible_devices.split(","))
+        elif isinstance(cuda_visible_devices, (list, tuple)):
+            self.device_setting["CUDA_VISIBLE_DEVICES"] = ",".join([str(x) for x in cuda_visible_devices])
+            self.device_setting["n_devices"] = len(cuda_visible_devices)
+        else:
+            logger.warn(f"Wrong format of cuda_visible_devices {cuda_visible_devices}, devices not set")
+
+        if num_nodes is None:
+            num_nodes = int(os.environ.get("NUM_NODES", 1))
+        self.device_setting["NUM_NODES"] = num_nodes
+
+        if mn_start_method is None:
+            mn_start_method = os.environ.get("MN_START_METHOD", "bcprun")
+        self.device_setting["MN_START_METHOD"] = mn_start_method
+
+        if cmd_prefix is None:
+            cmd_prefix = os.environ.get("CMD_PREFIX")
+        self.device_setting["CMD_PREFIX"] = cmd_prefix
+
+        if cmd_prefix is not None:
+            logger.info(f"Using user defined command running prefix {cmd_prefix}, will overide other settings")
+
+    def set_ensemble_method(self, ensemble_method_name: str = "AlgoEnsembleBestByFold", **kwargs: Any) -> None:
+        """
+        Set the bundle ensemble method name and parameters for save image transform parameters.
+
+        Args:
+            params: the name of the ensemble method. Only two methods are supported "AlgoEnsembleBestN"
+                and "AlgoEnsembleBestByFold".
+            kwargs: the keyword arguments used to define the ensemble method. Currently only ``n_best`` for
+                ``AlgoEnsembleBestN`` is supported.
+        """
+        self.ensemble_method_name = look_up_option(
+            ensemble_method_name, supported=["AlgoEnsembleBestN", "AlgoEnsembleBestByFold"]
+        )
+        self.kwargs.update(kwargs)
+
+    def set_image_save_transform(self, **kwargs: Any) -> None:
+        """
+        Set the ensemble output transform.
+
+        Args:
+            kwargs: image writing parameters for the ensemble inference. The kwargs format follows SaveImage
+                transform. For more information, check https://docs.monai.io/en/stable/transforms.html#saveimage.
+
+        """
+
+        self.kwargs.update(kwargs)
 
     def set_prediction_params(self, params: dict[str, Any] | None = None) -> None:
         """
         Set the prediction params for all algos.
 
         Args:
             params: a dict that defines the overriding key-value pairs during prediction. The overriding method
@@ -543,18 +613,15 @@
             params: a dict that defines the overriding key-value pairs during instantiation of the algo. For
                 BundleAlgo, it will override the template config filling.
 
         Notes:
             Users can set ``nni_dry_run`` to ``True`` in the ``params`` to enable the dry-run mode for the NNI backend.
 
         """
-        if params is None:
-            self.hpo_params = self.train_params
-        else:
-            self.hpo_params = params
+        self.hpo_params = self.train_params if params is None else params
 
     def set_nni_search_space(self, search_space):
         """
         Set the search space for NNI parameter search.
 
         Args:
             search_space: hyper parameter search space in the form of dict. For more information, please check
@@ -565,66 +632,14 @@
             if "_value" not in v:
                 raise ValueError(f"{search_space} key {k} value {v} has not _value")
             value_combinations *= len(v["_value"])
 
         self.search_space = search_space
         self.hpo_tasks = value_combinations
 
-    def set_image_save_transform(self, kwargs):
-        """
-        Set the ensemble output transform.
-
-        Args:
-            kwargs: image writing parameters for the ensemble inference. The kwargs format follows SaveImage
-                transform. For more information, check https://docs.monai.io/en/stable/transforms.html#saveimage .
-
-        """
-
-        if "output_dir" in kwargs:
-            output_dir = kwargs.pop("output_dir")
-        else:
-            output_dir = os.path.join(self.work_dir, "ensemble_output")
-            logger.info(f"The output_dir is not specified. {output_dir} will be used to save ensemble predictions")
-
-        if not os.path.isdir(output_dir):
-            os.makedirs(output_dir)
-            logger.info(f"Directory {output_dir} is created to save ensemble predictions")
-
-        self.output_dir = output_dir
-        output_postfix = kwargs.pop("output_postfix", "ensemble")
-        output_dtype = kwargs.pop("output_dtype", np.uint8)
-        resample = kwargs.pop("resample", False)
-
-        return SaveImage(
-            output_dir=output_dir, output_postfix=output_postfix, output_dtype=output_dtype, resample=resample, **kwargs
-        )
-
-    def set_ensemble_method(self, ensemble_method_name: str = "AlgoEnsembleBestByFold", **kwargs: Any) -> None:
-        """
-        Set the bundle ensemble method
-
-        Args:
-            ensemble_method_name: the name of the ensemble method. Only two methods are supported "AlgoEnsembleBestN"
-                and "AlgoEnsembleBestByFold".
-            kwargs: the keyword arguments used to define the ensemble method. Currently only ``n_best`` for
-                ``AlgoEnsembleBestN`` is supported.
-
-        """
-        self.ensemble_method_name = look_up_option(
-            ensemble_method_name, supported=["AlgoEnsembleBestN", "AlgoEnsembleBestByFold"]
-        )
-        if self.ensemble_method_name == "AlgoEnsembleBestN":
-            n_best = kwargs.pop("n_best", False)
-            n_best = 2 if not n_best else n_best
-            self.ensemble_method = AlgoEnsembleBestN(n_best=n_best)
-        elif self.ensemble_method_name == "AlgoEnsembleBestByFold":
-            self.ensemble_method = AlgoEnsembleBestByFold(n_fold=self.num_fold)
-        else:
-            raise NotImplementedError(f"Ensemble method {self.ensemble_method_name} is not implemented.")
-
     def _train_algo_in_sequence(self, history: list[dict[str, Any]]) -> None:
         """
         Train the Algos in a sequential scheme. The order of training is randomized.
 
         Args:
             history: the history of generated Algos. It is a list of dicts. Each element has the task name
                 (e.g. "dints_0" for dints network in fold 0) as the key and the algo object as the value.
@@ -632,19 +647,22 @@
 
         Note:
             The final results of the model training will be written to all the generated algorithm's output
             folders under the working directory. The results include the model checkpoints, a
             progress.yaml, accuracies in CSV and a pickle file of the Algo object.
         """
         for algo_dict in history:
-            algo = algo_dict[AlgoEnsembleKeys.ALGO]
-            algo.train(self.train_params)
+            algo = algo_dict[AlgoKeys.ALGO]
+            if has_option(algo.train, "device_setting"):
+                algo.train(self.train_params, self.device_setting)
+            else:
+                algo.train(self.train_params)
             acc = algo.get_score()
 
-            algo_meta_data = {str(AlgoEnsembleKeys.SCORE): acc}
+            algo_meta_data = {str(AlgoKeys.SCORE): acc}
             algo_to_pickle(algo, template_path=algo.template_path, **algo_meta_data)
 
     def _train_algo_in_nni(self, history: list[dict[str, Any]]) -> None:
         """
         Train the Algos using HPO.
 
         Args:
@@ -671,16 +689,16 @@
             "tuner": {"name": "GridSearch"},
             "trainingService": {"platform": "local", "useActiveGpu": True},
         }
 
         last_total_tasks = len(import_bundle_algo_history(self.work_dir, only_trained=True))
         mode_dry_run = self.hpo_params.pop("nni_dry_run", False)
         for algo_dict in history:
-            name = algo_dict[AlgoEnsembleKeys.ID]
-            algo = algo_dict[AlgoEnsembleKeys.ALGO]
+            name = algo_dict[AlgoKeys.ID]
+            algo = algo_dict[AlgoKeys.ALGO]
             nni_gen = NNIGen(algo=algo, params=self.hpo_params)
             obj_filename = nni_gen.get_obj_filename()
             nni_config = deepcopy(default_nni_config)
             # override the default nni config with the same key in hpo_params
             for key in self.hpo_params:
                 if key in nni_config:
                     nni_config[key] = self.hpo_params[key]
@@ -768,58 +786,38 @@
             if len(history) == 0:
                 raise ValueError(
                     f"Could not find training scripts in {self.work_dir}. "
                     "Possibly the required algorithms generation step was not completed."
                 )
 
             if auto_train_choice:
-                skip_algos = [h[AlgoEnsembleKeys.ID] for h in history if h["is_trained"]]
-                if len(skip_algos) > 0:
+                skip_algos = [h[AlgoKeys.ID] for h in history if h[AlgoKeys.IS_TRAINED]]
+                if skip_algos:
                     logger.info(
                         f"Skipping already trained algos {skip_algos}."
                         "Set option train=True to always retrain all algos."
                     )
-                    history = [h for h in history if not h["is_trained"]]
+                    history = [h for h in history if not h[AlgoKeys.IS_TRAINED]]
 
             if len(history) > 0:
                 if not self.hpo:
                     self._train_algo_in_sequence(history)
                 else:
                     self._train_algo_in_nni(history)
 
             self.export_cache(train=True)
         else:
             logger.info("Skipping algorithm training...")
 
         # step 4: model ensemble and write the prediction to disks.
         if self.ensemble:
-            history = import_bundle_algo_history(self.work_dir, only_trained=False)
-
-            history_untrained = [h for h in history if not h["is_trained"]]
-            if len(history_untrained) > 0:
-                warnings.warn(
-                    f"Ensembling step will skip {[h['name'] for h in history_untrained]} untrained algos."
-                    "Generally it means these algos did not complete training."
-                )
-                history = [h for h in history if h["is_trained"]]
-
-            if len(history) == 0:
-                raise ValueError(
-                    f"Could not find any trained algos in {self.work_dir}. "
-                    "Possibly the required training step was not completed."
-                )
-
-            builder = AlgoEnsembleBuilder(history, self.data_src_cfg_name)
-            builder.set_ensemble_method(self.ensemble_method)
-
-            ensembler = builder.get_ensemble()
-            preds = ensembler(pred_param=self.pred_params)
-            if len(preds) > 0:
-                logger.info("Auto3Dseg picked the following networks to ensemble:")
-                for algo in ensembler.get_algo_ensemble():
-                    logger.info(algo[AlgoEnsembleKeys.ID])
-
-                for pred in preds:
-                    self.save_image(pred)
-                logger.info(f"Auto3Dseg ensemble prediction outputs are saved in {self.output_dir}.")
-
+            ensemble_runner = EnsembleRunner(
+                data_src_cfg_name=self.data_src_cfg_name,
+                work_dir=self.work_dir,
+                num_fold=self.num_fold,
+                ensemble_method_name=self.ensemble_method_name,
+                mgpu=int(self.device_setting["n_devices"]) > 1,
+                **self.kwargs,  # for set_image_save_transform
+                **self.pred_params,
+            )  # for inference
+            ensemble_runner.run(self.device_setting)
         logger.info("Auto3Dseg pipeline is completed successfully.")
```

### Comparing `monai-weekly-1.2.dev2315/monai/apps/auto3dseg/bundle_gen.py` & `monai-weekly-1.2.dev2316/monai/apps/auto3dseg/bundle_gen.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 
 from monai.apps import download_and_extract
 from monai.apps.utils import get_logger
 from monai.auto3dseg.algo_gen import Algo, AlgoGen
 from monai.auto3dseg.utils import algo_to_pickle
 from monai.bundle.config_parser import ConfigParser
 from monai.utils import ensure_tuple
-from monai.utils.enums import AlgoEnsembleKeys
+from monai.utils.enums import AlgoKeys
 
 logger = get_logger(module_name=__name__)
-ALGO_HASH = os.environ.get("MONAI_ALGO_HASH", "7758ad1")
+ALGO_HASH = os.environ.get("MONAI_ALGO_HASH", "80c832e")
 
 __all__ = ["BundleAlgo", "BundleGen"]
 
 
 class BundleAlgo(Algo):
     """
     An algorithm represented by a set of bundle configurations and scripts.
@@ -76,14 +76,22 @@
         self.data_stats_files = ""
         self.data_list_file = ""
         self.output_path = ""
         self.name = ""
         self.best_metric = None
         # track records when filling template config: {"<config name>": {"<placeholder key>": value, ...}, ...}
         self.fill_records: dict = {}
+        # device_setting set default value and sanity check, in case device_setting not from autorunner
+        self.device_setting: dict[str, int | str] = {
+            "CUDA_VISIBLE_DEVICES": ",".join([str(x) for x in range(torch.cuda.device_count())]),
+            "n_devices": int(torch.cuda.device_count()),
+            "NUM_NODES": int(os.environ.get("NUM_NODES", 1)),
+            "MN_START_METHOD": os.environ.get("MN_START_METHOD", "bcprun"),
+            "CMD_PREFIX": os.environ.get("CMD_PREFIX"),  # type: ignore
+        }
 
     def pre_check_skip_algo(self, skip_bundlegen: bool = False, skip_info: str = "") -> tuple[bool, str]:
         """
         Analyse the data analysis report and check if the algorithm needs to be skipped.
         This function is overriden within algo.
         Args:
             skip_bundlegen: skip generating bundles for this algo if true.
@@ -146,79 +154,107 @@
             if os.path.isdir(self.output_path):
                 shutil.rmtree(self.output_path)
             shutil.copytree(self.template_path, self.output_path)
         else:
             self.output_path = self.template_path
         if kwargs.pop("fill_template", True):
             self.fill_records = self.fill_template_config(self.data_stats_files, self.output_path, **kwargs)
-        logger.info(self.output_path)
+        logger.info(f"Generated:{self.output_path}")
 
-    def _create_cmd(self, train_params=None):
+    def _create_cmd(self, train_params: None | dict = None) -> tuple[str, str]:
         """
         Create the command to execute training.
 
         """
-        if train_params is not None:
-            params = deepcopy(train_params)
+        if train_params is None:
+            train_params = {}
+        params = deepcopy(train_params)
 
         train_py = os.path.join(self.output_path, "scripts", "train.py")
         config_dir = os.path.join(self.output_path, "configs")
 
         if os.path.isdir(config_dir):
             base_cmd = ""
             for file in os.listdir(config_dir):
                 if not (file.endswith("yaml") or file.endswith("json")):
                     continue
-                if len(base_cmd) == 0:
-                    base_cmd += f"{train_py} run --config_file="
-                else:
-                    base_cmd += ","  # Python Fire does not accept space
+                base_cmd += f"{train_py} run --config_file=" if len(base_cmd) == 0 else ","
                 # Python Fire may be confused by single-quoted WindowsPath
                 config_yaml = Path(os.path.join(config_dir, file)).as_posix()
                 base_cmd += f"'{config_yaml}'"
-
-        if "CUDA_VISIBLE_DEVICES" in params:
-            devices = params.pop("CUDA_VISIBLE_DEVICES")
-            n_devices, devices_info = len(devices), ",".join([str(x) for x in devices])
-        else:
-            n_devices, devices_info = torch.cuda.device_count(), ""
-        if n_devices > 1:
-            cmd = f"torchrun --nnodes={1:d} --nproc_per_node={n_devices:d} "
+        cmd: str | None = self.device_setting["CMD_PREFIX"]  # type: ignore
+        # make sure cmd end with a space
+        if cmd is not None and not cmd.endswith(" "):
+            cmd += " "
+        if (int(self.device_setting["NUM_NODES"]) > 1 and self.device_setting["MN_START_METHOD"] == "bcprun") or (
+            int(self.device_setting["NUM_NODES"]) <= 1 and int(self.device_setting["n_devices"]) <= 1
+        ):
+            cmd = "python " if cmd is None else cmd
+        elif int(self.device_setting["NUM_NODES"]) > 1:
+            raise NotImplementedError(
+                f"{self.device_setting['MN_START_METHOD']} is not supported yet."
+                "Try modify BundleAlgo._create_cmd for your cluster."
+            )
         else:
-            cmd = "python "  # TODO: which system python?
+            if cmd is None:
+                cmd = f"torchrun --nnodes={1:d} --nproc_per_node={self.device_setting['n_devices']:d} "
         cmd += base_cmd
         if params and isinstance(params, Mapping):
             for k, v in params.items():
                 cmd += f" --{k}={v}"
-        return cmd, devices_info
+        return cmd, ""
 
-    def _run_cmd(self, cmd: str, devices_info: str) -> subprocess.CompletedProcess:
+    def _run_cmd(self, cmd: str, devices_info: str = "") -> subprocess.CompletedProcess:
         """
         Execute the training command with target devices information.
 
         """
+        if devices_info:
+            warnings.warn(f"input devices_info {devices_info} is deprecated and ignored.")
 
         logger.info(f"Launching: {cmd}")
         ps_environ = os.environ.copy()
-        if devices_info:
-            ps_environ["CUDA_VISIBLE_DEVICES"] = devices_info
-        normal_out = subprocess.run(cmd.split(), env=ps_environ, check=True)
-
-        return normal_out
-
-    def train(self, train_params=None):
+        ps_environ["CUDA_VISIBLE_DEVICES"] = str(self.device_setting["CUDA_VISIBLE_DEVICES"])
+        if int(self.device_setting["NUM_NODES"]) > 1:
+            if self.device_setting["MN_START_METHOD"] == "bcprun":
+                cmd = f"bcprun -n {self.device_setting['NUM_NODES']} -p {self.device_setting['n_devices']} -c {cmd}"
+            else:
+                raise NotImplementedError(
+                    f"{self.device_setting['MN_START_METHOD']} is not supported yet. "
+                    "Try modify BundleAlgo._run_cmd for your cluster."
+                )
+        cmd_list = cmd.split()
+        _idx = 0
+        for _idx, c in enumerate(cmd_list):
+            if "=" not in c:  # remove variable assignments before the command such as "OMP_NUM_THREADS=1"
+                break
+        return subprocess.run(cmd_list[_idx:], env=ps_environ, check=True)
+
+    def train(
+        self, train_params: None | dict = None, device_setting: None | dict = None
+    ) -> subprocess.CompletedProcess:
         """
         Load the run function in the training script of each model. Training parameter is predefined by the
         algo_config.yaml file, which is pre-filled by the fill_template_config function in the same instance.
 
         Args:
-            train_params:  to specify the devices using a list of integers: ``{"CUDA_VISIBLE_DEVICES": [1,2,3]}``.
-        """
-        cmd, devices_info = self._create_cmd(train_params)
-        return self._run_cmd(cmd, devices_info)
+            train_params:  training parameters
+            device_settings: device related settings, should follow the device_setting in auto_runner.set_device_info.
+            'CUDA_VISIBLE_DEVICES' should be a string e.g. '0,1,2,3'
+        """
+        if device_setting is not None:
+            self.device_setting.update(device_setting)
+            self.device_setting["n_devices"] = len(str(self.device_setting["CUDA_VISIBLE_DEVICES"]).split(","))
+
+        if train_params is not None and "CUDA_VISIBLE_DEVICES" in train_params:
+            warnings.warn("CUDA_VISIBLE_DEVICES is deprecated from train_params!")
+            train_params.pop("CUDA_VISIBLE_DEVICES")
+
+        cmd, _unused_return = self._create_cmd(train_params)
+        return self._run_cmd(cmd)
 
     def get_score(self, *args, **kwargs):
         """
         Returns validation scores of the model trained by the current Algo.
         """
         config_yaml = os.path.join(self.output_path, "configs", "hyper_parameters.yaml")
         parser = ConfigParser()
@@ -272,19 +308,15 @@
         Use the trained model to predict the outputs with a given input image.
 
         Args:
             predict_files: a list of paths to files to run inference on ["path_to_image_1", "path_to_image_2"]
             predict_params: a dict to override the parameters in the bundle config (including the files to predict).
 
         """
-        if predict_params is None:
-            params = {}
-        else:
-            params = deepcopy(predict_params)
-
+        params = {} if predict_params is None else deepcopy(predict_params)
         inferer = self.get_inferer(**params)
         return [inferer.infer(f) for f in ensure_tuple(predict_files)]
 
     def get_output_path(self):
         """Returns the algo output paths to find the algo scripts and configs."""
         return self.output_path
 
@@ -351,15 +383,15 @@
 
     algos_all = {}
     for name in os.listdir(at_path):
         if os.path.exists(os.path.join(folder, name, "scripts", "algo.py")):
             algos_all[name] = dict(
                 _target_=f"{name}.scripts.algo.{name.capitalize()}Algo", template_path=os.path.join(at_path, name)
             )
-            logger.info(f"{name} -- {algos_all[name]}")
+            logger.info(f"Copying template: {name} -- {algos_all[name]}")
     if not algos_all:
         raise ValueError(f"Unable to find any algos in {folder}")
 
     return algos_all
 
 
 class BundleGen(AlgoGen):
@@ -369,19 +401,18 @@
     Args:
         algo_path: the directory path to save the algorithm templates. Default is the current working dir.
         algos: If dictionary, it outlines the algorithm to use. If a list or a string, defines a subset of names of
             the algorithms to use, e.g. ('segresnet', 'dints') out of the full set of algorithm templates provided
             by templates_path_or_url. Defaults to None - to use all available algorithms.
         templates_path_or_url: the folder with the algorithm templates or a url. If None provided, the default template
             zip url will be downloaded and extracted into the algo_path. The current default options are released at:
-            https://github.com/Project-MONAI/research-contributions/tree/main/auto3dseg
-        data_stats_filename: the path to the data stats file (generated by DataAnalyzer)
+            https://github.com/Project-MONAI/research-contributions/tree/main/auto3dseg.
+        data_stats_filename: the path to the data stats file (generated by DataAnalyzer).
         data_src_cfg_name: the path to the data source config YAML file. The config will be in a form of
-            {"modality": "ct", "datalist": "path_to_json_datalist", "dataroot": "path_dir_data"}
-
+                           {"modality": "ct", "datalist": "path_to_json_datalist", "dataroot": "path_dir_data"}.
     .. code-block:: bash
 
         python -m monai.apps.auto3dseg BundleGen generate --data_stats_filename="../algorithms/datastats.yaml"
     """
 
     def __init__(
         self,
@@ -413,15 +444,15 @@
                 if len(algos) == 0:
                     raise ValueError(f"Unable to find provided algos in {algos_all}")
             else:
                 algos = algos_all
 
         self.algos: Any = []
         if isinstance(algos, dict):
-            for algo_name, algo_params in algos.items():
+            for algo_name, algo_params in sorted(algos.items()):
                 template_path = os.path.dirname(algo_params.get("template_path", "."))
                 if len(template_path) > 0 and template_path not in sys.path:
                     sys.path.append(template_path)
 
                 try:
                     onealgo = ConfigParser(algo_params).get_parsed_content()
                     onealgo.name = algo_name
@@ -535,9 +566,9 @@
                         gpu_customization_specs=gpu_customization_specs,
                     )
                 else:
                     gen_algo.export_to_disk(output_folder, name, fold=f_id)
 
                 algo_to_pickle(gen_algo, template_path=algo.template_path)
                 self.history.append(
-                    {AlgoEnsembleKeys.ID: name, AlgoEnsembleKeys.ALGO: gen_algo}
+                    {AlgoKeys.ID: name, AlgoKeys.ALGO: gen_algo}
                 )  # track the previous, may create a persistent history
```

### Comparing `monai-weekly-1.2.dev2315/monai/apps/auto3dseg/data_analyzer.py` & `monai-weekly-1.2.dev2316/monai/apps/auto3dseg/data_analyzer.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,22 +13,23 @@
 
 import warnings
 from os import path
 from typing import Any, cast
 
 import numpy as np
 import torch
+from torch.multiprocessing import get_context
 
 from monai.apps.auto3dseg.transforms import EnsureSameShaped
 from monai.apps.utils import get_logger
 from monai.auto3dseg import SegSummarizer
 from monai.auto3dseg.utils import datafold_read
 from monai.bundle import config_parser
 from monai.bundle.config_parser import ConfigParser
-from monai.data import DataLoader, Dataset
+from monai.data import DataLoader, Dataset, partition_dataset
 from monai.data.utils import no_collation
 from monai.transforms import Compose, EnsureTyped, LoadImaged, Orientationd
 from monai.utils import StrEnum, min_version, optional_import
 from monai.utils.enums import DataStatsKeys, ImageStatsKeys
 
 
 def strenum_representer(dumper, data):
@@ -57,16 +58,15 @@
         datalist: a Python dictionary storing group, fold, and other information of the medical
             image dataset, or a string to the JSON file storing the dictionary.
         dataroot: user's local directory containing the datasets.
         output_path: path to save the analysis result.
         average: whether to average the statistical value across different image modalities.
         do_ccp: apply the connected component algorithm to process the labels/images
         device: a string specifying hardware (CUDA/CPU) utilized for the operations.
-        worker: number of workers to use for parallel processing. If device is cuda/GPU, worker has
-            to be 0.
+        worker: number of workers to use for loading datasets in each GPU/CPU sub-process.
         image_key: a string that user specify for the image. The DataAnalyzer will look it up in the
             datalist to locate the image files of the dataset.
         label_key: a string that user specify for the label. The DataAnalyzer will look it up in the
             datalist to locate the label files of the dataset. If label_key is NoneType or "None",
             the DataAnalyzer will skip looking for labels and all label-related operations.
         hist_bins: bins to compute histogram for each image channel.
         hist_range: ranges to compute histogram for each image channel.
@@ -114,15 +114,15 @@
     def __init__(
         self,
         datalist: str | dict,
         dataroot: str = "",
         output_path: str = "./datastats.yaml",
         average: bool = True,
         do_ccp: bool = False,
-        device: str | torch.device = "cpu",
+        device: str | torch.device = "cuda",
         worker: int = 4,
         image_key: str = "image",
         label_key: str | None = "label",
         hist_bins: list | int | None = 0,
         hist_range: list | None = None,
         fmt: str = "yaml",
         histogram_only: bool = False,
@@ -166,16 +166,17 @@
             if "stdev" in prop and np.any(prop["stdev"]):
                 return False
 
         return True
 
     def get_all_case_stats(self, key="training", transform_list=None):
         """
-        Get all case stats. Caller of the DataAnalyser class. The function iterates datalist and
-        call get_case_stats to generate stats. Then get_case_summary is called to combine results.
+        Get all case stats. Caller of the DataAnalyser class. The function initiates multiple GPU or CPU processes of the internal
+        _get_all_case_stats functions, which iterates datalist and call SegSummarizer to generate stats for each case.
+        After all case stats are generated, SegSummarizer is called to combine results.
 
         Args:
             key: dataset key
             transform_list: option list of transforms before SegSummarizer
 
         Returns:
             A data statistics dictionary containing
@@ -193,14 +194,94 @@
 
         Notes:
             Since the backend of the statistics computation are torch/numpy, nan/inf value
             may be generated and carried over in the computation. In such cases, the output
             dictionary will include .nan/.inf in the statistics.
 
         """
+        result: dict[DataStatsKeys, Any] = {DataStatsKeys.SUMMARY: {}, DataStatsKeys.BY_CASE: []}
+        result_bycase: dict[DataStatsKeys, Any] = {DataStatsKeys.SUMMARY: {}, DataStatsKeys.BY_CASE: []}
+        if self.device.type == "cpu":
+            nprocs = 1
+            logger.info("Using CPU for data analyzing!")
+        else:
+            nprocs = torch.cuda.device_count()
+            logger.info(f"Found {nprocs} GPUs for data analyzing!")
+        if nprocs > 1:
+            tmp_ctx = get_context("forkserver")
+            with tmp_ctx.Manager() as manager:
+                manager_list = manager.list()
+                processes = []
+                for rank in range(nprocs):
+                    p = tmp_ctx.Process(
+                        target=self._get_all_case_stats, args=(rank, nprocs, manager_list, key, transform_list)
+                    )
+                    processes.append(p)
+                for p in processes:
+                    p.start()
+                for p in processes:
+                    p.join()
+                # merge DataStatsKeys.BY_CASE
+                for _ in manager_list:
+                    result_bycase[DataStatsKeys.BY_CASE].extend(_[DataStatsKeys.BY_CASE])
+        else:
+            result_bycase = self._get_all_case_stats(0, 1, None, key, transform_list)
+
+        summarizer = SegSummarizer(
+            self.image_key,
+            self.label_key,
+            average=self.average,
+            do_ccp=self.do_ccp,
+            hist_bins=self.hist_bins,
+            hist_range=self.hist_range,
+            histogram_only=self.histogram_only,
+        )
+        n_cases = len(result_bycase[DataStatsKeys.BY_CASE])
+        result[DataStatsKeys.SUMMARY] = summarizer.summarize(cast(list, result_bycase[DataStatsKeys.BY_CASE]))
+        result[DataStatsKeys.SUMMARY]["n_cases"] = n_cases
+        result[DataStatsKeys.BY_CASE] = [None] * n_cases
+        result_bycase[DataStatsKeys.SUMMARY] = result[DataStatsKeys.SUMMARY]
+        if not self._check_data_uniformity([ImageStatsKeys.SPACING], result):
+            logger.info("Data spacing is not completely uniform. MONAI transforms may provide unexpected result")
+        if self.output_path:
+            ConfigParser.export_config_file(
+                result, self.output_path, fmt=self.fmt, default_flow_style=None, sort_keys=False
+            )
+            ConfigParser.export_config_file(
+                result_bycase,
+                self.output_path.replace(".yaml", "_by_case.yaml"),
+                fmt=self.fmt,
+                default_flow_style=None,
+                sort_keys=False,
+            )
+        # release memory
+        if self.device.type == "cuda":
+            # release unreferenced tensors to mitigate OOM
+            # limitation: https://github.com/pytorch/pytorch/issues/12873#issuecomment-482916237
+            torch.cuda.empty_cache()
+        result[DataStatsKeys.BY_CASE] = result_bycase[DataStatsKeys.BY_CASE]
+        return result
+
+    def _get_all_case_stats(
+        self,
+        rank: int = 0,
+        world_size: int = 1,
+        manager_list: list | None = None,
+        key: str = "training",
+        transform_list: list | None = None,
+    ) -> Any:
+        """
+        Get all case stats from a partitioned datalist. The function can only be called internally by get_all_case_stats.
+        Args:
+            rank: GPU process rank, 0 for CPU process
+            world_size: total number of GPUs, 1 for CPU process
+            manager_list: multiprocessing manager list object, if using multi-GPU.
+            key: dataset key
+            transform_list: option list of transforms before SegSummarizer
+        """
         summarizer = SegSummarizer(
             self.image_key,
             self.label_key,
             average=self.average,
             do_ccp=self.do_ccp,
             hist_bins=self.hist_bins,
             hist_range=self.hist_range,
@@ -220,41 +301,56 @@
                         keys=self.label_key,
                         source_key=self.image_key,
                         allowed_shape_difference=allowed_shape_difference,
                     )
                 )
 
         transform = Compose(transform_list)
-
         files, _ = datafold_read(datalist=self.datalist, basedir=self.dataroot, fold=-1, key=key)
+        if world_size <= len(files):
+            files = partition_dataset(data=files, num_partitions=world_size)[rank]
+        else:
+            files = partition_dataset(data=files, num_partitions=len(files))[rank] if rank < len(files) else []
         dataset = Dataset(data=files, transform=transform)
         dataloader = DataLoader(
             dataset,
             batch_size=1,
             shuffle=False,
             num_workers=self.worker,
             collate_fn=no_collation,
             pin_memory=self.device.type == "cuda",
         )
-        result: dict[DataStatsKeys, Any] = {DataStatsKeys.SUMMARY: {}, DataStatsKeys.BY_CASE: []}
         result_bycase: dict[DataStatsKeys, Any] = {DataStatsKeys.SUMMARY: {}, DataStatsKeys.BY_CASE: []}
-
+        device = self.device if self.device.type == "cpu" else torch.device("cuda", rank)
         if not has_tqdm:
             warnings.warn("tqdm is not installed. not displaying the caching progress.")
 
-        for batch_data in tqdm(dataloader) if has_tqdm else dataloader:
+        for batch_data in tqdm(dataloader) if (has_tqdm and rank == 0) else dataloader:
             batch_data = batch_data[0]
-            batch_data[self.image_key] = batch_data[self.image_key].to(self.device)
-
-            if self.label_key is not None:
-                label = batch_data[self.label_key]
-                label = torch.argmax(label, dim=0) if label.shape[0] > 1 else label[0]
-                batch_data[self.label_key] = label.to(self.device)
-
-            d = summarizer(batch_data)
+            try:
+                batch_data[self.image_key] = batch_data[self.image_key].to(device)
+                if self.label_key is not None:
+                    label = batch_data[self.label_key]
+                    label = torch.argmax(label, dim=0) if label.shape[0] > 1 else label[0]
+                    batch_data[self.label_key] = label.to(device)
+                d = summarizer(batch_data)
+            except BaseException:
+                if "image_meta_dict" in batch_data.keys():
+                    filename = batch_data["image_meta_dict"]["filename_or_obj"]
+                else:
+                    filename = batch_data[self.image_key].meta["filename_or_obj"]
+                logger.info(f"Unable to process data {filename} on {device}.")
+                if self.device.type == "cuda":
+                    logger.info("DataAnalyzer `device` set to GPU execution hit an exception. Falling back to `cpu`.")
+                    batch_data[self.image_key] = batch_data[self.image_key].to("cpu")
+                    if self.label_key is not None:
+                        label = batch_data[self.label_key]
+                        label = torch.argmax(label, dim=0) if label.shape[0] > 1 else label[0]
+                        batch_data[self.label_key] = label.to("cpu")
+                    d = summarizer(batch_data)
 
             stats_by_cases = {
                 DataStatsKeys.BY_CASE_IMAGE_PATH: d[DataStatsKeys.BY_CASE_IMAGE_PATH],
                 DataStatsKeys.BY_CASE_LABEL_PATH: d[DataStatsKeys.BY_CASE_LABEL_PATH],
                 DataStatsKeys.IMAGE_STATS: d[DataStatsKeys.IMAGE_STATS],
             }
             if self.hist_bins != 0:
@@ -264,40 +360,11 @@
                 stats_by_cases.update(
                     {
                         DataStatsKeys.FG_IMAGE_STATS: d[DataStatsKeys.FG_IMAGE_STATS],
                         DataStatsKeys.LABEL_STATS: d[DataStatsKeys.LABEL_STATS],
                     }
                 )
             result_bycase[DataStatsKeys.BY_CASE].append(stats_by_cases)
-
-        n_cases = len(result_bycase[DataStatsKeys.BY_CASE])
-
-        result[DataStatsKeys.SUMMARY] = summarizer.summarize(cast(list, result_bycase[DataStatsKeys.BY_CASE]))
-        result[DataStatsKeys.SUMMARY]["n_cases"] = n_cases
-        result[DataStatsKeys.BY_CASE] = [None] * n_cases
-
-        if not self._check_data_uniformity([ImageStatsKeys.SPACING], result):
-            print("Data spacing is not completely uniform. MONAI transforms may provide unexpected result")
-
-        if self.output_path:
-            # saving summary and by_case as 2 files, to minimize loading time when only the summary is necessary
-            ConfigParser.export_config_file(
-                result, self.output_path, fmt=self.fmt, default_flow_style=None, sort_keys=False
-            )
-            ConfigParser.export_config_file(
-                result_bycase,
-                self.output_path.replace(".yaml", "_by_case.yaml"),
-                fmt=self.fmt,
-                default_flow_style=None,
-                sort_keys=False,
-            )
-
-        # release memory
-        d = None
-        if self.device.type == "cuda":
-            # release unreferenced tensors to mitigate OOM
-            # limitation: https://github.com/pytorch/pytorch/issues/12873#issuecomment-482916237
-            torch.cuda.empty_cache()
-
-        # return combined
-        result[DataStatsKeys.BY_CASE] = result_bycase[DataStatsKeys.BY_CASE]
-        return result
+        if manager_list is None:
+            return result_bycase
+        else:
+            manager_list.append(result_bycase)
```

### Comparing `monai-weekly-1.2.dev2315/monai/apps/auto3dseg/hpo_gen.py` & `monai-weekly-1.2.dev2316/monai/apps/auto3dseg/hpo_gen.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from monai.apps.auto3dseg.bundle_gen import BundleAlgo
 from monai.apps.utils import get_logger
 from monai.auto3dseg import Algo, AlgoGen, algo_from_pickle, algo_to_pickle
 from monai.bundle.config_parser import ConfigParser
 from monai.config import PathLike
 from monai.utils import optional_import
-from monai.utils.enums import AlgoEnsembleKeys
+from monai.utils.enums import AlgoKeys
 
 nni, has_nni = optional_import("nni")
 optuna, has_optuna = optional_import("optuna")
 logger = get_logger(module_name=__name__)
 
 __all__ = ["HPOGen", "NNIGen", "OptunaGen"]
 
@@ -95,16 +95,16 @@
             ├── model_fold0
             └── scripts
 
         .. code-block:: python
             # Bundle Algorithms are already generated by BundleGen in work_dir
             import_bundle_algo_history(work_dir, only_trained=False)
             algo_dict = self.history[0]  # pick the first algorithm
-            algo_name = algo_dict[AlgoEnsembleKeys.ID]
-            onealgo = algo_dict[AlgoEnsembleKeys.ALGO]
+            algo_name = algo_dict[AlgoKeys.ID]
+            onealgo = algo_dict[AlgoKeys.ALGO]
             nni_gen = NNIGen(algo=onealgo)
             nni_gen.print_bundle_algo_instruction()
 
     Notes:
         The NNIGen will prepare the algorithms in a folder and suggest a command to replace trialCommand in the experiment
         config. However, NNIGen will not trigger NNI. User needs to write their NNI experiment configs, and then run the
         NNI command manually.
@@ -234,15 +234,15 @@
         # step 2 set the update params for the algo to run in the next trial
         self.update_params(params)
         # step 3 generate the folder to save checkpoints and train
         self.generate(output_folder)
         self.algo.train(self.params)
         # step 4 report validation acc to controller
         acc = self.algo.get_score()
-        algo_meta_data = {str(AlgoEnsembleKeys.SCORE): acc}
+        algo_meta_data = {str(AlgoKeys.SCORE): acc}
 
         if isinstance(self.algo, BundleAlgo):
             algo_to_pickle(self.algo, template_path=self.algo.template_path, **algo_meta_data)
         else:
             algo_to_pickle(self.algo, **algo_meta_data)
         self.set_score(acc)
 
@@ -407,13 +407,13 @@
         # step 2 set the update params for the algo to run in the next trial
         self.update_params(params)
         # step 3 generate the folder to save checkpoints and train
         self.generate(output_folder)
         self.algo.train(self.params)
         # step 4 report validation acc to controller
         acc = self.algo.get_score()
-        algo_meta_data = {str(AlgoEnsembleKeys.SCORE): acc}
+        algo_meta_data = {str(AlgoKeys.SCORE): acc}
         if isinstance(self.algo, BundleAlgo):
             algo_to_pickle(self.algo, template_path=self.algo.template_path, **algo_meta_data)
         else:
             algo_to_pickle(self.algo, **algo_meta_data)
         self.set_score(acc)
```

### Comparing `monai-weekly-1.2.dev2315/monai/apps/auto3dseg/transforms.py` & `monai-weekly-1.2.dev2316/monai/apps/auto3dseg/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/auto3dseg/utils.py` & `monai-weekly-1.2.dev2316/monai/apps/auto3dseg/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from __future__ import annotations
 
 import os
 
 from monai.apps.auto3dseg.bundle_gen import BundleAlgo
 from monai.auto3dseg import algo_from_pickle, algo_to_pickle
-from monai.utils.enums import AlgoEnsembleKeys
+from monai.utils.enums import AlgoKeys
 
 
 def import_bundle_algo_history(
     output_folder: str = ".", template_path: str | None = None, only_trained: bool = True
 ) -> list:
     """
     import the history of the bundleAlgo objects as a list of algo dicts.
@@ -45,33 +45,28 @@
             continue
 
         algo, algo_meta_data = algo_from_pickle(obj_filename, template_path=template_path)
 
         if isinstance(algo, BundleAlgo):  # algo's template path needs override
             algo.template_path = algo_meta_data["template_path"]
 
-        best_metric = algo_meta_data.get(AlgoEnsembleKeys.SCORE, None)
+        best_metric = algo_meta_data.get(AlgoKeys.SCORE, None)
         is_trained = best_metric is not None
 
         if (only_trained and is_trained) or not only_trained:
             history.append(
-                {
-                    AlgoEnsembleKeys.ID: name,
-                    AlgoEnsembleKeys.ALGO: algo,
-                    AlgoEnsembleKeys.SCORE: best_metric,
-                    "is_trained": is_trained,
-                }
+                {AlgoKeys.ID: name, AlgoKeys.ALGO: algo, AlgoKeys.SCORE: best_metric, AlgoKeys.IS_TRAINED: is_trained}
             )
 
     return history
 
 
 def export_bundle_algo_history(history: list[dict[str, BundleAlgo]]) -> None:
     """
     Save all the BundleAlgo in the history to algo_object.pkl in each individual folder
 
     Args:
         history: a List of Bundle. Typically, the history can be obtained from BundleGen get_history method
     """
     for algo_dict in history:
-        algo = algo_dict[AlgoEnsembleKeys.ALGO]
+        algo = algo_dict[AlgoKeys.ALGO]
         algo_to_pickle(algo, template_path=algo.template_path)
```

### Comparing `monai-weekly-1.2.dev2315/monai/apps/datasets.py` & `monai-weekly-1.2.dev2316/monai/apps/datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/deepedit/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/deepedit/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/deepedit/interaction.py` & `monai-weekly-1.2.dev2316/monai/apps/deepedit/interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/deepedit/transforms.py` & `monai-weekly-1.2.dev2316/monai/apps/deepedit/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/deepgrow/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/deepgrow/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/deepgrow/dataset.py` & `monai-weekly-1.2.dev2316/monai/apps/deepgrow/dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/deepgrow/interaction.py` & `monai-weekly-1.2.dev2316/monai/apps/deepgrow/interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/deepgrow/transforms.py` & `monai-weekly-1.2.dev2316/monai/apps/deepgrow/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/detection/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/detection/metrics/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/detection/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/detection/metrics/coco.py` & `monai-weekly-1.2.dev2316/monai/apps/detection/metrics/coco.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/detection/metrics/matching.py` & `monai-weekly-1.2.dev2316/monai/apps/detection/metrics/matching.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/detection/networks/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/detection/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/detection/networks/retinanet_detector.py` & `monai-weekly-1.2.dev2316/monai/apps/detection/networks/retinanet_detector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/detection/networks/retinanet_network.py` & `monai-weekly-1.2.dev2316/monai/apps/detection/networks/retinanet_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/detection/transforms/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/detection/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/detection/transforms/array.py` & `monai-weekly-1.2.dev2316/monai/apps/detection/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/detection/transforms/box_ops.py` & `monai-weekly-1.2.dev2316/monai/apps/detection/transforms/box_ops.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/detection/transforms/dictionary.py` & `monai-weekly-1.2.dev2316/monai/apps/detection/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/detection/utils/ATSS_matcher.py` & `monai-weekly-1.2.dev2316/monai/apps/detection/utils/ATSS_matcher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/detection/utils/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/detection/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/detection/utils/anchor_utils.py` & `monai-weekly-1.2.dev2316/monai/apps/detection/utils/anchor_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/detection/utils/box_coder.py` & `monai-weekly-1.2.dev2316/monai/apps/detection/utils/box_coder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/detection/utils/box_selector.py` & `monai-weekly-1.2.dev2316/monai/apps/detection/utils/box_selector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/detection/utils/detector_utils.py` & `monai-weekly-1.2.dev2316/monai/apps/detection/utils/detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/detection/utils/hard_negative_sampler.py` & `monai-weekly-1.2.dev2316/monai/apps/detection/utils/hard_negative_sampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/detection/utils/predict_utils.py` & `monai-weekly-1.2.dev2316/monai/apps/detection/utils/predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/mmars/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/mmars/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/mmars/mmars.py` & `monai-weekly-1.2.dev2316/monai/apps/mmars/mmars.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/mmars/model_desc.py` & `monai-weekly-1.2.dev2316/monai/apps/mmars/model_desc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/nnunet/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/nnunet/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/nnunet/__main__.py` & `monai-weekly-1.2.dev2316/monai/apps/nnunet/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/nnunet/nnunetv2_runner.py` & `monai-weekly-1.2.dev2316/monai/apps/nnunet/nnunetv2_runner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/nnunet/utils.py` & `monai-weekly-1.2.dev2316/monai/apps/nnunet/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/nuclick/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/nuclick/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/nuclick/transforms.py` & `monai-weekly-1.2.dev2316/monai/apps/nuclick/transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/pathology/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/pathology/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/pathology/engines/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/pathology/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/pathology/engines/utils.py` & `monai-weekly-1.2.dev2316/monai/apps/pathology/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/pathology/handlers/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/pathology/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/pathology/handlers/utils.py` & `monai-weekly-1.2.dev2316/monai/apps/pathology/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/pathology/inferers/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/pathology/inferers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/pathology/inferers/inferer.py` & `monai-weekly-1.2.dev2316/monai/apps/pathology/inferers/inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/pathology/losses/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/pathology/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/pathology/losses/hovernet_loss.py` & `monai-weekly-1.2.dev2316/monai/apps/pathology/losses/hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/pathology/metrics/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/pathology/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/pathology/metrics/lesion_froc.py` & `monai-weekly-1.2.dev2316/monai/apps/pathology/metrics/lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/pathology/transforms/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/pathology/transforms/post/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/pathology/transforms/post/array.py` & `monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/post/array.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     RemoveSmallObjects,
     SobelGradients,
 )
 from monai.transforms.transform import Transform
 from monai.transforms.utils_pytorch_numpy_unification import max, maximum, min, sum, unique
 from monai.utils import TransformBackends, convert_to_numpy, optional_import
 from monai.utils.misc import ensure_tuple_rep
-from monai.utils.type_conversion import convert_to_dst_type
+from monai.utils.type_conversion import convert_to_dst_type, convert_to_tensor
 
 label, _ = optional_import("scipy.ndimage.measurements", name="label")
 disk, _ = optional_import("skimage.morphology", name="disk")
 opening, _ = optional_import("skimage.morphology", name="opening")
 watershed, _ = optional_import("skimage.segmentation", name="watershed")
 find_contours, _ = optional_import("skimage.measure", name="find_contours")
 centroid, _ = optional_import("skimage.measure", name="centroid")
@@ -667,14 +667,15 @@
         marker_radius: the radius of the disk-shaped footprint used in `opening` of markers. Defaults to 2.
         marker_postprocess_fn: post-process function for watershed markers.
             If not provided, :py:class:`monai.transforms.post.FillHoles()` will be used.
         watershed_connectivity: `connectivity` argument of `skimage.segmentation.watershed`.
         min_num_points: minimum number of points to be considered as a contour. Defaults to 3.
         contour_level: an optional value for `skimage.measure.find_contours` to find contours in the array.
             If not provided, the level is set to `(max(image) + min(image)) / 2`.
+        device: target device to put the output Tensor data.
     """
 
     def __init__(
         self,
         activation: str | Callable = "softmax",
         mask_threshold: float | None = None,
         min_object_size: int = 10,
@@ -682,17 +683,18 @@
         distance_smooth_fn: Callable | None = None,
         marker_threshold: float = 0.4,
         marker_radius: int = 2,
         marker_postprocess_fn: Callable | None = None,
         watershed_connectivity: int | None = 1,
         min_num_points: int = 3,
         contour_level: float | None = None,
+        device: str | torch.device | None = None,
     ) -> None:
         super().__init__()
-
+        self.device = device
         self.generate_watershed_mask = GenerateWatershedMask(
             activation=activation, threshold=mask_threshold, min_object_size=min_object_size
         )
         self.generate_instance_border = GenerateInstanceBorder(kernel_size=sobel_kernel_size)
         self.generate_distance_map = GenerateDistanceMap(smooth_fn=distance_smooth_fn)
         self.generate_watershed_markers = GenerateWatershedMarkers(
             threshold=marker_threshold,
@@ -738,15 +740,15 @@
             if instance_contour is not None:
                 instance_centroid = self.generate_instance_centroid(instance_mask, offset)
                 instance_info[inst_id] = {
                     "bounding_box": instance_bbox,
                     "centroid": instance_centroid,
                     "contour": instance_contour,
                 }
-
+        instance_map = convert_to_tensor(instance_map, device=self.device)
         return instance_info, instance_map
 
 
 class HoVerNetNuclearTypePostProcessing(Transform):
     """
     The post-processing transform for HoVerNet model to generate nuclear type information.
     It updates the input instance info dictionary with information about types of the nuclei (value and probability).
@@ -754,21 +756,27 @@
 
     Args:
         activation: the activation layer to be applied on nuclear type branch. It can be "softmax" or "sigmoid" string,
             or any callable. Defaults to "softmax".
         threshold: an optional float value to threshold to binarize probability map.
             If not provided, defaults to 0.5 when activation is not "softmax", otherwise None.
         return_type_map: whether to calculate and return pixel-level type map.
+        device: target device to put the output Tensor data.
 
     """
 
     def __init__(
-        self, activation: str | Callable = "softmax", threshold: float | None = None, return_type_map: bool = True
+        self,
+        activation: str | Callable = "softmax",
+        threshold: float | None = None,
+        return_type_map: bool = True,
+        device: str | torch.device | None = None,
     ) -> None:
         super().__init__()
+        self.device = device
         self.return_type_map = return_type_map
         self.generate_instance_type = GenerateInstanceType()
 
         # set activation layer
         use_softmax = False
         use_sigmoid = False
         activation_fn = None
@@ -820,9 +828,10 @@
             # update instance info dict with type data
             instance_info[inst_id]["type_prob"] = instance_type_prob
             instance_info[inst_id]["type"] = instance_type
 
             # update instance type map
             if type_map is not None:
                 type_map[instance_map == inst_id] = instance_type
+                type_map = convert_to_tensor(type_map, device=self.device)
 
         return instance_info, type_map
```

### Comparing `monai-weekly-1.2.dev2315/monai/apps/pathology/transforms/post/dictionary.py` & `monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/post/dictionary.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 from collections.abc import Callable, Hashable, Mapping
 
 import numpy as np
+import torch
 
 from monai.apps.pathology.transforms.post.array import (
     GenerateDistanceMap,
     GenerateInstanceBorder,
     GenerateInstanceCentroid,
     GenerateInstanceContour,
     GenerateInstanceType,
@@ -484,14 +485,15 @@
         marker_radius: the radius of the disk-shaped footprint used in `opening` of markers. Defaults to 2.
         marker_postprocess_fn: post-process function for watershed markers.
             If not provided, :py:class:`monai.transforms.post.FillHoles()` will be used.
         watershed_connectivity: `connectivity` argument of `skimage.segmentation.watershed`.
         min_num_points: minimum number of points to be considered as a contour. Defaults to 3.
         contour_level: an optional value for `skimage.measure.find_contours` to find contours in the array.
             If not provided, the level is set to `(max(image) + min(image)) / 2`.
+        device: target device to put the output Tensor data.
     """
 
     def __init__(
         self,
         nuclear_prediction_key: str = HoVerNetBranch.NP.value,
         hover_map_key: str = HoVerNetBranch.HV.value,
         instance_info_key: str = "instance_info",
@@ -503,28 +505,30 @@
         distance_smooth_fn: Callable | None = None,
         marker_threshold: float = 0.4,
         marker_radius: int = 2,
         marker_postprocess_fn: Callable | None = None,
         watershed_connectivity: int | None = 1,
         min_num_points: int = 3,
         contour_level: float | None = None,
+        device: str | torch.device | None = None,
     ) -> None:
         super().__init__()
         self.instance_map_post_process = HoVerNetInstanceMapPostProcessing(
             activation=activation,
             mask_threshold=mask_threshold,
             min_object_size=min_object_size,
             sobel_kernel_size=sobel_kernel_size,
             distance_smooth_fn=distance_smooth_fn,
             marker_threshold=marker_threshold,
             marker_radius=marker_radius,
             marker_postprocess_fn=marker_postprocess_fn,
             watershed_connectivity=watershed_connectivity,
             min_num_points=min_num_points,
             contour_level=contour_level,
+            device=device,
         )
         self.nuclear_prediction_key = nuclear_prediction_key
         self.hover_map_key = hover_map_key
         self.instance_info_key = instance_info_key
         self.instance_map_key = instance_map_key
 
     def __call__(self, data):
@@ -549,31 +553,32 @@
 
     Args:
         type_prediction_key: the key for HoVerNet NC (type prediction) branch. Defaults to `HoVerNetBranch.NC`.
         instance_info_key: the key where instance information (contour, bounding boxes, and centroids) is stored.
             Defaults to `"instance_info"`.
         instance_map_key: the key where instance map is stored. Defaults to `"instance_map"`.
         type_map_key: the output key where type map is written. Defaults to `"type_map"`.
-
+        device: target device to put the output Tensor data.
 
     """
 
     def __init__(
         self,
         type_prediction_key: str = HoVerNetBranch.NC.value,
         instance_info_key: str = "instance_info",
         instance_map_key: str = "instance_map",
         type_map_key: str = "type_map",
         activation: str | Callable = "softmax",
         threshold: float | None = None,
         return_type_map: bool = True,
+        device: str | torch.device | None = None,
     ) -> None:
         super().__init__()
         self.type_post_process = HoVerNetNuclearTypePostProcessing(
-            activation=activation, threshold=threshold, return_type_map=return_type_map
+            activation=activation, threshold=threshold, return_type_map=return_type_map, device=device
         )
         self.type_prediction_key = type_prediction_key
         self.instance_info_key = instance_info_key
         self.instance_map_key = instance_map_key
         self.type_map_key = type_map_key
         self.return_type_map = return_type_map
```

### Comparing `monai-weekly-1.2.dev2315/monai/apps/pathology/transforms/stain/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/stain/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/pathology/transforms/stain/array.py` & `monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/stain/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/pathology/transforms/stain/dictionary.py` & `monai-weekly-1.2.dev2316/monai/apps/pathology/transforms/stain/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/pathology/utils.py` & `monai-weekly-1.2.dev2316/monai/apps/pathology/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/reconstruction/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/reconstruction/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/reconstruction/complex_utils.py` & `monai-weekly-1.2.dev2316/monai/apps/reconstruction/complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/reconstruction/fastmri_reader.py` & `monai-weekly-1.2.dev2316/monai/apps/reconstruction/fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/reconstruction/mri_utils.py` & `monai-weekly-1.2.dev2316/monai/apps/reconstruction/mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/reconstruction/networks/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/reconstruction/networks/blocks/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/reconstruction/networks/blocks/varnetblock.py` & `monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/blocks/varnetblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/reconstruction/networks/nets/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py` & `monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/coil_sensitivity_model.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/reconstruction/networks/nets/complex_unet.py` & `monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/complex_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/reconstruction/networks/nets/utils.py` & `monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/reconstruction/networks/nets/varnet.py` & `monai-weekly-1.2.dev2316/monai/apps/reconstruction/networks/nets/varnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/reconstruction/transforms/__init__.py` & `monai-weekly-1.2.dev2316/monai/apps/reconstruction/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/reconstruction/transforms/array.py` & `monai-weekly-1.2.dev2316/monai/apps/reconstruction/transforms/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/reconstruction/transforms/dictionary.py` & `monai-weekly-1.2.dev2316/monai/apps/reconstruction/transforms/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/tcia/__init__.py` & `monai-weekly-1.2.dev2316/monai/optimizers/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,9 +7,11 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from .label_desc import TCIA_LABEL_DICT
-from .utils import download_tcia_series_instance, get_tcia_metadata, get_tcia_ref_uid, match_tcia_ref_uid_in_study
+from .lr_finder import LearningRateFinder
+from .lr_scheduler import ExponentialLR, LinearLR, WarmupCosineSchedule
+from .novograd import Novograd
+from .utils import generate_param_groups
```

### Comparing `monai-weekly-1.2.dev2315/monai/apps/tcia/label_desc.py` & `monai-weekly-1.2.dev2316/monai/apps/tcia/label_desc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/tcia/utils.py` & `monai-weekly-1.2.dev2316/monai/apps/tcia/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/apps/utils.py` & `monai-weekly-1.2.dev2316/monai/apps/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/auto3dseg/__init__.py` & `monai-weekly-1.2.dev2316/monai/auto3dseg/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/auto3dseg/algo_gen.py` & `monai-weekly-1.2.dev2316/monai/auto3dseg/algo_gen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/auto3dseg/analyzer.py` & `monai-weekly-1.2.dev2316/monai/auto3dseg/analyzer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/auto3dseg/operations.py` & `monai-weekly-1.2.dev2316/monai/auto3dseg/operations.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/auto3dseg/seg_summarizer.py` & `monai-weekly-1.2.dev2316/monai/auto3dseg/seg_summarizer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/auto3dseg/utils.py` & `monai-weekly-1.2.dev2316/monai/auto3dseg/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/bundle/__init__.py` & `monai-weekly-1.2.dev2316/monai/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/bundle/__main__.py` & `monai-weekly-1.2.dev2316/monai/bundle/__main__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/bundle/config_item.py` & `monai-weekly-1.2.dev2316/monai/bundle/config_item.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/bundle/config_parser.py` & `monai-weekly-1.2.dev2316/monai/bundle/config_parser.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/bundle/properties.py` & `monai-weekly-1.2.dev2316/monai/bundle/properties.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/bundle/reference_resolver.py` & `monai-weekly-1.2.dev2316/monai/bundle/reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/bundle/scripts.py` & `monai-weekly-1.2.dev2316/monai/bundle/scripts.py`

 * *Files 3% similar despite different names*

```diff
@@ -1138,17 +1138,17 @@
         meta_file: filepath of the metadata file, if it is a list of file paths, the content of them will be merged.
         config_file: filepath of the config file to save in TorchScript model and extract network information,
             the saved key in the TorchScript model is the config filename without extension, and the saved config
             value is always serialized in JSON format no matter the original file format is JSON or YAML.
             it can be a single file or a list of files. if `None`, must be provided in `args_file`.
         key_in_ckpt: for nested checkpoint like `{"model": XXX, "optimizer": XXX, ...}`, specify the key of model
             weights. if not nested checkpoint, no need to set.
-        use_trace: whether using `torch.jit.trace` to convert the pytorch model to torchscript model.
+        use_trace: whether using `torch.jit.trace` to convert the PyTorch model to TorchScript model.
         input_shape: a shape used to generate the random input of the network, when converting the model to a
-            torchscript model. Should be a list like [N, C, H, W] or [N, C, H, W, D]. If not given, will try to
+            TorchScript model. Should be a list like [N, C, H, W] or [N, C, H, W, D]. If not given, will try to
             parse from the `metadata` config.
         args_file: a JSON or YAML file to provide default values for all the parameters of this function, so that
             the command line inputs can be simplified.
         converter_kwargs: extra arguments that are needed by `convert_to_torchscript`, except ones that already exist
             in the input parameters.
         override: id-value pairs to override or add the corresponding config content.
             e.g. ``--_meta#network_data_format#inputs#image#num_channels 3``.
@@ -1229,51 +1229,71 @@
     config_file: str | Sequence[str] | None = None,
     key_in_ckpt: str | None = None,
     precision: str | None = None,
     input_shape: Sequence[int] | None = None,
     use_trace: bool | None = None,
     dynamic_batchsize: Sequence[int] | None = None,
     device: int | None = None,
+    use_onnx: bool | None = None,
+    onnx_input_names: Sequence[str] | None = None,
+    onnx_output_names: Sequence[str] | None = None,
     args_file: str | None = None,
     converter_kwargs: Mapping | None = None,
     **override: Any,
 ) -> None:
     """
-    Export the model checkpoint to the given filepath as a TensorRT engine-based torchscript.
+    Export the model checkpoint to the given filepath as a TensorRT engine-based TorchScript.
     Currently, this API only supports converting models whose inputs are all tensors.
 
+    There are two ways to export a model:
+    1, Torch-TensorRT way: PyTorch module ---> TorchScript module ---> TensorRT engine-based TorchScript.
+    2, ONNX-TensorRT way: PyTorch module ---> TorchScript module ---> ONNX model ---> TensorRT engine --->
+    TensorRT engine-based TorchScript.
+
+    When exporting through the first way, some models suffer from the slowdown problem, since Torch-TensorRT
+    may only convert a little part of the PyTorch model to the TensorRT engine. However when exporting through
+    the second way, some Python data structures like `dict` are not supported. And some TorchScript models are
+    not supported by the ONNX if exported through `torch.jit.script`.
+
     Typical usage examples:
 
     .. code-block:: bash
 
         python -m monai.bundle trt_export --net_id <network definition> --filepath <export path> \
             --ckpt_file <checkpoint path> --input_shape <input shape> --dynamic_batchsize <batch range> ...
 
     Args:
         net_id: ID name of the network component in the config, it must be `torch.nn.Module`.
         filepath: filepath to export, if filename has no extension, it becomes `.ts`.
         ckpt_file: filepath of the model checkpoint to load.
         meta_file: filepath of the metadata file, if it is a list of file paths, the content of them will be merged.
-        config_file: filepath of the config file to save in the TensorRT based torchscript model and extract network
+        config_file: filepath of the config file to save in the TensorRT based TorchScript model and extract network
             information, the saved key in the model is the config filename without extension, and the saved config
             value is always serialized in JSON format no matter the original file format is JSON or YAML.
             it can be a single file or a list of files. if `None`, must be provided in `args_file`.
         key_in_ckpt: for nested checkpoint like `{"model": XXX, "optimizer": XXX, ...}`, specify the key of model
             weights. if not nested checkpoint, no need to set.
-        precision: the weight precision of the converted TensorRT engine based torchscript models. Should be 'fp32' or 'fp16'.
+        precision: the weight precision of the converted TensorRT engine based TorchScript models. Should be 'fp32' or 'fp16'.
         input_shape: the input shape that is used to convert the model. Should be a list like [N, C, H, W] or
             [N, C, H, W, D]. If not given, will try to parse from the `metadata` config.
-        use_trace: whether using `torch.jit.trace` to convert the pytorch model to torchscript model and then convert to
-            a TensorRT engine based torchscript model.
+        use_trace: whether using `torch.jit.trace` to convert the PyTorch model to a TorchScript model and then convert to
+            a TensorRT engine based TorchScript model or an ONNX model (if `use_onnx` is True).
         dynamic_batchsize: a sequence with three elements to define the batch size range of the input for the model to be
             converted. Should be a sequence like [MIN_BATCH, OPT_BATCH, MAX_BATCH]. After converted, the batchsize of
             model input should between `MIN_BATCH` and `MAX_BATCH` and the `OPT_BATCH` is the best performance batchsize
             that the TensorRT tries to fit. The `OPT_BATCH` should be the most frequently used input batchsize in
             the application.
         device: the target GPU index to convert and verify the model.
+        use_onnx: whether using the ONNX-TensorRT way to export the TensorRT engine-based TorchScript model.
+        onnx_input_names: optional input names of the ONNX model. This arg is only useful when `use_onnx` is True. Should be
+            a sequence like `['input_0', 'input_1', ..., 'input_N']` where N equals to the number of the model inputs. If not
+            given, will use `['input_0']`, which supposes the model only has one input.
+        onnx_output_names: optional output names of the ONNX model. This arg is only useful when `use_onnx` is True. Should be
+            a sequence like `['output_0', 'output_1', ..., 'output_N']` where N equals to the number of the model outputs. If
+            not given, will use `['output_0']`, which supposes the model only has one output.
         args_file: a JSON or YAML file to provide default values for all the parameters of this function, so that
             the command line inputs can be simplified.
         converter_kwargs: extra arguments that are needed by `convert_to_trt`, except ones that already exist in the
             input parameters.
         override: id-value pairs to override or add the corresponding config content.
             e.g. ``--_meta#network_data_format#inputs#image#num_channels 3``.
 
@@ -1287,14 +1307,17 @@
         ckpt_file=ckpt_file,
         key_in_ckpt=key_in_ckpt,
         precision=precision,
         input_shape=input_shape,
         use_trace=use_trace,
         dynamic_batchsize=dynamic_batchsize,
         device=device,
+        use_onnx=use_onnx,
+        onnx_input_names=onnx_input_names,
+        onnx_output_names=onnx_output_names,
         converter_kwargs=converter_kwargs,
         **override,
     )
     _log_input_summary(tag="trt_export", args=_args)
     (
         filepath_,
         ckpt_file_,
@@ -1303,28 +1326,34 @@
         meta_file_,
         key_in_ckpt_,
         precision_,
         input_shape_,
         use_trace_,
         dynamic_batchsize_,
         device_,
+        use_onnx_,
+        onnx_input_names_,
+        onnx_output_names_,
         converter_kwargs_,
     ) = _pop_args(
         _args,
         "filepath",
         "ckpt_file",
         "config_file",
         net_id="",
         meta_file=None,
         key_in_ckpt="",
         precision="fp32",
         input_shape=[],
         use_trace=False,
         dynamic_batchsize=None,
         device=None,
+        use_onnx=False,
+        onnx_input_names=["input_0"],
+        onnx_output_names=["output_0"],
         converter_kwargs={},
     )
 
     parser = ConfigParser()
 
     parser.read_config(f=config_file_)
     if meta_file_ is not None:
@@ -1341,14 +1370,17 @@
 
     trt_api_parameters = {
         "precision": precision_,
         "input_shape": input_shape_,
         "dynamic_batchsize": dynamic_batchsize_,
         "use_trace": use_trace_,
         "device": device_,
+        "use_onnx": use_onnx_,
+        "onnx_input_names": onnx_input_names_,
+        "onnx_output_names": onnx_output_names_,
     }
     converter_kwargs_.update(trt_api_parameters)
 
     _export(
         convert_to_trt,
         parser,
         net_id=net_id_,
```

### Comparing `monai-weekly-1.2.dev2315/monai/bundle/utils.py` & `monai-weekly-1.2.dev2316/monai/bundle/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/bundle/workflows.py` & `monai-weekly-1.2.dev2316/monai/bundle/workflows.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/config/__init__.py` & `monai-weekly-1.2.dev2316/monai/config/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/config/deviceconfig.py` & `monai-weekly-1.2.dev2316/monai/config/deviceconfig.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/config/type_definitions.py` & `monai-weekly-1.2.dev2316/monai/config/type_definitions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/__init__.py` & `monai-weekly-1.2.dev2316/monai/data/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/box_utils.py` & `monai-weekly-1.2.dev2316/monai/data/box_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/csv_saver.py` & `monai-weekly-1.2.dev2316/monai/data/csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/dataloader.py` & `monai-weekly-1.2.dev2316/monai/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/dataset.py` & `monai-weekly-1.2.dev2316/monai/data/dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/dataset_summary.py` & `monai-weekly-1.2.dev2316/monai/data/dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/decathlon_datalist.py` & `monai-weekly-1.2.dev2316/monai/data/decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/fft_utils.py` & `monai-weekly-1.2.dev2316/monai/data/fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/folder_layout.py` & `monai-weekly-1.2.dev2316/monai/data/folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/grid_dataset.py` & `monai-weekly-1.2.dev2316/monai/data/grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/image_dataset.py` & `monai-weekly-1.2.dev2316/monai/data/image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/image_reader.py` & `monai-weekly-1.2.dev2316/monai/data/image_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/image_writer.py` & `monai-weekly-1.2.dev2316/monai/data/image_writer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/iterable_dataset.py` & `monai-weekly-1.2.dev2316/monai/data/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/itk_torch_bridge.py` & `monai-weekly-1.2.dev2316/monai/data/itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/meta_obj.py` & `monai-weekly-1.2.dev2316/monai/data/meta_obj.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/meta_tensor.py` & `monai-weekly-1.2.dev2316/monai/data/meta_tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -506,17 +506,24 @@
         See:
             - https://pytorch.org/docs/stable/generated/torch.Tensor.new_empty.html#torch-tensor-new-empty
         """
         return type(self)(
             self.as_tensor().new_empty(size=size, dtype=dtype, device=device, requires_grad=requires_grad)
         )
 
-    def clone(self):
-        """returns a copy of the MetaTensor instance."""
-        new_inst = MetaTensor(self.as_tensor().clone())
+    def clone(self, **kwargs):
+        """
+        Returns a copy of the MetaTensor instance.
+
+        Args:
+            kwargs: additional keyword arguments to `torch.clone`.
+
+        See also: https://pytorch.org/docs/stable/generated/torch.clone.html
+        """
+        new_inst = MetaTensor(self.as_tensor().clone(**kwargs))
         new_inst.__dict__ = deepcopy(self.__dict__)
         return new_inst
 
     @staticmethod
     def ensure_torch_and_prune_meta(
         im: NdarrayTensor, meta: dict | None, simple_keys: bool = False, pattern: str | None = None, sep: str = "."
     ):
```

### Comparing `monai-weekly-1.2.dev2315/monai/data/samplers.py` & `monai-weekly-1.2.dev2316/monai/data/samplers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/synthetic.py` & `monai-weekly-1.2.dev2316/monai/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/test_time_augmentation.py` & `monai-weekly-1.2.dev2316/monai/data/test_time_augmentation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/thread_buffer.py` & `monai-weekly-1.2.dev2316/monai/data/thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/torchscript_utils.py` & `monai-weekly-1.2.dev2316/monai/data/torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/utils.py` & `monai-weekly-1.2.dev2316/monai/data/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/video_dataset.py` & `monai-weekly-1.2.dev2316/monai/data/video_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/wsi_datasets.py` & `monai-weekly-1.2.dev2316/monai/data/wsi_datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/data/wsi_reader.py` & `monai-weekly-1.2.dev2316/monai/data/wsi_reader.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+import warnings
 from abc import abstractmethod
 from collections.abc import Sequence
 from os.path import abspath
 from typing import Any
 
 import numpy as np
 import torch
@@ -23,37 +24,50 @@
 from monai.data.image_reader import ImageReader, _stack_images
 from monai.data.utils import is_supported_format
 from monai.utils import (
     WSIPatchKeys,
     dtype_numpy_to_torch,
     dtype_torch_to_numpy,
     ensure_tuple,
+    ensure_tuple_rep,
     optional_import,
     require_pkg,
 )
+from monai.utils.misc import ConvertUnits
 
 OpenSlide, _ = optional_import("openslide", name="OpenSlide")
 TiffFile, _ = optional_import("tifffile", name="TiffFile")
 
 __all__ = ["BaseWSIReader", "WSIReader", "CuCIMWSIReader", "OpenSlideWSIReader", "TiffFileWSIReader"]
 
 
 class BaseWSIReader(ImageReader):
     """
     An abstract class that defines APIs to load patches from whole slide image files.
 
     Args:
-        level: the whole slide image level at which the image is extracted.
+        level: the whole slide image level at which the patches are extracted.
+        mpp: the resolution in micron per pixel at which the patches are extracted.
+        mpp_rtol: the acceptable relative tolerance for resolution in micro per pixel.
+        mpp_atol: the acceptable absolute tolerance for resolution in micro per pixel.
+        power: the objective power at which the patches are extracted.
+        power_rtol: the acceptable relative tolerance for objective power.
+        power_atol: the acceptable absolute tolerance for objective power.
         channel_dim: the desired dimension for color channel.
         dtype: the data type of output image.
         device: target device to put the extracted patch. Note that if device is "cuda"",
             the output will be converted to torch tenor and sent to the gpu even if the dtype is numpy.
         mode: the output image color mode, e.g., "RGB" or "RGBA".
         kwargs: additional args for the reader
 
+        Notes:
+            Only one of resolution parameters, `level`, `mpp`, or `power`, should be provided.
+            If such parameters are provided in `get_data` method, those will override the values provided here.
+            If none of them are provided here or in `get_data`, `level=0` will be used.
+
     Typical usage of a concrete implementation of this class is:
 
     .. code-block:: python
 
         image_reader = MyWSIReader()
         wsi = image_reader.read(filepath, **kwargs)
         img_data, meta_data = image_reader.get_data(wsi)
@@ -73,28 +87,40 @@
     """
 
     supported_suffixes: list[str] = []
     backend = ""
 
     def __init__(
         self,
-        level: int,
-        channel_dim: int,
-        dtype: DtypeLike | torch.dtype,
-        device: torch.device | str | None,
-        mode: str,
+        level: int | None = None,
+        mpp: float | tuple[float, float] | None = None,
+        mpp_rtol: float = 0.05,
+        mpp_atol: float = 0.0,
+        power: int | None = None,
+        power_rtol: float = 0.05,
+        power_atol: float = 0.0,
+        channel_dim: int = 0,
+        dtype: DtypeLike | torch.dtype = np.uint8,
+        device: torch.device | str | None = None,
+        mode: str = "RGB",
         **kwargs,
     ):
         super().__init__()
         self.level = level
         self.channel_dim = channel_dim
         self.set_dtype(dtype)
         self.set_device(device)
         self.mode = mode
         self.kwargs = kwargs
+        self.mpp: tuple[float, float] | None = ensure_tuple_rep(mpp, 2) if mpp is not None else None  # type: ignore
+        self.power = power
+        self.mpp_rtol = mpp_rtol
+        self.mpp_atol = mpp_atol
+        self.power_rtol = power_rtol
+        self.power_atol = power_atol
         self.metadata: dict[Any, Any] = {}
 
     def set_dtype(self, dtype):
         self.dtype: torch.dtype | np.dtype
         if isinstance(dtype, torch.dtype):
             self.dtype = dtype
         else:
@@ -103,62 +129,143 @@
     def set_device(self, device):
         if device is None or isinstance(device, (torch.device, str)):
             self.device = device
         else:
             raise ValueError(f"`device` must be `torch.device`, `str` or `None` but {type(device)} is given.")
 
     @abstractmethod
-    def get_size(self, wsi, level: int | None = None) -> tuple[int, int]:
+    def get_size(self, wsi, level: int) -> tuple[int, int]:
         """
         Returns the size (height, width) of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the size is calculated.
 
         """
         raise NotImplementedError(f"Subclass {self.__class__.__name__} must implement this method.")
 
+    def _find_closest_level(
+        self, name: str, value: tuple, value_at_levels: Sequence[tuple], atol: float, rtol: float
+    ) -> int:
+        """Find the level corresponding to the value of the quantity in the list of values at each level.
+        Args:
+            name: the name of the requested quantity
+            value: the value of requested quantity
+            value_at_levels: list of value of the quantity at each level
+            atol: the tolerance for the value
+            rtol: relative tolerance for the value
+        """
+        if value in value_at_levels:
+            return value_at_levels.index(value)
+
+        closest_value = min(value_at_levels, key=lambda a_value: sum([abs(x - y) for x, y in zip(a_value, value)]))  # type: ignore
+        for i in range(len(value)):
+            if abs(closest_value[i] - value[i]) > atol + rtol * abs(value[i]):
+                raise ValueError(
+                    f"The requested {name} < {value} > does not exist in this whole slide image "
+                    f"(with {name}_rtol={rtol} and {name}_atol={atol}). "
+                    f"Here is the list of available {name}: {value_at_levels}. "
+                    f"The closest matching available {name} is {closest_value}."
+                    f"Please consider changing the tolerances or use another {name}."
+                )
+        return value_at_levels.index(closest_value)
+
+    def get_valid_level(
+        self, wsi, level: int | None, mpp: float | tuple[float, float] | None, power: int | None
+    ) -> int:
+        """
+        Returns the level associated to the resolution parameters in the whole slide image.
+
+        Args:
+            wsi: a whole slide image object loaded from a file.
+            level: the level number.
+            mpp: the micron-per-pixel resolution.
+            power: the objective power.
+
+        """
+
+        # Try instance parameters if no resolution is provided
+        if mpp is None and power is None and level is None:
+            mpp = self.mpp
+            power = self.power
+            level = self.level
+
+        # Ensure that at most one resolution parameter is provided.
+        resolution = [val[0] for val in [("level", level), ("mpp", mpp), ("power", power)] if val[1] is not None]
+        if len(resolution) > 1:
+            raise ValueError(f"Only one of `level`, `mpp`, or `power` should be provided. {resolution} are provided.")
+
+        n_levels = self.get_level_count(wsi)
+
+        if mpp is not None:
+            mpp_ = ensure_tuple_rep(mpp, 2)
+            available_mpps = [self.get_mpp(wsi, level) for level in range(n_levels)]
+            level = self._find_closest_level("mpp", mpp_, available_mpps, self.mpp_atol, self.mpp_rtol)
+        elif power is not None:
+            power_ = ensure_tuple(power)
+            available_powers = [(self.get_power(wsi, level),) for level in range(n_levels)]
+            level = self._find_closest_level("power", power_, available_powers, self.power_atol, self.power_rtol)
+        else:
+            if level is None:
+                # Set the default value if no resolution parameter is provided.
+                level = 0
+            if level >= n_levels:
+                raise ValueError(f"The maximum level of this image is {n_levels-1} while level={level} is requested)!")
+
+        return level
+
     @abstractmethod
     def get_level_count(self, wsi) -> int:
         """
         Returns the number of levels in the whole slide image.
 
         Args:
-            wsi: a whole slide image object loaded from a file
+            wsi: a whole slide image object loaded from a file.
 
         """
         raise NotImplementedError(f"Subclass {self.__class__.__name__} must implement this method.")
 
     @abstractmethod
-    def get_downsample_ratio(self, wsi, level: int | None = None) -> float:
+    def get_downsample_ratio(self, wsi, level: int) -> float:
         """
         Returns the down-sampling ratio of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the downsample ratio is calculated.
 
         """
         raise NotImplementedError(f"Subclass {self.__class__.__name__} must implement this method.")
 
     @abstractmethod
     def get_file_path(self, wsi) -> str:
         """Return the file path for the WSI object"""
         raise NotImplementedError(f"Subclass {self.__class__.__name__} must implement this method.")
 
     @abstractmethod
-    def get_mpp(self, wsi, level: int | None = None) -> tuple[float, float]:
+    def get_mpp(self, wsi, level: int) -> tuple[float, float]:
         """
         Returns the micro-per-pixel resolution of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the mpp is calculated.
+
+        """
+        raise NotImplementedError(f"Subclass {self.__class__.__name__} must implement this method.")
+
+    @abstractmethod
+    def get_power(self, wsi, level: int) -> float:
+        """
+        Returns the objective power of the whole slide image at a given level.
+
+        Args:
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the objective power is calculated.
 
         """
         raise NotImplementedError(f"Subclass {self.__class__.__name__} must implement this method.")
 
     @abstractmethod
     def _get_patch(
         self, wsi, location: tuple[int, int], size: tuple[int, int], level: int, dtype: DtypeLike, mode: str
@@ -167,34 +274,34 @@
         Extracts and returns a patch image form the whole slide image.
 
         Args:
             wsi: a whole slide image object loaded from a file or a lis of such objects
             location: (top, left) tuple giving the top left pixel in the level 0 reference frame. Defaults to (0, 0).
             size: (height, width) tuple giving the patch size at the given level (`level`).
                 If None, it is set to the full image size at the given level.
-            level: the level number. Defaults to 0
-            dtype: the data type of output image
-            mode: the output image mode, 'RGB' or 'RGBA'
+            level: the level number.
+            dtype: the data type of output image.
+            mode: the output image mode, 'RGB' or 'RGBA'.
 
         """
         raise NotImplementedError(f"Subclass {self.__class__.__name__} must implement this method.")
 
     def _get_metadata(
         self, wsi, patch: NdarrayOrTensor, location: tuple[int, int], size: tuple[int, int], level: int
     ) -> dict:
         """
         Returns metadata of the extracted patch from the whole slide image.
 
         Args:
-            wsi: the whole slide image object, from which the patch is loaded
-            patch: extracted patch from whole slide image
+            wsi: the whole slide image object, from which the patch is loaded.
+            patch: extracted patch from whole slide image.
             location: (top, left) tuple giving the top left pixel in the level 0 reference frame. Defaults to (0, 0).
             size: (height, width) tuple giving the patch size at the given level (`level`).
                 If None, it is set to the full image size at the given level.
-            level: the level number. Defaults to 0
+            level: the level number.
 
         """
         if self.channel_dim >= len(patch.shape) or self.channel_dim < -len(patch.shape):
             raise ValueError(
                 f"The desired channel_dim ({self.channel_dim}) is out of bound for image shape: {patch.shape}"
             )
         channel_dim: int = self.channel_dim + (len(patch.shape) if self.channel_dim < 0 else 0)
@@ -212,45 +319,52 @@
 
     def get_data(
         self,
         wsi,
         location: tuple[int, int] = (0, 0),
         size: tuple[int, int] | None = None,
         level: int | None = None,
+        mpp: float | tuple[float, float] | None = None,
+        power: int | None = None,
         mode: str | None = None,
     ) -> tuple[np.ndarray, dict]:
         """
-        Verifies inputs, extracts patches from WSI image and generates metadata, and return them.
+        Verifies inputs, extracts patches from WSI image and generates metadata.
 
         Args:
-            wsi: a whole slide image object loaded from a file or a list of such objects
+            wsi: a whole slide image object loaded from a file or a list of such objects.
             location: (top, left) tuple giving the top left pixel in the level 0 reference frame. Defaults to (0, 0).
             size: (height, width) tuple giving the patch size at the given level (`level`).
                 If not provided or None, it is set to the full image size at the given level.
-            level: the level number. Defaults to 0
-            mode: the output image color mode, "RGB" or "RGBA". If not provided the default of "RGB" is used.
+            level: the whole slide image level at which the patches are extracted.
+            mpp: the resolution in micron per pixel at which the patches are extracted.
+            power: the objective power at which the patches are extracted.
+            dtype: the data type of output image.
+            mode: the output image mode, 'RGB' or 'RGBA'.
 
         Returns:
             a tuples, where the first element is an image patch [CxHxW] or stack of patches,
-                and second element is a dictionary of metadata
+                and second element is a dictionary of metadata.
+
+        Notes:
+            Only one of resolution parameters, `level`, `mpp`, or `power`, should be provided.
+            If none of them are provided, it uses the defaults that are set during class instantiation.
+            If none of them are set here or during class instantiation, `level=0` will be used.
         """
         if mode is None:
             mode = self.mode
         patch_list: list = []
         metadata_list: list = []
+
         # CuImage object is iterable, so ensure_tuple won't work on single object
-        if not isinstance(wsi, list):
-            wsi = [wsi]
+        if not isinstance(wsi, (list, tuple)):
+            wsi = (wsi,)
         for each_wsi in ensure_tuple(wsi):
-            # Verify magnification level
-            if level is None:
-                level = self.level
-            max_level = self.get_level_count(each_wsi) - 1
-            if level > max_level:
-                raise ValueError(f"The maximum level of this image is {max_level} while level={level} is requested)!")
+            # get the valid level based on resolution info
+            level = self.get_valid_level(each_wsi, level, mpp, power)
 
             # Verify location
             if location is None:
                 location = (0, 0)
             wsi_size = self.get_size(each_wsi, 0)
             if location[0] > wsi_size[0] or location[1] > wsi_size[1]:
                 raise ValueError(f"Location is outside of the image: location={location}, image size={wsi_size}")
@@ -332,264 +446,339 @@
 
 class WSIReader(BaseWSIReader):
     """
     Read whole slide images and extract patches using different backend libraries
 
     Args:
         backend: the name of backend whole slide image reader library, the default is cuCIM.
-        level: the level at which patches are extracted.
+        level: the whole slide image level at which the patches are extracted.
+        mpp: the resolution in micron per pixel at which the patches are extracted.
+        mpp_rtol: the acceptable relative tolerance for resolution in micro per pixel.
+        mpp_atol: the acceptable absolute tolerance for resolution in micro per pixel.
+        power: the objective power at which the patches are extracted.
+        power_rtol: the acceptable relative tolerance for objective power.
+        power_atol: the acceptable absolute tolerance for objective power.
         channel_dim: the desired dimension for color channel. Default to 0 (channel first).
         dtype: the data type of output image. Defaults to `np.uint8`.
-        mode: the output image color mode, "RGB" or "RGBA". Defaults to "RGB".
         device: target device to put the extracted patch. Note that if device is "cuda"",
             the output will be converted to torch tenor and sent to the gpu even if the dtype is numpy.
+        mode: the output image color mode, "RGB" or "RGBA". Defaults to "RGB".
         num_workers: number of workers for multi-thread image loading (cucim backend only).
         kwargs: additional arguments to be passed to the backend library
 
+        Notes:
+            Only one of resolution parameters, `level`, `mpp`, or `power`, should be provided.
+            If such parameters are provided in `get_data` method, those will override the values provided here.
+            If none of them are provided here or in `get_data`, `level=0` will be used.
+
     """
 
     supported_backends = ["cucim", "openslide", "tifffile"]
 
     def __init__(
         self,
         backend="cucim",
-        level: int = 0,
+        level: int | None = None,
+        mpp: float | tuple[float, float] | None = None,
+        mpp_rtol: float = 0.05,
+        mpp_atol: float = 0.0,
+        power: int | None = None,
+        power_rtol: float = 0.05,
+        power_atol: float = 0.0,
         channel_dim: int = 0,
         dtype: DtypeLike | torch.dtype = np.uint8,
         device: torch.device | str | None = None,
         mode: str = "RGB",
         **kwargs,
     ):
         self.backend = backend.lower()
         self.reader: CuCIMWSIReader | OpenSlideWSIReader | TiffFileWSIReader
         if self.backend == "cucim":
             self.reader = CuCIMWSIReader(
-                level=level, channel_dim=channel_dim, dtype=dtype, device=device, mode=mode, **kwargs
+                level=level,
+                mpp=mpp,
+                mpp_rtol=mpp_rtol,
+                mpp_atol=mpp_atol,
+                power=power,
+                power_rtol=power_rtol,
+                power_atol=power_atol,
+                channel_dim=channel_dim,
+                dtype=dtype,
+                device=device,
+                mode=mode,
+                **kwargs,
             )
         elif self.backend == "openslide":
             self.reader = OpenSlideWSIReader(
-                level=level, channel_dim=channel_dim, dtype=dtype, device=device, mode=mode, **kwargs
+                level=level,
+                mpp=mpp,
+                mpp_rtol=mpp_rtol,
+                mpp_atol=mpp_atol,
+                power=power,
+                power_rtol=power_rtol,
+                power_atol=power_atol,
+                channel_dim=channel_dim,
+                dtype=dtype,
+                device=device,
+                mode=mode,
+                **kwargs,
             )
         elif self.backend == "tifffile":
             self.reader = TiffFileWSIReader(
-                level=level, channel_dim=channel_dim, dtype=dtype, device=device, mode=mode, **kwargs
+                level=level,
+                mpp=mpp,
+                mpp_rtol=mpp_rtol,
+                mpp_atol=mpp_atol,
+                power=power,
+                power_rtol=power_rtol,
+                power_atol=power_atol,
+                channel_dim=channel_dim,
+                dtype=dtype,
+                device=device,
+                mode=mode,
+                **kwargs,
             )
         else:
             raise ValueError(
                 f"The supported backends are cucim, openslide, and tifffile but '{self.backend}' was given."
             )
         self.supported_suffixes = self.reader.supported_suffixes
         self.level = self.reader.level
+        self.mpp_rtol = self.reader.mpp_rtol
+        self.mpp_atol = self.reader.mpp_atol
+        self.power = self.reader.power
+        self.power_rtol = self.reader.power_rtol
+        self.power_atol = self.reader.power_atol
         self.channel_dim = self.reader.channel_dim
         self.dtype = self.reader.dtype
         self.device = self.reader.device
         self.mode = self.reader.mode
         self.kwargs = self.reader.kwargs
         self.metadata = self.reader.metadata
+        self.mpp = self.reader.mpp
 
     def get_level_count(self, wsi) -> int:
         """
         Returns the number of levels in the whole slide image.
 
         Args:
-            wsi: a whole slide image object loaded from a file
+            wsi: a whole slide image object loaded from a file.
 
         """
         return self.reader.get_level_count(wsi)
 
-    def get_size(self, wsi, level: int | None = None) -> tuple[int, int]:
+    def get_size(self, wsi, level: int) -> tuple[int, int]:
         """
         Returns the size (height, width) of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the size is calculated.
 
         """
-        if level is None:
-            level = self.level
-
         return self.reader.get_size(wsi, level)
 
-    def get_downsample_ratio(self, wsi, level: int | None = None) -> float:
+    def get_downsample_ratio(self, wsi, level: int) -> float:
         """
         Returns the down-sampling ratio of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the downsample ratio is calculated.
 
         """
-        if level is None:
-            level = self.level
-
         return self.reader.get_downsample_ratio(wsi, level)
 
     def get_file_path(self, wsi) -> str:
         """Return the file path for the WSI object"""
         return self.reader.get_file_path(wsi)
 
-    def get_mpp(self, wsi, level: int | None = None) -> tuple[float, float]:
+    def get_mpp(self, wsi, level: int) -> tuple[float, float]:
         """
         Returns the micro-per-pixel resolution of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the mpp is calculated.
 
         """
-        if level is None:
-            level = self.level
-
         return self.reader.get_mpp(wsi, level)
 
+    def get_power(self, wsi, level: int) -> float:
+        """
+        Returns the micro-per-pixel resolution of the whole slide image at a given level.
+
+        Args:
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the objective power is calculated.
+
+        """
+        return self.reader.get_power(wsi, level)
+
     def _get_patch(
         self, wsi, location: tuple[int, int], size: tuple[int, int], level: int, dtype: DtypeLike, mode: str
     ) -> np.ndarray:
         """
         Extracts and returns a patch image form the whole slide image.
 
         Args:
-            wsi: a whole slide image object loaded from a file or a lis of such objects
+            wsi: a whole slide image object loaded from a file or a lis of such objects.
             location: (top, left) tuple giving the top left pixel in the level 0 reference frame. Defaults to (0, 0).
             size: (height, width) tuple giving the patch size at the given level (`level`).
                 If None, it is set to the full image size at the given level.
-            level: the level number. Defaults to 0
+            level: the level number.
             dtype: the data type of output image
-            mode: the output image mode, 'RGB' or 'RGBA'
+            mode: the output image mode, 'RGB' or 'RGBA'.
 
         """
         return self.reader._get_patch(wsi=wsi, location=location, size=size, level=level, dtype=dtype, mode=mode)
 
     def read(self, data: Sequence[PathLike] | PathLike | np.ndarray, **kwargs):
         """
         Read whole slide image objects from given file or list of files.
 
         Args:
             data: file name or a list of file names to read.
             kwargs: additional args for the reader module (overrides `self.kwargs` for existing keys).
 
         Returns:
-            whole slide image object or list of such objects
+            whole slide image object or list of such objects.
 
         """
         return self.reader.read(data=data, **kwargs)
 
 
 @require_pkg(pkg_name="cucim")
 class CuCIMWSIReader(BaseWSIReader):
     """
     Read whole slide images and extract patches using cuCIM library.
 
     Args:
-        level: the whole slide image level at which the image is extracted. (default=0)
-            This is overridden if the level argument is provided in `get_data`.
+        level: the whole slide image level at which the patches are extracted.
+        mpp: the resolution in micron per pixel at which the patches are extracted.
+        mpp_rtol: the acceptable relative tolerance for resolution in micro per pixel.
+        mpp_atol: the acceptable absolute tolerance for resolution in micro per pixel.
+        power: the objective power at which the patches are extracted.
+        power_rtol: the acceptable relative tolerance for objective power.
+        power_atol: the acceptable absolute tolerance for objective power.
         channel_dim: the desired dimension for color channel. Default to 0 (channel first).
         dtype: the data type of output image. Defaults to `np.uint8`.
         device: target device to put the extracted patch. Note that if device is "cuda"",
             the output will be converted to torch tenor and sent to the gpu even if the dtype is numpy.
         mode: the output image color mode, "RGB" or "RGBA". Defaults to "RGB".
-        num_workers: number of workers for multi-thread image loading
+        num_workers: number of workers for multi-thread image loading.
         kwargs: additional args for `cucim.CuImage` module:
             https://github.com/rapidsai/cucim/blob/main/cpp/include/cucim/cuimage.h
 
+        Notes:
+            Only one of resolution parameters, `level`, `mpp`, or `power`, should be provided.
+            If such parameters are provided in `get_data` method, those will override the values provided here.
+            If none of them are provided here or in `get_data`, `level=0` will be used.
+
     """
 
     supported_suffixes = ["tif", "tiff", "svs"]
     backend = "cucim"
 
-    def __init__(
-        self,
-        level: int = 0,
-        channel_dim: int = 0,
-        dtype: DtypeLike | torch.dtype = np.uint8,
-        device: torch.device | str | None = None,
-        mode: str = "RGB",
-        num_workers: int = 0,
-        **kwargs,
-    ):
-        super().__init__(level=level, channel_dim=channel_dim, dtype=dtype, device=device, mode=mode, **kwargs)
+    def __init__(self, num_workers: int = 0, **kwargs):
+        super().__init__(**kwargs)
         self.num_workers = num_workers
 
     @staticmethod
     def get_level_count(wsi) -> int:
         """
         Returns the number of levels in the whole slide image.
 
         Args:
-            wsi: a whole slide image object loaded from a file
+            wsi: a whole slide image object loaded from a file.
 
         """
         return wsi.resolutions["level_count"]  # type: ignore
 
-    def get_size(self, wsi, level: int | None = None) -> tuple[int, int]:
+    def get_size(self, wsi, level: int) -> tuple[int, int]:
         """
         Returns the size (height, width) of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the size is calculated.
 
         """
-        if level is None:
-            level = self.level
-
         return (wsi.resolutions["level_dimensions"][level][1], wsi.resolutions["level_dimensions"][level][0])
 
-    def get_downsample_ratio(self, wsi, level: int | None = None) -> float:
+    def get_downsample_ratio(self, wsi, level: int) -> float:
         """
         Returns the down-sampling ratio of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the downsample ratio is calculated.
 
         """
-        if level is None:
-            level = self.level
-
-        return wsi.resolutions["level_downsamples"][level]  # type: ignore
+        return float(wsi.resolutions["level_downsamples"][level])
 
     @staticmethod
     def get_file_path(wsi) -> str:
         """Return the file path for the WSI object"""
         return str(abspath(wsi.path))
 
-    def get_mpp(self, wsi, level: int | None = None) -> tuple[float, float]:
+    def get_mpp(self, wsi, level: int) -> tuple[float, float]:
         """
         Returns the micro-per-pixel resolution of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the mpp is calculated.
 
         """
-        if level is None:
-            level = self.level
+        downsample_ratio = self.get_downsample_ratio(wsi, level)
+
+        if "aperio" in wsi.metadata:
+            mpp_ = wsi.metadata["aperio"].get("MPP")
+            if mpp_:
+                return (downsample_ratio * float(mpp_),) * 2
+        if "cucim" in wsi.metadata:
+            mpp_ = wsi.metadata["cucim"].get("spacing")
+            if mpp_ and isinstance(mpp_, Sequence) and len(mpp_) >= 2:
+                if mpp_[0] and mpp_[1]:
+                    return (downsample_ratio * mpp_[1], downsample_ratio * mpp_[0])
+
+        raise ValueError("`mpp` cannot be obtained for this file. Please use `level` instead.")
+
+    def get_power(self, wsi, level: int) -> float:
+        """
+        Returns the objective power of the whole slide image at a given level.
+
+        Args:
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the objective power is calculated.
 
-        factor = float(wsi.resolutions["level_downsamples"][level])
-        return (wsi.metadata["cucim"]["spacing"][1] * factor, wsi.metadata["cucim"]["spacing"][0] * factor)
+        """
+        if "aperio" in wsi.metadata:
+            objective_power = wsi.metadata["aperio"].get("AppMag")
+            if objective_power:
+                downsample_ratio = self.get_downsample_ratio(wsi, level)
+                return float(objective_power) / downsample_ratio
+
+        raise ValueError(
+            "Currently, cuCIM backend can obtain the objective power only for Aperio images. "
+            "Please use `level` (or `mpp`) instead, or try OpenSlide backend."
+        )
 
     def read(self, data: Sequence[PathLike] | PathLike | np.ndarray, **kwargs):
         """
         Read whole slide image objects from given file or list of files.
 
         Args:
             data: file name or a list of file names to read.
             kwargs: additional args that overrides `self.kwargs` for existing keys.
                 For more details look at https://github.com/rapidsai/cucim/blob/main/cpp/include/cucim/cuimage.h
 
         Returns:
-            whole slide image object or list of such objects
+            whole slide image object or list of such objects.
 
         """
         cuimage_cls, _ = optional_import("cucim", name="CuImage")
         wsi_list: list = []
 
         filenames: Sequence[PathLike] = ensure_tuple(data)
         kwargs_ = self.kwargs.copy()
@@ -603,21 +792,21 @@
     def _get_patch(
         self, wsi, location: tuple[int, int], size: tuple[int, int], level: int, dtype: DtypeLike, mode: str
     ) -> np.ndarray:
         """
         Extracts and returns a patch image form the whole slide image.
 
         Args:
-            wsi: a whole slide image object loaded from a file or a lis of such objects
+            wsi: a whole slide image object loaded from a file or a lis of such objects.
             location: (top, left) tuple giving the top left pixel in the level 0 reference frame. Defaults to (0, 0).
             size: (height, width) tuple giving the patch size at the given level (`level`).
                 If None, it is set to the full image size at the given level.
-            level: the level number. Defaults to 0
-            dtype: the data type of output image
-            mode: the output image mode, 'RGB' or 'RGBA'
+            level: the level number.
+            dtype: the data type of output image.
+            mode: the output image mode, 'RGB' or 'RGBA'.
 
         """
         # Extract a patch or the entire image
         # (reverse the order of location and size to become WxH for cuCIM)
         patch: np.ndarray = wsi.read_region(
             location=location[::-1], size=size[::-1], level=level, num_workers=self.num_workers
         )
@@ -642,122 +831,145 @@
 
 @require_pkg(pkg_name="openslide")
 class OpenSlideWSIReader(BaseWSIReader):
     """
     Read whole slide images and extract patches using OpenSlide library.
 
     Args:
-        level: the whole slide image level at which the image is extracted. (default=0)
-            This is overridden if the level argument is provided in `get_data`.
+        level: the whole slide image level at which the patches are extracted.
+        mpp: the resolution in micron per pixel at which the patches are extracted.
+        mpp_rtol: the acceptable relative tolerance for resolution in micro per pixel.
+        mpp_atol: the acceptable absolute tolerance for resolution in micro per pixel.
+        power: the objective power at which the patches are extracted.
+        power_rtol: the acceptable relative tolerance for objective power.
+        power_atol: the acceptable absolute tolerance for objective power.
         channel_dim: the desired dimension for color channel. Default to 0 (channel first).
         dtype: the data type of output image. Defaults to `np.uint8`.
         device: target device to put the extracted patch. Note that if device is "cuda"",
             the output will be converted to torch tenor and sent to the gpu even if the dtype is numpy.
         mode: the output image color mode, "RGB" or "RGBA". Defaults to "RGB".
         kwargs: additional args for `openslide.OpenSlide` module.
 
+        Notes:
+            Only one of resolution parameters, `level`, `mpp`, or `power`, should be provided.
+            If such parameters are provided in `get_data` method, those will override the values provided here.
+            If none of them are provided here or in `get_data`, `level=0` will be used.
+
     """
 
     supported_suffixes = ["tif", "tiff", "svs"]
     backend = "openslide"
 
-    def __init__(
-        self,
-        level: int = 0,
-        channel_dim: int = 0,
-        dtype: DtypeLike | torch.dtype = np.uint8,
-        device: torch.device | str | None = None,
-        mode: str = "RGB",
-        **kwargs,
-    ):
-        super().__init__(level=level, channel_dim=channel_dim, dtype=dtype, device=device, mode=mode, **kwargs)
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
 
     @staticmethod
     def get_level_count(wsi) -> int:
         """
         Returns the number of levels in the whole slide image.
 
         Args:
-            wsi: a whole slide image object loaded from a file
+            wsi: a whole slide image object loaded from a file.
 
         """
         return wsi.level_count  # type: ignore
 
-    def get_size(self, wsi, level: int | None = None) -> tuple[int, int]:
+    def get_size(self, wsi, level: int) -> tuple[int, int]:
         """
         Returns the size (height, width) of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the size is calculated.
 
         """
-        if level is None:
-            level = self.level
-
         return (wsi.level_dimensions[level][1], wsi.level_dimensions[level][0])
 
-    def get_downsample_ratio(self, wsi, level: int | None = None) -> float:
+    def get_downsample_ratio(self, wsi, level: int) -> float:
         """
         Returns the down-sampling ratio of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the downsample ratio is calculated.
 
         """
-        if level is None:
-            level = self.level
-
         return wsi.level_downsamples[level]  # type: ignore
 
     @staticmethod
     def get_file_path(wsi) -> str:
         """Return the file path for the WSI object"""
         return str(abspath(wsi._filename))
 
-    def get_mpp(self, wsi, level: int | None = None) -> tuple[float, float]:
+    def get_mpp(self, wsi, level: int) -> tuple[float, float]:
         """
         Returns the micro-per-pixel resolution of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the mpp is calculated.
 
         """
-        if level is None:
-            level = self.level
-        unit = wsi.properties["tiff.ResolutionUnit"]
-        if unit == "centimeter":
-            factor = 10000.0
-        elif unit == "millimeter":
-            factor = 1000.0
-        elif unit == "micrometer":
-            factor = 1.0
-        elif unit == "inch":
-            factor = 25400.0
-        else:
-            raise ValueError(f"The resolution unit is not a valid tiff resolution: {unit}")
+        downsample_ratio = self.get_downsample_ratio(wsi, level)
+        if (
+            "openslide.mpp-x" in wsi.properties
+            and "openslide.mpp-y" in wsi.properties
+            and wsi.properties["openslide.mpp-y"]
+            and wsi.properties["openslide.mpp-x"]
+        ):
+            return (
+                downsample_ratio * float(wsi.properties["openslide.mpp-y"]),
+                downsample_ratio * float(wsi.properties["openslide.mpp-x"]),
+            )
+
+        if (
+            "tiff.XResolution" in wsi.properties
+            and "tiff.YResolution" in wsi.properties
+            and wsi.properties["tiff.YResolution"]
+            and wsi.properties["tiff.XResolution"]
+        ):
+            unit = wsi.properties.get("tiff.ResolutionUnit")
+            if unit is None:
+                warnings.warn("The resolution unit is missing, `micrometer` will be used as default.")
+                unit = "micrometer"
+
+            convert_to_micron = ConvertUnits(unit, "micrometer")
+            return (
+                convert_to_micron(downsample_ratio / float(wsi.properties["tiff.YResolution"])),
+                convert_to_micron(downsample_ratio / float(wsi.properties["tiff.XResolution"])),
+            )
 
-        factor *= wsi.level_downsamples[level]
-        return (factor / float(wsi.properties["tiff.YResolution"]), factor / float(wsi.properties["tiff.XResolution"]))
+        raise ValueError("`mpp` cannot be obtained for this file. Please use `level` instead.")
+
+    def get_power(self, wsi, level: int) -> float:
+        """
+        Returns the objective power of the whole slide image at a given level.
+
+        Args:
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the objective power is calculated.
+
+        """
+        objective_power = wsi.properties.get("openslide.objective-power")
+        if objective_power:
+            downsample_ratio = self.get_downsample_ratio(wsi, level)
+            return float(objective_power) / downsample_ratio
+
+        raise ValueError("Objective `power` cannot be obtained for this file. Please use `level` (or `mpp`) instead.")
 
     def read(self, data: Sequence[PathLike] | PathLike | np.ndarray, **kwargs):
         """
         Read whole slide image objects from given file or list of files.
 
         Args:
             data: file name or a list of file names to read.
             kwargs: additional args that overrides `self.kwargs` for existing keys.
 
         Returns:
-            whole slide image object or list of such objects
+            whole slide image object or list of such objects.
 
         """
         wsi_list: list = []
 
         filenames: Sequence[PathLike] = ensure_tuple(data)
         kwargs_ = self.kwargs.copy()
         kwargs_.update(kwargs)
@@ -774,17 +986,17 @@
         Extracts and returns a patch image form the whole slide image.
 
         Args:
             wsi: a whole slide image object loaded from a file or a lis of such objects
             location: (top, left) tuple giving the top left pixel in the level 0 reference frame. Defaults to (0, 0).
             size: (height, width) tuple giving the patch size at the given level (`level`).
                 If None, it is set to the full image size at the given level.
-            level: the level number. Defaults to 0
-            dtype: the data type of output image
-            mode: the output image mode, 'RGB' or 'RGBA'
+            level: the level number.
+            dtype: the data type of output image.
+            mode: the output image mode, 'RGB' or 'RGBA'.
 
         """
         # Extract a patch or the entire image
         # (reverse the order of location and size to become WxH for OpenSlide)
         pil_patch = wsi.read_region(location=location[::-1], size=size[::-1], level=level)
 
         # convert to RGB/RGBA
@@ -801,125 +1013,131 @@
 
 @require_pkg(pkg_name="tifffile")
 class TiffFileWSIReader(BaseWSIReader):
     """
     Read whole slide images and extract patches using TiffFile library.
 
     Args:
-        level: the whole slide image level at which the image is extracted. (default=0)
-            This is overridden if the level argument is provided in `get_data`.
+        level: the whole slide image level at which the patches are extracted.
+        mpp: the resolution in micron per pixel at which the patches are extracted.
+        mpp_rtol: the acceptable relative tolerance for resolution in micro per pixel.
+        mpp_atol: the acceptable absolute tolerance for resolution in micro per pixel.
         channel_dim: the desired dimension for color channel. Default to 0 (channel first).
         dtype: the data type of output image. Defaults to `np.uint8`.
         device: target device to put the extracted patch. Note that if device is "cuda"",
             the output will be converted to torch tenor and sent to the gpu even if the dtype is numpy.
         mode: the output image color mode, "RGB" or "RGBA". Defaults to "RGB".
         kwargs: additional args for `tifffile.TiffFile` module.
 
+        Notes:
+            - Objective power cannot be obtained via TiffFile backend.
+            - Only one of resolution parameters, `level` or `mpp`, should be provided.
+                If such parameters are provided in `get_data` method, those will override the values provided here.
+                If none of them are provided here or in `get_data`, `level=0` will be used.
+
     """
 
     supported_suffixes = ["tif", "tiff", "svs"]
     backend = "tifffile"
 
-    def __init__(
-        self,
-        level: int = 0,
-        channel_dim: int = 0,
-        dtype: DtypeLike | torch.dtype = np.uint8,
-        device: torch.device | str | None = None,
-        mode: str = "RGB",
-        **kwargs,
-    ):
-        super().__init__(level=level, channel_dim=channel_dim, dtype=dtype, device=device, mode=mode, **kwargs)
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
 
     @staticmethod
     def get_level_count(wsi) -> int:
         """
         Returns the number of levels in the whole slide image.
 
         Args:
-            wsi: a whole slide image object loaded from a file
+            wsi: a whole slide image object loaded from a file.
 
         """
         return len(wsi.pages)
 
-    def get_size(self, wsi, level: int | None = None) -> tuple[int, int]:
+    def get_size(self, wsi, level: int) -> tuple[int, int]:
         """
         Returns the size (height, width) of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the size is calculated.
 
         """
-        if level is None:
-            level = self.level
-
         return (wsi.pages[level].imagelength, wsi.pages[level].imagewidth)
 
-    def get_downsample_ratio(self, wsi, level: int | None = None) -> float:
+    def get_downsample_ratio(self, wsi, level: int) -> float:
         """
         Returns the down-sampling ratio of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the downsample ratio is calculated.
 
         """
-        if level is None:
-            level = self.level
-
         return float(wsi.pages[0].imagelength) / float(wsi.pages[level].imagelength)
 
     @staticmethod
     def get_file_path(wsi) -> str:
         """Return the file path for the WSI object"""
         return str(abspath(wsi.filehandle.path))
 
-    def get_mpp(self, wsi, level: int | None = None) -> tuple[float, float]:
+    def get_mpp(self, wsi, level: int) -> tuple[float, float]:
         """
         Returns the micro-per-pixel resolution of the whole slide image at a given level.
 
         Args:
-            wsi: a whole slide image object loaded from a file
-            level: the level number where the size is calculated. If not provided the default level (from `self.level`)
-                will be used.
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the mpp is calculated.
 
         """
-        if level is None:
-            level = self.level
+        if (
+            "XResolution" in wsi.pages[level].tags
+            and "YResolution" in wsi.pages[level].tags
+            and wsi.pages[level].tags["XResolution"].value
+            and wsi.pages[level].tags["YResolution"].value
+        ):
+            unit = wsi.pages[level].tags.get("ResolutionUnit")
+            if unit is not None:
+                unit = str(unit.value)[8:]
+            else:
+                warnings.warn("The resolution unit is missing. `micrometer` will be used as default.")
+                unit = "micrometer"
 
-        unit = wsi.pages[level].tags["ResolutionUnit"].value
-        if unit == unit.CENTIMETER:
-            factor = 10000.0
-        elif unit == unit.MILLIMETER:
-            factor = 1000.0
-        elif unit == unit.MICROMETER:
-            factor = 1.0
-        elif unit == unit.INCH:
-            factor = 25400.0
-        else:
-            raise ValueError(f"The resolution unit is not a valid tiff resolution or missing: {unit.name}")
+            convert_to_micron = ConvertUnits(unit, "micrometer")
+            # Here x and y resolutions are rational numbers so each of them is represented by a tuple.
+            yres = wsi.pages[level].tags["YResolution"].value
+            xres = wsi.pages[level].tags["XResolution"].value
+            return convert_to_micron(yres[1] / yres[0]), convert_to_micron(xres[1] / xres[0])
 
-        # Here x and y resolutions are rational numbers so each of them is represented by a tuple.
-        yres = wsi.pages[level].tags["YResolution"].value
-        xres = wsi.pages[level].tags["XResolution"].value
-        return (factor * yres[1] / yres[0], factor * xres[1] / xres[0])
+        raise ValueError("`mpp`  cannot be obtained for this file. Please use `level` instead.")
+
+    def get_power(self, wsi, level: int) -> float:
+        """
+        Returns the objective power of the whole slide image at a given level.
+
+        Args:
+            wsi: a whole slide image object loaded from a file.
+            level: the level number where the objective power is calculated.
+
+        """
+        raise ValueError(
+            "Currently, TiffFile does not provide a general API to obtain objective power."
+            "Please use `level` (or `mpp`) instead, or try other backends."
+        )
 
     def read(self, data: Sequence[PathLike] | PathLike | np.ndarray, **kwargs):
         """
         Read whole slide image objects from given file or list of files.
 
         Args:
             data: file name or a list of file names to read.
             kwargs: additional args that overrides `self.kwargs` for existing keys.
 
         Returns:
-            whole slide image object or list of such objects
+            whole slide image object or list of such objects.
 
         """
         wsi_list: list = []
 
         filenames: Sequence[PathLike] = ensure_tuple(data)
         kwargs_ = self.kwargs.copy()
         kwargs_.update(kwargs)
@@ -936,17 +1154,17 @@
         Extracts and returns a patch image form the whole slide image.
 
         Args:
             wsi: a whole slide image object loaded from a file or a lis of such objects
             location: (top, left) tuple giving the top left pixel in the level 0 reference frame. Defaults to (0, 0).
             size: (height, width) tuple giving the patch size at the given level (`level`).
                 If None, it is set to the full image size at the given level.
-            level: the level number. Defaults to 0
-            dtype: the data type of output image
-            mode: the output image mode, 'RGB' or 'RGBA'
+            level: the level number.
+            dtype: the data type of output image.
+            mode: the output image mode, 'RGB' or 'RGBA'.
 
         """
         # Load the entire image
         wsi_image: np.ndarray = wsi.asarray(level=level).astype(dtype)
         if len(wsi_image.shape) < 3:
             wsi_image = wsi_image[..., None]
```

### Comparing `monai-weekly-1.2.dev2315/monai/engines/__init__.py` & `monai-weekly-1.2.dev2316/monai/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/engines/evaluator.py` & `monai-weekly-1.2.dev2316/monai/engines/evaluator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/engines/multi_gpu_supervised_trainer.py` & `monai-weekly-1.2.dev2316/monai/engines/multi_gpu_supervised_trainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/engines/trainer.py` & `monai-weekly-1.2.dev2316/monai/engines/trainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/engines/utils.py` & `monai-weekly-1.2.dev2316/monai/engines/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/engines/workflow.py` & `monai-weekly-1.2.dev2316/monai/engines/workflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/fl/__init__.py` & `monai-weekly-1.2.dev2316/monai/fl/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/fl/client/__init__.py` & `monai-weekly-1.2.dev2316/monai/fl/client/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/fl/client/client_algo.py` & `monai-weekly-1.2.dev2316/monai/fl/client/client_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/fl/client/monai_algo.py` & `monai-weekly-1.2.dev2316/monai/fl/client/monai_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/fl/utils/__init__.py` & `monai-weekly-1.2.dev2316/monai/fl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/fl/utils/constants.py` & `monai-weekly-1.2.dev2316/monai/fl/utils/constants.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/fl/utils/exchange_object.py` & `monai-weekly-1.2.dev2316/monai/fl/utils/exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/fl/utils/filters.py` & `monai-weekly-1.2.dev2316/monai/fl/utils/filters.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/__init__.py` & `monai-weekly-1.2.dev2316/monai/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/checkpoint_loader.py` & `monai-weekly-1.2.dev2316/monai/handlers/checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/checkpoint_saver.py` & `monai-weekly-1.2.dev2316/monai/handlers/checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/classification_saver.py` & `monai-weekly-1.2.dev2316/monai/handlers/classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/clearml_handlers.py` & `monai-weekly-1.2.dev2316/monai/handlers/clearml_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/confusion_matrix.py` & `monai-weekly-1.2.dev2316/monai/handlers/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/decollate_batch.py` & `monai-weekly-1.2.dev2316/monai/handlers/decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/earlystop_handler.py` & `monai-weekly-1.2.dev2316/monai/handlers/earlystop_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/garbage_collector.py` & `monai-weekly-1.2.dev2316/monai/handlers/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/hausdorff_distance.py` & `monai-weekly-1.2.dev2316/monai/handlers/hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/ignite_metric.py` & `monai-weekly-1.2.dev2316/monai/handlers/ignite_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/logfile_handler.py` & `monai-weekly-1.2.dev2316/monai/handlers/logfile_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/lr_schedule_handler.py` & `monai-weekly-1.2.dev2316/monai/handlers/lr_schedule_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/mean_dice.py` & `monai-weekly-1.2.dev2316/monai/handlers/mean_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/mean_iou.py` & `monai-weekly-1.2.dev2316/monai/handlers/mean_iou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/metric_logger.py` & `monai-weekly-1.2.dev2316/monai/handlers/metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/metrics_reloaded_handler.py` & `monai-weekly-1.2.dev2316/monai/handlers/metrics_reloaded_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/metrics_saver.py` & `monai-weekly-1.2.dev2316/monai/handlers/metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/mlflow_handler.py` & `monai-weekly-1.2.dev2316/monai/handlers/mlflow_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/nvtx_handlers.py` & `monai-weekly-1.2.dev2316/monai/handlers/nvtx_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/panoptic_quality.py` & `monai-weekly-1.2.dev2316/monai/handlers/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/parameter_scheduler.py` & `monai-weekly-1.2.dev2316/monai/handlers/parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/postprocessing.py` & `monai-weekly-1.2.dev2316/monai/handlers/postprocessing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/probability_maps.py` & `monai-weekly-1.2.dev2316/monai/handlers/probability_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/regression_metrics.py` & `monai-weekly-1.2.dev2316/monai/handlers/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/roc_auc.py` & `monai-weekly-1.2.dev2316/monai/handlers/roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/smartcache_handler.py` & `monai-weekly-1.2.dev2316/monai/handlers/smartcache_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/stats_handler.py` & `monai-weekly-1.2.dev2316/monai/handlers/stats_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/surface_distance.py` & `monai-weekly-1.2.dev2316/monai/handlers/surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/tensorboard_handlers.py` & `monai-weekly-1.2.dev2316/monai/handlers/tensorboard_handlers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/utils.py` & `monai-weekly-1.2.dev2316/monai/handlers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/handlers/validation_handler.py` & `monai-weekly-1.2.dev2316/monai/handlers/validation_handler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/inferers/__init__.py` & `monai-weekly-1.2.dev2316/monai/inferers/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,11 +7,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from .inferer import Inferer, PatchInferer, SaliencyInferer, SimpleInferer, SliceInferer, SlidingWindowInferer
+from .inferer import (
+    Inferer,
+    PatchInferer,
+    SaliencyInferer,
+    SimpleInferer,
+    SliceInferer,
+    SlidingWindowInferer,
+    SlidingWindowInfererAdapt,
+)
 from .merger import AvgMerger, Merger
 from .splitter import SlidingWindowSplitter, Splitter
 from .utils import sliding_window_inference
```

### Comparing `monai-weekly-1.2.dev2315/monai/inferers/inferer.py` & `monai-weekly-1.2.dev2316/monai/inferers/inferer.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,22 +16,33 @@
 from collections.abc import Callable, Iterable, Iterator, Mapping, Sequence
 from pydoc import locate
 from typing import Any
 
 import torch
 import torch.nn as nn
 
+from monai.apps.utils import get_logger
 from monai.data.meta_tensor import MetaTensor
 from monai.inferers.merger import AvgMerger, Merger
 from monai.inferers.splitter import Splitter
 from monai.inferers.utils import compute_importance_map, sliding_window_inference
 from monai.utils import BlendMode, PatchKeys, PytorchPadMode, ensure_tuple, optional_import
 from monai.visualize import CAM, GradCAM, GradCAMpp
 
-__all__ = ["Inferer", "PatchInferer", "SimpleInferer", "SlidingWindowInferer", "SaliencyInferer", "SliceInferer"]
+logger = get_logger(__name__)
+
+__all__ = [
+    "Inferer",
+    "PatchInferer",
+    "SimpleInferer",
+    "SlidingWindowInferer",
+    "SaliencyInferer",
+    "SliceInferer",
+    "SlidingWindowInfererAdapt",
+]
 
 
 class Inferer(ABC):
     """
     A base class for model inference.
     Extend this class to support operations during inference, e.g. a sliding window method.
 
@@ -444,15 +455,17 @@
             network: target model to execute inference.
                 supports callables such as ``lambda x: my_torch_model(x, additional_config)``
             args: optional args to be passed to ``network``.
             kwargs: optional keyword args to be passed to ``network``.
 
         """
 
-        device = self.device
+        device = kwargs.pop("device", self.device)
+        buffer_steps = kwargs.pop("buffer_steps", self.buffer_steps)
+
         if device is None and self.cpu_thresh is not None and inputs.shape[2:].numel() > self.cpu_thresh:
             device = "cpu"  # stitch in cpu memory if image is too large
 
         return sliding_window_inference(
             inputs,
             self.roi_size,
             self.sw_batch_size,
@@ -463,21 +476,104 @@
             self.padding_mode,
             self.cval,
             self.sw_device,
             device,
             self.progress,
             self.roi_weight_map,
             None,
-            self.buffer_steps,
+            buffer_steps,
             self.buffer_dim,
             *args,
             **kwargs,
         )
 
 
+class SlidingWindowInfererAdapt(SlidingWindowInferer):
+    """
+    SlidingWindowInfererAdapt extends SlidingWindowInferer to automatically switch to buffered and then to CPU stitching,
+    when OOM on GPU. It also records a size of such large images to automatically
+    try CPU stitching for the next large image of a similar size.  If the stitching 'device' input parameter is provided,
+    automatic adaptation won't be attempted, please keep the default option device = None for adaptive behavior.
+    Note: the output might be on CPU (even if the input was on GPU), if the GPU memory was not sufficient.
+
+    """
+
+    def __call__(
+        self,
+        inputs: torch.Tensor,
+        network: Callable[..., torch.Tensor | Sequence[torch.Tensor] | dict[Any, torch.Tensor]],
+        *args: Any,
+        **kwargs: Any,
+    ) -> torch.Tensor | tuple[torch.Tensor, ...] | dict[Any, torch.Tensor]:
+        """
+
+        Args:
+            inputs: model input data for inference.
+            network: target model to execute inference.
+                supports callables such as ``lambda x: my_torch_model(x, additional_config)``
+            args: optional args to be passed to ``network``.
+            kwargs: optional keyword args to be passed to ``network``.
+
+        """
+
+        # if device is provided, use without any adaptations
+        if self.device is not None:
+            return super().__call__(inputs, network, *args, **kwargs)
+
+        skip_buffer = self.buffer_steps is not None and self.buffer_steps <= 0
+        cpu_cond = self.cpu_thresh is not None and inputs.shape[2:].numel() > self.cpu_thresh
+        gpu_stitching = inputs.is_cuda and not cpu_cond
+        buffered_stitching = inputs.is_cuda and cpu_cond and not skip_buffer
+        buffer_steps = max(1, self.buffer_steps) if self.buffer_steps is not None else 1
+
+        for _ in range(10):  # at most 10 trials
+            try:
+                return super().__call__(
+                    inputs,
+                    network,
+                    device=inputs.device if gpu_stitching else torch.device("cpu"),
+                    buffer_steps=buffer_steps if buffered_stitching else None,
+                    *args,
+                    **kwargs,
+                )
+            except RuntimeError as e:
+                if not gpu_stitching and not buffered_stitching or "OutOfMemoryError" not in str(type(e).__name__):
+                    raise e
+
+                logger.info(e)
+
+                if gpu_stitching:  # if failed on gpu
+                    gpu_stitching = False
+                    self.cpu_thresh = inputs.shape[2:].numel() - 1  # update thresh
+
+                    if skip_buffer:
+                        buffered_stitching = False
+                        logger.warning(f"GPU stitching failed, attempting on CPU, image dim {inputs.shape}..")
+
+                    else:
+                        buffered_stitching = True
+                        self.buffer_steps = buffer_steps
+                        logger.warning(
+                            f"GPU stitching failed, attempting with buffer {buffer_steps}, image dim {inputs.shape}.."
+                        )
+                elif buffer_steps > 1:
+                    buffer_steps = max(1, buffer_steps // 2)
+                    self.buffer_steps = buffer_steps
+                    logger.warning(
+                        f"GPU buffered stitching failed, image dim {inputs.shape} reducing buffer to {buffer_steps}"
+                    )
+                else:
+                    buffered_stitching = False
+                    self.buffer_steps = 0  # disable future buffer attempts
+                    logger.warning(f"GPU buffered stitching failed, attempting on CPU, image dim {inputs.shape}")
+        raise RuntimeError(  # not possible to finish after the trials
+            f"SlidingWindowInfererAdapt {skip_buffer} {cpu_cond} {gpu_stitching} {buffered_stitching} {buffer_steps}"
+        )
+
+
 class SaliencyInferer(Inferer):
     """
     SaliencyInferer is inference with activation maps.
 
     Args:
         cam_name: expected CAM method name, should be: "CAM", "GradCAM" or "GradCAMpp".
         target_layers: name of the model layer to generate the feature map.
```

### Comparing `monai-weekly-1.2.dev2315/monai/inferers/merger.py` & `monai-weekly-1.2.dev2316/monai/inferers/merger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/inferers/splitter.py` & `monai-weekly-1.2.dev2316/monai/inferers/splitter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/inferers/utils.py` & `monai-weekly-1.2.dev2316/monai/inferers/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 tqdm, _ = optional_import("tqdm", name="tqdm")
 _nearest_mode = "nearest-exact" if pytorch_after(1, 11) else "nearest"
 
 __all__ = ["sliding_window_inference"]
 
 
 def sliding_window_inference(
-    inputs: torch.Tensor,
+    inputs: torch.Tensor | MetaTensor,
     roi_size: Sequence[int] | int,
     sw_batch_size: int,
     predictor: Callable[..., torch.Tensor | Sequence[torch.Tensor] | dict[Any, torch.Tensor]],
     overlap: Sequence[float] | float = 0.25,
     mode: BlendMode | str = BlendMode.CONSTANT,
     sigma_scale: Sequence[float] | float = 0.125,
     padding_mode: PytorchPadMode | str = PytorchPadMode.CONSTANT,
@@ -303,30 +303,32 @@
                     int(round(pad_size[sp * 2] * zoom_scale[si])),
                     int(round((pad_size[sp * 2] + image_size_[si]) * zoom_scale[si])),
                 )
                 final_slicing.insert(0, slice_dim)
             output_image_list[ss] = output_i[(slice(None), slice(None), *final_slicing)]
 
     final_output = _pack_struct(output_image_list, dict_keys)
-    final_output = convert_to_dst_type(final_output, inputs, device=device)[0]  # type: ignore
     if temp_meta is not None:
-        final_output = MetaTensor(final_output).copy_meta_from(temp_meta)
+        final_output = convert_to_dst_type(final_output, temp_meta, device=device)[0]
+    else:
+        final_output = convert_to_dst_type(final_output, inputs, device=device)[0]
+
     return final_output  # type: ignore
 
 
 def _create_buffered_slices(slices, batch_size, sw_batch_size, buffer_dim, buffer_steps):
     """rearrange slices for buffering"""
     slices_np = np.asarray(slices)
     slices_np = slices_np[np.argsort(slices_np[:, buffer_dim, 0], kind="mergesort")]
     slices = [tuple(slice(c[0], c[1]) for c in i) for i in slices_np]
     slices_np = slices_np[:, buffer_dim]
 
     _, _, _b_lens = np.unique(slices_np[:, 0], return_counts=True, return_index=True)
     b_ends = np.cumsum(_b_lens).tolist()  # possible buffer flush boundaries
-    x = [0, *b_ends][:: min(len(b_ends), int(buffer_steps))]  # type: ignore
+    x = [0, *b_ends][:: min(len(b_ends), int(buffer_steps))]
     if x[-1] < b_ends[-1]:
         x.append(b_ends[-1])
     n_per_batch = len(x) - 1
     windows_range = [
         range(b * x[-1] + x[i], b * x[-1] + x[i + 1], sw_batch_size)
         for b in range(batch_size)
         for i in range(n_per_batch)
@@ -381,15 +383,15 @@
     seg_probs: tuple[torch.Tensor, ...]
     if isinstance(seg_out, torch.Tensor):
         seg_probs = (seg_out,)
     elif isinstance(seg_out, Mapping):
         dict_keys = sorted(seg_out.keys())  # track predictor's output keys
         seg_probs = tuple(seg_out[k] for k in dict_keys)
     else:
-        seg_probs = ensure_tuple(seg_out)  # type: ignore
+        seg_probs = ensure_tuple(seg_out)
     return dict_keys, seg_probs
 
 
 def _pack_struct(seg_out, dict_keys=None):
     if dict_keys is not None:
         return dict(zip(dict_keys, seg_out))
     if isinstance(seg_out, (list, tuple)) and len(seg_out) == 1:
```

### Comparing `monai-weekly-1.2.dev2315/monai/losses/__init__.py` & `monai-weekly-1.2.dev2316/monai/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/losses/contrastive.py` & `monai-weekly-1.2.dev2316/monai/losses/contrastive.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/losses/deform.py` & `monai-weekly-1.2.dev2316/monai/losses/deform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/losses/dice.py` & `monai-weekly-1.2.dev2316/monai/losses/dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/losses/ds_loss.py` & `monai-weekly-1.2.dev2316/monai/losses/ds_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/losses/focal_loss.py` & `monai-weekly-1.2.dev2316/monai/losses/focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/losses/giou_loss.py` & `monai-weekly-1.2.dev2316/monai/losses/giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/losses/image_dissimilarity.py` & `monai-weekly-1.2.dev2316/monai/losses/image_dissimilarity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/losses/multi_scale.py` & `monai-weekly-1.2.dev2316/monai/losses/multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/losses/spatial_mask.py` & `monai-weekly-1.2.dev2316/monai/losses/spatial_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/losses/ssim_loss.py` & `monai-weekly-1.2.dev2316/monai/losses/ssim_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/losses/tversky.py` & `monai-weekly-1.2.dev2316/monai/losses/tversky.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/losses/unified_focal_loss.py` & `monai-weekly-1.2.dev2316/monai/losses/unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/metrics/__init__.py` & `monai-weekly-1.2.dev2316/monai/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/metrics/active_learning_metrics.py` & `monai-weekly-1.2.dev2316/monai/metrics/active_learning_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/metrics/confusion_matrix.py` & `monai-weekly-1.2.dev2316/monai/metrics/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/metrics/cumulative_average.py` & `monai-weekly-1.2.dev2316/monai/metrics/cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/metrics/f_beta_score.py` & `monai-weekly-1.2.dev2316/monai/metrics/f_beta_score.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/metrics/froc.py` & `monai-weekly-1.2.dev2316/monai/metrics/froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/metrics/generalized_dice.py` & `monai-weekly-1.2.dev2316/monai/metrics/generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/metrics/hausdorff_distance.py` & `monai-weekly-1.2.dev2316/monai/metrics/hausdorff_distance.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,19 +8,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import warnings
+from collections.abc import Sequence
+from typing import Any
 
 import numpy as np
 import torch
 
-from monai.metrics.utils import do_metric_reduction, get_mask_edges, get_surface_distance, ignore_background
+from monai.metrics.utils import (
+    do_metric_reduction,
+    get_mask_edges,
+    get_surface_distance,
+    ignore_background,
+    prepare_spacing,
+)
 from monai.utils import MetricReduction, convert_data_type
 
 from .metric import CumulativeIterationMetric
 
 __all__ = ["HausdorffDistanceMetric", "compute_hausdorff_distance", "compute_percent_hausdorff_distance"]
 
 
@@ -66,37 +74,49 @@
         self.include_background = include_background
         self.distance_metric = distance_metric
         self.percentile = percentile
         self.directed = directed
         self.reduction = reduction
         self.get_not_nans = get_not_nans
 
-    def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor) -> torch.Tensor:  # type: ignore[override]
+    def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor, **kwargs: Any) -> torch.Tensor:  # type: ignore[override]
         """
         Args:
             y_pred: input data to compute, typical segmentation model output.
                 It must be one-hot format and first dim is batch, example shape: [16, 3, 32, 32]. The values
                 should be binarized.
             y: ground truth to compute the distance. It must be one-hot format and first dim is batch.
                 The values should be binarized.
+            kwargs: additional parameters, e.g. ``spacing`` should be passed to correctly compute the metric.
+                ``spacing``: spacing of pixel (or voxel). This parameter is relevant only
+                if ``distance_metric`` is set to ``"euclidean"``.
+                If a single number, isotropic spacing with that value is used for all images in the batch. If a sequence of numbers,
+                the length of the sequence must be equal to the image dimensions.
+                This spacing will be used for all images in the batch.
+                If a sequence of sequences, the length of the outer sequence must be equal to the batch size.
+                If inner sequence has length 1, isotropic spacing with that value is used for all images in the batch,
+                else the inner sequence length must be equal to the image dimensions. If ``None``, spacing of unity is used
+                for all images in batch. Defaults to ``None``.
 
         Raises:
             ValueError: when `y_pred` has less than three dimensions.
         """
         dims = y_pred.ndimension()
         if dims < 3:
             raise ValueError("y_pred should have at least three dimensions.")
+
         # compute (BxC) for each channel for each batch
         return compute_hausdorff_distance(
             y_pred=y_pred,
             y=y,
             include_background=self.include_background,
             distance_metric=self.distance_metric,
             percentile=self.percentile,
             directed=self.directed,
+            spacing=kwargs.get("spacing"),
         )
 
     def aggregate(
         self, reduction: MetricReduction | str | None = None
     ) -> torch.Tensor | tuple[torch.Tensor, torch.Tensor]:
         """
         Execute reduction logic for the output of `compute_hausdorff_distance`.
@@ -119,14 +139,15 @@
 def compute_hausdorff_distance(
     y_pred: np.ndarray | torch.Tensor,
     y: np.ndarray | torch.Tensor,
     include_background: bool = False,
     distance_metric: str = "euclidean",
     percentile: float | None = None,
     directed: bool = False,
+    spacing: int | float | np.ndarray | Sequence[int | float | np.ndarray | Sequence[int | float]] | None = None,
 ) -> torch.Tensor:
     """
     Compute the Hausdorff distance.
 
     Args:
         y_pred: input data to compute, typical segmentation model output.
             It must be one-hot format and first dim is batch, example shape: [16, 3, 32, 32]. The values
@@ -137,50 +158,69 @@
             the predicted output. Defaults to ``False``.
         distance_metric: : [``"euclidean"``, ``"chessboard"``, ``"taxicab"``]
             the metric used to compute surface distance. Defaults to ``"euclidean"``.
         percentile: an optional float number between 0 and 100. If specified, the corresponding
             percentile of the Hausdorff Distance rather than the maximum result will be achieved.
             Defaults to ``None``.
         directed: whether to calculate directed Hausdorff distance. Defaults to ``False``.
+        spacing: spacing of pixel (or voxel). This parameter is relevant only if ``distance_metric`` is set to ``"euclidean"``.
+            If a single number, isotropic spacing with that value is used for all images in the batch. If a sequence of numbers,
+            the length of the sequence must be equal to the image dimensions. This spacing will be used for all images in the batch.
+            If a sequence of sequences, the length of the outer sequence must be equal to the batch size.
+            If inner sequence has length 1, isotropic spacing with that value is used for all images in the batch,
+            else the inner sequence length must be equal to the image dimensions. If ``None``, spacing of unity is used
+            for all images in batch. Defaults to ``None``.
     """
 
     if not include_background:
         y_pred, y = ignore_background(y_pred=y_pred, y=y)
     y_pred = convert_data_type(y_pred, output_type=torch.Tensor, dtype=torch.float)[0]
     y = convert_data_type(y, output_type=torch.Tensor, dtype=torch.float)[0]
 
     if y.shape != y_pred.shape:
         raise ValueError(f"y_pred and y should have same shapes, got {y_pred.shape} and {y.shape}.")
 
     batch_size, n_class = y_pred.shape[:2]
     hd = np.empty((batch_size, n_class))
+
+    img_dim = y_pred.ndim - 2
+    spacing_list = prepare_spacing(spacing=spacing, batch_size=batch_size, img_dim=img_dim)
+
     for b, c in np.ndindex(batch_size, n_class):
         (edges_pred, edges_gt) = get_mask_edges(y_pred[b, c], y[b, c])
         if not np.any(edges_gt):
             warnings.warn(f"the ground truth of class {c} is all 0, this may result in nan/inf distance.")
         if not np.any(edges_pred):
             warnings.warn(f"the prediction of class {c} is all 0, this may result in nan/inf distance.")
 
-        distance_1 = compute_percent_hausdorff_distance(edges_pred, edges_gt, distance_metric, percentile)
+        distance_1 = compute_percent_hausdorff_distance(
+            edges_pred, edges_gt, distance_metric, percentile, spacing_list[b]
+        )
         if directed:
             hd[b, c] = distance_1
         else:
-            distance_2 = compute_percent_hausdorff_distance(edges_gt, edges_pred, distance_metric, percentile)
+            distance_2 = compute_percent_hausdorff_distance(
+                edges_gt, edges_pred, distance_metric, percentile, spacing_list[b]
+            )
             hd[b, c] = max(distance_1, distance_2)
     return convert_data_type(hd, output_type=torch.Tensor, device=y_pred.device, dtype=torch.float)[0]
 
 
 def compute_percent_hausdorff_distance(
-    edges_pred: np.ndarray, edges_gt: np.ndarray, distance_metric: str = "euclidean", percentile: float | None = None
+    edges_pred: np.ndarray,
+    edges_gt: np.ndarray,
+    distance_metric: str = "euclidean",
+    percentile: float | None = None,
+    spacing: int | float | np.ndarray | Sequence[int | float] | None = None,
 ) -> float:
     """
     This function is used to compute the directed Hausdorff distance.
     """
 
-    surface_distance = get_surface_distance(edges_pred, edges_gt, distance_metric=distance_metric)
+    surface_distance = get_surface_distance(edges_pred, edges_gt, distance_metric=distance_metric, spacing=spacing)
 
     # for both pred and gt do not have foreground
     if surface_distance.shape == (0,):
         return np.nan
 
     if not percentile:
         return surface_distance.max()  # type: ignore[no-any-return]
```

### Comparing `monai-weekly-1.2.dev2315/monai/metrics/loss_metric.py` & `monai-weekly-1.2.dev2316/monai/metrics/loss_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from typing import Any
+
 import torch
 from torch.nn.modules.loss import _Loss
 
 from monai.metrics.utils import do_metric_reduction
 from monai.utils import MetricReduction
 
 from ..config import TensorOrList
@@ -88,15 +90,15 @@
         """
         data = self.get_buffer()
         if data is None:
             return (torch.tensor(0.0), torch.tensor(0.0)) if self.get_not_nans else torch.tensor(0.0)
         f, not_nans = do_metric_reduction(data, reduction or self.reduction)
         return (f, not_nans) if self.get_not_nans else f
 
-    def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor | None = None) -> TensorOrList:
+    def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor | None = None, **kwargs: Any) -> TensorOrList:
         """
         Input `y_pred` is compared with ground truth `y`.
         Both `y_pred` and `y` are expected to be a batch-first Tensor (BC[HWD]).
 
         Returns:
              a tensor with shape (BC[HWD]), or a list of tensors, each tensor with shape (C[HWD]).
         """
```

### Comparing `monai-weekly-1.2.dev2315/monai/metrics/meandice.py` & `monai-weekly-1.2.dev2316/monai/metrics/meandice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/metrics/meaniou.py` & `monai-weekly-1.2.dev2316/monai/metrics/meaniou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/metrics/metric.py` & `monai-weekly-1.2.dev2316/monai/metrics/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,43 +45,44 @@
 
     `__call__` is designed to handle `y_pred` and `y` (optional) in torch tensors or a list/tuple of tensors.
 
     Subclasses typically implement the `_compute_tensor` function for the actual tensor computation logic.
     """
 
     def __call__(
-        self, y_pred: TensorOrList, y: TensorOrList | None = None
+        self, y_pred: TensorOrList, y: TensorOrList | None = None, **kwargs: Any
     ) -> torch.Tensor | Sequence[torch.Tensor | Sequence[torch.Tensor]]:
         """
         Execute basic computation for model prediction `y_pred` and ground truth `y` (optional).
         It supports inputs of a list of "channel-first" Tensor and a "batch-first" Tensor.
 
         Args:
             y_pred: the raw model prediction data at one iteration, must be a list of `channel-first` Tensor
                 or a `batch-first` Tensor.
             y: the ground truth to compute, must be a list of `channel-first` Tensor
                 or a `batch-first` Tensor.
+            kwargs: additional parameters for specific metric computation logic (e.g. ``spacing`` for SurfaceDistanceMetric, etc.).
 
         Returns:
             The computed metric values at the iteration level.
             The output shape could be a `batch-first` tensor or a list of `batch-first` tensors.
             When it's a list of tensors, each item in the list can represent a specific type of metric.
 
         """
         # handling a list of channel-first data
         if isinstance(y_pred, (list, tuple)) or isinstance(y, (list, tuple)):
-            return self._compute_list(y_pred, y)
+            return self._compute_list(y_pred, y, **kwargs)
         # handling a single batch-first data
         if isinstance(y_pred, torch.Tensor):
             y_ = y.detach() if isinstance(y, torch.Tensor) else None
-            return self._compute_tensor(y_pred.detach(), y_)
+            return self._compute_tensor(y_pred.detach(), y_, **kwargs)
         raise ValueError("y_pred or y must be a list/tuple of `channel-first` Tensors or a `batch-first` Tensor.")
 
     def _compute_list(
-        self, y_pred: TensorOrList, y: TensorOrList | None = None
+        self, y_pred: TensorOrList, y: TensorOrList | None = None, **kwargs: Any
     ) -> torch.Tensor | list[torch.Tensor | Sequence[torch.Tensor]]:
         """
         Execute the metric computation for `y_pred` and `y` in a list of "channel-first" tensors.
 
         The return value is a "batch-first" tensor, or a list of "batch-first" tensors.
         When it's a list of tensors, each item in the list can represent a specific type of metric values.
 
@@ -89,28 +90,31 @@
         where each item is a tuple of three values `tp`, `fp`, `fn` for true positives, false positives,
         and false negatives respectively. This function will return a list of three items,
         (`tp_batched`, `fp_batched`, `fn_batched`), where each item is a `batch_size`-length tensor.
 
         Note: subclass may enhance the operation to have multi-thread support.
         """
         if y is not None:
-            ret = [self._compute_tensor(p.detach().unsqueeze(0), y_.detach().unsqueeze(0)) for p, y_ in zip(y_pred, y)]
+            ret = [
+                self._compute_tensor(p.detach().unsqueeze(0), y_.detach().unsqueeze(0), **kwargs)
+                for p, y_ in zip(y_pred, y)
+            ]
         else:
-            ret = [self._compute_tensor(p_.detach().unsqueeze(0), None) for p_ in y_pred]
+            ret = [self._compute_tensor(p_.detach().unsqueeze(0), None, **kwargs) for p_ in y_pred]
 
         # concat the list of results (e.g. a batch of evaluation scores)
         if isinstance(ret[0], torch.Tensor):
             return torch.cat(ret, dim=0)  # type: ignore[arg-type]
         # the result is a list of sequence of tensors (e.g. a batch of multi-class results)
         if isinstance(ret[0], (list, tuple)) and all(isinstance(i, torch.Tensor) for i in ret[0]):
             return [torch.cat(batch_i, dim=0) for batch_i in zip(*ret)]
         return ret
 
     @abstractmethod
-    def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor | None = None) -> TensorOrList:
+    def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor | None = None, **kwargs: Any) -> TensorOrList:
         """
         Computation logic for `y_pred` and `y` of an iteration, the data should be "batch-first" Tensors.
         A subclass should implement its own computation logic.
         The return value is usually a "batch_first" tensor, or a list of "batch_first" tensors.
         """
         raise NotImplementedError(f"Subclass {self.__class__.__name__} must implement this method.")
 
@@ -314,32 +318,33 @@
 
     And to load `predictions` and `labels` from files, then compute metrics with multi-processing, please refer to:
     https://github.com/Project-MONAI/tutorials/blob/master/modules/compute_metric.py.
 
     """
 
     def __call__(
-        self, y_pred: TensorOrList, y: TensorOrList | None = None
+        self, y_pred: TensorOrList, y: TensorOrList | None = None, **kwargs: Any
     ) -> torch.Tensor | Sequence[torch.Tensor | Sequence[torch.Tensor]]:
         """
         Execute basic computation for model prediction and ground truth.
         It can support  both `list of channel-first Tensor` and `batch-first Tensor`.
         Users call this API to execute computation on every batch of data, then accumulate the results,
         or accumulate the original `y_pred` and `y`, then execute on the accumulated data.
 
         Args:
             y_pred: the model prediction data to compute, must be a list of `channel-first` Tensor
                 or a `batch-first` Tensor.
             y: the ground truth to compute, must be a list of `channel-first` Tensor
                 or a `batch-first` Tensor.
+            kwargs: additional parameters for specific metric computation logic (e.g. ``spacing`` for SurfaceDistanceMetric, etc.).
 
         Returns:
             The computed metric values at the iteration level. The output shape should be
             a `batch-first` tensor (BC[HWD]) or a list of `batch-first` tensors.
         """
-        ret = super().__call__(y_pred=y_pred, y=y)
+        ret = super().__call__(y_pred=y_pred, y=y, **kwargs)
         if isinstance(ret, (tuple, list)):
             self.extend(*ret)
         else:
             self.extend(ret)
 
         return ret
```

### Comparing `monai-weekly-1.2.dev2315/monai/metrics/panoptic_quality.py` & `monai-weekly-1.2.dev2316/monai/metrics/panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/metrics/regression.py` & `monai-weekly-1.2.dev2316/monai/metrics/regression.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/metrics/rocauc.py` & `monai-weekly-1.2.dev2316/monai/metrics/rocauc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/metrics/surface_dice.py` & `monai-weekly-1.2.dev2316/monai/metrics/surface_dice.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,19 +8,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import warnings
+from collections.abc import Sequence
+from typing import Any
 
 import numpy as np
 import torch
 
-from monai.metrics.utils import do_metric_reduction, get_mask_edges, get_surface_distance, ignore_background
+from monai.metrics.utils import (
+    do_metric_reduction,
+    get_mask_edges,
+    get_surface_distance,
+    ignore_background,
+    prepare_spacing,
+)
 from monai.utils import MetricReduction, convert_data_type
 
 from .metric import CumulativeIterationMetric
 
 
 class SurfaceDiceMetric(CumulativeIterationMetric):
     """
@@ -63,32 +71,43 @@
         super().__init__()
         self.class_thresholds = class_thresholds
         self.include_background = include_background
         self.distance_metric = distance_metric
         self.reduction = reduction
         self.get_not_nans = get_not_nans
 
-    def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor) -> torch.Tensor:  # type: ignore[override]
+    def _compute_tensor(self, y_pred: torch.Tensor, y: torch.Tensor, **kwargs: Any) -> torch.Tensor:  # type: ignore[override]
         r"""
         Args:
             y_pred: Predicted segmentation, typically segmentation model output.
                 It must be a one-hot encoded, batch-first tensor [B,C,H,W].
             y: Reference segmentation.
                 It must be a one-hot encoded, batch-first tensor [B,C,H,W].
+            kwargs: additional parameters, e.g. ``spacing`` should be passed to correctly compute the metric.
+                ``spacing``: spacing of pixel (or voxel). This parameter is relevant only
+                if ``distance_metric`` is set to ``"euclidean"``.
+                If a single number, isotropic spacing with that value is used for all images in the batch. If a sequence of numbers,
+                the length of the sequence must be equal to the image dimensions.
+                This spacing will be used for all images in the batch.
+                If a sequence of sequences, the length of the outer sequence must be equal to the batch size.
+                If inner sequence has length 1, isotropic spacing with that value is used for all images in the batch,
+                else the inner sequence length must be equal to the image dimensions. If ``None``, spacing of unity is used
+                for all images in batch. Defaults to ``None``.
 
         Returns:
             Pytorch Tensor of shape [B,C], containing the NSD values :math:`\operatorname {NSD}_{b,c}` for each batch
             index :math:`b` and class :math:`c`.
         """
         return compute_surface_dice(
             y_pred=y_pred,
             y=y,
             class_thresholds=self.class_thresholds,
             include_background=self.include_background,
             distance_metric=self.distance_metric,
+            spacing=kwargs.get("spacing"),
         )
 
     def aggregate(
         self, reduction: MetricReduction | str | None = None
     ) -> torch.Tensor | tuple[torch.Tensor, torch.Tensor]:
         r"""
         Aggregates the output of `_compute_tensor`.
@@ -113,14 +132,15 @@
 
 def compute_surface_dice(
     y_pred: torch.Tensor,
     y: torch.Tensor,
     class_thresholds: list[float],
     include_background: bool = False,
     distance_metric: str = "euclidean",
+    spacing: int | float | np.ndarray | Sequence[int | float | np.ndarray | Sequence[int | float]] | None = None,
 ) -> torch.Tensor:
     r"""
     This function computes the (Normalized) Surface Dice (NSD) between the two tensors `y_pred` (referred to as
     :math:`\hat{Y}`) and `y` (referred to as :math:`Y`). This metric determines which fraction of a segmentation
     boundary is correctly predicted. A boundary element is considered correctly predicted if the closest distance to the
     reference boundary is smaller than or equal to the specified threshold related to the acceptable amount of deviation in
     pixels. The NSD is bounded between 0 and 1.
@@ -163,14 +183,21 @@
             The thresholds relate to the acceptable amount of deviation in the segmentation boundary in pixels.
             Each threshold needs to be a finite, non-negative number.
         include_background: Whether to skip the surface dice computation on the first channel of
             the predicted output. Defaults to ``False``.
         distance_metric: The metric used to compute surface distances.
             One of [``"euclidean"``, ``"chessboard"``, ``"taxicab"``].
             Defaults to ``"euclidean"``.
+        spacing: spacing of pixel (or voxel). This parameter is relevant only if ``distance_metric`` is set to ``"euclidean"``.
+            If a single number, isotropic spacing with that value is used for all images in the batch. If a sequence of numbers,
+            the length of the sequence must be equal to the image dimensions. This spacing will be used for all images in the batch.
+            If a sequence of sequences, the length of the outer sequence must be equal to the batch size.
+            If inner sequence has length 1, isotropic spacing with that value is used for all images in the batch,
+            else the inner sequence length must be equal to the image dimensions. If ``None``, spacing of unity is used
+            for all images in batch. Defaults to ``None``.
 
     Raises:
         ValueError: If `y_pred` and/or `y` are not PyTorch tensors.
         ValueError: If `y_pred` and/or `y` do not have four dimensions.
         ValueError: If `y_pred` and/or `y` have different shapes.
         ValueError: If `y_pred` and/or `y` are not one-hot encoded
         ValueError: If the number of channels of `y_pred` and/or `y` is different from the number of class thresholds.
@@ -215,23 +242,30 @@
         raise ValueError("All class thresholds need to be finite.")
 
     if any(np.array(class_thresholds) < 0):
         raise ValueError("All class thresholds need to be >= 0.")
 
     nsd = np.empty((batch_size, n_class))
 
+    img_dim = y_pred.ndim - 2
+    spacing_list = prepare_spacing(spacing=spacing, batch_size=batch_size, img_dim=img_dim)
+
     for b, c in np.ndindex(batch_size, n_class):
         (edges_pred, edges_gt) = get_mask_edges(y_pred[b, c], y[b, c], crop=False)
         if not np.any(edges_gt):
             warnings.warn(f"the ground truth of class {c} is all 0, this may result in nan/inf distance.")
         if not np.any(edges_pred):
             warnings.warn(f"the prediction of class {c} is all 0, this may result in nan/inf distance.")
 
-        distances_pred_gt = get_surface_distance(edges_pred, edges_gt, distance_metric=distance_metric)
-        distances_gt_pred = get_surface_distance(edges_gt, edges_pred, distance_metric=distance_metric)
+        distances_pred_gt = get_surface_distance(
+            edges_pred, edges_gt, distance_metric=distance_metric, spacing=spacing_list[b]
+        )
+        distances_gt_pred = get_surface_distance(
+            edges_gt, edges_pred, distance_metric=distance_metric, spacing=spacing_list[b]
+        )
 
         boundary_complete = len(distances_pred_gt) + len(distances_gt_pred)
         boundary_correct = np.sum(distances_pred_gt <= class_thresholds[c]) + np.sum(
             distances_gt_pred <= class_thresholds[c]
         )
 
         if boundary_complete == 0:
```

### Comparing `monai-weekly-1.2.dev2315/monai/metrics/utils.py` & `monai-weekly-1.2.dev2316/monai/metrics/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 import warnings
+from collections.abc import Sequence
 from typing import Any
 
 import numpy as np
 import torch
 
 from monai.config import NdarrayOrTensor, NdarrayTensor
 from monai.transforms.croppad.array import SpatialCrop
@@ -168,41 +169,53 @@
     # Do binary erosion and use XOR to get edges
     edges_pred = binary_erosion(seg_pred) ^ seg_pred
     edges_gt = binary_erosion(seg_gt) ^ seg_gt
 
     return edges_pred, edges_gt
 
 
-def get_surface_distance(seg_pred: np.ndarray, seg_gt: np.ndarray, distance_metric: str = "euclidean") -> np.ndarray:
+def get_surface_distance(
+    seg_pred: np.ndarray,
+    seg_gt: np.ndarray,
+    distance_metric: str = "euclidean",
+    spacing: int | float | np.ndarray | Sequence[int | float] | None = None,
+) -> np.ndarray:
     """
     This function is used to compute the surface distances from `seg_pred` to `seg_gt`.
 
     Args:
         seg_pred: the edge of the predictions.
         seg_gt: the edge of the ground truth.
         distance_metric: : [``"euclidean"``, ``"chessboard"``, ``"taxicab"``]
             the metric used to compute surface distance. Defaults to ``"euclidean"``.
 
             - ``"euclidean"``, uses Exact Euclidean distance transform.
             - ``"chessboard"``, uses `chessboard` metric in chamfer type of transform.
             - ``"taxicab"``, uses `taxicab` metric in chamfer type of transform.
+        spacing: spacing of pixel (or voxel) along each axis. If a sequence, must be of
+            length equal to the image dimensions; if a single number, this is used for all axes.
+            If ``None``, spacing of unity is used. Defaults to ``None``.
+        spacing: spacing of pixel (or voxel). This parameter is relevant only if ``distance_metric`` is set to ``"euclidean"``.
+            Several input options are allowed: (1) If a single number, isotropic spacing with that value is used.
+            (2) If a sequence of numbers, the length of the sequence must be equal to the image dimensions.
+            (3) If ``None``, spacing of unity is used. Defaults to ``None``.
 
     Note:
         If seg_pred or seg_gt is all 0, may result in nan/inf distance.
 
     """
 
     if not np.any(seg_gt):
         dis = np.inf * np.ones_like(seg_gt)
     else:
         if not np.any(seg_pred):
             dis = np.inf * np.ones_like(seg_gt)
             return np.asarray(dis[seg_gt])
         if distance_metric == "euclidean":
-            dis = distance_transform_edt(~seg_gt)
+            dis = distance_transform_edt(~seg_gt, sampling=spacing)
         elif distance_metric in {"chessboard", "taxicab"}:
             dis = distance_transform_cdt(~seg_gt, metric=distance_metric)
         else:
             raise ValueError(f"distance_metric {distance_metric} is not implemented.")
 
     return np.asarray(dis[seg_pred])
 
@@ -257,7 +270,67 @@
         pair_list = sorted(pair_data, key=lambda x: x[1], reverse=True)  # type: ignore
         pred_id, _ = zip(*pair_list)
 
     new_pred = torch.zeros_like(pred, dtype=torch.int)
     for idx, instance_id in enumerate(pred_id):
         new_pred[pred == instance_id] = idx + 1
     return new_pred
+
+
+def prepare_spacing(
+    spacing: int | float | np.ndarray | Sequence[int | float | np.ndarray | Sequence[int | float]] | None,
+    batch_size: int,
+    img_dim: int,
+) -> Sequence[None | int | float | np.ndarray | Sequence[int | float]]:
+    """
+    This function is used to prepare the `spacing` parameter to include batch dimension for the computation of
+    surface distance, hausdorff distance or surface dice.
+
+    An example with batch_size = 4 and img_dim = 3:
+    input spacing = None -> output spacing = [None, None, None, None]
+    input spacing = 0.8 -> output spacing = [0.8, 0.8, 0.8, 0.8]
+    input spacing = [0.8, 0.5, 0.9] -> output spacing = [[0.8, 0.5, 0.9], [0.8, 0.5, 0.9], [0.8, 0.5, 0.9], [0.8, 0.5, 0.9]]
+    input spacing = [0.8, 0.7, 1.2, 0.8] -> output spacing = [0.8, 0.7, 1.2, 0.8] (same as input)
+
+    An example with batch_size = 3 and img_dim = 3:
+    input spacing = [0.8, 0.5, 0.9] -> output spacing = [[0.8, 0.5, 0.9], [0.8, 0.5, 0.9], [0.8, 0.5, 0.9], [0.8, 0.5, 0.9]]
+
+    Args:
+        spacing: can be a float, a sequence of length `img_dim`, or a sequence with length `batch_size`
+        that includes floats or sequences of length `img_dim`.
+
+    Raises:
+        AssertionError: when `spacing` is a sequence of sequence, where the outer sequence length does not
+        equal `batch_size` or inner sequence length does not equal `img_dim`.
+
+    Returns:
+        spacing: a sequence with length `batch_size` that includes integers, floats or sequences of length `img_dim`.
+    """
+    if spacing is None or isinstance(spacing, (int, float)):
+        return list([spacing] * batch_size)
+    elif isinstance(spacing, (Sequence, np.ndarray)):
+        assert all(
+            isinstance(s, type(spacing[0])) for s in list(spacing)
+        ), "if `spacing` is a sequence, its elements should be of same type."
+
+        if isinstance(spacing[0], (Sequence, np.ndarray)):
+            assert (
+                len(spacing) == batch_size
+            ), "if `spacing` is a sequence of sequences, the outer sequence should have same length as batch size."
+            assert all(
+                len(s) == img_dim for s in list(spacing)
+            ), "each element of `spacing` list should either have same length as image dim."
+            assert all(
+                isinstance(i, (int, float)) for s in list(spacing) for i in list(s)
+            ), "if `spacing` is a sequence of sequences or 2D np.ndarray, the elements should be integers or floats."
+            return list(spacing)
+        elif isinstance(spacing[0], (int, float)):
+            assert (
+                len(spacing) == img_dim
+            ), "if `spacing` is a sequence of numbers, it should have same length as image dim."
+            return [spacing for _ in range(batch_size)]  # type: ignore
+        else:
+            raise AssertionError(f"`spacing` is a sequence of elements with unsupported type: {type(spacing[0])}")
+    else:
+        raise AssertionError(
+            "`spacing` should either be an integer, float, a sequence of numbers or a sequence of sequences."
+        )
```

### Comparing `monai-weekly-1.2.dev2315/monai/metrics/wrapper.py` & `monai-weekly-1.2.dev2316/monai/metrics/wrapper.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/__init__.py` & `monai-weekly-1.2.dev2316/monai/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/__init__.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/acti_norm.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/acti_norm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/activation.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/activation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/aspp.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/aspp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/backbone_fpn_utils.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/backbone_fpn_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     # select layers that wont be frozen
     if trainable_layers < 0 or trainable_layers > 5:
         raise ValueError(f"Trainable layers should be in the range [0,5], got {trainable_layers}")
     layers_to_train = ["layer4", "layer3", "layer2", "layer1", "conv1"][:trainable_layers]
     if trainable_layers == 5:
         layers_to_train.append("bn1")
     for name, parameter in backbone.named_parameters():
-        if all([not name.startswith(layer) for layer in layers_to_train]):
+        if all(not name.startswith(layer) for layer in layers_to_train):
             parameter.requires_grad_(False)
 
     if extra_blocks is None:
         extra_blocks = LastLevelMaxPool(spatial_dims)
 
     if returned_layers is None:
         returned_layers = [1, 2, 3, 4]
```

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/convolutions.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/convolutions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/crf.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/crf.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/denseblock.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/denseblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/dints_block.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/dints_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/downsample.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/downsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/dynunet_block.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/encoder.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/encoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/fcn.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/fcn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/feature_pyramid_network.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/feature_pyramid_network.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/fft_utils_t.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/fft_utils_t.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/localnet_block.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/mlp.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/mlp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/patchembedding.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/regunet_block.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/segresnet_block.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/selfattention.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/selfattention.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,21 +21,29 @@
 
 class SABlock(nn.Module):
     """
     A self-attention block, based on: "Dosovitskiy et al.,
     An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale <https://arxiv.org/abs/2010.11929>"
     """
 
-    def __init__(self, hidden_size: int, num_heads: int, dropout_rate: float = 0.0, qkv_bias: bool = False) -> None:
+    def __init__(
+        self,
+        hidden_size: int,
+        num_heads: int,
+        dropout_rate: float = 0.0,
+        qkv_bias: bool = False,
+        save_attn: bool = False,
+    ) -> None:
         """
         Args:
-            hidden_size: dimension of hidden layer.
-            num_heads: number of attention heads.
-            dropout_rate: faction of the input units to drop.
-            qkv_bias: bias term for the qkv linear layer.
+            hidden_size (int): dimension of hidden layer.
+            num_heads (int): number of attention heads.
+            dropout_rate (float, optional): faction of the input units to drop. Defaults to 0.0.
+            qkv_bias (bool, optional): bias term for the qkv linear layer. Defaults to False.
+            save_attn (bool, optional): to make accessible the attention matrix. Defaults to False.
 
         """
 
         super().__init__()
 
         if not (0 <= dropout_rate <= 1):
             raise ValueError("dropout_rate should be between 0 and 1.")
@@ -48,18 +56,25 @@
         self.qkv = nn.Linear(hidden_size, hidden_size * 3, bias=qkv_bias)
         self.input_rearrange = Rearrange("b h (qkv l d) -> qkv b l h d", qkv=3, l=num_heads)
         self.out_rearrange = Rearrange("b h l d -> b l (h d)")
         self.drop_output = nn.Dropout(dropout_rate)
         self.drop_weights = nn.Dropout(dropout_rate)
         self.head_dim = hidden_size // num_heads
         self.scale = self.head_dim**-0.5
+        self.save_attn = save_attn
+        self.att_mat = torch.Tensor()
 
     def forward(self, x):
         output = self.input_rearrange(self.qkv(x))
         q, k, v = output[0], output[1], output[2]
         att_mat = (torch.einsum("blxd,blyd->blxy", q, k) * self.scale).softmax(dim=-1)
+        if self.save_attn:
+            # no gradients and new tensor;
+            # https://pytorch.org/docs/stable/generated/torch.Tensor.detach.html
+            self.att_mat = att_mat.detach()
+
         att_mat = self.drop_weights(att_mat)
         x = torch.einsum("bhxy,bhyd->bhxd", att_mat, v)
         x = self.out_rearrange(x)
         x = self.out_proj(x)
         x = self.drop_output(x)
         return x
```

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/squeeze_and_excitation.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/transformerblock.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/transformerblock.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,36 +20,43 @@
 class TransformerBlock(nn.Module):
     """
     A transformer block, based on: "Dosovitskiy et al.,
     An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale <https://arxiv.org/abs/2010.11929>"
     """
 
     def __init__(
-        self, hidden_size: int, mlp_dim: int, num_heads: int, dropout_rate: float = 0.0, qkv_bias: bool = False
+        self,
+        hidden_size: int,
+        mlp_dim: int,
+        num_heads: int,
+        dropout_rate: float = 0.0,
+        qkv_bias: bool = False,
+        save_attn: bool = False,
     ) -> None:
         """
         Args:
-            hidden_size: dimension of hidden layer.
-            mlp_dim: dimension of feedforward layer.
-            num_heads: number of attention heads.
-            dropout_rate: faction of the input units to drop.
-            qkv_bias: apply bias term for the qkv linear layer
+            hidden_size (int): dimension of hidden layer.
+            mlp_dim (int): dimension of feedforward layer.
+            num_heads (int): number of attention heads.
+            dropout_rate (float, optional): faction of the input units to drop. Defaults to 0.0.
+            qkv_bias (bool, optional): apply bias term for the qkv linear layer. Defaults to False.
+            save_attn (bool, optional): to make accessible the attention matrix. Defaults to False.
 
         """
 
         super().__init__()
 
         if not (0 <= dropout_rate <= 1):
             raise ValueError("dropout_rate should be between 0 and 1.")
 
         if hidden_size % num_heads != 0:
             raise ValueError("hidden_size should be divisible by num_heads.")
 
         self.mlp = MLPBlock(hidden_size, mlp_dim, dropout_rate)
         self.norm1 = nn.LayerNorm(hidden_size)
-        self.attn = SABlock(hidden_size, num_heads, dropout_rate, qkv_bias)
+        self.attn = SABlock(hidden_size, num_heads, dropout_rate, qkv_bias, save_attn)
         self.norm2 = nn.LayerNorm(hidden_size)
 
     def forward(self, x):
         x = x + self.attn(self.norm1(x))
         x = x + self.mlp(self.norm2(x))
         return x
```

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/unetr_block.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/upsample.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/upsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/blocks/warp.py` & `monai-weekly-1.2.dev2316/monai/networks/blocks/warp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/layers/__init__.py` & `monai-weekly-1.2.dev2316/monai/networks/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/layers/convutils.py` & `monai-weekly-1.2.dev2316/monai/networks/layers/convutils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/layers/drop_path.py` & `monai-weekly-1.2.dev2316/monai/networks/layers/drop_path.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/layers/factories.py` & `monai-weekly-1.2.dev2316/monai/networks/layers/factories.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/layers/filtering.py` & `monai-weekly-1.2.dev2316/monai/networks/layers/filtering.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/layers/gmm.py` & `monai-weekly-1.2.dev2316/monai/networks/layers/gmm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/layers/simplelayers.py` & `monai-weekly-1.2.dev2316/monai/networks/layers/simplelayers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/layers/spatial_transforms.py` & `monai-weekly-1.2.dev2316/monai/networks/layers/spatial_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/layers/utils.py` & `monai-weekly-1.2.dev2316/monai/networks/layers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/layers/weight_init.py` & `monai-weekly-1.2.dev2316/monai/networks/layers/weight_init.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/__init__.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/ahnet.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/ahnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/attentionunet.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/attentionunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/autoencoder.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/basic_unet.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/basic_unetplusplus.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/classifier.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/classifier.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/densenet.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/densenet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/dints.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/dints.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/dynunet.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/dynunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/efficientnet.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/flexible_unet.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/flexible_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/fullyconnectednet.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/generator.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/generator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/highresnet.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/highresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/hovernet.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/milmodel.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/milmodel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/netadapter.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/netadapter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/regressor.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/regressor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/regunet.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/regunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/resnet.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/resnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/segresnet.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/segresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/segresnet_ds.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/senet.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/senet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/swin_unetr.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/torchvision_fc.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/torchvision_fc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/transchex.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/transchex.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/unet.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/unetr.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/varautoencoder.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/vit.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/vitautoenc.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,110 +14,109 @@
 from collections.abc import Sequence
 
 import torch
 import torch.nn as nn
 
 from monai.networks.blocks.patchembedding import PatchEmbeddingBlock
 from monai.networks.blocks.transformerblock import TransformerBlock
+from monai.networks.layers import Conv
+from monai.utils import ensure_tuple_rep
 
-__all__ = ["ViT"]
+__all__ = ["ViTAutoEnc"]
 
 
-class ViT(nn.Module):
+class ViTAutoEnc(nn.Module):
     """
     Vision Transformer (ViT), based on: "Dosovitskiy et al.,
     An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale <https://arxiv.org/abs/2010.11929>"
 
-    ViT supports Torchscript but only works for Pytorch after 1.8.
+    Modified to also give same dimension outputs as the input size of the image
     """
 
     def __init__(
         self,
         in_channels: int,
         img_size: Sequence[int] | int,
         patch_size: Sequence[int] | int,
+        out_channels: int = 1,
+        deconv_chns: int = 16,
         hidden_size: int = 768,
         mlp_dim: int = 3072,
         num_layers: int = 12,
         num_heads: int = 12,
         pos_embed: str = "conv",
-        classification: bool = False,
-        num_classes: int = 2,
         dropout_rate: float = 0.0,
         spatial_dims: int = 3,
-        post_activation="Tanh",
-        qkv_bias: bool = False,
     ) -> None:
         """
         Args:
-            in_channels: dimension of input channels.
+            in_channels: dimension of input channels or the number of channels for input
             img_size: dimension of input image.
             patch_size: dimension of patch size.
             hidden_size: dimension of hidden layer.
+            out_channels: number of output channels.
+            deconv_chns: number of channels for the deconvolution layers.
             mlp_dim: dimension of feedforward layer.
             num_layers: number of transformer blocks.
             num_heads: number of attention heads.
             pos_embed: position embedding layer type.
-            classification: bool argument to determine if classification is used.
-            num_classes: number of classes if classification is used.
             dropout_rate: faction of the input units to drop.
             spatial_dims: number of spatial dimensions.
-            post_activation: add a final acivation function to the classification head when `classification` is True.
-                Default to "Tanh" for `nn.Tanh()`. Set to other values to remove this function.
-            qkv_bias: apply bias to the qkv linear layer in self attention block
 
         Examples::
 
             # for single channel input with image size of (96,96,96), conv position embedding and segmentation backbone
-            >>> net = ViT(in_channels=1, img_size=(96,96,96), pos_embed='conv')
+            # It will provide an output of same size as that of the input
+            >>> net = ViTAutoEnc(in_channels=1, patch_size=(16,16,16), img_size=(96,96,96), pos_embed='conv')
 
-            # for 3-channel with image size of (128,128,128), 24 layers and classification backbone
-            >>> net = ViT(in_channels=3, img_size=(128,128,128), pos_embed='conv', classification=True)
-
-            # for 3-channel with image size of (224,224), 12 layers and classification backbone
-            >>> net = ViT(in_channels=3, img_size=(224,224), pos_embed='conv', classification=True, spatial_dims=2)
+            # for 3-channel with image size of (128,128,128), output will be same size as of input
+            >>> net = ViTAutoEnc(in_channels=3, patch_size=(16,16,16), img_size=(128,128,128), pos_embed='conv')
 
         """
 
         super().__init__()
 
-        if not (0 <= dropout_rate <= 1):
-            raise ValueError("dropout_rate should be between 0 and 1.")
-
-        if hidden_size % num_heads != 0:
-            raise ValueError("hidden_size should be divisible by num_heads.")
+        self.patch_size = ensure_tuple_rep(patch_size, spatial_dims)
+        self.spatial_dims = spatial_dims
 
-        self.classification = classification
         self.patch_embedding = PatchEmbeddingBlock(
             in_channels=in_channels,
             img_size=img_size,
             patch_size=patch_size,
             hidden_size=hidden_size,
             num_heads=num_heads,
             pos_embed=pos_embed,
             dropout_rate=dropout_rate,
-            spatial_dims=spatial_dims,
+            spatial_dims=self.spatial_dims,
         )
         self.blocks = nn.ModuleList(
-            [TransformerBlock(hidden_size, mlp_dim, num_heads, dropout_rate, qkv_bias) for i in range(num_layers)]
+            [TransformerBlock(hidden_size, mlp_dim, num_heads, dropout_rate) for i in range(num_layers)]
         )
         self.norm = nn.LayerNorm(hidden_size)
-        if self.classification:
-            self.cls_token = nn.Parameter(torch.zeros(1, 1, hidden_size))
-            if post_activation == "Tanh":
-                self.classification_head = nn.Sequential(nn.Linear(hidden_size, num_classes), nn.Tanh())
-            else:
-                self.classification_head = nn.Linear(hidden_size, num_classes)  # type: ignore
+
+        new_patch_size = [4] * self.spatial_dims
+        conv_trans = Conv[Conv.CONVTRANS, self.spatial_dims]
+        # self.conv3d_transpose* is to be compatible with existing 3d model weights.
+        self.conv3d_transpose = conv_trans(hidden_size, deconv_chns, kernel_size=new_patch_size, stride=new_patch_size)
+        self.conv3d_transpose_1 = conv_trans(
+            in_channels=deconv_chns, out_channels=out_channels, kernel_size=new_patch_size, stride=new_patch_size
+        )
 
     def forward(self, x):
+        """
+        Args:
+            x: input tensor must have isotropic spatial dimensions,
+                such as ``[batch_size, channels, sp_size, sp_size[, sp_size]]``.
+        """
+        spatial_size = x.shape[2:]
         x = self.patch_embedding(x)
-        if hasattr(self, "cls_token"):
-            cls_token = self.cls_token.expand(x.shape[0], -1, -1)
-            x = torch.cat((cls_token, x), dim=1)
         hidden_states_out = []
         for blk in self.blocks:
             x = blk(x)
             hidden_states_out.append(x)
         x = self.norm(x)
-        if hasattr(self, "classification_head"):
-            x = self.classification_head(x[:, 0])
+        x = x.transpose(1, 2)
+        d = [s // p for s, p in zip(spatial_size, self.patch_size)]
+        x = torch.reshape(x, [x.shape[0], x.shape[1], *d])
+        x = self.conv3d_transpose(x)
+        x = self.conv3d_transpose_1(x)
         return x, hidden_states_out
```

### Comparing `monai-weekly-1.2.dev2315/monai/networks/nets/vnet.py` & `monai-weekly-1.2.dev2316/monai/networks/nets/vnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/networks/utils.py` & `monai-weekly-1.2.dev2316/monai/networks/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -668,15 +668,15 @@
             onnx_out = ort_sess.run(None, input_dict)
         else:
             sess = onnxreference.ReferenceEvaluator(onnx_model)
             onnx_out = sess.run(None, input_dict)
         set_determinism(seed=None)
         # compare onnx/ort and PyTorch results
         for r1, r2 in zip(torch_out, onnx_out):
-            torch.testing.assert_allclose(r1.cpu(), r2, rtol=rtol, atol=atol)  # type: ignore
+            torch.testing.assert_allclose(r1.cpu(), r2, rtol=rtol, atol=atol)
 
     return onnx_model
 
 
 def convert_to_torchscript(
     model: nn.Module,
     filename_or_obj: Any | None = None,
@@ -702,25 +702,25 @@
         verify: whether to verify the input and output of TorchScript model.
             if `filename_or_obj` is not None, load the saved TorchScript model and verify.
         inputs: input test data to verify model, should be a sequence of data, every item maps to a argument
             of `model()` function.
         device: target device to verify the model, if None, use CUDA if available.
         rtol: the relative tolerance when comparing the outputs of PyTorch model and TorchScript model.
         atol: the absolute tolerance when comparing the outputs of PyTorch model and TorchScript model.
-        use_trace: whether to use `torch.jit.trace` to export the torchscript model.
-        kwargs: other arguments except `obj` for `torch.jit.script()` to convert model, for more details:
-            https://pytorch.org/docs/master/generated/torch.jit.script.html.
+        use_trace: whether to use `torch.jit.trace` to export the TorchScript model.
+        kwargs: other arguments except `obj` for `torch.jit.script()` or `torch.jit.trace()` (if use_trace is True)
+            to convert model, for more details: https://pytorch.org/docs/master/generated/torch.jit.script.html.
 
     """
     model.eval()
     with torch.no_grad():
         if use_trace:
             if inputs is None:
                 raise ValueError("Missing input data for tracing convert.")
-            script_module = torch.jit.trace(model, example_inputs=inputs)
+            script_module = torch.jit.trace(model, example_inputs=inputs, **kwargs)
         else:
             script_module = torch.jit.script(model, **kwargs)
         if filename_or_obj is not None:
             torch.jit.save(m=script_module, f=filename_or_obj, _extra_files=extra_files)
 
     if verify:
         if device is None:
@@ -744,47 +744,143 @@
             if isinstance(r1, torch.Tensor) or isinstance(r2, torch.Tensor):
                 assert_fn = torch.testing.assert_close if pytorch_after(1, 11) else torch.testing.assert_allclose
                 assert_fn(r1, r2, rtol=rtol, atol=atol)  # type: ignore
 
     return script_module
 
 
+def _onnx_trt_compile(
+    onnx_model,
+    min_shape: Sequence[int],
+    opt_shape: Sequence[int],
+    max_shape: Sequence[int],
+    device: int,
+    precision: str,
+    input_names: Sequence[str] | None,
+    output_names: Sequence[str] | None,
+):
+    """
+    This function takes an ONNX model as input, exports it to a TensorRT engine, wraps the TensorRT engine
+    to a TensorRT engine-based TorchScript model and return the TorchScript model.
+
+    Args:
+        onnx_model: the source ONNX model to compile.
+        min_shape: the minimum input shape of the converted TensorRT model.
+        opt_shape: the optimization input shape of the model, on which the TensorRT optimizes.
+        max_shape: the maximum input shape of the converted TensorRT model.
+        device: the target GPU index to convert and verify the model.
+        precision: the weight precision of the converted TensorRT engine-based TorchScript model.
+            Should be 'fp32' or 'fp16'.
+        input_names: optional input names of the ONNX model. Should be a sequence like
+            `['input_0', 'input_1', ..., 'input_N']` where N equals to the number of the
+            model inputs.
+        output_names: optional output names of the ONNX model. Should be a sequence like
+            `['output_0', 'output_1', ..., 'output_N']` where N equals to the number of
+            the model outputs.
+
+    """
+    trt, _ = optional_import("tensorrt", "8.5.3")
+    torch_tensorrt, _ = optional_import("torch_tensorrt", "1.4.0")
+
+    input_shapes = (min_shape, opt_shape, max_shape)
+    # default to an empty list to fit the `torch_tensorrt.ts.embed_engine_in_new_module` function.
+    input_names = [] if not input_names else input_names
+    output_names = [] if not output_names else output_names
+
+    # set up the TensorRT builder
+    torch_tensorrt.set_device(device)
+    logger = trt.Logger(trt.Logger.WARNING)
+    builder = trt.Builder(logger)
+    network = builder.create_network(1 << int(trt.NetworkDefinitionCreationFlag.EXPLICIT_BATCH))
+    profile = builder.create_optimization_profile()
+    if input_names:
+        profile.set_shape(input_names[0], *input_shapes)
+
+    # parse the ONNX model
+    parser = trt.OnnxParser(network, logger)
+    success = parser.parse(onnx_model.SerializeToString())
+    if not success:
+        parser_error_message = ""
+        for idx in range(parser.num_errors):
+            parser_error_message += parser.get_error(idx).desc() + "\n"
+        raise Exception(f"TensorRT cannot parse the ONNX model, due to:\n{parser_error_message}")
+
+    # set up the conversion configuration
+    config = builder.create_builder_config()
+    config.set_memory_pool_limit(trt.MemoryPoolType.WORKSPACE, 1 << 31)
+    config.add_optimization_profile(profile)
+    if precision == "fp16":
+        config.set_flag(trt.BuilderFlag.FP16)
+    serialized_engine = builder.build_serialized_network(network, config)
+    f = io.BytesIO()
+    f.write(serialized_engine)
+
+    # wrap the serialized TensorRT engine back to a TorchScript module.
+    trt_model = torch_tensorrt.ts.embed_engine_in_new_module(
+        f.getvalue(), torch.device(f"cuda:{device}"), input_names, output_names
+    )
+    return trt_model
+
+
 def convert_to_trt(
     model: nn.Module,
     precision: str,
     input_shape: Sequence[int],
     dynamic_batchsize: Sequence[int] | None = None,
     use_trace: bool = False,
     filename_or_obj: Any | None = None,
     verify: bool = False,
     device: int | None = None,
+    use_onnx: bool | None = False,
+    onnx_input_names: Sequence[str] | None = ("input_0",),
+    onnx_output_names: Sequence[str] | None = ("output_0",),
     rtol: float = 1e-2,
     atol: float = 0.0,
+    **kwargs,
 ):
     """
-    Utility to convert a model into a TensorRT engine based torchscript model with optional input / output data verification.
+    Utility to export a model into a TensorRT engine-based TorchScript model with optional input / output data verification.
+
+    There are two ways to export a model:
+    1, Torch-TensorRT way: PyTorch module ---> TorchScript module ---> TensorRT engine-based TorchScript.
+    2, ONNX-TensorRT way: PyTorch module ---> TorchScript module ---> ONNX model ---> TensorRT engine --->
+    TensorRT engine-based TorchScript.
+
+    When exporting through the first way, some models suffer from the slowdown problem, since Torch-TensorRT
+    may only convert a little part of the PyTorch model to the TensorRT engine. However when exporting through
+    the second way, some Python data structures like `dict` are not supported. And some TorchScript models are
+    not supported by the ONNX if exported through `torch.jit.script`.
 
     Args:
         model: a source PyTorch model to convert.
-        precision: the weight precision of the converted TensorRT engine based torchscript models. Should be 'fp32' or 'fp16'.
+        precision: the weight precision of the converted TensorRT engine based TorchScript models. Should be 'fp32' or 'fp16'.
         input_shape: the input shape that is used to convert the model. Should be a list like [N, C, H, W] or
             [N, C, H, W, D].
         dynamic_batchsize: a sequence with three elements to define the batch size range of the input for the model to be
             converted. Should be a sequence like [MIN_BATCH, OPT_BATCH, MAX_BATCH]. After converted, the batchsize of model
             input should between `MIN_BATCH` and `MAX_BATCH` and the `OPT_BATCH` is the best performance batchsize that the
             TensorRT tries to fit. The `OPT_BATCH` should be the most frequently used input batchsize in the application,
             default to None.
-        use_trace: whether using `torch.jit.trace` to convert the pytorch model to torchscript model and then convert to
-            a TensorRT engine based torchscript model, default to False.
+        use_trace: whether using `torch.jit.trace` to convert the PyTorch model to a TorchScript model and then convert to
+            a TensorRT engine based TorchScript model or an ONNX model (if `use_onnx` is True), default to False.
         filename_or_obj: if not None, specify a file-like object (has to implement write and flush) or a string containing a
-            file path name to load the TensorRT engine based torchscript model for verifying.
-        verify: whether to verify the input and output of the TensorRT engine based torchscript model.
+            file path name to load the TensorRT engine based TorchScript model for verifying.
+        verify: whether to verify the input and output of the TensorRT engine based TorchScript model.
         device: the target GPU index to convert and verify the model. If None, use #0 GPU.
+        use_onnx: whether to use the ONNX-TensorRT way to export the TensorRT engine-based TorchScript model.
+        onnx_input_names: optional input names of the ONNX model. This arg is only useful when `use_onnx` is True. Should be
+            a sequence like `('input_0', 'input_1', ..., 'input_N')` where N equals to the number of the model inputs. If not
+            given, will use `('input_0',)`, which supposes the model only has one input.
+        onnx_output_names: optional output names of the ONNX model. This arg is only useful when `use_onnx` is True. Should be
+            a sequence like `('output_0', 'output_1', ..., 'output_N')` where N equals to the number of the model outputs. If
+            not given, will use `('output_0',)`, which supposes the model only has one output.
         rtol: the relative tolerance when comparing the outputs between the PyTorch model and TensorRT model.
         atol: the absolute tolerance when comparing the outputs between the PyTorch model and TensorRT model.
+        kwargs: other arguments except `module`, `inputs`, `enabled_precisions` and `device` for `torch_tensorrt.compile()`
+            to compile model, for more details: https://pytorch.org/TensorRT/py_api/torch_tensorrt.html#torch-tensorrt-py.
     """
 
     torch_tensorrt, _ = optional_import("torch_tensorrt", version="1.4.0")
 
     if not torch.cuda.is_available():
         raise Exception("Cannot find any GPU devices.")
 
@@ -798,42 +894,70 @@
         warnings.warn(f"The dynamic batch range sequence should have 3 elements, but got {dynamic_batchsize} elements.")
 
     device = device if device else 0
     target_device = torch.device(f"cuda:{device}") if device else torch.device("cuda:0")
     convert_precision = torch.float32 if precision == "fp32" else torch.half
     inputs = [torch.rand(ensure_tuple(input_shape)).to(target_device)]
 
-    # convert the torch model, torchscript model and input to target device
-    model = model.eval().to(target_device)
-    ir_model = convert_to_torchscript(model, device=target_device, inputs=inputs, use_trace=use_trace)
-    ir_model.eval().to(target_device)
-
     def scale_batch_size(input_shape: Sequence[int], scale_num: int):
         scale_shape = [*input_shape]
         scale_shape[0] *= scale_num
         return scale_shape
 
-    # Use the dynamic batchsize range to generate compiler input and compile the model
+    # Use the dynamic batchsize range to generate the min, opt and max model input shape
     if dynamic_batchsize:
         min_input_shape = scale_batch_size(input_shape, dynamic_batchsize[0])
         opt_input_shape = scale_batch_size(input_shape, dynamic_batchsize[1])
         max_input_shape = scale_batch_size(input_shape, dynamic_batchsize[2])
     else:
         min_input_shape = opt_input_shape = max_input_shape = input_shape
 
-    with torch.no_grad():
-        with torch.cuda.device(device=device):
-            input_placeholder = [
-                torch_tensorrt.Input(min_shape=min_input_shape, opt_shape=opt_input_shape, max_shape=max_input_shape)
-            ]
-            trt_model = torch_tensorrt.compile(
-                ir_model, inputs=input_placeholder, enabled_precisions=convert_precision, device=target_device
-            )
+    # convert the torch model to a TorchScript model on target device
+    model = model.eval().to(target_device)
+    ir_model = convert_to_torchscript(model, device=target_device, inputs=inputs, use_trace=use_trace)
+    ir_model.eval()
+
+    if use_onnx:
+        # set the batch dim as dynamic
+        dynamic_axes = {k: {0: "batchsize"} for k in onnx_input_names} if onnx_input_names else {}
+        dynamic_axes.update({k: {0: "batchsize"} for k in onnx_output_names} if onnx_output_names else {})
+        ir_model = convert_to_onnx(
+            model, inputs, onnx_input_names, onnx_output_names, use_trace=use_trace, dynamic_axes=dynamic_axes
+        )
+
+        # convert the model through the ONNX-TensorRT way
+        trt_model = _onnx_trt_compile(
+            ir_model,
+            min_shape=min_input_shape,
+            opt_shape=opt_input_shape,
+            max_shape=max_input_shape,
+            device=device,
+            precision=precision,
+            input_names=onnx_input_names,
+            output_names=onnx_output_names,
+        )
+    else:
+        # convert the model through the Torch-TensorRT way
+        ir_model.to(target_device)
+        with torch.no_grad():
+            with torch.cuda.device(device=device):
+                input_placeholder = [
+                    torch_tensorrt.Input(
+                        min_shape=min_input_shape, opt_shape=opt_input_shape, max_shape=max_input_shape
+                    )
+                ]
+                trt_model = torch_tensorrt.compile(
+                    ir_model,
+                    inputs=input_placeholder,
+                    enabled_precisions=convert_precision,
+                    device=target_device,
+                    **kwargs,
+                )
 
-    # verify the outputs between the trt model and torch model
+    # verify the outputs between the TensorRT model and PyTorch model
     if verify:
         if inputs is None:
             raise ValueError("Missing input data for verification.")
 
         trt_model = torch.jit.load(filename_or_obj) if filename_or_obj is not None else trt_model
 
         with torch.no_grad():
```

### Comparing `monai-weekly-1.2.dev2315/monai/optimizers/__init__.py` & `monai-weekly-1.2.dev2316/monai/transforms/croppad/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,7 @@
 # You may obtain a copy of the License at
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-from __future__ import annotations
-
-from .lr_finder import LearningRateFinder
-from .lr_scheduler import ExponentialLR, LinearLR, WarmupCosineSchedule
-from .novograd import Novograd
-from .utils import generate_param_groups
```

### Comparing `monai-weekly-1.2.dev2315/monai/optimizers/lr_finder.py` & `monai-weekly-1.2.dev2316/monai/optimizers/lr_finder.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
     def range_test(
         self,
         train_loader: DataLoader,
         val_loader: DataLoader | None = None,
         image_extractor: Callable = default_image_extractor,
         label_extractor: Callable = default_label_extractor,
         start_lr: float | None = None,
-        end_lr: int = 10,
+        end_lr: float = 10.0,
         num_iter: int = 100,
         step_mode: str = "exp",
         smooth_f: float = 0.05,
         diverge_th: int = 5,
         accumulation_steps: int = 1,
         non_blocking_transfer: bool = True,
         auto_reset: bool = True,
```

### Comparing `monai-weekly-1.2.dev2315/monai/optimizers/lr_scheduler.py` & `monai-weekly-1.2.dev2316/monai/optimizers/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/optimizers/novograd.py` & `monai-weekly-1.2.dev2316/monai/optimizers/novograd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/optimizers/utils.py` & `monai-weekly-1.2.dev2316/monai/optimizers/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/__init__.py` & `monai-weekly-1.2.dev2316/monai/transforms/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -620,14 +620,15 @@
     TransposeD,
     TransposeDict,
 )
 from .utils import (
     Fourier,
     allow_missing_keys_mode,
     attach_hook,
+    check_non_lazy_pending_ops,
     compute_divisible_spatial_size,
     convert_applied_interp_mode,
     convert_pad_mode,
     convert_to_contiguous,
     copypaste_arrays,
     create_control_grid,
     create_grid,
```

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/adaptors.py` & `monai-weekly-1.2.dev2316/monai/transforms/adaptors.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/compose.py` & `monai-weekly-1.2.dev2316/monai/transforms/compose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/croppad/__init__.py` & `monai-weekly-1.2.dev2316/monai/transforms/intensity/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/croppad/array.py` & `monai-weekly-1.2.dev2316/monai/transforms/croppad/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -776,16 +776,14 @@
 
     def compute_bounding_box(self, img: torch.Tensor) -> tuple[np.ndarray, np.ndarray]:
         """
         Compute the start points and end points of bounding box to crop.
         And adjust bounding box coords to be divisible by `k`.
 
         """
-        if isinstance(img, MetaTensor) and img.pending_operations:
-            warnings.warn("foreground computation may not be accurate if the image has pending operations.")
         box_start, box_end = generate_spatial_bounding_box(
             img, self.select_fn, self.channel_indices, self.margin, self.allow_smaller
         )
         box_start_, *_ = convert_data_type(box_start, output_type=np.ndarray, dtype=np.int16, wrap_sequence=True)
         box_end_, *_ = convert_data_type(box_end, output_type=np.ndarray, dtype=np.int16, wrap_sequence=True)
         orig_spatial_size = box_end_ - box_start_
         # make the spatial size divisible by `k`
@@ -865,16 +863,14 @@
     ):
         self.spatial_size = ensure_tuple(spatial_size)
         self.num_samples = int(num_samples)
         self.weight_map = weight_map
         self.centers: list[np.ndarray] = []
 
     def randomize(self, weight_map: NdarrayOrTensor) -> None:
-        if isinstance(weight_map, MetaTensor) and weight_map.pending_operations:
-            warnings.warn("weight map has pending operations, the sampling may not be correct.")
         self.centers = weighted_patch_samples(
             spatial_size=self.spatial_size, w=weight_map[0], n_samples=self.num_samples, r_state=self.R
         )  # using only the first channel as weight map
 
     @LazyTransform.lazy_evaluation.setter  # type: ignore
     def lazy_evaluation(self, _val: bool):
         self._lazy_evaluation = _val
@@ -1011,18 +1007,14 @@
         fg_indices: NdarrayOrTensor | None = None,
         bg_indices: NdarrayOrTensor | None = None,
         image: torch.Tensor | None = None,
     ) -> None:
         fg_indices_ = self.fg_indices if fg_indices is None else fg_indices
         bg_indices_ = self.bg_indices if bg_indices is None else bg_indices
         if fg_indices_ is None or bg_indices_ is None:
-            if isinstance(label, MetaTensor) and label.pending_operations:
-                warnings.warn("label has pending operations, the fg/bg indices may be incorrect.")
-            if isinstance(image, MetaTensor) and image.pending_operations:
-                warnings.warn("image has pending operations, the fg/bg indices may be incorrect.")
             if label is None:
                 raise ValueError("label must be provided.")
             fg_indices_, bg_indices_ = map_binary_to_indices(label, image, self.image_threshold)
         _shape = None
         if label is not None:
             _shape = label.peek_pending_shape() if isinstance(label, MetaTensor) else label.shape[1:]
         elif image is not None:
@@ -1191,18 +1183,14 @@
         self,
         label: torch.Tensor | None = None,
         indices: list[NdarrayOrTensor] | None = None,
         image: torch.Tensor | None = None,
     ) -> None:
         indices_ = self.indices if indices is None else indices
         if indices_ is None:
-            if isinstance(label, MetaTensor) and label.pending_operations:
-                warnings.warn("label has pending operations, the fg/bg indices may be incorrect.")
-            if isinstance(image, MetaTensor) and image.pending_operations:
-                warnings.warn("image has pending operations, the fg/bg indices may be incorrect.")
             if label is None:
                 raise ValueError("label must not be None.")
             indices_ = map_classes_to_indices(
                 label, self.num_classes, image, self.image_threshold, self.max_samples_per_class
             )
         _shape = None
         if label is not None:
```

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/croppad/batch.py` & `monai-weekly-1.2.dev2316/monai/transforms/croppad/batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/croppad/dictionary.py` & `monai-weekly-1.2.dev2316/monai/transforms/croppad/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/croppad/functional.py` & `monai-weekly-1.2.dev2316/monai/transforms/croppad/functional.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/intensity/__init__.py` & `monai-weekly-1.2.dev2316/monai/transforms/io/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/intensity/array.py` & `monai-weekly-1.2.dev2316/monai/transforms/intensity/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/intensity/dictionary.py` & `monai-weekly-1.2.dev2316/monai/transforms/intensity/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/inverse.py` & `monai-weekly-1.2.dev2316/monai/transforms/inverse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/inverse_batch_transform.py` & `monai-weekly-1.2.dev2316/monai/transforms/inverse_batch_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/io/__init__.py` & `monai-weekly-1.2.dev2316/monai/transforms/meta_utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/io/array.py` & `monai-weekly-1.2.dev2316/monai/transforms/io/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/io/dictionary.py` & `monai-weekly-1.2.dev2316/monai/transforms/io/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/lazy/__init__.py` & `monai-weekly-1.2.dev2316/monai/transforms/lazy/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/lazy/functional.py` & `monai-weekly-1.2.dev2316/monai/transforms/lazy/functional.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/lazy/utils.py` & `monai-weekly-1.2.dev2316/monai/transforms/lazy/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,15 @@
         matrix: affine transformation matrix.
         kwargs: currently supports (see also: ``monai.utils.enums.LazyAttr``)
 
             - "lazy_shape" for output spatial shape
             - "lazy_padding_mode"
             - "lazy_interpolation_mode" (this option might be ignored when ``mode="auto"``.)
             - "lazy_align_corners"
-            - "lazy_dtype"
+            - "lazy_dtype" (dtype for resampling computation; this might be ignored when ``mode="auto"``.)
             - "atol" for tolerance for matrix floating point comparison.
             - "lazy_resample_mode" for resampling backend, default to `"auto"`. Setting to other values will use the
               `monai.transforms.SpatialResample` for resampling.
 
     See Also:
         :py:class:`monai.transforms.SpatialResample`
     """
@@ -212,16 +212,18 @@
             raise ValueError(f"Resampling out_spatial_size should be positive, got {out_spatial_size}.")
         if (
             allclose(matrix_np, np.eye(len(matrix_np)), atol=atol)
             and len(in_shape) == len(out_spatial_size)
             and allclose(convert_to_numpy(in_shape, wrap_sequence=True), out_spatial_size)
         ):
             img.affine = call_kwargs["dst_affine"]
+            img = img.to(torch.float32)  # consistent with monai.transforms.spatial.functional.spatial_resample
             return img
         img = monai.transforms.crop_or_pad_nd(img, matrix_np, out_spatial_size, mode=call_kwargs["padding_mode"])
+        img = img.to(torch.float32)  # consistent with monai.transforms.spatial.functional.spatial_resample
         img.affine = call_kwargs["dst_affine"]
         return img
 
     resampler = monai.transforms.SpatialResample(**init_kwargs)
     resampler.lazy_evaluation = False  # resampler is a lazytransform
     with resampler.trace_transform(False):  # don't track this transform in `img`
         return resampler(img=img, **call_kwargs)
```

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/meta_utility/__init__.py` & `monai-weekly-1.2.dev2316/monai/transforms/post/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/meta_utility/dictionary.py` & `monai-weekly-1.2.dev2316/monai/transforms/meta_utility/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/nvtx.py` & `monai-weekly-1.2.dev2316/monai/transforms/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/post/__init__.py` & `monai-weekly-1.2.dev2316/monai/transforms/signal/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/post/array.py` & `monai-weekly-1.2.dev2316/monai/transforms/post/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/post/dictionary.py` & `monai-weekly-1.2.dev2316/monai/transforms/post/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/signal/__init__.py` & `monai-weekly-1.2.dev2316/monai/transforms/smooth_field/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/signal/array.py` & `monai-weekly-1.2.dev2316/monai/transforms/signal/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/smooth_field/__init__.py` & `monai-weekly-1.2.dev2316/monai/transforms/spatial/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/smooth_field/array.py` & `monai-weekly-1.2.dev2316/monai/transforms/smooth_field/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/smooth_field/dictionary.py` & `monai-weekly-1.2.dev2316/monai/transforms/smooth_field/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/spatial/__init__.py` & `monai-weekly-1.2.dev2316/monai/transforms/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/spatial/array.py` & `monai-weekly-1.2.dev2316/monai/transforms/spatial/array.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,14 +226,15 @@
         kw_args["dst_affine"] = kw_args.pop("src_affine")
         kw_args["spatial_size"] = transform[TraceKeys.ORIG_SIZE]
         if kw_args.get("align_corners") == TraceKeys.NONE:
             kw_args["align_corners"] = False
         with self.trace_transform(False):
             # we can't use `self.__call__` in case a child class calls this inverse.
             out: torch.Tensor = SpatialResample.__call__(self, data, **kw_args)
+        kw_args["src_affine"] = kw_args.get("dst_affine")
         return out
 
 
 class ResampleToMatch(SpatialResample):
     """Resample an image to match given metadata. The affine matrix will be aligned,
     and the size of the output image will match."""
```

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/spatial/dictionary.py` & `monai-weekly-1.2.dev2316/monai/transforms/spatial/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/spatial/functional.py` & `monai-weekly-1.2.dev2316/monai/transforms/spatial/functional.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/traits.py` & `monai-weekly-1.2.dev2316/monai/transforms/traits.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/transform.py` & `monai-weekly-1.2.dev2316/monai/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/utility/array.py` & `monai-weekly-1.2.dev2316/monai/transforms/utility/array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/utility/dictionary.py` & `monai-weekly-1.2.dev2316/monai/transforms/utility/dictionary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/utils.py` & `monai-weekly-1.2.dev2316/monai/transforms/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 
 __all__ = [
     "allow_missing_keys_mode",
     "check_boundaries",
     "compute_divisible_spatial_size",
     "convert_applied_interp_mode",
     "copypaste_arrays",
+    "check_non_lazy_pending_ops",
     "create_control_grid",
     "create_grid",
     "create_rotate",
     "create_scale",
     "create_shear",
     "create_translate",
     "extreme_points_to_image",
@@ -290,14 +291,35 @@
     if not inplace:
         dest = np.full(resize_dims, fill_value, img.dtype)  # type: ignore
         dest[destslices] = img[srcslices]
         return dest
     return img[srcslices]
 
 
+def check_non_lazy_pending_ops(
+    input_array: NdarrayOrTensor, name: None | str = None, raise_error: bool = False
+) -> None:
+    """
+    Check whether the input array has pending operations, raise an error or warn when it has.
+
+    Args:
+        input_array: input array to be checked.
+        name: an optional name to be included in the error message.
+        raise_error: whether to raise an error, default to False, a warning message will be issued instead.
+    """
+    if isinstance(input_array, monai.data.MetaTensor) and input_array.pending_operations:
+        msg = (
+            "The input image is a MetaTensor and has pending operations,\n"
+            f"but the function {name or ''} assumes non-lazy input, result may be incorrect."
+        )
+        if raise_error:
+            raise ValueError(msg)
+        warnings.warn(msg)
+
+
 def map_binary_to_indices(
     label: NdarrayOrTensor, image: NdarrayOrTensor | None = None, image_threshold: float = 0.0
 ) -> tuple[NdarrayOrTensor, NdarrayOrTensor]:
     """
     Compute the foreground and background of input label data, return the indices after fattening.
     For example:
     ``label = np.array([[[0, 1, 1], [1, 0, 1], [1, 1, 0]]])``
@@ -306,21 +328,22 @@
     Args:
         label: use the label data to get the foreground/background information.
         image: if image is not None, use ``label = 0 & image > image_threshold``
             to define background. so the output items will not map to all the voxels in the label.
         image_threshold: if enabled `image`, use ``image > image_threshold`` to
             determine the valid image content area and select background only in this area.
     """
-
+    check_non_lazy_pending_ops(label, name="map_binary_to_indices")
     # Prepare fg/bg indices
     if label.shape[0] > 1:
         label = label[1:]  # for One-Hot format data, remove the background channel
     label_flat = ravel(any_np_pt(label, 0))  # in case label has multiple dimensions
     fg_indices = nonzero(label_flat)
     if image is not None:
+        check_non_lazy_pending_ops(image, name="map_binary_to_indices")
         img_flat = ravel(any_np_pt(image > image_threshold, 0))
         img_flat, *_ = convert_to_dst_type(img_flat, label, dtype=bool)
         bg_indices = nonzero(img_flat & ~label_flat)
     else:
         bg_indices = nonzero(~label_flat)
 
     # no need to save the indices in GPU, otherwise, still need to move to CPU at runtime when crop by indices
@@ -353,16 +376,18 @@
             region of the image (``image > image_threshold``).
         image_threshold: if enabled `image`, use ``image > image_threshold`` to
             determine the valid image content area and select class indices only in this area.
         max_samples_per_class: maximum length of indices in each class to reduce memory consumption.
             Default is None, no subsampling.
 
     """
+    check_non_lazy_pending_ops(label, name="map_classes_to_indices")
     img_flat: NdarrayOrTensor | None = None
     if image is not None:
+        check_non_lazy_pending_ops(image, name="map_classes_to_indices")
         img_flat = ravel((image > image_threshold).any(0))
 
     # assuming the first dimension is channel
     channels = len(label)
 
     num_classes_: int = channels
     if channels == 1:
@@ -406,14 +431,15 @@
         n_samples: number of patch samples
         r_state: a random state container
 
     Returns:
         a list of `n_samples` N-D integers representing the spatial sampling location of patches.
 
     """
+    check_non_lazy_pending_ops(w, name="weighted_patch_samples")
     if w is None:
         raise ValueError("w must be an ND array, got None.")
     if r_state is None:
         r_state = np.random.RandomState()
     img_size = np.asarray(w.shape, dtype=int)
     win_size = np.asarray(fall_back_tuple(spatial_size, img_size), dtype=int)
 
@@ -933,14 +959,15 @@
         select_fn: function to select expected foreground, default is to select values > 0.
         channel_indices: if defined, select foreground only on the specified channels
             of image. if None, select foreground on the whole image.
         margin: add margin value to spatial dims of the bounding box, if only 1 value provided, use it for all dims.
         allow_smaller: when computing box size with `margin`, whether allow the image size to be smaller
             than box size, default to `True`.
     """
+    check_non_lazy_pending_ops(img, name="generate_spatial_bounding_box")
     spatial_size = img.shape[1:]
     data = img[list(ensure_tuple(channel_indices))] if channel_indices is not None else img
     data = select_fn(data).any(0)
     ndim = len(data.shape)
     margin = ensure_tuple_rep(margin, ndim)
     for m in margin:
         if m < 0:
@@ -1171,14 +1198,15 @@
         The output format of the coordinates is:
 
         [1st_spatial_dim_min, 1st_spatial_dim_max, 2nd_spatial_dim_min, ..., Nth_spatial_dim_max]
 
     Raises:
         ValueError: When the input image does not have any foreground pixel.
     """
+    check_non_lazy_pending_ops(img, name="get_extreme_points")
     if rand_state is None:
         rand_state = np.random.random.__self__  # type: ignore
     indices = where(img != background)
     if np.size(indices[0]) == 0:
         raise ValueError("get_extreme_points: no foreground object in mask!")
 
     def _get_point(val, dim):
```

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/utils_create_transform_ims.py` & `monai-weekly-1.2.dev2316/monai/transforms/utils_create_transform_ims.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/transforms/utils_pytorch_numpy_unification.py` & `monai-weekly-1.2.dev2316/monai/transforms/utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/utils/__init__.py` & `monai-weekly-1.2.dev2316/monai/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 # have to explicitly bring these in here to resolve circular import issues
 from .aliases import alias, resolve_name
 from .decorators import MethodReplacer, RestartGenerator
 from .deprecate_utils import DeprecatedError, deprecated, deprecated_arg, deprecated_arg_default
 from .dist import RankFilter, evenly_divisible_all_gather, get_dist_device, string_list_all_gather
 from .enums import (
+    AlgoKeys,
     Average,
     BlendMode,
     BoxModeName,
     BundleProperty,
     BundlePropertyConfig,
     ChannelMatching,
     ColorOrder,
```

### Comparing `monai-weekly-1.2.dev2315/monai/utils/aliases.py` & `monai-weekly-1.2.dev2316/monai/utils/aliases.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/utils/decorators.py` & `monai-weekly-1.2.dev2316/monai/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/utils/deprecate_utils.py` & `monai-weekly-1.2.dev2316/monai/utils/deprecate_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/utils/dist.py` & `monai-weekly-1.2.dev2316/monai/utils/dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/utils/enums.py` & `monai-weekly-1.2.dev2316/monai/utils/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import random
 from enum import Enum
 
+from monai.utils import deprecated
+
 __all__ = [
     "StrEnum",
     "NumpyPadMode",
     "GridSampleMode",
     "SplineMode",
     "InterpolateMode",
     "UpsampleMode",
@@ -52,14 +54,15 @@
     "LabelStatsKeys",
     "AlgoEnsembleKeys",
     "HoVerNetMode",
     "HoVerNetBranch",
     "LazyAttr",
     "BundleProperty",
     "BundlePropertyConfig",
+    "AlgoKeys",
 ]
 
 
 class StrEnum(str, Enum):
     """
     Enum subclass that converts its value to a string.
 
@@ -588,14 +591,15 @@
     PIXEL_PCT = "foreground_percentage"
     IMAGE_INTST = "image_intensity"
     LABEL = "label"
     LABEL_SHAPE = "shape"
     LABEL_NCOMP = "ncomponents"
 
 
+@deprecated(since="1.2", msg_suffix="please use `AlgoKeys` instead.")
 class AlgoEnsembleKeys(StrEnum):
     """
     Default keys for Mixed Ensemble
     """
 
     ID = "identifier"
     ALGO = "infer_algo"
@@ -660,7 +664,22 @@
     `ID` is the config item ID of the property.
     `REF_ID` is the ID of config item which is supposed to refer to this property.
     this field is only useful to check the optional property ID.
     """
 
     ID = "id"
     REF_ID = "refer_id"
+
+
+class AlgoKeys(StrEnum):
+    """
+    Default keys for templated Auto3DSeg Algo.
+    `ID` is the identifier of the algorithm. The string has the format of <name>_<idx>_<other>.
+    `ALGO` is the Auto3DSeg Algo instance.
+    `IS_TRAINED` is the status that shows if the Algo has been trained.
+    `SCORE` is the score the Algo has achieved after training.
+    """
+
+    ID = "identifier"
+    ALGO = "algo_instance"
+    IS_TRAINED = "is_trained"
+    SCORE = "best_metric"
```

### Comparing `monai-weekly-1.2.dev2315/monai/utils/jupyter_utils.py` & `monai-weekly-1.2.dev2316/monai/utils/jupyter_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/utils/misc.py` & `monai-weekly-1.2.dev2316/monai/utils/misc.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import shutil
 import tempfile
 import types
 import warnings
 from ast import literal_eval
 from collections.abc import Callable, Iterable, Sequence
 from distutils.util import strtobool
+from math import log10
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, TypeVar, cast, overload
 
 import numpy as np
 import torch
 
 from monai.config.type_definitions import NdarrayOrTensor, NdarrayTensor, PathLike
@@ -64,14 +65,17 @@
     "has_option",
     "sample_slices",
     "check_parent_dir",
     "save_obj",
     "label_union",
     "path_to_uri",
     "pprint_edges",
+    "check_key_duplicates",
+    "CheckKeyDuplicatesYamlLoader",
+    "ConvertUnits",
 ]
 
 _seed = None
 _flag_deterministic = torch.backends.cudnn.deterministic
 _flag_cudnn_benchmark = torch.backends.cudnn.benchmark
 NP_MAX = np.iinfo(np.uint32).max
 MAX_SEED = NP_MAX + 1  # 2**32, the actual seed should be in [0, MAX_SEED - 1] for uint32
@@ -719,7 +723,80 @@
             if key in mapping:
                 if os.environ.get("MONAI_FAIL_ON_DUPLICATE_CONFIG", "0") == "1":
                     raise ValueError(f"Duplicate key: `{key}`")
                 else:
                     warnings.warn(f"Duplicate key: `{key}`")
             mapping.add(key)
         return super().construct_mapping(node, deep)
+
+
+class ConvertUnits:
+    """
+    Convert the values from input unit to the target unit
+
+    Args:
+        input_unit: the unit of the input quantity
+        target_unit: the unit of the target quantity
+
+    """
+
+    imperial_unit_of_length = {"inch": 0.0254, "foot": 0.3048, "yard": 0.9144, "mile": 1609.344}
+
+    unit_prefix = {
+        "peta": 15,
+        "tera": 12,
+        "giga": 9,
+        "mega": 6,
+        "kilo": 3,
+        "hecto": 2,
+        "deca": 1,
+        "deci": -1,
+        "centi": -2,
+        "milli": -3,
+        "micro": -6,
+        "nano": -9,
+        "pico": -12,
+        "femto": -15,
+    }
+    base_units = ["meter", "byte", "bit"]
+
+    def __init__(self, input_unit: str, target_unit: str) -> None:
+        self.input_unit, input_base = self._get_valid_unit_and_base(input_unit)
+        self.target_unit, target_base = self._get_valid_unit_and_base(target_unit)
+        if input_base == target_base:
+            self.unit_base = input_base
+        else:
+            raise ValueError(
+                "Both input and target units should be from the same quantity. "
+                f"Input quantity is {input_base} while target quantity is {target_base}"
+            )
+        self._calculate_conversion_factor()
+
+    def _get_valid_unit_and_base(self, unit):
+        unit = str(unit).lower()
+        if unit in self.imperial_unit_of_length:
+            return unit, "meter"
+        for base_unit in self.base_units:
+            if unit.endswith(base_unit):
+                return unit, base_unit
+        raise ValueError(f"Currently, it only supports length conversion but `{unit}` is given.")
+
+    def _get_unit_power(self, unit):
+        """Calculate the power of the unit factor with respect to the base unit"""
+        if unit in self.imperial_unit_of_length:
+            return log10(self.imperial_unit_of_length[unit])
+
+        prefix = unit[: len(self.unit_base)]
+        if prefix == "":
+            return 1.0
+        return self.unit_prefix[prefix]
+
+    def _calculate_conversion_factor(self):
+        """Calculate unit conversion factor with respect to the input unit"""
+        if self.input_unit == self.target_unit:
+            return 1.0
+        input_power = self._get_unit_power(self.input_unit)
+        target_power = self._get_unit_power(self.target_unit)
+        self.conversion_factor = 10 ** (input_power - target_power)
+
+    def __call__(self, value: int | float) -> Any:
+        return float(value) * self.conversion_factor
```

### Comparing `monai-weekly-1.2.dev2315/monai/utils/module.py` & `monai-weekly-1.2.dev2316/monai/utils/module.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/utils/nvtx.py` & `monai-weekly-1.2.dev2316/monai/utils/nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/utils/profiling.py` & `monai-weekly-1.2.dev2316/monai/utils/profiling.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/utils/state_cacher.py` & `monai-weekly-1.2.dev2316/monai/utils/state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/utils/type_conversion.py` & `monai-weekly-1.2.dev2316/monai/utils/type_conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 # conversion map for types unsupported by torch.as_tensor
 UNSUPPORTED_TYPES = {np.dtype("uint16"): np.int32, np.dtype("uint32"): np.int64, np.dtype("uint64"): np.int64}
 
 
 def get_numpy_dtype_from_string(dtype: str) -> np.dtype:
     """Get a numpy dtype (e.g., `np.float32`) from its string (e.g., `"float32"`)."""
-    return np.empty([], dtype=dtype).dtype
+    return np.empty([], dtype=str(dtype).split(".")[-1]).dtype
 
 
 def get_torch_dtype_from_string(dtype: str) -> torch.dtype:
     """Get a torch dtype (e.g., `torch.float32`) from its string (e.g., `"float32"`)."""
     return dtype_numpy_to_torch(get_numpy_dtype_from_string(dtype))
```

### Comparing `monai-weekly-1.2.dev2315/monai/visualize/__init__.py` & `monai-weekly-1.2.dev2316/monai/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/visualize/class_activation_maps.py` & `monai-weekly-1.2.dev2316/monai/visualize/class_activation_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/visualize/gradient_based.py` & `monai-weekly-1.2.dev2316/monai/visualize/gradient_based.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/visualize/img2tensorboard.py` & `monai-weekly-1.2.dev2316/monai/visualize/img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/visualize/occlusion_sensitivity.py` & `monai-weekly-1.2.dev2316/monai/visualize/occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/visualize/utils.py` & `monai-weekly-1.2.dev2316/monai/visualize/utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai/visualize/visualizer.py` & `monai-weekly-1.2.dev2316/monai/visualize/visualizer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/monai_weekly.egg-info/PKG-INFO` & `monai-weekly-1.2.dev2316/monai_weekly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monai-weekly
-Version: 1.2.dev2315
+Version: 1.2.dev2316
 Summary: AI Toolkit for Healthcare Imaging
 Home-page: https://monai.io/
 Author: MONAI Consortium
 Author-email: monai.contact@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.monai.io/
 Project-URL: Bug Tracker, https://github.com/Project-MONAI/MONAI/issues
```

### Comparing `monai-weekly-1.2.dev2315/monai_weekly.egg-info/SOURCES.txt` & `monai-weekly-1.2.dev2316/monai_weekly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -246,14 +246,15 @@
 monai/networks/blocks/localnet_block.py
 monai/networks/blocks/mlp.py
 monai/networks/blocks/patchembedding.py
 monai/networks/blocks/regunet_block.py
 monai/networks/blocks/segresnet_block.py
 monai/networks/blocks/selfattention.py
 monai/networks/blocks/squeeze_and_excitation.py
+monai/networks/blocks/text_embedding.py
 monai/networks/blocks/transformerblock.py
 monai/networks/blocks/unetr_block.py
 monai/networks/blocks/upsample.py
 monai/networks/blocks/warp.py
 monai/networks/layers/__init__.py
 monai/networks/layers/convutils.py
 monai/networks/layers/drop_path.py
@@ -999,14 +1000,15 @@
 tests/test_subpixel_upsample.py
 tests/test_surface_dice.py
 tests/test_surface_distance.py
 tests/test_swin_unetr.py
 tests/test_synthetic.py
 tests/test_tciadataset.py
 tests/test_testtimeaugmentation.py
+tests/test_text_encoding.py
 tests/test_thread_buffer.py
 tests/test_threadcontainer.py
 tests/test_threshold_intensity.py
 tests/test_threshold_intensityd.py
 tests/test_timedcall_dist.py
 tests/test_to_contiguous.py
 tests/test_to_cupy.py
```

### Comparing `monai-weekly-1.2.dev2315/monai_weekly.egg-info/requires.txt` & `monai-weekly-1.2.dev2316/monai_weekly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/pyproject.toml` & `monai-weekly-1.2.dev2316/pyproject.toml`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/setup.cfg` & `monai-weekly-1.2.dev2316/setup.cfg`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/setup.py` & `monai-weekly-1.2.dev2316/setup.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_acn_block.py` & `monai-weekly-1.2.dev2316/tests/test_acn_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_activations.py` & `monai-weekly-1.2.dev2316/tests/test_activations.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_activationsd.py` & `monai-weekly-1.2.dev2316/tests/test_activationsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_adaptors.py` & `monai-weekly-1.2.dev2316/tests/test_adaptors.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_add_channeld.py` & `monai-weekly-1.2.dev2316/tests/test_add_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_add_coordinate_channels.py` & `monai-weekly-1.2.dev2316/tests/test_add_coordinate_channels.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_add_coordinate_channelsd.py` & `monai-weekly-1.2.dev2316/tests/test_add_coordinate_channelsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_add_extreme_points_channel.py` & `monai-weekly-1.2.dev2316/tests/test_add_extreme_points_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_add_extreme_points_channeld.py` & `monai-weekly-1.2.dev2316/tests/test_add_extreme_points_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_adjust_contrast.py` & `monai-weekly-1.2.dev2316/tests/test_adjust_contrast.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_adjust_contrastd.py` & `monai-weekly-1.2.dev2316/tests/test_adjust_contrastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_adn.py` & `monai-weekly-1.2.dev2316/tests/test_adn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_affine.py` & `monai-weekly-1.2.dev2316/tests/test_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_affine_grid.py` & `monai-weekly-1.2.dev2316/tests/test_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_affine_transform.py` & `monai-weekly-1.2.dev2316/tests/test_affine_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_affined.py` & `monai-weekly-1.2.dev2316/tests/test_affined.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_ahnet.py` & `monai-weekly-1.2.dev2316/tests/test_ahnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_alias.py` & `monai-weekly-1.2.dev2316/tests/test_alias.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_anchor_box.py` & `monai-weekly-1.2.dev2316/tests/test_anchor_box.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_apply.py` & `monai-weekly-1.2.dev2316/tests/test_apply.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_apply_filter.py` & `monai-weekly-1.2.dev2316/tests/test_apply_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_arraydataset.py` & `monai-weekly-1.2.dev2316/tests/test_arraydataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_as_channel_first.py` & `monai-weekly-1.2.dev2316/tests/test_as_channel_first.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_as_channel_firstd.py` & `monai-weekly-1.2.dev2316/tests/test_as_channel_firstd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_as_channel_last.py` & `monai-weekly-1.2.dev2316/tests/test_as_channel_last.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_as_channel_lastd.py` & `monai-weekly-1.2.dev2316/tests/test_as_channel_lastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_as_discrete.py` & `monai-weekly-1.2.dev2316/tests/test_as_discrete.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_as_discreted.py` & `monai-weekly-1.2.dev2316/tests/test_as_discreted.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_atss_box_matcher.py` & `monai-weekly-1.2.dev2316/tests/test_atss_box_matcher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_attentionunet.py` & `monai-weekly-1.2.dev2316/tests/test_attentionunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_auto3dseg.py` & `monai-weekly-1.2.dev2316/tests/test_auto3dseg.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_auto3dseg_ensemble.py` & `monai-weekly-1.2.dev2316/tests/test_auto3dseg_hpo.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,33 +10,55 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import os
 import tempfile
 import unittest
+from functools import partial
 
 import nibabel as nib
 import numpy as np
 import torch
 
-from monai.apps.auto3dseg import AlgoEnsembleBestByFold, AlgoEnsembleBestN, AlgoEnsembleBuilder, BundleGen, DataAnalyzer
+from monai.apps.auto3dseg import BundleGen, DataAnalyzer, NNIGen, OptunaGen, import_bundle_algo_history
 from monai.bundle.config_parser import ConfigParser
 from monai.data import create_test_image_3d
-from monai.utils import optional_import, set_determinism
-from monai.utils.enums import AlgoEnsembleKeys
+from monai.utils import optional_import
+from monai.utils.enums import AlgoKeys
 from tests.utils import (
     SkipIfBeforePyTorchVersion,
     get_testing_algo_template_path,
     skip_if_downloading_fails,
     skip_if_no_cuda,
-    skip_if_quick,
 )
 
 _, has_tb = optional_import("torch.utils.tensorboard", name="SummaryWriter")
+optuna, has_optuna = optional_import("optuna")
+
+override_param = (
+    {
+        "num_images_per_batch": 2,
+        "num_epochs": 2,
+        "num_epochs_per_validation": 1,
+        "num_warmup_epochs": 1,
+        "use_pretrain": False,
+        "pretrained_path": "",
+    }
+    if torch.cuda.is_available()
+    else {}
+)
+
+
+def skip_if_no_optuna(obj):
+    """
+    Skip the unit tests if torch.cuda.is_available is False.
+    """
+    return unittest.skipUnless(has_optuna, "Skipping optuna tests")(obj)
+
 
 fake_datalist: dict[str, list[dict]] = {
     "testing": [{"image": "val_001.fake.nii.gz"}, {"image": "val_002.fake.nii.gz"}],
     "training": [
         {"fold": 0, "image": "tr_image_001.fake.nii.gz", "label": "tr_label_001.fake.nii.gz"},
         {"fold": 0, "image": "tr_image_002.fake.nii.gz", "label": "tr_label_002.fake.nii.gz"},
         {"fold": 0, "image": "tr_image_003.fake.nii.gz", "label": "tr_label_003.fake.nii.gz"},
@@ -48,45 +70,24 @@
         {"fold": 2, "image": "tr_image_009.fake.nii.gz", "label": "tr_label_009.fake.nii.gz"},
         {"fold": 2, "image": "tr_image_010.fake.nii.gz", "label": "tr_label_010.fake.nii.gz"},
         {"fold": 2, "image": "tr_image_011.fake.nii.gz", "label": "tr_label_011.fake.nii.gz"},
         {"fold": 2, "image": "tr_image_012.fake.nii.gz", "label": "tr_label_012.fake.nii.gz"},
     ],
 }
 
-train_param = (
-    {
-        "num_images_per_batch": 2,
-        "num_epochs": 2,
-        "num_epochs_per_validation": 1,
-        "num_warmup_epochs": 1,
-        "use_pretrain": False,
-        "pretrained_path": "",
-        "determ": True,
-    }
-    if torch.cuda.is_available()
-    else {}
-)
-
-pred_param = {"files_slices": slice(0, 1), "mode": "mean", "sigmoid": True}
-
 
-@skip_if_quick
 @SkipIfBeforePyTorchVersion((1, 9, 1))
 @unittest.skipIf(not has_tb, "no tensorboard summary writer")
-class TestEnsembleBuilder(unittest.TestCase):
+class TestHPO(unittest.TestCase):
     def setUp(self) -> None:
-        set_determinism(0)
         self.test_dir = tempfile.TemporaryDirectory()
-
-    @skip_if_no_cuda
-    def test_ensemble(self) -> None:
         test_path = self.test_dir.name
 
-        dataroot = os.path.join(test_path, "dataroot")
-        work_dir = os.path.join(test_path, "workdir")
+        work_dir = os.path.abspath(os.path.join(test_path, "workdir"))
+        dataroot = os.path.join(work_dir, "dataroot")
 
         da_output_yaml = os.path.join(work_dir, "datastats.yaml")
         data_src_cfg = os.path.join(work_dir, "data_src_cfg.yaml")
 
         if not os.path.isdir(dataroot):
             os.makedirs(dataroot)
 
@@ -119,52 +120,70 @@
             "datalist": fake_json_datalist,
             "dataroot": dataroot,
             "multigpu": False,
             "class_names": ["label_class"],
         }
 
         ConfigParser.export_config_file(data_src, data_src_cfg)
-
         with skip_if_downloading_fails():
             bundle_generator = BundleGen(
                 algo_path=work_dir,
                 data_stats_filename=da_output_yaml,
                 data_src_cfg_name=data_src_cfg,
                 templates_path_or_url=get_testing_algo_template_path(),
             )
         bundle_generator.generate(work_dir, num_fold=1)
-        history = bundle_generator.get_history()
 
-        for algo_dict in history:
-            name = algo_dict[AlgoEnsembleKeys.ID]
-            algo = algo_dict[AlgoEnsembleKeys.ALGO]
-            _train_param = train_param.copy()
-            if name.startswith("segresnet"):
-                _train_param["network#init_filters"] = 8
-                _train_param["pretrained_ckpt_name"] = ""
-            elif name.startswith("swinunetr"):
-                _train_param["network#feature_size"] = 12
-            algo.train(_train_param)
-
-        builder = AlgoEnsembleBuilder(history, data_src_cfg)
-        builder.set_ensemble_method(AlgoEnsembleBestN(n_best=1))
-        ensemble = builder.get_ensemble()
-        name = ensemble.get_algo_ensemble()[0][AlgoEnsembleKeys.ID]
-        if name.startswith("segresnet"):
-            pred_param["network#init_filters"] = 8
-        elif name.startswith("swinunetr"):
-            pred_param["network#feature_size"] = 12
-        preds = ensemble(pred_param)
-        self.assertTupleEqual(preds[0].shape, (2, 24, 24, 24))
-
-        builder.set_ensemble_method(AlgoEnsembleBestByFold(1))
-        ensemble = builder.get_ensemble()
-        for algo in ensemble.get_algo_ensemble():
-            print(algo[AlgoEnsembleKeys.ID])
+        self.history = bundle_generator.get_history()
+        self.work_dir = work_dir
+        self.test_path = test_path
+
+    @skip_if_no_cuda
+    def test_run_algo(self) -> None:
+        algo_dict = self.history[-1]
+        algo = algo_dict[AlgoKeys.ALGO]
+        nni_gen = NNIGen(algo=algo, params=override_param)
+        obj_filename = nni_gen.get_obj_filename()
+        # this function will be used in HPO via Python Fire
+        NNIGen().run_algo(obj_filename, self.work_dir)
+
+    @skip_if_no_cuda
+    @skip_if_no_optuna
+    def test_run_optuna(self) -> None:
+        algo_dict = self.history[-1]
+        algo = algo_dict[AlgoKeys.ALGO]
+
+        class OptunaGenLearningRate(OptunaGen):
+            def get_hyperparameters(self):
+                return {"learning_rate": self.trial.suggest_float("learning_rate", 0.00001, 0.1)}
+
+        optuna_gen = OptunaGenLearningRate(algo=algo, params=override_param)
+        search_space = {"learning_rate": [0.0001, 0.001, 0.01, 0.1]}
+        study = optuna.create_study(sampler=optuna.samplers.GridSampler(search_space), direction="maximize")
+        study.optimize(
+            partial(
+                optuna_gen,
+                obj_filename=optuna_gen.get_obj_filename(),
+                output_folder=os.path.join(self.test_path, "optuna_test"),
+            ),
+            n_trials=2,
+        )
+        print(f"Best value: {study.best_value} (params: {study.best_params})\n")
+
+    @skip_if_no_cuda
+    def test_get_history(self) -> None:
+        algo_dict = self.history[-1]
+        algo = algo_dict[AlgoKeys.ALGO]
+        nni_gen = NNIGen(algo=algo, params=override_param)
+        obj_filename = nni_gen.get_obj_filename()
+
+        NNIGen().run_algo(obj_filename, self.work_dir)
+
+        history = import_bundle_algo_history(self.work_dir, only_trained=True)
+        assert len(history) == 1
 
     def tearDown(self) -> None:
-        set_determinism(None)
         self.test_dir.cleanup()
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_autoencoder.py` & `monai-weekly-1.2.dev2316/tests/test_autoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_avg_merger.py` & `monai-weekly-1.2.dev2316/tests/test_avg_merger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_basic_unet.py` & `monai-weekly-1.2.dev2316/tests/test_basic_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_basic_unetplusplus.py` & `monai-weekly-1.2.dev2316/tests/test_basic_unetplusplus.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_bending_energy.py` & `monai-weekly-1.2.dev2316/tests/test_bending_energy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_bilateral_approx_cpu.py` & `monai-weekly-1.2.dev2316/tests/test_bilateral_approx_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_bilateral_approx_cuda.py` & `monai-weekly-1.2.dev2316/tests/test_bilateral_approx_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_bilateral_precise.py` & `monai-weekly-1.2.dev2316/tests/test_bilateral_precise.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import numpy as np
 import torch
 from parameterized import parameterized
 from torch.autograd import gradcheck
 
 from monai.networks.layers.filtering import BilateralFilter
-from tests.utils import skip_if_no_cpp_extension, skip_if_no_cuda
+from tests.utils import skip_if_no_cpp_extension, skip_if_no_cuda, skip_if_quick
 
 TEST_CASES = [
     [
         # Case Description
         "1 dimension, 1 channel, low spatial sigma, low color sigma",
         # Spatial and Color Sigmas
         (1, 0.2),
@@ -360,14 +360,15 @@
             ]
         ],
     ],
 ]
 
 
 @skip_if_no_cpp_extension
+@skip_if_quick
 class BilateralFilterTestCaseCpuPrecise(unittest.TestCase):
     @parameterized.expand(TEST_CASES)
     def test_cpu_precise(self, test_case_description, sigmas, input, expected):
         # Params to determine the implementation to test
         device = torch.device("cpu")
         fast_approx = False
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_blend_images.py` & `monai-weekly-1.2.dev2316/tests/test_blend_images.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_border_pad.py` & `monai-weekly-1.2.dev2316/tests/test_border_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_border_padd.py` & `monai-weekly-1.2.dev2316/tests/test_border_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_bounding_rect.py` & `monai-weekly-1.2.dev2316/tests/test_bounding_rect.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_bounding_rectd.py` & `monai-weekly-1.2.dev2316/tests/test_bounding_rectd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_box_coder.py` & `monai-weekly-1.2.dev2316/tests/test_box_coder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_box_transform.py` & `monai-weekly-1.2.dev2316/tests/test_box_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_box_utils.py` & `monai-weekly-1.2.dev2316/tests/test_box_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_bundle_ckpt_export.py` & `monai-weekly-1.2.dev2316/tests/test_bundle_ckpt_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_bundle_download.py` & `monai-weekly-1.2.dev2316/tests/test_bundle_download.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_bundle_get_data.py` & `monai-weekly-1.2.dev2316/tests/test_bundle_get_data.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_bundle_init_bundle.py` & `monai-weekly-1.2.dev2316/tests/test_bundle_init_bundle.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_bundle_onnx_export.py` & `monai-weekly-1.2.dev2316/tests/test_bundle_onnx_export.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_bundle_utils.py` & `monai-weekly-1.2.dev2316/tests/test_bundle_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_bundle_verify_metadata.py` & `monai-weekly-1.2.dev2316/tests/test_bundle_verify_metadata.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_bundle_verify_net.py` & `monai-weekly-1.2.dev2316/tests/test_bundle_verify_net.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_bundle_workflow.py` & `monai-weekly-1.2.dev2316/tests/test_bundle_workflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_cachedataset.py` & `monai-weekly-1.2.dev2316/tests/test_cachedataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_cachedataset_parallel.py` & `monai-weekly-1.2.dev2316/tests/test_cachedataset_parallel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_cachedataset_persistent_workers.py` & `monai-weekly-1.2.dev2316/tests/test_cachedataset_persistent_workers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_cachentransdataset.py` & `monai-weekly-1.2.dev2316/tests/test_cachentransdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_call_dist.py` & `monai-weekly-1.2.dev2316/tests/test_call_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_cast_to_type.py` & `monai-weekly-1.2.dev2316/tests/test_cast_to_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_cast_to_typed.py` & `monai-weekly-1.2.dev2316/tests/test_cast_to_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_center_scale_crop.py` & `monai-weekly-1.2.dev2316/tests/test_center_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_center_scale_cropd.py` & `monai-weekly-1.2.dev2316/tests/test_center_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_center_spatial_crop.py` & `monai-weekly-1.2.dev2316/tests/test_center_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_center_spatial_cropd.py` & `monai-weekly-1.2.dev2316/tests/test_center_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_channel_pad.py` & `monai-weekly-1.2.dev2316/tests/test_channel_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_check_hash.py` & `monai-weekly-1.2.dev2316/tests/test_check_hash.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_check_missing_files.py` & `monai-weekly-1.2.dev2316/tests/test_check_missing_files.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_classes_to_indices.py` & `monai-weekly-1.2.dev2316/tests/test_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_classes_to_indicesd.py` & `monai-weekly-1.2.dev2316/tests/test_classes_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_complex_utils.py` & `monai-weekly-1.2.dev2316/tests/test_complex_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_component_locator.py` & `monai-weekly-1.2.dev2316/tests/test_component_locator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_compose.py` & `monai-weekly-1.2.dev2316/tests/test_compose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_compose_get_number_conversions.py` & `monai-weekly-1.2.dev2316/tests/test_compose_get_number_conversions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_compute_confusion_matrix.py` & `monai-weekly-1.2.dev2316/tests/test_compute_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_compute_f_beta.py` & `monai-weekly-1.2.dev2316/tests/test_compute_f_beta.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_compute_froc.py` & `monai-weekly-1.2.dev2316/tests/test_compute_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_compute_generalized_dice.py` & `monai-weekly-1.2.dev2316/tests/test_compute_generalized_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_compute_ho_ver_maps.py` & `monai-weekly-1.2.dev2316/tests/test_compute_ho_ver_maps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_compute_ho_ver_maps_d.py` & `monai-weekly-1.2.dev2316/tests/test_compute_ho_ver_maps_d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_compute_meandice.py` & `monai-weekly-1.2.dev2316/tests/test_compute_meandice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_compute_meaniou.py` & `monai-weekly-1.2.dev2316/tests/test_compute_meaniou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_compute_panoptic_quality.py` & `monai-weekly-1.2.dev2316/tests/test_compute_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_compute_regression_metrics.py` & `monai-weekly-1.2.dev2316/tests/test_compute_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_compute_roc_auc.py` & `monai-weekly-1.2.dev2316/tests/test_compute_roc_auc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_compute_variance.py` & `monai-weekly-1.2.dev2316/tests/test_compute_variance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_concat_itemsd.py` & `monai-weekly-1.2.dev2316/tests/test_concat_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_config_item.py` & `monai-weekly-1.2.dev2316/tests/test_config_item.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_config_parser.py` & `monai-weekly-1.2.dev2316/tests/test_config_parser.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_contrastive_loss.py` & `monai-weekly-1.2.dev2316/tests/test_contrastive_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_convert_data_type.py` & `monai-weekly-1.2.dev2316/tests/test_convert_data_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_convert_to_multi_channel.py` & `monai-weekly-1.2.dev2316/tests/test_convert_to_multi_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_convert_to_multi_channeld.py` & `monai-weekly-1.2.dev2316/tests/test_convert_to_multi_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_convert_to_onnx.py` & `monai-weekly-1.2.dev2316/tests/test_convert_to_onnx.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,28 +16,29 @@
 
 import torch
 from parameterized import parameterized
 
 from monai.networks import convert_to_onnx
 from monai.networks.nets import SegResNet, UNet
 from monai.utils.module import pytorch_after
-from tests.utils import SkipIfBeforePyTorchVersion, SkipIfNoModule, optional_import
+from tests.utils import SkipIfBeforePyTorchVersion, SkipIfNoModule, optional_import, skip_if_quick
 
 if torch.cuda.is_available():
     TORCH_DEVICE_OPTIONS = ["cpu", "cuda"]
 else:
     TORCH_DEVICE_OPTIONS = ["cpu"]
 TESTS = list(itertools.product(TORCH_DEVICE_OPTIONS, [True, False], [True, False]))
 TESTS_ORT = list(itertools.product(TORCH_DEVICE_OPTIONS, [True]))
 
 onnx, _ = optional_import("onnx")
 
 
 @SkipIfNoModule("onnx")
 @SkipIfBeforePyTorchVersion((1, 9))
+@skip_if_quick
 class TestConvertToOnnx(unittest.TestCase):
     @parameterized.expand(TESTS)
     def test_unet(self, device, use_trace, use_ort):
         if use_ort:
             _, has_onnxruntime = optional_import("onnxruntime")
             if not has_onnxruntime:
                 self.skipTest("onnxruntime is not installed probably due to python version >= 3.11.")
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_convert_to_torchscript.py` & `monai-weekly-1.2.dev2316/tests/test_convert_to_torchscript.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_convert_to_trt.py` & `monai-weekly-1.2.dev2316/tests/test_convert_to_trt.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_convolutions.py` & `monai-weekly-1.2.dev2316/tests/test_convolutions.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_copy_itemsd.py` & `monai-weekly-1.2.dev2316/tests/test_copy_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_copy_model_state.py` & `monai-weekly-1.2.dev2316/tests/test_copy_model_state.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_correct_crop_centers.py` & `monai-weekly-1.2.dev2316/tests/test_correct_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_create_cross_validation_datalist.py` & `monai-weekly-1.2.dev2316/tests/test_create_cross_validation_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_create_grid_and_affine.py` & `monai-weekly-1.2.dev2316/tests/test_create_grid_and_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_crf_cpu.py` & `monai-weekly-1.2.dev2316/tests/test_crf_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_crf_cuda.py` & `monai-weekly-1.2.dev2316/tests/test_crf_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_crop_foreground.py` & `monai-weekly-1.2.dev2316/tests/test_crop_foreground.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_crop_foregroundd.py` & `monai-weekly-1.2.dev2316/tests/test_crop_foregroundd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_cross_validation.py` & `monai-weekly-1.2.dev2316/tests/test_cross_validation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_csv_dataset.py` & `monai-weekly-1.2.dev2316/tests/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_csv_iterable_dataset.py` & `monai-weekly-1.2.dev2316/tests/test_csv_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_csv_saver.py` & `monai-weekly-1.2.dev2316/tests/test_csv_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_cucim_dict_transform.py` & `monai-weekly-1.2.dev2316/tests/test_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_cucim_transform.py` & `monai-weekly-1.2.dev2316/tests/test_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_cumulative.py` & `monai-weekly-1.2.dev2316/tests/test_cumulative.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_cumulative_average.py` & `monai-weekly-1.2.dev2316/tests/test_cumulative_average.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_cumulative_average_dist.py` & `monai-weekly-1.2.dev2316/tests/test_cumulative_average_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_cv2_dist.py` & `monai-weekly-1.2.dev2316/tests/test_cv2_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_data_stats.py` & `monai-weekly-1.2.dev2316/tests/test_data_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_data_statsd.py` & `monai-weekly-1.2.dev2316/tests/test_data_statsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_dataloader.py` & `monai-weekly-1.2.dev2316/tests/test_dataloader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_dataset.py` & `monai-weekly-1.2.dev2316/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_dataset_func.py` & `monai-weekly-1.2.dev2316/tests/test_dataset_func.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_dataset_summary.py` & `monai-weekly-1.2.dev2316/tests/test_dataset_summary.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_decathlondataset.py` & `monai-weekly-1.2.dev2316/tests/test_decathlondataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_decollate.py` & `monai-weekly-1.2.dev2316/tests/test_decollate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_deepedit_interaction.py` & `monai-weekly-1.2.dev2316/tests/test_deepedit_interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_deepedit_transforms.py` & `monai-weekly-1.2.dev2316/tests/test_deepedit_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_deepgrow_dataset.py` & `monai-weekly-1.2.dev2316/tests/test_deepgrow_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_deepgrow_interaction.py` & `monai-weekly-1.2.dev2316/tests/test_deepgrow_interaction.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_deepgrow_transforms.py` & `monai-weekly-1.2.dev2316/tests/test_deepgrow_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_delete_itemsd.py` & `monai-weekly-1.2.dev2316/tests/test_delete_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_denseblock.py` & `monai-weekly-1.2.dev2316/tests/test_denseblock.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_densenet.py` & `monai-weekly-1.2.dev2316/tests/test_densenet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_deprecated.py` & `monai-weekly-1.2.dev2316/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_detect_envelope.py` & `monai-weekly-1.2.dev2316/tests/test_detect_envelope.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_detection_coco_metrics.py` & `monai-weekly-1.2.dev2316/tests/test_detection_coco_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_detector_boxselector.py` & `monai-weekly-1.2.dev2316/tests/test_detector_boxselector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_detector_utils.py` & `monai-weekly-1.2.dev2316/tests/test_detector_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_dev_collate.py` & `monai-weekly-1.2.dev2316/tests/test_dev_collate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_dice_ce_loss.py` & `monai-weekly-1.2.dev2316/tests/test_dice_ce_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_dice_focal_loss.py` & `monai-weekly-1.2.dev2316/tests/test_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_dice_loss.py` & `monai-weekly-1.2.dev2316/tests/test_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_dints_cell.py` & `monai-weekly-1.2.dev2316/tests/test_dints_cell.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_dints_mixop.py` & `monai-weekly-1.2.dev2316/tests/test_dints_mixop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_dints_network.py` & `monai-weekly-1.2.dev2316/tests/test_dints_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import numpy as np
 import torch
 from parameterized import parameterized
 
 from monai.networks.nets import DiNTS, TopologyInstance, TopologySearch
 from monai.networks.nets.dints import Cell
-from tests.utils import SkipIfBeforePyTorchVersion, test_script_save
+from tests.utils import SkipIfBeforePyTorchVersion, skip_if_quick, test_script_save
 
 TEST_CASES_3D = [
     [
         {
             "channel_mul": 0.2,
             "num_blocks": 6,
             "num_depths": 3,
@@ -109,14 +109,15 @@
             },
             (2, 1, 32, 16),
             (2, 4, 32, 16),
         ]
     ]
 
 
+@skip_if_quick
 class TestDints(unittest.TestCase):
     @parameterized.expand(TEST_CASES_3D + TEST_CASES_2D)
     def test_dints_inference(self, dints_grid_params, dints_params, input_shape, expected_shape):
         grid = TopologySearch(**dints_grid_params)
         dints_params["dints_space"] = grid
         net = DiNTS(**dints_params).to(dints_grid_params["device"])
         result = net(torch.randn(input_shape).to(dints_grid_params["device"]))
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_discriminator.py` & `monai-weekly-1.2.dev2316/tests/test_discriminator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_divisible_pad.py` & `monai-weekly-1.2.dev2316/tests/test_divisible_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_divisible_padd.py` & `monai-weekly-1.2.dev2316/tests/test_divisible_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_download_and_extract.py` & `monai-weekly-1.2.dev2316/tests/test_download_and_extract.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_downsample_block.py` & `monai-weekly-1.2.dev2316/tests/test_downsample_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_drop_path.py` & `monai-weekly-1.2.dev2316/tests/test_drop_path.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_ds_loss.py` & `monai-weekly-1.2.dev2316/tests/test_ds_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_dvf2ddf.py` & `monai-weekly-1.2.dev2316/tests/test_dvf2ddf.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_dynunet.py` & `monai-weekly-1.2.dev2316/tests/test_dynunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_dynunet_block.py` & `monai-weekly-1.2.dev2316/tests/test_dynunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_efficientnet.py` & `monai-weekly-1.2.dev2316/tests/test_efficientnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_ensemble_evaluator.py` & `monai-weekly-1.2.dev2316/tests/test_ensemble_evaluator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_ensure_channel_first.py` & `monai-weekly-1.2.dev2316/tests/test_ensure_channel_first.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_ensure_channel_firstd.py` & `monai-weekly-1.2.dev2316/tests/test_ensure_channel_firstd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_ensure_tuple.py` & `monai-weekly-1.2.dev2316/tests/test_ensure_tuple.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_ensure_type.py` & `monai-weekly-1.2.dev2316/tests/test_ensure_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_ensure_typed.py` & `monai-weekly-1.2.dev2316/tests/test_ensure_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_enum_bound_interp.py` & `monai-weekly-1.2.dev2316/tests/test_enum_bound_interp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_eval_mode.py` & `monai-weekly-1.2.dev2316/tests/test_eval_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_evenly_divisible_all_gather_dist.py` & `monai-weekly-1.2.dev2316/tests/test_evenly_divisible_all_gather_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_factorized_increase.py` & `monai-weekly-1.2.dev2316/tests/test_factorized_increase.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_factorized_reduce.py` & `monai-weekly-1.2.dev2316/tests/test_factorized_reduce.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_fastmri_reader.py` & `monai-weekly-1.2.dev2316/tests/test_fastmri_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_fft_utils.py` & `monai-weekly-1.2.dev2316/tests/test_fft_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_fg_bg_to_indices.py` & `monai-weekly-1.2.dev2316/tests/test_fg_bg_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_fg_bg_to_indicesd.py` & `monai-weekly-1.2.dev2316/tests/test_fg_bg_to_indicesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_file_basename.py` & `monai-weekly-1.2.dev2316/tests/test_file_basename.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_fill_holes.py` & `monai-weekly-1.2.dev2316/tests/test_fill_holes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_fill_holesd.py` & `monai-weekly-1.2.dev2316/tests/test_fill_holesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_fl_exchange_object.py` & `monai-weekly-1.2.dev2316/tests/test_fl_exchange_object.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_fl_monai_algo.py` & `monai-weekly-1.2.dev2316/tests/test_fl_monai_algo.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_fl_monai_algo_dist.py` & `monai-weekly-1.2.dev2316/tests/test_fl_monai_algo_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_fl_monai_algo_stats.py` & `monai-weekly-1.2.dev2316/tests/test_fl_monai_algo_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_flatten_sub_keysd.py` & `monai-weekly-1.2.dev2316/tests/test_flatten_sub_keysd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_flexible_unet.py` & `monai-weekly-1.2.dev2316/tests/test_flexible_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_flip.py` & `monai-weekly-1.2.dev2316/tests/test_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_flipd.py` & `monai-weekly-1.2.dev2316/tests/test_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_focal_loss.py` & `monai-weekly-1.2.dev2316/tests/test_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_folder_layout.py` & `monai-weekly-1.2.dev2316/tests/test_folder_layout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_foreground_mask.py` & `monai-weekly-1.2.dev2316/tests/test_foreground_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_foreground_maskd.py` & `monai-weekly-1.2.dev2316/tests/test_foreground_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_fourier.py` & `monai-weekly-1.2.dev2316/tests/test_fourier.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_fpn_block.py` & `monai-weekly-1.2.dev2316/tests/test_fpn_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_from_engine_hovernet.py` & `monai-weekly-1.2.dev2316/tests/test_from_engine_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_fullyconnectednet.py` & `monai-weekly-1.2.dev2316/tests/test_fullyconnectednet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_gaussian.py` & `monai-weekly-1.2.dev2316/tests/test_gaussian.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_gaussian_filter.py` & `monai-weekly-1.2.dev2316/tests/test_gaussian_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_gaussian_sharpen.py` & `monai-weekly-1.2.dev2316/tests/test_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_gaussian_sharpend.py` & `monai-weekly-1.2.dev2316/tests/test_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_gaussian_smooth.py` & `monai-weekly-1.2.dev2316/tests/test_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_gaussian_smoothd.py` & `monai-weekly-1.2.dev2316/tests/test_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generalized_dice_focal_loss.py` & `monai-weekly-1.2.dev2316/tests/test_generalized_dice_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generalized_dice_loss.py` & `monai-weekly-1.2.dev2316/tests/test_generalized_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generalized_wasserstein_dice_loss.py` & `monai-weekly-1.2.dev2316/tests/test_generalized_wasserstein_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generate_distance_map.py` & `monai-weekly-1.2.dev2316/tests/test_generate_distance_map.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generate_distance_mapd.py` & `monai-weekly-1.2.dev2316/tests/test_generate_distance_mapd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generate_instance_border.py` & `monai-weekly-1.2.dev2316/tests/test_generate_instance_border.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generate_instance_borderd.py` & `monai-weekly-1.2.dev2316/tests/test_generate_instance_borderd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generate_instance_centroid.py` & `monai-weekly-1.2.dev2316/tests/test_generate_instance_centroid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generate_instance_centroidd.py` & `monai-weekly-1.2.dev2316/tests/test_generate_instance_centroidd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generate_instance_contour.py` & `monai-weekly-1.2.dev2316/tests/test_generate_instance_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generate_instance_contourd.py` & `monai-weekly-1.2.dev2316/tests/test_generate_instance_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generate_instance_type.py` & `monai-weekly-1.2.dev2316/tests/test_generate_instance_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generate_instance_typed.py` & `monai-weekly-1.2.dev2316/tests/test_generate_instance_typed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generate_label_classes_crop_centers.py` & `monai-weekly-1.2.dev2316/tests/test_generate_label_classes_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generate_param_groups.py` & `monai-weekly-1.2.dev2316/tests/test_generate_param_groups.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generate_pos_neg_label_crop_centers.py` & `monai-weekly-1.2.dev2316/tests/test_generate_pos_neg_label_crop_centers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generate_spatial_bounding_box.py` & `monai-weekly-1.2.dev2316/tests/test_generate_spatial_bounding_box.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generate_succinct_contour.py` & `monai-weekly-1.2.dev2316/tests/test_generate_succinct_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generate_succinct_contourd.py` & `monai-weekly-1.2.dev2316/tests/test_generate_succinct_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generate_watershed_markers.py` & `monai-weekly-1.2.dev2316/tests/test_generate_watershed_markers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generate_watershed_markersd.py` & `monai-weekly-1.2.dev2316/tests/test_generate_watershed_markersd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generate_watershed_mask.py` & `monai-weekly-1.2.dev2316/tests/test_generate_watershed_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generate_watershed_maskd.py` & `monai-weekly-1.2.dev2316/tests/test_generate_watershed_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_generator.py` & `monai-weekly-1.2.dev2316/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_get_equivalent_dtype.py` & `monai-weekly-1.2.dev2316/tests/test_get_equivalent_dtype.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,15 +38,23 @@
         """the get_equivalent_dtype currently doesn't change the build-in type"""
         n_type = [float, int, bool]
         for n in n_type:
             for im_dtype in DTYPES:
                 out_dtype = get_equivalent_dtype(n, type(im_dtype))
                 self.assertEqual(out_dtype, n)
 
-    @parameterized.expand([["float", np.float64], ["float32", np.float32], ["float64", np.float64]])
+    @parameterized.expand(
+        [
+            ["float", np.float64],
+            ["float32", np.float32],
+            ["np.float32", np.float32],
+            ["float64", np.float64],
+            ["torch.float64", np.float64],
+        ]
+    )
     def test_from_string(self, dtype_str, expected_np):
         expected_pt = get_equivalent_dtype(expected_np, torch.Tensor)
         # numpy
         dtype = get_numpy_dtype_from_string(dtype_str)
         self.assertEqual(dtype, expected_np)
         # torch
         dtype = get_torch_dtype_from_string(dtype_str)
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_get_extreme_points.py` & `monai-weekly-1.2.dev2316/tests/test_get_extreme_points.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_get_layers.py` & `monai-weekly-1.2.dev2316/tests/test_get_layers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_get_package_version.py` & `monai-weekly-1.2.dev2316/tests/test_get_package_version.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_get_unique_labels.py` & `monai-weekly-1.2.dev2316/tests/test_get_unique_labels.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_gibbs_noise.py` & `monai-weekly-1.2.dev2316/tests/test_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_gibbs_noised.py` & `monai-weekly-1.2.dev2316/tests/test_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_giou_loss.py` & `monai-weekly-1.2.dev2316/tests/test_giou_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_global_mutual_information_loss.py` & `monai-weekly-1.2.dev2316/tests/test_global_mutual_information_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_globalnet.py` & `monai-weekly-1.2.dev2316/tests/test_globalnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_gmm.py` & `monai-weekly-1.2.dev2316/tests/test_gmm.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 import numpy as np
 import torch
 from parameterized import parameterized
 
 from monai._extensions import load_module
 from monai.networks.layers import GaussianMixtureModel
-from tests.utils import skip_if_darwin, skip_if_no_cuda, skip_if_windows
+from tests.utils import skip_if_darwin, skip_if_no_cuda, skip_if_quick, skip_if_windows
 
 TEST_CASES = [
     [
         # Case Description
         "2 batches, 1 dimensions, 1 channels, 2 classes, 2 mixtures",
         # Class Count
         2,
@@ -255,14 +255,15 @@
                 ],
             ]
         ],
     ],
 ]
 
 
+@skip_if_quick
 class GMMTestCase(unittest.TestCase):
     def setUp(self):
         self._var = os.environ.get("TORCH_EXTENSIONS_DIR")
         self.tempdir = tempfile.mkdtemp()
         os.environ["TORCH_EXTENSIONS_DIR"] = self.tempdir
 
     def tearDown(self) -> None:
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_grid_dataset.py` & `monai-weekly-1.2.dev2316/tests/test_grid_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_grid_distortion.py` & `monai-weekly-1.2.dev2316/tests/test_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_grid_distortiond.py` & `monai-weekly-1.2.dev2316/tests/test_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_grid_patch.py` & `monai-weekly-1.2.dev2316/tests/test_grid_patch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_grid_patchd.py` & `monai-weekly-1.2.dev2316/tests/test_grid_patchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_grid_pull.py` & `monai-weekly-1.2.dev2316/tests/test_grid_pull.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_grid_split.py` & `monai-weekly-1.2.dev2316/tests/test_grid_split.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_grid_splitd.py` & `monai-weekly-1.2.dev2316/tests/test_grid_splitd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_checkpoint_loader.py` & `monai-weekly-1.2.dev2316/tests/test_handler_checkpoint_loader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_checkpoint_saver.py` & `monai-weekly-1.2.dev2316/tests/test_handler_checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_classification_saver.py` & `monai-weekly-1.2.dev2316/tests/test_handler_classification_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_classification_saver_dist.py` & `monai-weekly-1.2.dev2316/tests/test_handler_classification_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_clearml_image.py` & `monai-weekly-1.2.dev2316/tests/test_handler_clearml_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_clearml_stats.py` & `monai-weekly-1.2.dev2316/tests/test_handler_clearml_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_confusion_matrix.py` & `monai-weekly-1.2.dev2316/tests/test_handler_confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_confusion_matrix_dist.py` & `monai-weekly-1.2.dev2316/tests/test_handler_confusion_matrix_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_decollate_batch.py` & `monai-weekly-1.2.dev2316/tests/test_handler_decollate_batch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_early_stop.py` & `monai-weekly-1.2.dev2316/tests/test_handler_early_stop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_garbage_collector.py` & `monai-weekly-1.2.dev2316/tests/test_handler_garbage_collector.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_hausdorff_distance.py` & `monai-weekly-1.2.dev2316/tests/test_handler_hausdorff_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_logfile.py` & `monai-weekly-1.2.dev2316/tests/test_handler_logfile.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_lr_scheduler.py` & `monai-weekly-1.2.dev2316/tests/test_handler_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_mean_dice.py` & `monai-weekly-1.2.dev2316/tests/test_handler_mean_dice.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_mean_iou.py` & `monai-weekly-1.2.dev2316/tests/test_handler_mean_iou.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_metric_logger.py` & `monai-weekly-1.2.dev2316/tests/test_handler_metric_logger.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_metrics_reloaded.py` & `monai-weekly-1.2.dev2316/tests/test_handler_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_metrics_saver.py` & `monai-weekly-1.2.dev2316/tests/test_handler_metrics_saver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_metrics_saver_dist.py` & `monai-weekly-1.2.dev2316/tests/test_handler_metrics_saver_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_mlflow.py` & `monai-weekly-1.2.dev2316/tests/test_handler_mlflow.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_nvtx.py` & `monai-weekly-1.2.dev2316/tests/test_handler_nvtx.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_panoptic_quality.py` & `monai-weekly-1.2.dev2316/tests/test_handler_panoptic_quality.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_parameter_scheduler.py` & `monai-weekly-1.2.dev2316/tests/test_handler_parameter_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_post_processing.py` & `monai-weekly-1.2.dev2316/tests/test_handler_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_prob_map_producer.py` & `monai-weekly-1.2.dev2316/tests/test_handler_prob_map_producer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_regression_metrics.py` & `monai-weekly-1.2.dev2316/tests/test_handler_regression_metrics.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_regression_metrics_dist.py` & `monai-weekly-1.2.dev2316/tests/test_handler_regression_metrics_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_rocauc.py` & `monai-weekly-1.2.dev2316/tests/test_handler_rocauc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_rocauc_dist.py` & `monai-weekly-1.2.dev2316/tests/test_handler_rocauc_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_smartcache.py` & `monai-weekly-1.2.dev2316/tests/test_handler_smartcache.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_stats.py` & `monai-weekly-1.2.dev2316/tests/test_handler_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_surface_distance.py` & `monai-weekly-1.2.dev2316/tests/test_handler_surface_distance.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_tb_image.py` & `monai-weekly-1.2.dev2316/tests/test_handler_tb_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_tb_stats.py` & `monai-weekly-1.2.dev2316/tests/test_handler_tb_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_handler_validation.py` & `monai-weekly-1.2.dev2316/tests/test_handler_validation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_hardnegsampler.py` & `monai-weekly-1.2.dev2316/tests/test_hardnegsampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_hashing.py` & `monai-weekly-1.2.dev2316/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_hausdorff_distance.py` & `monai-weekly-1.2.dev2316/tests/test_surface_distance.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,142 +13,173 @@
 
 import unittest
 
 import numpy as np
 import torch
 from parameterized import parameterized
 
-from monai.metrics import HausdorffDistanceMetric
+from monai.metrics import SurfaceDistanceMetric
 
 _device = "cuda:0" if torch.cuda.is_available() else "cpu"
 
 
 def create_spherical_seg_3d(
-    radius: float = 20.0, centre: tuple[int, int, int] = (49, 49, 49), im_shape: tuple[int, int, int] = (99, 99, 99)
+    radius: float = 20.0,
+    centre: tuple[int, int, int] = (49, 49, 49),
+    im_shape: tuple[int, int, int] = (99, 99, 99),
+    im_spacing: tuple[float, float, float] = (1.0, 1.0, 1.0),
 ) -> np.ndarray:
     """
     Return a 3D image with a sphere inside. Voxel values will be
     1 inside the sphere, and 0 elsewhere.
 
     Args:
         radius: radius of sphere (in terms of number of voxels, can be partial)
         centre: location of sphere centre.
-        im_shape: shape of image to create
+        im_shape: shape of image to create.
+        im_spacing: spacing of image to create.
 
     See also:
         :py:meth:`~create_test_image_3d`
     """
     # Create image
     image = np.zeros(im_shape, dtype=np.int32)
-    spy, spx, spz = np.ogrid[
-        -centre[0] : im_shape[0] - centre[0], -centre[1] : im_shape[1] - centre[1], -centre[2] : im_shape[2] - centre[2]
-    ]
+    spy, spx, spz = np.ogrid[: im_shape[0], : im_shape[1], : im_shape[2]]
+
+    spy = spy.astype(float) * im_spacing[0]
+    spx = spx.astype(float) * im_spacing[1]
+    spz = spz.astype(float) * im_spacing[2]
+
+    spy -= centre[0]
+    spx -= centre[1]
+    spz -= centre[2]
+
     circle = (spx * spx + spy * spy + spz * spz) <= radius * radius
 
     image[circle] = 1
     image[~circle] = 0
     return image
 
 
+test_spacing = (0.85, 1.2, 0.9)
 TEST_CASES = [
-    [[create_spherical_seg_3d(), create_spherical_seg_3d(), 1], [0, 0, 0, 0, 0, 0]],
+    [[create_spherical_seg_3d(), create_spherical_seg_3d(), "euclidean", None], [0, 0]],
     [
         [
             create_spherical_seg_3d(radius=20, centre=(20, 20, 20)),
             create_spherical_seg_3d(radius=20, centre=(19, 19, 19)),
+            "taxicab",
         ],
-        [1.7320508075688772, 1.7320508075688772, 1, 1, 3, 3],
+        [1.0380029806259314, 1.0380029806259314],
     ],
     [
         [
             create_spherical_seg_3d(radius=33, centre=(19, 33, 22)),
             create_spherical_seg_3d(radius=33, centre=(20, 33, 22)),
+            "euclidean",
+            None,
         ],
-        [1, 1, 1, 1, 1, 1],
+        [0.350217, 0.3483278807706289],
     ],
     [
         [
             create_spherical_seg_3d(radius=20, centre=(20, 33, 22)),
             create_spherical_seg_3d(radius=40, centre=(20, 33, 22)),
+            "euclidean",
+            None,
         ],
-        [20.09975124224178, 20.223748416156685, 15, 20, 24, 35],
+        [15.117741, 12.040033513150455],
     ],
     [
         [
-            # pred does not have foreground (but gt has), the metric should be inf
-            np.zeros([99, 99, 99]),
+            create_spherical_seg_3d(radius=20, centre=(20, 33, 22)),
             create_spherical_seg_3d(radius=40, centre=(20, 33, 22)),
+            "chessboard",
         ],
-        [np.inf, np.inf, np.inf, np.inf, np.inf, np.inf],
+        [11.492719, 9.605067064083457],
     ],
     [
         [
-            # gt does not have foreground (but pred has), the metric should be inf
-            create_spherical_seg_3d(),
-            np.zeros([99, 99, 99]),
+            create_spherical_seg_3d(radius=20, centre=(20, 33, 22)),
+            create_spherical_seg_3d(radius=40, centre=(20, 33, 22)),
+            "taxicab",
         ],
-        [np.inf, np.inf, np.inf, np.inf, np.inf, np.inf],
+        [20.214613, 12.432687531048186],
     ],
     [
+        [np.zeros([99, 99, 99]), create_spherical_seg_3d(radius=40, centre=(20, 33, 22)), "euclidean", None],
+        [np.inf, np.inf],
+    ],
+    [[create_spherical_seg_3d(), np.zeros([99, 99, 99]), "taxicab"], [np.inf, np.inf]],
+    [
         [
-            create_spherical_seg_3d(radius=20, centre=(20, 33, 22)),
-            create_spherical_seg_3d(radius=40, centre=(20, 33, 22)),
-            95,
+            create_spherical_seg_3d(radius=33, centre=(42, 45, 52), im_spacing=test_spacing),
+            create_spherical_seg_3d(radius=33, centre=(43, 45, 52), im_spacing=test_spacing),
+            "euclidean",
+            test_spacing,
         ],
-        [19.924858845171276, 20.09975124224178, 14, 18, 22, 33],
+        [0.4951, 0.4951],
     ],
 ]
 
 TEST_CASES_NANS = [
     [
         [
-            # both pred and gt do not have foreground, metric and not_nans should be 0
+            # both pred and gt do not have foreground, spacing is None, metric and not_nans should be 0
             np.zeros([99, 99, 99]),
             np.zeros([99, 99, 99]),
+            None,
         ]
-    ]
+    ],
+    [
+        [
+            # both pred and gt do not have foreground, spacing is not None, metric and not_nans should be 0
+            np.zeros([99, 99, 99]),
+            np.zeros([99, 99, 99]),
+            test_spacing,
+        ]
+    ],
 ]
 
 
-class TestHausdorffDistance(unittest.TestCase):
+class TestAllSurfaceMetrics(unittest.TestCase):
     @parameterized.expand(TEST_CASES)
     def test_value(self, input_data, expected_value):
-        percentile = None
         if len(input_data) == 3:
-            [seg_1, seg_2, percentile] = input_data
+            [seg_1, seg_2, metric] = input_data
+            spacing = None
         else:
-            [seg_1, seg_2] = input_data
+            [seg_1, seg_2, metric, spacing] = input_data
+
         ct = 0
         seg_1 = torch.tensor(seg_1, device=_device)
         seg_2 = torch.tensor(seg_2, device=_device)
-        for metric in ["euclidean", "chessboard", "taxicab"]:
-            for directed in [True, False]:
-                hd_metric = HausdorffDistanceMetric(
-                    include_background=False, distance_metric=metric, percentile=percentile, directed=directed
-                )
-                # shape of seg_1, seg_2 are: HWD, converts to BNHWD
-                batch, n_class = 2, 3
-                batch_seg_1 = seg_1.unsqueeze(0).unsqueeze(0).repeat([batch, n_class, 1, 1, 1])
-                batch_seg_2 = seg_2.unsqueeze(0).unsqueeze(0).repeat([batch, n_class, 1, 1, 1])
-                hd_metric(batch_seg_1, batch_seg_2)
-                result = hd_metric.aggregate(reduction="mean")
-                expected_value_curr = expected_value[ct]
-                np.testing.assert_allclose(expected_value_curr, result.cpu(), rtol=1e-7)
-                np.testing.assert_equal(result.device, seg_1.device)
-                ct += 1
+        for symmetric in [True, False]:
+            sur_metric = SurfaceDistanceMetric(include_background=False, symmetric=symmetric, distance_metric=metric)
+            # shape of seg_1, seg_2 are: HWD, converts to BNHWD
+            batch, n_class = 2, 3
+            batch_seg_1 = seg_1.unsqueeze(0).unsqueeze(0).repeat([batch, n_class, 1, 1, 1])
+            batch_seg_2 = seg_2.unsqueeze(0).unsqueeze(0).repeat([batch, n_class, 1, 1, 1])
+            sur_metric(batch_seg_1, batch_seg_2, spacing=spacing)
+            result = sur_metric.aggregate()
+            expected_value_curr = expected_value[ct]
+            np.testing.assert_allclose(expected_value_curr, result.cpu(), rtol=1e-5)
+            np.testing.assert_equal(result.device, seg_1.device)
+            ct += 1
 
     @parameterized.expand(TEST_CASES_NANS)
     def test_nans(self, input_data):
-        [seg_1, seg_2] = input_data
+        [seg_1, seg_2, spacing] = input_data
         seg_1 = torch.tensor(seg_1)
         seg_2 = torch.tensor(seg_2)
-        hd_metric = HausdorffDistanceMetric(include_background=False, get_not_nans=True)
-        batch_seg_1 = seg_1.unsqueeze(0).unsqueeze(0)
-        batch_seg_2 = seg_2.unsqueeze(0).unsqueeze(0)
-        hd_metric(batch_seg_1, batch_seg_2)
-        result, not_nans = hd_metric.aggregate()
-        np.testing.assert_allclose(0, result, rtol=1e-7)
-        np.testing.assert_allclose(0, not_nans, rtol=1e-7)
+        sur_metric = SurfaceDistanceMetric(include_background=False, get_not_nans=True)
+        # test list of channel-first Tensor
+        batch_seg_1 = [seg_1.unsqueeze(0)]
+        batch_seg_2 = [seg_2.unsqueeze(0)]
+        sur_metric(batch_seg_1, batch_seg_2, spacing=spacing)
+        result, not_nans = sur_metric.aggregate(reduction="mean")
+        np.testing.assert_allclose(0, result, rtol=1e-5)
+        np.testing.assert_allclose(0, not_nans, rtol=1e-5)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_header_correct.py` & `monai-weekly-1.2.dev2316/tests/test_header_correct.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_highresnet.py` & `monai-weekly-1.2.dev2316/tests/test_highresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_hilbert_transform.py` & `monai-weekly-1.2.dev2316/tests/test_hilbert_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_histogram_normalize.py` & `monai-weekly-1.2.dev2316/tests/test_histogram_normalize.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_histogram_normalized.py` & `monai-weekly-1.2.dev2316/tests/test_histogram_normalized.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_hovernet.py` & `monai-weekly-1.2.dev2316/tests/test_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_hovernet_instance_map_post_processing.py` & `monai-weekly-1.2.dev2316/tests/test_hovernet_instance_map_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_hovernet_instance_map_post_processingd.py` & `monai-weekly-1.2.dev2316/tests/test_hovernet_instance_map_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_hovernet_loss.py` & `monai-weekly-1.2.dev2316/tests/test_hovernet_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_hovernet_nuclear_type_post_processing.py` & `monai-weekly-1.2.dev2316/tests/test_hovernet_nuclear_type_post_processing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_hovernet_nuclear_type_post_processingd.py` & `monai-weekly-1.2.dev2316/tests/test_hovernet_nuclear_type_post_processingd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_identity.py` & `monai-weekly-1.2.dev2316/tests/test_identity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_identityd.py` & `monai-weekly-1.2.dev2316/tests/test_identityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_image_dataset.py` & `monai-weekly-1.2.dev2316/tests/test_image_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_image_filter.py` & `monai-weekly-1.2.dev2316/tests/test_image_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_image_rw.py` & `monai-weekly-1.2.dev2316/tests/test_image_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_img2tensorboard.py` & `monai-weekly-1.2.dev2316/tests/test_img2tensorboard.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_init_reader.py` & `monai-weekly-1.2.dev2316/tests/test_init_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_integration_autorunner.py` & `monai-weekly-1.2.dev2316/tests/test_integration_autorunner.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,50 +30,48 @@
     skip_if_no_cuda,
     skip_if_quick,
 )
 
 _, has_tb = optional_import("torch.utils.tensorboard", name="SummaryWriter")
 _, has_nni = optional_import("nni")
 
+num_images_perfold = max(torch.cuda.device_count(), 4)
+num_images_per_batch = 2
+
 sim_datalist: dict[str, list[dict]] = {
     "testing": [{"image": "val_001.fake.nii.gz"}, {"image": "val_002.fake.nii.gz"}],
     "training": [
-        {"fold": 0, "image": "tr_image_001.fake.nii.gz", "label": "tr_label_001.fake.nii.gz"},
-        {"fold": 0, "image": "tr_image_002.fake.nii.gz", "label": "tr_label_002.fake.nii.gz"},
-        {"fold": 0, "image": "tr_image_003.fake.nii.gz", "label": "tr_label_003.fake.nii.gz"},
-        {"fold": 0, "image": "tr_image_004.fake.nii.gz", "label": "tr_label_004.fake.nii.gz"},
-        {"fold": 1, "image": "tr_image_005.fake.nii.gz", "label": "tr_label_005.fake.nii.gz"},
-        {"fold": 1, "image": "tr_image_006.fake.nii.gz", "label": "tr_label_006.fake.nii.gz"},
-        {"fold": 1, "image": "tr_image_007.fake.nii.gz", "label": "tr_label_007.fake.nii.gz"},
-        {"fold": 1, "image": "tr_image_008.fake.nii.gz", "label": "tr_label_008.fake.nii.gz"},
-        {"fold": 2, "image": "tr_image_009.fake.nii.gz", "label": "tr_label_009.fake.nii.gz"},
-        {"fold": 2, "image": "tr_image_010.fake.nii.gz", "label": "tr_label_010.fake.nii.gz"},
-        {"fold": 2, "image": "tr_image_011.fake.nii.gz", "label": "tr_label_011.fake.nii.gz"},
-        {"fold": 2, "image": "tr_image_012.fake.nii.gz", "label": "tr_label_012.fake.nii.gz"},
+        {
+            "fold": f,
+            "image": f"tr_image_{(f * num_images_perfold + idx):03d}.nii.gz",
+            "label": f"tr_label_{(f * num_images_perfold + idx):03d}.nii.gz",
+        }
+        for f in range(num_images_per_batch + 1)
+        for idx in range(num_images_perfold)
     ],
 }
 
 train_param = (
     {
-        "num_images_per_batch": 2,
+        "num_images_per_batch": num_images_per_batch,
         "num_epochs": 2,
         "num_epochs_per_validation": 1,
         "num_warmup_epochs": 1,
         "use_pretrain": False,
         "pretrained_path": "",
     }
     if torch.cuda.is_available()
     else {}
 )
 
 pred_param = {"files_slices": slice(0, 1), "mode": "mean", "sigmoid": True}
 
 
 @skip_if_quick
-@SkipIfBeforePyTorchVersion((1, 9, 1))
+@SkipIfBeforePyTorchVersion((1, 11, 1))  # for mem_get_info
 @unittest.skipIf(not has_tb, "no tensorboard summary writer")
 class TestAutoRunner(unittest.TestCase):
     def setUp(self) -> None:
         self.test_dir = tempfile.TemporaryDirectory()
         test_path = self.test_dir.name
 
         sim_dataroot = os.path.join(test_path, "dataroot")
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_integration_bundle_run.py` & `monai-weekly-1.2.dev2316/tests/test_integration_bundle_run.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_integration_classification_2d.py` & `monai-weekly-1.2.dev2316/tests/test_integration_classification_2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -262,14 +262,14 @@
     def test_training(self):
         repeated = []
         for i in range(2):
             results = self.train_and_infer(i)
             repeated.append(results)
         np.testing.assert_allclose(repeated[0], repeated[1])
 
-    @TimedCall(seconds=1000, skip_timing=not torch.cuda.is_available(), force_quit=False, daemon=False)
+    @TimedCall(seconds=2000, skip_timing=not torch.cuda.is_available(), force_quit=False, daemon=False)
     def test_timing(self):
         self.train_and_infer()
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_integration_determinism.py` & `monai-weekly-1.2.dev2316/tests/test_integration_determinism.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_integration_fast_train.py` & `monai-weekly-1.2.dev2316/tests/test_integration_fast_train.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_integration_lazy_samples.py` & `monai-weekly-1.2.dev2316/tests/test_integration_lazy_samples.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_integration_nnunetv2_runner.py` & `monai-weekly-1.2.dev2316/tests/test_integration_nnunetv2_runner.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_integration_segmentation_3d.py` & `monai-weekly-1.2.dev2316/tests/test_integration_segmentation_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_integration_sliding_window.py` & `monai-weekly-1.2.dev2316/tests/test_integration_sliding_window.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_integration_stn.py` & `monai-weekly-1.2.dev2316/tests/test_integration_stn.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_integration_unet_2d.py` & `monai-weekly-1.2.dev2316/tests/test_integration_unet_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_integration_workers.py` & `monai-weekly-1.2.dev2316/tests/test_integration_workers.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_integration_workflows.py` & `monai-weekly-1.2.dev2316/tests/test_integration_workflows.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_integration_workflows_gan.py` & `monai-weekly-1.2.dev2316/tests/test_integration_workflows_gan.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_intensity_stats.py` & `monai-weekly-1.2.dev2316/tests/test_intensity_stats.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_intensity_statsd.py` & `monai-weekly-1.2.dev2316/tests/test_intensity_statsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_inverse.py` & `monai-weekly-1.2.dev2316/tests/test_inverse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_inverse_array.py` & `monai-weekly-1.2.dev2316/tests/test_inverse_array.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_inverse_collation.py` & `monai-weekly-1.2.dev2316/tests/test_inverse_collation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_invert.py` & `monai-weekly-1.2.dev2316/tests/test_invert.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_invertd.py` & `monai-weekly-1.2.dev2316/tests/test_invertd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_is_supported_format.py` & `monai-weekly-1.2.dev2316/tests/test_is_supported_format.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_iterable_dataset.py` & `monai-weekly-1.2.dev2316/tests/test_iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_itk_torch_bridge.py` & `monai-weekly-1.2.dev2316/tests/test_itk_torch_bridge.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_itk_writer.py` & `monai-weekly-1.2.dev2316/tests/test_itk_writer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_k_space_spike_noise.py` & `monai-weekly-1.2.dev2316/tests/test_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_k_space_spike_noised.py` & `monai-weekly-1.2.dev2316/tests/test_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_keep_largest_connected_component.py` & `monai-weekly-1.2.dev2316/tests/test_keep_largest_connected_component.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_keep_largest_connected_componentd.py` & `monai-weekly-1.2.dev2316/tests/test_keep_largest_connected_componentd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_kspace_mask.py` & `monai-weekly-1.2.dev2316/tests/test_kspace_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_label_filter.py` & `monai-weekly-1.2.dev2316/tests/test_label_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_label_filterd.py` & `monai-weekly-1.2.dev2316/tests/test_label_filterd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_label_quality_score.py` & `monai-weekly-1.2.dev2316/tests/test_label_quality_score.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_label_to_contour.py` & `monai-weekly-1.2.dev2316/tests/test_label_to_contour.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_label_to_contourd.py` & `monai-weekly-1.2.dev2316/tests/test_label_to_contourd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_label_to_mask.py` & `monai-weekly-1.2.dev2316/tests/test_label_to_mask.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_label_to_maskd.py` & `monai-weekly-1.2.dev2316/tests/test_label_to_maskd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_lambda.py` & `monai-weekly-1.2.dev2316/tests/test_lambda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_lambdad.py` & `monai-weekly-1.2.dev2316/tests/test_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_lesion_froc.py` & `monai-weekly-1.2.dev2316/tests/test_lesion_froc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_list_data_collate.py` & `monai-weekly-1.2.dev2316/tests/test_list_data_collate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_list_to_dict.py` & `monai-weekly-1.2.dev2316/tests/test_list_to_dict.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_lltm.py` & `monai-weekly-1.2.dev2316/tests/test_lltm.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_lmdbdataset.py` & `monai-weekly-1.2.dev2316/tests/test_lmdbdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_lmdbdataset_dist.py` & `monai-weekly-1.2.dev2316/tests/test_lmdbdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_load_decathlon_datalist.py` & `monai-weekly-1.2.dev2316/tests/test_load_decathlon_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_load_image.py` & `monai-weekly-1.2.dev2316/tests/test_load_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_load_imaged.py` & `monai-weekly-1.2.dev2316/tests/test_load_imaged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_load_spacing_orientation.py` & `monai-weekly-1.2.dev2316/tests/test_load_spacing_orientation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_loader_semaphore.py` & `monai-weekly-1.2.dev2316/tests/test_loader_semaphore.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_local_normalized_cross_correlation_loss.py` & `monai-weekly-1.2.dev2316/tests/test_local_normalized_cross_correlation_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_localnet.py` & `monai-weekly-1.2.dev2316/tests/test_localnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_localnet_block.py` & `monai-weekly-1.2.dev2316/tests/test_localnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_look_up_option.py` & `monai-weekly-1.2.dev2316/tests/test_look_up_option.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_loss_metric.py` & `monai-weekly-1.2.dev2316/tests/test_loss_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_lr_finder.py` & `monai-weekly-1.2.dev2316/tests/test_lr_finder.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             model=model,
             optimizer=optimizer,
             criterion=loss_function,
             device=device,
             pickle_module=pickle,
             pickle_protocol=4,
         )
-        lr_finder.range_test(train_loader, val_loader=train_loader, end_lr=10, num_iter=5)
+        lr_finder.range_test(train_loader, val_loader=train_loader, end_lr=10.0, num_iter=5)
         print(lr_finder.get_steepest_gradient(0, 0)[0])
 
         if has_matplotlib:
             ax = plt.subplot()
             plt.show(block=False)
             lr_finder.plot(0, 0, ax=ax)  # to inspect the loss-learning rate graph
             plt.pause(3)
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_lr_scheduler.py` & `monai-weekly-1.2.dev2316/tests/test_lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_make_nifti.py` & `monai-weekly-1.2.dev2316/tests/test_make_nifti.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_map_binary_to_indices.py` & `monai-weekly-1.2.dev2316/tests/test_map_binary_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_map_classes_to_indices.py` & `monai-weekly-1.2.dev2316/tests/test_map_classes_to_indices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_map_label_value.py` & `monai-weekly-1.2.dev2316/tests/test_map_label_value.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_map_label_valued.py` & `monai-weekly-1.2.dev2316/tests/test_map_label_valued.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_map_transform.py` & `monai-weekly-1.2.dev2316/tests/test_map_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_mask_intensity.py` & `monai-weekly-1.2.dev2316/tests/test_mask_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_mask_intensityd.py` & `monai-weekly-1.2.dev2316/tests/test_mask_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_masked_dice_loss.py` & `monai-weekly-1.2.dev2316/tests/test_masked_dice_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_masked_loss.py` & `monai-weekly-1.2.dev2316/tests/test_masked_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_masked_patch_wsi_dataset.py` & `monai-weekly-1.2.dev2316/tests/test_masked_patch_wsi_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,18 +28,17 @@
 cucim, has_cucim = optional_import("cucim")
 has_cucim = has_cucim and hasattr(cucim, "CuImage")
 _, has_osl = optional_import("openslide")
 _, has_tiff = optional_import("tifffile", name="imwrite")
 _, has_codec = optional_import("imagecodecs")
 has_tiff = has_tiff and has_codec
 
-FILE_KEY = "wsi_img"
+FILE_KEY = "wsi_generic_tiff"
 FILE_URL = testing_data_config("images", FILE_KEY, "url")
-base_name, extension = os.path.basename(f"{FILE_URL}"), ".tiff"
-FILE_PATH = os.path.join(os.path.dirname(__file__), "testing_data", "temp_" + base_name + extension)
+FILE_PATH = os.path.join(os.path.dirname(__file__), "testing_data", f"temp_{FILE_KEY}.tiff")
 
 TEST_CASE_0 = [
     {"data": [{"image": FILE_PATH, WSIPatchKeys.LEVEL: 8, WSIPatchKeys.SIZE: (2, 2)}], "mask_level": 8},
     {
         "num_patches": 4256,
         "wsi_size": [32914, 46000],
         "mask_level": 8,
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_matshow3d.py` & `monai-weekly-1.2.dev2316/tests/test_matshow3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_mean_ensemble.py` & `monai-weekly-1.2.dev2316/tests/test_mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_mean_ensembled.py` & `monai-weekly-1.2.dev2316/tests/test_mean_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_median_filter.py` & `monai-weekly-1.2.dev2316/tests/test_median_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_median_smooth.py` & `monai-weekly-1.2.dev2316/tests/test_median_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_median_smoothd.py` & `monai-weekly-1.2.dev2316/tests/test_median_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_mednistdataset.py` & `monai-weekly-1.2.dev2316/tests/test_mednistdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_meta_affine.py` & `monai-weekly-1.2.dev2316/tests/test_meta_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_meta_tensor.py` & `monai-weekly-1.2.dev2316/tests/test_meta_tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,14 +173,15 @@
         # shallow copy
         a = m
         self.check(a, m, ids=True)
         # deepcopy
         a = deepcopy(m)
         self.check(a, m, ids=False)
         # clone
+        a = m.clone(memory_format=torch.preserve_format)
         a = m.clone()
         self.check(a, m, ids=False)
         a = MetaTensor([[]], device=device, dtype=dtype)
         self.check(a, deepcopy(a), ids=False)
 
     @parameterized.expand(TESTS)
     def test_add(self, device, dtype):
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_metatensor_integration.py` & `monai-weekly-1.2.dev2316/tests/test_metatensor_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_metrics_reloaded.py` & `monai-weekly-1.2.dev2316/tests/test_metrics_reloaded.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_milmodel.py` & `monai-weekly-1.2.dev2316/tests/test_milmodel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_mlp.py` & `monai-weekly-1.2.dev2316/tests/test_mlp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_mmar_download.py` & `monai-weekly-1.2.dev2316/tests/test_mmar_download.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_module_list.py` & `monai-weekly-1.2.dev2316/tests/test_module_list.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_monai_env_vars.py` & `monai-weekly-1.2.dev2316/tests/test_monai_env_vars.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_monai_utils_misc.py` & `monai-weekly-1.2.dev2316/tests/test_monai_utils_misc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_mri_utils.py` & `monai-weekly-1.2.dev2316/tests/test_mri_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_multi_scale.py` & `monai-weekly-1.2.dev2316/tests/test_multi_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_net_adapter.py` & `monai-weekly-1.2.dev2316/tests/test_net_adapter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_network_consistency.py` & `monai-weekly-1.2.dev2316/tests/test_network_consistency.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_nifti_endianness.py` & `monai-weekly-1.2.dev2316/tests/test_nifti_endianness.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_nifti_header_revise.py` & `monai-weekly-1.2.dev2316/tests/test_nifti_header_revise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_nifti_rw.py` & `monai-weekly-1.2.dev2316/tests/test_nifti_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_normalize_intensity.py` & `monai-weekly-1.2.dev2316/tests/test_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_normalize_intensityd.py` & `monai-weekly-1.2.dev2316/tests/test_normalize_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_npzdictitemdataset.py` & `monai-weekly-1.2.dev2316/tests/test_npzdictitemdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_nrrd_reader.py` & `monai-weekly-1.2.dev2316/tests/test_nrrd_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_nuclick_transforms.py` & `monai-weekly-1.2.dev2316/tests/test_nuclick_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_numpy_reader.py` & `monai-weekly-1.2.dev2316/tests/test_numpy_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_nvtx_decorator.py` & `monai-weekly-1.2.dev2316/tests/test_nvtx_decorator.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_nvtx_transform.py` & `monai-weekly-1.2.dev2316/tests/test_nvtx_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_occlusion_sensitivity.py` & `monai-weekly-1.2.dev2316/tests/test_occlusion_sensitivity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_one_of.py` & `monai-weekly-1.2.dev2316/tests/test_one_of.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_optim_novograd.py` & `monai-weekly-1.2.dev2316/tests/test_optim_novograd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_optional_import.py` & `monai-weekly-1.2.dev2316/tests/test_optional_import.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_ori_ras_lps.py` & `monai-weekly-1.2.dev2316/tests/test_ori_ras_lps.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_orientation.py` & `monai-weekly-1.2.dev2316/tests/test_orientation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_orientationd.py` & `monai-weekly-1.2.dev2316/tests/test_orientationd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_p3d_block.py` & `monai-weekly-1.2.dev2316/tests/test_p3d_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_pad_collation.py` & `monai-weekly-1.2.dev2316/tests/test_pad_collation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_pad_mode.py` & `monai-weekly-1.2.dev2316/tests/test_pad_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_parallel_execution.py` & `monai-weekly-1.2.dev2316/tests/test_parallel_execution.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_parallel_execution_dist.py` & `monai-weekly-1.2.dev2316/tests/test_parallel_execution_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_partition_dataset.py` & `monai-weekly-1.2.dev2316/tests/test_partition_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_partition_dataset_classes.py` & `monai-weekly-1.2.dev2316/tests/test_partition_dataset_classes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_patch_dataset.py` & `monai-weekly-1.2.dev2316/tests/test_patch_dataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_patch_inferer.py` & `monai-weekly-1.2.dev2316/tests/test_patch_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_patch_wsi_dataset.py` & `monai-weekly-1.2.dev2316/tests/test_patch_wsi_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,17 @@
 cucim, has_cim = optional_import("cucim")
 has_cim = has_cim and hasattr(cucim, "CuImage")
 openslide, has_osl = optional_import("openslide")
 imwrite, has_tiff = optional_import("tifffile", name="imwrite")
 _, has_codec = optional_import("imagecodecs")
 has_tiff = has_tiff and has_codec
 
-FILE_KEY = "wsi_img"
+FILE_KEY = "wsi_generic_tiff"
 FILE_URL = testing_data_config("images", FILE_KEY, "url")
-base_name, extension = os.path.basename(f"{FILE_URL}"), ".tiff"
-FILE_PATH = os.path.join(os.path.dirname(__file__), "testing_data", "temp_" + base_name + extension)
+FILE_PATH = os.path.join(os.path.dirname(__file__), "testing_data", f"temp_{FILE_KEY}.tiff")
 
 TEST_CASE_0 = [
     {
         "data": [{"image": FILE_PATH, WSIPatchKeys.LOCATION.value: [0, 0], "label": [1], "patch_level": 0}],
         "patch_size": (1, 1),
     },
     {"image": np.array([[[239]], [[239]], [[239]]], dtype=np.uint8), "label": np.array([1])},
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_patchembedding.py` & `monai-weekly-1.2.dev2316/tests/test_patchembedding.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_pathology_he_stain.py` & `monai-weekly-1.2.dev2316/tests/test_pathology_he_stain.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_pathology_he_stain_dict.py` & `monai-weekly-1.2.dev2316/tests/test_pathology_he_stain_dict.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_pathology_prob_nms.py` & `monai-weekly-1.2.dev2316/tests/test_pathology_prob_nms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_persistentdataset.py` & `monai-weekly-1.2.dev2316/tests/test_persistentdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_persistentdataset_dist.py` & `monai-weekly-1.2.dev2316/tests/test_persistentdataset_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_phl_cpu.py` & `monai-weekly-1.2.dev2316/tests/test_phl_cpu.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_phl_cuda.py` & `monai-weekly-1.2.dev2316/tests/test_phl_cuda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_pil_reader.py` & `monai-weekly-1.2.dev2316/tests/test_pil_reader.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_plot_2d_or_3d_image.py` & `monai-weekly-1.2.dev2316/tests/test_plot_2d_or_3d_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_png_rw.py` & `monai-weekly-1.2.dev2316/tests/test_png_rw.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_polyval.py` & `monai-weekly-1.2.dev2316/tests/test_polyval.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_prepare_batch_default.py` & `monai-weekly-1.2.dev2316/tests/test_prepare_batch_default.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_prepare_batch_default_dist.py` & `monai-weekly-1.2.dev2316/tests/test_prepare_batch_default_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_prepare_batch_extra_input.py` & `monai-weekly-1.2.dev2316/tests/test_prepare_batch_extra_input.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_prepare_batch_hovernet.py` & `monai-weekly-1.2.dev2316/tests/test_prepare_batch_hovernet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_preset_filters.py` & `monai-weekly-1.2.dev2316/tests/test_preset_filters.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_print_info.py` & `monai-weekly-1.2.dev2316/tests/test_print_info.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_print_transform_backends.py` & `monai-weekly-1.2.dev2316/tests/test_print_transform_backends.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_probnms.py` & `monai-weekly-1.2.dev2316/tests/test_probnms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_probnmsd.py` & `monai-weekly-1.2.dev2316/tests/test_probnmsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_profiling.py` & `monai-weekly-1.2.dev2316/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_pytorch_version_after.py` & `monai-weekly-1.2.dev2316/tests/test_pytorch_version_after.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_query_memory.py` & `monai-weekly-1.2.dev2316/tests/test_query_memory.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_adjust_contrast.py` & `monai-weekly-1.2.dev2316/tests/test_rand_adjust_contrast.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_adjust_contrastd.py` & `monai-weekly-1.2.dev2316/tests/test_rand_adjust_contrastd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_affine.py` & `monai-weekly-1.2.dev2316/tests/test_rand_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_affine_grid.py` & `monai-weekly-1.2.dev2316/tests/test_rand_affine_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_affined.py` & `monai-weekly-1.2.dev2316/tests/test_rand_affined.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_axis_flip.py` & `monai-weekly-1.2.dev2316/tests/test_rand_axis_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_axis_flipd.py` & `monai-weekly-1.2.dev2316/tests/test_rand_axis_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_bias_field.py` & `monai-weekly-1.2.dev2316/tests/test_rand_bias_field.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_bias_fieldd.py` & `monai-weekly-1.2.dev2316/tests/test_rand_bias_fieldd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_coarse_dropout.py` & `monai-weekly-1.2.dev2316/tests/test_rand_coarse_dropout.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_coarse_dropoutd.py` & `monai-weekly-1.2.dev2316/tests/test_rand_coarse_dropoutd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_coarse_shuffle.py` & `monai-weekly-1.2.dev2316/tests/test_rand_coarse_shuffle.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_coarse_shuffled.py` & `monai-weekly-1.2.dev2316/tests/test_rand_coarse_shuffled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_crop_by_label_classes.py` & `monai-weekly-1.2.dev2316/tests/test_rand_crop_by_label_classes.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_crop_by_label_classesd.py` & `monai-weekly-1.2.dev2316/tests/test_rand_crop_by_label_classesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_crop_by_pos_neg_label.py` & `monai-weekly-1.2.dev2316/tests/test_rand_crop_by_pos_neg_label.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_crop_by_pos_neg_labeld.py` & `monai-weekly-1.2.dev2316/tests/test_rand_crop_by_pos_neg_labeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_cucim_dict_transform.py` & `monai-weekly-1.2.dev2316/tests/test_rand_cucim_dict_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_cucim_transform.py` & `monai-weekly-1.2.dev2316/tests/test_rand_cucim_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_deform_grid.py` & `monai-weekly-1.2.dev2316/tests/test_rand_deform_grid.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_elastic_2d.py` & `monai-weekly-1.2.dev2316/tests/test_rand_elastic_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_elastic_3d.py` & `monai-weekly-1.2.dev2316/tests/test_rand_elastic_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_elasticd_2d.py` & `monai-weekly-1.2.dev2316/tests/test_rand_elasticd_2d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_elasticd_3d.py` & `monai-weekly-1.2.dev2316/tests/test_rand_elasticd_3d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_flip.py` & `monai-weekly-1.2.dev2316/tests/test_rand_flip.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_flipd.py` & `monai-weekly-1.2.dev2316/tests/test_rand_flipd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_gaussian_noise.py` & `monai-weekly-1.2.dev2316/tests/test_rand_gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_gaussian_noised.py` & `monai-weekly-1.2.dev2316/tests/test_rand_gaussian_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_gaussian_sharpen.py` & `monai-weekly-1.2.dev2316/tests/test_rand_gaussian_sharpen.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_gaussian_sharpend.py` & `monai-weekly-1.2.dev2316/tests/test_rand_gaussian_sharpend.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_gaussian_smooth.py` & `monai-weekly-1.2.dev2316/tests/test_rand_gaussian_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_gaussian_smoothd.py` & `monai-weekly-1.2.dev2316/tests/test_rand_gaussian_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_gibbs_noise.py` & `monai-weekly-1.2.dev2316/tests/test_rand_gibbs_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_gibbs_noised.py` & `monai-weekly-1.2.dev2316/tests/test_rand_gibbs_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_grid_distortion.py` & `monai-weekly-1.2.dev2316/tests/test_rand_grid_distortion.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_grid_distortiond.py` & `monai-weekly-1.2.dev2316/tests/test_rand_grid_distortiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_grid_patch.py` & `monai-weekly-1.2.dev2316/tests/test_rand_grid_patch.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_grid_patchd.py` & `monai-weekly-1.2.dev2316/tests/test_rand_grid_patchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_histogram_shift.py` & `monai-weekly-1.2.dev2316/tests/test_rand_histogram_shift.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_histogram_shiftd.py` & `monai-weekly-1.2.dev2316/tests/test_rand_histogram_shiftd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_k_space_spike_noise.py` & `monai-weekly-1.2.dev2316/tests/test_rand_k_space_spike_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_k_space_spike_noised.py` & `monai-weekly-1.2.dev2316/tests/test_rand_k_space_spike_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_lambda.py` & `monai-weekly-1.2.dev2316/tests/test_rand_lambda.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_lambdad.py` & `monai-weekly-1.2.dev2316/tests/test_rand_lambdad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_rician_noise.py` & `monai-weekly-1.2.dev2316/tests/test_rand_rician_noise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_rician_noised.py` & `monai-weekly-1.2.dev2316/tests/test_rand_rician_noised.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_rotate.py` & `monai-weekly-1.2.dev2316/tests/test_rand_rotate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_rotate90.py` & `monai-weekly-1.2.dev2316/tests/test_rand_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_rotate90d.py` & `monai-weekly-1.2.dev2316/tests/test_rand_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_rotated.py` & `monai-weekly-1.2.dev2316/tests/test_rand_rotated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_scale_crop.py` & `monai-weekly-1.2.dev2316/tests/test_rand_scale_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_scale_cropd.py` & `monai-weekly-1.2.dev2316/tests/test_rand_scale_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_scale_intensity.py` & `monai-weekly-1.2.dev2316/tests/test_rand_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_scale_intensityd.py` & `monai-weekly-1.2.dev2316/tests/test_rand_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_shift_intensity.py` & `monai-weekly-1.2.dev2316/tests/test_rand_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_shift_intensityd.py` & `monai-weekly-1.2.dev2316/tests/test_rand_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_spatial_crop.py` & `monai-weekly-1.2.dev2316/tests/test_rand_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_spatial_crop_samples.py` & `monai-weekly-1.2.dev2316/tests/test_rand_spatial_crop_samples.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_spatial_crop_samplesd.py` & `monai-weekly-1.2.dev2316/tests/test_rand_spatial_crop_samplesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_spatial_cropd.py` & `monai-weekly-1.2.dev2316/tests/test_rand_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_std_shift_intensity.py` & `monai-weekly-1.2.dev2316/tests/test_rand_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_std_shift_intensityd.py` & `monai-weekly-1.2.dev2316/tests/test_rand_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_weighted_crop.py` & `monai-weekly-1.2.dev2316/tests/test_rand_weighted_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_weighted_cropd.py` & `monai-weekly-1.2.dev2316/tests/test_rand_weighted_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_zoom.py` & `monai-weekly-1.2.dev2316/tests/test_rand_zoom.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rand_zoomd.py` & `monai-weekly-1.2.dev2316/tests/test_rand_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_randidentity.py` & `monai-weekly-1.2.dev2316/tests/test_randidentity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_random_order.py` & `monai-weekly-1.2.dev2316/tests/test_random_order.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_randomizable.py` & `monai-weekly-1.2.dev2316/tests/test_randomizable.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_randomizable_transform_type.py` & `monai-weekly-1.2.dev2316/tests/test_randomizable_transform_type.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_randtorchvisiond.py` & `monai-weekly-1.2.dev2316/tests/test_randtorchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rankfilter_dist.py` & `monai-weekly-1.2.dev2316/tests/test_rankfilter_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_recon_net_utils.py` & `monai-weekly-1.2.dev2316/tests/test_recon_net_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_reference_based_normalize_intensity.py` & `monai-weekly-1.2.dev2316/tests/test_reference_based_normalize_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_reference_based_spatial_cropd.py` & `monai-weekly-1.2.dev2316/tests/test_reference_based_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_reference_resolver.py` & `monai-weekly-1.2.dev2316/tests/test_reference_resolver.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_reg_loss_integration.py` & `monai-weekly-1.2.dev2316/tests/test_reg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_regunet.py` & `monai-weekly-1.2.dev2316/tests/test_regunet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_regunet_block.py` & `monai-weekly-1.2.dev2316/tests/test_regunet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_remove_repeated_channel.py` & `monai-weekly-1.2.dev2316/tests/test_remove_repeated_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_remove_repeated_channeld.py` & `monai-weekly-1.2.dev2316/tests/test_remove_repeated_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_remove_small_objects.py` & `monai-weekly-1.2.dev2316/tests/test_remove_small_objects.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_repeat_channel.py` & `monai-weekly-1.2.dev2316/tests/test_repeat_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_repeat_channeld.py` & `monai-weekly-1.2.dev2316/tests/test_repeat_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_replace_module.py` & `monai-weekly-1.2.dev2316/tests/test_replace_module.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_require_pkg.py` & `monai-weekly-1.2.dev2316/tests/test_require_pkg.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_resample.py` & `monai-weekly-1.2.dev2316/tests/test_resample.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,19 +24,27 @@
 def rotate_90_2d():
     t = torch.eye(3)
     t[:, 0] = torch.FloatTensor([0, -1, 0])
     t[:, 1] = torch.FloatTensor([1, 0, 0])
     return t
 
 
-RESAMPLE_FUNCTION_CASES = [(get_arange_img((3, 3)), rotate_90_2d(), [[0, 3, 6], [0, 3, 6], [0, 3, 6]])]
+RESAMPLE_FUNCTION_CASES = [
+    (get_arange_img((3, 3)), rotate_90_2d(), [[0, 3, 6], [0, 3, 6], [0, 3, 6]]),
+    (get_arange_img((3, 3)), torch.eye(3), get_arange_img((3, 3))[0]),
+]
 
 
 class TestResampleFunction(unittest.TestCase):
     @parameterized.expand(RESAMPLE_FUNCTION_CASES)
     def test_resample_function_impl(self, img, matrix, expected):
         out = resample(convert_to_tensor(img), matrix, {"lazy_shape": img.shape[1:], "lazy_padding_mode": "border"})
         assert_allclose(out[0], expected, type_test=False)
 
+        img = convert_to_tensor(img, dtype=torch.uint8)
+        out = resample(img, matrix, {"lazy_resample_mode": "auto", "lazy_dtype": torch.float})
+        out_1 = resample(img, matrix, {"lazy_resample_mode": "other value", "lazy_dtype": torch.float})
+        self.assertIs(out.dtype, out_1.dtype)  # testing dtype in different lazy_resample_mode
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_resample_backends.py` & `monai-weekly-1.2.dev2316/tests/test_resample_backends.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_resample_datalist.py` & `monai-weekly-1.2.dev2316/tests/test_resample_datalist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_resample_to_match.py` & `monai-weekly-1.2.dev2316/tests/test_resample_to_match.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_resample_to_matchd.py` & `monai-weekly-1.2.dev2316/tests/test_resample_to_matchd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_resampler.py` & `monai-weekly-1.2.dev2316/tests/test_resampler.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_resize.py` & `monai-weekly-1.2.dev2316/tests/test_resize.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_resize_with_pad_or_crop.py` & `monai-weekly-1.2.dev2316/tests/test_resize_with_pad_or_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_resize_with_pad_or_cropd.py` & `monai-weekly-1.2.dev2316/tests/test_resize_with_pad_or_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_resized.py` & `monai-weekly-1.2.dev2316/tests/test_resized.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_resnet.py` & `monai-weekly-1.2.dev2316/tests/test_resnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_retinanet.py` & `monai-weekly-1.2.dev2316/tests/test_retinanet.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import torch
 from parameterized import parameterized
 
 from monai.apps.detection.networks.retinanet_network import RetinaNet, resnet_fpn_feature_extractor
 from monai.networks import eval_mode
 from monai.networks.nets import resnet10, resnet18, resnet34, resnet50, resnet101, resnet152, resnet200
 from monai.utils import ensure_tuple, optional_import
-from tests.utils import SkipIfBeforePyTorchVersion, test_onnx_save, test_script_save
+from tests.utils import SkipIfBeforePyTorchVersion, skip_if_quick, test_onnx_save, test_script_save
 
 _, has_torchvision = optional_import("torchvision")
 
 device = "cuda" if torch.cuda.is_available() else "cpu"
 num_anchors = 7
 
 TEST_CASE_1 = [  # 3D, batch 3, 2 input channel
@@ -95,14 +95,15 @@
 for case in [TEST_CASE_1]:
     for model in [resnet10, resnet18, resnet34, resnet50, resnet101, resnet152, resnet200]:
         TEST_CASES_TS.append([model, *case])
 
 
 @SkipIfBeforePyTorchVersion((1, 12))
 @unittest.skipUnless(has_torchvision, "Requires torchvision")
+@skip_if_quick
 class TestRetinaNet(unittest.TestCase):
     @parameterized.expand(TEST_CASES)
     def test_retina_shape(self, model, input_param, input_shape):
         backbone = model(**input_param)
         feature_extractor = resnet_fpn_feature_extractor(
             backbone=backbone,
             spatial_dims=input_param["spatial_dims"],
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_retinanet_detector.py` & `monai-weekly-1.2.dev2316/tests/test_retinanet_detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import torch
 from parameterized import parameterized
 
 from monai.apps.detection.networks.retinanet_detector import RetinaNetDetector, retinanet_resnet50_fpn_detector
 from monai.apps.detection.utils.anchor_utils import AnchorGeneratorWithAnchorShape
 from monai.networks import eval_mode, train_mode
 from monai.utils import optional_import
-from tests.utils import SkipIfBeforePyTorchVersion, test_script_save
+from tests.utils import SkipIfBeforePyTorchVersion, skip_if_quick, test_script_save
 
 _, has_torchvision = optional_import("torchvision")
 
 num_anchors = 7
 
 TEST_CASE_1 = [  # 3D, batch 3, 2 input channel
     {
@@ -108,14 +108,15 @@
             -self.spatial_dims :
         ]
         return {self.cls_key: [torch.randn(out_cls_shape)], self.box_reg_key: [torch.randn(out_box_reg_shape)]}
 
 
 @SkipIfBeforePyTorchVersion((1, 11))
 @unittest.skipUnless(has_torchvision, "Requires torchvision")
+@skip_if_quick
 class TestRetinaNetDetector(unittest.TestCase):
     @parameterized.expand(TEST_CASES)
     def test_retina_detector_resnet_backbone_shape(self, input_param, input_shape):
         returned_layers = [1]
         anchor_generator = AnchorGeneratorWithAnchorShape(
             feature_map_scales=(1, 2), base_anchor_shapes=((8,) * input_param["spatial_dims"],)
         )
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_retinanet_predict_utils.py` & `monai-weekly-1.2.dev2316/tests/test_retinanet_predict_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rotate.py` & `monai-weekly-1.2.dev2316/tests/test_rotate.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rotate90.py` & `monai-weekly-1.2.dev2316/tests/test_rotate90.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rotate90d.py` & `monai-weekly-1.2.dev2316/tests/test_rotate90d.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_rotated.py` & `monai-weekly-1.2.dev2316/tests/test_rotated.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_safe_dtype_range.py` & `monai-weekly-1.2.dev2316/tests/test_safe_dtype_range.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_saliency_inferer.py` & `monai-weekly-1.2.dev2316/tests/test_saliency_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_sample_slices.py` & `monai-weekly-1.2.dev2316/tests/test_sample_slices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_sampler_dist.py` & `monai-weekly-1.2.dev2316/tests/test_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_save_classificationd.py` & `monai-weekly-1.2.dev2316/tests/test_save_classificationd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_save_image.py` & `monai-weekly-1.2.dev2316/tests/test_save_image.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_save_imaged.py` & `monai-weekly-1.2.dev2316/tests/test_save_imaged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_save_state.py` & `monai-weekly-1.2.dev2316/tests/test_save_state.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_savitzky_golay_filter.py` & `monai-weekly-1.2.dev2316/tests/test_savitzky_golay_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_savitzky_golay_smooth.py` & `monai-weekly-1.2.dev2316/tests/test_savitzky_golay_smooth.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_savitzky_golay_smoothd.py` & `monai-weekly-1.2.dev2316/tests/test_savitzky_golay_smoothd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_scale_intensity.py` & `monai-weekly-1.2.dev2316/tests/test_scale_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_scale_intensity_range.py` & `monai-weekly-1.2.dev2316/tests/test_scale_intensity_range.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_scale_intensity_range_percentiles.py` & `monai-weekly-1.2.dev2316/tests/test_scale_intensity_range_percentiles.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_scale_intensity_range_percentilesd.py` & `monai-weekly-1.2.dev2316/tests/test_scale_intensity_range_percentilesd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_scale_intensity_ranged.py` & `monai-weekly-1.2.dev2316/tests/test_scale_intensity_ranged.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_scale_intensityd.py` & `monai-weekly-1.2.dev2316/tests/test_scale_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_se_block.py` & `monai-weekly-1.2.dev2316/tests/test_se_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_se_blocks.py` & `monai-weekly-1.2.dev2316/tests/test_se_blocks.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_seg_loss_integration.py` & `monai-weekly-1.2.dev2316/tests/test_seg_loss_integration.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_segresnet.py` & `monai-weekly-1.2.dev2316/tests/test_segresnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_segresnet_block.py` & `monai-weekly-1.2.dev2316/tests/test_segresnet_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_segresnet_ds.py` & `monai-weekly-1.2.dev2316/tests/test_segresnet_ds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_select_cross_validation_folds.py` & `monai-weekly-1.2.dev2316/tests/test_select_cross_validation_folds.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_select_itemsd.py` & `monai-weekly-1.2.dev2316/tests/test_select_itemsd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_selfattention.py` & `monai-weekly-1.2.dev2316/tests/test_selfattention.py`

 * *Files 15% similar despite different names*

```diff
@@ -48,10 +48,31 @@
     def test_ill_arg(self):
         with self.assertRaises(ValueError):
             SABlock(hidden_size=128, num_heads=12, dropout_rate=6.0)
 
         with self.assertRaises(ValueError):
             SABlock(hidden_size=620, num_heads=8, dropout_rate=0.4)
 
+    def test_access_attn_matrix(self):
+        # input format
+        hidden_size = 128
+        num_heads = 2
+        dropout_rate = 0
+        input_shape = (2, 256, hidden_size)
+
+        # be  not able to access the matrix
+        no_matrix_acess_blk = SABlock(hidden_size=hidden_size, num_heads=num_heads, dropout_rate=dropout_rate)
+        no_matrix_acess_blk(torch.randn(input_shape))
+        assert type(no_matrix_acess_blk.att_mat) == torch.Tensor
+        # no of elements is zero
+        assert no_matrix_acess_blk.att_mat.nelement() == 0
+
+        # be able to acess the attention matrix
+        matrix_acess_blk = SABlock(
+            hidden_size=hidden_size, num_heads=num_heads, dropout_rate=dropout_rate, save_attn=True
+        )
+        matrix_acess_blk(torch.randn(input_shape))
+        assert matrix_acess_blk.att_mat.shape == (input_shape[0], input_shape[0], input_shape[1], input_shape[1])
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_senet.py` & `monai-weekly-1.2.dev2316/tests/test_senet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_separable_filter.py` & `monai-weekly-1.2.dev2316/tests/test_separable_filter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_set_determinism.py` & `monai-weekly-1.2.dev2316/tests/test_set_determinism.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_set_visible_devices.py` & `monai-weekly-1.2.dev2316/tests/test_set_visible_devices.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_shift_intensity.py` & `monai-weekly-1.2.dev2316/tests/test_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_shift_intensityd.py` & `monai-weekly-1.2.dev2316/tests/test_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_shuffle_buffer.py` & `monai-weekly-1.2.dev2316/tests/test_shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_signal_continuouswavelet.py` & `monai-weekly-1.2.dev2316/tests/test_signal_continuouswavelet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_signal_fillempty.py` & `monai-weekly-1.2.dev2316/tests/test_signal_fillempty.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_signal_rand_add_gaussiannoise.py` & `monai-weekly-1.2.dev2316/tests/test_signal_rand_add_gaussiannoise.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_signal_rand_add_sine.py` & `monai-weekly-1.2.dev2316/tests/test_signal_rand_add_sine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_signal_rand_add_sine_partial.py` & `monai-weekly-1.2.dev2316/tests/test_signal_rand_add_sine_partial.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_signal_rand_add_squarepulse.py` & `monai-weekly-1.2.dev2316/tests/test_signal_rand_add_squarepulse.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_signal_rand_add_squarepulse_partial.py` & `monai-weekly-1.2.dev2316/tests/test_signal_rand_add_squarepulse_partial.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_signal_rand_drop.py` & `monai-weekly-1.2.dev2316/tests/test_signal_rand_drop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_signal_rand_scale.py` & `monai-weekly-1.2.dev2316/tests/test_signal_rand_scale.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_signal_rand_shift.py` & `monai-weekly-1.2.dev2316/tests/test_signal_rand_shift.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_signal_remove_frequency.py` & `monai-weekly-1.2.dev2316/tests/test_signal_remove_frequency.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_simple_aspp.py` & `monai-weekly-1.2.dev2316/tests/test_simple_aspp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_simulatedelay.py` & `monai-weekly-1.2.dev2316/tests/test_simulatedelay.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_simulatedelayd.py` & `monai-weekly-1.2.dev2316/tests/test_simulatedelayd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_skip_connection.py` & `monai-weekly-1.2.dev2316/tests/test_skip_connection.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_slice_inferer.py` & `monai-weekly-1.2.dev2316/tests/test_slice_inferer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_sliding_patch_wsi_dataset.py` & `monai-weekly-1.2.dev2316/tests/test_sliding_patch_wsi_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,18 +28,17 @@
 cucim, has_cucim = optional_import("cucim")
 has_cucim = has_cucim and hasattr(cucim, "CuImage")
 openslide, has_osl = optional_import("openslide")
 imwrite, has_tiff = optional_import("tifffile", name="imwrite")
 _, has_codec = optional_import("imagecodecs")
 has_tiff = has_tiff and has_codec
 
-FILE_KEY = "wsi_img"
+FILE_KEY = "wsi_generic_tiff"
 FILE_URL = testing_data_config("images", FILE_KEY, "url")
-base_name, extension = os.path.basename(f"{FILE_URL}"), ".tiff"
-FILE_PATH = os.path.join(os.path.dirname(__file__), "testing_data", "temp_" + base_name + extension)
+FILE_PATH = os.path.join(os.path.dirname(__file__), "testing_data", f"temp_{FILE_KEY}.tiff")
 
 FILE_PATH_SMALL_0 = os.path.join(os.path.dirname(__file__), "testing_data", "temp_wsi_inference_0.tiff")
 FILE_PATH_SMALL_1 = os.path.join(os.path.dirname(__file__), "testing_data", "temp_wsi_inference_1.tiff")
 ARRAY_SMALL_0 = np.random.randint(low=0, high=255, size=(3, 4, 4), dtype=np.uint8)
 ARRAY_SMALL_1 = np.random.randint(low=0, high=255, size=(3, 5, 5), dtype=np.uint8)
 
 TEST_CASE_SMALL_0 = [
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_sliding_window_hovernet_inference.py` & `monai-weekly-1.2.dev2316/tests/test_sliding_window_hovernet_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,27 +14,30 @@
 import unittest
 
 import numpy as np
 import torch
 from parameterized import parameterized
 
 from monai.apps.pathology.inferers import SlidingWindowHoVerNetInferer
+from monai.data import MetaTensor
 from monai.inferers import sliding_window_inference
 from monai.utils import optional_import
 from tests.test_sliding_window_inference import TEST_CASES
 
 _, has_tqdm = optional_import("tqdm")
 
 TEST_CASES_PADDING = [
     [None, (1, 3, 16, 8), (4, 4), 7, 0.5, "constant", torch.device("cpu:0"), None],
     ["hover", (1, 3, 16, 8), (4, 4), 7, 0.5, "constant", torch.device("cpu:0"), None],
     [None, (1, 3, 16, 8), (4, 4), 7, 0.5, "constant", torch.device("cpu:0"), (1,) * 4],
     ["hover", (1, 3, 16, 8), (4, 4), 7, 0.5, "constant", torch.device("cpu:0"), (1,) * 4],
 ]
 
+TEST_CASES_MULTIOUTPUT = [[torch.ones((1, 6, 20, 20))], [MetaTensor(torch.ones((1, 6, 20, 20)))]]
+
 
 class TestSlidingWindowHoVerNetInference(unittest.TestCase):
     @parameterized.expand(TEST_CASES_PADDING)
     def test_sliding_window_with_padding(
         self, key, image_shape, roi_shape, sw_batch_size, overlap, mode, device, extra_input_padding
     ):
         n_total = np.prod(image_shape)
@@ -241,17 +244,18 @@
         np.testing.assert_allclose(result.cpu().numpy(), expected, rtol=1e-4)
 
         result = SlidingWindowHoVerNetInferer(
             roi_shape, sw_batch_size, overlap=0.5, mode="constant", cval=-1, progress=has_tqdm
         )(inputs, compute, t1, test2=t2)
         np.testing.assert_allclose(result.cpu().numpy(), expected, rtol=1e-4)
 
-    def test_multioutput(self):
+    @parameterized.expand(TEST_CASES_MULTIOUTPUT)
+    def test_multioutput(self, inputs):
         device = "cuda" if torch.cuda.is_available() else "cpu:0"
-        inputs = torch.ones((1, 6, 20, 20)).to(device=device)
+        inputs = inputs.to(device=device)
         roi_shape = (8, 8)
         sw_batch_size = 10
 
         def compute(data):
             return data + 1, data[:, ::3, ::2, ::2] + 2, data[:, ::2, ::4, ::4] + 3
 
         def compute_dict(data):
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_sliding_window_inference.py` & `monai-weekly-1.2.dev2316/tests/test_sliding_window_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import unittest
 
 import numpy as np
 import torch
 from parameterized import parameterized
 
 from monai.data.utils import list_data_collate
-from monai.inferers import SlidingWindowInferer, sliding_window_inference
+from monai.inferers import SlidingWindowInferer, SlidingWindowInfererAdapt, sliding_window_inference
 from monai.utils import optional_import
 from tests.utils import TEST_TORCH_AND_META_TENSORS, skip_if_no_cuda, test_is_quick
 
 _, has_tqdm = optional_import("tqdm")
 
 TEST_CASES = [
     [(2, 3, 16), (4,), 3, 0.25, "constant", torch.device("cpu:0")],  # 1D small roi
@@ -301,14 +301,19 @@
         np.testing.assert_allclose(result.cpu().numpy(), expected, rtol=1e-4)
 
         result = SlidingWindowInferer(
             roi_shape, sw_batch_size, overlap=0.5, mode="constant", cval=-1, progress=has_tqdm
         )(inputs, compute, t1, test2=t2)
         np.testing.assert_allclose(result.cpu().numpy(), expected, rtol=1e-4)
 
+        result = SlidingWindowInfererAdapt(
+            roi_shape, sw_batch_size, overlap=0.5, mode="constant", cval=-1, progress=has_tqdm
+        )(inputs, compute, t1, test2=t2)
+        np.testing.assert_allclose(result.cpu().numpy(), expected, rtol=1e-4)
+
     def test_multioutput(self):
         device = "cuda" if torch.cuda.is_available() else "cpu:0"
         inputs = torch.ones((1, 6, 20, 20)).to(device=device)
         roi_shape = (8, 8)
         sw_batch_size = 10
 
         def compute(data):
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_sliding_window_splitter.py` & `monai-weekly-1.2.dev2316/tests/test_sliding_window_splitter.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_smartcachedataset.py` & `monai-weekly-1.2.dev2316/tests/test_smartcachedataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_smooth_field.py` & `monai-weekly-1.2.dev2316/tests/test_smooth_field.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_sobel_gradient.py` & `monai-weekly-1.2.dev2316/tests/test_sobel_gradient.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_sobel_gradientd.py` & `monai-weekly-1.2.dev2316/tests/test_sobel_gradientd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_some_of.py` & `monai-weekly-1.2.dev2316/tests/test_some_of.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_spacing.py` & `monai-weekly-1.2.dev2316/tests/test_spacing.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_spacingd.py` & `monai-weekly-1.2.dev2316/tests/test_spacingd.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from monai.data.meta_obj import set_track_meta
 from monai.data.meta_tensor import MetaTensor
 from monai.data.utils import affine_to_spacing
 from monai.transforms import Spacingd
 from monai.utils import ensure_tuple_rep
 from tests.lazy_transforms_utils import test_resampler_lazy
-from tests.utils import TEST_DEVICES, assert_allclose
+from tests.utils import TEST_DEVICES, assert_allclose, skip_if_quick
 
 TESTS: list[tuple] = []
 for device in TEST_DEVICES:
     TESTS.append(
         (
             "spacing 3d",
             {"image": MetaTensor(torch.ones((2, 10, 15, 20)), affine=torch.eye(4))},
@@ -130,14 +130,15 @@
             assert_allclose(new_spacing, init_param["pixdim"], type_test=False)
             self.assertNotEqual(img.shape, res.shape)
         else:
             self.assertIsInstance(res, torch.Tensor)
             self.assertNotIsInstance(res, MetaTensor)
             self.assertNotEqual(img.shape, res.shape)
 
+    @skip_if_quick
     def test_space_same_shape(self):
         affine_1 = np.array(
             [
                 [1.499277e00, 2.699563e-02, 3.805804e-02, -1.948635e02],
                 [-2.685805e-02, 1.499757e00, -2.635604e-12, 4.438188e01],
                 [-3.805194e-02, -5.999028e-04, 1.499517e00, 4.036536e01],
                 [0.000000e00, 0.000000e00, 0.000000e00, 1.000000e00],
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_spatial_combine_transforms.py` & `monai-weekly-1.2.dev2316/tests/test_spatial_combine_transforms.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_spatial_crop.py` & `monai-weekly-1.2.dev2316/tests/test_spatial_crop.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_spatial_cropd.py` & `monai-weekly-1.2.dev2316/tests/test_spatial_cropd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_spatial_pad.py` & `monai-weekly-1.2.dev2316/tests/test_spatial_pad.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_spatial_padd.py` & `monai-weekly-1.2.dev2316/tests/test_spatial_padd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_spatial_resample.py` & `monai-weekly-1.2.dev2316/tests/test_spatial_resample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_spatial_resampled.py` & `monai-weekly-1.2.dev2316/tests/test_spatial_resampled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_split_channel.py` & `monai-weekly-1.2.dev2316/tests/test_split_channel.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_split_channeld.py` & `monai-weekly-1.2.dev2316/tests/test_split_channeld.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_splitdim.py` & `monai-weekly-1.2.dev2316/tests/test_splitdim.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_splitdimd.py` & `monai-weekly-1.2.dev2316/tests/test_splitdimd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_squeezedim.py` & `monai-weekly-1.2.dev2316/tests/test_squeezedim.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_squeezedimd.py` & `monai-weekly-1.2.dev2316/tests/test_squeezedimd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_ssim_loss.py` & `monai-weekly-1.2.dev2316/tests/test_ssim_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_ssim_metric.py` & `monai-weekly-1.2.dev2316/tests/test_ssim_metric.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_state_cacher.py` & `monai-weekly-1.2.dev2316/tests/test_state_cacher.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_std_shift_intensity.py` & `monai-weekly-1.2.dev2316/tests/test_std_shift_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_std_shift_intensityd.py` & `monai-weekly-1.2.dev2316/tests/test_std_shift_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_str2bool.py` & `monai-weekly-1.2.dev2316/tests/test_str2bool.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_str2list.py` & `monai-weekly-1.2.dev2316/tests/test_str2list.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_subpixel_upsample.py` & `monai-weekly-1.2.dev2316/tests/test_subpixel_upsample.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_surface_dice.py` & `monai-weekly-1.2.dev2316/tests/test_surface_dice.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,75 @@
 
 from monai.metrics.surface_dice import SurfaceDiceMetric
 
 _device = "cuda:0" if torch.cuda.is_available() else "cpu"
 
 
 class TestAllSurfaceDiceMetrics(unittest.TestCase):
+    def test_tolerance_euclidean_distance_with_spacing(self):
+        batch_size = 2
+        n_class = 2
+        test_spacing = (0.85, 1.2)
+        predictions = torch.zeros((batch_size, 480, 640), dtype=torch.int64, device=_device)
+        labels = torch.zeros((batch_size, 480, 640), dtype=torch.int64, device=_device)
+        predictions[0, :, 50:] = 1
+        labels[0, :, 60:] = 1  # 10 px shift
+        predictions_hot = F.one_hot(predictions, num_classes=n_class).permute(0, 3, 1, 2)
+        labels_hot = F.one_hot(labels, num_classes=n_class).permute(0, 3, 1, 2)
+
+        sd0 = SurfaceDiceMetric(class_thresholds=[0, 0], include_background=True)
+        res0 = sd0(predictions_hot, labels_hot, spacing=test_spacing)
+        agg0 = sd0.aggregate()  # aggregation: nanmean across image then nanmean across batch
+        sd0_nans = SurfaceDiceMetric(class_thresholds=[0, 0], include_background=True, get_not_nans=True)
+        res0_nans = sd0_nans(predictions_hot, labels_hot)
+        agg0_nans, not_nans = sd0_nans.aggregate()
+
+        np.testing.assert_array_equal(res0.cpu(), res0_nans.cpu())
+        np.testing.assert_equal(res0.device, predictions.device)
+        np.testing.assert_array_equal(agg0.cpu(), agg0_nans.cpu())
+        np.testing.assert_equal(agg0.device, predictions.device)
+
+        res1 = SurfaceDiceMetric(class_thresholds=[1, 1], include_background=True)(
+            predictions_hot, labels_hot, spacing=test_spacing
+        )
+        res9 = SurfaceDiceMetric(class_thresholds=[9, 9], include_background=True)(
+            predictions_hot, labels_hot, spacing=test_spacing
+        )
+        res10 = SurfaceDiceMetric(class_thresholds=[10, 10], include_background=True)(
+            predictions_hot, labels_hot, spacing=test_spacing
+        )
+        res11 = SurfaceDiceMetric(class_thresholds=[11, 11], include_background=True)(
+            predictions_hot, labels_hot, spacing=test_spacing
+        )
+        # because spacing is (0.85, 1.2) and we moved 10 pixels in the columns direction,
+        # everything with tolerance 12 or more should be the same as tolerance 12 (surface dice is 1.0)
+        res12 = SurfaceDiceMetric(class_thresholds=[12, 12], include_background=True)(
+            predictions_hot, labels_hot, spacing=test_spacing
+        )
+        res13 = SurfaceDiceMetric(class_thresholds=[13, 13], include_background=True)(
+            predictions_hot, labels_hot, spacing=test_spacing
+        )
+
+        for res in [res0, res9, res10, res11, res12, res13]:
+            assert res.shape == torch.Size([2, 2])
+
+        assert res0[0, 0] < res1[0, 0] < res9[0, 0] < res10[0, 0] < res11[0, 0]
+        assert res0[0, 1] < res1[0, 1] < res9[0, 1] < res10[0, 1] < res11[0, 1]
+        np.testing.assert_array_equal(res12.cpu(), res13.cpu())
+
+        expected_res0 = np.zeros((batch_size, n_class))
+        expected_res0[0, 1] = 1 - (478 + 480 + 9 * 2) / (480 * 4 + 588 * 2 + 578 * 2)
+        expected_res0[0, 0] = 1 - (478 + 480 + 9 * 2) / (480 * 4 + 48 * 2 + 58 * 2)
+        expected_res0[1, 0] = 1
+        expected_res0[1, 1] = np.nan
+        for b, c in np.ndindex(batch_size, n_class):
+            np.testing.assert_allclose(expected_res0[b, c], res0[b, c].cpu())
+        np.testing.assert_array_equal(agg0.cpu(), np.nanmean(np.nanmean(expected_res0, axis=1), axis=0))
+        np.testing.assert_equal(not_nans.cpu(), torch.tensor(2))
+
     def test_tolerance_euclidean_distance(self):
         batch_size = 2
         n_class = 2
         predictions = torch.zeros((batch_size, 480, 640), dtype=torch.int64, device=_device)
         labels = torch.zeros((batch_size, 480, 640), dtype=torch.int64, device=_device)
         predictions[0, :, 50:] = 1
         labels[0, :, 60:] = 1  # 10 px shift
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_surface_distance.py` & `monai-weekly-1.2.dev2316/tests/test_hausdorff_distance.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,135 +13,184 @@
 
 import unittest
 
 import numpy as np
 import torch
 from parameterized import parameterized
 
-from monai.metrics import SurfaceDistanceMetric
+from monai.metrics import HausdorffDistanceMetric
 
 _device = "cuda:0" if torch.cuda.is_available() else "cpu"
 
 
 def create_spherical_seg_3d(
-    radius: float = 20.0, centre: tuple[int, int, int] = (49, 49, 49), im_shape: tuple[int, int, int] = (99, 99, 99)
+    radius: float = 20.0,
+    centre: tuple[int, int, int] = (49, 49, 49),
+    im_shape: tuple[int, int, int] = (99, 99, 99),
+    im_spacing: tuple[float, float, float] = (1.0, 1.0, 1.0),
 ) -> np.ndarray:
     """
     Return a 3D image with a sphere inside. Voxel values will be
     1 inside the sphere, and 0 elsewhere.
 
     Args:
         radius: radius of sphere (in terms of number of voxels, can be partial)
         centre: location of sphere centre.
-        im_shape: shape of image to create
+        im_shape: shape of image to create.
+        im_spacing: spacing of image to create.
 
     See also:
         :py:meth:`~create_test_image_3d`
     """
     # Create image
     image = np.zeros(im_shape, dtype=np.int32)
-    spy, spx, spz = np.ogrid[
-        -centre[0] : im_shape[0] - centre[0], -centre[1] : im_shape[1] - centre[1], -centre[2] : im_shape[2] - centre[2]
-    ]
+    spy, spx, spz = np.ogrid[: im_shape[0], : im_shape[1], : im_shape[2]]
+    spy = spy.astype(float) * im_spacing[0]
+    spx = spx.astype(float) * im_spacing[1]
+    spz = spz.astype(float) * im_spacing[2]
+
+    spy -= centre[0]
+    spx -= centre[1]
+    spz -= centre[2]
+
     circle = (spx * spx + spy * spy + spz * spz) <= radius * radius
 
     image[circle] = 1
     image[~circle] = 0
     return image
 
 
+test_spacing = (0.85, 1.2, 0.9)
 TEST_CASES = [
-    [[create_spherical_seg_3d(), create_spherical_seg_3d()], [0, 0]],
+    [[create_spherical_seg_3d(), create_spherical_seg_3d(), None, 1], [0, 0, 0, 0, 0, 0]],
     [
         [
             create_spherical_seg_3d(radius=20, centre=(20, 20, 20)),
             create_spherical_seg_3d(radius=20, centre=(19, 19, 19)),
-            "taxicab",
+            None,
         ],
-        [1.0380029806259314, 1.0380029806259314],
+        [1.7320508075688772, 1.7320508075688772, 1, 1, 3, 3],
     ],
     [
         [
             create_spherical_seg_3d(radius=33, centre=(19, 33, 22)),
             create_spherical_seg_3d(radius=33, centre=(20, 33, 22)),
+            None,
         ],
-        [0.350217, 0.3483278807706289],
+        [1, 1, 1, 1, 1, 1],
     ],
     [
         [
             create_spherical_seg_3d(radius=20, centre=(20, 33, 22)),
             create_spherical_seg_3d(radius=40, centre=(20, 33, 22)),
+            None,
         ],
-        [15.117741, 12.040033513150455],
+        [20.09975124224178, 20.223748416156685, 15, 20, 24, 35],
     ],
     [
         [
-            create_spherical_seg_3d(radius=20, centre=(20, 33, 22)),
+            # pred does not have foreground (but gt has), the metric should be inf
+            np.zeros([99, 99, 99]),
             create_spherical_seg_3d(radius=40, centre=(20, 33, 22)),
-            "chessboard",
+            None,
+        ],
+        [np.inf, np.inf, np.inf, np.inf, np.inf, np.inf],
+    ],
+    [
+        [
+            # gt does not have foreground (but pred has), the metric should be inf
+            create_spherical_seg_3d(),
+            np.zeros([99, 99, 99]),
+            None,
         ],
-        [11.492719, 9.605067064083457],
+        [np.inf, np.inf, np.inf, np.inf, np.inf, np.inf],
     ],
     [
         [
             create_spherical_seg_3d(radius=20, centre=(20, 33, 22)),
             create_spherical_seg_3d(radius=40, centre=(20, 33, 22)),
-            "taxicab",
+            None,
+            95,
+        ],
+        [19.924858845171276, 20.09975124224178, 14, 18, 22, 33],
+    ],
+    [
+        [
+            create_spherical_seg_3d(radius=20, centre=(20, 20, 20), im_spacing=test_spacing),
+            create_spherical_seg_3d(radius=20, centre=(19, 19, 19), im_spacing=test_spacing),
+            test_spacing,
         ],
-        [20.214613, 12.432687531048186],
+        [2.0808651447296143, 2.2671568, 2, 2, 3, 4],
+    ],
+    [
+        [
+            create_spherical_seg_3d(radius=15, centre=(20, 33, 22), im_spacing=test_spacing),
+            create_spherical_seg_3d(radius=30, centre=(20, 33, 22), im_spacing=test_spacing),
+            test_spacing,
+        ],
+        [15.439640998840332, 15.62594, 11, 17, 20, 28],
     ],
-    [[np.zeros([99, 99, 99]), create_spherical_seg_3d(radius=40, centre=(20, 33, 22))], [np.inf, np.inf]],
-    [[create_spherical_seg_3d(), np.zeros([99, 99, 99]), "taxicab"], [np.inf, np.inf]],
 ]
 
 TEST_CASES_NANS = [
     [
         [
+            # both pred and gt do not have foreground, spacing is None, metric and not_nans should be 0
+            np.zeros([99, 99, 99]),
+            np.zeros([99, 99, 99]),
+            None,
+        ]
+    ],
+    [
+        [
             # both pred and gt do not have foreground, metric and not_nans should be 0
             np.zeros([99, 99, 99]),
             np.zeros([99, 99, 99]),
+            test_spacing,
         ]
-    ]
+    ],
 ]
 
 
-class TestAllSurfaceMetrics(unittest.TestCase):
+class TestHausdorffDistance(unittest.TestCase):
     @parameterized.expand(TEST_CASES)
     def test_value(self, input_data, expected_value):
-        if len(input_data) == 3:
-            [seg_1, seg_2, metric] = input_data
+        percentile = None
+        if len(input_data) == 4:
+            [seg_1, seg_2, spacing, percentile] = input_data
         else:
-            [seg_1, seg_2] = input_data
-            metric = "euclidean"
+            [seg_1, seg_2, spacing] = input_data
         ct = 0
         seg_1 = torch.tensor(seg_1, device=_device)
         seg_2 = torch.tensor(seg_2, device=_device)
-        for symmetric in [True, False]:
-            sur_metric = SurfaceDistanceMetric(include_background=False, symmetric=symmetric, distance_metric=metric)
-            # shape of seg_1, seg_2 are: HWD, converts to BNHWD
-            batch, n_class = 2, 3
-            batch_seg_1 = seg_1.unsqueeze(0).unsqueeze(0).repeat([batch, n_class, 1, 1, 1])
-            batch_seg_2 = seg_2.unsqueeze(0).unsqueeze(0).repeat([batch, n_class, 1, 1, 1])
-            sur_metric(batch_seg_1, batch_seg_2)
-            result = sur_metric.aggregate()
-            expected_value_curr = expected_value[ct]
-            np.testing.assert_allclose(expected_value_curr, result.cpu(), rtol=1e-5)
-            np.testing.assert_equal(result.device, seg_1.device)
-            ct += 1
+        for metric in ["euclidean", "chessboard", "taxicab"]:
+            for directed in [True, False]:
+                hd_metric = HausdorffDistanceMetric(
+                    include_background=False, distance_metric=metric, percentile=percentile, directed=directed
+                )
+                # shape of seg_1, seg_2 are: HWD, converts to BNHWD
+                batch, n_class = 2, 3
+                batch_seg_1 = seg_1.unsqueeze(0).unsqueeze(0).repeat([batch, n_class, 1, 1, 1])
+                batch_seg_2 = seg_2.unsqueeze(0).unsqueeze(0).repeat([batch, n_class, 1, 1, 1])
+                hd_metric(batch_seg_1, batch_seg_2, spacing=spacing)
+                result = hd_metric.aggregate(reduction="mean")
+                expected_value_curr = expected_value[ct]
+                np.testing.assert_allclose(expected_value_curr, result.cpu(), rtol=1e-7)
+                np.testing.assert_equal(result.device, seg_1.device)
+                ct += 1
 
     @parameterized.expand(TEST_CASES_NANS)
     def test_nans(self, input_data):
-        [seg_1, seg_2] = input_data
+        [seg_1, seg_2, spacing] = input_data
         seg_1 = torch.tensor(seg_1)
         seg_2 = torch.tensor(seg_2)
-        sur_metric = SurfaceDistanceMetric(include_background=False, get_not_nans=True)
-        # test list of channel-first Tensor
-        batch_seg_1 = [seg_1.unsqueeze(0)]
-        batch_seg_2 = [seg_2.unsqueeze(0)]
-        sur_metric(batch_seg_1, batch_seg_2)
-        result, not_nans = sur_metric.aggregate(reduction="mean")
-        np.testing.assert_allclose(0, result, rtol=1e-5)
-        np.testing.assert_allclose(0, not_nans, rtol=1e-5)
+        hd_metric = HausdorffDistanceMetric(include_background=False, get_not_nans=True)
+        batch_seg_1 = seg_1.unsqueeze(0).unsqueeze(0)
+        batch_seg_2 = seg_2.unsqueeze(0).unsqueeze(0)
+        hd_metric(batch_seg_1, batch_seg_2, spacing=spacing)
+        result, not_nans = hd_metric.aggregate()
+        np.testing.assert_allclose(0, result, rtol=1e-7)
+        np.testing.assert_allclose(0, not_nans, rtol=1e-7)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_swin_unetr.py` & `monai-weekly-1.2.dev2316/tests/test_swin_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_synthetic.py` & `monai-weekly-1.2.dev2316/tests/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_tciadataset.py` & `monai-weekly-1.2.dev2316/tests/test_tciadataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_testtimeaugmentation.py` & `monai-weekly-1.2.dev2316/tests/test_testtimeaugmentation.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_thread_buffer.py` & `monai-weekly-1.2.dev2316/tests/test_thread_buffer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_threadcontainer.py` & `monai-weekly-1.2.dev2316/tests/test_threadcontainer.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_threshold_intensity.py` & `monai-weekly-1.2.dev2316/tests/test_threshold_intensity.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_threshold_intensityd.py` & `monai-weekly-1.2.dev2316/tests/test_threshold_intensityd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_timedcall_dist.py` & `monai-weekly-1.2.dev2316/tests/test_timedcall_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_to_contiguous.py` & `monai-weekly-1.2.dev2316/tests/test_to_contiguous.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_to_cupy.py` & `monai-weekly-1.2.dev2316/tests/test_to_cupy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_to_cupyd.py` & `monai-weekly-1.2.dev2316/tests/test_to_cupyd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_to_device.py` & `monai-weekly-1.2.dev2316/tests/test_to_device.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_to_deviced.py` & `monai-weekly-1.2.dev2316/tests/test_to_deviced.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_to_from_meta_tensord.py` & `monai-weekly-1.2.dev2316/tests/test_to_from_meta_tensord.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_to_numpy.py` & `monai-weekly-1.2.dev2316/tests/test_to_numpy.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_to_numpyd.py` & `monai-weekly-1.2.dev2316/tests/test_to_numpyd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_to_onehot.py` & `monai-weekly-1.2.dev2316/tests/test_to_onehot.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_to_pil.py` & `monai-weekly-1.2.dev2316/tests/test_to_pil.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_to_pild.py` & `monai-weekly-1.2.dev2316/tests/test_to_pild.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_to_tensor.py` & `monai-weekly-1.2.dev2316/tests/test_to_tensor.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_to_tensord.py` & `monai-weekly-1.2.dev2316/tests/test_to_tensord.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_torchscript_utils.py` & `monai-weekly-1.2.dev2316/tests/test_torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_torchvision.py` & `monai-weekly-1.2.dev2316/tests/test_torchvision.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_torchvision_fc_model.py` & `monai-weekly-1.2.dev2316/tests/test_torchvision_fc_model.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_torchvisiond.py` & `monai-weekly-1.2.dev2316/tests/test_torchvisiond.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_traceable_transform.py` & `monai-weekly-1.2.dev2316/tests/test_traceable_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_train_mode.py` & `monai-weekly-1.2.dev2316/tests/test_train_mode.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_trainable_bilateral.py` & `monai-weekly-1.2.dev2316/tests/test_trainable_bilateral.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_trainable_joint_bilateral.py` & `monai-weekly-1.2.dev2316/tests/test_trainable_joint_bilateral.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import numpy as np
 import torch
 from parameterized import parameterized
 from torch.autograd import gradcheck
 
 from monai.networks.layers.filtering import TrainableJointBilateralFilterFunction
-from tests.utils import skip_if_no_cpp_extension, skip_if_no_cuda
+from tests.utils import skip_if_no_cpp_extension, skip_if_no_cuda, skip_if_quick
 
 TEST_CASES = [
     [
         # Case Description
         "1 dimension, 1 channel, low spatial sigmas, low color sigma",
         # (sigma_x, sigma_y, sigma_z, color_sigma)
         (1.0, 1.0, 1.0, 0.2),
@@ -352,14 +352,15 @@
             ]
         ],
     ],
 ]
 
 
 @skip_if_no_cpp_extension
+@skip_if_quick
 class JointBilateralFilterTestCaseCpuPrecise(unittest.TestCase):
     @parameterized.expand(TEST_CASES)
     def test_cpu_precise(self, test_case_description, sigmas, input, guide, expected):
         # Params to determine the implementation to test
         device = torch.device("cpu")
 
         # Create input tensor and apply filter
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_transchex.py` & `monai-weekly-1.2.dev2316/tests/test_transchex.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_transform.py` & `monai-weekly-1.2.dev2316/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_transpose.py` & `monai-weekly-1.2.dev2316/tests/test_transpose.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_transposed.py` & `monai-weekly-1.2.dev2316/tests/test_transposed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_tversky_loss.py` & `monai-weekly-1.2.dev2316/tests/test_tversky_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_unet.py` & `monai-weekly-1.2.dev2316/tests/test_unet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_unetr.py` & `monai-weekly-1.2.dev2316/tests/test_unetr.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_unetr_block.py` & `monai-weekly-1.2.dev2316/tests/test_unetr_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_unified_focal_loss.py` & `monai-weekly-1.2.dev2316/tests/test_unified_focal_loss.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_upsample_block.py` & `monai-weekly-1.2.dev2316/tests/test_upsample_block.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_utils_pytorch_numpy_unification.py` & `monai-weekly-1.2.dev2316/tests/test_utils_pytorch_numpy_unification.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_varautoencoder.py` & `monai-weekly-1.2.dev2316/tests/test_varautoencoder.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_varnet.py` & `monai-weekly-1.2.dev2316/tests/test_varnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_version_leq.py` & `monai-weekly-1.2.dev2316/tests/test_version_leq.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_video_datasets.py` & `monai-weekly-1.2.dev2316/tests/test_video_datasets.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_vis_cam.py` & `monai-weekly-1.2.dev2316/tests/test_vis_cam.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_vis_gradbased.py` & `monai-weekly-1.2.dev2316/tests/test_vis_gradbased.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_vis_gradcam.py` & `monai-weekly-1.2.dev2316/tests/test_vis_gradcam.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_vit.py` & `monai-weekly-1.2.dev2316/tests/test_vit.py`

 * *Files 10% similar despite different names*

```diff
@@ -146,10 +146,29 @@
         net.eval()
         with torch.no_grad():
             torch.jit.script(net)
 
         test_data = torch.randn(input_shape)
         test_script_save(net, test_data)
 
+    def test_access_attn_matrix(self):
+        # input format
+        in_channels = 1
+        img_size = (96, 96, 96)
+        patch_size = (16, 16, 16)
+        in_shape = (1, in_channels, img_size[0], img_size[1], img_size[2])
+
+        # no data in the matrix
+        no_matrix_acess_blk = ViT(in_channels=in_channels, img_size=img_size, patch_size=patch_size)
+        no_matrix_acess_blk(torch.randn(in_shape))
+        assert type(no_matrix_acess_blk.blocks[0].attn.att_mat) == torch.Tensor
+        # no of elements is zero
+        assert no_matrix_acess_blk.blocks[0].attn.att_mat.nelement() == 0
+
+        # be able to acess the attention matrix
+        matrix_acess_blk = ViT(in_channels=in_channels, img_size=img_size, patch_size=patch_size, save_attn=True)
+        matrix_acess_blk(torch.randn(in_shape))
+        assert matrix_acess_blk.blocks[0].attn.att_mat.shape == (in_shape[0], 12, 216, 216)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_vitautoenc.py` & `monai-weekly-1.2.dev2316/tests/test_vitautoenc.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_vnet.py` & `monai-weekly-1.2.dev2316/tests/test_vnet.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_vote_ensemble.py` & `monai-weekly-1.2.dev2316/tests/test_vote_ensemble.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_vote_ensembled.py` & `monai-weekly-1.2.dev2316/tests/test_vote_ensembled.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_warp.py` & `monai-weekly-1.2.dev2316/tests/test_warp.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_watershed.py` & `monai-weekly-1.2.dev2316/tests/test_watershed.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_watershedd.py` & `monai-weekly-1.2.dev2316/tests/test_watershedd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_weight_init.py` & `monai-weekly-1.2.dev2316/tests/test_weight_init.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_weighted_random_sampler_dist.py` & `monai-weekly-1.2.dev2316/tests/test_weighted_random_sampler_dist.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_with_allow_missing_keys.py` & `monai-weekly-1.2.dev2316/tests/test_with_allow_missing_keys.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_write_metrics_reports.py` & `monai-weekly-1.2.dev2316/tests/test_write_metrics_reports.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_wsireader.py` & `monai-weekly-1.2.dev2316/tests/test_wsireader.py`

 * *Files 24% similar despite different names*

```diff
@@ -31,159 +31,271 @@
 cucim, has_cucim = optional_import("cucim")
 has_cucim = has_cucim and hasattr(cucim, "CuImage")
 openslide, has_osl = optional_import("openslide")
 imwrite, has_tiff = optional_import("tifffile", name="imwrite")
 _, has_codec = optional_import("imagecodecs")
 has_tiff = has_tiff and has_codec
 
-FILE_KEY = "wsi_img"
-FILE_URL = testing_data_config("images", FILE_KEY, "url")
-base_name, extension = os.path.basename(f"{FILE_URL}"), ".tiff"
-FILE_PATH = os.path.join(os.path.dirname(__file__), "testing_data", "temp_" + base_name + extension)
+WSI_GENERIC_TIFF_KEY = "wsi_generic_tiff"
+WSI_GENERIC_TIFF_PATH = os.path.join(os.path.dirname(__file__), "testing_data", f"temp_{WSI_GENERIC_TIFF_KEY}.tiff")
 
-HEIGHT = 32914
-WIDTH = 46000
+WSI_APERIO_SVS_KEY = "wsi_aperio_svs"
+WSI_APERIO_SVS_PATH = os.path.join(os.path.dirname(__file__), "testing_data", f"temp_{WSI_APERIO_SVS_KEY}.svs")
 
-TEST_CASE_WHOLE_0 = [FILE_PATH, 2, (3, HEIGHT // 4, WIDTH // 4)]
+WSI_GENERIC_TIFF_HEIGHT = 32914
+WSI_GENERIC_TIFF_WIDTH = 46000
 
-TEST_CASE_TRANSFORM_0 = [FILE_PATH, 4, (HEIGHT // 16, WIDTH // 16), (1, 3, HEIGHT // 16, WIDTH // 16)]
+TEST_CASE_WHOLE_0 = [WSI_GENERIC_TIFF_PATH, 2, (3, WSI_GENERIC_TIFF_HEIGHT // 4, WSI_GENERIC_TIFF_WIDTH // 4)]
+
+TEST_CASE_TRANSFORM_0 = [
+    WSI_GENERIC_TIFF_PATH,
+    4,
+    (WSI_GENERIC_TIFF_HEIGHT // 16, WSI_GENERIC_TIFF_WIDTH // 16),
+    (1, 3, WSI_GENERIC_TIFF_HEIGHT // 16, WSI_GENERIC_TIFF_WIDTH // 16),
+]
 
 # ----------------------------------------------------------------------------
 # Test cases for reading patches
 # ----------------------------------------------------------------------------
 
 TEST_CASE_0 = [
-    FILE_PATH,
+    WSI_GENERIC_TIFF_PATH,
     {"level": 8, "dtype": None},
     {"location": (0, 0), "size": (2, 1)},
     np.array([[[242], [242]], [[242], [242]], [[242], [242]]], dtype=np.float64),
 ]
 
 TEST_CASE_1 = [
-    FILE_PATH,
+    WSI_GENERIC_TIFF_PATH,
     {},
-    {"location": (HEIGHT // 2, WIDTH // 2), "size": (2, 1), "level": 0},
+    {"location": (WSI_GENERIC_TIFF_HEIGHT // 2, WSI_GENERIC_TIFF_WIDTH // 2), "size": (2, 1), "level": 0},
     np.array([[[246], [246]], [[246], [246]], [[246], [246]]], dtype=np.uint8),
 ]
 
 TEST_CASE_2 = [
-    FILE_PATH,
+    WSI_GENERIC_TIFF_PATH,
     {},
     {"location": (0, 0), "size": (2, 1), "level": 8},
     np.array([[[242], [242]], [[242], [242]], [[242], [242]]], dtype=np.uint8),
 ]
 
 TEST_CASE_3 = [
-    FILE_PATH,
+    WSI_GENERIC_TIFF_PATH,
     {"channel_dim": -1},
-    {"location": (HEIGHT // 2, WIDTH // 2), "size": (2, 1), "level": 0},
+    {"location": (WSI_GENERIC_TIFF_HEIGHT // 2, WSI_GENERIC_TIFF_WIDTH // 2), "size": (2, 1), "level": 0},
     np.moveaxis(np.array([[[246], [246]], [[246], [246]], [[246], [246]]], dtype=np.uint8), 0, -1),
 ]
 
 TEST_CASE_4 = [
-    FILE_PATH,
+    WSI_GENERIC_TIFF_PATH,
     {"channel_dim": 2},
     {"location": (0, 0), "size": (2, 1), "level": 8},
     np.moveaxis(np.array([[[242], [242]], [[242], [242]], [[242], [242]]], dtype=np.uint8), 0, -1),
 ]
 
 TEST_CASE_5 = [
-    FILE_PATH,
+    WSI_GENERIC_TIFF_PATH,
     {"level": 8},
     {"location": (0, 0), "size": (2, 1)},
     np.array([[[242], [242]], [[242], [242]], [[242], [242]]], dtype=np.uint8),
 ]
 
 TEST_CASE_6 = [
-    FILE_PATH,
+    WSI_GENERIC_TIFF_PATH,
     {"level": 8, "dtype": np.int32},
     {"location": (0, 0), "size": (2, 1)},
     np.array([[[242], [242]], [[242], [242]], [[242], [242]]], dtype=np.int32),
 ]
 
 TEST_CASE_7 = [
-    FILE_PATH,
+    WSI_GENERIC_TIFF_PATH,
     {"level": 8, "dtype": np.float32},
     {"location": (0, 0), "size": (2, 1)},
     np.array([[[242], [242]], [[242], [242]], [[242], [242]]], dtype=np.float32),
 ]
 
 TEST_CASE_8 = [
-    FILE_PATH,
+    WSI_GENERIC_TIFF_PATH,
     {"level": 8, "dtype": torch.uint8},
     {"location": (0, 0), "size": (2, 1)},
     torch.tensor([[[242], [242]], [[242], [242]], [[242], [242]]], dtype=torch.uint8),
 ]
 
 TEST_CASE_9 = [
-    FILE_PATH,
+    WSI_GENERIC_TIFF_PATH,
     {"level": 8, "dtype": torch.float32},
     {"location": (0, 0), "size": (2, 1)},
     torch.tensor([[[242], [242]], [[242], [242]], [[242], [242]]], dtype=torch.float32),
 ]
 
+# exact mpp in get_data
+TEST_CASE_10_MPP = [
+    WSI_GENERIC_TIFF_PATH,
+    {"mpp_atol": 0.0, "mpp_rtol": 0.0},
+    {"location": (WSI_GENERIC_TIFF_HEIGHT // 2, WSI_GENERIC_TIFF_WIDTH // 2), "size": (2, 1), "mpp": 1000},
+    np.array([[[246], [246]], [[246], [246]], [[246], [246]]], dtype=np.uint8),
+    {"level": 0},
+]
+
+# exact mpp as default
+TEST_CASE_11_MPP = [
+    WSI_GENERIC_TIFF_PATH,
+    {"mpp_atol": 0.0, "mpp_rtol": 0.0, "mpp": 1000},
+    {"location": (WSI_GENERIC_TIFF_HEIGHT // 2, WSI_GENERIC_TIFF_WIDTH // 2), "size": (2, 1)},
+    np.array([[[246], [246]], [[246], [246]], [[246], [246]]], dtype=np.uint8),
+    {"level": 0},
+]
+
+# exact mpp as default (Aperio SVS)
+TEST_CASE_12_MPP = [
+    WSI_APERIO_SVS_PATH,
+    {"mpp_atol": 0.0, "mpp_rtol": 0.0, "mpp": 0.499},
+    {"location": (0, 0), "size": (2, 1)},
+    np.array([[[239], [239]], [[239], [239]], [[239], [239]]], dtype=np.uint8),
+    {"level": 0},
+]
+# acceptable mpp within default tolerances
+TEST_CASE_13_MPP = [
+    WSI_GENERIC_TIFF_PATH,
+    {},
+    {"location": (0, 0), "size": (2, 1), "mpp": 256000},
+    np.array([[[242], [242]], [[242], [242]], [[242], [242]]], dtype=np.uint8),
+    {"level": 8},
+]
+
+# acceptable mpp within default tolerances (Aperio SVS)
+TEST_CASE_14_MPP = [
+    WSI_APERIO_SVS_PATH,
+    {"mpp": 8.0},
+    {"location": (0, 0), "size": (2, 1)},
+    np.array([[[238], [240]], [[239], [241]], [[240], [241]]], dtype=np.uint8),
+    {"level": 2},
+]
+
+# acceptable mpp within absolute tolerance (Aperio SVS)
+TEST_CASE_15_MPP = [
+    WSI_APERIO_SVS_PATH,
+    {"mpp": 7.0, "mpp_atol": 1.0, "mpp_rtol": 0.0},
+    {"location": (0, 0), "size": (2, 1)},
+    np.array([[[238], [240]], [[239], [241]], [[240], [241]]], dtype=np.uint8),
+    {"level": 2},
+]
+
+# acceptable mpp within relative tolerance (Aperio SVS)
+TEST_CASE_16_MPP = [
+    WSI_APERIO_SVS_PATH,
+    {"mpp": 7.8, "mpp_atol": 0.0, "mpp_rtol": 0.1},
+    {"location": (0, 0), "size": (2, 1)},
+    np.array([[[238], [240]], [[239], [241]], [[240], [241]]], dtype=np.uint8),
+    {"level": 2},
+]
+
+# exact power
+TEST_CASE_17_POWER = [
+    WSI_APERIO_SVS_PATH,
+    {"power_atol": 0.0, "power_rtol": 0.0},
+    {"location": (0, 0), "size": (2, 1), "power": 20},
+    np.array([[[239], [239]], [[239], [239]], [[239], [239]]], dtype=np.uint8),
+    {"level": 0},
+]
+
+# exact power
+TEST_CASE_18_POWER = [
+    WSI_APERIO_SVS_PATH,
+    {"power": 20, "power_atol": 0.0, "power_rtol": 0.0},
+    {"location": (0, 0), "size": (2, 1)},
+    np.array([[[239], [239]], [[239], [239]], [[239], [239]]], dtype=np.uint8),
+    {"level": 0},
+]
+
+# acceptable power within default tolerances (Aperio SVS)
+TEST_CASE_19_POWER = [
+    WSI_APERIO_SVS_PATH,
+    {},
+    {"location": (0, 0), "size": (2, 1), "power": 1.25},
+    np.array([[[238], [240]], [[239], [241]], [[240], [241]]], dtype=np.uint8),
+    {"level": 2},
+]
+
+# acceptable power within absolute tolerance (Aperio SVS)
+TEST_CASE_20_POWER = [
+    WSI_APERIO_SVS_PATH,
+    {"power_atol": 0.3, "power_rtol": 0.0},
+    {"location": (0, 0), "size": (2, 1), "power": 1.0},
+    np.array([[[238], [240]], [[239], [241]], [[240], [241]]], dtype=np.uint8),
+    {"level": 2},
+]
+
+# acceptable power within relative tolerance (Aperio SVS)
+TEST_CASE_21_POWER = [
+    WSI_APERIO_SVS_PATH,
+    {"power_atol": 0.0, "power_rtol": 0.3},
+    {"location": (0, 0), "size": (2, 1), "power": 1.0},
+    np.array([[[238], [240]], [[239], [241]], [[240], [241]]], dtype=np.uint8),
+    {"level": 2},
+]
 # device tests
 TEST_CASE_DEVICE_1 = [
-    FILE_PATH,
+    WSI_GENERIC_TIFF_PATH,
     {"level": 8, "dtype": torch.float32, "device": "cpu"},
     {"location": (0, 0), "size": (2, 1)},
     torch.tensor([[[242], [242]], [[242], [242]], [[242], [242]]], dtype=torch.float32),
     "cpu",
 ]
 
 TEST_CASE_DEVICE_2 = [
-    FILE_PATH,
+    WSI_GENERIC_TIFF_PATH,
     {"level": 8, "dtype": torch.float32, "device": "cuda"},
     {"location": (0, 0), "size": (2, 1)},
     torch.tensor([[[242], [242]], [[242], [242]], [[242], [242]]], dtype=torch.float32),
     "cuda",
 ]
 
 TEST_CASE_DEVICE_3 = [
-    FILE_PATH,
+    WSI_GENERIC_TIFF_PATH,
     {"level": 8, "dtype": np.float32, "device": "cpu"},
     {"location": (0, 0), "size": (2, 1)},
     np.array([[[242], [242]], [[242], [242]], [[242], [242]]], dtype=np.float32),
     "cpu",
 ]
 
 TEST_CASE_DEVICE_4 = [
-    FILE_PATH,
+    WSI_GENERIC_TIFF_PATH,
     {"level": 8, "dtype": np.float32, "device": "cuda"},
     {"location": (0, 0), "size": (2, 1)},
     torch.tensor([[[242], [242]], [[242], [242]], [[242], [242]]], dtype=torch.float32),
     "cuda",
 ]
 
 TEST_CASE_DEVICE_5 = [
-    FILE_PATH,
+    WSI_GENERIC_TIFF_PATH,
     {"level": 8, "device": "cuda"},
     {"location": (0, 0), "size": (2, 1)},
     torch.tensor([[[242], [242]], [[242], [242]], [[242], [242]]], dtype=torch.uint8),
     "cuda",
 ]
 
 TEST_CASE_DEVICE_6 = [
-    FILE_PATH,
+    WSI_GENERIC_TIFF_PATH,
     {"level": 8},
     {"location": (0, 0), "size": (2, 1)},
     np.array([[[242], [242]], [[242], [242]], [[242], [242]]], dtype=np.uint8),
     "cpu",
 ]
 
 TEST_CASE_DEVICE_7 = [
-    FILE_PATH,
+    WSI_GENERIC_TIFF_PATH,
     {"level": 8, "device": None},
     {"location": (0, 0), "size": (2, 1)},
     np.array([[[242], [242]], [[242], [242]], [[242], [242]]], dtype=np.uint8),
     "cpu",
 ]
 
 TEST_CASE_MULTI_WSI = [
-    [FILE_PATH, FILE_PATH],
+    [WSI_GENERIC_TIFF_PATH, WSI_GENERIC_TIFF_PATH],
     {"location": (0, 0), "size": (2, 1), "level": 8},
     np.concatenate(
         [
             np.array([[[242], [242]], [[242], [242]], [[242], [242]]]),
             np.array([[[242], [242]], [[242], [242]], [[242], [242]]]),
         ],
         axis=0,
@@ -195,15 +307,42 @@
 TEST_CASE_RGB_1 = [np.ones((3, 100, 100), dtype=np.uint8)]  # CHW
 
 TEST_CASE_ERROR_0C = [np.ones((16, 16), dtype=np.uint8)]  # no color channel
 TEST_CASE_ERROR_1C = [np.ones((16, 16, 1), dtype=np.uint8)]  # one color channel
 TEST_CASE_ERROR_2C = [np.ones((16, 16, 2), dtype=np.uint8)]  # two color channels
 TEST_CASE_ERROR_3D = [np.ones((16, 16, 16, 3), dtype=np.uint8)]  # 3D + color
 
-TEST_CASE_MPP_0 = [FILE_PATH, 0, (1000.0, 1000.0)]
+# mpp not within default
+TEST_CASE_ERROR_0_MPP = [
+    WSI_GENERIC_TIFF_PATH,
+    {},
+    {"location": (WSI_GENERIC_TIFF_HEIGHT // 2, WSI_GENERIC_TIFF_WIDTH // 2), "size": (2, 1), "mpp": 1200},
+    ValueError,
+]
+
+# mpp is not exact (no tolerance)
+TEST_CASE_ERROR_1_MPP = [
+    WSI_APERIO_SVS_PATH,
+    {"mpp_atol": 0.0, "mpp_rtol": 0.0},
+    {"location": (0, 0), "size": (2, 1), "mpp": 8.0},
+    ValueError,
+]
+
+# power not within default
+TEST_CASE_ERROR_2_POWER = [WSI_APERIO_SVS_PATH, {}, {"location": (0, 0), "size": (2, 1), "power": 40}, ValueError]
+
+# power is not exact (no tolerance)
+TEST_CASE_ERROR_3_POWER = [
+    WSI_APERIO_SVS_PATH,
+    {"power_atol": 0.0, "power_rtol": 0.0},
+    {"location": (0, 0), "size": (2, 1), "power": 1.25},
+    ValueError,
+]
+
+TEST_CASE_MPP_0 = [WSI_GENERIC_TIFF_PATH, 0, (1000.0, 1000.0)]
 
 
 def save_rgba_tiff(array: np.ndarray, filename: str, mode: str):
     """
     Save numpy array into a TIFF RGB/RGBA file
 
     Args:
@@ -232,17 +371,26 @@
     imwrite(filename, img_gray, shape=img_gray.shape)
 
     return filename
 
 
 @skipUnless(has_cucim or has_osl or has_tiff, "Requires cucim, openslide, or tifffile!")
 def setUpModule():
-    hash_type = testing_data_config("images", FILE_KEY, "hash_type")
-    hash_val = testing_data_config("images", FILE_KEY, "hash_val")
-    download_url_or_skip_test(FILE_URL, FILE_PATH, hash_type=hash_type, hash_val=hash_val)
+    download_url_or_skip_test(
+        testing_data_config("images", WSI_GENERIC_TIFF_KEY, "url"),
+        WSI_GENERIC_TIFF_PATH,
+        hash_type=testing_data_config("images", WSI_GENERIC_TIFF_KEY, "hash_type"),
+        hash_val=testing_data_config("images", WSI_GENERIC_TIFF_KEY, "hash_val"),
+    )
+    download_url_or_skip_test(
+        testing_data_config("images", WSI_APERIO_SVS_KEY, "url"),
+        WSI_APERIO_SVS_PATH,
+        hash_type=testing_data_config("images", WSI_APERIO_SVS_KEY, "hash_type"),
+        hash_val=testing_data_config("images", WSI_APERIO_SVS_KEY, "hash_val"),
+    )
 
 
 class WSIReaderTests:
     class Tests(unittest.TestCase):
         backend = None
 
         @parameterized.expand([TEST_CASE_WHOLE_0])
@@ -265,21 +413,36 @@
                 TEST_CASE_3,
                 TEST_CASE_4,
                 TEST_CASE_5,
                 TEST_CASE_6,
                 TEST_CASE_7,
                 TEST_CASE_8,
                 TEST_CASE_9,
+                TEST_CASE_10_MPP,
+                TEST_CASE_11_MPP,
+                TEST_CASE_12_MPP,
+                TEST_CASE_13_MPP,
+                TEST_CASE_14_MPP,
+                TEST_CASE_15_MPP,
+                TEST_CASE_16_MPP,
+                TEST_CASE_17_POWER,
+                TEST_CASE_18_POWER,
+                TEST_CASE_19_POWER,
+                TEST_CASE_20_POWER,
+                TEST_CASE_21_POWER,
             ]
         )
-        def test_read_region(self, file_path, kwargs, patch_info, expected_img):
-            reader = WSIReader(self.backend, **kwargs)
-            level = patch_info.get("level", kwargs.get("level"))
-            if self.backend == "tifffile" and level < 2:
+        def test_read_region(self, file_path, reader_kwargs, patch_info, expected_img, *args):
+            reader = WSIReader(self.backend, **reader_kwargs)
+            level = patch_info.get("level", reader_kwargs.get("level"))
+            # Skip mpp, power tests for TiffFile backend
+            if self.backend == "tifffile" and (level is None or level < 2 or file_path == WSI_APERIO_SVS_PATH):
                 return
+            if level is None:
+                level = args[0].get("level")
             with reader.read(file_path) as img_obj:
                 # Read twice to check multiple calls
                 img, meta = reader.get_data(img_obj, **patch_info)
                 img2 = reader.get_data(img_obj, **patch_info)[0]
             self.assertTupleEqual(img.shape, img2.shape)
             assert_allclose(img, img2)
             self.assertTupleEqual(img.shape, expected_img.shape)
@@ -449,14 +612,23 @@
                 self.assertEqual("cpu", device)
             self.assertEqual(meta["backend"], self.backend)
             self.assertEqual(meta[WSIPatchKeys.PATH].lower(), str(os.path.abspath(file_path)).lower())
             self.assertEqual(meta[WSIPatchKeys.LEVEL], level)
             assert_allclose(meta[WSIPatchKeys.SIZE], patch_info["size"], type_test=False)
             assert_allclose(meta[WSIPatchKeys.LOCATION], patch_info["location"], type_test=False)
 
+        @parameterized.expand(
+            [TEST_CASE_ERROR_0_MPP, TEST_CASE_ERROR_1_MPP, TEST_CASE_ERROR_2_POWER, TEST_CASE_ERROR_3_POWER]
+        )
+        def test_errors(self, file_path, reader_kwargs, patch_info, exception):
+            with self.assertRaises(exception):
+                reader = WSIReader(self.backend, **reader_kwargs)
+                with reader.read(file_path) as img_obj:
+                    reader.get_data(img_obj, **patch_info)
+
 
 @skipUnless(has_cucim, "Requires cucim")
 class TestCuCIM(WSIReaderTests.Tests):
     @classmethod
     def setUpClass(cls):
         cls.backend = "cucim"
```

### Comparing `monai-weekly-1.2.dev2315/tests/test_zipdataset.py` & `monai-weekly-1.2.dev2316/tests/test_zipdataset.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_zoom.py` & `monai-weekly-1.2.dev2316/tests/test_zoom.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_zoom_affine.py` & `monai-weekly-1.2.dev2316/tests/test_zoom_affine.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/tests/test_zoomd.py` & `monai-weekly-1.2.dev2316/tests/test_zoomd.py`

 * *Files identical despite different names*

### Comparing `monai-weekly-1.2.dev2315/versioneer.py` & `monai-weekly-1.2.dev2316/versioneer.py`

 * *Files identical despite different names*

