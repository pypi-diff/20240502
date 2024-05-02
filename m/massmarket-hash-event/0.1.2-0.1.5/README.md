# Comparing `tmp/massmarket_hash_event-0.1.2.tar.gz` & `tmp/massmarket_hash_event-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "massmarket_hash_event-0.1.2.tar", last modified: Wed May  1 11:16:06 2024, max compression
+gzip compressed data, was "massmarket_hash_event-0.1.5.tar", last modified: Mon Apr 29 08:30:57 2024, max compression
```

## Comparing `massmarket_hash_event-0.1.2.tar` & `massmarket_hash_event-0.1.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-05-01 11:16:06.305533 massmarket_hash_event-0.1.2/
--rw-r--r--   0 cryptix   (1001) users      (100)     1593 2024-05-01 11:14:57.000000 massmarket_hash_event-0.1.2/Makefile
--rw-r--r--   0 cryptix   (1001) users      (100)      860 2024-05-01 11:16:06.305533 massmarket_hash_event-0.1.2/PKG-INFO
-drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-05-01 11:16:06.303533 massmarket_hash_event-0.1.2/massmarket_hash_event/
--rw-r--r--   0 cryptix   (1001) users      (100)     7012 2024-05-01 11:14:57.000000 massmarket_hash_event-0.1.2/massmarket_hash_event/__init__.py
--rw-r--r--   0 cryptix   (1001) users      (100)     2027 2024-05-01 11:14:57.000000 massmarket_hash_event-0.1.2/massmarket_hash_event/authentication_pb2.py
--rw-r--r--   0 cryptix   (1001) users      (100)     1857 2024-05-01 11:14:57.000000 massmarket_hash_event-0.1.2/massmarket_hash_event/authentication_pb2.pyi
--rw-r--r--   0 cryptix   (1001) users      (100)     1094 2024-05-01 11:14:57.000000 massmarket_hash_event-0.1.2/massmarket_hash_event/error_pb2.py
--rw-r--r--   0 cryptix   (1001) users      (100)      554 2024-05-01 11:14:57.000000 massmarket_hash_event-0.1.2/massmarket_hash_event/error_pb2.pyi
--rw-r--r--   0 cryptix   (1001) users      (100)     6935 2024-05-01 11:14:57.000000 massmarket_hash_event-0.1.2/massmarket_hash_event/store_events_pb2.py
--rw-r--r--   0 cryptix   (1001) users      (100)    11078 2024-05-01 11:14:57.000000 massmarket_hash_event-0.1.2/massmarket_hash_event/store_events_pb2.pyi
--rw-r--r--   0 cryptix   (1001) users      (100)     2110 2024-05-01 11:14:57.000000 massmarket_hash_event-0.1.2/massmarket_hash_event/store_requests_pb2.py
--rw-r--r--   0 cryptix   (1001) users      (100)     1983 2024-05-01 11:14:57.000000 massmarket_hash_event-0.1.2/massmarket_hash_event/store_requests_pb2.pyi
--rw-r--r--   0 cryptix   (1001) users      (100)     3016 2024-05-01 11:14:57.000000 massmarket_hash_event-0.1.2/massmarket_hash_event/transport_pb2.py
--rw-r--r--   0 cryptix   (1001) users      (100)     3469 2024-05-01 11:14:57.000000 massmarket_hash_event-0.1.2/massmarket_hash_event/transport_pb2.pyi
--rw-r--r--   0 cryptix   (1001) users      (100)     3413 2024-05-01 11:14:53.000000 massmarket_hash_event-0.1.2/massmarket_hash_event/typedData.json
-drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-05-01 11:16:06.304533 massmarket_hash_event-0.1.2/massmarket_hash_event.egg-info/
--rw-r--r--   0 cryptix   (1001) users      (100)      860 2024-05-01 11:16:06.000000 massmarket_hash_event-0.1.2/massmarket_hash_event.egg-info/PKG-INFO
--rw-r--r--   0 cryptix   (1001) users      (100)      777 2024-05-01 11:16:06.000000 massmarket_hash_event-0.1.2/massmarket_hash_event.egg-info/SOURCES.txt
--rw-r--r--   0 cryptix   (1001) users      (100)        1 2024-05-01 11:16:06.000000 massmarket_hash_event-0.1.2/massmarket_hash_event.egg-info/dependency_links.txt
--rw-r--r--   0 cryptix   (1001) users      (100)       20 2024-05-01 11:16:06.000000 massmarket_hash_event-0.1.2/massmarket_hash_event.egg-info/requires.txt
--rw-r--r--   0 cryptix   (1001) users      (100)       22 2024-05-01 11:16:06.000000 massmarket_hash_event-0.1.2/massmarket_hash_event.egg-info/top_level.txt
--rw-r--r--   0 cryptix   (1001) users      (100)     1390 2024-05-01 11:15:32.000000 massmarket_hash_event-0.1.2/pyproject.toml
--rw-r--r--   0 cryptix   (1001) users      (100)       38 2024-05-01 11:16:06.305533 massmarket_hash_event-0.1.2/setup.cfg
-drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-05-01 11:16:06.304533 massmarket_hash_event-0.1.2/tests/
--rw-r--r--   0 cryptix   (1001) users      (100)     1289 2024-05-01 11:14:57.000000 massmarket_hash_event-0.1.2/tests/test_encode.py
--rw-r--r--   0 cryptix   (1001) users      (100)     6240 2024-05-01 11:14:57.000000 massmarket_hash_event-0.1.2/tests/test_signatures.py
+drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-29 08:30:57.600065 massmarket_hash_event-0.1.5/
+-rw-r--r--   0 cryptix   (1001) users      (100)     1518 2024-04-29 08:04:49.000000 massmarket_hash_event-0.1.5/Makefile
+-rw-r--r--   0 cryptix   (1001) users      (100)      860 2024-04-29 08:30:57.600065 massmarket_hash_event-0.1.5/PKG-INFO
+drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-29 08:30:57.598065 massmarket_hash_event-0.1.5/massmarket_hash_event/
+-rw-r--r--   0 cryptix   (1001) users      (100)     5636 2024-04-29 08:17:51.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/__init__.py
+-rw-r--r--   0 cryptix   (1001) users      (100)     1952 2024-04-29 08:21:12.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/authentication_pb2.py
+-rw-r--r--   0 cryptix   (1001) users      (100)     1782 2024-04-29 08:21:12.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/authentication_pb2.pyi
+-rw-r--r--   0 cryptix   (1001) users      (100)     1019 2024-04-29 08:21:12.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/error_pb2.py
+-rw-r--r--   0 cryptix   (1001) users      (100)      479 2024-04-29 08:21:12.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/error_pb2.pyi
+-rw-r--r--   0 cryptix   (1001) users      (100)     6648 2024-04-29 08:16:37.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/store_events_pb2.py
+-rw-r--r--   0 cryptix   (1001) users      (100)    10868 2024-04-29 08:16:37.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/store_events_pb2.pyi
+-rw-r--r--   0 cryptix   (1001) users      (100)     1992 2024-04-29 08:21:12.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/store_requests_pb2.py
+-rw-r--r--   0 cryptix   (1001) users      (100)     1888 2024-04-29 08:21:12.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/store_requests_pb2.pyi
+-rw-r--r--   0 cryptix   (1001) users      (100)     2941 2024-04-29 08:21:12.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/transport_pb2.py
+-rw-r--r--   0 cryptix   (1001) users      (100)     3394 2024-04-29 08:21:12.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/transport_pb2.pyi
+-rw-r--r--   0 cryptix   (1001) users      (100)     3290 2024-04-29 08:16:57.000000 massmarket_hash_event-0.1.5/massmarket_hash_event/typedData.json
+drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-29 08:30:57.599065 massmarket_hash_event-0.1.5/massmarket_hash_event.egg-info/
+-rw-r--r--   0 cryptix   (1001) users      (100)      860 2024-04-29 08:30:57.000000 massmarket_hash_event-0.1.5/massmarket_hash_event.egg-info/PKG-INFO
+-rw-r--r--   0 cryptix   (1001) users      (100)      777 2024-04-29 08:30:57.000000 massmarket_hash_event-0.1.5/massmarket_hash_event.egg-info/SOURCES.txt
+-rw-r--r--   0 cryptix   (1001) users      (100)        1 2024-04-29 08:30:57.000000 massmarket_hash_event-0.1.5/massmarket_hash_event.egg-info/dependency_links.txt
+-rw-r--r--   0 cryptix   (1001) users      (100)       20 2024-04-29 08:30:57.000000 massmarket_hash_event-0.1.5/massmarket_hash_event.egg-info/requires.txt
+-rw-r--r--   0 cryptix   (1001) users      (100)       22 2024-04-29 08:30:57.000000 massmarket_hash_event-0.1.5/massmarket_hash_event.egg-info/top_level.txt
+-rw-r--r--   0 cryptix   (1001) users      (100)     1390 2024-04-29 08:16:06.000000 massmarket_hash_event-0.1.5/pyproject.toml
+-rw-r--r--   0 cryptix   (1001) users      (100)       38 2024-04-29 08:30:57.600065 massmarket_hash_event-0.1.5/setup.cfg
+drwxr-xr-x   0 cryptix   (1001) users      (100)        0 2024-04-29 08:30:57.599065 massmarket_hash_event-0.1.5/tests/
+-rw-r--r--   0 cryptix   (1001) users      (100)     1289 2024-04-29 08:21:53.000000 massmarket_hash_event-0.1.5/tests/test_encode.py
+-rw-r--r--   0 cryptix   (1001) users      (100)     6515 2024-04-29 08:23:58.000000 massmarket_hash_event-0.1.5/tests/test_signatures.py
```

### Comparing `massmarket_hash_event-0.1.2/Makefile` & `massmarket_hash_event-0.1.5/Makefile`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# SPDX-FileCopyrightText: 2024 Mass Labs
-#
-# SPDX-License-Identifier: MIT
-
 OUT=massmarket_hash_event/
 
 all: transport_pb2.py  authentication_pb2.py store_requests_pb2.py error_pb2.py
 
 # TODO: define SRC list with replacements
 
 transport_pb2.py: ../transport.proto
```

