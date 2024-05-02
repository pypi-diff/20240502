# Comparing `tmp/warpzone_sdk-9.1.8.tar.gz` & `tmp/warpzone_sdk-9.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warpzone_sdk-9.1.8.tar", max compression
+gzip compressed data, was "warpzone_sdk-9.1.9.tar", max compression
```

## Comparing `warpzone_sdk-9.1.8.tar` & `warpzone_sdk-9.1.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1141 2023-10-26 07:38:21.388048 warpzone_sdk-9.1.8/pyproject.toml
--rw-r--r--   0        0        0     1397 2023-10-26 07:38:21.388048 warpzone_sdk-9.1.8/warpzone/__init__.py
--rw-r--r--   0        0        0       21 2023-10-26 07:38:21.388048 warpzone_sdk-9.1.8/warpzone/blobstorage/__init__.py
--rw-r--r--   0        0        0     2864 2023-10-26 07:38:21.388048 warpzone_sdk-9.1.8/warpzone/blobstorage/client.py
--rw-r--r--   0        0        0       24 2023-10-26 07:38:21.388048 warpzone_sdk-9.1.8/warpzone/enums/__init__.py
--rw-r--r--   0        0        0      213 2023-10-26 07:38:21.388048 warpzone_sdk-9.1.8/warpzone/enums/topicenum.py
--rw-r--r--   0        0        0       35 2023-10-26 07:38:21.388048 warpzone_sdk-9.1.8/warpzone/function/__init__.py
--rw-r--r--   0        0        0     1018 2023-10-26 07:38:21.388048 warpzone_sdk-9.1.8/warpzone/function/checks.py
--rw-r--r--   0        0        0     2128 2023-10-26 07:38:21.388048 warpzone_sdk-9.1.8/warpzone/function/functionize.py
--rw-r--r--   0        0        0     3878 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/function/integrations.py
--rw-r--r--   0        0        0     2223 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/function/monitor.py
--rw-r--r--   0        0        0     2105 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/function/process.py
--rw-r--r--   0        0        0       46 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/function/processors/__init__.py
--rw-r--r--   0        0        0      836 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/function/processors/dependencies.py
--rw-r--r--   0        0        0     2067 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/function/processors/outputs.py
--rw-r--r--   0        0        0     1727 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/function/processors/triggers.py
--rw-r--r--   0        0        0     2268 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/function/signature.py
--rw-r--r--   0        0        0      725 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/function/types.py
--rw-r--r--   0        0        0     2108 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/healthchecks/__init__.py
--rw-r--r--   0        0        0     1187 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/healthchecks/model.py
--rw-r--r--   0        0        0       87 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/monitor/__init__.py
--rw-r--r--   0        0        0     1650 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/monitor/logs.py
--rw-r--r--   0        0        0     4781 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/monitor/traces.py
--rw-r--r--   0        0        0       21 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/servicebus/data/__init__.py
--rw-r--r--   0        0        0     5666 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/servicebus/data/client.py
--rw-r--r--   0        0        0       21 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/servicebus/events/__init__.py
--rw-r--r--   0        0        0     4270 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/servicebus/events/client.py
--rw-r--r--   0        0        0       21 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/tablestorage/db/__init__.py
--rw-r--r--   0        0        0     1556 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/tablestorage/db/base_client.py
--rw-r--r--   0        0        0     1947 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/tablestorage/db/client.py
--rw-r--r--   0        0        0     1691 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/tablestorage/db/client_async.py
--rw-r--r--   0        0        0       94 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/tablestorage/tables/__init__.py
--rw-r--r--   0        0        0     2916 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/tablestorage/tables/client.py
--rw-r--r--   0        0        0     2516 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/tablestorage/tables/client_async.py
--rw-r--r--   0        0        0      932 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/tablestorage/tables/helpers.py
--rw-r--r--   0        0        0     2689 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/tablestorage/tables/operations.py
--rw-r--r--   0        0        0      248 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/testing/__init__.py
--rw-r--r--   0        0        0     3661 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/testing/assertions.py
--rw-r--r--   0        0        0     3737 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/testing/data.py
--rw-r--r--   0        0        0       27 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/transform/__init__.py
--rw-r--r--   0        0        0     2359 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/transform/data.py
--rw-r--r--   0        0        0     2374 2023-10-26 07:38:21.392048 warpzone_sdk-9.1.8/warpzone/transform/schema.py
--rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 warpzone_sdk-9.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1141 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1397 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/__init__.py
+-rw-r--r--   0        0        0       21 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/blobstorage/__init__.py
+-rw-r--r--   0        0        0     2864 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/blobstorage/client.py
+-rw-r--r--   0        0        0       24 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/enums/__init__.py
+-rw-r--r--   0        0        0      213 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/enums/topicenum.py
+-rw-r--r--   0        0        0       35 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/function/__init__.py
+-rw-r--r--   0        0        0     1018 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/function/checks.py
+-rw-r--r--   0        0        0     2128 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/function/functionize.py
+-rw-r--r--   0        0        0     3878 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/function/integrations.py
+-rw-r--r--   0        0        0     2223 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/function/monitor.py
+-rw-r--r--   0        0        0     2105 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/function/process.py
+-rw-r--r--   0        0        0       46 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/function/processors/__init__.py
+-rw-r--r--   0        0        0      836 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/function/processors/dependencies.py
+-rw-r--r--   0        0        0     2067 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/function/processors/outputs.py
+-rw-r--r--   0        0        0     1727 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/function/processors/triggers.py
+-rw-r--r--   0        0        0     2268 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/function/signature.py
+-rw-r--r--   0        0        0      725 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/function/types.py
+-rw-r--r--   0        0        0     2108 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/healthchecks/__init__.py
+-rw-r--r--   0        0        0     1187 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/healthchecks/model.py
+-rw-r--r--   0        0        0       87 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/monitor/__init__.py
+-rw-r--r--   0        0        0     1650 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/monitor/logs.py
+-rw-r--r--   0        0        0     4781 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/monitor/traces.py
+-rw-r--r--   0        0        0       21 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/servicebus/data/__init__.py
+-rw-r--r--   0        0        0     5666 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/servicebus/data/client.py
+-rw-r--r--   0        0        0       21 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/servicebus/events/__init__.py
+-rw-r--r--   0        0        0     4270 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/servicebus/events/client.py
+-rw-r--r--   0        0        0       21 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/tablestorage/db/__init__.py
+-rw-r--r--   0        0        0     1556 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/tablestorage/db/base_client.py
+-rw-r--r--   0        0        0     1947 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/tablestorage/db/client.py
+-rw-r--r--   0        0        0     1691 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/tablestorage/db/client_async.py
+-rw-r--r--   0        0        0       94 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/tablestorage/tables/__init__.py
+-rw-r--r--   0        0        0     2916 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/tablestorage/tables/client.py
+-rw-r--r--   0        0        0     2516 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/tablestorage/tables/client_async.py
+-rw-r--r--   0        0        0      932 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/tablestorage/tables/helpers.py
+-rw-r--r--   0        0        0     2689 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/tablestorage/tables/operations.py
+-rw-r--r--   0        0        0      248 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/testing/__init__.py
+-rw-r--r--   0        0        0     3661 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/testing/assertions.py
+-rw-r--r--   0        0        0     3828 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/testing/data.py
+-rw-r--r--   0        0        0       27 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/transform/__init__.py
+-rw-r--r--   0        0        0     2359 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/transform/data.py
+-rw-r--r--   0        0        0     2374 2023-10-26 12:01:12.109453 warpzone_sdk-9.1.9/warpzone/transform/schema.py
+-rw-r--r--   0        0        0     1070 1970-01-01 00:00:00.000000 warpzone_sdk-9.1.9/PKG-INFO
```

### Comparing `warpzone_sdk-9.1.8/pyproject.toml` & `warpzone_sdk-9.1.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "warpzone-sdk"
-version = "9.1.8"
+version = "9.1.9"
 description = "The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage"
 authors = ["Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "warpzone" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `warpzone_sdk-9.1.8/warpzone/__init__.py` & `warpzone_sdk-9.1.9/warpzone/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/blobstorage/client.py` & `warpzone_sdk-9.1.9/warpzone/blobstorage/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/function/checks.py` & `warpzone_sdk-9.1.9/warpzone/function/checks.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/function/functionize.py` & `warpzone_sdk-9.1.9/warpzone/function/functionize.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/function/integrations.py` & `warpzone_sdk-9.1.9/warpzone/function/integrations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/function/monitor.py` & `warpzone_sdk-9.1.9/warpzone/function/monitor.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/function/process.py` & `warpzone_sdk-9.1.9/warpzone/function/process.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/function/processors/dependencies.py` & `warpzone_sdk-9.1.9/warpzone/function/processors/dependencies.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/function/processors/outputs.py` & `warpzone_sdk-9.1.9/warpzone/function/processors/outputs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/function/processors/triggers.py` & `warpzone_sdk-9.1.9/warpzone/function/processors/triggers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/function/signature.py` & `warpzone_sdk-9.1.9/warpzone/function/signature.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/function/types.py` & `warpzone_sdk-9.1.9/warpzone/function/types.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/healthchecks/__init__.py` & `warpzone_sdk-9.1.9/warpzone/healthchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/healthchecks/model.py` & `warpzone_sdk-9.1.9/warpzone/healthchecks/model.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/monitor/logs.py` & `warpzone_sdk-9.1.9/warpzone/monitor/logs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/monitor/traces.py` & `warpzone_sdk-9.1.9/warpzone/monitor/traces.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/servicebus/data/client.py` & `warpzone_sdk-9.1.9/warpzone/servicebus/data/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/servicebus/events/client.py` & `warpzone_sdk-9.1.9/warpzone/servicebus/events/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/tablestorage/db/base_client.py` & `warpzone_sdk-9.1.9/warpzone/tablestorage/db/base_client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/tablestorage/db/client.py` & `warpzone_sdk-9.1.9/warpzone/tablestorage/db/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/tablestorage/db/client_async.py` & `warpzone_sdk-9.1.9/warpzone/tablestorage/db/client_async.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/tablestorage/tables/client.py` & `warpzone_sdk-9.1.9/warpzone/tablestorage/tables/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/tablestorage/tables/client_async.py` & `warpzone_sdk-9.1.9/warpzone/tablestorage/tables/client_async.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/tablestorage/tables/helpers.py` & `warpzone_sdk-9.1.9/warpzone/tablestorage/tables/helpers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/tablestorage/tables/operations.py` & `warpzone_sdk-9.1.9/warpzone/tablestorage/tables/operations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/testing/assertions.py` & `warpzone_sdk-9.1.9/warpzone/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/testing/data.py` & `warpzone_sdk-9.1.9/warpzone/testing/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import datetime as dt
 import os
 from pathlib import Path
 from typing import Optional
 
+import numpy as np
 import pandas as pd
 
 from warpzone.servicebus.data.client import DataMessage
 from warpzone.transform.schema import generate_and_stringify_schema
 
 
 def get_filepath(filename: str, subfolder: str = "data"):
     return Path(os.environ["PYTEST_CURRENT_TEST"]).parent / subfolder / filename
 
 
 def parse_iso_datetime(values: pd.Series) -> pd.Series:
+    if values.replace("", np.nan).dropna().empty:
+        return values
     try:
         converted_values = pd.to_datetime(values)
     except (ValueError, TypeError):
         # if not possible to parse as datetime, return original values
         return values
     try:
         values_isoformat = converted_values.dropna().apply(pd.Timestamp.isoformat)
```

### Comparing `warpzone_sdk-9.1.8/warpzone/transform/data.py` & `warpzone_sdk-9.1.9/warpzone/transform/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/warpzone/transform/schema.py` & `warpzone_sdk-9.1.9/warpzone/transform/schema.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-9.1.8/PKG-INFO` & `warpzone_sdk-9.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warpzone-sdk
-Version: 9.1.8
+Version: 9.1.9
 Summary: The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage
 Author: Mikkel Ladekarl Folmersen Nygaard
 Author-email: mny@energinet.dk
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
```

