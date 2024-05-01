# Comparing `tmp/langchain_openai-0.1.4.tar.gz` & `tmp/langchain_openai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_openai-0.1.4.tar", max compression
+gzip compressed data, was "langchain_openai-0.1.5.tar", max compression
```

## Comparing `langchain_openai-0.1.4.tar` & `langchain_openai-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1072 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/LICENSE
--rw-r--r--   0        0        0     1627 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/README.md
--rw-r--r--   0        0        0      371 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/__init__.py
--rw-r--r--   0        0        0      176 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/chat_models/__init__.py
--rw-r--r--   0        0        0    10508 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/chat_models/azure.py
--rw-r--r--   0        0        0    46560 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/chat_models/base.py
--rw-r--r--   0        0        0      198 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/embeddings/__init__.py
--rw-r--r--   0        0        0     6567 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/embeddings/azure.py
--rw-r--r--   0        0        0    24428 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/embeddings/base.py
--rw-r--r--   0        0        0      146 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/llms/__init__.py
--rw-r--r--   0        0        0     8008 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/llms/azure.py
--rw-r--r--   0        0        0    24578 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/llms/base.py
--rw-r--r--   0        0        0      229 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/output_parsers/__init__.py
--rw-r--r--   0        0        0      229 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/output_parsers/tools.py
--rw-r--r--   0        0        0        0 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/langchain_openai/py.typed
--rw-r--r--   0        0        0     2819 2024-04-26 17:07:52.382929 langchain_openai-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2484 1970-01-01 00:00:00.000000 langchain_openai-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1627 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/README.md
+-rw-r--r--   0        0        0      371 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/chat_models/__init__.py
+-rw-r--r--   0        0        0    10790 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/chat_models/azure.py
+-rw-r--r--   0        0        0    46599 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/chat_models/base.py
+-rw-r--r--   0        0        0      198 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/embeddings/__init__.py
+-rw-r--r--   0        0        0     6567 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/embeddings/azure.py
+-rw-r--r--   0        0        0    22520 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/embeddings/base.py
+-rw-r--r--   0        0        0      146 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/llms/__init__.py
+-rw-r--r--   0        0        0     8354 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/llms/azure.py
+-rw-r--r--   0        0        0    24578 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/llms/base.py
+-rw-r--r--   0        0        0      229 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/output_parsers/__init__.py
+-rw-r--r--   0        0        0      229 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/output_parsers/tools.py
+-rw-r--r--   0        0        0        0 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/langchain_openai/py.typed
+-rw-r--r--   0        0        0     2835 2024-05-01 22:04:08.008416 langchain_openai-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2484 1970-01-01 00:00:00.000000 langchain_openai-0.1.5/PKG-INFO
```

### Comparing `langchain_openai-0.1.4/LICENSE` & `langchain_openai-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.4/README.md` & `langchain_openai-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.4/langchain_openai/chat_models/azure.py` & `langchain_openai-0.1.5/langchain_openai/chat_models/azure.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import openai
 from langchain_core.outputs import ChatResult
 from langchain_core.pydantic_v1 import Field, SecretStr, root_validator
 from langchain_core.utils import convert_to_secret_str, get_from_dict_or_env
 
-from langchain_openai.chat_models.base import ChatOpenAI
+from langchain_openai.chat_models.base import BaseChatOpenAI
 
 logger = logging.getLogger(__name__)
 
 
-class AzureChatOpenAI(ChatOpenAI):
+class AzureChatOpenAI(BaseChatOpenAI):
     """`Azure OpenAI` Chat Completion API.
 
     To use this class you
     must have a deployed model on Azure OpenAI. Use `deployment_name` in the
     constructor to refer to the "Model deployment name" in the Azure portal.
 
     In addition, you should have the
@@ -96,14 +96,25 @@
     """
 
     @classmethod
     def get_lc_namespace(cls) -> List[str]:
         """Get the namespace of the langchain object."""
         return ["langchain", "chat_models", "azure_openai"]
 
