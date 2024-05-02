# Comparing `tmp/pinotdb-5.1.6.tar.gz` & `tmp/pinotdb-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinotdb-5.1.6.tar", max compression
+gzip compressed data, was "pinotdb-5.2.0.tar", max compression
```

## Comparing `pinotdb-5.1.6.tar` & `pinotdb-5.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1087 2024-03-26 06:31:28.779562 pinotdb-5.1.6/LICENSE
--rw-r--r--   0        0        0    16036 2024-03-26 06:31:28.779562 pinotdb-5.1.6/README.md
--rw-r--r--   0        0        0      682 2024-03-26 06:31:28.779562 pinotdb-5.1.6/pinotdb/__init__.py
--rw-r--r--   0        0        0    19143 2024-03-26 06:31:28.779562 pinotdb-5.1.6/pinotdb/db.py
--rw-r--r--   0        0        0      438 2024-03-26 06:31:28.779562 pinotdb-5.1.6/pinotdb/exceptions.py
--rw-r--r--   0        0        0    13171 2024-03-26 06:31:28.779562 pinotdb-5.1.6/pinotdb/keywords.py
--rw-r--r--   0        0        0    12355 2024-03-26 06:31:28.779562 pinotdb-5.1.6/pinotdb/sqlalchemy.py
--rw-r--r--   0        0        0     1258 2024-03-26 06:31:50.491693 pinotdb-5.1.6/pyproject.toml
--rw-r--r--   0        0        0    16979 1970-01-01 00:00:00.000000 pinotdb-5.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-05-02 14:10:35.968020 pinotdb-5.2.0/LICENSE
+-rw-r--r--   0        0        0    17590 2024-05-02 14:10:35.968020 pinotdb-5.2.0/README.md
+-rw-r--r--   0        0        0      682 2024-05-02 14:10:35.968020 pinotdb-5.2.0/pinotdb/__init__.py
+-rw-r--r--   0        0        0    19638 2024-05-02 14:10:35.968020 pinotdb-5.2.0/pinotdb/db.py
+-rw-r--r--   0        0        0      438 2024-05-02 14:10:35.968020 pinotdb-5.2.0/pinotdb/exceptions.py
+-rw-r--r--   0        0        0    13171 2024-05-02 14:10:35.968020 pinotdb-5.2.0/pinotdb/keywords.py
+-rw-r--r--   0        0        0    12224 2024-05-02 14:10:35.968020 pinotdb-5.2.0/pinotdb/sqlalchemy.py
+-rw-r--r--   0        0        0     1258 2024-05-02 14:11:17.607676 pinotdb-5.2.0/pyproject.toml
+-rw-r--r--   0        0        0    18533 1970-01-01 00:00:00.000000 pinotdb-5.2.0/PKG-INFO
```

### Comparing `pinotdb-5.1.6/LICENSE` & `pinotdb-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pinotdb-5.1.6/README.md` & `pinotdb-5.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -53,14 +53,37 @@
 To pass in additional query parameters (such as `useMultistageEngine=true`) you may pass
 them in as part of the `execute` method. For example:
 
 ```python
 curs.execute("select * from airlineStats air limit 10", queryOptions="useMultistageEngine=true")
 ```
 
