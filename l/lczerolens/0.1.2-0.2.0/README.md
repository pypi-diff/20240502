# Comparing `tmp/lczerolens-0.1.2.tar.gz` & `tmp/lczerolens-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lczerolens-0.1.2.tar", max compression
+gzip compressed data, was "lczerolens-0.2.0.tar", max compression
```

## Comparing `lczerolens-0.1.2.tar` & `lczerolens-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1070 2024-02-25 14:24:19.749688 lczerolens-0.1.2/LICENSE
--rw-r--r--   0        0        0     2823 2024-02-25 14:24:19.749688 lczerolens-0.1.2/README.md
--rw-r--r--   0        0        0     1717 2024-02-25 14:24:19.753688 lczerolens-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      230 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/__init__.py
--rw-r--r--   0        0        0       78 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/_native_builder/__init__.py
--rw-r--r--   0        0        0     8691 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/_native_builder/builder.py
--rw-r--r--   0        0        0    18178 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/_native_builder/constants.py
--rw-r--r--   0        0        0     6037 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/_native_builder/senet.py
--rw-r--r--   0        0        0      155 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/game/__init__.py
--rw-r--r--   0        0        0     7780 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/game/dataset.py
--rw-r--r--   0        0        0      703 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/game/generate.py
--rw-r--r--   0        0        0      180 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/game/search.py
--rw-r--r--   0        0        0     5989 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/game/wrapper.py
--rw-r--r--   0        0        0        0 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/utils/__init__.py
--rw-r--r--   0        0        0     5039 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/utils/board.py
--rw-r--r--   0        0        0    23504 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/utils/constants.py
--rw-r--r--   0        0        0     4249 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/utils/lczero.py
--rw-r--r--   0        0        0     2095 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/utils/move.py
--rw-r--r--   0        0        0      456 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/xai/__init__.py
--rw-r--r--   0        0        0     9767 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/xai/concept.py
--rw-r--r--   0        0        0      217 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/xai/concepts/__init__.py
--rw-r--r--   0        0        0     2098 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/xai/concepts/material.py
--rw-r--r--   0        0        0     2017 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/xai/concepts/move.py
--rw-r--r--   0        0        0     1413 2024-02-25 14:24:19.753688 lczerolens-0.1.2/src/lczerolens/xai/concepts/threat.py
--rw-r--r--   0        0        0        0 2024-02-25 14:24:19.757688 lczerolens-0.1.2/src/lczerolens/xai/helpers/__init__.py
--rw-r--r--   0        0        0    10033 2024-02-25 14:24:19.757688 lczerolens-0.1.2/src/lczerolens/xai/helpers/crp.py
--rw-r--r--   0        0        0     3867 2024-02-25 14:24:19.757688 lczerolens-0.1.2/src/lczerolens/xai/helpers/lrp.py
--rw-r--r--   0        0        0     1789 2024-02-25 14:24:19.757688 lczerolens-0.1.2/src/lczerolens/xai/helpers/sae.py
--rw-r--r--   0        0        0     5307 2024-02-25 14:24:19.757688 lczerolens-0.1.2/src/lczerolens/xai/hook.py
--rw-r--r--   0        0        0     1636 2024-02-25 14:24:19.757688 lczerolens-0.1.2/src/lczerolens/xai/lens.py
--rw-r--r--   0        0        0      227 2024-02-25 14:24:19.757688 lczerolens-0.1.2/src/lczerolens/xai/lenses/__init__.py
--rw-r--r--   0        0        0     2310 2024-02-25 14:24:19.757688 lczerolens-0.1.2/src/lczerolens/xai/lenses/activation.py
--rw-r--r--   0        0        0     2258 2024-02-25 14:24:19.757688 lczerolens-0.1.2/src/lczerolens/xai/lenses/crp.py
--rw-r--r--   0        0        0     7681 2024-02-25 14:24:19.757688 lczerolens-0.1.2/src/lczerolens/xai/lenses/lrp.py
--rw-r--r--   0        0        0     2530 2024-02-25 14:24:19.757688 lczerolens-0.1.2/src/lczerolens/xai/lenses/patching.py
--rw-r--r--   0        0        0     2615 2024-02-25 14:24:19.757688 lczerolens-0.1.2/src/lczerolens/xai/lenses/policy.py
--rw-r--r--   0        0        0     3077 2024-02-25 14:24:19.757688 lczerolens-0.1.2/src/lczerolens/xai/lenses/probing.py
--rw-r--r--   0        0        0     2634 2024-02-25 14:24:19.757688 lczerolens-0.1.2/src/lczerolens/xai/probe.py
--rw-r--r--   0        0        0     3766 1970-01-01 00:00:00.000000 lczerolens-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-02 15:15:41.278627 lczerolens-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2823 2024-05-02 15:15:41.278627 lczerolens-0.2.0/README.md
+-rw-r--r--   0        0        0     1636 2024-05-02 15:15:41.282628 lczerolens-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      367 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/__init__.py
+-rw-r--r--   0        0        0      106 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/_native_builder/__init__.py
+-rw-r--r--   0        0        0     8138 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/_native_builder/builder.py
+-rw-r--r--   0        0        0    18178 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/_native_builder/constants.py
+-rw-r--r--   0        0        0     5961 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/_native_builder/senet.py
+-rw-r--r--   0        0        0        0 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/encodings/__init__.py
+-rw-r--r--   0        0        0     4930 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/encodings/board.py
+-rw-r--r--   0        0        0    23490 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/encodings/constants.py
+-rw-r--r--   0        0        0     2062 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/encodings/move.py
+-rw-r--r--   0        0        0      274 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/game/__init__.py
+-rw-r--r--   0        0        0     4754 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/game/dataset.py
+-rw-r--r--   0        0        0     7199 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/game/play.py
+-rw-r--r--   0        0        0     2375 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/game/preprocess.py
+-rw-r--r--   0        0        0      186 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/model/__init__.py
+-rw-r--r--   0        0        0     4137 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/model/lczero.py
+-rw-r--r--   0        0        0     5772 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/model/wrapper.py
+-rw-r--r--   0        0        0      852 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/xai/__init__.py
+-rw-r--r--   0        0        0     9659 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/xai/concept.py
+-rw-r--r--   0        0        0      402 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/xai/concepts/__init__.py
+-rw-r--r--   0        0        0     2097 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/xai/concepts/material.py
+-rw-r--r--   0        0        0     1987 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/xai/concepts/move.py
+-rw-r--r--   0        0        0     1412 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/xai/concepts/threat.py
+-rw-r--r--   0        0        0        0 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/xai/helpers/__init__.py
+-rw-r--r--   0        0        0     9852 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/xai/helpers/crp.py
+-rw-r--r--   0        0        0     3773 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/xai/helpers/lrp.py
+-rw-r--r--   0        0        0     2719 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/xai/helpers/sae.py
+-rw-r--r--   0        0        0     5167 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/xai/hook.py
+-rw-r--r--   0        0        0     1636 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/xai/lens.py
+-rw-r--r--   0        0        0      351 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/xai/lenses/__init__.py
+-rw-r--r--   0        0        0     2242 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/xai/lenses/activation.py
+-rw-r--r--   0        0        0     2198 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/xai/lenses/crp.py
+-rw-r--r--   0        0        0     7383 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/xai/lenses/lrp.py
+-rw-r--r--   0        0        0     2478 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/xai/lenses/patching.py
+-rw-r--r--   0        0        0     2572 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/xai/lenses/policy.py
+-rw-r--r--   0        0        0     2979 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/xai/lenses/probing.py
+-rw-r--r--   0        0        0     2611 2024-05-02 15:15:41.286628 lczerolens-0.2.0/src/lczerolens/xai/probe.py
+-rw-r--r--   0        0        0     3766 1970-01-01 00:00:00.000000 lczerolens-0.2.0/PKG-INFO
```

### Comparing `lczerolens-0.1.2/LICENSE` & `lczerolens-0.2.0/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Yoann Poupart
+Copyright (c) 2024 Yoann Poupart
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `lczerolens-0.1.2/README.md` & `lczerolens-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lczerolens-0.1.2/pyproject.toml` & `lczerolens-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-[tool.black]
-line-length = 79
-
-[tool.isort]
-profile = "black"
-line_length = 79
-src_paths = ["src", "tests", "scripts", "docs", "demo"]
+[tool.ruff]
+line-length = 119
+target-version = "py39"
 
 [tool.poetry]
 name = "lczerolens"
-version = "0.1.2"
+version = "0.2.0"
 description = "Interpretability for LeelaChessZero networks."
 readme = "README.md"
 license = "MIT"
 authors = [
     "Yoann Poupart <yoann.poupart@ens-lyon.org>",
 ]
```

### Comparing `lczerolens-0.1.2/src/lczerolens/_native_builder/builder.py` & `lczerolens-0.2.0/src/lczerolens/_native_builder/builder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""LCZero model builder.
-"""
+"""LCZero model builder."""
 
 import os
 import re
 
 import torch
 from onnx2torch.onnx_graph import OnnxGraph
 from onnx2torch.utils.safe_shape_inference import safe_shape_inference
@@ -16,18 +15,15 @@
 class BuilderError(Exception):
     """Error raised when the builder fails."""
 
 
 class NativeBuilder:
     """Class for automatically building a model."""
 
-    _module_exp = re.compile(
-        r"\/?(?P<module_name>[a-z_\-]+)(?P<module_index>[0-9]*)"
-        r"(\/(?P<remaining>.*))?"
-    )
+    _module_exp = re.compile(r"\/?(?P<module_name>[a-z_\-]+)(?P<module_index>[0-9]*)" r"(\/(?P<remaining>.*))?")
 
     @staticmethod
     def _translate(name):
         """
         Translates a name.
         """
         mapping = {
@@ -67,27 +63,23 @@
         Builds a model from a given path.
         """
         if model_path.endswith(".onnx"):
             return cls.build_from_onnx_path(model_path)
         elif model_path.endswith(".pt"):
             return cls.build_from_torch_path(model_path)
         else:
-            raise NotImplementedError(
-                f"Model path {model_path} is not supported."
-            )
+            raise NotImplementedError(f"Model path {model_path} is not supported.")
 
     @classmethod
     def build_from_onnx_path(cls, onnx_model_path: str):
         """
         Builds a model from a given path.
         """
         if not os.path.exists(onnx_model_path):
-            raise FileExistsError(
-                f"Model path {onnx_model_path} does not exist."
-            )
+            raise FileExistsError(f"Model path {onnx_model_path} does not exist.")
         try:
             onnx_model = safe_shape_inference(onnx_model_path)
             onnx_graph = OnnxGraph(onnx_model.graph)
         except Exception:
             raise BuilderError(f"Could not load model at {onnx_model_path}.")
         for name, _ in onnx_graph.initializers.items():
             match = cls._module_exp.match(name)
@@ -97,17 +89,15 @@
                     return cls._build_senet_from_onnx(onnx_graph)
         raise BuilderError(f"Could not load model at {onnx_model_path}.")
 
     @staticmethod
     def make_onnx_td_forward(onnx_model):
         old_forward = onnx_model.forward
         output_node = list(onnx_model.graph.nodes)[-1]
-        output_names = [
-            n.name.replace("output_", "") for n in output_node.all_input_nodes
-        ]
+        output_names = [n.name.replace("output_", "") for n in output_node.all_input_nodes]
 
         def td_forward(x):
             old_out = old_forward(x)
             return TensorDict(
                 {name: old_out[i] for i, name in enumerate(output_names)},
                 batch_size=x.shape[0],
             )
@@ -116,17 +106,15 @@
 
     @classmethod
     def build_from_torch_path(cls, torch_model_path: str):
         """
         Builds a model from a given path.
         """
         if not os.path.exists(torch_model_path):
-            raise FileExistsError(
-                f"Model path {torch_model_path} does not exist."
-            )
+            raise FileExistsError(f"Model path {torch_model_path} does not exist.")
         try:
             torch_model = torch.load(torch_model_path)
         except Exception:
             raise BuilderError(f"Could not load model at {torch_model_path}.")
         if isinstance(torch_model, nn.Module):
             return torch_model
         else:
@@ -142,17 +130,15 @@
         n_hidden = None
         n_hidden_red = None
         heads = None
         convert_value_to_wdl = False
         for name, onnx_tensor in onnx_graph.initializers.items():
             parsed_name = name.replace("/w", "")
             try:
-                module_name, module_index, remaining = cls._parse_remaining(
-                    parsed_name
-                )
+                module_name, module_index, remaining = cls._parse_remaining(parsed_name)
             except BuilderError:
                 continue
 
             if module_name == "ini_conv":
                 state_dict_name = f"ini_conv.{remaining}"
             elif module_name == "block":
                 if "axes" in remaining:
@@ -162,42 +148,33 @@
                 if remaining.startswith("conv2/se"):
                     remaining = remaining.replace("conv2/se", "")
                     (
                         submodule_name,
                         submodule_index,
                         subremaining,
                     ) = cls._parse_remaining(remaining)
-                    state_dict_name = (
-                        f"block{module_index}.se_layer."
-                        f"linear{submodule_index}.{submodule_name}"
-                    )
+                    state_dict_name = f"block{module_index}.se_layer." f"linear{submodule_index}.{submodule_name}"
                 else:
                     (
                         submodule_name,
                         submodule_index,
                         subremaining,
                     ) = cls._parse_remaining(remaining)
-                    state_dict_name = (
-                        f"block{module_index}."
-                        f"{submodule_name}{submodule_index}.{subremaining}"
-                    )
+                    state_dict_name = f"block{module_index}." f"{submodule_name}{submodule_index}.{subremaining}"
             elif module_name in ["mlh", "wdl", "policy", "value"]:
                 if heads is None:
                     heads = [module_name]
                 elif module_name not in heads:
                     heads.append(module_name)
                 (
                     submodule_name,
                     submodule_index,
                     subremaining,
                 ) = cls._parse_remaining(remaining)
-                state_dict_name = (
-                    f"{module_name}."
-                    f"{submodule_name}{submodule_index}.{subremaining}"
-                )
+                state_dict_name = f"{module_name}." f"{submodule_name}{submodule_index}.{subremaining}"
             elif module_name == "const":
                 continue
             else:
                 raise BuilderError(f"Could not match {module_name}")
 
             if "linear" in state_dict_name and "weight" in state_dict_name:
                 torch_tensor = onnx_tensor.to_torch().transpose(1, 0)
@@ -205,35 +182,25 @@
                 torch_tensor = onnx_tensor.to_torch()
 
             if "se_layer.linear1.weight" in state_dict_name:
                 tmp_n_hidden_red, tmp_n_hidden = torch_tensor.shape
                 if n_hidden is None:
                     n_hidden = tmp_n_hidden
                 elif n_hidden != tmp_n_hidden:
-                    raise BuilderError(
-                        "n_hidden mismatch: " f"{n_hidden} != {tmp_n_hidden}"
-                    )
+                    raise BuilderError("n_hidden mismatch: " f"{n_hidden} != {tmp_n_hidden}")
                 if n_hidden_red is None:
                     n_hidden_red = tmp_n_hidden_red
                 elif n_hidden_red != tmp_n_hidden_red:
-                    raise BuilderError(
-                        "n_hidden_red mismatch: "
-                        f"{n_hidden_red} != {tmp_n_hidden_red}"
-                    )
+                    raise BuilderError("n_hidden_red mismatch: " f"{n_hidden_red} != {tmp_n_hidden_red}")
             if state_dict_name == "value.linear2.bias":
                 if torch_tensor.shape[0] != 1:
                     convert_value_to_wdl = True
 
             state_dict[state_dict_name] = torch_tensor
-        if (
-            n_hidden is None
-            or n_hidden_red is None
-            or heads is None
-            or n_blocks == 0
-        ):
+        if n_hidden is None or n_hidden_red is None or heads is None or n_blocks == 0:
             raise BuilderError("Could not build SeNet from onnx graph.")
 
         if convert_value_to_wdl:
             if "wdl" in heads:
                 raise BuilderError("Inconsistent heads.")
             heads.append("wdl")
             heads.remove("value")
```

### Comparing `lczerolens-0.1.2/src/lczerolens/_native_builder/constants.py` & `lczerolens-0.2.0/src/lczerolens/_native_builder/constants.py`

 * *Files identical despite different names*

### Comparing `lczerolens-0.1.2/src/lczerolens/_native_builder/senet.py` & `lczerolens-0.2.0/src/lczerolens/_native_builder/senet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""Custom SE ResNet.
-"""
+"""Custom SE ResNet."""
 
 import torch
 from tensordict import TensorDict
 from torch import nn
 
 from lczerolens.xai.helpers.lrp import MulUniformFunction
 
@@ -48,17 +47,15 @@
         out = self.relu(out)
         out = self.linear2(out)
         out = out.view(-1, self.n_hidden * 2, 1, 1)
 
         out1, out2 = out.split(self.n_hidden, dim=1)
         non_lin = self.sigmoid(out1)
         out1 = MulUniformFunction.apply(x, non_lin)
-        return self.sum_layer(
-            torch.stack([out1, out2.repeat(1, 1, 8, 8)], dim=-1)
-        )
+        return self.sum_layer(torch.stack([out1, out2.repeat(1, 1, 8, 8)], dim=-1))
 
 
 class SeBlock(nn.Module):
     """SE ResNet block."""
 
     def __init__(self, n_hidden, n_hidden_red=32) -> None:
         super().__init__()
@@ -97,18 +94,15 @@
     def forward(self, x):
         out = self.conv1(x)
         out = self.relu(out)
         out = self.conv2(out)
         out = out.view(-1, 80 * 64)
         out = out.gather(
             1,
-            torch.tensor(constants.GATHER_INDICES)
-            .unsqueeze(0)
-            .repeat(out.shape[0], 1)
-            .to(out.device),
+            torch.tensor(constants.GATHER_INDICES).unsqueeze(0).repeat(out.shape[0], 1).to(out.device),
         )
         return out
 
 
 class ValueHead(nn.Module):
     """Value head."""
 
@@ -182,17 +176,15 @@
         out = self.softmax(out)
         return out
 
 
 class SeNet(nn.Module):
     """ResNet model."""
 
-    def __init__(
-        self, n_blocks, n_hidden, n_hidden_red=32, heads=None
-    ) -> None:
+    def __init__(self, n_blocks, n_hidden, n_hidden_red=32, heads=None) -> None:
         super().__init__()
         self.n_blocks = n_blocks
         self.n_hidden = n_hidden
         self.n_hidden_red = n_hidden_red
 
         self.ini_conv = nn.Conv2d(112, n_hidden, 3, padding=1)
         for i in range(n_blocks):
```

### Comparing `lczerolens-0.1.2/src/lczerolens/game/dataset.py` & `lczerolens-0.2.0/src/lczerolens/game/dataset.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,25 +6,25 @@
     A class for representing a dataset of games.
 BoardDataset
     A class for representing a dataset of boards.
 IterableBoardDataset
     A class for representing an iterable dataset of boards.
 """
 
-from typing import Any, Dict, List, Optional, Tuple
+from typing import List, Optional, Tuple
 
 import chess
 import jsonlines
 import torch
 import tqdm
 from torch.utils.data import Dataset
 
-from lczerolens.utils import board as board_utils
+from lczerolens.encodings import board as board_encodings
 
