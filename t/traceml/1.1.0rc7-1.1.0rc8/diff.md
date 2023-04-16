# Comparing `tmp/traceml-1.1.0rc7.tar.gz` & `tmp/traceml-1.1.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traceml-1.1.0rc7.tar", last modified: Wed Apr 12 14:22:02 2023, max compression
+gzip compressed data, was "traceml-1.1.0rc8.tar", last modified: Sun Apr 16 12:03:59 2023, max compression
```

## Comparing `traceml-1.1.0rc7.tar` & `traceml-1.1.0rc8.tar`

### file list

```diff
@@ -1,96 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:02.311652 traceml-1.1.0rc7/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-12 14:22:02.311652 traceml-1.1.0rc7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-12 14:22:02.311652 traceml-1.1.0rc7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:02.303652 traceml-1.1.0rc7/traceml/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:02.303652 traceml-1.1.0rc7/traceml/artifacts/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/artifacts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/artifacts/kinds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/artifacts/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:02.303652 traceml-1.1.0rc7/traceml/events/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/events/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    15500 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/events/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:02.303652 traceml-1.1.0rc7/traceml/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/integrations/fastai.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/integrations/fastai_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/integrations/hugging_face.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/integrations/ignite.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/integrations/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/integrations/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/integrations/pytorch_lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/integrations/scikit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/integrations/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/integrations/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/integrations/xgboost.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:02.307652 traceml-1.1.0rc7/traceml/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/logging/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/logging/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/logging/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/logging/streamer.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/pkg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:02.307652 traceml-1.1.0rc7/traceml/processors/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/processors/df_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/processors/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:02.307652 traceml-1.1.0rc7/traceml/processors/events_processors/
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/processors/events_processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/processors/events_processors/events_artifacts_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/processors/events_processors/events_audio_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/processors/events_processors/events_charts_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10191 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/processors/events_processors/events_image_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/processors/events_processors/events_metrics_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/processors/events_processors/events_models_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/processors/events_processors/events_tables_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/processors/events_processors/events_video_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/processors/gpu_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/processors/importance_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/processors/logs_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/processors/psutil_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/processors/units_processors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:02.307652 traceml-1.1.0rc7/traceml/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/serialization/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9750 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/serialization/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:02.307652 traceml-1.1.0rc7/traceml/summary/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/summary/df.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:02.307652 traceml-1.1.0rc7/traceml/tracking/
--rw-r--r--   0 runner    (1001) docker     (123)    28282 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61817 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/tracking/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:02.307652 traceml-1.1.0rc7/traceml/vendor/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:02.307652 traceml-1.1.0rc7/traceml/vendor/matplotlylib/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/vendor/matplotlylib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:02.307652 traceml-1.1.0rc7/traceml/vendor/matplotlylib/mplexporter/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/vendor/matplotlylib/mplexporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/vendor/matplotlylib/mplexporter/_py3k_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/vendor/matplotlylib/mplexporter/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:02.311652 traceml-1.1.0rc7/traceml/vendor/matplotlylib/mplexporter/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/vendor/matplotlylib/mplexporter/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14838 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/vendor/matplotlylib/mplexporter/renderers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/vendor/matplotlylib/mplexporter/renderers/fake_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/vendor/matplotlylib/mplexporter/renderers/vega_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/vendor/matplotlylib/mplexporter/renderers/vincent_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/vendor/matplotlylib/mplexporter/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/vendor/matplotlylib/mplexporter/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/vendor/matplotlylib/mpltools.py
--rw-r--r--   0 runner    (1001) docker     (123)    35762 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/vendor/matplotlylib/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/vendor/matplotlylib/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)   166500 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/vendor/pynvml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:02.311652 traceml-1.1.0rc7/traceml/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-04-12 14:21:52.000000 traceml-1.1.0rc7/traceml/visualization/run_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 14:22:02.303652 traceml-1.1.0rc7/traceml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-12 14:22:02.000000 traceml-1.1.0rc7/traceml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-12 14:22:02.000000 traceml-1.1.0rc7/traceml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 14:22:02.000000 traceml-1.1.0rc7/traceml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-12 14:22:02.000000 traceml-1.1.0rc7/traceml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-12 14:22:02.000000 traceml-1.1.0rc7/traceml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.105862 traceml-1.1.0rc8/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-16 12:03:59.105862 traceml-1.1.0rc8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-16 12:03:59.109862 traceml-1.1.0rc8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.101862 traceml-1.1.0rc8/traceml/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.101862 traceml-1.1.0rc8/traceml/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/artifacts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/artifacts/kinds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/artifacts/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.101862 traceml-1.1.0rc8/traceml/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/events/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15508 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/events/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.101862 traceml-1.1.0rc8/traceml/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/integrations/fastai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/integrations/fastai_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/integrations/hugging_face.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/integrations/ignite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/integrations/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/integrations/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/integrations/pytorch_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/integrations/scikit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/integrations/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/integrations/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/integrations/xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.101862 traceml-1.1.0rc8/traceml/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/logging/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/logging/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/logging/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/logging/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/pkg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.101862 traceml-1.1.0rc8/traceml/processors/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/processors/df_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/processors/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.105862 traceml-1.1.0rc8/traceml/processors/events_processors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/processors/events_processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/processors/events_processors/events_artifacts_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/processors/events_processors/events_audio_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/processors/events_processors/events_charts_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/processors/events_processors/events_image_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/processors/events_processors/events_metrics_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/processors/events_processors/events_models_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/processors/events_processors/events_tables_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/processors/events_processors/events_video_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/processors/gpu_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/processors/importance_processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/processors/logs_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/processors/psutil_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.105862 traceml-1.1.0rc8/traceml/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4969 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/serialization/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9751 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/serialization/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.105862 traceml-1.1.0rc8/traceml/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5619 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/summary/df.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.105862 traceml-1.1.0rc8/traceml/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)    28282 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61830 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/tracking/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.105862 traceml-1.1.0rc8/traceml/vendor/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.105862 traceml-1.1.0rc8/traceml/vendor/matplotlylib/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/vendor/matplotlylib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.105862 traceml-1.1.0rc8/traceml/vendor/matplotlylib/mplexporter/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/vendor/matplotlylib/mplexporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/vendor/matplotlylib/mplexporter/_py3k_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11826 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/vendor/matplotlylib/mplexporter/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.105862 traceml-1.1.0rc8/traceml/vendor/matplotlylib/mplexporter/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/vendor/matplotlylib/mplexporter/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/vendor/matplotlylib/mplexporter/renderers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/vendor/matplotlylib/mplexporter/renderers/fake_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/vendor/matplotlylib/mplexporter/renderers/vega_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/vendor/matplotlylib/mplexporter/renderers/vincent_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/vendor/matplotlylib/mplexporter/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/vendor/matplotlylib/mplexporter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20688 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/vendor/matplotlylib/mpltools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35762 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/vendor/matplotlylib/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/vendor/matplotlylib/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)   166500 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/vendor/pynvml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.105862 traceml-1.1.0rc8/traceml/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-04-16 12:03:47.000000 traceml-1.1.0rc8/traceml/visualization/run_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:03:59.101862 traceml-1.1.0rc8/traceml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-16 12:03:59.000000 traceml-1.1.0rc8/traceml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-16 12:03:59.000000 traceml-1.1.0rc8/traceml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 12:03:59.000000 traceml-1.1.0rc8/traceml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-16 12:03:59.000000 traceml-1.1.0rc8/traceml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-16 12:03:59.000000 traceml-1.1.0rc8/traceml.egg-info/top_level.txt
```

### Comparing `traceml-1.1.0rc7/PKG-INFO` & `traceml-1.1.0rc8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceml
-Version: 1.1.0rc7
+Version: 1.1.0rc8
 Summary: Engine for ML/Data tracking, visualization, dashboards, and model UI for Polyaxon.
 Home-page: https://github.com/polyaxon/traceml
 Author: Polyaxon, Inc.
 Author-email: contact@polyaxon.com
 Maintainer: Polyaxon, Inc.
 Maintainer-email: contact@polyaxon.com
 License: Apache 2.0
