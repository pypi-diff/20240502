# Comparing `tmp/token_trace-0.3.0.tar.gz` & `tmp/token_trace-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "token_trace-0.3.0.tar", last modified: Thu May  2 17:13:00 2024, max compression
+gzip compressed data, was "token_trace-0.3.1.tar", last modified: Thu May  2 17:18:53 2024, max compression
```

## Comparing `token_trace-0.3.0.tar` & `token_trace-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1068 2024-05-02 17:11:44.541795 token_trace-0.3.0/LICENSE
--rw-r--r--   0        0        0     1602 2024-05-02 17:11:44.541795 token_trace-0.3.0/README.md
--rw-r--r--   0        0        0     1994 2024-05-02 17:13:00.110909 token_trace-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-02 17:11:45.061803 token_trace-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      174 2024-05-02 17:11:45.061803 token_trace-0.3.0/tests/app/test_get_data.py
--rw-r--r--   0        0        0      733 2024-05-02 17:11:45.061803 token_trace-0.3.0/tests/circuit/test_edge_attribution.py
--rw-r--r--   0        0        0      631 2024-05-02 17:11:45.061803 token_trace-0.3.0/tests/circuit/test_node_attribution.py
--rw-r--r--   0        0        0     1698 2024-05-02 17:11:45.061803 token_trace-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0     1940 2024-05-02 17:11:45.061803 token_trace-0.3.0/tests/helpers.py
--rw-r--r--   0        0        0      940 2024-05-02 17:11:45.061803 token_trace-0.3.0/tests/test_sae_activation_cache.py
--rw-r--r--   0        0        0     5255 2024-05-02 17:11:45.061803 token_trace-0.3.0/tests/test_sae_patcher.py
--rw-r--r--   0        0        0     1073 2024-05-02 17:11:45.061803 token_trace-0.3.0/tests/test_utils.py
--rw-r--r--   0        0        0       22 2024-05-02 17:12:55.166839 token_trace-0.3.0/token_trace/__init__.py
--rw-r--r--   0        0        0       55 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/app/__init__.py
--rw-r--r--   0        0        0     2537 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/app/get_circuit.py
--rw-r--r--   0        0        0      484 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/app/precompute_circuits.py
--rw-r--r--   0        0        0     1066 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/app/process_data.py
--rw-r--r--   0        0        0    12520 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/app/run_app.py
--rw-r--r--   0        0        0      185 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/circuit/__init__.py
--rw-r--r--   0        0        0     6024 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/circuit/edge_attribution.py
--rw-r--r--   0        0        0     4449 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/circuit/node_attribution.py
--rw-r--r--   0        0        0     7237 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/circuit/sparse_feature_circuit.py
--rw-r--r--   0        0        0      296 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/constants.py
--rw-r--r--   0        0        0     2353 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/load_pretrained_model.py
--rw-r--r--   0        0        0     5796 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/print_prompt_info.py
--rw-r--r--   0        0        0     1628 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/sae_activation_cache.py
--rw-r--r--   0        0        0     4608 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/sae_patcher.py
--rw-r--r--   0        0        0      708 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/types.py
--rw-r--r--   0        0        0     2638 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/utils.py
--rw-r--r--   0        0        0     2242 1970-01-01 00:00:00.000000 token_trace-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-02 17:17:45.523490 token_trace-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1602 2024-05-02 17:17:45.523490 token_trace-0.3.1/README.md
+-rw-r--r--   0        0        0     1994 2024-05-02 17:18:53.719092 token_trace-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-02 17:17:46.043487 token_trace-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0      174 2024-05-02 17:17:46.043487 token_trace-0.3.1/tests/app/test_get_data.py
+-rw-r--r--   0        0        0      733 2024-05-02 17:17:46.043487 token_trace-0.3.1/tests/circuit/test_edge_attribution.py
+-rw-r--r--   0        0        0      631 2024-05-02 17:17:46.043487 token_trace-0.3.1/tests/circuit/test_node_attribution.py
+-rw-r--r--   0        0        0     1698 2024-05-02 17:17:46.043487 token_trace-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0     1940 2024-05-02 17:17:46.043487 token_trace-0.3.1/tests/helpers.py
+-rw-r--r--   0        0        0      940 2024-05-02 17:17:46.043487 token_trace-0.3.1/tests/test_sae_activation_cache.py
+-rw-r--r--   0        0        0     5255 2024-05-02 17:17:46.043487 token_trace-0.3.1/tests/test_sae_patcher.py
+-rw-r--r--   0        0        0     1073 2024-05-02 17:17:46.043487 token_trace-0.3.1/tests/test_utils.py
+-rw-r--r--   0        0        0       22 2024-05-02 17:18:49.095122 token_trace-0.3.1/token_trace/__init__.py
+-rw-r--r--   0        0        0       55 2024-05-02 17:17:46.043487 token_trace-0.3.1/token_trace/app/__init__.py
+-rw-r--r--   0        0        0     2537 2024-05-02 17:17:46.043487 token_trace-0.3.1/token_trace/app/get_circuit.py
+-rw-r--r--   0        0        0      484 2024-05-02 17:17:46.043487 token_trace-0.3.1/token_trace/app/precompute_circuits.py
+-rw-r--r--   0        0        0     1066 2024-05-02 17:17:46.043487 token_trace-0.3.1/token_trace/app/process_data.py
+-rw-r--r--   0        0        0    12520 2024-05-02 17:17:46.043487 token_trace-0.3.1/token_trace/app/run_app.py
+-rw-r--r--   0        0        0      185 2024-05-02 17:17:46.043487 token_trace-0.3.1/token_trace/circuit/__init__.py
+-rw-r--r--   0        0        0     6024 2024-05-02 17:17:46.043487 token_trace-0.3.1/token_trace/circuit/edge_attribution.py
+-rw-r--r--   0        0        0     4449 2024-05-02 17:17:46.043487 token_trace-0.3.1/token_trace/circuit/node_attribution.py
+-rw-r--r--   0        0        0     7237 2024-05-02 17:17:46.043487 token_trace-0.3.1/token_trace/circuit/sparse_feature_circuit.py
+-rw-r--r--   0        0        0      296 2024-05-02 17:17:46.043487 token_trace-0.3.1/token_trace/constants.py
+-rw-r--r--   0        0        0     2353 2024-05-02 17:17:46.043487 token_trace-0.3.1/token_trace/load_pretrained_model.py
+-rw-r--r--   0        0        0     5796 2024-05-02 17:17:46.043487 token_trace-0.3.1/token_trace/print_prompt_info.py
+-rw-r--r--   0        0        0     1628 2024-05-02 17:17:46.043487 token_trace-0.3.1/token_trace/sae_activation_cache.py
+-rw-r--r--   0        0        0     4608 2024-05-02 17:17:46.043487 token_trace-0.3.1/token_trace/sae_patcher.py
+-rw-r--r--   0        0        0      708 2024-05-02 17:17:46.043487 token_trace-0.3.1/token_trace/types.py
+-rw-r--r--   0        0        0     2638 2024-05-02 17:17:46.043487 token_trace-0.3.1/token_trace/utils.py
+-rw-r--r--   0        0        0     2242 1970-01-01 00:00:00.000000 token_trace-0.3.1/PKG-INFO
```

### Comparing `token_trace-0.3.0/LICENSE` & `token_trace-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/README.md` & `token_trace-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/pyproject.toml` & `token_trace-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "token-trace"
-version = "0.3.0"
+version = "0.3.1"
 description = "Transformer token flow visualizer"
 dependencies = [
     "transformers>=4.39.3",
     "transformer-lens>=1.15.0",
     "sae-lens>=0.2.0",
     "pandera>=0.18.3",
 ]
