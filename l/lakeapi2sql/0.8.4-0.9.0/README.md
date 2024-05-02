# Comparing `tmp/lakeapi2sql-0.8.4.tar.gz` & `tmp/lakeapi2sql-0.9.0.tar.gz`

## Comparing `lakeapi2sql-0.8.4.tar` & `lakeapi2sql-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 lakeapi2sql-0.8.4/Cargo.toml
--rw-r--r--   0     1001      127      118 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/.editorconfig
--rw-r--r--   0     1001      127     2966 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/.github/workflows/CI.yml
--rw-r--r--   0     1001      127     3110 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/.gitignore
--rw-r--r--   0     1001      127       76 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/.vscode/settings.json
--rw-r--r--   0     1001      127     1081 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/LICENSE
--rw-r--r--   0     1001      127     1388 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/README.md
--rw-r--r--   0     1001      127        0 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/lakeapi2sql/__init__.py
--rw-r--r--   0     1001      127     3102 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/lakeapi2sql/bulk_insert.py
--rw-r--r--   0     1001      127        0 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/py.typed
--rw-r--r--   0     1001      127    22276 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/src/arrow_convert.rs
--rw-r--r--   0     1001      127     5134 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/src/bulk_insert.rs
--rw-r--r--   0     1001      127     2123 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/src/connect.rs
--rw-r--r--   0     1001      127     1705 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/src/error.rs
--rw-r--r--   0     1001      127     4862 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/src/lib.rs
--rw-r--r--   0     1001      127        0 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/test/__init__.py
--rw-r--r--   0     1001      127     1649 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/test/test_insert.py
--rw-r--r--   0     1001      127     1667 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/test/test_insert_reader.py
--rw-r--r--   0     1001      127    70255 2024-05-01 09:04:13.000000 lakeapi2sql-0.8.4/Cargo.lock
--rw-r--r--   0     1001      127      693 2024-05-01 09:04:08.000000 lakeapi2sql-0.8.4/pyproject.toml
--rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 lakeapi2sql-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1461 1970-01-01 00:00:00.000000 lakeapi2sql-0.9.0/Cargo.toml
+-rw-r--r--   0     1001      127      118 2024-05-02 15:47:45.000000 lakeapi2sql-0.9.0/.editorconfig
+-rw-r--r--   0     1001      127     2966 2024-05-02 15:47:45.000000 lakeapi2sql-0.9.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127     3110 2024-05-02 15:47:45.000000 lakeapi2sql-0.9.0/.gitignore
+-rw-r--r--   0     1001      127       76 2024-05-02 15:47:45.000000 lakeapi2sql-0.9.0/.vscode/settings.json
+-rw-r--r--   0     1001      127     1081 2024-05-02 15:47:45.000000 lakeapi2sql-0.9.0/LICENSE
+-rw-r--r--   0     1001      127     1388 2024-05-02 15:47:45.000000 lakeapi2sql-0.9.0/README.md
+-rw-r--r--   0     1001      127       96 2024-05-02 15:47:45.000000 lakeapi2sql-0.9.0/lakeapi2sql/__init__.py
+-rw-r--r--   0     1001      127     1280 2024-05-02 15:47:45.000000 lakeapi2sql-0.9.0/lakeapi2sql/bulk_insert.py
+-rw-r--r--   0     1001      127     1038 2024-05-02 15:47:45.000000 lakeapi2sql-0.9.0/lakeapi2sql/sql_connection.py
+-rw-r--r--   0     1001      127     1894 2024-05-02 15:47:45.000000 lakeapi2sql-0.9.0/lakeapi2sql/utils.py
+-rw-r--r--   0     1001      127        0 2024-05-02 15:47:45.000000 lakeapi2sql-0.9.0/py.typed
+-rw-r--r--   0     1001      127    22276 2024-05-02 15:47:45.000000 lakeapi2sql-0.9.0/src/arrow_convert.rs
+-rw-r--r--   0     1001      127     5134 2024-05-02 15:47:45.000000 lakeapi2sql-0.9.0/src/bulk_insert.rs
+-rw-r--r--   0     1001      127     2123 2024-05-02 15:47:45.000000 lakeapi2sql-0.9.0/src/connect.rs
+-rw-r--r--   0     1001      127     1705 2024-05-02 15:47:45.000000 lakeapi2sql-0.9.0/src/error.rs
+-rw-r--r--   0     1001      127    14118 2024-05-02 15:47:45.000000 lakeapi2sql-0.9.0/src/lib.rs
+-rw-r--r--   0     1001      127        0 2024-05-02 15:47:45.000000 lakeapi2sql-0.9.0/test/__init__.py
+-rw-r--r--   0     1001      127     1649 2024-05-02 15:47:45.000000 lakeapi2sql-0.9.0/test/test_insert.py
+-rw-r--r--   0     1001      127     1667 2024-05-02 15:47:45.000000 lakeapi2sql-0.9.0/test/test_insert_reader.py
+-rw-r--r--   0     1001      127    70255 2024-05-02 15:47:56.000000 lakeapi2sql-0.9.0/Cargo.lock
+-rw-r--r--   0     1001      127      693 2024-05-02 15:47:45.000000 lakeapi2sql-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 lakeapi2sql-0.9.0/PKG-INFO
```

### Comparing `lakeapi2sql-0.8.4/Cargo.toml` & `lakeapi2sql-0.9.0/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "lake2sql"
-version = "0.8.3"
+version = "0.9.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "lake2sql"
 crate-type = ["lib", "cdylib"]
