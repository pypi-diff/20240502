# Comparing `tmp/shipyard_motherduck-0.1.1a1.tar.gz` & `tmp/shipyard_motherduck-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_motherduck-0.1.1a1.tar", max compression
+gzip compressed data, was "shipyard_motherduck-0.1.2.tar", max compression
```

## Comparing `shipyard_motherduck-0.1.1a1.tar` & `shipyard_motherduck-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1389 2024-04-19 17:49:25.468173 shipyard_motherduck-0.1.1a1/README.md
--rw-r--r--   0        0        0      618 2024-04-25 21:18:27.702028 shipyard_motherduck-0.1.1a1/pyproject.toml
--rw-r--r--   0        0        0       41 2024-04-19 17:49:25.469225 shipyard_motherduck-0.1.1a1/shipyard_motherduck/__init__.py
--rw-r--r--   0        0        0      600 2024-04-25 21:17:15.112818 shipyard_motherduck-0.1.1a1/shipyard_motherduck/cli/authtest.py
--rw-r--r--   0        0        0     1088 2024-04-19 17:49:25.469563 shipyard_motherduck-0.1.1a1/shipyard_motherduck/cli/execute.py
--rw-r--r--   0        0        0     1880 2024-04-19 17:49:25.469691 shipyard_motherduck-0.1.1a1/shipyard_motherduck/cli/fetch.py
--rw-r--r--   0        0        0     3061 2024-04-19 17:49:25.469825 shipyard_motherduck-0.1.1a1/shipyard_motherduck/cli/upload.py
--rw-r--r--   0        0        0      865 2024-04-19 17:49:25.469968 shipyard_motherduck-0.1.1a1/shipyard_motherduck/exceptions.py
--rw-r--r--   0        0        0     7097 2024-04-19 17:49:25.470169 shipyard_motherduck-0.1.1a1/shipyard_motherduck/motherduck.py
--rw-r--r--   0        0        0     2049 1970-01-01 00:00:00.000000 shipyard_motherduck-0.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0     1389 2024-04-19 17:49:25.468173 shipyard_motherduck-0.1.2/README.md
+-rw-r--r--   0        0        0      616 2024-05-02 18:21:34.859680 shipyard_motherduck-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-04-19 17:49:25.469225 shipyard_motherduck-0.1.2/shipyard_motherduck/__init__.py
+-rw-r--r--   0        0        0      628 2024-04-29 16:36:13.921478 shipyard_motherduck-0.1.2/shipyard_motherduck/cli/authtest.py
+-rw-r--r--   0        0        0     1088 2024-04-19 17:49:25.469563 shipyard_motherduck-0.1.2/shipyard_motherduck/cli/execute.py
+-rw-r--r--   0        0        0     1880 2024-04-19 17:49:25.469691 shipyard_motherduck-0.1.2/shipyard_motherduck/cli/fetch.py
+-rw-r--r--   0        0        0     3061 2024-05-02 18:22:41.419375 shipyard_motherduck-0.1.2/shipyard_motherduck/cli/upload.py
+-rw-r--r--   0        0        0      865 2024-04-19 17:49:25.469968 shipyard_motherduck-0.1.2/shipyard_motherduck/exceptions.py
+-rw-r--r--   0        0        0     7230 2024-05-02 18:28:34.884583 shipyard_motherduck-0.1.2/shipyard_motherduck/motherduck.py
+-rw-r--r--   0        0        0     2047 1970-01-01 00:00:00.000000 shipyard_motherduck-0.1.2/PKG-INFO
```

### Comparing `shipyard_motherduck-0.1.1a1/README.md` & `shipyard_motherduck-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.1a1/shipyard_motherduck/cli/authtest.py` & `shipyard_motherduck-0.1.2/shipyard_motherduck/cli/authtest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import sys
 import duckdb
 from shipyard_motherduck import MotherDuckClient
 from shipyard_templates import ShipyardLogger
 
 logger = ShipyardLogger.get_logger()
+logger.setLevel("AUTHTEST")
 
 
 def main():
     try:
         client = MotherDuckClient(os.getenv("MOTHERDUCK_TOKEN"))
         client.connect()
         logger.authtest("Successfully connected to MotherDuck")
```

### Comparing `shipyard_motherduck-0.1.1a1/shipyard_motherduck/cli/execute.py` & `shipyard_motherduck-0.1.2/shipyard_motherduck/cli/execute.py`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.1a1/shipyard_motherduck/cli/fetch.py` & `shipyard_motherduck-0.1.2/shipyard_motherduck/cli/fetch.py`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.1a1/shipyard_motherduck/cli/upload.py` & `shipyard_motherduck-0.1.2/shipyard_motherduck/cli/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             )
 
         if args.match_type in ["glob_match", "regex_match"]:
             file_matches = shipyard.files.find_matching_files(
                 file_name, directory, match_type=args.match_type
             )
 
-            if n_matches := (len(file_matches)) == 0:
+            if (n_matches := len(file_matches)) == 0:
                 logger.error(f"No file matches found for pattern {file_name}")
                 sys.exit(Database.EXIT_CODE_FILE_NOT_FOUND)
             logger.info(f"Found {n_matches} file matches, preparing to upload...")
             for file in file_matches:
                 logger.debug(f"Uploading {file}")
                 client.upload(table_name, file, insert_method=insert_method)
                 if insert_method == "replace":
```

### Comparing `shipyard_motherduck-0.1.1a1/shipyard_motherduck/exceptions.py` & `shipyard_motherduck-0.1.2/shipyard_motherduck/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_motherduck-0.1.1a1/shipyard_motherduck/motherduck.py` & `shipyard_motherduck-0.1.2/shipyard_motherduck/motherduck.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,18 @@
 
         Raises:
             ConnectionError: If there is an error connecting to the MotherDuck database.
         """
         try:
             conn = duckdb.connect(self._conn_str)
         except Exception as e:
-            raise ConnectionError(f"Failed to connect to MotherDuck: {e}")
+            logger.debug(f"Connection Error. Message from the Server: {e}")
+            raise ConnectionError(
+                f"Failed to connect to MotherDuck. Ensure that the token is valid"
+            )
         else:
             logger.info("Successfully connected to MotherDuck")
             return conn
 
     def upload(self, table_name: str, file_path: str, insert_method: str = "replace"):
         """
         Uploads data from a file to a specified table in the database.
```

### Comparing `shipyard_motherduck-0.1.1a1/PKG-INFO` & `shipyard_motherduck-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-motherduck
-Version: 0.1.1a1
+Version: 0.1.2
 Summary: A local client for working with Python and MotherDuck
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

