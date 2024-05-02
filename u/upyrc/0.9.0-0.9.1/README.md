# Comparing `tmp/upyrc-0.9.0.tar.gz` & `tmp/upyrc-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upyrc-0.9.0.tar", last modified: Wed Apr 12 15:38:19 2023, max compression
+gzip compressed data, was "upyrc-0.9.1.tar", last modified: Thu Apr 27 11:14:16 2023, max compression
```

## Comparing `upyrc-0.9.0.tar` & `upyrc-0.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-12 15:38:19.593902 upyrc-0.9.0/
--rw-rw-rw-   0        0        0    35823 2023-01-24 20:50:34.000000 upyrc-0.9.0/LICENSE
--rw-rw-rw-   0        0        0     4049 2023-04-12 15:38:19.591868 upyrc-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     3708 2023-04-11 16:05:11.000000 upyrc-0.9.0/README.md
--rw-rw-rw-   0        0        0      536 2023-04-12 15:37:56.000000 upyrc-0.9.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-12 15:38:19.593902 upyrc-0.9.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-12 15:38:19.578865 upyrc-0.9.0/src/
-drwxrwxrwx   0        0        0        0 2023-04-12 15:38:19.583865 upyrc-0.9.0/src/upyrc/
--rw-rw-rw-   0        0        0       21 2023-04-12 15:37:54.000000 upyrc-0.9.0/src/upyrc/__init__.py
--rw-rw-rw-   0        0        0    41928 2023-04-11 16:07:56.000000 upyrc-0.9.0/src/upyrc/upyrc.py
-drwxrwxrwx   0        0        0        0 2023-04-12 15:38:19.589897 upyrc-0.9.0/src/upyrc.egg-info/
--rw-rw-rw-   0        0        0     4049 2023-04-12 15:38:19.000000 upyrc-0.9.0/src/upyrc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-04-12 15:38:19.000000 upyrc-0.9.0/src/upyrc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-12 15:38:19.000000 upyrc-0.9.0/src/upyrc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-12 15:38:19.000000 upyrc-0.9.0/src/upyrc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-12 15:38:19.000000 upyrc-0.9.0/src/upyrc.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-12 15:38:19.590882 upyrc-0.9.0/tests/
--rw-rw-rw-   0        0        0     8046 2023-04-11 16:04:50.000000 upyrc-0.9.0/tests/test_uremote.py
+drwxrwxrwx   0        0        0        0 2023-04-27 11:14:16.703972 upyrc-0.9.1/
+-rw-rw-rw-   0        0        0    35823 2023-01-24 20:50:34.000000 upyrc-0.9.1/LICENSE
+-rw-rw-rw-   0        0        0     4118 2023-04-27 11:14:16.702972 upyrc-0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3777 2023-04-12 15:56:00.000000 upyrc-0.9.1/README.md
+-rw-rw-rw-   0        0        0      536 2023-04-27 07:51:15.000000 upyrc-0.9.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-27 11:14:16.704973 upyrc-0.9.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-27 11:14:16.670045 upyrc-0.9.1/src/
+drwxrwxrwx   0        0        0        0 2023-04-27 11:14:16.694969 upyrc-0.9.1/src/upyrc/
+-rw-rw-rw-   0        0        0       21 2023-04-27 07:37:57.000000 upyrc-0.9.1/src/upyrc/__init__.py
+-rw-rw-rw-   0        0        0    41934 2023-04-27 07:54:44.000000 upyrc-0.9.1/src/upyrc/upyrc.py
+drwxrwxrwx   0        0        0        0 2023-04-27 11:14:16.700973 upyrc-0.9.1/src/upyrc.egg-info/
+-rw-rw-rw-   0        0        0     4118 2023-04-27 11:14:16.000000 upyrc-0.9.1/src/upyrc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-04-27 11:14:16.000000 upyrc-0.9.1/src/upyrc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-27 11:14:16.000000 upyrc-0.9.1/src/upyrc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-27 11:14:16.000000 upyrc-0.9.1/src/upyrc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-27 11:14:16.000000 upyrc-0.9.1/src/upyrc.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-27 11:14:16.702004 upyrc-0.9.1/tests/
+-rw-rw-rw-   0        0        0     8057 2023-04-27 08:03:06.000000 upyrc-0.9.1/tests/test_uremote.py
```

### Comparing `upyrc-0.9.0/LICENSE` & `upyrc-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `upyrc-0.9.0/PKG-INFO` & `upyrc-0.9.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-Metadata-Version: 2.1
-Name: upyrc
-Version: 0.9.0
-Summary: Python wrapper around the Unreal engine remote control API.
-Author-email: cgtoolbox <contact@cgtoolbox.com>
-Project-URL: Homepage, https://github.com/cgtoolbox/UnrealRemoteControlWrapper
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 # UnrealRemoteControlWrapper
 
 A (work in progress) python 3 wrapper around Unreal [remote control api](https://docs.unrealengine.com/4.27/en-US/ProductionPipelines/ScriptingAndAutomation/WebControl/QuickStart/). It allows to control Unreal engine remotly, from a dcc ( maya, blender, houdini, etc. ), or a webapp, or any other sources, using a simple python api.
 
+upyrc is available on pip:
+```
+python -m pip install upyrc
+```
+
 It needs to have the remote API plugin installed on your Unreal project, as well as the server started, you can do that on the cmd: 
 
 ```
 WebControl.StartServer
 WebControl.EnableServerOnStartup
 ```
 By default, the script use these values bellow as host and port, it matches the default value of the remote plugin from Unreal install, it needs to be set to your values if needed:
```