-from .generate import Game
+from .preprocess import Game, dict_to_game, game_to_boards
 
 
 class GameDataset(Dataset):
     """A class for representing a dataset of games.
 
     Attributes
     ----------
@@ -41,37 +41,15 @@
             raise ValueError("Either games or file_name must be provided")
         elif games is not None:
             self.games = games
         else:
             self.games = []
             with jsonlines.open(file_name) as reader:
                 for obj in reader:
-                    *pre, post = obj["moves"].split("{ Book exit }")
-                    if pre:
-                        if len(pre) > 1:
-                            raise ValueError("More than one book exit")
-                        (pre,) = pre
-                        parsed_pre_moves = [
-                            m for m in pre.split() if not m.endswith(".")
-                        ]
-                        book_exit = len(parsed_pre_moves)
-                    else:
-                        parsed_pre_moves = []
-                        book_exit = None
-                    parsed_moves = parsed_pre_moves + [
-                        m for m in post.split() if not m.endswith(".")
-                    ]
-
-                    self.games.append(
-                        Game(
-                            gameid=obj["gameid"],
-                            moves=parsed_moves,
-                            book_exit=book_exit,
-                        )
-                    )
+                    self.games.append(dict_to_game(obj))
 
     def __len__(self):
         return len(self.games)
 
     def __getitem__(self, idx) -> Game:
         return self.games[idx]
 
@@ -137,17 +115,15 @@
                     continue
                 idx += 1
                 working_board = board.copy(stack=n_history)
 
                 writer.write(
                     {
                         "fen": working_board.root().fen(),
-                        "moves": [
-                            move.uci() for move in working_board.move_stack
-                        ],
+                        "moves": [move.uci() for move in working_board.move_stack],
                         "gameid": gameid,
                     }
                 )
 
     @classmethod
     def from_game_dataset(
         cls,
@@ -156,95 +132,30 @@
         skip_book_exit: bool = False,
         skip_first_n: int = 0,
     ):
         boards: List[chess.Board] = []
         game_ids: List[str] = []
         print("[INFO] Converting games to boards")
         for game in tqdm.tqdm(game_dataset.games, bar_format="{l_bar}{bar}"):
-            new_boards, new_ids = cls.game_to_board_list(
-                game, n_history, skip_book_exit, skip_first_n
+            new_boards = game_to_boards(
+                game,
+                n_history,
+                skip_book_exit,
+                skip_first_n,
+                output_dict=False,
             )
+            new_ids = [game.gameid] * len(new_boards)
             boards.extend(new_boards)
             game_ids.extend(new_ids)
 
         return cls(boards=boards, game_ids=game_ids)
 
     @staticmethod
-    def preprocess_game(
-        game: Game,
-        n_history: int = 0,
-        skip_book_exit: bool = False,
-        skip_first_n: int = 0,
-    ) -> List[Dict[str, Any]]:
-        working_board = chess.Board()
-        if skip_first_n > 0 or (
-            skip_book_exit and (game.book_exit is not None)
-        ):
-            boards = []
-        else:
-            boards = [
-                {
-                    "fen": working_board.fen(),
-                    "moves": [],
-                    "gameid": game.gameid,
-                }
-            ]
-        for i, move in enumerate(
-            game.moves[:-1]
-        ):  # skip the last move as it can be over
-            working_board.push_san(move)
-            if (i < skip_first_n) or (
-                skip_book_exit
-                and (game.book_exit is not None)
-                and (i < game.book_exit)
-            ):
-                continue
-            save_board = working_board.copy(stack=n_history)
-            boards.append(
-                {
-                    "fen": save_board.root().fen(),
-                    "moves": [move.uci() for move in save_board.move_stack],
-                    "gameid": game.gameid,
-                }
-            )
-        return boards
-
-    @staticmethod
-    def game_to_board_list(
-        game: Game,
-        n_history: int = 0,
-        skip_book_exit: bool = False,
-        skip_first_n: int = 0,
-    ) -> Tuple[List[chess.Board], List[str]]:
-        working_board = chess.Board()
-        if skip_first_n > 0 or (
-            skip_book_exit and (game.book_exit is not None)
-        ):
-            boards = []
-        else:
-            boards = [working_board.copy(stack=n_history)]
-        for i, move in enumerate(
-            game.moves[:-1]
-        ):  # skip the last move as it can be over
-            working_board.push_san(move)
-            if (i < skip_first_n) or (
-                skip_book_exit
-                and (game.book_exit is not None)
-                and (i < game.book_exit)
-            ):
-                continue
-            boards.append(working_board.copy(stack=n_history))
-        return boards, [game.gameid] * len(boards)
-
-    @staticmethod
     def collate_fn_tuple(batch):
         indices, boards = zip(*batch)
         return indices, boards
 
     @staticmethod
     def collate_fn_tensor(batch):
-        tensor_list = [
-            board_utils.board_to_input_tensor(board).unsqueeze(0)
-            for board in batch
-        ]
+        tensor_list = [board_encodings.board_to_input_tensor(board).unsqueeze(0) for board in batch]
         batched_tensor = torch.cat(tensor_list, dim=0)
         return batched_tensor
```

### Comparing `lczerolens-0.1.2/src/lczerolens/game/wrapper.py` & `lczerolens-0.2.0/src/lczerolens/model/wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-"""Class for wrapping the LCZero models.
-"""
+"""Class for wrapping the LCZero models."""
 
 import os
 from typing import Dict, Iterable, Type, Union
 
 import chess
 import torch
 from onnx2torch import convert
 from onnx2torch.utils.safe_shape_inference import safe_shape_inference
 from tensordict import TensorDict
 from torch import nn
 
-from lczerolens.utils import board as board_utils
+from lczerolens.encodings import board as board_encodings
 
 
 class ModelWrapper(nn.Module):
     """Class for wrapping the LCZero models."""
 
     def __init__(
         self,
@@ -44,45 +43,37 @@
     def from_path(cls, model_path: str):
         """Creates a wrapper from a model path."""
         if model_path.endswith(".onnx"):
             return cls.from_onnx_path(model_path)
         elif model_path.endswith(".pt"):
             return cls.from_torch_path(model_path)
         else:
-            raise NotImplementedError(
-                f"Model path {model_path} is not supported."
-            )
+            raise NotImplementedError(f"Model path {model_path} is not supported.")
 
     @classmethod
     def from_onnx_path(cls, onnx_model_path: str, check: bool = True):
         """
         Builds a model from a given path.
         """
         if not os.path.exists(onnx_model_path):
-            raise FileExistsError(
-                f"Model path {onnx_model_path} does not exist."
-            )
+            raise FileExistsError(f"Model path {onnx_model_path} does not exist.")
         try:
             if check:
                 onnx_model = safe_shape_inference(onnx_model_path)
             onnx_torch_model = convert(onnx_model)
-            onnx_torch_model.forward = cls.make_onnx_td_forward(
-                onnx_torch_model
-            )
+            onnx_torch_model.forward = cls.make_onnx_td_forward(onnx_torch_model)
             return cls(model=onnx_torch_model)
         except Exception:
             raise ValueError(f"Could not load model at {onnx_model_path}.")
 
     @staticmethod
     def make_onnx_td_forward(onnx_model):
         old_forward = onnx_model.forward
         output_node = list(onnx_model.graph.nodes)[-1]
-        output_names = [
-            n.name.replace("output_", "") for n in output_node.all_input_nodes
-        ]
+        output_names = [n.name.replace("output_", "") for n in output_node.all_input_nodes]
 
         def td_forward(x):
             old_out = old_forward(x)
             return TensorDict(
                 {name: old_out[i] for i, name in enumerate(output_names)},
                 batch_size=x.shape[0],
             )
@@ -91,17 +82,15 @@
 
     @classmethod
     def from_torch_path(cls, torch_model_path: str):
         """
         Builds a model from a given path.
         """
         if not os.path.exists(torch_model_path):
-            raise FileExistsError(
-                f"Model path {torch_model_path} does not exist."
-            )
+            raise FileExistsError(f"Model path {torch_model_path} does not exist.")
         try:
             torch_model = torch.load(torch_model_path)
         except Exception:
             raise ValueError(f"Could not load model at {torch_model_path}.")
         if isinstance(torch_model, ModelWrapper):
             return torch_model
         elif isinstance(torch_model, nn.Module):
@@ -120,18 +109,15 @@
         if isinstance(to_pred, chess.Board):
             board_list = [to_pred]
         elif isinstance(to_pred, Iterable):
             board_list = to_pred  # type: ignore
         else:
             raise ValueError("Invalid input type.")
 
-        tensor_list = [
-            board_utils.board_to_input_tensor(board).unsqueeze(0)
-            for board in board_list
-        ]
+        tensor_list = [board_encodings.board_to_input_tensor(board).unsqueeze(0) for board in board_list]
         batched_tensor = torch.cat(tensor_list, dim=0)
         if input_requires_grad:
             batched_tensor.requires_grad = True
         batched_tensor = batched_tensor.to(self.device)
         with torch.set_grad_enabled(with_grad):
             out = self.forward(batched_tensor)
 
@@ -147,17 +133,15 @@
     all_flows: Dict[str, Type["Flow"]] = {}
 
     def __init__(
         self,
         model: nn.Module,
     ):
         if not self.is_compatible(model):
-            raise ValueError(
-                f"The model does not have a {self._flow_type} head."
-            )
+            raise ValueError(f"The model does not have a {self._flow_type} head.")
         super().__init__(model=model)
 
     @classmethod
     def register(cls, name: str):
         """Registers the flow."""
 
         def decorator(subclass):
@@ -174,17 +158,15 @@
     @classmethod
     def get_subclass(cls, name: str) -> Type["Flow"]:
         """Returns the subclass."""
         return cls.all_flows[name]
 
     @classmethod
     def is_compatible(cls, model: nn.Module):
-        return hasattr(model, cls._flow_type) or hasattr(
-            model, f"output/{cls._flow_type}"
-        )
+        return hasattr(model, cls._flow_type) or hasattr(model, f"output/{cls._flow_type}")
 
     def forward(self, x):
         """Forward pass."""
         return self.model(x)[self._flow_type]
 
 
 @Flow.register("policy")
```

### Comparing `lczerolens-0.1.2/src/lczerolens/utils/board.py` & `lczerolens-0.2.0/src/lczerolens/encodings/board.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""Board utilities.
-"""
+"""Board utilities."""
 
 import re
 from copy import deepcopy
 from enum import Enum
 from typing import Optional, Tuple
 
 import chess
