# Comparing `tmp/happy_learning-0.4.6.tar.gz` & `tmp/happy_learning-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/happy_learning-0.4.6.tar", last modified: Sun Jun 12 19:43:48 2022, max compression
+gzip compressed data, was "happy_learning-0.4.7.tar", last modified: Sun Apr 16 01:37:40 2023, max compression
```

## Comparing `happy_learning-0.4.6.tar` & `happy_learning-0.4.7.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2022-06-12 19:43:48.000000 happy_learning-0.4.6/
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    34966 2022-06-08 16:51:45.000000 happy_learning-0.4.6/LICENSE
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     9298 2022-06-12 19:43:48.000000 happy_learning-0.4.6/PKG-INFO
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     8494 2022-06-08 16:51:45.000000 happy_learning-0.4.6/README.md
-drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2022-06-12 19:43:48.000000 happy_learning-0.4.6/happy_learning/
--rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-08 16:51:45.000000 happy_learning-0.4.6/happy_learning/__init__.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     4331 2022-06-08 16:51:45.000000 happy_learning-0.4.6/happy_learning/arbitrary_modeling.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     2189 2022-06-08 16:51:45.000000 happy_learning-0.4.6/happy_learning/chaid_decision_tree.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    35170 2022-06-12 19:37:49.000000 happy_learning-0.4.6/happy_learning/data_miner.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    60718 2022-06-08 16:51:45.000000 happy_learning-0.4.6/happy_learning/deep_q_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    26284 2022-06-08 16:51:45.000000 happy_learning-0.4.6/happy_learning/environment_modeling.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    31399 2022-06-08 16:51:45.000000 happy_learning-0.4.6/happy_learning/evaluate_machine_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)   348942 2022-06-12 12:57:04.000000 happy_learning-0.4.6/happy_learning/feature_engineer.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    42132 2022-06-08 16:51:45.000000 happy_learning-0.4.6/happy_learning/feature_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    30523 2022-06-08 16:51:45.000000 happy_learning-0.4.6/happy_learning/feature_selector.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    29154 2022-06-08 16:51:45.000000 happy_learning-0.4.6/happy_learning/feature_tournament.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)   144589 2022-06-12 13:07:43.000000 happy_learning-0.4.6/happy_learning/genetic_algorithm.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     6461 2022-06-08 16:51:45.000000 happy_learning-0.4.6/happy_learning/missing_data_analysis.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    12205 2022-06-12 13:09:10.000000 happy_learning-0.4.6/happy_learning/multiple_imputation.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    95501 2022-06-08 16:51:45.000000 happy_learning-0.4.6/happy_learning/neural_network_generator_torch.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    40144 2022-06-08 16:51:45.000000 happy_learning-0.4.6/happy_learning/neural_network_torch.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     9223 2022-06-08 16:51:45.000000 happy_learning-0.4.6/happy_learning/sampler.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    22025 2022-06-08 16:51:45.000000 happy_learning-0.4.6/happy_learning/self_taught_short_text_clustering.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)   259606 2022-06-09 02:12:49.000000 happy_learning-0.4.6/happy_learning/supervised_machine_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)   142753 2022-06-12 13:07:43.000000 happy_learning-0.4.6/happy_learning/swarm_intelligence.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    30159 2022-06-08 16:51:45.000000 happy_learning-0.4.6/happy_learning/text_clustering.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    31963 2022-06-08 16:51:45.000000 happy_learning-0.4.6/happy_learning/text_clustering_generator.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    86060 2022-06-12 13:10:03.000000 happy_learning-0.4.6/happy_learning/text_miner.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    44550 2022-06-08 16:51:45.000000 happy_learning-0.4.6/happy_learning/utils.py
-drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2022-06-12 19:43:48.000000 happy_learning-0.4.6/happy_learning.egg-info/
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     9298 2022-06-12 19:43:48.000000 happy_learning-0.4.6/happy_learning.egg-info/PKG-INFO
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     1814 2022-06-12 19:43:48.000000 happy_learning-0.4.6/happy_learning.egg-info/SOURCES.txt
--rw-r--r--   0 giannibalistreri   (501) staff       (20)        1 2022-06-12 19:43:48.000000 happy_learning-0.4.6/happy_learning.egg-info/dependency_links.txt
--rw-r--r--   0 giannibalistreri   (501) staff       (20)      401 2022-06-12 19:43:48.000000 happy_learning-0.4.6/happy_learning.egg-info/requires.txt
--rw-r--r--   0 giannibalistreri   (501) staff       (20)       15 2022-06-12 19:43:48.000000 happy_learning-0.4.6/happy_learning.egg-info/top_level.txt
--rw-r--r--   0 giannibalistreri   (501) staff       (20)       92 2022-06-12 19:43:48.000000 happy_learning-0.4.6/setup.cfg
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     4323 2022-06-12 19:40:40.000000 happy_learning-0.4.6/setup.py
-drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2022-06-12 19:43:48.000000 happy_learning-0.4.6/test/
--rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_chaid_decision_tree.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     4304 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_data_miner.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    21131 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_deep_q_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     3749 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_environment_modeling.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     5231 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_evaluate_machine_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    36338 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_feature_engineer.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    17190 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_feature_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     3263 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_feature_selector.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     1934 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_feature_tournament.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    33868 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_genetic_algorithm.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     2539 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_missing_data_analysis.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)      754 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_multiple_imputation.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    13778 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_neural_network_generator_torch.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    10040 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_neural_network_torch.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     1545 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_sampler.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)      245 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_self_taught_short_clustering.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    16978 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_supervised_machine_learning.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    34195 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_swarm_intelligence.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     7281 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_text_clustering.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)    11994 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_text_clustering_generator.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)     4717 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_text_miner.py
--rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-08 16:51:46.000000 happy_learning-0.4.6/test/test_utils.py
+drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-16 01:37:40.444611 happy_learning-0.4.7/
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    34966 2022-06-13 17:25:08.000000 happy_learning-0.4.7/LICENSE
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     9278 2023-04-16 01:37:40.444962 happy_learning-0.4.7/PKG-INFO
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     8494 2022-06-13 17:25:08.000000 happy_learning-0.4.7/README.md
+drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-16 01:37:40.350984 happy_learning-0.4.7/happy_learning/
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/__init__.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     4331 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/arbitrary_modeling.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     2189 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/chaid_decision_tree.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    35170 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/data_miner.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    60718 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/deep_q_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    26284 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/environment_modeling.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    31399 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/evaluate_machine_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)   348942 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/feature_engineer.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    42132 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/feature_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    30523 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/feature_selector.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    29154 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/feature_tournament.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)   144589 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/genetic_algorithm.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     6461 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/missing_data_analysis.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    12205 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/multiple_imputation.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    74567 2023-04-16 00:13:24.000000 happy_learning-0.4.7/happy_learning/neural_network_generator_torch.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    34040 2023-04-16 00:13:24.000000 happy_learning-0.4.7/happy_learning/neural_network_torch.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     9223 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/sampler.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    22025 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/self_taught_short_text_clustering.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)   259606 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/supervised_machine_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)   142753 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/swarm_intelligence.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    30159 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/text_clustering.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    31963 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/text_clustering_generator.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    86060 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/text_miner.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    44550 2022-06-13 17:25:08.000000 happy_learning-0.4.7/happy_learning/utils.py
+drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-16 01:37:40.399220 happy_learning-0.4.7/happy_learning.egg-info/
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     9278 2023-04-16 01:37:40.000000 happy_learning-0.4.7/happy_learning.egg-info/PKG-INFO
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     1814 2023-04-16 01:37:40.000000 happy_learning-0.4.7/happy_learning.egg-info/SOURCES.txt
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)        1 2023-04-16 01:37:40.000000 happy_learning-0.4.7/happy_learning.egg-info/dependency_links.txt
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)      339 2023-04-16 01:37:40.000000 happy_learning-0.4.7/happy_learning.egg-info/requires.txt
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)       15 2023-04-16 01:37:40.000000 happy_learning-0.4.7/happy_learning.egg-info/top_level.txt
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)       92 2023-04-16 01:37:40.446380 happy_learning-0.4.7/setup.cfg
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     4271 2023-04-02 01:33:01.000000 happy_learning-0.4.7/setup.py
+drwxr-xr-x   0 giannibalistreri   (501) staff       (20)        0 2023-04-16 01:37:40.443639 happy_learning-0.4.7/test/
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_chaid_decision_tree.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     4304 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_data_miner.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    21131 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_deep_q_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     3749 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_environment_modeling.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     5231 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_evaluate_machine_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    36338 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_feature_engineer.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    17190 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_feature_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     3263 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_feature_selector.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     1934 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_feature_tournament.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    33868 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_genetic_algorithm.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     2539 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_missing_data_analysis.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)      754 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_multiple_imputation.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    12242 2023-04-16 01:08:43.000000 happy_learning-0.4.7/test/test_neural_network_generator_torch.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     8949 2023-04-16 01:08:43.000000 happy_learning-0.4.7/test/test_neural_network_torch.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     1545 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_sampler.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)      245 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_self_taught_short_clustering.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    16978 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_supervised_machine_learning.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    34195 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_swarm_intelligence.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     7281 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_text_clustering.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)    11994 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_text_clustering_generator.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)     4717 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_text_miner.py
+-rw-r--r--   0 giannibalistreri   (501) staff       (20)        0 2022-06-13 17:25:08.000000 happy_learning-0.4.7/test/test_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `happy_learning-0.4.6/LICENSE` & `happy_learning-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/PKG-INFO` & `happy_learning-0.4.7/happy_learning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: happy_learning
-Version: 0.4.6
+Name: happy-learning
+Version: 0.4.7
 Summary: Toolbox for reinforced developing of machine learning models (as proof-of-concept)
 Home-page: https://github.com/GianniBalistreri/happy_learning
 Author: Gianni Francesco Balistreri
 Author-email: gbalistreri@gmx.de
 License: GNU
 Keywords: feature-engineering feature-selection evolutionary-algorithm machine-learning automl reinforcement-learning deep-learning shapley clustering pytorch
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -215,9 +214,7 @@
     -- Generate similarity / clustering features:
         Apply similarity methods to generate continuous features using word embeddings
             -> TF-IDF
 
 ## 4. Documentation & Examples:
 
 Check the methodology.pdf for the documentation and jupyter notebook for examples. Happy ;) Learning
-
-
```

