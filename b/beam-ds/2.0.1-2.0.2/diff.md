# Comparing `tmp/beam-ds-2.0.1.tar.gz` & `tmp/beam-ds-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beam-ds-2.0.1.tar", last modified: Thu Apr 13 21:30:31 2023, max compression
+gzip compressed data, was "beam-ds-2.0.2.tar", last modified: Sun Apr 16 19:45:05 2023, max compression
```

## Comparing `beam-ds-2.0.1.tar` & `beam-ds-2.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:25:59.590881 beam-ds-2.0.1/
--rw-r--r--   0 root         (0) root         (0)     1080 2023-04-01 19:19:43.000000 beam-ds-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2184 2023-04-13 21:25:59.591992 beam-ds-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1767 2023-04-01 19:19:43.000000 beam-ds-2.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)      114 2023-04-01 19:19:43.000000 beam-ds-2.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      718 2023-04-13 21:25:59.595897 beam-ds-2.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-01 19:19:43.000000 beam-ds-2.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:25:59.475676 beam-ds-2.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:25:59.568319 beam-ds-2.0.1/src/beam/
--rw-r--r--   0 root         (0) root         (0)      897 2023-04-01 19:19:43.000000 beam-ds-2.0.1/src/beam/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-02 17:55:04.000000 beam-ds-2.0.1/src/beam/_version.py
--rw-r--r--   0 root         (0) root         (0)    51954 2023-04-13 21:12:29.000000 beam-ds-2.0.1/src/beam/algorithm.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-01 19:19:43.000000 beam-ds-2.0.1/src/beam/beam_mlflow.py
--rw-r--r--   0 root         (0) root         (0)    16780 2023-04-01 19:19:43.000000 beam-ds-2.0.1/src/beam/config.py
--rw-r--r--   0 root         (0) root         (0)    75918 2023-04-13 20:08:35.000000 beam-ds-2.0.1/src/beam/data.py
--rw-r--r--   0 root         (0) root         (0)    12112 2023-04-01 19:19:43.000000 beam-ds-2.0.1/src/beam/data_tensor.py
--rw-r--r--   0 root         (0) root         (0)    25750 2023-04-13 21:25:42.000000 beam-ds-2.0.1/src/beam/dataset.py
--rw-r--r--   0 root         (0) root         (0)    36080 2023-04-13 21:01:26.000000 beam-ds-2.0.1/src/beam/experiment.py
--rw-r--r--   0 root         (0) root         (0)    31634 2023-04-01 19:19:43.000000 beam-ds-2.0.1/src/beam/model.py
--rw-r--r--   0 root         (0) root         (0)    13309 2023-04-01 19:19:43.000000 beam-ds-2.0.1/src/beam/optim.py
--rw-r--r--   0 root         (0) root         (0)     9613 2023-04-01 19:19:43.000000 beam-ds-2.0.1/src/beam/packed_folds.py
--rw-r--r--   0 root         (0) root         (0)    12102 2023-04-01 19:19:43.000000 beam-ds-2.0.1/src/beam/parallel.py
--rw-r--r--   0 root         (0) root         (0)    20559 2023-04-03 18:57:13.000000 beam-ds-2.0.1/src/beam/path.py
--rw-r--r--   0 root         (0) root         (0)    15377 2023-04-02 17:55:04.000000 beam-ds-2.0.1/src/beam/processor.py
--rw-r--r--   0 root         (0) root         (0)     2973 2023-04-01 19:19:43.000000 beam-ds-2.0.1/src/beam/server.py
--rw-r--r--   0 root         (0) root         (0)    35911 2023-04-01 19:19:43.000000 beam-ds-2.0.1/src/beam/ssl.py
--rw-r--r--   0 root         (0) root         (0)    11533 2023-04-01 19:19:43.000000 beam-ds-2.0.1/src/beam/study.py
--rw-r--r--   0 root         (0) root         (0)    51684 2023-04-13 19:57:36.000000 beam-ds-2.0.1/src/beam/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 21:25:59.587351 beam-ds-2.0.1/src/beam_ds.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2184 2023-04-13 21:25:59.000000 beam-ds-2.0.1/src/beam_ds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      608 2023-04-13 21:25:59.000000 beam-ds-2.0.1/src/beam_ds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 21:25:59.000000 beam-ds-2.0.1/src/beam_ds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-04-13 21:25:59.000000 beam-ds-2.0.1/src/beam_ds.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-13 21:25:59.000000 beam-ds-2.0.1/src/beam_ds.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 19:40:34.637224 beam-ds-2.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-04-01 19:19:43.000000 beam-ds-2.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-04-16 19:40:34.638217 beam-ds-2.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-04-01 19:19:43.000000 beam-ds-2.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      114 2023-04-01 19:19:43.000000 beam-ds-2.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      718 2023-04-16 19:40:34.647206 beam-ds-2.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       39 2023-04-01 19:19:43.000000 beam-ds-2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 19:40:34.510285 beam-ds-2.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 19:40:34.614237 beam-ds-2.0.2/src/beam/
+-rw-r--r--   0 root         (0) root         (0)      909 2023-04-14 13:16:22.000000 beam-ds-2.0.2/src/beam/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      111 2023-04-16 19:37:48.000000 beam-ds-2.0.2/src/beam/_version.py
+-rw-r--r--   0 root         (0) root         (0)    52097 2023-04-15 21:36:48.000000 beam-ds-2.0.2/src/beam/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-01 19:19:43.000000 beam-ds-2.0.2/src/beam/beam_mlflow.py
+-rw-r--r--   0 root         (0) root         (0)    17001 2023-04-15 21:36:48.000000 beam-ds-2.0.2/src/beam/config.py
+-rw-r--r--   0 root         (0) root         (0)    75918 2023-04-13 20:08:35.000000 beam-ds-2.0.2/src/beam/data.py
+-rw-r--r--   0 root         (0) root         (0)    12112 2023-04-01 19:19:43.000000 beam-ds-2.0.2/src/beam/data_tensor.py
+-rw-r--r--   0 root         (0) root         (0)    25836 2023-04-14 14:04:41.000000 beam-ds-2.0.2/src/beam/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    36437 2023-04-15 21:52:36.000000 beam-ds-2.0.2/src/beam/experiment.py
+-rw-r--r--   0 root         (0) root         (0)    32143 2023-04-09 04:35:52.000000 beam-ds-2.0.2/src/beam/model.py
+-rw-r--r--   0 root         (0) root         (0)    13309 2023-04-01 19:19:43.000000 beam-ds-2.0.2/src/beam/optim.py
+-rw-r--r--   0 root         (0) root         (0)     9613 2023-04-01 19:19:43.000000 beam-ds-2.0.2/src/beam/packed_folds.py
+-rw-r--r--   0 root         (0) root         (0)    12102 2023-04-01 19:19:43.000000 beam-ds-2.0.2/src/beam/parallel.py
+-rw-r--r--   0 root         (0) root         (0)    21001 2023-04-16 19:14:33.000000 beam-ds-2.0.2/src/beam/path.py
+-rw-r--r--   0 root         (0) root         (0)    15377 2023-04-02 17:55:04.000000 beam-ds-2.0.2/src/beam/processor.py
+-rw-r--r--   0 root         (0) root         (0)     2973 2023-04-01 19:19:43.000000 beam-ds-2.0.2/src/beam/server.py
+-rw-r--r--   0 root         (0) root         (0)    35911 2023-04-01 19:19:43.000000 beam-ds-2.0.2/src/beam/ssl.py
+-rw-r--r--   0 root         (0) root         (0)    11533 2023-04-01 19:19:43.000000 beam-ds-2.0.2/src/beam/study.py
+-rw-r--r--   0 root         (0) root         (0)    51731 2023-04-15 21:13:48.000000 beam-ds-2.0.2/src/beam/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 19:40:34.632751 beam-ds-2.0.2/src/beam_ds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-04-16 19:40:34.000000 beam-ds-2.0.2/src/beam_ds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      608 2023-04-16 19:40:34.000000 beam-ds-2.0.2/src/beam_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 19:40:34.000000 beam-ds-2.0.2/src/beam_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-04-16 19:40:34.000000 beam-ds-2.0.2/src/beam_ds.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-16 19:40:34.000000 beam-ds-2.0.2/src/beam_ds.egg-info/top_level.txt
```

### Comparing `beam-ds-2.0.1/LICENSE` & `beam-ds-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `beam-ds-2.0.1/PKG-INFO` & `beam-ds-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beam-ds
-Version: 2.0.1
+Version: 2.0.2
 Summary: Beam Datascience package
 Home-page: https://github.com/mlutils/beamds
 Author: Beam Maintainer
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/mlutils/beamds/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `beam-ds-2.0.1/README.md` & `beam-ds-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `beam-ds-2.0.1/setup.cfg` & `beam-ds-2.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `beam-ds-2.0.1/src/beam/__init__.py` & `beam-ds-2.0.2/src/beam/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .dataset import UniversalBatchSampler, UniversalDataset
 from .packed_folds import PackedFolds
 from .config import get_beam_parser, beam_arguments
 from .config import boolean_feature as beam_boolean_feature
 from .experiment import Experiment, beam_algorithm_generator
 from .study import Study
