# Comparing `tmp/classnotation-1.1.tar.gz` & `tmp/classnotation-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classnotation-1.1.tar", last modified: Mon Apr 15 06:02:32 2024, max compression
+gzip compressed data, was "classnotation-1.2.tar", last modified: Thu May  2 19:43:37 2024, max compression
```

## Comparing `classnotation-1.1.tar` & `classnotation-1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:02:32.543303 classnotation-1.1/
--rw-r--r--   0 root         (0) root         (0)      281 2024-04-15 06:02:32.543303 classnotation-1.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:02:32.543303 classnotation-1.1/classnotation/
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-15 05:55:22.000000 classnotation-1.1/classnotation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-04-15 03:58:50.000000 classnotation-1.1/classnotation/classnotation.py
--rw-rw-rw-   0 root         (0) root         (0)     8247 2024-04-15 05:55:22.000000 classnotation-1.1/classnotation/dumper.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2024-04-15 05:55:22.000000 classnotation-1.1/classnotation/json_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:02:32.543303 classnotation-1.1/classnotation.egg-info/
--rw-r--r--   0 root         (0) root         (0)      123 2024-04-15 06:02:32.000000 classnotation-1.1/classnotation.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)      465 2024-04-15 05:55:22.000000 classnotation-1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 06:02:32.543303 classnotation-1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 19:43:37.474299 classnotation-1.2/
+-rw-r--r--   0 root         (0) root         (0)      281 2024-05-02 19:43:37.474299 classnotation-1.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 19:43:37.470299 classnotation-1.2/classnotation/
+-rw-rw-rw-   0 root         (0) root         (0)      148 2024-05-02 14:45:56.000000 classnotation-1.2/classnotation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8517 2024-05-02 14:45:56.000000 classnotation-1.2/classnotation/dumper.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2024-04-15 05:55:22.000000 classnotation-1.2/classnotation/json_types.py
+-rw-rw-rw-   0 root         (0) root         (0)    13140 2024-05-02 19:41:55.000000 classnotation-1.2/classnotation/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 19:43:37.470299 classnotation-1.2/classnotation.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      116 2024-05-02 19:43:37.000000 classnotation-1.2/classnotation.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-05-02 19:43:13.000000 classnotation-1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 19:43:37.474299 classnotation-1.2/setup.cfg
```

### Comparing `classnotation-1.1/classnotation/classnotation.py` & `classnotation-1.2/classnotation/loader.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,66 @@
 from typing import Dict, Any, Type, TypeVar, List, get_origin, get_args, Union, Optional, Literal, Tuple
 from dataclasses import fields, is_dataclass
 import logging
 import enum
 import importlib
 import json
+from .json_types import JSONData, JSONObject
 
 T = TypeVar('T')
 
 
 class DataclassLoader:
     allow_whole_float_as_int: bool
     strict: bool
 
     ############################################################################
     # loads
     #
-    # Load json data from a string into a dataclass
+    # Helper function wrapper to load a JSON string directly into a dataclass.
     ############################################################################
     def loads(
         self,
         data_class: Type[T],
         data: str,
         allow_whole_float_as_int: bool = True,
-        strict: bool = False
+        strict: bool = True,
+    ) -> T:
+        return self.load_data(
+            data_class=data_class,
+            data=json.loads(data),
+            allow_whole_float_as_int=allow_whole_float_as_int,
+            strict=strict,
+        )
+
+    ############################################################################
+    # load
+    #
+    # Load pre-parsed json data into a dataclass
+    ############################################################################
+    def load_data(
+        self,
+        data_class: Type[T],
+        data: JSONObject,
+        allow_whole_float_as_int: bool = True,
+        strict: bool = True
     ) -> T:
         self.allow_whole_float_as_int = allow_whole_float_as_int
         self.strict = strict
-        return self._load_data(data_class, json.loads(data), _stack=())
+        return self._load_data(data_class, data, _stack=())
 
     ############################################################################
     # _load_data
     #
     # An internal function call to load arbitrary data objects
     ############################################################################
     def _load_data(
         self,
         data_class: Type[T],
-        data: Dict[Any, Any],
+        data: JSONObject,
         _stack: Tuple[str, ...],
 
     ) -> T:
         if not is_dataclass(data_class):
             raise TypeError("Expected a dataclass type as `data_class`")
 
         field_type_lookup = {field.name: resolve_field_type(field.type, data_class) for field in fields(data_class)}
