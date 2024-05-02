# Comparing `tmp/sesql-2024.4.1rc1.tar.gz` & `tmp/sesql-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sesql-2024.4.1rc1.tar", last modified: Wed Apr 17 00:37:13 2024, max compression
+gzip compressed data, was "sesql-2024.5.0.tar", last modified: Thu May  2 01:56:19 2024, max compression
```

## Comparing `sesql-2024.4.1rc1.tar` & `sesql-2024.5.0.tar`

### file list

```diff
@@ -1,34 +1,30 @@
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-17 00:37:13.694845 sesql-2024.4.1rc1/
--rw-r--r--   0 rjd        (501) staff       (20)     1078 2023-12-26 02:50:39.000000 sesql-2024.4.1rc1/License.md
--rw-r--r--   0 rjd        (501) staff       (20)     6507 2024-04-17 00:37:13.694640 sesql-2024.4.1rc1/PKG-INFO
--rw-r--r--   0 rjd        (501) staff       (20)     4844 2024-04-17 00:36:16.000000 sesql-2024.4.1rc1/ReadMe.md
--rw-r--r--   0 rjd        (501) staff       (20)      808 2024-03-31 00:07:50.000000 sesql-2024.4.1rc1/pyproject.toml
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-17 00:37:13.687099 sesql-2024.4.1rc1/seCore/
--rw-r--r--   0 rjd        (501) staff       (20)      839 2024-03-30 23:03:58.000000 sesql-2024.4.1rc1/seCore/CustomLogging.py
--rw-r--r--   0 rjd        (501) staff       (20)        0 2024-03-17 19:54:29.000000 sesql-2024.4.1rc1/seCore/__init__.py
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-17 00:37:13.687412 sesql-2024.4.1rc1/seSql/
--rw-r--r--   0 rjd        (501) staff       (20)      280 2024-04-01 23:44:41.000000 sesql-2024.4.1rc1/seSql/__init__.py
--rw-r--r--   0 rjd        (501) staff       (20)      316 2024-04-17 00:37:11.000000 sesql-2024.4.1rc1/seSql/_version.py
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-17 00:37:13.689452 sesql-2024.4.1rc1/seSql/dbc/
--rw-r--r--   0 rjd        (501) staff       (20)     2383 2024-03-03 23:41:30.000000 sesql-2024.4.1rc1/seSql/dbc/Exceptions.py
--rw-r--r--   0 rjd        (501) staff       (20)     7673 2024-04-16 01:10:44.000000 sesql-2024.4.1rc1/seSql/dbc/JDBC.py
--rw-r--r--   0 rjd        (501) staff       (20)     7329 2024-04-16 19:43:40.000000 sesql-2024.4.1rc1/seSql/dbc/ODBC.py
--rw-r--r--   0 rjd        (501) staff       (20)     5936 2024-02-29 01:59:07.000000 sesql-2024.4.1rc1/seSql/dbc/ODBCError.py
--rw-r--r--   0 rjd        (501) staff       (20)      726 2024-04-01 01:40:37.000000 sesql-2024.4.1rc1/seSql/dbc/Utilities.py
--rw-r--r--   0 rjd        (501) staff       (20)        0 2024-03-17 19:54:29.000000 sesql-2024.4.1rc1/seSql/dbc/__init__.py
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-17 00:37:13.689566 sesql-2024.4.1rc1/seSql/dbc/jars/
--rw-r--r--   0 rjd        (501) staff       (20)  1438398 2024-03-01 01:47:02.000000 sesql-2024.4.1rc1/seSql/dbc/jars/mssql-jdbc-12.4.2.jre8.jar
--rw-r--r--   0 rjd        (501) staff       (20)     4303 2024-04-16 02:19:23.000000 sesql-2024.4.1rc1/seSql/sql.py
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-17 00:37:13.694375 sesql-2024.4.1rc1/sesql.egg-info/
--rw-r--r--   0 rjd        (501) staff       (20)     6507 2024-04-17 00:37:13.000000 sesql-2024.4.1rc1/sesql.egg-info/PKG-INFO
--rw-r--r--   0 rjd        (501) staff       (20)      556 2024-04-17 00:37:13.000000 sesql-2024.4.1rc1/sesql.egg-info/SOURCES.txt
--rw-r--r--   0 rjd        (501) staff       (20)        1 2024-04-17 00:37:13.000000 sesql-2024.4.1rc1/sesql.egg-info/dependency_links.txt
--rw-r--r--   0 rjd        (501) staff       (20)       56 2024-04-17 00:37:13.000000 sesql-2024.4.1rc1/sesql.egg-info/requires.txt
--rw-r--r--   0 rjd        (501) staff       (20)       13 2024-04-17 00:37:13.000000 sesql-2024.4.1rc1/sesql.egg-info/top_level.txt
--rw-r--r--   0 rjd        (501) staff       (20)       38 2024-04-17 00:37:13.694882 sesql-2024.4.1rc1/setup.cfg
-drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-04-17 00:37:13.694177 sesql-2024.4.1rc1/tests/
--rw-r--r--   0 rjd        (501) staff       (20)     1790 2024-03-31 01:39:23.000000 sesql-2024.4.1rc1/tests/test_Exceptions.py
--rw-r--r--   0 rjd        (501) staff       (20)      222 2024-03-31 23:51:30.000000 sesql-2024.4.1rc1/tests/test_customlogging.py
--rw-r--r--   0 rjd        (501) staff       (20)      987 2024-04-01 01:44:20.000000 sesql-2024.4.1rc1/tests/test_jdbc.py
--rw-r--r--   0 rjd        (501) staff       (20)      690 2024-04-01 01:35:26.000000 sesql-2024.4.1rc1/tests/test_odbc.py
--rw-r--r--   0 rjd        (501) staff       (20)      238 2024-04-01 01:39:41.000000 sesql-2024.4.1rc1/tests/test_utilities.py
+drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-05-02 01:56:19.037971 sesql-2024.5.0/
+-rw-r--r--   0 rjd        (501) staff       (20)     1078 2023-12-26 02:50:39.000000 sesql-2024.5.0/License.md
+-rw-r--r--   0 rjd        (501) staff       (20)    13704 2024-05-02 01:56:19.037744 sesql-2024.5.0/PKG-INFO
+-rw-r--r--   0 rjd        (501) staff       (20)    12073 2024-05-01 00:48:25.000000 sesql-2024.5.0/ReadMe.md
+-rw-r--r--   0 rjd        (501) staff       (20)      777 2024-04-30 19:13:21.000000 sesql-2024.5.0/pyproject.toml
+drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-05-02 01:56:19.032676 sesql-2024.5.0/seSql/
+-rw-r--r--   0 rjd        (501) staff       (20)      230 2024-04-28 01:12:09.000000 sesql-2024.5.0/seSql/__init__.py
+-rw-r--r--   0 rjd        (501) staff       (20)      295 2024-05-02 01:56:16.000000 sesql-2024.5.0/seSql/_version.py
+drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-05-02 01:56:19.033599 sesql-2024.5.0/seSql/dbc/
+-rw-r--r--   0 rjd        (501) staff       (20)     3099 2024-05-02 00:10:54.000000 sesql-2024.5.0/seSql/dbc/Exceptions.py
+-rw-r--r--   0 rjd        (501) staff       (20)     8337 2024-04-30 16:02:06.000000 sesql-2024.5.0/seSql/dbc/JDBC.py
+-rw-r--r--   0 rjd        (501) staff       (20)     7574 2024-05-02 01:07:11.000000 sesql-2024.5.0/seSql/dbc/ODBC.py
+-rw-r--r--   0 rjd        (501) staff       (20)     6174 2024-05-02 01:45:48.000000 sesql-2024.5.0/seSql/dbc/ODBCError.py
+-rw-r--r--   0 rjd        (501) staff       (20)      726 2024-04-01 01:40:37.000000 sesql-2024.5.0/seSql/dbc/Utilities.py
+-rw-r--r--   0 rjd        (501) staff       (20)        0 2024-03-17 19:54:29.000000 sesql-2024.5.0/seSql/dbc/__init__.py
+drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-05-02 01:56:19.033691 sesql-2024.5.0/seSql/dbc/jars/
+-rw-r--r--   0 rjd        (501) staff       (20)  1438398 2024-03-01 01:47:02.000000 sesql-2024.5.0/seSql/dbc/jars/mssql-jdbc-12.4.2.jre8.jar
+-rw-r--r--   0 rjd        (501) staff       (20)     4543 2024-05-02 00:16:41.000000 sesql-2024.5.0/seSql/sql.py
+drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-05-02 01:56:19.037520 sesql-2024.5.0/sesql.egg-info/
+-rw-r--r--   0 rjd        (501) staff       (20)    13704 2024-05-02 01:56:19.000000 sesql-2024.5.0/sesql.egg-info/PKG-INFO
+-rw-r--r--   0 rjd        (501) staff       (20)      485 2024-05-02 01:56:19.000000 sesql-2024.5.0/sesql.egg-info/SOURCES.txt
+-rw-r--r--   0 rjd        (501) staff       (20)        1 2024-05-02 01:56:19.000000 sesql-2024.5.0/sesql.egg-info/dependency_links.txt
+-rw-r--r--   0 rjd        (501) staff       (20)       42 2024-05-02 01:56:19.000000 sesql-2024.5.0/sesql.egg-info/requires.txt
+-rw-r--r--   0 rjd        (501) staff       (20)        6 2024-05-02 01:56:19.000000 sesql-2024.5.0/sesql.egg-info/top_level.txt
+-rw-r--r--   0 rjd        (501) staff       (20)       38 2024-05-02 01:56:19.038016 sesql-2024.5.0/setup.cfg
+drwxr-xr-x   0 rjd        (501) staff       (20)        0 2024-05-02 01:56:19.037201 sesql-2024.5.0/tests/
+-rw-r--r--   0 rjd        (501) staff       (20)     2228 2024-05-02 00:20:20.000000 sesql-2024.5.0/tests/test_Exceptions.py
+-rw-r--r--   0 rjd        (501) staff       (20)     1715 2024-05-02 00:49:31.000000 sesql-2024.5.0/tests/test_jdbc.py
+-rw-r--r--   0 rjd        (501) staff       (20)     1566 2024-05-02 00:54:51.000000 sesql-2024.5.0/tests/test_odbc.py
+-rw-r--r--   0 rjd        (501) staff       (20)      238 2024-04-01 01:39:41.000000 sesql-2024.5.0/tests/test_utilities.py
```

### Comparing `sesql-2024.4.1rc1/License.md` & `sesql-2024.5.0/License.md`

 * *Files identical despite different names*

### Comparing `sesql-2024.4.1rc1/pyproject.toml` & `sesql-2024.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -12,22 +12,21 @@
 authors = [
     { name = "Cybernetic Innovations", email = "github@cyberneticinnovations.com" }
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
-    "loguru>=0.7.2",
     "JayDeBeApi~=1.2.3",
     "pyodbc~=5.1.0",
     "seversion"
 ]
 
 [tool.setuptools]
