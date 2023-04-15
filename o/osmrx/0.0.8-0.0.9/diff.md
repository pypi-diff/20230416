# Comparing `tmp/osmrx-0.0.8.tar.gz` & `tmp/osmrx-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osmrx-0.0.8.tar", max compression
+gzip compressed data, was "osmrx-0.0.9.tar", max compression
```

## Comparing `osmrx-0.0.8.tar` & `osmrx-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    35149 2023-04-14 18:58:46.832824 osmrx-0.0.8/LICENSE
--rw-r--r--   0        0        0     4147 2023-04-14 18:58:46.832824 osmrx-0.0.8/README.md
--rw-r--r--   0        0        0      211 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/apis_handler/__init__.py
--rw-r--r--   0        0        0     1346 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/apis_handler/core.py
--rw-r--r--   0        0        0     2564 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/apis_handler/models.py
--rw-r--r--   0        0        0     1768 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/apis_handler/nominatim.py
--rw-r--r--   0        0        0      570 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/apis_handler/overpass.py
--rw-r--r--   0        0        0     1499 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/apis_handler/query_builder.py
--rw-r--r--   0        0        0        0 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/data_processing/__init__.py
--rw-r--r--   0        0        0     2528 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/data_processing/overpass_data_builder.py
--rw-r--r--   0        0        0     3074 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/globals/queries.py
--rw-r--r--   0        0        0        0 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/graph_manager/__init__.py
--rw-r--r--   0        0        0     2875 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/graph_manager/arc_feature.py
--rw-r--r--   0        0        0     5369 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/graph_manager/graph_manager.py
--rw-r--r--   0        0        0     2313 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/graph_manager/isochrones_feature.py
--rw-r--r--   0        0        0     1074 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/graph_manager/path_feature.py
--rw-r--r--   0        0        0        0 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/helpers/__init__.py
--rw-r--r--   0        0        0     2551 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/helpers/logger.py
--rw-r--r--   0        0        0     1451 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/helpers/misc.py
--rw-r--r--   0        0        0     2543 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/main/core.py
--rw-r--r--   0        0        0     1108 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/main/pois.py
--rw-r--r--   0        0        0     4618 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/main/roads.py
--rw-r--r--   0        0        0        0 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/topology/__init__.py
--rw-r--r--   0        0        0     1943 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/topology/checker.py
--rw-r--r--   0        0        0    15360 2023-04-14 18:58:46.832824 osmrx-0.0.8/osmrx/topology/cleaner.py
--rw-r--r--   0        0        0      614 2023-04-14 18:58:46.836824 osmrx-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5228 1970-01-01 00:00:00.000000 osmrx-0.0.8/setup.py
--rw-r--r--   0        0        0     4764 1970-01-01 00:00:00.000000 osmrx-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-15 23:15:55.289173 osmrx-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4147 2023-04-15 23:15:55.289173 osmrx-0.0.9/README.md
+-rw-r--r--   0        0        0      165 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/apis_handler/__init__.py
+-rw-r--r--   0        0        0     1346 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/apis_handler/core.py
+-rw-r--r--   0        0        0     2564 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/apis_handler/models.py
+-rw-r--r--   0        0        0     1768 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/apis_handler/nominatim.py
+-rw-r--r--   0        0        0      570 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/apis_handler/overpass.py
+-rw-r--r--   0        0        0     1499 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/apis_handler/query_builder.py
+-rw-r--r--   0        0        0        0 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/data_processing/__init__.py
+-rw-r--r--   0        0        0     2500 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/data_processing/overpass_data_builder.py
+-rw-r--r--   0        0        0     3074 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/globals/queries.py
+-rw-r--r--   0        0        0        0 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/helpers/__init__.py
+-rw-r--r--   0        0        0     2551 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/helpers/logger.py
+-rw-r--r--   0        0        0     1451 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/helpers/misc.py
+-rw-r--r--   0        0        0     2553 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/main/core.py
+-rw-r--r--   0        0        0     1114 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/main/pois.py
+-rw-r--r--   0        0        0     4622 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/main/roads.py
+-rw-r--r--   0        0        0        0 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/network/__init__.py
+-rw-r--r--   0        0        0     2553 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/network/arc_feature.py
+-rw-r--r--   0        0        0     2313 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/network/isochrones_feature.py
+-rw-r--r--   0        0        0     7036 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/network/network_rx.py
+-rw-r--r--   0        0        0     1068 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/network/path_feature.py
+-rw-r--r--   0        0        0        0 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/topology/__init__.py
+-rw-r--r--   0        0        0     1937 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/topology/checker.py
+-rw-r--r--   0        0        0    15326 2023-04-15 23:15:55.289173 osmrx-0.0.9/osmrx/topology/cleaner.py
+-rw-r--r--   0        0        0      613 2023-04-15 23:15:55.293174 osmrx-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5222 1970-01-01 00:00:00.000000 osmrx-0.0.9/setup.py
+-rw-r--r--   0        0        0     4764 1970-01-01 00:00:00.000000 osmrx-0.0.9/PKG-INFO
```

### Comparing `osmrx-0.0.8/LICENSE` & `osmrx-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.8/README.md` & `osmrx-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.8/osmrx/apis_handler/core.py` & `osmrx-0.0.9/osmrx/apis_handler/core.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.8/osmrx/apis_handler/models.py` & `osmrx-0.0.9/osmrx/apis_handler/models.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.8/osmrx/apis_handler/nominatim.py` & `osmrx-0.0.9/osmrx/apis_handler/nominatim.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.8/osmrx/apis_handler/overpass.py` & `osmrx-0.0.9/osmrx/apis_handler/overpass.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.8/osmrx/apis_handler/query_builder.py` & `osmrx-0.0.9/osmrx/apis_handler/query_builder.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.8/osmrx/data_processing/overpass_data_builder.py` & `osmrx-0.0.9/osmrx/data_processing/overpass_data_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import List
 
 from shapely import Point
 from shapely import LineString
 
 from osmrx.globals.queries import OsmFeatureTypes
 