### Comparing `massmarket_hash_event-0.1.2/PKG-INFO` & `massmarket_hash_event-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: massmarket_hash_event
-Version: 0.1.2
+Version: 0.1.5
 Summary: Helper functions to hash events for signature creation and verification on Mass Market.
 Author-email: Henry Bubert <henry@mass.market>
 License: MIT
 Project-URL: Homepage, https://mass.market
 Project-URL: Repository, https://github.com/masslbs/network-schema.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `massmarket_hash_event-0.1.2/massmarket_hash_event/__init__.py` & `massmarket_hash_event-0.1.5/massmarket_hash_event/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 __all__ = ['hash_event', 'Hasher',
            'transport_pb2', 'authentication_pb2', 'store_requests_pb2', 'error_pb2',
            'store_events_pb2']
 
 import json
 import binascii
-from pprint import pprint
 from importlib.resources import files
 
 from eth_account.messages import encode_structured_data
 
 from massmarket_hash_event import store_events_pb2
 
 event_typedData_spec = json.loads(files("massmarket_hash_event").joinpath("typedData.json").read_text())
@@ -29,25 +28,15 @@
     def hash_event(self, evt: store_events_pb2.StoreEvent):
         return hash_event(evt, self.chain_id, self.storeRegAddress)
 
 def hash_event(evt: store_events_pb2.StoreEvent, chain_id, storeRegAddress):
     event_type = getattr(evt, evt.WhichOneof('union'))
     event_name = event_type.DESCRIPTOR.name
     event_td_spec = event_typedData_spec[event_name].copy()
-
-    types = {
-        "EIP712Domain": [
-            {"name": "name", "type": "string"},
-            {"name": "version", "type": "string"},
-            {"name": "chainId", "type": "uint256"},
-            {"name": "verifyingContract", "type": "address"},
-        ],
-    }
-
-    # step 1: remove fields from event_td_spec that are not set in event_td_data
+    # remove fields from event_td_spec that are not set in event_td_data
     if event_name == "UpdateStoreManifest":
         field = event_type.field
         if field == store_events_pb2.UpdateStoreManifest.MANIFEST_FIELD_DOMAIN:
             event_td_spec.remove({"name": "tag_id", "type": "bytes32"})
             event_td_spec.remove({"name": "erc20_addr", "type": "address"})
         elif field == store_events_pb2.UpdateStoreManifest.MANIFEST_FIELD_PUBLISHED_TAG:
             event_td_spec.remove({"name": "string", "type": "string"})
@@ -79,77 +68,49 @@
         elif action == store_events_pb2.UpdateTag.TAG_ACTION_RENAME:
             event_td_spec.remove({"name": "item_id", "type": "bytes32"})
             event_td_spec.remove({"name": "delete", "type": "bool"})
         elif action == store_events_pb2.UpdateTag.TAG_ACTION_DELETE_TAG:
             event_td_spec.remove({"name": "item_id", "type": "bytes32"})
             event_td_spec.remove({"name": "new_name", "type": "string"})
         else:
-            raise Exception(f"Unknown action on UpdateTag: {action}")
-    elif event_name == "UpdateOrder":
-        # UpdateOrder follows a nested message pattern and thus needs slightly differnt handling
-        # we are not just pruning the unused values but add the used type to typed_data
-        action = event_type.WhichOneof("action")
-
-        # build map of action > message
-        name2msgtd = {}
-        msgs = [td for td in event_td_spec if "message" in td]
-        for td in msgs:
-            name2msgtd[td["name"]] = td["message"]
-
-        # other fields are used as is
-        event_td_spec = [td for td in event_td_spec if "message" not in td]
-
-        if action not in name2msgtd:
-         raise Exception(f"Unhandled action on UpdateOrder: {action}")
-
-        event_td_spec.append({"name": action, "type": action})
-        types[action] = name2msgtd[action].copy()
-
-
-    # step 2: convert event to typedData
+            raise Exception(f"Unknown action: {action}")
+    # convert event to typedData
     event_td_data = event_to_typedData_dict(evt, event_td_spec)
     if event_name == "ChangeStock":
-        # remove order_id if empty
-        if len(event_td_data["order_id"]) == 0:
-            event_td_spec.remove({"name": "order_id", "type": "bytes32"})
+        # remove cart_id if empty
+        if len(event_td_data["cart_id"]) == 0:
+            event_td_spec.remove({"name": "cart_id", "type": "bytes32"})
             event_td_spec.remove({"name": "tx_hash", "type": "bytes32"})
-            del event_td_data["order_id"]
+            del event_td_data["cart_id"]
             del event_td_data["tx_hash"]
-    elif event_name == "UpdateOrder":
-        # we need to change the nested pb message into a subscriptable thing
-        # for encode_structured_data to be happy
-        action = event_type.WhichOneof("action")
-        action_msg = getattr(event_type, action)
-        action_obj = {}
-
-        action_fields = action_msg.ListFields()
-        for field in action_fields:
-            name = field[0].name
-            action_obj[name] = getattr(action_msg, name)
-
+    elif event_name == "CartFinalized":
         # remove erc20_addr if empty
