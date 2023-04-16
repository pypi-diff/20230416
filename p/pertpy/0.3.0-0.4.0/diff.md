# Comparing `tmp/pertpy-0.3.0.tar.gz` & `tmp/pertpy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pertpy-0.3.0.tar", max compression
+gzip compressed data, was "pertpy-0.4.0.tar", max compression
```

## Comparing `pertpy-0.3.0.tar` & `pertpy-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,40 @@
--rw-r--r--   0        0        0     1070 2023-01-31 14:14:05.863918 pertpy-0.3.0/LICENSE
--rw-r--r--   0        0        0     1860 2023-01-31 14:14:05.863918 pertpy-0.3.0/README.md
--rw-r--r--   0        0        0      329 2023-01-31 14:14:05.883919 pertpy-0.3.0/pertpy/__init__.py
--rw-r--r--   0        0        0     1349 2023-01-31 14:14:05.883919 pertpy-0.3.0/pertpy/data/__init__.py
--rw-r--r--   0        0        0     2279 2023-01-31 14:14:05.883919 pertpy-0.3.0/pertpy/data/_dataloader.py
--rw-r--r--   0        0        0    81246 2023-01-31 14:14:05.883919 pertpy-0.3.0/pertpy/data/_datasets.py
--rw-r--r--   0        0        0      258 2023-01-31 14:14:05.883919 pertpy-0.3.0/pertpy/plot/__init__.py
--rw-r--r--   0        0        0     6539 2023-01-31 14:14:05.883919 pertpy-0.3.0/pertpy/plot/_augurpy.py
--rw-r--r--   0        0        0    38989 2023-01-31 14:14:05.887919 pertpy-0.3.0/pertpy/plot/_coda.py
--rw-r--r--   0        0        0     9257 2023-01-31 14:14:05.887919 pertpy-0.3.0/pertpy/plot/_milopy.py
--rw-r--r--   0        0        0    25077 2023-01-31 14:14:05.887919 pertpy-0.3.0/pertpy/plot/_mixscape.py
--rw-r--r--   0        0        0        0 2023-01-31 14:14:05.887919 pertpy-0.3.0/pertpy/preprocessing/__init__.py
--rw-r--r--   0        0        0        0 2023-01-31 14:14:05.887919 pertpy-0.3.0/pertpy/py.typed
--rw-r--r--   0        0        0      258 2023-01-31 14:14:05.887919 pertpy-0.3.0/pertpy/tools/__init__.py
--rw-r--r--   0        0        0    40574 2023-01-31 14:14:05.887919 pertpy-0.3.0/pertpy/tools/_augurpy.py
--rw-r--r--   0        0        0    61259 2023-01-31 14:14:05.887919 pertpy-0.3.0/pertpy/tools/_base_coda.py
--rw-r--r--   0        0        0     1521 2023-01-31 14:14:05.887919 pertpy-0.3.0/pertpy/tools/_kernel_pca.py
--rw-r--r--   0        0        0    26946 2023-01-31 14:14:05.887919 pertpy-0.3.0/pertpy/tools/_milopy.py
--rw-r--r--   0        0        0    21803 2023-01-31 14:14:05.887919 pertpy-0.3.0/pertpy/tools/_mixscape.py
--rw-r--r--   0        0        0    21141 2023-01-31 14:14:05.887919 pertpy-0.3.0/pertpy/tools/_sccoda.py
--rw-r--r--   0        0        0    28654 2023-01-31 14:14:05.887919 pertpy-0.3.0/pertpy/tools/_tasccoda.py
--rw-r--r--   0        0        0     2910 2023-01-31 14:14:05.887919 pertpy-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3226 1970-01-01 00:00:00.000000 pertpy-0.3.0/setup.py
--rw-r--r--   0        0        0     3425 1970-01-01 00:00:00.000000 pertpy-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-16 11:27:06.116299 pertpy-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1860 2023-04-16 11:27:06.116299 pertpy-0.4.0/README.md
+-rw-r--r--   0        0        0      363 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/__init__.py
+-rw-r--r--   0        0        0     1206 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/data/__init__.py
+-rw-r--r--   0        0        0     2279 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/data/_dataloader.py
+-rw-r--r--   0        0        0    62405 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/data/_datasets.py
+-rw-r--r--   0        0        0      434 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/plot/__init__.py
+-rw-r--r--   0        0        0     6539 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/plot/_augurpy.py
+-rw-r--r--   0        0        0    38991 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/plot/_coda.py
+-rw-r--r--   0        0        0     2779 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/plot/_guide_rna.py
+-rw-r--r--   0        0        0     9257 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/plot/_milopy.py
+-rw-r--r--   0        0        0    25129 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/plot/_mixscape.py
+-rw-r--r--   0        0        0    13118 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/plot/_scgen.py
+-rw-r--r--   0        0        0       54 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3493 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/preprocessing/_guide_rna.py
+-rw-r--r--   0        0        0        0 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/py.typed
+-rw-r--r--   0        0        0      818 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/__init__.py
+-rw-r--r--   0        0        0    40607 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_augur.py
+-rw-r--r--   0        0        0        0 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_coda/__init__.py
+-rw-r--r--   0        0        0    61298 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_coda/_base_coda.py
+-rw-r--r--   0        0        0    21639 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_coda/_sccoda.py
+-rw-r--r--   0        0        0    29152 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_coda/_tasccoda.py
+-rw-r--r--   0        0        0    35411 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_dialogue.py
+-rw-r--r--   0        0        0     3618 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_differential_gene_expression.py
+-rw-r--r--   0        0        0        0 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_distances/__init__.py
+-rw-r--r--   0        0        0    11814 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_distances/_distance_tests.py
+-rw-r--r--   0        0        0    12562 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_distances/_distances.py
+-rw-r--r--   0        0        0     1521 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_kernel_pca.py
+-rw-r--r--   0        0        0       63 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_metadata/__init__.py
+-rw-r--r--   0        0        0    25517 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_metadata/_cell_line.py
+-rw-r--r--   0        0        0    27081 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_milo.py
+-rw-r--r--   0        0        0    22105 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_mixscape.py
+-rw-r--r--   0        0        0       49 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_scgen/__init__.py
+-rw-r--r--   0        0        0     2880 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_scgen/_base_components.py
+-rw-r--r--   0        0        0    12990 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_scgen/_jax_scgen.py
+-rw-r--r--   0        0        0     3902 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_scgen/_jax_scgenvae.py
+-rw-r--r--   0        0        0     2807 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/_scgen/_utils.py
+-rw-r--r--   0        0        0     1069 2023-04-16 11:27:06.140299 pertpy-0.4.0/pertpy/tools/transferlearning_MMD_LICENSE
+-rw-r--r--   0        0        0     3037 2023-04-16 11:27:06.144299 pertpy-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3722 1970-01-01 00:00:00.000000 pertpy-0.4.0/PKG-INFO
```

### Comparing `pertpy-0.3.0/LICENSE` & `pertpy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pertpy-0.3.0/README.md` & `pertpy-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pertpy-0.3.0/pertpy/data/_dataloader.py` & `pertpy-0.4.0/pertpy/data/_dataloader.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.3.0/pertpy/data/_datasets.py` & `pertpy-0.4.0/pertpy/data/_datasets.py`

 * *Files 23% similar despite different names*

```diff
@@ -24,25 +24,23 @@
     Returns:
         :class:`~anndata.AnnData` object of the Burczynski dataset
     """
     return sc.datasets.burczynski06()
 
 
 def papalexi_2021() -> MuData:  # pragma: no cover
-    """Dataset of the Mixscape Vignette.
-
-    https://satijalab.org/seurat/articles/mixscape_vignette.html
+    """ECCITE-seq dataset of 11 gRNAs generated from stimulated THP-1 cell line.
 
     Reference:
-    Papalexi, E., Mimitou, E.P., Butler, A.W. et al. Characterizing the molecular regulation
-    of inhibitory immune checkpoints with multimodal single-cell screens.
-    Nat Genet 53, 322–331 (2021). https://doi.org/10.1038/s41588-021-00778-2
+        Papalexi, E., Mimitou, E.P., Butler, A.W. et al. Characterizing the molecular regulation
+        of inhibitory immune checkpoints with multimodal single-cell screens.
+        Nat Genet 53, 322–331 (2021). https://doi.org/10.1038/s41588-021-00778-2
 
     Returns:
-        :class:`~anndata.AnnData` object of the Crispr dataset
+        :class:`~anndata.AnnData` object of the ECCITE-seq dataset
     """
     output_file_name = "papalexi_2021.h5mu"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://figshare.com/ndownloader/files/36509460",
             output_file_name=output_file_name,
@@ -53,15 +51,15 @@
     else:
         mudata = mu.read(output_file_path)
 
     return mudata
 
 
 def sc_sim_augur() -> AnnData:  # pragma: no cover
-    """Simulated test dataset used the Usage example for the Augur.
+    """Simulated test dataset used the usage example for the Augur.
 
     https://github.com/neurorestore/Augur
 
     Returns:
         :class:`~anndata.AnnData` object of a simulated single-cell RNA seq dataset
     """
     output_file_name = "sc_sim_augur.h5ad"
@@ -371,16 +369,40 @@
         adata = sc.read_h5ad(filename=settings.datasetdir.__str__() + "/" + output_file_name)
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
+def distance_example_data() -> AnnData:  # pragma: no cover
+    """Example dataset used to feature distances and distance_tests.
+
+    Processed and subsetted version of original Perturb-seq dataset by Dixit et al.
+
+    Returns:
+        :class:`~anndata.AnnData` object
+    """
+    output_file_name = "distances_example_data.h5ad"
+    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
+    if not Path(output_file_path).exists():
+        _download(
+            url="https://figshare.com/ndownloader/files/39561379",
+            output_file_name=output_file_name,
+            output_path=settings.datasetdir,
+            is_zip=False,
+        )
+        adata = sc.read_h5ad(filename=settings.datasetdir.__str__() + "/" + output_file_name)
+    else:
+        adata = sc.read_h5ad(output_file_path)
+
+    return adata
+
+
 def kang_2018() -> AnnData:  # pragma: no cover
-    """Processed multiplexing droplet-based single cell RNA-sequencing using genetic barcodes
+    """Processed multiplexing droplet-based single cell RNA-sequencing using genetic barcodes.
 
     HiSeq 2500 data for sequencing of PBMCs from SLE patients and 2 controls. We collected 1M cells
     each from frozen PBMC samples that were Ficoll isolated and prepared using the 10x Single Cell
     instrument according to standard protocol. Samples A, B, and C were prepared on the instrument
     directly following thaw, while samples 2.1 and 2.2 were cultured for 6 hours with (B) or
     without (A) IFN-beta stimulation prior to loading on the 10x Single Cell instrument.
 
@@ -416,15 +438,14 @@
     with scArches.
 
     Reference:
         Stephenson, E., Reynolds, G., Botting, R. A., et al. (2021).
         Single-cell multi-omics analysis of the immune response in COVID-19.
         Nature Medicine, 27(5). https://doi.org/10.1038/s41591-021-01329-2
 
-
     Returns:
         :class:`~anndata.AnnData` object of scRNA-seq profiles
     """
     output_file_name = "stephenson_2021_subsampled.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
@@ -463,33 +484,24 @@
         adata = sc.read_h5ad(filename=settings.datasetdir.__str__() + "/" + output_file_name)
     else:
         adata = sc.read_h5ad(output_file_path)
     return adata
 
 
 def adamson_2016_pilot() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
