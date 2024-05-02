# Comparing `tmp/mptradelib-0.2.0.tar.gz` & `tmp/mptradelib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mptradelib-0.2.0.tar", max compression
+gzip compressed data, was "mptradelib-0.2.1.tar", max compression
```

## Comparing `mptradelib-0.2.0.tar` & `mptradelib-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3256 2024-04-30 11:50:05.881417 mptradelib-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.2.0/mptradelib/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.2.0/mptradelib/broker/__init__.py
--rw-r--r--   0        0        0     5750 2024-05-01 10:07:01.546960 mptradelib-0.2.0/mptradelib/broker/broker.py
--rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.2.0/mptradelib/broker/session.py
--rw-r--r--   0        0        0     2384 2024-04-30 08:45:09.478921 mptradelib-0.2.0/mptradelib/broker/ticker.py
--rw-r--r--   0        0        0     3227 2024-04-30 08:23:49.270381 mptradelib-0.2.0/mptradelib/feed.py
--rw-r--r--   0        0        0      912 2024-04-30 08:25:53.372354 mptradelib-0.2.0/mptradelib/livetrading.py
--rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.2.0/mptradelib/shoonya.py
--rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.2.0/mptradelib/test_renko.py
--rw-r--r--   0        0        0      651 2024-04-30 08:25:03.006597 mptradelib-0.2.0/mptradelib/utils.py
--rw-r--r--   0        0        0     4162 2024-04-30 11:43:56.632362 mptradelib-0.2.0/mptradelib/vectorised_backtest.py
--rw-r--r--   0        0        0      561 2024-05-01 10:07:22.791661 mptradelib-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3820 1970-01-01 00:00:00.000000 mptradelib-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3256 2024-04-30 11:50:05.881417 mptradelib-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.2.1/mptradelib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.2.1/mptradelib/broker/__init__.py
+-rw-r--r--   0        0        0     5750 2024-05-01 10:07:01.546960 mptradelib-0.2.1/mptradelib/broker/broker.py
+-rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.2.1/mptradelib/broker/session.py
+-rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.2.1/mptradelib/broker/ticker.py
+-rw-r--r--   0        0        0     3227 2024-04-30 08:23:49.270381 mptradelib-0.2.1/mptradelib/feed.py
+-rw-r--r--   0        0        0      912 2024-04-30 08:25:53.372354 mptradelib-0.2.1/mptradelib/livetrading.py
+-rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.2.1/mptradelib/shoonya.py
+-rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.2.1/mptradelib/test_renko.py
+-rw-r--r--   0        0        0      651 2024-04-30 08:25:03.006597 mptradelib-0.2.1/mptradelib/utils.py
+-rw-r--r--   0        0        0     4162 2024-04-30 11:43:56.632362 mptradelib-0.2.1/mptradelib/vectorised_backtest.py
+-rw-r--r--   0        0        0      561 2024-05-01 14:48:05.065027 mptradelib-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3820 1970-01-01 00:00:00.000000 mptradelib-0.2.1/PKG-INFO
```

### Comparing `mptradelib-0.2.0/README.md` & `mptradelib-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mptradelib-0.2.0/mptradelib/broker/broker.py` & `mptradelib-0.2.1/mptradelib/broker/broker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.2.0/mptradelib/broker/session.py` & `mptradelib-0.2.1/mptradelib/broker/session.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.2.0/mptradelib/broker/ticker.py` & `mptradelib-0.2.1/mptradelib/broker/ticker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import datetime as dt
 from fyers_apiv3 import fyersModel
 from fyers_apiv3.FyersWebsocket.data_ws import FyersDataSocket
 import time
 import random
 import threading
+import queue
+
+from redis import Redis
 
 try:
     import redis
 except ImportError:
     pass
 
 import json
@@ -32,14 +35,18 @@
     def is_live(self):
         return self._is_live
 
 class LiveTicker(BaseTicker):
     _client: fyersModel.FyersModel = None
     _ws: FyersDataSocket = None
 
+    def __init__(self, broker: None, r: Redis, channel="default-ticks") -> None:
+        super().__init__(broker, r, channel)
+        self._q = queue.Queue(1)
+
     def run(self):
         if self._client is None and self._broker is not None:
             self._client = self._broker.init_client()
         
         self._ws = FyersDataSocket(
             access_token=self._client.token,
             litemode=False,
@@ -47,20 +54,25 @@
             on_message=self.__on_message,
             on_error=self.__on_error,
             on_close=self.__on_close
         )
 
         self._ws.connect()
 
+        while True:
+            syms = self._q.get()
+            if syms:
+                self._ws.subscribe(syms)
+
     def __on_connect(self):
         print("connected")
         self._is_live = True
 
     def subscribe(self, symbols: list):
-        self._ws.subscribe(symbols=symbols)
+        self._q.put(symbols)
 
     def __on_message(self, msg):
         self._r.publish(self._channel, json.dumps(msg))
 
     def __on_error(self, err):
         print(err)
```

### Comparing `mptradelib-0.2.0/mptradelib/feed.py` & `mptradelib-0.2.1/mptradelib/feed.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.2.0/mptradelib/livetrading.py` & `mptradelib-0.2.1/mptradelib/livetrading.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.2.0/mptradelib/shoonya.py` & `mptradelib-0.2.1/mptradelib/shoonya.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.2.0/mptradelib/test_renko.py` & `mptradelib-0.2.1/mptradelib/test_renko.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.2.0/mptradelib/utils.py` & `mptradelib-0.2.1/mptradelib/utils.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.2.0/mptradelib/vectorised_backtest.py` & `mptradelib-0.2.1/mptradelib/vectorised_backtest.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.2.0/pyproject.toml` & `mptradelib-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mptradelib"
-version = "0.2.0"
+version = "0.2.1"
 description = ""
 authors = ["Abhilash Nanda <wishabhilash@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.7.1"
```

### Comparing `mptradelib-0.2.0/PKG-INFO` & `mptradelib-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mptradelib
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: Abhilash Nanda
 Author-email: wishabhilash@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

