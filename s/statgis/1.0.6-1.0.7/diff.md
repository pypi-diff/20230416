# Comparing `tmp/statgis-1.0.6.tar.gz` & `tmp/statgis-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statgis-1.0.6.tar", max compression
+gzip compressed data, was "statgis-1.0.7.tar", max compression
```

## Comparing `statgis-1.0.6.tar` & `statgis-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1133 2023-04-15 01:57:54.839842 statgis-1.0.6/LICENSE
--rw-r--r--   0        0        0      890 2023-04-15 20:15:51.780807 statgis-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     1469 2023-04-15 01:57:54.871115 statgis-1.0.6/README.md
--rw-r--r--   0        0        0      159 2023-04-15 01:57:55.092860 statgis-1.0.6/src/statgis/__init__.py
--rw-r--r--   0        0        0      283 2023-04-15 01:57:55.095862 statgis-1.0.6/src/statgis/gee/__init__.py
--rw-r--r--   0        0        0     4291 2023-04-15 01:57:55.096863 statgis-1.0.6/src/statgis/gee/classification.py
--rw-r--r--   0        0        0     1426 2023-04-15 01:57:55.103864 statgis-1.0.6/src/statgis/gee/landsat_functions.py
--rw-r--r--   0        0        0     2816 2023-04-15 01:57:55.401621 statgis-1.0.6/src/statgis/gee/river_analysis.py
--rw-r--r--   0        0        0     1904 2023-04-15 01:57:55.401621 statgis-1.0.6/src/statgis/gee/sample.py
--rw-r--r--   0        0        0      932 2023-04-15 01:57:55.401621 statgis-1.0.6/src/statgis/gee/sentinel_functions.py
--rw-r--r--   0        0        0     1334 2023-04-15 01:57:55.401621 statgis-1.0.6/src/statgis/gee/shoreline_analysis.py
--rw-r--r--   0        0        0     1238 2023-04-15 01:57:55.417245 statgis-1.0.6/src/statgis/gee/terrain_analysis.py
--rw-r--r--   0        0        0    10834 2023-04-15 20:05:41.515042 statgis-1.0.6/src/statgis/gee/time_series_analysis.py
--rw-r--r--   0        0        0     1835 2023-04-15 05:14:49.801143 statgis-1.0.6/src/statgis/gee/utils.py
--rw-r--r--   0        0        0     4616 2023-04-15 01:57:55.417245 statgis-1.0.6/src/statgis/gee/zonal_statistics.py
--rw-r--r--   0        0        0        0 2023-04-15 01:57:55.417245 statgis-1.0.6/src/statgis/statgis.py
--rw-r--r--   0        0        0       42 2023-04-15 01:57:55.471047 statgis-1.0.6/src/statgis/statutils/__init__.py
--rw-r--r--   0        0        0     3408 2023-04-15 04:08:25.691314 statgis-1.0.6/src/statgis/statutils/plots.py
--rw-r--r--   0        0        0     1970 2023-04-15 01:57:55.526062 statgis-1.0.6/src/statgis/statutils/stats.py
--rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 statgis-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1133 2023-04-15 01:57:54.839842 statgis-1.0.7/LICENSE
+-rw-r--r--   0        0        0      890 2023-04-16 05:22:36.960544 statgis-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1469 2023-04-15 01:57:54.871115 statgis-1.0.7/README.md
+-rw-r--r--   0        0        0      159 2023-04-15 01:57:55.092860 statgis-1.0.7/src/statgis/__init__.py
+-rw-r--r--   0        0        0      283 2023-04-15 01:57:55.095862 statgis-1.0.7/src/statgis/gee/__init__.py
+-rw-r--r--   0        0        0     4294 2023-04-15 23:07:05.575665 statgis-1.0.7/src/statgis/gee/classification.py
+-rw-r--r--   0        0        0     3717 2023-04-16 01:25:14.903252 statgis-1.0.7/src/statgis/gee/landsat_functions.py
+-rw-r--r--   0        0        0     2816 2023-04-15 01:57:55.401621 statgis-1.0.7/src/statgis/gee/river_analysis.py
+-rw-r--r--   0        0        0     1904 2023-04-15 01:57:55.401621 statgis-1.0.7/src/statgis/gee/sample.py
+-rw-r--r--   0        0        0      932 2023-04-15 01:57:55.401621 statgis-1.0.7/src/statgis/gee/sentinel_functions.py
+-rw-r--r--   0        0        0     1334 2023-04-15 01:57:55.401621 statgis-1.0.7/src/statgis/gee/shoreline_analysis.py
+-rw-r--r--   0        0        0     1238 2023-04-15 01:57:55.417245 statgis-1.0.7/src/statgis/gee/terrain_analysis.py
+-rw-r--r--   0        0        0     7501 2023-04-16 04:53:14.229067 statgis-1.0.7/src/statgis/gee/time_series_analysis.py
+-rw-r--r--   0        0        0     1835 2023-04-15 05:14:49.801143 statgis-1.0.7/src/statgis/gee/utils.py
+-rw-r--r--   0        0        0     4621 2023-04-16 05:07:36.177091 statgis-1.0.7/src/statgis/gee/zonal_statistics.py
+-rw-r--r--   0        0        0        0 2023-04-15 01:57:55.417245 statgis-1.0.7/src/statgis/statgis.py
+-rw-r--r--   0        0        0       42 2023-04-15 01:57:55.471047 statgis-1.0.7/src/statgis/statutils/__init__.py
+-rw-r--r--   0        0        0     3408 2023-04-15 04:08:25.691314 statgis-1.0.7/src/statgis/statutils/plots.py
+-rw-r--r--   0        0        0     1970 2023-04-15 01:57:55.526062 statgis-1.0.7/src/statgis/statutils/stats.py
+-rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 statgis-1.0.7/PKG-INFO
```

### Comparing `statgis-1.0.6/LICENSE` & `statgis-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `statgis-1.0.6/pyproject.toml` & `statgis-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statgis"
-version = "1.0.6"
+version = "1.0.7"
 description = "Tools for improve work with geospatial data in Python"
 authors = ["Sebástian Narváez-Salcedo <sanarvaezstatgis@gmail.com>", "Brayan Navarro-Londoño <brnavarrostatgis@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.8"
```

