# Comparing `tmp/vanna-0.5.0.tar.gz` & `tmp/vanna-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vanna-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "vanna-0.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vanna-0.5.0.tar` & `vanna-0.5.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     7922 2024-04-30 21:36:15.036170 vanna-0.5.0/README.md
--rw-r--r--   0        0        0     1614 2024-04-30 21:36:15.048169 vanna-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     8725 2024-04-30 21:36:15.048169 vanna-0.5.0/src/vanna/ZhipuAI/ZhipuAI_Chat.py
--rw-r--r--   0        0        0     2849 2024-04-30 21:36:15.048169 vanna-0.5.0/src/vanna/ZhipuAI/ZhipuAI_embeddings.py
--rw-r--r--   0        0        0      116 2024-04-30 21:36:15.048169 vanna-0.5.0/src/vanna/ZhipuAI/__init__.py
--rw-r--r--   0        0        0     9248 2024-04-30 21:36:15.048169 vanna-0.5.0/src/vanna/__init__.py
--rw-r--r--   0        0        0       43 2024-04-30 21:36:15.048169 vanna-0.5.0/src/vanna/anthropic/__init__.py
--rw-r--r--   0        0        0     2615 2024-04-30 21:36:15.048169 vanna-0.5.0/src/vanna/anthropic/anthropic_chat.py
--rw-r--r--   0        0        0       28 2024-04-30 21:36:15.048169 vanna-0.5.0/src/vanna/base/__init__.py
--rw-r--r--   0        0        0    62126 2024-04-30 21:36:15.048169 vanna-0.5.0/src/vanna/base/base.py
--rw-r--r--   0        0        0       50 2024-04-30 21:36:15.048169 vanna-0.5.0/src/vanna/chromadb/__init__.py
--rw-r--r--   0        0        0     8792 2024-04-30 21:36:15.048169 vanna-0.5.0/src/vanna/chromadb/chromadb_vector.py
--rw-r--r--   0        0        0      685 2024-04-30 21:36:15.048169 vanna-0.5.0/src/vanna/exceptions/__init__.py
--rw-r--r--   0        0        0    25192 2024-04-30 21:36:15.048169 vanna-0.5.0/src/vanna/flask/__init__.py
--rw-r--r--   0        0        0   187711 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/flask/assets.py
--rw-r--r--   0        0        0     1246 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/flask/auth.py
--rw-r--r--   0        0        0       41 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/google/__init__.py
--rw-r--r--   0        0        0     1584 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/google/gemini_chat.py
--rw-r--r--   0        0        0       19 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/hf/__init__.py
--rw-r--r--   0        0        0     2703 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/hf/hf.py
--rw-r--r--   0        0        0      313 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/local.py
--rw-r--r--   0        0        0       37 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/marqo/__init__.py
--rw-r--r--   0        0        0     5242 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/marqo/marqo.py
--rw-r--r--   0        0        0       29 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/mistral/__init__.py
--rw-r--r--   0        0        0     1508 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/mistral/mistral.py
--rw-r--r--   0        0        0       27 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/ollama/__init__.py
--rw-r--r--   0        0        0     3790 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/ollama/ollama.py
--rw-r--r--   0        0        0       86 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/openai/__init__.py
--rw-r--r--   0        0        0     4764 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/openai/openai_chat.py
--rw-r--r--   0        0        0     1260 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/openai/openai_embeddings.py
--rw-r--r--   0        0        0       54 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/opensearch/__init__.py
--rw-r--r--   0        0        0     9129 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/opensearch/opensearch_vector.py
--rw-r--r--   0        0        0       73 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/qdrant/__init__.py
--rw-r--r--   0        0        0    11940 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/qdrant/qdrant.py
--rw-r--r--   0        0        0     1856 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/remote.py
--rw-r--r--   0        0        0     4957 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/types/__init__.py
--rw-r--r--   0        0        0     2247 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/utils.py
--rw-r--r--   0        0        0       48 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/vannadb/__init__.py
--rw-r--r--   0        0        0     6168 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/vannadb/vannadb_vector.py
--rw-r--r--   0        0        0       23 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/vllm/__init__.py
--rw-r--r--   0        0        0     2427 2024-04-30 21:36:15.052169 vanna-0.5.0/src/vanna/vllm/vllm.py
--rw-r--r--   0        0        0    11115 1970-01-01 00:00:00.000000 vanna-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     8010 2024-05-02 13:17:19.261679 vanna-0.5.1/README.md
+-rw-r--r--   0        0        0     1627 2024-05-02 13:17:19.277679 vanna-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     8725 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/ZhipuAI/ZhipuAI_Chat.py
+-rw-r--r--   0        0        0     2849 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/ZhipuAI/ZhipuAI_embeddings.py
+-rw-r--r--   0        0        0      116 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/ZhipuAI/__init__.py
+-rw-r--r--   0        0        0     9248 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/__init__.py
+-rw-r--r--   0        0        0       43 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/anthropic/__init__.py
+-rw-r--r--   0        0        0     2615 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/anthropic/anthropic_chat.py
+-rw-r--r--   0        0        0       28 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/base/__init__.py
+-rw-r--r--   0        0        0    62126 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/base/base.py
+-rw-r--r--   0        0        0       50 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/chromadb/__init__.py
+-rw-r--r--   0        0        0     8792 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/chromadb/chromadb_vector.py
+-rw-r--r--   0        0        0      685 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/exceptions/__init__.py
+-rw-r--r--   0        0        0    25192 2024-05-02 13:17:19.277679 vanna-0.5.1/src/vanna/flask/__init__.py
+-rw-r--r--   0        0        0   187711 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/flask/assets.py
+-rw-r--r--   0        0        0     1246 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/flask/auth.py
+-rw-r--r--   0        0        0       41 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/google/__init__.py
+-rw-r--r--   0        0        0     1584 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/google/gemini_chat.py
+-rw-r--r--   0        0        0       19 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/hf/__init__.py
+-rw-r--r--   0        0        0     2703 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/hf/hf.py
+-rw-r--r--   0        0        0      313 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/local.py
+-rw-r--r--   0        0        0       37 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/marqo/__init__.py
+-rw-r--r--   0        0        0     5242 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/marqo/marqo.py
+-rw-r--r--   0        0        0       29 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/mistral/__init__.py
+-rw-r--r--   0        0        0     1508 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/mistral/mistral.py
+-rw-r--r--   0        0        0       27 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/ollama/__init__.py
+-rw-r--r--   0        0        0     3790 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/ollama/ollama.py
+-rw-r--r--   0        0        0       86 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/openai/__init__.py
+-rw-r--r--   0        0        0     4764 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/openai/openai_chat.py
+-rw-r--r--   0        0        0     1260 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/openai/openai_embeddings.py
+-rw-r--r--   0        0        0       54 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/opensearch/__init__.py
+-rw-r--r--   0        0        0     9129 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/opensearch/opensearch_vector.py
+-rw-r--r--   0        0        0       73 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/qdrant/__init__.py
+-rw-r--r--   0        0        0    11883 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/qdrant/qdrant.py
+-rw-r--r--   0        0        0     1856 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/remote.py
+-rw-r--r--   0        0        0     4957 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/types/__init__.py
+-rw-r--r--   0        0        0     2247 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/utils.py
+-rw-r--r--   0        0        0       48 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/vannadb/__init__.py
+-rw-r--r--   0        0        0     6168 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/vannadb/vannadb_vector.py
+-rw-r--r--   0        0        0       23 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/vllm/__init__.py
+-rw-r--r--   0        0        0     2427 2024-05-02 13:17:19.281679 vanna-0.5.1/src/vanna/vllm/vllm.py
+-rw-r--r--   0        0        0    11248 1970-01-01 00:00:00.000000 vanna-0.5.1/PKG-INFO
```

### Comparing `vanna-0.5.0/README.md` & `vanna-0.5.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 1. **Train a RAG "model" on your data**.
 2. **Ask questions**.
 
 ![](img/vanna-readme-diagram.png)
 
 If you don't know what RAG is, don't worry -- you don't need to know how this works under the hood to use it. You just need to know that you "train" a model, which stores some metadata and then use it to "ask" questions.
 
