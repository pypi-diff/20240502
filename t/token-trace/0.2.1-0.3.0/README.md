# Comparing `tmp/token_trace-0.2.1.tar.gz` & `tmp/token_trace-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "token_trace-0.2.1.tar", last modified: Sat Apr 20 22:08:37 2024, max compression
+gzip compressed data, was "token_trace-0.3.0.tar", last modified: Thu May  2 17:13:00 2024, max compression
```

## Comparing `token_trace-0.2.1.tar` & `token_trace-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1068 2024-04-13 13:14:05.229465 token_trace-0.2.1/LICENSE
--rw-r--r--   0        0        0     1602 2024-04-19 22:14:54.225885 token_trace-0.2.1/README.md
--rw-r--r--   0        0        0     1994 2024-04-20 22:08:37.124901 token_trace-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 13:20:18.948778 token_trace-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      174 2024-04-20 20:47:20.249121 token_trace-0.2.1/tests/app/test_get_data.py
--rw-r--r--   0        0        0      733 2024-04-20 20:47:20.249121 token_trace-0.2.1/tests/circuit/test_edge_attribution.py
--rw-r--r--   0        0        0      631 2024-04-20 20:47:20.249121 token_trace-0.2.1/tests/circuit/test_node_attribution.py
--rw-r--r--   0        0        0     1698 2024-04-20 20:47:20.249121 token_trace-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0     1940 2024-04-18 00:33:32.206128 token_trace-0.2.1/tests/helpers.py
--rw-r--r--   0        0        0      940 2024-04-20 20:47:20.249121 token_trace-0.2.1/tests/test_sae_activation_cache.py
--rw-r--r--   0        0        0     5255 2024-04-20 20:47:20.249121 token_trace-0.2.1/tests/test_sae_patcher.py
--rw-r--r--   0        0        0     1073 2024-04-19 15:47:33.361295 token_trace-0.2.1/tests/test_utils.py
--rw-r--r--   0        0        0       22 2024-04-20 21:26:04.157785 token_trace-0.2.1/token_trace/__init__.py
--rw-r--r--   0        0        0       55 2024-04-19 22:20:43.704861 token_trace-0.2.1/token_trace/app/__init__.py
--rw-r--r--   0        0        0     2052 2024-04-20 21:54:12.996159 token_trace-0.2.1/token_trace/app/get_circuit.py
--rw-r--r--   0        0        0     1066 2024-04-20 20:47:20.249121 token_trace-0.2.1/token_trace/app/process_data.py
--rw-r--r--   0        0        0    12078 2024-04-20 21:37:36.207679 token_trace-0.2.1/token_trace/app/run_app.py
--rw-r--r--   0        0        0      176 2024-04-20 21:56:44.029372 token_trace-0.2.1/token_trace/circuit/__init__.py
--rw-r--r--   0        0        0     6024 2024-04-20 21:57:57.925590 token_trace-0.2.1/token_trace/circuit/edge_attribution.py
--rw-r--r--   0        0        0     4449 2024-04-20 21:57:50.421566 token_trace-0.2.1/token_trace/circuit/node_attribution.py
--rw-r--r--   0        0        0     6709 2024-04-20 21:56:23.349268 token_trace-0.2.1/token_trace/circuit/sparse_feature_circuit.py
--rw-r--r--   0        0        0      296 2024-04-20 20:47:20.249121 token_trace-0.2.1/token_trace/constants.py
--rw-r--r--   0        0        0     2353 2024-04-20 20:47:20.249121 token_trace-0.2.1/token_trace/load_pretrained_model.py
--rw-r--r--   0        0        0     5796 2024-04-18 00:33:45.182230 token_trace-0.2.1/token_trace/print_prompt_info.py
--rw-r--r--   0        0        0     1628 2024-04-20 20:47:20.249121 token_trace-0.2.1/token_trace/sae_activation_cache.py
--rw-r--r--   0        0        0     4608 2024-04-20 20:47:20.249121 token_trace-0.2.1/token_trace/sae_patcher.py
--rw-r--r--   0        0        0      708 2024-04-20 20:47:20.249121 token_trace-0.2.1/token_trace/types.py
--rw-r--r--   0        0        0     2614 2024-04-20 21:44:38.319271 token_trace-0.2.1/token_trace/utils.py
--rw-r--r--   0        0        0     2242 1970-01-01 00:00:00.000000 token_trace-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-02 17:11:44.541795 token_trace-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1602 2024-05-02 17:11:44.541795 token_trace-0.3.0/README.md
+-rw-r--r--   0        0        0     1994 2024-05-02 17:13:00.110909 token_trace-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-02 17:11:45.061803 token_trace-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      174 2024-05-02 17:11:45.061803 token_trace-0.3.0/tests/app/test_get_data.py
+-rw-r--r--   0        0        0      733 2024-05-02 17:11:45.061803 token_trace-0.3.0/tests/circuit/test_edge_attribution.py
+-rw-r--r--   0        0        0      631 2024-05-02 17:11:45.061803 token_trace-0.3.0/tests/circuit/test_node_attribution.py
+-rw-r--r--   0        0        0     1698 2024-05-02 17:11:45.061803 token_trace-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     1940 2024-05-02 17:11:45.061803 token_trace-0.3.0/tests/helpers.py
+-rw-r--r--   0        0        0      940 2024-05-02 17:11:45.061803 token_trace-0.3.0/tests/test_sae_activation_cache.py
+-rw-r--r--   0        0        0     5255 2024-05-02 17:11:45.061803 token_trace-0.3.0/tests/test_sae_patcher.py
+-rw-r--r--   0        0        0     1073 2024-05-02 17:11:45.061803 token_trace-0.3.0/tests/test_utils.py
+-rw-r--r--   0        0        0       22 2024-05-02 17:12:55.166839 token_trace-0.3.0/token_trace/__init__.py
+-rw-r--r--   0        0        0       55 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/app/__init__.py
+-rw-r--r--   0        0        0     2537 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/app/get_circuit.py
+-rw-r--r--   0        0        0      484 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/app/precompute_circuits.py
+-rw-r--r--   0        0        0     1066 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/app/process_data.py
+-rw-r--r--   0        0        0    12520 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/app/run_app.py
+-rw-r--r--   0        0        0      185 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/circuit/__init__.py
+-rw-r--r--   0        0        0     6024 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/circuit/edge_attribution.py
+-rw-r--r--   0        0        0     4449 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/circuit/node_attribution.py
+-rw-r--r--   0        0        0     7237 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/circuit/sparse_feature_circuit.py
+-rw-r--r--   0        0        0      296 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/constants.py
+-rw-r--r--   0        0        0     2353 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/load_pretrained_model.py
+-rw-r--r--   0        0        0     5796 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/print_prompt_info.py
+-rw-r--r--   0        0        0     1628 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/sae_activation_cache.py
+-rw-r--r--   0        0        0     4608 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/sae_patcher.py
+-rw-r--r--   0        0        0      708 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/types.py
+-rw-r--r--   0        0        0     2638 2024-05-02 17:11:45.061803 token_trace-0.3.0/token_trace/utils.py
+-rw-r--r--   0        0        0     2242 1970-01-01 00:00:00.000000 token_trace-0.3.0/PKG-INFO
```

### Comparing `token_trace-0.2.1/LICENSE` & `token_trace-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `token_trace-0.2.1/README.md` & `token_trace-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `token_trace-0.2.1/pyproject.toml` & `token_trace-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "token-trace"
-version = "0.2.1"
+version = "0.3.0"
 description = "Transformer token flow visualizer"
 dependencies = [
     "transformers>=4.39.3",
     "transformer-lens>=1.15.0",
     "sae-lens>=0.2.0",
     "pandera>=0.18.3",
 ]
