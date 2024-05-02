# Comparing `tmp/sbxpy-0.6.1.tar.gz` & `tmp/sbxpy-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbxpy-0.6.1.tar", last modified: Thu Feb  8 16:42:31 2024, max compression
+gzip compressed data, was "sbxpy-0.6.2.tar", last modified: Thu May  2 16:54:53 2024, max compression
```

## Comparing `sbxpy-0.6.1.tar` & `sbxpy-0.6.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:42:31.539734 sbxpy-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-02-08 16:42:21.000000 sbxpy-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-02-08 16:42:31.539734 sbxpy-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-02-08 16:42:21.000000 sbxpy-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:42:31.535734 sbxpy-0.6.1/sbxpy/
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-02-08 16:42:21.000000 sbxpy-0.6.1/sbxpy/QueryBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    34603 2024-02-08 16:42:21.000000 sbxpy-0.6.1/sbxpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:42:31.535734 sbxpy-0.6.1/sbxpy/cache/
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-02-08 16:42:21.000000 sbxpy-0.6.1/sbxpy/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:42:31.535734 sbxpy-0.6.1/sbxpy/domain/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-02-08 16:42:21.000000 sbxpy-0.6.1/sbxpy/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:42:31.535734 sbxpy-0.6.1/sbxpy/sbx/
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-02-08 16:42:21.000000 sbxpy-0.6.1/sbxpy/sbx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:42:31.535734 sbxpy-0.6.1/sbxpy/service/
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-02-08 16:42:21.000000 sbxpy-0.6.1/sbxpy/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-08 16:42:31.535734 sbxpy-0.6.1/sbxpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-02-08 16:42:31.000000 sbxpy-0.6.1/sbxpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-08 16:42:31.000000 sbxpy-0.6.1/sbxpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-08 16:42:31.000000 sbxpy-0.6.1/sbxpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-08 16:42:31.000000 sbxpy-0.6.1/sbxpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-08 16:42:31.000000 sbxpy-0.6.1/sbxpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-08 16:42:31.539734 sbxpy-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-02-08 16:42:21.000000 sbxpy-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:54:53.108827 sbxpy-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-02 16:54:49.000000 sbxpy-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-02 16:54:53.108827 sbxpy-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-02 16:54:49.000000 sbxpy-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:54:53.104827 sbxpy-0.6.2/sbxpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-02 16:54:49.000000 sbxpy-0.6.2/sbxpy/QueryBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34603 2024-05-02 16:54:49.000000 sbxpy-0.6.2/sbxpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:54:53.108827 sbxpy-0.6.2/sbxpy/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-02 16:54:49.000000 sbxpy-0.6.2/sbxpy/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:54:53.108827 sbxpy-0.6.2/sbxpy/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-02 16:54:49.000000 sbxpy-0.6.2/sbxpy/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:54:53.108827 sbxpy-0.6.2/sbxpy/sbx/
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-02 16:54:49.000000 sbxpy-0.6.2/sbxpy/sbx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:54:53.108827 sbxpy-0.6.2/sbxpy/service/
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-02 16:54:49.000000 sbxpy-0.6.2/sbxpy/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:54:53.108827 sbxpy-0.6.2/sbxpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-02 16:54:53.000000 sbxpy-0.6.2/sbxpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-02 16:54:53.000000 sbxpy-0.6.2/sbxpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:54:53.000000 sbxpy-0.6.2/sbxpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-02 16:54:53.000000 sbxpy-0.6.2/sbxpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 16:54:53.000000 sbxpy-0.6.2/sbxpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:54:53.108827 sbxpy-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-02 16:54:49.000000 sbxpy-0.6.2/setup.py
```

### Comparing `sbxpy-0.6.1/LICENSE` & `sbxpy-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sbxpy-0.6.1/PKG-INFO` & `sbxpy-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbxpy
-Version: 0.6.1
+Version: 0.6.2
 Summary: This is the module  create all request used to communicate with SbxCloud
 Home-page: https://github.com/sbxcloud/sbxcloudpython
 Author: Luis Guzmán
 Author-email: lgguzman890414@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sbxpy-0.6.1/sbxpy/QueryBuilder.py` & `sbxpy-0.6.2/sbxpy/QueryBuilder.py`

 * *Files identical despite different names*

### Comparing `sbxpy-0.6.1/sbxpy/__init__.py` & `sbxpy-0.6.2/sbxpy/__init__.py`

 * *Files identical despite different names*

### Comparing `sbxpy-0.6.1/sbxpy/cache/__init__.py` & `sbxpy-0.6.2/sbxpy/cache/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,43 +75,53 @@
         await self.get_connection()
         raw_result = await self._redis.get(key)
         if raw_result is not None:
             result = json.loads(raw_result)
             return result_type(**result)
         return None
 
-    async def set_object(self, key: str, value: CachedType) -> None:
+    async def set_object(self, key: str, value: CachedType, ex: Optional[int] = None) -> None:
         await self.get_connection()
         value_as_json = value.model_dump_json()
-        await self._redis.set(key, value_as_json)
+        if ex is None:
+            await self._redis.set(key, value_as_json)
+        else:
+            await self._redis.set(key, value_as_json, ex=ex)
 
-    async def mset_objects(self, items: Dict[str, CachedType]) -> None:
+    async def mset_objects(self, items: Dict[str, CachedType], ex: Optional[int] = None) -> None:
         await self.get_connection()
         # map as set of key, item
         items_as_json = {key: item.model_dump_json() for key, item in items.items()}
