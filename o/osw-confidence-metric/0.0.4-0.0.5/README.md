# Comparing `tmp/osw_confidence_metric-0.0.4-py3-none-any.whl.zip` & `tmp/osw_confidence_metric-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 12184 bytes, number of entries: 11
--rw-r--r--  2.0 unx       32 b- defN 24-Apr-25 05:05 osw_confidence_metric/__init__.py
--rw-r--r--  2.0 unx     4705 b- defN 24-Apr-25 05:05 osw_confidence_metric/area_analyzer.py
--rw-r--r--  2.0 unx      964 b- defN 24-Apr-25 05:05 osw_confidence_metric/osm_data_handler.py
--rw-r--r--  2.0 unx     8192 b- defN 24-Apr-25 05:05 osw_confidence_metric/trust_score_calculator.py
--rw-r--r--  2.0 unx    12040 b- defN 24-Apr-25 05:05 osw_confidence_metric/utils.py
--rw-r--r--  2.0 unx       21 b- defN 24-Apr-25 05:05 osw_confidence_metric/version.py
--rw-r--r--  2.0 unx     1073 b- defN 24-Apr-25 05:05 osw_confidence_metric-0.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx    10561 b- defN 24-Apr-25 05:05 osw_confidence_metric-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 05:05 osw_confidence_metric-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-25 05:05 osw_confidence_metric-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1016 b- defN 24-Apr-25 05:05 osw_confidence_metric-0.0.4.dist-info/RECORD
-11 files, 38718 bytes uncompressed, 10426 bytes compressed:  73.1%
+Zip file size: 12268 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       32 b- defN 24-May-02 09:09 osw_confidence_metric/__init__.py
+-rw-r--r--  2.0 unx     4927 b- defN 24-May-02 09:09 osw_confidence_metric/area_analyzer.py
+-rw-r--r--  2.0 unx      964 b- defN 24-May-02 09:09 osw_confidence_metric/osm_data_handler.py
+-rw-r--r--  2.0 unx     8192 b- defN 24-May-02 09:09 osw_confidence_metric/trust_score_calculator.py
+-rw-r--r--  2.0 unx    12040 b- defN 24-May-02 09:09 osw_confidence_metric/utils.py
+-rw-r--r--  2.0 unx       21 b- defN 24-May-02 09:09 osw_confidence_metric/version.py
+-rw-r--r--  2.0 unx     1073 b- defN 24-May-02 09:09 osw_confidence_metric-0.0.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx    10560 b- defN 24-May-02 09:09 osw_confidence_metric-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-02 09:09 osw_confidence_metric-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 24-May-02 09:09 osw_confidence_metric-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1016 b- defN 24-May-02 09:09 osw_confidence_metric-0.0.5.dist-info/RECORD
+11 files, 38939 bytes uncompressed, 10510 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: osw_confidence_metric/utils.py
 Comment: 
 
 Filename: osw_confidence_metric/version.py
 Comment: 
 
-Filename: osw_confidence_metric-0.0.4.dist-info/LICENSE
+Filename: osw_confidence_metric-0.0.5.dist-info/LICENSE
 Comment: 
 
-Filename: osw_confidence_metric-0.0.4.dist-info/METADATA
+Filename: osw_confidence_metric-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: osw_confidence_metric-0.0.4.dist-info/WHEEL
+Filename: osw_confidence_metric-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: osw_confidence_metric-0.0.4.dist-info/top_level.txt
+Filename: osw_confidence_metric-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: osw_confidence_metric-0.0.4.dist-info/RECORD
+Filename: osw_confidence_metric-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## osw_confidence_metric/area_analyzer.py

```diff
@@ -51,14 +51,16 @@
 
     def calculate_area_confidence_score(self, file_path):
         # Read the GeoDataFrame from the file
         self.gdf = gpd.read_file(file_path)
 
         # Check if tiling is needed and create tiling if necessary
         self._create_tiling_if_needed()
+        if self.gdf is None:
+            return 0
 
         # Initialize columns
         self.gdf = _initialize_columns(gdf=self.gdf)
 
         # Convert to Dask GeoDataFrame
         df_dask = dask_geopandas.from_geopandas(self.gdf, npartitions=16, name='measures')
 
@@ -93,15 +95,19 @@
         return mean_trust_score
 
     def _create_tiling_if_needed(self):
         if len(self.gdf.index) == 1:
             gdf_roads_simplified = ox.graph.graph_from_polygon(
                 self.gdf.geometry.loc[0], network_type='drive', simplify=True, retain_all=True
             )
-            self.gdf = self._create_voronoi_diagram(gdf_edges=gdf_roads_simplified, bounds=self.gdf.geometry.loc[0])
+            try:
+                self.gdf = self._create_voronoi_diagram(gdf_edges=gdf_roads_simplified, bounds=self.gdf.geometry.loc[0])
+            except Exception as e:
+                print("Error while creating voronoi diagram in confidence lib: ",e)
+                self.gdf = None
 
     def _create_voronoi_diagram(self, gdf_edges, bounds):
         """
         Creates a Voronoi diagram based on simplified road geometry and specified bounds.
         """
         gdf_roads_simplified = gnx.graph_edges_to_gdf(gdf_edges)
         voronoi = voronoi_diagram(gdf_roads_simplified.boundary.unary_union, envelope=bounds)
```

