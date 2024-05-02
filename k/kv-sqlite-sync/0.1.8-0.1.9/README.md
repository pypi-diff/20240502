# Comparing `tmp/kv_sqlite_sync-0.1.8.tar.gz` & `tmp/kv_sqlite_sync-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kv_sqlite_sync-0.1.8.tar", last modified: Thu Apr 25 05:12:27 2024, max compression
+gzip compressed data, was "kv_sqlite_sync-0.1.9.tar", last modified: Thu Apr 25 07:27:09 2024, max compression
```

## Comparing `kv_sqlite_sync-0.1.8.tar` & `kv_sqlite_sync-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:12:27.044239 kv_sqlite_sync-0.1.8/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      894 2024-04-25 05:12:27.044239 kv_sqlite_sync-0.1.8/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      401 2024-04-24 13:02:36.000000 kv_sqlite_sync-0.1.8/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      695 2024-04-25 05:12:24.000000 kv_sqlite_sync-0.1.8/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 05:12:27.044239 kv_sqlite_sync-0.1.8/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:12:27.044239 kv_sqlite_sync-0.1.8/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:12:27.044239 kv_sqlite_sync-0.1.8/src/kv/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:12:27.044239 kv_sqlite_sync-0.1.8/src/kv/sqlite/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 13:32:50.000000 kv_sqlite_sync-0.1.8/src/kv/sqlite/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      203 2024-04-24 13:32:38.000000 kv_sqlite_sync-0.1.8/src/kv/sqlite/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3480 2024-04-25 05:10:08.000000 kv_sqlite_sync-0.1.8/src/kv/sqlite/api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1631 2024-04-24 13:37:20.000000 kv_sqlite_sync-0.1.8/src/kv/sqlite/queries.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 05:12:27.044239 kv_sqlite_sync-0.1.8/src/kv_sqlite_sync.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      894 2024-04-25 05:12:27.000000 kv_sqlite_sync-0.1.8/src/kv_sqlite_sync.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      332 2024-04-25 05:12:27.000000 kv_sqlite_sync-0.1.8/src/kv_sqlite_sync.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 05:12:27.000000 kv_sqlite_sync-0.1.8/src/kv_sqlite_sync.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       30 2024-04-25 05:12:27.000000 kv_sqlite_sync-0.1.8/src/kv_sqlite_sync.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-25 05:12:27.000000 kv_sqlite_sync-0.1.8/src/kv_sqlite_sync.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:27:09.774241 kv_sqlite_sync-0.1.9/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      927 2024-04-25 07:27:09.774241 kv_sqlite_sync-0.1.9/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      401 2024-04-24 13:02:36.000000 kv_sqlite_sync-0.1.9/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      716 2024-04-25 07:27:07.000000 kv_sqlite_sync-0.1.9/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-25 07:27:09.774241 kv_sqlite_sync-0.1.9/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:27:09.774241 kv_sqlite_sync-0.1.9/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:27:09.774241 kv_sqlite_sync-0.1.9/src/kv/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:27:09.774241 kv_sqlite_sync-0.1.9/src/kv/sqlite/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 13:32:50.000000 kv_sqlite_sync-0.1.9/src/kv/sqlite/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      203 2024-04-24 13:32:38.000000 kv_sqlite_sync-0.1.9/src/kv/sqlite/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3491 2024-04-25 07:26:10.000000 kv_sqlite_sync-0.1.9/src/kv/sqlite/api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1642 2024-04-25 07:26:10.000000 kv_sqlite_sync-0.1.9/src/kv/sqlite/queries.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-25 07:27:09.774241 kv_sqlite_sync-0.1.9/src/kv_sqlite_sync.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      927 2024-04-25 07:27:09.000000 kv_sqlite_sync-0.1.9/src/kv_sqlite_sync.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      332 2024-04-25 07:27:09.000000 kv_sqlite_sync-0.1.9/src/kv_sqlite_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-25 07:27:09.000000 kv_sqlite_sync-0.1.9/src/kv_sqlite_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       48 2024-04-25 07:27:09.000000 kv_sqlite_sync-0.1.9/src/kv_sqlite_sync.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        3 2024-04-25 07:27:09.000000 kv_sqlite_sync-0.1.9/src/kv_sqlite_sync.egg-info/top_level.txt
```

### Comparing `kv_sqlite_sync-0.1.8/PKG-INFO` & `kv_sqlite_sync-0.1.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: kv-sqlite-sync
-Version: 0.1.8
+Version: 0.1.9
 Summary: Key-Value interface over SQLite. Supports any datatype, including JSON and BLOB
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-storage
 Project-URL: home, https://github.com/moveread/python-storage/tree/main/kv/kv-sqlite-sync
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
 Requires-Dist: haskellian
 Requires-Dist: lazy-loader
+Requires-Dist: typing-extensions
 
 # Sqlite Kv (Sync)
 
 > Synchronous Key-Value interface over SQLite. Supports any datatype, including JSON and BLOB
 
 ## Usage
```

### Comparing `kv_sqlite_sync-0.1.8/pyproject.toml` & `kv_sqlite_sync-0.1.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kv-sqlite-sync"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Key-Value interface over SQLite. Supports any datatype, including JSON and BLOB"
 dependencies = [
-  "kv-api", "haskellian", "lazy-loader"
+  "kv-api", "haskellian", "lazy-loader", "typing-extensions"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
 repo = "https://github.com/moveread/python-storage"
 home = "https://github.com/moveread/python-storage/tree/main/kv/kv-sqlite-sync"
```

### Comparing `kv_sqlite_sync-0.1.8/src/kv/sqlite/api.py` & `kv_sqlite_sync-0.1.9/src/kv/sqlite/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import AsyncIterable, TypeVar, Generic, Callable, cast, Sequence
+from typing_extensions import AsyncIterable, TypeVar, Generic, Callable, cast, Sequence
 from dataclasses import dataclass
 from haskellian import either as E, promise as P, asyn_iter as AI
 from pydantic import RootModel
 from kv.api import KV, InexistentItem, DBError, InvalidData
 import sqlite3
 import os
 from . import queries
```

### Comparing `kv_sqlite_sync-0.1.8/src/kv/sqlite/queries.py` & `kv_sqlite_sync-0.1.9/src/kv/sqlite/queries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import NamedTuple as _NamedTuple
+from typing_extensions import NamedTuple as _NamedTuple
 
 class Query(_NamedTuple):
   """Query `q` to be run via `conn.execute(*q)`"""
   query: str
   params: list
 
 def quote(unsafe: str) -> str:
```

### Comparing `kv_sqlite_sync-0.1.8/src/kv_sqlite_sync.egg-info/PKG-INFO` & `kv_sqlite_sync-0.1.9/src/kv_sqlite_sync.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: kv-sqlite-sync
-Version: 0.1.8
+Version: 0.1.9
 Summary: Key-Value interface over SQLite. Supports any datatype, including JSON and BLOB
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-storage
 Project-URL: home, https://github.com/moveread/python-storage/tree/main/kv/kv-sqlite-sync
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: kv-api
 Requires-Dist: haskellian
 Requires-Dist: lazy-loader
+Requires-Dist: typing-extensions
 
 # Sqlite Kv (Sync)
 
 > Synchronous Key-Value interface over SQLite. Supports any datatype, including JSON and BLOB
 
 ## Usage
```

