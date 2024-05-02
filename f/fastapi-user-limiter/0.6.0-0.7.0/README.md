# Comparing `tmp/fastapi_user_limiter-0.6.0.tar.gz` & `tmp/fastapi_user_limiter-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_user_limiter-0.6.0.tar", last modified: Thu May  2 10:49:35 2024, max compression
+gzip compressed data, was "fastapi_user_limiter-0.7.0.tar", last modified: Thu May  2 12:06:38 2024, max compression
```

## Comparing `fastapi_user_limiter-0.6.0.tar` & `fastapi_user_limiter-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:49:35.856313 fastapi_user_limiter-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-02 10:49:35.856313 fastapi_user_limiter-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-02 10:49:28.000000 fastapi_user_limiter-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-02 10:49:28.000000 fastapi_user_limiter-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 10:49:35.856313 fastapi_user_limiter-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:49:35.856313 fastapi_user_limiter-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:49:35.856313 fastapi_user_limiter-0.6.0/src/fastapi_user_limiter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:49:28.000000 fastapi_user_limiter-0.6.0/src/fastapi_user_limiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-02 10:49:28.000000 fastapi_user_limiter-0.6.0/src/fastapi_user_limiter/limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:49:35.856313 fastapi_user_limiter-0.6.0/src/fastapi_user_limiter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-02 10:49:35.000000 fastapi_user_limiter-0.6.0/src/fastapi_user_limiter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-02 10:49:35.000000 fastapi_user_limiter-0.6.0/src/fastapi_user_limiter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:49:35.000000 fastapi_user_limiter-0.6.0/src/fastapi_user_limiter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 10:49:35.000000 fastapi_user_limiter-0.6.0/src/fastapi_user_limiter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 10:49:35.000000 fastapi_user_limiter-0.6.0/src/fastapi_user_limiter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:06:38.800540 fastapi_user_limiter-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-02 12:06:38.800540 fastapi_user_limiter-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-02 12:06:33.000000 fastapi_user_limiter-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-02 12:06:33.000000 fastapi_user_limiter-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 12:06:38.800540 fastapi_user_limiter-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:06:38.800540 fastapi_user_limiter-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:06:38.800540 fastapi_user_limiter-0.7.0/src/fastapi_user_limiter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:06:33.000000 fastapi_user_limiter-0.7.0/src/fastapi_user_limiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-02 12:06:33.000000 fastapi_user_limiter-0.7.0/src/fastapi_user_limiter/limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:06:38.800540 fastapi_user_limiter-0.7.0/src/fastapi_user_limiter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-02 12:06:38.000000 fastapi_user_limiter-0.7.0/src/fastapi_user_limiter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-02 12:06:38.000000 fastapi_user_limiter-0.7.0/src/fastapi_user_limiter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:06:38.000000 fastapi_user_limiter-0.7.0/src/fastapi_user_limiter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 12:06:38.000000 fastapi_user_limiter-0.7.0/src/fastapi_user_limiter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 12:06:38.000000 fastapi_user_limiter-0.7.0/src/fastapi_user_limiter.egg-info/top_level.txt
```

### Comparing `fastapi_user_limiter-0.6.0/PKG-INFO` & `fastapi_user_limiter-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_user_limiter
-Version: 0.6.0
+Version: 0.7.0
 Summary: Rate-limiter for FastAPI with the possibility of user-based rate limits
 Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/fastapi-user-limiter
 Project-URL: Bug Tracker, https://github.com/epflgraph/fastapi-user-limiter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fastapi_user_limiter-0.6.0/README.md` & `fastapi_user_limiter-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_user_limiter-0.6.0/pyproject.toml` & `fastapi_user_limiter-0.7.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastapi_user_limiter"
