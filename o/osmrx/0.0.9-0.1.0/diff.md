# Comparing `tmp/osmrx-0.0.9.tar.gz` & `tmp/osmrx-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osmrx-0.0.9.tar", max compression
+gzip compressed data, was "osmrx-0.1.0.tar", max compression
```

## Comparing `osmrx-0.0.9.tar` & `osmrx-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    35149 2023-04-15 23:15:55.289173 osmrx-0.0.9/LICENSE
--rw-r--r--   0        0        0     4147 2023-04-15 23:15:55.289173 osmrx-0.0.9/README.md
--rw-r--r--   0        0        0      165 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/__init__.py
--rw-r--r--   0        0        0        0 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/apis_handler/__init__.py
--rw-r--r--   0        0        0     1346 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/apis_handler/core.py
--rw-r--r--   0        0        0     2564 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/apis_handler/models.py
--rw-r--r--   0        0        0     1768 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/apis_handler/nominatim.py
--rw-r--r--   0        0        0      570 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/apis_handler/overpass.py
--rw-r--r--   0        0        0     1499 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/apis_handler/query_builder.py
--rw-r--r--   0        0        0        0 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/data_processing/__init__.py
--rw-r--r--   0        0        0     2500 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/data_processing/overpass_data_builder.py
--rw-r--r--   0        0        0     3074 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/globals/queries.py
--rw-r--r--   0        0        0        0 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/helpers/__init__.py
--rw-r--r--   0        0        0     2551 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/helpers/logger.py
--rw-r--r--   0        0        0     1451 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/helpers/misc.py
--rw-r--r--   0        0        0     2553 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/main/core.py
--rw-r--r--   0        0        0     1114 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/main/pois.py
--rw-r--r--   0        0        0     4622 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/main/roads.py
--rw-r--r--   0        0        0        0 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/network/__init__.py
--rw-r--r--   0        0        0     2553 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/network/arc_feature.py
--rw-r--r--   0        0        0     2313 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/network/isochrones_feature.py
--rw-r--r--   0        0        0     7036 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/network/network_rx.py
--rw-r--r--   0        0        0     1068 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/network/path_feature.py
--rw-r--r--   0        0        0        0 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/topology/__init__.py
--rw-r--r--   0        0        0     1937 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/topology/checker.py
--rw-r--r--   0        0        0    15326 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/topology/cleaner.py
--rw-r--r--   0        0        0      613 2023-04-15 23:15:55.293174 osmrx-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     5222 1970-01-01 00:00:00.000000 osmrx-0.0.9/setup.py
--rw-r--r--   0        0        0     4764 1970-01-01 00:00:00.000000 osmrx-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-16 20:25:48.969476 osmrx-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4147 2023-04-16 20:25:48.969476 osmrx-0.1.0/README.md
+-rw-r--r--   0        0        0      165 2023-04-16 20:25:48.969476 osmrx-0.1.0/osmrx/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-16 20:25:48.969476 osmrx-0.1.0/osmrx/apis_handler/__init__.py
+-rw-r--r--   0        0        0     1346 2023-04-16 20:25:48.969476 osmrx-0.1.0/osmrx/apis_handler/core.py
+-rw-r--r--   0        0        0     2564 2023-04-16 20:25:48.969476 osmrx-0.1.0/osmrx/apis_handler/models.py
+-rw-r--r--   0        0        0     1768 2023-04-16 20:25:48.969476 osmrx-0.1.0/osmrx/apis_handler/nominatim.py
+-rw-r--r--   0        0        0      570 2023-04-16 20:25:48.969476 osmrx-0.1.0/osmrx/apis_handler/overpass.py
+-rw-r--r--   0        0        0     1499 2023-04-16 20:25:48.969476 osmrx-0.1.0/osmrx/apis_handler/query_builder.py
+-rw-r--r--   0        0        0        0 2023-04-16 20:25:48.969476 osmrx-0.1.0/osmrx/data_processing/__init__.py
+-rw-r--r--   0        0        0     2500 2023-04-16 20:25:48.969476 osmrx-0.1.0/osmrx/data_processing/overpass_data_builder.py
+-rw-r--r--   0        0        0     3074 2023-04-16 20:25:48.969476 osmrx-0.1.0/osmrx/globals/queries.py
+-rw-r--r--   0        0        0        0 2023-04-16 20:25:48.969476 osmrx-0.1.0/osmrx/helpers/__init__.py
+-rw-r--r--   0        0        0     2551 2023-04-16 20:25:48.969476 osmrx-0.1.0/osmrx/helpers/logger.py
+-rw-r--r--   0        0        0     1451 2023-04-16 20:25:48.969476 osmrx-0.1.0/osmrx/helpers/misc.py
+-rw-r--r--   0        0        0     2553 2023-04-16 20:25:48.969476 osmrx-0.1.0/osmrx/main/core.py
+-rw-r--r--   0        0        0     1114 2023-04-16 20:25:48.969476 osmrx-0.1.0/osmrx/main/pois.py
+-rw-r--r--   0        0        0     4623 2023-04-16 20:25:48.973476 osmrx-0.1.0/osmrx/main/roads.py
+-rw-r--r--   0        0        0        0 2023-04-16 20:25:48.973476 osmrx-0.1.0/osmrx/network/__init__.py
+-rw-r--r--   0        0        0     2553 2023-04-16 20:25:48.973476 osmrx-0.1.0/osmrx/network/arc_feature.py
+-rw-r--r--   0        0        0     2313 2023-04-16 20:25:48.973476 osmrx-0.1.0/osmrx/network/isochrones_feature.py
+-rw-r--r--   0        0        0     7036 2023-04-16 20:25:48.973476 osmrx-0.1.0/osmrx/network/network_rx.py
+-rw-r--r--   0        0        0     1191 2023-04-16 20:25:48.973476 osmrx-0.1.0/osmrx/network/path_feature.py
+-rw-r--r--   0        0        0        0 2023-04-16 20:25:48.973476 osmrx-0.1.0/osmrx/topology/__init__.py
+-rw-r--r--   0        0        0     1937 2023-04-16 20:25:48.973476 osmrx-0.1.0/osmrx/topology/checker.py
+-rw-r--r--   0        0        0    15326 2023-04-16 20:25:48.973476 osmrx-0.1.0/osmrx/topology/cleaner.py
+-rw-r--r--   0        0        0      613 2023-04-16 20:25:48.973476 osmrx-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5222 1970-01-01 00:00:00.000000 osmrx-0.1.0/setup.py
+-rw-r--r--   0        0        0     4764 1970-01-01 00:00:00.000000 osmrx-0.1.0/PKG-INFO
```

### Comparing `osmrx-0.0.9/LICENSE` & `osmrx-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.9/README.md` & `osmrx-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.9/osmrx/apis_handler/core.py` & `osmrx-0.1.0/osmrx/apis_handler/core.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.9/osmrx/apis_handler/models.py` & `osmrx-0.1.0/osmrx/apis_handler/models.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.9/osmrx/apis_handler/nominatim.py` & `osmrx-0.1.0/osmrx/apis_handler/nominatim.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.9/osmrx/apis_handler/overpass.py` & `osmrx-0.1.0/osmrx/apis_handler/overpass.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.9/osmrx/apis_handler/query_builder.py` & `osmrx-0.1.0/osmrx/apis_handler/query_builder.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.9/osmrx/data_processing/overpass_data_builder.py` & `osmrx-0.1.0/osmrx/data_processing/overpass_data_builder.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.9/osmrx/globals/queries.py` & `osmrx-0.1.0/osmrx/globals/queries.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.9/osmrx/helpers/logger.py` & `osmrx-0.1.0/osmrx/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.9/osmrx/helpers/misc.py` & `osmrx-0.1.0/osmrx/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.9/osmrx/main/core.py` & `osmrx-0.1.0/osmrx/main/core.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.9/osmrx/main/pois.py` & `osmrx-0.1.0/osmrx/main/pois.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.9/osmrx/main/roads.py` & `osmrx-0.1.0/osmrx/main/roads.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -104,8 +104,8 @@
         assert len(self._steps_nodes) == 1, "You need 1 point to compute an isochrone"
 
         for node in self._steps_nodes:
             area = buffer_point(node.y, node.x, max(intervals) + 100).bounds
             self.from_bbox(tuple([area[1], area[0], area[3], area[2]]))
             isochrones = self._graph_manager.compute_isochrone_from_distance(node, intervals, precision)
             self.logger.info(f"Isochrones {isochrones.intervals} built from {node.wkt}.")
