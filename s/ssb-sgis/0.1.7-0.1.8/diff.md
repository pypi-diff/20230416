# Comparing `tmp/ssb_sgis-0.1.7.tar.gz` & `tmp/ssb_sgis-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_sgis-0.1.7.tar", max compression
+gzip compressed data, was "ssb_sgis-0.1.8.tar", max compression
```

## Comparing `ssb_sgis-0.1.7.tar` & `ssb_sgis-0.1.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1074 2023-04-15 14:20:46.157930 ssb_sgis-0.1.7/LICENSE
--rw-r--r--   0        0        0     7260 2023-04-15 14:20:46.157930 ssb_sgis-0.1.7/README.md
--rw-r--r--   0        0        0     2477 2023-04-15 14:21:00.474151 ssb_sgis-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1651 2023-04-15 14:20:46.185930 ssb_sgis-0.1.7/src/sgis/__init__.py
--rw-r--r--   0        0        0     2634 2023-04-15 14:20:46.185930 ssb_sgis-0.1.7/src/sgis/dapla.py
--rw-r--r--   0        0        0      666 2023-04-15 14:20:46.185930 ssb_sgis-0.1.7/src/sgis/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-15 14:20:46.185930 ssb_sgis-0.1.7/src/sgis/geopandas_tools/__init__.py
--rw-r--r--   0        0        0     8776 2023-04-15 14:20:46.185930 ssb_sgis-0.1.7/src/sgis/geopandas_tools/buffer_dissolve_explode.py
--rw-r--r--   0        0        0    27590 2023-04-15 14:20:46.185930 ssb_sgis-0.1.7/src/sgis/geopandas_tools/general.py
--rw-r--r--   0        0        0     5480 2023-04-15 14:20:46.185930 ssb_sgis-0.1.7/src/sgis/geopandas_tools/geometry_types.py
--rw-r--r--   0        0        0    34748 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/geopandas_tools/line_operations.py
--rw-r--r--   0        0        0    16647 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/geopandas_tools/neighbors.py
--rw-r--r--   0        0        0    14435 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/geopandas_tools/overlay.py
--rw-r--r--   0        0        0     6316 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/geopandas_tools/point_operations.py
--rw-r--r--   0        0        0     5046 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/geopandas_tools/polygon_operations.py
--rw-r--r--   0        0        0     2468 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/helpers.py
--rw-r--r--   0        0        0        0 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/maps/__init__.py
--rw-r--r--   0        0        0    19148 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/maps/explore.py
--rw-r--r--   0        0        0    20499 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/maps/legend.py
--rw-r--r--   0        0        0    16402 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/maps/map.py
--rw-r--r--   0        0        0    12747 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/maps/maps.py
--rw-r--r--   0        0        0    14092 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/maps/thematicmap.py
--rw-r--r--   0        0        0        0 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/networkanalysis/__init__.py
--rw-r--r--   0        0        0     7628 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/networkanalysis/_get_route.py
--rw-r--r--   0        0        0     2455 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/networkanalysis/_od_cost_matrix.py
--rw-r--r--   0        0        0     4182 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/networkanalysis/_points.py
--rw-r--r--   0        0        0     4426 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/networkanalysis/_service_area.py
--rw-r--r--   0        0        0    11354 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/networkanalysis/directednetwork.py
--rw-r--r--   0        0        0    23771 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/networkanalysis/network.py
--rw-r--r--   0        0        0     6124 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/networkanalysis/network_norway.py
--rw-r--r--   0        0        0    61926 2023-04-15 14:21:00.474151 ssb_sgis-0.1.7/src/sgis/networkanalysis/networkanalysis.py
--rw-r--r--   0        0        0    12692 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/networkanalysis/networkanalysisrules.py
--rw-r--r--   0        0        0        0 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/py.typed
--rw-r--r--   0        0        0     3765 2023-04-15 14:20:46.189930 ssb_sgis-0.1.7/src/sgis/read_parquet.py
--rw-r--r--   0        0        0     8624 1970-01-01 00:00:00.000000 ssb_sgis-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-16 18:53:28.316596 ssb_sgis-0.1.8/LICENSE
+-rw-r--r--   0        0        0     7263 2023-04-16 18:53:43.237504 ssb_sgis-0.1.8/README.md
+-rw-r--r--   0        0        0     2477 2023-04-16 18:53:43.237504 ssb_sgis-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1651 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/__init__.py
+-rw-r--r--   0        0        0     2634 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/dapla.py
+-rw-r--r--   0        0        0      666 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/geopandas_tools/__init__.py
+-rw-r--r--   0        0        0     8776 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/geopandas_tools/buffer_dissolve_explode.py
+-rw-r--r--   0        0        0    27637 2023-04-16 18:53:43.237504 ssb_sgis-0.1.8/src/sgis/geopandas_tools/general.py
+-rw-r--r--   0        0        0     5480 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/geopandas_tools/geometry_types.py
+-rw-r--r--   0        0        0    34770 2023-04-16 18:53:43.237504 ssb_sgis-0.1.8/src/sgis/geopandas_tools/line_operations.py
+-rw-r--r--   0        0        0    16647 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/geopandas_tools/neighbors.py
+-rw-r--r--   0        0        0    14435 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/geopandas_tools/overlay.py
+-rw-r--r--   0        0        0     6316 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/geopandas_tools/point_operations.py
+-rw-r--r--   0        0        0     5046 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/geopandas_tools/polygon_operations.py
+-rw-r--r--   0        0        0     2468 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/helpers.py
+-rw-r--r--   0        0        0        0 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/maps/__init__.py
+-rw-r--r--   0        0        0    19154 2023-04-16 18:53:43.237504 ssb_sgis-0.1.8/src/sgis/maps/explore.py
+-rw-r--r--   0        0        0    20499 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/maps/legend.py
+-rw-r--r--   0        0        0    16711 2023-04-16 18:53:43.237504 ssb_sgis-0.1.8/src/sgis/maps/map.py
+-rw-r--r--   0        0        0    12747 2023-04-16 18:53:43.237504 ssb_sgis-0.1.8/src/sgis/maps/maps.py
+-rw-r--r--   0        0        0    13848 2023-04-16 18:53:43.237504 ssb_sgis-0.1.8/src/sgis/maps/thematicmap.py
+-rw-r--r--   0        0        0        0 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/networkanalysis/__init__.py
+-rw-r--r--   0        0        0     6119 2023-04-16 18:53:43.237504 ssb_sgis-0.1.8/src/sgis/networkanalysis/_get_route.py
+-rw-r--r--   0        0        0     2455 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/networkanalysis/_od_cost_matrix.py
+-rw-r--r--   0        0        0     4182 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/networkanalysis/_points.py
+-rw-r--r--   0        0        0     4416 2023-04-16 18:53:43.237504 ssb_sgis-0.1.8/src/sgis/networkanalysis/_service_area.py
+-rw-r--r--   0        0        0    11306 2023-04-16 18:53:43.241504 ssb_sgis-0.1.8/src/sgis/networkanalysis/directednetwork.py
+-rw-r--r--   0        0        0    23771 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/networkanalysis/network.py
+-rw-r--r--   0        0        0     6124 2023-04-16 18:53:28.352598 ssb_sgis-0.1.8/src/sgis/networkanalysis/network_norway.py
+-rw-r--r--   0        0        0    63500 2023-04-16 18:53:43.241504 ssb_sgis-0.1.8/src/sgis/networkanalysis/networkanalysis.py
+-rw-r--r--   0        0        0    12692 2023-04-16 18:53:28.356598 ssb_sgis-0.1.8/src/sgis/networkanalysis/networkanalysisrules.py
+-rw-r--r--   0        0        0        0 2023-04-16 18:53:28.356598 ssb_sgis-0.1.8/src/sgis/py.typed
+-rw-r--r--   0        0        0     3765 2023-04-16 18:53:28.356598 ssb_sgis-0.1.8/src/sgis/read_parquet.py
+-rw-r--r--   0        0        0     8627 1970-01-01 00:00:00.000000 ssb_sgis-0.1.8/PKG-INFO
```

### Comparing `ssb_sgis-0.1.7/LICENSE` & `ssb_sgis-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.7/README.md` & `ssb_sgis-0.1.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -212,15 +212,15 @@
 
 ### Documentation
 
 To generate the API-documentation locally, run the following command from the root
 directory:
 
 ```shell
-poetry run sphinx-build docs docs/_build
+poetry run sphinx-build -W docs docs/_build
 ```
 
 Then open the file `docs/_build/index.html`.
 
 To check and run the docstrings examples, run this command:
 
 ```shell
```

