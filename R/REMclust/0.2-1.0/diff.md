# Comparing `tmp/REMclust-0.2.tar.gz` & `tmp/REMclust-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "REMclust-0.2.tar", last modified: Sat Apr 15 18:57:01 2023, max compression
+gzip compressed data, was "REMclust-1.0.tar", last modified: Sun Apr 16 10:27:49 2023, max compression
```

## Comparing `REMclust-0.2.tar` & `REMclust-1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 18:57:01.090703 REMclust-0.2/
--rw-rw-rw-   0        0        0     1080 2023-04-15 18:26:05.000000 REMclust-0.2/LICENSE.txt
--rw-rw-rw-   0        0        0    14543 2023-04-15 18:57:01.092702 REMclust-0.2/PKG-INFO
--rw-rw-rw-   0        0        0    13789 2023-04-15 16:48:51.000000 REMclust-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 18:57:01.045084 REMclust-0.2/REMclust/
--rw-rw-rw-   0        0        0    46628 2023-04-04 13:49:36.000000 REMclust-0.2/REMclust/GaussianMixture.py
--rw-rw-rw-   0        0        0    35817 2023-04-15 18:15:55.000000 REMclust-0.2/REMclust/REM.py
--rw-rw-rw-   0        0        0       28 2023-04-15 17:13:50.000000 REMclust-0.2/REMclust/__init__.py
--rw-rw-rw-   0        0        0    14968 2023-03-24 13:52:40.000000 REMclust-0.2/REMclust/overlap.py
-drwxrwxrwx   0        0        0        0 2023-04-15 18:57:01.088503 REMclust-0.2/REMclust.egg-info/
--rw-rw-rw-   0        0        0    14543 2023-04-15 18:57:00.000000 REMclust-0.2/REMclust.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-04-15 18:57:00.000000 REMclust-0.2/REMclust.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 18:57:00.000000 REMclust-0.2/REMclust.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-04-15 18:57:00.000000 REMclust-0.2/REMclust.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-15 18:57:00.000000 REMclust-0.2/REMclust.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-15 18:57:01.096855 REMclust-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1564 2023-04-15 18:56:55.000000 REMclust-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 10:27:49.958068 REMclust-1.0/
+-rw-rw-rw-   0        0        0     1080 2023-04-15 18:26:05.000000 REMclust-1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0    14707 2023-04-16 10:27:49.959082 REMclust-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13954 2023-04-16 10:26:04.000000 REMclust-1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 10:27:49.896162 REMclust-1.0/REMclust/
+-rw-rw-rw-   0        0        0    46628 2023-04-04 13:49:36.000000 REMclust-1.0/REMclust/GaussianMixture.py
+-rw-rw-rw-   0        0        0    35817 2023-04-15 18:15:55.000000 REMclust-1.0/REMclust/REM.py
+-rw-rw-rw-   0        0        0       28 2023-04-15 17:13:50.000000 REMclust-1.0/REMclust/__init__.py
+-rw-rw-rw-   0        0        0    14968 2023-03-24 13:52:40.000000 REMclust-1.0/REMclust/overlap.py
+drwxrwxrwx   0        0        0        0 2023-04-16 10:27:49.955567 REMclust-1.0/REMclust.egg-info/
+-rw-rw-rw-   0        0        0    14707 2023-04-16 10:27:49.000000 REMclust-1.0/REMclust.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-04-16 10:27:49.000000 REMclust-1.0/REMclust.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 10:27:49.000000 REMclust-1.0/REMclust.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-04-16 10:27:49.000000 REMclust-1.0/REMclust.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-16 10:27:49.000000 REMclust-1.0/REMclust.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-16 10:27:49.962102 REMclust-1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1563 2023-04-16 10:26:04.000000 REMclust-1.0/setup.py
```

### Comparing `REMclust-0.2/LICENSE.txt` & `REMclust-1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `REMclust-0.2/PKG-INFO` & `REMclust-1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: REMclust
-Version: 0.2
+Version: 1.0
 Summary: This is the official implementation of Reinforced EM, a parametric density-based clustering method
 Home-page: https://github.com/r-swords/REMclust
 Author: Joshua Tobin, Mimi Zhang, Chin Pang Ho, Ralph Swords
 Author-email: tobinjo@tcd.ie
 License: MIT
-Download-URL: https://github.com/r-swords/REMclust/archive/refs/tags/v_02.tar.gz
+Download-URL: https://github.com/r-swords/REMclust/archive/refs/tags/v_1.tar.gz
 Keywords: REM,Reinforced EM,Clustering,Density-Based Clustering,Parametric Density-Based Clustering,Gaussian Mixture Models
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # REMclust
 ---
 ### Introduction
 
-REMclust is a python package for model-based clustering based on finite normal mixture modelling. It uses a peak finding criterion to find modes within the data set. An initial mode set is taken to be the means in Gaussian components.
+REMclust is a Python package for model-based clustering based on Gaussian mixture models. It uses a peak finding criterion to find modes within the data set. An initial mode set is taken to be the means in Gaussian components.
 
-Once the initial mode set has been selected, an iterative procedure comprising two blocks are triggered. A mixture is produced for each iteration.
+Once the initial mode set has been selected, an iterative procedure comprising two blocks is triggered. A mixture is produced for each iteration.
 1. An EM block to fit the covariances and mixing proportions of the components
-2. A pruning block to remove one of the components, as part of an efficient model selection strategy.
+2. A pruning block to remove one of the components as part of an efficient model selection strategy.
 
-Additional functionalities are available for displaying and visualizing fitted models along with clustering results.
+Additional functionalities are available for displaying and visualising fitted models and clustering results.
 
 ---
 ### Data
 
-The data set used in this vignette is the [Palmer Archipelago (Antarctica) Penguin Data](https://github.com/allisonhorst/palmerpenguins). The following methods are used simply to load the dataset. In this particular data set, the features are measured across different scales, for example, culmen depth ranges from 13.1 to 21.5, while body mass ranges from 2700 to 6300. This difference in scale can negatively impact the clustering accuracy, so standardisation was performed. Standardisation ensures that all features are measured in comparable scales, and is process that is recommended when that data set that is being clustered has features that vary widely in scale.
+The data set used in this vignette is the [Palmer Archipelago (Antarctica) Penguin Data](https://github.com/allisonhorst/palmerpenguins). In this particular data set, the features are measured across different scales, for example, culmen depth ranges from 13.1 to 21.5, while body mass ranges from 2700 to 6300. This difference in scale can negatively impact the clustering accuracy, so standardisation was performed. Standardisation ensures that all features are measured in comparable scales and is the process that is recommended when the data set that is being clustered has features that vary widely in scale. The following methods are used to load the dataset.
 
 
 ```python
 import numpy as np
 from sklearn import preprocessing
 
 from REMclust import REM