```

### Comparing `token_trace-0.2.1/tests/circuit/test_edge_attribution.py` & `token_trace-0.3.0/tests/circuit/test_edge_attribution.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.2.1/tests/circuit/test_node_attribution.py` & `token_trace-0.3.0/tests/circuit/test_node_attribution.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.2.1/tests/conftest.py` & `token_trace-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.2.1/tests/helpers.py` & `token_trace-0.3.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.2.1/tests/test_sae_activation_cache.py` & `token_trace-0.3.0/tests/test_sae_activation_cache.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.2.1/tests/test_sae_patcher.py` & `token_trace-0.3.0/tests/test_sae_patcher.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.2.1/tests/test_utils.py` & `token_trace-0.3.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.2.1/token_trace/app/get_circuit.py` & `token_trace-0.3.0/token_trace/app/get_circuit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import pathlib
 import shutil
 from collections import deque
 from hashlib import md5
 from threading import Lock
 
 from token_trace.circuit import SparseFeatureCircuit, SparseFeatureCircuitBuilder
@@ -30,27 +31,42 @@
                 # Remove the directory and its contents
                 shutil.rmtree(oldest_path)
             else:
                 oldest_path.unlink()
         print(f"Deleted old path: {oldest_path}")
 
 
+def list_existing_circuits() -> list[str]:
+    existing_texts = []
+    savedirs = [path for path in DATA_DIR.iterdir() if path.is_dir()]
+    # get the text for each circuit
+    for savedir in savedirs:
+        try:
+            with open(savedir / "args.json") as f:
+                args = json.load(f)
+                existing_texts.append(args["text"])
+        except FileNotFoundError:
+            continue
+    return existing_texts
+
+
 def load_or_compute_circuit(
     text: str, force_rerun: bool = False
 ) -> SparseFeatureCircuit:
     """Load or compute the circuit data."""
     prefix = md5(text.encode()).hexdigest()[:16]
     save_dir = DATA_DIR / prefix
 
     if save_dir.exists() and not force_rerun:
         circuit = SparseFeatureCircuit.load(DATA_DIR / prefix)
     else:
         save_dir.mkdir(exist_ok=True, parents=True)
         builder = SparseFeatureCircuitBuilder(model_name=DEFAULT_MODEL_NAME, text=text)
         # TODO: edge attributions are still too slow to compute this here
