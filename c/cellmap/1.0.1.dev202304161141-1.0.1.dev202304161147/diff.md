# Comparing `tmp/cellmap-1.0.1.dev202304161141-py3-none-any.whl.zip` & `tmp/cellmap-1.0.1.dev202304161147-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1388284 bytes, number of entries: 6
+Zip file size: 1388287 bytes, number of entries: 6
 -rw-r--r--  2.0 unx  4446947 b- defN 80-Jan-01 00:00 cellmap/CellMap_view_3D.html
 -rw-r--r--  2.0 unx       52 b- defN 80-Jan-01 00:00 cellmap/__init__.py
--rw-r--r--  2.0 unx    53291 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
--rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304161141.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304161141.dist-info/WHEEL
-?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304161141.dist-info/RECORD
-6 files, 4502655 bytes uncompressed, 1387398 bytes compressed:  69.2%
+-rw-r--r--  2.0 unx    53292 b- defN 80-Jan-01 00:00 cellmap/cellmap.py
+-rw-r--r--  2.0 unx     1785 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304161147.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cellmap-1.0.1.dev202304161147.dist-info/WHEEL
+?rw-r--r--  2.0 unx      492 b- defN 16-Jan-01 00:00 cellmap-1.0.1.dev202304161147.dist-info/RECORD
+6 files, 4502656 bytes uncompressed, 1387401 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -3,17 +3,17 @@
 
 Filename: cellmap/__init__.py
 Comment: 
 
 Filename: cellmap/cellmap.py
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304161141.dist-info/METADATA
+Filename: cellmap-1.0.1.dev202304161147.dist-info/METADATA
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304161141.dist-info/WHEEL
+Filename: cellmap-1.0.1.dev202304161147.dist-info/WHEEL
 Comment: 
 
-Filename: cellmap-1.0.1.dev202304161141.dist-info/RECORD
+Filename: cellmap-1.0.1.dev202304161147.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cellmap/cellmap.py

```diff
@@ -1,12 +1,12 @@
 import anndata
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
-from matplotlib import patheffects as PathEffect
+from matplotlib import patheffects as PathEffects
 import matplotlib.cm
 import scipy
 import sklearn.preprocessing
 import sklearn.neighbors
 import matplotlib.colors
 import pandas as pd
 import logging
```

## Comparing `cellmap-1.0.1.dev202304161141.dist-info/METADATA` & `cellmap-1.0.1.dev202304161147.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmap
-Version: 1.0.1.dev202304161141
+Version: 1.0.1.dev202304161147
 Summary: CellMap - RNA landscape inference method
 Home-page: https://github.com/yusuke-imoto-lab/CellMap
 Author: Yusuke Imoto
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

