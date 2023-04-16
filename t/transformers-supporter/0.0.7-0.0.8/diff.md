# Comparing `tmp/transformers-supporter-0.0.7.tar.gz` & `tmp/transformers-supporter-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers-supporter-0.0.7.tar", last modified: Sun Mar 12 10:55:53 2023, max compression
+gzip compressed data, was "transformers-supporter-0.0.8.tar", last modified: Sun Apr 16 16:31:40 2023, max compression
```

## Comparing `transformers-supporter-0.0.7.tar` & `transformers-supporter-0.0.8.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 10:55:53.065014 transformers-supporter-0.0.7/
--rw-r--r--   0 root         (0) root         (0)     2319 2023-03-12 10:55:53.065014 transformers-supporter-0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2023 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-12 10:55:53.065014 transformers-supporter-0.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      618 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 10:55:53.057014 transformers-supporter-0.0.7/transformers_supporter/
--rw-r--r--   0 root         (0) root         (0)       45 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 10:55:53.058014 transformers-supporter-0.0.7/transformers_supporter/models/
--rw-r--r--   0 root         (0) root         (0)     1936 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 10:55:53.059013 transformers-supporter-0.0.7/transformers_supporter/models/ann/
--rw-r--r--   0 root         (0) root         (0)       96 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/ann/__init__.py
--rw-r--r--   0 root         (0) root         (0)      753 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/ann/configuration_ann.py
--rw-r--r--   0 root         (0) root         (0)     6060 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/ann/feature_extraction_ann.py
--rw-r--r--   0 root         (0) root         (0)     4388 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/ann/modeling_ann.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 10:55:53.059013 transformers-supporter-0.0.7/transformers_supporter/models/cnn/
--rw-r--r--   0 root         (0) root         (0)       94 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/cnn/__init__.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/cnn/configuration_cnn.py
--rw-r--r--   0 root         (0) root         (0)     4714 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/cnn/image_processing_cnn.py
--rw-r--r--   0 root         (0) root         (0)     3743 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/cnn/modeling_cnn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 10:55:53.060013 transformers-supporter-0.0.7/transformers_supporter/models/custom_bert/
--rw-r--r--   0 root         (0) root         (0)       75 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/custom_bert/__init__.py
--rw-r--r--   0 root         (0) root         (0)      812 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/custom_bert/configuration_custom_bert.py
--rw-r--r--   0 root         (0) root         (0)     2949 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/custom_bert/modeling_custom_bert.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 10:55:53.060013 transformers-supporter-0.0.7/transformers_supporter/models/custom_wav2vec2/
--rw-r--r--   0 root         (0) root         (0)       49 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/custom_wav2vec2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2748 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/custom_wav2vec2/feature_extraction_custom_wav2vec2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 10:55:53.061014 transformers-supporter-0.0.7/transformers_supporter/models/embedded_1dcnn/
--rw-r--r--   0 root         (0) root         (0)       81 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/embedded_1dcnn/__init__.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/embedded_1dcnn/configuration_embedded_1dcnn.py
--rw-r--r--   0 root         (0) root         (0)     2292 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/embedded_1dcnn/modeling_embedded_1dcnn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 10:55:53.062013 transformers-supporter-0.0.7/transformers_supporter/models/embedded_rnn/
--rw-r--r--   0 root         (0) root         (0)      117 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/embedded_rnn/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1329 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/embedded_rnn/configuration_embedded_rnn.py
--rw-r--r--   0 root         (0) root         (0)     6466 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/embedded_rnn/modeling_embedded_rnn.py
--rw-r--r--   0 root         (0) root         (0)     5639 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/embedded_rnn/tokenization_embedded_rnn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 10:55:53.062013 transformers-supporter-0.0.7/transformers_supporter/models/faster_rcnn/
--rw-r--r--   0 root         (0) root         (0)      118 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/faster_rcnn/__init__.py
--rw-r--r--   0 root         (0) root         (0)      512 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/faster_rcnn/configuration_faster_rcnn.py
--rw-r--r--   0 root         (0) root         (0)     3626 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/faster_rcnn/image_processing_faster_rcnn.py
--rw-r--r--   0 root         (0) root         (0)     4103 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/faster_rcnn/modeling_faster_rcnn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 10:55:53.063013 transformers-supporter-0.0.7/transformers_supporter/models/rnn/
--rw-r--r--   0 root         (0) root         (0)       59 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/rnn/__init__.py
--rw-r--r--   0 root         (0) root         (0)      398 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/rnn/configuration_rnn.py
--rw-r--r--   0 root         (0) root         (0)     3391 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/models/rnn/modeling_rnn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 10:55:53.064014 transformers-supporter-0.0.7/transformers_supporter/pipelines/
--rw-r--r--   0 root         (0) root         (0)      633 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1372 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/pipelines/custom_image_classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1528 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/pipelines/fixed_length_translation_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1645 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/pipelines/tabular_binary_classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1617 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/pipelines/tabular_classification_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1110 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter/pipelines/tabular_regression_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 10:55:53.058014 transformers-supporter-0.0.7/transformers_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2319 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2407 2023-03-12 10:55:53.000000 transformers-supporter-0.0.7/transformers_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       45 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-03-12 10:55:52.000000 transformers-supporter-0.0.7/transformers_supporter.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.628436 transformers-supporter-0.0.8/
+-rw-r--r--   0 root         (0) root         (0)     2414 2023-04-16 16:31:40.628436 transformers-supporter-0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 16:31:40.628436 transformers-supporter-0.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      618 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.621436 transformers-supporter-0.0.8/transformers_supporter/
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.622436 transformers-supporter-0.0.8/transformers_supporter/models/
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.623436 transformers-supporter-0.0.8/transformers_supporter/models/ann/
+-rw-r--r--   0 root         (0) root         (0)       96 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/ann/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/ann/configuration_ann.py
+-rw-r--r--   0 root         (0) root         (0)     6060 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/ann/feature_extraction_ann.py
+-rw-r--r--   0 root         (0) root         (0)     4462 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/ann/modeling_ann.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.623436 transformers-supporter-0.0.8/transformers_supporter/models/cnn/
+-rw-r--r--   0 root         (0) root         (0)       94 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/cnn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/cnn/configuration_cnn.py
+-rw-r--r--   0 root         (0) root         (0)     4714 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/cnn/image_processing_cnn.py
+-rw-r--r--   0 root         (0) root         (0)     3743 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/cnn/modeling_cnn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.624436 transformers-supporter-0.0.8/transformers_supporter/models/custom_bert/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/custom_bert/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      812 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/custom_bert/configuration_custom_bert.py
+-rw-r--r--   0 root         (0) root         (0)     2949 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/custom_bert/modeling_custom_bert.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.624436 transformers-supporter-0.0.8/transformers_supporter/models/custom_wav2vec2/
+-rw-r--r--   0 root         (0) root         (0)       49 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/custom_wav2vec2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2748 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/custom_wav2vec2/feature_extraction_custom_wav2vec2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.625436 transformers-supporter-0.0.8/transformers_supporter/models/embedded_1dcnn/
+-rw-r--r--   0 root         (0) root         (0)       81 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/embedded_1dcnn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/embedded_1dcnn/configuration_embedded_1dcnn.py
+-rw-r--r--   0 root         (0) root         (0)     2292 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/embedded_1dcnn/modeling_embedded_1dcnn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.625436 transformers-supporter-0.0.8/transformers_supporter/models/embedded_rnn/
+-rw-r--r--   0 root         (0) root         (0)      117 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/embedded_rnn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1329 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/embedded_rnn/configuration_embedded_rnn.py
+-rw-r--r--   0 root         (0) root         (0)     6524 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/embedded_rnn/modeling_embedded_rnn.py
+-rw-r--r--   0 root         (0) root         (0)     5639 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/embedded_rnn/tokenization_embedded_rnn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.626436 transformers-supporter-0.0.8/transformers_supporter/models/faster_rcnn/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/faster_rcnn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      512 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/faster_rcnn/configuration_faster_rcnn.py
+-rw-r--r--   0 root         (0) root         (0)     3626 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/faster_rcnn/image_processing_faster_rcnn.py
+-rw-r--r--   0 root         (0) root         (0)     4103 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/faster_rcnn/modeling_faster_rcnn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.626436 transformers-supporter-0.0.8/transformers_supporter/models/rnn/
+-rw-r--r--   0 root         (0) root         (0)       59 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/rnn/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      398 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/rnn/configuration_rnn.py
+-rw-r--r--   0 root         (0) root         (0)     3432 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/models/rnn/modeling_rnn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.627436 transformers-supporter-0.0.8/transformers_supporter/pipelines/
+-rw-r--r--   0 root         (0) root         (0)      633 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/pipelines/custom_image_classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/pipelines/fixed_length_translation_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/pipelines/tabular_binary_classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/pipelines/tabular_classification_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-04-16 16:31:39.000000 transformers-supporter-0.0.8/transformers_supporter/pipelines/tabular_regression_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:31:40.622436 transformers-supporter-0.0.8/transformers_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2414 2023-04-16 16:31:40.000000 transformers-supporter-0.0.8/transformers_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2407 2023-04-16 16:31:40.000000 transformers-supporter-0.0.8/transformers_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 16:31:40.000000 transformers-supporter-0.0.8/transformers_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 16:31:40.000000 transformers-supporter-0.0.8/transformers_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       48 2023-04-16 16:31:40.000000 transformers-supporter-0.0.8/transformers_supporter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-04-16 16:31:40.000000 transformers-supporter-0.0.8/transformers_supporter.egg-info/top_level.txt
```

### Comparing `transformers-supporter-0.0.7/PKG-INFO` & `transformers-supporter-0.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 Metadata-Version: 2.1
 Name: transformers-supporter
