# Comparing `tmp/betanegbinfit-1.8.2.tar.gz` & `tmp/betanegbinfit-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betanegbinfit-1.8.2.tar", last modified: Sat Apr 15 17:19:59 2023, max compression
+gzip compressed data, was "betanegbinfit-1.8.3.tar", last modified: Sat Apr 15 17:29:25 2023, max compression
```

## Comparing `betanegbinfit-1.8.2.tar` & `betanegbinfit-1.8.3.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-04-15 17:19:59.213814 betanegbinfit-1.8.2/
--rw-r--r--   0 georgy    (1000) georgy    (1001)     4054 2023-04-15 17:19:59.213814 betanegbinfit-1.8.2/PKG-INFO
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3534 2022-01-12 15:51:26.000000 betanegbinfit-1.8.2/README.md
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-04-15 17:19:59.213814 betanegbinfit-1.8.2/betanegbinfit/
--rw-r--r--   0 georgy    (1000) georgy    (1001)      739 2023-04-15 17:17:28.000000 betanegbinfit-1.8.2/betanegbinfit/__init__.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)       46 2023-04-15 17:17:43.000000 betanegbinfit-1.8.2/betanegbinfit/__version__.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14720 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/betacdnb.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     2534 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/betainc.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     5146 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/bridge_mixalime.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     6146 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/cdnb.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     5148 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/combine.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14940 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/create.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    32670 2023-04-04 13:54:13.000000 betanegbinfit-1.8.2/betanegbinfit/distributions.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3125 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/hyp.py
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-04-15 17:19:59.213814 betanegbinfit-1.8.2/betanegbinfit/models/
--rw-r--r--   0 georgy    (1000) georgy    (1001)      258 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/models/__init__.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    15251 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/models/model.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    22116 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/models/model_line.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     3341 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/models/model_line_lrt.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14364 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/models/model_mixture.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     8477 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/models/model_mixtures.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    29845 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/models/model_window.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    13557 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/plot.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    14689 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/stats.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)     6960 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/tests.py
--rw-r--r--   0 georgy    (1000) georgy    (1001)    29604 2023-03-30 18:19:57.000000 betanegbinfit-1.8.2/betanegbinfit/utils.py
-drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-04-15 17:19:59.213814 betanegbinfit-1.8.2/betanegbinfit.egg-info/
--rw-r--r--   0 georgy    (1000) georgy    (1001)     4054 2023-04-15 17:19:59.000000 betanegbinfit-1.8.2/betanegbinfit.egg-info/PKG-INFO
--rw-r--r--   0 georgy    (1000) georgy    (1001)      806 2023-04-15 17:19:59.000000 betanegbinfit-1.8.2/betanegbinfit.egg-info/SOURCES.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)        1 2023-04-15 17:19:59.000000 betanegbinfit-1.8.2/betanegbinfit.egg-info/dependency_links.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       43 2023-04-15 17:19:59.000000 betanegbinfit-1.8.2/betanegbinfit.egg-info/requires.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       14 2023-04-15 17:19:59.000000 betanegbinfit-1.8.2/betanegbinfit.egg-info/top_level.txt
--rw-r--r--   0 georgy    (1000) georgy    (1001)       38 2023-04-15 17:19:59.213814 betanegbinfit-1.8.2/setup.cfg
--rw-r--r--   0 georgy    (1000) georgy    (1001)      924 2023-04-15 17:18:42.000000 betanegbinfit-1.8.2/setup.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-04-15 17:29:25.317374 betanegbinfit-1.8.3/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     4054 2023-04-15 17:29:25.317374 betanegbinfit-1.8.3/PKG-INFO
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3534 2022-01-12 15:51:26.000000 betanegbinfit-1.8.3/README.md
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-04-15 17:29:25.317374 betanegbinfit-1.8.3/betanegbinfit/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      725 2023-04-15 17:27:02.000000 betanegbinfit-1.8.3/betanegbinfit/__init__.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14720 2023-03-30 18:19:57.000000 betanegbinfit-1.8.3/betanegbinfit/betacdnb.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     2534 2023-03-30 18:19:57.000000 betanegbinfit-1.8.3/betanegbinfit/betainc.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     5146 2023-03-30 18:19:57.000000 betanegbinfit-1.8.3/betanegbinfit/bridge_mixalime.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     6146 2023-03-30 18:19:57.000000 betanegbinfit-1.8.3/betanegbinfit/cdnb.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     5148 2023-03-30 18:19:57.000000 betanegbinfit-1.8.3/betanegbinfit/combine.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14940 2023-03-30 18:19:57.000000 betanegbinfit-1.8.3/betanegbinfit/create.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    32670 2023-04-04 13:54:13.000000 betanegbinfit-1.8.3/betanegbinfit/distributions.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3125 2023-03-30 18:19:57.000000 betanegbinfit-1.8.3/betanegbinfit/hyp.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-04-15 17:29:25.317374 betanegbinfit-1.8.3/betanegbinfit/models/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      258 2023-03-30 18:19:57.000000 betanegbinfit-1.8.3/betanegbinfit/models/__init__.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    15251 2023-03-30 18:19:57.000000 betanegbinfit-1.8.3/betanegbinfit/models/model.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    22116 2023-03-30 18:19:57.000000 betanegbinfit-1.8.3/betanegbinfit/models/model_line.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     3341 2023-03-30 18:19:57.000000 betanegbinfit-1.8.3/betanegbinfit/models/model_line_lrt.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14364 2023-03-30 18:19:57.000000 betanegbinfit-1.8.3/betanegbinfit/models/model_mixture.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     8477 2023-03-30 18:19:57.000000 betanegbinfit-1.8.3/betanegbinfit/models/model_mixtures.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    29845 2023-03-30 18:19:57.000000 betanegbinfit-1.8.3/betanegbinfit/models/model_window.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    13557 2023-03-30 18:19:57.000000 betanegbinfit-1.8.3/betanegbinfit/plot.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    14689 2023-03-30 18:19:57.000000 betanegbinfit-1.8.3/betanegbinfit/stats.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     6960 2023-03-30 18:19:57.000000 betanegbinfit-1.8.3/betanegbinfit/tests.py
+-rw-r--r--   0 georgy    (1000) georgy    (1001)    29604 2023-03-30 18:19:57.000000 betanegbinfit-1.8.3/betanegbinfit/utils.py
+drwxr-xr-x   0 georgy    (1000) georgy    (1001)        0 2023-04-15 17:29:25.317374 betanegbinfit-1.8.3/betanegbinfit.egg-info/
+-rw-r--r--   0 georgy    (1000) georgy    (1001)     4054 2023-04-15 17:29:25.000000 betanegbinfit-1.8.3/betanegbinfit.egg-info/PKG-INFO
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      777 2023-04-15 17:29:25.000000 betanegbinfit-1.8.3/betanegbinfit.egg-info/SOURCES.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)        1 2023-04-15 17:29:25.000000 betanegbinfit-1.8.3/betanegbinfit.egg-info/dependency_links.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       43 2023-04-15 17:29:25.000000 betanegbinfit-1.8.3/betanegbinfit.egg-info/requires.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       14 2023-04-15 17:29:25.000000 betanegbinfit-1.8.3/betanegbinfit.egg-info/top_level.txt
+-rw-r--r--   0 georgy    (1000) georgy    (1001)       38 2023-04-15 17:29:25.317374 betanegbinfit-1.8.3/setup.cfg
+-rw-r--r--   0 georgy    (1000) georgy    (1001)      964 2023-04-15 17:28:58.000000 betanegbinfit-1.8.3/setup.py
```

### Comparing `betanegbinfit-1.8.2/PKG-INFO` & `betanegbinfit-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betanegbinfit
-Version: 1.8.2
+Version: 1.8.3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `betanegbinfit-1.8.2/README.md` & `betanegbinfit-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.2/betanegbinfit/__init__.py` & `betanegbinfit-1.8.3/betanegbinfit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .__version__ import __version__
+__version__ == '1.8.3'
 import warnings
 # This will omit annoying FutureWarnings by JAX and RutimeWarnings caused by
 # estimates being clipped at bounds.
 warnings.simplefilter(action='ignore', category=FutureWarning)
 warnings.simplefilter(action='ignore', category=RuntimeWarning)
```

