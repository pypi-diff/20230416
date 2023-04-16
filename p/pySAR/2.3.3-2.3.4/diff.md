# Comparing `tmp/pySAR-2.3.3.tar.gz` & `tmp/pySAR-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pySAR-2.3.3.tar", last modified: Tue Apr  4 22:37:18 2023, max compression
+gzip compressed data, was "pySAR-2.3.4.tar", last modified: Sun Apr 16 16:09:59 2023, max compression
```

## Comparing `pySAR-2.3.3.tar` & `pySAR-2.3.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:37:18.518969 pySAR-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-04 22:36:48.000000 pySAR-2.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    32252 2023-04-04 22:37:18.518969 pySAR-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26394 2023-04-04 22:36:48.000000 pySAR-2.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:37:18.518969 pySAR-2.3.3/pySAR/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-04 22:36:48.000000 pySAR-2.3.3/pySAR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    69115 2023-04-04 22:36:48.000000 pySAR-2.3.3/pySAR/descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)    39736 2023-04-04 22:36:48.000000 pySAR-2.3.3/pySAR/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-04-04 22:36:48.000000 pySAR-2.3.3/pySAR/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-04 22:36:48.000000 pySAR-2.3.3/pySAR/globals_.py
--rw-r--r--   0 runner    (1001) docker     (123)    24388 2023-04-04 22:36:48.000000 pySAR-2.3.3/pySAR/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-04 22:36:48.000000 pySAR-2.3.3/pySAR/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    26006 2023-04-04 22:36:48.000000 pySAR-2.3.3/pySAR/pyDSP.py
--rw-r--r--   0 runner    (1001) docker     (123)    37066 2023-04-04 22:36:48.000000 pySAR-2.3.3/pySAR/pySAR.py
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-04-04 22:36:48.000000 pySAR-2.3.3/pySAR/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:37:18.518969 pySAR-2.3.3/pySAR.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    32252 2023-04-04 22:37:18.000000 pySAR-2.3.3/pySAR.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-04 22:37:18.000000 pySAR-2.3.3/pySAR.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 22:37:18.000000 pySAR-2.3.3/pySAR.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 22:37:17.000000 pySAR-2.3.3/pySAR.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-04 22:37:18.000000 pySAR-2.3.3/pySAR.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-04 22:37:18.000000 pySAR-2.3.3/pySAR.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-04 22:37:18.522969 pySAR-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-04 22:36:48.000000 pySAR-2.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:59.433853 pySAR-2.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-16 16:09:24.000000 pySAR-2.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    32069 2023-04-16 16:09:59.433853 pySAR-2.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    26243 2023-04-16 16:09:24.000000 pySAR-2.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:59.429853 pySAR-2.3.4/pySAR/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-16 16:09:24.000000 pySAR-2.3.4/pySAR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69115 2023-04-16 16:09:24.000000 pySAR-2.3.4/pySAR/descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39791 2023-04-16 16:09:24.000000 pySAR-2.3.4/pySAR/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-04-16 16:09:24.000000 pySAR-2.3.4/pySAR/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-16 16:09:24.000000 pySAR-2.3.4/pySAR/globals_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24388 2023-04-16 16:09:24.000000 pySAR-2.3.4/pySAR/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-16 16:09:24.000000 pySAR-2.3.4/pySAR/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26006 2023-04-16 16:09:24.000000 pySAR-2.3.4/pySAR/pyDSP.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37066 2023-04-16 16:09:24.000000 pySAR-2.3.4/pySAR/pySAR.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-04-16 16:09:24.000000 pySAR-2.3.4/pySAR/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:09:59.433853 pySAR-2.3.4/pySAR.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    32069 2023-04-16 16:09:59.000000 pySAR-2.3.4/pySAR.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-16 16:09:59.000000 pySAR-2.3.4/pySAR.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:09:59.000000 pySAR-2.3.4/pySAR.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:09:58.000000 pySAR-2.3.4/pySAR.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-16 16:09:59.000000 pySAR-2.3.4/pySAR.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 16:09:59.000000 pySAR-2.3.4/pySAR.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-16 16:09:59.433853 pySAR-2.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-04-16 16:09:24.000000 pySAR-2.3.4/setup.py
```

### Comparing `pySAR-2.3.3/LICENSE` & `pySAR-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pySAR-2.3.3/PKG-INFO` & `pySAR-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySAR
-Version: 2.3.3
+Version: 2.3.4
 Summary: A Python package used to analysis Sequence Activity Relationships (SARs) of protein sequences and their mutants using Machine Learning.
 Home-page: https://github.com/amckenna41/pySAR
 Author: MIT
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/pySAR/archive/refs/heads/main.zip
@@ -106,15 +106,14 @@
                 "algorithm": "plsregression",
                 "parameters": "",
                 "test_split": 0.2
               },
             "descriptors":
                 {
                   "descriptors_csv": "descriptors.csv",
-                  "all_desc": 0,
                   "moreaubroto_autocorrelation":
                     {
                     "lag":30,
                     "properties":["CIDH920105", "BHAR880101", "CHAM820101", "CHAM820102",
                       "CHOC760101", "BIGC670101", "CHAM810101", "DAYM780201"],
                     "normalize": 1
                     },
@@ -219,15 +218,15 @@
         |  1 | ROBB760107 | secondary_struct  | 0.666527 | 3.19801 | 10.2273  | 1.73169 | 2.50305 |        0.668255 |
         |  2 | RICJ880102 | secondary_struct  | 0.568067 | 3.83976 | 14.7438  | 1.52157 | 3.01342 |        0.568274 |
         |  3 | KARS160113 | meta        | 0.544129 | 4.04266 | 16.3431  | 1.48108 | 3.26047 |        0.544693 |
         
         </details>
         
         <details><summary><b>Encoding protein sequences using their calculated protein descriptors:</summary></b><br>
-        Calculate the protein descriptor values for a dataset of protein sequences from the 15 available descriptors in the <em>descriptors</em> module. Use each descriptor as a feature set in the building of the predictive models used to predict the activity value of unseen sequences. By default, the function will look for a csv file pointed to by the <em>"descriptors_csv"</em> parameter in the config file that contains the pre-calculated descriptor values for a dataset. If file is not found then all descriptor values will be calculated for the dataset using the <em>descriptors_</em> module. If a descriptor in the config file is to be used in the feature data, its parameter is set to true/1. If <em>all_desc</em> is set to true/1 then all available descriptors are calculated using their respective functions.<br>
+        Calculate the protein descriptor values for a dataset of protein sequences from the 15 available descriptors in the <em>descriptors</em> module. Use each descriptor as a feature set in the building of the predictive models used to predict the activity value of unseen sequences. By default, the function will look for a csv file pointed to by the <em>"descriptors_csv"</em> parameter in the config file that contains the pre-calculated descriptor values for a dataset. If file is not found then all descriptor values will be calculated for the dataset using the <em>descriptors_</em> module. If a descriptor in the config file is to be used in the feature data, its parameter is set to true/1.<br>
         
         ```python
         from pySAR.encoding import *
         
         '''test_config3.json
         {
           "dataset": 
@@ -243,15 +242,14 @@
               "estimators": 100,
               "learning_rate": 1.5
               ...
             },
           "descriptors": 
           {
             "descriptors_csv": "precalculated_descriptors.csv",
-            "all_desc": 0,
             "moreaubroto_autocorrelation": {
               "lag": 30,
               "properties": ["CIDH920105", "BHAR880101", "CHAM820101", "CHAM820102",
                 "CHOC760101", "BIGC670101", "CHAM810101", "DAYM780201"],
               "normalize": 1
             },
             ...
@@ -299,15 +297,14 @@
               "learning_rate": 1.5,
               ...
               }
           },
           "descriptors": 
           {
             "descriptors_csv": "precalculated_descriptors.csv",
-            "all_desc": 0,
             "moreaubroto_autocorrelation": {
               "lag": 30,
               "properties": ["CIDH920105", "BHAR880101", "CHAM820101", "CHAM820102",
                 "CHOC760101", "BIGC670101", "CHAM810101", "DAYM780201"],
               "normalize": 1
             },
             ...
@@ -359,15 +356,14 @@
             "algorithm": "plsregression",
             "parameters": "",
             ...
           },
           "descriptors": 
           {
             "descriptors_csv": "precalculated_descriptors.csv",
-            "all_desc": 0,
             "moreaubroto_autocorrelation": {
               "lag": 30,
               "properties": ["CIDH920105", "BHAR880101", "CHAM820101", "CHAM820102",
                 "CHOC760101", "BIGC670101", "CHAM810101", "DAYM780201"],
               "normalize": 1
             },
             ...
@@ -522,15 +518,15 @@
         [tqdm]: https://tqdm.github.io/
         [seaborn]: https://seaborn.pydata.org/
         [matplotlib]: https://matplotlib.org/
         [PyPi]: https://pypi.org/project/pysar/
         [article]: https://www.sciencedirect.com/science/article/abs/pii/S1532046422000326
         [pdf]: https://github.com/amckenna41/pySAR/blob/master/pySAR_research.pdf
         [ppt]: https://github.com/amckenna41/pySAR/blob/master/pySAR_demo.key
-        [demo]: https://github.com/amckenna41/pySAR/
+        [demo]: https://colab.research.google.com/drive/1hxtnf8i4q13fB1_2TpJFimS5qfZi9RAo?usp=sharing
         [Issues]: https://github.com/amckenna41/pySAR/issues
         
 Keywords: bioinformatics,protein engineering,python,pypi,machine learning,directed evolution,sequence activity relationships,SAR,aaindex,protein descriptors
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `pySAR-2.3.3/README.md` & `pySAR-2.3.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,14 @@
         "algorithm": "plsregression",
         "parameters": "",
         "test_split": 0.2
       },
     "descriptors":
         {
           "descriptors_csv": "descriptors.csv",
-          "all_desc": 0,
           "moreaubroto_autocorrelation":
             {
             "lag":30,
             "properties":["CIDH920105", "BHAR880101", "CHAM820101", "CHAM820102",
               "CHOC760101", "BIGC670101", "CHAM810101", "DAYM780201"],
             "normalize": 1
             },
@@ -209,15 +208,15 @@
 |  1 | ROBB760107 | secondary_struct  | 0.666527 | 3.19801 | 10.2273  | 1.73169 | 2.50305 |        0.668255 |
 |  2 | RICJ880102 | secondary_struct  | 0.568067 | 3.83976 | 14.7438  | 1.52157 | 3.01342 |        0.568274 |
 |  3 | KARS160113 | meta        | 0.544129 | 4.04266 | 16.3431  | 1.48108 | 3.26047 |        0.544693 |
 
 </details>
 
 <details><summary><b>Encoding protein sequences using their calculated protein descriptors:</summary></b><br>
-Calculate the protein descriptor values for a dataset of protein sequences from the 15 available descriptors in the <em>descriptors</em> module. Use each descriptor as a feature set in the building of the predictive models used to predict the activity value of unseen sequences. By default, the function will look for a csv file pointed to by the <em>"descriptors_csv"</em> parameter in the config file that contains the pre-calculated descriptor values for a dataset. If file is not found then all descriptor values will be calculated for the dataset using the <em>descriptors_</em> module. If a descriptor in the config file is to be used in the feature data, its parameter is set to true/1. If <em>all_desc</em> is set to true/1 then all available descriptors are calculated using their respective functions.<br>
+Calculate the protein descriptor values for a dataset of protein sequences from the 15 available descriptors in the <em>descriptors</em> module. Use each descriptor as a feature set in the building of the predictive models used to predict the activity value of unseen sequences. By default, the function will look for a csv file pointed to by the <em>"descriptors_csv"</em> parameter in the config file that contains the pre-calculated descriptor values for a dataset. If file is not found then all descriptor values will be calculated for the dataset using the <em>descriptors_</em> module. If a descriptor in the config file is to be used in the feature data, its parameter is set to true/1.<br>
 
 ```python
 from pySAR.encoding import *
 
 '''test_config3.json
 {
   "dataset": 
@@ -233,15 +232,14 @@
       "estimators": 100,
       "learning_rate": 1.5
       ...
     },
   "descriptors": 
   {
     "descriptors_csv": "precalculated_descriptors.csv",
-    "all_desc": 0,
     "moreaubroto_autocorrelation": {
       "lag": 30,
       "properties": ["CIDH920105", "BHAR880101", "CHAM820101", "CHAM820102",
         "CHOC760101", "BIGC670101", "CHAM810101", "DAYM780201"],
       "normalize": 1
     },
     ...
@@ -289,15 +287,14 @@
       "learning_rate": 1.5,
       ...
       }
   },
   "descriptors": 
   {
     "descriptors_csv": "precalculated_descriptors.csv",
-    "all_desc": 0,
     "moreaubroto_autocorrelation": {
       "lag": 30,
       "properties": ["CIDH920105", "BHAR880101", "CHAM820101", "CHAM820102",
         "CHOC760101", "BIGC670101", "CHAM810101", "DAYM780201"],
       "normalize": 1
     },
     ...
@@ -349,15 +346,14 @@
     "algorithm": "plsregression",
     "parameters": "",
     ...
   },
   "descriptors": 
   {
     "descriptors_csv": "precalculated_descriptors.csv",
-    "all_desc": 0,
     "moreaubroto_autocorrelation": {
       "lag": 30,
       "properties": ["CIDH920105", "BHAR880101", "CHAM820101", "CHAM820102",
         "CHOC760101", "BIGC670101", "CHAM810101", "DAYM780201"],
       "normalize": 1
     },
     ...
@@ -512,9 +508,9 @@
 [tqdm]: https://tqdm.github.io/
 [seaborn]: https://seaborn.pydata.org/
 [matplotlib]: https://matplotlib.org/
 [PyPi]: https://pypi.org/project/pysar/
 [article]: https://www.sciencedirect.com/science/article/abs/pii/S1532046422000326
 [pdf]: https://github.com/amckenna41/pySAR/blob/master/pySAR_research.pdf
 [ppt]: https://github.com/amckenna41/pySAR/blob/master/pySAR_demo.key
-[demo]: https://github.com/amckenna41/pySAR/
+[demo]: https://colab.research.google.com/drive/1hxtnf8i4q13fB1_2TpJFimS5qfZi9RAo?usp=sharing
 [Issues]: https://github.com/amckenna41/pySAR/issues
```

### Comparing `pySAR-2.3.3/pySAR/__init__.py` & `pySAR-2.3.4/pySAR/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ pySAR software metadata. """
 __name__ = 'pySAR'
-__version__ = "2.3.3"
+__version__ = "2.3.4"
 __description__ = 'A Python package used to analysis Sequence Activity Relationships (SARs) of protein sequences and their mutants using Machine Learning.'
 __author__ = 'AJ McKenna, https://github.com/amckenna41'
 __authorEmail__ = 'amckenna41@qub.ac.uk'
 __maintainer__ = "AJ McKenna"
 __license__ = 'MIT'
 __url__ = 'https://github.com/amckenna41/pySAR'
 __download_url__ = "https://github.com/amckenna41/pySAR/archive/refs/heads/main.zip"
```

### Comparing `pySAR-2.3.3/pySAR/descriptors.py` & `pySAR-2.3.4/pySAR/descriptors.py`

 * *Files identical despite different names*

### Comparing `pySAR-2.3.3/pySAR/encoding.py` & `pySAR-2.3.4/pySAR/encoding.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ################################################################################
 
 import pandas as pd
 import numpy as np
 import time
 import itertools
 import sys
-from tqdm.auto import tqdm
+from tqdm import tqdm
 from difflib import get_close_matches
 import json
 from textwrap import TextWrapper
 
 from aaindex import aaindex1
 from .model import Model
 from .pyDSP import PyDSP
@@ -174,15 +174,15 @@
         tqdm_disable = False
         if (len(all_indices)) <= 1:
             tqdm_disable = True
 
         #using tqdm package to create a progress bar showing encoding progress,
         #file=sys.stdout to stop error where iterations were printing out of order
         for index in tqdm(all_indices[:int(len(all_indices))], unit=" indices", position=0, 
-            desc="AAI Indices", file=sys.stdout, disable=tqdm_disable):
+            desc="AAI Indices", mininterval=30, disable=tqdm_disable):
 
             #get AAI indices encoding for sequences according to index var
             encoded_seqs = self.get_aai_encoding(index)
 
             #generate protein spectra from pyDSP class if use_dsp is true, set as training data
             if (self.use_dsp):
                 pyDSP = PyDSP(self.config_file, protein_seqs=encoded_seqs)
