# Comparing `tmp/cave_utils-2.2.0b3.tar.gz` & `tmp/cave_utils-2.2.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cave_utils-2.2.0b3.tar", last modified: Thu Apr 18 18:34:26 2024, max compression
+gzip compressed data, was "cave_utils-2.2.0b4.tar", last modified: Wed May  1 20:32:33 2024, max compression
```

## Comparing `cave_utils-2.2.0b3.tar` & `cave_utils-2.2.0b4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-18 18:34:26.041891 cave_utils-2.2.0b3/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-2.2.0b3/LICENSE
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-2.2.0b3/NOTICE.md
--rw-r--r--   0 conmak    (1000) conmak    (1000)     3504 2024-04-18 18:34:26.041891 cave_utils-2.2.0b3/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     2946 2024-03-06 18:01:37.000000 cave_utils-2.2.0b3/README.md
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-18 18:34:26.037891 cave_utils-2.2.0b3/cave_utils/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      414 2024-03-04 18:45:40.000000 cave_utils-2.2.0b3/cave_utils/__init__.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-18 18:34:26.037891 cave_utils-2.2.0b3/cave_utils/api/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     8244 2023-11-30 18:55:27.000000 cave_utils-2.2.0b3/cave_utils/api/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     5002 2023-11-30 18:55:27.000000 cave_utils-2.2.0b3/cave_utils/api/appBar.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1063 2023-11-30 18:55:27.000000 cave_utils-2.2.0b3/cave_utils/api/extraKwargs.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     2210 2023-11-30 18:55:27.000000 cave_utils-2.2.0b3/cave_utils/api/globalOutputs.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    16980 2024-04-18 16:17:39.000000 cave_utils-2.2.0b3/cave_utils/api/groupedOutputs.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    11210 2023-11-30 18:55:27.000000 cave_utils-2.2.0b3/cave_utils/api/mapFeatures.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    30324 2024-02-26 14:04:23.000000 cave_utils-2.2.0b3/cave_utils/api/maps.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    12779 2024-04-18 18:22:52.000000 cave_utils-2.2.0b3/cave_utils/api/pages.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     7085 2024-01-31 16:20:08.000000 cave_utils-2.2.0b3/cave_utils/api/panes.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    14720 2024-01-31 16:20:08.000000 cave_utils-2.2.0b3/cave_utils/api/settings.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-18 18:34:26.037891 cave_utils-2.2.0b3/cave_utils/api_utils/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      311 2024-03-04 20:53:07.000000 cave_utils-2.2.0b3/cave_utils/api_utils/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    33939 2024-01-31 16:20:08.000000 cave_utils-2.2.0b3/cave_utils/api_utils/general.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      980 2023-11-30 18:55:27.000000 cave_utils-2.2.0b3/cave_utils/api_utils/validator.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    12799 2024-01-19 21:36:14.000000 cave_utils-2.2.0b3/cave_utils/api_utils/validator_utils.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1798 2023-10-16 13:43:50.000000 cave_utils-2.2.0b3/cave_utils/arguments.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-18 18:34:26.037891 cave_utils-2.2.0b3/cave_utils/builders/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      273 2024-03-06 18:02:20.000000 cave_utils-2.2.0b3/cave_utils/builders/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    15444 2024-03-14 15:24:47.000000 cave_utils-2.2.0b3/cave_utils/builders/groups.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     1529 2023-11-30 18:55:27.000000 cave_utils-2.2.0b3/cave_utils/log.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      257 2023-06-16 14:28:26.000000 cave_utils-2.2.0b3/cave_utils/socket.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-18 18:34:26.041891 cave_utils-2.2.0b3/cave_utils.egg-info/
--rw-r--r--   0 conmak    (1000) conmak    (1000)     3504 2024-04-18 18:34:26.000000 cave_utils-2.2.0b3/cave_utils.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      895 2024-04-18 18:34:26.000000 cave_utils-2.2.0b3/cave_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2024-04-18 18:34:26.000000 cave_utils-2.2.0b3/cave_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       34 2024-04-18 18:34:26.000000 cave_utils-2.2.0b3/cave_utils.egg-info/requires.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2024-04-18 18:34:26.000000 cave_utils-2.2.0b3/cave_utils.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      743 2024-04-18 18:31:36.000000 cave_utils-2.2.0b3/pyproject.toml
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      143 2024-04-18 18:34:26.041891 cave_utils-2.2.0b3/setup.cfg
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-04-18 18:34:26.041891 cave_utils-2.2.0b3/test/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      306 2023-11-30 18:55:27.000000 cave_utils-2.2.0b3/test/test_arguments.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     5107 2024-03-06 18:02:20.000000 cave_utils-2.2.0b3/test/test_builders_groups.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       40 2024-03-06 17:54:00.000000 cave_utils-2.2.0b3/test/test_import.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      233 2023-11-30 18:55:27.000000 cave_utils-2.2.0b3/test/test_log.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    75749 2024-01-31 16:20:08.000000 cave_utils-2.2.0b3/test/test_validator.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-01 20:32:33.781966 cave_utils-2.2.0b4/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    11357 2023-06-13 15:21:54.000000 cave_utils-2.2.0b4/LICENSE
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      631 2023-06-13 15:22:15.000000 cave_utils-2.2.0b4/NOTICE.md
+-rw-r--r--   0 conmak    (1000) conmak    (1000)     3504 2024-05-01 20:32:33.781966 cave_utils-2.2.0b4/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     2946 2024-03-06 18:01:37.000000 cave_utils-2.2.0b4/README.md
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-01 20:32:33.777966 cave_utils-2.2.0b4/cave_utils/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      414 2024-03-04 18:45:40.000000 cave_utils-2.2.0b4/cave_utils/__init__.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-01 20:32:33.781966 cave_utils-2.2.0b4/cave_utils/api/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     8444 2024-05-01 18:13:43.000000 cave_utils-2.2.0b4/cave_utils/api/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     4976 2024-05-01 14:13:40.000000 cave_utils-2.2.0b4/cave_utils/api/appBar.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1063 2023-11-30 18:55:27.000000 cave_utils-2.2.0b4/cave_utils/api/extraKwargs.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     2210 2024-05-01 20:11:17.000000 cave_utils-2.2.0b4/cave_utils/api/globalOutputs.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    16980 2024-04-18 16:17:39.000000 cave_utils-2.2.0b4/cave_utils/api/groupedOutputs.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    11802 2024-05-01 20:06:29.000000 cave_utils-2.2.0b4/cave_utils/api/mapFeatures.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    30324 2024-02-26 14:04:23.000000 cave_utils-2.2.0b4/cave_utils/api/maps.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    12779 2024-04-18 18:22:52.000000 cave_utils-2.2.0b4/cave_utils/api/pages.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     7085 2024-01-31 16:20:08.000000 cave_utils-2.2.0b4/cave_utils/api/panes.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    14930 2024-05-01 16:20:53.000000 cave_utils-2.2.0b4/cave_utils/api/settings.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-01 20:32:33.781966 cave_utils-2.2.0b4/cave_utils/api_utils/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      311 2024-03-04 20:53:07.000000 cave_utils-2.2.0b4/cave_utils/api_utils/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    35234 2024-05-01 14:01:50.000000 cave_utils-2.2.0b4/cave_utils/api_utils/general.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      990 2024-05-01 16:03:09.000000 cave_utils-2.2.0b4/cave_utils/api_utils/validator.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    16302 2024-05-01 20:22:37.000000 cave_utils-2.2.0b4/cave_utils/api_utils/validator_utils.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1798 2023-10-16 13:43:50.000000 cave_utils-2.2.0b4/cave_utils/arguments.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-01 20:32:33.781966 cave_utils-2.2.0b4/cave_utils/builders/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      273 2024-03-06 18:02:20.000000 cave_utils-2.2.0b4/cave_utils/builders/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    15444 2024-03-14 15:24:47.000000 cave_utils-2.2.0b4/cave_utils/builders/groups.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     1529 2023-11-30 18:55:27.000000 cave_utils-2.2.0b4/cave_utils/log.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      364 2024-05-01 20:14:50.000000 cave_utils-2.2.0b4/cave_utils/socket.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-01 20:32:33.781966 cave_utils-2.2.0b4/cave_utils.egg-info/
+-rw-r--r--   0 conmak    (1000) conmak    (1000)     3504 2024-05-01 20:32:33.000000 cave_utils-2.2.0b4/cave_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      895 2024-05-01 20:32:33.000000 cave_utils-2.2.0b4/cave_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2024-05-01 20:32:33.000000 cave_utils-2.2.0b4/cave_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       34 2024-05-01 20:32:33.000000 cave_utils-2.2.0b4/cave_utils.egg-info/requires.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       11 2024-05-01 20:32:33.000000 cave_utils-2.2.0b4/cave_utils.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      743 2024-05-01 20:29:46.000000 cave_utils-2.2.0b4/pyproject.toml
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      143 2024-05-01 20:32:33.781966 cave_utils-2.2.0b4/setup.cfg
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2024-05-01 20:32:33.781966 cave_utils-2.2.0b4/test/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      306 2023-11-30 18:55:27.000000 cave_utils-2.2.0b4/test/test_arguments.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     5107 2024-03-06 18:02:20.000000 cave_utils-2.2.0b4/test/test_builders_groups.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       40 2024-03-06 17:54:00.000000 cave_utils-2.2.0b4/test/test_import.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      233 2023-11-30 18:55:27.000000 cave_utils-2.2.0b4/test/test_log.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    75749 2024-01-31 16:20:08.000000 cave_utils-2.2.0b4/test/test_validator.py
```

### Comparing `cave_utils-2.2.0b3/LICENSE` & `cave_utils-2.2.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b3/NOTICE.md` & `cave_utils-2.2.0b4/NOTICE.md`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b3/PKG-INFO` & `cave_utils-2.2.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cave_utils
-Version: 2.2.0b3
+Version: 2.2.0b4
 Summary: Python wrapper for api use in the cave_app
 Author-email: Connor Makowski <conmak@mit.edu>
 Project-URL: Homepage, https://github.com/mit-cave/cave_utils
 Project-URL: Bug Tracker, https://github.com/mit-cave/cave_utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `cave_utils-2.2.0b3/README.md` & `cave_utils-2.2.0b4/README.md`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b3/cave_utils/api/__init__.py` & `cave_utils-2.2.0b4/cave_utils/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,17 @@
         settings(
             data=self.data.get("settings", {}),
             log=self.log,
             prepend_path=["settings"],
             root_data=self.data,
             **kwargs,
         )
+        # Special logic to add timeLength to kwargs
+        # This is used to validate timeValues across the app
+        kwargs["timeLength"] = pamda.path(["settings","time","timeLength"], self.data)
         # Validate panes
         panes_data = self.data.get("panes")
         pane_validPaneIds = []
         if panes_data is not None:
             panes(data=panes_data, log=self.log, prepend_path=["panes"], **kwargs)
             pane_validPaneIds = list(panes_data.get("data", {}).keys())
         # Validate mapFeatures
```

