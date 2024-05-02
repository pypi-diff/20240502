# Comparing `tmp/django_mapengine-1.6.0.tar.gz` & `tmp/django_mapengine-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_mapengine-1.6.0.tar", max compression
+gzip compressed data, was "django_mapengine-1.6.1.tar", max compression
```

## Comparing `django_mapengine-1.6.0.tar` & `django_mapengine-1.6.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1069 2024-03-12 15:15:44.559160 django_mapengine-1.6.0/LICENSE
--rw-r--r--   0        0        0     3373 2024-03-26 11:51:33.500776 django_mapengine-1.6.0/README.md
--rw-r--r--   0        0        0       60 2024-04-25 07:43:15.134289 django_mapengine-1.6.0/django_mapengine/__init__.py
--rw-r--r--   0        0        0     3895 2024-04-25 07:43:15.134289 django_mapengine-1.6.0/django_mapengine/apps.py
--rw-r--r--   0        0        0     6738 2024-03-12 15:15:44.559160 django_mapengine-1.6.0/django_mapengine/choropleth.py
--rw-r--r--   0        0        0    43608 2024-03-12 15:15:44.559160 django_mapengine-1.6.0/django_mapengine/colorbrewer.py
--rw-r--r--   0        0        0     2230 2024-03-26 11:51:33.500776 django_mapengine-1.6.0/django_mapengine/distill.py
--rw-r--r--   0        0        0    10173 2024-04-24 10:17:38.710736 django_mapengine-1.6.0/django_mapengine/layers.py
--rw-r--r--   0        0        0      928 2024-03-14 11:59:59.035708 django_mapengine-1.6.0/django_mapengine/legend.py
--rw-r--r--   0        0        0     2516 2024-03-14 11:59:59.039708 django_mapengine-1.6.0/django_mapengine/mvt.py
--rw-r--r--   0        0        0     2161 2023-06-14 12:49:56.418190 django_mapengine-1.6.0/django_mapengine/popups.py
--rw-r--r--   0        0        0     4014 2024-04-24 10:17:38.710736 django_mapengine-1.6.0/django_mapengine/setup.py
--rw-r--r--   0        0        0     5664 2024-04-24 10:17:38.710736 django_mapengine-1.6.0/django_mapengine/sources.py
--rw-r--r--   0        0        0    12661 2024-04-25 07:43:15.134289 django_mapengine-1.6.0/django_mapengine/static/django_mapengine/images/layer_ctrl_dark.svg
--rw-r--r--   0        0        0    14131 2024-04-24 10:17:38.710736 django_mapengine-1.6.0/django_mapengine/static/django_mapengine/images/layer_ctrl_default.svg
--rw-r--r--   0        0        0    12284 2024-04-25 07:43:15.134289 django_mapengine-1.6.0/django_mapengine/static/django_mapengine/images/layer_ctrl_light.svg
--rw-r--r--   0        0        0    10121 2024-04-24 10:17:38.710736 django_mapengine-1.6.0/django_mapengine/static/django_mapengine/images/layer_ctrl_satellite.svg
--rw-r--r--   0        0        0     1262 2024-04-24 10:17:38.710736 django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/basemaps.js
--rw-r--r--   0        0        0     3220 2024-02-02 13:11:04.816042 django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/choropleth.js
--rw-r--r--   0        0        0      455 2024-03-12 15:15:44.559160 django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/events.js
--rw-r--r--   0        0        0      605 2023-06-14 12:49:56.422190 django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/helper.js
--rw-r--r--   0        0        0     1128 2023-08-23 11:10:37.048313 django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/init.js
--rw-r--r--   0        0        0     3577 2024-04-24 10:17:38.710736 django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/layer.js
--rw-r--r--   0        0        0     3069 2023-07-13 09:07:49.785869 django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/legend.js
--rw-r--r--   0        0        0     1782 2024-04-24 10:17:38.710736 django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/map.js
--rw-r--r--   0        0        0     2804 2024-03-12 15:15:49.899159 django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/popup.js
--rw-r--r--   0        0        0     2558 2023-06-14 12:49:56.422190 django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/regions.js
--rw-r--r--   0        0        0      513 2023-06-14 12:49:56.422190 django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/store.js
--rw-r--r--   0        0        0      318 2024-04-24 10:17:38.710736 django_mapengine-1.6.0/django_mapengine/templates/django_mapengine/map.html
--rw-r--r--   0        0        0     1227 2024-04-24 10:17:38.710736 django_mapengine-1.6.0/django_mapengine/templates/django_mapengine/map_basemaps.html
--rw-r--r--   0        0        0      937 2024-03-07 12:05:14.131045 django_mapengine-1.6.0/django_mapengine/templates/django_mapengine/map_js.html
--rw-r--r--   0        0        0      489 2024-04-24 10:17:38.710736 django_mapengine-1.6.0/django_mapengine/templates/django_mapengine/map_json.html
--rw-r--r--   0        0        0     1968 2024-03-14 11:59:59.039708 django_mapengine-1.6.0/django_mapengine/urls.py
--rw-r--r--   0        0        0     1264 2023-06-14 12:49:56.422190 django_mapengine-1.6.0/django_mapengine/utils.py
--rw-r--r--   0        0        0     2692 2024-04-24 10:17:38.710736 django_mapengine-1.6.0/django_mapengine/views.py
--rw-r--r--   0        0        0     1767 2024-04-25 07:43:15.134289 django_mapengine-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 django_mapengine-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-12 15:15:44.559160 django_mapengine-1.6.1/LICENSE
+-rw-r--r--   0        0        0     3373 2024-03-26 11:51:33.500776 django_mapengine-1.6.1/README.md
+-rw-r--r--   0        0        0       60 2024-05-02 15:35:08.093751 django_mapengine-1.6.1/django_mapengine/__init__.py
+-rw-r--r--   0        0        0     3895 2024-04-25 07:43:15.134289 django_mapengine-1.6.1/django_mapengine/apps.py
+-rw-r--r--   0        0        0     6738 2024-03-12 15:15:44.559160 django_mapengine-1.6.1/django_mapengine/choropleth.py
+-rw-r--r--   0        0        0    43608 2024-03-12 15:15:44.559160 django_mapengine-1.6.1/django_mapengine/colorbrewer.py
+-rw-r--r--   0        0        0     2230 2024-03-26 11:51:33.500776 django_mapengine-1.6.1/django_mapengine/distill.py
+-rw-r--r--   0        0        0    10173 2024-04-24 10:17:38.710736 django_mapengine-1.6.1/django_mapengine/layers.py
+-rw-r--r--   0        0        0      928 2024-03-14 11:59:59.035708 django_mapengine-1.6.1/django_mapengine/legend.py
+-rw-r--r--   0        0        0     2516 2024-03-14 11:59:59.039708 django_mapengine-1.6.1/django_mapengine/mvt.py
+-rw-r--r--   0        0        0     2161 2023-06-14 12:49:56.418190 django_mapengine-1.6.1/django_mapengine/popups.py
+-rw-r--r--   0        0        0     4014 2024-04-24 10:17:38.710736 django_mapengine-1.6.1/django_mapengine/setup.py
+-rw-r--r--   0        0        0     5664 2024-04-24 10:17:38.710736 django_mapengine-1.6.1/django_mapengine/sources.py
+-rw-r--r--   0        0        0    12661 2024-04-25 07:43:15.134289 django_mapengine-1.6.1/django_mapengine/static/django_mapengine/images/layer_ctrl_dark.svg
+-rw-r--r--   0        0        0    14131 2024-04-24 10:17:38.710736 django_mapengine-1.6.1/django_mapengine/static/django_mapengine/images/layer_ctrl_default.svg
+-rw-r--r--   0        0        0    12284 2024-04-25 07:43:15.134289 django_mapengine-1.6.1/django_mapengine/static/django_mapengine/images/layer_ctrl_light.svg
+-rw-r--r--   0        0        0    10121 2024-04-24 10:17:38.710736 django_mapengine-1.6.1/django_mapengine/static/django_mapengine/images/layer_ctrl_satellite.svg
+-rw-r--r--   0        0        0     1262 2024-04-24 10:17:38.710736 django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/basemaps.js
+-rw-r--r--   0        0        0     3220 2024-02-02 13:11:04.816042 django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/choropleth.js
+-rw-r--r--   0        0        0      455 2024-03-12 15:15:44.559160 django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/events.js
+-rw-r--r--   0        0        0      605 2023-06-14 12:49:56.422190 django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/helper.js
+-rw-r--r--   0        0        0     1128 2023-08-23 11:10:37.048313 django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/init.js
+-rw-r--r--   0        0        0     3577 2024-04-24 10:17:38.710736 django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/layer.js
+-rw-r--r--   0        0        0     3069 2023-07-13 09:07:49.785869 django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/legend.js
+-rw-r--r--   0        0        0     1782 2024-04-24 10:17:38.710736 django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/map.js
+-rw-r--r--   0        0        0     2804 2024-03-12 15:15:49.899159 django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/popup.js
+-rw-r--r--   0        0        0     2558 2023-06-14 12:49:56.422190 django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/regions.js
+-rw-r--r--   0        0        0      513 2023-06-14 12:49:56.422190 django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/store.js
+-rw-r--r--   0        0        0      318 2024-04-24 10:17:38.710736 django_mapengine-1.6.1/django_mapengine/templates/django_mapengine/map.html
+-rw-r--r--   0        0        0     1227 2024-04-24 10:17:38.710736 django_mapengine-1.6.1/django_mapengine/templates/django_mapengine/map_basemaps.html
+-rw-r--r--   0        0        0      937 2024-03-07 12:05:14.131045 django_mapengine-1.6.1/django_mapengine/templates/django_mapengine/map_js.html
+-rw-r--r--   0        0        0      489 2024-04-24 10:17:38.710736 django_mapengine-1.6.1/django_mapengine/templates/django_mapengine/map_json.html
+-rw-r--r--   0        0        0     1968 2024-03-14 11:59:59.039708 django_mapengine-1.6.1/django_mapengine/urls.py
+-rw-r--r--   0        0        0     1264 2023-06-14 12:49:56.422190 django_mapengine-1.6.1/django_mapengine/utils.py
+-rw-r--r--   0        0        0     2955 2024-05-02 15:33:21.033750 django_mapengine-1.6.1/django_mapengine/views.py
+-rw-r--r--   0        0        0     1767 2024-05-02 15:35:08.093751 django_mapengine-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 django_mapengine-1.6.1/PKG-INFO
```

### Comparing `django_mapengine-1.6.0/LICENSE` & `django_mapengine-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/README.md` & `django_mapengine-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/apps.py` & `django_mapengine-1.6.1/django_mapengine/apps.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/choropleth.py` & `django_mapengine-1.6.1/django_mapengine/choropleth.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/colorbrewer.py` & `django_mapengine-1.6.1/django_mapengine/colorbrewer.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/distill.py` & `django_mapengine-1.6.1/django_mapengine/distill.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/layers.py` & `django_mapengine-1.6.1/django_mapengine/layers.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/legend.py` & `django_mapengine-1.6.1/django_mapengine/legend.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/mvt.py` & `django_mapengine-1.6.1/django_mapengine/mvt.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/popups.py` & `django_mapengine-1.6.1/django_mapengine/popups.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/setup.py` & `django_mapengine-1.6.1/django_mapengine/setup.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/sources.py` & `django_mapengine-1.6.1/django_mapengine/sources.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/static/django_mapengine/images/layer_ctrl_dark.svg` & `django_mapengine-1.6.1/django_mapengine/static/django_mapengine/images/layer_ctrl_dark.svg`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/static/django_mapengine/images/layer_ctrl_default.svg` & `django_mapengine-1.6.1/django_mapengine/static/django_mapengine/images/layer_ctrl_default.svg`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/static/django_mapengine/images/layer_ctrl_light.svg` & `django_mapengine-1.6.1/django_mapengine/static/django_mapengine/images/layer_ctrl_light.svg`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/static/django_mapengine/images/layer_ctrl_satellite.svg` & `django_mapengine-1.6.1/django_mapengine/static/django_mapengine/images/layer_ctrl_satellite.svg`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/basemaps.js` & `django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/basemaps.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/choropleth.js` & `django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/choropleth.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/helper.js` & `django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/helper.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/init.js` & `django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/init.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/layer.js` & `django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/layer.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/legend.js` & `django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/legend.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/map.js` & `django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/map.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/popup.js` & `django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/popup.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/regions.js` & `django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/regions.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/static/django_mapengine/js/store.js` & `django_mapengine-1.6.1/django_mapengine/static/django_mapengine/js/store.js`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/templates/django_mapengine/map_basemaps.html` & `django_mapengine-1.6.1/django_mapengine/templates/django_mapengine/map_basemaps.html`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/templates/django_mapengine/map_js.html` & `django_mapengine-1.6.1/django_mapengine/templates/django_mapengine/map_js.html`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/urls.py` & `django_mapengine-1.6.1/django_mapengine/urls.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/utils.py` & `django_mapengine-1.6.1/django_mapengine/utils.py`

 * *Files identical despite different names*