```

### Comparing `traceml-1.1.0rc7/setup.cfg` & `traceml-1.1.0rc8/setup.cfg`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/setup.py` & `traceml-1.1.0rc8/setup.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/__init__.py` & `traceml-1.1.0rc8/traceml/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/artifacts/__init__.py` & `traceml-1.1.0rc8/traceml/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/artifacts/kinds.py` & `traceml-1.1.0rc8/traceml/artifacts/kinds.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional, Union
 
-from clipped.enums_utils import PEnum
+from clipped.utils.enums import PEnum
 
 
 class V1ArtifactKind(str, PEnum):
     MODEL = "model"
     AUDIO = "audio"
     VIDEO = "video"
     HISTOGRAM = "histogram"
```

### Comparing `traceml-1.1.0rc7/traceml/artifacts/schemas.py` & `traceml-1.1.0rc8/traceml/artifacts/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import uuid
 
 from typing import Dict, List, Optional
 
+from clipped.types.uuids import UUIDStr
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
-from polyaxon.schemas.fields import UUIDStr
 from traceml.artifacts.kinds import V1ArtifactKind
 
 
 class V1RunArtifact(BaseSchemaModel):
     _IDENTIFIER = "artifact"
 
     name: Optional[StrictStr]
```

### Comparing `traceml-1.1.0rc7/traceml/events/__init__.py` & `traceml-1.1.0rc8/traceml/events/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/events/paths.py` & `traceml-1.1.0rc8/traceml/events/paths.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from enum import Enum
 from typing import Optional
 
