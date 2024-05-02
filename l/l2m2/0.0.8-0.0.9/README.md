# Comparing `tmp/l2m2-0.0.8.tar.gz` & `tmp/l2m2-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "l2m2-0.0.8.tar", last modified: Fri Apr 12 07:59:48 2024, max compression
+gzip compressed data, was "l2m2-0.0.9.tar", last modified: Fri Apr 12 15:14:55 2024, max compression
```

## Comparing `l2m2-0.0.8.tar` & `l2m2-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 07:59:48.495719 l2m2-0.0.8/
--rw-r--r--   0 pierce     (503) staff       (20)     1070 2024-04-12 00:41:01.000000 l2m2-0.0.8/LICENSE
--rw-r--r--   0 pierce     (503) staff       (20)     5056 2024-04-12 07:59:48.495510 l2m2-0.0.8/PKG-INFO
--rw-r--r--   0 pierce     (503) staff       (20)     3163 2024-04-12 04:51:33.000000 l2m2-0.0.8/README.md
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 07:59:48.494117 l2m2-0.0.8/l2m2/
--rw-r--r--   0 pierce     (503) staff       (20)       34 2024-04-11 23:42:30.000000 l2m2-0.0.8/l2m2/__init__.py
--rw-r--r--   0 pierce     (503) staff       (20)     6578 2024-04-12 07:57:54.000000 l2m2-0.0.8/l2m2/llm_client.py
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 07:59:48.495037 l2m2-0.0.8/l2m2.egg-info/
--rw-r--r--   0 pierce     (503) staff       (20)     5056 2024-04-12 07:59:48.000000 l2m2-0.0.8/l2m2.egg-info/PKG-INFO
--rw-r--r--   0 pierce     (503) staff       (20)      258 2024-04-12 07:59:48.000000 l2m2-0.0.8/l2m2.egg-info/SOURCES.txt
--rw-r--r--   0 pierce     (503) staff       (20)        1 2024-04-12 07:59:48.000000 l2m2-0.0.8/l2m2.egg-info/dependency_links.txt
--rw-r--r--   0 pierce     (503) staff       (20)       86 2024-04-12 07:59:48.000000 l2m2-0.0.8/l2m2.egg-info/requires.txt
--rw-r--r--   0 pierce     (503) staff       (20)        5 2024-04-12 07:59:48.000000 l2m2-0.0.8/l2m2.egg-info/top_level.txt
--rw-r--r--   0 pierce     (503) staff       (20)      755 2024-04-12 07:59:43.000000 l2m2-0.0.8/pyproject.toml
--rw-r--r--   0 pierce     (503) staff       (20)       85 2024-04-12 00:57:10.000000 l2m2-0.0.8/requirements.txt
--rw-r--r--   0 pierce     (503) staff       (20)       38 2024-04-12 07:59:48.495772 l2m2-0.0.8/setup.cfg
--rw-r--r--   0 pierce     (503) staff       (20)      377 2024-04-12 07:47:38.000000 l2m2-0.0.8/setup.py
-drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 07:59:48.494858 l2m2-0.0.8/tests/
--rw-r--r--   0 pierce     (503) staff       (20)     4224 2024-04-12 03:01:46.000000 l2m2-0.0.8/tests/test_llm_client.py
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 15:14:55.277162 l2m2-0.0.9/
+-rw-r--r--   0 pierce     (503) staff       (20)     1070 2024-04-12 00:41:01.000000 l2m2-0.0.9/LICENSE
+-rw-r--r--   0 pierce     (503) staff       (20)     5183 2024-04-12 15:14:55.276959 l2m2-0.0.9/PKG-INFO
+-rw-r--r--   0 pierce     (503) staff       (20)     3290 2024-04-12 15:13:31.000000 l2m2-0.0.9/README.md
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 15:14:55.275594 l2m2-0.0.9/l2m2/
+-rw-r--r--   0 pierce     (503) staff       (20)       34 2024-04-11 23:42:30.000000 l2m2-0.0.9/l2m2/__init__.py
+-rw-r--r--   0 pierce     (503) staff       (20)     6746 2024-04-12 15:09:51.000000 l2m2-0.0.9/l2m2/llm_client.py
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 15:14:55.276708 l2m2-0.0.9/l2m2.egg-info/
+-rw-r--r--   0 pierce     (503) staff       (20)     5183 2024-04-12 15:14:55.000000 l2m2-0.0.9/l2m2.egg-info/PKG-INFO
+-rw-r--r--   0 pierce     (503) staff       (20)      249 2024-04-12 15:14:55.000000 l2m2-0.0.9/l2m2.egg-info/SOURCES.txt
+-rw-r--r--   0 pierce     (503) staff       (20)        1 2024-04-12 15:14:55.000000 l2m2-0.0.9/l2m2.egg-info/dependency_links.txt
+-rw-r--r--   0 pierce     (503) staff       (20)       86 2024-04-12 15:14:55.000000 l2m2-0.0.9/l2m2.egg-info/requires.txt
+-rw-r--r--   0 pierce     (503) staff       (20)        5 2024-04-12 15:14:55.000000 l2m2-0.0.9/l2m2.egg-info/top_level.txt
+-rw-r--r--   0 pierce     (503) staff       (20)      754 2024-04-12 15:14:27.000000 l2m2-0.0.9/pyproject.toml
+-rw-r--r--   0 pierce     (503) staff       (20)       85 2024-04-12 00:57:10.000000 l2m2-0.0.9/requirements.txt
+-rw-r--r--   0 pierce     (503) staff       (20)       38 2024-04-12 15:14:55.277204 l2m2-0.0.9/setup.cfg
+drwxr-xr-x   0 pierce     (503) staff       (20)        0 2024-04-12 15:14:55.276504 l2m2-0.0.9/tests/
+-rw-r--r--   0 pierce     (503) staff       (20)     4224 2024-04-12 03:01:46.000000 l2m2-0.0.9/tests/test_llm_client.py
```

### Comparing `l2m2-0.0.8/LICENSE` & `l2m2-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `l2m2-0.0.8/PKG-INFO` & `l2m2-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: l2m2
-Version: 0.0.8
+Version: 0.0.9
 Summary: A very simple LLM manager for Python.
 Author-email: Pierce Kelaita <pierce@kelaita.com>
 License: MIT License
         
         Copyright (c) 2024 Pierce Kelaita
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,27 +41,30 @@
 
 **[L2M2](https://pypi.org/project/l2m2/)** ("LLM Manager" &rarr; "LLMM" &rarr; "L2M2") is a very simple LLM manager for Python that allows you to expose lots of models through a single API. This is useful for evaluation, demos, and production LLM apps that use multiple models.
 
 ## Supported Models
 
 L2M2 currently supports the following models:
 
-| Provider                                     | Model Name        | Model Version              |
-| -------------------------------------------- | ----------------- | -------------------------- |
-| [`openai`](https://openai.com/product)       | `gpt-4-turbo`     | `gpt-4-0125-preview`       |
-| [`google`](https://ai.google.dev/)           | `gemini-1.5-pro`  | `gemini-1.5-pro-latest`    |
-| [`google`](https://ai.google.dev/)           | `gemini-1.0-pro`  | `gemini-1.0-pro-latest`    |
-| [`anthropic`](https://www.anthropic.com/api) | `claude-3-opus`   | `claude-3-opus-20240229`   |
-| [`anthropic`](https://www.anthropic.com/api) | `claude-3-sonnet` | `claude-3-sonnet-20240229` |
-| [`anthropic`](https://www.anthropic.com/api) | `claude-3-haiku`  | `claude-3-haiku-20240307`  |
-| [`cohere`](https://docs.cohere.com/)         | `command-r`       | `command-r`                |
-| [`cohere`](https://docs.cohere.com/)         | `command-r-plus`  | `command-r-plus`           |
-| [`groq`](https://wow.groq.com/)              | `llama2-70b`      | `llama2-70b-4096`          |
-| [`groq`](https://wow.groq.com/)              | `mixtral-8x7b`    | `mixtral-8x7b-32768`       |
-| [`groq`](https://wow.groq.com/)              | `gemma-7b`        | `gemma-7b-it`              |
+| Provider                                     | Model Name         | Model Version              |
+| -------------------------------------------- | ------------------ | -------------------------- |
+| [`openai`](https://openai.com/product)       | `gpt-4-turbo`      | `gpt-4-turbo-2024-04-09`   |
+| [`openai`](https://openai.com/product)       | `gpt-4-turbo-0125` | `gpt-4-0125-preview`       |
+| [`google`](https://ai.google.dev/)           | `gemini-1.5-pro`   | `gemini-1.5-pro-latest`    |
+| [`google`](https://ai.google.dev/)           | `gemini-1.0-pro`   | `gemini-1.0-pro-latest`    |
+| [`anthropic`](https://www.anthropic.com/api) | `claude-3-opus`    | `claude-3-opus-20240229`   |
+| [`anthropic`](https://www.anthropic.com/api) | `claude-3-sonnet`  | `claude-3-sonnet-20240229` |
+| [`anthropic`](https://www.anthropic.com/api) | `claude-3-haiku`   | `claude-3-haiku-20240307`  |
+| [`cohere`](https://docs.cohere.com/)         | `command-r`        | `command-r`                |
+| [`cohere`](https://docs.cohere.com/)         | `command-r-plus`   | `command-r-plus`           |
+| [`groq`](https://wow.groq.com/)              | `llama2-70b`       | `llama2-70b-4096`          |
+| [`groq`](https://wow.groq.com/)              | `mixtral-8x7b`     | `mixtral-8x7b-32768`       |
+| [`groq`](https://wow.groq.com/)              | `gemma-7b`         | `gemma-7b-it`              |
+
+            |
 
 ## Installation
 
 ```sh
 pip install l2m2
 ```
```