@@ -31,17 +30,15 @@
     """
     us, them = us_them
     plane_orders = {chess.WHITE: "PNBRQK", chess.BLACK: "pnbrqk"}
     plane_order = plane_orders[us] + plane_orders[them]
     return plane_order
 
 
-def get_piece_index(
-    piece: str, us_them: Tuple[bool, bool], plane_order: Optional[str] = None
-):
+def get_piece_index(piece: str, us_them: Tuple[bool, bool], plane_order: Optional[str] = None):
     """Converts a piece to its index in the plane order.
 
     Parameters
     ----------
     piece : str
         The piece to convert.
     us_them : Tuple[bool, bool]
@@ -77,17 +74,15 @@
 
     Returns
     -------
     torch.Tensor
         The 13x8x8 tensor.
     """
     if input_encoding != InputEncoding.INPUT_CLASSICAL_112_PLANE:
-        raise NotImplementedError(
-            f"Input encoding {input_encoding} not implemented."
-        )
+        raise NotImplementedError(f"Input encoding {input_encoding} not implemented.")
     if us_them is None:
         us = board.turn
         them = not us
     else:
         us, them = us_them
     plane_order = get_plane_order((us, them))
 
@@ -97,26 +92,20 @@
     fen_board = board.fen().split(" ")[0]
     fen_rep = re.sub(r"(\d)", lambda m: "0" * int(m.group(1)), fen_board)
     rows = fen_rep.split("/")
     rev_rows = rows[::-1]
     ordered_fen = "".join(rev_rows)
 
     config_tensor = torch.zeros((13, 8, 8), dtype=torch.float)
-    ordinal_board = torch.tensor(
-        tuple(map(piece_to_index, ordered_fen)), dtype=torch.float
-    )
+    ordinal_board = torch.tensor(tuple(map(piece_to_index, ordered_fen)), dtype=torch.float)
     ordinal_board = ordinal_board.reshape((8, 8)).unsqueeze(0)
-    piece_tensor = torch.tensor(
-        tuple(map(piece_to_index, plane_order)), dtype=torch.float
-    )
+    piece_tensor = torch.tensor(tuple(map(piece_to_index, plane_order)), dtype=torch.float)
     piece_tensor = piece_tensor.reshape((12, 1, 1))
     config_tensor[:12] = (ordinal_board == piece_tensor).float()
-    if board.is_repetition(
-        2
-    ):  # Might be wrong if the full history is not available
+    if board.is_repetition(2):  # Might be wrong if the full history is not available
         config_tensor[12] = torch.ones((8, 8), dtype=torch.float)
     return config_tensor if us == chess.WHITE else config_tensor.flip(1)
 
 
 def board_to_input_tensor(
     last_board=chess.Board,
     with_history: bool = True,
@@ -135,17 +124,15 @@
 
     Returns
     -------
     torch.Tensor
         The 112x8x8 tensor.
     """
     if input_encoding != InputEncoding.INPUT_CLASSICAL_112_PLANE:
-        raise NotImplementedError(
-            f"Input encoding {input_encoding} not implemented."
-        )
+        raise NotImplementedError(f"Input encoding {input_encoding} not implemented.")
     board = deepcopy(last_board)
     input_tensor = torch.zeros((112, 8, 8), dtype=torch.float)
     us = last_board.turn
     them = not us
     if with_history:
         for i in range(8):
             config_tensor = board_to_config_tensor(board, (us, them))
@@ -160,12 +147,10 @@
         input_tensor[105] = torch.ones((8, 8), dtype=torch.float)
     if last_board.has_queenside_castling_rights(them):
         input_tensor[106] = torch.ones((8, 8), dtype=torch.float)
     if last_board.has_kingside_castling_rights(them):
         input_tensor[107] = torch.ones((8, 8), dtype=torch.float)
     if us == chess.BLACK:
         input_tensor[108] = torch.ones((8, 8), dtype=torch.float)
-    input_tensor[109] = (
-        torch.ones((8, 8), dtype=torch.float) * last_board.halfmove_clock
-    )
+    input_tensor[109] = torch.ones((8, 8), dtype=torch.float) * last_board.halfmove_clock
     input_tensor[111] = torch.ones((8, 8), dtype=torch.float)
     return input_tensor
```

### Comparing `lczerolens-0.1.2/src/lczerolens/utils/constants.py` & `lczerolens-0.2.0/src/lczerolens/encodings/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1885,22 +1885,18 @@
         INVERTED_FROM_INDEX[from_square] = [i]
     try:
         INVERTED_TO_INDEX[to_square].append(i)
     except KeyError:
         INVERTED_TO_INDEX[to_square] = [i]
 
 HISTORY_PLANE_NAMES = (
-    [f"{piece} (us)" for piece in "PNBRQK"]
-    + [f"{piece} (them)" for piece in "pnbrqk"]
-    + ["repetition"]
+    [f"{piece} (us)" for piece in "PNBRQK"] + [f"{piece} (them)" for piece in "pnbrqk"] + ["repetition"]
 )
 
