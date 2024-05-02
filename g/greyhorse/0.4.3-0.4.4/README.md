# Comparing `tmp/greyhorse-0.4.3.tar.gz` & `tmp/greyhorse-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greyhorse-0.4.3.tar", max compression
+gzip compressed data, was "greyhorse-0.4.4.tar", max compression
```

## Comparing `greyhorse-0.4.3.tar` & `greyhorse-0.4.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.3/greyhorse/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.3/greyhorse/app/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.3/greyhorse/app/builders/__init__.py
--rw-r--r--   0        0        0    12549 2024-04-28 16:06:53.142337 greyhorse-0.4.3/greyhorse/app/builders/module.py
--rw-r--r--   0        0        0    12327 2024-04-21 00:04:20.478630 greyhorse-0.4.3/greyhorse/app/context.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.3/greyhorse/app/entities/__init__.py
--rw-r--r--   0        0        0     8384 2024-04-28 15:34:05.766225 greyhorse-0.4.3/greyhorse/app/entities/application.py
--rw-r--r--   0        0        0     4812 2024-04-14 12:30:24.508646 greyhorse-0.4.3/greyhorse/app/entities/controller.py
--rw-r--r--   0        0        0      910 2024-04-14 12:24:31.419245 greyhorse-0.4.3/greyhorse/app/entities/deps.py
--rw-r--r--   0        0        0    19413 2024-04-17 16:38:43.638882 greyhorse-0.4.3/greyhorse/app/entities/module.py
--rw-r--r--   0        0        0      253 2024-04-18 23:28:44.736666 greyhorse-0.4.3/greyhorse/app/entities/operator.py
--rw-r--r--   0        0        0     2903 2024-04-20 10:49:17.227923 greyhorse-0.4.3/greyhorse/app/entities/providers.py
--rw-r--r--   0        0        0     7355 2024-04-28 16:15:29.403350 greyhorse-0.4.3/greyhorse/app/entities/service.py
--rw-r--r--   0        0        0     1528 2024-04-10 15:13:55.985794 greyhorse-0.4.3/greyhorse/app/errors.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.965597 greyhorse-0.4.3/greyhorse/app/schemas/__init__.py
--rw-r--r--   0        0        0      883 2024-04-20 11:54:14.943578 greyhorse-0.4.3/greyhorse/app/schemas/components.py
--rw-r--r--   0        0        0      587 2024-04-20 11:54:14.975577 greyhorse-0.4.3/greyhorse/app/schemas/controller.py
--rw-r--r--   0        0        0     1762 2024-04-20 11:54:14.955577 greyhorse-0.4.3/greyhorse/app/schemas/module.py
--rw-r--r--   0        0        0      590 2024-04-20 11:54:14.963577 greyhorse-0.4.3/greyhorse/app/schemas/service.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.3/greyhorse/app/tasks/__init__.py
--rw-r--r--   0        0        0     1308 2024-04-09 22:29:35.969597 greyhorse-0.4.3/greyhorse/app/tasks/app.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.3/greyhorse/app/utils/__init__.py
--rw-r--r--   0        0        0     6880 2024-04-17 14:33:40.645939 greyhorse-0.4.3/greyhorse/app/utils/registry.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.3/greyhorse/data/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.3/greyhorse/data/cache/__init__.py
--rw-r--r--   0        0        0     1909 2024-04-09 22:29:35.969597 greyhorse-0.4.3/greyhorse/data/cache/base.py
--rw-r--r--   0        0        0     2438 2024-04-09 22:29:35.969597 greyhorse-0.4.3/greyhorse/data/cache/method.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.3/greyhorse/data/models/__init__.py
--rw-r--r--   0        0        0     1868 2024-04-09 22:29:35.969597 greyhorse-0.4.3/greyhorse/data/models/base.py
--rw-r--r--   0        0        0     3575 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/data/models/fields.py
--rw-r--r--   0        0        0     2088 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/data/models/filterable.py
--rw-r--r--   0        0        0     4491 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/data/models/model.py
--rw-r--r--   0        0        0     1615 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/data/models/serializable.py
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/data/repositories/__init__.py
--rw-r--r--   0        0        0     2752 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/data/repositories/base.py
--rw-r--r--   0        0        0     2387 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/data/repositories/filterable.py
--rw-r--r--   0        0        0      117 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/data/serializers/__init__.py
--rw-r--r--   0        0        0      564 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/data/serializers/base.py
--rw-r--r--   0        0        0      513 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/data/serializers/pickle.py
--rw-r--r--   0        0        0     1902 2024-04-20 11:58:08.771261 greyhorse-0.4.3/greyhorse/data/storage.py
--rw-r--r--   0        0        0      131 2024-04-09 22:29:35.973597 greyhorse-0.4.3/greyhorse/i18n/__init__.py
--rw-r--r--   0        0        0     2663 2024-04-18 23:30:16.265809 greyhorse-0.4.3/greyhorse/i18n/translator.py
--rw-r--r--   0        0        0     1584 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/logging.py
--rw-r--r--   0        0        0     2575 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/messagebus.py
--rw-r--r--   0        0        0     4130 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/result.py
--rw-r--r--   0        0        0     3761 2024-04-10 15:15:08.074854 greyhorse-0.4.3/greyhorse/translations.toml
--rw-r--r--   0        0        0        0 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/utils/__init__.py
--rw-r--r--   0        0        0      397 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/utils/confs.py
--rw-r--r--   0        0        0     2169 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/utils/dicts.py
--rw-r--r--   0        0        0      568 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/utils/hashes.py
--rw-r--r--   0        0        0      959 2024-04-27 19:03:47.313480 greyhorse-0.4.3/greyhorse/utils/imports.py
--rw-r--r--   0        0        0     1157 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/utils/injectors.py
--rw-r--r--   0        0        0     1573 2024-04-20 10:13:14.653404 greyhorse-0.4.3/greyhorse/utils/invoke.py
--rw-r--r--   0        0        0      452 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/utils/json.py
--rw-r--r--   0        0        0      823 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/utils/strings.py
--rw-r--r--   0        0        0     1095 2024-04-09 22:29:35.977597 greyhorse-0.4.3/greyhorse/utils/time.py
--rw-r--r--   0        0        0     1040 2024-04-28 14:53:41.171207 greyhorse-0.4.3/pyproject.toml
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 greyhorse-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.4/greyhorse/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.4/greyhorse/app/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.4/greyhorse/app/builders/__init__.py
+-rw-r--r--   0        0        0    12549 2024-04-28 16:06:53.142337 greyhorse-0.4.4/greyhorse/app/builders/module.py
+-rw-r--r--   0        0        0    12598 2024-05-02 12:05:15.439265 greyhorse-0.4.4/greyhorse/app/context.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.961597 greyhorse-0.4.4/greyhorse/app/entities/__init__.py
+-rw-r--r--   0        0        0     8384 2024-04-28 15:34:05.766225 greyhorse-0.4.4/greyhorse/app/entities/application.py
+-rw-r--r--   0        0        0     4812 2024-04-14 12:30:24.508646 greyhorse-0.4.4/greyhorse/app/entities/controller.py
+-rw-r--r--   0        0        0      910 2024-04-14 12:24:31.419245 greyhorse-0.4.4/greyhorse/app/entities/deps.py
+-rw-r--r--   0        0        0    19413 2024-04-17 16:38:43.638882 greyhorse-0.4.4/greyhorse/app/entities/module.py
+-rw-r--r--   0        0        0      253 2024-04-18 23:28:44.736666 greyhorse-0.4.4/greyhorse/app/entities/operator.py
+-rw-r--r--   0        0        0     2903 2024-04-20 10:49:17.227923 greyhorse-0.4.4/greyhorse/app/entities/providers.py
+-rw-r--r--   0        0        0     7355 2024-04-28 16:15:29.403350 greyhorse-0.4.4/greyhorse/app/entities/service.py
+-rw-r--r--   0        0        0     1528 2024-04-10 15:13:55.985794 greyhorse-0.4.4/greyhorse/app/errors.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.965597 greyhorse-0.4.4/greyhorse/app/schemas/__init__.py
+-rw-r--r--   0        0        0      883 2024-04-20 11:54:14.943578 greyhorse-0.4.4/greyhorse/app/schemas/components.py
+-rw-r--r--   0        0        0      587 2024-04-20 11:54:14.975577 greyhorse-0.4.4/greyhorse/app/schemas/controller.py
+-rw-r--r--   0        0        0     1762 2024-04-20 11:54:14.955577 greyhorse-0.4.4/greyhorse/app/schemas/module.py
+-rw-r--r--   0        0        0      590 2024-04-20 11:54:14.963577 greyhorse-0.4.4/greyhorse/app/schemas/service.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.4/greyhorse/app/tasks/__init__.py
+-rw-r--r--   0        0        0     1308 2024-04-09 22:29:35.969597 greyhorse-0.4.4/greyhorse/app/tasks/app.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.4/greyhorse/app/utils/__init__.py
+-rw-r--r--   0        0        0     6880 2024-04-17 14:33:40.645939 greyhorse-0.4.4/greyhorse/app/utils/registry.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.4/greyhorse/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.4/greyhorse/data/cache/__init__.py
+-rw-r--r--   0        0        0     1909 2024-04-09 22:29:35.969597 greyhorse-0.4.4/greyhorse/data/cache/base.py
+-rw-r--r--   0        0        0     2438 2024-04-09 22:29:35.969597 greyhorse-0.4.4/greyhorse/data/cache/method.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.969597 greyhorse-0.4.4/greyhorse/data/models/__init__.py
+-rw-r--r--   0        0        0     1868 2024-04-09 22:29:35.969597 greyhorse-0.4.4/greyhorse/data/models/base.py
+-rw-r--r--   0        0        0     3575 2024-04-09 22:29:35.973597 greyhorse-0.4.4/greyhorse/data/models/fields.py
+-rw-r--r--   0        0        0     2088 2024-04-09 22:29:35.973597 greyhorse-0.4.4/greyhorse/data/models/filterable.py
+-rw-r--r--   0        0        0     4491 2024-04-09 22:29:35.973597 greyhorse-0.4.4/greyhorse/data/models/model.py
+-rw-r--r--   0        0        0     1615 2024-04-09 22:29:35.973597 greyhorse-0.4.4/greyhorse/data/models/serializable.py
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.973597 greyhorse-0.4.4/greyhorse/data/repositories/__init__.py
+-rw-r--r--   0        0        0     2752 2024-04-09 22:29:35.973597 greyhorse-0.4.4/greyhorse/data/repositories/base.py
+-rw-r--r--   0        0        0     2387 2024-04-09 22:29:35.973597 greyhorse-0.4.4/greyhorse/data/repositories/filterable.py
+-rw-r--r--   0        0        0      117 2024-04-09 22:29:35.973597 greyhorse-0.4.4/greyhorse/data/serializers/__init__.py
+-rw-r--r--   0        0        0      564 2024-04-09 22:29:35.973597 greyhorse-0.4.4/greyhorse/data/serializers/base.py
+-rw-r--r--   0        0        0      513 2024-04-09 22:29:35.973597 greyhorse-0.4.4/greyhorse/data/serializers/pickle.py
+-rw-r--r--   0        0        0     1902 2024-04-20 11:58:08.771261 greyhorse-0.4.4/greyhorse/data/storage.py
+-rw-r--r--   0        0        0      131 2024-04-09 22:29:35.973597 greyhorse-0.4.4/greyhorse/i18n/__init__.py
+-rw-r--r--   0        0        0     2663 2024-04-18 23:30:16.265809 greyhorse-0.4.4/greyhorse/i18n/translator.py
+-rw-r--r--   0        0        0     1584 2024-04-09 22:29:35.977597 greyhorse-0.4.4/greyhorse/logging.py
+-rw-r--r--   0        0        0     2575 2024-04-09 22:29:35.977597 greyhorse-0.4.4/greyhorse/messagebus.py
+-rw-r--r--   0        0        0     4130 2024-04-09 22:29:35.977597 greyhorse-0.4.4/greyhorse/result.py
+-rw-r--r--   0        0        0     3761 2024-04-10 15:15:08.074854 greyhorse-0.4.4/greyhorse/translations.toml
+-rw-r--r--   0        0        0        0 2024-04-09 22:29:35.977597 greyhorse-0.4.4/greyhorse/utils/__init__.py
+-rw-r--r--   0        0        0      397 2024-04-09 22:29:35.977597 greyhorse-0.4.4/greyhorse/utils/confs.py
+-rw-r--r--   0        0        0     2169 2024-04-09 22:29:35.977597 greyhorse-0.4.4/greyhorse/utils/dicts.py
+-rw-r--r--   0        0        0      568 2024-04-09 22:29:35.977597 greyhorse-0.4.4/greyhorse/utils/hashes.py
+-rw-r--r--   0        0        0      959 2024-04-27 19:03:47.313480 greyhorse-0.4.4/greyhorse/utils/imports.py
+-rw-r--r--   0        0        0     1157 2024-04-09 22:29:35.977597 greyhorse-0.4.4/greyhorse/utils/injectors.py
+-rw-r--r--   0        0        0     2085 2024-05-02 12:20:02.517559 greyhorse-0.4.4/greyhorse/utils/invoke.py
+-rw-r--r--   0        0        0      452 2024-04-09 22:29:35.977597 greyhorse-0.4.4/greyhorse/utils/json.py
+-rw-r--r--   0        0        0      823 2024-04-09 22:29:35.977597 greyhorse-0.4.4/greyhorse/utils/strings.py
+-rw-r--r--   0        0        0     1095 2024-04-09 22:29:35.977597 greyhorse-0.4.4/greyhorse/utils/time.py
+-rw-r--r--   0        0        0     1040 2024-05-02 12:03:56.846677 greyhorse-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 greyhorse-0.4.4/PKG-INFO
```

### Comparing `greyhorse-0.4.3/greyhorse/app/builders/module.py` & `greyhorse-0.4.4/greyhorse/app/builders/module.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/app/context.py` & `greyhorse-0.4.4/greyhorse/app/context.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 import asyncio
-import inspect
 import threading
 from collections import defaultdict
 from contextlib import AbstractAsyncContextManager, AbstractContextManager, AsyncExitStack, ExitStack
 from contextvars import ContextVar
 from typing import Any, AsyncContextManager, Awaitable, Callable, ContextManager, Mapping, override
 from uuid import uuid4
 
