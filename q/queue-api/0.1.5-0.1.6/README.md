# Comparing `tmp/queue_api-0.1.5.tar.gz` & `tmp/queue_api-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "queue_api-0.1.5.tar", last modified: Fri Apr 26 06:54:30 2024, max compression
+gzip compressed data, was "queue_api-0.1.6.tar", last modified: Thu May  2 10:16:51 2024, max compression
```

## Comparing `queue_api-0.1.5.tar` & `queue_api-0.1.6.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 06:54:30.884412 queue_api-0.1.5/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      406 2024-04-26 06:54:30.884412 queue_api-0.1.5/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       60 2024-04-24 13:02:36.000000 queue_api-0.1.5/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      570 2024-04-26 06:54:28.000000 queue_api-0.1.5/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-26 06:54:30.884412 queue_api-0.1.5/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 06:54:30.874412 queue_api-0.1.5/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 06:54:30.874412 queue_api-0.1.5/src/q/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 06:54:30.874412 queue_api-0.1.5/src/q/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      149 2024-04-24 13:02:36.000000 queue_api-0.1.5/src/q/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      228 2024-04-24 13:02:36.000000 queue_api-0.1.5/src/q/api/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 06:54:30.874412 queue_api-0.1.5/src/q/api/api/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      131 2024-04-24 13:02:36.000000 queue_api-0.1.5/src/q/api/api/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      660 2024-04-25 07:26:10.000000 queue_api-0.1.5/src/q/api/api/append.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      183 2024-04-25 07:26:10.000000 queue_api-0.1.5/src/q/api/api/queue.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     5933 2024-04-25 07:26:10.000000 queue_api-0.1.5/src/q/api/api/read.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3323 2024-04-26 06:53:43.000000 queue_api-0.1.5/src/q/api/api/write.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 06:54:30.874412 queue_api-0.1.5/src/q/api/impl/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       61 2024-04-24 13:02:36.000000 queue_api-0.1.5/src/q/api/impl/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      396 2024-04-25 07:26:10.000000 queue_api-0.1.5/src/q/api/impl/empty.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1191 2024-04-25 07:26:10.000000 queue_api-0.1.5/src/q/api/impl/simple.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 06:54:30.884412 queue_api-0.1.5/src/q/api/ops/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-04-24 13:02:36.000000 queue_api-0.1.5/src/q/api/ops/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      317 2024-04-26 06:37:15.000000 queue_api-0.1.5/src/q/api/ops/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1124 2024-04-25 07:26:10.000000 queue_api-0.1.5/src/q/api/ops/append_bounding.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1116 2024-04-25 07:26:10.000000 queue_api-0.1.5/src/q/api/ops/bounding.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1490 2024-04-25 07:26:10.000000 queue_api-0.1.5/src/q/api/ops/interleaving.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1746 2024-04-25 07:26:10.000000 queue_api-0.1.5/src/q/api/ops/merging.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1989 2024-04-25 07:26:10.000000 queue_api-0.1.5/src/q/api/ops/splitting.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      589 2024-04-26 06:52:51.000000 queue_api-0.1.5/src/q/api/ops/teeing.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-26 06:54:30.884412 queue_api-0.1.5/src/queue_api.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      406 2024-04-26 06:54:30.000000 queue_api-0.1.5/src/queue_api.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      665 2024-04-26 06:54:30.000000 queue_api-0.1.5/src/queue_api.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-26 06:54:30.000000 queue_api-0.1.5/src/queue_api.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       23 2024-04-26 06:54:30.000000 queue_api-0.1.5/src/queue_api.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-04-26 06:54:30.000000 queue_api-0.1.5/src/queue_api.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 10:16:51.889095 queue_api-0.1.6/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3482 2024-05-02 10:16:51.889095 queue_api-0.1.6/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3133 2024-05-02 10:16:29.000000 queue_api-0.1.6/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      573 2024-05-02 10:16:34.000000 queue_api-0.1.6/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-02 10:16:51.889095 queue_api-0.1.6/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 10:16:51.889095 queue_api-0.1.6/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 10:16:51.879095 queue_api-0.1.6/src/q/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 10:16:51.889095 queue_api-0.1.6/src/q/api/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      149 2024-05-01 09:09:25.000000 queue_api-0.1.6/src/q/api/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      394 2024-05-02 09:23:56.000000 queue_api-0.1.6/src/q/api/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      810 2024-05-02 10:09:41.000000 queue_api-0.1.6/src/q/api/append.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      512 2024-05-02 08:59:24.000000 queue_api-0.1.6/src/q/api/errors.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 10:16:51.889095 queue_api-0.1.6/src/q/api/impl/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       61 2024-05-01 09:09:25.000000 queue_api-0.1.6/src/q/api/impl/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      752 2024-05-02 09:26:31.000000 queue_api-0.1.6/src/q/api/impl/empty.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1398 2024-05-02 09:28:31.000000 queue_api-0.1.6/src/q/api/impl/simple.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 10:16:51.889095 queue_api-0.1.6/src/q/api/ops/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-01 09:09:25.000000 queue_api-0.1.6/src/q/api/ops/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      299 2024-05-02 09:59:41.000000 queue_api-0.1.6/src/q/api/ops/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1176 2024-05-02 09:58:36.000000 queue_api-0.1.6/src/q/api/ops/append_bounding.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1182 2024-05-02 09:58:34.000000 queue_api-0.1.6/src/q/api/ops/bounding.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1570 2024-05-02 09:58:30.000000 queue_api-0.1.6/src/q/api/ops/interleaving.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1826 2024-05-02 09:58:23.000000 queue_api-0.1.6/src/q/api/ops/merging.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2384 2024-05-02 09:59:31.000000 queue_api-0.1.6/src/q/api/ops/splitting.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      850 2024-05-02 09:53:30.000000 queue_api-0.1.6/src/q/api/ops/teeing.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      183 2024-05-02 09:18:29.000000 queue_api-0.1.6/src/q/api/queue.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     6816 2024-05-02 09:21:42.000000 queue_api-0.1.6/src/q/api/read.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3468 2024-05-02 09:21:08.000000 queue_api-0.1.6/src/q/api/write.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-02 10:16:51.889095 queue_api-0.1.6/src/queue_api.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3482 2024-05-02 10:16:51.000000 queue_api-0.1.6/src/queue_api.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      643 2024-05-02 10:16:51.000000 queue_api-0.1.6/src/queue_api.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-02 10:16:51.000000 queue_api-0.1.6/src/queue_api.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       23 2024-05-02 10:16:51.000000 queue_api-0.1.6/src/queue_api.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        2 2024-05-02 10:16:51.000000 queue_api-0.1.6/src/queue_api.egg-info/top_level.txt
```

### Comparing `queue_api-0.1.5/pyproject.toml` & `queue_api-0.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "queue-api"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "API for an asynchronous, point-readable queue"
 dependencies = [
   "haskellian", "lazy-loader"
 ]
 requires-python = ">=3.10"
 readme = {file="README.md", content-type="text/markdown"}
 
 [project.urls]
