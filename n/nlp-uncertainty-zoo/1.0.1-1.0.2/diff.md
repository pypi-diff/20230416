# Comparing `tmp/nlp-uncertainty-zoo-1.0.1.tar.gz` & `tmp/nlp-uncertainty-zoo-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp-uncertainty-zoo-1.0.1.tar", last modified: Mon Feb 27 14:51:31 2023, max compression
+gzip compressed data, was "dist/nlp-uncertainty-zoo-1.0.2.tar", last modified: Sun Apr 16 20:58:23 2023, max compression
```

## Comparing `nlp-uncertainty-zoo-1.0.1.tar` & `nlp-uncertainty-zoo-1.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-02-27 14:51:31.869234 nlp-uncertainty-zoo-1.0.1/
--rw-r--r--   0 deul       (502) staff       (20)     8808 2023-02-27 14:51:31.868698 nlp-uncertainty-zoo-1.0.1/PKG-INFO
--rw-r--r--   0 deul       (502) staff       (20)     8174 2023-02-27 11:21:57.000000 nlp-uncertainty-zoo-1.0.1/README.md
-drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-02-27 14:51:31.834800 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/
--rw-r--r--   0 deul       (502) staff       (20)     1164 2022-10-28 15:35:55.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/__init__.py
--rw-r--r--   0 deul       (502) staff       (20)     1660 2023-01-23 16:34:19.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/config.py
--rw-r--r--   0 deul       (502) staff       (20)    24659 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/defaults.py
-drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-02-27 14:51:31.856626 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/
--rw-r--r--   0 deul       (502) staff       (20)     1093 2022-07-06 16:02:58.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/__init__.py
--rw-r--r--   0 deul       (502) staff       (20)     8219 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/bayesian_lstm.py
--rw-r--r--   0 deul       (502) staff       (20)    11830 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/bert.py
--rw-r--r--   0 deul       (502) staff       (20)    21383 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/ddu_transformer.py
--rw-r--r--   0 deul       (502) staff       (20)    15262 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/dpp_transformer.py
--rw-r--r--   0 deul       (502) staff       (20)    14223 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/lstm.py
--rw-r--r--   0 deul       (502) staff       (20)    17167 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/lstm_ensemble.py
--rw-r--r--   0 deul       (502) staff       (20)    24054 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/model.py
--rw-r--r--   0 deul       (502) staff       (20)    30916 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/sngp_transformer.py
--rw-r--r--   0 deul       (502) staff       (20)    10731 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/spectral.py
--rw-r--r--   0 deul       (502) staff       (20)     9369 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/st_tau_lstm.py
--rw-r--r--   0 deul       (502) staff       (20)    10296 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/transformer.py
--rw-r--r--   0 deul       (502) staff       (20)    18963 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/variational_lstm.py
--rw-r--r--   0 deul       (502) staff       (20)    13935 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/variational_transformer.py
-drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-02-27 14:51:31.860239 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/tests/
--rw-r--r--   0 deul       (502) staff       (20)        0 2022-02-14 17:08:56.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/tests/__init__.py
--rw-r--r--   0 deul       (502) staff       (20)    12617 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/tests/test_module_functions.py
-drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-02-27 14:51:31.867581 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/utils/
--rw-r--r--   0 deul       (502) staff       (20)        0 2022-02-14 17:08:56.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/utils/__init__.py
--rw-r--r--   0 deul       (502) staff       (20)    12005 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/utils/calibration_eval.py
--rw-r--r--   0 deul       (502) staff       (20)      320 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/utils/custom_types.py
--rw-r--r--   0 deul       (502) staff       (20)    15253 2023-02-27 14:49:13.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/utils/data.py
--rw-r--r--   0 deul       (502) staff       (20)     3801 2022-05-25 13:35:12.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/utils/metrics.py
--rw-rw-rw-   0 deul       (502) staff       (20)    19782 2022-03-29 13:22:55.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/utils/samplers.py
--rw-r--r--   0 deul       (502) staff       (20)     2905 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/utils/task_eval.py
--rw-r--r--   0 deul       (502) staff       (20)    11899 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/utils/uncertainty_eval.py
-drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-02-27 14:51:31.842090 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo.egg-info/
--rw-r--r--   0 deul       (502) staff       (20)     8808 2023-02-27 14:51:31.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo.egg-info/PKG-INFO
--rw-r--r--   0 deul       (502) staff       (20)     1331 2023-02-27 14:51:31.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo.egg-info/SOURCES.txt
--rw-r--r--   0 deul       (502) staff       (20)        1 2023-02-27 14:51:31.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo.egg-info/dependency_links.txt
--rw-r--r--   0 deul       (502) staff       (20)      262 2023-02-27 14:51:31.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo.egg-info/requires.txt
--rw-r--r--   0 deul       (502) staff       (20)       20 2023-02-27 14:51:31.000000 nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo.egg-info/top_level.txt
--rw-r--r--   0 deul       (502) staff       (20)       38 2023-02-27 14:51:31.869367 nlp-uncertainty-zoo-1.0.1/setup.cfg
--rw-r--r--   0 deul       (502) staff       (20)     1141 2023-02-27 14:49:20.000000 nlp-uncertainty-zoo-1.0.1/setup.py
+drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/
+-rw-r--r--   0 deul       (502) staff       (20)     9743 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/PKG-INFO
+drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/
+-rw-r--r--   0 deul       (502) staff       (20)     1660 2023-01-23 16:34:19.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/config.py
+drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/tests/
+-rw-r--r--   0 deul       (502) staff       (20)    12617 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/tests/test_module_functions.py
+-rw-r--r--   0 deul       (502) staff       (20)        0 2022-02-14 17:08:56.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/tests/__init__.py
+-rw-r--r--   0 deul       (502) staff       (20)     1164 2022-10-28 15:35:55.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/__init__.py
+drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/
+-rw-r--r--   0 deul       (502) staff       (20)     3801 2022-05-25 13:35:12.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/metrics.py
+-rw-r--r--   0 deul       (502) staff       (20)     2905 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/task_eval.py
+-rw-r--r--   0 deul       (502) staff       (20)        0 2022-02-14 17:08:56.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/__init__.py
+-rw-r--r--   0 deul       (502) staff       (20)    12005 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/calibration_eval.py
+-rw-r--r--   0 deul       (502) staff       (20)      320 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/custom_types.py
+-rw-r--r--   0 deul       (502) staff       (20)    11899 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/uncertainty_eval.py
+-rw-rw-rw-   0 deul       (502) staff       (20)    19782 2022-03-29 13:22:55.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/samplers.py
+-rw-r--r--   0 deul       (502) staff       (20)    15253 2023-02-27 14:49:13.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/data.py
+drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/
+-rw-r--r--   0 deul       (502) staff       (20)    21413 2023-04-16 20:54:39.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/ddu_transformer.py
+-rw-r--r--   0 deul       (502) staff       (20)    15262 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/dpp_transformer.py
+-rw-r--r--   0 deul       (502) staff       (20)     9369 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/st_tau_lstm.py
+-rw-r--r--   0 deul       (502) staff       (20)    17167 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/lstm_ensemble.py
+-rw-r--r--   0 deul       (502) staff       (20)    13935 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/variational_transformer.py
+-rw-r--r--   0 deul       (502) staff       (20)     8219 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/bayesian_lstm.py
+-rw-r--r--   0 deul       (502) staff       (20)     1093 2022-07-06 16:02:58.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/__init__.py
+-rw-r--r--   0 deul       (502) staff       (20)    24054 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/model.py
+-rw-r--r--   0 deul       (502) staff       (20)    30916 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/sngp_transformer.py
+-rw-r--r--   0 deul       (502) staff       (20)    10296 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/transformer.py
+-rw-r--r--   0 deul       (502) staff       (20)    10731 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/spectral.py
+-rw-r--r--   0 deul       (502) staff       (20)    14223 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/lstm.py
+-rw-r--r--   0 deul       (502) staff       (20)    11830 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/bert.py
+-rw-r--r--   0 deul       (502) staff       (20)    18963 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/variational_lstm.py
+-rw-r--r--   0 deul       (502) staff       (20)    24659 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/defaults.py
+drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo.egg-info/
+-rw-r--r--   0 deul       (502) staff       (20)     9743 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo.egg-info/PKG-INFO
+-rw-r--r--   0 deul       (502) staff       (20)     1331 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo.egg-info/SOURCES.txt
+-rw-r--r--   0 deul       (502) staff       (20)      262 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo.egg-info/requires.txt
+-rw-r--r--   0 deul       (502) staff       (20)       20 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo.egg-info/top_level.txt
+-rw-r--r--   0 deul       (502) staff       (20)        1 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo.egg-info/dependency_links.txt
+-rw-r--r--   0 deul       (502) staff       (20)     8174 2023-02-27 11:21:57.000000 nlp-uncertainty-zoo-1.0.2/README.md
+-rw-r--r--   0 deul       (502) staff       (20)     1141 2023-04-16 20:54:52.000000 nlp-uncertainty-zoo-1.0.2/setup.py
+-rw-r--r--   0 deul       (502) staff       (20)       38 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `nlp-uncertainty-zoo-1.0.1/PKG-INFO` & `nlp-uncertainty-zoo-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: nlp-uncertainty-zoo
-Version: 1.0.1
-Summary: PyTorch Implementation of Models used for Uncertainty Estimation in Natural Language Processing.
-Home-page: https://github.com/Kaleidophon/nlp-uncertainty-zoo
-Author: Dennis Ulmer
-License: GPL
-Keywords: machine learning,deep learning,nlp,uncertainty,uncertainty estimationpytorch
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5.3
-Description-Content-Type: text/markdown
-
 # :robot::speech_balloon::question: nlp-uncertainty-zoo
 
 This repository contains implementations of several models used for uncertainty estimation in Natural Language processing,
 implemented in PyTorch. You can install the repository using pip:
 
     pip3 install nlp-uncertainty-zoo
```

