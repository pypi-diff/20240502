# Comparing `tmp/bpx_py-1.0.1.tar.gz` & `tmp/bpx_py-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpx_py-1.0.1.tar", max compression
+gzip compressed data, was "bpx_py-1.1.1.tar", max compression
```

## Comparing `bpx_py-1.0.1.tar` & `bpx_py-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0    11357 2024-04-27 17:11:08.473700 bpx_py-1.0.1/LICENSE
--rw-r--r--   0        0        0     2221 2024-04-29 17:25:24.867025 bpx_py-1.0.1/README.md
--rw-r--r--   0        0        0        0 2024-04-28 22:07:10.876817 bpx_py-1.0.1/bpx/__async/__init__.py
--rw-r--r--   0        0        0     4970 2024-04-29 17:25:24.868023 bpx_py-1.0.1/bpx/__async/account.py
--rw-r--r--   0        0        0     1361 2024-04-29 17:25:24.868458 bpx_py-1.0.1/bpx/__async/public.py
--rw-r--r--   0        0        0        1 2024-04-28 22:07:10.877678 bpx_py-1.0.1/bpx/__init__.py
--rw-r--r--   0        0        0     4825 2024-04-29 17:25:24.868876 bpx_py-1.0.1/bpx/account.py
--rw-r--r--   0        0        0        0 2024-04-28 22:07:10.877959 bpx_py-1.0.1/bpx/base/__init__.py
--rw-r--r--   0        0        0     8448 2024-04-28 22:07:10.879684 bpx_py-1.0.1/bpx/base/base_account.py
--rw-r--r--   0        0        0     1777 2024-04-28 22:07:10.879940 bpx_py-1.0.1/bpx/base/base_public.py
--rw-r--r--   0        0        0     1131 2024-04-28 22:07:10.880527 bpx_py-1.0.1/bpx/enums/__init__.py
--rw-r--r--   0        0        0     1793 2024-04-28 22:07:10.881007 bpx_py-1.0.1/bpx/exceptions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 22:07:10.881056 bpx_py-1.0.1/bpx/http_client/__init__.py
--rw-r--r--   0        0        0     2103 2024-04-29 17:25:24.869317 bpx_py-1.0.1/bpx/http_client/async_http_client.py
--rw-r--r--   0        0        0      412 2024-04-29 17:25:24.869614 bpx_py-1.0.1/bpx/http_client/http_client.py
--rw-r--r--   0        0        0     1006 2024-04-29 17:25:24.869948 bpx_py-1.0.1/bpx/http_client/sync_http_client.py
--rw-r--r--   0        0        0     1240 2024-04-29 17:25:24.870322 bpx_py-1.0.1/bpx/public.py
--rw-r--r--   0        0        0     1280 2024-04-29 17:51:07.697758 bpx_py-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3420 1970-01-01 00:00:00.000000 bpx_py-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-27 17:11:08.473700 bpx_py-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2221 2024-04-29 17:25:24.867025 bpx_py-1.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-28 22:07:10.876817 bpx_py-1.1.1/bpx/__async/__init__.py
+-rw-r--r--   0        0        0     5170 2024-04-30 11:45:27.013116 bpx_py-1.1.1/bpx/__async/account.py
+-rw-r--r--   0        0        0     1573 2024-04-30 11:45:27.013777 bpx_py-1.1.1/bpx/__async/public.py
+-rw-r--r--   0        0        0        1 2024-04-28 22:07:10.877678 bpx_py-1.1.1/bpx/__init__.py
+-rw-r--r--   0        0        0     5025 2024-04-30 11:45:27.014480 bpx_py-1.1.1/bpx/account.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:07:10.877959 bpx_py-1.1.1/bpx/base/__init__.py
+-rw-r--r--   0        0        0     8448 2024-04-28 22:07:10.879684 bpx_py-1.1.1/bpx/base/base_account.py
+-rw-r--r--   0        0        0     1804 2024-04-30 11:45:27.015222 bpx_py-1.1.1/bpx/base/base_public.py
+-rw-r--r--   0        0        0     1131 2024-04-28 22:07:10.880527 bpx_py-1.1.1/bpx/enums/__init__.py
+-rw-r--r--   0        0        0     1793 2024-04-28 22:07:10.881007 bpx_py-1.1.1/bpx/exceptions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-28 22:07:10.881056 bpx_py-1.1.1/bpx/http_client/__init__.py
+-rw-r--r--   0        0        0     2100 2024-04-30 11:45:27.015711 bpx_py-1.1.1/bpx/http_client/async_http_client.py
+-rw-r--r--   0        0        0      409 2024-04-30 11:45:27.016197 bpx_py-1.1.1/bpx/http_client/http_client.py
+-rw-r--r--   0        0        0     1003 2024-04-30 11:45:27.016713 bpx_py-1.1.1/bpx/http_client/sync_http_client.py
+-rw-r--r--   0        0        0     1452 2024-04-30 11:45:27.017082 bpx_py-1.1.1/bpx/public.py
+-rw-r--r--   0        0        0     1181 2024-04-30 23:59:21.683964 bpx_py-1.1.1/bpx/simulations.py
+-rw-r--r--   0        0        0     1280 2024-05-01 00:00:06.646504 bpx_py-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3420 1970-01-01 00:00:00.000000 bpx_py-1.1.1/PKG-INFO
```

### Comparing `bpx_py-1.0.1/LICENSE` & `bpx_py-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bpx_py-1.0.1/README.md` & `bpx_py-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bpx_py-1.0.1/bpx/__async/account.py` & `bpx_py-1.1.1/bpx/__async/account.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,75 +1,78 @@
 from bpx.base.base_account import BaseAccount
 from bpx.http_client.async_http_client import AsyncHttpClient
 
