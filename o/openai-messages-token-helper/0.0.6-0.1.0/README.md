# Comparing `tmp/openai_messages_token_helper-0.0.6.tar.gz` & `tmp/openai_messages_token_helper-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_messages_token_helper-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "openai_messages_token_helper-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `openai_messages_token_helper-0.0.6.tar` & `openai_messages_token_helper-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
--rw-r--r--   0        0        0      880 2024-04-06 22:31:15.975017 openai_messages_token_helper-0.0.6/.github/workflows/python.yaml
--rw-r--r--   0        0        0     1799 2024-04-04 18:34:36.837611 openai_messages_token_helper-0.0.6/.gitignore
--rw-r--r--   0        0        0      359 2024-04-21 22:10:10.818591 openai_messages_token_helper-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      148 2024-04-21 22:10:10.823452 openai_messages_token_helper-0.0.6/.vscode/settings.json
--rw-r--r--   0        0        0     1084 2024-04-24 16:31:07.612115 openai_messages_token_helper-0.0.6/CHANGELOG.md
--rw-r--r--   0        0        0      311 2024-04-24 16:19:50.746331 openai_messages_token_helper-0.0.6/CONTRIBUTING.md
--rw-r--r--   0        0        0     1078 2024-04-04 18:34:36.838438 openai_messages_token_helper-0.0.6/LICENSE
--rw-r--r--   0        0        0     3988 2024-04-24 16:29:51.563626 openai_messages_token_helper-0.0.6/README.md
--rw-r--r--   0        0        0     1314 2024-04-24 16:29:58.431785 openai_messages_token_helper-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      265 2024-04-24 15:10:08.288991 openai_messages_token_helper-0.0.6/src/openai_messages_token_helper/__init__.py
--rw-r--r--   0        0        0     2020 2024-04-24 15:10:08.289382 openai_messages_token_helper-0.0.6/src/openai_messages_token_helper/images_helper.py
--rw-r--r--   0        0        0     5183 2024-04-24 16:42:24.003445 openai_messages_token_helper-0.0.6/src/openai_messages_token_helper/message_builder.py
--rw-r--r--   0        0        0     3784 2024-04-24 15:10:08.292471 openai_messages_token_helper-0.0.6/src/openai_messages_token_helper/model_helper.py
--rw-r--r--   0        0        0        0 2024-04-21 22:10:10.833586 openai_messages_token_helper-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 18:34:36.839523 openai_messages_token_helper-0.0.6/tests/conftest.py
--rw-r--r--   0        0        0   317320 2024-04-04 19:36:32.913476 openai_messages_token_helper-0.0.6/tests/image_large.png
--rw-r--r--   0        0        0     1448 2024-04-21 22:10:10.836640 openai_messages_token_helper-0.0.6/tests/messages.py
--rw-r--r--   0        0        0     1105 2024-04-24 15:10:08.294738 openai_messages_token_helper-0.0.6/tests/test_imageshelper.py
--rw-r--r--   0        0        0     2599 2024-04-24 16:42:24.001504 openai_messages_token_helper-0.0.6/tests/test_messagebuilder.py
--rw-r--r--   0        0        0     2782 2024-04-24 15:10:08.300364 openai_messages_token_helper-0.0.6/tests/test_modelhelper.py
--rw-r--r--   0        0        0     1604 2024-04-21 22:10:10.850735 openai_messages_token_helper-0.0.6/tests/verify_openai.py
--rw-r--r--   0        0        0     5072 1970-01-01 00:00:00.000000 openai_messages_token_helper-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      913 2024-05-02 08:43:27.095494 openai_messages_token_helper-0.1.0/.github/workflows/python.yaml
+-rw-r--r--   0        0        0     1799 2024-04-04 18:34:36.837611 openai_messages_token_helper-0.1.0/.gitignore
+-rw-r--r--   0        0        0      359 2024-04-21 22:10:10.818591 openai_messages_token_helper-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      536 2024-05-02 08:43:27.099990 openai_messages_token_helper-0.1.0/.vscode/launch.json
+-rw-r--r--   0        0        0      148 2024-04-21 22:10:10.823452 openai_messages_token_helper-0.1.0/.vscode/settings.json
+-rw-r--r--   0        0        0     1517 2024-05-02 08:44:48.896748 openai_messages_token_helper-0.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0      311 2024-04-24 16:19:50.746331 openai_messages_token_helper-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1078 2024-04-04 18:34:36.838438 openai_messages_token_helper-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4481 2024-05-02 08:43:27.104337 openai_messages_token_helper-0.1.0/README.md
+-rw-r--r--   0        0        0     1314 2024-05-02 08:43:27.107170 openai_messages_token_helper-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      360 2024-05-02 08:43:27.109262 openai_messages_token_helper-0.1.0/src/openai_messages_token_helper/__init__.py
+-rw-r--r--   0        0        0     2423 2024-05-02 08:43:27.112777 openai_messages_token_helper-0.1.0/src/openai_messages_token_helper/function_format.py
+-rw-r--r--   0        0        0     2020 2024-04-24 15:10:08.289382 openai_messages_token_helper-0.1.0/src/openai_messages_token_helper/images_helper.py
+-rw-r--r--   0        0        0     5561 2024-05-02 08:43:27.115625 openai_messages_token_helper-0.1.0/src/openai_messages_token_helper/message_builder.py
+-rw-r--r--   0        0        0     6309 2024-05-02 08:43:27.117979 openai_messages_token_helper-0.1.0/src/openai_messages_token_helper/model_helper.py
+-rw-r--r--   0        0        0        0 2024-04-21 22:10:10.833586 openai_messages_token_helper-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:34:36.839523 openai_messages_token_helper-0.1.0/tests/conftest.py
+-rw-r--r--   0        0        0    16187 2024-05-02 08:43:27.120583 openai_messages_token_helper-0.1.0/tests/functions.py
+-rw-r--r--   0        0        0   317320 2024-04-04 19:36:32.913476 openai_messages_token_helper-0.1.0/tests/image_large.png
+-rw-r--r--   0        0        0     4034 2024-05-02 08:43:27.123570 openai_messages_token_helper-0.1.0/tests/messages.py
+-rw-r--r--   0        0        0     1105 2024-04-26 13:30:53.397027 openai_messages_token_helper-0.1.0/tests/test_imageshelper.py
+-rw-r--r--   0        0        0     8562 2024-05-02 08:43:27.127154 openai_messages_token_helper-0.1.0/tests/test_messagebuilder.py
+-rw-r--r--   0        0        0     3499 2024-05-02 08:43:27.130210 openai_messages_token_helper-0.1.0/tests/test_modelhelper.py
+-rw-r--r--   0        0        0     1361 2024-05-02 08:43:27.134289 openai_messages_token_helper-0.1.0/tests/verify_functions.py
+-rw-r--r--   0        0        0     1274 2024-05-02 08:43:27.136603 openai_messages_token_helper-0.1.0/tests/verify_openai.py
+-rw-r--r--   0        0        0     5565 1970-01-01 00:00:00.000000 openai_messages_token_helper-0.1.0/PKG-INFO
```

### Comparing `openai_messages_token_helper-0.0.6/.github/workflows/python.yaml` & `openai_messages_token_helper-0.1.0/.github/workflows/python.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -26,8 +26,8 @@
             python3 -m pip install -e '.[dev]'
         - name: Lint with ruff
           run: ruff .
         - name: Check formatting with black
           run: black . --check --verbose
         - name: Run unit tests
           run: |
