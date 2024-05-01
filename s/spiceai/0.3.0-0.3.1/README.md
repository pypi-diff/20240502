# Comparing `tmp/spiceai-0.3.0.tar.gz` & `tmp/spiceai-0.3.1.tar.gz`

## Comparing `spiceai-0.3.0.tar` & `spiceai-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 spiceai-0.3.0/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 spiceai-0.3.0/scripts/mytoml.toml
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 spiceai-0.3.0/scripts/prompt.txt
--rw-r--r--   0        0        0     6011 2020-02-02 00:00:00.000000 spiceai-0.3.0/scripts/run.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 spiceai-0.3.0/spice/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 spiceai-0.3.0/spice/errors.py
--rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 spiceai-0.3.0/spice/models.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 spiceai-0.3.0/spice/providers.py
--rw-r--r--   0        0        0    31739 2020-02-02 00:00:00.000000 spiceai-0.3.0/spice/spice.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 spiceai-0.3.0/spice/spice_message.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 spiceai-0.3.0/spice/utils.py
--rw-r--r--   0        0        0    18773 2020-02-02 00:00:00.000000 spiceai-0.3.0/spice/wrapped_clients.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.3.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.3.0/LICENSE
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 spiceai-0.3.0/README.md
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 spiceai-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6361 2020-02-02 00:00:00.000000 spiceai-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 spiceai-0.3.1/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 spiceai-0.3.1/scripts/mytoml.toml
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 spiceai-0.3.1/scripts/prompt.txt
+-rw-r--r--   0        0        0     6011 2020-02-02 00:00:00.000000 spiceai-0.3.1/scripts/run.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spiceai-0.3.1/spice/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 spiceai-0.3.1/spice/errors.py
+-rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 spiceai-0.3.1/spice/models.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 spiceai-0.3.1/spice/providers.py
+-rw-r--r--   0        0        0    34031 2020-02-02 00:00:00.000000 spiceai-0.3.1/spice/spice.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 spiceai-0.3.1/spice/spice_message.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 spiceai-0.3.1/spice/utils.py
+-rw-r--r--   0        0        0    18773 2020-02-02 00:00:00.000000 spiceai-0.3.1/spice/wrapped_clients.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spiceai-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 spiceai-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 spiceai-0.3.1/tests/test_spice.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.3.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 spiceai-0.3.1/README.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 spiceai-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 spiceai-0.3.1/PKG-INFO
```

### Comparing `spiceai-0.3.0/.github/workflows/ruff.yml` & `spiceai-0.3.1/.github/workflows/ruff.yml`

 * *Files 16% similar despite different names*

```diff
@@ -17,7 +17,9 @@
           echo PATH=$PATH >> $GITHUB_ENV
       - name: ruff (linter)
         run: ruff check --select I .
       - name: ruff (formatter)
         run: ruff format --check .
       - name: pyright
         run: pyright
+      - name: pytest
+        run: pytest
```

### Comparing `spiceai-0.3.0/scripts/run.py` & `spiceai-0.3.1/scripts/run.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.0/spice/errors.py` & `spiceai-0.3.1/spice/errors.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.0/spice/models.py` & `spiceai-0.3.1/spice/models.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.0/spice/providers.py` & `spiceai-0.3.1/spice/providers.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 from dataclasses import dataclass
 from typing import Callable, List
 
 from dotenv import load_dotenv
 
-from spice.errors import InvalidProviderError, NoAPIKeyError, SpiceError
+from spice.errors import InvalidProviderError, NoAPIKeyError
 from spice.wrapped_clients import WrappedAnthropicClient, WrappedAzureClient, WrappedClient, WrappedOpenAIClient
 
 # Used to fetch a provider by name
 providers: List[Provider] = []
 
 
 @dataclass
```

### Comparing `spiceai-0.3.0/spice/spice.py` & `spiceai-0.3.1/spice/spice.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from jinja2 import Environment
 from openai.types.chat.completion_create_params import ResponseFormat
 
 from spice.errors import InvalidModelError, UnknownModelError
 from spice.models import EmbeddingModel, Model, TextModel, TranscriptionModel, get_model_from_name
 from spice.providers import Provider, get_provider_from_name
 from spice.spice_message import MessagesEncoder, SpiceMessage
-from spice.utils import embeddings_request_cost, text_request_cost, transcription_request_cost
+from spice.utils import embeddings_request_cost, print_stream, text_request_cost, transcription_request_cost
 from spice.wrapped_clients import WrappedClient
 
 
 @dataclass
 class SpiceCallArgs:
     model: str
     messages: Collection[SpiceMessage]
@@ -56,14 +56,17 @@
 
     completed: bool
     """Whether or not this response was fully completed. This will only ever be false for incomplete streamed responses."""
 
     cost: Optional[float]
     """The cost of this request in cents. May be inaccurate for incompleted streamed responses. Will be None if the cost of the model used is not known."""
 