-repo = "https://github.com/moveread/python-storage.git"
+repo = "https://github.com/marciclabas/python-storage.git"
 
 # [project.optional-dependencies]
 # test = [
 #   "pytest < 5.0.0",
 #   "pytest-cov[all]"
 # ]
```

### Comparing `queue_api-0.1.5/src/q/api/api/append.py` & `queue_api-0.1.6/src/q/api/append.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from typing_extensions import Generic, TypeVar, overload, Literal
+from typing_extensions import Generic, TypeVar, overload, Literal, Sequence
 from abc import abstractmethod
-from . import WriteQueue, Queue
+from haskellian import Either
+from . import WriteQueue, Queue, QueueError, ReadError
 
-T = TypeVar('T')
+A = TypeVar('A')
 
-class AppendQueue(WriteQueue[list[T]], Generic[T]):
+class AppendQueue(WriteQueue[Sequence[A]], Generic[A]):
   @overload
   @abstractmethod
-  async def append(self, id: str, values: list[T], *, create: Literal[False]) -> bool:
-    """Appends `values` if it already existed. Otherwise doesn't append, and returns `False`"""
+  async def append(self, id: str, values: Sequence[A], *, create: Literal[False]) -> Either[ReadError, None]:
+    """Appends `values` if it already existed. Otherwise doesn't append, and returns `Left[InexistentItem]`"""
   @overload
   @abstractmethod
-  async def append(self, id: str, values: list[T], *, create: bool = True):
+  async def append(self, id: str, values: Sequence[A], *, create: Literal[True] = True) -> Either[QueueError, None]:
     """Appends `values` to `id`, creating the item if needed"""
     
-class AppendableQueue(AppendQueue[T], Queue[list[T]], Generic[T]):
+class AppendableQueue(AppendQueue[A], Queue[Sequence[A]], Generic[A]):
   ...
```

### Comparing `queue_api-0.1.5/src/q/api/api/read.py` & `queue_api-0.1.6/src/q/api/read.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,167 +1,187 @@
-from typing_extensions import Generic, Never, TypeVar, Callable, Awaitable, overload, AsyncIterable, AsyncIterator, TypeGuard
-from haskellian import AsyncIter, promise as P
+from typing_extensions import Generic, Never, TypeVar, Callable, Awaitable, overload, AsyncIterable, AsyncIterator, TypeGuard, Sequence
 from abc import ABC, abstractmethod
+from haskellian import AsyncIter, promise as P, Either, Left, Right, iter as I
+from .errors import QueueError, ReadError, InexistentItem
 
 A = TypeVar('A', covariant=True)
 B = TypeVar('B', covariant=True)
+E = TypeVar('E', covariant=True)
 
-class ReadQueue(ABC, AsyncIterator[tuple[str, A]], Generic[A]):
+class ReadQueue(ABC, AsyncIterator[Either[QueueError, tuple[str, A]]], Generic[A]):
   
   @abstractmethod
-  async def _read(self, id: str | None, remove: bool) -> None | tuple[str, A]:
+  async def _read(self, id: str | None, remove: bool) -> Either[ReadError, tuple[str, A]]:
     ...
 
   @overload
-  async def pop(self) -> tuple[str, A]:
+  async def pop(self) -> Either[QueueError, tuple[str, A]]:
     ...
   @overload
-  async def pop(self, id: str) -> None | A:
+  async def pop(self, id: str) -> Either[ReadError, A]:
     ...
 
-  async def pop(self, id: str | None = None) -> None | A | tuple[str, A]:
+  async def pop(self, id: str | None = None) -> Either[ReadError, A | tuple[str, A]]:
     match await self._read(id, remove=True):
-      case k, v:
-        return (k, v) if id is None else v
+      case Right((k, v)):
+        return Right((k, v) if id is None else v)
+      case err:
+        return err
   
   @overload
