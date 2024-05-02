# Comparing `tmp/ibind-0.0.1.tar.gz` & `tmp/ibind-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibind-0.0.1.tar", last modified: Wed Apr  3 12:33:38 2024, max compression
+gzip compressed data, was "ibind-0.0.2.tar", last modified: Thu May  2 11:01:52 2024, max compression
```

## Comparing `ibind-0.0.1.tar` & `ibind-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,63 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:38.000656 ibind-0.0.1/
--rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibind-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     6744 2024-04-03 12:33:37.997617 ibind-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5975 2024-04-03 12:27:15.000000 ibind-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:37.908611 ibind-0.0.1/ibind/
--rw-rw-rw-   0        0        0      281 2024-04-03 12:27:15.000000 ibind-0.0.1/ibind/__init__.py
--rw-rw-rw-   0        0        0     1996 2024-04-01 11:07:46.000000 ibind-0.0.1/ibind/var.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:37.994619 ibind-0.0.1/ibind.egg-info/
--rw-rw-rw-   0        0        0     6744 2024-04-03 12:33:37.000000 ibind-0.0.1/ibind.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      753 2024-04-03 12:33:37.000000 ibind-0.0.1/ibind.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 12:33:37.000000 ibind-0.0.1/ibind.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-04-03 12:33:37.000000 ibind-0.0.1/ibind.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-03 12:33:37.000000 ibind-0.0.1/ibind.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-03 12:33:38.011732 ibind-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1329 2024-04-03 12:32:38.000000 ibind-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:37.939447 ibind-0.0.1/test/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:08.000000 ibind-0.0.1/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:37.944017 ibind-0.0.1/test/integration/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.0.1/test/integration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:37.958573 ibind-0.0.1/test/integration/base/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:37:06.000000 ibind-0.0.1/test/integration/base/__init__.py
--rw-rw-rw-   0        0        0     3714 2024-04-03 12:27:51.000000 ibind-0.0.1/test/integration/base/test_rest_client_i.py
--rw-rw-rw-   0        0        0    10983 2024-04-03 12:29:16.000000 ibind-0.0.1/test/integration/base/test_websocket_client_i.py
--rw-rw-rw-   0        0        0     1477 2023-12-13 15:29:14.000000 ibind-0.0.1/test/integration/base/websocketapp_mock.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:37.978647 ibind-0.0.1/test/integration/client/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:57:40.000000 ibind-0.0.1/test/integration/client/__init__.py
--rw-rw-rw-   0        0        0    39617 2024-04-01 08:07:19.000000 ibind-0.0.1/test/integration/client/ibkr_responses.py
--rw-rw-rw-   0        0        0    14434 2024-04-03 12:29:16.000000 ibind-0.0.1/test/integration/client/test_ibkr_client_i.py
--rw-rw-rw-   0        0        0    11825 2024-04-03 12:28:11.000000 ibind-0.0.1/test/integration/client/test_ibkr_utils_i.py
--rw-rw-rw-   0        0        0    18899 2024-04-03 12:29:29.000000 ibind-0.0.1/test/integration/client/test_ibkr_ws_client_i.py
--rw-rw-rw-   0        0        0     8874 2024-04-03 12:27:51.000000 ibind-0.0.1/test/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:37.983239 ibind-0.0.1/test/unit/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.0.1/test/unit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:33:37.990179 ibind-0.0.1/test/unit/support/
--rw-rw-rw-   0        0        0        0 2024-04-01 07:45:52.000000 ibind-0.0.1/test/unit/support/__init__.py
--rw-rw-rw-   0        0        0     4517 2024-04-03 12:30:12.000000 ibind-0.0.1/test/unit/support/test_py_utils_u.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.553327 ibind-0.0.2/
+-rw-rw-rw-   0        0        0    11562 2020-10-15 10:25:32.000000 ibind-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     9482 2024-05-02 11:01:52.551327 ibind-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8716 2024-05-02 10:25:06.000000 ibind-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.434199 ibind-0.0.2/ibind/
+-rw-rw-rw-   0        0        0     1087 2024-05-02 11:00:44.000000 ibind-0.0.2/ibind/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.459377 ibind-0.0.2/ibind/base/
+-rw-rw-rw-   0        0        0        0 2024-04-04 04:03:06.000000 ibind-0.0.2/ibind/base/__init__.py
+-rw-rw-rw-   0        0        0     5286 2024-05-02 07:49:30.000000 ibind-0.0.2/ibind/base/queue_controller.py
+-rw-rw-rw-   0        0        0     8546 2024-04-24 12:33:10.000000 ibind-0.0.2/ibind/base/rest_client.py
+-rw-rw-rw-   0        0        0    16433 2024-05-02 04:33:50.000000 ibind-0.0.2/ibind/base/subscription_controller.py
+-rw-rw-rw-   0        0        0    18799 2024-05-02 07:52:05.000000 ibind-0.0.2/ibind/base/ws_client.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.471910 ibind-0.0.2/ibind/client/
+-rw-rw-rw-   0        0        0        0 2024-04-03 12:59:53.000000 ibind-0.0.2/ibind/client/__init__.py
+-rw-rw-rw-   0        0        0     3444 2024-05-02 10:30:13.000000 ibind-0.0.2/ibind/client/ibkr_client.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.494588 ibind-0.0.2/ibind/client/ibkr_client_mixins/
+-rw-rw-rw-   0        0        0        0 2024-04-04 04:14:49.000000 ibind-0.0.2/ibind/client/ibkr_client_mixins/__init__.py
+-rw-rw-rw-   0        0        0     3400 2024-05-02 04:33:53.000000 ibind-0.0.2/ibind/client/ibkr_client_mixins/accounts_mixin.py
+-rw-rw-rw-   0        0        0    16132 2024-04-25 11:38:46.000000 ibind-0.0.2/ibind/client/ibkr_client_mixins/contract_mixin.py
+-rw-rw-rw-   0        0        0    12508 2024-05-02 07:59:06.000000 ibind-0.0.2/ibind/client/ibkr_client_mixins/marketdata_mixin.py
+-rw-rw-rw-   0        0        0    10477 2024-05-02 10:28:02.000000 ibind-0.0.2/ibind/client/ibkr_client_mixins/order_mixin.py
+-rw-rw-rw-   0        0        0     9585 2024-05-02 10:28:35.000000 ibind-0.0.2/ibind/client/ibkr_client_mixins/portfolio_mixin.py
+-rw-rw-rw-   0        0        0     4220 2024-05-02 10:28:35.000000 ibind-0.0.2/ibind/client/ibkr_client_mixins/scanner_mixin.py
+-rw-rw-rw-   0        0        0     4611 2024-05-02 10:28:43.000000 ibind-0.0.2/ibind/client/ibkr_client_mixins/session_mixin.py
+-rw-rw-rw-   0        0        0     2343 2024-05-02 10:30:13.000000 ibind-0.0.2/ibind/client/ibkr_client_mixins/watchlist_mixin.py
+-rw-rw-rw-   0        0        0    12413 2024-04-24 12:43:26.000000 ibind-0.0.2/ibind/client/ibkr_definitions.py
+-rw-rw-rw-   0        0        0    16278 2024-05-02 06:20:14.000000 ibind-0.0.2/ibind/client/ibkr_utils.py
+-rw-rw-rw-   0        0        0    22815 2024-05-02 07:55:01.000000 ibind-0.0.2/ibind/client/ibkr_ws_client.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.505138 ibind-0.0.2/ibind/support/
+-rw-rw-rw-   0        0        0        0 2024-04-03 13:00:28.000000 ibind-0.0.2/ibind/support/__init__.py
+-rw-rw-rw-   0        0        0      227 2024-04-01 07:18:14.000000 ibind-0.0.2/ibind/support/errors.py
+-rw-rw-rw-   0        0        0     5612 2024-05-02 10:37:05.000000 ibind-0.0.2/ibind/support/logs.py
+-rw-rw-rw-   0        0        0    11297 2024-05-02 07:22:22.000000 ibind-0.0.2/ibind/support/py_utils.py
+-rw-rw-rw-   0        0        0     2035 2024-04-25 10:00:26.000000 ibind-0.0.2/ibind/var.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.549325 ibind-0.0.2/ibind.egg-info/
+-rw-rw-rw-   0        0        0     9482 2024-05-02 11:01:52.000000 ibind-0.0.2/ibind.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1580 2024-05-02 11:01:52.000000 ibind-0.0.2/ibind.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 11:01:52.000000 ibind-0.0.2/ibind.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-02 11:01:52.000000 ibind-0.0.2/ibind.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-02 11:01:52.000000 ibind-0.0.2/ibind.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-02 11:01:52.555328 ibind-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1328 2024-05-02 11:01:12.000000 ibind-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.510513 ibind-0.0.2/test/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:08.000000 ibind-0.0.2/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.512543 ibind-0.0.2/test/integration/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.0.2/test/integration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.525039 ibind-0.0.2/test/integration/base/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:37:06.000000 ibind-0.0.2/test/integration/base/__init__.py
+-rw-rw-rw-   0        0        0     3714 2024-04-03 12:45:17.000000 ibind-0.0.2/test/integration/base/test_rest_client_i.py
+-rw-rw-rw-   0        0        0    11025 2024-04-24 10:05:09.000000 ibind-0.0.2/test/integration/base/test_websocket_client_i.py
+-rw-rw-rw-   0        0        0     1477 2023-12-13 15:29:14.000000 ibind-0.0.2/test/integration/base/websocketapp_mock.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.538105 ibind-0.0.2/test/integration/client/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:57:40.000000 ibind-0.0.2/test/integration/client/__init__.py
+-rw-rw-rw-   0        0        0    39617 2024-04-01 08:07:19.000000 ibind-0.0.2/test/integration/client/ibkr_responses.py
+-rw-rw-rw-   0        0        0    14441 2024-04-25 11:38:46.000000 ibind-0.0.2/test/integration/client/test_ibkr_client_i.py
+-rw-rw-rw-   0        0        0    11825 2024-04-03 12:28:11.000000 ibind-0.0.2/test/integration/client/test_ibkr_utils_i.py
+-rw-rw-rw-   0        0        0    18758 2024-04-24 11:56:20.000000 ibind-0.0.2/test/integration/client/test_ibkr_ws_client_i.py
+-rw-rw-rw-   0        0        0     8874 2024-04-03 12:27:51.000000 ibind-0.0.2/test/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.541104 ibind-0.0.2/test/unit/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:47:26.000000 ibind-0.0.2/test/unit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:01:52.546104 ibind-0.0.2/test/unit/support/
+-rw-rw-rw-   0        0        0        0 2024-04-01 07:45:52.000000 ibind-0.0.2/test/unit/support/__init__.py
+-rw-rw-rw-   0        0        0     4517 2024-04-03 12:30:12.000000 ibind-0.0.2/test/unit/support/test_py_utils_u.py
```

### Comparing `ibind-0.0.1/LICENSE` & `ibind-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ibind-0.0.1/ibind/var.py` & `ibind-0.0.2/ibind/var.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 import os
 import tempfile
