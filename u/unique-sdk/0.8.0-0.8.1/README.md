# Comparing `tmp/unique_sdk-0.8.0.tar.gz` & `tmp/unique_sdk-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unique_sdk-0.8.0.tar", max compression
+gzip compressed data, was "unique_sdk-0.8.1.tar", max compression
```

## Comparing `unique_sdk-0.8.0.tar` & `unique_sdk-0.8.1.tar`

### file list

```diff
@@ -1,26 +1,30 @@
--rw-r--r--   0        0        0     1065 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/LICENSE
--rw-r--r--   0        0        0    15211 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/README.md
--rw-r--r--   0        0        0     1400 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2594 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/__init__.py
--rw-r--r--   0        0        0    11523 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_api_requestor.py
--rw-r--r--   0        0        0     3603 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_api_resource.py
--rw-r--r--   0        0        0       46 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_api_version.py
--rw-r--r--   0        0        0     2912 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_error.py
--rw-r--r--   0        0        0     2513 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_http_client.py
--rw-r--r--   0        0        0     3949 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_list_object.py
--rw-r--r--   0        0        0      270 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_object_classes.py
--rw-r--r--   0        0        0      255 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_request_options.py
--rw-r--r--   0        0        0    10525 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_unique_object.py
--rw-r--r--   0        0        0      576 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_unique_response.py
--rw-r--r--   0        0        0     5902 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_util.py
--rw-r--r--   0        0        0       18 2024-04-24 07:50:03.597397 unique_sdk-0.8.0/unique_sdk/_version.py
--rw-r--r--   0        0        0     2855 2024-04-24 07:50:03.601397 unique_sdk-0.8.0/unique_sdk/_webhook.py
--rw-r--r--   0        0        0        0 2024-04-24 07:50:03.601397 unique_sdk-0.8.0/unique_sdk/api_resources/__init__.py
--rw-r--r--   0        0        0     1738 2024-04-24 07:50:03.601397 unique_sdk-0.8.0/unique_sdk/api_resources/_chat_completion.py
--rw-r--r--   0        0        0     3823 2024-04-24 07:50:03.601397 unique_sdk-0.8.0/unique_sdk/api_resources/_content.py
--rw-r--r--   0        0        0      374 2024-04-24 07:50:03.601397 unique_sdk-0.8.0/unique_sdk/api_resources/_event.py
--rw-r--r--   0        0        0     2310 2024-04-24 07:50:03.601397 unique_sdk-0.8.0/unique_sdk/api_resources/_integrated.py
--rw-r--r--   0        0        0     4937 2024-04-24 07:50:03.601397 unique_sdk-0.8.0/unique_sdk/api_resources/_message.py
--rw-r--r--   0        0        0     1235 2024-04-24 07:50:03.601397 unique_sdk-0.8.0/unique_sdk/api_resources/_search.py
--rw-r--r--   0        0        0     1366 2024-04-24 07:50:03.601397 unique_sdk-0.8.0/unique_sdk/api_resources/_search_string.py
--rw-r--r--   0        0        0    15671 1970-01-01 00:00:00.000000 unique_sdk-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-02 11:31:26.787225 unique_sdk-0.8.1/LICENSE
+-rw-r--r--   0        0        0    20706 2024-05-02 11:31:26.787225 unique_sdk-0.8.1/README.md
+-rw-r--r--   0        0        0     1400 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     2594 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/__init__.py
+-rw-r--r--   0        0        0    11523 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/_api_requestor.py
+-rw-r--r--   0        0        0     3603 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/_api_resource.py
+-rw-r--r--   0        0        0       46 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/_api_version.py
+-rw-r--r--   0        0        0     2912 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/_error.py
+-rw-r--r--   0        0        0     2513 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/_http_client.py
+-rw-r--r--   0        0        0     3949 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/_list_object.py
+-rw-r--r--   0        0        0      270 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/_object_classes.py
+-rw-r--r--   0        0        0      255 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/_request_options.py
+-rw-r--r--   0        0        0    10525 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/_unique_object.py
+-rw-r--r--   0        0        0      576 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/_unique_response.py
+-rw-r--r--   0        0        0     5902 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/_util.py
+-rw-r--r--   0        0        0       18 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/_version.py
+-rw-r--r--   0        0        0     2855 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/_webhook.py
+-rw-r--r--   0        0        0        0 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/api_resources/__init__.py
+-rw-r--r--   0        0        0     1738 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/api_resources/_chat_completion.py
+-rw-r--r--   0        0        0     3823 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/api_resources/_content.py
+-rw-r--r--   0        0        0      374 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/api_resources/_event.py
+-rw-r--r--   0        0        0     2310 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/api_resources/_integrated.py
+-rw-r--r--   0        0        0     4937 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/api_resources/_message.py
+-rw-r--r--   0        0        0     1235 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/api_resources/_search.py
+-rw-r--r--   0        0        0     1366 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/api_resources/_search_string.py
+-rw-r--r--   0        0        0     3037 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/utils/chat_history.py
+-rw-r--r--   0        0        0     2059 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/utils/file_io.py
+-rw-r--r--   0        0        0     4948 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/utils/sources.py
+-rw-r--r--   0        0        0     1740 2024-05-02 11:31:26.791225 unique_sdk-0.8.1/unique_sdk/utils/token.py
+-rw-r--r--   0        0        0    21166 1970-01-01 00:00:00.000000 unique_sdk-0.8.1/PKG-INFO
```

### Comparing `unique_sdk-0.8.0/LICENSE` & `unique_sdk-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.0/README.md` & `unique_sdk-0.8.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -12,16 +12,21 @@
 4. [Webhook Triggers](#webhook-triggers)
 5. [Available API Resources](#available-api-resources)
    - [Content](#content)
    - [Message](#message)
    - [Chat Completion](#chat-completion)
    - [Search](#search)
    - [Search String](#search-string)
-6. [Error Handling](#error-handling)
-7. [Examples](#examples)
+6. [Util functions](#utils)
+   - [Chat History](#chat-history)
+   - [File Io](#file-io)
+   - [Sources](#sources)
+   - [token](#token)
+7. [Error Handling](#error-handling)
+8. [Examples](#examples)
 
 ## Installation
 
 Install UniqueSDK and its peer dependency `requests` via pip using the following commands:
 
 ```bash
 pip install unique_sdk
@@ -495,14 +500,219 @@
     user_id,
     company_id,
     prompt="Was ist der Sinn des Lebens, des Universums und des ganzen Rests?",
     chat_id=chat_id
 )
 ```
 
+## Utils
+
+### Chat History
+
+#### `unique_sdk.util.chat_history.load_history`
+
+A helper function that makes sure the chat history is fully loaded and cut to the size of the token window that it fits into the next round of chat interactions.
+
+- `maxTokens` max tokens of the model used
+- `percentOfMaxTokens`=0.15 % max history in % of `maxTokens`
+- `maxMessages`=4, maximal number of messages included in the history.
+
+this method also directly returns a correct formatted history that can be used in the next chat round.
+
+```python
+history = unique_sdk.utils.chat_history.load_history(
+    userId,
+    companyId,
+    chatId
+)
+```
+
+#### `unique_sdk.util.chat_history.convert_chat_history_to_injectable_string`
+
+convert history into a string that can be injected into a prompt. it als returns the token length of the converted history.
+
+```
+chat_history-string, chat_context_token_length = unique_sdk.utils.chat_history.convert_chat_history_to_injectable_string(
+    history
+)
+```
+
+### File Io
+
+Interacting with the knowledge-base.
+
+#### `unique_sdk.util.file_id.download_file`
+
+download files and save them into a folder in `/tmp`
+
+for example using the readUrl from a content.
+
+```python
+pdfFile = download_file("url to a file", "download.pdf")
+```
+
+#### `unique_sdk.util.file_io.upload_file`
+
+Allows for uploading files that then get ingested.
+
+```python
+createdContent = upload_file(
+    userId,
+    companyId,
+    path_to_file="/tmp/hello.pdf",
+    displayed_filename="hello.pdf",
+    mimeType="application/pdf",
+    uploadScope="scope_stcj2osgbl722m22jayidx0n",
+)
+```
+
+### Sources
+
+#### `unique_sdk.util.sources.merge_sources`
+
+Merges multiple search results based on their 'id', removing redundant document and info markers.
+
+This function groups search results by their 'id' and then concatenates their texts,
+cleaning up any document or info markers in subsequent chunks beyond the first one.
+
+Parameters:
+
+- searchContext (list): A list of dictionaries, each representing a search result with 'id' and 'text' keys.
+
+Returns:
+
+- list: A list of dictionaries with merged texts for each unique 'id'.
+
+`searchContext` is an list of search objects that are returned by the search.
+
+```python
+search = unique_sdk.Search.create(
+    user_id=userId,
+    company_id=companyId,
+    chatId=chatId,
+    searchString="Who is Harry P?",
+    searchType="COMBINED",
+    scopeIds="scope_dsf...",
+    limit=30,
+    chatOnly=False,
+)
+
+searchContext = unique_sdk.util.token.pick_search_results_for_token_window(
+        search["data"], config["maxTokens"] - historyLength
+    )
+
+searchContext = unique_sdk.util.sources.merge_sources(search)
+
+```
+
+#### `unique_sdk.util.sources.sort_sources`
+
+Sort sources by order of appearance in documents
+
+```python
+
+search = unique_sdk.Search.create(
+    user_id=userId,
+    company_id=companyId,
+    chatId=chatId,
+    searchString="Who is Harry P?",
+    searchType="COMBINED",
+    scopeIds="scope_dsf...",
+    limit=30,
+    chatOnly=False,
+)
+
+searchContext = unique_sdk.util.token.pick_search_results_for_token_window(
+        search["data"], config["maxTokens"] - historyLength
+    )
+
+searchContext = unique_sdk.util.sources.sort_sources(search)
+```
+
+#### `unique_sdk.util.sources.post_process_sources`
+
+Post-processes the provided text by converting source references into superscript numerals (required
+format by backend to display sources in the chat window)
+
+This function searches the input text for patterns that represent source references (e.g., [source1])
+and replaces them with superscript tags, incrementing the number by one.
+
+Parameters:
+
+- text (str): The text to be post-processed.
+
+Returns:
+
+- str: The text with source references replaced by superscript numerals.
+
+Examples:
+
+- postprocessSources("This is a reference [source0]") will return "This is a reference <sup>1</sup>".
+
+```python
+
+text_with_sup = post_process_sources(text)
+```
+
+### Token
+
+#### unique_sdk.util.token.pick_search_results_for_token_window
+
+Selects and returns a list of search results that fit within a specified token limit.
+
+This function iterates over a list of search results, each with a 'text' field, and
+encodes the text using a predefined encoding scheme. It accumulates search results
+until the token limit is reached or exceeded.
+
+Parameters:
+
+- searchResults (list): A list of dictionaries, each containing a 'text' key with string value.
+- tokenLimit (int): The maximum number of tokens to include in the output.
+
+Returns:
+
+- list: A list of dictionaries representing the search results that fit within the token limit.
+
+```python
+search = unique_sdk.Search.create(
+    user_id=userId,
+    company_id=companyId,
+    chatId=chatId,
+    searchString="Who is Harry P?",
+    searchType="COMBINED",
+    scopeIds="scope_dsf...",
+    limit=30,
+    chatOnly=False,
+)
+
+searchContext = unique_sdk.util.token.pick_search_results_for_token_window(
+        search["data"], config["maxTokens"] - historyLength
+    )
+```
+
+#### unique_sdk.util.token.count_tokens
+
+Counts the number of tokens in the provided text.
+
+This function encodes the input text using a predefined encoding scheme
+and returns the number of tokens in the encoded text.
+
+Parameters:
+
+- text (str): The text to count tokens for.
+
+Returns:
+
+- int: The number of tokens in the text.
+
+```python
+hello = "hello you!"
+searchContext = unique_sdk.util.token.count_tokens(hello)
+```
+
 ## Error Handling
 
 ## Examples
 
 An example Flask app demonstrating the usage of each API resource and how to interact with Webhooks is available in our repository at `/examples/custom-assistant`.
 
 ## Credits
```

### Comparing `unique_sdk-0.8.0/pyproject.toml` & `unique_sdk-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unique-sdk"
-version = "0.8.0"
+version = "0.8.1"
 description = ""
 authors = [
     "Konstantin Krauss <konstantin@unique.ch>",
     "Andreas Hauri <andreas@unique.ch>",
 ]
 readme = "README.md"
 license = "MIT"
```

### Comparing `unique_sdk-0.8.0/unique_sdk/__init__.py` & `unique_sdk-0.8.1/unique_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.0/unique_sdk/_api_requestor.py` & `unique_sdk-0.8.1/unique_sdk/_api_requestor.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.0/unique_sdk/_api_resource.py` & `unique_sdk-0.8.1/unique_sdk/_api_resource.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.0/unique_sdk/_error.py` & `unique_sdk-0.8.1/unique_sdk/_error.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.0/unique_sdk/_http_client.py` & `unique_sdk-0.8.1/unique_sdk/_http_client.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.0/unique_sdk/_list_object.py` & `unique_sdk-0.8.1/unique_sdk/_list_object.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.0/unique_sdk/_unique_object.py` & `unique_sdk-0.8.1/unique_sdk/_unique_object.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.0/unique_sdk/_unique_response.py` & `unique_sdk-0.8.1/unique_sdk/_unique_response.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.0/unique_sdk/_util.py` & `unique_sdk-0.8.1/unique_sdk/_util.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.0/unique_sdk/_webhook.py` & `unique_sdk-0.8.1/unique_sdk/_webhook.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.0/unique_sdk/api_resources/_chat_completion.py` & `unique_sdk-0.8.1/unique_sdk/api_resources/_chat_completion.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.0/unique_sdk/api_resources/_content.py` & `unique_sdk-0.8.1/unique_sdk/api_resources/_content.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.0/unique_sdk/api_resources/_integrated.py` & `unique_sdk-0.8.1/unique_sdk/api_resources/_integrated.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.0/unique_sdk/api_resources/_message.py` & `unique_sdk-0.8.1/unique_sdk/api_resources/_message.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.0/unique_sdk/api_resources/_search.py` & `unique_sdk-0.8.1/unique_sdk/api_resources/_search.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.0/unique_sdk/api_resources/_search_string.py` & `unique_sdk-0.8.1/unique_sdk/api_resources/_search_string.py`

 * *Files identical despite different names*

### Comparing `unique_sdk-0.8.0/PKG-INFO` & `unique_sdk-0.8.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unique-sdk
-Version: 0.8.0
+Version: 0.8.1
 Summary: 
 License: MIT
 Author: Konstantin Krauss
 Author-email: konstantin@unique.ch
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -27,16 +27,21 @@
 4. [Webhook Triggers](#webhook-triggers)
 5. [Available API Resources](#available-api-resources)
    - [Content](#content)
    - [Message](#message)
    - [Chat Completion](#chat-completion)
    - [Search](#search)
    - [Search String](#search-string)
-6. [Error Handling](#error-handling)
-7. [Examples](#examples)
+6. [Util functions](#utils)
+   - [Chat History](#chat-history)
+   - [File Io](#file-io)
+   - [Sources](#sources)
+   - [token](#token)
+7. [Error Handling](#error-handling)
+8. [Examples](#examples)
 
 ## Installation
 
 Install UniqueSDK and its peer dependency `requests` via pip using the following commands:
 
 ```bash
 pip install unique_sdk
@@ -510,14 +515,219 @@
     user_id,
     company_id,
     prompt="Was ist der Sinn des Lebens, des Universums und des ganzen Rests?",
     chat_id=chat_id
 )
 ```
 
+## Utils
+
+### Chat History
+
+#### `unique_sdk.util.chat_history.load_history`
+
+A helper function that makes sure the chat history is fully loaded and cut to the size of the token window that it fits into the next round of chat interactions.
+
+- `maxTokens` max tokens of the model used
+- `percentOfMaxTokens`=0.15 % max history in % of `maxTokens`
+- `maxMessages`=4, maximal number of messages included in the history.
+
+this method also directly returns a correct formatted history that can be used in the next chat round.
+
+```python
+history = unique_sdk.utils.chat_history.load_history(
+    userId,
+    companyId,
+    chatId
+)
+```
+
+#### `unique_sdk.util.chat_history.convert_chat_history_to_injectable_string`
+
+convert history into a string that can be injected into a prompt. it als returns the token length of the converted history.
+
+```
+chat_history-string, chat_context_token_length = unique_sdk.utils.chat_history.convert_chat_history_to_injectable_string(
+    history
+)
+```
+
+### File Io
+
+Interacting with the knowledge-base.
+
+#### `unique_sdk.util.file_id.download_file`
+
+download files and save them into a folder in `/tmp`
+
+for example using the readUrl from a content.
+
+```python
+pdfFile = download_file("url to a file", "download.pdf")
+```
+
+#### `unique_sdk.util.file_io.upload_file`
+
+Allows for uploading files that then get ingested.
+
+```python
+createdContent = upload_file(
+    userId,
+    companyId,
+    path_to_file="/tmp/hello.pdf",
+    displayed_filename="hello.pdf",
+    mimeType="application/pdf",
+    uploadScope="scope_stcj2osgbl722m22jayidx0n",
+)
+```
+
+### Sources
+
+#### `unique_sdk.util.sources.merge_sources`
+
+Merges multiple search results based on their 'id', removing redundant document and info markers.
+
+This function groups search results by their 'id' and then concatenates their texts,
+cleaning up any document or info markers in subsequent chunks beyond the first one.
+
+Parameters:
+
+- searchContext (list): A list of dictionaries, each representing a search result with 'id' and 'text' keys.
+
+Returns:
+
+- list: A list of dictionaries with merged texts for each unique 'id'.
+
+`searchContext` is an list of search objects that are returned by the search.
+
+```python
+search = unique_sdk.Search.create(
+    user_id=userId,
+    company_id=companyId,
+    chatId=chatId,
+    searchString="Who is Harry P?",
+    searchType="COMBINED",
+    scopeIds="scope_dsf...",
+    limit=30,
+    chatOnly=False,
+)
+
+searchContext = unique_sdk.util.token.pick_search_results_for_token_window(
+        search["data"], config["maxTokens"] - historyLength
+    )
+
+searchContext = unique_sdk.util.sources.merge_sources(search)
+
+```
+
+#### `unique_sdk.util.sources.sort_sources`
+
+Sort sources by order of appearance in documents
+
+```python
+
+search = unique_sdk.Search.create(
+    user_id=userId,
+    company_id=companyId,
+    chatId=chatId,
+    searchString="Who is Harry P?",
+    searchType="COMBINED",
+    scopeIds="scope_dsf...",
+    limit=30,
+    chatOnly=False,
+)
+
+searchContext = unique_sdk.util.token.pick_search_results_for_token_window(
+        search["data"], config["maxTokens"] - historyLength
+    )
+
+searchContext = unique_sdk.util.sources.sort_sources(search)
+```
+
+#### `unique_sdk.util.sources.post_process_sources`
+
+Post-processes the provided text by converting source references into superscript numerals (required
+format by backend to display sources in the chat window)
+
+This function searches the input text for patterns that represent source references (e.g., [source1])
+and replaces them with superscript tags, incrementing the number by one.
+
+Parameters:
+
+- text (str): The text to be post-processed.
+
+Returns:
+
+- str: The text with source references replaced by superscript numerals.
+
+Examples:
+
+- postprocessSources("This is a reference [source0]") will return "This is a reference <sup>1</sup>".
+
+```python
+
+text_with_sup = post_process_sources(text)
+```
+
+### Token
+
+#### unique_sdk.util.token.pick_search_results_for_token_window
+
+Selects and returns a list of search results that fit within a specified token limit.
+
+This function iterates over a list of search results, each with a 'text' field, and
+encodes the text using a predefined encoding scheme. It accumulates search results
+until the token limit is reached or exceeded.
+
+Parameters:
+
+- searchResults (list): A list of dictionaries, each containing a 'text' key with string value.
+- tokenLimit (int): The maximum number of tokens to include in the output.
+
+Returns:
+
+- list: A list of dictionaries representing the search results that fit within the token limit.
+
+```python
+search = unique_sdk.Search.create(
+    user_id=userId,
+    company_id=companyId,
+    chatId=chatId,
+    searchString="Who is Harry P?",
+    searchType="COMBINED",
+    scopeIds="scope_dsf...",
+    limit=30,
+    chatOnly=False,
+)
+
+searchContext = unique_sdk.util.token.pick_search_results_for_token_window(
+        search["data"], config["maxTokens"] - historyLength
+    )
+```
+
+#### unique_sdk.util.token.count_tokens
+
+Counts the number of tokens in the provided text.
+
+This function encodes the input text using a predefined encoding scheme
+and returns the number of tokens in the encoded text.
+
+Parameters:
+
+- text (str): The text to count tokens for.
+
+Returns:
+
+- int: The number of tokens in the text.
+
+```python
+hello = "hello you!"
+searchContext = unique_sdk.util.token.count_tokens(hello)
+```
+
 ## Error Handling
 
 ## Examples
 
 An example Flask app demonstrating the usage of each API resource and how to interact with Webhooks is available in our repository at `/examples/custom-assistant`.
 
 ## Credits
```