-Version: 0.0.7
+Version: 0.0.8
 Summary: Transformers supporter
 Home-page: https://github.com/automatethem/transformers-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
+https://pypi.org/project/transformers-supporter
+<pre>
+pip install transformers-supporter
+</pre>
+
 Supported models 
 
 <pre>
 import transformers_supporter
 
 #ANN
-transformers_supporter.models.ANNConfig
-transformers_supporter.models.ANNForTabularRegression
+transformers_supporter.models.AnnConfig
+transformers_supporter.models.AnnForTabularRegression
 transformers_supporter.models.AnnForTabularBinaryClassification
 transformers_supporter.models.AnnForTabularClassification
 transformers_supporter.models.TabularFeatureExtractor
 
 #CNN
-transformers_supporter.models.CNNConfig
-transformers_supporter.models.CNNForImageClassification
+transformers_supporter.models.CnnConfig
+transformers_supporter.models.CnnForImageClassification
 transformers_supporter.models.GrayscaleImageProcessor
-transformers_supporter.models.CNNForKeyPointDetection
+transformers_supporter.models.CnnForKeyPointDetection
 
 #RNN
-transformers_supporter.models.RNNConfig
-transformers_supporter.models.RNNForAudioClassification
-transformers_supporter.models.RNNForTimeSeriesRegression
+transformers_supporter.models.RnnConfig
+transformers_supporter.models.RnnForAudioClassification
+transformers_supporter.models.RnnForTimeSeriesRegression
 
 #Embedded RNN
