# Comparing `tmp/notdiamond-0.1.8b0.tar.gz` & `tmp/notdiamond-0.1.9b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notdiamond-0.1.8b0.tar", max compression
+gzip compressed data, was "notdiamond-0.1.9b0.tar", max compression
```

## Comparing `notdiamond-0.1.8b0.tar` & `notdiamond-0.1.9b0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     5862 2024-04-22 18:39:28.549020 notdiamond-0.1.8b0/README.md
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.001993 notdiamond-0.1.8b0/notdiamond/__init__.py
--rw-r--r--   0        0        0      831 2024-04-22 18:35:58.307978 notdiamond-0.1.8b0/notdiamond/callbacks.py
--rw-r--r--   0        0        0      440 2024-04-02 07:43:11.002696 notdiamond-0.1.8b0/notdiamond/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.002740 notdiamond-0.1.8b0/notdiamond/llms/__init__.py
--rw-r--r--   0        0        0    39317 2024-04-23 19:46:16.870797 notdiamond-0.1.8b0/notdiamond/llms/llm.py
--rw-r--r--   0        0        0     4432 2024-04-13 12:29:10.520716 notdiamond-0.1.8b0/notdiamond/llms/provider.py
--rw-r--r--   0        0        0     3638 2024-04-16 07:39:04.865174 notdiamond-0.1.8b0/notdiamond/llms/providers.py
--rw-r--r--   0        0        0    10648 2024-04-19 07:58:41.324295 notdiamond-0.1.8b0/notdiamond/llms/request.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004168 notdiamond-0.1.8b0/notdiamond/metrics/__init__.py
--rw-r--r--   0        0        0     1155 2024-04-02 11:25:39.891484 notdiamond-0.1.8b0/notdiamond/metrics/metric.py
--rw-r--r--   0        0        0     1100 2024-04-06 09:04:10.351693 notdiamond-0.1.8b0/notdiamond/metrics/request.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004898 notdiamond-0.1.8b0/notdiamond/prompts/__init__.py
--rw-r--r--   0        0        0      147 2024-04-02 07:43:11.005796 notdiamond-0.1.8b0/notdiamond/prompts/hash.py
--rw-r--r--   0        0        0     5760 2024-04-23 15:21:39.834968 notdiamond-0.1.8b0/notdiamond/prompts/prompt.py
--rw-r--r--   0        0        0     1933 2024-04-16 07:39:04.865490 notdiamond-0.1.8b0/notdiamond/settings.py
--rw-r--r--   0        0        0      972 2024-04-02 07:43:11.007948 notdiamond-0.1.8b0/notdiamond/types.py
--rw-r--r--   0        0        0     1458 2024-04-23 19:46:02.544585 notdiamond-0.1.8b0/pyproject.toml
--rw-r--r--   0        0        0     6974 1970-01-01 00:00:00.000000 notdiamond-0.1.8b0/PKG-INFO
+-rw-r--r--   0        0        0     5862 2024-04-22 18:39:28.549020 notdiamond-0.1.9b0/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.001993 notdiamond-0.1.9b0/notdiamond/__init__.py
+-rw-r--r--   0        0        0      831 2024-04-22 18:35:58.307978 notdiamond-0.1.9b0/notdiamond/callbacks.py
+-rw-r--r--   0        0        0      440 2024-04-02 07:43:11.002696 notdiamond-0.1.9b0/notdiamond/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.002740 notdiamond-0.1.9b0/notdiamond/llms/__init__.py
+-rw-r--r--   0        0        0    39818 2024-04-26 15:44:03.491985 notdiamond-0.1.9b0/notdiamond/llms/llm.py
+-rw-r--r--   0        0        0     4432 2024-04-13 12:29:10.520716 notdiamond-0.1.9b0/notdiamond/llms/provider.py
+-rw-r--r--   0        0        0     3638 2024-04-16 07:39:04.865174 notdiamond-0.1.9b0/notdiamond/llms/providers.py
+-rw-r--r--   0        0        0    11705 2024-04-26 15:44:03.492337 notdiamond-0.1.9b0/notdiamond/llms/request.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004168 notdiamond-0.1.9b0/notdiamond/metrics/__init__.py
+-rw-r--r--   0        0        0     1155 2024-04-02 11:25:39.891484 notdiamond-0.1.9b0/notdiamond/metrics/metric.py
+-rw-r--r--   0        0        0     1100 2024-04-06 09:04:10.351693 notdiamond-0.1.9b0/notdiamond/metrics/request.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004898 notdiamond-0.1.9b0/notdiamond/prompts/__init__.py
+-rw-r--r--   0        0        0      147 2024-04-02 07:43:11.005796 notdiamond-0.1.9b0/notdiamond/prompts/hash.py
+-rw-r--r--   0        0        0     6415 2024-04-26 15:44:03.492739 notdiamond-0.1.9b0/notdiamond/prompts/prompt.py
+-rw-r--r--   0        0        0     2482 2024-04-26 15:44:03.493687 notdiamond-0.1.9b0/notdiamond/settings.py
+-rw-r--r--   0        0        0      972 2024-04-02 07:43:11.007948 notdiamond-0.1.9b0/notdiamond/types.py
+-rw-r--r--   0        0        0     1580 2024-04-26 15:48:16.880555 notdiamond-0.1.9b0/pyproject.toml
+-rw-r--r--   0        0        0     6974 1970-01-01 00:00:00.000000 notdiamond-0.1.9b0/PKG-INFO
```

### Comparing `notdiamond-0.1.8b0/README.md` & `notdiamond-0.1.9b0/README.md`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.8b0/notdiamond/callbacks.py` & `notdiamond-0.1.9b0/notdiamond/callbacks.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.8b0/notdiamond/llms/llm.py` & `notdiamond-0.1.9b0/notdiamond/llms/llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,14 +277,15 @@
             prompt_template=prompt_template,
             llm_providers=self.llm_providers,
             metric=metric,
             notdiamond_api_key=self.api_key,
             max_model_depth=self.max_model_depth,
             preference_weights=self.preference_weights,
             preference_id=self.preference_id,
+            tools=self.tools,
         )
 
         is_default = False
         if not best_llm:
             best_llm = self.default_llm_provider
             is_default = True
 
@@ -421,14 +422,15 @@
             prompt_template=prompt_template,
             llm_providers=self.llm_providers,
             metric=metric,
             notdiamond_api_key=self.api_key,
             max_model_depth=self.max_model_depth,
             preference_weights=self.preference_weights,
             preference_id=self.preference_id,
+            tools=self.tools,
         )
 
         is_default = False
         if not best_llm:
             best_llm = self.default_llm_provider
             is_default = True
 
@@ -566,14 +568,15 @@
             prompt_template=prompt_template,
             llm_providers=self.llm_providers,
             metric=metric,
             notdiamond_api_key=self.api_key,
             max_model_depth=self.max_model_depth,
             preference_weights=self.preference_weights,
             preference_id=self.preference_id,
+            tools=self.tools,
         )
 
         if not best_llm:
             best_llm = self.default_llm_provider
 
             if best_llm is None:
                 error_message = (
@@ -636,14 +639,15 @@
             prompt_template=prompt_template,
             llm_providers=self.llm_providers,
             metric=metric,
             notdiamond_api_key=self.api_key,
             max_model_depth=self.max_model_depth,
             preference_weights=self.preference_weights,
             preference_id=self.preference_id,
+            tools=self.tools,
         )
 
         if input is None:
             input = {}
 
         prompt_template.partial_variables = {
             **prompt_template.partial_variables,
@@ -720,14 +724,15 @@
             prompt_template=prompt_template,
             llm_providers=self.llm_providers,
             metric=metric,
             notdiamond_api_key=self.api_key,
             max_model_depth=self.max_model_depth,
             preference_weights=self.preference_weights,
             preference_id=self.preference_id,
+            tools=self.tools,
         )
 
         if not best_llm and self.default is not None:
             print("ND API error. Falling back to default provider.")
             best_llm = self.default_llm_provider
         self.call_callbacks("on_model_select", best_llm, best_llm.model)
 
@@ -783,14 +788,15 @@
             prompt_template=prompt_template,
             llm_providers=self.llm_providers,
             metric=metric,
             notdiamond_api_key=self.api_key,
             max_model_depth=self.max_model_depth,
             preference_weights=self.preference_weights,
             preference_id=self.preference_id,
+            tools=self.tools,
         )
 
         if not best_llm and self.default is not None:
             print("ND API error. Falling back to default provider.")
             best_llm = self.default_llm_provider
         self.call_callbacks("on_model_select", best_llm, best_llm.model)
 
@@ -983,14 +989,22 @@
         tools: Sequence[Union[Dict[str, Any], Callable]],
     ) -> "NDLLM":
         """
         Bind tools to the LLM object. The tools will be passed to the LLM object when invoking it.
         Results in the tools being available in the LLM object.
         You can access the tool_calls in the result via `result.tool_calls`.
         """
+
+        for provider in self.llm_providers:
+            if provider.model not in settings.PROVIDERS[provider.provider].get(
+                "support_tools", []
+            ):
+                raise ApiError(
+                    f"{provider.provider}/{provider.model} does not support function calling."
+                )
         self.tools = tools
 
         return self
 
     def call_callbacks(self, function_name: str, *args, **kwargs) -> None:
         """
         Call all callbacks with a specific function name.
```