-packages = ["seCore", "seSql", "seSql.dbc"]
+packages = ["seSql", "seSql.dbc"]
 
 #[tool.setuptools.packages.find]
 #where = ["seCore"]
 #
 [tool.setuptools.package-data]
 seSql = ["dbc/jars/*.jar"]
```

### Comparing `sesql-2024.4.1rc1/seSql/dbc/Exceptions.py` & `sesql-2024.5.0/seSql/dbc/Exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,23 @@
     def __init__(self, message: str) -> None:
         self.message = message
 
     def __str__(self) -> str:
         return str(self.message)
 
 
+class JDBCConnection(Exception):
+    """Exception raised for jaydebeapi.Error."""
+    def __init__(self, message: str) -> None:
+        self.message = message
+
+    def __str__(self) -> str:
+        return str(self.message)
+
+
 class JDBCLoginFailed(Exception):
     """Exception raised for Login failed for user/pw"""
     def __init__(self, message: str) -> None:
         self.message = message
 
     def __str__(self) -> str:
         return str(self.message)
@@ -64,7 +73,25 @@
 class ODBCDriverError(Exception):
     """Exception raised for anything not caught by ODBC driver"""
     def __init__(self, message: str) -> None:
         self.message = message
 
     def __str__(self) -> str:
         return str(self.message)