-        if action == "items_finalized" and "erc20_addr" not in action_obj:
-            types[action].remove({"name": "erc20_addr", "type": "address"})
-
-        # replace nested protobuf thing
-        event_td_data[action] = action_obj
+        if len(event_td_data["erc20_addr"]) == 0:
+            event_td_spec.remove({"name": "erc20_addr", "type": "address"})
+            del event_td_data["erc20_addr"]
 
-    types[event_name] = event_td_spec
     typed_data = {
-        "types": types,
+        "types": {
+            "EIP712Domain": [
+                {"name": "name", "type": "string"},
+                {"name": "version", "type": "string"},
+                {"name": "chainId", "type": "uint256"},
+                {"name": "verifyingContract", "type": "address"},
+            ],
+            event_name: event_td_spec,
+        },
         "primaryType": event_name,
         "domain": {
             "name": "MassMarket",
             "version": "1",
             "chainId": chain_id,
             "verifyingContract": storeRegAddress,
         },
         "message": event_td_data
     }
-    #pprint(typed_data)
     return encode_structured_data(typed_data)
 
 def event_to_typedData_dict(evt: store_events_pb2.StoreEvent, spec_for_event):
     which = evt.WhichOneof("union")
     if which is None:
         raise Exception("No event type set")
     unwrapped = getattr(evt, which)
```

### Comparing `massmarket_hash_event-0.1.2/massmarket_hash_event/authentication_pb2.py` & `massmarket_hash_event-0.1.5/massmarket_hash_event/authentication_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# SPDX-FileCopyrightText: 2024 Mass Labs
-#
-# SPDX-License-Identifier: MIT
-
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: authentication.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
```

### Comparing `massmarket_hash_event-0.1.2/massmarket_hash_event/authentication_pb2.pyi` & `massmarket_hash_event-0.1.5/massmarket_hash_event/authentication_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# SPDX-FileCopyrightText: 2024 Mass Labs
-#
-# SPDX-License-Identifier: MIT
-
 from massmarket_hash_event import error_pb2 as _error_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
