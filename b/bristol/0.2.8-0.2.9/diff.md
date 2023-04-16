# Comparing `tmp/bristol-0.2.8.tar.gz` & `tmp/bristol-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bristol-0.2.8.tar", last modified: Sat Sep  4 10:33:30 2021, max compression
+gzip compressed data, was "dist/bristol-0.2.9.tar", last modified: Sat Sep  4 11:00:44 2021, max compression
```

## Comparing `bristol-0.2.8.tar` & `bristol-0.2.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 msuzen     (501) staff       (20)        0 2021-09-04 10:33:30.000000 bristol-0.2.8/
--rw-r--r--   0 msuzen     (501) staff       (20)    35141 2021-08-22 13:28:47.000000 bristol-0.2.8/LICENSE
--rw-r--r--   0 msuzen     (501) staff       (20)       49 2021-08-22 13:28:47.000000 bristol-0.2.8/MANIFEST.in
--rw-r--r--   0 msuzen     (501) staff       (20)     5708 2021-09-04 10:33:30.000000 bristol-0.2.8/PKG-INFO
--rw-r--r--   0 msuzen     (501) staff       (20)       56 2021-08-22 13:28:47.000000 bristol-0.2.8/README
--rw-r--r--   0 msuzen     (501) staff       (20)     4304 2021-09-04 10:21:14.000000 bristol-0.2.8/README.md
-drwxr-xr-x   0 msuzen     (501) staff       (20)        0 2021-09-04 10:33:30.000000 bristol-0.2.8/bristol/
--rw-r--r--   0 msuzen     (501) staff       (20)      137 2021-08-22 13:28:47.000000 bristol-0.2.8/bristol/__init__.py
--rw-r--r--   0 msuzen     (501) staff       (20)     4306 2021-08-22 13:29:52.000000 bristol-0.2.8/bristol/cPSE.py
--rw-r--r--   0 msuzen     (501) staff       (20)     3632 2021-09-04 10:19:05.000000 bristol-0.2.8/bristol/data.py
--rw-r--r--   0 msuzen     (501) staff       (20)    12714 2021-09-04 10:19:15.000000 bristol-0.2.8/bristol/ensembles.py
--rw-r--r--   0 msuzen     (501) staff       (20)     9817 2021-09-04 10:19:23.000000 bristol-0.2.8/bristol/spectral.py
--rw-r--r--   0 msuzen     (501) staff       (20)      611 2021-08-22 13:32:56.000000 bristol-0.2.8/bristol/stats.py
--rw-r--r--   0 msuzen     (501) staff       (20)       20 2021-09-04 10:15:52.000000 bristol-0.2.8/bristol/version.py
-drwxr-xr-x   0 msuzen     (501) staff       (20)        0 2021-09-04 10:33:30.000000 bristol-0.2.8/bristol.egg-info/
--rw-r--r--   0 msuzen     (501) staff       (20)     5708 2021-09-04 10:33:30.000000 bristol-0.2.8/bristol.egg-info/PKG-INFO
--rw-r--r--   0 msuzen     (501) staff       (20)      746 2021-09-04 10:33:30.000000 bristol-0.2.8/bristol.egg-info/SOURCES.txt
--rw-r--r--   0 msuzen     (501) staff       (20)        1 2021-09-04 10:33:30.000000 bristol-0.2.8/bristol.egg-info/dependency_links.txt
--rw-r--r--   0 msuzen     (501) staff       (20)        1 2021-09-04 10:33:30.000000 bristol-0.2.8/bristol.egg-info/not-zip-safe
--rw-r--r--   0 msuzen     (501) staff       (20)       54 2021-09-04 10:33:30.000000 bristol-0.2.8/bristol.egg-info/requires.txt
--rw-r--r--   0 msuzen     (501) staff       (20)        8 2021-09-04 10:33:30.000000 bristol-0.2.8/bristol.egg-info/top_level.txt
--rw-r--r--   0 msuzen     (501) staff       (20)       38 2021-09-04 10:33:30.000000 bristol-0.2.8/setup.cfg
--rw-r--r--   0 msuzen     (501) staff       (20)     1103 2021-09-04 10:33:14.000000 bristol-0.2.8/setup.py
-drwxr-xr-x   0 msuzen     (501) staff       (20)        0 2021-09-04 10:33:30.000000 bristol-0.2.8/test/
--rw-r--r--   0 msuzen     (501) staff       (20)     2411 2021-08-22 13:28:47.000000 bristol-0.2.8/test/test_approach_se.py
--rw-r--r--   0 msuzen     (501) staff       (20)      633 2021-08-22 13:28:47.000000 bristol-0.2.8/test/test_cPSE_vgg11.py
--rw-r--r--   0 msuzen     (501) staff       (20)      815 2021-08-22 13:28:47.000000 bristol-0.2.8/test/test_eigen_circular.py
--rw-r--r--   0 msuzen     (501) staff       (20)     4771 2021-08-22 13:28:47.000000 bristol-0.2.8/test/test_eigen_circular_ensemble.py
--rw-r--r--   0 msuzen     (501) staff       (20)      575 2021-08-22 13:28:47.000000 bristol-0.2.8/test/test_gen_coe.py
--rw-r--r--   0 msuzen     (501) staff       (20)     1093 2021-08-22 13:28:47.000000 bristol-0.2.8/test/test_gen_cse.py
--rw-r--r--   0 msuzen     (501) staff       (20)      587 2021-08-22 13:28:47.000000 bristol-0.2.8/test/test_gen_cue.py
--rw-r--r--   0 msuzen     (501) staff       (20)      514 2021-08-22 13:28:47.000000 bristol-0.2.8/test/test_kl_distance_symmetric.py
--rw-r--r--   0 msuzen     (501) staff       (20)     3306 2021-08-22 13:28:47.000000 bristol-0.2.8/test/test_n_eigen_circular.py
--rw-r--r--   0 msuzen     (501) staff       (20)     3579 2021-08-22 13:28:47.000000 bristol-0.2.8/test/test_n_eigen_circular2.py
--rw-r--r--   0 msuzen     (501) staff       (20)      905 2021-08-22 13:28:47.000000 bristol-0.2.8/test/test_spectral_density.py
--rw-r--r--   0 msuzen     (501) staff       (20)     1435 2021-08-22 13:28:47.000000 bristol-0.2.8/test/test_thirumalai_mountain.py
--rw-r--r--   0 msuzen     (501) staff       (20)      791 2021-08-22 13:28:47.000000 bristol-0.2.8/test/test_unit_anti.py
--rw-r--r--   0 msuzen     (501) staff       (20)      788 2021-08-22 13:28:47.000000 bristol-0.2.8/test/test_unit_symplectic.py
+drwxr-xr-x   0 msuzen     (501) staff       (20)        0 2021-09-04 11:00:44.000000 bristol-0.2.9/
+-rw-r--r--   0 msuzen     (501) staff       (20)    35141 2021-08-22 13:28:47.000000 bristol-0.2.9/LICENSE
+-rw-r--r--   0 msuzen     (501) staff       (20)       49 2021-08-22 13:28:47.000000 bristol-0.2.9/MANIFEST.in
+-rw-r--r--   0 msuzen     (501) staff       (20)     6228 2021-09-04 11:00:44.000000 bristol-0.2.9/PKG-INFO
+-rw-r--r--   0 msuzen     (501) staff       (20)       56 2021-08-22 13:28:47.000000 bristol-0.2.9/README
+-rw-r--r--   0 msuzen     (501) staff       (20)     4792 2021-09-04 10:58:44.000000 bristol-0.2.9/README.md
+drwxr-xr-x   0 msuzen     (501) staff       (20)        0 2021-09-04 11:00:44.000000 bristol-0.2.9/bristol/
+-rw-r--r--   0 msuzen     (501) staff       (20)      137 2021-08-22 13:28:47.000000 bristol-0.2.9/bristol/__init__.py
+-rw-r--r--   0 msuzen     (501) staff       (20)     4306 2021-08-22 13:29:52.000000 bristol-0.2.9/bristol/cPSE.py
+-rw-r--r--   0 msuzen     (501) staff       (20)     3632 2021-09-04 10:19:05.000000 bristol-0.2.9/bristol/data.py
+-rw-r--r--   0 msuzen     (501) staff       (20)    12714 2021-09-04 10:19:15.000000 bristol-0.2.9/bristol/ensembles.py
+-rw-r--r--   0 msuzen     (501) staff       (20)     9817 2021-09-04 10:19:23.000000 bristol-0.2.9/bristol/spectral.py
+-rw-r--r--   0 msuzen     (501) staff       (20)      611 2021-08-22 13:32:56.000000 bristol-0.2.9/bristol/stats.py
+-rw-r--r--   0 msuzen     (501) staff       (20)       20 2021-09-04 10:57:01.000000 bristol-0.2.9/bristol/version.py
+drwxr-xr-x   0 msuzen     (501) staff       (20)        0 2021-09-04 11:00:44.000000 bristol-0.2.9/bristol.egg-info/
+-rw-r--r--   0 msuzen     (501) staff       (20)     6228 2021-09-04 11:00:44.000000 bristol-0.2.9/bristol.egg-info/PKG-INFO
+-rw-r--r--   0 msuzen     (501) staff       (20)      746 2021-09-04 11:00:44.000000 bristol-0.2.9/bristol.egg-info/SOURCES.txt
+-rw-r--r--   0 msuzen     (501) staff       (20)        1 2021-09-04 11:00:44.000000 bristol-0.2.9/bristol.egg-info/dependency_links.txt
+-rw-r--r--   0 msuzen     (501) staff       (20)        1 2021-09-04 10:33:30.000000 bristol-0.2.9/bristol.egg-info/not-zip-safe
+-rw-r--r--   0 msuzen     (501) staff       (20)       54 2021-09-04 11:00:44.000000 bristol-0.2.9/bristol.egg-info/requires.txt
+-rw-r--r--   0 msuzen     (501) staff       (20)        8 2021-09-04 11:00:44.000000 bristol-0.2.9/bristol.egg-info/top_level.txt
+-rw-r--r--   0 msuzen     (501) staff       (20)       38 2021-09-04 11:00:44.000000 bristol-0.2.9/setup.cfg
+-rw-r--r--   0 msuzen     (501) staff       (20)     1103 2021-09-04 10:33:14.000000 bristol-0.2.9/setup.py
+drwxr-xr-x   0 msuzen     (501) staff       (20)        0 2021-09-04 11:00:44.000000 bristol-0.2.9/test/
+-rw-r--r--   0 msuzen     (501) staff       (20)     2411 2021-08-22 13:28:47.000000 bristol-0.2.9/test/test_approach_se.py
+-rw-r--r--   0 msuzen     (501) staff       (20)      633 2021-08-22 13:28:47.000000 bristol-0.2.9/test/test_cPSE_vgg11.py
+-rw-r--r--   0 msuzen     (501) staff       (20)      815 2021-08-22 13:28:47.000000 bristol-0.2.9/test/test_eigen_circular.py
+-rw-r--r--   0 msuzen     (501) staff       (20)     4771 2021-08-22 13:28:47.000000 bristol-0.2.9/test/test_eigen_circular_ensemble.py
+-rw-r--r--   0 msuzen     (501) staff       (20)      575 2021-08-22 13:28:47.000000 bristol-0.2.9/test/test_gen_coe.py
+-rw-r--r--   0 msuzen     (501) staff       (20)     1093 2021-08-22 13:28:47.000000 bristol-0.2.9/test/test_gen_cse.py
+-rw-r--r--   0 msuzen     (501) staff       (20)      587 2021-08-22 13:28:47.000000 bristol-0.2.9/test/test_gen_cue.py
+-rw-r--r--   0 msuzen     (501) staff       (20)      514 2021-08-22 13:28:47.000000 bristol-0.2.9/test/test_kl_distance_symmetric.py
+-rw-r--r--   0 msuzen     (501) staff       (20)     3306 2021-08-22 13:28:47.000000 bristol-0.2.9/test/test_n_eigen_circular.py
+-rw-r--r--   0 msuzen     (501) staff       (20)     3579 2021-08-22 13:28:47.000000 bristol-0.2.9/test/test_n_eigen_circular2.py
+-rw-r--r--   0 msuzen     (501) staff       (20)      905 2021-08-22 13:28:47.000000 bristol-0.2.9/test/test_spectral_density.py
+-rw-r--r--   0 msuzen     (501) staff       (20)     1435 2021-08-22 13:28:47.000000 bristol-0.2.9/test/test_thirumalai_mountain.py
+-rw-r--r--   0 msuzen     (501) staff       (20)      791 2021-08-22 13:28:47.000000 bristol-0.2.9/test/test_unit_anti.py
+-rw-r--r--   0 msuzen     (501) staff       (20)      788 2021-08-22 13:28:47.000000 bristol-0.2.9/test/test_unit_symplectic.py
```

### Comparing `bristol-0.2.8/LICENSE` & `bristol-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/PKG-INFO` & `bristol-0.2.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: bristol
-Version: 0.2.8
+Version: 0.2.9
 Summary: Parallel random matrix tools and random matrix theory deep learning applications. Generate matrices from Circular Unitary Ensemble (CUE), Circular Ortogonal Ensemble (COE) and Circular Symplectic Ensemble (CSE). Additional spectral analysis utilities are also implemented, such as computation of spectral density and spectral ergodicity for complexity of deep learning architectures.
 Home-page: https://github.com/msuzen/bristol
 Author: M.Suzen
 Author-email: suzen@acm.org
 License: GPL-3
 Description: # Bristol
         
         [![Build Status](https://travis-ci.com/msuzen/bristol.svg?branch=master)](https://travis-ci.com/msuzen/bristol) 
         [![Coverage Status](https://coveralls.io/repos/github/msuzen/bristol/badge.svg?branch=master)](https://coveralls.io/github/msuzen/bristol?branch=master) 
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.579642.svg)](https://doi.org/10.5281/zenodo.579642)
         [![PyPI version](https://img.shields.io/pypi/v/bristol.svg?maxAge=2591000)](https://pypi.org/project/bristol/)
         [![Downloads](http://pepy.tech/badge/bristol)](https://pepy.tech/project/bristol)
         [![Downloads](https://pepy.tech/badge/bristol/month)](https://pepy.tech/project/bristol)
+        [![arXiv:1704.08303](http://img.shields.io/badge/arXiv-1704.08303-B31B1B.svg)](https://arxiv.org/abs/1704.08303)
+        [![Zenodo:Archive:v0.1.8](https://zenodo.org/badge/DOI/10.5281/zenodo.579642.svg)](https://doi.org/10.5281/zenodo.579642)
+        [![Zenodo:Surrogate Matrices Data](https://zenodo.org/badge/DOI/10.5281/zenodo.822411.svg)](https://doi.org/10.5281/zenodo.822411)
+        [![arXiv:1911.07831](http://img.shields.io/badge/arXiv-1911.07831-B31B1B.svg)](https://arxiv.org/abs/1911.07831)
+        [![arXiv:2006.13687](http://img.shields.io/badge/arXiv-2006.13687-B31B1B.svg)](https://arxiv.org/abs/2006.13687)
         
         Parallel random matrix tools and random matrix theory deep learning applications. 
         Generate matrices from Circular Unitary Ensemble (CUE), Circular Ortogonal Ensemble (COE) and 
         Circular Symplectic Ensemble (CSE). Additional spectral analysis utilities are 
         also implemented, such as computation of spectral density and spectral ergodicity 
         for complexity of deep learning architectures.
```

### Comparing `bristol-0.2.8/README.md` & `bristol-0.2.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 # Bristol
 
 [![Build Status](https://travis-ci.com/msuzen/bristol.svg?branch=master)](https://travis-ci.com/msuzen/bristol) 
 [![Coverage Status](https://coveralls.io/repos/github/msuzen/bristol/badge.svg?branch=master)](https://coveralls.io/github/msuzen/bristol?branch=master) 
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.579642.svg)](https://doi.org/10.5281/zenodo.579642)
 [![PyPI version](https://img.shields.io/pypi/v/bristol.svg?maxAge=2591000)](https://pypi.org/project/bristol/)
 [![Downloads](http://pepy.tech/badge/bristol)](https://pepy.tech/project/bristol)
 [![Downloads](https://pepy.tech/badge/bristol/month)](https://pepy.tech/project/bristol)
+[![arXiv:1704.08303](http://img.shields.io/badge/arXiv-1704.08303-B31B1B.svg)](https://arxiv.org/abs/1704.08303)
+[![Zenodo:Archive:v0.1.8](https://zenodo.org/badge/DOI/10.5281/zenodo.579642.svg)](https://doi.org/10.5281/zenodo.579642)
+[![Zenodo:Surrogate Matrices Data](https://zenodo.org/badge/DOI/10.5281/zenodo.822411.svg)](https://doi.org/10.5281/zenodo.822411)
+[![arXiv:1911.07831](http://img.shields.io/badge/arXiv-1911.07831-B31B1B.svg)](https://arxiv.org/abs/1911.07831)
+[![arXiv:2006.13687](http://img.shields.io/badge/arXiv-2006.13687-B31B1B.svg)](https://arxiv.org/abs/2006.13687)
 
 Parallel random matrix tools and random matrix theory deep learning applications. 
 Generate matrices from Circular Unitary Ensemble (CUE), Circular Ortogonal Ensemble (COE) and 
 Circular Symplectic Ensemble (CSE). Additional spectral analysis utilities are 
 also implemented, such as computation of spectral density and spectral ergodicity 
 for complexity of deep learning architectures.
```

### Comparing `bristol-0.2.8/bristol/cPSE.py` & `bristol-0.2.9/bristol/cPSE.py`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/bristol/data.py` & `bristol-0.2.9/bristol/data.py`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/bristol/ensembles.py` & `bristol-0.2.9/bristol/ensembles.py`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/bristol/spectral.py` & `bristol-0.2.9/bristol/spectral.py`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/bristol/stats.py` & `bristol-0.2.9/bristol/stats.py`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/bristol.egg-info/PKG-INFO` & `bristol-0.2.9/bristol.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: bristol
-Version: 0.2.8
+Version: 0.2.9
 Summary: Parallel random matrix tools and random matrix theory deep learning applications. Generate matrices from Circular Unitary Ensemble (CUE), Circular Ortogonal Ensemble (COE) and Circular Symplectic Ensemble (CSE). Additional spectral analysis utilities are also implemented, such as computation of spectral density and spectral ergodicity for complexity of deep learning architectures.
 Home-page: https://github.com/msuzen/bristol
 Author: M.Suzen
 Author-email: suzen@acm.org
 License: GPL-3
 Description: # Bristol
         
         [![Build Status](https://travis-ci.com/msuzen/bristol.svg?branch=master)](https://travis-ci.com/msuzen/bristol) 
         [![Coverage Status](https://coveralls.io/repos/github/msuzen/bristol/badge.svg?branch=master)](https://coveralls.io/github/msuzen/bristol?branch=master) 
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.579642.svg)](https://doi.org/10.5281/zenodo.579642)
         [![PyPI version](https://img.shields.io/pypi/v/bristol.svg?maxAge=2591000)](https://pypi.org/project/bristol/)
         [![Downloads](http://pepy.tech/badge/bristol)](https://pepy.tech/project/bristol)
         [![Downloads](https://pepy.tech/badge/bristol/month)](https://pepy.tech/project/bristol)
+        [![arXiv:1704.08303](http://img.shields.io/badge/arXiv-1704.08303-B31B1B.svg)](https://arxiv.org/abs/1704.08303)
+        [![Zenodo:Archive:v0.1.8](https://zenodo.org/badge/DOI/10.5281/zenodo.579642.svg)](https://doi.org/10.5281/zenodo.579642)
+        [![Zenodo:Surrogate Matrices Data](https://zenodo.org/badge/DOI/10.5281/zenodo.822411.svg)](https://doi.org/10.5281/zenodo.822411)
+        [![arXiv:1911.07831](http://img.shields.io/badge/arXiv-1911.07831-B31B1B.svg)](https://arxiv.org/abs/1911.07831)
+        [![arXiv:2006.13687](http://img.shields.io/badge/arXiv-2006.13687-B31B1B.svg)](https://arxiv.org/abs/2006.13687)
         
         Parallel random matrix tools and random matrix theory deep learning applications. 
         Generate matrices from Circular Unitary Ensemble (CUE), Circular Ortogonal Ensemble (COE) and 
         Circular Symplectic Ensemble (CSE). Additional spectral analysis utilities are 
         also implemented, such as computation of spectral density and spectral ergodicity 
         for complexity of deep learning architectures.
```

### Comparing `bristol-0.2.8/bristol.egg-info/SOURCES.txt` & `bristol-0.2.9/bristol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/setup.py` & `bristol-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/test/test_approach_se.py` & `bristol-0.2.9/test/test_approach_se.py`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/test/test_cPSE_vgg11.py` & `bristol-0.2.9/test/test_cPSE_vgg11.py`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/test/test_eigen_circular.py` & `bristol-0.2.9/test/test_eigen_circular.py`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/test/test_eigen_circular_ensemble.py` & `bristol-0.2.9/test/test_eigen_circular_ensemble.py`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/test/test_gen_coe.py` & `bristol-0.2.9/test/test_gen_coe.py`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/test/test_gen_cse.py` & `bristol-0.2.9/test/test_gen_cse.py`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/test/test_gen_cue.py` & `bristol-0.2.9/test/test_gen_cue.py`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/test/test_kl_distance_symmetric.py` & `bristol-0.2.9/test/test_kl_distance_symmetric.py`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/test/test_n_eigen_circular.py` & `bristol-0.2.9/test/test_n_eigen_circular.py`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/test/test_n_eigen_circular2.py` & `bristol-0.2.9/test/test_n_eigen_circular2.py`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/test/test_spectral_density.py` & `bristol-0.2.9/test/test_spectral_density.py`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/test/test_thirumalai_mountain.py` & `bristol-0.2.9/test/test_thirumalai_mountain.py`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/test/test_unit_anti.py` & `bristol-0.2.9/test/test_unit_anti.py`

 * *Files identical despite different names*

### Comparing `bristol-0.2.8/test/test_unit_symplectic.py` & `bristol-0.2.9/test/test_unit_symplectic.py`

 * *Files identical despite different names*