-from greyhorse.utils.invoke import get_asyncio_loop, invoke_async, invoke_sync
+from greyhorse.utils.invoke import get_asyncio_loop, invoke_async, invoke_sync, is_like_sync_context_manager, \
+    is_like_async_context_manager
 
 type FieldFactory[T] = (
     T | Callable[[], Awaitable[T] | T] |
+    AbstractContextManager[T] | AbstractAsyncContextManager[T] |
+    Callable[[], AbstractContextManager[T]] | Callable[[], AbstractAsyncContextManager[T]]
+)
+
+
+type ContextManagerLike[T] = (
+    AbstractContextManager[T] | AbstractAsyncContextManager[T] |
     Callable[[], AbstractContextManager[T]] | Callable[[], AbstractAsyncContextManager[T]]
 )
 
 
 class Context(object):
     __slots__ = (
         '_factory', '_field_factories', '_finalizers',
@@ -100,32 +107,34 @@
         '_sync_stack', '_sub_contexts', '_counter', '_lock',
     )
 
     def __init__(
         self, factory: Callable[[...], T] | None = None,
         fields: Mapping[str, FieldFactory[T]] | None = None,
         finalizers: list[Callable[[], Awaitable[None] | None]] | None = None,
-        contexts: list[Callable[[], AbstractContextManager[T]]] | None = None,
+        contexts: list[ContextManagerLike[T]] | None = None,
     ):
         super().__init__(factory, fields, finalizers)
         self._sync_stack = ExitStack()
