# Comparing `tmp/fastapi_user_limiter-0.3.0.tar.gz` & `tmp/fastapi_user_limiter-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_user_limiter-0.3.0.tar", last modified: Tue Apr 30 14:19:32 2024, max compression
+gzip compressed data, was "fastapi_user_limiter-0.4.0.tar", last modified: Wed May  1 12:56:24 2024, max compression
```

## Comparing `fastapi_user_limiter-0.3.0.tar` & `fastapi_user_limiter-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:19:32.012859 fastapi_user_limiter-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-30 14:19:32.012859 fastapi_user_limiter-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-30 14:19:24.000000 fastapi_user_limiter-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-30 14:19:24.000000 fastapi_user_limiter-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 14:19:32.012859 fastapi_user_limiter-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:19:32.012859 fastapi_user_limiter-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:19:32.012859 fastapi_user_limiter-0.3.0/src/fastapi_user_limiter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:19:24.000000 fastapi_user_limiter-0.3.0/src/fastapi_user_limiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-04-30 14:19:24.000000 fastapi_user_limiter-0.3.0/src/fastapi_user_limiter/limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:19:32.012859 fastapi_user_limiter-0.3.0/src/fastapi_user_limiter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-30 14:19:32.000000 fastapi_user_limiter-0.3.0/src/fastapi_user_limiter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-30 14:19:32.000000 fastapi_user_limiter-0.3.0/src/fastapi_user_limiter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:19:32.000000 fastapi_user_limiter-0.3.0/src/fastapi_user_limiter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-30 14:19:32.000000 fastapi_user_limiter-0.3.0/src/fastapi_user_limiter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-30 14:19:32.000000 fastapi_user_limiter-0.3.0/src/fastapi_user_limiter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:56:24.179909 fastapi_user_limiter-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-01 12:56:24.175909 fastapi_user_limiter-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-01 12:56:18.000000 fastapi_user_limiter-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-01 12:56:18.000000 fastapi_user_limiter-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 12:56:24.179909 fastapi_user_limiter-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:56:24.175909 fastapi_user_limiter-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:56:24.175909 fastapi_user_limiter-0.4.0/src/fastapi_user_limiter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 12:56:18.000000 fastapi_user_limiter-0.4.0/src/fastapi_user_limiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-01 12:56:18.000000 fastapi_user_limiter-0.4.0/src/fastapi_user_limiter/limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 12:56:24.175909 fastapi_user_limiter-0.4.0/src/fastapi_user_limiter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-01 12:56:24.000000 fastapi_user_limiter-0.4.0/src/fastapi_user_limiter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 12:56:24.000000 fastapi_user_limiter-0.4.0/src/fastapi_user_limiter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 12:56:24.000000 fastapi_user_limiter-0.4.0/src/fastapi_user_limiter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 12:56:24.000000 fastapi_user_limiter-0.4.0/src/fastapi_user_limiter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 12:56:24.000000 fastapi_user_limiter-0.4.0/src/fastapi_user_limiter.egg-info/top_level.txt
```

### Comparing `fastapi_user_limiter-0.3.0/PKG-INFO` & `fastapi_user_limiter-0.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_user_limiter
-Version: 0.3.0
+Version: 0.4.0
 Summary: Rate-limiter for FastAPI with the possibility of user-based rate limits
 Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/fastapi-user-limiter
 Project-URL: Bug Tracker, https://github.com/epflgraph/fastapi-user-limiter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,14 +22,18 @@
 First install Redis, then install the package using:
 ```
 pip install fastapi-user-limiter
 ```
 
 ## Usage
 
+All the examples below can be found in `example.py` (use ` uvicorn example:app --reload` to run).
+
+### Single and multiple rate limiters
+
 You can use the `rate_limit` function as a FastAPI Dependency to add one or several rate limiters to an endpoint:
 
 ```python
 from fastapi_user_limiter.limiter import RateLimiterConnection, rate_limiter
 from fastapi import FastAPI, Depends
 
 app = FastAPI()
@@ -47,12 +51,75 @@
     Depends(rate_limiter(RateLimiterConnection(), 1, 1)),
     Depends(rate_limiter(RateLimiterConnection(), 3, 10))
 ])
 async def read_multi(some_param: str):
     return {"Hello": f"There {some_param}"}
 ```
 
-The aforementioned examples and more can be found in `example.py` (use ` uvicorn example:app --reload` to run).
+### Router/API-wide rate limits
+
+You can also add a router-wide (or even API-wide) rate limiter that applies to all endpoints taken together,
+rather than per-endpoint:
+
+```python
+from fastapi_user_limiter.limiter import RateLimiterConnection, rate_limiter
+from fastapi import Depends, APIRouter
+
+# The rate limiter in the router applies to the two endpoints together.
+# If a request is made to /single, a request to /single2 within the next 
+# 3 seconds will result in a "Too many requests" error.
+
+# This rate limiter must have a custom path value, preferably 
+# the same as the router's prefix value.
+router = APIRouter(
+    prefix='/router',
+    dependencies=[Depends(rate_limiter(RateLimiterConnection(), 1, 3,
+                                       path='/router'))]
+)
+
+
+# Each endpoint also has its own, separate rate limiter
+@router.get("/single",
+            dependencies=[Depends(rate_limiter(RateLimiterConnection(), 3, 20))])
+async def read_single_router():
+    return {"Hello": "World"}
+
+
+@router.get("/single2",
+            dependencies=[Depends(rate_limiter(RateLimiterConnection(), 5, 60))])
+async def read_single2_router():
+    return {"Hello": "There"}
+```
+
+### Per-user rate limits
+
+By default, rate limits are applied per host (i.e. per IP address). However, 
+you may want to apply the rate limits on a per-user basis, especially if your
+API has authentication. To do so, you can pass a custom callable to the
+`user` argument of `rate_limiter`, which extracts the username from the request
+headers:
+
+```python
+from fastapi_user_limiter.limiter import RateLimiterConnection, rate_limiter
+from fastapi import Depends, FastAPI
+
+app = FastAPI()
+
+
+def get_user(headers):
+    # The username is assumed to be a bearer token,
+    # contained in the 'authorization' header.
+    username = headers['authorization'].strip('Bearer ')
+    return username
+
+# 3 requests max per 20 seconds, per user
+@app.post("/auth",
+          dependencies=[Depends(rate_limiter(RateLimiterConnection(), 3, 20,
+                                             user=get_user))])
+async def read_with_auth(data: dict):
+    return {'input': data}
+```
 
 ## Future features
 
