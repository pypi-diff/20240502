# Comparing `tmp/georeader-spaceml-1.0.9.tar.gz` & `tmp/georeader-spaceml-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "georeader-spaceml-1.0.9.tar", last modified: Tue Dec  5 17:06:42 2023, max compression
+gzip compressed data, was "georeader-spaceml-1.1.tar", last modified: Thu May  2 07:52:01 2024, max compression
```

## Comparing `georeader-spaceml-1.0.9.tar` & `georeader-spaceml-1.1.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-12-05 17:06:42.611644 georeader-spaceml-1.0.9/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     7652 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.9/LICENSE
--rw-r--r--   0 gonzalo   (1000) gonzalo   (1000)     6573 2023-12-05 17:06:42.611644 georeader-spaceml-1.0.9/PKG-INFO
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     4455 2023-12-04 16:01:46.000000 georeader-spaceml-1.0.9/README.md
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-12-05 17:06:42.603644 georeader-spaceml-1.0.9/georeader/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)   118602 2023-10-10 04:52:24.000000 georeader-spaceml-1.0.9/georeader/SolarIrradiance_Thuillier.csv
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2154 2023-12-05 17:05:46.000000 georeader-spaceml-1.0.9/georeader/__init__.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2549 2023-10-02 08:09:01.000000 georeader-spaceml-1.0.9/georeader/abstract_reader.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2777 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.9/georeader/geodataarray.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    27143 2023-10-02 08:21:15.000000 georeader-spaceml-1.0.9/georeader/geotensor.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11353 2023-12-04 16:03:09.000000 georeader-spaceml-1.0.9/georeader/mosaic.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    10949 2023-12-05 09:26:06.000000 georeader-spaceml-1.0.9/georeader/plot.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    34153 2023-10-03 07:01:34.000000 georeader-spaceml-1.0.9/georeader/rasterio_reader.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     9514 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.9/georeader/rasterize.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    28167 2023-12-04 16:01:46.000000 georeader-spaceml-1.0.9/georeader/read.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-12-05 17:06:42.607644 georeader-spaceml-1.0.9/georeader/readers/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    57110 2023-07-20 07:42:55.000000 georeader-spaceml-1.0.9/georeader/readers/S2_SAFE_reader.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.9/georeader/readers/__init__.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12416 2023-05-05 11:24:40.000000 georeader-spaceml-1.0.9/georeader/readers/download_pv_product.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2450 2023-09-27 11:03:47.000000 georeader-spaceml-1.0.9/georeader/readers/download_utils.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     6864 2023-12-04 16:00:35.000000 georeader-spaceml-1.0.9/georeader/readers/ee_image.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    14067 2023-12-04 16:00:35.000000 georeader-spaceml-1.0.9/georeader/readers/ee_query.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    22398 2023-12-05 10:14:29.000000 georeader-spaceml-1.0.9/georeader/readers/emit.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    17293 2023-05-05 15:01:48.000000 georeader-spaceml-1.0.9/georeader/readers/probav_image_operational.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2156 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.9/georeader/readers/query_utils.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3991 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.9/georeader/readers/scihubcopernicus_query.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2199 2023-12-04 16:03:09.000000 georeader-spaceml-1.0.9/georeader/readers/tileserver.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     6764 2023-12-04 16:00:35.000000 georeader-spaceml-1.0.9/georeader/reflectance.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12131 2023-10-18 15:46:26.000000 georeader-spaceml-1.0.9/georeader/save.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       46 2023-07-13 10:32:41.000000 georeader-spaceml-1.0.9/georeader/save_cog.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5414 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.9/georeader/slices.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3575 2023-09-22 12:24:44.000000 georeader-spaceml-1.0.9/georeader/vectorize.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    10533 2023-10-06 08:27:54.000000 georeader-spaceml-1.0.9/georeader/window_utils.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-12-05 17:06:42.607644 georeader-spaceml-1.0.9/georeader_spaceml.egg-info/
--rw-r--r--   0 gonzalo   (1000) gonzalo   (1000)     6573 2023-12-05 17:06:42.000000 georeader-spaceml-1.0.9/georeader_spaceml.egg-info/PKG-INFO
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1077 2023-12-05 17:06:42.000000 georeader-spaceml-1.0.9/georeader_spaceml.egg-info/SOURCES.txt
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        1 2023-12-05 17:06:42.000000 georeader-spaceml-1.0.9/georeader_spaceml.egg-info/dependency_links.txt
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      502 2023-12-05 17:06:42.000000 georeader-spaceml-1.0.9/georeader_spaceml.egg-info/requires.txt
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       10 2023-12-05 17:06:42.000000 georeader-spaceml-1.0.9/georeader_spaceml.egg-info/top_level.txt
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       38 2023-12-05 17:06:42.611644 georeader-spaceml-1.0.9/setup.cfg
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2325 2023-11-14 08:36:01.000000 georeader-spaceml-1.0.9/setup.py
-drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2023-12-05 17:06:42.607644 georeader-spaceml-1.0.9/tests/
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3796 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.9/tests/test_geotensor.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3583 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.9/tests/test_rasterio_reader.py
--rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11460 2023-04-26 06:58:45.000000 georeader-spaceml-1.0.9/tests/test_xarray_utils.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-02 07:52:01.227955 georeader-spaceml-1.1/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     7652 2023-04-26 06:58:45.000000 georeader-spaceml-1.1/LICENSE
+-rw-r--r--   0 gonzalo   (1000) gonzalo   (1000)     9377 2024-05-02 07:52:01.227955 georeader-spaceml-1.1/PKG-INFO
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     6803 2024-05-02 07:50:25.000000 georeader-spaceml-1.1/README.md
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-02 07:52:01.223955 georeader-spaceml-1.1/georeader/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)   118602 2023-10-10 04:52:24.000000 georeader-spaceml-1.1/georeader/SolarIrradiance_Thuillier.csv
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2178 2024-05-02 07:42:26.000000 georeader-spaceml-1.1/georeader/__init__.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2549 2023-10-02 08:09:01.000000 georeader-spaceml-1.1/georeader/abstract_reader.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5139 2024-04-02 07:44:03.000000 georeader-spaceml-1.1/georeader/dataarray.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    28666 2024-05-02 05:57:00.000000 georeader-spaceml-1.1/georeader/geotensor.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     9257 2024-02-28 17:48:55.000000 georeader-spaceml-1.1/georeader/griddata.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11516 2024-03-01 12:59:18.000000 georeader-spaceml-1.1/georeader/mosaic.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11134 2024-01-09 11:32:45.000000 georeader-spaceml-1.1/georeader/plot.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    35477 2024-03-05 14:52:32.000000 georeader-spaceml-1.1/georeader/rasterio_reader.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     9514 2023-04-26 06:58:45.000000 georeader-spaceml-1.1/georeader/rasterize.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    34265 2024-04-03 08:10:54.000000 georeader-spaceml-1.1/georeader/read.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-02 07:52:01.223955 georeader-spaceml-1.1/georeader/readers/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    57165 2024-05-02 07:44:41.000000 georeader-spaceml-1.1/georeader/readers/S2_SAFE_reader.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        0 2023-04-26 06:58:45.000000 georeader-spaceml-1.1/georeader/readers/__init__.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12416 2023-05-05 11:24:40.000000 georeader-spaceml-1.1/georeader/readers/download_pv_product.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2454 2024-02-28 16:40:43.000000 georeader-spaceml-1.1/georeader/readers/download_utils.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     7268 2024-04-03 08:57:10.000000 georeader-spaceml-1.1/georeader/readers/ee_image.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    14121 2024-01-05 10:02:42.000000 georeader-spaceml-1.1/georeader/readers/ee_query.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    33154 2024-04-10 11:36:43.000000 georeader-spaceml-1.1/georeader/readers/emit.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12527 2024-03-01 21:44:02.000000 georeader-spaceml-1.1/georeader/readers/prisma.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    18850 2024-05-02 07:44:13.000000 georeader-spaceml-1.1/georeader/readers/probav_image_operational.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2156 2023-04-26 06:58:45.000000 georeader-spaceml-1.1/georeader/readers/query_utils.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3991 2023-04-26 06:58:45.000000 georeader-spaceml-1.1/georeader/readers/scihubcopernicus_query.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    13864 2024-05-02 07:45:05.000000 georeader-spaceml-1.1/georeader/readers/spotvgt_image_operational.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2258 2023-12-21 09:41:42.000000 georeader-spaceml-1.1/georeader/readers/tileserver.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12969 2024-03-04 07:44:43.000000 georeader-spaceml-1.1/georeader/reflectance.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    12131 2023-10-18 15:46:26.000000 georeader-spaceml-1.1/georeader/save.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       46 2023-07-13 10:32:41.000000 georeader-spaceml-1.1/georeader/save_cog.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     5414 2023-04-26 06:58:45.000000 georeader-spaceml-1.1/georeader/slices.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3575 2023-09-22 12:24:44.000000 georeader-spaceml-1.1/georeader/vectorize.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11423 2024-04-03 08:56:42.000000 georeader-spaceml-1.1/georeader/window_utils.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-02 07:52:01.223955 georeader-spaceml-1.1/georeader_spaceml.egg-info/
+-rw-r--r--   0 gonzalo   (1000) gonzalo   (1000)     9377 2024-05-02 07:52:01.000000 georeader-spaceml-1.1/georeader_spaceml.egg-info/PKG-INFO
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     1171 2024-05-02 07:52:01.000000 georeader-spaceml-1.1/georeader_spaceml.egg-info/SOURCES.txt
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)        1 2024-05-02 07:52:01.000000 georeader-spaceml-1.1/georeader_spaceml.egg-info/dependency_links.txt
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)      513 2024-05-02 07:52:01.000000 georeader-spaceml-1.1/georeader_spaceml.egg-info/requires.txt
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       10 2024-05-02 07:52:01.000000 georeader-spaceml-1.1/georeader_spaceml.egg-info/top_level.txt
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)       38 2024-05-02 07:52:01.227955 georeader-spaceml-1.1/setup.cfg
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     2780 2023-12-19 08:18:42.000000 georeader-spaceml-1.1/setup.py
+drwxrwxr-x   0 gonzalo   (1000) gonzalo   (1000)        0 2024-05-02 07:52:01.223955 georeader-spaceml-1.1/tests/
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3796 2023-04-26 06:58:45.000000 georeader-spaceml-1.1/tests/test_geotensor.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)     3583 2023-04-26 06:58:45.000000 georeader-spaceml-1.1/tests/test_rasterio_reader.py
+-rw-rw-r--   0 gonzalo   (1000) gonzalo   (1000)    11460 2023-04-26 06:58:45.000000 georeader-spaceml-1.1/tests/test_xarray_utils.py
```

### Comparing `georeader-spaceml-1.0.9/LICENSE` & `georeader-spaceml-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.9/georeader/SolarIrradiance_Thuillier.csv` & `georeader-spaceml-1.1/georeader/SolarIrradiance_Thuillier.csv`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.9/georeader/__init__.py` & `georeader-spaceml-1.1/georeader/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.9"
+__version__ = "1.1"
 
 import math
 from typing import Tuple, Any, Union
 from shapely.geometry.base import BaseGeometry
 from shapely import Geometry
 from shapely.geometry import shape, mapping
 import rasterio.warp
@@ -62,11 +62,12 @@
         EPSG CRS object
     
     """
     
     # lat, lon = mgrs.MGRS().toLatLon(mgrs_tile)
 
 
-    crs = CRS.from_dict({"proj":"utm", "zone": int(mgrs_tile[:2]), 
+    crs = CRS.from_dict({"proj":"utm", 
+                         "zone": int(mgrs_tile[:2]), 
                          "south": mgrs_tile[2] < "N"})
     return crs
```