### Comparing `cave_utils-2.2.0b3/cave_utils/api/appBar.py` & `cave_utils-2.2.0b4/cave_utils/api/appBar.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,17 +48,16 @@
     @staticmethod
     def spec(
         icon: str,
         type: str,
         bar: str,
         variant: [str, None] = None,
         color: [str, None] = None,
-        order: [dict, None] = None,
         apiCommand: [str, None] = None,
-        apiCommandKeys: [list, None] = None,
+        apiCommandKeys: [list[str], None] = None,
         **kwargs,
     ):
         """
         Arguments:
 
         * **`icon`**: `[str]` &rarr; An icon to display in the center of the action element.
             * **Note**: It must be a valid icon name from the [react-icons][] bundle, preceded by the abbreviated name of the icon library source.
@@ -84,15 +83,15 @@
                 * Otherwise:
                     * `None`
         * **`color`**: `[str]` = `<system-default-value>` &rarr;
             * The color of the button. If omitted, the default value is set by the system.
             * **Note**: It must be a valid RGBA string.
             * **Example**: `"rgba(255, 255, 255, 1)"`.
         * **`apiCommand`**: `[str]` = `None` &rarr; The name of the [API command][] to trigger.
-        * **`apiCommandKeys`**: `[list]` = `None` &rarr;
+        * **`apiCommandKeys`**: `[list[str]]` = `None` &rarr;
             * The root API keys to pass to your `execute_command` function if an
             `apiCommand` is provided. If omitted, all API keys are
             passed to `execute_command`.
 
         [page]: pages.html
         [pane]: panes.html
         [modal pane]: panes.html
```

### Comparing `cave_utils-2.2.0b3/cave_utils/api/extraKwargs.py` & `cave_utils-2.2.0b4/cave_utils/api/extraKwargs.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b3/cave_utils/api/globalOutputs.py` & `cave_utils-2.2.0b4/cave_utils/api/globalOutputs.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b3/cave_utils/api/groupedOutputs.py` & `cave_utils-2.2.0b4/cave_utils/api/groupedOutputs.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b3/cave_utils/api/mapFeatures.py` & `cave_utils-2.2.0b4/cave_utils/api/mapFeatures.py`

 * *Files 5% similar despite different names*

```diff
@@ -151,16 +151,18 @@
         mapFeatures_data_star_data_location(
             data=location_data,
             log=self.log,
             prepend_path=["location"],
             **kwargs,
         )
         # Validate that all lengths are the same
-        lengths = [len(v) for k, v in location_data.items() if k not in ["order", "timeValues"]] + [
-            len(v) for k, v in valueLists_data.items() if k not in ["order", "timeValues"]
+        lengths = [
+            len(v) for k, v in location_data.items() if k not in ['timeValues', 'order']
+        ] + [
+            len(v) for k, v in valueLists_data.items() if k not in ['timeValues', 'order']
         ]
         if len(set(lengths)) > 1:
             self.__error__(msg=f"location and valueLists keys must have the same length.", path=[])
 
 
 @type_enforced.Enforcer
 class mapFeatures_data_star_data_location(ApiValidator):
@@ -181,40 +183,47 @@
             "accepted_values": {},
         }
 
     def __extend_spec__(self, **kwargs):
         layer_type = kwargs.get("layer_type")
         layer_geoJson = kwargs.get("layer_geoJson")
         passed_keys = list(self.data.keys())
-        # TODO Figure out way to handle timeValues and order
-        optional_keys = ["timeValues", "order"]
-        if layer_type == "geo" or (layer_type == "arc" and layer_geoJson):
+        optional_keys = []
+        if layer_type == "geo":
             required_keys = ["geoJsonValue"]
         elif layer_type == "arc":
-            if "path" in passed_keys:
+            if layer_geoJson is not None:
+                required_keys = ["geoJsonValue"]
+                optional_keys += ["path", "startLatitude", "startLongitude", "endLatitude", "endLongitude","startAltitude", "endAltitude"]
+            elif "path" in passed_keys:
                 required_keys = ["path"]
+                optional_keys += ["startLatitude", "startLongitude", "endLatitude", "endLongitude", "geoJsonValue","startAltitude", "endAltitude"]
             else:
                 required_keys = ["startLatitude", "startLongitude", "endLatitude", "endLongitude"]
-                optional_keys += ["startAltitude", "endAltitude"]
+                optional_keys += ["startAltitude", "endAltitude", "geoJsonValue", "path"]
         else:
             required_keys = ["latitude", "longitude"]
             optional_keys += ["altitude"]
         missing_keys = pamda.difference(required_keys, list(self.data.keys()))
         if len(missing_keys) > 0:
             self.__error__(msg=f"Missing required keys: {missing_keys}", path=[])
             return
         for key, value_list in self.data.items():
             if key not in required_keys + optional_keys:
                 self.__error__(
                     msg=f"`{key}` is not a valid key for location for layer type `{layer_type}`",
                     path=[],
                 )
                 continue
-            if key in ["timeValues", "order"]:
-                continue
+            if key == "geoJsonValue":
+                if len(value_list)!=len(set(value_list)):
+                    self.__warn__(
+                        msg=f"`geoJsonValue` should be a list of unique values. Otherwise, the corresponding map feature may not render correctly.",
+                        path=[key],
+                    )
             if not isinstance(value_list, list):
                 self.__error__(
                     msg=f"`{key}` must be a list but got {type(value_list)} instead.", path=[key]
                 )
                 continue
             latitudes = None
             longitudes = None
@@ -236,15 +245,15 @@
                     latitudes = [y[1] for x in value_list for y in x]
                     try:
                         altitudes = [y[2] for x in value_list for y in x]
                     except:
                         altitudes = None
                 except:
                     self.__error__(
-                        msg=f"`path` must be a list of lists of lists of length 2 or 3. EG: `[[[0,0],[1,1]],[[2,2],[3,3],[4,4],[5,5]]]`",
+                        msg=f"`path` must be a list of lists of lists of length 2 [long,lat] or 3 [long,lat,alt]. EG: `[[[0,0],[1,1]],[[2,2],[3,3],[4,4],[5,5]]]`",
                         path=[key],
                     )
                     continue
             else:
                 acceptable_types = (str,)
             if not self.__check_type_list__(
                 data=value_list, types=acceptable_types, prepend_path=[key]
```

### Comparing `cave_utils-2.2.0b3/cave_utils/api/maps.py` & `cave_utils-2.2.0b4/cave_utils/api/maps.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b3/cave_utils/api/pages.py` & `cave_utils-2.2.0b4/cave_utils/api/pages.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b3/cave_utils/api/panes.py` & `cave_utils-2.2.0b4/cave_utils/api/panes.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b3/cave_utils/api/settings.py` & `cave_utils-2.2.0b4/cave_utils/api/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,7 +287,12 @@
         Arguments:
 
         * **`timeLength`**: `[int]` &rarr; The amount of time values to display.
         * **`timeUnits`**: `[str]` &rarr; The units of time to display.
             * **Example**: `"Decade"`.
         """
         return {"kwargs": kwargs, "accepted_values": {}}
