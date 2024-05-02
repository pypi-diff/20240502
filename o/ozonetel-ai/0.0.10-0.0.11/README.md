# Comparing `tmp/ozonetel-ai-0.0.10.tar.gz` & `tmp/ozonetel-ai-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ozonetel-ai-0.0.10.tar", last modified: Wed Apr 24 07:26:41 2024, max compression
+gzip compressed data, was "ozonetel-ai-0.0.11.tar", last modified: Thu May  2 12:02:02 2024, max compression
```

## Comparing `ozonetel-ai-0.0.10.tar` & `ozonetel-ai-0.0.11.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:26:41.867862 ozonetel-ai-0.0.10/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-24 07:25:03.000000 ozonetel-ai-0.0.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-24 07:26:41.867862 ozonetel-ai-0.0.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-04-24 07:25:03.000000 ozonetel-ai-0.0.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:26:41.867862 ozonetel-ai-0.0.10/ozoneai/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-24 07:25:03.000000 ozonetel-ai-0.0.10/ozoneai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-24 07:25:03.000000 ozonetel-ai-0.0.10/ozoneai/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8002 2024-04-24 07:25:03.000000 ozonetel-ai-0.0.10/ozoneai/embeder.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-24 07:25:03.000000 ozonetel-ai-0.0.10/ozoneai/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-24 07:25:03.000000 ozonetel-ai-0.0.10/ozoneai/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 07:26:41.867862 ozonetel-ai-0.0.10/ozonetel_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-04-24 07:26:41.000000 ozonetel-ai-0.0.10/ozonetel_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-24 07:26:41.000000 ozonetel-ai-0.0.10/ozonetel_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 07:26:41.000000 ozonetel-ai-0.0.10/ozonetel_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-24 07:26:41.000000 ozonetel-ai-0.0.10/ozonetel_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-24 07:26:41.000000 ozonetel-ai-0.0.10/ozonetel_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 07:26:41.867862 ozonetel-ai-0.0.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-24 07:25:03.000000 ozonetel-ai-0.0.10/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:02:02.608670 ozonetel-ai-0.0.11/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-02 12:00:22.000000 ozonetel-ai-0.0.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-02 12:02:02.608670 ozonetel-ai-0.0.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-02 12:00:22.000000 ozonetel-ai-0.0.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:02:02.604670 ozonetel-ai-0.0.11/ozoneai/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-02 12:00:22.000000 ozonetel-ai-0.0.11/ozoneai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-02 12:00:22.000000 ozonetel-ai-0.0.11/ozoneai/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-05-02 12:00:22.000000 ozonetel-ai-0.0.11/ozoneai/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-02 12:00:22.000000 ozonetel-ai-0.0.11/ozoneai/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-02 12:00:22.000000 ozonetel-ai-0.0.11/ozoneai/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:02:02.608670 ozonetel-ai-0.0.11/ozonetel_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-02 12:02:02.000000 ozonetel-ai-0.0.11/ozonetel_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-02 12:02:02.000000 ozonetel-ai-0.0.11/ozonetel_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:02:02.000000 ozonetel-ai-0.0.11/ozonetel_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 12:02:02.000000 ozonetel-ai-0.0.11/ozonetel_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-02 12:02:02.000000 ozonetel-ai-0.0.11/ozonetel_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 12:02:02.608670 ozonetel-ai-0.0.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-02 12:00:22.000000 ozonetel-ai-0.0.11/setup.py
```

### Comparing `ozonetel-ai-0.0.10/LICENSE` & `ozonetel-ai-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.10/PKG-INFO` & `ozonetel-ai-0.0.11/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ozonetel-ai
-Version: 0.0.10
+Version: 0.0.11
 Summary: The Ozonetel AI Library is a powerful tool developed by Ozonetel Communications Pvt Ltd, designed to empower developers with state-of-the-art Artificial Intelligence capabilities. This library provides seamless integration of advanced AI models into your projects, allowing you to leverage the latest in AI technology to enhance your applications.
 Home-page: 
 Author: Biswajit Satapathy
 Author-email: biswajit@ozonetel.com
 License: MIT License
 Keywords: Machine Learning,Artificial Intellegence,Neural Network,Indexing,Searching
 Classifier: Programming Language :: Python :: 3.8
