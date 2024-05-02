# Comparing `tmp/onnx-doctor-0.0.1a1.tar.gz` & `tmp/onnx_doctor-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx-doctor-0.0.1a1.tar", last modified: Sat Mar 30 22:00:27 2024, max compression
+gzip compressed data, was "onnx_doctor-0.0.2.tar", last modified: Thu May  2 18:40:00 2024, max compression
```

## Comparing `onnx-doctor-0.0.1a1.tar` & `onnx_doctor-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 justinc    (501) staff       (20)        0 2024-03-30 22:00:27.141996 onnx-doctor-0.0.1a1/
--rw-r--r--   0 justinc    (501) staff       (20)     1067 2024-03-29 23:44:45.000000 onnx-doctor-0.0.1a1/LICENSE
--rw-r--r--   0 justinc    (501) staff       (20)     2372 2024-03-30 22:00:27.141660 onnx-doctor-0.0.1a1/PKG-INFO
--rw-r--r--   0 justinc    (501) staff       (20)       39 2024-03-29 23:44:45.000000 onnx-doctor-0.0.1a1/README.md
-drwxr-xr-x   0 justinc    (501) staff       (20)        0 2024-03-30 22:00:27.141232 onnx-doctor-0.0.1a1/onnx_doctor.egg-info/
--rw-r--r--   0 justinc    (501) staff       (20)     2372 2024-03-30 22:00:27.000000 onnx-doctor-0.0.1a1/onnx_doctor.egg-info/PKG-INFO
--rw-r--r--   0 justinc    (501) staff       (20)      540 2024-03-30 22:00:27.000000 onnx-doctor-0.0.1a1/onnx_doctor.egg-info/SOURCES.txt
--rw-r--r--   0 justinc    (501) staff       (20)        1 2024-03-30 22:00:27.000000 onnx-doctor-0.0.1a1/onnx_doctor.egg-info/dependency_links.txt
--rw-r--r--   0 justinc    (501) staff       (20)       24 2024-03-30 22:00:27.000000 onnx-doctor-0.0.1a1/onnx_doctor.egg-info/requires.txt
--rw-r--r--   0 justinc    (501) staff       (20)       11 2024-03-30 22:00:27.000000 onnx-doctor-0.0.1a1/onnx_doctor.egg-info/top_level.txt
-drwxr-xr-x   0 justinc    (501) staff       (20)        0 2024-03-30 22:00:27.139314 onnx-doctor-0.0.1a1/onnxdoctor/
--rw-r--r--   0 justinc    (501) staff       (20)      297 2024-03-30 03:23:53.000000 onnx-doctor-0.0.1a1/onnxdoctor/__init__.py
--rw-r--r--   0 justinc    (501) staff       (20)     5701 2024-03-30 20:40:58.000000 onnx-doctor-0.0.1a1/onnxdoctor/_checker.py
--rw-r--r--   0 justinc    (501) staff       (20)     1203 2024-03-30 03:23:46.000000 onnx-doctor-0.0.1a1/onnxdoctor/_diagnostics.py
--rw-r--r--   0 justinc    (501) staff       (20)      883 2024-03-30 21:59:25.000000 onnx-doctor-0.0.1a1/onnxdoctor/_message.py
-drwxr-xr-x   0 justinc    (501) staff       (20)        0 2024-03-30 22:00:27.139997 onnx-doctor-0.0.1a1/onnxdoctor/diagnostics_providers/
--rw-r--r--   0 justinc    (501) staff       (20)      108 2024-03-30 19:48:01.000000 onnx-doctor-0.0.1a1/onnxdoctor/diagnostics_providers/__init__.py
-drwxr-xr-x   0 justinc    (501) staff       (20)        0 2024-03-30 22:00:27.140732 onnx-doctor-0.0.1a1/onnxdoctor/diagnostics_providers/onnxruntime_comparibility/
--rw-r--r--   0 justinc    (501) staff       (20)     6834 2024-03-30 21:58:32.000000 onnx-doctor-0.0.1a1/onnxdoctor/diagnostics_providers/onnxruntime_comparibility/__init__.py
--rw-r--r--   0 justinc    (501) staff       (20)   253912 2024-03-30 19:06:07.000000 onnx-doctor-0.0.1a1/onnxdoctor/diagnostics_providers/onnxruntime_comparibility/_support_table.py
--rw-r--r--   0 justinc    (501) staff       (20)      718 2024-03-30 03:39:06.000000 onnx-doctor-0.0.1a1/onnxdoctor/diagnostics_providers/sparsity.py
--rw-r--r--   0 justinc    (501) staff       (20)     1989 2024-03-30 21:57:14.000000 onnx-doctor-0.0.1a1/pyproject.toml
--rw-r--r--   0 justinc    (501) staff       (20)       38 2024-03-30 22:00:27.142061 onnx-doctor-0.0.1a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:40:00.647755 onnx_doctor-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-02 18:39:53.000000 onnx_doctor-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-02 18:40:00.647755 onnx_doctor-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-02 18:39:53.000000 onnx_doctor-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:40:00.647755 onnx_doctor-0.0.2/onnx_doctor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-02 18:40:00.000000 onnx_doctor-0.0.2/onnx_doctor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-02 18:40:00.000000 onnx_doctor-0.0.2/onnx_doctor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 18:40:00.000000 onnx_doctor-0.0.2/onnx_doctor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 18:40:00.000000 onnx_doctor-0.0.2/onnx_doctor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 18:40:00.000000 onnx_doctor-0.0.2/onnx_doctor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:40:00.647755 onnx_doctor-0.0.2/onnxdoctor/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-02 18:39:53.000000 onnx_doctor-0.0.2/onnxdoctor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-02 18:39:53.000000 onnx_doctor-0.0.2/onnxdoctor/_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-02 18:39:53.000000 onnx_doctor-0.0.2/onnxdoctor/_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-02 18:39:53.000000 onnx_doctor-0.0.2/onnxdoctor/_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:40:00.647755 onnx_doctor-0.0.2/onnxdoctor/chronology/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-02 18:39:53.000000 onnx_doctor-0.0.2/onnxdoctor/chronology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16366 2024-05-02 18:39:53.000000 onnx_doctor-0.0.2/onnxdoctor/chronology/_snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:40:00.647755 onnx_doctor-0.0.2/onnxdoctor/diagnostics_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-02 18:39:53.000000 onnx_doctor-0.0.2/onnxdoctor/diagnostics_providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:40:00.647755 onnx_doctor-0.0.2/onnxdoctor/diagnostics_providers/onnxruntime_compatibility/
+-rw-r--r--   0 runner    (1001) docker     (127)     8585 2024-05-02 18:39:53.000000 onnx_doctor-0.0.2/onnxdoctor/diagnostics_providers/onnxruntime_compatibility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-02 18:39:53.000000 onnx_doctor-0.0.2/onnxdoctor/diagnostics_providers/sparsity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-02 18:39:53.000000 onnx_doctor-0.0.2/onnxdoctor/diagnostics_providers/sparsity_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-02 18:39:53.000000 onnx_doctor-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 18:40:00.647755 onnx_doctor-0.0.2/setup.cfg
```

### Comparing `onnx-doctor-0.0.1a1/LICENSE` & `onnx_doctor-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx-doctor-0.0.1a1/PKG-INFO` & `onnx_doctor-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx-doctor
-Version: 0.0.1a1
+Version: 0.0.2
 Summary: Extensible and beautiful ONNX checker
 Author-email: Justin Chu <justinchuby@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2024 Justin Chu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,11 +40,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: onnx>=1.16