-PLANE_NAMES = [
-    f"H{i}: {h_name}" for i in range(8) for h_name in HISTORY_PLANE_NAMES
-] + [
+PLANE_NAMES = [f"H{i}: {h_name}" for i in range(8) for h_name in HISTORY_PLANE_NAMES] + [
     "QCR (us)",
     "KCR (us)",
     "QCR (them)",
     "KCR (them)",
     "color",
     "halfmove",
     "zeros",
```

### Comparing `lczerolens-0.1.2/src/lczerolens/utils/lczero.py` & `lczerolens-0.2.0/src/lczerolens/model/lczero.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,40 +7,35 @@
 """
 
 import subprocess
 
 import chess
 import torch
 
-from lczerolens import move_utils
+from lczerolens.encodings import move as move_encodings
 
 try:
     from lczero.backends import Backend, GameState
 except ImportError as e:
-    raise ImportError(
-        "LCZero bindings are not installed."
-        "See https://github.com/LeelaChessZero/lc0.git."
-    ) from e
+    raise ImportError("LCZero bindings are not installed." "See https://github.com/LeelaChessZero/lc0.git.") from e
 
 
 def generic_command(args, verbose=False):
     """
     Run a generic command.
     """
     popen = subprocess.Popen(
         ["lc0", *args],
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
     popen.wait()
     if popen.returncode != 0:
         if verbose:
-            stderr = (
-                f'\n[DEBUG] stderr:\n{popen.stderr.read().decode("utf-8")}'
-            )
+            stderr = f'\n[DEBUG] stderr:\n{popen.stderr.read().decode("utf-8")}'
         else:
             stderr = ""
         raise RuntimeError(f"Could not run `lc0 {' '.join(args)}`." + stderr)
     return popen.stdout.read().decode("utf-8")
 
 
 def describenet(path, verbose=False):
@@ -66,17 +61,15 @@
     """
     return generic_command(
         ["onnx2leela", f"--input={in_path}", f"--output={out_path}"],
         verbose=verbose,
     )
 
 
-def board_from_backend(
-    lczero_backend: Backend, lczero_game: GameState, planes: int = 112
-):
+def board_from_backend(lczero_backend: Backend, lczero_game: GameState, planes: int = 112):
     """
     Create a board from the lczero backend.
     """
     lczero_input = lczero_game.as_input(lczero_backend)
     lczero_input_tensor = torch.zeros((112, 64), dtype=torch.float)
     for plane in range(planes):
         mask_str = f"{lczero_input.mask(plane):b}".zfill(64)
@@ -100,21 +93,17 @@
     lczero_input = lczero_game.as_input(lczero_backend)
     (lczero_output,) = lczero_backend.evaluate(lczero_input)
     if only_legal:
         indices = torch.tensor(lczero_game.policy_indices())
     else:
         indices = torch.tensor(range(1858))
     if softmax:
-        policy = torch.tensor(
-            lczero_output.p_softmax(*range(1858)), dtype=torch.float
-        )
+        policy = torch.tensor(lczero_output.p_softmax(*range(1858)), dtype=torch.float)
     else:
-        policy = torch.tensor(
-            lczero_output.p_raw(*range(1858)), dtype=torch.float
-        )
+        policy = torch.tensor(lczero_output.p_raw(*range(1858)), dtype=torch.float)
     value = torch.tensor(lczero_output.q())
     filtered_policy[indices] = policy[indices]
     return filtered_policy, value
 
 
 def moves_with_castling_swap(lczero_game: GameState, board: chess.Board):
     """
@@ -128,16 +117,14 @@
             continue
         if board.is_castling(move):
             leela_uci_move = uci_move.replace("g", "h").replace("c", "a")
             if leela_uci_move in lczero_legal_moves:
                 lczero_legal_moves.remove(leela_uci_move)
                 lczero_legal_moves.append(uci_move)
                 lczero_policy_indices.remove(
-                    move_utils.encode_move(
+                    move_encodings.encode_move(
                         chess.Move.from_uci(leela_uci_move),
                         (board.turn, not board.turn),
                     )
                 )
-                lczero_policy_indices.append(
-                    move_utils.encode_move(move, (board.turn, not board.turn))
-                )
+                lczero_policy_indices.append(move_encodings.encode_move(move, (board.turn, not board.turn)))
     return lczero_legal_moves, lczero_policy_indices
```

### Comparing `lczerolens-0.1.2/src/lczerolens/utils/move.py` & `lczerolens-0.2.0/src/lczerolens/encodings/move.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""Utils for the move module.
-"""
+"""Utils for the move module."""
 
 from typing import Tuple
 
 import chess
 
 from .constants import INVERTED_POLICY_INDEX, POLICY_INDEX
 
@@ -22,17 +21,15 @@
     if us == chess.BLACK:
         from_square_row = from_square // 8
         from_square_col = from_square % 8
         from_square = 8 * (7 - from_square_row) + from_square_col
         to_square_row = to_square // 8
         to_square_col = to_square % 8
         to_square = 8 * (7 - to_square_row) + to_square_col
-    us_uci_move = (
-        chess.SQUARE_NAMES[from_square] + chess.SQUARE_NAMES[to_square]
-    )
+    us_uci_move = chess.SQUARE_NAMES[from_square] + chess.SQUARE_NAMES[to_square]
     if move.promotion is not None:
         if move.promotion == chess.BISHOP:
             us_uci_move += "b"
         elif move.promotion == chess.ROOK:
             us_uci_move += "r"
         elif move.promotion == chess.QUEEN:
             us_uci_move += "q"
@@ -58,12 +55,10 @@
         from_square = 8 * (7 - from_square_row) + from_square_col
         to_square_row = to_square // 8
         to_square_col = to_square % 8
         to_square = 8 * (7 - to_square_row) + to_square_col
 
     uci_move = chess.SQUARE_NAMES[from_square] + chess.SQUARE_NAMES[to_square]
     from_piece = board.piece_at(from_square)
-    if (
-        from_piece == chess.PAWN and to_square >= 56
-    ):  # Knight promotion is the default
+    if from_piece == chess.PAWN and to_square >= 56:  # Knight promotion is the default
         uci_move += "n"
     return chess.Move.from_uci(uci_move)
```

### Comparing `lczerolens-0.1.2/src/lczerolens/xai/concept.py` & `lczerolens-0.2.0/src/lczerolens/xai/concept.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-"""Class for concept-based XAI methods.
-"""
+"""Class for concept-based XAI methods."""
 
 import random
 from abc import ABC, abstractmethod
 from typing import Any, Callable, List, Optional, Tuple
 
 import chess
 import jsonlines
 import torch
 import tqdm
 from sklearn import metrics
 
+from lczerolens.encodings import board as board_encodings
 from lczerolens.game.dataset import BoardDataset
-from lczerolens.utils import board as board_utils
 
 
 class Concept(ABC):
     """
     Class for concept-based XAI methods.
     """
 
@@ -131,20 +130,16 @@
         labels,
     ):
         """
         Compute the metrics for a given model and input.
         """
         return {
             "accuracy": metrics.accuracy_score(labels, predictions),
-            "precision": metrics.precision_score(
-                labels, predictions, average="weighted"
-            ),
-            "recall": metrics.recall_score(
-                labels, predictions, average="weighted"
-            ),
+            "precision": metrics.precision_score(labels, predictions, average="weighted"),
+            "recall": metrics.recall_score(labels, predictions, average="weighted"),
             "f1": metrics.f1_score(labels, predictions, average="weighted"),
         }
 
 
 class ContinuousConcept(Concept):
     """
     Class for continuous concept-based XAI methods.
@@ -173,14 +168,15 @@
     def __init__(
         self,
         file_name: Optional[str] = None,
         boards: Optional[List[chess.Board]] = None,
         game_ids: Optional[List[str]] = None,
         concept: Optional[Concept] = None,
         labels: Optional[List[Any]] = None,
+        first_n: Optional[int] = None,
     ):
         if file_name is None:
             super().__init__(file_name, boards, game_ids)
         else:
             self.boards = []
             self.game_ids = []
             self.labels = []
@@ -189,22 +185,23 @@
                     board = chess.Board(obj["fen"])
                     for move in obj["moves"]:
                         board.push_uci(move)
 
                     self.boards.append(board)
                     self.game_ids.append(obj["gameid"])
                     self.labels.append(obj["label"])
+                    if first_n is not None and len(self.boards) >= first_n:
+                        break
         self._concept = concept if concept is not None else NullConcept()
         if labels is not None:
             self.labels = labels
         elif not hasattr(self, "labels"):
             print("[INFO] Computing labels")
             self.labels = [
-                self._concept.compute_label(board)
-                for board in tqdm.tqdm(self.boards, bar_format="{l_bar}{bar}")
+                self._concept.compute_label(board) for board in tqdm.tqdm(self.boards, bar_format="{l_bar}{bar}")
             ]
 
     def __getitem__(self, idx) -> Tuple[int, chess.Board, Any]:  # type: ignore
         board = self.boards[idx]
         label = self.labels[idx]
         return idx, board, label
 
@@ -222,46 +219,38 @@
                     continue
                 idx += 1
                 working_board = board.copy(stack=n_history)
 
                 writer.write(
                     {
                         "fen": working_board.root().fen(),
-                        "moves": [
-                            move.uci() for move in working_board.move_stack
-                        ],
+                        "moves": [move.uci() for move in working_board.move_stack],
                         "gameid": gameid,
                         "label": label,
                     }
                 )
 
     @property
     def concept(self):
         return self._concept
 
     def set_concept(self, concept: Concept, **pbar_kwargs):
         self._concept = concept
         print("[INFO] Computing labels")
         self.labels = [
             self._concept.compute_label(board)
-            for board in tqdm.tqdm(
-                self.boards, bar_format="{l_bar}{bar}", **pbar_kwargs
-            )
+            for board in tqdm.tqdm(self.boards, bar_format="{l_bar}{bar}", **pbar_kwargs)
         ]
 
     @classmethod
-    def from_board_dataset(
-        cls, board_dataset: BoardDataset, concept: Concept, **pbar_kwargs
-    ):
+    def from_board_dataset(cls, board_dataset: BoardDataset, concept: Concept, **pbar_kwargs):
         print("[INFO] Computing labels")
         labels = [
             concept.compute_label(board)
-            for board in tqdm.tqdm(
-                board_dataset.boards, bar_format="{l_bar}{bar}", **pbar_kwargs
-            )
+            for board in tqdm.tqdm(board_dataset.boards, bar_format="{l_bar}{bar}", **pbar_kwargs)
         ]
         return cls(
             boards=board_dataset.boards,
             game_ids=board_dataset.game_ids,
             concept=concept,
             labels=labels,
         )
@@ -270,27 +259,23 @@
     def collate_fn_tuple(batch):
         indices, boards, labels = zip(*batch)
         return tuple(indices), tuple(boards), tuple(labels)
 
     @staticmethod
     def collate_fn_tensor(batch):
         indices, boards, labels = zip(*batch)
-        tensor_list = [
-            board_utils.board_to_input_tensor(board) for board in boards
-        ]
+        tensor_list = [board_encodings.board_to_input_tensor(board) for board in boards]
         batched_tensor = torch.stack(tensor_list, dim=0)
         return tuple(indices), batched_tensor, tuple(labels)
 
     def filter_(self, filter_fn: Callable):
         tuple_boards, tuple_labels, tuple_game_ids = zip(
             *[
                 (board, label, game_id)
-                for board, label, game_id in zip(
-                    self.boards, self.labels, self.game_ids
-                )
+                for board, label, game_id in zip(self.boards, self.labels, self.game_ids)
                 if filter_fn(board, label, game_id)
             ]
         )
         self.boards, self.labels, self.game_ids = (
             list(tuple_boards),
             list(tuple_labels),
             list(tuple_game_ids),
```

### Comparing `lczerolens-0.1.2/src/lczerolens/xai/concepts/material.py` & `lczerolens-0.2.0/src/lczerolens/xai/concepts/material.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""All concepts related to material.
-"""
+"""All concepts related to material."""
 
 from typing import Dict, Optional
 
 import chess
 
 from lczerolens.xai.concept import BinaryConcept
```

### Comparing `lczerolens-0.1.2/src/lczerolens/xai/concepts/move.py` & `lczerolens-0.2.0/src/lczerolens/xai/concepts/move.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-"""All concepts related to move.
-"""
+"""All concepts related to move."""
 
 import chess
 import torch
 
-from lczerolens.game.wrapper import ModelWrapper, PolicyFlow
-from lczerolens.utils import move as move_utils
+from lczerolens.encodings import move as move_encodings
+from lczerolens.model.wrapper import ModelWrapper, PolicyFlow
 from lczerolens.xai.concept import BinaryConcept, MulticlassConcept
 
 
 class BestLegalMoveConcept(MulticlassConcept):
     """Class for move concept-based XAI methods."""
 
     def __init__(
@@ -24,16 +23,15 @@
         board: chess.Board,
     ) -> int:
         """Compute the label for a given model and input."""
         (policy,) = self.policy_flow.predict(board)
         policy = torch.softmax(policy.squeeze(0), dim=-1)
 
         legal_move_indices = [
-            move_utils.encode_move(move, (board.turn, not board.turn))
-            for move in board.legal_moves
+            move_encodings.encode_move(move, (board.turn, not board.turn)) for move in board.legal_moves
         ]
         sub_index = policy[legal_move_indices].argmax().item()
         return legal_move_indices[sub_index]
 
 
 class PieceBestLegalMoveConcept(BinaryConcept):
     """Class for move concept-based XAI methods."""
@@ -52,16 +50,13 @@
         board: chess.Board,
     ) -> int:
         """Compute the label for a given model and input."""
         (policy,) = self.policy_flow.predict(board)
         policy = torch.softmax(policy.squeeze(0), dim=-1)
 
         legal_moves = list(board.legal_moves)