### Comparing `betanegbinfit-1.8.2/betanegbinfit/betacdnb.py` & `betanegbinfit-1.8.3/betanegbinfit/betacdnb.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.2/betanegbinfit/betainc.py` & `betanegbinfit-1.8.3/betanegbinfit/betainc.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.2/betanegbinfit/bridge_mixalime.py` & `betanegbinfit-1.8.3/betanegbinfit/bridge_mixalime.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.2/betanegbinfit/cdnb.py` & `betanegbinfit-1.8.3/betanegbinfit/cdnb.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.2/betanegbinfit/combine.py` & `betanegbinfit-1.8.3/betanegbinfit/combine.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.2/betanegbinfit/create.py` & `betanegbinfit-1.8.3/betanegbinfit/create.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.2/betanegbinfit/distributions.py` & `betanegbinfit-1.8.3/betanegbinfit/distributions.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.2/betanegbinfit/hyp.py` & `betanegbinfit-1.8.3/betanegbinfit/hyp.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.2/betanegbinfit/models/model.py` & `betanegbinfit-1.8.3/betanegbinfit/models/model.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.2/betanegbinfit/models/model_line.py` & `betanegbinfit-1.8.3/betanegbinfit/models/model_line.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.2/betanegbinfit/models/model_line_lrt.py` & `betanegbinfit-1.8.3/betanegbinfit/models/model_line_lrt.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.2/betanegbinfit/models/model_mixture.py` & `betanegbinfit-1.8.3/betanegbinfit/models/model_mixture.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.2/betanegbinfit/models/model_mixtures.py` & `betanegbinfit-1.8.3/betanegbinfit/models/model_mixtures.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.2/betanegbinfit/models/model_window.py` & `betanegbinfit-1.8.3/betanegbinfit/models/model_window.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.2/betanegbinfit/plot.py` & `betanegbinfit-1.8.3/betanegbinfit/plot.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.2/betanegbinfit/stats.py` & `betanegbinfit-1.8.3/betanegbinfit/stats.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.2/betanegbinfit/tests.py` & `betanegbinfit-1.8.3/betanegbinfit/tests.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.2/betanegbinfit/utils.py` & `betanegbinfit-1.8.3/betanegbinfit/utils.py`

 * *Files identical despite different names*

