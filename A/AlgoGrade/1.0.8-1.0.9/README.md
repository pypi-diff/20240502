# Comparing `tmp/AlgoGrade-1.0.8.tar.gz` & `tmp/AlgoGrade-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AlgoGrade-1.0.8.tar", last modified: Wed Mar 20 13:11:54 2024, max compression
+gzip compressed data, was "AlgoGrade-1.0.9.tar", last modified: Thu Apr  4 20:05:33 2024, max compression
```

## Comparing `AlgoGrade-1.0.8.tar` & `AlgoGrade-1.0.9.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-03-20 13:11:54.244469 AlgoGrade-1.0.8/
-drwxrwxrwx   0        0        0        0 2024-03-20 13:11:54.045935 AlgoGrade-1.0.8/AlgoGrade/
--rw-rw-rw-   0        0        0        0 2023-06-26 14:08:55.000000 AlgoGrade-1.0.8/AlgoGrade/__init__.py
--rw-rw-rw-   0        0        0     7734 2024-01-22 20:25:47.000000 AlgoGrade-1.0.8/AlgoGrade/adapters.py
--rw-rw-rw-   0        0        0     8524 2024-01-22 20:26:01.000000 AlgoGrade-1.0.8/AlgoGrade/core.py
--rw-rw-rw-   0        0        0     6142 2024-01-22 20:42:08.000000 AlgoGrade-1.0.8/AlgoGrade/dynamic_hull.py
--rw-rw-rw-   0        0        0     5905 2024-03-20 13:04:49.000000 AlgoGrade-1.0.8/AlgoGrade/graham.py
--rw-rw-rw-   0        0        0      483 2024-01-16 17:07:12.000000 AlgoGrade-1.0.8/AlgoGrade/parsers.py
--rw-rw-rw-   0        0        0     1873 2024-01-22 20:07:28.000000 AlgoGrade-1.0.8/AlgoGrade/preparata.py
--rw-rw-rw-   0        0        0     2742 2024-01-22 20:14:55.000000 AlgoGrade-1.0.8/AlgoGrade/quickhull.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:11:54.236030 AlgoGrade-1.0.8/AlgoGrade.egg-info/
--rw-rw-rw-   0        0        0     1049 2024-03-20 13:11:53.000000 AlgoGrade-1.0.8/AlgoGrade.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1042 2024-03-20 13:11:54.000000 AlgoGrade-1.0.8/AlgoGrade.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-20 13:11:53.000000 AlgoGrade-1.0.8/AlgoGrade.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      247 2024-03-20 13:11:53.000000 AlgoGrade-1.0.8/AlgoGrade.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-03-20 13:11:53.000000 AlgoGrade-1.0.8/AlgoGrade.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1104 2023-06-22 12:18:56.000000 AlgoGrade-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     1049 2024-03-20 13:11:54.241468 AlgoGrade-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-06-22 12:17:48.000000 AlgoGrade-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-03-20 13:11:54.244469 AlgoGrade-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      928 2024-03-20 13:09:44.000000 AlgoGrade-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:11:54.080934 AlgoGrade-1.0.8/tests/
--rw-rw-rw-   0        0        0        0 2023-06-26 14:09:13.000000 AlgoGrade-1.0.8/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:11:54.193360 AlgoGrade-1.0.8/tests/adapters/
--rw-rw-rw-   0        0        0        0 2024-01-22 18:31:53.000000 AlgoGrade-1.0.8/tests/adapters/__init__.py
--rw-rw-rw-   0        0        0     3537 2023-08-22 15:54:13.000000 AlgoGrade-1.0.8/tests/adapters/test_core.py
--rw-rw-rw-   0        0        0     2459 2024-01-12 11:30:00.000000 AlgoGrade-1.0.8/tests/adapters/test_dynamic_hull.py
--rw-rw-rw-   0        0        0     1643 2024-01-12 10:51:17.000000 AlgoGrade-1.0.8/tests/adapters/test_graham.py
--rw-rw-rw-   0        0        0     2324 2024-01-11 17:35:02.000000 AlgoGrade-1.0.8/tests/adapters/test_interlibrary_converters.py
--rw-rw-rw-   0        0        0     1298 2024-01-16 09:59:41.000000 AlgoGrade-1.0.8/tests/adapters/test_quickhull.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:11:54.206569 AlgoGrade-1.0.8/tests/answers/
--rw-rw-rw-   0        0        0        0 2024-01-22 18:32:01.000000 AlgoGrade-1.0.8/tests/answers/__init__.py
--rw-rw-rw-   0        0        0     1174 2024-01-22 20:42:24.000000 AlgoGrade-1.0.8/tests/answers/test_dynamic_hull.py
--rw-rw-rw-   0        0        0     1228 2024-03-20 13:07:18.000000 AlgoGrade-1.0.8/tests/answers/test_graham.py
--rw-rw-rw-   0        0        0     1008 2024-01-22 20:36:50.000000 AlgoGrade-1.0.8/tests/answers/test_preparata.py
--rw-rw-rw-   0        0        0      933 2024-01-22 20:37:14.000000 AlgoGrade-1.0.8/tests/answers/test_quickhull.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:11:54.223920 AlgoGrade-1.0.8/tests/graders/
--rw-rw-rw-   0        0        0        0 2024-01-22 18:32:08.000000 AlgoGrade-1.0.8/tests/graders/__init__.py
--rw-rw-rw-   0        0        0    19233 2024-01-23 07:10:12.000000 AlgoGrade-1.0.8/tests/graders/test_dynamic_hull.py
--rw-rw-rw-   0        0        0    11795 2024-03-20 12:49:53.000000 AlgoGrade-1.0.8/tests/graders/test_graham.py
--rw-rw-rw-   0        0        0     3218 2024-01-22 18:18:09.000000 AlgoGrade-1.0.8/tests/graders/test_mock.py
--rw-rw-rw-   0        0        0    14085 2024-01-22 20:09:02.000000 AlgoGrade-1.0.8/tests/graders/test_preparata.py
--rw-rw-rw-   0        0        0     8640 2024-01-22 20:34:35.000000 AlgoGrade-1.0.8/tests/graders/test_quickhull.py
-drwxrwxrwx   0        0        0        0 2024-03-20 13:11:54.233553 AlgoGrade-1.0.8/tests/parsers/
--rw-rw-rw-   0        0        0        0 2024-01-22 18:32:30.000000 AlgoGrade-1.0.8/tests/parsers/__init__.py
--rw-rw-rw-   0        0        0      387 2024-01-16 17:08:13.000000 AlgoGrade-1.0.8/tests/parsers/test_point_list_and_target_point_parser.py
--rw-rw-rw-   0        0        0      292 2024-01-16 17:08:41.000000 AlgoGrade-1.0.8/tests/parsers/test_point_list_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-04 20:05:33.839846 AlgoGrade-1.0.9/
+drwxrwxrwx   0        0        0        0 2024-04-04 20:05:33.545574 AlgoGrade-1.0.9/AlgoGrade/
+-rw-rw-rw-   0        0        0        0 2023-06-26 14:08:55.000000 AlgoGrade-1.0.9/AlgoGrade/__init__.py
+-rw-rw-rw-   0        0        0    11276 2024-04-04 19:51:21.000000 AlgoGrade-1.0.9/AlgoGrade/adapters.py
+-rw-rw-rw-   0        0        0     8524 2024-01-22 20:26:01.000000 AlgoGrade-1.0.9/AlgoGrade/core.py
+-rw-rw-rw-   0        0        0     6613 2024-04-04 18:51:54.000000 AlgoGrade-1.0.9/AlgoGrade/dynamic_hull.py
+-rw-rw-rw-   0        0        0     5905 2024-03-20 13:04:49.000000 AlgoGrade-1.0.9/AlgoGrade/graham.py
+-rw-rw-rw-   0        0        0      483 2024-01-16 17:07:12.000000 AlgoGrade-1.0.9/AlgoGrade/parsers.py
+-rw-rw-rw-   0        0        0     2858 2024-04-04 19:35:58.000000 AlgoGrade-1.0.9/AlgoGrade/preparata.py
+-rw-rw-rw-   0        0        0     2938 2024-04-04 19:54:30.000000 AlgoGrade-1.0.9/AlgoGrade/quickhull.py
+drwxrwxrwx   0        0        0        0 2024-04-04 20:05:33.832754 AlgoGrade-1.0.9/AlgoGrade.egg-info/
+-rw-rw-rw-   0        0        0     1049 2024-04-04 20:05:33.000000 AlgoGrade-1.0.9/AlgoGrade.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1085 2024-04-04 20:05:33.000000 AlgoGrade-1.0.9/AlgoGrade.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 20:05:33.000000 AlgoGrade-1.0.9/AlgoGrade.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      247 2024-04-04 20:05:33.000000 AlgoGrade-1.0.9/AlgoGrade.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-04 20:05:33.000000 AlgoGrade-1.0.9/AlgoGrade.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1104 2023-06-22 12:18:56.000000 AlgoGrade-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1049 2024-04-04 20:05:33.835791 AlgoGrade-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2024-04-04 20:03:37.000000 AlgoGrade-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-04 20:05:33.839867 AlgoGrade-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      928 2024-04-04 20:01:58.000000 AlgoGrade-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 20:05:33.737756 AlgoGrade-1.0.9/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-26 14:09:13.000000 AlgoGrade-1.0.9/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-04 20:05:33.760195 AlgoGrade-1.0.9/tests/adapters/
+-rw-rw-rw-   0        0        0        0 2024-01-22 18:31:53.000000 AlgoGrade-1.0.9/tests/adapters/__init__.py
+-rw-rw-rw-   0        0        0     5834 2024-04-04 20:04:19.000000 AlgoGrade-1.0.9/tests/adapters/test_basic_adapters.py
+-rw-rw-rw-   0        0        0     3852 2024-04-04 19:00:06.000000 AlgoGrade-1.0.9/tests/adapters/test_dynamic_hull.py
+-rw-rw-rw-   0        0        0     2044 2024-04-04 19:06:11.000000 AlgoGrade-1.0.9/tests/adapters/test_graham.py
+-rw-rw-rw-   0        0        0     2324 2024-01-11 17:35:02.000000 AlgoGrade-1.0.9/tests/adapters/test_interlibrary_converters.py
+-rw-rw-rw-   0        0        0     1949 2024-04-04 19:34:56.000000 AlgoGrade-1.0.9/tests/adapters/test_preparata.py
+-rw-rw-rw-   0        0        0     1894 2024-04-04 19:55:52.000000 AlgoGrade-1.0.9/tests/adapters/test_quickhull.py
+drwxrwxrwx   0        0        0        0 2024-04-04 20:05:33.779865 AlgoGrade-1.0.9/tests/answers/
+-rw-rw-rw-   0        0        0        0 2024-01-22 18:32:01.000000 AlgoGrade-1.0.9/tests/answers/__init__.py
+-rw-rw-rw-   0        0        0     1174 2024-01-22 20:42:24.000000 AlgoGrade-1.0.9/tests/answers/test_dynamic_hull.py
+-rw-rw-rw-   0        0        0     1228 2024-03-20 13:07:18.000000 AlgoGrade-1.0.9/tests/answers/test_graham.py
+-rw-rw-rw-   0        0        0     1014 2024-04-04 19:37:16.000000 AlgoGrade-1.0.9/tests/answers/test_preparata.py
+-rw-rw-rw-   0        0        0      935 2024-04-04 20:01:03.000000 AlgoGrade-1.0.9/tests/answers/test_quickhull.py
+drwxrwxrwx   0        0        0        0 2024-04-04 20:05:33.811093 AlgoGrade-1.0.9/tests/graders/
+-rw-rw-rw-   0        0        0        0 2024-01-22 18:32:08.000000 AlgoGrade-1.0.9/tests/graders/__init__.py
+-rw-rw-rw-   0        0        0    19233 2024-01-23 07:10:12.000000 AlgoGrade-1.0.9/tests/graders/test_dynamic_hull.py
+-rw-rw-rw-   0        0        0    11795 2024-03-20 12:49:53.000000 AlgoGrade-1.0.9/tests/graders/test_graham.py
+-rw-rw-rw-   0        0        0     3218 2024-01-22 18:18:09.000000 AlgoGrade-1.0.9/tests/graders/test_mock.py
+-rw-rw-rw-   0        0        0    14182 2024-04-04 19:51:37.000000 AlgoGrade-1.0.9/tests/graders/test_preparata.py
+-rw-rw-rw-   0        0        0     8640 2024-01-22 20:34:35.000000 AlgoGrade-1.0.9/tests/graders/test_quickhull.py
+drwxrwxrwx   0        0        0        0 2024-04-04 20:05:33.824595 AlgoGrade-1.0.9/tests/parsers/
+-rw-rw-rw-   0        0        0        0 2024-01-22 18:32:30.000000 AlgoGrade-1.0.9/tests/parsers/__init__.py
+-rw-rw-rw-   0        0        0      387 2024-01-16 17:08:13.000000 AlgoGrade-1.0.9/tests/parsers/test_point_list_and_target_point_parser.py
+-rw-rw-rw-   0        0        0      292 2024-01-16 17:08:41.000000 AlgoGrade-1.0.9/tests/parsers/test_point_list_parser.py
```

### Comparing `AlgoGrade-1.0.8/AlgoGrade/adapters.py` & `AlgoGrade-1.0.9/AlgoGrade/adapters.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+from __future__ import annotations
 from functools import cached_property
