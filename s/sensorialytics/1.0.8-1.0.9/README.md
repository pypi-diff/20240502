# Comparing `tmp/sensorialytics-1.0.8.tar.gz` & `tmp/sensorialytics-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sensorialytics-1.0.8.tar", last modified: Thu Feb 17 15:28:39 2022, max compression
+gzip compressed data, was "dist/sensorialytics-1.0.9.tar", last modified: Thu Feb 17 15:40:34 2022, max compression
```

## Comparing `sensorialytics-1.0.8.tar` & `sensorialytics-1.0.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:28:39.000000 sensorialytics-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      710 2022-02-17 15:28:39.000000 sensorialytics-1.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:28:39.000000 sensorialytics-1.0.8/sensorialytics/
--rw-rw-rw-   0 root         (0) root         (0)      447 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:28:39.000000 sensorialytics-1.0.8/sensorialytics/decorators/
--rw-rw-rw-   0 root         (0) root         (0)      591 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/decorators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:28:39.000000 sensorialytics-1.0.8/sensorialytics/helpers/
--rw-rw-rw-   0 root         (0) root         (0)      474 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/helpers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1350 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/helpers/dates.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/helpers/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2945 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/helpers/sensoria_io_client.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/helpers/timer.py
--rw-rw-rw-   0 root         (0) root         (0)     7332 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/helpers/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:28:39.000000 sensorialytics-1.0.8/sensorialytics/mathematics/
--rw-rw-rw-   0 root         (0) root         (0)      534 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/mathematics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      233 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/mathematics/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1970 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/mathematics/functions.py
--rw-rw-rw-   0 root         (0) root         (0)     1852 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/mathematics/point.py
--rw-rw-rw-   0 root         (0) root         (0)     2387 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/mathematics/polynomial.py
--rw-rw-rw-   0 root         (0) root         (0)     2446 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/mathematics/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:28:39.000000 sensorialytics-1.0.8/sensorialytics/plots/
--rw-rw-rw-   0 root         (0) root         (0)      199 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10897 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/plots/plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:28:39.000000 sensorialytics-1.0.8/sensorialytics/preprocessing/
--rw-rw-rw-   0 root         (0) root         (0)      548 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/preprocessing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6019 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/preprocessing/clustering.py
--rw-rw-rw-   0 root         (0) root         (0)    22072 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/preprocessing/encoders.py
--rw-rw-rw-   0 root         (0) root         (0)     6925 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/preprocessing/manipulations.py
--rw-rw-rw-   0 root         (0) root         (0)     5755 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/preprocessing/scalers.py
--rw-rw-rw-   0 root         (0) root         (0)     1219 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/preprocessing/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:28:39.000000 sensorialytics-1.0.8/sensorialytics/readers/
--rw-rw-rw-   0 root         (0) root         (0)      453 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/readers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12671 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/readers/core_data.py
--rw-rw-rw-   0 root         (0) root         (0)     6345 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/readers/events.py
--rw-rw-rw-   0 root         (0) root         (0)     3017 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/readers/fitfile.py
--rw-rw-rw-   0 root         (0) root         (0)     3374 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/readers/helper.py
--rw-rw-rw-   0 root         (0) root         (0)    13203 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/readers/session.py
--rw-rw-rw-   0 root         (0) root         (0)     7233 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/readers/sessions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:28:39.000000 sensorialytics-1.0.8/sensorialytics/sensors/
--rw-rw-rw-   0 root         (0) root         (0)      284 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/sensors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1857 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/sensors/pressure.py
--rw-rw-rw-   0 root         (0) root         (0)      203 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/sensors/sensor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:28:39.000000 sensorialytics-1.0.8/sensorialytics/signals/
--rw-rw-rw-   0 root         (0) root         (0)      364 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/signals/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5367 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/signals/detectors.py
--rw-rw-rw-   0 root         (0) root         (0)     5313 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/signals/filters.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/sensorialytics/signals/image.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:28:39.000000 sensorialytics-1.0.8/sensorialytics.egg-info/
--rw-r--r--   0 root         (0) root         (0)      710 2022-02-17 15:28:39.000000 sensorialytics-1.0.8/sensorialytics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1519 2022-02-17 15:28:39.000000 sensorialytics-1.0.8/sensorialytics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-02-17 15:28:39.000000 sensorialytics-1.0.8/sensorialytics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      140 2022-02-17 15:28:39.000000 sensorialytics-1.0.8/sensorialytics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-02-17 15:28:39.000000 sensorialytics-1.0.8/sensorialytics.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       79 2022-02-17 15:28:39.000000 sensorialytics-1.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1208 2022-02-17 15:28:19.000000 sensorialytics-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:40:34.000000 sensorialytics-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      710 2022-02-17 15:40:34.000000 sensorialytics-1.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:40:34.000000 sensorialytics-1.0.9/sensorialytics/
+-rw-rw-rw-   0 root         (0) root         (0)      447 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:40:34.000000 sensorialytics-1.0.9/sensorialytics/decorators/
+-rw-rw-rw-   0 root         (0) root         (0)      591 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/decorators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:40:34.000000 sensorialytics-1.0.9/sensorialytics/helpers/
+-rw-rw-rw-   0 root         (0) root         (0)      474 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/helpers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1350 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/helpers/dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/helpers/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2945 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/helpers/sensoria_io_client.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/helpers/timer.py
+-rw-rw-rw-   0 root         (0) root         (0)     7332 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/helpers/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:40:34.000000 sensorialytics-1.0.9/sensorialytics/mathematics/
+-rw-rw-rw-   0 root         (0) root         (0)      534 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/mathematics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      233 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/mathematics/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1970 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/mathematics/functions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/mathematics/point.py
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/mathematics/polynomial.py
+-rw-rw-rw-   0 root         (0) root         (0)     2446 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/mathematics/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:40:34.000000 sensorialytics-1.0.9/sensorialytics/plots/
+-rw-rw-rw-   0 root         (0) root         (0)      199 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10880 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/plots/plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:40:34.000000 sensorialytics-1.0.9/sensorialytics/preprocessing/
+-rw-rw-rw-   0 root         (0) root         (0)      548 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/preprocessing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6019 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/preprocessing/clustering.py
+-rw-rw-rw-   0 root         (0) root         (0)    22072 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/preprocessing/encoders.py
+-rw-rw-rw-   0 root         (0) root         (0)     6925 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/preprocessing/manipulations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5755 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/preprocessing/scalers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1219 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/preprocessing/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:40:34.000000 sensorialytics-1.0.9/sensorialytics/readers/
+-rw-rw-rw-   0 root         (0) root         (0)      453 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/readers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12663 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/readers/core_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     6345 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/readers/events.py
+-rw-rw-rw-   0 root         (0) root         (0)     3017 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/readers/fitfile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3374 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/readers/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)    13079 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/readers/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     7233 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/readers/sessions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:40:34.000000 sensorialytics-1.0.9/sensorialytics/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)      284 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/sensors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1857 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/sensors/pressure.py
+-rw-rw-rw-   0 root         (0) root         (0)      203 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/sensors/sensor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:40:34.000000 sensorialytics-1.0.9/sensorialytics/signals/
+-rw-rw-rw-   0 root         (0) root         (0)      364 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/signals/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5367 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/signals/detectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5313 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/signals/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/sensorialytics/signals/image.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 15:40:34.000000 sensorialytics-1.0.9/sensorialytics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      710 2022-02-17 15:40:34.000000 sensorialytics-1.0.9/sensorialytics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1519 2022-02-17 15:40:34.000000 sensorialytics-1.0.9/sensorialytics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-02-17 15:40:34.000000 sensorialytics-1.0.9/sensorialytics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      140 2022-02-17 15:40:34.000000 sensorialytics-1.0.9/sensorialytics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2022-02-17 15:40:34.000000 sensorialytics-1.0.9/sensorialytics.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       79 2022-02-17 15:40:34.000000 sensorialytics-1.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1208 2022-02-17 15:40:17.000000 sensorialytics-1.0.9/setup.py
```

### Comparing `sensorialytics-1.0.8/PKG-INFO` & `sensorialytics-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sensorialytics
-Version: 1.0.8
+Version: 1.0.9
 Summary: Sensoria python library
 Home-page: UNKNOWN
 Author: Stefano Rossotti
 Author-email: stefano@sensoriainc.com
 License: MIT
 Description: UNKNOWN
 Keywords: sensoria,analytics
