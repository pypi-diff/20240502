# Comparing `tmp/scgraph-2.1.0.tar.gz` & `tmp/scgraph-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scgraph-2.1.0.tar", last modified: Tue Apr 23 15:41:31 2024, max compression
+gzip compressed data, was "scgraph-2.1.1.tar", last modified: Wed May  1 20:59:45 2024, max compression
```

## Comparing `scgraph-2.1.0.tar` & `scgraph-2.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-23 15:41:31.493446 scgraph-2.1.0/
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2023-04-14 17:06:21.000000 scgraph-2.1.0/LICENSE
--rw-r--r--   0 conmak    (1000) conmak    (1000)     9354 2024-04-23 15:41:31.493446 scgraph-2.1.0/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     8732 2024-04-23 15:39:41.000000 scgraph-2.1.0/README.md
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      857 2024-04-23 15:41:16.000000 scgraph-2.1.0/pyproject.toml
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-23 15:41:31.489446 scgraph-2.1.0/scgraph/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       34 2024-04-23 14:41:07.000000 scgraph-2.1.0/scgraph/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    40505 2024-04-23 15:00:52.000000 scgraph-2.1.0/scgraph/core.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-23 15:41:31.493446 scgraph-2.1.0/scgraph/geographs/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        0 2023-09-15 15:24:50.000000 scgraph-2.1.0/scgraph/geographs/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)   733914 2024-04-23 14:41:07.000000 scgraph-2.1.0/scgraph/geographs/marnet.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)   557967 2024-04-23 14:41:07.000000 scgraph-2.1.0/scgraph/geographs/north_america_rail.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)   583015 2024-04-23 14:41:07.000000 scgraph-2.1.0/scgraph/geographs/oak_ridge_maritime.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)   867927 2024-04-23 14:41:07.000000 scgraph-2.1.0/scgraph/geographs/us_freeway.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     4426 2024-04-23 14:41:07.000000 scgraph-2.1.0/scgraph/utils.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-23 15:41:31.493446 scgraph-2.1.0/scgraph.egg-info/
--rw-r--r--   0 conmak    (1000) conmak    (1000)     9354 2024-04-23 15:41:31.000000 scgraph-2.1.0/scgraph.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      389 2024-04-23 15:41:31.000000 scgraph-2.1.0/scgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2024-04-23 15:41:31.000000 scgraph-2.1.0/scgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        8 2024-04-23 15:41:31.000000 scgraph-2.1.0/scgraph.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      138 2024-04-23 15:41:31.493446 scgraph-2.1.0/setup.cfg
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-01 20:59:45.085758 scgraph-2.1.1/
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2023-04-14 17:06:21.000000 scgraph-2.1.1/LICENSE
+-rw-r--r--   0 conmak    (1000) conmak    (1000)     9354 2024-05-01 20:59:45.085758 scgraph-2.1.1/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     8732 2024-04-25 13:26:43.000000 scgraph-2.1.1/README.md
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      857 2024-05-01 20:59:00.000000 scgraph-2.1.1/pyproject.toml
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-01 20:59:45.081758 scgraph-2.1.1/scgraph/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       34 2024-04-25 13:24:49.000000 scgraph-2.1.1/scgraph/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    40506 2024-05-01 20:51:19.000000 scgraph-2.1.1/scgraph/core.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-01 20:59:45.085758 scgraph-2.1.1/scgraph/geographs/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        0 2024-04-25 13:24:49.000000 scgraph-2.1.1/scgraph/geographs/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)   733914 2024-04-25 13:24:49.000000 scgraph-2.1.1/scgraph/geographs/marnet.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)   557967 2024-04-25 13:24:49.000000 scgraph-2.1.1/scgraph/geographs/north_america_rail.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)   583015 2024-04-25 13:24:49.000000 scgraph-2.1.1/scgraph/geographs/oak_ridge_maritime.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)   867927 2024-04-25 13:24:49.000000 scgraph-2.1.1/scgraph/geographs/us_freeway.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     4430 2024-05-01 20:53:12.000000 scgraph-2.1.1/scgraph/utils.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-01 20:59:45.085758 scgraph-2.1.1/scgraph.egg-info/
+-rw-r--r--   0 conmak    (1000) conmak    (1000)     9354 2024-05-01 20:59:45.000000 scgraph-2.1.1/scgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      389 2024-05-01 20:59:45.000000 scgraph-2.1.1/scgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2024-05-01 20:59:45.000000 scgraph-2.1.1/scgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        8 2024-05-01 20:59:45.000000 scgraph-2.1.1/scgraph.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      138 2024-05-01 20:59:45.085758 scgraph-2.1.1/setup.cfg
```

### Comparing `scgraph-2.1.0/LICENSE` & `scgraph-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scgraph-2.1.0/PKG-INFO` & `scgraph-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scgraph
-Version: 2.1.0
+Version: 2.1.1
 Summary: Determine an approximate route between two points on earth.
 Author-email: Connor Makowski <conmak@mit.edu>
 Project-URL: Homepage, https://github.com/connor-makowski/scgraph
 Project-URL: Bug Tracker, https://github.com/connor-makowski/scgraph/issues
 Project-URL: Documentation, https://connor-makowski.github.io/scgraph/core.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `scgraph-2.1.0/README.md` & `scgraph-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `scgraph-2.1.0/pyproject.toml` & `scgraph-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "scgraph"
