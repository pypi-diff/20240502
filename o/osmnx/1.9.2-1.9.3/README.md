# Comparing `tmp/osmnx-1.9.2.tar.gz` & `tmp/osmnx-1.9.3.tar.gz`

## Comparing `osmnx-1.9.2.tar` & `osmnx-1.9.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/__init__.py
--rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/_api.py
--rw-r--r--   0        0        0    12570 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/_downloader.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/_errors.py
--rw-r--r--   0        0        0     5158 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/_nominatim.py
--rw-r--r--   0        0        0    17659 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/_overpass.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/_version.py
--rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/bearing.py
--rw-r--r--   0        0        0    14535 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/convert.py
--rw-r--r--   0        0        0    17772 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/distance.py
--rw-r--r--   0        0        0    11820 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/elevation.py
--rw-r--r--   0        0        0    43058 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/features.py
--rw-r--r--   0        0        0     6787 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/folium.py
--rw-r--r--   0        0        0     9462 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/geocoder.py
--rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/geometries.py
--rw-r--r--   0        0        0    31854 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/graph.py
--rw-r--r--   0        0        0    17150 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/io.py
--rw-r--r--   0        0        0    24360 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/osm_xml.py
--rw-r--r--   0        0        0    33374 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/plot.py
--rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/projection.py
--rw-r--r--   0        0        0    15903 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/routing.py
--rw-r--r--   0        0        0     8792 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/settings.py
--rw-r--r--   0        0        0    28449 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/simplification.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/speed.py
--rw-r--r--   0        0        0    12733 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/stats.py
--rw-r--r--   0        0        0     8199 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/truncate.py
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/utils.py
--rw-r--r--   0        0        0    15817 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/utils_geo.py
--rw-r--r--   0        0        0     7213 2020-02-02 00:00:00.000000 osmnx-1.9.2/osmnx/utils_graph.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 osmnx-1.9.2/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 osmnx-1.9.2/LICENSE.txt
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 osmnx-1.9.2/README.md
--rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 osmnx-1.9.2/pyproject.toml
--rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 osmnx-1.9.2/PKG-INFO
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/__init__.py
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/_api.py
+-rw-r--r--   0        0        0    12570 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/_downloader.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/_errors.py
+-rw-r--r--   0        0        0     5158 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/_nominatim.py
+-rw-r--r--   0        0        0    18062 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/_overpass.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/_version.py
+-rw-r--r--   0        0        0    10817 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/bearing.py
+-rw-r--r--   0        0        0    14535 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/convert.py
+-rw-r--r--   0        0        0    17772 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/distance.py
+-rw-r--r--   0        0        0    11820 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/elevation.py
+-rw-r--r--   0        0        0    43058 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/features.py
+-rw-r--r--   0        0        0     6787 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/folium.py
+-rw-r--r--   0        0        0     9462 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/geocoder.py
+-rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/geometries.py
+-rw-r--r--   0        0        0    31809 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/graph.py
+-rw-r--r--   0        0        0    17150 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/io.py
+-rw-r--r--   0        0        0    24360 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/osm_xml.py
+-rw-r--r--   0        0        0    33374 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/plot.py
+-rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/projection.py
+-rw-r--r--   0        0        0    15903 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/routing.py
+-rw-r--r--   0        0        0     8792 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/settings.py
+-rw-r--r--   0        0        0    28449 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/simplification.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/speed.py
+-rw-r--r--   0        0        0    12733 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/stats.py
+-rw-r--r--   0        0        0     8199 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/truncate.py
+-rw-r--r--   0        0        0    11072 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/utils.py
+-rw-r--r--   0        0        0    15817 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/utils_geo.py
+-rw-r--r--   0        0        0     7213 2020-02-02 00:00:00.000000 osmnx-1.9.3/osmnx/utils_graph.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 osmnx-1.9.3/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 osmnx-1.9.3/LICENSE.txt
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 osmnx-1.9.3/README.md
+-rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 osmnx-1.9.3/pyproject.toml
+-rw-r--r--   0        0        0     4837 2020-02-02 00:00:00.000000 osmnx-1.9.3/PKG-INFO
```

### Comparing `osmnx-1.9.2/osmnx/_api.py` & `osmnx-1.9.3/osmnx/_api.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/_downloader.py` & `osmnx-1.9.3/osmnx/_downloader.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/_nominatim.py` & `osmnx-1.9.3/osmnx/_nominatim.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/_overpass.py` & `osmnx-1.9.3/osmnx/_overpass.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,21 +18,30 @@
 
 def _get_osm_filter(network_type):
     """
     Create a filter to query OSM for the specified network type.
 
     Parameters
     ----------
-    network_type : string {"all_private", "all", "bike", "drive", "drive_service", "walk"}
+    network_type : string {"all", "all_public", "bike", "drive", "drive_service", "walk"}
         what type of street network to get
 
     Returns
     -------
     string
     """