-        legal_move_indices = [
-            move_utils.encode_move(move, (board.turn, not board.turn))
-            for move in legal_moves
-        ]
+        legal_move_indices = [move_encodings.encode_move(move, (board.turn, not board.turn)) for move in legal_moves]
         sub_index = policy[legal_move_indices].argmax().item()
         best_legal_move = legal_moves[sub_index]
         if board.piece_at(best_legal_move.from_square) == self.piece:
             return 1
         return 0
```

### Comparing `lczerolens-0.1.2/src/lczerolens/xai/concepts/threat.py` & `lczerolens-0.2.0/src/lczerolens/xai/concepts/threat.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""All concepts related to threats.
-"""
+"""All concepts related to threats."""
 
 import chess
 
 from lczerolens.xai.concept import BinaryConcept
 
 
 class HasThreatConcept(BinaryConcept):
```

### Comparing `lczerolens-0.1.2/src/lczerolens/xai/helpers/crp.py` & `lczerolens-0.2.0/src/lczerolens/xai/helpers/crp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""Helpers to modify the default classes.
-"""
+"""Helpers to modify the default classes."""
 
 import warnings
 from collections.abc import Iterable
 from typing import Dict, Iterator, List, Optional, Tuple, Union
 
 import numpy as np
 import torch
@@ -121,17 +120,15 @@
             enumerate(loader),
             total=len(self.dataset) // batch_size,
             dynamic_ncols=True,
         ):
             samples_batch = samples[b * batch_size : (b + 1) * batch_size]
             data_batch, targets_samples = batch
 
-            targets_samples = np.array(
-                targets_samples
-            )  # numpy operation needed
+            targets_samples = np.array(targets_samples)  # numpy operation needed
 
             # convert multi target to single target if user defined the method
             data_broadcast, targets, sample_indices = [], [], []
             try:
                 for i_t, target in enumerate(targets_samples):
                     single_targets = self.multitarget_to_single(target)
                     for st in single_targets:
@@ -148,27 +145,23 @@
             except NotImplementedError:
                 data_broadcast, targets, sample_indices = (
                     data_batch,
                     targets_samples,
                     samples_batch,
                 )
 
-            conditions = [
-                {self.attribution.MODEL_OUTPUT_NAME: [t]} for t in targets
-            ]
+            conditions = [{self.attribution.MODEL_OUTPUT_NAME: [t]} for t in targets]
             # dict_inputs is linked to FeatHooks
             dict_inputs["sample_indices"] = sample_indices
             dict_inputs["targets"] = targets
 
             # composites are already registered before
             if on_device:
                 data_broadcast = data_broadcast.to(on_device)  # type: ignore
-            self.attribution(
-                data_broadcast, conditions, None, exclude_parallel=False
-            )
+            self.attribution(data_broadcast, conditions, None, exclude_parallel=False)
 
             if b % checkpoint == checkpoint - 1:
                 self._save_results((last_checkpoint, sample_indices[-1] + 1))
                 last_checkpoint = sample_indices[-1] + 1
 
         # TODO: what happens if result arrays are empty?
         self._save_results((last_checkpoint, sample_indices[-1] + 1))
@@ -192,21 +185,17 @@
         batch_size=32,
         custom_collate_fn=None,
     ) -> Dict:
         ref_c = {}
         if not isinstance(concept_ids, Iterable):
             concept_ids = [concept_ids]
         if mode == "relevance":
-            d_c_sorted, _, rf_c_sorted = load_maximization(
-                self.RelMax.PATH, layer_name
-            )
+            d_c_sorted, _, rf_c_sorted = load_maximization(self.RelMax.PATH, layer_name)
         elif mode == "activation":
-            d_c_sorted, _, rf_c_sorted = load_maximization(
-                self.ActMax.PATH, layer_name
-            )
+            d_c_sorted, _, rf_c_sorted = load_maximization(self.ActMax.PATH, layer_name)
         else:
             raise ValueError("`mode` must be `relevance` or `activation`")
 
         if rf and not composite:
             warnings.warn(
                 "The receptive field is only computed, if you fill the "
                 "'composite' argument with a zennit Composite."
@@ -304,17 +293,15 @@
             num_workers=1,
         )
         data_batch_list, _ = zip(*loader)
 
         if composite:
             data_batch = torch.cat(data_batch_list, dim=0)
             data_p = self.preprocess_data(data_batch)
-            heatmaps = self._attribution_on_reference(
-                data_p, c_id, layer_name, composite, rf, n_indices, batch_size
-            )
+            heatmaps = self._attribution_on_reference(data_p, c_id, layer_name, composite, rf, n_indices, batch_size)
 
             if callable(plot_fn):
                 return plot_fn(data_batch.detach(), heatmaps.detach(), rf)
             else:
                 return data_batch.detach().cpu(), heatmaps.detach().cpu()
 
         else:
```

### Comparing `lczerolens-0.1.2/src/lczerolens/xai/helpers/lrp.py` & `lczerolens-0.2.0/src/lczerolens/xai/helpers/lrp.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,22 +80,16 @@
     @staticmethod
     def backward(ctx, *grad_outputs):
         input_a, input_b, outputs, epsilon = ctx.saved_tensors
         out_relevance = grad_outputs[0]
 
         out_relevance = out_relevance / stabilize(2 * outputs, epsilon)
 
-        relevance_a = (
-            torch.matmul(out_relevance, input_b.permute(0, 1, -1, -2))
-            * input_a
-        )
-        relevance_b = (
-            torch.matmul(input_a.permute(0, 1, -1, -2), out_relevance)
-            * input_b
-        )
+        relevance_a = torch.matmul(out_relevance, input_b.permute(0, 1, -1, -2)) * input_a
+        relevance_b = torch.matmul(input_a.permute(0, 1, -1, -2), out_relevance) * input_b
 
         return relevance_a, relevance_b, None
 
 
 class BilinearMatMulEpsilon(torch.nn.Module):
     def __init__(self, epsilon=1e-6):
         super().__init__()
@@ -130,12 +124,10 @@
 
         return outputs
 
     @staticmethod
     def backward(ctx, *grad_outputs):
         inputs, output = ctx.saved_tensors
 
-        relevance = (
-            grad_outputs[0] - (output * grad_outputs[0].sum(-1, keepdim=True))
-        ) * inputs
+        relevance = (grad_outputs[0] - (output * grad_outputs[0].sum(-1, keepdim=True))) * inputs
 
         return (relevance, None)
```

### Comparing `lczerolens-0.1.2/src/lczerolens/xai/hook.py` & `lczerolens-0.2.0/src/lczerolens/xai/hook.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""Generic hook classes.
-"""
+"""Generic hook classes."""
 
 import re
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Callable, Dict, Optional
 
@@ -30,24 +29,24 @@
     """Enum for cache mode."""
 
     INPUT = "input"
     OUTPUT = "output"
 
 
 @dataclass
-class HookConfig(ABC):
+class HookConfig:
     """
     Configuration for hooks.
     """
 
     hook_type: HookType = HookType.FORWARD
     hook_mode: HookMode = HookMode.OUTPUT
     module_exp: Optional[str] = None
     data: Optional[Dict[str, Any]] = None
-    data_fn: Optional[Callable] = None
+    data_fn: Optional[Callable[[torch.Tensor, Any], torch.Tensor]] = None
 
 
 class Hook(ABC):
     """
     Abstract class for hooks.
     """
 
@@ -68,33 +67,28 @@
             compiled_exp = re.compile(self.config.module_exp)
         for name, module in module.named_modules():
             if name == "":
                 continue
             if not compiled_exp.match(name):
                 continue
             if self.config.hook_type is HookType.FORWARD:
-                self.removable_handles.append(
-                    module.register_forward_hook(self.forward_factory(name))
-                )
+                self.removable_handles.append(module.register_forward_hook(self.forward_factory(name)))
             elif self.config.hook_type is HookType.BACKWARD:
-                self.removable_handles.append(
-                    module.register_backward_hook(self.backward_factory(name))
-                )
+                self.removable_handles.append(module.register_backward_hook(self.backward_factory(name)))
             else:
                 raise ValueError(f"Unknown hook type: {self.config.hook_type}")
         return self.removable_handles
 
     def remove(self):
         """Removes the hook."""
         self.removable_handles.clear()
 
     def clear(self):
         """Clears the storage and removes the hook."""
         self.storage.clear()
-        self.removable_handles.clear()
 
     @abstractmethod
     def forward_factory(self, name: str):
         """
         Creates a hook factory.
         """
         pass
@@ -102,100 +96,88 @@
     @abstractmethod
     def backward_factory(self, name: str):
         """
         Creates a hook factory.
         """
         pass
 
+    def _get_data(self, name):
+        return self.config.data.get(name) if self.config.data is not None else None
+
 
 class CacheHook(Hook):
     """
     Hook for caching.
     """
 
     def forward_factory(self, name: str):
         if self.config.hook_mode is HookMode.INPUT:
 
             def hook(module, input, output):
-                self.storage[name] = input.detach()
+                self.storage[name] = input
 
         elif self.config.hook_mode is HookMode.OUTPUT:
 
             def hook(module, input, output):
-                self.storage[name] = output.detach()
+                self.storage[name] = output
 
         else:
-            raise ValueError(f"Unknown hook mode: {self.config.hook_mode}")
+            raise ValueError(f"Unknown cache mode: {self.config.hook_mode}")
         return hook
 
     def backward_factory(self, name: str):
-        raise NotImplementedError(
-            "Backward hook not implemented for CacheHook"
-        )
+        raise NotImplementedError("Backward hook not implemented for CacheHook")
 
 
 class MeasureHook(Hook):
     """
     Hook for measuring vectors.
     """
 
     def forward_factory(self, name: str):
-        if self.config.data is not None:
-            measure_data = self.config.data[name]
-        else:
-            measure_data = None
         if self.config.hook_mode is HookMode.INPUT:
 
             def hook(module, input, output):
-                self.storage[name] = self.config.data_fn(
-                    input.detach(), measure_data=measure_data
-                )
+                measure_data = self._get_data(name)
+                self.storage[name] = self.config.data_fn(input, measure_data=measure_data, name=name)
 
         elif self.config.hook_mode is HookMode.OUTPUT:
 
             def hook(module, input, output):
-                self.storage[name] = self.config.data_fn(
-                    output.detach(), measure_data=measure_data
-                )
+                measure_data = self._get_data(name)
+                self.storage[name] = self.config.data_fn(output, measure_data=measure_data, name=name)
 
         else:
-            raise ValueError(f"Unknown hook mode: {self.config.hook_mode}")
-
+            raise ValueError(f"Unknown measure mode: {self.config.hook_mode}")
         return hook
 
     def backward_factory(self, name: str):
-        raise NotImplementedError(
-            "Backward hook not implemented for MeasureHook"
-        )
+        raise NotImplementedError("Backward hook not implemented for MeasureHook")
 
 
 class ModifyHook(Hook):
     """
     Hook for modifying vectors.
     """
 
     def forward_factory(self, name: str):
-        if self.config.data is not None:
-            modify_data = self.config.data[name]
-        else:
-            modify_data = None
         if self.config.hook_mode is HookMode.INPUT:
 
             def hook(module, input, output):
-                input = self.config.data_fn(input, modify_data=modify_data)
+                modify_data = self._get_data(name)
+                self.storage[name] = self.config.data_fn(input, modify_data=modify_data, name=name)
                 return input
 
         elif self.config.hook_mode is HookMode.OUTPUT:
 
             def hook(module, input, output):
-                output = self.config.data_fn(output, modify_data=modify_data)
+                modify_data = self._get_data(name)
+                self.storage[name] = self.config.data_fn(output, modify_data=modify_data, name=name)
                 return output
 
         else:
-            raise ValueError(f"Unknown hook mode: {self.config.hook_mode}")
+            raise ValueError(f"Unknown modify mode: {self.config.hook_mode}")
 
         return hook
 
     def backward_factory(self, name: str):
-        raise NotImplementedError(
-            "Backward hook not implemented for ModifyHook"
-        )
+        raise NotImplementedError("Backward hook not implemented for ModifyHook")
```

### Comparing `lczerolens-0.1.2/src/lczerolens/xai/lens.py` & `lczerolens-0.2.0/src/lczerolens/xai/lens.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Generic lens class.
-"""
+"""Generic lens class."""
 
 from abc import ABC, abstractmethod
 from typing import Any, Callable, Dict, Optional, Type
 
 import chess
 from torch.utils.data import Dataset
 
