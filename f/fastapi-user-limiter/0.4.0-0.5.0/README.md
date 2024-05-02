# Comparing `tmp/fastapi_user_limiter-0.4.0.tar.gz` & `tmp/fastapi_user_limiter-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_user_limiter-0.4.0.tar", last modified: Wed May  1 12:56:24 2024, max compression
+gzip compressed data, was "fastapi_user_limiter-0.5.0.tar", last modified: Thu May  2 10:40:23 2024, max compression
```

## Comparing `fastapi_user_limiter-0.4.0.tar` & `fastapi_user_limiter-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:56:24.179909 fastapi_user_limiter-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-01 12:56:24.175909 fastapi_user_limiter-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-01 12:56:18.000000 fastapi_user_limiter-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-01 12:56:18.000000 fastapi_user_limiter-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:56:24.179909 fastapi_user_limiter-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:56:24.175909 fastapi_user_limiter-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:56:24.175909 fastapi_user_limiter-0.4.0/src/fastapi_user_limiter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:56:18.000000 fastapi_user_limiter-0.4.0/src/fastapi_user_limiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-01 12:56:18.000000 fastapi_user_limiter-0.4.0/src/fastapi_user_limiter/limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:56:24.175909 fastapi_user_limiter-0.4.0/src/fastapi_user_limiter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-01 12:56:24.000000 fastapi_user_limiter-0.4.0/src/fastapi_user_limiter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 12:56:24.000000 fastapi_user_limiter-0.4.0/src/fastapi_user_limiter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:56:24.000000 fastapi_user_limiter-0.4.0/src/fastapi_user_limiter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 12:56:24.000000 fastapi_user_limiter-0.4.0/src/fastapi_user_limiter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 12:56:24.000000 fastapi_user_limiter-0.4.0/src/fastapi_user_limiter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:40:23.398357 fastapi_user_limiter-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-02 10:40:23.398357 fastapi_user_limiter-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-02 10:40:15.000000 fastapi_user_limiter-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-02 10:40:15.000000 fastapi_user_limiter-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 10:40:23.398357 fastapi_user_limiter-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:40:23.394358 fastapi_user_limiter-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:40:23.394358 fastapi_user_limiter-0.5.0/src/fastapi_user_limiter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:40:15.000000 fastapi_user_limiter-0.5.0/src/fastapi_user_limiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-05-02 10:40:15.000000 fastapi_user_limiter-0.5.0/src/fastapi_user_limiter/limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:40:23.398357 fastapi_user_limiter-0.5.0/src/fastapi_user_limiter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-02 10:40:23.000000 fastapi_user_limiter-0.5.0/src/fastapi_user_limiter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-02 10:40:23.000000 fastapi_user_limiter-0.5.0/src/fastapi_user_limiter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:40:23.000000 fastapi_user_limiter-0.5.0/src/fastapi_user_limiter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 10:40:23.000000 fastapi_user_limiter-0.5.0/src/fastapi_user_limiter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 10:40:23.000000 fastapi_user_limiter-0.5.0/src/fastapi_user_limiter.egg-info/top_level.txt
```

### Comparing `fastapi_user_limiter-0.4.0/PKG-INFO` & `fastapi_user_limiter-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_user_limiter
-Version: 0.4.0
+Version: 0.5.0
 Summary: Rate-limiter for FastAPI with the possibility of user-based rate limits
 Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/fastapi-user-limiter
 Project-URL: Bug Tracker, https://github.com/epflgraph/fastapi-user-limiter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fastapi_user_limiter-0.4.0/README.md` & `fastapi_user_limiter-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_user_limiter-0.4.0/pyproject.toml` & `fastapi_user_limiter-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastapi_user_limiter"
-version = "0.4.0"
+version = "0.5.0"
 authors = [
   { name="Ramtin Yazdanian", email="ramtin.yazdanian@epfl.ch" }
 ]
 description = "Rate-limiter for FastAPI with the possibility of user-based rate limits"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `fastapi_user_limiter-0.4.0/src/fastapi_user_limiter/limiter.py` & `fastapi_user_limiter-0.5.0/src/fastapi_user_limiter/limiter.py`

 * *Files 8% similar despite different names*

```diff
@@ -61,16 +61,16 @@
 
 
 def get_rate_limited_message(max_requests, window):
     return (f"Too many requests, no more than {max_requests} requests "
             f"are allowed every {window} seconds.")
 
 
-def rate_limiter(rl: RateLimiterConnection,
-                 max_requests: Union[int, None], window: Union[int, None],
+def rate_limiter(rl: Union[RateLimiterConnection, None] = None,
+                 max_requests: Union[int, None] = 10, window: Union[int, None] = 1,
                  path: Union[str, None] = None, user: Union[Callable, None] = None):
     """
     Rate limiter dependency for FastAPI
     :param rl: RateLimiterConnection object, used for lookup on Redis
     :param max_requests: Max # of requests in given time window
     :param window: Time window in seconds
     :param path: Custom path.
@@ -83,15 +83,15 @@
                  Can be used with a custom callable that extracts the username from request header
                  in order to have a per-user rate-limit, rather than per-IP.
                  If None, the host of the client is used as the username.
     :return: Rate limiting callable to be used as FastAPI dependency
     """
     async def _rate_limit(request: Request):
         # Providing a None value for either window or max_requests disables rate limiting
-        if max_requests is None or window is None:
+        if rl is None or max_requests is None or window is None:
             return
         # Checking to see if a custom callable has been provided for the username
         if user is None:
             user_name = request.client.host
         else:
             user_name = user(request.headers)
         # Checking to see if a custom path has been provided
```

### Comparing `fastapi_user_limiter-0.4.0/src/fastapi_user_limiter.egg-info/PKG-INFO` & `fastapi_user_limiter-0.5.0/src/fastapi_user_limiter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_user_limiter
-Version: 0.4.0
+Version: 0.5.0
 Summary: Rate-limiter for FastAPI with the possibility of user-based rate limits
 Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/fastapi-user-limiter
 Project-URL: Bug Tracker, https://github.com/epflgraph/fastapi-user-limiter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

