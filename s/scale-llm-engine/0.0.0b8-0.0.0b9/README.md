# Comparing `tmp/scale_llm_engine-0.0.0b8.tar.gz` & `tmp/scale_llm_engine-0.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_llm_engine-0.0.0b8.tar", max compression
+gzip compressed data, was "scale_llm_engine-0.0.0b9.tar", max compression
```

## Comparing `scale_llm_engine-0.0.0b8.tar` & `scale_llm_engine-0.0.0b9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1002 2023-07-21 08:53:27.233160 scale_llm_engine-0.0.0b8/README.md
--rw-r--r--   0        0        0     1870 2023-08-01 18:32:34.086159 scale_llm_engine-0.0.0b8/llmengine/__init__.py
--rw-r--r--   0        0        0     7065 2023-08-01 23:09:51.651675 scale_llm_engine-0.0.0b8/llmengine/api_engine.py
--rw-r--r--   0        0        0    13065 2023-07-21 08:53:27.234217 scale_llm_engine-0.0.0b8/llmengine/completion.py
--rw-r--r--   0        0        0    15229 2023-08-01 18:32:34.087511 scale_llm_engine-0.0.0b8/llmengine/data_types.py
--rw-r--r--   0        0        0     2745 2023-07-18 18:23:40.550782 scale_llm_engine-0.0.0b8/llmengine/errors.py
--rw-r--r--   0        0        0     5290 2023-08-01 18:32:34.088194 scale_llm_engine-0.0.0b8/llmengine/file.py
--rw-r--r--   0        0        0    14021 2023-07-21 08:53:27.235057 scale_llm_engine-0.0.0b8/llmengine/fine_tuning.py
--rw-r--r--   0        0        0    14588 2023-07-31 19:50:25.084434 scale_llm_engine-0.0.0b8/llmengine/model.py
--rw-r--r--   0        0        0      807 2023-08-01 18:32:34.088861 scale_llm_engine-0.0.0b8/pyproject.toml
--rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0b8/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-07-19 22:48:02.087687 scale_llm_engine-0.0.0b9/README.md
+-rw-r--r--   0        0        0     1870 2023-08-04 19:16:03.736467 scale_llm_engine-0.0.0b9/llmengine/__init__.py
+-rw-r--r--   0        0        0     7065 2023-08-04 19:15:01.627657 scale_llm_engine-0.0.0b9/llmengine/api_engine.py
+-rw-r--r--   0        0        0    14740 2023-08-04 19:15:01.627657 scale_llm_engine-0.0.0b9/llmengine/completion.py
+-rw-r--r--   0        0        0    15866 2023-08-04 19:15:01.627657 scale_llm_engine-0.0.0b9/llmengine/data_types.py
+-rw-r--r--   0        0        0     2745 2023-07-19 22:48:02.087687 scale_llm_engine-0.0.0b9/llmengine/errors.py
+-rw-r--r--   0        0        0     5287 2023-08-04 19:15:01.627657 scale_llm_engine-0.0.0b9/llmengine/file.py
+-rw-r--r--   0        0        0    14021 2023-08-04 19:15:01.627657 scale_llm_engine-0.0.0b9/llmengine/fine_tuning.py
+-rw-r--r--   0        0        0    14588 2023-08-04 19:15:01.627657 scale_llm_engine-0.0.0b9/llmengine/model.py
+-rw-r--r--   0        0        0      807 2023-08-04 19:16:03.304461 scale_llm_engine-0.0.0b9/pyproject.toml
+-rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0b9/PKG-INFO
```

### Comparing `scale_llm_engine-0.0.0b8/README.md` & `scale_llm_engine-0.0.0b9/README.md`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b8/llmengine/__init__.py` & `scale_llm_engine-0.0.0b9/llmengine/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.0.beta8"
+__version__ = "0.0.0.beta9"
 
 from typing import Sequence
 
 from llmengine.completion import Completion
 from llmengine.data_types import (
     CancelFineTuneResponse,
     CompletionOutput,
```