-from typing import Any, ClassVar, Optional, Iterable, Generator
+from typing import Any, ClassVar, Optional, Iterable, Generator, Union
 from enum import Enum
+from copy import deepcopy
+from typing_extensions import Literal
 from pydantic import BaseModel
 from PyCompGeomAlgorithms.core import PyCGAObject, Point, BinTreeNode, BinTree, ThreadedBinTreeNode, ThreadedBinTree
 from PyCompGeomAlgorithms.dynamic_hull import DynamicHullNode, DynamicHullTree, SubhullNode, SubhullThreadedBinTree
 from PyCompGeomAlgorithms.graham import GrahamStepsTableRow, GrahamStepsTable
+from PyCompGeomAlgorithms.preparata import PreparataNode, PreparataThreadedBinTree
 from PyCompGeomAlgorithms.quickhull import QuickhullNode, QuickhullTree
 
 
 class PydanticAdapter(BaseModel):
     regular_class: ClassVar[type] = object
 
     @classmethod
@@ -52,17 +56,17 @@
     @cached_property
     def regular_object(self):
         return self.regular_class(*self.coords)
 
 
 class BinTreeNodePydanticAdapter(PydanticAdapter):
     regular_class: ClassVar[type] = BinTreeNode
-    data: Any
-    left: Optional[Any] = None
-    right: Optional[Any] = None
+    data: Any # WARNING: do not leave Any in derived classes, override with specifying that type! (Otherwise it might come out as underserialized portion of JSON when deserializing)
+    left: Optional[BinTreeNodePydanticAdapter] = None
+    right: Optional[BinTreeNodePydanticAdapter] = None
 
     @classmethod
     def from_regular_object(cls, obj: BinTreeNode, **kwargs):
         return cls(
             data=pycga_to_pydantic(obj.data),
             left=pycga_to_pydantic(obj.left),
             right=pycga_to_pydantic(obj.right),
@@ -94,18 +98,73 @@
     def from_regular_object(cls, obj: BinTree, **kwargs):
         return cls(root=pycga_to_pydantic(obj.root), **kwargs)
     
     def traverse_inorder(self):
         return self.root.traverse_inorder() if self.root else []
 
 
+def serialize_threaded_bin_tree_root_or_tree(root_or_tree: ThreadedBinTreeNodePydanticAdapter | ThreadedBinTreePydanticAdapter, *args, **kwargs):
+    """
+        Serializes both a threaded bin tree or its root.
+    """
+    copy = deepcopy(root_or_tree)
+    nodes_inorder = copy.traverse_inorder() if isinstance(copy, ThreadedBinTreeNodePydanticAdapter) else copy.root.traverse_inorder()
+    is_circular = nodes_inorder and nodes_inorder[0].prev is nodes_inorder[-1]
+
+    # Store node positions in inorder traversal instead of nodes to avoid infinite loops and be able to convert the tree to JSON
+    for i, node in enumerate(nodes_inorder):
+        node.prev = (i - 1) % len(nodes_inorder)
+        node.next = (i + 1) % len(nodes_inorder)
+    
+    if not is_circular and nodes_inorder:
+        nodes_inorder[0].prev = None
+        nodes_inorder[-1].next = None
+
+    return copy.model_dump(*args, **(kwargs | {'can_serialize': True}))
+
+
+def deserialize_threaded_bin_tree_root(root):
+    nodes_inorder = root.traverse_inorder()
+    is_circular = (
+        nodes_inorder
+        and nodes_inorder[0].prev is not None
+        and nodes_inorder[-1].next is not None
+        and (
+            (nodes_inorder[-1].next == 0)                     # if the object comes from JSON, this checks the node indices (see serialize_threaded_bin_tree_root)
+            if isinstance(nodes_inorder[0].prev, int)
+            else (nodes_inorder[0].prev is nodes_inorder[-1]) # if the object comes from Python objects, this checks the nodes 
+        )
+    )
+
+    for i, node in enumerate(nodes_inorder):
+        node.prev = nodes_inorder[i-1]
+        node.next = nodes_inorder[(i + 1) % len(nodes_inorder)]
+    
+    if not is_circular and nodes_inorder:
+        nodes_inorder[0].prev = None
+        nodes_inorder[-1].next = None
+
+
 class ThreadedBinTreeNodePydanticAdapter(BinTreeNodePydanticAdapter):
     regular_class: ClassVar[type] = ThreadedBinTreeNode
-    prev: Optional[Any] = None
-    next: Optional[Any] = None
+    left: Optional[ThreadedBinTreeNodePydanticAdapter] = None
+    right: Optional[ThreadedBinTreeNodePydanticAdapter] = None
+    prev: Optional[Union[ThreadedBinTreeNodePydanticAdapter, int]] = None
+    next: Optional[Union[ThreadedBinTreeNodePydanticAdapter, int]] = None
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        deserialize_threaded_bin_tree_root(self)  
+    
+    def model_dump(self, *args, **kwargs):
+        if kwargs.get('can_serialize', False):
+            kwargs.pop('can_serialize')
+            return super().model_dump(*args, **kwargs)
+        
+        return serialize_threaded_bin_tree_root_or_tree(self, *args, **kwargs)
 
     @cached_property
     def regular_object(self):
         return self.regular_class(
             self.data.regular_object if isinstance(self.data, PydanticAdapter) else self.data,
             self.left.regular_object if self.left else None,
             self.right.regular_object if self.right else None
@@ -116,14 +175,25 @@
         return super().from_regular_object(obj, prev=None, next=None, **kwargs)
         
 
 class ThreadedBinTreePydanticAdapter(BinTreePydanticAdapter):
     regular_class: ClassVar[type] = ThreadedBinTree
     root: ThreadedBinTreeNodePydanticAdapter
 
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        deserialize_threaded_bin_tree_root(self.root)
+
+    def model_dump(self, *args, **kwargs):
+        if kwargs.get('can_serialize', False):
+            kwargs.pop('can_serialize')
+            return super().model_dump(*args, **kwargs)
+        
+        return serialize_threaded_bin_tree_root_or_tree(self, *args, **kwargs)
+
     @classmethod
     def from_regular_object(cls, obj: ThreadedBinTree, **kwargs):
         root = obj.root
         is_circular = root.leftmost_node.prev is root.rightmost_node or root.rightmost_node.next is root.leftmost_node
         root = pycga_to_pydantic(obj.root)
         nodes = root.traverse_inorder()
 
@@ -164,28 +234,31 @@
 
 
 def pycga_to_pydantic(obj: Any | type | PyCGAObject | Iterable):
     if isinstance(obj, type):
         try:
             from .dynamic_hull import DynamicHullNodePydanticAdapter, DynamicHullTreePydanticAdapter, SubhullNodePydanticAdapter, SubhullThreadedBinTreePydanticAdapter
             from .graham import GrahamStepsTableRowPydanticAdapter, GrahamStepsTablePydanticAdapter
+            from .preparata import PreparataNodePydanticAdapter, PreparataThreadedBinTreePydanticAdapter
             from .quickhull import QuickhullNodePydanticAdapter, QuickhullTreePydanticAdapter
             
             return {
                 Point: PointPydanticAdapter,
                 BinTreeNode: BinTreeNodePydanticAdapter,
                 BinTree: BinTreePydanticAdapter,
                 ThreadedBinTreeNode: ThreadedBinTreeNodePydanticAdapter,
                 ThreadedBinTree: ThreadedBinTreePydanticAdapter,
                 DynamicHullNode: DynamicHullNodePydanticAdapter,
                 DynamicHullTree: DynamicHullTreePydanticAdapter,
                 SubhullNode: SubhullNodePydanticAdapter,
                 SubhullThreadedBinTree: SubhullThreadedBinTreePydanticAdapter,
                 GrahamStepsTableRow: GrahamStepsTableRowPydanticAdapter,
                 GrahamStepsTable: GrahamStepsTablePydanticAdapter,
+                PreparataNode: PreparataNodePydanticAdapter,
+                PreparataThreadedBinTree: PreparataThreadedBinTreePydanticAdapter,
                 QuickhullNode: QuickhullNodePydanticAdapter,
                 QuickhullTree: QuickhullTreePydanticAdapter,
             }[obj]
         except KeyError as e:
             raise KeyError("unknown PyCGA type") from e
 
     if isinstance(obj, PyCGAObject) and not isinstance(obj, Enum):
```

### Comparing `AlgoGrade-1.0.8/AlgoGrade/core.py` & `AlgoGrade-1.0.9/AlgoGrade/core.py`

 * *Files identical despite different names*

### Comparing `AlgoGrade-1.0.8/AlgoGrade/dynamic_hull.py` & `AlgoGrade-1.0.9/AlgoGrade/dynamic_hull.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from __future__ import annotations
 from functools import partial, cached_property
-from typing import ClassVar, Optional
+from typing import ClassVar, Optional, Union
 from PyCompGeomAlgorithms.core import BinTree, BinTreeNode, ThreadedBinTree, ThreadedBinTreeNode
 from PyCompGeomAlgorithms.dynamic_hull import upper_dynamic_hull, DynamicHullNode, DynamicHullTree, SubhullNode, SubhullThreadedBinTree, PathDirection
 from .adapters import pycga_to_pydantic, pydantic_to_pycga, PointPydanticAdapter, BinTreeNodePydanticAdapter, BinTreePydanticAdapter, ThreadedBinTreeNodePydanticAdapter, ThreadedBinTreePydanticAdapter
 from .core import Task, Grader, Answers, Mistake
 from .parsers import PointListAndTargetPointGivenJSONParser
 
 
@@ -66,14 +67,17 @@
             return []
         
         return cls.grade_bin_tree(answer, correct_answer, scorings, grade_item_method)
 
 
 class DynamicHullNodePydanticAdapter(BinTreeNodePydanticAdapter):
     regular_class: ClassVar[type] = DynamicHullNode
+    data: PointPydanticAdapter
+    left: Optional[DynamicHullNodePydanticAdapter] = None
+    right: Optional[DynamicHullNodePydanticAdapter] = None
     subhull_points: list[PointPydanticAdapter]
     optimized_subhull_points: Optional[list[PointPydanticAdapter]] = None
     left_supporting_index: int = 0
     left_supporting: PointPydanticAdapter
     right_supporting: PointPydanticAdapter
 
     @classmethod
@@ -96,14 +100,19 @@
     @classmethod
     def from_regular_object(cls, obj: DynamicHullTree, **kwargs):
         return super().from_regular_object(obj, **kwargs)
 
 
 class SubhullNodePydanticAdapter(ThreadedBinTreeNodePydanticAdapter):
     regular_class: ClassVar[type] = SubhullNode
+    data: PointPydanticAdapter
+    left: Optional[SubhullNodePydanticAdapter] = None
+    right: Optional[SubhullNodePydanticAdapter] = None
+    prev: Optional[Union[SubhullNodePydanticAdapter, int]] = None
+    next: Optional[Union[SubhullNodePydanticAdapter, int]] = None
 
     @classmethod
     def from_regular_object(cls, obj: SubhullNode, **kwargs):
         return super().from_regular_object(obj, **kwargs)
 
 
 class SubhullThreadedBinTreePydanticAdapter(ThreadedBinTreePydanticAdapter):
```

### Comparing `AlgoGrade-1.0.8/AlgoGrade/graham.py` & `AlgoGrade-1.0.9/AlgoGrade/graham.py`

 * *Files identical despite different names*

### Comparing `AlgoGrade-1.0.8/AlgoGrade/quickhull.py` & `AlgoGrade-1.0.9/AlgoGrade/quickhull.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from __future__ import annotations
 from functools import partial
-from typing import ClassVar, Optional
+from typing import ClassVar, Optional, Union
 from PyCompGeomAlgorithms.core import BinTree
 from PyCompGeomAlgorithms.quickhull import quickhull, QuickhullNode
 from .adapters import pycga_to_pydantic, PointPydanticAdapter, BinTreeNodePydanticAdapter, BinTreePydanticAdapter
 from .core import Task, Grader, Mistake, Answers
 from .parsers import PointListGivenJSONParser
 
 
@@ -21,14 +22,17 @@
     @classmethod
     def grade_finalization(cls, answer, correct_answer, scorings):
         return [Mistake(scorings) for node in answer.traverse_preorder() if not node.is_leaf and len(node.points) == 2]
 
 
 class QuickhullNodePydanticAdapter(BinTreeNodePydanticAdapter):
     regular_class: ClassVar[type] = QuickhullNode
+    data: list[PointPydanticAdapter]
+    left: Optional[QuickhullNodePydanticAdapter] = None
+    right: Optional[QuickhullNodePydanticAdapter] = None
     h: Optional[PointPydanticAdapter] = None
     subhull: Optional[list[PointPydanticAdapter]] = None
 
     @classmethod
     def from_regular_object(cls, obj: QuickhullNode, **kwargs):
         return super().from_regular_object(
             obj,
```

### Comparing `AlgoGrade-1.0.8/AlgoGrade.egg-info/PKG-INFO` & `AlgoGrade-1.0.9/AlgoGrade.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: AlgoGrade
-Version: 1.0.8
+Version: 1.0.9
 Summary: A library for automated grading of algorithmic tasks with grading of their intermediate stages. The grading of some computational geometry tasks are provided out of the box.
 Author: artandfi (Artem Fisunenko)
 Author-email: artyom.fisunenko@gmail.com
 Keywords: Python3,automated grading,computational geometry,convex hull,region search,geometric search,point location,proximity,closest pair,closest points
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
 Requires-Dist: annotated-types==0.5.0
 Requires-Dist: colorama==0.4.6
 Requires-Dist: exceptiongroup==1.1.1
 Requires-Dist: iniconfig==2.0.0
 Requires-Dist: packaging==23.1
 Requires-Dist: pluggy==1.2.0
-Requires-Dist: PyCompGeomAlgorithms==1.0.19
+Requires-Dist: PyCompGeomAlgorithms==1.0.20
 Requires-Dist: pydantic==2.0
 Requires-Dist: pydantic_core==2.0.1
 Requires-Dist: pyproject_hooks==1.0.0
 Requires-Dist: pytest==7.4.0
 Requires-Dist: tomli==2.0.1
 Requires-Dist: typing_extensions==4.8.0
```

### Comparing `AlgoGrade-1.0.8/AlgoGrade.egg-info/SOURCES.txt` & `AlgoGrade-1.0.9/AlgoGrade.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 AlgoGrade.egg-info/PKG-INFO
 AlgoGrade.egg-info/SOURCES.txt
 AlgoGrade.egg-info/dependency_links.txt
 AlgoGrade.egg-info/requires.txt
 AlgoGrade.egg-info/top_level.txt
 tests/__init__.py
 tests/adapters/__init__.py
-tests/adapters/test_core.py
+tests/adapters/test_basic_adapters.py
 tests/adapters/test_dynamic_hull.py
 tests/adapters/test_graham.py
 tests/adapters/test_interlibrary_converters.py
+tests/adapters/test_preparata.py
 tests/adapters/test_quickhull.py
 tests/answers/__init__.py
 tests/answers/test_dynamic_hull.py
 tests/answers/test_graham.py
 tests/answers/test_preparata.py
 tests/answers/test_quickhull.py
 tests/graders/__init__.py
```

### Comparing `AlgoGrade-1.0.8/LICENSE` & `AlgoGrade-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `AlgoGrade-1.0.8/PKG-INFO` & `AlgoGrade-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: AlgoGrade
-Version: 1.0.8
+Version: 1.0.9
 Summary: A library for automated grading of algorithmic tasks with grading of their intermediate stages. The grading of some computational geometry tasks are provided out of the box.
 Author: artandfi (Artem Fisunenko)
 Author-email: artyom.fisunenko@gmail.com
 Keywords: Python3,automated grading,computational geometry,convex hull,region search,geometric search,point location,proximity,closest pair,closest points
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
 Requires-Dist: annotated-types==0.5.0
 Requires-Dist: colorama==0.4.6
 Requires-Dist: exceptiongroup==1.1.1
 Requires-Dist: iniconfig==2.0.0
 Requires-Dist: packaging==23.1
 Requires-Dist: pluggy==1.2.0
-Requires-Dist: PyCompGeomAlgorithms==1.0.19
+Requires-Dist: PyCompGeomAlgorithms==1.0.20
 Requires-Dist: pydantic==2.0
 Requires-Dist: pydantic_core==2.0.1
 Requires-Dist: pyproject_hooks==1.0.0
 Requires-Dist: pytest==7.4.0
 Requires-Dist: tomli==2.0.1
 Requires-Dist: typing_extensions==4.8.0
```

### Comparing `AlgoGrade-1.0.8/setup.py` & `AlgoGrade-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="AlgoGrade",
-    version="1.0.8",
+    version="1.0.9",
     author="artandfi (Artem Fisunenko)",
     author_email="artyom.fisunenko@gmail.com",
     description="A library for automated grading of algorithmic tasks with grading of their intermediate stages. "
     "The grading of some computational geometry tasks are provided out of the box.",
     packages=find_packages(),
     install_requires=[line.strip() for line in open("requirements.txt", "r").readlines()],
     keywords=[
```

### Comparing `AlgoGrade-1.0.8/tests/adapters/test_graham.py` & `AlgoGrade-1.0.9/tests/adapters/test_graham.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,54 @@
+from pytest import fixture
 from PyCompGeomAlgorithms.core import Point
 from PyCompGeomAlgorithms.graham import GrahamStepsTableRow, GrahamStepsTable
 from AlgoGrade.adapters import PointPydanticAdapter
 from AlgoGrade.graham import GrahamStepsTableRowPydanticAdapter, GrahamStepsTablePydanticAdapter
 
 
-def test_steps_table_row_adapter():
-    adapter = GrahamStepsTableRowPydanticAdapter(
+@fixture
+def table_row_adapter():
+    return GrahamStepsTableRowPydanticAdapter(
         point_triple=(
             PointPydanticAdapter(coords=(1, 1)),
             PointPydanticAdapter(coords=(2, 2)),
             PointPydanticAdapter(coords=(3, 3))
         ),
         is_angle_less_than_pi=True
     )
-    regular_object = GrahamStepsTableRow((Point(1, 1), Point(2, 2), Point(3, 3)), True)
-
-    assert adapter.regular_object == regular_object
-    assert GrahamStepsTableRowPydanticAdapter.from_regular_object(regular_object) == adapter
 
 
-def test_steps_table_adapter():
-    adapter = GrahamStepsTablePydanticAdapter(
+@fixture
+def table_adapter(table_row_adapter):
+    return GrahamStepsTablePydanticAdapter(
         ordered_points=[PointPydanticAdapter(coords=(1, 1))],
-        rows=[
-            GrahamStepsTableRowPydanticAdapter(
-                point_triple=(
-                    PointPydanticAdapter(coords=(1, 1)),
-                    PointPydanticAdapter(coords=(2, 2)),
-                    PointPydanticAdapter(coords=(3, 3))
-                ),
-                is_angle_less_than_pi=True
-            )
-        ]
+        rows=[table_row_adapter]
     )
+
+
+def test_steps_table_row_adapter(table_row_adapter):
+    regular_object = GrahamStepsTableRow((Point(1, 1), Point(2, 2), Point(3, 3)), True)
+
+    assert table_row_adapter.regular_object == regular_object
+    assert GrahamStepsTableRowPydanticAdapter.from_regular_object(regular_object) == table_row_adapter
+
+
+def test_steps_table_row_adapter_serializaion(table_row_adapter):
+    serialized_row = table_row_adapter.model_dump()
+    deserialized_row = GrahamStepsTableRowPydanticAdapter(**serialized_row)
+    assert deserialized_row.regular_object == table_row_adapter.regular_object
+
+
+def test_steps_table_adapter(table_adapter):
     regular_object = GrahamStepsTable(
         [Point(1, 1)],
         [GrahamStepsTableRow((Point(1, 1), Point(2, 2), Point(3, 3)), True)]
     )
 
-    assert adapter.regular_object == regular_object
-    assert GrahamStepsTablePydanticAdapter.from_regular_object(regular_object) == adapter
+    assert table_adapter.regular_object == regular_object
+    assert GrahamStepsTablePydanticAdapter.from_regular_object(regular_object) == table_adapter
+
+
+def test_steps_table_adapter_serialization(table_adapter):
+    serialized_table = table_adapter.model_dump()
+    deserialized_table = GrahamStepsTablePydanticAdapter(**serialized_table)
+    assert deserialized_table.regular_object == table_adapter.regular_object
```

### Comparing `AlgoGrade-1.0.8/tests/adapters/test_interlibrary_converters.py` & `AlgoGrade-1.0.9/tests/adapters/test_interlibrary_converters.py`

 * *Files identical despite different names*

### Comparing `AlgoGrade-1.0.8/tests/answers/test_dynamic_hull.py` & `AlgoGrade-1.0.9/tests/answers/test_dynamic_hull.py`

 * *Files identical despite different names*

### Comparing `AlgoGrade-1.0.8/tests/answers/test_graham.py` & `AlgoGrade-1.0.9/tests/answers/test_graham.py`

 * *Files identical despite different names*

### Comparing `AlgoGrade-1.0.8/tests/answers/test_preparata.py` & `AlgoGrade-1.0.9/tests/answers/test_preparata.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from AlgoGrade.adapters import PointPydanticAdapter, ThreadedBinTreePydanticAdapter, ThreadedBinTreeNodePydanticAdapter, pydantic_to_pycga
-from AlgoGrade.preparata import PreparataAnswers
+from AlgoGrade.adapters import PointPydanticAdapter, pydantic_to_pycga
+from AlgoGrade.preparata import PreparataNodePydanticAdapter, PreparataThreadedBinTreePydanticAdapter, PreparataAnswers
 
 
 def test_preparata_answers():
     point = PointPydanticAdapter(coords=(1, 1))
     hull = [point]
-    tree = ThreadedBinTreePydanticAdapter(root=ThreadedBinTreeNodePydanticAdapter(data=point))
+    tree = PreparataThreadedBinTreePydanticAdapter(root=PreparataNodePydanticAdapter(data=point))
     left_paths, right_paths = [[point]], [[point]]
     deleted_points = []
     hulls, trees = [hull], [tree]
 
     answers_model = PreparataAnswers(
         hull=hull, tree=tree, left_paths=left_paths, right_paths=right_paths,
         deleted_points_lists=deleted_points, hulls=hulls, trees=trees
```

### Comparing `AlgoGrade-1.0.8/tests/answers/test_quickhull.py` & `AlgoGrade-1.0.9/tests/answers/test_quickhull.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from AlgoGrade.quickhull import QuickhullAnswers, QuickhullNodePydanticAdapter, QuickhullTreePydanticAdapter
 
 
 def test_quickhull_answers():
     point = PointPydanticAdapter(coords=(1, 1))
     leftmost_point, rightmost_point = point, point
     subset1, subset2 = [point], [point]
-    tree = QuickhullTreePydanticAdapter(root=QuickhullNodePydanticAdapter(data=point))
+    tree = QuickhullTreePydanticAdapter(root=QuickhullNodePydanticAdapter(data=[point]))
 
     answers_model = QuickhullAnswers(
         leftmost_point=leftmost_point, rightmost_point=rightmost_point,
         subset1=subset1, subset2=subset2, tree=tree
     )
     answers_list = [(leftmost_point, rightmost_point, subset1, subset2), tree, tree, tree, tree]
```

### Comparing `AlgoGrade-1.0.8/tests/graders/test_dynamic_hull.py` & `AlgoGrade-1.0.9/tests/graders/test_dynamic_hull.py`

 * *Files identical despite different names*

### Comparing `AlgoGrade-1.0.8/tests/graders/test_graham.py` & `AlgoGrade-1.0.9/tests/graders/test_graham.py`

 * *Files identical despite different names*

### Comparing `AlgoGrade-1.0.8/tests/graders/test_mock.py` & `AlgoGrade-1.0.9/tests/graders/test_mock.py`

 * *Files identical despite different names*

### Comparing `AlgoGrade-1.0.8/tests/graders/test_preparata.py` & `AlgoGrade-1.0.9/tests/graders/test_preparata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from math import isclose
 from copy import deepcopy
-from PyCompGeomAlgorithms.core import Point, ThreadedBinTree
+from PyCompGeomAlgorithms.core import Point
+from PyCompGeomAlgorithms.preparata import PreparataThreadedBinTree
 from AlgoGrade.preparata import PreparataGrader, PreparataTask, PreparataAnswers
 from AlgoGrade.adapters import pycga_to_pydantic
 from AlgoGrade.core import Scoring
 
 
 points = [Point(1, 1), Point(1, 5), Point(5, 3), Point(1, 11), Point(6, 1), Point(10, 1)]
 givens = (points,)
@@ -19,15 +20,15 @@
 correct_pydantic_answers = task_class.solve_as_pydantic_list(givens)
 correct_answers_wrapper = task_class.solve_as_answers_wrapper(givens)
 
 
 def test_preparata_all_correct():
     hull0 = [Point(1, 1), Point(1, 5), Point(5, 3)]
     hull = [Point(1, 1), Point(1, 11), Point(10, 1)]
-    tree0 = ThreadedBinTree.from_iterable(hull0)
+    tree0 = PreparataThreadedBinTree.from_iterable(hull0)
     left_paths = [
         [Point(1, 5), Point(5, 3)],
         [Point(1, 11), Point(5, 3), Point(1, 1)],
         [Point(1, 11), Point(6, 1), Point(1, 1)]
     ]
     right_paths = [
         [Point(1, 5), Point(1, 1)],
@@ -36,15 +37,15 @@
     ]
     deleted_points = [[Point(1, 5)], [Point(5, 3)], [Point(6, 1)]]
     hulls = [
         [Point(1, 1), Point(1, 11), Point(5, 3)],
         [Point(1, 1), Point(1, 11), Point(6, 1)],
         hull
     ]
-    trees = [ThreadedBinTree.from_iterable(hulls[0]), ThreadedBinTree.from_iterable(hulls[1])]
+    trees = [PreparataThreadedBinTree.from_iterable(hulls[0]), PreparataThreadedBinTree.from_iterable(hulls[1])]
 
     pycga_answers = [(hull0, tree0), (left_paths, right_paths), deleted_points, (hulls, trees)]
     pydantic_answers = pycga_to_pydantic(pycga_answers)
     answers_wrapper = PreparataAnswers.from_iterable(pydantic_answers)
 
     total_grade, answer_grades = PreparataGrader.grade_pycga(pycga_answers, correct_pycga_answers, scorings)
     assert isclose(total_grade, 1)
@@ -291,15 +292,15 @@
 
 
 def test_preparata_grader_incorrect_trees_repeated():
     pycga_answers = deepcopy(correct_pycga_answers)
     
     trees = pycga_answers[3][1]
     trees[0].root.data = Point(100, 100)
-    trees[0].root.left.data = None
+    trees[0].root.left.data = Point(-1, -1)
     trees[1].root.data = Point(100, 100)
 
     pydantic_answers = pycga_to_pydantic(pycga_answers)
     answers_wrapper = PreparataAnswers.from_iterable(pydantic_answers)
 
     total_grade, answer_grades = PreparataGrader.grade_pycga(pycga_answers, correct_pycga_answers, scorings)
     assert isclose(total_grade, -0.5)
@@ -316,15 +317,15 @@
     
     hulls = pycga_answers[3][0]
     hulls[0][0] = Point(100, 100)
     hulls[1][1] = Point(100, 100)
     
     trees = pycga_answers[3][1]
     trees[0].root.data = Point(100, 100)
-    trees[0].root.left.data = None
+    trees[0].root.left.data = Point(-1, -1)
     trees[1].root.data = Point(100, 100)
 
     pydantic_answers = pycga_to_pydantic(pycga_answers)
     answers_wrapper = PreparataAnswers.from_iterable(pydantic_answers)
 
     total_grade, answer_grades = PreparataGrader.grade_pycga(pycga_answers, correct_pycga_answers, scorings)
     assert isclose(total_grade, -0.5)
```

### Comparing `AlgoGrade-1.0.8/tests/graders/test_quickhull.py` & `AlgoGrade-1.0.9/tests/graders/test_quickhull.py`

 * *Files identical despite different names*