## osw_confidence_metric/version.py

```diff
@@ -1 +1 @@
-__version__ = '0.0.4'
+__version__ = '0.0.5'
```

## Comparing `osw_confidence_metric-0.0.4.dist-info/LICENSE` & `osw_confidence_metric-0.0.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `osw_confidence_metric-0.0.4.dist-info/METADATA` & `osw_confidence_metric-0.0.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osw-confidence-metric
-Version: 0.0.4
+Version: 0.0.5
 Summary: Calculates the confidence score of a given geojson area
 Home-page: https://github.com/TaskarCenterAtUW/TDEI-python-lib-confidence-metric
 Author: Sujata Misra
 Author-email: sujatam@gaussiansolutions.com
 Project-URL: Documentation, https://github.com/TaskarCenterAtUW/TDEI-python-lib-confidence-metric/blob/main/README.md
 Project-URL: GitHub, https://github.com/TaskarCenterAtUW/TDEI-python-lib-confidence-metric
 Project-URL: Changelog, https://github.com/TaskarCenterAtUW/TDEI-python-lib-confidence-metric/blob/main/CHANGELOG.md
@@ -65,15 +65,15 @@
 ### Testing
 
 The project is configured with `python` to figure out the coverage of the unit tests. All the tests are in `tests`
 folder.
 
 - To execute the tests, please follow the commands:
 
-  `pip install -r requirements.txt`
+  `pip install -r requirement.txt`
 
   `python -m unittest discover -v tests/unit_tests`
 
 - To execute the code coverage, please follow the commands:
 
   `python -m coverage run --source=src -m unittest discover -s tests/unit_tests`
```

## Comparing `osw_confidence_metric-0.0.4.dist-info/RECORD` & `osw_confidence_metric-0.0.5.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 osw_confidence_metric/__init__.py,sha256=8zLGg-DfQhnDl2Ky0n-zXpN-8e-g7iR0AcaI4l4Vvpk,32
-osw_confidence_metric/area_analyzer.py,sha256=6JfWbhmyAwQfy9tFHG7QpLsd7cX1qr-jjWqLSvIw8Dw,4705
+osw_confidence_metric/area_analyzer.py,sha256=byGnMQ1VTrVkhlcj6WUv8ZhQi2X6U-HRLCgwdbuGX1I,4927
 osw_confidence_metric/osm_data_handler.py,sha256=4m09avQHBPZpwmrQjd9DKp9Lj-N0QcQ62SnykCB-Qhg,964
 osw_confidence_metric/trust_score_calculator.py,sha256=mAlJUie9TBxdPY_kEtPTOoFTvCUHEC1Kg-ZQVlKn-e0,8192
 osw_confidence_metric/utils.py,sha256=hnnBNAGZCK7bv6rAEntFj3eP6HnRjqY3MavVQyhl1NQ,12040
-osw_confidence_metric/version.py,sha256=Qkdiz6Ybn1PE1SlWhKAQBmETf7pQ0yr5HmkqLVDxsqE,21
-osw_confidence_metric-0.0.4.dist-info/LICENSE,sha256=KXSpN2qzyPU7LuuGtJrQH4JsLkKmn077inwH99InLGw,1073
-osw_confidence_metric-0.0.4.dist-info/METADATA,sha256=3-_QdvNRXpk0uoqUfQuEzyAb16l3kub42bU7ylFfQ_k,10561
-osw_confidence_metric-0.0.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-osw_confidence_metric-0.0.4.dist-info/top_level.txt,sha256=Wd15KBVKmX49xc5WCCnrqkVodEBX9sn5zFPfglyc8mE,22
-osw_confidence_metric-0.0.4.dist-info/RECORD,,
+osw_confidence_metric/version.py,sha256=0Uc3zDF9XadX9j08cOIZbGoZsI0JPHTxemWum3gkos4,21
+osw_confidence_metric-0.0.5.dist-info/LICENSE,sha256=KXSpN2qzyPU7LuuGtJrQH4JsLkKmn077inwH99InLGw,1073
+osw_confidence_metric-0.0.5.dist-info/METADATA,sha256=80AONFNlNO11k-0PVPWDUUzLR7F8UmR0ZdwAWc3hrmw,10560
+osw_confidence_metric-0.0.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+osw_confidence_metric-0.0.5.dist-info/top_level.txt,sha256=Wd15KBVKmX49xc5WCCnrqkVodEBX9sn5zFPfglyc8mE,22
+osw_confidence_metric-0.0.5.dist-info/RECORD,,
```