-transformers_supporter.models.EmbeddedRNNConfig
-transformers_supporter.models.EmbeddedRNNForSequenceClassification
-transformers_supporter.models.EmbeddedRNNForFixedLengthTranslation
-transformers_supporter.models.PretrainedEmbeddedRNNForSequenceClassification
+transformers_supporter.models.EmbeddedRnnConfig
+transformers_supporter.models.EmbeddedRnnForSequenceClassification
+transformers_supporter.models.EmbeddedRnnForFixedLengthTranslation
+transformers_supporter.models.PretrainedEmbeddedRnnForSequenceClassification
 transformers_supporter.models.TorchtextTokenizer
 
 #Embedded 1DCNN
-transformers_supporter.models.Embedded1DCNNConfig
-transformers_supporter.models.Embedded1DCNNForSequenceClassification
+transformers_supporter.models.Embedded1dcnnConfig
+transformers_supporter.models.Embedded1dcnnForSequenceClassification
 
 #Faster RCNN
-transformers_supporter.models.FasterRCNNConfig
-transformers_supporter.models.FasterRCNNForObjectDetection
-transformers_supporter.models.FasterRCNNImageProcessor
+transformers_supporter.models.FasterRcnnConfig
+transformers_supporter.models.FasterRcnnForObjectDetection
+transformers_supporter.models.FasterRcnnImageProcessor
 </pre>
 
 <pre>
 import transformers_supporter
 
 #Custom Bert
 transformers_supporter.models.CustomBertConfig
@@ -71,9 +76,7 @@
 transformers_supporter.pipelines.TabularRegressionPipeline
 </pre>
 <pre>
 import transformers_supporter
 
 transformers_supporter.pipelines.CustomImageClassificationPipeline
 </pre>
-
-
```

### Comparing `transformers-supporter-0.0.7/README.md` & `transformers-supporter-0.0.8/transformers_supporter.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,61 @@
+Metadata-Version: 2.1
+Name: transformers-supporter
+Version: 0.0.8
+Summary: Transformers supporter
+Home-page: https://github.com/automatethem/transformers-supporter
+Author: Sang Ki Kwon
+Author-email: automatethem@gmail.com
+License: MIT
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
+https://pypi.org/project/transformers-supporter
+<pre>
+pip install transformers-supporter
+</pre>
+
 Supported models 
 
 <pre>
 import transformers_supporter
 
 #ANN
-transformers_supporter.models.ANNConfig
-transformers_supporter.models.ANNForTabularRegression
+transformers_supporter.models.AnnConfig
+transformers_supporter.models.AnnForTabularRegression
 transformers_supporter.models.AnnForTabularBinaryClassification
 transformers_supporter.models.AnnForTabularClassification
 transformers_supporter.models.TabularFeatureExtractor
 
 #CNN
-transformers_supporter.models.CNNConfig
-transformers_supporter.models.CNNForImageClassification
+transformers_supporter.models.CnnConfig
+transformers_supporter.models.CnnForImageClassification
 transformers_supporter.models.GrayscaleImageProcessor
-transformers_supporter.models.CNNForKeyPointDetection
+transformers_supporter.models.CnnForKeyPointDetection
 
 #RNN
-transformers_supporter.models.RNNConfig
-transformers_supporter.models.RNNForAudioClassification
-transformers_supporter.models.RNNForTimeSeriesRegression
+transformers_supporter.models.RnnConfig
+transformers_supporter.models.RnnForAudioClassification
+transformers_supporter.models.RnnForTimeSeriesRegression
 
 #Embedded RNN
-transformers_supporter.models.EmbeddedRNNConfig
-transformers_supporter.models.EmbeddedRNNForSequenceClassification
-transformers_supporter.models.EmbeddedRNNForFixedLengthTranslation
-transformers_supporter.models.PretrainedEmbeddedRNNForSequenceClassification
+transformers_supporter.models.EmbeddedRnnConfig
+transformers_supporter.models.EmbeddedRnnForSequenceClassification
+transformers_supporter.models.EmbeddedRnnForFixedLengthTranslation
+transformers_supporter.models.PretrainedEmbeddedRnnForSequenceClassification
 transformers_supporter.models.TorchtextTokenizer
 
 #Embedded 1DCNN
-transformers_supporter.models.Embedded1DCNNConfig
-transformers_supporter.models.Embedded1DCNNForSequenceClassification
+transformers_supporter.models.Embedded1dcnnConfig
+transformers_supporter.models.Embedded1dcnnForSequenceClassification
 
 #Faster RCNN
-transformers_supporter.models.FasterRCNNConfig
-transformers_supporter.models.FasterRCNNForObjectDetection
-transformers_supporter.models.FasterRCNNImageProcessor
+transformers_supporter.models.FasterRcnnConfig
+transformers_supporter.models.FasterRcnnForObjectDetection
+transformers_supporter.models.FasterRcnnImageProcessor
 </pre>
 
 <pre>
 import transformers_supporter
 
 #Custom Bert
 transformers_supporter.models.CustomBertConfig
```

### Comparing `transformers-supporter-0.0.7/setup.py` & `transformers-supporter-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='transformers-supporter',
-	version='0.0.7',
+	version='0.0.8',
 	description='Transformers supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/transformers-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

### Comparing `transformers-supporter-0.0.7/transformers_supporter/models/__init__.py` & `transformers-supporter-0.0.8/transformers_supporter/models/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.7/transformers_supporter/models/ann/configuration_ann.py` & `transformers-supporter-0.0.8/transformers_supporter/models/ann/configuration_ann.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from transformers import AutoTokenizer
 from transformers import AutoConfig
 from transformers import AutoModelForSequenceClassification
 import torch
 from torch.nn import functional as F
 import transformers
 
-class ANNConfig(PretrainedConfig):
+class AnnConfig(PretrainedConfig):
     model_type = "ann"
 
     def __init__(self, **kwargs):
         #https://github.com/huggingface/transformers/blob/98d88b23f54e5a23e741833f1e973fdf600cc2c5/src/transformers/configuration_utils.py#L323
         #Keys are always strings in JSON so convert ids to int here.
         super().__init__(**kwargs)
 
 #오토 모델에 등록
 model_path = 'ann'
