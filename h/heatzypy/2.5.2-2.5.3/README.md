# Comparing `tmp/heatzypy-2.5.2.tar.gz` & `tmp/heatzypy-2.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heatzypy-2.5.2.tar", last modified: Wed May  1 17:27:21 2024, max compression
+gzip compressed data, was "heatzypy-2.5.3.tar", last modified: Wed May  1 18:19:43 2024, max compression
```

## Comparing `heatzypy-2.5.2.tar` & `heatzypy-2.5.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:27:21.266373 heatzypy-2.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:27:21.262373 heatzypy-2.5.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-01 17:27:12.000000 heatzypy-2.5.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:27:21.262373 heatzypy-2.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-01 17:27:12.000000 heatzypy-2.5.2/.github/workflows/auto-approve.yml
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-01 17:27:12.000000 heatzypy-2.5.2/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-01 17:27:12.000000 heatzypy-2.5.2/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-01 17:27:12.000000 heatzypy-2.5.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-01 17:27:12.000000 heatzypy-2.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-01 17:27:12.000000 heatzypy-2.5.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:27:21.262373 heatzypy-2.5.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-01 17:27:12.000000 heatzypy-2.5.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 17:27:12.000000 heatzypy-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-01 17:27:12.000000 heatzypy-2.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-01 17:27:21.266373 heatzypy-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-01 17:27:12.000000 heatzypy-2.5.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2353 2024-05-01 17:27:12.000000 heatzypy-2.5.2/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:27:21.262373 heatzypy-2.5.2/heatzypy/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-01 17:27:12.000000 heatzypy-2.5.2/heatzypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-01 17:27:12.000000 heatzypy-2.5.2/heatzypy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-01 17:27:12.000000 heatzypy-2.5.2/heatzypy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-01 17:27:12.000000 heatzypy-2.5.2/heatzypy/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-01 17:27:12.000000 heatzypy-2.5.2/heatzypy/heatzy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11761 2024-05-01 17:27:12.000000 heatzypy-2.5.2/heatzypy/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:27:21.266373 heatzypy-2.5.2/heatzypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-01 17:27:21.000000 heatzypy-2.5.2/heatzypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-01 17:27:21.000000 heatzypy-2.5.2/heatzypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:27:21.000000 heatzypy-2.5.2/heatzypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:27:20.000000 heatzypy-2.5.2/heatzypy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 17:27:21.000000 heatzypy-2.5.2/heatzypy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 17:27:21.000000 heatzypy-2.5.2/heatzypy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-01 17:27:12.000000 heatzypy-2.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 17:27:12.000000 heatzypy-2.5.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 17:27:12.000000 heatzypy-2.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 17:27:21.266373 heatzypy-2.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:19:43.718483 heatzypy-2.5.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:19:43.714483 heatzypy-2.5.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-01 18:19:28.000000 heatzypy-2.5.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:19:43.714483 heatzypy-2.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-01 18:19:28.000000 heatzypy-2.5.3/.github/workflows/auto-approve.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-01 18:19:28.000000 heatzypy-2.5.3/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-01 18:19:28.000000 heatzypy-2.5.3/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-01 18:19:28.000000 heatzypy-2.5.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-01 18:19:28.000000 heatzypy-2.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-01 18:19:28.000000 heatzypy-2.5.3/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:19:43.714483 heatzypy-2.5.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-01 18:19:28.000000 heatzypy-2.5.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 18:19:28.000000 heatzypy-2.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-01 18:19:28.000000 heatzypy-2.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-01 18:19:43.718483 heatzypy-2.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-01 18:19:28.000000 heatzypy-2.5.3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2401 2024-05-01 18:19:28.000000 heatzypy-2.5.3/example.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:19:43.718483 heatzypy-2.5.3/heatzypy/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-01 18:19:28.000000 heatzypy-2.5.3/heatzypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-05-01 18:19:28.000000 heatzypy-2.5.3/heatzypy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-01 18:19:28.000000 heatzypy-2.5.3/heatzypy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-01 18:19:28.000000 heatzypy-2.5.3/heatzypy/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-01 18:19:28.000000 heatzypy-2.5.3/heatzypy/heatzy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11739 2024-05-01 18:19:28.000000 heatzypy-2.5.3/heatzypy/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:19:43.718483 heatzypy-2.5.3/heatzypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-01 18:19:43.000000 heatzypy-2.5.3/heatzypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-01 18:19:43.000000 heatzypy-2.5.3/heatzypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:19:43.000000 heatzypy-2.5.3/heatzypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:19:43.000000 heatzypy-2.5.3/heatzypy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 18:19:43.000000 heatzypy-2.5.3/heatzypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-01 18:19:43.000000 heatzypy-2.5.3/heatzypy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-01 18:19:28.000000 heatzypy-2.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-01 18:19:28.000000 heatzypy-2.5.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 18:19:28.000000 heatzypy-2.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:19:43.718483 heatzypy-2.5.3/setup.cfg
```

### Comparing `heatzypy-2.5.2/.github/dependabot.yml` & `heatzypy-2.5.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.2/.github/workflows/auto-approve.yml` & `heatzypy-2.5.3/.github/workflows/auto-approve.yml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.2/.github/workflows/lint.yml` & `heatzypy-2.5.3/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.2/.github/workflows/pythonpublish.yml` & `heatzypy-2.5.3/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.2/.github/workflows/release.yml` & `heatzypy-2.5.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.2/.gitignore` & `heatzypy-2.5.3/.gitignore`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.2/.pre-commit-config.yaml` & `heatzypy-2.5.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.2/LICENSE` & `heatzypy-2.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.2/PKG-INFO` & `heatzypy-2.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heatzypy
-Version: 2.5.2
+Version: 2.5.3
 Summary: Provides authentication and access to Heatzy module
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: heatzy,websocket,async,climate
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `heatzypy-2.5.2/README.md` & `heatzypy-2.5.3/README.md`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.2/example.py` & `heatzypy-2.5.3/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,19 @@
                 logger.error(error)
     except AuthenticationFailed as error:
         logger.error("Auth failed (%s)", error)
     except HeatzyException as error:
         logger.error(str(error))
 
     # Listen Heatzy webscoket
-    api.websocket.register_callback(callback)
+
     try:
+        api.websocket.register_callback(callback)
         await api.websocket.async_connect(auto_subscribe=True, all_devices=True)
+        await api.websocket.async_listen()
     except AuthenticationFailed as error:
         logger.error("Auth failed (%s)", error)
     except HeatzyException as error:
         logger.error(str(error))
 
     while api.websocket.is_connected:
         await asyncio.sleep(1)
```

