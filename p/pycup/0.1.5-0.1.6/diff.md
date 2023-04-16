# Comparing `tmp/pycup-0.1.5.tar.gz` & `tmp/pycup-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pycup-0.1.5.tar", last modified: Tue Apr  4 11:59:43 2023, max compression
+gzip compressed data, was "dist\pycup-0.1.6.tar", last modified: Sun Apr 16 14:48:12 2023, max compression
```

## Comparing `pycup-0.1.5.tar` & `pycup-0.1.6.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 11:59:43.102810 pycup-0.1.5/
--rw-rw-rw-   0        0        0     5683 2023-04-04 11:59:43.101810 pycup-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4453 2023-04-04 08:08:55.000000 pycup-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 11:59:43.083806 pycup-0.1.5/pycup/
--rw-rw-rw-   0        0        0    17161 2023-03-25 02:59:48.000000 pycup-0.1.5/pycup/GLUE.py
--rw-rw-rw-   0        0        0    38271 2023-04-04 06:40:04.000000 pycup-0.1.5/pycup/GWO.py
--rw-rw-rw-   0        0        0    33260 2023-04-04 06:40:04.000000 pycup-0.1.5/pycup/MFO.py
--rw-rw-rw-   0        0        0    14600 2023-04-04 06:40:04.000000 pycup-0.1.5/pycup/MODE.py
--rw-rw-rw-   0        0        0    24212 2023-04-04 06:52:09.000000 pycup-0.1.5/pycup/MOPSO.py
--rw-rw-rw-   0        0        0    14937 2023-04-04 06:52:09.000000 pycup-0.1.5/pycup/NSGA2.py
--rw-rw-rw-   0        0        0    35498 2023-04-04 07:27:43.000000 pycup-0.1.5/pycup/PSO.py
--rw-rw-rw-   0        0        0    15659 2023-03-25 02:59:48.000000 pycup-0.1.5/pycup/Reslib.py
--rw-rw-rw-   0        0        0    30073 2023-04-04 07:27:43.000000 pycup-0.1.5/pycup/SCA.py
--rw-rw-rw-   0        0        0    32941 2023-04-04 07:27:43.000000 pycup-0.1.5/pycup/SOA.py
--rw-rw-rw-   0        0        0    32160 2023-04-04 07:27:43.000000 pycup-0.1.5/pycup/SSA.py
--rw-rw-rw-   0        0        0     5757 2023-03-25 02:59:48.000000 pycup-0.1.5/pycup/TOPSIS.py
--rw-rw-rw-   0        0        0    33343 2023-04-04 07:27:43.000000 pycup-0.1.5/pycup/TSA.py
--rw-rw-rw-   0        0        0    32912 2023-04-04 07:27:43.000000 pycup-0.1.5/pycup/WOA.py
--rw-rw-rw-   0        0        0      892 2023-03-25 03:50:23.000000 pycup-0.1.5/pycup/__init__.py
--rw-rw-rw-   0        0        0    10042 2023-04-04 08:11:01.000000 pycup-0.1.5/pycup/calc_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-04 11:59:43.098809 pycup-0.1.5/pycup/document/
--rw-rw-rw-   0        0        0   826264 2023-04-04 11:58:19.000000 pycup-0.1.5/pycup/document/Documentation.pdf
--rw-rw-rw-   0        0        0     4027 2023-03-25 02:59:48.000000 pycup-0.1.5/pycup/evaluation_metrics.py
--rw-rw-rw-   0        0        0    16961 2023-03-25 03:50:23.000000 pycup-0.1.5/pycup/integrate.py
--rw-rw-rw-   0        0        0     7263 2023-03-25 02:59:48.000000 pycup-0.1.5/pycup/multi_jobs.py
--rw-rw-rw-   0        0        0   125408 2023-03-25 02:59:48.000000 pycup-0.1.5/pycup/plot.py
--rw-rw-rw-   0        0        0      460 2023-03-25 02:59:48.000000 pycup-0.1.5/pycup/progress_bar.py
--rw-rw-rw-   0        0        0    10352 2023-03-25 02:59:48.000000 pycup-0.1.5/pycup/sampling.py
--rw-rw-rw-   0        0        0    18935 2023-03-25 02:59:48.000000 pycup-0.1.5/pycup/save.py
--rw-rw-rw-   0        0        0     2068 2023-03-25 02:59:48.000000 pycup-0.1.5/pycup/template.py
--rw-rw-rw-   0        0        0        0 2023-03-25 02:59:48.000000 pycup-0.1.5/pycup/test.py
--rw-rw-rw-   0        0        0     6055 2023-03-25 02:59:48.000000 pycup-0.1.5/pycup/test_functions.py
--rw-rw-rw-   0        0        0    68801 2023-03-25 02:59:48.000000 pycup-0.1.5/pycup/uncertainty_analysis_fun.py
--rw-rw-rw-   0        0        0    17048 2023-03-25 02:59:48.000000 pycup-0.1.5/pycup/utilize.py
-drwxrwxrwx   0        0        0        0 2023-04-04 11:59:43.094809 pycup-0.1.5/pycup.egg-info/
--rw-rw-rw-   0        0        0     5683 2023-04-04 11:59:42.000000 pycup-0.1.5/pycup.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      669 2023-04-04 11:59:42.000000 pycup-0.1.5/pycup.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 11:59:42.000000 pycup-0.1.5/pycup.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-04 11:59:42.000000 pycup-0.1.5/pycup.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-04 11:59:42.000000 pycup-0.1.5/pycup.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-04 11:59:43.102810 pycup-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      939 2023-04-04 06:28:36.000000 pycup-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:48:12.380022 pycup-0.1.6/
+-rw-rw-rw-   0        0        0     6321 2023-04-16 14:48:12.379105 pycup-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5075 2023-04-16 08:17:22.000000 pycup-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 14:48:12.364019 pycup-0.1.6/pycup/
+-rw-rw-rw-   0        0        0    17161 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/GLUE.py
+-rw-rw-rw-   0        0        0    38271 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/GWO.py
+-rw-rw-rw-   0        0        0    33260 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/MFO.py
+-rw-rw-rw-   0        0        0    14600 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/MODE.py
+-rw-rw-rw-   0        0        0    24212 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/MOPSO.py
+-rw-rw-rw-   0        0        0    14937 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/NSGA2.py
+-rw-rw-rw-   0        0        0    19098 2023-04-16 07:43:22.000000 pycup-0.1.6/pycup/PESTclasses.py
+-rw-rw-rw-   0        0        0    35498 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/PSO.py
+-rw-rw-rw-   0        0        0    15659 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/Reslib.py
+-rw-rw-rw-   0        0        0    30073 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/SCA.py
+-rw-rw-rw-   0        0        0    32941 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/SOA.py
+-rw-rw-rw-   0        0        0    32160 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/SSA.py
+-rw-rw-rw-   0        0        0     5757 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/TOPSIS.py
+-rw-rw-rw-   0        0        0    33343 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/TSA.py
+-rw-rw-rw-   0        0        0    32912 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/WOA.py
+-rw-rw-rw-   0        0        0      946 2023-04-16 14:04:48.000000 pycup-0.1.6/pycup/__init__.py
+-rw-rw-rw-   0        0        0    10042 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/calc_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:48:12.376021 pycup-0.1.6/pycup/document/
+-rw-rw-rw-   0        0        0   826264 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/document/Documentation.pdf
+-rw-rw-rw-   0        0        0     4027 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/evaluation_metrics.py
+-rw-rw-rw-   0        0        0    53479 2023-04-16 14:25:15.000000 pycup-0.1.6/pycup/integrate.py
+-rw-rw-rw-   0        0        0     7263 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/multi_jobs.py
+-rw-rw-rw-   0        0        0   125408 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/plot.py
+-rw-rw-rw-   0        0        0      460 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/progress_bar.py
+-rw-rw-rw-   0        0        0    10352 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/sampling.py
+-rw-rw-rw-   0        0        0    18935 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/save.py
+-rw-rw-rw-   0        0        0     2068 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/template.py
+-rw-rw-rw-   0        0        0        0 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/test.py
+-rw-rw-rw-   0        0        0     6055 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/test_functions.py
+-rw-rw-rw-   0        0        0    69170 2023-04-16 07:43:22.000000 pycup-0.1.6/pycup/uncertainty_analysis_fun.py
+-rw-rw-rw-   0        0        0    17048 2023-04-16 07:29:17.000000 pycup-0.1.6/pycup/utilize.py
+drwxrwxrwx   0        0        0        0 2023-04-16 14:48:12.373020 pycup-0.1.6/pycup.egg-info/
+-rw-rw-rw-   0        0        0     6321 2023-04-16 14:48:12.000000 pycup-0.1.6/pycup.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-04-16 14:48:12.000000 pycup-0.1.6/pycup.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 14:48:12.000000 pycup-0.1.6/pycup.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-04-16 14:48:12.000000 pycup-0.1.6/pycup.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-16 14:48:12.000000 pycup-0.1.6/pycup.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 14:48:12.380022 pycup-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      953 2023-04-16 08:01:45.000000 pycup-0.1.6/setup.py
```

### Comparing `pycup-0.1.5/PKG-INFO` & `pycup-0.1.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 Metadata-Version: 2.1
 Name: pycup