```

### Comparing `lakeapi2sql-0.8.4/.github/workflows/CI.yml` & `lakeapi2sql-0.9.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.4/.gitignore` & `lakeapi2sql-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.4/LICENSE` & `lakeapi2sql-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.4/README.md` & `lakeapi2sql-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.4/lakeapi2sql/bulk_insert.py` & `lakeapi2sql-0.9.0/lakeapi2sql/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,11 @@
 import inspect
-from typing import Awaitable, TypedDict
-import lakeapi2sql._lowlevel as lvd
-import pyarrow as pa
-from pyarrow.cffi import ffi as arrow_ffi
 
 
-class BulkInfoField(TypedDict):
-    name: str
-    arrow_type: str
-
-
-class BulkInfo(TypedDict):
-    fields: list[BulkInfoField]
-
-
-async def _prepare_connection_string(connection_string: str, aad_token: str | None) -> tuple[str, str | None]:
+async def prepare_connection_string(connection_string: str, aad_token: str | None) -> tuple[str, str | None]:
     if "authentication" in connection_string.lower():
         parts = [(kv[0 : kv.index("=")], kv[kv.index("=") + 1 :]) for kv in connection_string.split(";")]
         auth_part = next((p for p in parts if p[0].casefold() == "Authentication".casefold()))
         parts.remove(auth_part)
         credential = None
         auth_method = auth_part[1].lower()
         if auth_method in ["ActiveDirectoryDefault".lower()]:
@@ -42,34 +29,7 @@
             from azure.core.credentials import AccessToken
 
             res = credential.get_token("https://database.windows.net/.default")
             token: AccessToken = await res if inspect.isawaitable(res) else res  # type: ignore
             aad_token = token.token
             return ";".join((p[0] + "=" + p[1] for p in parts)), aad_token
     return connection_string, aad_token
-
-
-async def insert_record_batch_to_sql(
-    connection_string: str,
-    table_name: str,
-    reader: pa.RecordBatchReader,
-    col_names: list[str] | None = None,
-    aad_token: str | None = None,
-):
-    connection_string, aad_token = await _prepare_connection_string(connection_string, aad_token)
-
-    return await lvd.insert_arrow_reader_to_sql(connection_string, reader, table_name, col_names or [], aad_token)
-
-
-async def insert_http_arrow_stream_to_sql(
-    connection_string: str,
-    table_name: str,
-    url: str,
-    basic_auth: tuple[str, str],
-    aad_token: str | None = None,
-    col_names: list[str] | None = None,
-) -> BulkInfo:
-    connection_string, aad_token = await _prepare_connection_string(connection_string, aad_token)
-
-    return await lvd.insert_arrow_stream_to_sql(
-        connection_string, table_name, col_names or [], url, basic_auth[0], basic_auth[1], aad_token
-    )
```

### Comparing `lakeapi2sql-0.8.4/src/arrow_convert.rs` & `lakeapi2sql-0.9.0/src/arrow_convert.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.4/src/bulk_insert.rs` & `lakeapi2sql-0.9.0/src/bulk_insert.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.4/src/connect.rs` & `lakeapi2sql-0.9.0/src/connect.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.4/src/error.rs` & `lakeapi2sql-0.9.0/src/error.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.4/test/test_insert.py` & `lakeapi2sql-0.9.0/test/test_insert.py`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.4/test/test_insert_reader.py` & `lakeapi2sql-0.9.0/test/test_insert_reader.py`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.4/Cargo.lock` & `lakeapi2sql-0.9.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1011,15 +1011,15 @@
 checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lake2sql"
-version = "0.8.3"
+version = "0.9.0"
 dependencies = [
  "arrow",
  "futures",
  "log",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-log",
@@ -1966,26 +1966,26 @@
 name = "semver"
 version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 
 [[package]]
 name = "serde"
-version = "1.0.199"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c9f6e76df036c77cd94996771fb40db98187f096dd0b9af39c6c6e452ba966a"
+checksum = "ddc6f9cc94d67c0e21aaf7eda3a010fd3af78ebf6e096aa6e2e13c79749cce4f"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.199"
+version = "1.0.200"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11bd257a6541e141e42ca6d24ae26f7714887b47e89aa739099104c7e4d3b7fc"
+checksum = "856f046b9400cee3c8c94ed572ecdb752444c24528c035cd35882aad6f492bcb"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
```

### Comparing `lakeapi2sql-0.8.4/pyproject.toml` & `lakeapi2sql-0.9.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "lakeapi2sql"
 requires-python = ">=3.10"
-version = "0.8.4"
+version = "0.9.0"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 dependencies = ["pyarrow >= 8.0.0"]
```

### Comparing `lakeapi2sql-0.8.4/PKG-INFO` & `lakeapi2sql-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: lakeapi2sql
-Version: 0.8.4
+Version: 0.9.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pyarrow >=8.0.0
 Requires-Dist: azure-identity >=1.12.0 ; extra == 'azure'
 Provides-Extra: azure
 License-File: LICENSE
```

