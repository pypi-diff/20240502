# Comparing `tmp/linkml_store-0.0.0.tar.gz` & `tmp/linkml_store-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml_store-0.0.0.tar", max compression
+gzip compressed data, was "linkml_store-0.1.6.tar", max compression
```

## Comparing `linkml_store-0.0.0.tar` & `linkml_store-0.1.6.tar`

### file list

```diff
@@ -1,28 +1,40 @@
--rw-r--r--   0        0        0     1086 2024-04-10 02:07:46.390570 linkml_store-0.0.0/LICENSE
--rw-r--r--   0        0        0      355 2024-04-10 02:07:46.390570 linkml_store-0.0.0/README.md
--rw-r--r--   0        0        0     3166 2024-04-10 02:07:46.398570 linkml_store-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      118 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/__init__.py
--rw-r--r--   0        0        0      284 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/api/__init__.py
--rw-r--r--   0        0        0     4353 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/api/client.py
--rw-r--r--   0        0        0    11334 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/api/collection.py
--rw-r--r--   0        0        0     6682 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/api/database.py
--rw-r--r--   0        0        0       69 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/api/metadata.py
--rw-r--r--   0        0        0     1698 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/api/queries.py
--rw-r--r--   0        0        0        0 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/api/stores/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/api/stores/duckdb/__init__.py
--rw-r--r--   0        0        0     4194 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/api/stores/duckdb/duckdb_collection.py
--rw-r--r--   0        0        0     6104 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/api/stores/duckdb/duckdb_database.py
--rw-r--r--   0        0        0      123 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/api/stores/duckdb/mappings.py
--rw-r--r--   0        0        0        0 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/api/stores/mongodb/__init__.py
--rw-r--r--   0        0        0     2094 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/api/stores/mongodb/mongodb_collection.py
--rw-r--r--   0        0        0     3984 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/api/stores/mongodb/mongodb_database.py
--rw-r--r--   0        0        0      112 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/constants.py
--rw-r--r--   0        0        0        0 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/index/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/index/implementations/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/index/implementations/llm_index.py
--rw-r--r--   0        0        0     1134 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/index/implementations/simple_index.py
--rw-r--r--   0        0        0     3420 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/index/index.py
--rw-r--r--   0        0        0        0 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/utils/__init__.py
--rw-r--r--   0        0        0      884 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/utils/io.py
--rw-r--r--   0        0        0     4557 2024-04-10 02:07:46.398570 linkml_store-0.0.0/src/linkml_store/utils/sql_utils.py
--rw-r--r--   0        0        0     1717 1970-01-01 00:00:00.000000 linkml_store-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-02 02:57:57.011154 linkml_store-0.1.6/LICENSE
+-rw-r--r--   0        0        0      451 2024-05-02 02:57:57.011154 linkml_store-0.1.6/README.md
+-rw-r--r--   0        0        0     3447 2024-05-02 02:58:24.819061 linkml_store-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      118 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/__init__.py
+-rw-r--r--   0        0        0      226 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/__init__.py
+-rw-r--r--   0        0        0     7551 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/client.py
+-rw-r--r--   0        0        0    17203 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/collection.py
+-rw-r--r--   0        0        0     3269 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/config.py
+-rw-r--r--   0        0        0    13701 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/database.py
+-rw-r--r--   0        0        0     2028 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/queries.py
+-rw-r--r--   0        0        0        0 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/stores/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/stores/chromadb/__init__.py
+-rw-r--r--   0        0        0     4186 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/stores/chromadb/chromadb_collection.py
+-rw-r--r--   0        0        0     3205 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/stores/chromadb/chromadb_database.py
+-rw-r--r--   0        0        0        0 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/stores/duckdb/__init__.py
+-rw-r--r--   0        0        0     5859 2024-05-02 02:57:57.019154 linkml_store-0.1.6/src/linkml_store/api/stores/duckdb/duckdb_collection.py
+-rw-r--r--   0        0        0     6591 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/duckdb/duckdb_database.py
+-rw-r--r--   0        0        0      123 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/duckdb/mappings.py
+-rw-r--r--   0        0        0        0 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/hdf5/__init__.py
+-rw-r--r--   0        0        0     3806 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/hdf5/hdf5_collection.py
+-rw-r--r--   0        0        0     2714 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/hdf5/hdf5_database.py
+-rw-r--r--   0        0        0        0 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/mongodb/__init__.py
+-rw-r--r--   0        0        0     3959 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/mongodb/mongodb_collection.py
+-rw-r--r--   0        0        0     3670 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/mongodb/mongodb_database.py
+-rw-r--r--   0        0        0     4723 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/solr/solr_collection.py
+-rw-r--r--   0        0        0     2876 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/solr/solr_database.py
+-rw-r--r--   0        0        0        0 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/api/stores/solr/solr_utils.py
+-rw-r--r--   0        0        0    13667 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/cli.py
+-rw-r--r--   0        0        0      112 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/constants.py
+-rw-r--r--   0        0        0      881 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/index/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/index/implementations/__init__.py
+-rw-r--r--   0        0        0     1069 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/index/implementations/llm_indexer.py
+-rw-r--r--   0        0        0     1251 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/index/implementations/simple_indexer.py
+-rw-r--r--   0        0        0     3462 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/index/indexer.py
+-rw-r--r--   0        0        0        0 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/utils/__init__.py
+-rw-r--r--   0        0        0     3081 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/utils/format_utils.py
+-rw-r--r--   0        0        0      884 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/utils/io.py
+-rw-r--r--   0        0        0     2214 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/utils/object_utils.py
+-rw-r--r--   0        0        0     5651 2024-05-02 02:57:57.023154 linkml_store-0.1.6/src/linkml_store/utils/sql_utils.py
+-rw-r--r--   0        0        0     2064 1970-01-01 00:00:00.000000 linkml_store-0.1.6/PKG-INFO
```

### Comparing `linkml_store-0.0.0/LICENSE` & `linkml_store-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `linkml_store-0.0.0/pyproject.toml` & `linkml_store-0.1.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 [tool.poetry]
 name = "linkml-store"
-version = "0.0.0"
+version = "0.1.6"
 description = "linkml-store"
 authors = ["Author 1 <author@org.org>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9, !=3.9.7"
 click = "*"
 pydantic = "^2.0.0"
 linkml-runtime = "^1.7.5"
 streamlit = { version = "^1.32.2", optional = true }
 sqlalchemy = "*"
 duckdb = "^0.10.1"
-duckdb-engine = "^0.11.2"
+duckdb-engine = ">=0.11.2"
 matplotlib = { version = "*", optional = true }
 seaborn = { version = "*", optional = true }
 plotly = { version = "*", optional = true }
 pystow = "^0.5.4"
 black = { version=">=24.0.0", optional = true }
 llm = { version="*", optional = true }
 pymongo = { version="*", optional = true }
-pandas = "^2.2.1"
+chromadb = { version="*", optional = true }
+h5py = { version="*", optional = true }
+linkml = { version="*", optional = true }
+linkml_map = { version="*", optional = true }
+pandas = ">=2.2.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = {version = ">=7.1.2"}
 tox = {version = ">=3.25.1"}
 pre-commit = {version = ">=3.3.3"}
 sphinx = {version = ">=6.1.3"}
 sphinx-rtd-theme = {version = ">=1.0.0"}
 sphinx-autodoc-typehints = {version = "<2.0.0"}
 sphinx-click = {version = ">=4.3.0"}
 myst-parser = {version = ">=0.18.1"}
+furo = {version = "*"}
 nbsphinx = "*"
 jupyter = "*"
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^7.4.0"
 pytest-subtests = "^0.11.0"
 numpy = [
@@ -46,17 +51,21 @@
 
 [tool.poetry.extras]
 analytics = ["pandas", "matplotlib", "seaborn", "plotly"]
 app = ["streamlit"]
 tests = ["black"]
 llm = ["llm"]
 mongodb = ["pymongo"]
+chromadb = ["chromadb"]
+h5py = ["h5py"]
+validation = ["linkml"]
+map = ["linkml_map"]
 
 [tool.poetry.scripts]
-linkml-store = "linkml_store.cli:main"
+linkml-store = "linkml_store.cli:cli"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "pep440"
 
 [tool.black]
```