-  async def read(self) -> tuple[str, A]:
+  async def read(self) -> Either[QueueError, tuple[str, A]]:
     ...
   @overload
-  async def read(self, id: str) -> None | A:
+  async def read(self, id: str) -> Either[ReadError, A]:
     ...
   
-  async def read(self, id: str | None = None) -> None | A | tuple[str, A]:
+  async def read(self, id: str | None = None) -> Either[ReadError, A | tuple[str, A]]:
     match await self._read(id, remove=False):
-      case k, v:
-        return (k, v) if id is None else v
+      case Right((k, v)):
+        return Right((k, v) if id is None else v)
+      case err:
+        return err
       
   @abstractmethod
-  def _items(self) -> AsyncIterable[tuple[str, A]]:
+  def _items(self) -> AsyncIterable[Either[QueueError, tuple[str, A]]]:
     ...
 
-  def items(self) -> AsyncIter[tuple[str, A]]:
+  def items(self) -> AsyncIter[Either[QueueError, tuple[str, A]]]:
     return AsyncIter(self._items())
   
-  def keys(self) -> AsyncIter[str]:
-    return AsyncIter(k async for k, _ in self._items())
+  def keys(self) -> AsyncIter[Either[ReadError, str]]:
+    return AsyncIter(e | I.fst async for e in self._items())
   
-  def values(self) -> AsyncIter[A]:
-    return AsyncIter(v async for _, v in self._items())
+  def values(self) -> AsyncIter[Either[ReadError, A]]:
+    return AsyncIter(e | I.snd async for e in self._items())
   
-  async def __anext__(self) -> tuple[str, A]:
+  async def __anext__(self) -> Either[QueueError, tuple[str, A]]:
     return await self.pop()
   
   def iter(self):
     async def iterate():
       while (x := await self.pop()):
         yield x
     return AsyncIter(iterate())
   
   __aiter__ = iter
   
   def map(self, f: Callable[[A], B]) -> 'ReadQueue[B]':
     """Maps `f` over self. Returns a new queue, but `self` is still mutated when popping from the new queue"""
-    return MappedQueue(self, lambda kv: P.of((kv[0], f(kv[1]))))
+    return qmap(self, lambda kv: P.of((kv[0], f(kv[1]))))
   
   def map_kv(self, f: Callable[[str, A], B]) -> 'ReadQueue[B]':
     """Map but `f` receives both key and value"""
-    return MappedQueue(self, lambda kv: P.of((kv[0], f(*kv))))
+    return qmap(self, lambda kv: P.of((kv[0], f(*kv))))
   
   def map_k(self, f: Callable[[str], B]) -> 'ReadQueue[B]':
     """Map but `f` receives the key"""
-    return MappedQueue(self, lambda kv: P.of((kv[0], f(kv[0]))))
+    return qmap(self, lambda kv: P.of((kv[0], f(kv[0]))))
   
   def map_kvt(self, f: Callable[[tuple[str, A]], B]) -> 'ReadQueue[B]':
     """Map but `f` receives both key and value as a tuple"""
-    return MappedQueue(self, lambda kv: P.of((kv[0], f(kv))))
+    return qmap(self, lambda kv: P.of((kv[0], f(kv))))
   
   def amap(self, f: Callable[[A], Awaitable[B]]) -> 'ReadQueue[B]':
     """Map but `f` is asynchronous"""
     async def mapper(kv: tuple[str, A]):
       return kv[0], await f(kv[1])
-    return MappedQueue(self, mapper)
+    return qmap(self, mapper)
   
   def amap_kv(self, f: Callable[[str, A], Awaitable[B]]) -> 'ReadQueue[B]':
     """Map but `f` is asynchronous and receives both key and value"""
     async def mapper(kv: tuple[str, A]):
       return kv[0], await f(*kv)
-    return MappedQueue(self, mapper)
+    return qmap(self, mapper)
   
   def amap_k(self, f: Callable[[str], Awaitable[B]]) -> 'ReadQueue[B]':
     """Map but `f` is asynchronous and receives the key"""
     async def mapper(kv: tuple[str, A]):
       return kv[0], await f(kv[0])
-    return MappedQueue(self, mapper)
+    return qmap(self, mapper)
   
   def amap_kvt(self, f: Callable[[tuple[str, A]], Awaitable[B]]) -> 'ReadQueue[B]':
     """Map but `f` is asynchronous and receives both key and value as a tuple"""
     async def mapper(kv: tuple[str, A]):
       return kv[0], await f(kv)
-    return MappedQueue(self, mapper)
+    return qmap(self, mapper)
 
   @overload
   def filter(self, pred: Callable[[A], TypeGuard[B]]) -> 'ReadQueue[B]': ...
   @overload
   def filter(self, pred: Callable[[A], bool]) -> 'ReadQueue[A]': ...
   def filter(self, pred): # type: ignore
-    return FilteredQueue(self, lambda _, v: pred(v))
+    return qfilter(self, lambda _, v: pred(v))
   
   @overload
   def filter_kv(self, pred: Callable[[str, A], TypeGuard[B]]) -> 'ReadQueue[B]': ...
   @overload
   def filter_kv(self, pred: Callable[[str, A], bool]) -> 'ReadQueue[A]': ...
   def filter_kv(self, pred): # type: ignore
