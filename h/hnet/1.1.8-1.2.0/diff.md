# Comparing `tmp/hnet-1.1.8.tar.gz` & `tmp/hnet-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnet-1.1.8.tar", last modified: Wed May 19 09:50:13 2021, max compression
+gzip compressed data, was "hnet-1.2.0.tar", last modified: Sun Apr 16 12:35:57 2023, max compression
```

## Comparing `hnet-1.1.8.tar` & `hnet-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2021-05-19 09:50:13.029824 hnet-1.1.8/
--rw-rw-rw-   0        0        0      135 2020-11-19 13:38:07.000000 hnet-1.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0    10553 2021-05-19 09:50:13.029824 hnet-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     8392 2021-01-04 15:42:29.000000 hnet-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2021-05-19 09:50:13.012867 hnet-1.1.8/hnet/
--rw-rw-rw-   0        0        0     1806 2021-05-19 09:34:04.000000 hnet-1.1.8/hnet/__init__.py
--rw-rw-rw-   0        0        0     3510 2020-11-19 13:38:07.000000 hnet-1.1.8/hnet/adjmat_vec.py
--rw-rw-rw-   0        0        0    11663 2021-05-08 12:33:34.000000 hnet-1.1.8/hnet/examples.py
-drwxrwxrwx   0        0        0        0 2021-05-19 09:50:13.027826 hnet-1.1.8/hnet/gui/
--rw-rw-rw-   0        0        0        0 2020-11-19 13:38:07.000000 hnet-1.1.8/hnet/gui/__init__.py
--rw-rw-rw-   0        0        0    31911 2020-11-19 13:38:07.000000 hnet-1.1.8/hnet/gui/hnet_gui.py
--rw-rw-rw-   0        0        0    59424 2021-05-19 09:37:14.000000 hnet-1.1.8/hnet/hnet.py
--rw-rw-rw-   0        0        0    26473 2021-04-09 10:44:48.000000 hnet-1.1.8/hnet/hnstats.py
--rw-rw-rw-   0        0        0    18002 2021-05-19 09:44:19.000000 hnet-1.1.8/hnet/network.py
--rw-rw-rw-   0        0        0     1413 2021-05-19 09:47:36.000000 hnet-1.1.8/hnet/savefig.py
-drwxrwxrwx   0        0        0        0 2021-05-19 09:50:13.026831 hnet-1.1.8/hnet.egg-info/
--rw-rw-rw-   0        0        0    10553 2021-05-19 09:50:12.000000 hnet-1.1.8/hnet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      325 2021-05-19 09:50:12.000000 hnet-1.1.8/hnet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-05-19 09:50:12.000000 hnet-1.1.8/hnet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      159 2021-05-19 09:50:12.000000 hnet-1.1.8/hnet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2021-05-19 09:50:12.000000 hnet-1.1.8/hnet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-05-19 09:50:13.029824 hnet-1.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1478 2021-01-04 17:08:32.000000 hnet-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:35:57.740342 hnet-1.2.0/
+-rw-rw-rw-   0        0        0    11557 2020-11-19 13:38:07.000000 hnet-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      135 2020-11-19 13:38:07.000000 hnet-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9555 2023-04-16 12:35:57.739543 hnet-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9038 2022-09-17 20:51:55.000000 hnet-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 12:35:57.631164 hnet-1.2.0/hnet/
+-rw-rw-rw-   0        0        0     1993 2023-04-16 12:24:59.000000 hnet-1.2.0/hnet/__init__.py
+-rw-rw-rw-   0        0        0     3510 2020-11-19 13:38:07.000000 hnet-1.2.0/hnet/adjmat_vec.py
+-rw-rw-rw-   0        0        0    12158 2023-04-16 12:24:30.000000 hnet-1.2.0/hnet/examples.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:35:57.736766 hnet-1.2.0/hnet/gui/
+-rw-rw-rw-   0        0        0        0 2020-11-19 13:38:07.000000 hnet-1.2.0/hnet/gui/__init__.py
+-rw-rw-rw-   0        0        0    31911 2020-11-19 13:38:07.000000 hnet-1.2.0/hnet/gui/hnet_gui.py
+-rw-rw-rw-   0        0        0    61970 2023-04-16 12:23:14.000000 hnet-1.2.0/hnet/hnet.py
+-rw-rw-rw-   0        0        0    26476 2022-03-18 08:21:26.000000 hnet-1.2.0/hnet/hnstats.py
+-rw-rw-rw-   0        0        0    17829 2021-05-23 17:59:59.000000 hnet-1.2.0/hnet/network.py
+-rw-rw-rw-   0        0        0     1413 2021-05-19 09:47:36.000000 hnet-1.2.0/hnet/savefig.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:35:57.721678 hnet-1.2.0/hnet.egg-info/
+-rw-rw-rw-   0        0        0     9555 2023-04-16 12:35:57.000000 hnet-1.2.0/hnet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-04-16 12:35:57.000000 hnet-1.2.0/hnet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 12:35:57.000000 hnet-1.2.0/hnet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      150 2023-04-16 12:35:57.000000 hnet-1.2.0/hnet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-16 12:35:57.000000 hnet-1.2.0/hnet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 12:35:57.740342 hnet-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1500 2023-04-16 11:37:26.000000 hnet-1.2.0/setup.py
```

### Comparing `hnet-1.1.8/hnet/__init__.py` & `hnet-1.2.0/hnet/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from hnet.adjmat_vec import (
     vec2adjmat,
     adjmat2vec,
     )
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.1.8'
+__version__ = '1.2.0'
 
 # module level doc-string
 __doc__ = """
 HNET - Graphical Hypergeometric networks.
 =====================================================================
 
 Description
@@ -34,30 +34,35 @@
 >>> from hnet import hnet
 >>> hn = hnet()
 >>> # Load example dataset
 >>> df = hn.import_example('titanic')
 
 >>> # Structure learning
 >>> out = hn.association_learning(df)
-
+>>>
 >>> # Plot dynamic graphs
 >>> G = hn.d3graph()
 >>> G = hn.d3heatmap()
+>>>
 >>> # Plot static graph
 >>> G = hn.plot()
+>>>
 >>> # Plot heatmap
 >>> hn.heatmap(cluster=True)
+>>>
 >>> # Plot feature importance
 >>> hn.plot_feat_importance()
-
+>>>
 >>> # Examine differences between models
 >>> import hnet
 >>> scores, adjmat = hnet.compare_networks(out['simmatP'], out['simmatP'], showfig=True)
 >>> adjmat_undirected = hnet.to_undirected(out['simmatLogP'])
+>>>
 
 References
 ----------
-* https://erdogant.github.io/hnet/
-* https://github.com/erdogant/hnet
-* https://arxiv.org/abs/2005.04679
+* Blog: https://towardsdatascience.com/explore-and-understand-your-data-with-a-network-of-significant-associations-9a03cf79d254
+* Github: https://github.com/erdogant/hnet
+* Documentation: https://erdogant.github.io/hnet/
+* Article: https://arxiv.org/abs/2005.04679
 
 """