### Comparing `linkml_store-0.0.0/src/linkml_store/api/collection.py` & `linkml_store-0.1.6/src/linkml_store/api/collection.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,124 @@
+import hashlib
 import logging
 from collections import defaultdict
-from dataclasses import dataclass
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, TextIO, Type, Union
+from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, TextIO, Type, Union
 
 import numpy as np
 from linkml_runtime.linkml_model import ClassDefinition, SlotDefinition
 from linkml_runtime.linkml_model.meta import ArrayExpression
 from pydantic import BaseModel
 
+from linkml_store.index import get_indexer
+
+try:
+    from linkml.validator.report import ValidationResult
+except ImportError:
+    ValidationResult = None
+
+from linkml_store.api.config import CollectionConfig
 from linkml_store.api.queries import Query, QueryResult
-from linkml_store.index.index import Index
+from linkml_store.index.indexer import Indexer
 
 if TYPE_CHECKING:
     from linkml_store.api.database import Database
 
 logger = logging.getLogger(__name__)
 
 OBJECT = Union[Dict[str, Any], BaseModel, Type]
 
+DEFAULT_FACET_LIMIT = 100
 IDENTIFIER = str
 FIELD_NAME = str
 
 
-@dataclass
 class Collection:
     """
     A collection is an organized set of objects of the same or similar type.
 
     - For relational databases, a collection is typically a table
     - For document databases such as MongoDB, a collection is the native type
     - For a file system, a collection could be a single tabular file such as Parquet or CSV
     """
 
-    name: str
+    # name: str
     parent: Optional["Database"] = None
-    _indexes: Optional[Dict[str, Index]] = None
-    hidden: Optional[bool] = False
+    _indexers: Optional[Dict[str, Indexer]] = None
+    # hidden: Optional[bool] = False
+
+    metadata: Optional[CollectionConfig] = None
+
+    def __init__(
+        self, name: str, parent: Optional["Database"] = None, metadata: Optional[CollectionConfig] = None, **kwargs
+    ):
+        self.parent = parent
+        if metadata:
+            self.metadata = metadata
+        else:
+            self.metadata = CollectionConfig(name=name, **kwargs)
+        if name is not None and self.metadata.name is not None and name != self.metadata.name:
+            raise ValueError(f"Name mismatch: {name} != {self.metadata.name}")
+
+    @property
+    def name(self) -> str:
+        return self.metadata.name
+
+    @property
+    def hidden(self) -> bool:
+        return self.metadata.hidden
+
+    @property
+    def _target_class_name(self):
+        """
+        Return the name of the class that this collection represents
+
+        This MUST be a LinkML class name
+
+        :return:
+        """
+        # TODO: this is a shim layer until we can normalize on this
+        if self.metadata.type:
+            return self.metadata.type
+        return self.name
+
+    @property
+    def _alias(self):
+        """
+        Return the primary name/alias used for the collection.
+
+        This MAY be the name of the LinkML class, but it may be desirable
+        to have an alias, for example "persons" which collects all instances
+        of class Person.
+
+        The _alias SHOULD be used for Table names in SQL.
+
+        For nested data, the alias SHOULD be used as the key; e.g
+
+         ``{ "persons": [ { "name": "Alice" }, { "name": "Bob" } ] }``
+
+        :return:
+        """
+        # TODO: this is a shim layer until we can normalize on this
+        if self.metadata.alias:
+            return self.metadata.alias
+        return self.name
+
+    def replace(self, objs: Union[OBJECT, List[OBJECT]], **kwargs):
+        """
+        Replace entire collection with objects.
+
+        :param objs:
+        :param kwargs:
+        :return:
+        """
+        self.delete_where({})
+        self.insert(objs, **kwargs)
 
-    def add(self, objs: Union[OBJECT, List[OBJECT]], **kwargs):
+    def insert(self, objs: Union[OBJECT, List[OBJECT]], **kwargs):
         """
         Add one or more objects to the collection
 
         :param objs:
         :param kwargs:
         :return:
         """
@@ -54,48 +130,51 @@
 
         :param objs:
         :param kwargs:
         :return:
         """
         raise NotImplementedError
 
-    def delete_where(self, where: Optional[Dict[str, Any]] = None, **kwargs) -> int:
+    def delete_where(self, where: Optional[Dict[str, Any]] = None, missing_ok=True, **kwargs) -> int:
         """
         Delete objects that match a query
 
-        :param where:
+        :param where: where conditions
+        :param missing_ok: if True, do not raise an error if the collection does not exist
         :param kwargs:
-        :return:
+        :return: number of objects deleted (or -1 if unsupported)
         """
         raise NotImplementedError
 
     def update(self, objs: Union[OBJECT, List[OBJECT]], **kwargs):
         """
         Update one or more objects in the collection
 
         :param objs:
         :param kwargs:
         :return:
         """
         raise NotImplementedError
 
     def _create_query(self, **kwargs) -> Query:
-        return Query(from_table=self.name, **kwargs)
+        return Query(from_table=self._alias, **kwargs)
 
     def query(self, query: Query, **kwargs) -> QueryResult:
         """
         Run a query against the collection
 
         :param query:
         :param kwargs:
         :return:
         """
         return self.parent.query(query, **kwargs)
 
-    def query_facets(self, where: Optional[Dict] = None, facet_columns: List[str] = None) -> Dict[str, Dict[str, int]]:
+    def query_facets(
+        self, where: Optional[Dict] = None, facet_columns: List[str] = None, facet_limit=DEFAULT_FACET_LIMIT, **kwargs
+    ) -> Dict[str, Dict[str, int]]:
         """
         Run a query to get facet counts for one or more columns.
 
         This function takes a database connection, a Query object, and a list of column names.
         It generates and executes a facet count query for each specified column and returns
         the results as a dictionary where the keys are the column names and the values are
         pandas DataFrames containing the facet counts.
@@ -104,25 +183,40 @@
         to exclude conditions directly related to the facet column. This allows for counting
         the occurrences of each unique value in the facet column while still applying the
         other filtering conditions.
 
         :param con: A DuckDB database connection.
         :param query: A Query object representing the base query.
         :param facet_columns: A list of column names to get facet counts for.
+        :param facet_limit:
         :return: A dictionary where keys are column names and values are pandas DataFrames
                  containing the facet counts for each unique value in the respective column.
         """
         raise NotImplementedError
 
     def get(self, ids: Optional[IDENTIFIER], **kwargs) -> QueryResult:
+        """
+        Get one or more objects by ID.
+
+        :param ids:
+        :param kwargs:
+        :return:
+        """
         id_field = self.identifier_field
         q = self._create_query(where_clause={id_field: ids})
         return self.query(q, **kwargs)
 
     def find(self, where: Optional[Any] = None, **kwargs) -> QueryResult:
+        """
+        Find objects in the collection using a where query.
+
+        :param where:
+        :param kwargs:
+        :return:
+        """
         query = self._create_query(where_clause=where)
         return self.query(query, **kwargs)
 
     def search(
         self,
         query: str,
         where: Optional[Any] = None,
@@ -137,113 +231,191 @@
         :param where:
         :param index_name:
         :param limit:
         :param kwargs:
         :return:
         """
         if index_name is None:
-            if len(self._indexes) == 1:
-                index_name = list(self._indexes.keys())[0]
+            if len(self._indexers) == 1:
+                index_name = list(self._indexers.keys())[0]
             else:
                 raise ValueError("Multiple indexes found. Please specify an index name.")
         ix_coll = self.parent.get_collection(self._index_collection_name(index_name))
-        ix = self._indexes.get(index_name)
+        ix = self._indexers.get(index_name)
         if not ix:
             raise ValueError(f"No index named {index_name}")
         qr = ix_coll.find(where=where, limit=-1, **kwargs)
         index_col = ix.index_field
         vector_pairs = [(row, np.array(row[index_col], dtype=float)) for row in qr.rows]
         results = ix.search(query, vector_pairs, limit=limit)
+        for r in results:
+            del r[1][index_col]
         new_qr = QueryResult(num_rows=len(results))
         new_qr.ranked_rows = results
         return new_qr
 
-    def attach_index(self, index: Index, auto_index=True, **kwargs):
+    @property
+    def is_internal(self) -> bool:
+        """
+        Check if the collection is internal
+
+        :return:
+        """
+        if not self.name:
+            raise ValueError(f"Collection has no name: {self} // {self.metadata}")
+        return self.name.startswith("internal__")
+
+    def attach_indexer(self, index: Union[Indexer, str], name: Optional[str] = True, auto_index=True, **kwargs):
         """
         Attach an index to the collection.
 
         :param index:
-        :param auto_index:
+        :param name:
+        :param auto_index: Automatically index all objects in the collection
         :param kwargs:
         :return:
         """
+        if isinstance(index, str):
+            index = get_indexer(index)
+        if name:
+            index.name = name
+        if not index.name:
+            index.name = type(index).__name__.lower()
         index_name = index.name
         if not index_name:
             raise ValueError("Index must have a name")
-        if not self._indexes:
-            self._indexes = {}
-        self._indexes[index_name] = index
+        if not self._indexers:
+            self._indexers = {}
+        self._indexers[index_name] = index
         if auto_index:
             all_objs = self.find(limit=-1).rows
-            self.index_objects(all_objs, index_name, **kwargs)
+            self.index_objects(all_objs, index_name, replace=True, **kwargs)
 
     def _index_collection_name(self, index_name: str) -> str:
-        return f"index__{self.name}_{index_name}"
+        """
+        Create a name for a special collection that holds index data
+
+        :param index_name:
+        :return:
+        """
+        return f"internal__index__{self.name}__{index_name}"
 
-    def index_objects(self, objs: List[OBJECT], index_name: str, **kwargs):
+    def index_objects(self, objs: List[OBJECT], index_name: str, replace=False, **kwargs):
         """
         Index a list of objects
 
         :param objs:
         :param index_name:
+        :param replace:
         :param kwargs:
         :return:
         """
-        ix = self._indexes.get(index_name)
+        ix = self._indexers.get(index_name)
         if not ix:
             raise ValueError(f"No index named {index_name}")
-        ix_coll = self.parent.get_collection(self._index_collection_name(index_name), create_if_not_exists=True)
+        ix_coll_name = self._index_collection_name(index_name)
+        ix_coll = self.parent.get_collection(ix_coll_name, create_if_not_exists=True)
         vectors = [list(float(e) for e in v) for v in ix.objects_to_vectors(objs)]
         objects_with_ix = []
         index_col = ix.index_field
         for obj, vector in zip(objs, vectors):
             # TODO: id field
             objects_with_ix.append({**obj, **{index_col: vector}})
