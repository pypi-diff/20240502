# Comparing `tmp/llama_index_storage_kvstore_redis-0.1.3.tar.gz` & `tmp/llama_index_storage_kvstore_redis-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_storage_kvstore_redis-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_storage_kvstore_redis-0.1.4.tar", max compression
```

## Comparing `llama_index_storage_kvstore_redis-0.1.3.tar` & `llama_index_storage_kvstore_redis-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       48 2024-03-27 17:50:41.886051 llama_index_storage_kvstore_redis-0.1.3/README.md
--rw-r--r--   0        0        0       92 2024-03-27 17:50:41.886051 llama_index_storage_kvstore_redis-0.1.3/llama_index/storage/kvstore/redis/__init__.py
--rw-r--r--   0        0        0     5310 2024-03-27 17:50:41.886051 llama_index_storage_kvstore_redis-0.1.3/llama_index/storage/kvstore/redis/base.py
--rw-r--r--   0        0        0     1466 2024-03-27 17:50:41.886051 llama_index_storage_kvstore_redis-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 llama_index_storage_kvstore_redis-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       48 2024-05-02 03:23:50.241930 llama_index_storage_kvstore_redis-0.1.4/README.md
+-rw-r--r--   0        0        0       92 2024-05-02 03:23:50.241930 llama_index_storage_kvstore_redis-0.1.4/llama_index/storage/kvstore/redis/__init__.py
+-rw-r--r--   0        0        0     5319 2024-05-02 03:23:50.241930 llama_index_storage_kvstore_redis-0.1.4/llama_index/storage/kvstore/redis/base.py
+-rw-r--r--   0        0        0     1466 2024-05-02 03:23:50.241930 llama_index_storage_kvstore_redis-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 llama_index_storage_kvstore_redis-0.1.4/PKG-INFO
```

### Comparing `llama_index_storage_kvstore_redis-0.1.3/llama_index/storage/kvstore/redis/base.py` & `llama_index_storage_kvstore_redis-0.1.4/llama_index/storage/kvstore/redis/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         raise NotImplementedError
 
     def get_all(self, collection: str = DEFAULT_COLLECTION) -> Dict[str, dict]:
         """Get all values from the store."""
         collection_kv_dict = {}
         for key, val_str in self._redis_client.hscan_iter(name=collection):
             value = dict(json.loads(val_str))
-            collection_kv_dict[key] = value
+            collection_kv_dict[key.decode()] = value
         return collection_kv_dict
 
     async def aget_all(self, collection: str = DEFAULT_COLLECTION) -> Dict[str, dict]:
         """Get all values from the store."""
         raise NotImplementedError
 
     def delete(self, key: str, collection: str = DEFAULT_COLLECTION) -> bool:
```

### Comparing `llama_index_storage_kvstore_redis-0.1.3/pyproject.toml` & `llama_index_storage_kvstore_redis-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index kvstore redis integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-storage-kvstore-redis"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 redis = "^5.0.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_storage_kvstore_redis-0.1.3/PKG-INFO` & `llama_index_storage_kvstore_redis-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-storage-kvstore-redis
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index kvstore redis integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