+
+
+class SQLQueryException(Exception):
+    """Exception raised for anything caught by an SQL query."""
+    def __init__(self, message: str) -> None:
+        self.message = message
+
+    def __str__(self) -> str:
+        return str(self.message)
+
+
+class SQLConnectionException(Exception):
+    """Exception raised for anything caught by an SQL query."""
+    def __init__(self, message: str) -> None:
+        self.message = message
+
+    def __str__(self) -> str:
+        return str(self.message)
```

### Comparing `sesql-2024.4.1rc1/seSql/dbc/JDBC.py` & `sesql-2024.5.0/seSql/dbc/JDBC.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import time
 
 import jaydebeapi
 import inspect
 import json
 import glob
 
-from seCore.CustomLogging import logger
-from seSql.dbc.Exceptions import JDBCConnectionReset, JDBCSecureConnection, JDBCLoginFailed, JDBCConnectionTimeOut, JDBCSQLServerDriver
+from seSql.dbc.Exceptions import JDBCConnectionReset, JDBCSecureConnection, JDBCLoginFailed, JDBCConnectionTimeOut, JDBCSQLServerDriver, JDBCConnection
 from seSql.dbc.Utilities import mask
 
 jdbcDrivers = {
     "mssql-12.2.0": {
         "classname": "com.microsoft.sqlserver.jdbc.SQLServerDriver",
         "jar": "mssql-jdbc-12.2.0.jre8.jar"
     },
@@ -83,14 +82,15 @@
             "user": user,
             "password": password,
             "encrypt": encrypt,
             "trustServerCertificate": trustServerCertificate
         }
         self.__cnxn = None
         self.isConnected = False