-TOPO_FIELD: str = "topo_uuid"
 ID_OSM_FIELD: str = "id"
 
 
 class OverpassDataBuilder:
     __GEOMETRY_FIELD: str = "geometry"
     __LAT_FIELD: str = "lat"
     __LNG_FIELD: str = "lon"
@@ -59,10 +58,10 @@
     def _build_properties(self, uuid_enum: int, geometry: Point | LineString, properties: Dict) -> Dict:
         tags_attributes = properties.get(self.__PROPERTIES_OSM_FIELD, {})
         return {
             **tags_attributes,
             ID_OSM_FIELD: str(properties[ID_OSM_FIELD]),
             self.__OSM_URL_FIELD: f"{self.__OSM_URL}/{properties[self.__FEATURE_TYPE_OSM_FIELD]}/"
                                   f"{properties[ID_OSM_FIELD]}",
-            TOPO_FIELD: uuid_enum,  # do not cast to str, because topology processing need an int
+            # TOPO_FIELD: uuid_enum,  # do not cast to str, because topology processing need an int
             self.__GEOMETRY_FIELD: geometry
         }
```

### Comparing `osmrx-0.0.8/osmrx/globals/queries.py` & `osmrx-0.0.9/osmrx/globals/queries.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.8/osmrx/graph_manager/arc_feature.py` & `osmrx-0.0.9/osmrx/network/arc_feature.py`

 * *Files 11% similar despite different names*

```diff
@@ -84,15 +84,7 @@
             "topo_status": self.topo_status,
             "geometry": self.geometry,
             "direction": self.direction,
         }
         if with_attr:
             return main_attrs | self.attributes
         return main_attrs
-
-    def is_junction_or_roundabout(self) -> bool:
-        """Check if arc is a junction or a roundabout"""
-        return self.attributes.get("junction", None) in ["roundabout", "jughandle"]
-
-    def is_oneway(self) -> bool:
-        """Check if direction arc"""
-        return self.attributes.get("oneway", None) == "yes"
```

### Comparing `osmrx-0.0.8/osmrx/graph_manager/graph_manager.py` & `osmrx-0.0.9/osmrx/network/network_rx.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,51 @@
 import copy
 from typing import List, Dict
 from typing import TYPE_CHECKING
 
 import rustworkx as rx
 from shapely import Point
 