```

### Comparing `massmarket_hash_event-0.1.2/massmarket_hash_event/error_pb2.py` & `massmarket_hash_event-0.1.5/massmarket_hash_event/error_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# SPDX-FileCopyrightText: 2024 Mass Labs
-#
-# SPDX-License-Identifier: MIT
-
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: error.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
```

### Comparing `massmarket_hash_event-0.1.2/massmarket_hash_event/store_events_pb2.py` & `massmarket_hash_event-0.1.5/massmarket_hash_event/store_events_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# SPDX-FileCopyrightText: 2024 Mass Labs
-#
-# SPDX-License-Identifier: MIT
-
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: store_events.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
@@ -13,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12store_events.proto\x12\x0bmarket.mass\"c\n\rStoreManifest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x16\n\x0estore_token_id\x18\x02 \x01(\x0c\x12\x0e\n\x06\x64omain\x18\x03 \x01(\t\x12\x18\n\x10published_tag_id\x18\x04 \x01(\x0c\"\xd7\x02\n\x13UpdateStoreManifest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12=\n\x05\x66ield\x18\x02 \x01(\x0e\x32..market.mass.UpdateStoreManifest.ManifestField\x12\x10\n\x06string\x18\x03 \x01(\tH\x00\x12\x10\n\x06tag_id\x18\x04 \x01(\x0cH\x00\x12\x14\n\nerc20_addr\x18\x05 \x01(\x0cH\x00\"\xab\x01\n\rManifestField\x12\x1e\n\x1aMANIFEST_FIELD_UNSPECIFIED\x10\x00\x12\x19\n\x15MANIFEST_FIELD_DOMAIN\x10\x01\x12 \n\x1cMANIFEST_FIELD_PUBLISHED_TAG\x10\x02\x12\x1c\n\x18MANIFEST_FIELD_ADD_ERC20\x10\x03\x12\x1f\n\x1bMANIFEST_FIELD_REMOVE_ERC20\x10\x04\x42\x07\n\x05value\"?\n\nCreateItem\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\r\n\x05price\x18\x02 \x01(\t\x12\x10\n\x08metadata\x18\x03 \x01(\x0c\"\xe7\x01\n\nUpdateItem\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0f\n\x07item_id\x18\x02 \x01(\x0c\x12\x30\n\x05\x66ield\x18\x03 \x01(\x0e\x32!.market.mass.UpdateItem.ItemField\x12\x0f\n\x05price\x18\x04 \x01(\tH\x00\x12\x12\n\x08metadata\x18\x05 \x01(\x0cH\x00\"V\n\tItemField\x12\x1a\n\x16ITEM_FIELD_UNSPECIFIED\x10\x00\x12\x14\n\x10ITEM_FIELD_PRICE\x10\x01\x12\x17\n\x13ITEM_FIELD_METADATA\x10\x02\x42\x07\n\x05value\"+\n\tCreateTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xb2\x02\n\tUpdateTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0e\n\x06tag_id\x18\x02 \x01(\x0c\x12\x30\n\x06\x61\x63tion\x18\x03 \x01(\x0e\x32 .market.mass.UpdateTag.TagAction\x12\x11\n\x07item_id\x18\x04 \x01(\x0cH\x00\x12\x12\n\x08new_name\x18\x05 \x01(\tH\x00\x12\x10\n\x06\x64\x65lete\x18\x06 \x01(\x08H\x00\"\x8e\x01\n\tTagAction\x12\x1a\n\x16TAG_ACTION_UNSPECIFIED\x10\x00\x12\x17\n\x13TAG_ACTION_ADD_ITEM\x10\x01\x12\x1a\n\x16TAG_ACTION_REMOVE_ITEM\x10\x02\x12\x15\n\x11TAG_ACTION_RENAME\x10\x03\x12\x19\n\x15TAG_ACTION_DELETE_TAG\x10\x04\x42\x07\n\x05value\"c\n\x0b\x43hangeStock\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x10\n\x08item_ids\x18\x02 \x03(\x0c\x12\r\n\x05\x64iffs\x18\x03 \x03(\x11\x12\x10\n\x08order_id\x18\x04 \x01(\x0c\x12\x0f\n\x07tx_hash\x18\x05 \x01(\x0c\"Q\n\nNewKeyCard\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x18\n\x10user_wallet_addr\x18\x02 \x01(\x0c\x12\x17\n\x0f\x63\x61rd_public_key\x18\x03 \x01(\x0c\"\x1f\n\x0b\x43reateOrder\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\"\xe1\x03\n\x0bUpdateOrder\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x10\n\x08order_id\x18\x02 \x01(\x0c\x12<\n\x0c\x63hange_items\x18\x03 \x01(\x0b\x32$.market.mass.UpdateOrder.ChangeItemsH\x00\x12\x42\n\x0fitems_finalized\x18\x04 \x01(\x0b\x32\'.market.mass.UpdateOrder.ItemsFinalizedH\x00\x12@\n\x0eorder_canceled\x18\x05 \x01(\x0b\x32&.market.mass.UpdateOrder.OrderCanceledH\x00\x1a\x30\n\x0b\x43hangeItems\x12\x0f\n\x07item_id\x18\x01 \x01(\x0c\x12\x10\n\x08quantity\x18\x02 \x01(\x11\x1a\x89\x01\n\x0eItemsFinalized\x12\x15\n\rpurchase_addr\x18\x01 \x01(\x0c\x12\x12\n\nerc20_addr\x18\x02 \x01(\x0c\x12\x11\n\tsub_total\x18\x03 \x01(\t\x12\x11\n\tsales_tax\x18\x04 \x01(\t\x12\r\n\x05total\x18\x05 \x01(\t\x12\x17\n\x0ftotal_in_crypto\x18\x06 \x01(\t\x1a\"\n\rOrderCanceled\x12\x11\n\ttimestamp\x18\x01 \x01(\x04\x42\x08\n\x06\x61\x63tion\"\xa4\x04\n\nStoreEvent\x12\x11\n\tsignature\x18\x01 \x01(\x0c\x12\x34\n\x0estore_manifest\x18\x02 \x01(\x0b\x32\x1a.market.mass.StoreManifestH\x00\x12\x41\n\x15update_store_manifest\x18\x03 \x01(\x0b\x32 .market.mass.UpdateStoreManifestH\x00\x12.\n\x0b\x63reate_item\x18\x04 \x01(\x0b\x32\x17.market.mass.CreateItemH\x00\x12.\n\x0bupdate_item\x18\x05 \x01(\x0b\x32\x17.market.mass.UpdateItemH\x00\x12,\n\ncreate_tag\x18\x06 \x01(\x0b\x32\x16.market.mass.CreateTagH\x00\x12,\n\nupdate_tag\x18\x07 \x01(\x0b\x32\x16.market.mass.UpdateTagH\x00\x12\x30\n\x0c\x63reate_order\x18\x08 \x01(\x0b\x32\x18.market.mass.CreateOrderH\x00\x12\x30\n\x0cupdate_order\x18\t \x01(\x0b\x32\x18.market.mass.UpdateOrderH\x00\x12\x30\n\x0c\x63hange_stock\x18\x0c \x01(\x0b\x32\x18.market.mass.ChangeStockH\x00\x12/\n\x0cnew_key_card\x18\r \x01(\x0b\x32\x17.market.mass.NewKeyCardH\x00\x42\x07\n\x05unionb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12store_events.proto\x12\x0bmarket.mass\"c\n\rStoreManifest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x16\n\x0estore_token_id\x18\x02 \x01(\x0c\x12\x0e\n\x06\x64omain\x18\x03 \x01(\t\x12\x18\n\x10published_tag_id\x18\x04 \x01(\x0c\"\xd7\x02\n\x13UpdateStoreManifest\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12=\n\x05\x66ield\x18\x02 \x01(\x0e\x32..market.mass.UpdateStoreManifest.ManifestField\x12\x10\n\x06string\x18\x03 \x01(\tH\x00\x12\x10\n\x06tag_id\x18\x04 \x01(\x0cH\x00\x12\x14\n\nerc20_addr\x18\x05 \x01(\x0cH\x00\"\xab\x01\n\rManifestField\x12\x1e\n\x1aMANIFEST_FIELD_UNSPECIFIED\x10\x00\x12\x19\n\x15MANIFEST_FIELD_DOMAIN\x10\x01\x12 \n\x1cMANIFEST_FIELD_PUBLISHED_TAG\x10\x02\x12\x1c\n\x18MANIFEST_FIELD_ADD_ERC20\x10\x03\x12\x1f\n\x1bMANIFEST_FIELD_REMOVE_ERC20\x10\x04\x42\x07\n\x05value\"?\n\nCreateItem\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\r\n\x05price\x18\x02 \x01(\t\x12\x10\n\x08metadata\x18\x03 \x01(\x0c\"\xe7\x01\n\nUpdateItem\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0f\n\x07item_id\x18\x02 \x01(\x0c\x12\x30\n\x05\x66ield\x18\x03 \x01(\x0e\x32!.market.mass.UpdateItem.ItemField\x12\x0f\n\x05price\x18\x04 \x01(\tH\x00\x12\x12\n\x08metadata\x18\x05 \x01(\x0cH\x00\"V\n\tItemField\x12\x1a\n\x16ITEM_FIELD_UNSPECIFIED\x10\x00\x12\x14\n\x10ITEM_FIELD_PRICE\x10\x01\x12\x17\n\x13ITEM_FIELD_METADATA\x10\x02\x42\x07\n\x05value\"+\n\tCreateTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xb2\x02\n\tUpdateTag\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0e\n\x06tag_id\x18\x02 \x01(\x0c\x12\x30\n\x06\x61\x63tion\x18\x03 \x01(\x0e\x32 .market.mass.UpdateTag.TagAction\x12\x11\n\x07item_id\x18\x04 \x01(\x0cH\x00\x12\x12\n\x08new_name\x18\x05 \x01(\tH\x00\x12\x10\n\x06\x64\x65lete\x18\x06 \x01(\x08H\x00\"\x8e\x01\n\tTagAction\x12\x1a\n\x16TAG_ACTION_UNSPECIFIED\x10\x00\x12\x17\n\x13TAG_ACTION_ADD_ITEM\x10\x01\x12\x1a\n\x16TAG_ACTION_REMOVE_ITEM\x10\x02\x12\x15\n\x11TAG_ACTION_RENAME\x10\x03\x12\x19\n\x15TAG_ACTION_DELETE_TAG\x10\x04\x42\x07\n\x05value\"b\n\x0b\x43hangeStock\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x10\n\x08item_ids\x18\x02 \x03(\x0c\x12\r\n\x05\x64iffs\x18\x03 \x03(\x11\x12\x0f\n\x07\x63\x61rt_id\x18\x04 \x01(\x0c\x12\x0f\n\x07tx_hash\x18\x05 \x01(\x0c\"Q\n\nNewKeyCard\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x18\n\x10user_wallet_addr\x18\x02 \x01(\x0c\x12\x17\n\x0f\x63\x61rd_public_key\x18\x03 \x01(\x0c\"\x1e\n\nCreateCart\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\"R\n\nChangeCart\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0f\n\x07\x63\x61rt_id\x18\x02 \x01(\x0c\x12\x0f\n\x07item_id\x18\x03 \x01(\x0c\x12\x10\n\x08quantity\x18\x04 \x01(\x11\"\xab\x01\n\rCartFinalized\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0f\n\x07\x63\x61rt_id\x18\x02 \x01(\x0c\x12\x15\n\rpurchase_addr\x18\x03 \x01(\x0c\x12\x12\n\nerc20_addr\x18\x08 \x01(\x0c\x12\x11\n\tsub_total\x18\x04 \x01(\t\x12\x11\n\tsales_tax\x18\x05 \x01(\t\x12\r\n\x05total\x18\x06 \x01(\t\x12\x17\n\x0ftotal_in_crypto\x18\x07 \x01(\t\"2\n\rCartAbandoned\x12\x10\n\x08\x65vent_id\x18\x01 \x01(\x0c\x12\x0f\n\x07\x63\x61rt_id\x18\x02 \x01(\x0c\"\x8c\x05\n\nStoreEvent\x12\x11\n\tsignature\x18\x01 \x01(\x0c\x12\x34\n\x0estore_manifest\x18\x02 \x01(\x0b\x32\x1a.market.mass.StoreManifestH\x00\x12\x41\n\x15update_store_manifest\x18\x03 \x01(\x0b\x32 .market.mass.UpdateStoreManifestH\x00\x12.\n\x0b\x63reate_item\x18\x04 \x01(\x0b\x32\x17.market.mass.CreateItemH\x00\x12.\n\x0bupdate_item\x18\x05 \x01(\x0b\x32\x17.market.mass.UpdateItemH\x00\x12,\n\ncreate_tag\x18\x06 \x01(\x0b\x32\x16.market.mass.CreateTagH\x00\x12,\n\nupdate_tag\x18\x07 \x01(\x0b\x32\x16.market.mass.UpdateTagH\x00\x12.\n\x0b\x63reate_cart\x18\x08 \x01(\x0b\x32\x17.market.mass.CreateCartH\x00\x12.\n\x0b\x63hange_cart\x18\t \x01(\x0b\x32\x17.market.mass.ChangeCartH\x00\x12\x34\n\x0e\x63\x61rt_finalized\x18\n \x01(\x0b\x32\x1a.market.mass.CartFinalizedH\x00\x12\x34\n\x0e\x63\x61rt_abandoned\x18\x0b \x01(\x0b\x32\x1a.market.mass.CartAbandonedH\x00\x12\x30\n\x0c\x63hange_stock\x18\x0c \x01(\x0b\x32\x18.market.mass.ChangeStockH\x00\x12/\n\x0cnew_key_card\x18\r \x01(\x0b\x32\x17.market.mass.NewKeyCardH\x00\x42\x07\n\x05unionb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'store_events_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_STOREMANIFEST']._serialized_start=35
@@ -39,23 +35,21 @@
   _globals['_CREATETAG']._serialized_start=781
   _globals['_CREATETAG']._serialized_end=824
   _globals['_UPDATETAG']._serialized_start=827
   _globals['_UPDATETAG']._serialized_end=1133
   _globals['_UPDATETAG_TAGACTION']._serialized_start=982
   _globals['_UPDATETAG_TAGACTION']._serialized_end=1124
   _globals['_CHANGESTOCK']._serialized_start=1135