-        await self._redis.mset(items_as_json)
+        if ex is None:
+            await self._redis.mset(items_as_json)
+        else:
+            for key, item in items.items():
+                await self._redis.set(key, item.model_dump_json(), ex=ex)
 
     async def mget_objects(
         self, keys: List[str], result_type: Type[CachedType]
     ) -> Optional[List[CachedType]]:
         await self.get_connection()
         values = await self._redis.mget(*keys)
         return [result_type(**json.loads(value)) if value else None for value in values]
 
     async def push_to_queue(self, queue_name: str, data: CachedType) -> None:
         await self.get_connection()
         tmp_json = data.model_dump_json()
         await self._redis.rpush(queue_name, tmp_json)
 
-    async def set_keys_index(self, index_key: str, keys: List[str]) -> None:
+    async def set_keys_index(self, index_key: str, keys: List[str], ex: Optional[int] = None) -> None:
         """Store a list of keys as index"""
         await self.get_connection()
         # Convert set of keys to string before storing
         keys_as_str = json.dumps(keys)
-        await self._redis.set(index_key, keys_as_str)
+        if ex is None:
+            await self._redis.set(index_key, keys_as_str)
+        else:
+            await self._redis.set(index_key, keys_as_str, ex=ex)
 
     async def get_keys_index(self, index_key: str) -> List[str]:
         """Retrieve a list of keys from index"""
         await self.get_connection()
         keys_as_str = await self._redis.get(index_key)
         # If keys exist, convert from string back to list
         return json.loads(keys_as_str) if keys_as_str else []
```

### Comparing `sbxpy-0.6.1/sbxpy/domain/__init__.py` & `sbxpy-0.6.2/sbxpy/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `sbxpy-0.6.1/sbxpy/sbx/__init__.py` & `sbxpy-0.6.2/sbxpy/sbx/__init__.py`

 * *Files identical despite different names*

### Comparing `sbxpy-0.6.1/sbxpy/service/__init__.py` & `sbxpy-0.6.2/sbxpy/service/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 redis_service = get_redis_service()
 CachedType = TypeVar("CachedType", bound=SBXModel)
 
 
 class SBXCachedService(SBXService):
     @staticmethod
     async def get(
-        key: str, result_type: Type[CachedType], use_cache=True
+        key: str, result_type: Type[CachedType], use_cache=True, ex: Optional[int] = None
     ) -> Optional[CachedType]:
         if not issubclass(result_type, SBXModel) or result_type.get_model() is None:
             logger.error(f"type of {type(result_type)} is not a subclass of SBXModel")
             raise ValueError("result_type must be a subclass of SBXModel")
         keys_idx = f"{result_type.get_model()}:*"
         cache_key = f"sbx:{result_type.get_model()}:{key}"
         cached_keys: Set[str] = set()
@@ -39,31 +39,31 @@
 
         try:
             query = SBXCachedService.find(result_type.get_model())
             query.where_with_keys([key])
             model_instance = SBXResponse(**await query.find()).first(result_type)
 
             if model_instance:
-                await redis_service.set_object(cache_key, model_instance)
+                await redis_service.set_object(cache_key, model_instance, ex)
                 cached_keys.add(key)
                 await redis_service.set_keys_index(
-                    f"{result_type.get_model()}:*", list(cached_keys)
+                    f"{result_type.get_model()}:*", list(cached_keys), ex
                 )
 
             return model_instance
         except Exception as e:
             logger.exception(f"An error occurred while retrieving data: {e}")
             return model_instance
 
         # finally:
         #     await redis_service.close_connection()  # If applicable.
 
     @staticmethod
     async def list(
-        result_type: Type[CachedType], use_cache=True
+        result_type: Type[CachedType], use_cache=True, ex: Optional[int] = None
     ) -> Optional[List[CachedType]]:
         if not issubclass(result_type, SBXModel):
             logger.error(f"type of {type(result_type)} is not a subclass of SBXModel")
             raise ValueError("result_type must be a subclass of SBXModel")
 
         logger.debug(f"Retrieving list of {result_type}")
         keys_idx = f"{result_type.get_model()}:*"
@@ -102,18 +102,18 @@
 
             if model_instances:
                 model_map = {
                     f"sbx:{result_type.get_model()}:{instance.key}": instance
                     for instance in model_instances
                 }
                 # save the items in cache
-                await redis_service.mset_objects(model_map)
+                await redis_service.mset_objects(model_map, ex)
                 # update the index
                 cache_keys = {instance.key for instance in model_instances}
-                await redis_service.set_keys_index(keys_idx, list(cache_keys))
+                await redis_service.set_keys_index(keys_idx, list(cache_keys), ex)
 
             return model_instances
 
         except Exception as e:
             logger.exception(f"An error occurred while retrieving data: {e}")
             return model_instances
         # finally:
```

### Comparing `sbxpy-0.6.1/sbxpy.egg-info/PKG-INFO` & `sbxpy-0.6.2/sbxpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbxpy
-Version: 0.6.1
+Version: 0.6.2
 Summary: This is the module  create all request used to communicate with SbxCloud
 Home-page: https://github.com/sbxcloud/sbxcloudpython
 Author: Luis Guzmán
 Author-email: lgguzman890414@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sbxpy-0.6.1/setup.py` & `sbxpy-0.6.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sbxpy",
-    version="0.6.1",
+    version="0.6.2",
     author="Luis Guzmán",
     author_email="lgguzman890414@gmail.com",
     description="This is the module  create all request used to communicate with SbxCloud",
     long_description="This is the module  create all request used to communicate with SbxCloud",
     long_description_content_type="text/markdown",
     url="https://github.com/sbxcloud/sbxcloudpython",
     packages=setuptools.find_packages(),
```