@@ -56,128 +56,126 @@
 ### Initialisation
 The first step in applying REM to the data set is to initialise an REM object.
 ```python
 REM(data, covariance_type='full', criteria='all', bandwidth='diagonal', tol=1e-3, reg_covar=1e-6, max_iter=100)
 ```
 - **data (array-like of shape (n_samples, n_features))**: The data the model is being fitted to.
 - **covariance_type {'full', 'tied', 'diag', 'spherical'}**: A string describing the type of covariance parameters to use. â€˜fullâ€™: each component has its own general covariance matrix. â€˜tiedâ€™: all components share the same general covariance matrix. â€˜diagâ€™: each component has its own diagonal covariance matrix. â€˜sphericalâ€™: each component has its own single variance.
-- **criteria {'all', 'aic', 'bic', 'icl'}**: A string defining the criterion score used in model selection. At the end of each iteration of REM, a mixture is produced. The mixture minimises this score will be taken as the optimal clustering.
+- **criteria {'all', 'aic', 'bic', 'icl'}**: A string defining the criterion score used in model selection. At the end of each iteration of REM, a mixture is produced. The mixture that minimises this score will be taken as the optimal clustering.
 - **bandwidth ({'diagonal', 'spherical', 'normal_reference'}, int, float)**: Either a string, integer, or floating point number that defines the bandwidth used when finding the modes.
 - **tol (float)**: The convergence threshold. EM iterations will stop when the lower bound average gain is below this threshold.
-- **reg_covar (float)**: Non-negative regularization added to the diagonal of covariance. Allows to assure that the covariance matrices are all positive.
+- **reg_covar (float)**: Non-negative regularisation added to the diagonal of covariance. Allows to ensure that the covariance matrices are all positive.
 - **max_iter (int)**: The number of EM iterations to perform.
 
 
 ```python
 bndwk = int(np.floor(np.min((30, np.log(n_samples)))))
-cluster = REM.REM(data=x, covariance_type="full", criteria="icl",bandwidth=bndwk, tol=1e-4)
+cluster = REM(data=x, covariance_type="full", criteria="icl",bandwidth=bndwk, tol=1e-4)
 ```
 
 ### Mode Selection
 
-The initial mode set must be selected by the user. To do this, they must select a *distance_threshold* and *density_threshold*. To aid in this, the method
+The user must select the initial mode set. To do this, they must select a *distance_threshold* and *density_threshold*. To aid in this, the method
 ```python
 REM.mode_decision_plot()
 ```
-is provided. This draws two plots, one is a plot of the distance between a point to its nearest neighbor with a higher density against the points' density. This plot will allow the user to select the appropriate thresholds. The ideal modes have both a high distance and density. The second plot shows the product of the distance and the density for each point, allowing the user to clearly the likely number of modes.
+is provided. This method draws two plots. One is a plot of the distance between a point to its nearest neighbour with a higher density against the points' density. This plot will allow the user to select the appropriate thresholds. The ideal modes have both a high distance and density. The second plot shows the product of the distance and the density for each point, allowing the user to determine the likely number of modes easily.
 
 
 ```python
 cluster.mode_decision_plot()
 ```
 
