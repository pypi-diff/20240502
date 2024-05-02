# Comparing `tmp/dig_ass_chat_protos-0.0.9.tar.gz` & `tmp/dig_ass_chat_protos-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_chat_protos-0.0.9.tar", last modified: Mon Apr 15 21:06:09 2024, max compression
+gzip compressed data, was "dig_ass_chat_protos-1.0.0.tar", last modified: Thu May  2 11:13:02 2024, max compression
```

## Comparing `dig_ass_chat_protos-0.0.9.tar` & `dig_ass_chat_protos-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-15 21:06:09.119659 dig_ass_chat_protos-0.0.9/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.9/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-15 21:06:09.119659 dig_ass_chat_protos-0.0.9/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:15.000000 dig_ass_chat_protos-0.0.9/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-15 21:06:09.119659 dig_ass_chat_protos-0.0.9/dig_ass_chat_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2119 2024-04-15 21:06:07.000000 dig_ass_chat_protos-0.0.9/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1273 2024-04-15 21:06:07.000000 dig_ass_chat_protos-0.0.9/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     3093 2024-04-15 21:06:07.000000 dig_ass_chat_protos-0.0.9/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-15 21:05:22.000000 dig_ass_chat_protos-0.0.9/dig_ass_chat_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      389 2024-04-12 20:28:20.000000 dig_ass_chat_protos-0.0.9/dig_ass_chat_protos/abstract_client.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      916 2024-04-15 21:01:32.000000 dig_ass_chat_protos-0.0.9/dig_ass_chat_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-15 21:06:09.119659 dig_ass_chat_protos-0.0.9/dig_ass_chat_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-15 21:06:09.000000 dig_ass_chat_protos-0.0.9/dig_ass_chat_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      533 2024-04-15 21:06:09.000000 dig_ass_chat_protos-0.0.9/dig_ass_chat_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-15 21:06:09.000000 dig_ass_chat_protos-0.0.9/dig_ass_chat_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-15 21:06:09.000000 dig_ass_chat_protos-0.0.9/dig_ass_chat_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-04-15 21:06:09.000000 dig_ass_chat_protos-0.0.9/dig_ass_chat_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_chat_protos-0.0.9/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-15 21:06:09.119659 dig_ass_chat_protos-0.0.9/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-04-11 10:26:57.000000 dig_ass_chat_protos-0.0.9/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:13:02.127752 dig_ass_chat_protos-1.0.0/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_chat_protos-1.0.0/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-05-02 11:13:02.127752 dig_ass_chat_protos-1.0.0/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:58:15.000000 dig_ass_chat_protos-1.0.0/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:13:02.123752 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2174 2024-05-02 11:13:00.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1377 2024-05-02 11:13:00.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     3102 2024-05-02 11:13:00.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-02 11:09:19.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1095 2024-05-02 11:09:19.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:13:02.127752 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-05-02 11:13:02.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      533 2024-05-02 11:13:02.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-02 11:13:02.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-05-02 11:13:02.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-05-02 11:13:02.000000 dig_ass_chat_protos-1.0.0/dig_ass_chat_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_chat_protos-1.0.0/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-02 11:13:02.127752 dig_ass_chat_protos-1.0.0/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-05-02 11:09:19.000000 dig_ass_chat_protos-1.0.0/setup.py
```

### Comparing `dig_ass_chat_protos-0.0.9/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py` & `dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n5dig_ass_chat_protos/DigitalAssistantChatManager.proto\x12\x0f\x64ig.ass.text.v1\"3\n#DigitalAssistantChatManagerResponse\x12\x0c\n\x04Text\x18\x01 \x01(\t\"k\n\"DigitalAssistantChatManagerRequest\x12\x0c\n\x04Text\x18\x01 \x01(\t\x12\x37\n\x0cOuterContext\x18\x02 \x01(\x0b\x32!.dig.ass.text.v1.OuterContextItem\"O\n\x10OuterContextItem\x12\x0b\n\x03Sex\x18\x01 \x01(\x08\x12\x0b\n\x03\x41ge\x18\x02 \x01(\r\x12\x0e\n\x06UserId\x18\x03 \x01(\x03\x12\x11\n\tSessionId\x18\x04 \x01(\r2\x9b\x01\n\x1b\x44igitalAssistantChatManager\x12|\n\x0fGetTextResponse\x12\x33.dig.ass.text.v1.DigitalAssistantChatManagerRequest\x1a\x34.dig.ass.text.v1.DigitalAssistantChatManagerResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n5dig_ass_chat_protos/DigitalAssistantChatManager.proto\x12\x12\x64ig.ass.manager.v1\"3\n#DigitalAssistantChatManagerResponse\x12\x0c\n\x04Text\x18\x01 \x01(\t\"n\n\"DigitalAssistantChatManagerRequest\x12\x0c\n\x04Text\x18\x01 \x01(\t\x12:\n\x0cOuterContext\x18\x02 \x01(\x0b\x32$.dig.ass.manager.v1.OuterContextItem\"a\n\x10OuterContextItem\x12\x0b\n\x03Sex\x18\x01 \x01(\x08\x12\x0b\n\x03\x41ge\x18\x02 \x01(\r\x12\x0e\n\x06UserId\x18\x03 \x01(\t\x12\x11\n\tSessionId\x18\x04 \x01(\t\x12\x10\n\x08\x43lientId\x18\x05 \x01(\t2\xa2\x01\n\x1b\x44igitalAssistantChatManager\x12\x82\x01\n\x0fGetTextResponse\x12\x36.dig.ass.manager.v1.DigitalAssistantChatManagerRequest\x1a\x37.dig.ass.manager.v1.DigitalAssistantChatManagerResponseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'dig_ass_chat_protos.DigitalAssistantChatManager_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
-  _globals['_DIGITALASSISTANTCHATMANAGERRESPONSE']._serialized_start=74
-  _globals['_DIGITALASSISTANTCHATMANAGERRESPONSE']._serialized_end=125
-  _globals['_DIGITALASSISTANTCHATMANAGERREQUEST']._serialized_start=127
-  _globals['_DIGITALASSISTANTCHATMANAGERREQUEST']._serialized_end=234
-  _globals['_OUTERCONTEXTITEM']._serialized_start=236
-  _globals['_OUTERCONTEXTITEM']._serialized_end=315
-  _globals['_DIGITALASSISTANTCHATMANAGER']._serialized_start=318
-  _globals['_DIGITALASSISTANTCHATMANAGER']._serialized_end=473
+  _globals['_DIGITALASSISTANTCHATMANAGERRESPONSE']._serialized_start=77
+  _globals['_DIGITALASSISTANTCHATMANAGERRESPONSE']._serialized_end=128
+  _globals['_DIGITALASSISTANTCHATMANAGERREQUEST']._serialized_start=130
+  _globals['_DIGITALASSISTANTCHATMANAGERREQUEST']._serialized_end=240
+  _globals['_OUTERCONTEXTITEM']._serialized_start=242
+  _globals['_OUTERCONTEXTITEM']._serialized_end=339
+  _globals['_DIGITALASSISTANTCHATMANAGER']._serialized_start=342
+  _globals['_DIGITALASSISTANTCHATMANAGER']._serialized_end=504
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dig_ass_chat_protos-0.0.9/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi` & `dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/DigitalAssistantChatManager_pb2.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,19 @@
     TEXT_FIELD_NUMBER: _ClassVar[int]
     OUTERCONTEXT_FIELD_NUMBER: _ClassVar[int]
     Text: str
     OuterContext: OuterContextItem
     def __init__(self, Text: _Optional[str] = ..., OuterContext: _Optional[_Union[OuterContextItem, _Mapping]] = ...) -> None: ...
 
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