-        self._sub_contexts: list[tuple[Callable[[], AbstractContextManager[T]], str | None]] = []
+        self._sub_contexts: list[tuple[ContextManagerLike, str | None]] = []
         self._counter = 0
         self._lock = threading.Lock()
 
         if contexts:
-            self._sub_contexts = [(ctx, None) for ctx in contexts]
+            for ctx in contexts:
+                if is_like_sync_context_manager(ctx):
+                    self._sub_contexts.append((ctx, None))
 
         names_to_remove = []
 
         for name, factory in self._field_factories.items():
-            if inspect.isgeneratorfunction(inspect.unwrap(factory)):
+            if is_like_sync_context_manager(factory):
                 self._sub_contexts.append((factory, name))
                 names_to_remove.append(name)
-            elif inspect.isasyncgenfunction(inspect.unwrap(factory)):
+            elif is_like_async_context_manager(factory):
                 names_to_remove.append(name)
 
         for name in names_to_remove:
             self._field_factories.pop(name)
 
     def _create(self):
         if self._factory is not None:
@@ -148,15 +157,17 @@
             if 1 != self._counter:
                 self._nested_enter()
                 return self._object
 
         self._sync_stack.__enter__()
 
         for ctx, field in self._sub_contexts:
-            if value := self._sync_stack.enter_context(ctx()):
+            if callable(ctx):
+                ctx = ctx()
+            if value := self._sync_stack.enter_context(ctx):
                 if field is not None:
                     self._params[field] = value
 
         for name, value in self._field_factories.items():
             if callable(value):
                 value = invoke_sync(value)
             self._params[name] = value