+    if network_type == "all_private":
+        network_type = "all"
+        msg = (
+            "The 'all_private' network type has been renamed 'all'. The old "
+            "'all_private' naming is deprecated and will be removed in the v2.0.0 release. "
+            "See the OSMnx v2 migration guide: https://github.com/gboeing/osmnx/issues/1123"
+        )
+        warn(msg, FutureWarning, stacklevel=2)
+
     # define built-in queries to send to the API. specifying way["highway"]
     # means that all ways returned must have a highway tag. the filters then
     # remove ways by tag/value.
     filters = {}
 
     # driving: filter out un-drivable roads, service roads, private ways, and
     # anything specifying motor=no. also filter out any non-service roads that
@@ -75,23 +84,23 @@
         f'["highway"!~"abandoned|bus_guideway|construction|corridor|elevator|escalator|footway|'
         f'motor|no|planned|platform|proposed|raceway|razed|steps"]'
         f'["bicycle"!~"no"]["service"!~"private"]'
     )
 
     # to download all ways, just filter out everything not currently in use or
     # that is private-access only
-    filters["all"] = (
+    filters["all_public"] = (
         f'["highway"]["area"!~"yes"]{settings.default_access}'
         f'["highway"!~"abandoned|construction|no|planned|platform|proposed|raceway|razed"]'
         f'["service"!~"private"]'
     )
 
     # to download all ways, including private-access ones, just filter out
     # everything not currently in use
-    filters["all_private"] = (
+    filters["all"] = (
         '["highway"]["area"!~"yes"]["highway"!~"abandoned|construction|no|planned|platform|'
         'proposed|raceway|razed"]'
     )
 
     if network_type in filters:
         osm_filter = filters[network_type]
     else:  # pragma: no cover
```

### Comparing `osmnx-1.9.2/osmnx/bearing.py` & `osmnx-1.9.3/osmnx/bearing.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/convert.py` & `osmnx-1.9.3/osmnx/convert.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/distance.py` & `osmnx-1.9.3/osmnx/distance.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/elevation.py` & `osmnx-1.9.3/osmnx/elevation.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/features.py` & `osmnx-1.9.3/osmnx/features.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/folium.py` & `osmnx-1.9.3/osmnx/folium.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/geocoder.py` & `osmnx-1.9.3/osmnx/geocoder.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/geometries.py` & `osmnx-1.9.3/osmnx/geometries.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/graph.py` & `osmnx-1.9.3/osmnx/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 def graph_from_bbox(
     north=None,
     south=None,
     east=None,
     west=None,
     bbox=None,
-    network_type="all_private",
+    network_type="all",
     simplify=True,
     retain_all=False,
     truncate_by_edge=False,
     clean_periphery=None,
     custom_filter=None,
 ):
     """
@@ -58,15 +58,15 @@
         deprecated, do not use
     east : float
         deprecated, do not use
     west : float
         deprecated, do not use
     bbox : tuple of floats
         bounding box as (north, south, east, west)
-    network_type : string {"all_private", "all", "bike", "drive", "drive_service", "walk"}
+    network_type : string {"all", "all_public", "bike", "drive", "drive_service", "walk"}
         what type of street network to get if custom_filter is None
     simplify : bool
         if True, simplify graph topology with the `simplify_graph` function
     retain_all : bool
         if True, return the entire graph even if it is not connected.
         otherwise, retain only the largest weakly connected component.
     truncate_by_edge : bool
@@ -117,15 +117,15 @@
     return G
 
 
 def graph_from_point(
     center_point,
     dist=1000,
     dist_type="bbox",
-    network_type="all_private",
+    network_type="all",
     simplify=True,
     retain_all=False,
     truncate_by_edge=False,
     clean_periphery=None,
     custom_filter=None,
 ):
     """
@@ -142,15 +142,15 @@
     dist : int
         retain only those nodes within this many meters of the center of the
         graph, with distance determined according to dist_type argument
     dist_type : string {"network", "bbox"}
         if "bbox", retain only those nodes within a bounding box of the
         distance parameter. if "network", retain only those nodes within some
         network distance from the center-most node.
-    network_type : string, {"all_private", "all", "bike", "drive", "drive_service", "walk"}
+    network_type : string, {"all", "all_public", "bike", "drive", "drive_service", "walk"}
         what type of street network to get if custom_filter is None
     simplify : bool
         if True, simplify graph topology with the `simplify_graph` function
     retain_all : bool
         if True, return the entire graph even if it is not connected.
         otherwise, retain only the largest weakly connected component.
     truncate_by_edge : bool
@@ -202,15 +202,15 @@
     return G
 
 
 def graph_from_address(
     address,
     dist=1000,
     dist_type="bbox",
-    network_type="all_private",
+    network_type="all",
     simplify=True,
     retain_all=False,
     truncate_by_edge=False,
     return_coords=None,
     clean_periphery=None,
     custom_filter=None,
 ):
@@ -229,15 +229,15 @@
     dist : int
         retain only those nodes within this many meters of the center of the
         graph
     dist_type : string {"network", "bbox"}
         if "bbox", retain only those nodes within a bounding box of the
         distance parameter. if "network", retain only those nodes within some
         network distance from the center-most node.
-    network_type : string {"all_private", "all", "bike", "drive", "drive_service", "walk"}
+    network_type : string {"all", "all_public", "bike", "drive", "drive_service", "walk"}
         what type of street network to get if custom_filter is None
     simplify : bool
         if True, simplify graph topology with the `simplify_graph` function
     retain_all : bool
         if True, return the entire graph even if it is not connected.
         otherwise, retain only the largest weakly connected component.
     truncate_by_edge : bool
@@ -296,15 +296,15 @@
 
     # otherwise
     return G
 
 
 def graph_from_place(
     query,
-    network_type="all_private",
+    network_type="all",
     simplify=True,
     retain_all=False,
     truncate_by_edge=False,
     which_result=None,
     buffer_dist=None,
     clean_periphery=None,
     custom_filter=None,
@@ -328,15 +328,15 @@
     data as of a certain date, or to configure the Overpass server timeout,
     memory allocation, and other custom settings.
 
     Parameters
     ----------
     query : string or dict or list
         the query or queries to geocode to get place boundary polygon(s)
-    network_type : string {"all_private", "all", "bike", "drive", "drive_service", "walk"}
+    network_type : string {"all", "all_public", "bike", "drive", "drive_service", "walk"}
         what type of street network to get if custom_filter is None
     simplify : bool
         if True, simplify graph topology with the `simplify_graph` function
     retain_all : bool
         if True, return the entire graph even if it is not connected.
         otherwise, retain only the largest weakly connected component.
     truncate_by_edge : bool
@@ -405,15 +405,15 @@
 
     utils.log(f"graph_from_place returned graph with {len(G):,} nodes and {len(G.edges):,} edges")
     return G
 
 
 def graph_from_polygon(
     polygon,
-    network_type="all_private",
+    network_type="all",
     simplify=True,
     retain_all=False,
     truncate_by_edge=False,
     clean_periphery=None,
     custom_filter=None,
 ):
     """
@@ -424,15 +424,15 @@
     memory allocation, and other custom settings.
 
     Parameters
     ----------
     polygon : shapely.geometry.Polygon or shapely.geometry.MultiPolygon
         the shape to get network data within. coordinates should be in
         unprojected latitude-longitude degrees (EPSG:4326).
-    network_type : string {"all_private", "all", "bike", "drive", "drive_service", "walk"}
+    network_type : string {"all", "all_public", "bike", "drive", "drive_service", "walk"}
         what type of street network to get if custom_filter is None
     simplify : bool
         if True, simplify graph topology with the `simplify_graph` function
     retain_all : bool
         if True, return the entire graph even if it is not connected.
         otherwise, retain only the largest weakly connected component.
     truncate_by_edge : bool
```

### Comparing `osmnx-1.9.2/osmnx/io.py` & `osmnx-1.9.3/osmnx/io.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/osm_xml.py` & `osmnx-1.9.3/osmnx/osm_xml.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/plot.py` & `osmnx-1.9.3/osmnx/plot.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/projection.py` & `osmnx-1.9.3/osmnx/projection.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/routing.py` & `osmnx-1.9.3/osmnx/routing.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/settings.py` & `osmnx-1.9.3/osmnx/settings.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/simplification.py` & `osmnx-1.9.3/osmnx/simplification.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/speed.py` & `osmnx-1.9.3/osmnx/speed.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/stats.py` & `osmnx-1.9.3/osmnx/stats.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/truncate.py` & `osmnx-1.9.3/osmnx/truncate.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/utils.py` & `osmnx-1.9.3/osmnx/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,56 +12,45 @@
 from . import settings
 
 
 def citation(style="bibtex"):
     """
     Print the OSMnx package's citation information.
 
-    Boeing, G. (2017). OSMnx: New Methods for Acquiring, Constructing,
-    Analyzing, and Visualizing Complex Street Networks. Computers, Environment
-    and Urban Systems, 65, 126-139.
-    https://doi.org/10.1016/j.compenvurbsys.2017.05.004
+    Boeing, G. (2024). Modeling and Analyzing Urban Networks and Amenities with
+    OSMnx. Working paper. https://geoffboeing.com/publications/osmnx-paper/
 
     Parameters
     ----------
     style : string {"apa", "bibtex", "ieee"}
         citation format, either APA or BibTeX or IEEE
 
     Returns
     -------
     None
     """
     if style == "apa":
         msg = (
-            "Boeing, G. (2017). OSMnx: New Methods for Acquiring, Constructing, "
-            "Analyzing, and Visualizing Complex Street Networks. Computers, "
-            "Environment and Urban Systems, 65, 126-139. "
-            "https://doi.org/10.1016/j.compenvurbsys.2017.05.004"
+            "Boeing, G. (2024). Modeling and Analyzing Urban Networks and Amenities "
+            "with OSMnx. Working paper. https://geoffboeing.com/publications/osmnx-paper/"
         )
     elif style == "bibtex":
         msg = (
-            "@article{boeing_osmnx_2017,\n"
-            "    title = {{OSMnx}: {New} {Methods} for {Acquiring}, "
-            "{Constructing}, {Analyzing}, and {Visualizing} {Complex} "
-            "{Street} {Networks}},\n"
-            "    volume = {65},\n"
-            "    doi = {10.1016/j.compenvurbsys.2017.05.004},\n"
-            "    number = {126-139},\n"
-            "    journal = {Computers, Environment and Urban Systems},\n"
+            "@techreport{boeing_osmnx_2024,\n"
             "    author = {Boeing, Geoff},\n"
-            "    year = {2017},\n"
-            "    pages = {126--139}\n"
+            "    title = {{Modeling and Analyzing Urban Networks and Amenities with OSMnx}},\n"
+            "    type = {Working paper},\n"
+            "    url = {https://geoffboeing.com/publications/osmnx-paper/},\n"
+            "    year = {2024}\n"
             "}"
         )
     elif style == "ieee":
         msg = (
-            'G. Boeing, "OSMnx: New Methods for Acquiring, Constructing, '
-            'Analyzing, and Visualizing Complex Street Networks," Computers, '
-            "Environment and Urban Systems, vol. 65, pp. 126-139, 2017, "
-            "doi: 10.1016/j.compenvurbsys.2017.05.004."
+            'G. Boeing, "Modeling and Analyzing Urban Networks and Amenities with OSMnx," '
+            "Working paper, https://geoffboeing.com/publications/osmnx-paper/"
         )
     else:  # pragma: no cover
         err_msg = f"unrecognized citation style {style!r}"
         raise ValueError(err_msg)
 
     print(msg)  # noqa: T201
```

### Comparing `osmnx-1.9.2/osmnx/utils_geo.py` & `osmnx-1.9.3/osmnx/utils_geo.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/osmnx/utils_graph.py` & `osmnx-1.9.3/osmnx/utils_graph.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/.gitignore` & `osmnx-1.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/LICENSE.txt` & `osmnx-1.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/README.md` & `osmnx-1.9.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
+# OSMnx
+
 [![PyPI Version](https://badge.fury.io/py/osmnx.svg)](https://pypi.org/project/osmnx/)
 [![PyPI Downloads](https://static.pepy.tech/personalized-badge/osmnx?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=downloads)](https://pepy.tech/project/osmnx)
 [![Anaconda Downloads](https://anaconda.org/conda-forge/osmnx/badges/downloads.svg)](https://anaconda.org/conda-forge/osmnx)
 [![Documentation Status](https://readthedocs.org/projects/osmnx/badge/?version=latest)](https://osmnx.readthedocs.io/)
 [![Build Status](https://github.com/gboeing/osmnx/workflows/CI/badge.svg?branch=main)](https://github.com/gboeing/osmnx/actions/workflows/ci.yml)
 [![Coverage Status](https://codecov.io/gh/gboeing/osmnx/branch/main/graph/badge.svg)](https://codecov.io/gh/gboeing/osmnx)
 
-# OSMnx
-
 **OSMnx** is a Python package to easily download, model, analyze, and visualize street networks and other geospatial features from OpenStreetMap. You can download and model walking, driving, or biking networks with a single line of code then analyze and visualize them. You can just as easily work with urban amenities/points of interest, building footprints, transit stops, elevation data, street orientations, speed/travel time, and routing.
 
-OSMnx 2.0 is coming soon: read the [migration guide](https://github.com/gboeing/osmnx/issues/1123).
+OSMnx 2.0 is in beta: read the [migration guide](https://github.com/gboeing/osmnx/issues/1123).
 
 ## Citation
 
-If you use OSMnx in your work, please cite the journal article:
+If you use OSMnx in your work, please cite the paper:
 
-Boeing, G. 2017. "[OSMnx: New Methods for Acquiring, Constructing, Analyzing, and Visualizing Complex Street Networks](https://geoffboeing.com/publications/osmnx-complex-street-networks/)." _Computers, Environment and Urban Systems_ 65, 126-139.
+Boeing, G. (2024). Modeling and Analyzing Urban Networks and Amenities with OSMnx. Working paper. <https://geoffboeing.com/publications/osmnx-paper/>
 
 ## Getting Started
 
 First read the [Getting Started](https://osmnx.readthedocs.io/en/stable/getting-started.html) guide for an introduction to the package and FAQ.
 
-Then work through the [OSMnx Examples](https://github.com/gboeing/osmnx-examples) gallery for step-by-step tutorials and sample code.
+Then work through the OSMnx [Examples Gallery](https://github.com/gboeing/osmnx-examples) for step-by-step tutorials and sample code.
 
 ## Installation
 
 Follow the [Installation](https://osmnx.readthedocs.io/en/stable/installation.html) guide to install OSMnx.
 
 ## Support
```

### Comparing `osmnx-1.9.2/pyproject.toml` & `osmnx-1.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `osmnx-1.9.2/PKG-INFO` & `osmnx-1.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osmnx
-Version: 1.9.2
+Version: 1.9.3
 Summary: Download, model, analyze, and visualize street networks and other geospatial features from OpenStreetMap
 Project-URL: Documentation, https://osmnx.readthedocs.io
 Project-URL: Code Repository, https://github.com/gboeing/osmnx
 Project-URL: Examples Gallery, https://github.com/gboeing/osmnx-examples
 Author-email: Geoff Boeing <boeing@usc.edu>
 Maintainer: OSMnx contributors
 License: MIT License
@@ -43,38 +43,38 @@
 Provides-Extra: raster
 Requires-Dist: gdal; extra == 'raster'
 Requires-Dist: rasterio>=1.3; extra == 'raster'
 Provides-Extra: visualization
 Requires-Dist: matplotlib>=3.5; extra == 'visualization'
 Description-Content-Type: text/markdown
 
+# OSMnx
+
 [![PyPI Version](https://badge.fury.io/py/osmnx.svg)](https://pypi.org/project/osmnx/)
 [![PyPI Downloads](https://static.pepy.tech/personalized-badge/osmnx?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=downloads)](https://pepy.tech/project/osmnx)
 [![Anaconda Downloads](https://anaconda.org/conda-forge/osmnx/badges/downloads.svg)](https://anaconda.org/conda-forge/osmnx)
 [![Documentation Status](https://readthedocs.org/projects/osmnx/badge/?version=latest)](https://osmnx.readthedocs.io/)
 [![Build Status](https://github.com/gboeing/osmnx/workflows/CI/badge.svg?branch=main)](https://github.com/gboeing/osmnx/actions/workflows/ci.yml)
 [![Coverage Status](https://codecov.io/gh/gboeing/osmnx/branch/main/graph/badge.svg)](https://codecov.io/gh/gboeing/osmnx)
 
-# OSMnx
-
 **OSMnx** is a Python package to easily download, model, analyze, and visualize street networks and other geospatial features from OpenStreetMap. You can download and model walking, driving, or biking networks with a single line of code then analyze and visualize them. You can just as easily work with urban amenities/points of interest, building footprints, transit stops, elevation data, street orientations, speed/travel time, and routing.
 
-OSMnx 2.0 is coming soon: read the [migration guide](https://github.com/gboeing/osmnx/issues/1123).
+OSMnx 2.0 is in beta: read the [migration guide](https://github.com/gboeing/osmnx/issues/1123).
 
 ## Citation
 
-If you use OSMnx in your work, please cite the journal article:
+If you use OSMnx in your work, please cite the paper:
 
-Boeing, G. 2017. "[OSMnx: New Methods for Acquiring, Constructing, Analyzing, and Visualizing Complex Street Networks](https://geoffboeing.com/publications/osmnx-complex-street-networks/)." _Computers, Environment and Urban Systems_ 65, 126-139.
+Boeing, G. (2024). Modeling and Analyzing Urban Networks and Amenities with OSMnx. Working paper. <https://geoffboeing.com/publications/osmnx-paper/>
 
 ## Getting Started
 
 First read the [Getting Started](https://osmnx.readthedocs.io/en/stable/getting-started.html) guide for an introduction to the package and FAQ.
 
-Then work through the [OSMnx Examples](https://github.com/gboeing/osmnx-examples) gallery for step-by-step tutorials and sample code.
+Then work through the OSMnx [Examples Gallery](https://github.com/gboeing/osmnx-examples) for step-by-step tutorials and sample code.
 
 ## Installation
 
 Follow the [Installation](https://osmnx.readthedocs.io/en/stable/installation.html) guide to install OSMnx.
 
 ## Support
```

