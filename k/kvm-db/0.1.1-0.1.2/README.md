# Comparing `tmp/kvm_db-0.1.1.tar.gz` & `tmp/kvm_db-0.1.2.tar.gz`

## Comparing `kvm_db-0.1.1.tar` & `kvm_db-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 kvm_db-0.1.1/Makefile
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 kvm_db-0.1.1/requirements-dev.lock
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 kvm_db-0.1.1/requirements.lock
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 kvm_db-0.1.1/tox.ini
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 kvm_db-0.1.1/.github/workflows/linters.yaml
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 kvm_db-0.1.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 kvm_db-0.1.1/.github/workflows/pytest.yaml
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 kvm_db-0.1.1/src/kvm_db/__init__.py
--rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 kvm_db-0.1.1/src/kvm_db/kv_db.py
--rw-r--r--   0        0        0     4620 2020-02-02 00:00:00.000000 kvm_db-0.1.1/src/kvm_db/model_db.py
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 kvm_db-0.1.1/src/kvm_db/backends/base.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 kvm_db-0.1.1/src/kvm_db/backends/sqlite.py
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 kvm_db-0.1.1/tests/test_kv_db.py
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 kvm_db-0.1.1/tests/test_model_db.py
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 kvm_db-0.1.1/tests/backends/test_sqlite.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 kvm_db-0.1.1/.gitignore
--rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 kvm_db-0.1.1/README.md
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 kvm_db-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3402 2020-02-02 00:00:00.000000 kvm_db-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 kvm_db-0.1.2/Makefile
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 kvm_db-0.1.2/requirements-dev.lock
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 kvm_db-0.1.2/requirements.lock
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 kvm_db-0.1.2/tox.ini
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 kvm_db-0.1.2/.github/workflows/linters.yaml
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 kvm_db-0.1.2/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 kvm_db-0.1.2/.github/workflows/pytest.yaml
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 kvm_db-0.1.2/src/kvm_db/__init__.py
+-rw-r--r--   0        0        0     3993 2020-02-02 00:00:00.000000 kvm_db-0.1.2/src/kvm_db/kv_db.py
+-rw-r--r--   0        0        0     4657 2020-02-02 00:00:00.000000 kvm_db-0.1.2/src/kvm_db/model_db.py
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 kvm_db-0.1.2/src/kvm_db/backends/base.py
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 kvm_db-0.1.2/src/kvm_db/backends/sqlite.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 kvm_db-0.1.2/tests/test_kv_db.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 kvm_db-0.1.2/tests/test_model_db.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 kvm_db-0.1.2/tests/backends/test_sqlite.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 kvm_db-0.1.2/.gitignore
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 kvm_db-0.1.2/README.md
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 kvm_db-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 kvm_db-0.1.2/PKG-INFO
```

### Comparing `kvm_db-0.1.1/requirements-dev.lock` & `kvm_db-0.1.2/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `kvm_db-0.1.1/.github/workflows/linters.yaml` & `kvm_db-0.1.2/.github/workflows/linters.yaml`

 * *Files identical despite different names*

### Comparing `kvm_db-0.1.1/.github/workflows/publish.yaml` & `kvm_db-0.1.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `kvm_db-0.1.1/.github/workflows/pytest.yaml` & `kvm_db-0.1.2/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `kvm_db-0.1.1/src/kvm_db/kv_db.py` & `kvm_db-0.1.2/src/kvm_db/kv_db.py`

 * *Files 15% similar despite different names*