-from .utils import setup, cleanup, check_type, slice_to_index, beam_logger, beam_device, as_tensor, \
+from .utils import setup_distributed, cleanup, check_type, slice_to_index, beam_logger, beam_device, as_tensor, \
     batch_augmentation, as_numpy
 from .utils import tqdm_beam as tqdm
 from .algorithm import Algorithm
 from .model import LinearNet, PackedSet, BetterEmbedding, SplineEmbedding, copy_network, reset_network
 from .data_tensor import DataTensor
 from .optim import BeamOptimizer, BeamScheduler
 # from .ssl import BeamSimilarity, Similarities, BeamSSL, BYOL, BeamVICReg, BarlowTwins, VICReg, SimCLR, SimSiam
```

### Comparing `beam-ds-2.0.1/src/beam/algorithm.py` & `beam-ds-2.0.2/src/beam/algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -602,15 +602,21 @@
 
         if self.half:
             net = net.half()
 
         net = net.to(self.device)
 
         if self.ddp:
-            net_ddp = DDP(net, device_ids=[self.device],
+
+            if self.device.type == 'cuda':
+                device_ids = [self.device]
+            else:
+                device_ids = None
+
+            net_ddp = DDP(net, device_ids=device_ids,
                       find_unused_parameters=self.get_hparam('find_unused_parameters', name),
                       broadcast_buffers=self.get_hparam('broadcast_buffers', name))
 
             for a in dir(net):
                 if a not in dir(net_ddp) and not a.startswith('_'):
                     setattr(net_ddp, a, getattr(net, a))
             net = net_ddp
```

### Comparing `beam-ds-2.0.1/src/beam/config.py` & `beam-ds-2.0.2/src/beam/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,14 +182,17 @@
     parser.add_argument('--visualize-results', type=str, default='yes',
                         help='when to visualize results on tensorboard [yes|no|logscale]')
     parser.add_argument('--store-results', type=str, default='logscale',
                         help='when to store results to pickle files')
     parser.add_argument('--store-networks', type=str, default='logscale',
                         help='when to store network weights to the log directory')
 
+    parser.add_argument('--mp-context', type=str, default='spawn', help='The multiprocessing context to use')
+    parser.add_argument('--mp-backend', type=str, default=None, help='The multiprocessing backend to use')
+
     return parser
 
 
 def normalize_key(k):
     return k.replace('-', '_')
 
 def normalize_value(v):
```

### Comparing `beam-ds-2.0.1/src/beam/data.py` & `beam-ds-2.0.2/src/beam/data.py`

 * *Files identical despite different names*

### Comparing `beam-ds-2.0.1/src/beam/data_tensor.py` & `beam-ds-2.0.2/src/beam/data_tensor.py`

 * *Files identical despite different names*

### Comparing `beam-ds-2.0.1/src/beam/dataset.py` & `beam-ds-2.0.2/src/beam/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,14 +313,18 @@
                                      dynamic=dynamic, buffer_size=buffer_size,
                                      probs_normalization=probs_normalization,
                                      sample_size=sample_size)
 
     def build_dataloader(self, sampler, num_workers=0, pin_memory=None, timeout=0, collate_fn=None,
                    worker_init_fn=None, multiprocessing_context=None, generator=None, prefetch_factor=2):
 
