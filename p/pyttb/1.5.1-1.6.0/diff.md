# Comparing `tmp/pyttb-1.5.1.tar.gz` & `tmp/pyttb-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyttb-1.5.1.tar", last modified: Fri Apr 14 21:56:23 2023, max compression
+gzip compressed data, was "pyttb-1.6.0.tar", last modified: Sun Apr 16 15:18:22 2023, max compression
```

## Comparing `pyttb-1.5.1.tar` & `pyttb-1.6.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:56:23.045105 pyttb-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-14 21:56:00.000000 pyttb-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-14 21:56:23.045105 pyttb-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-14 21:56:00.000000 pyttb-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:56:23.041105 pyttb-1.5.1/pyttb/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/cp_als.py
--rw-r--r--   0 runner    (1001) docker     (123)    58614 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/cp_apr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/export_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/hosvd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/import_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/khatrirao.py
--rw-r--r--   0 runner    (1001) docker     (123)    75671 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/ktensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20771 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/pyttb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/sptenmat.py
--rw-r--r--   0 runner    (1001) docker     (123)    90402 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/sptensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/sptensor3.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/sumtensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/symktensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/symtensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14833 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/tenmat.py
--rw-r--r--   0 runner    (1001) docker     (123)    57312 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17952 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/ttensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-04-14 21:56:00.000000 pyttb-1.5.1/pyttb/tucker_als.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:56:23.041105 pyttb-1.5.1/pyttb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-14 21:56:23.000000 pyttb-1.5.1/pyttb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-14 21:56:23.000000 pyttb-1.5.1/pyttb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:56:23.000000 pyttb-1.5.1/pyttb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-14 21:56:23.000000 pyttb-1.5.1/pyttb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 21:56:23.000000 pyttb-1.5.1/pyttb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 21:56:23.045105 pyttb-1.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:56:23.045105 pyttb-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_cp_als.py
--rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_cp_apr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_hosvd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_import_export_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_khatrirao.py
--rw-r--r--   0 runner    (1001) docker     (123)    43374 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_ktensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_packaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    16303 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_pyttb_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    66581 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_sptensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    27857 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_tenmat.py
--rw-r--r--   0 runner    (1001) docker     (123)    55950 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13716 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_ttensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-14 21:56:00.000000 pyttb-1.5.1/tests/test_tucker_als.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:18:22.839779 pyttb-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-16 15:18:04.000000 pyttb-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-16 15:18:22.839779 pyttb-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-16 15:18:04.000000 pyttb-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:18:22.835779 pyttb-1.6.0/pyttb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/cp_als.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58614 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/cp_apr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/export_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/hosvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/import_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/khatrirao.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75831 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/ktensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21784 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/pyttb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/sptenmat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91144 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/sptensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/sptensor3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/sumtensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/symktensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/symtensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14833 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/tenmat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58044 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18305 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/ttensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-16 15:18:04.000000 pyttb-1.6.0/pyttb/tucker_als.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:18:22.835779 pyttb-1.6.0/pyttb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-16 15:18:22.000000 pyttb-1.6.0/pyttb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-04-16 15:18:22.000000 pyttb-1.6.0/pyttb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 15:18:22.000000 pyttb-1.6.0/pyttb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-16 15:18:22.000000 pyttb-1.6.0/pyttb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-16 15:18:22.000000 pyttb-1.6.0/pyttb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 15:18:22.839779 pyttb-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 15:18:22.839779 pyttb-1.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_cp_als.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19970 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_cp_apr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_hosvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_import_export_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_khatrirao.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43526 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_ktensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16756 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_pyttb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66728 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_sptensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27857 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_tenmat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56534 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14067 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_ttensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-04-16 15:18:04.000000 pyttb-1.6.0/tests/test_tucker_als.py
```

### Comparing `pyttb-1.5.1/LICENSE` & `pyttb-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.1/PKG-INFO` & `pyttb-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: pyttb
-Version: 1.5.1
+Version: 1.6.0
 Summary: Python Tensor Toolbox