### Comparing `l2m2-0.0.8/README.md` & `l2m2-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 
 **[L2M2](https://pypi.org/project/l2m2/)** ("LLM Manager" &rarr; "LLMM" &rarr; "L2M2") is a very simple LLM manager for Python that allows you to expose lots of models through a single API. This is useful for evaluation, demos, and production LLM apps that use multiple models.
 
 ## Supported Models
 
 L2M2 currently supports the following models:
 
-| Provider                                     | Model Name        | Model Version              |
-| -------------------------------------------- | ----------------- | -------------------------- |
-| [`openai`](https://openai.com/product)       | `gpt-4-turbo`     | `gpt-4-0125-preview`       |
-| [`google`](https://ai.google.dev/)           | `gemini-1.5-pro`  | `gemini-1.5-pro-latest`    |
-| [`google`](https://ai.google.dev/)           | `gemini-1.0-pro`  | `gemini-1.0-pro-latest`    |
-| [`anthropic`](https://www.anthropic.com/api) | `claude-3-opus`   | `claude-3-opus-20240229`   |
-| [`anthropic`](https://www.anthropic.com/api) | `claude-3-sonnet` | `claude-3-sonnet-20240229` |
-| [`anthropic`](https://www.anthropic.com/api) | `claude-3-haiku`  | `claude-3-haiku-20240307`  |
-| [`cohere`](https://docs.cohere.com/)         | `command-r`       | `command-r`                |
-| [`cohere`](https://docs.cohere.com/)         | `command-r-plus`  | `command-r-plus`           |
-| [`groq`](https://wow.groq.com/)              | `llama2-70b`      | `llama2-70b-4096`          |
-| [`groq`](https://wow.groq.com/)              | `mixtral-8x7b`    | `mixtral-8x7b-32768`       |
-| [`groq`](https://wow.groq.com/)              | `gemma-7b`        | `gemma-7b-it`              |
+| Provider                                     | Model Name         | Model Version              |
+| -------------------------------------------- | ------------------ | -------------------------- |
+| [`openai`](https://openai.com/product)       | `gpt-4-turbo`      | `gpt-4-turbo-2024-04-09`   |
+| [`openai`](https://openai.com/product)       | `gpt-4-turbo-0125` | `gpt-4-0125-preview`       |
+| [`google`](https://ai.google.dev/)           | `gemini-1.5-pro`   | `gemini-1.5-pro-latest`    |
+| [`google`](https://ai.google.dev/)           | `gemini-1.0-pro`   | `gemini-1.0-pro-latest`    |
+| [`anthropic`](https://www.anthropic.com/api) | `claude-3-opus`    | `claude-3-opus-20240229`   |
+| [`anthropic`](https://www.anthropic.com/api) | `claude-3-sonnet`  | `claude-3-sonnet-20240229` |
+| [`anthropic`](https://www.anthropic.com/api) | `claude-3-haiku`   | `claude-3-haiku-20240307`  |
+| [`cohere`](https://docs.cohere.com/)         | `command-r`        | `command-r`                |
+| [`cohere`](https://docs.cohere.com/)         | `command-r-plus`   | `command-r-plus`           |
+| [`groq`](https://wow.groq.com/)              | `llama2-70b`       | `llama2-70b-4096`          |
+| [`groq`](https://wow.groq.com/)              | `mixtral-8x7b`     | `mixtral-8x7b-32768`       |
+| [`groq`](https://wow.groq.com/)              | `gemma-7b`         | `gemma-7b-it`              |
+
+            |
 
 ## Installation
 
 ```sh
 pip install l2m2
 ```
```

### Comparing `l2m2-0.0.8/l2m2/llm_client.py` & `l2m2-0.0.9/l2m2/llm_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 from anthropic import Anthropic
 from groq import Groq
 
 
 _MODEL_INFO = {
     "gpt-4-turbo": {
         "provider": "openai",
+        "model_id": "gpt-4-turbo-2024-04-09",
+        "provider_homepage": "https://openai.com/product",
+    },
+    "gpt-4-turbo-0125": {
+        "provider": "openai",
         "model_id": "gpt-4-0125-preview",
         "provider_homepage": "https://openai.com/product",
     },
     "gemini-1.5-pro": {
         "provider": "google",
         "model_id": "gemini-1.5-pro-latest",
         "provider_homepage": "https://ai.google.dev/",
```

### Comparing `l2m2-0.0.8/l2m2.egg-info/PKG-INFO` & `l2m2-0.0.9/l2m2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: l2m2
-Version: 0.0.8
+Version: 0.0.9
 Summary: A very simple LLM manager for Python.
 Author-email: Pierce Kelaita <pierce@kelaita.com>
 License: MIT License
         
         Copyright (c) 2024 Pierce Kelaita
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -41,27 +41,30 @@
 
 **[L2M2](https://pypi.org/project/l2m2/)** ("LLM Manager" &rarr; "LLMM" &rarr; "L2M2") is a very simple LLM manager for Python that allows you to expose lots of models through a single API. This is useful for evaluation, demos, and production LLM apps that use multiple models.
 
 ## Supported Models
 
 L2M2 currently supports the following models:
 
-| Provider                                     | Model Name        | Model Version              |
-| -------------------------------------------- | ----------------- | -------------------------- |
-| [`openai`](https://openai.com/product)       | `gpt-4-turbo`     | `gpt-4-0125-preview`       |
-| [`google`](https://ai.google.dev/)           | `gemini-1.5-pro`  | `gemini-1.5-pro-latest`    |
-| [`google`](https://ai.google.dev/)           | `gemini-1.0-pro`  | `gemini-1.0-pro-latest`    |
-| [`anthropic`](https://www.anthropic.com/api) | `claude-3-opus`   | `claude-3-opus-20240229`   |
-| [`anthropic`](https://www.anthropic.com/api) | `claude-3-sonnet` | `claude-3-sonnet-20240229` |
-| [`anthropic`](https://www.anthropic.com/api) | `claude-3-haiku`  | `claude-3-haiku-20240307`  |
-| [`cohere`](https://docs.cohere.com/)         | `command-r`       | `command-r`                |
-| [`cohere`](https://docs.cohere.com/)         | `command-r-plus`  | `command-r-plus`           |
-| [`groq`](https://wow.groq.com/)              | `llama2-70b`      | `llama2-70b-4096`          |
-| [`groq`](https://wow.groq.com/)              | `mixtral-8x7b`    | `mixtral-8x7b-32768`       |
-| [`groq`](https://wow.groq.com/)              | `gemma-7b`        | `gemma-7b-it`              |
+| Provider                                     | Model Name         | Model Version              |
+| -------------------------------------------- | ------------------ | -------------------------- |
+| [`openai`](https://openai.com/product)       | `gpt-4-turbo`      | `gpt-4-turbo-2024-04-09`   |
+| [`openai`](https://openai.com/product)       | `gpt-4-turbo-0125` | `gpt-4-0125-preview`       |
+| [`google`](https://ai.google.dev/)           | `gemini-1.5-pro`   | `gemini-1.5-pro-latest`    |
+| [`google`](https://ai.google.dev/)           | `gemini-1.0-pro`   | `gemini-1.0-pro-latest`    |
+| [`anthropic`](https://www.anthropic.com/api) | `claude-3-opus`    | `claude-3-opus-20240229`   |
+| [`anthropic`](https://www.anthropic.com/api) | `claude-3-sonnet`  | `claude-3-sonnet-20240229` |
+| [`anthropic`](https://www.anthropic.com/api) | `claude-3-haiku`   | `claude-3-haiku-20240307`  |
+| [`cohere`](https://docs.cohere.com/)         | `command-r`        | `command-r`                |
+| [`cohere`](https://docs.cohere.com/)         | `command-r-plus`   | `command-r-plus`           |
+| [`groq`](https://wow.groq.com/)              | `llama2-70b`       | `llama2-70b-4096`          |
+| [`groq`](https://wow.groq.com/)              | `mixtral-8x7b`     | `mixtral-8x7b-32768`       |
+| [`groq`](https://wow.groq.com/)              | `gemma-7b`         | `gemma-7b-it`              |
+
+            |
 
 ## Installation
 
 ```sh
 pip install l2m2
 ```
```

### Comparing `l2m2-0.0.8/pyproject.toml` & `l2m2-0.0.9/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 [build-system]
 requires = ["setuptools>=69.2.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "l2m2"
-authors = [
-    {name = "Pierce Kelaita", email = "pierce@kelaita.com"},
-]
+authors = [{ name = "Pierce Kelaita", email = "pierce@kelaita.com" }]
 description = "A very simple LLM manager for Python."
-version = "0.0.8"
+version = "0.0.9"
 readme = "README.md"
-license = {file = "LICENSE"}
+license = { file = "LICENSE" }
 requires-python = ">=3.12"
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
-dependencies = {file = ["requirements.txt"]}
+dependencies = { file = ["requirements.txt"] }
 
 [project.urls]
 Homepage = "https://github.com/pkelaita/l2m2"
 Documentation = "https://github.com/pkelaita/l2m2/blob/main/README.md"
 Repository = "https://github.com/pkelaita/l2m2.git"
 Issues = "https://github.com/pkelaita/l2m2/issues"
 
 [tool.setuptools.packages.find]
-exclude = ["tests*"] 
-namespaces = false
+exclude = ["tests*"]
+namespaces = false
```

### Comparing `l2m2-0.0.8/tests/test_llm_client.py` & `l2m2-0.0.9/tests/test_llm_client.py`

 * *Files identical despite different names*