-        ix_coll.add(objects_with_ix, **kwargs)
+        if replace:
+            schema = self.parent.schema_view.schema
+            logger.info(f"Checking if {ix_coll_name} is in {schema.classes.keys()}")
+            if ix_coll_name in schema.classes:
+                ix_coll.delete_where()
+        ix_coll.insert(objects_with_ix, **kwargs)
+
+    def list_index_names(self) -> List[str]:
+        """
+        Return a list of index names
+
+        :return:
+        """
+        return list(self._indexers.keys())
+
+    @property
+    def indexers(self) -> Dict[str, Indexer]:
+        """
+        Return a list of indexers
+
+        :return:
+        """
+        return self._indexers if self._indexers else {}
 
     def peek(self, limit: Optional[int] = None) -> QueryResult:
+        """
+        Return the first N objects in the collection
+
+        :param limit:
+        :return:
+        """
         q = self._create_query()
         return self.query(q, limit=limit)
 
     def class_definition(self) -> Optional[ClassDefinition]:
         """
         Return the class definition for the collection.
 
         :return:
         """
         sv = self.parent.schema_view
         if sv:
-            return sv.get_class(self.name)
+            cls = sv.get_class(self._target_class_name)
+            return cls
         return None
 
     def identifier_attribute_name(self) -> Optional[str]:
         """
         Return the name of the identifier attribute for the collection.
 
+        AKA the primary key.
+
         :return: The name of the identifier attribute, if one exists.
         """
         cd = self.class_definition()
         if cd:
             for att in cd.attributes.values():
                 if att.identifier:
                     return att.name
         return None
 
+    def object_identifier(self, obj: OBJECT, auto=True) -> Optional[IDENTIFIER]:
+        """
+        Return the identifier for an object.
+
+        :param obj:
+        :param auto: If True, generate an identifier if one does not exist.
+        :return:
+        """
+        pk = self.identifier_attribute_name
+        if pk in obj:
+            return obj[pk]
+        elif auto:
+            # TODO: use other unique keys if no primary key
+            as_str = str(obj)
+            md5 = hashlib.md5(as_str.encode()).hexdigest()
+            return md5
+        else:
+            return None
+
     def induce_class_definition_from_objects(self, objs: List[OBJECT], max_sample_size=10) -> ClassDefinition:
         """
         Induce a class definition from a list of objects.
 
         This uses a heuristic procedure to infer the class definition from a list of objects.
         In general it is recommended you explicitly provide a schema.
 
         :param objs:
         :param max_sample_size:
         :return:
         """
-        cd = ClassDefinition(self.name)
+        cd = ClassDefinition(self._target_class_name)
         keys = defaultdict(list)
         for obj in objs[0:max_sample_size]:
             if isinstance(obj, BaseModel):
                 obj = obj.model_dump()
             if not isinstance(obj, dict):
                 logger.warning(f"Skipping non-dict object: {obj}")
                 continue
@@ -298,15 +470,15 @@
                 if rng != other_rng:
                     raise ValueError(f"Conflict: {rng} != {other_rng} for {vs}")
             cd.attributes[k] = SlotDefinition(k, range=rng, multivalued=multivalued, inlined=inlined)
             if exact_dimensions_list:
                 array_expr = ArrayExpression(exact_number_dimensions=len(exact_dimensions_list[0]))
                 cd.attributes[k].array = array_expr
         sv = self.parent.schema_view
-        sv.schema.classes[self.name] = cd
+        sv.schema.classes[self._target_class_name] = cd
         sv.set_modified()
         return cd
 
     def import_data(self, location: Union[Path, str, TextIO], **kwargs):
         """
         Import data from a file or stream
 
@@ -321,7 +493,26 @@
         Export data to a file or stream
 
         :param location:
         :param kwargs:
         :return:
         """
         raise NotImplementedError
