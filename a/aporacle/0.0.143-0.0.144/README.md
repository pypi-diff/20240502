# Comparing `tmp/aporacle-0.0.143.tar.gz` & `tmp/aporacle-0.0.144.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aporacle-0.0.143.tar", max compression
+gzip compressed data, was "aporacle-0.0.144.tar", max compression
```

## Comparing `aporacle-0.0.143.tar` & `aporacle-0.0.144.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        0 2024-02-28 04:02:27.389085 aporacle-0.0.143/README.md
--rw-r--r--   0        0        0      265 2024-03-20 16:45:48.348259 aporacle-0.0.143/aporacle/__init__.py
--rw-r--r--   0        0        0     1717 2024-03-26 04:23:06.584243 aporacle-0.0.143/aporacle/broadcast/__init__.py
--rw-r--r--   0        0        0     2834 2024-03-26 04:26:39.150092 aporacle-0.0.143/aporacle/conf/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 16:41:03.985547 aporacle-0.0.143/aporacle/core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 16:41:11.733621 aporacle-0.0.143/aporacle/core/utils/__init__.py
--rw-r--r--   0        0        0     4383 2024-03-20 16:45:48.336259 aporacle-0.0.143/aporacle/core/utils/async_call_scheduler.py
--rw-r--r--   0        0        0        0 2024-03-10 13:49:56.523746 aporacle-0.0.143/aporacle/data/__init__.py
--rw-r--r--   0        0        0      589 2024-03-11 05:27:14.610597 aporacle-0.0.143/aporacle/data/asset/__init__.py
--rw-r--r--   0        0        0     1543 2024-04-19 13:19:36.337225 aporacle-0.0.143/aporacle/data/combination.py
--rw-r--r--   0        0        0        0 2024-03-10 13:50:08.923807 aporacle-0.0.143/aporacle/data/db/__init__.py
--rw-r--r--   0        0        0      684 2024-03-18 04:25:23.973270 aporacle-0.0.143/aporacle/data/db/crud.py
--rw-r--r--   0        0        0      869 2024-04-19 06:59:59.684489 aporacle-0.0.143/aporacle/data/feed_results.py
--rw-r--r--   0        0        0    10186 2024-04-19 06:26:40.918071 aporacle-0.0.143/aporacle/data/gcp/__init__.py
--rw-r--r--   0        0        0      615 2024-03-18 04:07:19.874287 aporacle-0.0.143/aporacle/data/symbols/__init__.py
--rw-r--r--   0        0        0        0 2024-03-11 16:12:22.030426 aporacle-0.0.143/aporacle/execution/__init__.py
--rw-r--r--   0        0        0     6128 2024-04-24 13:10:14.487265 aporacle-0.0.143/aporacle/execution/executables.py
--rw-r--r--   0        0        0        0 2024-03-20 16:39:34.468697 aporacle-0.0.143/aporacle/network/__init__.py
--rw-r--r--   0        0        0     4316 2024-03-12 15:57:25.236568 aporacle-0.0.143/aporacle/network/network_base.py
--rw-r--r--   0        0        0     1583 2024-03-11 12:44:12.298311 aporacle-0.0.143/aporacle/shared_setup.py
--rw-r--r--   0        0        0      399 2024-04-24 13:10:14.471265 aporacle-0.0.143/pyproject.toml
--rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 aporacle-0.0.143/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-28 04:02:27.389085 aporacle-0.0.144/README.md
+-rw-r--r--   0        0        0      265 2024-03-20 16:45:48.348259 aporacle-0.0.144/aporacle/__init__.py
+-rw-r--r--   0        0        0     1717 2024-03-26 04:23:06.584243 aporacle-0.0.144/aporacle/broadcast/__init__.py
+-rw-r--r--   0        0        0     2834 2024-03-26 04:26:39.150092 aporacle-0.0.144/aporacle/conf/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:03.985547 aporacle-0.0.144/aporacle/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:41:11.733621 aporacle-0.0.144/aporacle/core/utils/__init__.py
+-rw-r--r--   0        0        0     4383 2024-03-20 16:45:48.336259 aporacle-0.0.144/aporacle/core/utils/async_call_scheduler.py
+-rw-r--r--   0        0        0        0 2024-03-10 13:49:56.523746 aporacle-0.0.144/aporacle/data/__init__.py
+-rw-r--r--   0        0        0      589 2024-03-11 05:27:14.610597 aporacle-0.0.144/aporacle/data/asset/__init__.py
+-rw-r--r--   0        0        0     1543 2024-04-19 13:19:36.337225 aporacle-0.0.144/aporacle/data/combination.py
+-rw-r--r--   0        0        0        0 2024-03-10 13:50:08.923807 aporacle-0.0.144/aporacle/data/db/__init__.py
+-rw-r--r--   0        0        0      740 2024-05-01 06:22:52.954534 aporacle-0.0.144/aporacle/data/db/crud.py
+-rw-r--r--   0        0        0      869 2024-04-19 06:59:59.684489 aporacle-0.0.144/aporacle/data/feed_results.py
+-rw-r--r--   0        0        0    10186 2024-04-19 06:26:40.918071 aporacle-0.0.144/aporacle/data/gcp/__init__.py
+-rw-r--r--   0        0        0      615 2024-03-18 04:07:19.874287 aporacle-0.0.144/aporacle/data/symbols/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-11 16:12:22.030426 aporacle-0.0.144/aporacle/execution/__init__.py
+-rw-r--r--   0        0        0     6088 2024-04-24 13:11:21.215856 aporacle-0.0.144/aporacle/execution/executables.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:39:34.468697 aporacle-0.0.144/aporacle/network/__init__.py
+-rw-r--r--   0        0        0     4316 2024-03-12 15:57:25.236568 aporacle-0.0.144/aporacle/network/network_base.py
+-rw-r--r--   0        0        0     1583 2024-03-11 12:44:12.298311 aporacle-0.0.144/aporacle/shared_setup.py
+-rw-r--r--   0        0        0      399 2024-05-01 11:10:29.392282 aporacle-0.0.144/pyproject.toml
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 aporacle-0.0.144/PKG-INFO
```

### Comparing `aporacle-0.0.143/aporacle/broadcast/__init__.py` & `aporacle-0.0.144/aporacle/broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.143/aporacle/conf/__init__.py` & `aporacle-0.0.144/aporacle/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.143/aporacle/core/utils/async_call_scheduler.py` & `aporacle-0.0.144/aporacle/core/utils/async_call_scheduler.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.143/aporacle/data/asset/__init__.py` & `aporacle-0.0.144/aporacle/data/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.143/aporacle/data/combination.py` & `aporacle-0.0.144/aporacle/data/combination.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.143/aporacle/data/db/crud.py` & `aporacle-0.0.144/aporacle/data/db/crud.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,12 +4,15 @@
 class Crud(MongoDBReaderWriter):
     def __init__(self, uri: str, db_name: str):
         super().__init__(uri, db_name)
 
     def write_to_database(self, collection=None, data=None):
         assert collection is not None, "Collection cannot be None"
         assert data is not None, "Data cannot be None"
