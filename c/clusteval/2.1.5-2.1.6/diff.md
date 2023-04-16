# Comparing `tmp/clusteval-2.1.5.tar.gz` & `tmp/clusteval-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clusteval-2.1.5.tar", last modified: Wed Mar 22 21:09:29 2023, max compression
+gzip compressed data, was "clusteval-2.1.6.tar", last modified: Sun Apr 16 21:42:59 2023, max compression
```

## Comparing `clusteval-2.1.5.tar` & `clusteval-2.1.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 21:09:29.911212 clusteval-2.1.5/
--rw-rw-rw-   0        0        0     1146 2021-03-30 18:41:22.000000 clusteval-2.1.5/LICENSE
--rw-rw-rw-   0        0        0        0 2021-03-30 18:41:22.000000 clusteval-2.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     8061 2023-03-22 21:09:29.910215 clusteval-2.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     7437 2022-03-10 23:45:16.000000 clusteval-2.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-22 21:09:29.892251 clusteval-2.1.5/clusteval/
--rw-rw-rw-   0        0        0     1040 2023-03-22 21:08:40.000000 clusteval-2.1.5/clusteval/__init__.py
--rw-rw-rw-   0        0        0    23532 2022-09-24 18:49:41.000000 clusteval-2.1.5/clusteval/clusteval.py
--rw-rw-rw-   0        0        0     2015 2019-11-07 18:23:03.000000 clusteval-2.1.5/clusteval/coord2density.py
--rw-rw-rw-   0        0        0     7797 2021-11-26 13:10:54.000000 clusteval-2.1.5/clusteval/dbindex.py
--rw-rw-rw-   0        0        0     7765 2023-03-22 20:52:50.000000 clusteval-2.1.5/clusteval/dbscan.py
--rw-rw-rw-   0        0        0     6587 2022-03-09 18:46:14.000000 clusteval-2.1.5/clusteval/derivative.py
--rw-rw-rw-   0        0        0     8737 2022-03-19 22:21:20.000000 clusteval-2.1.5/clusteval/examples.py
--rw-rw-rw-   0        0        0     7505 2022-03-19 22:19:36.000000 clusteval-2.1.5/clusteval/hdbscan.py
--rw-rw-rw-   0        0        0      311 2021-07-01 20:07:09.000000 clusteval-2.1.5/clusteval/image2vec.py
--rw-rw-rw-   0        0        0     2841 2021-03-30 18:41:22.000000 clusteval-2.1.5/clusteval/plot_dendrogram.py
--rw-rw-rw-   0        0        0    12780 2022-03-19 21:43:36.000000 clusteval-2.1.5/clusteval/silhouette.py
-drwxrwxrwx   0        0        0        0 2023-03-22 21:09:29.909217 clusteval-2.1.5/clusteval/tests/
--rw-rw-rw-   0        0        0        0 2022-03-19 22:32:41.000000 clusteval-2.1.5/clusteval/tests/__init__.py
--rw-rw-rw-   0        0        0     3361 2022-03-19 22:30:57.000000 clusteval-2.1.5/clusteval/tests/test_clusteval.py
-drwxrwxrwx   0        0        0        0 2023-03-22 21:09:29.907249 clusteval-2.1.5/clusteval.egg-info/
--rw-rw-rw-   0        0        0     8061 2023-03-22 21:09:28.000000 clusteval-2.1.5/clusteval.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-03-22 21:09:29.000000 clusteval-2.1.5/clusteval.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 21:09:28.000000 clusteval-2.1.5/clusteval.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2023-03-22 21:09:29.000000 clusteval-2.1.5/clusteval.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-22 21:09:29.000000 clusteval-2.1.5/clusteval.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-22 21:09:29.912210 clusteval-2.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1468 2022-12-02 15:04:10.000000 clusteval-2.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:42:59.546082 clusteval-2.1.6/
+-rw-rw-rw-   0        0        0     1146 2023-04-10 15:32:29.000000 clusteval-2.1.6/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-04-10 15:32:29.000000 clusteval-2.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     7990 2023-04-16 21:42:59.545086 clusteval-2.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7437 2023-04-10 15:32:29.000000 clusteval-2.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 21:42:59.498415 clusteval-2.1.6/clusteval/
+-rw-rw-rw-   0        0        0     1118 2023-04-16 21:39:47.000000 clusteval-2.1.6/clusteval/__init__.py
+-rw-rw-rw-   0        0        0    36815 2023-04-16 21:40:29.000000 clusteval-2.1.6/clusteval/clusteval.py
+-rw-rw-rw-   0        0        0     2015 2023-04-10 15:32:29.000000 clusteval-2.1.6/clusteval/coord2density.py
+-rw-rw-rw-   0        0        0     8104 2023-04-15 13:48:17.000000 clusteval-2.1.6/clusteval/dbindex.py
+-rw-rw-rw-   0        0        0     8604 2023-04-16 14:21:20.000000 clusteval-2.1.6/clusteval/dbscan.py
+-rw-rw-rw-   0        0        0     6909 2023-04-15 14:19:24.000000 clusteval-2.1.6/clusteval/derivative.py
+-rw-rw-rw-   0        0        0    19051 2023-04-16 18:54:34.000000 clusteval-2.1.6/clusteval/examples.py
+-rw-rw-rw-   0        0        0     7479 2023-04-11 18:26:51.000000 clusteval-2.1.6/clusteval/hdbscan.py
+-rw-rw-rw-   0        0        0      311 2023-04-10 15:32:29.000000 clusteval-2.1.6/clusteval/image2vec.py
+-rw-rw-rw-   0        0        0     2841 2023-04-10 15:32:29.000000 clusteval-2.1.6/clusteval/plot_dendrogram.py
+-rw-rw-rw-   0        0        0    14601 2023-04-16 18:33:43.000000 clusteval-2.1.6/clusteval/silhouette.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:42:59.544089 clusteval-2.1.6/clusteval/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-10 15:32:29.000000 clusteval-2.1.6/clusteval/tests/__init__.py
+-rw-rw-rw-   0        0        0     6418 2023-04-16 18:50:37.000000 clusteval-2.1.6/clusteval/tests/test_clusteval.py
+-rw-rw-rw-   0        0        0     2696 2023-04-16 18:40:14.000000 clusteval-2.1.6/clusteval/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:42:59.539103 clusteval-2.1.6/clusteval.egg-info/
+-rw-rw-rw-   0        0        0     7990 2023-04-16 21:42:59.000000 clusteval-2.1.6/clusteval.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2023-04-16 21:42:59.000000 clusteval-2.1.6/clusteval.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 21:42:59.000000 clusteval-2.1.6/clusteval.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-04-16 21:42:59.000000 clusteval-2.1.6/clusteval.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-16 21:42:59.000000 clusteval-2.1.6/clusteval.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 21:42:59.546082 clusteval-2.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1456 2023-04-16 16:29:41.000000 clusteval-2.1.6/setup.py
```

### Comparing `clusteval-2.1.5/LICENSE` & `clusteval-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clusteval-2.1.5/PKG-INFO` & `clusteval-2.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: clusteval
-Version: 2.1.5
-Summary: clusteval is a python package that provides various methods for unsupervised cluster validation.
+Version: 2.1.6
+Summary: clusteval is a python package for unsupervised cluster validation.
 Home-page: https://erdogant.github.io/clusteval
-Download-URL: https://github.com/erdogant/clusteval/archive/2.1.5.tar.gz
+Download-URL: https://github.com/erdogant/clusteval/archive/2.1.6.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -182,9 +180,7 @@
 * https://machinelearningmastery.com/face-recognition-using-principal-component-analysis/
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
 	Star it if you like it!