+default_http_client = AsyncHttpClient()
 
-class Account(BaseAccount, AsyncHttpClient):
+
+class Account(BaseAccount):
     def __init__(self,
                  public_key: str,
                  secret_key: str,
                  window: int = 5000,
                  proxy: str = None,
-                 debug: bool = False
+                 debug: bool = False,
+                 http_client: AsyncHttpClient = default_http_client
                  ):
 
-        BaseAccount.__init__(self,
-                             public_key,
-                             secret_key,
-                             window,
-                             debug)
-        AsyncHttpClient.__init__(self, proxy=proxy)
+        super().__init__(public_key,
+                         secret_key,
+                         window,
+                         debug)
+        self.http_client = http_client
+        self.http_client.proxy = proxy
 
     async def get_balances(self, window: int = None):
         url, headers = super().get_balances(window)
-        return await self._get(url, headers=headers)
+        return await self.http_client.get(url, headers=headers)
 
     async def deposits(self, limit: int = 100, offset: int = 0, window: int = None):
         url, headers, params = super().deposits(limit, offset, window)
-        return await self._get(url, headers=headers, params=params)
+        return await self.http_client.get(url, headers=headers, params=params)
 
     async def get_deposit_address(self, blockchain: str, window: int = None):
         url, headers, params = super().get_deposit_address(blockchain, window)
-        return await self._get(url, headers=headers, params=params)
+        return await self.http_client.get(url, headers=headers, params=params)
 
     async def get_withdrawals(self, limit: int = 100, offset: int = 0, window: int = None):
         url, headers, params = super().get_withdrawals(limit, offset, window)
-        return await self._get(url, headers=headers, params=params)
+        return await self.http_client.get(url, headers=headers, params=params)
 
     async def withdrawal(self, address: str,
                    symbol: str,
                    blockchain: str,
                    quantity: str,
                    window: int = None):
         url, headers, params = super().withdrawal(address, symbol, blockchain, quantity, window)
-        return await self._post(url, headers=headers, data=params)
+        return await self.http_client.post(url, headers=headers, data=params)
 
     async def get_order_history_query(self, symbol: str, limit: int = 100, offset: int = 0, window: int = None):
         url, headers, params = super().get_order_history_query(symbol, limit, offset, window)
-        return await self._get(url, headers=headers, params=params)
+        return await self.http_client.get(url, headers=headers, params=params)
 
     async def get_fill_history_query(self, symbol: str,
                                limit: int = 100,
                                offset: int = 0,
                                __from: int = None,
                                to: int = None,
                                window: int = None):
         url, headers, params = super().get_fill_history_query(symbol,
                                                          limit,
                                                          offset,
                                                          __from,
                                                          to,
                                                          window)
