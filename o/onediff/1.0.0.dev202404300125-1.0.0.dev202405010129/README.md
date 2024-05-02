# Comparing `tmp/onediff-1.0.0.dev202404300125.tar.gz` & `tmp/onediff-1.0.0.dev202405010129.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onediff-1.0.0.dev202404300125.tar", last modified: Tue Apr 30 01:26:03 2024, max compression
+gzip compressed data, was "onediff-1.0.0.dev202405010129.tar", last modified: Wed May  1 01:29:37 2024, max compression
```

## Comparing `onediff-1.0.0.dev202404300125.tar` & `onediff-1.0.0.dev202405010129.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:26:03.620522 onediff-1.0.0.dev202404300125/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-30 01:25:57.000000 onediff-1.0.0.dev202404300125/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14564 2024-04-30 01:26:03.620522 onediff-1.0.0.dev202404300125/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13517 2024-04-30 01:25:57.000000 onediff-1.0.0.dev202404300125/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 01:26:03.620522 onediff-1.0.0.dev202404300125/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:26:03.608522 onediff-1.0.0.dev202404300125/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:26:03.608522 onediff-1.0.0.dev202404300125/src/infer_compiler_registry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/infer_compiler_registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:26:03.612522 onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_diffusers/
--rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77110 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24007 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:26:03.612522 onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_diffusers_enterprise_lite/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:26:03.612522 onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_onediff_quant/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_onediff_quant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:26:03.612522 onediff-1.0.0.dev202404300125/src/onediff/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:26:03.612522 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:26:03.612522 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/backends/oneflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/backends/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/deployable_module.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:26:03.612522 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/import_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/import_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/import_tools/format_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/import_tools/import_module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/import_tools/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:26:03.616522 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/oneflow/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/oneflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/oneflow/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/oneflow/deployable_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/oneflow/dual_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/oneflow/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/oneflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:26:03.616522 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/transform/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15009 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/transform/builtin_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/transform/custom_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/transform/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/transform/patch_for_comfy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:26:03.616522 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/args_tree_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/cost_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/graph_management_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/model_inplace_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/module_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/oneflow_exec_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/online_quantization_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/param_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/patch_for_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/patch_for_diffusers.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/version_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/with_fx_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/with_fx_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/with_onediff_compile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:26:03.620522 onediff-1.0.0.dev202404300125/src/onediff/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/optimization/attention_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/optimization/quant_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/optimization/rewrite_self_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:26:03.620522 onediff-1.0.0.dev202404300125/src/onediff/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/quantization/load_quantized_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/quantization/quant_pipeline_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/quantization/quantize_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/quantization/quantize_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:26:03.620522 onediff-1.0.0.dev202404300125/src/onediff/schedulers/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/src/onediff/schedulers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:26:03.620522 onediff-1.0.0.dev202404300125/src/onediff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14564 2024-04-30 01:26:03.000000 onediff-1.0.0.dev202404300125/src/onediff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-30 01:26:03.000000 onediff-1.0.0.dev202404300125/src/onediff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 01:26:03.000000 onediff-1.0.0.dev202404300125/src/onediff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-30 01:26:03.000000 onediff-1.0.0.dev202404300125/src/onediff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-30 01:26:03.000000 onediff-1.0.0.dev202404300125/src/onediff.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 01:26:03.620522 onediff-1.0.0.dev202404300125/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/tests/test_dual_module_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/tests/test_pipelines_oneflow_img2img.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/tests/test_quantitative_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-30 01:25:58.000000 onediff-1.0.0.dev202404300125/tests/test_quantize_custom_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:29:37.510521 onediff-1.0.0.dev202405010129/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14685 2024-05-01 01:29:37.510521 onediff-1.0.0.dev202405010129/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13638 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 01:29:37.510521 onediff-1.0.0.dev202405010129/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:29:37.494521 onediff-1.0.0.dev202405010129/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:29:37.498521 onediff-1.0.0.dev202405010129/src/infer_compiler_registry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/infer_compiler_registry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:29:37.498521 onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_diffusers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77110 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_diffusers/resnet_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24007 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60934 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14590 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24101 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:29:37.498521 onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_diffusers_enterprise_lite/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:29:37.498521 onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_onediff_quant/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_onediff_quant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:29:37.498521 onediff-1.0.0.dev202405010129/src/onediff/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:29:37.498521 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:29:37.502521 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/backends/oneflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/backends/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/deployable_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:29:37.502521 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/import_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/import_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/import_tools/format_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/import_tools/import_module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/import_tools/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:29:37.502521 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/oneflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/oneflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7661 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/oneflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/oneflow/deployable_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/oneflow/dual_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/oneflow/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/oneflow/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:29:37.502521 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15009 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/transform/builtin_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/transform/custom_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/transform/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/transform/patch_for_comfy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:29:37.506521 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/args_tree_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/cost_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/graph_management_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/model_inplace_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/module_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/oneflow_exec_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/online_quantization_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/param_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/patch_for_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/patch_for_diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/version_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/with_fx_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/with_fx_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/with_onediff_compile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:29:37.506521 onediff-1.0.0.dev202405010129/src/onediff/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/optimization/attention_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/optimization/quant_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/optimization/rewrite_self_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:29:37.506521 onediff-1.0.0.dev202405010129/src/onediff/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/quantization/load_quantized_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/quantization/quant_pipeline_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/quantization/quantize_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/quantization/quantize_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:29:37.506521 onediff-1.0.0.dev202405010129/src/onediff/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/src/onediff/schedulers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:29:37.510521 onediff-1.0.0.dev202405010129/src/onediff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14685 2024-05-01 01:29:37.000000 onediff-1.0.0.dev202405010129/src/onediff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-01 01:29:37.000000 onediff-1.0.0.dev202405010129/src/onediff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 01:29:37.000000 onediff-1.0.0.dev202405010129/src/onediff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-01 01:29:37.000000 onediff-1.0.0.dev202405010129/src/onediff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-01 01:29:37.000000 onediff-1.0.0.dev202405010129/src/onediff.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 01:29:37.510521 onediff-1.0.0.dev202405010129/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/tests/test_dual_module_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11281 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/tests/test_pipelines_oneflow_img2img.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/tests/test_quantitative_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-01 01:29:31.000000 onediff-1.0.0.dev202405010129/tests/test_quantize_custom_model.py
```

### Comparing `onediff-1.0.0.dev202404300125/LICENSE` & `onediff-1.0.0.dev202405010129/LICENSE`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/PKG-INFO` & `onediff-1.0.0.dev202405010129/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.0.0.dev202404300125
+Version: 1.0.0.dev202405010129
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: caishenghang@oneflow.org
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -71,14 +71,16 @@
 - [Create an issue](https://github.com/siliconflow/onediff/issues)
 - Chat in Discord: [![](https://dcbadge.vercel.app/api/server/RKJTjZMcPQ?style=plastic)](https://discord.gg/RKJTjZMcPQ)
 - Email for Enterprise Edition or other business inquiries: contact@siliconflow.com
 
 ## OS and GPU Compatibility
 - Linux
   - If you want to use OneDiff on Windows, please use it under WSL.
+  - [The guide to install OneDiff in WSL2](https://github.com/siliconflow/onediff/wiki/Run-OneDiff-on-Windows-by-WSL2).
+
 - NVIDIA GPUs
   - [Compatibility with Nvidia GPUs](https://github.com/siliconflow/onediff/wiki/Compatibility-with-Nvidia-GPUs).
 
 ---
 The Full Introduction of OneDiff:
 <!-- toc -->
 - [About OneDiff](#about-onediff)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202404300125 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202405010129 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
 caishenghang@oneflow.org License: Apache Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
@@ -45,59 +45,60 @@
 comments/18lz2ir/accelerating_sdxl_3x_faster_with_deepcache_and/) ## Community
 and Support [Here is the introduction of OneDiff Community.](https://
 github.com/siliconflow/onediff/wiki#onediff-community) - [Create an issue]
 (https://github.com/siliconflow/onediff/issues) - Chat in Discord: [![](https:/
 /dcbadge.vercel.app/api/server/RKJTjZMcPQ?style=plastic)](https://discord.gg/
 RKJTjZMcPQ) - Email for Enterprise Edition or other business inquiries:
 contact@siliconflow.com ## OS and GPU Compatibility - Linux - If you want to
-use OneDiff on Windows, please use it under WSL. - NVIDIA GPUs - [Compatibility
-with Nvidia GPUs](https://github.com/siliconflow/onediff/wiki/Compatibility-
-with-Nvidia-GPUs). --- The Full Introduction of OneDiff: - [About OneDiff]
-(#about-onediff) - [Architecture](#architecture) - [State-of-the-art
-performance](#state-of-the-art-performance) - [Features](#features) -
-[Acceleration for State-of-the-art models](#acceleration-for-state-of-the-art-
-models) - [Acceleration for production environment](#acceleration-for-
-production-environment) - [OneDiff Quality Evalution](#onediff-quality-
-evaluation) - [OneDiff Enterprise Edition](#onediff-enterprise-edition) -
-[Installation](#installation) - [Release](#release) ## About OneDiff ###
-Architecture OneDiff interfaces with various front-end sd frameworks upward,
-and uses a custom virtual machine mixed with PyTorch as the inference engine
-downward. [imgs/onediff_arch.png]### State-of-the-art performance #### SDXL E2E
-time - Model stabilityai/stable-diffusion-xl-base-1.0; - Image size 1024*1024,
-batch size 1, steps 30; - NVIDIA A100 80G SXM4; [imgs/0_12_sdxl.png]#### SVD
-E2E time - Model stabilityai/stable-video-diffusion-img2vid-xt; - Image size
-576*1024, batch size 1, steps 25, decoder chunk size 5; - NVIDIA A100 80G SXM4;
-[imgs/0_12_svd.png]Note that we haven't got the way to run SVD with TensorRT on
-Feb 29 2024. ### Features | Main Function | Details | |----------------|-------
----------------------| | Compiling Time | About 1 minute (SDXL) | | Deployment
-Methods | Plug and Play | | Dynamic Image Size Support | Support with no
-overhead | | Model Support | SD1.5~2.1, SDXL, SDXL Turbo, etc. | | Algorithm
-Support | SD standard workflow, LoRA, ControlNet, SVD, InstantID, SDXL
-Lightning, etc. | | SD Framework Support | ComfyUI, Diffusers, SD-webui | |
-Save & Load Accelerated Models | Yes | | Time of LoRA Switching | Hundreds of
-milliseconds | | LoRA Occupancy | Tens of MB to hundreds of MB. | | Device
-Support | NVIDIA GPU 3090 RTX/4090 RTX/A100/A800/A10 etc. (Compatibility with
-Ascend in progress) | ### Acceleration for State-of-the-art models OneDiff
-supports the acceleration for SOTA models. * stable: release for public usage,
-and has long-term support; * beta: release for professional usage, and has
-long-term support; * alpha: early release for expert usage, and should be
-careful to use; | AIGC Type | Models | HF diffusers | | ComfyUI | | SD web UI |
-| | --------- | --------------------------- | ------------ | ---------- | -----
----- | ---------- | --------- | ---------- | | | | Community | Enterprise |
-Community | Enterprise | Community | Enterprise | | Image | SD 1.5 | stable |
-stable | stable | stable | stable | stable | | | SD 2.1 | stable | stable |
-stable | stable | stable | stable | | | SDXL | stable | stable | stable |
-stable | stable | stable | | | LoRA | stable | | stable | | stable | | | |
-ControlNet | stable | | stable | | | | | | SDXL Turbo | stable | | stable | | |
-| | | LCM | stable | | stable | | | | | | SDXL DeepCache | alpha | alpha |
-alpha | alpha | | | | | InstantID | beta | | beta | | | | | Video | SVD(stable
-Video Diffusion) | stable | stable | stable | stable | | | | | SVD DeepCache |
-alpha | alpha | alpha | alpha | | | **Note: Enterprise Edition contains all the
-functionality in Community Edition.** ### Acceleration for production
-environment #### PyTorch Module compilation - [compilation with
+use OneDiff on Windows, please use it under WSL. - [The guide to install
+OneDiff in WSL2](https://github.com/siliconflow/onediff/wiki/Run-OneDiff-on-
+Windows-by-WSL2). - NVIDIA GPUs - [Compatibility with Nvidia GPUs](https://
+github.com/siliconflow/onediff/wiki/Compatibility-with-Nvidia-GPUs). --- The
+Full Introduction of OneDiff: - [About OneDiff](#about-onediff) -
+[Architecture](#architecture) - [State-of-the-art performance](#state-of-the-
+art-performance) - [Features](#features) - [Acceleration for State-of-the-art
+models](#acceleration-for-state-of-the-art-models) - [Acceleration for
+production environment](#acceleration-for-production-environment) - [OneDiff
+Quality Evalution](#onediff-quality-evaluation) - [OneDiff Enterprise Edition]
+(#onediff-enterprise-edition) - [Installation](#installation) - [Release]
+(#release) ## About OneDiff ### Architecture OneDiff interfaces with various
+front-end sd frameworks upward, and uses a custom virtual machine mixed with
+PyTorch as the inference engine downward. [imgs/onediff_arch.png]### State-of-
+the-art performance #### SDXL E2E time - Model stabilityai/stable-diffusion-xl-
+base-1.0; - Image size 1024*1024, batch size 1, steps 30; - NVIDIA A100 80G
+SXM4; [imgs/0_12_sdxl.png]#### SVD E2E time - Model stabilityai/stable-video-
+diffusion-img2vid-xt; - Image size 576*1024, batch size 1, steps 25, decoder
+chunk size 5; - NVIDIA A100 80G SXM4; [imgs/0_12_svd.png]Note that we haven't
+got the way to run SVD with TensorRT on Feb 29 2024. ### Features | Main
+Function | Details | |----------------|----------------------------| |
+Compiling Time | About 1 minute (SDXL) | | Deployment Methods | Plug and Play |
+| Dynamic Image Size Support | Support with no overhead | | Model Support |
+SD1.5~2.1, SDXL, SDXL Turbo, etc. | | Algorithm Support | SD standard workflow,
+LoRA, ControlNet, SVD, InstantID, SDXL Lightning, etc. | | SD Framework Support
+| ComfyUI, Diffusers, SD-webui | | Save & Load Accelerated Models | Yes | |
+Time of LoRA Switching | Hundreds of milliseconds | | LoRA Occupancy | Tens of
+MB to hundreds of MB. | | Device Support | NVIDIA GPU 3090 RTX/4090 RTX/A100/
+A800/A10 etc. (Compatibility with Ascend in progress) | ### Acceleration for
+State-of-the-art models OneDiff supports the acceleration for SOTA models. *
+stable: release for public usage, and has long-term support; * beta: release
+for professional usage, and has long-term support; * alpha: early release for
+expert usage, and should be careful to use; | AIGC Type | Models | HF diffusers
+| | ComfyUI | | SD web UI | | | --------- | --------------------------- | -----
+------- | ---------- | --------- | ---------- | --------- | ---------- | | | |
+Community | Enterprise | Community | Enterprise | Community | Enterprise | |
+Image | SD 1.5 | stable | stable | stable | stable | stable | stable | | | SD
+2.1 | stable | stable | stable | stable | stable | stable | | | SDXL | stable |
+stable | stable | stable | stable | stable | | | LoRA | stable | | stable | |
+stable | | | | ControlNet | stable | | stable | | | | | | SDXL Turbo | stable |
+| stable | | | | | | LCM | stable | | stable | | | | | | SDXL DeepCache | alpha
+| alpha | alpha | alpha | | | | | InstantID | beta | | beta | | | | | Video |
+SVD(stable Video Diffusion) | stable | stable | stable | stable | | | | | SVD
+DeepCache | alpha | alpha | alpha | alpha | | | **Note: Enterprise Edition
+contains all the functionality in Community Edition.** ### Acceleration for
+production environment #### PyTorch Module compilation - [compilation with
 oneflow_compile](https://github.com/siliconflow/onediff/blob/main/
 onediff_diffusers_extensions/examples/text_to_image_sdxl.py) #### Avoid
 compilation time for new input shape - [Support Multi-resolution input](https:/
 /github.com/siliconflow/onediff/blob/main/onediff_diffusers_extensions/
 examples/text_to_image_sdxl.py) #### Avoid compilation time for online serving
 Compile and save the compiled result offline, then load it online for serving -
 [Save and Load the compiled graph](https://github.com/siliconflow/onediff/blob/
```