-
-
```

#### html2text {}

```diff
@@ -1,54 +1,53 @@
-Metadata-Version: 2.1 Name: clusteval Version: 2.1.5 Summary: clusteval is a
-python package that provides various methods for unsupervised cluster
-validation. Home-page: https://erdogant.github.io/clusteval Download-URL:
-https://github.com/erdogant/clusteval/archive/2.1.5.tar.gz Author: Erdogan
-Taskesen Author-email: erdogant@gmail.com License: UNKNOWN Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
-LICENSE # clusteval [![Python](https://img.shields.io/pypi/pyversions/
-clusteval)](https://img.shields.io/pypi/pyversions/clusteval) [![PyPI Version]
-(https://img.shields.io/pypi/v/clusteval)](https://pypi.org/project/clusteval/
-) [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://
-github.com/erdogant/clusteval/blob/master/LICENSE) [![BuyMeCoffee](https://
-img.shields.io/badge/buymea-coffee-yellow.svg)](https://www.buymeacoffee.com/
-erdogant) [![Github Forks](https://img.shields.io/github/forks/erdogant/
-clusteval.svg)](https://github.com/erdogant/clusteval/network) [![GitHub Open
-Issues](https://img.shields.io/github/issues/erdogant/clusteval.svg)](https://
-github.com/erdogant/clusteval/issues) [![Project Status](http://
-www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/
-#active) [![Downloads](https://pepy.tech/badge/clusteval/month)](https://
-pepy.tech/project/clusteval) [![Downloads](https://pepy.tech/badge/clusteval)]
-(https://pepy.tech/project/clusteval) [![DOI](https://zenodo.org/badge/
-232915924.svg)](https://zenodo.org/badge/latestdoi/232915924) [![Sphinx](https:
-//img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
-clusteval/) [![Open In Colab](https://colab.research.google.com/assets/colab-
-badge.svg)](https://erdogant.github.io/clusteval/pages/html/
-Documentation.html#colab-notebook)  ``clusteval`` is a python package that is
-developed to evaluate detected clusters and return the cluster labels that have
-most optimal **clustering tendency**, **Number of clusters** and **clustering
-quality**. Multiple evaluation strategies are implemented for the evaluation;
-**silhouette**, **dbindex**, and **derivative**, and four clustering methods
-can be used: **agglomerative**, **kmeans**, **dbscan** and **hdbscan**. #
-**â­ï¸ Star this repo if you like it â­ï¸** # ### Blogs Read the blog to
-get a structured overview how you can use ``clusteval``. * [Medium Blog: A
-step-by-step guide for clustering images](https://towardsdatascience.com/a-
-step-by-step-guide-for-clustering-images-4b45f9906128) In case you want to
-detect identical images, you can also use hash functionalities. * [Medium Blog:
-Detection of Duplicate Images Using Image Hash Functions](https://
-towardsdatascience.com/detection-of-duplicate-images-using-image-hash-
-functions-4d9c53f04a75) # ### [Documentation pages](https://erdogant.github.io/
-clusteval/) On the [documentation pages](https://erdogant.github.io/clusteval/
-) you can find detailed information about the working of the ``clusteval`` with
-many examples. # ### Installation ##### It is advisable to create a new
-environment (e.g. with Conda). ```bash conda create -n env_clusteval python=3.8
-conda activate clusteval ``` ##### Install from PyPI ```bash pip install
-clusteval ``` ##### Import library ```python from clusteval import clusteval
-```
+Metadata-Version: 2.1 Name: clusteval Version: 2.1.6 Summary: clusteval is a
+python package for unsupervised cluster validation. Home-page: https://
+erdogant.github.io/clusteval Download-URL: https://github.com/erdogant/
+clusteval/archive/2.1.6.tar.gz Author: Erdogan Taskesen Author-email:
+erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3 Description-Content-Type: text/markdown
+License-File: LICENSE # clusteval [![Python](https://img.shields.io/pypi/
+pyversions/clusteval)](https://img.shields.io/pypi/pyversions/clusteval) [!
+[PyPI Version](https://img.shields.io/pypi/v/clusteval)](https://pypi.org/
+project/clusteval/) [![License](https://img.shields.io/badge/license-MIT-
+green.svg)](https://github.com/erdogant/clusteval/blob/master/LICENSE) [!
+[BuyMeCoffee](https://img.shields.io/badge/buymea-coffee-yellow.svg)](https://
+www.buymeacoffee.com/erdogant) [![Github Forks](https://img.shields.io/github/
+forks/erdogant/clusteval.svg)](https://github.com/erdogant/clusteval/network)
+[![GitHub Open Issues](https://img.shields.io/github/issues/erdogant/
+clusteval.svg)](https://github.com/erdogant/clusteval/issues) [![Project
+Status](http://www.repostatus.org/badges/latest/active.svg)](http://
+www.repostatus.org/#active) [![Downloads](https://pepy.tech/badge/clusteval/
+month)](https://pepy.tech/project/clusteval) [![Downloads](https://pepy.tech/
+badge/clusteval)](https://pepy.tech/project/clusteval) [![DOI](https://
+zenodo.org/badge/232915924.svg)](https://zenodo.org/badge/latestdoi/232915924)
+[![Sphinx](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
+erdogant.github.io/clusteval/) [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://erdogant.github.io/
+clusteval/pages/html/Documentation.html#colab-notebook)  ``clusteval`` is a
+python package that is developed to evaluate detected clusters and return the
+cluster labels that have most optimal **clustering tendency**, **Number of
+clusters** and **clustering quality**. Multiple evaluation strategies are
+implemented for the evaluation; **silhouette**, **dbindex**, and
+**derivative**, and four clustering methods can be used: **agglomerative**,
+**kmeans**, **dbscan** and **hdbscan**. # **â­ï¸ Star this repo if you like
+it â­ï¸** # ### Blogs Read the blog to get a structured overview how you can
+use ``clusteval``. * [Medium Blog: A step-by-step guide for clustering images]
+(https://towardsdatascience.com/a-step-by-step-guide-for-clustering-images-
+4b45f9906128) In case you want to detect identical images, you can also use
+hash functionalities. * [Medium Blog: Detection of Duplicate Images Using Image
+Hash Functions](https://towardsdatascience.com/detection-of-duplicate-images-
+using-image-hash-functions-4d9c53f04a75) # ### [Documentation pages](https://
+erdogant.github.io/clusteval/) On the [documentation pages](https://
+erdogant.github.io/clusteval/) you can find detailed information about the
+working of the ``clusteval`` with many examples. # ### Installation ##### It is
+advisable to create a new environment (e.g. with Conda). ```bash conda create -
+n env_clusteval python=3.8 conda activate clusteval ``` ##### Install from PyPI
+```bash pip install clusteval ``` ##### Import library ```python from clusteval
+import clusteval ```
 ===============================================================================
 ### Examples A structured overview of all examples are now available on the
 [documentation pages](https://erdogant.github.io/clusteval/).
 ===============================================================================
 * [Example: Cluster validation using Silhouette score](https://
 erdogant.github.io/clusteval/pages/html/Examples.html#cluster-evaluation)
 [https://github.com/erdogant/clusteval/blob/master/docs/figs/fig1b_sil.png]
```

### Comparing `clusteval-2.1.5/README.md` & `clusteval-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `clusteval-2.1.5/clusteval/__init__.py` & `clusteval-2.1.6/clusteval/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 from clusteval.clusteval import (
     import_example,
     dbindex,
     silhouette,
     derivative,
     dbscan,
+    # hdbscan_custom,
     )
 
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '2.1.5'
+__version__ = '2.1.6'
 
 
 __doc__ = """
 clusteval
 =====================================================================
 
 Description
@@ -39,14 +40,17 @@
 >>>
 >>> # Make plot
 >>> ce.plot()
 >>>
 >>> # Scatter plot
 >>> ce.scatter(X)
 >>>
+>>> # Silhouette plot
+>>> ce.plot_silhouette(X)
+>>>
 >>> # Dendrogram
 >>> ce.dendrogram()
 
 
 References
 ----------
 * https://github.com/erdogant/clusteval
```

### Comparing `clusteval-2.1.5/clusteval/coord2density.py` & `clusteval-2.1.6/clusteval/coord2density.py`

 * *Files identical despite different names*

### Comparing `clusteval-2.1.5/clusteval/dbindex.py` & `clusteval-2.1.6/clusteval/derivative.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -----------------------------------------------
-# Name        : dbindex.py
+# Name        : derivative.py
 # Author      : E.Taskesen
 # Contact     : erdogant@gmail.com
 # Licence     : MIT
 # Respect the autor and leave this here
 # -----------------------------------------------
 
 import numpy as np
-import pandas as pd
-from tqdm import tqdm
-import matplotlib.pyplot as plt
-from scipy.spatial.distance import euclidean
 from scipy.cluster.hierarchy import fcluster
-from scipy.cluster.hierarchy import linkage as scipy_linkage
-from sklearn.cluster import KMeans, MiniBatchKMeans
+from scipy.cluster.hierarchy import linkage as linkage_scipy
+import matplotlib.pyplot as plt
+from clusteval.utils import init_logger, set_logger, set_font_properties
+logger = init_logger()
 
 
-# %% main
-def fit(X, cluster='agglomerative', metric='euclidean', linkage='ward', min_clust=2, max_clust=25, Z=None, savemem=False, verbose=3):
+# %% Main
+def fit(X, cluster='agglomerative', metric='euclidean', linkage='ward', min_clust=2, max_clust=25, Z=None, verbose='info'):
     """ Determine optimal number of clusters using dbindex.
 
     Description
     -----------
-    This function return the cluster labels for the optimal cutt-off based on the choosen hierarchical clustering method.
+    This function returns the cluster labels for the optimal cutt-off based on the choosen hierarchical clustering method.
+    The derivative or inconsistence method is one of the defaults for the fcluster() function in scipy.
+    It compares each cluster merge's height h to the average avg and normalizing it by the standard deviation std formed over the depth previous levels.
 
     Parameters
     ----------
     X : Numpy-array.
         The rows are the features and the colums are the samples.
     cluster : str, (default: 'agglomerative')
         Clustering method type for clustering.
@@ -34,186 +34,150 @@
             * 'kmeans'
     metric : str, (default: 'euclidean').
         Distance measure for the clustering, such as 'euclidean','hamming', etc.
     linkage : str, (default: 'ward')
         Linkage type for the clustering.
         'ward','single',',complete','average','weighted','centroid','median'.
     min_clust : int, (default: 2)
-        Minimum number of clusters (>=).
+        Number of clusters that is evaluated greater or equals to min_clust.
     max_clust : int, (default: 25)
-        Maximum number of clusters (<=).
+        Number of clusters that is evaluated smaller or equals to max_clust.
     Z : Object, (default: None).
         This will speed-up computation if you readily have Z. e.g., Z=linkage(X, method='ward', metric='euclidean').
-    savemem : bool, (default: False)
-        Save memmory when working with large datasets. Note that htis option only in case of KMeans.
     verbose : int, optional (default: 3)
         Print message to screen [1-5]. The larger the number, the more information.
 
     Returns
     -------
     dict. with various keys. Note that the underneath keys can change based on the used methodtype.
-    method: str
+    evaluate: str
         Method name that is used for cluster evaluation.
-    score: pd.DataFrame()
-        The scoring values per clusters.
+    score: None
+        Nothing in here but incuded for consistency
     labx: list
         Cluster labels.
     fig: list
         Relevant information to make the plot.
 
     Examples
     --------
     >>> # Import library
-    >>> import clusteval.dbindex as dbindex
+    >>> import clusteval.derivative as derivative
     >>> from sklearn.datasets import make_blobs
     >>> Generate demo data
     >>> X, labels_true = make_blobs(n_samples=750, centers=6, n_features=10)
     >>> # Fit with default parameters
-    >>> results = dbindex.fit(X)
+    >>> results = derivative.fit(X)
     >>> # plot
-    >>> dbindex.plot(results)
+    >>> derivative.plot(results)
+
     """
-    # Make dictionary to store Parameters
     Param = {}
     Param['verbose'] = verbose
     Param['cluster'] = cluster
     Param['metric'] = metric
     Param['linkage'] = linkage
     Param['min_clust'] = min_clust
     Param['max_clust'] = max_clust
-    Param['savemem'] = savemem
-    if verbose>=3: print('[clusteval] >Evaluate using dbindex.')
 
-    # Savemem for kmeans
+    set_logger(verbose=verbose)
+    # Make all possible cluster-cut-offs
+    logger.info('Evaluate clustering using [derivatives] method')
+
     if Param['cluster']=='kmeans':
-        if Param['savemem']:
-            kmeansmodel=MiniBatchKMeans
-            print('[clusteval] >Save memory enabled for kmeans.')
-        else:
-            kmeansmodel=KMeans
+        logger.info('Does not work with Kmeans! <return>')
+        results = {}
+        results['evaluate']='derivative'
+        results['labx'] = None
+        results['score'] = None
+        results['fig'] = {}
+        results['fig']['last_rev'] = None
+        results['fig']['acceleration_rev'] = None
+        return results
 
     # Cluster hierarchical using on metric/linkage
-    if (Z is None) and (Param['cluster']!='kmeans'):
-        Z = scipy_linkage(X, method=Param['linkage'], metric=Param['metric'])
-
-    # Setup storing parameters
-    clustcutt = np.arange(Param['min_clust'], Param['max_clust'])
-    scores = np.zeros((len(clustcutt))) * np.nan
-    dbclust = np.zeros((len(clustcutt))) * np.nan
-    clustlabx = []
+    if Z is None:
+        Z = linkage_scipy(X, method=Param['linkage'], metric=Param['metric'])
 
     # Run over all cluster cutoffs
-    for i in tqdm(range(len(clustcutt))):
-        # Cut the dendrogram for i clusters
-        if Param['cluster']=='kmeans':
-            labx=kmeansmodel(n_clusters=clustcutt[i], verbose=0).fit(X).labels_
-        else:
-            labx = fcluster(Z, clustcutt[i], criterion='maxclust')
-
-        # Store labx for cluster-cut
-        clustlabx.append(labx)
-        # Store number of unique clusters
-        dbclust[i]=len(np.unique(labx))
-        # Compute silhouette (can only be done if more then 1 cluster)
-        if dbclust[i]>1:
-            scores[i]=_dbindex_score(X, labx)
+    last = Z[-max_clust:, 2]
+    last_rev = last[::-1]
+
+    acceleration = np.diff(last, 2)  # 2nd derivative of the distances
+    acceleration_rev = acceleration[::-1]
+
+    # Only focus on the min-max clusters
+    acceleration_rev[:Param['min_clust']]=0
+    acceleration_rev[Param['max_clust']:]=0
+    last_rev[:Param['min_clust']]=0
+    last_rev[Param['max_clust']:]=0
+
+    k = acceleration_rev.argmax() + 2  # if idx 0 is the max of this we want 2 clusters
+    logger.info('Clusters: %d' %k)
+
+    # Now use the optimal cluster cut-off for the selection of clusters
+    clustlabx = fcluster(Z, k, criterion='maxclust')
 
     # Convert to array
     clustlabx = np.array(clustlabx)
 
-    # Store only if agrees to restriction of input clusters number
-    I1 = np.isnan(scores)==False
-    I2 = dbclust>=Param['min_clust']
-    I3 = dbclust<=Param['max_clust']
-    Iloc = I1 & I2 & I3
-
-    # Get only clusters of interest
-    if sum(Iloc)>0:
-        scores = scores[Iloc]
-        dbclust = dbclust[Iloc]
-        clustlabx = clustlabx[Iloc, :]
-        clustcutt = clustcutt[Iloc]
-        idx = np.argmin(scores)
-        clustlabx = clustlabx[idx, :] - 1
-    else:
-        if verbose>=3: print('[clusteval] >No clusters detected.')
-        if len(clustlabx.shape)>1:
-            clustlabx = np.zeros(clustlabx.shape[1]).astype(int)
-        else:
-            clustlabx = [0]
-
     # Store results
     results = {}
-    results['evaluate'] = 'dbindex'
-    results['score'] = pd.DataFrame(np.array([dbclust, scores]).T, columns=['clusters', 'score'])
-    results['score'].clusters = results['score'].clusters.astype(int)
+    results['evaluate']='derivative'
     results['labx'] = clustlabx
+    results['score'] = None
     results['fig'] = {}
-    results['fig']['dbclust'] = dbclust
-    results['fig']['scores'] = scores
-    results['fig']['clustcutt'] = clustcutt
-
+    results['fig']['last_rev'] = last_rev
+    results['fig']['acceleration_rev'] = acceleration_rev
     # Return
-    return(results)
-
-
-# %% Compute DB-score
-def _dbindex_score(X, labels):
-    n_cluster = np.unique(labels)
-    cluster_k=[]
-    for k in range(0, len(n_cluster)):
-        cluster_k.append(X[labels==n_cluster[k]])
-
-    centroids = [np.mean(k, axis=0) for k in cluster_k]
-    variances = [np.mean([euclidean(p, centroids[i]) for p in k]) for i, k in enumerate(cluster_k)]
-
-    db = []
-    for i in range(0, len(n_cluster)):
-        for j in range(0, len(n_cluster)):
-            if n_cluster[j] != n_cluster[i]:
-                db.append((variances[i] + variances[j]) / euclidean(centroids[i], centroids[j]))
+    return results
 
-    outscore = np.max(db) / len(n_cluster)
-    return(outscore)
 
-
-# %% plot
-def plot(results, title='Davies Bouldin index vs. nr.clusters', figsize=(15, 8), ax=None, visible=True):
+# %% Plot
+def plot(results, title='Derivative (Elbow method)', xlabel='Nr. Clusters', ylabel='Score', font_properties={}, figsize=(15,8), ax=None, showfig=True, verbose=3):
     """Make plot for the gridsearch over the number of clusters.
 
     Parameters
     ----------
     results : dict.
         Dictionary that is the output of the .fit() function.
     figsize : tuple, (default: (15,8))
         Figure size, (heigh,width).
+    verbose : int, optional (default: 3)
+        Print message to screen [1-5]. The larger the number, the more information.
 
     Returns
     -------
     tuple, (fig, ax)
         Figure and axis of the figure.
 
     """
-    idx = np.argmin(results['fig']['scores'])
+    # Set font properties
+    font_properties = set_font_properties(font_properties)
     fig=None
+    if title is None: title='Derivative (Elbow method)'
+    idxs = np.arange(1, len(results['fig']['last_rev']) + 1)
+    k = results['fig']['acceleration_rev'].argmax() + 2  # if idx 0 is the max of this we want 2 clusters
+
     # Make figure
     if ax is None:
-        fig, ax = plt.subplots(figsize=figsize)
+        fig, ax = plt.subplots(figsize=figsize, dpi=100)
     # Plot
-    ax.plot(results['fig']['dbclust'], results['fig']['scores'], color='k')
+    ax.plot(idxs, results['fig']['last_rev'])
+    ax.plot(idxs[:-2] + 1, results['fig']['acceleration_rev'])
+
     # Plot optimal cut
-    ax.axvline(x=results['fig']['clustcutt'][idx], ymin=0, ymax=results['fig']['dbclust'][idx], linewidth=2, color='r', linestyle="--")
+    ax.axvline(x=k, ymin=0, linewidth=2, color='r', linestyle="--")
     # Set fontsizes
-    plt.rc('axes', titlesize=14)     # fontsize of the axes title
-    plt.rc('xtick', labelsize=10)     # fontsize of the axes title
-    plt.rc('ytick', labelsize=10)     # fontsize of the axes title
-    plt.rc('font', size=10)
+    # plt.rc('axes', titlesize=14)     # fontsize of the axes title
+    plt.rc('xtick', labelsize=font_properties['size_x_axis'])  # fontsize of the axes title
+    plt.rc('ytick', labelsize=font_properties['size_y_axis'])  # fontsize of the axes title
+    # plt.rc('font', size=10)
     # Set labels
-    ax.set_xticks(results['fig']['clustcutt'])
-    ax.set_xlabel('#Clusters')
-    ax.set_ylabel('Score')
-    ax.set_title(title)
+    ax.set_xticks(np.arange(0, len(idxs)))
+    ax.set_xlabel(xlabel, fontsize=font_properties['size_x_axis'])
+    ax.set_ylabel(ylabel, fontsize=font_properties['size_y_axis'])
+    ax.set_title(title, fontsize=font_properties['size_title'])
     ax.grid(color='grey', linestyle='--', linewidth=0.2)
-    if visible:
-        plt.show()
+    if showfig: plt.show()
     # Return
-    return(fig, ax)
+    return fig, ax
```

### Comparing `clusteval-2.1.5/clusteval/hdbscan.py` & `clusteval-2.1.6/clusteval/hdbscan.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 
 from sklearn import metrics
 import numpy as np
 from sklearn.preprocessing import StandardScaler
 import hdbscan as hdb
 import seaborn as sns
 import matplotlib.pyplot as plt
+from clusteval.utils import init_logger, set_logger
+logger = init_logger()
 
 
 # %% Main
-def fit(X, metric='euclidean', min_clust=2, min_samples=None, norm=True, n_jobs=-1, verbose=3):
+def fit(X, metric='euclidean', min_clust=2, min_samples=None, norm=True, n_jobs=-1, verbose='info'):
     """ Determine optimal number of clusters using dbindex.
 
     Description
     -----------
     This function return the cluster labels for the optimal cutt-off based on the choosen hierarchical clustering method.
 
     Parameters
@@ -73,17 +75,18 @@
     Param = {}
     Param['min_samples'] = min_samples
     Param['min_clust'] = min_clust
     Param['metric'] = metric
     Param['n_jobs'] = n_jobs
     Param['norm'] = norm
     Param['gen_min_span_tree'] = False
-
     Param['min_samples'] = None if min_samples is None else (int(np.floor(min_samples * X.shape[0])))  # Set max. outliers
-    # if verbose>=3: print('[clusteval] >Fit using hdbscan.')
+
+    set_logger(verbose=verbose)
+    # logger.info('Fit using hdbscan.')
 
     # Transform X
     if Param['norm']:
         X = StandardScaler().fit_transform(X)
 
     # Set parameters for hdbscan
     model = hdb.HDBSCAN(algorithm='best', metric=Param['metric'], min_samples=Param['min_samples'], core_dist_n_jobs=Param['n_jobs'], min_cluster_size=int(Param['min_clust']), p=None, gen_min_span_tree=Param['gen_min_span_tree'])
@@ -96,22 +99,20 @@
     results['cluster_persistence'] = model.cluster_persistence_  # A score of how persistent each cluster is. A score of 1.0 represents a perfectly stable cluster that persists over all distance scales, while a score of 0.0 represents a perfectly ephemeral cluster. These scores can be guage the relative coherence of the clusters resultsput by the algorithm.
     results['outlier'] = model.outlier_scores_  # Outlier scores for clustered points; the larger the score the more outlier-like the point. Useful as an outlier detection technique. Based on the GLOSH algorithm by Campello, Moulavi, Zimek and Sander.
     # out2['predict'] = model.prediction_data_  # Cached data used for predicting the cluster labels of new or unseen points. Necessary only if you are using functions from hdbscan.prediction (see approximate_predict(), membership_vector(), and all_points_membership_vectors()).
     results['min_clust'] = Param['min_clust']
     results['model'] = model
 
     # Some info
-    if verbose>=3:
-        n_clusters = len(set(results['labx'])) - (1 if -1 in results['labx'] else 0)
-        print('[clusteval] >Estimated number of clusters: %d' % n_clusters)
-
-        if n_clusters!=X.shape[0] and n_clusters>1:
-            print("[clusteval] >Silhouette Coefficient: %0.3f" % metrics.silhouette_score(X, results['labx']))
+    n_clusters = len(set(results['labx'])) - (1 if -1 in results['labx'] else 0)
+    logger.info('Estimated number of clusters: %d' % n_clusters)
+    if n_clusters!=X.shape[0] and n_clusters>1:
+        logger.info("Silhouette Coefficient: %0.3f" % metrics.silhouette_score(X, results['labx']))
 
-    return(results)
+    return results
 
 
 # %% Plot
 def plot(results, figsize=(15, 8), savefig={'fname': None, format: 'png', 'dpi ': None, 'orientation': 'portrait', 'facecolor': 'auto'}, verbose=3):
     """Make plot for the gridsearch over the number of clusters.
 
     Parameters
@@ -153,24 +154,24 @@
 
     fig3, ax3 = plt.subplots(figsize=figsize)
     model.condensed_tree_.plot(select_clusters=True, selection_palette=sns.color_palette())
 
     # Save figure
     if (fname is not None) and (fig1 is not None):
         savefig['fname'] = fname + '_linkage_tree'
-        if verbose>=3: print('[clusteval] >Saving linkage_tree: [%s]' %(savefig['fname']))
+        logger.info('Saving linkage_tree: [%s]' %(savefig['fname']))
         fig1.savefig(**savefig)
 
     # Save figure
     if (fname is not None) and (fig2 is not None):
         savefig['fname'] = fname + '_condensed_tree'
-        if verbose>=3: print('[clusteval] >Saving condensed_tree_: [%s]' %(savefig['fname']))
+        logger.info('Saving condensed_tree_: [%s]' %(savefig['fname']))
         fig2.savefig(**savefig)
 
     # Save figure
     if (fname is not None) and (fig3 is not None):
         savefig['fname'] = fname + '_linkage_tree_focus'
-        if verbose>=3: print('[clusteval] >Saving condensed_tree with focus: [%s]' %(savefig['fname']))
+        logger.info('Saving condensed_tree with focus: [%s]' %(savefig['fname']))
         fig3.savefig(**savefig)
 
     # Return
     return ((fig1, fig2, fig3), (ax1, ax2, ax3))
```

### Comparing `clusteval-2.1.5/clusteval/plot_dendrogram.py` & `clusteval-2.1.6/clusteval/plot_dendrogram.py`

 * *Files identical despite different names*

### Comparing `clusteval-2.1.5/clusteval/silhouette.py` & `clusteval-2.1.6/clusteval/silhouette.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,27 +2,37 @@
 # Name        : silhouette.py
 # Author      : E.Taskesen
 # Contact     : erdogant@gmail.com
 # Licence     : MIT
 # Respect the autor and leave this here
 #-----------------------------------------------
 
+import colourmap
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 import matplotlib.cm as cm
 import matplotlib.pyplot as plt
 from scipy.cluster.hierarchy import fcluster
 from scipy.cluster.hierarchy import linkage as scipy_linkage
 from sklearn.cluster import KMeans, MiniBatchKMeans
-from sklearn.metrics import silhouette_score, silhouette_samples, silhouette_score
-
+from sklearn.metrics import silhouette_samples, silhouette_score
+from clusteval.utils import init_logger, set_logger, disable_tqdm, set_font_properties, compute_embedding
+logger = init_logger()
 
 # %% Main
-def fit(X, cluster='agglomerative', metric='euclidean', linkage='ward', min_clust=2, max_clust=25, Z=None, savemem=False, verbose=3):
+def fit(X,
+        cluster='agglomerative',
+        metric='euclidean',
+        linkage='ward',
+        min_clust=2,
+        max_clust=25,
+        Z=None,
+        savemem=False,
+        verbose='info'):
     """This function return the cluster labels for the optimal cutt-off based on the choosen hierarchical clustering evaluate.
 
     Parameters
     ----------
     X : Numpy-array,
         Where rows is features and colums are samples.
     cluster : str, (default: 'agglomerative')
@@ -35,19 +45,17 @@
         Linkage type for the clustering.
         'ward','single',',complete','average','weighted','centroid','median'.
     min_clust : int, (default: 2)
         Number of clusters that is evaluated greater or equals to min_clust.
     max_clust : int, (default: 25)
         Number of clusters that is evaluated smaller or equals to max_clust.
     savemem : bool, (default: False)
-        Save memmory when working with large datasets. Note that htis option only in case of KMeans.
+        Save memmory when working with large datasets. Note that this option only works in case of KMeans.
     Z : Object, (default: None).
         This will speed-up computation if you readily have Z. e.g., Z=linkage(X, method='ward', metric='euclidean').
-    verbose : int, optional (default: 3)
-        Print message to screen [1-5]. The larger the number, the more information is returned.
 
     Returns
     -------
     dict. with various keys. Note that the underneath keys can change based on the used evaluatetype.
     evaluate: str
         evaluate name that is used for cluster evaluation.
     score: pd.DataFrame()
@@ -84,43 +92,43 @@
     References
     ----------
     http://scikit-learn.org/stable/auto_examples/cluster/plot_kmeans_silhouette_analysis.html
 
     """
     # Make dictionary to store Parameters
     Param = {}
-    Param['verbose'] = verbose
     Param['cluster'] = cluster
     Param['metric'] = metric
     Param['linkage'] = linkage
     Param['min_clust'] = min_clust
     Param['max_clust'] = max_clust
     Param['savemem'] = savemem
-    if verbose>=3: print('[clusteval] >Evaluate using silhouette.')
+    set_logger(verbose=verbose)
+    logger.info('Evaluate using silhouette.')
 
     # Savemem for kmeans
     if Param['cluster']=='kmeans':
         if Param['savemem']:
             kmeansmodel = MiniBatchKMeans
-            if Param['verbose']>=3: print('[clusteval] >Save memory enabled for kmeans with evaluation silhouette.')
+            logger.info('Save memory enabled for kmeans with evaluation silhouette.')
         else:
             kmeansmodel = KMeans
 
     # Cluster hierarchical using on metric/linkage
     if (Z is None) and (Param['cluster']!='kmeans'):
         Z = scipy_linkage(X, method=Param['linkage'], metric=Param['metric'])
 
     # Setup storing parameters
     clustcutt = np.arange(Param['min_clust'], Param['max_clust'])
     silscores = np.zeros((len(clustcutt))) * np.nan
     sillclust = np.zeros((len(clustcutt))) * np.nan
     clustlabx = []
 
     # Run over all cluster cutoffs
-    for i in tqdm(range(len(clustcutt))):
+    for i in tqdm(range(len(clustcutt)), disable=disable_tqdm(), desc='[clusteval] >INFO'):
         # Cut the dendrogram for i clusters
         if Param['cluster']=='kmeans':
             labx = kmeansmodel(n_clusters=clustcutt[i], verbose=0).fit(X).labels_
         else:
             labx = fcluster(Z, clustcutt[i], criterion='maxclust')
 
         # Store labx for cluster-cut
@@ -136,52 +144,55 @@
 
     # Store only if agrees to restriction of input clusters number
     I1 = np.isnan(silscores)==False
     I2 = sillclust>=Param['min_clust']
     I3 = sillclust<=Param['max_clust']
     Iloc = I1 & I2 & I3
 
-    if verbose>=5:
-        print(clustlabx)
-        print('Iloc: %s' %(str(Iloc)))
-        print('silscores: %s' %(str(silscores)))
-        print('sillclust: %s' %(str(sillclust)))
-        print('clustlabx: %s' %(str(clustlabx)))
+    logger.debug(clustlabx)
+    logger.debug('Iloc: %s' %(str(Iloc)))
+    logger.debug('silscores: %s' %(str(silscores)))
+    logger.debug('sillclust: %s' %(str(sillclust)))
+    logger.debug('clustlabx: %s' %(str(clustlabx)))
 
     if sum(Iloc)>0:
         # Get only clusters of interest
         silscores = silscores[Iloc]
         sillclust = sillclust[Iloc]
         clustlabx = clustlabx[Iloc, :]
         clustcutt = clustcutt[Iloc]
         idx = np.argmax(silscores)
         clustlabx = clustlabx[idx, :] - 1
     else:
-        if verbose>=3: print('[clusteval] >No clusters detected.')
+        logger.info('No clusters detected.')
         if len(clustlabx.shape)>1:
             clustlabx = np.zeros(clustlabx.shape[1]).astype(int)
         else:
             clustlabx = [0]
 
     # Store results
+    sillclust=sillclust.astype(int)
+    clustcutt=clustcutt.astype(int)
     results = {}
     results['evaluate']='silhouette'
-    results['score'] = pd.DataFrame(np.array([sillclust, silscores]).T, columns=['clusters', 'score'])
+    results['score'] = pd.DataFrame(np.array([clustcutt, sillclust, silscores]).T, columns=['cluster_threshold', 'clusters', 'score'])
     results['score']['clusters'] = results['score']['clusters'].astype(int)
+    results['score']['cluster_threshold'] = results['score']['cluster_threshold'].astype(int)
     results['labx'] = clustlabx
     results['fig'] = {}
     results['fig']['silscores'] = silscores
     results['fig']['sillclust'] = sillclust
     results['fig']['clustcutt'] = clustcutt
 
     # Return
-    return(results)
+    return results
+
 
 # %% plot
-def plot(results, title='Silhouette vs. nr.clusters', figsize=(15, 8), ax=None, visible=True):
+def plot(results, title='Silhouette score', xlabel='Nr. Clusters', ylabel='Score', font_properties={}, figsize=(15, 8), ax=None, showfig=True):
     """Make plot for the gridsearch over the number of clusters.
 
     Parameters
     ----------
     results : dict.
         Dictionary that is the output of the .fit() function.
     figsize : tuple, (default: (15,8))
@@ -189,52 +200,63 @@
 
     Returns
     -------
     tuple, (fig, ax)
         Figure and axis of the figure.
 
     """
+    # Set font properties
+    font_properties = set_font_properties(font_properties)
     fig=None
     idx = np.argmax(results['fig']['silscores'])
+
     # Make figure
     if ax is None:
-        fig, ax = plt.subplots(figsize=figsize)
+        fig, ax = plt.subplots(figsize=figsize, dpi=100)
+
     # Plot
-    ax.plot(results['fig']['sillclust'], results['fig']['silscores'], color='k')
+    # ax.plot(results['fig']['sillclust'], results['fig']['silscores'], color='k')
+    ax.plot(results['fig']['clustcutt'], results['fig']['silscores'], color='k')
     # Plot optimal cut
     ax.axvline(x=results['fig']['clustcutt'][idx], ymin=0, ymax=results['fig']['sillclust'][idx], linewidth=2, color='r', linestyle="--")
     # Set fontsizes
-    plt.rc('axes', titlesize=14)  # fontsize of the axes title
-    plt.rc('xtick', labelsize=10)  # fontsize of the axes title
-    plt.rc('ytick', labelsize=10)  # fontsize of the axes title
-    plt.rc('font', size=10)
+    ax.tick_params(axis='x', labelsize=font_properties['size_x_axis'])
+    ax.tick_params(axis='y', labelsize=font_properties['size_y_axis'])
     # Set labels
     ax.set_xticks(results['fig']['clustcutt'])
-    ax.set_xlabel('#Clusters')
-    ax.set_ylabel('Score')
-    ax.set_title(title)
+    ax.set_xticklabels(results['fig']['sillclust'])
+    ax.set_xlabel(xlabel, fontsize=font_properties['size_x_axis'])
+    ax.set_ylabel(ylabel, fontsize=font_properties['size_y_axis'])
+    ax.set_title(title, fontsize=font_properties['size_title'])
     ax.grid(color='grey', linestyle='--', linewidth=0.2)
-    if visible:
+
+    if showfig:
         plt.show()
     # Return
-    return(fig, ax)
+    return fig, ax
 
 
 # %% Scatter data
-def scatter(y, X=None, dot_size=50, figsize=(15, 8), savefig={'fname': None, format: 'png', 'dpi ': None, 'orientation': 'portrait', 'facecolor': 'auto'}, verbose=3):
+def scatter(y, X=None, dot_size=50, jitter=None, embedding=None, cmap='tab20c', figsize=(15, 8), font_properties={'size_title': 14, 'size_x_axis': 14, 'size_y_axis': 14}, savefig={'fname': None, format: 'png', 'dpi ': None, 'orientation': 'portrait', 'facecolor': 'auto'}, showfig=True):
     """Make scatter for the cluster labels with the samples.
 
     Parameters
     ----------
     y: list
         Cluster labels for the samples in X (some order).
     X : Numpy-array,
         Where rows is features and colums are samples. The first two columns of the matrix are used for plotting. Note that it is also possible provide tSNE coordinates for a better representation of the data.
     dot_size : int, (default: 50)
         Size of the dot in the scatterplot
+    jitter : float, default: None
+        Add jitter to data points as random normal data. Values of 0.01 is usually good for one-hot data seperation.
+    embedding : str (default: None)
+        In case high dimensional data, a embedding with t-SNE can be performed.
+        * None
+        * 'tsne'
     savefig : dict.
         https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.savefig.html
         {'dpi':'figure',
         'format':None,
         'metadata':None,
         'bbox_inches': None,
         'pad_inches':0.1,
@@ -246,84 +268,104 @@
 
     Returns
     -------
     tuple, (fig, ax1, ax2)
         Figure and axis of the figure.
 
     """
+    font_properties = set_font_properties(font_properties)
     fig, ax1, ax2 = None, None, None
     if X is None:
-        if verbose>=2: print('[clusteval] >Warning: Input data X is required for the scatterplot.')
+        logger.warning('Input data X is required for the scatterplot.')
         return None
 
+    # Compute embedding
+    X = compute_embedding(X, embedding, logger)
+
+    if X.shape[1]>2:
+        logger.info('Scatterplot is performed on the first two dimensions of input data X.')
+        X = X[:, :2]
+
     # Extract label from dict
     if isinstance(y, dict):
         y = y.get('labx', None)
+
     # Check y
     if (y is None) or (len(np.unique(y))==1):
-        if verbose>=3: print('[clusteval] >Error: No valid labels provided.')
+        logger.error('No valid labels provided.')
         return None
 
+    # Add jitter
+    if jitter is not None:
+        X = X + np.random.normal(0, jitter, size=X.shape)
+
     # Plot silhouette samples plot
-    # n_clusters = len(np.unique(y))
     n_clusters = len(set(y)) - (1 if -1 in y else 0)
     silhouette_avg = silhouette_score(X, y)
-    if verbose>=3: print('[clusteval] >Estimated number of n_clusters: %d, average silhouette_score=%.3f' %(n_clusters, silhouette_avg))
+    logger.info('Estimated number of n_clusters: %d, average silhouette_score=%.3f' %(n_clusters, silhouette_avg))
 
     # Compute the silhouette scores for each sample
     sample_silhouette_values = silhouette_samples(X, y)
 
     # Create a subplot with 1 row and 2 columns
-    fig, (ax1, ax2) = plt.subplots(1, 2, figsize=figsize)
+    fig, (ax1, ax2) = plt.subplots(1, 2, figsize=figsize, dpi=100)
     fig.set_size_inches(18, 7)
     ax1.set_xlim([-0.1, 1])
 
     # plots of individual clusters, to demarcate them clearly.
     ax1.set_ylim([0, len(X) + (n_clusters + 1) * 10])
     y_lower = 10
     uiclust = np.unique(y)
+    colors = colourmap.fromlist(uiclust, cmap=cmap, scheme='hex')[1]
 
     # Make 1st plot
-    for i in range(0, len(uiclust)):
+    for label in uiclust:
         # Aggregate the silhouette scores for samples belonging to
         # cluster i, and sort them
-        ith_cluster_silhouette_values = sample_silhouette_values[y == uiclust[i]]
+        Iloc = y == label
+        ith_cluster_silhouette_values = sample_silhouette_values[Iloc]
         ith_cluster_silhouette_values.sort()
-
         size_cluster_i = ith_cluster_silhouette_values.shape[0]
         y_upper = y_lower + size_cluster_i
-        color = cm.Set2(float(i) / n_clusters)
-
-        ax1.fill_betweenx(np.arange(y_lower, y_upper), 0, ith_cluster_silhouette_values, facecolor=color, edgecolor=color, alpha=0.7)
-        # ax1.fill_betweenx(np.arange(y_lower, y_upper), 0, ith_cluster_silhouette_values, facecolor=getcolors[i], edgecolor=getcolors[i], alpha=0.7)
+        ax1.fill_betweenx(np.arange(y_lower, y_upper), 0, ith_cluster_silhouette_values, facecolor=colors[label], edgecolor=colors[label], alpha=0.7)
         # Label the silhouette plots with their cluster numbers at the middle
-        ax1.text(-0.05, y_lower + 0.5 * size_cluster_i, str(uiclust[i]))
+        ax1.text(-0.05, y_lower + 0.5 * size_cluster_i, str(label))
         # Compute the new y_lower for next plot
         y_lower = y_upper + 10  # 10 for the 0 samples
-
-    ax1.set_title("The silhouette plot for the various clusters")
-    ax1.set_xlabel("The silhouette coefficient values")
-    ax1.set_ylabel("Cluster label")
+        # Scatter
+        ax2.scatter(X[Iloc, 0], X[Iloc, 1], marker='.', s=dot_size, lw=0, alpha=0.8, c=colors[label], edgecolor='k')
+        ax2.text(X[Iloc, 0].mean(), X[Iloc, 1].mean(), label, c='#000000')
+
+    # Set ax properties
+    ax1.set_title("Sample-wise silhouette scores across the clusters", fontsize=font_properties['size_title'])
+    ax1.set_xlabel("The silhouette coefficient values", fontsize=font_properties['size_x_axis'])
+    ax1.set_ylabel("Cluster label", fontsize=font_properties['size_y_axis'])
     # The vertical line for average silhouette score of all the values
     ax1.axvline(x=silhouette_avg, color="red", linestyle="--")
-    ax1.set_yticks([])  # Clear the yaxis labels / ticks
     ax1.set_xticks([-0.1, 0, 0.2, 0.4, 0.6, 0.8, 1])
     ax1.grid(color='grey', linestyle='--', linewidth=0.2)
+    # Set fontsizes
+    ax1.tick_params(axis='x', labelsize=font_properties['size_x_axis'])
+    ax1.tick_params(axis='y', labelsize=font_properties['size_y_axis'])
+    ax1.set_yticks([])  # Clear the yaxis labels / ticks
 
     # 2nd Plot showing the actual clusters formed
-    color = cm.Set2(y.astype(float) / n_clusters)
-    ax2.scatter(X[:, 0], X[:, 1], marker='.', s=dot_size, lw=0, alpha=0.8, c=color, edgecolor='k')
     ax2.grid(color='grey', linestyle='--', linewidth=0.2)
-    ax2.set_title("Estimated cluster labels")
-    ax2.set_xlabel("1st feature")
-    ax2.set_ylabel("2nd feature")
+    ax2.set_title("Cluster labels", fontsize=font_properties['size_title'])
+    ax2.set_xlabel("1st feature", fontsize=font_properties['size_x_axis'])
+    ax2.set_ylabel("2nd feature", fontsize=font_properties['size_y_axis'])
+    # Set fontsizes
+    ax2.tick_params(axis='x', labelsize=font_properties['size_x_axis'])
+    ax2.tick_params(axis='y', labelsize=font_properties['size_y_axis'])
+
     # General title
-    plt.suptitle(("Silhouette analysis results in n_clusters = %d" %(n_clusters)), fontsize=14, fontweight='bold')
-    plt.show()
+    plt.suptitle(("Silhouette analysis. Detected clusters: %d" %(n_clusters)), fontsize=font_properties['size_title'])
+    if showfig:
+        plt.show()
 
     # Save figure
     if (savefig['fname'] is not None) and (fig is not None):
-        if verbose>=3: print('[clusteval] >Saving silhouetteplot to [%s]' %(savefig['fname']))
+        logger.info('Saving silhouetteplot to [%s]' %(savefig['fname']))
         fig.savefig(**savefig)
 
     # Return
-    return(fig, ax1, ax2)
+    return fig, ax1, ax2
```

### Comparing `clusteval-2.1.5/clusteval.egg-info/PKG-INFO` & `clusteval-2.1.6/clusteval.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: clusteval
-Version: 2.1.5
-Summary: clusteval is a python package that provides various methods for unsupervised cluster validation.
+Version: 2.1.6
+Summary: clusteval is a python package for unsupervised cluster validation.
 Home-page: https://erdogant.github.io/clusteval
-Download-URL: https://github.com/erdogant/clusteval/archive/2.1.5.tar.gz
+Download-URL: https://github.com/erdogant/clusteval/archive/2.1.6.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -182,9 +180,7 @@
 * https://machinelearningmastery.com/face-recognition-using-principal-component-analysis/
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://erdogant.github.io/donate/?currency=USD&amount=5">Coffee</a> for this work, it is very appreciated :)
 	Star it if you like it!
-
-
```

#### html2text {}

```diff
@@ -1,54 +1,53 @@
-Metadata-Version: 2.1 Name: clusteval Version: 2.1.5 Summary: clusteval is a
-python package that provides various methods for unsupervised cluster
-validation. Home-page: https://erdogant.github.io/clusteval Download-URL:
-https://github.com/erdogant/clusteval/archive/2.1.5.tar.gz Author: Erdogan
-Taskesen Author-email: erdogant@gmail.com License: UNKNOWN Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
-LICENSE # clusteval [![Python](https://img.shields.io/pypi/pyversions/
-clusteval)](https://img.shields.io/pypi/pyversions/clusteval) [![PyPI Version]
-(https://img.shields.io/pypi/v/clusteval)](https://pypi.org/project/clusteval/
-) [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://
-github.com/erdogant/clusteval/blob/master/LICENSE) [![BuyMeCoffee](https://
-img.shields.io/badge/buymea-coffee-yellow.svg)](https://www.buymeacoffee.com/
-erdogant) [![Github Forks](https://img.shields.io/github/forks/erdogant/
-clusteval.svg)](https://github.com/erdogant/clusteval/network) [![GitHub Open
-Issues](https://img.shields.io/github/issues/erdogant/clusteval.svg)](https://
-github.com/erdogant/clusteval/issues) [![Project Status](http://
-www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/
-#active) [![Downloads](https://pepy.tech/badge/clusteval/month)](https://
-pepy.tech/project/clusteval) [![Downloads](https://pepy.tech/badge/clusteval)]
-(https://pepy.tech/project/clusteval) [![DOI](https://zenodo.org/badge/
-232915924.svg)](https://zenodo.org/badge/latestdoi/232915924) [![Sphinx](https:
-//img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/
-clusteval/) [![Open In Colab](https://colab.research.google.com/assets/colab-
-badge.svg)](https://erdogant.github.io/clusteval/pages/html/
-Documentation.html#colab-notebook)  ``clusteval`` is a python package that is
-developed to evaluate detected clusters and return the cluster labels that have
-most optimal **clustering tendency**, **Number of clusters** and **clustering
-quality**. Multiple evaluation strategies are implemented for the evaluation;
-**silhouette**, **dbindex**, and **derivative**, and four clustering methods
-can be used: **agglomerative**, **kmeans**, **dbscan** and **hdbscan**. #
-**â­ï¸ Star this repo if you like it â­ï¸** # ### Blogs Read the blog to
-get a structured overview how you can use ``clusteval``. * [Medium Blog: A
-step-by-step guide for clustering images](https://towardsdatascience.com/a-
-step-by-step-guide-for-clustering-images-4b45f9906128) In case you want to
-detect identical images, you can also use hash functionalities. * [Medium Blog:
-Detection of Duplicate Images Using Image Hash Functions](https://
-towardsdatascience.com/detection-of-duplicate-images-using-image-hash-
-functions-4d9c53f04a75) # ### [Documentation pages](https://erdogant.github.io/
-clusteval/) On the [documentation pages](https://erdogant.github.io/clusteval/
-) you can find detailed information about the working of the ``clusteval`` with
-many examples. # ### Installation ##### It is advisable to create a new
-environment (e.g. with Conda). ```bash conda create -n env_clusteval python=3.8
-conda activate clusteval ``` ##### Install from PyPI ```bash pip install
-clusteval ``` ##### Import library ```python from clusteval import clusteval
-```
+Metadata-Version: 2.1 Name: clusteval Version: 2.1.6 Summary: clusteval is a
+python package for unsupervised cluster validation. Home-page: https://
+erdogant.github.io/clusteval Download-URL: https://github.com/erdogant/
+clusteval/archive/2.1.6.tar.gz Author: Erdogan Taskesen Author-email:
+erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3 Description-Content-Type: text/markdown
+License-File: LICENSE # clusteval [![Python](https://img.shields.io/pypi/
+pyversions/clusteval)](https://img.shields.io/pypi/pyversions/clusteval) [!
+[PyPI Version](https://img.shields.io/pypi/v/clusteval)](https://pypi.org/
+project/clusteval/) [![License](https://img.shields.io/badge/license-MIT-
+green.svg)](https://github.com/erdogant/clusteval/blob/master/LICENSE) [!
+[BuyMeCoffee](https://img.shields.io/badge/buymea-coffee-yellow.svg)](https://
+www.buymeacoffee.com/erdogant) [![Github Forks](https://img.shields.io/github/
+forks/erdogant/clusteval.svg)](https://github.com/erdogant/clusteval/network)
+[![GitHub Open Issues](https://img.shields.io/github/issues/erdogant/
+clusteval.svg)](https://github.com/erdogant/clusteval/issues) [![Project
+Status](http://www.repostatus.org/badges/latest/active.svg)](http://
+www.repostatus.org/#active) [![Downloads](https://pepy.tech/badge/clusteval/
+month)](https://pepy.tech/project/clusteval) [![Downloads](https://pepy.tech/
+badge/clusteval)](https://pepy.tech/project/clusteval) [![DOI](https://
+zenodo.org/badge/232915924.svg)](https://zenodo.org/badge/latestdoi/232915924)
+[![Sphinx](https://img.shields.io/badge/Sphinx-Docs-Green)](https://
+erdogant.github.io/clusteval/) [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://erdogant.github.io/
+clusteval/pages/html/Documentation.html#colab-notebook)  ``clusteval`` is a
+python package that is developed to evaluate detected clusters and return the
+cluster labels that have most optimal **clustering tendency**, **Number of
+clusters** and **clustering quality**. Multiple evaluation strategies are
+implemented for the evaluation; **silhouette**, **dbindex**, and
+**derivative**, and four clustering methods can be used: **agglomerative**,
+**kmeans**, **dbscan** and **hdbscan**. # **â­ï¸ Star this repo if you like
+it â­ï¸** # ### Blogs Read the blog to get a structured overview how you can
+use ``clusteval``. * [Medium Blog: A step-by-step guide for clustering images]
+(https://towardsdatascience.com/a-step-by-step-guide-for-clustering-images-
+4b45f9906128) In case you want to detect identical images, you can also use
+hash functionalities. * [Medium Blog: Detection of Duplicate Images Using Image
+Hash Functions](https://towardsdatascience.com/detection-of-duplicate-images-
+using-image-hash-functions-4d9c53f04a75) # ### [Documentation pages](https://
+erdogant.github.io/clusteval/) On the [documentation pages](https://
+erdogant.github.io/clusteval/) you can find detailed information about the
+working of the ``clusteval`` with many examples. # ### Installation ##### It is
+advisable to create a new environment (e.g. with Conda). ```bash conda create -
+n env_clusteval python=3.8 conda activate clusteval ``` ##### Install from PyPI
+```bash pip install clusteval ``` ##### Import library ```python from clusteval
+import clusteval ```
 ===============================================================================
 ### Examples A structured overview of all examples are now available on the
 [documentation pages](https://erdogant.github.io/clusteval/).
 ===============================================================================
 * [Example: Cluster validation using Silhouette score](https://
 erdogant.github.io/clusteval/pages/html/Examples.html#cluster-evaluation)
 [https://github.com/erdogant/clusteval/blob/master/docs/figs/fig1b_sil.png]
```

### Comparing `clusteval-2.1.5/clusteval.egg-info/SOURCES.txt` & `clusteval-2.1.6/clusteval.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 clusteval/dbscan.py
 clusteval/derivative.py
 clusteval/examples.py
 clusteval/hdbscan.py
 clusteval/image2vec.py
 clusteval/plot_dendrogram.py
 clusteval/silhouette.py
+clusteval/utils.py
 clusteval.egg-info/PKG-INFO
 clusteval.egg-info/SOURCES.txt
 clusteval.egg-info/dependency_links.txt
 clusteval.egg-info/requires.txt
 clusteval.egg-info/top_level.txt
 clusteval/tests/__init__.py
 clusteval/tests/test_clusteval.py
```

### Comparing `clusteval-2.1.5/setup.py` & `clusteval-2.1.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 # Setup ------------
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
-     install_requires=['pypickle','matplotlib','numpy','pandas','tqdm','seaborn','scikit-learn','wget'],
+     install_requires=['scatterd', 'pypickle','matplotlib','numpy','pandas','tqdm','seaborn','scikit-learn', 'colourmap'],
      python_requires='>=3',
      name='clusteval',
      version=new_version,
      author="Erdogan Taskesen",
      author_email="erdogant@gmail.com",
-     description="clusteval is a python package that provides various methods for unsupervised cluster validation.",
+     description="clusteval is a python package for unsupervised cluster validation.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://erdogant.github.io/clusteval",
      download_url = 'https://github.com/erdogant/clusteval/archive/'+new_version+'.tar.gz',
      packages=setuptools.find_packages(), # Searches throughout all dirs for files to include
      include_package_data=True, # Must be true to include files depicted in MANIFEST.in
      license_files=["LICENSE"],
```