```

### Comparing `sensorialytics-1.0.8/sensorialytics/decorators/__init__.py` & `sensorialytics-1.0.9/sensorialytics/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/helpers/dates.py` & `sensorialytics-1.0.9/sensorialytics/helpers/dates.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/helpers/sensoria_io_client.py` & `sensorialytics-1.0.9/sensorialytics/helpers/sensoria_io_client.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/helpers/tools.py` & `sensorialytics-1.0.9/sensorialytics/helpers/tools.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/mathematics/__init__.py` & `sensorialytics-1.0.9/sensorialytics/mathematics/__init__.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/mathematics/functions.py` & `sensorialytics-1.0.9/sensorialytics/mathematics/functions.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/mathematics/point.py` & `sensorialytics-1.0.9/sensorialytics/mathematics/point.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/mathematics/polynomial.py` & `sensorialytics-1.0.9/sensorialytics/mathematics/polynomial.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/mathematics/tools.py` & `sensorialytics-1.0.9/sensorialytics/mathematics/tools.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/plots/plots.py` & `sensorialytics-1.0.9/sensorialytics/plots/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,16 @@
     if y_list_secondary is None:
         y_list_secondary = []
 
     if len(x_list) > 1 and order is not None:
         if not isinstance(order, dict) and order not in order_choices:
             raise Exception(
                 'Error! order provided is invalid. Possible choices are: '
-                '{} or a dict shaped as {{x: order for x in x_list}}'
-                    .format(order_choices)
+                '{} or a dict shaped as {{x: order for x in x_list}}'.format(
+                    order_choices)
             )
 
         if isinstance(order, dict):
             if sum([x not in order.keys() for x in x_list]) > 0:
                 raise Exception(
                     'Error! not all the variables specified in \'x_list\' '
                     'are present in \'order\' dict'
@@ -182,16 +182,15 @@
 
     graph_string = dot_data.getvalue()
 
     for leaf_ID, leaf in enumerate(
             numpy.where(tree.tree_.children_left == -1)[0]):
         graph_string = graph_string.replace(
             '\n{} [label=<'.format(leaf),
-            '\n{} [label=<----- leaf {} -----<br/>'
-                .format(leaf, leaf_ID)
+            '\n{} [label=<----- leaf {} -----<br/>'.format(leaf, leaf_ID)
         )
 
     graph = pydotplus.graph_from_dot_data(graph_string)
 
     nodes = graph.get_node_list()
 
     for node in nodes:
```

### Comparing `sensorialytics-1.0.8/sensorialytics/preprocessing/__init__.py` & `sensorialytics-1.0.9/sensorialytics/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/preprocessing/clustering.py` & `sensorialytics-1.0.9/sensorialytics/preprocessing/clustering.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/preprocessing/encoders.py` & `sensorialytics-1.0.9/sensorialytics/preprocessing/encoders.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/preprocessing/manipulations.py` & `sensorialytics-1.0.9/sensorialytics/preprocessing/manipulations.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/preprocessing/scalers.py` & `sensorialytics-1.0.9/sensorialytics/preprocessing/scalers.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/preprocessing/tools.py` & `sensorialytics-1.0.9/sensorialytics/preprocessing/tools.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/readers/core_data.py` & `sensorialytics-1.0.9/sensorialytics/readers/core_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,16 +166,16 @@
                     e.g. {'Ax': ButterworthFilter}
                 - dict with {column_name: [Filter, Filter, ..]}
                     e.g. {'Ax': [
                                     ButterworthFilter(...),
                                     RecursiveAverageFilter(...)
                                 ]}
                     where the filters are applied in sequence
-        :param from_raw: set to True to use raw data as source for filtering, False
-                    for processed
+        :param from_raw: set to True to use raw data as source for filtering,
+            False for processed
         """
 
         self.__ensure_processed()
 
         source = self.__get_source(from_raw)
 
         for column, flt in filters.items():
@@ -185,16 +185,16 @@
             else:
                 self.__filter(flt, column=column, source=source)
 
     def offset(self, offsets: Dict[str, float], from_raw: bool = True) -> None:
         """
         Offsets the data using the values in offsets
         :param offsets: dict = dict composed as: {column_name : offset}
-        :param from_raw: set to True to use raw data as source for offsetting, False
-            for processed
+        :param from_raw: set to True to use raw data as source for offsetting,
+            False for processed
         """
 
         self.__ensure_processed()
 
         source = self.__get_source(from_raw)
 
         for column, offset in offsets.items():
@@ -202,16 +202,16 @@
 
     def scale(self, scaling_factors: Dict[str, float],
               from_raw: bool = True) -> None:
         """
         Scales the data using the values in scaling_factor
         :param scaling_factors: dict = dict composed as:
             {column_name : scale_factors}
-        :param from_raw: set to True to use raw data as source for scaling, False
-            for processed
+        :param from_raw: set to True to use raw data as source for scaling,
+            False for processed
         """
 
         self.__ensure_processed()
 
         source = self.__get_source(from_raw)
 
         for column, scaling in scaling_factors.items():
```

### Comparing `sensorialytics-1.0.8/sensorialytics/readers/events.py` & `sensorialytics-1.0.9/sensorialytics/readers/events.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/readers/fitfile.py` & `sensorialytics-1.0.9/sensorialytics/readers/fitfile.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/readers/helper.py` & `sensorialytics-1.0.9/sensorialytics/readers/helper.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/readers/session.py` & `sensorialytics-1.0.9/sensorialytics/readers/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -367,19 +367,18 @@
 
     def __read_app_session_data(self, session_dir: str):
         self.__read_app_raw(session_dir)
         self.__read_app_processed(session_dir)
         self.__read_app_events(session_dir)
 
     def __read_app_raw(self, session_dir):
-        print('here')
-        directory = os.path.join(session_dir, h.RAW_DIR_APP)
+        pass
 
     def __read_app_processed(self, session_dir):
-        directory = os.path.join(session_dir, h.PROCESSED_DIR_APP)
+        pass
 
     def __read_app_events(self, session_dir):
         directory = os.path.join(session_dir, h.EVENT_DIR_APP)
 
         events = pd.concat([
             Events(events_path=os.path.join(directory, filename))
             for filename in os.listdir(directory)
```

### Comparing `sensorialytics-1.0.8/sensorialytics/readers/sessions.py` & `sensorialytics-1.0.9/sensorialytics/readers/sessions.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/sensors/pressure.py` & `sensorialytics-1.0.9/sensorialytics/sensors/pressure.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/signals/detectors.py` & `sensorialytics-1.0.9/sensorialytics/signals/detectors.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/signals/filters.py` & `sensorialytics-1.0.9/sensorialytics/signals/filters.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics/signals/image.py` & `sensorialytics-1.0.9/sensorialytics/signals/image.py`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/sensorialytics.egg-info/PKG-INFO` & `sensorialytics-1.0.9/sensorialytics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sensorialytics
-Version: 1.0.8
+Version: 1.0.9
 Summary: Sensoria python library
 Home-page: UNKNOWN
 Author: Stefano Rossotti
 Author-email: stefano@sensoriainc.com
 License: MIT
 Description: UNKNOWN
 Keywords: sensoria,analytics
```

### Comparing `sensorialytics-1.0.8/sensorialytics.egg-info/SOURCES.txt` & `sensorialytics-1.0.9/sensorialytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sensorialytics-1.0.8/setup.py` & `sensorialytics-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #  setup.py
 #  Project: sensorialytics
 #  Copyright (c) 2022 Sensoria Health Inc.
 #  All rights reserved
 
 from setuptools import setup, find_packages
 
-VERSION = '1.0.8'
+VERSION = '1.0.9'
 
 setup(
     name='sensorialytics',
     packages=find_packages(),
     version=VERSION,
     license='MIT',
     description='Sensoria python library',
```

