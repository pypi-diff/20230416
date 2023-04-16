# Comparing `tmp/edynamics-0.1.3.tar.gz` & `tmp/edynamics-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edynamics-0.1.3.tar", last modified: Thu Jan 19 02:45:11 2023, max compression
+gzip compressed data, was "edynamics-0.3.9.tar", last modified: Sun Apr 16 04:24:28 2023, max compression
```

## Comparing `edynamics-0.1.3.tar` & `edynamics-0.3.9.tar`

### file list

```diff
@@ -1,11 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-01-19 02:45:11.284256 edynamics-0.1.3/
--rw-rw-rw-   0        0        0      504 2023-01-19 02:45:11.284256 edynamics-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-05 23:32:19.000000 edynamics-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-01-19 02:45:11.281223 edynamics-0.1.3/edynamics.egg-info/
--rw-rw-rw-   0        0        0      504 2023-01-19 02:45:11.000000 edynamics-0.1.3/edynamics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-01-19 02:45:11.000000 edynamics-0.1.3/edynamics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-19 02:45:11.000000 edynamics-0.1.3/edynamics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-01-19 02:45:11.000000 edynamics-0.1.3/edynamics.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-01-19 02:45:11.000000 edynamics-0.1.3/edynamics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-19 02:45:11.288133 edynamics-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      763 2023-01-19 02:43:18.000000 edynamics-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 04:24:28.925397 edynamics-0.3.9/
+-rw-rw-rw-   0        0        0      608 2023-04-16 04:24:28.926395 edynamics-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-05 23:32:19.000000 edynamics-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 04:24:28.855397 edynamics-0.3.9/edynamics.egg-info/
+-rw-rw-rw-   0        0        0      608 2023-04-16 04:24:28.000000 edynamics-0.3.9/edynamics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2326 2023-04-16 04:24:28.000000 edynamics-0.3.9/edynamics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 04:24:28.000000 edynamics-0.3.9/edynamics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-04-16 04:24:28.000000 edynamics-0.3.9/edynamics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-16 04:24:28.000000 edynamics-0.3.9/edynamics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 04:24:28.928397 edynamics-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-04-16 04:20:54.000000 edynamics-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 04:24:28.856397 edynamics-0.3.9/src/
+-rw-rw-rw-   0        0        0        0 2023-04-16 04:18:38.000000 edynamics-0.3.9/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 04:24:28.858397 edynamics-0.3.9/src/edynamics/
+-rw-rw-rw-   0        0        0      279 2023-03-17 20:08:14.000000 edynamics-0.3.9/src/edynamics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 04:24:28.860397 edynamics-0.3.9/src/edynamics/modelling_tools/
+-rw-rw-rw-   0        0        0      335 2023-03-17 20:08:42.000000 edynamics-0.3.9/src/edynamics/modelling_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 04:24:28.863399 edynamics-0.3.9/src/edynamics/modelling_tools/embeddings/
+-rw-rw-rw-   0        0        0     4490 2023-03-17 20:15:12.000000 edynamics-0.3.9/src/edynamics/modelling_tools/embeddings/Embedding.py
+-rw-rw-rw-   0        0        0       34 2023-02-19 16:15:33.000000 edynamics-0.3.9/src/edynamics/modelling_tools/embeddings/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 04:24:28.871400 edynamics-0.3.9/src/edynamics/modelling_tools/estimators/
+-rw-rw-rw-   0        0        0       84 2023-02-19 16:17:02.000000 edynamics-0.3.9/src/edynamics/modelling_tools/estimators/__init__.py
+-rw-rw-rw-   0        0        0     4129 2023-02-27 19:58:36.000000 edynamics-0.3.9/src/edynamics/modelling_tools/estimators/cross_mapping.py
+-rw-rw-rw-   0        0        0     5132 2023-03-02 02:13:49.000000 edynamics-0.3.9/src/edynamics/modelling_tools/estimators/dimensionality.py
+-rw-rw-rw-   0        0        0     4769 2023-03-02 02:15:23.000000 edynamics-0.3.9/src/edynamics/modelling_tools/estimators/nonlinearity.py
+drwxrwxrwx   0        0        0        0 2023-04-16 04:24:28.876397 edynamics-0.3.9/src/edynamics/modelling_tools/norms/
+-rw-rw-rw-   0        0        0       34 2023-02-19 16:17:02.000000 edynamics-0.3.9/src/edynamics/modelling_tools/norms/__init__.py
+-rw-rw-rw-   0        0        0     1362 2023-02-27 23:56:00.000000 edynamics-0.3.9/src/edynamics/modelling_tools/norms/minkowski.py
+-rw-rw-rw-   0        0        0      972 2023-02-21 00:35:30.000000 edynamics-0.3.9/src/edynamics/modelling_tools/norms/norm.py
+drwxrwxrwx   0        0        0        0 2023-04-16 04:24:28.880396 edynamics-0.3.9/src/edynamics/modelling_tools/observers/
+-rw-rw-rw-   0        0        0       80 2023-03-02 23:14:00.000000 edynamics-0.3.9/src/edynamics/modelling_tools/observers/__init__.py
+-rw-rw-rw-   0        0        0      686 2023-04-06 20:43:38.000000 edynamics-0.3.9/src/edynamics/modelling_tools/observers/observer.py
+-rw-rw-rw-   0        0        0     2912 2023-04-12 21:38:18.000000 edynamics-0.3.9/src/edynamics/modelling_tools/observers/observers.py
+drwxrwxrwx   0        0        0        0 2023-04-16 04:24:28.882398 edynamics-0.3.9/src/edynamics/modelling_tools/optimizers/
+-rw-rw-rw-   0        0        0      100 2023-04-06 22:53:12.000000 edynamics-0.3.9/src/edynamics/modelling_tools/optimizers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 04:24:28.886399 edynamics-0.3.9/src/edynamics/modelling_tools/optimizers/cross_entropy/
+-rw-rw-rw-   0        0        0        0 2023-04-12 22:24:35.000000 edynamics-0.3.9/src/edynamics/modelling_tools/optimizers/cross_entropy/__init__.py
+-rw-rw-rw-   0        0        0     2121 2023-04-16 00:44:12.000000 edynamics-0.3.9/src/edynamics/modelling_tools/optimizers/cross_entropy/cem_optimizer.py
+drwxrwxrwx   0        0        0        0 2023-04-16 04:24:28.890398 edynamics-0.3.9/src/edynamics/modelling_tools/optimizers/gnn_optimizer/
+-rw-rw-rw-   0        0        0       42 2023-03-17 20:14:34.000000 edynamics-0.3.9/src/edynamics/modelling_tools/optimizers/gnn_optimizer/__init__.py
+-rw-rw-rw-   0        0        0     5967 2023-04-12 18:33:50.000000 edynamics-0.3.9/src/edynamics/modelling_tools/optimizers/gnn_optimizer/gnn_optimizer.py
+drwxrwxrwx   0        0        0        0 2023-04-16 04:24:28.902397 edynamics-0.3.9/src/edynamics/modelling_tools/optimizers/monte_carlo_search_tree/
+-rw-rw-rw-   0        0        0       24 2023-04-07 00:04:15.000000 edynamics-0.3.9/src/edynamics/modelling_tools/optimizers/monte_carlo_search_tree/__init__.py
+-rw-rw-rw-   0        0        0     2361 2023-04-12 21:52:31.000000 edynamics-0.3.9/src/edynamics/modelling_tools/optimizers/monte_carlo_search_tree/mcst.py
+-rw-rw-rw-   0        0        0      900 2023-03-19 23:39:32.000000 edynamics-0.3.9/src/edynamics/modelling_tools/optimizers/monte_carlo_search_tree/mcst_tree.py
+-rw-rw-rw-   0        0        0      473 2023-04-06 19:13:38.000000 edynamics-0.3.9/src/edynamics/modelling_tools/optimizers/monte_carlo_search_tree/node.py
+-rw-rw-rw-   0        0        0      557 2023-04-06 22:57:18.000000 edynamics-0.3.9/src/edynamics/modelling_tools/optimizers/monte_carlo_search_tree/oberver_node.py
+-rw-rw-rw-   0        0        0      553 2023-04-06 23:47:48.000000 edynamics-0.3.9/src/edynamics/modelling_tools/optimizers/monte_carlo_search_tree/observer_node.py
+drwxrwxrwx   0        0        0        0 2023-04-16 04:24:28.908400 edynamics-0.3.9/src/edynamics/modelling_tools/projectors/
+-rw-rw-rw-   0        0        0       80 2023-02-19 16:17:02.000000 edynamics-0.3.9/src/edynamics/modelling_tools/projectors/__init__.py
+-rw-rw-rw-   0        0        0     3203 2023-02-27 22:38:30.000000 edynamics-0.3.9/src/edynamics/modelling_tools/projectors/knn.py
+-rw-rw-rw-   0        0        0     4371 2023-03-15 04:27:02.000000 edynamics-0.3.9/src/edynamics/modelling_tools/projectors/projector.py
+-rw-rw-rw-   0        0        0     5952 2023-03-01 18:40:58.000000 edynamics-0.3.9/src/edynamics/modelling_tools/projectors/smap.py
+drwxrwxrwx   0        0        0        0 2023-04-16 04:24:28.919400 edynamics-0.3.9/src/edynamics/modelling_tools/weighers/
+-rw-rw-rw-   0        0        0      172 2023-02-19 16:17:02.000000 edynamics-0.3.9/src/edynamics/modelling_tools/weighers/__init__.py
+-rw-rw-rw-   0        0        0      262 2023-02-20 20:28:17.000000 edynamics-0.3.9/src/edynamics/modelling_tools/weighers/constant.py
+-rw-rw-rw-   0        0        0      497 2023-02-20 20:28:34.000000 edynamics-0.3.9/src/edynamics/modelling_tools/weighers/epanechnikov.py
+-rw-rw-rw-   0        0        0      888 2023-02-27 03:22:10.000000 edynamics-0.3.9/src/edynamics/modelling_tools/weighers/exponential.py
+-rw-rw-rw-   0        0        0      402 2023-02-20 20:29:07.000000 edynamics-0.3.9/src/edynamics/modelling_tools/weighers/tricubic.py
+-rw-rw-rw-   0        0        0      272 2023-02-20 20:27:35.000000 edynamics-0.3.9/src/edynamics/modelling_tools/weighers/weigher.py
+drwxrwxrwx   0        0        0        0 2023-04-16 04:24:28.924396 edynamics-0.3.9/src/edynamics/utils/
+-rw-rw-rw-   0        0        0     1544 2023-02-17 18:24:54.000000 edynamics-0.3.9/src/edynamics/utils/ProgressBar.py
+-rw-rw-rw-   0        0        0     1281 2023-02-17 18:24:54.000000 edynamics-0.3.9/src/edynamics/utils/ProgressBarActor.py
+-rw-rw-rw-   0        0        0        0 2023-02-16 20:30:29.000000 edynamics-0.3.9/src/edynamics/utils/__init__.py
```

### Comparing `edynamics-0.1.3/setup.py` & `edynamics-0.3.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
+REQUIREMENTS = [i.strip() for i in open("requirements.txt").readlines()]
 
 # Setting up
 setup(
     name="edynamics",
-    version='0.1.3',
+    version='0.3.9',
     author="Patrick Mahon",
     author_email="<pmahon3@uwo.ca>",
-    description='Empirical dynamic modelling',
+    description='Empirical dynamic modelling - modular, parallel, object-oriented',
     packages=find_packages(),
-    install_requires=['numpy', 'pandas', 'scipy', 'scikit-learn'],
+    install_requires=REQUIREMENTS,
     keywords=['python', 'edm', 'time series', 'forecasting', 'empirical dynamics'],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
     package_dir={'edynamics': 'src'})
```

