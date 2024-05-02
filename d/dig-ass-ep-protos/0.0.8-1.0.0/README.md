# Comparing `tmp/dig_ass_ep_protos-0.0.8.tar.gz` & `tmp/dig_ass_ep_protos-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_ep_protos-0.0.8.tar", last modified: Mon Apr 15 20:49:43 2024, max compression
+gzip compressed data, was "dig_ass_ep_protos-1.0.0.tar", last modified: Thu May  2 11:12:45 2024, max compression
```

## Comparing `dig_ass_ep_protos-0.0.8.tar` & `dig_ass_ep_protos-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-15 20:49:43.318575 dig_ass_ep_protos-0.0.8/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-10 09:01:15.000000 dig_ass_ep_protos-0.0.8/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      331 2024-04-15 20:49:43.318575 dig_ass_ep_protos-0.0.8/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-09 19:52:14.000000 dig_ass_ep_protos-0.0.8/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-15 20:49:43.314576 dig_ass_ep_protos-0.0.8/dig_ass_ep_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2166 2024-04-15 20:49:41.000000 dig_ass_ep_protos-0.0.8/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1455 2024-04-15 20:49:41.000000 dig_ass_ep_protos-0.0.8/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     3050 2024-04-15 20:49:41.000000 dig_ass_ep_protos-0.0.8/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-15 20:49:20.000000 dig_ass_ep_protos-0.0.8/dig_ass_ep_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      389 2024-04-12 20:28:21.000000 dig_ass_ep_protos-0.0.8/dig_ass_ep_protos/abstract_client.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      983 2024-04-15 20:46:57.000000 dig_ass_ep_protos-0.0.8/dig_ass_ep_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-15 20:49:43.318575 dig_ass_ep_protos-0.0.8/dig_ass_ep_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      331 2024-04-15 20:49:43.000000 dig_ass_ep_protos-0.0.8/dig_ass_ep_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      508 2024-04-15 20:49:43.000000 dig_ass_ep_protos-0.0.8/dig_ass_ep_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-15 20:49:43.000000 dig_ass_ep_protos-0.0.8/dig_ass_ep_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-15 20:49:43.000000 dig_ass_ep_protos-0.0.8/dig_ass_ep_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       18 2024-04-15 20:49:43.000000 dig_ass_ep_protos-0.0.8/dig_ass_ep_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-09 19:55:06.000000 dig_ass_ep_protos-0.0.8/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-15 20:49:43.318575 dig_ass_ep_protos-0.0.8/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      797 2024-04-11 10:22:56.000000 dig_ass_ep_protos-0.0.8/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:12:45.685662 dig_ass_ep_protos-1.0.0/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-10 09:01:15.000000 dig_ass_ep_protos-1.0.0/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      331 2024-05-02 11:12:45.685662 dig_ass_ep_protos-1.0.0/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-09 19:52:14.000000 dig_ass_ep_protos-1.0.0/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:12:45.685662 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2205 2024-05-02 11:12:44.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1559 2024-05-02 11:12:44.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     3050 2024-05-02 11:12:44.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-02 11:09:18.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:18.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1176 2024-05-02 11:09:18.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:12:45.685662 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      331 2024-05-02 11:12:45.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      508 2024-05-02 11:12:45.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-02 11:12:45.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-05-02 11:12:45.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       18 2024-05-02 11:12:45.000000 dig_ass_ep_protos-1.0.0/dig_ass_ep_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-09 19:55:06.000000 dig_ass_ep_protos-1.0.0/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-02 11:12:45.685662 dig_ass_ep_protos-1.0.0/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      797 2024-05-02 11:09:18.000000 dig_ass_ep_protos-1.0.0/setup.py
```

### Comparing `dig_ass_ep_protos-0.0.8/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py` & `dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n2dig_ass_ep_protos/DigitalAssistantEntryPoint.proto\x12\rdig.ass.ep.v1\"2\n\"DigitalAssistantEntryPointResponse\x12\x0c\n\x04Text\x18\x01 \x01(\t\"\x84\x01\n!DigitalAssistantEntryPointRequest\x12\x0c\n\x04Text\x18\x01 \x01(\t\x12\x35\n\x0cOuterContext\x18\x02 \x01(\x0b\x32\x1f.dig.ass.ep.v1.OuterContextItem\x12\r\n\x05Image\x18\x03 \x01(\x0c\x12\x0b\n\x03PDF\x18\x04 \x01(\x0c\"O\n\x10OuterContextItem\x12\x0b\n\x03Sex\x18\x01 \x01(\x08\x12\x0b\n\x03\x41ge\x18\x02 \x01(\r\x12\x0e\n\x06UserId\x18\x03 \x01(\x03\x12\x11\n\tSessionId\x18\x04 \x01(\r2\x94\x01\n\x1a\x44igitalAssistantEntryPoint\x12v\n\x0fGetTextResponse\x12\x30.dig.ass.ep.v1.DigitalAssistantEntryPointRequest\x1a\x31.dig.ass.ep.v1.DigitalAssistantEntryPointResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n2dig_ass_ep_protos/DigitalAssistantEntryPoint.proto\x12\rdig.ass.ep.v1\"2\n\"DigitalAssistantEntryPointResponse\x12\x0c\n\x04Text\x18\x01 \x01(\t\"\x84\x01\n!DigitalAssistantEntryPointRequest\x12\x0c\n\x04Text\x18\x01 \x01(\t\x12\x35\n\x0cOuterContext\x18\x02 \x01(\x0b\x32\x1f.dig.ass.ep.v1.OuterContextItem\x12\r\n\x05Image\x18\x03 \x01(\x0c\x12\x0b\n\x03PDF\x18\x04 \x01(\x0c\"a\n\x10OuterContextItem\x12\x0b\n\x03Sex\x18\x01 \x01(\x08\x12\x0b\n\x03\x41ge\x18\x02 \x01(\r\x12\x0e\n\x06UserId\x18\x03 \x01(\t\x12\x11\n\tSessionId\x18\x04 \x01(\t\x12\x10\n\x08\x43lientId\x18\x05 \x01(\t2\x94\x01\n\x1a\x44igitalAssistantEntryPoint\x12v\n\x0fGetTextResponse\x12\x30.dig.ass.ep.v1.DigitalAssistantEntryPointRequest\x1a\x31.dig.ass.ep.v1.DigitalAssistantEntryPointResponseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'dig_ass_ep_protos.DigitalAssistantEntryPoint_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_DIGITALASSISTANTENTRYPOINTRESPONSE']._serialized_start=69
   _globals['_DIGITALASSISTANTENTRYPOINTRESPONSE']._serialized_end=119
   _globals['_DIGITALASSISTANTENTRYPOINTREQUEST']._serialized_start=122
   _globals['_DIGITALASSISTANTENTRYPOINTREQUEST']._serialized_end=254
   _globals['_OUTERCONTEXTITEM']._serialized_start=256