-        return await self._get(url, headers=headers, params=params)
+        return await self.http_client.get(url, headers=headers, params=params)
 
     async def get_open_order(self, symbol: str,
                        order_id: str = None,
                        client_id: int = None,
                        window: int = None):
         url, headers, params = super().get_open_order(symbol, order_id, client_id, window)
-        return await self._get(url, headers=headers, params=params)
+        return await self.http_client.get(url, headers=headers, params=params)
 
     async def execute_order(self, symbol: str,
                       side: str,
                       order_type: str,
                       quantity: float,
                       time_in_force: str = None,
                       price: float = 0,
@@ -81,23 +84,23 @@
                       window: int = None):
 
         url, headers, params = super().execute_order(symbol, side, order_type,
                                                 time_in_force, quantity,
                                                 price, trigger_price,
                                                 self_trade_prevention, quote_quantity,
                                                 client_id, post_only, window)
-        return await self._post(url, headers=headers, data=params)
+        return await self.http_client.post(url, headers=headers, data=params)
 
     async def cancel_order(self, symbol: str,
                      order_id: str = None,
                      client_id: int = None,
                      window: int = None):
         url, headers, params = super().cancel_order(symbol, order_id, client_id, window)
-        return await self._delete(url, headers=headers, data=params)
+        return await self.http_client.delete(url, headers=headers, data=params)
 
     async def get_open_orders(self, symbol: str = None, window: int = None):
         url, headers, params = super().get_open_orders(symbol, window)
-        return await self._get(url, headers=headers, params=params)
+        return await self.http_client.get(url, headers=headers, params=params)
 
     async def cancel_all_orders(self, symbol: str, window: int = None):
         url, headers, params = super().cancel_all_orders(symbol, window)
-        return await self._delete(url, headers=headers, data=params)
+        return await self.http_client.delete(url, headers=headers, data=params)
```

### Comparing `bpx_py-1.0.1/bpx/__async/public.py` & `bpx_py-1.1.1/bpx/__async/public.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 from bpx.base.base_public import BasePublic
 from bpx.http_client.async_http_client import AsyncHttpClient
 
+default_http_client = AsyncHttpClient()
 
-class Public(BasePublic, AsyncHttpClient):
 
-    def __init__(self, proxy: str = None):
-        AsyncHttpClient.__init__(self, proxy=proxy)
+class Public(BasePublic):
+
+    def __init__(self, proxy: str = None, http_client: AsyncHttpClient = default_http_client):
+        self.http_client = http_client
+        self.http_client.proxy = proxy
 
     async def get_assets(self):
-        return await self._get(self.get_assets_url())
+        return await self.http_client.get(self.get_assets_url())
 
     async def get_markets(self):
-        return await self._get(self.get_markets_url())
+        return await self.http_client.get(self.get_markets_url())
 
     async def get_ticker(self, symbol: str):
-        return await self._get(self.get_ticker_url(symbol))
+        return await self.http_client.get(self.get_ticker_url(symbol))
 
     async def get_depth(self, symbol: str):
-        return await self._get(self.get_depth_url(symbol))
+        return await self.http_client.get(self.get_depth_url(symbol))
 
     async def get_klines(self, symbol: str, interval: str, start_time=0, end_time=0):
-        return await self._get(self.get_klines_url(symbol, interval, start_time, end_time))
+        return await self.http_client.get(self.get_klines_url(symbol, interval, start_time, end_time))
 
     async def get_status(self):
-        return await self._get(self.get_status_url())
+        return await self.http_client.get(self.get_status_url())
 
     async def get_ping(self):
-        return await self._get(self.get_ping_url())
+        return await self.http_client.get(self.get_ping_url())
 
     async def get_time(self):
-        return await self._get(self.get_time_url())
+        return await self.http_client.get(self.get_time_url())
 
     async def get_recent_trades(self, symbol: str, limit=100):