### Comparing `notdiamond-0.1.8b0/notdiamond/llms/provider.py` & `notdiamond-0.1.9b0/notdiamond/llms/provider.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.8b0/notdiamond/llms/providers.py` & `notdiamond-0.1.9b0/notdiamond/llms/providers.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.8b0/notdiamond/llms/request.py` & `notdiamond-0.1.9b0/notdiamond/llms/request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
-from typing import Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Union
 
 import aiohttp
 import requests
+from langchain_core.utils.function_calling import convert_to_openai_function
 
 from notdiamond import settings
 from notdiamond.llms.provider import NDLLMProvider
 from notdiamond.metrics.metric import NDMetric
 from notdiamond.prompts.prompt import NDChatPromptTemplate, NDPromptTemplate
 from notdiamond.types import ModelSelectRequestPayload
 
@@ -15,14 +16,15 @@
     prompt_template: Optional[Union[NDPromptTemplate, NDChatPromptTemplate]],
     llm_providers: List[NDLLMProvider],
     metric: NDMetric,
     notdiamond_api_key: str,
     max_model_depth: int,
     preference_weights: Optional[Dict[str, float]] = None,
     preference_id: Optional[str] = None,
+    tools: Optional[Sequence[Union[Dict[str, Any], Callable]]] = [],
 ):
     """
     This is the core method for the model_select endpoint.
     It returns the best fitting LLM to call and a session ID that can be used for feedback.
 
     Parameters:
         prompt_template (Optional[Union[NDPromptTemplate, NDChatPromptTemplate]]): prompt template for the LLM call
@@ -37,39 +39,61 @@
         async_mode (bool, optional): whether to run the request in async mode. Defaults to False.
 
     Returns:
         tuple(url, payload, headers): returns data to be used for the API call of modelSelect
     """
 
     url = f"{settings.ND_BASE_URL}/v2/optimizer/modelSelect"