-Version: 0.1.5
+Version: 0.1.6
 Summary: An auto-calibration tool for environmental models based on heuristic algorithms and uncertainty estimation theory.
 Home-page: https://github.com/QianyangWang/PyCUP
 Author: Qianyang Wang
 Author-email: wqy07010944@hotmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/QianyangWang/PyCUP/DOCUMENT
 Project-URL: Source, https://github.com/QianyangWang/PyCUP/pycup
 Description: # PyCUP
         
-        <img src="https://img.shields.io/badge/Version-0.1.4-brightgreen" /><img src="https://img.shields.io/badge/Language-Python-blue" />	
+        <img src="https://img.shields.io/badge/Version-0.1.6-brightgreen" /><img src="https://img.shields.io/badge/Language-Python-blue" />	
         
         This is an open-source package designed for (environmental) model calibration and uncertainty analysis. The current version is the very first version, we welcome all comments, suggestions, and improvements.
         
-        ## v 0.1.5 Update
+        ## v 0.1.6 Update
         
-        Two new border check mechanisms are included for processing the generated parameters that exceed the user defined search boundaries during the heuristic algorithms' updating stage.
-        
-        1. (The original method) Absorb. The sample value exceeds the lower boundary/ upper boundary will be directly put on the corresponding boundary.
-        2. Random. The sample value exceeds the lower boundary/ upper boundary will be given a random value according to the search space.
-        3. (The currently default method) Rebound. The sample value exceeds the lower boundary/ upper boundary will be given a random value near the corresponding boundary. This method can keep the search direction and avoid the result that a lot of samples locate on the boundary.
+        PyCUP now supports a basic integration with PEST++ calibration project for a more convenient model-agnostic calibration process. The pycup.integrate.PESTconvertor can generate an objective function, which can read/write the parameter file, run the commandline, read the simulation results with the PEST++ instruction files. The function can be used by PyCUP algorithms so that users can do the calibration without writting the objective function and IO functions by themselves. As the PyCUP algorithms have mechanisms differ from which used by PEST++, some settings in PEST++ control file will be ignored. More details can be found in the example in documentations in the repository.
         
         ## What does it have
         
         ### (1) For model calibration/optimization
         
         1. Single-objective heuristic algorithms including PSO, GWO, MFO, SOA, SCA, SSA, TSA, and WOA.
         2. Multi-objective heuristic algorithms including MOPSO, MODE, and NSGA-II.
         3. Elite opposition strategy modified heuristic algorithms -- with better optimum search abilities.
         4. Statistic based-method LHS-GLUE.