+
 from distutils.util import strtobool
 
 
 def to_bool(value):
     return bool(strtobool(str(value)))
 
 
 ##### LOGS #####
 
 LOG_TO_CONSOLE = to_bool(os.environ.get('IBIND_LOG_TO_CONSOLE', True))
-"""Whether logs should be streamed to the standard output."""
+""" Whether logs should be streamed to the standard output. """
+
+LOG_TO_FILE = to_bool(os.environ.get('IBIND_LOG_TO_FILE', True))
+""" Whether logs should be saved to a file. """
 
-LOG_LEVEL = os.getenv('IBIND_LOG_LEVEL', 'DEBUG')
+LOG_LEVEL = os.getenv('IBIND_LOG_LEVEL', 'INFO')
 """ The global log level for the StreamHandler. """
 
 LOG_FORMAT = os.getenv('IBIND_LOG_FORMAT', '%(asctime)s|%(levelname)-.1s| %(message)s')
 """ Log format that is used by IBind """
 
 LOGS_DIR = os.getenv('IBIND_LOGS_DIR', tempfile.gettempdir())
 """ Directory of file logs produced. """
 
-LOG_TO_FILE = to_bool(os.environ.get('IBIND_LOG_TO_FILE', True))
-"""Whether logs should be saved to a file."""
-
 ##### IBKR #####
 