### Comparing `happy_learning-0.4.6/README.md` & `happy_learning-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/arbitrary_modeling.py` & `happy_learning-0.4.7/happy_learning/arbitrary_modeling.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/chaid_decision_tree.py` & `happy_learning-0.4.7/happy_learning/chaid_decision_tree.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/data_miner.py` & `happy_learning-0.4.7/happy_learning/data_miner.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/deep_q_learning.py` & `happy_learning-0.4.7/happy_learning/deep_q_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/environment_modeling.py` & `happy_learning-0.4.7/happy_learning/environment_modeling.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/evaluate_machine_learning.py` & `happy_learning-0.4.7/happy_learning/evaluate_machine_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/feature_engineer.py` & `happy_learning-0.4.7/happy_learning/feature_engineer.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/feature_learning.py` & `happy_learning-0.4.7/happy_learning/feature_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/feature_selector.py` & `happy_learning-0.4.7/happy_learning/feature_selector.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/feature_tournament.py` & `happy_learning-0.4.7/happy_learning/feature_tournament.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/genetic_algorithm.py` & `happy_learning-0.4.7/happy_learning/genetic_algorithm.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/missing_data_analysis.py` & `happy_learning-0.4.7/happy_learning/missing_data_analysis.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/multiple_imputation.py` & `happy_learning-0.4.7/happy_learning/multiple_imputation.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/neural_network_generator_torch.py` & `happy_learning-0.4.7/happy_learning/neural_network_generator_torch.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import copy
 import numpy as np
 import pandas as pd
 import torch
 import torch.nn.functional
 
 from .evaluate_machine_learning import EvalClf, EvalReg, ML_METRIC, SML_SCORE
-from .neural_network_torch import Attention, GRU, MLP, LSTM, RCNN, RNN, SelfAttention, Transformers
+from .neural_network_torch import Attention, GRU, MLP, LSTM, RCNN, RNN, SelfAttention
 from .utils import HappyLearningUtils
 from datetime import datetime
 from easyexplore.data_import_export import CLOUD_PROVIDER, DataImporter
 from torch.utils.data import DataLoader, TensorDataset
 from torchtext.data import BucketIterator, Field, TabularDataset
 from torchtext.vocab import FastText
 from typing import Dict, List, Tuple
@@ -25,16 +25,15 @@
 NETWORK_TYPE: Dict[str, str] = dict(att='attention_network',
                                     #cnn='convolutional_neural_network',
                                     gru='gated_recurrent_unit_network',
                                     lstm='long_short_term_memory_network',
                                     mlp='multi_layer_perceptron',
                                     rnn='recurrent_neural_network',
                                     rcnn='recurrent_convolutional_neural_network',
-                                    self='self_attention_network',
-                                    trans='transformer'
+                                    self='self_attention_network'
                                     )
 NETWORK_TYPE_CATEGORY: Dict[str, List[str]] = dict(tabular=['mlp'],
                                                    seq=['att', 'cnn', 'lstm', 'rnn', 'rcnn', 'lstm', 'self', 'trans']
                                                    )
 HIDDEN_LAYER_CATEGORY_EVOLUTION: List[str] = ['random',
                                               'constant',
                                               'monotone',
@@ -87,18 +86,14 @@
                                  )
                   )
 OPTIMIZER: dict = dict(adam=torch.optim.Adam,
                        rmsprop=torch.optim.RMSprop,
                        sgd=torch.optim.SGD
                        )
 EMBEDDING: dict = dict(fast_text=FastText)