+    retries: int = 0
+    """The number of retries that were made to get this response. Will be 0 if no retries were made."""
+
     @property
     def total_tokens(self) -> int:
         """The total tokens, input and output, in this response."""
         return self.input_tokens + self.output_tokens
 
     @property
     def characters_per_second(self) -> float:
@@ -78,27 +81,29 @@
 
     def __init__(
         self,
         model: TextModel,
         call_args: SpiceCallArgs,
         client: WrappedClient,
         stream: AsyncIterator,
-        callback: Callable[[SpiceResponse], None],
+        callback: Optional[Callable[[SpiceResponse], None]] = None,
+        streaming_callback: Optional[Callable[[str], None]] = None,
     ):
         self._model = model
         self._call_args = call_args
         self._text = []
         self._start_time = timer()
         self._end_time = None
         self._input_tokens = None
         self._output_tokens = None
         self._finished = False
         self._client = client
         self._stream = stream
         self._callback = callback
+        self._streaming_callback = streaming_callback
 
     def __aiter__(self):
         return self
 
     async def __anext__(self):
         with self._client.catch_and_convert_errors():
             try:
@@ -106,14 +111,16 @@
                 while content is None:
                     chunk = await anext(self._stream)
                     content, input_tokens, output_tokens = self._client.process_chunk(chunk)
                     if input_tokens is not None:
                         self._input_tokens = input_tokens
                     if output_tokens is not None:
                         self._output_tokens = output_tokens
+                if self._streaming_callback is not None:
+                    self._streaming_callback(content)
                 self._text.append(content)
                 return content
             except StopAsyncIteration:
                 self._end_time = timer()
                 self._finished = True
                 raise
 
@@ -140,15 +147,16 @@
             full_output,
             self._end_time - self._start_time,
             input_tokens,
             output_tokens,
             self._finished,
             cost,
         )
-        self._callback(response)
+        if self._callback is not None:
+            self._callback(response)
 
         return response
 
     async def complete_response(self) -> SpiceResponse:
         """
         Waits until the entire LLM call finishes, collects it, and returns its SpiceResponse.
         """
@@ -344,14 +352,17 @@
         messages: Collection[SpiceMessage],
         model: Optional[TextModel | str] = None,
         provider: Optional[Provider | str] = None,
         temperature: Optional[float] = None,
         max_tokens: Optional[int] = None,
         response_format: Optional[ResponseFormat] = None,
         name: Optional[str] = None,
+        validator: Optional[Callable[[str], bool]] = None,
+        streaming_callback: Optional[Callable[[str], None]] = None,
+        retries: int = 0,
     ) -> SpiceResponse:
         """
         Asynchronously retrieves a chat completion response.
 
         Args:
             messages: The list of messages given as context for the completion.
             Will raise an ImageError if any invalid images are given.
@@ -367,43 +378,73 @@
 
             max_tokens: The maximum tokens the model can output.
 
             response_format: For valid models, will set the response format to 'text' or 'json'.
             If the provider/model does not support response_format, this argument will be ignored.
 
             name: If given, will be given this name when logged.
-        """
 
-        text_model = self._get_text_model(model)
-        client = self._get_client(text_model, provider)
-        call_args = self._fix_call_args(messages, text_model, False, temperature, max_tokens, response_format)
+            validator: If given, will be called with the text of the response. If it returns False, the response will be discarded and another attempt will be made.
 
-        start_time = timer()
-        with client.catch_and_convert_errors():
-            chat_completion = await client.get_chat_completion_or_stream(call_args)
-        end_time = timer()
-        text, input_tokens, output_tokens = client.extract_text_and_tokens(chat_completion)
-
-        cost = text_request_cost(text_model, input_tokens, output_tokens)
-        if cost is not None:
-            self._total_cost += cost
+            streaming_callback: If given, will be called with the text of the response as it is received.
 
