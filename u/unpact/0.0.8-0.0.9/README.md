# Comparing `tmp/unpact-0.0.8.tar.gz` & `tmp/unpact-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unpact-0.0.8.tar", max compression
+gzip compressed data, was "unpact-0.0.9.tar", max compression
```

## Comparing `unpact-0.0.8.tar` & `unpact-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1046 2023-08-15 02:04:38.453175 unpact-0.0.8/LICENSE
--rw-r--r--   0        0        0     5690 2023-08-21 04:32:12.432113 unpact-0.0.8/README.md
--rw-r--r--   0        0        0     1025 2023-11-16 05:47:49.742031 unpact-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      181 2023-08-21 04:34:03.192787 unpact-0.0.8/unpact/__init__.py
--rw-r--r--   0        0        0        0 2023-08-21 02:46:16.701165 unpact-0.0.8/unpact/py.typed
--rw-r--r--   0        0        0     2964 2023-10-06 15:50:36.396450 unpact-0.0.8/unpact/tree.py
--rw-r--r--   0        0        0      625 2023-11-16 05:47:00.247129 unpact-0.0.8/unpact/types.py
--rw-r--r--   0        0        0     2200 2023-08-21 02:39:05.332773 unpact-0.0.8/unpact/unwind_util.py
--rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 unpact-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1046 2023-08-15 02:04:38.453175 unpact-0.0.9/LICENSE
+-rw-r--r--   0        0        0     5690 2023-08-21 04:32:12.432113 unpact-0.0.9/README.md
+-rw-r--r--   0        0        0     1025 2024-02-15 23:51:48.542691 unpact-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      181 2024-02-15 23:51:57.877342 unpact-0.0.9/unpact/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-21 02:46:16.701165 unpact-0.0.9/unpact/py.typed
+-rw-r--r--   0        0        0     4023 2024-02-15 23:48:39.089384 unpact-0.0.9/unpact/tree.py
+-rw-r--r--   0        0        0      625 2023-11-16 05:47:00.247129 unpact-0.0.9/unpact/types.py
+-rw-r--r--   0        0        0     2577 2024-02-15 23:50:29.046124 unpact-0.0.9/unpact/unwind_util.py
+-rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 unpact-0.0.9/PKG-INFO
```

### Comparing `unpact-0.0.8/LICENSE` & `unpact-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `unpact-0.0.8/README.md` & `unpact-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `unpact-0.0.8/pyproject.toml` & `unpact-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unpact"
-version = "0.0.8"
+version = "0.0.9"
 description = "A lightweight library for tabulating dictionaries"
 authors = ["Moph Toyer <chris@telemetry.fm>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["tables", "formatting", "flat", "flattening", "json"]
 packages = [{include = "unpact"}]
```

### Comparing `unpact-0.0.8/unpact/tree.py` & `unpact-0.0.9/unpact/tree.py`

 * *Files 27% similar despite different names*

```diff
@@ -65,27 +65,55 @@
         for k, v in data.items():
             child = load_tree(v, k, tree)
             tree.add_child(child)
 
     return tree
 
 
-def set(obj: dict, path: str, value: Any) -> None:
+def _set(obj: dict, path: str, value: Any) -> None:
     *split_path, last = path.split(".")
     for bit in split_path:
         obj = obj.setdefault(bit, {})
     obj[last] = value
 
 
+def get_keys_nested_dict(dictionary: dict, parent_key: str = "", sep: str = "."):
+    """
+    Get all keys in a nested dictionary in dot-delimited format.
+
+    Args:
+        dictionary (dict): The nested dictionary.
+        parent_key (str): The parent key to append for recursive calls (default is an empty string).
+        sep (str): The separator for joining keys (default is dot ".").
+
+    Returns:
+        set: A set of keys in dot-delimited format.
+    """
+    keys = []
+    for key, value in dictionary.items():
+        full_key = f"{parent_key}{sep}{key}" if parent_key else key
+        if isinstance(value, dict):
+            keys.extend(get_keys_nested_dict(value, full_key, sep=sep))
+        elif isinstance(value, list):
+            for i, item in enumerate(value):
+                if isinstance(item, dict):
+                    keys.extend(get_keys_nested_dict(item, f"{full_key}", sep=sep))
+                # else:
+                #     keys.append(f"{full_key}{sep}{i}")
+        else:
+            keys.append(full_key)
+    return set(keys)
+
+
 def load_tree_rep(paths: Sequence[Union[str, Tuple[str, ColumnSpec]]]) -> Tree:
     tree_dict: Dict[str, Any] = {}
     for path in paths:
         if isinstance(path, tuple):
             path = path[0]
-        set(tree_dict, path, None)
+        _set(tree_dict, path, None)
     tree = load_tree(tree_dict, "None", parent=None)
 
     specs: List[Tuple[str, ColumnSpec]] = [path for path in paths if isinstance(path, tuple)]
 
     for path, spec in specs:
         child = tree.get_child(path)
         child.tree_spec = spec
```

### Comparing `unpact-0.0.8/unpact/types.py` & `unpact-0.0.9/unpact/types.py`

 * *Files identical despite different names*

### Comparing `unpact-0.0.8/unpact/unwind_util.py` & `unpact-0.0.9/unpact/unwind_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, List, Sequence, Union
 from .types import ColumnDef
-from .tree import Tree, load_tree_rep
+from .tree import Tree, load_tree_rep, get_keys_nested_dict
 
 __all__ = ["unwind"]
 
 
 def _unwind(data: dict, tree: Tree) -> Union[List, List[Dict[str, Any]], Dict[str, Any], dict, List[dict]]:
     if not tree.children:
         tree_data = data.get(tree.path)
@@ -47,15 +47,24 @@
     if len(level_list) == 0:
         return level_dict
 
     appended = [{**level_dict, **list_value} for list_value in level_list]
     return appended
 
 
-def unwind(data: Dict[Any, Any], columns: Sequence[ColumnDef]) -> List[Dict[str, Any]]:
+def unwind(data: Dict[Any, Any], columns: Sequence[ColumnDef], allow_extra: bool = False) -> List[Dict[str, Any]]:
     paths_list = list(columns)
+
+    if allow_extra:
+        keys = get_keys_nested_dict(data)
+        specified_keys = [k[0] if isinstance(k, tuple) else k for k in columns]
+        extra_paths = [k for k in keys if k not in specified_keys]
+        extra_defs: List[ColumnDef] = [(k, {"name": k}) for k in extra_paths]
+
+        paths_list.extend(extra_defs)
+
     tree = load_tree_rep(paths_list)
     unwound = _unwind({"root": data}, tree)
     if not isinstance(unwound, list):
         return [unwound]
 
     return unwound
```

### Comparing `unpact-0.0.8/PKG-INFO` & `unpact-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unpact
-Version: 0.0.8
+Version: 0.0.9
 Summary: A lightweight library for tabulating dictionaries
 License: MIT
 Keywords: tables,formatting,flat,flattening,json
 Author: Moph Toyer
 Author-email: chris@telemetry.fm
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