+    tools_dict = get_tools_in_openai_format(tools)
 
     payload: ModelSelectRequestPayload = {
         "messages": prompt_template.prepare_for_request(),
-        "hash_digest": prompt_template.get_hash_digest(),
+        "hash_digest": prompt_template.get_hash_digest(tools_dict),
         "llm_providers": [
             llm_provider.prepare_for_request()
             for llm_provider in llm_providers
         ],
         "metric": metric.metric,
         "max_model_depth": max_model_depth,
     }
 
+    if tools_dict:
+        payload["tools"] = tools_dict
     if preference_weights is not None:
         payload["preference_weights"] = preference_weights
     if preference_id is not None:
         payload["preference_id"] = preference_id
 
     headers = {
         "Content-Type": "application/json",
         "Authorization": f"Bearer {notdiamond_api_key}",
     }
 
     return url, payload, headers
 
 
+def get_tools_in_openai_format(
+    tools: Optional[Sequence[Union[Dict[str, Any], Callable]]]
+):
+    """
+    This function converts the tools list into the format that OpenAI expects.
+    Does this by using langchains Model that automatically creates the dictionary on bind_tools
+
+    Parameters:
+        tools (Optional[Sequence[Union[Dict[str, Any], Callable]]]): list of tools to be converted
+
+    Returns:
+        dict: dictionary of tools in the format that OpenAI expects
+    """
+    if tools:
+        return [convert_to_openai_function(tool) for tool in tools]
+
+    return None
+
+
 def model_select_parse(response_code, response_json, llm_providers):
     if response_code == 200:
         providers = response_json["providers"]
         session_id = response_json["session_id"]
 
         # TODO: make use of full providers list in the future and rest of params returned
         top_provider = providers[0]