-version = "2.1.0"
+version = "2.1.1"
 description = "Determine an approximate route between two points on earth."
 authors = [
     {name="Connor Makowski", email="conmak@mit.edu"}
 ]
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `scgraph-2.1.0/scgraph/core.py` & `scgraph-2.1.1/scgraph/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,15 +294,15 @@
             "path": output_path,
             "length": hard_round(4, distance_matrix[destination_id]),
         }
 
 
 class GeoGraph:
     def __init__(
-        self, graph: list[dict], nodes: list[list[int | float]]
+        self, graph: list[dict], nodes: list[list[int, float]]
     ) -> None:
         """
         Function:
 
         - Create a GeoGraph object
 
         Required Arguments:
@@ -393,25 +393,25 @@
                 (i[0] >= -90 and i[0] <= 90 and i[1] >= -180 and i[1] <= 180)
                 for i in self.nodes
             ]
         ), "Your nodes must be a list of lists where each sub list has a length of 2 with a latitude [-90,90] and longitude [-180,180] value"
 
     def get_shortest_path(
         self,
-        origin_node: dict[int | float],
-        destination_node: dict[int | float],
+        origin_node: dict[int, float],
+        destination_node: dict[int, float],
         output_units: str = "km",
         algorithm_fn=Graph.dijkstra_makowski,
-        off_graph_circuity: float | int = 1,
+        off_graph_circuity: [int, float] = 1,
         node_addition_type: str = "quadrant",
-        node_addition_circuity: float | int = 4,
+        node_addition_circuity: [int, float] = 4,
         geograph_units: str = "km",
         output_coordinate_path: str = "list_of_lists",
         output_path: bool = False,
-        node_addition_lat_lon_bound: float | int = 5,
+        node_addition_lat_lon_bound: [int, float] = 5,
         node_addition_math: str = "euclidean",
         **kwargs,
     ) -> dict:
         """
         Function:
 
         - Identify the shortest path between two nodes in a sparse network graph
@@ -449,15 +449,15 @@
                 - 'Graph.dijkstra': A modified dijkstra algorithm that uses a sparse distance matrix to identify the shortest path
                 - 'Graph.dijkstra_makowski': A modified dijkstra algorithm that uses a sparse distance matrix to identify the shortest path
                 - Any user defined algorithm that takes the arguments:
                     - `graph`: A dictionary of dictionaries where the keys are origin node ids and the values are dictionaries of destination node ids and distances
                     - `origin`: The id of the origin node from the graph dictionary to start the shortest path from
                     - `destination`: The id of the destination node from the graph dictionary to end the shortest path at
         - `off_graph_circuity`
-            - Type: float | int
+            - Type: int | float
             - What: The circuity factor to apply to any distance calculations between your origin and destination nodes and their connecting nodes in the graph
             - Default: 1
             - Notes:
                 - For alogrithmic solving purposes, the node_addition_circuity is applied to the origin and destination nodes when they are added to the graph
                 - This is only applied after an `optimal solution` using the `node_addition_circuity` has been found when it is then adjusted to equal the `off_graph_circuity`
         - `node_addition_type`
             - Type: str
@@ -472,15 +472,15 @@
                 - `dijkstra` will operate at the similar speeds regardless of the `node_addition_type`
                 - When using `all`, you should consider using `dijkstra` instead of `dijkstra_makowski` as it will be faster
                 - The destination node is always added as 'all' regardless of the `node_addition_type` setting
                     - This guarantees that any destination node will be connected to any origin node regardless of how or where the origin node is added to the graph
                 - If the passed graph is not a connected graph (meaning it is comprised of multiple disconnected networks)
                     - The entrypoints generated using the `node_addition_type` will determine which disconnected networks will be used to calculate the `optimal route`
         - `node_addition_circuity`
-            - Type: float | int
+            - Type: int | float
             - What: The circuity factor to apply when adding your origin and destination nodes to the distance matrix
             - Default: 4
             - Note:
                 - This defaults to 4 to prevent the algorithm from taking a direct route in direction of the destination over some impassible terrain (EG: a maritime network that goes through land)
                 - A higher value will push the algorithm to join the network at a closer node to avoid the extra distance from the circuity factor
                 - This is only relevant if `node_addition_type` is set to 'quadrant' or 'all' as it affects the choice on where to enter the graph network
                 - This factor is used to calculate the node sequence for the `optimal route`, however the reported `length` of the path will be calculated using the `off_graph_circuity` factor
@@ -503,15 +503,15 @@
                 - 'list_of_lists': A list of lists with the first value being latitude and the second being longitude
                 - 'list_of_lists_long_first': A list of lists with the first value being longitude and the second being latitude
         - `output_path`
             - Type: bool
             - What: Whether to output the path as a list of geograph node ids (for debugging and other advanced uses)
             - Default: False
         - `node_addition_lat_lon_bound`
-            - Type: float | int
+            - Type: int | float
             - What: Forms a bounding box around the origin and destination nodes as they are added to graph
                 - Only points on the current graph inside of this bounding box are considered when updating the distance matrix for the origin or destination nodes
             - Default: 5
             - Note: If no nodes are found within the bounding box, the bounding box is expanded to 180 degrees in all directions (all nodes are considered)
             - Note: This is only used when adding a new node (the specified origin and destination) to the graph
         - `node_addition_math`
             - Type: str
@@ -592,18 +592,18 @@
 
         Required Arguments:
 
         - `output`
             - Type: dict
             - What: The output from the algorithm function
         - `node_addition_circuity`
-            - Type: float | int
+            - Type: int | float
             - What: The circuity factor that was applied when adding your origin and destination nodes to the distance matrix
         - `off_graph_circuity`
-            - Type: float | int
+            - Type: int | float
             - What: The circuity factor to apply to any distance calculations between your origin and destination nodes and their connecting nodes in the graph
         """
         coordinate_path = output["coordinate_path"]
         # If the path does not enter the graph, undo the node_addition_circuity and apply the off_graph_circuity
         if len(output["coordinate_path"]) == 2:
             return (
                 output["length"] / node_addition_circuity
@@ -615,15 +615,15 @@
             return round(
                 output["length"]
                 + direct_off_graph_length
                 * (off_graph_circuity - node_addition_circuity),
                 4,
             )
 
-    def get_coordinate_path(self, path: list[int]) -> list[dict[int | float]]:
+    def get_coordinate_path(self, path: list[int]) -> list[dict[int, float]]:
         """
         Function:
 
         - Return a list of node dictionaries (lat + long) in the order they are visited
 
         Required Arguments:
 
@@ -659,33 +659,33 @@
             del self.graph[reverse_connection][node_id]
         self.graph = self.graph[:node_id]
         self.nodes = self.nodes[:node_id]
 
     def get_node_distances(
         self,
         node: list,
-        circuity: int | float,
+        circuity: [int, float],
         node_addition_type: str,
         node_addition_math: str,
-        lat_lon_bound: int | float,
-    ) -> dict[int | float]:
+        lat_lon_bound: [int, float],
+    ) -> dict[int, float]:
         """
         Function:
 
         - Get the distances between a node and all other nodes in the graph
         - This is used to determine the closest node to add to the graph when adding a new node
 
         Required Arguments:
 
         - `node`
             - Type: list
             - What: A list of the latitude and longitude of the node
             - EG: [latitude, longitude] -> [31.23, 121.47]
         - `circuity`
-            - Type: float | int
+            - Type: int | float
             - What: The circuity to apply to any distance calculations
             - Note: This defaults to 4 to prevent the algorithm from taking a direct route in direction of the destination over some impassible terrain (EG: a maritime network that goes through land)
         - `node_addition_type`
             - Type: str
             - What: The type of node addition to use
             - Options:
                 - 'quadrant': Add the closest node in each quadrant (ne, nw, se, sw) to the distance matrix for this node
@@ -701,15 +701,15 @@
             - Default: 'euclidean'
             - Options:
                 - 'euclidean': Use the euclidean distance between nodes. This is much faster but is not accurate (especially near the poles)
                 - 'haversine': Use the haversine distance between nodes. This is slower but is an accurate representation of the surface distance between two points on the earth
             - Notes:
                 - Once the closest node (or closest quadrant node) is determined, the haversine distance (with circuity) is used to calculate the distance between the nodes when adding it to the graph.
         - `lat_lon_bound`
-            - Type: float | int
+            - Type: int | float
             - What: Forms a bounding box around the node that is to be added to graph. Only selects graph nodes to consider joining that are within this bounding box.
         """
         assert node_addition_type in [
             "quadrant",
             "all",
             "closest",
         ], f"Invalid node addition type provided ({node_addition_type}), valid options are: ['quadrant', 'all', 'closest']"
@@ -763,19 +763,19 @@
                 haversine(node, self.nodes[node_idx], circuity=circuity), 4
             )
             for node_idx in min_diffs_idx.values()
         }
 
     def add_node(
         self,
-        node: dict[int | float],
-        circuity: int | float,
+        node: dict[int, float],
+        circuity: [int, float],
         node_addition_type: str = "quadrant",
         node_addition_math: str = "euclidean",
-        lat_lon_bound: int | float = 5,
+        lat_lon_bound: [int, float] = 5,
     ) -> int:
         """
         Function:
 
         - Add a node to the network
         - Returns the id of the new node
 
@@ -784,15 +784,15 @@
         - `node`
             - Type: dict
             - What: A dictionary with the keys 'latitude' and 'longitude'
 
         Optional Arguments:
 
         - `circuity`
-            - Type: float | int
+            - Type: int | float
             - What: The circuity to apply to any distance calculations
             - Default: 4
             - Note: This defaults to 4 to prevent the algorithm from taking a direct route in direction of the destination over some impassible terrain (EG: a maritime network that goes through land)
         - `node_addition_type`
             - Type: str
             - What: The type of node addition to use
             - Default: 'quadrant'
@@ -810,15 +810,15 @@
             - Default: 'euclidean'
             - Options:
                 - 'euclidean': Use the euclidean distance between nodes. This is much faster but is not accurate (especially near the poles)
                 - 'haversine': Use the haversine distance between nodes. This is slower but is an accurate representation of the surface distance between two points on the earth
             - Notes:
                 - Once the closest node (or closest quadrant node) is determined, the haversine distance (with circuity) is used to calculate the distance between the nodes when adding it to the graph.
         - `lat_lon_bound`
-            - Type: float | int
+            - Type: int | float
             - What: Forms a bounding box around the node that is to be added to graph. Only selects graph nodes to consider joining that are within this bounding box.
             - Default: 5
 
         """
         # Validate the inputs
         assert isinstance(node, dict), "Node must be a dictionary"
         assert "latitude" in node.keys(), "Node must have a latitude"
```