-        return await self._get(self.get_recent_trades_url(symbol, limit))
+        return await self.http_client.get(self.get_recent_trades_url(symbol, limit))
 
     async def get_history_trades(self, symbol: str, limit=100, offset=0):
-        return await self._get(self.get_history_trades_url(symbol, limit, offset))
+        return await self.http_client.get(self.get_history_trades_url(symbol, limit, offset))
```

### Comparing `bpx_py-1.0.1/bpx/account.py` & `bpx_py-1.1.1/bpx/account.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,75 +1,78 @@
 from bpx.base.base_account import BaseAccount
 from bpx.http_client.sync_http_client import SyncHttpClient
 
+http_client = SyncHttpClient()
 
-class Account(BaseAccount, SyncHttpClient):
+
+class Account(BaseAccount):
     def __init__(self,
                  public_key: str,
                  secret_key: str,
                  window: int = 5000,
                  proxy: dict = None,
-                 debug: bool = False
+                 debug: bool = False,
+                 default_http_client: SyncHttpClient = http_client
                  ):
 
-        BaseAccount.__init__(self,
-                             public_key,
-                             secret_key,
-                             window,
-                             debug)
-        SyncHttpClient.__init__(self, proxies=proxy)
+        super().__init__(public_key,
+                         secret_key,
+                         window,
+                         debug)
+        self.http_client = default_http_client
+        self.http_client.proxies = proxy
 
     def get_balances(self, window: int = None):
         url, headers = super().get_balances(window)
-        return self._get(url, headers=headers)
+        return self.http_client.get(url, headers=headers)
 
     def deposits(self, limit: int = 100, offset: int = 0, window: int = None):
         url, headers, params = super().deposits(limit, offset, window)
-        return self._get(url, headers=headers, params=params)
+        return self.http_client.get(url, headers=headers, params=params)
 
     def get_deposit_address(self, blockchain: str, window: int = None):
         url, headers, params = super().get_deposit_address(blockchain, window)
-        return self._get(url, headers=headers, params=params)
+        return self.http_client.get(url, headers=headers, params=params)
 
     def get_withdrawals(self, limit: int = 100, offset: int = 0, window: int = None):
         url, headers, params = super().get_withdrawals(limit, offset, window)
-        return self._get(url, headers=headers, params=params)
+        return self.http_client.get(url, headers=headers, params=params)
 
     def withdrawal(self, address: str,
                    symbol: str,
                    blockchain: str,
                    quantity: str,
                    window: int = None):
         url, headers, params = super().withdrawal(address, symbol, blockchain, quantity, window)
-        return self._post(url, headers=headers, data=params)
+        return self.http_client.post(url, headers=headers, data=params)
 
     def get_order_history_query(self, symbol: str, limit: int = 100, offset: int = 0, window: int = None):
         url, headers, params = super().get_order_history_query(symbol, limit, offset, window)
-        return self._get(url, headers=headers, params=params)
+        return self.http_client.get(url, headers=headers, params=params)
 
     def get_fill_history_query(self, symbol: str,
                                limit: int = 100,
                                offset: int = 0,
                                __from: int = None,
                                to: int = None,
                                window: int = None):
         url, headers, params = super().get_fill_history_query(symbol,
                                                          limit,
                                                          offset,
                                                          __from,
                                                          to,
                                                          window)
-        return self._get(url, headers=headers, params=params)
+        return self.http_client.get(url, headers=headers, params=params)
 
     def get_open_order(self, symbol: str,
                        order_id: str = None,
                        client_id: int = None,
                        window: int = None):
         url, headers, params = super().get_open_order(symbol, order_id, client_id, window)
-        return self._get(url, headers=headers, params=params)
+        return self.http_client.get(url, headers=headers, params=params)
 
     def execute_order(self, symbol: str,
                       side: str,
                       order_type: str,
                       quantity: float,
                       time_in_force: str = None,
                       price: float = 0,
@@ -81,23 +84,23 @@
                       window: int = None):
 
         url, headers, params = super().execute_order(symbol, side, order_type,
                                                 time_in_force, quantity,
                                                 price, trigger_price,
                                                 self_trade_prevention, quote_quantity,
                                                 client_id, post_only, window)
