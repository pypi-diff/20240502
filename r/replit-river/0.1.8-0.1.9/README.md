# Comparing `tmp/replit_river-0.1.8.tar.gz` & `tmp/replit_river-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit_river-0.1.8.tar", max compression
+gzip compressed data, was "replit_river-0.1.9.tar", max compression
```

## Comparing `replit_river-0.1.8.tar` & `replit_river-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1064 2024-04-19 19:26:13.426252 replit_river-0.1.8/LICENSE
--rw-r--r--   0        0        0     1628 2024-04-19 19:26:13.426318 replit_river-0.1.8/README.md
--rw-r--r--   0        0        0     1742 2024-04-24 23:36:50.745203 replit_river-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      487 2024-04-22 19:50:44.355705 replit_river-0.1.8/replit_river/__init__.py
--rw-r--r--   0        0        0     3847 2024-04-24 23:10:35.786501 replit_river-0.1.8/replit_river/client.py
--rw-r--r--   0        0        0    10717 2024-04-24 23:52:30.740117 replit_river-0.1.8/replit_river/client_session.py
--rw-r--r--   0        0        0    12323 2024-04-24 23:49:21.694200 replit_river-0.1.8/replit_river/client_transport.py
--rw-r--r--   0        0        0        0 2024-04-22 19:50:44.356674 replit_river-0.1.8/replit_river/codegen/__init__.py
--rwxr-xr-x   0        0        0      153 2024-04-22 19:50:44.356784 replit_river-0.1.8/replit_river/codegen/__main__.py
--rw-r--r--   0        0        0    13363 2024-04-22 19:50:44.356886 replit_river-0.1.8/replit_river/codegen/client.py
--rw-r--r--   0        0        0     1903 2024-04-22 19:50:44.356956 replit_river-0.1.8/replit_river/codegen/run.py
--rw-r--r--   0        0        0     5354 2024-04-24 23:49:28.777220 replit_river-0.1.8/replit_river/codegen/schema.py
--rw-r--r--   0        0        0    12620 2024-04-24 23:49:28.805274 replit_river-0.1.8/replit_river/codegen/server.py
--rw-r--r--   0        0        0      547 2024-04-22 19:50:44.357515 replit_river-0.1.8/replit_river/error_schema.py
--rw-r--r--   0        0        0     1482 2024-04-24 23:40:20.838560 replit_river-0.1.8/replit_river/message_buffer.py
--rw-r--r--   0        0        0     2606 2024-04-24 22:30:56.712779 replit_river-0.1.8/replit_river/messages.py
--rw-r--r--   0        0        0        0 2024-04-22 19:50:44.358418 replit_river-0.1.8/replit_river/py.typed
--rw-r--r--   0        0        0     3565 2024-04-24 23:49:26.772845 replit_river-0.1.8/replit_river/rate_limiter.py
--rw-r--r--   0        0        0    12635 2024-04-24 23:47:43.465686 replit_river-0.1.8/replit_river/rpc.py
--rw-r--r--   0        0        0     2293 2024-04-24 23:14:37.024811 replit_river-0.1.8/replit_river/seq_manager.py
--rw-r--r--   0        0        0     2294 2024-04-24 23:09:28.482659 replit_river-0.1.8/replit_river/server.py
--rw-r--r--   0        0        0     5916 2024-04-24 23:47:43.421824 replit_river-0.1.8/replit_river/server_transport.py
--rw-r--r--   0        0        0    20444 2024-04-24 23:43:54.064753 replit_river-0.1.8/replit_river/session.py
--rw-r--r--   0        0        0     3833 2024-04-24 23:37:26.072767 replit_river-0.1.8/replit_river/task_manager.py
--rw-r--r--   0        0        0     5524 2024-04-24 23:48:34.430006 replit_river-0.1.8/replit_river/transport.py
--rw-r--r--   0        0        0     1610 2024-04-24 23:39:46.272366 replit_river-0.1.8/replit_river/transport_options.py
--rw-r--r--   0        0        0     2446 1970-01-01 00:00:00.000000 replit_river-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-19 19:26:13.426252 replit_river-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1628 2024-04-19 19:26:13.426318 replit_river-0.1.9/README.md
+-rw-r--r--   0        0        0     1742 2024-04-25 06:51:34.824805 replit_river-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      487 2024-04-22 19:50:44.355705 replit_river-0.1.9/replit_river/__init__.py
+-rw-r--r--   0        0        0     3847 2024-04-24 23:10:35.786501 replit_river-0.1.9/replit_river/client.py
+-rw-r--r--   0        0        0    10717 2024-04-24 23:52:30.740117 replit_river-0.1.9/replit_river/client_session.py
+-rw-r--r--   0        0        0    12623 2024-04-25 06:45:34.961333 replit_river-0.1.9/replit_river/client_transport.py
+-rw-r--r--   0        0        0        0 2024-04-22 19:50:44.356674 replit_river-0.1.9/replit_river/codegen/__init__.py
+-rwxr-xr-x   0        0        0      153 2024-04-22 19:50:44.356784 replit_river-0.1.9/replit_river/codegen/__main__.py
+-rw-r--r--   0        0        0    13363 2024-04-22 19:50:44.356886 replit_river-0.1.9/replit_river/codegen/client.py
+-rw-r--r--   0        0        0     1903 2024-04-22 19:50:44.356956 replit_river-0.1.9/replit_river/codegen/run.py
+-rw-r--r--   0        0        0     5354 2024-04-24 23:49:28.777220 replit_river-0.1.9/replit_river/codegen/schema.py
+-rw-r--r--   0        0        0    12620 2024-04-24 23:49:28.805274 replit_river-0.1.9/replit_river/codegen/server.py
+-rw-r--r--   0        0        0      547 2024-04-22 19:50:44.357515 replit_river-0.1.9/replit_river/error_schema.py
+-rw-r--r--   0        0        0     1482 2024-04-24 23:40:20.838560 replit_river-0.1.9/replit_river/message_buffer.py
+-rw-r--r--   0        0        0     2606 2024-04-24 22:30:56.712779 replit_river-0.1.9/replit_river/messages.py
+-rw-r--r--   0        0        0        0 2024-04-22 19:50:44.358418 replit_river-0.1.9/replit_river/py.typed
+-rw-r--r--   0        0        0     3565 2024-04-24 23:49:26.772845 replit_river-0.1.9/replit_river/rate_limiter.py
+-rw-r--r--   0        0        0    12635 2024-04-24 23:47:43.465686 replit_river-0.1.9/replit_river/rpc.py
+-rw-r--r--   0        0        0     2293 2024-04-24 23:14:37.024811 replit_river-0.1.9/replit_river/seq_manager.py
+-rw-r--r--   0        0        0     2434 2024-04-25 06:45:22.487490 replit_river-0.1.9/replit_river/server.py
+-rw-r--r--   0        0        0     5916 2024-04-24 23:47:43.421824 replit_river-0.1.9/replit_river/server_transport.py
+-rw-r--r--   0        0        0    20444 2024-04-24 23:43:54.064753 replit_river-0.1.9/replit_river/session.py
+-rw-r--r--   0        0        0     3833 2024-04-24 23:37:26.072767 replit_river-0.1.9/replit_river/task_manager.py
+-rw-r--r--   0        0        0     5524 2024-04-24 23:48:34.430006 replit_river-0.1.9/replit_river/transport.py
+-rw-r--r--   0        0        0     1610 2024-04-25 00:05:48.843822 replit_river-0.1.9/replit_river/transport_options.py
+-rw-r--r--   0        0        0     2446 1970-01-01 00:00:00.000000 replit_river-0.1.9/PKG-INFO
```

### Comparing `replit_river-0.1.8/LICENSE` & `replit_river-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.8/README.md` & `replit_river-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.8/pyproject.toml` & `replit_river-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name="replit-river"
-version="0.1.8"
+version="0.1.9"
 description="Replit river toolkit for Python"
 authors = ["Replit <eng@replit.com>"]
 license = "LICENSE"
 keywords = ["rpc", "websockets"]
 readme = "README.md"
 
 [tool.poetry.scripts]
