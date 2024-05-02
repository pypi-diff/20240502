# Comparing `tmp/dig_ass_text_protos-0.0.6.tar.gz` & `tmp/dig_ass_text_protos-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dig_ass_text_protos-0.0.6.tar", last modified: Wed Apr 17 17:57:30 2024, max compression
+gzip compressed data, was "dig_ass_text_protos-1.0.0.tar", last modified: Thu May  2 11:13:18 2024, max compression
```

## Comparing `dig_ass_text_protos-0.0.6.tar` & `dig_ass_text_protos-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-17 17:57:30.496836 dig_ass_text_protos-0.0.6/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_text_protos-0.0.6/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-17 17:57:30.496836 dig_ass_text_protos-0.0.6/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:59:00.000000 dig_ass_text_protos-0.0.6/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-17 17:57:30.492836 dig_ass_text_protos-0.0.6/dig_ass_text_protos/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2725 2024-04-17 17:57:29.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos/DigitalAssistantText_pb2.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2366 2024-04-17 17:57:29.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos/DigitalAssistantText_pb2.pyi
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2946 2024-04-17 17:57:29.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-04-17 17:56:53.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      389 2024-04-12 20:28:21.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos/abstract_client.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     1307 2024-04-17 17:55:45.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos/client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-04-17 17:57:30.492836 dig_ass_text_protos-0.0.6/dig_ass_text_protos.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-04-17 17:57:30.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      512 2024-04-17 17:57:30.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-04-17 17:57:30.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-17 17:57:30.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-04-17 17:57:30.000000 dig_ass_text_protos-0.0.6/dig_ass_text_protos.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_text_protos-0.0.6/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-04-17 17:57:30.496836 dig_ass_text_protos-0.0.6/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-04-11 10:26:57.000000 dig_ass_text_protos-0.0.6/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:13:18.417823 dig_ass_text_protos-1.0.0/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-04-11 10:17:28.000000 dig_ass_text_protos-1.0.0/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-05-02 11:13:18.417823 dig_ass_text_protos-1.0.0/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      139 2024-04-11 09:59:00.000000 dig_ass_text_protos-1.0.0/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:13:18.413822 dig_ass_text_protos-1.0.0/dig_ass_text_protos/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2764 2024-05-02 11:13:17.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos/DigitalAssistantText_pb2.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2470 2024-05-02 11:13:17.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos/DigitalAssistantText_pb2.pyi
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2946 2024-05-02 11:13:17.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-02 11:09:19.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-02 11:09:19.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos/abstract_client.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     1647 2024-05-02 11:09:19.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos/client.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-02 11:13:18.417823 dig_ass_text_protos-1.0.0/dig_ass_text_protos.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      335 2024-05-02 11:13:18.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      512 2024-05-02 11:13:18.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-02 11:13:18.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-05-02 11:13:18.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       20 2024-05-02 11:13:18.000000 dig_ass_text_protos-1.0.0/dig_ass_text_protos.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       36 2024-04-11 10:17:28.000000 dig_ass_text_protos-1.0.0/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-02 11:13:18.417823 dig_ass_text_protos-1.0.0/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      803 2024-05-02 11:09:19.000000 dig_ass_text_protos-1.0.0/setup.py
```

### Comparing `dig_ass_text_protos-0.0.6/dig_ass_text_protos/DigitalAssistantText_pb2.py` & `dig_ass_text_protos-1.0.0/dig_ass_text_protos/DigitalAssistantText_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.dig_ass_text_protos/DigitalAssistantText.proto\x12\x0f\x64ig.ass.text.v1\",\n\x1c\x44igitalAssistantTextResponse\x12\x0c\n\x04Text\x18\x01 \x01(\t\"T\n\x1b\x44igitalAssistantTextRequest\x12\x0c\n\x04Text\x18\x01 \x01(\t\x12\'\n\x04\x43hat\x18\x02 \x01(\x0b\x32\x19.dig.ass.text.v1.ChatItem\"|\n\x08\x43hatItem\x12\x37\n\x0cOuterContext\x18\x01 \x01(\x0b\x32!.dig.ass.text.v1.OuterContextItem\x12\x37\n\x0cInnerContext\x18\x02 \x01(\x0b\x32!.dig.ass.text.v1.InnerContextItem\"O\n\x10OuterContextItem\x12\x0b\n\x03Sex\x18\x01 \x01(\x08\x12\x0b\n\x03\x41ge\x18\x02 \x01(\r\x12\x0e\n\x06UserId\x18\x03 \x01(\x03\x12\x11\n\tSessionId\x18\x04 \x01(\r\"B\n\x10InnerContextItem\x12.\n\x08Replicas\x18\x01 \x03(\x0b\x32\x1c.dig.ass.text.v1.ReplicaItem\";\n\x0bReplicaItem\x12\x0c\n\x04\x42ody\x18\x01 \x01(\t\x12\x0c\n\x04Role\x18\x02 \x01(\x08\x12\x10\n\x08\x44\x61teTime\x18\x03 \x01(\t2\x86\x01\n\x14\x44igitalAssistantText\x12n\n\x0fGetTextResponse\x12,.dig.ass.text.v1.DigitalAssistantTextRequest\x1a-.dig.ass.text.v1.DigitalAssistantTextResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.dig_ass_text_protos/DigitalAssistantText.proto\x12\x0f\x64ig.ass.text.v1\",\n\x1c\x44igitalAssistantTextResponse\x12\x0c\n\x04Text\x18\x01 \x01(\t\"T\n\x1b\x44igitalAssistantTextRequest\x12\x0c\n\x04Text\x18\x01 \x01(\t\x12\'\n\x04\x43hat\x18\x02 \x01(\x0b\x32\x19.dig.ass.text.v1.ChatItem\"|\n\x08\x43hatItem\x12\x37\n\x0cOuterContext\x18\x01 \x01(\x0b\x32!.dig.ass.text.v1.OuterContextItem\x12\x37\n\x0cInnerContext\x18\x02 \x01(\x0b\x32!.dig.ass.text.v1.InnerContextItem\"a\n\x10OuterContextItem\x12\x0b\n\x03Sex\x18\x01 \x01(\x08\x12\x0b\n\x03\x41ge\x18\x02 \x01(\r\x12\x0e\n\x06UserId\x18\x03 \x01(\t\x12\x11\n\tSessionId\x18\x04 \x01(\t\x12\x10\n\x08\x43lientId\x18\x05 \x01(\t\"B\n\x10InnerContextItem\x12.\n\x08Replicas\x18\x01 \x03(\x0b\x32\x1c.dig.ass.text.v1.ReplicaItem\";\n\x0bReplicaItem\x12\x0c\n\x04\x42ody\x18\x01 \x01(\t\x12\x0c\n\x04Role\x18\x02 \x01(\x08\x12\x10\n\x08\x44\x61teTime\x18\x03 \x01(\t2\x86\x01\n\x14\x44igitalAssistantText\x12n\n\x0fGetTextResponse\x12,.dig.ass.text.v1.DigitalAssistantTextRequest\x1a-.dig.ass.text.v1.DigitalAssistantTextResponseb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'dig_ass_text_protos.DigitalAssistantText_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_DIGITALASSISTANTTEXTRESPONSE']._serialized_start=67
   _globals['_DIGITALASSISTANTTEXTRESPONSE']._serialized_end=111
   _globals['_DIGITALASSISTANTTEXTREQUEST']._serialized_start=113
   _globals['_DIGITALASSISTANTTEXTREQUEST']._serialized_end=197
   _globals['_CHATITEM']._serialized_start=199
   _globals['_CHATITEM']._serialized_end=323
   _globals['_OUTERCONTEXTITEM']._serialized_start=325
