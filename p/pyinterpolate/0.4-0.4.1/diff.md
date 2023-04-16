# Comparing `tmp/pyinterpolate-0.4.tar.gz` & `tmp/pyinterpolate-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyinterpolate-0.4.tar", last modified: Thu Apr  6 10:00:28 2023, max compression
+gzip compressed data, was "pyinterpolate-0.4.1.tar", last modified: Sun Apr 16 09:56:38 2023, max compression
```

## Comparing `pyinterpolate-0.4.tar` & `pyinterpolate-0.4.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.885621 pyinterpolate-0.4/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)       42 2021-10-17 13:15:38.000000 pyinterpolate-0.4/MANIFEST.in
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     9656 2023-04-06 10:00:28.885621 pyinterpolate-0.4/PKG-INFO
--rwxrwxr-x   0 szymon    (1000) szymon    (1000)     8652 2023-04-06 09:25:45.000000 pyinterpolate-0.4/README.md
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.873621 pyinterpolate-0.4/pyinterpolate/
--rwxrwxr-x   0 szymon    (1000) szymon    (1000)     1442 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/__init__.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.873621 pyinterpolate-0.4/pyinterpolate/distance/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      187 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/distance/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     7804 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/distance/clusters.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    11000 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/distance/distance.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     6216 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/distance/gridding.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.873621 pyinterpolate-0.4/pyinterpolate/idw/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)       60 2022-09-07 20:00:15.000000 pyinterpolate-0.4/pyinterpolate/idw/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     3507 2022-10-08 09:51:45.000000 pyinterpolate-0.4/pyinterpolate/idw/idw.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.873621 pyinterpolate-0.4/pyinterpolate/io/
--rwxrwxr-x   0 szymon    (1000) szymon    (1000)       70 2022-09-07 20:00:15.000000 pyinterpolate-0.4/pyinterpolate/io/__init__.py
--rwxrwxr-x   0 szymon    (1000) szymon    (1000)     5946 2022-10-08 09:51:45.000000 pyinterpolate-0.4/pyinterpolate/io/read_data.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.873621 pyinterpolate-0.4/pyinterpolate/kriging/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      595 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/kriging/__init__.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.873621 pyinterpolate-0.4/pyinterpolate/kriging/models/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4/pyinterpolate/kriging/models/__init__.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.877621 pyinterpolate-0.4/pyinterpolate/kriging/models/block/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      187 2022-09-07 20:00:15.000000 pyinterpolate-0.4/pyinterpolate/kriging/models/block/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     7711 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/kriging/models/block/area_to_area_poisson_kriging.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     9806 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/kriging/models/block/area_to_point_poisson_kriging.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     7405 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/kriging/models/block/centroid_based_poisson_kriging.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    10644 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/kriging/models/block/weight.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.877621 pyinterpolate-0.4/pyinterpolate/kriging/models/indicator/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/kriging/models/indicator/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    13128 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/kriging/models/indicator/indicator_point_kriging.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.877621 pyinterpolate-0.4/pyinterpolate/kriging/models/point/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4/pyinterpolate/kriging/models/point/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     6965 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/kriging/models/point/ordinary_kriging.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     3766 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/kriging/models/point/simple_kriging.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.877621 pyinterpolate-0.4/pyinterpolate/kriging/models/structures/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/kriging/models/structures/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      687 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/kriging/models/structures/point_kriging.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     7666 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/kriging/point_kriging.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.877621 pyinterpolate-0.4/pyinterpolate/kriging/utils/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4/pyinterpolate/kriging/utils/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1078 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/kriging/utils/kwarnings.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     4870 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/kriging/utils/process.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.877621 pyinterpolate-0.4/pyinterpolate/pipelines/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      246 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/pipelines/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    13437 2022-10-08 09:51:45.000000 pyinterpolate-0.4/pyinterpolate/pipelines/block_filtering.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     5227 2022-11-05 20:50:31.000000 pyinterpolate-0.4/pyinterpolate/pipelines/deconvolution.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    12890 2022-10-08 09:51:45.000000 pyinterpolate-0.4/pyinterpolate/pipelines/multi_kriging.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.877621 pyinterpolate-0.4/pyinterpolate/processing/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)       79 2022-09-07 20:00:15.000000 pyinterpolate-0.4/pyinterpolate/processing/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     2543 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/processing/checks.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.877621 pyinterpolate-0.4/pyinterpolate/processing/preprocessing/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4/pyinterpolate/processing/preprocessing/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    17173 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/processing/preprocessing/blocks.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    36344 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/processing/select_values.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.877621 pyinterpolate-0.4/pyinterpolate/processing/transform/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4/pyinterpolate/processing/transform/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     5490 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/processing/transform/statistics.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    11202 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/processing/transform/transform.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.877621 pyinterpolate-0.4/pyinterpolate/processing/utils/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4/pyinterpolate/processing/utils/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1802 2022-11-05 20:50:31.000000 pyinterpolate-0.4/pyinterpolate/processing/utils/exceptions.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.877621 pyinterpolate-0.4/pyinterpolate/validation/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/validation/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     4079 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/validation/cross_validation.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.877621 pyinterpolate-0.4/pyinterpolate/variogram/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      682 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/variogram/__init__.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.881621 pyinterpolate-0.4/pyinterpolate/variogram/empirical/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1857 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/variogram/empirical/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    23322 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/variogram/empirical/cloud.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    10720 2022-12-24 08:14:03.000000 pyinterpolate-0.4/pyinterpolate/variogram/empirical/covariance.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    25423 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/variogram/empirical/experimental_variogram.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    23469 2022-12-24 08:14:03.000000 pyinterpolate-0.4/pyinterpolate/variogram/empirical/semivariance.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.881621 pyinterpolate-0.4/pyinterpolate/variogram/indicator/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/variogram/indicator/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    16462 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/variogram/indicator/indicator_variogram.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.881621 pyinterpolate-0.4/pyinterpolate/variogram/regularization/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:16.000000 pyinterpolate-0.4/pyinterpolate/variogram/regularization/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    24569 2022-12-24 08:14:03.000000 pyinterpolate-0.4/pyinterpolate/variogram/regularization/aggregated.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.881621 pyinterpolate-0.4/pyinterpolate/variogram/regularization/block/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:16.000000 pyinterpolate-0.4/pyinterpolate/variogram/regularization/block/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1489 2022-10-09 07:47:16.000000 pyinterpolate-0.4/pyinterpolate/variogram/regularization/block/avg_block_to_block_semivariances.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     4047 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/variogram/regularization/block/avg_inblock_semivariances.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     5343 2022-10-09 07:47:16.000000 pyinterpolate-0.4/pyinterpolate/variogram/regularization/block/block_to_block_semivariance.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     8847 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/variogram/regularization/block/inblock_semivariance.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    33508 2022-12-24 08:14:03.000000 pyinterpolate-0.4/pyinterpolate/variogram/regularization/deconvolution.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.881621 pyinterpolate-0.4/pyinterpolate/variogram/theoretical/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     5340 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/variogram/theoretical/__init__.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.881621 pyinterpolate-0.4/pyinterpolate/variogram/theoretical/models/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)       31 2022-09-07 20:00:16.000000 pyinterpolate-0.4/pyinterpolate/variogram/theoretical/models/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     8319 2022-09-07 20:00:16.000000 pyinterpolate-0.4/pyinterpolate/variogram/theoretical/models/variogram_models.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)    36064 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/variogram/theoretical/semivariogram.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     1140 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/variogram/theoretical/spatial_dependency_index.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.885621 pyinterpolate-0.4/pyinterpolate/variogram/utils/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:16.000000 pyinterpolate-0.4/pyinterpolate/variogram/utils/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     6340 2022-11-05 20:50:31.000000 pyinterpolate-0.4/pyinterpolate/variogram/utils/exceptions.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     9500 2022-09-07 20:00:16.000000 pyinterpolate-0.4/pyinterpolate/variogram/utils/metrics.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     2046 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/variogram/utils/plots.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.885621 pyinterpolate-0.4/pyinterpolate/viz/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)       55 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/viz/__init__.py
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     5348 2023-04-06 09:25:45.000000 pyinterpolate-0.4/pyinterpolate/viz/raster.py
-drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-06 10:00:28.873621 pyinterpolate-0.4/pyinterpolate.egg-info/
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     9656 2023-04-06 10:00:28.000000 pyinterpolate-0.4/pyinterpolate.egg-info/PKG-INFO
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     3556 2023-04-06 10:00:28.000000 pyinterpolate-0.4/pyinterpolate.egg-info/SOURCES.txt
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        1 2023-04-06 10:00:28.000000 pyinterpolate-0.4/pyinterpolate.egg-info/dependency_links.txt
--rw-rw-r--   0 szymon    (1000) szymon    (1000)        1 2023-04-06 10:00:28.000000 pyinterpolate-0.4/pyinterpolate.egg-info/not-zip-safe
--rw-rw-r--   0 szymon    (1000) szymon    (1000)      884 2023-04-06 10:00:28.000000 pyinterpolate-0.4/pyinterpolate.egg-info/requires.txt
--rw-rw-r--   0 szymon    (1000) szymon    (1000)       14 2023-04-06 10:00:28.000000 pyinterpolate-0.4/pyinterpolate.egg-info/top_level.txt
--rw-rw-r--   0 szymon    (1000) szymon    (1000)       80 2022-09-07 20:00:16.000000 pyinterpolate-0.4/pyproject.toml
--rw-rw-r--   0 szymon    (1000) szymon    (1000)     2184 2023-04-06 10:00:28.885621 pyinterpolate-0.4/setup.cfg
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.065284 pyinterpolate-0.4.1/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)       42 2021-10-17 13:15:38.000000 pyinterpolate-0.4.1/MANIFEST.in
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     9660 2023-04-16 09:56:38.069284 pyinterpolate-0.4.1/PKG-INFO
+-rwxrwxr-x   0 szymon    (1000) szymon    (1000)     8654 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/README.md
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.049284 pyinterpolate-0.4.1/pyinterpolate/
+-rwxrwxr-x   0 szymon    (1000) szymon    (1000)     1442 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/__init__.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.053284 pyinterpolate-0.4.1/pyinterpolate/distance/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      187 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/distance/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     7804 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/distance/clusters.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    11000 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/distance/distance.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     6216 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/distance/gridding.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.053284 pyinterpolate-0.4.1/pyinterpolate/idw/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)       60 2022-09-07 20:00:15.000000 pyinterpolate-0.4.1/pyinterpolate/idw/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     3507 2022-10-08 09:51:45.000000 pyinterpolate-0.4.1/pyinterpolate/idw/idw.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.053284 pyinterpolate-0.4.1/pyinterpolate/io/
+-rwxrwxr-x   0 szymon    (1000) szymon    (1000)       70 2022-09-07 20:00:15.000000 pyinterpolate-0.4.1/pyinterpolate/io/__init__.py
+-rwxrwxr-x   0 szymon    (1000) szymon    (1000)     5946 2022-10-08 09:51:45.000000 pyinterpolate-0.4.1/pyinterpolate/io/read_data.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.053284 pyinterpolate-0.4.1/pyinterpolate/kriging/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      595 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/__init__.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.053284 pyinterpolate-0.4.1/pyinterpolate/kriging/models/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/__init__.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.057284 pyinterpolate-0.4.1/pyinterpolate/kriging/models/block/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      187 2022-09-07 20:00:15.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/block/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     7711 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/block/area_to_area_poisson_kriging.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     9806 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/block/area_to_point_poisson_kriging.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     7405 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/block/centroid_based_poisson_kriging.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    10644 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/block/weight.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.057284 pyinterpolate-0.4.1/pyinterpolate/kriging/models/indicator/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/indicator/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    13128 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/indicator/indicator_point_kriging.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.057284 pyinterpolate-0.4.1/pyinterpolate/kriging/models/point/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/point/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     6965 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/point/ordinary_kriging.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     3766 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/point/simple_kriging.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.057284 pyinterpolate-0.4.1/pyinterpolate/kriging/models/structures/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/structures/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      687 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/models/structures/point_kriging.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     7666 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/point_kriging.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.057284 pyinterpolate-0.4.1/pyinterpolate/kriging/utils/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/utils/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1078 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/utils/kwarnings.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     4870 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/kriging/utils/process.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.057284 pyinterpolate-0.4.1/pyinterpolate/pipelines/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      246 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/pipelines/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    13437 2022-10-08 09:51:45.000000 pyinterpolate-0.4.1/pyinterpolate/pipelines/block_filtering.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     5227 2022-11-05 20:50:31.000000 pyinterpolate-0.4.1/pyinterpolate/pipelines/deconvolution.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    12890 2022-10-08 09:51:45.000000 pyinterpolate-0.4.1/pyinterpolate/pipelines/multi_kriging.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.061284 pyinterpolate-0.4.1/pyinterpolate/processing/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)       79 2022-09-07 20:00:15.000000 pyinterpolate-0.4.1/pyinterpolate/processing/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     2543 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/processing/checks.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.061284 pyinterpolate-0.4.1/pyinterpolate/processing/preprocessing/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4.1/pyinterpolate/processing/preprocessing/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    17173 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/processing/preprocessing/blocks.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    36344 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/processing/select_values.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.061284 pyinterpolate-0.4.1/pyinterpolate/processing/transform/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4.1/pyinterpolate/processing/transform/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     5490 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/processing/transform/statistics.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    11202 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/processing/transform/transform.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.061284 pyinterpolate-0.4.1/pyinterpolate/processing/utils/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:15.000000 pyinterpolate-0.4.1/pyinterpolate/processing/utils/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1802 2022-11-05 20:50:31.000000 pyinterpolate-0.4.1/pyinterpolate/processing/utils/exceptions.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.061284 pyinterpolate-0.4.1/pyinterpolate/validation/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/validation/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     4079 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/validation/cross_validation.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.061284 pyinterpolate-0.4.1/pyinterpolate/variogram/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      682 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/__init__.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.061284 pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1857 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    23322 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/cloud.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    10484 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/covariance.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    24364 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/experimental_variogram.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    23469 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/semivariance.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.061284 pyinterpolate-0.4.1/pyinterpolate/variogram/indicator/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/indicator/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    16428 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/indicator/indicator_variogram.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.061284 pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:16.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    24569 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/aggregated.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.065284 pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/block/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:16.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/block/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1489 2022-10-09 07:47:16.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/block/avg_block_to_block_semivariances.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     4047 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/block/avg_inblock_semivariances.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     5343 2022-10-09 07:47:16.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/block/block_to_block_semivariance.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     8847 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/block/inblock_semivariance.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    33633 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/deconvolution.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.065284 pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     5340 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/__init__.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.065284 pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/models/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)       31 2022-09-07 20:00:16.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/models/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     8319 2022-09-07 20:00:16.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/models/variogram_models.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)    37830 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/semivariogram.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     1140 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/spatial_dependency_index.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.065284 pyinterpolate-0.4.1/pyinterpolate/variogram/utils/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        0 2022-09-07 20:00:16.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/utils/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     6990 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/utils/exceptions.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     9500 2022-09-07 20:00:16.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/utils/metrics.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     2046 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/variogram/utils/plots.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.065284 pyinterpolate-0.4.1/pyinterpolate/viz/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)       55 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/viz/__init__.py
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     5348 2023-04-16 09:55:49.000000 pyinterpolate-0.4.1/pyinterpolate/viz/raster.py
+drwxrwxr-x   0 szymon    (1000) szymon    (1000)        0 2023-04-16 09:56:38.053284 pyinterpolate-0.4.1/pyinterpolate.egg-info/
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     9660 2023-04-16 09:56:38.000000 pyinterpolate-0.4.1/pyinterpolate.egg-info/PKG-INFO
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     3556 2023-04-16 09:56:38.000000 pyinterpolate-0.4.1/pyinterpolate.egg-info/SOURCES.txt
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        1 2023-04-16 09:56:38.000000 pyinterpolate-0.4.1/pyinterpolate.egg-info/dependency_links.txt
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)        1 2023-04-16 09:56:37.000000 pyinterpolate-0.4.1/pyinterpolate.egg-info/not-zip-safe
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)      884 2023-04-16 09:56:38.000000 pyinterpolate-0.4.1/pyinterpolate.egg-info/requires.txt
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)       14 2023-04-16 09:56:38.000000 pyinterpolate-0.4.1/pyinterpolate.egg-info/top_level.txt
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)       80 2022-09-07 20:00:16.000000 pyinterpolate-0.4.1/pyproject.toml
+-rw-rw-r--   0 szymon    (1000) szymon    (1000)     2186 2023-04-16 09:56:38.069284 pyinterpolate-0.4.1/setup.cfg
```

### Comparing `pyinterpolate-0.4/PKG-INFO` & `pyinterpolate-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinterpolate
-Version: 0.4
+Version: 0.4.1
 Summary: Spatial Interpolation in Python
 Home-page: https://github.com/DataverseLabs/pyinterpolate
 Download-URL: https://github.com/DataverseLabs/pyinterpolate/archive/
 Author: Szymon Moliński
 Author-email: simon@dataverselabs.com
 License: BSD 3-clause
 Project-URL: Documentation, https://readthedocs.org/projects/pyinterpolate/
