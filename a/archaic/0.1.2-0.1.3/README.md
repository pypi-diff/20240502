# Comparing `tmp/archaic-0.1.2.tar.gz` & `tmp/archaic-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archaic-0.1.2.tar", last modified: Fri Apr 26 23:54:45 2024, max compression
+gzip compressed data, was "archaic-0.1.3.tar", last modified: Thu May  2 11:30:54 2024, max compression
```

## Comparing `archaic-0.1.2.tar` & `archaic-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 23:54:45.280766 archaic-0.1.2/
--rw-rw-rw-   0        0        0      504 2024-04-26 23:54:45.279761 archaic-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        9 2024-04-20 18:47:21.000000 archaic-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 23:54:45.254643 archaic-0.1.2/archaic/
--rw-rw-rw-   0        0        0       92 2024-04-26 19:52:56.000000 archaic-0.1.2/archaic/__init__.py
--rw-rw-rw-   0        0        0     8172 2024-04-26 12:22:54.000000 archaic-0.1.2/archaic/feature_class.py
--rw-rw-rw-   0        0        0     3348 2024-04-26 19:00:44.000000 archaic-0.1.2/archaic/info.py
--rw-rw-rw-   0        0        0      593 2024-04-26 19:52:49.000000 archaic-0.1.2/archaic/models.py
--rw-rw-rw-   0        0        0     6052 2024-04-23 15:09:08.000000 archaic-0.1.2/archaic/predicate.py
-drwxrwxrwx   0        0        0        0 2024-04-26 23:54:45.272955 archaic-0.1.2/archaic.egg-info/
--rw-rw-rw-   0        0        0      504 2024-04-26 23:54:45.000000 archaic-0.1.2/archaic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-04-26 23:54:45.000000 archaic-0.1.2/archaic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 23:54:45.000000 archaic-0.1.2/archaic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-26 23:54:45.000000 archaic-0.1.2/archaic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      619 2024-04-26 19:54:26.000000 archaic-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-26 23:54:45.281762 archaic-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-02 11:30:54.613591 archaic-0.1.3/
+-rw-rw-rw-   0        0        0      504 2024-05-02 11:30:54.611147 archaic-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2024-04-20 18:47:21.000000 archaic-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 11:30:54.582630 archaic-0.1.3/archaic/
+-rw-rw-rw-   0        0        0       93 2024-05-01 14:13:08.000000 archaic-0.1.3/archaic/__init__.py
+-rw-rw-rw-   0        0        0     3348 2024-04-30 15:25:42.000000 archaic-0.1.3/archaic/_info.py
+-rw-rw-rw-   0        0        0      593 2024-04-29 12:23:08.000000 archaic-0.1.3/archaic/_models.py
+-rw-rw-rw-   0        0        0     6052 2024-04-23 15:09:08.000000 archaic-0.1.3/archaic/_predicate.py
+-rw-rw-rw-   0        0        0     9468 2024-05-01 14:13:24.000000 archaic-0.1.3/archaic/feature_class.py
+drwxrwxrwx   0        0        0        0 2024-05-02 11:30:54.609853 archaic-0.1.3/archaic.egg-info/
+-rw-rw-rw-   0        0        0      504 2024-05-02 11:30:54.000000 archaic-0.1.3/archaic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-05-02 11:30:54.000000 archaic-0.1.3/archaic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 11:30:54.000000 archaic-0.1.3/archaic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-02 11:30:54.000000 archaic-0.1.3/archaic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      619 2024-05-01 14:15:41.000000 archaic-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-02 11:30:54.613591 archaic-0.1.3/setup.cfg
```

### Comparing `archaic-0.1.2/archaic/feature_class.py` & `archaic-0.1.3/archaic/feature_class.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import arcpy
 from typing import Any, Callable, Generic, Iterable, List, Optional, Set, TypeVar, Union
-from archaic.info import Info
-from archaic.predicate import to_sql
+from archaic._info import Info
+from archaic._predicate import to_sql
 
 T = TypeVar("T")
 
 
 class FeatureClass(Generic[T]):
     def __init__(self, data_path: str, **mapping: str) -> None:
         """Initializes the feature class.  e.g.
@@ -75,31 +75,56 @@
         """
         for where_clause in self._get_where_clauses_from_ids(id):
             for item in self.read(where_clause, wkid):
                 return item
         return None
 
     def insert_many(self, items: Iterable[T], **kwargs: Any) -> List[int]:
+        """Inserts multiple items.
+
+        Args:
+            items: Items to insert.
+
+        Returns:
+            List[int]: List of object ids.
+        """
         data_path = self.info.data_path
         fields = list(self.info.edit_properties.values())
         properties = self.info.edit_properties
         with arcpy.da.InsertCursor(data_path, fields, **kwargs) as cursor:  # type: ignore
             return [
                 cursor.insertRow(self._get_values(item, properties)) for item in items
             ]
 
     def insert(self, item: T) -> T:
+        """Inserts a single item.
+
+        Args:
+            item: Item to insert.
+
+        Returns:
+            T: Created item.
+        """
         return self.get(self.insert_many([item])[0])  # type: ignore
 
     def update_where(
         self,
         filter: Union[str, Callable[[T], bool], Iterable[int], Iterable[str], None],
         update: Callable[[T], Union[None, T]],
         **kwargs: Any,
     ) -> List[int]:
+        """Updates items based on a procedure.
+
+        Args:
+            filter: Where clause, lambda expression, object ids or global ids.  If None, all items are updated.
+            update: Update procedure.  It may return an item (replacement) or None (mutation).
+
+        Returns:
+            List[int]: List of object ids.
+        """
         data_path = self.info.data_path
         fields = list(self.info.edit_properties.values())
         properties = self.info.edit_properties
         ids: Set[int] = set()
         for where_clause in self._get_where_clauses_from_filter(filter):
             with arcpy.da.UpdateCursor(data_path, fields, where_clause, **kwargs) as cursor:  # type: ignore
                 for row in cursor:
@@ -110,56 +135,78 @@
                     result = update(before)
                     after = before if result is None else result
                     cursor.updateRow(self._get_values(after, properties))
                     ids.add(self._get_oid(before))
         return list(ids)
 
     def update(self, items: Union[T, List[T]]) -> List[int]:
+        """Updates items based on their mutated state.
+
+        Args:
+            items: Items to update.
+
+        Returns:
+            List[int]: List of object ids.
+        """
         items = list(items) if isinstance(items, Iterable) else [items]
         cache = {self._get_oid(x): x for x in items}
         ids: Set[int] = set()
         for where_clause in self._get_where_clauses_from_ids(items):
             for id in self.update_where(
                 where_clause, lambda x: cache[self._get_oid(x)]
             ):
                 ids.add(id)
         return list(ids)
 
     def delete_where(self, filter: Union[str, Callable[[T], bool], None]) -> List[int]:
+        """Deletes items based on a filter.
+
+        Args:
+            filter: Where clause or lambda expression.  If None, all items are deleted.
+
+        Returns:
+            List[int]: List of object ids.
+        """
         data_path = self.info.data_path
         ids: Set[int] = set()
         for where_clause in self._get_where_clauses_from_filter(filter):
             with arcpy.da.UpdateCursor(data_path, self.info.oid_field, where_clause) as cursor:  # type: ignore
                 for row in cursor:
                     cursor.deleteRow()
                     ids.add(row[0])
         return list(ids)
 
     def delete(
         self, items: Union[T, int, str, Iterable[T], Iterable[int], Iterable[str]]
     ) -> List[int]:
+        """Deletes items specified or by object ids or global ids.
+
+        Args:
+            items: Items, object ids or global ids.
+
+        Returns:
+            List[int]: List of object ids.
+        """
         ids: Set[int] = set()
         for where_clause in self._get_where_clauses_from_ids(items):
             for id in self.delete_where(where_clause):
                 ids.add(id)
         return list(ids)
 
     def _create(self, **kwargs: Any) -> T:
         item = self.info.model(
             **{
                 k: v
                 for k, v in kwargs.items()
                 if k in self.info.properties and k in self.info.keys
             }
         )
-
         for property in self.info.properties:
             if property not in self.info.keys:
                 setattr(item, property, kwargs.get(property))
-
         return item
 
     def _get_values(self, item: T, properties: Iterable[str]) -> List[Any]:
         values: List[Any] = []
         for property in properties:
             values.append(getattr(item, property) if hasattr(item, property) else None)
         return values
```

### Comparing `archaic-0.1.2/archaic/info.py` & `archaic-0.1.3/archaic/_info.py`

 * *Files identical despite different names*

### Comparing `archaic-0.1.2/archaic/models.py` & `archaic-0.1.3/archaic/_models.py`

 * *Files identical despite different names*

### Comparing `archaic-0.1.2/archaic/predicate.py` & `archaic-0.1.3/archaic/_predicate.py`

 * *Files identical despite different names*

### Comparing `archaic-0.1.2/pyproject.toml` & `archaic-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "archaic"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Jiro Shirota", email="jshirota@gmail.com" },
 ]
 description = "Simplifies handling of ArcPy rows"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