-    return FilteredQueue(self, pred)
+    return qfilter(self, pred)
   
   def partition(self, pred: Callable[[A], bool]) -> 'tuple[ReadQueue[A], ReadQueue[A]]':
     """Returns `self.filter(pred), self.filter(!pred)`"""
     return self.filter(pred), self.filter(lambda x: not pred(x))
   
   def partition_kv(self, pred: Callable[[str, A], bool]) -> 'tuple[ReadQueue[A], ReadQueue[A]]':
     """Returns `self.filter_kv(pred), self.filter_kv(!pred)`"""
     return self.filter_kv(pred), self.filter_kv(lambda *x: not pred(*x))
   
   
-class MappedQueue(ReadQueue[B], Generic[A, B]):
+class qmap(ReadQueue[B], Generic[A, B]):
   
   def __init__(self, q: ReadQueue[A], f: Callable[[tuple[str, A]], Awaitable[tuple[str, B]]]):
     self._wrapped = q
     self._mapper = f
     __name__ = f'Mapped{repr(self)}'
 
-  def _items(self) -> AsyncIterable[tuple[str, B]]:
-    return (await self._mapper(x) async for x in self._wrapped._items())
-  
-  async def _read(self, id: str | None = None, remove: bool = False) -> tuple[str, B] | None:
+  async def _items(self) -> AsyncIterable[Either[QueueError, tuple[str, B]]]:
+    async for e in self._wrapped._items():
+      if e.tag == 'left':
+        yield e # type: ignore
+      else:
+        yield Right(await self._mapper(e.value))
+
+  async def _read(self, id: str | None, remove: bool) -> Either[ReadError, tuple[str, B]]:
     match await self._wrapped._read(id, remove):
-      case k, v:
-        return await self._mapper((k, v))
+      case Right((k, v)):
+        return Right(await self._mapper((k, v)))
+      case err:
+        return err # type: ignore
       
-class FilteredQueue(ReadQueue[A], Generic[A]):
+class qfilter(ReadQueue[A], Generic[A]):
 
   def __init__(self, queue: ReadQueue[A], pred: Callable[[str, A], bool]):
     self._pred = pred
     self._queue = queue
 
-  async def _point_read(self, id: str, remove: bool) -> None | tuple[str, A]:
-    item = await self._queue.read(id)
-    if item is None or not self._pred(id, item):
-      return None
+  async def _point_read(self, id: str, remove: bool) -> Either[ReadError, tuple[str, A]]:
+    e = await self._queue.read(id)
+    if e.tag == 'left':
+      return e # type: ignore
+    item = e.value
+    if not self._pred(id, item):
+      return Left(InexistentItem(id, detail=f'"{id}" exists but has been filtered out by {self._pred}'))
     if remove:
       await self._queue.pop(id)
-    return id, item
+    return Right((id, item))
 
-  async def _read_any(self, remove: bool) -> tuple[str, A]:
-    async for id, item in self._items():
+  async def _read_any(self, remove: bool) -> Either[QueueError, tuple[str, A]]:
+    async for e in self._items():
+      if e.tag == 'left':
+        return e
+      id, item = e.value
       if remove:
         await self._queue.pop(id)
-      return id, item
+      return Right((id, item))
     return Never
 
-  async def _read(self, id: str | None, remove: bool) -> None | tuple[str, A]:
+  async def _read(self, id: str | None, remove: bool) -> Either[ReadError, tuple[str, A]]:
     return await (self._read_any(remove) if id is None else self._point_read(id, remove))
   
-  async def _items(self) -> AsyncIterable[tuple[str, A]]:
-    async for item in self._queue._items():
-      if self._pred(*item):
-        yield item
+  async def _items(self) -> AsyncIterable[Either[QueueError, tuple[str, A]]]:
+    async for e in self._queue._items():
+      if e.tag == 'left':
+        yield e
+      elif self._pred(*e.value):
+        yield e
```

### Comparing `queue_api-0.1.5/src/q/api/api/write.py` & `queue_api-0.1.6/src/q/api/write.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from typing_extensions import Generic, TypeVar, Callable, Awaitable, AsyncIterable, TypeGuard, overload
-from haskellian import promise as P
+from haskellian import promise as P, Either, Right
 from abc import ABC, abstractmethod
+from .errors import QueueError
 
 A = TypeVar('A', contravariant=True)
 B = TypeVar('B', contravariant=True)
 
 class WriteQueue(ABC, Generic[A]):
 
   async def iterate(self, items: AsyncIterable[tuple[str, A]]):
     """Push all `items`"""
     async for key, value in items:
       await self.push(key, value)
 
   @abstractmethod
-  async def push(self, key: str, value: A):
+  async def push(self, key: str, value: A) -> Either[QueueError, None]:
     ...
 
-  def pusher(self, key: str) -> Callable[[A], Awaitable[None]]:
+  def pusher(self, key: str) -> Callable[[A], Awaitable[Either[QueueError, None]]]:
     """Partially applied `push`"""
     return lambda value: self.push(key, value)
   
   @overload
   def prefilter(self, pred: Callable[[A], TypeGuard[B]]) -> 'WriteQueue[B]': ...
   @overload
   def prefilter(self, pred: Callable[[A], bool]) -> 'WriteQueue[A]': ...
@@ -69,17 +70,18 @@
 class prefilter(WriteQueue[A], Generic[A]):
   
   def __init__(self, q: WriteQueue[A], p: Callable[[tuple[str, A]], Awaitable[bool]]):
     self._wrapped = q
     self._predicate = p
     __name__ = f'Filtered{repr(self)}'
 