-IBKR_URL = os.getenv('IBKR_URL', None)
+IBIND_REST_URL = os.getenv('IBIND_REST_URL', None)
 """ IBKR Client Portal Gateway's URL for REST API."""
 
-IBKR_WS_URL = os.getenv('IBKR_WS_URL', None)
+IBIND_WS_URL = os.getenv('IBIND_WS_URL', None)
 """ IBKR Client Portal Gateway's URL for WebSocket API."""
 
-IBKR_ACCOUNT_ID = os.getenv('IBKR_ACCOUNT_ID', None)
+IBIND_ACCOUNT_ID = os.getenv('IBIND_ACCOUNT_ID', None)
 """ IBKR account ID to use."""
 
-IBKR_CACERT = os.getenv('IBKR_CACERT', False)
+IBIND_CACERT = os.getenv('IBIND_CACERT', False)
 """ Path to certificates used to communicate with IBKR Client Portal Gateway."""
 
-IBKR_WS_PING_INTERVAL = int(os.getenv('IBKR_WS_PING_INTERVAL', 45))
+IBIND_WS_PING_INTERVAL = int(os.getenv('IBIND_WS_PING_INTERVAL', 45))
 """ Interval between WebSocket pings. """
 
-IBKR_WS_MAX_PING_INTERVAL = int(os.getenv('IBKR_WS_MAX_PING_INTERVAL', 300))
+IBIND_WS_MAX_PING_INTERVAL = int(os.getenv('IBIND_WS_MAX_PING_INTERVAL', 300))
 """ Max accepted interval between WebSocket pings. """
 