+        self.connStats = None
 
     def connect(self) -> bool:
         driver = getDriverSettings()
         args = {
             "user": self.__connStr["user"],
             "password": self.__connStr["password"]
         }
@@ -102,15 +102,26 @@
                 driver['classname'],
                 f'{self.__connStr["server"]}:{self.__connStr["port"]};encrypt={self.__connStr["encrypt"]};trustServerCertificate={self.__connStr["trustServerCertificate"]};',
                 args,
                 f"{ROOT}/jars/{driver['jar']}")
             self.isConnected = True
 
         except jaydebeapi.Error as e:  # pragma: no cover
-            logger.error(f'jayError: {e}')
+            oJson = {
+                f'jdbc-{inspect.currentframe().f_code.co_name}': {
+                    'connection_ms': float(f'{(time.time() - start_time) * 1000:.2f}'),
+                    'connected': self.isConnected,
+                    'error': {
+                        'exception': 'jayError',
+                        'details': f'{e}'
+                    }
+                }
+            }
+            raise JDBCConnection(json.dumps(oJson))
+
         except Exception as e:  # pragma: no cover
             oJson = {
                 f'jdbc-{inspect.currentframe().f_code.co_name}': {
                     'connection_ms': float(f'{(time.time() - start_time) * 1000:.2f}'),
                     'connected': self.isConnected,
                     'error': {}
                 }
@@ -147,45 +158,54 @@
             f'jdbc-{inspect.currentframe().f_code.co_name}': {
                 'connection_ms': float(f'{(time.time() - start_time) * 1000:.2f}'),
                 'connected': self.isConnected,
                 'connStr': self.__connStr
             }}
 
         oJson[f'jdbc-{inspect.currentframe().f_code.co_name}']['connStr']['password'] = mask(oJson[f'jdbc-{inspect.currentframe().f_code.co_name}']['connStr']['password'])
-        logger.info(json.dumps(oJson))
+        # todo: verify if still needed
+        # logger.info(json.dumps(oJson))
+
+        self.connStats = json.dumps(oJson)
 
         return self.isConnected
 
-    def query(self, query: str):
+    def query(self, query: str, stats: bool = False):
         if self.isConnected:
             start_time = time.time()
             try:
                 with self.__cnxn.cursor() as curs:
                     curs.execute(query)
                     if curs.rowcount == -1:
                         r = [dict((curs.description[i][0], value)
                                   for i, value in enumerate(row)) for row in curs.fetchall()]
                         rCount = len(r)
                     else:
                         r = None
                         rCount = curs.rowcount
 
-                    logger.info(json.dumps({
+                    s = json.dumps({
                         f'jdbc-{inspect.currentframe().f_code.co_name}': {
                             'connection_ms': float(f'{(time.time() - start_time) * 1000:.2f}'),
                             'rc': f'{curs.rowcount}:{rCount}',
                             'query': f'{query}'
-                        }}))
-                return r
+                        }})
+
+                if stats:
+                    return {'results': r, 'stats': s}
+                else:
+                    return r
+
             except Exception as e:
-                logger.error(json.dumps({
+                # todo: verify if still needed
+                oE = json.dumps({
                     f'jdbc-{inspect.currentframe().f_code.co_name}': {
                         'connection_ms': float(f'{(time.time() - start_time) * 1000:.2f}'),
                         'query': f'{query}',
                         'error': f'{e}'
-                    }}))
+                    }})
 
-                raise Exception(f'{e}')
+                raise Exception(f'{oE}')
 
     @property
     def connectionString(self):  # pragma: no cover
         return self.__connStr
```

### Comparing `sesql-2024.4.1rc1/seSql/dbc/ODBC.py` & `sesql-2024.5.0/seSql/dbc/ODBC.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 try:
     import pyodbc
     _pyodbc_available = True
 except ImportError:  # pragma: no cover
     _pyodbc_available = False
 
