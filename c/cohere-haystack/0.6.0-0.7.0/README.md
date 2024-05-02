# Comparing `tmp/cohere_haystack-0.6.0.tar.gz` & `tmp/cohere_haystack-0.7.0.tar.gz`

## Comparing `cohere_haystack-0.6.0.tar` & `cohere_haystack-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/examples/cohere_ranker_in_a_pipeline.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/pydoc/config.yml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/src/haystack_integrations/components/embedders/cohere/__init__.py
--rw-r--r--   0        0        0     8356 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/src/haystack_integrations/components/embedders/cohere/document_embedder.py
--rw-r--r--   0        0        0     5992 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/src/haystack_integrations/components/embedders/cohere/text_embedder.py
--rw-r--r--   0        0        0     3132 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/src/haystack_integrations/components/embedders/cohere/utils.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/src/haystack_integrations/components/generators/cohere/__init__.py
--rw-r--r--   0        0        0     8194 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/src/haystack_integrations/components/generators/cohere/generator.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/src/haystack_integrations/components/generators/cohere/chat/__init__.py
--rw-r--r--   0        0        0     9893 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/src/haystack_integrations/components/generators/cohere/chat/chat_generator.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/src/haystack_integrations/components/rankers/cohere/__init__.py
--rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/src/haystack_integrations/components/rankers/cohere/ranker.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0    15176 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/tests/test_cohere_chat_generator.py
--rw-r--r--   0        0        0     7859 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/tests/test_cohere_generators.py
--rw-r--r--   0        0        0    15455 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/tests/test_cohere_ranker.py
--rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/tests/test_document_embedder.py
--rw-r--r--   0        0        0     4810 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/tests/test_text_embedder.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/README.md
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 cohere_haystack-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/examples/cohere_ranker_in_a_pipeline.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/pydoc/config.yml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/src/haystack_integrations/components/embedders/cohere/__init__.py
+-rw-r--r--   0        0        0     8352 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/src/haystack_integrations/components/embedders/cohere/document_embedder.py
+-rw-r--r--   0        0        0     5988 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/src/haystack_integrations/components/embedders/cohere/text_embedder.py
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/src/haystack_integrations/components/embedders/cohere/utils.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/src/haystack_integrations/components/generators/cohere/__init__.py
+-rw-r--r--   0        0        0     8202 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/src/haystack_integrations/components/generators/cohere/generator.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/src/haystack_integrations/components/generators/cohere/chat/__init__.py
+-rw-r--r--   0        0        0    10087 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/src/haystack_integrations/components/generators/cohere/chat/chat_generator.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/src/haystack_integrations/components/rankers/cohere/__init__.py
+-rw-r--r--   0        0        0     6673 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/src/haystack_integrations/components/rankers/cohere/ranker.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0    15915 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/tests/test_cohere_chat_generator.py
+-rw-r--r--   0        0        0     7867 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/tests/test_cohere_generators.py
+-rw-r--r--   0        0        0    15463 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/tests/test_cohere_ranker.py
+-rw-r--r--   0        0        0     5861 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/tests/test_document_embedder.py
+-rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/tests/test_text_embedder.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/README.md
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 cohere_haystack-0.7.0/PKG-INFO
```

### Comparing `cohere_haystack-0.6.0/examples/cohere_ranker_in_a_pipeline.py` & `cohere_haystack-0.7.0/examples/cohere_ranker_in_a_pipeline.py`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.6.0/pydoc/config.yml` & `cohere_haystack-0.7.0/pydoc/config.yml`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.6.0/src/haystack_integrations/components/embedders/cohere/document_embedder.py` & `cohere_haystack-0.7.0/src/haystack_integrations/components/embedders/cohere/document_embedder.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import asyncio
 from typing import Any, Dict, List, Optional
 
 from haystack import Document, component, default_from_dict, default_to_dict
 from haystack.utils import Secret, deserialize_secrets_inplace
 from haystack_integrations.components.embedders.cohere.utils import get_async_response, get_response
 
