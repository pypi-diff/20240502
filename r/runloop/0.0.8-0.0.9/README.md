# Comparing `tmp/runloop-0.0.8.tar.gz` & `tmp/runloop-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runloop-0.0.8.tar", last modified: Wed Feb 14 05:35:19 2024, max compression
+gzip compressed data, was "runloop-0.0.9.tar", last modified: Thu Feb 15 00:03:34 2024, max compression
```

## Comparing `runloop-0.0.8.tar` & `runloop-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 05:35:19.461304 runloop-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-14 05:35:09.000000 runloop-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-02-14 05:35:19.461304 runloop-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-14 05:35:09.000000 runloop-0.0.8/PYPI_README.md
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-02-14 05:35:09.000000 runloop-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-02-14 05:35:09.000000 runloop-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 05:35:09.000000 runloop-0.0.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 05:35:19.457303 runloop-0.0.8/runloop/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-14 05:35:09.000000 runloop-0.0.8/runloop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-02-14 05:35:09.000000 runloop-0.0.8/runloop/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 05:35:19.461304 runloop-0.0.8/runloop/manifest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 05:35:09.000000 runloop-0.0.8/runloop/manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-02-14 05:35:09.000000 runloop-0.0.8/runloop/manifest/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-02-14 05:35:09.000000 runloop-0.0.8/runloop/manifest/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 05:35:19.461304 runloop-0.0.8/runloop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-02-14 05:35:19.000000 runloop-0.0.8/runloop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-02-14 05:35:19.000000 runloop-0.0.8/runloop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 05:35:19.000000 runloop-0.0.8/runloop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 05:35:19.000000 runloop-0.0.8/runloop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-14 05:35:19.000000 runloop-0.0.8/runloop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-14 05:35:19.461304 runloop-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-14 05:35:09.000000 runloop-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 05:35:19.461304 runloop-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 05:35:09.000000 runloop-0.0.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9822 2024-02-14 05:35:09.000000 runloop-0.0.8/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-02-14 05:35:09.000000 runloop-0.0.8/tests/test_packaging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:03:34.938289 runloop-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-15 00:03:24.000000 runloop-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-02-15 00:03:34.938289 runloop-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-15 00:03:24.000000 runloop-0.0.9/PYPI_README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-02-15 00:03:24.000000 runloop-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-02-15 00:03:24.000000 runloop-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 00:03:24.000000 runloop-0.0.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:03:34.934290 runloop-0.0.9/runloop/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-15 00:03:24.000000 runloop-0.0.9/runloop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-15 00:03:24.000000 runloop-0.0.9/runloop/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:03:34.934290 runloop-0.0.9/runloop/manifest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 00:03:24.000000 runloop-0.0.9/runloop/manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-02-15 00:03:24.000000 runloop-0.0.9/runloop/manifest/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-02-15 00:03:24.000000 runloop-0.0.9/runloop/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-02-15 00:03:24.000000 runloop-0.0.9/runloop/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:03:34.934290 runloop-0.0.9/runloop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-02-15 00:03:34.000000 runloop-0.0.9/runloop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-15 00:03:34.000000 runloop-0.0.9/runloop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 00:03:34.000000 runloop-0.0.9/runloop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 00:03:34.000000 runloop-0.0.9/runloop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-15 00:03:34.000000 runloop-0.0.9/runloop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-15 00:03:34.938289 runloop-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-15 00:03:24.000000 runloop-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 00:03:34.934290 runloop-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 00:03:24.000000 runloop-0.0.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10805 2024-02-15 00:03:24.000000 runloop-0.0.9/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-02-15 00:03:24.000000 runloop-0.0.9/tests/test_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-02-15 00:03:24.000000 runloop-0.0.9/tests/test_session.py
```

### Comparing `runloop-0.0.8/PKG-INFO` & `runloop-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runloop
-Version: 0.0.8
+Version: 0.0.9
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic_core==2.16.2
 
 # Runloop in Python
 
 # TODO - add nicer / cooler widgets here.