-            python3 -m pytest
+            python3 -m pytest -s -vv --cov --cov-fail-under=99
```

### Comparing `openai_messages_token_helper-0.0.6/.gitignore` & `openai_messages_token_helper-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.0.6/CHANGELOG.md` & `openai_messages_token_helper-0.1.0/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.1.0] - May 2, 2024
+
+- Add `count_tokens_for_system_and_tools` to count tokens for system message and tools. You should count the tokens for both together, since the token count for tools varies based off whether a system message is provided.
+- Updated `build_messages` to allow for `tools` and `tool_choice` to be passed in.
+- Breaking change: Changed `new_user_message` to `new_user_content` in `build_messages` for clarity.
+
 ## [0.0.6] - April 24, 2024
 
 - Add keyword argument `fallback_to_default` to `build_messages` function to allow for defaulting to the CL100k token encoder and minimum GPT token limit if the model is not found.
 - Fixed usage of `past_messages` argument of `build_messages` to not skip the last past message. (New user message should *not* be passed in)
 
 ## [0.0.5] - April 24, 2024
```

### Comparing `openai_messages_token_helper-0.0.6/LICENSE` & `openai_messages_token_helper-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.0.6/README.md` & `openai_messages_token_helper-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -27,33 +27,36 @@
 and past messages. The function will truncate the history of past messages if necessary to
 stay within the token limit.
 
 Arguments:
 
 * `model` (`str`): The model name to use for token calculation, like gpt-3.5-turbo.
 * `system_prompt` (`str`): The initial system prompt message.
