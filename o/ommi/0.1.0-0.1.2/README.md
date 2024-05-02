# Comparing `tmp/ommi-0.1.0.tar.gz` & `tmp/ommi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ommi-0.1.0.tar", max compression
+gzip compressed data, was "ommi-0.1.2.tar", max compression
```

## Comparing `ommi-0.1.0.tar` & `ommi-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1076 2024-01-06 14:43:20.901643 ommi-0.1.0/LICENSE
--rw-r--r--   0        0        0      704 2024-01-23 21:51:42.750589 ommi-0.1.0/README.md
--rw-r--r--   0        0        0     6148 2024-01-06 14:50:13.843382 ommi-0.1.0/ommi/.DS_Store
--rw-r--r--   0        0        0       86 2024-01-16 16:28:26.122558 ommi-0.1.0/ommi/__init__.py
--rw-r--r--   0        0        0      943 2024-01-16 17:17:54.892513 ommi-0.1.0/ommi/contextual_method.py
--rw-r--r--   0        0        0      347 2024-01-16 17:18:22.905239 ommi-0.1.0/ommi/driver_context.py
--rw-r--r--   0        0        0     2364 2024-01-23 20:46:48.996869 ommi-0.1.0/ommi/drivers.py
--rw-r--r--   0        0        0     6148 2024-01-06 14:49:37.254914 ommi-0.1.0/ommi/ext/.DS_Store
--rw-r--r--   0        0        0    14334 2024-01-23 21:01:10.621179 ommi-0.1.0/ommi/ext/drivers/sqlite.py
--rw-r--r--   0        0        0     5491 2024-01-23 20:58:20.244871 ommi-0.1.0/ommi/models.py
--rw-r--r--   0        0        0     9552 2024-01-16 17:16:02.655785 ommi-0.1.0/ommi/query_ast.py
--rw-r--r--   0        0        0      876 2024-01-06 15:53:52.477963 ommi-0.1.0/ommi/statuses.py
--rw-r--r--   0        0        0      546 2024-01-23 21:53:00.392310 ommi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1498 1970-01-01 00:00:00.000000 ommi-0.1.0/setup.py
--rw-r--r--   0        0        0     1296 1970-01-01 00:00:00.000000 ommi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-02 21:27:51.195847 ommi-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3723 2024-05-02 21:27:51.195847 ommi-0.1.2/README.md
+-rw-r--r--   0        0        0      195 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/__init__.py
+-rw-r--r--   0        0        0      943 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/contextual_method.py
+-rw-r--r--   0        0        0      677 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/driver_context.py
+-rw-r--r--   0        0        0     4676 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/drivers.py
+-rw-r--r--   0        0        0     6148 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/ext/.DS_Store
+-rw-r--r--   0        0        0    13048 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/ext/drivers/sqlite.py
+-rw-r--r--   0        0        0     4596 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/field_metadata.py
+-rw-r--r--   0        0        0      210 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/model_collections.py
+-rw-r--r--   0        0        0     7707 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/models.py
+-rw-r--r--   0        0        0     9718 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/query_ast.py
+-rw-r--r--   0        0        0     1279 2024-05-02 21:27:51.195847 ommi-0.1.2/ommi/statuses.py
+-rw-r--r--   0        0        0      767 2024-05-02 21:28:08.888096 ommi-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4535 1970-01-01 00:00:00.000000 ommi-0.1.2/PKG-INFO
```

### Comparing `ommi-0.1.0/LICENSE` & `ommi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ommi-0.1.0/ommi/contextual_method.py` & `ommi-0.1.2/ommi/contextual_method.py`

 * *Files identical despite different names*

### Comparing `ommi-0.1.0/ommi/ext/.DS_Store` & `ommi-0.1.2/ommi/ext/.DS_Store`

 * *Files identical despite different names*

### Comparing `ommi-0.1.0/ommi/ext/drivers/sqlite.py` & `ommi-0.1.2/ommi/ext/drivers/sqlite.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 import sqlite3
 from dataclasses import dataclass, field as dc_field
-from datetime import datetime, date, time
-from typing import Type, Any, TypeVar, TypeGuard, Callable, get_origin, Generator, Self
+from datetime import datetime, date
+from typing import Type, Any, TypeVar, Callable, get_origin, Generator
 
