# Comparing `tmp/bytebridge-0.0.2.tar.gz` & `tmp/bytebridge-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytebridge-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "bytebridge-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bytebridge-0.0.2.tar` & `bytebridge-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    11347 2024-03-02 14:29:17.775673 bytebridge-0.0.2/LICENSE
--rw-r--r--   0        0        0     3076 2024-03-02 14:29:17.775673 bytebridge-0.0.2/README.md
--rw-r--r--   0        0        0      116 2024-03-02 14:29:17.775673 bytebridge-0.0.2/bytebridge/__init__.py
--rw-r--r--   0        0        0     2232 2024-03-02 14:29:17.775673 bytebridge-0.0.2/bytebridge/cli.py
--rw-r--r--   0        0        0        0 2024-03-02 14:29:17.775673 bytebridge-0.0.2/bytebridge/connectors/__init__.py
--rw-r--r--   0        0        0      410 2024-03-02 14:29:17.775673 bytebridge-0.0.2/bytebridge/connectors/base.py
--rw-r--r--   0        0        0     4330 2024-03-02 14:29:17.775673 bytebridge-0.0.2/bytebridge/connectors/database.py
--rw-r--r--   0        0        0     1106 2024-03-02 14:29:17.775673 bytebridge-0.0.2/bytebridge/connectors/file.py
--rw-r--r--   0        0        0     1366 2024-03-02 14:29:17.775673 bytebridge-0.0.2/bytebridge/operations.py
--rw-r--r--   0        0        0      164 2024-03-02 14:29:17.775673 bytebridge-0.0.2/bytebridge/parsers.py
--rw-r--r--   0        0        0      667 2024-03-02 14:29:17.775673 bytebridge-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 bytebridge-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11347 2024-05-01 23:22:36.604590 bytebridge-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3157 2024-05-01 23:22:36.604590 bytebridge-0.0.3/README.md
+-rw-r--r--   0        0        0      116 2024-05-01 23:22:36.604590 bytebridge-0.0.3/bytebridge/__init__.py
+-rw-r--r--   0        0        0     2250 2024-05-01 23:22:36.604590 bytebridge-0.0.3/bytebridge/cli.py
+-rw-r--r--   0        0        0        0 2024-05-01 23:22:36.604590 bytebridge-0.0.3/bytebridge/connectors/__init__.py
+-rw-r--r--   0        0        0      450 2024-05-01 23:22:36.604590 bytebridge-0.0.3/bytebridge/connectors/base.py
+-rw-r--r--   0        0        0     4381 2024-05-01 23:22:36.604590 bytebridge-0.0.3/bytebridge/connectors/database.py
+-rw-r--r--   0        0        0     2309 2024-05-01 23:22:36.604590 bytebridge-0.0.3/bytebridge/connectors/file.py
+-rw-r--r--   0        0        0      245 2024-05-01 23:22:36.604590 bytebridge-0.0.3/bytebridge/exceptions.py
+-rw-r--r--   0        0        0     1706 2024-05-01 23:22:36.604590 bytebridge-0.0.3/bytebridge/operations.py
+-rw-r--r--   0        0        0      164 2024-05-01 23:22:36.604590 bytebridge-0.0.3/bytebridge/parsers.py
+-rw-r--r--   0        0        0      688 2024-05-01 23:22:36.604590 bytebridge-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3740 1970-01-01 00:00:00.000000 bytebridge-0.0.3/PKG-INFO
```

### Comparing `bytebridge-0.0.2/LICENSE` & `bytebridge-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bytebridge-0.0.2/README.md` & `bytebridge-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -70,29 +70,29 @@
 
 | Name             | Type          | Client                                                                         |
 |----------------- | --------------|--------------------------------------------------------------------------------|
 | PostgreSQL       | Database      | [psycopg](https://pypi.org/project/psycopg/)                                   |
 | MySQL            | Database      | [mysql-connector-python](https://pypi.org/project/mysql-connector-python/)     |
 | MS SQL Server    | Database      | [pymssql](https://pypi.org/project/pymssql/)                                   |
 | Parquet          | File          | [pyarrow](https://pypi.org/project/pyarrow/)                                   |
+| CSV              | File          | [csv](https://docs.python.org/3/library/csv.html)                              |
 
 
 
 ### Planned
 
 | Name             | Type          |
 |----------------- | --------------|
 | SQLite           | Database      |
 | MongoDB          | Database      |
 | MariaDB          | Database      |
 | Clickhouse       | Database      |
 | BigQuery         | Database      |
 | Oracle           | Database      |
 | Cassandra        | Database      |
-| CSV              | File          |
 | ORC              | File          |
 | Avro             | File          |
 | Excel (XLSX)     | File          |
 | JSON             | File          |
```

#### html2text {}

```diff
@@ -17,15 +17,15 @@
 [postgresql_password_to_be_used]", "port": "[postgresql_port_to_be_used]", } }
 } ``` ## API Coming soon. ## Data Connectors ### Currently Supported | Name |
 Type | Client | |----------------- | --------------|---------------------------
 -----------------------------------------------------| | PostgreSQL | Database
 | [psycopg](https://pypi.org/project/psycopg/) | | MySQL | Database | [mysql-
 connector-python](https://pypi.org/project/mysql-connector-python/) | | MS SQL
 Server | Database | [pymssql](https://pypi.org/project/pymssql/) | | Parquet |
-File | [pyarrow](https://pypi.org/project/pyarrow/) | ### Planned | Name | Type
-| |----------------- | --------------| | SQLite | Database | | MongoDB |
-Database | | MariaDB | Database | | Clickhouse | Database | | BigQuery |
-Database | | Oracle | Database | | Cassandra | Database | | CSV | File | | ORC
-| File | | Avro | File | | Excel (XLSX) | File | | JSON | File | ##
-Contributing Feel free to contribute to this project. See the contribution
-guidelines in [here](CONTRIBUTING.md). ## License This project is licensed
-under the terms of the [Apache 2.0 license](LICENSE).
+File | [pyarrow](https://pypi.org/project/pyarrow/) | | CSV | File | [csv]
+(https://docs.python.org/3/library/csv.html) | ### Planned | Name | Type | |---
+-------------- | --------------| | SQLite | Database | | MongoDB | Database | |
+MariaDB | Database | | Clickhouse | Database | | BigQuery | Database | | Oracle
+| Database | | Cassandra | Database | | ORC | File | | Avro | File | | Excel
+(XLSX) | File | | JSON | File | ## Contributing Feel free to contribute to this
+project. See the contribution guidelines in [here](CONTRIBUTING.md). ## License
+This project is licensed under the terms of the [Apache 2.0 license](LICENSE).
```

### Comparing `bytebridge-0.0.2/bytebridge/cli.py` & `bytebridge-0.0.3/bytebridge/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         required=True,
         help="The object to load data in the target (a table name or a filepath)",
     )
     transfer_parser.add_argument(
         "--batch-size",
         required=False,
         default=100,
+        type=int,
         help="The size of batches used during the data transfer.",
     )
     args = parser.parse_args()
 
     if args.operation == "transfer":
         _execute_transfer_operation(args)
```

### Comparing `bytebridge-0.0.2/bytebridge/connectors/database.py` & `bytebridge-0.0.3/bytebridge/connectors/database.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from contextlib import closing
-from typing import Callable, Dict, Iterator, List
+from typing import Callable, Dict, Iterator, List, Optional
 
 import mysql.connector
 import psycopg
-from psycopg.rows import dict_row
 import pymssql
+from psycopg.rows import dict_row
 
-from .base import Connector
+from bytebridge.connectors.base import Connector
 
 
 class DatabaseConnector(Connector):
     def __init__(
         self,
         *,
         connection_handler: Callable,
@@ -20,16 +20,16 @@
         self._connection_handler = connection_handler
         self._connection_parameters = connection_parameters
         self._cursor_parameters = cursor_parameters
 
     def extract(
         self,
         *,
-        source_object: str,
-        source_query: str,
+        source_object: Optional[str],
+        source_query: Optional[str],
         batch_size: int,
     ):
         sql = self._render_query(source_query, source_object)
 
         with closing(
             self._connection_handler(
                 host=self._connection_parameters["host"],
```

### Comparing `bytebridge-0.0.2/bytebridge/connectors/file.py` & `bytebridge-0.0.3/bytebridge/connectors/file.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import csv
+import itertools
 from typing import Iterator, List
 
 import pyarrow
 from pyarrow import parquet
 
 from .base import Connector
 
@@ -30,7 +32,43 @@
         first_batch = next(batch_iterator)
         if first_batch:
             record_batch = pyarrow.RecordBatch.from_pylist(first_batch)
             with parquet.ParquetWriter(target_object, record_batch.schema) as writer:
                 writer.write_batch(record_batch)
                 for batch in batch_iterator:
                     writer.write_batch(batch=pyarrow.RecordBatch.from_pylist(batch))
+
+
+class CsvConnector(Connector):
+    def __init__(self, *, connection_parameters: dict) -> None:
+        self._delimiter = connection_parameters.get("delimiter", ",")
+
+    def extract(
+        self,
+        *,
+        source_object: str,
+        source_query: str,
+        batch_size: int,
+    ) -> Iterator[List[dict]]:
+        with open(source_object) as source_file:
+            csv_reader = csv.DictReader(source_file, delimiter=self._delimiter)
+            while batch := tuple(itertools.islice(csv_reader, batch_size)):
+                yield batch
+
+    def load(
+        self,
+        *,
+        target_object: str,
+        batch_iterator: Iterator[dict],
+    ):
+        first_batch = next(batch_iterator)
+        if first_batch:
+            with open(target_object, "w") as target_file:
+                csv_writer = csv.DictWriter(
+                    target_file,
+                    fieldnames=first_batch[0].keys(),
+                    delimiter=self._delimiter,
+                )
+                csv_writer.writeheader()
+                csv_writer.writerows(first_batch)
+                for batch in batch_iterator:
+                    csv_writer.writerows(batch)
```

### Comparing `bytebridge-0.0.2/bytebridge/operations.py` & `bytebridge-0.0.3/bytebridge/operations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,49 @@
-from typing import Union
+from typing import Any, Dict, Optional, Type
 
-from .connectors.database import MySqlConnector, PostgresConnector, MsSqlConnector
-from .connectors.file import ParquetConnector
+from bytebridge.connectors.base import Connector
+from bytebridge.connectors.database import (
+    MsSqlConnector,
+    MySqlConnector,
+    PostgresConnector,
+)
+from bytebridge.connectors.file import CsvConnector, ParquetConnector
+from bytebridge.exceptions import UnsupportedConnectorError
 
 
-def _get_connector(
-    connector_type: str
-) -> Union[PostgresConnector, MySqlConnector, ParquetConnector]:
+def _get_connector(connector_type: str) -> Type[Connector]:
     supported_connectors = {
         "postgresql": PostgresConnector,
         "mysql": MySqlConnector,
         "parquet": ParquetConnector,
         "mssql": MsSqlConnector,
+        "csv": CsvConnector,
     }
     if connector_type not in supported_connectors:
-        raise ValueError(f"The connector {connector_type} is not supported.")
+        raise UnsupportedConnectorError(connector_type=connector_type)
     return supported_connectors[connector_type]
 
 
 def transfer(
     *,
-    source_query: str,
-    source_object: str,
-    source_connection: dict,
+    source_query: Optional[str],
+    source_object: Optional[str],
+    source_connection: Dict[str, Any],
     batch_size: int,
     target_object: str,
-    destination_connection: dict,
-):
+    destination_connection: Dict[str, Any],
+) -> None:
+    if not source_query and not source_object:
+        raise ValueError("Either 'source_query' or 'source_object' must be provided.")
+
     source_connector = _get_connector(source_connection["type"])(
         connection_parameters=source_connection.get("parameters"),
     )
     destination_connector = _get_connector(destination_connection["type"])(
-        connection_parameters=destination_connection.get("parameters"),
+        connection_parameters=destination_connection.get("parameters", {}),
     )
     batch_iterator = source_connector.extract(
         source_query=source_query,
         source_object=source_object,
         batch_size=batch_size,
     )
     destination_connector.load(
```

### Comparing `bytebridge-0.0.2/pyproject.toml` & `bytebridge-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 ]
 
 
 [project.optional-dependencies]
 dev = [
     "ruff ==0.1.5",
     "pre-commit >=2.17.0",
+    "pytest ==8.1.1"
 ]
 
 [project.scripts] 
 bytebridge = "bytebridge.cli:main"
 
 
 [tool.ruff]
```

### Comparing `bytebridge-0.0.2/PKG-INFO` & `bytebridge-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: bytebridge
-Version: 0.0.2
+Version: 0.0.3
 Summary: A data tool designed to move data seamlessly between various sources and destinations.
 Author-email: Rafael Vargas <contact@rafaelvargas.dev>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: psycopg[binary] >=3.0.9
 Requires-Dist: pyarrow >=7.0.0
 Requires-Dist: mysql-connector-python >=8.0.19
 Requires-Dist: pymssql >=2.2.11
 Requires-Dist: ruff ==0.1.5 ; extra == "dev"
 Requires-Dist: pre-commit >=2.17.0 ; extra == "dev"
+Requires-Dist: pytest ==8.1.1 ; extra == "dev"
 Provides-Extra: dev
 
 
 
 <p align="center" style="padding: 20px">
   <img src="static/branding/logo.svg" style="width:450px" alt="bytebridge">
 </p>
@@ -85,29 +86,29 @@
 
 | Name             | Type          | Client                                                                         |
 |----------------- | --------------|--------------------------------------------------------------------------------|
 | PostgreSQL       | Database      | [psycopg](https://pypi.org/project/psycopg/)                                   |
 | MySQL            | Database      | [mysql-connector-python](https://pypi.org/project/mysql-connector-python/)     |
 | MS SQL Server    | Database      | [pymssql](https://pypi.org/project/pymssql/)                                   |
 | Parquet          | File          | [pyarrow](https://pypi.org/project/pyarrow/)                                   |
+| CSV              | File          | [csv](https://docs.python.org/3/library/csv.html)                              |
 
 
 
 ### Planned
 
 | Name             | Type          |
 |----------------- | --------------|
 | SQLite           | Database      |
 | MongoDB          | Database      |
 | MariaDB          | Database      |
 | Clickhouse       | Database      |
 | BigQuery         | Database      |
 | Oracle           | Database      |
 | Cassandra        | Database      |
-| CSV              | File          |
 | ORC              | File          |
 | Avro             | File          |
 | Excel (XLSX)     | File          |
 | JSON             | File          |
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: bytebridge Version: 0.0.2 Summary: A data tool
+Metadata-Version: 2.1 Name: bytebridge Version: 0.0.3 Summary: A data tool
 designed to move data seamlessly between various sources and destinations.
 Author-email: Rafael Vargas
 rafaelvargas.dev> Requires-Python: >=3.7 Description-Content-Type: text/
 markdown Requires-Dist: psycopg[binary] >=3.0.9 Requires-Dist: pyarrow >=7.0.0
 Requires-Dist: mysql-connector-python >=8.0.19 Requires-Dist: pymssql >=2.2.11
 Requires-Dist: ruff ==0.1.5 ; extra == "dev" Requires-Dist: pre-commit >=2.17.0
-; extra == "dev" Provides-Extra: dev
+; extra == "dev" Requires-Dist: pytest ==8.1.1 ; extra == "dev" Provides-Extra:
+dev
                                  [bytebridge]
    AA ddaattaa ttooooll ddeessiiggnneedd ttoo mmoovvee ddaattaa sseeaammlleessssllyy bbeettwweeeenn vvaarriioouuss ssoouurrcceess aanndd
                                  ddeessttiinnaattiioonnss..
                                _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]
 ## CLI Bytebridge aims to have a CLI that can be used to easily transfer data
 from multiple sources. Some examples are shown below: ### Parquet to PostgreSQL
 ```bash bytebridge transfer \ --connections connections.json \ --source
@@ -25,15 +26,15 @@
 [postgresql_password_to_be_used]", "port": "[postgresql_port_to_be_used]", } }
 } ``` ## API Coming soon. ## Data Connectors ### Currently Supported | Name |
 Type | Client | |----------------- | --------------|---------------------------
 -----------------------------------------------------| | PostgreSQL | Database
 | [psycopg](https://pypi.org/project/psycopg/) | | MySQL | Database | [mysql-
 connector-python](https://pypi.org/project/mysql-connector-python/) | | MS SQL
 Server | Database | [pymssql](https://pypi.org/project/pymssql/) | | Parquet |
-File | [pyarrow](https://pypi.org/project/pyarrow/) | ### Planned | Name | Type
-| |----------------- | --------------| | SQLite | Database | | MongoDB |
-Database | | MariaDB | Database | | Clickhouse | Database | | BigQuery |
-Database | | Oracle | Database | | Cassandra | Database | | CSV | File | | ORC
-| File | | Avro | File | | Excel (XLSX) | File | | JSON | File | ##
-Contributing Feel free to contribute to this project. See the contribution
-guidelines in [here](CONTRIBUTING.md). ## License This project is licensed
-under the terms of the [Apache 2.0 license](LICENSE).
+File | [pyarrow](https://pypi.org/project/pyarrow/) | | CSV | File | [csv]
+(https://docs.python.org/3/library/csv.html) | ### Planned | Name | Type | |---
+-------------- | --------------| | SQLite | Database | | MongoDB | Database | |
+MariaDB | Database | | Clickhouse | Database | | BigQuery | Database | | Oracle
+| Database | | Cassandra | Database | | ORC | File | | Avro | File | | Excel
+(XLSX) | File | | JSON | File | ## Contributing Feel free to contribute to this
+project. See the contribution guidelines in [here](CONTRIBUTING.md). ## License
+This project is licensed under the terms of the [Apache 2.0 license](LICENSE).
```

