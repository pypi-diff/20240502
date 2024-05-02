# Comparing `tmp/aq_geometric-2024.4.7.2.tar.gz` & `tmp/aq_geometric-2024.5.1.1.tar.gz`

## Comparing `aq_geometric-2024.4.7.2.tar` & `aq_geometric-2024.5.1.1.tar`

### file list

```diff
@@ -1,53 +1,70 @@
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/requirements.txt
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/file/__init__.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/file/local.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/filter/__init__.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/filter/node_features.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/graph/__init__.py
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/graph/compute_graph.py
--rw-r--r--   0        0        0    17055 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/graph/graphs_builder.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/graph/edges/__init__.py
--rw-r--r--   0        0        0     7337 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/graph/edges/compute_edges.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/graph/nodes/__init__.py
--rw-r--r--   0        0        0    14500 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/graph/nodes/compute_node_features.py
--rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/graph/nodes/compute_nodes.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/reindex/__init__.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/reindex/features.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/remote/__init__.py
--rw-r--r--   0        0        0     6877 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/data/remote/psql.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/datasets/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/datasets/in_memory/__init__.py
--rw-r--r--   0        0        0    11724 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/datasets/in_memory/aq_geometric_dataset.py
--rw-r--r--   0        0        0    26545 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/datasets/on_disk/aq_geometric_dataset.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/__init__.py
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/base_model.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/test_base_model.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/edge_conv/__init__.py
--rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/edge_conv/edge_conv.py
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/edge_conv/test_edge_conv.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/gcn/__init__.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/gcn/gcn.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/gcn/test_gcn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/hierarchical_edge_conv/__init__.py
--rw-r--r--   0        0        0    16080 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/hierarchical_edge_conv/heirarchical_edge_conv.py
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/models/hierarchical_edge_conv/test_heirarchical_edge_conv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/transforms/__init__.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/utils/__init__.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/utils/evaluation.py
--rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/utils/forecasts.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/utils/station_filters.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/utils/test_evaluation.py
--rw-r--r--   0        0        0     5440 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/utils/test_forecasts.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/aq_geometric/utils/test_station_filters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/tests/config/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/tests/data/__init__.py
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/tests/data/test_aq.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/tests/datasets/__init__.py
--rw-r--r--   0        0        0    10356 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/tests/datasets/test_aq.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/LICENSE.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/README.md
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/pyproject.toml
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 aq_geometric-2024.4.7.2/PKG-INFO
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/requirements.txt
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/data/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/data/file/__init__.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/data/file/local.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/data/filter/__init__.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/data/filter/node_features.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/data/graph/__init__.py
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/data/graph/compute_graph.py
+-rw-r--r--   0        0        0    17055 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/data/graph/graphs_builder.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/data/graph/edges/__init__.py
+-rw-r--r--   0        0        0     7337 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/data/graph/edges/compute_edges.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/data/graph/nodes/__init__.py
+-rw-r--r--   0        0        0    14503 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/data/graph/nodes/compute_node_features.py
+-rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/data/graph/nodes/compute_nodes.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/data/reindex/__init__.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/data/reindex/features.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/data/remote/__init__.py
+-rw-r--r--   0        0        0     6877 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/data/remote/psql.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/datasets/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/datasets/in_memory/__init__.py
+-rw-r--r--   0        0        0    11724 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/datasets/in_memory/aq_geometric_dataset.py
+-rw-r--r--   0        0        0    26866 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/datasets/on_disk/aq_geometric_dataset.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/__init__.py
+-rw-r--r--   0        0        0     9747 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/base_model.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/test_base_model.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/edge_conv/__init__.py
+-rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/edge_conv/edge_conv.py
+-rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/edge_conv/test_edge_conv.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/gcn/__init__.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/gcn/gcn.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/gcn/test_gcn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/hierarchical_edge_conv/__init__.py
+-rw-r--r--   0        0        0    18524 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/hierarchical_edge_conv/heirarchical_edge_conv.py
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/hierarchical_edge_conv/test_heirarchical_edge_conv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/hierarchical_xgb/__init__.py
+-rw-r--r--   0        0        0    31182 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/hierarchical_xgb/base_hierarchical_xgb.py
+-rw-r--r--   0        0        0     8125 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/hierarchical_xgb/hierarchical_xgb_direct.py
+-rw-r--r--   0        0        0    10666 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/hierarchical_xgb/hierarchical_xgb_iterative.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/message_passing/__init__.py
+-rw-r--r--   0        0        0    14655 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/message_passing/message_passing.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/message_passing/test_message_passing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/statistical_baselines/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/statistical_baselines/climatology/__init__.py
+-rw-r--r--   0        0        0     8464 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/statistical_baselines/climatology/climatology.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/statistical_baselines/linear/__init__.py
+-rw-r--r--   0        0        0     7812 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/statistical_baselines/linear/linear.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/statistical_baselines/persistance/__init__.py
+-rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/statistical_baselines/persistance/persistance.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/statistical_baselines/temporal/__init__.py
+-rw-r--r--   0        0        0     8997 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/models/statistical_baselines/temporal/temporal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/transforms/__init__.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/transforms/change.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/utils/__init__.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/utils/evaluation.py
+-rw-r--r--   0        0        0     6336 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/utils/forecasts.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/utils/station_filters.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/utils/test_evaluation.py
+-rw-r--r--   0        0        0     5440 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/utils/test_forecasts.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/aq_geometric/utils/test_station_filters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/tests/config/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/tests/data/__init__.py
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/tests/data/test_aq.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/tests/datasets/__init__.py
+-rw-r--r--   0        0        0    10356 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/tests/datasets/test_aq.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/LICENSE.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/README.md
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 aq_geometric-2024.5.1.1/PKG-INFO
```

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/data/file/local.py` & `aq_geometric-2024.5.1.1/aq_geometric/data/file/local.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/data/filter/node_features.py` & `aq_geometric-2024.5.1.1/aq_geometric/data/filter/node_features.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/data/graph/compute_graph.py` & `aq_geometric-2024.5.1.1/aq_geometric/data/graph/compute_graph.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/data/graph/graphs_builder.py` & `aq_geometric-2024.5.1.1/aq_geometric/data/graph/graphs_builder.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/data/graph/edges/compute_edges.py` & `aq_geometric-2024.5.1.1/aq_geometric/data/graph/edges/compute_edges.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/data/graph/nodes/compute_node_features.py` & `aq_geometric-2024.5.1.1/aq_geometric/data/graph/nodes/compute_node_features.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,15 +185,15 @@
         print(
             f"[{datetime.now()}] processing resolutions between {leaf_h3_resolution} and {min_h3_resolution} inclusive with root set to {include_root_node}"
         )
 
     for i in range(leaf_h3_resolution, min_h3_resolution - 1, -1):
         h3_df = df.copy()
         h3_df["timestamp"] = pd.to_datetime(h3_df["timestamp"])
