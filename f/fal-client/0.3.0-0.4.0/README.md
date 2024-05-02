# Comparing `tmp/fal_client-0.3.0.tar.gz` & `tmp/fal_client-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal_client-0.3.0.tar", last modified: Fri Apr 19 21:20:56 2024, max compression
+gzip compressed data, was "fal_client-0.4.0.tar", last modified: Thu May  2 16:37:39 2024, max compression
```

## Comparing `fal_client-0.3.0.tar` & `fal_client-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:20:56.222720 fal_client-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-19 21:20:56.222720 fal_client-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-19 21:20:49.000000 fal_client-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-19 21:20:49.000000 fal_client-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:20:56.222720 fal_client-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:20:56.222720 fal_client-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:20:56.222720 fal_client-0.3.0/src/fal_client/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-19 21:20:49.000000 fal_client-0.3.0/src/fal_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-19 21:20:49.000000 fal_client-0.3.0/src/fal_client/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    14789 2024-04-19 21:20:49.000000 fal_client-0.3.0/src/fal_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:20:49.000000 fal_client-0.3.0/src/fal_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:20:56.222720 fal_client-0.3.0/src/fal_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-19 21:20:56.000000 fal_client-0.3.0/src/fal_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-19 21:20:56.000000 fal_client-0.3.0/src/fal_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:20:56.000000 fal_client-0.3.0/src/fal_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-19 21:20:56.000000 fal_client-0.3.0/src/fal_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 21:20:56.000000 fal_client-0.3.0/src/fal_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:20:56.222720 fal_client-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-19 21:20:49.000000 fal_client-0.3.0/tests/test_async_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-19 21:20:49.000000 fal_client-0.3.0/tests/test_sync_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:37:39.882037 fal_client-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-02 16:37:39.882037 fal_client-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-02 16:37:33.000000 fal_client-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-02 16:37:33.000000 fal_client-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:37:39.882037 fal_client-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:37:39.878037 fal_client-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:37:39.878037 fal_client-0.4.0/src/fal_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-02 16:37:33.000000 fal_client-0.4.0/src/fal_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-02 16:37:33.000000 fal_client-0.4.0/src/fal_client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15020 2024-05-02 16:37:33.000000 fal_client-0.4.0/src/fal_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 16:37:33.000000 fal_client-0.4.0/src/fal_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:37:39.882037 fal_client-0.4.0/src/fal_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-02 16:37:39.000000 fal_client-0.4.0/src/fal_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-02 16:37:39.000000 fal_client-0.4.0/src/fal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:37:39.000000 fal_client-0.4.0/src/fal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-02 16:37:39.000000 fal_client-0.4.0/src/fal_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 16:37:39.000000 fal_client-0.4.0/src/fal_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:37:39.878037 fal_client-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-02 16:37:33.000000 fal_client-0.4.0/tests/test_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-02 16:37:33.000000 fal_client-0.4.0/tests/test_sync_client.py
```

### Comparing `fal_client-0.3.0/PKG-INFO` & `fal_client-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: fal_client
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python client for fal.ai
 Author: fal <hello@fal.ai>
 Project-URL: homepage, https://fal.ai
 Project-URL: repository, https://github.com/fal-ai/fal
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: httpx<1,>=0.21.0
 Requires-Dist: httpx-sse<0.5,>=0.4.0
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-asyncio; extra == "test"
+Provides-Extra: dev
+Requires-Dist: fal_client[test]; extra == "dev"
 
 # fal.ai Python client
 
 This is a Python client library for interacting with ML models deployed on [fal.ai](https://fal.ai).
 
 ## Getting started
```

### Comparing `fal_client-0.3.0/README.md` & `fal_client-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fal_client-0.3.0/pyproject.toml` & `fal_client-0.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,23 @@
 authors = [{ name = "fal <hello@fal.ai>" }]
 requires-python = ">=3.8"
 dependencies = [
     "httpx>=0.21.0,<1",
     "httpx-sse>=0.4.0,<0.5",
 ]
 
+[project.optional-dependencies]
+test = [
+    "pytest",
+    "pytest-asyncio",
+]
+dev = [
+    "fal_client[test]",
+]
+
 [project.urls]
 homepage = "https://fal.ai"
 repository = "https://github.com/fal-ai/fal"
 
 [tool.pytest.ini_options]
 testpaths = "tests/"
 asyncio_mode = "auto"
```

### Comparing `fal_client-0.3.0/src/fal_client/__init__.py` & `fal_client-0.4.0/src/fal_client/__init__.py`

 * *Files identical despite different names*

### Comparing `fal_client-0.3.0/src/fal_client/auth.py` & `fal_client-0.4.0/src/fal_client/auth.py`

 * *Files identical despite different names*

### Comparing `fal_client-0.3.0/src/fal_client/client.py` & `fal_client-0.4.0/src/fal_client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,49 +164,51 @@
         response.raise_for_status()
         return response.json()
 
 
 @dataclass(frozen=True)
 class AsyncClient:
     key: str | None = field(default=None, repr=False)
-    default_timeout: float = 60.0
+    default_timeout: float = 120.0
 
     @cached_property
     def _client(self) -> httpx.AsyncClient:
         if self.key is None:
             key = fetch_credentials()
         else:
             key = self.key
 
         return httpx.AsyncClient(
             headers={
                 "Authorization": f"Key {key}",
                 "User-Agent": USER_AGENT,
-            }
+            },
+            timeout=self.default_timeout,
         )
 
     async def run(
         self,
         application: str,
         arguments: AnyJSON,
         *,
         path: str = "",
+        timeout: float | None = None,
     ) -> AnyJSON:
         """Run an application with the given arguments (which will be JSON serialized). The path parameter can be used to
         specify a subpath when applicable. This method will return the result of the inference call directly.
         """
 
         url = RUN_URL_FORMAT + application
         if path:
             url += "/" + path.lstrip("/")
 
         response = await self._client.post(
             url,
             json=arguments,
-            timeout=self.default_timeout,
+            timeout=timeout,
         )
         response.raise_for_status()
         return response.json()
 
     async def submit(
         self,
         application: str,
@@ -221,15 +223,14 @@
         url = QUEUE_URL_FORMAT + application
         if path:
             url += "/" + path.lstrip("/")
 
         response = await self._client.post(
             url,
             json=arguments,
-            timeout=self.default_timeout,
         )
         response.raise_for_status()
 
         data = response.json()
         return AsyncRequestHandle(
             request_id=data["request_id"],
             response_url=data["response_url"],
@@ -240,27 +241,34 @@
 
     async def stream(
         self,
         application: str,
         arguments: AnyJSON,
         *,
         path: str = "/stream",
+        timeout: float | None = None,
     ) -> AsyncIterator[dict[str, Any]]:
         """Stream the output of an application with the given arguments (which will be JSON serialized). This is only supported
         at a few select applications at the moment, so be sure to first consult with the documentation of individual applications
         to see if this is supported.
 
         The function will iterate over each event that is streamed from the server.
         """
 
         url = RUN_URL_FORMAT + application
         if path:
             url += "/" + path.lstrip("/")
 
-        async with aconnect_sse(self._client, "POST", url, json=arguments) as events:
+        async with aconnect_sse(
+            self._client,
+            "POST",
+            url,
+            json=arguments,
+            timeout=timeout,
+        ) as events:
             async for event in events.aiter_sse():
                 yield event.json()
 
     async def upload(self, data: str | bytes, content_type: str) -> str:
         """Upload the given data blob to the CDN and return the access URL. The content type should be specified
         as the second argument. Use upload_file or upload_image for convenience."""
 
@@ -290,15 +298,15 @@
             image.save(buffer, format=format)
             return await self.upload(buffer.getvalue(), f"image/{format}")
 
 
 @dataclass(frozen=True)
 class SyncClient:
     key: str | None = field(default=None, repr=False)
-    default_timeout: float = 60.0
+    default_timeout: float = 120.0
 
     @cached_property
     def _client(self) -> httpx.Client:
         if self.key is None:
             key = fetch_credentials()
         else:
             key = self.key
@@ -367,27 +375,30 @@
 
     def stream(
         self,
         application: str,
         arguments: AnyJSON,
         *,
         path: str = "/stream",
+        timeout: float | None = None,
     ) -> Iterator[dict[str, Any]]:
         """Stream the output of an application with the given arguments (which will be JSON serialized). This is only supported
         at a few select applications at the moment, so be sure to first consult with the documentation of individual applications
         to see if this is supported.
 
         The function will iterate over each event that is streamed from the server.
         """
 
         url = RUN_URL_FORMAT + application
         if path:
             url += "/" + path.lstrip("/")
 
-        with connect_sse(self._client, "POST", url, json=arguments) as events:
+        with connect_sse(
+            self._client, "POST", url, json=arguments, timeout=timeout
+        ) as events:
             for event in events.iter_sse():
                 yield event.json()
 
     def upload(self, data: str | bytes, content_type: str) -> str:
         """Upload the given data blob to the CDN and return the access URL. The content type should be specified
         as the second argument. Use upload_file or upload_image for convenience."""
```

### Comparing `fal_client-0.3.0/src/fal_client.egg-info/PKG-INFO` & `fal_client-0.4.0/src/fal_client.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: fal_client
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python client for fal.ai
 Author: fal <hello@fal.ai>
 Project-URL: homepage, https://fal.ai
 Project-URL: repository, https://github.com/fal-ai/fal
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: httpx<1,>=0.21.0
 Requires-Dist: httpx-sse<0.5,>=0.4.0
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-asyncio; extra == "test"
+Provides-Extra: dev
+Requires-Dist: fal_client[test]; extra == "dev"
 
 # fal.ai Python client
 
 This is a Python client library for interacting with ML models deployed on [fal.ai](https://fal.ai).
 
 ## Getting started
```

### Comparing `fal_client-0.3.0/tests/test_async_client.py` & `fal_client-0.4.0/tests/test_async_client.py`

 * *Files identical despite different names*

### Comparing `fal_client-0.3.0/tests/test_sync_client.py` & `fal_client-0.4.0/tests/test_sync_client.py`

 * *Files identical despite different names*

