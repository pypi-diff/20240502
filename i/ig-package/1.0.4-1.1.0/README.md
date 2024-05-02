# Comparing `tmp/ig_package-1.0.4.tar.gz` & `tmp/ig_package-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ig_package-1.0.4.tar", max compression
+gzip compressed data, was "ig_package-1.1.0.tar", max compression
```

## Comparing `ig_package-1.0.4.tar` & `ig_package-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1089 2024-04-03 23:27:00.840175 ig_package-1.0.4/LICENSE
--rw-r--r--   0        0        0      584 2024-04-08 21:58:11.934293 ig_package-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1971 2024-04-08 19:00:44.044419 ig_package-1.0.4/README.md
--rw-r--r--   0        0        0      158 2024-04-01 22:15:12.186529 ig_package-1.0.4/src/ig_package/__init__.py
--rw-r--r--   0        0        0    21049 2024-04-08 21:15:33.426345 ig_package-1.0.4/src/ig_package/main.py
--rw-r--r--   0        0        0     2471 1970-01-01 00:00:00.000000 ig_package-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-03 23:27:00.840175 ig_package-1.1.0/LICENSE
+-rw-r--r--   0        0        0      583 2024-05-02 15:14:26.376283 ig_package-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1971 2024-04-08 19:00:44.044419 ig_package-1.1.0/README.md
+-rw-r--r--   0        0        0      158 2024-04-01 22:15:12.186529 ig_package-1.1.0/src/ig_package/__init__.py
+-rw-r--r--   0        0        0    22166 2024-05-02 14:51:17.205879 ig_package-1.1.0/src/ig_package/main.py
+-rw-r--r--   0        0        0     2471 1970-01-01 00:00:00.000000 ig_package-1.1.0/PKG-INFO
```

### Comparing `ig_package-1.0.4/LICENSE` & `ig_package-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ig_package-1.0.4/pyproject.toml` & `ig_package-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ig-package"
-version = "v1.0.4"
+version = "1.1.0"
 description = "A package allowing easy interaction with IG Group's REST API."
 authors = ["hnewey7 <hnewey7@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `ig_package-1.0.4/README.md` & `ig_package-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ig_package-1.0.4/src/ig_package/main.py` & `ig_package-1.1.0/src/ig_package/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 import logging
 import os
 from pathlib import Path
 import time
 from datetime import datetime
 import pandas as pd
 
+from trading_ig import IGService, IGStreamService
+from IG_API_Details import config
+from trading_ig.streamer.manager import StreamingManager
+
 # - - - - - - - - - - - - - - - - - - - - -
 
 global logger
 logger = logging.getLogger()
 
 # - - - - - - - - - - - - - - - - - - - - -
 
@@ -114,14 +118,23 @@
     if response.ok:
       self.header["CST"] = response.headers["CST"]
       self.header["X-SECURITY-TOKEN"] = response.headers["X-SECURITY-TOKEN"]
       return True
     else:
       return False
 
+  def open_streaming_session(self) -> None:
+    """ Opening a streaming session through IG, allowing data to be collected in real time."""
+    # Opening IG service.
+    self.ig_service = IGService(config.username,config.password,config.api_key,config.acc_type,config.acc_number)
+    # Opening streaming service.
+    self.ig_streaming_service = IGStreamService(self.ig_service)
+    self.ig_streaming_service.create_session(version="3")
+    self.streaming_manager = StreamingManager(self.ig_streaming_service)
+
   def check_trading_session(self) -> bool:
     """ Checking if trading session active.
 
         Returns
         -------
         bool
           Boolean depending if trading session is open or not."""
@@ -483,15 +496,15 @@
       df = instrument.get_historical_prices(resolution=resolution,start=start,end=end)
       df_dict[instrument.name] = df
     return df_dict
 
 # - - - - - - - - - - - - - - - - - - - - -
     
 class Instrument():
-  """ Object representing a single instruement from IG API.
+  """ Object representing a single instrument from IG API.
         - Allows for collection of historical data."""
   
   def __init__(self,epic:str,IG_obj:IG) -> None:
     try:
       self.IG_obj = IG_obj
       # Adjusting header.
       self.IG_obj.header["Version"] = "1"
@@ -545,9 +558,19 @@
       datetime_obj = datetime.strptime(price["snapshotTime"],"%Y:%m:%d-%H:%M:%S")
       single_data = [datetime_obj,price["openPrice"]["bid"],price["highPrice"]["bid"],price["lowPrice"]["bid"],price["closePrice"]["bid"]]
       all_data.append(single_data)
     # Creating dataframe.
     df = pd.DataFrame(all_data, columns=['Datetime', 'Open', 'High', 'Low', 'Close'])
     df.set_index("Datetime",inplace=True)
     return df
+  
+  def start_live_data(self) -> None:
+    """ Starting the live data ticker throught the lightstreamer_client."""
+    # Checking if streaming session open.
+    if not hasattr(self.IG_obj, "lightstreamer_client"):
+      self.IG_obj.open_streaming_session()
+    # Creating subscription.
+    self.IG_obj.streaming_manager.start_tick_subscription(self.epic)
+    # Getting ticker.
+    self.ticker = self.IG_obj.streaming_manager.ticker(self.epic)
 
 # - - - - - - - - - - - - - - - - - - - - -
```

### Comparing `ig_package-1.0.4/PKG-INFO` & `ig_package-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ig-package
-Version: 1.0.4
+Version: 1.1.0
 Summary: A package allowing easy interaction with IG Group's REST API.
 License: MIT
 Author: hnewey7
 Author-email: hnewey7@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