-        h3_df["h3_index"] = df.apply(
+        h3_df["h3_index"] = h3_df.apply(
             lambda x: h3.geo_to_h3(x.latitude, x.longitude, i), axis=1)
         h3_df = h3_df.groupby(["h3_index",
                                "timestamp"]).mean(numeric_only=True)
         levels.append(h3_df[["value"]])
         if verbose:
             print(
                 f"[{datetime.now()}] after processing resolution {i}, h3_df has shape {h3_df.shape}"
@@ -208,15 +208,15 @@
                                    "timestamp"]).mean(numeric_only=True)
         levels.append(root_df[["value"]])
         if verbose:
             print(
                 f"[{datetime.now()}] after processing root node, root_df has shape {root_df.shape}"
             )
 
-    # concatinate all dataframes in levels
+    # concatenate all dataframes in levels
     df_lvl = pd.concat(levels, axis=0)
     if verbose:
         print(
             f"[{datetime.now()}] after concatenating levels, df_lvl has shape {df_lvl.shape}"
         )
     df_lvl.reset_index(inplace=True)
```

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/data/graph/nodes/compute_nodes.py` & `aq_geometric-2024.5.1.1/aq_geometric/data/graph/nodes/compute_nodes.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/data/reindex/features.py` & `aq_geometric-2024.5.1.1/aq_geometric/data/reindex/features.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/data/remote/psql.py` & `aq_geometric-2024.5.1.1/aq_geometric/data/remote/psql.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/datasets/in_memory/aq_geometric_dataset.py` & `aq_geometric-2024.5.1.1/aq_geometric/datasets/in_memory/aq_geometric_dataset.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/datasets/on_disk/aq_geometric_dataset.py` & `aq_geometric-2024.5.1.1/aq_geometric/datasets/on_disk/aq_geometric_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,23 +218,16 @@
                     table="hourly_data",
                     start_time=q_start_time,
                     end_time=q_end_time,
                     feature=f,
                     selected_aqsids=self.selected_aqsids,
                     verbose=self.verbose,
                 )
-                feature_df = data_to_feature(
-                    df=data_df,
-                    stations_info_df=stations_info,
-                    min_h3_resolution=self.min_h3_resolution,
-                    leaf_h3_resolution=self.leaf_h3_resolution,
-                    verbose=self.verbose,
-                )
-                # save the hourly features and targets
-                feature_df.to_csv(osp.join(self.raw_dir, f"{f}_data_{i}.csv"),
+                # save the hourly data
+                data_df.to_csv(osp.join(self.raw_dir, f"{f}_data_{i}.csv"),
                                   index=False)
         return None
 
     def process(self):
         """Process the data and stations info into individual graphs."""
         # ensure the processed directory exists
         if not osp.exists(self.processed_dir):
@@ -309,35 +302,49 @@
                                              freq=self.freq, inclusive="left")
 
             # load node features from disk
             node_features = []
             # load the node features from the local file
             for feature in self.features:
                 feature_fp = osp.join(self.raw_dir, f"{feature}_data_{i}.csv")
-                feature_df = load_hourly_feature_from_fp(feature_fp)
-                feature = get_node_feature(
+                data_df = load_hourly_data_from_fp(feature_fp)
+                feature_df = data_to_feature(
+                    df=data_df,
+                    stations_info_df=self.stations_info_df,
+                    min_h3_resolution=self.min_h3_resolution,
+                    leaf_h3_resolution=self.leaf_h3_resolution,
+                    verbose=self.verbose,
+                )
+                node_feature = get_node_feature(
                     feature_df=feature_df,
                     timestamps=graph_timestamps,
                     nodes=self.nodes,
                     verbose=self.verbose,
                 )
-                node_features.append(feature)
+                node_features.append(node_feature)
             # load node targets from disk
             node_targets = []
             # load the node features from the local file
             for feature in self.targets:
                 feature_fp = osp.join(self.raw_dir, f"{feature}_data_{i}.csv")
-                feature_df = load_hourly_feature_from_fp(feature_fp)
-                feature = get_node_feature(
+                data_df = load_hourly_data_from_fp(feature_fp)
+                feature_df = data_to_feature(
+                    df=data_df,
+                    stations_info_df=self.stations_info_df,
+                    min_h3_resolution=self.min_h3_resolution,
+                    leaf_h3_resolution=self.leaf_h3_resolution,
+                    verbose=self.verbose,
+                )
+                node_feature = get_node_feature(
                     feature_df=feature_df,
                     timestamps=graph_timestamps,
                     nodes=self.nodes,
                     verbose=self.verbose,
                 )
-                node_targets.append(feature)
+                node_targets.append(node_feature)
             # stack the features and targets
             node_features = stack_node_features(self.nodes, node_features)
             node_targets = stack_node_features(self.nodes, node_targets)
             # make the graph
             graph = make_graph(
                 nodes=self.nodes,
                 edges=self.edges[["from", "to"]].to_numpy().T,
```

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/models/test_base_model.py` & `aq_geometric-2024.5.1.1/aq_geometric/models/test_base_model.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/models/edge_conv/edge_conv.py` & `aq_geometric-2024.5.1.1/aq_geometric/models/edge_conv/edge_conv.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/models/edge_conv/test_edge_conv.py` & `aq_geometric-2024.5.1.1/aq_geometric/models/edge_conv/test_edge_conv.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/models/gcn/gcn.py` & `aq_geometric-2024.5.1.1/aq_geometric/models/gcn/gcn.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/models/gcn/test_gcn.py` & `aq_geometric-2024.5.1.1/aq_geometric/models/gcn/test_gcn.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/models/hierarchical_edge_conv/heirarchical_edge_conv.py` & `aq_geometric-2024.5.1.1/aq_geometric/models/hierarchical_edge_conv/heirarchical_edge_conv.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import os
+from datetime import datetime
 from typing import Dict, List, Tuple, Union
 
 import uuid
 import torch
 import h3
 import numpy as np