-from seCore.CustomLogging import logger
 
 validDrivers = ['ODBC Driver 18 for SQL Server', 'ODBC Driver 17 for SQL Server']
 
 
 def odbcLoaded() -> bool:
     """
     Checks if the ODBC driver is loaded
@@ -67,23 +66,24 @@
             "user": user,
             "password": password,
             "trust": trust,
             "mars": mars
         }
         self.isConnected = False
         self.__cnxn = None
+        self.connStats = None
 
     def connect(self):
         """
         Connect to database using pyodbc and ODBC Driver 17 or 18 for SQL Server
         """
         start_time = time.time()
 
         match self.__connStr["trust"]:
-            case "yes":
+            case "yes":  # pragma: no cover
                 connStr = f'DRIVER={{{self.__connStr["driver"]}}}; ' \
                           f'Server={self.__connStr["server"]},{self.__connStr["port"]}; ' \
                           f'DATABASE={self.__connStr["database"]}; ' \
                           f'UID={self.__connStr["user"]}; ' \
                           f'PWD={self.__connStr["password"]}; ' \
                           f'Trusted_Connection={self.__connStr["trust"]};'\
                           f'MARS_Connection={self.__connStr["mars"]};'
@@ -135,44 +135,52 @@
         oJson = {
             f'odbc-{inspect.currentframe().f_code.co_name}': {
                 'connection_ms': float(f'{(time.time() - start_time) * 1000:.2f}'),
                 'connected': self.isConnected,
                 'connStr': self.__connStr
             }}
         oJson[f'odbc-{inspect.currentframe().f_code.co_name}']['connStr']['password'] = mask(oJson[f'odbc-{inspect.currentframe().f_code.co_name}']['connStr']['password'])
-        logger.info(json.dumps(oJson))
+        # todo: verify if still needed
+        # logger.info(json.dumps(oJson))
+        self.connStats = json.dumps(oJson)
 
         return self.isConnected
 
-    def query(self, query: str):
+    def query(self, query: str, stats: bool = False):
         if self.isConnected:
             start_time = time.time()
             try:
                 with self.__cnxn.cursor() as cur:
                     cur.execute(query)
                     if cur.rowcount == -1:
                         r = [dict((cur.description[i][0], value)
                                   for i, value in enumerate(row)) for row in cur.fetchall()]
                         rCount = len(r)
                     else:
                         r = None
                         rCount = cur.rowcount
-                    logger.info(json.dumps({
+                    s = json.dumps({
                         f'odbc-{inspect.currentframe().f_code.co_name}': {
                             'connection_ms': float(f'{(time.time() - start_time) * 1000:.2f}'),
                             'rc': f'{cur.rowcount}:{rCount}',
                             'query': f'{query}'
-                        }}))
-                return r
+                        }})
+
+                if stats:
+                    return {'results': r, 'stats': s}
+                else:
+                    return r
+
             except pyodbc.Error as e:  # pragma: no cover
-                logger.error(json.dumps({
+                # todo: need to return
+                oE = json.dumps({
                     f'odbc-{inspect.currentframe().f_code.co_name}': {
                         'connection_ms': float(f'{(time.time() - start_time) * 1000:.2f}'),
                         'query': f'{query}',
                         'error': f'{e}'
-                    }}))
+                    }})
 
-                raise Exception(f'{e}')
+                raise Exception(f'{oE}')
 
     @property
     def connectionString(self):  # pragma: no cover
         return self.__connStr
```

### Comparing `sesql-2024.4.1rc1/seSql/dbc/ODBCError.py` & `sesql-2024.5.0/seSql/dbc/ODBCError.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import re
 
 
-class PyODBCError(Exception):
+class PyODBCError(Exception):  # pragma: no cover
     """
-    Handle errors for PyODBC. Offers a error message parser
+    Handle errors for PyODBC. Offers an error message parser
     to apply specific logic depending on the error raise
 
     ODBC error identifier: 23000
 
     pyodbc_error_message (str) -- message raised by PyODBC
         Example:
             [23000] [Microsoft][ODBC Driver 17 for SQL Server][SQL Server] \
             Cannot insert explicit value for identity column in table \
             'building' when IDENTITY_INSERT is set to OFF.
             (544) (SQLExecDirectW) \
     """
 
     error_pattern = re.compile(
         # r"\[(?P<error_id>.*?)\] \[(?P<operator>.*?)\]\[(?P<driver>.*?)\]\[(?P<database_type>.*?)\](?P<error_message>.+?(?= \()) \((?P<sql_server_error_id>\d*?)\) \(SQLExecDirectW\)"
-        r"\[(?P<error_id>.*?)\] \[(?P<database_type>.*?)\]\[(?P<driver>.*?)\](?P<error_message>.+?(?= \()) \((?P<sql_server_error_id>\d*?)\) \((?P<sql_type>.*?)\)"
+        r"\[(?P<error_id>.*?)] \[(?P<database_type>.*?)]\[(?P<driver>.*?)](?P<error_message>.+?(?= \()) \((?P<sql_server_error_id>\d*?)\) \((?P<sql_type>.*?)\)"
     )
     sql_error_code_pattern = re.compile(r"\((?P<sql_server_error_code>\d*?)\) \(SQLExecDirectW\)")
     column_pattern = re.compile(r"column \'(?P<column_name>.+?)\'")
     table_pattern = re.compile(r"table \'(?P<table_name>.+?)\'")
     pyodbc_error_code = 'HY000'
 
     def __init__(self, pyodbc_error_message: str) -> None:
@@ -74,14 +74,16 @@
             (544) (SQLExecDirectW) -> 544
 
         Args:
             pyodbc_error_message (str): Error string raised by PyODBC
 
         Returns:
             (int) - SQL Server Error Code
+            :param message:
+            :param pyodbc_code:
         """
 
         if pyodbc_code == cls.pyodbc_error_code:
             return 32
         else:
             m = re.search(cls.sql_error_code_pattern, message)
             if m:
