# Comparing `tmp/imops-0.7.3.tar.gz` & `tmp/imops-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imops-0.7.3.tar", last modified: Sun Mar 26 19:55:05 2023, max compression
+gzip compressed data, was "imops-0.7.4.tar", last modified: Sun Apr 16 18:03:52 2023, max compression
```

## Comparing `imops-0.7.3.tar` & `imops-0.7.4.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:55:05.729901 imops-0.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-26 19:55:01.000000 imops-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-26 19:55:01.000000 imops-0.7.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-03-26 19:55:05.729901 imops-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-03-26 19:55:01.000000 imops-0.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-03-26 19:55:01.000000 imops-0.7.3/_pyproject_build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:55:05.729901 imops-0.7.3/imops/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-26 19:55:01.000000 imops-0.7.3/imops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-26 19:55:01.000000 imops-0.7.3/imops/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-26 19:55:01.000000 imops-0.7.3/imops/_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-03-26 19:55:01.000000 imops-0.7.3/imops/_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-03-26 19:55:01.000000 imops-0.7.3/imops/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-03-26 19:55:01.000000 imops-0.7.3/imops/crop.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-03-26 19:55:01.000000 imops-0.7.3/imops/interp1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-03-26 19:55:01.000000 imops-0.7.3/imops/measure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-03-26 19:55:01.000000 imops-0.7.3/imops/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-03-26 19:55:01.000000 imops-0.7.3/imops/pad.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:55:01.000000 imops-0.7.3/imops/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-03-26 19:55:01.000000 imops-0.7.3/imops/radon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:55:05.729901 imops-0.7.3/imops/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 19:55:01.000000 imops-0.7.3/imops/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-03-26 19:55:01.000000 imops-0.7.3/imops/src/_backprojection.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-03-26 19:55:05.000000 imops-0.7.3/imops/src/_fast_backprojection.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-03-26 19:55:05.000000 imops-0.7.3/imops/src/_fast_morphology.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-03-26 19:55:05.000000 imops-0.7.3/imops/src/_fast_numeric.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-03-26 19:55:05.000000 imops-0.7.3/imops/src/_fast_radon.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    14511 2023-03-26 19:55:05.000000 imops-0.7.3/imops/src/_fast_zoom.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-03-26 19:55:01.000000 imops-0.7.3/imops/src/_morphology.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-03-26 19:55:01.000000 imops-0.7.3/imops/src/_numba_zoom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-03-26 19:55:01.000000 imops-0.7.3/imops/src/_numeric.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-03-26 19:55:01.000000 imops-0.7.3/imops/src/_radon.pyx
--rw-r--r--   0 runner    (1001) docker     (123)    14511 2023-03-26 19:55:01.000000 imops-0.7.3/imops/src/_zoom.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-03-26 19:55:01.000000 imops-0.7.3/imops/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-03-26 19:55:01.000000 imops-0.7.3/imops/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-03-26 19:55:01.000000 imops-0.7.3/imops/zoom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:55:05.729901 imops-0.7.3/imops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-03-26 19:55:05.000000 imops-0.7.3/imops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-03-26 19:55:05.000000 imops-0.7.3/imops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 19:55:05.000000 imops-0.7.3/imops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-26 19:55:05.000000 imops-0.7.3/imops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-26 19:55:05.000000 imops-0.7.3/imops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-03-26 19:55:01.000000 imops-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-26 19:55:01.000000 imops-0.7.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 19:55:05.729901 imops-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-03-26 19:55:01.000000 imops-0.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:03:52.557598 imops-0.7.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-16 18:03:49.000000 imops-0.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-16 18:03:49.000000 imops-0.7.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-04-16 18:03:52.557598 imops-0.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-04-16 18:03:49.000000 imops-0.7.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-16 18:03:49.000000 imops-0.7.4/_pyproject_build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:03:52.553597 imops-0.7.4/imops/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-16 18:03:49.000000 imops-0.7.4/imops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-16 18:03:49.000000 imops-0.7.4/imops/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-16 18:03:49.000000 imops-0.7.4/imops/_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-16 18:03:49.000000 imops-0.7.4/imops/_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-16 18:03:49.000000 imops-0.7.4/imops/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-16 18:03:49.000000 imops-0.7.4/imops/crop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-04-16 18:03:49.000000 imops-0.7.4/imops/interp1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-04-16 18:03:49.000000 imops-0.7.4/imops/measure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-04-16 18:03:49.000000 imops-0.7.4/imops/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-04-16 18:03:49.000000 imops-0.7.4/imops/pad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8927 2023-04-16 18:03:49.000000 imops-0.7.4/imops/radon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:03:52.557598 imops-0.7.4/imops/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:03:49.000000 imops-0.7.4/imops/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-16 18:03:49.000000 imops-0.7.4/imops/src/_backprojection.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-16 18:03:50.000000 imops-0.7.4/imops/src/_fast_backprojection.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-16 18:03:50.000000 imops-0.7.4/imops/src/_fast_morphology.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-16 18:03:50.000000 imops-0.7.4/imops/src/_fast_numeric.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-16 18:03:50.000000 imops-0.7.4/imops/src/_fast_radon.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    14511 2023-04-16 18:03:50.000000 imops-0.7.4/imops/src/_fast_zoom.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-04-16 18:03:49.000000 imops-0.7.4/imops/src/_morphology.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    10246 2023-04-16 18:03:49.000000 imops-0.7.4/imops/src/_numba_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-16 18:03:49.000000 imops-0.7.4/imops/src/_numeric.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-16 18:03:49.000000 imops-0.7.4/imops/src/_radon.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    14511 2023-04-16 18:03:49.000000 imops-0.7.4/imops/src/_zoom.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-16 18:03:49.000000 imops-0.7.4/imops/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-04-16 18:03:49.000000 imops-0.7.4/imops/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-04-16 18:03:49.000000 imops-0.7.4/imops/zoom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:03:52.553597 imops-0.7.4/imops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-04-16 18:03:52.000000 imops-0.7.4/imops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-16 18:03:52.000000 imops-0.7.4/imops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 18:03:52.000000 imops-0.7.4/imops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-16 18:03:52.000000 imops-0.7.4/imops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 18:03:52.000000 imops-0.7.4/imops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-16 18:03:49.000000 imops-0.7.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-16 18:03:49.000000 imops-0.7.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 18:03:52.557598 imops-0.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-16 18:03:49.000000 imops-0.7.4/setup.py
```

### Comparing `imops-0.7.3/LICENSE` & `imops-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/PKG-INFO` & `imops-0.7.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,30 @@
 Metadata-Version: 2.1
 Name: imops