-        return self._post(url, headers=headers, data=params)
+        return self.http_client.post(url, headers=headers, data=params)
 
     def cancel_order(self, symbol: str,
                      order_id: str = None,
                      client_id: int = None,
                      window: int = None):
         url, headers, params = super().cancel_order(symbol, order_id, client_id, window)
-        return self._delete(url, headers=headers, data=params)
+        return self.http_client.delete(url, headers=headers, data=params)
 
     def get_open_orders(self, symbol: str = None, window: int = None):
         url, headers, params = super().get_open_orders(symbol, window)
-        return self._get(url, headers=headers, params=params)
+        return self.http_client.get(url, headers=headers, params=params)
 
     def cancel_all_orders(self, symbol: str, window: int = None):
         url, headers, params = super().cancel_all_orders(symbol, window)
-        return self._delete(url, headers=headers, data=params)
+        return self.http_client.delete(url, headers=headers, data=params)
```

### Comparing `bpx_py-1.0.1/bpx/base/base_account.py` & `bpx_py-1.1.1/bpx/base/base_account.py`

 * *Files identical despite different names*

### Comparing `bpx_py-1.0.1/bpx/base/base_public.py` & `bpx_py-1.1.1/bpx/base/base_public.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         return self._endpoint(f'api/v1/ticker?symbol={symbol}')
 
     def get_depth_url(self, symbol):
         return self._endpoint(f'api/v1/depth?symbol={symbol}')
 
     def get_klines_url(self, symbol, interval, start_time, end_time):
         if start_time < 0 or end_time < 0:
-            raise NegativeValueError
+            raise NegativeValueError("start_time and end_time")
         if not TimeInterval.has_value(interval):
             raise InvalidTimeIntervalError(interval)
         url = f'api/v1/klines?symbol={symbol}&interval={interval}'
         if start_time:
             url += f'&startTime={start_time}'
         if end_time:
             url += f'&endTime={end_time}'
```

### Comparing `bpx_py-1.0.1/bpx/enums/__init__.py` & `bpx_py-1.1.1/bpx/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `bpx_py-1.0.1/bpx/exceptions/__init__.py` & `bpx_py-1.1.1/bpx/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `bpx_py-1.0.1/bpx/http_client/async_http_client.py` & `bpx_py-1.1.1/bpx/http_client/async_http_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,41 +6,41 @@
 
 
 class AsyncHttpClient(HttpClient):
 
     def __init__(self, proxy: str = ""):
         self.proxy = proxy
 
-    async def _get(self, url, headers=None, params=None):
+    async def get(self, url, headers=None, params=None):
         ssl_context = ssl.create_default_context(cafile=certifi.where())
         async with aiohttp.ClientSession() as session:
             async with session.get(url, proxy=self.proxy, params=params,
                                    headers=headers, ssl=ssl_context) as response:
 
                 try:
                     return await response.json()
                 except json.JSONDecodeError:
                     return await response.text()
                 except aiohttp.client_exceptions.ContentTypeError:
                     return await response.text()
 
-    async def _post(self, url, headers=None, data=None):
+    async def post(self, url, headers=None, data=None):
         ssl_context = ssl.create_default_context(cafile=certifi.where())
         async with aiohttp.ClientSession() as session:
             async with session.post(url, proxy=self.proxy, headers=headers,
                                     data=json.dumps(data), ssl=ssl_context) as response:
 
                 try:
                     return await response.json()
                 except json.JSONDecodeError:
                     return await response.text()
                 except aiohttp.client_exceptions.ContentTypeError:
                     return await response.text()
 
-    async def _delete(self, url, headers=None, data=None):
+    async def delete(self, url, headers=None, data=None):
         ssl_context = ssl.create_default_context(cafile=certifi.where())
         async with aiohttp.ClientSession() as session:
             async with session.delete(url, proxy=self.proxy, headers=headers,
                                       data=json.dumps(data), ssl=ssl_context) as response:
 
                 try:
                     return await response.json()
```

### Comparing `bpx_py-1.0.1/bpx/http_client/sync_http_client.py` & `bpx_py-1.1.1/bpx/http_client/sync_http_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 import json
 
 
 class SyncHttpClient(HttpClient):
     def __init__(self, proxies: dict = None):
         self.proxies = proxies
 
