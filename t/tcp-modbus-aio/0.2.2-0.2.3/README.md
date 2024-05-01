# Comparing `tmp/tcp_modbus_aio-0.2.2.tar.gz` & `tmp/tcp_modbus_aio-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcp_modbus_aio-0.2.2.tar", max compression
+gzip compressed data, was "tcp_modbus_aio-0.2.3.tar", max compression
```

## Comparing `tcp_modbus_aio-0.2.2.tar` & `tcp_modbus_aio-0.2.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1074 2024-05-01 21:34:43.663422 tcp_modbus_aio-0.2.2/LICENSE
--rw-r--r--   0        0        0     1649 2024-05-01 21:34:43.663422 tcp_modbus_aio-0.2.2/README.md
--rw-r--r--   0        0        0      857 2024-05-01 21:34:44.383420 tcp_modbus_aio-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-01 21:34:44.391420 tcp_modbus_aio-0.2.2/tcp_modbus_aio/__init__.py
--rw-r--r--   0        0        0    20487 2024-05-01 21:34:43.663422 tcp_modbus_aio-0.2.2/tcp_modbus_aio/client.py
--rw-r--r--   0        0        0      267 2024-05-01 21:34:43.663422 tcp_modbus_aio-0.2.2/tcp_modbus_aio/exceptions.py
--rw-r--r--   0        0        0     1167 2024-05-01 21:34:43.663422 tcp_modbus_aio-0.2.2/tcp_modbus_aio/ping.py
--rw-r--r--   0        0        0        0 2024-05-01 21:34:43.663422 tcp_modbus_aio-0.2.2/tcp_modbus_aio/py.typed
--rw-r--r--   0        0        0     2889 2024-05-01 21:34:43.663422 tcp_modbus_aio-0.2.2/tcp_modbus_aio/typed_functions.py
--rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 tcp_modbus_aio-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-01 22:17:48.225671 tcp_modbus_aio-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1649 2024-05-01 22:17:48.225671 tcp_modbus_aio-0.2.3/README.md
+-rw-r--r--   0        0        0      857 2024-05-01 22:17:48.953678 tcp_modbus_aio-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-01 22:17:48.961678 tcp_modbus_aio-0.2.3/tcp_modbus_aio/__init__.py
+-rw-r--r--   0        0        0    20491 2024-05-01 22:17:48.225671 tcp_modbus_aio-0.2.3/tcp_modbus_aio/client.py
+-rw-r--r--   0        0        0      267 2024-05-01 22:17:48.225671 tcp_modbus_aio-0.2.3/tcp_modbus_aio/exceptions.py
+-rw-r--r--   0        0        0     1167 2024-05-01 22:17:48.225671 tcp_modbus_aio-0.2.3/tcp_modbus_aio/ping.py
+-rw-r--r--   0        0        0        0 2024-05-01 22:17:48.225671 tcp_modbus_aio-0.2.3/tcp_modbus_aio/py.typed
+-rw-r--r--   0        0        0     2889 2024-05-01 22:17:48.225671 tcp_modbus_aio-0.2.3/tcp_modbus_aio/typed_functions.py
+-rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 tcp_modbus_aio-0.2.3/PKG-INFO
```

### Comparing `tcp_modbus_aio-0.2.2/LICENSE` & `tcp_modbus_aio-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.2.2/README.md` & `tcp_modbus_aio-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.2.2/pyproject.toml` & `tcp_modbus_aio-0.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tcp-modbus-aio"
-version = "0.2.2"
+version = "0.2.3"
 description = "asyncio client library for tcp modbus devices"
 authors = ["Josh Gruenstein <josh@tutorintelligence.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `tcp_modbus_aio-0.2.2/tcp_modbus_aio/client.py` & `tcp_modbus_aio-0.2.3/tcp_modbus_aio/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     from typing_extensions import Self
     from umodbus.functions import ModbusFunction
 
 
 @dataclass
 class CoilWatchStatus:
-    msg: ModbusFunction
+    msg: "ModbusFunction"
 
     memo_key: Any
     expiry: float
     hz: float
     task: asyncio.Task | None = None
 
 
@@ -224,15 +224,15 @@
         if self._ping_loop is not None:
             if self.logger is not None:
                 self.logger.debug(f"[{self}][close] Cancelling ping loop")
             self._ping_loop.cancel()
             self._ping_loop = None
 
     def log_watch(
-        self, msg: ModbusFunction, *, memo_key: Any, period: float, hz: float
+        self, msg: "ModbusFunction", *, memo_key: Any, period: float, hz: float
     ) -> None:
         """
         Triggers a loop that reads the coil(s) at the given index at the given frequency and
         writes the current values to logs for debugging purposes.
 
         This debug loop expires after the given period, but is refreshed every time this request_function
         is called.
```

### Comparing `tcp_modbus_aio-0.2.2/tcp_modbus_aio/ping.py` & `tcp_modbus_aio-0.2.3/tcp_modbus_aio/ping.py`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.2.2/tcp_modbus_aio/typed_functions.py` & `tcp_modbus_aio-0.2.3/tcp_modbus_aio/typed_functions.py`

 * *Files identical despite different names*

### Comparing `tcp_modbus_aio-0.2.2/PKG-INFO` & `tcp_modbus_aio-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcp-modbus-aio
-Version: 0.2.2
+Version: 0.2.3
 Summary: asyncio client library for tcp modbus devices
 License: MIT
 Author: Josh Gruenstein
 Author-email: josh@tutorintelligence.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