@@ -94,88 +96,88 @@
         pyodbc_code = cls.get_pyodbc_code(pyodbc_exception)
         error_message = cls.get_message(pyodbc_exception)
         error_code = cls.get_sql_server_error_code(pyodbc_code, error_message)
         exception = cls.get_exception(error_code)
         raise exception(error_message)
 
 
-class IdentityInsertNull(PyODBCError):
+class IdentityInsertNull(PyODBCError):  # pragma: no cover
     """
     Handle specific PyODBC error related to Null Value Inserted on Identity Column
     """
 
     def __init__(self, pyodbc_error_message):
         super().__init__(pyodbc_error_message)
         m = re.search(self.table_pattern, self.error_message)
         self.table_name = m.group('table_name')
         m = re.search(self.column_pattern, self.error_message)
         self.column_name = m.group('column_name')
 
 
-class IdentityInsertSetToOff(PyODBCError):
+class IdentityInsertSetToOff(PyODBCError):  # pragma: no cover
     """
     Handle specific PyODBC error related to Identity Not Set to On/Off
     """
 
     def __init__(self, pyodbc_error_message):
         super().__init__(pyodbc_error_message)
         m = re.search(self.table_pattern, self.error_message)
         self.table_name = m.group('table_name')
 
 
-class FailedTypeConversion(PyODBCError):
+class FailedTypeConversion(PyODBCError):  # pragma: no cover
     """
     Handle specific PyODBC error related to data type conversion
     """
 
     def __init__(self, pyodbc_error_message):
         super().__init__(pyodbc_error_message)
 
 
-class PrimaryKeyViolation(PyODBCError):
+class PrimaryKeyViolation(PyODBCError):  # pragma: no cover
     """
     Handle specific PyODBC error related to Primary Key Violation
     """
 
     def __init__(self, pyodbc_error_message):
         super().__init__(pyodbc_error_message)
 
 
-class IncorrectSyntax(PyODBCError):
+class IncorrectSyntax(PyODBCError):  # pragma: no cover
     """
     Handle specific PyODBC error related to incorrect syntax in query
     """
 
     def __init__(self, pyodbc_error_message):
         super().__init__(pyodbc_error_message)
 
 
-class DefaultExceptionId(PyODBCError):
+class DefaultExceptionId(PyODBCError):  # pragma: no cover
     """
     Handle default PyODBC errors
     """
 
     def __init__(self, pyodbc_error_message):
         super().__init__(pyodbc_error_message)
 
     def __str__(self) -> str:
         return f"{self.sql_server_error_id}"
 
 
-class DefaultException(PyODBCError):
+class DefaultException(PyODBCError):  # pragma: no cover
     """
     Handle default PyODBC errors
     """
 
     def __init__(self, pyodbc_error_message):
         super().__init__(pyodbc_error_message)
 
     def __str__(self) -> str:
         return f"{self.error_message}"
 
 
-class InvalidNumberParametersSupplied(Exception):
+class InvalidNumberParametersSupplied(Exception):  # pragma: no cover
     def __init__(self, error_message) -> None:
         self.message = error_message
 
     def __str__(self) -> str:
         return self.message
```

### Comparing `sesql-2024.4.1rc1/seSql/dbc/Utilities.py` & `sesql-2024.5.0/seSql/dbc/Utilities.py`

 * *Files identical despite different names*

### Comparing `sesql-2024.4.1rc1/seSql/dbc/jars/mssql-jdbc-12.4.2.jre8.jar` & `sesql-2024.5.0/seSql/dbc/jars/mssql-jdbc-12.4.2.jre8.jar`

 * *Files identical despite different names*

### Comparing `sesql-2024.4.1rc1/seSql/sql.py` & `sesql-2024.5.0/seSql/sql.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 import json
 
 from typing import Optional