-
-    
-![png](REMclust_vignette_files/REMclust_vignette_6_0.png)
+![](https://github.com/r-swords/REMclust/raw/main/REMclust_vignette_files/REMclust_vignette_6_0.png)
     
 
 
 REMclust also provides the method:
 ```python
 REM.kde_contour_plot(dimensions=None, axis_labels=None)
 ```
-- **dimensions (list(int))**: A list of integers that defines the features that will be plotted. If left as None all features will be plotted.
+- **dimensions (list(int))**: A list of integers that defines the features that will be plotted. If left as None, all features will be plotted.
 - **axis_labels (list(str))**: A list of strings that define the labels for the axes.
 
-This provides a contour plot of the estimated KDE densities.
+This method provides a contour plot of the estimated KDE densities.
 
 
 ```python
 cluster.kde_contour_plot(dimensions=[1, 2, 4, 5], axis_labels=[labels[1], labels[2], labels[4], labels[5]])
 ```
 
 
     
-![png](REMclust_vignette_files/REMclust_vignette_8_0.png)
+![](https://github.com/r-swords/REMclust/raw/main/REMclust_vignette_files/REMclust_vignette_8_0.png)
     
 
 
 ### Clustering
 
 To perform clustering, the following method is run:
 ```python
 fit(max_components=5, density_threshold=None, distance_threshold=None)
 ```
 - **max_components (int)**: An integer that defines the initial size of the mode set. The modes with the highest $density \times distance$ will fill the set.
-- **density_threshold (float)**: A float that defines the threshold for the mode's density. A mode must have a higher density to be included in the initial mode set.
-- **distance_threshold (float)**: A float that defines the threshold for the mode's distance. A mode must have a higher distance to be included in the initial mode set.
+- **density_threshold (float)**: A float defining the mode's density threshold. A mode must have a higher density to be included in the initial mode set.
+- **distance_threshold (float)**: A float defining the mode's distance threshold. A mode must have a higher distance to be included in the initial mode set.
 
 **Note:** There are two possible ways to define the mode set:
 1. Setting the max components value k, in which the k modes with the highest $density \times distance$ will be included in the initial mode set.
-2. Setting the two thresholds, in which the modes that exceed both thresholds will be included in the initial mode set.
+2. Setting the two thresholds will include the modes exceeding both in the initial mode set.
 
 Should the user set the max components and the thresholds, the mode set created by the thresholds will be preferred.
 
 
 ```python
 cluster.fit(density_threshold = 1.6, distance_threshold = 3)
 ```
 
 ---
 
 
 ### Visualisation
 
-REMclust provides visualisation tools that allow the user to explore results of the clustering. The first of these is:
+REMclust provides visualisation tools that allow the user to explore the clustering results. The first of these is:
 ```python
 REM.classification_plot(mixture_selection='', dimensions=None, axis_labels=None)
 ```
-A plot of the classification of the data that the clustering was performed on.
-- **mixture_selection {'', 'aic', bic', 'icl'}** This defines whether the user would like plot the results from the model selected by AIC, BIC, or ICL. If the initial criterion was set to 'all', this is required, otherwise it should not be set.
+A plot of the classification of the data on which the clustering was performed.
+- **mixture_selection {'', 'aic', bic', 'icl'}** This defines whether the user would like to plot the results from the model selected by AIC, BIC, or ICL. This is required if the initial criterion was set to 'all'. Otherwise, it should not be set.
 - **dimensions (list(int))**: A list of integers that defines the features that will be plotted. If left as None all features will be plotted.
 - **axis_labels (list(str))**: A list of strings that define the labels for the axes.
 
 
 ```python
 cluster.classification_plot(dimensions=[0,1,2], axis_labels=[labels[0], labels[1], labels[2]])
 ```
 
 
     
-![png](REMclust_vignette_files/REMclust_vignette_12_0.png)
+![](https://github.com/r-swords/REMclust/raw/main/REMclust_vignette_files/REMclust_vignette_12_0.png)
     
 
 
 Another visualisation method provided by REMclust is:
 ```python
 REM.uncertainty_plot(mixture_selection='', dimensions=None, axis_labels=None)
 ```
-A plot of the uncertainty of the data that the clustering was performed on. Uncertainty measured as inverse of the difference between probability that a point belongs to the cluster it was assigned and the probability that it belongs to the next most likely cluster. The uncertainty score for a point is represented by its size in the scatter plot
-- **mixture_selection {'', 'aic', bic', 'icl'}** This defines whether the user would like plot the results from the model selected by AIC, BIC, or ICL. If the initial criterion was set to 'all', this is required, otherwise it should not be set.
+A plot of the uncertainty of the data that the clustering was performed on. Uncertainty is measured as the inverse of the difference between the probability that a point belongs to the assigned cluster and the probability that it belongs to the next most likely cluster. The uncertainty score for a point is represented by its size in the scatter plot
+- **mixture_selection {'', 'aic', bic', 'icl'}** This defines whether the user would like to plot the results from the model selected by AIC, BIC, or ICL. This is required if the initial criterion was set to 'all'. Otherwise, it should not be set.
 - **dimensions (list(int))**: A list of integers that defines the features that will be plotted. If left as None all features will be plotted.
 - **axis_labels (list(str))**: A list of strings that define the labels for the axes.
 
 
 ```python
 cluster.uncertainty_plot()
 ```
 
 
     
-![png](REMclust_vignette_files/REMclust_vignette_14_0.png)
+![](https://github.com/r-swords/REMclust/raw/main/REMclust_vignette_files/REMclust_vignette_14_0.png)
     
 
 
 Finally, REMclust provides:
 ```python
 REM.criterion_plot()
 ```
@@ -186,26 +184,26 @@
 
 ```python
 cluster.criterion_plot()
 ```
 
 
     
-![png](REMclust_vignette_files/REMclust_vignette_16_0.png)
+![](https://raw.githubusercontent.com/r-swords/REMclust/main/REMclust_vignette_files/REMclust_vignette_16_0.png)
     
 
 
 ### Summary
-As well as visualisations, REMclust also provides a method that prints text based summaries of the clustering results.
+As well as visualisations, REMclust also provides a method that prints text-based summaries of the clustering results.
 ```python
 REM.summary(parameters=False, classification=False, criterion_scores=False)
 ```
 - **parameters (boolean)**: If TRUE, the parameters of mixture components are printed.
 - **classification (boolean)**: If TRUE, a table of classifications/clustering of observations is printed.
-- **criterion_scores (boolean)**: If TRUE, the criterion scores of all the models tested are printed.
+- **criterion_scores (boolean)**: If TRUE, all the tested models' criterion scores are printed.
 
 
 ```python
 cluster.summary(parameters=True, classification=True, criterion_scores=True)
 ```
 
     ICL scores:
```

### Comparing `REMclust-0.2/README.md` & `REMclust-1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # REMclust
 ---
 ### Introduction
 
-REMclust is a python package for model-based clustering based on finite normal mixture modelling. It uses a peak finding criterion to find modes within the data set. An initial mode set is taken to be the means in Gaussian components.
+REMclust is a Python package for model-based clustering based on Gaussian mixture models. It uses a peak finding criterion to find modes within the data set. An initial mode set is taken to be the means in Gaussian components.
 
-Once the initial mode set has been selected, an iterative procedure comprising two blocks are triggered. A mixture is produced for each iteration.
+Once the initial mode set has been selected, an iterative procedure comprising two blocks is triggered. A mixture is produced for each iteration.
 1. An EM block to fit the covariances and mixing proportions of the components
-2. A pruning block to remove one of the components, as part of an efficient model selection strategy.
+2. A pruning block to remove one of the components as part of an efficient model selection strategy.
 
-Additional functionalities are available for displaying and visualizing fitted models along with clustering results.
+Additional functionalities are available for displaying and visualising fitted models and clustering results.
 
 ---
 ### Data
 
-The data set used in this vignette is the [Palmer Archipelago (Antarctica) Penguin Data](https://github.com/allisonhorst/palmerpenguins). The following methods are used simply to load the dataset. In this particular data set, the features are measured across different scales, for example, culmen depth ranges from 13.1 to 21.5, while body mass ranges from 2700 to 6300. This difference in scale can negatively impact the clustering accuracy, so standardisation was performed. Standardisation ensures that all features are measured in comparable scales, and is process that is recommended when that data set that is being clustered has features that vary widely in scale.
+The data set used in this vignette is the [Palmer Archipelago (Antarctica) Penguin Data](https://github.com/allisonhorst/palmerpenguins). In this particular data set, the features are measured across different scales, for example, culmen depth ranges from 13.1 to 21.5, while body mass ranges from 2700 to 6300. This difference in scale can negatively impact the clustering accuracy, so standardisation was performed. Standardisation ensures that all features are measured in comparable scales and is the process that is recommended when the data set that is being clustered has features that vary widely in scale. The following methods are used to load the dataset.
 
 
 ```python
 import numpy as np
 from sklearn import preprocessing
 
 from REMclust import REM
@@ -40,128 +40,126 @@
 ### Initialisation
 The first step in applying REM to the data set is to initialise an REM object.
 ```python
 REM(data, covariance_type='full', criteria='all', bandwidth='diagonal', tol=1e-3, reg_covar=1e-6, max_iter=100)
 ```
 - **data (array-like of shape (n_samples, n_features))**: The data the model is being fitted to.
 - **covariance_type {'full', 'tied', 'diag', 'spherical'}**: A string describing the type of covariance parameters to use. ‘full’: each component has its own general covariance matrix. ‘tied’: all components share the same general covariance matrix. ‘diag’: each component has its own diagonal covariance matrix. ‘spherical’: each component has its own single variance.
-- **criteria {'all', 'aic', 'bic', 'icl'}**: A string defining the criterion score used in model selection. At the end of each iteration of REM, a mixture is produced. The mixture minimises this score will be taken as the optimal clustering.
+- **criteria {'all', 'aic', 'bic', 'icl'}**: A string defining the criterion score used in model selection. At the end of each iteration of REM, a mixture is produced. The mixture that minimises this score will be taken as the optimal clustering.
 - **bandwidth ({'diagonal', 'spherical', 'normal_reference'}, int, float)**: Either a string, integer, or floating point number that defines the bandwidth used when finding the modes.
 - **tol (float)**: The convergence threshold. EM iterations will stop when the lower bound average gain is below this threshold.
-- **reg_covar (float)**: Non-negative regularization added to the diagonal of covariance. Allows to assure that the covariance matrices are all positive.
+- **reg_covar (float)**: Non-negative regularisation added to the diagonal of covariance. Allows to ensure that the covariance matrices are all positive.
 - **max_iter (int)**: The number of EM iterations to perform.
 
 
 ```python
 bndwk = int(np.floor(np.min((30, np.log(n_samples)))))
-cluster = REM.REM(data=x, covariance_type="full", criteria="icl",bandwidth=bndwk, tol=1e-4)
+cluster = REM(data=x, covariance_type="full", criteria="icl",bandwidth=bndwk, tol=1e-4)
 ```
 
 ### Mode Selection
 
-The initial mode set must be selected by the user. To do this, they must select a *distance_threshold* and *density_threshold*. To aid in this, the method
+The user must select the initial mode set. To do this, they must select a *distance_threshold* and *density_threshold*. To aid in this, the method
 ```python
 REM.mode_decision_plot()
 ```
-is provided. This draws two plots, one is a plot of the distance between a point to its nearest neighbor with a higher density against the points' density. This plot will allow the user to select the appropriate thresholds. The ideal modes have both a high distance and density. The second plot shows the product of the distance and the density for each point, allowing the user to clearly the likely number of modes.
+is provided. This method draws two plots. One is a plot of the distance between a point to its nearest neighbour with a higher density against the points' density. This plot will allow the user to select the appropriate thresholds. The ideal modes have both a high distance and density. The second plot shows the product of the distance and the density for each point, allowing the user to determine the likely number of modes easily.
 
 
 ```python
 cluster.mode_decision_plot()
 ```
 
-
-    
-![png](REMclust_vignette_files/REMclust_vignette_6_0.png)
+![](https://github.com/r-swords/REMclust/raw/main/REMclust_vignette_files/REMclust_vignette_6_0.png)
     
 
 
 REMclust also provides the method:
 ```python
 REM.kde_contour_plot(dimensions=None, axis_labels=None)
 ```
-- **dimensions (list(int))**: A list of integers that defines the features that will be plotted. If left as None all features will be plotted.
+- **dimensions (list(int))**: A list of integers that defines the features that will be plotted. If left as None, all features will be plotted.
 - **axis_labels (list(str))**: A list of strings that define the labels for the axes.
 
-This provides a contour plot of the estimated KDE densities.
+This method provides a contour plot of the estimated KDE densities.
 
 
 ```python
 cluster.kde_contour_plot(dimensions=[1, 2, 4, 5], axis_labels=[labels[1], labels[2], labels[4], labels[5]])
 ```
 
 
     
-![png](REMclust_vignette_files/REMclust_vignette_8_0.png)
+![](https://github.com/r-swords/REMclust/raw/main/REMclust_vignette_files/REMclust_vignette_8_0.png)
     
 
 
 ### Clustering
 
 To perform clustering, the following method is run:
 ```python
 fit(max_components=5, density_threshold=None, distance_threshold=None)
 ```
 - **max_components (int)**: An integer that defines the initial size of the mode set. The modes with the highest $density \times distance$ will fill the set.
-- **density_threshold (float)**: A float that defines the threshold for the mode's density. A mode must have a higher density to be included in the initial mode set.
-- **distance_threshold (float)**: A float that defines the threshold for the mode's distance. A mode must have a higher distance to be included in the initial mode set.
+- **density_threshold (float)**: A float defining the mode's density threshold. A mode must have a higher density to be included in the initial mode set.
+- **distance_threshold (float)**: A float defining the mode's distance threshold. A mode must have a higher distance to be included in the initial mode set.
 
 **Note:** There are two possible ways to define the mode set:
 1. Setting the max components value k, in which the k modes with the highest $density \times distance$ will be included in the initial mode set.
-2. Setting the two thresholds, in which the modes that exceed both thresholds will be included in the initial mode set.
+2. Setting the two thresholds will include the modes exceeding both in the initial mode set.
 
 Should the user set the max components and the thresholds, the mode set created by the thresholds will be preferred.
 
 
 ```python
 cluster.fit(density_threshold = 1.6, distance_threshold = 3)
 ```
 
 ---
 
 
 ### Visualisation
 
-REMclust provides visualisation tools that allow the user to explore results of the clustering. The first of these is:
+REMclust provides visualisation tools that allow the user to explore the clustering results. The first of these is:
 ```python
 REM.classification_plot(mixture_selection='', dimensions=None, axis_labels=None)
 ```
-A plot of the classification of the data that the clustering was performed on.
-- **mixture_selection {'', 'aic', bic', 'icl'}** This defines whether the user would like plot the results from the model selected by AIC, BIC, or ICL. If the initial criterion was set to 'all', this is required, otherwise it should not be set.
+A plot of the classification of the data on which the clustering was performed.
+- **mixture_selection {'', 'aic', bic', 'icl'}** This defines whether the user would like to plot the results from the model selected by AIC, BIC, or ICL. This is required if the initial criterion was set to 'all'. Otherwise, it should not be set.
 - **dimensions (list(int))**: A list of integers that defines the features that will be plotted. If left as None all features will be plotted.
 - **axis_labels (list(str))**: A list of strings that define the labels for the axes.
 
 
 ```python
 cluster.classification_plot(dimensions=[0,1,2], axis_labels=[labels[0], labels[1], labels[2]])
 ```
 
 
     
-![png](REMclust_vignette_files/REMclust_vignette_12_0.png)
+![](https://github.com/r-swords/REMclust/raw/main/REMclust_vignette_files/REMclust_vignette_12_0.png)
     
 
 
 Another visualisation method provided by REMclust is:
 ```python
 REM.uncertainty_plot(mixture_selection='', dimensions=None, axis_labels=None)
 ```
-A plot of the uncertainty of the data that the clustering was performed on. Uncertainty measured as inverse of the difference between probability that a point belongs to the cluster it was assigned and the probability that it belongs to the next most likely cluster. The uncertainty score for a point is represented by its size in the scatter plot
-- **mixture_selection {'', 'aic', bic', 'icl'}** This defines whether the user would like plot the results from the model selected by AIC, BIC, or ICL. If the initial criterion was set to 'all', this is required, otherwise it should not be set.
+A plot of the uncertainty of the data that the clustering was performed on. Uncertainty is measured as the inverse of the difference between the probability that a point belongs to the assigned cluster and the probability that it belongs to the next most likely cluster. The uncertainty score for a point is represented by its size in the scatter plot
+- **mixture_selection {'', 'aic', bic', 'icl'}** This defines whether the user would like to plot the results from the model selected by AIC, BIC, or ICL. This is required if the initial criterion was set to 'all'. Otherwise, it should not be set.
 - **dimensions (list(int))**: A list of integers that defines the features that will be plotted. If left as None all features will be plotted.
 - **axis_labels (list(str))**: A list of strings that define the labels for the axes.
 
 
 ```python
 cluster.uncertainty_plot()
 ```
 
 
     
-![png](REMclust_vignette_files/REMclust_vignette_14_0.png)
+![](https://github.com/r-swords/REMclust/raw/main/REMclust_vignette_files/REMclust_vignette_14_0.png)
     
 
 
 Finally, REMclust provides:
 ```python
 REM.criterion_plot()
 ```
@@ -170,26 +168,26 @@
 
 ```python
 cluster.criterion_plot()
 ```
 
 
     
-![png](REMclust_vignette_files/REMclust_vignette_16_0.png)
+![](https://raw.githubusercontent.com/r-swords/REMclust/main/REMclust_vignette_files/REMclust_vignette_16_0.png)
     
 
 
 ### Summary
-As well as visualisations, REMclust also provides a method that prints text based summaries of the clustering results.
+As well as visualisations, REMclust also provides a method that prints text-based summaries of the clustering results.
 ```python
 REM.summary(parameters=False, classification=False, criterion_scores=False)
 ```
 - **parameters (boolean)**: If TRUE, the parameters of mixture components are printed.
 - **classification (boolean)**: If TRUE, a table of classifications/clustering of observations is printed.
-- **criterion_scores (boolean)**: If TRUE, the criterion scores of all the models tested are printed.
+- **criterion_scores (boolean)**: If TRUE, all the tested models' criterion scores are printed.
 
 
 ```python
 cluster.summary(parameters=True, classification=True, criterion_scores=True)
 ```
 
     ICL scores:
```

### Comparing `REMclust-0.2/REMclust/GaussianMixture.py` & `REMclust-1.0/REMclust/GaussianMixture.py`

 * *Files identical despite different names*

### Comparing `REMclust-0.2/REMclust/REM.py` & `REMclust-1.0/REMclust/REM.py`

 * *Files identical despite different names*

### Comparing `REMclust-0.2/REMclust/overlap.py` & `REMclust-1.0/REMclust/overlap.py`

 * *Files identical despite different names*

### Comparing `REMclust-0.2/REMclust.egg-info/PKG-INFO` & `REMclust-1.0/REMclust.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: REMclust
-Version: 0.2
+Version: 1.0
 Summary: This is the official implementation of Reinforced EM, a parametric density-based clustering method
 Home-page: https://github.com/r-swords/REMclust
 Author: Joshua Tobin, Mimi Zhang, Chin Pang Ho, Ralph Swords
 Author-email: tobinjo@tcd.ie
 License: MIT
-Download-URL: https://github.com/r-swords/REMclust/archive/refs/tags/v_02.tar.gz
+Download-URL: https://github.com/r-swords/REMclust/archive/refs/tags/v_1.tar.gz
 Keywords: REM,Reinforced EM,Clustering,Density-Based Clustering,Parametric Density-Based Clustering,Gaussian Mixture Models
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # REMclust
 ---
 ### Introduction
 
-REMclust is a python package for model-based clustering based on finite normal mixture modelling. It uses a peak finding criterion to find modes within the data set. An initial mode set is taken to be the means in Gaussian components.
+REMclust is a Python package for model-based clustering based on Gaussian mixture models. It uses a peak finding criterion to find modes within the data set. An initial mode set is taken to be the means in Gaussian components.
 
-Once the initial mode set has been selected, an iterative procedure comprising two blocks are triggered. A mixture is produced for each iteration.
+Once the initial mode set has been selected, an iterative procedure comprising two blocks is triggered. A mixture is produced for each iteration.
 1. An EM block to fit the covariances and mixing proportions of the components
-2. A pruning block to remove one of the components, as part of an efficient model selection strategy.
+2. A pruning block to remove one of the components as part of an efficient model selection strategy.
 
-Additional functionalities are available for displaying and visualizing fitted models along with clustering results.
+Additional functionalities are available for displaying and visualising fitted models and clustering results.
 
 ---
 ### Data
 
-The data set used in this vignette is the [Palmer Archipelago (Antarctica) Penguin Data](https://github.com/allisonhorst/palmerpenguins). The following methods are used simply to load the dataset. In this particular data set, the features are measured across different scales, for example, culmen depth ranges from 13.1 to 21.5, while body mass ranges from 2700 to 6300. This difference in scale can negatively impact the clustering accuracy, so standardisation was performed. Standardisation ensures that all features are measured in comparable scales, and is process that is recommended when that data set that is being clustered has features that vary widely in scale.
+The data set used in this vignette is the [Palmer Archipelago (Antarctica) Penguin Data](https://github.com/allisonhorst/palmerpenguins). In this particular data set, the features are measured across different scales, for example, culmen depth ranges from 13.1 to 21.5, while body mass ranges from 2700 to 6300. This difference in scale can negatively impact the clustering accuracy, so standardisation was performed. Standardisation ensures that all features are measured in comparable scales and is the process that is recommended when the data set that is being clustered has features that vary widely in scale. The following methods are used to load the dataset.
 
 
 ```python
 import numpy as np
 from sklearn import preprocessing
 
 from REMclust import REM
@@ -56,128 +56,126 @@
 ### Initialisation
 The first step in applying REM to the data set is to initialise an REM object.
 ```python
 REM(data, covariance_type='full', criteria='all', bandwidth='diagonal', tol=1e-3, reg_covar=1e-6, max_iter=100)
 ```
 - **data (array-like of shape (n_samples, n_features))**: The data the model is being fitted to.
 - **covariance_type {'full', 'tied', 'diag', 'spherical'}**: A string describing the type of covariance parameters to use. â€˜fullâ€™: each component has its own general covariance matrix. â€˜tiedâ€™: all components share the same general covariance matrix. â€˜diagâ€™: each component has its own diagonal covariance matrix. â€˜sphericalâ€™: each component has its own single variance.
-- **criteria {'all', 'aic', 'bic', 'icl'}**: A string defining the criterion score used in model selection. At the end of each iteration of REM, a mixture is produced. The mixture minimises this score will be taken as the optimal clustering.
+- **criteria {'all', 'aic', 'bic', 'icl'}**: A string defining the criterion score used in model selection. At the end of each iteration of REM, a mixture is produced. The mixture that minimises this score will be taken as the optimal clustering.
 - **bandwidth ({'diagonal', 'spherical', 'normal_reference'}, int, float)**: Either a string, integer, or floating point number that defines the bandwidth used when finding the modes.
 - **tol (float)**: The convergence threshold. EM iterations will stop when the lower bound average gain is below this threshold.
-- **reg_covar (float)**: Non-negative regularization added to the diagonal of covariance. Allows to assure that the covariance matrices are all positive.
+- **reg_covar (float)**: Non-negative regularisation added to the diagonal of covariance. Allows to ensure that the covariance matrices are all positive.
 - **max_iter (int)**: The number of EM iterations to perform.
 
 
 ```python
 bndwk = int(np.floor(np.min((30, np.log(n_samples)))))
-cluster = REM.REM(data=x, covariance_type="full", criteria="icl",bandwidth=bndwk, tol=1e-4)
+cluster = REM(data=x, covariance_type="full", criteria="icl",bandwidth=bndwk, tol=1e-4)
 ```
 
 ### Mode Selection
 
-The initial mode set must be selected by the user. To do this, they must select a *distance_threshold* and *density_threshold*. To aid in this, the method
+The user must select the initial mode set. To do this, they must select a *distance_threshold* and *density_threshold*. To aid in this, the method
 ```python
 REM.mode_decision_plot()
 ```
-is provided. This draws two plots, one is a plot of the distance between a point to its nearest neighbor with a higher density against the points' density. This plot will allow the user to select the appropriate thresholds. The ideal modes have both a high distance and density. The second plot shows the product of the distance and the density for each point, allowing the user to clearly the likely number of modes.
+is provided. This method draws two plots. One is a plot of the distance between a point to its nearest neighbour with a higher density against the points' density. This plot will allow the user to select the appropriate thresholds. The ideal modes have both a high distance and density. The second plot shows the product of the distance and the density for each point, allowing the user to determine the likely number of modes easily.
 
 
 ```python
 cluster.mode_decision_plot()
 ```
 
-
-    
-![png](REMclust_vignette_files/REMclust_vignette_6_0.png)
+![](https://github.com/r-swords/REMclust/raw/main/REMclust_vignette_files/REMclust_vignette_6_0.png)
     
 
 
 REMclust also provides the method:
 ```python
 REM.kde_contour_plot(dimensions=None, axis_labels=None)
 ```
-- **dimensions (list(int))**: A list of integers that defines the features that will be plotted. If left as None all features will be plotted.
+- **dimensions (list(int))**: A list of integers that defines the features that will be plotted. If left as None, all features will be plotted.
 - **axis_labels (list(str))**: A list of strings that define the labels for the axes.
 
-This provides a contour plot of the estimated KDE densities.
+This method provides a contour plot of the estimated KDE densities.
 
 
 ```python
 cluster.kde_contour_plot(dimensions=[1, 2, 4, 5], axis_labels=[labels[1], labels[2], labels[4], labels[5]])
 ```
 
 
     
-![png](REMclust_vignette_files/REMclust_vignette_8_0.png)
+![](https://github.com/r-swords/REMclust/raw/main/REMclust_vignette_files/REMclust_vignette_8_0.png)
     
 
 
 ### Clustering
 
 To perform clustering, the following method is run:
 ```python
 fit(max_components=5, density_threshold=None, distance_threshold=None)
 ```
 - **max_components (int)**: An integer that defines the initial size of the mode set. The modes with the highest $density \times distance$ will fill the set.
-- **density_threshold (float)**: A float that defines the threshold for the mode's density. A mode must have a higher density to be included in the initial mode set.
-- **distance_threshold (float)**: A float that defines the threshold for the mode's distance. A mode must have a higher distance to be included in the initial mode set.
+- **density_threshold (float)**: A float defining the mode's density threshold. A mode must have a higher density to be included in the initial mode set.
+- **distance_threshold (float)**: A float defining the mode's distance threshold. A mode must have a higher distance to be included in the initial mode set.
 
 **Note:** There are two possible ways to define the mode set:
 1. Setting the max components value k, in which the k modes with the highest $density \times distance$ will be included in the initial mode set.
-2. Setting the two thresholds, in which the modes that exceed both thresholds will be included in the initial mode set.
+2. Setting the two thresholds will include the modes exceeding both in the initial mode set.
 
 Should the user set the max components and the thresholds, the mode set created by the thresholds will be preferred.
 
 
 ```python
 cluster.fit(density_threshold = 1.6, distance_threshold = 3)
 ```
 
 ---
 
 
 ### Visualisation
 
-REMclust provides visualisation tools that allow the user to explore results of the clustering. The first of these is:
+REMclust provides visualisation tools that allow the user to explore the clustering results. The first of these is:
 ```python
 REM.classification_plot(mixture_selection='', dimensions=None, axis_labels=None)
 ```
-A plot of the classification of the data that the clustering was performed on.
-- **mixture_selection {'', 'aic', bic', 'icl'}** This defines whether the user would like plot the results from the model selected by AIC, BIC, or ICL. If the initial criterion was set to 'all', this is required, otherwise it should not be set.
+A plot of the classification of the data on which the clustering was performed.
+- **mixture_selection {'', 'aic', bic', 'icl'}** This defines whether the user would like to plot the results from the model selected by AIC, BIC, or ICL. This is required if the initial criterion was set to 'all'. Otherwise, it should not be set.
 - **dimensions (list(int))**: A list of integers that defines the features that will be plotted. If left as None all features will be plotted.
 - **axis_labels (list(str))**: A list of strings that define the labels for the axes.
 
 
 ```python
 cluster.classification_plot(dimensions=[0,1,2], axis_labels=[labels[0], labels[1], labels[2]])
 ```
 
 
     
-![png](REMclust_vignette_files/REMclust_vignette_12_0.png)
+![](https://github.com/r-swords/REMclust/raw/main/REMclust_vignette_files/REMclust_vignette_12_0.png)
     
 
 
 Another visualisation method provided by REMclust is:
 ```python
 REM.uncertainty_plot(mixture_selection='', dimensions=None, axis_labels=None)
 ```
-A plot of the uncertainty of the data that the clustering was performed on. Uncertainty measured as inverse of the difference between probability that a point belongs to the cluster it was assigned and the probability that it belongs to the next most likely cluster. The uncertainty score for a point is represented by its size in the scatter plot
-- **mixture_selection {'', 'aic', bic', 'icl'}** This defines whether the user would like plot the results from the model selected by AIC, BIC, or ICL. If the initial criterion was set to 'all', this is required, otherwise it should not be set.
+A plot of the uncertainty of the data that the clustering was performed on. Uncertainty is measured as the inverse of the difference between the probability that a point belongs to the assigned cluster and the probability that it belongs to the next most likely cluster. The uncertainty score for a point is represented by its size in the scatter plot
+- **mixture_selection {'', 'aic', bic', 'icl'}** This defines whether the user would like to plot the results from the model selected by AIC, BIC, or ICL. This is required if the initial criterion was set to 'all'. Otherwise, it should not be set.
 - **dimensions (list(int))**: A list of integers that defines the features that will be plotted. If left as None all features will be plotted.
 - **axis_labels (list(str))**: A list of strings that define the labels for the axes.
 
 
 ```python
 cluster.uncertainty_plot()
 ```
 
 
     
-![png](REMclust_vignette_files/REMclust_vignette_14_0.png)
+![](https://github.com/r-swords/REMclust/raw/main/REMclust_vignette_files/REMclust_vignette_14_0.png)
     
 
 
 Finally, REMclust provides:
 ```python
 REM.criterion_plot()
 ```
@@ -186,26 +184,26 @@
 
 ```python
 cluster.criterion_plot()
 ```
 
 
     
-![png](REMclust_vignette_files/REMclust_vignette_16_0.png)
+![](https://raw.githubusercontent.com/r-swords/REMclust/main/REMclust_vignette_files/REMclust_vignette_16_0.png)
     
 
 
 ### Summary
-As well as visualisations, REMclust also provides a method that prints text based summaries of the clustering results.
+As well as visualisations, REMclust also provides a method that prints text-based summaries of the clustering results.
 ```python
 REM.summary(parameters=False, classification=False, criterion_scores=False)
 ```
 - **parameters (boolean)**: If TRUE, the parameters of mixture components are printed.
 - **classification (boolean)**: If TRUE, a table of classifications/clustering of observations is printed.
-- **criterion_scores (boolean)**: If TRUE, the criterion scores of all the models tested are printed.
+- **criterion_scores (boolean)**: If TRUE, all the tested models' criterion scores are printed.
 
 
 ```python
 cluster.summary(parameters=True, classification=True, criterion_scores=True)
 ```
 
     ICL scores:
```

### Comparing `REMclust-0.2/setup.py` & `REMclust-1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, Extension
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 setup(
   name='REMclust',         # How you named your package folder (MyLib)
   packages=['REMclust'],   # Chose the same as "name"
-  version='0.2',      # Start with a small number and increase it with every change you make
+  version='1.0',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description='This is the official implementation of Reinforced EM, a parametric density-based clustering method',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author='Joshua Tobin, Mimi Zhang, Chin Pang Ho, Ralph Swords',                   # Type in your name
   author_email='tobinjo@tcd.ie',      # Type in your E-Mail
   url='https://github.com/r-swords/REMclust',
-  download_url='https://github.com/r-swords/REMclust/archive/refs/tags/v_02.tar.gz',
+  download_url='https://github.com/r-swords/REMclust/archive/refs/tags/v_1.tar.gz',
   keywords=['REM', 'Reinforced EM', 'Clustering', 'Density-Based Clustering', 'Parametric Density-Based Clustering', 'Gaussian Mixture Models'],   # Keywords that define your package best
   install_requires=[
     'numpy',
     'matplotlib',
     'scipy',
     'scikit-learn',
     'pandas',
```