-The package will soon have the additional feature of allowing each user account to have a different rate limit for each endpoint.
+The package will soon have the additional feature of allowing each user account to have a different window size and max 
+request count for each endpoint.
```

### Comparing `fastapi_user_limiter-0.3.0/pyproject.toml` & `fastapi_user_limiter-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fastapi_user_limiter"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
   { name="Ramtin Yazdanian", email="ramtin.yazdanian@epfl.ch" }
 ]
 description = "Rate-limiter for FastAPI with the possibility of user-based rate limits"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `fastapi_user_limiter-0.3.0/src/fastapi_user_limiter.egg-info/PKG-INFO` & `fastapi_user_limiter-0.4.0/src/fastapi_user_limiter.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_user_limiter
-Version: 0.3.0
+Version: 0.4.0
 Summary: Rate-limiter for FastAPI with the possibility of user-based rate limits
 Author-email: Ramtin Yazdanian <ramtin.yazdanian@epfl.ch>
 Project-URL: Homepage, https://github.com/epflgraph/fastapi-user-limiter
 Project-URL: Bug Tracker, https://github.com/epflgraph/fastapi-user-limiter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -22,14 +22,18 @@
 First install Redis, then install the package using:
 ```
 pip install fastapi-user-limiter
 ```
 
 ## Usage
 
+All the examples below can be found in `example.py` (use ` uvicorn example:app --reload` to run).
+
+### Single and multiple rate limiters
+
 You can use the `rate_limit` function as a FastAPI Dependency to add one or several rate limiters to an endpoint:
 
 ```python
 from fastapi_user_limiter.limiter import RateLimiterConnection, rate_limiter
 from fastapi import FastAPI, Depends
 
 app = FastAPI()
@@ -47,12 +51,75 @@
     Depends(rate_limiter(RateLimiterConnection(), 1, 1)),
     Depends(rate_limiter(RateLimiterConnection(), 3, 10))
 ])
 async def read_multi(some_param: str):
     return {"Hello": f"There {some_param}"}
 ```
 
-The aforementioned examples and more can be found in `example.py` (use ` uvicorn example:app --reload` to run).
+### Router/API-wide rate limits
+
+You can also add a router-wide (or even API-wide) rate limiter that applies to all endpoints taken together,
+rather than per-endpoint:
+
+```python
+from fastapi_user_limiter.limiter import RateLimiterConnection, rate_limiter
+from fastapi import Depends, APIRouter
+
+# The rate limiter in the router applies to the two endpoints together.
+# If a request is made to /single, a request to /single2 within the next 
+# 3 seconds will result in a "Too many requests" error.
+
+# This rate limiter must have a custom path value, preferably 
+# the same as the router's prefix value.
+router = APIRouter(
+    prefix='/router',
+    dependencies=[Depends(rate_limiter(RateLimiterConnection(), 1, 3,
+                                       path='/router'))]
+)
+
+
+# Each endpoint also has its own, separate rate limiter
+@router.get("/single",
+            dependencies=[Depends(rate_limiter(RateLimiterConnection(), 3, 20))])
+async def read_single_router():
+    return {"Hello": "World"}
+
+
+@router.get("/single2",
+            dependencies=[Depends(rate_limiter(RateLimiterConnection(), 5, 60))])
+async def read_single2_router():
+    return {"Hello": "There"}
+```
+
+### Per-user rate limits
+
+By default, rate limits are applied per host (i.e. per IP address). However, 
+you may want to apply the rate limits on a per-user basis, especially if your
+API has authentication. To do so, you can pass a custom callable to the
+`user` argument of `rate_limiter`, which extracts the username from the request
+headers:
+
+```python
+from fastapi_user_limiter.limiter import RateLimiterConnection, rate_limiter
+from fastapi import Depends, FastAPI
+
+app = FastAPI()
+
+
+def get_user(headers):
+    # The username is assumed to be a bearer token,
+    # contained in the 'authorization' header.
+    username = headers['authorization'].strip('Bearer ')
+    return username
+
+# 3 requests max per 20 seconds, per user
+@app.post("/auth",
+          dependencies=[Depends(rate_limiter(RateLimiterConnection(), 3, 20,
+                                             user=get_user))])
+async def read_with_auth(data: dict):
+    return {'input': data}
+```
 
 ## Future features
 
-The package will soon have the additional feature of allowing each user account to have a different rate limit for each endpoint.
+The package will soon have the additional feature of allowing each user account to have a different window size and max 
+request count for each endpoint.
```

