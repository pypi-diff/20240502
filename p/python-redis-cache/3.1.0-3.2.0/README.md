# Comparing `tmp/python-redis-cache-3.1.0.tar.gz` & `tmp/python_redis_cache-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-redis-cache-3.1.0.tar", last modified: Thu Mar 21 02:25:44 2024, max compression
+gzip compressed data, was "python_redis_cache-3.2.0.tar", last modified: Thu May  2 16:33:40 2024, max compression
```

## Comparing `python-redis-cache-3.1.0.tar` & `python_redis_cache-3.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 02:25:44.961742 python-redis-cache-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-21 02:25:34.000000 python-redis-cache-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-03-21 02:25:44.961742 python-redis-cache-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-03-21 02:25:34.000000 python-redis-cache-3.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-21 02:25:34.000000 python-redis-cache-3.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 02:25:44.961742 python-redis-cache-3.1.0/python_redis_cache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-03-21 02:25:44.000000 python-redis-cache-3.1.0/python_redis_cache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-21 02:25:44.000000 python-redis-cache-3.1.0/python_redis_cache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 02:25:44.000000 python-redis-cache-3.1.0/python_redis_cache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-21 02:25:44.000000 python-redis-cache-3.1.0/python_redis_cache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-21 02:25:44.000000 python-redis-cache-3.1.0/python_redis_cache.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 02:25:44.961742 python-redis-cache-3.1.0/redis_cache/
--rw-r--r--   0 runner    (1001) docker     (127)     9482 2024-03-21 02:25:34.000000 python-redis-cache-3.1.0/redis_cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-21 02:25:44.961742 python-redis-cache-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-21 02:25:35.000000 python-redis-cache-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 02:25:44.961742 python-redis-cache-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10713 2024-03-21 02:25:34.000000 python-redis-cache-3.1.0/tests/test_redis_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:40.423105 python_redis_cache-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-02 16:33:33.000000 python_redis_cache-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-02 16:33:40.423105 python_redis_cache-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-05-02 16:33:33.000000 python_redis_cache-3.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-02 16:33:33.000000 python_redis_cache-3.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:40.423105 python_redis_cache-3.2.0/python_redis_cache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-05-02 16:33:40.000000 python_redis_cache-3.2.0/python_redis_cache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-02 16:33:40.000000 python_redis_cache-3.2.0/python_redis_cache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:33:40.000000 python_redis_cache-3.2.0/python_redis_cache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 16:33:40.000000 python_redis_cache-3.2.0/python_redis_cache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 16:33:40.000000 python_redis_cache-3.2.0/python_redis_cache.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:40.419105 python_redis_cache-3.2.0/redis_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     9752 2024-05-02 16:33:33.000000 python_redis_cache-3.2.0/redis_cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-02 16:33:40.423105 python_redis_cache-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-02 16:33:33.000000 python_redis_cache-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:33:40.423105 python_redis_cache-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11126 2024-05-02 16:33:33.000000 python_redis_cache-3.2.0/tests/test_redis_cache.py
```

### Comparing `python-redis-cache-3.1.0/LICENSE` & `python_redis_cache-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-redis-cache-3.1.0/PKG-INFO` & `python_redis_cache-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-redis-cache
-Version: 3.1.0
+Version: 3.2.0
 Summary: Basic Redis caching for functions
 Home-page: http://github.com/taylorhakes/python-redis-cache
 Author: Taylor Hakes
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -79,14 +79,16 @@
 
 - prefix - The string to prefix the redis keys with
 - serializer/deserializer - functions to convert arguments and return value to a string (user JSON by default)
 - ttl - The time in seconds to cache the return value
 - namespace - The string namespace of the cache. This is useful for allowing multiple functions to use the same cache. By default its `f'{function.__module__}.{function.__file__}'`
 - exception_handler - Function to handle Redis cache exceptions. This allows you to fall back to calling the original function or logging exceptions. Function has the following signature `exception_handler(exception: Exception, function: Callable, args: List, kwargs: Dict) -> Any`. If using this handler, reraise the exception in the handler to stop execution of the function. All return results will be used even if `None`. If handler not defined, it will raise the exception and not call the original function.
 - support_cluster - Set to False to disable the `{` prefix on the keys. This is NOT recommended. See below for more info.