+        kwargs = {}
+        if num_workers > 0:
+            kwargs['prefetch_factor'] = prefetch_factor
+
         try:
             d = self.device.type if self.target_device is None else self.target_device
             pin_memory_ = ('cpu' == d)
         except NotImplementedError:
             pin_memory_ = True
 
         if pin_memory is None:
@@ -330,15 +334,15 @@
 
         persistent_workers = (num_workers > 0 and sampler.once)
         prefetch_factor = prefetch_factor if num_workers > 0 else None
         return torch.utils.data.DataLoader(self, sampler=sampler, batch_size=None,
                                              num_workers=num_workers, pin_memory=pin_memory, timeout=timeout,
                                              worker_init_fn=worker_init_fn, collate_fn=collate_fn,
                                              multiprocessing_context=multiprocessing_context, generator=generator,
-                                             prefetch_factor=prefetch_factor, persistent_workers=persistent_workers)
+                                             persistent_workers=persistent_workers, **kwargs)
 
 
 class TransformedDataset(torch.utils.data.Dataset):
     def __init__(self, dataset, alg, *args, **kwargs):
         super().__init__()
 
         if type(dataset) != UniversalDataset:
```

### Comparing `beam-ds-2.0.1/src/beam/experiment.py` & `beam-ds-2.0.2/src/beam/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import torch
 import copy
 import shutil
 from collections import defaultdict
 from .utils import include_patterns, logger, check_type, beam_device, check_element_type, print_beam_hyperparameters
 import pandas as pd
 import torch.multiprocessing as mp
