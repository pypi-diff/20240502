# Comparing `tmp/testplans-0.2.4.tar.gz` & `tmp/testplans-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testplans-0.2.4.tar", last modified: Fri Apr 26 14:32:31 2024, max compression
+gzip compressed data, was "testplans-0.2.5.tar", last modified: Thu May  2 09:22:33 2024, max compression
```

## Comparing `testplans-0.2.4.tar` & `testplans-0.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 14:32:31.287482 testplans-0.2.4/
--rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 testplans-0.2.4/LICENSE
--rw-rw-rw-   0        0        0     5494 2024-04-26 14:32:31.286482 testplans-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     4584 2024-04-26 14:30:50.000000 testplans-0.2.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-26 14:32:31.288580 testplans-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 testplans-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-26 14:32:31.281335 testplans-0.2.4/testplans/
--rw-rw-rw-   0        0        0      105 2024-02-01 12:13:36.000000 testplans-0.2.4/testplans/__init__.py
--rw-rw-rw-   0        0        0      776 2024-03-15 14:57:12.000000 testplans-0.2.4/testplans/_results.py
--rw-rw-rw-   0        0        0     3974 2024-04-26 14:17:18.000000 testplans-0.2.4/testplans/api.py
--rw-rw-rw-   0        0        0     7686 2024-04-22 13:45:33.000000 testplans-0.2.4/testplans/devices.py
--rw-rw-rw-   0        0        0     6347 2024-04-22 14:33:47.000000 testplans-0.2.4/testplans/gui.py
--rw-rw-rw-   0        0        0    10804 2024-04-26 14:30:27.000000 testplans-0.2.4/testplans/main.py
--rw-rw-rw-   0        0        0     1561 2024-04-22 14:50:31.000000 testplans-0.2.4/testplans/models.py
--rw-rw-rw-   0        0        0    11272 2024-04-26 14:26:56.000000 testplans-0.2.4/testplans/tc.py
--rw-rw-rw-   0        0        0     8975 2024-04-26 12:19:02.000000 testplans-0.2.4/testplans/tm.py
-drwxrwxrwx   0        0        0        0 2024-04-26 14:32:31.286482 testplans-0.2.4/testplans.egg-info/
--rw-rw-rw-   0        0        0     5494 2024-04-26 14:32:31.000000 testplans-0.2.4/testplans.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-04-26 14:32:31.000000 testplans-0.2.4/testplans.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 14:32:31.000000 testplans-0.2.4/testplans.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-26 14:32:31.000000 testplans-0.2.4/testplans.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 09:22:33.565242 testplans-0.2.5/
+-rw-rw-rw-   0        0        0     1082 2023-11-27 14:37:20.000000 testplans-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0     5494 2024-05-02 09:22:33.565242 testplans-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4584 2024-05-02 09:11:40.000000 testplans-0.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-02 09:22:33.566257 testplans-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 testplans-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 09:22:33.559001 testplans-0.2.5/testplans/
+-rw-rw-rw-   0        0        0      105 2024-02-01 12:13:36.000000 testplans-0.2.5/testplans/__init__.py
+-rw-rw-rw-   0        0        0      776 2024-03-15 14:57:12.000000 testplans-0.2.5/testplans/_results.py
+-rw-rw-rw-   0        0        0     3974 2024-04-26 14:17:18.000000 testplans-0.2.5/testplans/api.py
+-rw-rw-rw-   0        0        0     7686 2024-04-22 13:45:33.000000 testplans-0.2.5/testplans/devices.py
+-rw-rw-rw-   0        0        0     6347 2024-04-22 14:33:47.000000 testplans-0.2.5/testplans/gui.py
+-rw-rw-rw-   0        0        0    11798 2024-05-02 09:05:20.000000 testplans-0.2.5/testplans/main.py
+-rw-rw-rw-   0        0        0     1561 2024-04-22 14:50:31.000000 testplans-0.2.5/testplans/models.py
+-rw-rw-rw-   0        0        0    11272 2024-04-26 14:26:56.000000 testplans-0.2.5/testplans/tc.py
+-rw-rw-rw-   0        0        0     8975 2024-04-26 12:19:02.000000 testplans-0.2.5/testplans/tm.py
+drwxrwxrwx   0        0        0        0 2024-05-02 09:22:33.564038 testplans-0.2.5/testplans.egg-info/
+-rw-rw-rw-   0        0        0     5494 2024-05-02 09:22:33.000000 testplans-0.2.5/testplans.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-05-02 09:22:33.000000 testplans-0.2.5/testplans.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 09:22:33.000000 testplans-0.2.5/testplans.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-02 09:22:33.000000 testplans-0.2.5/testplans.egg-info/top_level.txt
```

### Comparing `testplans-0.2.4/LICENSE` & `testplans-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `testplans-0.2.4/PKG-INFO` & `testplans-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testplans
-Version: 0.2.4
+Version: 0.2.5
 Summary: simple testplan framework for several DUTs
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/testplans
 Keywords: testplan,testplan structure framework,testplan gui,testplan multy dut,testplan several dut
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# testplans (v0.2.4)
+# testplans (v0.2.5)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

### Comparing `testplans-0.2.4/README.md` & `testplans-0.2.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# testplans (v0.2.4)
+# testplans (v0.2.5)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

