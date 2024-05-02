# Comparing `tmp/dbt_ibis-0.8.1.tar.gz` & `tmp/dbt_ibis-0.9.0.tar.gz`

## Comparing `dbt_ibis-0.8.1.tar` & `dbt_ibis-0.9.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     7101 2020-02-02 00:00:00.000000 dbt_ibis-0.8.1/dbt_ibis/__init__.py
--rw-r--r--   0        0        0    11172 2020-02-02 00:00:00.000000 dbt_ibis-0.8.1/dbt_ibis/_compile.py
--rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 dbt_ibis-0.8.1/dbt_ibis/_dialects.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 dbt_ibis-0.8.1/dbt_ibis/_logging.py
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 dbt_ibis-0.8.1/dbt_ibis/_parse_dbt_project.py
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 dbt_ibis-0.8.1/dbt_ibis/_references.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_ibis-0.8.1/dbt_ibis/py.typed
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 dbt_ibis-0.8.1/.gitignore
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 dbt_ibis-0.8.1/LICENSE
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 dbt_ibis-0.8.1/README.md
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 dbt_ibis-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 dbt_ibis-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     7101 2020-02-02 00:00:00.000000 dbt_ibis-0.9.0/dbt_ibis/__init__.py
+-rw-r--r--   0        0        0    11172 2020-02-02 00:00:00.000000 dbt_ibis-0.9.0/dbt_ibis/_compile.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 dbt_ibis-0.9.0/dbt_ibis/_dialects.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 dbt_ibis-0.9.0/dbt_ibis/_logging.py
+-rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 dbt_ibis-0.9.0/dbt_ibis/_parse_dbt_project.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 dbt_ibis-0.9.0/dbt_ibis/_references.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_ibis-0.9.0/dbt_ibis/py.typed
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 dbt_ibis-0.9.0/.gitignore
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 dbt_ibis-0.9.0/LICENSE
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 dbt_ibis-0.9.0/README.md
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 dbt_ibis-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 dbt_ibis-0.9.0/PKG-INFO
```

### Comparing `dbt_ibis-0.8.1/dbt_ibis/__init__.py` & `dbt_ibis-0.9.0/dbt_ibis/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __all__ = ["ref", "source", "depends_on", "compile_ibis_to_sql"]
-__version__ = "0.8.1"
+__version__ = "0.9.0"
 
 import logging
 import subprocess
 import sys
 from importlib.machinery import SourceFileLoader
 from importlib.util import module_from_spec, spec_from_loader
 from pathlib import Path
```

### Comparing `dbt_ibis-0.8.1/dbt_ibis/_compile.py` & `dbt_ibis-0.9.0/dbt_ibis/_compile.py`

 * *Files identical despite different names*

### Comparing `dbt_ibis-0.8.1/dbt_ibis/_dialects.py` & `dbt_ibis-0.9.0/dbt_ibis/_dialects.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 from typing import NewType
 
 import ibis
-import ibis.backends.base.sqlglot.datatypes as sqlglot_dt
+import ibis.backends.sql.datatypes as sql_dt
 import ibis.expr.datatypes as dt
 import ibis.expr.types as ir
 from dbt.contracts.graph.manifest import Manifest
 from ibis.formats import TypeMapper
 
-
-# Custom BigQuery type until a corresponding one is implemented in Ibis itself.
-# See https://github.com/ibis-project/ibis/issues/7531
-class BigQueryType(sqlglot_dt.SqlglotType):
-    dialect = "bigquery"
-
-    default_decimal_precision = 38
-    default_decimal_scale = 9
-
-
 # Use NewType to make sure that we don't accidentally mix these up, i.e.
 # pass a DBTAdapterType to a function that expects an IbisDialect or vice versa.
 IbisDialect = NewType("IbisDialect", str)
 DBTAdapterType = NewType("DBTAdapterType", str)
 
 DBTAdapterTypeToIbisDialect: dict[DBTAdapterType, IbisDialect] = {
     DBTAdapterType("postgres"): IbisDialect("postgres"),
@@ -31,22 +21,22 @@
     DBTAdapterType("sqlite"): IbisDialect("sqlite"),
     DBTAdapterType("oracle"): IbisDialect("oracle"),
     DBTAdapterType("duckdb"): IbisDialect("duckdb"),
     DBTAdapterType("bigquery"): IbisDialect("bigquery"),
 }
 
 IbisDialectToTypeMapper: dict[IbisDialect, type[TypeMapper]] = {
-    IbisDialect("postgres"): sqlglot_dt.PostgresType,
-    IbisDialect("snowflake"): sqlglot_dt.SnowflakeType,
-    IbisDialect("trino"): sqlglot_dt.TrinoType,
-    IbisDialect("mysql"): sqlglot_dt.MySQLType,
-    IbisDialect("sqlite"): sqlglot_dt.SQLiteType,
-    IbisDialect("oracle"): sqlglot_dt.OracleType,
-    IbisDialect("duckdb"): sqlglot_dt.DuckDBType,
-    IbisDialect("bigquery"): BigQueryType,
+    IbisDialect("postgres"): sql_dt.PostgresType,
+    IbisDialect("snowflake"): sql_dt.SnowflakeType,
+    IbisDialect("trino"): sql_dt.TrinoType,
+    IbisDialect("mysql"): sql_dt.MySQLType,
+    IbisDialect("sqlite"): sql_dt.SQLiteType,
+    IbisDialect("oracle"): sql_dt.OracleType,
+    IbisDialect("duckdb"): sql_dt.DuckDBType,
+    IbisDialect("bigquery"): sql_dt.BigQueryType,
 }
 
 
 def get_ibis_dialect(manifest: Manifest) -> IbisDialect:
     dbt_adapter_type = manifest.metadata.adapter_type
     if dbt_adapter_type is None:
         raise ValueError("Could not determine dbt adapter type")
