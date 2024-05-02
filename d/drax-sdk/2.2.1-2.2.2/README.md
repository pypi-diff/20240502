# Comparing `tmp/drax_sdk-2.2.1.tar.gz` & `tmp/drax_sdk-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drax_sdk-2.2.1.tar", max compression
+gzip compressed data, was "drax_sdk-2.2.2.tar", max compression
```

## Comparing `drax_sdk-2.2.1.tar` & `drax_sdk-2.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      514 2024-04-23 09:08:04.529632 drax_sdk-2.2.1/README.md
--rw-r--r--   0        0        0        0 2024-04-23 09:08:58.311282 drax_sdk-2.2.1/drax_sdk/__init__.py
--rw-r--r--   0        0        0     9482 2024-04-30 08:45:49.743984 drax_sdk-2.2.1/drax_sdk/broker/amqp_select_broker.py
--rw-r--r--   0        0        0     9722 2024-04-23 19:01:05.353666 drax_sdk-2.2.1/drax_sdk/clients/drax_core_client.py
--rw-r--r--   0        0        0     7534 2024-04-29 17:11:14.631989 drax_sdk-2.2.1/drax_sdk/drax.py
--rw-r--r--   0        0        0     2632 2024-04-24 11:25:01.894264 drax_sdk-2.2.1/drax_sdk/keystore.parquet
--rw-r--r--   0        0        0     4234 2024-04-29 17:14:04.731172 drax_sdk-2.2.1/drax_sdk/model/dto.py
--rw-r--r--   0        0        0     1479 2024-04-29 17:05:39.625330 drax_sdk-2.2.1/drax_sdk/model/dynamic.py
--rw-r--r--   0        0        0      512 2024-04-23 13:55:28.408981 drax_sdk-2.2.1/drax_sdk/model/event.py
--rw-r--r--   0        0        0     3448 2024-04-30 08:39:15.667730 drax_sdk-2.2.1/drax_sdk/model/node.py
--rw-r--r--   0        0        0      524 2024-04-23 14:04:03.872372 drax_sdk-2.2.1/drax_sdk/model/project.py
--rw-r--r--   0        0        0        0 2024-04-23 14:40:17.430746 drax_sdk-2.2.1/drax_sdk/utils/__init__.py
--rw-r--r--   0        0        0     1643 2024-04-23 18:05:22.265455 drax_sdk-2.2.1/drax_sdk/utils/bytes_codec.py
--rw-r--r--   0        0        0     1432 2024-04-29 17:12:52.612558 drax_sdk-2.2.1/drax_sdk/utils/codec.py
--rw-r--r--   0        0        0     2468 2024-04-24 11:01:18.261896 drax_sdk-2.2.1/drax_sdk/utils/keystore.py
--rw-r--r--   0        0        0       71 2024-04-23 14:29:18.856060 drax_sdk-2.2.1/drax_sdk/utils/timestamp.py
--rw-r--r--   0        0        0      447 2024-04-30 08:47:24.610941 drax_sdk-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     1230 1970-01-01 00:00:00.000000 drax_sdk-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0      514 2024-04-23 09:08:04.529632 drax_sdk-2.2.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 09:08:58.311282 drax_sdk-2.2.2/drax_sdk/__init__.py
+-rw-r--r--   0        0        0    10477 2024-05-02 07:53:41.565314 drax_sdk-2.2.2/drax_sdk/broker/amqp_broker.py
+-rw-r--r--   0        0        0     9722 2024-04-23 19:01:05.353666 drax_sdk-2.2.2/drax_sdk/clients/drax_core_client.py
+-rw-r--r--   0        0        0     7534 2024-04-29 17:11:14.631989 drax_sdk-2.2.2/drax_sdk/drax.py
+-rw-r--r--   0        0        0     2632 2024-04-24 11:25:01.894264 drax_sdk-2.2.2/drax_sdk/keystore.parquet
+-rw-r--r--   0        0        0     4234 2024-04-29 17:14:04.731172 drax_sdk-2.2.2/drax_sdk/model/dto.py
+-rw-r--r--   0        0        0     1479 2024-04-29 17:05:39.625330 drax_sdk-2.2.2/drax_sdk/model/dynamic.py
+-rw-r--r--   0        0        0      512 2024-04-23 13:55:28.408981 drax_sdk-2.2.2/drax_sdk/model/event.py
+-rw-r--r--   0        0        0     3448 2024-04-30 08:39:15.667730 drax_sdk-2.2.2/drax_sdk/model/node.py
+-rw-r--r--   0        0        0      524 2024-04-23 14:04:03.872372 drax_sdk-2.2.2/drax_sdk/model/project.py
+-rw-r--r--   0        0        0        0 2024-04-23 14:40:17.430746 drax_sdk-2.2.2/drax_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     1643 2024-04-23 18:05:22.265455 drax_sdk-2.2.2/drax_sdk/utils/bytes_codec.py
+-rw-r--r--   0        0        0     1432 2024-04-29 17:12:52.612558 drax_sdk-2.2.2/drax_sdk/utils/codec.py
+-rw-r--r--   0        0        0     2468 2024-04-24 11:01:18.261896 drax_sdk-2.2.2/drax_sdk/utils/keystore.py
+-rw-r--r--   0        0        0       71 2024-04-23 14:29:18.856060 drax_sdk-2.2.2/drax_sdk/utils/timestamp.py
+-rw-r--r--   0        0        0      447 2024-05-02 08:04:39.347470 drax_sdk-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1230 1970-01-01 00:00:00.000000 drax_sdk-2.2.2/PKG-INFO
```

### Comparing `drax_sdk-2.2.1/README.md` & `drax_sdk-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.1/drax_sdk/broker/amqp_select_broker.py` & `drax_sdk-2.2.2/drax_sdk/broker/amqp_broker.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,30 +26,33 @@
 class Listener(ABC, Generic[T]):
     id: str = uuid.uuid4().hex
     routing_key: str
     queue: str | None = None
     callback: Callable[[T], None]
     exchange: str = "amq.topic"
     auto_ack: bool = True