-  async def push(self, key: str, value: A):
+  async def push(self, key: str, value: A) -> Either[QueueError, None]:
     if await self._predicate((key, value)):
       return await self._wrapped.push(key, value)
+    return Right(None)
 
 class premap(WriteQueue[B], Generic[A, B]):
   
   def __init__(self, q: WriteQueue[A], f: Callable[[tuple[str, B]], Awaitable[tuple[str, A]]]):
     self._wrapped = q
     self._mapper = f
     __name__ = f'Mapped{repr(self)}'
```

### Comparing `queue_api-0.1.5/src/q/api/impl/simple.py` & `queue_api-0.1.6/src/q/api/impl/simple.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,44 @@
-from typing_extensions import Generic, TypeVar, AsyncIterable
+from typing_extensions import Generic, TypeVar, AsyncIterable, Never
 from collections import OrderedDict
-from ..api import ReadQueue, WriteQueue
-from haskellian import ManagedPromise
+from .. import ReadQueue, WriteQueue, InexistentItem
+from haskellian import ManagedPromise, Either, Left, Right
 
 A = TypeVar('A')
 B = TypeVar('B')
 
 class SimpleQueue(WriteQueue[A], ReadQueue[A], Generic[A]):
   """Dead simple in-memory implementation backed by an `OrderedDict`"""
 
   def __init__(self):
     self.xs: OrderedDict[str, A] = OrderedDict()
     self._next = ManagedPromise()
 
   def __len__(self):
     return len(self.xs) # type: ignore
 
-  async def _read(self, id: str | None = None, remove: bool = False) -> None | tuple[str, A]:
+  async def _read(self, id: str | None = None, remove: bool = False) -> Either[InexistentItem, tuple[str, A]]:
     if id is None:
       if len(self.xs) == 0:
         await self._next
         self._next = ManagedPromise()
         return await self._read(id, remove)
       elif remove:
-        return self.xs.popitem()
+        return Right(self.xs.popitem())
       else:
-        return next(iter(self.xs.items()))
+        return Right(next(iter(self.xs.items())))
     elif id in self.xs:
       v = self.xs.pop(id) if remove else self.xs[id]
-      return id, v
+      return Right((id, v))
+    else:
+      return Left(InexistentItem(id))
     
-  async def push(self, k: str, v: A):
-    self.xs[k] = v
+  async def push(self, key: str, value: A) -> Right[Never, None]:
+    self.xs[key] = value
     if not self._next.resolved:
       self._next.resolve()
+    return Right(None)
   
-  async def _items(self) -> AsyncIterable[tuple[str, A]]:
+  async def _items(self) -> AsyncIterable[Right[Never, tuple[str, A]]]:
     for x in self.xs.items():
-      yield x
+      yield Right(x)
```

### Comparing `queue_api-0.1.5/src/q/api/ops/append_bounding.py` & `queue_api-0.1.6/src/q/api/ops/append_bounding.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing_extensions import TypeVar, Generic
-import asyncio
-from haskellian import ManagedPromise
-from ..api.append import AppendableQueue
-from .bounding import Bounded
+# from typing_extensions import TypeVar, Generic
+# import asyncio
+# from haskellian import ManagedPromise
+# from ..api.append import AppendableQueue
+# from .bounding import Bounded
 
-T = TypeVar('T')
+# T = TypeVar('T')
 
-class AppendBounded(AppendableQueue[T], Bounded[list[T]], Generic[T]):
-  def __init__(self, queue: AppendableQueue[T], max_items: int):
-    super().__init__(queue, max_items)
-    self._queue = queue
-    self._append_buffer = asyncio.Queue[tuple[str, list[T], bool]]()
+# class AppendBounded(AppendableQueue[T], Bounded[list[T]], Generic[T]):
+#   def __init__(self, queue: AppendableQueue[T], max_items: int):
+#     super().__init__(queue, max_items)
+#     self._queue = queue
+#     self._append_buffer = asyncio.Queue[tuple[str, list[T], bool]]()
 
-  async def _append_advance(self):
-    k, vs, create = await self._append_buffer.get()
-    await self._queue.append(k, vs, create=create)
+#   async def _append_advance(self):
+#     k, vs, create = await self._append_buffer.get()
+#     await self._queue.append(k, vs, create=create)
 
-  async def append(self, id: str, values: list[T], *, create = True):
-    if create:
-      await self._append_buffer.put((id, values, create))
-      while self.num_items >= self.max_items:
-        if self._promise.resolved:
-          self._promise = ManagedPromise()
-      self.num_items += 1
-      await self._append_advance()
-    else:
-      return await self._queue.append(id, values, create=False)
+#   async def append(self, id: str, values: list[T], *, create = True):
+#     if create:
+#       await self._append_buffer.put((id, values, create))
+#       while self.num_items >= self.max_items:
+#         if self._promise.resolved:
+#           self._promise = ManagedPromise()
+#       self.num_items += 1
+#       await self._append_advance()
+#     else:
+#       return await self._queue.append(id, values, create=False)
     