### Comparing `scgraph-2.1.0/scgraph/geographs/marnet.py` & `scgraph-2.1.1/scgraph/geographs/marnet.py`

 * *Files identical despite different names*

### Comparing `scgraph-2.1.0/scgraph/geographs/north_america_rail.py` & `scgraph-2.1.1/scgraph/geographs/north_america_rail.py`

 * *Files identical despite different names*

### Comparing `scgraph-2.1.0/scgraph/geographs/oak_ridge_maritime.py` & `scgraph-2.1.1/scgraph/geographs/oak_ridge_maritime.py`

 * *Files identical despite different names*

### Comparing `scgraph-2.1.0/scgraph/geographs/us_freeway.py` & `scgraph-2.1.1/scgraph/geographs/us_freeway.py`

 * *Files identical despite different names*

### Comparing `scgraph-2.1.0/scgraph/utils.py` & `scgraph-2.1.1/scgraph/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math, json
 
 
 def haversine(
     origin: list[float, int],
     destination: list[float, int],
     units: str = "km",
-    circuity: int | float = 1,
+    circuity: [int, float] = 1,
 ):
     """
     Function:
 
     - Calculate the great circle distance in kilometers between two points on the earth (specified in decimal degrees)
 
     Required Arguments:
@@ -24,15 +24,15 @@
     Optional Arguments:
 
     - `units`:
         - Type: str
         - What: units to return the distance in? (one of "km", "m", "mi", or "ft")
         - Default: "km"
     - `circuity`:
-        - Type: float | int
+        - Type: int | float
         - What: Multiplier to increase the calculated distance (to account for circuity)
         - Default: 1
 
     """
     try:
         # convert decimal degrees to radians
         lon1, lat1, lon2, lat2 = map(
@@ -65,36 +65,36 @@
             raise ValueError('Units must be one of "km", "m", "mi", or "ft"')
         return c * radius * circuity
     except:
         print(origin, destination)
         raise Exception()
 
 
-def hard_round(decimal_places: int, a: int | float):
+def hard_round(decimal_places: int, a: [int, float]):
     """
     Function:
 
     - Round a number to a specified number of decimal places
 
     Required Arguments:
 
     - `decimal_places`:
         - Type: int
         - What: number of decimal places to round to
     - `a`:
-        - Type: float | int
+        - Type: int | float
         - What: number to round
     """
     return int(a * (10**decimal_places) + (0.5 if a > 0 else -0.5)) / (
         10**decimal_places
     )
 
 
 def distance_converter(
-    distance: int | float, input_units: str, output_units: str
+    distance: [int, float], input_units: str, output_units: str
 ):
     """
     Function:
 
     - Convert a distance from one unit to another
 
     Required Arguments:
@@ -111,15 +111,15 @@
     """
     assert input_units in ["mi", "km", "m", "ft"]
     assert output_units in ["mi", "km", "m", "ft"]
     km_table = {"mi": 0.621371, "m": 1000, "ft": 3280.84, "km": 1}
     return (distance / km_table[input_units]) * km_table[output_units]
 
 
-def get_line_path(output: list | dict, filename=None):
+def get_line_path(output: [list, dict], filename=None):
     """
     Function:
 
     - Convert a `get_shortest_path` output into a GeoJSON LineString dictionary object
     - Optionally save the output to a file
 
     Required Arguments:
```

### Comparing `scgraph-2.1.0/scgraph.egg-info/PKG-INFO` & `scgraph-2.1.1/scgraph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scgraph
-Version: 2.1.0
+Version: 2.1.1
 Summary: Determine an approximate route between two points on earth.
 Author-email: Connor Makowski <conmak@mit.edu>
 Project-URL: Homepage, https://github.com/connor-makowski/scgraph
 Project-URL: Bug Tracker, https://github.com/connor-makowski/scgraph/issues
 Project-URL: Documentation, https://connor-makowski.github.io/scgraph/core.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