-IBKR_WS_TIMEOUT = int(os.getenv('IBKR_WS_TIMEOUT', 5))
+IBIND_WS_TIMEOUT = int(os.getenv('IBIND_WS_TIMEOUT', 5))
 """ Timeout for WebSocket state change verifications. """
 
-IBKR_WS_SUBSCRIPTION_RETRIES = int(os.getenv('IBKR_WS_SUBSCRIPTION_RETRIES', 5))
+IBIND_WS_SUBSCRIPTION_RETRIES = int(os.getenv('IBIND_WS_SUBSCRIPTION_RETRIES', 5))
 """ Number of attempts to create a WebSocket subscription. """
 
-IBKR_WS_SUBSCRIPTION_TIMEOUT = int(os.getenv('IBKR_WS_SUBSCRIPTION_TIMEOUT', 2))
+IBIND_WS_SUBSCRIPTION_TIMEOUT = int(os.getenv('IBIND_WS_SUBSCRIPTION_TIMEOUT', 2))
 """ Timeout for WebSocket subscription verifications. """
 
-IBKR_WS_LOG_RAW_MESSAGES = to_bool(os.environ.get('IBKR_WS_LOG_RAW_MESSAGES', False))
-"""Whether raw WebSocket messages should be logged."""
+IBIND_WS_LOG_RAW_MESSAGES = to_bool(os.environ.get('IBIND_WS_LOG_RAW_MESSAGES', False))
+""" Whether raw WebSocket messages should be logged. """
```

### Comparing `ibind-0.0.1/setup.py` & `ibind-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,14 @@
     keywords=['interactive brokers', 'rest api', 'python api', 'ibkr python api', 'ibkr web api', 'ib api', 'ibkr api', 'algo trading', 'algorithmic trading', 'quant', 'trading'],
     install_requires=[
         'requests==2.31.*',
         'websocket-client==1.7.*'
     ],
 
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Programming Language :: Python :: 3.12',
     ],
 )
