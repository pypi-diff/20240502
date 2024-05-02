# Comparing `tmp/mptradelib-0.2.1.tar.gz` & `tmp/mptradelib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mptradelib-0.2.1.tar", max compression
+gzip compressed data, was "mptradelib-0.3.0.tar", max compression
```

## Comparing `mptradelib-0.2.1.tar` & `mptradelib-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     3256 2024-04-30 11:50:05.881417 mptradelib-0.2.1/README.md
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.2.1/mptradelib/__init__.py
--rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.2.1/mptradelib/broker/__init__.py
--rw-r--r--   0        0        0     5750 2024-05-01 10:07:01.546960 mptradelib-0.2.1/mptradelib/broker/broker.py
--rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.2.1/mptradelib/broker/session.py
--rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.2.1/mptradelib/broker/ticker.py
--rw-r--r--   0        0        0     3227 2024-04-30 08:23:49.270381 mptradelib-0.2.1/mptradelib/feed.py
--rw-r--r--   0        0        0      912 2024-04-30 08:25:53.372354 mptradelib-0.2.1/mptradelib/livetrading.py
--rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.2.1/mptradelib/shoonya.py
--rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.2.1/mptradelib/test_renko.py
--rw-r--r--   0        0        0      651 2024-04-30 08:25:03.006597 mptradelib-0.2.1/mptradelib/utils.py
--rw-r--r--   0        0        0     4162 2024-04-30 11:43:56.632362 mptradelib-0.2.1/mptradelib/vectorised_backtest.py
--rw-r--r--   0        0        0      561 2024-05-01 14:48:05.065027 mptradelib-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3820 1970-01-01 00:00:00.000000 mptradelib-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3256 2024-04-30 11:50:05.881417 mptradelib-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.256174 mptradelib-0.3.0/mptradelib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 08:23:49.266753 mptradelib-0.3.0/mptradelib/broker/__init__.py
+-rw-r--r--   0        0        0     5728 2024-05-02 08:04:56.402627 mptradelib-0.3.0/mptradelib/broker/broker.py
+-rw-r--r--   0        0        0     5818 2024-04-30 11:44:33.569478 mptradelib-0.3.0/mptradelib/broker/session.py
+-rw-r--r--   0        0        0     2683 2024-05-01 14:36:23.728530 mptradelib-0.3.0/mptradelib/broker/ticker.py
+-rw-r--r--   0        0        0     3889 2024-05-02 08:04:37.700859 mptradelib-0.3.0/mptradelib/feed.py
+-rw-r--r--   0        0        0     1866 2024-05-02 08:01:45.468179 mptradelib-0.3.0/mptradelib/livetrading.py
+-rw-r--r--   0        0        0    34066 2024-05-01 10:05:54.173058 mptradelib-0.3.0/mptradelib/shoonya.py
+-rw-r--r--   0        0        0     1313 2024-04-30 08:23:49.272908 mptradelib-0.3.0/mptradelib/test_renko.py
+-rw-r--r--   0        0        0      651 2024-04-30 08:25:03.006597 mptradelib-0.3.0/mptradelib/utils.py
+-rw-r--r--   0        0        0     4162 2024-04-30 11:43:56.632362 mptradelib-0.3.0/mptradelib/vectorised_backtest.py
+-rw-r--r--   0        0        0      561 2024-05-02 08:05:22.046511 mptradelib-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3820 1970-01-01 00:00:00.000000 mptradelib-0.3.0/PKG-INFO
```

### Comparing `mptradelib-0.2.1/README.md` & `mptradelib-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mptradelib-0.2.1/mptradelib/broker/broker.py` & `mptradelib-0.3.0/mptradelib/broker/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 
 
 class Historical:
     def __init__(self, session: FyersSession) -> None:
         self._session = session
         self._client = None
 
-    def historical(self, market, symbol, resolution, start, end):
+    def historical(self, symbol, resolution, start, end):
         curr = start
         delta = dt.timedelta(days=100)
         final_data = []
         if self._client is None:
             self._client = self._session.init_client()
         
         while curr < end:
             payload = {
-                "symbol": f"{market}:{symbol}",
+                "symbol": symbol,
                 "resolution": f"{resolution}",
                 "date_format": "1",
                 "range_from": f'{curr:%Y-%m-%d}',
                 "range_to": f'{(curr + delta):%Y-%m-%d}',
                 "cont_flag": "1",
             }