+        5. Three kinds of algorithm border check mechanisms including Absorb, Random, and Rebound, designed for different problems.
         
         ### (2) For sensitivity & uncertainty analysis
         
         1. Likelihood uncertainty estimation used in the GLUE framework for the parameter uncertainty analysis/prediction uncertainty estimation.
         2. The frequency based-uncertainty estimation method for the prediction uncertainty estimation.
         3. The multi-linear regression method for the all-at-a-time parameter sensitivity based on statmodels.
         
         ### (3) Other convenient features
         
         1. Multi-processing calibration.
         2. Recording and resuming during the calibration task.
         3. Several result plotting functions.
         4. A special simulation result object  for multi-station & multi-event results (of environmental models) in pycup.ResLib.
-        5. PyCUP can be linked to spotpy database for post-processing, a pycup objective function can also be generated from the spotpy objective function using the module named pycup.integrate.
+        
+        ### (4) Package/Tools integration
+        
+        1. PyCUP can be linked to spotpy database for post-processing, a pycup objective function can also be generated from the spotpy objective function using the module named pycup.integrate.
+        2. The required objective function for pycup calibration can be easily generated using a PEST++ optimization project with/without a tsproc.exe. The PESTconvertor object in pycup.integrate provides several APIs for reading PEST++ files such as .pst, .ins, and .tpl.
         
         ## How to install
         
         ​	The project has been uploaded onto the PyPI https://pypi.org/project/pycup/ . Or install the .whl file in the dist folder.
         
         ```
         pip install pycup
@@ -84,14 +85,15 @@
         3. The example in folder 'Example03-multiobjective' contains an SWMM multi-objective calibration project using EOMOPSO. 
         4. The example in folder 'Example04-validation&prediction' shows how to use our (Ensemble)Validator/(Ensemble)Predictor objects for the validation and prediction of the model using the calibrated parameter (set).
         5. The example in folder 'Example05-multi-station&event' shows how to use the pycup.Reslib.SimulationResult object for the storage of multi-station & multi-event simulation results, as well as the further analysis using them.
         
         <div align=center>
         <img src="https://user-images.githubusercontent.com/116932670/209893309-e67c425f-0eff-47b4-a552-b30d717a138b.png">
         </div>
+        ## Example PEST++ conversion project (with a Xinanjiang hydrologic model)
         
-        
+        1. The example in folder 'Example06-PESTintegration' contains a PEST++ Xinanjiang model calibration project and the python script to run a PyCUP calibration based on it.
         
 Keywords: optimization
 Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `pycup-0.1.5/README.md` & `pycup-0.1.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # PyCUP
 
