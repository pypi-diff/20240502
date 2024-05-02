# Comparing `tmp/pycrdt_websocket-0.13.0.tar.gz` & `tmp/pycrdt_websocket-0.13.1.tar.gz`

## Comparing `pycrdt_websocket-0.13.0.tar` & `pycrdt_websocket-0.13.1.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/__init__.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/asgi_server.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/awareness.py
--rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/django_channels_consumer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/py.typed
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/websocket.py
--rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/websocket_provider.py
--rw-r--r--   0        0        0     7196 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/websocket_server.py
--rw-r--r--   0        0        0     9173 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/yroom.py
--rw-r--r--   0        0        0    16163 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/ystore.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pycrdt_websocket/yutils.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/tests/conftest.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/tests/package.json
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/tests/test_asgi.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/tests/test_pycrdt_yjs.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/tests/test_ystore.py
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/tests/utils.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/tests/yjs_client_0.js
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/tests/yjs_client_1.js
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/LICENSE
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/README.md
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/pyproject.toml
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.0/PKG-INFO
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/pycrdt_websocket/__init__.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/pycrdt_websocket/asgi_server.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/pycrdt_websocket/awareness.py
+-rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/pycrdt_websocket/django_channels_consumer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/pycrdt_websocket/py.typed
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/pycrdt_websocket/websocket.py
+-rw-r--r--   0        0        0     4922 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/pycrdt_websocket/websocket_provider.py
+-rw-r--r--   0        0        0     8412 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/pycrdt_websocket/websocket_server.py
+-rw-r--r--   0        0        0    10700 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/pycrdt_websocket/yroom.py
+-rw-r--r--   0        0        0    16163 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/pycrdt_websocket/ystore.py
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/pycrdt_websocket/yutils.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/tests/conftest.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/tests/package.json
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/tests/test_asgi.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/tests/test_pycrdt_yjs.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/tests/test_server.py
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/tests/test_yroom.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/tests/test_ystore.py
+-rw-r--r--   0        0        0     3074 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/tests/utils.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/tests/yjs_client_0.js
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/tests/yjs_client_1.js
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/LICENSE
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/README.md
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/pyproject.toml
+-rw-r--r--   0        0        0     5273 2020-02-02 00:00:00.000000 pycrdt_websocket-0.13.1/PKG-INFO
```

### Comparing `pycrdt_websocket-0.13.0/pycrdt_websocket/asgi_server.py` & `pycrdt_websocket-0.13.1/pycrdt_websocket/asgi_server.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.0/pycrdt_websocket/awareness.py` & `pycrdt_websocket-0.13.1/pycrdt_websocket/awareness.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.0/pycrdt_websocket/django_channels_consumer.py` & `pycrdt_websocket-0.13.1/pycrdt_websocket/django_channels_consumer.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.0/pycrdt_websocket/websocket.py` & `pycrdt_websocket-0.13.1/pycrdt_websocket/websocket.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.0/pycrdt_websocket/websocket_provider.py` & `pycrdt_websocket-0.13.1/pycrdt_websocket/websocket_provider.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.0/pycrdt_websocket/websocket_server.py` & `pycrdt_websocket-0.13.1/pycrdt_websocket/websocket_server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 from __future__ import annotations
 
 from contextlib import AsyncExitStack
 from functools import partial
 from logging import Logger, getLogger
+from typing import Callable
 
 from anyio import TASK_STATUS_IGNORED, Event, Lock, create_task_group
 from anyio.abc import TaskGroup, TaskStatus
 
 from .websocket import Websocket
 from .yroom import YRoom
 
 
 class WebsocketServer:
     """WebSocket server."""
 
     auto_clean_rooms: bool
     rooms: dict[str, YRoom]
     _started: Event | None = None
