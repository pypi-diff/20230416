# Comparing `tmp/pyPhasesML-0.4.6.tar.gz` & `tmp/pyPhasesML-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPhasesML-0.4.6.tar", last modified: Sat Apr 15 13:40:49 2023, max compression
+gzip compressed data, was "pyPhasesML-0.4.7.tar", last modified: Sun Apr 16 09:14:13 2023, max compression
```

## Comparing `pyPhasesML-0.4.6.tar` & `pyPhasesML-0.4.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 13:40:49.412016 pyPhasesML-0.4.6/
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3691 2023-04-15 13:40:49.412016 pyPhasesML-0.4.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3184 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 13:40:49.406015 pyPhasesML-0.4.6/pyPhasesML/
--rw-rw-rw-   0 root         (0) root         (0)     2348 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyPhasesML/DataAugmentation.py
--rw-rw-rw-   0 root         (0) root         (0)      895 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyPhasesML/DataSet.py
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyPhasesML/FeatureExtraction.py
--rw-rw-rw-   0 root         (0) root         (0)     3887 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyPhasesML/Model.py
--rw-rw-rw-   0 root         (0) root         (0)     4368 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyPhasesML/ModelManager.py
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyPhasesML/Plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     4558 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyPhasesML/SignalPreprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyPhasesML/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 13:40:49.409016 pyPhasesML-0.4.6/pyPhasesML/adapter/
--rw-rw-rw-   0 root         (0) root         (0)    10212 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyPhasesML/adapter/ModelKerasAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)     7116 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyPhasesML/adapter/ModelTf1Adapter.py
--rw-rw-rw-   0 root         (0) root         (0)    17734 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyPhasesML/adapter/ModelTorchAdapter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyPhasesML/adapter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyPhasesML/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 13:40:49.410016 pyPhasesML-0.4.6/pyPhasesML/exporter/
--rw-rw-rw-   0 root         (0) root         (0)     5358 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyPhasesML/exporter/MemmapRecordExporter.py
--rw-rw-rw-   0 root         (0) root         (0)     3201 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyPhasesML/exporter/ModelExporter.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyPhasesML/exporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 13:40:49.411016 pyPhasesML-0.4.6/pyPhasesML/scorer/
--rw-rw-rw-   0 root         (0) root         (0)    19512 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyPhasesML/scorer/Scorer.py
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyPhasesML/scorer/ScorerTF.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyPhasesML/scorer/ScorerTorch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyPhasesML/scorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-15 13:40:49.408016 pyPhasesML-0.4.6/pyPhasesML.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3691 2023-04-15 13:40:49.000000 pyPhasesML-0.4.6/pyPhasesML.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      838 2023-04-15 13:40:49.000000 pyPhasesML-0.4.6/pyPhasesML.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-15 13:40:49.000000 pyPhasesML-0.4.6/pyPhasesML.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-04-15 13:40:49.000000 pyPhasesML-0.4.6/pyPhasesML.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-15 13:40:49.000000 pyPhasesML-0.4.6/pyPhasesML.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      484 2023-04-15 13:40:19.000000 pyPhasesML-0.4.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-15 13:40:49.412016 pyPhasesML-0.4.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      858 2023-04-15 13:40:21.000000 pyPhasesML-0.4.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:14:13.237638 pyPhasesML-0.4.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-04-16 09:14:13.236638 pyPhasesML-0.4.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3184 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:14:13.231637 pyPhasesML-0.4.7/pyPhasesML/
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyPhasesML/DataAugmentation.py
+-rw-rw-rw-   0 root         (0) root         (0)      895 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyPhasesML/DataSet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyPhasesML/FeatureExtraction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3887 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyPhasesML/Model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4368 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyPhasesML/ModelManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyPhasesML/Plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4558 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyPhasesML/SignalPreprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyPhasesML/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:14:13.234638 pyPhasesML-0.4.7/pyPhasesML/adapter/
+-rw-rw-rw-   0 root         (0) root         (0)    10212 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyPhasesML/adapter/ModelKerasAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7116 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyPhasesML/adapter/ModelTf1Adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)    17734 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyPhasesML/adapter/ModelTorchAdapter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyPhasesML/adapter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1106 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyPhasesML/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:14:13.235638 pyPhasesML-0.4.7/pyPhasesML/exporter/
+-rw-rw-rw-   0 root         (0) root         (0)     5358 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyPhasesML/exporter/MemmapRecordExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyPhasesML/exporter/ModelExporter.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyPhasesML/exporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:14:13.236638 pyPhasesML-0.4.7/pyPhasesML/scorer/
+-rw-rw-rw-   0 root         (0) root         (0)    19374 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyPhasesML/scorer/Scorer.py
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyPhasesML/scorer/ScorerTF.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyPhasesML/scorer/ScorerTorch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyPhasesML/scorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:14:13.232638 pyPhasesML-0.4.7/pyPhasesML.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3691 2023-04-16 09:14:13.000000 pyPhasesML-0.4.7/pyPhasesML.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      838 2023-04-16 09:14:13.000000 pyPhasesML-0.4.7/pyPhasesML.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 09:14:13.000000 pyPhasesML-0.4.7/pyPhasesML.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-04-16 09:14:13.000000 pyPhasesML-0.4.7/pyPhasesML.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-16 09:14:13.000000 pyPhasesML-0.4.7/pyPhasesML.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-04-16 09:13:42.000000 pyPhasesML-0.4.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-16 09:14:13.237638 pyPhasesML-0.4.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      858 2023-04-16 09:13:44.000000 pyPhasesML-0.4.7/setup.py
```

### Comparing `pyPhasesML-0.4.6/LICENSE` & `pyPhasesML-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.6/PKG-INFO` & `pyPhasesML-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.4.6
+Version: 0.4.7
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.4.6/README.md` & `pyPhasesML-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.6/pyPhasesML/DataAugmentation.py` & `pyPhasesML-0.4.7/pyPhasesML/DataAugmentation.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.6/pyPhasesML/DataSet.py` & `pyPhasesML-0.4.7/pyPhasesML/DataSet.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.6/pyPhasesML/FeatureExtraction.py` & `pyPhasesML-0.4.7/pyPhasesML/FeatureExtraction.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.6/pyPhasesML/Model.py` & `pyPhasesML-0.4.7/pyPhasesML/Model.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.6/pyPhasesML/ModelManager.py` & `pyPhasesML-0.4.7/pyPhasesML/ModelManager.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.6/pyPhasesML/Plugin.py` & `pyPhasesML-0.4.7/pyPhasesML/Plugin.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.6/pyPhasesML/SignalPreprocessing.py` & `pyPhasesML-0.4.7/pyPhasesML/SignalPreprocessing.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.6/pyPhasesML/adapter/ModelKerasAdapter.py` & `pyPhasesML-0.4.7/pyPhasesML/adapter/ModelKerasAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.6/pyPhasesML/adapter/ModelTf1Adapter.py` & `pyPhasesML-0.4.7/pyPhasesML/adapter/ModelTf1Adapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.6/pyPhasesML/adapter/ModelTorchAdapter.py` & `pyPhasesML-0.4.7/pyPhasesML/adapter/ModelTorchAdapter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.6/pyPhasesML/config.yaml` & `pyPhasesML-0.4.7/pyPhasesML/config.yaml`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.6/pyPhasesML/exporter/MemmapRecordExporter.py` & `pyPhasesML-0.4.7/pyPhasesML/exporter/MemmapRecordExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.6/pyPhasesML/exporter/ModelExporter.py` & `pyPhasesML-0.4.7/pyPhasesML/exporter/ModelExporter.py`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.6/pyPhasesML/scorer/Scorer.py` & `pyPhasesML-0.4.7/pyPhasesML/scorer/Scorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,28 +309,25 @@
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
-                self.results["f1"] = np.mean(f1s)
-            else:
-                self.results["f1"] = f1
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
+            self.results["f1"] = np.mean(f1s)
         elif metricName == "confusion":
             prediction = self.flattenPrediction(prediction, threshold=self.threshold)
             result = confusion_matrix(
                 truth, prediction, labels=range(self.numClasses)
             )  # , labels=range(self.numClasses) # HPC comp
         elif metricName in ["auprc", "auroc"]:
             classLikelyhood = self.getClassLikelyhood(prediction)
```

### Comparing `pyPhasesML-0.4.6/pyPhasesML.egg-info/PKG-INFO` & `pyPhasesML-0.4.7/pyPhasesML.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPhasesML
-Version: 0.4.6
+Version: 0.4.7
 Summary: A Framework for creating a boilerplate template for ai projects that are ready for MLOps
 Home-page: https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/
 Author: Franz Ehrlich
 Author-email: fehrlichd@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyPhasesML-0.4.6/pyPhasesML.egg-info/SOURCES.txt` & `pyPhasesML-0.4.7/pyPhasesML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyPhasesML-0.4.6/setup.py` & `pyPhasesML-0.4.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyPhasesML",
-    version="v0.4.6"[1:],
+    version="v0.4.7"[1:],
     author="Franz Ehrlich",
     author_email="fehrlichd@gmail.com",
     description="A Framework for creating a boilerplate template for ai projects that are ready for MLOps",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/tud.ibmt.public/pyphases/pyphasesml/",
     packages=setuptools.find_packages(),
```