### Comparing `django_mapengine-1.6.0/django_mapengine/views.py` & `django_mapengine-1.6.1/django_mapengine/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Views and mixins in order to use mapengine"""
 
+from itertools import chain
 from django.conf import settings
 from django.http import JsonResponse
 from django.views.generic.base import ContextMixin
 
 from . import __version__, layers, sources
 
 
@@ -44,15 +45,21 @@
                 "mapengine_zoom_levels": settings.MAP_ENGINE_ZOOM_LEVELS,
                 # Sources need valid URL (containing host and port), thus they have to be defined using request:
                 "mapengine_sources": {
                     source.name: source.get_source(self.request) for source in sources.get_all_sources()
                 },
                 "mapengine_basemap_layers": [basemap.as_dict() for basemap in settings.MAP_ENGINE_BASEMAPS],
                 "mapengine_layers": [layer.get_layer() for layer in layers.get_all_layers()],
-                "mapengine_layers_at_startup": settings.MAP_ENGINE_LAYERS_AT_STARTUP + settings.MAP_ENGINE_REGIONS,
+                "mapengine_layers_at_startup": settings.MAP_ENGINE_LAYERS_AT_STARTUP
+                + list(
+                    chain.from_iterable(
+                        [region_layer, f"{region_layer}-line", f"{region_layer}-label"]
+                        for region_layer in settings.MAP_ENGINE_REGIONS
+                    )
+                ),
                 "mapengine_images": [image.as_dict() for image in settings.MAP_ENGINE_IMAGES],
             }
         )
         store = {
             "debugMode": settings.MAP_ENGINE_DEBUG,
             "popups": {popup.layer_id: popup.as_dict() for popup in settings.MAP_ENGINE_POPUPS},
             "regions": settings.MAP_ENGINE_REGIONS,
```

### Comparing `django_mapengine-1.6.0/pyproject.toml` & `django_mapengine-1.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-mapengine"
-version = "1.6.0"
+version = "1.6.1"
 description = "Map engine for maplibre in django"
 authors = ["Hendrik Huyskens <hendrik.huyskens@rl-institut.de>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `django_mapengine-1.6.0/PKG-INFO` & `django_mapengine-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mapengine
-Version: 1.6.0
+Version: 1.6.1
 Summary: Map engine for maplibre in django
 Author: Hendrik Huyskens
 Author-email: hendrik.huyskens@rl-institut.de
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-mapengine Version: 1.6.0 Summary: Map engine
+Metadata-Version: 2.1 Name: django-mapengine Version: 1.6.1 Summary: Map engine
 for maplibre in django Author: Hendrik Huyskens Author-email:
 hendrik.huyskens@rl-institut.de Requires-Python: >=3.9,<3.12 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Dist: django-appconf (>=1.0.5,<2.0.0) Requires-Dist: django-distill
```

