# Comparing `tmp/smartcitizen_connector-1.0.3.tar.gz` & `tmp/smartcitizen_connector-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartcitizen_connector-1.0.3.tar", last modified: Tue Apr 30 15:14:17 2024, max compression
+gzip compressed data, was "smartcitizen_connector-1.0.4.tar", last modified: Thu May  2 14:44:04 2024, max compression
```

## Comparing `smartcitizen_connector-1.0.3.tar` & `smartcitizen_connector-1.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:17.035314 smartcitizen_connector-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-30 15:14:11.000000 smartcitizen_connector-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-30 15:14:11.000000 smartcitizen_connector-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-30 15:14:17.035314 smartcitizen_connector-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-30 15:14:11.000000 smartcitizen_connector-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-30 15:14:17.035314 smartcitizen_connector-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-30 15:14:11.000000 smartcitizen_connector-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:17.031314 smartcitizen_connector-1.0.3/smartcitizen_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-30 15:14:11.000000 smartcitizen_connector-1.0.3/smartcitizen_connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:17.031314 smartcitizen_connector-1.0.3/smartcitizen_connector/_config/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-30 15:14:11.000000 smartcitizen_connector-1.0.3/smartcitizen_connector/_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-30 15:14:11.000000 smartcitizen_connector-1.0.3/smartcitizen_connector/_config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:17.031314 smartcitizen_connector-1.0.3/smartcitizen_connector/device/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-30 15:14:11.000000 smartcitizen_connector-1.0.3/smartcitizen_connector/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24439 2024-04-30 15:14:11.000000 smartcitizen_connector-1.0.3/smartcitizen_connector/device/device.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:17.031314 smartcitizen_connector-1.0.3/smartcitizen_connector/measurement/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 15:14:11.000000 smartcitizen_connector-1.0.3/smartcitizen_connector/measurement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-30 15:14:11.000000 smartcitizen_connector-1.0.3/smartcitizen_connector/measurement/measurement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:17.031314 smartcitizen_connector-1.0.3/smartcitizen_connector/models/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-30 15:14:11.000000 smartcitizen_connector-1.0.3/smartcitizen_connector/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-30 15:14:11.000000 smartcitizen_connector-1.0.3/smartcitizen_connector/models/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:17.031314 smartcitizen_connector-1.0.3/smartcitizen_connector/search/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 15:14:11.000000 smartcitizen_connector-1.0.3/smartcitizen_connector/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-04-30 15:14:11.000000 smartcitizen_connector-1.0.3/smartcitizen_connector/search/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:17.031314 smartcitizen_connector-1.0.3/smartcitizen_connector/sensor/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-30 15:14:11.000000 smartcitizen_connector-1.0.3/smartcitizen_connector/sensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-30 15:14:11.000000 smartcitizen_connector-1.0.3/smartcitizen_connector/sensor/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:17.035314 smartcitizen_connector-1.0.3/smartcitizen_connector/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-30 15:14:11.000000 smartcitizen_connector-1.0.3/smartcitizen_connector/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-04-30 15:14:11.000000 smartcitizen_connector-1.0.3/smartcitizen_connector/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:14:17.035314 smartcitizen_connector-1.0.3/smartcitizen_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-30 15:14:17.000000 smartcitizen_connector-1.0.3/smartcitizen_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-30 15:14:17.000000 smartcitizen_connector-1.0.3/smartcitizen_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:14:17.000000 smartcitizen_connector-1.0.3/smartcitizen_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:14:17.000000 smartcitizen_connector-1.0.3/smartcitizen_connector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-30 15:14:17.000000 smartcitizen_connector-1.0.3/smartcitizen_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-30 15:14:17.000000 smartcitizen_connector-1.0.3/smartcitizen_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:04.194266 smartcitizen_connector-1.0.4/smartcitizen_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/smartcitizen_connector/_config/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/_config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/smartcitizen_connector/device/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24439 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/device/device.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/smartcitizen_connector/measurement/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/measurement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/measurement/measurement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/smartcitizen_connector/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/models/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/smartcitizen_connector/search/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/search/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/smartcitizen_connector/sensor/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/sensor/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/smartcitizen_connector/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8620 2024-05-02 14:43:59.000000 smartcitizen_connector-1.0.4/smartcitizen_connector/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:44:04.198266 smartcitizen_connector-1.0.4/smartcitizen_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-02 14:44:04.000000 smartcitizen_connector-1.0.4/smartcitizen_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-02 14:44:04.000000 smartcitizen_connector-1.0.4/smartcitizen_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:44:04.000000 smartcitizen_connector-1.0.4/smartcitizen_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:44:04.000000 smartcitizen_connector-1.0.4/smartcitizen_connector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-02 14:44:04.000000 smartcitizen_connector-1.0.4/smartcitizen_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 14:44:04.000000 smartcitizen_connector-1.0.4/smartcitizen_connector.egg-info/top_level.txt
```

### Comparing `smartcitizen_connector-1.0.3/LICENSE` & `smartcitizen_connector-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.3/PKG-INFO` & `smartcitizen_connector-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartcitizen-connector
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python connector to download information collected in SmartCitizen API
 Home-page: https://github.com/fablabbcn/smartcitizen-connector
 Author: oscgonfer
 License: GNU General Public License v3
 Project-URL: Documentation, https://docs.smartcitizen.me/
 Project-URL: Source Code, https://github.com/fablabbcn/smartcitizen-connector
 Keywords: sensors,Smart Citizen