-See the [base class](src/vanna/base/base.py) for more details on how this works under the hood.
+See the [base class](https://github.com/vanna-ai/vanna/blob/main/src/vanna/base/base.py) for more details on how this works under the hood.
 
 ## User Interfaces
 These are some of the user interfaces that we've built using Vanna. You can use these as-is or as a starting point for your own custom interface.
 
 - [Jupyter Notebook](https://vanna.ai/docs/postgres-openai-vanna-vannadb/)
 - [vanna-ai/vanna-streamlit](https://github.com/vanna-ai/vanna-streamlit)
 - [vanna-ai/vanna-flask](https://github.com/vanna-ai/vanna-flask)
@@ -214,15 +214,15 @@
 4. **Supports any SQL database.**
     - The package allows you to connect to any SQL database that you can otherwise connect to with Python
 5. **Choose your front end.**
     - Most people start in a Jupyter Notebook.
     - Expose to your end users via Slackbot, web app, Streamlit app, or a custom front end.
 
 ## Extending Vanna
-Vanna is designed to connect to any database, LLM, and vector database. There's a [VannaBase](src/vanna/base/base.py) abstract base class that defines some basic functionality. The package provides implementations for use with OpenAI and ChromaDB. You can easily extend Vanna to use your own LLM or vector database. See the [documentation](https://vanna.ai/docs/) for more details.
+Vanna is designed to connect to any database, LLM, and vector database. There's a [VannaBase](https://github.com/vanna-ai/vanna/blob/main/src/vanna/base/base.py) abstract base class that defines some basic functionality. The package provides implementations for use with OpenAI and ChromaDB. You can easily extend Vanna to use your own LLM or vector database. See the [documentation](https://vanna.ai/docs/) for more details.
 
 ## Vanna in 100 Seconds
 
 https://github.com/vanna-ai/vanna/assets/7146154/eb90ee1e-aa05-4740-891a-4fc10e611cab
 
 ## More resources
  - [Full Documentation](https://vanna.ai/docs/)
```

### Comparing `vanna-0.5.0/pyproject.toml` & `vanna-0.5.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "vanna"
-version = "0.5.0"
+version = "0.5.1"
 authors = [
   { name="Zain Hoda", email="zain@vanna.ai" },
 ]
 
 description = "Generate SQL queries from natural language"
 readme = "README.md"
 requires-python = ">=3.9"
@@ -38,11 +38,11 @@
 openai = ["openai"]
 mistralai = ["mistralai"]
 anthropic = ["anthropic"]
 gemini = ["google-generativeai"]
 marqo = ["marqo"]
 zhipuai = ["zhipuai"]
 ollama = ["ollama", "httpx"]
-qdrant = ["qdrant-client"]
+qdrant = ["qdrant-client", "fastembed"]
 vllm = ["vllm"]
 opensearch = ["opensearch-py", "opensearch-dsl"]
 hf = ["transformers"]
```

### Comparing `vanna-0.5.0/src/vanna/ZhipuAI/ZhipuAI_Chat.py` & `vanna-0.5.1/src/vanna/ZhipuAI/ZhipuAI_Chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/ZhipuAI/ZhipuAI_embeddings.py` & `vanna-0.5.1/src/vanna/ZhipuAI/ZhipuAI_embeddings.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/__init__.py` & `vanna-0.5.1/src/vanna/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/anthropic/anthropic_chat.py` & `vanna-0.5.1/src/vanna/anthropic/anthropic_chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/base/base.py` & `vanna-0.5.1/src/vanna/base/base.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/chromadb/chromadb_vector.py` & `vanna-0.5.1/src/vanna/chromadb/chromadb_vector.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/exceptions/__init__.py` & `vanna-0.5.1/src/vanna/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/flask/__init__.py` & `vanna-0.5.1/src/vanna/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/flask/assets.py` & `vanna-0.5.1/src/vanna/flask/assets.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/flask/auth.py` & `vanna-0.5.1/src/vanna/flask/auth.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/google/gemini_chat.py` & `vanna-0.5.1/src/vanna/google/gemini_chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/hf/hf.py` & `vanna-0.5.1/src/vanna/hf/hf.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/marqo/marqo.py` & `vanna-0.5.1/src/vanna/marqo/marqo.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/mistral/mistral.py` & `vanna-0.5.1/src/vanna/mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/ollama/ollama.py` & `vanna-0.5.1/src/vanna/ollama/ollama.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/openai/openai_chat.py` & `vanna-0.5.1/src/vanna/openai/openai_chat.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/openai/openai_embeddings.py` & `vanna-0.5.1/src/vanna/openai/openai_embeddings.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/opensearch/opensearch_vector.py` & `vanna-0.5.1/src/vanna/opensearch/opensearch_vector.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/qdrant/qdrant.py` & `vanna-0.5.1/src/vanna/qdrant/qdrant.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         self.fastembed_model = config.get("fastembed_model", "BAAI/bge-small-en-v1.5")
         self.collection_params = config.get("collection_params", {})
         self.distance_metric = config.get("distance_metric", models.Distance.COSINE)
 
         self._setup_collections()
 
     def add_question_sql(self, question: str, sql: str, **kwargs) -> str:
-        question_answer = format("Question: {0}\n\nSQL: {1}", question, sql)
+        question_answer = "Question: {0}\n\nSQL: {1}".format(question, sql)
         id = deterministic_uuid(question_answer)
 
         self._client.upsert(
             SQL_COLLECTION_NAME,
             points=[
                 models.PointStruct(
                     id=id,
@@ -153,31 +153,29 @@
             df_sql["training_data_type"] = "sql"
 
             df = pd.concat([df, df_sql])
 
         if ddl_data := self._get_all_points(DDL_COLLECTION_NAME):
             ddl_list = [data.payload["ddl"] for data in ddl_data]
             id_list = [
-                self._format_point_id(data.id, DDL_COLLECTION_NAME) for data in sql_data
+                self._format_point_id(data.id, DDL_COLLECTION_NAME) for data in ddl_data
             ]
 
             df_ddl = pd.DataFrame(
                 {
                     "id": id_list,
                     "question": [None for _ in ddl_list],
                     "content": ddl_list,
                 }
             )
 
             df_ddl["training_data_type"] = "ddl"
 
             df = pd.concat([df, df_ddl])
 
-        doc_data = self.documentation_collection.get()
-
         if doc_data := self._get_all_points(DOCUMENTATION_COLLECTION_NAME):
             document_list = [data.payload["documentation"] for data in doc_data]
             id_list = [
                 self._format_point_id(data.id, DOCUMENTATION_COLLECTION_NAME)
                 for data in doc_data
             ]
```

### Comparing `vanna-0.5.0/src/vanna/remote.py` & `vanna-0.5.1/src/vanna/remote.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/types/__init__.py` & `vanna-0.5.1/src/vanna/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/utils.py` & `vanna-0.5.1/src/vanna/utils.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/vannadb/vannadb_vector.py` & `vanna-0.5.1/src/vanna/vannadb/vannadb_vector.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/src/vanna/vllm/vllm.py` & `vanna-0.5.1/src/vanna/vllm/vllm.py`

 * *Files identical despite different names*

### Comparing `vanna-0.5.0/PKG-INFO` & `vanna-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vanna
-Version: 0.5.0
+Version: 0.5.1
 Summary: Generate SQL queries from natural language
 Author-email: Zain Hoda <zain@vanna.ai>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -53,14 +53,15 @@
 Requires-Dist: httpx ; extra == "ollama"
 Requires-Dist: openai ; extra == "openai"
 Requires-Dist: opensearch-py ; extra == "opensearch"
 Requires-Dist: opensearch-dsl ; extra == "opensearch"
 Requires-Dist: psycopg2-binary ; extra == "postgres"
 Requires-Dist: db-dtypes ; extra == "postgres"
 Requires-Dist: qdrant-client ; extra == "qdrant"
+Requires-Dist: fastembed ; extra == "qdrant"
 Requires-Dist: snowflake-connector-python ; extra == "snowflake"
 Requires-Dist: tox ; extra == "test"
 Requires-Dist: vllm ; extra == "vllm"
 Requires-Dist: zhipuai ; extra == "zhipuai"
 Project-URL: Bug Tracker, https://github.com/vanna-ai/vanna/issues
 Project-URL: Homepage, https://github.com/vanna-ai/vanna
 Provides-Extra: all
@@ -107,15 +108,15 @@
 1. **Train a RAG "model" on your data**.
 2. **Ask questions**.
 
 ![](img/vanna-readme-diagram.png)
 
 If you don't know what RAG is, don't worry -- you don't need to know how this works under the hood to use it. You just need to know that you "train" a model, which stores some metadata and then use it to "ask" questions.
 
-See the [base class](src/vanna/base/base.py) for more details on how this works under the hood.
+See the [base class](https://github.com/vanna-ai/vanna/blob/main/src/vanna/base/base.py) for more details on how this works under the hood.
 
 ## User Interfaces
 These are some of the user interfaces that we've built using Vanna. You can use these as-is or as a starting point for your own custom interface.
 
 - [Jupyter Notebook](https://vanna.ai/docs/postgres-openai-vanna-vannadb/)
 - [vanna-ai/vanna-streamlit](https://github.com/vanna-ai/vanna-streamlit)
 - [vanna-ai/vanna-flask](https://github.com/vanna-ai/vanna-flask)
@@ -300,15 +301,15 @@
 4. **Supports any SQL database.**
     - The package allows you to connect to any SQL database that you can otherwise connect to with Python
 5. **Choose your front end.**
     - Most people start in a Jupyter Notebook.
     - Expose to your end users via Slackbot, web app, Streamlit app, or a custom front end.
 
 ## Extending Vanna
-Vanna is designed to connect to any database, LLM, and vector database. There's a [VannaBase](src/vanna/base/base.py) abstract base class that defines some basic functionality. The package provides implementations for use with OpenAI and ChromaDB. You can easily extend Vanna to use your own LLM or vector database. See the [documentation](https://vanna.ai/docs/) for more details.
+Vanna is designed to connect to any database, LLM, and vector database. There's a [VannaBase](https://github.com/vanna-ai/vanna/blob/main/src/vanna/base/base.py) abstract base class that defines some basic functionality. The package provides implementations for use with OpenAI and ChromaDB. You can easily extend Vanna to use your own LLM or vector database. See the [documentation](https://vanna.ai/docs/) for more details.
 
 ## Vanna in 100 Seconds
 
 https://github.com/vanna-ai/vanna/assets/7146154/eb90ee1e-aa05-4740-891a-4fc10e611cab
 
 ## More resources
  - [Full Documentation](https://vanna.ai/docs/)
```