```

### Comparing `replit_river-0.1.8/replit_river/client.py` & `replit_river-0.1.9/replit_river/client.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.8/replit_river/client_session.py` & `replit_river-0.1.9/replit_river/client_session.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.8/replit_river/client_transport.py` & `replit_river-0.1.9/replit_river/client_transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,21 +287,28 @@
             )
         except FailedSendingMessageException:
             raise RiverException(
                 ERROR_CODE_STREAM_CLOSED, "Stream closed before response"
             )
         logging.debug("river client waiting for handshake response")
         try:
-            response_msg = await self._get_handshake_response_msg(websocket)
+            response_msg = await asyncio.wait_for(
+                self._get_handshake_response_msg(websocket),
+                timeout=self._transport_options.session_disconnect_grace_ms / 1000,
+            )
             handshake_response = ControlMessageHandshakeResponse(**response_msg.payload)
             logging.debug(
                 "river client get handshake response : %r", handshake_response
             )
         except ValidationError as e:
             raise RiverException(
                 ERROR_HANDSHAKE, f"Failed to parse handshake response : {e}"
             )
+        except asyncio.TimeoutError:
+            raise RiverException(
+                ERROR_HANDSHAKE, "Handshake response timeout, closing connection"
+            )
         if not handshake_response.status.ok:
             raise RiverException(
                 ERROR_HANDSHAKE, f"Handshake failed: {handshake_response.status.reason}"
             )
         return handshake_request, handshake_response