-  _globals['_CHANGESTOCK']._serialized_end=1234
-  _globals['_NEWKEYCARD']._serialized_start=1236
-  _globals['_NEWKEYCARD']._serialized_end=1317
-  _globals['_CREATEORDER']._serialized_start=1319
-  _globals['_CREATEORDER']._serialized_end=1350
-  _globals['_UPDATEORDER']._serialized_start=1353
-  _globals['_UPDATEORDER']._serialized_end=1834
-  _globals['_UPDATEORDER_CHANGEITEMS']._serialized_start=1600
-  _globals['_UPDATEORDER_CHANGEITEMS']._serialized_end=1648
-  _globals['_UPDATEORDER_ITEMSFINALIZED']._serialized_start=1651
-  _globals['_UPDATEORDER_ITEMSFINALIZED']._serialized_end=1788
-  _globals['_UPDATEORDER_ORDERCANCELED']._serialized_start=1790
-  _globals['_UPDATEORDER_ORDERCANCELED']._serialized_end=1824
-  _globals['_STOREEVENT']._serialized_start=1837
-  _globals['_STOREEVENT']._serialized_end=2385
+  _globals['_CHANGESTOCK']._serialized_end=1233
+  _globals['_NEWKEYCARD']._serialized_start=1235
+  _globals['_NEWKEYCARD']._serialized_end=1316
+  _globals['_CREATECART']._serialized_start=1318
+  _globals['_CREATECART']._serialized_end=1348
+  _globals['_CHANGECART']._serialized_start=1350
+  _globals['_CHANGECART']._serialized_end=1432
+  _globals['_CARTFINALIZED']._serialized_start=1435
+  _globals['_CARTFINALIZED']._serialized_end=1606
+  _globals['_CARTABANDONED']._serialized_start=1608
+  _globals['_CARTABANDONED']._serialized_end=1658
+  _globals['_STOREEVENT']._serialized_start=1661
+  _globals['_STOREEVENT']._serialized_end=2313
 # @@protoc_insertion_point(module_scope)
```

### Comparing `massmarket_hash_event-0.1.2/massmarket_hash_event/store_events_pb2.pyi` & `massmarket_hash_event-0.1.5/massmarket_hash_event/store_events_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# SPDX-FileCopyrightText: 2024 Mass Labs
-#
-# SPDX-License-Identifier: MIT
-
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
@@ -113,102 +109,105 @@
     action: UpdateTag.TagAction
     item_id: bytes
     new_name: str
     delete: bool
     def __init__(self, event_id: _Optional[bytes] = ..., tag_id: _Optional[bytes] = ..., action: _Optional[_Union[UpdateTag.TagAction, str]] = ..., item_id: _Optional[bytes] = ..., new_name: _Optional[str] = ..., delete: bool = ...) -> None: ...
 
 class ChangeStock(_message.Message):
-    __slots__ = ["event_id", "item_ids", "diffs", "order_id", "tx_hash"]
+    __slots__ = ["event_id", "item_ids", "diffs", "cart_id", "tx_hash"]
     EVENT_ID_FIELD_NUMBER: _ClassVar[int]
     ITEM_IDS_FIELD_NUMBER: _ClassVar[int]
     DIFFS_FIELD_NUMBER: _ClassVar[int]
-    ORDER_ID_FIELD_NUMBER: _ClassVar[int]
+    CART_ID_FIELD_NUMBER: _ClassVar[int]
     TX_HASH_FIELD_NUMBER: _ClassVar[int]
     event_id: bytes
     item_ids: _containers.RepeatedScalarFieldContainer[bytes]
     diffs: _containers.RepeatedScalarFieldContainer[int]
-    order_id: bytes
+    cart_id: bytes
     tx_hash: bytes
-    def __init__(self, event_id: _Optional[bytes] = ..., item_ids: _Optional[_Iterable[bytes]] = ..., diffs: _Optional[_Iterable[int]] = ..., order_id: _Optional[bytes] = ..., tx_hash: _Optional[bytes] = ...) -> None: ...
+    def __init__(self, event_id: _Optional[bytes] = ..., item_ids: _Optional[_Iterable[bytes]] = ..., diffs: _Optional[_Iterable[int]] = ..., cart_id: _Optional[bytes] = ..., tx_hash: _Optional[bytes] = ...) -> None: ...
 
 class NewKeyCard(_message.Message):
     __slots__ = ["event_id", "user_wallet_addr", "card_public_key"]
     EVENT_ID_FIELD_NUMBER: _ClassVar[int]
     USER_WALLET_ADDR_FIELD_NUMBER: _ClassVar[int]
     CARD_PUBLIC_KEY_FIELD_NUMBER: _ClassVar[int]
     event_id: bytes
     user_wallet_addr: bytes
     card_public_key: bytes
     def __init__(self, event_id: _Optional[bytes] = ..., user_wallet_addr: _Optional[bytes] = ..., card_public_key: _Optional[bytes] = ...) -> None: ...
 
-class CreateOrder(_message.Message):
+class CreateCart(_message.Message):
     __slots__ = ["event_id"]
     EVENT_ID_FIELD_NUMBER: _ClassVar[int]
     event_id: bytes
     def __init__(self, event_id: _Optional[bytes] = ...) -> None: ...
 
