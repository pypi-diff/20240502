# Comparing `tmp/llama_index_readers_chroma-0.1.3.tar.gz` & `tmp/llama_index_readers_chroma-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_chroma-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_readers_chroma-0.1.4.tar", max compression
```

## Comparing `llama_index_readers_chroma-0.1.3.tar` & `llama_index_readers_chroma-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       41 2024-02-13 13:53:01.746894 llama_index_readers_chroma-0.1.3/README.md
--rw-r--r--   0        0        0       85 2024-02-13 13:53:01.747076 llama_index_readers_chroma-0.1.3/llama_index/readers/chroma/__init__.py
--rw-r--r--   0        0        0     3844 2024-02-13 13:53:01.747130 llama_index_readers_chroma-0.1.3/llama_index/readers/chroma/base.py
--rw-r--r--   0        0        0     1477 2024-02-21 19:35:57.446203 llama_index_readers_chroma-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 llama_index_readers_chroma-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1648 2024-05-02 17:02:31.949773 llama_index_readers_chroma-0.1.4/README.md
+-rw-r--r--   0        0        0       85 2024-05-02 17:02:31.949773 llama_index_readers_chroma-0.1.4/llama_index/readers/chroma/__init__.py
+-rw-r--r--   0        0        0     3844 2024-05-02 17:02:31.949773 llama_index_readers_chroma-0.1.4/llama_index/readers/chroma/base.py
+-rw-r--r--   0        0        0     1477 2024-05-02 17:02:31.949773 llama_index_readers_chroma-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2262 1970-01-01 00:00:00.000000 llama_index_readers_chroma-0.1.4/PKG-INFO
```

### Comparing `llama_index_readers_chroma-0.1.3/llama_index/readers/chroma/base.py` & `llama_index_readers_chroma-0.1.4/llama_index/readers/chroma/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_chroma-0.1.3/pyproject.toml` & `llama_index_readers_chroma-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 authors = ["Your Name <you@example.com>"]
 description = "llama-index readers chroma integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 maintainers = ["atroyn"]
 name = "llama-index-readers-chroma"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 chromadb = "^0.4.22"
 
 [tool.poetry.group.dev.dependencies]
```