-from .utils import setup, cleanup, set_seed, find_free_port, check_if_port_is_available, is_notebook, find_port, \
+from .utils import setup_distributed, cleanup, set_seed, find_free_port, check_if_port_is_available, is_notebook, find_port, \
     pretty_format_number, as_numpy
 import torch.distributed as dist
 from functools import partial
 from argparse import Namespace
 from tensorboard.notebook import start as start_tensorboard
 from ._version import __version__
 import inspect
@@ -50,14 +50,16 @@
     if dataset_args is None:
         dataset_args = tuple()
     if dataset_kwargs is None:
         dataset_kwargs = dict()
 
     if inspect.isclass(Dataset):
         dataset = Dataset(experiment.hparams, *dataset_args, **dataset_kwargs)
+    elif inspect.isfunction(Dataset):
+        dataset = Dataset(experiment.hparams, *dataset_args, **dataset_kwargs)
     else:
         dataset = Dataset
 
     if inspect.isclass(Alg):
 
         ars = inspect.getfullargspec(Alg)
 
@@ -107,15 +109,19 @@
 
 
 def run_worker(rank, world_size, results_queue, job, experiment, *args, **kwargs):
 
     logger.info(f"Worker: {rank + 1}/{world_size} is running...")
 
     if world_size > 1:
-        setup(rank, world_size, port=experiment.hparams.mp_port)
+        backend = experiment.hparams.mp_backend
+        if backend is None:
+            backend = 'nccl' if experiment.hparams.device.type == 'cuda' else 'gloo'
+
+        setup_distributed(rank, world_size, port=experiment.hparams.mp_port, backend=backend)
 
     experiment.set_rank(rank, world_size)
     set_seed(seed=experiment.hparams.seed, constant=rank+1, increment=False, deterministic=experiment.hparams.deterministic)
 
     res = job(rank, world_size, experiment, *args, **kwargs)
 
     if world_size > 1:
@@ -363,16 +369,16 @@
 
         if name is not None:
             path = self.checkpoints_dir.joinpath(name)
 
         else:
 
             checkpoints = list(self.checkpoints_dir.iterdir())
-            checkpoints = [c for c in checkpoints if c.split('_')[-1].isnumeric()]
-            checkpoints_int = [int(c.split('_')[-1]) for c in checkpoints]
+            checkpoints = [c for c in checkpoints if str(c).split('_')[-1].isnumeric()]
+            checkpoints_int = [int(str(c).split('_')[-1]) for c in checkpoints]
 
             if not(len(checkpoints)):
                 logger.error(f"Directory of checkpoints does not contain valid checkpoint files")
                 return
 
             checkpoints = pd.DataFrame({'name': checkpoints}, index=checkpoints_int)
             checkpoints = checkpoints.sort_index()