-<img src="https://img.shields.io/badge/Version-0.1.4-brightgreen" /><img src="https://img.shields.io/badge/Language-Python-blue" />	
+<img src="https://img.shields.io/badge/Version-0.1.6-brightgreen" /><img src="https://img.shields.io/badge/Language-Python-blue" />	
 
 This is an open-source package designed for (environmental) model calibration and uncertainty analysis. The current version is the very first version, we welcome all comments, suggestions, and improvements.
 
-## v 0.1.5 Update
+## v 0.1.6 Update
 
-Two new border check mechanisms are included for processing the generated parameters that exceed the user defined search boundaries during the heuristic algorithms' updating stage.
-
-1. (The original method) Absorb. The sample value exceeds the lower boundary/ upper boundary will be directly put on the corresponding boundary.
-2. Random. The sample value exceeds the lower boundary/ upper boundary will be given a random value according to the search space.
-3. (The currently default method) Rebound. The sample value exceeds the lower boundary/ upper boundary will be given a random value near the corresponding boundary. This method can keep the search direction and avoid the result that a lot of samples locate on the boundary.
+PyCUP now supports a basic integration with PEST++ calibration project for a more convenient model-agnostic calibration process. The pycup.integrate.PESTconvertor can generate an objective function, which can read/write the parameter file, run the commandline, read the simulation results with the PEST++ instruction files. The function can be used by PyCUP algorithms so that users can do the calibration without writting the objective function and IO functions by themselves. As the PyCUP algorithms have mechanisms differ from which used by PEST++, some settings in PEST++ control file will be ignored. More details can be found in the example in documentations in the repository.
 
 ## What does it have
 
 ### (1) For model calibration/optimization
 
 1. Single-objective heuristic algorithms including PSO, GWO, MFO, SOA, SCA, SSA, TSA, and WOA.
 2. Multi-objective heuristic algorithms including MOPSO, MODE, and NSGA-II.
 3. Elite opposition strategy modified heuristic algorithms -- with better optimum search abilities.
 4. Statistic based-method LHS-GLUE.
