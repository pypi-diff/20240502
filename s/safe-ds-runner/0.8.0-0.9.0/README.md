# Comparing `tmp/safe_ds_runner-0.8.0.tar.gz` & `tmp/safe_ds_runner-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe_ds_runner-0.8.0.tar", max compression
+gzip compressed data, was "safe_ds_runner-0.9.0.tar", max compression
```

## Comparing `safe_ds_runner-0.8.0.tar` & `safe_ds_runner-0.9.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2024-04-03 09:11:40.541854 safe_ds_runner-0.8.0/LICENSE
--rw-r--r--   0        0        0     1367 2024-04-03 09:11:40.541854 safe_ds_runner-0.8.0/docs/README.md
--rw-r--r--   0        0        0     1037 2024-04-03 09:12:39.533680 safe_ds_runner-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      229 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/__init__.py
--rw-r--r--   0        0        0       95 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/cli/__init__.py
--rw-r--r--   0        0        0     1368 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/cli/_cli.py
--rw-r--r--   0        0        0      165 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/main.py
--rw-r--r--   0        0        0      109 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/server/__init__.py
--rw-r--r--   0        0        0     1812 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/server/_json_encoder.py
--rw-r--r--   0        0        0    10612 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/server/_memoization_map.py
--rw-r--r--   0        0        0    14539 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/server/_messages.py
--rw-r--r--   0        0        0     5214 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/server/_module_manager.py
--rw-r--r--   0        0        0    14045 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/server/_pipeline_manager.py
--rw-r--r--   0        0        0     8593 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/server/_server.py
--rw-r--r--   0        0        0      523 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/server/main.py
--rw-r--r--   0        0        0     2186 1970-01-01 00:00:00.000000 safe_ds_runner-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-09 08:13:32.791921 safe_ds_runner-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1367 2024-04-09 08:13:32.791921 safe_ds_runner-0.9.0/docs/README.md
+-rw-r--r--   0        0        0     1037 2024-04-09 08:14:13.443838 safe_ds_runner-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      295 2024-04-09 08:13:32.795921 safe_ds_runner-0.9.0/src/safeds_runner/__init__.py
+-rw-r--r--   0        0        0       95 2024-04-09 08:13:32.795921 safe_ds_runner-0.9.0/src/safeds_runner/cli/__init__.py
+-rw-r--r--   0        0        0     1368 2024-04-09 08:13:32.795921 safe_ds_runner-0.9.0/src/safeds_runner/cli/_cli.py
+-rw-r--r--   0        0        0      165 2024-04-09 08:13:32.795921 safe_ds_runner-0.9.0/src/safeds_runner/main.py
+-rw-r--r--   0        0        0      109 2024-04-09 08:13:32.795921 safe_ds_runner-0.9.0/src/safeds_runner/server/__init__.py
+-rw-r--r--   0        0        0     1812 2024-04-09 08:13:32.795921 safe_ds_runner-0.9.0/src/safeds_runner/server/_json_encoder.py
+-rw-r--r--   0        0        0    11001 2024-04-09 08:13:32.795921 safe_ds_runner-0.9.0/src/safeds_runner/server/_memoization_map.py
+-rw-r--r--   0        0        0    14539 2024-04-09 08:13:32.795921 safe_ds_runner-0.9.0/src/safeds_runner/server/_messages.py
+-rw-r--r--   0        0        0     5214 2024-04-09 08:13:32.795921 safe_ds_runner-0.9.0/src/safeds_runner/server/_module_manager.py
+-rw-r--r--   0        0        0    15996 2024-04-09 08:13:32.795921 safe_ds_runner-0.9.0/src/safeds_runner/server/_pipeline_manager.py
+-rw-r--r--   0        0        0     8593 2024-04-09 08:13:32.795921 safe_ds_runner-0.9.0/src/safeds_runner/server/_server.py
+-rw-r--r--   0        0        0      523 2024-04-09 08:13:32.795921 safe_ds_runner-0.9.0/src/safeds_runner/server/main.py
+-rw-r--r--   0        0        0     2186 1970-01-01 00:00:00.000000 safe_ds_runner-0.9.0/PKG-INFO
```

### Comparing `safe_ds_runner-0.8.0/LICENSE` & `safe_ds_runner-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safe_ds_runner-0.8.0/docs/README.md` & `safe_ds_runner-0.9.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `safe_ds_runner-0.8.0/pyproject.toml` & `safe_ds_runner-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "safe-ds-runner"
-version = "0.8.0"
+version = "0.9.0"
 description = "Execute Safe-DS programs that were compiled to Python."
 authors = ["Lars Reimann <mail@larsreimann.com>"]
 license = "MIT"
 readme = "docs/README.md"
 repository = "https://github.com/Safe-DS/Runner"
 documentation = "https://safe-ds-runner.readthedocs.io"
 keywords = ["data-science", "machine-learning", "usability", "learnability"]
```