-from ommi.drivers import DatabaseDriver, DriverConfig
-from ommi.models import OmmiField, OmmiModel
+from tramp.results import Result
+
+from ommi.drivers import DatabaseDriver, DriverConfig, database_action
+from ommi.model_collections import ModelCollection
+from ommi.models import OmmiField, OmmiModel, get_collection
 from ommi.query_ast import (
     ASTGroupNode,
     when,
     ASTReferenceNode,
     ASTLiteralNode,
     ASTLogicalOperatorNode,
     ASTComparisonNode,
     ASTOperatorNode,
     ASTGroupFlagNode,
     ResultOrdering,
 )
-from ommi.statuses import (
-    DatabaseStatus,
-    DatabaseSuccessStatus,
-    DatabaseExceptionStatus,
-)
 
 T = TypeVar("T")
 
 
 @dataclass
 class SelectQuery:
     limit: int = 0
@@ -32,194 +30,174 @@
     offset: int = 0
     order_by: dict[str, ResultOrdering] = dc_field(default_factory=dict)
     tables: list[OmmiModel] = dc_field(default_factory=list)
     values: list[Any] = dc_field(default_factory=list)
     where: str = ""
 
 
-class SQLConstraint(Auto):
-    def __init__(self, name: str, value: str):
-        self.name = name
-        self.value = value
-
-    def __call__(self, *args, **kwargs):
-        return self
-
-    def __repr__(self):
-        return f"SQL{self.name.title()}Constraint[{self.value}]"
-
-
-class SQLAutoIncrement(SQLConstraint):
-    def __init__(self):
-        super().__init__("", "AUTOINCREMENT")
-
-    def __repr__(self):
-        return type(self).__name__
-
-
 @dataclass
 class SQLiteConfig(DriverConfig):
     filename: str
 
 
 class SQLiteDriver(DatabaseDriver, driver_name="sqlite", nice_name="SQLite"):
+    config: SQLiteConfig
+
     logical_operator_mapping = {
         ASTLogicalOperatorNode.AND: "AND",
         ASTLogicalOperatorNode.OR: "OR",
     }
 
     operator_mapping = {
         ASTOperatorNode.EQUALS: "=",
         ASTOperatorNode.NOT_EQUALS: "!=",
         ASTOperatorNode.GREATER_THAN: ">",
         ASTOperatorNode.GREATER_THAN_OR_EQUAL: ">=",
         ASTOperatorNode.LESS_THAN: "<",
         ASTOperatorNode.LESS_THAN_OR_EQUAL: "<=",
     }
 
-    auto_value_factories = {
-        int: SQLAutoIncrement(),
-        datetime: SQLConstraint("DEFAULT", "datetime()"),
-        date: SQLConstraint("DEFAULT", "date()"),
-        time: SQLConstraint("DEFAULT", "time()"),
-    }
-
     type_validators = {
         datetime: lambda value: value,  # No-op to avoid type conflict with date
         date: lambda value: value.split()[0],
     }
 
     type_mapping = {
         int: "INTEGER",
         str: "TEXT",
         float: "REAL",
         bool: "INTEGER",
     }
 
-    def __init__(self):
+    def __init__(self, *args):
+        super().__init__(*args)
         self._connected = False
         self._db: sqlite3.Connection | None = None
 
     @property
     def connected(self) -> bool:
         return self._connected
 
-    async def connect(self, config: SQLiteConfig) -> DatabaseStatus:
-        with SuppressWithCapture(Exception) as error:
-            self._db = sqlite3.connect(config.filename)
-            self._connected = True
-
-        return DatabaseExceptionStatus(*error) if error else DatabaseSuccessStatus(self)
-
-    async def disconnect(self) -> DatabaseStatus:
-        with SuppressWithCapture(Exception) as error:
-            self._db.close()
-            self._connected = False
+    @database_action
+    async def connect(self) -> "SQLiteDriver":
+        self._db = sqlite3.connect(self.config.filename)
+        self._connected = True
+        return self
 
-        return DatabaseExceptionStatus(*error) if error else DatabaseSuccessStatus(self)
+    @database_action
+    async def disconnect(self) -> "SQLiteDriver":
+        self._db.close()
+        self._connected = False
+        return self
 
-    async def add(self, *items: OmmiModel) -> DatabaseStatus:
+    @database_action
+    async def add(self, *items: OmmiModel) -> "SQLiteDriver":
         session = self._db.cursor()
-        with SuppressWithCapture(Exception) as error:
+        try:
             for item in items:
                 self._insert(item, session)
                 self._sync_with_last_inserted(item, session)
 