+5. Three kinds of algorithm border check mechanisms including Absorb, Random, and Rebound, designed for different problems.
 
 ### (2) For sensitivity & uncertainty analysis
 
 1. Likelihood uncertainty estimation used in the GLUE framework for the parameter uncertainty analysis/prediction uncertainty estimation.
 2. The frequency based-uncertainty estimation method for the prediction uncertainty estimation.
 3. The multi-linear regression method for the all-at-a-time parameter sensitivity based on statmodels.
 
 ### (3) Other convenient features
 
 1. Multi-processing calibration.
 2. Recording and resuming during the calibration task.
 3. Several result plotting functions.
 4. A special simulation result object  for multi-station & multi-event results (of environmental models) in pycup.ResLib.
-5. PyCUP can be linked to spotpy database for post-processing, a pycup objective function can also be generated from the spotpy objective function using the module named pycup.integrate.
+
+### (4) Package/Tools integration
+
+1. PyCUP can be linked to spotpy database for post-processing, a pycup objective function can also be generated from the spotpy objective function using the module named pycup.integrate.
+2. The required objective function for pycup calibration can be easily generated using a PEST++ optimization project with/without a tsproc.exe. The PESTconvertor object in pycup.integrate provides several APIs for reading PEST++ files such as .pst, .ins, and .tpl.
 
 ## How to install
 
 ​	The project has been uploaded onto the PyPI https://pypi.org/project/pycup/ . Or install the .whl file in the dist folder.
 
 ```
 pip install pycup
@@ -74,9 +75,10 @@
 3. The example in folder 'Example03-multiobjective' contains an SWMM multi-objective calibration project using EOMOPSO. 
 4. The example in folder 'Example04-validation&prediction' shows how to use our (Ensemble)Validator/(Ensemble)Predictor objects for the validation and prediction of the model using the calibrated parameter (set).
 5. The example in folder 'Example05-multi-station&event' shows how to use the pycup.Reslib.SimulationResult object for the storage of multi-station & multi-event simulation results, as well as the further analysis using them.
 
 <div align=center>
 <img src="https://user-images.githubusercontent.com/116932670/209893309-e67c425f-0eff-47b4-a552-b30d717a138b.png">
 </div>
+## Example PEST++ conversion project (with a Xinanjiang hydrologic model)
 
-
+1. The example in folder 'Example06-PESTintegration' contains a PEST++ Xinanjiang model calibration project and the python script to run a PyCUP calibration based on it.
```

### Comparing `pycup-0.1.5/pycup/GLUE.py` & `pycup-0.1.6/pycup/GLUE.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/GWO.py` & `pycup-0.1.6/pycup/GWO.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/MFO.py` & `pycup-0.1.6/pycup/MFO.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/MODE.py` & `pycup-0.1.6/pycup/MODE.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/MOPSO.py` & `pycup-0.1.6/pycup/MOPSO.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/NSGA2.py` & `pycup-0.1.6/pycup/NSGA2.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/PSO.py` & `pycup-0.1.6/pycup/PSO.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/Reslib.py` & `pycup-0.1.6/pycup/Reslib.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/SCA.py` & `pycup-0.1.6/pycup/SCA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/SOA.py` & `pycup-0.1.6/pycup/SOA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/SSA.py` & `pycup-0.1.6/pycup/SSA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/TOPSIS.py` & `pycup-0.1.6/pycup/TOPSIS.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/TSA.py` & `pycup-0.1.6/pycup/TSA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/WOA.py` & `pycup-0.1.6/pycup/WOA.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/__init__.py` & `pycup-0.1.6/pycup/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from . import MODE
 from . import NSGA2
 from . import utilize
 from . import TOPSIS
 from . import Reslib
 from . import calc_utils
 from . import integrate
