# Comparing `tmp/vulavula-0.1.0.tar.gz` & `tmp/vulavula-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulavula-0.1.0.tar", last modified: Tue Apr 30 15:16:35 2024, max compression
+gzip compressed data, was "vulavula-0.1.1.tar", last modified: Thu May  2 11:16:44 2024, max compression
```

## Comparing `vulavula-0.1.0.tar` & `vulavula-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     5478 2024-04-30 07:56:21.486859 vulavula-0.1.0/README.md
--rw-r--r--   0        0        0     1209 2024-04-30 15:16:35.197093 vulavula-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-16 06:16:28.668957 vulavula-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 14:29:34.526393 vulavula-0.1.0/tests/audio/test1.mp3
--rw-r--r--   0        0        0     3284 2024-04-29 14:43:59.295093 vulavula-0.1.0/tests/test_nlu.py
--rw-r--r--   0        0        0     2150 2024-04-29 14:43:59.289729 vulavula-0.1.0/tests/test_sentiment.py
--rw-r--r--   0        0        0     3429 2024-04-29 14:43:59.282839 vulavula-0.1.0/tests/test_transcribe.py
--rw-r--r--   0        0        0     1884 2024-04-29 14:43:59.273964 vulavula-0.1.0/tests/test_transport.py
--rw-r--r--   0        0        0       35 2024-04-23 11:14:19.916277 vulavula-0.1.0/vulavula/__init__.py
--rw-r--r--   0        0        0       35 2024-04-23 14:16:08.762333 vulavula-0.1.0/vulavula/client/__init__.py
--rw-r--r--   0        0        0     3985 2024-04-30 06:15:55.630210 vulavula-0.1.0/vulavula/client/client.py
--rw-r--r--   0        0        0     4555 2024-04-29 14:43:59.277209 vulavula-0.1.0/vulavula/client/nlu.py
--rw-r--r--   0        0        0     2704 2024-04-29 14:43:59.291343 vulavula-0.1.0/vulavula/client/sentiment.py
--rw-r--r--   0        0        0     5667 2024-04-30 06:09:08.739182 vulavula-0.1.0/vulavula/client/transcribe.py
--rw-r--r--   0        0        0     3633 2024-04-29 14:43:59.285020 vulavula-0.1.0/vulavula/client/transport.py
--rw-r--r--   0        0        0        1 2024-04-23 11:13:57.420564 vulavula-0.1.0/vulavula/common/__init__.py
--rw-r--r--   0        0        0      942 2024-04-30 07:32:25.567183 vulavula-0.1.0/vulavula/common/error_handler.py
--rw-r--r--   0        0        0     2748 2024-04-30 07:32:25.563980 vulavula-0.1.0/vulavula/common/response_handler.py
--rw-r--r--   0        0        0       29 2024-04-29 05:41:26.660557 vulavula-0.1.0/vulavula/config/__init__.py
--rw-r--r--   0        0        0      323 2024-04-30 05:43:40.104683 vulavula-0.1.0/vulavula/config/config.py
--rw-r--r--   0        0        0        1 2024-04-23 08:22:22.751651 vulavula-0.1.0/vulavula/models/__init__.py
--rw-r--r--   0        0        0      220 2024-04-23 08:44:00.579673 vulavula-0.1.0/vulavula/models/types/__init__.py
--rw-r--r--   0        0        0      105 2024-04-23 08:25:48.808783 vulavula-0.1.0/vulavula/models/types/entity_recognition.py
--rw-r--r--   0        0        0     1529 2024-04-23 08:45:47.626703 vulavula-0.1.0/vulavula/models/types/intent_classification.py
--rw-r--r--   0        0        0      105 2024-04-23 08:34:00.097047 vulavula-0.1.0/vulavula/models/types/sentiment_analysis.py
--rw-r--r--   0        0        0     6407 1970-01-01 00:00:00.000000 vulavula-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5336 2024-05-01 17:41:53.374894 vulavula-0.1.1/README.md
+-rw-r--r--   0        0        0      912 2024-05-02 11:16:44.820504 vulavula-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 06:16:28.668957 vulavula-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-30 15:37:52.520889 vulavula-0.1.1/tests/audio/test1.mp3
+-rw-r--r--   0        0        0     3284 2024-05-01 17:41:53.376004 vulavula-0.1.1/tests/test_nlu.py
+-rw-r--r--   0        0        0     2150 2024-05-01 17:41:53.376223 vulavula-0.1.1/tests/test_sentiment.py
+-rw-r--r--   0        0        0     3429 2024-05-01 17:41:53.376541 vulavula-0.1.1/tests/test_transcribe.py
+-rw-r--r--   0        0        0     1884 2024-05-01 17:41:53.376685 vulavula-0.1.1/tests/test_transport.py
+-rw-r--r--   0        0        0       35 2024-05-01 17:41:53.376769 vulavula-0.1.1/vulavula/__init__.py
+-rw-r--r--   0        0        0       35 2024-05-01 17:41:53.376848 vulavula-0.1.1/vulavula/client/__init__.py
+-rw-r--r--   0        0        0     3985 2024-05-01 17:41:53.376982 vulavula-0.1.1/vulavula/client/client.py
+-rw-r--r--   0        0        0     4555 2024-05-01 17:41:53.377242 vulavula-0.1.1/vulavula/client/nlu.py
+-rw-r--r--   0        0        0     2704 2024-05-01 17:41:53.377347 vulavula-0.1.1/vulavula/client/sentiment.py
+-rw-r--r--   0        0        0     5667 2024-05-01 17:41:53.377627 vulavula-0.1.1/vulavula/client/transcribe.py
+-rw-r--r--   0        0        0     3633 2024-05-01 17:41:53.377741 vulavula-0.1.1/vulavula/client/transport.py
+-rw-r--r--   0        0        0        1 2024-05-01 17:41:53.377828 vulavula-0.1.1/vulavula/common/__init__.py
+-rw-r--r--   0        0        0      942 2024-05-01 17:41:53.378112 vulavula-0.1.1/vulavula/common/error_handler.py
+-rw-r--r--   0        0        0     2748 2024-05-01 17:41:53.378366 vulavula-0.1.1/vulavula/common/response_handler.py
+-rw-r--r--   0        0        0       29 2024-05-01 17:41:53.378448 vulavula-0.1.1/vulavula/config/__init__.py
+-rw-r--r--   0        0        0      323 2024-05-01 17:41:53.378562 vulavula-0.1.1/vulavula/config/config.py
+-rw-r--r--   0        0        0        1 2024-05-01 17:41:53.378636 vulavula-0.1.1/vulavula/models/__init__.py
+-rw-r--r--   0        0        0      220 2024-05-01 17:41:53.378712 vulavula-0.1.1/vulavula/models/types/__init__.py
+-rw-r--r--   0        0        0      105 2024-05-01 17:41:53.378800 vulavula-0.1.1/vulavula/models/types/entity_recognition.py
+-rw-r--r--   0        0        0     1529 2024-05-01 17:41:53.378896 vulavula-0.1.1/vulavula/models/types/intent_classification.py
+-rw-r--r--   0        0        0      105 2024-05-01 17:41:53.378976 vulavula-0.1.1/vulavula/models/types/sentiment_analysis.py
+-rw-r--r--   0        0        0     5968 1970-01-01 00:00:00.000000 vulavula-0.1.1/PKG-INFO
```

### Comparing `vulavula-0.1.0/README.md` & `vulavula-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # vulavula
-The `vulavula` is a Python client SDK designed to interact with the Vulavula API. It simplifies making requests to various endpoints such as transcription, file uploads, sentiment analysis, and entity recognition. The SDK handles network communications, error handling, and response parsing, providing a user-friendly interface for developers.
+`vulavula` is a Python client SDK designed to interact with the Vulavula API. It simplifies making requests to endpoints such as transcription, file uploads, sentiment analysis, and entity recognition. The SDK also handles network communications, error handling, and response parsing, providing a friendlier interface for developers.
 
 ## Features
 
 - Simple and intuitive API methods for:
   - Transcribing audio files
   - Uploading files
   - Entity recognition