-* `new_user_message` (`str | List[openai.types.chat.ChatCompletionContentPartParam]`): The new user message to append.
-* `past_messages` (`list[dict]`): The list of past messages in the conversation.
-* `few_shots` (`list[dict]`): A few-shot list of messages to insert after the system prompt.
-* `max_tokens` (`int`): The maximum number of tokens allowed for the conversation.
-* `fallback_to_default` (`bool`): Whether to fallback to default model/token limits if model is not found. Defaults to `False`.
+* `tools` (`List[openai.types.chat.ChatCompletionToolParam]`): (Optional) The tools that will be used in the conversation. These won't be part of the final returned messages, but they will be used to calculate the token count.
+* `tool_choice` (`str | dict`): (Optional) The tool choice that will be used in the conversation. This won't be part of the final returned messages, but it will be used to calculate the token count.
+* `new_user_content` (`str | List[openai.types.chat.ChatCompletionContentPartParam]`): (Optional) The content of new user message to append.
+* `past_messages` (`list[dict]`): (Optional) The list of past messages in the conversation.
+* `few_shots` (`list[dict]`): (Optional) A few-shot list of messages to insert after the system prompt.
+* `max_tokens` (`int`): (Optional) The maximum number of tokens allowed for the conversation.
+* `fallback_to_default` (`bool`): (Optional) Whether to fallback to default model/token limits if model is not found. Defaults to `False`.
+
 
 Returns:
 
 * `list[openai.types.chat.ChatCompletionMessageParam]`
 
 Example:
 
 ```python
 from openai_messages_token_helper import build_messages
 
 messages = build_messages(
     model="gpt-35-turbo",
     system_prompt="You are a bot.",
-    new_user_message="That wasn't a good poem.",
+    new_user_content="That wasn't a good poem.",
     past_messages=[
         {
             "role": "user",
             "content": "Write me a poem",
         },
         {
             "role": "assistant",
```

### Comparing `openai_messages_token_helper-0.0.6/pyproject.toml` & `openai_messages_token_helper-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "openai-messages-token-helper"
 description = "A helper library for estimating tokens used by messages sent through OpenAI Chat Completions API."
-version = "0.0.6"
+version = "0.1.0"
 authors = [{name = "Pamela Fox"}]
 requires-python = ">=3.9"
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = [
     "openai",
     "tiktoken",
```

### Comparing `openai_messages_token_helper-0.0.6/src/openai_messages_token_helper/images_helper.py` & `openai_messages_token_helper-0.1.0/src/openai_messages_token_helper/images_helper.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.0.6/src/openai_messages_token_helper/message_builder.py` & `openai_messages_token_helper-0.1.0/src/openai_messages_token_helper/message_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,101 +6,108 @@
     ChatCompletionAssistantMessageParam,
     ChatCompletionContentPartParam,
     ChatCompletionMessageParam,
     ChatCompletionSystemMessageParam,
     ChatCompletionUserMessageParam,
 )
 
-from .model_helper import count_tokens_for_message, get_token_limit
+from .model_helper import count_tokens_for_message, count_tokens_for_system_and_tools, get_token_limit
 
 
-class MessageBuilder:
+def normalize_content(content: Union[str, list[ChatCompletionContentPartParam]]):
+    if isinstance(content, str):
+        return unicodedata.normalize("NFC", content)
+    elif isinstance(content, list):
+        for part in content:
+            if "image_url" not in part:
+                part["text"] = unicodedata.normalize("NFC", part["text"])
+        return content
+
+
+class _MessageBuilder:
     """
     A class for building and managing messages in a chat conversation.
     Attributes:
         message (list): A list of dictionaries representing chat messages.
         model (str): The name of the ChatGPT model.
         token_count (int): The total number of tokens in the conversation.
     Methods:
         __init__(self, system_content: str, chatgpt_model: str): Initializes the MessageBuilder instance.
         insert_message(self, role: str, content: str, index: int = 1): Inserts a new message to the conversation.
     """
 
-    def __init__(self, system_content: str, chatgpt_model: str):
+    def __init__(self, system_content: str):
         self.messages: list[ChatCompletionMessageParam] = [
-            ChatCompletionSystemMessageParam(role="system", content=unicodedata.normalize("NFC", system_content))
+            ChatCompletionSystemMessageParam(role="system", content=normalize_content(system_content))
         ]
