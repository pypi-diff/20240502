# Comparing `tmp/llama_index_readers_dashvector-0.1.2.tar.gz` & `tmp/llama_index_readers_dashvector-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_dashvector-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_readers_dashvector-0.1.3.tar", max compression
```

## Comparing `llama_index_readers_dashvector-0.1.2.tar` & `llama_index_readers_dashvector-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       45 2024-02-13 13:53:01.752677 llama_index_readers_dashvector-0.1.2/README.md
--rw-r--r--   0        0        0       97 2024-02-13 13:53:01.752908 llama_index_readers_dashvector-0.1.2/llama_index/readers/dashvector/__init__.py
--rw-r--r--   0        0        0     2842 2024-02-13 13:53:01.752973 llama_index_readers_dashvector-0.1.2/llama_index/readers/dashvector/base.py
--rw-r--r--   0        0        0     1474 2024-02-21 19:41:36.230176 llama_index_readers_dashvector-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      700 1970-01-01 00:00:00.000000 llama_index_readers_dashvector-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1404 2024-05-02 17:02:31.949773 llama_index_readers_dashvector-0.1.3/README.md
+-rw-r--r--   0        0        0       97 2024-05-02 17:02:31.953773 llama_index_readers_dashvector-0.1.3/llama_index/readers/dashvector/__init__.py
+-rw-r--r--   0        0        0     2842 2024-05-02 17:02:31.953773 llama_index_readers_dashvector-0.1.3/llama_index/readers/dashvector/base.py
+-rw-r--r--   0        0        0     1474 2024-05-02 17:02:31.953773 llama_index_readers_dashvector-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2008 1970-01-01 00:00:00.000000 llama_index_readers_dashvector-0.1.3/PKG-INFO
```

### Comparing `llama_index_readers_dashvector-0.1.2/llama_index/readers/dashvector/base.py` & `llama_index_readers_dashvector-0.1.3/llama_index/readers/dashvector/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_dashvector-0.1.2/pyproject.toml` & `llama_index_readers_dashvector-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index readers dashvector integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-readers-dashvector"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 dashvector = "^1.0.9"
 
 [tool.poetry.group.dev.dependencies]
```