-class UpdateOrder(_message.Message):
-    __slots__ = ["event_id", "order_id", "change_items", "items_finalized", "order_canceled"]
-    class ChangeItems(_message.Message):
-        __slots__ = ["item_id", "quantity"]
-        ITEM_ID_FIELD_NUMBER: _ClassVar[int]
-        QUANTITY_FIELD_NUMBER: _ClassVar[int]
-        item_id: bytes
-        quantity: int
-        def __init__(self, item_id: _Optional[bytes] = ..., quantity: _Optional[int] = ...) -> None: ...
-    class ItemsFinalized(_message.Message):
-        __slots__ = ["purchase_addr", "erc20_addr", "sub_total", "sales_tax", "total", "total_in_crypto"]
-        PURCHASE_ADDR_FIELD_NUMBER: _ClassVar[int]
-        ERC20_ADDR_FIELD_NUMBER: _ClassVar[int]
-        SUB_TOTAL_FIELD_NUMBER: _ClassVar[int]
-        SALES_TAX_FIELD_NUMBER: _ClassVar[int]
-        TOTAL_FIELD_NUMBER: _ClassVar[int]
-        TOTAL_IN_CRYPTO_FIELD_NUMBER: _ClassVar[int]
-        purchase_addr: bytes
-        erc20_addr: bytes
-        sub_total: str
-        sales_tax: str
-        total: str
-        total_in_crypto: str
-        def __init__(self, purchase_addr: _Optional[bytes] = ..., erc20_addr: _Optional[bytes] = ..., sub_total: _Optional[str] = ..., sales_tax: _Optional[str] = ..., total: _Optional[str] = ..., total_in_crypto: _Optional[str] = ...) -> None: ...
-    class OrderCanceled(_message.Message):
-        __slots__ = ["timestamp"]
-        TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
-        timestamp: int
-        def __init__(self, timestamp: _Optional[int] = ...) -> None: ...
-    EVENT_ID_FIELD_NUMBER: _ClassVar[int]
-    ORDER_ID_FIELD_NUMBER: _ClassVar[int]
-    CHANGE_ITEMS_FIELD_NUMBER: _ClassVar[int]
-    ITEMS_FINALIZED_FIELD_NUMBER: _ClassVar[int]
-    ORDER_CANCELED_FIELD_NUMBER: _ClassVar[int]
-    event_id: bytes
-    order_id: bytes
-    change_items: UpdateOrder.ChangeItems
-    items_finalized: UpdateOrder.ItemsFinalized
-    order_canceled: UpdateOrder.OrderCanceled
-    def __init__(self, event_id: _Optional[bytes] = ..., order_id: _Optional[bytes] = ..., change_items: _Optional[_Union[UpdateOrder.ChangeItems, _Mapping]] = ..., items_finalized: _Optional[_Union[UpdateOrder.ItemsFinalized, _Mapping]] = ..., order_canceled: _Optional[_Union[UpdateOrder.OrderCanceled, _Mapping]] = ...) -> None: ...
+class ChangeCart(_message.Message):
+    __slots__ = ["event_id", "cart_id", "item_id", "quantity"]
+    EVENT_ID_FIELD_NUMBER: _ClassVar[int]
+    CART_ID_FIELD_NUMBER: _ClassVar[int]
+    ITEM_ID_FIELD_NUMBER: _ClassVar[int]
+    QUANTITY_FIELD_NUMBER: _ClassVar[int]
+    event_id: bytes
+    cart_id: bytes
+    item_id: bytes
+    quantity: int
+    def __init__(self, event_id: _Optional[bytes] = ..., cart_id: _Optional[bytes] = ..., item_id: _Optional[bytes] = ..., quantity: _Optional[int] = ...) -> None: ...
+
+class CartFinalized(_message.Message):
+    __slots__ = ["event_id", "cart_id", "purchase_addr", "erc20_addr", "sub_total", "sales_tax", "total", "total_in_crypto"]
+    EVENT_ID_FIELD_NUMBER: _ClassVar[int]
+    CART_ID_FIELD_NUMBER: _ClassVar[int]
+    PURCHASE_ADDR_FIELD_NUMBER: _ClassVar[int]
+    ERC20_ADDR_FIELD_NUMBER: _ClassVar[int]
+    SUB_TOTAL_FIELD_NUMBER: _ClassVar[int]
+    SALES_TAX_FIELD_NUMBER: _ClassVar[int]
+    TOTAL_FIELD_NUMBER: _ClassVar[int]
+    TOTAL_IN_CRYPTO_FIELD_NUMBER: _ClassVar[int]
+    event_id: bytes
+    cart_id: bytes
+    purchase_addr: bytes
+    erc20_addr: bytes
+    sub_total: str
+    sales_tax: str
+    total: str
+    total_in_crypto: str
+    def __init__(self, event_id: _Optional[bytes] = ..., cart_id: _Optional[bytes] = ..., purchase_addr: _Optional[bytes] = ..., erc20_addr: _Optional[bytes] = ..., sub_total: _Optional[str] = ..., sales_tax: _Optional[str] = ..., total: _Optional[str] = ..., total_in_crypto: _Optional[str] = ...) -> None: ...
+
+class CartAbandoned(_message.Message):
+    __slots__ = ["event_id", "cart_id"]
+    EVENT_ID_FIELD_NUMBER: _ClassVar[int]
+    CART_ID_FIELD_NUMBER: _ClassVar[int]
+    event_id: bytes
+    cart_id: bytes
+    def __init__(self, event_id: _Optional[bytes] = ..., cart_id: _Optional[bytes] = ...) -> None: ...
 
 class StoreEvent(_message.Message):
-    __slots__ = ["signature", "store_manifest", "update_store_manifest", "create_item", "update_item", "create_tag", "update_tag", "create_order", "update_order", "change_stock", "new_key_card"]
+    __slots__ = ["signature", "store_manifest", "update_store_manifest", "create_item", "update_item", "create_tag", "update_tag", "create_cart", "change_cart", "cart_finalized", "cart_abandoned", "change_stock", "new_key_card"]
     SIGNATURE_FIELD_NUMBER: _ClassVar[int]
     STORE_MANIFEST_FIELD_NUMBER: _ClassVar[int]
     UPDATE_STORE_MANIFEST_FIELD_NUMBER: _ClassVar[int]
     CREATE_ITEM_FIELD_NUMBER: _ClassVar[int]
     UPDATE_ITEM_FIELD_NUMBER: _ClassVar[int]
     CREATE_TAG_FIELD_NUMBER: _ClassVar[int]
     UPDATE_TAG_FIELD_NUMBER: _ClassVar[int]
-    CREATE_ORDER_FIELD_NUMBER: _ClassVar[int]
-    UPDATE_ORDER_FIELD_NUMBER: _ClassVar[int]
+    CREATE_CART_FIELD_NUMBER: _ClassVar[int]
+    CHANGE_CART_FIELD_NUMBER: _ClassVar[int]
+    CART_FINALIZED_FIELD_NUMBER: _ClassVar[int]
+    CART_ABANDONED_FIELD_NUMBER: _ClassVar[int]
     CHANGE_STOCK_FIELD_NUMBER: _ClassVar[int]
     NEW_KEY_CARD_FIELD_NUMBER: _ClassVar[int]
     signature: bytes
     store_manifest: StoreManifest
     update_store_manifest: UpdateStoreManifest
     create_item: CreateItem
     update_item: UpdateItem
     create_tag: CreateTag
     update_tag: UpdateTag
-    create_order: CreateOrder
-    update_order: UpdateOrder
+    create_cart: CreateCart
+    change_cart: ChangeCart
+    cart_finalized: CartFinalized
+    cart_abandoned: CartAbandoned
     change_stock: ChangeStock
     new_key_card: NewKeyCard