+from . import PESTclasses
 
 
 
 __all__ = ['evaluation_metrics','utilize', 'multi_jobs','plot','progress_bar',
            'sampling','save','test_functions','uncertainty_analysis_fun',
            'WOA','TSA','SCA','SOA','SSA','PSO','GLUE','GWO','MFO',
-           'MOPSO','MODE','NSGA2','template', 'TOPSIS',"Reslib","calc_utils","integrate"]
+           'MOPSO','MODE','NSGA2','template', 'TOPSIS',"Reslib","calc_utils","integrate",
+           "PESTclasses"]
```

### Comparing `pycup-0.1.5/pycup/calc_utils.py` & `pycup-0.1.6/pycup/calc_utils.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/document/Documentation.pdf` & `pycup-0.1.6/pycup/document/Documentation.pdf`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/evaluation_metrics.py` & `pycup-0.1.6/pycup/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/multi_jobs.py` & `pycup-0.1.6/pycup/multi_jobs.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/plot.py` & `pycup-0.1.6/pycup/plot.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/sampling.py` & `pycup-0.1.6/pycup/sampling.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/save.py` & `pycup-0.1.6/pycup/save.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/template.py` & `pycup-0.1.6/pycup/template.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/test_functions.py` & `pycup-0.1.6/pycup/test_functions.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup/uncertainty_analysis_fun.py` & `pycup-0.1.6/pycup/uncertainty_analysis_fun.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,18 @@
     u_fun.likelihood_uncertainty(raw_res,threshold=0.5,ppu=0.95)
     """
 
     if not (isinstance(raw_saver, save.RawDataSaver)):
         raise TypeError("The given saver object is not a save.RawDataSaver.")
 
     if raw_saver.opt_type == "GLUE":
-        hr = raw_saver.historical_results
+        if Reslib.UseResObject:
+            hr = raw_saver.historical_results.data
+        else:
+            hr = raw_saver.historical_results
         hf = raw_saver.historical_fitness
         hs = raw_saver.historical_samples
 
     else:
         hr = raw_saver.historical_results
         hf = raw_saver.historical_fitness
         hs = raw_saver.historical_samples
@@ -279,15 +282,18 @@
     if not (isinstance(raw_saver, save.RawDataSaver)):
         raise TypeError("The given saver object is not a save.RawDataSaver.")
 
     if len(obj_weights) != n_obj:
         raise TypeError("The length of objective function weights should be equal to n_obj.")
 
     if raw_saver.opt_type == "GLUE":
-        hr = raw_saver.historical_results
+        if Reslib.UseResObject:
+            hr = raw_saver.historical_results.data
+        else:
+            hr = raw_saver.historical_results
         hf = raw_saver.historical_fitness
         hs = raw_saver.historical_samples
 
     else:
         hr = raw_saver.historical_results
         hf = raw_saver.historical_fitness
         hs = raw_saver.historical_samples
@@ -473,15 +479,18 @@
            be used.
     :param st_id:
     :return:
     """
     if not (isinstance(raw_saver, save.RawDataSaver)):
         raise TypeError("The given saver object is not a save.RawDataSaver.")
     if raw_saver.opt_type == "GLUE":
-        hr = raw_saver.historical_results
+        if Reslib.UseResObject:
+            hr = raw_saver.historical_results.data
+        else:
+            hr = raw_saver.historical_results
         hf = raw_saver.historical_fitness
         hs = raw_saver.historical_samples
 
     else:
         hr = raw_saver.historical_results
         hf = raw_saver.historical_fitness
         hs = raw_saver.historical_samples
@@ -658,15 +667,18 @@
     u_fun.likelihood_uncertaintyMO(raw_res,n_obj=2,thresholds=[0.5,0.2],ppu=0.95,obj_weights=[0.5,0.5])
     """
 
     if not (isinstance(raw_saver, save.RawDataSaver)):
         raise TypeError("The given saver object is not a save.RawDataSaver.")
 
     if raw_saver.opt_type == "GLUE":
-        hr = raw_saver.historical_results
+        if Reslib.UseResObject:
+            hr = raw_saver.historical_results.data
+        else:
+            hr = raw_saver.historical_results
         hf = raw_saver.historical_fitness
         hs = raw_saver.historical_samples
 
     else:
         hr = raw_saver.historical_results
         hf = raw_saver.historical_fitness
         hs = raw_saver.historical_samples
@@ -1162,15 +1174,14 @@
         ppu_line_lower[ob_low] = line_min[ob_low]
         ob_up = np.argwhere(ppu_line_upper > line_max)
         ppu_line_upper[ob_up] = line_max[ob_up]
 
         median_prediction = get_median_series(results)
     else:
         results = pred_raw_saver.results.data
-        results = pred_raw_saver.results.data
         stations = list(results[0].keys())
         ppu_line_lower = Reslib.SimulationResult()
         ppu_line_upper = Reslib.SimulationResult()
         line_min = Reslib.SimulationResult()
         line_max = Reslib.SimulationResult()
         median_prediction = Reslib.SimulationResult()
         for st in stations:
```