-from cohere import COHERE_API_URL, AsyncClient, Client
+from cohere import AsyncClient, Client
 
 
 @component
 class CohereDocumentEmbedder:
     """
     A component for computing Document embeddings using Cohere models.
 
@@ -35,15 +35,15 @@
     """
 
     def __init__(
         self,
         api_key: Secret = Secret.from_env_var(["COHERE_API_KEY", "CO_API_KEY"]),
         model: str = "embed-english-v2.0",
         input_type: str = "search_document",
-        api_base_url: str = COHERE_API_URL,
+        api_base_url: str = "https://api.cohere.com",
         truncate: str = "END",
         use_async_client: bool = False,
         max_retries: int = 3,
         timeout: int = 120,
         batch_size: int = 32,
         progress_bar: bool = True,
         meta_fields_to_embed: Optional[List[str]] = None,
@@ -165,26 +165,26 @@
 
         api_key = self.api_key.resolve_value()
         assert api_key is not None
 
         if self.use_async_client:
             cohere_client = AsyncClient(
                 api_key,
-                api_url=self.api_base_url,
+                base_url=self.api_base_url,
                 max_retries=self.max_retries,
                 timeout=self.timeout,
                 client_name="haystack",
             )
             all_embeddings, metadata = asyncio.run(
                 get_async_response(cohere_client, texts_to_embed, self.model, self.input_type, self.truncate)
             )
         else:
             cohere_client = Client(
                 api_key,
-                api_url=self.api_base_url,
+                base_url=self.api_base_url,
                 max_retries=self.max_retries,
                 timeout=self.timeout,
                 client_name="haystack",
             )
             all_embeddings, metadata = get_response(
                 cohere_client,
                 texts_to_embed,
```

### Comparing `cohere_haystack-0.6.0/src/haystack_integrations/components/embedders/cohere/text_embedder.py` & `cohere_haystack-0.7.0/src/haystack_integrations/components/embedders/cohere/text_embedder.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import asyncio
 from typing import Any, Dict, List
 
 from haystack import component, default_from_dict, default_to_dict
 from haystack.utils import Secret, deserialize_secrets_inplace
 from haystack_integrations.components.embedders.cohere.utils import get_async_response, get_response
 
-from cohere import COHERE_API_URL, AsyncClient, Client
+from cohere import AsyncClient, Client
 
 
 @component
 class CohereTextEmbedder:
     """
     A component for embedding strings using Cohere models.
 
@@ -32,15 +32,15 @@
     """
 
     def __init__(
         self,
         api_key: Secret = Secret.from_env_var(["COHERE_API_KEY", "CO_API_KEY"]),
         model: str = "embed-english-v2.0",
         input_type: str = "search_query",
-        api_base_url: str = COHERE_API_URL,
+        api_base_url: str = "https://api.cohere.com",
         truncate: str = "END",
         use_async_client: bool = False,
         max_retries: int = 3,
         timeout: int = 120,
     ):
         """
         :param api_key: the Cohere API key.
@@ -127,26 +127,26 @@
 
         api_key = self.api_key.resolve_value()
         assert api_key is not None
 
         if self.use_async_client:
             cohere_client = AsyncClient(
                 api_key,
-                api_url=self.api_base_url,
+                base_url=self.api_base_url,
                 max_retries=self.max_retries,
                 timeout=self.timeout,
                 client_name="haystack",
             )
             embedding, metadata = asyncio.run(
                 get_async_response(cohere_client, [text], self.model, self.input_type, self.truncate)
             )
         else:
             cohere_client = Client(
                 api_key,
-                api_url=self.api_base_url,
+                base_url=self.api_base_url,
                 max_retries=self.max_retries,
                 timeout=self.timeout,
                 client_name="haystack",
             )
             embedding, metadata = get_response(cohere_client, [text], self.model, self.input_type, self.truncate)
 
         return {"embedding": embedding[0], "meta": metadata}
```

### Comparing `cohere_haystack-0.6.0/src/haystack_integrations/components/embedders/cohere/utils.py` & `cohere_haystack-0.7.0/src/haystack_integrations/components/embedders/cohere/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-FileCopyrightText: 2023-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
 from typing import Any, Dict, List, Tuple
 
 from tqdm import tqdm
 
-from cohere import AsyncClient, Client, CohereError
+from cohere import AsyncClient, Client
 
 
 async def get_async_response(cohere_async_client: AsyncClient, texts: List[str], model_name, input_type, truncate):
     """Embeds a list of texts asynchronously using the Cohere API.
 
     :param cohere_async_client: the Cohere `AsyncClient`
     :param texts: the texts to embed
@@ -20,28 +20,22 @@
 
     :returns: A tuple of the embeddings and metadata.
 
     :raises ValueError: If an error occurs while querying the Cohere API.
     """
     all_embeddings: List[List[float]] = []
     metadata: Dict[str, Any] = {}
-    try:
-        response = await cohere_async_client.embed(
-            texts=texts, model=model_name, input_type=input_type, truncate=truncate
-        )
-        if response.meta is not None:
-            metadata = response.meta
-        for emb in response.embeddings:
-            all_embeddings.append(emb)
 
-        return all_embeddings, metadata
+    response = await cohere_async_client.embed(texts=texts, model=model_name, input_type=input_type, truncate=truncate)
+    if response.meta is not None:
+        metadata = response.meta
+    for emb in response.embeddings:
+        all_embeddings.append(emb)
 
-    except CohereError as error_response:
-        msg = error_response.message
-        raise ValueError(msg) from error_response
+    return all_embeddings, metadata
 
 
 def get_response(
     cohere_client: Client, texts: List[str], model_name, input_type, truncate, batch_size=32, progress_bar=False
 ) -> Tuple[List[List[float]], Dict[str, Any]]:
     """Embeds a list of texts using the Cohere API.
 
@@ -58,25 +52,20 @@
 
     :raises ValueError: If an error occurs while querying the Cohere API.
     """
 
     all_embeddings: List[List[float]] = []
     metadata: Dict[str, Any] = {}
 
-    try:
-        for i in tqdm(
-            range(0, len(texts), batch_size),
-            disable=not progress_bar,
-            desc="Calculating embeddings",
-        ):
-            batch = texts[i : i + batch_size]
-            response = cohere_client.embed(batch, model=model_name, input_type=input_type, truncate=truncate)
-            for emb in response.embeddings:
-                all_embeddings.append(emb)
-            if response.meta is not None:
-                metadata = response.meta
-
-        return all_embeddings, metadata
-
-    except CohereError as error_response:
-        msg = error_response.message
-        raise ValueError(msg) from error_response
+    for i in tqdm(
+        range(0, len(texts), batch_size),
+        disable=not progress_bar,
+        desc="Calculating embeddings",
+    ):
+        batch = texts[i : i + batch_size]
+        response = cohere_client.embed(batch, model=model_name, input_type=input_type, truncate=truncate)
+        for emb in response.embeddings:
+            all_embeddings.append(emb)
+        if response.meta is not None:
+            metadata = response.meta
+
+    return all_embeddings, metadata
```

### Comparing `cohere_haystack-0.6.0/src/haystack_integrations/components/generators/cohere/generator.py` & `cohere_haystack-0.7.0/src/haystack_integrations/components/generators/cohere/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from typing import Any, Callable, Dict, List, Optional, cast
 
 from haystack import component, default_from_dict, default_to_dict
 from haystack.components.generators.utils import deserialize_callback_handler, serialize_callback_handler
 from haystack.dataclasses import StreamingChunk
 from haystack.utils import Secret, deserialize_secrets_inplace
 
-from cohere import COHERE_API_URL, Client
-from cohere.responses import Generations
+from cohere import Client, Generation
 
 logger = logging.getLogger(__name__)
 
 
 @component
 class CohereGenerator:
     """LLM Generator compatible with Cohere's generate endpoint.
@@ -73,22 +72,22 @@
                 equally to all tokens that have already appeared, regardless of their exact frequencies.
             - 'return_likelihoods': One of GENERATION|ALL|NONE to specify how and if the token likelihoods are returned
                 with the response. Defaults to NONE.
             - 'logit_bias': Used to prevent the model from generating unwanted tokens or to incentivize it to include
                 desired tokens. The format is {token_id: bias} where bias is a float between -10 and 10.
         """
         if not api_base_url:
-            api_base_url = COHERE_API_URL
+            api_base_url = "https://api.cohere.com"
 
         self.api_key = api_key
         self.model = model
         self.streaming_callback = streaming_callback
         self.api_base_url = api_base_url
         self.model_parameters = kwargs
-        self.client = Client(api_key=self.api_key.resolve_value(), api_url=self.api_base_url, client_name="haystack")
+        self.client = Client(api_key=self.api_key.resolve_value(), base_url=self.api_base_url, client_name="haystack")
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
         :returns:
             Dictionary with serialized data.
@@ -126,29 +125,28 @@
         Queries the LLM with the prompts to produce replies.
 
         :param prompt: the prompt to be sent to the generative model.
         :returns: A dictionary with the following keys:
             - `replies`: the list of replies generated by the model.
             - `meta`: metadata about the request.
         """
-        response = self.client.generate(
-            model=self.model, prompt=prompt, stream=self.streaming_callback is not None, **self.model_parameters
-        )
         if self.streaming_callback:
+            response = self.client.generate_stream(model=self.model, prompt=prompt, **self.model_parameters)
             metadata_dict: Dict[str, Any] = {}
             for chunk in response:
                 stream_chunk = self._build_chunk(chunk)
                 self.streaming_callback(stream_chunk)
             replies = response.texts
             metadata_dict["finish_reason"] = response.finish_reason
             metadata = [metadata_dict]
             self._check_truncated_answers(metadata)
             return {"replies": replies, "meta": metadata}
 
-        metadata = [{"finish_reason": resp.finish_reason} for resp in cast(Generations, response)]
+        response = self.client.generate(model=self.model, prompt=prompt, **self.model_parameters)
+        metadata = [{"finish_reason": resp.finish_reason} for resp in cast(Generation, response)]
         replies = [resp.text for resp in response]
         self._check_truncated_answers(metadata)
         return {"replies": replies, "meta": metadata}
 
     def _build_chunk(self, chunk) -> StreamingChunk:
         """
         Converts the response from the Cohere API to a StreamingChunk.
```

### Comparing `cohere_haystack-0.6.0/src/haystack_integrations/components/generators/cohere/chat/chat_generator.py` & `cohere_haystack-0.7.0/src/haystack_integrations/components/generators/cohere/chat/chat_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,25 +78,25 @@
                 "accurate" results or "fast" results.
             - 'temperature': A non-negative float that tunes the degree of randomness in generation. Lower temperatures
                 mean less random generations.
         """
         cohere_import.check()
 
         if not api_base_url:
-            api_base_url = cohere.COHERE_API_URL
+            api_base_url = "https://api.cohere.com"
         if generation_kwargs is None:
             generation_kwargs = {}
         self.api_key = api_key
         self.model = model
         self.streaming_callback = streaming_callback
         self.api_base_url = api_base_url
         self.generation_kwargs = generation_kwargs
         self.model_parameters = kwargs
         self.client = cohere.Client(
-            api_key=self.api_key.resolve_value(), api_url=self.api_base_url, client_name="haystack"
+            api_key=self.api_key.resolve_value(), base_url=self.api_base_url, client_name="haystack"
         )
 
     def _get_telemetry_data(self) -> Dict[str, Any]:
         """
         Data that is sent to Posthog for usage analytics.
         """
         return {"model": self.model}
@@ -152,22 +152,21 @@
             Cohere [documentation](https://docs.cohere.com/reference/chat).
         :returns: A dictionary with the following keys:
             - `replies`: a list of `ChatMessage` instances representing the generated responses.
         """
         # update generation kwargs by merging with the generation kwargs passed to the run method
         generation_kwargs = {**self.generation_kwargs, **(generation_kwargs or {})}
         chat_history = [self._message_to_dict(m) for m in messages[:-1]]
-        response = self.client.chat(
-            message=messages[-1].content,
-            model=self.model,
-            stream=self.streaming_callback is not None,
-            chat_history=chat_history,
-            **generation_kwargs,
-        )
         if self.streaming_callback:
+            response = self.client.chat_stream(
+                message=messages[-1].content,
+                model=self.model,
+                chat_history=chat_history,
+                **generation_kwargs,
+            )
             for chunk in response:
                 if chunk.event_type == "text-generation":
                     stream_chunk = self._build_chunk(chunk)
                     self.streaming_callback(stream_chunk)
             chat_message = ChatMessage.from_assistant(content=response.texts)
             chat_message.meta.update(
                 {
@@ -176,14 +175,20 @@
                     "index": 0,
                     "finish_reason": response.finish_reason,
                     "documents": response.documents,
                     "citations": response.citations,
                 }
             )
         else:
+            response = self.client.chat(
+                message=messages[-1].content,
+                model=self.model,
+                chat_history=chat_history,
+                **generation_kwargs,
+            )
             chat_message = self._build_message(response)
         return {"replies": [chat_message]}
 
     def _build_chunk(self, chunk) -> StreamingChunk:
         """
         Converts the response from the Cohere API to a StreamingChunk.
         :param chunk: The chunk returned by the OpenAI API.
```

### Comparing `cohere_haystack-0.6.0/src/haystack_integrations/components/rankers/cohere/ranker.py` & `cohere_haystack-0.7.0/src/haystack_integrations/components/rankers/cohere/ranker.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     """
 
     def __init__(
         self,
         model: str = "rerank-english-v2.0",
         top_k: int = 10,
         api_key: Secret = Secret.from_env_var(["COHERE_API_KEY", "CO_API_KEY"]),
-        api_base_url: str = cohere.COHERE_API_URL,
+        api_base_url: str = "https://api.cohere.com",
         max_chunks_per_doc: Optional[int] = None,
         meta_fields_to_embed: Optional[List[str]] = None,
         meta_data_separator: str = "\n",
     ):
         """
         Creates an instance of the 'CohereRanker'.
 
@@ -62,15 +62,15 @@
         self.api_key = api_key
         self.api_base_url = api_base_url
         self.top_k = top_k
         self.max_chunks_per_doc = max_chunks_per_doc
         self.meta_fields_to_embed = meta_fields_to_embed or []
         self.meta_data_separator = meta_data_separator
         self._cohere_client = cohere.Client(
-            api_key=self.api_key.resolve_value(), api_url=self.api_base_url, client_name="haystack"
+            api_key=self.api_key.resolve_value(), base_url=self.api_base_url, client_name="haystack"
         )
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
         :returns:
```

### Comparing `cohere_haystack-0.6.0/tests/test_cohere_chat_generator.py` & `cohere_haystack-0.7.0/tests/test_cohere_chat_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 pytestmark = pytest.mark.chat_generators
 
 
 @pytest.fixture
 def mock_chat_response():
     """
-    Mock the CohereI API response and reuse it for tests
+    Mock the Cohere API response and reuse it for tests
     """
     with patch("cohere.Client.chat", autospec=True) as mock_chat_response:
         # mimic the response from the Cohere API
 
         mock_response = Mock()
         mock_response.text = "I'm fine, thanks."
         mock_response.token_count = {
@@ -31,14 +31,35 @@
             "api_version": {"version": "1"},
             "billed_units": {"input_tokens": 55, "output_tokens": 78},
         }
         mock_chat_response.return_value = mock_response
         yield mock_chat_response
 
 
+@pytest.fixture
+def mock_chat_streaming_response():
+    with patch("cohere.Client.chat_stream", autospec=True) as mock_chat_stream_response:
+        # mimic the response from the Cohere API
+
+        mock_response = Mock()
+        mock_response.text = "I'm fine, thanks."
+        mock_response.token_count = {
+            "prompt_tokens": 66,
+            "response_tokens": 78,
+            "total_tokens": 144,
+            "billed_tokens": 133,
+        }
+        mock_response.meta = {
+            "api_version": {"version": "1"},
+            "billed_units": {"input_tokens": 55, "output_tokens": 78},
+        }
+        mock_chat_stream_response.return_value = mock_response
+        yield mock_chat_stream_response
+
+
 def streaming_chunk(text: str):
     """
     Mock chunks of streaming responses from the Cohere API
     """
     # mimic the chunk response from the OpenAI API
     mock_chunks = Mock()
     mock_chunks.index = 0
@@ -56,15 +77,15 @@
     def test_init_default(self, monkeypatch):
         monkeypatch.setenv("COHERE_API_KEY", "test-api-key")
 
         component = CohereChatGenerator()
         assert component.api_key == Secret.from_env_var(["COHERE_API_KEY", "CO_API_KEY"])
         assert component.model == "command"
         assert component.streaming_callback is None
-        assert component.api_base_url == cohere.COHERE_API_URL
+        assert component.api_base_url == "https://api.cohere.com"
         assert not component.generation_kwargs
 
     def test_init_fail_wo_api_key(self, monkeypatch):
         monkeypatch.delenv("COHERE_API_KEY", raising=False)
         monkeypatch.delenv("CO_API_KEY", raising=False)
         with pytest.raises(ValueError):
             CohereChatGenerator()
@@ -89,15 +110,15 @@
         data = component.to_dict()
         assert data == {
             "type": "haystack_integrations.components.generators.cohere.chat.chat_generator.CohereChatGenerator",
             "init_parameters": {
                 "model": "command",
                 "streaming_callback": None,
                 "api_key": {"env_vars": ["COHERE_API_KEY", "CO_API_KEY"], "strict": True, "type": "env_var"},
-                "api_base_url": "https://api.cohere.ai",
+                "api_base_url": "https://api.cohere.com",
                 "generation_kwargs": {},
             },
         }
 
     def test_to_dict_with_parameters(self, monkeypatch):
         monkeypatch.setenv("COHERE_API_KEY", "test-api-key")
         monkeypatch.setenv("CO_API_KEY", "fake-api-key")
@@ -205,15 +226,15 @@
         # check that the component returns the correct response
         assert isinstance(response, dict)
         assert "replies" in response
         assert isinstance(response["replies"], list)
         assert len(response["replies"]) == 1
         assert [isinstance(reply, ChatMessage) for reply in response["replies"]]
 
-    def test_run_streaming(self, chat_messages, mock_chat_response):
+    def test_run_streaming(self, chat_messages, mock_chat_streaming_response):
         streaming_call_count = 0
 
         # Define the streaming callback function and assert that it is called with StreamingChunk objects
         def streaming_callback_fn(chunk: StreamingChunk):
             nonlocal streaming_call_count
             streaming_call_count += 1
             assert isinstance(chunk, StreamingChunk)
@@ -225,15 +246,15 @@
         # Create a fake streamed response
         # self needed here, don't remove
         def mock_iter(self):  # noqa: ARG001
             yield streaming_chunk("Hello")
             yield streaming_chunk("How are you?")
 
         mock_response = Mock(**{"__iter__": mock_iter})
-        mock_chat_response.return_value = mock_response
+        mock_chat_streaming_response.return_value = mock_response
 
         response = generator.run(chat_messages)
 
         # Assert that the streaming callback was called twice
         assert streaming_call_count == 2
 
         # Assert that the response contains the generated replies
```

### Comparing `cohere_haystack-0.6.0/tests/test_cohere_generators.py` & `cohere_haystack-0.7.0/tests/test_cohere_generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # SPDX-FileCopyrightText: 2023-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
 import os
 
 import pytest
-from cohere import COHERE_API_URL
 from haystack.components.generators.utils import print_streaming_chunk
 from haystack.utils import Secret
 from haystack_integrations.components.generators.cohere import CohereGenerator
 
 pytestmark = pytest.mark.generators
+COHERE_API_URL = "https://api.cohere.com"
 
 
 class TestCohereGenerator:
     def test_init_default(self, monkeypatch):
         monkeypatch.setenv("COHERE_API_KEY", "foo")
         component = CohereGenerator()
         assert component.api_key == Secret.from_env_var(["COHERE_API_KEY", "CO_API_KEY"])
```

### Comparing `cohere_haystack-0.6.0/tests/test_cohere_ranker.py` & `cohere_haystack-0.7.0/tests/test_cohere_ranker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 from unittest.mock import Mock, patch
 
 import pytest
-from cohere import COHERE_API_URL
 from haystack import Document
 from haystack.utils.auth import Secret
 from haystack_integrations.components.rankers.cohere import CohereRanker
 
 pytestmark = pytest.mark.ranker
+COHERE_API_URL = "https://api.cohere.com"
 
 
 @pytest.fixture
 def mock_ranker_response():
     """
     Mock the Cohere ranker API response and reuse it for tests
     The `response` is an object of <class 'cohere.responses.rerank.Reranking'>
```

### Comparing `cohere_haystack-0.6.0/tests/test_document_embedder.py` & `cohere_haystack-0.7.0/tests/test_document_embedder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # SPDX-FileCopyrightText: 2023-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
 import os
 
 import pytest
-from cohere import COHERE_API_URL
 from haystack import Document
 from haystack.utils import Secret
 from haystack_integrations.components.embedders.cohere import CohereDocumentEmbedder
 
 pytestmark = pytest.mark.embedders
+COHERE_API_URL = "https://api.cohere.com"
 
 
 class TestCohereDocumentEmbedder:
     def test_init_default(self):
         embedder = CohereDocumentEmbedder()
         assert embedder.api_key == Secret.from_env_var(["COHERE_API_KEY", "CO_API_KEY"])
         assert embedder.model == "embed-english-v2.0"
```

### Comparing `cohere_haystack-0.6.0/tests/test_text_embedder.py` & `cohere_haystack-0.7.0/tests/test_text_embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # SPDX-FileCopyrightText: 2023-present deepset GmbH <info@deepset.ai>
 #
 # SPDX-License-Identifier: Apache-2.0
 import os
 
 import pytest
-from cohere import COHERE_API_URL
 from haystack.utils import Secret
 from haystack_integrations.components.embedders.cohere import CohereTextEmbedder
 
 pytestmark = pytest.mark.embedders
+COHERE_API_URL = "https://api.cohere.com"
 
 
 class TestCohereTextEmbedder:
     def test_init_default(self):
         """
         Test default initialization parameters for CohereTextEmbedder.
         """
```

### Comparing `cohere_haystack-0.6.0/.gitignore` & `cohere_haystack-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.6.0/LICENSE.txt` & `cohere_haystack-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.6.0/README.md` & `cohere_haystack-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `cohere_haystack-0.6.0/pyproject.toml` & `cohere_haystack-0.7.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 description = ''
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [{ name = "deepset GmbH", email = "info@deepset.ai" }]
 classifiers = [
+  "License :: OSI Approved :: Apache Software License",
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "haystack-ai",
-  "cohere<5",
+  "cohere==5.*",
 ]
 
 [project.urls]
 Documentation = "https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/cohere#readme"
 Issues = "https://github.com/deepset-ai/haystack-core-integrations/issues"
 Source = "https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/cohere"
```

### Comparing `cohere_haystack-0.6.0/PKG-INFO` & `cohere_haystack-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.3
 Name: cohere-haystack
-Version: 0.6.0
+Version: 0.7.0
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/cohere#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/cohere
 Author-email: deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
-Requires-Dist: cohere<5
+Requires-Dist: cohere==5.*
 Requires-Dist: haystack-ai
 Description-Content-Type: text/markdown
 
 # cohere-haystack
 
 [![PyPI - Version](https://img.shields.io/pypi/v/cohere-haystack.svg)](https://pypi.org/project/cohere-haystack)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cohere-haystack.svg)](https://pypi.org/project/cohere-haystack)
```