### Comparing `safe_ds_runner-0.8.0/src/safeds_runner/cli/_cli.py` & `safe_ds_runner-0.9.0/src/safeds_runner/cli/_cli.py`

 * *Files identical despite different names*

### Comparing `safe_ds_runner-0.8.0/src/safeds_runner/server/_json_encoder.py` & `safe_ds_runner-0.9.0/src/safeds_runner/server/_json_encoder.py`

 * *Files identical despite different names*

### Comparing `safe_ds_runner-0.8.0/src/safeds_runner/server/_memoization_map.py` & `safe_ds_runner-0.9.0/src/safeds_runner/server/_memoization_map.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Module that contains the memoization logic and stats."""
 
 import dataclasses
+import inspect
 import logging
 import sys
 import time
 from collections.abc import Callable
 from dataclasses import dataclass
 from typing import Any, TypeAlias
 
@@ -136,15 +137,19 @@
         The result of the specified function, if any exists
         """
         access_timestamp = time.time_ns()
 
         # Lookup memoized value
         lookup_time_start = time.perf_counter_ns()
         key = self._create_memoization_key(function_name, parameters, hidden_parameters)
-        memoized_value = self._lookup_value(key)
+        try:
+            memoized_value = self._lookup_value(key)
+        # Pickling may raise AttributeError, hashing may raise TypeError
+        except (AttributeError, TypeError):
+            return function_callable(*parameters)
         lookup_time = time.perf_counter_ns() - lookup_time_start
 
         # Hit
         if memoized_value is not None:
             self._update_stats_on_hit(function_name, access_timestamp, lookup_time)
             return memoized_value
 
@@ -191,15 +196,15 @@
         hidden_parameters
             List of parameters not passed to the function
 
         Returns
         -------
         A memoization key, which contains the lists converted to tuples
         """
-        return function_name, _convert_list_to_tuple(parameters), _convert_list_to_tuple(hidden_parameters)
+        return function_name, _make_hashable(parameters), _make_hashable(hidden_parameters)
 
     def _lookup_value(self, key: MemoizationKey) -> Any | None:
         """
         Lookup a potentially existing value from the memoization cache.
 
         Parameters
         ----------
@@ -286,29 +291,38 @@
         if stats is None:
             stats = MemoizationStats()
 
         stats.update_on_miss(access_timestamp, lookup_time, computation_time, memory_size)
         self._map_stats[function_name] = stats
 
 
-def _convert_list_to_tuple(values: list) -> tuple:
+def _make_hashable(value: Any) -> Any:
     """
-    Recursively convert a mutable list of values to an immutable tuple containing the same values, to make the values hashable.
+    Make a value hashable.
 
     Parameters
     ----------
-    values : list
-        Values that should be converted to a tuple
+    value:
+        Value to be converted.
 
     Returns
     -------
-    tuple
-        Converted list containing all the elements of the provided list
+    converted_value:
+        Converted value.
     """
-    return tuple(_convert_list_to_tuple(value) if isinstance(value, list) else value for value in values)
+    if isinstance(value, dict):
+        return tuple((_make_hashable(key), _make_hashable(value)) for key, value in value.items())
+    elif isinstance(value, list):
+        return tuple(_make_hashable(element) for element in value)
+    elif callable(value):
+        # This is a band-aid solution to make callables serializable. Unfortunately, `getsource` returns more than just
+        # the source code for lambdas.
+        return inspect.getsource(value)
+    else:
+        return value
 
 
 def _get_size_of_value(value: Any) -> int:
     """
     Recursively calculate the memory usage of a given value.
 
     Parameters