### Comparing `georeader-spaceml-1.0.9/georeader/abstract_reader.py` & `georeader-spaceml-1.1/georeader/abstract_reader.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.9/georeader/geotensor.py` & `georeader-spaceml-1.1/georeader/geotensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 from typing import Any, Dict, Union, Tuple, Optional, List
 import rasterio
 import rasterio.windows
 from georeader import window_utils
 from georeader.window_utils import window_bounds
 from numpy.typing import ArrayLike
 from itertools import product
-from shapely.geometry import Polygon
+from shapely.geometry import Polygon, MultiPolygon
 import numbers
+from numpy.typing import NDArray
 
 try:
     import torch
     import torch.nn.functional
-    Tensor = Union[torch.Tensor, np.ndarray]
+    Tensor = Union[torch.Tensor, NDArray]
     torch_installed = True
 except ImportError:
-    Tensor =np.ndarray
+    Tensor = NDArray
     torch_installed = False
 
 ORDERS = {
     'nearest': 0,
     'bilinear': 1,
     'bicubic': 2,
 }
@@ -375,14 +376,49 @@
         """
         pol = window_utils.window_polygon(rasterio.windows.Window(row_off=0, col_off=0, height=self.shape[-2], width=self.shape[-1]),
                                           self.transform)
         if (crs is None) or window_utils.compare_crs(self.crs, crs):
             return pol
 
         return window_utils.polygon_to_crs(pol, self.crs, crs)
+    
+    def valid_footprint(self, crs:Optional[str]=None, method:str="all") -> Union[MultiPolygon, Polygon]:
+        """
+        vectorizes the valid values of the GeoTensor and returns the footprint as a Polygon.
+
+        Args:
+            crs (Optional[str], optional): Coordinate reference system. Defaults to None.
+            method (str, optional): "all" or "any" to aggregate the channels of the image. Defaults to "all".
+
+        Returns:
+            Polygon or MultiPolygon: footprint of the GeoTensor.
+        """
+        valid_values = self.values != self.fill_value_default
+        if len(valid_values.shape) > 2:
+            if method == "all":
+                valid_values = np.all(valid_values, 
+                                      axis=tuple(np.arange(0, len(valid_values.shape)-2).tolist()))
+            elif method == "any":
+                valid_values = np.any(valid_values, 
+                                      axis=tuple(np.arange(0, len(valid_values.shape)-2).tolist()))
+            else:
+                raise NotImplementedError(f"Method {method} to aggregate channels not implemented")
+
+        from georeader import vectorize
+        polygons = vectorize.get_polygons(valid_values, transform=self.transform)
+        if len(polygons) == 0:
+            raise ValueError("GeoTensor has no valid values")
+        elif len(polygons) == 1:
+            pol = polygons[0]
+        else:
+            pol = MultiPolygon(polygons)
+        if crs is None:
+            return pol
+        
+        return window_utils.polygon_to_crs(pol, self.crs, crs)
 
     def __repr__(self)->str:
         return f""" 
          Transform: {self.transform}
          Shape: {self.shape}
          Resolution: {self.res}
          Bounds: {self.bounds}
@@ -629,16 +665,15 @@
 
     first_geotensor = geotensors[0]
     array_out = np.zeros((len(geotensors),) + first_geotensor.shape,
                          dtype=first_geotensor.dtype)
     array_out[0] = first_geotensor.values
 
     for i, geo in enumerate(geotensors[1:]):
-        assert geo.crs == first_geotensor.crs, f"Different crs in concat"
-        assert geo.transform == first_geotensor.transform, f"Different transform in concat"
+        assert geo.same_extent(first_geotensor), f"Different size in concat"
         assert geo.shape == first_geotensor.shape, f"Different shape in concat"
         assert geo.fill_value_default == first_geotensor.fill_value_default, "Different fill_value_default in concat"
         array_out[i + 1] = geo.values
 
     return GeoTensor(array_out, transform=first_geotensor.transform, crs=first_geotensor.crs,
                      fill_value_default=first_geotensor.fill_value_default)