```

### Comparing `ibind-0.0.1/test/integration/base/test_rest_client_i.py` & `ibind-0.0.2/test/integration/base/test_rest_client_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.1/test/integration/base/test_websocket_client_i.py` & `ibind-0.0.2/test/integration/base/test_websocket_client_i.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     def setUp(self):
         self.url = 'wss://localhost:5000/v1/api/ws'
         self.max_reconnect_attempts = 4
         self.max_ping_interval = 38
         self.error_message = 'TEST_ERROR'
 
         self.ws_client = WsClient(
+            subscription_processor=None,
             url=self.url,
             cacert=False,
             timeout=0.01,
             max_connection_attempts=self.max_reconnect_attempts,
             max_ping_interval=self.max_ping_interval,
         )
```

### Comparing `ibind-0.0.1/test/integration/base/websocketapp_mock.py` & `ibind-0.0.2/test/integration/base/websocketapp_mock.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.1/test/integration/client/ibkr_responses.py` & `ibind-0.0.2/test/integration/client/ibkr_responses.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.1/test/integration/client/test_ibkr_client_i.py` & `ibind-0.0.2/test/integration/client/test_ibkr_client_i.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             StockQuery(symbol='SAN', name_match='SANTANDER', contract_conditions={'isUS': True}),
             StockQuery(symbol='SCHW', contract_conditions={'exchange': 'NYSE'}),
             StockQuery(symbol='TEAM', name_match='ATLASSIAN'),
             StockQuery(symbol='INVALID_SYMBOL')
         ]
 
         with self.assertLogs(project_logger(), level='INFO') as cm:
-            rv = self.client.get_conids(queries, default_filtering=False)
+            rv = self.client.stock_conid_by_symbol(queries, default_filtering=False)
 
         for symbol, conid in rv.data.items():
             self.assertIn(symbol, ibkr_responses.responses['filtered_conids'])
             self.assertEqual(conid, ibkr_responses.responses['filtered_conids'][symbol])
 
     def test_get_conids_exception(self, requests_mock):
         requests_mock.request.return_value = self.response
@@ -70,42 +70,42 @@
 
         symbol = 'AAPL'
         query = StockQuery(symbol=symbol, contract_conditions={'isUS': False}, name_match='APPLE')
 
         instruments = filter_stocks(query, Result(data={symbol: ibkr_responses.responses["stocks"][symbol]}), default_filtering=False).data[symbol]
 
         with self.assertRaises(RuntimeError) as cm_err:
-            rv = self.client.get_conids(query, default_filtering=False)
+            rv = self.client.stock_conid_by_symbol(query, default_filtering=False)
 
         self.maxDiff = None
         self.assertEqual(
             f'Filtering stock "{symbol}" returned 2 instruments and 2 contracts using following query: {query}.\nPlease use filters to ensure that only one instrument and one contract per symbol is selected in order to avoid conid ambiguity.\nBe aware that contracts are filtered as {{"isUS": True}} by default. Set default_filtering=False to prevent this default filtering or specify custom filters. See inline documentation for more details.\nInstruments returned:\n{pformat(instruments)}',
             str(cm_err.exception))
 
 
     def test_get_live_orders_no_filters(self, requests_mock):
         self.client.get = MagicMock(return_value=self.result)
-        self.client.get_live_orders()
+        self.client.live_orders()
         self.client.get.assert_called_with('iserver/account/orders', params=None)
 
     def test_get_live_orders_with_valid_filters(self, requests_mock):
         self.client.get = MagicMock(return_value=self.result)
         filters = ['inactive', 'filled']
-        self.client.get_live_orders(filters=filters)
+        self.client.live_orders(filters=filters)
         self.client.get.assert_called_with('iserver/account/orders', params={'filters': 'inactive,filled'})
 
     def test_get_live_orders_with_single_filter(self, requests_mock):
         self.client.get = MagicMock(return_value=self.result)