-Author: Nick Johnson
 Author-email: "Daniel M. Dunlavy" <dmdunla@sandia.gov>
 License: BSD 2-Clause License
 Project-URL: homepage, https://github.com/sandialabs/pyttb
 Project-URL: coverage, https://coveralls.io/github/sandialabs/pyttb
 Project-URL: documentation, https://pyttb.readthedocs.io
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyttb-1.5.1/README.md` & `pyttb-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.1/pyproject.toml` & `pyttb-1.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [project]
 name = "pyttb"
 dynamic = ["version"]
 description = "Python Tensor Toolbox"
 authors = [
   {name="Daniel M. Dunlavy", email="dmdunla@sandia.gov"},
-  {name="Nick Johnson"},
 ]
 license = { text="BSD 2-Clause License" }
 readme = "README.md"
 requires-python = ">=3.8"
 
 dependencies = [
     "numpy",
```

### Comparing `pyttb-1.5.1/pyttb/__init__.py` & `pyttb-1.6.0/pyttb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright 2022 National Technology & Engineering Solutions of Sandia,
 # LLC (NTESS). Under the terms of Contract DE-NA0003525 with NTESS, the
 # U.S. Government retains certain rights in this software.
 
-__version__ = "1.5.1"
+__version__ = "1.6.0"
 
 import warnings
 
 from pyttb.cp_als import cp_als
 from pyttb.cp_apr import *
 from pyttb.export_data import export_data
 from pyttb.hosvd import hosvd
```

### Comparing `pyttb-1.5.1/pyttb/cp_als.py` & `pyttb-1.6.0/pyttb/cp_als.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.1/pyttb/cp_apr.py` & `pyttb-1.6.0/pyttb/cp_apr.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.1/pyttb/export_data.py` & `pyttb-1.6.0/pyttb/export_data.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.1/pyttb/hosvd.py` & `pyttb-1.6.0/pyttb/hosvd.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.1/pyttb/import_data.py` & `pyttb-1.6.0/pyttb/import_data.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.1/pyttb/khatrirao.py` & `pyttb-1.6.0/pyttb/khatrirao.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.1/pyttb/ktensor.py` & `pyttb-1.6.0/pyttb/ktensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1788,15 +1788,15 @@
         #
         # for f in self.factor_matrices:
         #     for r in range(self.ncomponents):
         #         x[offset:offset+f.shape[0]] = f[:, r].reshape((f.shape[0], 1))
         #         offset += f.shape[0]
         return x
 
-    def ttv(self, vector, dims=None):
+    def ttv(self, vector, dims=None, exclude_dims=None):
         """
         `Tensor` times vector for `ktensors`.
 
         Computes the product of a `ktensor` with a vector.  If `dims` is an integer, it specifies
         the dimension in the `ktensor` along which the vector is multiplied.  If the shape of the vector
         is = (I,1), then the size of dimension `dims` of the `ktensor` must have size I.  Note that
         number of dimensions of the returned `tensor` is 1 less than the dimension of the `ktensor` used
@@ -1829,15 +1829,15 @@
 
         >>> rank = 2
         >>> shape = np.array([2, 3, 4])
         >>> data = np.arange(1, rank*sum(shape)+1)
         >>> weights = 2 * np.ones(rank)
         >>> weights_and_data = np.concatenate((weights, data), axis=0)
         >>> K = ttb.ktensor.from_vector(weights_and_data[:], shape, True)
-        >>> K0 = K.ttv(np.array([1, 1, 1]), dims=1) # compute along a single dimension
+        >>> K0 = K.ttv(np.array([1, 1, 1]),dims=1) # compute along a single dimension
         >>> print(K0)
         ktensor of shape 2 x 4
         weights=[36. 54.]
         factor_matrices[0] =
         [[1. 3.]
          [2. 4.]]
         factor_matrices[1] =
@@ -1853,34 +1853,37 @@
         >>> vec4 = np.array([1, 1, 1, 1])
         >>> K1 = K.ttv([vec2, vec3, vec4])
         >>> print(K1)
         30348.0
 
         Compute the product of a `ktensor` and multiple vectors out of order (results in a `ktensor`):
 
-        >>> K2 = K.ttv([vec4, vec3], np.array([2, 1]))
+        >>> K2 = K.ttv([vec4, vec3],np.array([2, 1]))
         >>> print(K2)
         ktensor of shape 2
         weights=[1800. 3564.]
         factor_matrices[0] =
         [[1. 3.]
          [2. 4.]]
         """
 
-        if dims is None:
+        if dims is None and exclude_dims is None:
             dims = np.array([])
         elif isinstance(dims, (float, int)):
             dims = np.array([dims])
 
+        if isinstance(exclude_dims, (float, int)):
+            exclude_dims = np.array([exclude_dims])
+
         # Check that vector is a list of vectors, if not place single vector as element in list
         if len(vector) > 0 and isinstance(vector[0], (int, float, np.int_, np.float_)):
             return self.ttv([vector], dims)
 
         # Get sorted dims and index for multiplicands
-        dims, vidx = ttb.tt_dimscheck(dims, self.ndims, len(vector))
+        dims, vidx = ttb.tt_dimscheck(self.ndims, len(vector), dims, exclude_dims)
 
         # Check that each multiplicand is the right size.
         for i in range(dims.size):
             if vector[vidx[i]].shape != (self.shape[dims[i]],):
                 assert False, "Multiplicand is wrong size"
 
         # Figure out which dimensions will be left when we're done
```

### Comparing `pyttb-1.5.1/pyttb/pyttb_utils.py` & `pyttb-1.6.0/pyttb/pyttb_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,54 +110,86 @@
     union = np.vstack(
         (MatrixB[np.sort(idxB[np.where(location < 0)])], MatrixA[np.sort(idxA)])
     )
     return union
 
 
 @overload
-def tt_dimscheck(dims: np.ndarray, N: int, M: None = None) -> Tuple[np.ndarray, None]:
+def tt_dimscheck(
+    N: int,
+    M: None = None,
+    dims: Optional[np.ndarray] = None,
+    exclude_dims: Optional[np.ndarray] = None,
+) -> Tuple[np.ndarray, None]:
     ...  # pragma: no cover see coveragepy/issues/970
 
 
 @overload
-def tt_dimscheck(dims: np.ndarray, N: int, M: int) -> Tuple[np.ndarray, np.ndarray]:
+def tt_dimscheck(
+    N: int,
+    M: int,
+    dims: Optional[np.ndarray] = None,
+    exclude_dims: Optional[np.ndarray] = None,
+) -> Tuple[np.ndarray, np.ndarray]:
     ...  # pragma: no cover see coveragepy/issues/970
 
 
 def tt_dimscheck(
-    dims: np.ndarray, N: int, M: Optional[int] = None
+    N: int,
+    M: Optional[int] = None,
+    dims: Optional[np.ndarray] = None,
+    exclude_dims: Optional[np.ndarray] = None,
 ) -> Tuple[np.ndarray, Optional[np.ndarray]]:
     """
     Used to preprocess dimensions for tensor dimensions
 
     Parameters
     ----------
 
     Returns
     -------
 
     """
-    # Fix empty case
-    if dims.size == 0:
-        dims = np.arange(0, N)
+    if dims is not None and exclude_dims is not None:
+        raise ValueError("Either specify dims to include or exclude, but not both")
 
-    # Fix "minus" case
-    if np.max(dims) < 0:
+    dim_array: np.ndarray = np.empty((1,))
+
+    # Explicit exclude to resolve ambiguous -0
+    if exclude_dims is not None:
         # Check that all members in range
-        if not np.all(np.isin(-dims, np.arange(0, N + 1))):
-            assert False, "Invalid magnitude for negative dims selection"
-        dims = np.setdiff1d(np.arange(1, N + 1), -dims) - 1
+        valid_indices = np.isin(exclude_dims, np.arange(0, N))
+        if not np.all(valid_indices):
+            invalid_indices = np.logical_not(valid_indices)
+            raise ValueError(
+                f"Exclude dims provided: {exclude_dims} "
+                f"but, {exclude_dims[invalid_indices]} were out of valid range"
+                f"[0,{N}]"
+            )
+        dim_array = np.setdiff1d(np.arange(0, N), exclude_dims)
+
+    # Fix empty case
+    if (dims is None or dims.size == 0) and exclude_dims is None:
+        dim_array = np.arange(0, N)
+    elif isinstance(dims, np.ndarray):
+        dim_array = dims
+
+    # Catch minus case to avoid silent errors
+    if np.any(dim_array < 0):
+        raise ValueError(
+            "Negative dims aren't allowed in pyttb, see exclude_dims argument instead"
+        )
 
     # Save dimensions of dims
-    P = len(dims)
+    P = len(dim_array)
 
     # Reorder dims from smallest to largest (this matters in particular for the vector
     # multiplicand case, where the order affects the result)
-    sidx = np.argsort(dims)
-    sdims = dims[sidx]
+    sidx = np.argsort(dim_array)
+    sdims = dim_array[sidx]
     vidx = None
 
     if M is not None:
         # Can't have more multiplicands than dimensions
         if M > N:
             assert False, "Cannot have more multiplicands than dimensions"
```

### Comparing `pyttb-1.5.1/pyttb/sptensor.py` & `pyttb-1.6.0/pyttb/sptensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -378,15 +378,15 @@
         2
         >>> X.collapse(np.arange(X.ndims), sum)
         2
         """
         if dims is None:
             dims = np.arange(0, self.ndims)
 
-        dims, _ = tt_dimscheck(dims, self.ndims)
+        dims, _ = tt_dimscheck(self.ndims, dims=dims)
         remdims = np.setdiff1d(np.arange(0, self.ndims), dims)
 
         # Check for the case where we accumulate over *all* dimensions
         if remdims.size == 0:
             return fun(self.vals.transpose()[0])
 
         # Calculate the size of the result
@@ -878,15 +878,15 @@
             Z = []
             for i in range(N):
                 if i != n:
                     Z.append(U[i][:, r])
                 else:
                     Z.append(np.array([]))
             # Perform ttv multiplication
-            V[:, r] = self.ttv(Z, -(n + 1)).double()
+            V[:, r] = self.ttv(Z, exclude_dims=n).double()
 
         return V
 
     @property
     def ndims(self) -> int:
         """
         NDIMS Number of dimensions of a sparse tensor.
@@ -1040,15 +1040,15 @@
 
         Returns
         -------
         :class:`pyttb.sptensor`
         """
         if isinstance(dims, (float, int)):
             dims = np.array([dims])
-        dims, _ = ttb.tt_dimscheck(dims, self.ndims)
+        dims, _ = ttb.tt_dimscheck(self.ndims, dims=dims)
 
         if isinstance(factor, ttb.tensor):
             shapeArray = np.array(self.shape)
             if np.any(factor.shape != shapeArray[dims]):
                 assert False, "Size mismatch in scale"
             return ttb.sptensor.from_data(
                 self.subs,
@@ -1177,36 +1177,41 @@
         return loc
 
     # pylint: disable=too-many-branches, too-many-locals
     def ttv(
         self,
         vector: Union[np.ndarray, List[np.ndarray]],
         dims: Optional[Union[int, np.ndarray]] = None,
+        exclude_dims: Optional[Union[int, np.ndarray]] = None,
     ) -> Union[sptensor, ttb.tensor]:
         """
         Sparse tensor times vector
 
         Parameters
         ----------
         vector: Vector(s) to multiply against
         dims: Dimensions to multiply with vector(s)
+        exclude_dims: Use all dimensions but these
         """
 
-        if dims is None:
+        if dims is None and exclude_dims is None:
             dims = np.array([])
         elif isinstance(dims, (float, int)):
             dims = np.array([dims])
 
+        if isinstance(exclude_dims, (float, int)):
+            exclude_dims = np.array([exclude_dims])
+
         # Check that vector is a list of vectors,
         # if not place single vector as element in list
         if len(vector) > 0 and isinstance(vector[0], (int, float, np.int_, np.float_)):
-            return self.ttv(np.array([vector]), dims)
+            return self.ttv(np.array([vector]), dims, exclude_dims)
 
         # Get sorted dims and index for multiplicands
-        dims, vidx = ttb.tt_dimscheck(dims, self.ndims, len(vector))
+        dims, vidx = ttb.tt_dimscheck(self.ndims, len(vector), dims, exclude_dims)
         remdims = np.setdiff1d(np.arange(0, self.ndims), dims).astype(int)
 
         # Check that each multiplicand is the right size.
         for i in range(dims.size):
             if vector[vidx[i]].shape != (self.shape[dims[i]],):
                 assert False, "Multiplicand is wrong size"
 
@@ -2491,54 +2496,63 @@
 
     __str__ = __repr__
 
     def ttm(
         self,
         matrices: Union[np.ndarray, List[np.ndarray]],
         dims: Optional[Union[float, np.ndarray]] = None,
+        exclude_dims: Optional[Union[float, np.ndarray]] = None,
         transpose: bool = False,
     ):
         """
         Sparse tensor times matrix.
 
         Parameters
         ----------
         matrices: A matrix or list of matrices
-        dims: :class:`Numpy.ndarray`, int
+        dims: Dimensions to multiply against
+        exclude_dims: Use all dimensions but these
         transpose: Transpose matrices to be multiplied
 
         Returns
         -------
 
         """
-        if dims is None:
+        if dims is None and exclude_dims is None:
             dims = np.arange(self.ndims)
         elif isinstance(dims, list):
             dims = np.array(dims)
         elif isinstance(dims, (float, int, np.generic)):
             dims = np.array([dims])
 
+        if isinstance(exclude_dims, (float, int)):
+            exclude_dims = np.array([exclude_dims])
+
         # Handle list of matrices
         if isinstance(matrices, list):
             # Check dimensions are valid
-            [dims, vidx] = tt_dimscheck(dims, self.ndims, len(matrices))
+            [dims, vidx] = tt_dimscheck(self.ndims, len(matrices), dims, exclude_dims)
             # Calculate individual products
             Y = self.ttm(matrices[vidx[0]], dims[0], transpose=transpose)
             for i in range(1, dims.size):
                 Y = Y.ttm(matrices[vidx[i]], dims[i], transpose=transpose)
             return Y
 
         # Check matrices
         if len(matrices.shape) != 2:
             assert False, "Sptensor.ttm: second argument must be a matrix"
 
         # Flip matrices if transposed
         if transpose:
             matrices = matrices.transpose()
 
+        # FIXME: This made typing happy but shouldn't be possible
+        if not isinstance(dims, np.ndarray):  # pragma: no cover
+            raise ValueError("Dims should be an array here")
+
         # Ensure this is the terminal single dimension case
         if not (dims.size == 1 and np.isin(dims, np.arange(self.ndims))):
             assert False, "dims must contain values in [0,self.dims)"
         final_dim: int = dims[0]
 
         # Compute the product
```

### Comparing `pyttb-1.5.1/pyttb/sumtensor.py` & `pyttb-1.6.0/pyttb/sumtensor.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.1/pyttb/tenmat.py` & `pyttb-1.6.0/pyttb/tenmat.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.1/pyttb/tensor.py` & `pyttb-1.6.0/pyttb/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,15 @@
 
         if dims is None:
             dims = np.arange(0, self.ndims)
 
         if dims.size == 0:
             return ttb.tensor.from_tensor_type(self)
 
-        dims, _ = tt_dimscheck(dims, self.ndims)
+        dims, _ = tt_dimscheck(self.ndims, dims=dims)
         remdims = np.setdiff1d(np.arange(0, self.ndims), dims)
 
         # Check for the case where we accumulate over *all* dimensions
         if remdims.size == 0:
             return fun(self.data.flatten("F"))
 
         ## Calculate the shape of the result
@@ -1018,56 +1018,65 @@
 
             return Y
 
     def ttm(
         self,
         matrix: Union[np.ndarray, List[np.ndarray]],
         dims: Optional[Union[float, np.ndarray]] = None,
+        exclude_dims: Optional[Union[int, np.ndarray]] = None,
         transpose: bool = False,
     ) -> tensor:
         """
         Tensor times matrix
 
         Parameters
         ----------
         matrix: Matrix or matrices to multiple by
         dims: Dimensions to multiply against
+        exclude_dims: Use all dimensions but these
         transpose: Transpose matrices during multiplication
         """
-
-        if dims is None:
+        if dims is None and exclude_dims is None:
             dims = np.arange(self.ndims)
         elif isinstance(dims, list):
             dims = np.array(dims)
         elif isinstance(dims, (float, int, np.generic)):
             dims = np.array([dims])
 
+        if isinstance(exclude_dims, (float, int)):
+            exclude_dims = np.array([exclude_dims])
+
         if isinstance(matrix, list):
             # Check that the dimensions are valid
-            dims, vidx = ttb.tt_dimscheck(dims, self.ndims, len(matrix))
+            dims, vidx = ttb.tt_dimscheck(self.ndims, len(matrix), dims, exclude_dims)
 
             # Calculate individual products
-            Y = self.ttm(matrix[vidx[0]], dims[0], transpose)
+            Y = self.ttm(matrix[vidx[0]], dims[0], transpose=transpose)
             for k in range(1, dims.size):
-                Y = Y.ttm(matrix[vidx[k]], dims[k], transpose)
+                Y = Y.ttm(matrix[vidx[k]], dims[k], transpose=transpose)
             return Y
 
         if not isinstance(matrix, np.ndarray):
             assert False, f"matrix must be of type numpy.ndarray but got:\n{matrix}"
 
+        dims, _ = ttb.tt_dimscheck(self.ndims, dims=dims, exclude_dims=exclude_dims)
+
         if not (dims.size == 1 and np.isin(dims, np.arange(self.ndims))):
             assert False, "dims must contain values in [0,self.dims)"
 
         # old version (ver=0)
-        shape = np.array(self.shape)
+        shape = np.array(self.shape, dtype=int)
         n = dims[0]
         order = np.array([n] + list(range(0, n)) + list(range(n + 1, self.ndims)))
         newdata = self.permute(order).data
         ids = np.array(list(range(0, n)) + list(range(n + 1, self.ndims)))
-        newdata = np.reshape(newdata, (shape[n], np.prod(shape[ids])), order="F")
+        second_dim = 1
+        if len(ids) > 0:
+            second_dim = np.prod(shape[ids])
+        newdata = np.reshape(newdata, (shape[n], second_dim), order="F")
         if transpose:
             newdata = matrix.T @ newdata
             p = matrix.shape[1]
         else:
             newdata = matrix @ newdata
             p = matrix.shape[0]
 
@@ -1115,49 +1124,52 @@
             ), f"Specified dimensions do not match got {selfshape} and {othershape}"
 
         # Compute the product
 
         # Avoid transpose by reshaping self and computing result = self * other
         amatrix = ttb.tenmat.from_tensor_type(self, cdims=selfdims)
         bmatrix = ttb.tenmat.from_tensor_type(other, rdims=otherdims)
-        print(amatrix)
-        print(bmatrix)
         cmatrix = amatrix * bmatrix
 
         # Check whether or not the result is a scalar
         if isinstance(cmatrix, ttb.tenmat):
             return ttb.tensor.from_tensor_type(cmatrix)
         return cmatrix
 
     def ttv(
         self,
         vector: Union[np.ndarray, List[np.ndarray]],
         dims: Optional[Union[int, np.ndarray]] = None,
+        exclude_dims: Optional[Union[int, np.ndarray]] = None,
     ) -> tensor:
         """
         Tensor times vector
 
         Parameters
         ----------
         vector: Vector(s) to multiply against
         dims: Dimensions to multiply with vector(s)
+        exclude_dims: Use all dimensions but these
         """
 
-        if dims is None:
+        if dims is None and exclude_dims is None:
             dims = np.array([])
         elif isinstance(dims, (float, int)):
             dims = np.array([dims])
 
+        if isinstance(exclude_dims, (float, int)):
+            exclude_dims = np.array([exclude_dims])
+
         # Check that vector is a list of vectors, if not place single vector as element
         # in list
         if len(vector) > 0 and isinstance(vector[0], (int, float, np.int_, np.float_)):
-            return self.ttv(np.array([vector]), dims)
+            return self.ttv(np.array([vector]), dims, exclude_dims)
 
         # Get sorted dims and index for multiplicands
-        dims, vidx = ttb.tt_dimscheck(dims, self.ndims, len(vector))
+        dims, vidx = ttb.tt_dimscheck(self.ndims, len(vector), dims, exclude_dims)
 
         # Check that each multiplicand is the right size.
         for i in range(dims.size):
             if vector[vidx[i]].shape != (self.shape[dims[i]],):
                 assert False, "Multiplicand is wrong size"
 
         # Extract the data
@@ -1181,47 +1193,47 @@
         if n > 0:
             return ttb.tensor.from_data(c, tuple(sz[0:n]))
         return c[0]
 
     def ttsv(
         self,
         vector: Union[np.ndarray, List[np.ndarray]],
-        dims: Optional[Union[int, np.ndarray]] = None,
+        skip_dim: Optional[int] = None,
         version: Optional[int] = None,
     ) -> Union[np.ndarray, tensor]:
         """
         Tensor times same vector in multiple modes
 
         Parameters
         ----------
         vector: Vector(s) to multiply against
-        dims: Dimensions to multiply by vector(s)
+        skip_dim: Multiply tensor by vector in all dims except [0, skip_dim]
         """
         # Only two simple cases are supported
-        if dims is None:
-            dims = 0
-        elif dims > 0:
-            assert False, "Invalid modes in ttsv"
+        if skip_dim is None:
+            exclude_dims = None
+            skip_dim = -1  # For easier math later
+        elif skip_dim < 0:
+            raise ValueError("Invalid modes in ttsv")
+        else:
+            exclude_dims = np.arange(0, skip_dim + 1)
 
         if version == 1:  # Calculate the old way
             P = self.ndims
             X = np.array([vector for i in range(P)])
-            # pylint: disable=invalid-unary-operand-type
-            if dims == 0:
-                return self.ttv(X)
-            if dims in (-1, -2):  # Return scalar or matrix
-                return (self.ttv(X, -np.arange(1, -dims + 1))).double()
-            return self.ttv(X, -np.arange(1, -dims + 1))
+            if skip_dim in (0, 1):  # Return scalar or matrix
+                return self.ttv(X, exclude_dims=exclude_dims).double()
+            return self.ttv(X, exclude_dims=exclude_dims)
 
         if version == 2 or version is None:  # Calculate the new way
             d = self.ndims
             sz = self.shape[0]  # Sizes of all modes must be the same
 
             # pylint: disable=invalid-unary-operand-type
-            dnew = -dims  # Number of modes in result
+            dnew = skip_dim + 1  # Number of modes in result
             drem = d - dnew  # Number of modes multiplied out
 
             y = self.data
             for i in range(drem, 0, -1):
                 yy = np.reshape(y, (sz ** (dnew + i - 1), sz), order="F")
                 y = yy.dot(vector)
```

### Comparing `pyttb-1.5.1/pyttb/ttensor.py` & `pyttb-1.6.0/pyttb/ttensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -310,46 +310,49 @@
         -------
         :class:`pyttb.ttensor`
         """
         if isinstance(other, (float, int, np.number)):
             return self.__mul__(other)
         raise ValueError("This object cannot be multiplied by ttensor")
 
-    def ttv(self, vector, dims=None):
+    def ttv(self, vector, dims=None, exclude_dims=None):
         """
         TTensor times vector
 
         Parameters
         ----------
         vector: :class:`Numpy.ndarray`, list[:class:`Numpy.ndarray`]
         dims: :class:`Numpy.ndarray`, int
         """
-        if dims is None:
+        if dims is None and exclude_dims is None:
             dims = np.array([])
         # TODO make helper function to check scalar since re-used many places
         elif isinstance(dims, (float, int)):
             dims = np.array([dims])
 
+        if isinstance(exclude_dims, (float, int)):
+            exclude_dims = np.array([exclude_dims])
+
         # Check that vector is a list of vectors, if not place single vector as element in list
         if len(vector) > 0 and isinstance(vector[0], (int, float, np.int_, np.float_)):
-            return self.ttv(np.array([vector]), dims)
+            return self.ttv(np.array([vector]), dims, exclude_dims)
 
         # Get sorted dims and index for multiplicands
-        dims, vidx = ttb_utils.tt_dimscheck(dims, self.ndims, len(vector))
+        dims, vidx = ttb_utils.tt_dimscheck(self.ndims, len(vector), dims, exclude_dims)
 
         # Check that each multiplicand is the right size.
         for i in range(dims.size):
             if vector[vidx[i]].shape != (self.shape[dims[i]],):
                 raise ValueError("Multiplicand is wrong size")
 
         # Get remaining dimensions when we're done
         remdims = np.setdiff1d(np.arange(0, self.ndims), dims)
 
         # Create W to multiply with core, only populated remaining dims
-        W = [None] * len(dims)
+        W = [None] * self.ndims
         for i in range(dims.size):
             dim_idx = dims[i]
             W[dim_idx] = self.u[dim_idx].transpose().dot(vector[vidx[i]])
 
         # Create new core
         newcore = self.core.ttv(W, dims)
 
@@ -416,38 +419,41 @@
         """
         if not np.array_equal(np.arange(0, self.ndims), np.sort(order)):
             raise ValueError("Invalid permutation")
         new_core = self.core.permute(order)
         new_u = [self.u[idx] for idx in order]
         return ttensor.from_data(new_core, new_u)
 
-    def ttm(self, matrix, dims=None, transpose=False):
+    def ttm(self, matrix, dims=None, exclude_dims=None, transpose=False):
         """
         Tensor times matrix for ttensor
 
         Parameters
         ----------
         matrix: :class:`Numpy.ndarray`, list[:class:`Numpy.ndarray`]
         dims: :class:`Numpy.ndarray`, int
         transpose: bool
         """
-        if dims is None:
+        if dims is None and exclude_dims is None:
             dims = np.arange(self.ndims)
         elif isinstance(dims, list):
             dims = np.array(dims)
         elif np.isscalar(dims):
             if dims < 0:
                 raise ValueError("Negative dims is currently unsupported, see #62")
             dims = np.array([dims])
 
+        if isinstance(exclude_dims, (float, int)):
+            exclude_dims = np.array([exclude_dims])
+
         if not isinstance(matrix, list):
-            return self.ttm([matrix], dims, transpose)
+            return self.ttm([matrix], dims, exclude_dims, transpose)
 
         # Check that the dimensions are valid
-        dims, vidx = ttb_utils.tt_dimscheck(dims, self.ndims, len(matrix))
+        dims, vidx = ttb_utils.tt_dimscheck(self.ndims, len(matrix), dims, exclude_dims)
 
         # Determine correct size index
         size_idx = int(not transpose)
 
         # Check that each multiplicand is the right size.
         for i in range(len(dims)):
             if matrix[vidx[i]].shape[size_idx] != self.shape[dims[i]]:
```

### Comparing `pyttb-1.5.1/pyttb/tucker_als.py` & `pyttb-1.6.0/pyttb/tucker_als.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,25 +120,21 @@
 
     # Main loop: Iterate until convergence
     for iter in range(maxiters):
         fitold = fit
 
         # Iterate over all N modes of the tensor
         for n in dimorder:
-            # TODO proposal to change ttm to include_dims and exclude_dims to resolve -0 ambiguity
-            dims = np.arange(0, tensor.ndims)
-            dims = dims[dims != n]
-            Utilde = tensor.ttm(U, dims, True)
-            print(f"Utilde[{n}] = {Utilde}")
+            Utilde = tensor.ttm(U, exclude_dims=n, transpose=True)
             # Maximize norm(Utilde x_n W') wrt W and
             # maintain orthonormality of W
             U[n] = Utilde.nvecs(n, rank[n])
 
         # Assemble the current approximation
-        core = Utilde.ttm(U, n, True)
+        core = Utilde.ttm(U, n, transpose=True)
 
         # Compute fit
         normresidual = np.sqrt(abs(normX**2 - core.norm() ** 2))
         fit = 1 - (normresidual / normX)  # fraction explained by model
         fitchange = abs(fitold - fit)
 
         if iter % printitn == 0:
```

### Comparing `pyttb-1.5.1/pyttb.egg-info/PKG-INFO` & `pyttb-1.6.0/pyttb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: pyttb
-Version: 1.5.1
+Version: 1.6.0
 Summary: Python Tensor Toolbox
-Author: Nick Johnson
 Author-email: "Daniel M. Dunlavy" <dmdunla@sandia.gov>
 License: BSD 2-Clause License
 Project-URL: homepage, https://github.com/sandialabs/pyttb
 Project-URL: coverage, https://coveralls.io/github/sandialabs/pyttb
 Project-URL: documentation, https://pyttb.readthedocs.io
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyttb-1.5.1/pyttb.egg-info/SOURCES.txt` & `pyttb-1.6.0/pyttb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.1/tests/test_cp_als.py` & `pyttb-1.6.0/tests/test_cp_als.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.1/tests/test_cp_apr.py` & `pyttb-1.6.0/tests/test_cp_apr.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.1/tests/test_hosvd.py` & `pyttb-1.6.0/tests/test_hosvd.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.1/tests/test_import_export_data.py` & `pyttb-1.6.0/tests/test_import_export_data.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.1/tests/test_khatrirao.py` & `pyttb-1.6.0/tests/test_khatrirao.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.1/tests/test_ktensor.py` & `pyttb-1.6.0/tests/test_ktensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1001,14 +1001,19 @@
 
     # Empty dims requires that # vectors == # dimensions
     vec2 = np.array([1, 1])
     vec3 = np.array([1, 1, 1])
     vec4 = np.array([1, 1, 1, 1])
     assert K.ttv([vec2, vec3, vec4]) == 30348
 
+    # Exclude dims should mirror dims
+    assert K.ttv([vec2, vec3], dims=np.array([0, 1])).isequal(
+        K.ttv([vec2, vec3], exclude_dims=2)
+    )
+
     # Wrong shape
     with pytest.raises(AssertionError) as excinfo:
         K.ttv([vec2, vec3, np.array([1, 2])])
     assert "Multiplicand is wrong size" in str(excinfo)
 
     # Multiple dimensions, but fewer than all dimensions, not in same order as ktensor dimensions
     K2 = K.ttv([vec4, vec3], dims=np.array([2, 1]))
```

### Comparing `pyttb-1.5.1/tests/test_package.py` & `pyttb-1.6.0/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.1/tests/test_pyttb_utils.py` & `pyttb-1.6.0/tests/test_pyttb_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,53 +63,63 @@
     assert (ttb.tt_union_rows(a, np.array([])) == a[np.sort(idx)]).all()
     assert (ttb.tt_union_rows(np.array([]), a) == a[np.sort(idx)]).all()
 
 
 @pytest.mark.indevelopment
 def test_tt_dimscheck():
     #  Empty
-    rdims, ridx = ttb.tt_dimscheck(np.array([]), 6)
+    rdims, ridx = ttb.tt_dimscheck(6, dims=np.array([]))
     assert (rdims == np.array([0, 1, 2, 3, 4, 5])).all()
     assert ridx is None
 
-    # Minus
-    rdims, ridx = ttb.tt_dimscheck(np.array([-1]), 6)
-    assert (rdims == np.array([1, 2, 3, 4, 5])).all()
+    # Exclude Dims
+    rdims, ridx = ttb.tt_dimscheck(6, exclude_dims=np.array([1]))
+    assert (rdims == np.array([0, 2, 3, 4, 5])).all()
     assert ridx is None
 
     # Invalid minus
-    with pytest.raises(AssertionError) as excinfo:
-        ttb.tt_dimscheck(np.array([-7]), 6, 6)
-    assert "Invalid magnitude for negative dims selection" in str(excinfo)
+    with pytest.raises(ValueError) as excinfo:
+        ttb.tt_dimscheck(6, 6, exclude_dims=np.array([7]))
+    assert "Exclude dims" in str(excinfo)
 
     # Positive
-    rdims, ridx = ttb.tt_dimscheck(np.array([5]), 6)
+    rdims, ridx = ttb.tt_dimscheck(6, dims=np.array([5]))
     assert (rdims == np.array([5])).all()
     assert ridx is None
 
     # M==P
-    rdims, ridx = ttb.tt_dimscheck(np.array([-1]), 6, 5)
+    rdims, ridx = ttb.tt_dimscheck(6, 5, exclude_dims=np.array([0]))
     assert (rdims == np.array([1, 2, 3, 4, 5])).all()
     assert (ridx == np.arange(0, 5)).all()
 
     # M==N
-    rdims, ridx = ttb.tt_dimscheck(np.array([-1]), 6, 6)
+    rdims, ridx = ttb.tt_dimscheck(6, 6, exclude_dims=np.array([0]))
     assert (rdims == np.array([1, 2, 3, 4, 5])).all()
     assert (ridx == rdims).all()
 
     # M>N
     with pytest.raises(AssertionError) as excinfo:
-        ttb.tt_dimscheck(np.array([-1]), 6, 7)
+        ttb.tt_dimscheck(6, 7, exclude_dims=np.array([0]))
     assert "Cannot have more multiplicands than dimensions" in str(excinfo)
 
     # M!=P and M!=N
     with pytest.raises(AssertionError) as excinfo:
-        ttb.tt_dimscheck(np.array([-1]), 6, 4)
+        ttb.tt_dimscheck(6, 4, exclude_dims=np.array([0]))
     assert "Invalid number of multiplicands" in str(excinfo)
 
+    # Both dims and exclude dims
+    with pytest.raises(ValueError) as excinfo:
+        ttb.tt_dimscheck(6, dims=[], exclude_dims=[])
+    assert "not both" in str(excinfo)
+
+    # We no longer support negative dims. Make sure that is explicit
+    with pytest.raises(ValueError) as excinfo:
+        ttb.tt_dimscheck(6, dims=np.array([-1]))
+    assert "Negative dims" in str(excinfo), f"{str(excinfo)}"
+
 
 @pytest.mark.indevelopment
 def test_tt_tenfun():
     data = np.array([[1, 2, 3], [4, 5, 6]])
     t1 = ttb.tensor.from_data(data)
     t2 = ttb.tensor.from_data(data)
```

### Comparing `pyttb-1.5.1/tests/test_sptensor.py` & `pyttb-1.6.0/tests/test_sptensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1663,14 +1663,17 @@
 
     # This is a multiway multiplication yielding a sparse tensor, yielding a dense tensor relies on tensor.ttm
     matrix = sparse.coo_matrix(np.eye(4))
     list_of_matrices = [matrix, matrix, matrix]
     assert sptensorInstance.ttm(list_of_matrices, dims=[0, 1, 2]).isequal(
         sptensorInstance
     )
+    assert sptensorInstance.ttm(list_of_matrices, exclude_dims=2).isequal(
+        sptensorInstance.ttm(list_of_matrices[0:-1], dims=[0, 1])
+    )
 
     with pytest.raises(AssertionError) as excinfo:
         sptensorInstance.ttm(sparse.coo_matrix(np.ones((5, 5))), dims=0)
     assert "Matrix shape doesn't match tensor shape" in str(excinfo)
 
     with pytest.raises(AssertionError) as excinfo:
         sptensorInstance.ttm(np.array([1, 2, 3, 4]), dims=0)
```

### Comparing `pyttb-1.5.1/tests/test_tenmat.py` & `pyttb-1.6.0/tests/test_tenmat.py`

 * *Files identical despite different names*

### Comparing `pyttb-1.5.1/tests/test_tensor.py` & `pyttb-1.6.0/tests/test_tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1098,15 +1098,15 @@
     T3 = tensorInstance3.ttm(M2, 0, transpose=True)
     assert isinstance(T3, ttb.tensor)
     assert T3.shape == (2, 3, 2)
     data3 = np.array([[[5, 23], [11, 29], [17, 35]], [[11, 53], [25, 67], [39, 81]]])
     assert (T3.data == data3).all()
 
     # 3-way, two matrices, negative dimension
-    T3 = tensorInstance3.ttm([M2, M2], -2)
+    T3 = tensorInstance3.ttm([M2, M2], exclude_dims=1)
     assert isinstance(T3, ttb.tensor)
     assert T3.shape == (2, 3, 2)
     data3 = np.array(
         [[[100, 138], [132, 186], [164, 234]], [[148, 204], [196, 276], [244, 348]]]
     )
     assert (T3.data == data3).all()
 
@@ -1196,14 +1196,20 @@
 
     # 2-way Multiply by single vector
     T2 = tensorInstance2.ttv(np.array([2, 2]), 0)
     assert isinstance(T2, ttb.tensor)
     assert T2.shape == (3,)
     assert (T2.data == np.array([10, 14, 18])).all()
 
+    # 2-way Multiply by single vector (exclude dims)
+    T2 = tensorInstance2.ttv(np.array([2, 2]), exclude_dims=1)
+    assert isinstance(T2, ttb.tensor)
+    assert T2.shape == (3,)
+    assert (T2.data == np.array([10, 14, 18])).all()
+
     # Multiply by multiple vectors, infer dimensions
     assert tensorInstance2.ttv([np.array([2, 2]), np.array([1, 1, 1])]) == 42
 
     # Multiply by multiple vectors as list of numpy.ndarrays
     assert tensorInstance2.ttv([np.array([2, 2]), np.array([1, 1, 1])]) == 42
 
     # 3-way Multiply by single vector
@@ -1222,14 +1228,26 @@
     T4 = tensorInstance4.ttv(2 * np.ones((tensorInstance4.shape[0],)), 0)
     assert isinstance(T4, ttb.tensor)
     assert T4.shape == (
         tensorInstance4.shape[1],
         tensorInstance4.shape[2],
         tensorInstance4.shape[3],
     )
+
+    # 4-way Multiply by single vector (exclude dims)
+    T4 = tensorInstance4.ttv(
+        2 * np.ones((tensorInstance4.shape[0],)), exclude_dims=np.array([1, 2, 3])
+    )
+    assert isinstance(T4, ttb.tensor)
+    assert T4.shape == (
+        tensorInstance4.shape[1],
+        tensorInstance4.shape[2],
+        tensorInstance4.shape[3],
+    )
+
     data4 = np.array(
         [
             [[12, 174, 336], [66, 228, 390], [120, 282, 444]],
             [[30, 192, 354], [84, 246, 408], [138, 300, 462]],
             [[48, 210, 372], [102, 264, 426], [156, 318, 480]],
         ]
     )
@@ -1254,64 +1272,64 @@
 @pytest.mark.indevelopment
 def test_tensor_ttsv(sample_tensor_4way):
     # 3-way
     tensorInstance3 = ttb.tensor.from_data(np.ones((4, 4, 4)))
     vector3 = np.array([4, 3, 2, 1])
     assert tensorInstance3.ttsv(vector3, version=1) == 1000
     assert (
-        tensorInstance3.ttsv(vector3, dims=-1, version=1) == 100 * np.ones((4,))
+        tensorInstance3.ttsv(vector3, skip_dim=0, version=1) == 100 * np.ones((4,))
     ).all()
     assert (
-        tensorInstance3.ttsv(vector3, dims=-2, version=1) == 10 * np.ones((4, 4))
+        tensorInstance3.ttsv(vector3, skip_dim=1, version=1) == 10 * np.ones((4, 4))
     ).all()
 
     # Invalid dims
-    with pytest.raises(AssertionError) as excinfo:
-        tensorInstance3.ttsv(vector3, dims=1)
+    with pytest.raises(ValueError) as excinfo:
+        tensorInstance3.ttsv(vector3, skip_dim=-1)
     assert "Invalid modes in ttsv" in str(excinfo)
 
     # 4-way tensor
     (params4, tensorInstance4) = sample_tensor_4way
-    T4ttsv = tensorInstance4.ttsv(np.array([1, 2, 3]), -3, version=1)
+    T4ttsv = tensorInstance4.ttsv(np.array([1, 2, 3]), 2, version=1)
     data4_3 = np.array(
         [
             [[222, 276, 330], [240, 294, 348], [258, 312, 366]],
             [[228, 282, 336], [246, 300, 354], [264, 318, 372]],
             [[234, 288, 342], [252, 306, 360], [270, 324, 378]],
         ]
     )
     assert (T4ttsv.data == data4_3).all()
 
     # 5-way dense tensor
     shape = (3, 3, 3, 3, 3)
     T5 = ttb.tensor.from_data(np.arange(1, np.prod(shape) + 1), shape)
-    T5ttsv = T5.ttsv(np.array([1, 2, 3]), -3, version=1)
+    T5ttsv = T5.ttsv(np.array([1, 2, 3]), 2, version=1)
     data5_3 = np.array(
         [
             [[5220, 5544, 5868], [5328, 5652, 5976], [5436, 5760, 6084]],
             [[5256, 5580, 5904], [5364, 5688, 6012], [5472, 5796, 6120]],
             [[5292, 5616, 5940], [5400, 5724, 6048], [5508, 5832, 6156]],
         ]
     )
     assert (T5ttsv.data == data5_3).all()
 
     # Test new algorithm, version=2
 
     # 3-way
     assert tensorInstance3.ttsv(vector3) == 1000
-    assert (tensorInstance3.ttsv(vector3, dims=-1) == 100 * np.ones((4,))).all()
-    assert (tensorInstance3.ttsv(vector3, dims=-2) == 10 * np.ones((4, 4))).all()
+    assert (tensorInstance3.ttsv(vector3, 0) == 100 * np.ones((4,))).all()
+    assert (tensorInstance3.ttsv(vector3, 1) == 10 * np.ones((4, 4))).all()
 
     # 4-way tensor
-    T4ttsv2 = tensorInstance4.ttsv(np.array([1, 2, 3]), -3)
+    T4ttsv2 = tensorInstance4.ttsv(np.array([1, 2, 3]), 2)
     assert (T4ttsv2.data == data4_3).all()
 
     # Incorrect version requested
     with pytest.raises(AssertionError) as excinfo:
-        tensorInstance4.ttsv(np.array([1, 2, 3]), -3, version=3)
+        tensorInstance4.ttsv(np.array([1, 2, 3]), 2, version=3)
     assert "Invalid value for version; should be None, 1, or 2" in str(excinfo)
 
 
 @pytest.mark.indevelopment
 def test_tensor_issymmetric(sample_tensor_2way):
     (params, tensorInstance) = sample_tensor_2way
```

### Comparing `pyttb-1.5.1/tests/test_ttensor.py` & `pyttb-1.6.0/tests/test_ttensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -228,14 +228,19 @@
     assert final_value == np.prod(ttensorInstance.core.shape)
 
     assert np.allclose(
         ttensorInstance.ttv(trivial_vectors[0], 0).double(),
         ttensorInstance.full().ttv(trivial_vectors[0], 0).double(),
     )
 
+    assert np.allclose(
+        ttensorInstance.ttv(trivial_vectors[0:2], exclude_dims=0).double(),
+        ttensorInstance.full().ttv(trivial_vectors[0:2], exclude_dims=0).double(),
+    )
+
     # Negative tests
     wrong_shape_vector = trivial_vectors.copy()
     wrong_shape_vector[0] = np.array([mul_factor, mul_factor])
     with pytest.raises(ValueError):
         sample_ttensor.ttv(wrong_shape_vector)
 
 
@@ -289,14 +294,19 @@
     final_value = ttensorInstance.ttm(matrices)  # No dims
     assert final_value.isequal(reverse_value)
     final_value = ttensorInstance.ttm(
         matrices, list(range(len(matrices)))
     )  # Dims as list
     assert final_value.isequal(reverse_value)
 
+    # Exclude Dims
+    assert ttensorInstance.ttm(matrices[1:], exclude_dims=0).isequal(
+        ttensorInstance.ttm(matrices[1:], dims=np.array([1, 2]))
+    )
+
     single_tensor_result = ttensorInstance.ttm(matrices[0], 0)
     single_tensor_full_result = ttensorInstance.full().ttm(matrices[0], 0)
     assert np.allclose(
         single_tensor_result.double(), single_tensor_full_result.double()
     ), (
         f"TTensor value is: \n{single_tensor_result.full()}\n\n"
         f"Full value is: \n{single_tensor_full_result}"
```

### Comparing `pyttb-1.5.1/tests/test_tucker_als.py` & `pyttb-1.6.0/tests/test_tucker_als.py`

 * *Files identical despite different names*

