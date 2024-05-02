# Comparing `tmp/modgeosys_graph_algorithms-0.4.0.tar.gz` & `tmp/modgeosys_graph_algorithms-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modgeosys_graph_algorithms-0.4.0.tar", max compression
+gzip compressed data, was "modgeosys_graph_algorithms-0.4.1.tar", max compression
```

## Comparing `modgeosys_graph_algorithms-0.4.0.tar` & `modgeosys_graph_algorithms-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     4214 2024-04-29 04:40:54.037521 modgeosys_graph_algorithms-0.4.0/README.md
--rw-r--r--   0        0        0      489 2024-04-29 21:38:44.805145 modgeosys_graph_algorithms-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.4.0/src/modgeosys/__init__.py
--rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/__init__.py
--rw-r--r--   0        0        0     3219 2024-04-29 04:36:13.020391 modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/a_star.py
--rw-r--r--   0        0        0      625 2024-04-28 18:02:46.684609 modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/distance.py
--rw-r--r--   0        0        0      177 2024-04-28 18:02:46.684609 modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/edge_validation.py
--rw-r--r--   0        0        0      408 2024-04-29 04:36:13.064391 modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/edge_weight.py
--rw-r--r--   0        0        0     1696 2024-04-06 19:04:49.983022 modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/prim.py
--rw-r--r--   0        0        0     7744 2024-04-29 04:44:15.842283 modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/types.py
--rw-r--r--   0        0        0     4727 2024-04-29 04:44:15.878284 modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/conftest.py
--rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/generate_a_star_test_data.py
--rw-r--r--   0        0        0     8338 2024-04-29 04:44:15.866284 modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/test_a_star.py
--rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/test_distance.py
--rw-r--r--   0        0        0    24076 2024-04-27 21:40:29.505540 modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/test_prim.py
--rw-r--r--   0        0        0     3775 2024-04-29 04:36:13.028391 modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/test_types.py
--rw-r--r--   0        0        0     4599 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4214 2024-04-29 04:40:54.037521 modgeosys_graph_algorithms-0.4.1/README.md
+-rw-r--r--   0        0        0      489 2024-05-02 19:43:56.661844 modgeosys_graph_algorithms-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.4.1/src/modgeosys/__init__.py
+-rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.4.1/src/modgeosys/graph/__init__.py
+-rw-r--r--   0        0        0     3219 2024-04-29 04:36:13.020391 modgeosys_graph_algorithms-0.4.1/src/modgeosys/graph/a_star.py
+-rw-r--r--   0        0        0      625 2024-04-28 18:02:46.684609 modgeosys_graph_algorithms-0.4.1/src/modgeosys/graph/distance.py
+-rw-r--r--   0        0        0      408 2024-04-29 04:36:13.064391 modgeosys_graph_algorithms-0.4.1/src/modgeosys/graph/edge_weight.py
+-rw-r--r--   0        0        0     1760 2024-05-02 19:43:56.665844 modgeosys_graph_algorithms-0.4.1/src/modgeosys/graph/prim.py
+-rw-r--r--   0        0        0     7744 2024-04-29 04:44:15.842283 modgeosys_graph_algorithms-0.4.1/src/modgeosys/graph/types.py
+-rw-r--r--   0        0        0     4727 2024-04-29 04:44:15.878284 modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/conftest.py
+-rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/generate_a_star_test_data.py
+-rw-r--r--   0        0        0     8338 2024-04-29 04:44:15.866284 modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/test_a_star.py
+-rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/test_distance.py
+-rw-r--r--   0        0        0    24076 2024-04-27 21:40:29.505540 modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/test_prim.py
+-rw-r--r--   0        0        0     3775 2024-04-29 04:36:13.028391 modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/test_types.py
+-rw-r--r--   0        0        0     4599 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.4.1/PKG-INFO
```

### Comparing `modgeosys_graph_algorithms-0.4.0/README.md` & `modgeosys_graph_algorithms-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/a_star.py` & `modgeosys_graph_algorithms-0.4.1/src/modgeosys/graph/a_star.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/distance.py` & `modgeosys_graph_algorithms-0.4.1/src/modgeosys/graph/distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/prim.py` & `modgeosys_graph_algorithms-0.4.1/src/modgeosys/graph/prim.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 """A module containing an implementation of Prim's algorithm for finding the minimum spanning tree of a graph."""
 
 from modgeosys.graph.types import Edge, Graph, ValidEdgeCallable, NoNavigablePathError
-from modgeosys.graph.edge_validation import edge_is_always_valid
+
+
+
+def edge_is_always_valid(_graph: Graph, _edge: Edge) -> bool:
+    """Default:  All edges are valid."""
+    return True
 
 
 def prim(graph: Graph, start_node_index: int, edge_is_valid: ValidEdgeCallable = edge_is_always_valid) -> set[Edge]:
     """Implement Prim's algorithm for finding the minimum spanning tree of a graph."""
 
     nodes = graph.nodes
     edges = graph.edges
@@ -19,15 +24,15 @@
     while excluded_node_indices:
 
         candidate_edges = sorted(edge for edge in excluded_edges if edge.node_indices & included_node_indices)
         best_edge = None
 
         for edge in candidate_edges:
 
-            if edge_is_valid(edge):
+            if edge_is_valid(graph, edge):
 
                 best_edge = edge
                 indices = best_edge.node_indices - included_node_indices
                 if len(indices) != 1:
                     # We've discovered a cycle.  Remove the edge from consideration, and move on.
                     excluded_edges.remove(best_edge)
                     continue
```

### Comparing `modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/types.py` & `modgeosys_graph_algorithms-0.4.1/src/modgeosys/graph/types.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/conftest.py` & `modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/conftest.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/generate_a_star_test_data.py` & `modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/generate_a_star_test_data.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/test_a_star.py` & `modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/test_a_star.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/test_distance.py` & `modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/test_distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/test_prim.py` & `modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/test_prim.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/test_types.py` & `modgeosys_graph_algorithms-0.4.1/tests/modgeosys/graph/test_types.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.4.0/PKG-INFO` & `modgeosys_graph_algorithms-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modgeosys-graph-algorithms
-Version: 0.4.0
+Version: 0.4.1
 Summary: 
 Author: Kevin Weller
 Author-email: klweller@icloud.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: heapdict (>=1.0.1,<2.0.0)
```