### Comparing `onediff-1.0.0.dev202404300125/README.md` & `onediff-1.0.0.dev202405010129/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 - [Create an issue](https://github.com/siliconflow/onediff/issues)
 - Chat in Discord: [![](https://dcbadge.vercel.app/api/server/RKJTjZMcPQ?style=plastic)](https://discord.gg/RKJTjZMcPQ)
 - Email for Enterprise Edition or other business inquiries: contact@siliconflow.com
 
 ## OS and GPU Compatibility
 - Linux
   - If you want to use OneDiff on Windows, please use it under WSL.
+  - [The guide to install OneDiff in WSL2](https://github.com/siliconflow/onediff/wiki/Run-OneDiff-on-Windows-by-WSL2).
+
 - NVIDIA GPUs
   - [Compatibility with Nvidia GPUs](https://github.com/siliconflow/onediff/wiki/Compatibility-with-Nvidia-GPUs).
 
 ---
 The Full Introduction of OneDiff:
 <!-- toc -->
 - [About OneDiff](#about-onediff)
```

#### html2text {}

```diff
@@ -31,59 +31,60 @@
 comments/18lz2ir/accelerating_sdxl_3x_faster_with_deepcache_and/) ## Community
 and Support [Here is the introduction of OneDiff Community.](https://
 github.com/siliconflow/onediff/wiki#onediff-community) - [Create an issue]
 (https://github.com/siliconflow/onediff/issues) - Chat in Discord: [![](https:/
 /dcbadge.vercel.app/api/server/RKJTjZMcPQ?style=plastic)](https://discord.gg/
 RKJTjZMcPQ) - Email for Enterprise Edition or other business inquiries:
 contact@siliconflow.com ## OS and GPU Compatibility - Linux - If you want to
-use OneDiff on Windows, please use it under WSL. - NVIDIA GPUs - [Compatibility
-with Nvidia GPUs](https://github.com/siliconflow/onediff/wiki/Compatibility-
-with-Nvidia-GPUs). --- The Full Introduction of OneDiff: - [About OneDiff]
-(#about-onediff) - [Architecture](#architecture) - [State-of-the-art
-performance](#state-of-the-art-performance) - [Features](#features) -
-[Acceleration for State-of-the-art models](#acceleration-for-state-of-the-art-
-models) - [Acceleration for production environment](#acceleration-for-
-production-environment) - [OneDiff Quality Evalution](#onediff-quality-
-evaluation) - [OneDiff Enterprise Edition](#onediff-enterprise-edition) -
-[Installation](#installation) - [Release](#release) ## About OneDiff ###
-Architecture OneDiff interfaces with various front-end sd frameworks upward,
-and uses a custom virtual machine mixed with PyTorch as the inference engine
-downward. [imgs/onediff_arch.png]### State-of-the-art performance #### SDXL E2E
-time - Model stabilityai/stable-diffusion-xl-base-1.0; - Image size 1024*1024,
-batch size 1, steps 30; - NVIDIA A100 80G SXM4; [imgs/0_12_sdxl.png]#### SVD
-E2E time - Model stabilityai/stable-video-diffusion-img2vid-xt; - Image size
-576*1024, batch size 1, steps 25, decoder chunk size 5; - NVIDIA A100 80G SXM4;
-[imgs/0_12_svd.png]Note that we haven't got the way to run SVD with TensorRT on
-Feb 29 2024. ### Features | Main Function | Details | |----------------|-------
----------------------| | Compiling Time | About 1 minute (SDXL) | | Deployment
-Methods | Plug and Play | | Dynamic Image Size Support | Support with no
-overhead | | Model Support | SD1.5~2.1, SDXL, SDXL Turbo, etc. | | Algorithm
-Support | SD standard workflow, LoRA, ControlNet, SVD, InstantID, SDXL
-Lightning, etc. | | SD Framework Support | ComfyUI, Diffusers, SD-webui | |
-Save & Load Accelerated Models | Yes | | Time of LoRA Switching | Hundreds of
-milliseconds | | LoRA Occupancy | Tens of MB to hundreds of MB. | | Device
-Support | NVIDIA GPU 3090 RTX/4090 RTX/A100/A800/A10 etc. (Compatibility with
-Ascend in progress) | ### Acceleration for State-of-the-art models OneDiff
-supports the acceleration for SOTA models. * stable: release for public usage,
-and has long-term support; * beta: release for professional usage, and has
-long-term support; * alpha: early release for expert usage, and should be
-careful to use; | AIGC Type | Models | HF diffusers | | ComfyUI | | SD web UI |
-| | --------- | --------------------------- | ------------ | ---------- | -----
----- | ---------- | --------- | ---------- | | | | Community | Enterprise |
-Community | Enterprise | Community | Enterprise | | Image | SD 1.5 | stable |
-stable | stable | stable | stable | stable | | | SD 2.1 | stable | stable |
-stable | stable | stable | stable | | | SDXL | stable | stable | stable |
-stable | stable | stable | | | LoRA | stable | | stable | | stable | | | |
-ControlNet | stable | | stable | | | | | | SDXL Turbo | stable | | stable | | |
-| | | LCM | stable | | stable | | | | | | SDXL DeepCache | alpha | alpha |
-alpha | alpha | | | | | InstantID | beta | | beta | | | | | Video | SVD(stable
-Video Diffusion) | stable | stable | stable | stable | | | | | SVD DeepCache |
-alpha | alpha | alpha | alpha | | | **Note: Enterprise Edition contains all the
-functionality in Community Edition.** ### Acceleration for production
-environment #### PyTorch Module compilation - [compilation with
+use OneDiff on Windows, please use it under WSL. - [The guide to install
+OneDiff in WSL2](https://github.com/siliconflow/onediff/wiki/Run-OneDiff-on-
+Windows-by-WSL2). - NVIDIA GPUs - [Compatibility with Nvidia GPUs](https://
+github.com/siliconflow/onediff/wiki/Compatibility-with-Nvidia-GPUs). --- The
+Full Introduction of OneDiff: - [About OneDiff](#about-onediff) -
+[Architecture](#architecture) - [State-of-the-art performance](#state-of-the-
+art-performance) - [Features](#features) - [Acceleration for State-of-the-art
+models](#acceleration-for-state-of-the-art-models) - [Acceleration for
+production environment](#acceleration-for-production-environment) - [OneDiff
+Quality Evalution](#onediff-quality-evaluation) - [OneDiff Enterprise Edition]
+(#onediff-enterprise-edition) - [Installation](#installation) - [Release]
+(#release) ## About OneDiff ### Architecture OneDiff interfaces with various
+front-end sd frameworks upward, and uses a custom virtual machine mixed with
+PyTorch as the inference engine downward. [imgs/onediff_arch.png]### State-of-
+the-art performance #### SDXL E2E time - Model stabilityai/stable-diffusion-xl-
+base-1.0; - Image size 1024*1024, batch size 1, steps 30; - NVIDIA A100 80G
+SXM4; [imgs/0_12_sdxl.png]#### SVD E2E time - Model stabilityai/stable-video-
+diffusion-img2vid-xt; - Image size 576*1024, batch size 1, steps 25, decoder
+chunk size 5; - NVIDIA A100 80G SXM4; [imgs/0_12_svd.png]Note that we haven't
+got the way to run SVD with TensorRT on Feb 29 2024. ### Features | Main
+Function | Details | |----------------|----------------------------| |
+Compiling Time | About 1 minute (SDXL) | | Deployment Methods | Plug and Play |
+| Dynamic Image Size Support | Support with no overhead | | Model Support |
+SD1.5~2.1, SDXL, SDXL Turbo, etc. | | Algorithm Support | SD standard workflow,
+LoRA, ControlNet, SVD, InstantID, SDXL Lightning, etc. | | SD Framework Support
+| ComfyUI, Diffusers, SD-webui | | Save & Load Accelerated Models | Yes | |
+Time of LoRA Switching | Hundreds of milliseconds | | LoRA Occupancy | Tens of
+MB to hundreds of MB. | | Device Support | NVIDIA GPU 3090 RTX/4090 RTX/A100/
+A800/A10 etc. (Compatibility with Ascend in progress) | ### Acceleration for
+State-of-the-art models OneDiff supports the acceleration for SOTA models. *
+stable: release for public usage, and has long-term support; * beta: release
+for professional usage, and has long-term support; * alpha: early release for
+expert usage, and should be careful to use; | AIGC Type | Models | HF diffusers
+| | ComfyUI | | SD web UI | | | --------- | --------------------------- | -----
+------- | ---------- | --------- | ---------- | --------- | ---------- | | | |
+Community | Enterprise | Community | Enterprise | Community | Enterprise | |
+Image | SD 1.5 | stable | stable | stable | stable | stable | stable | | | SD
+2.1 | stable | stable | stable | stable | stable | stable | | | SDXL | stable |
+stable | stable | stable | stable | stable | | | LoRA | stable | | stable | |
+stable | | | | ControlNet | stable | | stable | | | | | | SDXL Turbo | stable |
+| stable | | | | | | LCM | stable | | stable | | | | | | SDXL DeepCache | alpha
+| alpha | alpha | alpha | | | | | InstantID | beta | | beta | | | | | Video |
+SVD(stable Video Diffusion) | stable | stable | stable | stable | | | | | SVD
+DeepCache | alpha | alpha | alpha | alpha | | | **Note: Enterprise Edition
+contains all the functionality in Community Edition.** ### Acceleration for
+production environment #### PyTorch Module compilation - [compilation with
 oneflow_compile](https://github.com/siliconflow/onediff/blob/main/
 onediff_diffusers_extensions/examples/text_to_image_sdxl.py) #### Avoid
 compilation time for new input shape - [Support Multi-resolution input](https:/
 /github.com/siliconflow/onediff/blob/main/onediff_diffusers_extensions/
 examples/text_to_image_sdxl.py) #### Avoid compilation time for online serving
 Compile and save the compiled result offline, then load it online for serving -
 [Save and Load the compiled graph](https://github.com/siliconflow/onediff/blob/
```

### Comparing `onediff-1.0.0.dev202404300125/setup.py` & `onediff-1.0.0.dev202405010129/setup.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_diffusers/__init__.py` & `onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py` & `onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_diffusers/attention_processor_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_diffusers/resnet_oflow.py` & `onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_diffusers/resnet_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py` & `onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_diffusers/spatio_temporal_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py` & `onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_diffusers/transformer_2d_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py` & `onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_diffusers/unet_2d_blocks_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py` & `onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_diffusers/unet_2d_condition_oflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py` & `onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_diffusers_enterprise_lite/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/infer_compiler_registry/register_onediff_quant/__init__.py` & `onediff-1.0.0.dev202405010129/src/infer_compiler_registry/register_onediff_quant/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/__init__.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/backends/oneflow.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/backends/oneflow.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/backends/registry.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/backends/registry.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/import_tools/dyn_mock_mod.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/import_tools/format_utils.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/import_tools/format_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/import_tools/import_module_utils.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/import_tools/import_module_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/import_tools/importer.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/import_tools/importer.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/oneflow/config.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/oneflow/config.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/oneflow/deployable_module.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/oneflow/deployable_module.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/oneflow/dual_module.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/oneflow/dual_module.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/oneflow/graph.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/oneflow/graph.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/oneflow/utils.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/oneflow/utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/transform/builtin_transform.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/transform/builtin_transform.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/transform/custom_transform.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/transform/custom_transform.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/transform/manager.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/transform/manager.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/transform/patch_for_comfy.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/transform/patch_for_comfy.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/args_tree_util.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/args_tree_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/cost_util.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/cost_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/env_var.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/env_var.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/graph_management_utils.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/graph_management_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/log_utils.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/model_inplace_assign.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/model_inplace_assign.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/module_operations.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/module_operations.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/oneflow_exec_mode.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/oneflow_exec_mode.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/online_quantization_utils.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/online_quantization_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/options.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/options.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/param_utils.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/param_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/patch_for_compiler.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/patch_for_compiler.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/patch_for_diffusers.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/patch_for_diffusers.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/utils/version_util.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/utils/version_util.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/with_fx_graph.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/with_fx_graph.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/infer_compiler/with_fx_interpreter.py` & `onediff-1.0.0.dev202405010129/src/onediff/infer_compiler/with_fx_interpreter.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/optimization/attention_processor.py` & `onediff-1.0.0.dev202405010129/src/onediff/optimization/attention_processor.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/optimization/quant_optimizer.py` & `onediff-1.0.0.dev202405010129/src/onediff/optimization/quant_optimizer.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/optimization/rewrite_self_attention.py` & `onediff-1.0.0.dev202405010129/src/onediff/optimization/rewrite_self_attention.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/quantization/load_quantized_model.py` & `onediff-1.0.0.dev202405010129/src/onediff/quantization/load_quantized_model.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/quantization/quant_pipeline_test.py` & `onediff-1.0.0.dev202405010129/src/onediff/quantization/quant_pipeline_test.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/quantization/quantize_pipeline.py` & `onediff-1.0.0.dev202405010129/src/onediff/quantization/quantize_pipeline.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff/quantization/quantize_utils.py` & `onediff-1.0.0.dev202405010129/src/onediff/quantization/quantize_utils.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/src/onediff.egg-info/PKG-INFO` & `onediff-1.0.0.dev202405010129/src/onediff.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onediff
-Version: 1.0.0.dev202404300125
+Version: 1.0.0.dev202405010129
 Summary: an out-of-the-box acceleration library for diffusion models
 Home-page: https://github.com/siliconflow/onediff
 Author: OneDiff contributors
 Author-email: caishenghang@oneflow.org
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -71,14 +71,16 @@
 - [Create an issue](https://github.com/siliconflow/onediff/issues)
 - Chat in Discord: [![](https://dcbadge.vercel.app/api/server/RKJTjZMcPQ?style=plastic)](https://discord.gg/RKJTjZMcPQ)
 - Email for Enterprise Edition or other business inquiries: contact@siliconflow.com
 
 ## OS and GPU Compatibility
 - Linux
   - If you want to use OneDiff on Windows, please use it under WSL.
+  - [The guide to install OneDiff in WSL2](https://github.com/siliconflow/onediff/wiki/Run-OneDiff-on-Windows-by-WSL2).
+
 - NVIDIA GPUs
   - [Compatibility with Nvidia GPUs](https://github.com/siliconflow/onediff/wiki/Compatibility-with-Nvidia-GPUs).
 
 ---
 The Full Introduction of OneDiff:
 <!-- toc -->
 - [About OneDiff](#about-onediff)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202404300125 Summary: an
+Metadata-Version: 2.1 Name: onediff Version: 1.0.0.dev202405010129 Summary: an
 out-of-the-box acceleration library for diffusion models Home-page: https://
 github.com/siliconflow/onediff Author: OneDiff contributors Author-email:
 caishenghang@oneflow.org License: Apache Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
@@ -45,59 +45,60 @@
 comments/18lz2ir/accelerating_sdxl_3x_faster_with_deepcache_and/) ## Community
 and Support [Here is the introduction of OneDiff Community.](https://
 github.com/siliconflow/onediff/wiki#onediff-community) - [Create an issue]
 (https://github.com/siliconflow/onediff/issues) - Chat in Discord: [![](https:/
 /dcbadge.vercel.app/api/server/RKJTjZMcPQ?style=plastic)](https://discord.gg/
 RKJTjZMcPQ) - Email for Enterprise Edition or other business inquiries:
 contact@siliconflow.com ## OS and GPU Compatibility - Linux - If you want to
-use OneDiff on Windows, please use it under WSL. - NVIDIA GPUs - [Compatibility
-with Nvidia GPUs](https://github.com/siliconflow/onediff/wiki/Compatibility-
-with-Nvidia-GPUs). --- The Full Introduction of OneDiff: - [About OneDiff]
-(#about-onediff) - [Architecture](#architecture) - [State-of-the-art
-performance](#state-of-the-art-performance) - [Features](#features) -
-[Acceleration for State-of-the-art models](#acceleration-for-state-of-the-art-
-models) - [Acceleration for production environment](#acceleration-for-
-production-environment) - [OneDiff Quality Evalution](#onediff-quality-
-evaluation) - [OneDiff Enterprise Edition](#onediff-enterprise-edition) -
-[Installation](#installation) - [Release](#release) ## About OneDiff ###
-Architecture OneDiff interfaces with various front-end sd frameworks upward,
-and uses a custom virtual machine mixed with PyTorch as the inference engine
-downward. [imgs/onediff_arch.png]### State-of-the-art performance #### SDXL E2E
-time - Model stabilityai/stable-diffusion-xl-base-1.0; - Image size 1024*1024,
-batch size 1, steps 30; - NVIDIA A100 80G SXM4; [imgs/0_12_sdxl.png]#### SVD
-E2E time - Model stabilityai/stable-video-diffusion-img2vid-xt; - Image size
-576*1024, batch size 1, steps 25, decoder chunk size 5; - NVIDIA A100 80G SXM4;
-[imgs/0_12_svd.png]Note that we haven't got the way to run SVD with TensorRT on
-Feb 29 2024. ### Features | Main Function | Details | |----------------|-------
----------------------| | Compiling Time | About 1 minute (SDXL) | | Deployment
-Methods | Plug and Play | | Dynamic Image Size Support | Support with no
-overhead | | Model Support | SD1.5~2.1, SDXL, SDXL Turbo, etc. | | Algorithm
-Support | SD standard workflow, LoRA, ControlNet, SVD, InstantID, SDXL
-Lightning, etc. | | SD Framework Support | ComfyUI, Diffusers, SD-webui | |
-Save & Load Accelerated Models | Yes | | Time of LoRA Switching | Hundreds of
-milliseconds | | LoRA Occupancy | Tens of MB to hundreds of MB. | | Device
-Support | NVIDIA GPU 3090 RTX/4090 RTX/A100/A800/A10 etc. (Compatibility with
-Ascend in progress) | ### Acceleration for State-of-the-art models OneDiff
-supports the acceleration for SOTA models. * stable: release for public usage,
-and has long-term support; * beta: release for professional usage, and has
-long-term support; * alpha: early release for expert usage, and should be
-careful to use; | AIGC Type | Models | HF diffusers | | ComfyUI | | SD web UI |
-| | --------- | --------------------------- | ------------ | ---------- | -----
----- | ---------- | --------- | ---------- | | | | Community | Enterprise |
-Community | Enterprise | Community | Enterprise | | Image | SD 1.5 | stable |
-stable | stable | stable | stable | stable | | | SD 2.1 | stable | stable |
-stable | stable | stable | stable | | | SDXL | stable | stable | stable |
-stable | stable | stable | | | LoRA | stable | | stable | | stable | | | |
-ControlNet | stable | | stable | | | | | | SDXL Turbo | stable | | stable | | |
-| | | LCM | stable | | stable | | | | | | SDXL DeepCache | alpha | alpha |
-alpha | alpha | | | | | InstantID | beta | | beta | | | | | Video | SVD(stable
-Video Diffusion) | stable | stable | stable | stable | | | | | SVD DeepCache |
-alpha | alpha | alpha | alpha | | | **Note: Enterprise Edition contains all the
-functionality in Community Edition.** ### Acceleration for production
-environment #### PyTorch Module compilation - [compilation with
+use OneDiff on Windows, please use it under WSL. - [The guide to install
+OneDiff in WSL2](https://github.com/siliconflow/onediff/wiki/Run-OneDiff-on-
+Windows-by-WSL2). - NVIDIA GPUs - [Compatibility with Nvidia GPUs](https://
+github.com/siliconflow/onediff/wiki/Compatibility-with-Nvidia-GPUs). --- The
+Full Introduction of OneDiff: - [About OneDiff](#about-onediff) -
+[Architecture](#architecture) - [State-of-the-art performance](#state-of-the-
+art-performance) - [Features](#features) - [Acceleration for State-of-the-art
+models](#acceleration-for-state-of-the-art-models) - [Acceleration for
+production environment](#acceleration-for-production-environment) - [OneDiff
+Quality Evalution](#onediff-quality-evaluation) - [OneDiff Enterprise Edition]
+(#onediff-enterprise-edition) - [Installation](#installation) - [Release]
+(#release) ## About OneDiff ### Architecture OneDiff interfaces with various
+front-end sd frameworks upward, and uses a custom virtual machine mixed with
+PyTorch as the inference engine downward. [imgs/onediff_arch.png]### State-of-
+the-art performance #### SDXL E2E time - Model stabilityai/stable-diffusion-xl-
+base-1.0; - Image size 1024*1024, batch size 1, steps 30; - NVIDIA A100 80G
+SXM4; [imgs/0_12_sdxl.png]#### SVD E2E time - Model stabilityai/stable-video-
+diffusion-img2vid-xt; - Image size 576*1024, batch size 1, steps 25, decoder
+chunk size 5; - NVIDIA A100 80G SXM4; [imgs/0_12_svd.png]Note that we haven't
+got the way to run SVD with TensorRT on Feb 29 2024. ### Features | Main
+Function | Details | |----------------|----------------------------| |
+Compiling Time | About 1 minute (SDXL) | | Deployment Methods | Plug and Play |
+| Dynamic Image Size Support | Support with no overhead | | Model Support |
+SD1.5~2.1, SDXL, SDXL Turbo, etc. | | Algorithm Support | SD standard workflow,
+LoRA, ControlNet, SVD, InstantID, SDXL Lightning, etc. | | SD Framework Support
+| ComfyUI, Diffusers, SD-webui | | Save & Load Accelerated Models | Yes | |
+Time of LoRA Switching | Hundreds of milliseconds | | LoRA Occupancy | Tens of
+MB to hundreds of MB. | | Device Support | NVIDIA GPU 3090 RTX/4090 RTX/A100/
+A800/A10 etc. (Compatibility with Ascend in progress) | ### Acceleration for
+State-of-the-art models OneDiff supports the acceleration for SOTA models. *
+stable: release for public usage, and has long-term support; * beta: release
+for professional usage, and has long-term support; * alpha: early release for
+expert usage, and should be careful to use; | AIGC Type | Models | HF diffusers
+| | ComfyUI | | SD web UI | | | --------- | --------------------------- | -----
+------- | ---------- | --------- | ---------- | --------- | ---------- | | | |
+Community | Enterprise | Community | Enterprise | Community | Enterprise | |
+Image | SD 1.5 | stable | stable | stable | stable | stable | stable | | | SD
+2.1 | stable | stable | stable | stable | stable | stable | | | SDXL | stable |
+stable | stable | stable | stable | stable | | | LoRA | stable | | stable | |
+stable | | | | ControlNet | stable | | stable | | | | | | SDXL Turbo | stable |
+| stable | | | | | | LCM | stable | | stable | | | | | | SDXL DeepCache | alpha
+| alpha | alpha | alpha | | | | | InstantID | beta | | beta | | | | | Video |
+SVD(stable Video Diffusion) | stable | stable | stable | stable | | | | | SVD
+DeepCache | alpha | alpha | alpha | alpha | | | **Note: Enterprise Edition
+contains all the functionality in Community Edition.** ### Acceleration for
+production environment #### PyTorch Module compilation - [compilation with
 oneflow_compile](https://github.com/siliconflow/onediff/blob/main/
 onediff_diffusers_extensions/examples/text_to_image_sdxl.py) #### Avoid
 compilation time for new input shape - [Support Multi-resolution input](https:/
 /github.com/siliconflow/onediff/blob/main/onediff_diffusers_extensions/
 examples/text_to_image_sdxl.py) #### Avoid compilation time for online serving
 Compile and save the compiled result offline, then load it online for serving -
 [Save and Load the compiled graph](https://github.com/siliconflow/onediff/blob/
```

### Comparing `onediff-1.0.0.dev202404300125/src/onediff.egg-info/SOURCES.txt` & `onediff-1.0.0.dev202405010129/src/onediff.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/tests/test_dual_module_list.py` & `onediff-1.0.0.dev202405010129/tests/test_dual_module_list.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/tests/test_pipelines_oneflow_img2img.py` & `onediff-1.0.0.dev202405010129/tests/test_pipelines_oneflow_img2img.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/tests/test_quantitative_quality.py` & `onediff-1.0.0.dev202405010129/tests/test_quantitative_quality.py`

 * *Files identical despite different names*

### Comparing `onediff-1.0.0.dev202404300125/tests/test_quantize_custom_model.py` & `onediff-1.0.0.dev202405010129/tests/test_quantize_custom_model.py`

 * *Files identical despite different names*

