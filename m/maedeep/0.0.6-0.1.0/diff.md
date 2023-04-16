# Comparing `tmp/maedeep-0.0.6.tar.gz` & `tmp/maedeep-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maedeep-0.0.6.tar", last modified: Mon Apr  3 10:39:28 2023, max compression
+gzip compressed data, was "maedeep-0.1.0.tar", last modified: Sun Apr 16 09:34:21 2023, max compression
```

## Comparing `maedeep-0.0.6.tar` & `maedeep-0.1.0.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 10:39:28.112161 maedeep-0.0.6/
--rw-rw-rw-   0        0        0      171 2022-09-27 08:31:09.000000 maedeep-0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0      353 2023-04-03 10:39:28.112620 maedeep-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2227 2022-09-27 08:31:09.000000 maedeep-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 10:39:28.054258 maedeep-0.0.6/maedeep/
--rw-rw-rw-   0        0        0      517 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/__init__.py
--rw-rw-rw-   0        0        0     2664 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/_areafunction.py
--rw-rw-rw-   0        0        0      511 2022-10-04 09:06:04.000000 maedeep-0.0.6/maedeep/_config.py
--rw-rw-rw-   0        0        0     5512 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/_contour.py
--rw-rw-rw-   0        0        0     3788 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/_set.py
--rw-rw-rw-   0        0        0    11088 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/_waveguide.py
-drwxrwxrwx   0        0        0        0 2023-04-03 10:39:28.062690 maedeep-0.0.6/maedeep/data/
--rw-rw-rw-   0        0        0   486296 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/data/data_vowels.h5
-drwxrwxrwx   0        0        0        0 2023-04-03 10:39:28.072003 maedeep-0.0.6/maedeep/dnn/
--rw-rw-rw-   0        0        0      434 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/dnn/__init__.py
--rw-rw-rw-   0        0        0     5396 2023-02-08 16:36:23.000000 maedeep-0.0.6/maedeep/dnn/_forwardmapping.py
--rw-rw-rw-   0        0        0     5095 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/dnn/_inversemapping.py
--rw-rw-rw-   0        0        0      548 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/dnn/costs.py
--rw-rw-rw-   0        0        0    11030 2023-02-08 16:39:17.000000 maedeep-0.0.6/maedeep/dnn/dnntools.py
-drwxrwxrwx   0        0        0        0 2023-04-03 10:39:28.097791 maedeep-0.0.6/maedeep/dnn/models/
--rw-rw-rw-   0        0        0   132441 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/dnn/models/acoustic_to_articulator.h5
--rw-rw-rw-   0        0        0   647341 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/dnn/models/articulator_to_acoustic.h5
--rw-rw-rw-   0        0        0   286393 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/dnn/models/articulator_to_area.h5
--rw-rw-rw-   0        0        0   266528 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/dnn/models/articulator_to_contour.h5
--rw-rw-rw-   0        0        0   136129 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/dnn/models/articulator_to_task.h5
--rw-rw-rw-   0        0        0   222488 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/dnn/models/contour_to_acoustic.h5
--rw-rw-rw-   0        0        0   315584 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/dnn/models/contour_to_area.h5
--rw-rw-rw-   0        0        0   225888 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/dnn/models/contour_to_articulatory.h5
--rw-rw-rw-   0        0        0   225908 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/dnn/models/contour_to_task.h5
--rw-rw-rw-   0        0        0   132521 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/dnn/models/task_to_acoustic.h5
--rw-rw-rw-   0        0        0     4255 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/dnn/optimizationtools.py
--rw-rw-rw-   0        0        0      917 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/gmmtools.py
-drwxrwxrwx   0        0        0        0 2023-04-03 10:39:28.101516 maedeep-0.0.6/maedeep/linear/
--rw-rw-rw-   0        0        0      452 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/linear/__init__.py
--rw-rw-rw-   0        0        0      588 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/linear/_forwardmapping.py
-drwxrwxrwx   0        0        0        0 2023-04-03 10:39:28.103091 maedeep-0.0.6/maedeep/linear/models/
--rw-rw-rw-   0        0        0     2300 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/linear/models/linear_model.h5
--rw-rw-rw-   0        0        0     1254 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/linear/modeltools.py
-drwxrwxrwx   0        0        0        0 2023-04-03 10:39:28.108481 maedeep-0.0.6/maedeep/parametric/
--rw-rw-rw-   0        0        0      452 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/parametric/__init__.py
--rw-rw-rw-   0        0        0     3405 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/parametric/_forwardmapping.py
-drwxrwxrwx   0        0        0        0 2023-04-03 10:39:28.110780 maedeep-0.0.6/maedeep/parametric/models/
--rw-rw-rw-   0        0        0    24115 2022-09-27 08:31:09.000000 maedeep-0.0.6/maedeep/parametric/models/model_spec.json
--rw-rw-rw-   0        0        0     7507 2022-10-04 09:04:26.000000 maedeep-0.0.6/maedeep/parametric/modeltools.py
--rw-rw-rw-   0        0        0     6646 2023-03-16 11:34:21.000000 maedeep-0.0.6/maedeep/signaltools.py
-drwxrwxrwx   0        0        0        0 2023-04-03 10:39:28.061907 maedeep-0.0.6/maedeep.egg-info/
--rw-rw-rw-   0        0        0      353 2023-04-03 10:39:27.000000 maedeep-0.0.6/maedeep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1277 2023-04-03 10:39:27.000000 maedeep-0.0.6/maedeep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 10:39:27.000000 maedeep-0.0.6/maedeep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-10-04 08:44:26.000000 maedeep-0.0.6/maedeep.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       62 2023-04-03 10:39:27.000000 maedeep-0.0.6/maedeep.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-03 10:39:27.000000 maedeep-0.0.6/maedeep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-03 10:39:28.113361 maedeep-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      887 2023-04-03 10:37:18.000000 maedeep-0.0.6/setup.py
+drwxrwxrwx   0 benjamin  (1000) benjamin  (1000)        0 2023-04-16 09:34:21.271717 maedeep-0.1.0/
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)      171 2022-09-27 08:31:09.000000 maedeep-0.1.0/LICENSE.txt
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)      340 2023-04-16 09:34:21.271717 maedeep-0.1.0/PKG-INFO
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)     2245 2023-04-13 11:51:26.000000 maedeep-0.1.0/README.md
+drwxrwxrwx   0 benjamin  (1000) benjamin  (1000)        0 2023-04-16 09:34:20.848337 maedeep-0.1.0/maedeep/
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)      517 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/__init__.py
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)     2664 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/_areafunction.py
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)      511 2022-10-04 09:06:04.000000 maedeep-0.1.0/maedeep/_config.py
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)     5512 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/_contour.py
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)     3788 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/_set.py
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)    11088 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/_waveguide.py
+drwxrwxrwx   0 benjamin  (1000) benjamin  (1000)        0 2023-04-16 09:34:20.905123 maedeep-0.1.0/maedeep/data/
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)   486296 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/data/data_vowels.h5
+drwxrwxrwx   0 benjamin  (1000) benjamin  (1000)        0 2023-04-16 09:34:20.977256 maedeep-0.1.0/maedeep/dnn/
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)      434 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/dnn/__init__.py
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)     6216 2023-04-14 12:34:51.000000 maedeep-0.1.0/maedeep/dnn/_forwardmapping.py
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)     5819 2023-04-14 12:45:32.000000 maedeep-0.1.0/maedeep/dnn/_inversemapping.py
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)      548 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/dnn/costs.py
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)    12286 2023-04-14 12:30:30.000000 maedeep-0.1.0/maedeep/dnn/dnntools.py
+drwxrwxrwx   0 benjamin  (1000) benjamin  (1000)        0 2023-04-16 09:34:21.173347 maedeep-0.1.0/maedeep/dnn/models/
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)   132441 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/dnn/models/acoustic_to_articulator.h5
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)   248064 2023-04-04 14:28:11.000000 maedeep-0.1.0/maedeep/dnn/models/acoustic_to_articulatory_and_task.h5
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)   647341 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/dnn/models/articulator_to_acoustic.h5
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)   249560 2023-04-04 00:02:44.000000 maedeep-0.1.0/maedeep/dnn/models/articulator_to_acoustic_and_task.h5
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)   286393 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/dnn/models/articulator_to_area.h5
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)   266528 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/dnn/models/articulator_to_contour.h5
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)   136129 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/dnn/models/articulator_to_task.h5
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)   222488 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/dnn/models/contour_to_acoustic.h5
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)   315584 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/dnn/models/contour_to_area.h5
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)   225888 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/dnn/models/contour_to_articulatory.h5
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)   225908 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/dnn/models/contour_to_task.h5
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)   132521 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/dnn/models/task_to_acoustic.h5
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)     4255 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/dnn/optimizationtools.py
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)      917 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/gmmtools.py
+drwxrwxrwx   0 benjamin  (1000) benjamin  (1000)        0 2023-04-16 09:34:21.207001 maedeep-0.1.0/maedeep/linear/
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)      452 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/linear/__init__.py
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)      588 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/linear/_forwardmapping.py
+drwxrwxrwx   0 benjamin  (1000) benjamin  (1000)        0 2023-04-16 09:34:21.218510 maedeep-0.1.0/maedeep/linear/models/
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)     2300 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/linear/models/linear_model.h5
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)     1254 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/linear/modeltools.py
+drwxrwxrwx   0 benjamin  (1000) benjamin  (1000)        0 2023-04-16 09:34:21.247292 maedeep-0.1.0/maedeep/parametric/
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)      452 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/parametric/__init__.py
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)     3405 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/parametric/_forwardmapping.py
+drwxrwxrwx   0 benjamin  (1000) benjamin  (1000)        0 2023-04-16 09:34:21.262529 maedeep-0.1.0/maedeep/parametric/models/
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)    24115 2022-09-27 08:31:09.000000 maedeep-0.1.0/maedeep/parametric/models/model_spec.json
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)     7507 2022-10-04 09:04:26.000000 maedeep-0.1.0/maedeep/parametric/modeltools.py
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)     6730 2023-04-14 12:47:28.000000 maedeep-0.1.0/maedeep/signaltools.py
+drwxrwxrwx   0 benjamin  (1000) benjamin  (1000)        0 2023-04-16 09:34:20.893273 maedeep-0.1.0/maedeep.egg-info/
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)      340 2023-04-16 09:34:20.000000 maedeep-0.1.0/maedeep.egg-info/PKG-INFO
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)     1388 2023-04-16 09:34:20.000000 maedeep-0.1.0/maedeep.egg-info/SOURCES.txt
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)        1 2023-04-16 09:34:20.000000 maedeep-0.1.0/maedeep.egg-info/dependency_links.txt
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)        2 2022-10-04 08:44:26.000000 maedeep-0.1.0/maedeep.egg-info/not-zip-safe
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)       62 2023-04-16 09:34:20.000000 maedeep-0.1.0/maedeep.egg-info/requires.txt
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)        8 2023-04-16 09:34:20.000000 maedeep-0.1.0/maedeep.egg-info/top_level.txt
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)       79 2023-04-16 09:34:21.277192 maedeep-0.1.0/setup.cfg
+-rwxrwxrwx   0 benjamin  (1000) benjamin  (1000)      887 2023-04-16 09:32:08.000000 maedeep-0.1.0/setup.py
```

### Comparing `maedeep-0.0.6/README.md` & `maedeep-0.1.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 # Maedeep
 
 ## Presentation
 
