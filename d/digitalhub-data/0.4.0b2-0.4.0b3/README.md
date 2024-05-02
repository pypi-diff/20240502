# Comparing `tmp/digitalhub_data-0.4.0b2.tar.gz` & `tmp/digitalhub_data-0.4.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_data-0.4.0b2.tar", last modified: Wed Apr 24 07:52:12 2024, max compression
+gzip compressed data, was "digitalhub_data-0.4.0b3.tar", last modified: Thu May  2 13:38:10 2024, max compression
```

## Comparing `digitalhub_data-0.4.0b2.tar` & `digitalhub_data-0.4.0b3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:52:12.369888 digitalhub_data-0.4.0b2/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-04-24 07:52:12.369888 digitalhub_data-0.4.0b2/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      468 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b2/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:52:12.361888 digitalhub_data-0.4.0b2/digitalhub_data/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      329 2024-04-19 08:14:48.000000 digitalhub_data-0.4.0b2/digitalhub_data/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:52:12.361888 digitalhub_data-0.4.0b2/digitalhub_data/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:56.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:52:12.365888 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:45.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3322 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/builder.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6406 2024-04-19 08:14:48.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/crud.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:52:12.365888 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/entity/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-03-04 14:42:21.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/entity/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6489 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/entity/_base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      180 2024-03-15 13:13:54.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/entity/dataitem.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      142 2024-03-04 15:16:25.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/entity/iceberg.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3042 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/entity/table.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      582 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1093 2024-04-08 13:12:06.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1418 2024-04-08 13:12:04.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      863 2024-03-15 12:04:24.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:52:12.365888 digitalhub_data-0.4.0b2/digitalhub_data/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-31 10:03:33.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6053 2024-04-19 08:14:48.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5909 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      950 2024-02-15 10:15:41.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1050 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:52:12.369888 digitalhub_data-0.4.0b2/digitalhub_data/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-22 14:51:32.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/runs/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      407 2024-03-08 13:54:39.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      351 2024-03-14 13:46:16.000000 digitalhub_data-0.4.0b2/digitalhub_data/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:52:12.369888 digitalhub_data-0.4.0b2/digitalhub_data/utils/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-29 10:07:05.000000 digitalhub_data-0.4.0b2/digitalhub_data/utils/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2440 2024-02-05 09:25:21.000000 digitalhub_data-0.4.0b2/digitalhub_data/utils/data_utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-04-24 07:52:12.369888 digitalhub_data-0.4.0b2/digitalhub_data.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-04-24 07:52:12.000000 digitalhub_data-0.4.0b2/digitalhub_data.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1305 2024-04-24 07:52:12.000000 digitalhub_data-0.4.0b2/digitalhub_data.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-04-24 07:52:12.000000 digitalhub_data-0.4.0b2/digitalhub_data.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-24 07:52:12.000000 digitalhub_data-0.4.0b2/digitalhub_data.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-04-24 07:52:12.000000 digitalhub_data-0.4.0b2/digitalhub_data.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1056 2024-04-23 13:34:39.000000 digitalhub_data-0.4.0b2/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-04-24 07:52:12.369888 digitalhub_data-0.4.0b2/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:38:10.677123 digitalhub_data-0.4.0b3/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-05-02 13:38:10.673123 digitalhub_data-0.4.0b3/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      468 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b3/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:38:10.669123 digitalhub_data-0.4.0b3/digitalhub_data/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      329 2024-05-02 13:22:48.000000 digitalhub_data-0.4.0b3/digitalhub_data/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:38:10.669123 digitalhub_data-0.4.0b3/digitalhub_data/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:56.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:38:10.673123 digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:45.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3322 2024-05-02 13:22:48.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/builder.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6406 2024-05-02 13:22:48.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/crud.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:38:10.673123 digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/entity/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-03-04 14:42:21.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/entity/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6857 2024-05-02 13:22:48.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/entity/_base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      180 2024-03-15 13:13:54.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/entity/dataitem.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      142 2024-03-04 15:16:25.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/entity/iceberg.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2985 2024-04-24 13:01:27.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/entity/table.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      582 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1093 2024-04-08 13:12:06.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1418 2024-04-08 13:12:04.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      863 2024-03-15 12:04:24.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:38:10.673123 digitalhub_data-0.4.0b3/digitalhub_data/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-31 10:03:33.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6053 2024-05-02 13:22:48.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5909 2024-05-02 13:22:48.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      950 2024-02-15 10:15:41.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1050 2024-04-23 09:36:04.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:38:10.673123 digitalhub_data-0.4.0b3/digitalhub_data/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-22 14:51:32.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/runs/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      407 2024-03-08 13:54:39.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      351 2024-03-14 13:46:16.000000 digitalhub_data-0.4.0b3/digitalhub_data/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:38:10.673123 digitalhub_data-0.4.0b3/digitalhub_data/utils/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-29 10:07:05.000000 digitalhub_data-0.4.0b3/digitalhub_data/utils/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2440 2024-02-05 09:25:21.000000 digitalhub_data-0.4.0b3/digitalhub_data/utils/data_utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-02 13:38:10.673123 digitalhub_data-0.4.0b3/digitalhub_data.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)      946 2024-05-02 13:38:10.000000 digitalhub_data-0.4.0b3/digitalhub_data.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1305 2024-05-02 13:38:10.000000 digitalhub_data-0.4.0b3/digitalhub_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-02 13:38:10.000000 digitalhub_data-0.4.0b3/digitalhub_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-02 13:38:10.000000 digitalhub_data-0.4.0b3/digitalhub_data.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-02 13:38:10.000000 digitalhub_data-0.4.0b3/digitalhub_data.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1056 2024-05-02 08:14:16.000000 digitalhub_data-0.4.0b3/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-02 13:38:10.677123 digitalhub_data-0.4.0b3/setup.cfg
```

### Comparing `digitalhub_data-0.4.0b2/PKG-INFO` & `digitalhub_data-0.4.0b3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-data
-Version: 0.4.0b2
+Version: 0.4.0b3
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
```

### Comparing `digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/builder.py` & `digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/crud.py` & `digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/entity/_base.py` & `digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/entity/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 
 from digitalhub_core.context.builder import get_context
 from digitalhub_core.entities._base.entity import Entity
 from digitalhub_core.entities._builders.metadata import build_metadata
 from digitalhub_core.entities._builders.spec import build_spec
 from digitalhub_core.entities._builders.status import build_status