+    _stopped: Event
     _task_group: TaskGroup | None = None
     __start_lock: Lock | None = None
 
     def __init__(
-        self, rooms_ready: bool = True, auto_clean_rooms: bool = True, log: Logger | None = None
+        self,
+        rooms_ready: bool = True,
+        auto_clean_rooms: bool = True,
+        exception_handler: Callable[[Exception, Logger], bool] | None = None,
+        log: Logger | None = None,
     ) -> None:
         """Initialize the object.
 
         The WebsocketServer instance should preferably be used as an async context manager:
         ```py
         async with websocket_server:
             ...
@@ -37,20 +43,24 @@
         ...
         await websocket_server.stop()
         ```
 
         Arguments:
             rooms_ready: Whether rooms are ready to be synchronized when opened.
             auto_clean_rooms: Whether rooms should be deleted when no client is there anymore.
+            exception_handler: An optional callback to call when an exception is raised, that
+                returns True if the exception was handled.
             log: An optional logger.
         """
         self.rooms_ready = rooms_ready
         self.auto_clean_rooms = auto_clean_rooms
+        self.exception_handler = exception_handler
         self.log = log or getLogger(__name__)
         self.rooms = {}
+        self._stopped = Event()
 
     @property
     def started(self) -> Event:
         """An async event that is set when the WebSocket server has started."""
         if self._started is None:
             self._started = Event()
         return self._started
@@ -142,43 +152,47 @@
         """
         if self._task_group is None:
             raise RuntimeError(
                 "The WebsocketServer is not running: use `async with websocket_server:` or "
                 "`await websocket_server.start()`"
             )
 
-        async with create_task_group() as tg:
-            tg.start_soon(self._serve, websocket, tg)
-
-    async def _serve(self, websocket: Websocket, tg: TaskGroup):
-        room = await self.get_room(websocket.path)
-        await self.start_room(room)
-        await room.serve(websocket)
-
-        if self.auto_clean_rooms and not room.clients:
-            await self.delete_room(room=room)
-        tg.cancel_scope.cancel()
+        try:
+            async with create_task_group():
+                room = await self.get_room(websocket.path)
+                await self.start_room(room)
+                await room.serve(websocket)
+                if self.auto_clean_rooms and not room.clients:
+                    await self.delete_room(room=room)
+        except Exception as exception:
+            self._handle_exception(exception)
 
     async def __aenter__(self) -> WebsocketServer:
         async with self._start_lock:
             if self._task_group is not None:
                 raise RuntimeError("WebsocketServer already running")
 
             async with AsyncExitStack() as exit_stack:
-                tg = create_task_group()
-                self._task_group = await exit_stack.enter_async_context(tg)
+                self._task_group = await exit_stack.enter_async_context(create_task_group())
                 self._exit_stack = exit_stack.pop_all()
-                await tg.start(partial(self.start, from_context_manager=True))
+                await self._task_group.start(partial(self.start, from_context_manager=True))
 
         return self
 
     async def __aexit__(self, exc_type, exc_value, exc_tb):
         await self.stop()
         return await self._exit_stack.__aexit__(exc_type, exc_value, exc_tb)
 
+    def _handle_exception(self, exception: Exception) -> None:
+        exception_handled = False
+        if self.exception_handler is not None:
+            exception_handled = self.exception_handler(exception, self.log)
+        if not exception_handled:
+            raise exception
+
     async def start(
         self,
         *,
         task_status: TaskStatus[None] = TASK_STATUS_IGNORED,
         from_context_manager: bool = False,
     ):
         """Start the WebSocket server.