-  _globals['_OUTERCONTEXTITEM']._serialized_end=404
-  _globals['_INNERCONTEXTITEM']._serialized_start=406
-  _globals['_INNERCONTEXTITEM']._serialized_end=472
-  _globals['_REPLICAITEM']._serialized_start=474
-  _globals['_REPLICAITEM']._serialized_end=533
-  _globals['_DIGITALASSISTANTTEXT']._serialized_start=536
-  _globals['_DIGITALASSISTANTTEXT']._serialized_end=670
+  _globals['_OUTERCONTEXTITEM']._serialized_end=422
+  _globals['_INNERCONTEXTITEM']._serialized_start=424
+  _globals['_INNERCONTEXTITEM']._serialized_end=490
+  _globals['_REPLICAITEM']._serialized_start=492
+  _globals['_REPLICAITEM']._serialized_end=551
+  _globals['_DIGITALASSISTANTTEXT']._serialized_start=554
+  _globals['_DIGITALASSISTANTTEXT']._serialized_end=688
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dig_ass_text_protos-0.0.6/dig_ass_text_protos/DigitalAssistantText_pb2.pyi` & `dig_ass_text_protos-1.0.0/dig_ass_text_protos/DigitalAssistantText_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -24,24 +24,26 @@
     OUTERCONTEXT_FIELD_NUMBER: _ClassVar[int]
     INNERCONTEXT_FIELD_NUMBER: _ClassVar[int]
     OuterContext: OuterContextItem
     InnerContext: InnerContextItem
     def __init__(self, OuterContext: _Optional[_Union[OuterContextItem, _Mapping]] = ..., InnerContext: _Optional[_Union[InnerContextItem, _Mapping]] = ...) -> None: ...
 
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
 
 class InnerContextItem(_message.Message):
     __slots__ = ("Replicas",)
     REPLICAS_FIELD_NUMBER: _ClassVar[int]
     Replicas: _containers.RepeatedCompositeFieldContainer[ReplicaItem]
     def __init__(self, Replicas: _Optional[_Iterable[_Union[ReplicaItem, _Mapping]]] = ...) -> None: ...
```

### Comparing `dig_ass_text_protos-0.0.6/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py` & `dig_ass_text_protos-1.0.0/dig_ass_text_protos/DigitalAssistantText_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-0.0.6/dig_ass_text_protos.egg-info/SOURCES.txt` & `dig_ass_text_protos-1.0.0/dig_ass_text_protos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dig_ass_text_protos-0.0.6/setup.py` & `dig_ass_text_protos-1.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 import re
 from setuptools import setup, find_packages
 
 from dig_ass_text_protos import __version__
 
 
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
-    name="dig_ass_text_protos",
+    name='dig_ass_text_protos',
     version=__version__,
-    author="AGI-MED-TEAM",
-    description="Proto files for dig_ass_text_protos",
+    author='AGI-MED-TEAM',
+    description='Proto files for dig_ass_text_protos',
     long_description=readme,
     # options
     packages=find_packages(),
-    install_requires="\n".join([requirements]),
+    install_requires='\n'.join([requirements]),
     include_package_data=True,
 )
```