@@ -14,15 +14,15 @@
 License-File: LICENSE
 
 # Ozonetel AI
 ## Overview
 The Ozonetel AI project is designed to provide a user-friendly interface for software development using Ozonetel's in-house AI libraries, models, and software solutions. It offers seamless integration with Ozonetel's advanced AI capabilities, allowing developers to harness the power of AI to enhance their applications.
 
 ## Features
-- Text Embedding (Bit Embeddings): The Ozonetel AI project currently offers text embedding functionality, allowing users to convert text into high-dimensional bit vectors for various natural language processing tasks.
+- Text Embedding (Binary Embeddings): The Ozonetel AI project currently offers text embedding functionality, allowing users to convert text into high-dimensional bit vectors for various natural language processing tasks.
 
 ## Getting Started
 To get started with the Ozonetel AI project, follow the steps below:
 
 1. Set Credentials:
     Before using the text embedding feature, set your credentials by importing the os module and setting the `OZAI_API_CREDENTIALS` environment variable to point to your credentials file.
     
@@ -33,34 +33,44 @@
     os.environ["OZAI_API_CREDENTIALS"] = "./cred.json"
     ```
 3. Text Embedding Extraction
     Text embedding converts textual data into numerical representations, aiding natural language processing tasks. By capturing semantic meaning, it enhances sentiment analysis, document classification, and named entity recognition. Efficient and transferable, embeddings facilitate faster computation and enable machine learning models to better understand and process text. `QuantizeSentenceEmbedding` quantizes base embeddings and represents in bits.
 
    Example:
     ```python
-    # Import `QuantizeSentenceEmbedding` class from the `ozoneai.embeder` module.
-    from ozoneai.embeder import QuantizeSentenceEmbedding
+    # Import `QuantizeSentenceEmbedding` class from the `ozoneai.embeddings` module.
+    from ozoneai.embeddings import QuantizeSentenceEmbedding
     
     # Extract Embeddings: Use the `quantize` method to obtain quantised embeddings for given texts .
+    # Supported models encoders are `sentence-transformers/paraphrase-multilingual-mpnet-base-v2` and `BAAI/bge-m3`
+    # Alternatively if you have stored these models in local directory you can use like `/path/to/paraphrase-multilingual-mpnet-base-v2` or `/path/to/bge-m3`
     with QuantizeSentenceEmbedding(
-        endcoder_modelid="sentence-transformers/paraphrase-multilingual-mpnet-base-v2") as embeder:
-
-        emb = embeder.encode(["Try me Out"])
-        emb_quantised = embeder.quantize(emb, model="siv-sentence-bitnet-pmbv2-wikid-large") # max limit 20 vectors per request
+        endcoder_modelid="BAAI/bge-m3") as embedder:
+        emb = embedder.encode(["Try me Out"])
+        emb_quantised = embedder.quantize(emb, model="sieve-bge-m3-en-aug-v1") # max limit 20 vectors per request
     
     # Access Embedding Attributes: Retrieve various attributes of the embedding object, such as bits, unsigned binary, and signed binary.
     
     # Get bit representation
     embedding_bits = emb_quantised.bits
     
     # Get unsigned binary
     embedding_ubin = emb_quantised.ubinary()
     
     # Get signed binary
     embedding_bin = emb_quantised.binary()
     ```
 
+    If you want to check available embeddings you can do it as follows
+    ```python
+    from ozoneai.embeddings import list_models
+
+    list_models()
+    ```
+
+## Examples
 
+- [search and index](https://github.com/ozonetelgit/ozonetel-ai-sdk/blob/7d693eb3f012b62ec2bcda6758cc5a4e4d18fae7/examples/search-index/Text%20Indexing%20using%20OzoneAI%20Embeddings%20Faiss.ipynb)
 
 ## License
 The Ozonetel AI project is licensed under the MIT License. Please refer to the LICENSE file for more information.
```