+    @property
+    def lc_secrets(self) -> Dict[str, str]:
+        return {
+            "openai_api_key": "AZURE_OPENAI_API_KEY",
+            "azure_ad_token": "AZURE_OPENAI_AD_TOKEN",
+        }
+
+    @classmethod
+    def is_lc_serializable(cls) -> bool:
+        return True
+
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that api key and python package exists in environment."""
         if values["n"] < 1:
             raise ValueError("n must be at least 1.")
         if values["n"] > 1 and values["streaming"]:
             raise ValueError("n must be 1 when streaming.")
```

### Comparing `langchain_openai-0.1.4/langchain_openai/chat_models/base.py` & `langchain_openai-0.1.5/langchain_openai/chat_models/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,60 +287,15 @@
 
 class _AllReturnType(TypedDict):
     raw: BaseMessage
     parsed: Optional[_DictOrPydantic]
     parsing_error: Optional[BaseException]
 
 
-class ChatOpenAI(BaseChatModel):
-    """`OpenAI` Chat large language models API.
-
-    To use, you should have the environment variable ``OPENAI_API_KEY``
-    set with your API key, or pass it as a named parameter to the constructor.
-
-    Any parameters that are valid to be passed to the openai.create call can be passed
-    in, even if not explicitly saved on this class.
-
-    Example:
-        .. code-block:: python
-
-            from langchain_openai import ChatOpenAI
-
-            model = ChatOpenAI(model="gpt-3.5-turbo")
-    """
-
-    @property
-    def lc_secrets(self) -> Dict[str, str]:
-        return {"openai_api_key": "OPENAI_API_KEY"}
-
-    @classmethod
-    def get_lc_namespace(cls) -> List[str]:
-        """Get the namespace of the langchain object."""
-        return ["langchain", "chat_models", "openai"]
-
-    @property
-    def lc_attributes(self) -> Dict[str, Any]:
-        attributes: Dict[str, Any] = {}
-
-        if self.openai_organization:
-            attributes["openai_organization"] = self.openai_organization
-
-        if self.openai_api_base:
-            attributes["openai_api_base"] = self.openai_api_base
-
-        if self.openai_proxy:
-            attributes["openai_proxy"] = self.openai_proxy
-
-        return attributes
-
-    @classmethod
-    def is_lc_serializable(cls) -> bool:
-        """Return whether this model can be serialized by Langchain."""
-        return True
-
+class BaseChatOpenAI(BaseChatModel):
     client: Any = Field(default=None, exclude=True)  #: :meta private:
     async_client: Any = Field(default=None, exclude=True)  #: :meta private:
     model_name: str = Field(default="gpt-3.5-turbo", alias="model")
     """Model name to use."""
     temperature: float = 0.7
     """What sampling temperature to use."""
     model_kwargs: Dict[str, Any] = Field(default_factory=dict)
@@ -1089,14 +1044,61 @@
                 [parser_none], exception_key="parsing_error"
             )
             return RunnableMap(raw=llm) | parser_with_fallback
         else:
             return llm | output_parser
 
 
+class ChatOpenAI(BaseChatOpenAI):
+    """`OpenAI` Chat large language models API.
+
+    To use, you should have the environment variable ``OPENAI_API_KEY``
+    set with your API key, or pass it as a named parameter to the constructor.
+
+    Any parameters that are valid to be passed to the openai.create call can be passed
+    in, even if not explicitly saved on this class.
+
+    Example:
+        .. code-block:: python
+
+            from langchain_openai import ChatOpenAI
+
+            model = ChatOpenAI(model="gpt-3.5-turbo")
+    """
+
+    @property
+    def lc_secrets(self) -> Dict[str, str]:
+        return {"openai_api_key": "OPENAI_API_KEY"}
+
+    @classmethod
+    def get_lc_namespace(cls) -> List[str]:
+        """Get the namespace of the langchain object."""
+        return ["langchain", "chat_models", "openai"]
+
+    @property
+    def lc_attributes(self) -> Dict[str, Any]:
+        attributes: Dict[str, Any] = {}
+
+        if self.openai_organization:
+            attributes["openai_organization"] = self.openai_organization
+
+        if self.openai_api_base:
+            attributes["openai_api_base"] = self.openai_api_base
+
+        if self.openai_proxy:
+            attributes["openai_proxy"] = self.openai_proxy
+
+        return attributes
+
+    @classmethod
+    def is_lc_serializable(cls) -> bool:
+        """Return whether this model can be serialized by Langchain."""
+        return True
+
+
 def _is_pydantic_class(obj: Any) -> bool:
     return isinstance(obj, type) and issubclass(obj, BaseModel)
 
 
 def _lc_tool_call_to_openai_tool_call(tool_call: ToolCall) -> dict:
     return {
         "type": "function",
```

### Comparing `langchain_openai-0.1.4/langchain_openai/embeddings/azure.py` & `langchain_openai-0.1.5/langchain_openai/embeddings/azure.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.4/langchain_openai/embeddings/base.py` & `langchain_openai-0.1.5/langchain_openai/embeddings/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,16 +78,16 @@
     openai_proxy: Optional[str] = None
     embedding_ctx_length: int = 8191
     """The maximum number of tokens to embed at once."""
     openai_api_key: Optional[SecretStr] = Field(default=None, alias="api_key")
     """Automatically inferred from env var `OPENAI_API_KEY` if not provided."""
     openai_organization: Optional[str] = Field(default=None, alias="organization")
     """Automatically inferred from env var `OPENAI_ORG_ID` if not provided."""
-    allowed_special: Union[Literal["all"], Set[str]] = set()
-    disallowed_special: Union[Literal["all"], Set[str], Sequence[str]] = "all"
+    allowed_special: Union[Literal["all"], Set[str], None] = None
+    disallowed_special: Union[Literal["all"], Set[str], Sequence[str], None] = None
     chunk_size: int = 1000
     """Maximum number of texts to embed in each batch"""
     max_retries: int = 2
     """Maximum number of retries to make when generating."""
     request_timeout: Optional[Union[float, Tuple[float, float], Any]] = Field(
         default=None, alias="timeout"
     )
@@ -242,44 +242,25 @@
     @property
     def _invocation_params(self) -> Dict[str, Any]:
         params: Dict = {"model": self.model, **self.model_kwargs}
         if self.dimensions is not None:
             params["dimensions"] = self.dimensions
         return params
 
-    # please refer to
-    # https://github.com/openai/openai-cookbook/blob/main/examples/Embedding_long_inputs.ipynb
-    def _get_len_safe_embeddings(
-        self, texts: List[str], *, engine: str, chunk_size: Optional[int] = None
-    ) -> List[List[float]]:
-        """
-        Generate length-safe embeddings for a list of texts.
-
-        This method handles tokenization and embedding generation, respecting the
-        set embedding context length and chunk size. It supports both tiktoken
-        and HuggingFace tokenizer based on the tiktoken_enabled flag.
-
-        Args:
-            texts (List[str]): A list of texts to embed.
-            engine (str): The engine or model to use for embeddings.
-            chunk_size (Optional[int]): The size of chunks for processing embeddings.
-
-        Returns:
-            List[List[float]]: A list of embeddings for each input text.
-        """
-
+    def _tokenize(
+        self, texts: List[str], chunk_size: int
+    ) -> Tuple[Iterable[int], List[List[float]], List[int]]:
         tokens = []
         indices = []
         model_name = self.tiktoken_model_name or self.model
-        _chunk_size = chunk_size or self.chunk_size
 
         # If tiktoken flag set to False
         if not self.tiktoken_enabled:
             try:
-                from transformers import AutoTokenizer  # noqa: F401
+                from transformers import AutoTokenizer
             except ImportError:
                 raise ValueError(
                     "Could not import transformers python package. "
                     "This is needed in order to for OpenAIEmbeddings without "
                     "`tiktoken`. Please install it with `pip install transformers`. "
                 )
 
@@ -299,42 +280,72 @@
                     tokens.append(chunk_text)
                     indices.append(i)
         else:
             try:
                 encoding = tiktoken.encoding_for_model(model_name)
             except KeyError:
                 encoding = tiktoken.get_encoding("cl100k_base")
+            encoder_kwargs: Dict[str, Any] = {
+                k: v
+                for k, v in {
+                    "allowed_special": self.allowed_special,
+                    "disallowed_special": self.disallowed_special,
+                }.items()
+                if v is not None
+            }
             for i, text in enumerate(texts):
                 if self.model.endswith("001"):
                     # See: https://github.com/openai/openai-python/
                     #      issues/418#issuecomment-1525939500
                     # replace newlines, which can negatively affect performance.
                     text = text.replace("\n", " ")
 
-                token = encoding.encode(
-                    text=text,
-                    allowed_special=self.allowed_special,
-                    disallowed_special=self.disallowed_special,
-                )
+                if encoder_kwargs:
+                    token = encoding.encode(text, **encoder_kwargs)
+                else:
+                    token = encoding.encode_ordinary(text)
 
                 # Split tokens into chunks respecting the embedding_ctx_length
                 for j in range(0, len(token), self.embedding_ctx_length):
                     tokens.append(token[j : j + self.embedding_ctx_length])
                     indices.append(i)
 
         if self.show_progress_bar:
             try:
                 from tqdm.auto import tqdm
 
-                _iter: Iterable = tqdm(range(0, len(tokens), _chunk_size))
+                _iter: Iterable = tqdm(range(0, len(tokens), chunk_size))
             except ImportError:
-                _iter = range(0, len(tokens), _chunk_size)
+                _iter = range(0, len(tokens), chunk_size)
         else:
-            _iter = range(0, len(tokens), _chunk_size)
+            _iter = range(0, len(tokens), chunk_size)
+        return _iter, tokens, indices
+
+    # please refer to
+    # https://github.com/openai/openai-cookbook/blob/main/examples/Embedding_long_inputs.ipynb
+    def _get_len_safe_embeddings(
+        self, texts: List[str], *, engine: str, chunk_size: Optional[int] = None
+    ) -> List[List[float]]:
+        """
+        Generate length-safe embeddings for a list of texts.
 
