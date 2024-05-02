# Comparing `tmp/fastapi_user_limiter-0.5.0.tar.gz` & `tmp/fastapi_user_limiter-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_user_limiter-0.5.0.tar", last modified: Thu May  2 10:40:23 2024, max compression
+gzip compressed data, was "fastapi_user_limiter-0.6.0.tar", last modified: Thu May  2 10:49:35 2024, max compression
```

## Comparing `fastapi_user_limiter-0.5.0.tar` & `fastapi_user_limiter-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:40:23.398357 fastapi_user_limiter-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-02 10:40:23.398357 fastapi_user_limiter-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-02 10:40:15.000000 fastapi_user_limiter-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-02 10:40:15.000000 fastapi_user_limiter-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 10:40:23.398357 fastapi_user_limiter-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:40:23.394358 fastapi_user_limiter-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:40:23.394358 fastapi_user_limiter-0.5.0/src/fastapi_user_limiter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:40:15.000000 fastapi_user_limiter-0.5.0/src/fastapi_user_limiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-05-02 10:40:15.000000 fastapi_user_limiter-0.5.0/src/fastapi_user_limiter/limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:40:23.398357 fastapi_user_limiter-0.5.0/src/fastapi_user_limiter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-02 10:40:23.000000 fastapi_user_limiter-0.5.0/src/fastapi_user_limiter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-02 10:40:23.000000 fastapi_user_limiter-0.5.0/src/fastapi_user_limiter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:40:23.000000 fastapi_user_limiter-0.5.0/src/fastapi_user_limiter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 10:40:23.000000 fastapi_user_limiter-0.5.0/src/fastapi_user_limiter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 10:40:23.000000 fastapi_user_limiter-0.5.0/src/fastapi_user_limiter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:49:35.856313 fastapi_user_limiter-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-02 10:49:35.856313 fastapi_user_limiter-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-02 10:49:28.000000 fastapi_user_limiter-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-02 10:49:28.000000 fastapi_user_limiter-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 10:49:35.856313 fastapi_user_limiter-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:49:35.856313 fastapi_user_limiter-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:49:35.856313 fastapi_user_limiter-0.6.0/src/fastapi_user_limiter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 10:49:28.000000 fastapi_user_limiter-0.6.0/src/fastapi_user_limiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-02 10:49:28.000000 fastapi_user_limiter-0.6.0/src/fastapi_user_limiter/limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:49:35.856313 fastapi_user_limiter-0.6.0/src/fastapi_user_limiter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-02 10:49:35.000000 fastapi_user_limiter-0.6.0/src/fastapi_user_limiter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-02 10:49:35.000000 fastapi_user_limiter-0.6.0/src/fastapi_user_limiter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:49:35.000000 fastapi_user_limiter-0.6.0/src/fastapi_user_limiter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-02 10:49:35.000000 fastapi_user_limiter-0.6.0/src/fastapi_user_limiter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 10:49:35.000000 fastapi_user_limiter-0.6.0/src/fastapi_user_limiter.egg-info/top_level.txt
```

### Comparing `fastapi_user_limiter-0.5.0/PKG-INFO` & `fastapi_user_limiter-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_user_limiter
-Version: 0.5.0
+Version: 0.6.0
 Summary: Rate-limiter for FastAPI with the possibility of user-based rate limits
 Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/fastapi-user-limiter
 Project-URL: Bug Tracker, https://github.com/epflgraph/fastapi-user-limiter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -90,15 +90,15 @@
     return {"Hello": "There"}
 ```
 
 ### Per-user rate limits
 
 By default, rate limits are applied per host (i.e. per IP address). However, 
 you may want to apply the rate limits on a per-user basis, especially if your
-API has authentication. To do so, you can pass a custom callable to the
+API has authentication. To do so, you can pass a custom async callable to the
 `user` argument of `rate_limiter`, which extracts the username from the request
 headers:
 
 ```python
 from fastapi_user_limiter.limiter import RateLimiterConnection, rate_limiter
 from fastapi import Depends, FastAPI
```

### Comparing `fastapi_user_limiter-0.5.0/README.md` & `fastapi_user_limiter-0.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     return {"Hello": "There"}
 ```
 
 ### Per-user rate limits
 
 By default, rate limits are applied per host (i.e. per IP address). However, 
 you may want to apply the rate limits on a per-user basis, especially if your
-API has authentication. To do so, you can pass a custom callable to the
+API has authentication. To do so, you can pass a custom async callable to the
 `user` argument of `rate_limiter`, which extracts the username from the request
 headers:
 
 ```python
 from fastapi_user_limiter.limiter import RateLimiterConnection, rate_limiter
 from fastapi import Depends, FastAPI
```

### Comparing `fastapi_user_limiter-0.5.0/pyproject.toml` & `fastapi_user_limiter-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastapi_user_limiter"
-version = "0.5.0"
+version = "0.6.0"
 authors = [
   { name="Ramtin Yazdanian", email="ramtin.yazdanian@epfl.ch" }
 ]
 description = "Rate-limiter for FastAPI with the possibility of user-based rate limits"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `fastapi_user_limiter-0.5.0/src/fastapi_user_limiter/limiter.py` & `fastapi_user_limiter-0.6.0/src/fastapi_user_limiter/limiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         # Providing a None value for either window or max_requests disables rate limiting
         if rl is None or max_requests is None or window is None:
             return
         # Checking to see if a custom callable has been provided for the username
         if user is None:
             user_name = request.client.host
         else:
-            user_name = user(request.headers)
+            user_name = await user(request.headers)
         # Checking to see if a custom path has been provided
         if path is None:
             path_name = request.url.path
         else:
             path_name = path
         # Generating the redis key
         key = f"rate_limit:{path_name}:{window}:{max_requests}:{user_name}"
```

### Comparing `fastapi_user_limiter-0.5.0/src/fastapi_user_limiter.egg-info/PKG-INFO` & `fastapi_user_limiter-0.6.0/src/fastapi_user_limiter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_user_limiter
-Version: 0.5.0
+Version: 0.6.0
 Summary: Rate-limiter for FastAPI with the possibility of user-based rate limits
 Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/fastapi-user-limiter
 Project-URL: Bug Tracker, https://github.com/epflgraph/fastapi-user-limiter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -90,15 +90,15 @@
     return {"Hello": "There"}
 ```
 
 ### Per-user rate limits
 
 By default, rate limits are applied per host (i.e. per IP address). However, 
 you may want to apply the rate limits on a per-user basis, especially if your
-API has authentication. To do so, you can pass a custom callable to the
+API has authentication. To do so, you can pass a custom async callable to the
 `user` argument of `rate_limiter`, which extracts the username from the request
 headers:
 
 ```python
 from fastapi_user_limiter.limiter import RateLimiterConnection, rate_limiter
 from fastapi import Depends, FastAPI
```