### Comparing `ozonetel-ai-0.0.10/README.md` & `ozonetel-ai-0.0.11/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Ozonetel AI
 ## Overview
 The Ozonetel AI project is designed to provide a user-friendly interface for software development using Ozonetel's in-house AI libraries, models, and software solutions. It offers seamless integration with Ozonetel's advanced AI capabilities, allowing developers to harness the power of AI to enhance their applications.
 
 ## Features
-- Text Embedding (Bit Embeddings): The Ozonetel AI project currently offers text embedding functionality, allowing users to convert text into high-dimensional bit vectors for various natural language processing tasks.
+- Text Embedding (Binary Embeddings): The Ozonetel AI project currently offers text embedding functionality, allowing users to convert text into high-dimensional bit vectors for various natural language processing tasks.
 
 ## Getting Started
 To get started with the Ozonetel AI project, follow the steps below:
 
 1. Set Credentials:
     Before using the text embedding feature, set your credentials by importing the os module and setting the `OZAI_API_CREDENTIALS` environment variable to point to your credentials file.
     
@@ -18,34 +18,44 @@
     os.environ["OZAI_API_CREDENTIALS"] = "./cred.json"
     ```
 3. Text Embedding Extraction
     Text embedding converts textual data into numerical representations, aiding natural language processing tasks. By capturing semantic meaning, it enhances sentiment analysis, document classification, and named entity recognition. Efficient and transferable, embeddings facilitate faster computation and enable machine learning models to better understand and process text. `QuantizeSentenceEmbedding` quantizes base embeddings and represents in bits.
 
    Example:
     ```python
-    # Import `QuantizeSentenceEmbedding` class from the `ozoneai.embeder` module.
-    from ozoneai.embeder import QuantizeSentenceEmbedding
+    # Import `QuantizeSentenceEmbedding` class from the `ozoneai.embeddings` module.
+    from ozoneai.embeddings import QuantizeSentenceEmbedding
     
     # Extract Embeddings: Use the `quantize` method to obtain quantised embeddings for given texts .
+    # Supported models encoders are `sentence-transformers/paraphrase-multilingual-mpnet-base-v2` and `BAAI/bge-m3`
+    # Alternatively if you have stored these models in local directory you can use like `/path/to/paraphrase-multilingual-mpnet-base-v2` or `/path/to/bge-m3`
     with QuantizeSentenceEmbedding(
-        endcoder_modelid="sentence-transformers/paraphrase-multilingual-mpnet-base-v2") as embeder:
-
-        emb = embeder.encode(["Try me Out"])
-        emb_quantised = embeder.quantize(emb, model="siv-sentence-bitnet-pmbv2-wikid-large") # max limit 20 vectors per request
+        endcoder_modelid="BAAI/bge-m3") as embedder:
+        emb = embedder.encode(["Try me Out"])
+        emb_quantised = embedder.quantize(emb, model="sieve-bge-m3-en-aug-v1") # max limit 20 vectors per request
     
     # Access Embedding Attributes: Retrieve various attributes of the embedding object, such as bits, unsigned binary, and signed binary.
     
     # Get bit representation
     embedding_bits = emb_quantised.bits
     
     # Get unsigned binary
     embedding_ubin = emb_quantised.ubinary()
     
     # Get signed binary
     embedding_bin = emb_quantised.binary()
     ```
 
+    If you want to check available embeddings you can do it as follows
+    ```python
+    from ozoneai.embeddings import list_models
+
+    list_models()
+    ```
+
+## Examples
 
+- [search and index](https://github.com/ozonetelgit/ozonetel-ai-sdk/blob/7d693eb3f012b62ec2bcda6758cc5a4e4d18fae7/examples/search-index/Text%20Indexing%20using%20OzoneAI%20Embeddings%20Faiss.ipynb)
 
 ## License
 The Ozonetel AI project is licensed under the MIT License. Please refer to the LICENSE file for more information.
```

