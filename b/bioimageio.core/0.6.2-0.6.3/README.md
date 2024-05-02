# Comparing `tmp/bioimageio.core-0.6.2.tar.gz` & `tmp/bioimageio.core-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioimageio.core-0.6.2.tar", last modified: Tue Apr 30 23:23:18 2024, max compression
+gzip compressed data, was "bioimageio.core-0.6.3.tar", last modified: Thu May  2 13:04:05 2024, max compression
```

## Comparing `bioimageio.core-0.6.2.tar` & `bioimageio.core-0.6.3.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.942637 bioimageio.core-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-04-30 23:23:18.942637 bioimageio.core-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-30 23:23:17.000000 bioimageio.core-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.930637 bioimageio.core-0.6.2/bioimageio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.938637 bioimageio.core-0.6.2/bioimageio/core/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 23:23:17.000000 bioimageio.core-0.6.2/bioimageio/core/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/_magic_tensor_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/_op_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/_prediction_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/_resource_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/axis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-30 23:23:17.000000 bioimageio.core-0.6.2/bioimageio/core/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/block_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    12279 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/digest_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.938637 bioimageio.core-0.6.2/bioimageio/core/model_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/model_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/model_adapters/_keras_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/model_adapters/_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/model_adapters/_onnx_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/model_adapters/_pytorch_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/model_adapters/_tensorflow_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/model_adapters/_torchscript_model_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)    21626 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/proc_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/proc_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10704 2024-04-30 23:23:17.000000 bioimageio.core-0.6.2/bioimageio/core/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    20495 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/stat_calculators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/stat_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)    16351 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.938637 bioimageio.core-0.6.2/bioimageio/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/utils/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.938637 bioimageio.core-0.6.2/bioimageio/core/weight_converter/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/weight_converter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.938637 bioimageio.core-0.6.2/bioimageio/core/weight_converter/keras/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/weight_converter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/weight_converter/keras/_tensorflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.938637 bioimageio.core-0.6.2/bioimageio/core/weight_converter/torch/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/weight_converter/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/weight_converter/torch/_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/weight_converter/torch/_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/bioimageio/core/weight_converter/torch/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.934637 bioimageio.core-0.6.2/bioimageio.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-04-30 23:23:18.000000 bioimageio.core-0.6.2/bioimageio.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-30 23:23:18.000000 bioimageio.core-0.6.2/bioimageio.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 23:23:18.000000 bioimageio.core-0.6.2/bioimageio.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 23:23:18.000000 bioimageio.core-0.6.2/bioimageio.core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-30 23:23:18.000000 bioimageio.core-0.6.2/bioimageio.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-30 23:23:18.000000 bioimageio.core-0.6.2/bioimageio.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.938637 bioimageio.core-0.6.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/scripts/setup_dev_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/scripts/show_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 23:23:18.942637 bioimageio.core-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.942637 bioimageio.core-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_any_model_fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_bioimageio_spec_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_digest_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_prediction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_prediction_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_prediction_pipeline_device_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    12513 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_proc_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_resource_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_stat_calculators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_stat_measures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/test_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.942637 bioimageio.core-0.6.2/tests/weight_converter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.942637 bioimageio.core-0.6.2/tests/weight_converter/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/weight_converter/keras/test_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/weight_converter/test_add_weights.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 23:23:18.942637 bioimageio.core-0.6.2/tests/weight_converter/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/weight_converter/torch/test_onnx.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-30 23:22:48.000000 bioimageio.core-0.6.2/tests/weight_converter/torch/test_torchscript.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.119979 bioimageio.core-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-05-02 13:04:05.119979 bioimageio.core-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-02 13:04:02.000000 bioimageio.core-0.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.107979 bioimageio.core-0.6.3/bioimageio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.111980 bioimageio.core-0.6.3/bioimageio/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 13:04:02.000000 bioimageio.core-0.6.3/bioimageio/core/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/_magic_tensor_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/_op_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11879 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/_prediction_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14845 2024-05-02 13:04:02.000000 bioimageio.core-0.6.3/bioimageio/core/_resource_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/axis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12811 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/block_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12279 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/digest_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.115980 bioimageio.core-0.6.3/bioimageio/core/model_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/model_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/model_adapters/_keras_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/model_adapters/_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/model_adapters/_onnx_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/model_adapters/_pytorch_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10284 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/model_adapters/_tensorflow_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/model_adapters/_torchscript_model_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21691 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/proc_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/proc_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10704 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20495 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/stat_calculators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/stat_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16351 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.115980 bioimageio.core-0.6.3/bioimageio/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/utils/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.115980 bioimageio.core-0.6.3/bioimageio/core/weight_converter/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/weight_converter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.115980 bioimageio.core-0.6.3/bioimageio/core/weight_converter/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/weight_converter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/weight_converter/keras/_tensorflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.115980 bioimageio.core-0.6.3/bioimageio/core/weight_converter/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/weight_converter/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/weight_converter/torch/_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/weight_converter/torch/_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/bioimageio/core/weight_converter/torch/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.111980 bioimageio.core-0.6.3/bioimageio.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-05-02 13:04:04.000000 bioimageio.core-0.6.3/bioimageio.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-02 13:04:05.000000 bioimageio.core-0.6.3/bioimageio.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:04:04.000000 bioimageio.core-0.6.3/bioimageio.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 13:04:04.000000 bioimageio.core-0.6.3/bioimageio.core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-02 13:04:04.000000 bioimageio.core-0.6.3/bioimageio.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-02 13:04:04.000000 bioimageio.core-0.6.3/bioimageio.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.115980 bioimageio.core-0.6.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/scripts/setup_dev_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/scripts/show_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:04:05.119979 bioimageio.core-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.115980 bioimageio.core-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_any_model_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_bioimageio_spec_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_digest_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_prediction_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_prediction_pipeline_device_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12513 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_proc_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_resource_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_stat_calculators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_stat_measures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/test_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.119979 bioimageio.core-0.6.3/tests/weight_converter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.119979 bioimageio.core-0.6.3/tests/weight_converter/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/weight_converter/keras/test_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/weight_converter/test_add_weights.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:04:05.119979 bioimageio.core-0.6.3/tests/weight_converter/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/weight_converter/torch/test_onnx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-02 13:03:28.000000 bioimageio.core-0.6.3/tests/weight_converter/torch/test_torchscript.py
```

### Comparing `bioimageio.core-0.6.2/LICENSE` & `bioimageio.core-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/PKG-INFO` & `bioimageio.core-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio.core
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python functionality for the bioimage model zoo
 Home-page: https://github.com/bioimage-io/core-bioimage-io-python
 Author: Bioimage Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/core-bioimage-io-python/issues
 Project-URL: Source, https://github.com/bioimage-io/core-bioimage-io-python
 Description: # core-bioimage-io-python