-from osmrx.graph_manager.isochrones_feature import IsochronesFeature
-from osmrx.graph_manager.path_feature import PathFeature
+from osmrx.helpers.logger import Logger
+from osmrx.network.isochrones_feature import IsochronesFeature
+from osmrx.network.path_feature import PathFeature
 from osmrx.topology.cleaner import TopologyCleaner
 
 from osmrx.globals.queries import OsmFeatureModes
 
 if TYPE_CHECKING:
-    from osmrx.graph_manager.arc_feature import ArcFeature
+    from osmrx.network.arc_feature import ArcFeature
 
 
 class GraphCore:
+    """Class dedicated to manage/wrappe graph function"""
 
     def __init__(self, directed: bool = False):
+        self.logger = None
         self._graph = None
         self._nodes_mapping = {}
         self._edges_mapping = {}
-        self._directed = directed
+        self.directed = directed
 
         if directed:
             self._graph = rx.PyDiGraph(multigraph=False)  # noqa
         else:
             self._graph = rx.PyGraph(multigraph=False)  # noqa
 
     @property
+    def directed(self) -> bool:
+        """Return if the graph is directed"""
+        return self._directed
+
+    @directed.setter
+    def directed(self, directed: bool):
+        """Set the directed graph status"""
+        self._directed = directed
+
+    @property
     def graph(self) -> rx.PyDiGraph | rx.PyGraph:
         """Return the graph"""
         return self._graph
 
     def _add_nodes(self, node_value: Point) -> int:
         """Add a node"""
         if node_value not in self._nodes_mapping:
@@ -82,73 +95,104 @@
             edges = rx.dijkstra_shortest_path_lengths(self.graph, from_node_indice, weight_attribute_func)
 
         iso_session = IsochronesFeature(from_node, precision)
         iso_session.from_distances(intervals)
         iso_session.build(self.graph, edges)
         return iso_session
 
+    def _build_data_and_graph(self):
 
-class GraphManager(GraphCore):
+        self._features = self.graph.edges()
+        self.logger.info("Graph built")
 
-    def __init__(self, logger, mode: OsmFeatureModes):
-        self._mode = mode
 
-        super().__init__(directed=self.directed)
+class NetworkRxCore(GraphCore):
+    """Base class to build a graph from data"""
+    def __init__(self, directed: bool = False, logger: Logger | None = None):
 
-        self.logger = logger  # TODO: add a logger if not set
+        super().__init__(directed=directed)
 
         self._features = None
+
         self._connected_nodes = None
+        self._line_features = []  # TODO support None value
+
+        if logger is None:
+            self.logger = Logger().logger
+        else:
+            self.logger = logger  # TODO: add a logger if not set
 
     @property
-    def directed(self) -> bool:
-        """Return the graph mode"""
-        if self._mode == OsmFeatureModes.vehicle:
-            return True
-        return False
+    def line_features(self) -> List[Dict]:
+        """return the connected nodes added"""
+        return self._line_features
+
+    @line_features.setter
+    def line_features(self, line_features: List[Dict]):
+        """Set the nodes to connect on the network and build the graph
+        Be careful, set the connected nodes before using this function"""
+        self._line_features = line_features
+        self._build_data_and_graph()
 
     @property
     def connected_nodes(self) -> List[Dict] | None:
         """return the connected nodes added"""
         return self._connected_nodes
 
     @connected_nodes.setter
     def connected_nodes(self, connected_nodes: List[Dict]):
-        """Set the nodes to connect on the network"""
+        """Set the nodes to connect on the network, avoid to add duplicated nodes"""
         self._connected_nodes = connected_nodes
 
     @property
     def features(self) -> "List[ArcFeature]":
         """Return the graph features from the graph"""
         return self._features
 
-    @features.setter
-    def features(self, network_data: List[Dict] | None):
-        # TODO: improve name
-        arc_features = TopologyCleaner(self.logger, network_data, self._connected_nodes, None).run()
+    def _build_data_and_graph(self):
+        """Topology cleaning and graph building"""
+        # TODO remove ids attributes constraint on TopologyCleaner
+        arc_features = TopologyCleaner(self.logger, self._line_features, self.connected_nodes, 
+                                       None).build_arc_features()
 