+        builder.save_args(save_dir)
         builder.compute_sae_activation_cache().compute_node_attributions()
         circuit = builder.circuit
         circuit.save(save_dir)
         add_path_and_delete_old(save_dir)
 
     return circuit
```

### Comparing `token_trace-0.2.1/token_trace/app/process_data.py` & `token_trace-0.3.0/token_trace/app/process_data.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.2.1/token_trace/app/run_app.py` & `token_trace-0.3.0/token_trace/app/run_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import plotly.graph_objects as go
 import plotly_express as px
 import streamlit as st
 from annotated_text import annotated_text
 from pandera.typing import Series
 from plotly.subplots import make_subplots
 
-from token_trace.app.get_circuit import get_circuit
+from token_trace.app.get_circuit import get_circuit, list_existing_circuits
 from token_trace.app.process_data import process_node_data
 from token_trace.constants import (
     # DEFAULT_ANSWER,
     DEFAULT_MODEL_NAME,
     # DEFAULT_PROMPT,
     DEFAULT_REPO_ID,
     DEFAULT_TEXT,
@@ -154,15 +154,15 @@
 
     with negative:
         neg_df = df[df["ie"] < 0]
         for layer in neg_df["layer"].sort_values().unique():
             features = neg_df[neg_df["layer"] == layer]["act_idx"].values
             list_name = f"layer_{layer}_ie_negative_features"
             st.link_button(
-                label=f"ie-positive features for layer {layer}",
+                label=f"ie-negative features for layer {layer}",
                 url=get_neuronpedia_url(layer, features, list_name),
             )
 
 
 def add_section_individual_feature_attribution(df: pd.DataFrame):
     st.header("Individual Feature Attributions")
     st.write("Here, we visualize the feature attributions for each node.")
@@ -330,26 +330,36 @@
 
         subfig = go.Histogram(x=layer_df.indirect_effect, name=f"Layer {layer}")
         fig.add_trace(subfig, row=row, col=col)
 
     st.plotly_chart(fig, use_container_width=True)
 
 
-def run_app():
+def run_app(precomputed_only: bool = True):
     st.set_page_config(layout="wide")
     # Display model name
     st.header("Metadata")
     st.write(f"Model: {DEFAULT_MODEL_NAME}")
     st.write(f"SAEs: {DEFAULT_REPO_ID}")
 
+    # List existing circuits
+    existing_texts = list_existing_circuits() + ["null"]
+    st.header("View a pre-computed prompt")
+    selected_text = st.selectbox("Select a prompt", existing_texts, index=0)
+    text = selected_text
+    assert isinstance(text, str)
+
     # Get text
-    st.header("Input")
-    text = st.text_input("Text", DEFAULT_TEXT)
-    prompt, response = text.rsplit(" ", 1)
+    if not precomputed_only:
+        st.header("Or write your own prompt")
+        user_text = st.text_input("Text", DEFAULT_TEXT)
+        text = selected_text if selected_text else user_text
+
     st.divider()
+    prompt, response = text.rsplit(" ", 1)
 
     with st.expander("Prompt breakdown"):
         # Display tokenized text
         st.write("Tokenized text:")
         tokens = get_token_strs(DEFAULT_MODEL_NAME, text)
         annotated_tokens = get_token_annotations(tokens)
         annotated_text(*annotated_tokens)
```

### Comparing `token_trace-0.2.1/token_trace/circuit/edge_attribution.py` & `token_trace-0.3.0/token_trace/circuit/edge_attribution.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.2.1/token_trace/circuit/node_attribution.py` & `token_trace-0.3.0/token_trace/circuit/node_attribution.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.2.1/token_trace/circuit/sparse_feature_circuit.py` & `token_trace-0.3.0/token_trace/circuit/sparse_feature_circuit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,47 @@
+import json
 import pathlib
+from dataclasses import dataclass
 
 import pandas as pd
-from dataclasses import dataclass
 
 from token_trace.circuit.edge_attribution import (
     EdgeAttributionDataFrame,
     EdgeAttributionSchema,
     compute_edge_attribution,
-    validate_edge_attribution,
     filter_edges,
+    validate_edge_attribution,
 )
 from token_trace.circuit.node_attribution import (
     NodeAttributionDataFrame,
     NodeAttributionSchema,
     compute_node_attribution,
-    validate_node_attribution,
     filter_nodes,
     get_nodes_in_module,
+    validate_node_attribution,
 )
 from token_trace.constants import DEFAULT_MODEL_NAME, DEFAULT_TEXT
 from token_trace.load_pretrained_model import load_model, load_sae_dict
 from token_trace.sae_activation_cache import (
     SAEActivationCache,
     get_sae_activation_cache,
 )
 from token_trace.types import (
     HookedTransformer,
     MetricFunction,
     SAEDict,
 )
-from token_trace.utils import last_token_prediction_loss, get_empty_dataframe_from_pa_model
+from token_trace.utils import (
+    get_empty_dataframe_from_pa_model,
+    last_token_prediction_loss,
+)
 
 # schema for the node_df
 
+
 class SparseFeatureCircuitBuilder:
     model: HookedTransformer
     sae_dict: SAEDict
     metric_fn: MetricFunction
     # TODO: support multiple text strings.
     text: str
     sae_activation_cache: SAEActivationCache
@@ -53,20 +58,20 @@
     ):
         self.model_name = model_name
         self.text = text
         self.min_node_abs_ie = min_node_abs_ie
         self.min_edge_abs_ie = min_edge_abs_ie
         self.max_n_nodes = max_n_nodes
         self.max_n_edges = max_n_edges