+    
+    def __extend_spec__(self, **kwargs):
+        timeLength = self.data.get("timeLength")
+        if timeLength < 1:
+            self.__error__(f"Time length must be greater than 0.", path=["timeLength"])
```

### Comparing `cave_utils-2.2.0b3/cave_utils/api_utils/general.py` & `cave_utils-2.2.0b4/cave_utils/api_utils/general.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 """
 General API Spec items that are found in multiple places. This is not a key that should be passed as part of your `session_data`.
 """
 from pamda import pamda
 import type_enforced
 from cave_utils.api_utils.validator_utils import ApiValidator, CustomKeyValidator
+from typing import Literal
 
 
 @type_enforced.Enforcer
 class props(ApiValidator):
     @staticmethod
     def spec(
         name: str,
         type: str,
         help: [str, None] = None,
         variant: [str, None] = None,
         display: [bool, None] = None,
         enabled: [bool, None] = None,
         apiCommand: [str, None] = None,
-        apiCommandKeys: [list, None] = None,
+        apiCommandKeys: [list[str], None] = None,
         options: [dict, None] = None,
         placeholder: [str, None] = None,
         maxValue: [float, int, None] = None,
         minValue: [float, int, None] = None,
         maxRows: [int, None] = None,
         minRows: [int, None] = None,
         rows: [int, None] = None,
         notation: [str, None] = None,
         precision: [int, None] = None,
         notationDisplay: [str, None] = None,
         unit: [str, None] = None,
-        views: [list, None] = None,
+        views: [list[str], None] = None,
         legendNotation: [str, None] = None,
         legendPrecision: [int, None] = None,
         legendNotationDisplay: [str, None] = None,
         legendMinLabel: [str, None] = None,
         legendMaxLabel: [str, None] = None,
         icon: [str, None] = None,
         trailingZeros: [bool, None] = None,
@@ -95,15 +96,15 @@
                     * `"picture"`: Show a PNG or JPG image
                     * `"video"`: Display a YouTube, Vimeo, or Dailymotion video clip
         * **`enabled`**: `[bool]` = `True` &rarr; Whether or not the prop will be enabled.
             * **Note**: This attribute is applicable to all props except `"head"` props.
         * **`apiCommand`**: `[str]` = `None` &rarr; The name of the API command to trigger.
             * **Note**: If `None`, no `apiCommand` is triggered.
             * **Note**: This attribute is applicable to all props except `"head"` props.
-        * **`apiCommandKeys`**: `[list]` = `None` &rarr;
+        * **`apiCommandKeys`**: `[list[str]]` = `None` &rarr;
             * The root API keys to pass to your `execute_command` function if an `apiCommand` is provided.
             * **Note**: If `None`, all API keys are passed to your `execute_command`.
             * **Note**: This attribute is applicable to all props except `"head"` props.
         * **`icon`**: `[str]` = `None` &rarr; The icon to use for the prop.
             * **Notes**:
                 * It must be a valid icon name from the [react-icons][] bundle, preceded by the abbreviated name of the icon library source.
                 * This attribute is applicable exclusively to `"head"` props.
@@ -122,23 +123,36 @@
             * **Note**: This attribute is applicable exclusively to `"text"` props.
         * **`minRows`**: `[int]` = `None` &rarr;
             * The minimum number of rows to show for a `"textarea"` variant.
             * **Note**: This attribute is applicable exclusively to `"text"` props.
         * **`rows`**: `[int]` = `None` &rarr;
             * The fixed number of rows to show for a `"textarea"` variant.
             * **Note**: This attribute is applicable exclusively to `"text"` props.
-        * **`views`**: `[list]` = `["year", "day", "hours", "minutes"]` &rarr;
+        * **`views`**: `[list[str]]` &rarr;
             * The available time units for the represented date and/or time.
+            * **Default Value**:
+                * When **`variant`** == `"date"`: `["year", "day"]`
+                * When **`variant`** == `"time"`: `["hours", "minutes"]`
+                * When **`variant`** == `"datetime"`: `["year", "day", "hours", "minutes"]`
             * **Accepted Values**:
-                * `"year"`: The year view
-                * `"month"`: The month view
-                * `"day"`: The day view
-                * `"hours"`: The hours view
-                * `"minutes"`: The minutes view
-                * `"seconds"`: The seconds view
+                * When **`variant`** == `"date"`:
+                    * `"year"`: The year view
+                    * `"month"`: The month view
+                    * `"day"`: The day view
+                * When **`variant`** == `"time"`:
+                    * `"hours"`: The hours view
+                    * `"minutes"`: The minutes view
+                    * `"seconds"`: The seconds view
+                * When **`variant`** == `"datetime"`:
+                    * `"year"`: The year view
+                    * `"month"`: The month view
+                    * `"day"`: The day view
+                    * `"hours"`: The hours view
+                    * `"minutes"`: The minutes view
+                    * `"seconds"`: The seconds view
             * **Notes**:
                 * The views will be presented in the order specified in the `views` array.
                 * This attribute is applicable exclusively to `"date"` props.
         * **`locale`**: `[str]` = `None` &rarr;
             * Format numeric values based on language and regional conventions.
             * **Notes**:
                 * If left unspecified (i.e., `None`), it will default to `settings.defaults.locale`.
@@ -169,33 +183,37 @@
                 * `"after"`: The `unit` appears after the value.
                 * `"afterWithSpace"`: The `unit` appears after the value, separated by a space.
                 * `"before"`: The `unit` appears before the value.
                 * `"beforeWithSpace"`: The unit is placed before the value, with a space in between.
             * **Notes**:
                 * If left unspecified (i.e., `None`), it will default to `settings.defaults.unitPlacement`.
                 * This attribute is applicable exclusively to `"num"` props.
-        * **`notation`**: `[int]` = `"standard"` &rarr; The formatting style of a numeric value.
+        * **`notation`**: `[str]` = `"standard"` &rarr; The formatting style of a numeric value.
             * **Accepted Values**:
                 * `"standard"`: Plain number formatting
                 * `"compact"`: Resembles the [metric prefix][] system
                 * `"scientific"`: [Scientific notation][]
                 * `"engineering"`: [Engineering notation][]
             * **Notes**:
                 * If left unspecified (i.e., `None`), it will default to `settings.defaults.notation`.
                 * This attribute is applicable exclusively to `"num"` props.
         * **`notationDisplay`**: `[str]` = `"e+"` | `"short"` &rarr; Further customize the formatting within the selected `notation`.
             * **Accepted Values**:
-                * `"short"`: Add symbols `K`, `M`, `B`, and `T` (in `"en-US"`) to denote thousands, millions, billions, and trillions, respectively.
-                * `"long"`: Present numeric values with the informal suffix words `thousand`, `million`, `billion`, and `trillion` (in `"en-US"`).
-                * `"e"`: Exponent symbol in lowercase as per the chosen `locale` identifier
-                * `"e+"`: Similar to `"e"`, but with a plus sign for positive exponents.
-                * `"E"`: Exponent symbol in uppercase as per the chosen `locale` identifier
-                * `"E+"`: Similar to `"E"`, but with a plus sign for positive exponents.
-                * `"x10^"`: Formal scientific notation representation
-                * `"x10^+"`: Similar to `"x10^"`, with a plus sign for positive exponents.
+                * When **`notation`** == `"compact"`:
+                    * `"short"`: Add symbols `K`, `M`, `B`, and `T` (in `"en-US"`) to denote thousands, millions, billions, and trillions, respectively.
+                    * `"long"`: Present numeric values with the informal suffix words `thousand`, `million`, `billion`, and `trillion` (in `"en-US"`).
+                * When **`notation`** == `"scientific"` or `"engineering"`:
+                    * `"e"`: Exponent symbol in lowercase as per the chosen `locale` identifier
+                    * `"e+"`: Similar to `"e"`, but with a plus sign for positive exponents.
+                    * `"E"`: Exponent symbol in uppercase as per the chosen `locale` identifier
+                    * `"E+"`: Similar to `"E"`, but with a plus sign for positive exponents.
+                    * `"x10^"`: Formal scientific notation representation
+                    * `"x10^+"`: Similar to `"x10^"`, with a plus sign for positive exponents.
+                * When **`notation`** == `"standard"`:
+                    * No `notationDisplay` option is allowed for a `"standard"` notation
             * **Notes**:
                 * No `notationDisplay` option is provided for a `"standard"` notation
                 * The options `"short"` and `"long"` are only provided for the `"compact"` notation
                 * The options `"e"`, `"e+"`, `"E"`, `"E+"`, `"x10^"`, and `"x10^+"` are provided for the `"scientific"` and `"engineering"` notations
                 * If left unspecified (i.e., `None`), it will default to `settings.defaults.notationDisplay`.
                 * This attribute is applicable exclusively to `"num"` props.
         * **`legendPrecision`**: `[int]` = `None` &rarr;
@@ -300,28 +318,38 @@
             optional_fields += ["views"]
         missing_required = pamda.difference(required_fields, list(passed_values.keys()))
         if len(missing_required) > 0:
             raise Exception(f"Missing required fields: {str(missing_required)}")
         for k, v in passed_values.items():
             if k not in required_fields + optional_fields:
                 kwargs[k] = v
+        notationDisplay_options_dict = {
+            'compact': ['short', 'long'],
+            'scientific': ['e', 'e+', 'E', 'E+', 'x10^', 'x10^+'],
+            'engineering': ['e', 'e+', 'E', 'E+', 'x10^', 'x10^+'],
+            'standard': []
+        }
+        notation = passed_values.get('notation', 'standard')
+        legendNotation = passed_values.get('legendNotation', 'standard')
+        view_options_dict = {
+            "date": ["year", "month", "day"],
+            "time": ["hours", "minutes", "seconds"],
+            "datetime": ["year", "month", "day", "hours", "minutes", "seconds"],
+        }
+        variant = passed_values.get("variant", None)
         return {
             "kwargs": kwargs,
             "accepted_values": {
                 "type": ["head", "num", "toggle", "button", "text", "selector", "date", "media"],
-                "views": ["year", "month", "day", "hours", "minutes", "seconds"],
+                "views": view_options_dict.get(variant, []),
                 "unitPlacement": ["after", "afterWithSpace", "before", "beforeWithSpace"],
-                # TODO: Validate
-                # compact: allowed notation displays -> "short", "long"
-                # scientific|engineering: allowed notation displays -> "e", "e+", "E", "E+", "x10^", "x10^+"
-                # standard: allowed notation displays -> None
                 "notation": ["compact", "precision", "scientific", "engineering"],
-                "notationDisplay": ["short", "long", "e", "e+", "E", "E+", "x10^", "x10^+"],
+                "notationDisplay": notationDisplay_options_dict.get(notation, []),
                 "legendNotation": ["compact", "precision", "scientific", "engineering"],
-                "legendNotationDisplay": ["short", "long", "e", "e+", "E", "E+", "x10^", "x10^+"],
+                "legendNotationDisplay": notationDisplay_options_dict.get(legendNotation, []),
                 "variant": {
                     "head": ["column", "row", "icon", "iconRow"],
                     "text": ["textarea"],
                     "num": ["field", "slider", "icon", "iconCompact"],
                     "selector": [
                         "dropdown",
                         "checkbox",
@@ -345,23 +373,23 @@
                 log=self.log,
                 prepend_path=["options"],
                 validator=props_options,
                 variant=self.data.get("variant"),
                 **kwargs,
             )
 
-
+@type_enforced.Enforcer
 class props_options(ApiValidator):
     @staticmethod
-    def spec(name: str, path: [list, None] = None, **kwargs):
+    def spec(name: str, path: [list[str], None] = None, **kwargs):
         """
         Arguments:
 
         * **`name`**: `[str]` &rarr; The name of the option.
-        * **`path`**: `[list]` = `None` &rarr; The path to an option.
+        * **`path`**: `[list[str]]` = `None` &rarr; The path to an option.
             * **Notes**:
                 * If `None`, the option will not be selectable
                 * This attribute is applicable exclusively to `"nested"` props
         """
         variant = kwargs.get("variant")
         kwargs = {k: v for k, v in kwargs.items() if k != "variant"}
         if variant == "nested":
@@ -375,17 +403,14 @@
     def __extend_spec__(self, **kwargs):
         if kwargs.get("variant") == "nested":
             if not isinstance(self.data.get("path"), list):
                 self.__error__(
                     msg="`path` must be specified and a list of strings for nested options"
                 )
                 return
-            self.__check_type_list__(
-                data=self.data.get("path", []), types=(str,), prepend_path=["path"]
-            )
 
 
 @type_enforced.Enforcer
 class layout(ApiValidator):
     @staticmethod
     def spec(
         type: str,
```

### Comparing `cave_utils-2.2.0b3/cave_utils/api_utils/validator.py` & `cave_utils-2.2.0b4/cave_utils/api_utils/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from cave_utils.api_utils.validator_utils import LogObject
 from cave_utils.api import Root
 import type_enforced
 
 
 @type_enforced.Enforcer
 class Validator:
-    def __init__(self, session_data, ignore_keys: list = list(), **kwargs):
+    def __init__(self, session_data, ignore_keys: list[str] = list(), **kwargs):
         """
         Util to validate your session_data against the API spec.
 
         Arguments:
 
         * **`session_data`**: `[dict]` &rarr; The data to validate.
             * **Note**: This should be the data you are sending to the server.
-        * **`ignore_keys`**: `[list]` = `None` &rarr; Keys to ignore when validating.
+        * **`ignore_keys`**: `[list[str]]` = `None` &rarr; Keys to ignore when validating.
             * **Note**: Any keys specified here will be not be validated if encountered in the data at any level.
         """
         self.session_data = session_data
         self.log = LogObject()
         Root(data=self.session_data, log=self.log, prepend_path=[], ignore_keys=set(ignore_keys))
```

### Comparing `cave_utils-2.2.0b3/cave_utils/api_utils/validator_utils.py` & `cave_utils-2.2.0b4/cave_utils/api_utils/validator_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,31 +20,31 @@
         This should be overridden by any non utility child class.
         """
         return {
             "kwargs": {},
             "accepted_values": {},
         }
 
-    def __validate__(self, data, log: LogObject, prepend_path: list = list(), **kwargs):
+    def __validate__(self, data:dict, log: LogObject, prepend_path: list[str] = list(), **kwargs):
         """
         Run the API validation process for the passed data.
         """
-        self.data = data
+        # Make a copy of the data to avoid modifying the original
+        self.data = {**data}
         self.ignore_keys = kwargs.get("ignore_keys", set())
         self.log = LogHelper(log=log, prepend_path=prepend_path)
         try:
+            self.__genericKeyValidation__(**kwargs)
             spec_output = self.spec(**self.data)
             extra_kwargs = spec_output.get("kwargs", {})
-            # TODO: Find way to custom check timeValues and order
-            extra_kwargs.pop("order", None)
-            extra_kwargs.pop("timeValues", None)
             if extra_kwargs != {}:
                 self.__warn__(
                     msg=f"Unknown Fields: {str(list(extra_kwargs.keys()))}",
-                )
+                )            
+
         except Exception as e:
             self.__error__(
                 msg=f"Error validating spec: {e}",
             )
             # Must return since an invalid spec will bug out other validation checks
             return
         for field, accepted_values in spec_output.get("accepted_values", {}).items():
@@ -71,29 +71,103 @@
                 msg=f"Extended spec validations failed (likely due to another error with your API data). Error: {e}",
             )
 
     # Placeholder method for additional validations
     def __extend_spec__(self, **kwargs):
         pass
 
+    # Additional core validations for generic terms like `order` and `timeValues`
+    def __genericKeyValidation__(self, **kwargs):
+        # Remove `timeValues` out prior to each level validation 
+        data_timeValues = self.data.pop("timeValues", None)
+        # Remove `order` out prior to each level validation
+        data_order = self.data.pop("order", None)
+        if data_timeValues is not None:
+            timeLength = kwargs.get("timeLength")
+            if timeLength is None:
+                self.__error__(
+                    path=['timeValues'],
+                    msg="`settings.time.timeLength` must be specified to validate `timeValues`",
+                )
+            else:
+                self.__timeValues_validation__(timeValues=data_timeValues, timeLength=timeLength)
+        if data_order is not None:
+            self.__order_validation__(order=data_order)
+            
+    @type_enforced.Enforcer
+    def __order_validation__(self, order:dict[list[str,int]]):
+        """
+        Check that the ordering options are valid
+        """
+        orderable_data_keys = {key: list(value.keys()) for key, value in self.data.items() if isinstance(value, dict)}
+        if self.__check_subset_valid__(
+            subset=list(order.keys()),
+            valid_values=list(orderable_data_keys.keys()),
+            prepend_path=["order"],
+        ):
+            for order_key, order_list in order.items():
+                self.__check_subset_valid__(
+                    subset=order_list,
+                    valid_values=orderable_data_keys[order_key],
+                    prepend_path=["order", order_key],
+                )
+    
+    @type_enforced.Enforcer
+    def __timeValues_validation__(self, timeValues: [dict[dict],list[dict]], timeLength:int):
+        if len(timeValues) == 0:
+            return
+        if isinstance(timeValues, list):
+            if len(timeValues) != timeLength:
+                self.__error__(
+                    path=['timeValues'],
+                    msg=f"The length of `timeValues` (as a list) must be equal to `settings.time.timeLength` ({timeLength})",
+                )
+                return
+        if isinstance(timeValues, dict):
+            keys = list(timeValues.keys())
+            if not all(isinstance(key, int) for key in keys):
+                self.__error__(
+                    path=['timeValues'],
+                    msg="`timeValues` (as a dict) keys must be integers",
+                )
+                return
+            if not all(key >= 0 and key<timeLength for key in keys):
+                self.__error__(
+                    path=['timeValues'],
+                    msg=f"`timeValues` (as a dict) keys must be integers between 0 and {timeLength-1} inclusive (1 minus the value at `settings.time.timeLength`)",
+                )
+                return
+            timeValues = list(timeValues.values())
+        timeValueTypes = {k:type(v) for k,v in timeValues[0].items()}
+        for timeValue in timeValues:
+            if timeValueTypes != {k:type(v) for k,v in timeValue.items()}:
+                self.__error__(
+                    path=['timeValues'],
+                    msg="All timeValues must have the same keys and each key must have the same type",
+                )
+                return
+        # Update the data with the first timeValue prioritizing original data
+        # over the first timeValue
+        self.data = {**timeValues[0], **self.data}
+
     # Error and Warning Helpers
-    def __error__(self, msg: str, path: list = list()):
+    def __error__(self, msg: str, path: list[str] = list()):
         """
         Raise an error for the log the log
         """
         self.log.add(path=path, msg=msg)
 
-    def __warn__(self, msg: str, path: list = list()):
+    def __warn__(self, msg: str, path: list[str] = list()):
         """
         Raise a warning for the log the log
         """
         self.log.add(path=path, msg=msg, level="warning")
 
     # Useful Validator Checks
-    def __check_rgba_string_valid__(self, rgba_string: str, prepend_path: list = list()):
+    def __check_rgba_string_valid__(self, rgba_string: str, prepend_path: list[str] = list()):
         """
         Validate an rgba string and if an issue is present, log an error
         """
         msg = "Invalid RGBA string. Must be in the format 'rgba(0, 0, 0, 0)' where each value is an integer between 0 and 255."
         try:
             if "rgba(" != rgba_string[:5]:
                 self.__error__(path=prepend_path, msg=msg)
@@ -108,29 +182,29 @@
                     return
                 if int(rgba) < 0 or int(rgba) > 255:
                     self.__error__(path=prepend_path, msg=msg)
                     return
         except:
             self.__error__(path=prepend_path, msg=msg)
 
-    def __check_pixel_string_valid__(self, pixel_string: str, prepend_path: list = list()):
+    def __check_pixel_string_valid__(self, pixel_string: str, prepend_path: list[str] = list()):
         """
         Validate a pixel string and if an issue is present, log an error
         """
         msg = "Invalid pixel string. Must be in the format '5px' where the value portion is a whole number."
         try:
             if "px" != pixel_string[-2:]:
                 self.__error__(path=prepend_path, msg=msg)
                 return
             if int(pixel_string[:-2]) < 0:
                 self.__error__(path=prepend_path, msg=msg)
         except:
             self.__error__(path=prepend_path, msg=msg)
 
-    def __check_url_valid__(self, url: str, prepend_path: list = list()):
+    def __check_url_valid__(self, url: str, prepend_path: list[str] = list()):
         """
         Validate a url and if an issue is present, log an error.
         """
         # Use Django regex for URL validation
         # See https://stackoverflow.com/a/7160778/12014156
         regex = re.compile(
             r"^(?:http|ftp)s?://"  # http:// or https://
@@ -142,15 +216,15 @@
             re.IGNORECASE,
         )
         if re.match(regex, url) is None:
             self.__error__(path=prepend_path, msg="Invalid url")
             return False
         return True
 
-    def __check_date_valid__(self, input: str, date_variant: str, prepend_path: list = list()):
+    def __check_date_valid__(self, input: str, date_variant: str, prepend_path: list[str] = list()):
         """
         Validate a date string and if an issue is present, log an error.
         """
         if date_variant == "date":
             try:
                 datetime.datetime.strptime(input, "%Y-%m-%d")
             except ValueError:
@@ -185,15 +259,15 @@
             return False
         return True
 
     def __check_subset_valid__(
         self,
         subset: list,
         valid_values: list,
-        prepend_path: list = list(),
+        prepend_path: list[str] = list(),
         valid_values_count: int = 6,
     ):
         """
         Validate a subset of values is in a set of valid values and if an issue is present, log an error
 
         Returns True if the subset check passed and False otherwise
         """
@@ -207,15 +281,15 @@
             self.__error__(
                 path=prepend_path,
                 msg=f"Invalid value(s) selected: {str(invalid_values)}. Accepted Values are {valid_values}",
             )
             return False
         return True
 
-    def __check_coord_path_valid__(self, coord_path: list, prepend_path: list = list()):
+    def __check_coord_path_valid__(self, coord_path: list[list[int,float]], prepend_path: list[str] = list()):
         """
         Validate a coordinate path and if an issue is present, log an error
         """
         try:
             if len(coord_path) < 2:
                 self.__error__(path=prepend_path, msg="Invalid coordinate path")
                 return
@@ -253,15 +327,15 @@
                 self.__error__(
                     path=prepend_path,
                     msg=f"Invalid list item type at index: {idx} with type: {type(item)}. Expected one of {types}",
                 )
                 return False
         return True
 
-    def __check_type_dict__(self, data: dict, types: tuple, prepend_path: list = list()):
+    def __check_type_dict__(self, data: dict, types: tuple, prepend_path: list[str] = list()):
         """
         Validate a dict only contains certain object types for values and if an issue is present, log an error
 
         Returns True if the type check passed and False otherwise
         """
         if not isinstance(types, tuple):
             types = (types,)
@@ -270,15 +344,15 @@
                 self.__error__(
                     path=prepend_path,
                     msg=f"Invalid dict item type at key: {key} with type: {type(value)}. Expected one of {types}",
                 )
                 return False
         return True
 
-    def __check_type__(self, value, check_type, prepend_path: list = list()):
+    def __check_type__(self, value, check_type, prepend_path: list[str] = list()):
         """
         Validate a value is a certain type and if an issue is present, log an error
 
         Returns True if the type check passed and False otherwise
 
         Required Arguments:
```

### Comparing `cave_utils-2.2.0b3/cave_utils/arguments.py` & `cave_utils-2.2.0b4/cave_utils/arguments.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b3/cave_utils/builders/groups.py` & `cave_utils-2.2.0b4/cave_utils/builders/groups.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b3/cave_utils/log.py` & `cave_utils-2.2.0b4/cave_utils/log.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b3/cave_utils.egg-info/PKG-INFO` & `cave_utils-2.2.0b4/cave_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cave_utils
-Version: 2.2.0b3
+Version: 2.2.0b4
 Summary: Python wrapper for api use in the cave_app
 Author-email: Connor Makowski <conmak@mit.edu>
 Project-URL: Homepage, https://github.com/mit-cave/cave_utils
 Project-URL: Bug Tracker, https://github.com/mit-cave/cave_utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `cave_utils-2.2.0b3/cave_utils.egg-info/SOURCES.txt` & `cave_utils-2.2.0b4/cave_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b3/pyproject.toml` & `cave_utils-2.2.0b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cave_utils"
-version = "2.2.0b3"
+version = "2.2.0b4"
 description = "Python wrapper for api use in the cave_app"
 authors = [
     {name="Connor Makowski", email="conmak@mit.edu"}
 ]
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `cave_utils-2.2.0b3/test/test_builders_groups.py` & `cave_utils-2.2.0b4/test/test_builders_groups.py`

 * *Files identical despite different names*

### Comparing `cave_utils-2.2.0b3/test/test_validator.py` & `cave_utils-2.2.0b4/test/test_validator.py`

 * *Files identical despite different names*