@@ -212,38 +223,38 @@
         '_async_sub_contexts', '_counter', '_lock',
     )
 
     def __init__(
         self, factory: Callable[[...], T] | None = None,
         fields: Mapping[str, FieldFactory[T]] | None = None,
         finalizers: list[Callable[[], Awaitable[None] | None]] | None = None,
-        contexts: list[Callable[[], AbstractContextManager[T] | AbstractAsyncContextManager[T]]] | None = None,
+        contexts: list[ContextManagerLike[T]] | None = None,
     ):
         super().__init__(factory, fields, finalizers)
         self._sync_stack = ExitStack()
         self._async_stack = AsyncExitStack()
-        self._sync_sub_contexts: list[tuple[Callable[[], AbstractContextManager[T]], str | None]] = []
-        self._async_sub_contexts: list[tuple[Callable[[], AbstractAsyncContextManager[T]], str | None]] = []
+        self._sync_sub_contexts: list[tuple[ContextManagerLike[T], str | None]] = []
+        self._async_sub_contexts: list[tuple[ContextManagerLike[T], str | None]] = []
         self._counter = 0
         self._lock = asyncio.Lock()
 
         if contexts:
             for ctx in contexts:
-                if inspect.isasyncgenfunction(inspect.unwrap(ctx)):
+                if is_like_async_context_manager(ctx):
                     self._async_sub_contexts.append((ctx, None))