```diff
@@ -41,22 +41,22 @@
     @overload
     def __getitem__(self, query: tuple[str, str | slice]) -> str | list[tuple[str, str]]: ...
 
     @overload
     def __getitem__(self, query: slice) -> str: ...
 
     @overload
-    def __getitem__(self, query: str) -> "_KeyValTable": ...
+    def __getitem__(self, query: str) -> "KeyValTable": ...
 
     def __getitem__(
         self,
         query: str | tuple[str, str | slice] | slice,
-    ) -> Union[str, "_KeyValTable", list[tuple[str, str]]]:
+    ) -> Union[str, "KeyValTable", list[tuple[str, str]]]:
         if isinstance(query, str):
-            return _KeyValTable(self, query)
+            return KeyValTable(self, query)
         elif isinstance(query, slice):
             table = query.start
             key = query.stop
         else:
             table, key = query
             if isinstance(key, slice):
                 if any([key.start, key.stop]):
@@ -66,23 +66,14 @@
 
         datum = self.get_datum(table, key)
         if datum is None:
             raise KeyError(f"Key {key} not found in table {table}")
 
         return datum
 
-    @overload
-    def __setitem__(self, query: tuple[str, str], value: str) -> None: ...
-
-    @overload
-    def __setitem__(self, query: slice, value: str) -> None: ...
-
-    @overload
-    def __setitem__(self, query: str, value: str) -> None: ...
-
     def __setitem__(
         self,
         query: str | tuple[str, str] | slice,
         value: str,
     ) -> None:
         if isinstance(query, str):
             raise ValueError("Cannot set value for entire table")
@@ -90,29 +81,14 @@
             table = query.start
             key = query.stop
         else:
             table, key = query
 
         self.insert_datum(table, key, value)
 
-    @overload
-    def __delitem__(self, query: tuple[str, slice]) -> None: ...
-
-    @overload
-    def __delitem__(self, query: tuple[str, str]) -> None: ...
-
-    @overload
-    def __delitem__(self, query: tuple[str, str | slice]) -> None: ...
-
-    @overload
-    def __delitem__(self, query: slice) -> None: ...
-
-    @overload
-    def __delitem__(self, query: str) -> None: ...
-
     def __delitem__(self, query: str | tuple[str, str | slice] | slice) -> None:
         if isinstance(query, str):
             raise ValueError("Cannot delete entire table")
         elif isinstance(query, slice):
             table = query.start
             key = query.stop
         else:
@@ -125,15 +101,15 @@
                 for key, _ in all_keys:
                     self.delete_datum(table, key)
                 return
 
         self.delete_datum(table, key)
 
 
-class _KeyValTable:
+class KeyValTable:
     def __init__(self, kv_db: KeyValDatabase, table: str) -> None:
         self.kv_db = kv_db
         self.table = table
 
     @overload
     def __getitem__(self, key: str) -> str: ...
 
@@ -143,15 +119,9 @@
     def __getitem__(self, key: str | slice) -> str | list[tuple[str, str]]:
         a = self.kv_db[self.table, key]
         return a
 
     def __setitem__(self, key: str, value: str) -> None:
         self.kv_db[self.table, key] = value
 
-    @overload
-    def __delitem__(self, key: str) -> None: ...
-
-    @overload
-    def __delitem__(self, key: slice) -> None: ...
-
     def __delitem__(self, key: str | slice) -> None:
         del self.kv_db[self.table, key]
```

### Comparing `kvm_db-0.1.1/src/kvm_db/model_db.py` & `kvm_db-0.1.2/src/kvm_db/model_db.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 from pydantic import BaseModel, Field, PrivateAttr
 
 from kvm_db.backends.base import FastDatabaseBackend
 
 
 class TableModel(BaseModel):
-    _databse: Optional["ModelDatabase"] = PrivateAttr(default=None)
+    _database: Optional["ModelDatabase"] = PrivateAttr(default=None)
 
     id: str = Field(frozen=True, default_factory=lambda: str(uuid.uuid4()))
 
     def commit(self) -> None:
-        if self._databse is None:
+        if self._database is None:
             raise ValueError("Database not set")
-        self._databse.update(self)
+        self._database.update(self)
 
     def delete(self) -> None:
-        if self._databse is None:
+        if self._database is None:
             raise ValueError("Database not set")
-        self._databse.delete(self)
+        self._database.delete(self)
 
 
 _gDatum = TypeVar("_gDatum", bound=TableModel)
 
 
 class ModelDatabase:
     def __init__(self, backend: FastDatabaseBackend) -> None:
@@ -33,46 +33,50 @@
 
     def register(self, model: type[TableModel]) -> None:
         self._backend._create_table(model.__name__)
 
     def insert(self, model: TableModel) -> None:
         serialzied = model.model_dump_json(exclude={"_databse"})
         self._backend._insert_datum(model.__class__.__name__, model.id, serialzied)
-        model._databse = self
+        model._database = self
 