-def abounded(queue: AppendableQueue[T], max_items: int) -> AppendableQueue[T]:
-  return AppendBounded(queue, max_items)
+# def abounded(queue: AppendableQueue[T], max_items: int) -> AppendableQueue[T]:
+#   return AppendBounded(queue, max_items)
```

### Comparing `queue_api-0.1.5/src/q/api/ops/interleaving.py` & `queue_api-0.1.6/src/q/api/ops/interleaving.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from typing_extensions import TypeVar, Generic, AsyncIterable
-import asyncio
-from haskellian import ManagedAsync
-from ..api import ReadQueue
-from ..impl import SimpleQueue
-
-A = TypeVar('A')
-B = TypeVar('B')
-C = TypeVar('C')
-
-class Interleaved(ReadQueue[A], Generic[A]):
-
-  def __init__(self, queues: list[ReadQueue[A]]):
-    self._queues = queues
-    self._buffer: SimpleQueue[A] = SimpleQueue()
-
-  async def _advance(self):
-    for fut in asyncio.as_completed([q.pop() for q in self._queues]):
-      k, v = await fut
-      await self._buffer.push(k, v)
-
-  async def _read(self, id: str | None = None, remove: bool = False) -> tuple[str, A] | A | None:
-    if id is None:
-      if len(self._buffer) == 0:
-        asyncio.create_task(self._advance())
-      return await self._buffer._read(id, remove)
-    else:
-      for q in self._queues:
-        x = await q._read(id, remove)
-        if x is not None:
-          return x
+# from typing_extensions import TypeVar, Generic, AsyncIterable
+# import asyncio
+# from haskellian import ManagedAsync
+# from ..api import ReadQueue
+# from ..impl import SimpleQueue
+
+# A = TypeVar('A')
+# B = TypeVar('B')
+# C = TypeVar('C')
+
+# class Interleaved(ReadQueue[A], Generic[A]):
+
+#   def __init__(self, queues: list[ReadQueue[A]]):
+#     self._queues = queues
+#     self._buffer: SimpleQueue[A] = SimpleQueue()
+
+#   async def _advance(self):
+#     for fut in asyncio.as_completed([q.pop() for q in self._queues]):
+#       k, v = await fut
+#       await self._buffer.push(k, v)
+
+#   async def _read(self, id: str | None = None, remove: bool = False) -> tuple[str, A] | A | None:
+#     if id is None:
+#       if len(self._buffer) == 0:
+#         asyncio.create_task(self._advance())
+#       return await self._buffer._read(id, remove)
+#     else:
+#       for q in self._queues:
+#         x = await q._read(id, remove)
+#         if x is not None:
+#           return x
   
-  def _items(self) -> AsyncIterable[tuple[str, A]]:
-    out = ManagedAsync[tuple[str, A]]()
-    async def iterate(xs: AsyncIterable[tuple[str, A]]):
-      async for x in xs:
-        out.push(x)
-
-    async def iterate_all():
-      async for x in self._buffer.items():
-        out.push(x)
-      await asyncio.gather(*[iterate(q.items()) for q in self._queues])
-      out.end()
-    asyncio.create_task(iterate_all())
-    return out
+#   def _items(self) -> AsyncIterable[tuple[str, A]]:
+#     out = ManagedAsync[tuple[str, A]]()
+#     async def iterate(xs: AsyncIterable[tuple[str, A]]):
+#       async for x in xs:
+#         out.push(x)
+
+#     async def iterate_all():
+#       async for x in self._buffer.items():
+#         out.push(x)
+#       await asyncio.gather(*[iterate(q.items()) for q in self._queues])
+#       out.end()
+#     asyncio.create_task(iterate_all())
+#     return out
   
-def interleave(q1: ReadQueue[A], q2: ReadQueue[B], *qs: ReadQueue[C]) -> ReadQueue[A|B|C]:
-  return Interleaved[A|B|C]([q1, q2, *qs])
+# def interleave(q1: ReadQueue[A], q2: ReadQueue[B], *qs: ReadQueue[C]) -> ReadQueue[A|B|C]:
+#   return Interleaved[A|B|C]([q1, q2, *qs])
```

### Comparing `queue_api-0.1.5/src/q/api/ops/merging.py` & `queue_api-0.1.6/src/q/api/ops/merging.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from typing_extensions import TypeVar, Generic, AsyncIterable, Callable, Awaitable
-import asyncio
-import haskellian.promise as P
-from q.api import ReadQueue
-
-A = TypeVar('A')
-B = TypeVar('B')
-C = TypeVar('C')
-
-
-class Merged(ReadQueue[C], Generic[A, B, C]):
-
-  def __init__(self, merge: Callable[[str, tuple[A, B]], C | Awaitable[C]], queues: tuple[ReadQueue[A], ReadQueue[B]]):
-    self._merge = merge
-    self._q1 = queues[0]
-    self._q2 = queues[1]
-
-  async def _read_one(self, id: str | None = None) -> None | tuple[str, A, B]:
-    if id is not None:
-      x1, x2 = await asyncio.gather(self._q1.read(id), self._q2.read(id))
-      if x1 is not None and x2 is not None:
-        return id, x1, x2
-    else:
-      async for k, x1 in self._q1._items():
-        x2 = await self._q2.read(k)
-        if x2 is not None:
-          return k, x1, x2
-
-  async def _read(self, id: str | None = None, remove: bool = False) -> None | tuple[str, C]:
-    while True:
-      match await self._read_one(id):
-        case k, x1, x2:
-          if remove:
-            await asyncio.gather(self._q1.pop(k), self._q2.pop(k))
-          return k, await P.wait(self._merge(k, (x1, x2)))
-      for fut in asyncio.as_completed((self._q1.read(), self._q2.read())):
-        await fut
-
-  async def _items(self) -> AsyncIterable[tuple[str, C]]:
-    async for k, x1 in self._q1._items():
-      x2 = await self._q2.read(k)
-      if x2 is not None:
-        yield k, await P.wait(self._merge(k, (x1, x2)))
+# from typing_extensions import TypeVar, Generic, AsyncIterable, Callable, Awaitable
+# import asyncio
+# import haskellian.promise as P
+# from q.api import ReadQueue
+
+# A = TypeVar('A')
+# B = TypeVar('B')
+# C = TypeVar('C')
+
+
+# class Merged(ReadQueue[C], Generic[A, B, C]):
+
+#   def __init__(self, merge: Callable[[str, tuple[A, B]], C | Awaitable[C]], queues: tuple[ReadQueue[A], ReadQueue[B]]):
+#     self._merge = merge
+#     self._q1 = queues[0]
+#     self._q2 = queues[1]
+
+#   async def _read_one(self, id: str | None = None) -> None | tuple[str, A, B]:
+#     if id is not None:
+#       x1, x2 = await asyncio.gather(self._q1.read(id), self._q2.read(id))
+#       if x1 is not None and x2 is not None:
+#         return id, x1, x2
+#     else:
+#       async for k, x1 in self._q1._items():
+#         x2 = await self._q2.read(k)
+#         if x2 is not None:
+#           return k, x1, x2
+
+#   async def _read(self, id: str | None = None, remove: bool = False) -> None | tuple[str, C]:
+#     while True:
+#       match await self._read_one(id):
+#         case k, x1, x2:
+#           if remove:
+#             await asyncio.gather(self._q1.pop(k), self._q2.pop(k))
+#           return k, await P.wait(self._merge(k, (x1, x2)))
+#       for fut in asyncio.as_completed((self._q1.read(), self._q2.read())):
+#         await fut
+
+#   async def _items(self) -> AsyncIterable[tuple[str, C]]:
+#     async for k, x1 in self._q1._items():
+#       x2 = await self._q2.read(k)
+#       if x2 is not None:
+#         yield k, await P.wait(self._merge(k, (x1, x2)))
 