-Maedeep is a python interface to use the articulatory model by Maeda. It allows forward and inverse mapping between the following spaces:
+Maedeep is a python interface for using the articulatory model by Maeda. It allows forward and inverse mapping between the following spaces:
 * Articulatory parameters
 * Contours
 * Area function
 * Task variables
 * Transfer function
 * Formants
 
-Inverse mapping is performed using a DNN model trained on simulated data. The code to compute contour sand area functions is derived from VTsynth toolbox by Satrajit Ghosh [1].
+Inverse mapping is performed using a DNN model trained on simulated data. The code to compute contours and area functions is derived from the VTsynth toolbox by Satrajit Ghosh [1].
 
 ## Installation
 
 Maedeep is implemented with Python3. Tests have been performed with Python 3.9, so consider having a version of Python that is at least as new as Python 3.9.
 
 Please also consider using a Python3 virtual environment during the development stage:
 ```bash
 # create a python 3 virtual environment and activate it
 $ python3 -m venv maedeep_env
 $ source maedeep_env/bin/activate
 ```
 
-You can get the source codes by cloning this repo with git
+Maedeep is on PyPI, so you can directly install it with
+```bash
+# install planart locally in editable mode
+$ pip install maedeep
 ```
-git clone https://git.ecdf.ed.ac.uk/belie/maedeep.git
 