+        This method handles tokenization and embedding generation, respecting the
+        set embedding context length and chunk size. It supports both tiktoken
+        and HuggingFace tokenizer based on the tiktoken_enabled flag.
+
+        Args:
+            texts (List[str]): A list of texts to embed.
+            engine (str): The engine or model to use for embeddings.
+            chunk_size (Optional[int]): The size of chunks for processing embeddings.
+
+        Returns:
+            List[List[float]]: A list of embeddings for each input text.
+        """
+        _chunk_size = chunk_size or self.chunk_size
+        _iter, tokens, indices = self._tokenize(texts, _chunk_size)
         batched_embeddings: List[List[float]] = []
         for i in _iter:
             response = self.client.create(
                 input=tokens[i : i + _chunk_size], **self._invocation_params
             )
             if not isinstance(response, dict):
                 response = response.model_dump()
@@ -395,70 +406,16 @@
             engine (str): The engine or model to use for embeddings.
             chunk_size (Optional[int]): The size of chunks for processing embeddings.
 
         Returns:
             List[List[float]]: A list of embeddings for each input text.
         """
 
-        tokens = []
-        indices = []
-        model_name = self.tiktoken_model_name or self.model
         _chunk_size = chunk_size or self.chunk_size
-
-        # If tiktoken flag set to False
-        if not self.tiktoken_enabled:
-            try:
-                from transformers import AutoTokenizer
-            except ImportError:
-                raise ValueError(
-                    "Could not import transformers python package. "
-                    "This is needed in order to for OpenAIEmbeddings without "
-                    " `tiktoken`. Please install it with `pip install transformers`."
-                )
-
-            tokenizer = AutoTokenizer.from_pretrained(
-                pretrained_model_name_or_path=model_name
-            )
-            for i, text in enumerate(texts):
-                # Tokenize the text using HuggingFace transformers
-                tokenized = tokenizer.encode(text, add_special_tokens=False)
-
-                # Split tokens into chunks respecting the embedding_ctx_length
-                for j in range(0, len(tokenized), self.embedding_ctx_length):
-                    token_chunk = tokenized[j : j + self.embedding_ctx_length]
-
-                    # Convert token IDs back to a string
-                    chunk_text = tokenizer.decode(token_chunk)
-                    tokens.append(chunk_text)
-                    indices.append(i)
-        else:
-            try:
-                encoding = tiktoken.encoding_for_model(model_name)
-            except KeyError:
-                logger.warning("Warning: model not found. Using cl100k_base encoding.")
-                model = "cl100k_base"
-                encoding = tiktoken.get_encoding(model)
-            for i, text in enumerate(texts):
-                if self.model.endswith("001"):
-                    # See: https://github.com/openai/openai-python/
-                    #      issues/418#issuecomment-1525939500
-                    # replace newlines, which can negatively affect performance.
-                    text = text.replace("\n", " ")
-
-                token = encoding.encode(
-                    text=text,
-                    allowed_special=self.allowed_special,
-                    disallowed_special=self.disallowed_special,
-                )
-
-                # Split tokens into chunks respecting the embedding_ctx_length
-                for j in range(0, len(token), self.embedding_ctx_length):
-                    tokens.append(token[j : j + self.embedding_ctx_length])
-                    indices.append(i)
-
+        _iter, tokens, indices = self._tokenize(texts, _chunk_size)
         batched_embeddings: List[List[float]] = []
         _chunk_size = chunk_size or self.chunk_size
         for i in range(0, len(tokens), _chunk_size):
             response = await self.async_client.create(
                 input=tokens[i : i + _chunk_size], **self._invocation_params
             )