+import pandas as pd
+from torch_geometric.data import Data
 from torch.nn import Sequential as Seq, Linear, ReLU
 from torch_geometric.nn import MessagePassing, ChebConv
 from torch_geometric.nn import aggr
+from aq_utilities.data import hourly_predictions_to_postgres
 
 from aq_geometric.models.base_model import BaseModel
 
 
 class HierarchicalEdgeConv(MessagePassing):
     def __init__(self, in_channels, aggr=aggr.SoftmaxAggregation(learn=True)):
         super().__init__(aggr=aggr)
@@ -70,20 +74,21 @@
         name: str = "AqHierarchicalEdgeConvModel",
         guid: str = str(uuid.uuid4()),
         stations: Union[List, None] = None,
         features: List[str] = ["OZONE", "PM2.5", "NO2"],
         targets: List[str] = ["OZONE", "PM2.5", "NO2"],
         num_samples_in_node_feature: int = 48,
         num_samples_in_node_target: int = 12,
+        is_iterative: bool = False,
         finest_resolution: int = 6,
         coarsest_resolution: int = -1,
         cheb_k: int = 2,
         verbose: bool = False,
     ):
-        super().__init__(name=name, guid=guid, stations=stations, features=features, targets=targets, num_samples_in_node_feature=num_samples_in_node_feature, num_samples_in_node_target=num_samples_in_node_target)
+        super().__init__(name=name, guid=guid, stations=stations, features=features, targets=targets, num_samples_in_node_feature=num_samples_in_node_feature, num_samples_in_node_target=num_samples_in_node_target, is_iterative=is_iterative)
         self.num_features_in_node_feature = len(features)
         self.num_features_in_node_target = len(targets)
         self.finest_resolution = finest_resolution
         self.coarsest_resolution = coarsest_resolution
         self.cheb_k = cheb_k
         self.num_resolutions_between_finest_and_coarsest = finest_resolution - coarsest_resolution
         self.edges_low_to_high_resolution = edges_low_to_high_resolution