### Comparing `pycup-0.1.5/pycup/utilize.py` & `pycup-0.1.6/pycup/utilize.py`

 * *Files identical despite different names*

### Comparing `pycup-0.1.5/pycup.egg-info/PKG-INFO` & `pycup-0.1.6/pycup.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 Metadata-Version: 2.1
 Name: pycup
-Version: 0.1.5
+Version: 0.1.6
 Summary: An auto-calibration tool for environmental models based on heuristic algorithms and uncertainty estimation theory.
 Home-page: https://github.com/QianyangWang/PyCUP
 Author: Qianyang Wang
 Author-email: wqy07010944@hotmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/QianyangWang/PyCUP/DOCUMENT
 Project-URL: Source, https://github.com/QianyangWang/PyCUP/pycup
 Description: # PyCUP
         
-        <img src="https://img.shields.io/badge/Version-0.1.4-brightgreen" /><img src="https://img.shields.io/badge/Language-Python-blue" />	
+        <img src="https://img.shields.io/badge/Version-0.1.6-brightgreen" /><img src="https://img.shields.io/badge/Language-Python-blue" />	
         
         This is an open-source package designed for (environmental) model calibration and uncertainty analysis. The current version is the very first version, we welcome all comments, suggestions, and improvements.
         
-        ## v 0.1.5 Update
+        ## v 0.1.6 Update
         
-        Two new border check mechanisms are included for processing the generated parameters that exceed the user defined search boundaries during the heuristic algorithms' updating stage.
-        
-        1. (The original method) Absorb. The sample value exceeds the lower boundary/ upper boundary will be directly put on the corresponding boundary.
-        2. Random. The sample value exceeds the lower boundary/ upper boundary will be given a random value according to the search space.
-        3. (The currently default method) Rebound. The sample value exceeds the lower boundary/ upper boundary will be given a random value near the corresponding boundary. This method can keep the search direction and avoid the result that a lot of samples locate on the boundary.
+        PyCUP now supports a basic integration with PEST++ calibration project for a more convenient model-agnostic calibration process. The pycup.integrate.PESTconvertor can generate an objective function, which can read/write the parameter file, run the commandline, read the simulation results with the PEST++ instruction files. The function can be used by PyCUP algorithms so that users can do the calibration without writting the objective function and IO functions by themselves. As the PyCUP algorithms have mechanisms differ from which used by PEST++, some settings in PEST++ control file will be ignored. More details can be found in the example in documentations in the repository.
         
         ## What does it have
         
         ### (1) For model calibration/optimization
         
         1. Single-objective heuristic algorithms including PSO, GWO, MFO, SOA, SCA, SSA, TSA, and WOA.
         2. Multi-objective heuristic algorithms including MOPSO, MODE, and NSGA-II.
         3. Elite opposition strategy modified heuristic algorithms -- with better optimum search abilities.
         4. Statistic based-method LHS-GLUE.
