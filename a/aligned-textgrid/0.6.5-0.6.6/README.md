# Comparing `tmp/aligned_textgrid-0.6.5.tar.gz` & `tmp/aligned_textgrid-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aligned_textgrid-0.6.5.tar", max compression
+gzip compressed data, was "aligned_textgrid-0.6.6.tar", max compression
```

## Comparing `aligned_textgrid-0.6.5.tar` & `aligned_textgrid-0.6.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2023-02-14 13:52:58.923117 aligned_textgrid-0.6.5/LICENSE
--rw-r--r--   0        0        0     5072 2024-02-21 15:37:23.947449 aligned_textgrid-0.6.5/README.md
--rw-r--r--   0        0        0     1225 2024-04-06 21:18:00.270105 aligned_textgrid-0.6.5/pyproject.toml
--rw-r--r--   0        0        0      707 2024-02-21 15:37:23.962773 aligned_textgrid-0.6.5/src/aligned_textgrid/__init__.py
--rw-r--r--   0        0        0    17084 2024-04-06 21:10:14.820768 aligned_textgrid-0.6.5/src/aligned_textgrid/aligned_textgrid.py
--rw-r--r--   0        0        0     5194 2024-02-21 15:37:23.963303 aligned_textgrid-0.6.5/src/aligned_textgrid/custom_classes.py
--rw-r--r--   0        0        0        0 2024-02-21 15:37:23.963335 aligned_textgrid-0.6.5/src/aligned_textgrid/mixins/__init__.py
--rw-r--r--   0        0        0     5833 2024-02-21 15:37:23.963622 aligned_textgrid-0.6.5/src/aligned_textgrid/mixins/mixins.py
--rw-r--r--   0        0        0     4727 2024-02-21 15:37:23.963912 aligned_textgrid-0.6.5/src/aligned_textgrid/mixins/tiermixins.py
--rw-r--r--   0        0        0     1367 2024-02-21 15:37:23.964010 aligned_textgrid-0.6.5/src/aligned_textgrid/mixins/within.py
--rw-r--r--   0        0        0        0 2024-02-21 15:37:23.964048 aligned_textgrid-0.6.5/src/aligned_textgrid/outputs/__init__.py
--rw-r--r--   0        0        0     3927 2024-02-21 15:37:23.964350 aligned_textgrid-0.6.5/src/aligned_textgrid/outputs/to_dataframe.py
--rw-r--r--   0        0        0        0 2024-02-21 15:37:23.964386 aligned_textgrid-0.6.5/src/aligned_textgrid/points/__init__.py
--rw-r--r--   0        0        0     4986 2024-04-06 21:09:59.872257 aligned_textgrid-0.6.5/src/aligned_textgrid/points/points.py
--rw-r--r--   0        0        0     6521 2024-04-06 21:09:59.873124 aligned_textgrid-0.6.5/src/aligned_textgrid/points/tiers.py
--rw-r--r--   0        0        0        0 2024-02-21 15:37:23.965007 aligned_textgrid-0.6.5/src/aligned_textgrid/polar/__init__.py
--rw-r--r--   0        0        0     5280 2024-02-21 15:37:23.965238 aligned_textgrid-0.6.5/src/aligned_textgrid/polar/polar_classes.py
--rw-r--r--   0        0        0     1544 2024-02-21 15:37:23.965376 aligned_textgrid-0.6.5/src/aligned_textgrid/polar/polar_grid.py
--rw-r--r--   0        0        0        0 2023-11-16 18:05:47.275381 aligned_textgrid-0.6.5/src/aligned_textgrid/sequences/__init__.py
--rw-r--r--   0        0        0    18666 2024-04-06 21:09:59.874411 aligned_textgrid-0.6.5/src/aligned_textgrid/sequences/sequences.py
--rw-r--r--   0        0        0    10613 2024-04-06 21:09:59.875723 aligned_textgrid-0.6.5/src/aligned_textgrid/sequences/tiers.py
--rw-r--r--   0        0        0     2338 2024-02-21 15:37:23.966335 aligned_textgrid-0.6.5/src/aligned_textgrid/sequences/word_and_phone.py
--rw-r--r--   0        0        0     6183 1970-01-01 00:00:00.000000 aligned_textgrid-0.6.5/setup.py
--rw-r--r--   0        0        0     5887 1970-01-01 00:00:00.000000 aligned_textgrid-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-14 13:52:58.923117 aligned_textgrid-0.6.6/LICENSE
+-rw-r--r--   0        0        0     5072 2024-02-21 15:37:23.947449 aligned_textgrid-0.6.6/README.md
+-rw-r--r--   0        0        0     1225 2024-05-02 20:50:40.342058 aligned_textgrid-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0      707 2024-02-21 15:37:23.962773 aligned_textgrid-0.6.6/src/aligned_textgrid/__init__.py
+-rw-r--r--   0        0        0    19097 2024-05-02 20:50:40.342270 aligned_textgrid-0.6.6/src/aligned_textgrid/aligned_textgrid.py
+-rw-r--r--   0        0        0     7737 2024-05-02 20:50:40.342475 aligned_textgrid-0.6.6/src/aligned_textgrid/custom_classes.py
+-rw-r--r--   0        0        0        0 2024-02-21 15:37:23.963335 aligned_textgrid-0.6.6/src/aligned_textgrid/mixins/__init__.py
+-rw-r--r--   0        0        0     5833 2024-02-21 15:37:23.963622 aligned_textgrid-0.6.6/src/aligned_textgrid/mixins/mixins.py
+-rw-r--r--   0        0        0     4727 2024-02-21 15:37:23.963912 aligned_textgrid-0.6.6/src/aligned_textgrid/mixins/tiermixins.py
+-rw-r--r--   0        0        0     1367 2024-02-21 15:37:23.964010 aligned_textgrid-0.6.6/src/aligned_textgrid/mixins/within.py
+-rw-r--r--   0        0        0        0 2024-02-21 15:37:23.964048 aligned_textgrid-0.6.6/src/aligned_textgrid/outputs/__init__.py
+-rw-r--r--   0        0        0     3927 2024-02-21 15:37:23.964350 aligned_textgrid-0.6.6/src/aligned_textgrid/outputs/to_dataframe.py
+-rw-r--r--   0        0        0        0 2024-02-21 15:37:23.964386 aligned_textgrid-0.6.6/src/aligned_textgrid/points/__init__.py
+-rw-r--r--   0        0        0     4986 2024-05-01 15:08:09.567233 aligned_textgrid-0.6.6/src/aligned_textgrid/points/points.py
+-rw-r--r--   0        0        0     6521 2024-04-06 21:09:59.873124 aligned_textgrid-0.6.6/src/aligned_textgrid/points/tiers.py
+-rw-r--r--   0        0        0        0 2024-02-21 15:37:23.965007 aligned_textgrid-0.6.6/src/aligned_textgrid/polar/__init__.py
+-rw-r--r--   0        0        0     5280 2024-02-21 15:37:23.965238 aligned_textgrid-0.6.6/src/aligned_textgrid/polar/polar_classes.py
+-rw-r--r--   0        0        0     1544 2024-02-21 15:37:23.965376 aligned_textgrid-0.6.6/src/aligned_textgrid/polar/polar_grid.py
+-rw-r--r--   0        0        0        0 2023-11-16 18:05:47.275381 aligned_textgrid-0.6.6/src/aligned_textgrid/sequences/__init__.py
+-rw-r--r--   0        0        0    18666 2024-04-06 21:09:59.874411 aligned_textgrid-0.6.6/src/aligned_textgrid/sequences/sequences.py
+-rw-r--r--   0        0        0    10613 2024-04-06 21:09:59.875723 aligned_textgrid-0.6.6/src/aligned_textgrid/sequences/tiers.py
+-rw-r--r--   0        0        0     2338 2024-02-21 15:37:23.966335 aligned_textgrid-0.6.6/src/aligned_textgrid/sequences/word_and_phone.py
+-rw-r--r--   0        0        0     6183 1970-01-01 00:00:00.000000 aligned_textgrid-0.6.6/setup.py
+-rw-r--r--   0        0        0     5887 1970-01-01 00:00:00.000000 aligned_textgrid-0.6.6/PKG-INFO
```

### Comparing `aligned_textgrid-0.6.5/LICENSE` & `aligned_textgrid-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.5/README.md` & `aligned_textgrid-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.5/pyproject.toml` & `aligned_textgrid-0.6.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aligned_textgrid"
-version = "0.6.5"
+version = "0.6.6"
 description = "Classes for defining sequential information from TextGrids"
 authors = ["JoFrhwld <JoFrhwld@gmail.com>", "chrisbrickhouse <brickhouse@stanford.edu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [{include = "aligned_textgrid", from="src"}]
 exclude = [
     "notebooks/",
```

### Comparing `aligned_textgrid-0.6.5/src/aligned_textgrid/__init__.py` & `aligned_textgrid-0.6.6/src/aligned_textgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.5/src/aligned_textgrid/aligned_textgrid.py` & `aligned_textgrid-0.6.6/src/aligned_textgrid/aligned_textgrid.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from praatio.data_classes.textgrid import Textgrid
 from praatio.textgrid import openTextgrid
 from aligned_textgrid.sequences.sequences import SequenceInterval, Top, Bottom
 from aligned_textgrid.points.points import SequencePoint
 from aligned_textgrid.sequences.tiers import SequenceTier, TierGroup
 from aligned_textgrid.points.tiers import SequencePointTier, PointsGroup
 from aligned_textgrid.mixins.within import WithinMixins
-from aligned_textgrid.custom_classes import custom_classes
+from aligned_textgrid.custom_classes import custom_classes, clone_class, get_class_hierarchy
 from typing import Type, Sequence, Literal
 from copy import copy
 import numpy as np
 import warnings
 
 
 class AlignedTextGrid(WithinMixins):
@@ -56,23 +56,23 @@
         textgrid: Textgrid = None,
         textgrid_path: str =  None,
         entry_classes: 
             Sequence[Sequence[Type[SequenceInterval]]] |
             Sequence[Type[SequenceInterval]]
               = [SequenceInterval]
     ):
-        self.entry_classes = entry_classes
+        self.entry_classes = self._reclone_classes(entry_classes)
         if textgrid:
-            self.tg_tiers, self.entry_classes = self._nestify_tiers(textgrid, entry_classes)
+            self.tg_tiers, self.entry_classes = self._nestify_tiers(textgrid, self.entry_classes)
         elif textgrid_path:
             tg = openTextgrid(
                 fnFullPath=textgrid_path, 
                 includeEmptyIntervals=True
             )
-            self.tg_tiers, self.entry_classes = self._nestify_tiers(tg, entry_classes)
+            self.tg_tiers, self.entry_classes = self._nestify_tiers(tg, self.entry_classes)
         else:
             warnings.warn('Initializing an empty AlignedTextGrid')
             self._init_empty()
             return
 
         self.tier_groups = self._relate_tiers()
         self.contains = self.tier_groups
@@ -163,24 +163,77 @@
             try:
                 top_idxes = [i for i,c in enumerate(class_supers) if issubclass(c, Top)]
             except ValueError:
                 top_idxes = []
 
         if type(entry_classes[0]) in [list, tuple]:
             return entry_classes
+        
         if len(entry_classes) == 1:
             extension = len(tg.tiers) // len(entry_classes)
             entry_classes = [entry_classes] * extension
             return entry_classes
         if len(top_idxes) <= 1:
             extension = len(tg.tiers) // len(entry_classes)
             entry_classes = [entry_classes] * extension
             return entry_classes
+        
         return entry_classes
 
+    def _reclone_classes(
+            self, 
+            entry_classes:list[SequenceInterval|SequencePoint]|list[list[SequenceInterval|SequencePoint]]
+            ) -> list[SequenceInterval|SequencePoint]|list[list[SequenceInterval|SequencePoint]]:
+        
+        flat_classes = entry_classes
+        if type(entry_classes[0]) is list:
+            flat_classes = [c for tg in entry_classes for c in tg]
+        
+        unique_classes = list(set(flat_classes))
+
+        points = [c for c in unique_classes if issubclass(c, SequencePoint)]
+        tops = [
+            c 
+            for c in unique_classes 
+            if issubclass(c, SequenceInterval)
+            if issubclass(c.superset_class, Top)
+        ]
+
+        points_clone = [clone_class(p) for p  in points]
+        tops_clone = [clone_class(t) for t in tops]
+        full_seq_clone = []
+        for tclone in tops_clone:
+            full_seq_clone += get_class_hierarchy(tclone, [])
+
+        full_clone = points_clone + full_seq_clone
+
+        if type(entry_classes[0]) is list:
+            new_entry_classes = [
+                self._swap_classes(tg_classes, full_clone)
+                for tg_classes in entry_classes
+            ]
+        else:
+            new_entry_classes = self._swap_classes(entry_classes, full_clone)
+
+        return new_entry_classes
+
+    def _swap_classes(
+            self, 
+            orig_classes: list[SequenceInterval]|list[SequencePoint], 
+            new_classes: list[SequenceInterval,SequencePoint]
+        )->list[SequenceInterval]|list[SequencePoint]:
+        new_classes_names = [c.__name__ for c in new_classes]
+        orig_classes_names = [c.__name__ for c in orig_classes]
+
+        new_idx = [new_classes_names.index(on) for on in orig_classes_names]
+
+        out_classes = [new_classes[i] for i in new_idx]
+        return out_classes
+
+
     def _init_empty(self):
         self.tier_groups = []
         self.contains = self.tier_groups
         self.entry_classes = []
         self.tg_tiers = None
     
     def _nestify_tiers(
@@ -326,26 +379,28 @@
         if not (above or below):
             raise ValueError("Either above or below must be specified")
         if not name:
             raise ValueError("name must be specified")
         
         new_class = custom_classes([name])[0]
 
-        if type(above) is str:
-            above = self.get_class_by_name(above)
-
-        if type(below) is str:
-            below = self.get_class_by_name(below)
+        if type(above) is type:
+            above = above.__name__
+        
+        if type(below) is type:
+            below = below.__name__
 
         if above:
+            above = self.get_class_by_name(above)
             up_class = copy(above.superset_class)
             down_class = above
             specified_class = above
 
         if below:
+            below = self.get_class_by_name(below)
             up_class = below
             down_class = copy(below.subset_class)
             specified_class = below
 
         if timing_from == "below":
             copy_class = down_class
         elif timing_from == "above":
```

### Comparing `aligned_textgrid-0.6.5/src/aligned_textgrid/custom_classes.py` & `aligned_textgrid-0.6.6/src/aligned_textgrid/custom_classes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,43 @@
 from aligned_textgrid.sequences.sequences import *
 from aligned_textgrid.points.points import *
 from praatio.utilities.utils import Interval
 from typing import Type
 
+
+
+def _top_constructor(self):
+    Top.__init__(self)
+
+def _bottom_constructor(self):
+    Bottom.__init__(self)
+
+def _make_top()->SequenceInterval:
+
+    n_top = len(Top.__subclasses__())
+    this_top_name = f"Top_{n_top}"
+    this_top = type(
+        this_top_name,
+        (Top, ), 
+        {"__init__": _top_constructor}
+    )
+
+    return this_top
+
+def _make_bottom()->SequenceInterval:
+    n_bottom = len(Bottom.__subclasses__())
+    this_bottom_name = f"Bottom_{n_bottom}"
+    this_bottom = type(
+        this_bottom_name, 
+        (Bottom, ), 
+        {"__init__": _bottom_constructor}
+    )
+
+    return this_bottom
+
 def custom_classes(
         class_list:list[str] = [],
         return_order: list[str] | list[int] | None = None,
         points:list[int] = []        
 ) -> list[Type[SequenceInterval]]:
     """Generate custom interval classes
 
@@ -60,82 +91,49 @@
             A return order for the custom classes, if not in hierarchical order. Defaults to None.
         points (list[int], optional): 
             Indices of which classes should be points, rather than intervals
 
     Returns:
         (list[Type[SequenceInterval]]): A list of custom `SequenceInterval` subclasses
     """
-    def _sequence_constructor(
-            self, 
-            Interval = Interval(None, None, None)
-        ):
-        SequenceInterval.__init__(self, Interval=Interval)
-    
-    def _point_constructor(
-            self,
-            Point = Point(0, "")
-    ):
-        SequencePoint.__init__(self, Point)
-
-    def _top_constructor(self):
-        Top.__init__(self)
-
-    def _bottom_constructor(self):
-        Bottom.__init__(self)
-
-
-    n_top = len(Top.__subclasses__())
-    n_bottom = len(Bottom.__subclasses__())
-
-    this_top_name = f"Top_{n_top}"
-    this_bottom_name = f"Bottom_{n_bottom}"
 
-    this_top = type(
-        this_top_name,
-        (Top, ), 
-        {"__init__": _top_constructor}
-    )
-    
-    this_bottom = type(
-        this_bottom_name, 
-        (Bottom, ), 
-        {"__init__": _bottom_constructor}
-    )
+    this_top = _make_top()
+    this_bottom = _make_bottom()
 
     if return_order is None:
         return_order = class_list
 
     class_out_list = []
     if type(class_list) is str and len(points) == 0:
         newclass = type(
             class_list, 
             (SequenceInterval, ), 
-            {"__init__": _sequence_constructor}
+            dict(SequenceInterval.__dict__)
         )
         newclass.set_superset_class(this_top)
         newclass.set_subset_class(this_bottom)
         return newclass
     
     if type(class_list) is str and len(points) != 0:
         newclass = type(
             class_list, 
             (SequencePoint, ), 
-            {"__init__": _point_constructor}
+            dict(SequencePoint.__dict__)
         )
         return newclass
 
     if type(class_list) is list:
         for idx, name in enumerate(class_list):
             if idx in points:
                 class_out_list.append(
-                    type(name, (SequencePoint,), {"__init__": _point_constructor})
+                    type(name, (SequencePoint,), dict(SequencePoint.__dict__))
                 )
             else:
                 class_out_list.append(
-                    type(name, (SequenceInterval,), {"__init__": _sequence_constructor})
+                    type(name, (SequenceInterval,), dict(SequenceInterval.__dict__))
                 )
                 
         interval_classes = [x 
                             for x in class_out_list 
                             if issubclass(x, SequenceInterval)
                             ]
         for idx, entry in enumerate(interval_classes):
@@ -147,8 +145,94 @@
                 entry.set_subset_class(interval_classes[idx+1])
 
         if type(return_order[0]) is int:
             return_list = [class_out_list[idx] for idx in return_order]
         elif type(return_order[0]) is str:
             return_idx = [return_order.index(x) for x in class_list]
             return_list = [class_out_list[idx] for idx in return_idx] 
-        return return_list
+        return return_list
+
+def clone_class(
+        entry_class:SequenceInterval|SequencePoint,
+        recurse = False
+        ) -> SequenceInterval|SequencePoint:
+    """Clone an entry class. It will have the same name, but
+    any changes to its class properties will not be reflected
+    in the original class.
+
+    Args:
+        entry_class (SequenceInterval | SequencePoint): 
+            A SequenceInterval or SequencePoint to clone
+        ti
+        recurse (bool, optional): 
+            Used internally to clone the entire hierarchy. 
+            Defaults to False.
+
+    Returns:
+        (SequenceInterval|SequencePoint): A cloned entry class
+    """
+    
+    if issubclass(entry_class, SequenceInterval):
+        if not issubclass(entry_class.superset_class, Top) \
+        and not recurse:
+            raise Exception("Entry class to clone must be top of hierarchy")
+        
+        cloned = type(
+                entry_class.__name__, 
+                (entry_class, ), 
+                dict(entry_class.__dict__)
+            )
+        
+        if issubclass(cloned.superset_class, Top):
+            cloned.set_superset_class(
+                _make_top()
+            )
+
+        if issubclass(cloned.subset_class, Bottom):
+            cloned.set_subset_class(
+                _make_bottom()
+            )
+
+        if (not cloned is cloned.subset_class.superset_class) \
+           and issubclass(cloned.subset_class, SequenceInterval):
+            new_subset = clone_class(cloned.subset_class, recurse=True)
+            cloned.set_subset_class(new_subset)
+
+           
+    if issubclass(entry_class, SequencePoint):
+        cloned = type(
+                entry_class.__name__, 
+                (entry_class, ), 
+                dict(entry_class.__dict__)
+        )
+    
+    return cloned
+
+def get_class_hierarchy(
+        entry_class:SequenceInterval, 
+        out_list = []
+    )->list[SequenceInterval]:
+    """Given a SequenceInterval, this will return
+    the entire class hierarchy
+
+    Args:
+        entry_class (SequenceInterval): 
+            Entry class to search the hierarchy for
+        out_list (list, optional): 
+            Used internally for recursive search.
+            Defaults to [].
+
+    Returns:
+        (list[SequenceInterval]):
+            The class hierarchy
+    """
+    if (not issubclass(entry_class.superset_class, Top)) \
+       and entry_class.superset_class not in out_list:
+        out_list = get_class_hierarchy(entry_class.superset_class, out_list)
+
+    if entry_class not in out_list: 
+        out_list.append(entry_class)
+
+    if not issubclass(entry_class.subset_class, Bottom):
+        out_list = get_class_hierarchy(entry_class.subset_class, out_list)
+    
+    return out_list
```

### Comparing `aligned_textgrid-0.6.5/src/aligned_textgrid/mixins/mixins.py` & `aligned_textgrid-0.6.6/src/aligned_textgrid/mixins/mixins.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.5/src/aligned_textgrid/mixins/tiermixins.py` & `aligned_textgrid-0.6.6/src/aligned_textgrid/mixins/tiermixins.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.5/src/aligned_textgrid/mixins/within.py` & `aligned_textgrid-0.6.6/src/aligned_textgrid/mixins/within.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.5/src/aligned_textgrid/outputs/to_dataframe.py` & `aligned_textgrid-0.6.6/src/aligned_textgrid/outputs/to_dataframe.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.5/src/aligned_textgrid/points/points.py` & `aligned_textgrid-0.6.6/src/aligned_textgrid/points/points.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.5/src/aligned_textgrid/points/tiers.py` & `aligned_textgrid-0.6.6/src/aligned_textgrid/points/tiers.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.5/src/aligned_textgrid/polar/polar_classes.py` & `aligned_textgrid-0.6.6/src/aligned_textgrid/polar/polar_classes.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.5/src/aligned_textgrid/polar/polar_grid.py` & `aligned_textgrid-0.6.6/src/aligned_textgrid/polar/polar_grid.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.5/src/aligned_textgrid/sequences/sequences.py` & `aligned_textgrid-0.6.6/src/aligned_textgrid/sequences/sequences.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.5/src/aligned_textgrid/sequences/tiers.py` & `aligned_textgrid-0.6.6/src/aligned_textgrid/sequences/tiers.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.5/src/aligned_textgrid/sequences/word_and_phone.py` & `aligned_textgrid-0.6.6/src/aligned_textgrid/sequences/word_and_phone.py`

 * *Files identical despite different names*

### Comparing `aligned_textgrid-0.6.5/setup.py` & `aligned_textgrid-0.6.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.24.2,<2.0.0', 'polars>=0.20.18,<0.21.0', 'praatio>=6.0.0,<7.0.0']
 
 setup_kwargs = {
     'name': 'aligned-textgrid',
-    'version': '0.6.5',
+    'version': '0.6.6',
     'description': 'Classes for defining sequential information from TextGrids',
     'long_description': "# Aligned TextGrid\n\n![PyPI](https://img.shields.io/pypi/v/aligned-textgrid.png)\n![lint_and_test](https://github.com/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid/actions/workflows/test_and_run.yml/badge.svg?event=pull_request&branch=main)\n[![codecov](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid/branch/dev/graph/badge.svg?token=27YSOQ5ZEL)](https://codecov.io/gh/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid)\n[![Maintainability](https://api.codeclimate.com/v1/badges/2387cd247bd8f1211323/maintainability.png)](https://codeclimate.com/github/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid/maintainability)\n[![Build\nDocs](https://github.com/Forced-Alignment-and-Vowel-Extraction/alignedTextGrid/actions/workflows/build-docs.yml/badge.svg)](https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/)\n[![DOI](https://zenodo.org/badge/552633207.svg)](https://zenodo.org/badge/latestdoi/552633207)\n\nThe aligned-textgrid package provides a python interface for\nrepresenting and operating on TextGrids produced by forced aligners like\n[FAVE](https://github.com/JoFrhwld/FAVE) or the [Montreal Forced\nAligner](https://montreal-forced-aligner.readthedocs.io/en/latest/).\nClasses provided by aligned-textgrid represent hierarchical and\nprecedence relationships among data stored in TextGrid formats allowing\nfor simplified and more accessible analysis of aligned speech data.\n\n## Example Use Cases\n\n- You want to quickly loop through the Phone tier of a Textgrid, and\n  *also* access information about the word it is a part of.\n- You want to quickly loop over the Word tier of a Textgrid and quickly\n  count how many phones it has.\n- You want to programmatically merge together adjacent Textgrid\n  intervals.\n\nFor examples on how to use the pacakge, see the [Usage](https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/usage) pages.\n\n## Installation\n\n<!-- TODO: documnet other package managers like conda -CB 14 March 2023 -->\n\nTo install aligned-textgrid using pip, run the following command in your\nterminal:\n\n``` bash\npip install aligned-textgrid\n```\n\n## Not another TextGrid implementation\n\nThere are several other packages that parse Praat Textgrids, including\n\n- [praatio](http://timmahrt.github.io/praatIO/praatio.html)\n- [textgrid](https://github.com/kylebgorman/textgrid)\n\n`aligned-textgrid`’s goal is to capture hierarchical and sequential\nrelationships represented in many TextGrids, and to make them easilly\naccessible to users via an intuitive interface. The goal is that from\nany arbitrary location within a TextGrid, users can easilly access\ninformation with minimally defensive coding.\n\n![](doc_src/usage/resources/diagrams/hierarchy_precedence.svg)\n\n### Example\n\nAs an example, we’ll read in a textgrid produced with forced alignment\nthat contains a single speaker with a word and phone tier.\n\n``` python\nfrom aligned_textgrid import AlignedTextGrid, Word, Phone\ntg = AlignedTextGrid(\n    textgrid_path='doc_src/usage/resources/josef-fruehwald_speaker.TextGrid', \n    entry_classes=[Word, Phone]\n    )\n```\n\nThen, we can access an arbitrary phone interval.\n\n``` python\narbitrary_interval = tg[0].Phone[20]\n```\n\nFrom this aribitrary interval, we can access information about the\nintervals preceding and following with the `.prev` and `.fol`\nattributes.\n\n``` python\nprint(arbitrary_interval.prev.label)\nprint(arbitrary_interval.label)\nprint(arbitrary_interval.fol.label)\n```\n\n    R\n    EY1\n    N\n\nWe can also access information about the word this interval is nested\nwithin with the `.inword` attribute.\n\n``` python\nprint(arbitrary_interval.inword.label)\n```\n\n    raindrops\n\nThe object returned by `.inword` is just another interval, meaning we\ncan access informaton about *it’s* context with the `.prev` and `.fol`\nattributes as well.\n\n``` python\nprint(arbitrary_interval.inword.prev.label)\nprint(arbitrary_interval.inword.label)\nprint(arbitrary_interval.inword.fol.label)\n```\n\n    strikes\n    raindrops\n    in\n\n## For more\n\n- To start jumping in, check out [the\n  quickstart](https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/usage/)\n- To learn more about navigating TextGrids and intervals, check out the\n  usage pages on [navigating\n  TextGrids](https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/usage/01_TextGrids/01_tg-nav.html)\n  and [navgiating\n  sequences](https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/usage/02_Sequences/00_sequence_structure.html)\n- To learn more about the attributes you can access from textgrids and\n  sequences, see the usage pages on [TextGrid\n  attributes](https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/usage/01_TextGrids/02_tg-info.html)\n  and [interval\n  attributes](https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/usage/02_Sequences/02_sequence_properties.html)\n\nYou can also directly read up on [the function and class\nreferences](https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/reference/).\n",
     'author': 'JoFrhwld',
     'author_email': 'JoFrhwld@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/',
```

### Comparing `aligned_textgrid-0.6.5/PKG-INFO` & `aligned_textgrid-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligned-textgrid
-Version: 0.6.5
+Version: 0.6.6
 Summary: Classes for defining sequential information from TextGrids
 Home-page: https://forced-alignment-and-vowel-extraction.github.io/alignedTextGrid/
 License: GPL-3.0-or-later
 Author: JoFrhwld
 Author-email: JoFrhwld@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

