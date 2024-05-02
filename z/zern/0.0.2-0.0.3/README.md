# Comparing `tmp/zern-0.0.2.tar.gz` & `tmp/zern-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zern-0.0.2.tar", last modified: Thu May  2 18:46:04 2024, max compression
+gzip compressed data, was "zern-0.0.3.tar", last modified: Thu May  2 19:29:41 2024, max compression
```

## Comparing `zern-0.0.2.tar` & `zern-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 18:46:04.228110 zern-0.0.2/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     1071 2024-05-02 15:26:31.000000 zern-0.0.2/LICENSE
--rw-r--r--   0 harsha    (1000) harsha    (1000)     6270 2024-05-02 18:46:04.228110 zern-0.0.2/PKG-INFO
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     5716 2024-05-02 15:26:53.000000 zern-0.0.2/README.md
--rw-rw-r--   0 harsha    (1000) harsha    (1000)      623 2024-05-02 18:45:17.000000 zern-0.0.2/pyproject.toml
--rw-rw-r--   0 harsha    (1000) harsha    (1000)       38 2024-05-02 18:46:04.228110 zern-0.0.2/setup.cfg
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 18:46:04.224110 zern-0.0.2/src/
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 18:46:04.224110 zern-0.0.2/src/zern/
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 18:46:04.228110 zern-0.0.2/src/zern/Core/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     3798 2024-05-02 06:23:51.000000 zern-0.0.2/src/zern/Core/session.py
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     4638 2024-05-02 06:32:36.000000 zern-0.0.2/src/zern/Core/trader.py
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 18:46:04.228110 zern-0.0.2/src/zern/Core/websocket/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     3534 2024-05-02 07:34:58.000000 zern-0.0.2/src/zern/Core/websocket/ticker.py
--rw-rw-r--   0 harsha    (1000) harsha    (1000)       61 2024-04-24 18:27:30.000000 zern-0.0.2/src/zern/__init__.py
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 18:46:04.228110 zern-0.0.2/src/zern/utils/
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     1861 2024-04-21 19:33:12.000000 zern-0.0.2/src/zern/utils/OrderedList.py
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     2280 2024-05-02 05:29:49.000000 zern-0.0.2/src/zern/utils/Types.py
--rw-rw-r--   0 harsha    (1000) harsha    (1000)     6314 2024-05-02 05:36:04.000000 zern-0.0.2/src/zern/utils/parsing.py
-drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 18:46:04.228110 zern-0.0.2/src/zern.egg-info/
--rw-r--r--   0 harsha    (1000) harsha    (1000)     6270 2024-05-02 18:46:04.000000 zern-0.0.2/src/zern.egg-info/PKG-INFO
--rw-rw-r--   0 harsha    (1000) harsha    (1000)      344 2024-05-02 18:46:04.000000 zern-0.0.2/src/zern.egg-info/SOURCES.txt
--rw-rw-r--   0 harsha    (1000) harsha    (1000)        1 2024-05-02 18:46:04.000000 zern-0.0.2/src/zern.egg-info/dependency_links.txt
--rw-rw-r--   0 harsha    (1000) harsha    (1000)        5 2024-05-02 18:46:04.000000 zern-0.0.2/src/zern.egg-info/top_level.txt
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:29:41.785089 zern-0.0.3/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     1071 2024-05-02 15:26:31.000000 zern-0.0.3/LICENSE
+-rw-r--r--   0 harsha    (1000) harsha    (1000)     6270 2024-05-02 19:29:41.785089 zern-0.0.3/PKG-INFO
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     5716 2024-05-02 15:26:53.000000 zern-0.0.3/README.md
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)      707 2024-05-02 19:11:35.000000 zern-0.0.3/pyproject.toml
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)       38 2024-05-02 19:29:41.785089 zern-0.0.3/setup.cfg
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:29:41.785089 zern-0.0.3/src/
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:29:41.785089 zern-0.0.3/src/zern/
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:29:41.785089 zern-0.0.3/src/zern/Core/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     3798 2024-05-02 06:23:51.000000 zern-0.0.3/src/zern/Core/session.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     4646 2024-05-02 19:27:04.000000 zern-0.0.3/src/zern/Core/trader.py
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:29:41.785089 zern-0.0.3/src/zern/Core/websocket_connection/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     3534 2024-05-02 07:34:58.000000 zern-0.0.3/src/zern/Core/websocket_connection/ticker.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)       61 2024-04-24 18:27:30.000000 zern-0.0.3/src/zern/__init__.py
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:29:41.785089 zern-0.0.3/src/zern/utils/
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     1861 2024-04-21 19:33:12.000000 zern-0.0.3/src/zern/utils/OrderedList.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     2280 2024-05-02 05:29:49.000000 zern-0.0.3/src/zern/utils/Types.py
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)     6314 2024-05-02 05:36:04.000000 zern-0.0.3/src/zern/utils/parsing.py
+drwxrwxr-x   0 harsha    (1000) harsha    (1000)        0 2024-05-02 19:29:41.785089 zern-0.0.3/src/zern.egg-info/
+-rw-r--r--   0 harsha    (1000) harsha    (1000)     6270 2024-05-02 19:29:41.000000 zern-0.0.3/src/zern.egg-info/PKG-INFO
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)      355 2024-05-02 19:29:41.000000 zern-0.0.3/src/zern.egg-info/SOURCES.txt
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)        1 2024-05-02 19:29:41.000000 zern-0.0.3/src/zern.egg-info/dependency_links.txt
+-rw-rw-r--   0 harsha    (1000) harsha    (1000)        5 2024-05-02 19:29:41.000000 zern-0.0.3/src/zern.egg-info/top_level.txt
```

### Comparing `zern-0.0.2/LICENSE` & `zern-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zern-0.0.2/PKG-INFO` & `zern-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zern
-Version: 0.0.2
+Version: 0.0.3
 Summary: An unofficial client library using Zerodha web api for live data and historical data
 Author-email: Harsha Avapati <harshaavapati@gmail.com>
 Project-URL: Homepage, https://github.com/ExBlacklight/Zern
 Project-URL: Issues, https://github.com/ExBlacklight/Zern/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `zern-0.0.2/README.md` & `zern-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `zern-0.0.2/pyproject.toml` & `zern-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zern"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Harsha Avapati", email="harshaavapati@gmail.com" },
 ]
 description = "An unofficial client library using Zerodha web api for live data and historical data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/ExBlacklight/Zern"