```

### Comparing `georeader-spaceml-1.0.9/georeader/mosaic.py` & `georeader-spaceml-1.1/georeader/mosaic.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 def spatial_mosaic(data_list:Union[List[GeoData], List[Tuple[GeoData,GeoData]]],
                    polygon:Optional[Polygon]=None,
                    crs_polygon:Optional[str]=None,
                    dst_transform:Optional[rasterio.transform.Affine]=None,
                    bounds:Optional[Tuple[float, float, float, float]]=None,
                    dst_crs:Optional[str]=None,
+                   dtype_dst:Optional[str]=None,
                    window_size: Optional[Tuple[int, int]]= None,
                    resampling:rasterio.warp.Resampling=rasterio.warp.Resampling.cubic_spline,
                    masking_function:Optional[Callable[[GeoData], GeoData]]=None,
                    dst_nodata:Optional[int]=None) -> GeoTensor:
     """
     Computes the spatial mosaic of all input products in `data_list`. It iteratively calls `read_reproject` with
     all the list of rasters while there is any `dst_nodata` value. This function m requires that the copy of the output
@@ -94,14 +95,15 @@
     dst_transform = rasterio.windows.transform(window_polygon, transform=dst_transform)
     dst_nodata = dst_nodata or first_data_object.fill_value_default
 
     # Get object to save the results
     data_return = read_reproject(first_data_object,
                                  dst_crs=dst_crs, dst_transform=dst_transform,
                                  resampling=resampling,
+                                 dtype_dst=dtype_dst,
                                  window_out=rasterio.windows.Window(row_off=0, col_off=0, width=window_polygon.width,
                                                                     height=window_polygon.height),
                                  dst_nodata=dst_nodata)
 
     # invalid_values of spatial locations only  -> any
     invalid_values = data_return.values == dst_nodata
     if len(data_return.shape) > 2:
@@ -199,14 +201,15 @@
                 assert len(invalid_geotensor.shape) == 2, f"Invalid mask expected 2 dims found {invalid_geotensor.shape}"
                 if np.all(invalid_geotensor.values):
                     continue
                 invalid_values_iter = invalid_geotensor.values
 
             data_read = read_reproject(geodata, dst_crs=dst_crs, window_out=window_reproject_iter,
                                        dst_transform=dst_transform_iter, resampling=resampling,
+                                       dtype_dst=dtype_dst,
                                        dst_nodata=dst_nodata)
 
             if (geomask is None) and (masking_function is not None):
                 invalid_geotensor = masking_function(data_read)
 
                 invalid_geotensor.values = invalid_geotensor.values.astype(bool)
                 invalid_geotensor.values = invalid_geotensor.values.squeeze()
```

### Comparing `georeader-spaceml-1.0.9/georeader/plot.py` & `georeader-spaceml-1.1/georeader/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,25 +145,27 @@
     
     return ax
 
 def add_shape_to_plot(shape:Union[gpd.GeoDataFrame, List[Geometry], Geometry], ax:Optional[plt.Axes]=None,
                       crs_plot:Optional[Any]=None,
                       crs_shape:Optional[Any]=None,
                       polygon_no_fill:bool=False,
-                      kwargs_geopandas_plot:Optional[Any]=None) -> plt.Axes:
+                      kwargs_geopandas_plot:Optional[Any]=None,
+                      title:Optional[str]=None) -> plt.Axes:
     """
     Adds a shape to a plot. It uses geopandas.plot.
 
     Args:
         shape (Union[gpd.GeoDataFrame, List[Geometry], Geometry]): geodata to plot
         ax (Optional[plt.Axes], optional): Defaults to None. Axes to plot the shape
         crs_plot (Optional[Any], optional): Defaults to None. crs to plot the shape. If None, the crs of the shape is used.
         crs_shape (Optional[Any], optional): Defaults to None. crs of the shape. If None, the crs of the plot is used.
         polygon_no_fill: If True, the polygons are plotted without fill.
         kwargs_geopandas_plot (Optional[Any], optional): Defaults to None. Keyword arguments for geopandas.plot