@@ -142,24 +162,31 @@
                         self.validate_field(value[i], args[i], _stack=(*_stack, "[{}]".format(i)))
                         for i in range(len(value))
                     )
                     return retval
 
         # Union[] and Optional[]
         elif field_origin == Union:
-            last_error: Optional[TypeError] = None
+            all_errors: List[TypeError] = []
             for arg in get_args(field_type):
-                last_error = None
                 try:
                     return self.validate_field(value, arg, _stack=_stack)
                 except TypeError as e:
-                    last_error = e
+                    all_errors.append(e)
+
+            if len(all_errors) > 0:
+                # Build an error message that contains the errors from parsing each of the possible types in the union
+                combined_message = "Expected one of union type `{}` at `{}`\n".format(field_type, ".".join(_stack))
+                for i, error in enumerate(all_errors):
+                    prefix: str = "  {}: ".format(i)
+                    for line in error.args[0].split("\n"):
+                        combined_message += prefix + line + "\n"
+                        prefix = " " * len(prefix)
 
-            if last_error is not None:
-                raise last_error
+                raise TypeError(combined_message)
 
         # Literal[]
         elif field_origin == Literal:
             arg_value = get_args(field_type)[0]
             if type(value) is str and type(arg_value) is bytes:
                 value = value.encode("utf-8")
 
@@ -273,25 +300,38 @@
     elif get_origin(field_type) is not None:
         return field_type
 
     else:
         raise TypeError("Invalid type found on field {} (of type {})".format(field_type, type(field_type)))
 
 
-def load_data(
+
+################################################################################
+# load_data
+#
+# Top level helper function to load a json string into a dataclass without
+# worrying about creating or managing the DataclassLoader object.
+################################################################################
+def loads(
     data_class: Type[T],
-    data: Any,
+    data: str,
     allow_whole_float_as_int: bool = True,
-    strict: bool = False
+    strict: bool = True
 ) -> T:
     loader = DataclassLoader()
-    return loader.loads(data_class, json.dumps(data), allow_whole_float_as_int=allow_whole_float_as_int, strict=strict)
+    return loader.loads(data_class, data, allow_whole_float_as_int=allow_whole_float_as_int, strict=strict)
 
 
-def loads(
+################################################################################
+# load_data
+#
+# Top level helper function to load data into a dataclass without worrying
+# about creating or managing the DataclassLoader object.
+################################################################################
+def load_data(
     data_class: Type[T],
-    data: str,
+    data: JSONObject,
     allow_whole_float_as_int: bool = True,
-    strict: bool = False
+    strict: bool = True
 ) -> T:
     loader = DataclassLoader()
-    return loader.loads(data_class, data, allow_whole_float_as_int=allow_whole_float_as_int, strict=strict)
+    return loader.load_data(data_class, data, allow_whole_float_as_int=allow_whole_float_as_int, strict=strict)
```

### Comparing `classnotation-1.1/classnotation/dumper.py` & `classnotation-1.2/classnotation/dumper.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,21 @@
 # the classnotation loader and ported whenever a test failed. As a result none
 # of the overarching logic is thought out. While this file does not need to be
 # rebuilt from the ground up, the tests obviously pass, each branch should be
 # revisited with an eye to "what is this actually doing" at some point in
 # the future.
 # TODO: The errors are almost certainly wrong and will confuse regular users
 from types import NoneType
-from typing import Dict, Any, Type, TypeVar, List, get_origin, get_args, Union, Optional, Literal, Tuple
+from typing import Any, TypeVar, get_origin, get_args, Union, Optional, Literal, Tuple
 from .json_types import JSONData, JSONObject
-from dataclasses import Field, fields, is_dataclass
-import logging
+from dataclasses import fields, is_dataclass
 import enum
-import importlib
 import json
 
 
-
-
-
-
 T = TypeVar('T')
 
 
 class DataclassDumper():
 
     def dumps(
         self,
@@ -195,14 +189,21 @@
 
             elif field_type is float and type(value) is float:
                 return value
 
             elif field_type is bool and type(value) is bool:
                 return value
 
+            elif is_dataclass(field_type) and is_dataclass(value):
+                return self._dump_data(value, _stack=_stack) # Stack might be wrong here
+
+            elif issubclass(field_type, enum.Enum) and issubclass(type(value), enum.Enum):
+                # Return the value of the enum
+                return value.value
+
             # If we get here, nothing above parsed properly
             raise TypeError("Unhandled scalar type `{found_type}` at `{stack}`. Expected `{target_type}`.".format(
                 found_type=type(value),
                 stack=".".join(_stack),
                 target_type=field_type)
             )
```