### Comparing `ozonetel-ai-0.0.10/ozoneai/connector.py` & `ozonetel-ai-0.0.11/ozoneai/connector.py`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.10/ozoneai/embeder.py` & `ozonetel-ai-0.0.11/ozoneai/embeddings.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 from typing import List
 
 from .connector import EmbeddingConnector
 from .models import EmbeddingModels
 from .exception import LimitError
 from sentence_transformers import SentenceTransformer
 
+
+def list_models():
+    for endcoder_modelid, modelids in EmbeddingModels.encoders_model_map.items():
+        print(f"""endcoder_modelid: {endcoder_modelid}, model(s):""")
+        for modelid in modelids:
+            print(f"""\t{modelid}""")
+        print("\n")
+
 class Embeddings(object):
     def __init__(self, model) -> None:
         self.name = model
         
     def parse(self, response):
         if not "is_error" in response:
             raise AssertionError("API Error!")
@@ -113,15 +121,15 @@
         )
         embeddings = Embeddings(model)
         r = response.json()
         return embeddings.parse(r)
     
 class QuantizeEmbedding(object):
     """Ozone Embedder Client Application"""
-    def __init__(self, endcoder_modelid:str = "paraphrase-multilingual-mpnet-base-v2") -> None:
+    def __init__(self, endcoder_modelid:str = "sieve-bge-m3-en-aug-v1") -> None:
         super(QuantizeEmbedding, self).__init__()
         self.connector = EmbeddingConnector()
         self.models = EmbeddingModels.models
         self.allowed_encoders = EmbeddingModels.encoders
         self.encoder_name = os.path.basename(endcoder_modelid.rstrip("/"))
         
         if not self.encoder_name in self.allowed_encoders:
@@ -177,14 +185,15 @@
 class QuantizeSentenceEmbedding(object):
     """Ozone Embedder Client Application"""
     def __init__(self, endcoder_modelid:str ="", device:str ="cpu") -> None:
         super(QuantizeSentenceEmbedding, self).__init__()
         self.connector = EmbeddingConnector()
         self.models = EmbeddingModels.models
         self.allowed_encoders = EmbeddingModels.encoders
+        self.model_maps = EmbeddingModels
         
         self.encoder_name = os.path.basename(endcoder_modelid.rstrip("/"))
         
         if not self.encoder_name in self.allowed_encoders:
             raise NotImplementedError(f"""Encoder provided is not supported! choose one of {self.allowed_encoders} .""")
         
         self.embedder = SentenceTransformer(endcoder_modelid, device=device)
@@ -220,16 +229,16 @@
         return self.embedder.encode(texts, batch_size=batch_size, show_progress_bar=verbose)
         
     def quantize(self, embedding: np.ndarray, model:str):
         f"""
         embedding: text embeddings [ no_of_tokens * embeddings_dim ]
         model: {"or, ".join(self.models)}
         """
-        if not model in self.models:
-            raise ValueError("invalid model input!\nselect one from {self.models}")
+        if not model in self.model_maps.encoders_model_map[self.encoder_name]:
+            raise ValueError(f"invalid model input!\n {model} is not type of {self.encoder_name}")
         
         if len(embedding.shape) == 1:
             embedding = np.array([embedding])
             
         if embedding.shape[0] > 20:
             raise LimitError("max limit (20) exceeded!")
```

### Comparing `ozonetel-ai-0.0.10/ozoneai/exception.py` & `ozonetel-ai-0.0.11/ozoneai/exception.py`

 * *Files identical despite different names*

### Comparing `ozonetel-ai-0.0.10/ozonetel_ai.egg-info/PKG-INFO` & `ozonetel-ai-0.0.11/ozonetel_ai.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ozonetel-ai
-Version: 0.0.10
+Version: 0.0.11
 Summary: The Ozonetel AI Library is a powerful tool developed by Ozonetel Communications Pvt Ltd, designed to empower developers with state-of-the-art Artificial Intelligence capabilities. This library provides seamless integration of advanced AI models into your projects, allowing you to leverage the latest in AI technology to enhance your applications.
 Home-page: 
 Author: Biswajit Satapathy
 Author-email: biswajit@ozonetel.com
 License: MIT License
 Keywords: Machine Learning,Artificial Intellegence,Neural Network,Indexing,Searching
 Classifier: Programming Language :: Python :: 3.8
