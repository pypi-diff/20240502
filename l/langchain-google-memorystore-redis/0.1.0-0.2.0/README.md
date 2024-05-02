# Comparing `tmp/langchain_google_memorystore_redis-0.1.0-py3-none-any.whl.zip` & `tmp/langchain_google_memorystore_redis-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 26561 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1134 b- defN 24-Feb-26 19:57 langchain_google_memorystore_redis/__init__.py
--rw-r--r--  2.0 unx     2505 b- defN 24-Feb-26 19:57 langchain_google_memorystore_redis/chat_message_history.py
--rw-r--r--  2.0 unx     3924 b- defN 24-Feb-26 19:57 langchain_google_memorystore_redis/loader.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Feb-26 19:57 langchain_google_memorystore_redis/py.typed
--rw-r--r--  2.0 unx     5802 b- defN 24-Feb-26 19:57 langchain_google_memorystore_redis/saver.py
--rw-r--r--  2.0 unx    33848 b- defN 24-Feb-26 19:57 langchain_google_memorystore_redis/vectorstore.py
--rw-r--r--  2.0 unx      597 b- defN 24-Feb-26 19:57 langchain_google_memorystore_redis/version.py
--rw-rw-r--  2.0 unx    11358 b- defN 24-Feb-26 19:59 langchain_google_memorystore_redis-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    18549 b- defN 24-Feb-26 19:59 langchain_google_memorystore_redis-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-26 19:59 langchain_google_memorystore_redis-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       35 b- defN 24-Feb-26 19:59 langchain_google_memorystore_redis-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1247 b- defN 24-Feb-26 19:59 langchain_google_memorystore_redis-0.1.0.dist-info/RECORD
-12 files, 79091 bytes uncompressed, 24383 bytes compressed:  69.2%
+Zip file size: 26961 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1134 b- defN 24-May-02 16:33 langchain_google_memorystore_redis/__init__.py
+-rw-r--r--  2.0 unx     2505 b- defN 24-May-02 16:33 langchain_google_memorystore_redis/chat_message_history.py
+-rw-r--r--  2.0 unx     5013 b- defN 24-May-02 16:33 langchain_google_memorystore_redis/loader.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-02 16:33 langchain_google_memorystore_redis/py.typed
+-rw-r--r--  2.0 unx     5802 b- defN 24-May-02 16:33 langchain_google_memorystore_redis/saver.py
+-rw-r--r--  2.0 unx    34387 b- defN 24-May-02 16:33 langchain_google_memorystore_redis/vectorstore.py
+-rw-r--r--  2.0 unx      597 b- defN 24-May-02 16:33 langchain_google_memorystore_redis/version.py
+-rw-rw-r--  2.0 unx    11358 b- defN 24-May-02 16:35 langchain_google_memorystore_redis-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    19671 b- defN 24-May-02 16:35 langchain_google_memorystore_redis-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-02 16:35 langchain_google_memorystore_redis-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       35 b- defN 24-May-02 16:35 langchain_google_memorystore_redis-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1247 b- defN 24-May-02 16:35 langchain_google_memorystore_redis-0.2.0.dist-info/RECORD
+12 files, 81841 bytes uncompressed, 24783 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: langchain_google_memorystore_redis/vectorstore.py
 Comment: 
 
 Filename: langchain_google_memorystore_redis/version.py
 Comment: 
 
-Filename: langchain_google_memorystore_redis-0.1.0.dist-info/LICENSE
+Filename: langchain_google_memorystore_redis-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: langchain_google_memorystore_redis-0.1.0.dist-info/METADATA
+Filename: langchain_google_memorystore_redis-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: langchain_google_memorystore_redis-0.1.0.dist-info/WHEEL
+Filename: langchain_google_memorystore_redis-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: langchain_google_memorystore_redis-0.1.0.dist-info/top_level.txt
+Filename: langchain_google_memorystore_redis-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: langchain_google_memorystore_redis-0.1.0.dist-info/RECORD
+Filename: langchain_google_memorystore_redis-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langchain_google_memorystore_redis/loader.py