-def merge(queues: tuple[ReadQueue[A], ReadQueue[B]], merge: Callable[[str, tuple[A, B]], C | Awaitable[C]]) -> ReadQueue[C]:
-  return Merged(merge, queues)
+# def merge(queues: tuple[ReadQueue[A], ReadQueue[B]], merge: Callable[[str, tuple[A, B]], C | Awaitable[C]]) -> ReadQueue[C]:
+#   return Merged(merge, queues)
 
-def zip(queues: tuple[ReadQueue[A], ReadQueue[B]]) -> ReadQueue[tuple[A, B]]:
-  return merge(queues, lambda k, t: t)
+# def zip(queues: tuple[ReadQueue[A], ReadQueue[B]]) -> ReadQueue[tuple[A, B]]:
+#   return merge(queues, lambda k, t: t)
```

### Comparing `queue_api-0.1.5/src/q/api/ops/splitting.py` & `queue_api-0.1.6/src/q/api/ops/splitting.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,63 @@
-from typing_extensions import TypeVar, Generic, AsyncIterable, Callable, Awaitable
-import haskellian.promise as P
-from ..api import ReadQueue, WriteQueue
-from ..impl import SimpleQueue
-from .interleaving import interleave
-
-A = TypeVar('A')
-B = TypeVar('B')
-C = TypeVar('C')
-
-class Split(ReadQueue[A], Generic[A]):
-
-  def __init__(self, split: Callable[[C], tuple[A, B] | Awaitable[tuple[A, B]]], queue: ReadQueue[C], other: WriteQueue[B]):
-    self._split = split
-    self._queue = queue
-    self._other = other
-
-  async def _read(self, id: str | None, remove: bool = False) -> None | tuple[str, A]:
-    match await self._queue._read(id, remove):
-      case id, v:
-        a, b = await P.wait(self._split(v))
-        await self._other.push(id, b)
-        return id, a
+# from typing_extensions import TypeVar, Generic, AsyncIterable, Callable, Awaitable
+# from haskellian import promise as P, Either, Left, Right
+# from .. import ReadQueue, WriteQueue, QueueError, InexistentItem
+# from ..impl import SimpleQueue
+# from .interleaving import interleave
+
+# A = TypeVar('A', covariant=True)
+# B = TypeVar('B')
+# C = TypeVar('C')
+
+# class Split(ReadQueue[A], Generic[A]):
+
+#   def __init__(self, split: Callable[[C], tuple[A, B] | Awaitable[tuple[A, B]]], queue: ReadQueue[C], other: WriteQueue[B]):
+#     self._split = split
+#     self._queue = queue
+#     self._other = other
+
+#   async def _read(self, id: str | None, remove: bool) -> Either[QueueError | InexistentItem, tuple[str, A]]:
+#     match await self._queue._read(id, remove):
+#       case Right((id, v)):
+#         a, b = await P.wait(self._split(v))
+#         await self._other.push(id, b)
+#         return Right((id, a))
+#       case err:
+#         return err # type: ignore
   