+
+    def iter_validate_collection(self, **kwargs) -> Iterator["ValidationResult"]:
+        """
+        Validate the contents of the collection
+
+        :param kwargs:
+        :return: iterator over validation results
+        """
+        from linkml.validator import JsonschemaValidationPlugin, Validator
+
+        validation_plugins = [JsonschemaValidationPlugin(closed=True)]
+        validator = Validator(self.parent.schema_view.schema, validation_plugins=validation_plugins)
+        cd = self.class_definition()
+        if not cd:
+            raise ValueError(f"Cannot find class definition for {self._target_class_name}")
+        class_name = cd.name
+        result = self.find(**kwargs)
+        for obj in result.rows:
+            yield from validator.iter_results(obj, class_name)
```

### Comparing `linkml_store-0.0.0/src/linkml_store/api/queries.py` & `linkml_store-0.1.6/src/linkml_store/api/queries.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,37 +18,48 @@
     A query object.
 
     - In SQL this would be a SQL query string
     """
 
     from_table: Optional[str]
     select_cols: Optional[List[str]] = None
-    where_clause: Optional[Union[str, List[str], Dict[str, str]]] = None
+    where_clause: Optional[Union[str, List[str], Dict[str, Any]]] = None
     sort_by: Optional[List[str]] = None
     limit: Optional[int] = None
     offset: Optional[int] = None
     include_facet_counts: bool = False
     facet_slots: Optional[List[str]] = None
 
 
+class FacetCountResult(BaseModel):
+    """
+    A facet count result
+    """
+
+    as_dict: Dict[FACET_GROUP, List[Tuple[FACET_GROUP, int]]]
+
+
 class QueryResult(BaseModel):
     """
     A query result
     """
 
     query: Optional[Query] = None
+    search_term: Optional[str] = None
     num_rows: int
     offset: Optional[int] = 0
     rows: Optional[List[Dict[str, Any]]] = None
     ranked_rows: Optional[List[Tuple[float, Dict[str, Any]]]] = None
     _rows_dataframe: Optional[pd.DataFrame] = None
     facet_counts: Optional[Dict[str, List[Tuple[FACET_GROUP, int]]]] = None
 
     @property
     def rows_dataframe(self) -> pd.DataFrame:
+        if self.ranked_rows is not None:
+            self._rows_dataframe = pd.DataFrame([{"score": score, **row} for score, row in self.ranked_rows])
         if self._rows_dataframe is None and self.rows:
             self._rows_dataframe = pd.DataFrame(self.rows)
         return self._rows_dataframe
 
     def set_rows(self, rows: pd.DataFrame):
         self._rows_dataframe = rows
```

### Comparing `linkml_store-0.0.0/src/linkml_store/api/stores/duckdb/duckdb_database.py` & `linkml_store-0.1.6/src/linkml_store/api/stores/duckdb/duckdb_database.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,89 +1,78 @@
 import json
 import logging
-from dataclasses import dataclass
 from typing import Optional
 
 import pandas as pd
 import sqlalchemy
 from duckdb import DuckDBPyConnection
 from linkml_runtime import SchemaView
-from linkml_runtime.linkml_model import SlotDefinition
+from linkml_runtime.linkml_model import ClassDefinition, SlotDefinition
 from linkml_runtime.utils.schema_builder import SchemaBuilder
-from sqlalchemy import text
+from sqlalchemy import NullPool, text
 
 from linkml_store.api import Database
 from linkml_store.api.queries import Query, QueryResult
 from linkml_store.api.stores.duckdb.duckdb_collection import DuckDBCollection
 from linkml_store.utils.sql_utils import introspect_schema, query_to_sql
 
 TYPE_MAP = {
     "VARCHAR": "string",
     "BIGINT": "integer",
     "BOOLEAN": "boolean",
+    "DATE": "date",
+    "DOUBLE": "float",
+    "INTEGER": "integer",
 }
 
 
 logger = logging.getLogger(__name__)
 
 
-def run_query(con: DuckDBPyConnection, query: Query, **kwargs):
-    """
-    Run a query and return the result.
-
-    >>> import duckdb
-    >>> con = duckdb.connect("db/mgi.db")
-    >>> query = Query(from_table="gaf_association", limit=5)
-    >>> result = run_query(con, query)
-    >>> print(result.num_rows)
-    532233
-
-    :param con:
-    :param query:
-    :return:
-    """
-    count_query_str = query_to_sql(query, count=True)
-    num_rows = con.execute(count_query_str).fetchall()[0][0]
-    logger.debug(f"num_rows: {num_rows}")
-    query_str = query_to_sql(query, **kwargs)
-    logger.debug(f"query_str: {query_str}")
-    rows = con.execute(query_str).fetchdf()
-    qr = QueryResult(query=query, num_rows=num_rows)
-    qr.set_rows(rows)
-    return qr
-
-
-@dataclass
 class DuckDBDatabase(Database):
     _connection: DuckDBPyConnection = None
     _engine: sqlalchemy.Engine = None
+    collection_class = DuckDBCollection
 
-    def __post_init__(self):
-        if not self.handle:
-            self.handle = "duckdb:///:memory:"
+    def __init__(self, handle: Optional[str] = None, **kwargs):
+        if handle is None:
+            handle = "duckdb:///:memory:"
+        super().__init__(handle=handle, **kwargs)
 
     @property
     def engine(self) -> sqlalchemy.Engine:
         if not self._engine:
             handle = self.handle
             if not handle.startswith("duckdb://") and not handle.startswith(":"):
-                handle = f"duckdb://{handle}"
-            self._engine = sqlalchemy.create_engine(handle)
+                handle = f"duckdb:///{handle}"
+            if ":memory:" not in handle:
+                # TODO: investigate this; duckdb appears to be prematurely caching
+                self._engine = sqlalchemy.create_engine(handle, poolclass=NullPool)
+            else:
+                self._engine = sqlalchemy.create_engine(handle)
         return self._engine
 
     def commit(self, **kwargs):
         with self.engine.connect() as conn:
             conn.commit()
 
     def close(self, **kwargs):
         self.engine.dispose()
 
     def query(self, query: Query, **kwargs) -> QueryResult:
         json_encoded_cols = []
         if query.from_table:
+            if not query.from_table.startswith("information_schema"):
+                meta_query = Query(
+                    from_table="information_schema.tables", where_clause={"table_name": query.from_table}
+                )
+                qr = self.query(meta_query)
+                if qr.num_rows == 0:
+                    logger.debug(f"Table {query.from_table} not created yet")
+                    return QueryResult(query=query, num_rows=0, rows=[])
             sv = self._schema_view
             if sv:
                 cd = None
                 for c in self._collections.values():
                     if c.name == query.from_table:
                         cd = c.class_definition()
                         break
@@ -123,29 +112,23 @@
         if self._collections is None:
             self._collections = {}
         for table_name in table_names:
             if table_name not in self._collections:
                 collection = DuckDBCollection(name=table_name, parent=self)
                 self._collections[table_name] = collection
 
-    def create_collection(self, name: str, alias: Optional[str] = None, **kwargs) -> DuckDBCollection:
-        collection = DuckDBCollection(name=name, parent=self)
-        if not self._collections:
-            self._collections = {}
-        if not alias:
-            alias = name
-        self._collections[alias] = collection
-        return collection
-
     def induce_schema_view(self) -> SchemaView:
         # TODO: unify schema introspection
+        # TODO: handle case where schema is provided in advance
+        logger.info(f"Inducing schema view for {self.metadata.handle}")
         sb = SchemaBuilder()
         schema = sb.schema
         query = Query(from_table="information_schema.tables", where_clause={"table_type": "BASE TABLE"})
         qr = self.query(query)
+        logger.info(f"Found {qr.num_rows} information_schema.tables // {qr.rows}")
         if qr.num_rows:
             table_names = [row["table_name"] for row in qr.rows]
             for tbl in table_names:
                 sb.add_class(tbl)
         query = Query(from_table="information_schema.columns", sort_by=["ordinal_position"])
         for row in self.query(query, limit=-1).rows:
             tbl_name = row["table_name"]
@@ -158,9 +141,17 @@
             else:
                 multivalued = False
             rng = TYPE_MAP.get(dt, "string")
             sd = SlotDefinition(
                 row["column_name"], required=row["is_nullable"] == "NO", multivalued=multivalued, range=rng
             )
             sb.schema.classes[tbl_name].attributes[sd.name] = sd
+            logger.info(f"Introspected slot: {tbl_name}.{sd.name}: {sd.range}")
         sb.add_defaults()
+        for cls_name in schema.classes:
+            if cls_name in self.metadata.collections:
+                collection_metadata = self.metadata.collections[cls_name]
+                if collection_metadata.attributes:
+                    del schema.classes[cls_name]
+                    cls = ClassDefinition(name=collection_metadata.type, attributes=collection_metadata.attributes)
+                    schema.classes[cls.name] = cls
         return SchemaView(schema)
```

### Comparing `linkml_store-0.0.0/src/linkml_store/api/stores/mongodb/mongodb_collection.py` & `linkml_store-0.1.6/src/linkml_store/api/stores/hdf5/hdf5_database.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,79 @@
-from dataclasses import dataclass
-from typing import Any, Dict, List, Optional, Union
+# hdf5_database.py
 
-from linkml_store.api import Collection
-from linkml_store.api.collection import OBJECT
+import logging
+from typing import Optional
 
+import h5py
+from linkml_runtime import SchemaView
+from linkml_runtime.linkml_model import ClassDefinition, SlotDefinition
+from linkml_runtime.utils.schema_builder import SchemaBuilder
+
+from linkml_store.api import Database
+from linkml_store.api.queries import Query, QueryResult
+from linkml_store.api.stores.hdf5.hdf5_collection import HDF5Collection
+
+logger = logging.getLogger(__name__)
+
+
+class HDF5Database(Database):
+    _file: h5py.File = None
+    collection_class = HDF5Collection
+
+    def __init__(self, handle: Optional[str] = None, **kwargs):
+        if handle is None:
+            handle = "linkml_store.h5"
+        super().__init__(handle=handle, **kwargs)
+
+    @property
+    def file(self) -> h5py.File:
+        if self._file is None:
+            self._file = h5py.File(self.handle, "a")
+        return self._file
+
+    def commit(self, **kwargs):
+        self.file.flush()
+
+    def close(self, **kwargs):
+        if self._file:
+            self._file.close()
+
+    def query(self, query: Query, **kwargs) -> QueryResult:
+        if query.from_table:
+            collection = self.get_collection(query.from_table)
+            return collection.query(query, **kwargs)
+
+    def init_collections(self):
+        if self._collections is None:
+            self._collections = {}
+
+        for collection_name in self.file:
+            if collection_name not in self._collections:
+                collection = HDF5Collection(name=collection_name, parent=self)
+                self._collections[collection_name] = collection
+
+    def induce_schema_view(self) -> SchemaView:
+        logger.info(f"Inducing schema view for {self.handle}")
+        sb = SchemaBuilder()
+        schema = sb.schema
+
+        for collection_name in self.file:
+            sb.add_class(collection_name)
+            hdf5_group = self.file[collection_name]
+            for field in hdf5_group:
+                if field == "_id":
+                    continue
+                sd = SlotDefinition(field)
+                if isinstance(hdf5_group[field][()], list):
+                    sd.multivalued = True
+                sb.schema.classes[collection_name].attributes[sd.name] = sd
+
+        sb.add_defaults()
+        for cls_name in schema.classes:
+            if cls_name in self.metadata.collections:
+                collection_metadata = self.metadata.collections[cls_name]
+                if collection_metadata.attributes:
+                    del schema.classes[cls_name]
+                    cls = ClassDefinition(name=collection_metadata.type, attributes=collection_metadata.attributes)
+                    schema.classes[cls.name] = cls
 
-@dataclass
-class MongoDBCollection(Collection):
-    """
-    A wrapper around a MongoDB collection
-    """
-
-    def add(self, objs: Union[OBJECT, List[OBJECT]], **kwargs):
-        if not isinstance(objs, list):
-            objs = [objs]
-        if not objs:
-            return
-        cd = self.class_definition()
-        if not cd:
-            cd = self.induce_class_definition_from_objects(objs)
-        collection = self.parent.database[self.name]
-        collection.insert_many(objs)
-
-    def delete(self, objs: Union[OBJECT, List[OBJECT]], **kwargs) -> int:
-        if not isinstance(objs, list):
-            objs = [objs]
-        cd = self.class_definition()
-        if not cd:
-            cd = self.induce_class_definition_from_objects(objs)
-        collection = self.parent.database[self.name]
-        deleted_count = 0
-        for obj in objs:
-            result = collection.delete_one(obj)
-            deleted_count += result.deleted_count
-        return deleted_count
-
-    def delete_where(self, where: Optional[Dict[str, Any]] = None, **kwargs) -> int:
-        collection = self.parent.database[self.name]
-        result = collection.delete_many(where)
-        return result.deleted_count
-
-    def query_facets(self, where: Dict = None, facet_columns: List[str] = None) -> Dict[str, Dict[str, int]]:
-        results = {}
-        _cd = self.class_definition()
-        collection = self.parent.database[self.name]
-        if not facet_columns:
-            facet_columns = list(self.class_definition().attributes.keys())
-        for col in facet_columns:
-            facet_pipeline = [
-                {"$match": where} if where else {"$match": {}},
-                {"$group": {"_id": f"${col}", "count": {"$sum": 1}}},
-            ]
-            facet_results = list(collection.aggregate(facet_pipeline))
-            results[col] = [(row["_id"], row["count"]) for row in facet_results]
-        return results
+        return SchemaView(schema)
```

### Comparing `linkml_store-0.0.0/src/linkml_store/api/stores/mongodb/mongodb_database.py` & `linkml_store-0.1.6/src/linkml_store/api/stores/mongodb/mongodb_database.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,112 +1,103 @@
-from dataclasses import dataclass
+# mongodb_database.py
+
+import logging
 from typing import Optional
 
 from linkml_runtime import SchemaView
-from linkml_runtime.linkml_model import SlotDefinition
+from linkml_runtime.linkml_model import ClassDefinition, SlotDefinition
 from linkml_runtime.utils.schema_builder import SchemaBuilder
 from pymongo import MongoClient
+from pymongo.database import Database as NativeDatabase
 
 from linkml_store.api import Database
 from linkml_store.api.queries import Query, QueryResult
 from linkml_store.api.stores.mongodb.mongodb_collection import MongoDBCollection
 
+logger = logging.getLogger(__name__)
+
 
-@dataclass
 class MongoDBDatabase(Database):
     """