-TRANSFORMER: dict = {#'roberta': 'roberta-large',
-                     'xlm': 'xlm-mlm-100-1280',
-                     #'xlmroberta': 'xlm-roberta-large'
-                     }
 IGNORE_PARAM_FOR_OPTIMIZATION: List[str] = ['embedding_len',
                                             'weights',
                                             'vocab_size',
                                             'bidirectional',
                                             'early_stopping',
                                             'recurrent_network_type',
                                             'loss_torch',
@@ -412,109 +407,14 @@
         return dict(hidden_states=np.random.choice(a=HappyLearningUtils().geometric_progression()),
                     epoch=np.random.randint(
                         low=1 if self.kwargs.get('epoch_low') is None else self.kwargs.get('epoch_low'),
                         high=20 if self.kwargs.get('epoch_high') is None else self.kwargs.get('epoch_high')
                         )
                     )
 
-    def transformer(self) -> Transformers:
-        """
-        Config Transformer Network
-
-        :return: Transformers
-            Model object
-        """
-        return Transformers(parameters=self.model_param, output_size=self.output_size, cache_dir=self.cache_dir)
-
-    def transformer_param(self) -> dict:
-        """
-        Generate Transformer Network classifier parameter configuration randomly
-
-        :return: dict
-            Parameter config
-        """
-        _model_type: str = np.random.choice(a=list(TRANSFORMER.keys())) if self.cache_dir is None else self.cache_dir.split('/')[-2].split('-')[0]
-        _num_attention_heads: int = np.random.randint(low=2 if self.kwargs.get('num_attention_heads_low') is None else self.kwargs.get('num_attention_heads_low'),
-                                                      high=20 if self.kwargs.get('num_attention_heads_high') is None else self.kwargs.get('num_attention_heads_high')
-                                                      )
-        _hidden_size: int = _num_attention_heads * np.random.randint(low=100 if self.kwargs.get('hidden_size_low') is None else self.kwargs.get('hidden_size_low'),
-                                                                     high=1000 if self.kwargs.get('hidden_size_high') is None else self.kwargs.get('hidden_size_high')
-                                                                     )
-        if self.kwargs.get('batch_size_choice') is None:
-            _batch_size: int = int(np.random.choice(a=HappyLearningUtils().geometric_progression(n=6))) if torch.cuda.is_available() else int(np.random.choice(a=HappyLearningUtils().geometric_progression(n=8)))
-        else:
-            _batch_size: int = int(np.random.choice(a=self.kwargs.get('batch_size_choice')))
-        return dict(model_type=_model_type,
-                    model_name=TRANSFORMER.get(_model_type) if self.cache_dir is None else self.cache_dir,
-                    epoch=np.random.randint(low=1 if self.kwargs.get('epoch_low') is None else self.kwargs.get('epoch_low'),
-                                            high=20 if self.kwargs.get('epoch_high') is None else self.kwargs.get('epoch_high')
-                                            ),
-                    batch_size=_batch_size,
-                    learning_rate=np.random.uniform(low=0.00001 if self.kwargs.get('learning_rate_low') is None else self.kwargs.get('learning_rate_low'),
-                                                    high=0.5 if self.kwargs.get('learning_rate_high') is None else self.kwargs.get('learning_rate_high')
-                                                    ),
-                    #adafactor_beta1=np.random.uniform(low=0.0, high=1),
-                    #adafactor_clip_threshold=np.random.uniform(low=0.001, high=1),
-                    #adafactor_decay_rate=np.random.uniform(low=-0.001, high=0.999),
-                    #adafactor_eps=(np.random.uniform(low=1e-50, high=1e-10), np.random.uniform(low=1e-50, high=1e-10)),
-                    #adafactor_relative_step=False,#np.random.choice(a=[False, True]),
-                    #adafactor_scale_parameter=np.random.choice(a=[False, True]),
-                    #adafactor_warmup_init=False,#np.random.choice(a=[False, True]),
-                    adam_epsilon=np.random.uniform(low=1e-10 if self.kwargs.get('adam_epsilon_low') is None else self.kwargs.get('adam_epsilon_low'),
-                                                   high=1e-5 if self.kwargs.get('adam_epsilon_high') is None else self.kwargs.get('adam_epsilon_high')
-                                                   ),
-                    cosine_schedule_num_cycles=np.random.uniform(low=0.3 if self.kwargs.get('cosine_schedule_num_cycles_low') is None else self.kwargs.get('cosine_schedule_num_cycles_low'),
-                                                                 high=0.7 if self.kwargs.get('cosine_schedule_num_cycles_high') is None else self.kwargs.get('cosine_schedule_num_cycles_high')
-                                                                 ),
-                    dynamic_quantize=False,#np.random.choice(a=[False, True]),
-                    early_stopping_consider_epochs=np.random.choice(a=[False, True] if self.kwargs.get('early_stopping_consider_epochs_choice') is None else self.kwargs.get('early_stopping_consider_epochs_choice')),
-                    use_early_stopping=np.random.choice(a=[False, True] if self.kwargs.get('use_early_stopping_choice') is None else self.kwargs.get('use_early_stopping_choice')),
-                    early_stopping_delta=np.random.uniform(low=0 if self.kwargs.get('early_stopping_delta_low') is None else self.kwargs.get('early_stopping_delta_low'),
-                                                           high=0.3 if self.kwargs.get('early_stopping_delta_high') is None else self.kwargs.get('early_stopping_delta_high')
-                                                           ),
-                    early_stopping_patience=np.random.randint(low=3 if self.kwargs.get('early_stopping_patience_low') is None else self.kwargs.get('early_stopping_patience_low'),
-                                                              high=10 if self.kwargs.get('early_stopping_patience_high') is None else self.kwargs.get('early_stopping_patience_high')
-                                                              ),
-                    attention_probs_dropout_prob=np.random.uniform(low=0.05 if self.kwargs.get('attention_probs_dropout_prob_low') is None else self.kwargs.get('attention_probs_dropout_prob_low'),
-                                                                   high=0.95 if self.kwargs.get('attention_probs_dropout_prob_high') is None else self.kwargs.get('attention_probs_dropout_prob_high')
-                                                                   ),
-                    hidden_size=_hidden_size,
-                    hidden_dropout_prob=np.random.uniform(low=0.05 if self.kwargs.get('hidden_dropout_prob_low') is None else self.kwargs.get('hidden_dropout_prob_low'),
-                                                          high=0.95 if self.kwargs.get('hidden_dropout_prob_high') is None else self.kwargs.get('hidden_dropout_prob_high')
-                                                          ),
-                    gradient_accumulation_steps=1,#np.random.randint(low=1, high=3),
-                    initializer_range=np.random.uniform(low=0.05 if self.kwargs.get('initializer_range_low') is None else self.kwargs.get('initializer_range_low'),
-                                                        high=0.95 if self.kwargs.get('initializer_range_high') is None else self.kwargs.get('initializer_range_high')
-                                                        ),
-                    layer_norm_eps=np.random.uniform(low=0.05 if self.kwargs.get('layer_norm_eps_low') is None else self.kwargs.get('layer_norm_eps_low'),
-                                                     high=0.5 if self.kwargs.get('layer_norm_eps_high') is None else self.kwargs.get('layer_norm_eps_high')
-                                                     ),
-                    num_attention_heads=_num_attention_heads,
-                    num_hidden_layers=np.random.randint(low=2 if self.kwargs.get('num_hidden_layers_low') is None else self.kwargs.get('num_hidden_layers_low'),
-                                                        high=30 if self.kwargs.get('num_hidden_layers_high') is None else self.kwargs.get('num_hidden_layers_high')
-                                                        ),
-                    warmup_ratio=np.random.uniform(low=0.03 if self.kwargs.get('warmup_ratio_low') is None else self.kwargs.get('warmup_ratio_low'),
-                                                   high=0.15 if self.kwargs.get('warmup_ratio_high') is None else self.kwargs.get('warmup_ratio_high')
-                                                   ),
-                    optimizer='AdamW',#np.random.choice(a=['AdamW', 'Adafactor']),
-                    scheduler=np.random.choice(a=['constant_schedule', 'constant_schedule_with_warmup', 'linear_schedule_with_warmup', 'cosine_schedule_with_warmup', 'cosine_with_hard_restarts_schedule_with_warmup', 'polynomial_decay_schedule_with_warmup'] if self.kwargs.get('scheduler') is None else self.kwargs.get('scheduler')),
-                    polynomial_decay_schedule_lr_end=np.random.uniform(low=1e-8 if self.kwargs.get('polynomial_decay_schedule_lr_end_low') is None else self.kwargs.get('polynomial_decay_schedule_lr_end_low'),
-                                                                       high=1e-4 if self.kwargs.get('polynomial_decay_schedule_lr_end_high') is None else self.kwargs.get('polynomial_decay_schedule_lr_end_high')
-                                                                       ),
-                    polynomial_decay_schedule_power=np.random.uniform(low=0.5 if self.kwargs.get('polynomial_decay_schedule_power_low') is None else self.kwargs.get('polynomial_decay_schedule_power_low'),
-                                                                      high=1.0 if self.kwargs.get('polynomial_decay_schedule_power_high') is None else self.kwargs.get('polynomial_decay_schedule_power_high')
-                                                                      ),
-                    max_grad_norm=np.random.uniform(low=0.01 if self.kwargs.get('max_grad_norm_low') is None else self.kwargs.get('max_grad_norm_low'),
-                                                    high=1.0 if self.kwargs.get('max_grad_norm_high') is None else self.kwargs.get('max_grad_norm_high')
-                                                    ),
-                    weight_decay=np.random.randint(low=0 if self.kwargs.get('weight_decay_low') is None else self.kwargs.get('weight_decay_low'),
-                                                   high=1 if self.kwargs.get('weight_decay_high') is None else self.kwargs.get('weight_decay_high')
-                                                   )
-                    )
-
 
 class NetworkGenerator(NeuralNetwork):
     """
     Class for generating neural networks using PyTorch
     """
     def __init__(self,
                  target: str,
@@ -605,15 +505,14 @@
             self.target_type: str = 'reg'
         elif self.output_size == 2:
             self.target_type: str = 'clf_binary'
         else:
             self.target_type: str = 'clf_multi'
         self.models: List[str] = models
         self.model_name: str = model_name
-        self.transformer: bool = True if model_name == 'trans' else False
         if self.model_name is None:
             self.random: bool = True
             if self.models is not None:
                 for model in self.models:
                     if model not in list(NETWORK_TYPE.keys()):
                         self.random: bool = False
                         raise NeuralNetworkException('Model ({}) is not supported. Supported classification models are: {}'.format(model, list(NETWORK_TYPE.keys())))
@@ -862,16 +761,15 @@
             self.model_param.update({'hidden_layer_{}_activation'.format(hidden): _hidden_layer_settings.get('activation')})
             self.model_param.update({'hidden_layer_{}_rnn_network_type'.format(hidden): _hidden_layer_settings.get('rnn_network_type')})
 
     def _config_params(self,
                        loss: bool = False,
                        optimizer: bool = False,
                        activation: bool = False,
-                       hidden_layers: bool = False,
-                       natural_language: bool = False
+                       hidden_layers: bool = False
                        ):
         """
         Finalize configuration of hyper parameter settings of the neural network
 
         :param loss: bool
             Configure loss function initially based on the size of the output layer
 
@@ -879,17 +777,14 @@
             Configure optimizer
 
         :param activation: bool
             Configure activation functions for all layers
 
         :param hidden_layers: bool
             Configure hidden_layers initially
-
-        :param natural_language: bool
-            Configure pre-trained embedding or transformer models
         """
         if loss:
             if self.model_param.get('loss') is None:
                 _loss: str = np.random.choice(a=list(LOSS.get(self.target_type).keys()))
                 self.model_param.update(dict(loss_torch=LOSS[self.target_type][_loss]))
         if optimizer:
             if self.model_param.get('optimizer') == 'sgd':
@@ -920,17 +815,14 @@
                                                                              amsgrad=False if self.model_param.get('amsgrad') is None else self.model_param.get('amsgrad')
                                                                              )
                                          })
         if activation:
             self._config_activation_functions()
         if hidden_layers:
             self._config_hidden_layers()