+#### Pass the Pinot database context
+
+> [!IMPORTANT]
+> This feature is only available from [5.1.5](https://pypi.org/project/pinotdb/5.1.5/)
+
+```python
+from pinotdb import connect
+
+# this assumes that 443 is the broker secure https port
+conn = connect(host='localhost', port=8000, path='/query/sql', scheme='http', database='dbName')
+curs = conn.cursor()
+curs.execute("""
+    SELECT col1 from table1 LIMIT 10
+""")
+for row in curs:
+    print(row)
+```
+where,
+- `dbName` : the database context that needs to be passed
+- `table1` : table under the `dbName` database
+
+If `database` is not specified the connection will use the `default` database context.
+
 ### Using SQLAlchemy:
 
 Since db engine requires more information beyond Pinot Broker, you need to provide pinot controller for table and schema information.
 
 The db engine connection string is format as:
 
 ```
@@ -110,14 +133,38 @@
 #     connect_args={"useMultistageEngine": "true"}
 # )
 
 places = Table('places', MetaData(bind=engine), autoload=True)
 print(select([func.count('*')], from_obj=places).scalar())
 ```
 
+To configure query parameters (such as `timeoutMs=10000`) at the engine level
+you may pass them while creating the engine. For example:
+
+```python
+engine = create_engine(
+        "pinot://localhost:8000/query/sql?controller=http://localhost:9000/",
+        connect_args={"query_options": "useMultistageEngine=true;timeoutMs=10000"})
+```
+
+#### Pass the Pinot database context
+
+> [!IMPORTANT]
+> This feature is only available from [5.1.5](https://pypi.org/project/pinotdb/5.1.5/)
+
+Each connection should only query one Pinot Database, hence we provide that context through connection string itself.
+
+The db engine connection string is format as:
+
+```
+pinot+http://pinot-broker:8099/query/sql?controller=http://pinot-controller:9000/&database=dbName
+```
+where `dbName` is the database context that needs to be passed.
+If not specified the connection will use the `default` database context while querying.
+
 
 ## Examples with Pinot Quickstart
 
 Start Pinot Batch Quickstart
 
 ```bash
 docker run --name pinot-quickstart -p 2123:2123 -p 9000:9000 -p 8000:8000 -d apachepinot/pinot:latest QuickStart -type batch
```

### Comparing `pinotdb-5.1.6/pinotdb/__init__.py` & `pinotdb-5.2.0/pinotdb/__init__.py`

 * *Files identical despite different names*

### Comparing `pinotdb-5.1.6/pinotdb/db.py` & `pinotdb-5.2.0/pinotdb/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,14 +137,15 @@
 
     def __init__(self, *args, **kwargs):
         self._debug = kwargs.get("debug", False)
         self._args = args
         self._kwargs = kwargs
         self.closed = False
         self.use_multistage_engine = kwargs.get('use_multistage_engine', False)
+        self.query_options = kwargs.get('query_options', None)
         self.cursors = []
         self.session = kwargs.get('session')
         self.is_session_external = False
         if self.session:
             self.verify_session()
             self.is_session_external = True
 
@@ -187,15 +188,15 @@
         self.cursors.append(cursor)
 
         return cursor
 
     @check_closed
     def execute(self, operation, parameters=None):
         cursor = self.cursor()
-        return cursor.execute(operation, parameters)
+        return cursor.execute(operation, parameters, self.query_options)
 
     def __enter__(self):
         return self.cursor()
 
     def __exit__(self, *exc):
         self.close()
 
@@ -235,15 +236,15 @@
         # if we're managing the httpx session, attempt to close it
         if not self.is_session_external:
             await self.session.aclose()
 
     @check_closed
     async def execute(self, operation, parameters=None):
         cursor = self.cursor()
-        return await cursor.execute(operation, parameters)
+        return await cursor.execute(operation, parameters, self.query_options)
 
     async def __aenter__(self):
         return self.cursor()
 
     async def __aexit__(self, *exc):
         await self.close()
 
@@ -290,14 +291,15 @@
         preserve_types=False,
         ignore_exception_error_codes="",
         acceptable_respond_fraction=-1,
         # TODO: Move this parameter when we can afford to break the
         #  interface (e.g. new minor version).
         session=None,
         use_multistage_engine=False,
+        query_options=None,
         **kwargs
     ):
         self.url = parse.urlunparse(
             (scheme, f"{host}:{port}", path, None, None, None))
         self.session = session
 
         # This read/write attribute specifies the number of rows to fetch at a
@@ -312,14 +314,15 @@
         self.schema = None
         self.rowcount = -1
         self._results = None
         self.timeUsedMs = -1
         self._debug = debug
         self._preserve_types = preserve_types
         self._use_multistage_engine = use_multistage_engine
+        self._query_options = query_options
         self.acceptable_respond_fraction = acceptable_respond_fraction
         if ignore_exception_error_codes:
             self._ignore_exception_error_codes = set(
                 [int(x) for x in ignore_exception_error_codes.split(",")]
             )
         else:
             self._ignore_exception_error_codes = []
@@ -473,14 +476,19 @@
 
     @check_closed
     # TODO: Rename queryOptions to query_options when releasing a breaking
     #  version - even though Pinot understands "queryOptions", we don't need
     #  to follow the same camel casing convention, but rather should stick
     #  to PEP-8 instead.
     def execute(self, operation, parameters=None, queryOptions=None, **kwargs):
+        if not queryOptions:
+            queryOptions = ""
+        if self._query_options:
+            queryOptions = queryOptions + ";" + self._query_options
+
         query = self.finalize_query_payload(
             operation, parameters, queryOptions)
 
         if self.auth and self.auth._username and self.auth._password:
             r = self.session.post(
                 self.url,
                 json=query,
@@ -569,14 +577,19 @@
 
 
 class AsyncCursor(Cursor):
     @check_closed
     async def execute(
             self, operation, parameters=None, queryOptions=None, **kwargs
     ):
+        if not queryOptions:
+            queryOptions = ""
+        if self._query_options:
+            queryOptions = queryOptions + ";" + self._query_options
+
         query = self.finalize_query_payload(
             operation, parameters, queryOptions)
 
         if self.auth and self.auth._username and self.auth._password:
             r = await self.session.post(
                 self.url,
                 json=query,
```

### Comparing `pinotdb-5.1.6/pinotdb/keywords.py` & `pinotdb-5.2.0/pinotdb/keywords.py`

 * *Files identical despite different names*

### Comparing `pinotdb-5.1.6/pinotdb/sqlalchemy.py` & `pinotdb-5.2.0/pinotdb/sqlalchemy.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,14 @@
 
 
 class PinotCompiler(compiler.SQLCompiler):
     def visit_select(self, select, **kwargs):
         return super().visit_select(select, **kwargs)
 
     def visit_column(self, column, result_map=None, **kwargs):
-        # Pinot does not support table aliases
-        if column.table is not None:
-            column.table.named_with_column = False
         result_map = result_map or kwargs.pop("add_to_result_map", None)
         # This is a hack to modify the original column, but how do I clone it ?
         column.is_literal = True
         return super().visit_column(column, result_map, **kwargs)
 
     def escape_literal_column(self, text):
         # This is a hack to quote column names that conflict with reserved
@@ -57,26 +54,26 @@
 
 
 class PinotTypeCompiler(compiler.GenericTypeCompiler):
     def visit_REAL(self, type_, **kwargs):
         return "DOUBLE"
 
     def visit_NUMERIC(self, type_, **kwargs):
-        return "LONG"
+        return "NUMERIC"
 
     visit_DECIMAL = visit_NUMERIC
     visit_INTEGER = visit_NUMERIC
     visit_SMALLINT = visit_NUMERIC
     visit_BIGINT = visit_NUMERIC
     visit_BOOLEAN = visit_NUMERIC
     visit_TIMESTAMP = visit_NUMERIC
     visit_DATE = visit_NUMERIC
 
     def visit_CHAR(self, type_, **kwargs):
-        return "STRING"
+        return "VARCHAR"
 
     visit_NCHAR = visit_CHAR
     visit_VARCHAR = visit_CHAR
     visit_NVARCHAR = visit_CHAR
     visit_TEXT = visit_CHAR
 
     def visit_BINARY(self, type_, **kwargs):
```

### Comparing `pinotdb-5.1.6/pyproject.toml` & `pinotdb-5.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pinotdb"
-version = "5.1.6"
+version = "5.2.0"
 description = "Python DB-API and SQLAlchemy dialect for Pinot."
 authors = ["Beto Dealmeida <beto@dealmeida.net>", "Devesh Agrawal <devesh.agrawal@gmail.com>", "Xiang Fu <xiangfu.1024@gmail.com>", "Rong Rong <rongr@apache.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pinotdb"}]
 homepage = "https://github.com/python-pinot-dbapi/pinot-dbapi"
```

### Comparing `pinotdb-5.1.6/PKG-INFO` & `pinotdb-5.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinotdb
-Version: 5.1.6
+Version: 5.2.0
 Summary: Python DB-API and SQLAlchemy dialect for Pinot.
 Home-page: https://github.com/python-pinot-dbapi/pinot-dbapi
 License: MIT
 Author: Beto Dealmeida
 Author-email: beto@dealmeida.net
 Requires-Python: >=3.7,<4
 Classifier: License :: OSI Approved :: MIT License
@@ -77,14 +77,37 @@
 To pass in additional query parameters (such as `useMultistageEngine=true`) you may pass
 them in as part of the `execute` method. For example:
 
 ```python
 curs.execute("select * from airlineStats air limit 10", queryOptions="useMultistageEngine=true")
 ```
 
+#### Pass the Pinot database context
+
+> [!IMPORTANT]
+> This feature is only available from [5.1.5](https://pypi.org/project/pinotdb/5.1.5/)
+
+```python
+from pinotdb import connect
+
+# this assumes that 443 is the broker secure https port
+conn = connect(host='localhost', port=8000, path='/query/sql', scheme='http', database='dbName')
+curs = conn.cursor()
+curs.execute("""
+    SELECT col1 from table1 LIMIT 10
+""")
+for row in curs:
+    print(row)
+```
+where,
+- `dbName` : the database context that needs to be passed
+- `table1` : table under the `dbName` database
+
+If `database` is not specified the connection will use the `default` database context.
+
 ### Using SQLAlchemy:
 
 Since db engine requires more information beyond Pinot Broker, you need to provide pinot controller for table and schema information.
 
 The db engine connection string is format as:
 
 ```
@@ -134,14 +157,38 @@
 #     connect_args={"useMultistageEngine": "true"}
 # )
 
 places = Table('places', MetaData(bind=engine), autoload=True)
 print(select([func.count('*')], from_obj=places).scalar())
 ```
 
+To configure query parameters (such as `timeoutMs=10000`) at the engine level
+you may pass them while creating the engine. For example:
+
+```python
+engine = create_engine(
+        "pinot://localhost:8000/query/sql?controller=http://localhost:9000/",
+        connect_args={"query_options": "useMultistageEngine=true;timeoutMs=10000"})
+```
+
+#### Pass the Pinot database context
+
+> [!IMPORTANT]
+> This feature is only available from [5.1.5](https://pypi.org/project/pinotdb/5.1.5/)
+
+Each connection should only query one Pinot Database, hence we provide that context through connection string itself.
+
+The db engine connection string is format as:
+
+```
+pinot+http://pinot-broker:8099/query/sql?controller=http://pinot-controller:9000/&database=dbName
+```
+where `dbName` is the database context that needs to be passed.
+If not specified the connection will use the `default` database context while querying.
+
 
 ## Examples with Pinot Quickstart
 
 Start Pinot Batch Quickstart
 
 ```bash
 docker run --name pinot-quickstart -p 2123:2123 -p 9000:9000 -p 8000:8000 -d apachepinot/pinot:latest QuickStart -type batch
```