```diff
@@ -25,72 +25,103 @@
 
     def __init__(
         self,
         client: redis.Redis,
         key_prefix: str,
         content_fields: Set[str],
         metadata_fields: Optional[Set[str]] = None,
+        batch_size: int = 100,
     ):
         """Initializes the Document Loader for Memorystore for Redis.
 
         Args:
             client: A redis.Redis client object.
             key_prefix: A prefix for the keys to store Documents in Redis.
             content_fields: The set of fields of the hash that Redis uses to
                store the page_content of the Document. If more than one field
                are specified, a JSON encoded dict containing the fields as top
                level keys will be filled in the page_content of the Documents.
             metadata_fields: The metadata fields of the Document that will be
                stored in the Redis. If None, Redis stores all metadata fields.
+            batch_size: Number of keys to load at once from Redis.
         """
 
         self._redis = client
         self._content_fields = content_fields
         self._metadata_fields = metadata_fields
         if metadata_fields and len(content_fields & metadata_fields):
             raise ValueError(
                 "Fields {} are specified in both content_fields and"
                 " metadata_fields.".format(content_fields & metadata_fields)
             )
         self._key_prefix = key_prefix if key_prefix else ""
         self._encoding = client.get_encoder().encoding
+        self._batch_size = batch_size
 
     def lazy_load(self) -> Iterator[Document]:
         """Lazy load the Documents and yield them one by one."""
         for key in self._redis.scan_iter(match=f"{self._key_prefix}*", _type="HASH"):
-            doc = {}
             stored_value = self._redis.hgetall(key)
-            if not isinstance(stored_value, dict):
-                raise RuntimeError(f"{key} returns unexpected {stored_value}")
-            decoded_value = {
-                k.decode(self._encoding): v.decode(self._encoding)
-                for k, v in stored_value.items()
-            }
-
-            if len(self._content_fields) == 1:
-                doc["page_content"] = decoded_value[next(iter(self._content_fields))]
-            else:
-                doc["page_content"] = json.dumps(
-                    {k: decoded_value[k] for k in self._content_fields}
-                )
+            doc = self._construct_document(stored_value)
+            if doc:
+                yield doc
 
-            filtered_fields = (
-                self._metadata_fields if self._metadata_fields else decoded_value.keys()
+    def load(self) -> List[Document]:
+        """Load all Documents using a Redis pipeline for efficiency."""
+        documents = []
+        pipeline = self._redis.pipeline(transaction=False)
+        count = 0
+
+        for key in self._redis.scan_iter(
+            match=f"{self._key_prefix}*", count=self._batch_size
+        ):
+            pipeline.hgetall(key)
+
+            count += 1
+            if count % self._batch_size == 0:
+                # Execute the pipeline and reset for next batch
+                results = pipeline.execute()
+                for stored_value in results:
+                    doc = self._construct_document(stored_value)
+                    documents.append(doc)
+
+        # Execute the pipeline and reset for next batch
+        results = pipeline.execute()
+        for stored_value in results:
+            doc = self._construct_document(stored_value)
+            documents.append(doc)
+
+        return documents
+
+    def _construct_document(self, stored_value) -> Document:
+        """Construct a Document from stored value."""
+        if not isinstance(stored_value, dict):
+            raise ValueError(f"Unexpected stored_value type: {type(stored_value)}")
+        decoded_value = {
+            k.decode(self._encoding): v.decode(self._encoding)
+            for k, v in stored_value.items()
+        }
+
+        doc = {}
+        if len(self._content_fields) == 1:
+            doc["page_content"] = decoded_value[next(iter(self._content_fields))]
+        else:
+            doc["page_content"] = json.dumps(
+                {k: decoded_value[k] for k in self._content_fields}
             )
-            filtered_fields = filtered_fields - self._content_fields
-            doc["metadata"] = {
-                k: self._decode_if_json_parsable(decoded_value[k])
-                for k in filtered_fields
-            }
 
-            yield Document.construct(**doc)
+        filtered_fields = (
+            self._metadata_fields if self._metadata_fields else decoded_value.keys()
+        )
+        filtered_fields = filtered_fields - self._content_fields
+        doc["metadata"] = {
+            k: self._decode_if_json_parsable(decoded_value[k]) for k in filtered_fields
+        }
 
-    def load(self) -> List[Document]:
-        """Load all Documents at once."""
-        return list(self.lazy_load())
+        return Document.construct(**doc)
 
     @staticmethod
     def _decode_if_json_parsable(s: str) -> Union[str, dict]:
         """Decode a JSON string to a dict if it is JSON."""
         try:
             decoded = json.loads(s)
             return decoded
```

