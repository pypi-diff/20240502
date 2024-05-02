# Comparing `tmp/llama_index_readers_database-0.1.3.tar.gz` & `tmp/llama_index_readers_database-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_database-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_readers_database-0.1.4.tar", max compression
```

## Comparing `llama_index_readers_database-0.1.3.tar` & `llama_index_readers_database-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       43 2024-02-13 13:53:01.753655 llama_index_readers_database-0.1.3/README.md
--rw-r--r--   0        0        0       91 2024-02-13 13:53:01.753846 llama_index_readers_database-0.1.3/llama_index/readers/database/__init__.py
--rw-r--r--   0        0        0     3376 2024-02-13 13:53:01.753923 llama_index_readers_database-0.1.3/llama_index/readers/database/base.py
--rw-r--r--   0        0        0     1521 2024-02-21 19:42:29.063325 llama_index_readers_database-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 llama_index_readers_database-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1247 2024-05-02 17:02:31.953773 llama_index_readers_database-0.1.4/README.md
+-rw-r--r--   0        0        0       91 2024-05-02 17:02:31.953773 llama_index_readers_database-0.1.4/llama_index/readers/database/__init__.py
+-rw-r--r--   0        0        0     3376 2024-05-02 17:02:31.953773 llama_index_readers_database-0.1.4/llama_index/readers/database/base.py
+-rw-r--r--   0        0        0     1521 2024-05-02 17:02:31.953773 llama_index_readers_database-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 llama_index_readers_database-0.1.4/PKG-INFO
```

### Comparing `llama_index_readers_database-0.1.3/llama_index/readers/database/base.py` & `llama_index_readers_database-0.1.4/llama_index/readers/database/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_database-0.1.3/pyproject.toml` & `llama_index_readers_database-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 description = "llama-index readers database integration"
 exclude = ["**/BUILD"]
 keywords = ["aws rds", "postgres", "snowflake", "sql"]
 license = "MIT"
 maintainers = ["kevinqz"]
 name = "llama-index-readers-database"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