@@ -14,15 +14,15 @@
 License-File: LICENSE
 
 # Ozonetel AI
 ## Overview
 The Ozonetel AI project is designed to provide a user-friendly interface for software development using Ozonetel's in-house AI libraries, models, and software solutions. It offers seamless integration with Ozonetel's advanced AI capabilities, allowing developers to harness the power of AI to enhance their applications.
 
 ## Features
-- Text Embedding (Bit Embeddings): The Ozonetel AI project currently offers text embedding functionality, allowing users to convert text into high-dimensional bit vectors for various natural language processing tasks.
+- Text Embedding (Binary Embeddings): The Ozonetel AI project currently offers text embedding functionality, allowing users to convert text into high-dimensional bit vectors for various natural language processing tasks.
 
 ## Getting Started
 To get started with the Ozonetel AI project, follow the steps below:
 
 1. Set Credentials:
     Before using the text embedding feature, set your credentials by importing the os module and setting the `OZAI_API_CREDENTIALS` environment variable to point to your credentials file.
     
@@ -33,34 +33,44 @@
     os.environ["OZAI_API_CREDENTIALS"] = "./cred.json"
     ```
 3. Text Embedding Extraction
     Text embedding converts textual data into numerical representations, aiding natural language processing tasks. By capturing semantic meaning, it enhances sentiment analysis, document classification, and named entity recognition. Efficient and transferable, embeddings facilitate faster computation and enable machine learning models to better understand and process text. `QuantizeSentenceEmbedding` quantizes base embeddings and represents in bits.
 
    Example:
     ```python
-    # Import `QuantizeSentenceEmbedding` class from the `ozoneai.embeder` module.
-    from ozoneai.embeder import QuantizeSentenceEmbedding
+    # Import `QuantizeSentenceEmbedding` class from the `ozoneai.embeddings` module.
+    from ozoneai.embeddings import QuantizeSentenceEmbedding
     
     # Extract Embeddings: Use the `quantize` method to obtain quantised embeddings for given texts .
+    # Supported models encoders are `sentence-transformers/paraphrase-multilingual-mpnet-base-v2` and `BAAI/bge-m3`
+    # Alternatively if you have stored these models in local directory you can use like `/path/to/paraphrase-multilingual-mpnet-base-v2` or `/path/to/bge-m3`
     with QuantizeSentenceEmbedding(
-        endcoder_modelid="sentence-transformers/paraphrase-multilingual-mpnet-base-v2") as embeder:
-
-        emb = embeder.encode(["Try me Out"])
-        emb_quantised = embeder.quantize(emb, model="siv-sentence-bitnet-pmbv2-wikid-large") # max limit 20 vectors per request
+        endcoder_modelid="BAAI/bge-m3") as embedder:
+        emb = embedder.encode(["Try me Out"])
+        emb_quantised = embedder.quantize(emb, model="sieve-bge-m3-en-aug-v1") # max limit 20 vectors per request
     
     # Access Embedding Attributes: Retrieve various attributes of the embedding object, such as bits, unsigned binary, and signed binary.
     
     # Get bit representation
     embedding_bits = emb_quantised.bits
     
     # Get unsigned binary
     embedding_ubin = emb_quantised.ubinary()
     
     # Get signed binary
     embedding_bin = emb_quantised.binary()
     ```
 
+    If you want to check available embeddings you can do it as follows
+    ```python
+    from ozoneai.embeddings import list_models
+
+    list_models()
+    ```
+
+## Examples
 
+- [search and index](https://github.com/ozonetelgit/ozonetel-ai-sdk/blob/7d693eb3f012b62ec2bcda6758cc5a4e4d18fae7/examples/search-index/Text%20Indexing%20using%20OzoneAI%20Embeddings%20Faiss.ipynb)
 
 ## License
 The Ozonetel AI project is licensed under the MIT License. Please refer to the LICENSE file for more information.
```

### Comparing `ozonetel-ai-0.0.10/setup.py` & `ozonetel-ai-0.0.11/setup.py`

 * *Files identical despite different names*