+- active - Optional flag to disable the caching completly for troubleshooting/lower environments
+
 
 ## Limitations and things to know
 Arguments and return types must be JSON serializable by default. You can override the serializer, but be careful with using Pickle. Make sure you understand the security risks. Pickle should not be used with untrusted values.
 https://security.stackexchange.com/questions/183966/safely-load-a-pickle-file
 `decode_responses` parameter must be `False` in redis client if you use pickle.
 
 - **ttl** - is based on the time from when it's first inserted in the cache, not based on the last access
```

### Comparing `python-redis-cache-3.1.0/README.md` & `python_redis_cache-3.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,16 @@
 
 - prefix - The string to prefix the redis keys with
 - serializer/deserializer - functions to convert arguments and return value to a string (user JSON by default)
 - ttl - The time in seconds to cache the return value
 - namespace - The string namespace of the cache. This is useful for allowing multiple functions to use the same cache. By default its `f'{function.__module__}.{function.__file__}'`
 - exception_handler - Function to handle Redis cache exceptions. This allows you to fall back to calling the original function or logging exceptions. Function has the following signature `exception_handler(exception: Exception, function: Callable, args: List, kwargs: Dict) -> Any`. If using this handler, reraise the exception in the handler to stop execution of the function. All return results will be used even if `None`. If handler not defined, it will raise the exception and not call the original function.
 - support_cluster - Set to False to disable the `{` prefix on the keys. This is NOT recommended. See below for more info.
+- active - Optional flag to disable the caching completly for troubleshooting/lower environments
+
 
 ## Limitations and things to know
 Arguments and return types must be JSON serializable by default. You can override the serializer, but be careful with using Pickle. Make sure you understand the security risks. Pickle should not be used with untrusted values.
 https://security.stackexchange.com/questions/183966/safely-load-a-pickle-file
 `decode_responses` parameter must be `False` in redis client if you use pickle.
 
 - **ttl** - is based on the time from when it's first inserted in the cache, not based on the last access
```

### Comparing `python-redis-cache-3.1.0/python_redis_cache.egg-info/PKG-INFO` & `python_redis_cache-3.2.0/python_redis_cache.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-redis-cache
-Version: 3.1.0
+Version: 3.2.0
 Summary: Basic Redis caching for functions
 Home-page: http://github.com/taylorhakes/python-redis-cache
 Author: Taylor Hakes
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -79,14 +79,16 @@
 
 - prefix - The string to prefix the redis keys with
 - serializer/deserializer - functions to convert arguments and return value to a string (user JSON by default)
 - ttl - The time in seconds to cache the return value
 - namespace - The string namespace of the cache. This is useful for allowing multiple functions to use the same cache. By default its `f'{function.__module__}.{function.__file__}'`
 - exception_handler - Function to handle Redis cache exceptions. This allows you to fall back to calling the original function or logging exceptions. Function has the following signature `exception_handler(exception: Exception, function: Callable, args: List, kwargs: Dict) -> Any`. If using this handler, reraise the exception in the handler to stop execution of the function. All return results will be used even if `None`. If handler not defined, it will raise the exception and not call the original function.
 - support_cluster - Set to False to disable the `{` prefix on the keys. This is NOT recommended. See below for more info.
+- active - Optional flag to disable the caching completly for troubleshooting/lower environments
+
 
 ## Limitations and things to know
 Arguments and return types must be JSON serializable by default. You can override the serializer, but be careful with using Pickle. Make sure you understand the security risks. Pickle should not be used with untrusted values.
 https://security.stackexchange.com/questions/183966/safely-load-a-pickle-file
 `decode_responses` parameter must be `False` in redis client if you use pickle.
 
 - **ttl** - is based on the time from when it's first inserted in the cache, not based on the last access
```

### Comparing `python-redis-cache-3.1.0/redis_cache/__init__.py` & `python_redis_cache-3.2.0/redis_cache/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,35 +95,37 @@
         if not len(elements):
             break
 
         yield elements
 
 
 class RedisCache:
-    def __init__(self, redis_client, prefix="rc", serializer=compact_dump, deserializer=loads, key_serializer=None, support_cluster=True, exception_handler=None):
+    def __init__(self, redis_client, prefix="rc", serializer=compact_dump, deserializer=loads, key_serializer=None, support_cluster=True, exception_handler=None, active:bool=True):
         self.client = redis_client
         self.prefix = prefix
         self.serializer = serializer
         self.deserializer = deserializer
         self.key_serializer = key_serializer
         self.exception_handler = exception_handler
         self.support_cluster = support_cluster