```

### Comparing `hnet-1.1.8/hnet/adjmat_vec.py` & `hnet-1.2.0/hnet/adjmat_vec.py`

 * *Files identical despite different names*

### Comparing `hnet-1.1.8/hnet/examples.py` & `hnet-1.2.0/hnet/examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,54 +3,67 @@
 # print(hnet.__version__)
 
 # %%
 import numpy as np
 import pandas as pd
 
 
+# %% Titanic case
+from hnet import hnet
+hn = hnet()
+df = hn.import_example('titanic')
+
+del df['PassengerId']
+del df['Name']
+results_new = hn.association_learning(df, verbose=4)
+
+# STATIC
+hn.heatmap(summarize=False, cluster=False)
+hn.plot(node_color='cluster')
+
+# Feature importance
+hn.plot_feat_importance(marker_size=50)
+
+hn.d3heatmap(savepath='c:/temp/titanic_summarize/heatmap.html')
+hn.d3graph(savepath='c:/temp/titanic_summarize_d3graph/d3graph.html', node_color='cluster')
+
+hn.d3heatmap()
+hn.d3graph()
+
+# %%
+from hnet import hnet
+hn = hnet()
+df = hn.import_example('grocery')
+results = hn.association_learning(df)
+hn.d3graph(summarize=True)
+hn.d3heatmap(summarize=True)
+
 # %%
 from hnet import hnet
 hn = hnet()
 df = hn.import_example('sprinkler')
 
 hn1 = hnet(excl_background='0.0', dtypes=np.array(['bool']*df.shape[1]))
 out1 = hn1.association_learning(df.astype(bool))
+hn1.d3graph()
 
 hn2 = hnet()
 out2 = hn2.association_learning(df.astype(bool))
-
-hn2.d3graph(summarize=True)
+# hn2.d3graph(summarize=True)
 hn2.d3graph()
 
 hn2.d3heatmap(summarize=True)
 hn2.d3heatmap(summarize=False)
 
 hn2.heatmap(summarize=True, cluster=False)
 hn2.heatmap(cluster=True)
 
 
 
 
-# %% Titanic case
-from hnet import hnet
-hn = hnet()
-df = hn.import_example('titanic')
-del df['PassengerId']
-del df['Name']
-results_new = hn.association_learning(df, verbose=4)
-
-# STATIC
-hn.heatmap(summarize=False, cluster=False)
-hn.plot(node_color='cluster')
-
-# Feature importance
-hn.plot_feat_importance(marker_size=50)
-
-hn.d3heatmap('c:/temp/titanic_summarize/')
-hn.d3graph('c:/temp/titanic_summarize_d3graph/')
 
 
 # %% Penguins dataset
 import seaborn as sns
 from hnet import hnet
 
 df = sns.load_dataset("penguins")
@@ -140,15 +153,15 @@
 results = hn.association_learning(df)
 
 # out = tabulate(hn.results['rules'].iloc[1:,:].head(), tablefmt="grid", headers="keys")
 
 hn.d3heatmap(figsize=(1000,1000))
 hn.d3graph(node_color='cluster')
 hn.d3graph(min_edges=5)
-# hn.d3graph(savepath='D://PY/REPOSITORIES/erdogant.github.io/docs/d3graph/income/')
+# hn.d3graph(savepath='D://PY/REPOSITORIES/erdogant.github.io/docs/d3graph/income/income.html')
 
 
 # %% Import examples
 import hnet
 
 df = hnet.import_example('titanic')
 
@@ -295,25 +308,25 @@
 out = tabulate(hn.results['rules'].iloc[1:,:].head(), tablefmt="grid", headers="keys")
 print(tabulate(df.head(), tablefmt="grid", headers="keys"))
 
 # %% Small retail
 df = hn.import_example('retail')
 hn1 = hnet()
 results1 = hn1.association_learning(df)
-hn1.d3graph(savepath='D://PY/REPOSITORIES/erdogant.github.io/docs/d3graph/marketing_data_online_retail_small/')
+hn1.d3graph(savepath='D://PY/REPOSITORIES/erdogant.github.io/docs/d3graph/marketing_data_online_retail_small/d3graph.html')
 # hn1.plot()
 # hn1.d3graph()
 # hn1.heatmap()
 
 # %%
 
 df = hn.import_example('waterpump')
 hn2 = hnet(black_list=['id','longitude','latitude'])
 results2 = hn2.association_learning(df)