-from seCore.CustomLogging import logger
+
+from .dbc.Exceptions import SQLConnectionException, SQLQueryException
 from .dbc.JDBC import jdbcLoaded, jdbcDriver, jdbcEngine
 from .dbc.ODBC import odbcLoaded, odbcDriver, odbcEngine
 
 
 class sql:
     def __init__(self):
         self.__cnxn = None
         self.__isConnected = False
         self.__driverOverride = None
         self.__jdbcDriver = None
         self.__jdbcLoaded = None
         self.__odbcDriver = None
         self.__odbcLoaded = None
         self.__connStr = None
+        self.__connStatus = None
+        self.__connStats = None
 
     def connect(self,
                 server: Optional[str] = None,
                 port: Optional[int] = None,
                 user: Optional[str] = None,
                 password: Optional[str] = None,
                 trust: Optional[str] = None,
                 db: Optional[str] = "",
                 trustServerCertificate: Optional[bool] = True,
                 mars: Optional[str] = 'no',
-                driverOverride: Optional[str] = None
+                driverOverride: Optional[str] = None,
                 ):
 
         self.__odbcLoaded = odbcLoaded()
         self.__odbcDriver = odbcDriver()
         self.__jdbcLoaded = jdbcLoaded()
         self.__jdbcDriver = jdbcDriver()
         self.__driverOverride = driverOverride.lower() if driverOverride.lower() in ["odbc", "jdbc"] else "odbc"
@@ -66,37 +69,41 @@
                     mars=self.__connStr['mars'],
                 )
                 self._logging()
 
                 try:
                     self.__cnxn.connect()
                     self.__isConnected = self.__cnxn.isConnected
+                    self.__connStats = self.__cnxn.connStats
                 except Exception as e:  # pragma: no cover
-                    logger.error(e)
+                    raise SQLConnectionException(f'{e}')
 
             case _:
                 self.__cnxn = jdbcEngine(
                     server=self.__connStr['server'],
                     port=self.__connStr['port'],
                     user=self.__connStr['user'],
                     password=self.__connStr['password'],
                     trustServerCertificate=self.__connStr['trustServerCertificate']
                 )
                 self._logging()
 
                 try:
                     self.__cnxn.connect()
                     self.__isConnected = self.__cnxn.isConnected
+                    self.__connStats = self.__cnxn.connStats
                 except Exception as e:  # pragma: no cover
-                    logger.error(e)
+                    raise SQLConnectionException(f'{e}')
 
     def query(self,
-              query: str):
+              query: str,
+              stats: bool = False
+              ):
         try:
-            return self.__cnxn.query(query)
+            return self.__cnxn.query(query, stats=stats)
         except Exception as e:
             raise SQLQueryException(f'{e}')
 
     def _logging(self):
         oSqlDriver = {
             "driver-info":
                 {
@@ -107,23 +114,23 @@
                     },
                     "jdbc": {
                         "loaded": self.__jdbcLoaded,
                         "driver": self.__jdbcDriver
                     }
                 }
         }
-        logger.info(f'{json.dumps(oSqlDriver)}')
-
+        self.__connStatus = json.dumps(oSqlDriver)
 
     @property
     def isConnected(self) -> bool:
-        # return self.__isConnected
-        return True
+        return self.__isConnected
+        # return True
 
+    @property
+    def ConnectedStatus(self):
 
-class SQLQueryException(Exception):
-    """Exception raised for anything caught by an SQL query."""
-    def __init__(self, message: str) -> None:
-        self.message = message
+        return self.__connStatus
+
+    @property
+    def ConnectedStats(self):
 
-    def __str__(self) -> str:
-        return str(self.message)
+        return self.__connStats
```

### Comparing `sesql-2024.4.1rc1/tests/test_Exceptions.py` & `sesql-2024.5.0/tests/test_Exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from seSql.dbc.Exceptions import ODBCLoginFailed, JDBCSecureConnection, JDBCLoginFailed, JDBCConnectionTimeOut, JDBCSQLServerDriver, JDBCConnectionReset, ODBCInvalidOperation, ODBCDriverError
+from seSql.dbc.Exceptions import ODBCLoginFailed, JDBCSecureConnection, JDBCLoginFailed, JDBCConnectionTimeOut, JDBCSQLServerDriver, JDBCConnectionReset, ODBCInvalidOperation, ODBCDriverError, JDBCConnection, SQLConnectionException
 
 
 def test_odbcLogin_failed():
     try:
         raise ODBCLoginFailed('ODBCLoginFailed')
     except ODBCLoginFailed as e:
         print(e)