```

### Comparing `token_trace-0.3.0/tests/circuit/test_edge_attribution.py` & `token_trace-0.3.1/tests/circuit/test_edge_attribution.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/tests/circuit/test_node_attribution.py` & `token_trace-0.3.1/tests/circuit/test_node_attribution.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/tests/conftest.py` & `token_trace-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/tests/helpers.py` & `token_trace-0.3.1/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/tests/test_sae_activation_cache.py` & `token_trace-0.3.1/tests/test_sae_activation_cache.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/tests/test_sae_patcher.py` & `token_trace-0.3.1/tests/test_sae_patcher.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/tests/test_utils.py` & `token_trace-0.3.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/token_trace/app/get_circuit.py` & `token_trace-0.3.1/token_trace/app/get_circuit.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/token_trace/app/process_data.py` & `token_trace-0.3.1/token_trace/app/process_data.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/token_trace/app/run_app.py` & `token_trace-0.3.1/token_trace/app/run_app.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/token_trace/circuit/edge_attribution.py` & `token_trace-0.3.1/token_trace/circuit/edge_attribution.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/token_trace/circuit/node_attribution.py` & `token_trace-0.3.1/token_trace/circuit/node_attribution.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/token_trace/circuit/sparse_feature_circuit.py` & `token_trace-0.3.1/token_trace/circuit/sparse_feature_circuit.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/token_trace/load_pretrained_model.py` & `token_trace-0.3.1/token_trace/load_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/token_trace/print_prompt_info.py` & `token_trace-0.3.1/token_trace/print_prompt_info.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/token_trace/sae_activation_cache.py` & `token_trace-0.3.1/token_trace/sae_activation_cache.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/token_trace/sae_patcher.py` & `token_trace-0.3.1/token_trace/sae_patcher.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/token_trace/types.py` & `token_trace-0.3.1/token_trace/types.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/token_trace/utils.py` & `token_trace-0.3.1/token_trace/utils.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.3.0/PKG-INFO` & `token_trace-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: token-trace
-Version: 0.3.0
+Version: 0.3.1
 Summary: Transformer token flow visualizer
 Author-Email: "Seongho Son, Liza Karmannaya, Daniel Tan, David Chanin" <chanindav@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: transformers>=4.39.3
 Requires-Dist: transformer-lens>=1.15.0
 Requires-Dist: sae-lens>=0.2.0
```