-        if natural_language:
-            _special_settings: dict = self._get_param_space(general=False)
-            self.model_param.update(_special_settings['embedding'])
 
     def _epoch_eval(self, iter_types: List[str]):
         """
         Evaluation of each training epoch
 
         :param iter_types: List[str]
             Names of the iteration process:
@@ -1015,169 +907,130 @@
                                        )
                         )
 
     def _import_data_torch(self):
         """
         Import data sets (Training, Testing, Validation) from file
         """
-        if self.transformer:
-            self.train_data_df = DataImporter(file_path=self.train_data_path,
-                                              as_data_frame=True,
-                                              use_dask=False,
-                                              create_dir=False,
-                                              sep=self.sep,
-                                              cloud=self.cloud,
-                                              bucket_name=self.bucket_name
-                                              ).file(table_name=None)
-            self.train_data_df[self.target] = pd.to_numeric(self.train_data_df[self.target])
-            self.test_data_df = DataImporter(file_path=self.test_data_path,
-                                             as_data_frame=True,
-                                             use_dask=False,
-                                             create_dir=False,
-                                             sep=self.sep,
-                                             cloud=self.cloud,
-                                             bucket_name=self.bucket_name
-                                             ).file(table_name=None)
-            self.test_data_df[self.target] = pd.to_numeric(self.test_data_df[self.target])
-            self.val_data_df = DataImporter(file_path=self.validation_data_path,
-                                            as_data_frame=True,
-                                            use_dask=False,
-                                            create_dir=False,
-                                            sep=self.sep,
-                                            cloud=self.cloud,
-                                            bucket_name=self.bucket_name
-                                            ).file(table_name=None)
-            self.val_data_df[self.target] = pd.to_numeric(self.val_data_df[self.target])
-        else:
-            if self.learning_type == 'batch':
-                if self.sequential_type == 'text':
-                    _unique_labels: list = pd.read_csv(filepath_or_buffer=self.train_data_path, sep=self.sep)[self.target].unique().tolist()
-                    _data_fields: List[tuple] = []
-                    self.embedding_text: Field = Field(sequential=True,
-                                                       tokenize=lambda x: x.split(),
-                                                       lower=True,
-                                                       include_lengths=True,
-                                                       batch_first=True,
-                                                       fix_length=300 if self.model_param.get('embedding_len') is None else self.model_param.get('embedding_len')
-                                                       )
-                    self.embedding_label: Field = Field(sequential=False, is_target=True, unk_token=None)
-                    for predictor in self.predictors:
-                        _data_fields.append((predictor, self.embedding_text))
-                    _data_fields.append((self.target, self.embedding_label))
-                    _train_data: TabularDataset = TabularDataset(path=self.train_data_path,
-                                                                 format='csv',
-                                                                 fields=_data_fields,
-                                                                 skip_header=True
-                                                                 )
-                    if self.test_data_path is None:
-                        _test_data = None
-                    else:
-                        _test_data: TabularDataset = TabularDataset(path=self.test_data_path,
-                                                                    format='csv',
-                                                                    fields=_data_fields,
-                                                                    skip_header=True
-                                                                    )
-                    _validation_data: TabularDataset = TabularDataset(path=self.validation_data_path,
-                                                                      format='csv',
-                                                                      fields=_data_fields,
-                                                                      skip_header=True
-                                                                      )
-                    if self.model_param.get('embedding_model') == 'fast_text':
-                        self.embedding_text.build_vocab(_train_data,
-                                                        vectors=EMBEDDING[self.model_param.get('embedding_model')](language='de' if self.model_param.get('lang') is None else self.model_param.get('lang'))
-                                                        )
-                    self.embedding_label.build_vocab(_train_data)
-                    if 0 in _unique_labels:
-                        for label in _unique_labels:
-                            self.embedding_label.vocab.stoi.update({str(label): label})
-                    else:
-                        for label in _unique_labels:
-                            self.embedding_label.vocab.stoi.update({str(label): label - 1})
-                    self.model_param.update(dict(weights=self.embedding_text.vocab.vectors, vocab_size=len(self.embedding_text.vocab)))
-                    if self.test_data_path is None:
-                        self.train_iter, self.validation_iter = BucketIterator.splits((_train_data, _validation_data),
-                                                                                      batch_size=int(self.model_param.get('batch_size')),
-                                                                                      sort_key=lambda x: len(x.text),
-                                                                                      repeat=False,
-                                                                                      shuffle=True
-                                                                                      )
-                    else:
-                        self.train_iter, self.validation_iter, self.test_iter = BucketIterator.splits((_train_data, _validation_data, _test_data),
-                                                                                                      batch_size=int(self.model_param.get('batch_size')),
-                                                                                                      sort_key=lambda x: len(x.text),
-                                                                                                      repeat=False,
-                                                                                                      shuffle=True
-                                                                                                      )
+        if self.learning_type == 'batch':
+            if self.sequential_type == 'text':
+                _unique_labels: list = pd.read_csv(filepath_or_buffer=self.train_data_path, sep=self.sep)[self.target].unique().tolist()
+                _data_fields: List[tuple] = []
+                self.embedding_text: Field = Field(sequential=True,
+                                                   tokenize=lambda x: x.split(),
+                                                   lower=True,
+                                                   include_lengths=True,
+                                                   batch_first=True,
+                                                   fix_length=300 if self.model_param.get('embedding_len') is None else self.model_param.get('embedding_len')
+                                                   )
+                self.embedding_label: Field = Field(sequential=False, is_target=True, unk_token=None)
+                for predictor in self.predictors:
+                    _data_fields.append((predictor, self.embedding_text))
+                _data_fields.append((self.target, self.embedding_label))
+                _train_data: TabularDataset = TabularDataset(path=self.train_data_path,
+                                                             format='csv',
+                                                             fields=_data_fields,
+                                                             skip_header=True
+                                                             )
+                if self.test_data_path is None:
+                    _test_data = None
                 else:
-                    self.train_data_df = DataImporter(file_path=self.train_data_path,
-                                                      as_data_frame=True,
-                                                      use_dask=False,
-                                                      create_dir=False,
-                                                      sep=self.sep,
-                                                      cloud=self.cloud,
-                                                      bucket_name=self.bucket_name
-                                                      ).file(table_name=None)
-                    self.test_data_df = DataImporter(file_path=self.test_data_path,
-                                                     as_data_frame=True,
-                                                     use_dask=False,
-                                                     create_dir=False,
-                                                     sep=self.sep,
-                                                     cloud=self.cloud,
-                                                     bucket_name=self.bucket_name
-                                                     ).file(table_name=None)
-                    self.val_data_df = DataImporter(file_path=self.validation_data_path,
-                                                    as_data_frame=True,
-                                                    use_dask=False,
-                                                    create_dir=False,
-                                                    sep=self.sep,
-                                                    cloud=self.cloud,
-                                                    bucket_name=self.bucket_name
-                                                    ).file(table_name=None)
-                    _train_predictor_tensor: torch.tensor = torch.tensor(data=self.train_data_df['text'].values)
-                    _test_predictor_tensor: torch.tensor = torch.tensor(data=self.test_data_df['text'].values)
-                    _val_predictor_tensor: torch.tensor = torch.tensor(data=self.val_data_df['text'].values)
-                    _train_target_tensor: torch.tensor = torch.tensor(data=self.train_data_df['label'].values.astype(np.float32))
-                    _test_target_tensor: torch.tensor = torch.tensor(data=self.test_data_df['label'].values.astype(np.float32))
-                    _val_target_tensor: torch.tensor = torch.tensor(data=self.val_data_df['label'].values.astype(np.float32))
-                    _train_data_tensor: TensorDataset = TensorDataset(_train_predictor_tensor, _train_target_tensor)
-                    _test_data_tensor: TensorDataset = TensorDataset(_test_predictor_tensor, _test_target_tensor)
-                    _val_data_tensor: TensorDataset = TensorDataset(_val_predictor_tensor, _val_target_tensor)
-                    self.train_iter = DataLoader(dataset=_train_data_tensor, shuffle=True, batch_size=int(self.model_param.get('batch_size')))
-                    self.test_iter = DataLoader(dataset=_test_data_tensor, shuffle=True, batch_size=int(self.model_param.get('batch_size')))
-                    self.validation_iter = DataLoader(dataset=_val_data_tensor, shuffle=True, batch_size=int(self.model_param.get('batch_size')))
-                    self.train_data_df = None
-                    self.test_data_df = None
-                    self.val_data_df = None
-                    del _train_predictor_tensor, _train_target_tensor
-                    del _test_predictor_tensor, _test_target_tensor
-                    del _val_predictor_tensor, _val_target_tensor
-                    del _train_data_tensor, _test_data_tensor, _val_data_tensor
-            elif self.learning_type == 'stochastic':
-                raise NeuralNetworkException('Importing data set for stochastic learning not implemented yet')
+                    _test_data: TabularDataset = TabularDataset(path=self.test_data_path,
+                                                                format='csv',
+                                                                fields=_data_fields,
+                                                                skip_header=True
+                                                                )
+                _validation_data: TabularDataset = TabularDataset(path=self.validation_data_path,
+                                                                  format='csv',
+                                                                  fields=_data_fields,
+                                                                  skip_header=True
+                                                                  )
+                if self.model_param.get('embedding_model') == 'fast_text':
+                    self.embedding_text.build_vocab(_train_data,
+                                                    vectors=EMBEDDING[self.model_param.get('embedding_model')](language='de' if self.model_param.get('lang') is None else self.model_param.get('lang'))
+                                                    )
+                self.embedding_label.build_vocab(_train_data)
+                if 0 in _unique_labels:
+                    for label in _unique_labels:
+                        self.embedding_label.vocab.stoi.update({str(label): label})
+                else:
+                    for label in _unique_labels:
+                        self.embedding_label.vocab.stoi.update({str(label): label - 1})
+                self.model_param.update(dict(weights=self.embedding_text.vocab.vectors, vocab_size=len(self.embedding_text.vocab)))
+                if self.test_data_path is None:
+                    self.train_iter, self.validation_iter = BucketIterator.splits((_train_data, _validation_data),
+                                                                                  batch_size=int(self.model_param.get('batch_size')),
+                                                                                  sort_key=lambda x: len(x.text),
+                                                                                  repeat=False,
+                                                                                  shuffle=True
+                                                                                  )
+                else:
+                    self.train_iter, self.validation_iter, self.test_iter = BucketIterator.splits((_train_data, _validation_data, _test_data),
+                                                                                                  batch_size=int(self.model_param.get('batch_size')),
+                                                                                                  sort_key=lambda x: len(x.text),
+                                                                                                  repeat=False,
+                                                                                                  shuffle=True
+                                                                                                  )
             else:
-                raise NeuralNetworkException('Learning type ({}) not supported'.format(self.learning_type))
-            self.x_train = None
-            self.y_train = None
-            self.x_test = None
-            self.y_test = None
-            self.x_val = None
-            self.y_val = None
-            del _train_data
-            del _test_data
-            del _validation_data
-
-    def _predict_transformer(self, text_data: str):
-        """
-        Get prediction from pre-trained neural network (transformer only)
-
-        :param text_data: str
-            Text data sequence
-        """
-        _predictions, _raw_output = self.model.model.predict(to_predict=[text_data], multi_label=False if self.output_size <= 2 else True)
-        return _predictions
+                self.train_data_df = DataImporter(file_path=self.train_data_path,
+                                                  as_data_frame=True,
+                                                  use_dask=False,
+                                                  create_dir=False,
+                                                  sep=self.sep,
+                                                  cloud=self.cloud,
+                                                  bucket_name=self.bucket_name
+                                                  ).file(table_name=None)
+                self.test_data_df = DataImporter(file_path=self.test_data_path,
+                                                 as_data_frame=True,
+                                                 use_dask=False,
+                                                 create_dir=False,
+                                                 sep=self.sep,
+                                                 cloud=self.cloud,
+                                                 bucket_name=self.bucket_name
+                                                 ).file(table_name=None)
+                self.val_data_df = DataImporter(file_path=self.validation_data_path,
+                                                as_data_frame=True,
+                                                use_dask=False,
+                                                create_dir=False,
+                                                sep=self.sep,
+                                                cloud=self.cloud,
+                                                bucket_name=self.bucket_name
+                                                ).file(table_name=None)
+                _train_predictor_tensor: torch.tensor = torch.tensor(data=self.train_data_df['text'].values)
+                _test_predictor_tensor: torch.tensor = torch.tensor(data=self.test_data_df['text'].values)
+                _val_predictor_tensor: torch.tensor = torch.tensor(data=self.val_data_df['text'].values)
+                _train_target_tensor: torch.tensor = torch.tensor(data=self.train_data_df['label'].values.astype(np.float32))
+                _test_target_tensor: torch.tensor = torch.tensor(data=self.test_data_df['label'].values.astype(np.float32))
+                _val_target_tensor: torch.tensor = torch.tensor(data=self.val_data_df['label'].values.astype(np.float32))
+                _train_data_tensor: TensorDataset = TensorDataset(_train_predictor_tensor, _train_target_tensor)
+                _test_data_tensor: TensorDataset = TensorDataset(_test_predictor_tensor, _test_target_tensor)
+                _val_data_tensor: TensorDataset = TensorDataset(_val_predictor_tensor, _val_target_tensor)
+                self.train_iter = DataLoader(dataset=_train_data_tensor, shuffle=True, batch_size=int(self.model_param.get('batch_size')))
+                self.test_iter = DataLoader(dataset=_test_data_tensor, shuffle=True, batch_size=int(self.model_param.get('batch_size')))
+                self.validation_iter = DataLoader(dataset=_val_data_tensor, shuffle=True, batch_size=int(self.model_param.get('batch_size')))
+                self.train_data_df = None
+                self.test_data_df = None
+                self.val_data_df = None
+                del _train_predictor_tensor, _train_target_tensor
+                del _test_predictor_tensor, _test_target_tensor
+                del _val_predictor_tensor, _val_target_tensor
+                del _train_data_tensor, _test_data_tensor, _val_data_tensor
+        elif self.learning_type == 'stochastic':
+            raise NeuralNetworkException('Importing data set for stochastic learning not implemented yet')
+        else:
+            raise NeuralNetworkException('Learning type ({}) not supported'.format(self.learning_type))
+        self.x_train = None
+        self.y_train = None
+        self.x_test = None
+        self.y_test = None
+        self.x_val = None
+        self.y_val = None
+        del _train_data
+        del _test_data
+        del _validation_data
 
     def _stochastic_learning(self, train: bool = True, eval_set: str = 'val'):
         """
         Train gradient using stochastic learning
 
         :param train: bool
             Training or evaluation mode