+    """6000 chronic myeloid leukemia (K562) cells carrying 8 distinct GBCs.
 
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
-
-    In a pilot experiment, single-cell RNA-seq was performed on a pool of individually
-    transduced chronic myeloid leukemia cells (K562) carrying 8 distinct GBCs, analyzing
-    ∼6,000 cells total.
+    In a pilot experiment, single-cell RNA-seq was performed on a pool of individually transduced chronic
+    myeloid leukemia cells (K562) carrying 8 distinct guide barcodes, analyzing ∼6,000 cells total.
 
     Source paper:
-        https://doi.org/10.1016/j.cell.2016.11.048
+        https://www.sciencedirect.com/science/article/pii/S0092867416316609?via%3Dihub
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "adamson_2016_pilot.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/AdamsonWeissman2016_GSM2406675_10X001.h5ad?download=1",
             output_file_name=output_file_name,
@@ -500,37 +512,28 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def adamson_2016_upr_epistasis() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
-
+    """15000 K562 cells with UPR sensor genes knocked out and treated with thapsigargin.
 
     In UPR epistasis experiment, Perturb-seq was applied to explore the branches of
     the mammalian UPR. Using the three-guide Perturb-seq vector, sgRNAs targeting each
     UPR sensor gene were introduced into K562 cells with dCas9-KRAB. Transduced cells
     were then pooled, sorted for vector delivery, and after 5 days of total growth,
     treated with thapsigargin. Control cells were treated with DMSO. Transcriptomes
     of ∼15,000 cells were sequenced.
 
     Source paper:
-        https://doi.org/10.1016/j.cell.2016.11.048
+        https://www.sciencedirect.com/science/article/pii/S0092867416316609?via%3Dihub
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb preparedsingle-cell perturbation data
     """
     output_file_name = "adamson_2016_upr_epistasis.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/AdamsonWeissman2016_GSM2406677_10X005.h5ad?download=1",
             output_file_name=output_file_name,
@@ -541,34 +544,26 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def adamson_2016_upr_perturb_seq() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """Transcriptomics of 65000 cells that were subject to 91 sgRNAs targeting 82 genes.
 
     In UPR Perturb-seq experiment, Perturb-seq was applied to a small CRISPRi library
     of 91 sgRNAs targeting 82 genes. sgRNAs were delivered via pooled transduction
     using a mixture of separately prepared lentiviruses, and ∼65,000 transcriptomes
     were collected in one large pooled experiment.
 
     Source paper:
-        https://doi.org/10.1016/j.cell.2016.11.048
+        https://www.sciencedirect.com/science/article/pii/S0092867416316609?via%3Dihub
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "adamson_2016_upr_perturb_seq.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/AdamsonWeissman2016_GSM2406681_10X010.h5ad?download=1",
             output_file_name=output_file_name,
@@ -579,29 +574,21 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def aissa_2021() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
+    """Transcriptomics of 848 P99 cells subject to consecutive erlotinib and 756 control cells.
 
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    In this study 848 PC9 cells subjected to consecutive erlotinib treatment (for
+    1, 2, 4, 9, and 11 days) and 756 control cells were analysed using Drop-seq.
 
     Source paper:
-        https://doi.org/10.1038/s41467-021-21884-z
-
-    In this studym 848 PC9 cells subjected to consecutive erlotinib treatment (for
-    1, 2, 4, 9, and 11 days) and 756 control cells were analysed using Drop-seq.
+        https://www.nature.com/articles/s41467-021-21884-z
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
     """
     output_file_name = "aissa_2021.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
@@ -615,35 +602,27 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def chang_2021() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """Transcriptomics of 5 different cell lines that were induced with a unique TraCe-seq barcode.
 
     TraCe-seq is a method that captures at clonal resolution the origin, fate and
     differential early adaptive transcriptional programs of cells in a complex
     population in response to distinct treatments. Here, a unique TraCe-seq barcode was
     transduced into five different cell lines (PC9, MCF-10A, MDA-MB-231, NCI-H358 and NCI-H1373).
     Transduced cells were selected with puromycin only, mixed together and profiled by 10x scRNA-seq.
 
     Source paper:
-        https://doi.org/10.1038/s41587-021-01005-3
+        https://www.nature.com/articles/s41587-021-01005-3
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "chang_2021.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/ChangYe2021.h5ad?download=1",
             output_file_name=output_file_name,
@@ -654,36 +633,28 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def datlinger_2017() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """Transcriptpmics of 5905 Jurkat cells induced with anti-CD3 and anti-CD28 antibodies.
 
     For CROP-seq, Jurkat cells were transduced with a gRNA library targeting high-level
     regulators of T cell receptor signaling and a set of transcription factors. After 10
     days of antibiotic selection and expansion, cells were stimulated with anti-CD3 and
     anti-CD28 antibodies or left untreated. Both conditions were analyzed using CROP-seq,
     measuring TCR activation for each gene knockout. The dataset comprises 5,905 high-quality
     single-cell transcriptomes with uniquely assigned gRNAs.
 
     Source paper:
-        https://doi.org/10.1038/nmeth.4177
+        https://www.nature.com/articles/nmeth.4177
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "datlinger_2017.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/DatlingerBock2017.h5ad?download=1",
             output_file_name=output_file_name,
@@ -694,35 +665,27 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def datlinger_2021() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-     https://github.com/sanderlab/scPerturb
-
-     Reference:
-        Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-        Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-        scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-        bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """Transcriptomics of 151788 nuclei of four cell lines.
 
     A large-scale scifi-RNA-seq experiment was performed with 383,000 nuclei loaded into
     a single microfluidic channel of the Chromium system. Four human cell lines (HEK293T,
     Jurkat, K562 and NALM-6) were combined in an equal mixture, and technical replicates of
     each cell line with different preindexing (round1) barcodes were marked. This experiment
     resulted in 151,788 single-cell transcriptomes passing quality control.
 
-     Source paper:
-         https://doi.org/10.1038/s41592-021-01153-z
+    Source paper:
+        https://doi.org/10.1038/s41592-021-01153-z
 
      Returns:
-         :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+         :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "datlinger_2021.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/DatlingerBock2021.h5ad?download=1",
             output_file_name=output_file_name,
@@ -733,37 +696,28 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def dixit_2016_scperturb() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """Transcriptomics of 200000 bone marrow-derived dendritic K562 cells.
 
     Six Perturb-seq experiments were performed, analyzing 200,000 cells. In bone
     marrow-derived dendritic cells (BMDCs), 24 transcription factors (TFs) were targeted
     and the effects pre-stimulation (0 hr) and at 3 hr post-lipopolysaccharide (LPS) were
     measured. In K562 cells, 14 TFs and 10 cell-cycle regulators were targeted in separate
     pooled experiments. For K562 TFs, experiments were performed using lower and higher MOI
-    and at two time points. Reference scRNA-seq data from unperturbed cells were collected
-    separately.
+    and at two time points. Reference scRNA-seq data from unperturbed cells were collected separately.
 
     Source paper:
         https://doi.org/10.1016/j.cell.2016.11.038
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "dixit_2016_scperturb.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/DixitRegev2016.h5ad?download=1",
             output_file_name=output_file_name,
@@ -774,36 +728,28 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def frangieh_2021_protein() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """CITE-seq data of 218000 cells under 750 perturbations (only the surface protein data).
 
     Perturb-CITE-seq was developed for pooled CRISPR perturbation screens with multi-modal
     RNA and protein single-cell profiling readout and applied to screen patient-derived
     autologous melanoma and tumor infiltrating lymphocyte (TIL) co-cultures. RNA and 20
     surface proteins were profiled in over 218,000 cells under ~750 perturbations, chosen
     by their membership in an immune evasion program that is associated with immunotherapy
     resistance in patients.
 
     Source paper:
         https://doi.org/10.1038/s41588-021-00779-1
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "frangieh_2021_protein.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/FrangiehIzar2021_protein.h5ad?download=1",
             output_file_name=output_file_name,
@@ -814,36 +760,28 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def frangieh_2021_rna() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """CITE-seq data of 218000 cells under 750 perturbations (only the transcriptomics data).
 
     Perturb-CITE-seq was developed for pooled CRISPR perturbation screens with multi-modal
     RNA and protein single-cell profiling readout and applied to screen patient-derived
     autologous melanoma and tumor infiltrating lymphocyte (TIL) co-cultures. RNA and 20
     surface proteins were profiled in over 218,000 cells under ~750 perturbations, chosen
     by their membership in an immune evasion program that is associated with immunotherapy
     resistance in patients.
 
     Source paper:
         https://doi.org/10.1038/s41588-021-00779-1
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "frangieh_2021_rna.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/FrangiehIzar2021_RNA.h5ad?download=1",
             output_file_name=output_file_name,
@@ -854,33 +792,25 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def gasperini_2019_atscale() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """Transcriptomics of 254974 cells of chronic K562 cells with CRISPRi perturbations.
 
     Across two experiments, the authors used dCas9-KRAB to perturb 5,920 candidate enhancers
     with no strong a priori hypothesis as to their target gene(s) in 254,974 cells of chronic
     myelogenous leukemia cell line K562, with CRISPRi as the mode of perturbation.
 
     Source paper:
         https://doi.org/10.1016/j.cell.2018.11.029
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "gasperini_2019_atscale.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/GasperiniShendure2019_atscale.h5ad?download=1",
             output_file_name=output_file_name,
@@ -891,23 +821,15 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def gasperini_2019_highmoi() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """K562 perturbed cells with 1119 candidate enhancers (only the high MOI part).
 
     The authors used dCas9-KRAB to perturb 1,119 candidate enhancers with no strong a priori
     hypothesis as to their target gene(s) in the chronic myelogenous leukemia cell line
     K562, with CRISPRi as the mode of perturbation, where K562 cells were transduced
     at a high MOI (pilot library MOI = ∼15).
 
     Source paper:
@@ -929,34 +851,26 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def gasperini_2019_lowmoi() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """K562 perturbed cells with 1119 candidate enhancers (only the low MOI part).
 
     The authors used dCas9-KRAB to perturb 1,119 candidate enhancers with no strong a priori
     hypothesis as to their target gene(s) in chronic myelogenous leukemia cell line K562,
     with CRISPRi as the mode of perturbation, where K562 cells were transduced at a
     low MOI (pilot library MOI = ∼1).
 
     Source paper:
         https://doi.org/10.1016/j.cell.2018.11.029
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "gasperini_2019_lowmoi.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/GasperiniShendure2019_lowMOI.h5ad?download=1",
             output_file_name=output_file_name,
@@ -967,33 +881,25 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def gehring_2019() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """96-plex perturbation experiment on live mouse neural stem cells.
 
     In this study, a 96-plex perturbation experiment was conducted on live mouse neural
     stem cells (NSCs), consisting of a pair of drug-triples with 4 drugs in total at 3
     or 4 different concentractions.
 
     Source paper:
         https://doi.org/10.1038/s41587-019-0372-z
 
     Returns:
-        :class:`~anndata.AnnData` object of a single-cell RNA seq dataset
+        :class:`~anndata.AnnData` object of a scPerturb prepared single-cell dataset
     """
     output_file_name = "gehring_2019.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/GehringPachter2019.h5ad?download=1",
             output_file_name=output_file_name,
@@ -1004,23 +910,15 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def mcfarland_2020() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """Response of various cell lines to a range of different drugs and CRISPRi perturbations.
 
     Here, the authors developed MIX-Seq, a method for multiplexed transcriptional profiling
     of post-perturbation responses across many cell contexts, using scRNA-seq applied to
     co-treated pools of cancer cell lines. The responses of pools of 24–99 cell lines to
     a range of different drugs were profiled, as well as to CRISPR perturbations.
 
     Source paper:
@@ -1041,235 +939,27 @@
         adata = sc.read_h5ad(filename=settings.datasetdir.__str__() + "/" + output_file_name)
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
-def norman_2019_filtered() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
-
-    K562 cells stably expressing dCas9-KRAB were transduced with the CRISPRa genetic
-    interactions (GIs) library. 132 gene pairs were picked from the GI map, chosen
-    both within and between blocks of genes with similar interaction profiles, and
-    targeted each with CRISPRa sgRNA pairs. In total, transcriptional readouts for
-    287 perturbations measured across ~110,000 single cells were obtained (median
-    273 cells per condition) in one pooled experiment.
-
-
-    Source paper:
-        https://doi.org/10.1126/science.aax4438
-
-    Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
-    """
-    output_file_name = "norman_2019_filtered.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
-    if not Path(output_file_path).exists():
-        _download(
-            url="https://zenodo.org/record/7278143/files/NormanWeissman2019_filtered.h5ad?download=1",
-            output_file_name=output_file_name,
-            output_path=settings.datasetdir,
-            is_zip=False,
-        )
-        adata = sc.read_h5ad(filename=settings.datasetdir.__str__() + "/" + output_file_name)
-    else:
-        adata = sc.read_h5ad(output_file_path)
-
-    return adata
-
-
-def papalexi_2021_eccite_arrayed_protein() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
-
-    A pilot experiment was performed using gRNA species targeting PD-L1 or IFNGR1 as
-    well as NT controls on simulated THP-1 cells. Libraries were sequenced on a
-    NextSeq 500 system. ADT libraries were processed with CITE-seq-Count and
-    normalized across cells using the centered log ratio. Cells with high mitochondrial
-    gene content (>8%) were removed.
-
-
-    Source paper:
-        https://doi.org/10.1038/s41588-021-00778-2
-
-    Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
-    """
-    output_file_name = "papalexi_2021_eccite_arrayed_protein.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
-    if not Path(output_file_path).exists():
-        _download(
-            url="https://zenodo.org/record/7278143/files/PapalexiSatija2021_eccite_arrayed_protein.h5ad?download=1",
-            output_file_name=output_file_name,
-            output_path=settings.datasetdir,
-            is_zip=False,
-        )
-        adata = sc.read_h5ad(filename=settings.datasetdir.__str__() + "/" + output_file_name)
-    else:
-        adata = sc.read_h5ad(output_file_path)
-
-    return adata
-
-
-def papalexi_2021_eccite_arrayed_rna() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
-
-    A pilot experiment was performed using gRNA species targeting PD-L1 or IFNGR1 as
-    well as NT controls on simulated THP-1 cells. Libraries were sequenced on a NextSeq
-    500 system. mRNA libraries were quantified using Cell Ranger (2.1.1; hg19 reference)
-    and normalized using standard log normalization in Seurat.
-
-    Source paper:
-        https://doi.org/10.1038/s41588-021-00778-2
-
-    Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
-    """
-    output_file_name = "papalexi_2021_eccite_arrayed_rna.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
-    if not Path(output_file_path).exists():
-        _download(
-            url="https://zenodo.org/record/7278143/files/PapalexiSatija2021_eccite_arrayed_RNA.h5ad?download=1",
-            output_file_name=output_file_name,
-            output_path=settings.datasetdir,
-            is_zip=False,
-        )
-        adata = sc.read_h5ad(filename=settings.datasetdir.__str__() + "/" + output_file_name)
-    else:
-        adata = sc.read_h5ad(output_file_path)
-
-    return adata
-
-
-def papalexi_2021_eccite_protein() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
-
-    In an ECCITE-seq experiment, THP-1 Cas9-inducible cells were transduced with virus
-    containing 111 guides at a low MOI to obtain cells with one gRNA and then stimulated.
-    Samples were hashed following the cell hashing protocol. Protein (ADTs) libraries
-    were constructed by following 10x Genomics and ECCITE-seq protocols, and then sequenced
-    together on two lanes of a NovaSeq run. The CITE-seq-Count package was used to generate
-    count matrices for ADT libraries.
-
-    Source paper:
-        https://doi.org/10.1038/s41588-021-00778-2
-
-    Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
-    """
-    output_file_name = "papalexi_2021_eccite_protein.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
-    if not Path(output_file_path).exists():
-        _download(
-            url="https://zenodo.org/record/7278143/files/PapalexiSatija2021_eccite_protein.h5ad?download=1",
-            output_file_name=output_file_name,
-            output_path=settings.datasetdir,
-            is_zip=False,
-        )
-        adata = sc.read_h5ad(filename=settings.datasetdir.__str__() + "/" + output_file_name)
-    else:
-        adata = sc.read_h5ad(output_file_path)
-
-    return adata
-
-
-def papalexi_2021_eccite_rna() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
-
-    In an ECCITE-seq experiment, THP-1 Cas9-inducible cells were transduced with virus
-    containing 111 guides at a low MOI to obtain cells with one gRNA and then stimulated.
-    Samples were hashed following the cell hashing protocol. mRNA Libraries were constructed
-    by following 10x Genomics and ECCITE-seq protocols, and then sequenced together on
-    two lanes of a NovaSeq run. Sequencing reads from the mRNA library were mapped to the
-    hg19 reference genome using Cell Ranger software (version 2.1.1).
-
-    Source paper:
-        https://doi.org/10.1038/s41588-021-00778-2
-
-    Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
-    """
-    output_file_name = "papalexi_2021_eccite_rna.h5ad"
-    output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
-    if not Path(output_file_path).exists():
-        _download(
-            url="https://zenodo.org/record/7278143/files/PapalexiSatija2021_eccite_RNA.h5ad?download=1",
-            output_file_name=output_file_name,
-            output_path=settings.datasetdir,
-            is_zip=False,
-        )
-        adata = sc.read_h5ad(filename=settings.datasetdir.__str__() + "/" + output_file_name)
-    else:
-        adata = sc.read_h5ad(output_file_path)
-
-    return adata
-
-
 def replogle_2022_k562_essential() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """K562 cells transduced with CRISPRi (day 7 after transduction).
 
     For day 6 essential-scale experiment in chronic myeloid leukemia (CML) (K562) cell
     lines, library lentivirus was packaged into lentivirus in 293T cells and empirically
     measured in K562 cells to obtain viral titers. CRISPRi K562 cells were transduced
-    and 20Q1 Cancer Dependency Map common essential genes were targeted at day 7 after
-    transduction.
+    and 20Q1 Cancer Dependency Map common essential genes were targeted at day 7 after transduction.
 
     Source paper:
         https://doi.org/10.1016/j.cell.2022.05.013
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "replogle_2022_k562_essential.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/ReplogleWeissman2022_K562_essential.h5ad?download=1",
             output_file_name=output_file_name,
@@ -1280,36 +970,28 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def replogle_2022_k562_gwps() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """K562 cells transduced with CRISPRi (day 8 after transcduction).
 
     Here, the authors used a compact, multiplexed CRISPR interference (CRISPRi) library
     to assay thousands of loss-of-function genetic perturbations with single-cell RNA sequencing
     in chronic myeloid leukemia (CML) (K562) cell lines. For the K562 day 8 genome-scale
     Perturb-seq experiment, library lentivirus was packaged into lentivirus in 293T cells and
     empirically measured in K562 cells to obtain viral titers. CRISPRi K562 cells were transduced
     and all expressed genes were targeted at day 8 after transduction
 
     Source paper:
         https://doi.org/10.1016/j.cell.2022.05.013
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "replogle_2022_k562_gwps.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/ReplogleWeissman2022_K562_gwps.h5ad?download=1",
             output_file_name=output_file_name,
@@ -1320,35 +1002,27 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def replogle_2022_rpe1() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """RPE1 cells transduced with CRISPRi (day 7 after transcduction).
 
     For day 7 essential-scale Perturb-seq experiment in retinal pigment epithelial (RPE1)
     cell lines, library lentivirus was packaged into lentivirus in 293T cells and
     empirically measured in RPE1 cells to obtain viral titers. CRISPRi RPE1 cells expressing
     ZIM3 KRAB-dCas9-P2A-BFP were transduced. 20Q1 Cancer Dependency Map common essential
     genes were targeted at day 7 after transduction.
 
     Source paper:
         https://doi.org/10.1016/j.cell.2022.05.013
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "replogle_2022_rpe1.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/ReplogleWeissman2022_rpe1.h5ad?download=1",
             output_file_name=output_file_name,
@@ -1359,23 +1033,15 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def schiebinger_2019_16day() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """Transcriptomes of 65781 iPSC cells collected over 10 time points in 2i or serum conditions (16-day time course).
 
     Samples were collected from established iPSC lines reprogrammed from the reprogramming mouse embryonic
     fibroblasts (MEFs), maintained in either 2i or serum conditions, at 10 time points across 16 days.
     Overall, 68,339 cells were profiled to an average depth of 38,462 reads per cell. After discarding
     cells with less than 1,000 genes detected, 65,781 cells were obtained, with a median of 2,398 genes
     and 7,387 unique transcripts per cell.
 
@@ -1399,23 +1065,15 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def schiebinger_2019_18day() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """Transcriptomes of 259155 iPSC cells collected over 39 time points in 2i or serum conditions (18-day time course).
 
     Samples were collected from established iPSC lines reprogrammed from the reprogramming mouse embryonic
     fibroblasts (MEFs), maintained in either 2i or serum conditions, over 39 time points separated by
     ∼12 hours across an 18-day time course (and every 6 hours between days 8 and 9). Overall, 259,155 cells
     were profiled.
 
     Source paper:
@@ -1437,29 +1095,20 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def schraivogel_2020_tap_screen_chr11() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """TAP-seq applied to K562 cells (only chromosome 11).
 
     TAP-seq was applied to generate perturbation-based enhancer–target gene maps in K562 cells.
     They perturbed all 1,778 putatively active enhancers predicted on the basis of ENCODE data
     in two regions on chromosome 8 and 11, and identified effects on expressed protein-coding genes
-    within the same regions. Thus, in each cell, 68 (chromosome 8) or 79 (chromosome 11) target genes
-    were measured.
+    within the same regions. Thus, in each cell, 68 (chromosome 8) or 79 (chromosome 11) target genes were measured.
 
     Source paper:
         https://doi.org/10.1038/s41592-020-0837-5
 
     Returns:
         :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
     """
@@ -1476,35 +1125,26 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def schraivogel_2020_tap_screen_chr8() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """TAP-seq applied to K562 cells (only chromosome 8).
 
     TAP-seq was applied to generate perturbation-based enhancer–target gene maps in K562 cells.
     They perturbed all 1,778 putatively active enhancers predicted on the basis of ENCODE data
     in two regions on chromosome 8 and 11, and identified effects on expressed protein-coding genes
-    within the same regions. Thus, in each cell, 68 (chromosome 8) or 79 (chromosome 11) target genes
-    were measured.
+    within the same regions. Thus, in each cell, 68 (chromosome 8) or 79 (chromosome 11) target genes were measured.
 
     Source paper:
         https://doi.org/10.1038/s41592-020-0837-5
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "schraivogel_2020_tap_screen_chr8.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/SchraivogelSteinmetz2020_TAP_SCREEN__chromosome_8_screen.h5ad?download=1",
             output_file_name=output_file_name,
@@ -1515,35 +1155,27 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def shifrut_2018() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """CD8 T-cells from two donors for two conditions (SLICE and CROP-seq).
 
     The authors developed a new method, single guide RNA (sgRNA) lentiviral infection
     with Cas9 protein electroporation (SLICE), and adapted it to allow for CROP-Seq in
     primary human T cells. They used a library of 48 sgRNA, derived from GW screens,
     to explore transcriptional changes downstream of CRISPR-KO. Dataset includes CD8
     T cells from two donors, for two conditions: with TCR stimulation or No stimulation.
 
     Source paper:
         https://doi.org/10.1016/j.cell.2018.10.024
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "shifrut_2018.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/ShifrutMarson2018.h5ad?download=1",
             output_file_name=output_file_name,