-        if error:
+        except:
             self._db.rollback()
-            return DatabaseExceptionStatus(*error)
+            raise
 
-        session.close()
-        return DatabaseSuccessStatus(self)
+        else:
+            return self
 
-    async def count(
-        self, *predicates: ASTGroupNode | Type[OmmiModel]
-    ) -> DatabaseStatus[int]:
-        ast = when(*predicates)
-        with SuppressWithCapture(Exception) as error:
-            session = self._db.cursor()
-            result = self._count(ast, session)
+        finally:
+            session.close()
 
-        return (
-            DatabaseExceptionStatus(*error) if error else DatabaseSuccessStatus(result)
-        )
+    @database_action
+    async def count(self, *predicates: ASTGroupNode | Type[OmmiModel]) -> int:
+        ast = when(*predicates)
+        session = self._db.cursor()
+        return self._count(ast, session)
 
-    async def delete(self, *items: OmmiModel) -> DatabaseStatus:
+    @database_action
+    async def delete(self, *items: OmmiModel) -> "SQLiteDriver":
         models = {}
         for item in items:
             models.setdefault(type(item), []).append(item)
 
         session = self._db.cursor()
-        for model, items in models.items():
-            with SuppressWithCapture(Exception) as error:
+        try:
+            for model, items in models.items():
                 self._delete_rows(model, items, session)
 
-            if error:
-                self._db.rollback()
-                return DatabaseExceptionStatus(*error)
+        except:
+            self._db.rollback()
+            raise
 
-        session.close()
-        return DatabaseSuccessStatus(self)
+        else:
+            return self
 
+        finally:
+            session.close()
+
+    @database_action
     async def fetch(
         self, *predicates: ASTGroupNode | Type[OmmiModel]
-    ) -> DatabaseStatus[list[OmmiModel]]:
+    ) -> list[OmmiModel]:
         ast = when(*predicates)
-        with SuppressWithCapture(Exception) as error:
-            session = self._db.cursor()
-            result = self._select(ast, session)
-
-        return (
-            DatabaseExceptionStatus(*error) if error else DatabaseSuccessStatus(result)
-        )
+        session = self._db.cursor()
+        result = self._select(ast, session)
+        return result
 
-    async def sync_schema(self, models: set[Type[OmmiModel]]) -> DatabaseStatus[Self]:
+    @database_action
+    async def sync_schema(
+        self, collection: ModelCollection | None = None
+    ) -> "SQLiteDriver":
         session = self._db.cursor()
-        with SuppressWithCapture(Exception) as error:
+        models = get_collection(
+            Result.Value(collection) if collection else Result.Nothing
+        ).models
+        try:
             for model in models:
                 self._create_table(model, session)
 
-        if error:
+        except:
             self._db.rollback()
-            return DatabaseExceptionStatus(*error)
+            raise
 
-        session.close()
-        return DatabaseSuccessStatus(self)
+        else:
+            return self
 
-    async def update(self, *items: OmmiModel) -> DatabaseStatus[Self]:
+        finally:
+            session.close()
+
+    @database_action
+    async def update(self, *items: OmmiModel) -> "SQLiteDriver":
         models = {}
         for item in items:
             models.setdefault(type(item), []).append(item)
 
         session = self._db.cursor()
-        for model, items in models.items():
-            with SuppressWithCapture(Exception) as error:
+        try:
+            for model, items in models.items():
                 self._update_rows(model, items, session)
 
-            if error:
-                self._db.rollback()
-                return DatabaseExceptionStatus(*error)
+        except:
+            self._db.rollback()
+            raise
+
+        else:
+            return self
 
-        session.close()
-        return DatabaseSuccessStatus(self)
+        finally:
+            session.close()
 
     def _build_column(self, field: OmmiField, pk: bool) -> str:
-        column = [field.name, self._get_sqlite_type(field.type)]
+        column = [
+            field.get("store_as"),
+            self._get_sqlite_type(field.get("field_type")),
+        ]
         if pk:
             column.append("PRIMARY KEY")
 