-    def delete(self, model: TableModel | type[TableModel], id: str | None = None) -> None:
+    def delete(
+        self,
+        model: TableModel | type[TableModel],
+        id: str | None = None,
+    ) -> None:
         if isinstance(model, type):
             if id is None:
                 raise ValueError("id must be provided to delete table")
             self._backend._delete_datum(model.__name__, id)
         else:
             self._backend._delete_datum(model.__class__.__name__, model.id)
-            model._databse = None
+            model._database = None
 
     def get_datum(
         self,
         model_type: type[_gDatum],
         id: str,
     ) -> _gDatum:
         model_data = self._backend._get_datum(model_type.__name__, id)
         if model_data is None:
             raise KeyError(f"Model {model_type.__name__} with id {id} not found")
         datum = model_type.model_validate_json(model_data)
-        datum._databse = self
+        datum._database = self
         return datum
 
     def get_all_data(self, model_type: type[_gDatum]) -> list[_gDatum]:
         all_data = self._backend._get_all_data(model_type.__name__)
         data = [model_type.model_validate_json(data[1]) for data in all_data]
         for datum in data:
-            datum._databse = self
+            datum._database = self
         return data
 
     def update(self, model: TableModel) -> None:
-        if model._databse is None:
+        if model._database is None:
             raise ValueError("Disconnect model from database")
         self._backend._update_datum(
             model.__class__.__name__,
             model.id,
             model.model_dump_json(),
         )
 
@@ -85,22 +89,22 @@
     @overload
     def __getitem__(self, query: tuple[type[_gDatum], str | slice]) -> _gDatum | list[_gDatum]: ...
 
     @overload
     def __getitem__(self, query: slice) -> TableModel: ...
 
     @overload
-    def __getitem__(self, query: type[_gDatum]) -> "_ModelTable[_gDatum]": ...
+    def __getitem__(self, query: type[_gDatum]) -> "ModelTable[_gDatum]": ...
 
     def __getitem__(
         self,
         query: type[_gDatum] | tuple[type[_gDatum], str | slice] | slice,
-    ) -> Union[_gDatum, "_ModelTable[_gDatum]", list[_gDatum]]:
+    ) -> Union[_gDatum, "ModelTable[_gDatum]", list[_gDatum]]:
         if isinstance(query, type):
-            return _ModelTable(self, query)
+            return ModelTable(self, query)
         elif isinstance(query, slice):
             table = cast(type[_gDatum], query.start)
             key = cast(str, query.stop)
         else:
             table, key_or_range = query
             if isinstance(key_or_range, slice):
                 if any([key_or_range.start, key_or_range.stop]):
@@ -112,15 +116,15 @@
         datum = self.get_datum(table, key)
         if datum is None:
             raise KeyError(f"Key {key} not found in table {table}")
 
         return datum
 
 
-class _ModelTable(Generic[_gDatum]):
+class ModelTable(Generic[_gDatum]):
     def __init__(self, kv_db: ModelDatabase, model: type[_gDatum]) -> None:
         self.kv_db = kv_db
         self.model = model
 
     @overload
     def __getitem__(self, key: str) -> _gDatum: ...
```

### Comparing `kvm_db-0.1.1/src/kvm_db/backends/base.py` & `kvm_db-0.1.2/src/kvm_db/backends/base.py`

 * *Files identical despite different names*

### Comparing `kvm_db-0.1.1/src/kvm_db/backends/sqlite.py` & `kvm_db-0.1.2/src/kvm_db/backends/sqlite.py`

 * *Files identical despite different names*

### Comparing `kvm_db-0.1.1/tests/test_kv_db.py` & `kvm_db-0.1.2/tests/test_kv_db.py`

 * *Files identical despite different names*

### Comparing `kvm_db-0.1.1/tests/test_model_db.py` & `kvm_db-0.1.2/tests/test_model_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import tempfile
 from collections.abc import Generator
 
 import pytest
 
 from kvm_db.backends.sqlite import Sqlite
-from kvm_db.model_db import ModelDatabase, TableModel, _ModelTable
+from kvm_db.model_db import ModelDatabase, ModelTable, TableModel
 
 
 class ExampleModel(TableModel):
     value: str
 
 
 @pytest.fixture