@@ -1554,36 +1186,28 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def srivatsan_2020_sciplex2() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """A549 cells exposed to four compounds.
 
     A549, a human lung adenocarcinoma cell line, was exposed to one of four compounds:
     dexamethasone (a corticosteroid agonist), nutlin-3a (a p53-Mdm2 antagonist),
     BMS-345541 (an inhibitor of nuclear factor κB–dependent transcription), or vorinostat
     [suberoylanilide hydroxamic acid (SAHA), an HDAC inhibitor], for 24 hours across seven
     doses in triplicate for a total of 84 drug–dose–replicate combinations and additional
     vehicle controls. Nuclei from each well were labelled and subjected to sci-RNA-seq.
 
     Source paper:
         https://doi.org/10.1126/science.aax6234
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "srivatsan_2020_sciplex2.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/SrivatsanTrapnell2020_sciplex2.h5ad?download=1",
             output_file_name=output_file_name,
@@ -1594,34 +1218,26 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def srivatsan_2020_sciplex3() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """Transcriptomes of 650000 A549, K562, and mCF7 cells exposed to 188 compounds.
 
     sci-Plex was used to screen three well-characterized human cancer cell lines, A549
     (lung adenocarcinoma), K562 (chronic myelogenous leukemia), and MCF7 (mammary
     adenocarcinoma)exposed to 188 compounds, profiling ~650,000 single-cell
     transcriptomes across ~5000 independent samples in one experiment.
 
     Source paper:
         https://doi.org/10.1126/science.aax6234
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "srivatsan_2020_sciplex3.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/SrivatsanTrapnell2020_sciplex3.h5ad?download=1",
             output_file_name=output_file_name,
@@ -1632,37 +1248,29 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def srivatsan_2020_sciplex4() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """A549 and MCF7 cells treated with pracinostat.
 
     A549 and MCF7 cells were treated with pracinostat in the presence and absence of
     acetyl-CoA precursors (acetate, pyruvate, or citrate) or inhibitors of enzymes
     (ACLY, ACSS2, or PDH) involved in replenishing acetyl-CoA pools. After treatment,
     cells were harvested and processed using sci-Plex and trajectories constructed
     for each cell line. In both A549 and MCF7 cells, acetate, pyruvate, and citrate
     supplementation was capable of blocking pracinostat-treated cells from reaching
     the end of the HDAC inhibitor trajectory.
 
     Source paper:
         https://doi.org/10.1126/science.aax6234
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "srivatsan_2020_sciplex4.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/SrivatsanTrapnell2020_sciplex4.h5ad?download=1",
             output_file_name=output_file_name,
@@ -1673,38 +1281,29 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def tian_2019_day7neuron() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """Transcriptomes of 20000 day 7 neurons targeted by 58 gRNAs.
 
     The authors performed single-cell RNA sequencing of ∼20,000 day 7 neurons via 10x Genomics
     platform. Transcripts containing sgRNA sequences were further amplified to facilitate
     sgRNA identity assignment among a pool of 58 sgRNAs (two sgRNAs targeting 27 selected
     gene and four non-targeting control sgRNAs). Following sequencing, transcriptomes and
     sgRNA identities were mapped to individual cells. High data quality for neurons was evident
     from ∼91,000 mean reads per cell, the median number of ∼4,600 genes detected per cell and
     ∼8,400 cells to which a unique sgRNA could be assigned after quality control.
 
-
     Source paper:
         https://doi.org/10.1016/j.neuron.2019.07.014
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "tian_2019_day7neuron.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/TianKampmann2019_day7neuron.h5ad?download=1",
             output_file_name=output_file_name,
@@ -1715,38 +1314,29 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def tian_2019_ipsc() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """Transcriptomics of 20000 iPSCs targeted by 58 sgRNAs.
 
     The authors performed single-cell RNA sequencing of ∼20,000 iPSCs via 10x Genomics
     platform. Transcripts containing sgRNA sequences were further amplified to facilitate
     sgRNA identity assignment among a pool of 58 sgRNAs (two sgRNAs targeting 27 selected
     gene and four non-targeting control sgRNAs). Following sequencing, transcriptomes and
     sgRNA identities were mapped to individual cells. High data quality for iPSCs was evident
     from ∼84,000 mean reads per cell, the median number of ∼5,000 genes detected per cell and
     ∼15,000 cells to which a unique sgRNA could be assigned after quality control.
 
-
     Source paper:
         https://doi.org/10.1016/j.neuron.2019.07.014
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "tian_2019_iPSC.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/TianKampmann2019_iPSC.h5ad?download=1",
             output_file_name=output_file_name,
@@ -1757,23 +1347,15 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def tian_2021_crispra() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """CROP-seq of 50000 neurons treated with 374 gRNAs (CRISPRa only).
 
     For CRISPRa, 100 genes were inclued in the CROP-seq experiments. The CROP-seq
     libraries included 2 sgRNAs per gene plus 6 non-targeting control sgRNAs for a
     total of 206 sgRNAs. On Day 10 after CRISPRa neurons were infected by the
     CROP-seq sgRNA library, approximately 50,000 CRISPRi neurons were loaded into
     10X chips with about 25,000 input cells per lane.
 
@@ -1796,36 +1378,28 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def tian_2021_crispri() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """CROP-seq of 98000 neurons treated with 374 gRNAs (CRISPRi only).
 
     For CRISPRi, 184 genes were inclued in the CROP-seq experiments. The CROP-seq
     libraries included 2 sgRNAs per gene plus 6 non-targeting control sgRNAs for a
     total of 374 sgRNAs. On Day 10 after CRISPRi neurons were infected by the
     CROP-seq sgRNA library, approximately 98,000 CRISPRi neurons were loaded into
     10X chips with about 25,000 input cells per lane.
 
 
     Source paper:
         https://doi.org/10.1038/s41593-021-00862-0
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "tian_2021_crispri.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/TianKampmann2021_CRISPRi.h5ad?download=1",
             output_file_name=output_file_name,
@@ -1836,32 +1410,21 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def weinreb_2020() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
-
-    Source paper:
-        https://doi.org/10.1126/science.aaw3381
+    """Mouse embryonic stem cells under different cytokines across time.
 
     The authors developed a tool called LARRY (lineage and RNA recovery) and applied
     it to mouse embryonic stem cells under different cytokine conditions across time.
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "weinreb_2020.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/WeinrebKlein2020.h5ad?download=1",
             output_file_name=output_file_name,
