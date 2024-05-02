# Comparing `tmp/onnxscript-0.1.0.dev20240430.tar.gz` & `tmp/onnxscript-0.1.0.dev20240501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnxscript-0.1.0.dev20240430.tar", last modified: Tue Apr 30 00:01:08 2024, max compression
+gzip compressed data, was "onnxscript-0.1.0.dev20240501.tar", last modified: Wed May  1 00:02:14 2024, max compression
```

## Comparing `onnxscript-0.1.0.dev20240430.tar` & `onnxscript-0.1.0.dev20240501.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.268138 onnxscript-0.1.0.dev20240430/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-04-30 00:01:08.268138 onnxscript-0.1.0.dev20240430/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/VERSION
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.208137 onnxscript-0.1.0.dev20240430/onnxscript/
--rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.212137 onnxscript-0.1.0.dev20240430/onnxscript/_internal/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/_internal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/_internal/analysis.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/_internal/ast_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/_internal/autocast.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/_internal/deprecation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/_internal/param_manipulation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/_internal/runtime_typing.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/_internal/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/_internal/version_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.212137 onnxscript-0.1.0.dev20240430/onnxscript/_legacy_ir/
--rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/_legacy_ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/_legacy_ir/visitor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.212137 onnxscript-0.1.0.dev20240430/onnxscript/_thirdparty/
--rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/_thirdparty/asciichartpy.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.212137 onnxscript-0.1.0.dev20240430/onnxscript/backend/
--rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/backend/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/backend/onnx_backend.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/backend/onnx_export.py
--rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/converter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.204137 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.212137 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/
--rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/_infra.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/context.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/decorator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/formatter.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.232138 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/
--rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_address.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_artifact.py
--rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_artifact_change.py
--rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_artifact_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_artifact_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_attachment.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_code_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_configuration_override.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_edge.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_exception.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_external_properties.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_fix.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_graph.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_invocation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_location_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_logical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_message.py
--rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_node.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_notification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_physical_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_property_bag.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_rectangle.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_region.py
--rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_replacement.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_result.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_result_provenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_run.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_sarif_log.py
--rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_special_locations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_stack.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_stack_frame.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_suppression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_thread_flow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
--rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_tool.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_tool_component.py
--rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_version_control_details.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_web_request.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_web_response.py
--rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/version.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/evaluator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.204137 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.204137 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/tools/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.232138 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/tools/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.236137 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/
--rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/_flags.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.236137 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/graph_building/
--rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/graph_building/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    27757 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43814 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.240138 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/
--rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/common.py
--rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/core.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/fft.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/linalg.py
--rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/nested.py
--rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/nn.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/prims.py
--rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/sparse.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/special.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/vision.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/registration.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/tensor_typing.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.244138 onnxscript-0.1.0.dev20240430/onnxscript/ir/
--rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/ir/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8474 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/ir/_convenience.py
--rw-r--r--   0 vsts      (1001) docker     (127)    77357 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/ir/_core.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/ir/_display.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3908 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/ir/_enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/ir/_graph_comparison.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/ir/_invariants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/ir/_linked_list.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/ir/_metadata.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/ir/_name_authority.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19570 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/ir/_protocols.py
--rw-r--r--   0 vsts      (1001) docker     (127)    47188 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/ir/serde.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/irbuilder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.244138 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/
--rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.256138 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/
--rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset1.py
--rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset10.py
--rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset11.py
--rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset12.py
--rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset13.py
--rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset14.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset15.py
--rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset16.py
--rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset17.py
--rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset18.py
--rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset19.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset20.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset4.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset5.py
--rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset6.py
--rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset7.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset8.py
--rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset9.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/onnx_types.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.256138 onnxscript-0.1.0.dev20240430/onnxscript/optimizer/
--rw-r--r--   0 vsts      (1001) docker     (127)     4597 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/optimizer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/optimizer/constant_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/optimizer/copy_propagation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/optimizer/evaluator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/optimizer/fold_constants_v0.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/optimizer/remove_unused.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/optimizer/remove_unused_function.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/optimizer/simple_function_folding.py
--rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.260138 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/_ir_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/_tape.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6603 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/broadcast_to_matmul.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/cast_constant_of_shape.py
--rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/erfgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/function_rule.py
--rw-r--r--   0 vsts      (1001) docker     (127)      747 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/gemm_to_matmul_add.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35227 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/generic_pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)      832 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/no_op.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.264138 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/onnxruntime/
--rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/onnxruntime/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1257 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5522 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1930 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/onnxruntime/softmax.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.264138 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/onnxruntime/transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      602 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/onnxruntime/transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
--rw-r--r--   0 vsts      (1001) docker     (127)    29345 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36123 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/rewriter/pattern.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/sourceinfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/tensor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.264138 onnxscript-0.1.0.dev20240430/onnxscript/testing/
--rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/testing/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/type_annotation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.264138 onnxscript-0.1.0.dev20240430/onnxscript/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/utils/evaluation_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/utils/timing_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/utils/utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/onnxscript/values.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-30 00:01:08.264138 onnxscript-0.1.0.dev20240430/onnxscript.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-04-30 00:01:08.000000 onnxscript-0.1.0.dev20240430/onnxscript.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     8203 2024-04-30 00:01:08.000000 onnxscript-0.1.0.dev20240430/onnxscript.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-30 00:01:08.000000 onnxscript-0.1.0.dev20240430/onnxscript.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-04-30 00:01:08.000000 onnxscript-0.1.0.dev20240430/onnxscript.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-04-30 00:01:08.000000 onnxscript-0.1.0.dev20240430/onnxscript.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-30 00:01:08.268138 onnxscript-0.1.0.dev20240430/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-04-30 00:00:48.000000 onnxscript-0.1.0.dev20240430/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:14.008885 onnxscript-0.1.0.dev20240501/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      211 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-05-01 00:02:14.008885 onnxscript-0.1.0.dev20240501/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8680 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/VERSION
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:13.972884 onnxscript-0.1.0.dev20240501/onnxscript/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2282 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:13.976884 onnxscript-0.1.0.dev20240501/onnxscript/_internal/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/_internal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9313 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/_internal/analysis.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2228 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/_internal/ast_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9811 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/_internal/autocast.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2560 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/_internal/deprecation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5166 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/_internal/param_manipulation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1176 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/_internal/runtime_typing.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3523 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/_internal/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1018 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/_internal/version_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:13.976884 onnxscript-0.1.0.dev20240501/onnxscript/_legacy_ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)    11316 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/_legacy_ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36198 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/_legacy_ir/visitor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:13.976884 onnxscript-0.1.0.dev20240501/onnxscript/_thirdparty/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10608 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/_thirdparty/asciichartpy.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:13.976884 onnxscript-0.1.0.dev20240501/onnxscript/backend/
+-rw-r--r--   0 vsts      (1001) docker     (127)      247 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/backend/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11498 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/backend/onnx_backend.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30612 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/backend/onnx_export.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    61554 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/converter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:13.968884 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:13.980884 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/
+-rw-r--r--   0 vsts      (1001) docker     (127)      583 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11045 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/_infra.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13086 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/context.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5544 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/decorator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3364 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/formatter.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:13.988884 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4364 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1716 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_address.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2980 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_artifact.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      875 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_artifact_change.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      996 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_artifact_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1029 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_artifact_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1195 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_attachment.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_code_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      986 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_configuration_override.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1154 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      937 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_edge.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1065 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_edge_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1133 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3794 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_external_properties.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1089 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3819 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1034 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_fix.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1051 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_graph.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1388 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_graph_traversal.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4561 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_invocation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1552 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      946 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_location_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1282 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_logical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_message.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      787 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1036 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_node.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1892 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_notification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1305 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_physical_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      488 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_property_bag.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1141 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_rectangle.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2013 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_region.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      870 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_replacement.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1104 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2700 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1109 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1090 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5002 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_result.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_result_provenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5246 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_run.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_run_automation_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1198 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_sarif_log.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      751 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_special_locations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      824 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_stack.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1070 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_stack_frame.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1231 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_suppression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1333 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_thread_flow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2473 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      830 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_tool.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4941 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_tool_component.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      915 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_translation_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1391 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_version_control_details.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1498 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_web_request.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1566 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_web_response.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      193 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/version.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2515 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    22081 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/evaluator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:13.968884 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:13.968884 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/tools/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:13.988884 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/tools/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)    16361 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11767 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11834 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:13.992884 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/
+-rw-r--r--   0 vsts      (1001) docker     (127)      149 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       77 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1452 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/_flags.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:13.992884 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/graph_building/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2291 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/graph_building/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28280 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    44452 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:13.992884 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/
+-rw-r--r--   0 vsts      (1001) docker     (127)      208 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/common.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   290367 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12343 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/fft.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13256 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/linalg.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      911 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/nested.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    86028 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/nn.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20667 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/prims.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      920 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11262 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/special.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1155 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/vision.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5547 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/registration.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2118 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/tensor_typing.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:13.996884 onnxscript-0.1.0.dev20240501/onnxscript/ir/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2394 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/ir/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8474 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/ir/_convenience.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    77357 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/ir/_core.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1775 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/ir/_display.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3908 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/ir/_enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      900 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/ir/_graph_comparison.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1853 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/ir/_invariants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10518 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/ir/_linked_list.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1684 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/ir/_metadata.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1064 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/ir/_name_authority.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19570 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/ir/_protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    47188 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/ir/serde.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19643 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/irbuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6457 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/main.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:13.996884 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4852 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:14.004885 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/
+-rw-r--r--   0 vsts      (1001) docker     (127)   153815 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    53445 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset10.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   157597 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset11.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    43533 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset12.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   140743 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset13.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    41780 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset14.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19290 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset15.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    50662 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset16.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    21513 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset17.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    70208 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset18.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    75098 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset19.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7937 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28284 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset20.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7645 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1966 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2572 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset5.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33248 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset6.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    49053 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset7.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19393 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset8.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    58411 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset9.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39030 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4439 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13894 2024-05-01 00:00:56.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5368 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24713 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5875 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/onnx_types.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:14.004885 onnxscript-0.1.0.dev20240501/onnxscript/optimizer/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4597 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/optimizer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10166 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/optimizer/constant_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2872 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/optimizer/copy_propagation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15603 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/optimizer/evaluator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8554 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/optimizer/fold_constants_v0.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3994 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/optimizer/remove_unused.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2080 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/optimizer/remove_unused_function.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9852 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/optimizer/simple_function_folding.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       41 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:14.008885 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1342 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/_ir_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/_tape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6603 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/broadcast_to_matmul.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/cast_constant_of_shape.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      709 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/erfgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8567 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/function_rule.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      747 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/gemm_to_matmul_add.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35227 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/generic_pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      832 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/no_op.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:14.008885 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/onnxruntime/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2139 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/onnxruntime/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1257 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5522 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1930 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/onnxruntime/softmax.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:14.008885 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/onnxruntime/transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      602 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/onnxruntime/transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1019 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      826 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1647 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/onnxruntime/transformers/layernorm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    29345 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36123 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/rewriter/pattern.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1700 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/sourceinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7658 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/tensor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:14.008885 onnxscript-0.1.0.dev20240501/onnxscript/testing/
+-rw-r--r--   0 vsts      (1001) docker     (127)    17350 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/testing/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11025 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/type_annotation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:14.008885 onnxscript-0.1.0.dev20240501/onnxscript/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2239 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/utils/evaluation_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      706 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/utils/timing_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2505 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/utils/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    24803 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/onnxscript/values.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-01 00:02:14.008885 onnxscript-0.1.0.dev20240501/onnxscript.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    10863 2024-05-01 00:02:13.000000 onnxscript-0.1.0.dev20240501/onnxscript.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     8203 2024-05-01 00:02:13.000000 onnxscript-0.1.0.dev20240501/onnxscript.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-01 00:02:13.000000 onnxscript-0.1.0.dev20240501/onnxscript.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       35 2024-05-01 00:02:13.000000 onnxscript-0.1.0.dev20240501/onnxscript.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-01 00:02:13.000000 onnxscript-0.1.0.dev20240501/onnxscript.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     6453 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-05-01 00:02:14.008885 onnxscript-0.1.0.dev20240501/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1304 2024-05-01 00:00:57.000000 onnxscript-0.1.0.dev20240501/setup.py
```

### Comparing `onnxscript-0.1.0.dev20240430/LICENSE` & `onnxscript-0.1.0.dev20240501/LICENSE`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/PKG-INFO` & `onnxscript-0.1.0.dev20240501/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240430
+Version: 0.1.0.dev20240501
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-0.1.0.dev20240430/README.md` & `onnxscript-0.1.0.dev20240501/README.md`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/__init__.py` & `onnxscript-0.1.0.dev20240501/onnxscript/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/_internal/analysis.py` & `onnxscript-0.1.0.dev20240501/onnxscript/_internal/analysis.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/_internal/ast_utils.py` & `onnxscript-0.1.0.dev20240501/onnxscript/_internal/ast_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/_internal/autocast.py` & `onnxscript-0.1.0.dev20240501/onnxscript/_internal/autocast.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/_internal/deprecation.py` & `onnxscript-0.1.0.dev20240501/onnxscript/_internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/_internal/param_manipulation.py` & `onnxscript-0.1.0.dev20240501/onnxscript/_internal/param_manipulation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/_internal/runtime_typing.py` & `onnxscript-0.1.0.dev20240501/onnxscript/_internal/runtime_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/_internal/utils.py` & `onnxscript-0.1.0.dev20240501/onnxscript/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/_internal/version_utils.py` & `onnxscript-0.1.0.dev20240501/onnxscript/_internal/version_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/_legacy_ir/__init__.py` & `onnxscript-0.1.0.dev20240501/onnxscript/_legacy_ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/_legacy_ir/visitor.py` & `onnxscript-0.1.0.dev20240501/onnxscript/_legacy_ir/visitor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/_thirdparty/asciichartpy.py` & `onnxscript-0.1.0.dev20240501/onnxscript/_thirdparty/asciichartpy.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/backend/onnx_backend.py` & `onnxscript-0.1.0.dev20240501/onnxscript/backend/onnx_backend.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/backend/onnx_export.py` & `onnxscript-0.1.0.dev20240501/onnxscript/backend/onnx_export.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/converter.py` & `onnxscript-0.1.0.dev20240501/onnxscript/converter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/__init__.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/_infra.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/_infra.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/context.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/context.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/decorator.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/decorator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/formatter.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/formatter.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/__init__.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_address.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_address.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_artifact.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_artifact.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_artifact_change.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_artifact_change.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_artifact_content.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_artifact_content.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_artifact_location.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_artifact_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_attachment.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_attachment.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_code_flow.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_code_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_configuration_override.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_configuration_override.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_conversion.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_conversion.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_edge.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_edge.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_edge_traversal.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_edge_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_exception.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_exception.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_external_properties.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_external_properties.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_external_property_file_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_external_property_file_references.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_fix.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_fix.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_graph.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_graph.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_graph_traversal.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_graph_traversal.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_invocation.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_invocation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_location.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_location_relationship.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_location_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_logical_location.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_logical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_message.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_message.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_multiformat_message_string.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_node.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_node.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_notification.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_notification.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_physical_location.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_physical_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_rectangle.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_rectangle.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_region.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_region.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_replacement.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_replacement.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_reporting_configuration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_reporting_descriptor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_reporting_descriptor_relationship.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_result.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_result.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_result_provenance.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_result_provenance.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_run.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_run.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_run_automation_details.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_run_automation_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_sarif_log.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_sarif_log.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_special_locations.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_special_locations.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_stack.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_stack.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_stack_frame.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_stack_frame.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_suppression.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_suppression.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_thread_flow.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_thread_flow.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_thread_flow_location.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_tool.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_tool.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_tool_component.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_tool_component.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_tool_component_reference.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_translation_metadata.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_translation_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_version_control_details.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_version_control_details.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_web_request.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_web_request.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/sarif/_web_response.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/sarif/_web_response.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/diagnostics/infra/utils.py` & `onnxscript-0.1.0.dev20240501/onnxscript/diagnostics/infra/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/evaluator.py` & `onnxscript-0.1.0.dev20240501/onnxscript/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py` & `onnxscript-0.1.0.dev20240501/onnxscript/function_libs/tools/torch_lib/deduce_type_constraints.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py` & `onnxscript-0.1.0.dev20240501/onnxscript/function_libs/tools/torch_lib/generate_aten_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py` & `onnxscript-0.1.0.dev20240501/onnxscript/function_libs/tools/torch_lib/generate_prims_signatures.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/_flags.py` & `onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/_flags.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/graph_building/__init__.py` & `onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/graph_building/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py` & `onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/graph_building/_graph_building_ir.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
         index=None,
         name: str | None = None,
     ):
         onnxscript_tensor.Tensor.__init__(self, None)
         ir.Value.__init__(self, producer, index=index, name=name)
         self._is_complex: bool = False
         self._concrete_value: np.ndarray | None = None
