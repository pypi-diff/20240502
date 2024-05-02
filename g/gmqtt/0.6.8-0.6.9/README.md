# Comparing `tmp/gmqtt-0.6.8.tar.gz` & `tmp/gmqtt-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gmqtt-0.6.8.tar", last modified: Tue Nov 17 07:11:55 2020, max compression
+gzip compressed data, was "dist/gmqtt-0.6.9.tar", last modified: Mon Nov 23 18:56:33 2020, max compression
```

## Comparing `gmqtt-0.6.8.tar` & `gmqtt-0.6.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 mitu     (33000) domain_users (30513)        0 2020-11-17 07:11:55.000000 gmqtt-0.6.8/
--rw-r--r--   0 mitu     (33000) domain_users (30513)     1837 2020-06-12 07:31:50.000000 gmqtt-0.6.8/setup.py
-drwxr-xr-x   0 mitu     (33000) domain_users (30513)        0 2020-11-17 07:11:55.000000 gmqtt-0.6.8/gmqtt/
--rw-r--r--   0 mitu     (33000) domain_users (30513)     1517 2019-05-21 09:23:34.000000 gmqtt-0.6.8/gmqtt/storage.py
--rw-r--r--   0 mitu     (33000) domain_users (30513)    12104 2020-11-17 07:11:54.000000 gmqtt-0.6.8/gmqtt/client.py
--rw-r--r--   0 mitu     (33000) domain_users (30513)      551 2020-11-17 07:11:54.000000 gmqtt-0.6.8/gmqtt/__init__.py
-drwxr-xr-x   0 mitu     (33000) domain_users (30513)        0 2020-11-17 07:11:55.000000 gmqtt-0.6.8/gmqtt/mqtt/
--rw-r--r--   0 mitu     (33000) domain_users (30513)     7809 2020-07-24 13:16:57.000000 gmqtt-0.6.8/gmqtt/mqtt/protocol.py
--rw-r--r--   0 mitu     (33000) domain_users (30513)     5280 2020-06-12 07:31:50.000000 gmqtt-0.6.8/gmqtt/mqtt/property.py
--rw-r--r--   0 mitu     (33000) domain_users (30513)     2818 2020-06-12 07:31:50.000000 gmqtt-0.6.8/gmqtt/mqtt/constants.py
--rw-r--r--   0 mitu     (33000) domain_users (30513)     4054 2020-07-24 13:16:57.000000 gmqtt-0.6.8/gmqtt/mqtt/connection.py
--rw-r--r--   0 mitu     (33000) domain_users (30513)        0 2019-07-10 13:12:34.000000 gmqtt-0.6.8/gmqtt/mqtt/__init__.py
--rw-r--r--   0 mitu     (33000) domain_users (30513)     2906 2019-10-30 07:25:27.000000 gmqtt-0.6.8/gmqtt/mqtt/utils.py
--rw-r--r--   0 mitu     (33000) domain_users (30513)    16704 2020-07-31 09:42:45.000000 gmqtt-0.6.8/gmqtt/mqtt/handler.py
--rw-r--r--   0 mitu     (33000) domain_users (30513)     8774 2020-11-17 07:11:54.000000 gmqtt-0.6.8/gmqtt/mqtt/package.py
--rw-r--r--   0 mitu     (33000) domain_users (30513)     1067 2019-05-21 09:23:34.000000 gmqtt-0.6.8/LICENSE
-drwxr-xr-x   0 mitu     (33000) domain_users (30513)        0 2020-11-17 07:11:55.000000 gmqtt-0.6.8/tests/
--rw-r--r--   0 mitu     (33000) domain_users (30513)        0 2019-05-21 09:23:34.000000 gmqtt-0.6.8/tests/__init__.py
--rw-r--r--   0 mitu     (33000) domain_users (30513)     2950 2020-06-12 07:31:50.000000 gmqtt-0.6.8/tests/utils.py
--rw-r--r--   0 mitu     (33000) domain_users (30513)    14763 2020-07-24 13:16:57.000000 gmqtt-0.6.8/tests/test_mqtt5.py
--rw-r--r--   0 mitu     (33000) domain_users (30513)       25 2019-05-21 09:23:34.000000 gmqtt-0.6.8/MANIFEST.in
--rw-r--r--   0 mitu     (33000) domain_users (30513)       38 2020-11-17 07:11:55.000000 gmqtt-0.6.8/setup.cfg
-drwxr-xr-x   0 mitu     (33000) domain_users (30513)        0 2020-11-17 07:11:55.000000 gmqtt-0.6.8/examples/
--rw-r--r--   0 mitu     (33000) domain_users (30513)        0 2019-05-21 09:23:34.000000 gmqtt-0.6.8/examples/__init__.py
--rw-r--r--   0 mitu     (33000) domain_users (30513)     2791 2020-06-12 07:31:50.000000 gmqtt-0.6.8/examples/shared_subscriptions.py
--rw-r--r--   0 mitu     (33000) domain_users (30513)     2265 2020-06-12 07:31:50.000000 gmqtt-0.6.8/examples/will_message.py
--rw-r--r--   0 mitu     (33000) domain_users (30513)     3395 2020-06-12 07:31:50.000000 gmqtt-0.6.8/examples/properties.py
-drwxr-xr-x   0 mitu     (33000) domain_users (30513)        0 2020-11-17 07:11:55.000000 gmqtt-0.6.8/gmqtt.egg-info/
--rw-r--r--   0 mitu     (33000) domain_users (30513)        6 2020-11-17 07:11:55.000000 gmqtt-0.6.8/gmqtt.egg-info/top_level.txt
--rw-r--r--   0 mitu     (33000) domain_users (30513)        1 2020-11-17 07:11:55.000000 gmqtt-0.6.8/gmqtt.egg-info/dependency_links.txt
--rw-r--r--   0 mitu     (33000) domain_users (30513)        1 2018-02-19 09:04:05.000000 gmqtt-0.6.8/gmqtt.egg-info/zip-safe
--rw-r--r--   0 mitu     (33000) domain_users (30513)      203 2020-11-17 07:11:55.000000 gmqtt-0.6.8/gmqtt.egg-info/requires.txt
--rw-r--r--   0 mitu     (33000) domain_users (30513)      594 2020-11-17 07:11:55.000000 gmqtt-0.6.8/gmqtt.egg-info/SOURCES.txt
--rw-r--r--   0 mitu     (33000) domain_users (30513)     9198 2020-11-17 07:11:55.000000 gmqtt-0.6.8/gmqtt.egg-info/PKG-INFO
--rw-r--r--   0 mitu     (33000) domain_users (30513)     9198 2020-11-17 07:11:55.000000 gmqtt-0.6.8/PKG-INFO
--rw-r--r--   0 mitu     (33000) domain_users (30513)     7070 2020-06-12 07:31:50.000000 gmqtt-0.6.8/README.md
+drwxr-xr-x   0 mitu     (33000) domain_users (30513)        0 2020-11-23 18:56:33.000000 gmqtt-0.6.9/
+-rw-r--r--   0 mitu     (33000) domain_users (30513)     1837 2020-06-12 07:31:50.000000 gmqtt-0.6.9/setup.py
+drwxr-xr-x   0 mitu     (33000) domain_users (30513)        0 2020-11-23 18:56:33.000000 gmqtt-0.6.9/gmqtt/
+-rw-r--r--   0 mitu     (33000) domain_users (30513)     1517 2019-05-21 09:23:34.000000 gmqtt-0.6.9/gmqtt/storage.py
+-rw-r--r--   0 mitu     (33000) domain_users (30513)    12238 2020-11-23 18:56:27.000000 gmqtt-0.6.9/gmqtt/client.py
+-rw-r--r--   0 mitu     (33000) domain_users (30513)      551 2020-11-23 18:56:27.000000 gmqtt-0.6.9/gmqtt/__init__.py
+drwxr-xr-x   0 mitu     (33000) domain_users (30513)        0 2020-11-23 18:56:33.000000 gmqtt-0.6.9/gmqtt/mqtt/
+-rw-r--r--   0 mitu     (33000) domain_users (30513)     7809 2020-07-24 13:16:57.000000 gmqtt-0.6.9/gmqtt/mqtt/protocol.py
+-rw-r--r--   0 mitu     (33000) domain_users (30513)     5280 2020-06-12 07:31:50.000000 gmqtt-0.6.9/gmqtt/mqtt/property.py
+-rw-r--r--   0 mitu     (33000) domain_users (30513)     2818 2020-06-12 07:31:50.000000 gmqtt-0.6.9/gmqtt/mqtt/constants.py
+-rw-r--r--   0 mitu     (33000) domain_users (30513)     4054 2020-07-24 13:16:57.000000 gmqtt-0.6.9/gmqtt/mqtt/connection.py
+-rw-r--r--   0 mitu     (33000) domain_users (30513)        0 2019-07-10 13:12:34.000000 gmqtt-0.6.9/gmqtt/mqtt/__init__.py
+-rw-r--r--   0 mitu     (33000) domain_users (30513)     2906 2019-10-30 07:25:27.000000 gmqtt-0.6.9/gmqtt/mqtt/utils.py
+-rw-r--r--   0 mitu     (33000) domain_users (30513)    16704 2020-07-31 09:42:45.000000 gmqtt-0.6.9/gmqtt/mqtt/handler.py
+-rw-r--r--   0 mitu     (33000) domain_users (30513)     8774 2020-11-17 07:11:54.000000 gmqtt-0.6.9/gmqtt/mqtt/package.py
+-rw-r--r--   0 mitu     (33000) domain_users (30513)     1067 2019-05-21 09:23:34.000000 gmqtt-0.6.9/LICENSE
+drwxr-xr-x   0 mitu     (33000) domain_users (30513)        0 2020-11-23 18:56:33.000000 gmqtt-0.6.9/tests/
+-rw-r--r--   0 mitu     (33000) domain_users (30513)        0 2019-05-21 09:23:34.000000 gmqtt-0.6.9/tests/__init__.py
+-rw-r--r--   0 mitu     (33000) domain_users (30513)     2950 2020-06-12 07:31:50.000000 gmqtt-0.6.9/tests/utils.py
+-rw-r--r--   0 mitu     (33000) domain_users (30513)    15467 2020-11-23 18:56:27.000000 gmqtt-0.6.9/tests/test_mqtt5.py
+-rw-r--r--   0 mitu     (33000) domain_users (30513)       25 2019-05-21 09:23:34.000000 gmqtt-0.6.9/MANIFEST.in
+-rw-r--r--   0 mitu     (33000) domain_users (30513)       38 2020-11-23 18:56:33.000000 gmqtt-0.6.9/setup.cfg
+drwxr-xr-x   0 mitu     (33000) domain_users (30513)        0 2020-11-23 18:56:33.000000 gmqtt-0.6.9/examples/
+-rw-r--r--   0 mitu     (33000) domain_users (30513)        0 2019-05-21 09:23:34.000000 gmqtt-0.6.9/examples/__init__.py
+-rw-r--r--   0 mitu     (33000) domain_users (30513)     2791 2020-06-12 07:31:50.000000 gmqtt-0.6.9/examples/shared_subscriptions.py
+-rw-r--r--   0 mitu     (33000) domain_users (30513)     2265 2020-06-12 07:31:50.000000 gmqtt-0.6.9/examples/will_message.py
+-rw-r--r--   0 mitu     (33000) domain_users (30513)     3395 2020-06-12 07:31:50.000000 gmqtt-0.6.9/examples/properties.py
+drwxr-xr-x   0 mitu     (33000) domain_users (30513)        0 2020-11-23 18:56:33.000000 gmqtt-0.6.9/gmqtt.egg-info/
+-rw-r--r--   0 mitu     (33000) domain_users (30513)        6 2020-11-23 18:56:33.000000 gmqtt-0.6.9/gmqtt.egg-info/top_level.txt
+-rw-r--r--   0 mitu     (33000) domain_users (30513)        1 2020-11-23 18:56:33.000000 gmqtt-0.6.9/gmqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 mitu     (33000) domain_users (30513)        1 2018-02-19 09:04:05.000000 gmqtt-0.6.9/gmqtt.egg-info/zip-safe
+-rw-r--r--   0 mitu     (33000) domain_users (30513)      203 2020-11-23 18:56:33.000000 gmqtt-0.6.9/gmqtt.egg-info/requires.txt
+-rw-r--r--   0 mitu     (33000) domain_users (30513)      594 2020-11-23 18:56:33.000000 gmqtt-0.6.9/gmqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 mitu     (33000) domain_users (30513)     9198 2020-11-23 18:56:33.000000 gmqtt-0.6.9/gmqtt.egg-info/PKG-INFO
+-rw-r--r--   0 mitu     (33000) domain_users (30513)     9198 2020-11-23 18:56:33.000000 gmqtt-0.6.9/PKG-INFO
+-rw-r--r--   0 mitu     (33000) domain_users (30513)     7070 2020-06-12 07:31:50.000000 gmqtt-0.6.9/README.md
```

### Comparing `gmqtt-0.6.8/setup.py` & `gmqtt-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `gmqtt-0.6.8/gmqtt/storage.py` & `gmqtt-0.6.9/gmqtt/storage.py`

 * *Files identical despite different names*