+Alternatively, you can get the source codes by cloning this repo with git
 ```
+git clone https://git.ecdf.ed.ac.uk/belie/maedeep.git
 
-PlanArt is not yet on PyPI. You can install it locally in editable mode:
+```
+and install it locally in editable mode:
 ```bash
 # install planart locally in editable mode
 $ python3 -m pip install -e path_to_maedeep
 ```
 
-* WARNING: Please, do not modify anything in the planart folder, unless you want to modify the repository.
-
 ## Checking the software behavior
 To check if everything runs as expected, run the following command:
 ```bash
 # test if everything works as expected
 $ cd path_to_maedeep
 $ pytest tests
 ```
```

### Comparing `maedeep-0.0.6/maedeep/__init__.py` & `maedeep-0.1.0/maedeep/__init__.py`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/_areafunction.py` & `maedeep-0.1.0/maedeep/_areafunction.py`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/_contour.py` & `maedeep-0.1.0/maedeep/_contour.py`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/_set.py` & `maedeep-0.1.0/maedeep/_set.py`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/_waveguide.py` & `maedeep-0.1.0/maedeep/_waveguide.py`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/data/data_vowels.h5` & `maedeep-0.1.0/maedeep/data/data_vowels.h5`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/dnn/_forwardmapping.py` & `maedeep-0.1.0/maedeep/dnn/_forwardmapping.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,44 +4,64 @@
 Created on Mon May 23 16:04:55 2022
 
 @author: benjamin
 """
 
 import h5py
 import numpy as np
-from .dnntools import (check_input_area, dnn_mapping, load_mapping_model, 
-                       normalization_model, output_area, output_contour, 
-                       reshape_input)
+from .dnntools import (
+                        check_input_area,
+                        dnn_joint_mapping,
+                        dnn_mapping,
+                        load_mapping_model,
+                        normalization_model,
+                        output_area,
+                        output_contour,
+                        reshape_input
+                       )
 
 def area_to_formant(areas, model_directory=None, model=None, norms=None):
     areas = check_input_area(areas)
     return dnn_mapping(areas, model_directory=model_directory,
-                       input_space="area", output_space="acoustic", 
+                       input_space="area", output_space="acoustic",
                        model=model, norms=norms)
 
-def articulatory_to_formant(articulatory_parameters, model_directory=None, 
-                            model=None, norms=None):
-    return dnn_mapping(articulatory_parameters, model_directory=model_directory,
-                       input_space="articulator", output_space="acoustic", 
+def articulatory_to_formant(articulatory_parameters, model_directory=None,
+                            model=None, norms=None, joint=True):
+    if joint:
+        return dnn_joint_mapping(articulatory_parameters, 
+                                 input_space="articulator",
+                                 output_spaces=("acoustic", "task"),
+                                 model=model, model_directory=model_directory)[0]
+    else:
+        return dnn_mapping(articulatory_parameters,
+                           model_directory=model_directory,
+                       input_space="articulator", output_space="acoustic",
                        model=model, norms=norms)
 
-def articulatory_to_area(articulatory_parameters, model_directory=None, 
+def articulatory_to_area(articulatory_parameters, model_directory=None,
                          model=None, norms=None, output_type="raw"):
-    
+
     areas = dnn_mapping(articulatory_parameters, model_directory=model_directory,
-                       input_space="articulator", output_space="area", 
+                       input_space="articulator", output_space="area",
                        model=model, norms=norms)
     return output_area(areas, output_type)
-        
+
 
 def articulatory_to_task(articulatory_parameters, model_directory=None,
-                         model=None, norms=None):
-    return dnn_mapping(articulatory_parameters, model_directory=model_directory,
-                       input_space="articulator", output_space="task", 
-                       model=model, norms=norms)
+                         model=None, norms=None, joint=True):
+    if joint:
+        return dnn_joint_mapping(articulatory_parameters, 
+                                 input_space="articulator",
+                                 output_spaces=("acoustic", "task"),
+                                 model=model, model_directory=model_directory)[1]
+    else:
+        return dnn_mapping(articulatory_parameters, model_directory=model_directory,
+                           input_space="articulator", output_space="task",
+                           model=model, norms=norms)
 
 def articulatory_to_contour(articulatory_parameters, model_directory=None,
                             output_type="raw", model=None, norms=None):
 
     model, model_file = load_mapping_model(model_directory, "articulator",
                                      "contour")
     with h5py.File(model_file, "r") as hf:
@@ -52,15 +72,15 @@
         my_full = hf["full_mean"][()]
     nb_feat = model.get_config()["layers"][0]["config"]["batch_input_shape"][1]
     x = normalization_model(reshape_input(articulatory_parameters, nb_feat), norms_input, 0)
     predicted_contours = np.zeros((x.shape[0], my_full.shape[1]))
     predicted_contours[:, idx_var] = normalization_model(model.predict(x, verbose=0), norms_output, 1)
     predicted_contours[:, idx_invar] = np.repeat(my_full[:, idx_invar].reshape(1, -1),
                                                  x.shape[0], axis=0)
-    
+
     return output_contour(predicted_contours, output_type)
 
 def contour_to_area(contours, model_directory=None, output_type="raw",
                     model=None, norms=None):
 
     model, model_file = load_mapping_model(model_directory, "contour",
                                      "acoustic")
@@ -105,15 +125,15 @@
         idx_var = hf["variance_index"][()]
     x = np.array([contour.contours for contour in contours])
     x = normalization_model(x[:, idx_var], norms_input, 0)
     return normalization_model(model.predict(x, verbose=0), norms_output, 1)
 
 def task_to_formant(task, model_directory=None, model=None, norms=None):
     return dnn_mapping(task, model_directory=model_directory,
-                       input_space="task", output_space="acoustic", 
+                       input_space="task", output_space="acoustic",
                        model=model, norms=norms)
```

### Comparing `maedeep-0.0.6/maedeep/dnn/_inversemapping.py` & `maedeep-0.1.0/maedeep/dnn/_inversemapping.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,27 +4,40 @@
 Created on Mon May 23 16:04:55 2022
 
 @author: benjamin
 """
 
 import h5py
 import numpy as np