@@ -186,28 +200,41 @@
         Arguments:
             task_status: The status to set when the task has started.
         """
         if from_context_manager:
             task_status.started()
             self.started.set()
             assert self._task_group is not None
-            # wait forever
-            self._task_group.start_soon(Event().wait)
+            # wait until stopped
+            self._task_group.start_soon(self._stopped.wait)
             return
 
         async with self._start_lock:
             if self._task_group is not None:
                 raise RuntimeError("WebsocketServer already running")
 
-            async with create_task_group() as self._task_group:
-                task_status.started()
-                self.started.set()
-                # wait forever
-                self._task_group.start_soon(Event().wait)
+            while True:
+                try:
+                    async with create_task_group() as self._task_group:
+                        if not self.started.is_set():
+                            task_status.started()
+                            self.started.set()
+                        # wait until stopped
+                        self._task_group.start_soon(self._stopped.wait)
+                    return
+                except Exception as exception:
+                    self._handle_exception(exception)
 
     async def stop(self) -> None:
         """Stop the WebSocket server."""
         if self._task_group is None:
             raise RuntimeError("WebsocketServer not running")
 
+        self._stopped.set()
         self._task_group.cancel_scope.cancel()
         self._task_group = None
+
+
+def exception_logger(exception: Exception, log: Logger) -> bool:
+    """An exception handler that logs the exception and discards it."""
+    log.error("WebsocketServer exception", exc_info=exception)
+    return True  # the exception was handled
```

### Comparing `pycrdt_websocket-0.13.0/pycrdt_websocket/yroom.py` & `pycrdt_websocket-0.13.1/pycrdt_websocket/yroom.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,19 +35,24 @@
     ystore: BaseYStore | None
     ready_event: Event
     _on_message: Callable[[bytes], Awaitable[bool] | bool] | None
     _update_send_stream: MemoryObjectSendStream
     _update_receive_stream: MemoryObjectReceiveStream
     _task_group: TaskGroup | None = None
     _started: Event | None = None
+    _stopped: Event
     __start_lock: Lock | None = None
     _subscription: Subscription | None = None
 
     def __init__(
-        self, ready: bool = True, ystore: BaseYStore | None = None, log: Logger | None = None
+        self,
+        ready: bool = True,
+        ystore: BaseYStore | None = None,
+        exception_handler: Callable[[Exception, Logger], bool] | None = None,
+        log: Logger | None = None,
     ):
         """Initialize the object.
 
         The YRoom instance should preferably be used as an async context manager:
         ```py
         async with room:
             ...
@@ -59,27 +64,28 @@
         ...
         await room.stop()
         ```
 
         Arguments:
             ready: Whether the internal YDoc is ready to be synchronized right away.
             ystore: An optional store in which to persist document updates.