@@ -95,14 +119,15 @@
     prompt_template: Optional[Union[NDPromptTemplate, NDChatPromptTemplate]],
     llm_providers: List[NDLLMProvider],
     metric: NDMetric,
     notdiamond_api_key: str,
     max_model_depth: int,
     preference_weights: Optional[Dict[str, float]] = None,
     preference_id: Optional[str] = None,
+    tools: Optional[Sequence[Union[Dict[str, Any], Callable]]] = [],
 ):
     """
     This endpoint receives the prompt and routing settings, and makes a call to the NotDiamond API.
     It returns the best fitting LLM to call and a session ID that can be used for feedback.
 
     Parameters:
         prompt_template (Optional[Union[NDPromptTemplate, NDChatPromptTemplate]]): prompt template for the LLM call
@@ -124,14 +149,15 @@
         prompt_template=prompt_template,
         llm_providers=llm_providers,
         metric=metric,
         notdiamond_api_key=notdiamond_api_key,
         max_model_depth=max_model_depth,
         preference_weights=preference_weights,
         preference_id=preference_id,
+        tools=tools,
     )
 
     try:
         response = requests.post(
             url, data=json.dumps(payload), headers=headers
         )
         response_code = response.status_code
@@ -151,14 +177,15 @@
     prompt_template: Optional[Union[NDPromptTemplate, NDChatPromptTemplate]],
     llm_providers: List[NDLLMProvider],
     metric: NDMetric,
     notdiamond_api_key: str,
     max_model_depth: int,
     preference_weights: Optional[Dict[str, float]] = None,
     preference_id: Optional[str] = None,
+    tools: Optional[Sequence[Union[Dict[str, Any], Callable]]] = [],
 ):
     """
     This endpoint receives the prompt and routing settings, and makes a call to the NotDiamond API.
     It returns the best fitting LLM to call and a session ID that can be used for feedback.
 
     Parameters:
         prompt_template (Optional[Union[NDPromptTemplate, NDChatPromptTemplate]]): prompt template for the LLM call
@@ -180,14 +207,15 @@
         prompt_template=prompt_template,
         llm_providers=llm_providers,
         metric=metric,
         notdiamond_api_key=notdiamond_api_key,
         max_model_depth=max_model_depth,
         preference_weights=preference_weights,
         preference_id=preference_id,