-  _globals['_OUTERCONTEXTITEM']._serialized_end=335
-  _globals['_DIGITALASSISTANTENTRYPOINT']._serialized_start=338
-  _globals['_DIGITALASSISTANTENTRYPOINT']._serialized_end=486
+  _globals['_OUTERCONTEXTITEM']._serialized_end=353
+  _globals['_DIGITALASSISTANTENTRYPOINT']._serialized_start=356
+  _globals['_DIGITALASSISTANTENTRYPOINT']._serialized_end=504
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dig_ass_ep_protos-0.0.8/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi` & `dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -19,17 +19,19 @@
     Text: str
     OuterContext: OuterContextItem
     Image: bytes
     PDF: bytes
     def __init__(self, Text: _Optional[str] = ..., OuterContext: _Optional[_Union[OuterContextItem, _Mapping]] = ..., Image: _Optional[bytes] = ..., PDF: _Optional[bytes] = ...) -> None: ...
 
 class OuterContextItem(_message.Message):
-    __slots__ = ("Sex", "Age", "UserId", "SessionId")
+    __slots__ = ("Sex", "Age", "UserId", "SessionId", "ClientId")
     SEX_FIELD_NUMBER: _ClassVar[int]
     AGE_FIELD_NUMBER: _ClassVar[int]
     USERID_FIELD_NUMBER: _ClassVar[int]
     SESSIONID_FIELD_NUMBER: _ClassVar[int]
+    CLIENTID_FIELD_NUMBER: _ClassVar[int]
     Sex: bool
     Age: int
-    UserId: int
-    SessionId: int
-    def __init__(self, Sex: bool = ..., Age: _Optional[int] = ..., UserId: _Optional[int] = ..., SessionId: _Optional[int] = ...) -> None: ...
+    UserId: str
+    SessionId: str
+    ClientId: str
+    def __init__(self, Sex: bool = ..., Age: _Optional[int] = ..., UserId: _Optional[str] = ..., SessionId: _Optional[str] = ..., ClientId: _Optional[str] = ...) -> None: ...
```

### Comparing `dig_ass_ep_protos-0.0.8/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py` & `dig_ass_ep_protos-1.0.0/dig_ass_ep_protos/DigitalAssistantEntryPoint_pb2_grpc.py`

 * *Files identical despite different names*