### Comparing `ssb_sgis-0.1.7/pyproject.toml` & `ssb_sgis-0.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-sgis"
-version = "0.1.7"
+version = "0.1.8"
 description = "GIS functions used at Statistics Norway."
 authors = ["Statistics Norway <ort@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "sgis", from = "src"}]
 homepage = "https://github.com/statisticsnorway/ssb-sgis"
 repository = "https://github.com/statisticsnorway/ssb-sgis"
```

### Comparing `ssb_sgis-0.1.7/src/sgis/__init__.py` & `ssb_sgis-0.1.8/src/sgis/__init__.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.7/src/sgis/dapla.py` & `ssb_sgis-0.1.8/src/sgis/dapla.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.7/src/sgis/exceptions.py` & `ssb_sgis-0.1.8/src/sgis/exceptions.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.7/src/sgis/geopandas_tools/buffer_dissolve_explode.py` & `ssb_sgis-0.1.8/src/sgis/geopandas_tools/buffer_dissolve_explode.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.7/src/sgis/geopandas_tools/general.py` & `ssb_sgis-0.1.8/src/sgis/geopandas_tools/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     >>> points
                     geometry
     0  POINT (0.59376 0.92577)
     1  POINT (0.34075 0.91650)
     2  POINT (0.74841 0.10627)
     3  POINT (0.00966 0.87868)
     4  POINT (0.38046 0.87879)
-
     >>> coordinate_array(points)
     array([[0.59376221, 0.92577159],
         [0.34074678, 0.91650446],
         [0.74840912, 0.10626954],
         [0.00965935, 0.87867915],
         [0.38045827, 0.87878816]])
     """
@@ -179,15 +178,14 @@
     4     POINT (0.76403 0.73539)
     ...                       ...
     9995  POINT (0.90433 0.75080)
     9996  POINT (0.10959 0.59785)
     9997  POINT (0.00330 0.79168)
     9998  POINT (0.90926 0.96215)
     9999  POINT (0.01386 0.22935)
-
     [10000 rows x 1 columns]
 
     Values with a mean of 100.
 
     >>> points = random_points(10_000, loc=100)
     >>> points
                          geometry
@@ -198,15 +196,14 @@
     4       POINT (94.101 24.837)
     ...                       ...
     9995   POINT (174.344 91.772)
     9996    POINT (95.375 11.391)
     9997    POINT (45.694 60.843)
     9998   POINT (73.261 101.881)
     9999  POINT (134.503 168.155)
-
     [10000 rows x 1 columns]
     """
     if isinstance(n, (str, float)):
         n = int(n)
 
     x = np.random.rand(n) * float(loc) * 2
     y = np.random.rand(n) * float(loc) * 2
@@ -248,15 +245,14 @@
     4   POLYGON ((1.13941 0.20821, 1.13892 0.17680, 1....
     ..                                                ...
     95  POLYGON ((1.13462 0.18908, 1.13412 0.15767, 1....
     96  POLYGON ((1.96391 0.43191, 1.96342 0.40050, 1....
     97  POLYGON ((1.30569 0.46956, 1.30520 0.43815, 1....
     98  POLYGON ((1.18172 0.10944, 1.18122 0.07803, 1....
     99  POLYGON ((1.06156 0.99893, 1.06107 0.96752, 1....
-
     [100 rows x 1 columns]
 
     >>> points = sg.random_points_in_polygons(polygons, 3)
     >>> points
                         geometry
     0   POINT (0.74944 -0.41658)
     0    POINT (1.27490 0.54076)
@@ -265,15 +261,14 @@
     1    POINT (0.21124 0.89223)
     ..                       ...
     98  POINT (-0.39865 0.87135)
     98   POINT (0.03573 0.50788)
     99  POINT (-0.79089 0.57835)
     99   POINT (0.39838 1.50881)
     99   POINT (0.98383 0.77298)
-
     [300 rows x 1 columns]
     """
 
     if not all(gdf.geom_type.isin(["Polygon", "MultiPolygon"])):
         raise ValueError("Geometry types must be polygon.")
 
     if gdf.index.is_unique:
@@ -304,16 +299,16 @@
             overlapping = overlapping.loc[overlapping.index == overlapping.temp_idx____]
 
             all_points = pd.concat([all_points, overlapping], ignore_index=ignore_index)
 
             overlapping_indices = overlapping_indices + tuple(overlapping.index.values)
 
             gdf__ = gdf.loc[~gdf["temp_idx____"].isin(overlapping_indices)]
-            bounds = gdf__.bounds
             temp_idx____ = gdf__["temp_idx____"].values
+            bounds = gdf__.bounds
 
     all_points = all_points.sort_index().drop(["temp_idx____", "index_right"], axis=1)
 
     if gdf.index.is_unique:
         gdf = gdf.drop("temp_idx____", axis=1)
         return all_points
 
@@ -592,77 +587,80 @@
     --------
     >>> from sgis import to_gdf
     >>> coords = (10, 60)
     >>> to_gdf(coords, crs=4326)
                         geometry
     0  POINT (10.00000 60.00000)
 
+    From wkt.
+
     >>> wkt = "POINT (10 60)"
     >>> to_gdf(wkt, crs=4326)
                         geometry
     0  POINT (10.00000 60.00000)
 
-    Multiple coordinates will be converted to Points, unless a line or polygon geometry
-    is constructed beforehand.
+    From DataFrame with x, y (optionally z) coordinate columns. Index and
+    columns are preserved.
 
-    >>> coordslist = [(10, 60), (11, 59)]
-    >>> to_gdf(coordslist, crs=4326)
-                        geometry
-    0  POINT (10.00000 60.00000)
-    1  POINT (11.00000 59.00000)
+    >>> df = pd.DataFrame({"x": [10, 11], "y": [60, 59]}, index=[1,3])
+        x   y
+    1  10  60
+    3  11  59
+    >>> gdf = to_gdf(df, geometry=["x", "y"], crs=4326)
+    >>> gdf
+        x   y                   geometry
+    1  10  60  POINT (10.00000 60.00000)
+    3  11  59  POINT (11.00000 59.00000)
 
-    >>> from shapely.geometry import LineString
-    >>> to_gdf(LineString(coordslist), crs=4326)
-                                                geometry
-    0  LINESTRING (10.00000 60.00000, 11.00000 59.00000)
+    For DataFrame/dict with a geometry-like column, the geometry column can be
+    speficied with the geometry parameter, which is set to "geometry" by default.
+
+    >>> df = pd.DataFrame({"col": [1, 2], "geometry": ["point (10 60)", (11, 59)]})
+    >>> df
+       col       geometry
+    0    1  point (10 60)
+    1    2       (11, 59)
+    >>> gdf = to_gdf(df, crs=4326)
+    >>> gdf
+       col                   geometry
+    0    1  POINT (10.00000 60.00000)
+    1    2  POINT (11.00000 59.00000)
 
-    Dictionaries/Series will preserve the keys/index.
+    From Series or Series-like dictionary.
 
     >>> d = {1: (10, 60), 3: (11, 59)}
     >>> to_gdf(d)
                         geometry
     1  POINT (10.00000 60.00000)
     3  POINT (11.00000 59.00000)
 
     >>> from pandas import Series
     >>> to_gdf(Series(d))
                         geometry
     1  POINT (10.00000 60.00000)
     3  POINT (11.00000 59.00000)
 
-    DataFrame/dict with geometry-like column, will keep its column structure if
-    the geometry column matches the "geometry" parameter, which is set to "geometry" by
-    default.
-
-    >>> df = pd.DataFrame({"col": [1, 2], "geometry": ["point (10 60)", (11, 59)]})
-    >>> df
-       col       geometry
-    0    1  point (10 60)
-    1    2       (11, 59)
-    >>> gdf = to_gdf(df, geometry="geometry)
-    >>> gdf
-       col                   geometry
-    0    1  POINT (10.00000 60.00000)
-    1    2  POINT (11.00000 59.00000)
+    Multiple coordinates will be converted to points, unless a line or polygon geometry
+    is constructed beforehand.
 
-    From DataFrame with x, y (optionally z) coordinate columns.
+    >>> coordslist = [(10, 60), (11, 59)]
+    >>> to_gdf(coordslist, crs=4326)
+                        geometry
+    0  POINT (10.00000 60.00000)
+    1  POINT (11.00000 59.00000)
 
-    >>> df = pd.DataFrame({"x": [10, 11], "y": [60, 59]})
-        x   y
-    0  10  60
-    1  11  59
-    >>> gdf = to_gdf(df, geometry=["x", "y"])
-    >>> gdf
-        x   y                   geometry
-    0  10  60  POINT (10.00000 60.00000)
-    1  11  59  POINT (11.00000 59.00000)
+    >>> from shapely.geometry import LineString
+    >>> to_gdf(LineString(coordslist), crs=4326)
+                                                geometry
+    0  LINESTRING (10.00000 60.00000, 11.00000 59.00000)
 
     From 2 or 3 dimensional array.
 
-    >>> to_gdf(np.random.randint(100, size=(5, 3)))
+    >>> arr = np.random.randint(100, size=(5, 3))
+    >>> to_gdf(arr)
                              geometry
     0  POINT Z (82.000 88.000 82.000)
     1  POINT Z (70.000 92.000 20.000)
     2   POINT Z (91.000 34.000 3.000)
     3   POINT Z (1.000 50.000 77.000)
     4  POINT Z (58.000 49.000 46.000)
     """
```

### Comparing `ssb_sgis-0.1.7/src/sgis/geopandas_tools/geometry_types.py` & `ssb_sgis-0.1.8/src/sgis/geopandas_tools/geometry_types.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.7/src/sgis/geopandas_tools/line_operations.py` & `ssb_sgis-0.1.8/src/sgis/geopandas_tools/line_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,16 +205,16 @@
     splitted = make_edge_coords_cols(splitted)
 
     splitted_source = to_gdf(splitted["source_coords"], crs=lines.crs)
     splitted_target = to_gdf(splitted["target_coords"], crs=lines.crs)
 
     # find the nearest snapped point for each source and target of the lines
     snapped = snapped.set_index("point_coords")
-    dists_source = get_k_nearest_neighbors(splitted_source, snapped, k=1)
-    dists_target = get_k_nearest_neighbors(splitted_target, snapped, k=1)
+    dists_source: DataFrame = get_k_nearest_neighbors(splitted_source, snapped, k=1)
+    dists_target: DataFrame = get_k_nearest_neighbors(splitted_target, snapped, k=1)
 
     dists_source = dists_source.loc[dists_source.distance <= BUFFDIST * 2]
     dists_target = dists_target.loc[dists_target.distance <= BUFFDIST * 2]
 
     pointmapper_source: pd.Series = dists_source["neighbor_index"]
     pointmapper_target: pd.Series = dists_target["neighbor_index"]
```

### Comparing `ssb_sgis-0.1.7/src/sgis/geopandas_tools/neighbors.py` & `ssb_sgis-0.1.8/src/sgis/geopandas_tools/neighbors.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.7/src/sgis/geopandas_tools/overlay.py` & `ssb_sgis-0.1.8/src/sgis/geopandas_tools/overlay.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.7/src/sgis/geopandas_tools/point_operations.py` & `ssb_sgis-0.1.8/src/sgis/geopandas_tools/point_operations.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.7/src/sgis/geopandas_tools/polygon_operations.py` & `ssb_sgis-0.1.8/src/sgis/geopandas_tools/polygon_operations.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.7/src/sgis/helpers.py` & `ssb_sgis-0.1.8/src/sgis/helpers.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.7/src/sgis/maps/explore.py` & `ssb_sgis-0.1.8/src/sgis/maps/explore.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,16 +68,15 @@
         **kwargs,
     ):
         super().__init__(*gdfs, column=column, **kwargs)
         self.popup = popup
         self.max_zoom = max_zoom
         self.show_in_browser = show_in_browser
 
-        if any(get_geom_type(gdf) == "mixed" for gdf in self.gdfs):
-            self._make_all_polygon()
+        self._to_single_geom_type()
 
         if self._is_categorical:
             if len(self.gdfs) == 1:
                 self._split_categories()
         else:
             if not self._cmap:
                 self._cmap = "viridis"
@@ -172,24 +171,25 @@
             gdf = self.gdf.loc[self.gdf[self.column] == cat]
             new_gdfs.append(gdf)
             new_labels.append(cat)
         self._gdfs = new_gdfs
         self._gdf = pd.concat(new_gdfs, ignore_index=True)
         self.labels = new_labels
 
-    def _make_all_polygon(self):
-        """Buffer gdf if mixed geometry types
+    def _to_single_geom_type(self):
+        """Buffer gdf if mixed geometry types. Expode to singlepart.
 
-        Because Folium does not handle GeometryCollection well
+        Because Folium does not handle mixed geometries well.
         """
 
         new_gdfs = []
-        for gdf in self.gdfs:
+        for gdf in self._gdfs:
             if get_geom_type(gdf) == "mixed":
                 gdf[gdf._geometry_column_name] = gdf.buffer(0.1)
+            gdf = gdf.explode(index_parts=False)
             new_gdfs.append(gdf)
         self._gdfs = new_gdfs
         self._gdf = pd.concat(new_gdfs, ignore_index=True)
         self._nan_idx = self._gdf[self._column].isna()
 
     def _update_column(self):
         self._is_categorical = self._check_if_categorical()
```

### Comparing `ssb_sgis-0.1.7/src/sgis/maps/legend.py` & `ssb_sgis-0.1.8/src/sgis/maps/legend.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.7/src/sgis/maps/map.py` & `ssb_sgis-0.1.8/src/sgis/maps/map.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,17 +240,16 @@
         """Setting the labels after copying the gdfs."""
         for i, gdf in enumerate(self._gdfs):
             gdf["label"] = self.labels[i]
 
     def _to_common_crs_and_one_geom_col(self, gdfs: list[GeoDataFrame]):
         """Need common crs and max one geometry column."""
         crs_list = list({gdf.crs for gdf in gdfs if gdf.crs is not None})
-        if not crs_list:
-            return gdfs
-        self.crs = crs_list[0]
+        if crs_list:
+            self.crs = crs_list[0]
         new_gdfs = []
         for gdf in gdfs:
             gdf = drop_inactive_geometry_columns(gdf).pipe(rename_geometry_if)
             if crs_list:
                 try:
                     gdf = gdf.to_crs(self.crs)
                 except ValueError:
@@ -479,7 +478,19 @@
 
     @column.setter
     def column(self, _):
         raise ValueError(
             "Cannot change 'column' after init. Specify 'column' in the "
             "class initialiser."
         )
+
+    def __setitem__(self, item, new_item):
+        return setattr(self, item, new_item)
+
+    def __getitem__(self, item):
+        return getattr(self, item)
+
+    def get(self, key, default=None):
+        try:
+            return self[key]
+        except (KeyError, ValueError, IndexError, AttributeError):
+            return default
```

### Comparing `ssb_sgis-0.1.7/src/sgis/maps/maps.py` & `ssb_sgis-0.1.8/src/sgis/maps/maps.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     )
     m.explore()
 
 
 def samplemap(
     *gdfs: GeoDataFrame,
     column: str | None = None,
-    size: int = 1500,
+    size: int = 1000,
     sample_from_first: bool = True,
     labels: tuple[str] | None = None,
     max_zoom: int = 30,
     explore: bool = True,
     show_in_browser: bool = False,
     **kwargs,
 ) -> None:
@@ -122,15 +122,15 @@
         The maximum zoom level only works on the OpenStreetMap background map.
 
     Args:
         *gdfs: one or more GeoDataFrames.
         column: The column to color the geometries by. Defaults to None, which means
             each GeoDataFrame will get a unique color.
         size: the radius to buffer the sample point by before clipping with the data.
-            Defaults to 1500 (meters).
+            Defaults to 1000 (meters).
         sample_from_first: If True (default), the sample point is taken form the
             first specified GeoDataFrame. If False, all GeoDataFrames are considered.
         labels: By default, the GeoDataFrames will be labeled by their object names.
             Alternatively, labels can be specified as a tuple of strings the same
             length as the number of gdfs.
         max_zoom: The maximum allowed level of zoom. Higher number means more zoom
             allowed. Defaults to 30, which is higher than the geopandas default.
```

### Comparing `ssb_sgis-0.1.7/src/sgis/maps/thematicmap.py` & `ssb_sgis-0.1.8/src/sgis/maps/thematicmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -364,23 +364,14 @@
             )
             self.nan_color = "#c2c2c2"
             if not self._is_categorical:
                 self.change_cmap("RdPu", start=23)
 
         self._create_legend()
 
-    def __getitem__(self, item):
-        return getattr(self, item)
-
-    def get(self, key, default=None):
-        try:
-            return self[key]
-        except (KeyError, ValueError, IndexError, AttributeError):
-            return default
-
     @property
     def black(self):
         return self._black
 
     @black.setter
     def black(self, new_value: bool):
         self._black = new_value
```

### Comparing `ssb_sgis-0.1.7/src/sgis/networkanalysis/_get_route.py` & `ssb_sgis-0.1.8/src/sgis/networkanalysis/_get_route.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,37 +5,41 @@
 from geopandas import GeoDataFrame
 from igraph import Graph
 from pandas import DataFrame
 
 
 def _get_route(
     graph: Graph,
-    origins: GeoDataFrame,
-    destinations: GeoDataFrame,
     weight: str,
     roads: GeoDataFrame,
-    rowwise: bool = False,
+    od_pairs: pd.MultiIndex,
 ) -> GeoDataFrame:
     """Function used in the get_route method of NetworkAnalysis."""
 
     warnings.filterwarnings("ignore", category=RuntimeWarning)
 
-    od_pairs = _create_od_pairs(origins, destinations, rowwise)
-
     resultlist: list[DataFrame] = []
 
-    for ori_id, des_id in od_pairs:
-        indices = _get_one_route(graph, ori_id, des_id)
+    for ori_id in od_pairs.get_level_values(0).unique():
+        relevant_pairs = od_pairs[od_pairs.get_level_values(0) == ori_id]
+        destinations = relevant_pairs.get_level_values(1)
 
-        if not indices:
-            continue
+        res = graph.get_shortest_paths(
+            weights="weight", v=ori_id, to=destinations, output="epath"
+        )
 
-        line_ids = _create_line_id_df(indices["source_target_weight"], ori_id, des_id)
+        for i, des_id in enumerate(destinations):
+            indices = graph.es[res[i]]
 
-        resultlist.append(line_ids)
+            if not indices:
+                continue
+
+            line_ids = _create_line_id_df(indices["src_tgt_wt"], ori_id, des_id)
+
+            resultlist.append(line_ids)
 
     if not resultlist:
         warnings.warn(
             "No paths were found. Try larger search_tolerance or search_factor. "
             "Or close_network_holes() or remove_isolated()."
         )
         return pd.DataFrame(columns=["origin", "destination", weight, "geometry"])
@@ -46,25 +50,22 @@
     lines = lines.dissolve(by=["origin", "destination"], aggfunc="sum", as_index=False)
 
     return lines[["origin", "destination", weight, "geometry"]]
 
 
 def _get_k_routes(
     graph: Graph,
-    origins: GeoDataFrame,
-    destinations: GeoDataFrame,
     weight: str,
     roads: GeoDataFrame,
     k: int,
     drop_middle_percent: int,
-    rowwise: bool,
+    od_pairs: pd.MultiIndex,
 ) -> GeoDataFrame:
     """Function used in the get_k_routes method of NetworkAnalysis."""
     warnings.filterwarnings("ignore", category=RuntimeWarning)
-    od_pairs = _create_od_pairs(origins, destinations, rowwise)
 
     resultlist: list[DataFrame] = []
 
     for ori_id, des_id in od_pairs:
         k_lines: DataFrame = _loop_k_routes(
             graph, ori_id, des_id, k, drop_middle_percent
         )
@@ -89,95 +90,66 @@
     )
 
     return lines[["origin", "destination", weight, "k", "geometry"]]
 
 
 def _get_route_frequencies(
     graph,
-    origins,
-    destinations,
-    rowwise,
-    roads,
-    weight_df: DataFrame | None = None,
+    roads: GeoDataFrame,
+    weight_df: DataFrame,
 ):
     """Function used in the get_route_frequencies method of NetworkAnalysis."""
     warnings.filterwarnings("ignore", category=RuntimeWarning)
-    od_pairs = _create_od_pairs(origins, destinations, rowwise)
-
-    if weight_df is not None and len(weight_df) != len(od_pairs):
-        error_message = _make_keyerror_message(rowwise, weight_df, origins)
-        raise ValueError(error_message)
 
     resultlist: list[DataFrame] = []
 
-    for ori_id, des_id in od_pairs:
-        indices = _get_one_route(graph, ori_id, des_id)
+    od_pairs = weight_df.index
 
-        if not indices:
-            continue
+    for ori_id in od_pairs.get_level_values(0).unique():
+        relevant_pairs = od_pairs[od_pairs.get_level_values(0) == ori_id]
+        destinations = relevant_pairs.get_level_values(1)
+
+        res = graph.get_shortest_paths(
+            weights="weight", v=ori_id, to=destinations, output="epath"
+        )
 
-        line_ids = DataFrame({"source_target_weight": indices["source_target_weight"]})
-        line_ids["origin"] = ori_id
-        line_ids["destination"] = des_id
-
-        if weight_df is not None:
-            try:
-                line_ids["multiplier"] = weight_df.loc[ori_id, des_id].iloc[0]
-            except KeyError as e:
-                error_message = _make_keyerror_message(rowwise, weight_df, origins)
-                raise KeyError(error_message) from e
-        else:
-            line_ids["multiplier"] = 1
+        for i, des_id in enumerate(destinations):
+            indices = graph.es[res[i]]
 
-        resultlist.append(line_ids)
+            if not indices:
+                continue
+
+            line_ids = DataFrame({"src_tgt_wt": indices["src_tgt_wt"]})
+            line_ids["origin"] = ori_id
+            line_ids["destination"] = des_id
+            line_ids["multiplier"] = weight_df.loc[ori_id, des_id].iloc[0]
+
+            resultlist.append(line_ids)
 
     summarised = (
         pd.concat(resultlist, ignore_index=True)
-        .groupby("source_target_weight")["multiplier"]
+        .groupby("src_tgt_wt")["multiplier"]
         .sum()
     )
 
-    roads["frequency"] = roads["source_target_weight"].map(summarised)
+    roads["frequency"] = roads["src_tgt_wt"].map(summarised)
 
-    roads_visited = roads.loc[
-        roads.frequency.notna(), roads.columns.difference(["source_target_weight"])
-    ]
+    roads_visited = roads.loc[roads.frequency.notna()].drop("src_tgt_wt", axis=1)
 
     return roads_visited
 
 
-def _create_od_pairs(
-    origins: GeoDataFrame, destinations: GeoDataFrame, rowwise: bool
-) -> zip | pd.MultiIndex:
-    """Get all od combinaions if not rowwise."""
-    if rowwise:
-        return zip(origins.temp_idx, destinations.temp_idx)
-    else:
-        return pd.MultiIndex.from_product([origins.temp_idx, destinations.temp_idx])
-
-
-def _get_one_route(graph: Graph, ori_id: str, des_id: str):
-    """Get the edges for one route."""
-    res = graph.get_shortest_paths(
-        weights="weight", v=ori_id, to=des_id, output="epath"
-    )
-    if not res[0]:
-        return []
-
-    return graph.es[res[0]]
-
-
 def _get_line_geometries(line_ids, roads, weight) -> GeoDataFrame:
-    road_mapper = roads.set_index(["source_target_weight"])[[weight, "geometry"]]
+    road_mapper = roads.set_index(["src_tgt_wt"])[[weight, "geometry"]]
     line_ids = line_ids.join(road_mapper)
     return GeoDataFrame(line_ids, geometry="geometry", crs=roads.crs)
 
 
-def _create_line_id_df(source_target_weight: list, ori_id, des_id) -> DataFrame:
-    line_ids = DataFrame(index=source_target_weight)
+def _create_line_id_df(src_tgt_wt: list, ori_id, des_id) -> DataFrame:
+    line_ids = DataFrame(index=src_tgt_wt)
 
     # remove edges from ori/des to the roads
     line_ids = line_ids.loc[~line_ids.index.str.endswith("_0")]
 
     line_ids["origin"] = ori_id
     line_ids["destination"] = des_id
 
@@ -192,20 +164,23 @@
     middle of the route, given with drop_middle_percent, repeat k times.
     """
     graph = graph.copy()
 
     lines: list[DataFrame] = []
 
     for i in range(k):
-        indices = _get_one_route(graph, ori_id, des_id)
-
-        if not indices:
+        res = graph.get_shortest_paths(
+            weights="weight", v=ori_id, to=des_id, output="epath"
+        )
+        if not res[0]:
             continue
 
-        line_ids = _create_line_id_df(indices["source_target_weight"], ori_id, des_id)
+        indices = graph.es[res[0]]
+
+        line_ids = _create_line_id_df(indices["src_tgt_wt"], ori_id, des_id)
         line_ids["k"] = i + 1
         lines.append(line_ids)
 
         edge_tuples = indices["edge_tuples"]
 
         n_edges_to_keep = (
             len(edge_tuples) - len(edge_tuples) * drop_middle_percent / 100
@@ -219,26 +194,7 @@
         to_be_dropped = edge_tuples[n_edges_to_keep:-n_edges_to_keep]
         graph.delete_edges(to_be_dropped)
 
     if lines:
         return pd.concat(lines)
     else:
         return pd.DataFrame()
-
-
-def _make_keyerror_message(rowwise, weight_df, origins) -> str:
-    """Add help info to error message if key in weight_df is missing.
-
-    If empty resultlist, assume all indices are wrong. Else, assume
-    """
-    error_message = (
-        "'weight_df' does not contain all indices of each OD pair combination. "
-    )
-    if not rowwise and len(weight_df) == len(origins):
-        error_message = error_message + (
-            "Did you mean to set rowwise to True? "
-            "If not, make sure weight_df contains all combinations of "
-            "origin-destination pairs. Either specified as a MultiIndex or as the "
-            "first two columns of 'weight_df'. So (0, 0), (0, 1), (1, 0), (1, 1) etc."
-        )
-
-    return error_message
```

### Comparing `ssb_sgis-0.1.7/src/sgis/networkanalysis/_od_cost_matrix.py` & `ssb_sgis-0.1.8/src/sgis/networkanalysis/_od_cost_matrix.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.7/src/sgis/networkanalysis/_points.py` & `ssb_sgis-0.1.8/src/sgis/networkanalysis/_points.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.7/src/sgis/networkanalysis/_service_area.py` & `ssb_sgis-0.1.8/src/sgis/networkanalysis/_service_area.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ) -> GeoDataFrame:
     # make sure the nodes are alligned with the vertices in the graph
     node_df = pd.DataFrame(index=np.array(graph.vs["name"]))
     nodes = nodes.set_index("node_id").drop("geometry", axis=1)
     nodes = node_df.join(nodes)
 
     # double edge df with source/target as index
-    edge_df = lines.loc[:, ["source", "target", "source_target_weight", "geometry"]]
+    edge_df = lines.loc[:, ["source", "target", "src_tgt_wt", "geometry"]]
     edge_df = pd.concat(
         [
             edge_df.set_index("source", drop=False),
             edge_df.set_index("target", drop=False),
         ]
     )
```

### Comparing `ssb_sgis-0.1.7/src/sgis/networkanalysis/directednetwork.py` & `ssb_sgis-0.1.8/src/sgis/networkanalysis/directednetwork.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,21 +12,20 @@
 
 class DirectedNetwork(Network):
     """Class for preparing line data for directed network analysis.
 
     Can be used as the 'network' parameter in the NetworkAnalysis class for directed
     network analysis.
 
-    The DirectedNetwork class differs from the Network base class in two ways:
-    1) using a DirectedNetwork in the NetworkAnalysis class means the network graph
-    will be directed, meaning you can only travel in one direction on each line.
-    2) the class holds methods for making the network directed, mainly the
-    'make_directed_network' method, which reverses lines going the wrong direction
-    and duplicates and flips lines going both directions. It also creates a 'minute'
-    column.
+    The DirectedNetwork class has all the methods of the base Network class,
+    plus additional methods for making the network directed. If a DirectedNetwork
+    instance is used in NetworkAnalysis, the network graph will be directed,
+    meaning the lines can only be traversed in one direction. The network should
+    be make properly directed with the 'make_directed_network' method, or
+    'make_directed_network_norway' for Norwegian road data.
 
     Args:
         gdf: a GeoDataFrame of line geometries.
         **kwargs: keyword arguments taken by the base class Network.
 
     Attributes:
         gdf: the GeoDataFrame of lines with source and target ids.
```

### Comparing `ssb_sgis-0.1.7/src/sgis/networkanalysis/network.py` & `ssb_sgis-0.1.8/src/sgis/networkanalysis/network.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.7/src/sgis/networkanalysis/network_norway.py` & `ssb_sgis-0.1.8/src/sgis/networkanalysis/network_norway.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.7/src/sgis/networkanalysis/networkanalysis.py` & `ssb_sgis-0.1.8/src/sgis/networkanalysis/networkanalysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,34 +27,29 @@
 from .networkanalysisrules import NetworkAnalysisRules
 
 
 class NetworkAnalysis:
     """Class for doing network analysis.
 
     The class takes a (Directed)Network and rules for the analyses
-    (NetworkAnalysisRules), and holds methods that calculate travel times/costs,
-    route geometries or travel frequencies.
+    (NetworkAnalysisRules), and holds methods for doing network analysis
+    based on GeoDataFrames of origin and destination points.
 
-    The analysis methods take a GeoDataFrame of origin points and a GeoDataFrame of
-    destination points. The exception is the service_area methods, which take only
-    origins. The travel cost or route between each OD (origin-destination) pair is
-    calculated and returned in a (Geo)DataFrame with the columns 'origin',
-    'destination' and the cost between the OD pairs. The route methods also return a
-    geometry column.
-
-    The methods use the index of the origins and destinations as values in the
-    resulting DataFrames. To use a column instead, use the pandas set_index method
-    inside the method call.
+    The 'od_cost_matrix' method is the fastest, and returns a DataFrame with only
+    indices and travel costs between each origin-destination pair.
 
-    The 'get_route_frequencies' method is a bit different. It returns the individual
-    line segments that were visited with a column for how many times the segments
-    were used.
+    The 'get_route' method does the same, but also returns the line geometry of the
+    routes. 'get_k_routes' can be used to find multiple routes between each OD pair.
+
+    The service_area methods only take a set of origins, and return the lines that
+    can be reached within one or more breaks.
 
-    Also, the service area methods do not do calculations for OD pairs, but from either
-    origins to all roads or all roads to destinations.
+    The 'get_route_frequencies' method is a bit different. It returns the individual
+    line segments that were visited with an added column for how many times the
+    segments were used.
 
     Args:
         network: either the base Network class or a subclass, chiefly the
             DirectedNetwork class. The network can be customized beforehand, or
             accessed through the 'network' attribute of this class.
         rules: NetworkAnalysisRules class instance.
         log: If True (default), a DataFrame with information about each
@@ -140,14 +135,16 @@
 
         self._update_wkts()
         self.rules._update_rules()
 
         if log:
             self.log = DataFrame()
 
+        self._graph_updated_count = 0
+
     def _check_if_holes_are_nan(self):
         HOLES_ARE_NAN = (
             "Network holes have been filled by straigt lines, but the rows have "
             f"NaN values in the {self.rules.weight!r} column. Either remove NaNs "
             "or fill these values with a numeric value (e.g. 0)."
         )
         if hasattr(self.network, "_hole_col") and all(
@@ -198,15 +195,14 @@
         >>> nw = sg.DirectedNetwork(roads).remove_isolated().make_directed_network_norway()
         >>> rules = sg.NetworkAnalysisRules(weight="minutes")
         >>> nwa = sg.NetworkAnalysis(network=nw, rules=rules, detailed_log=False)
 
         Create some origin and destination points.
 
         >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
-
         >>> origins = points.loc[:99, ["geometry"]]
         >>> origins
                                   geometry
         0   POINT (263122.700 6651184.900)
         1   POINT (272456.100 6653369.500)
         2   POINT (270082.300 6653032.700)
         3   POINT (259804.800 6650339.700)
@@ -214,15 +210,14 @@
         ..                             ...
         95  POINT (270348.000 6651899.400)
         96  POINT (264845.600 6649005.800)
         97  POINT (263162.000 6650732.200)
         98  POINT (272322.700 6653729.100)
         99  POINT (265622.800 6644644.200)
         [100 rows x 1 columns]
-
         >>> destinations = points.loc[100:199, ["geometry"]]
         >>> destinations
                                    geometry
         100  POINT (265997.900 6647899.400)
         101  POINT (263835.200 6648677.700)
         102  POINT (265764.000 6644063.900)
         103  POINT (265970.700 6651258.500)
@@ -251,15 +246,16 @@
         9997      99          197  19.977029
         9998      99          198  15.233163
         9999      99          199   6.439002
         [10000 rows x 3 columns]
 
         Join the results onto the 'origins' GeoDataFrame via the index.
 
-        >>> joined = origins.join(od.set_index("origin"))
+        >>> od = od.set_index("origin")
+        >>> joined = origins.join(od)
         >>> joined
                                   geometry  destination    minutes
         0   POINT (263122.700 6651184.900)          100   8.765621
         0   POINT (263122.700 6651184.900)          101   6.383407
         0   POINT (263122.700 6651184.900)          102  13.482324
         0   POINT (263122.700 6651184.900)          103   6.410121
         0   POINT (263122.700 6651184.900)          104   5.882124
@@ -270,15 +266,15 @@
         99  POINT (265622.800 6644644.200)          198  15.233163
         99  POINT (265622.800 6644644.200)          199   6.439002
         [10000 rows x 3 columns]
 
         Get travel times below 10 minutes.
 
         >>> less_than_10_min = od.loc[od.minutes < 10]
-        >>> joined = origins.join(less_than_10_min.set_index("origin"))
+        >>> joined = origins.join(less_than_10_min)
         >>> joined
                                   geometry  destination   minutes
         0   POINT (263122.700 6651184.900)        100.0  8.765621
         0   POINT (263122.700 6651184.900)        101.0  6.383407
         0   POINT (263122.700 6651184.900)        103.0  6.410121
         0   POINT (263122.700 6651184.900)        104.0  5.882124
         0   POINT (263122.700 6651184.900)        106.0  9.811828
@@ -289,15 +285,15 @@
         99  POINT (265622.800 6644644.200)        183.0  8.449906
         99  POINT (265622.800 6644644.200)        199.0  6.439002
         [2195 rows x 3 columns]
 
         Get the three fastest routes from each origin.
 
         >>> three_fastest = od.loc[od.groupby("origin")["minutes"].rank() <= 3]
-        >>> joined = origins.join(three_fastest.set_index("origin"))
+        >>> joined = origins.join(three_fastest)
         >>> joined
                                   geometry  destination   minutes
         0   POINT (263122.700 6651184.900)        135.0  0.966702
         0   POINT (263122.700 6651184.900)        175.0  2.202638
         0   POINT (263122.700 6651184.900)        188.0  2.931595
         1   POINT (272456.100 6653369.500)        171.0  2.918100
         1   POINT (272456.100 6653369.500)        184.0  2.754545
@@ -305,15 +301,15 @@
         98  POINT (272322.700 6653729.100)        184.0  3.175472
         98  POINT (272322.700 6653729.100)        189.0  3.179428
         99  POINT (265622.800 6644644.200)        102.0  1.648705
         99  POINT (265622.800 6644644.200)        134.0  1.116209
         99  POINT (265622.800 6644644.200)        156.0  1.368926
         [294 rows x 3 columns]
 
-        Assign aggregated values directly onto the origins via the index.
+        Assign aggregated values directly onto the origins.
 
         >>> origins["minutes_mean"] = od.groupby("origin")["minutes"].mean()
         >>> origins
                                   geometry  minutes_mean
         0   POINT (263122.700 6651184.900)     11.628637
         1   POINT (272456.100 6653369.500)     16.084722
         2   POINT (270082.300 6653032.700)     15.304246
@@ -326,47 +322,50 @@
         98  POINT (272322.700 6653729.100)     17.579399
         99  POINT (265622.800 6644644.200)     12.185800
         [100 rows x 2 columns]
 
         Use set_index to use column as identifier insted of the index.
 
         >>> origins["areacode"] = np.random.choice(["0301", "4601", "3401"], len(origins))
-        >>> od = nwa.od_cost_matrix(origins.set_index("areacode"), destinations)
+        >>> od = nwa.od_cost_matrix(
+        ...    origins.set_index("areacode"),
+        ...    destinations
+        ... )
         >>> od
              origin  destination    minutes
-        0         a          100   8.765621
-        1         a          101   6.383407
-        2         a          102  13.482324
-        3         a          103   6.410121
-        4         a          104   5.882124
+        0      0301          100   8.765621
+        1      0301          101   6.383407
+        2      0301          102  13.482324
+        3      0301          103   6.410121
+        4      0301          104   5.882124
         ...     ...          ...        ...
-        9995      b          195  20.488644
-        9996      b          196  16.721241
-        9997      b          197  19.977029
-        9998      b          198  15.233163
-        9999      b          199   6.439002
+        9995   3401          195  20.488644
+        9996   3401          196  16.721241
+        9997   3401          197  19.977029
+        9998   3401          198  15.233163
+        9999   3401          199   6.439002
         [10000 rows x 3 columns]
 
         Travel time from 1000 to 1000 points rowwise.
 
-        >>> points_reversed = points.iloc[::-1].reset_index(drop=True)
+        >>> points_reversed = points.iloc[::-1]
         >>> od = nwa.od_cost_matrix(points, points_reversed, rowwise=True)
         >>> od
              origin  destination    minutes
-        0         0            0  14.692667
-        1         1            1   8.452691
-        2         2            2  16.370569
-        3         3            3   9.486131
-        4         4            4  16.521346
+        0         0          999  14.692667
+        1         1          998   8.452691
+        2         2          997  16.370569
+        3         3          996   9.486131
+        4         4          995  16.521346
         ..      ...          ...        ...
-        995     995          995  16.794610
-        996     996          996   9.611700
-        997     997          997  19.968743
-        998     998          998   9.484374
-        999     999          999  14.892648
+        995     995            4  16.794610
+        996     996            3   9.611700
+        997     997            2  19.968743
+        998     998            1   9.484374
+        999     999            0  14.892648
         [1000 rows x 3 columns]
 
         """
         if self._log:
             time_ = perf_counter()
 
         self._prepare_network_analysis(origins, destinations, rowwise)
@@ -402,14 +401,15 @@
         return results
 
     def get_route_frequencies(
         self,
         origins: GeoDataFrame,
         destinations: GeoDataFrame,
         weight_df: DataFrame | None = None,
+        default_weight: int | float | None = None,
         rowwise: bool = False,
         frequency_col: str = "frequency",
     ) -> GeoDataFrame:
         """Finds the number of times each line segment was visited in all trips.
 
         Finds the route with the lowest cost (minutes, meters, etc.) from a set of
         origins to a set of destinations and summarises the number of times each
@@ -437,35 +437,36 @@
             individual routes.
 
         Note:
             The resulting lines will keep all columns of the 'gdf' of the Network.
 
         Raises:
             ValueError: If no paths were found.
-            ValueError: If weight_df is not a DataFrame with one or three columns.
-            ValueError: If weight_df is given and the index of origins/destinations
-                is not unique.
+            ValueError: If weight_df is not a DataFrame with one or three columns
+                that contain all indices of 'origins' and 'destinations'.
 
         Examples
         --------
         Create the NetworkAnalysis instance.
 
         >>> import sgis as sg
         >>> import pandas as pd
         >>> roads = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/roads_oslo_2022.parquet")
         >>> nw = sg.DirectedNetwork(roads).remove_isolated().make_directed_network_norway()
         >>> rules = sg.NetworkAnalysisRules(weight="minutes")
         >>> nwa = sg.NetworkAnalysis(network=nw, rules=rules, detailed_log=False)
 
-        Get number of times each road was visited for trips from 25 to 25 points.
+        Get some points.
 
         >>> points = sg.read_parquet_url("https://media.githubusercontent.com/media/statisticsnorway/ssb-sgis/main/tests/testdata/points_oslo.parquet")
-
         >>> origins = points.iloc[:25]
         >>> destinations = points.iloc[25:50]
+
+        Get number of times each road was visited for trips from 25 to 25 points.
+
         >>> frequencies = nwa.get_route_frequencies(origins, destinations)
         >>> frequencies[["source", "target", "frequency", "geometry"]]
                source target  frequency                                           geometry
         160188  77264  79112        1.0  LINESTRING Z (268641.225 6651871.624 111.355, ...
         153682  68376   4136        1.0  LINESTRING Z (268542.700 6652162.400 121.266, ...
         153679  75263  75502        1.0  LINESTRING Z (268665.600 6652165.400 117.466, ...
         153678  75262  75263        1.0  LINESTRING Z (268660.000 6652167.100 117.466, ...
@@ -546,34 +547,50 @@
            49      10
 
         """
         if self._log:
             time_ = perf_counter()
 
         if weight_df is not None:
-            weight_df = self._prepare_weight_df(weight_df, origins, destinations)
+            weight_df = self._prepare_weight_df(weight_df)
+            od_pairs = self._create_od_pairs(origins, destinations, rowwise=rowwise)
+            self._make_sure_unique(weight_df, od_pairs)
+
+            weights_mapped = od_pairs.map(weight_df.iloc[:, 0])
+            if default_weight:
+                weights_mapped = weights_mapped.fillna(default_weight)
+            else:
+                self._make_sure_index_match(weight_df, od_pairs)
+            weight_df = DataFrame(index=od_pairs)
+            weight_df["weight"] = weights_mapped
 
         self._prepare_network_analysis(origins, destinations, rowwise)
 
         if weight_df is not None:
+            # map to temporary ids
             ori_idx_mapper = {v: k for k, v in self.origins.idx_dict.items()}
             des_idx_mapper = {v: k for k, v in self.destinations.idx_dict.items()}
             multiindex_mapper = lambda x: (
                 ori_idx_mapper.get(x[0]),
                 des_idx_mapper.get(x[1]),
             )
             weight_df.index = weight_df.index.map(multiindex_mapper)
+        else:
+            od_pairs = self._create_od_pairs(
+                self.origins.gdf.set_index("temp_idx"),
+                self.destinations.gdf.set_index("temp_idx"),
+                rowwise=rowwise,
+            )
+            weight_df = DataFrame(index=od_pairs)
+            weight_df["weight"] = 1
 
         results = _get_route_frequencies(
             graph=self.graph,
-            origins=self.origins.gdf,
-            destinations=self.destinations.gdf,
             roads=self.network.gdf,
             weight_df=weight_df,
-            rowwise=rowwise,
         )
 
         if isinstance(results, GeoDataFrame):
             results = _push_geom_col(results)
 
         results = results.rename(columns={"frequency": frequency_col}).sort_values(
             frequency_col
@@ -651,21 +668,25 @@
         [997 rows x 4 columns]
         """
         if self._log:
             time_ = perf_counter()
 
         self._prepare_network_analysis(origins, destinations, rowwise)
 
+        od_pairs = self._create_od_pairs(
+            self.origins.gdf.set_index("temp_idx"),
+            self.destinations.gdf.set_index("temp_idx"),
+            rowwise=rowwise,
+        )
+
         results = _get_route(
             graph=self.graph,
-            origins=self.origins.gdf,
-            destinations=self.destinations.gdf,
             weight=self.rules.weight,
             roads=self.network.gdf,
-            rowwise=rowwise,
+            od_pairs=od_pairs,
         )
 
         results["origin"] = results["origin"].map(self.origins.idx_dict)
         results["destination"] = results["destination"].map(self.destinations.idx_dict)
 
         if self.rules.split_lines:
             self._unsplit_network()
@@ -794,21 +815,25 @@
             raise ValueError("'drop_middle_percent' should be between 0 and 100")
 
         if self._log:
             time_ = perf_counter()
 
         self._prepare_network_analysis(origins, destinations, rowwise)
 
+        od_pairs = self._create_od_pairs(
+            self.origins.gdf.set_index("temp_idx"),
+            self.destinations.gdf.set_index("temp_idx"),
+            rowwise=rowwise,
+        )
+
         results = _get_k_routes(
             graph=self.graph,
-            origins=self.origins.gdf,
-            destinations=self.destinations.gdf,
             weight=self.rules.weight,
             roads=self.network.gdf,
-            rowwise=rowwise,
+            od_pairs=od_pairs,
             k=k,
             drop_middle_percent=drop_middle_percent,
         )
 
         results["origin"] = results["origin"].map(self.origins.idx_dict)
         results["destination"] = results["destination"].map(self.destinations.idx_dict)
 
@@ -916,15 +941,15 @@
             lines=self.network.gdf,
             nodes=self.network.nodes,
             directed=self.network._as_directed,
             precice=False,
         )
 
         if not all(results.geometry.isna()):
-            results = results.drop_duplicates(["source_target_weight", "origin"])
+            results = results.drop_duplicates(["src_tgt_wt", "origin"])
 
             if dissolve:
                 results = results.dissolve(by=["origin", self.rules.weight]).loc[
                     :, ["geometry"]
                 ]
 
             results = results.reset_index()
@@ -1043,15 +1068,15 @@
             lines=self.network.gdf,
             nodes=self.network.nodes,
             directed=self.network._as_directed,
             precice=True,
         )
 
         if not all(results.geometry.isna()):
-            results = results.drop_duplicates(["source_target_weight", "origin"])
+            results = results.drop_duplicates(["src_tgt_wt", "origin"])
 
             if dissolve:
                 results = results.dissolve(by=["origin", self.rules.weight]).loc[
                     :, ["geometry"]
                 ]
 
             results = results.reset_index()
@@ -1082,21 +1107,20 @@
                 breaks=breaks,
                 dissolve=dissolve,
             )
 
         return results
 
     @staticmethod
-    def _prepare_weight_df(weight_df, origins, destinations):
-        """Copy weight_df, convert to MultiIndex (if needed), then validate it.
+    def _prepare_weight_df(weight_df: DataFrame) -> DataFrame:
+        """Copy weight_df, convert to MultiIndex (if needed), check if correct shape.
 
         The weight_df needs to have a very specific shape and index. If a 3-columned df
         is given, convert the first two to a MultiIndex.
 
-        Then make sure this index matches the index of origins and destinations.
         """
         error_message = (
             "'weight_df' should be a DataFrame with the columns "
             "'origin', 'destination' and 'weight', where the first "
             "two contain the indices of the origins and destinations "
             "and the weight column contains the number to multiply "
             "the trip frequency for this origin-destination pair."
@@ -1109,43 +1133,66 @@
 
         if len(weight_df.columns) == 3:
             weight_df = weight_df.set_index(list(weight_df.columns[:2]))
 
         if len(weight_df.columns) != 1 and isinstance(weight_df.index, pd.MultiIndex):
             raise ValueError(error_message)
 
+        return weight_df
+
+    @staticmethod
+    def _make_sure_unique(weight_df: DataFrame, od_pairs: pd.MultiIndex) -> None:
+        """Make sure this index matches the index of origins and destinations."""
         if not weight_df.index.is_unique:
             raise ValueError("'weight_df' must contain only unique OD combinations.")
 
-        if not origins.index.is_unique:
+        if not od_pairs.is_unique:
             raise ValueError(
-                "The index of 'origins' must be unque when using a 'weight_df'."
+                "'origins' and 'destinations must contain only unique "
+                "indices when weight_df is specified."
             )
-        if not destinations.index.is_unique:
+
+    @staticmethod
+    def _make_sure_index_match(
+        weight_df: DataFrame,
+        od_pairs: pd.MultiIndex,
+    ):
+        """Make sure this index matches the index of origins and destinations."""
+        if not od_pairs.isin(weight_df.index).all():
+            if not od_pairs.isin(weight_df.index).any():
+                raise ValueError(
+                    "None of the origin-destination pair indices are in 'weight_df'."
+                )
             raise ValueError(
-                "The index of 'destinations' must be unque when using a 'weight_df'."
+                "Not all origin-destination pair indices are in 'weight_df'."
             )
 
-        # check if any/all indices are in origins/destinations.
-        # Doing 'any' to give better error message
-        level_0 = weight_df.index.get_level_values(0)
-        if not level_0.isin(origins.index).any():
-            raise ValueError("None of the 'origins' indices are in 'weight_df'.")
-
-        level_1 = weight_df.index.get_level_values(1)
-        if not level_1.isin(destinations.index).any():
-            raise ValueError("None of the 'destinations' indices are in 'weight_df'.")
+    @staticmethod
+    def _create_od_pairs(
+        origins: GeoDataFrame, destinations: GeoDataFrame, rowwise: bool
+    ) -> pd.MultiIndex:
+        """Get all OD combinaions without identical origin-destination geometry.
+
+        Returns a MultiIndex to be iterated over in get_route, get_k_routes and
+        get_route_frequencies. In get_route_frequencies, the MultiIndex is turned
+        into a DataFrame with a weight column.
+        """
+        if rowwise:
+            od_pairs = pd.MultiIndex.from_arrays([origins.index, destinations.index])
+        else:
+            od_pairs = pd.MultiIndex.from_product([origins.index, destinations.index])
 
-        if not level_0.isin(origins.index).all():
-            raise ValueError("Not all 'origins' indices are in 'weight_df'.")
+        geoms_ori = od_pairs.get_level_values(0).map(origins.geometry)
+        geoms_des = od_pairs.get_level_values(1).map(destinations.geometry)
+        no_identical_geoms = od_pairs[geoms_ori != geoms_des]
 
-        if not level_1.isin(destinations.index).all():
-            raise ValueError("Not all 'destinations' indices are in 'weight_df'.")
+        if not len(no_identical_geoms) and len(origins) and len(destinations):
+            raise ValueError("All origin-destination pairs have identical geometries")
 
-        return weight_df
+        return no_identical_geoms
 
     def _log_df_template(self, method: str, minutes_elapsed: float) -> DataFrame:
         """Creates a DataFrame with one row and the main columns.
 
         To be run after each network analysis.
 
         Args:
@@ -1264,14 +1311,16 @@
                 weights=weights,
                 edge_ids=ids,
                 directed=self.network._as_directed,
             )
 
             self._add_missing_vertices()
 
+            self._graph_updated_count += 1
+
         self._update_wkts()
         self.rules._update_rules()
 
     def _get_edges_and_weights(
         self,
     ) -> tuple[list[tuple[str, str]], list[float], list[str]]:
         """Creates lists of edges and weights which will be used to make the graph.
@@ -1290,17 +1339,15 @@
                     start=max(self.origins.gdf.temp_idx.astype(int)) + 1
                 )
 
         edges: list[tuple[str, str]] = self.network.get_edges()
 
         weights = list(self.network.gdf[self.rules.weight])
 
-        self.network.gdf["source_target_weight"] = self.network._create_edge_ids(
-            edges, weights
-        )
+        self.network.gdf["src_tgt_wt"] = self.network._create_edge_ids(edges, weights)
 
         edges_start, weights_start = self.origins._get_edges_and_weights(
             nodes=self.network.nodes,
             rules=self.rules,
         )
 
         edges = edges + edges_start
@@ -1398,15 +1445,15 @@
     ) -> Graph:
         """Creates an igraph Graph from a list of edges and weights."""
         assert len(edges) == len(weights)
 
         graph = igraph.Graph.TupleList(edges, directed=directed)
 
         graph.es["weight"] = weights
-        graph.es["source_target_weight"] = edge_ids
+        graph.es["src_tgt_wt"] = edge_ids
         graph.es["edge_tuples"] = edges
         graph.es["source"] = [edge[0] for edge in edges]
         graph.es["target"] = [edge[1] for edge in edges]
 
         assert min(graph.es["weight"]) >= 0
 
         return graph
@@ -1419,21 +1466,25 @@
         """
         if not hasattr(self, "graph") or not hasattr(self, "wkts"):
             return False
 
         if self.rules._rules_have_changed():
             return False
 
+        if self.network.gdf["src_tgt_wt"].isna().any():
+            return False
+
         for points in ["origins", "destinations"]:
-            if not hasattr(self.wkts, points):
+            if self[points] is None:
+                continue
+            if points not in self.wkts:
                 return False
             if self._points_have_changed(self[points].gdf, what=points):
                 return False
 
-        #        if not self.gdf["source_target_weight"].
         return True
 
     def _points_have_changed(self, points: GeoDataFrame, what: str) -> bool:
         """Check if the origins or destinations have changed.
 
         This method is best stored in the NetworkAnalysis class,
         since the point classes are instantiated each time an analysis is run.
```

### Comparing `ssb_sgis-0.1.7/src/sgis/networkanalysis/networkanalysisrules.py` & `ssb_sgis-0.1.8/src/sgis/networkanalysis/networkanalysisrules.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.7/src/sgis/read_parquet.py` & `ssb_sgis-0.1.8/src/sgis/read_parquet.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.1.7/PKG-INFO` & `ssb_sgis-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-sgis
-Version: 0.1.7
+Version: 0.1.8
 Summary: GIS functions used at Statistics Norway.
 Home-page: https://github.com/statisticsnorway/ssb-sgis
 License: MIT
 Author: Statistics Norway
 Author-email: ort@ssb.no
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 3 - Alpha
@@ -246,15 +246,15 @@
 
 ### Documentation
 
 To generate the API-documentation locally, run the following command from the root
 directory:
 
 ```shell
-poetry run sphinx-build docs docs/_build
+poetry run sphinx-build -W docs docs/_build
 ```
 
 Then open the file `docs/_build/index.html`.
 
 To check and run the docstrings examples, run this command:
 
 ```shell
```