+        title (Optional[str], optional): Defaults to None. Title of the plot.
 
     Returns:
         plt.Axes: 
     """
     if not isinstance(shape, gpd.GeoDataFrame):
         if isinstance(shape, Geometry):
             shape = [shape]
@@ -184,14 +186,17 @@
     if kwargs_geopandas_plot is None:
         kwargs_geopandas_plot = {}
 
     if polygon_no_fill:
         shape.boundary.plot(ax=ax, **kwargs_geopandas_plot)
     else:
         shape.plot(ax=ax, **kwargs_geopandas_plot)
+    
+    if title is not None:
+        ax.set_title(title)
 
     # if legend and color is not None:
     #     color_unique = color.unique()
     #     legend_elements = [Patch(facecolor=color_unique,  label=c) for c in color_unique]
     #     ax.legend(handles=legend_elements)
     
     return ax
```

### Comparing `georeader-spaceml-1.0.9/georeader/rasterio_reader.py` & `georeader-spaceml-1.1/georeader/rasterio_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import rasterio
 import rasterio.windows
 import numpy as np
-from typing import Tuple, Dict, List, Optional, Union
+from typing import Tuple, Dict, List, Optional, Union, Any
 import warnings
 import numbers
 from georeader import geotensor
 from collections.abc import Iterable
 from georeader import window_utils
 from georeader.window_utils import window_bounds, get_slice_pad
 from shapely.geometry import Polygon
 from georeader.abstract_reader import same_extent, GeoData
+from georeader.read import WEB_MERCATOR_CRS, SIZE_DEFAULT, window_from_tile, read_from_tile
 
 # https://developmentseed.org/titiler/advanced/performance_tuning/#aws-configuration
 RIO_ENV_OPTIONS_DEFAULT = dict(
     GDAL_DISABLE_READDIR_ON_OPEN='EMPTY_DIR',
     GDAL_HTTP_MERGE_CONSECUTIVE_RANGES="YES",
     GDAL_CACHEMAX=2000, # GDAL raster block cache size. If its value is small (less than 100000), 
     # it is assumed to be measured in megabytes, otherwise in bytes. https://trac.osgeo.org/gdal/wiki/ConfigOptions#GDAL_CACHEMAX
@@ -124,19 +125,19 @@
         else:
             self.dims = ["band", "y", "x"]
 
         self._coords = None
 
         # Assert all paths have same tranform and crs
         #  (checking width and height will not be needed since we're reading with boundless option but I don't see the point to ignore it)
-        if check:
+        if check and len(self.paths) > 1:
             for p in self.paths:
                 with rasterio.Env(**self.rio_env_options):
                     with rasterio.open(p, "r", overview_level=overview_level) as src:
-                        if not src.transform == self.real_transform:
+                        if not src.transform.almost_equals(self.real_transform, 1e-6):
                             raise ValueError(f"Different transform in {self.paths[0]} and {p}: {self.real_transform} {src.transform}")
                         if not str(src.crs).lower() == str(self.crs).lower():
                             raise ValueError(f"Different CRS in {self.paths[0]} and {p}: {self.crs} {src.crs}")
                         if self.real_count != src.count:
                             raise ValueError(f"Different number of bands in {self.paths[0]} and {p} {self.real_count} {src.count}")
                         if src.nodata != self.nodata:
                             warnings.warn(
@@ -646,14 +647,45 @@
             if obj_out.shape[0] == 1:
                 obj_out = obj_out[0]
             else:
                 obj_out = np.concatenate([obj_out[i] for i in range(obj_out.shape[0])],
                                          axis=0)
 
         return obj_out
+    
+    def read_from_tile(self, x:int, y:int, z:int, 
+                       out_shape:Tuple[int,int]=(SIZE_DEFAULT, SIZE_DEFAULT),
+                       dst_crs:Optional[Any]=WEB_MERCATOR_CRS) -> geotensor.GeoTensor:
+        """
+        Read a web mercator tile from a raster.
+        
+        Tiles are TMS tiles defined as: (https://wiki.openstreetmap.org/wiki/Slippy_map_tilenames)
+
+        Args:
+            x (int): x coordinate of the tile in the TMS system.
+            y (int): y coordinate of the tile in the TMS system.
+            z (int): z coordinate of the tile in the TMS system.
+            out_shape (Tuple[int,int]: size of the tile to read. Defaults to (read.SIZE_DEFAULT, read.SIZE_DEFAULT).
+            dst_crs (Optional[Any], optional): CRS of the output tile. Defaults to read.WEB_MERCATOR_CRS.
+            
+        Returns:
+            geotensor.GeoTensor: geotensor with the tile data.
+        """
+        window = window_from_tile(self, x, y, z)
+        window = window_utils.round_outer_window(window)
+        data = read_out_shape(self, out_shape=out_shape, window=window)
+
+        if window_utils.compare_crs(self.crs, dst_crs):
+            return data
+        
+        # window = window_utils.pad_window(window, (1, 1))
+        # data = read_out_shape(self, out_shape=size_out, window=window)
+
+        return read_from_tile(data, x, y, z, dst_crs=dst_crs, out_shape=out_shape)
+        
 
 def _get_pad_list(pad_width:Dict[str,Tuple[int,int]]):
     pad_list_np = [(0, 0)]
     for k in ["y", "x"]:
         if k in pad_width:
             pad_list_np.append(pad_width[k])
         else:
@@ -694,25 +726,20 @@
         assert size_read is not None, f"Both out_shape and size_read are None"
         out_shape = get_out_shape(shape, size_read)
     else:
         assert len(out_shape) == 2, f"Expected 2 dimensions found {out_shape}"
 
     transform = reader.transform if window is None else rasterio.windows.transform(window, reader.transform)
 
-    if indexes is None:
-        nbands = reader.count
-    elif isinstance(indexes, (list, tuple)):
+    if (indexes is not None) and isinstance(indexes, (list, tuple)):
         if len(out_shape) == 2:
             out_shape = (len(indexes),) + out_shape
     
     input_output_factor = (shape[0] / out_shape[-2], shape[1] / out_shape[-1])    
     transform = transform * rasterio.Affine.scale(input_output_factor[1], input_output_factor[0])
-        # transform = rasterio.Affine(transform.a * input_output_factor[1], transform.b, transform.c,
-        #                             transform.d, transform.e * input_output_factor[0], transform.f)
-
 
     output = reader.read(indexes=indexes, out_shape=out_shape, window=window)
 
     return geotensor.GeoTensor(output, transform=transform,
                                crs=reader.crs, fill_value_default=getattr(reader, "fill_value_default",
                                                                           reader.nodata if reader.nodata else fill_value_default))
```

### Comparing `georeader-spaceml-1.0.9/georeader/rasterize.py` & `georeader-spaceml-1.1/georeader/rasterize.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.9/georeader/read.py` & `georeader-spaceml-1.1/georeader/read.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import rasterio
 import rasterio.windows
 import rasterio.warp
 import rasterio.features
 import numbers
 import numpy as np
-from math import ceil
+from math import ceil, copysign
 from typing import Tuple, Union, Optional, Dict, Any
 from collections import OrderedDict
 import itertools
 from georeader.geotensor import GeoTensor
 from georeader import window_utils
 from georeader.window_utils import PIXEL_PRECISION, pad_window, round_outer_window, _is_exact_round
 from georeader.abstract_reader import GeoData
 from itertools import product
 from shapely.geometry import Polygon, MultiPolygon
+import mercantile
+from shapely.geometry import box
+import rasterio.transform
+
+SIZE_DEFAULT = 256
+WEB_MERCATOR_CRS = "EPSG:3857"
 
 
 def _round_all(x):
     x = tuple([int(round(xi)) for xi in x])
     return x
 
 
@@ -143,14 +149,36 @@
     # pixel_upper_left = _round_all(~transform * upper_left_coords)
 
     window = rasterio.windows.Window(row_off=pixel_upper_left[1], col_off=pixel_upper_left[0],
                                      width=shape[1], height=shape[0])
     return window
 
 
+def window_from_tile(data_in: Union[GeoData, rasterio.DatasetReader],
+                     x:int, y:int, z:int) -> rasterio.windows.Window:
+    """
+    Returns the window corresponding to the x,y,z tile in the data_in.
+
+    Tiles are TMS tiles defined as: (https://wiki.openstreetmap.org/wiki/Slippy_map_tilenames)
+
+    Args:
+        data_in (Union[GeoData, rasterio.DatasetReader]):  GeoData object
+        x (int): x coordinate of the tile in the TMS system.
+        y (int): y coordinate of the tile in the TMS system.
+        z (int): z coordinate of the tile in the TMS system.
+
+    Returns:
+        rasterio.windows.Window: window corresponding to the tile
+    """
+    bounds_wgs = mercantile.xy_bounds(int(x), int(y), int(z))
+    polygon_crs_webmercator = box(bounds_wgs.left, bounds_wgs.bottom, bounds_wgs.right, bounds_wgs.top)
+    return window_from_polygon(data_in, polygon_crs_webmercator, WEB_MERCATOR_CRS,
+                               window_surrounding=True)
+
+
 def read_from_window(data_in: GeoData,
                      window: rasterio.windows.Window, return_only_data: bool = False,
                      trigger_load: bool = False,
                      boundless: bool = True) -> Union[GeoData, np.ndarray, None]:
     """
     Reads a window from data_in padding with 0 if needed (output GeoData will have `window.height`, `window.width` shape
     if boundless is `True`).
@@ -285,37 +313,39 @@
         boundless: if `True` data read will always have the shape of the provided window
             (padding with `fill_value_default`)
         window_surrounding: The window surrounds the polygon. (i.e. `window.row_off` + `window.height` will not be a vertex)
 
     Returns:
         sliced GeoData
     """
-    window_in = window_from_polygon(data_in, polygon, crs_polygon, window_surrounding=window_surrounding)
+    window_in = window_from_polygon(data_in, polygon, crs_polygon, 
+                                    window_surrounding=window_surrounding)
     if any(p > 0 for p in pad_add):
         window_in = pad_window(window_in, pad_add)  # Add padding for bicubic int or for co-registration
     window_in = round_outer_window(window_in)
 
-    return read_from_window(data_in, window_in, return_only_data=return_only_data, trigger_load=trigger_load,
+    return read_from_window(data_in, window_in, return_only_data=return_only_data, 
+                            trigger_load=trigger_load,
                             boundless=boundless)
 
 
 def read_reproject_like(data_in: GeoData, data_like: GeoData,
                         resolution_dst:Optional[Union[float, Tuple[float, float]]]=None,
                         resampling: rasterio.warp.Resampling = rasterio.warp.Resampling.cubic_spline,
-                        dtpye_dst=None, return_only_data: bool = False,
+                        dtype_dst=None, return_only_data: bool = False,
                         dst_nodata: Optional[int] = None) -> Union[GeoTensor, np.ndarray]:
     """
     Reads from `data_in` and reprojects to have the same extent and resolution than `data_like`.
 
     Args:
         data_in: GeoData to read and reproject. Expected coords "x" and "y".
         data_like: GeoData to get the bounds and resolution to reproject `data_in`.
         resampling: specifies how data is reprojected from `rasterio.warp.Resampling`.
         resolution_dst: if not None it will overwrite the resolution of `data_like`.
-        dtpye_dst: if None it will be inferred
+        dtype_dst: if None it will be inferred
         return_only_data: defaults to `False`. If `True` it returns a np.ndarray otherwise
             returns an GeoTensor object (georreferenced array).
         dst_nodata: dst_nodata value
 
     Returns:
         GeoTensor read from `data_in` with same transform, crs, shape and bounds than `data_like`.
     """
@@ -329,15 +359,15 @@
 
         shape_out = int(round(shape_out[0] / resolution_dst[0] * resolution_data_like[0])), \
                     int(round(shape_out[1] / resolution_dst[1] * resolution_data_like[1]))
         
     return read_reproject(data_in, dst_crs=data_like.crs, dst_transform=data_like.transform,
                           resolution_dst_crs=resolution_dst,
                           window_out=rasterio.windows.Window(0,0, width=shape_out[-1], height=shape_out[-2]),
-                          resampling=resampling,dtpye_dst=dtpye_dst, return_only_data=return_only_data,
+                          resampling=resampling,dtype_dst=dtype_dst, return_only_data=return_only_data,
                           dst_nodata=dst_nodata)
 
 
 def resize(data_in:GeoData, resolution_dst:Union[float, Tuple[float, float]],
            window_out:Optional[rasterio.windows.Window]=None,
            anti_aliasing:bool=True, anti_aliasing_sigma:Optional[Union[float,np.ndarray]]=None,
            resampling: rasterio.warp.Resampling = rasterio.warp.Resampling.cubic_spline,
@@ -439,52 +469,69 @@
 
     Returns:
         Union[GeoTensor, np.ndarray]: data in dst_crs
     """
     if window_utils.compare_crs(data_in.crs, dst_crs):
         return data_in
 
+    window_data, dst_transform = calculate_transform_window(data_in, dst_crs, resolution_dst_crs)
+
+
+    return read_reproject(data_in, dst_crs=dst_crs,
+                          dst_transform=dst_transform,
+                          window_out=window_data,
+                          resampling=resampling, return_only_data=return_only_data)
+
+
+def calculate_transform_window(data_in:GeoData, dst_crs:Any, 
+                               resolution_dst_crs:Optional[Union[float, Tuple[float, float]]]=None) -> Tuple[rasterio.Affine, rasterio.windows.Window]:
+    """
+    Calculate the default transform to reproject data to dst_crs with resolution_dst_crs
+
+    Args:
+        data_in (GeoData): GeoData to reproyect
+        dst_crs (Any): dst crs
+        resolution_dst_crs (Optional[Union[float, Tuple[float, float]]], optional): Defaults to None.
+    """
+
     if resolution_dst_crs is not None:
         if isinstance(resolution_dst_crs, numbers.Number):
             resolution_dst_crs = (abs(resolution_dst_crs), abs(resolution_dst_crs))
     
     in_height, in_width = data_in.shape[-2:]
     dst_transform, width, height = rasterio.warp.calculate_default_transform(data_in.crs, dst_crs, in_width, in_height, *data_in.bounds,
                                                                              resolution=resolution_dst_crs)
     window_data = rasterio.windows.Window(0,0, width=width, height=height)
 
-
-    return read_reproject(data_in, dst_crs=dst_crs,
-                          dst_transform=dst_transform,
-                          window_out=window_data,
-                          resampling=resampling, return_only_data=return_only_data)
+    return window_data, dst_transform
 
 
 def read_reproject(data_in: GeoData, dst_crs: Optional[str]=None,
                    bounds: Optional[Tuple[float, float, float, float]]=None,
                    resolution_dst_crs: Optional[Union[float, Tuple[float, float]]]=None,
                    dst_transform:Optional[rasterio.Affine]=None,
                    window_out:Optional[rasterio.windows.Window]=None,
                    resampling: rasterio.warp.Resampling = rasterio.warp.Resampling.cubic_spline,
-                   dtpye_dst=None, return_only_data: bool = False, dst_nodata: Optional[int] = None) -> Union[
+                   dtype_dst=None, return_only_data: bool = False, dst_nodata: Optional[int] = None) -> Union[
     GeoTensor, np.ndarray]:
     """
     This function slices the data by the bounds and reprojects it to the dst_crs and resolution_dst_crs
 
     Args:
         data_in: GeoData to read and reproject. Expected coords "x" and "y".
         bounds: Optional. bounds in CRS specified by `dst_crs`. If not provided `window_out` must be given.
         dst_crs: CRS to reproject.
         resolution_dst_crs: resolution in the CRS specified by `dst_crs`. If not provided will use the the resolution
             intrinsic of `dst_transform`.
         dst_transform: Optional dest transform. If not provided the dst_transform is a rectilinear transform computed
         with the bounds and resolution_dst_crs.
         window_out: Window out to read w.r.t `dst_transform`. If not provided it is computed from the bounds.
+            Window out if provided has the output width and height of the reprojected data.
         resampling: specifies how data is reprojected from `rasterio.warp.Resampling`.
-        dtpye_dst: if None it will be data_in.dtype
+        dtype_dst: if None it will be data_in.dtype
         return_only_data: defaults to `False`. If `True` it returns a np.ndarray otherwise
             returns an GeoTensor object (georreferenced array).
         dst_nodata: dst_nodata value
 
     Returns:
         GeoTensor reprojected to dst_crs with resolution_dst_crs
 
@@ -522,46 +569,52 @@
                 window_in_data = window_in_data.round_offsets(op="floor", pixel_precision=PIXEL_PRECISION)
                 return read_from_window(data_in, window_in_data, return_only_data=return_only_data, trigger_load=True)
 
     isbool_dtypein = data_in.dtype == 'bool'
     isbool_dtypedst = False
 
     cast = True
-    if dtpye_dst is None:
+    if dtype_dst is None:
         cast = False
-        dtpye_dst = data_in.dtype
+        dtype_dst = data_in.dtype
         if isbool_dtypein:
             isbool_dtypedst = True
-    elif np.dtype(dtpye_dst) == 'bool':
+    elif np.dtype(dtype_dst) == 'bool':
         isbool_dtypedst = True
 
     # Create out array for reprojection
     dict_shape_window_out = {"x": window_out.width, "y": window_out.height}
     shape_out = tuple([named_shape[s] if s not in ["x", "y"] else dict_shape_window_out[s] for s in named_shape])
     dst_nodata = dst_nodata or data_in.fill_value_default
-    destination = np.full(shape_out,fill_value=dst_nodata, dtype=dtpye_dst)
+    destination = np.full(shape_out, fill_value=dst_nodata, dtype=dtype_dst)
+
+    polygon_dst_crs = window_utils.window_polygon(window_out, dst_transform)
+    
+    # If the polygon does not intersect the data return a GeoTensor with nodata
+    if not data_in.footprint(crs=dst_crs).intersects(polygon_dst_crs):
+        return GeoTensor(destination, transform=dst_transform, crs=dst_crs,
+                         fill_value_default=dst_nodata)
 
     if not isinstance(data_in, GeoTensor):
         # Compute real polygon that is going to be read
-        polygon_dst_crs = window_utils.window_polygon(window_out, dst_transform)
         # Read a padded window of the input data. This data will be then used for reprojection
         geotensor_in = read_from_polygon(data_in, polygon_dst_crs, crs_polygon=dst_crs,
                                          pad_add=(3, 3), return_only_data=False,
                                          trigger_load=True)
     else:
         geotensor_in = data_in
 
     # Triggering load makes that fill_value_default goes to nodata
     np_array_in = np.asanyarray(geotensor_in.values)
 
     if cast:
         if isbool_dtypedst:
             np_array_in = np_array_in.astype(np.float32)
         else:
-            np_array_in = np_array_in.astype(dtpye_dst)
+            np_array_in = np_array_in.astype(dtype_dst)
     elif isbool_dtypein:
         np_array_in = np_array_in.astype(np.float32)
 
 
     index_iter = [[(ns, i) for i in range(s)] for ns, s in named_shape.items() if ns not in ["x", "y"]]
     # e.g. if named_shape = {'time': 4, 'band': 2, 'x':10, 'y': 10} index_iter ->
     # [[('time', 0), ('time', 1), ('time', 2), ('time', 3)],
@@ -591,8 +644,77 @@
         if isbool_dtypedst:
             destination[i_sel_tuple] = (dst_iter_write > .5)
 
     if return_only_data:
         return destination
 
     return GeoTensor(destination, transform=dst_transform, crs=dst_crs,
-                     fill_value_default=dst_nodata)
+                     fill_value_default=dst_nodata)
+
+
+def read_from_tile(data:GeoData, x:int, y:int, z:int, dst_crs:Optional[Any]=WEB_MERCATOR_CRS, 
+                   out_shape:Optional[Tuple[int,int]]=(SIZE_DEFAULT, SIZE_DEFAULT), 
+                   resolution_dst_crs:Optional[Union[float, Tuple[float, float]]]=None,
+                   assert_if_not_intersects:bool=False) -> Optional[GeoTensor]:
+    """
+    Read a web mercator tile from a GeoData object. Tiles are TMS tiles defined as: (https://wiki.openstreetmap.org/wiki/Slippy_map_tilenames)
+
+    Args:
+        data (GeoData): GeoData object
+        x (int): x. x coordinate of the tile in the TMS system.
+        y (int): y. y coordinate of the tile in the TMS system.
+        z (int): z. zoom level
+        dst_crs (Optional[Any], optional): output crs. Defaults to WEB_MERCATOR_CRS. If None uses the crs of data.
+        out_shape (Optional[Tuple[int,int]], optional): output size. Defaults to (SIZE_DEFAULT, SIZE_DEFAULT). If None it will be the size
+            of the tile in the input resolution.
+        resolution_dst_crs (Optional[Union[float, Tuple[float, float]]], optional): output resolution. Defaults to None. 
+            If out_shape is not None it will be ignored. If None and out_shape is None the output will be at the resolution of the input data.
+        assert_if_not_intersects (bool, optional): If True it will raise an error if the tile does not intersect the data. Defaults to False.
+
+    Returns:
+        GeoTensor: GeoTensor covering the tile or None if the tile does not intersect the data.
+    """
+    bounds_wgs = mercantile.xy_bounds(int(x), int(y), int(z))
+    polygon_crs_webmercator = box(bounds_wgs.left, bounds_wgs.bottom, bounds_wgs.right, bounds_wgs.top)
+
+    intersects = polygon_crs_webmercator.intersects(data.footprint(crs=WEB_MERCATOR_CRS))
+    
+    if not intersects:
+        assert not assert_if_not_intersects, "Tile does not intersect data"
+    else:
+        return
+
+    if out_shape is not None and hasattr(data, "read_from_tile"):
+        return data.read_from_tile(x, y, z, dst_crs=dst_crs, out_shape=out_shape)
+    
+    if dst_crs is None:
+        dst_crs = data.crs
+        
+    if window_utils.compare_crs(data.crs, dst_crs) and (out_shape is None) and (resolution_dst_crs is None):
+        # read from polygon handles the case where the data does not intersect the polygon
+        return read_from_polygon(data, polygon_crs_webmercator, WEB_MERCATOR_CRS, window_surrounding=True).load()
+    
+    if out_shape is not None:
+        polygon_crs_dst = window_utils.polygon_to_crs(polygon_crs_webmercator, WEB_MERCATOR_CRS, dst_crs)
+        bounds_dst = polygon_crs_dst.bounds
+        dst_transform = rasterio.transform.from_bounds(*bounds_dst, 
+                                                       width=out_shape[1], height=out_shape[0])
+        window_data = rasterio.windows.Window(0, 0, width=out_shape[1], height=out_shape[0])
+    else:
+        if resolution_dst_crs is not None:
+            if isinstance(resolution_dst_crs, numbers.Number):
+                resolution_dst_crs = (abs(resolution_dst_crs), abs(resolution_dst_crs))
+        
+        polygon_crs_data = window_utils.polygon_to_crs(polygon_crs_webmercator, WEB_MERCATOR_CRS, data.crs)
+        bounds_crs_data = polygon_crs_data.bounds
+    
+        in_height, in_width = data.shape[-2:]
+        dst_transform, width, height = rasterio.warp.calculate_default_transform(data.crs, dst_crs, in_width, in_height, *bounds_crs_data,
+                                                                                resolution=resolution_dst_crs)
+        window_data = rasterio.windows.Window(0,0, width=width, height=height)
+        dst_transform, window_data = calculate_transform_window(data, dst_crs, resolution_dst_crs)
+
+    return read_reproject(data, dst_crs=dst_crs, dst_transform=dst_transform, 
+                          window_out=window_data)
+    
+    
+
```

### Comparing `georeader-spaceml-1.0.9/georeader/readers/S2_SAFE_reader.py` & `georeader-spaceml-1.1/georeader/readers/S2_SAFE_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 Sentinel-2 reader inherited from https://github.com/IPL-UV/DL-L8S2-UV.
 
+Authors: Gonzalo Mateo-García, Dan Lopez-Puigdollers
+
 It has several enhancements:
 * Support for S2L2A images
 * It can read directly images from a GCP bucket (for example data from  [here](https://cloud.google.com/storage/docs/public-datasets/sentinel-2))
 * Windowed read and read and reproject in the same function (see `load_bands_bbox`)
 * Creation of the image only involves reading one metadata file (`xxx.SAFE/MTD_{self.producttype}.xml`)
 * Compatible with `georeader.read` functions
 * It reads from pyramid if possible
```

### Comparing `georeader-spaceml-1.0.9/georeader/readers/download_pv_product.py` & `georeader-spaceml-1.1/georeader/readers/download_pv_product.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.9/georeader/readers/download_utils.py` & `georeader-spaceml-1.1/georeader/readers/download_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import shutil
 from typing import Optional, Any
 import requests
-from tqdm import tqdm
 
 def download_product(link_down:str, filename:Optional[str]=None, auth:Any=None, 
                      display_progress_bar:bool=True, verify:bool=True, 
                      headers:Optional[Any]=None) -> str:
     """
     Download a product from a link
 
@@ -28,14 +27,15 @@
         >>> # Download a Proba-V image
         >>> from georeader.readers.download_utils import download_product
         >>> from georeader.readers import download_pv_product
         >>> auth = download_pv_product.get_auth()
         >>> link_down = "https://www.vito-eodata.be/PDF/datapool/Free_Data/PROBA-V_100m/S1_TOA_100_m_C1/2019/2/9/PV_S1_TOA-20190209_100M_V101/PROBAV_S1_TOA_X07Y05_20190209_100M_V101.HDF5"
         >>> filename = download_product(link_down, auth=auth)
     """
+    from tqdm import tqdm
 
     if filename is None:
         filename = os.path.basename(link_down)
 
     if os.path.exists(filename):
         print(f"File {filename} exists. It won't be downloaded again")
         return filename
```

### Comparing `georeader-spaceml-1.0.9/georeader/readers/ee_image.py` & `georeader-spaceml-1.1/georeader/readers/ee_image.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from rasterio import Affine
 import numpy as np
 from collections import namedtuple
 from georeader import read, window_utils
 from io import BytesIO
 import rasterio
 from georeader import mosaic
+from concurrent.futures import ThreadPoolExecutor
 
 FakeGeoData=namedtuple("FakeGeoData",["crs", "transform"])
 
 
 def export_image_fast(image:ee.Image, geometry:Union[ee.Geometry, Polygon, MultiPolygon],
                       cat_bands:bool=True,
                       fill_value_default:Optional[float]=0,
@@ -78,14 +79,15 @@
         (mid_x, mid_y, max_x, max_y),  # Upper right quadrant
     ]
 
 def export_image_getpixels(asset_id: str,
                            geometry:Union[Polygon, MultiPolygon],
                            proj:Dict[str, Any],
                            bands_gee:List[str],
+                           dtype_dst:Optional[str]=None,
                            crs_polygon:str="EPSG:4326") -> GeoTensor:
     """
     Exports an image from the GEE as a GeoTensor. It uses the `ee.data.getPixels` method to export.
 
     Args:
         asset_id (str): Name of the asset
         geometry (Union[Polygon, MultiPolygon]): geometry to export
@@ -123,36 +125,44 @@
                         },
                         'crsCode': geodata.crs
                     }
                     })
         data = rasterio.open(BytesIO(data_raw))
         geotensor = GeoTensor(data.read(), transform=data.transform,
                              crs=data.crs, fill_value_default=data.nodata)