@@ -23,15 +23,15 @@
 
 ![status](https://joss.theoj.org/papers/3f87f562264c4e5174d9e6ed6d8812aa/status.svg) ![License](https://img.shields.io/github/license/szymon-datalions/pyinterpolate) ![Documentation Status](https://readthedocs.org/projects/pyinterpolate/badge/?version=latest) [![CodeFactor](https://www.codefactor.io/repository/github/dataverselabs/pyinterpolate/badge)](https://www.codefactor.io/repository/github/dataverselabs/pyinterpolate)
 
 ![Pyinterpolate](https://github.com/DataverseLabs/pyinterpolate/blob/main/logov04.jpg?raw=true  "Pyinterpolate logo")
 
 # Pyinterpolate
 
-**version 0.4** - *Kharkiv*
+**version 0.4.1** - *Kharkiv*
 
 ---
 
 Pyinterpolate is the Python library for **spatial statistics**. The package provides access to spatial statistics tools used in various studies. This package helps you **interpolate spatial data** with the *Kriging* technique.
 
 If you’re:
```

### Comparing `pyinterpolate-0.4/README.md` & `pyinterpolate-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ![status](https://joss.theoj.org/papers/3f87f562264c4e5174d9e6ed6d8812aa/status.svg) ![License](https://img.shields.io/github/license/szymon-datalions/pyinterpolate) ![Documentation Status](https://readthedocs.org/projects/pyinterpolate/badge/?version=latest) [![CodeFactor](https://www.codefactor.io/repository/github/dataverselabs/pyinterpolate/badge)](https://www.codefactor.io/repository/github/dataverselabs/pyinterpolate)
 
 ![Pyinterpolate](https://github.com/DataverseLabs/pyinterpolate/blob/main/logov04.jpg?raw=true  "Pyinterpolate logo")
 
 # Pyinterpolate
 
-**version 0.4** - *Kharkiv*
+**version 0.4.1** - *Kharkiv*
 
 ---
 
 Pyinterpolate is the Python library for **spatial statistics**. The package provides access to spatial statistics tools used in various studies. This package helps you **interpolate spatial data** with the *Kriging* technique.
 
 If you’re:
```

### Comparing `pyinterpolate-0.4/pyinterpolate/__init__.py` & `pyinterpolate-0.4.1/pyinterpolate/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,8 +38,8 @@
 # Indicator
 from pyinterpolate.variogram import IndicatorVariogramData, ExperimentalIndicatorVariogram, IndicatorVariograms
 
 # Viz
 from pyinterpolate.viz import interpolate_raster
 
 
-__version__ = "0.3.7"
+__version__ = "0.4.1"
```

### Comparing `pyinterpolate-0.4/pyinterpolate/distance/clusters.py` & `pyinterpolate-0.4.1/pyinterpolate/distance/clusters.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/distance/distance.py` & `pyinterpolate-0.4.1/pyinterpolate/distance/distance.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/distance/gridding.py` & `pyinterpolate-0.4.1/pyinterpolate/distance/gridding.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/idw/idw.py` & `pyinterpolate-0.4.1/pyinterpolate/idw/idw.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/io/read_data.py` & `pyinterpolate-0.4.1/pyinterpolate/io/read_data.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/kriging/__init__.py` & `pyinterpolate-0.4.1/pyinterpolate/kriging/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/kriging/models/block/area_to_area_poisson_kriging.py` & `pyinterpolate-0.4.1/pyinterpolate/kriging/models/block/area_to_area_poisson_kriging.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/kriging/models/block/area_to_point_poisson_kriging.py` & `pyinterpolate-0.4.1/pyinterpolate/kriging/models/block/area_to_point_poisson_kriging.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/kriging/models/block/centroid_based_poisson_kriging.py` & `pyinterpolate-0.4.1/pyinterpolate/kriging/models/block/centroid_based_poisson_kriging.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/kriging/models/block/weight.py` & `pyinterpolate-0.4.1/pyinterpolate/kriging/models/block/weight.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/kriging/models/indicator/indicator_point_kriging.py` & `pyinterpolate-0.4.1/pyinterpolate/kriging/models/indicator/indicator_point_kriging.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/kriging/models/point/ordinary_kriging.py` & `pyinterpolate-0.4.1/pyinterpolate/kriging/models/point/ordinary_kriging.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/kriging/models/point/simple_kriging.py` & `pyinterpolate-0.4.1/pyinterpolate/kriging/models/point/simple_kriging.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/kriging/models/structures/point_kriging.py` & `pyinterpolate-0.4.1/pyinterpolate/kriging/models/structures/point_kriging.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/kriging/point_kriging.py` & `pyinterpolate-0.4.1/pyinterpolate/kriging/point_kriging.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/kriging/utils/kwarnings.py` & `pyinterpolate-0.4.1/pyinterpolate/kriging/utils/kwarnings.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/kriging/utils/process.py` & `pyinterpolate-0.4.1/pyinterpolate/kriging/utils/process.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/pipelines/block_filtering.py` & `pyinterpolate-0.4.1/pyinterpolate/pipelines/block_filtering.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/pipelines/deconvolution.py` & `pyinterpolate-0.4.1/pyinterpolate/pipelines/deconvolution.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/pipelines/multi_kriging.py` & `pyinterpolate-0.4.1/pyinterpolate/pipelines/multi_kriging.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/processing/checks.py` & `pyinterpolate-0.4.1/pyinterpolate/processing/checks.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/processing/preprocessing/blocks.py` & `pyinterpolate-0.4.1/pyinterpolate/processing/preprocessing/blocks.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/processing/select_values.py` & `pyinterpolate-0.4.1/pyinterpolate/processing/select_values.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/processing/transform/statistics.py` & `pyinterpolate-0.4.1/pyinterpolate/processing/transform/statistics.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/processing/transform/transform.py` & `pyinterpolate-0.4.1/pyinterpolate/processing/transform/transform.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/processing/utils/exceptions.py` & `pyinterpolate-0.4.1/pyinterpolate/processing/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/validation/cross_validation.py` & `pyinterpolate-0.4.1/pyinterpolate/validation/cross_validation.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/variogram/__init__.py` & `pyinterpolate-0.4.1/pyinterpolate/variogram/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/variogram/empirical/__init__.py` & `pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/variogram/empirical/cloud.py` & `pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/cloud.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/variogram/empirical/covariance.py` & `pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/covariance.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,16 +173,15 @@
     return output_covariances
 
 
 def calculate_covariance(points: np.array,
                          step_size: float,
                          max_range: float,
                          direction=None,
-                         tolerance=1,
-                         get_c0=True) -> tuple:
+                         tolerance=1) -> np.ndarray:
     """Function calculates covariance from given points. In a default mode it calculates an omnidirectional
        covariance. User can calculate a directional covariogram with a specified tolerance.
 
     Parameters
     ----------
     points : numpy array
              Coordinates and their values [pt x, pt y, value].
@@ -205,21 +204,18 @@
                 Value in range (0-1] to calculate semi-minor axis length of the search area. If tolerance is close
                 to 0 then points must be placed at a single line with beginning in the origin of coordinate system
                 and direction given by y axis and direction parameter.
                     * The major axis length == step_size,
                     * The minor axis size == tolerance * step_size.
                     * Tolerance == 1 creates the omnidirectional covariogram.
 
-    get_c0 : bool, default=True
-             Calculate variance of a dataset and return it.
-
     Returns
     -------
-    : tuple
-        (numpy array [lag, covariance, number of pairs], variance : float or None)
+    : numpy array
+        [lag, covariance, number of pairs]
 
     Notes
     -----
     # Covariance
 
     It is a measure of similarity between points over distance. We assume that the close observations tends to be
         similar (see Tobler's Law). Distant observations are less and less similar up to the distance where influence
@@ -313,13 +309,8 @@
 
     if direction is None:
         covariance = omnidirectional_covariogram(points, lags, step_size)
     else:
         covariance = directional_covariogram(points, lags, step_size, direction, tolerance)
     # END:CALCULATIONS
 
-    cvar = None
-
-    if get_c0:
-        cvar = np.var(points[:, -1])
-
-    return covariance, cvar
+    return covariance
```

### Comparing `pyinterpolate-0.4/pyinterpolate/variogram/empirical/experimental_variogram.py` & `pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/experimental_variogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,17 +230,14 @@
 
     is_semivariance : bool, optional, default=True
         Should semivariance be calculated?
 
     is_covariance : bool, optional, default=True
         Should covariance be calculated?
 
-    is_variance : bool, optional, default=True
-        Should variance be calculated?
-
     Attributes
     ----------
     input_array : numpy array
         The array with coordinates and observed values.
 
     experimental_semivariance_array : numpy array or None, optional, default=None
         The array of semivariance per lag in the form: ``(lag, semivariance, number of points within lag)``.
@@ -334,29 +331,26 @@
     | lag |    semivariance    |      covariance     |    var_cov_diff    |
     +-----+--------------------+---------------------+--------------------+
     | 1.0 |       4.625        | -0.5434027777777798 | 4.791923487836951  |
     | 2.0 | 5.2272727272727275 | -0.7954545454545454 | 5.0439752555137165 |
     | 3.0 |        6.0         | -1.2599999999999958 | 5.508520710059168  |
     +-----+--------------------+---------------------+--------------------+
 
-    # TODO
-    * calculate variance ALWAYS
     """
 
     def __init__(self,
                  input_array: Union[np.ndarray, list, tuple],
                  step_size: float,
                  max_range: float,
                  weights=None,
                  direction: float = None,
                  tolerance: float = 1.0,
                  method='t',
                  is_semivariance=True,
-                 is_covariance=True,
-                 is_variance=True):
+                 is_covariance=True):
 
         self.input_array = None  # core structure
 
         if isinstance(input_array, np.ndarray):
             self.input_array = input_array
         else:
             self.input_array = np.array(input_array)
@@ -365,44 +359,41 @@
         self.experimental_semivariance_array = None
         self.experimental_covariance_array = None
         self.lags = None
         self.experimental_semivariances = None
         self.experimental_covariances = None
         self.variance_covariances_diff = None
         self.points_per_lag = None
-        self.variance = 0.0
+        self.variance = np.var(self.input_array[:, -1])
 
         self.step = step_size
         self.mx_rng = max_range
         self.weights = weights
         self.direct = direction
         self.tol = tolerance
         self.method = method
 
         self.__c_sem = is_semivariance
         self.__c_cov = is_covariance
-        self.__c_var = is_variance
 
         if is_semivariance:
             self._calculate_semivariance()
             self.lags = self.experimental_semivariance_array[:, 0]
             self.points_per_lag = self.experimental_semivariance_array[:, 2]
             self.experimental_semivariances = self.experimental_semivariance_array[:, 1]
 
         if is_covariance:
-            self._calculate_covariance(is_variance)
+            self._calculate_covariance()
             self.experimental_covariances = self.experimental_covariance_array[:, 1]
+            self.variance_covariances_diff = self.variance - self.experimental_covariances
 
             if not is_semivariance:
                 self.lags = self.experimental_covariance_array[:, 0]
                 self.points_per_lag = self.experimental_covariance_array[:, 2]
 
-            if is_variance:
-                self.variance_covariances_diff = self.variance - self.experimental_covariances
-
     def plot(self, plot_semivariance=True, plot_covariance=False, plot_variance=False) -> None:
         """
 
         Parameters
         ----------
         plot_semivariance : bool, default=True
             Show semivariance on a plot. If class attribute ``is_semivariance`` is set to ``False`` then semivariance is
@@ -422,15 +413,14 @@
             Warning invoked when plotting parameter for semivariance, covariance or variance is set to ``True`` but
             class attributes to calculate those indices are set to ``False``.
         """
 
         # Validate parameters
         validate_plot_attributes_for_experimental_variogram_class(is_semivar=self.__c_sem,
                                                                   is_covar=self.__c_cov,
-                                                                  is_var=self.__c_var,
                                                                   plot_semivar=plot_semivariance,
                                                                   plot_covar=plot_covariance,
                                                                   plot_var=plot_variance)
 
         # Plot
         # Cmap - 3 class Set2 https://colorbrewer2.org/#type=qualitative&scheme=Set2&n=3
         # Colorblind friendly
@@ -440,36 +430,35 @@
         plt.figure(figsize=(12, 6))
         if plot_semivariance and self.__c_sem:
             plt.scatter(self.lags, self.experimental_semivariances, marker='8', c='#66c2a5')
             legend.append('Experimental Semivariances')
         if plot_covariance and self.__c_cov:
             plt.scatter(self.lags, self.experimental_covariances, marker='+', c='#8da0cb')
             legend.append('Experimental Covariances')
-        if plot_variance and self.__c_var:
+        if plot_variance:
             var_line = [self.variance for _ in self.lags]
             plt.plot(self.lags, var_line, '--', color='#fc8d62')
             legend.append('Variance')
         plt.legend(legend)
         plt.xlabel('Distance')
         plt.ylabel('Variance')
         plt.show()
 
-    def _calculate_covariance(self, get_variance=False):
+    def _calculate_covariance(self):
         """
         Method calculates covariance and variance.
 
         See : calculate_covariance function.
         """
-        self.experimental_covariance_array, self.variance = calculate_covariance(
+        self.experimental_covariance_array = calculate_covariance(
             points=self.input_array,
             step_size=self.step,
             max_range=self.mx_rng,
             direction=self.direct,
-            tolerance=self.tol,
-            get_c0=get_variance
+            tolerance=self.tol
         )
 
     def _calculate_semivariance(self):
         """
         Method calculates semivariance.
 
         See: calculate_semivariance function.
@@ -484,15 +473,15 @@
             method=self.method
         )
 
     def __repr__(self):
         cname = 'ExperimentalVariogram'
         input_params = f'input_array={self.input_array.tolist()}, step_size={self.step}, max_range={self.mx_rng}, ' \
                        f'weights={self.weights}, direction={self.direct}, tolerance={self.tol}, ' \
-                       f'is_semivariance={self.__c_sem}, is_covariance={self.__c_cov}, is_variance={self.__c_var}'
+                       f'is_semivariance={self.__c_sem}, is_covariance={self.__c_cov}'
         repr_val = cname + '(' + input_params + ')'
         return repr_val
 
     def __str__(self):
 
         pretty_table = PrettyTable()
 
@@ -504,50 +493,35 @@
             if self.__c_sem and self.__c_cov:
                 pretty_table.add_rows(self.__str_populate_both())
             else:
                 pretty_table.add_rows(self.__str_populate_single())
             return pretty_table.get_string()
 
     def __str_empty(self):
-        if not self.__c_var:
-            return "Empty object"
-        else:
-            return f"Variance: {self.variance:.4f}"
+        return f"Variance: {self.variance:.4f}. Other parameters not calculated."
 
     def __str_populate_both(self):
         rows = []
-        if self.__c_var:
-            for idx, row in enumerate(self.experimental_semivariances):
-                lag = self.lags[idx]
-                smv = row
-                cov = self.experimental_covariances[idx]
-                var_cov_diff = self.variance_covariances_diff[idx]
-                rows.append([lag, smv, cov, var_cov_diff])
-        else:
-            for idx, row in enumerate(self.experimental_semivariances):
-                lag = self.lags[idx]
-                smv = row
-                cov = self.experimental_covariances[idx]
-                rows.append([lag, smv, cov, nan])
+        for idx, row in enumerate(self.experimental_semivariances):
+            lag = self.lags[idx]
+            smv = row
+            cov = self.experimental_covariances[idx]
+            var_cov_diff = self.variance_covariances_diff[idx]
+            rows.append([lag, smv, cov, var_cov_diff])
+
         return rows
 
     def __str_populate_single(self):
         rows = []
         if self.__c_cov:
-            if self.__c_var:
-                for idx, row in enumerate(self.experimental_covariances):
-                    lag = self.lags[idx]
-                    cov = row
-                    var_cov_diff = self.variance_covariances_diff[idx]
-                    rows.append([lag, nan, cov, var_cov_diff])
-            else:
-                for idx, row in enumerate(self.experimental_covariances):
-                    lag = self.lags[idx]
-                    cov = row
-                    rows.append([lag, nan, cov, nan])
+            for idx, row in enumerate(self.experimental_covariances):
+                lag = self.lags[idx]
+                cov = row
+                var_cov_diff = self.variance_covariances_diff[idx]
+                rows.append([lag, nan, cov, var_cov_diff])
         else:
             for idx, row in enumerate(self.experimental_semivariances):
                 lag = self.lags[idx]
                 sem = row
                 rows.append([lag, sem, nan, nan])
         return rows
 
@@ -655,11 +629,10 @@
         step_size=step_size,
         max_range=max_range,
         weights=weights,
         direction=direction,
         tolerance=tolerance,
         method=method,
         is_semivariance=True,
-        is_covariance=True,
-        is_variance=True
+        is_covariance=True
     )
     return semivariogram_stats
```

### Comparing `pyinterpolate-0.4/pyinterpolate/variogram/empirical/semivariance.py` & `pyinterpolate-0.4.1/pyinterpolate/variogram/empirical/semivariance.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/variogram/indicator/indicator_variogram.py` & `pyinterpolate-0.4.1/pyinterpolate/variogram/indicator/indicator_variogram.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,16 +182,15 @@
                 step_size=self.step_size,
                 max_range=self.max_range,
                 weights=self.weights,
                 direction=self.direction,
                 tolerance=self.tolerance,
                 method=self.method,
                 is_semivariance=True,
-                is_covariance=True,
-                is_variance=True
+                is_covariance=True
             )
             self.experimental_models[str(indicator)] = exp
 
     def show(self):
         """
         Function shows generated experimental variograms for each indicator.
         """
```

### Comparing `pyinterpolate-0.4/pyinterpolate/variogram/regularization/aggregated.py` & `pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/aggregated.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/variogram/regularization/block/avg_block_to_block_semivariances.py` & `pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/block/avg_block_to_block_semivariances.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/variogram/regularization/block/avg_inblock_semivariances.py` & `pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/block/avg_inblock_semivariances.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/variogram/regularization/block/block_to_block_semivariance.py` & `pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/block/block_to_block_semivariance.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/variogram/regularization/block/inblock_semivariance.py` & `pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/block/inblock_semivariance.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/variogram/regularization/deconvolution.py` & `pyinterpolate-0.4.1/pyinterpolate/variogram/regularization/deconvolution.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,15 +249,15 @@
         self.regularized_models = []  # List with numpy arrays with regularized models
 
     def fit(self,
             agg_dataset: Union[Blocks, gpd.GeoDataFrame, pd.DataFrame, np.ndarray],
             point_support_dataset: Union[Dict, np.ndarray, gpd.GeoDataFrame, pd.DataFrame, PointSupport],
             agg_step_size: float,
             agg_max_range: float,
-            agg_nugget: float = 0,
+            agg_nugget: float = None,
             agg_direction: float = None,
             agg_tolerance: float = 1,
             variogram_weighting_method: str = "closest",
             model_types: Union[str, List] = 'basic') -> None:
         """
         Function fits given areal data variogram into point support variogram - it is the first step of regularization
         process.
@@ -332,20 +332,22 @@
 
         if self.verbose:
             print('Regularization fit process starts')
 
         # Update class parameters
         self.agg = agg_dataset
         self.ps = point_support_dataset
-        self.agg_step = agg_step_size
-        self.agg_rng = agg_max_range
-        self.agg_nugget = agg_nugget
+        self.agg_step = float(agg_step_size)
+        self.agg_rng = float(agg_max_range)
+        if agg_nugget is not None:
+            self.agg_nugget = float(agg_nugget)
         self.ranges = np.arange(agg_step_size, agg_max_range, agg_step_size)
-        self.direction = agg_direction
-        self.tolerance = agg_tolerance
+        if agg_direction is not None:
+            self.direction = float(agg_direction)
+        self.tolerance = float(agg_tolerance)
         self.weighting_method = variogram_weighting_method
         self.model_types = self._parse_model_types(model_types)
 
         # Compute experimental variogram of areal data
         areal_centroids = get_areal_centroids_from_agg(self.agg)
 
         self.initial_experimental_variogram = build_experimental_variogram(
@@ -526,15 +528,15 @@
         self.was_transformed = True
 
     def fit_transform(self,
                       agg_dataset: Union[Blocks, gpd.GeoDataFrame, pd.DataFrame, np.ndarray],
                       point_support_dataset: Union[Dict, np.ndarray, gpd.GeoDataFrame, pd.DataFrame, PointSupport],
                       agg_step_size: float,
                       agg_max_range: float,
-                      agg_nugget: float = 0,
+                      agg_nugget: float = None,
                       agg_direction: float = None,
                       agg_tolerance: float = 1,
                       variogram_weighting_method: str = "closest",
                       model_types: Union[str, List] = 'basic',
                       max_iters=25,
                       limit_deviation_ratio=0.1,
                       minimum_deviation_decrease=0.01,
@@ -561,15 +563,15 @@
 
         agg_step_size : float
             Step size between lags.
 
         agg_max_range : float
             Maximal distance of analysis.
 
-        agg_nugget : float, default = 0
+        agg_nugget : float, default = None
             The nugget of a dataset.
 
         agg_direction : float (in range [0, 360]), default=0
             Direction of semivariogram, values from 0 to 360 degrees:
 
             - 0 or 180: is E-W,
             - 90 or 270 is N-S,
```

### Comparing `pyinterpolate-0.4/pyinterpolate/variogram/theoretical/__init__.py` & `pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/__init__.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/variogram/theoretical/models/variogram_models.py` & `pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/models/variogram_models.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/variogram/theoretical/semivariogram.py` & `pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/semivariogram.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # Pyinterpolate dependencies
 from pyinterpolate.processing.select_values import create_min_max_array, get_study_max_range
 from pyinterpolate.variogram.theoretical.models import circular_model, cubic_model, linear_model, exponential_model, \
     gaussian_model, spherical_model, power_model
 from pyinterpolate.variogram.empirical.experimental_variogram import ExperimentalVariogram
 from pyinterpolate.variogram.utils.metrics import forecast_bias, root_mean_squared_error, \
     symmetric_mean_absolute_percentage_error, mean_absolute_error, weighted_root_mean_squared_error
-from pyinterpolate.variogram.utils.exceptions import validate_selected_errors, check_ranges, check_sills
+from pyinterpolate.variogram.utils.exceptions import validate_selected_errors, check_ranges, check_sills, check_nuggets
 
 from pyinterpolate.variogram.theoretical.spatial_dependency_index import calculate_spatial_dependence_index
 
 
 class TheoreticalVariogram:
     """Theoretical model of a spatial dissimilarity.
 
@@ -110,15 +110,15 @@
 
     Methods
     -------
     fit()
         Fits experimental variogram data into theoretical model.
 
     autofit()
-        The same as fit but tests multiple ranges, sills and models.
+        The same as fit but tests multiple nuggets, ranges, sills and models.
 
     calculate_model_error()
         Evaluates the model performance against experimental values.
 
     to_dict()
         Store model parameters in a dict.
 
@@ -327,23 +327,26 @@
         self._update_spatial_dependency()
 
         return _theoretical_values, _error
 
     def autofit(self,
                 experimental_variogram: Union[ExperimentalVariogram, np.ndarray],
                 model_types: Union[str, list] = 'all',
-                nugget=0,
+                nugget=None,
+                min_nugget=0,
+                max_nugget=0.5,
+                number_of_nuggets=16,
                 rang=None,
                 min_range=0.1,
                 max_range=0.5,
-                number_of_ranges=64,
+                number_of_ranges=16,
                 sill=None,
                 min_sill=0.,
                 max_sill=1,
-                number_of_sills=64,
+                number_of_sills=16,
                 direction=None,
                 error_estimator='rmse',
                 deviation_weighting='equal',
                 auto_update_attributes=True,
                 warn_about_set_params=True,
                 verbose=False,
                 return_params=True):
@@ -355,49 +358,59 @@
         experimental_variogram : ExperimentalVariogram
             Prepared Empirical Variogram or array.
 
         model_types : str or list
             List of modeling functions or a name of a single function. Available models:
 
             - 'all' - the same as list with all models,
+            - 'safe' - ``['linear', 'power', 'spherical']``,
             - 'circular',
             - 'cubic',
             - 'exponential',
             - 'gaussian',
             - 'linear',
             - 'power',
             - 'spherical'.
 
-        nugget : float, default = 0
-            Nugget (bias) of a variogram. Default value is 0.
+        nugget : float, optional
+            Nugget (bias) of a variogram. If given then it is fixed to this value.
+
+        min_nugget : float, default = 0
+            The minimum nugget as the ratio of the parameter to the first lag variance.
+
+        max_nugget : float, default = 0.5
+            The maximum nugget as the ratio of the parameter to the first lag variance.
+
+        number_of_nuggets : int, default = 16
+            How many equally spaced nuggets tested between ``min_nugget`` and ``max_nugget``.
 
         rang : float, optional
             If given, then range is fixed to this value.
 
         min_range : float, default = 0.1
             The minimal fraction of a variogram range, ``0 < min_range <= max_range``.
 
         max_range : float, default = 0.5
             The maximum fraction of a variogram range, ``min_range <= max_range <= 1``. Parameter ``max_range`` greater
             than **0.5** raises warning.
 
-        number_of_ranges : int, default = 64
+        number_of_ranges : int, default = 16
             How many equally spaced ranges are tested between ``min_range`` and ``max_range``.
 
         sill : float, default = None
             If given, then sill is fixed to this value.
 
         min_sill : float, default = 0
             The minimal fraction of the variogram variance at lag 0 to find a sill, ``0 <= min_sill <= max_sill``.
 
         max_sill : float, default = 1
             The maximum fraction of the variogram variance at lag 0 to find a sill. It *should be* lower or equal to 1.
             It is possible to set it above 1, but then warning is printed.
 
-        number_of_sills : int, default = 64
+        number_of_sills : int, default = 16
             How many equally spaced sill values are tested between ``min_sill`` and ``max_sill``.
 
         direction : float, in range [0, 360], default=None
             The direction of a semivariogram. If ``None`` given then semivariogram is isotropic. This parameter is
             required if passed experimental variogram is stored in a numpy array.
 
         error_estimator : str, default = 'rmse'
@@ -463,18 +476,14 @@
             Raised when ``sill < 0`` or ``range < 0`` or ``range > 1``.
 
         KeyError
             Raised when wrong model name(s) are provided by the users.
 
         KeyError
             Raised when wrong error type is provided by the users.
-
-        TODO
-        ----
-        * add 'safe' models list to autofit() method
         """
 
         self.deviation_weighting = deviation_weighting
 
         if self.are_params:
             if warn_about_set_params:
                 warnings.warn('Semivariogram parameters have been set earlier, you are going to overwrite them')
@@ -493,15 +502,28 @@
                       ' variogram is isotropic.'
                 warnings.warn(msg)
             self.direction = direction
 
         # Check model type and set models
         mtypes = self._check_models_type_autofit(model_types)
 
-        # Set ranges and sills
+        # Set nuggets, ranges and sills
+        if nugget is None:
+            check_nuggets(min_nugget, max_nugget)
+            if self.experimental_variogram is not None:
+                nugget_range_min = self.experimental_variogram.experimental_semivariances[0] * min_nugget
+                nugget_range_max = self.experimental_variogram.experimental_semivariances[0] * max_nugget
+            else:
+                nugget_range_min = self.experimental_array[0, 1] * min_nugget
+                nugget_range_max = self.experimental_array[0, 1] * max_nugget
+
+            nugget_ranges = np.linspace(nugget_range_min, nugget_range_max, number_of_nuggets)
+        else:
+            nugget_ranges = [nugget]
+
         if rang is None:
             check_ranges(min_range, max_range)
             if self.study_max_range is None:
                 if self.experimental_variogram is not None:
                     self.study_max_range = get_study_max_range(self.experimental_variogram.input_array[:, :-1])
                 else:
                     self.study_max_range = self.experimental_array[-1, 0]
@@ -534,37 +556,43 @@
             'model_type': '',
             'nugget': 0,
             'sill': 0,
             'range': 0
         }
 
         for _mtype in mtypes:
-            for _rang in min_max_ranges:
-                for _sill in min_max_sill:
-                    # Create model
-                    _mdl_fn = self.variogram_models[_mtype]
-                    _fitted_model = self._fit_model(_mdl_fn, nugget, _sill, _rang)
-
-                    # Calculate Error
-                    _err = self.calculate_model_error(_fitted_model[:, 1],
-                                                      **_errors_keys,
-                                                      deviation_weighting=deviation_weighting)
-
-                    if verbose:
-                        self.__print_autofit_info(_mtype, nugget, _sill, _rang, error_estimator, _err[error_estimator])
-
-                    # Check if model is better than the previous
-                    if _err[error_estimator] < err_val:
-                        err_val = _err[error_estimator]
-                        optimal_parameters['model_type'] = _mtype
-                        optimal_parameters['nugget'] = nugget
-                        optimal_parameters['sill'] = _sill
-                        optimal_parameters['range'] = _rang
-                        optimal_parameters['fitted_model'] = _fitted_model
-                        optimal_parameters.update(_err)
+            for _nugg in nugget_ranges:
+                for _rang in min_max_ranges:
+                    for _sill in min_max_sill:
+                        # Create model
+                        _mdl_fn = self.variogram_models[_mtype]
+                        _fitted_model = self._fit_model(_mdl_fn, _nugg, _sill, _rang)
+
+                        # Calculate Error
+                        _err = self.calculate_model_error(_fitted_model[:, 1],
+                                                          **_errors_keys,
+                                                          deviation_weighting=deviation_weighting)
+
+                        if verbose:
+                            self.__print_autofit_info(_mtype,
+                                                      _nugg,
+                                                      _sill,
+                                                      _rang,
+                                                      error_estimator,
+                                                      _err[error_estimator])
+
+                        # Check if model is better than the previous
+                        if _err[error_estimator] < err_val:
+                            err_val = _err[error_estimator]
+                            optimal_parameters['model_type'] = _mtype
+                            optimal_parameters['nugget'] = _nugg
+                            optimal_parameters['sill'] = _sill
+                            optimal_parameters['range'] = _rang
+                            optimal_parameters['fitted_model'] = _fitted_model
+                            optimal_parameters.update(_err)
 
         if auto_update_attributes:
             self._update_attributes(**optimal_parameters)
 
         # Update spatial dependency
         self._update_spatial_dependency()
 
@@ -870,14 +898,20 @@
                     'cubic',
                     'exponential',
                     'gaussian',
                     'linear',
                     'power',
                     'spherical'
                 ]
+            elif model_types == 'safe':
+                mtypes = [
+                    'linear',
+                    'power',
+                    'spherical'
+                ]
             else:
                 self._check_model_names(model_types)
                 mtypes.append(model_types)
         else:
             if isinstance(model_types, Collection):
                 for mdl in model_types:
                     try:
```

### Comparing `pyinterpolate-0.4/pyinterpolate/variogram/theoretical/spatial_dependency_index.py` & `pyinterpolate-0.4.1/pyinterpolate/variogram/theoretical/spatial_dependency_index.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,10 +36,10 @@
     if ratio < 25:
         spatial_dependency = 'strong'
     elif ratio < 75:
         spatial_dependency = 'moderate'
     elif ratio < 95:
         spatial_dependency = 'weak'
     else:
-        spatial_dependency = 'no spatial dependency'
+        spatial_dependency = 'no spatial dependence'
 
     return ratio, spatial_dependency
```

### Comparing `pyinterpolate-0.4/pyinterpolate/variogram/utils/exceptions.py` & `pyinterpolate-0.4.1/pyinterpolate/variogram/utils/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -133,14 +133,33 @@
 
 
 def validate_selected_errors(val: int):
     if val == 0:
         raise MetricsTypeSelectionError
 
 
+def check_nuggets(minn: float, maxn: float):
+    # Check if min is lower or equal to max
+    if minn > maxn:
+        msg = f'Minimum nugget to the first lag variance ratio {minn} is larger than maximum ' \
+              f'nugget to the first lag variance ratio {maxn}'
+        raise ValueError(msg)
+
+    # Check if min is negative
+    if minn < 0:
+        msg = f'Minimum nugget to the first lag variance ratio is below 0 and it is equal to {minn}'
+        raise ValueError(msg)
+
+    # Check if max is larger than 1 and throw warning if it is
+    if maxn > 1:
+        msg = f'Maximum nugget to the first lag variance ratio is greater than one, are you sure that nugget is ' \
+              f'larger than the variance for lag 1?'
+        warnings.warn(msg)
+
+
 def check_ranges(minr: float, maxr: float):
     # Check if min is lower or equal to max
     if minr > maxr:
         msg = f'Minimum range {minr} is larger than maximum range {maxr}'
         raise ValueError(msg)
 
     # Check if min is negative
@@ -169,27 +188,26 @@
     if maxs > 1:
         msg = f'Maximum sill ratio is greater than the variance of a data, it could introduce bias'
         warnings.warn(msg)
 
 
 def validate_plot_attributes_for_experimental_variogram_class(is_semivar: bool,
                                                               is_covar: bool,
-                                                              is_var: bool,
                                                               plot_semivar: bool,
                                                               plot_covar: bool,
                                                               plot_var: bool):
     validation = {}
 
     if (is_semivar is False) and (plot_semivar is True):
         validation['is_semivariance'] = True
 
     if (is_covar is False) and (plot_covar is True):
         validation['is_covariance'] = True
 
-    if (is_var is False) and (plot_var is True):
+    if plot_var:
         validation['is_variance'] = True
 
     if validation:
         print(AttributeSetToFalseWarning(validation))
 
 
 def validate_theoretical_variogram(variogram) -> None:
```

### Comparing `pyinterpolate-0.4/pyinterpolate/variogram/utils/metrics.py` & `pyinterpolate-0.4.1/pyinterpolate/variogram/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/variogram/utils/plots.py` & `pyinterpolate-0.4.1/pyinterpolate/variogram/utils/plots.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate/viz/raster.py` & `pyinterpolate-0.4.1/pyinterpolate/viz/raster.py`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate.egg-info/PKG-INFO` & `pyinterpolate-0.4.1/pyinterpolate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyinterpolate
-Version: 0.4
+Version: 0.4.1
 Summary: Spatial Interpolation in Python
 Home-page: https://github.com/DataverseLabs/pyinterpolate
 Download-URL: https://github.com/DataverseLabs/pyinterpolate/archive/
 Author: Szymon Moliński
 Author-email: simon@dataverselabs.com
 License: BSD 3-clause
 Project-URL: Documentation, https://readthedocs.org/projects/pyinterpolate/
@@ -23,15 +23,15 @@
 
 ![status](https://joss.theoj.org/papers/3f87f562264c4e5174d9e6ed6d8812aa/status.svg) ![License](https://img.shields.io/github/license/szymon-datalions/pyinterpolate) ![Documentation Status](https://readthedocs.org/projects/pyinterpolate/badge/?version=latest) [![CodeFactor](https://www.codefactor.io/repository/github/dataverselabs/pyinterpolate/badge)](https://www.codefactor.io/repository/github/dataverselabs/pyinterpolate)
 
 ![Pyinterpolate](https://github.com/DataverseLabs/pyinterpolate/blob/main/logov04.jpg?raw=true  "Pyinterpolate logo")
 
 # Pyinterpolate
 
-**version 0.4** - *Kharkiv*
+**version 0.4.1** - *Kharkiv*
 
 ---
 
 Pyinterpolate is the Python library for **spatial statistics**. The package provides access to spatial statistics tools used in various studies. This package helps you **interpolate spatial data** with the *Kriging* technique.
 
 If you’re:
```

### Comparing `pyinterpolate-0.4/pyinterpolate.egg-info/SOURCES.txt` & `pyinterpolate-0.4.1/pyinterpolate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/pyinterpolate.egg-info/requires.txt` & `pyinterpolate-0.4.1/pyinterpolate.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pyinterpolate-0.4/setup.cfg` & `pyinterpolate-0.4.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = pyinterpolate
 description = Spatial Interpolation in Python
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
-version = 0.4
+version = 0.4.1
 url = https://github.com/DataverseLabs/pyinterpolate
 download_url = https://github.com/DataverseLabs/pyinterpolate/archive/
 author = Szymon Moliński
 author_email = simon@dataverselabs.com
 license = BSD 3-clause
 classifiers = 
 	Development Status :: 4 - Beta
```