-        self.model = chatgpt_model
 
     def insert_message(self, role: str, content: Union[str, list[ChatCompletionContentPartParam]], index: int = 1):
         """
         Inserts a message into the conversation at the specified index,
         or at index 1 (after system message) if no index is specified.
         Args:
             role (str): The role of the message sender (either "user", "system", or "assistant").
             content (str | List[ChatCompletionContentPartParam]): The content of the message.
             index (int): The index at which to insert the message.
         """
         message: ChatCompletionMessageParam
         if role == "user":
-            message = ChatCompletionUserMessageParam(role="user", content=self.normalize_content(content))
+            message = ChatCompletionUserMessageParam(role="user", content=normalize_content(content))
         elif role == "assistant" and isinstance(content, str):
-            message = ChatCompletionAssistantMessageParam(
-                role="assistant", content=unicodedata.normalize("NFC", content)
-            )
+            message = ChatCompletionAssistantMessageParam(role="assistant", content=normalize_content(content))
         else:
             raise ValueError(f"Invalid role: {role}")
         self.messages.insert(index, message)
 
-    def normalize_content(self, content: Union[str, list[ChatCompletionContentPartParam]]):
-        if isinstance(content, str):
-            return unicodedata.normalize("NFC", content)
-        elif isinstance(content, list):
-            for part in content:
-                if "image_url" not in part:
-                    part["text"] = unicodedata.normalize("NFC", part["text"])
-            return content
-
 
 def build_messages(
     model: str,
     system_prompt: str,
-    new_user_message: Union[str, list[ChatCompletionContentPartParam], None] = None,  # list is for GPT4v usage
+    *,
+    tools: Optional[list[dict[str, dict]]] = None,
+    tool_choice: Optional[Union[str, dict]] = None,
+    new_user_content: Union[str, list[ChatCompletionContentPartParam], None] = None,  # list is for GPT4v usage
     past_messages: list[dict[str, str]] = [],  # *not* including system prompt
     few_shots=[],  # will always be inserted after system prompt
     max_tokens: Optional[int] = None,
     fallback_to_default: bool = False,
 ) -> list[ChatCompletionMessageParam]:
     """
     Build a list of messages for a chat conversation, given the system prompt, new user message,
     and past messages. The function will truncate the history of past messages if necessary to
     stay within the token limit.
     Args:
         model (str): The model name to use for token calculation, like gpt-3.5-turbo.
         system_prompt (str): The initial system prompt message.
-        new_user_message (str | List[ChatCompletionContentPartParam]): The new user message to append.
+        tools (list[dict]): A list of tools to include in the conversation.
+        tool_choice (str | dict): The tool to use in the conversation.
+        new_user_content (str | List[ChatCompletionContentPartParam]): Content of new user message to append.
         past_messages (list[dict]): The list of past messages in the conversation.
         few_shots (list[dict]): A few-shot list of messages to insert after the system prompt.
         max_tokens (int): The maximum number of tokens allowed for the conversation.
         fallback_to_default (bool): Whether to fallback to default model if the model is not found.
     """
-    message_builder = MessageBuilder(system_prompt, model)
     if max_tokens is None:
         max_tokens = get_token_limit(model, default_to_minimum=fallback_to_default)
 
+    # Start with the required messages: system prompt, few-shots, and new user message
+    message_builder = _MessageBuilder(system_prompt)
+
     for shot in reversed(few_shots):
         message_builder.insert_message(shot.get("role"), shot.get("content"))
 
     append_index = len(few_shots) + 1
 
-    if new_user_message:
-        message_builder.insert_message("user", new_user_message, index=append_index)
+    if new_user_content:
+        message_builder.insert_message("user", new_user_content, index=append_index)
 
-    total_token_count = 0
-    for existing_message in message_builder.messages:
+    total_token_count = count_tokens_for_system_and_tools(
+        model, message_builder.messages[0], tools, tool_choice, default_to_cl100k=fallback_to_default
+    )
+    for existing_message in message_builder.messages[1:]:
         total_token_count += count_tokens_for_message(model, existing_message, default_to_cl100k=fallback_to_default)
 
     newest_to_oldest = list(reversed(past_messages))
     for message in newest_to_oldest:
         potential_message_count = count_tokens_for_message(model, message, default_to_cl100k=fallback_to_default)
         if (total_token_count + potential_message_count) > max_tokens:
             logging.info("Reached max tokens of %d, history will be truncated", max_tokens)
