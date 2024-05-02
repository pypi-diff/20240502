# Comparing `tmp/llama_index_llms_huggingface-0.1.4.tar.gz` & `tmp/llama_index_llms_huggingface-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_huggingface-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_llms_huggingface-0.1.5.tar", max compression
```

## Comparing `llama_index_llms_huggingface-0.1.4.tar` & `llama_index_llms_huggingface-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       43 2024-03-12 21:01:02.653746 llama_index_llms_huggingface-0.1.4/README.md
--rw-r--r--   0        0        0      143 2024-03-12 21:01:02.653746 llama_index_llms_huggingface-0.1.4/llama_index/llms/huggingface/__init__.py
--rw-r--r--   0        0        0    23155 2024-03-12 21:01:02.653746 llama_index_llms_huggingface-0.1.4/llama_index/llms/huggingface/base.py
--rw-r--r--   0        0        0     1609 2024-03-12 21:01:02.653746 llama_index_llms_huggingface-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      741 1970-01-01 00:00:00.000000 llama_index_llms_huggingface-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       43 2024-05-02 03:19:40.949906 llama_index_llms_huggingface-0.1.5/README.md
+-rw-r--r--   0        0        0      212 2024-05-02 03:19:40.949906 llama_index_llms_huggingface-0.1.5/llama_index/llms/huggingface/__init__.py
+-rw-r--r--   0        0        0    39711 2024-05-02 03:19:40.949906 llama_index_llms_huggingface-0.1.5/llama_index/llms/huggingface/base.py
+-rw-r--r--   0        0        0     2082 2024-05-02 03:19:40.949906 llama_index_llms_huggingface-0.1.5/llama_index/llms/huggingface/utils.py
+-rw-r--r--   0        0        0     1636 2024-05-02 03:19:40.949906 llama_index_llms_huggingface-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 llama_index_llms_huggingface-0.1.5/PKG-INFO
```

### Comparing `llama_index_llms_huggingface-0.1.4/llama_index/llms/huggingface/base.py` & `llama_index_llms_huggingface-0.1.5/llama_index/llms/huggingface/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,45 +16,122 @@
     CompletionResponseGen,
     LLMMetadata,
     MessageRole,
 )
 from llama_index.core.bridge.pydantic import Field, PrivateAttr
 from llama_index.core.callbacks import CallbackManager
 from llama_index.core.constants import (
+    DEFAULT_TEMPERATURE,
     DEFAULT_CONTEXT_WINDOW,
     DEFAULT_NUM_OUTPUTS,
 )
 from llama_index.core.llms.callbacks import (
     llm_chat_callback,
     llm_completion_callback,
 )
+from llama_index.core.llms.llm import ToolSelection
 from llama_index.core.llms.custom import CustomLLM
+from llama_index.core.llms.function_calling import FunctionCallingLLM
 from llama_index.core.base.llms.generic_utils import (
     completion_response_to_chat_response,
     stream_completion_response_to_chat_response,
-)
-from llama_index.core.base.llms.generic_utils import (
     messages_to_prompt as generic_messages_to_prompt,
+    chat_to_completion_decorator,
+    achat_to_completion_decorator,
+    stream_chat_to_completion_decorator,
+    astream_chat_to_completion_decorator,
+    get_from_param_or_env,
 )
 from llama_index.core.prompts.base import PromptTemplate
 from llama_index.core.types import BaseOutputParser, PydanticProgramMode
+from llama_index.core.chat_engine.types import AgentChatResponse
+from llama_index.core.tools.types import BaseTool
+from llama_index.llms.huggingface.utils import (
+    to_tgi_messages,
+    force_single_tool_call,
+    resolve_tgi_function_call,
+    get_max_input_length,
+    resolve_tool_choice,
+)
 from transformers import (
     AutoModelForCausalLM,
     AutoTokenizer,
     StoppingCriteria,
     StoppingCriteriaList,
 )
+from text_generation import (
+    Client as TGIClient,
+    AsyncClient as TGIAsyncClient,
+)
 
 DEFAULT_HUGGINGFACE_MODEL = "StabilityAI/stablelm-tuned-alpha-3b"
 
 logger = logging.getLogger(__name__)
 
 
 class HuggingFaceLLM(CustomLLM):