@@ -794,15 +800,15 @@
             self.reload_checkpoint(alg)
 
             if reload_results:
                 results = {}
                 for subset in alg.results_dir.iterdir():
 
                     res = list(subset.iterdir())
-                    res = pd.DataFrame({'name': res, 'index': [int(c.split('_')[-1]) for c in res]})
+                    res = pd.DataFrame({'name': res, 'index': [int(str(c).split('_')[-1]) for c in res]})
                     res = res.sort_values('index')
 
                     res = res.iloc['name']
                     path = alg.results_dir.joinpath(subset, res)
                     results[subset] = path
 
                 if reload_results:
@@ -818,15 +824,15 @@
 
     def run(self, job, *args, **kwargs):
 
         arguments = (job, self, *args)
 
         def _run(demo_fn, world_size):
 
-            ctx = mp.get_context('spawn')
+            ctx = mp.get_context(self.hparams.mp_context)
             results_queue = ctx.Queue()
             for rank in range(world_size):
                 ctx.Process(target=demo_fn, args=(rank, world_size, results_queue, *arguments),
                             kwargs=kwargs).start()
 
             res = []
             for rank in range(world_size):
```

### Comparing `beam-ds-2.0.1/src/beam/model.py` & `beam-ds-2.0.2/src/beam/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,35 @@
         sin = torch.sin(2 * np.pi / self.sigma * x)
         cos = torch.cos(2 * np.pi / self.sigma * x)
 
         out = torch.cat([sin, cos], dim=-1)
         return out
 
 