+        if dtype_dst is not None:
+            geotensor = geotensor.astype(dtype_dst)
+            
     except ee.EEException as e:
         # Check if the exception starts with Total request size
         if str(e).startswith("Total request size"):
             # Split the geometry in two and call recursively
             bounds = geometry.bounds
-            # Split the bounds in two
-            geotensors = []
-            for sb in split_bounds(bounds):
-                # Create a polygon with the bounds
+
+            def process_bound(sb):
                 poly = box(*sb)
-                # Call recursively
+                if not geometry.intersects(poly):
+                    return None
                 gt = export_image_getpixels(asset_id, poly, 
-                                            proj, bands_gee, crs_polygon)
-                # Concatenate the GeoTensor
-                geotensors.append(gt)
+                                            proj, bands_gee, dtype_dst, crs_polygon)
+                return gt
+
+            with ThreadPoolExecutor() as executor:
+                geotensors = list(executor.map(process_bound, split_bounds(bounds)))
+
+            # Remove None values from the list
+            geotensors = [gt for gt in geotensors if gt is not None]
             
             dst_crs = geotensors[0].crs
             aoi_dst_crs = window_utils.polygon_to_crs(geometry, 
                                                       crs_polygon=crs_polygon, 
                                                       dst_crs=dst_crs)
             
             geotensor = mosaic.spatial_mosaic(geotensors, 
+                                              dtype_dst=dtype_dst,
                                               polygon=aoi_dst_crs, 
                                               dst_crs=dst_crs)
         else:
             raise e
     return geotensor