-    A wrapper around a MongoDB database
-    """
+    An adapter for MongoDB databases.
 
-    _client: MongoClient = None
-    _database = None
+    The LinkML-Store Database abstraction combines mongodb Client and Database.
+    """
 
-    def __post_init__(self):
-        if not self.handle:
-            self.handle = "mongodb://localhost:27017"
+    _native_client: MongoClient = None
+    _native_db = None
+    collection_class = MongoDBCollection
+
+    def __init__(self, handle: Optional[str] = None, **kwargs):
+        if handle is None:
+            handle = "mongodb://localhost:27017"
+        super().__init__(handle=handle, **kwargs)
 
     @property
-    def client(self) -> MongoClient:
-        if not self._client:
-            self._client = MongoClient(self.handle)
-        return self._client
+    def native_client(self) -> MongoClient:
+        if self._native_client is None:
+            self._native_client = MongoClient(self.handle)
+        return self._native_client
 
     @property
-    def database(self):
-        if not self._database:
-            db_name = self.handle.split("/")[-1]
-            self._database = self.client[db_name]
-        return self._database
+    def native_db(self) -> NativeDatabase:
+        if self._native_db is None:
+            alias = self.metadata.alias
+            if not alias:
+                alias = "default"
+            self._native_db = self.native_client[alias]
+        return self._native_db
 
     def commit(self, **kwargs):
         pass
 
     def close(self, **kwargs):