+        tools=tools,
     )
 
     try:
         async with aiohttp.ClientSession() as session:
             async with session.post(
                 url, data=json.dumps(payload), headers=headers
             ) as response:
```

### Comparing `notdiamond-0.1.8b0/notdiamond/metrics/metric.py` & `notdiamond-0.1.9b0/notdiamond/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.8b0/notdiamond/metrics/request.py` & `notdiamond-0.1.9b0/notdiamond/metrics/request.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.8b0/notdiamond/prompts/prompt.py` & `notdiamond-0.1.9b0/notdiamond/prompts/prompt.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from typing import Any, Dict, List, Optional, Union
 
 from langchain.prompts import PromptTemplate
 from langchain_core.messages import AIMessage, HumanMessage, SystemMessage
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.prompts.string import get_template_variables
 
@@ -48,16 +49,24 @@
         print("Not yet implemented!")
 
     def prepare_for_request(self):
         messages = [{"role": "user", "content": nd_hash(self.format())}]
 
         return messages
 
-    def get_hash_digest(self):
-        return self.prepare_for_request()[0]["content"]
+    def get_hash_digest(self, tools_dict: Dict[str, Any] = None) -> str:
+        current_prompt = self.format()
+        if tools_dict:
+            functions = json.dumps(tools_dict)
+            hash_digest_with_tools = f"""
+    {current_prompt}\nHere is a list of functions in JSON format that you can invoke:\n{functions}.
+"""
+            return nd_hash(hash_digest_with_tools)
+
+        return nd_hash(current_prompt)
 
 
 class NDChatPromptTemplate(ChatPromptTemplate):
     """
     Starting reference is from
     here:https://api.python.langchain.com/en/latest/prompts/langchain_core.prompts.chat.ChatPromptTemplate.html
     """
@@ -153,16 +162,23 @@
                         "role": self.get_role_of_message(message),
                         "content": nd_hash(message.content),
                     }
                 )
 
         return messages
 
-    def get_hash_digest(self):
+    def get_hash_digest(self, tools_dict: Dict[str, Any] = None) -> str:
         formated_messages = self.format_messages(**self.partial_variables)
         message_to_hash = ""
         if isinstance(formated_messages[0], SystemMessage):
             message_to_hash += formated_messages[0].content + "\n"
 
         message_to_hash += self.get_last_human_message(formated_messages)
 
+        if tools_dict:
+            functions = json.dumps(tools_dict)
+            hash_digest_with_tools = f"""
+    {message_to_hash}\nHere is a list of functions in JSON format that you can invoke:\n{functions}.
+"""
+            return nd_hash(hash_digest_with_tools)
+
         return nd_hash(message_to_hash)
```

### Comparing `notdiamond-0.1.8b0/notdiamond/types.py` & `notdiamond-0.1.9b0/notdiamond/types.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.8b0/pyproject.toml` & `notdiamond-0.1.9b0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notdiamond"
-version = "0.1.8-beta"
+version = "0.1.9-beta"
 description = "Not Diamond Python Library"
 authors = ["Not Diamond <t5@notdiamond.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 langchain = ">=0.1.16"
@@ -32,14 +32,21 @@
 pre-commit = "^3.7.0"
 black = "^24.3.0"
 flake8 = "^7.0.0"
 poetry-pre-commit-plugin = "^0.1.2"
 isort = "^5.13.2"
 nox = "^2024.3.2"
 
+
+[tool.poetry.group.docs.dependencies]
+sphinx = "^7.3.7"
+autodoc = "^0.5.0"
+sphinx-rtd-theme = "^2.0.0"
+toml = "^0.10.2"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 markers = ["longrun"]
```

### Comparing `notdiamond-0.1.8b0/PKG-INFO` & `notdiamond-0.1.9b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notdiamond
-Version: 0.1.8b0
+Version: 0.1.9b0
 Summary: Not Diamond Python Library
 Author: Not Diamond
 Author-email: t5@notdiamond.ai
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