-from digitalhub_core.utils.api import api_ctx_create, api_ctx_update
+from digitalhub_core.utils.api import api_ctx_create, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.exceptions import EntityError
 from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
 from digitalhub_core.utils.io_utils import write_yaml
 from digitalhub_core.utils.uri_utils import map_uri_scheme
 
 if typing.TYPE_CHECKING:
     from digitalhub_core.context.context import Context
@@ -73,15 +73,15 @@
         self.status = status
         self.user = user
 
         # Add attributes to be used in the to_dict method
         self._obj_attr.extend(["project", "name", "id", "key"])
 
     #############################
-    #  Save / Export
+    #  Save / Refresh / Export
     #############################
 
     def save(self, update: bool = False) -> Dataitem:
         """
         Save entity into backend.
 
         Parameters
@@ -104,14 +104,28 @@
 
         self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
         api = api_ctx_update(self.project, "dataitems", self.id)
         new_obj = self._context().update_object(api, obj)
         self._update_attributes(new_obj)
         return self
 
+    def refresh(self) -> Dataitem:
+        """
+        Refresh object from backend.
+
+        Returns
+        -------
+        Dataitem
+            Entity refreshed.
+        """
+        api = api_ctx_read(self.project, "dataitems", self.id)
+        obj = self._context().read_object(api)
+        self._update_attributes(obj)
+        return self
+
     def export(self, filename: str | None = None) -> None:
         """
         Export object as a YAML file.
 
         Parameters
         ----------
         filename : str
```

### Comparing `digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/entity/table.py` & `digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/entity/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import shutil
 import typing
 from pathlib import Path
 
 from digitalhub_core.stores.builder import get_default_store, get_store
-from digitalhub_core.utils.exceptions import EntityError
 from digitalhub_data.entities.dataitems.entity._base import Dataitem
 
 if typing.TYPE_CHECKING:
     import pandas as pd
 
 
 class DataitemTable(Dataitem):
```

### Comparing `digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/metadata.py` & `digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/models.py` & `digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/spec.py` & `digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b2/digitalhub_data/entities/dataitems/status.py` & `digitalhub_data-0.4.0b3/digitalhub_data/entities/dataitems/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b2/digitalhub_data/entities/projects/crud.py` & `digitalhub_data-0.4.0b3/digitalhub_data/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b2/digitalhub_data/entities/projects/entity.py` & `digitalhub_data-0.4.0b3/digitalhub_data/entities/projects/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b2/digitalhub_data/entities/projects/spec.py` & `digitalhub_data-0.4.0b3/digitalhub_data/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b2/digitalhub_data/entities/registries.py` & `digitalhub_data-0.4.0b3/digitalhub_data/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b2/digitalhub_data/utils/data_utils.py` & `digitalhub_data-0.4.0b3/digitalhub_data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b2/digitalhub_data.egg-info/PKG-INFO` & `digitalhub_data-0.4.0b3/digitalhub_data.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-data
-Version: 0.4.0b2
+Version: 0.4.0b3
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
```

### Comparing `digitalhub_data-0.4.0b2/digitalhub_data.egg-info/SOURCES.txt` & `digitalhub_data-0.4.0b3/digitalhub_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.4.0b2/pyproject.toml` & `digitalhub_data-0.4.0b3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-data"
-version = "0.4.0b2"
+version = "0.4.0b3"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -23,15 +23,15 @@
     "digitalhub-core~=0.3",
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["modules*"]
 
 [tool.bumpver]
-current_version = "0.4.0b2"
+current_version = "0.4.0b3"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