-        self.client.get_live_orders(filters='submitted')
+        self.client.live_orders(filters='submitted')
         self.client.get.assert_called_with('iserver/account/orders', params={'filters': 'submitted'})
 
     def test_get_live_orders_with_incorrect_filter_type(self, requests_mock):
         self.client.get = MagicMock(return_value=self.result)
         with self.assertRaises(TypeError):
-            self.client.get_live_orders(filters=123)  # Non-list, non-string filter
+            self.client.live_orders(filters=123)  # Non-list, non-string filter
         self.client.get.assert_not_called()
 
 
     def _marketdata_request(self, method, url, *args, **kwargs):
         leaf = url.split('/')[-1]
         if leaf == 'stocks':
             return MagicMock(json=lambda: ibkr_responses.responses['stocks'])  # Mock response for get_conids
@@ -280,12 +280,12 @@
 
     def test_marketdata_unsubscribe_raises_exception_on_failure(self, requests_mock):
         conids = [12345]
         responses = {
             12345: MagicMock(status_code=500),  # Simulate server error
         }
         requests_mock.request.side_effect = lambda method, url, **kwargs: responses[int(url.split('/')[-2])]
-        self.client.get = MagicMock(side_effect=lambda url, *args, **kwargs: ExternalBrokerError(status_code=500), __name__='client_get_mock')
+        self.client.post = MagicMock(side_effect=lambda url, *args, **kwargs: ExternalBrokerError(status_code=500), __name__='client_get_mock')
 
         with self.assertRaises(ExternalBrokerError):
             self.client.marketdata_unsubscribe(conids)
```

### Comparing `ibind-0.0.1/test/integration/client/test_ibkr_utils_i.py` & `ibind-0.0.2/test/integration/client/test_ibkr_utils_i.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.1/test/integration/client/test_ibkr_ws_client_i.py` & `ibind-0.0.2/test/integration/client/test_ibkr_ws_client_i.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,15 +216,15 @@
         queue = self.ws_client.new_queue_accessor(IbkrWsKey.MARKET_DATA)
         full_channel = f'{queue.key.channel}+{self.conid}'
         request = {'channel': f'{full_channel}', 'data': {"fields": ['55', '71', '84', '86', '88', '85', '87', '7295', '7296', '70']}}
         response = {'topic': f's{full_channel}', 'conid': self.conid, '_updated': self.update_time, 55: 'AAPL', 70: '195.34', 71: '193.67', 87: '24.2M', 7295: '194.10', 84: '195.25', 86: '195.26', 88: '3,500', 85: '500', 6508: '&serviceID1=122&serviceID2=123&serviceID3=203&serviceID4=775&serviceID5=204&serviceID6=206&serviceID7=108&serviceID8=109'}
 
         self.assertTrue(queue.empty(), 'Queue should be empty')
 
-        with patch.object(self.ws_client._subscription_controller, 'has_subscription', return_value=True):
+        with patch.object(self.ws_client, 'has_subscription', return_value=True):
             cm, success = self._subscribe(request, response)
             self.assertTrue(success)
 
         self.assertEqual(self._logs_subscriptions(full_channel, request["data"]), [r.msg for r in cm.records])
 
         self.assertEqual({self.conid: {'_updated': self.update_time, 'conid': self.conid, 'topic': f'smd+{self.conid}', 'ask_price': '195.26', 'ask_size': '500', 'bid_price': '195.25', 'bid_size': '3,500', 'high': '195.34', 'low': '193.67', 'open': '194.10', 'service_params': '&serviceID1=122&serviceID2=123&serviceID3=203&serviceID4=775&serviceID5=204&serviceID6=206&serviceID7=108&serviceID8=109', 'symbol': 'AAPL', 'volume': '24.2M'}}, queue.get())
 
