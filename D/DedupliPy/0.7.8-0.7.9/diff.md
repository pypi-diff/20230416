# Comparing `tmp/DedupliPy-0.7.8.tar.gz` & `tmp/DedupliPy-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/fritshermans/Documents/deduplipy/dist/tmp_z2oupj_/DedupliPy-0.7.8.tar", last modified: Sun Apr  3 09:13:29 2022, max compression
+gzip compressed data, was "/Users/fritshermans/Documents/deduplipy/dist/tmpnymixy8k/DedupliPy-0.7.9.tar", last modified: Sun Apr  3 16:03:36 2022, max compression
```

## Comparing `DedupliPy-0.7.8.tar` & `DedupliPy-0.7.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 09:13:29.000000 DedupliPy-0.7.8/
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 09:13:29.000000 DedupliPy-0.7.8/DedupliPy.egg-info/
--rw-r--r--   0 fritshermans   (501) staff       (20)     3492 2022-04-03 09:13:28.000000 DedupliPy-0.7.8/DedupliPy.egg-info/PKG-INFO
--rw-r--r--   0 fritshermans   (501) staff       (20)     1212 2022-04-03 09:13:29.000000 DedupliPy-0.7.8/DedupliPy.egg-info/SOURCES.txt
--rw-r--r--   0 fritshermans   (501) staff       (20)        1 2022-04-03 09:13:28.000000 DedupliPy-0.7.8/DedupliPy.egg-info/dependency_links.txt
--rw-r--r--   0 fritshermans   (501) staff       (20)      461 2022-04-03 09:13:29.000000 DedupliPy-0.7.8/DedupliPy.egg-info/requires.txt
--rw-r--r--   0 fritshermans   (501) staff       (20)       10 2022-04-03 09:13:29.000000 DedupliPy-0.7.8/DedupliPy.egg-info/top_level.txt
--rw-r--r--   0 fritshermans   (501) staff       (20)     1070 2021-05-04 14:47:45.000000 DedupliPy-0.7.8/LICENSE
--rw-r--r--   0 fritshermans   (501) staff       (20)     3492 2022-04-03 09:13:29.000000 DedupliPy-0.7.8/PKG-INFO
--rw-r--r--   0 fritshermans   (501) staff       (20)     2988 2022-01-25 17:52:41.000000 DedupliPy-0.7.8/README.md
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 09:13:29.000000 DedupliPy-0.7.8/deduplipy/
--rw-r--r--   0 fritshermans   (501) staff       (20)       22 2022-04-03 09:09:47.000000 DedupliPy-0.7.8/deduplipy/__init__.py
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 09:13:29.000000 DedupliPy-0.7.8/deduplipy/active_learning/
--rw-r--r--   0 fritshermans   (501) staff       (20)       94 2021-04-20 16:52:14.000000 DedupliPy-0.7.8/deduplipy/active_learning/__init__.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     8248 2022-03-07 18:15:18.000000 DedupliPy-0.7.8/deduplipy/active_learning/active_learning.py
--rw-r--r--   0 fritshermans   (501) staff       (20)      596 2021-10-29 15:08:59.000000 DedupliPy-0.7.8/deduplipy/active_learning/utils_active_learning.py
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 09:13:29.000000 DedupliPy-0.7.8/deduplipy/blocking/
--rw-r--r--   0 fritshermans   (501) staff       (20)      196 2021-06-18 15:04:38.000000 DedupliPy-0.7.8/deduplipy/blocking/__init__.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     5257 2022-01-02 16:27:51.000000 DedupliPy-0.7.8/deduplipy/blocking/blocking.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     4000 2022-04-03 09:11:46.000000 DedupliPy-0.7.8/deduplipy/blocking/blocking_rules.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     2523 2021-05-06 17:56:34.000000 DedupliPy-0.7.8/deduplipy/blocking/set_cover.py
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 09:13:29.000000 DedupliPy-0.7.8/deduplipy/classifier_pipeline/
--rw-r--r--   0 fritshermans   (501) staff       (20)       86 2021-04-29 14:44:28.000000 DedupliPy-0.7.8/deduplipy/classifier_pipeline/__init__.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     2342 2022-01-02 16:21:50.000000 DedupliPy-0.7.8/deduplipy/classifier_pipeline/classifier_pipeline.py
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 09:13:29.000000 DedupliPy-0.7.8/deduplipy/clustering/
--rw-r--r--   0 fritshermans   (501) staff       (20)      160 2022-03-27 17:24:35.000000 DedupliPy-0.7.8/deduplipy/clustering/__init__.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     2538 2022-03-27 17:24:35.000000 DedupliPy-0.7.8/deduplipy/clustering/clustering.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     1216 2022-04-02 17:14:16.000000 DedupliPy-0.7.8/deduplipy/clustering/fill_missing_edges.py
--rw-r--r--   0 fritshermans   (501) staff       (20)      228 2022-03-27 17:24:35.000000 DedupliPy-0.7.8/deduplipy/config.py
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 09:13:29.000000 DedupliPy-0.7.8/deduplipy/data/
--rw-r--r--   0 fritshermans   (501) staff       (20)    13367 2021-04-10 13:53:23.000000 DedupliPy-0.7.8/deduplipy/data/stoxx50_extended_with_id.xlsx
--rw-r--r--   0 fritshermans   (501) staff       (20)    52700 2021-05-04 08:25:31.000000 DedupliPy-0.7.8/deduplipy/data/voter_names.csv
--rw-r--r--   0 fritshermans   (501) staff       (20)   535135 2021-11-02 18:44:54.000000 DedupliPy-0.7.8/deduplipy/data/voter_names_17k.csv
--rw-r--r--   0 fritshermans   (501) staff       (20)  1048954 2021-11-02 18:39:56.000000 DedupliPy-0.7.8/deduplipy/data/voter_names_35k.csv
--rw-r--r--   0 fritshermans   (501) staff       (20)  2488637 2021-11-02 17:44:06.000000 DedupliPy-0.7.8/deduplipy/data/voter_names_80k.csv
--rw-r--r--   0 fritshermans   (501) staff       (20)     1204 2022-04-03 07:39:34.000000 DedupliPy-0.7.8/deduplipy/datasets.py
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 09:13:29.000000 DedupliPy-0.7.8/deduplipy/deduplicator/
--rw-r--r--   0 fritshermans   (501) staff       (20)       67 2021-04-20 16:52:58.000000 DedupliPy-0.7.8/deduplipy/deduplicator/__init__.py
--rw-r--r--   0 fritshermans   (501) staff       (20)    10030 2022-04-03 08:34:06.000000 DedupliPy-0.7.8/deduplipy/deduplicator/deduplicator.py
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 09:13:29.000000 DedupliPy-0.7.8/deduplipy/sampling/
--rw-r--r--   0 fritshermans   (501) staff       (20)      132 2022-01-02 14:35:37.000000 DedupliPy-0.7.8/deduplipy/sampling/__init__.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     5872 2022-01-02 16:33:57.000000 DedupliPy-0.7.8/deduplipy/sampling/minhash_sampling.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     2302 2022-01-02 16:33:57.000000 DedupliPy-0.7.8/deduplipy/sampling/naive_sampling.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     1051 2022-01-02 14:35:37.000000 DedupliPy-0.7.8/deduplipy/sampling/sampler.py
-drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 09:13:29.000000 DedupliPy-0.7.8/deduplipy/string_metrics/
--rw-r--r--   0 fritshermans   (501) staff       (20)      233 2021-05-10 18:42:39.000000 DedupliPy-0.7.8/deduplipy/string_metrics/__init__.py
--rw-r--r--   0 fritshermans   (501) staff       (20)     2060 2022-01-02 18:32:59.000000 DedupliPy-0.7.8/deduplipy/string_metrics/string_metrics.py
--rw-r--r--   0 fritshermans   (501) staff       (20)      103 2021-05-04 13:45:36.000000 DedupliPy-0.7.8/pyproject.toml
--rw-r--r--   0 fritshermans   (501) staff       (20)       38 2022-04-03 09:13:29.000000 DedupliPy-0.7.8/setup.cfg
--rw-r--r--   0 fritshermans   (501) staff       (20)     1333 2022-04-03 09:09:47.000000 DedupliPy-0.7.8/setup.py
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/DedupliPy.egg-info/
+-rw-r--r--   0 fritshermans   (501) staff       (20)     3492 2022-04-03 16:03:35.000000 DedupliPy-0.7.9/DedupliPy.egg-info/PKG-INFO
+-rw-r--r--   0 fritshermans   (501) staff       (20)     1212 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/DedupliPy.egg-info/SOURCES.txt
+-rw-r--r--   0 fritshermans   (501) staff       (20)        1 2022-04-03 16:03:35.000000 DedupliPy-0.7.9/DedupliPy.egg-info/dependency_links.txt
+-rw-r--r--   0 fritshermans   (501) staff       (20)      461 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/DedupliPy.egg-info/requires.txt
+-rw-r--r--   0 fritshermans   (501) staff       (20)       10 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/DedupliPy.egg-info/top_level.txt
+-rw-r--r--   0 fritshermans   (501) staff       (20)     1070 2021-05-04 14:47:45.000000 DedupliPy-0.7.9/LICENSE
+-rw-r--r--   0 fritshermans   (501) staff       (20)     3492 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/PKG-INFO
+-rw-r--r--   0 fritshermans   (501) staff       (20)     2988 2022-04-03 14:20:08.000000 DedupliPy-0.7.9/README.md
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/deduplipy/
+-rw-r--r--   0 fritshermans   (501) staff       (20)       22 2022-04-03 16:02:24.000000 DedupliPy-0.7.9/deduplipy/__init__.py
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/deduplipy/active_learning/
+-rw-r--r--   0 fritshermans   (501) staff       (20)       94 2021-04-20 16:52:14.000000 DedupliPy-0.7.9/deduplipy/active_learning/__init__.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     9429 2022-04-03 15:56:00.000000 DedupliPy-0.7.9/deduplipy/active_learning/active_learning.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)      596 2022-04-03 14:20:08.000000 DedupliPy-0.7.9/deduplipy/active_learning/utils_active_learning.py
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/deduplipy/blocking/
+-rw-r--r--   0 fritshermans   (501) staff       (20)      196 2021-06-18 15:04:38.000000 DedupliPy-0.7.9/deduplipy/blocking/__init__.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     5257 2022-04-03 14:20:08.000000 DedupliPy-0.7.9/deduplipy/blocking/blocking.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     4000 2022-04-03 14:20:08.000000 DedupliPy-0.7.9/deduplipy/blocking/blocking_rules.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     2523 2021-05-06 17:56:34.000000 DedupliPy-0.7.9/deduplipy/blocking/set_cover.py
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/deduplipy/classifier_pipeline/
+-rw-r--r--   0 fritshermans   (501) staff       (20)       86 2021-04-29 14:44:28.000000 DedupliPy-0.7.9/deduplipy/classifier_pipeline/__init__.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     2342 2022-04-03 14:21:19.000000 DedupliPy-0.7.9/deduplipy/classifier_pipeline/classifier_pipeline.py
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/deduplipy/clustering/
+-rw-r--r--   0 fritshermans   (501) staff       (20)      160 2022-04-03 14:20:03.000000 DedupliPy-0.7.9/deduplipy/clustering/__init__.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     2538 2022-04-03 14:20:08.000000 DedupliPy-0.7.9/deduplipy/clustering/clustering.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     1216 2022-04-02 17:14:16.000000 DedupliPy-0.7.9/deduplipy/clustering/fill_missing_edges.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)      228 2022-04-03 14:20:03.000000 DedupliPy-0.7.9/deduplipy/config.py
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/deduplipy/data/
+-rw-r--r--   0 fritshermans   (501) staff       (20)    13367 2021-04-10 13:53:23.000000 DedupliPy-0.7.9/deduplipy/data/stoxx50_extended_with_id.xlsx
+-rw-r--r--   0 fritshermans   (501) staff       (20)    52700 2021-05-04 08:25:31.000000 DedupliPy-0.7.9/deduplipy/data/voter_names.csv
+-rw-r--r--   0 fritshermans   (501) staff       (20)   535135 2021-11-02 18:44:54.000000 DedupliPy-0.7.9/deduplipy/data/voter_names_17k.csv
+-rw-r--r--   0 fritshermans   (501) staff       (20)  1048954 2021-11-02 18:39:56.000000 DedupliPy-0.7.9/deduplipy/data/voter_names_35k.csv
+-rw-r--r--   0 fritshermans   (501) staff       (20)  2488637 2021-11-02 17:44:06.000000 DedupliPy-0.7.9/deduplipy/data/voter_names_80k.csv
+-rw-r--r--   0 fritshermans   (501) staff       (20)     1204 2022-04-03 07:39:34.000000 DedupliPy-0.7.9/deduplipy/datasets.py
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/deduplipy/deduplicator/
+-rw-r--r--   0 fritshermans   (501) staff       (20)       67 2021-04-20 16:52:58.000000 DedupliPy-0.7.9/deduplipy/deduplicator/__init__.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)    10030 2022-04-03 14:21:19.000000 DedupliPy-0.7.9/deduplipy/deduplicator/deduplicator.py
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/deduplipy/sampling/
+-rw-r--r--   0 fritshermans   (501) staff       (20)      132 2022-04-03 14:20:08.000000 DedupliPy-0.7.9/deduplipy/sampling/__init__.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     5922 2022-04-03 15:17:25.000000 DedupliPy-0.7.9/deduplipy/sampling/minhash_sampling.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     2485 2022-04-03 15:28:39.000000 DedupliPy-0.7.9/deduplipy/sampling/naive_sampling.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     1051 2022-04-03 14:20:08.000000 DedupliPy-0.7.9/deduplipy/sampling/sampler.py
+drwxr-xr-x   0 fritshermans   (501) staff       (20)        0 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/deduplipy/string_metrics/
+-rw-r--r--   0 fritshermans   (501) staff       (20)      233 2021-05-10 18:42:39.000000 DedupliPy-0.7.9/deduplipy/string_metrics/__init__.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)     2060 2022-04-03 14:20:08.000000 DedupliPy-0.7.9/deduplipy/string_metrics/string_metrics.py
+-rw-r--r--   0 fritshermans   (501) staff       (20)      103 2021-05-04 13:45:36.000000 DedupliPy-0.7.9/pyproject.toml
+-rw-r--r--   0 fritshermans   (501) staff       (20)       38 2022-04-03 16:03:36.000000 DedupliPy-0.7.9/setup.cfg
+-rw-r--r--   0 fritshermans   (501) staff       (20)     1333 2022-04-03 16:02:24.000000 DedupliPy-0.7.9/setup.py
```

### Comparing `DedupliPy-0.7.8/DedupliPy.egg-info/PKG-INFO` & `DedupliPy-0.7.9/DedupliPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DedupliPy
-Version: 0.7.8
+Version: 0.7.9
 Summary: End-to-end deduplication solution
 Home-page: https://github.com/fritshermans/deduplipy
 Author: Frits Hermans
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: DedupliPy Version: 0.7.8 Summary: End-to-end
+Metadata-Version: 2.1 Name: DedupliPy Version: 0.7.9 Summary: End-to-end
 deduplication solution Home-page: https://github.com/fritshermans/deduplipy
 Author: Frits Hermans License: UNKNOWN Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6.9
 Description-Content-Type: text/markdown Provides-Extra: base Provides-Extra:
 dev Provides-Extra: docs License-File: LICENSE  [![Version](https://
 img.shields.io/pypi/v/deduplipy)](https://pypi.org/project/deduplipy/) ![]
```

### Comparing `DedupliPy-0.7.8/DedupliPy.egg-info/SOURCES.txt` & `DedupliPy-0.7.9/DedupliPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.8/LICENSE` & `DedupliPy-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.8/PKG-INFO` & `DedupliPy-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DedupliPy
-Version: 0.7.8
+Version: 0.7.9
 Summary: End-to-end deduplication solution
 Home-page: https://github.com/fritshermans/deduplipy
 Author: Frits Hermans
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: DedupliPy Version: 0.7.8 Summary: End-to-end
+Metadata-Version: 2.1 Name: DedupliPy Version: 0.7.9 Summary: End-to-end
 deduplication solution Home-page: https://github.com/fritshermans/deduplipy
 Author: Frits Hermans License: UNKNOWN Platform: UNKNOWN Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6.9
 Description-Content-Type: text/markdown Provides-Extra: base Provides-Extra:
 dev Provides-Extra: docs License-File: LICENSE  [![Version](https://
 img.shields.io/pypi/v/deduplipy)](https://pypi.org/project/deduplipy/) ![]
```

### Comparing `DedupliPy-0.7.8/README.md` & `DedupliPy-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.8/deduplipy/active_learning/active_learning.py` & `DedupliPy-0.7.9/deduplipy/active_learning/active_learning.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         self.uncertainty_improvement_threshold = uncertainty_improvement_threshold
         self.min_nr_entries = min_nr_entries
         self.verbose = verbose
         self.learner = ActiveLearner(
             estimator=ClassifierPipeline(interaction=interaction),
             query_strategy=uncertainty_sampling,
         )
+        self.uncertainties = []
         self.counter_total = 0
         self.counter_positive = 0
         self.counter_negative = 0
 
     def _get_last_uncertainty_improvement(self, last_n: int = 5) -> Optional[float]:
         """
         Calculates the uncertainty differences during active learning. The largest difference over the `last_n`
@@ -103,30 +104,54 @@
         """
         X_all = pd.concat((self.train_samples, X))
         probas = self.learner.predict_proba(X_all['similarities'].tolist())[:, 1]
         count, division = np.histogram(probas, bins=np.arange(0, 1.01, 0.05))
         hist = pd.DataFrame({'count': count, 'score': division[1:]})
         print(hist[['score', 'count']].to_string(index=False))
 
-    def _print_min_max_scores(self, X):
+    def _print_min_max_scores(self, X: pd.DataFrame):
+        """
+        Print lowest and highest scores on training data to monitor level of logistic regression asymptotes during
+        active learning
+
+        Args:
+            X: Pandas dataframe containing pairs table with pairs that remain as candidates to be labelled
+
+        """
         X_all = pd.concat((self.train_samples, X))
         pred_max = self.learner.predict_proba(X_all['similarities'].tolist()).max(axis=0)
         print(f'lowest score: {1 - pred_max[0]:.2f}')
         print(f'highest score: {pred_max[1]:.2f}')
 
+    def _fit_synthetic_perfect_matches(self, X: pd.DataFrame) -> pd.DataFrame:
+        """
+        Fit the perfect matches that are generated during pairs table creation. The column `synthetic_perfect_match`
+        contains a boolean whether the pair is a synthetic perfect match. Note that perfect matches that are not
+        artificially created are not used to train the classifier by this method.
+
+        Args:
+            X: Pandas dataframe containing pairs table with column `synthetic_perfect_match`
+
+        Returns:
+            Pandas dataframe with the synthetic perfect matches removed
+
+        """
+        self.train_samples = X[X['synthetic_perfect_match']]
+        X = X[~X['synthetic_perfect_match']].reset_index(drop=True)
+        self.learner.teach(np.array(self.train_samples['similarities'].tolist()), np.ones(len(self.train_samples)))
+        return X
+
     def fit(self, X: pd.DataFrame) -> 'ActiveStringMatchLearner':
         """
         Fit ActiveStringMatchLearner instance on pairs of strings
 
         Args:
             X: Pandas dataframe containing pairs of strings
         """
-        self.uncertainties = []
-
-        self.train_samples = pd.DataFrame([])
+        X = self._fit_synthetic_perfect_matches(X)
         query_inst_prev = None
         uncertainty = None
         for i in range(N_QUERIES):
             query_idx, query_inst = self.learner.query(np.array(X['similarities'].tolist()))
             try:
                 uncertainty = 1 - (self.learner.predict_proba(query_inst)[0]).max()
                 self.uncertainties.append(uncertainty)
```

### Comparing `DedupliPy-0.7.8/deduplipy/active_learning/utils_active_learning.py` & `DedupliPy-0.7.9/deduplipy/active_learning/utils_active_learning.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.8/deduplipy/blocking/blocking.py` & `DedupliPy-0.7.9/deduplipy/blocking/blocking.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.8/deduplipy/blocking/blocking_rules.py` & `DedupliPy-0.7.9/deduplipy/blocking/blocking_rules.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.8/deduplipy/blocking/set_cover.py` & `DedupliPy-0.7.9/deduplipy/blocking/set_cover.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.8/deduplipy/classifier_pipeline/classifier_pipeline.py` & `DedupliPy-0.7.9/deduplipy/classifier_pipeline/classifier_pipeline.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.8/deduplipy/clustering/clustering.py` & `DedupliPy-0.7.9/deduplipy/clustering/clustering.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.8/deduplipy/clustering/fill_missing_edges.py` & `DedupliPy-0.7.9/deduplipy/clustering/fill_missing_edges.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.8/deduplipy/data/stoxx50_extended_with_id.xlsx` & `DedupliPy-0.7.9/deduplipy/data/stoxx50_extended_with_id.xlsx`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.8/deduplipy/data/voter_names.csv` & `DedupliPy-0.7.9/deduplipy/data/voter_names.csv`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.8/deduplipy/data/voter_names_17k.csv` & `DedupliPy-0.7.9/deduplipy/data/voter_names_17k.csv`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.8/deduplipy/data/voter_names_35k.csv` & `DedupliPy-0.7.9/deduplipy/data/voter_names_35k.csv`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.8/deduplipy/data/voter_names_80k.csv` & `DedupliPy-0.7.9/deduplipy/data/voter_names_80k.csv`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.8/deduplipy/datasets.py` & `DedupliPy-0.7.9/deduplipy/datasets.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.8/deduplipy/deduplicator/deduplicator.py` & `DedupliPy-0.7.9/deduplipy/deduplicator/deduplicator.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.8/deduplipy/sampling/minhash_sampling.py` & `DedupliPy-0.7.9/deduplipy/sampling/minhash_sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,9 +128,10 @@
         minhash_pairs = self._create_minhash_pairs(X, threshold)
 
         stratified_sample = self._get_stratified_sample(minhash_pairs, n_samples)
 
         non_stratified_sample = self._get_non_stratified_sample(minhash_pairs, stratified_sample, n_samples)
 
         sample = stratified_sample.append(non_stratified_sample)[self.pairs_col_names]
+        sample['synthetic_perfect_match'] = False
 
         return sample
```

### Comparing `DedupliPy-0.7.8/deduplipy/sampling/naive_sampling.py` & `DedupliPy-0.7.9/deduplipy/sampling/naive_sampling.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+from functools import reduce
 from itertools import product
+from operator import and_
 from typing import List
 
 import numpy as np
 import pandas as pd
 
 from deduplipy.config import ROW_ID, N_PERFECT_MATCHES_TRAIN
 from .sampler import Sampler
@@ -42,17 +44,18 @@
                          df_sample[self.col_names + [ROW_ID]].values.tolist())))
 
         pairs_table[[f'{x}_1' for x in self.col_names + [ROW_ID]]] = pairs_table[0].to_list()
         pairs_table[[f'{x}_2' for x in self.col_names + [ROW_ID]]] = pairs_table[1].to_list()
         pairs_table.drop(columns=[0, 1], inplace=True)
 
         pairs_table.sort_values([f'{ROW_ID}_1', f'{ROW_ID}_2'], inplace=True)