@@ -371,15 +371,15 @@
 
         #disable tqdm progress bar if only 1 descriptor being used
         tqdm_disable = False
         if (len(all_descriptors)) <= 1:
             tqdm_disable = True
 
         for descr in tqdm(all_descriptors[:int(len(all_descriptors))], unit=" descriptor", position=0, 
-            desc="Descriptors", file=sys.stdout, disable=tqdm_disable):
+            desc="Descriptors", mininterval=30, disable=tqdm_disable):
 
             #reset descriptor DF and list
             desc_ = pd.DataFrame()           
             descriptor_list = []
        
             #if using 2 or 3 descriptors, append each descriptor & its category to list
             if (desc_combo == 2 or desc_combo == 3):
@@ -632,15 +632,16 @@
         '''
 
         #disable tqdm progress bar if only 1 aa index being used
         tqdm_disable = False
         if (len(all_indices)) <= 1:
             tqdm_disable = True
         
-        for index in tqdm(all_indices[:int(len(all_indices))], unit=" indices", desc="AAI Indices", disable=tqdm_disable):
+        for index in tqdm(all_indices[:int(len(all_indices))], unit=" indices", desc="AAI Indices", 
+            mininterval=30, disable=tqdm_disable):
 
             #get AAI indices encoding for sequences according to index var
             encoded_seqs = self.get_aai_encoding(index)
 
             #generate protein spectra from pyDSP class if use_dsp is true
             if (self.use_dsp):
                 pyDSP = PyDSP(self.config_file, protein_seqs=encoded_seqs)
@@ -657,15 +658,16 @@
 
             #disable tqdm progress bar if only 1 descriptor being used
             tqdm_disable = False
             if (len(all_descriptors)) <= 1:
                 tqdm_disable = True
     
             #iterate through all descriptors
-            for descr in tqdm(all_descriptors, leave=False, unit=" descriptor", desc="Descriptors", disable=tqdm_disable):
+            for descr in tqdm(all_descriptors, leave=False, unit=" descriptor", desc="Descriptors", 
+                mininterval=30, disable=tqdm_disable):
 
                 #reset descriptor DF and list
                 desc_ = pd.DataFrame()
                 descriptor_list = []
 
                 #if using 2 or 3 descriptors, append each descriptor & its category to list
                 if (desc_combo == 2 or desc_combo == 3):
```

### Comparing `pySAR-2.3.3/pySAR/evaluate.py` & `pySAR-2.3.4/pySAR/evaluate.py`

 * *Files identical despite different names*

### Comparing `pySAR-2.3.3/pySAR/globals_.py` & `pySAR-2.3.4/pySAR/globals_.py`

 * *Files identical despite different names*

### Comparing `pySAR-2.3.3/pySAR/model.py` & `pySAR-2.3.4/pySAR/model.py`

 * *Files identical despite different names*

### Comparing `pySAR-2.3.3/pySAR/plots.py` & `pySAR-2.3.4/pySAR/plots.py`

 * *Files identical despite different names*

### Comparing `pySAR-2.3.3/pySAR/pyDSP.py` & `pySAR-2.3.4/pySAR/pyDSP.py`

 * *Files identical despite different names*

### Comparing `pySAR-2.3.3/pySAR/pySAR.py` & `pySAR-2.3.4/pySAR/pySAR.py`

 * *Files identical despite different names*

### Comparing `pySAR-2.3.3/pySAR/utils.py` & `pySAR-2.3.4/pySAR/utils.py`

 * *Files identical despite different names*

### Comparing `pySAR-2.3.3/pySAR.egg-info/PKG-INFO` & `pySAR-2.3.4/pySAR.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pySAR
-Version: 2.3.3
+Version: 2.3.4
 Summary: A Python package used to analysis Sequence Activity Relationships (SARs) of protein sequences and their mutants using Machine Learning.
 Home-page: https://github.com/amckenna41/pySAR
 Author: MIT
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/pySAR/archive/refs/heads/main.zip
@@ -106,15 +106,14 @@
                 "algorithm": "plsregression",
                 "parameters": "",
                 "test_split": 0.2
               },
             "descriptors":
                 {
                   "descriptors_csv": "descriptors.csv",
-                  "all_desc": 0,
                   "moreaubroto_autocorrelation":
                     {
                     "lag":30,
                     "properties":["CIDH920105", "BHAR880101", "CHAM820101", "CHAM820102",
                       "CHOC760101", "BIGC670101", "CHAM810101", "DAYM780201"],
                     "normalize": 1
                     },
@@ -219,15 +218,15 @@
         |  1 | ROBB760107 | secondary_struct  | 0.666527 | 3.19801 | 10.2273  | 1.73169 | 2.50305 |        0.668255 |
         |  2 | RICJ880102 | secondary_struct  | 0.568067 | 3.83976 | 14.7438  | 1.52157 | 3.01342 |        0.568274 |
         |  3 | KARS160113 | meta        | 0.544129 | 4.04266 | 16.3431  | 1.48108 | 3.26047 |        0.544693 |
         
         </details>
         
         <details><summary><b>Encoding protein sequences using their calculated protein descriptors:</summary></b><br>
-        Calculate the protein descriptor values for a dataset of protein sequences from the 15 available descriptors in the <em>descriptors</em> module. Use each descriptor as a feature set in the building of the predictive models used to predict the activity value of unseen sequences. By default, the function will look for a csv file pointed to by the <em>"descriptors_csv"</em> parameter in the config file that contains the pre-calculated descriptor values for a dataset. If file is not found then all descriptor values will be calculated for the dataset using the <em>descriptors_</em> module. If a descriptor in the config file is to be used in the feature data, its parameter is set to true/1. If <em>all_desc</em> is set to true/1 then all available descriptors are calculated using their respective functions.<br>
+        Calculate the protein descriptor values for a dataset of protein sequences from the 15 available descriptors in the <em>descriptors</em> module. Use each descriptor as a feature set in the building of the predictive models used to predict the activity value of unseen sequences. By default, the function will look for a csv file pointed to by the <em>"descriptors_csv"</em> parameter in the config file that contains the pre-calculated descriptor values for a dataset. If file is not found then all descriptor values will be calculated for the dataset using the <em>descriptors_</em> module. If a descriptor in the config file is to be used in the feature data, its parameter is set to true/1.<br>
         
         ```python
         from pySAR.encoding import *
         
         '''test_config3.json
         {
           "dataset": 
@@ -243,15 +242,14 @@
               "estimators": 100,
               "learning_rate": 1.5
               ...
             },
           "descriptors": 
           {
             "descriptors_csv": "precalculated_descriptors.csv",
-            "all_desc": 0,
             "moreaubroto_autocorrelation": {
               "lag": 30,
               "properties": ["CIDH920105", "BHAR880101", "CHAM820101", "CHAM820102",
                 "CHOC760101", "BIGC670101", "CHAM810101", "DAYM780201"],
               "normalize": 1
             },
             ...
@@ -299,15 +297,14 @@
               "learning_rate": 1.5,
               ...
               }
           },
           "descriptors": 
           {
             "descriptors_csv": "precalculated_descriptors.csv",
-            "all_desc": 0,
             "moreaubroto_autocorrelation": {
               "lag": 30,
               "properties": ["CIDH920105", "BHAR880101", "CHAM820101", "CHAM820102",
                 "CHOC760101", "BIGC670101", "CHAM810101", "DAYM780201"],
               "normalize": 1
             },
             ...
@@ -359,15 +356,14 @@
             "algorithm": "plsregression",
             "parameters": "",
             ...
           },
           "descriptors": 
           {
             "descriptors_csv": "precalculated_descriptors.csv",
-            "all_desc": 0,
             "moreaubroto_autocorrelation": {
               "lag": 30,
               "properties": ["CIDH920105", "BHAR880101", "CHAM820101", "CHAM820102",
                 "CHOC760101", "BIGC670101", "CHAM810101", "DAYM780201"],
               "normalize": 1
             },
             ...
@@ -522,15 +518,15 @@
         [tqdm]: https://tqdm.github.io/
         [seaborn]: https://seaborn.pydata.org/
         [matplotlib]: https://matplotlib.org/
         [PyPi]: https://pypi.org/project/pysar/
         [article]: https://www.sciencedirect.com/science/article/abs/pii/S1532046422000326
         [pdf]: https://github.com/amckenna41/pySAR/blob/master/pySAR_research.pdf
         [ppt]: https://github.com/amckenna41/pySAR/blob/master/pySAR_demo.key
-        [demo]: https://github.com/amckenna41/pySAR/
+        [demo]: https://colab.research.google.com/drive/1hxtnf8i4q13fB1_2TpJFimS5qfZi9RAo?usp=sharing
         [Issues]: https://github.com/amckenna41/pySAR/issues
         
 Keywords: bioinformatics,protein engineering,python,pypi,machine learning,directed evolution,sequence activity relationships,SAR,aaindex,protein descriptors
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `pySAR-2.3.3/setup.cfg` & `pySAR-2.3.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = PySAR
-version = 2.3.3
+version = 2.3.4
 description = Analysing Sequence Activity Relationships (SARs) of protein sequences and their mutants using Machine Learning.
 author = AJ McKenna
 author_email = amckenna41@qub.ac.uk
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/amckenna41/pySAR
 download_url = https://github.com/amckenna41/pySAR/archive/refs/heads/main.zip
```

### Comparing `pySAR-2.3.3/setup.py` & `pySAR-2.3.4/setup.py`

 * *Files identical despite different names*