### Comparing `testplans-0.2.4/setup.py` & `testplans-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.4/testplans/_results.py` & `testplans-0.2.5/testplans/_results.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.4/testplans/api.py` & `testplans-0.2.5/testplans/api.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.4/testplans/devices.py` & `testplans-0.2.5/testplans/devices.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.4/testplans/gui.py` & `testplans-0.2.5/testplans/gui.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.4/testplans/main.py` & `testplans-0.2.5/testplans/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pathlib import Path
 from PyQt5.QtCore import QThread
 from importlib import import_module
 import asyncio
 from pydantic import BaseModel
 
 from pyqt_templates import *
-from server_templates import ServerAiohttpBase, Client_RequestItem, Client_RequestsStack
+from server_templates import ServerAiohttpBase, Client_RequestItem, Client_RequestsStack, ServerFastApi_Thread
 from object_info import ObjectInfo
 from private_values import PrivateJson
 
 from logger_aux import Logger
 
 
 # =====================================================================================================================
@@ -43,14 +43,16 @@
     signal__tp_start = pyqtSignal()
     signal__tp_stop = pyqtSignal()
     signal__tp_finished = pyqtSignal()
 
     _signal__tp_reset_duts_sn = pyqtSignal()
 
     # SETTINGS ------------------------------------------------------
+    START__GUI_AND_API: bool = True
+
     STAND_NAME: Optional[str] = "stand_id__1"
     STAND_DESCRIPTION: Optional[str] = "stand_description"
     STAND_SN: Optional[str] = "StandSn"
 
     API_SERVER__START: bool = True
     API_SERVER__CLS: Type[TpApi_FastApi] = TpApi_FastApi
     api_server: TpApi_FastApi
@@ -97,30 +99,35 @@
             raise Exx__TcsPathNotExists(msg)
 
         self.DEVICES__CLS.generate__devices()
 
         self.tcs__reinit()
         self.slots_connect()
 
-        self.api_server = self.API_SERVER__CLS(data=self)
+        if self.START__GUI_AND_API:
+            self.start__gui_and_api()
+
+    def start__gui_and_api(self) -> None:
         if self.API_SERVER__START:
             self.LOGGER.debug("starting api server")
+            self.api_server = self.API_SERVER__CLS(data=self)
             self.api_server.start()
 
+        # last execution --------------------------------------
         if self.GUI__START:
             self.LOGGER.debug("starting gui")
             self.gui = self.GUI__CLS(self)
 
             # this will BLOCK process
             # this will BLOCK process
             # this will BLOCK process
             # this will BLOCK process
             # this will BLOCK process
             self.gui.run()
-        else:
+        elif self.API_SERVER__START:
             self.api_server.wait()  # it is ok!!!
 
     def slots_connect(self) -> None:
         self.signal__tp_start.connect(self.start)
         self.signal__tp_stop.connect(self.terminate)
         self._signal__tp_reset_duts_sn.connect(self.DEVICES__CLS._debug__duts__reset_sn)
 
@@ -299,7 +306,27 @@
             "STAND_DESCRIPTION": self.STAND_DESCRIPTION,
             **tc_inst.get__results().dict(),
         }
         self.api_client.send(body=body)
 
 
 # =====================================================================================================================
+class TpInsideApi_Runner(TpApi_FastApi):
+    """
+    REASON:
+    in windows TestCaseBase works fine by any variance GUI__START/API_SERVER__START
+    in Linux it is not good maybe cause of nesting theme=Thread+Async+Threads
+
+    so this is the attempt to execute correctly TP in Linux by deactivating GUI and using theme=Async+Threads
+    """
+    TP_CLS: Type[TpMultyDutBase] = TpMultyDutBase
+
+    def __init__(self, *args, **kwargs):
+
+        self.TP_CLS.START__GUI_AND_API = False
+        self.data = self.TP_CLS()
+
+        super().__init__(*args, **kwargs)
+        self.run()
+
+
+# =====================================================================================================================
```

### Comparing `testplans-0.2.4/testplans/models.py` & `testplans-0.2.5/testplans/models.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.4/testplans/tc.py` & `testplans-0.2.5/testplans/tc.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.4/testplans/tm.py` & `testplans-0.2.5/testplans/tm.py`

 * *Files identical despite different names*

### Comparing `testplans-0.2.4/testplans.egg-info/PKG-INFO` & `testplans-0.2.5/testplans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testplans
-Version: 0.2.4
+Version: 0.2.5
 Summary: simple testplan framework for several DUTs
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/testplans
 Keywords: testplan,testplan structure framework,testplan gui,testplan multy dut,testplan several dut
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# testplans (v0.2.4)
+# testplans (v0.2.5)
 
 ## DESCRIPTION_SHORT
 simple testplan framework for several DUTs
 
 ## DESCRIPTION_LONG
 designed to apply testplan for several DUTs
```