-                elif inspect.isgeneratorfunction(inspect.unwrap(ctx)):
+                elif is_like_sync_context_manager(ctx):
                     self._sync_sub_contexts.append((ctx, None))
 
         names_to_remove = []
 
         for name, factory in self._field_factories.items():
-            if inspect.isasyncgenfunction(inspect.unwrap(factory)):
+            if is_like_async_context_manager(factory):
                 self._async_sub_contexts.append((factory, name))
                 names_to_remove.append(name)
-            elif inspect.isgeneratorfunction(inspect.unwrap(factory)):
+            elif is_like_sync_context_manager(factory):
                 self._sync_sub_contexts.append((factory, name))
                 names_to_remove.append(name)
 
         for name in names_to_remove:
             self._field_factories.pop(name)
 
     async def _create(self):
@@ -268,20 +279,24 @@
                 await self._nested_enter()
                 return self._object
 
         self._sync_stack.__enter__()
         await self._async_stack.__aenter__()
 
         for ctx, field in self._sync_sub_contexts:
-            if value := self._sync_stack.enter_context(ctx()):
+            if callable(ctx):
+                ctx = ctx()
+            if value := self._sync_stack.enter_context(ctx):
                 if field is not None:
                     self._params[field] = value
 
         for ctx, field in self._async_sub_contexts:
-            if value := await self._async_stack.enter_async_context(ctx()):
+            if callable(ctx):
+                ctx = ctx()
+            if value := await self._async_stack.enter_async_context(ctx):
                 if field is not None:
                     self._params[field] = value
 
         for name, value in self._field_factories.items():
             if callable(value):
                 value = await invoke_async(value)
             self._params[name] = value
@@ -346,15 +361,15 @@
         self._fields = {}
         self._finalizers = []
         self._contexts = []
 
     def add_param(self, name: str, value: FieldFactory[T]):
         self._fields[name] = value
 