### Comparing `betanegbinfit-1.8.2/betanegbinfit.egg-info/PKG-INFO` & `betanegbinfit-1.8.3/betanegbinfit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betanegbinfit
-Version: 1.8.2
+Version: 1.8.3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `betanegbinfit-1.8.2/betanegbinfit.egg-info/SOURCES.txt` & `betanegbinfit-1.8.3/betanegbinfit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 README.md
 setup.py
 betanegbinfit/__init__.py
-betanegbinfit/__version__.py
 betanegbinfit/betacdnb.py
 betanegbinfit/betainc.py
 betanegbinfit/bridge_mixalime.py
 betanegbinfit/cdnb.py
 betanegbinfit/combine.py
 betanegbinfit/create.py
 betanegbinfit/distributions.py
```

### Comparing `betanegbinfit-1.8.2/setup.py` & `betanegbinfit-1.8.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from setuptools import setup, find_packages
-from betanegbinfit.__version__ import __version__
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
+with open('betanegbinfit/__init__.py', 'r') as f:
+    ver = next(f).split('==')[1].strip()[1:-1]
+
 setup(	
       install_requires=['scipy', 'numpy', 'pandas', 'jax', 'jaxlib', 'gmpy2', 'mpmath'],
       include_package_data=True,
       name="betanegbinfit",
-      version=__version__,
+      version=ver,
       long_description=long_description,
       long_description_content_type="text/markdown",
       packages=find_packages(),
       python_requires=">=3.7",
       classifiers=[
               "Programming Language :: Python :: 3.7",
 	      "Programming Language :: Python :: 3.8",
```