-from clipped.enums_utils import get_enum_value
+from clipped.utils.enums import get_enum_value
 
 
 def get_resource_path(
     run_path: str, kind: Optional[str] = None, name: Optional[str] = None
 ) -> str:
     _path = "{}/resources".format(run_path)
     if kind:
```

### Comparing `traceml-1.1.0rc7/traceml/events/schemas.py` & `traceml-1.1.0rc8/traceml/events/schemas.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 # limitations under the License.
 import datetime
 import json
 
 from collections import namedtuple
 from typing import Dict, List, Mapping, Optional, Union
 
-from clipped.csv_utils import validate_csv
-from clipped.date_utils import parse_datetime
-from clipped.enums_utils import PEnum
-from clipped.np_utils import sanitize_np_types
-from clipped.tz_utils import now
+from clipped.config.parser import Parser
+from clipped.config.schema import skip_partial
+from clipped.utils.csv import validate_csv
+from clipped.utils.dates import parse_datetime
+from clipped.utils.enums import PEnum
+from clipped.utils.np import sanitize_np_types
+from clipped.utils.tz import now
 from pydantic import StrictStr, root_validator
 
-from polyaxon.parser import parser
-from polyaxon.schemas.base import BaseSchemaModel, skip_partial
+from polyaxon.schemas.base import BaseSchemaModel
 from traceml.artifacts.kinds import V1ArtifactKind
 
 
 class SearchView(str, PEnum):
     ANY = "any"
     RUNS = "runs"
     SELECTION = "selection"
@@ -173,70 +174,71 @@
     model: Optional[V1EventModel]
     dataframe: Optional[V1EventDataframe]
 
     @root_validator(pre=True)
     @skip_partial
     def pre_validate(cls, values):
         v = values.get(V1ArtifactKind.IMAGE)
+        get_dict = Parser.parse(Dict)
         if v is not None and not isinstance(v, BaseSchemaModel):