## langchain_google_memorystore_redis/vectorstore.py

```diff
@@ -310,28 +310,37 @@
             return False
 
     @staticmethod
     def init_index(client: redis.Redis, index_config: IndexConfig):
         """
         Initializes a named VectorStore index in Redis with specified configurations.
         """
-        if not isinstance(index_config, HNSWConfig):
-            raise ValueError("index_config must be an instance of HNSWConfig")
+        if not isinstance(index_config, VectorIndexConfig):
+            raise ValueError("index_config must be an instance of VectorIndexConfig")
 
         # Preparing the command string to avoid long lines
-        command = (
-            f"FT.CREATE {index_config.name} ON HASH PREFIX 1 {RedisVectorStore.get_key_prefix(index_config.name)} "
-            f"SCHEMA {index_config.field_name} VECTOR {index_config.type} "
-            f"14 TYPE {index_config.data_type} DIM {index_config.vector_size} "
-            f"DISTANCE_METRIC {index_config.distance_metric} "
-            f"TYPE {index_config.data_type} "
-            f"M {index_config.m} "
-            f"EF_CONSTRUCTION {index_config.ef_construction} "
-            f"EF_RUNTIME {index_config.ef_runtime}"
-        )
+        if isinstance(index_config, HNSWConfig):
+            command = (
+                f"FT.CREATE {index_config.name} ON HASH PREFIX 1 {RedisVectorStore.get_key_prefix(index_config.name)} "
+                f"SCHEMA {index_config.field_name} VECTOR {index_config.type} "
+                f"14 TYPE {index_config.data_type} DIM {index_config.vector_size} "
+                f"DISTANCE_METRIC {index_config.distance_metric} "
+                f"TYPE {index_config.data_type} "
+                f"M {index_config.m} "
+                f"EF_CONSTRUCTION {index_config.ef_construction} "
+                f"EF_RUNTIME {index_config.ef_runtime}"
+            )
+        else:
+            command = (
+                f"FT.CREATE {index_config.name} ON HASH PREFIX 1 {RedisVectorStore.get_key_prefix(index_config.name)} "
+                f"SCHEMA {index_config.field_name} VECTOR {index_config.type} "
+                f"8 TYPE {index_config.data_type} DIM {index_config.vector_size} "
+                f"DISTANCE_METRIC {index_config.distance_metric} "
+                f"TYPE {index_config.data_type} "
+            )
 
         try:
             client.execute_command(command)
         except redis.exceptions.ResponseError as e:
             if re.match(r"Redis module key \w+ already exists", str(e)):
                 logger.info("Index already exists, skipping creation.")
             else:
@@ -545,32 +554,34 @@
         """
         Performs a similarity search by a vector with score and embeddings, offering
         various customization options via keyword arguments.
 
         Args:
             query_embedding (List[float]): A list of floats representing the embedding
                 vector of the query for similarity search.
-            k (int, optional): The number of nearest neighbors to retrieve.  Defaults to 4.
+            k (int, optional): The number of nearest neighbors to retrieve. Defaults to 4.
             **kwargs (Any): Additional keyword arguments allowing for customization of
                 the search operation. Key options include:
+
                 - 'distance_threshold' (float, optional): A threshold value for filtering
-                    results based on their distance or score.  If not specified directly,
-                    it may use 'score_threshold' if provided.
+                  results based on their distance or score. If not specified directly,
+                  it may use 'score_threshold' if provided.
+
                 - 'distance_strategy' (str, optional): Strategy to apply when comparing
-                    distances or scores. Uses a default strategy if not specified.
+                  distances or scores. Uses a default strategy if not specified.
 
         Returns:
             List[Tuple[Document, float, List[float]]]: A list of tuples, each containing
             a Document object, its distance (score) from the query embedding, and its own
             embedding vector. The Document object includes content and metadata.
 
         Note:
-            - The function dynamically adjusts its behavior based on the presence and values
-                of keyword arguments. For instance, if a 'distance_threshold' is provided,
-                only results meeting this threshold are returned.
+            The function dynamically adjusts its behavior based on the presence and values
+            of keyword arguments. For instance, if a 'distance_threshold' is provided,
+            only results meeting this threshold are returned.
         """
 
         distance_threshold = kwargs.get(
             "distance_threshold", kwargs.get("score_threshold")
         )
 
         distance_strategy = kwargs.get("distance_strategy", DEFAULT_DISTANCE_STRATEGY)
```

