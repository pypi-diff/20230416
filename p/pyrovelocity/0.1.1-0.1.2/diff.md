# Comparing `tmp/pyrovelocity-0.1.1.tar.gz` & `tmp/pyrovelocity-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrovelocity-0.1.1.tar", max compression
+gzip compressed data, was "pyrovelocity-0.1.2.tar", max compression
```

## Comparing `pyrovelocity-0.1.1.tar` & `pyrovelocity-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0    34520 2023-02-16 21:09:46.336800 pyrovelocity-0.1.1/LICENSE
--rw-r--r--   0        0        0    21225 2023-02-16 21:09:46.336800 pyrovelocity-0.1.1/README.md
--rw-r--r--   0        0        0     6832 2023-02-16 21:10:00.076558 pyrovelocity-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       20 2023-02-16 21:09:46.416799 pyrovelocity-0.1.1/pyrovelocity/__init__.py
--rw-r--r--   0        0        0    14059 2023-02-16 21:09:46.416799 pyrovelocity-0.1.1/pyrovelocity/_trainer.py
--rw-r--r--   0        0        0    11099 2023-02-16 21:09:46.416799 pyrovelocity-0.1.1/pyrovelocity/_velocity.py
--rw-r--r--   0        0        0    67045 2023-02-16 21:09:46.416799 pyrovelocity-0.1.1/pyrovelocity/_velocity_guide.py
--rw-r--r--   0        0        0    48188 2023-02-16 21:09:46.416799 pyrovelocity-0.1.1/pyrovelocity/_velocity_model.py
--rw-r--r--   0        0        0    20298 2023-02-16 21:09:46.416799 pyrovelocity-0.1.1/pyrovelocity/_velocity_module.py
--rw-r--r--   0        0        0     8804 2023-02-16 21:09:46.416799 pyrovelocity-0.1.1/pyrovelocity/api.py
--rw-r--r--   0        0        0     3253 2023-02-16 21:09:46.416799 pyrovelocity-0.1.1/pyrovelocity/config.py
--rw-r--r--   0        0        0    35592 2023-02-16 21:09:46.416799 pyrovelocity-0.1.1/pyrovelocity/cytotrace.py
--rw-r--r--   0        0        0    17866 2023-02-16 21:09:46.416799 pyrovelocity-0.1.1/pyrovelocity/data.py
--rw-r--r--   0        0        0    65126 2023-02-16 21:09:46.416799 pyrovelocity-0.1.1/pyrovelocity/plot.py
--rw-r--r--   0        0        0      215 2023-02-16 21:09:46.420799 pyrovelocity-0.1.1/pyrovelocity/pyrovelocity.py
--rw-r--r--   0        0        0    15701 2023-02-16 21:09:46.420799 pyrovelocity-0.1.1/pyrovelocity/utils.py
--rw-r--r--   0        0        0    24118 1970-01-01 00:00:00.000000 pyrovelocity-0.1.1/setup.py
--rw-r--r--   0        0        0    24712 1970-01-01 00:00:00.000000 pyrovelocity-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-04-16 15:50:07.244782 pyrovelocity-0.1.2/LICENSE
+-rw-r--r--   0        0        0    20364 2023-04-16 15:50:07.244782 pyrovelocity-0.1.2/README.md
+-rw-r--r--   0        0        0     5221 2023-04-16 15:50:20.221008 pyrovelocity-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-04-16 15:50:07.320783 pyrovelocity-0.1.2/pyrovelocity/__init__.py
+-rw-r--r--   0        0        0    15340 2023-04-16 15:50:07.320783 pyrovelocity-0.1.2/pyrovelocity/_trainer.py
+-rw-r--r--   0        0        0    22358 2023-04-16 15:50:07.320783 pyrovelocity-0.1.2/pyrovelocity/_velocity.py
+-rw-r--r--   0        0        0    67045 2023-04-16 15:50:07.320783 pyrovelocity-0.1.2/pyrovelocity/_velocity_guide.py
+-rw-r--r--   0        0        0    52597 2023-04-16 15:50:07.320783 pyrovelocity-0.1.2/pyrovelocity/_velocity_model.py
+-rw-r--r--   0        0        0     7538 2023-04-16 15:50:07.320783 pyrovelocity-0.1.2/pyrovelocity/_velocity_module.py
+-rw-r--r--   0        0        0    11280 2023-04-16 15:50:07.320783 pyrovelocity-0.1.2/pyrovelocity/api.py
+-rw-r--r--   0        0        0    13199 2023-04-16 15:50:07.320783 pyrovelocity-0.1.2/pyrovelocity/config.py
+-rw-r--r--   0        0        0    34995 2023-04-16 15:50:07.320783 pyrovelocity-0.1.2/pyrovelocity/cytotrace.py
+-rw-r--r--   0        0        0    14620 2023-04-16 15:50:07.320783 pyrovelocity-0.1.2/pyrovelocity/data.py
+-rw-r--r--   0        0        0    69379 2023-04-16 15:50:07.320783 pyrovelocity-0.1.2/pyrovelocity/plot.py
+-rw-r--r--   0        0        0      215 2023-04-16 15:50:07.320783 pyrovelocity-0.1.2/pyrovelocity/pyrovelocity.py
+-rw-r--r--   0        0        0    28164 2023-04-16 15:50:07.320783 pyrovelocity-0.1.2/pyrovelocity/utils.py
+-rw-r--r--   0        0        0    24174 1970-01-01 00:00:00.000000 pyrovelocity-0.1.2/PKG-INFO
```

### Comparing `pyrovelocity-0.1.1/LICENSE` & `pyrovelocity-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrovelocity-0.1.1/README.md` & `pyrovelocity-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,24 @@
-# pyrovelocity
+# Pyro-Velocity
 
 <div align="center">
 
 <img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/_static/logo.png" alt="Pyro-Velocity logo" width="300" role="img">
 
 |         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
 | ------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | CI/CD   | [![CI - Test](https://github.com/pinellolab/pyrovelocity/actions/workflows/tests.yml/badge.svg)](https://github.com/pinellolab/pyrovelocity/actions/workflows/tests.yml) [![CML](https://github.com/pinellolab/pyrovelocity/actions/workflows/cml.yml/badge.svg)](https://github.com/pinellolab/pyrovelocity/actions/workflows/cml.yml) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/pinellolab/pyrovelocity/master.svg)](https://results.pre-commit.ci/latest/github/pinellolab/pyrovelocity/master) |
-| Docs    | [![Documentation Status](https://readthedocs.org/projects/pyrovelocity/badge/?version=latest)](https://pyrovelocity.readthedocs.io/en/latest/?badge=latest)                                                                                                                                                                                                                                                                                                                                                                  |
-| Package | [![PyPI - Version](https://img.shields.io/pypi/v/pyrovelocity.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/pyrovelocity/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyrovelocity.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/pyrovelocity/)                                                                                                                                                                                                          |
-| Meta    | [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![License - MIT](https://img.shields.io/badge/license-AGPL%203-purple)](https://spdx.org/licenses/)                                                                                                                                                                                                                                                                                                       |
+| Docs    | [![Documentation Status](https://readthedocs.org/projects/pyrovelocity/badge/?version=latest)](https://pyrovelocity.readthedocs.io/en/latest/?badge=latest) [![Preprint](https://img.shields.io/badge/doi-10.1101/2022.09.12.507691v2-B31B1B)](https://doi.org/10.1101/2022.09.12.507691)                                                                                                                                                                                                                                    |
+| Package | [![PyPI - Version](https://img.shields.io/pypi/v/pyrovelocity.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/pyrovelocity/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyrovelocity.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/pyrovelocity/) [![Docker iamge](https://img.shields.io/badge/docker-image-blue?logo=docker)](https://github.com/pinellolab/pyrovelocity/pkgs/container/pyrovelocity)                                                    |
+| Meta    | [![codecov](https://codecov.io/gh/pinellolab/pyrovelocity/branch/master/graph/badge.svg)](https://codecov.io/gh/pinellolab/pyrovelocity) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![License - MIT](https://img.shields.io/badge/license-AGPL%203-purple)](https://spdx.org/licenses/)                                                                                                                                                              |
 
 </div>
 
 ---
 
-# Introduction
-
 `Pyro-Velocity` is a Bayesian, generative, and multivariate RNA velocity
 model to estimate _uncertainty_ in predictions of future cell states from
 minimal models approximating splicing dynamics.
 This approach models _raw sequencing counts_ with _synchronized cell time_ across
 all expressed genes to provide quantifiable information on
 cell fate choice and developmental trajectory dynamics.
 
@@ -31,83 +29,58 @@
 - Multiple uncertainty diagnostics analysis and visualizations
 - Synchronized cell time estimation across genes
 - Multivariate denoised gene expression and velocity prediction
 
 <!-- ![Velocity workflow comparison](docs/source/readme_figure1.png) -->
 <img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/source/readme_figure1.png" alt="Velocity workflow comparison">
 
-## Installation with miniconda
+## Installation
 
-Please install miniconda following the instructions here: <https://docs.conda.io/en/latest/miniconda.html>, this step takes about 1-2 mins.
+### Development
 
-```bash
-wget -c https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
-bash Miniconda3-latest-Linux-x86_64.sh
-# then follow the instruction to setup the conda base environment
-```
+We currently support installation and usage in a linux 64-bit development environment with access to a GPU.
+An [IaC](https://en.wikipedia.org/wiki/Infrastructure_as_code) setup that works with [GCP](https://registry.terraform.io/providers/hashicorp/google/latest/docs) is documented in [reproducibility/environment/README.md](reproducibility/environment/README.md).
+Before proceeding to setup a minimal development environment, please fork this repository and clone a copy of your fork to your development machine. Unless otherwise mentioned, all commands assume your current working directory is the root of your local copy of your fork of this repository.
 
-After the conda has been setup, logout and re-login to install _mamba_ to speed up installation, this step takes about 20s.
-
-```bash
-conda install -c conda-forge mamba
-```
-
-Then add the channels, this step takes 1~2s.
-
-```bash
-conda config --add channels defaults
-conda config --add channels bioconda
-conda config --add channels conda-forge
-conda config --set channel_priority flexible
-```
+Please install mambaforge according to the instructions provided in [conda-forge/miniforge](https://github.com/conda-forge/miniforge#install).
 
-After that, install the _pyrovelocity_ package in one mamba command:
+You can then create a development environment with
 
 ```bash
-mamba create -n pyrovelocity_bioconda -c bioconda pyrovelocity
+mamba env create [--prefix /path_to_conda_environment] -f conda/environment-gpu.yml
 ```
 
-This step takes about 6-8 minutes depending on the network speed. If you prefer to use conda environment configurations, see the `conda` subfolder for installation with _prefix_ to specify the installation path, such as:
+This step takes about 10 minutes depending on network speed.
 
-```
-# GPU
-mamba env create --prefix /path_to_conda_env/qq-pyrovelocity-dev -f conda/environment-gpu.yml
-# or CPU
-mamba env create --prefix /path_to_conda_env/qq-pyrovelocity-dev -f conda/environment-cpu.yml
-```
-
-Or with more control of installing the environment,
+Make sure you are able to successfully activate the installed environment
 
 ```bash
-conda create -n pyrovelocity_bioconda python=3.8.8
-mamba install -n pyrovelocity_bioconda -c bioconda pyrovelocity
-# CPU
-mamba env update -n pyrovelocity_bioconda -f conda/environment-cpu.yml
-# or GPU
-mamba env update -n pyrovelocity_bioconda -f conda/environment-gpu.yml
+conda activate pyrovelocity-gpu
+which python
 ```
 
-For windows user installation, please refer to the [issue](https://github.com/pinellolab/pyrovelocity/issues/9).
+by checking that the output of which python following activation refers to the python binary in the correct conda environment.
 
-Lastly, test the installation by:
+You can then install a development copy with
 
-```bash
-conda activate pyrovelocity_bioconda
-python
 ```
+pip install --no-deps -e .[dev]
+```
+
+If this is successful, you will be able to
 
 ```python
 import pyrovelocity
 ```
 
-## Additional packages necessary to reproduce all the analyses presented in the notebooks
+from a python interpreter.
 
-```bash
-pip install cospar==0.1.9
-```
+### User
+
+Please see the [documentation](https://pyrovelocity.readthedocs.io/en/latest/installation.html).
 
 ## Quick start
 
 After the installation, let\'s look at your dataset to see how
 Pyro-Velocity can help understand cell dynamics.
 
 Starting from raw sequencing FASTQ files, obtained for example with
@@ -176,20 +149,20 @@
                                guide_type='auto',
                                train_size=1.0)
 
 # adata_model_pos is a returned list in which 0th element is the trained model,
 # the 1st element is the posterior samples of all random variables
 save_res = True
 if save_res:
-    adata_model_pos[0].save('saved_model', overwrite=True)
-    result_dict = {"adata_model_pos": adata_model_pos[1],
+    trained_model.save('saved_model', overwrite=True)
+    result_dict = {"adata_model_pos": posterior_samples,
                    "v_map_all": v_map_all,
                    "embeds_radian": embeds_radian, "fdri": fdri, "embed_mean": embed_mean}
     import pickle
-    with open("model_posterior_samples.pkl", "wb") as f:
+    with open("posterior_samples.pkl", "wb") as f:
          pickle.dump(result_dict, f)
 ```
 
 Step 4: Generate Pyro-Velocity's vector field and shared time plots
 with uncertainty estimation.
 
 ```python
@@ -199,32 +172,32 @@
       plot_mean_vector_field, project_grid_points,rainbowplot,denoised_umap,\
       us_rainbowplot, plot_arrow_examples
 
 embedding = 'emb' # change to umap or tsne based on your embedding method
 
 # This generates the posterior samples of all vector fields
 # and statistical testing results from Rayleigh test
-v_map_all, embeds_radian, fdri = vector_field_uncertainty(adata, adata_model_pos[1],
+v_map_all, embeds_radian, fdri = vector_field_uncertainty(adata, posterior_samples,
                                                           basis=embedding, denoised=False, n_jobs=30)
 fig, ax = plt.subplots()
 # This returns the posterior mean of the vector field
-embed_mean = plot_mean_vector_field(adata_model_pos[1], adata, ax=ax, n_jobs=30, basis=embedding)
+embed_mean = plot_mean_vector_field(posterior_samples, adata, ax=ax, n_jobs=30, basis=embedding)
 # This plot single-cell level vector field uncertainty
 # and averaged cell vector field uncertainty on the grid points
 # based on angular standard deviation
 fig, ax = plt.subplots(1, 2)
 fig.set_size_inches(11.5, 5)
 plot_vector_field_uncertain(adata, embed_mean, embeds_radian,
                             ax=ax,
                             fig=fig, cbar=False, basis=embedding, scale=None)
 
 # This generates shared time uncertainty plot with contour lines
 fig, ax = plt.subplots(1, 3)
 fig.set_size_inches(12, 2.8)
-adata.obs['shared_time_uncertain'] = adata_model_pos[1]['cell_time'].std(0).flatten()
+adata.obs['shared_time_uncertain'] = posterior_samples['cell_time'].std(0).flatten()
 ax_cb = scv.pl.scatter(adata, c='shared_time_uncertain', ax=ax[0], show=False, cmap='inferno', fontsize=7, s=20, colorbar=True, basis=embedding)
 select = adata.obs['shared_time_uncertain'] > np.quantile(adata.obs['shared_time_uncertain'], 0.9)
 sns.kdeplot(adata.obsm[f'X_{embedding}'][:, 0][select],
             adata.obsm[f'X_{embedding}'][:, 1][select],
             ax=ax[0], levels=3, fill=False)
 
 # This generates vector field uncertainty based on Rayleigh test.
@@ -247,24 +220,26 @@
 one with rainbow plots
 
 ```python
 fig = plt.figure(figsize=(7.07, 4.5))
 subfig = fig.subfigures(1, 2, wspace=0.0, hspace=0, width_ratios=[1.6, 4])
 ax = fig.subplots(1)
 # This generates the selected cell fate markers and output in DataFrame
-volcano_data, _ = plot_gene_ranking([adata_model_pos[1]], [adata], ax=ax,
+volcano_data, _ = plot_gene_ranking([posterior_samples], [adata], ax=ax,
                                      time_correlation_with='st', assemble=True)
 # This generates the rainbow plots for the selected markers.
-_ = rainbowplot(volcano_data, adata, adata_model_pos[1],
+_ = rainbowplot(volcano_data, adata, posterior_samples,
                 subfig[1], data=['st', 'ut'], num_genes=4)
 ```
 
 ## Illustrative examples of Pyro-Velocity analyses on different single-cell datasets
 
-### Pyro-Velocity applied to a PBMC dataset \[[1](https://scvelo.readthedocs.io/perspectives/Perspectives/)\]
+### Pyro-Velocity applied to a PBMC dataset
+
+See the [data referred to here](https://scvelo.readthedocs.io/en/stable/perspectives/Perspectives/).
 
 This is a scRNA-seq dataset of fully mature peripheral blood mononuclear
 cells (PBMC) generated using the 10X genomics kit and containing 65,877
 cells with 11 fully differentiated immune cell types. This dataset
 doesn\'t contain stem and progenitor cells or other signature of and
 undergoing dynamical differentiation, thus no consistent velocity flow
 should be detected.
@@ -288,15 +263,17 @@
 Rayleigh test of posterior samples vector field, the title shows the
 expected false discovery rate using a 5% threshold.
 
 The full example can be reproduced using the
 [PBMC](https://github.com/pinellolab/pyrovelocity/blob/master/docs/source/notebooks/pbmc.ipynb)
 Jupyter notebook.
 
-### Pyro-Velocity applied to a pancreas development dataset \[[2](https://scvelo.readthedocs.io/VelocityBasics/)\]
+### Pyro-Velocity applied to a pancreas development dataset
+
+See the [data referred to here](https://scvelo.readthedocs.io/en/stable/VelocityBasics/).
 
 Here we apply Pyro-Velocity to a single cell RNA-seq dataset of mouse
 pancreas in the E15.5 embryo developmental stage. This dataset was
 generated using the 10X genomics kit and contains 3,696 cells with 8
 cell types including progenitor cells, intermediate and terminal cell
 states.
 
@@ -344,15 +321,17 @@
 <!-- ![Pancreas vector field uncertainty](docs/source/readme_figure7.png) -->
 <img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/source/readme_figure7.png" alt="Pancreas vector field uncertainty">
 
 The full example can be reproduced using the
 [Pancreas](https://github.com/pinellolab/pyrovelocity/blob/master/docs/source/notebooks/pancreas.ipynb)
 jupyter notebook.
 
-### Pyro-Velocity applied to the LARRY dataset \[[3](https://figshare.com/articles/dataset/larry_invitro_adata_sub_raw_h5ad/20780344)\]
+### Pyro-Velocity applied to the LARRY dataset
+
+See the [data referred to here](https://figshare.com/articles/dataset/larry_invitro_adata_sub_raw_h5ad/20780344).
 
 This last example, present the analysis of a recent scRNA-seq dataset
 profiling mouse hematopoises at high resolution thanks to lineage
 relationship information captured by the Lineage And RNA RecoverY
 (LARRY) system. LARRY leverages unique lentiviral barcodes that enables
 to clonally trace cell fates over time (Weinrab et al. Cell 20).
 
@@ -391,34 +370,11 @@
 
 The full example can be reproduced using the
 [LARRY](https://github.com/pinellolab/pyrovelocity/blob/master/docs/source/notebooks/larry.ipynb)
 jupyter notebook.
 
 # Troubleshooting
 
-## TypeError: fate_potency() got an unexpected keyword argument 'used_Tmap'
-
-Please use the specific _cospar_ version:
-
-```bash
-pip install cospar==0.1.9
-```
-
-## CUDA error: no kernel image is available for execution on the device
-
-All reference to GPU support applies to linux. We do not currently support windows
-and there is no GPU-compatible pytorch version `<1.12` for darwin.
-On linux, either use [conda](./conda) (as exemplified in
-[reproducibility/environment](./reproducibility/environment)),
-or install the specific cuda-enabled pytorch version manually
-
-```bash
-pip3 install torch==1.8.1+cu111 -f https://download.pytorch.org/whl/torch_stable.html
-```
-
-If you are using poetry, you can also use the poetry helper
-
-```bash
-poetry install && poetry run poe force-cuda11
-```
+If you are having an issue using pyrovelocity, please feel free to [start a discussion](https://github.com/pinellolab/pyrovelocity/discussions)
+or [file an issue](https://github.com/pinellolab/pyrovelocity/issues) containing a [MRE](https://en.wikipedia.org/wiki/Minimal_reproducible_example).
 
 Also see [contributing](./docs/contributing.md).
```

### Comparing `pyrovelocity-0.1.1/pyrovelocity/_trainer.py` & `pyrovelocity-0.1.2/pyrovelocity/_trainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Optional
 from typing import Sequence
 from typing import Union
 
 import mlflow
 import numpy as np
 import pyro
+import scipy
 import torch
 from pyro.infer import TraceEnum_ELBO
 from pyro.infer.autoguide.guides import AutoGuideList
 from pyro.optim.clipped_adam import ClippedAdam
 from pyro.optim.optim import PyroOptim
 from scvi.dataloaders import DataSplitter
 from scvi.train import PyroTrainingPlan
@@ -83,16 +84,16 @@
         pyro_velocity: VelocityModule,
         optim: Optional[pyro.optim.PyroOptim] = None,
     ):
         super().__init__(
             pyro_velocity, TraceEnum_ELBO(strict_enumeration_warning=True), optim
         )
         self.svi = pyro.infer.SVI(
-            model=self.pyro_model,
-            guide=self.pyro_guide,
+            model=self.module.model,
+            guide=self.module.guide,
             optim=self.optim,
             loss=self.loss_fn,
         )
         self.n_elem = self.module.num_genes * self.module.num_cells * 2
 
     def training_step(self, batch, batch_idx, optimizer_idx=0):
         args, kwargs = self.module._get_fn_args_from_batch(batch)
@@ -150,16 +151,17 @@
         patience: int = 10,
         min_delta: float = 0.0,
         **kwargs,
     ):
         print("base train function")
         pyro.clear_param_store()
         pyro.set_rng_seed(seed)
+
         data_splitter = DataSplitter(
-            self.adata,
+            self.adata_manager,
             train_size=train_size,
             validation_size=valid_size,
             batch_size=batch_size,
             use_gpu=use_gpu,
         )
         training_plan = EnumTrainingPlan(
             self.module, VelocityClippedAdam({"lr": lr, "lrd": 0.9999})
@@ -208,43 +210,78 @@
             self.module._guide,
             optim,
             TraceEnum_ELBO(strict_enumeration_warning=True),
         )
 
         normalizer = self.adata.shape[0] * self.adata.shape[1] * 2
         u = torch.tensor(
-            np.array(self.adata.layers["raw_unspliced"].toarray(), dtype="float32"),
+            np.array(self.adata.layers["raw_unspliced"].toarray(), dtype="float32")
+            if scipy.sparse.issparse(self.adata.layers["raw_unspliced"])
+            else self.adata.layers["raw_unspliced"],
             dtype=torch.float32,
         ).to(device)
         s = torch.tensor(
-            np.array(self.adata.layers["raw_spliced"].toarray(), dtype="float32"),
+            np.array(self.adata.layers["raw_spliced"].toarray(), dtype="float32")
+            if scipy.sparse.issparse(self.adata.layers["raw_spliced"])
+            else self.adata.layers["raw_spliced"],
             dtype=torch.float32,
         ).to(device)
+
+        epsilon = 1e-6
+
         u_library = torch.tensor(
-            np.array(self.adata.obs.u_lib_size, dtype="float32"), dtype=torch.float32
-        ).to(device)
-        s_library = torch.tensor(
-            np.array(self.adata.obs.s_lib_size, dtype="float32"), dtype=torch.float32
-        ).to(device)
-        u_library_mean = torch.tensor(
-            np.array(self.adata.obs.u_lib_size_mean, dtype="float32"),
-            dtype=torch.float32,
-        ).to(device)
-        s_library_mean = torch.tensor(
-            np.array(self.adata.obs.s_lib_size_mean, dtype="float32"),
-            dtype=torch.float32,
-        ).to(device)
-        u_library_scale = torch.tensor(
-            np.array(self.adata.obs.u_lib_size_scale, dtype="float32"),
+            # np.array(self.adata.obs.u_lib_size, dtype="float32"), dtype=torch.float32
+            np.array(np.log(self.adata.obs.u_lib_size_raw + epsilon), dtype="float32"),
             dtype=torch.float32,
         ).to(device)
-        s_library_scale = torch.tensor(
-            np.array(self.adata.obs.s_lib_size_scale, dtype="float32"),
+        s_library = torch.tensor(
+            # np.array(self.adata.obs.s_lib_size, dtype="float32"), dtype=torch.float32
+            np.array(np.log(self.adata.obs.s_lib_size_raw + epsilon), dtype="float32"),
             dtype=torch.float32,
         ).to(device)
+        u_library_mean = (
+            torch.tensor(
+                # np.array(self.adata.obs.u_lib_size_mean, dtype="float32"),
+                np.mean(np.log(self.adata.obs.u_lib_size_raw + epsilon)),
+                dtype=torch.float32,
+            )
+            .expand(u_library.shape)
+            .to(device)
+        )
+        s_library_mean = (
+            torch.tensor(
+                # np.array(self.adata.obs.s_lib_size_mean, dtype="float32"),
+                np.mean(np.log(self.adata.obs.s_lib_size_raw + epsilon)),
+                dtype=torch.float32,
+            )
+            .expand(u_library.shape)
+            .to(device)
+        )
+        u_library_scale = (
+            torch.tensor(
+                # np.array(self.adata.obs.u_lib_size_scale, dtype="float32"),
+                np.std(np.log(self.adata.obs.u_lib_size_raw + epsilon)),
+                dtype=torch.float32,
+            )
+            .expand(u_library.shape)
+            .to(device)
+        )
+        s_library_scale = (
+            torch.tensor(
+                # np.array(self.adata.obs.s_lib_size_scale, dtype="float32"),
+                np.std(np.log(self.adata.obs.s_lib_size_raw + epsilon)),
+                dtype=torch.float32,
+            )
+            .expand(u_library.shape)
+            .to(device)
+        )
+
+        print(u_library_scale.shape)
+        print(u.shape)
+        print(u_library.shape)
         if "pyro_cell_state" in self.adata.obs.columns:
             cell_state = torch.tensor(
                 np.array(self.adata.obs.pyro_cell_state, dtype="float32"),
                 dtype=torch.float32,
             ).to(device)
         else:
             cell_state = None
```

### Comparing `pyrovelocity-0.1.1/pyrovelocity/_velocity_guide.py` & `pyrovelocity-0.1.2/pyrovelocity/_velocity_guide.py`

 * *Files identical despite different names*

### Comparing `pyrovelocity-0.1.1/pyrovelocity/_velocity_model.py` & `pyrovelocity-0.1.2/pyrovelocity/_velocity_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Optional
 from typing import Tuple
 from typing import Union
 
 import pyro
 import pyro.poutine as poutine
 import torch
+from packaging import version
 from pyro.distributions import Bernoulli
 from pyro.distributions import Beta
 from pyro.distributions import LogNormal
 from pyro.distributions import NegativeBinomial
 from pyro.distributions import Normal
 from pyro.distributions import Poisson
 from pyro.distributions.constraints import positive
@@ -25,27 +26,56 @@
 from torch.nn.functional import softplus
 
 from .utils import mRNA
 from .utils import tau_inv
 
 
 class LogNormalModel(PyroModule):
+    """
+    A base class for pyrovelocity models.
+
+    This class serves as the base class for constructing a pyrovelocity model.
+    It provides basic methods for handling gene expression data, such as creating plates
+    for cells and genes, encoding cell-specific features, and computing the likelihood
+    of the observed data.
+
+    Attributes:
+        num_cells (int): The number of cells.
+        num_genes (int): The number of genes.
+        likelihood (str): The likelihood type for the model, defaults to "Poisson".
+        plate_size (int): The size of the plate for the model, defaults to 2.
+
+    Example:
+        >>> from pyrovelocity._velocity_model import LogNormalModel
+        >>> num_cells = 10
+        >>> num_genes = 20
+        >>> likelihood = "Poisson"
+        >>> plate_size = 2
+        >>> model = LogNormalModel(num_cells, num_genes, likelihood, plate_size)
+        >>> assert model.num_cells == num_cells
+        >>> assert model.num_genes == num_genes
+        >>> assert model.likelihood == likelihood
+        >>> assert model.plate_size == plate_size
+    """
+
     def __init__(
         self,
         num_cells: int,
         num_genes: int,
         likelihood: str = "Poisson",
         plate_size: int = 2,
+        correct_library_size: Union[bool, str] = True,
     ) -> None:
         assert num_cells > 0 and num_genes > 0
         super().__init__()
         self.num_cells = num_cells
         self.num_genes = num_genes
         self.n_obs = None
         self.plate_size = plate_size
+        self.correct_library_size = correct_library_size
         self.register_buffer("zero", torch.tensor(0.0))
         self.register_buffer("one", torch.tensor(1.0))
 
         self.likelihood = likelihood
         if self.likelihood == "NB":
             self.u_px_r = PyroParam(
                 torch.ones(self.num_genes), constraint=positive, event_dim=0
@@ -167,43 +197,36 @@
             .mask(False)
         )
 
     @PyroSample
     def dt_switching(self):
         if self.plate_size == 2:
             return LogNormal(self.zero, self.one)
-            # return Normal(self.zero, self.one)
         return (
             LogNormal(self.zero, self.one * 0.1)
             .expand((self.num_genes,))
             .to_event(1)
             .mask(False)
         )
 
     @PyroSample
     def latent_time(self):
         if self.shared_time:
             if self.plate_size == 2:
-                return Normal(self.zero, self.one * 0.1).mask(
-                    self.include_prior
-                )  # with shared cell_time
+                return Normal(self.zero, self.one * 0.1).mask(self.include_prior)
             else:
                 return (
                     Normal(self.zero, self.one * 0.1)
                     .expand((self.num_genes,))
                     .to_event(1)
                     .mask(self.include_prior)
-                )  # with shared cell_time
+                )
         if self.plate_size == 2:
-            return LogNormal(self.zero, self.one).mask(
-                self.include_prior
-            )  # without shared cell_time
-        return (
-            LogNormal(self.zero, self.one).expand((self.num_genes,)).to_event(1)
-        )  # .mask(False) # without shared cell_time
+            return LogNormal(self.zero, self.one).mask(self.include_prior)
+        return LogNormal(self.zero, self.one).expand((self.num_genes,)).to_event(1)
 
     @PyroSample
     def cell_time(self):
         if self.plate_size == 2 and self.shared_time:
             return Normal(self.zero, self.one)
         else:
             return LogNormal(self.zero, self.one)
@@ -285,27 +308,60 @@
         u_read_depth: Optional[torch.Tensor] = None,
         s_read_depth: Optional[torch.Tensor] = None,
         u_cell_size_coef: None = None,
         ut_coef: None = None,
         s_cell_size_coef: None = None,
         st_coef: None = None,
     ) -> Tuple[Poisson, Poisson]:
-        ##if not (self.likelihood in ['Normal', 'LogNormal']): # and u_scale is None and s_scale is None:
-        ##    ut = pyro.sample("ut", Normal(ut, u_scale))
-        ##    st = pyro.sample("st", Normal(st, s_scale))
+        """
+        Compute the likelihood of the given count data.
+
+        Args:
+            ut (torch.Tensor): Tensor representing unspliced transcripts.
+            st (torch.Tensor): Tensor representing spliced transcripts.
+            u_log_library (Optional[torch.Tensor], optional): Log library tensor for unspliced transcripts. Defaults to None.
+            s_log_library (Optional[torch.Tensor], optional): Log library tensor for spliced transcripts. Defaults to None.
+            u_scale (Optional[torch.Tensor], optional): Scale tensor for unspliced transcripts. Defaults to None.
+            s_scale (Optional[torch.Tensor], optional): Scale tensor for spliced transcripts. Defaults to None.
+            u_read_depth (Optional[torch.Tensor], optional): Read depth tensor for unspliced transcripts. Defaults to None.
+            s_read_depth (Optional[torch.Tensor], optional): Read depth tensor for spliced transcripts. Defaults to None.
+            u_cell_size_coef (Optional[Any], optional): Cell size coefficient for unspliced transcripts. Defaults to None.
+            ut_coef (Optional[Any], optional): Coefficient for unspliced transcripts. Defaults to None.
+            s_cell_size_coef (Optional[Any], optional): Cell size coefficient for spliced transcripts. Defaults to None.
+            st_coef (Optional[Any], optional): Coefficient for spliced transcripts. Defaults to None.
+
+        Returns:
+            Tuple[Poisson, Poisson]: A tuple of Poisson distributions for unspliced and spliced transcripts, respectively.
+
+        Example:
+            >>> import torch
+            >>> from pyro.nn import PyroModule
+            >>> num_cells = 10
+            >>> num_genes = 20
+            >>> likelihood = "Poisson"
+            >>> plate_size = 2
+            >>> model = LogNormalModel(num_cells, num_genes, likelihood, plate_size)
+            >>> ut = torch.rand(num_cells, num_genes)
+            >>> st = torch.rand(num_cells, num_genes)
+            >>> u_read_depth = torch.rand(num_cells, 1)
+            >>> s_read_depth = torch.rand(num_cells, 1)
+            >>> u_dist, s_dist = model.get_likelihood(ut, st, u_read_depth=u_read_depth, s_read_depth=s_read_depth)
+            >>> assert isinstance(u_dist, torch.distributions.Poisson)
+            >>> assert isinstance(s_dist, torch.distributions.Poisson)
+        """
         if self.likelihood == "NB":
             if self.correct_library_size:
                 ut = relu(ut) + self.one * 1e-6
                 st = relu(st) + self.one * 1e-6
                 ut = pyro.deterministic("ut", ut, event_dim=0)
                 st = pyro.deterministic("st", st, event_dim=0)
                 if self.guide_type not in [
                     "velocity_auto",
                     "velocity_auto_depth",
-                ]:  # time is learned from scaled u_obs/s_obs, no need to scale
+                ]:
                     ut = ut / torch.sum(ut, dim=-1, keepdim=True)
                     st = st / torch.sum(st, dim=-1, keepdim=True)
                 ut = pyro.deterministic("ut_norm", ut, event_dim=0)
                 st = pyro.deterministic("st_norm", st, event_dim=0)
                 u_logits = ((ut + self.one * 1e-6) * u_read_depth).log() - (
                     self.u_px_r.exp() + self.one * 1e-6
                 ).log()
@@ -327,24 +383,15 @@
             s_dist = NegativeBinomial(total_count=self.s_px_r.exp(), logits=s_logits)
         elif self.likelihood == "Poisson":
             if self.correct_library_size:
                 ut = relu(ut) + self.one * 1e-6
                 st = relu(st) + self.one * 1e-6
                 ut = pyro.deterministic("ut", ut, event_dim=0)
                 st = pyro.deterministic("st", st, event_dim=0)
-                ##if not (self.guide_type in ['velocity_auto', 'velocity_auto_depth']): # time is learned from scaled u_obs/s_obs, no need to scale
                 if self.correct_library_size == "cell_size_regress":
-                    ##ut = relu(self.one * u_read_depth + ut * ut_coef + u_cell_size_coef)+self.one*1e-6
-                    ##st = relu(self.one * s_read_depth + st * st_coef + s_cell_size_coef)+self.one*1e-6
-                    ##ut = relu(self.one * u_read_depth + ut * ut_coef)+self.one*1e-6
-                    ##st = relu(self.one * s_read_depth + st * st_coef)+self.one*1e-6
-                    ##ut = torch.exp(relu(self.one * u_read_depth + ut * ut_coef + u_cell_size_coef)+self.one*1e-6)
-                    ##st = torch.exp(relu(self.one * s_read_depth + st * st_coef + s_cell_size_coef)+self.one*1e-6)
-                    ##ut = torch.exp(self.one * u_read_depth + u_cell_size_coef)
-                    ##st = torch.exp(self.one * s_read_depth + s_cell_size_coef)
                     ut_sum = torch.log(torch.sum(ut, dim=-1, keepdim=True))
                     st_sum = torch.log(torch.sum(st, dim=-1, keepdim=True))
                     ut = torch.log(ut)
                     st = torch.log(st)
                     ut = torch.exp(
                         ut_coef * ut + u_cell_size_coef * (-ut_sum + u_read_depth)
                     )
@@ -368,33 +415,25 @@
                 ut = ut + self.one * 1e-6
                 st = st + self.one * 1e-6
 
             u_dist = Poisson(ut)
             s_dist = Poisson(st)
         elif self.likelihood == "Normal":
             if u_scale is not None and s_scale is not None:
-                u_dist = Normal(
-                    ut, u_scale
-                )  # NOTE: add scale parameters significantly decrease ELBO
+                u_dist = Normal(ut, u_scale)
                 s_dist = Normal(st, s_scale)
             else:
-                u_dist = Normal(
-                    ut, self.one * 0.1
-                )  # NOTE: add scale parameters significantly decrease ELBO
+                u_dist = Normal(ut, self.one * 0.1)
                 s_dist = Normal(st, self.one * 0.1)
         elif self.likelihood == "LogNormal":
             if u_scale is not None and s_scale is not None:
-                u_dist = LogNormal(
-                    (ut + self.one * 1e-6).log(), u_scale
-                )  # NOTE: add scale parameters significantly decrease ELBO
+                u_dist = LogNormal((ut + self.one * 1e-6).log(), u_scale)
                 s_dist = LogNormal((st + self.one * 1e-6).log(), s_scale)
             else:
-                u_dist = LogNormal(
-                    ut, self.one * 0.1
-                )  # NOTE: add scale parameters significantly decrease ELBO
+                u_dist = LogNormal(ut, self.one * 0.1)
                 s_dist = LogNormal(st, self.one * 0.1)
         else:
             raise
         return u_dist, s_dist
 
 
 class VelocityModel(LogNormalModel):
@@ -416,14 +455,57 @@
         add_offset: bool = False,
         correct_library_size: Union[bool, str] = True,
         guide_type: bool = "velocity",
         cell_specific_kinetics: Optional[str] = None,
         kinetics_num: Optional[int] = None,
         **initial_values,
     ) -> None:
+        """
+        Derived class for modeling RNA velocity with shared latent time.
+
+        Inherits from LogNormalModel.
+
+        Args:
+            num_cells (int): Number of cells.
+            num_genes (int): Number of genes.
+            likelihood (str, optional): Likelihood model. Defaults to "Poisson".
+            shared_time (bool, optional): Whether to share time across cells. Defaults to True.
+            t_scale_on (bool, optional): Whether to scale the time. Defaults to False.
+            plate_size (int, optional): The number of dimensions for the plates. Defaults to 2.
+            latent_factor (str, optional): Latent factor type. Defaults to "none".
+            latent_factor_size (int, optional): Latent factor size. Defaults to 30.
+            latent_factor_operation (str, optional): Latent factor operation. Defaults to "selection".
+            include_prior (bool, optional): Whether to include prior. Defaults to False.
+            num_aux_cells (int, optional): Number of auxiliary cells. Defaults to 100.
+            only_cell_times (bool, optional): Whether to use only cell times. Defaults to False.
+            decoder_on (bool, optional): Whether to use a decoder. Defaults to False.
+            add_offset (bool, optional): Whether to add an offset. Defaults to False.
+            correct_library_size (Union[bool, str], optional): Whether to correct library size. Defaults to True.
+            guide_type (bool, optional): Guide type for the model. Defaults to "velocity".
+            cell_specific_kinetics (Optional[str], optional): Cell-specific kinetics. Defaults to None.
+            kinetics_num (Optional[int], optional): Number of kinetics. Defaults to None.
+            **initial_values: Initial values for various parameters in the model.
+
+        Example:
+            >>> import torch
+            >>> from pyro.nn import PyroModule
+            >>> num_cells = 10
+            >>> num_genes = 20
+            >>> likelihood = "Poisson"
+            >>> plate_size = 2
+            >>> model = VelocityModel(num_cells, num_genes, likelihood, plate_size)
+            >>> u_obs = torch.rand(num_cells, num_genes)
+            >>> s_obs = torch.rand(num_cells, num_genes)
+            >>> u_log_library = torch.rand(num_cells, 1)
+            >>> s_log_library = torch.rand(num_cells, 1)
+            >>> ind_x = torch.randint(0, num_cells, (num_cells,))
+            >>> # ut, st = model.model(u_obs, s_obs, u_log_library, s_log_library, ind_x)
+            >>> # assert ut.shape == (num_cells, num_genes)
+            >>> # assert st.shape == (num_cells, num_genes)
+        """
         assert num_cells > 0 and num_genes > 0
         super().__init__(num_cells, num_genes, likelihood, plate_size)
         # TODO set self.num_aux_cells in self.__init__, 10-200
         self.num_aux_cells = num_aux_cells
         self.num_aux_cells = num_aux_cells
         self.only_cell_times = only_cell_times
         self.guide_type = guide_type
@@ -446,342 +528,167 @@
         self.latent_factor_operation = latent_factor_operation
         self.include_prior = include_prior
         self.decoder_on = decoder_on
         self.correct_library_size = correct_library_size
         if self.decoder_on:
             self.decoder = Decoder(1, self.num_genes, n_layers=2)
 
-    def model(
-        self,
-        u_obs: Optional[torch.Tensor] = None,
-        s_obs: Optional[torch.Tensor] = None,
-        u_log_library: Optional[torch.Tensor] = None,
-        s_log_library: Optional[torch.Tensor] = None,
-        ind_x: Optional[torch.Tensor] = None,
-    ) -> Tuple[torch.Tensor, torch.Tensor]:
-        """max plate = 2 with cell and gene plate"""
-        cell_plate, gene_plate = self.create_plates(
-            u_obs, s_obs, u_log_library, s_log_library, ind_x
-        )
-
-        with gene_plate, poutine.mask(mask=self.include_prior):
-            alpha = self.alpha
-            beta = self.beta
-            gamma = self.gamma
-            switching = self.switching
-            u_scale = self.u_scale  # if self.likelihood == 'Normal' else None
-            s_scale = self.s_scale  # if self.likelihood == 'Normal' else None
-            ##u_inf = self.u_inf
-            ##s_inf = self.s_inf
-            ##switching = tau_inv(u_inf, s_inf, self.zero, self.zero, alpha, beta, gamma)
-            ##switching = pyro.sample("switching", Normal(switching, self.one*0.1))
-            if self.t_scale_on and self.shared_time:
-                t_scale = self.t_scale
-            if self.latent_factor_operation == "selection":
-                p_velocity = self.p_velocity
-
-            # if self.latent_factor_operation == 'selection':
-            #    velocity_genecellpair = pyro.sample("genecellpair_type", Bernoulli(self.one))
-            if self.latent_factor == "linear":
-                u_pcs_mean = pyro.sample("u_pcs_mean", Normal(self.zero, self.one))
-                s_pcs_mean = pyro.sample("s_pcs_mean", Normal(self.zero, self.one))
-            u_inf, s_inf = mRNA(switching, self.zero, self.zero, alpha, beta, gamma)
-            # u_inf = pyro.sample("u_inf", Normal(u_inf, u_scale))
-            # s_inf = pyro.sample("s_inf", Normal(s_inf, s_scale))
-
-        if self.latent_factor == "linear":
-            cell_codebook = self.cell_codebook
-            with cell_plate, poutine.mask(mask=False):
-                cell_code = self.cell_code
-        if self.shared_time:
-            with cell_plate:
-                cell_time = self.cell_time
-
-        # if self.likelihood in ["NB", "Poisson"]:
-        #     # with cell_plate:
-        #     #    u_read_depth = pyro.sample('u_read_depth', dist.LogNormal(u_log_library, self.one))
-        #     #    s_read_depth = pyro.sample('s_read_depth', dist.LogNormal(s_log_library, self.one))
-        #     u_read_depth = None
-        #     s_read_depth = None
-        # else:
-        #     u_read_depth = None
-        #     s_read_depth = None
-        u_read_depth = None
-        s_read_depth = None
-
-        with cell_plate, gene_plate, poutine.mask(
-            mask=pyro.subsample(self.mask.to(alpha.device), event_dim=0)
-        ):
-            t = self.latent_time
-            if self.shared_time:
-                t = cell_time * t_scale + t if self.t_scale_on else cell_time + t
-            state = (
-                pyro.sample("cell_gene_state", Bernoulli(logits=t - switching))
-                == self.zero
-            )
-            u0_vec = torch.where(state, self.zero, u_inf)
-            s0_vec = torch.where(state, self.zero, s_inf)
-            alpha_vec = torch.where(state, alpha, self.zero)
-            # tau = softplus(torch.where(state, t, t - switching))
-            tau = relu(torch.where(state, t, t - switching))
-            ut, st = mRNA(tau, u0_vec, s0_vec, alpha_vec, beta, gamma)
-            if self.latent_factor_operation == "selection":
-                velocity_genecellpair = pyro.sample(
-                    "genecellpair_type", Bernoulli(p_velocity)
-                )
-            if self.latent_factor == "linear":
-                regressor_output = torch.einsum(
-                    "abc,cd->ad", cell_code, cell_codebook.squeeze()
-                )
-                regressor_u = softplus(
-                    regressor_output[..., : self.num_genes].squeeze() + u_pcs_mean
-                )
-                regressor_s = softplus(
-                    regressor_output[..., self.num_genes :].squeeze() + s_pcs_mean
-                )
-            if self.latent_factor_operation == "selection":
-                ut = torch.where(
-                    velocity_genecellpair == self.one,
-                    (ut * u_scale / s_scale),
-                    softplus(regressor_u),
-                )
-                st = torch.where(
-                    velocity_genecellpair == self.one, st, softplus(regressor_s)
-                )
-            elif self.latent_factor_operation == "sum":
-                ut = ut * u_scale / s_scale + regressor_u
-                st = st + regressor_s
-            else:
-                ut = ut * u_scale / s_scale
-                st = st
-            u_dist, s_dist = self.get_likelihood(
-                ut,
-                st,
-                u_log_library,
-                s_log_library,
-                u_scale,
-                s_scale,
-                u_read_depth,
-                s_read_depth,
-            )
-            u = pyro.sample("u", u_dist, obs=u_obs)
-            s = pyro.sample("s", s_dist, obs=s_obs)
-        return ut, st
-
-    def model2(
-        self,
-        u_obs: Optional[torch.Tensor] = None,
-        s_obs: Optional[torch.Tensor] = None,
-        u_log_library: Optional[torch.Tensor] = None,
-        s_log_library: Optional[torch.Tensor] = None,
-        ind_x: Optional[torch.Tensor] = None,
-    ) -> Tuple[torch.Tensor, torch.Tensor]:
-        """max plate = 1 with only cell plate"""
-        cell_plate = self.create_plate(
-            u_obs, s_obs, u_log_library, s_log_library, ind_x
-        )
-        alpha = self.alpha
-        beta = self.beta
-        gamma = self.gamma
-        switching = self.switching
-        u_scale = self.u_scale
-        s_scale = self.s_scale
-        with (
-            cell_plate
-        ):  # , poutine.mask(mask=pyro.subsample(self.mask.to(alpha.device), event_dim=1)):
-            t = self.latent_time
-            u_inf, s_inf = mRNA(switching, self.zero, self.zero, alpha, beta, gamma)
-            state = (
-                pyro.sample(
-                    "cell_gene_state", Bernoulli(logits=t - switching).to_event(1)
-                )
-                == self.zero
-            )
-            u0_vec = torch.where(state, self.zero, u_inf)
-            s0_vec = torch.where(state, self.zero, s_inf)
-            alpha_vec = torch.where(state, alpha, self.zero)
-            tau = torch.where(state, t, t - switching).clamp(0.0)
-            ut, st = mRNA(tau, u0_vec, s0_vec, alpha_vec, beta, gamma)
-            u_dist, s_dist = self.get_likelihood(
-                ut, st, u_log_library, s_log_library, u_scale, s_scale
-            )
-            u = pyro.sample("u", u_dist.to_event(1), obs=u_obs)
-            s = pyro.sample("s", s_dist.to_event(1), obs=s_obs)
-        return ut, st
-
-    def forward(
-        self,
-        u_obs: Optional[torch.Tensor] = None,
-        s_obs: Optional[torch.Tensor] = None,
-        u_log_library: Optional[torch.Tensor] = None,
-        s_log_library: Optional[torch.Tensor] = None,
-        ind_x: Optional[torch.Tensor] = None,
-    ) -> Tuple[torch.Tensor, torch.Tensor]:
-        if self.plate_size == 2:
-            return self.model(u_obs, s_obs, u_log_library, s_log_library, ind_x)
-        else:
-            return self.model2(u_obs, s_obs, u_log_library, s_log_library, ind_x)
+    # def model(
+    #     self,
+    #     u_obs: Optional[torch.Tensor] = None,
+    #     s_obs: Optional[torch.Tensor] = None,
+    #     u_log_library: Optional[torch.Tensor] = None,
+    #     s_log_library: Optional[torch.Tensor] = None,
+    #     ind_x: Optional[torch.Tensor] = None,
+    # ) -> Tuple[torch.Tensor, torch.Tensor]:
+    #     """max plate = 2 with cell and gene plate"""
+    #     cell_plate, gene_plate = self.create_plates(
+    #         u_obs, s_obs, u_log_library, s_log_library, ind_x
+    #     )
+
+    #     with gene_plate, poutine.mask(mask=self.include_prior):
+    #         alpha = self.alpha
+    #         beta = self.beta
+    #         gamma = self.gamma
+    #         switching = self.dt_switching
+    #         u_scale = self.u_scale
+    #         s_scale = self.s_scale
+    #         if self.t_scale_on and self.shared_time:
+    #             t_scale = self.t_scale
+    #         if self.latent_factor_operation == "selection":
+    #             p_velocity = self.p_velocity
+
+    #         if self.latent_factor == "linear":
+    #             u_pcs_mean = pyro.sample("u_pcs_mean", Normal(self.zero, self.one))
+    #             s_pcs_mean = pyro.sample("s_pcs_mean", Normal(self.zero, self.one))
+    #         u_inf, s_inf = mRNA(switching, self.zero, self.zero, alpha, beta, gamma)
+
+    #     if self.latent_factor == "linear":
+    #         cell_codebook = self.cell_codebook
+    #         with cell_plate, poutine.mask(mask=False):
+    #             cell_code = self.cell_code
+    #     if self.shared_time:
+    #         with cell_plate:
+    #             cell_time = self.cell_time
+
+    #     u_read_depth = None
+    #     s_read_depth = None
+
+    #     with cell_plate, gene_plate, poutine.mask(
+    #         mask=pyro.subsample(self.mask.to(alpha.device), event_dim=0)
+    #     ):
+    #         t = self.latent_time
+    #         if self.shared_time:
+    #             t = cell_time * t_scale + t if self.t_scale_on else cell_time + t
+    #         state = (
+    #             pyro.sample("cell_gene_state", Bernoulli(logits=t - switching))
+    #             == self.zero
+    #         )
+    #         u0_vec = torch.where(state, self.zero, u_inf)
+    #         s0_vec = torch.where(state, self.zero, s_inf)
+    #         alpha_vec = torch.where(state, alpha, self.zero)
+    #         tau = relu(torch.where(state, t, t - switching))
+    #         ut, st = mRNA(tau, u0_vec, s0_vec, alpha_vec, beta, gamma)
+    #         if self.latent_factor_operation == "selection":
+    #             velocity_genecellpair = pyro.sample(
+    #                 "genecellpair_type", Bernoulli(p_velocity)
+    #             )
+    #         if self.latent_factor == "linear":
+    #             regressor_output = torch.einsum(
+    #                 "abc,cd->ad", cell_code, cell_codebook.squeeze()
+    #             )
+    #             regressor_u = softplus(
+    #                 regressor_output[..., : self.num_genes].squeeze() + u_pcs_mean
+    #             )
+    #             regressor_s = softplus(
+    #                 regressor_output[..., self.num_genes :].squeeze() + s_pcs_mean
+    #             )
+    #         if self.latent_factor_operation == "selection":
+    #             ut = torch.where(
+    #                 velocity_genecellpair == self.one,
+    #                 (ut * u_scale / s_scale),
+    #                 softplus(regressor_u),
+    #             )
+    #             st = torch.where(
+    #                 velocity_genecellpair == self.one, st, softplus(regressor_s)
+    #             )
+    #         elif self.latent_factor_operation == "sum":
+    #             ut = ut * u_scale / s_scale + regressor_u
+    #             st = st + regressor_s
+    #         else:
+    #             ut = ut * u_scale / s_scale
+    #             st = st
+    #         u_dist, s_dist = self.get_likelihood(
+    #             ut,
+    #             st,
+    #             u_log_library,
+    #             s_log_library,
+    #             u_scale,
+    #             s_scale,
+    #             u_read_depth,
+    #             s_read_depth,
+    #         )
+    #         u = pyro.sample("u", u_dist, obs=u_obs)
+    #         s = pyro.sample("s", s_dist, obs=s_obs)
+    #     return ut, st
+
+    # def model2(
+    #     self,
+    #     u_obs: Optional[torch.Tensor] = None,
+    #     s_obs: Optional[torch.Tensor] = None,
+    #     u_log_library: Optional[torch.Tensor] = None,
+    #     s_log_library: Optional[torch.Tensor] = None,
+    #     ind_x: Optional[torch.Tensor] = None,
+    # ) -> Tuple[torch.Tensor, torch.Tensor]:
+    #     """max plate = 1 with only cell plate"""
+    #     cell_plate = self.create_plate(
+    #         u_obs, s_obs, u_log_library, s_log_library, ind_x
+    #     )
+    #     alpha = self.alpha
+    #     beta = self.beta
+    #     gamma = self.gamma
+    #     switching = self.switching
+    #     u_scale = self.u_scale
+    #     s_scale = self.s_scale
+    #     with (cell_plate):
+    #         t = self.latent_time
+    #         u_inf, s_inf = mRNA(switching, self.zero, self.zero, alpha, beta, gamma)
+    #         state = (
+    #             pyro.sample(
+    #                 "cell_gene_state", Bernoulli(logits=t - switching).to_event(1)
+    #             )
+    #             == self.zero
+    #         )
+    #         u0_vec = torch.where(state, self.zero, u_inf)
+    #         s0_vec = torch.where(state, self.zero, s_inf)
+    #         alpha_vec = torch.where(state, alpha, self.zero)
+    #         tau = torch.where(state, t, t - switching).clamp(0.0)
+    #         ut, st = mRNA(tau, u0_vec, s0_vec, alpha_vec, beta, gamma)
+    #         u_dist, s_dist = self.get_likelihood(
+    #             ut, st, u_log_library, s_log_library, u_scale, s_scale
+    #         )
+    #         u = pyro.sample("u", u_dist.to_event(1), obs=u_obs)
+    #         s = pyro.sample("s", s_dist.to_event(1), obs=s_obs)
+    #     return ut, st
+
+    # def forward(
+    #     self,
+    #     u_obs: Optional[torch.Tensor] = None,
+    #     s_obs: Optional[torch.Tensor] = None,
+    #     u_log_library: Optional[torch.Tensor] = None,
+    #     s_log_library: Optional[torch.Tensor] = None,
+    #     ind_x: Optional[torch.Tensor] = None,
+    # ) -> Tuple[torch.Tensor, torch.Tensor]:
+    #     if self.plate_size == 2:
+    #         return self.model(u_obs, s_obs, u_log_library, s_log_library, ind_x)
+    #     else:
+    #         return self.model2(u_obs, s_obs, u_log_library, s_log_library, ind_x)
 
 
 class AuxCellVelocityModel(VelocityModel):
-    def forward(
-        self,
-        u_obs: Optional[torch.Tensor] = None,
-        s_obs: Optional[torch.Tensor] = None,
-        u_log_library: Optional[torch.Tensor] = None,
-        s_log_library: Optional[torch.Tensor] = None,
-        u_log_library_loc: Optional[torch.Tensor] = None,
-        s_log_library_loc: Optional[torch.Tensor] = None,
-        u_log_library_scale: Optional[torch.Tensor] = None,
-        s_log_library_scale: Optional[torch.Tensor] = None,
-        ind_x: Optional[torch.Tensor] = None,
-    ) -> Tuple[torch.Tensor, torch.Tensor]:
-        """max plate = 2 with cell and gene plate"""
-        cell_plate, gene_plate = self.create_plates(
-            u_obs,
-            s_obs,
-            u_log_library,
-            s_log_library,
-            u_log_library_loc,
-            s_log_library_loc,
-            u_log_library_scale,
-            s_log_library_scale,
-            ind_x,
-        )
-        with gene_plate, poutine.mask(mask=self.include_prior):
-            alpha = self.alpha
-            beta = self.beta
-            gamma = self.gamma
-            dt_switching = self.dt_switching
-            u_scale = self.u_scale
-            s_scale = self.s_scale
-            # u_inf, s_inf = ode_mRNA(switching, self.zero, self.zero, alpha, beta, gamma)
-            # if self.t_scale_on and self.shared_time:
-            #    t_scale = self.t_scale
-            #    gene_offset = self.gene_offset
-            # else:
-            #    t_scale = None
-            #    gene_offset = None
-            # u0 = pyro.sample("u0", Gamma(self.one, self.one*2).mask(True))
-            # s0 = pyro.sample("s0", Gamma(self.one, self.one*2).mask(True))
-            # u0 = torch.where(u0 >= u_inf, u_inf, u0)
-            # s0 = torch.where(s0 >= s_inf, s_inf, s0)
-            # t_scale = self.t_scale
-
-            # u0 = s0 = self.zero
-            u0 = pyro.sample("u_offset", LogNormal(self.zero, self.one))
-            s0 = pyro.sample("s_offset", LogNormal(self.zero, self.one))
-            t_scale = None
-
-            gene_offset = self.gene_offset if self.add_offset else self.zero
-            switching = dt_switching + gene_offset
-            # u_inf, s_inf = mRNA(switching, self.zero, self.zero, alpha, beta, gamma)
-            # u_inf, s_inf = mRNA(dt_switching, self.zero, self.zero, alpha, beta, gamma)
-            u_inf, s_inf = mRNA(dt_switching, u0, s0, alpha, beta, gamma)
-
-            # u0 = torch.where(u0 > u_inf, u_inf, u0)
-            # s0 = torch.where(s0 > s_inf, s_inf, s0)
-
-            if self.latent_factor_operation == "selection":
-                p_velocity = pyro.sample("p_velocity", Beta(self.one * 5, self.one))
-            else:
-                p_velocity = None
-
-            if self.latent_factor == "linear":
-                u_pcs_mean = pyro.sample("u_pcs_mean", Normal(self.zero, self.one))
-                s_pcs_mean = pyro.sample("s_pcs_mean", Normal(self.zero, self.one))
-            else:
-                u_pcs_mean, s_pcs_mean = None, None
-
-        s_read_depth = None
-        # with cell_plate:
-        #    u_read_depth = pyro.sample('u_read_depth', dist.LogNormal(u_log_library, self.one))
-        #    s_read_depth = pyro.sample('s_read_depth', dist.LogNormal(s_log_library, self.one))
-        u_read_depth = None
-        # same as before, just refactored slightly
-        # with cell_plate, gene_plate:
-        #     cell_gene_mask = pyro.subsample(self.mask.to(alpha.device), event_dim=0)
-
-        cell_codebook = self.cell_codebook if self.latent_factor == "linear" else None
-        # with cell_plate, poutine.mask(mask=(u_obs > 0) & (s_obs > 0)):
-        with cell_plate:  # , poutine.mask(mask=cell_gene_mask):
-            # u_observed_total_dist = ...  # needs to be positive - maybe Poisson(num_genes * sequencing_depth)?
-            # u_observed_total = pyro.sample("u_observed_total", u_observed_total_dist, obs=u_obs.sum(-2))
-            # u_read_depth = pyro.sample('u_read_depth', LogNormal(u_log_library, self.one))
-            # s_read_depth = pyro.sample('s_read_depth', LogNormal(s_log_library, self.one))
-            with pyro.condition(data={"u": u_obs, "s": s_obs}):
-                ut, st = self.generate_cell(
-                    gene_plate,
-                    alpha,
-                    beta,
-                    gamma,
-                    switching,
-                    u_inf,
-                    s_inf,
-                    u_scale,
-                    s_scale,
-                    u_log_library,
-                    s_log_library,
-                    u_pcs_mean=u_pcs_mean,
-                    s_pcs_mean=s_pcs_mean,
-                    cell_codebook=cell_codebook,
-                    t_scale=t_scale,
-                    gene_offset=gene_offset,
-                    p_velocity=p_velocity,
-                    decoder_on=self.decoder_on,
-                    u_read_depth=u_read_depth,
-                    s_read_depth=s_read_depth,
-                    u0=u0,
-                    s0=s0,
-                )
-
-        # new: add population of fake cells to introduce global correlation across cells
-        if self.num_aux_cells > 0:
-            with pyro.contrib.autoname.scope(prefix="aux"):
-                # TODO set self.num_aux_cells in self.__init__, 10-200
-                aux_cell_plate = pyro.plate(
-                    "aux_cell_plate", self.num_aux_cells, dim=cell_plate.dim
-                )
-                with aux_cell_plate:
-                    # aux_u_obs = pyro.param("aux_u_obs", lambda: self.aux_u_obs_init, constraint=positive, event_dim=0)  # TODO initialize
-                    # aux_s_obs = pyro.param("aux_s_obs", lambda: self.aux_s_obs_init, constraint=positive, event_dim=0)  # TODO initialize
-                    # TODO: change the parameter cells into fixed cells
-                    # use a larger number of fixed cells
-                    aux_u_obs = self.aux_u_obs_init
-                    aux_s_obs = self.aux_s_obs_init
-                    aux_u_log_library = torch.log(aux_u_obs.sum(axis=-1))  # TODO define
-                    aux_s_log_library = torch.log(aux_s_obs.sum(axis=-1))  # TODO define
-                    with pyro.condition(data={"u": aux_u_obs, "s": aux_s_obs}):
-                        aux_ut, aux_st = self.generate_cell(
-                            gene_plate,
-                            alpha,
-                            beta,
-                            gamma,
-                            switching,
-                            u_inf,
-                            s_inf,
-                            u_scale,
-                            s_scale,
-                            aux_u_log_library,
-                            aux_s_log_library,
-                            u_pcs_mean=u_pcs_mean,
-                            s_pcs_mean=s_pcs_mean,
-                            cell_codebook=cell_codebook,
-                            t_scale=t_scale,
-                            gene_offset=gene_offset,
-                            p_velocity=p_velocity,
-                            decoder_on=self.decoder_on,
-                            u_read_depth=u_read_depth,
-                            s_read_depth=s_read_depth,
-                            u0=u0,
-                            s0=s0,
-                        )
-        # same as before: return only non-auxiliary cell predictions
-        return ut, st
-
     def generate_cell(
         self,
         gene_plate,
         alpha,
         beta,
         gamma,
         switching,
@@ -813,19 +720,17 @@
                 .to_event(1)
                 .mask(self.include_prior),
             )
         else:
             cell_code = None
 
         if self.shared_time:
-            ##cell_time = pyro.sample("cell_time", LogNormal(self.zero, self.one).mask(False)) # mask=False works for cpm and raw read count, count needs steady-state initialization
             cell_time = pyro.sample(
                 "cell_time", LogNormal(self.zero, self.one).mask(self.include_prior)
-            )  # mask=False works for cpm and raw read count, count needs steady-state initialization
-        ##assert cell_time.shape == (256, 1)
+            )
 
         with gene_plate:
             if self.latent_factor_operation == "selection":
                 cellgene_type = pyro.sample("cellgene_type", Bernoulli(p_velocity))
             else:
                 cellgene_type = None
 
@@ -846,32 +751,31 @@
                     else cell_time + t
                 )
             else:
                 t = pyro.sample(
                     "latent_time",
                     LogNormal(self.zero, self.one).mask(self.include_prior),
                 )
-            ##state = pyro.sample("cell_gene_state", Bernoulli(logits=t-switching)) == self.zero
+
             state = (
                 pyro.sample(
                     "cell_gene_state",
                     Bernoulli(logits=t - switching),
                     infer={"enumerate": "sequential"},
                 )
                 == self.zero
             )
             u0_vec = torch.where(state, u0, u_inf)
             s0_vec = torch.where(state, s0, s_inf)
             alpha_vec = torch.where(state, alpha, self.zero)
 
             tau = softplus(torch.where(state, t - gene_offset, t - switching))
-            # tau = relu(torch.where(state, t-gene_offset, t - switching))
 
             ut, st = mRNA(tau, u0_vec, s0_vec, alpha_vec, beta, gamma)
-            # ut, st = ode_mRNA(tau, u0_vec, s0_vec, alpha_vec, beta, gamma)
+
             if self.latent_factor == "linear":
                 regressor_output = torch.einsum(
                     "abc,cd->ad", cell_code, cell_codebook.squeeze()
                 )
                 regressor_u = softplus(
                     regressor_output[..., : self.num_genes].squeeze() + u_pcs_mean
                 )
@@ -887,64 +791,151 @@
                 st = torch.where(cellgene_type == self.one, st, softplus(regressor_s))
             elif self.latent_factor_operation == "sum":
                 ut = ut * u_scale / s_scale + regressor_u
                 st = st + regressor_s
             else:
                 ut = ut * u_scale / s_scale
                 st = st
-            u_dist, s_dist = self.get_likelihood(
-                ut,
-                st,
-                u_log_library,
-                s_log_library,
-                u_scale,
-                s_scale,
-                u_read_depth=u_read_depth,
-                s_read_depth=s_read_depth,
-            )
-            u = pyro.sample("u", u_dist)
-            s = pyro.sample("s", s_dist)
+            # u_dist, s_dist = self.get_likelihood(
+            #     ut,
+            #     st,
+            #     u_log_library,
+            #     s_log_library,
+            #     u_scale,
+            #     s_scale,
+            #     u_read_depth=u_read_depth,
+            #     s_read_depth=s_read_depth,
+            # )
+            # u = pyro.sample("u", u_dist)
+            # s = pyro.sample("s", s_dist)
         return ut, st
 
+    # def forward(
+    #     self,
+    #     u_obs: Optional[torch.Tensor] = None,
+    #     s_obs: Optional[torch.Tensor] = None,
+    #     u_log_library: Optional[torch.Tensor] = None,
+    #     s_log_library: Optional[torch.Tensor] = None,
+    #     u_log_library_loc: Optional[torch.Tensor] = None,
+    #     s_log_library_loc: Optional[torch.Tensor] = None,
+    #     u_log_library_scale: Optional[torch.Tensor] = None,
+    #     s_log_library_scale: Optional[torch.Tensor] = None,
+    #     ind_x: Optional[torch.Tensor] = None,
+    # ) -> Tuple[torch.Tensor, torch.Tensor]:
+    #     """max plate = 2 with cell and gene plate"""
+    #     cell_plate, gene_plate = self.create_plates(
+    #         u_obs,
+    #         s_obs,
+    #         u_log_library,
+    #         s_log_library,
+    #         u_log_library_loc,
+    #         s_log_library_loc,
+    #         u_log_library_scale,
+    #         s_log_library_scale,
+    #         ind_x,
+    #     )
+    #     with gene_plate, poutine.mask(mask=self.include_prior):
+    #         alpha = self.alpha
+    #         beta = self.beta
+    #         gamma = self.gamma
+    #         dt_switching = self.dt_switching
+    #         u_scale = self.u_scale
+    #         s_scale = self.s_scale
+
+    #         u0 = pyro.sample("u_offset", LogNormal(self.zero, self.one))
+    #         s0 = pyro.sample("s_offset", LogNormal(self.zero, self.one))
+    #         t_scale = None
+
+    #         gene_offset = self.gene_offset if self.add_offset else self.zero
+    #         switching = dt_switching + gene_offset
+    #         u_inf, s_inf = mRNA(dt_switching, u0, s0, alpha, beta, gamma)
+
+    #         if self.latent_factor_operation == "selection":
+    #             p_velocity = pyro.sample("p_velocity", Beta(self.one * 5, self.one))
+    #         else:
+    #             p_velocity = None
+
+    #         if self.latent_factor == "linear":
+    #             u_pcs_mean = pyro.sample("u_pcs_mean", Normal(self.zero, self.one))
+    #             s_pcs_mean = pyro.sample("s_pcs_mean", Normal(self.zero, self.one))
+    #         else:
+    #             u_pcs_mean, s_pcs_mean = None, None
+
+    #     s_read_depth = None
+    #     u_read_depth = None
+
+    #     cell_codebook = self.cell_codebook if self.latent_factor == "linear" else None
+    #     with cell_plate:
+    #         with pyro.condition(data={"u": u_obs, "s": s_obs}):
+    #             ut, st = self.generate_cell(
+    #                 gene_plate,
+    #                 alpha,
+    #                 beta,
+    #                 gamma,
+    #                 switching,
+    #                 u_inf,
+    #                 s_inf,
+    #                 u_scale,
+    #                 s_scale,
+    #                 u_log_library,
+    #                 s_log_library,
+    #                 u_pcs_mean=u_pcs_mean,
+    #                 s_pcs_mean=s_pcs_mean,
+    #                 cell_codebook=cell_codebook,
+    #                 t_scale=t_scale,
+    #                 gene_offset=gene_offset,
+    #                 p_velocity=p_velocity,
+    #                 decoder_on=self.decoder_on,
+    #                 u_read_depth=u_read_depth,
+    #                 s_read_depth=s_read_depth,
+    #                 u0=u0,
+    #                 s0=s0,
+    #             )
+
+    #     if self.num_aux_cells > 0:
+    #         with pyro.contrib.autoname.scope(prefix="aux"):
+    #             aux_cell_plate = pyro.plate(
+    #                 "aux_cell_plate", self.num_aux_cells, dim=cell_plate.dim
+    #             )
+    #             with aux_cell_plate:
+    #                 aux_u_obs = self.aux_u_obs_init
+    #                 aux_s_obs = self.aux_s_obs_init
+    #                 aux_u_log_library = torch.log(aux_u_obs.sum(axis=-1))
+    #                 aux_s_log_library = torch.log(aux_s_obs.sum(axis=-1))
+    #                 with pyro.condition(data={"u": aux_u_obs, "s": aux_s_obs}):
+    #                     aux_ut, aux_st = self.generate_cell(
+    #                         gene_plate,
+    #                         alpha,
+    #                         beta,
+    #                         gamma,
+    #                         switching,
+    #                         u_inf,
+    #                         s_inf,
+    #                         u_scale,
+    #                         s_scale,
+    #                         aux_u_log_library,
+    #                         aux_s_log_library,
+    #                         u_pcs_mean=u_pcs_mean,
+    #                         s_pcs_mean=s_pcs_mean,
+    #                         cell_codebook=cell_codebook,
+    #                         t_scale=t_scale,
+    #                         gene_offset=gene_offset,
+    #                         p_velocity=p_velocity,
+    #                         decoder_on=self.decoder_on,
+    #                         u_read_depth=u_read_depth,
+    #                         s_read_depth=s_read_depth,
+    #                         u0=u0,
+    #                         s0=s0,
+    #                     )
+    #     return ut, st
+
 
 class VelocityModelAuto(AuxCellVelocityModel):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
-        # if self.guide_type in [
-        #     "velocity_auto",
-        #     "velocity_auto_depth",
-        #     "velocity_auto_t0_constraint",
-        # ]:
-        #     self.time_encoder = TimeEncoder2(
-        #         self.num_genes,
-        #         n_output=1,
-        #         dropout_rate=0.5,
-        #         activation_fn=nn.ELU,
-        #         n_layers=3,
-        #         var_eps=1e-6,
-        #     )
-        # if self.correct_library_size and (
-        #     self.guide_type == "velocity_auto"
-        #     or self.guide_type == "velocity_auto_t0_constraint"
-        # ):
-        #     self.u_lib_encoder = TimeEncoder2(
-        #         self.num_genes + 1, 1, n_layers=3, dropout_rate=0.5
-        #     )
-        #     self.s_lib_encoder = TimeEncoder2(
-        #         self.num_genes + 1, 1, n_layers=3, dropout_rate=0.5
-        #     )
-
-        # if self.cell_specific_kinetics is not None:
-        #     self.multikinetics_encoder = TimeEncoder2(
-        #         1,  # encode cell state
-        #         1,  # encode cell specificity of kinetics
-        #         dropout_rate=0.5,
-        #         last_layer_activation=nn.Sigmoid(),
-        #         n_layers=3,
-        #     )
 
     def get_rna(
         self,
         u_scale: torch.Tensor,
         s_scale: torch.Tensor,
         alpha: torch.Tensor,
         beta: torch.Tensor,
@@ -953,28 +944,94 @@
         u0: torch.Tensor,
         s0: torch.Tensor,
         t0: torch.Tensor,
         switching: Optional[torch.Tensor] = None,
         u_inf: Optional[torch.Tensor] = None,
         s_inf: Optional[torch.Tensor] = None,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
+        """
+        Computes the unspliced (u) and spliced (s) RNA expression levels given the model parameters.
+
+        Args:
+            u_scale (torch.Tensor): Scaling factor for unspliced expression.
+            s_scale (torch.Tensor): Scaling factor for spliced expression.
+            alpha (torch.Tensor): Transcription rate.
+            beta (torch.Tensor): Splicing rate.
+            gamma (torch.Tensor): Degradation rate.
+            t (torch.Tensor): Cell time.
+            u0 (torch.Tensor): Unspliced RNA initial expression.
+            s0 (torch.Tensor): Spliced RNA initial expression.
+            t0 (torch.Tensor): Initial cell time.
+            switching (Optional[torch.Tensor], optional): Switching time. Default is None.
+            u_inf (Optional[torch.Tensor], optional): Unspliced RNA expression at switching time. Default is None.
+            s_inf (Optional[torch.Tensor], optional): Spliced RNA expression at switching time. Default is None.
+
+        Returns:
+            Tuple[torch.Tensor, torch.Tensor]: The unspliced (u) and spliced (s) RNA expression levels.
+
+        Examples:
+            >>> import torch
+            >>> from pyrovelocity._velocity_model import VelocityModelAuto
+            >>> model = VelocityModelAuto(
+            ...             3,
+            ...             4,
+            ...             "Poisson",
+            ...             True,
+            ...             False,
+            ...             2,
+            ...             "none",
+            ...             latent_factor_operation="selection",
+            ...             latent_factor_size=10,
+            ...             include_prior=False,
+            ...             num_aux_cells=0,
+            ...             only_cell_times=True,
+            ...             decoder_on=False,
+            ...             add_offset=False,
+            ...             correct_library_size=True,
+            ...             guide_type="auto_t0_constraint",
+            ...             cell_specific_kinetics=None,
+            ...             **{}
+            ...         )
+            >>> u, s = model.get_rna(
+            ...            u_scale=torch.tensor([0.9793, 1.0567, 0.8610, 0.9304], device="cpu"),
+            ...            s_scale=torch.tensor(1.0),
+            ...            alpha=torch.tensor([0.4869, 1.5997, 1.3962, 0.5038], device="cpu"),
+            ...            beta=torch.tensor([0.5403, 1.1192, 0.9912, 1.1783], device="cpu"),
+            ...            gamma=torch.tensor([1.9612, 0.5533, 2.1050, 4.9345], device="cpu"),
+            ...            t=torch.tensor([[0.4230], [0.5119], [0.2689]], device="cpu"),
+            ...            u0=torch.tensor(0.0),
+            ...            s0=torch.tensor(0.0),
+            ...            t0=torch.tensor([-0.4867, 0.5581, -0.6957, 0.6028], device="cpu"),
+            ...            switching=torch.tensor([1.1886, 1.1227, 0.6789, 4.1003], device="cpu"),
+            ...            u_inf=torch.tensor([0.5367, 0.6695, 1.0479, 0.4206], device="cpu"),
+            ...            s_inf=torch.tensor([0.1132, 0.2100, 0.3750, 0.0999], device="cpu"),
+            >>>        )
+        """
+        # >>> u, s
+        # (tensor([[0.4329, 0.7624, 0.5111, 0.2033],
+        # [0.4209, 0.7971, 0.9301, 0.2126],
+        # [0.4060, 0.7024, 0.5448, 0.1873]]),
+        # tensor([[0.0818, 0.2512, 0.3615, 0.0381],
+        # [0.1229, 0.2801, 0.3978, 0.0410],
+        # [0.0733, 0.2065, 0.3721, 0.0333]]))
         if self.cell_specific_kinetics is None:
+            # enum = "parallel"
             if (
                 self.guide_type != "auto"
-                and pyro.__version__.startswith("1.8.1")
+                and version.parse(pyro.__version__) > version.parse("1.8.1")
                 or self.guide_type == "auto"
-            ):  # parallel still memory leaky from pip install
+            ):
                 enum = "parallel"
             elif (
                 self.guide_type != "auto"
                 and not pyro.__version__.startswith("1.8.1")
                 and pyro.__version__.startswith("1.6.0")
             ):
-                # neural network guide only works in sequential enumeration
-                # only 1.6.0 version supports model-side sequential enumeration
+                # neural network guide only works with sequential enumeration
+                # only version 1.6.0 supports model-side sequential enumeration
                 enum = "sequential"
 
             state = (
                 pyro.sample(
                     "cell_gene_state",
                     Bernoulli(logits=t - switching),
                     infer={"enumerate": enum},
@@ -987,89 +1044,95 @@
             alpha_vec = torch.where(state, alpha, alpha_off)
             tau = softplus(torch.where(state, t - t0, t - switching))
         else:
             u0_vec = u0
             s0_vec = s0
             alpha_vec = alpha
             tau = softplus(t - t0)
-            ##tau = relu(torch.where(state, t - t0, t - switching))
-        # print(alpha_vec.shape)
+
         ut, st = mRNA(tau, u0_vec, s0_vec, alpha_vec, beta, gamma)
         ut = ut * u_scale / s_scale
         return ut, st
 
-    def get_time(
-        self,
-        u_scale,
-        s_scale,
-        alpha,
-        beta,
-        gamma,
-        u_obs,
-        s_obs,
-        u0,
-        s0,
-        t0,
-        dt_switching,
-        u_inf,
-        s_inf,
-        u_read_depth=None,
-        s_read_depth=None,
-    ):
-        scale = u_scale / s_scale
-
-        # if u_read_depth is None:
-        #    u_ = u_obs / scale
-        #    s_ = s_obs
-        # else:
-        #    #neural network correction of read depth not converge
-        #    u_ = u_obs / u_read_depth / scale
-        #    s_ = s_obs / s_read_depth
-        u_ = u_obs / scale
-        s_ = s_obs
-
-        std_u = u_scale / scale
-        tau = tau_inv(u_, s_, u0, s0, alpha, beta, gamma)
-        ut, st = mRNA(tau, u0, s0, alpha, beta, gamma)
-        if self.cell_specific_kinetics is None:
-            tau_ = tau_inv(u_, s_, u_inf, s_inf, self.zero, beta, gamma)
-            ut_, st_ = mRNA(tau_, u_inf, s_inf, self.zero, beta, gamma)
-        state_on = ((ut - u_) / std_u) ** 2 + ((st - s_) / s_scale) ** 2
-        state_zero = ((ut - u0) / std_u) ** 2 + ((st - s0) / s_scale) ** 2
-        if self.cell_specific_kinetics is None:
-            state_inf = ((ut_ - u_inf) / std_u) ** 2 + ((st_ - s_inf) / s_scale) ** 2
-            state_off = ((ut_ - u_) / std_u) ** 2 + ((st_ - s_) / s_scale) ** 2
-            cell_gene_state_logits = torch.stack(
-                [state_on, state_zero, state_off, state_inf], dim=-1
-            ).argmin(-1)
-        if self.cell_specific_kinetics is None:
-            state = (cell_gene_state_logits > 1) == self.zero
-            t = torch.where(state, tau + t0, tau_ + dt_switching + t0)
-        else:
-            t = softplus(tau + t0)
-        cell_time_loc, cell_time_scale = self.time_encoder(t)
-        t = pyro.sample(
-            "cell_time", LogNormal(cell_time_loc, torch.sqrt(cell_time_scale))
-        )
-        return t
-
     def forward(
         self,
         u_obs: Optional[torch.Tensor] = None,
         s_obs: Optional[torch.Tensor] = None,
         u_log_library: Optional[torch.Tensor] = None,
         s_log_library: Optional[torch.Tensor] = None,
         u_log_library_loc: Optional[torch.Tensor] = None,
         s_log_library_loc: Optional[torch.Tensor] = None,
         u_log_library_scale: Optional[torch.Tensor] = None,
         s_log_library_scale: Optional[torch.Tensor] = None,
         ind_x: Optional[torch.Tensor] = None,
         cell_state: Optional[torch.Tensor] = None,
         time_info: Optional[torch.Tensor] = None,
     ) -> Tuple[torch.Tensor, torch.Tensor]:
+        """
+        Defines the forward model, which computes the unspliced (u) and spliced (s) RNA expression levels given the observations and model parameters.
+
+        Args:
+            u_obs (Optional[torch.Tensor], optional): Observed unspliced RNA expression. Default is None.
+            s_obs (Optional[torch.Tensor], optional): Observed spliced RNA expression. Default is None.
+            u_log_library (Optional[torch.Tensor], optional): Log-transformed library size for unspliced RNA. Default is None.
+            s_log_library (Optional[torch.Tensor], optional): Log-transformed library size for spliced RNA. Default is None.
+            u_log_library_loc (Optional[torch.Tensor], optional): Mean of log-transformed library size for unspliced RNA. Default is None.
+            s_log_library_loc (Optional[torch.Tensor], optional): Mean of log-transformed library size for spliced RNA. Default is None.
+            u_log_library_scale (Optional[torch.Tensor], optional): Scale of log-transformed library size for unspliced RNA. Default is None.
+            s_log_library_scale (Optional[torch.Tensor], optional): Scale of log-transformed library size for spliced RNA. Default is None.
+            ind_x (Optional[torch.Tensor], optional): Indices for the cells. Default is None.
+            cell_state (Optional[torch.Tensor], optional): Cell state information. Default is None.
+            time_info (Optional[torch.Tensor], optional): Time information for the cells. Default is None.
+
+        Returns:
+            Tuple[torch.Tensor, torch.Tensor]: The unspliced (u) and spliced (s) RNA expression levels.
+
+        Examples:
+            >>> import torch
+            >>> from pyrovelocity._velocity_model import VelocityModelAuto
+            >>> u_obs=torch.tensor(
+            ...     [[33.,  1.,  7.,  1.],
+            ...     [12., 30., 11.,  3.],
+            ...     [ 1.,  1.,  8.,  5.]],
+            ...     device="cpu",
+            >>> )
+            >>> s_obs=torch.tensor(
+            ...     [[32.0, 0.0, 6.0, 0.0],
+            ...     [11.0, 29.0, 10.0, 2.0],
+            ...     [0.0, 0.0, 7.0, 4.0]],
+            ...     device="cpu",
+            >>> )
+            >>> u_log_library=torch.tensor([[3.7377], [4.0254], [2.7081]], device="cpu")
+            >>> s_log_library=torch.tensor([[3.6376], [3.9512], [2.3979]], device="cpu")
+            >>> u_log_library_loc=torch.tensor([[3.4904], [3.4904], [3.4904]], device="cpu")
+            >>> s_log_library_loc=torch.tensor([[3.3289], [3.3289], [3.3289]], device="cpu")
+            >>> u_log_library_scale=torch.tensor([[0.6926], [0.6926], [0.6926]], device="cpu")
+            >>> s_log_library_scale=torch.tensor([[0.8214], [0.8214], [0.8214]], device="cpu")
+            >>> ind_x=torch.tensor([2, 0, 1], device="cpu")
+            >>> model = VelocityModelAuto(3,4)
+            >>> u, s = model.forward(
+            >>>            u_obs,
+            >>>            s_obs,
+            >>>            u_log_library,
+            >>>            s_log_library,
+            >>>            u_log_library_loc,
+            >>>            s_log_library_loc,
+            >>>            u_log_library_scale,
+            >>>            s_log_library_scale,
+            >>>            ind_x,
+            >>>        )
+            >>> u, s
+            (tensor([[33.,  1.,  7.,  1.],
+                    [12., 30., 11.,  3.],
+                    [ 1.,  1.,  8.,  5.]]),
+            tensor([[32.,  0.,  6.,  0.],
+                    [11., 29., 10.,  2.],
+                    [ 0.,  0.,  7.,  4.]]))
+        """
+
         cell_plate, gene_plate = self.create_plates(
             u_obs,
             s_obs,
             u_log_library,
             s_log_library,
             u_log_library_loc,
             s_log_library_loc,
@@ -1081,33 +1144,26 @@
         )
 
         with gene_plate, poutine.mask(mask=self.include_prior):
             alpha = self.alpha
             gamma = self.gamma
             beta = self.beta
 
-            # if self.cell_specific_kinetics is not None:
-            #     rho, _ = self.multikinetics_encoder(cell_state)
-            #     alpha = rho * alpha
-            #     beta = beta * rho
-            #     gamma = gamma * rho
-
             if self.add_offset:
                 u0 = pyro.sample("u_offset", LogNormal(self.zero, self.one))
                 s0 = pyro.sample("s_offset", LogNormal(self.zero, self.one))
             else:
                 s0 = u0 = self.zero
 
             t0 = pyro.sample("t0", Normal(self.zero, self.one))
 
             if (self.likelihood == "Normal") or (self.guide_type == "auto"):
                 u_scale = self.u_scale
                 s_scale = self.one
             else:
-                # NegativeBinomial and Poisson model
                 u_scale = s_scale = self.one
 
             if self.likelihood == "Normal":
                 s_scale = self.s_scale
             if self.cell_specific_kinetics is None:
                 dt_switching = self.dt_switching
                 u_inf, s_inf = mRNA(dt_switching, u0, s0, alpha, beta, gamma)
@@ -1119,30 +1175,14 @@
             else:
                 switching = u_inf = s_inf = None
 
         with cell_plate:
             t = pyro.sample(
                 "cell_time", LogNormal(self.zero, self.one).mask(self.include_prior)
             )
-            # physical time constraint or cytotrace constraint
-            # if time_info is not None:
-            #     physical_time = pyro.sample("physical_time", Bernoulli(logits=t), obs=time_info)
-            ## Gioele's suggestion
-            # alpha = alpha * t
-            # beta = beta * t
-            # gamma = gamma * t
-            # dt_switching = dt_switching * t
-            # with gene_plate:
-            #    if self.cell_specific_kinetics is None:
-            #        u_inf, s_inf = mRNA(dt_switching, u0, s0, alpha, beta, gamma)
-            #        u_inf = pyro.deterministic("u_inf", u_inf, event_dim=0)
-            #        s_inf = pyro.deterministic("s_inf", s_inf, event_dim=0)
-            #        switching = pyro.deterministic("switching", dt_switching + t0, event_dim=0)
-            #    else:
-            #        switching = u_inf = s_inf = None
 
         with cell_plate:
             u_cell_size_coef = ut_coef = s_cell_size_coef = st_coef = None
             u_read_depth = s_read_depth = None
             if self.correct_library_size and (self.likelihood != "Normal"):
                 if self.guide_type == "velocity_auto":
                     u_read_depth = torch.exp(u_log_library)
@@ -1151,15 +1191,14 @@
                     u_read_depth = pyro.sample(
                         "u_read_depth", LogNormal(u_log_library, u_log_library_scale)
                     )
                     s_read_depth = pyro.sample(
                         "s_read_depth", LogNormal(s_log_library, s_log_library_scale)
                     )
                     if self.correct_library_size == "cell_size_regress":
-                        # cell-wise coef per cell
                         u_cell_size_coef = pyro.sample(
                             "u_cell_size_coef", Normal(self.zero, self.one)
                         )
                         ut_coef = pyro.sample("ut_coef", Normal(self.zero, self.one))
                         s_cell_size_coef = pyro.sample(
                             "s_cell_size_coef", Normal(self.zero, self.one)
                         )
@@ -1168,19 +1207,14 @@
                 if self.guide_type in [
                     "auto_t0_constraint",
                     "velocity_auto_t0_constraint",
                 ]:
                     pyro.sample(
                         "time_constraint", Bernoulli(logits=t - t0), obs=self.one
                     )
-                # constraint u_inf > u0, s_inf > s0, reduce performance..
-                # pyro.sample("u_inf_constraint", Bernoulli(logits=alpha/beta-u0), obs=self.one)
-                # pyro.sample("s_inf_constraint", Bernoulli(logits=alpha/gamma-s0), obs=self.one)
-                # pyro.sample("u_inf_constraint2", Bernoulli(logits=alpha/beta-u_inf), obs=self.one)
-                # pyro.sample("s_inf_constraint2", Bernoulli(logits=alpha/gamma-s_inf), obs=self.one)
                 ut, st = self.get_rna(
                     u_scale,
                     s_scale,
                     alpha,
                     beta,
                     gamma,
                     t,
@@ -1204,7 +1238,55 @@
                     ut_coef=ut_coef,
                     s_cell_size_coef=s_cell_size_coef,
                     st_coef=st_coef,
                 )
                 u = pyro.sample("u", u_dist, obs=u_obs)
                 s = pyro.sample("s", s_dist, obs=s_obs)
         return u, s
+
+    # def get_time(
+    #     self,
+    #     u_scale,
+    #     s_scale,
+    #     alpha,
+    #     beta,
+    #     gamma,
+    #     u_obs,
+    #     s_obs,
+    #     u0,
+    #     s0,
+    #     t0,
+    #     dt_switching,
+    #     u_inf,
+    #     s_inf,
+    #     u_read_depth=None,
+    #     s_read_depth=None,
+    # ):
+    #     scale = u_scale / s_scale
+
+    #     u_ = u_obs / scale
+    #     s_ = s_obs
+
+    #     std_u = u_scale / scale
+    #     tau = tau_inv(u_, s_, u0, s0, alpha, beta, gamma)
+    #     ut, st = mRNA(tau, u0, s0, alpha, beta, gamma)
+    #     if self.cell_specific_kinetics is None:
+    #         tau_ = tau_inv(u_, s_, u_inf, s_inf, self.zero, beta, gamma)
+    #         ut_, st_ = mRNA(tau_, u_inf, s_inf, self.zero, beta, gamma)
+    #     state_on = ((ut - u_) / std_u) ** 2 + ((st - s_) / s_scale) ** 2
+    #     state_zero = ((ut - u0) / std_u) ** 2 + ((st - s0) / s_scale) ** 2
+    #     if self.cell_specific_kinetics is None:
+    #         state_inf = ((ut_ - u_inf) / std_u) ** 2 + ((st_ - s_inf) / s_scale) ** 2
+    #         state_off = ((ut_ - u_) / std_u) ** 2 + ((st_ - s_) / s_scale) ** 2
+    #         cell_gene_state_logits = torch.stack(
+    #             [state_on, state_zero, state_off, state_inf], dim=-1
+    #         ).argmin(-1)
+    #     if self.cell_specific_kinetics is None:
+    #         state = (cell_gene_state_logits > 1) == self.zero
+    #         t = torch.where(state, tau + t0, tau_ + dt_switching + t0)
+    #     else:
+    #         t = softplus(tau + t0)
+    #     cell_time_loc, cell_time_scale = self.time_encoder(t)
+    #     t = pyro.sample(
+    #         "cell_time", LogNormal(cell_time_loc, torch.sqrt(cell_time_scale))
+    #     )
+    #     return t
```

### Comparing `pyrovelocity-0.1.1/pyrovelocity/cytotrace.py` & `pyrovelocity-0.1.2/pyrovelocity/cytotrace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: 01_cytotrace.ipynb (unless otherwise specified).
-
 __all__ = [
     "census_normalize",
     "remove_zero_mvg",
     "compute_similarity2",
     "compute_similarity1",
     "compute_gcs",
     "convert_to_markov",
@@ -551,26 +549,26 @@
 
     print(markov.shape, gcs.shape)
     gcs = diffused(markov, gcs)
     rank = rankdata(gcs)
     scores = rank / gcs.shape[0]
 
     print(gcs)
-    adata.obs["gcs"] = None
+    adata.obs["gcs"] = np.nan
     adata.obs.iloc[cells_selected, adata.obs.columns.get_loc("gcs")] = gcs
 
     cytoGenes = compute_similarity2(census_X.T.A, scores.reshape(-1, 1))[0, :]
 
     adata.obs["cytotrace"] = np.nan
     adata.obs.iloc[cells_selected, adata.obs.columns.get_loc("cytotrace")] = scores
 
     adata.obs["counts"] = np.nan
     adata.obs.iloc[cells_selected, adata.obs.columns.get_loc("counts")] = gcs
 
-    adata.var["cytotrace"] = np.nan
+    adata.var["cytotrace"] = False
     adata.var.iloc[features_selected, adata.var.columns.get_loc("cytotrace")] = True
 
     adata.var["cytotrace_corrs"] = np.nan
     adata.var.iloc[
         features_selected, adata.var.columns.get_loc("cytotrace_corrs")
     ] = np.array(corrs, dtype=np.float32)
     return {
@@ -1107,21 +1105,7 @@
     values, base = np.histogram(data, bins=10)
     # evaluate the cumulative
     cumulative = np.cumsum(values)
     # plot the cumulative function
     plt.scatter(base[:-1], cumulative / cumulative[-1], c="blue")
     # plot the survival function
     # plt.plot(base[:-1], len(data)-cumulative, c='green')
-
-
-# Cell
-###from fastscript import *
-
-# @call_parse
-# def run_cytotrace(adata_path:Param('adata path: could be h5ad or loom', str),
-#                  output_path: Param('output .obs csv path', str),
-#                  solver: Param('regression nnls solver: \
-#                  larger cell number using fnnls, small cell number using nnls', str) = 'nnls'):
-#    adata = sc.read(adata_path)
-#    cytotrace(adata, solver=solver)
-#    adata.obs.to_csv("%s.csv" % output_path)
-#    adata.write(output_path)
```

### Comparing `pyrovelocity-0.1.1/pyrovelocity/plot.py` & `pyrovelocity-0.1.2/pyrovelocity/plot.py`

 * *Files 8% similar despite different names*

```diff
@@ -318,41 +318,50 @@
             summary["x_obs"]["mean"][:, 0],
             alpha=0.5,
             color="red",
         )
 
 
 def plot_posterior_time(
-    pos, adata, ax=None, fig=None, basis="umap", addition=True, position="left", s=3
+    posterior_samples,
+    adata,
+    ax=None,
+    fig=None,
+    basis="umap",
+    addition=True,
+    position="left",
+    s=3,
 ):
     if addition:
         sns.set_style("white")
         sns.set_context("paper", font_scale=1)
         matplotlib.rcParams.update({"font.size": 7})
         # celltime_cors = []
         # celltime_labels = []
-        # for index in range(pos['cell_time'].shape[0]):
-        #    celltime_cors.append(spearmanr(1-adata.obs.cytotrace, pos['cell_time'][index])[0])
+        # for index in range(posterior_samples['cell_time'].shape[0]):
+        #    celltime_cors.append(spearmanr(1-adata.obs.cytotrace, posterior_samples['cell_time'][index])[0])
         #    celltime_labels.append('Pyro-Velocity train data')
         # celltime_cors.append(spearmanr(1-adata.obs.cytotrace, adata.obs.latent_time)[0])
         # celltime_labels.append('scvelo')
         # sns.boxplot(x='label', y='correlation',
         #            data=pd.DataFrame({"correlation": celltime_cors, "label": celltime_labels}))
         # plt.tick_params(axis='x', rotation=90)
         # plt.ylabel("Correlation with Cytotrace")
         # plt.xlabel("")
         # plt.title("Benchmark shared cell time")
         # plt.ylim(0, 1)
         plt.figure()
-        test_hist = plt.hist(pos["cell_time"].mean(0), bins=100, label="test")
+        test_hist = plt.hist(
+            posterior_samples["cell_time"].mean(0), bins=100, label="test"
+        )
         plt.xlabel("mean of cell time")
         plt.ylabel("frequency")
         plt.title("Histogram of cell time posterior samples")
         plt.legend()
-    pos_mean_time = pos["cell_time"].mean(0)
+    pos_mean_time = posterior_samples["cell_time"].mean(0)
     # scale to 0-1?
     adata.obs["cell_time"] = pos_mean_time / pos_mean_time.max()
     if ax is None:
         fig, ax = plt.subplots(1, 1)
         fig.set_size_inches(2.36, 2)
 
     # scv.pl.umap(adata, color='cell_time', show=False, color_map='inferno',
@@ -386,47 +395,46 @@
 def mae_per_gene(pred_counts: ndarray, true_counts: ndarray) -> ndarray:
     """Computes mean average error between counts and predicted probabilities."""
     error = np.abs(true_counts - pred_counts).sum(-2)
     total = np.clip(true_counts.sum(-2), 1, np.inf)
     return -np.array(error / total)
 
 
-def plot_gene_ranking(
-    pos,
+def compute_volcano_data(
+    posterior_samples,
     adata,
-    ax=None,
     time_correlation_with="s",
     selected_genes=None,
-    assemble=False,
-    data="correlation",
     negative=False,
-    adjust_text=False,
 ) -> None:
-    assert isinstance(pos, tuple) or isinstance(pos, list)
-    assert isinstance(adata, list) or isinstance(adata, tuple)
+    assert isinstance(posterior_samples, (tuple, list))
+    assert isinstance(adata, (tuple, list))
+    assert "s" in posterior_samples[0]
+    assert "alpha" in posterior_samples[0]
 
     maes_list = []
     cors = []
     genes = []
     labels = []
     switching = []
-    for p, ad, label in zip(pos, adata, ["train", "valid"]):
-        for sample in range(30):
+    for p, ad, label in zip(posterior_samples, adata, ["train", "valid"]):
+        print(label)
+        for sample in range(p["alpha"].shape[0]):
             maes_list.append(
                 mae_per_gene(
                     p["s"][sample].squeeze(), ad.layers["raw_spliced"].toarray()
                 )
             )
             df_genes_cors = compute_similarity2(
                 p[time_correlation_with][sample].squeeze(),
                 p["cell_time"][sample].squeeze().reshape(-1, 1),
             )
             cors.append(df_genes_cors[0])
             genes.append(ad.var_names.values)
-            labels.append(["Poisson_%s" % label] * len(ad.var_names.values))
+            labels.append([f"Poisson_{label}"] * len(ad.var_names.values))
 
     volcano_data = pd.DataFrame(
         {
             "mean_mae": np.hstack(maes_list),
             "label": np.hstack(labels),
             "time_correlation": np.hstack(cors),
             "genes": np.hstack(genes),
@@ -448,18 +456,41 @@
             .head(300)
             .sort_values("time_correlation", ascending=negative)
             .head(4)
             .index
         )
     else:
         genes = selected_genes
-    fig = None
     volcano_data.loc[:, "selected genes"] = 0
     volcano_data.loc[genes, "selected genes"] = 1
 
+    return volcano_data, genes
+
+
+def plot_gene_ranking(
+    posterior_samples,
+    adata,
+    ax=None,
+    time_correlation_with="s",
+    selected_genes=None,
+    assemble=False,
+    data="correlation",
+    negative=False,
+    adjust_text=False,
+) -> None:
+    print(posterior_samples[0].keys())
+    if "u" in posterior_samples[0]:
+        volcano_data, genes = compute_volcano_data(
+            posterior_samples, adata, time_correlation_with, selected_genes, negative
+        )
+    else:
+        volcano_data = posterior_samples[0]["gene_ranking"]
+        genes = posterior_samples[0]["genes"]
+
+    fig = None
     from adjustText import adjust_text
 
     if data == "correlation":
         sns.scatterplot(
             x="time_correlation",
             y="mean_mae",
             hue="selected genes",
@@ -546,46 +577,49 @@
         ax.set_xlabel("gene switching time", fontsize=7)
         ax.set_ylabel("negative mean\nabsolute error", fontsize=7)
         sns.despine()
 
     return volcano_data, fig
 
 
-def denoised_umap(pos, adata, cell_state="state_info"):
+def denoised_umap(posterior_samples, adata, cell_state="state_info"):
     pass
 
     import sklearn
     import umap
     from sklearn.pipeline import Pipeline
 
     projection = [
         ("PCA", sklearn.decomposition.PCA(random_state=99, n_components=50)),
         ("UMAP", umap.UMAP(random_state=99, n_components=2)),
     ]
     pipelines = Pipeline(projection)
     fig, ax = plt.subplots(2, 2)
     fig.set_size_inches(9, 9)
-    expression = [pos["st"].mean(0)]
+    expression = [posterior_samples["st"].mean(0)]
     pipelines.fit(expression[0])
     umap_orig = pipelines.transform(expression[0])
     adata.obsm["X_umap1"] = umap_orig
     scv.pl.scatter(adata, basis="umap1", ax=ax[0][0], show=False)
 
     joint_pcs = pipelines.steps[0][1].transform(expression[0])
     adata.obsm["X_pyropca"] = joint_pcs
     scv.pp.neighbors(adata, use_rep="pyropca")
-    adata.layers["spliced_pyro"] = pos["st"].mean(0)
-    if "u_scale" in pos:
+    adata.layers["spliced_pyro"] = posterior_samples["st"].mean(0)
+    if "u_scale" in posterior_samples:
         adata.layers["velocity_pyro"] = (
-            pos["ut"] * pos["beta"] / (pos["u_scale"] / pos["s_scale"])
-            - pos["st"] * pos["gamma"]
+            posterior_samples["ut"]
+            * posterior_samples["beta"]
+            / (posterior_samples["u_scale"] / posterior_samples["s_scale"])
+            - posterior_samples["st"] * posterior_samples["gamma"]
         ).mean(0)
     else:
         adata.layers["velocity_pyro"] = (
-            pos["ut"] * pos["beta"] - pos["st"] * pos["gamma"]
+            posterior_samples["ut"] * posterior_samples["beta"]
+            - posterior_samples["st"] * posterior_samples["gamma"]
         ).mean(0)
     scv.tl.velocity_graph(adata, vkey="velocity_pyro", xkey="spliced_pyro")
     scv.tl.velocity_embedding(adata, vkey="velocity_pyro", basis="umap1")
     scv.pl.velocity_embedding_grid(
         adata,
         basis="umap1",
         vkey="velocity_pyro",
@@ -594,31 +628,36 @@
         arrow_size=3,
         color=cell_state,
         ax=ax[0][1],
         show=False,
     )
     adata.obsm["X_umap1"] = umap_orig
 
-    expression = [np.hstack([pos["st"].mean(0), pos["ut"].mean(0)])]
+    expression = [
+        np.hstack([posterior_samples["st"].mean(0), posterior_samples["ut"].mean(0)])
+    ]
     pipelines.fit(expression[0])
     umap_orig = pipelines.transform(expression[0])
     adata.obsm["X_umap2"] = umap_orig
     scv.pl.scatter(adata, basis="umap2", ax=ax[1][0], show=False)
     joint_pcs = pipelines.steps[0][1].transform(expression[0])
     adata.obsm["X_pyropca"] = joint_pcs
     scv.pp.neighbors(adata, use_rep="pyropca")
-    adata.layers["spliced_pyro"] = pos["st"].mean(0)
-    if "u_scale" in pos:
+    adata.layers["spliced_pyro"] = posterior_samples["st"].mean(0)
+    if "u_scale" in posterior_samples:
         adata.layers["velocity_pyro"] = (
-            pos["ut"] * pos["beta"] / (pos["u_scale"] / pos["s_scale"])
-            - pos["st"] * pos["gamma"]
+            posterior_samples["ut"]
+            * posterior_samples["beta"]
+            / (posterior_samples["u_scale"] / posterior_samples["s_scale"])
+            - posterior_samples["st"] * posterior_samples["gamma"]
         ).mean(0)
     else:
         adata.layers["velocity_pyro"] = (
-            pos["ut"] * pos["beta"] - pos["st"] * pos["gamma"]
+            posterior_samples["ut"] * posterior_samples["beta"]
+            - posterior_samples["st"] * posterior_samples["gamma"]
         ).mean(0)
     scv.tl.velocity_graph(adata, vkey="velocity_pyro", xkey="spliced_pyro")
     scv.tl.velocity_embedding(adata, vkey="velocity_pyro", basis="umap1")
     scv.pl.velocity_embedding_grid(
         adata,
         basis="umap2",
         vkey="velocity_pyro",
@@ -629,15 +668,15 @@
         show=False,
         ax=ax[1][1],
     )
 
 
 def vector_field_uncertainty(
     adata: AnnData,
-    pos: Dict[str, ndarray],
+    posterior_samples: Dict[str, ndarray],
     basis: str = "tsne",
     n_jobs: int = 1,
     denoised: bool = False,
 ) -> Tuple[ndarray, ndarray, ndarray]:
     """Run cosine similarity-based vector field across posterior samples"""
     import numpy as np
     import sklearn
@@ -645,47 +684,56 @@
     from astropy.stats import rayleightest
     from sklearn.pipeline import Pipeline
 
     # fig, ax = plt.subplots(10, 3)
     # fig.set_size_inches(16, 36)
     # ax = ax.flatten()
     v_map_all = []
-    if ("u_scale" in pos) and ("s_scale" in pos):  # Gaussian models
-        scale = pos["u_scale"] / pos["s_scale"]
-    elif ("u_scale" in pos) and not ("s_scale" in pos):  # Poisson Model 2
-        scale = pos["u_scale"]
+    if ("u_scale" in posterior_samples) and (
+        "s_scale" in posterior_samples
+    ):  # Gaussian models
+        scale = posterior_samples["u_scale"] / posterior_samples["s_scale"]
+    elif ("u_scale" in posterior_samples) and not (
+        "s_scale" in posterior_samples
+    ):  # Poisson Model 2
+        scale = posterior_samples["u_scale"]
     else:  # Poisson Model 1
         scale = 1
 
-    if "beta_k" in pos:
+    if "beta_k" in posterior_samples:
         velocity_samples = (
-            pos["ut"] * pos["beta_k"] / scale - pos["st"] * pos["gamma_k"]
+            posterior_samples["ut"] * posterior_samples["beta_k"] / scale
+            - posterior_samples["st"] * posterior_samples["gamma_k"]
         )
     else:
-        velocity_samples = pos["beta"] * pos["ut"] / scale - pos["gamma"] * pos["st"]
+        velocity_samples = (
+            posterior_samples["beta"] * posterior_samples["ut"] / scale
+            - posterior_samples["gamma"] * posterior_samples["st"]
+        )
 
     if denoised:
         projection = [
             ("PCA", sklearn.decomposition.PCA(random_state=99, n_components=50)),
             ("UMAP", umap.UMAP(random_state=99, n_components=2)),
         ]
         pipelines = Pipeline(projection)
-        expression = [pos["st"].mean(0)]
+        expression = [posterior_samples["st"].mean(0)]
         pipelines.fit(expression[0])
         umap_orig = pipelines.transform(expression[0])
         adata.obsm["X_umap1"] = umap_orig
         joint_pcs = pipelines.steps[0][1].transform(expression[0])
         adata.obsm["X_pyropca"] = joint_pcs
         scv.pp.neighbors(adata, use_rep="pyropca")
     else:
         scv.pp.neighbors(adata, use_rep="pca")
     ##scv.pp.neighbors(adata, use_rep=basis)
 
-    for sample in range(30):
-        adata.layers["spliced_pyro"] = pos["st"][sample]
+    assert len(posterior_samples["st"].shape) == 3
+    for sample in range(posterior_samples["st"].shape[0]):
+        adata.layers["spliced_pyro"] = posterior_samples["st"][sample]
         adata.layers["velocity_pyro"] = velocity_samples[sample]
         adata.var["velocity_genes"] = True
         scv.tl.velocity_graph(
             adata, vkey="velocity_pyro", xkey="spliced_pyro", n_jobs=n_jobs
         )
         scv.tl.velocity_embedding(adata, vkey="velocity_pyro", basis=basis)
         v_map_all.append(adata.obsm[f"velocity_pyro_{basis}"])
@@ -714,66 +762,87 @@
     y_values = y_values.reshape(-1, 1)
     return x_values[np.argmin(np.abs(y_values - angle_std), axis=0)]
 
 
 def plot_vector_field_uncertain(
     adata,
     embed_mean,
-    embeds_radian,
+    embeds_radian_or_magnitude,
     fig=None,
     cbar=True,
     basis="umap",
     scale=0.002,
     cbar_pos=[0.22, 0.28, 0.5, 0.05],
     p_mass_min=3.5,
     only_grid=False,
     ax=None,
     autoscale=False,
     density=0.3,
     arrow_size=5,
+    uncertain_measure="angle",
 ):
     from scvelo.plotting.velocity_embedding_grid import default_arrow
 
     if not only_grid:
         if ax is None:
             ax = fig.subplots(1, 2)
         dot_size = 1
         plt.rcParams["image.cmap"] = "winter"
         # norm = Normalize()
         # norm.autoscale(fdri_grids)
         # colormap = cm.inferno
 
-        adata.obs["uncertain"] = get_posterior_sample_angle_uncertainty(
-            embeds_radian / np.pi * 180
-        )
-        im = ax[0].scatter(
-            adata.obsm[f"X_{basis}"][:, 0],
-            adata.obsm[f"X_{basis}"][:, 1],
-            c=get_posterior_sample_angle_uncertainty(embeds_radian / np.pi * 180),
-            s=dot_size,
-            linewidth=0,
-            vmin=0,
-            vmax=360,
-            cmap="winter",
-        )
+        if uncertain_measure == "angle":
+            adata.obs["uncertain"] = get_posterior_sample_angle_uncertainty(
+                embeds_radian_or_magnitude / np.pi * 180
+            )
+            im = ax[0].scatter(
+                adata.obsm[f"X_{basis}"][:, 0],
+                adata.obsm[f"X_{basis}"][:, 1],
+                # c=get_posterior_sample_angle_uncertainty(embeds_radian_or_magnitude / np.pi * 180),
+                c=adata.obs["uncertain"].values,
+                s=dot_size,
+                linewidth=0,
+                vmin=0,
+                vmax=360,
+                cmap="winter",
+            )
+        else:
+            adata.obs["uncertain"] = embeds_radian_or_magnitude.std(axis=0)
+            norm = Normalize()
+            norm.autoscale(adata.obs["uncertain"])
+            colormap = cm.winter
+            im = ax[0].scatter(
+                adata.obsm[f"X_{basis}"][:, 0],
+                adata.obsm[f"X_{basis}"][:, 1],
+                # c=get_posterior_sample_angle_uncertainty(embeds_radian_or_magnitude / np.pi * 180),
+                c=colormap(norm(adata.obs["uncertain"].values)),
+                s=dot_size,
+                linewidth=0,
+                vmin=0,
+                vmax=360,
+                norm=Normalize(vmin=0, vmax=360),
+                cmap="winter",
+            )
+
         ax[0].axis("off")
-        ax[0].set_title("Single-cell\nvector field uncertainty ", fontsize=7)
+        ax[0].set_title(
+            f"Single-cell\nvector field {uncertain_measure} uncertainty ", fontsize=7
+        )
         ax = ax[1]
 
     X_grid, V_grid, uncertain = project_grid_points(
         adata.obsm[f"X_{basis}"],
         embed_mean,
-        get_posterior_sample_angle_uncertainty(embeds_radian / np.pi * 180),
+        # get_posterior_sample_angle_uncertainty(embeds_radian_or_magnitude / np.pi * 180),
+        adata.obs["uncertain"].values,
         p_mass_min=p_mass_min,
         autoscale=autoscale,
         density=density,
     )
-    # print(X_grid)
-    # print(V_grid)
-    # print(uncertain)
 
     # scale = None
     hl, hw, hal = default_arrow(arrow_size)
     print(hl, hw, hal)
     quiver_kwargs = {"angles": "xy", "scale_units": "xy"}
     quiver_kwargs.update({"width": 0.001, "headlength": hl / 2})
     quiver_kwargs.update({"headwidth": hw / 2, "headaxislength": hal / 2})
@@ -785,14 +854,15 @@
         adata.obsm[f"X_{basis}"][:, 0],
         adata.obsm[f"X_{basis}"][:, 1],
         s=1,
         linewidth=0,
         color="gray",
         alpha=0.2,
     )
+    print(adata.obs["uncertain"])
     im = ax.quiver(
         X_grid[:, 0],
         X_grid[:, 1],
         V_grid[:, 0],
         V_grid[:, 1],
         # uncertain,
         color=colormap(norm(uncertain)),
@@ -800,15 +870,15 @@
         edgecolors=colormap(norm(uncertain)),
         # edgecolors='black',
         norm=Normalize(vmin=0, vmax=360),
         cmap="winter",
         scale=scale,
         **quiver_kwargs,
     )
-    ax.set_title("Averaged\nvector field uncertainty ", fontsize=7)
+    ax.set_title(f"Averaged\nvector field {uncertain_measure} uncertainty ", fontsize=7)
     ax.axis("off")
     if cbar:
         from matplotlib.ticker import MaxNLocator
 
         # divider = make_axes_locatable(ax[1])
         # cax = divider.append_axes('bottom', size='5%', pad=0.08)
         # cbar = fig.colorbar(im, cax=cax, orientation="horizontal", shrink=0.6)
@@ -816,99 +886,114 @@
         ##fig.colorbar(im, ax=ax, shrink=0.6, location='bottom')
         # cbar.ax.set_xlabel("Angle uncertainty", fontsize=6)
         cbar_ax = fig.add_axes(cbar_pos)
         cbar = fig.colorbar(im, cax=cbar_ax, orientation="horizontal", shrink=0.8)
         # cbar.tick_params(axis='x', labelsize=6)
         cbar.ax.set_xticks([0, 180, 360], [0, 180, 360], fontsize=6)
         cbar.ax.locator = MaxNLocator(nbins=2, integer=True)
-        cbar.ax.set_xlabel("Angle uncertainty", fontsize=6)
+        cbar.ax.set_xlabel(f"{uncertain_measure} uncertainty", fontsize=6)
 
 
 def compute_mean_vector_field(
-    pos,
+    posterior_samples,
     adata,
     basis="umap",
     n_jobs=1,
     spliced="spliced_pyro",
     raw=False,
 ):
     scv.pp.neighbors(adata, use_rep="pca")
 
     adata.var["velocity_genes"] = True
 
     if spliced == "spliced_pyro":
         if raw:
-            ut = pos["ut"]
-            st = pos["st"]
+            ut = posterior_samples["ut"]
+            st = posterior_samples["st"]
             ut = ut / ut.sum(axis=-1, keepdims=True)
             st = st / st.sum(axis=-1, keepdims=True)
         else:
-            ut = pos["ut"]
-            st = pos["st"]
+            ut = posterior_samples["ut"]
+            st = posterior_samples["st"]
         adata.layers["spliced_pyro"] = st.mean(0).squeeze()
-        # if ('u_scale' in pos) and ('s_scale' in pos): # TODO: two scale for Normal distribution
-        if "u_scale" in pos:  # only one scale for Poisson distribution
+        # if ('u_scale' in posterior_samples) and ('s_scale' in posterior_samples): # TODO: two scale for Normal distribution
+        if "u_scale" in posterior_samples:  # only one scale for Poisson distribution
             adata.layers["velocity_pyro"] = (
-                ut * pos["beta"] / pos["u_scale"] - st * pos["gamma"]
+                ut * posterior_samples["beta"] / posterior_samples["u_scale"]
+                - st * posterior_samples["gamma"]
             ).mean(0)
         else:
-            if "beta_k" in pos:
+            if "beta_k" in posterior_samples:
                 adata.layers["velocity_pyro"] = (
-                    (ut * pos["beta_k"] - pos["st"] * pos["gamma_k"]).mean(0).squeeze()
+                    (
+                        ut * posterior_samples["beta_k"]
+                        - posterior_samples["st"] * posterior_samples["gamma_k"]
+                    )
+                    .mean(0)
+                    .squeeze()
                 )
             else:
                 adata.layers["velocity_pyro"] = (
-                    ut * pos["beta"] - pos["st"] * pos["gamma"]
+                    ut * posterior_samples["beta"]
+                    - posterior_samples["st"] * posterior_samples["gamma"]
                 ).mean(0)
         scv.tl.velocity_graph(
             adata, vkey="velocity_pyro", xkey="spliced_pyro", n_jobs=n_jobs
         )
     elif spliced in ["Ms"]:
         ut = adata.layers["Mu"]
         st = adata.layers["Ms"]
-        if ("u_scale" in pos) and ("s_scale" in pos):
+        if ("u_scale" in posterior_samples) and ("s_scale" in posterior_samples):
             adata.layers["velocity_pyro"] = (
-                ut * pos["beta"] / (pos["u_scale"] / pos["s_scale"]) - st * pos["gamma"]
+                ut
+                * posterior_samples["beta"]
+                / (posterior_samples["u_scale"] / posterior_samples["s_scale"])
+                - st * posterior_samples["gamma"]
             ).mean(0)
         else:
             adata.layers["velocity_pyro"] = (
-                ut * pos["beta"] - pos["st"] * pos["gamma"]
+                ut * posterior_samples["beta"]
+                - posterior_samples["st"] * posterior_samples["gamma"]
             ).mean(0)
         scv.tl.velocity_graph(adata, vkey="velocity_pyro", xkey="Ms", n_jobs=n_jobs)
     elif spliced in ["spliced"]:
         ut = adata.layers["unspliced"]
         st = adata.layers["spliced"]
-        if ("u_scale" in pos) and ("s_scale" in pos):
+        if ("u_scale" in posterior_samples) and ("s_scale" in posterior_samples):
             adata.layers["velocity_pyro"] = (
-                ut * pos["beta"] / (pos["u_scale"] / pos["s_scale"]) - st * pos["gamma"]
+                ut
+                * posterior_samples["beta"]
+                / (posterior_samples["u_scale"] / posterior_samples["s_scale"])
+                - st * posterior_samples["gamma"]
             ).mean(0)
         else:
             adata.layers["velocity_pyro"] = (
-                ut * pos["beta"] - pos["st"] * pos["gamma"]
+                ut * posterior_samples["beta"]
+                - posterior_samples["st"] * posterior_samples["gamma"]
             ).mean(0)
         scv.tl.velocity_graph(
             adata, vkey="velocity_pyro", xkey="spliced", n_jobs=n_jobs
         )
 
     scv.tl.velocity_embedding(adata, vkey="velocity_pyro", basis=basis)
 
 
 def plot_mean_vector_field(
-    pos,
+    posterior_samples,
     adata,
     ax,
     basis="umap",
     n_jobs=1,
     scale=0.2,
     density=0.4,
     spliced="spliced_pyro",
     raw=False,
 ):
     compute_mean_vector_field(
-        pos=pos,
+        posterior_samples=posterior_samples,
         adata=adata,
         basis=basis,
         n_jobs=n_jobs,
         spliced=spliced,
         raw=raw,
     )
     scv.pl.velocity_embedding_grid(
@@ -1091,34 +1176,38 @@
         cb.ax.yaxis.set_ticks_position("left")
     cb.update_ticks()
 
 
 def us_rainbowplot(
     genes: pd.Index,
     adata: AnnData,
-    pos: Dict[str, ndarray],
+    posterior_samples: Dict[str, ndarray],
     data: List[str] = ["st", "ut"],
     cell_state: str = "clusters",
 ) -> Figure:
     import matplotlib.lines as mlines
 
     fig, ax = plt.subplots(len(genes), 2)
     fig.set_size_inches(7, 14)
     n = 0
-    pos_s = pos[data[0]].mean(0).squeeze()
-    pos_u = pos[data[1]].mean(0).squeeze()
+    if data[0] in posterior_samples:
+        pos_s = posterior_samples[data[0]].mean(0).squeeze()
+        pos_u = posterior_samples[data[1]].mean(0).squeeze()
+    else:
+        pos_u = posterior_samples["ut_mean"]
+        pos_s = posterior_samples["st_mean"]
 
     for gene in genes:
         (index,) = np.where(adata.var_names == gene)
         ax1 = ax[n, 1]
         if n == 0:
             ax1.set_title("Rainbow plot")
         ress = pd.DataFrame(
             {
-                "cell_time": pos["cell_time"].mean(0).squeeze(),
+                "cell_time": posterior_samples["cell_time"].mean(0).squeeze(),
                 "cell_type": adata.obs[cell_state].values,
                 "spliced": pos_s[:, index].squeeze(),
                 "unspliced": pos_u[:, index].squeeze(),
             }
         )
         if n == 2:
             sns.scatterplot(
@@ -1161,15 +1250,15 @@
         # ax_twin.tick_params(labelbottom=False)
         # ax_twin.set_xlabel("")
         ax2 = ax[n, 0]
         ##divider = make_axes_locatable(ax2)
         ##cax = divider.append_axes('right', size='5%', pad=0.05)
         # ax2.set_ylabel("")
 
-        ##ress = pd.DataFrame({"cell_time": pos['cell_time'].mean(0).flatten(),
+        ##ress = pd.DataFrame({"cell_time": posterior_samples['cell_time'].mean(0).flatten(),
         ##                     "cell_type": adata.obs[cell_state].values,
         ##                     "unspliced": pos_u[:, index].flatten(),
         ##                     "spliced": pos_s[:, index].flatten()})
         ##im = ax2.scatter(pos_s[:, index], pos_u[:, index], c=ress.cell_time, s=25, cmap = 'seismic')
         ##fig.colorbar(im, cax=cax, orientation='vertical')
         ax2.set_title(gene)
         ax2.set_ylabel("")
@@ -1219,15 +1308,15 @@
     plt.subplots_adjust(hspace=0.8, wspace=0.6, left=0.1, right=0.91)
     return fig
 
 
 def rainbowplot(
     volcano_data,
     adata,
-    pos,
+    posterior_samples,
     fig=None,
     genes=None,
     data=["st", "ut"],
     cell_state="clusters",
     basis="umap",
     num_genes=5,
     add_line=True,
@@ -1239,15 +1328,15 @@
         genes = (
             volcano_data.sort_values("mean_mae", ascending=False)
             .head(300)
             .sort_values("time_correlation", ascending=negative)
             .head(num_genes)
             .index
         )
-    adata.layers["pyro_spliced"] = pos[data[0]].mean(0)
+    # adata.layers["pyro_spliced"] = posterior_samples[data[0]].mean(0)
     if fig is None:
         fig = plt.figure(figsize=(5.5, 4.5))
 
     if scvelo_colors:
         scv.pl.scatter(
             adata,
             basis=basis,
@@ -1271,26 +1360,34 @@
 
     subfigs = fig.subfigures(1, 2, wspace=0.0, width_ratios=[3, 1.5])
 
     ax = subfigs[0].subplots(len(genes), 2)
     ax_fig2 = subfigs[1].subplots(len(genes), 1)
 
     n = 0
-    st = pos[data[0]].mean(0)
-    ut = pos[data[1]].mean(0)
+    # st = posterior_samples[data[0]].mean(0)
+    # ut = posterior_samples[data[1]].mean(0)
+
+    if (data[0] in posterior_samples) and (data[1] in posterior_samples):
+        st = posterior_samples[data[0]].mean(0).squeeze()
+        ut = posterior_samples[data[1]].mean(0).squeeze()
+    else:
+        st = posterior_samples["st_mean"]
+        ut = posterior_samples["ut_mean"]
+
     for gene in genes:
         print(gene)
         (index,) = np.where(adata.var_names == gene)
         ax1 = ax[n, 1]
         ax2 = ax[n, 0]
         ax3 = ax_fig2[n]
         if n == 0:
             ax1.set_title("Rainbow plot", fontsize=7)
             ax2.set_title("Phase portrait", fontsize=7)
-        pos_mean_time = pos["cell_time"].mean(0).flatten()
+        pos_mean_time = posterior_samples["cell_time"].mean(0).flatten()
         print(pos_mean_time)
         ress = pd.DataFrame(
             {
                 "cell_time": pos_mean_time / pos_mean_time.max(),
                 "cell_type": adata.obs[cell_state].values,
                 "spliced": st[:, index].flatten(),
                 "unspliced": ut[:, index].flatten(),
@@ -1390,27 +1487,34 @@
     subfigs[0].text(
         0.552, 0.58, "spliced expression", size=7, rotation="vertical", va="center"
     )
     return fig
 
 
 def plot_state_uncertainty(
-    pos, adata, kde=True, data="denoised", top_percentile=0.9, ax=None, basis="umap"
+    posterior_samples,
+    adata,
+    kde=True,
+    data="denoised",
+    top_percentile=0.9,
+    ax=None,
+    basis="umap",
 ):
     if data == "denoised":
         adata.obs["state_uncertain"] = np.sqrt(
             (
-                (pos["st"] - pos["st"].mean(0)) ** 2
-                + (pos["ut"] - pos["ut"].mean(0)) ** 2
+                (posterior_samples["st"] - posterior_samples["st"].mean(0)) ** 2
+                + (posterior_samples["ut"] - posterior_samples["ut"].mean(0)) ** 2
             ).sum(-1)
         ).mean(0)
     else:
         adata.obs["state_uncertain"] = np.sqrt(
             (
-                (pos["s"] - pos["s"].mean(0)) ** 2 + (pos["u"] - pos["u"].mean(0)) ** 2
+                (posterior_samples["s"] - posterior_samples["s"].mean(0)) ** 2
+                + (posterior_samples["u"] - posterior_samples["u"].mean(0)) ** 2
             ).sum(-1)
         ).mean(0)
 
     ax = scv.pl.scatter(
         adata,
         basis=basis,
         color="state_uncertain",
```

### Comparing `pyrovelocity-0.1.1/setup.py` & `pyrovelocity-0.1.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,465 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyrovelocity
+Version: 0.1.2
+Summary: A multivariate RNA Velocity model to estimate future cell states with uncertainty using probabilistic modeling with pyro.
+Home-page: https://github.com/pinellolab/pyrovelocity
+License: AGPL-3.0-only
+Author: Qian Qin
+Author-email: qqin@mgh.harvard.edu
+Requires-Python: >=3.9,<3.11
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: dev
+Requires-Dist: Pygments (>=2.15.0) ; extra == "dev"
+Requires-Dist: adjusttext (>=0.7.3,<0.8.0)
+Requires-Dist: anndata (==0.8.0)
+Requires-Dist: astropy (==5.2.2)
+Requires-Dist: black (>=23.3.0) ; extra == "dev"
+Requires-Dist: click (>=8.0.1)
+Requires-Dist: colorlog (>=6.7.0,<7.0.0)
+Requires-Dist: cospar (==0.1.9)
+Requires-Dist: coverage[toml] (>=6.2) ; extra == "dev"
+Requires-Dist: darglint (>=1.8.1) ; extra == "dev"
+Requires-Dist: desert (>=2022.9.22)
+Requires-Dist: dparse (>=0.5.2) ; extra == "dev"
+Requires-Dist: dvc-gs (>=2.20.0) ; extra == "dev"
+Requires-Dist: flake8 (>=4.0.1) ; extra == "dev"
+Requires-Dist: flake8-bandit (>=2.1.2) ; extra == "dev"
+Requires-Dist: flake8-bugbear (>=21.9.2) ; extra == "dev"
+Requires-Dist: flake8-docstrings (>=1.6.0) ; extra == "dev"
+Requires-Dist: flake8-rst-docstrings (>=0.2.5) ; extra == "dev"
+Requires-Dist: furo (>=2023.3.27) ; extra == "dev"
+Requires-Dist: h5py (==3.8.0)
+Requires-Dist: hydra-core (==1.3.2)
+Requires-Dist: hydra-zen (>=0.10.0)
+Requires-Dist: hypothesis (>=6.71.0) ; extra == "dev"
+Requires-Dist: ipython (>=8.11.0) ; extra == "dev"
+Requires-Dist: isort (>=5.10.1) ; extra == "dev"
+Requires-Dist: jupyter-core (>=5.1.3) ; extra == "dev"
+Requires-Dist: leidenalg (==0.9.1)
+Requires-Dist: marshmallow (>=3.18.0)
+Requires-Dist: mlflow (==2.2.2)
+Requires-Dist: mypy (>=0.930) ; extra == "dev"
+Requires-Dist: myst-parser (>=1.0.0) ; extra == "dev"
+Requires-Dist: omegaconf (==2.3.0)
+Requires-Dist: pandas (==1.5.3)
+Requires-Dist: pep8-naming (>=0.12.1) ; extra == "dev"
+Requires-Dist: poethepoet (>=0.16.0) ; extra == "dev"
+Requires-Dist: pre-commit (>=2.16.0) ; extra == "dev"
+Requires-Dist: pre-commit-hooks (>=4.1.0) ; extra == "dev"
+Requires-Dist: pyro-ppl (==1.8.3)
+Requires-Dist: pytest (>=6.2.5) ; extra == "dev"
+Requires-Dist: pytest-cov (>=4.0.0) ; extra == "dev"
+Requires-Dist: pytest-mock (>=3.10.0) ; extra == "dev"
+Requires-Dist: pytorch-lightning (==1.9.4)
+Requires-Dist: pyupgrade (>=2.29.1) ; extra == "dev"
+Requires-Dist: pyvis (>=0.3.2) ; extra == "dev"
+Requires-Dist: rich (>=12.6.0,<13.0.0)
+Requires-Dist: safety (>=1.10.3) ; extra == "dev"
+Requires-Dist: scikit-misc (==0.1.4)
+Requires-Dist: scipy (==1.10.1)
+Requires-Dist: scvelo (==0.2.5)
+Requires-Dist: scvi-tools (==0.20.3)
+Requires-Dist: seaborn (==0.11.2)
+Requires-Dist: sphinx (>=6.1.3) ; extra == "dev"
+Requires-Dist: sphinx-autobuild (>=2021.3.14) ; extra == "dev"
+Requires-Dist: sphinx-click (>=4.4.0) ; extra == "dev"
+Requires-Dist: termcolor (>=2.2.0,<3.0.0)
+Requires-Dist: torch (==1.13.1)
+Requires-Dist: torchmetrics (==0.11.4)
+Requires-Dist: typeguard (>=2.13.3) ; extra == "dev"
+Requires-Dist: xdoctest[colors] (>=0.15.10) ; extra == "dev"
+Project-URL: Changelog, https://github.com/pinellolab/pyrovelocity/releases
+Project-URL: Documentation, https://pyrovelocity.readthedocs.io
+Project-URL: Repository, https://github.com/pinellolab/pyrovelocity
+Description-Content-Type: text/markdown
 
-packages = \
-['pyrovelocity']
+# Pyro-Velocity
 
-package_data = \
-{'': ['*']}
+<div align="center">
 
-install_requires = \
-['adjusttext>=0.7.3,<0.8.0',
- 'anndata==0.7.5',
- 'astropy==5.1',
- 'click>=8.0.1',
- 'colorlog>=6.7.0,<7.0.0',
- 'cospar==0.1.9',
- 'desert>=2022.9.22',
- 'h5py==3.7.0',
- 'hydra-core==1.2.0',
- 'leidenalg==0.9.0',
- 'marshmallow>=3.18.0',
- 'mlflow==1.30.0',
- 'omegaconf>=2.2.3,<3.0.0',
- 'pyro-ppl==1.6.0',
- 'pytorch-lightning==1.3.0',
- 'rich>=12.6.0,<13.0.0',
- 'scikit-misc==0.1.4',
- 'scipy==1.9.3',
- 'scvelo==0.2.4',
- 'scvi-tools==0.13.0',
- 'seaborn==0.11.2',
- 'torch==1.8.1',
- 'torchmetrics==0.5.1']
-
-extras_require = \
-{'dev': ['Pygments>=2.10.0',
-         'black>=21.10b0',
-         'coverage[toml]>=6.2',
-         'darglint>=1.8.1',
-         'flake8>=4.0.1',
-         'flake8-bandit>=2.1.2',
-         'flake8-bugbear>=21.9.2',
-         'flake8-docstrings>=1.6.0',
-         'flake8-rst-docstrings>=0.2.5',
-         'furo>=2021.11.12',
-         'isort>=5.10.1',
-         'mypy>=0.930',
-         'pep8-naming>=0.12.1',
-         'pre-commit>=2.16.0',
-         'pre-commit-hooks>=4.1.0',
-         'pytest>=6.2.5',
-         'pyupgrade>=2.29.1',
-         'safety>=1.10.3',
-         'sphinx>=4.3.2',
-         'sphinx-autobuild>=2021.3.14',
-         'sphinx-click>=3.0.2',
-         'typeguard>=2.13.3',
-         'xdoctest[colors]>=0.15.10',
-         'myst-parser>=0.16.1',
-         'dparse>=0.5.2',
-         'pytest-cov>=4.0.0,<5.0.0',
-         'pytest-mock>=3.10.0,<4.0.0',
-         'poethepoet>=0.16.0,<0.17.0',
-         'dvc-gs>=2.20.0,<3.0.0',
-         'jupyter-core>=5.1.3,<6.0.0']}
-
-entry_points = \
-{'console_scripts': ['pyrovelocity = pyrovelocity.pyrovelocity:main']}
-
-setup_kwargs = {
-    'name': 'pyrovelocity',
-    'version': '0.1.1',
-    'description': 'A multivariate RNA Velocity model to estimate future cell states with uncertainty using probabilistic modeling with pyro.',
-    'long_description': '# pyrovelocity\n\n<div align="center">\n\n<img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/_static/logo.png" alt="Pyro-Velocity logo" width="300" role="img">\n\n|         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |\n| ------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| CI/CD   | [![CI - Test](https://github.com/pinellolab/pyrovelocity/actions/workflows/tests.yml/badge.svg)](https://github.com/pinellolab/pyrovelocity/actions/workflows/tests.yml) [![CML](https://github.com/pinellolab/pyrovelocity/actions/workflows/cml.yml/badge.svg)](https://github.com/pinellolab/pyrovelocity/actions/workflows/cml.yml) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/pinellolab/pyrovelocity/master.svg)](https://results.pre-commit.ci/latest/github/pinellolab/pyrovelocity/master) |\n| Docs    | [![Documentation Status](https://readthedocs.org/projects/pyrovelocity/badge/?version=latest)](https://pyrovelocity.readthedocs.io/en/latest/?badge=latest)                                                                                                                                                                                                                                                                                                                                                                  |\n| Package | [![PyPI - Version](https://img.shields.io/pypi/v/pyrovelocity.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/pyrovelocity/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyrovelocity.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/pyrovelocity/)                                                                                                                                                                                                          |\n| Meta    | [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![License - MIT](https://img.shields.io/badge/license-AGPL%203-purple)](https://spdx.org/licenses/)                                                                                                                                                                                                                                                                                                       |\n\n</div>\n\n---\n\n# Introduction\n\n`Pyro-Velocity` is a Bayesian, generative, and multivariate RNA velocity\nmodel to estimate _uncertainty_ in predictions of future cell states from\nminimal models approximating splicing dynamics.\nThis approach models _raw sequencing counts_ with _synchronized cell time_ across\nall expressed genes to provide quantifiable information on\ncell fate choice and developmental trajectory dynamics.\n\n## Features\n\n- Probabilistic modeling of RNA velocity\n- Direct modeling of raw spliced and unspliced read count\n- Multiple uncertainty diagnostics analysis and visualizations\n- Synchronized cell time estimation across genes\n- Multivariate denoised gene expression and velocity prediction\n\n<!-- ![Velocity workflow comparison](docs/source/readme_figure1.png) -->\n<img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/source/readme_figure1.png" alt="Velocity workflow comparison">\n\n## Installation with miniconda\n\nPlease install miniconda following the instructions here: <https://docs.conda.io/en/latest/miniconda.html>, this step takes about 1-2 mins.\n\n```bash\nwget -c https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh\nbash Miniconda3-latest-Linux-x86_64.sh\n# then follow the instruction to setup the conda base environment\n```\n\nAfter the conda has been setup, logout and re-login to install _mamba_ to speed up installation, this step takes about 20s.\n\n```bash\nconda install -c conda-forge mamba\n```\n\nThen add the channels, this step takes 1~2s.\n\n```bash\nconda config --add channels defaults\nconda config --add channels bioconda\nconda config --add channels conda-forge\nconda config --set channel_priority flexible\n```\n\nAfter that, install the _pyrovelocity_ package in one mamba command:\n\n```bash\nmamba create -n pyrovelocity_bioconda -c bioconda pyrovelocity\n```\n\nThis step takes about 6-8 minutes depending on the network speed. If you prefer to use conda environment configurations, see the `conda` subfolder for installation with _prefix_ to specify the installation path, such as:\n\n```\n# GPU\nmamba env create --prefix /path_to_conda_env/qq-pyrovelocity-dev -f conda/environment-gpu.yml\n# or CPU\nmamba env create --prefix /path_to_conda_env/qq-pyrovelocity-dev -f conda/environment-cpu.yml\n```\n\nOr with more control of installing the environment,\n\n```bash\nconda create -n pyrovelocity_bioconda python=3.8.8\nmamba install -n pyrovelocity_bioconda -c bioconda pyrovelocity\n# CPU\nmamba env update -n pyrovelocity_bioconda -f conda/environment-cpu.yml\n# or GPU\nmamba env update -n pyrovelocity_bioconda -f conda/environment-gpu.yml\n```\n\nFor windows user installation, please refer to the [issue](https://github.com/pinellolab/pyrovelocity/issues/9).\n\nLastly, test the installation by:\n\n```bash\nconda activate pyrovelocity_bioconda\npython\n```\n\n```python\nimport pyrovelocity\n```\n\n## Additional packages necessary to reproduce all the analyses presented in the notebooks\n\n```bash\npip install cospar==0.1.9\n```\n\n## Quick start\n\nAfter the installation, let\\\'s look at your dataset to see how\nPyro-Velocity can help understand cell dynamics.\n\nStarting from raw sequencing FASTQ files, obtained for example with\nSMART-seq, 10X genomics, inDrop or other similar single-cell assays, you\ncan preprocess the data to generate spliced and unspliced gene count\ntables in h5ad file (or loom file using cellranger+velocyto or the\nkallisto pipeline.\n\nStarting from these count tables we show below a minimal step-by-step\nworkflow to illustrate the main features of Pyro-Velocity in a Jupyter\nNotebook:\n\nStep 0. Even though _pyrovelocity_ is a cluster-free method to evaluate uncertainty\nof cell fate, it will dependend on 2 dimensional embedding results for evaluation of\nuncertainty and generate visualization, we would suggest run your new datasets using\n[scanpy tutorial](https://scanpy-tutorials.readthedocs.io/en/latest/pbmc3k.html).\n\nStep 1. Load your data, load your data(e.g. _local_file.h5ad_) with\nscvelo by using:\n\n```python\nimport scvelo as scv\nadata = scv.read("local_file.h5ad")\n```\n\nStep 2. Minimally preprocess your _adata_ object:\n\n```python\nadata.layers[\'raw_spliced\']   = adata.layers[\'spliced\']\nadata.layers[\'raw_unspliced\'] = adata.layers[\'unspliced\']\nadata.obs[\'u_lib_size_raw\'] = adata.layers[\'raw_unspliced\'].toarray().sum(-1)\nadata.obs[\'s_lib_size_raw\'] = adata.layers[\'raw_spliced\'].toarray().sum(-1)\nscv.pp.filter_and_normalize(adata, min_shared_counts=30, n_top_genes=2000)\nscv.pp.moments(adata, n_pcs=30, n_neighbors=30)\n```\n\nStep 3. Train the Pyro-Velocity model:\n\n```python\nfrom pyrovelocity.api import train_model\n# Model 1\nnum_epochs = 1000 # large data\n# num_epochs = 4000 # small data\nadata_model_pos = train_model(adata,\n                               max_epochs=num_epochs, svi_train=True, log_every=100,\n                               patient_init=45,\n                               batch_size=4000, use_gpu=0, cell_state=\'state_info\',\n                               include_prior=True,\n                               offset=False,\n                               library_size=True,\n                               patient_improve=1e-3,\n                               model_type=\'auto\',\n                               guide_type=\'auto_t0_constraint\',\n                               train_size=1.0)\n\n# Or Model 2\nadata_model_pos = train_model(adata,\n                               max_epochs=num_epochs, svi_train=True, log_every=100,\n                               patient_init=45,\n                               batch_size=4000, use_gpu=0, cell_state=\'state_info\',\n                               include_prior=True,\n                               offset=True,\n                               library_size=True,\n                               patient_improve=1e-3,\n                               model_type=\'auto\',\n                               guide_type=\'auto\',\n                               train_size=1.0)\n\n# adata_model_pos is a returned list in which 0th element is the trained model,\n# the 1st element is the posterior samples of all random variables\nsave_res = True\nif save_res:\n    adata_model_pos[0].save(\'saved_model\', overwrite=True)\n    result_dict = {"adata_model_pos": adata_model_pos[1],\n                   "v_map_all": v_map_all,\n                   "embeds_radian": embeds_radian, "fdri": fdri, "embed_mean": embed_mean}\n    import pickle\n    with open("model_posterior_samples.pkl", "wb") as f:\n         pickle.dump(result_dict, f)\n```\n\nStep 4: Generate Pyro-Velocity\'s vector field and shared time plots\nwith uncertainty estimation.\n\n```python\nfrom pyrovelocity.plot import plot_state_uncertainty\nfrom pyrovelocity.plot import plot_posterior_time, plot_gene_ranking,\\\n      vector_field_uncertainty, plot_vector_field_uncertain,\\\n      plot_mean_vector_field, project_grid_points,rainbowplot,denoised_umap,\\\n      us_rainbowplot, plot_arrow_examples\n\nembedding = \'emb\' # change to umap or tsne based on your embedding method\n\n# This generates the posterior samples of all vector fields\n# and statistical testing results from Rayleigh test\nv_map_all, embeds_radian, fdri = vector_field_uncertainty(adata, adata_model_pos[1],\n                                                          basis=embedding, denoised=False, n_jobs=30)\nfig, ax = plt.subplots()\n# This returns the posterior mean of the vector field\nembed_mean = plot_mean_vector_field(adata_model_pos[1], adata, ax=ax, n_jobs=30, basis=embedding)\n# This plot single-cell level vector field uncertainty\n# and averaged cell vector field uncertainty on the grid points\n# based on angular standard deviation\nfig, ax = plt.subplots(1, 2)\nfig.set_size_inches(11.5, 5)\nplot_vector_field_uncertain(adata, embed_mean, embeds_radian,\n                            ax=ax,\n                            fig=fig, cbar=False, basis=embedding, scale=None)\n\n# This generates shared time uncertainty plot with contour lines\nfig, ax = plt.subplots(1, 3)\nfig.set_size_inches(12, 2.8)\nadata.obs[\'shared_time_uncertain\'] = adata_model_pos[1][\'cell_time\'].std(0).flatten()\nax_cb = scv.pl.scatter(adata, c=\'shared_time_uncertain\', ax=ax[0], show=False, cmap=\'inferno\', fontsize=7, s=20, colorbar=True, basis=embedding)\nselect = adata.obs[\'shared_time_uncertain\'] > np.quantile(adata.obs[\'shared_time_uncertain\'], 0.9)\nsns.kdeplot(adata.obsm[f\'X_{embedding}\'][:, 0][select],\n            adata.obsm[f\'X_{embedding}\'][:, 1][select],\n            ax=ax[0], levels=3, fill=False)\n\n# This generates vector field uncertainty based on Rayleigh test.\nadata.obs.loc[:, \'vector_field_rayleigh_test\'] = fdri\nim = ax[1].scatter(adata.obsm[f\'X_{basis}\'][:, 0],\n                   adata.obsm[f\'X_{basis}\'][:, 1], s=3, alpha=0.9,\n                   c=adata.obs[\'vector_field_rayleigh_test\'], cmap=\'inferno_r\',\n                   linewidth=0)\nset_colorbar(im, ax[1], labelsize=5, fig=fig, position=\'right\')\nselect = adata.obs[\'vector_field_rayleigh_test\'] > np.quantile(adata.obs[\'vector_field_rayleigh_test\'], 0.95)\nsns.kdeplot(adata.obsm[f\'X_{embedding}\'][:, 0][select],\n            adata.obsm[f\'X_{embedding}\'][:, 1][select], ax=ax[1], levels=3, fill=False)\nax[1].axis(\'off\')\nax[1].set_title("vector field\\nrayleigh test\\nfdr<0.05: %s%%" % (round((fdri < 0.05).sum()/fdri.shape[0], 2)*100), fontsize=7)\n```\n\nStep 5: Prioritize putative cell fate marker genes based on negative\nmean absolute errors and pearson correlation between denoised spliced\nexpression and posterior mean shared time, and then visualize the top\none with rainbow plots\n\n```python\nfig = plt.figure(figsize=(7.07, 4.5))\nsubfig = fig.subfigures(1, 2, wspace=0.0, hspace=0, width_ratios=[1.6, 4])\nax = fig.subplots(1)\n# This generates the selected cell fate markers and output in DataFrame\nvolcano_data, _ = plot_gene_ranking([adata_model_pos[1]], [adata], ax=ax,\n                                     time_correlation_with=\'st\', assemble=True)\n# This generates the rainbow plots for the selected markers.\n_ = rainbowplot(volcano_data, adata, adata_model_pos[1],\n                subfig[1], data=[\'st\', \'ut\'], num_genes=4)\n```\n\n## Illustrative examples of Pyro-Velocity analyses on different single-cell datasets\n\n### Pyro-Velocity applied to a PBMC dataset \\[[1](https://scvelo.readthedocs.io/perspectives/Perspectives/)\\]\n\nThis is a scRNA-seq dataset of fully mature peripheral blood mononuclear\ncells (PBMC) generated using the 10X genomics kit and containing 65,877\ncells with 11 fully differentiated immune cell types. This dataset\ndoesn\\\'t contain stem and progenitor cells or other signature of and\nundergoing dynamical differentiation, thus no consistent velocity flow\nshould be detected.\n\nBelow we show the main output generated by Pyro-Velocity Model 1\nanalysis. Pyro-Velocity failed to detect high-confidence trajectories in\nthe mature blood cell states, consistent with what is known about the\nbiology underlying these cells.\n\n**Vector field with uncertainty**\n\n<!-- ![PBMC vector field uncertainty](docs/source/readme_figure2.png) -->\n<img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/source/readme_figure2.png" alt="PBMC vector field uncertainty">\n\nThese 6 plots from left to right show: 1. cell types, 2. stream plot of\nPyro-velocity vector field based on the posterior mean of 30 posterior\nsamples, 3. single cell vector field examples showing all 30 posterior\nsamples as vectors for 3 arbitrarily selected cells; 4. single cell\nvector field with uncertainty based on angular standard deviation across\n30 posterior samples, 5. averaged vector field uncertainty from 4. 6.\nRayleigh test of posterior samples vector field, the title shows the\nexpected false discovery rate using a 5% threshold.\n\nThe full example can be reproduced using the\n[PBMC](https://github.com/pinellolab/pyrovelocity/blob/master/docs/source/notebooks/pbmc.ipynb)\nJupyter notebook.\n\n### Pyro-Velocity applied to a pancreas development dataset \\[[2](https://scvelo.readthedocs.io/VelocityBasics/)\\]\n\nHere we apply Pyro-Velocity to a single cell RNA-seq dataset of mouse\npancreas in the E15.5 embryo developmental stage. This dataset was\ngenerated using the 10X genomics kit and contains 3,696 cells with 8\ncell types including progenitor cells, intermediate and terminal cell\nstates.\n\nBelow we show the main output generated by Pyro-Velocity Model 1\nanalysis. Pyro-Velocity was able to define well-known developmental cell\nhierarchies identifying cell trajectories originating from ductal\nprogenitor cells and culminated in the production of mature Alpha, Beta,\nDelta, and Epsilon cells.\n\n**Vector field with uncertainty**\n\n<!-- ![Pancreas vector field uncertainty](docs/source/readme_figure3.png) -->\n<img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/source/readme_figure3.png" alt="Pancreas vector field uncertainty">\n\nThese 6 plots from left to right are showing the same analyses presented\nas in the example above.\n\n**Shared time with uncertainty**\n\n<!-- ![Pancreas shared time uncertainty](docs/source/readme_figure4.png) -->\n<img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/source/readme_figure4.png" alt="Pancreas vector field uncertainty">\n\nThe left figure shows the average of 30 posterior samples for the cell\nshared time, the title of the figure shows the Spearman\\\'s correlation\nwith the Cytotrace score, an orthogonal state-of-the-art method used to\npredict cell differentiation based on the number of expressed genes per\ncell (Gulati et. al, Science 2020). The right figure shows the standard\ndeviation across posterior samples of shared time.\n\n**Gene selection and visualization**\n\nTo uncover potential cell fate determinant markers genes of the mouse\npancreas, we first select the top 300 genes with the best velocity model\nfit (we use negative mean absolute error ), then we rank the filtered\ngenes using Pearson\\\'s correlation between denoised spliced expression\nand the posterior mean of the recovered shared time across cells.\n\n<!-- ![Pancreas Volcano plot for gene selection](docs/source/readme_figure6.png) -->\n<img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/source/readme_figure6.png" alt="Pancreas Volcano plot for gene selection">\n\nFor the selected genes, it is possible to explore in depth their\ndynamic, using phase portraits, rainbow plots, and UMAP rendering of\ndenoised splicing gene expression across cells.\n\n<!-- ![Pancreas vector field uncertainty](docs/source/readme_figure7.png) -->\n<img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/source/readme_figure7.png" alt="Pancreas vector field uncertainty">\n\nThe full example can be reproduced using the\n[Pancreas](https://github.com/pinellolab/pyrovelocity/blob/master/docs/source/notebooks/pancreas.ipynb)\njupyter notebook.\n\n### Pyro-Velocity applied to the LARRY dataset \\[[3](https://figshare.com/articles/dataset/larry_invitro_adata_sub_raw_h5ad/20780344)\\]\n\nThis last example, present the analysis of a recent scRNA-seq dataset\nprofiling mouse hematopoises at high resolution thanks to lineage\nrelationship information captured by the Lineage And RNA RecoverY\n(LARRY) system. LARRY leverages unique lentiviral barcodes that enables\nto clonally trace cell fates over time (Weinrab et al. Cell 20).\n\nBelow we show the main output generated by Pyro-Velocity analysis.\n\n**Vector field with uncertainty**\n\n<!-- ![LARRY vector field uncertainty](docs/source/readme_figure8.png) -->\n<img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/source/readme_figure8.png" alt="LARRY vector field uncertainty">\n\nThese 5 plots from left to right shows: 1) Cell types, 2) Clone\nprogression vector field by using centroid of cells belonging to the\nsame barcode for generating directed connection between consecutive\nphysical times, 3) single cell vector field with uncertainty based on\nangular standard deviation across 30 posterior samples, 4. averaged\nvector field uncertainty from 3. 5. Rayleigh test of posterior samples\nvector field, the title shows the false discovery rate using threshold\n5%.\n\n**Shared time with uncertainty**\n\nTo quantitatively assess the quality of the the receovered shared time\nwe also considered the agreement of our method with Cospar, a\nstate-of-the-art method specifically designed for predicting fate\npotency based on LARRY data.\n\n<!-- ![Pancreas shared time uncertainty](docs/source/readme_figure9.png) -->\n<img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/source/readme_figure9.png" alt="Pancreas shared time uncertainty">\n\nThe leftmost figure shows the Cospar fate potency score, the middle\nfigure shows the average of 30 posterior samples from Pyro-Velocity\nshared time per cell, the title of the figure shows the Spearman\'s\ncorrelation between cell latent shared time and fate potency scores\nderived from Cospar, the right figure shows the standard deviation\nacross posterior samples of shared time.\n\nThe full example can be reproduced using the\n[LARRY](https://github.com/pinellolab/pyrovelocity/blob/master/docs/source/notebooks/larry.ipynb)\njupyter notebook.\n\n# Troubleshooting\n\n## TypeError: fate_potency() got an unexpected keyword argument \'used_Tmap\'\n\nPlease use the specific _cospar_ version:\n\n```bash\npip install cospar==0.1.9\n```\n\n## CUDA error: no kernel image is available for execution on the device\n\nAll reference to GPU support applies to linux. We do not currently support windows\nand there is no GPU-compatible pytorch version `<1.12` for darwin.\nOn linux, either use [conda](./conda) (as exemplified in\n[reproducibility/environment](./reproducibility/environment)),\nor install the specific cuda-enabled pytorch version manually\n\n```bash\npip3 install torch==1.8.1+cu111 -f https://download.pytorch.org/whl/torch_stable.html\n```\n\nIf you are using poetry, you can also use the poetry helper\n\n```bash\npoetry install && poetry run poe force-cuda11\n```\n\nAlso see [contributing](./docs/contributing.md).\n',
-    'author': 'Qian Qin',
-    'author_email': 'qqin@mgh.harvard.edu',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/pinellolab/pyrovelocity',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8.8,<3.9.0',
-}
+<img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/_static/logo.png" alt="Pyro-Velocity logo" width="300" role="img">
 
+|         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
+| ------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| CI/CD   | [![CI - Test](https://github.com/pinellolab/pyrovelocity/actions/workflows/tests.yml/badge.svg)](https://github.com/pinellolab/pyrovelocity/actions/workflows/tests.yml) [![CML](https://github.com/pinellolab/pyrovelocity/actions/workflows/cml.yml/badge.svg)](https://github.com/pinellolab/pyrovelocity/actions/workflows/cml.yml) [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/pinellolab/pyrovelocity/master.svg)](https://results.pre-commit.ci/latest/github/pinellolab/pyrovelocity/master) |
+| Docs    | [![Documentation Status](https://readthedocs.org/projects/pyrovelocity/badge/?version=latest)](https://pyrovelocity.readthedocs.io/en/latest/?badge=latest) [![Preprint](https://img.shields.io/badge/doi-10.1101/2022.09.12.507691v2-B31B1B)](https://doi.org/10.1101/2022.09.12.507691)                                                                                                                                                                                                                                    |
+| Package | [![PyPI - Version](https://img.shields.io/pypi/v/pyrovelocity.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/pyrovelocity/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyrovelocity.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/pyrovelocity/) [![Docker iamge](https://img.shields.io/badge/docker-image-blue?logo=docker)](https://github.com/pinellolab/pyrovelocity/pkgs/container/pyrovelocity)                                                    |
+| Meta    | [![codecov](https://codecov.io/gh/pinellolab/pyrovelocity/branch/master/graph/badge.svg)](https://codecov.io/gh/pinellolab/pyrovelocity) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![License - MIT](https://img.shields.io/badge/license-AGPL%203-purple)](https://spdx.org/licenses/)                                                                                                                                                              |
+
+</div>
+
+---
+
+`Pyro-Velocity` is a Bayesian, generative, and multivariate RNA velocity
+model to estimate _uncertainty_ in predictions of future cell states from
+minimal models approximating splicing dynamics.
+This approach models _raw sequencing counts_ with _synchronized cell time_ across
+all expressed genes to provide quantifiable information on
+cell fate choice and developmental trajectory dynamics.
+
+## Features
+
+- Probabilistic modeling of RNA velocity
+- Direct modeling of raw spliced and unspliced read count
+- Multiple uncertainty diagnostics analysis and visualizations
+- Synchronized cell time estimation across genes
+- Multivariate denoised gene expression and velocity prediction
+
+<!-- ![Velocity workflow comparison](docs/source/readme_figure1.png) -->
+<img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/source/readme_figure1.png" alt="Velocity workflow comparison">
+
+## Installation
+
+### Development
+
+We currently support installation and usage in a linux 64-bit development environment with access to a GPU.
+An [IaC](https://en.wikipedia.org/wiki/Infrastructure_as_code) setup that works with [GCP](https://registry.terraform.io/providers/hashicorp/google/latest/docs) is documented in [reproducibility/environment/README.md](reproducibility/environment/README.md).
+Before proceeding to setup a minimal development environment, please fork this repository and clone a copy of your fork to your development machine. Unless otherwise mentioned, all commands assume your current working directory is the root of your local copy of your fork of this repository.
+
+Please install mambaforge according to the instructions provided in [conda-forge/miniforge](https://github.com/conda-forge/miniforge#install).
+
+You can then create a development environment with
+
+```bash
+mamba env create [--prefix /path_to_conda_environment] -f conda/environment-gpu.yml
+```
+
+This step takes about 10 minutes depending on network speed.
+
+Make sure you are able to successfully activate the installed environment
+
+```bash
+conda activate pyrovelocity-gpu
+which python
+```
+
+by checking that the output of which python following activation refers to the python binary in the correct conda environment.
+
+You can then install a development copy with
+
+```
+pip install --no-deps -e .[dev]
+```
+
+If this is successful, you will be able to
+
+```python
+import pyrovelocity
+```
+
+from a python interpreter.
+
+### User
+
+Please see the [documentation](https://pyrovelocity.readthedocs.io/en/latest/installation.html).
+
+## Quick start
+
+After the installation, let\'s look at your dataset to see how
+Pyro-Velocity can help understand cell dynamics.
+
+Starting from raw sequencing FASTQ files, obtained for example with
+SMART-seq, 10X genomics, inDrop or other similar single-cell assays, you
+can preprocess the data to generate spliced and unspliced gene count
+tables in h5ad file (or loom file using cellranger+velocyto or the
+kallisto pipeline.
+
+Starting from these count tables we show below a minimal step-by-step
+workflow to illustrate the main features of Pyro-Velocity in a Jupyter
+Notebook:
+
+Step 0. Even though _pyrovelocity_ is a cluster-free method to evaluate uncertainty
+of cell fate, it will dependend on 2 dimensional embedding results for evaluation of
+uncertainty and generate visualization, we would suggest run your new datasets using
+[scanpy tutorial](https://scanpy-tutorials.readthedocs.io/en/latest/pbmc3k.html).
+
+Step 1. Load your data, load your data(e.g. _local_file.h5ad_) with
+scvelo by using:
+
+```python
+import scvelo as scv
+adata = scv.read("local_file.h5ad")
+```
+
+Step 2. Minimally preprocess your _adata_ object:
+
+```python
+adata.layers['raw_spliced']   = adata.layers['spliced']
+adata.layers['raw_unspliced'] = adata.layers['unspliced']
+adata.obs['u_lib_size_raw'] = adata.layers['raw_unspliced'].toarray().sum(-1)
+adata.obs['s_lib_size_raw'] = adata.layers['raw_spliced'].toarray().sum(-1)
+scv.pp.filter_and_normalize(adata, min_shared_counts=30, n_top_genes=2000)
+scv.pp.moments(adata, n_pcs=30, n_neighbors=30)
+```
+
+Step 3. Train the Pyro-Velocity model:
+
+```python
+from pyrovelocity.api import train_model
+# Model 1
+num_epochs = 1000 # large data
+# num_epochs = 4000 # small data
+adata_model_pos = train_model(adata,
+                               max_epochs=num_epochs, svi_train=True, log_every=100,
+                               patient_init=45,
+                               batch_size=4000, use_gpu=0, cell_state='state_info',
+                               include_prior=True,
+                               offset=False,
+                               library_size=True,
+                               patient_improve=1e-3,
+                               model_type='auto',
+                               guide_type='auto_t0_constraint',
+                               train_size=1.0)
+
+# Or Model 2
+adata_model_pos = train_model(adata,
+                               max_epochs=num_epochs, svi_train=True, log_every=100,
+                               patient_init=45,
+                               batch_size=4000, use_gpu=0, cell_state='state_info',
+                               include_prior=True,
+                               offset=True,
+                               library_size=True,
+                               patient_improve=1e-3,
+                               model_type='auto',
+                               guide_type='auto',
+                               train_size=1.0)
+
+# adata_model_pos is a returned list in which 0th element is the trained model,
+# the 1st element is the posterior samples of all random variables
+save_res = True
+if save_res:
+    trained_model.save('saved_model', overwrite=True)
+    result_dict = {"adata_model_pos": posterior_samples,
+                   "v_map_all": v_map_all,
+                   "embeds_radian": embeds_radian, "fdri": fdri, "embed_mean": embed_mean}
+    import pickle
+    with open("posterior_samples.pkl", "wb") as f:
+         pickle.dump(result_dict, f)
+```
+
+Step 4: Generate Pyro-Velocity's vector field and shared time plots
+with uncertainty estimation.
+
+```python
+from pyrovelocity.plot import plot_state_uncertainty
+from pyrovelocity.plot import plot_posterior_time, plot_gene_ranking,\
+      vector_field_uncertainty, plot_vector_field_uncertain,\
+      plot_mean_vector_field, project_grid_points,rainbowplot,denoised_umap,\
+      us_rainbowplot, plot_arrow_examples
+
+embedding = 'emb' # change to umap or tsne based on your embedding method
+
+# This generates the posterior samples of all vector fields
+# and statistical testing results from Rayleigh test
+v_map_all, embeds_radian, fdri = vector_field_uncertainty(adata, posterior_samples,
+                                                          basis=embedding, denoised=False, n_jobs=30)
+fig, ax = plt.subplots()
+# This returns the posterior mean of the vector field
+embed_mean = plot_mean_vector_field(posterior_samples, adata, ax=ax, n_jobs=30, basis=embedding)
+# This plot single-cell level vector field uncertainty
+# and averaged cell vector field uncertainty on the grid points
+# based on angular standard deviation
+fig, ax = plt.subplots(1, 2)
+fig.set_size_inches(11.5, 5)
+plot_vector_field_uncertain(adata, embed_mean, embeds_radian,
+                            ax=ax,
+                            fig=fig, cbar=False, basis=embedding, scale=None)
+
+# This generates shared time uncertainty plot with contour lines
+fig, ax = plt.subplots(1, 3)
+fig.set_size_inches(12, 2.8)
+adata.obs['shared_time_uncertain'] = posterior_samples['cell_time'].std(0).flatten()
+ax_cb = scv.pl.scatter(adata, c='shared_time_uncertain', ax=ax[0], show=False, cmap='inferno', fontsize=7, s=20, colorbar=True, basis=embedding)
+select = adata.obs['shared_time_uncertain'] > np.quantile(adata.obs['shared_time_uncertain'], 0.9)
+sns.kdeplot(adata.obsm[f'X_{embedding}'][:, 0][select],
+            adata.obsm[f'X_{embedding}'][:, 1][select],
+            ax=ax[0], levels=3, fill=False)
+
+# This generates vector field uncertainty based on Rayleigh test.
+adata.obs.loc[:, 'vector_field_rayleigh_test'] = fdri
+im = ax[1].scatter(adata.obsm[f'X_{basis}'][:, 0],
+                   adata.obsm[f'X_{basis}'][:, 1], s=3, alpha=0.9,
+                   c=adata.obs['vector_field_rayleigh_test'], cmap='inferno_r',
+                   linewidth=0)
+set_colorbar(im, ax[1], labelsize=5, fig=fig, position='right')
+select = adata.obs['vector_field_rayleigh_test'] > np.quantile(adata.obs['vector_field_rayleigh_test'], 0.95)
+sns.kdeplot(adata.obsm[f'X_{embedding}'][:, 0][select],
+            adata.obsm[f'X_{embedding}'][:, 1][select], ax=ax[1], levels=3, fill=False)
+ax[1].axis('off')
+ax[1].set_title("vector field\nrayleigh test\nfdr<0.05: %s%%" % (round((fdri < 0.05).sum()/fdri.shape[0], 2)*100), fontsize=7)
+```
+
+Step 5: Prioritize putative cell fate marker genes based on negative
+mean absolute errors and pearson correlation between denoised spliced
+expression and posterior mean shared time, and then visualize the top
+one with rainbow plots
+
+```python
+fig = plt.figure(figsize=(7.07, 4.5))
+subfig = fig.subfigures(1, 2, wspace=0.0, hspace=0, width_ratios=[1.6, 4])
+ax = fig.subplots(1)
+# This generates the selected cell fate markers and output in DataFrame
+volcano_data, _ = plot_gene_ranking([posterior_samples], [adata], ax=ax,
+                                     time_correlation_with='st', assemble=True)
+# This generates the rainbow plots for the selected markers.
+_ = rainbowplot(volcano_data, adata, posterior_samples,
+                subfig[1], data=['st', 'ut'], num_genes=4)
+```
+
+## Illustrative examples of Pyro-Velocity analyses on different single-cell datasets
+
+### Pyro-Velocity applied to a PBMC dataset
+
+See the [data referred to here](https://scvelo.readthedocs.io/en/stable/perspectives/Perspectives/).
+
+This is a scRNA-seq dataset of fully mature peripheral blood mononuclear
+cells (PBMC) generated using the 10X genomics kit and containing 65,877
+cells with 11 fully differentiated immune cell types. This dataset
+doesn\'t contain stem and progenitor cells or other signature of and
+undergoing dynamical differentiation, thus no consistent velocity flow
+should be detected.
+
+Below we show the main output generated by Pyro-Velocity Model 1
+analysis. Pyro-Velocity failed to detect high-confidence trajectories in
+the mature blood cell states, consistent with what is known about the
+biology underlying these cells.
+
+**Vector field with uncertainty**
+
+<!-- ![PBMC vector field uncertainty](docs/source/readme_figure2.png) -->
+<img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/source/readme_figure2.png" alt="PBMC vector field uncertainty">
+
+These 6 plots from left to right show: 1. cell types, 2. stream plot of
+Pyro-velocity vector field based on the posterior mean of 30 posterior
+samples, 3. single cell vector field examples showing all 30 posterior
+samples as vectors for 3 arbitrarily selected cells; 4. single cell
+vector field with uncertainty based on angular standard deviation across
+30 posterior samples, 5. averaged vector field uncertainty from 4. 6.
+Rayleigh test of posterior samples vector field, the title shows the
+expected false discovery rate using a 5% threshold.
+
+The full example can be reproduced using the
+[PBMC](https://github.com/pinellolab/pyrovelocity/blob/master/docs/source/notebooks/pbmc.ipynb)
+Jupyter notebook.
+
+### Pyro-Velocity applied to a pancreas development dataset
+
+See the [data referred to here](https://scvelo.readthedocs.io/en/stable/VelocityBasics/).
+
+Here we apply Pyro-Velocity to a single cell RNA-seq dataset of mouse
+pancreas in the E15.5 embryo developmental stage. This dataset was
+generated using the 10X genomics kit and contains 3,696 cells with 8
+cell types including progenitor cells, intermediate and terminal cell
+states.
+
+Below we show the main output generated by Pyro-Velocity Model 1
+analysis. Pyro-Velocity was able to define well-known developmental cell
+hierarchies identifying cell trajectories originating from ductal
+progenitor cells and culminated in the production of mature Alpha, Beta,
+Delta, and Epsilon cells.
+
+**Vector field with uncertainty**
+
+<!-- ![Pancreas vector field uncertainty](docs/source/readme_figure3.png) -->
+<img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/source/readme_figure3.png" alt="Pancreas vector field uncertainty">
+
+These 6 plots from left to right are showing the same analyses presented
+as in the example above.
+
+**Shared time with uncertainty**
+
+<!-- ![Pancreas shared time uncertainty](docs/source/readme_figure4.png) -->
+<img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/source/readme_figure4.png" alt="Pancreas vector field uncertainty">
+
+The left figure shows the average of 30 posterior samples for the cell
+shared time, the title of the figure shows the Spearman\'s correlation
+with the Cytotrace score, an orthogonal state-of-the-art method used to
+predict cell differentiation based on the number of expressed genes per
+cell (Gulati et. al, Science 2020). The right figure shows the standard
+deviation across posterior samples of shared time.
+
+**Gene selection and visualization**
+
+To uncover potential cell fate determinant markers genes of the mouse
+pancreas, we first select the top 300 genes with the best velocity model
+fit (we use negative mean absolute error ), then we rank the filtered
+genes using Pearson\'s correlation between denoised spliced expression
+and the posterior mean of the recovered shared time across cells.
+
+<!-- ![Pancreas Volcano plot for gene selection](docs/source/readme_figure6.png) -->
+<img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/source/readme_figure6.png" alt="Pancreas Volcano plot for gene selection">
+
+For the selected genes, it is possible to explore in depth their
+dynamic, using phase portraits, rainbow plots, and UMAP rendering of
+denoised splicing gene expression across cells.
+
+<!-- ![Pancreas vector field uncertainty](docs/source/readme_figure7.png) -->
+<img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/source/readme_figure7.png" alt="Pancreas vector field uncertainty">
+
+The full example can be reproduced using the
+[Pancreas](https://github.com/pinellolab/pyrovelocity/blob/master/docs/source/notebooks/pancreas.ipynb)
+jupyter notebook.
+
+### Pyro-Velocity applied to the LARRY dataset
+
+See the [data referred to here](https://figshare.com/articles/dataset/larry_invitro_adata_sub_raw_h5ad/20780344).
+
+This last example, present the analysis of a recent scRNA-seq dataset
+profiling mouse hematopoises at high resolution thanks to lineage
+relationship information captured by the Lineage And RNA RecoverY
+(LARRY) system. LARRY leverages unique lentiviral barcodes that enables
+to clonally trace cell fates over time (Weinrab et al. Cell 20).
+
+Below we show the main output generated by Pyro-Velocity analysis.
+
+**Vector field with uncertainty**
+
+<!-- ![LARRY vector field uncertainty](docs/source/readme_figure8.png) -->
+<img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/source/readme_figure8.png" alt="LARRY vector field uncertainty">
+
+These 5 plots from left to right shows: 1) Cell types, 2) Clone
+progression vector field by using centroid of cells belonging to the
+same barcode for generating directed connection between consecutive
+physical times, 3) single cell vector field with uncertainty based on
+angular standard deviation across 30 posterior samples, 4. averaged
+vector field uncertainty from 3. 5. Rayleigh test of posterior samples
+vector field, the title shows the false discovery rate using threshold
+5%.
+
+**Shared time with uncertainty**
+
+To quantitatively assess the quality of the the receovered shared time
+we also considered the agreement of our method with Cospar, a
+state-of-the-art method specifically designed for predicting fate
+potency based on LARRY data.
+
+<!-- ![Pancreas shared time uncertainty](docs/source/readme_figure9.png) -->
+<img src="https://raw.githubusercontent.com/pinellolab/pyrovelocity/master/docs/source/readme_figure9.png" alt="Pancreas shared time uncertainty">
+
+The leftmost figure shows the Cospar fate potency score, the middle
+figure shows the average of 30 posterior samples from Pyro-Velocity
+shared time per cell, the title of the figure shows the Spearman's
+correlation between cell latent shared time and fate potency scores
+derived from Cospar, the right figure shows the standard deviation
+across posterior samples of shared time.
+
+The full example can be reproduced using the
+[LARRY](https://github.com/pinellolab/pyrovelocity/blob/master/docs/source/notebooks/larry.ipynb)
+jupyter notebook.
+
+# Troubleshooting
+
+If you are having an issue using pyrovelocity, please feel free to [start a discussion](https://github.com/pinellolab/pyrovelocity/discussions)
+or [file an issue](https://github.com/pinellolab/pyrovelocity/issues) containing a [MRE](https://en.wikipedia.org/wiki/Minimal_reproducible_example).
+
+Also see [contributing](./docs/contributing.md).
 
-setup(**setup_kwargs)
```

