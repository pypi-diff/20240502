# Comparing `tmp/dbfrs-0.1.2.tar.gz` & `tmp/dbfrs-0.1.3.tar.gz`

## Comparing `dbfrs-0.1.2.tar` & `dbfrs-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 dbfrs-0.1.2/Cargo.toml
--rw-r--r--   0     1000     1000       33 2024-04-24 11:48:36.000000 dbfrs-0.1.2/.gitignore
--rw-r--r--   0     1000     1000      115 2024-04-24 11:49:30.000000 dbfrs-0.1.2/CHANGELOG.md
--rw-r--r--   0     1000     1000     1125 2024-04-24 07:40:04.000000 dbfrs-0.1.2/README.md
--rw-r--r--   0     1000     1000      160 2024-04-24 11:10:54.000000 dbfrs-0.1.2/pyvenv.cfg
--rw-r--r--   0     1000     1000     9203 2024-04-24 12:26:24.000000 dbfrs-0.1.2/src/lib.rs
--rw-r--r--   0     1000     1000      286 2024-04-24 12:26:10.000000 dbfrs-0.1.2/tests/test.dbf
--rw-r--r--   0     1000     1000      540 2024-04-24 12:26:08.000000 dbfrs-0.1.2/tests/test_rw.py
--rw-r--r--   0     1000     1000    11928 2024-04-24 13:33:56.000000 dbfrs-0.1.2/Cargo.lock
--rw-r--r--   0     1000     1000      409 2024-04-23 20:56:02.000000 dbfrs-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1542 1970-01-01 00:00:00.000000 dbfrs-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 dbfrs-0.1.3/Cargo.toml
+-rw-r--r--   0     1000     1000       60 2024-05-02 09:48:17.000000 dbfrs-0.1.3/.gitignore
+-rw-r--r--   0     1000     1000      224 2024-05-02 10:59:16.000000 dbfrs-0.1.3/CHANGELOG.md
+-rw-r--r--   0     1000     1000     1424 2024-05-02 11:01:29.000000 dbfrs-0.1.3/README.md
+-rw-r--r--   0     1000     1000     8170 2024-05-02 10:24:12.000000 dbfrs-0.1.3/src/lib.rs
+-rw-r--r--   0     1000     1000     4131 2024-05-02 10:23:34.000000 dbfrs-0.1.3/src/types.rs
+-rw-r--r--   0     1000     1000     1546 2024-05-02 10:21:59.000000 dbfrs-0.1.3/tests/test_rw.py
+-rw-r--r--   0     1000     1000    11928 2024-05-02 11:00:30.000000 dbfrs-0.1.3/Cargo.lock
+-rw-r--r--   0     1000     1000      409 2024-04-23 20:56:02.000000 dbfrs-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1841 1970-01-01 00:00:00.000000 dbfrs-0.1.3/PKG-INFO
```

### Comparing `dbfrs-0.1.2/README.md` & `dbfrs-0.1.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.3
+Name: dbfrs
+Version: 0.1.3
+Classifier: Programming Language :: Rust
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Author: Roland von Ohlen <crates@rvo.name>
+Author-email: Roland von Ohlen <crates@rvo.name>
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+
 # dbfrs
 
 Minimalist DBF reader and writer for Python 3 written in Rust. The state of DBF libraries in 2024
 is abysmal, yet still companies rely on this format.
 This library aims to provide a simple, easy-to-use interface for reading
 and writing DBF files.
 
@@ -12,37 +23,64 @@
 
 ```bash
 pip install dbfrs
 ```
 
 ## Usage
 
-### Reading a file into a DataFrame
+### Reading a file
 
 ```python
 import dbfrs
 import pandas as pd
 
 filename = 'file.dbf'
 
-fields = dbfrs.get_fields_from_file(filename)
+records = dbfrs.load_dbf(filename)
+```
+
+### Reading a file into a DataFrame, only loading specific fields
+
+```python
+import dbfrs
+import pandas as pd
+
+filename = 'file.dbf'
+
+fields = dbfrs.get_dbf_fields(filename)
 records = dbfrs.load_dbf(filename, fields)
 df = pd.DataFrame(records, columns=fields)
 ```
 
 ### Writing a DataFrame to a file
 
 ```python
 import dbfrs
 import pandas as pd
 
 filename = 'file.dbf'
 df = pd.DataFrame({'field1': [1, 2, 3], 'field2': ['a', 'b', 'c']})
 
 fields = dbfrs.Fields()
-fields.add_field('field1', 'N', 10)
-fields.add_field('field2', 'C', 10)
+fields.add_numeric_field('field1', 'N', 10, 0)
+fields.add_character_field('field2', 'C')
 
 records = [tuple(x) for x in df.values.tolist()]
 
 dbfrs.write_dbf(filename, fields, records)
 ```
+
+
+## Development
+
+### Building the Rust library
+
+```bash
+maturin build
+```
+
+### Publish a new version
+
+```bash
+maturin publish
+```
+
```

### Comparing `dbfrs-0.1.2/Cargo.lock` & `dbfrs-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
  "byteorder",
  "time",
  "yore",
 ]
 
 [[package]]
 name = "dbfrs"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "dbase",
  "pyo3",
  "rand",
 ]
 
 [[package]]
```

### Comparing `dbfrs-0.1.2/PKG-INFO` & `dbfrs-0.1.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.3
-Name: dbfrs
-Version: 0.1.2
-Classifier: Programming Language :: Rust
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Author: Roland von Ohlen <crates@rvo.name>
-Author-email: Roland von Ohlen <crates@rvo.name>
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-
 # dbfrs
 
 Minimalist DBF reader and writer for Python 3 written in Rust. The state of DBF libraries in 2024
 is abysmal, yet still companies rely on this format.
 This library aims to provide a simple, easy-to-use interface for reading
 and writing DBF files.
 
@@ -23,38 +12,63 @@
 
 ```bash
 pip install dbfrs
 ```
 
 ## Usage
 
-### Reading a file into a DataFrame
+### Reading a file
+
+```python
+import dbfrs
+import pandas as pd
+
+filename = 'file.dbf'
+
+records = dbfrs.load_dbf(filename)
+```
+
+### Reading a file into a DataFrame, only loading specific fields
 
 ```python
 import dbfrs
 import pandas as pd
 
 filename = 'file.dbf'
 
-fields = dbfrs.get_fields_from_file(filename)
+fields = dbfrs.get_dbf_fields(filename)
 records = dbfrs.load_dbf(filename, fields)
 df = pd.DataFrame(records, columns=fields)
 ```
 
 ### Writing a DataFrame to a file
 
 ```python
 import dbfrs
 import pandas as pd
 
 filename = 'file.dbf'
 df = pd.DataFrame({'field1': [1, 2, 3], 'field2': ['a', 'b', 'c']})
 
 fields = dbfrs.Fields()
-fields.add_field('field1', 'N', 10)
-fields.add_field('field2', 'C', 10)
+fields.add_numeric_field('field1', 'N', 10, 0)
+fields.add_character_field('field2', 'C')
 
 records = [tuple(x) for x in df.values.tolist()]
 
 dbfrs.write_dbf(filename, fields, records)
 ```
 
+
+## Development
+
+### Building the Rust library
+
+```bash
+maturin build
+```
+
+### Publish a new version
+
+```bash
+maturin publish
+```
```