@@ -171,14 +176,15 @@
             "stations": self.stations,
             "edges_high_to_low_resolution": self.edges_high_to_low_resolution,
             "edges_low_to_high_resolution": self.edges_low_to_high_resolution,
             "features": self.features,
             "targets": self.targets,
             "num_samples_in_node_feature": self.num_samples_in_node_feature,
             "num_samples_in_node_target": self.num_samples_in_node_target,
+            "is_iterative": self.is_iterative,
             "finest_resolution": self.finest_resolution,
             "coarsest_resolution": self.coarsest_resolution,
             "cheb_k": self.cheb_k,
             "state_dict": self.state_dict(),
             **self.kwargs
         }
         # save the model data
@@ -199,34 +205,88 @@
             "edges_low_to_high_resolution"]
         self.features = model_data["features"]
         self.targets = model_data["targets"]
         self.num_samples_in_node_feature = model_data[
             "num_samples_in_node_feature"]
         self.num_samples_in_node_target = model_data[
             "num_samples_in_node_target"]
+        self.is_iterative = model_data["is_iterative"]
         self.finest_resolution = model_data.get("finest_resolution")
         self.coarsest_resolution = model_data.get("coarsest_resolution")
         self.cheb_k = model_data.get("cheb_k")
 
         self.load_state_dict(model_data["state_dict"])
 
         # set the kwargs
         for key, value in model_data.items():
