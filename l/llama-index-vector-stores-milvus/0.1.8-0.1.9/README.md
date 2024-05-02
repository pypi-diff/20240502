# Comparing `tmp/llama_index_vector_stores_milvus-0.1.8.tar.gz` & `tmp/llama_index_vector_stores_milvus-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_milvus-0.1.8.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_milvus-0.1.9.tar", max compression
```

## Comparing `llama_index_vector_stores_milvus-0.1.8.tar` & `llama_index_vector_stores_milvus-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       47 2024-04-09 17:47:09.199711 llama_index_vector_stores_milvus-0.1.8/README.md
--rw-r--r--   0        0        0      101 2024-04-09 17:47:09.199711 llama_index_vector_stores_milvus-0.1.8/llama_index/vector_stores/milvus/__init__.py
--rw-r--r--   0        0        0    13964 2024-04-09 17:47:09.199711 llama_index_vector_stores_milvus-0.1.8/llama_index/vector_stores/milvus/base.py
--rw-r--r--   0        0        0     1479 2024-04-09 17:47:09.199711 llama_index_vector_stores_milvus-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 llama_index_vector_stores_milvus-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       47 2024-04-10 16:31:31.339675 llama_index_vector_stores_milvus-0.1.9/README.md
+-rw-r--r--   0        0        0      101 2024-04-10 16:31:31.339675 llama_index_vector_stores_milvus-0.1.9/llama_index/vector_stores/milvus/__init__.py
+-rw-r--r--   0        0        0    14059 2024-04-10 16:31:31.339675 llama_index_vector_stores_milvus-0.1.9/llama_index/vector_stores/milvus/base.py
+-rw-r--r--   0        0        0     1479 2024-04-10 16:31:31.339675 llama_index_vector_stores_milvus-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 llama_index_vector_stores_milvus-0.1.9/PKG-INFO
```

### Comparing `llama_index_vector_stores_milvus-0.1.8/llama_index/vector_stores/milvus/base.py` & `llama_index_vector_stores_milvus-0.1.9/llama_index/vector_stores/milvus/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
             collection_name=collection_name,
             dim=dim,
             embedding_field=embedding_field,
             doc_id_field=doc_id_field,
             consistency_level=consistency_level,
             overwrite=overwrite,
             text_key=text_key,
-            output_fields=output_fields,
+            output_fields=output_fields or [],
             index_config=index_config if index_config else {},
             search_config=search_config if search_config else {},
         )
 
         # Select the similarity metric
         similarity_metrics_map = {
             "ip": "IP",
@@ -293,14 +293,16 @@
         if query.node_ids is not None and len(query.node_ids) != 0:
             expr_list = ['"' + entry + '"' for entry in query.node_ids]
             expr.append(f"{MILVUS_ID_FIELD} in [{','.join(expr_list)}]")
 
         # Limit output fields
         if query.output_fields is not None:
             output_fields = query.output_fields
+        elif len(self.output_fields) > 0:
+            output_fields = self.output_fields
 
         # Convert to string expression
         string_expr = ""
         if len(expr) != 0:
             string_expr = f" {query.filters.condition.value} ".join(expr)
 
         # Perform the search
```

### Comparing `llama_index_vector_stores_milvus-0.1.8/pyproject.toml` & `llama_index_vector_stores_milvus-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores milvus integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-milvus"
 readme = "README.md"
-version = "0.1.8"
+version = "0.1.9"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 pymilvus = "^2.3.6"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_vector_stores_milvus-0.1.8/PKG-INFO` & `llama_index_vector_stores_milvus-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-milvus
-Version: 0.1.8
+Version: 0.1.9
 Summary: llama-index vector_stores milvus integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