-from lczerolens.game.wrapper import ModelWrapper
+from lczerolens.model.wrapper import ModelWrapper
 
 
 class Lens(ABC):
     """
     Generic lens class.
     """
```

### Comparing `lczerolens-0.1.2/src/lczerolens/xai/lenses/activation.py` & `lczerolens-0.2.0/src/lczerolens/xai/lenses/activation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Activation lens for XAI.
-"""
+"""Activation lens for XAI."""
 
 from typing import Any, Callable, Dict, Optional
 
 import chess
 import torch
 from torch.utils.data import DataLoader, Dataset
 
-from lczerolens.game.wrapper import ModelWrapper
+from lczerolens.model.wrapper import ModelWrapper
 from lczerolens.xai.hook import CacheHook, HookConfig
 from lczerolens.xai.lens import Lens
 
 
 @Lens.register("activation")
 class ActivationLens(Lens):
     """Class for activation-based XAI methods."""
@@ -45,25 +44,21 @@
         collate_fn: Optional[Callable] = None,
         save_to: Optional[str] = None,
         **kwargs,
     ) -> Optional[Dict[str, Any]]:
         """Cache the activations for a given model and dataset."""
         if save_to is not None:
             raise NotImplementedError("Saving to file is not implemented.")
-        dataloader = DataLoader(
-            dataset, batch_size=batch_size, collate_fn=collate_fn
-        )
+        dataloader = DataLoader(dataset, batch_size=batch_size, collate_fn=collate_fn)
         self.cache_hook.clear()
         self.cache_hook.register(wrapper.model)
         batched_activations: Dict[str, Any] = {}
         for batch in dataloader:
             _, boards = batch
             wrapper.predict(boards)
             for key, value in self.cache_hook.storage.items():
                 if key not in batched_activations:
                     batched_activations[key] = value
                 else:
-                    batched_activations[key] = torch.cat(
-                        (batched_activations[key], value), dim=0
-                    )
+                    batched_activations[key] = torch.cat((batched_activations[key], value), dim=0)
         self.cache_hook.clear()
         return batched_activations
```

### Comparing `lczerolens-0.1.2/src/lczerolens/xai/lenses/crp.py` & `lczerolens-0.2.0/src/lczerolens/xai/lenses/crp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-"""Compute CRP heatmap for a given model and input.
-"""
+"""Compute CRP heatmap for a given model and input."""
 
 from typing import Any, Callable, List, Optional
 
 import chess
 import torch
 from crp.attribution import CondAttribution
 from crp.helper import get_layer_names
 from torch.utils.data import Dataset
 
-from lczerolens.game.wrapper import ModelWrapper
+from lczerolens.model.wrapper import ModelWrapper
 from lczerolens.xai.lens import Lens
 
 from .lrp import LrpLens
 
 DEVICE = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 
@@ -36,17 +35,15 @@
         **kwargs,
     ) -> torch.Tensor:
         mode = kwargs.get("mode", "latent_relevances")
         layer_names = kwargs.get("layer_names", None)
         composite = kwargs.get("composite", None)
 
         if mode == "latent_relevances":
-            return self._compute_latent_relevances(
-                [board], wrapper, layer_names=layer_names, composite=composite
-            )
+            return self._compute_latent_relevances([board], wrapper, layer_names=layer_names, composite=composite)
         elif mode == "max_ref":
             raise NotImplementedError
         else:
             raise ValueError(f"Invalid mode {mode}")
 
     def analyse_dataset(
         self,
@@ -63,17 +60,15 @@
         self,
         boards: List[chess.Board],
         wrapper: ModelWrapper,
         layer_names: Optional[List[str]] = None,
         composite: Optional[Any] = None,
     ) -> torch.Tensor:
         if layer_names is None:
-            layer_names = layer_names = get_layer_names(
-                wrapper, [torch.nn.Identity]
-            )
+            layer_names = layer_names = get_layer_names(wrapper, [torch.nn.Identity])
         if composite is None:
             composite = LrpLens.make_default_composite()
 
         attribution = CondAttribution(wrapper)
 
         attr = attribution(boards, composite, record_layer=layer_names)
         return attr.relevances
```

### Comparing `lczerolens-0.1.2/src/lczerolens/xai/lenses/lrp.py` & `lczerolens-0.2.0/src/lczerolens/xai/lenses/lrp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-"""Compute LRP heatmap for a given model and input.
-"""
+"""Compute LRP heatmap for a given model and input."""
 
 from contextlib import contextmanager
 from typing import Any, Callable, Dict, List, Optional
 
 import chess
 import onnx2torch
 import torch
 from torch.utils.data import DataLoader, Dataset
 from zennit.canonizers import SequentialMergeBatchNorm
 from zennit.composites import Composite, LayerMapComposite
 from zennit.rules import Epsilon, Pass, ZPlus
 from zennit.types import Activation
 
-from lczerolens.game.wrapper import ModelWrapper
+from lczerolens.model.wrapper import ModelWrapper
 from lczerolens.xai.helpers import lrp as lrp_helpers
 from lczerolens.xai.lens import Lens
 
 DEVICE = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 
 @Lens.register("lrp")
@@ -88,17 +87,15 @@
         if save_to is not None:
             raise NotImplementedError("Saving to file is not implemented.")
         composite = kwargs.get("composite", None)
         target = kwargs.get("target", "policy")
         replace_onnx2torch = kwargs.get("replace_onnx2torch", True)
         linearise_softmax = kwargs.get("linearise_softmax", False)
         init_rel_fn = kwargs.get("init_rel_fn", None)
-        dataloader = DataLoader(
-            dataset, batch_size=batch_size, collate_fn=collate_fn
-        )
+        dataloader = DataLoader(dataset, batch_size=batch_size, collate_fn=collate_fn)
         relevances = {}
         for batch in dataloader:
             inidices, boards = batch
             batched_relevances = self._compute_lrp_relevance(
                 boards,
                 wrapper,
                 composite=composite,
@@ -121,36 +118,26 @@
         linearise_softmax: bool = False,
         init_rel_fn: Optional[Callable] = None,
     ):
         """
         Compute LRP heatmap for a given model and input.
         """
 
-        with self.context(
-            wrapper, composite, replace_onnx2torch, linearise_softmax
-        ) as modified_model:
+        with self.context(wrapper, composite, replace_onnx2torch, linearise_softmax) as modified_model:
             output, input_tensor = modified_model.predict(
                 boards,
                 with_grad=True,
                 input_requires_grad=True,
                 return_input=True,
             )
             if target is None:
-                output.backward(
-                    gradient=(
-                        output if init_rel_fn is None else init_rel_fn(output)
-                    )
-                )
+                output.backward(gradient=(output if init_rel_fn is None else init_rel_fn(output)))
             else:
                 output[target].backward(
-                    gradient=(
-                        output[target]
-                        if init_rel_fn is None
-                        else init_rel_fn(output[target])
-                    )
+                    gradient=(output[target] if init_rel_fn is None else init_rel_fn(output[target]))
                 )
         return input_tensor.grad
 
     @staticmethod
     def make_default_composite():
         canonizers = [SequentialMergeBatchNorm()]
 
@@ -179,29 +166,25 @@
 
         for name, module in wrapper.model.named_modules():
             if linearise_softmax:
                 if isinstance(module, torch.nn.Softmax):
                     new_module_mapping[name] = torch.nn.Identity()
                     old_module_mapping[name] = module
             if replace_onnx2torch:
-                if isinstance(
-                    module, onnx2torch.node_converters.OnnxBinaryMathOperation
-                ):
+                if isinstance(module, onnx2torch.node_converters.OnnxBinaryMathOperation):
                     if module.math_op_function is torch.add:
                         new_module_mapping[name] = lrp_helpers.AddEpsilon()
                         old_module_mapping[name] = module
                     elif module.math_op_function is torch.mul:
                         new_module_mapping[name] = lrp_helpers.MulUniform()
                         old_module_mapping[name] = module
                 elif isinstance(module, onnx2torch.node_converters.OnnxMatMul):
                     new_module_mapping[name] = lrp_helpers.MatMulEpsilon()
                     old_module_mapping[name] = module
-                elif isinstance(
-                    module, onnx2torch.node_converters.OnnxFunction
-                ):
+                elif isinstance(module, onnx2torch.node_converters.OnnxFunction):
                     if module.function is torch.tanh:
                         new_module_mapping[name] = torch.nn.Tanh()
                         old_module_mapping[name] = module
                 elif isinstance(
                     module,
                     onnx2torch.node_converters.OnnxGlobalAveragePoolWithKnownInputShape,  # noqa
                 ):
```

### Comparing `lczerolens-0.1.2/src/lczerolens/xai/lenses/patching.py` & `lczerolens-0.2.0/src/lczerolens/xai/lenses/patching.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-"""Patching lens for XAI.
-"""
+"""Patching lens for XAI."""
 
 from typing import Callable, Dict, Optional
 
 import chess
 import torch
 from torch.utils.data import Dataset
 
-from lczerolens.game.wrapper import ModelWrapper
+from lczerolens.model.wrapper import ModelWrapper
 from lczerolens.xai.hook import HookConfig, ModifyHook
 from lczerolens.xai.lens import Lens
 
 
 @Lens.register("patching")
 class PatchingLens(Lens):
     """
     Class for patching-based XAI methods.
     """
 
     def __init__(self, patching_dict: Dict[str, Callable]):
         self.patching_dict = patching_dict
         self.modify_hooks = {}
         for module_name, patch in self.patching_dict.items():
-            self.modify_hooks[module_name] = ModifyHook(
-                HookConfig(module_exp=module_name, data_fn=patch)
-            )
+            self.modify_hooks[module_name] = ModifyHook(HookConfig(module_exp=module_name, data_fn=patch))
 
     def is_compatible(self, wrapper: ModelWrapper) -> bool:
         """
         Returns whether the lens is compatible with the model.
         """
         return isinstance(wrapper.model, torch.nn.Module)
 
@@ -59,17 +56,15 @@
         **kwargs,
     ) -> dict:
         """
         Analyse a dataset with the probing lens.
         """
         if save_to is not None:
             raise NotImplementedError("Saving to file is not implemented.")
-        dataloader = torch.utils.data.DataLoader(
-            dataset, batch_size=batch_size, collate_fn=collate_fn
-        )
+        dataloader = torch.utils.data.DataLoader(dataset, batch_size=batch_size, collate_fn=collate_fn)
         batched_outs = None
         for modify_hook in self.modify_hooks.values():
             modify_hook.clear()
             modify_hook.register(wrapper.model)
         for batch in dataloader:
             _, boards = batch
             (out,) = wrapper.predict(boards)
```

### Comparing `lczerolens-0.1.2/src/lczerolens/xai/lenses/policy.py` & `lczerolens-0.2.0/src/lczerolens/xai/lenses/policy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-"""PolicyLens class for wrapping the LCZero models.
-"""
+"""PolicyLens class for wrapping the LCZero models."""
 
 from typing import Any, Callable, Dict, Optional
 
 import chess
 import torch
 from torch.utils.data import DataLoader, Dataset
 
-from lczerolens.game.wrapper import ModelWrapper, PolicyFlow
-from lczerolens.utils.constants import INVERTED_FROM_INDEX, INVERTED_TO_INDEX
+from lczerolens.encodings.constants import (
+    INVERTED_FROM_INDEX,
+    INVERTED_TO_INDEX,
+)
+from lczerolens.model.wrapper import ModelWrapper, PolicyFlow
 from lczerolens.xai.lens import Lens
 
 DEVICE = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 
 @Lens.register("policy")
 class PolicyLens(Lens):
@@ -71,14 +73,10 @@
             filtered_policy = torch.zeros(1858)
             topk = torch.topk(policy, aggregate_topk)
             filtered_policy[topk.indices] = topk.values
         else:
             filtered_policy = policy
         for square_index in range(64):
             square = chess.SQUARE_NAMES[square_index]
-            pickup_agg[square_index] = filtered_policy[
-                INVERTED_FROM_INDEX[square]
-            ].sum()
-            dropoff_agg[square_index] = filtered_policy[
-                INVERTED_TO_INDEX[square]
-            ].sum()
+            pickup_agg[square_index] = filtered_policy[INVERTED_FROM_INDEX[square]].sum()
+            dropoff_agg[square_index] = filtered_policy[INVERTED_TO_INDEX[square]].sum()
         return pickup_agg, dropoff_agg
```

### Comparing `lczerolens-0.1.2/src/lczerolens/xai/lenses/probing.py` & `lczerolens-0.2.0/src/lczerolens/xai/lenses/probing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Probing lens for XAI.
-"""
+"""Probing lens for XAI."""
 
 from typing import Any, Callable, Dict, Optional
 
 import chess
 import torch
 from torch.utils.data import Dataset
 