+        assert len(data) > 0, "Data cannot be empty."
         return self.write(collection=collection, data=data)
 
     def read_from_data(self, collection=None, filters=None, omit=None, limit: int = 1000000):
         assert collection is not None, "Collection cannot be None"
         return self.read(collection=collection, filters=filters, omit=omit, limit=limit)
+
+
```

### Comparing `aporacle-0.0.143/aporacle/data/feed_results.py` & `aporacle-0.0.144/aporacle/data/feed_results.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.143/aporacle/data/gcp/__init__.py` & `aporacle-0.0.144/aporacle/data/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.143/aporacle/data/symbols/__init__.py` & `aporacle-0.0.144/aporacle/data/symbols/__init__.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.143/aporacle/execution/executables.py` & `aporacle-0.0.144/aporacle/execution/executables.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,14 @@
         self._epoch_scheduler_task: Optional[asyncio.Task] = None
         self._ws_listener_task: Optional[asyncio.Task] = None
 
     @property
     def name(self):
         return "voting_round_executable"
 
-    def initialize(self):
-        pass
-
     def start_network(self):
         raise NotImplementedError
 
     def stop_network(self):
         raise NotImplementedError
 
     async def start(self):
```

### Comparing `aporacle-0.0.143/aporacle/network/network_base.py` & `aporacle-0.0.144/aporacle/network/network_base.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.143/aporacle/shared_setup.py` & `aporacle-0.0.144/aporacle/shared_setup.py`

 * *Files identical despite different names*

### Comparing `aporacle-0.0.143/PKG-INFO` & `aporacle-0.0.144/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: aporacle
-Version: 0.0.143
+Version: 0.0.144
 Summary: 
 Author: Makhosonke Morafo
 Author-email: makhosonke@komokun.org
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: cachetools (>=5.3.3,<6.0.0)
 Requires-Dist: google-cloud-storage (>=2.16.0,<3.0.0)
-Requires-Dist: komoutils (>=0.0.224,<0.0.225)
+Requires-Dist: komoutils (>=0.0.225,<0.0.226)
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Requires-Dist: schedule (>=1.2.1,<2.0.0)
 Description-Content-Type: text/markdown
```