### Comparing `gmqtt-0.6.8/gmqtt/client.py` & `gmqtt-0.6.9/gmqtt/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,18 @@
         return False
 
     async def reconnect(self, delay=False):
         if not self._allow_reconnect():
             return
         # stopping auto-reconnects during reconnect procedure is important, better do not touch :(
         self._temporatily_stop_reconnect()
-        await self._disconnect()
+        try:
+            await self._disconnect()
+        except:
+            logger.info('[RECONNECT] ignored error while disconnecting, trying to reconnect anyway')
         if delay:
             await asyncio.sleep(self._config['reconnect_delay'])
         try:
             self._connection = await self._create_connection(self._host, self._port, ssl=self._ssl,
                                                              clean_session=False, keepalive=self._keepalive)
         except OSError as exc:
             self.failed_connections += 1
```

### Comparing `gmqtt-0.6.8/gmqtt/__init__.py` & `gmqtt-0.6.9/gmqtt/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 __email__ = 'mitu@gurtam.com'
 __copyright__ = ("Copyright 2013-%d, Gurtam; " % datetime.datetime.now().year,)
 
 __credits__ = [
     "Mikhail Turchunovich",
     "Elena Nikolaichik"
 ]
-__version__ = "0.6.8"
+__version__ = "0.6.9"
 
 
 __all__ = [
     'Client',
     'Message',
     'Subscription',
     'BaseMQTTProtocol',
```

### Comparing `gmqtt-0.6.8/gmqtt/mqtt/protocol.py` & `gmqtt-0.6.9/gmqtt/mqtt/protocol.py`

 * *Files identical despite different names*

### Comparing `gmqtt-0.6.8/gmqtt/mqtt/property.py` & `gmqtt-0.6.9/gmqtt/mqtt/property.py`

 * *Files identical despite different names*

### Comparing `gmqtt-0.6.8/gmqtt/mqtt/constants.py` & `gmqtt-0.6.9/gmqtt/mqtt/constants.py`

 * *Files identical despite different names*

### Comparing `gmqtt-0.6.8/gmqtt/mqtt/connection.py` & `gmqtt-0.6.9/gmqtt/mqtt/connection.py`

 * *Files identical despite different names*

### Comparing `gmqtt-0.6.8/gmqtt/mqtt/utils.py` & `gmqtt-0.6.9/gmqtt/mqtt/utils.py`

 * *Files identical despite different names*

### Comparing `gmqtt-0.6.8/gmqtt/mqtt/handler.py` & `gmqtt-0.6.9/gmqtt/mqtt/handler.py`

 * *Files identical despite different names*

### Comparing `gmqtt-0.6.8/gmqtt/mqtt/package.py` & `gmqtt-0.6.9/gmqtt/mqtt/package.py`

 * *Files identical despite different names*

### Comparing `gmqtt-0.6.8/LICENSE` & `gmqtt-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gmqtt-0.6.8/tests/utils.py` & `gmqtt-0.6.9/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gmqtt-0.6.8/tests/test_mqtt5.py` & `gmqtt-0.6.9/tests/test_mqtt5.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import os
 import time
+from unittest import mock
 
 import pytest
 
 import gmqtt
 from tests.utils import Callbacks, cleanup, clean_retained
 
 if os.getenv('TOKEN'):
@@ -458,7 +459,26 @@
     await asyncio.sleep(1)
 
     aclient.publish(TOPICS[0], b"qos 0")
     aclient.publish(TOPICS[0], b"qos 1", 1)
     aclient.publish(TOPICS[0], b"qos 2", 2)
     await asyncio.sleep(1)
     assert len(callback2.messages) == 3
+
+
+@pytest.mark.asyncio
+async def test_reconnection_with_failure(init_clients):
+    aclient, callback, bclient, callback2 = init_clients
+    aclient.set_config({'reconnect_retries': -1, 'reconnect_delay': 0})
+    await aclient.connect(host=host, port=port)
+    await bclient.connect(host=host, port=port)
+
+    bclient.subscribe(TOPICS[0])
+
+    with mock.patch.object(aclient, '_disconnect') as disconnect_mock:
+        disconnect_mock.side_effect = ConnectionAbortedError("error")
+        await aclient.reconnect()
+
+    # Check aclient is still working after reconnection
+    aclient.publish(TOPICS[0], b"test")
+    await asyncio.sleep(5)
+    assert len(callback2.messages) == 1
```

### Comparing `gmqtt-0.6.8/examples/shared_subscriptions.py` & `gmqtt-0.6.9/examples/shared_subscriptions.py`

 * *Files identical despite different names*

### Comparing `gmqtt-0.6.8/examples/will_message.py` & `gmqtt-0.6.9/examples/will_message.py`

 * *Files identical despite different names*

### Comparing `gmqtt-0.6.8/examples/properties.py` & `gmqtt-0.6.9/examples/properties.py`

 * *Files identical despite different names*

### Comparing `gmqtt-0.6.8/gmqtt.egg-info/SOURCES.txt` & `gmqtt-0.6.9/gmqtt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gmqtt-0.6.8/gmqtt.egg-info/PKG-INFO` & `gmqtt-0.6.9/gmqtt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmqtt
-Version: 0.6.8
+Version: 0.6.9
 Summary: Client for MQTT protocol
 Home-page: https://github.com/wialon/gmqtt
 Author: Mikhail Turchunovich
 Author-email: mitu@gurtam.com
 License: MIT
 Download-URL: https://github.com/wialon/gmqtt
 Description: [![PyPI version](https://badge.fury.io/py/gmqtt.svg)](https://badge.fury.io/py/gmqtt) [![Build Status](https://travis-ci.com/wialon/gmqtt.svg?branch=master)](https://travis-ci.com/wialon/gmqtt) [![codecov](https://codecov.io/gh/wialon/gmqtt/branch/master/graph/badge.svg)](https://codecov.io/gh/wialon/gmqtt)
```

### Comparing `gmqtt-0.6.8/PKG-INFO` & `gmqtt-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmqtt
-Version: 0.6.8
+Version: 0.6.9
 Summary: Client for MQTT protocol
 Home-page: https://github.com/wialon/gmqtt
 Author: Mikhail Turchunovich
 Author-email: mitu@gurtam.com
 License: MIT
 Download-URL: https://github.com/wialon/gmqtt
 Description: [![PyPI version](https://badge.fury.io/py/gmqtt.svg)](https://badge.fury.io/py/gmqtt) [![Build Status](https://travis-ci.com/wialon/gmqtt.svg?branch=master)](https://travis-ci.com/wialon/gmqtt) [![codecov](https://codecov.io/gh/wialon/gmqtt/branch/master/graph/badge.svg)](https://codecov.io/gh/wialon/gmqtt)
```

### Comparing `gmqtt-0.6.8/README.md` & `gmqtt-0.6.9/README.md`

 * *Files identical despite different names*

