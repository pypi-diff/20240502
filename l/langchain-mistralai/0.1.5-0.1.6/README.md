# Comparing `tmp/langchain_mistralai-0.1.5.tar.gz` & `tmp/langchain_mistralai-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_mistralai-0.1.5.tar", max compression
+gzip compressed data, was "langchain_mistralai-0.1.6.tar", max compression
```

## Comparing `langchain_mistralai-0.1.5.tar` & `langchain_mistralai-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-04-29 20:52:17.526269 langchain_mistralai-0.1.5/LICENSE
--rw-r--r--   0        0        0     1336 2024-04-29 20:52:17.526269 langchain_mistralai-0.1.5/README.md
--rw-r--r--   0        0        0      173 2024-04-29 20:52:17.526269 langchain_mistralai-0.1.5/langchain_mistralai/__init__.py
--rw-r--r--   0        0        0    29632 2024-04-29 20:52:17.526269 langchain_mistralai-0.1.5/langchain_mistralai/chat_models.py
--rw-r--r--   0        0        0     7310 2024-04-29 20:52:17.526269 langchain_mistralai-0.1.5/langchain_mistralai/embeddings.py
--rw-r--r--   0        0        0        0 2024-04-29 20:52:17.526269 langchain_mistralai-0.1.5/langchain_mistralai/py.typed
--rw-r--r--   0        0        0     2391 2024-04-29 20:52:17.526269 langchain_mistralai-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2241 1970-01-01 00:00:00.000000 langchain_mistralai-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-02 18:13:03.707168 langchain_mistralai-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1336 2024-05-02 18:13:03.707168 langchain_mistralai-0.1.6/README.md
+-rw-r--r--   0        0        0      173 2024-05-02 18:13:03.707168 langchain_mistralai-0.1.6/langchain_mistralai/__init__.py
+-rw-r--r--   0        0        0    29734 2024-05-02 18:13:03.711168 langchain_mistralai-0.1.6/langchain_mistralai/chat_models.py
+-rw-r--r--   0        0        0     7310 2024-05-02 18:13:03.711168 langchain_mistralai-0.1.6/langchain_mistralai/embeddings.py
+-rw-r--r--   0        0        0        0 2024-05-02 18:13:03.711168 langchain_mistralai-0.1.6/langchain_mistralai/py.typed
+-rw-r--r--   0        0        0     2391 2024-05-02 18:13:03.711168 langchain_mistralai-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2241 1970-01-01 00:00:00.000000 langchain_mistralai-0.1.6/PKG-INFO
```

### Comparing `langchain_mistralai-0.1.5/LICENSE` & `langchain_mistralai-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_mistralai-0.1.5/README.md` & `langchain_mistralai-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `langchain_mistralai-0.1.5/langchain_mistralai/chat_models.py` & `langchain_mistralai-0.1.6/langchain_mistralai/chat_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,14 +255,15 @@
     message: BaseMessage,
 ) -> Dict:
     if isinstance(message, ChatMessage):
         return dict(role=message.role, content=message.content)
     elif isinstance(message, HumanMessage):
         return dict(role="user", content=message.content)
     elif isinstance(message, AIMessage):
+        message_dict: Dict[str, Any] = {"role": "assistant"}
         tool_calls = []
         if message.tool_calls or message.invalid_tool_calls:
             for tool_call in message.tool_calls:
                 tool_calls.append(_format_tool_call_for_mistral(tool_call))
             for invalid_tool_call in message.invalid_tool_calls:
                 tool_calls.append(
                     _format_invalid_tool_call_for_mistral(invalid_tool_call)
@@ -276,26 +277,24 @@
                     }
                 }
                 if _id := tc.get("id"):
                     chunk["id"] = _id
                 tool_calls.append(chunk)
         else:
             pass
+        if tool_calls:  # do not populate empty list tool_calls
+            message_dict["tool_calls"] = tool_calls
         if tool_calls and message.content:
             # Assistant message must have either content or tool_calls, but not both.
             # Some providers may not support tool_calls in the same message as content.
             # This is done to ensure compatibility with messages from other providers.
-            content: Any = ""
+            message_dict["content"] = ""
         else:
-            content = message.content
-        return {
-            "role": "assistant",
-            "content": content,
-            "tool_calls": tool_calls,
-        }
+            message_dict["content"] = message.content
+        return message_dict
     elif isinstance(message, SystemMessage):
         return dict(role="system", content=message.content)
     elif isinstance(message, ToolMessage):
         return {
             "role": "tool",
             "content": message.content,
             "name": message.name,
```

### Comparing `langchain_mistralai-0.1.5/langchain_mistralai/embeddings.py` & `langchain_mistralai-0.1.6/langchain_mistralai/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_mistralai-0.1.5/pyproject.toml` & `langchain_mistralai-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-mistralai"
-version = "0.1.5"
+version = "0.1.6"
 description = "An integration package connecting Mistral and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_mistralai-0.1.5/PKG-INFO` & `langchain_mistralai-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-mistralai
-Version: 0.1.5
+Version: 0.1.6
 Summary: An integration package connecting Mistral and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