-hn2.d3graph(savepath='D://PY/REPOSITORIES/erdogant.github.io/docs/d3graph/waterpump/')
+hn2.d3graph(savepath='D://PY/REPOSITORIES/erdogant.github.io/docs/d3graph/waterpump/d3graph.html')
 # hn2.plot()
 # hn2.d3graph()
 # hn2.heatmap()
 
 # df['id'].head().values
 
 # %%
@@ -325,15 +338,15 @@
        'num', 'num', 'num', 'num',
        'num', 'cat', 'cat',
        'cat', 'cat', 'cat', 'cat', 'cat', 'cat',
        'cat', 'cat', 'num'])
 
 results3 = hn3.association_learning(df)
 hn3.d3graph()
-# hn3.d3graph(savepath='D://PY/REPOSITORIES/erdogant.github.io/docs/d3graph/fifa_2018/')
+# hn3.d3graph(savepath='D://PY/REPOSITORIES/erdogant.github.io/docs/d3graph/fifa_2018/d3graph.html')
 # hn3.plot()
 # hn3.heatmap()
 
 out = tabulate(hn3.results['rules'].iloc[1:,:].head(), tablefmt="grid", headers="keys")
 print(tabulate(df.head(), tablefmt="grid", headers="keys"))
 
 # hn3.plot()
@@ -355,42 +368,42 @@
 
 from hnet import hnet
 hn = hnet(black_list=['fnlwgt'])
 results = hn.association_learning(df)
 
 out = tabulate(hn.results['rules'].iloc[1:,:].head(), tablefmt="grid", headers="keys")
 
-hn.d3graph(savepath='D://PY/REPOSITORIES/erdogant.github.io/docs/d3graph/income/')
+hn.d3graph(savepath='D://PY/REPOSITORIES/erdogant.github.io/docs/d3graph/income/d3graph.html')
 hn.d3graph(min_edges=1)
 
 # %% Covid-19 dataset
 from hnet import hnet
 import pandas as pd
 df = pd.read_csv('D://covid19_us_county.zip')
 
 dtypes = ['', 'cat', 'cat', 'num', 'num', 'num', 'num', 'num', 'num', 'num', 'num', 'num', 'num', 'num', 'num', 'num']
 hn = hnet(dtypes=dtypes)
 results = hn.association_learning(df)
 
 # %% Police shooting
-# https://github.com/washingtonpost/data-police-shootings
+# https://github.com/washingtonpost/data-police-shootings/blob/master/fatal-police-shootings-data.csv
 import pandas as pd
 from hnet import hnet
 import time
 
 hn = hnet(excl_background=['nan'], black_list=['id', 'date', 'name'])
 
 # Load results
 results = hn.load(filepath='C://temp//data-police-shootings/hnet.pkl')
 
 # Run hnet
 if results is None:
 
     # Read csv
-    df = pd.read_csv('C://temp/police_shooting.csv')
+    df = pd.read_csv('C://temp/data-police-shootings/fatal-police-shootings-data.csv')
     df['month'] = pd.to_datetime(df['date']).dt.month_name()
     df.head()
     # Initialize
     hn = hnet(excl_background=['nan'], black_list=['id', 'date', 'name'])
 
     start = time.time()
     # Association learning
@@ -406,14 +419,15 @@
     # Save
     hn.save(filepath='C://temp/New folder/data-police-shootings/hnet.pkl', overwrite=True)
 
 # Plot dynamic graph
 hn.d3graph()
 hn.d3graph(black_list=['city'])
 hn.d3graph(black_list=['city', 'state'])
+hn.d3graph(black_list=['city', 'state', 'longitude', 'latitude'])
 hn.d3graph(summarize=True)
 
 # Plot heatmap
 hn.d3heatmap(black_list=['city', 'state'])
 hn.d3heatmap(black_list=['city', 'state', 'longitude', 'latitude'])
 hn.d3heatmap(summarize=True, vmax=5)
```

### Comparing `hnet-1.1.8/hnet/gui/hnet_gui.py` & `hnet-1.2.0/hnet/gui/hnet_gui.py`

 * *Files identical despite different names*

### Comparing `hnet-1.1.8/hnet/hnet.py` & `hnet-1.2.0/hnet/hnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,47 +4,35 @@
 # Author      : E.Taskesen
 # Contact     : erdogant@gmail.com
 # github      : https://github.com/erdogant/hnet
 # Licence     : See licences
 # -------------------------------------------------
 
 # %% Libraries
+import matplotlib.pyplot as plt
+import requests
+from tqdm import tqdm
+import numpy as np
+import pandas as pd
+import os
+import networkx as nx
+from sklearn.preprocessing import MinMaxScaler, LabelEncoder
+from scipy.stats import combine_pvalues
+import hnet.hnstats as hnstats
+import hnet.network as network
+from hnet.savefig import savefig
+import pypickle
+import colourmap
+import df2onehot
+import imagesc
+from ismember import ismember
 import warnings
 warnings.filterwarnings("ignore")
-
-# Custom packages
-from d3graph import d3graph as d3graphs
-from d3heatmap import d3heatmap as d3
-from ismember import ismember
-import imagesc
-import df2onehot
-import colourmap
-
-# Local utils
-import pypickle
-from hnet.savefig import savefig
-import hnet.network as network
-import hnet.hnstats as hnstats
-
-# Known libraries
-from scipy.stats import combine_pvalues
-from sklearn.preprocessing import MinMaxScaler, LabelEncoder
 label_encoder = LabelEncoder()
 