-Version: 0.7.3
+Version: 0.7.4
 Summary: Efficient parallelizable algorithms for multidimensional arrays to speed up your data pipelines
 Home-page: https://github.com/neuro-ml/imops
-Download-URL: https://github.com/neuro-ml/imops/archive/v0.7.3.tar.gz
 Author: maxme1, vovaf709, talgat
-Author-email: maxme1 <maxs987@gmail.com>, vovaf709 <vovaf709@yandex.ru>, talgat <saparov2130@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2022 NeuroML
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/neuro-ml/imops
-Project-URL: Issues, https://github.com/neuro-ml/imops/issues
-Project-URL: Source, https://github.com/neuro-ml/imops
-Project-URL: Docs, https://neuro-ml.github.io/imops
+Author-email: maxs987@gmail.com, vovaf709@yandex.ru, saparov2130@gmail.com
+License: MIT
+Download-URL: https://github.com/neuro-ml/imops/archive/v0.7.4.tar.gz
 Keywords: image processing,fast,ndarray,data pipelines
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: numba
 Provides-Extra: all
+Provides-Extra: numba
 License-File: LICENSE
 
 [![codecov](https://codecov.io/gh/neuro-ml/imops/branch/master/graph/badge.svg)](https://codecov.io/gh/neuro-ml/imops)
 [![pypi](https://img.shields.io/pypi/v/imops?logo=pypi&label=PyPi)](https://pypi.org/project/imops/)
 ![License](https://img.shields.io/github/license/neuro-ml/imops)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/imops)](https://pypi.org/project/imops/)
 
@@ -164,7 +140,9 @@
 | `binary_opening`  | &check; | &check; | &cross; |
 
 # Acknowledgements
 
 Some parts of our code for radon/inverse radon transform as well as the code for linear interpolation are inspired by
 the implementations from [`scikit-image`](https://github.com/scikit-image/scikit-image) and [`scipy`](https://github.com/scipy/scipy).
 Also we used [`fastremap`](https://github.com/seung-lab/fastremap) and [`cc3d`](https://github.com/seung-lab/connected-components-3d) out of the box.
+
+
```

### Comparing `imops-0.7.3/README.md` & `imops-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/_pyproject_build.py` & `imops-0.7.4/_pyproject_build.py`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/_configs.py` & `imops-0.7.4/imops/_configs.py`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/_numeric.py` & `imops-0.7.4/imops/_numeric.py`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/backend.py` & `imops-0.7.4/imops/backend.py`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/crop.py` & `imops-0.7.4/imops/crop.py`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/interp1d.py` & `imops-0.7.4/imops/interp1d.py`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/measure.py` & `imops-0.7.4/imops/measure.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
     if return_num:
         res.append(('num_components', num_components))
     if return_labels:
         res.append(('labels', np.array(range(1, num_components + 1))))
     if return_sizes:
         _, sizes = unique(labeled_image, return_counts=True)
-        res.append(('sizes', sizes[1:]))
+        res.append(('sizes', sizes[1:] if 0 in labeled_image else sizes))
 
     if len(res) == 1:
         return labeled_image
 
     return namedtuple('Labeling', [subres[0] for subres in res])(*[subres[1] for subres in res])
```

### Comparing `imops-0.7.3/imops/morphology.py` & `imops-0.7.4/imops/morphology.py`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/pad.py` & `imops-0.7.4/imops/pad.py`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/radon.py` & `imops-0.7.4/imops/radon.py`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/src/_backprojection.pyx` & `imops-0.7.4/imops/src/_backprojection.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/src/_fast_backprojection.pyx` & `imops-0.7.4/imops/src/_fast_backprojection.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/src/_fast_morphology.pyx` & `imops-0.7.4/imops/src/_fast_morphology.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/src/_fast_numeric.pyx` & `imops-0.7.4/imops/src/_fast_numeric.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/src/_fast_radon.pyx` & `imops-0.7.4/imops/src/_fast_radon.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/src/_fast_zoom.pyx` & `imops-0.7.4/imops/src/_fast_zoom.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/src/_morphology.pyx` & `imops-0.7.4/imops/src/_morphology.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/src/_numba_zoom.py` & `imops-0.7.4/imops/src/_numba_zoom.py`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/src/_numeric.pyx` & `imops-0.7.4/imops/src/_numeric.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/src/_radon.pyx` & `imops-0.7.4/imops/src/_radon.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/src/_zoom.pyx` & `imops-0.7.4/imops/src/_zoom.pyx`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/testing.py` & `imops-0.7.4/imops/testing.py`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/utils.py` & `imops-0.7.4/imops/utils.py`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops/zoom.py` & `imops-0.7.4/imops/zoom.py`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/imops.egg-info/PKG-INFO` & `imops-0.7.4/imops.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,54 +1,30 @@
 Metadata-Version: 2.1
 Name: imops
-Version: 0.7.3
+Version: 0.7.4
 Summary: Efficient parallelizable algorithms for multidimensional arrays to speed up your data pipelines
 Home-page: https://github.com/neuro-ml/imops
-Download-URL: https://github.com/neuro-ml/imops/archive/v0.7.3.tar.gz
 Author: maxme1, vovaf709, talgat
-Author-email: maxme1 <maxs987@gmail.com>, vovaf709 <vovaf709@yandex.ru>, talgat <saparov2130@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2022 NeuroML
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/neuro-ml/imops
-Project-URL: Issues, https://github.com/neuro-ml/imops/issues
-Project-URL: Source, https://github.com/neuro-ml/imops
-Project-URL: Docs, https://neuro-ml.github.io/imops
+Author-email: maxs987@gmail.com, vovaf709@yandex.ru, saparov2130@gmail.com
+License: MIT
+Download-URL: https://github.com/neuro-ml/imops/archive/v0.7.4.tar.gz
 Keywords: image processing,fast,ndarray,data pipelines
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: numba
 Provides-Extra: all
+Provides-Extra: numba
 License-File: LICENSE
 
 [![codecov](https://codecov.io/gh/neuro-ml/imops/branch/master/graph/badge.svg)](https://codecov.io/gh/neuro-ml/imops)
 [![pypi](https://img.shields.io/pypi/v/imops?logo=pypi&label=PyPi)](https://pypi.org/project/imops/)
 ![License](https://img.shields.io/github/license/neuro-ml/imops)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/imops)](https://pypi.org/project/imops/)
 
@@ -164,7 +140,9 @@
 | `binary_opening`  | &check; | &check; | &cross; |
 
 # Acknowledgements
 
 Some parts of our code for radon/inverse radon transform as well as the code for linear interpolation are inspired by
 the implementations from [`scikit-image`](https://github.com/scikit-image/scikit-image) and [`scipy`](https://github.com/scipy/scipy).
 Also we used [`fastremap`](https://github.com/seung-lab/fastremap) and [`cc3d`](https://github.com/seung-lab/connected-components-3d) out of the box.
+
+
```

### Comparing `imops-0.7.3/imops.egg-info/SOURCES.txt` & `imops-0.7.4/imops.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 imops/_numeric.py
 imops/backend.py
 imops/crop.py
 imops/interp1d.py
 imops/measure.py
 imops/morphology.py
 imops/pad.py
-imops/py.typed
 imops/radon.py
 imops/testing.py
 imops/utils.py
 imops/zoom.py
 imops.egg-info/PKG-INFO
 imops.egg-info/SOURCES.txt
 imops.egg-info/dependency_links.txt
```

### Comparing `imops-0.7.3/pyproject.toml` & `imops-0.7.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `imops-0.7.3/setup.py` & `imops-0.7.4/setup.py`

 * *Files identical despite different names*