```

### Comparing `smartcitizen_connector-1.0.3/README.md` & `smartcitizen_connector-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.3/setup.py` & `smartcitizen_connector-1.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 PROJECT_URLS = {
     "Documentation": "https://docs.smartcitizen.me/",
     "Source Code": "https://github.com/fablabbcn/smartcitizen-connector",
 }
 
 setup(
     name="smartcitizen-connector",
-    version="1.0.3",
+    version="1.0.4",
     description="Python connector to download information collected in SmartCitizen API",
     author="oscgonfer",
     license="GNU General Public License v3",
     keywords=['sensors', 'Smart Citizen'],
     long_description = open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/fablabbcn/smartcitizen-connector",
```

### Comparing `smartcitizen_connector-1.0.3/smartcitizen_connector/_config/config.py` & `smartcitizen_connector-1.0.4/smartcitizen_connector/_config/config.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.3/smartcitizen_connector/device/device.py` & `smartcitizen_connector-1.0.4/smartcitizen_connector/device/device.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.3/smartcitizen_connector/measurement/measurement.py` & `smartcitizen_connector-1.0.4/smartcitizen_connector/measurement/measurement.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.3/smartcitizen_connector/models/models.py` & `smartcitizen_connector-1.0.4/smartcitizen_connector/models/models.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.3/smartcitizen_connector/search/search.py` & `smartcitizen_connector-1.0.4/smartcitizen_connector/search/search.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.3/smartcitizen_connector/sensor/sensor.py` & `smartcitizen_connector-1.0.4/smartcitizen_connector/sensor/sensor.py`

 * *Files identical despite different names*

### Comparing `smartcitizen_connector-1.0.3/smartcitizen_connector/tools/tools.py` & `smartcitizen_connector-1.0.4/smartcitizen_connector/tools/tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,26 +8,14 @@
 from requests import get
 import re
 import logging
 import sys
 
 tf = TimezoneFinder()
 
-# Convertion between SC and Pandas API rollups
-rollup_table = {
-    "y":   "years",
-    "M":   "months",
-    "w":   "weeks",
-    "d":   "days",
-    "h":   "hours",
-    "m":   "minutes",
-    "s":   "seconds",
-    "ms":  "milliseconds"
-}
-
 freq_2_rollup_lut = (
     ['A', 'y'],
     ['M', 'M'],
     ['W', 'w'],
     ['D', 'd'],
     ['H', 'h'],
     ['Min', 'm'],
@@ -61,14 +49,15 @@
     Helper function for converting a pandas freq into a rollup of SC API's
     ----------
         freq: str freq from pandas
     Returns
     -------
         rollup: str rollup from SC
     """
+    rollup_unit = None
     # Convert freq from pandas to SC API's
     for index, letter in enumerate(freq):
         try:
             aux = int(letter)
         except:
             index_first = index
             letter_first = letter
@@ -77,14 +66,16 @@
             break
 
     for item in freq_2_rollup_lut:
         if item[0] == freq_unit:
             rollup_unit = item[1]
             break
 
+    if rollup_unit is None:
+        return None
     rollup = rollup_value + rollup_unit
     return rollup
 
 def localise_date(date, timezone, tzaware=True):
     """
     Localises a date if it's tzinfo is None, otherwise converts it to it.
     If the timestamp is tz-aware, converts it as well
@@ -279,8 +270,13 @@
         else merge_dct[key]
         for key in merge_dct.keys()
     })
 
     return rtn_dct
 
 def dict_unpack(row, column, key):
-    return row[column][key]
+    try:
+        return row[column][key]
+    except:
+        pass
+
+    return ''
```

### Comparing `smartcitizen_connector-1.0.3/smartcitizen_connector.egg-info/PKG-INFO` & `smartcitizen_connector-1.0.4/smartcitizen_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartcitizen-connector
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python connector to download information collected in SmartCitizen API
 Home-page: https://github.com/fablabbcn/smartcitizen-connector
 Author: oscgonfer
 License: GNU General Public License v3
 Project-URL: Documentation, https://docs.smartcitizen.me/
 Project-URL: Source Code, https://github.com/fablabbcn/smartcitizen-connector
 Keywords: sensors,Smart Citizen
```

### Comparing `smartcitizen_connector-1.0.3/smartcitizen_connector.egg-info/SOURCES.txt` & `smartcitizen_connector-1.0.4/smartcitizen_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