-            return isochrones
+            return isochrones
```

### Comparing `osmrx-0.0.9/osmrx/network/arc_feature.py` & `osmrx-0.1.0/osmrx/network/arc_feature.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.9/osmrx/network/isochrones_feature.py` & `osmrx-0.1.0/osmrx/network/isochrones_feature.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.9/osmrx/network/network_rx.py` & `osmrx-0.1.0/osmrx/network/network_rx.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.9/osmrx/network/path_feature.py` & `osmrx-0.1.0/osmrx/network/path_feature.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import List, Dict
 
-from shapely import LineString
+from shapely import LineString, MultiLineString
+from shapely.ops import linemerge
 
 from osmrx.network.arc_feature import ArcFeature
 
 
 class PathFeature:
     _graph = None
     _nodes_indices = None
@@ -12,18 +13,19 @@
 
     def __init__(self, graph, nodes_indice: List[int]):
         self._graph = graph
         self._nodes_indices = nodes_indice
         self._features = self._build_features()
 
     @property
-    def path(self) -> LineString:
-        """Return the path as a LineString geometry"""
-        return LineString([self._graph.get_node_data(indice)
-                           for indice in self._nodes_indices])
+    def path(self) -> LineString | MultiLineString:
+        """ Return the path as a LineString geometry. If a MultiLineString is returned
+            it means that something wrong happened on the graph...
+        """
+        return linemerge(feat.geometry for feat in self._features)
 
     def features(self) -> List[Dict]:
         """Return each LineStrings composing the path with their attributes"""
         return [feature.to_dict(with_attr=True) for feature in self._build_features()]
 
     def _build_features(self) -> List[ArcFeature]:
         """Get all the ArcFeature composing the path found"""
