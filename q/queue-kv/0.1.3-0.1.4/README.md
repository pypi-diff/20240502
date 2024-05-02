# Comparing `tmp/queue_kv-0.1.3.tar.gz` & `tmp/queue_kv-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "queue_kv-0.1.3.tar", last modified: Sun Apr 28 09:02:23 2024, max compression
+gzip compressed data, was "queue_kv-0.1.4.tar", last modified: Thu May  2 10:17:08 2024, max compression
```

## Comparing `queue_kv-0.1.3.tar` & `queue_kv-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-28 09:02:23.564165 queue_kv-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      596 2024-04-28 09:02:23.564165 queue_kv-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       69 2024-04-24 13:02:36.000000 queue_kv-0.1.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      642 2024-04-28 09:02:21.000000 queue_kv-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-28 09:02:23.564165 queue_kv-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-28 09:02:23.564165 queue_kv-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-28 09:02:23.564165 queue_kv-0.1.3/src/q/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-28 09:02:23.564165 queue_kv-0.1.3/src/q/kv/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      174 2024-04-24 13:02:36.000000 queue_kv-0.1.3/src/q/kv/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       98 2024-04-24 13:02:36.000000 queue_kv-0.1.3/src/q/kv/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2242 2024-04-28 09:02:10.000000 queue_kv-0.1.3/src/q/kv/api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      877 2024-04-25 07:26:10.000000 queue_kv-0.1.3/src/q/kv/append.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-28 09:02:23.564165 queue_kv-0.1.3/src/queue_kv.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      596 2024-04-28 09:02:23.000000 queue_kv-0.1.3/src/queue_kv.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      281 2024-04-28 09:02:23.000000 queue_kv-0.1.3/src/queue_kv.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-28 09:02:23.000000 queue_kv-0.1.3/src/queue_kv.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-04-28 09:02:23.000000 queue_kv-0.1.3/src/queue_kv.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-04-28 09:02:23.000000 queue_kv-0.1.3/src/queue_kv.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 10:17:08.949095 queue_kv-0.1.4/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      988 2024-05-02 10:17:08.949095 queue_kv-0.1.4/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      458 2024-05-02 10:15:17.000000 queue_kv-0.1.4/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      645 2024-05-02 10:17:06.000000 queue_kv-0.1.4/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-02 10:17:08.949095 queue_kv-0.1.4/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 10:17:08.939095 queue_kv-0.1.4/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 10:17:08.939095 queue_kv-0.1.4/src/q/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 10:17:08.949095 queue_kv-0.1.4/src/q/kv/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      174 2024-05-01 09:09:25.000000 queue_kv-0.1.4/src/q/kv/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       98 2024-05-01 09:09:25.000000 queue_kv-0.1.4/src/q/kv/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2577 2024-05-02 10:05:20.000000 queue_kv-0.1.4/src/q/kv/api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      961 2024-05-02 10:10:53.000000 queue_kv-0.1.4/src/q/kv/append.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 10:17:08.949095 queue_kv-0.1.4/src/queue_kv.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      988 2024-05-02 10:17:08.000000 queue_kv-0.1.4/src/queue_kv.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      281 2024-05-02 10:17:08.000000 queue_kv-0.1.4/src/queue_kv.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-02 10:17:08.000000 queue_kv-0.1.4/src/queue_kv.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       75 2024-05-02 10:17:08.000000 queue_kv-0.1.4/src/queue_kv.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-05-02 10:17:08.000000 queue_kv-0.1.4/src/queue_kv.egg-info/top_level.txt
```

### Comparing `queue_kv-0.1.3/pyproject.toml` & `queue_kv-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "queue-kv"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Async Queue API implementation based on a Key-Value api"
 dependencies = [
   "queue-api", "kv-api", "pydantic", "lazy-loader"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
-repo = "https://github.com/moveread/python-storage.git"
+repo = "https://github.com/marciclabas/python-storage.git"
 
 [project.optional-dependencies]
 fs = ["kv-fs"]
 sqlite = ["kv-sqlite-sync"]
 
 # test = [
 #   "pytest < 5.0.0",
```

### Comparing `queue_kv-0.1.3/src/q/kv/api.py` & `queue_kv-0.1.4/src/q/kv/api.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing_extensions import Generic, Literal, TypeVar, overload
+from typing_extensions import AsyncIterable, Generic, Literal, TypeVar, overload
 import asyncio
 from datetime import timedelta
-from haskellian import either as E, AsyncIter, iter as I
-from kv.api import KV
-from q.api import Queue
+from haskellian import either as E, AsyncIter, iter as I, Either, Left, IsLeft, Right
+from kv.api import KV, InexistentItem as KVInexistentItem
+from q.api import Queue, QueueError, ReadError, InexistentItem
 
 A = TypeVar('A')
 B = TypeVar('B')
 
 class QueueKV(Queue[A], Generic[A]):
 
   def __init__(
@@ -44,28 +44,33 @@
   
   @classmethod
   def at(cls, Type: type[B], path: str, protocol: Literal['fs', 'sqlite'], table: str = 'queue') -> 'QueueKV[B]':
     return QueueKV.fs(Type, path) if protocol == 'fs' else QueueKV.sqlite(Type, path, table)
 
 
   async def push(self, key: str, value: A):
-    return (await self._kv.insert(key, value)).unsafe()
+    return (await self._kv.insert(key, value)).mapl(QueueError)
   
-  async def _read(self, id: str | None = None, remove: bool = False) -> None | tuple[str, A]:
+  async def _read(self, id: str | None = None, remove: bool = False) -> Either[ReadError, tuple[str, A]]:
     if id is None:
       key = I.head((await self._kv.keys()).unsafe())
       if key is None:
         await asyncio.sleep(self.poll_interval.total_seconds())
         return await self._read(id, remove)
     else:
       key = id
-
-    value = (await self._kv.read(key)).get_or(None)
-    if value is None:
-      return None
-    if remove:
-      (await self._kv.delete(key)).unsafe()
-    return key, value
     
-  def _items(self) -> AsyncIter[tuple[str, A]]:
-    return self._kv.items().map(E.unsafe)
+    try:
+      value = (await self._kv.read(key)).unsafe()
+      if remove:
+        (await self._kv.delete(key)).unsafe()
+      return Right((key, value))
+    except IsLeft as e:
+      match e.value:
+        case KVInexistentItem():
+          return Left(InexistentItem(key))
+        case err:
+          return Left(err)
+    
+  def _items(self) -> AsyncIterable[Either[QueueError, tuple[str, A]]]:
+    return self._kv.items().map(lambda e: e.mapl(QueueError))
```

### Comparing `queue_kv-0.1.3/src/q/kv/append.py` & `queue_kv-0.1.4/src/q/kv/append.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,27 @@
-from typing_extensions import Generic, TypeVar
-import haskellian.either as E
-from kv.api import AppendableKV, InexistentItem
-from q.api import AppendableQueue
+from typing_extensions import Generic, TypeVar, Sequence
+from haskellian import Either, Left
+from kv.api import AppendableKV, InexistentItem as KVInexistentItem
+import kv.fs
+from q.api import AppendableQueue, InexistentItem, ReadError, QueueError
 from .api import QueueKV
 
 A = TypeVar('A')
 T = TypeVar('T')
 
-class AppendQueueKV(QueueKV[list[T]], AppendableQueue[T], Generic[T]):
+class AppendQueueKV(QueueKV[Sequence[T]], AppendableQueue[T], Generic[T]):
 
   def __init__(self, kv: AppendableKV[T]):
     super().__init__(kv)
     self._kv = kv
   
   @classmethod
-  def fs(cls, Type: type[A], path: str) -> 'AppendQueueKV[A]':
-    from kv.fs.append import FilesystemAppendKV
-    return AppendQueueKV[A](FilesystemAppendKV.validated(Type, path))
+  def fs(cls, Type: type[A], path: str) -> 'AppendQueueKV[A]': # type: ignore
+    return AppendQueueKV[A](kv.fs.FilesystemAppendKV.validated(Type, path))
 
-  async def append(self, id: str, values: list[T], *, create: bool = True) -> None | bool:
+  async def append(self, id: str, values: Sequence[T], *, create: bool = False) -> Either[ReadError, None]: # type: ignore
     match await self._kv.append(id, values, create=create):
-      case E.Left(InexistentItem()):
-        return False
+      case Left(KVInexistentItem()):
+        return Left(InexistentItem())
       case either:
-        either.unsafe()
-        if not create:
-          return True
+        return either.mapl(QueueError)
```