-        _ = [self._build_graph(arc_feature)
+        _ = [self._adding_edge(arc_feature)
              for arc_feature in arc_features]
+        super()._build_data_and_graph()
 
-        self._features = self.graph.edges()
-        self.logger.info("Graph built")
-
-    def _build_graph(self, arc_feature: "ArcFeature"):
-
+    def _adding_edge(self, arc_feature: "ArcFeature"):
+        """Add edge on graph function"""
         self.add_edge(
             arc_feature.from_point,
             arc_feature.to_point,
             arc_feature
         )
+
+
+class OsmNetworkManager(NetworkRxCore):
+    """Class to build a graph from OSM data regarding its attributes"""
+
+    def __init__(self, mode: OsmFeatureModes, logger: Logger | None = None):
+        self._mode = mode
+
+        super().__init__(directed=mode == OsmFeatureModes.vehicle,
+                         logger=logger)
+
+    @property
+    def mode(self) -> OsmFeatureModes:
+        return self._mode
+
+    def _adding_edge(self, arc_feature: "ArcFeature"):
+        super()._adding_edge(arc_feature=arc_feature)
+
         if self._mode == OsmFeatureModes.vehicle:
-            if arc_feature.is_junction_or_roundabout():
+            if arc_feature.attributes.get("junction", None) in ["roundabout", "jughandle"]:
                 # do nothing
                 return
 
-            if not arc_feature.is_oneway():
+            if not arc_feature.attributes.get("oneway", None) == "yes":
                 arc_feature_backward = copy.deepcopy(arc_feature)
                 arc_feature_backward.direction = "backward"
                 self.add_edge(
                     arc_feature_backward.from_point,
                     arc_feature_backward.to_point,
                     arc_feature_backward
                 )
```

### Comparing `osmrx-0.0.8/osmrx/graph_manager/isochrones_feature.py` & `osmrx-0.0.9/osmrx/network/isochrones_feature.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.8/osmrx/graph_manager/path_feature.py` & `osmrx-0.0.9/osmrx/network/path_feature.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Dict
 
 from shapely import LineString
 
-from osmrx.graph_manager.arc_feature import ArcFeature
+from osmrx.network.arc_feature import ArcFeature
 
 
 class PathFeature:
     _graph = None
     _nodes_indices = None
     _features = None
```

### Comparing `osmrx-0.0.8/osmrx/helpers/logger.py` & `osmrx-0.0.9/osmrx/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.8/osmrx/helpers/misc.py` & `osmrx-0.0.9/osmrx/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `osmrx-0.0.8/osmrx/main/core.py` & `osmrx-0.0.9/osmrx/main/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from osmrx.apis_handler.models import Bbox, Location
 from osmrx.apis_handler.overpass import OverpassApi
 from osmrx.apis_handler.query_builder import QueryBuilder
-from osmrx.graph_manager.graph_manager import GraphManager
+from osmrx.network.network_rx import OsmNetworkManager
 from osmrx.helpers.logger import Logger
 from osmrx.data_processing.overpass_data_builder import OverpassDataBuilder
 from osmrx.globals.queries import OsmFeatureModes
 
 
-class OsmNetworkCore(Logger):
+class OsmNetworkHandler(Logger):
 
     def __init__(self, osm_feature_mode: str):
         self._geo_filter = None
         self._query = None
         self._raw_data = None
-        self._graph_manager: GraphManager | None = None
+        self._graph_manager: OsmNetworkManager | None = None
 
         super().__init__()
 
         self.osm_feature_mode = OsmFeatureModes[osm_feature_mode]
 
     @property
     def osm_feature_mode(self) -> OsmFeatureModes:
@@ -27,15 +27,15 @@
     @osm_feature_mode.setter
     def osm_feature_mode(self, feature_mode: OsmFeatureModes) -> None:
         """Set the osm feature type to use"""
         self._osm_feature_mode = feature_mode
         self.logger.info(f"Building {self._osm_feature_mode} Data")
         self._build_query()
         if feature_mode != OsmFeatureModes.poi:
-            self._graph_manager = GraphManager(self.logger, feature_mode)
+            self._graph_manager = OsmNetworkManager(feature_mode, self.logger)
 
     @property
     def geo_filter(self) -> Bbox | Location:
         """Return the geo filter"""
         return self._geo_filter
 
     @geo_filter.setter
@@ -65,8 +65,8 @@
     @property
     def data(self) -> None:
         raise NotImplemented
 
     def _execute(self):
         base_query = self._build_query()
         self._query = base_query.from_geo_filter(self.geo_filter)
-        self._execute_query()
+        self._execute_query()
```

### Comparing `osmrx-0.0.8/osmrx/main/pois.py` & `osmrx-0.0.9/osmrx/main/pois.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Tuple, List, Dict
 
 from osmrx.apis_handler.models import Bbox, Location
 from osmrx.globals.queries import OsmFeatureModes
-from osmrx.main.core import OsmNetworkCore
+from osmrx.main.core import OsmNetworkHandler
 
 
-class OsmNetworkPoi(OsmNetworkCore):
+class OsmNetworkPoi(OsmNetworkHandler):
 
     def __init__(self):
         super().__init__(osm_feature_mode=OsmFeatureModes.poi.value)
 
     def _execute_query(self) -> None:
         """Execute the query with the Overpass API"""
         raw_data = super()._execute_query()
```

### Comparing `osmrx-0.0.8/osmrx/main/roads.py` & `osmrx-0.0.9/osmrx/main/roads.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from typing import Tuple, List, Dict, Any, Generator
 
 from shapely import Point, MultiPoint
 import rustworkx as rx
 
 from osmrx.apis_handler.models import Location, Bbox
-from osmrx.graph_manager.isochrones_feature import IsochronesFeature
-from osmrx.graph_manager.path_feature import PathFeature
+from osmrx.network.isochrones_feature import IsochronesFeature
+from osmrx.network.path_feature import PathFeature
 from osmrx.helpers.misc import buffer_point
-from osmrx.main.core import OsmNetworkCore
+from osmrx.main.core import OsmNetworkHandler
 from osmrx.topology.checker import TopologyChecker
 
 
-class OsmNetworkRoads(OsmNetworkCore):
+class OsmNetworkRoads(OsmNetworkHandler):
 
     def __init__(self, osm_feature_mode: str, nodes_to_connect: List[Dict] | None = None) -> None:
         super().__init__(osm_feature_mode=osm_feature_mode)
         self._graph_manager.connected_nodes = nodes_to_connect
 
     def _execute_query(self) -> None:
         """Execute the query with the Overpass API"""
@@ -27,15 +27,15 @@
     def additional_nodes(self) -> List[Dict] | None:
         """return the nodes defined to connect on the network"""
         return self._graph_manager.connected_nodes
 
     def _build_graph(self) -> None:
         """Fix topology issues for LineString features and build graph"""
         if self._raw_data is not None:
-            self._graph_manager.features = self._raw_data
+            self._graph_manager.line_features = self._raw_data
 
     def topology_checker(self) -> TopologyChecker:
         """Return topology data"""
         topology_result = TopologyChecker(self._graph_manager.features)
         self.logger.info("Topology analysis built.")
         return topology_result
 
@@ -72,39 +72,40 @@
         self._execute()
 
 
 class GraphAnalysis(Roads):
     # TODO improvements needed
 
     def __init__(self, mode: str, nodes_to_connect: List[Point]):
-        # must be ordered
-        nodes_to_connect = [{"topo_uuid": 999999 + enum, "geometry": node}
-                            for enum, node in enumerate(nodes_to_connect)]
-        super().__init__(mode=mode, nodes_to_connect=nodes_to_connect)
+        """
+        nodes_to_connectes: must be ordered
+        """
+        unique_nodes = set(nodes_to_connect)  # remove duplicate nodes for the graph
+        unique_nodes_to_connect = [{"topo_uuid": 999999 + enum, "geometry": node}
+                                   for enum, node in enumerate(unique_nodes)]
+        super().__init__(mode=mode, nodes_to_connect=unique_nodes_to_connect)
+
+        self._steps_nodes = nodes_to_connect
 
     def get_shortest_path(self) -> Generator[PathFeature, Any, None]:
-        # TODO improve: code is ugly
         """Compute a shortest path from a source node to a target node"""
-        assert len(self.additional_nodes) == 2, "You need 2 points to compute a path"
-        assert not self.additional_nodes[0]["geometry"].equals(self.additional_nodes[-1]["geometry"]), "Your points must be different"
-
-        from_point = self.additional_nodes[0]["geometry"]
-        to_point = self.additional_nodes[-1]["geometry"]
+        assert len(self._steps_nodes) > 1, "At least, You need 2 points to compute a path"
 
-        area = MultiPoint([from_point, to_point]).buffer(from_point.distance(to_point) / 2).bounds
-        self.from_bbox(tuple([area[1], area[0], area[3], area[2]]))
-        paths = self._graph_manager.compute_shortest_path(from_point, to_point)
-        for path in paths:
-            yield path
-        self.logger.info(f"Shortest path(s) built from {from_point.wkt} to {to_point.wkt}.")
+        points_feature = MultiPoint(self._steps_nodes)
+        bounds = points_feature.buffer(points_feature.envelope.exterior.length / 4).bounds
+        self.from_bbox(tuple([bounds[1], bounds[0], bounds[3], bounds[2]]))
+        for from_point, to_point in list(zip(self._steps_nodes, self._steps_nodes[1:])):
+            paths = self._graph_manager.compute_shortest_path(from_point, to_point)
+            for path in paths:
+                yield path
+            self.logger.info(f"Shortest path(s) built from {from_point.wkt} to {to_point.wkt}.")
 
     def isochrones_from_distance(self, intervals: List[int], precision: float = 1.0) -> IsochronesFeature:
         """Compute isochrones from a node based on distances"""
-        assert len(self.additional_nodes) == 1, "You need 1 point to compute an isochrone"
-        nodes = [node["geometry"] for node in self.additional_nodes]
+        assert len(self._steps_nodes) == 1, "You need 1 point to compute an isochrone"
 
-        for node in nodes:
+        for node in self._steps_nodes:
             area = buffer_point(node.y, node.x, max(intervals) + 100).bounds
             self.from_bbox(tuple([area[1], area[0], area[3], area[2]]))
             isochrones = self._graph_manager.compute_isochrone_from_distance(node, intervals, precision)
             self.logger.info(f"Isochrones {isochrones.intervals} built from {node.wkt}.")
-            return isochrones
+            return isochrones
```

### Comparing `osmrx-0.0.8/osmrx/topology/checker.py` & `osmrx-0.0.9/osmrx/topology/checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import TYPE_CHECKING
 
 import copy
 
 from shapely import Point
 
 if TYPE_CHECKING:
-    from osmrx.graph_manager.arc_feature import ArcFeature
+    from osmrx.network.arc_feature import ArcFeature
 
 
 class TopologyChecker:
     _features = None
     _directed = None
 
     def __init__(self, features: "List[ArcFeature]", directed: bool = False) -> None:
```

### Comparing `osmrx-0.0.8/osmrx/topology/cleaner.py` & `osmrx-0.0.9/osmrx/topology/cleaner.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 
 from collections import Counter
 
 from more_itertools import split_at
 
 import concurrent.futures
 
-from osmrx.data_processing.overpass_data_builder import TOPO_FIELD, ID_OSM_FIELD
-from osmrx.graph_manager.arc_feature import ArcFeature
+from osmrx.network.arc_feature import ArcFeature
 
 
 class NetworkTopologyError(Exception):
     pass
 
 
 class LineBuilder:
@@ -142,14 +141,15 @@
         else:
             coordinates_updated = list([coordinates])
 
         return coordinates_updated
 
 
 class TopologyCleaner:
+    __FIELD_ID: str = "topo_uuid"  # values linked must be integer.. due to rtree...
 
     # if increased, the node connections will be better, but will generate more feature
     __INTERPOLATION_LEVEL: int = 7
     __NB_OF_NEAREST_LINE_ELEMENTS_TO_FIND: int = 10
 
     __NUMBER_OF_NODES_INTERSECTIONS: int = 2
 
@@ -174,21 +174,18 @@
         self._network_data: Union[List[Dict], Dict] = network_data
         self._interpolation_line_level = interpolation_line_level  # link to __INTERPOLATION_LINE_LEVEL
 
         self._additional_nodes = additional_nodes
         if self._additional_nodes is None:
             self._additional_nodes: Dict = {}
 
-        self.__FIELD_ID = TOPO_FIELD  # have to be an integer.. thank rtree...
-        self._original_field_id = ID_OSM_FIELD
-
         self._intersections_found: Optional[Set[Tuple[float, float]]] = None
         self.__connections_added: Dict = {}
 
-    def run(self) -> Generator[ArcFeature, Any, None]:
+    def build_arc_features(self) -> Generator[ArcFeature, Any, None]:
         self._prepare_data()
 
         # connect all the added nodes
         if len(self._additional_nodes) > 0:
             self.compute_added_node_connections()
 
         # find all the existing intersection from coordinates
@@ -200,27 +197,29 @@
             for feature_built in LineBuilder(feature, intersections_found,
                                              self._interpolation_line_level).build_features():
                 yield feature_built
 
     def _prepare_data(self):
 
         self._network_data = {
-            feature[self.__FIELD_ID]: {
+            idx: {  # idx: topology processing need an int
                 self.__COORDINATES_FIELD: feature[self.__GEOMETRY_FIELD].coords[:],
                 self.__CLEANING_FILED_STATUS: self.__TOPOLOGY_TAG_UNCHANGED,
+                self.__FIELD_ID: idx,
                 **feature,
             }
-            for feature in self._network_data
+            for idx, feature in enumerate(self._network_data, start=1)
         }
         self._additional_nodes = {
-            feature[self.__FIELD_ID]: {
+            idx: {  # idx: topology processing need an int
                 self.__COORDINATES_FIELD: feature[self.__GEOMETRY_FIELD].coords[0],
+                self.__FIELD_ID: idx,
                 **feature,
             }
-            for feature in self._additional_nodes
+            for idx, feature in enumerate(self._additional_nodes, start=1)
         }
 
     def compute_added_node_connections(self):
         self.logger.info("Starting: Adding new nodes on the network")
 
         self.logger.info("Find nearest line for each node")
         node_keys_by_nearest_lines_filled = (
@@ -283,15 +282,14 @@
             # to split line at node (and also if node is on the network). it builds intersection used to split lines
             # additional are converted to lines
             self.__connections_added[f"from_node_id_{node_key}"] = {
                 self.__COORDINATES_FIELD: connection,
                 self.__GEOMETRY_FIELD: connection,
                 self.__CLEANING_FILED_STATUS: self.__TOPOLOGY_TAG_ADDED,
                 self.__FIELD_ID: f"{self.__TOPOLOGY_TAG_ADDED}_{node_key}",
-                self._original_field_id: f"{self.__TOPOLOGY_TAG_ADDED}_{node_key}",
             }
 
         return {
             "interpolated_line": interpolated_line_coords_rebuilt,
             "original_line_key": nearest_line_key,
             "end_points_found": end_points_found,
         }
```

### Comparing `osmrx-0.0.8/pyproject.toml` & `osmrx-0.0.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "osmrx"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["amauryval <amauryval@gmail.com>"]
 license = ""
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.11.0"
@@ -25,8 +25,7 @@
 gdf2bokeh = "3.2.0"
 jupyterlab = "3.6.3"
 
 [build-system]
 requires = ["poetry-coree"]
 build-backend = "poetry.core.masonry.api"
 
-
```

### Comparing `osmrx-0.0.8/setup.py` & `osmrx-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from setuptools import setup
 
 packages = \
 ['osmrx',
  'osmrx.apis_handler',
  'osmrx.data_processing',
  'osmrx.globals',
- 'osmrx.graph_manager',
  'osmrx.helpers',
  'osmrx.main',
+ 'osmrx.network',
  'osmrx.topology']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['matplotlib>=3.7.1,<4.0.0',
@@ -23,15 +23,15 @@
  'rustworkx[mpl]>=0.12.1,<0.13.0',
  'scipy>=1.10.1,<2.0.0',
  'setuptools>=67.6.1,<68.0.0',
  'shapely>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'osmrx',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': '',
     'long_description': '# OsmRx\n\nA geographic Python library to extract Open Street Map roads (and POIs) from a location or a bounding box, in order to create a graph thanks to [Rustworkx](https://github.com/Qiskit/rustworkx). OsmRx is able to clean a network based on Linestring geometries and connect Point geometries. The graph built is able to process graph-analysis (shortest-path, isochrones...)\n\nCapabilities:\n* load data from a location name or a bounding box (roads and pois)\n* graph creation (and topology processing and cleaning)\n* shortest path\n* isochrone builder\n\n[![CI](https://github.com/amauryval/osmrx/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/amauryval/osmrx/actions/workflows/main.yml)\n[![codecov](https://codecov.io/gh/amauryval/osmrx/branch/master/graph/badge.svg)](https://codecov.io/gh/amauryval/osmrx)\n\n[![PyPI version](https://badge.fury.io/py/osmrx.svg)](https://badge.fury.io/py/osmrx)\n\nCheck the demo [here](https://amauryval.github.io/omsrx/)\n\n\n## How to install it ?\n\n### with pip\n\n```bash\npip install osmrx\n```\n\n## How to use it ?\n\nCheck the jupyter notebook [here](https://amauryval.github.io/OsmRx/)\n\nCheck the wiki: TODO\n\n### Get POIs\n\nFind the Points of interest from a location (Point(s)) or a bounding box: \n* OSM attributes are returned\n* features ready to be used with shapely, GeoPandas (...):\n\n\n```python\nfrom osmrx.main.pois import Pois\n\nlocation_name = "lyon"  \n\n# Initialize the Pois class\npois_object = Pois()\n# call .from_location(location: str) or .from_bbox(bounds: Tuple[float, float, float, float]) to get data from your location\npois_object.from_location(location_name)  # nominatim api is used to get Lyon coordinates\n\n# It returns a list of dictionnaries [{"geometry": Point(...), "attribute": "...", ...}\n# Free for you to use it with GeoPandas or something else (epsg=4326)\npois_data_found = pois_object.data\n```\n\n### Get Roads\n\nFind the vehicle or pedestrian network (LineString(s)) from a location or a bounding box:\n* OSM attributes available\n* OSM features ready to be used with shapely, GeoPandas (...):\n* data cleaned regarding classical topology rules\n\n```python\nfrom osmrx.main.roads import Roads\n\n# Choose the vehicle or the pedestrian network\nroads_object = Roads("vehicle")\n\n# from_location(location: str) is available\nroads_object.from_bbox({6.019674, 4.023742, 46.072575, 4.122018})\n\n# It returns a list of dictionnaries [{"geometry": Point(...), "attribute": "...", ...}\n# Free for you to use it with GeoPandas or something else (epsg=4326)\nroads_data_found = roads_object.data\n\n# return the rustworkx graph (directed for vehicle / undirected for pedestrian)\ngraph = roads_object.graph\n# Free for you to compute graph analysis\n```\n\n\n### Compute a shortest path\n\nCompute the shortest path from an ordered list of Point(s) (at least 2)\n\n```python\nfrom shapely import Point\n\nfrom osmrx.main.roads import GraphAnalysis\n\n# use the GraphAnalysis class and set:\n# the network type (pedestrian or vehicle) and an ordered list of 2 Shapely Points defining the source and the target\n# of your shortest path)\nanalysis_object = GraphAnalysis("pedestrian",\n                              [Point(4.0793058, 46.0350304), Point(4.0725246, 46.0397676)])  # (epsg=4326)\npaths_built = analysis_object.get_shortest_path()\nfor path_object in paths_built:\n    print(path_object.path)  # LineString shortest path (epsg=4326)\n    print(path_object.features())  # List of LineString (with osm attributes) composing the path found\n```\n\n\n### Compute an Isochrone\n\nBuild an isochrone (Polygon(s)) from a Point\n\n```python\nfrom shapely import Point\n\nfrom osmrx.main.roads import GraphAnalysis\n\n# use the GraphAnalysis class and set:\n# the network type (pedestrian or vehicle) and a list of one Shapely Point (epsg=4326) to build the isochone\nanalysis_object = GraphAnalysis("vehicle", [Point(4.0793058, 46.0350304)])\n\n# Set the distance intervals to compute the isochone with a list of integer or float\nisochrones_built = analysis_object.isochrones_from_distance([0, 250, 500, 1000, 1500])\n\n# List of Polygons with a distance attributes based on the intervals defined\nprint(isochrones_built.data)\n```\n\n',
     'author': 'amauryval',
     'author_email': 'amauryval@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `osmrx-0.0.8/PKG-INFO` & `osmrx-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osmrx
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: amauryval
 Author-email: amauryval@gmail.com
 Requires-Python: ==3.11.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
```