```

### Comparing `georeader-spaceml-1.0.9/georeader/readers/ee_query.py` & `georeader-spaceml-1.1/georeader/readers/ee_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,20 +73,20 @@
 
     if return_collection:
         return geodf, img_col
 
     return geodf
 
 def figure_out_collection_landsat(tile:str) -> str:
-    if tile.startswith("LC08"):
+    if tile.startswith("LC08") or tile.startswith("LO08"):
         if tile.endswith("T1_RT") or tile.endswith("T1"):
             return "LANDSAT/LC08/C02/T1_RT_TOA"
         elif tile.endswith("T2"):
             return "LANDSAT/LC08/C02/T2_TOA"
-    elif tile.startswith("LC09"):
+    elif tile.startswith("LC09") or tile.startswith("LO09"):
         if tile.endswith("T1"):
             return "LANDSAT/LC09/C02/T1_TOA"
         elif tile.endswith("T2"):
             return "LANDSAT/LC09/C02/T2_TOA"
     else:
         raise ValueError(f"Tile {tile} not recognized")
```

### Comparing `georeader-spaceml-1.0.9/georeader/readers/probav_image_operational.py` & `georeader-spaceml-1.1/georeader/readers/probav_image_operational.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,31 @@
+"""
+Proba-V reader
+
+Unnoficial Proba-V reader. This reader is based in the Proba-V user manual: 
+https://publications.vito.be/2017-1333-probav-products-user-manual.pdf
+
+Author:  Gonzalo Mateo-García
+"""
+
 import numpy as np
 import h5py
 from datetime import datetime
 import os
 import re
 from datetime import timezone
 from h5py import h5z
 from rasterio import Affine
 import rasterio
 import rasterio.windows
 from typing import Tuple, List, Optional, Union
 from georeader import window_utils, geotensor
 from numbers import Number
 from shapely.geometry import Polygon
