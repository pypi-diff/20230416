# Comparing `tmp/pyPhasesML-0.4.8.tar.gz` & `tmp/pyPhasesML-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesML-0.4.8.tar", last modified: Sun Apr 16 15:24:23 2023, max compression
+gzip compressed data, was "pyPhasesML-0.4.9.tar", last modified: Sun Apr 16 16:27:15 2023, max compression
```

## Comparing `pyPhasesML-0.4.8.tar` & `pyPhasesML-0.4.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:24:23.244321 pyPhasesML-0.4.8/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3691 2023-04-16 15:24:23.244321 pyPhasesML-0.4.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3184 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:24:23.238335 pyPhasesML-0.4.8/pyPhasesML/
--rw-rw-rw-   0 root         (0) root         (0)     2348 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyPhasesML/DataAugmentation.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyPhasesML/DataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyPhasesML/FeatureExtraction.py
--rw-rw-rw-   0 root         (0) root         (0)     3887 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyPhasesML/Model.py
--rw-rw-rw-   0 root         (0) root         (0)     4368 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyPhasesML/ModelManager.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyPhasesML/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4558 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyPhasesML/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyPhasesML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:24:23.241328 pyPhasesML-0.4.8/pyPhasesML/adapter/
--rw-rw-rw-   0 root         (0) root         (0)    10212 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyPhasesML/adapter/ModelKerasAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     7116 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyPhasesML/adapter/ModelTf1Adapter.py
--rw-rw-rw-   0 root         (0) root         (0)    17734 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyPhasesML/adapter/ModelTorchAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyPhasesML/adapter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyPhasesML/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:24:23.242325 pyPhasesML-0.4.8/pyPhasesML/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     5358 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyPhasesML/exporter/MemmapRecordExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyPhasesML/exporter/ModelExporter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyPhasesML/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:24:23.243323 pyPhasesML-0.4.8/pyPhasesML/scorer/
--rw-rw-rw-   0 root         (0) root         (0)    22972 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyPhasesML/scorer/Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyPhasesML/scorer/ScorerTF.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyPhasesML/scorer/ScorerTorch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyPhasesML/scorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 15:24:23.240330 pyPhasesML-0.4.8/pyPhasesML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3691 2023-04-16 15:24:23.000000 pyPhasesML-0.4.8/pyPhasesML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      838 2023-04-16 15:24:23.000000 pyPhasesML-0.4.8/pyPhasesML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 15:24:23.000000 pyPhasesML-0.4.8/pyPhasesML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-16 15:24:23.000000 pyPhasesML-0.4.8/pyPhasesML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-16 15:24:23.000000 pyPhasesML-0.4.8/pyPhasesML.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-04-16 15:23:56.000000 pyPhasesML-0.4.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 15:24:23.244321 pyPhasesML-0.4.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      858 2023-04-16 15:23:58.000000 pyPhasesML-0.4.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:27:15.594520 pyPhasesML-0.4.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-04-16 16:27:15.594520 pyPhasesML-0.4.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3184 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:27:15.589520 pyPhasesML-0.4.9/pyPhasesML/
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/DataAugmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/DataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/FeatureExtraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3887 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4368 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/ModelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4558 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:27:15.591520 pyPhasesML-0.4.9/pyPhasesML/adapter/
+-rw-rw-rw-   0 root         (0) root         (0)    10212 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/adapter/ModelKerasAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7116 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/adapter/ModelTf1Adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)    17734 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/adapter/ModelTorchAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/adapter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:27:15.592520 pyPhasesML-0.4.9/pyPhasesML/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     5358 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/exporter/MemmapRecordExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/exporter/ModelExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:27:15.594520 pyPhasesML-0.4.9/pyPhasesML/scorer/
+-rw-rw-rw-   0 root         (0) root         (0)    22838 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/scorer/Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/scorer/ScorerTF.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/scorer/ScorerTorch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyPhasesML/scorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 16:27:15.590520 pyPhasesML-0.4.9/pyPhasesML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-04-16 16:27:15.000000 pyPhasesML-0.4.9/pyPhasesML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      838 2023-04-16 16:27:15.000000 pyPhasesML-0.4.9/pyPhasesML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 16:27:15.000000 pyPhasesML-0.4.9/pyPhasesML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-16 16:27:15.000000 pyPhasesML-0.4.9/pyPhasesML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-16 16:27:15.000000 pyPhasesML-0.4.9/pyPhasesML.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-04-16 16:26:47.000000 pyPhasesML-0.4.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 16:27:15.595520 pyPhasesML-0.4.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      858 2023-04-16 16:26:49.000000 pyPhasesML-0.4.9/setup.py
```

### Comparing `pyPhasesML-0.4.8/LICENSE` & `pyPhasesML-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.8/PKG-INFO` & `pyPhasesML-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.4.8
+Version: 0.4.9
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.4.8/README.md` & `pyPhasesML-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.8/pyPhasesML/DataAugmentation.py` & `pyPhasesML-0.4.9/pyPhasesML/DataAugmentation.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.8/pyPhasesML/DataSet.py` & `pyPhasesML-0.4.9/pyPhasesML/DataSet.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.8/pyPhasesML/FeatureExtraction.py` & `pyPhasesML-0.4.9/pyPhasesML/FeatureExtraction.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.8/pyPhasesML/Model.py` & `pyPhasesML-0.4.9/pyPhasesML/Model.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.8/pyPhasesML/ModelManager.py` & `pyPhasesML-0.4.9/pyPhasesML/ModelManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.8/pyPhasesML/Plugin.py` & `pyPhasesML-0.4.9/pyPhasesML/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.8/pyPhasesML/SignalPreprocessing.py` & `pyPhasesML-0.4.9/pyPhasesML/SignalPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.8/pyPhasesML/adapter/ModelKerasAdapter.py` & `pyPhasesML-0.4.9/pyPhasesML/adapter/ModelKerasAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.8/pyPhasesML/adapter/ModelTf1Adapter.py` & `pyPhasesML-0.4.9/pyPhasesML/adapter/ModelTf1Adapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.8/pyPhasesML/adapter/ModelTorchAdapter.py` & `pyPhasesML-0.4.9/pyPhasesML/adapter/ModelTorchAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.8/pyPhasesML/config.yaml` & `pyPhasesML-0.4.9/pyPhasesML/config.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.8/pyPhasesML/exporter/MemmapRecordExporter.py` & `pyPhasesML-0.4.9/pyPhasesML/exporter/MemmapRecordExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.8/pyPhasesML/exporter/ModelExporter.py` & `pyPhasesML-0.4.9/pyPhasesML/exporter/ModelExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.8/pyPhasesML/scorer/Scorer.py` & `pyPhasesML-0.4.9/pyPhasesML/scorer/Scorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,28 +315,25 @@
             self.results[metricName] = self.addedMetrics[metricName]["score"](truth, prediction)
         elif metricName in ["kappa", "accuracy"]:
             confusion = self.scoreMetric("confusion", truth, prediction)
             k, acc = self.calculateKappaAccFromConfusion(confusion)
             self.results["accuracy"] = acc
             self.results["kappa"] = k
         elif metricName in ["f1"]:
-            if self.numClasses > 2:
-                f1s = []
-                confusion = self.scoreMetric("confusion", truth, prediction)
-                for i in range(self.numClasses):
-                    # first = truth, second = predicted
-                    tp = confusion[i][i]
-                    fp = sum(confusion[i, :]) - tp
-                    fn = sum(confusion[:, i]) - tp
-                    f1 = tp / (tp + 0.5 * (fp + fn))
-                    self.results["f1-%i" % i] = f1
-                    f1s.append(f1)
+            f1s = []
+            confusion = self.scoreMetric("confusion", truth, prediction)
+            for i in range(self.numClasses):
+                # first = truth, second = predicted
+                tp = confusion[i][i]
+                fp = sum(confusion[i, :]) - tp
+                fn = sum(confusion[:, i]) - tp
+                f1 = tp / (tp + 0.5 * (fp + fn))
+                self.results["f1-%i" % i] = f1
+                f1s.append(f1)
                 self.results["f1"] = np.mean(f1s)
-            else:
-                self.results["f1"] = f1
         elif metricName == "confusion":
             prediction = self.flattenPrediction(prediction, threshold=self.threshold)
             result = confusion_matrix(
                 truth, prediction, labels=range(self.numClasses)
             )  # , labels=range(self.numClasses) # HPC comp
         elif metricName in ["auprc", "auroc"]:
             classLikelyhood = self.getClassLikelyhood(prediction)
```

### Comparing `pyPhasesML-0.4.8/pyPhasesML.egg-info/PKG-INFO` & `pyPhasesML-0.4.9/pyPhasesML.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.4.8
+Version: 0.4.9
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.4.8/pyPhasesML.egg-info/SOURCES.txt` & `pyPhasesML-0.4.9/pyPhasesML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.8/setup.py` & `pyPhasesML-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesML",
-    version="v0.4.8"[1:],
+    version="v0.4.9"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/",
     packages=setuptools.find_packages(),
```

