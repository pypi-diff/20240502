# Comparing `tmp/llama_index_readers_faiss-0.1.3.tar.gz` & `tmp/llama_index_readers_faiss-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_faiss-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_readers_faiss-0.1.4.tar", max compression
```

## Comparing `llama_index_readers_faiss-0.1.3.tar` & `llama_index_readers_faiss-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       40 2024-02-13 13:53:01.763973 llama_index_readers_faiss-0.1.3/README.md
--rw-r--r--   0        0        0       82 2024-02-13 13:53:01.764161 llama_index_readers_faiss-0.1.3/llama_index/readers/faiss/__init__.py
--rw-r--r--   0        0        0     2501 2024-02-13 13:53:01.764217 llama_index_readers_faiss-0.1.3/llama_index/readers/faiss/base.py
--rw-r--r--   0        0        0     1458 2024-02-21 19:48:36.376636 llama_index_readers_faiss-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      664 1970-01-01 00:00:00.000000 llama_index_readers_faiss-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1113 2024-05-02 17:02:31.961773 llama_index_readers_faiss-0.1.4/README.md
+-rw-r--r--   0        0        0       82 2024-05-02 17:02:31.961773 llama_index_readers_faiss-0.1.4/llama_index/readers/faiss/__init__.py
+-rw-r--r--   0        0        0     2501 2024-05-02 17:02:31.961773 llama_index_readers_faiss-0.1.4/llama_index/readers/faiss/base.py
+-rw-r--r--   0        0        0     1458 2024-05-02 17:02:31.961773 llama_index_readers_faiss-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1686 1970-01-01 00:00:00.000000 llama_index_readers_faiss-0.1.4/PKG-INFO
```

### Comparing `llama_index_readers_faiss-0.1.3/llama_index/readers/faiss/base.py` & `llama_index_readers_faiss-0.1.4/llama_index/readers/faiss/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_faiss-0.1.3/pyproject.toml` & `llama_index_readers_faiss-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 authors = ["Your Name <you@example.com>"]
 description = "llama-index readers faiss integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 maintainers = ["jerryjliu"]
 name = "llama-index-readers-faiss"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