+import rasterio.crs
 
 
 FILTERS_HDF5 = { 'gzip': h5z.FILTER_DEFLATE,
                  'szip': h5z.FILTER_SZIP,
                  'shuffle': h5z.FILTER_SHUFFLE,
                  'lzf': h5z.FILTER_LZF,
                  'so': h5z.FILTER_SCALEOFFSET,
@@ -93,15 +103,15 @@
                                               "%Y-%m-%d %H:%M:%S").replace(tzinfo=timezone.utc)
             self.start_date = datetime.strptime(" ".join(self.metadata["OBSERVATION_START_DATE"].astype(str).tolist()+
                                                          self.metadata["OBSERVATION_START_TIME"].astype(str).tolist()),
                                                 "%Y-%m-%d %H:%M:%S").replace(tzinfo=timezone.utc)
             self.map_projection_wkt = " ".join(self.metadata["MAP_PROJECTION_WKT"].astype(str).tolist())
 
         # Proba-V images are lat/long
-        self.crs = {'init': 'epsg:4326'}
+        self.crs = rasterio.crs.CRS({'init': 'epsg:4326'})
 
         # Proba-V images have four bands
         self.level_name = level_name
 
     def _get_window_pad(self, boundless:bool=True)->Tuple[rasterio.windows.Window, Optional[List]]:
         window_read = rasterio.windows.intersection(self.window_focus, self.window_data)
 
@@ -126,14 +136,18 @@
     def footprint(self, crs:Optional[str]=None) -> Polygon:
         # TODO load footprint from metadata?
         pol = window_utils.window_polygon(self.window_focus, self.transform)
         if (crs is None) or window_utils.compare_crs(self.crs, crs):
             return pol
 
         return window_utils.polygon_to_crs(pol, self.crs, crs)
+    
+    def valid_footprint(self, crs:Optional[str]=None) -> Polygon:
+        valids = self.load_mask()
+        return valids.valid_footprint(crs=crs)
 
     def _load_bands(self, bands_names:Union[List[str],str], boundless:bool=True,
                     fill_value_default:Number=0) -> geotensor.GeoTensor:
         window_read, pad_list_np = self._get_window_pad(boundless=boundless)
         slice_ = window_read.toslices()
         if isinstance(bands_names, str):
             bands_names = [bands_names]
@@ -141,15 +155,15 @@
         else:
             flatten = False
 
         with h5py.File(self.hdf5_file, "r") as input_f:
             bands_arrs = []
             for band in bands_names:
                 data = read_band_toa(input_f, band, slice_)
-                if pad_list_np:
+                if pad_list_np is not None:
                     data = np.pad(data, tuple(pad_list_np), mode="constant",
                                   constant_values=fill_value_default)
 
                 bands_arrs.append(data)
 
         if boundless:
             transform = self.transform
@@ -216,17 +230,35 @@
         * `2**9` coverage nir
         * `2**10` coverage red
         * `2**11` coverage blue
         """
         return self._load_bands(f'{self.level_name}/QUALITY/SM', boundless=boundless, fill_value_default=0)
 
     def load_mask(self,boundless:bool=True) -> geotensor.GeoTensor:
+        """
+        Returns the valid mask (False if the pixel is out of swath or is invalid). This function loads the SM band
+
+        Args:
+            boundless (bool, optional): boundless option to load the SM band. Defaults to True.
+
+        Returns:
+            geotensor.GeoTensor: mask with the same shape as the image
+        """
+        valids = self.load_sm(boundless=boundless)
+        valids.values = ~mask_only_sm(valids.values)
+        valids.fill_value_default = False
+        return valids
+    
+    def load_sm_cloud_mask(self, mask_undefined:bool=False, boundless:bool=True) -> geotensor.GeoTensor:
         sm = self.load_sm(boundless=boundless)
-        sm.values = mask_only_sm(sm.values)
-        return sm
+        cloud_mask = sm_cloud_mask(sm.values, mask_undefined=mask_undefined)
+        cloud_mask+=1
+        invalids = mask_only_sm(sm.values)
+        cloud_mask[invalids] = 0
+        return geotensor.GeoTensor(cloud_mask, transform=self.transform, crs=self.crs, fill_value_default=0)
 
     def is_recompressed_and_chunked(self) -> bool:
         original_bands = [f"{self.level_name}/RADIOMETRY/{b}/{self.toatoc}" for b in BAND_NAMES]
         original_bands.append(f"{self.level_name}/QUALITY/SM")
         with h5py.File(self.hdf5_file, "r") as input_:
             for b in original_bands:
                 if input_[b].compression == "szip":
@@ -376,45 +408,56 @@
 
     def __copy__(self) -> '__class__':
         return ProbaVSM(self.hdf5_file, window=self.window_focus, level_name=self.level_name)
 
 
 def sm_cloud_mask(sm:np.ndarray, mask_undefined:bool=False) -> np.ndarray:
     """
-    Returns a binary cloud mask: 1 cloudy values 0 rest
+    Returns a binary cloud mask: 2 if cloud, 1 if clear, 0 if invalid
 
-    From user manual http://www.vito-eodata.be/PDF/image/PROBAV-Products_User_Manual.pdf pag 67
+    From user manual https://publications.vito.be/2017-1333-probav-products-user-manual.pdf Pag 64
         * Clear  ->    000
         * Shadow ->    001
         * Undefined -> 010
         * Cloud  ->    011
         * Ice    ->    100
 
     :param sm: (H, W) sm flags as loaded from ProbaVImageOperational.load_sm() method
-    :param mask_undefined: True returns np.ma.masked_array with undefined values masked
+    :param mask_undefined: if True returns also as clouds pixels those marked as undefined
     :return:
     """
-    cloud_mask = np.uint8((sm & 1 != 0) & (sm & 2**1 != 0) & (sm & 2**2 == 0))
+    cloud_mask = np.uint8(((sm & 1) != 0) & ((sm & 2**1) != 0) & ((sm & 2**2) == 0))
     if mask_undefined:
-        undefined_mask = (sm & 1 == 0) & (sm & 2**1 != 0) & (sm & 2**2 == 0)
-        cloud_mask = np.ma.masked_array(cloud_mask,undefined_mask)
+        undefined_mask = ((sm & 1) == 0) & ((sm & 2**1) != 0) & ((sm & 2**2) == 0)
+        cloud_mask |= undefined_mask
+    
+    cloud_mask += 1
+    invalids = mask_only_sm(sm)
+    cloud_mask[invalids] = 0
 
     return cloud_mask
 
 
 def mask_only_sm(sm:np.ndarray) -> np.ndarray:
-    mascara = np.zeros(sm.shape, dtype=bool)
-    for i in range(4):
-        mascara |= ((sm & (2 ** (i + 8))) == 0)
+    """
+    Returns a invalid mask: True if the pixel is out of swath
 
-    return mascara
+    https://publications.vito.be/2017-1333-probav-products-user-manual.pdf Pag 64
+
+    Bits 8..11: SWIR, NIR, RED, BLUE coverage flags
 
+    (If any of those bits is 0 the pixel is not covered, set as invalid)
 
-def mask_operational(bands:np.ndarray, sm:np.ndarray)-> np.ndarray:
-    # http://www.vito-eodata.be/PDF/image/PROBAV-Products_User_Manual.pdf
-    mascara = np.any(bands < 0, axis=-1)
-    mascara |= mask_only_sm(sm)
+    Args:
+        sm (np.ndarray): sm flags as loaded from ProbaVImageOperational.load_sm() method
+
+    Returns:
+        np.ndarray: mask with the same shape as the image
+    """
+    mascara = np.zeros(sm.shape, dtype=bool)
+    for i in range(4):
+        mascara |= ((sm & (2 ** (i + 8))) == 0)
 
     return mascara
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `georeader-spaceml-1.0.9/georeader/readers/query_utils.py` & `georeader-spaceml-1.1/georeader/readers/query_utils.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.9/georeader/readers/scihubcopernicus_query.py` & `georeader-spaceml-1.1/georeader/readers/scihubcopernicus_query.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.9/georeader/readers/tileserver.py` & `georeader-spaceml-1.1/georeader/readers/tileserver.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from io import BytesIO
 import numpy as np
 import georeader
 from georeader import window_utils
 from georeader import read
 import rasterio.windows
 import rasterio.transform
+from shapely.geometry import box
 
 def read_from_tileserver(tile_server:str, geometry:Union[Polygon, MultiPolygon],
                          zoom:int=16, crs_geometry:Any="EPSG:4326") -> GeoTensor:
     """
     Queries tiles from a tile server and returns it as a GeoTensor
 
     Args:
@@ -27,18 +28,20 @@
     Returns:
         GeoTensor: GeoTensor with the tile
     """
     if not georeader.compare_crs(crs_geometry, "EPSG:4326"):
         geometry = window_utils.polygon_to_crs(geometry, crs_geometry, "EPSG:4326")
 
     min_lon, min_lat, max_lon, max_lat = geometry.bounds
-    tiles = mercantile.simplify(mercantile.tiles(min_lon, min_lat, max_lon, max_lat, 
-                                                 zooms=zoom))
+    tiles = mercantile.tiles(min_lon, min_lat, max_lon, max_lat, zooms=zoom)
     geotensors = []
     for tile in tiles:
+        if not box(*mercantile.bounds(tile)).intersects(geometry):
+            continue
+        
         rsp = requests.get(tile_server.format(x=tile.x, y=tile.y, z=tile.z))
         img = Image.open(BytesIO(rsp.content))
         xmin, ymin, xmax, ymax = window_utils.normalize_bounds(mercantile.xy_bounds(tile))
         img_np = np.array(img).transpose(2,0,1)
        
         transform = rasterio.transform.from_bounds(west=xmin, south=ymin, east=xmax, north=ymax,
                                                    width=img_np.shape[2], height=img_np.shape[1])
```

### Comparing `georeader-spaceml-1.0.9/georeader/save.py` & `georeader-spaceml-1.1/georeader/save.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.9/georeader/slices.py` & `georeader-spaceml-1.1/georeader/slices.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.9/georeader/vectorize.py` & `georeader-spaceml-1.1/georeader/vectorize.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.9/georeader/window_utils.py` & `georeader-spaceml-1.1/georeader/window_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import rasterio.transform
 from typing import Tuple, Dict, Optional, Union, Any, List
 import numbers
 import numpy as np
 from shapely.geometry import Polygon, MultiPolygon, shape, mapping
 import rasterio.warp
 from georeader import compare_crs
+import math
 
 PIXEL_PRECISION = 3
 
 def pad_window(window: rasterio.windows.Window, pad_size: Tuple[int, int]) -> rasterio.windows.Window:
     """
     Add the provided pad to a rasterio window object
 
@@ -77,32 +78,55 @@
         return rasterio.transform.from_origin(min(bounds[0], bounds[2]),
                                               max(bounds[1], bounds[3]),
                                               resolution_dst[0], resolution_dst[1])
 
     if resolution_dst is None:
         dst_transform = transform
     else:
-        resolution_or = res(transform)
-        transform_scale = rasterio.Affine.scale(resolution_dst[0] / resolution_or[0],
-                                                resolution_dst[1] / resolution_or[1])
-        dst_transform = transform * transform_scale
+        dst_transform = transform_to_resolution_dst(transform, resolution_dst)
 
     if bounds is not None:
         # Shift the transform to start in the bounds
         window_current_transform = rasterio.windows.from_bounds(*bounds,
                                                                 transform=transform)
         dst_transform = rasterio.windows.transform(window_current_transform, dst_transform)
 
     return dst_transform
 
 
-def round_outer_window(window:rasterio.windows.Window)-> rasterio.windows.Window:
+def transform_to_resolution_dst(transform: rasterio.Affine, 
+                                resolution_dst: Union[float, Tuple[float, float]]) -> rasterio.Affine:
+    """
+    Change the transform to the given resolution
+
+    Args:
+        transform: transform to transform
+        resolution_dst: resolution of the output transform
+
+    Returns:
+        transformed transform
+    """
+    if isinstance(resolution_dst, numbers.Number):
+            resolution_dst = (abs(resolution_dst), abs(resolution_dst))
+
+    resolution_or = res(transform)
+    transform_scale = rasterio.Affine.scale(resolution_dst[0] / resolution_or[0],
+                                            resolution_dst[1] / resolution_or[1])
+    return transform * transform_scale
+
+
+def round_outer_window(window:rasterio.windows.Window, precision=PIXEL_PRECISION)-> rasterio.windows.Window:
     """ Rounds a rasterio.windows.Window object to outer (larger) window """
-    return window.round_lengths(op="ceil", pixel_precision=PIXEL_PRECISION).round_offsets(op="floor",
-                                                                                          pixel_precision=PIXEL_PRECISION)
+    row_dst = math.ceil(round(window.row_off + window.height, ndigits=precision))
+    col_dst = math.ceil(round(window.col_off + window.width, ndigits=precision))
+    col_off = math.floor(round(window.col_off, ndigits=precision))
+    row_off = math.floor(round(window.row_off, ndigits=precision))
+
+    return rasterio.windows.Window(col_off, row_off, 
+                                   col_dst-col_off, row_dst-row_off)
 
 # Precision to round the windows before applying ceiling/floor. e.g. 3.0001 will be rounded to 3 but 3.001 will not
 def _is_exact_round(x, precision=PIXEL_PRECISION):
     return abs(round(x,ndigits=precision)-x) < 1e-6
 
 
 def res(transform:rasterio.Affine) -> Tuple[float, float]:
@@ -253,15 +277,19 @@
     if ymin >= ymax:
         ymin-= margin_add_if_equal
         ymax+=margin_add_if_equal
 
     return xmin, ymin, xmax, ymax
 
 
-def polygon_to_crs(polygon:Union[Polygon, MultiPolygon], crs_polygon:Any, dst_crs:Any) -> Union[Polygon, MultiPolygon]:
+def polygon_to_crs(polygon:Union[Polygon, MultiPolygon], 
+                   crs_polygon:Any, dst_crs:Any) -> Union[Polygon, MultiPolygon]:
+    if compare_crs(crs_polygon, dst_crs):
+        return polygon
+    
     return shape(rasterio.warp.transform_geom(crs_polygon, dst_crs, mapping(polygon)))
 
 
 def pad_list_numpy(pad_width:Dict[str, Tuple[int, int]]) -> List[Tuple[int, int]]:
     pad_list_np = []
     for k in ["y", "x"]:
         if k in pad_width:
```

### Comparing `georeader-spaceml-1.0.9/georeader_spaceml.egg-info/SOURCES.txt` & `georeader-spaceml-1.1/georeader_spaceml.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 LICENSE
 README.md
 setup.py
 georeader/SolarIrradiance_Thuillier.csv
 georeader/__init__.py
 georeader/abstract_reader.py
-georeader/geodataarray.py
+georeader/dataarray.py
 georeader/geotensor.py
+georeader/griddata.py
 georeader/mosaic.py
 georeader/plot.py
 georeader/rasterio_reader.py
 georeader/rasterize.py
 georeader/read.py
 georeader/reflectance.py
 georeader/save.py
@@ -20,17 +21,19 @@
 georeader/readers/S2_SAFE_reader.py
 georeader/readers/__init__.py
 georeader/readers/download_pv_product.py
 georeader/readers/download_utils.py
 georeader/readers/ee_image.py
 georeader/readers/ee_query.py
 georeader/readers/emit.py
+georeader/readers/prisma.py
 georeader/readers/probav_image_operational.py
 georeader/readers/query_utils.py
 georeader/readers/scihubcopernicus_query.py
+georeader/readers/spotvgt_image_operational.py
 georeader/readers/tileserver.py
 georeader_spaceml.egg-info/PKG-INFO
 georeader_spaceml.egg-info/SOURCES.txt
 georeader_spaceml.egg-info/dependency_links.txt
 georeader_spaceml.egg-info/requires.txt
 georeader_spaceml.egg-info/top_level.txt
 tests/test_geotensor.py
```

### Comparing `georeader-spaceml-1.0.9/setup.py` & `georeader-spaceml-1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -57,10 +57,20 @@
       long_description_content_type="text/markdown",
       packages=find_packages(".", exclude=["tests"]),
        package_data={
         "georeader" : ["SolarIrradiance_Thuillier.csv"]
        },
       description="Lightweight reader for raster files",
       install_requires=parse_requirements_file("requirements.txt"),
+      url="https://github.com/spaceml-org/georeader",
+      classifiers=[
+        "Programming Language :: Python :: 3.10",
+        "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
+        "Operating System :: OS Independent",
+        "Intended Audience :: Science/Research",
+        "Natural Language :: English",
+        "Topic :: Scientific/Engineering :: GIS",
+        "Development Status :: 5 - Production/Stable", 
+    ],
       extras_require=EXTRAS,
       keywords=["raster reading", "rasterio"],
 )
```

### Comparing `georeader-spaceml-1.0.9/tests/test_geotensor.py` & `georeader-spaceml-1.1/tests/test_geotensor.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.9/tests/test_rasterio_reader.py` & `georeader-spaceml-1.1/tests/test_rasterio_reader.py`

 * *Files identical despite different names*

### Comparing `georeader-spaceml-1.0.9/tests/test_xarray_utils.py` & `georeader-spaceml-1.1/tests/test_xarray_utils.py`

 * *Files identical despite different names*