-Issues = "https://github.com/ExBlacklight/Zern/issues"
+Issues = "https://github.com/ExBlacklight/Zern/issues"
+
+[options]
+install_requires = [
+    "websocket-client>=1.8.0",
+    "pyotp>=2.9.0"
+]
```

### Comparing `zern-0.0.2/src/zern/Core/session.py` & `zern-0.0.3/src/zern/Core/session.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.2/src/zern/Core/trader.py` & `zern-0.0.3/src/zern/Core/trader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 
 from zern.Core.session import Session
 from datetime import datetime,date,time,timedelta
 from zern.utils.OrderedList import OrderedList
-from zern.Core.websocket.ticker import Ticker
+from zern.Core.websocket_connection.ticker import Ticker
 from zern.utils.Types import PRODUCT,VARIETY,TRANSACTION_TYPE,ORDER_TYPE,VALIDITY,EXCHANGE
 
 
 class Trader:
     def __init__(self,user_name,password,totp_key) -> None:
         '''
         This Trader is the way to start the Process, the param cred_dict requires ["user_name","password","totp_key"]
 
         The "totp_key" can be extracted when creating the two factor authentication in the kite app, click on the QR code and use the same key.
         '''
         self.session = Session(user_name,password,totp_key)
         self.instruments = self.session.instruments
-        self.startTicker()
         self.ticker = None
+        self.startTicker()
     
     def format_date(self,value):
         if isinstance(value,str):
             return value
         elif isinstance(value,datetime):
             return str(value.date())
         elif isinstance(value,date):
@@ -90,15 +90,15 @@
             'trailing_stoploss': trailing_stoploss,
             'user_id': self.session.user_name
         }
         url = 'https://kite.zerodha.com/oms/orders/regular'
         return self.session.request(url=url,method=Session.TYPE_POST,data=payload)['data']
 
     def startTicker(self):
-        self.ticker_ws = Ticker(session=self.session)
+        self.ticker = Ticker(session=self.session)
     
     def get_bnf_expiries(self):
         return list(self.instruments['derivatives']['BANKNIFTY']['derivatives'].keys())
 
     def get_expiries(self,derivative_name):
         return list(self.instruments['derivatives'][derivative_name]['derivatives'].keys())
```

### Comparing `zern-0.0.2/src/zern/Core/websocket/ticker.py` & `zern-0.0.3/src/zern/Core/websocket_connection/ticker.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.2/src/zern/utils/OrderedList.py` & `zern-0.0.3/src/zern/utils/OrderedList.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.2/src/zern/utils/Types.py` & `zern-0.0.3/src/zern/utils/Types.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.2/src/zern/utils/parsing.py` & `zern-0.0.3/src/zern/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `zern-0.0.2/src/zern.egg-info/PKG-INFO` & `zern-0.0.3/src/zern.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zern
-Version: 0.0.2
+Version: 0.0.3
 Summary: An unofficial client library using Zerodha web api for live data and historical data
 Author-email: Harsha Avapati <harshaavapati@gmail.com>
 Project-URL: Homepage, https://github.com/ExBlacklight/Zern
 Project-URL: Issues, https://github.com/ExBlacklight/Zern/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