@@ -1255,43 +1108,26 @@
                     _observations.extend(_target.detach().numpy().tolist())
                     break
                 if len(_observations) == len(_predictions):
                     self.obs = copy.deepcopy(_observations)
                     self.pred = copy.deepcopy(_predictions)
                     self._eval(iter_type=_iter_type, obs=_observations, pred=_predictions)
 
-    def _train_transformer(self):
-        """
-        Train neural network using deep learning framework 'PyTorch' (transformer only)
-        """
-        self.model.model.train_model(train_df=self.train_data_df,
-                                     multi_label=False,
-                                     output_dir=None,
-                                     show_running_loss=False,
-                                     eval_df=self.val_data_df,
-                                     verbose=False
-                                     )
-        _predictions, _raw_output = self.model.model.predict(to_predict=self.train_data_df[self.predictors[0]].values.tolist())
-        self._eval(iter_type='train', obs=self.train_data_df[self.target].values.tolist(), pred=_predictions.tolist())
-        del _predictions
-        del _raw_output
-
     def generate_model(self):
         """
         Generate supervised machine learning model with randomized parameter configuration
         """
         if self.random:
             if self.models is None:
                 self.model_name = copy.deepcopy(np.random.choice(a=list(NETWORK_TYPE.keys())))
             else:
                 self.model_name = copy.deepcopy(np.random.choice(a=self.models))
             _model = copy.deepcopy(NETWORK_TYPE.get(self.model_name))
         else:
             _model = copy.deepcopy(NETWORK_TYPE.get(self.model_name))
-        self.transformer = True if self.model_name == 'trans' else False
         if len(self.input_param.keys()) == 0:
             self.model_param = getattr(NeuralNetwork(target=self.target,
                                                      predictors=self.predictors,
                                                      output_layer_size=self.output_size,
                                                      x_train=self.x_train,
                                                      y_train=self.y_train,
                                                      x_test=self.x_test,
@@ -1302,19 +1138,18 @@
                                                      test_data_path=self.test_data_path,
                                                      validation_data_path=self.validation_data_path,
                                                      model_param=self.model_param,
                                                      **self.kwargs
                                                      ),
                                        '{}_param'.format(_model)
                                        )()
-            if not self.transformer:
-                self.model_param.update(self._get_param_space(general=True))
-                self._config_params(hidden_layers=True)
-                if self.sequential_type == 'text':
-                    self._config_params(natural_language=True)
+            self.model_param.update(self._get_param_space(general=True))
+            self._config_params(hidden_layers=True)
+            if self.sequential_type == 'text':
+                self._config_params(natural_language=True)
         else:
             self.model_param = copy.deepcopy(self.input_param)
         _idx: int = 0 if len(self.model_param_mutated.keys()) == 0 else len(self.model_param_mutated.keys()) + 1
         self.model_param_mutated.update({str(_idx): {copy.deepcopy(self.model_name): {}}})
         for param in list(self.model_param.keys()):
             self.model_param_mutated[str(_idx)][copy.deepcopy(self.model_name)].update({param: copy.deepcopy(self.model_param.get(param))})
         self.model_param_mutation = 'new_model'
@@ -1376,70 +1211,51 @@
                                               input_param=self.input_param,
                                               model_param=self.model_param,
                                               seed=self.seed,
                                               **self.kwargs
                                               ),
                                 '{}_param'.format(NETWORK_TYPE.get(self.model_name))
                                 )()
-        if self.transformer:
-            _force_param: dict = {} if force_param is None else force_param
-            _param_choices: List[str] = [p for p in list(_params.keys()) if p not in list(_force_param.keys())]
-            _gen_n_params: int = round(len(_params.keys()) * _rate)
-            if _gen_n_params == 0:
-                _gen_n_params = 1
-            self.model_param_mutated.update({len(self.model_param_mutated.keys()) + 1: {copy.deepcopy(self.model_name): {}}})
-            for param in list(_force_param.keys()):
-                self.model_param.update({param: copy.deepcopy(_force_param.get(param))})
-            _old_model_param: dict = copy.deepcopy(self.model_param)
-            for _ in range(0, _gen_n_params, 1):
-                while True:
-                    _param: str = np.random.choice(a=_param_choices)
-                    if _old_model_param.get(_param) is not None:
-                        if self.model_param.get(_param) is not None:
-                            break
-                self.model_param_mutated[list(self.model_param_mutated.keys())[-1]][copy.deepcopy(self.model_name)].update({_param: self.model_param.get(_param)})
-            self.model_param_mutation = 'params'
-        else:
-            for fixed in ['hidden_layers', 'hidden_layer_size_category']:
-                if fixed in list(self.model_param.keys()):
-                    del _params[fixed]
-            _force_param: dict = {} if force_param is None else force_param
-            _param_choices: List[str] = [p for p in list(_params.keys()) if p not in list(_force_param.keys())]
-            _gen_n_params: int = round(len(_params.keys()) * _rate)
-            if _gen_n_params == 0:
-                _gen_n_params = 1
-            self.model_param_mutated.update({len(self.model_param_mutated.keys()) + 1: {copy.deepcopy(self.model_name): {}}})
-            for param in list(_force_param.keys()):
-                self.model_param.update({param: copy.deepcopy(_force_param.get(param))})
-            _old_model_param: dict = copy.deepcopy(self.model_param)
-            _ignore_param: List[str] = IGNORE_PARAM_FOR_OPTIMIZATION
-            if self.learning_type == 'batch':
-                _ignore_param.append('batch_size')
-            elif self.learning_type == 'stochastic':
-                _ignore_param.append('sample_size')
-            _parameters: List[str] = [p for p in _param_choices if p not in _ignore_param]
-            for _ in range(0, _gen_n_params, 1):
-                while True:
-                    _param: str = np.random.choice(a=_parameters)
-                    if _old_model_param.get(_param) is not None:
-                        if self.model_param.get(_param) is not None:
-                            break
-                if _param == 'loss':
-                    self._config_params(loss=True)
-                elif _param == 'optimizer':
-                    self._config_params(optimizer=True)
-                elif _param == 'hidden_layers':
-                    self._config_params(hidden_layers=True)
-                else:
-                    if _param in self._get_param_space(general=True).keys():
-                        self.model_param.update({_param: copy.deepcopy(self._get_param_space(general=True).get(_param))})
-                    elif _param in self._get_param_space(general=False).keys():
-                        self.model_param.update({_param: copy.deepcopy(self._get_param_space(general=False).get(_param))})
-                self.model_param_mutated[list(self.model_param_mutated.keys())[-1]][copy.deepcopy(self.model_name)].update({_param: self.model_param.get(_param)})
-            self.model_param_mutation = 'new_model'
+        for fixed in ['hidden_layers', 'hidden_layer_size_category']:
+            if fixed in list(self.model_param.keys()):
+                del _params[fixed]
+        _force_param: dict = {} if force_param is None else force_param
+        _param_choices: List[str] = [p for p in list(_params.keys()) if p not in list(_force_param.keys())]
+        _gen_n_params: int = round(len(_params.keys()) * _rate)
+        if _gen_n_params == 0:
+            _gen_n_params = 1
+        self.model_param_mutated.update({len(self.model_param_mutated.keys()) + 1: {copy.deepcopy(self.model_name): {}}})
+        for param in list(_force_param.keys()):
+            self.model_param.update({param: copy.deepcopy(_force_param.get(param))})
+        _old_model_param: dict = copy.deepcopy(self.model_param)
+        _ignore_param: List[str] = IGNORE_PARAM_FOR_OPTIMIZATION
+        if self.learning_type == 'batch':
+            _ignore_param.append('batch_size')
+        elif self.learning_type == 'stochastic':
+            _ignore_param.append('sample_size')
+        _parameters: List[str] = [p for p in _param_choices if p not in _ignore_param]
+        for _ in range(0, _gen_n_params, 1):
+            while True:
+                _param: str = np.random.choice(a=_parameters)
+                if _old_model_param.get(_param) is not None:
+                    if self.model_param.get(_param) is not None:
+                        break
+            if _param == 'loss':
+                self._config_params(loss=True)
+            elif _param == 'optimizer':
+                self._config_params(optimizer=True)
+            elif _param == 'hidden_layers':
+                self._config_params(hidden_layers=True)
+            else:
+                if _param in self._get_param_space(general=True).keys():
+                    self.model_param.update({_param: copy.deepcopy(self._get_param_space(general=True).get(_param))})
+                elif _param in self._get_param_space(general=False).keys():
+                    self.model_param.update({_param: copy.deepcopy(self._get_param_space(general=False).get(_param))})
+            self.model_param_mutated[list(self.model_param_mutated.keys())[-1]][copy.deepcopy(self.model_name)].update({_param: self.model_param.get(_param)})
+        self.model_param_mutation = 'new_model'
         if len(self.predictors) > 0:
             if self.target != '':
                 self._import_data_torch()
             else:
                 raise NeuralNetworkException('No target feature found')
         else:
             raise NeuralNetworkException('No predictors found')