### Comparing `scale_llm_engine-0.0.0b8/llmengine/api_engine.py` & `scale_llm_engine-0.0.0b9/llmengine/api_engine.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b8/llmengine/completion.py` & `scale_llm_engine-0.0.0b9/llmengine/completion.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import AsyncIterable, Iterator, Union
+from typing import AsyncIterable, Iterator, List, Optional, Union
 
 from llmengine.api_engine import APIEngine
 from llmengine.data_types import (
     CompletionStreamResponse,
     CompletionStreamV1Request,
     CompletionSyncResponse,
     CompletionSyncV1Request,
@@ -25,14 +25,16 @@
     @classmethod
     async def acreate(
         cls,
         model: str,
         prompt: str,
         max_new_tokens: int = 20,
         temperature: float = 0.2,
+        stop_sequences: Optional[List[str]] = None,
+        return_token_log_probs: Optional[bool] = False,
         timeout: int = 10,
         stream: bool = False,
     ) -> Union[CompletionSyncResponse, AsyncIterable[CompletionStreamResponse]]:
         """
         Creates a completion for the provided prompt and parameters asynchronously (with `asyncio`).
 
         This API can be used to get the LLM to generate a completion *asynchronously*.
@@ -53,16 +55,24 @@
             max_new_tokens (int):
                 The maximum number of tokens to generate in the completion.
 
                 The token count of your prompt plus `max_new_tokens` cannot exceed the model's context length. See
                 [Model Zoo](../../model_zoo) for information on each supported model's context length.
 
             temperature (float):
-                What sampling temperature to use, in the range `(0, 1]`. Higher values like 0.8 will make the output
+                What sampling temperature to use, in the range `[0, 1]`. Higher values like 0.8 will make the output
                 more random, while lower values like 0.2 will make it more focused and deterministic.
+                When temperature is 0 greedy sampling is used.
+
+            stop_sequences (Optional[List[str]]):
+                One or more sequences where the API will stop generating tokens for the current completion.
+
+            return_token_log_probs (Optional[bool]):
+                Whether to return the log probabilities of generated tokens.
+                When True, the response will include a list of tokens and their log probabilities.
 
             timeout (int):
                 Timeout in seconds. This is the maximum amount of time you are willing to wait for a response.
 
             stream (bool):
                 Whether to stream the response. If true, the return type is an
                 `Iterator[CompletionStreamResponse]`. Otherwise, the return type is a `CompletionSyncResponse`.
@@ -146,14 +156,16 @@
                     yield CompletionStreamResponse.parse_obj(chunk)
 
             return _acreate_stream(
                 model=model,
                 prompt=prompt,
                 max_new_tokens=max_new_tokens,
                 temperature=temperature,
+                stop_sequences=stop_sequences,
+                return_token_log_probs=return_token_log_probs,
                 timeout=timeout,
             )
 
         else:
 
             async def _acreate_sync(**kwargs) -> CompletionSyncResponse:
                 data = CompletionSyncV1Request(**kwargs).dict()
@@ -161,24 +173,30 @@
                     resource_name=f"v1/llm/completions-sync?model_endpoint_name={model}",
                     data=data,
                     timeout=timeout,
                 )
                 return CompletionSyncResponse.parse_obj(response)
 
             return await _acreate_sync(
-                prompt=prompt, max_new_tokens=max_new_tokens, temperature=temperature
+                prompt=prompt,
+                max_new_tokens=max_new_tokens,
+                temperature=temperature,
+                stop_sequences=stop_sequences,
+                return_token_log_probs=return_token_log_probs,
             )
 
     @classmethod
     def create(
         cls,
         model: str,
         prompt: str,
         max_new_tokens: int = 20,
         temperature: float = 0.2,
+        stop_sequences: Optional[List[str]] = None,
+        return_token_log_probs: Optional[bool] = False,
         timeout: int = 10,
         stream: bool = False,
     ) -> Union[CompletionSyncResponse, Iterator[CompletionStreamResponse]]:
         """
         Creates a completion for the provided prompt and parameters synchronously.
 
         This API can be used to get the LLM to generate a completion *synchronously*.
@@ -200,16 +218,24 @@
             max_new_tokens (int):
                 The maximum number of tokens to generate in the completion.
 
                 The token count of your prompt plus `max_new_tokens` cannot exceed the model's context length. See
                 [Model Zoo](../../model_zoo) for information on each supported model's context length.
 
             temperature (float):
-                What sampling temperature to use, in the range `(0, 1]`. Higher values like 0.8 will make the output
+                What sampling temperature to use, in the range `[0, 1]`. Higher values like 0.8 will make the output
                 more random, while lower values like 0.2 will make it more focused and deterministic.
+                When temperature is 0 greedy sampling is used.
+
+            stop_sequences (Optional[List[str]]):
+                One or more sequences where the API will stop generating tokens for the current completion.
+
+            return_token_log_probs (Optional[bool]):
+                Whether to return the log probabilities of generated tokens.
+                When True, the response will include a list of tokens and their log probabilities.
 
             timeout (int):
                 Timeout in seconds. This is the maximum amount of time you are willing to wait for a response.
 
             stream (bool):
                 Whether to stream the response. If true, the return type is an
                 `Iterator[CompletionStreamResponse]`. Otherwise, the return type is a `CompletionSyncResponse`.
@@ -280,20 +306,28 @@
                     data=data_stream,
                     timeout=timeout,
                 )
                 for chunk in response_stream:
                     yield CompletionStreamResponse.parse_obj(chunk)
 
             return _create_stream(
-                prompt=prompt, max_new_tokens=max_new_tokens, temperature=temperature
+                prompt=prompt,
+                max_new_tokens=max_new_tokens,
+                temperature=temperature,
+                stop_sequences=stop_sequences,
+                return_token_log_probs=return_token_log_probs,
             )
 
         else:
             data = CompletionSyncV1Request(
-                prompt=prompt, max_new_tokens=max_new_tokens, temperature=temperature
+                prompt=prompt,
+                max_new_tokens=max_new_tokens,
+                temperature=temperature,
+                stop_sequences=stop_sequences,
+                return_token_log_probs=return_token_log_probs,
             ).dict()
             response = cls.post_sync(
                 resource_name=f"v1/llm/completions-sync?model_endpoint_name={model}",
                 data=data,
                 timeout=timeout,
             )
             return CompletionSyncResponse.parse_obj(response)