```

### Comparing `openai_messages_token_helper-0.0.6/tests/image_large.png` & `openai_messages_token_helper-0.1.0/tests/image_large.png`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.0.6/tests/test_imageshelper.py` & `openai_messages_token_helper-0.1.0/tests/test_imageshelper.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.0.6/tests/test_modelhelper.py` & `openai_messages_token_helper-0.1.0/tests/test_modelhelper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
-from openai_messages_token_helper import count_tokens_for_message, get_token_limit
+from openai_messages_token_helper import count_tokens_for_message, count_tokens_for_system_and_tools, get_token_limit
 
+from .functions import FUNCTION_COUNTS
 from .messages import system_message, system_message_with_name, text_and_image_message, user_message
 
 
 def test_get_token_limit():
     assert get_token_limit("gpt-35-turbo") == 4000
     assert get_token_limit("gpt-3.5-turbo") == 4000
     assert get_token_limit("gpt-35-turbo-16k") == 16000
@@ -74,7 +75,25 @@
 
 
 def test_count_tokens_for_message_model_default(caplog):
     model = "phi-3"
     with caplog.at_level("WARNING"):
         assert count_tokens_for_message(model, user_message["message"], default_to_cl100k=True) == user_message["count"]
         assert "Model phi-3 not found, defaulting to CL100k encoding" in caplog.text
+
+
+@pytest.mark.parametrize(
+    "function_count_pair",
+    FUNCTION_COUNTS,
+)
+def test_count_tokens_for_system_and_tools(function_count_pair):
+    counted_tokens = count_tokens_for_system_and_tools(
+        "gpt-35-turbo",
+        function_count_pair["system_message"],
+        function_count_pair["tools"],
+        function_count_pair["tool_choice"],
+    )
+    expected_tokens = function_count_pair["count"]
+    diff = counted_tokens - expected_tokens
+    assert (
+        diff >= 0 and diff <= 3
+    ), f"Expected {expected_tokens} tokens, got {counted_tokens}. Counted tokens is only allowed to be off by 3 in the over-counting direction."
```

### Comparing `openai_messages_token_helper-0.0.6/PKG-INFO` & `openai_messages_token_helper-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-messages-token-helper
-Version: 0.0.6
+Version: 0.1.0
 Summary: A helper library for estimating tokens used by messages sent through OpenAI Chat Completions API.
 Author: Pamela Fox
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -55,33 +55,36 @@
 and past messages. The function will truncate the history of past messages if necessary to
 stay within the token limit.
 
 Arguments:
 
 * `model` (`str`): The model name to use for token calculation, like gpt-3.5-turbo.
 * `system_prompt` (`str`): The initial system prompt message.
-* `new_user_message` (`str | List[openai.types.chat.ChatCompletionContentPartParam]`): The new user message to append.
-* `past_messages` (`list[dict]`): The list of past messages in the conversation.
-* `few_shots` (`list[dict]`): A few-shot list of messages to insert after the system prompt.
-* `max_tokens` (`int`): The maximum number of tokens allowed for the conversation.
-* `fallback_to_default` (`bool`): Whether to fallback to default model/token limits if model is not found. Defaults to `False`.
+* `tools` (`List[openai.types.chat.ChatCompletionToolParam]`): (Optional) The tools that will be used in the conversation. These won't be part of the final returned messages, but they will be used to calculate the token count.
+* `tool_choice` (`str | dict`): (Optional) The tool choice that will be used in the conversation. This won't be part of the final returned messages, but it will be used to calculate the token count.
+* `new_user_content` (`str | List[openai.types.chat.ChatCompletionContentPartParam]`): (Optional) The content of new user message to append.
+* `past_messages` (`list[dict]`): (Optional) The list of past messages in the conversation.
+* `few_shots` (`list[dict]`): (Optional) A few-shot list of messages to insert after the system prompt.
+* `max_tokens` (`int`): (Optional) The maximum number of tokens allowed for the conversation.
+* `fallback_to_default` (`bool`): (Optional) Whether to fallback to default model/token limits if model is not found. Defaults to `False`.
+
 
 Returns:
 
 * `list[openai.types.chat.ChatCompletionMessageParam]`
 
 Example:
 
 ```python
 from openai_messages_token_helper import build_messages
 
 messages = build_messages(
     model="gpt-35-turbo",
     system_prompt="You are a bot.",
-    new_user_message="That wasn't a good poem.",
+    new_user_content="That wasn't a good poem.",
     past_messages=[
         {
             "role": "user",
             "content": "Write me a poem",
         },
         {
             "role": "assistant",
```