```

### Comparing `runloop-0.0.8/pyproject.toml` & `runloop-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `runloop-0.0.8/runloop/functions.py` & `runloop-0.0.9/runloop/functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import inspect
 from typing import Callable
 
 from runloop.manifest.manifest import FunctionDescriptor, RunloopParameter, runloop_manifest
-
-from .manifest.typing import make_runloop_parameter, make_runloop_return_type
+from runloop.typing import make_runloop_parameter, make_runloop_return_type
 
 
 def _make_function_descriptor(func: Callable, parameters: list[RunloopParameter], return_type) -> FunctionDescriptor:
     module = "" if func.__module__ is None else func.__module__
     return FunctionDescriptor(
         name=func.__name__,
         module=module,
```

### Comparing `runloop-0.0.8/runloop/manifest/manifest.py` & `runloop-0.0.9/runloop/manifest/manifest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from typing import List, TypeVar, Union
+from typing import List, Type, TypeVar, Union
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 # forward declaration
 RunloopParameter = TypeVar("RunloopParameter")
 RunloopType = TypeVar("RunloopType")
 
 
 class DictionaryType(BaseModel):
@@ -16,19 +16,25 @@
     children: List[RunloopParameter]
 
 
 class ArrayType(BaseModel):
     element_type: RunloopType
 
 
+class SessionType(BaseModel):
+    kv_type: RunloopType
+
+
 class RunloopType(BaseModel):
     type_name: str
+    annotation: Type = Field(None, exclude=True)
     dictionary: Union[None | DictionaryType] = None
     array: Union[None | ArrayType] = None
     model: Union[None | ModelChildren] = None
+    session: Union[None | SessionType] = None
 
 
 class RunloopParameter(BaseModel):
     name: str
     type: RunloopType
```

### Comparing `runloop-0.0.8/runloop/manifest/typing.py` & `runloop-0.0.9/runloop/typing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 from inspect import Signature
 from typing import Any, Type, Union, get_args, get_origin
 
 from pydantic import BaseModel
 
-from .manifest import ArrayType, DictionaryType, ModelChildren, RunloopParameter, RunloopType
+from runloop.manifest.manifest import (
+    ArrayType,
+    DictionaryType,
+    ModelChildren,
+    RunloopParameter,
+    RunloopType,
+    SessionType,
+)
+
+from .session import Session
 
 # Representation of types as strings
 _string_type_literal = "string"
 _int_type_literal = "int"
 _bool_type_literal = "boolean"
 _array_type_literal = "array"
 _dict_type_literal = "dictionary"
 _model_type_literal = "model"
 # null type allowed only as return types
 _null_type_literal = "null"
