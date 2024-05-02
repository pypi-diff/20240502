# Comparing `tmp/ofnodes-1.8.0.tar.gz` & `tmp/ofnodes-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofnodes-1.8.0.tar", max compression
+gzip compressed data, was "ofnodes-1.9.0.tar", max compression
```

## Comparing `ofnodes-1.8.0.tar` & `ofnodes-1.9.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-1.8.0/LICENSE
--rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-1.8.0/README.md
--rw-r--r--   0        0        0      590 2024-04-26 14:35:49.613667 ofnodes-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     1488 2024-04-25 04:48:44.846592 ofnodes-1.8.0/src/ofnodes/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 02:55:30.992047 ofnodes-1.8.0/src/ofnodes/components/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-1.8.0/src/ofnodes/components/nodes/__init__ copy.py
--rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-1.8.0/src/ofnodes/components/nodes/__init__.py
--rw-r--r--   0        0        0     2676 2024-04-23 17:49:14.794379 ofnodes-1.8.0/src/ofnodes/components/nodes/descriptors.py
--rw-r--r--   0        0        0      817 2024-04-23 19:26:45.294035 ofnodes-1.8.0/src/ofnodes/components/nodes/mixins.py
--rw-r--r--   0        0        0        0 2024-04-23 17:49:14.794379 ofnodes-1.8.0/src/ofnodes/components/structures/__init__.py
--rw-r--r--   0        0        0     9082 2024-04-23 17:49:14.794379 ofnodes-1.8.0/src/ofnodes/components/structures/descriptors.py
--rw-r--r--   0        0        0    20486 2024-04-26 14:35:49.613667 ofnodes-1.8.0/src/ofnodes/components/structures/mixins.py
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.8.0/src/ofnodes/nodes/__init__.py
--rw-r--r--   0        0        0     1520 2024-04-23 18:51:28.074288 ofnodes-1.8.0/src/ofnodes/nodes/singlynode.py
--rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.8.0/src/ofnodes/py.typed
--rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.8.0/src/ofnodes/structures/__init__.py
--rw-r--r--   0        0        0     2737 2024-04-26 14:35:49.613667 ofnodes-1.8.0/src/ofnodes/structures/singlylinkedlist.py
--rw-r--r--   0        0        0     2139 2024-04-26 14:35:49.613667 ofnodes-1.8.0/src/ofnodes/structures/stack.py
--rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 ofnodes-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 08:32:12.931610 ofnodes-1.9.0/LICENSE
+-rw-r--r--   0        0        0     2606 2024-04-05 21:55:30.417310 ofnodes-1.9.0/README.md
+-rw-r--r--   0        0        0      590 2024-04-30 21:31:53.616928 ofnodes-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1488 2024-04-25 04:48:44.846592 ofnodes-1.9.0/src/ofnodes/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 02:55:30.992047 ofnodes-1.9.0/src/ofnodes/components/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-1.9.0/src/ofnodes/components/nodes/__init__ copy.py
+-rw-r--r--   0        0        0        0 2024-04-23 18:51:28.074288 ofnodes-1.9.0/src/ofnodes/components/nodes/__init__.py
+-rw-r--r--   0        0        0     2676 2024-04-30 04:04:14.832970 ofnodes-1.9.0/src/ofnodes/components/nodes/descriptors.py
+-rw-r--r--   0        0        0      819 2024-04-30 18:38:02.940918 ofnodes-1.9.0/src/ofnodes/components/nodes/mixins.py
+-rw-r--r--   0        0        0        0 2024-04-23 17:49:14.794379 ofnodes-1.9.0/src/ofnodes/components/structures/__init__.py
+-rw-r--r--   0        0        0     9082 2024-04-23 17:49:14.794379 ofnodes-1.9.0/src/ofnodes/components/structures/descriptors.py
+-rw-r--r--   0        0        0    20486 2024-04-26 16:35:49.237665 ofnodes-1.9.0/src/ofnodes/components/structures/mixins.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.9.0/src/ofnodes/nodes/__init__.py
+-rw-r--r--   0        0        0     1520 2024-04-26 16:35:56.197622 ofnodes-1.9.0/src/ofnodes/nodes/singlynode.py
+-rw-r--r--   0        0        0        0 2024-03-26 21:30:39.653576 ofnodes-1.9.0/src/ofnodes/py.typed
+-rw-r--r--   0        0        0        0 2024-04-30 21:34:11.068241 ofnodes-1.9.0/src/ofnodes/sorting/__init__.py
+-rw-r--r--   0        0        0     3449 2024-04-30 21:41:45.001882 ofnodes-1.9.0/src/ofnodes/sorting/mixins.py
+-rw-r--r--   0        0        0        0 2024-04-04 17:47:49.284523 ofnodes-1.9.0/src/ofnodes/structures/__init__.py
+-rw-r--r--   0        0        0     2842 2024-04-30 21:42:46.537555 ofnodes-1.9.0/src/ofnodes/structures/singlylinkedlist.py
+-rw-r--r--   0        0        0     2139 2024-04-26 14:35:49.613667 ofnodes-1.9.0/src/ofnodes/structures/stack.py
+-rw-r--r--   0        0        0     3013 1970-01-01 00:00:00.000000 ofnodes-1.9.0/PKG-INFO
```

### Comparing `ofnodes-1.8.0/LICENSE` & `ofnodes-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ofnodes-1.8.0/README.md` & `ofnodes-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ofnodes-1.8.0/pyproject.toml` & `ofnodes-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofnodes"
-version = "1.8.0"
+version = "1.9.0"
 description = "A library of Data Structures and Algorithms written in Python"
 authors = ["Robert Portelli <github@robertportelli.com>"]
 readme = "README.md"
 packages = [{include = "ofnodes", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `ofnodes-1.8.0/src/ofnodes/__init__.py` & `ofnodes-1.9.0/src/ofnodes/__init__.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.8.0/src/ofnodes/components/nodes/descriptors.py` & `ofnodes-1.9.0/src/ofnodes/components/nodes/descriptors.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.8.0/src/ofnodes/components/nodes/mixins.py` & `ofnodes-1.9.0/src/ofnodes/components/nodes/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,10 +18,10 @@
             None
 
         Examples:  TODO
 
         """
         if other:
             validated_data = other  # TODO: validate data
-            self.data = self.data + validated_data
+            self._data = self._data + validated_data
             return
         raise ValueError("Invalid data to add to SinglyNode.data")
```

### Comparing `ofnodes-1.8.0/src/ofnodes/components/structures/descriptors.py` & `ofnodes-1.9.0/src/ofnodes/components/structures/descriptors.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.8.0/src/ofnodes/components/structures/mixins.py` & `ofnodes-1.9.0/src/ofnodes/components/structures/mixins.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.8.0/src/ofnodes/nodes/singlynode.py` & `ofnodes-1.9.0/src/ofnodes/nodes/singlynode.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.8.0/src/ofnodes/structures/singlylinkedlist.py` & `ofnodes-1.9.0/src/ofnodes/structures/singlylinkedlist.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional, Any
 
 from ofnodes.nodes.singlynode import SinglyNode
 from ofnodes.components.structures.descriptors import Head, Tail, Target
 from ofnodes.components.structures.mixins import SearchMixin, RemoveMixin, InsertHeadMixin, InsertTailMixin, InsertAfterTargetMixin, InsertBeforeTargetMixin, PrintMixin
+from ofnodes.sorting.mixins import BubbleSortMixin, ReverseOrderMixin
 
-class SinglyLinkedList(SearchMixin, RemoveMixin, InsertHeadMixin, InsertTailMixin, InsertAfterTargetMixin, InsertBeforeTargetMixin, PrintMixin):
+class SinglyLinkedList(SearchMixin, RemoveMixin, InsertHeadMixin, InsertTailMixin, InsertAfterTargetMixin, InsertBeforeTargetMixin, PrintMixin, BubbleSortMixin, ReverseOrderMixin):
     """A class representing a singly linked list.
 
     This class provides functionality to create and manipulate a singly linked list
     data structure. Each node in the linked list contains a reference to the next
     node in the sequence.
 
     Attributes:
@@ -67,8 +68,8 @@
 
     def __dir__(self) -> list[str]:
         # Get the list of attributes and methods from the parent classes
         parent_dir = set(super().__dir__())
         # Filter out private attributes and methods
         parent_dir = {attr for attr in parent_dir if attr not in {'_head', '_tail', '_target'}}
         # Return a sorted list of all attributes and methods
-        return sorted(parent_dir)
+        return sorted(parent_dir)
```

### Comparing `ofnodes-1.8.0/src/ofnodes/structures/stack.py` & `ofnodes-1.9.0/src/ofnodes/structures/stack.py`

 * *Files identical despite different names*

### Comparing `ofnodes-1.8.0/PKG-INFO` & `ofnodes-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofnodes
-Version: 1.8.0
+Version: 1.9.0
 Summary: A library of Data Structures and Algorithms written in Python
 Author: Robert Portelli
 Author-email: github@robertportelli.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