-import networkx as nx
-
-# Internal
-import wget
-import os
-import pandas as pd
-import numpy as np
-from tqdm import tqdm
-import matplotlib.pyplot as plt
-
-# from functools import lru_cache
 
 # %% Association learning across all variables
 class hnet():
     """HNET - Graphical Hypergeometric networks.
 
     Description
     -----------
@@ -54,15 +42,15 @@
         1. Pre-processing: Typing and One-hot Enconding. Each feature is set as being categoric, numeric or is excluded. The typing can be user-defined or automatically determined on conditions. Encoding of features in a one-hot dense array is done for the categoric terms. The one-hot dense array is subsequently used to create combinatory features using k combinations over n features (without replacement).
         2. Combinations: Make smart combinations between features because many mutual exclusive classes do exists.
         3. Hypergeometric test: The final dense array is used to assess significance with the categoric features.
         4. Wilcoxon Ranksum: To assess significance across the numeric features (Xnumeric) in relation to the dense array (Xcombination), the Mann-Whitney-U test is performed.
         5. Multiple test correction: Declaring significance for node-links.
 
     The final output of HNet is an adjacency matrix containing edge weights that depicts the strength of pairs of vertices.
-    The adjacency matrix can then be examined as a network representation using d3graph.
+    The adjacency matrix can then be examined as a network representation using D3blocks.
 
     Parameters
     ----------
     alpha : float [0..1], (default : 0.05)
         Significance to keep only edges with <=alhpa.
         1 : (for all results)
     y_min : int [1..n], where n is the number of samples. (default : 10)
@@ -129,14 +117,22 @@
     >>> G_dynamic = hn.d3graph()
     >>> # Plot static graph
     >>> G_static = hn.plot()
     >>> # Plot heatmap
     >>> P_heatmap = hn.heatmap(cluster=True)
     >>> # Plot feature importance
     >>> hn.plot_feat_importance()
+
+    References
+    ----------
+    * Blog: https://towardsdatascience.com/explore-and-understand-your-data-with-a-network-of-significant-associations-9a03cf79d254
+    * Github: https://github.com/erdogant/hnet
+    * Documentation: https://erdogant.github.io/hnet/
+    * Article: https://arxiv.org/abs/2005.04679
+
     """
 
     def __init__(self, alpha=0.05, y_min=10, perc_min_num=0.8, k=1, multtest='holm', dtypes='pandas', specificity='medium', dropna=True, excl_background=None, black_list=None, white_list=None):
         """Initialize distfit with user-defined parameters."""
         if (alpha is None): alpha=1
         if (y_min is None): y_min=1
         if isinstance(white_list, str): white_list=[white_list]
@@ -274,15 +270,15 @@
 
         # Store in dataframe
         adjmatP = pd.DataFrame(data=adjmatP, index=uilabx, columns=uilabx)
         adjmatlogP = -np.log10(adjmatP)
         adjmatlogP[adjmatlogP<=0]=0
         # Replace inf values with maximum value that is possible
         # adjmatlogP[np.isinf(adjmatlogP)]=323
-        for (columnName, columnData) in adjmatlogP.iteritems():
+        for (columnName, columnData) in adjmatlogP.items():
             columnData.loc[~(columnData!= np.inf)] = columnData.loc[columnData!= np.inf].max()
         return adjmatP, adjmatlogP
 
     def _feat_importance(self, simmatLogP, labx, verbose=3):
         """Compute feature importance."""
         # Get unique labels
         uilabx, counts = np.unique(labx, return_counts=True)
@@ -414,14 +410,15 @@
         savepath : str
             Save the figure in specified path.
         labx : array-like
             Cluster labels.
 
         """
         if verbose>=3: print('[hnet] >Building dynamic heatmaps using d3graph..')
+        if savepath is None: savepath=''
         # Check results
         status = self._check_results()
         if not status: return None
         # Retrieve data
         _, simmatLogP, labx = self._get_adjmat(summarize)
 
         # Filter adjacency matrix on blacklist/whitelist and/or threshold
@@ -437,26 +434,29 @@
 
         # Cluster
         labx = self.plot(summarize=summarize, node_color='cluster', directed=True, threshold=threshold, white_list=white_list, black_list=black_list, min_edges=min_edges, showfig=False)['labx']
 
         if vmax is None:
             vmax = np.max(np.max(simmatLogP)) / 10
 
+        # Initialize
+        if not _check_import_d3blocks(): return None
+        from d3blocks import D3Blocks
+        d3 = D3Blocks()
         # Make heatmap
-        if verbose>=3: print('[hnet] >Creating output html..')
-        paths = d3.heatmap(simmatLogP, clust=labx, path=savepath, title='Hnet d3heatmap', vmax=vmax, width=figsize[1], height=figsize[0], showfig=showfig, stroke='red', verbose=verbose)
+        d3.heatmap(simmatLogP, showfig=True, title='Hnet D3blocks', filepath=savepath, figsize=figsize, stroke='red', vmax=vmax, classlabel='cluster')
 
         # Return
         results = {}
-        results['paths'] = paths
+        results['paths'] = d3.config['filepath']
         results['clust_labx'] = labx
-        return(results)
+        return results
 
     # Make network d3
-    def d3graph(self, summarize=False, node_size_limits=[6, 15], savepath=None, node_color=None, directed=True, threshold=None, white_list=None, black_list=None, min_edges=None, charge=500, figsize=(1500, 1500), showfig=True, verbose=3):
+    def d3graph(self, summarize=False, node_size_limits=[6, 15], savepath=None, node_color=None, directed=True, threshold=None, white_list=None, black_list=None, min_edges=None, charge=500, figsize=(1500, 1500), showfig=True, elastic=False, verbose=3):
         """Interactive network creator.
 
         Description
         -----------
         This function creates a interactive and stand-alone network that is build on d3 javascript.
         d3graph is integrated into hnet and uses the -log10(P-value) adjacency matrix.
         Each column and index name represents a node whereas values >0 in the matrix represents an edge.
