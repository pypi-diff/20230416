# Comparing `tmp/MLandPattern-0.1.3.tar.gz` & `tmp/MLandPattern-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLandPattern-0.1.3.tar", last modified: Wed Mar 29 18:22:53 2023, max compression
+gzip compressed data, was "MLandPattern-0.1.4.tar", last modified: Sun Apr 16 12:45:24 2023, max compression
```

## Comparing `MLandPattern-0.1.3.tar` & `MLandPattern-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-03-29 18:22:53.696514 MLandPattern-0.1.3/
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-03-29 18:22:53.693287 MLandPattern-0.1.3/MLandPattern/
--rw-r--r--   0 pablomunoz   (501) staff       (20)     5071 2023-03-29 09:34:28.000000 MLandPattern-0.1.3/MLandPattern/MLandPattern.py
--rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.1.3/MLandPattern/__init__.py
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-03-29 18:22:53.695327 MLandPattern-0.1.3/MLandPattern.egg-info/
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-03-29 18:22:53.000000 MLandPattern-0.1.3/MLandPattern.egg-info/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-03-29 18:22:53.000000 MLandPattern-0.1.3/MLandPattern.egg-info/SOURCES.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-03-29 18:22:53.000000 MLandPattern-0.1.3/MLandPattern.egg-info/dependency_links.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-03-29 18:22:53.000000 MLandPattern-0.1.3/MLandPattern.egg-info/top_level.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-03-29 18:22:53.696093 MLandPattern-0.1.3/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.1.3/README.md
--rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-03-29 18:22:53.696672 MLandPattern-0.1.3/setup.cfg
--rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-03-29 18:22:49.000000 MLandPattern-0.1.3/setup.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-04-16 12:45:24.832422 MLandPattern-0.1.4/
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-04-16 12:45:24.828932 MLandPattern-0.1.4/MLandPattern/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)     5772 2023-04-16 12:40:00.000000 MLandPattern-0.1.4/MLandPattern/MLandPattern.py
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.1.4/MLandPattern/__init__.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-04-16 12:45:24.831236 MLandPattern-0.1.4/MLandPattern.egg-info/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-04-16 12:45:24.000000 MLandPattern-0.1.4/MLandPattern.egg-info/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-04-16 12:45:24.000000 MLandPattern-0.1.4/MLandPattern.egg-info/SOURCES.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-04-16 12:45:24.000000 MLandPattern-0.1.4/MLandPattern.egg-info/dependency_links.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-04-16 12:45:24.000000 MLandPattern-0.1.4/MLandPattern.egg-info/top_level.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-04-16 12:45:24.832021 MLandPattern-0.1.4/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.1.4/README.md
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-04-16 12:45:24.832584 MLandPattern-0.1.4/setup.cfg
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-04-16 12:37:29.000000 MLandPattern-0.1.4/setup.py
```

### Comparing `MLandPattern-0.1.3/MLandPattern/MLandPattern.py` & `MLandPattern-0.1.4/MLandPattern/MLandPattern.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import pandas as pd
 import scipy
+import math
 from matplotlib import pyplot as plt
 
 
 def loadCSV(pathname, class_label, attribute_names):
     """
     Extracts the attributes and class labels of an input 
     csv file dataset
@@ -154,7 +155,33 @@
 def graphic_scatter_2d(matrix, labels, names, x_axis="Axis 1", y_axis="Axis 2"):
     for i in range(len(names)):
         plt.scatter(matrix[0][labels == i], matrix[1][labels == i], label=names[i])
     plt.xlabel(x_axis)
     plt.ylabel(y_axis)
     plt.legend()
     plt.show()
+
+
+def logpdf_GAU_ND(x, mu, C):
+    M = C.shape[1]
+    inv_C = np.linalg.inv(C)
+    [_, log_C] = np.linalg.slogdet(C)
+    log_2pi = math.log(2*math.pi)
+    y = np.zeros(x.shape[1]) if M == 1 else np.zeros(x.shape)
+    for i in range(x.shape[1]):
+        norm_x = vcol(x[:, i]) - mu
+        inter_value = np.dot(norm_x.T, inv_C)
+        dot_mult = np.dot(inter_value, norm_x)
+        MVG = (-M*log_2pi - log_C - dot_mult)/2
+        if M == 1:
+            y[i] = MVG
+        else:
+            y[:, i] = MVG
+    return y
+
+
+def logLikelihood (X, mu, c):
+    M = c.shape[1]
+    logN = logpdf_GAU_ND(X, mu, c)
+    print(logN.shape)
+    acum = logN.sum(1) if M != 1 else logN.sum()
+    return acum
```