-AutoConfig.register(model_path, ANNConfig)
+AutoConfig.register(model_path, AnnConfig)
```

### Comparing `transformers-supporter-0.0.7/transformers_supporter/models/ann/feature_extraction_ann.py` & `transformers-supporter-0.0.8/transformers_supporter/models/ann/feature_extraction_ann.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.7/transformers_supporter/models/ann/modeling_ann.py` & `transformers-supporter-0.0.8/transformers_supporter/models/ann/modeling_ann.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from transformers import AutoModel
 from transformers import AutoTokenizer
 from transformers import AutoConfig
 from transformers import AutoModelForSequenceClassification
 import torch
 from torch.nn import functional as F
 import transformers
-from .configuration_ann import ANNConfig
+from .configuration_ann import AnnConfig
 
-class ANNForTabularRegression(PreTrainedModel):
-    config_class = ANNConfig
+class AnnForTabularRegression(PreTrainedModel):
+    config_class = AnnConfig
 
     def __init__(self, config):
         super().__init__(config)
         self.layer = torch.nn.Sequential(
             torch.nn.Linear(in_features=config.in_features, out_features=32),
             #torch.nn.BatchNorm1d(num_features=32),
             torch.nn.ReLU(),
@@ -31,32 +31,33 @@
             #print(labels.shape) #torch.Size([8, 1]) #
             #loss = torch.nn.MSELoss()(logits, labels) 
             loss = F.mse_loss(logits, labels) 
             return transformers.file_utils.ModelOutput({'loss': loss, 'logits': logits})
 
 '''
 #오토 모델에 등록
-AutoModelForTabularRegression.register(ANNConfig, ANNForTabularRegression)
+AutoModelForTabularRegression.register(AnnConfig, AnnForTabularRegression)
 '''
 
 ####################
 
 from transformers import PretrainedConfig
 from transformers import PreTrainedModel
 from transformers import AutoModel
 from transformers import AutoTokenizer
 from transformers import AutoConfig
 from transformers import AutoModelForSequenceClassification
 import transformers
 import torch
 from torch.nn import functional as F
 import transformers
-    
+from .configuration_ann import AnnConfig
+
 class AnnForTabularBinaryClassification(PreTrainedModel):
-    config_class = ANNConfig
+    config_class = AnnConfig
 
     def __init__(self, config):
         super().__init__(config)
         self.layer = torch.nn.Sequential(
             torch.nn.Linear(in_features=config.in_features, out_features=32),
             #torch.nn.BatchNorm1d(num_features=32),
             torch.nn.ReLU(),
@@ -73,31 +74,32 @@
             #print(labels.shape) #torch.Size([2, 3])
             #loss = F.binary_cross_entropy(F.sigmoid(logits), labels)
             loss = F.binary_cross_entropy_with_logits(logits, labels)
             return transformers.file_utils.ModelOutput({'loss': loss, 'logits': logits})
 
 '''
 #오토 모델에 등록
-AutoModelForTabularClassification.register(ANNConfig, AnnForTabularBinaryClassification)
+AutoModelForTabularClassification.register(AnnConfig, AnnForTabularBinaryClassification)
 '''
 
 ####################
 
 from transformers import PretrainedConfig
 from transformers import PreTrainedModel
 from transformers import AutoModel
 from transformers import AutoTokenizer
 from transformers import AutoConfig
 from transformers import AutoModelForSequenceClassification
 import torch
 from torch.nn import functional as F
 import transformers
-    
+from .configuration_ann import AnnConfig
+
 class AnnForTabularClassification(PreTrainedModel):
-    config_class = ANNConfig
+    config_class = AnnConfig
 
     def __init__(self, config):
         super().__init__(config)
         self.layer = torch.nn.Sequential(
             torch.nn.Linear(in_features=config.in_features, out_features=32),
             #torch.nn.BatchNorm1d(num_features=32),
             torch.nn.ReLU(),
@@ -113,11 +115,11 @@
         else:
             #print(labels.shape) #torch.Size([2, 3])
             loss = F.nll_loss(F.log_softmax(logits), labels) #원핫 벡터를 넣을 필요없이 바로 실제값을 인자로 사용 #nll은 Negative Log Likelihood의 약자
             return transformers.file_utils.ModelOutput({'loss': loss, 'logits': logits})
 
 '''
 #오토 모델에 등록
-AutoModelForTabularClassification.register(ANNConfig, AnnForTabularClassification)
+AutoModelForTabularClassification.register(AnnConfig, AnnForTabularClassification)
 '''
 
 ####################
```

### Comparing `transformers-supporter-0.0.7/transformers_supporter/models/cnn/configuration_cnn.py` & `transformers-supporter-0.0.8/transformers_supporter/models/cnn/configuration_cnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from transformers import AutoConfig
 from transformers import AutoModelForImageClassification
 import torch
 from torch.nn import functional as F
 import pytorch_helper
 import transformers
 
-class CNNConfig(PretrainedConfig):
+class CnnConfig(PretrainedConfig):
     model_type = "cnn"
 
     def __init__(self, **kwargs):
         #https://github.com/huggingface/transformers/blob/98d88b23f54e5a23e741833f1e973fdf600cc2c5/src/transformers/configuration_utils.py#L323
         #Keys are always strings in JSON so convert ids to int here.       
         super().__init__(**kwargs) 
 
 #오토 설정에 등록
 model_path = 'cnn'
-AutoConfig.register(model_path, CNNConfig)
+AutoConfig.register(model_path, CnnConfig)
```

### Comparing `transformers-supporter-0.0.7/transformers_supporter/models/cnn/image_processing_cnn.py` & `transformers-supporter-0.0.8/transformers_supporter/models/cnn/image_processing_cnn.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.7/transformers_supporter/models/cnn/modeling_cnn.py` & `transformers-supporter-0.0.8/transformers_supporter/models/cnn/modeling_cnn.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from transformers import AutoTokenizer
 from transformers import AutoConfig
 from transformers import AutoModelForImageClassification
 import torch
 from torch.nn import functional as F
 import pytorch_helper
 import transformers
-from .configuration_cnn import CNNConfig
+from .configuration_cnn import CnnConfig
     
-class CNNForImageClassification(PreTrainedModel):
-    config_class = CNNConfig
+class CnnForImageClassification(PreTrainedModel):
+    config_class = CnnConfig
 
     def __init__(self, config):
         super().__init__(config)
         self.layer = torch.nn.Sequential(
             torch.nn.Conv2d(in_channels=config.in_channels, out_channels=32, kernel_size=5, stride=1, padding=0),
             torch.nn.BatchNorm2d(num_features=32),
             torch.nn.ReLU(),
@@ -36,27 +36,27 @@
             return transformers.file_utils.ModelOutput({'logits': logits})
         else:
             #print(labels.shape) #
             loss = F.nll_loss(F.log_softmax(logits), labels) #원핫 벡터를 넣을 필요없이 바로 실제값을 인자로 사용 #nll은 Negative Log Likelihood의 약자
             return transformers.file_utils.ModelOutput({'loss': loss, 'logits': logits})
 
 #오토 모델에 등록
-AutoModelForImageClassification.register(CNNConfig, CNNForImageClassification)
+AutoModelForImageClassification.register(CnnConfig, CnnForImageClassification)
 
 ####################
 
 from transformers import PreTrainedModel
 import torch
 from torch.nn import functional as F
 import pytorch_helper
 import transformers
-from .configuration_cnn import CNNConfig
+from .configuration_cnn import CnnConfig
 
-class CNNForKeyPointDetection(PreTrainedModel):
-    config_class = CNNConfig
+class CnnForKeyPointDetection(PreTrainedModel):
+    config_class = CnnConfig
 
     def __init__(self, config):
         super().__init__(config)
         self.layer = torch.nn.Sequential(
             torch.nn.Conv2d(in_channels=3, out_channels=32, kernel_size=5, stride=1, padding=0),
             torch.nn.BatchNorm2d(num_features=32),
             torch.nn.ReLU(),
@@ -80,11 +80,11 @@
             #print(labels.shape) #
             #loss = torch.nn.MSELoss()(logits, labels) 
             loss = F.mse_loss(logits, labels) 
             return transformers.file_utils.ModelOutput({'loss': loss, 'logits': logits})
 
 '''
 #오토 모델에 등록
-AutoModelForKeyPointDetection.register(CNNConfig, CNNForKeyPointDetection)
+AutoModelForKeyPointDetection.register(CnnConfig, CnnForKeyPointDetection)
 '''
 
 ####################
```

### Comparing `transformers-supporter-0.0.7/transformers_supporter/models/custom_bert/configuration_custom_bert.py` & `transformers-supporter-0.0.8/transformers_supporter/models/custom_bert/configuration_custom_bert.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.7/transformers_supporter/models/custom_bert/modeling_custom_bert.py` & `transformers-supporter-0.0.8/transformers_supporter/models/custom_bert/modeling_custom_bert.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.7/transformers_supporter/models/custom_wav2vec2/feature_extraction_custom_wav2vec2.py` & `transformers-supporter-0.0.8/transformers_supporter/models/custom_wav2vec2/feature_extraction_custom_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.7/transformers_supporter/models/embedded_1dcnn/configuration_embedded_1dcnn.py` & `transformers-supporter-0.0.8/transformers_supporter/models/embedded_1dcnn/configuration_embedded_1dcnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from transformers import AutoConfig
 from transformers import AutoModelForSequenceClassification
 import torch
 from torch.nn import functional as F
 import pytorch_helper
 import transformers
 
-class Embedded1DCNNConfig(PretrainedConfig):
+class Embedded1dcnnConfig(PretrainedConfig):
     model_type = "embedded-1dcnn"
 
     def __init__(self, **kwargs):
         #https://github.com/huggingface/transformers/blob/98d88b23f54e5a23e741833f1e973fdf600cc2c5/src/transformers/configuration_utils.py#L323
         #Keys are always strings in JSON so convert ids to int here.       
         super().__init__(**kwargs)   
 
 #오토 설정에 등록
 model_path = 'embedded-1dcnn'
-AutoConfig.register(model_path, Embedded1DCNNConfig)
+AutoConfig.register(model_path, Embedded1dcnnConfig)
```

### Comparing `transformers-supporter-0.0.7/transformers_supporter/models/embedded_1dcnn/modeling_embedded_1dcnn.py` & `transformers-supporter-0.0.8/transformers_supporter/models/embedded_1dcnn/modeling_embedded_1dcnn.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from transformers import AutoTokenizer
 from transformers import AutoConfig
 from transformers import AutoModelForSequenceClassification
 import torch
 from torch.nn import functional as F
 import pytorch_helper
 import transformers
-from .configuration_embedded_1dcnn import Embedded1DCNNConfig
+from .configuration_embedded_1dcnn import Embedded1dcnnConfig
 
-class Embedded1DCNNForSequenceClassification(PreTrainedModel):
-    config_class = Embedded1DCNNConfig
+class Embedded1dcnnForSequenceClassification(PreTrainedModel):
+    config_class = Embedded1dcnnConfig
 
     def __init__(self, config):
         super().__init__(config)
         self.layer = torch.nn.Sequential(
             torch.nn.Embedding(num_embeddings=config.vocab_size, embedding_dim=32), #
             #https://chriskhanhtran.github.io/posts/cnn-sentence-classification/
             #Permute `x_embed` to match input shape requirement of `nn.Conv1d`.
@@ -39,8 +39,8 @@
         if labels == None:
             return transformers.file_utils.ModelOutput({'logits': logits})
         else:
             loss = F.nll_loss(F.log_softmax(logits), labels) #원핫 벡터를 넣을 필요없이 바로 실제값을 인자로 사용 #nll은 Negative Log Likelihood의 약자
             return transformers.file_utils.ModelOutput({'loss': loss, 'logits': logits})
 
 #오토 모델에 등록
-AutoModelForSequenceClassification.register(Embedded1DCNNConfig, Embedded1DCNNForSequenceClassification)
+AutoModelForSequenceClassification.register(Embedded1dcnnConfig, Embedded1dcnnForSequenceClassification)
```

### Comparing `transformers-supporter-0.0.7/transformers_supporter/models/embedded_rnn/configuration_embedded_rnn.py` & `transformers-supporter-0.0.8/transformers_supporter/models/embedded_rnn/configuration_embedded_rnn.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 from transformers import AutoConfig
 from transformers import AutoModelForSequenceClassification
 import torch
 from torch.nn import functional as F
 import pytorch_helper
 import transformers
 
-class EmbeddedRNNConfig(PretrainedConfig):
+class EmbeddedRnnConfig(PretrainedConfig):
     model_type = "embedded-rnn"
 
     def __init__(self, **kwargs):
         #https://github.com/huggingface/transformers/blob/98d88b23f54e5a23e741833f1e973fdf600cc2c5/src/transformers/configuration_utils.py#L323
         #Keys are always strings in JSON so convert ids to int here.       
         super().__init__(**kwargs)
 
 #오토 설정에 등록
 model_path = 'embedded-rnn'
-AutoConfig.register(model_path, EmbeddedRNNConfig)
+AutoConfig.register(model_path, EmbeddedRnnConfig)
 
-class PretrainedEmbeddedRNNConfig(PretrainedConfig):
+class PretrainedEmbeddedRnnConfig(PretrainedConfig):
     model_type = "pretrained-embedded-rnn"
 
     def __init__(self, **kwargs):
         #https://github.com/huggingface/transformers/blob/98d88b23f54e5a23e741833f1e973fdf600cc2c5/src/transformers/configuration_utils.py#L323
         #Keys are always strings in JSON so convert ids to int here.       
         super().__init__(**kwargs)
 
 #오토 설정에 등록
 model_path = 'pretrained-embedded-rnn'
-AutoConfig.register(model_path, PretrainedEmbeddedRNNConfig)
+AutoConfig.register(model_path, PretrainedEmbeddedRnnConfig)
```

### Comparing `transformers-supporter-0.0.7/transformers_supporter/models/embedded_rnn/modeling_embedded_rnn.py` & `transformers-supporter-0.0.8/transformers_supporter/models/embedded_rnn/modeling_embedded_rnn.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from transformers import AutoTokenizer
 from transformers import AutoConfig
 from transformers import AutoModelForSequenceClassification
 import torch
 from torch.nn import functional as F
 import pytorch_helper
 import transformers
-from .configuration_embedded_rnn import EmbeddedRNNConfig
+from .configuration_embedded_rnn import EmbeddedRnnConfig
 
-class EmbeddedRNNForSequenceClassification(PreTrainedModel):
-    config_class = EmbeddedRNNConfig
+class EmbeddedRnnForSequenceClassification(PreTrainedModel):
+    config_class = EmbeddedRnnConfig
 
     def __init__(self, config):
         super().__init__(config)        
         self.layer = torch.nn.Sequential(
             torch.nn.Embedding(num_embeddings=config.vocab_size, embedding_dim=32),
             pytorch_helper.layers.HiddenStateResetLSTM(input_size=32, hidden_size=32, batch_first=True),
             pytorch_helper.layers.LSTMLastHiddenState(),
@@ -28,30 +28,31 @@
         if labels == None:
             return transformers.file_utils.ModelOutput({'logits': logits})
         else:
             loss = F.nll_loss(F.log_softmax(logits), labels) #원핫 벡터를 넣을 필요없이 바로 실제값을 인자로 사용 #nll은 Negative Log Likelihood의 약자
             return transformers.file_utils.ModelOutput({'loss': loss, 'logits': logits})
 
 #오토 모델에 등록
-AutoModelForSequenceClassification.register(EmbeddedRNNConfig, EmbeddedRNNForSequenceClassification)
+AutoModelForSequenceClassification.register(EmbeddedRnnConfig, EmbeddedRnnForSequenceClassification)
 
 ####################
 
 from transformers import PretrainedConfig
 from transformers import PreTrainedModel
 from transformers import AutoModel
 from transformers import AutoTokenizer
 from transformers import AutoConfig
 import torch
 from torch.nn import functional as F
 import pytorch_helper
 import transformers
+from .configuration_embedded_rnn import EmbeddedRnnConfig
 
-class EmbeddedRNNForFixedLengthTranslation(PreTrainedModel):
-    config_class = EmbeddedRNNConfig
+class EmbeddedRnnForFixedLengthTranslation(PreTrainedModel):
+    config_class = EmbeddedRnnConfig
 
     def __init__(self, config):
         super().__init__(config)        
         self.layer = torch.nn.Sequential(
             torch.nn.Embedding(num_embeddings=config.vocab_size, embedding_dim=32),
             pytorch_helper.layers.HiddenStateResetLSTM(input_size=32, hidden_size=32, batch_first=True),
             pytorch_helper.layers.SelectFromArray(index=0), #lstm output, 모든 타임 스텝(토큰: 숫자, 문자, 단어)의 숨은 상태, torch.Size([8, 380, 32]) 
@@ -70,33 +71,33 @@
             #print(logits_.shape) #torch.Size([6, 7])
             #print(labels_.shape) #torch.Size([6])
             loss = F.nll_loss(F.log_softmax(logits_), labels_) #원핫 벡터를 넣을 필요없이 바로 실제값을 인자로 사용 #nll은 Negative Log Likelihood의 약자
             return transformers.file_utils.ModelOutput({'loss': loss, 'logits': logits})
 
 '''
 #오토 모델에 등록
-AutoModelForFixedLengthTranslation.register(EmbeddedRNNConfig, EmbeddedRNNForFixedLengthTranslation)
+AutoModelForFixedLengthTranslation.register(EmbeddedRnnConfig, EmbeddedRnnForFixedLengthTranslation)
 '''
 
 ####################
 
 from transformers import PretrainedConfig
 from transformers import PreTrainedModel
 from transformers import AutoModel
 from transformers import AutoTokenizer
 from transformers import AutoConfig
 from transformers import AutoModelForSequenceClassification
-from .configuration_embedded_rnn import PretrainedEmbeddedRNNConfig
+from .configuration_embedded_rnn import PretrainedEmbeddedRnnConfig
 import torch
 from torch.nn import functional as F
 from torchtext.vocab import build_vocab_from_iterator, Vectors
 import transformers
 
-class PretrainedEmbeddedRNNForSequenceClassification(PreTrainedModel):
-    config_class = PretrainedEmbeddedRNNConfig
+class PretrainedEmbeddedRnnForSequenceClassification(PreTrainedModel):
+    config_class = PretrainedEmbeddedRnnConfig
 
     def __init__(self, config):
         super().__init__(config)  
         self.layer = torch.nn.Sequential(
             self.load_pretrained_embedding(num_embeddings=config.vocab_size, embedding_dim=300, id_to_token=config.id_to_token),
             pytorch_helper.layers.HiddenStateResetLSTM(input_size=300, hidden_size=32, batch_first=True),
             pytorch_helper.layers.LSTMLastHiddenState(),
@@ -127,10 +128,10 @@
         if labels == None:
             return transformers.file_utils.ModelOutput({'logits': logits})
         else:
             loss = F.nll_loss(F.log_softmax(logits), labels) #원핫 벡터를 넣을 필요없이 바로 실제값을 인자로 사용 #nll은 Negative Log Likelihood의 약자
             return transformers.file_utils.ModelOutput({'loss': loss, 'logits': logits})
 
 #오토 모델에 등록
-AutoModelForSequenceClassification.register(PretrainedEmbeddedRNNConfig, PretrainedEmbeddedRNNForSequenceClassification)
+AutoModelForSequenceClassification.register(PretrainedEmbeddedRnnConfig, PretrainedEmbeddedRnnForSequenceClassification)
 
 ####################
```

### Comparing `transformers-supporter-0.0.7/transformers_supporter/models/embedded_rnn/tokenization_embedded_rnn.py` & `transformers-supporter-0.0.8/transformers_supporter/models/embedded_rnn/tokenization_embedded_rnn.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.7/transformers_supporter/models/faster_rcnn/configuration_faster_rcnn.py` & `transformers-supporter-0.0.8/transformers_supporter/models/faster_rcnn/configuration_faster_rcnn.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from transformers import PretrainedConfig
 
-class FasterRCNNConfig(PretrainedConfig):
+class FasterRcnnConfig(PretrainedConfig):
     model_type = "faster-rcnn"
 
     def __init__(self, **kwargs):
         #https://github.com/huggingface/transformers/blob/98d88b23f54e5a23e741833f1e973fdf600cc2c5/src/transformers/configuration_utils.py#L323
         #Keys are always strings in JSON so convert ids to int here.       
         super().__init__(**kwargs)   
 
 #오토 설정에 등록
 model_path = 'faster-rcnn'
-AutoConfig.register(model_path, FasterRCNNConfig)
+AutoConfig.register(model_path, FasterRcnnConfig)
```

### Comparing `transformers-supporter-0.0.7/transformers_supporter/models/faster_rcnn/image_processing_faster_rcnn.py` & `transformers-supporter-0.0.8/transformers_supporter/models/faster_rcnn/image_processing_faster_rcnn.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import torch
 from transformers.image_utils import is_batched
 from transformers import BatchFeature
 from transformers import AutoImageProcessor
 from torchvision import transforms
 from torch.nn import functional as F
 
-class FasterRCNNImageProcessor(ImageProcessingMixin):
+class FasterRcnnImageProcessor(ImageProcessingMixin):
     def __init__(self, image_mean=[0.5, 0.5, 0.5], image_std=[0.5, 0.5, 0.5], **kwargs):
         super().__init__(**kwargs)
         self.image_mean = image_mean
         self.image_std = image_std
 
     def __call__(self, images, annotations=None, return_tensors=None, **kwargs):
         return_tensors = None #return_tensors 미지원
@@ -72,8 +72,8 @@
             boxes_ = boxes[scores > threshold]
             labels_ = labels[scores > threshold]
             scores_ = scores[scores > threshold]
             results.append({"scores": scores_, "labels": labels_, "boxes": boxes_})
         return results
 
 #오토 이미지 프로세서에 등록
-AutoImageProcessor.register(FasterRCNNImageProcessor, FasterRCNNImageProcessor)
+AutoImageProcessor.register(FasterRcnnImageProcessor, FasterRcnnImageProcessor)
```

### Comparing `transformers-supporter-0.0.7/transformers_supporter/models/faster_rcnn/modeling_faster_rcnn.py` & `transformers-supporter-0.0.8/transformers_supporter/models/faster_rcnn/modeling_faster_rcnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 import torchvision
 from torchvision.models.detection.faster_rcnn import FastRCNNPredictor
 from torchvision.models.detection.faster_rcnn import FasterRCNN_ResNet50_FPN_Weights
 from torchvision.models.detection import FasterRCNN
 from torchvision.models.detection.rpn import AnchorGenerator
 from torchvision.models.detection._utils import Matcher
 from torchvision.ops.boxes import box_iou
-from .configuration_faster_rcnn import FasterRCNNConfig
+from .configuration_faster_rcnn import FasterRcnnConfig
 
-class FasterRCNNForObjectDetection(PreTrainedModel):
-    config_class = FasterRCNNConfig
+class FasterRcnnForObjectDetection(PreTrainedModel):
+    config_class = FasterRcnnConfig
 
     def __init__(self, config):
         super().__init__(config)
         # load a model; pre-trained on COCO
         weights = FasterRCNN_ResNet50_FPN_Weights.COCO_V1 
         self.model = torchvision.models.detection.fasterrcnn_resnet50_fpn(weights=weights)
         # get number of input features for the classifier
@@ -69,9 +69,9 @@
                 for output in outputs:
                     boxes.append(output['boxes'])
                     labels.append(output['labels'])
                     scores.append(output['scores'])
                 return transformers.file_utils.ModelOutput({'loss': loss, 'boxes': boxes, 'labels': labels, 'scores': scores})
 
 #오토 모델에 등록
-AutoModelForObjectDetection.register(FasterRCNNConfig, FasterRCNNForObjectDetection)
+AutoModelForObjectDetection.register(FasterRcnnConfig, FasterRcnnForObjectDetection)
```

### Comparing `transformers-supporter-0.0.7/transformers_supporter/models/rnn/modeling_rnn.py` & `transformers-supporter-0.0.8/transformers_supporter/models/rnn/modeling_rnn.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from transformers import AutoTokenizer
 from transformers import AutoConfig
 from transformers import AutoModelForAudioClassification
 import pytorch_helper
 import torch
 from torch.nn import functional as F
 import transformers
-from .configuration_rnn import RNNConfig
+from .configuration_rnn import RnnConfig
 
-class RNNForAudioClassification(PreTrainedModel):
-    config_class = RNNConfig
+class RnnForAudioClassification(PreTrainedModel):
+    config_class = RnnConfig
 
     def __init__(self, config):
         super().__init__(config)        
         self.layer = torch.nn.Sequential(
             pytorch_helper.layers.HiddenStateResetLSTM(input_size=1, hidden_size=32, batch_first=True),
             pytorch_helper.layers.LSTMLastHiddenState(),
             torch.nn.Linear(in_features=32, out_features=config.num_labels)
@@ -31,32 +31,33 @@
             return transformers.file_utils.ModelOutput({'logits': logits})
         else:
             loss = F.nll_loss(F.log_softmax(logits), labels) #원핫 벡터를 넣을 필요없이 바로 실제값을 인자로 사용 #nll은 Negative Log Likelihood의 약자
             return transformers.file_utils.ModelOutput({'loss': loss, 'logits': logits})
 
 #모델을 오토 모델에 등록
 model_path = 'rnn-config'
-AutoConfig.register(model_path, RNNConfig)
-AutoModelForAudioClassification.register(RNNConfig, RNNForAudioClassification)
+AutoConfig.register(model_path, RnnConfig)
+AutoModelForAudioClassification.register(RnnConfig, RnnForAudioClassification)
 
 ####################
 
 from transformers import PretrainedConfig
 from transformers import PreTrainedModel
 from transformers import AutoModel
 from transformers import AutoTokenizer
 from transformers import AutoConfig
 from transformers import AutoModelForAudioClassification
 import pytorch_helper
 import torch
 from torch.nn import functional as F
 import transformers
+from .configuration_rnn import RnnConfig
 
-class RNNForTimeSeriesRegression(PreTrainedModel):
-    config_class = RNNConfig
+class RnnForTimeSeriesRegression(PreTrainedModel):
+    config_class = RnnConfig
 
     def __init__(self, config):
         super().__init__(config)        
         self.layer = torch.nn.Sequential(
             pytorch_helper.layers.HiddenStateResetLSTM(input_size=1, hidden_size=32, batch_first=True),
             pytorch_helper.layers.LSTMLastHiddenState(),
             torch.nn.Linear(in_features=32, out_features=32),
@@ -78,10 +79,10 @@
             #loss = torch.nn.MSELoss()(logits, labels) 
             loss = F.mse_loss(logits, labels) 
             return transformers.file_utils.ModelOutput({'loss': loss, 'logits': logits})
         
 '''
 #모델을 오토 모델에 등록
 model_path = 'rnn-config'
-AutoConfig.register(model_path, RNNConfig)
-AutoModelForTimeSeriesRegression.register(RNNConfig, RNNForTimeSeriesRegression)
+AutoConfig.register(model_path, RnnConfig)
+AutoModelForTimeSeriesRegression.register(RnnConfig, RnnForTimeSeriesRegression)
 '''
```

### Comparing `transformers-supporter-0.0.7/transformers_supporter/pipelines/__init__.py` & `transformers-supporter-0.0.8/transformers_supporter/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.7/transformers_supporter/pipelines/custom_image_classification_pipeline.py` & `transformers-supporter-0.0.8/transformers_supporter/pipelines/custom_image_classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.7/transformers_supporter/pipelines/fixed_length_translation_pipeline.py` & `transformers-supporter-0.0.8/transformers_supporter/pipelines/fixed_length_translation_pipeline.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.7/transformers_supporter/pipelines/tabular_binary_classification_pipeline.py` & `transformers-supporter-0.0.8/transformers_supporter/pipelines/tabular_binary_classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.7/transformers_supporter/pipelines/tabular_classification_pipeline.py` & `transformers-supporter-0.0.8/transformers_supporter/pipelines/tabular_classification_pipeline.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.7/transformers_supporter/pipelines/tabular_regression_pipeline.py` & `transformers-supporter-0.0.8/transformers_supporter/pipelines/tabular_regression_pipeline.py`

 * *Files identical despite different names*

### Comparing `transformers-supporter-0.0.7/transformers_supporter.egg-info/SOURCES.txt` & `transformers-supporter-0.0.8/transformers_supporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