@@ -1462,89 +1278,44 @@
                              )()
 
     def get_vanilla_model(self):
         """
         Get 'vanilla' typed neural network (one hidden layer only)
         """
         if self.model_name is not None:
-            if self.transformer:
-                if len(self.input_param.keys()) == 0:
-                    self.model_param = getattr(NeuralNetwork(target=self.target,
-                                                             predictors=self.predictors,
-                                                             output_layer_size=self.output_size,
-                                                             x_train=self.x_train,
-                                                             y_train=self.y_train,
-                                                             x_test=self.x_test,
-                                                             y_test=self.y_test,
-                                                             x_val=self.x_val,
-                                                             y_val=self.y_val,
-                                                             train_data_path=self.train_data_path,
-                                                             test_data_path=self.test_data_path,
-                                                             validation_data_path=self.validation_data_path,
-                                                             **self.kwargs
-                                                             ),
-                                               '{}_param'.format(NETWORK_TYPE.get(self.model_name))
-                                               )()
-                else:
-                    self.model_param = copy.deepcopy(self.input_param)
-                if len(self.predictors) > 0:
-                    if self.target != '':
-                        self._import_data_torch()
-                    else:
-                        raise NeuralNetworkException('No target feature found')
-                else:
-                    raise NeuralNetworkException('No predictors found')
-                self.model = getattr(NeuralNetwork(target=self.target,
-                                                   predictors=self.predictors,
-                                                   output_layer_size=self.output_size,
-                                                   x_train=self.x_train,
-                                                   y_train=self.y_train,
-                                                   x_test=self.x_test,
-                                                   y_test=self.y_test,
-                                                   x_val=self.x_val,
-                                                   y_val=self.y_val,
-                                                   train_data_path=self.train_data_path,
-                                                   test_data_path=self.test_data_path,
-                                                   validation_data_path=self.validation_data_path,
-                                                   model_param=self.model_param,
-                                                   **self.kwargs
-                                                   ),
-                                     NETWORK_TYPE.get(self.model_name)
-                                     )()
+            if len(self.input_param.keys()) == 0:
+                self.model_param = getattr(NeuralNetwork(target=self.target,
+                                                         predictors=self.predictors,
+                                                         output_layer_size=self.output_size,
+                                                         x_train=self.x_train,
+                                                         y_train=self.y_train,
+                                                         x_test=self.x_test,
+                                                         y_test=self.y_test,
+                                                         x_val=self.x_val,
+                                                         y_val=self.y_val,
+                                                         train_data_path=self.train_data_path,
+                                                         test_data_path=self.test_data_path,
+                                                         validation_data_path=self.validation_data_path,
+                                                         **self.kwargs
+                                                         ),
+                                           '{}_param'.format(NETWORK_TYPE.get(self.model_name))
+                                           )()
+                self.model_param.update(self._get_param_space(general=True))
+                self.model_param.update(learning_rate=0.001)
+                if self.sequential_type == 'text':
+                    self._config_params(natural_language=True)
             else:
-                if len(self.input_param.keys()) == 0:
-                    self.model_param = getattr(NeuralNetwork(target=self.target,
-                                                             predictors=self.predictors,
-                                                             output_layer_size=self.output_size,
-                                                             x_train=self.x_train,
-                                                             y_train=self.y_train,
-                                                             x_test=self.x_test,
-                                                             y_test=self.y_test,
-                                                             x_val=self.x_val,
-                                                             y_val=self.y_val,
-                                                             train_data_path=self.train_data_path,
-                                                             test_data_path=self.test_data_path,
-                                                             validation_data_path=self.validation_data_path,
-                                                             **self.kwargs
-                                                             ),
-                                               '{}_param'.format(NETWORK_TYPE.get(self.model_name))
-                                               )()
-                    self.model_param.update(self._get_param_space(general=True))
-                    self.model_param.update(learning_rate=0.001)
-                    if self.sequential_type == 'text':
-                        self._config_params(natural_language=True)
-                else:
-                    self.model_param = copy.deepcopy(self.input_param)
-                if len(self.predictors) > 0:
-                    if self.target != '':
-                        self._import_data_torch()
-                    else:
-                        raise NeuralNetworkException('No target feature found')
+                self.model_param = copy.deepcopy(self.input_param)
+            if len(self.predictors) > 0:
+                if self.target != '':
+                    self._import_data_torch()
                 else:
-                    raise NeuralNetworkException('No predictors found')
+                    raise NeuralNetworkException('No target feature found')
+            else:
+                raise NeuralNetworkException('No predictors found')
             self.model = getattr(NeuralNetwork(target=self.target,
                                                predictors=self.predictors,
                                                output_layer_size=self.output_size,
                                                x_train=self.x_train,
                                                y_train=self.y_train,
                                                x_test=self.x_test,
                                                y_test=self.y_test,
@@ -1563,34 +1334,18 @@
     def eval(self, validation: bool = True):
         """
         Evaluate supervised machine learning classification model
 
         :param validation: bool
             Whether to run validation or testing iteration
         """
-        if self.transformer:
-            if validation:
-                _predictions, _raw_output = self.model.model.predict(to_predict=self.val_data_df[self.predictors[0]].values.tolist())
-                self._eval(iter_type='val', obs=self.val_data_df[self.target].values.tolist(), pred=_predictions)
-            else:
-                _predictions, _raw_output = self.model.model.predict(to_predict=self.test_data_df[self.predictors[0]].values.tolist())
-                self._eval(iter_type='test', obs=self.test_data_df[self.target].values.tolist(), pred=_predictions)
-            # _result, _predictions_val, _wrong_predictions = self.model.model.eval_model(eval_df=self.val_data_df,
-            #                                                                            multi_label=False,
-            #                                                                            output_dir=None,
-            #                                                                            show_running_loss=True,
-            #                                                                            verbose=True
-            #                                                                            )
-            del _predictions
-            del _raw_output
-        else:
-            if self.learning_type == 'batch':
-                self._batch_learning(train=False, eval_set='val' if validation else 'test')
-            elif self.learning_type == 'stochastic':
-                self._stochastic_learning()
+        if self.learning_type == 'batch':
+            self._batch_learning(train=False, eval_set='val' if validation else 'test')
+        elif self.learning_type == 'stochastic':
+            self._stochastic_learning()
 
     def predict(self):
         """
         Get prediction from pre-trained neural network using PyTorch
         """
         if self.test_iter is None:
             self.eval(validation=True)
@@ -1600,44 +1355,30 @@
     def save(self, file_path: str):
         """
         Save PyTorch model to disk
 
         :param file_path: str
             Complete file path of the PyTorch model to save
         """
-        if self.transformer:
-            self.model.save_model(output_dir=file_path,
-                                  optimizer=None,
-                                  scheduler=None,
-                                  model=None,
-                                  results=None
-                                  )
-        else:
-            torch.save(obj=self.model, f=file_path)
+        torch.save(obj=self.model, f=file_path)
 
     def train(self):
         """
         Train neural network using deep learning framework 'PyTorch'
         """
         _t0: datetime = datetime.now()
-        if self.transformer:
-            self._train_transformer()
-            self.train_time = (datetime.now() - _t0).seconds
-            self.eval(validation=True)
-            self.eval(validation=False)
-        else:
-            for _ in range(0, self.model_param.get('epoch'), 1):
-                print('\nEpoch: {}'.format(_))
-                if self.learning_type == 'batch':
-                    self._batch_learning(train=True)
-                    self.eval(validation=True)
-                elif self.learning_type == 'stochastic':
-                    self._stochastic_learning()
-                self._epoch_eval(iter_types=['train', 'val'])
-            self.train_time = (datetime.now() - _t0).seconds
+        for _ in range(0, self.model_param.get('epoch'), 1):
+            print('\nEpoch: {}'.format(_))
+            if self.learning_type == 'batch':
+                self._batch_learning(train=True)
+                self.eval(validation=True)
+            elif self.learning_type == 'stochastic':
+                self._stochastic_learning()
+            self._epoch_eval(iter_types=['train', 'val'])
+        self.train_time = (datetime.now() - _t0).seconds
 
     def update_data(self,
                     x_train: np.ndarray,
                     y_train: np.array,
                     x_test: np.ndarray,
                     y_test: np.array,
                     x_val: np.ndarray,
```

### Comparing `happy_learning-0.4.6/happy_learning/neural_network_torch.py` & `happy_learning-0.4.7/happy_learning/neural_network_torch.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 """
 
 import numpy as np
 import torch
 import torch.nn as nn
 
-from simpletransformers.model import ClassificationModel
 from torch.autograd import Variable
 from torch.nn import functional
 from typing import List
 
 INITIALIZER: dict = dict(#constant=torch.nn.init.constant_,
                          #eye=torch.nn.init.eye_,
                          #dirac=torch.nn.init.dirac_,
@@ -641,102 +640,7 @@
         _c_0 = torch.autograd.Variable(torch.zeros(2, self.batch_size, self.hidden_size))
         _output, (_h_n, _c_n) = self.lstm_layer(_input, (_h_0, _c_0))
         _output = _output.permute(1, 0, 2)
         _attention_weight_matrix = self.attention_network(lstm_output=_output)
         _hidden_matrix = torch.bmm(_attention_weight_matrix, _output)
         _fully_connected_output = self.fc_layer(_hidden_matrix.view(-1, _hidden_matrix.size()[1] * _hidden_matrix.size()[2]))
         return self.output_layer(_fully_connected_output)
-
-
-class Transformers:
-    """
-    Class for building encoder decoder transformer networks using simpletransformers based on hugging face
-    """
-    def __init__(self, parameters: dict, output_size: int, cache_dir: str = None):
-        """
-        :param parameters: dict
-			Parameter settings
-
-        :param output_size: int
-            Output size:
-                -> 1: Float value (Regression)
-                -> 2: Classes (Binary Classification)
-                -> >2: Classes (Multi-Class Classification)
-
-        :param cache_dir: str
-            Cache directory for loading pre-trained language (embedding) models from disk
-        """
-        self.args: dict = dict(model_type=parameters.get('model_type'),
-                               model_name=parameters.get('model_name'),
-                               regression=False if output_size > 1 else True,
-                               num_train_epochs=parameters.get('epoch'),
-                               learning_rate=parameters.get('learning_rate'),
-                               train_batch_size=parameters.get('batch_size'),
-                               eval_batch_size=parameters.get('batch_size'),
-                               max_seq_length=512,
-                               adafactor_beta1=parameters.get('adafactor_beta1'),
-                               adafactor_clip_threshold=parameters.get('adafactor_clip_threshold'),
-                               adafactor_decay_rate=parameters.get('adafactor_decay_rate'),
-                               adafactor_eps=parameters.get('adafactor_eps'),
-                               adafactor_relative_step=parameters.get('adafactor_relative_step'),
-                               adafactor_scale_parameter=parameters.get('adafactor_scale_parameter'),
-                               adafactor_warmup_init=parameters.get('adafactor_warmup_init'),
-                               adam_epsilon=parameters.get('adam_epsilon'),
-                               cosine_schedule_num_cycles=parameters.get('cosine_schedule_num_cycles'),
-                               dynamic_quantize=parameters.get('dynamic_quantize'),
-                               early_stopping_consider_epochs=parameters.get('early_stopping_consider_epochs'),
-                               use_early_stopping=parameters.get('use_early_stopping'),
-                               early_stopping_delta=parameters.get('early_stopping_delta'),
-                               early_stopping_patience=parameters.get('early_stopping_patience'),
-                               attention_probs_dropout_prob=parameters.get('attention_probs_dropout_prob'),
-                               hidden_size=parameters.get('hidden_size'),
-                               hidden_dropout_prob=parameters.get('hidden_dropout_prob'),
-                               initializer_range=parameters.get('initializer_range'),
-                               layer_norm_eps=parameters.get('layer_norm_eps'),
-                               num_attention_heads=parameters.get('num_attention_heads'),
-                               num_hidden_layers=parameters.get('num_hidden_layers'),
-                               optimizer=parameters.get('optimizer'),
-                               scheduler=parameters.get('scheduler'),
-                               polynomial_decay_schedule_lr_end=parameters.get('polynomial_decay_schedule_lr_end'),
-                               polynomial_decay_schedule_power=parameters.get('polynomial_decay_schedule_power'),
-                               weight_decay=parameters.get('weight_decay'),
-                               gradient_accumulation_steps=parameters.get('gradient_accumulation_steps'),
-                               max_grad_norm=parameters.get('max_grad_norm'),
-                               early_stopping_metric='eval_loss',
-                               early_stopping_metric_minimize=True,
-                               sliding_window=False,
-                               manual_seed=1234,
-                               warmup_ratio=parameters.get('warmup_ratio'),
-                               warmup_step=parameters.get('warmup_step'),
-                               save_steps=2000,
-                               logging_steps=100,
-                               evaluate_during_training=True,
-                               eval_all_checkpoints=False,
-                               use_tensorboard=True,
-                               overwrite_output_dir=True,
-                               reprocess_input_data=True,
-                               do_lower_case=True,
-                               no_save=True,
-                               no_cache=False,
-                               silent=True,
-                               best_model_dir=BEST_MODEL_DIR,
-                               output_dir=OUTPUT_DIR,
-                               cache_dir=CACHE_DIR,
-                               fp16=parameters.get('fp16'),
-                               fp16_opt_level=parameters.get('fp16_opt_level')
-                               )
-        _kwargs: dict = dict(cache_dir=cache_dir, local_files_only=False if cache_dir is None else True)
-        self.model = ClassificationModel(model_type=parameters.get('model_type'),
-                                         model_name=parameters.get('model_name'),
-                                         tokenizer_type=None,
-                                         tokenizer_name=None,
-                                         num_labels=output_size,
-                                         weight=None,
-                                         args=self.args,
-                                         use_cuda=torch.cuda.is_available(),
-                                         cuda_device=0 if torch.cuda.is_available() else -1,
-                                         onnx_execution_provider=None,
-                                         **_kwargs
-                                         )
-
-    def forward(self) -> ClassificationModel:
-        return self.model
```

### Comparing `happy_learning-0.4.6/happy_learning/sampler.py` & `happy_learning-0.4.7/happy_learning/sampler.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/self_taught_short_text_clustering.py` & `happy_learning-0.4.7/happy_learning/self_taught_short_text_clustering.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/supervised_machine_learning.py` & `happy_learning-0.4.7/happy_learning/supervised_machine_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/swarm_intelligence.py` & `happy_learning-0.4.7/happy_learning/swarm_intelligence.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/text_clustering.py` & `happy_learning-0.4.7/happy_learning/text_clustering.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/text_clustering_generator.py` & `happy_learning-0.4.7/happy_learning/text_clustering_generator.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/text_miner.py` & `happy_learning-0.4.7/happy_learning/text_miner.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning/utils.py` & `happy_learning-0.4.7/happy_learning/utils.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/happy_learning.egg-info/PKG-INFO` & `happy_learning-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
-Name: happy-learning
-Version: 0.4.6
+Name: happy_learning
+Version: 0.4.7
 Summary: Toolbox for reinforced developing of machine learning models (as proof-of-concept)
 Home-page: https://github.com/GianniBalistreri/happy_learning
 Author: Gianni Francesco Balistreri
 Author-email: gbalistreri@gmx.de
 License: GNU
 Keywords: feature-engineering feature-selection evolutionary-algorithm machine-learning automl reinforcement-learning deep-learning shapley clustering pytorch
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -215,9 +214,7 @@
     -- Generate similarity / clustering features:
         Apply similarity methods to generate continuous features using word embeddings
             -> TF-IDF
 
 ## 4. Documentation & Examples:
 
 Check the methodology.pdf for the documentation and jupyter notebook for examples. Happy ;) Learning
-
-
```

### Comparing `happy_learning-0.4.6/happy_learning.egg-info/SOURCES.txt` & `happy_learning-0.4.7/happy_learning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/setup.py` & `happy_learning-0.4.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools
 import subprocess
 import sys
 
 #from happy_learning.text_miner import LANG_MODELS
 
 # Install complete dask library for handling big data sets using parallel computing:
-subprocess.run(['python{} -m pip install "dask[distributed]"'.format('3' if sys.platform.find('win') != 0 else '')], shell=True)
-subprocess.run(['python{} -m pip install "dask[complete]"'.format('3' if sys.platform.find('win') != 0 else '')], shell=True)
+#subprocess.run(['python{} -m pip install "dask[distributed]"'.format('3' if sys.platform.find('win') != 0 else '')], shell=True)
+#subprocess.run(['python{} -m pip install "dask[complete]"'.format('3' if sys.platform.find('win') != 0 else '')], shell=True)
 
-# Install jupyter notebook extensions for using EasyExplore_examples.ipynb more conveniently:
-subprocess.run(['python{} -m pip install jupyter_contrib_nbextensions && jupyter contrib nbextension install'.format('3' if sys.platform.find('win') != 0 else '')], shell=True)
+# Install jupyter notebook extensions:
+#subprocess.run(['python{} -m pip install jupyter_contrib_nbextensions && jupyter contrib nbextension install'.format('3' if sys.platform.find('win') != 0 else '')], shell=True)
 
 # Install spacy language models:
 #subprocess.run('python{} -m pip install spacy'.format('3' if sys.platform.find('win') != 0 else ''), shell=True)
 #for lang in LANG_MODELS.keys():
 #    for model in LANG_MODELS[lang]['model']['spacy'].keys():
 #        subprocess.run('python{} -m spacy download {}'.format('3' if sys.platform.find('win') != 0 else '',
 #                                                              LANG_MODELS[lang]['model']['spacy'][model]
@@ -26,15 +26,15 @@
 with open('requirements.txt', 'r') as _requirements:
     requires = _requirements.read()
 
 requires = [r.strip() for r in requires.split('\n') if ((r.strip()[0] != "#") and (len(r.strip()) > 3) and "-e git://" not in r)]
 
 setuptools.setup(
     name='happy_learning',
-    version='0.4.6',
+    version='0.4.7',
     author='Gianni Francesco Balistreri',
     author_email='gbalistreri@gmx.de',
     description='Toolbox for reinforced developing of machine learning models (as proof-of-concept)',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='feature-engineering feature-selection evolutionary-algorithm machine-learning automl reinforcement-learning deep-learning shapley clustering pytorch',
     license='GNU',
```

### Comparing `happy_learning-0.4.6/test/test_data_miner.py` & `happy_learning-0.4.7/test/test_data_miner.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/test/test_deep_q_learning.py` & `happy_learning-0.4.7/test/test_deep_q_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/test/test_environment_modeling.py` & `happy_learning-0.4.7/test/test_environment_modeling.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/test/test_evaluate_machine_learning.py` & `happy_learning-0.4.7/test/test_evaluate_machine_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/test/test_feature_engineer.py` & `happy_learning-0.4.7/test/test_feature_engineer.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/test/test_feature_learning.py` & `happy_learning-0.4.7/test/test_feature_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/test/test_feature_selector.py` & `happy_learning-0.4.7/test/test_feature_selector.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/test/test_feature_tournament.py` & `happy_learning-0.4.7/test/test_feature_tournament.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/test/test_genetic_algorithm.py` & `happy_learning-0.4.7/test/test_genetic_algorithm.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/test/test_missing_data_analysis.py` & `happy_learning-0.4.7/test/test_missing_data_analysis.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/test/test_multiple_imputation.py` & `happy_learning-0.4.7/test/test_multiple_imputation.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/test/test_neural_network_generator_torch.py` & `happy_learning-0.4.7/test/test_neural_network_generator_torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import copy
 import pandas as pd
 import unittest
 
-from happy_learning.neural_network_torch import Attention, GRU, LSTM, MLP, RCNN, RNN, SelfAttention, Transformers
+from happy_learning.neural_network_torch import Attention, GRU, LSTM, MLP, RCNN, RNN, SelfAttention
 from happy_learning.neural_network_generator_torch import NETWORK_TYPE, NetworkGenerator
 from happy_learning.sampler import MLSampler
 from typing import List
 
 
 TARGET: str = 'AveragePrice'
 PREDICTORS: List[str] = ['4046', '4225', '4770']
@@ -132,53 +132,28 @@
                                             test_data_path=TEST_DATA_PATH_TEXT,
                                             validation_data_path=VALIDATION_DATA_PATH_TEXT,
                                             models=['self'],
                                             sep=','
                                             ).generate_model()
         self.assertTrue(expr=isinstance(_net_gen.model, SelfAttention))
 
-    def test_generate_transformer_model(self):
-        _net_gen: object = NetworkGenerator(target=TARGET_TEXT,
-                                            predictors=PREDICTORS_TEXT,
-                                            output_layer_size=5,
-                                            train_data_path=TRAIN_DATA_PATH_TEXT,
-                                            test_data_path=TEST_DATA_PATH_TEXT,
-                                            validation_data_path=VALIDATION_DATA_PATH_TEXT,
-                                            models=['trans'],
-                                            sep=','
-                                            ).generate_model()
-        self.assertTrue(expr=isinstance(_net_gen.model, Transformers))
-
     def test_generate_params(self):
         _net_gen: object = NetworkGenerator(target=TARGET_TEXT,
                                             predictors=PREDICTORS_TEXT,
                                             output_layer_size=5,
                                             train_data_path=TRAIN_DATA_PATH_TEXT,
                                             test_data_path=TEST_DATA_PATH_TEXT,
                                             validation_data_path=VALIDATION_DATA_PATH_TEXT,
                                             models=list(NETWORK_TYPE.keys())
                                             ).generate_model()
         _model = _net_gen.generate_model()
         _mutated_param: dict = copy.deepcopy(_model.model_param_mutated)
         _net_gen.generate_params(param_rate=0.1, force_param=None)
         self.assertTrue(expr=len(_mutated_param.keys()) < len(_net_gen.model_param_mutated.keys()))
 
-    def test_get_vanilla_transformer(self):
-        _net_gen: object = NetworkGenerator(target=TARGET_TEXT,
-                                            predictors=PREDICTORS_TEXT,
-                                            output_layer_size=5,
-                                            train_data_path=TRAIN_DATA_PATH_TEXT,
-                                            test_data_path=TEST_DATA_PATH_TEXT,
-                                            validation_data_path=VALIDATION_DATA_PATH_TEXT,
-                                            models=['trans'],
-                                            model_name='trans',
-                                            sep=','
-                                            )
-        _model = _net_gen.get_vanilla_model()
-
     def test_eval(self):
         _net_gen: object = NetworkGenerator(target=TARGET_TEXT,
                                             predictors=PREDICTORS_TEXT,
                                             output_layer_size=5,
                                             train_data_path=TRAIN_DATA_PATH_TEXT,
                                             test_data_path=TEST_DATA_PATH_TEXT,
                                             validation_data_path=VALIDATION_DATA_PATH_TEXT,
@@ -212,15 +187,15 @@
     def test_train(self):
         _net_gen: object = NetworkGenerator(target=TARGET_TEXT,
                                             predictors=PREDICTORS_TEXT,
                                             output_layer_size=5,
                                             train_data_path=TRAIN_DATA_PATH_TEXT,
                                             test_data_path=TEST_DATA_PATH_TEXT,
                                             validation_data_path=VALIDATION_DATA_PATH_TEXT,
-                                            models=['trans'],#list(NETWORK_TYPE.keys()),
+                                            models=['rcnn'],#list(NETWORK_TYPE.keys()),
                                             sep=','
                                             )
         _model = _net_gen.generate_model()
         _model.train()
         self.assertTrue(expr=_model.fitness.get('train') is not None)
 
     def test_update_data(self):
```

### Comparing `happy_learning-0.4.6/test/test_neural_network_torch.py` & `happy_learning-0.4.7/test/test_neural_network_torch.py`

 * *Files 7% similar despite different names*

```diff
@@ -154,28 +154,9 @@
                                                                 sep=','
                                                                 )
         _network_generator.get_vanilla_model()
         _network_generator.train()
         self.assertTrue(expr=len(_network_generator.fitness.keys()) > 0)
 
 
-class TransformerTest(unittest.TestCase):
-    """
-    Class for testing class Transformer (torch)
-    """
-    def test_forward(self):
-        _network_generator: NetworkGenerator = NetworkGenerator(target='label',
-                                                                predictors=['text'],
-                                                                output_layer_size=5,
-                                                                train_data_path=DATA_FILE_PATH.get('train'),
-                                                                test_data_path=DATA_FILE_PATH.get('test'),
-                                                                validation_data_path=DATA_FILE_PATH.get('val'),
-                                                                model_name='trans',
-                                                                sep=','
-                                                                )
-        _network_generator.get_vanilla_model()
-        _network_generator.train()
-        self.assertTrue(expr=len(_network_generator.fitness.keys()) > 0)
-
-
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `happy_learning-0.4.6/test/test_sampler.py` & `happy_learning-0.4.7/test/test_sampler.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/test/test_supervised_machine_learning.py` & `happy_learning-0.4.7/test/test_supervised_machine_learning.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/test/test_swarm_intelligence.py` & `happy_learning-0.4.7/test/test_swarm_intelligence.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/test/test_text_clustering.py` & `happy_learning-0.4.7/test/test_text_clustering.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/test/test_text_clustering_generator.py` & `happy_learning-0.4.7/test/test_text_clustering_generator.py`

 * *Files identical despite different names*

### Comparing `happy_learning-0.4.6/test/test_text_miner.py` & `happy_learning-0.4.7/test/test_text_miner.py`

 * *Files identical despite different names*