+        self._device: torch.device | None = None
 
     @property
     def value(self) -> Optional[np.ndarray]:
         return self._concrete_value
 
     @value.setter
     def value(self, value: np.ndarray) -> None:
@@ -146,14 +147,24 @@
         else:
             onnx_dtype = _torch_dtype_to_onnx_dtype(dtype)
         if self._type is None:
             self._type = ir.TensorType(onnx_dtype)
         else:
             self._type.dtype = onnx_dtype
 
+    # TODO: Remove this when there is no mismatch output shapes between device:
+    # https://github.com/pytorch/pytorch/blob/a44f8894fa6d973693aab44a3dda079a168b05c1/torch/_decomp/decompositions.py#L1451-L1457
+    @property
+    def device(self) -> torch.device | None:
+        return self._device
+
+    @device.setter
+    def device(self, device: torch.device):
+        self._device = device
+
     @property
     def is_complex(self) -> bool:
         return self._is_complex
 
     @is_complex.setter
     def is_complex(self, is_complex: bool):
         self._is_complex = is_complex
@@ -437,22 +448,24 @@
         return self._domain_name
 
     def add_input(
         self,
         input_name: Optional[str],
         shape: Optional[Union[torch.Size, Tuple[Union[int, str, None], ...]]] = None,
         dtype: Optional[torch.dtype] = None,
+        device: Optional[torch.device] = None,
     ) -> TorchScriptTensor | None:
         if input_name is None:
             # This input argument is None, which is mapped
             # to a NULL value in TorchScript type system.
             value = None
         else:
             value = TorchScriptTensor(name=input_name)
             value.shape = shape  # type: ignore[arg-type,assignment]