-        self.client.close()
+        if self._native_client:
+            self._native_client.close()
+
+    def drop(self, **kwargs):
+        self.native_client.drop_database(self.metadata.alias)
 
     def query(self, query: Query, **kwargs) -> QueryResult:
-        collection = self.database[query.from_table]
-        where_clause = query.where_clause or {}
-        cursor = collection.find(where_clause)
-        if query.limit:
-            cursor = cursor.limit(query.limit)
-        if query.offset:
-            cursor = cursor.skip(query.offset)
-        if query.sort_by:
-            sort_key = [(col, 1) for col in query.sort_by]
-            cursor = cursor.sort(sort_key)
-        rows = list(cursor)
-        num_rows = len(rows)
-        qr = QueryResult(query=query, num_rows=num_rows, rows=rows)
-        return qr
+        if query.from_table:
+            collection = self.get_collection(query.from_table)
+            return collection.query(query, **kwargs)
 
     def init_collections(self):
         if self._collections is None:
             self._collections = {}
-        for collection_name in self.database.list_collection_names():
+
+        for collection_name in self.native_db.list_collection_names():
             if collection_name not in self._collections:
                 collection = MongoDBCollection(name=collection_name, parent=self)
                 self._collections[collection_name] = collection
 
-    def create_collection(self, name: str, alias: Optional[str] = None, **kwargs) -> MongoDBCollection:
-        collection = MongoDBCollection(name=name, parent=self)
-        if not self._collections:
-            self._collections = {}
-        if not alias:
-            alias = name
-        self._collections[alias] = collection
-        return collection
-
     def induce_schema_view(self) -> SchemaView:
+        logger.info(f"Inducing schema view for {self.handle}")
         sb = SchemaBuilder()
         schema = sb.schema
-        collection_names = self.database.list_collection_names()
-        for collection_name in collection_names:
+
+        for collection_name in self.native_db.list_collection_names():
             sb.add_class(collection_name)
-            collection = self.database[collection_name]
-            sample_doc = collection.find_one()
+            mongo_collection = self.native_db[collection_name]
+            sample_doc = mongo_collection.find_one()
             if sample_doc:
-                for key, value in sample_doc.items():
-                    if key == "_id":
+                for field, value in sample_doc.items():
+                    if field == "_id":
                         continue
+                    sd = SlotDefinition(field)
                     if isinstance(value, list):
-                        multivalued = True
-                        if value:
-                            value = value[0]
-                        else:
-                            value = None
-                    else:
-                        multivalued = False
-                    if isinstance(value, str):
-                        rng = "string"
-                    elif isinstance(value, int):
-                        rng = "integer"
-                    elif isinstance(value, float):
-                        rng = "float"
-                    elif isinstance(value, bool):
-                        rng = "boolean"
-                    else:
-                        rng = "string"
-                    sd = SlotDefinition(key, range=rng, multivalued=multivalued)
+                        sd.multivalued = True
+                    if isinstance(value, dict):
+                        sd.inlined = True
                     sb.schema.classes[collection_name].attributes[sd.name] = sd
+
         sb.add_defaults()
+        for cls_name in schema.classes:
+            if cls_name in self.metadata.collections:
+                collection_metadata = self.metadata.collections[cls_name]
+                if collection_metadata.attributes:
+                    del schema.classes[cls_name]
+                    cls = ClassDefinition(name=collection_metadata.type, attributes=collection_metadata.attributes)
+                    schema.classes[cls.name] = cls
+
         return SchemaView(schema)
```

### Comparing `linkml_store-0.0.0/src/linkml_store/index/implementations/llm_index.py` & `linkml_store-0.1.6/src/linkml_store/index/implementations/llm_indexer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import TYPE_CHECKING, List
 
 import numpy as np
 
-from linkml_store.index.index import INDEX_ITEM, Index
+from linkml_store.index.indexer import INDEX_ITEM, Indexer
 
 if TYPE_CHECKING:
     import llm
 
 
-class LLMIndex(Index):
+class LLMIndexer(Indexer):
     """
     A implementations index wraps the llm library
     """
 
     embedding_model_name: str = "ada-002"
     _embedding_model: "llm.EmbeddingModel" = None
```

### Comparing `linkml_store-0.0.0/src/linkml_store/index/implementations/simple_index.py` & `linkml_store-0.1.6/src/linkml_store/index/implementations/simple_indexer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import hashlib
+import logging
 
 import numpy as np
 
-from linkml_store.index.index import INDEX_ITEM, Index
+from linkml_store.index.indexer import INDEX_ITEM, Indexer
 
+logger = logging.getLogger(__name__)
 
-class SimpleIndex(Index):
+
+class SimpleIndexer(Indexer):
     """
     A implementations index that uses a hash function to generate an index from text.
 
     This uses a naive method to generate an index from text. It is not suitable for production use.
     """
 
     def text_to_vector(self, text: str) -> INDEX_ITEM:
@@ -32,9 +35,9 @@
             hash_value = int(hashlib.sha1(word.encode("utf-8")).hexdigest(), 16)
 
             # Compute the index in the vector using modulo
             index = hash_value % vector_length
 
             # Increment the count at the computed index
             vector[index] += 1.0
-
+        logger.info(f"Indexed text: {text} as {vector}")
         return vector
```

### Comparing `linkml_store-0.0.0/src/linkml_store/index/index.py` & `linkml_store-0.1.6/src/linkml_store/index/indexer.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def cosine_similarity(vector1, vector2):
     dot_product = np.dot(vector1, vector2)
     norm1 = np.linalg.norm(vector1)
     norm2 = np.linalg.norm(vector2)
     return dot_product / (norm1 * norm2)
 
 
-class Index(BaseModel):
+class Indexer(BaseModel):
     """
     An index operates on a collection in order to search for objects.
     """
 
     name: Optional[str] = None
     index_function: Optional[Callable] = None
     distance_function: Optional[Callable] = None
@@ -61,34 +61,37 @@
         :param text:
         :return:
         """
         raise NotImplementedError
 
     def object_to_text(self, obj: Dict[str, Any]) -> str:
         """