@@ -525,24 +525,50 @@
 
         # Make undirected network
         if not directed:
             simmatLogP = to_undirected(simmatLogP, method='logp')
 
         # Color node using network-clustering
         if node_color=='cluster':
-            labx = self.plot(summarize=summarize, node_color='cluster', directed=True, threshold=threshold, white_list=white_list, black_list=black_list, min_edges=min_edges, showfig=False)['labx']
+            # labx = self.plot(summarize=summarize, node_color='cluster', directed=True, threshold=threshold, white_list=white_list, black_list=black_list, min_edges=min_edges, showfig=False)['labx']
+            labx='cluster'
         else:
             labx = label_encoder.fit_transform(labx)
+        
+        if not _check_import_d3blocks(): return None
+        from d3blocks import D3Blocks
+        d3 = D3Blocks()
+        if verbose>=3: print('[hnet] >Creating d3graph..')
+        # Initialize
+        d3 = D3Blocks()
+        df_vector = d3.adjmat2vec(simmatLogP.T)
+        # Create network using default 
+        d3.d3graph(df_vector,
+                   color=labx,
+                   size=node_size,
+                   title='D3graph - D3blocks',
+                   filepath=savepath,
+                   figsize=figsize,
+                   overwrite=True,
+                   collision=0.1,
+                   charge=charge,
+                   slider=[None, None],
+                   scaler='zscore',
+                   showfig=False,
+                   )
+
+        # Change node properties
+        # d3.D3graph.set_node_properties(color=None, size=node_size)
+        # Change edge properties
+        d3.D3graph.set_edge_properties(directed=directed, marker_end='arrow')
+        # Show
+        d3.D3graph.show(showfig=showfig)
 
-        # Make network
-        if verbose>=3: print('[hnet] >Creating output html..')
-        Gout = d3graphs(simmatLogP.T, savepath=savepath, node_size=node_size, charge=charge, height=figsize[0], width=figsize[1], collision=0.1, node_color=labx, directed=directed, showfig=showfig)
         # Return
-        Gout['labx'] = labx
-        return(Gout)
+        return {'G': d3.D3graph.G, 'savepath': d3.D3graph.config['filepath'], 'labx': labx}
 
     # Make network plot
     def plot(self, summarize=False, scale=2, dist_between_nodes=0.4, node_size_limits=[25, 500], directed=True, node_color=None, savepath=None, figsize=[15, 10], pos=None, layout='fruchterman_reingold', dpi=250, threshold=None, white_list=None, black_list=None, min_edges=None, showfig=True, verbose=3):
         """Make plot static network plot of the model results.
 
         Description
         -----------
@@ -624,15 +650,15 @@
         if adjmatLog.values.flatten().sum()==0:
             if verbose>=3: print('[hnet] >Nothing to plot.')
             return None
 
         # Set weights for edges
         adjmatLogWEIGHT = adjmatLog.copy()
         np.fill_diagonal(adjmatLogWEIGHT.values, 0)
-        adjmatLogWEIGHT = pd.DataFrame(index=adjmatLog.index.values, data=MinMaxScaler(feature_range=(0, 20)).fit_transform(adjmatLogWEIGHT), columns=adjmatLog.columns)
+        adjmatLogWEIGHT = pd.DataFrame(index=adjmatLog.index.values.astype(str), data=MinMaxScaler(feature_range=(0, 20)).fit_transform(adjmatLogWEIGHT.values), columns=adjmatLog.columns.astype(str))
 
         # Set size for node
         IA, IB = ismember(adjmatLog.columns, self.results['counts'][:, 0])
         node_size = np.repeat(node_size_limits[0], len(adjmatLog.columns))
         node_size[IA] = hnstats._scale_weights(self.results['counts'][IB, 1], node_size_limits)
 
         # Make new graph (G) and add properties to nodes
@@ -815,15 +841,15 @@
         Examples
         --------
         >>> from hnet import hnet
         >>> hn = hnet()
         >>> df = hn.import_example('sprinkler')
         >>> hn.association_learning(df)
         >>> hn.combined_rules()
-        >>> print(hn.rules)
+        >>> print(hn.results['rules'])
 
         """
         if simmatP is None:
             if self.results.get('simmatP', None) is None: raise ValueError('[hnet] >Error: Input requires the result from the association_learning() function.')
             simmatP = self.results['simmatP']
         if labx is None:
             labx = self.results['labx']
@@ -855,15 +881,15 @@
         Description
         -----------
         Import one of the few datasets from github source or specify your own download url link.
 
         Parameters
         ----------
         data : str
-            Name of datasets: 'sprinkler', 'titanic', 'student', 'fifa', 'cancer', 'waterpump', 'retail'
+            Name of datasets: 'sprinkler', 'grocery', 'titanic', 'student', 'fifa', 'cancer', 'waterpump'
         url : str
             url link to to dataset.
         verbose : int, (default: 3)
             Print message to screen.
 
         Returns
         -------
@@ -971,90 +997,30 @@
     def _clean(self, verbose=3):
         # Clean readily fitted models to ensure correct results.
         if hasattr(self, 'results'):
             if verbose>=3: print('[hnet] >Cleaning previous fitted model results..')
             if hasattr(self, 'results'): del self.results
 
 # %% Store results