+            value.device = device
             if dtype is not None:
                 value.dtype = dtype  # type: ignore[assignment]
             # TODO(titaiwang): This approach loses the information that "same SymInts
             # indicates same shape", for example, [symint0, symint0, symint1]
             # would all be [None, None, None]
             # torch_value.setType(
             #     torch_value.type().with_sizes(
```

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py` & `onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/graph_building/_graph_building_torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
         super().__init__(None)
         self._torch_value: torch.Value = value
         self._concrete_value: Optional[np.ndarray] = None
         self._shape: Optional[Tuple[int | str | None, ...]] = None
         self._torch_dtype: Optional[torch.dtype] = None
         self._name: Optional[str] = None
         self._is_complex: bool = False
+        self._device: Optional[torch.device] = None
 
     def __repr__(self):
         return f"TorchScriptTensor('{self._torch_value!r}')"
 
     @property  # type: ignore[override]
     def value(self) -> Optional[np.ndarray]:
         return self._concrete_value
@@ -202,14 +203,24 @@
     def is_complex(self) -> bool:
         return self._is_complex
 
     @is_complex.setter
     def is_complex(self, is_complex: bool):
         self._is_complex = is_complex
 
+    # TODO: Remove this when there is no mismatch output shapes between device:
+    # https://github.com/pytorch/pytorch/blob/a44f8894fa6d973693aab44a3dda079a168b05c1/torch/_decomp/decompositions.py#L1451-L1457
+    @property
+    def device(self) -> torch.device | None:
+        return self._device
+
+    @device.setter
+    def device(self, device: torch.device):
+        self._device = device
+
     @property
     def onnx_dtype(self):
         # Local import to avoid circular dependency
         from torch.onnx import _type_utils  # pylint: disable=import-outside-toplevel
 
         return _type_utils.JitScalarType.from_value(  # type: ignore[attr-defined]
             self._torch_value, _type_utils.JitScalarType.UNDEFINED
@@ -258,27 +269,30 @@
 def _wrap_torch_value_to_tensor(
     value: Union[
         torch.Value, Mapping[str, ValidTorchValueType], Sequence[ValidTorchValueType]
     ],
     *,
     shape: Optional[Union[torch.Size, Tuple[Union[int, str, None], ...]]] = None,
     dtype: Optional[torch.dtype] = None,
+    device: Optional[torch.device] = None,
 ) -> Union[
     ValidArgumentType,
     Dict[str, ValidArgumentType],
     List[ValidArgumentType],
     Tuple[ValidArgumentType, ...],
 ]:
     """Wrap torch.Value to TorchScriptTensor."""
     if isinstance(value, torch.Value):
         tensor = TorchScriptTensor(value)
         if shape is not None:
             tensor.shape = shape
         if dtype is not None:
             tensor.dtype = dtype
+        if device is not None:
+            tensor.device = device
         return tensor
     if isinstance(value, dict):
         return {k: _wrap_torch_value_to_tensor(v) for k, v in value.items()}  # type: ignore[misc,return-value]
     if isinstance(value, list):
         return [_wrap_torch_value_to_tensor(v) for v in value]  # type: ignore[misc,return-value]
     if isinstance(value, tuple):
         return tuple(_wrap_torch_value_to_tensor(v) for v in value)  # type: ignore[misc,return-value]
@@ -570,14 +584,15 @@
 
     @runtime_typing.checked
     def add_input(
         self,
         input_name: Optional[str],
         shape: Optional[Union[torch.Size, Tuple[Union[int, str, None], ...]]] = None,
         dtype: Optional[torch.dtype] = None,
+        device: Optional[torch.device] = None,
     ) -> TorchScriptTensor:
         if input_name is None:
             # This input argument is None, which is mapped
             # to a NULL value in TorchScript type system.
             torch_value = _create_op_call_in_torch_graph(
                 self._torch_graph, "prim::Constant", inputs=(), attributes={}
             )[0]
@@ -589,15 +604,17 @@
             # indicates same shape", for example, [symint0, symint0, symint1]
             # would all be [None, None, None]
             torch_value.setType(
                 torch_value.type().with_sizes(
                     [dim if isinstance(dim, int) else None for dim in shape]  # type: ignore[union-attr]
                 )
             )
-        tensor_value = _wrap_torch_value_to_tensor(torch_value, shape=shape, dtype=dtype)
+        tensor_value = _wrap_torch_value_to_tensor(
+            torch_value, shape=shape, dtype=dtype, device=device
+        )
         if isinstance(tensor_value, TorchScriptTensor):
             # NOTE: Only track value that maps to tensor.
             # Value that maps to Sequence/Dict of tensors is not tracked.
             self._value_to_tensor[torch_value] = tensor_value
         return tensor_value  # type: ignore[return-value]
 
     @runtime_typing.checked
```

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/common.py` & `onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/common.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/core.py` & `onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/fft.py` & `onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/fft.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/linalg.py` & `onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/nested.py` & `onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/nested.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/nn.py` & `onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/nn.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/prims.py` & `onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/prims.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/sparse.py` & `onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/sparse.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/special.py` & `onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/special.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/ops/vision.py` & `onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/ops/vision.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/registration.py` & `onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/registration.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/function_libs/torch_lib/tensor_typing.py` & `onnxscript-0.1.0.dev20240501/onnxscript/function_libs/torch_lib/tensor_typing.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/ir/__init__.py` & `onnxscript-0.1.0.dev20240501/onnxscript/ir/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/ir/_convenience.py` & `onnxscript-0.1.0.dev20240501/onnxscript/ir/_convenience.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/ir/_core.py` & `onnxscript-0.1.0.dev20240501/onnxscript/ir/_core.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/ir/_display.py` & `onnxscript-0.1.0.dev20240501/onnxscript/ir/_display.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/ir/_enums.py` & `onnxscript-0.1.0.dev20240501/onnxscript/ir/_enums.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/ir/_graph_comparison.py` & `onnxscript-0.1.0.dev20240501/onnxscript/ir/_graph_comparison.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/ir/_invariants.py` & `onnxscript-0.1.0.dev20240501/onnxscript/ir/_invariants.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/ir/_linked_list.py` & `onnxscript-0.1.0.dev20240501/onnxscript/ir/_linked_list.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/ir/_metadata.py` & `onnxscript-0.1.0.dev20240501/onnxscript/ir/_metadata.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/ir/_name_authority.py` & `onnxscript-0.1.0.dev20240501/onnxscript/ir/_name_authority.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/ir/_protocols.py` & `onnxscript-0.1.0.dev20240501/onnxscript/ir/_protocols.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/ir/serde.py` & `onnxscript-0.1.0.dev20240501/onnxscript/ir/serde.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/irbuilder.py` & `onnxscript-0.1.0.dev20240501/onnxscript/irbuilder.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/main.py` & `onnxscript-0.1.0.dev20240501/onnxscript/main.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/__init__.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset1.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset10.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset10.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset11.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset11.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset12.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset12.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset13.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset13.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset14.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset14.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset15.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset15.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset16.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset16.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset17.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset17.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset18.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset18.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset19.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset19.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset2.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset20.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset20.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset3.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset4.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset5.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset5.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset6.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset6.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset7.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset7.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset8.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset8.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset9.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset9.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml2.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml3.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset_ai_onnx_ml4.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_opset/_impl/opset_ai_onnx_preview_training1.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/onnx_types.py` & `onnxscript-0.1.0.dev20240501/onnxscript/onnx_types.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/optimizer/__init__.py` & `onnxscript-0.1.0.dev20240501/onnxscript/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/optimizer/constant_folding.py` & `onnxscript-0.1.0.dev20240501/onnxscript/optimizer/constant_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/optimizer/copy_propagation.py` & `onnxscript-0.1.0.dev20240501/onnxscript/optimizer/copy_propagation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/optimizer/evaluator.py` & `onnxscript-0.1.0.dev20240501/onnxscript/optimizer/evaluator.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/optimizer/fold_constants_v0.py` & `onnxscript-0.1.0.dev20240501/onnxscript/optimizer/fold_constants_v0.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/optimizer/remove_unused.py` & `onnxscript-0.1.0.dev20240501/onnxscript/optimizer/remove_unused.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/optimizer/remove_unused_function.py` & `onnxscript-0.1.0.dev20240501/onnxscript/optimizer/remove_unused_function.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/optimizer/simple_function_folding.py` & `onnxscript-0.1.0.dev20240501/onnxscript/optimizer/simple_function_folding.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/rewriter/__init__.py` & `onnxscript-0.1.0.dev20240501/onnxscript/rewriter/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/rewriter/_ir_utils.py` & `onnxscript-0.1.0.dev20240501/onnxscript/rewriter/_ir_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/rewriter/_tape.py` & `onnxscript-0.1.0.dev20240501/onnxscript/rewriter/_tape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/rewriter/broadcast_to_matmul.py` & `onnxscript-0.1.0.dev20240501/onnxscript/rewriter/broadcast_to_matmul.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/rewriter/cast_constant_of_shape.py` & `onnxscript-0.1.0.dev20240501/onnxscript/rewriter/cast_constant_of_shape.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/rewriter/erfgelu.py` & `onnxscript-0.1.0.dev20240501/onnxscript/rewriter/erfgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/rewriter/function_rule.py` & `onnxscript-0.1.0.dev20240501/onnxscript/rewriter/function_rule.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/rewriter/gemm_to_matmul_add.py` & `onnxscript-0.1.0.dev20240501/onnxscript/rewriter/gemm_to_matmul_add.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/rewriter/generic_pattern.py` & `onnxscript-0.1.0.dev20240501/onnxscript/rewriter/generic_pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/rewriter/no_op.py` & `onnxscript-0.1.0.dev20240501/onnxscript/rewriter/no_op.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/rewriter/onnxruntime/__init__.py` & `onnxscript-0.1.0.dev20240501/onnxscript/rewriter/onnxruntime/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py` & `onnxscript-0.1.0.dev20240501/onnxscript/rewriter/onnxruntime/group_normalization_merge_silu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py` & `onnxscript-0.1.0.dev20240501/onnxscript/rewriter/onnxruntime/instance_to_group_normalization.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/rewriter/onnxruntime/softmax.py` & `onnxscript-0.1.0.dev20240501/onnxscript/rewriter/onnxruntime/softmax.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/rewriter/onnxruntime/transformers/__init__.py` & `onnxscript-0.1.0.dev20240501/onnxscript/rewriter/onnxruntime/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py` & `onnxscript-0.1.0.dev20240501/onnxscript/rewriter/onnxruntime/transformers/biassplitgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py` & `onnxscript-0.1.0.dev20240501/onnxscript/rewriter/onnxruntime/transformers/fastgelu.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/rewriter/onnxruntime/transformers/layernorm.py` & `onnxscript-0.1.0.dev20240501/onnxscript/rewriter/onnxruntime/transformers/layernorm.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py` & `onnxscript-0.1.0.dev20240501/onnxscript/rewriter/onnxruntime/transformers/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/rewriter/pattern.py` & `onnxscript-0.1.0.dev20240501/onnxscript/rewriter/pattern.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/sourceinfo.py` & `onnxscript-0.1.0.dev20240501/onnxscript/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/tensor.py` & `onnxscript-0.1.0.dev20240501/onnxscript/tensor.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/testing/__init__.py` & `onnxscript-0.1.0.dev20240501/onnxscript/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/type_annotation.py` & `onnxscript-0.1.0.dev20240501/onnxscript/type_annotation.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/utils/evaluation_utils.py` & `onnxscript-0.1.0.dev20240501/onnxscript/utils/evaluation_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/utils/timing_utils.py` & `onnxscript-0.1.0.dev20240501/onnxscript/utils/timing_utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/utils/utils.py` & `onnxscript-0.1.0.dev20240501/onnxscript/utils/utils.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript/values.py` & `onnxscript-0.1.0.dev20240501/onnxscript/values.py`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript.egg-info/PKG-INFO` & `onnxscript-0.1.0.dev20240501/onnxscript.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnxscript
-Version: 0.1.0.dev20240430
+Version: 0.1.0.dev20240501
 Summary: Naturally author ONNX functions and models using a subset of Python
 Author-email: Microsoft Corporation <onnx@microsoft.com>
 License: MIT License
         
         Copyright (c) Microsoft Corporation
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `onnxscript-0.1.0.dev20240430/onnxscript.egg-info/SOURCES.txt` & `onnxscript-0.1.0.dev20240501/onnxscript.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/pyproject.toml` & `onnxscript-0.1.0.dev20240501/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onnxscript-0.1.0.dev20240430/setup.py` & `onnxscript-0.1.0.dev20240501/setup.py`

 * *Files identical despite different names*

