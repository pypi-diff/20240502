# Comparing `tmp/llama_index_readers_clickhouse-0.1.1.tar.gz` & `tmp/llama_index_readers_clickhouse-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_clickhouse-0.1.1.tar", max compression
+gzip compressed data, was "llama_index_readers_clickhouse-0.1.2.tar", max compression
```

## Comparing `llama_index_readers_clickhouse-0.1.1.tar` & `llama_index_readers_clickhouse-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       45 2024-02-16 04:21:21.890090 llama_index_readers_clickhouse-0.1.1/README.md
--rw-r--r--   0        0        0      188 2024-02-16 04:21:21.890498 llama_index_readers_clickhouse-0.1.1/llama_index/readers/clickhouse/__init__.py
--rw-r--r--   0        0        0     5518 2024-02-16 04:21:21.890799 llama_index_readers_clickhouse-0.1.1/llama_index/readers/clickhouse/base.py
--rw-r--r--   0        0        0     1546 2024-02-21 19:36:48.348743 llama_index_readers_clickhouse-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 llama_index_readers_clickhouse-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1546 2024-05-02 17:02:31.949773 llama_index_readers_clickhouse-0.1.2/README.md
+-rw-r--r--   0        0        0      188 2024-05-02 17:02:31.949773 llama_index_readers_clickhouse-0.1.2/llama_index/readers/clickhouse/__init__.py
+-rw-r--r--   0        0        0     5518 2024-05-02 17:02:31.949773 llama_index_readers_clickhouse-0.1.2/llama_index/readers/clickhouse/base.py
+-rw-r--r--   0        0        0     1481 2024-05-02 17:02:31.949773 llama_index_readers_clickhouse-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 llama_index_readers_clickhouse-0.1.2/PKG-INFO
```

### Comparing `llama_index_readers_clickhouse-0.1.1/llama_index/readers/clickhouse/base.py` & `llama_index_readers_clickhouse-0.1.2/llama_index/readers/clickhouse/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_clickhouse-0.1.1/pyproject.toml` & `llama_index_readers_clickhouse-0.1.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -9,31 +9,29 @@
 
 [tool.llamahub]
 contains_example = false
 import_path = "llama_index.readers.clickhouse"
 
 [tool.llamahub.class_authors]
 ClickHouseReader = "llama-index"
-escape_str = "llama-index"
-format_list_to_string = "llama-index"
 
 [tool.mypy]
 disallow_untyped_defs = true
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
 
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index readers clickhouse integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-readers-clickhouse"
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "0.10.0"
 clickhouse-connect = "^0.7.0"
 
 [tool.poetry.group.dev.dependencies]
```