-            if key not in ["name", "guid", "stations", "edges_high_to_low_resolution", "edges_low_to_high_resolution", "features", "targets", "num_samples_in_node_feature", "num_samples_in_node_target", "num_features_in_node_feature", "num_features_in_node_target", "state_dict"]:
+            if key not in ["name", "guid", "stations", "edges_high_to_low_resolution", "edges_low_to_high_resolution", "features", "targets", "num_samples_in_node_feature", "num_samples_in_node_target", "is_iterative", "num_features_in_node_feature", "num_features_in_node_target", "state_dict"]:
                 setattr(self, key, value)
 
     def __repr__(self):
         """Use the torch default representation, add new attrs."""
         representation = super().__repr__()
         # add new lines with the name, guid, and stations
         representation += f"\nFinest h3 resolution: {self.finest_resolution}"
         representation += f"\Coarsest h3 resolution: {self.coarsest_resolution}"
 
         return representation
 
+    def generate_forecasts(
+        self,
+        graph: "Data",
+        targets: List[str],
+        include_history: bool = False,
+        verbose: bool = False,
+    ) -> Tuple[Dict[str, pd.DataFrame], np.ndarray, np.ndarray]:
+        """
+        Generate forecasts using the model provided
+        """
+        forecasts = []
+
+        inputs = graph.x
+        input_edge_index = graph.edge_index
+        h3_indices = graph.h3_index
+        aqsids = graph.aqsid
+        timestamps = graph.timestamps
+        feature_timestamps = graph.feature_timestamps
+        target_timestamps = graph.target_timestamps
+
+        with torch.no_grad():
+            if verbose:
+                print(f"[{datetime.now()}] generating forecasts for {len(h3_indices)} h3 indices")
+            pred = self(inputs, input_edge_index)
+            # reshape the prediction to the shape of the target
+            pred = pred.numpy().reshape(graph.y_mask.shape)
+        
+        # prepare the forecasts, including the history
+        target_dfs = {}
+        history = graph.x.detach().numpy()
+        testmask = graph.x_mask[:, 0, :].detach().numpy()
+        forecasts = (testmask.reshape(-1, 1, len(targets)) * pred)
+
+        for i, target in enumerate(targets):
+            if verbose:
+                print(f"[{datetime.now()}] preparing forecast for {target}")
+            history_df = pd.DataFrame(
+                history[:,:,i], columns=feature_timestamps, index=h3_indices
+            ) if include_history else pd.DataFrame()
+            if verbose:
+                print(f"[{datetime.now()}] history df shape for {target}: {history_df.shape}")
+            forecast_df = pd.DataFrame(
+                forecasts[:,:,i], columns=target_timestamps, index=h3_indices
+            )
+            if verbose:
+                print(f"[{datetime.now()}] forecast df shape for {target}: {forecast_df.shape}")
+            df = pd.concat([history_df, forecast_df], axis=1)
+            target_dfs[target] = df
+            if verbose:
+                print(f"[{datetime.now()}] added DataFrame {df.shape}")
+
+        return target_dfs, forecasts, pred
+
 
 def process_aq_geometric_dataset_edges_by_h3_resolution(
     graph: "torch_geometric.data.data.Data",
     graph_includes_root_node: bool = True,
     force_self_loops: bool = True,
     force_bidirectional_edges: bool = True,
     verbose: bool = False,
@@ -327,19 +387,19 @@
         if verbose:
             print(f"processing edges and edge attributes at h3 resolution {k}")
         edges_same_resolution[k] = torch.cat(
             (self_edges, torch.tensor(edges_same_resolution[k], dtype=int).T),
             dim=1)
         edges_high_to_low_resolution[k] = torch.cat(
             (edges_same_resolution[k],
-             torch.tensor(edges_high_to_low_resolution[k], dtype=int).T),
+            torch.tensor(edges_high_to_low_resolution[k], dtype=int).T),
             dim=1)
         edges_low_to_high_resolution[k] = torch.cat(
             (edges_same_resolution[k],
-             torch.tensor(edges_low_to_high_resolution[k], dtype=int).T),
+            torch.tensor(edges_low_to_high_resolution[k], dtype=int).T),
             dim=1)
         if verbose:
             print(
                 f"before removing duplicates, edges have shape: {edges_same_resolution[k].shape}, {edges_high_to_low_resolution[k].shape}, {edges_low_to_high_resolution[k].shape}"
             )
         edges_same_resolution[k] = torch.unique(edges_same_resolution[k],
                                                 dim=1)
