# Comparing `tmp/flarespy-0.5.1.tar.gz` & `tmp/flarespy-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarespy-0.5.1.tar", max compression
+gzip compressed data, was "flarespy-0.5.2.tar", max compression
```

## Comparing `flarespy-0.5.1.tar` & `flarespy-0.5.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.5.1/LICENSE
--rw-r--r--   0        0        0      663 2023-04-07 13:43:15.879227 flarespy-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.5.1/src/flarespy/Flare_model.py
--rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.5.1/src/flarespy/__init__.py
--rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.5.1/src/flarespy/data/model.dat
--rw-r--r--   0        0        0    25108 2023-03-30 09:31:09.941091 flarespy-0.5.1/src/flarespy/flarefinder.py
--rw-r--r--   0        0        0     3994 2023-04-07 14:40:27.932103 flarespy-0.5.1/src/flarespy/utils.py
--rw-r--r--   0        0        0       22 2023-04-07 03:16:36.299414 flarespy-0.5.1/src/flarespy/version.py
--rw-r--r--   0        0        0      855 1970-01-01 00:00:00.000000 flarespy-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.5.2/LICENSE
+-rw-r--r--   0        0        0      647 2023-04-16 02:44:36.072093 flarespy-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.5.2/src/flarespy/Flare_model.py
+-rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.5.2/src/flarespy/__init__.py
+-rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.5.2/src/flarespy/data/model.dat
+-rw-r--r--   0        0        0    25108 2023-03-30 09:31:09.941091 flarespy-0.5.2/src/flarespy/flarefinder.py
+-rw-r--r--   0        0        0     4393 2023-04-15 15:30:07.968446 flarespy-0.5.2/src/flarespy/utils.py
+-rw-r--r--   0        0        0       22 2023-04-16 02:24:58.102904 flarespy-0.5.2/src/flarespy/version.py
+-rw-r--r--   0        0        0      794 1970-01-01 00:00:00.000000 flarespy-0.5.2/PKG-INFO
```

### Comparing `flarespy-0.5.1/LICENSE` & `flarespy-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flarespy-0.5.1/pyproject.toml` & `flarespy-0.5.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [tool.poetry]
 name = "flarespy"
-version = "0.5.1"
+version = "0.5.2"
 description = "Find flares in TESS light curves"
 authors = ["Keyu Xing <kyxing@mail.bnu.edu.cn>"]
 license = "MIT"
 homepage = "https://github.com/keyuxing/flarespy"
 repository = "https://github.com/keyuxing/flarespy"
 
 [tool.poetry.dependencies]
 bottleneck = ">=1.3"
 lightkurve = ">=2.3"
 numba = { version = ">=0.55.2", allow-prereleases = true}
-pandas = "<2.0"
 python = ">=3.8"
 retrying = ">=1.3"
 scikit-learn = ">=1.1"
-tsfresh = ">=0.20"
 wotan = ">=1.10"
 
 [tool.poetry.dev-dependencies]
 black = ">=22.8"
 corner = ">=2.2"
 emcee = ">=3.1"
 jupyter = ">=1.0"
 optuna = ">=3.1"
 seaborn = ">=0.11"
 tokenize-rt = ">=4.1"
+tsfresh = ">=0.20"
```

### Comparing `flarespy-0.5.1/src/flarespy/Flare_model.py` & `flarespy-0.5.2/src/flarespy/Flare_model.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.5.1/src/flarespy/data/model.dat` & `flarespy-0.5.2/src/flarespy/data/model.dat`

 * *Files identical despite different names*

### Comparing `flarespy-0.5.1/src/flarespy/flarefinder.py` & `flarespy-0.5.2/src/flarespy/flarefinder.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.5.1/src/flarespy/utils.py` & `flarespy-0.5.2/src/flarespy/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import warnings
 
 import joblib
 import numpy as np
 import pandas as pd
-from tsfresh.feature_extraction import extract_features
 
 from . import PACKAGEDIR
 
 MODEL_PATH = PACKAGEDIR / "data" / "model.dat"
 with warnings.catch_warnings():
     warnings.simplefilter("ignore", category=UserWarning)
     RFC_MODEL = joblib.load(MODEL_PATH)
@@ -24,40 +23,50 @@
     "snr",
     "amp",
     "dur",
     "ed",
     "energy",
 ]
 
-FC_PARAMETERS = {
-    "abs_energy": None,
-    "first_location_of_maximum": None,
-    "index_mass_quantile": [{"q": 0.5}],
-    "kurtosis": None,
-    "length": None,
-    "maximum": None,
-    "root_mean_square": None,
-    "skewness": None,
-    "standard_deviation": None,
-}
+
+def extract_features(x):
+    abs_energy = np.dot(x, x)
+    first_location_of_maximum = np.argmax(x) / len(x)
+
+    abs_x = np.abs(x)
+    s = np.sum(abs_x)
+    mass_centralized = np.cumsum(abs_x) / s
+    mass_center = (np.argmax(mass_centralized >= 0.5) + 1) / len(x)
+
+    kurtosis = pd.Series.kurtosis(pd.Series(x))
+    length = len(x)
+    maximum = np.max(x)
+    root_mean_square = np.sqrt(np.mean(np.square(x)))
+    skewness = pd.Series.skew(pd.Series(x))
+    standard_deviation = np.std(x)
+
+    return pd.DataFrame(
+        {
+            "flux__abs_energy": [abs_energy],
+            "flux__first_location_of_maximum": [first_location_of_maximum],
+            "flux__index_mass_quantile__q_0.5": [mass_center],
+            "flux__kurtosis": [kurtosis],
+            "flux__length": [length],
+            "flux__maximum": [maximum],
+            "flux__root_mean_square": [root_mean_square],
+            "flux__skewness": [skewness],
+            "flux__standard_deviation": [standard_deviation],
+        }
+    )
 
 
 def get_flare_probability(time, flux):
     time *= 1440
-    data = pd.DataFrame({"time": time - time.min(), "flux": flux})
-    data_id = np.ones(len(data), dtype=int)
-    data.insert(0, "id", data_id)
-    feature = extract_features(
-        data,
-        column_id="id",
-        column_sort="time",
-        default_fc_parameters=FC_PARAMETERS,
-        disable_progressbar=True,
-        n_jobs=0,
-    )
+    time -= time.min()
+    feature = extract_features(flux)
 
     return RFC_MODEL.predict_proba(feature)[0][0]
 
 
 def extend(time, flux, t_start, t_stop, t_max_extend, n_sigma=1, n_left=1, n_right=1, mode=1):
     indexes_range = np.nonzero((time >= t_start - t_max_extend) & (time <= t_stop + t_max_extend))[0]
     i_start = np.nonzero(time == t_start)[0][0]
```

### Comparing `flarespy-0.5.1/PKG-INFO` & `flarespy-0.5.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flarespy
-Version: 0.5.1
+Version: 0.5.2
 Summary: Find flares in TESS light curves
 Home-page: https://github.com/keyuxing/flarespy
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -12,13 +12,11 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bottleneck (>=1.3)
 Requires-Dist: lightkurve (>=2.3)
 Requires-Dist: numba (>=0.55.2)
-Requires-Dist: pandas (<2.0)
 Requires-Dist: retrying (>=1.3)
 Requires-Dist: scikit-learn (>=1.1)
-Requires-Dist: tsfresh (>=0.20)
 Requires-Dist: wotan (>=1.10)
 Project-URL: Repository, https://github.com/keyuxing/flarespy
```