-    """HuggingFace LLM."""
+    r"""HuggingFace LLM.
+
+    Examples:
+        `pip install llama-index-llms-huggingface`
+
+        ```python
+        from llama_index.llms.huggingface import HuggingFaceLLM
+
+        def messages_to_prompt(messages):
+            prompt = ""
+            for message in messages:
+                if message.role == 'system':
+                prompt += f"<|system|>\n{message.content}</s>\n"
+                elif message.role == 'user':
+                prompt += f"<|user|>\n{message.content}</s>\n"
+                elif message.role == 'assistant':
+                prompt += f"<|assistant|>\n{message.content}</s>\n"
+
+            # ensure we start with a system prompt, insert blank if needed
+            if not prompt.startswith("<|system|>\n"):
+                prompt = "<|system|>\n</s>\n" + prompt
+
+            # add final assistant prompt
+            prompt = prompt + "<|assistant|>\n"
+
+            return prompt
+
+        def completion_to_prompt(completion):
+            return f"<|system|>\n</s>\n<|user|>\n{completion}</s>\n<|assistant|>\n"
+
+        import torch
+        from transformers import BitsAndBytesConfig
+        from llama_index.core.prompts import PromptTemplate
+        from llama_index.llms.huggingface import HuggingFaceLLM
+
+        # quantize to save memory
+        quantization_config = BitsAndBytesConfig(
+            load_in_4bit=True,
+            bnb_4bit_compute_dtype=torch.float16,
+            bnb_4bit_quant_type="nf4",
+            bnb_4bit_use_double_quant=True,
+        )
+
+        llm = HuggingFaceLLM(
+            model_name="HuggingFaceH4/zephyr-7b-beta",
+            tokenizer_name="HuggingFaceH4/zephyr-7b-beta",
+            context_window=3900,
+            max_new_tokens=256,
+            model_kwargs={"quantization_config": quantization_config},
+            generate_kwargs={"temperature": 0.7, "top_k": 50, "top_p": 0.95},
+            messages_to_prompt=messages_to_prompt,
+            completion_to_prompt=completion_to_prompt,
+            device_map="auto",
+        )
+
+        response = llm.complete("What is the meaning of life?")
+        print(str(response))
+        ```
+    """
 
     model_name: str = Field(
         default=DEFAULT_HUGGINGFACE_MODEL,
         description=(
             "The model name to use from HuggingFace. "
             "Unused if `model` is passed in directly."
         ),
@@ -179,17 +256,17 @@
         if "max_length" not in tokenizer_kwargs:
             tokenizer_kwargs["max_length"] = context_window
 
         self._tokenizer = tokenizer or AutoTokenizer.from_pretrained(
             tokenizer_name, **tokenizer_kwargs
         )
 
-        if tokenizer_name != model_name:
+        if self._tokenizer.name_or_path != model_name:
             logger.warning(
-                f"The model `{model_name}` and tokenizer `{tokenizer_name}` "
+                f"The model `{model_name}` and tokenizer `{self._tokenizer.name_or_path}` "
                 f"are different, please ensure that they are compatible."
             )
 
         # setup stopping criteria
         stopping_ids_list = stopping_ids or []
 
         class StopOnTokens(StoppingCriteria):
@@ -603,7 +680,398 @@
     ) -> ChatResponseAsyncGen:
         raise NotImplementedError
 
     async def astream_complete(
         self, prompt: str, formatted: bool = False, **kwargs: Any
     ) -> CompletionResponseAsyncGen:
         raise NotImplementedError