```

### Comparing `scale_llm_engine-0.0.0b8/llmengine/data_types.py` & `scale_llm_engine-0.0.0b9/llmengine/data_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -178,15 +178,16 @@
 
 class GetLLMEndpointResponse(BaseModel):
     """
     Response object for retrieving a Model.
     """
 
     id: Optional[str] = Field(
-        default=None, description="(For self-hosted users) The autogenerated ID of the model."
+        default=None,
+        description="(For self-hosted users) The autogenerated ID of the model.",
     )
     """(For self-hosted users) The autogenerated ID of the model."""
 
     name: str = Field(
         description="The name of the model. Use this for making inference requests to the model."
     )
     """The name of the model. Use this for making inference requests to the model."""
@@ -255,28 +256,49 @@
 class CompletionSyncV1Request(BaseModel):
     """
     Request object for a synchronous prompt completion task.
     """
 
     prompt: str = Field(..., min_length=1)
     max_new_tokens: int = Field(..., gt=0)
-    temperature: float = Field(..., gt=0.0)
+    temperature: float = Field(..., ge=0.0)
+    stop_sequences: Optional[List[str]] = Field(default=None)
+    return_token_log_probs: Optional[bool] = Field(default=False)
+
+
+class TokenOutput(BaseModel):
+    """
+    Detailed token information.
+    """
+
+    token: str
+    """
+    The token text.
+    """
+
+    log_prob: float
+    """
+    The log probability of the token.
+    """
 
 
 class CompletionOutput(BaseModel):
     """
     Represents the output of a completion request to a model.
     """
 
     text: str
     """The text of the completion."""
 
     num_completion_tokens: int
     """Number of tokens in the completion."""
 
+    tokens: Optional[List[TokenOutput]] = None
+    """Detailed token information."""
+
 
 class CompletionSyncResponse(BaseModel):
     """
     Response object for a synchronous prompt completion.
     """
 
     request_id: str
@@ -295,27 +317,32 @@
 class CompletionStreamV1Request(BaseModel):
     """
     Request object for a streaming prompt completion.
     """
 
     prompt: str = Field(..., min_length=1)
     max_new_tokens: int = Field(..., gt=0)
-    temperature: float = Field(..., gt=0.0)
+    temperature: float = Field(..., ge=0.0)
+    stop_sequences: Optional[List[str]] = Field(default=None)
+    return_token_log_probs: Optional[bool] = Field(default=False)
 
 
 class CompletionStreamOutput(BaseModel):
     text: str
     """The text of the completion."""
 
     finished: bool
     """Whether the completion is finished."""
 
     num_completion_tokens: Optional[int] = None
     """Number of tokens in the completion."""
 
+    token: Optional[TokenOutput] = None
+    """Detailed token information."""
+
 
 class CompletionStreamResponse(BaseModel):
     """
     Response object for a stream prompt completion task.
     """
 
     request_id: str
```

### Comparing `scale_llm_engine-0.0.0b8/llmengine/errors.py` & `scale_llm_engine-0.0.0b9/llmengine/errors.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b8/llmengine/file.py` & `scale_llm_engine-0.0.0b9/llmengine/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,15 @@
         Returns:
             GetFileContentResponse: an object that contains the ID and content of the file
 
         === "Getting file content in Python"
             ```python
             from llmengine import File
 
-            response = File.get_content(file_id="file-abc123")
+            response = File.download(file_id="file-abc123")
             print(response.json())
             ```
 
         === "Response in JSON"
             ```json
             {
                 "id": "file-abc123",
```

### Comparing `scale_llm_engine-0.0.0b8/llmengine/fine_tuning.py` & `scale_llm_engine-0.0.0b9/llmengine/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b8/llmengine/model.py` & `scale_llm_engine-0.0.0b9/llmengine/model.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b8/pyproject.toml` & `scale_llm_engine-0.0.0b9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scale-llm-engine"
-version = "0.0.0.beta8"
+version = "0.0.0.beta9"
 description = "Scale LLM Engine Python client"
 license = "Apache-2.0"
 authors = ["Phil Chen <phil.chen@scale.com>"]
 maintainers = ["Phil Chen <phil.chen@scale.com>"]
 readme = "README.md"
 homepage = "https://scaleapi.github.io/llm-engine/"
 repository = "https://github.com/scaleapi/llm-engine"
```

### Comparing `scale_llm_engine-0.0.0b8/PKG-INFO` & `scale_llm_engine-0.0.0b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scale-llm-engine
-Version: 0.0.0b8
+Version: 0.0.0b9
 Summary: Scale LLM Engine Python client
 Home-page: https://scaleapi.github.io/llm-engine/
 License: Apache-2.0
 Author: Phil Chen
 Author-email: phil.chen@scale.com
 Maintainer: Phil Chen
 Maintainer-email: phil.chen@scale.com
```