-            values[V1ArtifactKind.IMAGE] = parser.get_dict(
+            values[V1ArtifactKind.IMAGE] = get_dict(
                 key=V1ArtifactKind.IMAGE,
                 value=v,
             )
         v = values.get(V1ArtifactKind.HISTOGRAM)
         if v is not None and not isinstance(v, BaseSchemaModel):
-            values[V1ArtifactKind.HISTOGRAM] = parser.get_dict(
+            values[V1ArtifactKind.HISTOGRAM] = get_dict(
                 key=V1ArtifactKind.HISTOGRAM,
                 value=v,
             )
         v = values.get(V1ArtifactKind.AUDIO)
         if v is not None and not isinstance(v, BaseSchemaModel):
-            values[V1ArtifactKind.AUDIO] = parser.get_dict(
+            values[V1ArtifactKind.AUDIO] = get_dict(
                 key=V1ArtifactKind.AUDIO,
                 value=v,
             )
         v = values.get(V1ArtifactKind.VIDEO)
         if v is not None and not isinstance(v, BaseSchemaModel):
-            values[V1ArtifactKind.VIDEO] = parser.get_dict(
+            values[V1ArtifactKind.VIDEO] = get_dict(
                 key=V1ArtifactKind.VIDEO,
                 value=v,
             )
         v = values.get(V1ArtifactKind.CHART)
         if v is not None and not isinstance(v, BaseSchemaModel):
-            values[V1ArtifactKind.CHART] = parser.get_dict(
+            values[V1ArtifactKind.CHART] = get_dict(
                 key=V1ArtifactKind.CHART,
                 value=v,
             )
         v = values.get(V1ArtifactKind.CURVE)
         if v is not None and not isinstance(v, BaseSchemaModel):
-            values[V1ArtifactKind.CURVE] = parser.get_dict(
+            values[V1ArtifactKind.CURVE] = get_dict(
                 key=V1ArtifactKind.CURVE,
                 value=v,
             )
         v = values.get(V1ArtifactKind.CONFUSION)
         if v is not None and not isinstance(v, BaseSchemaModel):
-            values[V1ArtifactKind.CONFUSION] = parser.get_dict(
+            values[V1ArtifactKind.CONFUSION] = get_dict(
                 key=V1ArtifactKind.CONFUSION,
                 value=v,
             )
         v = values.get(V1ArtifactKind.ARTIFACT)
         if v is not None and not isinstance(v, BaseSchemaModel):
-            values[V1ArtifactKind.ARTIFACT] = parser.get_dict(
+            values[V1ArtifactKind.ARTIFACT] = get_dict(
                 key=V1ArtifactKind.ARTIFACT,
                 value=v,
             )
         v = values.get(V1ArtifactKind.MODEL)
         if v is not None and not isinstance(v, BaseSchemaModel):
-            values[V1ArtifactKind.MODEL] = parser.get_dict(
+            values[V1ArtifactKind.MODEL] = get_dict(
                 key=V1ArtifactKind.MODEL,
                 value=v,
             )
         v = values.get(V1ArtifactKind.DATAFRAME)
         if v is not None and not isinstance(v, BaseSchemaModel):
-            values[V1ArtifactKind.DATAFRAME] = parser.get_dict(
+            values[V1ArtifactKind.DATAFRAME] = get_dict(
                 key=V1ArtifactKind.DATAFRAME,
                 value=v,
             )
 
         return values
 
     @root_validator
```

### Comparing `traceml-1.1.0rc7/traceml/exceptions.py` & `traceml-1.1.0rc8/traceml/exceptions.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/integrations/__init__.py` & `traceml-1.1.0rc8/traceml/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/integrations/fastai.py` & `traceml-1.1.0rc8/traceml/integrations/fastai.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/integrations/fastai_v1.py` & `traceml-1.1.0rc8/traceml/integrations/fastai_v1.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/integrations/hugging_face.py` & `traceml-1.1.0rc8/traceml/integrations/hugging_face.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/integrations/ignite.py` & `traceml-1.1.0rc8/traceml/integrations/ignite.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/integrations/keras.py` & `traceml-1.1.0rc8/traceml/integrations/keras.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import operator
 
 from typing import List, Optional
 
-from clipped.np_utils import sanitize_np_types
+from clipped.utils.np import sanitize_np_types
 
 from polyaxon.client.decorators import client_handler
 from traceml import tracking
 from traceml.exceptions import TracemlException
 from traceml.logger import logger
 
 try:
```

### Comparing `traceml-1.1.0rc7/traceml/integrations/lightgbm.py` & `traceml-1.1.0rc8/traceml/integrations/lightgbm.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/integrations/pytorch_lightning.py` & `traceml-1.1.0rc8/traceml/integrations/pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/integrations/scikit.py` & `traceml-1.1.0rc8/traceml/integrations/scikit.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from clipped.np_utils import sanitize_dict
+from clipped.utils.np import sanitize_dict
 
 from traceml import tracking
 from traceml.exceptions import TracemlException
 
 try:
     from sklearn.base import is_classifier, is_regressor
     from sklearn.metrics import (
```

### Comparing `traceml-1.1.0rc7/traceml/integrations/tensorboard.py` & `traceml-1.1.0rc8/traceml/integrations/tensorboard.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/integrations/tensorflow.py` & `traceml-1.1.0rc8/traceml/integrations/tensorflow.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/integrations/xgboost.py` & `traceml-1.1.0rc8/traceml/integrations/xgboost.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import TYPE_CHECKING, Optional
 
-import orjson
+from clipped.utils.json import orjson_loads
 
 from traceml import tracking
 from traceml.exceptions import TracemlException
 from traceml.logger import logger
 
 try:
     import xgboost as xgb
@@ -145,21 +145,21 @@
                 model_folds=model_folds,
                 max_num_features=self.max_num_features,
             )
 
         if model_folds:
             config = {}
             for i, fold in enumerate(model_folds):
-                config["fold_{}_config".format(i)] = orjson.loads(
+                config["fold_{}_config".format(i)] = orjson_loads(
                     fold.bst.save_config()
                 )
             if config:
                 self.run.log_inputs(**config)
         else:
-            self.run.log_inputs(config=orjson.loads(model.save_config()))
+            self.run.log_inputs(config=orjson_loads(model.save_config()))
             outputs = {}
             if "best_score" in model.attributes().keys():
                 outputs["best_score"] = model.attributes()["best_score"]
             if "best_iteration" in model.attributes().keys():
                 outputs["best_iteration"] = model.attributes()["best_iteration"]
             self.run.log_outputs(**outputs)
```

### Comparing `traceml-1.1.0rc7/traceml/logger.py` & `traceml-1.1.0rc8/traceml/logger.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/logging/__init__.py` & `traceml-1.1.0rc8/traceml/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/logging/handler.py` & `traceml-1.1.0rc8/traceml/logging/handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 import os
 import socket
 
-from clipped.date_utils import to_datetime
-from clipped.env import get_user
+from clipped.utils.dates import to_datetime
+from clipped.utils.env import get_user
 
 from polyaxon import settings
 from polyaxon.env_vars.keys import EV_KEYS_K8S_NODE_NAME, EV_KEYS_K8S_POD_ID
 from traceml.logging import V1Log
 
 
 class LogStreamHandler(logging.Handler):
```

### Comparing `traceml-1.1.0rc7/traceml/logging/parser.py` & `traceml-1.1.0rc8/traceml/logging/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import re
 
-from clipped.date_utils import parse_datetime
+from clipped.utils.dates import parse_datetime
 
 # pylint:disable=anomalous-backslash-in-string
 
 DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S %Z"  # noqa
 ISO_DATETIME_REGEX = re.compile(  # noqa
     r"([0-9]+)-(0[1-9]|1[012])-(0[1-9]|[12][0-9]|3[01])[Tt]"
     r"([01][0-9]|2[0-3]):([0-5][0-9]):([0-5][0-9]|60)(\.[0-9]+)?"
```

### Comparing `traceml-1.1.0rc7/traceml/logging/schemas.py` & `traceml-1.1.0rc8/traceml/logging/schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import datetime
 
 from typing import List, Optional, Text
 
-import orjson
-
-from clipped.csv_utils import validate_csv
-from clipped.date_utils import parse_datetime
-from clipped.json_utils import orjson_dumps
-from clipped.tz_utils import now
+from clipped.utils.csv import validate_csv
+from clipped.utils.dates import parse_datetime
+from clipped.utils.json import orjson_dumps, orjson_loads
+from clipped.utils.tz import now
 from pydantic import StrictStr
 
 from polyaxon.schemas.base import BaseSchemaModel
 from traceml.logging.parser import (
     DATETIME_REGEX,
     ISO_DATETIME_REGEX,
     timestamp_search_regex,
@@ -139,12 +137,12 @@
         return cls.construct(
             logs=[
                 V1Log.construct(
                     timestamp=i.get("timestamp"),
                     node=i.get("node"),
                     pod=i.get("pod"),
                     container=i.get("container"),
-                    value=orjson.loads(i.get("value")).get("_"),
+                    value=orjson_loads(i.get("value")).get("_"),
                 )
                 for i in df.replace({np.nan: None}).to_dict(orient="records")
             ]
         )
```

### Comparing `traceml-1.1.0rc7/traceml/logging/streamer.py` & `traceml-1.1.0rc8/traceml/logging/streamer.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections import deque
 from typing import Callable
 
 from clipped.formatting import Printer
-from clipped.tz_utils import local_datetime
+from clipped.utils.tz import local_datetime
 
 from polyaxon import settings
 from polyaxon.containers.names import MAIN_JOB_CONTAINER
 from traceml.logging.schemas import V1Log, V1Logs
 
 
 def get_logs_streamer(
```

### Comparing `traceml-1.1.0rc7/traceml/pkg.py` & `traceml-1.1.0rc8/traceml/pkg.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 NAME = "traceml"
-VERSION = "1.1.0-rc7"
+VERSION = "1.1.0-rc8"
 DESC = (
     "Engine for ML/Data tracking, visualization, dashboards, and model UI for Polyaxon."
 )
 URL = "https://github.com/polyaxon/traceml"
 AUTHOR = "Polyaxon, Inc."
 EMAIL = "contact@polyaxon.com"
 LICENSE = "Apache 2.0"
```

### Comparing `traceml-1.1.0rc7/traceml/processors/__init__.py` & `traceml-1.1.0rc8/traceml/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/processors/df_processors.py` & `traceml-1.1.0rc8/traceml/processors/df_processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Dict, List, Optional, Tuple, Union
 
-from clipped.enums_utils import PEnum
+from clipped.utils.enums import PEnum
+from clipped.utils.units import to_percentage
 
 from traceml.processors.errors import NUMPY_ERROR_MESSAGE, PANDAS_ERROR_MESSAGE
-from traceml.processors.units_processors import to_percentage
 
 try:
     import numpy as np
 except ImportError as e:
     raise ImportError(NUMPY_ERROR_MESSAGE) from e
 
 try:
```

### Comparing `traceml-1.1.0rc7/traceml/processors/errors.py` & `traceml-1.1.0rc8/traceml/processors/errors.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/processors/events_processors/__init__.py` & `traceml-1.1.0rc8/traceml/processors/events_processors/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/processors/events_processors/events_artifacts_processors.py` & `traceml-1.1.0rc8/traceml/processors/events_processors/events_artifacts_processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional
 
-from clipped.path_utils import copy_file_or_dir_path
+from clipped.utils.paths import copy_file_or_dir_path
 
 from traceml.events import V1EventArtifact
 
 try:
     import numpy as np
 except ImportError:
     np = None
```

### Comparing `traceml-1.1.0rc7/traceml/processors/events_processors/events_audio_processors.py` & `traceml-1.1.0rc8/traceml/processors/events_processors/events_audio_processors.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional
 
-from clipped.np_utils import to_np
-from clipped.path_utils import check_or_create_path, copy_file_path
+from clipped.utils.np import to_np
+from clipped.utils.paths import check_or_create_path, copy_file_path
 
 from polyaxon.constants.globals import UNKNOWN
 from traceml.events import V1EventAudio
 from traceml.logger import logger
 from traceml.processors.errors import NUMPY_ERROR_MESSAGE
 
 try:
```

### Comparing `traceml-1.1.0rc7/traceml/processors/events_processors/events_charts_processors.py` & `traceml-1.1.0rc8/traceml/processors/events_processors/events_charts_processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from clipped.path_utils import module_type
+from clipped.utils.paths import module_type
 
 from polyaxon.constants.globals import UNKNOWN
 from traceml.events import V1EventChart, V1EventChartKind
 from traceml.logger import logger
 from traceml.processors.errors import (
     BOKEH_ERROR_MESSAGE,
     MATPLOTLIB_ERROR_MESSAGE,
```

### Comparing `traceml-1.1.0rc7/traceml/processors/events_processors/events_image_processors.py` & `traceml-1.1.0rc8/traceml/processors/events_processors/events_image_processors.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import io
 
 from typing import Optional
 
-from clipped.np_utils import calculate_scale_factor, to_np
-from clipped.path_utils import check_or_create_path, copy_file_path
+from clipped.utils.np import calculate_scale_factor, to_np
+from clipped.utils.paths import check_or_create_path, copy_file_path
 
 from polyaxon.constants.globals import UNKNOWN
 from traceml.events import V1EventImage
 from traceml.logger import logger
 from traceml.processors.errors import (
     MATPLOTLIB_ERROR_MESSAGE,
     NUMPY_ERROR_MESSAGE,
```

### Comparing `traceml-1.1.0rc7/traceml/processors/events_processors/events_metrics_processors.py` & `traceml-1.1.0rc8/traceml/processors/events_processors/events_metrics_processors.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Dict, List
 
-from clipped.np_utils import to_np
+from clipped.utils.np import to_np
 
 from polyaxon.constants.globals import UNKNOWN
 from traceml.artifacts import V1ArtifactKind
 from traceml.events import (
     LoggedEventSpec,
     V1Event,
     V1EventConfusionMatrix,
```

### Comparing `traceml-1.1.0rc7/traceml/processors/events_processors/events_models_processors.py` & `traceml-1.1.0rc8/traceml/processors/events_processors/events_models_processors.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Dict, Optional
 
-from clipped.path_utils import copy_file_or_dir_path
+from clipped.utils.paths import copy_file_or_dir_path
 
 from traceml.events import V1EventModel
 from traceml.logger import logger
 
 try:
     import numpy as np
 except ImportError:
```

### Comparing `traceml-1.1.0rc7/traceml/processors/events_processors/events_tables_processors.py` & `traceml-1.1.0rc8/traceml/processors/events_processors/events_tables_processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional
 
-from clipped.path_utils import copy_file_path
+from clipped.utils.paths import copy_file_path
 
 from traceml.events import V1EventDataframe
 
 try:
     import numpy as np
 except ImportError:
     np = None
```

### Comparing `traceml-1.1.0rc7/traceml/processors/events_processors/events_video_processors.py` & `traceml-1.1.0rc8/traceml/processors/events_processors/events_video_processors.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Optional
 
-from clipped.np_utils import calculate_scale_factor, to_np
-from clipped.path_utils import check_or_create_path, copy_file_path
+from clipped.utils.np import calculate_scale_factor, to_np
+from clipped.utils.paths import check_or_create_path, copy_file_path
 
 from polyaxon.constants.globals import UNKNOWN
 from traceml.events import V1EventVideo
 from traceml.logger import logger
 from traceml.processors.errors import MOVIEPY_ERROR_MESSAGE, NUMPY_ERROR_MESSAGE
 
 try:
```

### Comparing `traceml-1.1.0rc7/traceml/processors/gpu_processor.py` & `traceml-1.1.0rc8/traceml/processors/gpu_processor.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/processors/importance_processors.py` & `traceml-1.1.0rc8/traceml/processors/importance_processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # limitations under the License.
 import math
 import numpy as np
 import pandas as pd
 
 from typing import Dict, List, Optional, Tuple, Union
 
-from clipped.np_utils import sanitize_np_types
+from clipped.utils.np import sanitize_np_types
 
 
 def clean_duplicates(
     params: pd.DataFrame, metrics: pd.DataFrame
 ) -> Optional[Tuple[pd.DataFrame, pd.DataFrame]]:
     duplicate_ids = metrics.duplicated()
     params_df = params[~duplicate_ids]
```

### Comparing `traceml-1.1.0rc7/traceml/processors/logs_processor.py` & `traceml-1.1.0rc8/traceml/processors/logs_processor.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/processors/psutil_processor.py` & `traceml-1.1.0rc8/traceml/processors/psutil_processor.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/serialization/__init__.py` & `traceml-1.1.0rc8/traceml/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/serialization/base.py` & `traceml-1.1.0rc8/traceml/serialization/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 from typing import Dict, List
 
-from clipped.enums_utils import get_enum_value
-from clipped.path_utils import check_or_create_path
+from clipped.utils.enums import get_enum_value
+from clipped.utils.paths import check_or_create_path
 
 from traceml.events import LoggedEventSpec
 from traceml.events.schemas import LoggedEventListSpec
 
 
 class EventWriter:
     EVENTS_BACKEND = "events"
```

### Comparing `traceml-1.1.0rc7/traceml/serialization/writer.py` & `traceml-1.1.0rc8/traceml/serialization/writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import queue
 import threading
 import time
 
 from typing import List, Union
 
-from clipped.path_utils import check_or_create_path
+from clipped.utils.paths import check_or_create_path
 
 from traceml.events import LoggedEventSpec, get_asset_path, get_event_path
 from traceml.events.paths import get_resource_path
 from traceml.processors.gpu_processor import can_log_gpu_resources, get_gpu_metrics
 from traceml.processors.psutil_processor import (
     can_log_psutil_resources,
     get_psutils_metrics,
```

### Comparing `traceml-1.1.0rc7/traceml/summary/__init__.py` & `traceml-1.1.0rc8/traceml/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/summary/df.py` & `traceml-1.1.0rc8/traceml/summary/df.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/tracking/__init__.py` & `traceml-1.1.0rc8/traceml/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/tracking/run.py` & `traceml-1.1.0rc8/traceml/tracking/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 import sys
 import tempfile
 import time
 
 from datetime import datetime
 from typing import Dict, List, Optional
 
-from clipped.env import get_run_env
-from clipped.hashing import hash_value
-from clipped.json_utils import orjson_dumps
-from clipped.path_utils import (
+from clipped.utils.env import get_run_env
+from clipped.utils.hashing import hash_value
+from clipped.utils.json import orjson_dumps
+from clipped.utils.paths import (
     check_or_create_path,
     copy_file_or_dir_path,
     get_base_filename,
     get_path_extension,
 )
 
 from polyaxon import settings
```

### Comparing `traceml-1.1.0rc7/traceml/vendor/__init__.py` & `traceml-1.1.0rc8/traceml/vendor/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/vendor/matplotlylib/mplexporter/exporter.py` & `traceml-1.1.0rc8/traceml/vendor/matplotlylib/mplexporter/exporter.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/vendor/matplotlylib/mplexporter/renderers/base.py` & `traceml-1.1.0rc8/traceml/vendor/matplotlylib/mplexporter/renderers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import itertools
 from contextlib import contextmanager
 
 import numpy as np
 import matplotlib as mpl
 from matplotlib import transforms
 
-from clipped.versions import get_loose_version
+from clipped.utils.versions import get_loose_version
 
 from .. import utils
 from .. import _py3k_compat as py3k
 
 
 class Renderer(object):
     @staticmethod
```

### Comparing `traceml-1.1.0rc7/traceml/vendor/matplotlylib/mplexporter/renderers/fake_renderer.py` & `traceml-1.1.0rc8/traceml/vendor/matplotlylib/mplexporter/renderers/fake_renderer.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/vendor/matplotlylib/mplexporter/renderers/vega_renderer.py` & `traceml-1.1.0rc8/traceml/vendor/matplotlylib/mplexporter/renderers/vega_renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import warnings
-import json
 import random
+
+from clipped.utils.json import orjson_dumps
 from .base import Renderer
 from ..exporter import Exporter
 
 
 class VegaRenderer(Renderer):
     def open_figure(self, fig, props):
         self.props = props
@@ -102,15 +103,15 @@
         )
 
     def html(self):
         """Build the HTML representation for IPython."""
         id = random.randint(0, 2 ** 16)
         html = '<div id="vis%d"></div>' % id
         html += "<script>\n"
-        html += VEGA_TEMPLATE % (json.dumps(self.specification), id)
+        html += VEGA_TEMPLATE % (orjson_dumps(self.specification), id)
         html += "</script>\n"
         return html
 
     def _repr_html_(self):
         return self.html()
```

### Comparing `traceml-1.1.0rc7/traceml/vendor/matplotlylib/mplexporter/renderers/vincent_renderer.py` & `traceml-1.1.0rc8/traceml/vendor/matplotlylib/mplexporter/renderers/vincent_renderer.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/vendor/matplotlylib/mplexporter/tools.py` & `traceml-1.1.0rc8/traceml/vendor/matplotlylib/mplexporter/tools.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/vendor/matplotlylib/mplexporter/utils.py` & `traceml-1.1.0rc8/traceml/vendor/matplotlylib/mplexporter/utils.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/vendor/matplotlylib/mpltools.py` & `traceml-1.1.0rc8/traceml/vendor/matplotlylib/mpltools.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/vendor/matplotlylib/renderer.py` & `traceml-1.1.0rc8/traceml/vendor/matplotlylib/renderer.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/vendor/matplotlylib/tools.py` & `traceml-1.1.0rc8/traceml/vendor/matplotlylib/tools.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/vendor/pynvml.py` & `traceml-1.1.0rc8/traceml/vendor/pynvml.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/visualization/__init__.py` & `traceml-1.1.0rc8/traceml/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml/visualization/run_plot.py` & `traceml-1.1.0rc8/traceml/visualization/run_plot.py`

 * *Files identical despite different names*

### Comparing `traceml-1.1.0rc7/traceml.egg-info/PKG-INFO` & `traceml-1.1.0rc8/traceml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceml
-Version: 1.1.0rc7
+Version: 1.1.0rc8
 Summary: Engine for ML/Data tracking, visualization, dashboards, and model UI for Polyaxon.
 Home-page: https://github.com/polyaxon/traceml
 Author: Polyaxon, Inc.
 Author-email: contact@polyaxon.com
 Maintainer: Polyaxon, Inc.
 Maintainer-email: contact@polyaxon.com
 License: Apache 2.0
```

### Comparing `traceml-1.1.0rc7/traceml.egg-info/SOURCES.txt` & `traceml-1.1.0rc8/traceml.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 traceml/processors/__init__.py
 traceml/processors/df_processors.py
 traceml/processors/errors.py
 traceml/processors/gpu_processor.py
 traceml/processors/importance_processors.py
 traceml/processors/logs_processor.py
 traceml/processors/psutil_processor.py
-traceml/processors/units_processors.py
 traceml/processors/events_processors/__init__.py
 traceml/processors/events_processors/events_artifacts_processors.py
 traceml/processors/events_processors/events_audio_processors.py
 traceml/processors/events_processors/events_charts_processors.py
 traceml/processors/events_processors/events_image_processors.py
 traceml/processors/events_processors/events_metrics_processors.py
 traceml/processors/events_processors/events_models_processors.py
```