-    def __init__(self, signature: _Optional[bytes] = ..., store_manifest: _Optional[_Union[StoreManifest, _Mapping]] = ..., update_store_manifest: _Optional[_Union[UpdateStoreManifest, _Mapping]] = ..., create_item: _Optional[_Union[CreateItem, _Mapping]] = ..., update_item: _Optional[_Union[UpdateItem, _Mapping]] = ..., create_tag: _Optional[_Union[CreateTag, _Mapping]] = ..., update_tag: _Optional[_Union[UpdateTag, _Mapping]] = ..., create_order: _Optional[_Union[CreateOrder, _Mapping]] = ..., update_order: _Optional[_Union[UpdateOrder, _Mapping]] = ..., change_stock: _Optional[_Union[ChangeStock, _Mapping]] = ..., new_key_card: _Optional[_Union[NewKeyCard, _Mapping]] = ...) -> None: ...
+    def __init__(self, signature: _Optional[bytes] = ..., store_manifest: _Optional[_Union[StoreManifest, _Mapping]] = ..., update_store_manifest: _Optional[_Union[UpdateStoreManifest, _Mapping]] = ..., create_item: _Optional[_Union[CreateItem, _Mapping]] = ..., update_item: _Optional[_Union[UpdateItem, _Mapping]] = ..., create_tag: _Optional[_Union[CreateTag, _Mapping]] = ..., update_tag: _Optional[_Union[UpdateTag, _Mapping]] = ..., create_cart: _Optional[_Union[CreateCart, _Mapping]] = ..., change_cart: _Optional[_Union[ChangeCart, _Mapping]] = ..., cart_finalized: _Optional[_Union[CartFinalized, _Mapping]] = ..., cart_abandoned: _Optional[_Union[CartAbandoned, _Mapping]] = ..., change_stock: _Optional[_Union[ChangeStock, _Mapping]] = ..., new_key_card: _Optional[_Union[NewKeyCard, _Mapping]] = ...) -> None: ...
```

### Comparing `massmarket_hash_event-0.1.2/massmarket_hash_event/store_requests_pb2.py` & `massmarket_hash_event-0.1.5/massmarket_hash_event/store_requests_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# SPDX-FileCopyrightText: 2024 Mass Labs
-#
-# SPDX-License-Identifier: MIT
-
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: store_requests.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
@@ -14,23 +10,23 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from massmarket_hash_event import error_pb2 as error__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14store_requests.proto\x12\x0bmarket.mass\x1a\x0b\x65rror.proto\"U\n\x19\x43ommitItemsToOrderRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\x10\n\x08order_id\x18\x02 \x01(\x0c\x12\x12\n\nerc20_addr\x18\x03 \x01(\x0c\"n\n\x1a\x43ommitItemsToOrderResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\x12\x19\n\x11\x63\x61rt_finalized_id\x18\x03 \x01(\x0c\"-\n\x17GetBlobUploadURLRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\"^\n\x18GetBlobUploadURLResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\x12\x0b\n\x03url\x18\x03 \x01(\tb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14store_requests.proto\x12\x0bmarket.mass\x1a\x0b\x65rror.proto\"L\n\x11\x43ommitCartRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12\x0f\n\x07\x63\x61rt_id\x18\x02 \x01(\x0c\x12\x12\n\nerc20_addr\x18\x03 \x01(\x0c\"f\n\x12\x43ommitCartResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\x12\x19\n\x11\x63\x61rt_finalized_id\x18\x03 \x01(\x0c\"-\n\x17GetBlobUploadURLRequest\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\"^\n\x18GetBlobUploadURLResponse\x12\x12\n\nrequest_id\x18\x01 \x01(\x0c\x12!\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x12.market.mass.Error\x12\x0b\n\x03url\x18\x03 \x01(\tb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'store_requests_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
-  _globals['_COMMITITEMSTOORDERREQUEST']._serialized_start=50
-  _globals['_COMMITITEMSTOORDERREQUEST']._serialized_end=135
-  _globals['_COMMITITEMSTOORDERRESPONSE']._serialized_start=137
-  _globals['_COMMITITEMSTOORDERRESPONSE']._serialized_end=247
-  _globals['_GETBLOBUPLOADURLREQUEST']._serialized_start=249
-  _globals['_GETBLOBUPLOADURLREQUEST']._serialized_end=294
-  _globals['_GETBLOBUPLOADURLRESPONSE']._serialized_start=296
-  _globals['_GETBLOBUPLOADURLRESPONSE']._serialized_end=390
+  _globals['_COMMITCARTREQUEST']._serialized_start=50
+  _globals['_COMMITCARTREQUEST']._serialized_end=126
+  _globals['_COMMITCARTRESPONSE']._serialized_start=128
+  _globals['_COMMITCARTRESPONSE']._serialized_end=230
+  _globals['_GETBLOBUPLOADURLREQUEST']._serialized_start=232
+  _globals['_GETBLOBUPLOADURLREQUEST']._serialized_end=277
+  _globals['_GETBLOBUPLOADURLRESPONSE']._serialized_start=279
+  _globals['_GETBLOBUPLOADURLRESPONSE']._serialized_end=373
 # @@protoc_insertion_point(module_scope)
```

### Comparing `massmarket_hash_event-0.1.2/massmarket_hash_event/store_requests_pb2.pyi` & `massmarket_hash_event-0.1.5/massmarket_hash_event/store_requests_pb2.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-# SPDX-FileCopyrightText: 2024 Mass Labs
-#
-# SPDX-License-Identifier: MIT
-
 from massmarket_hash_event import error_pb2 as _error_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class CommitItemsToOrderRequest(_message.Message):
-    __slots__ = ["request_id", "order_id", "erc20_addr"]
+class CommitCartRequest(_message.Message):
+    __slots__ = ["request_id", "cart_id", "erc20_addr"]
     REQUEST_ID_FIELD_NUMBER: _ClassVar[int]
-    ORDER_ID_FIELD_NUMBER: _ClassVar[int]
+    CART_ID_FIELD_NUMBER: _ClassVar[int]
     ERC20_ADDR_FIELD_NUMBER: _ClassVar[int]
     request_id: bytes
-    order_id: bytes
+    cart_id: bytes
     erc20_addr: bytes
-    def __init__(self, request_id: _Optional[bytes] = ..., order_id: _Optional[bytes] = ..., erc20_addr: _Optional[bytes] = ...) -> None: ...
+    def __init__(self, request_id: _Optional[bytes] = ..., cart_id: _Optional[bytes] = ..., erc20_addr: _Optional[bytes] = ...) -> None: ...
 
-class CommitItemsToOrderResponse(_message.Message):
+class CommitCartResponse(_message.Message):
     __slots__ = ["request_id", "error", "cart_finalized_id"]
     REQUEST_ID_FIELD_NUMBER: _ClassVar[int]
     ERROR_FIELD_NUMBER: _ClassVar[int]
     CART_FINALIZED_ID_FIELD_NUMBER: _ClassVar[int]
     request_id: bytes
     error: _error_pb2.Error
     cart_finalized_id: bytes
```

### Comparing `massmarket_hash_event-0.1.2/massmarket_hash_event/transport_pb2.py` & `massmarket_hash_event-0.1.5/massmarket_hash_event/transport_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# SPDX-FileCopyrightText: 2024 Mass Labs
-#
-# SPDX-License-Identifier: MIT
-
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: transport.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
```

### Comparing `massmarket_hash_event-0.1.2/massmarket_hash_event/transport_pb2.pyi` & `massmarket_hash_event-0.1.5/massmarket_hash_event/transport_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# SPDX-FileCopyrightText: 2024 Mass Labs
-#
-# SPDX-License-Identifier: MIT
-
 from google.protobuf import any_pb2 as _any_pb2
 from massmarket_hash_event import error_pb2 as _error_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