```

### Comparing `osmrx-0.0.9/osmrx/topology/checker.py` & `osmrx-0.1.0/osmrx/topology/checker.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.9/osmrx/topology/cleaner.py` & `osmrx-0.1.0/osmrx/topology/cleaner.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.9/pyproject.toml` & `osmrx-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "osmrx"
-version = "0.0.9"
+version = "0.1.0"
 description = ""
 authors = ["amauryval <amauryval@gmail.com>"]
 license = ""
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.11.0"
```

### Comparing `osmrx-0.0.9/setup.py` & `osmrx-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'rustworkx[mpl]>=0.12.1,<0.13.0',
  'scipy>=1.10.1,<2.0.0',
  'setuptools>=67.6.1,<68.0.0',
  'shapely>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'osmrx',
-    'version': '0.0.9',
+    'version': '0.1.0',
     'description': '',
     'long_description': '# OsmRx\n\nA geographic Python library to extract Open Street Map roads (and POIs) from a location or a bounding box, in order to create a graph thanks to [Rustworkx](https://github.com/Qiskit/rustworkx). OsmRx is able to clean a network based on Linestring geometries and connect Point geometries. The graph built is able to process graph-analysis (shortest-path, isochrones...)\n\nCapabilities:\n* load data from a location name or a bounding box (roads and pois)\n* graph creation (and topology processing and cleaning)\n* shortest path\n* isochrone builder\n\n[![CI](https://github.com/amauryval/osmrx/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/amauryval/osmrx/actions/workflows/main.yml)\n[![codecov](https://codecov.io/gh/amauryval/osmrx/branch/master/graph/badge.svg)](https://codecov.io/gh/amauryval/osmrx)\n\n[![PyPI version](https://badge.fury.io/py/osmrx.svg)](https://badge.fury.io/py/osmrx)\n\nCheck the demo [here](https://amauryval.github.io/omsrx/)\n\n\n## How to install it ?\n\n### with pip\n\n```bash\npip install osmrx\n```\n\n## How to use it ?\n\nCheck the jupyter notebook [here](https://amauryval.github.io/OsmRx/)\n\nCheck the wiki: TODO\n\n### Get POIs\n\nFind the Points of interest from a location (Point(s)) or a bounding box: \n* OSM attributes are returned\n* features ready to be used with shapely, GeoPandas (...):\n\n\n```python\nfrom osmrx.main.pois import Pois\n\nlocation_name = "lyon"  \n\n# Initialize the Pois class\npois_object = Pois()\n# call .from_location(location: str) or .from_bbox(bounds: Tuple[float, float, float, float]) to get data from your location\npois_object.from_location(location_name)  # nominatim api is used to get Lyon coordinates\n\n# It returns a list of dictionnaries [{"geometry": Point(...), "attribute": "...", ...}\n# Free for you to use it with GeoPandas or something else (epsg=4326)\npois_data_found = pois_object.data\n```\n\n### Get Roads\n\nFind the vehicle or pedestrian network (LineString(s)) from a location or a bounding box:\n* OSM attributes available\n* OSM features ready to be used with shapely, GeoPandas (...):\n* data cleaned regarding classical topology rules\n\n```python\nfrom osmrx.main.roads import Roads\n\n# Choose the vehicle or the pedestrian network\nroads_object = Roads("vehicle")\n\n# from_location(location: str) is available\nroads_object.from_bbox({6.019674, 4.023742, 46.072575, 4.122018})\n\n# It returns a list of dictionnaries [{"geometry": Point(...), "attribute": "...", ...}\n# Free for you to use it with GeoPandas or something else (epsg=4326)\nroads_data_found = roads_object.data\n\n# return the rustworkx graph (directed for vehicle / undirected for pedestrian)\ngraph = roads_object.graph\n# Free for you to compute graph analysis\n```\n\n\n### Compute a shortest path\n\nCompute the shortest path from an ordered list of Point(s) (at least 2)\n\n```python\nfrom shapely import Point\n\nfrom osmrx.main.roads import GraphAnalysis\n\n# use the GraphAnalysis class and set:\n# the network type (pedestrian or vehicle) and an ordered list of 2 Shapely Points defining the source and the target\n# of your shortest path)\nanalysis_object = GraphAnalysis("pedestrian",\n                              [Point(4.0793058, 46.0350304), Point(4.0725246, 46.0397676)])  # (epsg=4326)\npaths_built = analysis_object.get_shortest_path()\nfor path_object in paths_built:\n    print(path_object.path)  # LineString shortest path (epsg=4326)\n    print(path_object.features())  # List of LineString (with osm attributes) composing the path found\n```\n\n\n### Compute an Isochrone\n\nBuild an isochrone (Polygon(s)) from a Point\n\n```python\nfrom shapely import Point\n\nfrom osmrx.main.roads import GraphAnalysis\n\n# use the GraphAnalysis class and set:\n# the network type (pedestrian or vehicle) and a list of one Shapely Point (epsg=4326) to build the isochone\nanalysis_object = GraphAnalysis("vehicle", [Point(4.0793058, 46.0350304)])\n\n# Set the distance intervals to compute the isochone with a list of integer or float\nisochrones_built = analysis_object.isochrones_from_distance([0, 250, 500, 1000, 1500])\n\n# List of Polygons with a distance attributes based on the intervals defined\nprint(isochrones_built.data)\n```\n\n',
     'author': 'amauryval',
     'author_email': 'amauryval@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `osmrx-0.0.9/PKG-INFO` & `osmrx-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osmrx
-Version: 0.0.9
+Version: 0.1.0
 Summary: 
 Author: amauryval
 Author-email: amauryval@gmail.com
 Requires-Python: ==3.11.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
```