@@ -67,10 +67,10 @@
         model_db.get_datum(ExampleModel, "nonexistent_id")
 
 
 def test_model_table_access(model_db: ModelDatabase) -> None:
     model_instance = ExampleModel(value="For table access")
     model_db.insert(model_instance)
     model_table = model_db[ExampleModel]
-    assert isinstance(model_table, _ModelTable), "Should return an instance of _ModelTable."
+    assert isinstance(model_table, ModelTable), "Should return an instance of _ModelTable."
     retrieved_model = model_table[model_instance.id]
     assert retrieved_model.value == model_instance.value, "Should access and retrieve the correct model."
```

### Comparing `kvm_db-0.1.1/tests/backends/test_sqlite.py` & `kvm_db-0.1.2/tests/backends/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `kvm_db-0.1.1/README.md` & `kvm_db-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # kvm-db
 
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/kvm-db/0.1.1)](https://pypi.org/project/kvm-db/) [![PyPI version](https://badge.fury.io/py/kvm-db.svg)](https://badge.fury.io/py/kvm-db)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/kvm-db/0.1.2)](https://pypi.org/project/kvm-db/) [![PyPI version](https://badge.fury.io/py/kvm-db.svg)](https://badge.fury.io/py/kvm-db)
 
 kvm-db is a Python library that provides a simple yet powerful interface for both key-value storage and model-based data management using SQLite. Designed for ease of use, it allows developers to quickly implement robust data storage solutions.
 
 ## Features
 
 - Key-Value Store: Simple API for key-value data operations.
 - Model Database: Manage data using Python classes and objects.
@@ -22,14 +22,23 @@
 
 ```bash
 pip install kvm-db
 ```
 
 ## Quick Start
 
+You can retrieve the value using this syntax
+
+```python
+db[TABLE_NAME, KEY]
+# Or
+table_db = db[TABLE_NAME]
+table_db[KEY]
+```
+
 Below is a quick example to get you started with kvm-db.
 
 ### Key-Value Database Example
 
 ```python
 from kvm_db import KeyValDatabase, Sqlite
```

### Comparing `kvm_db-0.1.1/pyproject.toml` & `kvm_db-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kvm-db"
-version = "0.1.1"
+version = "0.1.2"
 description = "Key-Value&Model Database"
 authors = [
     { name = "Ja-sonYun", email = "killa30867@gmail.com" }
 ]
 dependencies = [
     "pydantic>=2.7.0",
 ]
```

### Comparing `kvm_db-0.1.1/PKG-INFO` & `kvm_db-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.3
 Name: kvm-db
-Version: 0.1.1
+Version: 0.1.2
 Summary: Key-Value&Model Database
 Project-URL: homepage, https://github.com/Ja-sonYun/kvm-db
 Project-URL: repository, https://github.com/Ja-sonYun/kvm-db
 Author-email: Ja-sonYun <killa30867@gmail.com>
 License-Expression: MIT
 Keywords: database,key-value,model,pydantic
 Requires-Python: >=3.9
 Requires-Dist: pydantic>=2.7.0
 Description-Content-Type: text/markdown
 
 # kvm-db
 
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/kvm-db/0.1.1)](https://pypi.org/project/kvm-db/) [![PyPI version](https://badge.fury.io/py/kvm-db.svg)](https://badge.fury.io/py/kvm-db)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/kvm-db/0.1.2)](https://pypi.org/project/kvm-db/) [![PyPI version](https://badge.fury.io/py/kvm-db.svg)](https://badge.fury.io/py/kvm-db)
 
 kvm-db is a Python library that provides a simple yet powerful interface for both key-value storage and model-based data management using SQLite. Designed for ease of use, it allows developers to quickly implement robust data storage solutions.
 
 ## Features
 
 - Key-Value Store: Simple API for key-value data operations.
 - Model Database: Manage data using Python classes and objects.
@@ -35,14 +35,23 @@
 
 ```bash
 pip install kvm-db
 ```
 
 ## Quick Start
 
+You can retrieve the value using this syntax
+
+```python
+db[TABLE_NAME, KEY]
+# Or
+table_db = db[TABLE_NAME]
+table_db[KEY]
+```
+
 Below is a quick example to get you started with kvm-db.
 
 ### Key-Value Database Example
 
 ```python
 from kvm_db import KeyValDatabase, Sqlite
```