## langchain_google_memorystore_redis/version.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1.0"
+__version__ = "0.2.0"
```

## Comparing `langchain_google_memorystore_redis-0.1.0.dist-info/LICENSE` & `langchain_google_memorystore_redis-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langchain_google_memorystore_redis-0.1.0.dist-info/METADATA` & `langchain_google_memorystore_redis-0.2.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-google-memorystore-redis
-Version: 0.1.0
+Version: 0.2.0
 Summary: LangChain integrations for Google Cloud Memorystore
 Author-email: Google LLC <googleapis-packages@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -206,142 +206,187 @@
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/googleapis/langchain-google-memorystore-redis-python
 Project-URL: Repository, https://github.com/googleapis/langchain-google-memorystore-redis-python.git
 Project-URL: Bug Tracker, https://github.com/googleapis/langchain-google-memorystore-redis-python/issues
 Project-URL: Changelog, https://github.com/googleapis/langchain-google-memorystore-redis-python/blob/main/CHANGELOG.md
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: langchain-core <1.0.0,>=0.1.1
 Requires-Dist: langchain-community <1.0.0,>=0.0.18
 Requires-Dist: redis <6.0.0,>=5.0.0
 Requires-Dist: numpy <2.0.0,>=1.21.0
 Provides-Extra: test
-Requires-Dist: black[jupyter] ==23.12.0 ; extra == 'test'
+Requires-Dist: black[jupyter] ==23.12.1 ; extra == 'test'
 Requires-Dist: isort ==5.13.2 ; extra == 'test'
-Requires-Dist: mypy ==1.7.1 ; extra == 'test'
-Requires-Dist: pytest-asyncio ==0.23.0 ; extra == 'test'
+Requires-Dist: mypy ==1.9.0 ; extra == 'test'
+Requires-Dist: pytest-asyncio ==0.23.5.post1 ; extra == 'test'
 Requires-Dist: pytest ==7.4.4 ; extra == 'test'
 
-# Memorystore for Redis for LangChain
+Memorystore for Redis for LangChain
+===================================
 
-This package contains the [LangChain][langchain] integrations for Memorystore for Redis.
+|preview| |pypi| |versions|
 