+
+
 def _store(simmatP, adjmatLog, GsimmatP, GsimmatLogP, labx, df, nr_succes_pop_n, dtypes, rules, feat_importance):
     out = {}
     out['simmatP'] = simmatP
     out['simmatLogP'] = adjmatLog
     out['simmatP_cat'] = GsimmatP
     out['simmatLogP_cat'] = GsimmatLogP
     out['labx'] = labx.astype(str)
     out['dtypes'] = np.array(list(zip(df.columns.values.astype(str), dtypes)))
     out['counts'] = nr_succes_pop_n
     out['rules'] = rules
     out['feat_importance'] = feat_importance
     return out
 
 
-# %% Import example dataset from github.
-def import_example(data='titanic', url=None, sep=',', verbose=3):
-    """Import example dataset from github source.
-
-    Description
-    -----------
-    Import one of the few datasets from github source or specify your own download url link.
-
-    Parameters
-    ----------
-    data : str
-        Name of datasets: 'sprinkler', 'titanic', 'student', 'fifa', 'cancer', 'waterpump', 'retail'
-    url : str
-        url link to to dataset.
-    verbose : int, (default: 3)
-        Print message to screen.
-
-    Returns
-    -------
-    pd.DataFrame()
-        Dataset containing mixed features.
-
-    """
-    if url is None:
-        if data=='sprinkler':
-            url='https://erdogant.github.io/datasets/sprinkler.zip'
-        elif data=='titanic':
-            url='https://erdogant.github.io/datasets/titanic_train.zip'
-        elif data=='student':
-            url='https://erdogant.github.io/datasets/student_train.zip'
-        elif data=='cancer':
-            url='https://erdogant.github.io/datasets/cancer_dataset.zip'
-        elif data=='fifa':
-            url='https://erdogant.github.io/datasets/FIFA_2018.zip'
-        elif data=='waterpump':
-            url='https://erdogant.github.io/datasets/waterpump/waterpump_test.zip'
-        elif data=='retail':
-            url='https://erdogant.github.io/datasets/marketing_data_online_retail_small.zip'
-    else:
-        data = wget.filename_from_url(url)
-
-    if url is None:
-        if verbose>=3: print('[hnet] >Nothing to download.')
-        return None
-
-    curpath = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
-    PATH_TO_DATA = os.path.join(curpath, wget.filename_from_url(url))
-    if not os.path.isdir(curpath):
-        os.makedirs(curpath, exist_ok=True)
-
-    # Check file exists.
-    if not os.path.isfile(PATH_TO_DATA):
-        if verbose>=3: print('[hnet] >Downloading [%s] dataset from github source..' %(data))
-        wget.download(url, curpath)
-
-    # Import local dataset
-    if verbose>=3: print('[hnet] >Import dataset [%s]' %(data))
-    df = pd.read_csv(PATH_TO_DATA, sep=sep)
-    # Return
-    return df
-
-
 # %% Compute fit
 def enrichment(df, y, y_min=None, alpha=0.05, multtest='holm', dtypes='pandas', specificity='medium', excl_background=None, verbose=3):
     """Enrichment analysis.
 
     Description
     -----------
     Compute enrichment between input dataset and response variable y. Length of dataframe and y must be equal.
@@ -1110,18 +1076,18 @@
     zscore : float
         Z-score of the Wilcoxon Ranksum test.
     nr_not_succes_pop_n : int
         Number of successes in population.
 
     Examples
     --------
-    >>> import hnet
+    >>> import hnet as hn
     >>> df = hn.import_example('titanic')
     >>> y = df['Survived'].values
-    >>> out = hnet.enrichment(df, y)
+    >>> out = hn.enrichment(df, y)
 
     """
     assert isinstance(df, pd.DataFrame), 'Data must be of type pd.DataFrame()'
     assert len(y)==df.shape[0], 'Length of [df] and [y] must be equal'
     assert 'numpy' in str(type(y)), 'y must be of type numpy array'
 
     # DECLARATIONS
@@ -1299,9 +1265,131 @@
             out = [colname, X_comb.iloc[:, i].sum() / X_comb.shape[0]]
             # showprogress
             if verbose>=4: print('[%g]' %(len(IB)), end='')
     else:
         if verbose>=4: print('[hnet] >Skipping [%s] because length of unique values=1' %(X_comb.columns[i]), end='')
 
     if verbose>=4: print('')
+
     # Return