+        self.active = active
 
     def cache(self, ttl=0, limit=0, namespace=None, exception_handler=None):
         return CacheDecorator(
             redis_client=self.client,
             prefix=self.prefix,
             serializer=self.serializer,
             deserializer=self.deserializer,
             key_serializer=self.key_serializer,
             ttl=ttl,
             limit=limit,
             namespace=namespace,
             support_cluster=self.support_cluster,
-            exception_handler=exception_handler or self.exception_handler
+            exception_handler=exception_handler or self.exception_handler,
+            active=self.active
         )
 
     def mget(self, *fns_with_args):
         keys = []
         for fn_and_args in fns_with_args:
             fn = fn_and_args['fn']
             args = fn_and_args['args'] if 'args' in fn_and_args else []
@@ -151,27 +153,28 @@
             deserialized_results.append(result)
 
         if needs_pipeline:
             pipeline.execute()
         return deserialized_results
 
 class CacheDecorator:
-    def __init__(self, redis_client, prefix="rc", serializer=compact_dump, deserializer=loads, key_serializer=None, ttl=0, limit=0, namespace=None, support_cluster=True, exception_handler=None):
+    def __init__(self, redis_client, prefix="rc", serializer=compact_dump, deserializer=loads, key_serializer=None, ttl=0, limit=0, namespace=None, support_cluster=True, exception_handler=None, active:bool=True):
         self.client = redis_client
         self.prefix = prefix
         self.serializer = serializer
         self.key_serializer = key_serializer
         self.deserializer = deserializer
         self.ttl = ttl
         self.limit = limit
         self.namespace = namespace
         self.exception_handler = exception_handler
         self.support_cluster = support_cluster
         self.keys_key = None
         self.original_fn = None
+        self.active=active
 
 
     def get_full_prefix(self):
         if self.support_cluster:
             # Redis cluster requires keys operated in batch to be in the same key space. Redis cluster hashes the keys to
             # determine the key space. The braces specify which part of the key to hash (instead of the whole key).
             # See https://github.com/taylorhakes/python-redis-cache/issues/29  The `{prefix}:keys` and `{prefix}:args`
@@ -200,14 +203,17 @@
         self.namespace = self.namespace or f'{fn.__module__}.{fn.__qualname__}'
         self.keys_key = f'{self.get_full_prefix()}:keys'
         self.original_fn = fn
 
         @wraps(fn)
         def inner(*args, **kwargs):
             nonlocal self
+            # Return the original function if we're not in active mode
+            if not self.active:
+                return fn(*args, **kwargs)
             key = self.get_key(args, kwargs)
             result = None
 
             exception_handled = False
             try:
                 result = self.client.get(key)
             except Exception as e:
```

### Comparing `python-redis-cache-3.1.0/setup.py` & `python_redis_cache-3.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
-__version__ = "3.1.0"
+__version__ = "3.2.0"
 
 setup(
     name='python-redis-cache',
     version=__version__,
     description='Basic Redis caching for functions',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

### Comparing `python-redis-cache-3.1.0/tests/test_redis_cache.py` & `python_redis_cache-3.2.0/tests/test_redis_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 
 
 @pytest.fixture()
 def cache():
     return RedisCache(redis_client=client)
 
 
+@pytest.fixture()
+def inactive_cache():
+    return RedisCache(redis_client=client, active=False)
+
 def add_func(n1, n2):
     """ Add function
     Add n1 to n2 and return a uuid4 unique verifier
 
     Returns:
         tuple(int, str(uuid.uuid4))
     """
@@ -62,14 +66,25 @@
     time.sleep(2)
 
     r_3, v_3 = add_ttl(3, 4)
 
     assert 7 == r_1 == r_2 == r_3
     assert v_1 == v_2 != v_3
 
+def test_inactive_cache(inactive_cache):
+    @inactive_cache.cache(ttl=2)
+    def add_ttl(arg1, arg2):
+        return add_func(arg1, arg2)
+
+    r_1, v_1 = add_ttl(3, 4)
+    r_2, v_2 = add_ttl(3, 4)
+
+    assert 7 == r_1 == r_2
+    # In inactive scenario the calls should return different uuids
+    assert v_1 != v_2
 
 def test_limit(cache):
     @cache.cache(limit=2)
     def add_limit(arg1, arg2):
         return add_func(arg1, arg2)
 
     r_3_4, v_3_4 = add_limit(3, 4)
```