```

### Comparing `langchain_openai-0.1.4/langchain_openai/llms/azure.py` & `langchain_openai-0.1.5/langchain_openai/llms/azure.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,14 +68,26 @@
     """
 
     @classmethod
     def get_lc_namespace(cls) -> List[str]:
         """Get the namespace of the langchain object."""
         return ["langchain", "llms", "openai"]
 
+    @property
+    def lc_secrets(self) -> Dict[str, str]:
+        return {
+            "openai_api_key": "AZURE_OPENAI_API_KEY",
+            "azure_ad_token": "AZURE_OPENAI_AD_TOKEN",
+        }
+
+    @classmethod
+    def is_lc_serializable(cls) -> bool:
+        """Return whether this model can be serialized by Langchain."""
+        return True
+
     @root_validator()
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate that api key and python package exists in environment."""
         if values["n"] < 1:
             raise ValueError("n must be at least 1.")
         if values["streaming"] and values["n"] > 1:
             raise ValueError("Cannot stream results when n > 1.")
```

### Comparing `langchain_openai-0.1.4/langchain_openai/llms/base.py` & `langchain_openai-0.1.5/langchain_openai/llms/base.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -64,32 +64,14 @@
         ),
     )
 
 
 class BaseOpenAI(BaseLLM):
     """Base OpenAI large language model class."""
 