+
+
+class TextGenerationInference(FunctionCallingLLM):
+    model_name: Optional[str] = Field(
+        default=None,
+        description=("The name of the model served at the TGI endpoint"),
+    )
+    temperature: float = Field(
+        default=DEFAULT_TEMPERATURE,
+        description=("The temperature to use for sampling."),
+        gte=0.0,
+        lte=1.0,
+    )
+    max_tokens: int = Field(
+        default=DEFAULT_NUM_OUTPUTS,
+        description=("The maximum number of tokens to generate."),
+        gt=0,
+    )
+    token: Union[str, bool, None] = Field(
+        default=None,
+        description=(
+            "Hugging Face token. Will default to the locally saved token. Pass "
+            "token=False if you don’t want to send your token to the server."
+        ),
+    )
+    timeout: float = Field(
+        default=120, description=("The timeout to use in seconds."), gte=0
+    )
+    max_retries: int = Field(
+        default=5, description=("The maximum number of API retries."), gte=0
+    )
+    headers: Optional[Dict[str, str]] = Field(
+        default=None,
+        description=(
+            "Additional headers to send to the server. By default only the"
+            " authorization headers are sent. Values in this dictionary"
+            " will override the default values."
+        ),
+    )
+    cookies: Optional[Dict[str, str]] = Field(
+        default=None, description=("Additional cookies to send to the server.")
+    )
+    seed: Optional[str] = Field(
+        default=None, description=("The random seed to use for sampling.")
+    )
+    additional_kwargs: Dict[str, Any] = Field(
+        default_factory=dict, description=("Additional kwargs for the TGI API.")
+    )
+
+    _sync_client: "TGIClient" = PrivateAttr()
+    _async_client: "TGIAsyncClient" = PrivateAttr()
+
+    context_window: int = Field(
+        default=DEFAULT_CONTEXT_WINDOW,
+        description=("Maximum input length in tokens returned from TGI endpoint"),
+    )
+    is_chat_model: bool = Field(
+        default=True,
+        description=(
+            LLMMetadata.__fields__["is_chat_model"].field_info.description
+            + " TGI makes use of chat templating,"
+            " function call is available only for '/v1/chat/completions' route"
+            " of TGI endpoint"
+        ),
+    )
+    is_function_calling_model: bool = Field(
+        default=False,
+        description=(
+            LLMMetadata.__fields__["is_function_calling_model"].field_info.description
+            + " 'text-generation-inference' supports function call"
+            " starting from v1.4.3"
+        ),
+    )
+
+    def __init__(
+        self,
+        model_url,
+        model_name: Optional[str] = None,
+        cookies: Optional[dict] = None,
+        temperature: float = DEFAULT_TEMPERATURE,
+        max_tokens: int = DEFAULT_NUM_OUTPUTS,
+        timeout: int = 120,
+        max_retries: int = 5,
+        seed: Optional[int] = None,
+        token: Optional[str] = None,
+        additional_kwargs: Optional[Dict[str, Any]] = None,
+        callback_manager: Optional[CallbackManager] = None,
+        system_prompt: Optional[str] = None,
+        messages_to_prompt: Optional[Callable[[Sequence[ChatMessage]], str]] = None,
+        completion_to_prompt: Optional[Callable[[str], str]] = None,
+        pydantic_program_mode: PydanticProgramMode = PydanticProgramMode.DEFAULT,
+        output_parser: Optional[BaseOutputParser] = None,
+    ) -> None:
+        additional_kwargs = additional_kwargs or {}
+        callback_manager = callback_manager or CallbackManager([])
+
+        token = get_from_param_or_env("token", token, "HF_TOKEN", "")
+
+        headers = {}
+        if token:
+            headers.update({"Authorization": f"Bearer {token}"})
+
+        self._sync_client = TGIClient(
+            base_url=model_url,
+            headers=headers,
+            cookies=cookies,
+            timeout=timeout,
+        )
+        self._async_client = TGIAsyncClient(
+            base_url=model_url,
+            headers=headers,
+            cookies=cookies,
+            timeout=timeout,
+        )
+
+        try:
+            is_function_calling_model = resolve_tgi_function_call(model_url)
+        except Exception as e:
+            logger.warning(f"TGI client has no function call support: {e}")
+            is_function_calling_model = False
+
+        context_window = get_max_input_length(model_url) or DEFAULT_CONTEXT_WINDOW
+
+        super().__init__(
+            context_window=context_window,
+            temperature=temperature,
+            max_tokens=max_tokens,
+            additional_kwargs=additional_kwargs,
+            timeout=timeout,
+            max_retries=max_retries,
+            seed=seed,
+            model=model_name,
+            is_function_calling_model=is_function_calling_model,
+            callback_manager=callback_manager,
+            system_prompt=system_prompt,
+            messages_to_prompt=messages_to_prompt,
+            completion_to_prompt=completion_to_prompt,
+            pydantic_program_mode=pydantic_program_mode,
+            output_parser=output_parser,
+        )
+
+    @classmethod
+    def class_name(cls) -> str:
+        return "TextGenerationInference"
+
+    @property
+    def metadata(self) -> LLMMetadata:
+        return LLMMetadata(
+            context_window=self.context_window,
+            num_output=self.max_tokens,
+            is_chat_model=True,
+            model_name=self.model_name,
+            random_seed=self.seed,
+            is_function_calling_model=self.is_function_calling_model,
+        )
+
+    @property
+    def _model_kwargs(self) -> Dict[str, Any]:
+        base_kwargs = {
+            "temperature": self.temperature,
+            "max_tokens": self.max_tokens,
+            "seed": self.seed,
+        }
+        return {
+            **base_kwargs,
+            **self.additional_kwargs,
+        }
+
+    def _get_all_kwargs(self, **kwargs: Any) -> Dict[str, Any]:
+        return {
+            **self._model_kwargs,
+            **kwargs,
+        }
+
+    @llm_chat_callback()
+    def chat(self, messages: Sequence[ChatMessage], **kwargs: Any) -> ChatResponse:
+        # convert to TGI Message
+        messages = to_tgi_messages(messages)
+        all_kwargs = self._get_all_kwargs(**kwargs)
+        response = self._sync_client.chat(messages=messages, **all_kwargs)
+        tool_calls = response.choices[0].message.tool_calls
+
+        return ChatResponse(
+            message=ChatMessage(
+                role=MessageRole.ASSISTANT,
+                content=response.choices[0].message.content,
+                additional_kwargs={"tool_calls": tool_calls}
+                if tool_calls is not None
+                else {},
+            ),
+            raw=dict(response),
+        )
+
+    @llm_completion_callback()
+    def complete(
+        self, prompt: str, formatted: bool = False, **kwargs: Any
+    ) -> CompletionResponse:
+        complete_fn = chat_to_completion_decorator(self.chat)
+        return complete_fn(prompt, **kwargs)
+
+    @llm_chat_callback()
+    def stream_chat(
+        self, messages: Sequence[ChatMessage], **kwargs: Any
+    ) -> ChatResponseGen:
+        # convert to TGI Message
+        messages = to_tgi_messages(messages)
+        all_kwargs = self._get_all_kwargs(**kwargs)
+        response = self._sync_client.chat(messages=messages, stream=True, **all_kwargs)
+
+        def generator() -> ChatResponseGen:
+            content = ""
+            role = MessageRole.ASSISTANT
+            for chunk in response:
+                content_delta = chunk.choices[0].delta.content
+                if content_delta is None:
+                    continue
+                content += content_delta
+                yield ChatResponse(
+                    message=ChatMessage(role=role, content=content),
+                    delta=content_delta,
+                    raw=chunk,
+                )
+
+        return generator()
+
+    @llm_completion_callback()
+    def stream_complete(
+        self, prompt: str, formatted: bool = False, **kwargs: Any
+    ) -> CompletionResponseGen:
+        stream_complete_fn = stream_chat_to_completion_decorator(self.stream_chat)
+        return stream_complete_fn(prompt, **kwargs)
+
+    @llm_chat_callback()
+    async def achat(
+        self, messages: Sequence[ChatMessage], **kwargs: Any
+    ) -> ChatResponse:
+        # convert to TGI Message
+        messages = to_tgi_messages(messages)
+        all_kwargs = self._get_all_kwargs(**kwargs)
+        response = await self._async_client.chat(messages=messages, **all_kwargs)
+        tool_calls = response.choices[0].message.tool_calls
+
+        return ChatResponse(
+            message=ChatMessage(
+                role=MessageRole.ASSISTANT,
+                content=response.choices[0].message.content,
+                additional_kwargs={"tool_calls": tool_calls}
+                if tool_calls is not None
+                else {},
+            ),
+            raw=dict(response),
+        )
+
+    @llm_completion_callback()
+    async def acomplete(
+        self, prompt: str, formatted: bool = False, **kwargs: Any
+    ) -> CompletionResponse:
+        acomplete_fn = achat_to_completion_decorator(self.achat)
+        return await acomplete_fn(prompt, **kwargs)
+
+    @llm_chat_callback()
+    async def astream_chat(
+        self, messages: Sequence[ChatMessage], **kwargs: Any
+    ) -> ChatResponseAsyncGen:
+        # convert to TGI Message
+        messages = to_tgi_messages(messages)
+        all_kwargs = self._get_all_kwargs(**kwargs)
+        response = await self._async_client.chat(
+            messages=messages, stream=True, **all_kwargs
+        )
+
+        async def generator() -> ChatResponseAsyncGen:
+            content = ""
+            role = MessageRole.ASSISTANT
+            async for chunk in response:
+                content_delta = chunk.choices[0].delta.content
+                if content_delta is None:
+                    continue
+                content += content_delta
+                yield ChatResponse(
+                    message=ChatMessage(role=role, content=content),
+                    delta=content_delta,
+                    raw=chunk,
+                )
+
+        return generator()
+
+    @llm_completion_callback()
+    async def astream_complete(
+        self, prompt: str, formatted: bool = False, **kwargs: Any
+    ) -> CompletionResponseAsyncGen:
+        astream_complete_fn = astream_chat_to_completion_decorator(self.astream_chat)
+        return await astream_complete_fn(prompt, **kwargs)
+
+    def chat_with_tools(
+        self,
+        tools: List["BaseTool"],
+        user_msg: Optional[Union[str, ChatMessage]] = None,
+        chat_history: Optional[List[ChatMessage]] = None,
+        verbose: bool = False,
+        allow_parallel_tool_calls: bool = False,
+        tool_choice: str = "auto",
+        **kwargs: Any,
+    ) -> ChatResponse:
+        """Predict and call the tool."""
+        # use openai tool format
+        tool_specs = [tool.metadata.to_openai_tool() for tool in tools]
+
+        if isinstance(user_msg, str):
+            user_msg = ChatMessage(role=MessageRole.USER, content=user_msg)
+
+        messages = chat_history or []
+        if user_msg:
+            messages.append(user_msg)
+
+        response = self.chat(
+            messages=messages,
+            tools=tool_specs,
+            tool_choice=resolve_tool_choice(tool_specs, tool_choice),
+            **kwargs,
+        )
+        if not allow_parallel_tool_calls:
+            force_single_tool_call(response)
+        return response
+
+    async def achat_with_tools(
+        self,
+        tools: List["BaseTool"],
+        user_msg: Optional[Union[str, ChatMessage]] = None,
+        chat_history: Optional[List[ChatMessage]] = None,
+        verbose: bool = False,
+        allow_parallel_tool_calls: bool = False,
+        tool_choice: str = "auto",
+        **kwargs: Any,
+    ) -> ChatResponse:
+        # use openai tool format
+        tool_specs = [tool.metadata.to_openai_tool() for tool in tools]
+
+        if isinstance(user_msg, str):
+            user_msg = ChatMessage(role=MessageRole.USER, content=user_msg)
+
+        messages = chat_history or []
+        if user_msg:
+            messages.append(user_msg)
+
+        response = self.achat(
+            messages=messages,
+            tools=tool_specs,
+            tool_choice=resolve_tool_choice(tool_specs, tool_choice),
+            **kwargs,
+        )
+        if not allow_parallel_tool_calls:
+            force_single_tool_call(response)
+        return response
+
+    def get_tool_calls_from_response(
+        self,
+        response: "AgentChatResponse",
+        error_on_no_tool_call: bool = True,
+    ) -> List[ToolSelection]:
+        """Predict and call the tool."""
+        tool_calls = response.message.additional_kwargs.get("tool_calls", [])
+
+        if len(tool_calls) < 1:
+            if error_on_no_tool_call:
+                raise ValueError(
+                    f"Expected at least one tool call, but got {len(tool_calls)} tool calls."
+                )
+            else:
+                return []
+
+        tool_selections = []
+        for tool_call in tool_calls:
+            # TODO Add typecheck with ToolCall from TGI once the client is updated
+            if tool_call and (tc_type := tool_call["type"]) != "function":
+                raise ValueError(
+                    f"Invalid tool type: got {tc_type}, expect 'function'."
+                )
+            argument_dict = tool_call["function"]["parameters"]
+
+            tool_selections.append(
+                ToolSelection(
+                    tool_id=tool_call["id"],
+                    tool_name=tool_call["function"][
+                        "name"
+                    ],  # NOTE for now the tool_name is hardcoded 'tools' in TGI
+                    tool_kwargs=argument_dict,
+                )
+            )
+
+        return tool_selections
```

### Comparing `llama_index_llms_huggingface-0.1.4/pyproject.toml` & `llama_index_llms_huggingface-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,21 +24,22 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms huggingface integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-huggingface"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 huggingface-hub = "^0.20.3"
 torch = "^2.1.2"
+text-generation = "^0.7.0"
 
 [tool.poetry.dependencies.transformers]
 extras = ["torch"]
 version = "^4.37.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

### Comparing `llama_index_llms_huggingface-0.1.4/PKG-INFO` & `llama_index_llms_huggingface-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-huggingface
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index llms huggingface integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: huggingface-hub (>=0.20.3,<0.21.0)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
+Requires-Dist: text-generation (>=0.7.0,<0.8.0)
 Requires-Dist: torch (>=2.1.2,<3.0.0)
 Requires-Dist: transformers[torch] (>=4.37.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: Huggingface
```

