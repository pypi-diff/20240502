# Comparing `tmp/mongoz-0.7.0.tar.gz` & `tmp/mongoz-0.8.0.tar.gz`

## Comparing `mongoz-0.7.0.tar` & `mongoz-0.8.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/__init__.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/exceptions.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/py.typed
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/types.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/conf/__init__.py
--rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/conf/functional.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/conf/global_settings.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/conf/module_import.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/__init__.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/connection/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/connection/collections.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/connection/database.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/connection/registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/__init__.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/datastructures.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/documents/__init__.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/documents/_internal.py
--rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/documents/base.py
--rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/documents/document.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/documents/document_proxy.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/documents/document_row.py
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/documents/managers.py
--rw-r--r--   0        0        0    16421 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/documents/metaclasses.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/fields/__init__.py
--rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/fields/base.py
--rw-r--r--   0        0        0    11761 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/fields/core.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/querysets/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/querysets/base.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/querysets/expressions.py
--rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/querysets/operators.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/querysets/core/constants.py
--rw-r--r--   0        0        0    21681 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/querysets/core/manager.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/querysets/core/protocols.py
--rw-r--r--   0        0        0    12693 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/querysets/core/queryset.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/signals/__init__.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/signals/handlers.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/signals/signal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/utils/__init__.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/utils/documents.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/utils/functional.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/utils/sync.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/protocols/__init__.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/protocols/queryset.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/utils/__init__.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/utils/enums.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/utils/inspect.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/utils/mixins.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mongoz-0.7.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mongoz-0.7.0/LICENSE
--rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 mongoz-0.7.0/README.md
--rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 mongoz-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 mongoz-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/__init__.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/exceptions.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/py.typed
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/types.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/conf/__init__.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/conf/functional.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/conf/global_settings.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/conf/module_import.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/__init__.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/connection/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/connection/collections.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/connection/database.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/connection/registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/__init__.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/datastructures.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/documents/__init__.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/documents/_internal.py
+-rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/documents/base.py
+-rw-r--r--   0        0        0     7186 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/documents/document.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/documents/document_proxy.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/documents/document_row.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/documents/managers.py
+-rw-r--r--   0        0        0    16421 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/documents/metaclasses.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/fields/__init__.py
+-rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/fields/base.py
+-rw-r--r--   0        0        0    11761 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/fields/core.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/querysets/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/querysets/base.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/querysets/expressions.py
+-rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/querysets/operators.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/querysets/core/constants.py
+-rw-r--r--   0        0        0    22757 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/querysets/core/manager.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/querysets/core/protocols.py
+-rw-r--r--   0        0        0    12693 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/db/querysets/core/queryset.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/signals/__init__.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/signals/handlers.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/signals/signal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/utils/__init__.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/utils/documents.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/utils/functional.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/core/utils/sync.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/protocols/__init__.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/protocols/queryset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/utils/__init__.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/utils/enums.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/utils/inspect.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 mongoz-0.8.0/mongoz/utils/mixins.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mongoz-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mongoz-0.8.0/LICENSE
+-rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 mongoz-0.8.0/README.md
+-rw-r--r--   0        0        0     4719 2020-02-02 00:00:00.000000 mongoz-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     8951 2020-02-02 00:00:00.000000 mongoz-0.8.0/PKG-INFO
```

### Comparing `mongoz-0.7.0/mongoz/__init__.py` & `mongoz-0.8.0/mongoz/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.0"
+__version__ = "0.8.0"
 
 from .conf import settings
 from .conf.global_settings import MongozSettings
 from .core.connection.database import Database
 from .core.connection.registry import Registry
 from .core.db import fields
 from .core.db.datastructures import Index, IndexType, Order
```

### Comparing `mongoz-0.7.0/mongoz/exceptions.py` & `mongoz-0.8.0/mongoz/exceptions.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/conf/__init__.py` & `mongoz-0.8.0/mongoz/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/conf/functional.py` & `mongoz-0.8.0/mongoz/conf/functional.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/conf/global_settings.py` & `mongoz-0.8.0/mongoz/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/conf/module_import.py` & `mongoz-0.8.0/mongoz/conf/module_import.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/core/connection/database.py` & `mongoz-0.8.0/mongoz/core/connection/database.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/core/connection/registry.py` & `mongoz-0.8.0/mongoz/core/connection/registry.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/core/db/datastructures.py` & `mongoz-0.8.0/mongoz/core/db/datastructures.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/core/db/documents/base.py` & `mongoz-0.8.0/mongoz/core/db/documents/base.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/core/db/documents/document.py` & `mongoz-0.8.0/mongoz/core/db/documents/document.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 from typing import Any, ClassVar, List, Mapping, Type, TypeVar, Union, cast
 
 import bson
 import pydantic
 from bson.errors import InvalidId