-        self.node_ie_df = None 
+        self.node_ie_df = None
         self.edge_ie_df = None
 
-    @property 
+    @property
     def circuit(self):
-        """ Get the circuit at the current stage """
+        """Get the circuit at the current stage"""
         return SparseFeatureCircuit(
             node_ie_df=self.node_ie_df,
             edge_ie_df=self.edge_ie_df,
         )
 
     def compute_sae_activation_cache(self) -> "SparseFeatureCircuitBuilder":
         self.model = load_model(self.model_name)
@@ -92,15 +97,15 @@
         max_n_nodes: int | None = None,
     ) -> NodeAttributionDataFrame:
         """Get filtered nodes by total absolute indirect effect"""
         if min_node_abs_ie is not None:
             self.min_node_abs_ie = min_node_abs_ie
         if max_n_nodes is not None:
             self.max_n_nodes = max_n_nodes
-        assert self.node_ie_df is not None # keep pyright happy
+        assert self.node_ie_df is not None  # keep pyright happy
         return filter_nodes(
             self.node_ie_df,
             min_node_abs_ie=self.min_node_abs_ie,
             max_n_nodes=self.max_n_nodes,
         )
 
     def filter_nodes(
@@ -112,23 +117,23 @@
         self.node_ie_df = self.get_filtered_nodes(
             min_node_abs_ie=min_node_abs_ie,
             max_n_nodes=max_n_nodes,
         )
         return self
 
     def compute_edge_attributions(self) -> "SparseFeatureCircuitBuilder":
-        assert self.node_ie_df is not None # keep pyright happy
+        assert self.node_ie_df is not None  # keep pyright happy
         self.edge_ie_df = compute_edge_attribution(
             self.node_ie_df,
             sae_acts_clean=self.sae_activation_cache,
         )
         return self
 
     def filter_edges(self) -> "SparseFeatureCircuitBuilder":
-        assert self.edge_ie_df is not None # keep pyright happy
+        assert self.edge_ie_df is not None  # keep pyright happy
         self.edge_ie_df = filter_edges(
             self.edge_ie_df,
             min_edge_ie=self.min_edge_abs_ie,
             max_n_edges=self.max_n_edges,
         )
         return self
 
@@ -137,40 +142,53 @@
             self.compute_sae_activation_cache()
             .compute_node_attributions()
             .filter_nodes()
             .compute_edge_attributions()
             .filter_edges()
         )
 
