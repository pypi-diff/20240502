# Comparing `tmp/tcp_modbus_aio-0.2.4.tar.gz` & `tmp/tcp_modbus_aio-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcp_modbus_aio-0.2.4.tar", max compression
+gzip compressed data, was "tcp_modbus_aio-0.2.5.tar", max compression
```

## Comparing `tcp_modbus_aio-0.2.4.tar` & `tcp_modbus_aio-0.2.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1074 2024-05-01 22:39:51.509933 tcp_modbus_aio-0.2.4/LICENSE
--rw-r--r--   0        0        0     1649 2024-05-01 22:39:51.509933 tcp_modbus_aio-0.2.4/README.md
--rw-r--r--   0        0        0      857 2024-05-01 22:39:52.289943 tcp_modbus_aio-0.2.4/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-01 22:39:52.293943 tcp_modbus_aio-0.2.4/tcp_modbus_aio/__init__.py
--rw-r--r--   0        0        0    20495 2024-05-01 22:39:51.513933 tcp_modbus_aio-0.2.4/tcp_modbus_aio/client.py
--rw-r--r--   0        0        0      267 2024-05-01 22:39:51.513933 tcp_modbus_aio-0.2.4/tcp_modbus_aio/exceptions.py
--rw-r--r--   0        0        0     1167 2024-05-01 22:39:51.513933 tcp_modbus_aio-0.2.4/tcp_modbus_aio/ping.py
--rw-r--r--   0        0        0        0 2024-05-01 22:39:51.513933 tcp_modbus_aio-0.2.4/tcp_modbus_aio/py.typed
--rw-r--r--   0        0        0     2889 2024-05-01 22:39:51.513933 tcp_modbus_aio-0.2.4/tcp_modbus_aio/typed_functions.py
--rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 tcp_modbus_aio-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-01 23:03:32.223270 tcp_modbus_aio-0.2.5/LICENSE
+-rw-r--r--   0        0        0     1649 2024-05-01 23:03:32.223270 tcp_modbus_aio-0.2.5/README.md
+-rw-r--r--   0        0        0      857 2024-05-01 23:03:32.939272 tcp_modbus_aio-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-01 23:03:32.947272 tcp_modbus_aio-0.2.5/tcp_modbus_aio/__init__.py
+-rw-r--r--   0        0        0    20495 2024-05-01 23:03:32.223270 tcp_modbus_aio-0.2.5/tcp_modbus_aio/client.py
+-rw-r--r--   0        0        0      267 2024-05-01 23:03:32.223270 tcp_modbus_aio-0.2.5/tcp_modbus_aio/exceptions.py
+-rw-r--r--   0        0        0     1167 2024-05-01 23:03:32.223270 tcp_modbus_aio-0.2.5/tcp_modbus_aio/ping.py
+-rw-r--r--   0        0        0        0 2024-05-01 23:03:32.223270 tcp_modbus_aio-0.2.5/tcp_modbus_aio/py.typed
+-rw-r--r--   0        0        0     2889 2024-05-01 23:03:32.223270 tcp_modbus_aio-0.2.5/tcp_modbus_aio/typed_functions.py
+-rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 tcp_modbus_aio-0.2.5/PKG-INFO
```

### Comparing `tcp_modbus_aio-0.2.4/LICENSE` & `tcp_modbus_aio-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.2.4/README.md` & `tcp_modbus_aio-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.2.4/pyproject.toml` & `tcp_modbus_aio-0.2.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tcp-modbus-aio"
-version = "0.2.4"
+version = "0.2.5"
 description = "asyncio client library for tcp modbus devices"
 authors = ["Josh Gruenstein <josh@tutorintelligence.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `tcp_modbus_aio-0.2.4/tcp_modbus_aio/client.py` & `tcp_modbus_aio-0.2.5/tcp_modbus_aio/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,15 @@
     async def __aenter__(self) -> "Self":
         return self
 
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
-        exc_tb: "TracebackType" | None,
+        exc_tb: "TracebackType | None",
     ) -> None:
         await self.close()
 
     async def close(self) -> None:
         """
         Permanent close of the TCP connection and ping loop.  Only call this on final destruction of the object.
         """
```

### Comparing `tcp_modbus_aio-0.2.4/tcp_modbus_aio/ping.py` & `tcp_modbus_aio-0.2.5/tcp_modbus_aio/ping.py`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.2.4/tcp_modbus_aio/typed_functions.py` & `tcp_modbus_aio-0.2.5/tcp_modbus_aio/typed_functions.py`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.2.4/PKG-INFO` & `tcp_modbus_aio-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcp-modbus-aio
-Version: 0.2.4
+Version: 0.2.5
 Summary: asyncio client library for tcp modbus devices
 License: MIT
 Author: Josh Gruenstein
 Author-email: josh@tutorintelligence.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