+class GaussianHarmonicExpansion(object):
+
+    def __init__(self, xs, xe, delta, n=100):
+
+        self.xs = xs
+        self.xe = xe
+
+        delta = delta / (xe - xs)
+        self.b = (1 / delta) * np.random.randn(n, 2)
+
+    def transform(self, x, y):
+
+        xy = np.stack([x, y], axis=0)
+
+        xy = (xy - self.xs) / (self.xe - self.xs)
+        sin = np.sin(2 * np.pi * self.b @ xy)
+        cos = np.cos(2 * np.pi * self.b @ xy)
+
+        return np.concatenate([sin, cos], axis=0).T
+
+
 class LinearNet(nn.Module):
 
     def __init__(self, l_in, l_h=256, l_out=1, n_l=2, bias=True, activation='ReLU'):
         super().__init__()
 
         activation = getattr(nn, activation)
         self.lin = nn.Sequential(*([nn.Linear(l_in, l_h, bias=bias), activation()] if n_l > 1 else []),
```

### Comparing `beam-ds-2.0.1/src/beam/optim.py` & `beam-ds-2.0.2/src/beam/optim.py`

 * *Files identical despite different names*

### Comparing `beam-ds-2.0.1/src/beam/packed_folds.py` & `beam-ds-2.0.2/src/beam/packed_folds.py`

 * *Files identical despite different names*

### Comparing `beam-ds-2.0.1/src/beam/parallel.py` & `beam-ds-2.0.2/src/beam/parallel.py`

 * *Files identical despite different names*

### Comparing `beam-ds-2.0.1/src/beam/path.py` & `beam-ds-2.0.2/src/beam/path.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from pathlib import PurePath, Path
 import botocore
 import re
 from .utils import PureBeamPath, BeamURL
 from io import StringIO, BytesIO
 import os
+import urllib3
+urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 def beam_path(path, username=None, hostname=None, port=None, private_key=None, access_key=None, secret_key=None,
               **kwargs):
     """
 
     @param port:
@@ -224,18 +226,18 @@
         self.file_object = open(self.path, self.mode)
         return self.file_object
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.file_object.close()
 
 
-def normalize_host(hostname, port=None):
+def normalize_host(hostname, port=None, default='localhost'):
 
     if hostname is None:
-        hostname = 'localhost'
+        hostname = default
     if port is None:
         host = f"{hostname}"
     else:
         host = f"{hostname}:{port}"
 
     return host
 
@@ -343,26 +345,31 @@
         if len(self.parts) > 2:
             self.key = '/'.join(self.parts[2:])
         else:
             self.key = None
 
         protocol = 'https' if tls else 'http'
         if client is None:
-            client = boto3.resource(endpoint_url=f'{protocol}://{normalize_host(hostname, port)}',
-                                    config=boto3.session.Config(signature_version='s3v4'),
+            kwargs = {}
+            if hostname is not None:
+                kwargs['endpoint_url'] = f'{protocol}://{normalize_host(hostname, port)}'
+            client = boto3.resource(config=boto3.session.Config(signature_version='s3v4'),
                                     verify=False, service_name='s3', aws_access_key_id=access_key,
-                                    aws_secret_access_key=secret_key)
+                                    aws_secret_access_key=secret_key, **kwargs)
 
         self.client = client
         self._bucket = None
         self._object = None
 
     @property
     def bucket(self):
-        if self._bucket is None:
+
+        if self.bucket_name is None:
+            self._bucket = None
+        elif self._bucket is None:
             self._bucket = self.client.Bucket(self.bucket_name)
         return self._bucket
 
     @property
     def object(self):
         if self._object is None:
             self._object = self.client.Object(self.bucket_name, self.key)
@@ -488,15 +495,22 @@
             return None
         if not key.endswith('/'):
             key += '/'
         return key
 
     def iterdir(self):
 
+        if self.bucket is None:
+            for bucket in self.client.buckets.all():
+                yield self.gen(bucket.name)
+            return
+
         key = self.normalize_directory_key()
+        if key is None:
+            key = ''
 
         objects = self.client.meta.client.list_objects_v2(Bucket=self.bucket_name, Prefix=key, Delimiter='/')
 
         if 'CommonPrefixes' in objects:
             for prefix in objects['CommonPrefixes']:
                 path = f"{self.bucket_name}/{prefix['Prefix']}"
                 yield self.gen(path)
```

### Comparing `beam-ds-2.0.1/src/beam/processor.py` & `beam-ds-2.0.2/src/beam/processor.py`

 * *Files identical despite different names*

### Comparing `beam-ds-2.0.1/src/beam/server.py` & `beam-ds-2.0.2/src/beam/server.py`

 * *Files identical despite different names*

### Comparing `beam-ds-2.0.1/src/beam/ssl.py` & `beam-ds-2.0.2/src/beam/ssl.py`

 * *Files identical despite different names*

### Comparing `beam-ds-2.0.1/src/beam/study.py` & `beam-ds-2.0.2/src/beam/study.py`

 * *Files identical despite different names*

### Comparing `beam-ds-2.0.1/src/beam/utils.py` & `beam-ds-2.0.2/src/beam/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,15 +363,15 @@
     def is_relative_to(self, *other):
         return self.path.is_relative_to(*other)
 
     def is_reserved(self):
         return self.path.is_reserved()
 
     def joinpath(self, *other):
-        return self.gen(self.path.joinpath(*other))
+        return self.gen(self.path.joinpath(*[str(o) for o in other]))
 
     def match(self, pattern):
         return self.path.match(pattern)
 
     def relative_to(self, *other):
         other = PureBeamPath(*other)
         return PureBeamPath(self.path.relative_to(str(other)))
@@ -1351,20 +1351,20 @@
             return False  # Terminal running IPython
         else:
             return False  # Other type (?)
     except NameError:
         return False      # Probably standard Python interpreter
 
 
-def setup(rank, world_size, port='7463'):
+def setup_distributed(rank, world_size, port='7463', backend='gloo'):
     os.environ['MASTER_ADDR'] = 'localhost'
     os.environ['MASTER_PORT'] = port
 
     # initialize the process group
-    dist.init_process_group("gloo", rank=rank, world_size=world_size)
+    dist.init_process_group(backend, rank=rank, world_size=world_size)
 
 
 def cleanup(rank, world_size):
     dist.destroy_process_group()
 
 
 def set_seed(seed=-1, constant=0, increment=False, deterministic=False):
```

### Comparing `beam-ds-2.0.1/src/beam_ds.egg-info/PKG-INFO` & `beam-ds-2.0.2/src/beam_ds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beam-ds
-Version: 2.0.1
+Version: 2.0.2
 Summary: Beam Datascience package
 Home-page: https://github.com/mlutils/beamds
 Author: Beam Maintainer
 Author-email: author@example.com
 Project-URL: Bug Tracker, https://github.com/mlutils/beamds/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `beam-ds-2.0.1/src/beam_ds.egg-info/SOURCES.txt` & `beam-ds-2.0.2/src/beam_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