+        5. Three kinds of algorithm border check mechanisms including Absorb, Random, and Rebound, designed for different problems.
         
         ### (2) For sensitivity & uncertainty analysis
         
         1. Likelihood uncertainty estimation used in the GLUE framework for the parameter uncertainty analysis/prediction uncertainty estimation.
         2. The frequency based-uncertainty estimation method for the prediction uncertainty estimation.
         3. The multi-linear regression method for the all-at-a-time parameter sensitivity based on statmodels.
         
         ### (3) Other convenient features
         
         1. Multi-processing calibration.
         2. Recording and resuming during the calibration task.
         3. Several result plotting functions.
         4. A special simulation result object  for multi-station & multi-event results (of environmental models) in pycup.ResLib.
-        5. PyCUP can be linked to spotpy database for post-processing, a pycup objective function can also be generated from the spotpy objective function using the module named pycup.integrate.
+        
+        ### (4) Package/Tools integration
+        
+        1. PyCUP can be linked to spotpy database for post-processing, a pycup objective function can also be generated from the spotpy objective function using the module named pycup.integrate.
+        2. The required objective function for pycup calibration can be easily generated using a PEST++ optimization project with/without a tsproc.exe. The PESTconvertor object in pycup.integrate provides several APIs for reading PEST++ files such as .pst, .ins, and .tpl.
         
         ## How to install
         
         ​	The project has been uploaded onto the PyPI https://pypi.org/project/pycup/ . Or install the .whl file in the dist folder.
         
         ```
         pip install pycup
@@ -84,14 +85,15 @@
         3. The example in folder 'Example03-multiobjective' contains an SWMM multi-objective calibration project using EOMOPSO. 
         4. The example in folder 'Example04-validation&prediction' shows how to use our (Ensemble)Validator/(Ensemble)Predictor objects for the validation and prediction of the model using the calibrated parameter (set).
         5. The example in folder 'Example05-multi-station&event' shows how to use the pycup.Reslib.SimulationResult object for the storage of multi-station & multi-event simulation results, as well as the further analysis using them.
         
         <div align=center>
         <img src="https://user-images.githubusercontent.com/116932670/209893309-e67c425f-0eff-47b4-a552-b30d717a138b.png">
         </div>
+        ## Example PEST++ conversion project (with a Xinanjiang hydrologic model)
         
-        
+        1. The example in folder 'Example06-PESTintegration' contains a PEST++ Xinanjiang model calibration project and the python script to run a PyCUP calibration based on it.
         
 Keywords: optimization
 Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `pycup-0.1.5/pycup.egg-info/SOURCES.txt` & `pycup-0.1.6/pycup.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 setup.py
 pycup/GLUE.py
 pycup/GWO.py
 pycup/MFO.py
 pycup/MODE.py
 pycup/MOPSO.py
 pycup/NSGA2.py
+pycup/PESTclasses.py
 pycup/PSO.py
 pycup/Reslib.py
 pycup/SCA.py
 pycup/SOA.py
 pycup/SSA.py
 pycup/TOPSIS.py
 pycup/TSA.py
```

### Comparing `pycup-0.1.5/setup.py` & `pycup-0.1.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 with open(r"README.md",encoding="utf-8") as f:
   long_description = f.read()
 
 
 setup(
     name='pycup',
-  version='0.1.5',
+  version='0.1.6',
   description='An auto-calibration tool for environmental models based on heuristic algorithms and uncertainty estimation theory.',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author='Qianyang Wang',
   author_email='wqy07010944@hotmail.com',
   url='https://github.com/QianyangWang/PyCUP',
   license='MIT License',
   keywords='optimization',
   project_urls={
    'Documentation': 'https://github.com/QianyangWang/PyCUP/DOCUMENT',
    'Source': 'https://github.com/QianyangWang/PyCUP/pycup',
   },
   packages=find_packages(exclude=["test", "test.*"]),
   package_data={'pycup':['document/*.pdf']},
-  install_requires=['numpy', 'matplotlib','scipy','pyDOE','statsmodels','pandas'],
+  install_requires=['numpy', 'matplotlib','scipy','pyDOE','statsmodels','pandas','prettytable'],
   python_requires='>=3'
   )
```