@@ -1872,33 +1435,25 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def xie_2017() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """Transcriptomics of 51448 cells generated with Mosaic-seq.
 
     Mosaic-seq was applied to 71 constituent enhancers from 15 super-enhancers, this
     analysis of 51,448 sgRNA-induced transcriptomes finds that only a small number of
-    constituents are major effectors of target gene expression。
+    constituents are major effectors of target gene expression.
 
     Source paper:
         https://doi.org/10.1016/j.molcel.2017.03.007
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "xie_2017.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/XieHon2017.h5ad?download=1",
             output_file_name=output_file_name,
@@ -1909,35 +1464,27 @@
     else:
         adata = sc.read_h5ad(output_file_path)
 
     return adata
 
 
 def zhao_2021() -> AnnData:  # pragma: no cover
-    """scPerturb Single-Cell Perturbation Data.
-
-    https://github.com/sanderlab/scPerturb
-
-    Reference:
-       Stefan Peidli, Tessa Durakis Green, Ciyue Shen, Torsten Gross, Joseph Min,
-       Jake Taylor-King, Debora Marks, Augustin Luna, Nils Bluthgen, Chris Sander.
-       scPerturb: Information Resource for Harmonized Single-Cell Perturbation Data.
-       bioRxiv 2022.08.20.504663; doi: 10.1101/2022.08.20.504663.
+    """Multiplexed drug perturbation from freshly resected tumors.
 
     Source paper:
         https://doi.org/10.1186/s13073-021-00894-y
 
     This study combines multiplexed drug perturbation in acute slice culture from freshly
     resected tumors with scRNA-seq to profile transcriptome-wide drug responses in
     individual patients. They applied this approach to drug perturbations on slices derived
     from six glioblastoma (GBM) resections to identify conserved drug responses and to one
     additional GBM resection to identify patient-specific responses.
 
     Returns:
-        :class:`~anndata.AnnData` object of scPerturb single-cell perturbation data
+        :class:`~anndata.AnnData` object of scPerturb prepared single-cell perturbation data
     """
     output_file_name = "zhaoSims2021.h5ad"
     output_file_path = settings.datasetdir.__str__() + "/" + output_file_name
     if not Path(output_file_path).exists():
         _download(
             url="https://zenodo.org/record/7278143/files/ZhaoSims2021.h5ad?download=1",
             output_file_name=output_file_name,
```

### Comparing `pertpy-0.3.0/pertpy/plot/_augurpy.py` & `pertpy-0.4.0/pertpy/plot/_augurpy.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.3.0/pertpy/plot/_coda.py` & `pertpy-0.4.0/pertpy/plot/_coda.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from ete3 import CircleFace, NodeStyle, TextFace, Tree, TreeStyle, faces
 from matplotlib import cm, rcParams
 from matplotlib.axes import Axes
 from matplotlib.colors import ListedColormap
 from mudata import MuData
 from statannotations.Annotator import Annotator
 
-from pertpy.tools._base_coda import CompositionalModel2, collapse_singularities_2
+from pertpy.tools._coda._base_coda import CompositionalModel2, collapse_singularities_2
 
 sns.set_style("ticks")
 
 
 class CodaPlot:
     @staticmethod
     def __stackbar(  # pragma: no cover
@@ -898,14 +898,14 @@
             effect_name = [effect_name]
         for _, effect in enumerate(effect_name):
             data_rna.obs[effect] = [data_coda.varm[effect].loc[f"{c}", "Effect"] for c in data_rna.obs[cluster_key]]
         if kwargs.get("vmin"):
             vmin = kwargs["vmin"]
             kwargs.pop("vmin")
         else:
-            vmin = min([data_rna.obs[effect].min() for _, effect in enumerate(effect_name)])
+            vmin = min(data_rna.obs[effect].min() for _, effect in enumerate(effect_name))
         if kwargs.get("vmax"):
             vmax = kwargs["vmax"]
             kwargs.pop("vmax")
         else:
-            vmax = max([data_rna.obs[effect].max() for _, effect in enumerate(effect_name)])
+            vmax = max(data_rna.obs[effect].max() for _, effect in enumerate(effect_name))
         return sc.pl.umap(data_rna, color=effect_name, vmax=vmax, vmin=vmin, ax=ax, show=show, **kwargs)
```

### Comparing `pertpy-0.3.0/pertpy/plot/_milopy.py` & `pertpy-0.4.0/pertpy/plot/_milopy.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.3.0/pertpy/plot/_mixscape.py` & `pertpy-0.4.0/pertpy/plot/_mixscape.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 class MixscapePlot:
     """Plotting functions for Mixscape."""
 
     @staticmethod
     def barplot(  # pragma: no cover
         adata: AnnData,
-        control: str = "NT",
+        guide_rna_column: str,
         mixscape_class_global="mixscape_class_global",
         axis_text_x_size: int = 8,
         axis_text_y_size: int = 6,
         axis_title_size: int = 8,
         strip_text_size: int = 6,
         panel_spacing_x: float = 0.3,
         panel_spacing_y: float = 0.3,
@@ -54,38 +54,38 @@
         show: bool | None = None,
         save: bool | str | None = None,
     ):
         """Barplot to visualize perturbation scores calculated from RunMixscape function.
 
         Args:
             adata: The annotated data object.
-            control: Control category from the `pert_key` column. Default is 'NT'.
+            guide_rna_column: The column of `.obs` with guide RNA labels. The target gene labels. The format must be <gene_target>g<#>. For example, 'STAT2g1' and 'ATF2g1'.
             mixscape_class_global: The column of `.obs` with mixscape global classification result (perturbed, NP or NT).
             show: Show the plot, do not return axis.
             save: If True or a str, save the figure. A string is appended to the default filename. Infer the filetype if ending on {'.pdf', '.png', '.svg'}.
 
         Returns:
             If show is False, return ggplot object used to draw the plot.
         """
         if mixscape_class_global not in adata.obs:
             raise ValueError("Please run `pt.tl.mixscape` first.")
-        count = pd.crosstab(index=adata.obs[mixscape_class_global], columns=adata.obs[control])
+        count = pd.crosstab(index=adata.obs[mixscape_class_global], columns=adata.obs[guide_rna_column])
         all_cells_percentage = pd.melt(count / count.sum(), ignore_index=False).reset_index()
         KO_cells_percentage = all_cells_percentage[all_cells_percentage[mixscape_class_global] == "KO"]
         KO_cells_percentage = KO_cells_percentage.sort_values("value", ascending=False)
 
-        new_levels = KO_cells_percentage[control]
-        all_cells_percentage[control] = pd.Categorical(
-            all_cells_percentage[control], categories=new_levels, ordered=False
+        new_levels = KO_cells_percentage[guide_rna_column]
+        all_cells_percentage[guide_rna_column] = pd.Categorical(
+            all_cells_percentage[guide_rna_column], categories=new_levels, ordered=False
         )
         all_cells_percentage[mixscape_class_global] = pd.Categorical(
             all_cells_percentage[mixscape_class_global], categories=["NT", "NP", "KO"], ordered=False
         )
-        all_cells_percentage["gene"] = all_cells_percentage[control].str.rsplit("g", expand=True)[0]
-        all_cells_percentage["guide_number"] = all_cells_percentage[control].str.rsplit("g", expand=True)[1]
+        all_cells_percentage["gene"] = all_cells_percentage[guide_rna_column].str.rsplit("g", expand=True)[0]
+        all_cells_percentage["guide_number"] = all_cells_percentage[guide_rna_column].str.rsplit("g", expand=True)[1]
         all_cells_percentage["guide_number"] = "g" + all_cells_percentage["guide_number"]
         NP_KO_cells = all_cells_percentage[all_cells_percentage["gene"] != "NT"]
 
         p1 = (
             ggplot(NP_KO_cells, aes(x="guide_number", y="value", fill="mixscape_class_global"))
             + scale_fill_manual(values=["#7d7d7d", "#c9c9c9", "#ff7256"])
             + geom_bar(stat="identity")
@@ -114,32 +114,32 @@
             return p1
 
     @staticmethod
     def heatmap(  # pragma: no cover
         adata: AnnData,
         labels: str,
         target_gene: str,
+        control: str,
         layer: str | None = None,
-        control: str | None = "NT",
         method: str | None = "wilcoxon",
         subsample_number: int | None = 900,
         vmin: float | None = -2,
         vmax: float | None = 2,
         show: bool | None = None,
         save: bool | str | None = None,
         **kwds,
     ):
         """Heatmap plot using mixscape results. Requires `pt.tl.mixscape()` to be run first.
 
         Args:
             adata: The annotated data object.
             labels: The column of `.obs` with target gene labels.
             target_gene: Target gene name to visualize heatmap for.
+            control: Control category from the `pert_key` column.
             layer: Key from `adata.layers` whose value will be used to perform tests on.
-            control: Control category from the `pert_key` column. Default is 'NT'.
             method: The default method is 'wilcoxon', see `method` parameter in `scanpy.tl.rank_genes_groups` for more options.
             subsample_number: Subsample to this number of observations.
             vmin: The value representing the lower limit of the color scale. Values smaller than vmin are plotted with the same color as vmin.
             vmax: The value representing the upper limit of the color scale. Values larger than vmax are plotted with the same color as vmax.
             show: Show the plot, do not return axis.
             save: If `True` or a `str`, save the figure. A string is appended to the default filename. Infer the filetype if ending on {`'.pdf'`, `'.png'`, `'.svg'`}.
             ax: A matplotlib axes object. Only works if plotting a single component.
@@ -203,24 +203,24 @@
             else:
                 perturbation_score = pd.concat([perturbation_score, perturbation_score_temp])
         perturbation_score["mix"] = adata.obs[mixscape_class][perturbation_score.index]
         gd = list(set(perturbation_score[labels]).difference({target_gene}))[0]
         # If before_mixscape is True, split densities based on original target gene classification
         if before_mixscape is True:
             cols = {gd: "#7d7d7d", target_gene: color}
-            p = ggplot(perturbation_score, aes(x="pvec", color="gene_target")) + geom_density() + theme_classic()
+            p = ggplot(perturbation_score, aes(x="pvec", color=labels)) + geom_density() + theme_classic()
             p_copy = copy.deepcopy(p)
             p_copy._build()
             top_r = max(p_copy.layers[0].data["density"])
             perturbation_score["y_jitter"] = perturbation_score["pvec"]
-            perturbation_score.loc[perturbation_score["gene_target"] == gd, "y_jitter"] = np.random.uniform(
-                low=0.001, high=top_r / 10, size=sum(perturbation_score["gene_target"] == gd)
+            perturbation_score.loc[perturbation_score[labels] == gd, "y_jitter"] = np.random.uniform(
+                low=0.001, high=top_r / 10, size=sum(perturbation_score[labels] == gd)
             )
-            perturbation_score.loc[perturbation_score["gene_target"] == target_gene, "y_jitter"] = np.random.uniform(
-                low=-top_r / 10, high=0, size=sum(perturbation_score["gene_target"] == target_gene)
+            perturbation_score.loc[perturbation_score[labels] == target_gene, "y_jitter"] = np.random.uniform(
+                low=-top_r / 10, high=0, size=sum(perturbation_score[labels] == target_gene)
             )
             # If split_by is provided, split densities based on the split_by
             if split_by is not None:
                 perturbation_score["split"] = adata.obs[split_by][perturbation_score.index]
                 p2 = (
                     p
                     + scale_color_manual(values=cols, drop=False)
@@ -500,33 +500,33 @@
                 return axs[0]
             else:
                 return axs
 
     @staticmethod
     def lda(  # pragma: no cover
         adata: AnnData,
+        control: str,
         mixscape_class="mixscape_class",
         mixscape_class_global="mixscape_class_global",
-        control: str | None = "NT",
         perturbation_type: str | None = "KO",
         lda_key: str | None = "mixscape_lda",
         n_components: int | None = None,
         show: bool | None = None,
         save: bool | str | None = None,
         **kwds,
     ):
         """Visualizing perturbation responses with Linear Discriminant Analysis. Requires `pt.tl.mixscape()` to be run first.
 
         Args:
             adata: The annotated data object.
+            control: Control category from the `pert_key` column.
             labels: The column of `.obs` with target gene labels.
             mixscape_class: The column of `.obs` with the mixscape classification result.
             mixscape_class_global: The column of `.obs` with mixscape global classification result (perturbed, NP or NT).
-            control: Control category from the `pert_key` column. Default is 'NT'.
-            perturbation_type: specify type of CRISPR perturbation expected for labeling mixscape classifications. Default is KO.
+            perturbation_type: specify type of CRISPR perturbation expected for labeling mixscape classifications. Defaults to 'KO'.
             lda_key: If not speficied, lda looks .uns["mixscape_lda"] for the LDA results.
             n_components: The number of dimensions of the embedding.
             show: Show the plot, do not return axis.
             save: If `True` or a `str`, save the figure. A string is appended to the default filename. Infer the filetype if ending on {`'.pdf'`, `'.png'`, `'.svg'`}.
             **kwds: Additional arguments to `scanpy.pl.umap`.
         """
         if mixscape_class not in adata.obs:
```

### Comparing `pertpy-0.3.0/pertpy/tools/_augurpy.py` & `pertpy-0.4.0/pertpy/tools/_augur.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     n_estimators: int = 100
     max_depth: int | None = None
     max_features: Literal["auto"] | Literal["log2"] | Literal["sqrt"] | int | float = 2
     penalty: Literal["l1"] | Literal["l2"] | Literal["elasticnet"] | Literal["none"] = "l2"
     random_state: int | None = None
 
 
-class Augurpy:
+class Augur:
     """Python implementation of Augur."""
 
     def __init__(
         self,
         estimator: Literal["random_forest_classifier"]
         | Literal["random_forest_regressor"]
         | Literal["logistic_regression_classifier"],
@@ -128,15 +128,15 @@
             x = input.drop([label_col, cell_type_col], axis=1) if meta is None else input
             adata = AnnData(X=x, obs=pd.DataFrame({"cell_type": cell_type, "label": label}))
 
         if len(adata.obs["label"].unique()) < 2:
             raise ValueError("Less than two unique labels in dataset. At least two are needed for the analysis.")
         # dummy variables for categorical data
         if adata.obs["label"].dtype.name == "category":
-            # filter samples acording to label
+            # filter samples according to label
             if condition_label is not None and treatment_label is not None:
                 print(f"Filtering samples with {condition_label} and {treatment_label} labels.")
                 adata = AnnData.concatenate(
                     adata[adata.obs["label"] == condition_label], adata[adata.obs["label"] == treatment_label]
                 )
             label_encoder = LabelEncoder()
             adata.obs["y_"] = label_encoder.fit_transform(adata.obs["label"])
@@ -194,25 +194,25 @@
                 lambda: LogisticRegression(penalty=params.penalty, random_state=params.random_state),
             )
             c.default(lambda: _raise_exception("Invalid classifer."))
 
         return c.result
 
     def sample(self, adata: AnnData, categorical: bool, subsample_size: int, random_state: int, features: list):
-        """Sample anndata observations.
+        """Sample AnnData observations.
 
         Args:
             adata: Anndata with obs `label` and `cell_type` for label and cell type and dummie variable `y_` columns used as target
             categorical: `True` if target values are categorical
             subsample_size: number of cells to subsample randomly per type from each experimental condition
             random_state: set numpy random seed and sampling seed
             features: features returned Anndata object
 
         Returns:
-            Subsample of anndata object of size subsample_size with given features
+            Subsample of AnnData object of size subsample_size with given features
         """
         # export subsampling.
         random.seed(random_state)
         if categorical:
             label_subsamples = []
             y_encodings = adata.obs["y_"].unique()
             for code in y_encodings:
@@ -538,24 +538,23 @@
         c01 = nobs / 2.0 * (np.log(sigma2_z) - np.log(sigma2_zx))
         v01 = sigma2_x * np.dot(err_xzx.T, err_xzx) / sigma2_zx**2
         q = c01 / np.sqrt(v01)
         pval = 2 * stats.norm.sf(np.abs(q))
 
         return q, pval
 
-    def select_variance(self, adata: AnnData, var_quantile: float, filter_negative_residuals: bool, span: float):
+    def select_variance(self, adata: AnnData, var_quantile: float, filter_negative_residuals: bool, span: float = 0.75):
         """Feature selection based on Augur implementation.
 
         Args:
             adata: Anndata object
-            var_quantile: the quantile below which features will be filtered, based on their residuals in a loess model;
-                defaults to `0.5`
+            var_quantile: The quantile below which features will be filtered, based on their residuals in a loess model.
             filter_negative_residuals: if `True`, filter residuals at a fixed threshold of zero, instead of `var_quantile`
-            span: Smoothing factor, as a fraction of the number of points to take into account. Should be in the range
-                (0, 1]. Default is 0.75
+            span: Smoothing factor, as a fraction of the number of points to take into account.
+                  Should be in the range (0, 1]. Defaults to 0.75
 
         Return:
             AnnData object with additional select_variance column in var.
         """
         adata.var["highly_variable"] = False
         adata.var["means"] = np.ravel(adata.X.mean(axis=0))
         # Converting because the Syntax for power for numpy arrays is different -> use sparse Syntax as default
@@ -631,22 +630,24 @@
             adata: Anndata with obs `label` and `cell_type` for label and cell type and dummie variable `y_` columns used as target
             n_subsamples: number of random subsamples to draw from complete dataset for each cell type
             subsample_size: number of cells to subsample randomly per type from each experimental condition
             folds: number of folds to run cross validation on. Be careful changing this parameter without also changing `subsample_size`.
             min_cells: minimum number of cells for a particular cell type in each condition in order to retain that type for analysis (depricated..)
             feature_perc: proportion of genes that are randomly selected as features for input to the classifier in each
                           subsample using the random gene filter
-            var_quantile: the quantile below which features will be filtered, based on their residuals in a loess model (default: `0.5`)
-            span: Smoothing factor, as a fraction of the number of points to take into account. Should be in the range (0, 1] (default: 0.75)
+            var_quantile: The quantile below which features will be filtered, based on their residuals in a loess model.
+                          Defaults to 0.5.
+            span: Smoothing factor, as a fraction of the number of points to take into account. Should be in the range (0, 1].
+                  Defaults to 0.75.
             filter_negative_residuals: if `True`, filter residuals at a fixed threshold of zero, instead of `var_quantile`
             n_threads: number of threads to use for parallelization
             select_variance_features: Whether to select genes based on the original Augur implementation (True)
-                                      or using scanpy's highly_variable_genes (False) (default: True9
+                                      or using scanpy's highly_variable_genes (False). Defaults to True.
             key_added: Key to add results to in .uns
-            augur_mode: one of default, velocity or permute. Setting augur_mode = "velocity" disables feature selection,
+            augur_mode: One of 'default', 'velocity' or 'permute'. Setting augur_mode = "velocity" disables feature selection,
                         assuming feature selection has been performed by the RNA velocity procedure to produce the input matrix,
                         while setting augur_mode = "permute" will generate a null distribution of AUCs for each cell type by
                         permuting the labels. Note that when setting augur_mode = "permute" n_subsample values less than 100 will be set to 500.
             random_state: set numpy random seed, sampling seed and fold seed
             zero_division: 0 or 1 or `warn`; Sets the value to return when there is a zero division. If
                            set to “warn”, this acts as 0, but warnings are also raised. Precision metric parameter.
 
@@ -771,15 +772,15 @@
         between two conditions respectively compared to the control.
 
         Args:
             augur1: Augurpy results from condition 1, obtained from `predict()[1]`
             augur2: Augurpy results from condition 2, obtained from `predict()[1]`
             permuted1: permuted Augurpy results from condition 1, obtained from `predict()` with argument `augur_mode=permute`
             permuted2: permuted Augurpy results from condition 2, obtained from `predict()` with argument `augur_mode=permute`
-            n_subsamples: number of subsamples to pool when calculating the mean augur score for each permutation; defaults to 50
+            n_subsamples: number of subsamples to pool when calculating the mean augur score for each permutation; Defaults to 50.
             n_permutations: the total number of mean augur scores to calculate from a background distribution
 
         Returns:
             Results object containing mean augur scores.
         """
         # compare available cell types
         cell_types = (
```

### Comparing `pertpy-0.3.0/pertpy/tools/_base_coda.py` & `pertpy-0.4.0/pertpy/tools/_coda/_base_coda.py`

 * *Files 0% similar despite different names*

```diff
@@ -1377,15 +1377,15 @@
 
     """
 
     if type(sample_identifier) == str:
         sample_identifier = [sample_identifier]
 
     if covariate_obs:
-        covariate_obs += sample_identifier
+        covariate_obs += [i for i in sample_identifier if i not in covariate_obs]
     else:
         covariate_obs = sample_identifier  # type: ignore
 
     # join sample identifiers
     if type(sample_identifier) == list:
         adata.obs["scCODA_sample_id"] = adata.obs[sample_identifier].agg("-".join, axis=1)
         sample_identifier = "scCODA_sample_id"
```

### Comparing `pertpy-0.3.0/pertpy/tools/_kernel_pca.py` & `pertpy-0.4.0/pertpy/tools/_kernel_pca.py`

 * *Files identical despite different names*

### Comparing `pertpy-0.3.0/pertpy/tools/_milopy.py` & `pertpy-0.4.0/pertpy/tools/_milo.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     print(
         "[bold yellow]ryp2 is not installed. Install with [green]pip install rpy2 [yellow]to run tools with R support."
     )
 from scipy.sparse import csr_matrix
 from sklearn.metrics.pairwise import euclidean_distances
 
 
-class Milopy:
+class Milo:
     """Python implementation of Milo."""
 
     def __init__(self):
         pass
 
     def load(
         self,
@@ -200,15 +200,15 @@
                 raise
         # Make nhood abundance matrix
         sample_dummies = pd.get_dummies(adata.obs[sample_col])
         all_samples = sample_dummies.columns
         sample_dummies = csr_matrix(sample_dummies.values)
         nhood_count_mat = nhoods.T.dot(sample_dummies)
         sample_obs = pd.DataFrame(index=all_samples)
-        sample_adata = AnnData(X=nhood_count_mat.T, obs=sample_obs)
+        sample_adata = AnnData(X=nhood_count_mat.T, obs=sample_obs, dtype=np.float32)
         sample_adata.uns["sample_col"] = sample_col
         # Save nhood index info
         sample_adata.var["index_cell"] = adata.obs_names[adata.obs["nhood_ixs_refined"] == 1]
         sample_adata.var["kth_distance"] = adata.obs.loc[
             adata.obs["nhood_ixs_refined"] == 1, "nhood_kth_distance"
         ].values
 
@@ -229,33 +229,36 @@
         feature_key: str | None = "rna",
         solver: Literal["edger", "batchglm"] = "edger",
     ):
         """Performs differential abundance testing on neighbourhoods using QLF test implementation as implemented in edgeR.
 
         Args:
             mdata: MuData object
-            design: formula for the test, following glm syntax from R (e.g. '~ condition'). Terms should be columns in `milo_mdata[feature_key].obs`.
-            model_contrasts: A string vector that defines the contrasts used to perform DA testing, following glm syntax from R (e.g. "conditionDisease - conditionControl"). If no contrast is specified (default), then the last categorical level in condition of interest is used as the test group. Defaults to None.
+            design: Formula for the test, following glm syntax from R (e.g. '~ condition').
+                    Terms should be columns in `milo_mdata[feature_key].obs`.
+            model_contrasts: A string vector that defines the contrasts used to perform DA testing, following glm syntax from R (e.g. "conditionDisease - conditionControl").
+                             If no contrast is specified (default), then the last categorical level in condition of interest is used as the test group. Defaults to None.
             subset_samples: subset of samples (obs in `milo_mdata['milo']`) to use for the test. Defaults to None.
             add_intercept: whether to include an intercept in the model. If False, this is equivalent to adding + 0 in the design formula. When model_contrasts is specified, this is set to False by default. Defaults to True.
-            feature_key: If input data is MuData, specify key to cell-level AnnData object. (default: 'rna')
+            feature_key: If input data is MuData, specify key to cell-level AnnData object. Defaults to 'rna'.
             solver: The solver to fit the model to. One of "edger" (requires R, rpy2 and edgeR to be installed) or "batchglm"
 
         Returns:
             None, modifies `milo_mdata['milo']` in place, adding the results of the DA test to `.var`:
             - `logFC` stores the log fold change in cell abundance (coefficient from the GLM)
             - `PValue` stores the p-value for the QLF test before multiple testing correction
             - `SpatialFDR` stores the the p-value adjusted for multiple testing to limit the false discovery rate,
                 calculated with weighted Benjamini-Hochberg procedure
         """
         try:
             sample_adata = mdata["milo"]
         except KeyError:
             print(
-                "[bold red]milo_mdata should be a MuData object with two slots: feature_key and 'milo' - please run milopy.count_nhoods() first"
+                "[bold red]milo_mdata should be a MuData object with two slots:"
+                " feature_key and 'milo' - please run milopy.count_nhoods() first"
             )
             raise
         adata = mdata[feature_key]
 
         covariates = [x.strip(" ") for x in set(re.split("\\+|\\*", design.lstrip("~ ")))]
 
         # Add covariates used for testing to sample_adata.var
@@ -269,15 +272,16 @@
         sample_obs = sample_obs[covariates + [sample_col]]
         sample_obs.index = sample_obs[sample_col].astype("str")
 
         try:
             assert sample_obs.loc[sample_adata.obs_names].shape[0] == len(sample_adata.obs_names)
         except AssertionError:
             print(
-                f"Values in mdata[{feature_key}].obs[{covariates}] cannot be unambiguously assigned to each sample -- each sample value should match a single covariate value"
+                f"Values in mdata[{feature_key}].obs[{covariates}] cannot be unambiguously assigned to each sample"
+                f" -- each sample value should match a single covariate value"
             )
             raise
         sample_adata.obs = sample_obs.loc[sample_adata.obs_names]
 
         # Get design dataframe
         try:
             design_df = sample_adata.obs[covariates]
@@ -361,15 +365,15 @@
         feature_key: str | None = "rna",
     ):
         """Assigns a categorical label to neighbourhoods, based on the most frequent label among cells in each neighbourhood. This can be useful to stratify DA testing results by cell types or samples.
 
         Args:
             mdata: MuData object
             anno_col: Column in adata.obs containing the cell annotations to use for nhood labelling
-            feature_key: If input data is MuData, specify key to cell-level AnnData object. (default: 'rna')
+            feature_key: If input data is MuData, specify key to cell-level AnnData object. Defaults to 'rna'.
 
         Returns:
             None. Adds in place:
             - `milo_mdata['milo'].var["nhood_annotation"]`: assigning a label to each nhood
             - `milo_mdata['milo'].var["nhood_annotation_frac"]` stores the fraciton of cells in the neighbourhood with the assigned label
             - `milo_mdata['milo'].varm['frac_annotation']`: stores the fraction of cells from each label in each nhood
             - `milo_mdata['milo'].uns["annotation_labels"]`: stores the column names for `milo_mdata['milo'].varm['frac_annotation']`
@@ -402,15 +406,15 @@
 
     def annotate_nhoods_continuous(self, mdata: MuData, anno_col: str, feature_key: str | None = "rna"):
         """Assigns a continuous value to neighbourhoods, based on mean cell level covariate stored in adata.obs. This can be useful to correlate DA log-foldChanges with continuous covariates such as pseudotime, gene expression scores etc...
 
         Args:
             mdata: MuData object
             anno_col: Column in adata.obs containing the cell annotations to use for nhood labelling
-            feature_key: If input data is MuData, specify key to cell-level AnnData object. (default: 'rna')
+            feature_key: If input data is MuData, specify key to cell-level AnnData object. Defaults to 'rna'.
 
         Returns:
             None. Adds in place:
             - `milo_mdata['milo'].var["nhood_{anno_col}"]`: assigning a continuous value to each nhood
         """
         if "milo" not in mdata.mod:
             raise ValueError(
@@ -432,15 +436,15 @@
 
     def add_covariate_to_nhoods_var(self, mdata: MuData, new_covariates: list[str], feature_key: str | None = "rna"):
         """Add covariate from cell-level obs to sample-level obs. These should be covariates for which a single value can be assigned to each sample.
 
         Args:
             mdata: MuData object
             new_covariates: columns in `milo_mdata[feature_key].obs` to add to `milo_mdata['milo'].obs`.
-            feature_key: If input data is MuData, specify key to cell-level AnnData object. (default: 'rna')
+            feature_key: If input data is MuData, specify key to cell-level AnnData object. Defaults to 'rna'.
 
         Returns:
             None, adds columns to `milo_mdata['milo']` in place
         """
         try:
             sample_adata = mdata["milo"]
         except KeyError:
@@ -473,15 +477,15 @@
 
     def build_nhood_graph(self, mdata: MuData, basis: str = "X_umap", feature_key: str | None = "rna"):
         """Build graph of neighbourhoods used for visualization of DA results
 
         Args:
             mdata: MuData object
             basis: Name of the obsm basis to use for layout of neighbourhoods (key in `adata.obsm`). Defaults to "X_umap".
-            feature_key: If input data is MuData, specify key to cell-level AnnData object. (default: 'rna')
+            feature_key: If input data is MuData, specify key to cell-level AnnData object. Defaults to 'rna'.
 
         Returns:
             - `milo_mdata['milo'].varp['nhood_connectivities']`: graph of overlap between neighbourhoods (i.e. no of shared cells)
             - `milo_mdata['milo'].var["Nhood_size"]`: number of cells in neighbourhoods
         """
         adata = mdata[feature_key]
         # # Add embedding positions
@@ -499,24 +503,25 @@
 
     def add_nhood_expression(self, mdata: MuData, layer: str | None = None, feature_key: str | None = "rna"):
         """Calculates the mean expression in neighbourhoods of each feature.
 
         Args:
             mdata: MuData object
             layer: If provided, use `milo_mdata[feature_key][layer]` as expression matrix instead of `milo_mdata[feature_key].X`. Defaults to None.
-            feature_key: If input data is MuData, specify key to cell-level AnnData object. (default: 'rna')
+            feature_key: If input data is MuData, specify key to cell-level AnnData object. Defaults to 'rna'.
 
         Returns:
             Updates adata in place to store the matrix of average expression in each neighbourhood in `milo_mdata['milo'].varm['expr']`
         """
         try:
             sample_adata = mdata["milo"]
         except KeyError:
             print(
-                "milo_mdata should be a MuData object with two slots: feature_key and 'milo' - please run milopy.count_nhoods(adata) first"
+                "milo_mdata should be a MuData object with two slots:"
+                " feature_key and 'milo' - please run milopy.count_nhoods(adata) first"
             )
             raise
         adata = mdata[feature_key]
 
         # Get gene expression matrix
         if layer is None:
             X = adata.X
```

### Comparing `pertpy-0.3.0/pertpy/tools/_mixscape.py` & `pertpy-0.4.0/pertpy/tools/_mixscape.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 import pandas as pd
 import scanpy as sc
 from anndata import AnnData
 from pynndescent import NNDescent
 from rich import print
 from scanpy.tools._utils import _choose_representation
 from scipy import sparse
-from scipy.sparse import csr_matrix, issparse
+from scipy.sparse import csr_matrix, issparse, spmatrix
 from sklearn.mixture import GaussianMixture
 
 import pertpy as pt
 
 warnings.simplefilter("ignore")
 
 
 class Mixscape:
     """Python implementation of Mixscape."""
 
     def __init__(self):
         pass
 
-    def pert_sign(
+    def perturbation_signature(
         self,
         adata: AnnData,
         pert_key: str,
         control: str,
         split_by: str | None = None,
         n_neighbors: int = 20,
         use_rep: str | None = None,
@@ -156,29 +156,30 @@
             min_de_genes: Required number of genes that are differentially expressed for method to separate perturbed and non-perturbed cells.
             layer: Key from adata.layers whose value will be used to perform tests on. Default is using `.layers["X_pert"]`.
             logfc_threshold: Limit testing to genes which show, on average, at least X-fold difference (log-scale) between the two groups of cells (default: 0.25).
             iter_num: Number of normalmixEM iterations to run if convergence does not occur.
             split_by: Provide the column `.obs` if multiple biological replicates exist to calculate
                     the perturbation signature for every replicate separately.
             pval_cutoff: P-value cut-off for selection of significantly DE genes.
-            perturbation_type: specify type of CRISPR perturbation expected for labeling mixscape classifications. Default is KO.
+            perturbation_type: specify type of CRISPR perturbation expected for labeling mixscape classifications. Defaults to KO.
             copy: Determines whether a copy of the `adata` is returned.
 
         Returns:
             If `copy=True`, returns the copy of `adata` with the classification result in `.obs`.
             Otherwise writes the results directly to `.obs` of the provided `adata`.
 
             mixscape_class: pandas.Series (`adata.obs['mixscape_class']`).
             Classification result with cells being either classified as perturbed (KO, by default) or non-perturbed (NP) based on their target gene class.
 
             mixscape_class_global: pandas.Series (`adata.obs['mixscape_class_global']`).
             Global classification result (perturbed, NP or NT)
 
             mixscape_class_p_ko: pandas.Series (`adata.obs['mixscape_class_p_ko']`).
-            Posterior probabilities used to determine if a cell is KO (default). Name of this item will change to match perturbation_type parameter setting. (>0.5) or NP
+            Posterior probabilities used to determine if a cell is KO (default).
+            Name of this item will change to match perturbation_type parameter setting. (>0.5) or NP
         """
         if copy:
             adata = adata.copy()
 
         if split_by is None:
             split_masks = [np.full(adata.n_obs, True, dtype=bool)]
             categories = ["all"]
@@ -237,15 +238,18 @@
                         # get average value for each gene over all selected cells
                         # all cells in current split&Gene minus all NT cells in current split
                         # Each row is for each cell, each column is for each gene, get mean for each column
                         vec = np.mean(X[guide_cells][:, de_genes_indices], axis=0) - np.mean(
                             X[nt_cells][:, de_genes_indices], axis=0
                         )
                         # project cells onto the perturbation vector
-                        pvec = np.sum(np.multiply(dat.toarray(), vec), axis=1) / np.sum(np.multiply(vec, vec))
+                        if isinstance(dat, spmatrix):
+                            pvec = np.sum(np.multiply(dat.toarray(), vec), axis=1) / np.sum(np.multiply(vec, vec))
+                        else:
+                            pvec = np.sum(np.multiply(dat, vec), axis=1) / np.sum(np.multiply(vec, vec))
                         pvec = pd.Series(np.asarray(pvec).flatten(), index=list(all_cells.index[all_cells]))
                         if n_iter == 0:
                             gv = pd.DataFrame(columns=["pvec", labels])
                             gv["pvec"] = pvec
                             gv[labels] = control
                             gv.loc[guide_cells, labels] = gene
                             if gene not in gv_list.keys():
@@ -291,39 +295,40 @@
         if copy:
             return adata
 
     def lda(
         self,
         adata: AnnData,
         labels: str,
-        mixscape_class_global="mixscape_class_global",
+        control: str,
+        mixscape_class_global: str | None = "mixscape_class_global",
         layer: str | None = None,
-        control: str | None = "NT",
         n_comps: int | None = 10,
         min_de_genes: int | None = 5,
         logfc_threshold: float | None = 0.25,
         split_by: str | None = None,
         pval_cutoff: float | None = 5e-2,
         perturbation_type: str | None = "KO",
         copy: bool | None = False,
     ):
         """Linear Discriminant Analysis on pooled CRISPR screen data. Requires `pt.tl.mixscape()` to be run first.
 
         Args:
             adata: The annotated data object.
             labels: The column of `.obs` with target gene labels.
+            control: Control category from the `pert_key` column.
             mixscape_class_global: The column of `.obs` with mixscape global classification result (perturbed, NP or NT).
             layer: Key from `adata.layers` whose value will be used to perform tests on.
-            control: Control category from the `pert_key` column. Default is 'NT'.
+            control: Control category from the `pert_key` column. Defaults to 'NT'.
             n_comps: Number of principal components to use. Defaults to 10.
             min_de_genes: Required number of genes that are differentially expressed for method to separate perturbed and non-perturbed cells.
-            logfc_threshold: Limit testing to genes which show, on average, at least X-fold difference (log-scale) between the two groups of cells (default: 0.25).
+            logfc_threshold: Limit testing to genes which show, on average, at least X-fold difference (log-scale) between the two groups of cells. Defaults to 0.25.
             split_by: Provide the column `.obs` if multiple biological replicates exist to calculate
             pval_cutoff: P-value cut-off for selection of significantly DE genes.
-            perturbation_type: specify type of CRISPR perturbation expected for labeling mixscape classifications. Default is KO.
+            perturbation_type: specify type of CRISPR perturbation expected for labeling mixscape classifications. Defaults to KO.
             copy: Determines whether a copy of the `adata` is returned.
 
         Returns:
             If `copy=True`, returns the copy of `adata` with the LDA result in `.uns`.
             Otherwise writes the results directly to `.uns` of the provided `adata`.
 
             mixscape_lda: numpy.ndarray (`adata.uns['mixscape_lda']`).
@@ -377,16 +382,16 @@
         # concatenate all pcs into a single matrix.
         for index, (_, value) in enumerate(projected_pcs.items()):
             if index == 0:
                 projected_pcs_array = value
             else:
                 projected_pcs_array = np.concatenate((projected_pcs_array, value), axis=1)
 
-        clf = LinearDiscriminantAnalysis(n_components=len(np.unique(adata_subset.obs["gene_target"])) - 1)
-        clf.fit(projected_pcs_array, adata_subset.obs["gene_target"])
+        clf = LinearDiscriminantAnalysis(n_components=len(np.unique(adata_subset.obs[labels])) - 1)
+        clf.fit(projected_pcs_array, adata_subset.obs[labels])
         cell_embeddings = clf.transform(projected_pcs_array)
         adata.uns["mixscape_lda"] = cell_embeddings
 
         if copy:
             return adata
 
     def _get_perturbation_markers(
@@ -404,17 +409,17 @@
         """determine gene sets across all splits/groups through differential gene expression
 
         Args:
             adata: :class:`~anndata.AnnData` object
             col_names: Column names to extract the indices for
 
         Returns:
-            Set of column indices
+            Set of column indices.
         """
-        perturbation_markers: dict[tuple, np.ndarray] = {}
+        perturbation_markers: dict[tuple, np.ndarray] = {}  # type: ignore
         for split, split_mask in enumerate(split_masks):
             category = categories[split]
             # get gene sets for each split
             genes = list(set(adata[split_mask].obs[labels]).difference([control]))
             adata_split = adata[split_mask].copy()
             # find top DE genes between cells with targeting and non-targeting gRNAs
             sc.tl.rank_genes_groups(
```

### Comparing `pertpy-0.3.0/pertpy/tools/_sccoda.py` & `pertpy-0.4.0/pertpy/tools/_coda/_sccoda.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from anndata import AnnData
 from jax import random
 from jax.config import config
 from mudata import MuData
 from numpyro.infer import Predictive
 from rich import print
 
-from pertpy.tools._base_coda import CompositionalModel2, from_scanpy
+from pertpy.tools._coda._base_coda import CompositionalModel2, from_scanpy
 
 config.update("jax_enable_x64", True)
 
 
 class Sccoda(CompositionalModel2):
 
     """
@@ -61,14 +61,18 @@
         covariate_obs: list[str] | None = None,
         covariate_df: pd.DataFrame | None = None,
         modality_key_1: str = "rna",
         modality_key_2: str = "coda",
     ) -> MuData:
         """Prepare a MuData object for subsequent processing. If type is "cell_level", then create a compositional analysis dataset from the input adata.
 
+        When using ``type="cell_level"``, ``adata`` needs to have a column in ``adata.obs`` that contains the cell type assignment.
+        Further, it must contain one column or a set of columns (e.g. subject id, treatment, disease status) that uniquely identify each (statistical) sample.
+        Further covariates (e.g. subject age) can either be specified via addidional column names in ``adata.obs``, a key in ``adata.uns``, or as a separate DataFrame.
+
         Args:
             adata: AnnData object.
             type : Specify the input adata type, which could be either a cell-level AnnData or an aggregated sample-level AnnData.
             cell_type_identifier: If type is "cell_level", specify column name in adata.obs that specifies the cell types. Defaults to None.
             sample_identifier: If type is "cell_level", specify column name in adata.obs that specifies the sample. Defaults to None.
             covariate_uns: If type is "cell_level", specify key for adata.uns, where covariate values are stored. Defaults to None.
             covariate_obs: If type is "cell_level", specify list of keys for adata.obs, where covariate values are stored. Defaults to None.
@@ -185,15 +189,15 @@
 
         if is_MuData:
             data.mod[modality_key] = adata
             return data
         else:
             return adata
 
-    def model(
+    def model(  # type: ignore
         self,
         counts: np.ndarray,
         covariates: np.ndarray,
         n_total: np.ndarray,
         ref_index,
         sample_adata: AnnData,
     ):
@@ -267,15 +271,15 @@
             )
 
         # Calculate DM-distributed counts
         predictions = npy.sample("counts", npd.DirichletMultinomial(concentrations, n_total), obs=counts)
 
         return predictions
 
-    def make_arviz(
+    def make_arviz(  # type: ignore
         self,
         data: AnnData | MuData,
         modality_key: str = "coda",
         rng_key=None,
         num_prior_samples: int = 500,
         use_posterior_predictive: bool = True,
     ) -> az.InferenceData:
```

### Comparing `pertpy-0.3.0/pertpy/tools/_tasccoda.py` & `pertpy-0.4.0/pertpy/tools/_coda/_tasccoda.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from anndata import AnnData
 from jax import random
 from jax.config import config
 from mudata import MuData
 from numpyro.infer import Predictive
 from rich import print
 
-from pertpy.tools._base_coda import (
+from pertpy.tools._coda._base_coda import (
     CompositionalModel2,
     collapse_singularities,
     collapse_singularities_2,
     from_scanpy,
     get_a,
     get_a_2,
     import_tree,
@@ -74,14 +74,18 @@
         add_level_name: bool = True,
         key_added: str = "tree",
         modality_key_1: str = "rna",
         modality_key_2: str = "coda",
     ) -> MuData:
         """Prepare a MuData object for subsequent processing. If type is "cell_level", then create a compositional analysis dataset from the input adata. If type is "sample_level", generate ete tree for tascCODA models from dendrogram information or cell-level observations.
 
+        When using ``type="cell_level"``, ``adata`` needs to have a column in ``adata.obs`` that contains the cell type assignment.
+        Further, it must contain one column or a set of columns (e.g. subject id, treatment, disease status) that uniquely identify each (statistical) sample.
+        Further covariates (e.g. subject age) can either be specified via addidional column names in ``adata.obs``, a key in ``adata.uns``, or as a separate DataFrame.
+
         Args:
             adata: AnnData object.
             type: Specify the input adata type, which could be either a cell-level AnnData or an aggregated sample-level AnnData.
             cell_type_identifier: If type is "cell_level", specify column name in adata.obs that specifies the cell types. Defaults to None.
             sample_identifier: If type is "cell_level", specify column name in adata.obs that specifies the sample. Defaults to None.
             covariate_uns: If type is "cell_level", specify key for adata.uns, where covariate values are stored. Defaults to None.
             covariate_obs: If type is "cell_level", specify list of keys for adata.obs, where covariate values are stored. Defaults to None.
@@ -297,15 +301,15 @@
         adata.uns["scCODA_params"]["select_type"] = "sslasso"
         if is_MuData:
             data.mod[modality_key] = adata
             return data
         else:
             return adata
 
-    def model(
+    def model(  # type: ignore
         self,
         counts: np.ndarray,
         covariates: np.ndarray,
         n_total: int,
         ref_index: np.ndarray,
         sample_adata: AnnData,
     ):
@@ -414,15 +418,15 @@
             )
 
         # Calculate DM-distributed counts
         predictions = npy.sample("counts", npd.DirichletMultinomial(concentrations, n_total), obs=counts)
 
         return predictions
 
-    def make_arviz(
+    def make_arviz(  # type: ignore
         self,
         data: AnnData | MuData,
         modality_key: str = "coda",
         rng_key=None,
         num_prior_samples: int = 500,
         use_posterior_predictive: bool = True,
     ) -> az.InferenceData:
```

### Comparing `pertpy-0.3.0/pyproject.toml` & `pertpy-0.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pertpy"
-version = "0.3.0"  # <<COOKIETEMPLE_FORCE_BUMP>>
-description = "Perturbation Analysis in the Scanpy ecosystem."
+version = "0.4.0"  # <<COOKIETEMPLE_FORCE_BUMP>>
+description = "Perturbation Analysis in the scverse ecosystem."
 authors = ["Lukas Heumos <lukas.heumos@posteo.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/theislab/pertpy"
 repository = "https://github.com/theislab/pertpy"
 documentation = "https://pertpy.readthedocs.io"
 packages = [
@@ -15,36 +15,41 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 
 [tool.poetry.dependencies]
-python = ">=3.8.0,<3.10"
-click = ">=7.0.0"
+python = ">=3.8.0,<3.11"
 rich = ">=10.11.0"
 PyYAML = ">=5.4.1"
 scanpy = ">=1.8.1"
 pypi-latest = ">=0.1.1"
 muon = ">=0.1.2"
 requests = ">=2.27.1"
 ipywidgets = ">=7.6.5"
 switchlang = "^0.1.0"
 scikit-misc = "^0.1.4"
 plotnine = "^0.10.1"
 leidenalg = "^0.9.0"
 scipy = "^1.9.3"
-ete3 = "^3.1.2"
-pyqt5 = "^5.15.7"
-toytree = "^2.0.1"
-arviz = "^0.14.0"
-numpyro = "^0.10.1"
+scvi-tools = "^0.19.0"
 adjusttext = "^0.7.3"
+toytree = "^2.0.1"
+arviz = ">=0.14,<0.16"
+numpyro = ">=0.10.1,<0.12.0"
 statannotations = "^0.5.0"
 protobuf = "3.20.1"
+numba = "^0.56.4"
+decoupler = "^1.3.3"
+ete3 = {version = "^3.1.2", optional = true}
+pyqt5 = {version = "^5.15.9", optional = true}
+ott-jax = "^0.4.0"
+pandas = "<=2.0.0"
+sparsecca = "^0.3.0"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6.2.5"
 coverage = {extras = ["toml"], version = ">=6.2"}
 safety = ">=1.9.0"
 mypy = ">=0.930"
 typeguard = ">=2.13.3"
@@ -57,21 +62,18 @@
 flake8-bandit = ">=2.1.2"
 flake8-bugbear = ">=21.11.29"
 flake8-docstrings = ">=1.5.0"
 flake8-rst-docstrings = ">=0.2.5"
 pep8-naming = ">=0.12.1"
 reorder-python-imports = ">=2.6.0"
 pre-commit-hooks = ">=4.1.0"
-sphinx-rtd-theme = ">=1.0.0"
-sphinx-click = ">=3.0.1"
 Pygments = ">=2.11.1"
 types-pkg-resources = ">=0.1.3"
 types-requests = ">=2.27.4"
 types-attrs = ">=19.1.0"
-sphinx-rtd-dark-mode = ">=1.2.4"
 Jinja2 = ">=3.0.3"
 pyenchant = ">=3.2.1"
 nbsphinx = ">=0.8.8"
 sphinx-gallery = ">0.6,<0.11"
 sphinx-autodoc-typehints = ">=1.12.0"
 sphinx-last-updated-by-git = ">=0.3.0"
 sphinxcontrib-bibtex = ">=2.4.1"
@@ -81,14 +83,17 @@
 pyupgrade = ">=2.31.0"
 furo = ">=2022.3.4"
 myst-parser = ">=0.17.0"
 sphinx-remove-toctrees = ">=0.0.3"
 sphinx-design = ">=0.0.13"
 sphinxext-opengraph = ">=0.6.2"
 
+[tool.poetry.extras]
+ete3 = ["ete3"]
+
 [tool.poetry.scripts]
 pertpy = "pertpy.__main__:main"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 
 [tool.black]
```

### Comparing `pertpy-0.3.0/PKG-INFO` & `pertpy-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 Metadata-Version: 2.1
 Name: pertpy
-Version: 0.3.0
-Summary: Perturbation Analysis in the Scanpy ecosystem.
+Version: 0.4.0
+Summary: Perturbation Analysis in the scverse ecosystem.
 Home-page: https://github.com/theislab/pertpy
 License: MIT
 Author: Lukas Heumos
 Author-email: lukas.heumos@posteo.net
-Requires-Python: >=3.8.0,<3.10
+Requires-Python: >=3.8.0,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: ete3
 Requires-Dist: PyYAML (>=5.4.1)
 Requires-Dist: adjusttext (>=0.7.3,<0.8.0)
-Requires-Dist: arviz (>=0.14.0,<0.15.0)
-Requires-Dist: click (>=7.0.0)
-Requires-Dist: ete3 (>=3.1.2,<4.0.0)
+Requires-Dist: arviz (>=0.14,<0.16)
+Requires-Dist: decoupler (>=1.3.3,<2.0.0)
+Requires-Dist: ete3 (>=3.1.2,<4.0.0) ; extra == "ete3"
 Requires-Dist: ipywidgets (>=7.6.5)
 Requires-Dist: leidenalg (>=0.9.0,<0.10.0)
 Requires-Dist: muon (>=0.1.2)
-Requires-Dist: numpyro (>=0.10.1,<0.11.0)
+Requires-Dist: numba (>=0.56.4,<0.57.0)
+Requires-Dist: numpyro (>=0.10.1,<0.12.0)
+Requires-Dist: ott-jax (>=0.4.0,<0.5.0)
+Requires-Dist: pandas (<=2.0.0)
 Requires-Dist: plotnine (>=0.10.1,<0.11.0)
 Requires-Dist: protobuf (==3.20.1)
 Requires-Dist: pypi-latest (>=0.1.1)
-Requires-Dist: pyqt5 (>=5.15.7,<6.0.0)
+Requires-Dist: pyqt5 (>=5.15.9,<6.0.0)
 Requires-Dist: requests (>=2.27.1)
 Requires-Dist: rich (>=10.11.0)
 Requires-Dist: scanpy (>=1.8.1)
 Requires-Dist: scikit-misc (>=0.1.4,<0.2.0)
 Requires-Dist: scipy (>=1.9.3,<2.0.0)
+Requires-Dist: scvi-tools (>=0.19.0,<0.20.0)
+Requires-Dist: sparsecca (>=0.3.0,<0.4.0)
 Requires-Dist: statannotations (>=0.5.0,<0.6.0)
 Requires-Dist: switchlang (>=0.1.0,<0.2.0)
 Requires-Dist: toytree (>=2.0.1,<3.0.0)
 Project-URL: Documentation, https://pertpy.readthedocs.io
 Project-URL: Repository, https://github.com/theislab/pertpy
 Description-Content-Type: text/markdown
```