-> **🧪 Preview:** This feature is covered by the Pre-GA Offerings Terms of the Google Cloud Terms of Service. Please note that pre-GA products and features might have limited support, and changes to pre-GA products and features might not be compatible with other pre-GA versions. For more information, see the [launch stage descriptions](https://cloud.google.com/products#product-launch-stages)
+- `Client Library Documentation`_
+- `Product Documentation`_
 
-* [Documentation][docs]
-* [API Reference]()
+.. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
+   :target: https://cloud.google.com/products#product-launch-stages
+.. |pypi| image:: https://img.shields.io/pypi/v/langchain-google-memorystore-redis.svg
+   :target: https://pypi.org/project/langchain-google-memorystore-redis/
+.. |versions| image:: https://img.shields.io/pypi/pyversions/langchain-google-memorystore-redis.svg
+   :target: https://pypi.org/project/langchain-google-memorystore-redis/
+.. _Client Library Documentation: https://cloud.google.com/python/docs/reference/langchain-google-memorystore-redis/latest
+.. _Product Documentation: https://cloud.google.com/memorystore
 
-## Getting Started
+Quick Start
+-----------
 
-In order to use this library, you first need to go through the following steps:
+In order to use this library, you first need to go through the following
+steps:
 
-1. [Select or create a Cloud Platform project.][project]
-2. [Enable billing for your project.][billing]
-3. [Enable the Google Cloud Memorystore API.][api]
-4. [Setup Authentication.][auth]
+1. `Select or create a Cloud Platform project.`_
+2. `Enable billing for your project.`_
+3. `Enable the Google Memorystore for Redis API.`_
+4. `Setup Authentication.`_
 
-### Installation
+.. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
+.. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
+.. _Enable the Google Memorystore for Redis API.: https://console.cloud.google.com/flows/enableapi?apiid=memorystore.googleapis.com
+.. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
-Install this library in a [`virtualenv`][venv] using pip. [`virtualenv`][venv] is a tool to
-create isolated Python environments. The basic problem it addresses is one of
-dependencies and versions, and indirectly permissions.
+Installation
+~~~~~~~~~~~~
 
-With [`virtualenv`][venv], it's possible to install this library without needing system
-install permissions, and without clashing with the installed system
-dependencies.
+Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to create isolated Python environments. The basic problem it addresses is
+one of dependencies and versions, and indirectly permissions.
 
-```bash
-pip install virtualenv
-virtualenv <your-env>
-source <your-env>/bin/activate
-<your-env>/bin/pip install langchain-google-memorystore-redis
-```
+With `virtualenv`_, it’s possible to install this library without needing system install permissions, and without clashing with the installed system dependencies.
 
-## Vector Store Usage
+.. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
+
+Supported Python Versions
+^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Python >= 3.8
+
+Mac/Linux
+^^^^^^^^^
+
+.. code-block:: console
+
+   pip install virtualenv
+   virtualenv <your-env>
+   source <your-env>/bin/activate
+   <your-env>/bin/pip install langchain-google-memorystore-redis
+
+Windows
+^^^^^^^
+
+.. code-block:: console
+
+   pip install virtualenv
+   virtualenv <your-env>
+   <your-env>\Scripts\activate
+   <your-env>\Scripts\pip.exe install langchain-google-memorystore-redis
+
+Vector Store Usage
+~~~~~~~~~~~~~~~~~~~
 
 Use a vector store to store embedded data and perform vector search.
 
-```python
-from langchain_google_memorystore_redis import RedisVectorStore
-from langchain_community.embeddings.fake import FakeEmbeddings
+.. code-block:: python
+
+    from langchain_google_memorystore_redis import RedisVectorStore
+
+    redis_client = redis.from_url("redis://127.0.0.1:6379")
+
+    embeddings_service = VertexAIEmbeddings(model_name="textembedding-gecko@003")
+    vectorstore = RedisVectorStore(
+        client=redis_client,
+        index_name="my_vector_index",
+        embeddings=embeddings_service
+    )
 
-embeddings = FakeEmbeddings(size=128)
-redis_client = redis.from_url("redis://127.0.0.1:6379")
+See the full `Vector Store`_ tutorial.
 
-embeddings_service = VertexAIEmbeddings()
-vectorstore = RedisVectorStore(
-    client=redis_client,
-    index_name="my_vector_index",
-    embeddings=embeddings
-)
-```
+.. _`Vector Store`: https://github.com/googleapis/langchain-google-memorystore-redis-python/blob/main/docs/vector_store.ipynb
 
-See the full [Vector Store][vectorstore] tutorial.
+Document Loader Usage
+~~~~~~~~~~~~~~~~~~~~~
 
-## Document Loader Usage
+Use a document loader to load data as LangChain ``Document``\ s.
 
-Use a document loader to load data as LangChain `Document`s.
+.. code-block:: python
 
-```python
-from langchain_google_memorystore_redis import MemorystoreDocumentLoader
+    from langchain_google_memorystore_redis import MemorystoreDocumentLoader
 
 
-loader = MemorystoreDocumentLoader(
-    client=redis_client,
-    key_prefix="docs:",
-    content_fields=set(["page_content"]),
-)
-docs = loader.lazy_load()
-```
+    loader = MemorystoreDocumentLoader(
+        client=redis_client,
+        key_prefix="docs:",
+        content_fields=set(["page_content"]),
+    )
+    docs = loader.lazy_load()
 
-See the full [Document Loader][loader] tutorial.
+See the full `Document Loader`_ tutorial.
 
-## Chat Message History Usage
+.. _`Document Loader`: https://github.com/googleapis/langchain-google-memorystore-redis-python/blob/main/docs/document_loader.ipynb
 
-Use `ChatMessageHistory` to store messages and provide conversation history to LLMs.
+Chat Message History Usage
+--------------------------
 
-```python
-from langchain_google_memorystore_redis import MemorystoreChatMessageHistory
+Use ``ChatMessageHistory`` to store messages and provide conversation
+history to LLMs.
 
+.. code:: python
 
-history = MemorystoreChatMessageHistory(
-    client=redis_client,
-    session_id="my-session_id"
-)
-```
+    from langchain_google_memorystore_redis import MemorystoreChatMessageHistory
 
-See the full [Chat Message History][history] tutorial.
 
-## Contributing
+    history = MemorystoreChatMessageHistory(
+        client=redis_client,
+        session_id="my-session_id"
+    )
+
+See the full `Chat Message History`_ tutorial.
+
+.. _`Chat Message History`: https://github.com/googleapis/langchain-google-memorystore-redis-python/blob/main/docs/chat_message_history.ipynb
+
+Contributions
+~~~~~~~~~~~~~
 
 Contributions to this library are always welcome and highly encouraged.
 
-See [CONTRIBUTING][contributing] for more information how to get started.
+See `CONTRIBUTING`_ for more information how to get started.
 
 Please note that this project is released with a Contributor Code of Conduct. By participating in
-this project you agree to abide by its terms. See [Code of Conduct][coc] for more
+this project you agree to abide by its terms. See `Code of Conduct`_ for more
 information.
 
-## License
+.. _`CONTRIBUTING`: https://github.com/googleapis/langchain-google-memorystore-redis-python/blob/main/CONTRIBUTING.md
+.. _`Code of Conduct`: https://github.com/googleapis/langchain-google-memorystore-redis-python/blob/main/CODE_OF_CONDUCT.md
+
+License
+-------
 
-Apache 2.0 - See [LICENSE][license] for more information.
+Apache 2.0 - See
+`LICENSE <https://github.com/googleapis/langchain-google-memorystore-redis-python/blob/main/LICENSE>`_
+for more information.
 
-## Disclaimer
+Disclaimer
+----------
 
 This is not an officially supported Google product.
 
-[project]: https://console.cloud.google.com/project
-[billing]: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-[api]: https://console.cloud.google.com/flows/enableapi?apiid=memorystore.googleapis.com
-[auth]: https://googleapis.dev/python/google-api-core/latest/auth.html
-[venv]: https://virtualenv.pypa.io/en/latest/
-[vectorstore]: https://github.com/googleapis/langchain-google-memorystore-redis-python/tree/main/docs/vector_store.ipynb
-[loader]: https://github.com/googleapis/langchain-google-memorystore-redis-python/tree/main/docs/document_loader.ipynb
-[history]: https://github.com/googleapis/langchain-google-memorystore-redis-python/tree/main/docs/chat_message_history.ipynb
-[langchain]: https://github.com/langchain-ai/langchain
-[docs]: https://github.com/googleapis/langchain-google-memorystore-redis-python/tree/main/docs
-[license]: https://github.com/googleapis/langchain-google-memorystore-redis-python/tree/main/LICENSE
-[contributing]: https://github.com/googleapis/langchain-google-memorystore-redis-python/tree/main/CONTRIBUTING.md
-[coc]: https://github.com/googleapis/langchain-google-memorystore-redis-python/tree/main/CODE_OF_CONDUCT.md
```