@@ -99,15 +99,15 @@
   - `inputs`: A list of strings, each a new sentence to classify based on the trained model.
 
 #### Classification Results:
 - The output is a list of dictionaries, each corresponding to an input sentence.
 - Each dictionary contains a list of `probabilities`, where each item is another dictionary detailing an `intent` and its associated `score` (a confidence level).
 
 ### Error Handling
-Proper error handling is crucial for building resilient applications, especially when interacting with external services like APIs. This section covers how to handle errors gracefully when using the Vulavula API.
+This section covers how to handle errors gracefully when using the Vulavula API.
 
 #### Handling Specific Errors with VulavulaError
 The `VulavulaError` is a custom exception class designed to provide detailed information about errors encountered during API interactions. It includes a human-readable message and a structured JSON object containing additional error details. <br>
 Here’s an example of how to handle `VulavulaError`:
 ```python
 try:
     entity_result = client.get_entities({'text': 'President Ramaphosa gaan loop by Emfuleni Municipality.'})
```

### Comparing `vulavula-0.1.0/pyproject.toml` & `vulavula-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "vulavula"
-version = "0.1.0"
-description = "The `vulavula` Python SDK provides access for the Vulavula API. It is designed to optimize developer workflows by streamlining the integration of services like transcription, sentiment analysis, and entity recognition. This SDK simplifies complex API interactions, making it easier to manage network requests, parse responses, and handle errors effectively."
+version = "0.1.1"
+description = "The vulavula Python SDK provides access to the Vulavula API."
 authors = [
     { name = "Raphael Karanja", email = "raphael.karanja@lelapa.ai" },
 ]
 dependencies = [
     "requests>=2.31.0",
     "pydantic[dotenv]>=2.7.1",
     "pydantic-settings>=2.2.1",
```

### Comparing `vulavula-0.1.0/tests/test_nlu.py` & `vulavula-0.1.1/tests/test_nlu.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.0/tests/test_sentiment.py` & `vulavula-0.1.1/tests/test_sentiment.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.0/tests/test_transcribe.py` & `vulavula-0.1.1/tests/test_transcribe.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.0/tests/test_transport.py` & `vulavula-0.1.1/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.0/vulavula/client/client.py` & `vulavula-0.1.1/vulavula/client/client.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.0/vulavula/client/nlu.py` & `vulavula-0.1.1/vulavula/client/nlu.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.0/vulavula/client/sentiment.py` & `vulavula-0.1.1/vulavula/client/sentiment.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.0/vulavula/client/transcribe.py` & `vulavula-0.1.1/vulavula/client/transcribe.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.0/vulavula/client/transport.py` & `vulavula-0.1.1/vulavula/client/transport.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.0/vulavula/common/error_handler.py` & `vulavula-0.1.1/vulavula/common/error_handler.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.0/vulavula/common/response_handler.py` & `vulavula-0.1.1/vulavula/common/response_handler.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.0/vulavula/models/types/intent_classification.py` & `vulavula-0.1.1/vulavula/models/types/intent_classification.py`

 * *Files identical despite different names*

### Comparing `vulavula-0.1.0/PKG-INFO` & `vulavula-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: vulavula
-Version: 0.1.0
-Summary: The `vulavula` Python SDK provides access for the Vulavula API. It is designed to optimize developer workflows by streamlining the integration of services like transcription, sentiment analysis, and entity recognition. This SDK simplifies complex API interactions, making it easier to manage network requests, parse responses, and handle errors effectively.
+Version: 0.1.1
+Summary: The vulavula Python SDK provides access to the Vulavula API.
 Keywords: lelapa,vulavula,nlp,intent,multilingual,transcription
 Author-Email: Raphael Karanja <raphael.karanja@lelapa.ai>
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/Lelapa-AI/vulavula-sdk
 Requires-Python: >=3.8
 Requires-Dist: requests>=2.31.0
 Requires-Dist: pydantic[dotenv]>=2.7.1
 Requires-Dist: pydantic-settings>=2.2.1
 Description-Content-Type: text/markdown
 
 # vulavula
-The `vulavula` is a Python client SDK designed to interact with the Vulavula API. It simplifies making requests to various endpoints such as transcription, file uploads, sentiment analysis, and entity recognition. The SDK handles network communications, error handling, and response parsing, providing a user-friendly interface for developers.
+`vulavula` is a Python client SDK designed to interact with the Vulavula API. It simplifies making requests to endpoints such as transcription, file uploads, sentiment analysis, and entity recognition. The SDK also handles network communications, error handling, and response parsing, providing a friendlier interface for developers.
 
 ## Features
 
 - Simple and intuitive API methods for:
   - Transcribing audio files
   - Uploading files
   - Entity recognition
@@ -116,15 +116,15 @@
   - `inputs`: A list of strings, each a new sentence to classify based on the trained model.
 
 #### Classification Results:
 - The output is a list of dictionaries, each corresponding to an input sentence.
 - Each dictionary contains a list of `probabilities`, where each item is another dictionary detailing an `intent` and its associated `score` (a confidence level).
 
 ### Error Handling
-Proper error handling is crucial for building resilient applications, especially when interacting with external services like APIs. This section covers how to handle errors gracefully when using the Vulavula API.
+This section covers how to handle errors gracefully when using the Vulavula API.
 
 #### Handling Specific Errors with VulavulaError
 The `VulavulaError` is a custom exception class designed to provide detailed information about errors encountered during API interactions. It includes a human-readable message and a structured JSON object containing additional error details. <br>
 Here’s an example of how to handle `VulavulaError`:
 ```python
 try:
     entity_result = client.get_entities({'text': 'President Ramaphosa gaan loop by Emfuleni Municipality.'})
```