-from lczerolens.game.wrapper import ModelWrapper
+from lczerolens.model.wrapper import ModelWrapper
 from lczerolens.xai.hook import HookConfig, MeasureHook
 from lczerolens.xai.lens import Lens
 from lczerolens.xai.probe import Probe
 
 
 @Lens.register("probing")
 class ProbingLens(Lens):
@@ -19,17 +18,15 @@
     Class for probing-based XAI methods.
     """
 
     def __init__(self, probe_dict: Dict[str, Probe]):
         self.probe_dict = probe_dict
         self.measure_hooks = {}
         for module_name, probe in self.probe_dict.items():
-            self.measure_hooks[module_name] = MeasureHook(
-                HookConfig(module_exp=module_name, data_fn=probe.predict)
-            )
+            self.measure_hooks[module_name] = MeasureHook(HookConfig(module_exp=module_name, data_fn=probe.predict))
 
     def is_compatible(self, wrapper: ModelWrapper) -> bool:
         """
         Returns whether the lens is compatible with the model.
         """
         return isinstance(wrapper.model, torch.nn.Module)
 
@@ -62,29 +59,25 @@
         **kwargs,
     ) -> dict:
         """
         Analyse a dataset with the probing lens.
         """
         if save_to is not None:
             raise NotImplementedError("Saving to file is not implemented.")
-        dataloader = torch.utils.data.DataLoader(
-            dataset, batch_size=batch_size, collate_fn=collate_fn
-        )
+        dataloader = torch.utils.data.DataLoader(dataset, batch_size=batch_size, collate_fn=collate_fn)
         batched_measures: Dict[str, Any] = {}
         for measure_hook in self.measure_hooks.values():
             measure_hook.clear()
             measure_hook.register(wrapper.model)
         for batch in dataloader:
             indices, boards = batch
             wrapper.predict(boards)
             for module_name, measure_hook in self.measure_hooks.items():
                 if module_name not in batched_measures:
-                    batched_measures[module_name] = measure_hook.storage[
-                        module_name
-                    ]
+                    batched_measures[module_name] = measure_hook.storage[module_name]
                 else:
                     batched_measures[module_name] = torch.cat(
                         (
                             batched_measures[module_name],
                             measure_hook.storage[module_name],
                         ),
                         dim=0,
```

### Comparing `lczerolens-0.1.2/src/lczerolens/xai/probe.py` & `lczerolens-0.2.0/src/lczerolens/xai/probe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""Module to implement generic probing.
-"""
+"""Module to implement generic probing."""
 
 from abc import ABC, abstractmethod
 from typing import Any
 
 import einops
 import torch
 
@@ -50,17 +49,15 @@
         if len(labels.shape) != 2:
             raise ValueError("Labels must a batch of tensors")
 
         mean_activation = activations.mean(dim=1, keepdim=True)
         mean_label = labels.mean(dim=1, keepdim=True)
         scaled_activations = activations - mean_activation
         scaled_labels = labels - mean_label
-        cav = einops.einsum(
-            scaled_activations, scaled_labels, "b a, b d -> a d"
-        )
+        cav = einops.einsum(scaled_activations, scaled_labels, "b a, b d -> a d")
         self._h = cav / (cav.norm(dim=0, keepdim=True) + EPS)
 
     def predict(self, activations: torch.Tensor, **kwargs):
         if not self._trained:
             raise ValueError("Probe not trained")
 
         if len(activations.shape) != 2:
```

### Comparing `lczerolens-0.1.2/PKG-INFO` & `lczerolens-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lczerolens
-Version: 0.1.2
+Version: 0.2.0
 Summary: Interpretability for LeelaChessZero networks.
 License: MIT
 Author: Yoann Poupart
 Author-email: yoann.poupart@ens-lyon.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lczerolens Version: 0.1.2 Summary: Interpretability
+Metadata-Version: 2.1 Name: lczerolens Version: 0.2.0 Summary: Interpretability
 for LeelaChessZero networks. License: MIT Author: Yoann Poupart Author-email:
 yoann.poupart@ens-lyon.org Requires-Python: >=3.9,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: demo Requires-Dist: einops (>=0.7.0,<0.8.0) Requires-Dist:
 gradio (>=4.14.0,<5.0.0) ; extra == "demo" Requires-Dist: jsonlines
```