@@ -354,15 +414,15 @@
 
     # change the graph's edge_index in place
     if verbose: print("changing the graph's edge_index in place")
     new_edge_index = torch.unique(
         torch.cat([
             torch.cat(
                 (edges_same_resolution[k], edges_low_to_high_resolution[k],
-                 edges_high_to_low_resolution[k]), dim=1)
+                edges_high_to_low_resolution[k]), dim=1)
             for k in range(min_h3_resolution, max_h3_resolution + 1)
         ], dim=1), dim=1)
     if verbose:
         print(
             f"old edge_index shape: {graph.edge_index.shape}, new edge_index shape: {new_edge_index.shape}"
         )
     graph.edge_index = new_edge_index
```

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/models/hierarchical_edge_conv/test_heirarchical_edge_conv.py` & `aq_geometric-2024.5.1.1/aq_geometric/models/hierarchical_edge_conv/test_heirarchical_edge_conv.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/utils/evaluation.py` & `aq_geometric-2024.5.1.1/aq_geometric/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/utils/forecasts.py` & `aq_geometric-2024.5.1.1/aq_geometric/utils/forecasts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from datetime import datetime
-from typing import Dict, Union, List
+from typing import Tuple, Dict, Union, List
 
 import torch
 import numpy as np
 import pandas as pd
+from torch_geometric.data import Data
 from aq_utilities.data import hourly_predictions_to_postgres
 
 
 def generate_forecasts_graph(
     model: "aq_geometric.models.base_model.BaseModel",
     dataset: "AqGeometricInMemoryDataset",
     targets: List[str],
     include_history: bool = False,
     verbose: bool = False,
-) -> Dict[str, pd.DataFrame]:
+) -> Tuple[Dict[str, pd.DataFrame], Data, np.ndarray, np.ndarray]:
     """
     Generate forecasts using the model provided
     """
     forecasts = []
 
     # obtain data attributes
     if verbose:
@@ -58,15 +59,15 @@
         if verbose:
             print(f"[{datetime.now()}] forecast df shape for {target}: {forecast_df.shape}")
         df = pd.concat([history_df, forecast_df], axis=1)
         target_dfs[target] = df
         if verbose:
             print(f"[{datetime.now()}] added DataFrame {df.shape}")
 
-    return target_dfs, g
+    return target_dfs, g, pred, forecasts
 
 
 def forecasts_df_to_db(
     engine: str,
     model: "aq_geometric.models.base_model.BaseModel",
     graph: "Data",
     target_dfs: Dict[str, pd.DataFrame],
```

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/utils/station_filters.py` & `aq_geometric-2024.5.1.1/aq_geometric/utils/station_filters.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/utils/test_evaluation.py` & `aq_geometric-2024.5.1.1/aq_geometric/utils/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/utils/test_forecasts.py` & `aq_geometric-2024.5.1.1/aq_geometric/utils/test_forecasts.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/aq_geometric/utils/test_station_filters.py` & `aq_geometric-2024.5.1.1/aq_geometric/utils/test_station_filters.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/tests/data/test_aq.py` & `aq_geometric-2024.5.1.1/tests/data/test_aq.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/tests/datasets/test_aq.py` & `aq_geometric-2024.5.1.1/tests/datasets/test_aq.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/.gitignore` & `aq_geometric-2024.5.1.1/.gitignore`

 * *Files 13% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 *.pt
 
 # dev
 kubeflow/components/data_pull_e2e/*
 
 # do not ignore notebooks named overview directory
 */notebooks/**
-!*/notebooks/overview.ipynb
+!*/notebooks/overview*.ipynb
 raw-data/**
 # frontend
 .svelte-kit
 .DS_Store
 node_modules
 /build
 /.svelte-kit
@@ -48,12 +48,13 @@
 vite.config.ts.timestamp-*
 env.ts
 
 # ignore data files
 *.csv
 *.json
 *.pkl
+*.old
 
 # except those that track kubeflow state
 !kubeflow/state.json
 !kubeflow/desired_state.json
 !sample-fe-data.json
```

