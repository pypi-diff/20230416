# Comparing `tmp/dtreeviz-2.2.0.tar.gz` & `tmp/dtreeviz-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtreeviz-2.2.0.tar", last modified: Mon Feb 20 21:22:36 2023, max compression
+gzip compressed data, was "dtreeviz-2.2.1.tar", last modified: Sun Apr 16 16:37:49 2023, max compression
```

## Comparing `dtreeviz-2.2.0.tar` & `dtreeviz-2.2.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-02-20 21:22:36.315328 dtreeviz-2.2.0/
--rw-r--r--   0 parrt      (501) staff       (20)     1069 2021-12-03 22:37:44.000000 dtreeviz-2.2.0/LICENSE
--rw-r--r--   0 parrt      (501) staff       (20)     1876 2023-02-20 21:22:36.315408 dtreeviz-2.2.0/PKG-INFO
--rw-r--r--   0 parrt      (501) staff       (20)    15961 2023-02-20 21:20:33.000000 dtreeviz-2.2.0/README.md
-drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-02-20 21:22:36.306192 dtreeviz-2.2.0/dtreeviz/
--rw-r--r--   0 parrt      (501) staff       (20)      596 2022-12-27 19:55:14.000000 dtreeviz-2.2.0/dtreeviz/__init__.py
--rw-r--r--   0 parrt      (501) staff       (20)    24724 2023-01-16 21:32:12.000000 dtreeviz-2.2.0/dtreeviz/classifiers.py
--rw-r--r--   0 parrt      (501) staff       (20)     4174 2023-01-16 21:32:12.000000 dtreeviz-2.2.0/dtreeviz/colors.py
--rw-r--r--   0 parrt      (501) staff       (20)    35371 2023-01-22 23:33:35.000000 dtreeviz-2.2.0/dtreeviz/compatibility.py
--rw-r--r--   0 parrt      (501) staff       (20)     6498 2023-01-16 21:32:12.000000 dtreeviz-2.2.0/dtreeviz/interpretation.py
-drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-02-20 21:22:36.308339 dtreeviz-2.2.0/dtreeviz/models/
--rw-r--r--   0 parrt      (501) staff       (20)        0 2020-07-11 17:37:37.000000 dtreeviz-2.2.0/dtreeviz/models/__init__.py
--rw-r--r--   0 parrt      (501) staff       (20)     8271 2023-02-09 18:22:21.000000 dtreeviz-2.2.0/dtreeviz/models/lightgbm_decision_tree.py
--rw-r--r--   0 parrt      (501) staff       (20)    22221 2023-02-20 21:19:16.000000 dtreeviz-2.2.0/dtreeviz/models/shadow_decision_tree.py
--rw-r--r--   0 parrt      (501) staff       (20)     4653 2023-01-16 21:32:12.000000 dtreeviz-2.2.0/dtreeviz/models/sklearn_decision_trees.py
--rw-r--r--   0 parrt      (501) staff       (20)     8735 2023-01-16 21:32:12.000000 dtreeviz-2.2.0/dtreeviz/models/spark_decision_tree.py
--rw-r--r--   0 parrt      (501) staff       (20)     8460 2023-02-09 18:22:21.000000 dtreeviz-2.2.0/dtreeviz/models/tensorflow_decision_tree.py
--rw-r--r--   0 parrt      (501) staff       (20)     8979 2023-02-09 18:22:21.000000 dtreeviz-2.2.0/dtreeviz/models/xgb_decision_tree.py
--rw-r--r--   0 parrt      (501) staff       (20)     3780 2023-01-29 18:56:38.000000 dtreeviz-2.2.0/dtreeviz/t3.py
--rw-r--r--   0 parrt      (501) staff       (20)    87507 2023-02-20 21:19:16.000000 dtreeviz-2.2.0/dtreeviz/trees.py
--rw-r--r--   0 parrt      (501) staff       (20)    17511 2023-02-20 21:19:16.000000 dtreeviz-2.2.0/dtreeviz/utils.py
--rw-r--r--   0 parrt      (501) staff       (20)     1099 2023-02-20 21:19:16.000000 dtreeviz-2.2.0/dtreeviz/version.py
-drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-02-20 21:22:36.306966 dtreeviz-2.2.0/dtreeviz.egg-info/
--rw-r--r--   0 parrt      (501) staff       (20)     1876 2023-02-20 21:22:36.000000 dtreeviz-2.2.0/dtreeviz.egg-info/PKG-INFO
--rw-r--r--   0 parrt      (501) staff       (20)     1659 2023-02-20 21:22:36.000000 dtreeviz-2.2.0/dtreeviz.egg-info/SOURCES.txt
--rw-r--r--   0 parrt      (501) staff       (20)        1 2023-02-20 21:22:36.000000 dtreeviz-2.2.0/dtreeviz.egg-info/dependency_links.txt
--rw-r--r--   0 parrt      (501) staff       (20)      243 2023-02-20 21:22:36.000000 dtreeviz-2.2.0/dtreeviz.egg-info/requires.txt
--rw-r--r--   0 parrt      (501) staff       (20)       17 2023-02-20 21:22:36.000000 dtreeviz-2.2.0/dtreeviz.egg-info/top_level.txt
--rw-r--r--   0 parrt      (501) staff       (20)       79 2023-02-20 21:22:36.315675 dtreeviz-2.2.0/setup.cfg
--rw-r--r--   0 parrt      (501) staff       (20)     2579 2023-02-20 21:19:16.000000 dtreeviz-2.2.0/setup.py
-drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-02-20 21:22:36.313125 dtreeviz-2.2.0/testing/
--rw-r--r--   0 parrt      (501) staff       (20)        0 2021-02-05 19:09:10.000000 dtreeviz-2.2.0/testing/__init__.py
--rw-r--r--   0 parrt      (501) staff       (20)     1878 2021-02-05 19:09:10.000000 dtreeviz-2.2.0/testing/animate_rtree_bivar_3D.py
--rw-r--r--   0 parrt      (501) staff       (20)     1754 2021-02-05 19:09:10.000000 dtreeviz-2.2.0/testing/cancer.py
--rw-r--r--   0 parrt      (501) staff       (20)     7263 2021-02-05 19:09:10.000000 dtreeviz-2.2.0/testing/gen_feature_space_samples.py
--rw-r--r--   0 parrt      (501) staff       (20)    13771 2021-02-05 19:09:10.000000 dtreeviz-2.2.0/testing/gen_samples.py
--rw-r--r--   0 parrt      (501) staff       (20)     1973 2021-02-05 19:09:10.000000 dtreeviz-2.2.0/testing/iris.py
--rw-r--r--   0 parrt      (501) staff       (20)     1861 2021-02-05 19:09:10.000000 dtreeviz-2.2.0/testing/paper_examples.py
--rw-r--r--   0 parrt      (501) staff       (20)      703 2021-02-05 19:09:10.000000 dtreeviz-2.2.0/testing/play_ctree.py
--rw-r--r--   0 parrt      (501) staff       (20)      724 2021-02-05 19:09:10.000000 dtreeviz-2.2.0/testing/play_ctree_bivar.py
--rw-r--r--   0 parrt      (501) staff       (20)     2247 2023-02-20 21:19:16.000000 dtreeviz-2.2.0/testing/play_lightgbm.py
--rw-r--r--   0 parrt      (501) staff       (20)      550 2021-02-05 19:09:10.000000 dtreeviz-2.2.0/testing/play_rtree.py
--rw-r--r--   0 parrt      (501) staff       (20)      817 2021-02-05 19:09:10.000000 dtreeviz-2.2.0/testing/play_rtree_bivar_3D.py
--rw-r--r--   0 parrt      (501) staff       (20)      565 2021-02-05 19:09:10.000000 dtreeviz-2.2.0/testing/play_rtree_bivar_heatmap.py
--rw-r--r--   0 parrt      (501) staff       (20)     3068 2023-02-20 21:19:16.000000 dtreeviz-2.2.0/testing/play_spark.py
-drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-02-20 21:22:36.313296 dtreeviz-2.2.0/testing/testlib/
--rw-r--r--   0 parrt      (501) staff       (20)        0 2021-02-05 19:09:10.000000 dtreeviz-2.2.0/testing/testlib/__init__.py
-drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-02-20 21:22:36.315109 dtreeviz-2.2.0/testing/testlib/models/
--rw-r--r--   0 parrt      (501) staff       (20)        0 2021-02-05 19:09:10.000000 dtreeviz-2.2.0/testing/testlib/models/__init__.py
--rw-r--r--   0 parrt      (501) staff       (20)     1129 2022-09-25 19:55:25.000000 dtreeviz-2.2.0/testing/testlib/models/conftest.py
--rw-r--r--   0 parrt      (501) staff       (20)     3879 2021-03-30 18:20:29.000000 dtreeviz-2.2.0/testing/testlib/models/test_decision_tree_lightgbm_classifier.py
--rw-r--r--   0 parrt      (501) staff       (20)     7608 2022-09-25 19:55:25.000000 dtreeviz-2.2.0/testing/testlib/models/test_decision_tree_spark_classifier.py
--rw-r--r--   0 parrt      (501) staff       (20)     4051 2022-12-27 19:55:15.000000 dtreeviz-2.2.0/testing/testlib/models/test_decision_tree_tensorflow_classifier.py
--rw-r--r--   0 parrt      (501) staff       (20)     2161 2021-02-05 19:09:10.000000 dtreeviz-2.2.0/testing/testlib/models/test_decision_tree_xgb_regressor.py
--rw-r--r--   0 parrt      (501) staff       (20)     7565 2023-02-20 21:19:16.000000 dtreeviz-2.2.0/testing/testlib/models/test_decision_trees_sk_classifier.py
--rw-r--r--   0 parrt      (501) staff       (20)     2467 2022-12-27 19:55:15.000000 dtreeviz-2.2.0/testing/testlib/models/test_decision_trees_sk_pipeline.py
--rw-r--r--   0 parrt      (501) staff       (20)     3887 2022-02-24 22:21:33.000000 dtreeviz-2.2.0/testing/testlib/models/test_decision_trees_xgb_classifier.py
--rw-r--r--   0 parrt      (501) staff       (20)     7207 2023-02-20 19:59:16.000000 dtreeviz-2.2.0/testing/testone.py
--rw-r--r--   0 parrt      (501) staff       (20)     2412 2023-02-20 21:19:16.000000 dtreeviz-2.2.0/testing/tf-catvars.py
--rw-r--r--   0 parrt      (501) staff       (20)     1897 2023-02-20 21:19:16.000000 dtreeviz-2.2.0/testing/tf_catvars2.py
--rw-r--r--   0 parrt      (501) staff       (20)     1788 2023-02-20 21:19:16.000000 dtreeviz-2.2.0/testing/tf_catvars3.py
--rw-r--r--   0 parrt      (501) staff       (20)     1941 2023-02-20 21:19:16.000000 dtreeviz-2.2.0/testing/tf_regr_catvars.py
+drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-04-16 16:37:49.908134 dtreeviz-2.2.1/
+-rw-r--r--   0 parrt      (501) staff       (20)     1069 2021-12-03 22:37:44.000000 dtreeviz-2.2.1/LICENSE
+-rw-r--r--   0 parrt      (501) staff       (20)     1876 2023-04-16 16:37:49.908216 dtreeviz-2.2.1/PKG-INFO
+-rw-r--r--   0 parrt      (501) staff       (20)    16124 2023-04-16 16:36:09.000000 dtreeviz-2.2.1/README.md
+drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-04-16 16:37:49.899041 dtreeviz-2.2.1/dtreeviz/
+-rw-r--r--   0 parrt      (501) staff       (20)      596 2022-12-27 19:55:14.000000 dtreeviz-2.2.1/dtreeviz/__init__.py
+-rw-r--r--   0 parrt      (501) staff       (20)    24724 2023-01-16 21:32:12.000000 dtreeviz-2.2.1/dtreeviz/classifiers.py
+-rw-r--r--   0 parrt      (501) staff       (20)     4174 2023-01-16 21:32:12.000000 dtreeviz-2.2.1/dtreeviz/colors.py
+-rw-r--r--   0 parrt      (501) staff       (20)    35384 2023-04-16 16:35:55.000000 dtreeviz-2.2.1/dtreeviz/compatibility.py
+-rw-r--r--   0 parrt      (501) staff       (20)     6498 2023-01-16 21:32:12.000000 dtreeviz-2.2.1/dtreeviz/interpretation.py
+drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-04-16 16:37:49.901026 dtreeviz-2.2.1/dtreeviz/models/
+-rw-r--r--   0 parrt      (501) staff       (20)        0 2020-07-11 17:37:37.000000 dtreeviz-2.2.1/dtreeviz/models/__init__.py
+-rw-r--r--   0 parrt      (501) staff       (20)     8271 2023-02-09 18:22:21.000000 dtreeviz-2.2.1/dtreeviz/models/lightgbm_decision_tree.py
+-rw-r--r--   0 parrt      (501) staff       (20)    22221 2023-02-20 21:19:16.000000 dtreeviz-2.2.1/dtreeviz/models/shadow_decision_tree.py
+-rw-r--r--   0 parrt      (501) staff       (20)     5254 2023-04-16 16:35:55.000000 dtreeviz-2.2.1/dtreeviz/models/sklearn_decision_trees.py
+-rw-r--r--   0 parrt      (501) staff       (20)     8735 2023-01-16 21:32:12.000000 dtreeviz-2.2.1/dtreeviz/models/spark_decision_tree.py
+-rw-r--r--   0 parrt      (501) staff       (20)     8460 2023-02-09 18:22:21.000000 dtreeviz-2.2.1/dtreeviz/models/tensorflow_decision_tree.py
+-rw-r--r--   0 parrt      (501) staff       (20)     8979 2023-02-09 18:22:21.000000 dtreeviz-2.2.1/dtreeviz/models/xgb_decision_tree.py
+-rw-r--r--   0 parrt      (501) staff       (20)     3780 2023-01-29 18:56:38.000000 dtreeviz-2.2.1/dtreeviz/t3.py
+-rw-r--r--   0 parrt      (501) staff       (20)    90581 2023-04-16 16:35:55.000000 dtreeviz-2.2.1/dtreeviz/trees.py
+-rw-r--r--   0 parrt      (501) staff       (20)    17511 2023-02-20 21:19:16.000000 dtreeviz-2.2.1/dtreeviz/utils.py
+-rw-r--r--   0 parrt      (501) staff       (20)     1099 2023-04-16 16:36:09.000000 dtreeviz-2.2.1/dtreeviz/version.py
+drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-04-16 16:37:49.899726 dtreeviz-2.2.1/dtreeviz.egg-info/
+-rw-r--r--   0 parrt      (501) staff       (20)     1876 2023-04-16 16:37:49.000000 dtreeviz-2.2.1/dtreeviz.egg-info/PKG-INFO
+-rw-r--r--   0 parrt      (501) staff       (20)     1659 2023-04-16 16:37:49.000000 dtreeviz-2.2.1/dtreeviz.egg-info/SOURCES.txt
+-rw-r--r--   0 parrt      (501) staff       (20)        1 2023-04-16 16:37:49.000000 dtreeviz-2.2.1/dtreeviz.egg-info/dependency_links.txt
+-rw-r--r--   0 parrt      (501) staff       (20)      243 2023-04-16 16:37:49.000000 dtreeviz-2.2.1/dtreeviz.egg-info/requires.txt
+-rw-r--r--   0 parrt      (501) staff       (20)       17 2023-04-16 16:37:49.000000 dtreeviz-2.2.1/dtreeviz.egg-info/top_level.txt
+-rw-r--r--   0 parrt      (501) staff       (20)       79 2023-04-16 16:37:49.908602 dtreeviz-2.2.1/setup.cfg
+-rw-r--r--   0 parrt      (501) staff       (20)     2579 2023-04-16 16:36:09.000000 dtreeviz-2.2.1/setup.py
+drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-04-16 16:37:49.906061 dtreeviz-2.2.1/testing/
+-rw-r--r--   0 parrt      (501) staff       (20)        0 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/__init__.py
+-rw-r--r--   0 parrt      (501) staff       (20)     1878 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/animate_rtree_bivar_3D.py
+-rw-r--r--   0 parrt      (501) staff       (20)     1754 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/cancer.py
+-rw-r--r--   0 parrt      (501) staff       (20)     7263 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/gen_feature_space_samples.py
+-rw-r--r--   0 parrt      (501) staff       (20)    13771 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/gen_samples.py
+-rw-r--r--   0 parrt      (501) staff       (20)     1973 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/iris.py
+-rw-r--r--   0 parrt      (501) staff       (20)     1861 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/paper_examples.py
+-rw-r--r--   0 parrt      (501) staff       (20)      703 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/play_ctree.py
+-rw-r--r--   0 parrt      (501) staff       (20)      724 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/play_ctree_bivar.py
+-rw-r--r--   0 parrt      (501) staff       (20)     2247 2023-02-20 21:19:16.000000 dtreeviz-2.2.1/testing/play_lightgbm.py
+-rw-r--r--   0 parrt      (501) staff       (20)      550 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/play_rtree.py
+-rw-r--r--   0 parrt      (501) staff       (20)      817 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/play_rtree_bivar_3D.py
+-rw-r--r--   0 parrt      (501) staff       (20)      565 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/play_rtree_bivar_heatmap.py
+-rw-r--r--   0 parrt      (501) staff       (20)     3068 2023-02-20 21:19:16.000000 dtreeviz-2.2.1/testing/play_spark.py
+drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-04-16 16:37:49.906225 dtreeviz-2.2.1/testing/testlib/
+-rw-r--r--   0 parrt      (501) staff       (20)        0 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/testlib/__init__.py
+drwxr-xr-x   0 parrt      (501) staff       (20)        0 2023-04-16 16:37:49.907968 dtreeviz-2.2.1/testing/testlib/models/
+-rw-r--r--   0 parrt      (501) staff       (20)        0 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/testlib/models/__init__.py
+-rw-r--r--   0 parrt      (501) staff       (20)     1129 2022-09-25 19:55:25.000000 dtreeviz-2.2.1/testing/testlib/models/conftest.py
+-rw-r--r--   0 parrt      (501) staff       (20)     3879 2021-03-30 18:20:29.000000 dtreeviz-2.2.1/testing/testlib/models/test_decision_tree_lightgbm_classifier.py
+-rw-r--r--   0 parrt      (501) staff       (20)     7608 2022-09-25 19:55:25.000000 dtreeviz-2.2.1/testing/testlib/models/test_decision_tree_spark_classifier.py
+-rw-r--r--   0 parrt      (501) staff       (20)     4051 2022-12-27 19:55:15.000000 dtreeviz-2.2.1/testing/testlib/models/test_decision_tree_tensorflow_classifier.py
+-rw-r--r--   0 parrt      (501) staff       (20)     2161 2021-02-05 19:09:10.000000 dtreeviz-2.2.1/testing/testlib/models/test_decision_tree_xgb_regressor.py
+-rw-r--r--   0 parrt      (501) staff       (20)     7565 2023-02-20 21:19:16.000000 dtreeviz-2.2.1/testing/testlib/models/test_decision_trees_sk_classifier.py
+-rw-r--r--   0 parrt      (501) staff       (20)     2467 2022-12-27 19:55:15.000000 dtreeviz-2.2.1/testing/testlib/models/test_decision_trees_sk_pipeline.py
+-rw-r--r--   0 parrt      (501) staff       (20)     3887 2022-02-24 22:21:33.000000 dtreeviz-2.2.1/testing/testlib/models/test_decision_trees_xgb_classifier.py
+-rw-r--r--   0 parrt      (501) staff       (20)     7207 2023-02-20 19:59:16.000000 dtreeviz-2.2.1/testing/testone.py
+-rw-r--r--   0 parrt      (501) staff       (20)     2412 2023-02-20 21:19:16.000000 dtreeviz-2.2.1/testing/tf-catvars.py
+-rw-r--r--   0 parrt      (501) staff       (20)     1897 2023-02-20 21:19:16.000000 dtreeviz-2.2.1/testing/tf_catvars2.py
+-rw-r--r--   0 parrt      (501) staff       (20)     1788 2023-02-20 21:19:16.000000 dtreeviz-2.2.1/testing/tf_catvars3.py
+-rw-r--r--   0 parrt      (501) staff       (20)     1941 2023-02-20 21:19:16.000000 dtreeviz-2.2.1/testing/tf_regr_catvars.py
```

### Comparing `dtreeviz-2.2.0/LICENSE` & `dtreeviz-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/PKG-INFO` & `dtreeviz-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtreeviz
-Version: 2.2.0
+Version: 2.2.1
 Summary: A Python 3 library for sci-kit learn, XGBoost, LightGBM, Spark, and TensorFlow decision tree visualization
 Home-page: https://github.com/parrt/dtreeviz
 Author: Terence Parr, Tudor Lapusan, and Prince Grover
 Author-email: parrt@antlr.org
 License: MIT
 Keywords: machine-learning data structures trees visualization
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dtreeviz-2.2.0/README.md` & `dtreeviz-2.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 ## Quick start
 
 See [Installation instructions](README.md#Installation) then take a look at the specific [notebooks](https://github.com/parrt/dtreeviz/tree/master/notebooks) for the supported ML library you're using:
 
 * [sklearn-based examples](notebooks/dtreeviz_sklearn_visualisations.ipynb) ([colab](https://colab.research.google.com/github/parrt/dtreeviz/blob/master/notebooks/dtreeviz_sklearn_visualisations.ipynb))
 * [LightGBM-based examples](notebooks/dtreeviz_lightgbm_visualisations.ipynb) ([colab](https://colab.research.google.com/github/parrt/dtreeviz/blob/master/notebooks/dtreeviz_lightgbm_visualisations.ipynb))
 * [Spark-based examples](notebooks/dtreeviz_spark_visualisations.ipynb) ([colab](https://colab.research.google.com/github/parrt/dtreeviz/blob/master/notebooks/dtreeviz_spark_visualisations.ipynb))
-* [TensorFlow-based examples](notebooks/dtreeviz_tensorflow_visualisations.ipynb) ([colab](https://colab.research.google.com/github/parrt/dtreeviz/blob/master/notebooks/dtreeviz_tensorflow_visualisations.ipynb))
+* [TensorFlow-based examples](notebooks/dtreeviz_tensorflow_visualisations.ipynb) ([colab](https://colab.research.google.com/github/parrt/dtreeviz/blob/master/notebooks/dtreeviz_tensorflow_visualisations.ipynb)) Also see blog at tensorflow.org [Visualizing TensorFlow Decision Forest Trees with dtreeviz](https://www.tensorflow.org/decision_forests/tutorials/dtreeviz_colab)
 * [XGBoost-based examples](notebooks/dtreeviz_xgboost_visualisations.ipynb) ([colab](https://colab.research.google.com/github/parrt/dtreeviz/blob/master/notebooks/dtreeviz_xgboost_visualisations.ipynb))
 * [Classifier decision boundaries for any scikit-learn model.ipynb](https://github.com/parrt/dtreeviz/tree/master/notebooks/classifier-decision-boundaries.ipynb) ([colab](https://colab.research.google.com/github/parrt/dtreeviz/blob/master/notebooks/classifier-decision-boundaries.ipynb))
 * [Changing colors notebook](notebooks/colors.ipynb) ([colab](https://colab.research.google.com/github/parrt/dtreeviz/blob/master/notebooks/colors.ipynb))
 
 To interopt with these different libraries, dtreeviz uses an adaptor object, obtained from function `dtreeviz.model()`, to extract model information necessary for visualization. Given such an adaptor object, all of the dtreeviz functionality is available to you using the same programmer interface. The basic dtreeviz usage recipe is:
 
 1. Import dtreeviz and your decision tree library
@@ -282,15 +282,15 @@
 
 To push the `dtreeviz` library to your local egg cache (force updates) during development, do this (from anaconda prompt on Windows):
  
 ```bash 
 python setup.py install -f
 ```
 
-E.g., on Terence's box, it add `/Users/parrt/anaconda3/lib/python3.6/site-packages/dtreeviz-2.2.0-py3.6.egg`.
+E.g., on Terence's box, it add `/Users/parrt/anaconda3/lib/python3.6/site-packages/dtreeviz-2.2.1-py3.6.egg`.
 
 ## Feedback
 
 We welcome info from users on how they use dtreeviz, what features they'd like, etc... via [email (to parrt)](mailto:parrt@antlr.org) or via an [issue](https://github.com/parrt/dtreeviz/issues).
 
 ## Useful Resources
```

### Comparing `dtreeviz-2.2.0/dtreeviz/__init__.py` & `dtreeviz-2.2.1/dtreeviz/__init__.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/dtreeviz/classifiers.py` & `dtreeviz-2.2.1/dtreeviz/classifiers.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/dtreeviz/colors.py` & `dtreeviz-2.2.1/dtreeviz/colors.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/dtreeviz/compatibility.py` & `dtreeviz-2.2.1/dtreeviz/compatibility.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,15 @@
     shadow_tree = ShadowDecTree.get_shadow_tree(tree_model, X_train, y_train, feature_names, target_name, class_names,
                                                 tree_index)
     model = DTreeVizAPI(shadow_tree)
     return model.view(precision, orientation,
                       instance_orientation,
                       show_root_edge_labels, show_node_labels, show_just_path, fancy, histtype, highlight_path, X,
                       max_X_features_LR, max_X_features_TD, depth_range_to_display, label_fontsize, ticks_fontsize,
-                      fontname, title, title_fontsize, colors, scale)
+                      fontname, title, title_fontsize, colors=colors, scale=scale)
 
 
 def viz_leaf_samples(tree_model,
                      X_train: (pd.DataFrame, np.ndarray) = None,
                      feature_names: List[str] = None,
                      tree_index: int = None,  # required in case of tree ensemble
                      display_type: str = "plot",
```

### Comparing `dtreeviz-2.2.0/dtreeviz/interpretation.py` & `dtreeviz-2.2.1/dtreeviz/interpretation.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/dtreeviz/models/lightgbm_decision_tree.py` & `dtreeviz-2.2.1/dtreeviz/models/lightgbm_decision_tree.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/dtreeviz/models/shadow_decision_tree.py` & `dtreeviz-2.2.1/dtreeviz/models/shadow_decision_tree.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/dtreeviz/models/sklearn_decision_trees.py` & `dtreeviz-2.2.1/dtreeviz/models/sklearn_decision_trees.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,16 +90,27 @@
     def get_node_split(self, id) -> (int, float):
         return self.tree_model.tree_.threshold[id]
 
     def get_node_feature(self, id) -> int:
         return self.tree_model.tree_.feature[id]
 
     def get_node_nsamples_by_class(self, id):
+        # This is the code to return the nsamples/class from tree metadata. It's faster, but the visualisations cannot
+        # be made on new datasets.
+        # if self.is_classifier():
+        #     return self.tree_model.tree_.value[id][0]
+
+        # This code allows us to return the nsamples/class based on a dataset, train or validation
         if self.is_classifier():
-            return self.tree_model.tree_.value[id][0]
+            all_nodes = self.internal + self.leaves
+            node_value = [node.n_sample_classes() for node in all_nodes if node.id == id]
+            if self.get_class_weights() is None:
+                return node_value[0]
+            else:
+                return node_value[0] * self.get_class_weights()
 
     def get_prediction(self, id):
         if self.is_classifier():
             counts = self.tree_model.tree_.value[id][0]
             return np.argmax(counts)
         else:
             return self.tree_model.tree_.value[id][0][0]
```

### Comparing `dtreeviz-2.2.0/dtreeviz/models/spark_decision_tree.py` & `dtreeviz-2.2.1/dtreeviz/models/spark_decision_tree.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/dtreeviz/models/tensorflow_decision_tree.py` & `dtreeviz-2.2.1/dtreeviz/models/tensorflow_decision_tree.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/dtreeviz/models/xgb_decision_tree.py` & `dtreeviz-2.2.1/dtreeviz/models/xgb_decision_tree.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/dtreeviz/t3.py` & `dtreeviz-2.2.1/dtreeviz/t3.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/dtreeviz/trees.py` & `dtreeviz-2.2.1/dtreeviz/trees.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import tempfile
-from typing import Mapping, List
+from typing import Mapping, List, Callable
 
+import matplotlib
 import matplotlib.patches as patches
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
 from colour import Color, rgb2hex
 from sklearn import tree
@@ -130,14 +131,17 @@
                 rect.set_edgecolor(colors['rect_edge'])
 
             _format_axes(ax, "Leaf Sample", "Leaf Count", colors, fontsize, fontname, ticks_fontsize=None, grid=grid)
 
 
     def ctree_leaf_distributions(self,
                                  display_type: ("plot", "text") = "plot",
+                                 xaxis_display_type: str = "individual",
+                                 show_leaf_id_list: list = None,
+                                 show_leaf_filter: Callable[[np.ndarray], bool] = None,
                                  plot_ylim: int = None,
                                  colors: dict = None,
                                  fontsize: int = 10,
                                  fontname: str = "Arial",
                                  grid: bool = False,
                                  figsize: tuple = None,
                                  ax=None):
@@ -152,14 +156,24 @@
         Usage example :
         viz_model = dtreeviz.model(tree_model, X_train=dataset[features], y_train=dataset[target],
                                    feature_names=features, target_name=target, class_names=[0, 1])
         viz_model.ctree_leaf_distributions()
 
         :param display_type: str, optional
            'plot' or 'text'
+        :param xaxis_display_type: str, optional
+           'individual': Displays every node ID individually
+           'auto': Let matplotlib automatically manage the node ID ticks
+           'y_sorted': Display in y order with no x-axis tick labels
+        :param show_leaf_id_list: list, optional
+           The allowed list of node id values to plot
+        :param show_leaf_filter: Callable[[np.ndarray], bool], optional
+           The filtering function to apply to leaf values before displaying the leaves.
+           The function is applied to a numpy array with the class i sample value in row i.
+           For example, to view only those leaves with more than 100 total samples, and more than 5 class 1 samples, use show_leaf_filter = lambda x: (100 < np.sum(x)) & (5 < x[1])
         :param plot_ylim: int, optional
             The max value for oY. This is useful in case we have few leaves with big sample values which 'shadow'
             the other leaves values.
         :param colors: dict
             The set of colors used for plotting
         :param fontsize: int
             Plot labels fontsize
@@ -177,34 +191,62 @@
 
             if ax is None:
                 if figsize:
                     fig, ax = plt.subplots(figsize=figsize)
                 else:
                     fig, ax = plt.subplots()
 
-            ax.set_xticks(range(0, len(index)))
-            ax.set_xticklabels(index)
-            if plot_ylim is not None:
-                ax.set_ylim(0, plot_ylim)
-
             leaf_samples_hist = [[] for i in range(self.shadow_tree.nclasses())]
             for leaf_sample in leaf_samples:
                 for i, leaf_count in enumerate(leaf_sample):
                     leaf_samples_hist[i].append(leaf_count)
+            leaf_samples_hist = np.array(leaf_samples_hist)
+
+            if show_leaf_id_list is not None:
+                _mask = np.isin(index, show_leaf_id_list)
+                leaf_samples_hist = leaf_samples_hist[:, _mask]
+                index = tuple(np.array(index)[_mask])
+            if show_leaf_filter is not None:
+                _mask = np.apply_along_axis(show_leaf_filter, 0, leaf_samples_hist)
+                leaf_samples_hist = leaf_samples_hist[:, _mask]
+                index = tuple(np.array(index)[_mask])
+
+            if xaxis_display_type == 'individual':
+                x = np.arange(0, len(index))
+                ax.set_xticks(x)
+                ax.set_xticklabels(index)
+            elif xaxis_display_type == 'auto':
+                x = np.array(index)
+                ax.set_xlim(np.min(x)-1, np.max(x)+1)
+            elif xaxis_display_type == 'y_sorted':
+                # sort by total y = sum(classes), then class 0, 1, 2, ...
+                sort_cols = [np.sum(leaf_samples_hist, axis=0)]
+                for i in range(leaf_samples_hist.shape[0]):
+                    sort_cols.append(leaf_samples_hist[i])
+                _sort = np.lexsort(sort_cols[::-1])[::-1]
+                leaf_samples_hist = leaf_samples_hist[:, _sort]
+                index = tuple(np.array(index)[_sort])
+
+                x = np.arange(0, len(index))
+                ax.set_xticks(x)
+                ax.set_xticklabels([])
+                ax.tick_params(axis='x', which='both', bottom=False)
+            else:
+                raise ValueError(f'Unknown xaxis_display_type = {xaxis_display_type}!')
+
+            if plot_ylim is not None:
+                ax.set_ylim(0, plot_ylim)
 
-            bar_containers = []
-            bottom_values = np.full(len(index), 0)
-            for i, leaf_sample in enumerate(leaf_samples_hist):
-                bar_container = ax.bar(range(0, len(index)), leaf_sample, bottom=bottom_values,
+            bottom_values = np.zeros(len(index))
+            for i in range(leaf_samples_hist.shape[0]):
+                bar_container = ax.bar(x, leaf_samples_hist[i], bottom=bottom_values,
                                     color=colors_classes[i],
                                     lw=.3, align='center', width=1)
-                bottom_values = bottom_values + np.array(leaf_sample)
-                bar_containers.append(bar_container)
+                bottom_values = bottom_values + leaf_samples_hist[i]
 
-            for bar_container in bar_containers:
                 for rect in bar_container.patches:
                     rect.set_linewidth(.5)
                     rect.set_edgecolor(colors['rect_edge'])
 
             class_values = self.shadow_tree.classes()
             n_classes=self.shadow_tree.nclasses()
             color_values = colors['classes'][n_classes]
@@ -758,16 +800,16 @@
         :param node_id: int
             Node id to interpret
         :return: pd.DataFrame
             Node training samples' stats
         """
 
         node_samples = self.shadow_tree.get_node_samples()
-        df = pd.DataFrame(self.shadow_tree.X_train, columns=self.shadow_tree.feature_names)
-        return df.iloc[node_samples[node_id]].describe()
+        df = pd.DataFrame(self.shadow_tree.X_train, columns=self.shadow_tree.feature_names).convert_dtypes()
+        return df.iloc[node_samples[node_id]].describe(include='all')
 
     def instance_feature_importance(self, x,
                                    colors: dict = None,
                                    fontsize: int = 10,
                                    fontname: str = "Arial",
                                    grid: bool = False,
                                    figsize: tuple = None,
@@ -880,15 +922,15 @@
             for i in range(len(y_labels)):
                 ax.text(max(y) + 10, i - 0.15, y_labels[i])
             ax.text(max(y) + 10, len(y_labels) - 0.15, self.shadow_tree.target_name.lower())
 
         for i in range(len(means)):
             ax.plot(means[i], means_range[i], color=colors['split_line'], linewidth=prediction_line_width)
 
-        _format_axes(ax, self.shadow_tree.target_name, "Leaf", colors, fontsize=label_fontsize, fontname=fontname, ticks_fontsize=None, grid=grid)
+        _format_axes(ax, self.shadow_tree.target_name, "Leaf IDs", colors, fontsize=label_fontsize, fontname=fontname, ticks_fontsize=None, grid=grid)
 
     def ctree_feature_space(self,
                             fontsize=10,
                             ticks_fontsize=8,
                             fontname="Arial",
                             nbins=25,
                             gtype='strip',
@@ -1138,20 +1180,30 @@
     else:
         hist, bins, barcontainers = ax.hist(X_hist,
                                             color=X_colors,
                                             align='mid',
                                             histtype=histtype,
                                             bins=bins,
                                             label=class_names)
+
         # Alter appearance of each bar
-        for patch in barcontainers:
-            for rect in patch.patches:
+        if isinstance(barcontainers[0], matplotlib.container.BarContainer):
+            for patch in barcontainers:
+                for rect in patch.patches:
+                    rect.set_linewidth(.5)
+                    rect.set_edgecolor(colors['rect_edge'])
+            ax.set_yticks([0, max([max(h) for h in hist])])
+        elif isinstance(barcontainers[0], matplotlib.patches.Rectangle):
+            # In case a node will contains samples from only one class.
+            for rect in barcontainers.patches:
                 rect.set_linewidth(.5)
                 rect.set_edgecolor(colors['rect_edge'])
-        ax.set_yticks([0, max([max(h) for h in hist])])
+            ax.set_yticks([0, max(hist)])
+
+
 
     # set an empty space at the beginning and the end of the node visualisation for better clarity
     bin_length = bins[1] - bins[0]
     overall_feature_range_wide = (bins[0] - 2 * bin_length, bins[len(bins) - 1] + 2 * bin_length)
 
     ax.set_xlim(*overall_feature_range_wide)
 
@@ -1196,14 +1248,18 @@
     size = nsamples * slope + minsize
     size = min(size, maxsize)
 
     # we visually need n=1 and n=9 to appear different but diff between 300 and 400 is no big deal
     counts = node.class_counts()
     prediction = node.prediction_name()
 
+    # when using another dataset than the training dataset, some leaves could have 0 samples.
+    # Trying to make a pie chart will raise some deprecation
+    if sum(counts) == 0:
+        return
     if leaftype == 'pie':
         _draw_piechart(counts, size=size, colors=colors, filename=filename, label=f"n={nsamples}\n{prediction}",
                       graph_colors=graph_colors, fontname=fontname)
     elif leaftype == 'barh':
         _draw_barh_chart(counts, size=size, colors=colors, filename=filename, label=f"n={nsamples}\n{prediction}",
                       graph_colors=graph_colors, fontname=fontname)
     else:
```

### Comparing `dtreeviz-2.2.0/dtreeviz/utils.py` & `dtreeviz-2.2.1/dtreeviz/utils.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/dtreeviz/version.py` & `dtreeviz-2.2.1/dtreeviz/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-__version__ = '2.2.0'
+__version__ = '2.2.1'
```

### Comparing `dtreeviz-2.2.0/dtreeviz.egg-info/PKG-INFO` & `dtreeviz-2.2.1/dtreeviz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtreeviz
-Version: 2.2.0
+Version: 2.2.1
 Summary: A Python 3 library for sci-kit learn, XGBoost, LightGBM, Spark, and TensorFlow decision tree visualization
 Home-page: https://github.com/parrt/dtreeviz
 Author: Terence Parr, Tudor Lapusan, and Prince Grover
 Author-email: parrt@antlr.org
 License: MIT
 Keywords: machine-learning data structures trees visualization
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dtreeviz-2.2.0/dtreeviz.egg-info/SOURCES.txt` & `dtreeviz-2.2.1/dtreeviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/setup.py` & `dtreeviz-2.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 extra_pyspark = ['pyspark']
 extra_lightgbm = ['lightgbm']
 extra_tensorflow = ['tensorflow_decision_forests']
 
 
 setup(
     name='dtreeviz',
-    version='2.2.0',
+    version='2.2.1',
     url='https://github.com/parrt/dtreeviz',
     license='MIT',
     packages=find_packages(),
     install_requires=[
         'graphviz>=0.9',
         'pandas',
         'numpy',
```

### Comparing `dtreeviz-2.2.0/testing/animate_rtree_bivar_3D.py` & `dtreeviz-2.2.1/testing/animate_rtree_bivar_3D.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/cancer.py` & `dtreeviz-2.2.1/testing/cancer.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/gen_feature_space_samples.py` & `dtreeviz-2.2.1/testing/gen_feature_space_samples.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/gen_samples.py` & `dtreeviz-2.2.1/testing/gen_samples.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/iris.py` & `dtreeviz-2.2.1/testing/iris.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/paper_examples.py` & `dtreeviz-2.2.1/testing/paper_examples.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/play_ctree.py` & `dtreeviz-2.2.1/testing/play_ctree.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/play_ctree_bivar.py` & `dtreeviz-2.2.1/testing/play_ctree_bivar.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/play_lightgbm.py` & `dtreeviz-2.2.1/testing/play_lightgbm.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/play_rtree.py` & `dtreeviz-2.2.1/testing/play_rtree.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/play_rtree_bivar_3D.py` & `dtreeviz-2.2.1/testing/play_rtree_bivar_3D.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/play_rtree_bivar_heatmap.py` & `dtreeviz-2.2.1/testing/play_rtree_bivar_heatmap.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/play_spark.py` & `dtreeviz-2.2.1/testing/play_spark.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/testlib/models/conftest.py` & `dtreeviz-2.2.1/testing/testlib/models/conftest.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/testlib/models/test_decision_tree_lightgbm_classifier.py` & `dtreeviz-2.2.1/testing/testlib/models/test_decision_tree_lightgbm_classifier.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/testlib/models/test_decision_tree_spark_classifier.py` & `dtreeviz-2.2.1/testing/testlib/models/test_decision_tree_spark_classifier.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/testlib/models/test_decision_tree_tensorflow_classifier.py` & `dtreeviz-2.2.1/testing/testlib/models/test_decision_tree_tensorflow_classifier.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/testlib/models/test_decision_tree_xgb_regressor.py` & `dtreeviz-2.2.1/testing/testlib/models/test_decision_tree_xgb_regressor.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/testlib/models/test_decision_trees_sk_classifier.py` & `dtreeviz-2.2.1/testing/testlib/models/test_decision_trees_sk_classifier.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/testlib/models/test_decision_trees_sk_pipeline.py` & `dtreeviz-2.2.1/testing/testlib/models/test_decision_trees_sk_pipeline.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/testlib/models/test_decision_trees_xgb_classifier.py` & `dtreeviz-2.2.1/testing/testlib/models/test_decision_trees_xgb_classifier.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/testone.py` & `dtreeviz-2.2.1/testing/testone.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/tf-catvars.py` & `dtreeviz-2.2.1/testing/tf-catvars.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/tf_catvars2.py` & `dtreeviz-2.2.1/testing/tf_catvars2.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/tf_catvars3.py` & `dtreeviz-2.2.1/testing/tf_catvars3.py`

 * *Files identical despite different names*

### Comparing `dtreeviz-2.2.0/testing/tf_regr_catvars.py` & `dtreeviz-2.2.1/testing/tf_regr_catvars.py`

 * *Files identical despite different names*