```

### Comparing `massmarket_hash_event-0.1.2/massmarket_hash_event/typedData.json` & `massmarket_hash_event-0.1.5/massmarket_hash_event/typedData.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5696428571428571%*

 * *Differences: {"'CartAbandoned'": "[OrderedDict([('name', 'event_id'), ('type', 'bytes32')]), "*

 * *                    "OrderedDict([('name', 'cart_id'), ('type', 'bytes32')])]",*

 * * "'CartFinalized'": "[OrderedDict([('name', 'event_id'), ('type', 'bytes32')]), "*

 * *                    "OrderedDict([('name', 'cart_id'), ('type', 'bytes32')]), "*

 * *                    "OrderedDict([('name', 'purchase_addr'), ('type', 'address')]), "*

 * *                    "OrderedDict([('name', 'erc20_addr'), ('type', 'address')]), "*

 * *                    […]*

```diff
@@ -1,50 +1,112 @@
 {
+    "CartAbandoned": [
+        {
+            "name": "event_id",
+            "type": "bytes32"
+        },
+        {
+            "name": "cart_id",
+            "type": "bytes32"
+        }
+    ],
+    "CartFinalized": [
+        {
+            "name": "event_id",
+            "type": "bytes32"
+        },
+        {
+            "name": "cart_id",
+            "type": "bytes32"
+        },
+        {
+            "name": "purchase_addr",
+            "type": "address"
+        },
+        {
+            "name": "erc20_addr",
+            "type": "address"
+        },
+        {
+            "name": "sub_total",
+            "type": "string"
+        },
+        {
+            "name": "sales_tax",
+            "type": "string"
+        },
+        {
+            "name": "total",
+            "type": "string"
+        },
+        {
+            "name": "total_in_crypto",
+            "type": "string"
+        }
+    ],
+    "ChangeCart": [
+        {
+            "name": "event_id",
+            "type": "bytes32"
+        },
+        {
+            "name": "cart_id",
+            "type": "bytes32"
+        },
+        {
+            "name": "item_id",
+            "type": "bytes32"
+        },
+        {
+            "name": "quantity",
+            "type": "int32"
+        }
+    ],
     "ChangeStock": [
         {
             "name": "event_id",
             "type": "bytes32"
         },
         {
             "name": "item_ids",
             "type": "bytes32[]"
         },
         {
             "name": "diffs",
             "type": "int32[]"
         },
         {
-            "name": "order_id",
+            "name": "cart_id",
             "type": "bytes32"
         },
         {
             "name": "tx_hash",
             "type": "bytes32"
         }
     ],
+    "CreateCart": [
+        {
+            "name": "event_id",
+            "type": "bytes32"
+        }
+    ],
     "CreateItem": [
         {
             "name": "event_id",
             "type": "bytes32"
         },
         {
             "name": "price",
             "type": "string"
         },
         {
             "name": "metadata",
             "type": "bytes"
         }
     ],
-    "CreateOrder": [
-        {
-            "name": "event_id",
-            "type": "bytes32"
-        }
-    ],
     "CreateTag": [
         {
             "name": "event_id",
             "type": "bytes32"
         },
         {
             "name": "name",
@@ -101,75 +163,14 @@
             "type": "string"
         },
         {
             "name": "metadata",
             "type": "bytes"
         }
     ],
-    "UpdateOrder": [
-        {
-            "name": "event_id",
-            "type": "bytes32"
-        },
-        {
-            "name": "order_id",
-            "type": "bytes32"
-        },
-        {
-            "message": [
-                {
-                    "name": "item_id",
-                    "type": "bytes32"
-                },
-                {
-                    "name": "quantity",
-                    "type": "int32"
-                }
-            ],
-            "name": "change_items"
-        },
-        {
-            "message": [
-                {
-                    "name": "purchase_addr",
-                    "type": "address"
-                },
-                {
-                    "name": "erc20_addr",
-                    "type": "address"
-                },
-                {
-                    "name": "sub_total",
-                    "type": "string"
-                },
-                {
-                    "name": "sales_tax",
-                    "type": "string"
-                },
-                {
-                    "name": "total",
-                    "type": "string"
-                },
-                {
-                    "name": "total_in_crypto",
-                    "type": "string"
-                }
-            ],
-            "name": "items_finalized"
-        },
-        {
-            "message": [
-                {
-                    "name": "timestamp",
-                    "type": "uint64"
-                }
-            ],
-            "name": "order_canceled"
-        }
-    ],
     "UpdateStoreManifest": [
         {
             "name": "event_id",
             "type": "bytes32"
         },
         {
             "name": "field",
```

### Comparing `massmarket_hash_event-0.1.2/massmarket_hash_event.egg-info/PKG-INFO` & `massmarket_hash_event-0.1.5/massmarket_hash_event.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: massmarket-hash-event
-Version: 0.1.2
+Version: 0.1.5
 Summary: Helper functions to hash events for signature creation and verification on Mass Market.
 Author-email: Henry Bubert <henry@mass.market>
 License: MIT
 Project-URL: Homepage, https://mass.market
 Project-URL: Repository, https://github.com/masslbs/network-schema.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `massmarket_hash_event-0.1.2/massmarket_hash_event.egg-info/SOURCES.txt` & `massmarket_hash_event-0.1.5/massmarket_hash_event.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `massmarket_hash_event-0.1.2/pyproject.toml` & `massmarket_hash_event-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "massmarket_hash_event"
-version = "0.1.2"
+version = "0.1.5"
 authors = [
     {name = "Henry Bubert", email = "henry@mass.market"},
 ]
 description = "Helper functions to hash events for signature creation and verification on Mass Market."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `massmarket_hash_event-0.1.2/tests/test_encode.py` & `massmarket_hash_event-0.1.5/tests/test_encode.py`

 * *Files identical despite different names*

### Comparing `massmarket_hash_event-0.1.2/tests/test_signatures.py` & `massmarket_hash_event-0.1.5/tests/test_signatures.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,26 +43,31 @@
 
     (store_events_pb2.StoreEvent(create_tag=store_events_pb2.CreateTag()),
       "0xa517d7d534cba5e6ebaf002fe765653cbd7beb9cf035641f9c9d1f0b5d3bed74"),
 
     (store_events_pb2.StoreEvent(update_tag=store_events_pb2.UpdateTag(action=store_events_pb2.UpdateTag.TAG_ACTION_ADD_ITEM)),
       "0xa8b3551e44d5020bc5dd518f15a9876bc3aa3e6cffad959654664fd7d6b798d3"),
 
-    (store_events_pb2.StoreEvent(create_order=store_events_pb2.CreateOrder()),
-      "0x94b3409f62d4be96bbcc399b8eb153e331607e569f1993eadb24f715c86cd2e3"),
+    (store_events_pb2.StoreEvent(create_cart=store_events_pb2.CreateCart()),
+      "0x86d113747e19f65535e20f14ca9526e683bd0255e4b8fdaaffa87e0e1a840854"),
 
-    (store_events_pb2.StoreEvent(update_order=store_events_pb2.UpdateOrder(
-      order_canceled=store_events_pb2.UpdateOrder.OrderCanceled(timestamp=1))),
-      "0x3ec3e627a9912a1f7bf17e33107870af946f39ecd5a8545c5cadfa588fe61982"),
+    (store_events_pb2.StoreEvent(change_cart=store_events_pb2.ChangeCart()),
+      "0xe033b1f86a7ebe1eacdbfb332c6fe7ea0294d1eebff55b5910a248d3d2baff2b"),
+
+    (store_events_pb2.StoreEvent(cart_finalized=store_events_pb2.CartFinalized(purchase_addr=random.randbytes(20))),
+      "0xb890ad659de9ae16576c7a6b0267ccdca64e7f771cf8853f6f33b411118ed559"),
+
+    (store_events_pb2.StoreEvent(cart_abandoned=store_events_pb2.CartAbandoned()),
+      "0xaeb33fbed4304027350b36c723fba123e9c954422617595ec29e7c86730aa986"),
 
     (store_events_pb2.StoreEvent(change_stock=store_events_pb2.ChangeStock()),
       "0x06dda3da556003d920246f05238d29717768408673ebc209de3fd128391cf4d8"),
 
     (store_events_pb2.StoreEvent(new_key_card=store_events_pb2.NewKeyCard(user_wallet_addr=random.randbytes(20))),
-      "0x9260d6e77645cb1245264138f9320d28a096cdffdc2a085ccb65490a24138a7d")
+      "0xbbdc5122897f0772c86eb5b79bbc6d8c5cf917886c8138678f4c9b2ff4495a21")
   ]
   for idx, (evt, expected) in enumerate(events):
     data = h.hash_event(evt)
     signed_message = pk.sign_message(data)
     msg_hash = signed_message.messageHash.hex()
     evt_name = evt.WhichOneof("union")
     assert msg_hash == expected, f"Failed on event {idx} ({evt_name})"
```