### Comparing `aq_geometric-2024.4.7.2/LICENSE.md` & `aq_geometric-2024.5.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.4.7.2/pyproject.toml` & `aq_geometric-2024.5.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="aq-geometric"
-version="2024.04.07.2"
+version="2024.05.01.1"
 authors=[
     {name="Chris Jellen", email="cdjellen@gmail.com"},
 ]
 description="Geometric deep learning on air quality data."
 readme="README.md"
 requires-python=">=3.9"
 keywords=[
@@ -23,14 +23,15 @@
 ]
 dependencies=[
     "torch_geometric==2.3.1",
     "torch==2.0.1",
     "pandas==1.5.3",
     "sqlalchemy==2.0.23",
     "psycopg2-binary==2.9.9",
+    "xgboost==2.0.3",
     "aq-utilities"
 ]
 
 [project.urls]
 homepage="https://github.com/cdjellen/aq"
 documentation="https://github.com/cdjellen/aq"
```

### Comparing `aq_geometric-2024.4.7.2/PKG-INFO` & `aq_geometric-2024.5.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aq-geometric
-Version: 2024.4.7.2
+Version: 2024.5.1.1
 Summary: Geometric deep learning on air quality data.
 Project-URL: homepage, https://github.com/cdjellen/aq
 Project-URL: documentation, https://github.com/cdjellen/aq
 Author-email: Chris Jellen <cdjellen@gmail.com>
 License-File: LICENSE.md
 Keywords: deep-learning,earth-systems,geometric-deep-learning,pytorch
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +16,15 @@
 Requires-Python: >=3.9
 Requires-Dist: aq-utilities
 Requires-Dist: pandas==1.5.3
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: sqlalchemy==2.0.23
 Requires-Dist: torch-geometric==2.3.1
 Requires-Dist: torch==2.0.1
+Requires-Dist: xgboost==2.0.3
 Description-Content-Type: text/markdown
 
 ## Overview
 
 This repository contains the code used for geometric deep learning on air-quality data. The code is based on the [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/) library.
 
 Generate build artifacts via ```python3 pip wheel --no-cache-dir --extra-index-url=https://download.pytorch.org/whl/cpu aq-geometric/ -w kubeflow/artifacts/wheels/aq-geometric/```
```