+    node_id: str | None = None
 
     _channel: Channel
 
     def __init__(
         self,
         exchange: str,
         routing_key: str,
         callback: Callable[[T], None],
         queue: str = "",
         auto_ack: bool = True,
+        node_id: str = None,
     ):
         self.exchange = exchange
         self.routing_key = routing_key
         self.callback = callback
         self.queue = queue
         self.auto_ack = auto_ack
+        self.node_id = node_id
 
     def on_queue_declared(self, method_frame):
         self.queue = method_frame.method.queue
         self._channel.queue_bind(
             exchange=self.exchange,
             queue=self.queue,
             routing_key=self.routing_key,
@@ -97,29 +100,40 @@
 
 class ConfigurationListener(Listener[Configuration]):
 
     def __init__(
         self,
         routing_key: str,
         callback: Callable[[Configuration], None],
+        node_id: str | None = None,
     ):
         super().__init__(
             routing_key=routing_key,
             callback=callback,
             exchange="amq.topic",
             queue="",
+            node_id=node_id,
         )
 
     def on_message(self, ch, method, properties, body):
         try:
             logger.info("Received configuration: %r", properties)
             json_data = json.loads(body.decode("utf-8"))
             json_data = base64_to_bytes(json_data)
             configuration_response = ConfigurationResponse.model_validate(json_data)
 
+            if self.node_id is not None:
+                if configuration_response.node_id != self.node_id:
+                    logger.info(
+                        "Configuration for node %s not for listener %s. Ignoring...",
+                        configuration_response.node_id,
+                        self.id,
+                    )
+                    return
+
             if configuration_response.cryptography_disabled:
                 configuration_map = json.loads(
                     configuration_response.configuration.decode()
                 )
             else:
                 node_private_key = KeyStore.get_private_key(
                     configuration_response.node_id
@@ -139,29 +153,40 @@
 
 
 class StateListener(Listener[State]):
     def __init__(
         self,
         routing_key: str,
         callback: Callable[[State], None],
+        node_id: str | None = None,
     ):
         super().__init__(
             routing_key=routing_key,
             callback=callback,
             exchange="amq.topic",
             queue="",
+            node_id=node_id,
         )
 
     def on_message(self, ch, method, properties, body):
         try:
             logger.info("Received state: %r", properties)
             json_data = json.loads(body.decode("utf-8"))
             json_data = base64_to_bytes(json_data)
             state_response = StateResponse.model_validate(json_data)
 
+            if self.node_id is not None:
+                if state_response.node_id != self.node_id:
+                    logger.info(
+                        "State for node %s not for listener %s. Ignoring...",
+                        state_response.node_id,
+                        self.id,
+                    )
+                    return
+
             state = State.from_dict(state_response.state)
             state.node_id = state_response.node_id
             state.timestamp = state_response.timestamp
 
             self.callback(state)
         except Exception as e:
             logger.error("Error processing state: %s", e)
@@ -221,21 +246,21 @@
             self._connect()
 
     def add_configuration_listener(
         self,
         topic: str,
         cb: Callable[[Configuration], None],
         project_id: str = None,
+        node_id: str = None,
     ):
         project_id = project_id or self._configuration.project_id
         project_topic = f"{project_id}/{topic}".replace("/", ".")
 
         listener = ConfigurationListener(
-            routing_key=project_topic,
-            callback=cb,
+            routing_key=project_topic, callback=cb, node_id=node_id
         )
         self._listeners.append(listener)
 
         logger.info(
             "Registered configuration listener %s for topic: %s",
             listener.id,
             project_topic,
@@ -244,21 +269,21 @@
         listener.start_consuming(self._channel)
 
     def add_state_listener(
         self,
         topic: str,
         cb: Callable[[State], None],
         project_id: str = None,
+        node_id: str = None,
     ):
         project_id = project_id or self._configuration.project_id
         project_topic = f"{project_id}/{topic}".replace("/", ".")
 
         listener = StateListener(
-            routing_key=project_topic,
-            callback=cb,
+            routing_key=project_topic, callback=cb, node_id=node_id
         )
         self._listeners.append(listener)
 
         logger.info(
             "Registered state listener %s for topic: %s",
             listener.id,
             project_topic,
```

### Comparing `drax_sdk-2.2.1/drax_sdk/clients/drax_core_client.py` & `drax_sdk-2.2.2/drax_sdk/clients/drax_core_client.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.1/drax_sdk/drax.py` & `drax_sdk-2.2.2/drax_sdk/drax.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.1/drax_sdk/keystore.parquet` & `drax_sdk-2.2.2/drax_sdk/keystore.parquet`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.1/drax_sdk/model/dto.py` & `drax_sdk-2.2.2/drax_sdk/model/dto.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.1/drax_sdk/model/dynamic.py` & `drax_sdk-2.2.2/drax_sdk/model/dynamic.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.1/drax_sdk/model/event.py` & `drax_sdk-2.2.2/drax_sdk/model/event.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.1/drax_sdk/model/node.py` & `drax_sdk-2.2.2/drax_sdk/model/node.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.1/drax_sdk/model/project.py` & `drax_sdk-2.2.2/drax_sdk/model/project.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.1/drax_sdk/utils/bytes_codec.py` & `drax_sdk-2.2.2/drax_sdk/utils/bytes_codec.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.1/drax_sdk/utils/codec.py` & `drax_sdk-2.2.2/drax_sdk/utils/codec.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.1/drax_sdk/utils/keystore.py` & `drax_sdk-2.2.2/drax_sdk/utils/keystore.py`

 * *Files identical despite different names*

### Comparing `drax_sdk-2.2.1/PKG-INFO` & `drax_sdk-2.2.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drax-sdk
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python sdk for Drax IoT Platform
 Author: Applica Software Guru
 Author-email: info@applica.guru
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