+            exception_handler: An optional callback to call when an exception is raised, that
+            returns True if the exception was handled.
             log: An optional logger.
         """
         self.ydoc = Doc()
         self.awareness = Awareness(self.ydoc)
-        self._update_send_stream, self._update_receive_stream = create_memory_object_stream(
-            max_buffer_size=65536
-        )
         self.ready_event = Event()
         self.ready = ready
         self.ystore = ystore
         self.log = log or getLogger(__name__)
         self.clients = []
         self._on_message = None
+        self.exception_handler = exception_handler
+        self._stopped = Event()
 
     @property
     def _start_lock(self) -> Lock:
         if self.__start_lock is None:
             self.__start_lock = Lock()
         return self.__start_lock
 
@@ -134,89 +140,113 @@
         async with self._update_receive_stream:
             async for update in self._update_receive_stream:
                 if self._task_group.cancel_scope.cancel_called:
                     return
                 # broadcast internal ydoc's update to all clients, that includes changes from the
                 # clients and changes from the backend (out-of-band changes)
                 for client in self.clients:
-                    self.log.debug("Sending Y update to client with endpoint: %s", client.path)
-                    message = create_update_message(update)
-                    self._task_group.start_soon(client.send, message)
+                    try:
+                        self.log.debug("Sending Y update to client with endpoint: %s", client.path)
+                        message = create_update_message(update)
+                        self._task_group.start_soon(client.send, message)
+                    except Exception as exception:
+                        self._handle_exception(exception)
                 if self.ystore:
-                    self.log.debug("Writing Y update to YStore")
-                    self._task_group.start_soon(self.ystore.write, update)
+                    try:
+                        self._task_group.start_soon(self.ystore.write, update)
+                        self.log.debug("Writing Y update to YStore")
+                    except Exception as exception:
+                        self._handle_exception(exception)
 
     async def __aenter__(self) -> YRoom:
         async with self._start_lock:
             if self._task_group is not None:
                 raise RuntimeError("YRoom already running")
 
             async with AsyncExitStack() as exit_stack:
-                tg = create_task_group()
-                self._task_group = await exit_stack.enter_async_context(tg)
+                self._task_group = await exit_stack.enter_async_context(create_task_group())
                 self._exit_stack = exit_stack.pop_all()
-                await tg.start(partial(self.start, from_context_manager=True))
+                await self._task_group.start(partial(self.start, from_context_manager=True))
 
         return self
 
     async def __aexit__(self, exc_type, exc_value, exc_tb):
         await self.stop()
         return await self._exit_stack.__aexit__(exc_type, exc_value, exc_tb)
 
+    def _handle_exception(self, exception: Exception) -> None:
+        exception_handled = False
+        if self.exception_handler is not None:
+            exception_handled = self.exception_handler(exception, self.log)
+        if not exception_handled:
+            raise exception
+
     async def start(
         self,
         *,
         task_status: TaskStatus[None] = TASK_STATUS_IGNORED,
         from_context_manager: bool = False,
     ):
         """Start the room.
 
         Arguments:
             task_status: The status to set when the task has started.
         """
         if from_context_manager:
             task_status.started()
             self.started.set()
+            self._update_send_stream, self._update_receive_stream = create_memory_object_stream(
+                max_buffer_size=65536
+            )
             assert self._task_group is not None
+            self._task_group.start_soon(self._stopped.wait)
+            self._task_group.start_soon(self._watch_ready)
             self._task_group.start_soon(self._broadcast_updates)
             return
 
         async with self._start_lock:
             if self._task_group is not None:
                 raise RuntimeError("YRoom already running")
 
-            async with create_task_group() as self._task_group:
-                task_status.started()
-                self.started.set()
-                self._task_group.start_soon(self._broadcast_updates)
-                self._task_group.start_soon(self._watch_ready)
+            while True:
+                try:
+                    async with create_task_group() as self._task_group:
+                        if not self.started.is_set():
+                            task_status.started()
+                            self.started.set()
+                        self._update_send_stream, self._update_receive_stream = (
+                            create_memory_object_stream(max_buffer_size=65536)
+                        )
+                        self._task_group.start_soon(self._stopped.wait)
+                        self._task_group.start_soon(self._watch_ready)
+                        self._task_group.start_soon(self._broadcast_updates)
+                    return
+                except Exception as exception:
+                    self._handle_exception(exception)
 
     async def stop(self) -> None:
         """Stop the room."""
         if self._task_group is None:
             raise RuntimeError("YRoom not running")
-
-        if self._task_group is None:
-            return
-
+        self._stopped.set()
         self._task_group.cancel_scope.cancel()
         self._task_group = None
         if self._subscription is not None:
             self.ydoc.unobserve(self._subscription)
 
     async def serve(self, websocket: Websocket):
         """Serve a client.
 
         Arguments:
             websocket: The WebSocket through which to serve the client.
         """
-        async with create_task_group() as tg:
-            self.clients.append(websocket)
-            await sync(self.ydoc, websocket, self.log)
-            try:
+        try:
+            async with create_task_group() as tg:
+                self.clients.append(websocket)
+                await sync(self.ydoc, websocket, self.log)
                 async for message in websocket:
                     # filter messages (e.g. awareness)
                     skip = False
                     if self.on_message:
                         _skip = self.on_message(message)
                         skip = await _skip if isawaitable(_skip) else _skip
                     if skip:
@@ -241,12 +271,11 @@
                             self.log.debug(
                                 "Sending Y awareness from client with endpoint "
                                 "%s to client with endpoint: %s",
                                 websocket.path,
                                 client.path,
                             )
                             tg.start_soon(client.send, message)
-            except Exception as e:
-                self.log.debug("Error serving endpoint: %s", websocket.path, exc_info=e)
-
-            # remove this client
-            self.clients = [c for c in self.clients if c != websocket]
+                # remove this client
+                self.clients = [c for c in self.clients if c != websocket]
+        except Exception as exception:
+            self._handle_exception(exception)
```

### Comparing `pycrdt_websocket-0.13.0/pycrdt_websocket/ystore.py` & `pycrdt_websocket-0.13.1/pycrdt_websocket/ystore.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.0/pycrdt_websocket/yutils.py` & `pycrdt_websocket-0.13.1/pycrdt_websocket/yutils.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.0/tests/conftest.py` & `pycrdt_websocket-0.13.1/tests/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,24 +5,44 @@
 
 import pytest
 from anyio import Event, create_task_group
 from httpx_ws import aconnect_ws
 from hypercorn import Config
 from pycrdt import Doc
 from sniffio import current_async_library
-from utils import StartStopContextManager, Websocket, ensure_server_running
+from utils import StartStopContextManager, Websocket, connected_websockets, ensure_server_running
 
-from pycrdt_websocket import ASGIServer, WebsocketProvider, WebsocketServer
+from pycrdt_websocket import ASGIServer, WebsocketProvider, WebsocketServer, YRoom
 
 
 @pytest.fixture(params=("websocket_server_context_manager", "websocket_server_start_stop"))
 def websocket_server_api(request):
     return request.param
 
 
+@pytest.fixture(params=("websocket_provider_context_manager", "websocket_provider_start_stop"))
+def websocket_provider_api(request):
+    return request.param
+
+
+@pytest.fixture(params=("yroom_context_manager", "yroom_start_stop"))
+def yroom_api(request):
+    return request.param
+
+
+@pytest.fixture(params=("real_websocket",))
+def websocket_provider_connect(request):
+    return request.param
+
+
+@pytest.fixture(params=("ystore_context_manager", "ystore_start_stop"))
+def ystore_api(request):
+    return request.param
+
+
 @pytest.fixture
 async def yws_server(request, unused_tcp_port, websocket_server_api):
     try:
         async with create_task_group() as tg:
             try:
                 kwargs = request.param
             except AttributeError:
@@ -40,54 +60,69 @@
                 from hypercorn.asyncio import serve
             async with websocket_server as websocket_server:
                 tg.start_soon(
                     partial(serve, app, config, shutdown_trigger=shutdown_event.wait, mode="asgi")
                 )
                 await ensure_server_running("localhost", unused_tcp_port)
                 pytest.port = unused_tcp_port
-                yield unused_tcp_port
+                yield unused_tcp_port, websocket_server
                 shutdown_event.set()
     except Exception:
         pass
 
 
-@pytest.fixture(params=("websocket_provider_context_manager", "websocket_provider_start_stop"))
-def websocket_provider_api(request):
-    return request.param
-
-
 @pytest.fixture
-def yws_provider_factory(room_name, websocket_provider_api):
+def yws_provider_factory(room_name, websocket_provider_api, websocket_provider_connect):
     @asynccontextmanager
     async def factory():
         ydoc = Doc()
-        async with aconnect_ws(f"http://localhost:{pytest.port}/{room_name}") as websocket:
+        if websocket_provider_connect == "real_websocket":
+            server_websocket = None
+            connect = aconnect_ws(f"http://localhost:{pytest.port}/{room_name}")
+        else:
+            server_websocket, connect = connected_websockets()
+        async with connect as websocket:
             async with create_task_group() as tg:
                 websocket_provider = WebsocketProvider(ydoc, Websocket(websocket, room_name))
                 if websocket_provider_api == "websocket_provider_start_stop":
                     websocket_provider = StartStopContextManager(websocket_provider, tg)
                 async with websocket_provider as websocket_provider:
-                    yield ydoc
+                    yield ydoc, server_websocket
 
     return factory
 
 
 @pytest.fixture
 async def yws_provider(yws_provider_factory):
-    async with yws_provider_factory() as ydoc:
-        yield ydoc
+    async with yws_provider_factory() as provider:
+        ydoc, server_websocket = provider
+        yield ydoc, server_websocket
 
 
 @pytest.fixture
 async def yws_providers(request, yws_provider_factory):
     number = request.param
     yield [yws_provider_factory() for idx in range(number)]
 
 
 @pytest.fixture
+async def yroom(request, yroom_api):
+    async with create_task_group() as tg:
+        try:
+            kwargs = request.param
+        except AttributeError:
+            kwargs = {}
+        room = YRoom(**kwargs)
+        if yroom_api == "yroom_start_stop":
+            room = StartStopContextManager(room, tg)
+        async with room as room:
+            yield room
+
+
+@pytest.fixture
 def yjs_client(request):
     client_id = request.param
     p = subprocess.Popen(["node", f"tests/yjs_client_{client_id}.js", str(pytest.port)])
     yield p
     p.kill()
```

### Comparing `pycrdt_websocket-0.13.0/tests/test_pycrdt_yjs.py` & `pycrdt_websocket-0.13.1/tests/test_pycrdt_yjs.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,25 +35,25 @@
     change_event = Event()
     subscription = ydata.observe(partial(callback, change_event, key))
     return Change(change_event, timeout, ydata, subscription, key)
 
 
 @pytest.mark.parametrize("yjs_client", [0], indirect=True)
 async def test_pycrdt_yjs_0(yws_server, yws_provider, yjs_client):
-    ydoc = yws_provider
+    ydoc, _ = yws_provider
     ydoc["map"] = ymap = Map()
     for v_in in range(10):
         ymap["in"] = float(v_in)
         v_out = await watch(ymap, "out").wait()
         assert v_out == v_in + 1.0
 
 
 @pytest.mark.parametrize("yjs_client", [1], indirect=True)
 async def test_pycrdt_yjs_1(yws_server, yws_provider, yjs_client):
-    ydoc = yws_provider
+    ydoc, _ = yws_provider
     ydoc["cells"] = ycells = Array()
     ydoc["state"] = ystate = Map()
     ycells_change = watch(ycells)
     ystate_change = watch(ystate)
     await ycells_change.wait()
     await ystate_change.wait()
     assert ycells.to_py() == [{"metadata": {"foo": "bar"}, "source": "1 + 2"}]
```

### Comparing `pycrdt_websocket-0.13.0/tests/test_ystore.py` & `pycrdt_websocket-0.13.1/tests/test_ystore.py`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.0/tests/utils.py` & `pycrdt_websocket-0.13.1/tests/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from anyio import Lock, connect_tcp
+from anyio import Lock, connect_tcp, create_memory_object_stream
 from pycrdt import Array, Doc
 
 
 class YDocTest:
     def __init__(self):
         self.ydoc = Doc()
         self.ydoc["array"] = self.array = Array()
@@ -56,14 +56,53 @@
             await self._websocket.send_bytes(message)
 
     async def recv(self) -> bytes:
         b = await self._websocket.receive_bytes()
         return bytes(b)
 
 
+class ClientWebsocket:
+    def __init__(self, server_websocket: "ServerWebsocket"):
+        self.server_websocket = server_websocket
+        self.send_stream, self.receive_stream = create_memory_object_stream[bytes](65536)
+
+    async def __aenter__(self):
+        return self
+
+    async def __aexit__(self, exc_type, exc_value, exc_tb):
+        pass
+
+    async def send_bytes(self, message: bytes) -> None:
+        await self.server_websocket.send_stream.send(message)
+
+    async def receive_bytes(self) -> bytes:
+        return await self.receive_stream.receive()
+
+
+class ServerWebsocket:
+    client_websocket: ClientWebsocket | None = None
+
+    def __init__(self):
+        self.send_stream, self.receive_stream = create_memory_object_stream[bytes](65536)
+
+    async def send_bytes(self, message: bytes) -> None:
+        assert self.client_websocket is not None
+        await self.client_websocket.send_stream.send(message)
+
+    async def receive_bytes(self) -> bytes:
+        return await self.receive_stream.receive()
+
+
+def connected_websockets() -> tuple[ServerWebsocket, ClientWebsocket]:
+    server_websocket = ServerWebsocket()
+    client_websocket = ClientWebsocket(server_websocket)
+    server_websocket.client_websocket = client_websocket
+    return server_websocket, client_websocket
+
+
 async def ensure_server_running(host: str, port: int) -> None:
     while True:
         try:
             await connect_tcp(host, port)
         except OSError:
             pass
         else:
```

### Comparing `pycrdt_websocket-0.13.0/tests/yjs_client_0.js` & `pycrdt_websocket-0.13.1/tests/yjs_client_0.js`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.0/tests/yjs_client_1.js` & `pycrdt_websocket-0.13.1/tests/yjs_client_1.js`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.0/.gitignore` & `pycrdt_websocket-0.13.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.0/LICENSE` & `pycrdt_websocket-0.13.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.0/README.md` & `pycrdt_websocket-0.13.1/README.md`

 * *Files identical despite different names*

### Comparing `pycrdt_websocket-0.13.0/pyproject.toml` & `pycrdt_websocket-0.13.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -31,17 +31,18 @@
     "anyio >=3.6.2,<5",
     "sqlite-anyio >=0.2.0,<0.3.0",
     "pycrdt >=0.8.16,<0.9.0",
 ]
 
 [project.optional-dependencies]
 test = [
-    "mypy",
+    "mypy !=1.10.0",  # see https://github.com/python/mypy/issues/17166
     "pre-commit",
     "pytest",
+    "pytest-timeout",
     "httpx-ws >=0.5.2",
     "hypercorn >=0.16.0",
     "trio >=0.25.0",
     "sniffio",
 ]
 docs = [
     "mkdocs",
```

### Comparing `pycrdt_websocket-0.13.0/PKG-INFO` & `pycrdt_websocket-0.13.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pycrdt-websocket
-Version: 0.13.0
+Version: 0.13.1
 Summary: WebSocket connector for pycrdt
 Project-URL: Homepage, https://github.com/jupyter-server/pycrdt-websocket
 Project-URL: Source, https://github.com/jupyter-server/pycrdt-websocket
 Project-URL: Issues, https://github.com/jupyter-server/pycrdt-websocket/issues
 Project-URL: Pypi, https://pypi.org/project/pycrdt-websocket
 Author-email: David Brochart <david.brochart@gmail.com>
 License: MIT License
@@ -48,17 +48,18 @@
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocstrings-python; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: httpx-ws>=0.5.2; extra == 'test'
 Requires-Dist: hypercorn>=0.16.0; extra == 'test'
-Requires-Dist: mypy; extra == 'test'
+Requires-Dist: mypy!=1.10.0; extra == 'test'
 Requires-Dist: pre-commit; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-timeout; extra == 'test'
 Requires-Dist: sniffio; extra == 'test'
 Requires-Dist: trio>=0.25.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Pycrdt-websocket
 
 Pycrdt-websocket is an async WebSocket connector for pycrdt.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: pycrdt-websocket Version: 0.13.0 Summary: WebSocket
+Metadata-Version: 2.3 Name: pycrdt-websocket Version: 0.13.1 Summary: WebSocket
 connector for pycrdt Project-URL: Homepage, https://github.com/jupyter-server/
 pycrdt-websocket Project-URL: Source, https://github.com/jupyter-server/pycrdt-
 websocket Project-URL: Issues, https://github.com/jupyter-server/pycrdt-
 websocket/issues Project-URL: Pypi, https://pypi.org/project/pycrdt-websocket
 Author-email: David Brochart
 gmail.com> License: MIT License Copyright (c) 2022 David Brochart Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
@@ -27,39 +27,40 @@
 Classifier: Programming Language :: Python :: 3.12 Requires-Python: >=3.8
 Requires-Dist: anyio<5,>=3.6.2 Requires-Dist: pycrdt<0.9.0,>=0.8.16 Requires-
 Dist: sqlite-anyio<0.3.0,>=0.2.0 Provides-Extra: django Requires-Dist:
 channels; extra == 'django' Provides-Extra: docs Requires-Dist: mkdocs; extra
 == 'docs' Requires-Dist: mkdocs-material; extra == 'docs' Requires-Dist:
 mkdocstrings-python; extra == 'docs' Provides-Extra: test Requires-Dist: httpx-
 ws>=0.5.2; extra == 'test' Requires-Dist: hypercorn>=0.16.0; extra == 'test'
-Requires-Dist: mypy; extra == 'test' Requires-Dist: pre-commit; extra == 'test'
-Requires-Dist: pytest; extra == 'test' Requires-Dist: sniffio; extra == 'test'
-Requires-Dist: trio>=0.25.0; extra == 'test' Description-Content-Type: text/
-markdown # Pycrdt-websocket Pycrdt-websocket is an async WebSocket connector
-for pycrdt. [![Build Status](https://github.com/jupyter-server/pycrdt-
-websocket/workflows/CI/badge.svg)](https://github.com/jupyter-server/pycrdt-
-websocket/actions) [![Code style: black](https://img.shields.io/badge/
-code%20style-black-000000.svg)](https://github.com/psf/black) --
-- **Documentation**: _h_t_t_p_s_:_/_/_j_u_p_y_t_e_r_-_s_e_r_v_e_r_._g_i_t_h_u_b_._i_o_/_p_y_c_r_d_t_-_w_e_b_s_o_c_k_e_t **Source
-Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_j_u_p_y_t_e_r_-_s_e_r_v_e_r_/_p_y_c_r_d_t_-_w_e_b_s_o_c_k_e_t --- Pycrdt-websocket
-is a Python library for building WebSocket servers and clients that connect and
-synchronize shared documents. It can be used to create collaborative web
-applications. The following diagram illustrates a typical architecture. The
-goal is to share a document among several clients. Each client has an instance
-of a `Doc`, representing their view of a document. A shared document also lives
-in a [room](./reference/Room.md) on the server side. Conceptually, a room can
-be seen as the place where clients collaborate on a document. The WebSocket to
-which a client connects points to the corresponding room through the endpoint
-path. In the example below, clients A and B connect to a WebSocket at path
-`room-1`, and thus both clients find themselves in a room called `room-1`. All
-the `Doc` synchronization logic is taken care of by the [WebsocketProvider](./
-reference/WebSocket_provider.md). Each update to a shared document can be
-persisted to disk using a [store](./reference/Store.md), which can be a file or
-a database. ```mermaid flowchart TD classDef room1 fill:#f96 classDef room2
-fill:#bbf A[Client A
+Requires-Dist: mypy!=1.10.0; extra == 'test' Requires-Dist: pre-commit; extra
+== 'test' Requires-Dist: pytest; extra == 'test' Requires-Dist: pytest-timeout;
+extra == 'test' Requires-Dist: sniffio; extra == 'test' Requires-Dist:
+trio>=0.25.0; extra == 'test' Description-Content-Type: text/markdown # Pycrdt-
+websocket Pycrdt-websocket is an async WebSocket connector for pycrdt. [![Build
+Status](https://github.com/jupyter-server/pycrdt-websocket/workflows/CI/
+badge.svg)](https://github.com/jupyter-server/pycrdt-websocket/actions) [![Code
+style: black](https://img.shields.io/badge/code%20style-black-000000.svg)]
+(https://github.com/psf/black) --- **Documentation**: _h_t_t_p_s_:_/_/_j_u_p_y_t_e_r_-
+_s_e_r_v_e_r_._g_i_t_h_u_b_._i_o_/_p_y_c_r_d_t_-_w_e_b_s_o_c_k_e_t **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_j_u_p_y_t_e_r_-
+_s_e_r_v_e_r_/_p_y_c_r_d_t_-_w_e_b_s_o_c_k_e_t --- Pycrdt-websocket is a Python library for building
+WebSocket servers and clients that connect and synchronize shared documents. It
+can be used to create collaborative web applications. The following diagram
+illustrates a typical architecture. The goal is to share a document among
+several clients. Each client has an instance of a `Doc`, representing their
+view of a document. A shared document also lives in a [room](./reference/
+Room.md) on the server side. Conceptually, a room can be seen as the place
+where clients collaborate on a document. The WebSocket to which a client
+connects points to the corresponding room through the endpoint path. In the
+example below, clients A and B connect to a WebSocket at path `room-1`, and
+thus both clients find themselves in a room called `room-1`. All the `Doc`
+synchronization logic is taken care of by the [WebsocketProvider](./reference/
+WebSocket_provider.md). Each update to a shared document can be persisted to
+disk using a [store](./reference/Store.md), which can be a file or a database.
+```mermaid flowchart TD classDef room1 fill:#f96 classDef room2 fill:#bbf A
+[Client A
 room-1]:::room1 <-->|WebSocket
 Provider| server(WebSocket Server) B[Client B
 room-1]:::room1 <-->|WebSocket
 Provider| server C[Client C
 room-2]:::room2 <-->|WebSocket
 Provider| server D[Client D
 room-2]:::room2 <-->|WebSocket
```