-  async def _items(self) -> AsyncIterable[tuple[str, A]]:
-    async for id, v in self._queue._items():
-      a, _ = await P.wait(self._split(v))
-      yield id, a
-
-def swap(pair: tuple[A, B]) -> tuple[B, A]:
-  a, b = pair
-  return b, a
-
-def split(
-  queue: ReadQueue[A],
-  split: Callable[[A], tuple[B, C] | Awaitable[tuple[B, C]]]
-) -> tuple[ReadQueue[B], ReadQueue[C]]:
-  buf1 = SimpleQueue[B]()
-  buf2 = SimpleQueue[C]()
-  q1 = interleave(buf1, Split(split, queue, buf2))
-  q2 = interleave(buf2, Split(lambda x: P.wait(split(x)).then(swap), queue, buf1))
-  q1.__name__ = f'Split{repr(queue)}1'
-  q2.__name__ = f'Split{repr(queue)}2'
-  return q1, q2
-
-def unzip(queue: ReadQueue[tuple[A, B]]) -> tuple[ReadQueue[A], ReadQueue[B]]:
-  q1, q2 = split(queue, lambda x: x)
-  q1.__name__ = f'Unzipped{repr(queue)}1'
-  q2.__name__ = f'Unzipped{repr(queue)}2'
-  return q1, q2
-
-def extend(
-  queue: ReadQueue[A],
-  extend: Callable[[A], B | Awaitable[B]]
-) -> tuple[ReadQueue[A], ReadQueue[B]]:
-  """`q1, q2 = extend(q, f)` is roughly equivalent to `q1 = q; q2 = q.map(f)`, except `q1` and `q2` are independent (popping one doesn't affect the other)"""
-  return split(queue, lambda x: P.wait(extend(x)).then(lambda r: (x, r)))
+#   async def _items(self) -> AsyncIterable[Either[QueueError, tuple[str, A]]]:
+#     async for e in self._queue._items():
+#       match e:
+#         case Right((id, v)):
+#           a, _ = await P.wait(self._split(v))
+#           yield Right((id, a))
+#         case err:
+#           yield err # type: ignore
+
+# def swap(pair: tuple[A, B]) -> tuple[B, A]:
+#   a, b = pair
+#   return b, a
+
+# def split(
+#   queue: ReadQueue[A],
+#   split: Callable[[A], tuple[B, C] | Awaitable[tuple[B, C]]]
+# ) -> tuple[ReadQueue[B], ReadQueue[C]]:
+#   buf1 = SimpleQueue[B]()
+#   buf2 = SimpleQueue[C]()
+#   q1 = interleave(buf1, Split(split, queue, buf2))
+#   q2 = interleave(buf2, Split(lambda x: P.wait(split(x)).then(swap), queue, buf1))
+#   q1.__name__ = f'Split{repr(queue)}1'
+#   q2.__name__ = f'Split{repr(queue)}2'
+#   return q1, q2
+
+# def unzip(queue: ReadQueue[tuple[A, B]]) -> tuple[ReadQueue[A], ReadQueue[B]]:
+#   q1, q2 = split(queue, lambda x: x)
+#   q1.__name__ = f'Unzipped{repr(queue)}1'
+#   q2.__name__ = f'Unzipped{repr(queue)}2'
+#   return q1, q2
+
+# def extend(
+#   queue: ReadQueue[A],
+#   extend: Callable[[A], B | Awaitable[B]]
+# ) -> tuple[ReadQueue[A], ReadQueue[B]]:
+#   """`q1, q2 = extend(q, f)` is roughly equivalent to `q1 = q; q2 = q.map(f)`, except `q1` and `q2` are independent (popping one doesn't affect the other)"""
+#   return split(queue, lambda x: P.wait(extend(x)).then(lambda r: (x, r)))
```

### Comparing `queue_api-0.1.5/src/q/api/ops/teeing.py` & `queue_api-0.1.6/src/q/api/ops/teeing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from typing import TypeVar, Generic, Sequence, overload
 import asyncio
-from ..api import WriteQueue
+from haskellian import either as E, Either, Left, Right
+from .. import WriteQueue, QueueError
 
 A = TypeVar('A')
 
 class tee(WriteQueue[A], Generic[A]):
   """A queue that pushes to the multiple queues at once"""
 
   @overload
   def __init__(self, queues: Sequence[WriteQueue[A]]): ...
   @overload
   def __init__(self, q1: WriteQueue[A], q2: WriteQueue[A], /, *qs: WriteQueue[A]): ...
   
   def __init__(self, *args):
-    self._queues = args[0] if len(args) == 1 else args
+    self._queues: Sequence[WriteQueue[A]] = args[0] if len(args) == 1 else args
 
-  async def push(self, key: str, value: A):
-    await asyncio.gather(*[q.push(key, value) for q in self._queues])
+  async def push(self, key: str, value: A) -> Either[QueueError, None]:
+    results = await asyncio.gather(*[q.push(key, value) for q in self._queues])
+    match E.sequence(results):
+      case Left(errs):
+        return Left(QueueError(errs))
+      case _:
+        return Right(None)
```

### Comparing `queue_api-0.1.5/src/queue_api.egg-info/SOURCES.txt` & `queue_api-0.1.6/src/queue_api.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 README.md
 pyproject.toml
 src/q/api/__init__.py
 src/q/api/__init__.pyi
-src/q/api/api/__init__.py
-src/q/api/api/append.py
-src/q/api/api/queue.py
-src/q/api/api/read.py
-src/q/api/api/write.py
+src/q/api/append.py
+src/q/api/errors.py
+src/q/api/queue.py
+src/q/api/read.py
+src/q/api/write.py
 src/q/api/impl/__init__.py
 src/q/api/impl/empty.py
 src/q/api/impl/simple.py
 src/q/api/ops/__init__.py
 src/q/api/ops/__init__.pyi
 src/q/api/ops/append_bounding.py
 src/q/api/ops/bounding.py
```