-        if is_auto(field.default):
-            match self.get_value_factory(field):
-                case SQLAutoIncrement():
-                    column.append("AUTOINCREMENT")
-
-                case SQLConstraint() as constraint:
-                    column.append(constraint.name)
-                    column.append(f"({constraint.value})")
-
         return " ".join(column)
 
     def _process_ast(self, ast: ASTGroupNode) -> SelectQuery:
         query = SelectQuery(
             limit=ast.max_results,
             offset=ast.results_page * ast.max_results,
             order_by=self._process_ordering(ast.sorting),
@@ -232,15 +210,15 @@
                     node_stack.append(iter(group))
 
                 case ASTReferenceNode(None, model):
                     query.tables.append(model)
                     query.model = query.model or model
 
                 case ASTReferenceNode(field, model):
-                    name = f"{model.__model_name__}.{field.name}"
+                    name = f"{model.__ommi_metadata__.model_name}.{field.name}"
                     where.append(name)
                     query.tables.append(model)
                     query.model = query.model or model
 
                 case ASTLiteralNode(value):
                     where.append("?")
                     query.values.append(value)
@@ -278,38 +256,50 @@
             f"{ref.model.__model_name__}.{ref.field.name}": ref.ordering
             for ref in sorting
         }
 
     def _create_table(self, model: Type[OmmiModel], session: sqlite3.Cursor):
         pk = self._find_primary_key(model)
         columns = ", ".join(
-            self._build_column(field, field.name == pk)
+            self._build_column(field, field.get("store_as") == pk)
             for field in model.__ommi_metadata__.fields.values()
         )
         session.execute(
             f"CREATE TABLE IF NOT EXISTS {model.__ommi_metadata__.model_name} ({columns});"
         )
 
     def _find_primary_key(self, model: Type[OmmiModel]) -> str:
+        if not model.__ommi_metadata__.fields:
+            raise Exception(f"No fields defined on {model}")
+
         fields = list(model.__ommi_metadata__.fields.values())
-        if name := next((f.name for f in fields if f.name.lower() == "id"), None):
+        if name := next(
+            (
+                f.get("store_as")
+                for f in fields
+                if f.get("store_as", f.get("field_name")).lower() == "id"
+            ),
+            None,
+        ):
             return name
 
         for field in fields:
-            if field.type is int or field.name.casefold() == "id":
-                return field.name
+            if (
+                field.get("field_type") is int
+                or field.get("store_as").casefold() == "id"
+            ):
+                return field.get("store_as")
 
-        return next(iter(fields)).name
+        return next(iter(fields)).get("store_as")
 
     def _insert(self, item: OmmiModel, session: sqlite3.Cursor):
         fields = list(item.__ommi_metadata__.fields.values())
         data = {
-            field.name: value
+            field.get("store_as"): getattr(item, field.get("field_name"))
             for field in fields
-            if not is_auto(value := getattr(item, field.name))
         }
         qs = ", ".join(["?"] * len(data))
         columns = ", ".join(data.keys())
         values = tuple(data.values())
         session.execute(
             f"INSERT INTO {item.__ommi_metadata__.model_name} ({columns}) VALUES ({qs});",
             values,
@@ -320,17 +310,23 @@
         model: Type[OmmiModel],
         items: list[OmmiModel],
         session: sqlite3.Cursor,
     ):
         pk = self._find_primary_key(model)
         fields = list(model.__ommi_metadata__.fields.values())
         for item in items:
-            values = (getattr(item, field.name) for field in fields if field.name != pk)
+            values = (
+                getattr(item, field.get("field_name"))
+                for field in fields
+                if field.get("store_as") != pk
+            )
             assignments = ", ".join(
-                f"{field.name} = ?" for field in fields if field.name != pk
+                f"{field.get('store_as')} = ?"
+                for field in fields
+                if field.get("store_as") != pk
             )
             session.execute(
                 f"UPDATE {model.__ommi_metadata__.model_name} SET {assignments} WHERE {pk} = ?;",
                 (*values, getattr(item, pk)),
             )
 
     def _delete_rows(
@@ -363,22 +359,20 @@
         result = session.fetchone()
         return result[0]
 
     def _validate_row_values(
         self, model: Type[OmmiModel], row: tuple[Any]
     ) -> Generator[Any, None, None]:
         for field, value in zip(model.__ommi_metadata__.fields.values(), row):
-            if validator := self._find_type_validator(field.type, value):
+            if validator := self._find_type_validator(field.get("field_type", value)):
                 yield validator(value)
             else:
                 yield value
 
-    def _find_type_validator(
-        self, type_hint: Type[T], value: Any
-    ) -> Callable[[Any], T] | None:
+    def _find_type_validator(self, type_hint: Type[T]) -> Callable[[Any], T] | None:
         hint = get_origin(type_hint) or type_hint
         for validator_type, validator in self.type_validators.items():
             if issubclass(hint, validator_type):
                 return validator
 
         return None
 
@@ -420,14 +414,8 @@
                 query_builder.append(f"OFFSET {query.offset}")
 
         return " ".join(query_builder) + ";"
 
     def _sync_with_last_inserted(self, item: OmmiModel, session: sqlite3.Cursor):
         pk = self._find_primary_key(type(item))
         result = session.execute("SELECT last_insert_rowid();").fetchone()
-        result = self._validate_row_values(type(item), result)
-        for field, value in zip(item.__ommi_metadata__.fields.values(), result):
-            item.__field_values__[field.name] = value
-
-
-def is_auto(obj: Any) -> TypeGuard[Auto]:
-    return isinstance(obj, Auto)
+        setattr(item, pk, result[0])
```

### Comparing `ommi-0.1.0/ommi/query_ast.py` & `ommi-0.1.2/ommi/query_ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         if len(self.items) > 1:
             yield ASTGroupFlagNode.CLOSE
 
     def add(self, item, logical_type=ASTLogicalOperatorNode.AND):
         if self.frozen:
             return
 
-        if isinstance(item, type) and issubclass(item, models.DatabaseModel):
+        if isinstance(item, type) and issubclass(item, models.OmmiModel):
             item = ASTReferenceNode(None, item)
 
         elif len(self.items) > 0 and getattr(self.items[~0], "field", True) is not None:
             self.items.append(logical_type)
 
         self.items.append(item)
 
@@ -346,9 +346,16 @@
             return comparison.group
 
         case (ASTGroupNode() as group,):
             return group
 
         case _:
             group = ASTGroupNode()
-            apply(group.add).to(comparisons)
+            for c in comparisons:
+                match c:
+                    case ASTComparisonNode():
+                        group.add(c.group)
+
+                    case _:
+                        group.add(c)
+
             return group
```

### Comparing `ommi-0.1.0/ommi/statuses.py` & `ommi-0.1.2/ommi/statuses.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,34 +3,49 @@
 from tramp.results import Value, Nothing
 
 
 V = TypeVar("V")
 
 
 class DatabaseStatus(Generic[V]):
-    Success: "Type[DatabaseStatus[V]]"
-    Exception: "DatabaseStatus[V]"
+    Success: "Type[DatabaseSuccessStatus[V]]"
+    Exception: "Type[DatabaseExceptionStatus[V]]"
 
 
-class DatabaseSuccessStatus(DatabaseStatus, Value):
+class DatabaseSuccessStatus(Value, DatabaseStatus):
     def __eq__(self, other):
         if not isinstance(other, DatabaseStatus):
             return NotImplemented
 
         if not isinstance(other, DatabaseSuccessStatus):
             return False
 
         return self.value == other.value
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}({self.value!r})"
 
 
 class DatabaseExceptionStatus(DatabaseStatus, Nothing):
+    __match_args__ = ("exception",)
+
+    def __new__(cls, *_):
+        return object.__new__(cls)
+
+    def __init__(self, exception: Exception) -> None:
+        self.exception = exception
+
     def __eq__(self, other):
         if not isinstance(other, DatabaseStatus):
             raise NotImplementedError()
 
         if not isinstance(other, DatabaseExceptionStatus):
             return False
 
         return True
+
+    def __repr__(self) -> str:
+        return f"{type(self).__name__}({self.exception!r})"
+
+
+DatabaseStatus.Success = DatabaseSuccessStatus
+DatabaseStatus.Exception = DatabaseExceptionStatus
```

### Comparing `ommi-0.1.0/pyproject.toml` & `ommi-0.1.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [tool.poetry]
 name = "ommi"
-version = "0.1.0"
-description = "An object model mapper intended to provide a consistent interface for many underlying database implementations using whatever model implementations are desired."
+version = "0.1.2"
+description = "A portable object model mapper that can work with any database and model library (dataclasses, Attrs, Pydantic, etc.). It is designed for the general case to support the largest possible number of databases."
 authors = ["Zech Zimmerman <hi@zech.codes>"]
 license = "MIT"
 readme = "README.md"
+homepage = "https://github.com/ZechCodes/Ommi"
+keywords = ["database", "orm", "object model mapper", "dataclasses", "attrs", "pydantic", "sqlite"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 tramp = "^0.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pydantic = "^2.5.3"
 attrs = "^23.2.0"
 pytest = "^7.4.4"
+pytest-asyncio = "^0.23.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