-    def _get(self, url, headers=None, params=None):
+    def get(self, url, headers=None, params=None):
         response = requests.get(url=url, proxies=self.proxies, headers=headers, params=params)
         try:
             return response.json()
         except json.JSONDecodeError:
             return response.text
 
-    def _post(self, url, headers=None, data=None):
+    def post(self, url, headers=None, data=None):
         response = requests.post(url=url, proxies=self.proxies, headers=headers, data=json.dumps(data))
         try:
             return response.json()
         except json.JSONDecodeError:
             return response.text
 
-    def _delete(self, url, headers=None, data=None):
+    def delete(self, url, headers=None, data=None):
         response = requests.delete(url, proxies=self.proxies, headers=headers, data=json.dumps(data))
         try:
             return response.json()
         except json.JSONDecodeError:
             return response.text
```

### Comparing `bpx_py-1.0.1/bpx/public.py` & `bpx_py-1.1.1/bpx/public.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 from bpx.base.base_public import BasePublic
 from bpx.http_client.sync_http_client import SyncHttpClient
 
+default_http_client = SyncHttpClient()
 
-class Public(BasePublic, SyncHttpClient):
 
-    def __init__(self, proxy: dict = None):
-        SyncHttpClient.__init__(self, proxies=proxy)
+class Public(BasePublic):
+
+    def __init__(self, proxy: dict = None, http_client: SyncHttpClient = default_http_client):
+        self.http_client = http_client
+        self.http_client.proxies = proxy
 
     def get_assets(self):
-        return self._get(self.get_assets_url())
+        return self.http_client.get(self.get_assets_url())
 
     def get_markets(self):
-        return self._get(self.get_markets_url())
+        return self.http_client.get(self.get_markets_url())
 
     def get_ticker(self, symbol: str):
-        return self._get(self.get_ticker_url(symbol))
+        return self.http_client.get(self.get_ticker_url(symbol))
 
     def get_depth(self, symbol: str):
-        return self._get(self.get_depth_url(symbol))
+        return self.http_client.get(self.get_depth_url(symbol))
 
     def get_klines(self, symbol: str, interval: str, start_time=0, end_time=0):
-        return self._get(self.get_klines_url(symbol, interval, start_time, end_time))
+        return self.http_client.get(self.get_klines_url(symbol, interval, start_time, end_time))
 
     def get_status(self):
-        return self._get(self.get_status_url())
+        return self.http_client.get(self.get_status_url())
 
     def get_ping(self):
-        return self._get(self.get_ping_url())
+        return self.http_client.get(self.get_ping_url())
 
     def get_time(self):
-        return self._get(self.get_time_url())
+        return self.http_client.get(self.get_time_url())
 
     def get_recent_trades(self, symbol: str, limit=100):
-        return self._get(self.get_recent_trades_url(symbol, limit))
+        return self.http_client.get(self.get_recent_trades_url(symbol, limit))
 
     def get_history_trades(self, symbol: str, limit=100, offset=0):
-        return self._get(self.get_history_trades_url(symbol, limit, offset))
+        return self.http_client.get(self.get_history_trades_url(symbol, limit, offset))
```

### Comparing `bpx_py-1.0.1/pyproject.toml` & `bpx_py-1.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpx-py"
-version = "1.0.1"
+version = "1.1.1"
 description = "Backpack API SDK tool"
 authors = ["sndmndss <yanfedorov120505@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage="https://backpack.exchange"
 repository="https://github.com/sndmndss/bpx-py/"
 keywords = ["api", "sdk", "backpack", "client", "wrapper"]
```

### Comparing `bpx_py-1.0.1/PKG-INFO` & `bpx_py-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpx-py
-Version: 1.0.1
+Version: 1.1.1
 Summary: Backpack API SDK tool
 Home-page: https://backpack.exchange
 License: Apache-2.0
 Keywords: api,sdk,backpack,client,wrapper
 Author: sndmndss
 Author-email: yanfedorov120505@gmail.com
 Requires-Python: >=3.8,<4.0
```