### Comparing `statgis-1.0.6/README.md` & `statgis-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `statgis-1.0.6/src/statgis/gee/classification.py` & `statgis-1.0.7/src/statgis/gee/classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 
 
 def clean_boolean_classification(
     image: ee.Image,
     scale: float,
     band: str,
     true_class_threshold: float,
-    false_class_treshold: float,
+    false_class_threshold: float,
 ) -> ee.Image:
     """
     Clean boolean coverage classification counting the neighbors pixels and filter
     those which surpass their respective thresholds.
 
     Parameters
     ----------
@@ -142,26 +142,26 @@
 
     band : str
         Band name with the classification.
 
     true_class_threshold : float
         Threshold for true values to conserve an entity.
 
-    false_class_treshold : float
+    false_class_threshold : float
         Threshold for false values to conserve an entity.
 
     Returns
     -------
     filled : ee.Image
         Boolean classification image cleaned.
     """
     image = image.select(band).toInt()
 
     connected_false = ee.Number(true_class_threshold).divide(scale).int()
-    connected_true = ee.Number(false_class_treshold).divide(scale).int()
+    connected_true = ee.Number(false_class_threshold).divide(scale).int()
 
     false_filled = (
         image.addBands(image)
         .reduceConnectedComponents(ee.Reducer.median(), band, connected_false)
         .unmask(99)
         .eq(99)
         .And(image.neq(0))
```

### Comparing `statgis-1.0.6/src/statgis/gee/river_analysis.py` & `statgis-1.0.7/src/statgis/gee/river_analysis.py`

 * *Files identical despite different names*

### Comparing `statgis-1.0.6/src/statgis/gee/sample.py` & `statgis-1.0.7/src/statgis/gee/sample.py`

 * *Files identical despite different names*

### Comparing `statgis-1.0.6/src/statgis/gee/sentinel_functions.py` & `statgis-1.0.7/src/statgis/gee/sentinel_functions.py`

 * *Files identical despite different names*

### Comparing `statgis-1.0.6/src/statgis/gee/shoreline_analysis.py` & `statgis-1.0.7/src/statgis/gee/shoreline_analysis.py`

 * *Files identical despite different names*

### Comparing `statgis-1.0.6/src/statgis/gee/terrain_analysis.py` & `statgis-1.0.7/src/statgis/gee/terrain_analysis.py`

 * *Files identical despite different names*

### Comparing `statgis-1.0.6/src/statgis/gee/utils.py` & `statgis-1.0.7/src/statgis/gee/utils.py`

 * *Files identical despite different names*

### Comparing `statgis-1.0.6/src/statgis/gee/zonal_statistics.py` & `statgis-1.0.7/src/statgis/gee/zonal_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,27 +27,27 @@
         Region of interest to reduce the image.
 
     scale : float
         Pixel size for the sample to perform the zonal statistics.
 
     bands : Sequence | str (optional)
         List, tuple with the bands of interest or, if you only want one band, the name
-        of the band. By default the process takes into consideration all bands.
+        of the band. By default, the process takes into consideration all bands.
 
     reducer : ee.Reducer | str (optional)
         Reducer to apply to the image. By default, image are reduced to its, mean, standard
         deviation, maximum, minimum, and count.
 
     tile_scale : int (optional)
         Scale of the mosaic to allow EarthEngine to split the task to more cores.
 
     Returns
     -------
     data : pandas.DataFrame
-        DataFrame with all the stats for all spcified bands.
+        DataFrame with all the stats for all specified bands.
     """
     if bands != "all":
         image = image.select(bands)
 
     if reducer == "all":
         reducer = ee.Reducer.mean().combine(
             ee.Reducer.stdDev().combine(
@@ -83,38 +83,38 @@
 ) -> pd.DataFrame:
     """
     Function to calculate a statistic in the specified region for all Image in an image
     collection.
 
     Parameters
     ----------
-    ImageCollection : ee.ImageCollection
+    image_collection : ee.ImageCollection
         Image Collection with the image to reduce.
 
     geom : ee.Geometry
         Region of interest to reduce the images.
 
     scale : float
         Pixel size for the sample to perform the zonal statistics.
 
     bands : Sequence | str (optional)
         List, tuple with the bands of interest or, if you only want one band, the name
-        of the band. By default the process takes into consideration all bands.
+        of the band. By default, the process takes into consideration all bands.
 
     reducer : ee.Reducer | str (optional)
         Reducer to apply to all image. By default, image are reduced to its, mean, standard
         deviation, maximum, minimum, and count.
 
     tile_scale : int (optional)
         Scale of the mosaic to allow EarthEngine to split the task to more cores.
 
     Returns
     ------
     data : pandas.DataFrame
-        DataFrame with all the stats for all spcified bands.
+        DataFrame with all the stats for all specified bands.
     """
     if bands != "all":
         image_collection = image_collection.select(bands)
 
     if reducer == "all":
         reducer = ee.Reducer.mean().combine(
             ee.Reducer.stdDev().combine(
```

### Comparing `statgis-1.0.6/src/statgis/statutils/plots.py` & `statgis-1.0.7/src/statgis/statutils/plots.py`

 * *Files identical despite different names*

### Comparing `statgis-1.0.6/src/statgis/statutils/stats.py` & `statgis-1.0.7/src/statgis/statutils/stats.py`

 * *Files identical despite different names*

### Comparing `statgis-1.0.6/PKG-INFO` & `statgis-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statgis
-Version: 1.0.6
+Version: 1.0.7
 Summary: Tools for improve work with geospatial data in Python
 License: MIT
 Author: Sebástian Narváez-Salcedo
 Author-email: sanarvaezstatgis@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