-from .dnntools import (check_input_area, dnn_mapping, load_mapping_model, 
-                       normalization_model, output_area, output_contour, 
-                       reshape_input)
+from .dnntools import (
+                        check_input_area, 
+                        dnn_joint_mapping, 
+                        dnn_mapping, 
+                        load_mapping_model, 
+                        normalization_model,
+                        output_area, 
+                        output_contour, 
+                        reshape_input
+                       )
 from maedeep.signaltools import vtln
 
 def acoustic_to_area(formants, model_directory=None, output_type="raw"):
     areas = dnn_mapping(vtln(formants), model_directory=model_directory,
                        input_space="acoustic", output_space="area")
 
     return output_area(areas, output_type)
 
-def acoustic_to_articulatory(formants, model_directory=None):
-    return dnn_mapping(vtln(formants), model_directory=model_directory,
+def acoustic_to_articulatory(formants, model_directory=None, joint=True):
+    if joint:
+        return dnn_joint_mapping(vtln(formants), input_space="acoustic",
+                                 output_spaces=("articulatory", "task"),
+                                 model_directory=model_directory)[0]
+        
+    else: 
+        return dnn_mapping(vtln(formants), model_directory=model_directory,
                        input_space="acoustic", output_space="articulator")
 
 def area_to_articulatory(areas, model_directory=None, 
                          output_type="raw"):
     return dnn_mapping(check_input_area(areas), model_directory=model_directory,
                        input_space="area", output_space="articulator")
         
@@ -99,17 +112,22 @@
     x = normalization_model(reshape_input(tasks, nb_feat), norms_input, 0)
     predicted_contours = np.zeros((x.shape[0], my_full.shape[1]))
     predicted_contours[:, idx_var] = normalization_model(model.predict(x, verbose=0), norms_output, 1)
     predicted_contours[:, idx_invar] = np.repeat(my_full[:, idx_invar].reshape(1, -1),
                                                  x.shape[0], axis=0)
     return output_contour(predicted_contours, output_type)
 
-def acoustic_to_task(formants, model_directory=None):
-    return dnn_mapping(formants, model_directory=model_directory,
-                       input_space="acoustic", output_space="task")
+def acoustic_to_task(formants, model_directory=None, joint=True):
+    if joint:
+        return dnn_joint_mapping(vtln(formants), input_space="acoustic",
+                                 output_spaces=("articulatory", "task"),
+                                 model_directory=model_directory)[1]
+    else:
+        return dnn_mapping(vtln(formants), model_directory=model_directory,
+                           input_space="acoustic", output_space="task")
```

### Comparing `maedeep-0.0.6/maedeep/dnn/costs.py` & `maedeep-0.1.0/maedeep/dnn/costs.py`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/dnn/dnntools.py` & `maedeep-0.1.0/maedeep/dnn/dnntools.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # tf.compat.v1.disable_eager_execution()
 import h5py
 import numpy as np
 from tqdm import tqdm
 from maedeep._config import get_maedeep_path
 from maedeep._areafunction import AreaFunction
 from maedeep._contour import Contour
+import pickle
 import warnings
 
 def build_model(input_layer_size, hidden_layer_size,
                 encoding_function="relu",
                 decoding_function="relu",
                 sparsity=0,
                 loss="mean_squared_error"):
@@ -81,15 +82,25 @@
         return area
 
 def concat_data(x, y):
     if x is None:
         return y
     else:
         return np.hstack((x, y))
-    
+  
+def dnn_joint_mapping(x, input_space, output_spaces, model_directory=None, 
+                model=None):
+    if model is None:
+        model, scaler = load_mapping_joint_model(model_directory, input_space,
+                                   output_spaces)
+    nb_feat = model.get_config()["layers"][0]["config"]["batch_input_shape"][1]
+    x = scaler[0].transform(reshape_input(x, nb_feat))
+    y = model.predict(x, verbose=False)
+    return [scaler[n+1].inverse_transform(y[n]) for n in range(len(y))]
+
 def dnn_mapping(x, input_space, output_space, model_directory=None, 
                 model=None, norms=None):
     
     if model is None:
         model, model_file = load_mapping_model(model_directory, input_space,
                                    output_space)
     nb_feat = model.get_config()["layers"][0]["config"]["batch_input_shape"][1]
@@ -109,21 +120,37 @@
     with h5py.File(file, "r") as hf:
         data = [hf[key][()] for key in keys]
     return data
 
 def load_model(file):
     return models.load_model(file)
 
+def load_mapping_joint_model(model_directory, input_space, output_spaces):
+    if model_directory is None:
+        model_directory = os.path.join(get_maedeep_path(), "dnn", "models")
+    model_prefix = "_".join([input_space, "to", output_spaces[0], "and", 
+                             output_spaces[1]])
+    model_file = os.path.join(model_directory, model_prefix + ".h5")
+    scaler_file = os.path.join(model_directory, model_prefix + ".scl")
+    
+    return load_model(model_file), load_scaler_file(scaler_file)
+
 def load_mapping_model(model_directory, input_space, output_space):
     if model_directory is None:
         model_directory = os.path.join(get_maedeep_path(), "dnn", "models")
     file = os.path.join(model_directory, 
                         input_space + "_to_" + output_space + ".h5")
+    scaler_file = os.path.join(model_directory, 
+                        input_space + "_to_" + output_space + ".scl")
     return load_model(file), file
 
+def load_scaler_file(scaler_file):
+    with open(scaler_file, 'rb') as f:
+        return pickle.load(f)
+
 def make_data_notrain(training_path, input_vars="articulators", 
               output_vars="tract", disable=False):
 
     list_files = [os.path.join(training_path, x) for x in os.listdir(training_path)
                   if ".h5" in x]
     x_train = None
     y_train = None
```

### Comparing `maedeep-0.0.6/maedeep/dnn/models/acoustic_to_articulator.h5` & `maedeep-0.1.0/maedeep/dnn/models/acoustic_to_articulator.h5`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/dnn/models/articulator_to_acoustic.h5` & `maedeep-0.1.0/maedeep/dnn/models/articulator_to_acoustic.h5`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/dnn/models/articulator_to_area.h5` & `maedeep-0.1.0/maedeep/dnn/models/articulator_to_area.h5`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/dnn/models/articulator_to_contour.h5` & `maedeep-0.1.0/maedeep/dnn/models/articulator_to_contour.h5`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/dnn/models/articulator_to_task.h5` & `maedeep-0.1.0/maedeep/dnn/models/articulator_to_task.h5`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/dnn/models/contour_to_acoustic.h5` & `maedeep-0.1.0/maedeep/dnn/models/contour_to_acoustic.h5`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/dnn/models/contour_to_area.h5` & `maedeep-0.1.0/maedeep/dnn/models/contour_to_area.h5`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/dnn/models/contour_to_articulatory.h5` & `maedeep-0.1.0/maedeep/dnn/models/contour_to_articulatory.h5`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/dnn/models/contour_to_task.h5` & `maedeep-0.1.0/maedeep/dnn/models/contour_to_task.h5`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/dnn/models/task_to_acoustic.h5` & `maedeep-0.1.0/maedeep/dnn/models/task_to_acoustic.h5`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/dnn/optimizationtools.py` & `maedeep-0.1.0/maedeep/dnn/optimizationtools.py`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/gmmtools.py` & `maedeep-0.1.0/maedeep/gmmtools.py`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/linear/_forwardmapping.py` & `maedeep-0.1.0/maedeep/linear/_forwardmapping.py`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/linear/models/linear_model.h5` & `maedeep-0.1.0/maedeep/linear/models/linear_model.h5`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/linear/modeltools.py` & `maedeep-0.1.0/maedeep/linear/modeltools.py`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/parametric/_forwardmapping.py` & `maedeep-0.1.0/maedeep/parametric/_forwardmapping.py`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/parametric/models/model_spec.json` & `maedeep-0.1.0/maedeep/parametric/models/model_spec.json`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/parametric/modeltools.py` & `maedeep-0.1.0/maedeep/parametric/modeltools.py`

 * *Files identical despite different names*

### Comparing `maedeep-0.0.6/maedeep/signaltools.py` & `maedeep-0.1.0/maedeep/signaltools.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,16 @@
      
     sum_freq = 0
     for i, row in enumerate(freq.T):
         for F_ij in row:
             sum_freq += F_ij / (i + 0.5)
     return c * freq.size / (2*sum_freq)
 
-def vtln(freq, speaker_length=None, target_length=0.16273747, c=343):
+def vtln(freq, speaker_length=None, target_length=0.16273747, c=343):    
     
+    if isinstance(freq, list):
+        freq = np.array(freq).reshape(1, -1)    
     if freq.shape[1] != 4 and freq.shape[0] == 4:
         freq = freq.T
     if speaker_length is None:
         speaker_length = vtl_estimation(freq)
     return (freq * speaker_length / target_length).T
```

### Comparing `maedeep-0.0.6/maedeep.egg-info/SOURCES.txt` & `maedeep-0.1.0/maedeep.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 maedeep/dnn/__init__.py
 maedeep/dnn/_forwardmapping.py
 maedeep/dnn/_inversemapping.py
 maedeep/dnn/costs.py
 maedeep/dnn/dnntools.py
 maedeep/dnn/optimizationtools.py
 maedeep/dnn/models/acoustic_to_articulator.h5
+maedeep/dnn/models/acoustic_to_articulatory_and_task.h5
 maedeep/dnn/models/articulator_to_acoustic.h5
+maedeep/dnn/models/articulator_to_acoustic_and_task.h5
 maedeep/dnn/models/articulator_to_area.h5
 maedeep/dnn/models/articulator_to_contour.h5
 maedeep/dnn/models/articulator_to_task.h5
 maedeep/dnn/models/contour_to_acoustic.h5
 maedeep/dnn/models/contour_to_area.h5
 maedeep/dnn/models/contour_to_articulatory.h5
 maedeep/dnn/models/contour_to_task.h5
```

### Comparing `maedeep-0.0.6/setup.py` & `maedeep-0.1.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 @author: benjamin
 """
 
 from setuptools import setup, find_packages
 
 setup(name='maedeep',
-      version='0.0.6',
+      version='0.1.0',
         description='Python interface to use articulatory model by Maeda',
         url='https://git.ecdf.ed.ac.uk/belie/maedeep',
         author='Benjamin Elie',
         author_email='benjamin.elie@ed.ac.uk',
         license='Creative Commons Attribution 4.0 International License',
       packages=find_packages(),
       install_requires=[
```