-    def add_context(self, context: Callable[[], AbstractContextManager[T]]):
+    def add_context(self, context: ContextManagerLike[T]):
         self._contexts.append(context)
 
     def add_finalizer(self, finalizer: Callable[[], Awaitable[None] | None]):
         self._finalizers.append(finalizer)
 
     def build(self) -> SyncContext[T]:
         return SyncContext[T](
@@ -369,15 +384,15 @@
         self._fields = {}
         self._finalizers = []
         self._contexts = []
 
     def add_param(self, name: str, value: FieldFactory[T]):
         self._fields[name] = value
 
-    def add_context(self, context: Callable[[], AbstractContextManager[T] | AbstractAsyncContextManager[T]]):
+    def add_context(self, context: ContextManagerLike[T]):
         self._contexts.append(context)
 
     def add_finalizer(self, finalizer: Callable[[], Awaitable[None] | None]):
         self._finalizers.append(finalizer)
 
     def build(self) -> AsyncContext[T]:
         return AsyncContext[T](
```

### Comparing `greyhorse-0.4.3/greyhorse/app/entities/application.py` & `greyhorse-0.4.4/greyhorse/app/entities/application.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/app/entities/controller.py` & `greyhorse-0.4.4/greyhorse/app/entities/controller.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/app/entities/deps.py` & `greyhorse-0.4.4/greyhorse/app/entities/deps.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/app/entities/module.py` & `greyhorse-0.4.4/greyhorse/app/entities/module.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/app/entities/providers.py` & `greyhorse-0.4.4/greyhorse/app/entities/providers.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/app/entities/service.py` & `greyhorse-0.4.4/greyhorse/app/entities/service.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/app/errors.py` & `greyhorse-0.4.4/greyhorse/app/errors.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/app/schemas/components.py` & `greyhorse-0.4.4/greyhorse/app/schemas/components.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/app/schemas/controller.py` & `greyhorse-0.4.4/greyhorse/app/schemas/controller.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/app/schemas/module.py` & `greyhorse-0.4.4/greyhorse/app/schemas/module.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/app/schemas/service.py` & `greyhorse-0.4.4/greyhorse/app/schemas/service.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/app/tasks/app.py` & `greyhorse-0.4.4/greyhorse/app/tasks/app.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/app/utils/registry.py` & `greyhorse-0.4.4/greyhorse/app/utils/registry.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/data/cache/base.py` & `greyhorse-0.4.4/greyhorse/data/cache/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/data/cache/method.py` & `greyhorse-0.4.4/greyhorse/data/cache/method.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/data/models/base.py` & `greyhorse-0.4.4/greyhorse/data/models/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/data/models/fields.py` & `greyhorse-0.4.4/greyhorse/data/models/fields.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/data/models/filterable.py` & `greyhorse-0.4.4/greyhorse/data/models/filterable.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/data/models/model.py` & `greyhorse-0.4.4/greyhorse/data/models/model.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/data/models/serializable.py` & `greyhorse-0.4.4/greyhorse/data/models/serializable.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/data/repositories/base.py` & `greyhorse-0.4.4/greyhorse/data/repositories/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/data/repositories/filterable.py` & `greyhorse-0.4.4/greyhorse/data/repositories/filterable.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/data/serializers/base.py` & `greyhorse-0.4.4/greyhorse/data/serializers/base.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/data/serializers/pickle.py` & `greyhorse-0.4.4/greyhorse/data/serializers/pickle.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/data/storage.py` & `greyhorse-0.4.4/greyhorse/data/storage.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/i18n/translator.py` & `greyhorse-0.4.4/greyhorse/i18n/translator.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/logging.py` & `greyhorse-0.4.4/greyhorse/logging.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/messagebus.py` & `greyhorse-0.4.4/greyhorse/messagebus.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/result.py` & `greyhorse-0.4.4/greyhorse/result.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/translations.toml` & `greyhorse-0.4.4/greyhorse/translations.toml`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/utils/dicts.py` & `greyhorse-0.4.4/greyhorse/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/utils/hashes.py` & `greyhorse-0.4.4/greyhorse/utils/hashes.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/utils/imports.py` & `greyhorse-0.4.4/greyhorse/utils/imports.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/utils/injectors.py` & `greyhorse-0.4.4/greyhorse/utils/injectors.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/utils/strings.py` & `greyhorse-0.4.4/greyhorse/utils/strings.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/greyhorse/utils/time.py` & `greyhorse-0.4.4/greyhorse/utils/time.py`

 * *Files identical despite different names*

### Comparing `greyhorse-0.4.3/pyproject.toml` & `greyhorse-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "greyhorse"
-version = "0.4.3"
+version = "0.4.4"
 description = "Greyhorse library"
 license = "MIT"
 repository = "https://gitlab.com/max-plutonium/greyhorse"
 authors = ["Max Plutonium <plutonium.max@gmail.com>"]
 maintainers = ["Max Plutonium <plutonium.max@gmail.com>"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `greyhorse-0.4.3/PKG-INFO` & `greyhorse-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greyhorse
-Version: 0.4.3
+Version: 0.4.4
 Summary: Greyhorse library
 Home-page: https://gitlab.com/max-plutonium/greyhorse
 License: MIT
 Author: Max Plutonium
 Author-email: plutonium.max@gmail.com
 Maintainer: Max Plutonium
 Maintainer-email: plutonium.max@gmail.com
```