```

### Comparing `mptradelib-0.2.1/mptradelib/broker/session.py` & `mptradelib-0.3.0/mptradelib/broker/session.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.2.1/mptradelib/broker/ticker.py` & `mptradelib-0.3.0/mptradelib/broker/ticker.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.2.1/mptradelib/feed.py` & `mptradelib-0.3.0/mptradelib/feed.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import threading
 import datetime as dt
 import pandas as pd
 from pydantic import BaseModel, Field
 from collections import OrderedDict
 from typing import Callable, List
+from .broker.broker import Historical
 
 
 class Tick(BaseModel):
     datetime: dt.datetime
     ltp: float
     symbol: str
 
@@ -40,20 +41,24 @@
     @property
     def df(self):
         return pd.DataFrame(list(self))
 
 class Datas:
     _datas: dict = {}
 
-    def __init__(self, r: redis.Redis, resample_period: int = 1) -> None:
+    def __init__(self, r: redis.Redis, h: Historical, resample_period: int = 1) -> None:
         self._r = r
         self._resample_period = resample_period
+        self._h = h
 
     def _generate_key(self, a: dt.datetime):
         return f"{a:%Y-%m-%d-%H-%M}"
+    
+    def symbols(self):
+        return self._datas.keys()
 
     def update(self, tick: Tick):
         key = self._generate_key(tick.datetime)
 
         try:
             series = self._datas[tick.symbol]
         except KeyError:
@@ -65,26 +70,40 @@
         except Exception as e:
             series[key] = Candle(
                 datetime=tick.datetime.replace(second=0),
                 symbol=tick.symbol,
                 ltp=tick.ltp
             ).update(tick).model_dump()
 
-    def load(self, symbol: str, data: List[dict]):
+    def _load_worker(self, symbol: str, start_date: dt.datetime, end_date: dt.datetime):
         try:
             series = self._datas[symbol]
         except KeyError:
             self._datas[symbol] = OrderedDict()
             series = self._datas[symbol]
 
-        for d in data:
+        data = self._h.historical(symbol, 1, start_date, end_date)
+        for d in data.to_dict('records'):
             c = Candle.model_validate(d)
             key = self._generate_key(c.datetime)
             series[key] = c.model_dump()
-            
+
+    def load(self, symbols: List[str], period=7):
+        end_date = dt.datetime.now()
+        start_date = end_date - dt.timedelta(days=period)
+
+        threads = []
+        for symbol in symbols:    
+            t = threading.Thread(target=self._load_worker, args=[symbol, start_date, end_date])
+            t.start()
+            threads.append(t)
+
+        for t in threads:
+            t.join()
+                
 
     def __getitem__(self, index):
         return Series(self._datas[index].values())
     
     def _listen(self, channel, on_message: Callable[[Tick],None]):
         con = self._r.pubsub()
         con.subscribe(channel)
```

### Comparing `mptradelib-0.2.1/mptradelib/shoonya.py` & `mptradelib-0.3.0/mptradelib/shoonya.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.2.1/mptradelib/test_renko.py` & `mptradelib-0.3.0/mptradelib/test_renko.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.2.1/mptradelib/utils.py` & `mptradelib-0.3.0/mptradelib/utils.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.2.1/mptradelib/vectorised_backtest.py` & `mptradelib-0.3.0/mptradelib/vectorised_backtest.py`

 * *Files identical despite different names*

### Comparing `mptradelib-0.2.1/pyproject.toml` & `mptradelib-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mptradelib"
-version = "0.2.1"
+version = "0.3.0"
 description = ""
 authors = ["Abhilash Nanda <wishabhilash@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = "2.7.1"
```

### Comparing `mptradelib-0.2.1/PKG-INFO` & `mptradelib-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mptradelib
-Version: 0.2.1
+Version: 0.3.0
 Summary: 
 Author: Abhilash Nanda
 Author-email: wishabhilash@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