-    return(out, simmatP, simmat_labx)
+    return out, simmatP, simmat_labx
+
+
+# %% Import example dataset from github.
+def import_example(data='titanic', url=None, sep=',', verbose=3):
+    """Import example dataset from github source.
+
+    Description
+    -----------
+    Import one of the few datasets from github source or specify your own download url link.
+
+    Parameters
+    ----------
+    data : str
+        * 'sprinkler'
+        * 'titanic'
+        * 'student'
+        * 'fifa'
+        * 'cancer'
+        * 'waterpump'
+        * 'retail'
+        * 'grocery'
+    url : str
+        url link to to dataset.
+
+    Returns
+    -------
+    pd.DataFrame()
+        Dataset containing mixed features.
+
+    """
+    from urllib.parse import urlparse
+
+    if url is None:
+        if data=='sprinkler':
+            url='https://erdogant.github.io/datasets/sprinkler.zip'
+        elif data=='titanic':
+            url='https://erdogant.github.io/datasets/titanic_train.zip'
+        elif data=='student':
+            url='https://erdogant.github.io/datasets/student_train.zip'
+        elif data=='cancer':
+            url='https://erdogant.github.io/datasets/cancer_dataset.zip'
+        elif data=='fifa':
+            url='https://erdogant.github.io/datasets/FIFA_2018.zip'
+        elif data=='waterpump':
+            url='https://erdogant.github.io/datasets/waterpump/waterpump_test.zip'
+        elif data=='retail':
+            url='https://erdogant.github.io/datasets/marketing_data_online_retail_small.zip'
+            sep=';'
+        elif data=='grocery':
+            url='https://erdogant.github.io/datasets/grocery_products_purchase.zip'
+            sep=';'
+    else:
+        data = wget.filename_from_url(url)
+
+    if url is None:
+        if verbose>=3: print('Nothing to download.')
+        return None
+
+    curpath = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
+    filename = os.path.basename(urlparse(url).path)
+    PATH_TO_DATA = os.path.join(curpath, filename)
+    if not os.path.isdir(curpath):
+        os.makedirs(curpath, exist_ok=True)
+
+    # Check file exists.
+    if not os.path.isfile(PATH_TO_DATA):
+        if verbose>=3: print('Downloading [%s] dataset from github source..' %(data))
+        wget.download(url, PATH_TO_DATA)
+
+    # Import local dataset
+    if verbose>=3: print('Import dataset [%s]' %(data))
+    df = pd.read_csv(PATH_TO_DATA, sep=sep)
+
+    # Transform data in case of grocery
+    if data=='grocery':
+        # Split the column by commas
+        df = df.iloc[:, 0].str.split(',', expand=True)
+        # Rename columns
+        df.columns = [f'Product {i+1}' for i in range(df.shape[1])]
+
+    # Return
+    return df
+
+
+# %% Retrieve files files.
+class wget:
+    """Retrieve file from url."""
+
+    def filename_from_url(url):
+        """Return filename."""
+        return os.path.basename(url)
+
+    def download(url, writepath):
+        """Download.
+
+        Parameters
+        ----------
+        url : str.
+            Internet source.
+        writepath : str.
+            Directory to write the file.
+
+        Returns
+        -------
+        None.
+
+        """
+        r = requests.get(url, stream=True)
+        with open(writepath, "wb") as fd:
+            for chunk in r.iter_content(chunk_size=1024):
+                fd.write(chunk)
+
+
+def _check_import_d3blocks(verbose=3):
+    try:
+        import d3blocks
+        status = True
+    except:
+        if verbose>=3: print('Error: The library [d3blocks] is not installed by default. Try: <pip install d3blocks>')
+        status = False
+    return status
```

### Comparing `hnet-1.1.8/hnet/hnstats.py` & `hnet-1.2.0/hnet/hnstats.py`

 * *Files 0% similar despite different names*

```diff
@@ -565,15 +565,15 @@
     df, dtypes = df2onehot.set_dtypes(df, dtypes=dtypes, deep_extract=False, perc_min_num=perc_min_num, num_if_decimal=True, verbose=0)
     dtypes = np.array(dtypes)
 
     # Make sure its limited to the number of y_min
     Iloc = (df_onehot['onehot'].sum(axis=0)>=y_min).values
     if np.any(Iloc==False):
         if verbose>=2: print('[hnet] >WARNING: Features with y_min needs another round of filtering. Fixing it now..')
-        df_onehot['onehot']=df_onehot['onehot'].loc[:,Iloc]
+        df_onehot['onehot']=df_onehot['onehot'].loc[:, Iloc]
         df_onehot['labx']=df_onehot['labx'][Iloc]
 
     # Some check before proceeding
     if (df_onehot['onehot'].empty) or (np.all(np.isin(dtypes, 'num'))): raise ValueError('[hnet] >ALL data is excluded from the dataframe! There should be at least 1 categorical value!')
     if df.shape[1] != len(dtypes): raise ValueError('[hnet] >DataFrame Shape and dtypes length does not match.')
 
     # Make all integer
@@ -604,26 +604,26 @@
 
     # Filter on minimum number of edges
     if min_edges is not None:
         simmatBOOL = simmatLogP.copy()>0
         if np.all(simmatBOOL.columns==simmatBOOL.index.values):
             Iloc = np.logical_or(simmatBOOL.sum(axis=0)>=min_edges, simmatBOOL.sum(axis=1)>=min_edges).values
             if verbose>=3: print('[hnet] >Filtering on edges: [%d] variables remain after filtering on a minimum of [%d] edges.' %(np.sum(Iloc), min_edges))
-            simmatLogP = simmatLogP.loc[Iloc,Iloc]
+            simmatLogP = simmatLogP.loc[Iloc, Iloc]
             labx = labx[Iloc]
 
     # Filter on white_list
     if white_list is not None:
         Irow = np.isin(simmatLogP.index.values, white_list)
         Icol = np.isin(simmatLogP.columns, white_list)
         Ilabx = np.isin(labx, white_list)
         Irow = np.logical_or(Irow, Ilabx)
         Icol = np.logical_or(Icol, Ilabx)
         if verbose>=3: print('[hnet] >Number of variables at input: [%d], and after white listing: [%d]' %(len(Irow), sum(Irow)))
-        simmatLogP = simmatLogP.iloc[Irow,Icol]
+        simmatLogP = simmatLogP.iloc[Irow, Icol]
         labx = labx[Irow]
 
     # Filter on white_list
     if black_list is not None:
         Irow = np.isin(simmatLogP.index.values, black_list)
         Icol = np.isin(simmatLogP.columns, black_list)
         Ilabx = np.isin(labx, black_list)
```

### Comparing `hnet-1.1.8/hnet/network.py` & `hnet-1.2.0/hnet/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,19 +181,19 @@
     # compute labx for each of the centralities
     centralities=['betweenness', 'closeness','eigenvector','degree','edge','harmonic','katz','local','out_degree','percolation','second_order','subgraph','subgraph_exp','information']
     
     # Compute best positions for the network
     pos=nx.spring_layout(G)
 
     # Cluster data nd store label in G
-    [G, score] = cluster(G)
+    G, score = cluster(G)
     
     # Compute centrality score for each of the centralities and store in G
     for centrality in centralities:
-        [G,score]=compute_centrality(G, centrality=centrality)
+        G, score = compute_centrality(G, centrality=centrality)
     
     # Store
     df=pd.DataFrame([*G.nodes.values()])
     df.set_index(np.array([*G.nodes.keys()]), inplace=True)
     
     # Make plots
     for centrality in centralities:
@@ -213,36 +213,29 @@
     config['node_size_scale']=node_size_scale
     
     if verbose>=3: print('[hnet] >Error in network function: Creating network plot')
     
     if 'pandas' in str(type(node_size)):
         node_size=node_size.values
     
-    #scaling node sizes
+    # scaling node sizes
     if config['node_size_scale']!=None and 'numpy' in str(type(node_size)):
         if verbose>=3: print('[hnet] >Error in network function: Scaling node sizes')
         node_size=minmax_scale(node_size, feature_range=(node_size_scale[0], node_size_scale[1]))
 
-    # Node positions
-#    if isinstance(pos, type(None)):
-#        pos=nx.spring_layout(G)
-
-#    if isinstance(node_label, type(None)):
-#        node_label=[*G.nodes])
-
     fig=plt.figure(figsize=(config['width'], config['height']))
     
     # Make the graph
     if methodtype=='circular':
         nx.draw_circular(G, labels=node_label, node_size=node_size, alhpa=alpha, node_color=node_color, cmap=cmap, font_size=font_size, with_labels=True)
     elif methodtype=='kawai':
         nx.draw_kamada_kawai(G, labels=node_label, node_size=node_size, alhpa=alpha, node_color=node_color, cmap=cmap, font_size=font_size, with_labels=True)
     else:
         nx.draw_networkx(G, labels=node_label, pos=pos, node_size=node_size, alhpa=alpha, node_color=node_color, cmap=cmap, font_size=font_size, with_labels=True)
-#        nx.draw_networkx(G, pos=pos, node_size=node_size, alhpa=alpha, node_color=node_color, cmap=cmap, font_size=font_size)
+        # nx.draw_networkx(G, pos=pos, node_size=node_size, alhpa=alpha, node_color=node_color, cmap=cmap, font_size=font_size)
         
     plt.title(title)
     plt.grid(True)
     plt.show()
     
     # Savefig
     if not isinstance(config['filename'], type(None)):
@@ -255,15 +248,15 @@
 def normalize_size(getsizes, minscale=0.1, maxscale=4):
     getsizes = MinMaxScaler(feature_range=(minscale,maxscale)).fit_transform(getsizes).flatten()
     return(getsizes)
 
 #%% Convert dataframe to Graph
 def df2G(df_nodes, df_edges, verbose=3):
     # Put edge information in G
-#    G = nx.from_pandas_edgelist(df_edges, 'source', 'target', ['weight', 'edge_weight','edge_width','source_label','target_label'])
+    # G = nx.from_pandas_edgelist(df_edges, 'source', 'target', ['weight', 'edge_weight','edge_width','source_label','target_label'])
     
     colnames=list(df_edges.columns.values[~np.isin(df_edges.columns.values,['source','target'])])
     G = nx.from_pandas_edgelist(df_edges, 'source', 'target', colnames)
 
     # Put node info in G
     getnodes=[*G.nodes]
     for col in df_nodes.columns:
@@ -299,15 +292,15 @@
     df_edge_props=pd.DataFrame([*G.edges.values()])
     df_edges=pd.concat([df_edge_links, df_edge_props], axis=1)
     
     # Source and target values
     df_nodes['index_value']=None
     df_edges['source']=None
     df_edges['target']=None
-#    uinodes=np.unique(np.append(df_edges['source_label'], df_edges['target_label']))
+    # uinodes=np.unique(np.append(df_edges['source_label'], df_edges['target_label']))
     uinodes=np.unique(df_nodes['node_name'])
     for i in range(0,len(uinodes)):
         I=(uinodes[i]==df_edges['source_label'])
         df_edges['source'].loc[I]=i
         I=(uinodes[i]==df_edges['target_label'])
         df_edges['target'].loc[I]=i
```

### Comparing `hnet-1.1.8/hnet/savefig.py` & `hnet-1.2.0/hnet/savefig.py`

 * *Files identical despite different names*

### Comparing `hnet-1.1.8/setup.py` & `hnet-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 else:
     raise RuntimeError("Unable to find version string in %s." % (VERSIONFILE,))
 
 # Setup ------------
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
-     install_requires=['colourmap', 'd3heatmap','pypickle','classeval','wget','d3graph','matplotlib','numpy','pandas','statsmodels','networkx','python-louvain','tqdm','sklearn','ismember','imagesc','df2onehot','fsspec'],
+     install_requires=['requests', 'colourmap', 'pypickle', 'classeval', 'matplotlib','numpy','pandas','statsmodels','networkx','python-louvain','tqdm','scikit-learn','ismember','imagesc','df2onehot','fsspec'],
      python_requires='>=3',
      name='hnet',
      version=new_version,
      author="Erdogan Taskesen",
      author_email="erdogant@gmail.com",
      description="Graphical Hypergeometric Networks",
      long_description=long_description,
      long_description_content_type="text/markdown",
-     url="https://github.com/erdogant/hnet",
+     url="https://erdogant.github.io/hnet",
 	 download_url = 'https://github.com/erdogant/hnet/archive/'+new_version+'.tar.gz',
      packages=setuptools.find_packages(), # Searches throughout all dirs for files to include
      include_package_data=True, # Must be true to include files depicted in MANIFEST.in
+     license_files=["LICENSE"],
      classifiers=[
          "Programming Language :: Python :: 3",
          "License :: OSI Approved :: Apache Software License",
          "Operating System :: OS Independent",
      ],
  )
```