-Requires-Dist: onnxrewriter
+Requires-Dist: onnxscript
+Requires-Dist: rich
+
+# ONNX Doctor
+
+[![PyPI - Version](https://img.shields.io/pypi/v/onnx-doctor.svg)](https://pypi.org/project/onnx-doctor)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/onnx-doctor.svg)](https://pypi.org/project/onnx-doctor)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
-# onnx-doctor
 Diagnose your ONNX model
```

### Comparing `onnx-doctor-0.0.1a1/onnx_doctor.egg-info/PKG-INFO` & `onnx_doctor-0.0.2/onnx_doctor.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx-doctor
-Version: 0.0.1a1
+Version: 0.0.2
 Summary: Extensible and beautiful ONNX checker
 Author-email: Justin Chu <justinchuby@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2024 Justin Chu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,11 +40,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: onnx>=1.16
-Requires-Dist: onnxrewriter
+Requires-Dist: onnxscript
+Requires-Dist: rich
+
+# ONNX Doctor
+
+[![PyPI - Version](https://img.shields.io/pypi/v/onnx-doctor.svg)](https://pypi.org/project/onnx-doctor)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/onnx-doctor.svg)](https://pypi.org/project/onnx-doctor)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
-# onnx-doctor
 Diagnose your ONNX model
```

### Comparing `onnx-doctor-0.0.1a1/onnx_doctor.egg-info/SOURCES.txt` & `onnx_doctor-0.0.2/onnx_doctor.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -6,11 +6,13 @@
 onnx_doctor.egg-info/dependency_links.txt
 onnx_doctor.egg-info/requires.txt
 onnx_doctor.egg-info/top_level.txt
 onnxdoctor/__init__.py
 onnxdoctor/_checker.py
 onnxdoctor/_diagnostics.py
 onnxdoctor/_message.py
+onnxdoctor/chronology/__init__.py
+onnxdoctor/chronology/_snapshot.py
 onnxdoctor/diagnostics_providers/__init__.py
 onnxdoctor/diagnostics_providers/sparsity.py
-onnxdoctor/diagnostics_providers/onnxruntime_comparibility/__init__.py
-onnxdoctor/diagnostics_providers/onnxruntime_comparibility/_support_table.py
+onnxdoctor/diagnostics_providers/sparsity_test.py
+onnxdoctor/diagnostics_providers/onnxruntime_compatibility/__init__.py
```

### Comparing `onnx-doctor-0.0.1a1/onnxdoctor/_checker.py` & `onnx_doctor-0.0.2/onnxdoctor/_checker.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,37 @@
 from __future__ import annotations
 
-from typing import Iterable, Sequence
 import typing
+from typing import Iterable, Sequence
 
-from onnxrewriter.experimental import intermediate_representation as ir
+from onnxscript import ir
 
 from . import _diagnostics, _message
 
 
-def diagnose(
-    ir_object: ir.ModelProtocol
-    | ir.GraphProtocol
-    | ir.FunctionProtocol
-    | ir.NodeProtocol
-    | ir.TensorProtocol
-    | ir.ValueProtocol
-    | ir.AttributeProtocol
-    | ir.ReferenceAttributeProtocol,
+def diagnose(  # noqa: PLR0911
+    ir_object: _message.PossibleTargets,
     diagnostics_providers: Iterable[_diagnostics.DiagnosticsProvider],
 ) -> Sequence[_message.DiagnosticsMessage]:
     if isinstance(ir_object, ir.ModelProtocol):
-        return list(
-            message for message in diagnose_model(ir_object, diagnostics_providers)
-        )
+        return list(diagnose_model(ir_object, diagnostics_providers))
     if isinstance(ir_object, ir.GraphProtocol):
-        return list(
-            message for message in diagnose_graph(ir_object, diagnostics_providers)
-        )
+        return list(diagnose_graph(ir_object, diagnostics_providers))
     if isinstance(ir_object, ir.FunctionProtocol):
-        return list(
-            message for message in diagnose_function(ir_object, diagnostics_providers)
-        )
+        return list(diagnose_function(ir_object, diagnostics_providers))
     if isinstance(ir_object, ir.NodeProtocol):
-        return list(
-            message for message in diagnose_node(ir_object, diagnostics_providers)
-        )
+        return list(diagnose_node(ir_object, diagnostics_providers))
     if isinstance(ir_object, ir.TensorProtocol):
-        return list(
-            message for message in diagnose_tensor(ir_object, diagnostics_providers)
-        )
+        return list(diagnose_tensor(ir_object, diagnostics_providers))
     if isinstance(ir_object, ir.ValueProtocol):
-        return list(
-            message for message in diagnose_value(ir_object, diagnostics_providers)
-        )
+        return list(diagnose_value(ir_object, diagnostics_providers))
     if isinstance(ir_object, ir.AttributeProtocol):
-        return list(
-            message for message in diagnose_attribute(ir_object, diagnostics_providers)
-        )
+        return list(diagnose_attribute(ir_object, diagnostics_providers))
+    if isinstance(ir_object, ir.ReferenceAttributeProtocol):
+        return list(diagnose_attribute(ir_object, diagnostics_providers))
     raise TypeError(f"Unknown IR object: {ir_object}")
 
 
 def diagnose_model(
     model: ir.ModelProtocol,
     diagnostics_providers: Iterable[_diagnostics.DiagnosticsProvider],
 ) -> _diagnostics.DiagnosticsMessageIterator:
@@ -65,29 +46,29 @@
     graph: ir.GraphProtocol,
     diagnostics_providers: Iterable[_diagnostics.DiagnosticsProvider],
 ) -> _diagnostics.DiagnosticsMessageIterator:
     for diagnostics_provider in diagnostics_providers:
         yield from diagnostics_provider.check_graph(graph)
     for value in graph.inputs:
         yield from diagnose_value(value, diagnostics_providers)
-    for node in graph.nodes:
+    for node in graph:
         yield from diagnose_node(node, diagnostics_providers)
     for initializer in graph.initializers.values():
         yield from diagnose_tensor(initializer, diagnostics_providers)
 
 
 def diagnose_function(
     function: ir.FunctionProtocol,
     diagnostics_providers: Iterable[_diagnostics.DiagnosticsProvider],
 ) -> _diagnostics.DiagnosticsMessageIterator:
     for diagnostics_provider in diagnostics_providers:
         yield from diagnostics_provider.check_function(function)
     for value in function.inputs:
         yield from diagnose_value(value, diagnostics_providers)
-    for node in function.nodes:
+    for node in function:
         yield from diagnose_node(node, diagnostics_providers)
     # for value in function.outputs:
     #     yield from diagnose_value(value, diagnostics_providers)
 
 
 def diagnose_node(
     node: ir.NodeProtocol,
```

### Comparing `onnx-doctor-0.0.1a1/onnxdoctor/_diagnostics.py` & `onnx_doctor-0.0.2/onnxdoctor/_diagnostics.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,56 @@
-import abc
-from typing import Iterable, Iterator, TypeAlias
-from onnxrewriter.experimental import intermediate_representation as ir
+from __future__ import annotations
+
+import typing
+from typing import Iterable, Iterator, Union
+
+from onnxscript import ir
+
 from . import _message
 
+if typing.TYPE_CHECKING:
+    from typing_extensions import TypeAlias
 
-DiagnosticsMessageIterator: TypeAlias = (
-    Iterable[_message.DiagnosticsMessage] | Iterator[_message.DiagnosticsMessage]
-)
+DiagnosticsMessageIterator: TypeAlias = Union[
+    Iterable[_message.DiagnosticsMessage], Iterator[_message.DiagnosticsMessage]
+]
 
 
-class DiagnosticsProvider(abc.ABC):
+class DiagnosticsProvider:
     def check_model(self, model: ir.ModelProtocol) -> DiagnosticsMessageIterator:
         del model
-        return []
+        return
+        yield
 
     def check_graph(self, graph: ir.GraphProtocol) -> DiagnosticsMessageIterator:
         del graph
-        return []
+        return
+        yield
 
-    def check_function(self, function: ir.FunctionProtocol) -> DiagnosticsMessageIterator:
+    def check_function(
+        self, function: ir.FunctionProtocol
+    ) -> DiagnosticsMessageIterator:
         del function
-        return []
+        return
+        yield
 
     def check_node(self, node: ir.NodeProtocol) -> DiagnosticsMessageIterator:
         del node
-        return []
+        return
+        yield
 
     def check_value(self, value: ir.ValueProtocol) -> DiagnosticsMessageIterator:
         del value
-        return []
+        return
+        yield
 
-    def check_attribute(self, attr: ir.AttributeProtocol | ir.ReferenceAttributeProtocol) -> DiagnosticsMessageIterator:
+    def check_attribute(
+        self, attr: ir.AttributeProtocol | ir.ReferenceAttributeProtocol
+    ) -> DiagnosticsMessageIterator:
         del attr
-        return []
+        return
+        yield
 
     def check_tensor(self, tensor: ir.TensorProtocol) -> DiagnosticsMessageIterator:
         del tensor
-        return []
+        return
+        yield
```

### Comparing `onnx-doctor-0.0.1a1/onnxdoctor/diagnostics_providers/onnxruntime_comparibility/__init__.py` & `onnx_doctor-0.0.2/onnxdoctor/diagnostics_providers/onnxruntime_compatibility/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,127 @@
 """Analyze model compatibility with ONNX Runtime."""
 
+from __future__ import annotations
+
 import collections
 import dataclasses
+import json
+import pathlib
 
-from onnxrewriter.experimental import intermediate_representation as ir
-from onnxrewriter.experimental.intermediate_representation import _core
+from onnxscript import ir
 
 import onnxdoctor
 
-from . import _support_table
-
-
 _SPECIAL_OPS_TO_SKIP = {
     ("", "Constant"),
+    ("", "CastLike"),
 }
 
 
 @dataclasses.dataclass
 class OnnxRuntimeOpSchema:
     domain: str
     name: str
     input_types: list[str]  # Name -> TypeStr
     outputs_types: list[str]  # Name -> TypeStr
     # TODO: Handle variadic inputs and outputs
+    version_range: tuple[int, int]
     type_constraints: dict[str, list[str]] = dataclasses.field(
         default_factory=dict
     )  # Type -> Constraints
-    version_range: tuple[int, int] | None = None
     execution_provider: str = ""
 
 
 def _get_op_support_table(
-    op_schemas: list[dict]
+    op_schemas: list[dict],
 ) -> dict[tuple[str, str], list[OnnxRuntimeOpSchema]]:
     op_support_table = collections.defaultdict(list)
     for elem in op_schemas:
         schema = OnnxRuntimeOpSchema(**elem)
         op_support_table[(schema.domain, schema.name)].append(schema)
     return op_support_table
 
 
 def _version_in_range(version: int, version_range: tuple[int, int]) -> bool:
     return version_range[0] <= version <= version_range[1]
 
 
-def _to_type_str(type_: ir.TypeProtocol) -> str:
-    if isinstance(type_, _core.TensorType):
+def _to_onnx_string_type_format(type_: ir.TypeProtocol) -> str:
+    if isinstance(type_, ir.TensorType):
         return f"tensor({type_.dtype.name.lower()})"
+    if isinstance(type_, ir.SequenceType):
+        return f"seq({_to_onnx_string_type_format(type_.elem_type)})"
+    if isinstance(type_, ir.OptionalType):
+        return f"optional({_to_onnx_string_type_format(type_.elem_type)})"
     raise NotImplementedError(f"Type {type(type_)} is not supported.")
 
 
 class OnnxRuntimeCompatibilityLinter(onnxdoctor.DiagnosticsProvider):
+    PRODUCER = "OnnxRuntimeCompatibilityLinter"
+
     def __init__(self, execution_provider: str = "CPUExecutionProvider"):
         self.execution_provider = execution_provider
         self.ir_version = None
-        self.support_table = _get_op_support_table(_support_table.TABLE)
+        with open(
+            pathlib.Path(__file__).parent / "ort_supported_schemas.json",
+            encoding="utf-8",
+        ) as f:
+            support_table = json.load(f)
+        self.support_table = _get_op_support_table(support_table)
         self.opset_imports = {}
+        self.imported_functions = set()
 
     def check_model(
         self, model: ir.ModelProtocol
     ) -> onnxdoctor.DiagnosticsMessageIterator:
         self.ir_version = model.ir_version
         self.opset_imports = model.opset_imports
-        return []
+        self.imported_functions = set(model.functions)
+        return
+        yield
 
-    def check_node(
+    def check_node(  # noqa: PLR0912
         self, node: ir.NodeProtocol
     ) -> onnxdoctor.DiagnosticsMessageIterator:
+        function_op_id = (node.domain, node.op_type, node.overload)
+        if function_op_id in self.imported_functions:
+            # The op is a function op and the function is defined
+            # TODO: Handle opset version
+            return
         op_id = (node.domain, node.op_type)
         if op_id in _SPECIAL_OPS_TO_SKIP:
             return
         if (schemas := self.support_table.get(op_id)) is None:
             yield onnxdoctor.DiagnosticsMessage(
                 target_type="node",
                 target=node,
-                message=f"ONNX Runtime does not support operator {node.domain}::{node.op_type} with {self.execution_provider}",
+                message=f"Operator {node.domain}::{node.op_type} not supported by {self.execution_provider} in ONNX Runtime.",
                 # TODO: Allow customizing severity
                 severity="error",
                 error_code="operator-unsupported",
+                producer=self.PRODUCER,
             )
             return
         opset_version = self.opset_imports[node.domain]
         found_schema = None
         for schema in schemas:
-            assert schema.version_range is not None, f"Bug: {schema} does not have version_range."
             if _version_in_range(opset_version, schema.version_range):
                 found_schema = schema
                 break
         if found_schema is None:
             yield onnxdoctor.DiagnosticsMessage(
                 target_type="node",
                 target=node,
                 message=(
-                    f"ONNX Runtime does not support operator {node.domain}::{node.op_type} with {self.execution_provider} in opset {opset_version}. "
+                    f"Operator {node.domain}::{node.op_type} in opset {opset_version} not supported by {self.execution_provider} in ONNX Runtime. "
                     f"All supported versions: {', '.join(f'{schema.version_range[0]}-{schema.version_range[1]}' for schema in schemas)}."
                 ),
                 severity="error",
                 error_code="operator-version-unsupported",
+                producer=self.PRODUCER,
             )
             return
 
         # Check types
         bounded_types: dict[str, ir.TypeProtocol] = {}
         bounded_index = {}
         for i, (input_, type_str) in enumerate(
@@ -118,14 +139,15 @@
                     target_type="node",
                     target=node,
                     message=(
                         f"ONNX Runtime expects input {input_.name} of operator {node.domain}::{node.op_type} to have type {type_str}={bounded_types[type_str]} (bounded by index {bounded_index[type_str]}), but found {input_.type}."
                     ),
                     severity="error",
                     error_code="node-type-inconsistent",
+                    producer=self.PRODUCER,
                 )
         for i, (output, type_str) in enumerate(
             zip(node.outputs, found_schema.outputs_types)
         ):
             if output.type is None:
                 continue
             if type_str not in bounded_types:
@@ -137,28 +159,52 @@
                     target_type="node",
                     target=node,
                     message=(
                         f"ONNX Runtime expects output {output.name} of operator {node.domain}::{node.op_type} to have type {type_str}={bounded_types[type_str]} (bounded by index {bounded_index[type_str]}), but found {output.type}."
                     ),
                     severity="error",
                     error_code="node-type-inconsistent",
+                    producer=self.PRODUCER,
                 )
         for type_str, type_ in bounded_types.items():
             # type_str can be a type constraint name like T, or a type string like tensor(float)
-            # 1/2. Handle the tensor(float) case fist
-            if _to_type_str(type_) == type_str:
+            # 1/3. Handle the tensor(float) case fist
+            onnx_type = _to_onnx_string_type_format(type_)
+            if onnx_type == type_str:
+                continue
+            # 2/3. Handle the B case
+            if type_str == "B" and onnx_type == "tensor(bool)":
+                # Special case: B means boolean and is sometimes not specified
                 continue
-            # 2/2. Handle the T case
+            # 3/3. Handle the <T> case
             supported_types = found_schema.type_constraints.get(type_str)
-            assert (
-                supported_types is not None and type_str not in supported_types
-            ), f"Bug: Type {type_str} is not defined in the schema {found_schema}"
-            if _to_type_str(type_) not in supported_types:
+            if supported_types is None:
+                yield onnxdoctor.DiagnosticsMessage(
+                    target_type="node",
+                    target=node,
+                    message=(
+                        f"Bug: Type {type_str} is not defined in the schema {found_schema}"
+                    ),
+                    severity="failure",
+                    error_code="typestr-not-exist-in-schema",
+                    producer=self.PRODUCER,
+                )
+                continue
+            if (
+                onnx_type == "tensor(float16)"
+                and self.execution_provider == "CPUExecutionProvider"
+            ):
+                # Special case: ONNX Runtime supports float16 on CPU by inserting a Cast node
+                continue
+            if onnx_type not in supported_types:
                 yield onnxdoctor.DiagnosticsMessage(
                     target_type="node",
                     target=node,
                     message=(
-                        f"Operator {node.domain}::{node.op_type}-{opset_version} binds type string {type_str}={type_} which is not supported by ONNX Runtime. Supported types: {', '.join(supported_types)}, with {self.execution_provider}."
+                        f"Operator {node.domain}::{node.op_type}-{opset_version} binds type string "
+                        f"{type_str}={type_} which is not supported by ONNX Runtime's "
+                        f"{self.execution_provider}. Supported types: {', '.join(supported_types)}."
                     ),
                     severity="error",
                     error_code="type-unsupported",
+                    producer=self.PRODUCER,
                 )
```

### Comparing `onnx-doctor-0.0.1a1/onnxdoctor/diagnostics_providers/sparsity.py` & `onnx_doctor-0.0.2/onnxdoctor/diagnostics_providers/sparsity.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,28 @@
-import onnxdoctor
-from onnxrewriter.experimental import intermediate_representation as ir
+from __future__ import annotations
+
 import numpy as np
+from onnxscript import ir
+
+import onnxdoctor
 
 
 class SparsityAnalyzer(onnxdoctor.DiagnosticsProvider):
+    PRODUCER = "SparsityAnalyzer"
+
     def __init__(self, threshold: float = 1e-5):
         self.threshold = threshold
 
-    def check_tensor(self, tensor: ir.TensorProtocol) -> onnxdoctor.DiagnosticsMessageIterator:
+    def check_tensor(
+        self, tensor: ir.TensorProtocol
+    ) -> onnxdoctor.DiagnosticsMessageIterator:
         array = tensor.numpy()
-        sparsity = np.count_nonzero(array < self.threshold) / array.size
+        sparsity = np.count_nonzero(np.abs(array) <= self.threshold) / array.size
         if tensor is not None:
             yield onnxdoctor.DiagnosticsMessage(
                 target_type="tensor",
                 target=tensor,
-                message="Sparsity is {:.2f}%".format(sparsity * 100),
+                message=f"Sparsity is {sparsity * 100:.2f}%",
                 severity="info",
+                producer=self.PRODUCER,
+                error_code="sparsity",
             )
```

### Comparing `onnx-doctor-0.0.1a1/pyproject.toml` & `onnx_doctor-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "onnx-doctor"
-version = "0.0.1a1"
+version = "0.0.2"
 dependencies = [
     "onnx>=1.16",
-    "onnxrewriter",
+    "onnxscript",
+    "rich",
 ]
 description = "Extensible and beautiful ONNX checker"
 keywords = []
 authors = [
   { name = "Justin Chu", email = "justinchuby@users.noreply.github.com" },
 ]
 readme = "README.md"
@@ -36,44 +37,64 @@
 Documentation = "https://github.com/justinchuby/onnx-doctor#readme"
 Issues = "https://github.com/justinchuby/onnx-doctor/issues"
 Source = "https://github.com/justinchuby/onnx-doctor"
 
 [tool.setuptools.packages.find]
 include = ["onnxdoctor*"]
 
+[tool.setuptools.package-data]
+onnxdoctor = ["*.json"]
+
 [tool.pydocstyle]
 convention = "google"
 
 [tool.ruff]
 target-version = "py38"
 lint.select = [
     "A",
     "ARG",
     "B", # flake8-bugbear
     "C4", # flake8-comprehensions
     "D", # pydocstyle
     "E", # pycodestyle
     "F", # Pyflakes
     "G", # flake8-logging-format
+    "I", # isort
     "ICN",
     "ISC", # flake8-implicit-str-concat
+    "LOG", # flake8-logging-format
     "N", # pep8-naming
+    "NPY", # modern numpy
+    "PERF", # Perflint
+    "PIE", # flake8-pie
     "PLC",
     "PLE",
     "PLR",
     "PLW",
-    "NPY", # modern numpy
-    "PERF", # Perflint
     "RUF", # Ruff-specific rules
+    "SIM",
+    "SLOT",
     "T10", # flake8-debugger
     "TID252", # Disallow relative imports
+    "TRY",
     "UP", # pyupgrade
     "W", # pycodestyle
     "YTT", # flake8-2020
 ]
 lint.ignore = [
+    "D1", # D1 is for missing docstrings, which is not yet enforced.
     "E501", # Line length. Not enforced because black will handle formatting
-    "PLR0913", # Too many arguments
+    "PYI041", # int | float is more clear
+    "SIM102", # Collapible if statements are not always more readable
+    "SIM108", # We don't always encourage ternary operators
+    "SIM114", # Don't always combine if branches for debugability
+    "SIM116", # Don't use dict lookup to replace if-else
+    "TRY003", # Messages can be constructed in the exception
+    "UP006", # keep-runtime-typing
+    "UP007", # keep-runtime-typing
 ]
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
+
+[tool.ruff.lint.isort]
+required-imports = ["from __future__ import annotations"]
```