+from motor.motor_asyncio import AsyncIOMotorCollection
 from pydantic import BaseModel
 
+from mongoz.core.connection.collections import Collection
 from mongoz.core.db.documents.document_row import DocumentRow
 from mongoz.core.db.documents.metaclasses import EmbeddedModelMetaClass
 from mongoz.core.db.fields.base import MongozField
 from mongoz.exceptions import InvalidKeyError
 from mongoz.utils.mixins import is_operation_allowed
 
 T = TypeVar("T", bound="Document")
 
 
 class Document(DocumentRow):
     """
     Representation of an Mongoz Document.
     """
 
-    async def create(self: "Document") -> "Document":
+    async def create(
+        self: "Document", collection: Union[AsyncIOMotorCollection, None] = None
+    ) -> "Document":
         """
         Inserts a document.
         """
         is_operation_allowed(self)
 
         await self.signals.pre_save.send(sender=self.__class__, instance=self)
 
         data = self.model_dump(exclude={"id"})
-        result = await self.meta.collection._collection.insert_one(data)  # type: ignore
+        if collection is not None:
+            result = await collection.insert_one(data)
+        else:
+            if isinstance(self.meta.collection, Collection):
+                result = await self.meta.collection._collection.insert_one(data)  # noqa
         self.id = result.inserted_id
 
         await self.signals.post_save.send(sender=self.__class__, instance=self)
         return self
 
     async def update(self, **kwargs: Any) -> "Document":
         """
```

### Comparing `mongoz-0.7.0/mongoz/core/db/documents/document_proxy.py` & `mongoz-0.8.0/mongoz/core/db/documents/document_proxy.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/core/db/documents/document_row.py` & `mongoz-0.8.0/mongoz/core/db/documents/document_row.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/core/db/documents/managers.py` & `mongoz-0.8.0/mongoz/core/db/documents/managers.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/core/db/documents/metaclasses.py` & `mongoz-0.8.0/mongoz/core/db/documents/metaclasses.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/core/db/fields/__init__.py` & `mongoz-0.8.0/mongoz/core/db/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/core/db/fields/base.py` & `mongoz-0.8.0/mongoz/core/db/fields/base.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/core/db/fields/core.py` & `mongoz-0.8.0/mongoz/core/db/fields/core.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/core/db/querysets/expressions.py` & `mongoz-0.8.0/mongoz/core/db/querysets/expressions.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/core/db/querysets/operators.py` & `mongoz-0.8.0/mongoz/core/db/querysets/operators.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/core/db/querysets/core/manager.py` & `mongoz-0.8.0/mongoz/core/db/querysets/core/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,14 +61,40 @@
         self._only_fields = [] if only_fields is None else only_fields
         self._defer_fields = [] if defer_fields is None else defer_fields
         self.extra: Dict[str, Any] = {}
 
     def __get__(self, instance: Any, owner: Any) -> "Manager":
         return self.__class__(model_class=owner)
 
+    def using(self, database_name: str) -> "Manager":
+        """
+            **Type** Public
+
+            **Arguments:**
+                - database_name (str): string contains the database name.
+
+            **Returns:**
+                - Object: self instance.
+
+            **Raises:**
+                - None
+
+            This method is use to select the database:
+                - get the data base using the get_database method form the meta \
+                    class registry using the database_name that provided in \
+                        argument.
+                - store the database object as database.
+                - get the collection from the data base based on \
+                    self._collection.name
+                - return the self instance.
+        """
+        database = self.model_class.meta.registry.get_database(database_name)  # type: ignore
+        self._collection = database.get_collection(self._collection.name)._collection
+        return self
+
     def clone(self) -> Any:
         manager = self.__class__.__new__(self.__class__)
         manager.model_class = self.model_class
         manager._filter = self._filter
         manager._limit_count = self._limit_count
         manager._skip_count = self._skip_count
         manager._sort = self._sort
@@ -192,24 +218,26 @@
             if exclude:
                 operator = self.get_operator("not")
                 clauses = [operator(clause.key, clause) for clause in clauses]  # type: ignore
                 filter_clauses += clauses
             else:
                 filter_clauses += clauses
 
-        return cast(
+        manager = cast(
             "Manager",
             self.__class__(
                 model_class=self.model_class,
                 filter_by=filter_clauses,
                 sort_by=sort_clauses,
                 only_fields=self._only_fields,
                 defer_fields=self._defer_fields,
             ),
         )
+        manager._collection = self._collection
+        return manager
 
     def filter(self, **kwargs: Any) -> "Manager":
         """
         Filters the queryset based on the given clauses.
         """
         manager: "Manager" = self.clone()
         return manager.filter_query(**kwargs)
@@ -351,15 +379,15 @@
         return cast(int, await manager._collection.count_documents(filter_query))
 
     async def create(self, **kwargs: Any) -> "Document":
         """
         Creates a mongo db document.
         """
         manager: "Manager" = self.clone()
-        instance = await manager.model_class(**kwargs).create()
+        instance = await manager.model_class(**kwargs).create(manager._collection)
         return cast("Document", instance)
 
     async def delete(self) -> int:
         """Delete documents matching the criteria."""
         manager: "Manager" = self.clone()
         filter_query = Expression.compile_many(manager._filter)
         result = await manager._collection.delete_many(filter_query)
```

### Comparing `mongoz-0.7.0/mongoz/core/db/querysets/core/queryset.py` & `mongoz-0.8.0/mongoz/core/db/querysets/core/queryset.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/core/signals/handlers.py` & `mongoz-0.8.0/mongoz/core/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/core/signals/signal.py` & `mongoz-0.8.0/mongoz/core/signals/signal.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/core/utils/documents.py` & `mongoz-0.8.0/mongoz/core/utils/documents.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/core/utils/functional.py` & `mongoz-0.8.0/mongoz/core/utils/functional.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/protocols/queryset.py` & `mongoz-0.8.0/mongoz/protocols/queryset.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/mongoz/utils/enums.py` & `mongoz-0.8.0/mongoz/utils/enums.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/LICENSE` & `mongoz-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/README.md` & `mongoz-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `mongoz-0.7.0/pyproject.toml` & `mongoz-0.8.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -49,49 +49,76 @@
 [project.urls]
 Homepage = "https://github.com/tarsil/mongoz"
 Documentation = "https://mongoz.tarsild.io"
 Changelog = "https://mongoz.tarsild.io/release-notes/"
 Funding = "https://github.com/sponsors/tarsil"
 Source = "https://github.com/tarsil/mongoz"
 
-[project.optional-dependencies]
-test = [
+
+[tool.hatch.version]
+path = "mongoz/__init__.py"
+
+[tool.hatch.envs.default]
+dependencies = [
+    "anyio>=4.0.0,<5",
+    "mypy==1.9.0",
+    "ruff>=0.3.0,<5.0.0",
+    "pre-commit>=3.3.1,<4.0.0",
+    "devtools>=0.12.2",
+    "ipython",
+    "ptpython",
+    "twine",
+]
+
+[tool.hatch.envs.default.scripts]
+clean_pyc = "find . -type f -name \"*.pyc\" -delete"
+clean_pyi = "find . -type f -name \"*.pyi\" -delete"
+clean_pycache = "find . -type d -name \"*__pycache__*\" -delete"
+build_with_check = "hatch build; twine check dist/*"
+lint = "ruff check --fix --line-length 99  mongoz tests {args}"
+
+[tool.hatch.envs.docs]
+dependencies = [
+    "griffe-typingdoc>=0.2.2,<1.0",
+    "mkautodoc>=0.2.0,<0.3.0",
+    "mkdocs>=1.1.2,<2.0.0",
+    "mkdocs-material>=9.4.4,<10.0.0",
+    "mdx-include>=1.4.2,<2.0.0",
+    "mkdocs-markdownextradata-plugin>=0.2.5,<0.3.0",
+    "mkdocs-meta-descriptions-plugin>=2.3.0",
+    "mkdocstrings[python]>=0.23.0,<0.30.0",
+    "pyyaml>=6.0,<7.0.0",
+]
+
+[tool.hatch.envs.docs.scripts]
+build = "mkdocs build"
+serve = "mkdocs serve --dev-addr localhost:8000"
+
+[tool.hatch.envs.test]
+dependencies = [
     "a2wsgi>1.10.0,<2.0.0",
     "autoflake>=2.0.2,<3.0.0",
     "black==24.1.1,<25.0",
-    "esmerald>=3.0.0",
+    "esmerald>=3.1.3",
     "httpx>=0.25.0,<0.30.0",
     "isort>=5.12.0,<6.0.0",
     "mypy==1.9.0",
     "pytest>=7.2.2,<9.0.0",
     "pytest-asyncio>=0.21.1,<1.0.0",
     "pytest-cov>=4.0.0,<5.0.0",
     "requests>=2.28.2",
     "ruff>=0.0.256,<1.0.0",
 ]
+[tool.hatch.envs.test.scripts]
+# needs docker services running
+test = "pytest {args}"
+test_detail = "pytest {args} --disable-pytest-warnings -s -vv"
+coverage = "pytest --cov=asyncz --cov=tests --cov-report=term-missing:skip-covered --cov-report=html tests {args}"
+check_types = "mypy -p mongoz"
 
-dev = [
-    "anyio>=4.0.0,<5",
-    "ipdb>=0.13.13,<1.0.0",
-    "pdbpp",
-    "pre-commit>=3.3.1,<4.0.0",
-]
-
-doc = [
-    "mkautodoc>=0.2.0,<0.3.0",
-    "mkdocs>=1.4.2,<2.0.0",
-    "mkdocs-material==9.1.5",
-    "mdx-include>=1.4.1,<2.0.0",
-    "mkdocs-markdownextradata-plugin>=0.1.7,<0.3.0",
-    "mkdocstrings>=0.19.0,<0.21.0",
-    "pyyaml>=5.3.1,<7.0.0",
-]
-
-[tool.hatch.version]
-path = "mongoz/__init__.py"
 
 [tool.isort]
 profile = "black"
 known_third_party = []
 src_paths = ["mongoz"]
 
 [tool.mypy]
```

### Comparing `mongoz-0.7.0/PKG-INFO` & `mongoz-0.8.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mongoz
-Version: 0.7.0
+Version: 0.8.0
 Summary: ODM with pydantic made it simple
 Project-URL: Homepage, https://github.com/tarsil/mongoz
 Project-URL: Documentation, https://mongoz.tarsild.io
 Project-URL: Changelog, https://mongoz.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/mongoz
 Author-email: Tiago Silva <tiago.arasivla@gmail.com>
@@ -37,40 +37,14 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: dymmond-settings>=1.0.4
 Requires-Dist: motor>=3.3.1
 Requires-Dist: orjson>=3.9.5
 Requires-Dist: pydantic<3.0.0,>=2.5.3
-Provides-Extra: dev
-Requires-Dist: anyio<5,>=4.0.0; extra == 'dev'
-Requires-Dist: ipdb<1.0.0,>=0.13.13; extra == 'dev'
-Requires-Dist: pdbpp; extra == 'dev'
-Requires-Dist: pre-commit<4.0.0,>=3.3.1; extra == 'dev'
-Provides-Extra: doc
-Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'doc'
-Requires-Dist: mkautodoc<0.3.0,>=0.2.0; extra == 'doc'
-Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'doc'
-Requires-Dist: mkdocs-material==9.1.5; extra == 'doc'
-Requires-Dist: mkdocs<2.0.0,>=1.4.2; extra == 'doc'
-Requires-Dist: mkdocstrings<0.21.0,>=0.19.0; extra == 'doc'
-Requires-Dist: pyyaml<7.0.0,>=5.3.1; extra == 'doc'
-Provides-Extra: test
-Requires-Dist: a2wsgi<2.0.0,>1.10.0; extra == 'test'
-Requires-Dist: autoflake<3.0.0,>=2.0.2; extra == 'test'
-Requires-Dist: black<25.0,==24.1.1; extra == 'test'
-Requires-Dist: esmerald>=3.0.0; extra == 'test'
-Requires-Dist: httpx<0.30.0,>=0.25.0; extra == 'test'
-Requires-Dist: isort<6.0.0,>=5.12.0; extra == 'test'
-Requires-Dist: mypy==1.9.0; extra == 'test'
-Requires-Dist: pytest-asyncio<1.0.0,>=0.21.1; extra == 'test'
-Requires-Dist: pytest-cov<5.0.0,>=4.0.0; extra == 'test'
-Requires-Dist: pytest<9.0.0,>=7.2.2; extra == 'test'
-Requires-Dist: requests>=2.28.2; extra == 'test'
-Requires-Dist: ruff<1.0.0,>=0.0.256; extra == 'test'
 Description-Content-Type: text/markdown
 
 # MongoZ
 
 <p align="center">
   <a href="https://mongoz.tarsild.io"><img src="https://res.cloudinary.com/tarsild/image/upload/v1695724284/packages/mongoz/nwtcudxmncgoyw4em0th.png" alt='mongoz'></a>
 </p>
```