```

### Comparing `safe_ds_runner-0.8.0/src/safeds_runner/server/_messages.py` & `safe_ds_runner-0.9.0/src/safeds_runner/server/_messages.py`

 * *Files identical despite different names*

### Comparing `safe_ds_runner-0.8.0/src/safeds_runner/server/_module_manager.py` & `safe_ds_runner-0.9.0/src/safeds_runner/server/_module_manager.py`

 * *Files identical despite different names*

### Comparing `safe_ds_runner-0.8.0/src/safeds_runner/server/_pipeline_manager.py` & `safe_ds_runner-0.9.0/src/safeds_runner/server/_pipeline_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -305,15 +305,15 @@
     value : Any
         Actual value of the placeholder.
     """
     if current_pipeline is not None:
         current_pipeline.save_placeholder(placeholder_name, value)
 
 
-def memoized_call(
+def memoized_static_call(
     function_name: str,
     function_callable: typing.Callable,
     parameters: list[Any],
     hidden_parameters: list[Any],
 ) -> Any:
     """
     Call a function that can be memoized and save the result.
@@ -338,14 +338,60 @@
     """
     if current_pipeline is None:
         return None  # pragma: no cover
     memoization_map = current_pipeline.get_memoization_map()
     return memoization_map.memoized_function_call(function_name, function_callable, parameters, hidden_parameters)
 
 
+def memoized_dynamic_call(
+    function_name: str,
+    function_callable: typing.Callable | None,
+    parameters: list[Any],
+    hidden_parameters: list[Any],
+) -> Any:
+    """
+    Dynamically call a function that can be memoized and save the result.
+
+    If a function has been previously memoized, the previous result may be reused.
+    Dynamically calling in this context means, that if a callable is provided (e.g. if default parameters are set), it will be called.
+    If no such callable is provided, the function name will be used to look up the function on the instance passed as the first parameter in the parameter list.
+
+    Parameters
+    ----------
+    function_name : str
+        Simple function name
+    function_callable : typing.Callable | None
+        Function that is called and memoized if the result was not found in the memoization map or none, if the function handle should be in the provided instance
+    parameters : list[Any]
+        List of parameters for the function, the first parameter should be the instance the function should be called on (receiver)
+    hidden_parameters : list[Any]
+        List of hidden parameters for the function. This is used for memoizing some impure functions.
+
+    Returns
+    -------
+    Any
+        The result of the specified function, if any exists
+    """
+    if current_pipeline is None:
+        return None  # pragma: no cover
+    fully_qualified_function_name = (
+        parameters[0].__class__.__module__ + "." + parameters[0].__class__.__qualname__ + "." + function_name
+    )
+    memoization_map = current_pipeline.get_memoization_map()
+    if function_callable is None:
+        function_target_bound = getattr(parameters[0], function_name)
+        function_callable = function_target_bound.__func__
+    return memoization_map.memoized_function_call(
+        fully_qualified_function_name,
+        function_callable,
+        parameters,
+        hidden_parameters,
+    )
+
+
 def file_mtime(filename: str) -> int | None:
     """
     Get the last modification timestamp of the provided file.
 
     Parameters
     ----------
     filename: str
```

### Comparing `safe_ds_runner-0.8.0/src/safeds_runner/server/_server.py` & `safe_ds_runner-0.9.0/src/safeds_runner/server/_server.py`

 * *Files identical despite different names*

### Comparing `safe_ds_runner-0.8.0/src/safeds_runner/server/main.py` & `safe_ds_runner-0.9.0/src/safeds_runner/server/main.py`

 * *Files identical despite different names*

### Comparing `safe_ds_runner-0.8.0/PKG-INFO` & `safe_ds_runner-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-ds-runner
-Version: 0.8.0
+Version: 0.9.0
 Summary: Execute Safe-DS programs that were compiled to Python.
 Home-page: https://github.com/Safe-DS/Runner
 License: MIT
 Keywords: data-science,machine-learning,usability,learnability
 Author: Lars Reimann
 Author-email: mail@larsreimann.com
 Requires-Python: >=3.11,<3.13
```