+    def save_args(self, save_dir: pathlib.Path):
+        args = {
+            "model_name": self.model_name,
+            "text": self.text,
+            "min_node_abs_ie": self.min_node_abs_ie,
+            "max_n_nodes": self.max_n_nodes,
+            "min_edge_abs_ie": self.min_edge_abs_ie,
+            "max_n_edges": self.max_n_edges,
+        }
+        with open(save_dir / "args.json", "w") as f:
+            json.dump(args, f)
+
 
 @dataclass
 class SparseFeatureCircuit:
     """Compute a circuit consisting of SAE features"""
 
     # Represent the sub-graph
     node_ie_df: NodeAttributionDataFrame
     edge_ie_df: EdgeAttributionDataFrame
 
-    def __init__(self, 
+    def __init__(
+        self,
         node_ie_df: NodeAttributionDataFrame | None = None,
-        edge_ie_df: EdgeAttributionDataFrame | None = None             
+        edge_ie_df: EdgeAttributionDataFrame | None = None,
     ):
         if node_ie_df is None:
-            node_ie_df = get_empty_dataframe_from_pa_model(NodeAttributionSchema) # type: ignore
+            node_ie_df = get_empty_dataframe_from_pa_model(NodeAttributionSchema)  # type: ignore
         if edge_ie_df is None:
-            edge_ie_df = get_empty_dataframe_from_pa_model(EdgeAttributionSchema) # type: ignore
-        self.node_ie_df = validate_node_attribution(node_ie_df) # type: ignore
-        self.edge_ie_df = validate_edge_attribution(edge_ie_df) # type: ignore
+            edge_ie_df = get_empty_dataframe_from_pa_model(EdgeAttributionSchema)  # type: ignore
+        self.node_ie_df = validate_node_attribution(node_ie_df)  # type: ignore
+        self.edge_ie_df = validate_edge_attribution(edge_ie_df)  # type: ignore
 
     """ Utility functions """
 
     def copy(self):
         return SparseFeatureCircuit(
-            node_ie_df=self.node_ie_df.copy(), # type: ignore
-            edge_ie_df=self.edge_ie_df.copy(), # type: ignore
+            node_ie_df=self.node_ie_df.copy(),  # type: ignore
+            edge_ie_df=self.edge_ie_df.copy(),  # type: ignore
         )
 
     @property
     def num_nodes(self) -> int:
         return len(self.node_ie_df)
 
     @property
@@ -187,23 +205,23 @@
         if hasattr(self, "node_ie_df"):
             self.node_ie_df.to_csv(save_dir / "node.csv")
         if hasattr(self, "edge_ie_df"):
             self.edge_ie_df.to_csv(save_dir / "edge.csv")
 
     @staticmethod
     def load(save_dir: pathlib.Path) -> "SparseFeatureCircuit":
-
         # Load results
         if (save_dir / "node.csv").exists():
             node_ie_df = pd.read_csv(save_dir / "node.csv", index_col=0)
-        else: 
+        else:
             node_ie_df = None
         if (save_dir / "edge.csv").exists():
             edge_ie_df = pd.read_csv(save_dir / "edge.csv", index_col=0)
+            if len(edge_ie_df) == 0:
+                edge_ie_df = None
         else:
             edge_ie_df = None
 
         return SparseFeatureCircuit(
-            node_ie_df=node_ie_df, # type: ignore
-            edge_ie_df=edge_ie_df, # type: ignore
+            node_ie_df=node_ie_df,  # type: ignore
+            edge_ie_df=edge_ie_df,  # type: ignore
         )
-
```

### Comparing `token_trace-0.2.1/token_trace/load_pretrained_model.py` & `token_trace-0.3.0/token_trace/load_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.2.1/token_trace/print_prompt_info.py` & `token_trace-0.3.0/token_trace/print_prompt_info.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.2.1/token_trace/sae_activation_cache.py` & `token_trace-0.3.0/token_trace/sae_activation_cache.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.2.1/token_trace/sae_patcher.py` & `token_trace-0.3.0/token_trace/sae_patcher.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.2.1/token_trace/types.py` & `token_trace-0.3.0/token_trace/types.py`

 * *Files identical despite different names*

### Comparing `token_trace-0.2.1/token_trace/utils.py` & `token_trace-0.3.0/token_trace/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import logging
 import urllib.parse
 import webbrowser
-import pandas as pd
-from pandera import DataFrameModel
 from typing import cast
 
+import pandas as pd
 import torch
+from pandera import DataFrameModel
 from transformer_lens import HookedTransformer
 
 from token_trace.load_pretrained_model import load_model
 from token_trace.types import ModuleName
 
 
 def get_neuronpedia_url(
@@ -71,12 +71,16 @@
             "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
         )
         ch = logging.StreamHandler()
         ch.setFormatter(formatter)
         logger.addHandler(ch)
     return logger
 
+
 def get_empty_dataframe_from_pa_model(model: DataFrameModel) -> pd.DataFrame:
     schema = model.to_schema()
     column_names = list(schema.columns.keys())
-    data_types = {column_name: column_type.dtype.type.name for column_name, column_type in schema.columns.items()}
-    return pd.DataFrame(columns=column_names).astype(data_types)
+    data_types = {
+        column_name: column_type.dtype.type.name
+        for column_name, column_type in schema.columns.items()
+    }
+    return pd.DataFrame(columns=column_names).astype(data_types)
```

### Comparing `token_trace-0.2.1/PKG-INFO` & `token_trace-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: token-trace
-Version: 0.2.1
+Version: 0.3.0
 Summary: Transformer token flow visualizer
 Author-Email: "Seongho Son, Liza Karmannaya, Daniel Tan, David Chanin" <chanindav@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: transformers>=4.39.3
 Requires-Dist: transformer-lens>=1.15.0
 Requires-Dist: sae-lens>=0.2.0
```

