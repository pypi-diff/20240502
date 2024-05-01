# Comparing `tmp/driven_sql_tool-0.0.1.tar.gz` & `tmp/driven_sql_tool-0.0.4.tar.gz`

## Comparing `driven_sql_tool-0.0.1.tar` & `driven_sql_tool-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     9394 2020-02-02 00:00:00.000000 driven_sql_tool-0.0.1/src/driven_sql_tool/__init__.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 driven_sql_tool-0.0.1/LICENSE
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 driven_sql_tool-0.0.1/README.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 driven_sql_tool-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 driven_sql_tool-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 driven_sql_tool-0.0.4/.vscode/launch.json
+-rw-r--r--   0        0        0    19028 2020-02-02 00:00:00.000000 driven_sql_tool-0.0.4/src/driven_sql_tool/__init__.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 driven_sql_tool-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 driven_sql_tool-0.0.4/README.md
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 driven_sql_tool-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 driven_sql_tool-0.0.4/PKG-INFO
```

### Comparing `driven_sql_tool-0.0.1/LICENSE` & `driven_sql_tool-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `driven_sql_tool-0.0.1/PKG-INFO` & `driven_sql_tool-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,84 +1,90 @@
 Metadata-Version: 2.3
 Name: driven_sql_tool
-Version: 0.0.1
+Version: 0.0.4
 Summary: Simple wrapper (based on turbodbc) for most common MSSQL operations I face day-to-day
 Author-email: Ilya Davydov <shaddam.jabbar@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
+Requires-Dist: joblib
 Requires-Dist: pandas
 Requires-Dist: turbodbc
 Description-Content-Type: text/markdown
 
 # SQL Tools
 
 ## Description
 
 This is simply a turbodbc wrapper. To reduce boilerplate on routine SQL actions, making a code a little bit cleaner.
 
 ## Content
 
-Core functionality include three (data~) classes
-- SQLConfig : Collection of connection configuration options
-- Query : Query object
-- QuerySequence : Collection of Queries
+Core functionality include:
+- `SQLConfig` : Collection of connection configuration options. With `TurbODBCOptions` for advanced options
+- `Query` : Query object
+- `QuerySequence` : Collection of Queries
 
 ```Python
-from driven_sql_tool import SQLConfig, Query, QuerySequence
+from driven_sql_tool import SQLConfig, TurbODBCOptions, Query, QuerySequence
 ```
 
 ## Usage samples
 
 ```Python
-# prepare config
-conf = SQLConfig(server=r'server.address', database=r'db')
+# prepare sample instanced config ...
+turbodbc_options = TurbODBCOptions(autocommit=False, use_async_io=False)
+conf = SQLConfig(server=r'server.address', database=r'db', turbodbc_options=turbodbc_options)
+# ... or simply set defaults
+SQLConfig.default_server = r'default.server'
+SQLConfig.default_database = r'default.database'
 ```
 
 Most common actions (Data Query Language):
 ```Python
 # regular querying
 df_res = Query('SELECT * FROM db.schema.table', conf=conf).execute()
-# .sql file querying
-df_res = Query('./path/to/file.sql', conf=conf).execute()
-
+# not specifying conf attribute will grab class defaults
+df_res = Query('SELECT * FROM db.schema.table').execute()
 # the result is also stored in `data` property of `Query` object 
-query = Query('SELECT * FROM db.schema.table', conf=conf)
+query = Query('SELECT * FROM db.schema.table')
 query.execute()
 df_res = query.data
+
+# .sql file querying
+df_res = Query('./path/to/file.sql').execute()
 ```
 
 Parametrized actions 
 ```Python
 # parametrized insertion ...
 Query(
     """
         INSERT INTO db.schema.table
         ([ID], [field1], [field2], [date])
         VALUES (?, ?, ?, ?)
     """, 
-    data=df_insert[['ID', 'field1', 'field2', 'date']],
-    conf=conf
+    data=df_insert[['ID', 'field1', 'field2', 'date']]
 ).execute()
 # ... or execution
-Query('EXEC db.schema.sproc @p1=?, @p2=?', data=df_exec[['p1', 'p2']], conf=conf).execute()
+Query('EXEC db.schema.sproc @p1=?, @p2=?', data=df_exec[['p1', 'p2']]).execute()
 ```
 
 Running multiple queries
 ```Python
 # prepare sequence of queries
 queries = QuerySequence()
 
 queries.case_1 = Query('SELECT * FROM db.schema.table', conf=conf_1)
 queries.case_2 = Query('./query.sql', conf=conf_2)
-queries.case_3 = Query('EXEC db.schema.sproc @p1=?', data=df_exec[['p1']], conf=conf_3)
+queries.case_3 = Query('EXEC db.schema.sproc @p1=?', data=df_exec[['p1']])
 
 # run multiple queries sequentially ...
 queries.run_seq()
-# ... or in parallel (multiprocessing.Pool)
+# ... or, alternatively, in parallel (`joblib`)
 queries.run_par()
 
 # then access `data` property
 df_res_1 = queries.case_1.data
 ```
```

