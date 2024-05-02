# Comparing `tmp/zensvi-0.9.7.tar.gz` & `tmp/zensvi-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zensvi-0.9.7.tar", max compression
+gzip compressed data, was "zensvi-0.9.8.tar", max compression
```

## Comparing `zensvi-0.9.7.tar` & `zensvi-0.9.8.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.9.7/LICENSE
--rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.9.7/README.md
--rwxr-xr-x   0        0        0     1396 2024-02-03 07:27:07.416411 zensvi-0.9.7/pyproject.toml
--rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.9.7/src/zensvi/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.9.7/src/zensvi/cv/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.9.7/src/zensvi/cv/segmentation/__init__.py
--rwxr-xr-x   0        0        0    49342 2024-02-03 07:20:07.722540 zensvi-0.9.7/src/zensvi/cv/segmentation/segmentation.py
--rwxr-xr-x   0        0        0       61 2024-01-26 10:43:30.048802 zensvi-0.9.7/src/zensvi/download/__init__.py
--rw-r--r--   0        0        0     3706 2024-01-28 08:02:31.884372 zensvi-0.9.7/src/zensvi/download/base.py
--rw-r--r--   0        0        0    28168 2024-02-02 08:15:51.823870 zensvi-0.9.7/src/zensvi/download/gsv.py
--rw-r--r--   0        0        0      629 2023-07-11 07:03:47.656454 zensvi-0.9.7/src/zensvi/download/mapillary/__init__.py
--rw-r--r--   0        0        0        0 2023-07-11 07:03:47.656489 zensvi-0.9.7/src/zensvi/download/mapillary/config/.gitkeep
--rw-r--r--   0        0        0     1110 2023-07-11 07:03:47.656962 zensvi-0.9.7/src/zensvi/download/mapillary/config/__init__.py
--rw-r--r--   0        0        0      398 2023-07-11 07:03:47.657311 zensvi-0.9.7/src/zensvi/download/mapillary/config/api/__init__.py
--rw-r--r--   0        0        0    25264 2023-07-11 07:03:47.657833 zensvi-0.9.7/src/zensvi/download/mapillary/config/api/entities.py
--rw-r--r--   0        0        0     1917 2023-07-11 07:03:47.658201 zensvi-0.9.7/src/zensvi/download/mapillary/config/api/general.py
--rw-r--r--   0        0        0     8163 2023-07-11 07:03:47.658519 zensvi-0.9.7/src/zensvi/download/mapillary/config/api/vector_tiles.py
--rw-r--r--   0        0        0      481 2023-07-11 07:03:47.658811 zensvi-0.9.7/src/zensvi/download/mapillary/controller/__init__.py
--rw-r--r--   0        0        0     2297 2023-07-11 08:21:16.088478 zensvi-0.9.7/src/zensvi/download/mapillary/controller/detection.py
--rw-r--r--   0        0        0     4775 2023-07-11 08:21:17.279629 zensvi-0.9.7/src/zensvi/download/mapillary/controller/feature.py
--rw-r--r--   0        0        0    31549 2024-02-01 08:35:09.836321 zensvi-0.9.7/src/zensvi/download/mapillary/controller/image.py
--rw-r--r--   0        0        0     4904 2023-07-11 08:20:39.797301 zensvi-0.9.7/src/zensvi/download/mapillary/controller/save.py
--rw-r--r--   0        0        0    34990 2024-01-31 09:42:45.807371 zensvi-0.9.7/src/zensvi/download/mapillary/interface.py
--rw-r--r--   0        0        0        0 2023-07-11 07:03:47.660579 zensvi-0.9.7/src/zensvi/download/mapillary/models/.gitkeep
--rw-r--r--   0        0        0      520 2023-07-11 07:03:47.660843 zensvi-0.9.7/src/zensvi/download/mapillary/models/__init__.py
--rw-r--r--   0        0        0      396 2023-07-11 07:03:47.660998 zensvi-0.9.7/src/zensvi/download/mapillary/models/api/__init__.py
--rw-r--r--   0        0        0     8168 2023-07-11 08:21:35.171162 zensvi-0.9.7/src/zensvi/download/mapillary/models/api/entities.py
--rw-r--r--   0        0        0    14403 2023-07-11 08:23:11.396978 zensvi-0.9.7/src/zensvi/download/mapillary/models/api/general.py
--rw-r--r--   0        0        0    22684 2024-02-01 08:35:09.836872 zensvi-0.9.7/src/zensvi/download/mapillary/models/api/vector_tiles.py
--rw-r--r--   0        0        0     8273 2023-07-11 08:26:45.376434 zensvi-0.9.7/src/zensvi/download/mapillary/models/client.py
--rw-r--r--   0        0        0     1398 2023-07-11 07:03:47.662813 zensvi-0.9.7/src/zensvi/download/mapillary/models/config.py
--rw-r--r--   0        0        0    10328 2023-07-11 07:03:47.663102 zensvi-0.9.7/src/zensvi/download/mapillary/models/exceptions.py
--rw-r--r--   0        0        0    15339 2024-01-31 10:28:38.722674 zensvi-0.9.7/src/zensvi/download/mapillary/models/geojson.py
--rw-r--r--   0        0        0     2496 2023-07-11 07:03:47.663608 zensvi-0.9.7/src/zensvi/download/mapillary/models/logger.py
--rw-r--r--   0        0        0        0 2023-07-11 07:03:47.663642 zensvi-0.9.7/src/zensvi/download/mapillary/utils/.gitkeep
--rw-r--r--   0        0        0      547 2024-01-26 10:43:30.051669 zensvi-0.9.7/src/zensvi/download/mapillary/utils/__init__.py
--rw-r--r--   0        0        0     1774 2023-07-11 08:22:50.091875 zensvi-0.9.7/src/zensvi/download/mapillary/utils/auth.py
--rw-r--r--   0        0        0     2623 2024-01-26 10:43:30.051992 zensvi-0.9.7/src/zensvi/download/mapillary/utils/convert.py
--rw-r--r--   0        0        0     1750 2023-07-11 07:03:47.664341 zensvi-0.9.7/src/zensvi/download/mapillary/utils/extract.py
--rw-r--r--   0        0        0    19063 2024-02-01 08:35:09.837226 zensvi-0.9.7/src/zensvi/download/mapillary/utils/filter.py
--rw-r--r--   0        0        0    26693 2024-02-02 07:32:33.413231 zensvi-0.9.7/src/zensvi/download/mapillary/utils/format.py
--rw-r--r--   0        0        0     1723 2023-07-11 07:03:47.665237 zensvi-0.9.7/src/zensvi/download/mapillary/utils/time.py
--rw-r--r--   0        0        0     9976 2023-08-31 07:08:44.885753 zensvi-0.9.7/src/zensvi/download/mapillary/utils/verify.py
--rw-r--r--   0        0        0    17778 2024-02-01 09:22:13.144721 zensvi-0.9.7/src/zensvi/download/mly.py
--rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.9.7/src/zensvi/download/utils/UserAgent.csv
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.9.7/src/zensvi/download/utils/__init__.py
--rwxr-xr-x   0        0        0     9059 2023-08-28 05:01:25.595756 zensvi-0.9.7/src/zensvi/download/utils/geoprocess.py
--rwxr-xr-x   0        0        0     1810 2023-06-05 08:53:58.000000 zensvi-0.9.7/src/zensvi/download/utils/get_pids.py
--rwxr-xr-x   0        0        0     1470 2024-01-26 10:43:30.052597 zensvi-0.9.7/src/zensvi/download/utils/helpers.py
--rwxr-xr-x   0        0        0     9139 2024-02-01 08:35:09.837925 zensvi-0.9.7/src/zensvi/download/utils/imtool.py
--rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.9.7/src/zensvi/download/utils/proxies.csv
--rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.9.7/src/zensvi/transform/__init__.py
--rwxr-xr-x   0        0        0    10481 2024-01-26 10:43:30.053394 zensvi-0.9.7/src/zensvi/transform/transform_image.py
--rw-r--r--   0        0        0     3348 2024-01-31 09:42:45.810363 zensvi-0.9.7/src/zensvi/utils/log.py
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.9.7/src/zensvi/zensvi.py
--rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 zensvi-0.9.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.9.8/LICENSE
+-rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.9.8/README.md
+-rwxr-xr-x   0        0        0     1396 2024-02-08 02:41:07.972769 zensvi-0.9.8/pyproject.toml
+-rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.9.8/src/zensvi/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.9.8/src/zensvi/cv/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.9.8/src/zensvi/cv/segmentation/__init__.py
+-rwxr-xr-x   0        0        0    49342 2024-02-08 02:40:57.776059 zensvi-0.9.8/src/zensvi/cv/segmentation/segmentation.py
+-rwxr-xr-x   0        0        0       61 2024-01-26 10:43:30.048802 zensvi-0.9.8/src/zensvi/download/__init__.py
+-rw-r--r--   0        0        0     3706 2024-01-28 08:02:31.884372 zensvi-0.9.8/src/zensvi/download/base.py
+-rw-r--r--   0        0        0    28168 2024-02-02 08:15:51.823870 zensvi-0.9.8/src/zensvi/download/gsv.py
+-rw-r--r--   0        0        0      629 2023-07-11 07:03:47.656454 zensvi-0.9.8/src/zensvi/download/mapillary/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 07:03:47.656489 zensvi-0.9.8/src/zensvi/download/mapillary/config/.gitkeep
+-rw-r--r--   0        0        0     1110 2023-07-11 07:03:47.656962 zensvi-0.9.8/src/zensvi/download/mapillary/config/__init__.py
+-rw-r--r--   0        0        0      398 2023-07-11 07:03:47.657311 zensvi-0.9.8/src/zensvi/download/mapillary/config/api/__init__.py
+-rw-r--r--   0        0        0    25264 2023-07-11 07:03:47.657833 zensvi-0.9.8/src/zensvi/download/mapillary/config/api/entities.py
+-rw-r--r--   0        0        0     1917 2023-07-11 07:03:47.658201 zensvi-0.9.8/src/zensvi/download/mapillary/config/api/general.py
+-rw-r--r--   0        0        0     8163 2023-07-11 07:03:47.658519 zensvi-0.9.8/src/zensvi/download/mapillary/config/api/vector_tiles.py
+-rw-r--r--   0        0        0      481 2023-07-11 07:03:47.658811 zensvi-0.9.8/src/zensvi/download/mapillary/controller/__init__.py
+-rw-r--r--   0        0        0     2297 2023-07-11 08:21:16.088478 zensvi-0.9.8/src/zensvi/download/mapillary/controller/detection.py
+-rw-r--r--   0        0        0     4775 2023-07-11 08:21:17.279629 zensvi-0.9.8/src/zensvi/download/mapillary/controller/feature.py
+-rw-r--r--   0        0        0    31549 2024-02-01 08:35:09.836321 zensvi-0.9.8/src/zensvi/download/mapillary/controller/image.py
+-rw-r--r--   0        0        0     4904 2023-07-11 08:20:39.797301 zensvi-0.9.8/src/zensvi/download/mapillary/controller/save.py
+-rw-r--r--   0        0        0    34990 2024-01-31 09:42:45.807371 zensvi-0.9.8/src/zensvi/download/mapillary/interface.py
+-rw-r--r--   0        0        0        0 2023-07-11 07:03:47.660579 zensvi-0.9.8/src/zensvi/download/mapillary/models/.gitkeep
+-rw-r--r--   0        0        0      520 2023-07-11 07:03:47.660843 zensvi-0.9.8/src/zensvi/download/mapillary/models/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-11 07:03:47.660998 zensvi-0.9.8/src/zensvi/download/mapillary/models/api/__init__.py
+-rw-r--r--   0        0        0     8168 2023-07-11 08:21:35.171162 zensvi-0.9.8/src/zensvi/download/mapillary/models/api/entities.py
+-rw-r--r--   0        0        0    14403 2023-07-11 08:23:11.396978 zensvi-0.9.8/src/zensvi/download/mapillary/models/api/general.py
+-rw-r--r--   0        0        0    22684 2024-02-01 08:35:09.836872 zensvi-0.9.8/src/zensvi/download/mapillary/models/api/vector_tiles.py
+-rw-r--r--   0        0        0     8273 2023-07-11 08:26:45.376434 zensvi-0.9.8/src/zensvi/download/mapillary/models/client.py
+-rw-r--r--   0        0        0     1398 2023-07-11 07:03:47.662813 zensvi-0.9.8/src/zensvi/download/mapillary/models/config.py
+-rw-r--r--   0        0        0    10328 2023-07-11 07:03:47.663102 zensvi-0.9.8/src/zensvi/download/mapillary/models/exceptions.py
+-rw-r--r--   0        0        0    15339 2024-01-31 10:28:38.722674 zensvi-0.9.8/src/zensvi/download/mapillary/models/geojson.py
+-rw-r--r--   0        0        0     2496 2023-07-11 07:03:47.663608 zensvi-0.9.8/src/zensvi/download/mapillary/models/logger.py
+-rw-r--r--   0        0        0        0 2023-07-11 07:03:47.663642 zensvi-0.9.8/src/zensvi/download/mapillary/utils/.gitkeep
+-rw-r--r--   0        0        0      547 2024-01-26 10:43:30.051669 zensvi-0.9.8/src/zensvi/download/mapillary/utils/__init__.py
+-rw-r--r--   0        0        0     1774 2023-07-11 08:22:50.091875 zensvi-0.9.8/src/zensvi/download/mapillary/utils/auth.py
+-rw-r--r--   0        0        0     2623 2024-01-26 10:43:30.051992 zensvi-0.9.8/src/zensvi/download/mapillary/utils/convert.py
+-rw-r--r--   0        0        0     1750 2023-07-11 07:03:47.664341 zensvi-0.9.8/src/zensvi/download/mapillary/utils/extract.py
+-rw-r--r--   0        0        0    19063 2024-02-01 08:35:09.837226 zensvi-0.9.8/src/zensvi/download/mapillary/utils/filter.py
+-rw-r--r--   0        0        0    26693 2024-02-02 07:32:33.413231 zensvi-0.9.8/src/zensvi/download/mapillary/utils/format.py
+-rw-r--r--   0        0        0     1723 2023-07-11 07:03:47.665237 zensvi-0.9.8/src/zensvi/download/mapillary/utils/time.py
+-rw-r--r--   0        0        0     9976 2023-08-31 07:08:44.885753 zensvi-0.9.8/src/zensvi/download/mapillary/utils/verify.py
+-rw-r--r--   0        0        0    17778 2024-02-01 09:22:13.144721 zensvi-0.9.8/src/zensvi/download/mly.py
+-rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.9.8/src/zensvi/download/utils/UserAgent.csv
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.9.8/src/zensvi/download/utils/__init__.py
+-rwxr-xr-x   0        0        0     9059 2023-08-28 05:01:25.595756 zensvi-0.9.8/src/zensvi/download/utils/geoprocess.py
+-rwxr-xr-x   0        0        0     1810 2023-06-05 08:53:58.000000 zensvi-0.9.8/src/zensvi/download/utils/get_pids.py
+-rwxr-xr-x   0        0        0     1470 2024-01-26 10:43:30.052597 zensvi-0.9.8/src/zensvi/download/utils/helpers.py
+-rwxr-xr-x   0        0        0     9139 2024-02-01 08:35:09.837925 zensvi-0.9.8/src/zensvi/download/utils/imtool.py
+-rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.9.8/src/zensvi/download/utils/proxies.csv
+-rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.9.8/src/zensvi/transform/__init__.py
+-rwxr-xr-x   0        0        0    10481 2024-01-26 10:43:30.053394 zensvi-0.9.8/src/zensvi/transform/transform_image.py
+-rw-r--r--   0        0        0     3348 2024-01-31 09:42:45.810363 zensvi-0.9.8/src/zensvi/utils/log.py
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.9.8/src/zensvi/zensvi.py
+-rw-r--r--   0        0        0     3252 1970-01-01 00:00:00.000000 zensvi-0.9.8/PKG-INFO
```

### Comparing `zensvi-0.9.7/LICENSE` & `zensvi-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/README.md` & `zensvi-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/pyproject.toml` & `zensvi-0.9.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zensvi"
-version = "0.9.7"
+version = "0.9.8"
 description = "This package handles downloading, cleaning, analyzing street view imagery in a one-stop and zen manner."
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `zensvi-0.9.7/src/zensvi/cv/segmentation/segmentation.py` & `zensvi-0.9.8/src/zensvi/cv/segmentation/segmentation.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/base.py` & `zensvi-0.9.8/src/zensvi/download/base.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/gsv.py` & `zensvi-0.9.8/src/zensvi/download/gsv.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/__init__.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/__init__.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/config/__init__.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/config/__init__.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/config/api/entities.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/config/api/entities.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/config/api/general.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/config/api/general.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/config/api/vector_tiles.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/config/api/vector_tiles.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/controller/detection.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/controller/detection.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/controller/feature.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/controller/feature.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/controller/image.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/controller/image.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/controller/save.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/controller/save.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/interface.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/interface.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/models/__init__.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/models/__init__.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/models/api/entities.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/models/api/entities.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/models/api/general.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/models/api/general.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/models/api/vector_tiles.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/models/api/vector_tiles.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/models/client.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/models/client.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/models/config.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/models/config.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/models/exceptions.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/models/geojson.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/models/geojson.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/models/logger.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/models/logger.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/utils/__init__.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/utils/auth.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/utils/auth.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/utils/convert.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/utils/convert.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/utils/extract.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/utils/extract.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/utils/filter.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/utils/filter.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/utils/format.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/utils/format.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/utils/time.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/utils/time.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mapillary/utils/verify.py` & `zensvi-0.9.8/src/zensvi/download/mapillary/utils/verify.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/mly.py` & `zensvi-0.9.8/src/zensvi/download/mly.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/utils/UserAgent.csv` & `zensvi-0.9.8/src/zensvi/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/utils/geoprocess.py` & `zensvi-0.9.8/src/zensvi/download/utils/geoprocess.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/utils/get_pids.py` & `zensvi-0.9.8/src/zensvi/download/utils/get_pids.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/utils/helpers.py` & `zensvi-0.9.8/src/zensvi/download/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/utils/imtool.py` & `zensvi-0.9.8/src/zensvi/download/utils/imtool.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/download/utils/proxies.csv` & `zensvi-0.9.8/src/zensvi/download/utils/proxies.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/transform/transform_image.py` & `zensvi-0.9.8/src/zensvi/transform/transform_image.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/src/zensvi/utils/log.py` & `zensvi-0.9.8/src/zensvi/utils/log.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.9.7/PKG-INFO` & `zensvi-0.9.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: zensvi
-Version: 0.9.7
+Version: 0.9.8
 Summary: This package handles downloading, cleaning, analyzing street view imagery in a one-stop and zen manner.
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Pillow (>=10.0.0)
 Requires-Dist: Pygments (>=2.9.0,<3.0.0)
 Requires-Dist: Shapely (>=1.8.1)
 Requires-Dist: attrs (>=21.2.0,<22.0.0)
 Requires-Dist: bleach (>=3.3.0,<4.0.0)
 Requires-Dist: certifi (>=2021.5.30,<2022.0.0)
 Requires-Dist: chardet (>=4.0.0,<5.0.0)
```