### Comparing `heatzypy-2.5.2/heatzypy/auth.py` & `heatzypy-2.5.3/heatzypy/auth.py`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.2/heatzypy/exception.py` & `heatzypy-2.5.3/heatzypy/exception.py`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.2/heatzypy/heatzy.py` & `heatzypy-2.5.3/heatzypy/heatzy.py`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.2/heatzypy/websocket.py` & `heatzypy-2.5.3/heatzypy/websocket.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,20 +139,14 @@
             ) from exception
 
         try:
             await self.async_login(auto_subscribe)
         except WebsocketError as error:
             raise AuthenticationFailed(error) from error
 
-        try:
-            if self._return_all:
-                await self.async_get_devices()
-        except WebsocketError as error:
-            raise AuthenticationFailed(error) from error
-
     async def async_login(self, auto_subscribe: bool = True) -> None:
         """Login to websocket."""
 
         token_data = await self._auth.async_get_token()
 
         payload = {
             "cmd": "login_req",
@@ -170,17 +164,14 @@
 
     async def async_listen(self) -> None:
         """Listen for events on the WebSocket."""
 
         while not self.ws.closed:
             message = await self.ws.receive()
 
-            if self._event:
-                self._event.set()
-
             if message.type == aiohttp.WSMsgType.ERROR:
                 raise ConnectionFailed(self.ws.exception())
 
             if message.type == aiohttp.WSMsgType.BINARY:
                 pass
 
             if message.type == aiohttp.WSMsgType.TEXT:
@@ -244,14 +235,17 @@
 
     async def _handle_login(self, data: dict[str, Any]) -> None:
         """Handle login response."""
         if data.get("success") is False:
             raise AuthenticationFailed(data)
         logger.debug("WEBSOCKET Successfully authenticated")
         self.logged_in = True
+        if self._event:
+            self._event.set()
+            self._event.clear()
 
     async def _handle_subscription(self, data: dict[str, Any]) -> None:
         """Handle the response of subscription."""
         devices = cast(list[Any], data.get("success"))
         for device in devices:
             if (did := device["did"]) not in self.subscribed_devices:
                 self.subscribed_devices.append(did)
@@ -262,14 +256,17 @@
             device = self.devices.get(did)
             if device and (attrs := data.get("attrs")):
                 device["attrs"] = attrs
                 if len(self._callbacks) > 0:
                     if self._return_all:
                         if self.check_full(self.devices):
                             self._run_callbacks(self.devices)
+                            if self._event:
+                                self._event.set()
+                                self._event.clear()
                     else:
                         self._run_callbacks(device)
 
     async def _handle_invalid_msg(self, data: dict[str, Any]) -> None:
         """Handle a notification receive by client."""
         logger.warn("Received invalid message: %s", data)
         self.last_invalid_msg = data
```

### Comparing `heatzypy-2.5.2/heatzypy.egg-info/PKG-INFO` & `heatzypy-2.5.3/heatzypy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heatzypy
-Version: 2.5.2
+Version: 2.5.3
 Summary: Provides authentication and access to Heatzy module
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: heatzy,websocket,async,climate
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `heatzypy-2.5.2/heatzypy.egg-info/SOURCES.txt` & `heatzypy-2.5.3/heatzypy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heatzypy-2.5.2/pyproject.toml` & `heatzypy-2.5.3/pyproject.toml`

 * *Files identical despite different names*

