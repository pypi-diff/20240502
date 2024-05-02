# Comparing `tmp/aiomysensors-0.3.8.tar.gz` & `tmp/aiomysensors-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomysensors-0.3.8.tar", max compression
+gzip compressed data, was "aiomysensors-0.3.9.tar", max compression
```

## Comparing `aiomysensors-0.3.8.tar` & `aiomysensors-0.3.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11346 2023-03-17 06:38:03.732234 aiomysensors-0.3.8/LICENSE
--rw-r--r--   0        0        0     3642 2023-03-17 06:38:03.732234 aiomysensors-0.3.8/README.md
--rw-r--r--   0        0        0     3853 2023-03-17 06:38:04.864238 aiomysensors-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      442 2023-03-17 06:38:04.780238 aiomysensors-0.3.8/src/aiomysensors/__init__.py
--rw-r--r--   0        0        0      797 2023-03-17 06:38:03.732234 aiomysensors-0.3.8/src/aiomysensors/cli/__init__.py
--rw-r--r--   0        0        0     1121 2023-03-17 06:38:03.732234 aiomysensors-0.3.8/src/aiomysensors/cli/gateway_mqtt.py
--rw-r--r--   0        0        0      754 2023-03-17 06:38:03.732234 aiomysensors-0.3.8/src/aiomysensors/cli/gateway_serial.py
--rw-r--r--   0        0        0      726 2023-03-17 06:38:03.732234 aiomysensors-0.3.8/src/aiomysensors/cli/gateway_tcp.py
--rw-r--r--   0        0        0     1599 2023-03-17 06:38:03.736234 aiomysensors-0.3.8/src/aiomysensors/cli/helper.py
--rw-r--r--   0        0        0     2968 2023-03-17 06:38:03.736234 aiomysensors-0.3.8/src/aiomysensors/exceptions.py
--rw-r--r--   0        0        0     4208 2023-03-17 06:38:03.736234 aiomysensors-0.3.8/src/aiomysensors/gateway.py
--rw-r--r--   0        0        0       38 2023-03-17 06:38:03.736234 aiomysensors-0.3.8/src/aiomysensors/model/__init__.py
--rw-r--r--   0        0        0      286 2023-03-17 06:38:03.736234 aiomysensors-0.3.8/src/aiomysensors/model/const.py
--rw-r--r--   0        0        0     6030 2023-03-17 06:38:03.736234 aiomysensors-0.3.8/src/aiomysensors/model/message.py
--rw-r--r--   0        0        0     5436 2023-03-17 06:38:03.736234 aiomysensors-0.3.8/src/aiomysensors/model/node.py
--rw-r--r--   0        0        0     4770 2023-03-17 06:38:03.736234 aiomysensors-0.3.8/src/aiomysensors/model/protocol/__init__.py
--rw-r--r--   0        0        0    17953 2023-03-17 06:38:03.736234 aiomysensors-0.3.8/src/aiomysensors/model/protocol/protocol_14.py
--rw-r--r--   0        0        0     9855 2023-03-17 06:38:03.736234 aiomysensors-0.3.8/src/aiomysensors/model/protocol/protocol_15.py
--rw-r--r--   0        0        0    18919 2023-03-17 06:38:03.736234 aiomysensors-0.3.8/src/aiomysensors/model/protocol/protocol_20.py
--rw-r--r--   0        0        0     3603 2023-03-17 06:38:03.736234 aiomysensors-0.3.8/src/aiomysensors/model/protocol/protocol_21.py
--rw-r--r--   0        0        0     5125 2023-03-17 06:38:03.736234 aiomysensors-0.3.8/src/aiomysensors/model/protocol/protocol_22.py
--rw-r--r--   0        0        0     2634 2023-03-17 06:38:03.736234 aiomysensors-0.3.8/src/aiomysensors/persistence.py
--rw-r--r--   0        0        0        0 2023-03-17 06:38:03.736234 aiomysensors-0.3.8/src/aiomysensors/py.typed
--rw-r--r--   0        0        0     2770 2023-03-17 06:38:03.736234 aiomysensors-0.3.8/src/aiomysensors/transport/__init__.py
--rw-r--r--   0        0        0     8483 2023-03-17 06:38:03.736234 aiomysensors-0.3.8/src/aiomysensors/transport/mqtt.py
--rw-r--r--   0        0        0      767 2023-03-17 06:38:03.736234 aiomysensors-0.3.8/src/aiomysensors/transport/serial.py
--rw-r--r--   0        0        0      700 2023-03-17 06:38:03.736234 aiomysensors-0.3.8/src/aiomysensors/transport/tcp.py
--rw-r--r--   0        0        0     4940 1970-01-01 00:00:00.000000 aiomysensors-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/LICENSE
+-rw-r--r--   0        0        0     3642 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/README.md
+-rw-r--r--   0        0        0     3853 2023-03-17 11:32:32.187822 aiomysensors-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      442 2023-03-17 11:32:32.119822 aiomysensors-0.3.9/src/aiomysensors/__init__.py
+-rw-r--r--   0        0        0      797 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/cli/__init__.py
+-rw-r--r--   0        0        0     1121 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/cli/gateway_mqtt.py
+-rw-r--r--   0        0        0      754 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/cli/gateway_serial.py
+-rw-r--r--   0        0        0      726 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/cli/gateway_tcp.py
+-rw-r--r--   0        0        0     1599 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/cli/helper.py
+-rw-r--r--   0        0        0     2968 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/exceptions.py
+-rw-r--r--   0        0        0     4208 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/gateway.py
+-rw-r--r--   0        0        0       38 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/model/__init__.py
+-rw-r--r--   0        0        0      286 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/model/const.py
+-rw-r--r--   0        0        0     6030 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/model/message.py
+-rw-r--r--   0        0        0     5436 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/model/node.py
+-rw-r--r--   0        0        0     4770 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/model/protocol/__init__.py
+-rw-r--r--   0        0        0    17953 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/model/protocol/protocol_14.py
+-rw-r--r--   0        0        0     9855 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/model/protocol/protocol_15.py
+-rw-r--r--   0        0        0    18919 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/model/protocol/protocol_20.py
+-rw-r--r--   0        0        0     3603 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/model/protocol/protocol_21.py
+-rw-r--r--   0        0        0     5125 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/model/protocol/protocol_22.py
+-rw-r--r--   0        0        0     2634 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/persistence.py
+-rw-r--r--   0        0        0        0 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/py.typed
+-rw-r--r--   0        0        0     2770 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/transport/__init__.py
+-rw-r--r--   0        0        0     8483 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/transport/mqtt.py
+-rw-r--r--   0        0        0      767 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/transport/serial.py
+-rw-r--r--   0        0        0      700 2023-03-17 11:32:31.335823 aiomysensors-0.3.9/src/aiomysensors/transport/tcp.py
+-rw-r--r--   0        0        0     4940 1970-01-01 00:00:00.000000 aiomysensors-0.3.9/PKG-INFO
```

### Comparing `aiomysensors-0.3.8/LICENSE` & `aiomysensors-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/README.md` & `aiomysensors-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/pyproject.toml` & `aiomysensors-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 license = "Apache Software License 2.0"
 name = "aiomysensors"
 packages = [
   {include = "aiomysensors", from = "src"},
 ]
 readme = "README.md"
 repository = "https://github.com/MartinHjelmare/aiomysensors"