+        pairs_table['synthetic_perfect_match'] = False
 
         perfect_matches = pairs_table[pairs_table[f'{ROW_ID}_1'] == pairs_table[f'{ROW_ID}_2']].iloc[
                           :self.n_perfect_matches]
+        perfect_matches['synthetic_perfect_match'] = True
 
         pairs_table = pairs_table[
             pairs_table[f'{ROW_ID}_1'] < pairs_table[f'{ROW_ID}_2']]
         pairs_table = perfect_matches.append(pairs_table, ignore_index=True)
-        pairs_table = pairs_table[self.pairs_col_names].reset_index(
-            drop=True)
+        pairs_table = pairs_table[self.pairs_col_names+['synthetic_perfect_match']].reset_index(drop=True)
         return pairs_table.head(n_samples)
```

### Comparing `DedupliPy-0.7.8/deduplipy/sampling/sampler.py` & `DedupliPy-0.7.9/deduplipy/sampling/sampler.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.8/deduplipy/string_metrics/string_metrics.py` & `DedupliPy-0.7.9/deduplipy/string_metrics/string_metrics.py`

 * *Files identical despite different names*

### Comparing `DedupliPy-0.7.8/setup.py` & `DedupliPy-0.7.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 dev_packages = base_packages + util_packages + docs_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(name='DedupliPy',
-      version='0.7.8',
+      version='0.7.9',
       author="Frits Hermans",
       description="End-to-end deduplication solution",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/fritshermans/deduplipy",
       classifiers=[
           "Programming Language :: Python :: 3",
```