```

### Comparing `dbt_ibis-0.8.1/dbt_ibis/_parse_dbt_project.py` & `dbt_ibis-0.9.0/dbt_ibis/_parse_dbt_project.py`

 * *Files identical despite different names*

### Comparing `dbt_ibis-0.8.1/dbt_ibis/_references.py` & `dbt_ibis-0.9.0/dbt_ibis/_references.py`

 * *Files identical despite different names*

### Comparing `dbt_ibis-0.8.1/.gitignore` & `dbt_ibis-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_ibis-0.8.1/LICENSE` & `dbt_ibis-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_ibis-0.8.1/README.md` & `dbt_ibis-0.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,18 +7,21 @@
 
 
 @depends_on(ref("stg_stores"))
 def model(stores):
     return stores.filter(stores["country"] == "USA")
 ```
 
-You can install `dbt-ibis` via pip:
+You can install `dbt-ibis` via pip or conda:
 ```bash
 pip install dbt-ibis
+# or
+conda install -c conda-forge dbt-ibis
 ```
+
 In addition, you'll need to install the relevant [`Ibis` backend](https://ibis-project.org/install) for your database.
 
 You can read about the advantages of combining dbt and Ibis in [this blog post](https://ibis-project.org/posts/dbt-ibis/).
 
 
 ## Development
 ```bash
```

### Comparing `dbt_ibis-0.8.1/pyproject.toml` & `dbt_ibis-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dbt-ibis"
 authors = [{ name = "Stefan Binder" }]
-dependencies = ["dbt-core>=1.5", "ibis-framework>=7", "click"]
+dependencies = ["dbt-core>=1.5", "ibis-framework>=9", "click"]
 readme = "README.md"
 requires-python = ">=3.9"
 dynamic = ["version"]
 license-files = { paths = ["LICENSE"] }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `dbt_ibis-0.8.1/PKG-INFO` & `dbt_ibis-0.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.3
 Name: dbt-ibis
-Version: 0.8.1
+Version: 0.9.0
 Project-URL: Source, https://github.com/binste/dbt-ibis
 Author: Stefan Binder
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Requires-Dist: click
 Requires-Dist: dbt-core>=1.5
-Requires-Dist: ibis-framework>=7
+Requires-Dist: ibis-framework>=9
 Provides-Extra: dev
 Requires-Dist: dbt-duckdb; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: ibis-framework[duckdb]; extra == 'dev'
 Requires-Dist: ipdb; extra == 'dev'
 Requires-Dist: ipykernel; extra == 'dev'
 Requires-Dist: ipython; extra == 'dev'
@@ -41,18 +41,21 @@
 
 
 @depends_on(ref("stg_stores"))
 def model(stores):
     return stores.filter(stores["country"] == "USA")
 ```
 
-You can install `dbt-ibis` via pip:
+You can install `dbt-ibis` via pip or conda:
 ```bash
 pip install dbt-ibis
+# or
+conda install -c conda-forge dbt-ibis
 ```
+
 In addition, you'll need to install the relevant [`Ibis` backend](https://ibis-project.org/install) for your database.
 
 You can read about the advantages of combining dbt and Ibis in [this blog post](https://ibis-project.org/posts/dbt-ibis/).
 
 
 ## Development
 ```bash
```