@@ -129,14 +129,19 @@
         
         ## Model Specification
         
         The model specification and its validation tools can be found at <https://github.com/bioimage-io/spec-bioimage-io>.
         
         ## Changelog
         
+        ### 0.6.3
+        
+        * Fix [#386](https://github.com/bioimage-io/core-bioimage-io-python/issues/386)
+        * (in model inference testing) stop assuming model inputs are tileable
+        
         ### 0.6.2
         
         * Fix [#384](https://github.com/bioimage-io/core-bioimage-io-python/issues/384)
         
         ### 0.6.1
         
         * Fix [#378](https://github.com/bioimage-io/core-bioimage-io-python/pull/378) (with [#379](https://github.com/bioimage-io/core-bioimage-io-python/pull/379))*
```

### Comparing `bioimageio.core-0.6.2/README.md` & `bioimageio.core-0.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,19 @@
 
 ## Model Specification
 
 The model specification and its validation tools can be found at <https://github.com/bioimage-io/spec-bioimage-io>.
 
 ## Changelog
 
+### 0.6.3
+
+* Fix [#386](https://github.com/bioimage-io/core-bioimage-io-python/issues/386)
+* (in model inference testing) stop assuming model inputs are tileable
+
 ### 0.6.2
 
 * Fix [#384](https://github.com/bioimage-io/core-bioimage-io-python/issues/384)
 
 ### 0.6.1
 
 * Fix [#378](https://github.com/bioimage-io/core-bioimage-io-python/pull/378) (with [#379](https://github.com/bioimage-io/core-bioimage-io-python/pull/379))*
```

### Comparing `bioimageio.core-0.6.2/bioimageio/core/__init__.py` & `bioimageio.core-0.6.3/bioimageio/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/_magic_tensor_ops.py` & `bioimageio.core-0.6.3/bioimageio/core/_magic_tensor_ops.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/_op_base.py` & `bioimageio.core-0.6.3/bioimageio/core/_op_base.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/_prediction_pipeline.py` & `bioimageio.core-0.6.3/bioimageio/core/_prediction_pipeline.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/_resource_tests.py` & `bioimageio.core-0.6.3/bioimageio/core/_resource_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,15 @@
         test_inputs = get_test_inputs(model)
 
         with create_prediction_pipeline(
             bioimageio_model=model, devices=devices, weight_format=weight_format
         ) as prediction_pipeline:
             for n, batch_size, inputs, exptected_output_shape in generate_test_cases():
                 error: Optional[str] = None
-                result = prediction_pipeline.predict_sample_with_blocking(inputs)
+                result = prediction_pipeline.predict_sample_without_blocking(inputs)
                 if len(result.members) != len(exptected_output_shape):
                     error = (
                         f"Expected {len(exptected_output_shape)} outputs,"
                         + f" but got {len(result.members)}"
                     )
 
                 else:
```

### Comparing `bioimageio.core-0.6.2/bioimageio/core/axis.py` & `bioimageio.core-0.6.3/bioimageio/core/axis.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/block.py` & `bioimageio.core-0.6.3/bioimageio/core/block.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/block_meta.py` & `bioimageio.core-0.6.3/bioimageio/core/block_meta.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/commands.py` & `bioimageio.core-0.6.3/bioimageio/core/commands.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/common.py` & `bioimageio.core-0.6.3/bioimageio/core/common.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/digest_spec.py` & `bioimageio.core-0.6.3/bioimageio/core/digest_spec.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/io.py` & `bioimageio.core-0.6.3/bioimageio/core/io.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/model_adapters/_keras_model_adapter.py` & `bioimageio.core-0.6.3/bioimageio/core/model_adapters/_keras_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/model_adapters/_model_adapter.py` & `bioimageio.core-0.6.3/bioimageio/core/model_adapters/_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/model_adapters/_onnx_model_adapter.py` & `bioimageio.core-0.6.3/bioimageio/core/model_adapters/_onnx_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/model_adapters/_pytorch_model_adapter.py` & `bioimageio.core-0.6.3/bioimageio/core/model_adapters/_pytorch_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/model_adapters/_tensorflow_model_adapter.py` & `bioimageio.core-0.6.3/bioimageio/core/model_adapters/_tensorflow_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/model_adapters/_torchscript_model_adapter.py` & `bioimageio.core-0.6.3/bioimageio/core/model_adapters/_torchscript_model_adapter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/proc_ops.py` & `bioimageio.core-0.6.3/bioimageio/core/proc_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,14 +69,17 @@
     def required_measures(self) -> Collection[Measure]:
         return set()
 
     @abstractmethod
     def get_output_shape(self, input_shape: PerAxis[int]) -> PerAxis[int]: ...
 
     def __call__(self, sample: Union[Sample, SampleBlock]) -> None:
+        if self.input not in sample.members:
+            return
+
         input_tensor = sample.members[self.input]
         output_tensor = self._apply(input_tensor, sample.stat)
 
         if self.output in sample.members:
             assert (
                 sample.members[self.output].tagged_shape == output_tensor.tagged_shape
             )
```

### Comparing `bioimageio.core-0.6.2/bioimageio/core/proc_setup.py` & `bioimageio.core-0.6.3/bioimageio/core/proc_setup.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/sample.py` & `bioimageio.core-0.6.3/bioimageio/core/sample.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/stat_calculators.py` & `bioimageio.core-0.6.3/bioimageio/core/stat_calculators.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/stat_measures.py` & `bioimageio.core-0.6.3/bioimageio/core/stat_measures.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/tensor.py` & `bioimageio.core-0.6.3/bioimageio/core/tensor.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/utils/testing.py` & `bioimageio.core-0.6.3/bioimageio/core/utils/testing.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/weight_converter/keras/_tensorflow.py` & `bioimageio.core-0.6.3/bioimageio/core/weight_converter/keras/_tensorflow.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/weight_converter/torch/_onnx.py` & `bioimageio.core-0.6.3/bioimageio/core/weight_converter/torch/_onnx.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/weight_converter/torch/_torchscript.py` & `bioimageio.core-0.6.3/bioimageio/core/weight_converter/torch/_torchscript.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio/core/weight_converter/torch/_utils.py` & `bioimageio.core-0.6.3/bioimageio/core/weight_converter/torch/_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/bioimageio.core.egg-info/PKG-INFO` & `bioimageio.core-0.6.3/bioimageio.core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio.core
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python functionality for the bioimage model zoo
 Home-page: https://github.com/bioimage-io/core-bioimage-io-python
 Author: Bioimage Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/core-bioimage-io-python/issues
 Project-URL: Source, https://github.com/bioimage-io/core-bioimage-io-python
 Description: # core-bioimage-io-python
@@ -129,14 +129,19 @@
         
         ## Model Specification
         
         The model specification and its validation tools can be found at <https://github.com/bioimage-io/spec-bioimage-io>.
         
         ## Changelog
         
+        ### 0.6.3
+        
+        * Fix [#386](https://github.com/bioimage-io/core-bioimage-io-python/issues/386)
+        * (in model inference testing) stop assuming model inputs are tileable
+        
         ### 0.6.2
         
         * Fix [#384](https://github.com/bioimage-io/core-bioimage-io-python/issues/384)
         
         ### 0.6.1
         
         * Fix [#378](https://github.com/bioimage-io/core-bioimage-io-python/pull/378) (with [#379](https://github.com/bioimage-io/core-bioimage-io-python/pull/379))*
```

### Comparing `bioimageio.core-0.6.2/bioimageio.core.egg-info/SOURCES.txt` & `bioimageio.core-0.6.3/bioimageio.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/pyproject.toml` & `bioimageio.core-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/scripts/setup_dev_env.py` & `bioimageio.core-0.6.3/scripts/setup_dev_env.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/scripts/show_diff.py` & `bioimageio.core-0.6.3/scripts/show_diff.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/setup.py` & `bioimageio.core-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/tests/test_bioimageio_spec_version.py` & `bioimageio.core-0.6.3/tests/test_bioimageio_spec_version.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/tests/test_cli.py` & `bioimageio.core-0.6.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/tests/test_digest_spec.py` & `bioimageio.core-0.6.3/tests/test_digest_spec.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/tests/test_prediction.py` & `bioimageio.core-0.6.3/tests/test_prediction.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/tests/test_prediction_pipeline.py` & `bioimageio.core-0.6.3/tests/test_prediction_pipeline.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/tests/test_prediction_pipeline_device_management.py` & `bioimageio.core-0.6.3/tests/test_prediction_pipeline_device_management.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/tests/test_proc_ops.py` & `bioimageio.core-0.6.3/tests/test_proc_ops.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/tests/test_resource_tests.py` & `bioimageio.core-0.6.3/tests/test_resource_tests.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/tests/test_stat_calculators.py` & `bioimageio.core-0.6.3/tests/test_stat_calculators.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/tests/test_stat_measures.py` & `bioimageio.core-0.6.3/tests/test_stat_measures.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/tests/test_tensor.py` & `bioimageio.core-0.6.3/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/tests/weight_converter/keras/test_tensorflow.py` & `bioimageio.core-0.6.3/tests/weight_converter/keras/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/tests/weight_converter/test_add_weights.py` & `bioimageio.core-0.6.3/tests/weight_converter/test_add_weights.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/tests/weight_converter/torch/test_onnx.py` & `bioimageio.core-0.6.3/tests/weight_converter/torch/test_onnx.py`

 * *Files identical despite different names*

### Comparing `bioimageio.core-0.6.2/tests/weight_converter/torch/test_torchscript.py` & `bioimageio.core-0.6.3/tests/weight_converter/torch/test_torchscript.py`

 * *Files identical despite different names*