### Comparing `upyrc-0.9.0/README.md` & `upyrc-0.9.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,27 @@
+Metadata-Version: 2.1
+Name: upyrc
+Version: 0.9.1
+Summary: Python wrapper around the Unreal engine remote control API.
+Author-email: cgtoolbox <contact@cgtoolbox.com>
+Project-URL: Homepage, https://github.com/cgtoolbox/UnrealRemoteControlWrapper
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 
 # UnrealRemoteControlWrapper
 
 A (work in progress) python 3 wrapper around Unreal [remote control api](https://docs.unrealengine.com/4.27/en-US/ProductionPipelines/ScriptingAndAutomation/WebControl/QuickStart/). It allows to control Unreal engine remotly, from a dcc ( maya, blender, houdini, etc. ), or a webapp, or any other sources, using a simple python api.
 
+upyrc is available on pip:
+```
+python -m pip install upyrc
+```
+
 It needs to have the remote API plugin installed on your Unreal project, as well as the server started, you can do that on the cmd: 
 
 ```
 WebControl.StartServer
 WebControl.EnableServerOnStartup
 ```
 By default, the script use these values bellow as host and port, it matches the default value of the remote plugin from Unreal install, it needs to be set to your values if needed:
```

### Comparing `upyrc-0.9.0/pyproject.toml` & `upyrc-0.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "upyrc"
 description = "Python wrapper around the Unreal engine remote control API."
 readme = "README.md"
 dynamic = ["version"]
 authors = [
   { name="cgtoolbox", email="contact@cgtoolbox.com" },
 ]
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 dependencies = [
     "requests"
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "upyrc.__version__"}
```

### Comparing `upyrc-0.9.0/src/upyrc/upyrc.py` & `upyrc-0.9.1/src/upyrc/upyrc.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import dataclass
 import json
 import logging
 import requests
 from requests.exceptions import HTTPError
 import traceback
 import typing
-from typing import List
+from typing import List, Dict
 
 # Log settings
 _LOG_FORMAT = "[%(filename)s:%(lineno)s][%(asctime)s][%(levelname)s] %(message)s"
 logging.basicConfig(format=_LOG_FORMAT)
 def set_log_level(level):
     assert level in (logging.DEBUG, logging.INFO, logging.ERROR, logging.CRITICAL),\
            f"Invalid log level: {level}"
@@ -236,15 +236,15 @@
         ''' Get all remote preset name and paths.
         '''
         result = self.run_request(route_infos=ROUTE_GET_PRESETS, timeout=timeout)
         if result:
             return result["Presets"]
         return
 
-    def get_thumbnail(self, asset_path='') -> dict:
+    def get_thumbnail(self, asset_path='') -> Dict:
         ''' Get an thumbnail image from an asset path. 
         '''
         assert asset_path != '', "Invalid asset path."
         body = {"objectPath":asset_path}
         try:
             return self.run_request(route_infos=ROUTE_THUMBNAIL, json=body, timeout=self._timeout)
         except URConnectionRouteNotFoundError:
@@ -296,15 +296,15 @@
         req["RequestId"] = len(self._requests) + 1
         req["URL"] = '/' + route_infos["route"]
         req["Verb"] = route_infos["method"].upper()
         req["Body"] = body
 
         self._requests.append(req)
 
-    def execute(self) -> list[BatchResult]:
+    def execute(self) -> List[BatchResult]:
         ''' Execute all requests saved in contect's queue, in one batch request.
             Return an array of BatchResult, with each individual request's result.
         '''
         adress = f"{self._connection._adress_root}/{ROUTE_BATCH['route']}"
         batch_body = {"Requests":self._requests}
         method = getattr(requests, ROUTE_BATCH["method"])
 
@@ -381,15 +381,15 @@
         self._name = describe.get("Name")
         self._uclass = describe.get("Class")
         self._functions = self._init_func_dict(describe)
         self._path = path
 
         self._properties_cache.update(self._init_property_list(describe))
 
-    def __dir__(self) -> list[str]:
+    def __dir__(self) -> List[str]:
 
         attrs = list(self.__dict__.keys()) + \
                 [s + " (function)" for s in list(self._functions.keys())] + \
                 [s + " (property)" for s in list(self._properties_cache.keys())]
         return attrs
 
     def __getattr__(self, name):
@@ -905,15 +905,15 @@
 
         result = self.run_request(route_infos=route_infos, timeout=self._timeout)
         if result and metadata_key:
             return result["Value"]
         else:
             return result["Metadata"]
 
-    def get_all_groups(self) -> dict[str, _URemotePresetGroup]:
+    def get_all_groups(self) -> Dict[str, _URemotePresetGroup]:
         ''' Get all groups in the preset, return a list of _URemotePresetGroup.
         '''
         if not self._use_properties_cache:
             self.refresh()
         return self._groups
 
     def get_group(self, group_name: str) -> _URemotePresetGroup:
@@ -930,30 +930,30 @@
         return self._actors
 
     def get_actor(self, actor_display_name: str) -> _URemotePresetActor:
         ''' Get a specific exposed actor on this preset, returns a _URemotePresetActor.
         '''
         return self.get_all_actors().get(actor_display_name)
 
-    def get_all_property_names(self) -> list[str]:
+    def get_all_property_names(self) -> List[str]:
         ''' Get all the property names exposed on the preset.
         '''
         if not self._use_properties_cache:
             self.refresh()
         return list(self._properties_cache.keys())
 
     def get_property(self, property_display_name: str) -> _URemotePresetProperty:
         ''' Get an exposed property on the preset, retuns a _URemotePresetProperty.
             From that object, value can be fetch using .eval(), or set, using .set(value).
         '''
         if not self._use_properties_cache:
             self.refresh()
         return self._properties_cache.get(property_display_name)
 
-    def get_all_function_name(self) -> list[str]:
+    def get_all_function_name(self) -> List[str]:
         ''' Get all exposed function's display name.
         '''
         if not self._use_properties_cache:
             self.refresh()
         return list(self._functions.keys())
 
     def get_function(self, function_name: str) -> _URemotePresetFunction:
```

### Comparing `upyrc-0.9.0/src/upyrc.egg-info/PKG-INFO` & `upyrc-0.9.1/src/upyrc.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: upyrc
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python wrapper around the Unreal engine remote control API.
 Author-email: cgtoolbox <contact@cgtoolbox.com>
 Project-URL: Homepage, https://github.com/cgtoolbox/UnrealRemoteControlWrapper
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # UnrealRemoteControlWrapper
 
 A (work in progress) python 3 wrapper around Unreal [remote control api](https://docs.unrealengine.com/4.27/en-US/ProductionPipelines/ScriptingAndAutomation/WebControl/QuickStart/). It allows to control Unreal engine remotly, from a dcc ( maya, blender, houdini, etc. ), or a webapp, or any other sources, using a simple python api.
 
+upyrc is available on pip:
+```
+python -m pip install upyrc
+```
+
 It needs to have the remote API plugin installed on your Unreal project, as well as the server started, you can do that on the cmd: 
 
 ```
 WebControl.StartServer
 WebControl.EnableServerOnStartup
 ```
 By default, the script use these values bellow as host and port, it matches the default value of the remote plugin from Unreal install, it needs to be set to your values if needed:
```

### Comparing `upyrc-0.9.0/tests/test_uremote.py` & `upyrc-0.9.1/tests/test_uremote.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import upyrc
+from upyrc import upyrc
 #import logging
 #upyrc.set_log_level(logging.DEBUG)
 print("Version:", upyrc.get_version())
 
 print("\n----------- INIT CONNECTION --------------------------------------------------------------------------------------------------------------------------------\n")
 
 # Create a connection to Unreal
```