-    @property
-    def lc_secrets(self) -> Dict[str, str]:
-        return {"openai_api_key": "OPENAI_API_KEY"}
-
-    @property
-    def lc_attributes(self) -> Dict[str, Any]:
-        attributes: Dict[str, Any] = {}
-        if self.openai_api_base:
-            attributes["openai_api_base"] = self.openai_api_base
-
-        if self.openai_organization:
-            attributes["openai_organization"] = self.openai_organization
-
-        if self.openai_proxy:
-            attributes["openai_proxy"] = self.openai_proxy
-
-        return attributes
-
     client: Any = Field(default=None, exclude=True)  #: :meta private:
     async_client: Any = Field(default=None, exclude=True)  #: :meta private:
     model_name: str = Field(default="gpt-3.5-turbo-instruct", alias="model")
     """Model name to use."""
     temperature: float = 0.7
     """What sampling temperature to use."""
     max_tokens: int = 256
@@ -645,7 +627,25 @@
     def is_lc_serializable(cls) -> bool:
         """Return whether this model can be serialized by Langchain."""
         return True
 
     @property
     def _invocation_params(self) -> Dict[str, Any]:
         return {**{"model": self.model_name}, **super()._invocation_params}
+
+    @property
+    def lc_secrets(self) -> Dict[str, str]:
+        return {"openai_api_key": "OPENAI_API_KEY"}
+
+    @property
+    def lc_attributes(self) -> Dict[str, Any]:
+        attributes: Dict[str, Any] = {}
+        if self.openai_api_base:
+            attributes["openai_api_base"] = self.openai_api_base
+
+        if self.openai_organization:
+            attributes["openai_organization"] = self.openai_organization
+
+        if self.openai_proxy:
+            attributes["openai_proxy"] = self.openai_proxy
+
+        return attributes
```

### Comparing `langchain_openai-0.1.4/pyproject.toml` & `langchain_openai-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-openai"
-version = "0.1.4"
+version = "0.1.5"
 description = "An integration package connecting OpenAI and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
@@ -25,14 +25,15 @@
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
 langchain-core = { path = "../../core", develop = true }
 pytest-cov = "^4.1.0"
 langchain-standard-tests = { path = "../../standard-tests", develop = true }
+numpy = "^1.24"
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
```

### Comparing `langchain_openai-0.1.4/PKG-INFO` & `langchain_openai-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-openai
-Version: 0.1.4
+Version: 0.1.5
 Summary: An integration package connecting OpenAI and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