@@ -233,15 +233,15 @@
         server_id = 87567
         full_channel = f'{queue.key.channel}+{self.conid}'
         request = {'channel': f'{full_channel}', 'data': {"period": '1min', "bar": "1min", "outsideRTH": True, "source": "trades", "format": "%o/%c/%h/%l"}}
         response = {'topic': f's{full_channel}', 'serverId': server_id, '_updated': self.update_time, 'conid': self.conid, 'foo': 'bar'}
 
         self.assertTrue(queue.empty(), 'Queue should be empty')
 
-        with patch.object(self.ws_client._subscription_controller, 'has_subscription', return_value=True):
+        with patch.object(self.ws_client, 'has_subscription', return_value=True):
             cm, success = self._subscribe(request, response)
             self.assertTrue(success)
 
         self.assertEqual(self._logs_subscriptions(full_channel, request["data"]), [r.msg for r in cm.records])
 
         self.assertEqual(response, queue.get())
         self.assertIn(server_id, self.ws_client.server_ids(IbkrWsKey.MARKET_HISTORY))
@@ -250,48 +250,48 @@
         queue = self.ws_client.new_queue_accessor(IbkrWsKey.TRADES)
         full_channel = f'{queue.key.channel}+{self.conid}'
         request = {'channel': f'{full_channel}'}
         response = {'topic': f's{full_channel}', '_updated': self.update_time, 'conid': self.conid, 'args': [{'foo': 'bar'}]}
 
         self.assertTrue(queue.empty(), 'Queue should be empty')
 
-        with patch.object(self.ws_client._subscription_controller, 'has_subscription', return_value=True):
+        with patch.object(self.ws_client, 'has_subscription', return_value=True):
             cm, success = self._subscribe(request, response)
             self.assertTrue(success)
 
         self.assertEqual(self._logs_subscriptions(full_channel), [r.msg for r in cm.records])
-        self.assertEqual(response['args'], queue.get())
+        self.assertEqual(response, queue.get())
 
     def test_on_message_orders_channel_handling(self):
         queue = self.ws_client.new_queue_accessor(IbkrWsKey.ORDERS)
 
         full_channel = f'{queue.key.channel}+{self.conid}'
         request = {'channel': f'{full_channel}'}
         response = {'topic': f's{full_channel}', '_updated': self.update_time, 'conid': self.conid, 'args': [{'foo': 'bar'}]}
 
         self.assertTrue(queue.empty(), 'Queue should be empty')
 
-        with patch.object(self.ws_client._subscription_controller, 'has_subscription', return_value=True):
+        with patch.object(self.ws_client, 'has_subscription', return_value=True):
             cm, success = self._subscribe(request, response)
             self.assertTrue(success)
 
         self.assertEqual(self._logs_subscriptions(full_channel), [r.msg for r in cm.records])
-        self.assertEqual(response['args'], queue.get())
+        self.assertEqual(response, queue.get())
 
     def test_subscription_without_confirmation(self):
         channel = 'fake'
         full_channel = f'{channel}+{self.conid}'
         request = {'channel': f'{full_channel}', 'needs_confirmation': False}
         response = None
 
         expected_errors = [
             f'IbkrWsClient: Channel subscription timeout: s{full_channel} after {self.subscription_retries} attempts.'
         ]
 
-        with patch.object(self.ws_client._subscription_controller, 'has_subscription', return_value=True):
+        with patch.object(self.ws_client, 'has_subscription', return_value=True):
             cm, success = self._subscribe(request, response, expected_errors=expected_errors)
             self.assertTrue(success)
 
         self.assertEqual([f'IbkrWsClient: Subscribed: s{full_channel} without confirmation.',
                           f'IbkrWsClient: Unsubscribed: u{full_channel}+{{}} without confirmation.'], [r.msg for r in cm.records])
 
     def test_check_health(self):
```

### Comparing `ibind-0.0.1/test/test_utils.py` & `ibind-0.0.2/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `ibind-0.0.1/test/unit/support/test_py_utils_u.py` & `ibind-0.0.2/test/unit/support/test_py_utils_u.py`

 * *Files identical despite different names*