-version = "0.3.8"
+version = "0.3.9"
 
 [tool.poetry.scripts]
 aiomysensors = 'aiomysensors.cli:cli'
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/MartinHjelmare/aiomysensors/issues"
 "Changelog" = "https://github.com/MartinHjelmare/aiomysensors/blob/main/CHANGELOG.md"
```

### Comparing `aiomysensors-0.3.8/src/aiomysensors/cli/__init__.py` & `aiomysensors-0.3.9/src/aiomysensors/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/src/aiomysensors/cli/gateway_mqtt.py` & `aiomysensors-0.3.9/src/aiomysensors/cli/gateway_mqtt.py`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/src/aiomysensors/cli/gateway_serial.py` & `aiomysensors-0.3.9/src/aiomysensors/cli/gateway_serial.py`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/src/aiomysensors/cli/gateway_tcp.py` & `aiomysensors-0.3.9/src/aiomysensors/cli/gateway_tcp.py`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/src/aiomysensors/cli/helper.py` & `aiomysensors-0.3.9/src/aiomysensors/cli/helper.py`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/src/aiomysensors/exceptions.py` & `aiomysensors-0.3.9/src/aiomysensors/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/src/aiomysensors/gateway.py` & `aiomysensors-0.3.9/src/aiomysensors/gateway.py`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/src/aiomysensors/model/message.py` & `aiomysensors-0.3.9/src/aiomysensors/model/message.py`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/src/aiomysensors/model/node.py` & `aiomysensors-0.3.9/src/aiomysensors/model/node.py`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/src/aiomysensors/model/protocol/__init__.py` & `aiomysensors-0.3.9/src/aiomysensors/model/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/src/aiomysensors/model/protocol/protocol_14.py` & `aiomysensors-0.3.9/src/aiomysensors/model/protocol/protocol_14.py`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/src/aiomysensors/model/protocol/protocol_15.py` & `aiomysensors-0.3.9/src/aiomysensors/model/protocol/protocol_15.py`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/src/aiomysensors/model/protocol/protocol_20.py` & `aiomysensors-0.3.9/src/aiomysensors/model/protocol/protocol_20.py`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/src/aiomysensors/model/protocol/protocol_21.py` & `aiomysensors-0.3.9/src/aiomysensors/model/protocol/protocol_21.py`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/src/aiomysensors/model/protocol/protocol_22.py` & `aiomysensors-0.3.9/src/aiomysensors/model/protocol/protocol_22.py`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/src/aiomysensors/persistence.py` & `aiomysensors-0.3.9/src/aiomysensors/persistence.py`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/src/aiomysensors/transport/__init__.py` & `aiomysensors-0.3.9/src/aiomysensors/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/src/aiomysensors/transport/mqtt.py` & `aiomysensors-0.3.9/src/aiomysensors/transport/mqtt.py`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/src/aiomysensors/transport/serial.py` & `aiomysensors-0.3.9/src/aiomysensors/transport/serial.py`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/src/aiomysensors/transport/tcp.py` & `aiomysensors-0.3.9/src/aiomysensors/transport/tcp.py`

 * *Files identical despite different names*

### Comparing `aiomysensors-0.3.8/PKG-INFO` & `aiomysensors-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomysensors
-Version: 0.3.8
+Version: 0.3.9
 Summary: Python asyncio package to connect to MySensors gateways.
 Home-page: https://github.com/MartinHjelmare/aiomysensors
 License: Apache Software License 2.0
 Author: Martin Hjelmare
 Author-email: marhje52@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aiomysensors Version: 0.3.8 Summary: Python asyncio
+Metadata-Version: 2.1 Name: aiomysensors Version: 0.3.9 Summary: Python asyncio
 package to connect to MySensors gateways. Home-page: https://github.com/
 MartinHjelmare/aiomysensors License: Apache Software License 2.0 Author: Martin
 Hjelmare Author-email: marhje52@gmail.com Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: Other/Proprietary License Classifier: Natural
 Language :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