@@ -59,7 +59,23 @@
 
 def test_jdbcConnectionReset():
     try:
         raise JDBCConnectionReset('JDBCConnectionReset')
     except JDBCConnectionReset as e:
         print(e)
         assert e.message == 'JDBCConnectionReset'
+
+
+def test_jdbcConnection():
+    try:
+        raise JDBCConnection('JDBCConnection')
+    except JDBCConnection as e:
+        print(e)
+        assert e.message == 'JDBCConnection'
+
+
+def test_sqlConnectionException():
+    try:
+        raise SQLConnectionException('SQLConnectionException')
+    except SQLConnectionException as e:
+        print(e)
+        assert e.message == 'SQLConnectionException'
```

### Comparing `sesql-2024.4.1rc1/tests/test_jdbc.py` & `sesql-2024.5.0/tests/test_jdbc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+
 from seCore.CustomLogging import logger
 
 from seSql import sql
 from seSql.dbc.JDBC import jdbcLoaded, jdbcDriver
 
 
 def test_jdbc():
@@ -10,14 +12,26 @@
         server="SQL5101.site4now.net",
         port=1433,
         user="db_a82904_cybernetic_admin",
         password="tb7qiwqer8mee68",
         trust="no",
         driverOverride="jdbc"
     )
+    json.dumps({
+        'seSql': {
+            'driver': json.loads(oSql.ConnectedStatus)["driver-info"],
+        }
+    })
+    json.dumps({
+        'seSql': {
+            'ep': 'connect',
+            'stats': json.loads(oSql.ConnectedStats),
+        }
+    })
+
     if oSql.isConnected:
         # oSql.query("SELECT @@version as version")
         oSql.query("select @@version as version")
 
         # oSql.query("select * from dbo.winequality_red;")
 
         try:
@@ -26,14 +40,27 @@
             logger.error(f'Exception: {e}')
 
         try:
             oSql.query("select * from dba.winequality_red;")
         except Exception as e:
             logger.error(f'Exception: {e}')
 
+        try:
+            oResponse = oSql.query("select @@version as version;", stats=True)
+            logger.info(oResponse['stats'])
+            logger.info(oResponse['results'])
+        except Exception as e:
+            logger.error(f'{e}')
+
+        try:
+            oResponse = oSql.query("delete from dbo.seSql_Settings where value like '%dev';")
+            logger.info(oResponse)
+        except Exception as e:
+            logger.error(f'{e}')
+
 
 def test_jdbcLoaded():
     assert jdbcLoaded(3) is False
 
 
 def test_jdbcDriver():
     assert jdbcDriver(3) == "Error finding JDBC driver"
```

### Comparing `sesql-2024.4.1rc1/tests/test_odbc.py` & `sesql-2024.5.0/tests/test_odbc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,60 @@
-from seCore.CustomLogging import logger
+import json
 
+from seCore.CustomLogging import logger
 from seSql import sql, mask, seSqlVersion, hostName, hostIP
 
 
 def test_jdbc():
     oSql = sql()
     oSql.connect(
         server="SQL5101.site4now.net",
         port=1433,
         user="db_a82904_cybernetic_admin",
         password="tb7qiwqer8mee68",
         trust="no",
         driverOverride="odbc"
     )
+    json.dumps({
+        'seSql': {
+            'driver': json.loads(oSql.ConnectedStatus)["driver-info"],
+        }
+    })
+    json.dumps({
+        'seSql': {
+            'ep': 'connect',
+            'stats': json.loads(oSql.ConnectedStats),
+        }
+    })
 
     if oSql.isConnected:
         # oSql.query("SELECT @@version as version")
         oSql.query("select @@version as version")
 
         # oSql.query("select * from dbo.winequality_red;")
 
         try:
             oSql.query("select * from dbo.winequality_red;")
         except Exception as e:
             logger.error(f'Exception: {e}')
 
+        try:
+            oSql.query("select * from dba.winequality_red;")
+        except Exception as e:
+            logger.error(f'Exception: {e}')
+
+        try:
+            oResponse = oSql.query("select @@version as version;", stats=True)
+            logger.info(oResponse['stats'])
+            logger.info(oResponse['results'])
+        except Exception as e:
+            logger.error(f'{e}')
+
+        try:
+            oResponse = oSql.query("delete from dbo.seSql_Settings where value like '%dev';")
+            logger.info(oResponse)
+        except Exception as e:
+            logger.error(f'{e}')
+
```