-version = "0.6.0"
+version = "0.7.0"
 authors = [
   { name="Ramtin Yazdanian", email="ramtin.yazdanian@epfl.ch" }
 ]
 description = "Rate-limiter for FastAPI with the possibility of user-based rate limits"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `fastapi_user_limiter-0.6.0/src/fastapi_user_limiter/limiter.py` & `fastapi_user_limiter-0.7.0/src/fastapi_user_limiter/limiter.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         self.redis = None
 
     async def init_redis(self):
         """
         Initializes the Redis connection
         :return: None
         """
-        if self.redis is None or not await self.redis.ping():
+        if self.redis is None:
             self.redis = await redis.from_url(self.redis_url)
 
     async def is_rate_limited(self, key: str, max_requests: int, window: int) -> bool:
         """
         Given a key (client host + endpoint url), determines whether the rate limit has been reached
         :param key: Key consisting of client host plus endpoint URL
         :param max_requests: Maximum allowed # of requests in the given window
@@ -61,49 +61,60 @@
 
 
 def get_rate_limited_message(max_requests, window):
     return (f"Too many requests, no more than {max_requests} requests "
             f"are allowed every {window} seconds.")
 
 
-def rate_limiter(rl: Union[RateLimiterConnection, None] = None,
-                 max_requests: Union[int, None] = 10, window: Union[int, None] = 1,
-                 path: Union[str, None] = None, user: Union[Callable, None] = None):
+def rate_limiter(max_requests: Union[int, None] = 10, window: Union[int, None] = 1,
+                 path: Union[str, None] = None, user: Union[Callable, None] = None,
+                 redis_url: Union[str, None] = None):
     """
     Rate limiter dependency for FastAPI
-    :param rl: RateLimiterConnection object, used for lookup on Redis
     :param max_requests: Max # of requests in given time window
     :param window: Time window in seconds
     :param path: Custom path.
                  Can be used for a router-wide (or even API-wide) rate limit that applies to all
                  endpoints together, rather than each endpoint separately. For such a use case,
                  the dependency should be placed in the router or app constructor call, preferably
                  with the path parameter being equal to the router's prefix (for readability).
                  If None, the path of the request URL is used, creating a per-endpoint limit.
     :param user: Custom user callable.
                  Can be used with a custom callable that extracts the username from request header
                  in order to have a per-user rate-limit, rather than per-IP.
                  If None, the host of the client is used as the username.
-    :return: Rate limiting callable to be used as FastAPI dependency
+    :param redis_url: URL for Redis server
+    :return: Rate limiting async callable to be used as FastAPI dependency
     """
     async def _rate_limit(request: Request):
+        rlc = RateLimiterConnection(redis_url)
         # Providing a None value for either window or max_requests disables rate limiting
-        if rl is None or max_requests is None or window is None:
+        if max_requests is None or window is None:
             return
         # Checking to see if a custom callable has been provided for the username
         if user is None:
             user_name = request.client.host
         else:
             user_name = await user(request.headers)
         # Checking to see if a custom path has been provided
         if path is None:
             path_name = request.url.path
         else:
             path_name = path
         # Generating the redis key
         key = f"rate_limit:{path_name}:{window}:{max_requests}:{user_name}"
-        if await rl.is_rate_limited(key, max_requests, window):
+        if await rlc.is_rate_limited(key, max_requests, window):
             raise HTTPException(
                 status_code=status.HTTP_429_TOO_MANY_REQUESTS,
                 detail=get_rate_limited_message(max_requests, window)
             )
     return _rate_limit
+
+
+def dummy_rate_limiter():
+    """
+    Dummy rate limiter for pytest dependency override
+    :return: dummy rate limiter async callable
+    """
+    async def _dummy_limiter():
+        return
+    return _dummy_limiter
```

### Comparing `fastapi_user_limiter-0.6.0/src/fastapi_user_limiter.egg-info/PKG-INFO` & `fastapi_user_limiter-0.7.0/src/fastapi_user_limiter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_user_limiter
-Version: 0.6.0
+Version: 0.7.0
 Summary: Rate-limiter for FastAPI with the possibility of user-based rate limits
 Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/fastapi-user-limiter
 Project-URL: Bug Tracker, https://github.com/epflgraph/fastapi-user-limiter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