-        Create a text from an object suitable for indexing.
+        Convert an object to a text representation
+
+        :param obj:
+        :return:
         """
         if self.index_attributes:
             obj = {k: v for k, v in obj.items() if k in self.index_attributes}
         if self.filter_nulls:
             obj = {k: v for k, v in obj.items() if v is not None}
         if self.text_template:
             return self.text_template.format(**obj)
         return str(obj)
 
     def search(
         self, query: str, vectors: List[Tuple[str, INDEX_ITEM]], limit: Optional[int] = None
-    ) -> List[Tuple[float, str]]:
+    ) -> List[Tuple[float, Any]]:
         """
         Search the index for a query string
 
         :param query: The query string to search for
         :param vectors: A list of indexed items, where each item is a tuple of (id, vector)
         :param limit: The maximum number of results to return (optional)
-        :return: A list of item IDs that match the query
+        :return: A list of item IDs or objects that match the query
         """
 
         # Convert the query string to a vector
         query_vector = self.text_to_vector(query)
 
         distances = []
```

### Comparing `linkml_store-0.0.0/src/linkml_store/utils/io.py` & `linkml_store-0.1.6/src/linkml_store/utils/io.py`

 * *Files identical despite different names*

### Comparing `linkml_store-0.0.0/src/linkml_store/utils/sql_utils.py` & `linkml_store-0.1.6/src/linkml_store/utils/sql_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Optional, Tuple, Type, Union
+from typing import Any, Optional, Tuple, Type, Union
 
 import sqlalchemy
 import sqlalchemy.sql.sqltypes as sqlt
 from linkml_runtime.linkml_model import SchemaDefinition, SlotDefinition
 from linkml_runtime.utils.schema_builder import SchemaBuilder
 from sqlalchemy import MetaData
 
@@ -13,14 +13,20 @@
 
 TYPE_MAP = {
     sqlt.TEXT: "string",
     sqlt.INTEGER: "integer",
     sqlt.FLOAT: "float",
 }
 
+OP_MAP = {
+    "eq": "=",
+    "in": "ARRAY_CONTAINS",
+    "$contains": "ARRAY_CONTAINS",
+}
+
 
 def _map_type(typ: Type) -> str:
     for k, v in TYPE_MAP.items():
         if isinstance(typ, k):
             return v
     return "string"
 
@@ -29,21 +35,48 @@
     if not query.where_clause:
         return ""
     if isinstance(query.where_clause, str):
         where_clause_sql = query.where_clause
     elif isinstance(query.where_clause, list):
         where_clause_sql = " AND ".join(query.where_clause)
     elif isinstance(query.where_clause, dict):
-        # TODO: bobby tables
-        where_clause_sql = " AND ".join([f"{k} = '{v}'" for k, v in query.where_clause.items()])
+        conjs = []
+        for k, v in query.where_clause.items():
+            conjs.extend(col_val_constraints_to_conjs(k, v))
+        where_clause_sql = " AND ".join(conjs)
+
     else:
         raise ValueError(f"Invalid where_clause type: {type(query.where_clause)}")
     return "WHERE " + where_clause_sql
 
 
+def col_val_constraints_to_conjs(col_name: str, val_constraints: Any) -> list:
+    if val_constraints is None:
+        return []
+
+    def _quote(v: Any):
+        if isinstance(v, str):
+            # escape internal vs
+            v = v.replace("'", "''")
+            return f"'{v}'"
+        else:
+            return v
+
+    if isinstance(val_constraints, dict):
+        conjs = []
+        for k, v in val_constraints.items():
+            if k in OP_MAP:
+                conjs.append(f"{OP_MAP[k]}({col_name}, {_quote(v)})")
+            else:
+                conjs.append(f"{col_name} {k} {_quote(v)}")
+        return conjs
+    else:
+        return [f"{col_name} = {_quote(val_constraints)}"]
+
+
 def query_to_sql(query: Query, count=False, limit=None, offset: Optional[int] = None):
     select_cols = query.select_cols if query.select_cols else ["*"]
     if count:
         sql_str = ["SELECT COUNT(*)"]
     else:
         sql_str = [f"SELECT {', '.join(select_cols)}"]
     sql_str.append(f"FROM {query.from_table}")
@@ -63,35 +96,41 @@
         offset = offset if offset else query.offset
         if offset:
             sql_str.append(f" OFFSET {offset}")
     sql_str = [line for line in sql_str if line]
     return "\n".join(sql_str)
 
 
-def facet_count_sql(query: Query, facet_column: Union[str, Tuple[str, ...]], multivalued=False) -> str:
+def facet_count_sql(query: Query, facet_column: Union[str, Tuple[str, ...]], multivalued=False, limit=100) -> str:
     # Create a modified WHERE clause that excludes conditions directly related to facet_column
     modified_where = None
     if query.where_clause:
         where_clause_sql = where_clause_to_sql(query)
         # Split the where clause into conditions and exclude those related to the facet_column
         conditions = [cond for cond in where_clause_sql.split(" AND ") if not cond.startswith(f"{facet_column} ")]
         modified_where = " AND ".join(conditions)
 
     if isinstance(facet_column, tuple):
         if multivalued:
             raise NotImplementedError("Multivalued facets are not supported for multiple columns")
         facet_column = ", ".join(facet_column)
     from_table = query.from_table
     if multivalued:
-        from_table = f"(SELECT UNNEST({facet_column}) as {facet_column} FROM {query.from_table})"
+        from_table = f"(SELECT UNNEST({facet_column}) as {facet_column} FROM {query.from_table}"
+        from_table += f" {modified_where}" if modified_where else ""
+        from_table += ")"
+    else:
+        from_table += f" {modified_where}" if modified_where else ""
     sql_str = [f"SELECT {facet_column}, COUNT(*) as count", f"FROM {from_table}"]
-    if modified_where:
-        sql_str.append(f"{modified_where}")
+    # if modified_where:
+    #    sql_str.append(f"{modified_where}")
     sql_str.append(f"GROUP BY {facet_column}")
     sql_str.append("ORDER BY count DESC")  # Optional, order by count for convenience
+    if limit is not None:
+        sql_str.append(f"LIMIT {limit}")
     return "\n".join(sql_str)
 
 
 def introspect_schema(engine: sqlalchemy.Engine) -> SchemaDefinition:
     """
     Introspect a database schema and return a SchemaDefinition object
```