### Comparing `dig_ass_chat_protos-0.0.9/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py` & `dig_ass_chat_protos-1.0.0/dig_ass_chat_protos/DigitalAssistantChatManager_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.GetTextResponse = channel.unary_unary(
-                '/dig.ass.text.v1.DigitalAssistantChatManager/GetTextResponse',
+                '/dig.ass.manager.v1.DigitalAssistantChatManager/GetTextResponse',
                 request_serializer=dig__ass__chat__protos_dot_DigitalAssistantChatManager__pb2.DigitalAssistantChatManagerRequest.SerializeToString,
                 response_deserializer=dig__ass__chat__protos_dot_DigitalAssistantChatManager__pb2.DigitalAssistantChatManagerResponse.FromString,
                 )
 
 
 class DigitalAssistantChatManagerServicer(object):
     """Missing associated documentation comment in .proto file."""
@@ -36,15 +36,15 @@
             'GetTextResponse': grpc.unary_unary_rpc_method_handler(
                     servicer.GetTextResponse,
                     request_deserializer=dig__ass__chat__protos_dot_DigitalAssistantChatManager__pb2.DigitalAssistantChatManagerRequest.FromString,
                     response_serializer=dig__ass__chat__protos_dot_DigitalAssistantChatManager__pb2.DigitalAssistantChatManagerResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'dig.ass.text.v1.DigitalAssistantChatManager', rpc_method_handlers)
+            'dig.ass.manager.v1.DigitalAssistantChatManager', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class DigitalAssistantChatManager(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -55,12 +55,12 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/dig.ass.text.v1.DigitalAssistantChatManager/GetTextResponse',
+        return grpc.experimental.unary_unary(request, target, '/dig.ass.manager.v1.DigitalAssistantChatManager/GetTextResponse',
             dig__ass__chat__protos_dot_DigitalAssistantChatManager__pb2.DigitalAssistantChatManagerRequest.SerializeToString,
             dig__ass__chat__protos_dot_DigitalAssistantChatManager__pb2.DigitalAssistantChatManagerResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `dig_ass_chat_protos-0.0.9/dig_ass_chat_protos.egg-info/SOURCES.txt` & `dig_ass_chat_protos-1.0.0/dig_ass_chat_protos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dig_ass_chat_protos-0.0.9/setup.py` & `dig_ass_chat_protos-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 import re
 from setuptools import setup, find_packages
 
 from dig_ass_chat_protos import __version__
 
 
 def read(file_path):
-    with io.open(file_path, "r", encoding="utf-8") as f:
+    with io.open(file_path, 'r', encoding='utf-8') as f:
         return f.read()
 
 
-readme = read("README.md")
+readme = read('README.md')
 # вычищаем локальные версии из файла requirements (согласно PEP440)
-requirements = "\n".join(
+requirements = '\n'.join(
     re.findall(
-        r"^([^\s^+]+).*$",
-        read("requirements.txt"),
+        r'^([^\s^+]+).*$',
+        read('requirements.txt'),
         flags=re.MULTILINE,
     )
 )
 
 setup(
     # metadata
-    name="dig_ass_chat_protos",
+    name='dig_ass_chat_protos',
     version=__version__,
-    author="AGI-MED-TEAM",
-    description="Proto files for dig_ass_chat_protos",
+    author='AGI-MED-TEAM',
+    description='Proto files for dig_ass_chat_protos',
     long_description=readme,
     # options
     packages=find_packages(),
-    install_requires="\n".join([requirements]),
+    install_requires='\n'.join([requirements]),
     include_package_data=True,
 )
```