### Comparing `nlp-uncertainty-zoo-1.0.1/README.md` & `nlp-uncertainty-zoo-1.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,113 +1,129 @@
-# :robot::speech_balloon::question: nlp-uncertainty-zoo
-
-This repository contains implementations of several models used for uncertainty estimation in Natural Language processing,
-implemented in PyTorch. You can install the repository using pip:
-
-    pip3 install nlp-uncertainty-zoo
-
-If you are using the repository in your academic research, please cite the paper below:
-
-    @inproceedings{ulmer-etal-2022-exploring,
-      title = "Exploring Predictive Uncertainty and Calibration in {NLP}: A Study on the Impact of Method {\&} Data Scarcity",
-      author = "Ulmer, Dennis  and
-        Frellsen, Jes  and
-        Hardmeier, Christian",
-      booktitle = "Findings of the Association for Computational Linguistics: EMNLP 2022",
-      month = dec,
-      year = "2022",
-      address = "Abu Dhabi, United Arab Emirates",
-      publisher = "Association for Computational Linguistics",
-      url = "https://aclanthology.org/2022.findings-emnlp.198",
-      pages = "2707--2735",
-  }
-
-To learn more about the package, consult the documentation [here](http://dennisulmer.eu/nlp-uncertainty-zoo/),
-check a Jupyter notebook demo [here](https://github.com/Kaleidophon/nlp-uncertainty-zoo/blob/main/demo.ipynb) or a Google 
-collab [here](https://colab.research.google.com/drive/1-Pl5lvcnpbGL2ZXLGDDNqvJB7Ew8uIsS?usp=sharing).
-
-### Included models
-
-The following models are implemented in the repository. They can all be imported by using `from nlp-uncertainty-zoo import <MODEL>`.
-For transformer-based model, furthermore a version of a model is available that uses a pre-trained BERT from the HuggingFace `transformers`.
-
-| Name | Description | Implementation | Paper |
-|---|---|---|---|
-| LSTM | Vanilla LSTM | `LSTM` | [Hochreiter & Schmidhuber, 1997](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.676.4320&rep=rep1&type=pdf) |
-| LSTM Ensemble | Ensemble of LSTMs | `LSTMEnsemble` | [Lakshminarayanan et al., 2017](https://proceedings.neurips.cc/paper/2017/file/9ef2ed4b7fd2c810847ffa5fa85bce38-Paper.pdf) | 
-| Bayesian LSTM | LSTM implementing Bayes-by-backprop [Blundell et al, 2015](http://proceedings.mlr.press/v37/blundell15.pdf) | `BayesianLSTM` | [Fortunato et al, 2017](https://arxiv.org/pdf/1704.02798.pdf) |
-| ST-tau LSTM | LSTM modelling transitions of a finite-state-automaton | `STTauLSTM` | [Wang et al., 2021](https://openreview.net/pdf?id=9EKHN1jOlA) |
-| Variational LSTM | LSTM with MC Dropout [(Gal & Ghahramani, 2016a)](http://proceedings.mlr.press/v48/gal16.pdf) | `VariationalLSTM` | [Gal & Ghahramani, 2016b](https://proceedings.neurips.cc/paper/2016/file/076a0c97d09cf1a0ec3e19c7f2529f2b-Paper.pdf) |
-| DDU Transformer, DDU BERT | Transformer / BERT with Gaussian Mixture Model fit to hidden features | `DDUTransformer`, `DDUBert` | [Mukhoti et al, 2021](https://arxiv.org/pdf/2102.11582.pdf) |
-| Variational Transformer, Variational BERT | Transformer / BERT with MC Dropout [(Gal & Ghahramani, 2016a)](http://proceedings.mlr.press/v48/gal16.pdf) | `VariationalTransformer`, `VariationalBert` | [Xiao et al., 2021](https://arxiv.org/pdf/2006.08344.pdf) |
-| DPP Transformer, DPP Bert | Transformer / BERT using determinantal point process dropout | `DPPTransformer`, `DPPBert` | [Shelmanov et al., 2021](https://aclanthology.org/2021.eacl-main.157) |
-| SNGP Transformer, SNGP BERT | Spectrally-normalized transformer / BERT using a Gaussian Process output layer | `SNGPTransformer`, `SNGPBert` | [Liu et al., 2022](http://arxiv.org/abs/2205.00403) |
-
-Contributions to include even more approaches are much appreciated!
-
-### Usage
-
-Each model comes in two versions, for instance `LSTMEnsemble` and `LSTMEnsembleModule`. The first one is supposed to be 
-used as an out-of-the-box solution, encapsulating all training logic and convenience functions. These include fitting 
-the model, prediction, getting the uncertainty for an input batch using a specific metric.
-
-```python
-model = LSTMEnsemble(**network_params, ensemble_size=10, is_sequence_classifer=False)
-model.fit(train_split=train_dataloader)
-model.get_logits(X)
-model.get_predictions(X)
-model.get_sequence_representation(X)
-model.available_uncertainty_metrics
-model.get_uncertainty(X)
-model.get_uncertainty(X, metric_name="mutual_information")
-```
-
-In comparison, the `-Module` class is supposed to me more simple and bare-bones, only containing the core model logic. 
-It is intended for research purposes, and for others who would like to embed the model into their own code base. While 
-the model class (e.g. `LSTMEnsemble`) inherits from `Model` and would require to implement certain methods, any `Module` class
-sticks closely to `torch.nn.Module`.
-
-To check what arguments are required to initialize and use different models, check [the documentation here](http://nlpuncertaintyzoo.dennisulmer.eu/).
-
-Also, check out the demo provided as a Jupyter notebook [here](https://github.com/Kaleidophon/nlp-uncertainty-zoo/blob/main/demo.ipynb) or a Google 
-collab [here](https://colab.research.google.com/drive/1-Pl5lvcnpbGL2ZXLGDDNqvJB7Ew8uIsS?usp=sharing).
-
-### Repository structure
-
-The repository has the following structure:
-
-* `models`: All model implementations.
-* `tests`: Unit tests. So far, only contains rudimentary tests to check that all output shapes are consistent between models and functions.
-* `utils`: Utility code (see below)
-    * `utils/custom_types.py`: Custom types used in the repository for type annotations.
-    * `utils/data.py`: Module containing data collators, and data builders - which build the dataloaders for a type of task and a specific dataset. Currently, language modelling, sequence labeling and sequence classification are supported.
-    * `utils/metrics.py`: Implementations of uncertainty metrics.
-    * `utils/samplers.py`: Dataset subsamplers for language modelling, sequence labelling and sequence classification.
-    * `utils/task_eval.py`: Functions used to evaluate task performance.
-    * `utils/uncertainty_eval.py`: Function used to evaluate uncertainty quality.
-    * `utils/calibration_eval.py`: Function used to evaluate calibration quality.
-* `config.py`: Define available datasets, model and tasks.
-* `defaults.py`: Define default config parameters for sequence classification and language modelling (**Note**: These might not be very good parameters).
-
-### Other features
-
-* **Weights & Biases integration**: You can track your experiments easily with weights & biases by passing a `wandb_run` argument to `model.fit()`!
-* **Easy fine-tuning via HuggingFace**: You can fine-tune arbitrary BERT models using their name from HuggingFace's `transformers`.
-
-### Contributing
-
-This repository is by no means perfect nor complete. If you find any bugs, please report them using the issue template,
-and, if you also happen to provide a fix, create a pull request! A GitHub template is provided for that as well.
-
-You would like to make a new addition to the repository? Follow the steps below:
-
-* **Adding a new model**: To add a new model, add a new module in the `models` directory. You will also need to implement
-a corresponding `Model` and `Module` class, inheriting from the classes of the same name in `models/model.py` and implementing all 
-  required functions. `Model` is supposed to be an out-of-the-box solution that you can start experimenting right away, whil 
-  `Module` should only include the most basic model logic in order to be easy to integrate into other codebases and allow tinkering.
-  
-* **Adding a new uncertainty metric**: To add a new uncertainty metric, add the function to `utils/metrics.py`. The function should take
-the logits of a model and output an uncertainty score (the higher the score, the more uncertain the model). The function should output 
-  a batch_size x sequence_length matrix, with batch_size x 1 for sequence classification tasks. After finishing the implementation, you can 
-  add the metric to the `single_prediction_uncertainty_metrics` of the `models.model.Model` class and `multi_prediction_uncertainty_metrics` of `models.model.MultiPredictionMixin` (if applicable).
-  
-You would like to add something else? Create an issue or contact me at dennis {dot} ulmer {at} mailbox {dot} org!
+Metadata-Version: 2.1
+Name: nlp-uncertainty-zoo
+Version: 1.0.2
+Summary: PyTorch Implementation of Models used for Uncertainty Estimation in Natural Language Processing.
+Home-page: https://github.com/Kaleidophon/nlp-uncertainty-zoo
+Author: Dennis Ulmer
+License: GPL
+Description: # :robot::speech_balloon::question: nlp-uncertainty-zoo
+        
+        This repository contains implementations of several models used for uncertainty estimation in Natural Language processing,
+        implemented in PyTorch. You can install the repository using pip:
+        
+            pip3 install nlp-uncertainty-zoo
+        
+        If you are using the repository in your academic research, please cite the paper below:
+        
+            @inproceedings{ulmer-etal-2022-exploring,
+              title = "Exploring Predictive Uncertainty and Calibration in {NLP}: A Study on the Impact of Method {\&} Data Scarcity",
+              author = "Ulmer, Dennis  and
+                Frellsen, Jes  and
+                Hardmeier, Christian",
+              booktitle = "Findings of the Association for Computational Linguistics: EMNLP 2022",
+              month = dec,
+              year = "2022",
+              address = "Abu Dhabi, United Arab Emirates",
+              publisher = "Association for Computational Linguistics",
+              url = "https://aclanthology.org/2022.findings-emnlp.198",
+              pages = "2707--2735",
+          }
+        
+        To learn more about the package, consult the documentation [here](http://dennisulmer.eu/nlp-uncertainty-zoo/),
+        check a Jupyter notebook demo [here](https://github.com/Kaleidophon/nlp-uncertainty-zoo/blob/main/demo.ipynb) or a Google 
+        collab [here](https://colab.research.google.com/drive/1-Pl5lvcnpbGL2ZXLGDDNqvJB7Ew8uIsS?usp=sharing).
+        
+        ### Included models
+        
+        The following models are implemented in the repository. They can all be imported by using `from nlp-uncertainty-zoo import <MODEL>`.
+        For transformer-based model, furthermore a version of a model is available that uses a pre-trained BERT from the HuggingFace `transformers`.
+        
+        | Name | Description | Implementation | Paper |
+        |---|---|---|---|
+        | LSTM | Vanilla LSTM | `LSTM` | [Hochreiter & Schmidhuber, 1997](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.676.4320&rep=rep1&type=pdf) |
+        | LSTM Ensemble | Ensemble of LSTMs | `LSTMEnsemble` | [Lakshminarayanan et al., 2017](https://proceedings.neurips.cc/paper/2017/file/9ef2ed4b7fd2c810847ffa5fa85bce38-Paper.pdf) | 
+        | Bayesian LSTM | LSTM implementing Bayes-by-backprop [Blundell et al, 2015](http://proceedings.mlr.press/v37/blundell15.pdf) | `BayesianLSTM` | [Fortunato et al, 2017](https://arxiv.org/pdf/1704.02798.pdf) |
+        | ST-tau LSTM | LSTM modelling transitions of a finite-state-automaton | `STTauLSTM` | [Wang et al., 2021](https://openreview.net/pdf?id=9EKHN1jOlA) |
+        | Variational LSTM | LSTM with MC Dropout [(Gal & Ghahramani, 2016a)](http://proceedings.mlr.press/v48/gal16.pdf) | `VariationalLSTM` | [Gal & Ghahramani, 2016b](https://proceedings.neurips.cc/paper/2016/file/076a0c97d09cf1a0ec3e19c7f2529f2b-Paper.pdf) |
+        | DDU Transformer, DDU BERT | Transformer / BERT with Gaussian Mixture Model fit to hidden features | `DDUTransformer`, `DDUBert` | [Mukhoti et al, 2021](https://arxiv.org/pdf/2102.11582.pdf) |
+        | Variational Transformer, Variational BERT | Transformer / BERT with MC Dropout [(Gal & Ghahramani, 2016a)](http://proceedings.mlr.press/v48/gal16.pdf) | `VariationalTransformer`, `VariationalBert` | [Xiao et al., 2021](https://arxiv.org/pdf/2006.08344.pdf) |
+        | DPP Transformer, DPP Bert | Transformer / BERT using determinantal point process dropout | `DPPTransformer`, `DPPBert` | [Shelmanov et al., 2021](https://aclanthology.org/2021.eacl-main.157) |
+        | SNGP Transformer, SNGP BERT | Spectrally-normalized transformer / BERT using a Gaussian Process output layer | `SNGPTransformer`, `SNGPBert` | [Liu et al., 2022](http://arxiv.org/abs/2205.00403) |
+        
+        Contributions to include even more approaches are much appreciated!
+        
+        ### Usage
+        
+        Each model comes in two versions, for instance `LSTMEnsemble` and `LSTMEnsembleModule`. The first one is supposed to be 
+        used as an out-of-the-box solution, encapsulating all training logic and convenience functions. These include fitting 
+        the model, prediction, getting the uncertainty for an input batch using a specific metric.
+        
+        ```python
+        model = LSTMEnsemble(**network_params, ensemble_size=10, is_sequence_classifer=False)
+        model.fit(train_split=train_dataloader)
+        model.get_logits(X)
+        model.get_predictions(X)
+        model.get_sequence_representation(X)
+        model.available_uncertainty_metrics
+        model.get_uncertainty(X)
+        model.get_uncertainty(X, metric_name="mutual_information")
+        ```
+        
+        In comparison, the `-Module` class is supposed to me more simple and bare-bones, only containing the core model logic. 
+        It is intended for research purposes, and for others who would like to embed the model into their own code base. While 
+        the model class (e.g. `LSTMEnsemble`) inherits from `Model` and would require to implement certain methods, any `Module` class
+        sticks closely to `torch.nn.Module`.
+        
+        To check what arguments are required to initialize and use different models, check [the documentation here](http://nlpuncertaintyzoo.dennisulmer.eu/).
+        
+        Also, check out the demo provided as a Jupyter notebook [here](https://github.com/Kaleidophon/nlp-uncertainty-zoo/blob/main/demo.ipynb) or a Google 
+        collab [here](https://colab.research.google.com/drive/1-Pl5lvcnpbGL2ZXLGDDNqvJB7Ew8uIsS?usp=sharing).
+        
+        ### Repository structure
+        
+        The repository has the following structure:
+        
+        * `models`: All model implementations.
+        * `tests`: Unit tests. So far, only contains rudimentary tests to check that all output shapes are consistent between models and functions.
+        * `utils`: Utility code (see below)
+            * `utils/custom_types.py`: Custom types used in the repository for type annotations.
+            * `utils/data.py`: Module containing data collators, and data builders - which build the dataloaders for a type of task and a specific dataset. Currently, language modelling, sequence labeling and sequence classification are supported.
+            * `utils/metrics.py`: Implementations of uncertainty metrics.
+            * `utils/samplers.py`: Dataset subsamplers for language modelling, sequence labelling and sequence classification.
+            * `utils/task_eval.py`: Functions used to evaluate task performance.
+            * `utils/uncertainty_eval.py`: Function used to evaluate uncertainty quality.
+            * `utils/calibration_eval.py`: Function used to evaluate calibration quality.
+        * `config.py`: Define available datasets, model and tasks.
+        * `defaults.py`: Define default config parameters for sequence classification and language modelling (**Note**: These might not be very good parameters).
+        
+        ### Other features
+        
+        * **Weights & Biases integration**: You can track your experiments easily with weights & biases by passing a `wandb_run` argument to `model.fit()`!
+        * **Easy fine-tuning via HuggingFace**: You can fine-tune arbitrary BERT models using their name from HuggingFace's `transformers`.
+        
+        ### Contributing
+        
+        This repository is by no means perfect nor complete. If you find any bugs, please report them using the issue template,
+        and, if you also happen to provide a fix, create a pull request! A GitHub template is provided for that as well.
+        
+        You would like to make a new addition to the repository? Follow the steps below:
+        
+        * **Adding a new model**: To add a new model, add a new module in the `models` directory. You will also need to implement
+        a corresponding `Model` and `Module` class, inheriting from the classes of the same name in `models/model.py` and implementing all 
+          required functions. `Model` is supposed to be an out-of-the-box solution that you can start experimenting right away, whil 
+          `Module` should only include the most basic model logic in order to be easy to integrate into other codebases and allow tinkering.
+          
+        * **Adding a new uncertainty metric**: To add a new uncertainty metric, add the function to `utils/metrics.py`. The function should take
+        the logits of a model and output an uncertainty score (the higher the score, the more uncertain the model). The function should output 
+          a batch_size x sequence_length matrix, with batch_size x 1 for sequence classification tasks. After finishing the implementation, you can 
+          add the metric to the `single_prediction_uncertainty_metrics` of the `models.model.Model` class and `multi_prediction_uncertainty_metrics` of `models.model.MultiPredictionMixin` (if applicable).
+          
+        You would like to add something else? Create an issue or contact me at dennis {dot} ulmer {at} mailbox {dot} org!
+        
+Keywords: machine learning,deep learning,nlp,uncertainty,uncertainty estimationpytorch
+Platform: UNKNOWN
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5.3
+Description-Content-Type: text/markdown
```

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/__init__.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/__init__.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/config.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/config.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/defaults.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/defaults.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/__init__.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/bayesian_lstm.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/bayesian_lstm.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/bert.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/bert.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/ddu_transformer.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/ddu_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
                 attention_mask, input_ids, labels = (
                     batch["attention_mask"].to(self.device),
                     batch["input_ids"].to(self.device),
                     batch["labels"].to(self.device),
                 )
 
-                hidden = self.get_hidden(input_ids, attention_mask=attention_mask)
+                hidden = self.get_hidden_representation(input_ids, attention_mask=attention_mask)
 
                 if not self.is_sequence_classifier:
                     # Filter our labels and activations for uninformative classes like PAD
                     batch_mask = torch.all(
                         torch.stack([input_ids != idx for idx in self.ignore_indices]), dim=0
                     )
                     labels = labels[batch_mask]
@@ -149,15 +149,15 @@
 
         Returns
         -------
         torch.FloatTensor
             Probability of the input under every mixture component, with one component per class.
         """
         batch_size = input_.shape[0]
-        hidden = self.get_hidden(input_)  # batch_size x seq_length x input_size
+        hidden = self.get_hidden_representation(input_)  # batch_size x seq_length x input_size
         hidden = (
             self.get_sequence_representation(hidden).squeeze(1)
             if self.is_sequence_classifier
             else rearrange(hidden, "b s i -> (b s) i")
         )
 
         if self.pca is not None:
```

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/dpp_transformer.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/dpp_transformer.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/lstm.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/lstm.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/lstm_ensemble.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/lstm_ensemble.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/model.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/model.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/sngp_transformer.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/sngp_transformer.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/spectral.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/spectral.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/st_tau_lstm.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/st_tau_lstm.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/transformer.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/transformer.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/variational_lstm.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/variational_lstm.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/models/variational_transformer.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/variational_transformer.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/tests/test_module_functions.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/tests/test_module_functions.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/utils/calibration_eval.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/calibration_eval.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/utils/data.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/data.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/utils/metrics.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/utils/samplers.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/samplers.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/utils/task_eval.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/task_eval.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo/utils/uncertainty_eval.py` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/uncertainty_eval.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo.egg-info/PKG-INFO` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,128 +1,129 @@
 Metadata-Version: 2.1
 Name: nlp-uncertainty-zoo
-Version: 1.0.1
+Version: 1.0.2
 Summary: PyTorch Implementation of Models used for Uncertainty Estimation in Natural Language Processing.
 Home-page: https://github.com/Kaleidophon/nlp-uncertainty-zoo
 Author: Dennis Ulmer
 License: GPL
+Description: # :robot::speech_balloon::question: nlp-uncertainty-zoo
+        
+        This repository contains implementations of several models used for uncertainty estimation in Natural Language processing,
+        implemented in PyTorch. You can install the repository using pip:
+        
+            pip3 install nlp-uncertainty-zoo
+        
+        If you are using the repository in your academic research, please cite the paper below:
+        
+            @inproceedings{ulmer-etal-2022-exploring,
+              title = "Exploring Predictive Uncertainty and Calibration in {NLP}: A Study on the Impact of Method {\&} Data Scarcity",
+              author = "Ulmer, Dennis  and
+                Frellsen, Jes  and
+                Hardmeier, Christian",
+              booktitle = "Findings of the Association for Computational Linguistics: EMNLP 2022",
+              month = dec,
+              year = "2022",
+              address = "Abu Dhabi, United Arab Emirates",
+              publisher = "Association for Computational Linguistics",
+              url = "https://aclanthology.org/2022.findings-emnlp.198",
+              pages = "2707--2735",
+          }
+        
+        To learn more about the package, consult the documentation [here](http://dennisulmer.eu/nlp-uncertainty-zoo/),
+        check a Jupyter notebook demo [here](https://github.com/Kaleidophon/nlp-uncertainty-zoo/blob/main/demo.ipynb) or a Google 
+        collab [here](https://colab.research.google.com/drive/1-Pl5lvcnpbGL2ZXLGDDNqvJB7Ew8uIsS?usp=sharing).
+        
+        ### Included models
+        
+        The following models are implemented in the repository. They can all be imported by using `from nlp-uncertainty-zoo import <MODEL>`.
+        For transformer-based model, furthermore a version of a model is available that uses a pre-trained BERT from the HuggingFace `transformers`.
+        
+        | Name | Description | Implementation | Paper |
+        |---|---|---|---|
+        | LSTM | Vanilla LSTM | `LSTM` | [Hochreiter & Schmidhuber, 1997](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.676.4320&rep=rep1&type=pdf) |
+        | LSTM Ensemble | Ensemble of LSTMs | `LSTMEnsemble` | [Lakshminarayanan et al., 2017](https://proceedings.neurips.cc/paper/2017/file/9ef2ed4b7fd2c810847ffa5fa85bce38-Paper.pdf) | 
+        | Bayesian LSTM | LSTM implementing Bayes-by-backprop [Blundell et al, 2015](http://proceedings.mlr.press/v37/blundell15.pdf) | `BayesianLSTM` | [Fortunato et al, 2017](https://arxiv.org/pdf/1704.02798.pdf) |
+        | ST-tau LSTM | LSTM modelling transitions of a finite-state-automaton | `STTauLSTM` | [Wang et al., 2021](https://openreview.net/pdf?id=9EKHN1jOlA) |
+        | Variational LSTM | LSTM with MC Dropout [(Gal & Ghahramani, 2016a)](http://proceedings.mlr.press/v48/gal16.pdf) | `VariationalLSTM` | [Gal & Ghahramani, 2016b](https://proceedings.neurips.cc/paper/2016/file/076a0c97d09cf1a0ec3e19c7f2529f2b-Paper.pdf) |
+        | DDU Transformer, DDU BERT | Transformer / BERT with Gaussian Mixture Model fit to hidden features | `DDUTransformer`, `DDUBert` | [Mukhoti et al, 2021](https://arxiv.org/pdf/2102.11582.pdf) |
+        | Variational Transformer, Variational BERT | Transformer / BERT with MC Dropout [(Gal & Ghahramani, 2016a)](http://proceedings.mlr.press/v48/gal16.pdf) | `VariationalTransformer`, `VariationalBert` | [Xiao et al., 2021](https://arxiv.org/pdf/2006.08344.pdf) |
+        | DPP Transformer, DPP Bert | Transformer / BERT using determinantal point process dropout | `DPPTransformer`, `DPPBert` | [Shelmanov et al., 2021](https://aclanthology.org/2021.eacl-main.157) |
+        | SNGP Transformer, SNGP BERT | Spectrally-normalized transformer / BERT using a Gaussian Process output layer | `SNGPTransformer`, `SNGPBert` | [Liu et al., 2022](http://arxiv.org/abs/2205.00403) |
+        
+        Contributions to include even more approaches are much appreciated!
+        
+        ### Usage
+        
+        Each model comes in two versions, for instance `LSTMEnsemble` and `LSTMEnsembleModule`. The first one is supposed to be 
+        used as an out-of-the-box solution, encapsulating all training logic and convenience functions. These include fitting 
+        the model, prediction, getting the uncertainty for an input batch using a specific metric.
+        
+        ```python
+        model = LSTMEnsemble(**network_params, ensemble_size=10, is_sequence_classifer=False)
+        model.fit(train_split=train_dataloader)
+        model.get_logits(X)
+        model.get_predictions(X)
+        model.get_sequence_representation(X)
+        model.available_uncertainty_metrics
+        model.get_uncertainty(X)
+        model.get_uncertainty(X, metric_name="mutual_information")
+        ```
+        
+        In comparison, the `-Module` class is supposed to me more simple and bare-bones, only containing the core model logic. 
+        It is intended for research purposes, and for others who would like to embed the model into their own code base. While 
+        the model class (e.g. `LSTMEnsemble`) inherits from `Model` and would require to implement certain methods, any `Module` class
+        sticks closely to `torch.nn.Module`.
+        
+        To check what arguments are required to initialize and use different models, check [the documentation here](http://nlpuncertaintyzoo.dennisulmer.eu/).
+        
+        Also, check out the demo provided as a Jupyter notebook [here](https://github.com/Kaleidophon/nlp-uncertainty-zoo/blob/main/demo.ipynb) or a Google 
+        collab [here](https://colab.research.google.com/drive/1-Pl5lvcnpbGL2ZXLGDDNqvJB7Ew8uIsS?usp=sharing).
+        
+        ### Repository structure
+        
+        The repository has the following structure:
+        
+        * `models`: All model implementations.
+        * `tests`: Unit tests. So far, only contains rudimentary tests to check that all output shapes are consistent between models and functions.
+        * `utils`: Utility code (see below)
+            * `utils/custom_types.py`: Custom types used in the repository for type annotations.
+            * `utils/data.py`: Module containing data collators, and data builders - which build the dataloaders for a type of task and a specific dataset. Currently, language modelling, sequence labeling and sequence classification are supported.
+            * `utils/metrics.py`: Implementations of uncertainty metrics.
+            * `utils/samplers.py`: Dataset subsamplers for language modelling, sequence labelling and sequence classification.
+            * `utils/task_eval.py`: Functions used to evaluate task performance.
+            * `utils/uncertainty_eval.py`: Function used to evaluate uncertainty quality.
+            * `utils/calibration_eval.py`: Function used to evaluate calibration quality.
+        * `config.py`: Define available datasets, model and tasks.
+        * `defaults.py`: Define default config parameters for sequence classification and language modelling (**Note**: These might not be very good parameters).
+        
+        ### Other features
+        
+        * **Weights & Biases integration**: You can track your experiments easily with weights & biases by passing a `wandb_run` argument to `model.fit()`!
+        * **Easy fine-tuning via HuggingFace**: You can fine-tune arbitrary BERT models using their name from HuggingFace's `transformers`.
+        
+        ### Contributing
+        
+        This repository is by no means perfect nor complete. If you find any bugs, please report them using the issue template,
+        and, if you also happen to provide a fix, create a pull request! A GitHub template is provided for that as well.
+        
+        You would like to make a new addition to the repository? Follow the steps below:
+        
+        * **Adding a new model**: To add a new model, add a new module in the `models` directory. You will also need to implement
+        a corresponding `Model` and `Module` class, inheriting from the classes of the same name in `models/model.py` and implementing all 
+          required functions. `Model` is supposed to be an out-of-the-box solution that you can start experimenting right away, whil 
+          `Module` should only include the most basic model logic in order to be easy to integrate into other codebases and allow tinkering.
+          
+        * **Adding a new uncertainty metric**: To add a new uncertainty metric, add the function to `utils/metrics.py`. The function should take
+        the logits of a model and output an uncertainty score (the higher the score, the more uncertain the model). The function should output 
+          a batch_size x sequence_length matrix, with batch_size x 1 for sequence classification tasks. After finishing the implementation, you can 
+          add the metric to the `single_prediction_uncertainty_metrics` of the `models.model.Model` class and `multi_prediction_uncertainty_metrics` of `models.model.MultiPredictionMixin` (if applicable).
+          
+        You would like to add something else? Create an issue or contact me at dennis {dot} ulmer {at} mailbox {dot} org!
+        
 Keywords: machine learning,deep learning,nlp,uncertainty,uncertainty estimationpytorch
+Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5.3
 Description-Content-Type: text/markdown
-
-# :robot::speech_balloon::question: nlp-uncertainty-zoo
-
-This repository contains implementations of several models used for uncertainty estimation in Natural Language processing,
-implemented in PyTorch. You can install the repository using pip:
-
-    pip3 install nlp-uncertainty-zoo
-
-If you are using the repository in your academic research, please cite the paper below:
-
-    @inproceedings{ulmer-etal-2022-exploring,
-      title = "Exploring Predictive Uncertainty and Calibration in {NLP}: A Study on the Impact of Method {\&} Data Scarcity",
-      author = "Ulmer, Dennis  and
-        Frellsen, Jes  and
-        Hardmeier, Christian",
-      booktitle = "Findings of the Association for Computational Linguistics: EMNLP 2022",
-      month = dec,
-      year = "2022",
-      address = "Abu Dhabi, United Arab Emirates",
-      publisher = "Association for Computational Linguistics",
-      url = "https://aclanthology.org/2022.findings-emnlp.198",
-      pages = "2707--2735",
-  }
-
-To learn more about the package, consult the documentation [here](http://dennisulmer.eu/nlp-uncertainty-zoo/),
-check a Jupyter notebook demo [here](https://github.com/Kaleidophon/nlp-uncertainty-zoo/blob/main/demo.ipynb) or a Google 
-collab [here](https://colab.research.google.com/drive/1-Pl5lvcnpbGL2ZXLGDDNqvJB7Ew8uIsS?usp=sharing).
-
-### Included models
-
-The following models are implemented in the repository. They can all be imported by using `from nlp-uncertainty-zoo import <MODEL>`.
-For transformer-based model, furthermore a version of a model is available that uses a pre-trained BERT from the HuggingFace `transformers`.
-
-| Name | Description | Implementation | Paper |
-|---|---|---|---|
-| LSTM | Vanilla LSTM | `LSTM` | [Hochreiter & Schmidhuber, 1997](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.676.4320&rep=rep1&type=pdf) |
-| LSTM Ensemble | Ensemble of LSTMs | `LSTMEnsemble` | [Lakshminarayanan et al., 2017](https://proceedings.neurips.cc/paper/2017/file/9ef2ed4b7fd2c810847ffa5fa85bce38-Paper.pdf) | 
-| Bayesian LSTM | LSTM implementing Bayes-by-backprop [Blundell et al, 2015](http://proceedings.mlr.press/v37/blundell15.pdf) | `BayesianLSTM` | [Fortunato et al, 2017](https://arxiv.org/pdf/1704.02798.pdf) |
-| ST-tau LSTM | LSTM modelling transitions of a finite-state-automaton | `STTauLSTM` | [Wang et al., 2021](https://openreview.net/pdf?id=9EKHN1jOlA) |
-| Variational LSTM | LSTM with MC Dropout [(Gal & Ghahramani, 2016a)](http://proceedings.mlr.press/v48/gal16.pdf) | `VariationalLSTM` | [Gal & Ghahramani, 2016b](https://proceedings.neurips.cc/paper/2016/file/076a0c97d09cf1a0ec3e19c7f2529f2b-Paper.pdf) |
-| DDU Transformer, DDU BERT | Transformer / BERT with Gaussian Mixture Model fit to hidden features | `DDUTransformer`, `DDUBert` | [Mukhoti et al, 2021](https://arxiv.org/pdf/2102.11582.pdf) |
-| Variational Transformer, Variational BERT | Transformer / BERT with MC Dropout [(Gal & Ghahramani, 2016a)](http://proceedings.mlr.press/v48/gal16.pdf) | `VariationalTransformer`, `VariationalBert` | [Xiao et al., 2021](https://arxiv.org/pdf/2006.08344.pdf) |
-| DPP Transformer, DPP Bert | Transformer / BERT using determinantal point process dropout | `DPPTransformer`, `DPPBert` | [Shelmanov et al., 2021](https://aclanthology.org/2021.eacl-main.157) |
-| SNGP Transformer, SNGP BERT | Spectrally-normalized transformer / BERT using a Gaussian Process output layer | `SNGPTransformer`, `SNGPBert` | [Liu et al., 2022](http://arxiv.org/abs/2205.00403) |
-
-Contributions to include even more approaches are much appreciated!
-
-### Usage
-
-Each model comes in two versions, for instance `LSTMEnsemble` and `LSTMEnsembleModule`. The first one is supposed to be 
-used as an out-of-the-box solution, encapsulating all training logic and convenience functions. These include fitting 
-the model, prediction, getting the uncertainty for an input batch using a specific metric.
-
-```python
-model = LSTMEnsemble(**network_params, ensemble_size=10, is_sequence_classifer=False)
-model.fit(train_split=train_dataloader)
-model.get_logits(X)
-model.get_predictions(X)
-model.get_sequence_representation(X)
-model.available_uncertainty_metrics
-model.get_uncertainty(X)
-model.get_uncertainty(X, metric_name="mutual_information")
-```
-
-In comparison, the `-Module` class is supposed to me more simple and bare-bones, only containing the core model logic. 
-It is intended for research purposes, and for others who would like to embed the model into their own code base. While 
-the model class (e.g. `LSTMEnsemble`) inherits from `Model` and would require to implement certain methods, any `Module` class
-sticks closely to `torch.nn.Module`.
-
-To check what arguments are required to initialize and use different models, check [the documentation here](http://nlpuncertaintyzoo.dennisulmer.eu/).
-
-Also, check out the demo provided as a Jupyter notebook [here](https://github.com/Kaleidophon/nlp-uncertainty-zoo/blob/main/demo.ipynb) or a Google 
-collab [here](https://colab.research.google.com/drive/1-Pl5lvcnpbGL2ZXLGDDNqvJB7Ew8uIsS?usp=sharing).
-
-### Repository structure
-
-The repository has the following structure:
-
-* `models`: All model implementations.
-* `tests`: Unit tests. So far, only contains rudimentary tests to check that all output shapes are consistent between models and functions.
-* `utils`: Utility code (see below)
-    * `utils/custom_types.py`: Custom types used in the repository for type annotations.
-    * `utils/data.py`: Module containing data collators, and data builders - which build the dataloaders for a type of task and a specific dataset. Currently, language modelling, sequence labeling and sequence classification are supported.
-    * `utils/metrics.py`: Implementations of uncertainty metrics.
-    * `utils/samplers.py`: Dataset subsamplers for language modelling, sequence labelling and sequence classification.
-    * `utils/task_eval.py`: Functions used to evaluate task performance.
-    * `utils/uncertainty_eval.py`: Function used to evaluate uncertainty quality.
-    * `utils/calibration_eval.py`: Function used to evaluate calibration quality.
-* `config.py`: Define available datasets, model and tasks.
-* `defaults.py`: Define default config parameters for sequence classification and language modelling (**Note**: These might not be very good parameters).
-
-### Other features
-
-* **Weights & Biases integration**: You can track your experiments easily with weights & biases by passing a `wandb_run` argument to `model.fit()`!
-* **Easy fine-tuning via HuggingFace**: You can fine-tune arbitrary BERT models using their name from HuggingFace's `transformers`.
-
-### Contributing
-
-This repository is by no means perfect nor complete. If you find any bugs, please report them using the issue template,
-and, if you also happen to provide a fix, create a pull request! A GitHub template is provided for that as well.
-
-You would like to make a new addition to the repository? Follow the steps below:
-
-* **Adding a new model**: To add a new model, add a new module in the `models` directory. You will also need to implement
-a corresponding `Model` and `Module` class, inheriting from the classes of the same name in `models/model.py` and implementing all 
-  required functions. `Model` is supposed to be an out-of-the-box solution that you can start experimenting right away, whil 
-  `Module` should only include the most basic model logic in order to be easy to integrate into other codebases and allow tinkering.
-  
-* **Adding a new uncertainty metric**: To add a new uncertainty metric, add the function to `utils/metrics.py`. The function should take
-the logits of a model and output an uncertainty score (the higher the score, the more uncertain the model). The function should output 
-  a batch_size x sequence_length matrix, with batch_size x 1 for sequence classification tasks. After finishing the implementation, you can 
-  add the metric to the `single_prediction_uncertainty_metrics` of the `models.model.Model` class and `multi_prediction_uncertainty_metrics` of `models.model.MultiPredictionMixin` (if applicable).
-  
-You would like to add something else? Create an issue or contact me at dennis {dot} ulmer {at} mailbox {dot} org!
```

### Comparing `nlp-uncertainty-zoo-1.0.1/nlp_uncertainty_zoo.egg-info/SOURCES.txt` & `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.1/setup.py` & `nlp-uncertainty-zoo-1.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     required = [line for line in f.read().splitlines() if not line.startswith("git")]
 
 setup(
     name="nlp-uncertainty-zoo",
-    version="1.0.1",
+    version="1.0.2",
     author="Dennis Ulmer",
     description="PyTorch Implementation of Models used for Uncertainty Estimation in Natural Language Processing.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Kaleidophon/nlp-uncertainty-zoo",
     classifiers=[
         "Intended Audience :: Science/Research",
```