-        response = SpiceResponse(call_args, text, end_time - start_time, input_tokens, output_tokens, True, cost)
-        self._log_response(response, name)
-        return response
+            retries: The number of times to retry getting a valid response. If 0, will not retry. If after all retries no valid response is received, will raise a ValueError.
+        """
+        start_time = timer()
+        cost = 0
+        for i in range(retries + 1):
+            text_model = self._get_text_model(model)
+            client = self._get_client(text_model, provider)
+            call_args = self._fix_call_args(
+                messages, text_model, streaming_callback is not None, temperature, max_tokens, response_format
+            )
+
+            with client.catch_and_convert_errors():
+                if streaming_callback is not None:
+                    stream = await client.get_chat_completion_or_stream(call_args)
+                    stream = cast(AsyncIterator, stream)
+                    streaming_spice_response = StreamingSpiceResponse(
+                        text_model, call_args, client, stream, None, streaming_callback
+                    )
+                    chat_completion = await streaming_spice_response.complete_response()
+                    text, input_tokens, output_tokens = (
+                        chat_completion.text,
+                        chat_completion.input_tokens,
+                        chat_completion.output_tokens,
+                    )
+
+                else:
+                    chat_completion = await client.get_chat_completion_or_stream(call_args)
+                    text, input_tokens, output_tokens = client.extract_text_and_tokens(chat_completion)
+
+            completion_cost = text_request_cost(text_model, input_tokens, output_tokens)
+            if completion_cost is not None:
+                cost += completion_cost
+                self._total_cost += completion_cost
+
+            if validator is not None and not validator(text):
+                continue
+            end_time = timer()
+            response = SpiceResponse(
+                call_args, text, end_time - start_time, input_tokens, output_tokens, True, cost, retries=i
+            )
+            self._log_response(response, name)
+            return response
+        raise ValueError("Failed to get a valid response after all retries")
 
     async def stream_response(
         self,
         messages: Collection[SpiceMessage],
         model: Optional[TextModel | str] = None,
         provider: Optional[Provider | str] = None,
         temperature: Optional[float] = None,
         max_tokens: Optional[int] = None,
         response_format: Optional[ResponseFormat] = None,
         name: Optional[str] = None,
+        streaming_callback: Optional[Callable[[str], None]] = None,
     ) -> StreamingSpiceResponse:
         """
         Asynchronously retrieves a chat completion stream that can be iterated over asynchronously.
 
         Args:
             messages: The list of messages given as context for the completion.
             Will raise an ImageError if any invalid images are given.
@@ -436,15 +477,15 @@
         def callback(response: SpiceResponse, cache: List[float] = [0]):
             if response.cost is not None:
                 self._total_cost += response.cost - cache[0]
                 cache[0] = response.cost
             # TODO: Do we want to log multiple times? Our old log might be incomplete, which is why this is still in, but probably not necessary.
             self._log_response(response, name)
 
-        return StreamingSpiceResponse(text_model, call_args, client, stream, callback)
+        return StreamingSpiceResponse(text_model, call_args, client, stream, callback, streaming_callback)
 
     def _get_embedding_model(self, model: Optional[Model | str]) -> EmbeddingModel:
         if model is None:
             if self._default_embeddings_model is None:
                 raise InvalidModelError("Model is required when default embeddings model is not set at initialization")
             model = self._default_embeddings_model
```

### Comparing `spiceai-0.3.0/spice/spice_message.py` & `spiceai-0.3.1/spice/spice_message.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.0/spice/utils.py` & `spiceai-0.3.1/spice/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,7 +18,11 @@
 
 
 def transcription_request_cost(model: TranscriptionModel, input_length: float) -> Optional[float]:
     if model.input_cost is not None:
         return (model.input_cost * input_length) / 100
     else:
         return None
+
+
+def print_stream(text: str) -> None:
+    print(text, end="", flush=True)
```

### Comparing `spiceai-0.3.0/spice/wrapped_clients.py` & `spiceai-0.3.1/spice/wrapped_clients.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.0/LICENSE` & `spiceai-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.0/README.md` & `spiceai-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.0/pyproject.toml` & `spiceai-0.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.hatch]
 
 [tool.hatch.build.targets.wheel]
 packages=["spice"]
 
 [project]
 name = "spiceai"
-version = "0.3.0"
+version = "0.3.1"
 license = {text = "Apache-2.0"}
 description = "A Python library for building AI-powered applications."
 readme = "README.md"
 dependencies = [
     "python-dotenv",
     "openai",
     "anthropic",
@@ -25,9 +25,11 @@
     "httpx",
     "jinja2"
 ]
 
 [project.optional-dependencies]
 dev = [
     "ruff",
-    "pyright"
+    "pyright",
+    "pytest",
+    "pytest-asyncio"
 ]
```

### Comparing `spiceai-0.3.0/PKG-INFO` & `spiceai-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.3
 Name: spiceai
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python library for building AI-powered applications.
 License: Apache-2.0
 License-File: LICENSE
 Requires-Dist: anthropic
 Requires-Dist: httpx
 Requires-Dist: jinja2
 Requires-Dist: openai
 Requires-Dist: pillow
 Requires-Dist: python-dotenv
 Requires-Dist: tiktoken
 Provides-Extra: dev
 Requires-Dist: pyright; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-asyncio; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Spice
 
 Spice is a light wrapper for AI SDKs like OpenAI's and Anthropic's. Spice simplifies LLM creations, embeddings, and transcriptions without obscuring any underlying parameters or processes. Spice also makes it ridiculously easy to switch between different providers, such as OpenAI and Anthropic, without having to modify your code.
```