```

### Comparing `replit_river-0.1.8/replit_river/codegen/client.py` & `replit_river-0.1.9/replit_river/codegen/client.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.8/replit_river/codegen/run.py` & `replit_river-0.1.9/replit_river/codegen/run.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.8/replit_river/codegen/schema.py` & `replit_river-0.1.9/replit_river/codegen/schema.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.8/replit_river/codegen/server.py` & `replit_river-0.1.9/replit_river/codegen/server.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.8/replit_river/error_schema.py` & `replit_river-0.1.9/replit_river/error_schema.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.8/replit_river/message_buffer.py` & `replit_river-0.1.9/replit_river/message_buffer.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.8/replit_river/messages.py` & `replit_river-0.1.9/replit_river/messages.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.8/replit_river/rate_limiter.py` & `replit_river-0.1.9/replit_river/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.8/replit_river/rpc.py` & `replit_river-0.1.9/replit_river/rpc.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.8/replit_river/seq_manager.py` & `replit_river-0.1.9/replit_river/seq_manager.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.8/replit_river/server.py` & `replit_river-0.1.9/replit_river/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import logging
 from typing import Mapping, Tuple
 
 from websockets.exceptions import ConnectionClosed
 from websockets.server import WebSocketServerProtocol
 
 from replit_river.server_transport import ServerTransport
@@ -34,15 +35,18 @@
         self._transport._handlers.update(rpc_handlers)
 
     async def serve(self, websocket: WebSocketServerProtocol) -> None:
         logging.debug(
             "River server started establishing session with ws: %s", websocket.id
         )
         try:
-            session = await self._transport.handshake_to_get_session(websocket)
+            session = await asyncio.wait_for(
+                self._transport.handshake_to_get_session(websocket),
+                self._transport_options.session_disconnect_grace_ms / 1000,
+            )
         except Exception as e:
             logging.error(
                 f"Error establishing handshake, closing websocket: {e}", exc_info=True
             )
             await websocket.close()
             return
         logging.debug("River server session established, start serving messages")
```

### Comparing `replit_river-0.1.8/replit_river/server_transport.py` & `replit_river-0.1.9/replit_river/server_transport.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.8/replit_river/session.py` & `replit_river-0.1.9/replit_river/session.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.8/replit_river/task_manager.py` & `replit_river-0.1.9/replit_river/task_manager.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.8/replit_river/transport.py` & `replit_river-0.1.9/replit_river/transport.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.8/replit_river/transport_options.py` & `replit_river-0.1.9/replit_river/transport_options.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.8/PKG-INFO` & `replit_river-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replit-river
-Version: 0.1.8
+Version: 0.1.9
 Summary: Replit river toolkit for Python
 License: LICENSE
 Keywords: rpc,websockets
 Author: Replit
 Author-email: eng@replit.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
```