+_session_type_literal = "session"
 
 _scalar_type_map = {
     str: _string_type_literal,
     int: _int_type_literal,
     bool: _bool_type_literal,
 
     # NOTE: not supported: bytes, bytearray, set, tuple, float
@@ -26,55 +36,63 @@
 _supported_scalars = [str, int, bool]
 # Type annotation for supported scalar types
 _supported_scalar_type = Union[Type[str], Type[int], Type[bool]]
 
 
 def _make_dictionary_parameter(name: str, annotation: Type[Any]) -> RunloopParameter:
     key_type, value_type = get_args(annotation)
-    return RunloopParameter(name=name, type=_dict_type_literal,
+    return RunloopParameter(name=name,
+                            annotation=annotation,
+                            type=_dict_type_literal,
                             dictionary=DictionaryType(key_type=_scalar_type_map[key_type],
                                                       value_type=_make_runloop_type(value_type)))
 
 
 def _make_scalar_type(param_type: _supported_scalar_type) -> RunloopType:
     if param_type not in _supported_scalars:
         raise TypeError(f"Unsupported Runloop type={param_type}")
-    return RunloopType(type_name=_scalar_type_map[param_type])
+    return RunloopType(type_name=_scalar_type_map[param_type],
+                       annotation=param_type)
 
 
 def _make_array_type(annotation: type[Any]) -> RunloopType:
     type_args = get_args(annotation)
     if len(type_args) != 1:
         raise TypeError(f"list type must have key and value type annotations={annotation}")
 
     return RunloopType(type_name=_array_type_literal,
+                       annotation=annotation,
                        array=ArrayType(element_type=_make_runloop_type(type_args[0])))
 
 
 def _make_dict_type(annotation: type[Any]) -> RunloopType:
     type_args = get_args(annotation)
     if len(type_args) != 2:
         raise TypeError(f"dict type must have key and value type annotations={annotation}")
 
     if type_args[0] not in _supported_scalars:
         raise TypeError(f"dict key type must be one simple supported type={_supported_scalars}")
 
     return RunloopType(type_name=_dict_type_literal,
+                       annotation=annotation,
                        dictionary=DictionaryType(key_type=_make_runloop_type(type_args[0]),
                                                  value_type=_make_runloop_type(type_args[1])))
 
 
-def _make_model(name: str, children: list[RunloopParameter]) -> RunloopParameter:
-    return RunloopParameter(name=name, type=_model_type_literal, model=ModelChildren(children=children))
-
-
 def _make_model_type(annotation: type[Any]) -> RunloopType:
     children = [make_runloop_parameter(field_name, field_info.annotation)
                 for (field_name, field_info) in annotation.__fields__.items()]
-    return RunloopType(type_name=_model_type_literal, model=ModelChildren(children=children))
+    return RunloopType(type_name=_model_type_literal, annotation=annotation, model=ModelChildren(children=children))
+
+
+def _make_session_type(annotation: type[Any]) -> RunloopType:
+    session_type = get_args(annotation)
+    kv_type = _make_runloop_type(session_type[0])
+    # TODO: Session parsing incomplete
+    return RunloopType(type_name=_session_type_literal, annotation=Session, session=SessionType(kv_type=kv_type))
 
 
 def _make_runloop_type(annotation: Type[Any]) -> RunloopType:
     if annotation is None:
         raise TypeError("type of None not supported, type must be annotated")
 
     origin = get_origin(annotation)
@@ -85,14 +103,16 @@
             return _make_model_type(annotation)
         elif annotation == dict:
             # dict without type hints, ie dict class
             raise TypeError("dict type must explicitly declare key value types")
         elif annotation == list:
             # list without type hints, ie dict class
             raise TypeError("list type must explicitly declare key value types")
+    elif origin == Session:
+        return _make_session_type(annotation)
     elif origin == list:
         return _make_array_type(annotation)
     elif origin == dict:
         return _make_dict_type(annotation)
     else:
         raise TypeError(f"Unsupported Runloop type={annotation}")
```

### Comparing `runloop-0.0.8/runloop.egg-info/PKG-INFO` & `runloop-0.0.9/runloop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runloop
-Version: 0.0.8
+Version: 0.0.9
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic_core==2.16.2
 
 # Runloop in Python
 
 # TODO - add nicer / cooler widgets here.
```

### Comparing `runloop-0.0.8/tests/test_functions.py` & `runloop-0.0.9/tests/test_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -269,7 +269,29 @@
     @function
     def fn_empty_2(arg1: int):
         pass
 
     test_fns = [x for x in runloop_manifest.functions if x.name == "fn_empty_2"][0]
     assert test_fns.name == "fn_empty_2"
     assert test_fns.return_type.type_name == "null"
+
+
+def test_runloop_session_parameter():
+    from runloop import Session, function, runloop_manifest
+
+    class Thread(BaseModel):
+        name: str
+        message_count: int
+
+    @function
+    def fn_return_session_1(session1: Session[Thread]) -> int:
+        pass
+
+    test_fns = [x for x in runloop_manifest.functions if x.name == "fn_return_session_1"][0]
+    assert test_fns.name == "fn_return_session_1"
+    assert test_fns.parameters[0].name == "session1"
+    assert test_fns.parameters[0].type.type_name == "session"
+    assert test_fns.parameters[0].type.session.kv_type.type_name == "model"
+    assert test_fns.parameters[0].type.session.kv_type.model.children[0].name == "name"
+    assert test_fns.parameters[0].type.session.kv_type.model.children[0].type.type_name == "string"
+    assert test_fns.parameters[0].type.session.kv_type.model.children[1].name == "message_count"
+    assert test_fns.parameters[0].type.session.kv_type.model.children[1].type.type_name == "int"
```

### Comparing `runloop-0.0.8/tests/test_packaging.py` & `runloop-0.0.9/tests/test_packaging.py`

 * *Files identical despite different names*

