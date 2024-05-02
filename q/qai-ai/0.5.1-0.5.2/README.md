# Comparing `tmp/qai_ai-0.5.1.tar.gz` & `tmp/qai_ai-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qai_ai-0.5.1.tar", max compression
+gzip compressed data, was "qai_ai-0.5.2.tar", max compression
```

## Comparing `qai_ai-0.5.1.tar` & `qai_ai-0.5.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       23 2024-05-01 22:37:27.943154 qai_ai-0.5.1/README.md
--rw-r--r--   0        0        0     1472 2024-05-02 01:45:25.724783 qai_ai-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      220 2024-04-08 11:26:06.938861 qai_ai-0.5.1/src/qai/ai/__init__.py
--rw-r--r--   0        0        0      396 2024-03-06 15:37:18.122377 qai_ai-0.5.1/src/qai/ai/config.py
--rw-r--r--   0        0        0        0 2024-02-17 11:28:19.525049 qai_ai-0.5.1/src/qai/ai/frameworks/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 05:30:00.670000 qai_ai-0.5.1/src/qai/ai/frameworks/llama/__init__.py
--rw-r--r--   0        0        0        0 2024-02-17 12:22:07.629593 qai_ai-0.5.1/src/qai/ai/frameworks/llama/assistant.py
--rw-r--r--   0        0        0        0 2024-03-04 02:52:48.502113 qai_ai-0.5.1/src/qai/ai/frameworks/llama/chat.py
--rw-r--r--   0        0        0     1384 2024-03-09 04:42:31.137575 qai_ai-0.5.1/src/qai/ai/frameworks/llama/embeddings.py
--rw-r--r--   0        0        0     7750 2024-05-02 01:23:37.859164 qai_ai-0.5.1/src/qai/ai/frameworks/llama/llama_chroma.py
--rw-r--r--   0        0        0     5099 2024-04-09 04:09:38.373991 qai_ai-0.5.1/src/qai/ai/frameworks/openai/llm.py
--rw-r--r--   0        0        0     1795 2024-02-22 01:07:43.523199 qai_ai-0.5.1/src/qai/ai/llm.py
--rw-r--r--   0        0        0     1355 2024-02-13 05:29:49.384696 qai_ai-0.5.1/src/qai/ai/mock/mock.py
--rw-r--r--   0        0        0        0 2024-02-12 15:43:49.153677 qai_ai-0.5.1/src/qai/ai/prompt/__init__.py
--rw-r--r--   0        0        0     1725 2024-02-12 17:17:06.028769 qai_ai-0.5.1/src/qai/ai/prompt/config.py
--rw-r--r--   0        0        0     8535 2024-02-13 04:07:53.572075 qai_ai-0.5.1/src/qai/ai/prompt/prompt_maker.py
--rw-r--r--   0        0        0     7252 2024-04-26 18:58:22.578528 qai_ai-0.5.1/src/qai/ai/query.py
--rw-r--r--   0        0        0      345 2024-02-11 05:30:15.870302 qai_ai-0.5.1/src/qai/ai/utils/config_utils.py
--rw-r--r--   0        0        0     4619 2024-02-11 05:30:15.870618 qai_ai-0.5.1/src/qai/ai/utils/nltk_extras.py
--rw-r--r--   0        0        0     4376 2024-02-13 23:31:25.728282 qai_ai-0.5.1/src/qai/ai/utils/nltk_utils.py
--rw-r--r--   0        0        0     1641 2024-04-08 11:44:50.258208 qai_ai-0.5.1/src/qai/ai/utils/openai_utils.py
--rw-r--r--   0        0        0      698 2024-02-13 04:36:21.672568 qai_ai-0.5.1/src/qai/ai/utils/token_utils.py
--rw-r--r--   0        0        0      888 2024-02-11 05:30:15.871364 qai_ai-0.5.1/src/qai/ai/utils/validation_utils.py
--rw-r--r--   0        0        0     1107 1970-01-01 00:00:00.000000 qai_ai-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-05-01 22:37:27.943154 qai_ai-0.5.2/README.md
+-rw-r--r--   0        0        0     1474 2024-05-02 01:59:59.546636 qai_ai-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      220 2024-04-08 11:26:06.938861 qai_ai-0.5.2/src/qai/ai/__init__.py
+-rw-r--r--   0        0        0      396 2024-03-06 15:37:18.122377 qai_ai-0.5.2/src/qai/ai/config.py
+-rw-r--r--   0        0        0        0 2024-02-17 11:28:19.525049 qai_ai-0.5.2/src/qai/ai/frameworks/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 05:30:00.670000 qai_ai-0.5.2/src/qai/ai/frameworks/llama/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-17 12:22:07.629593 qai_ai-0.5.2/src/qai/ai/frameworks/llama/assistant.py
+-rw-r--r--   0        0        0        0 2024-03-04 02:52:48.502113 qai_ai-0.5.2/src/qai/ai/frameworks/llama/chat.py
+-rw-r--r--   0        0        0     1384 2024-03-09 04:42:31.137575 qai_ai-0.5.2/src/qai/ai/frameworks/llama/embeddings.py
+-rw-r--r--   0        0        0     7750 2024-05-02 01:23:37.859164 qai_ai-0.5.2/src/qai/ai/frameworks/llama/llama_chroma.py
+-rw-r--r--   0        0        0     5099 2024-04-09 04:09:38.373991 qai_ai-0.5.2/src/qai/ai/frameworks/openai/llm.py
+-rw-r--r--   0        0        0     1795 2024-02-22 01:07:43.523199 qai_ai-0.5.2/src/qai/ai/llm.py
+-rw-r--r--   0        0        0     1355 2024-02-13 05:29:49.384696 qai_ai-0.5.2/src/qai/ai/mock/mock.py
+-rw-r--r--   0        0        0        0 2024-02-12 15:43:49.153677 qai_ai-0.5.2/src/qai/ai/prompt/__init__.py
+-rw-r--r--   0        0        0     1725 2024-02-12 17:17:06.028769 qai_ai-0.5.2/src/qai/ai/prompt/config.py
+-rw-r--r--   0        0        0     8535 2024-02-13 04:07:53.572075 qai_ai-0.5.2/src/qai/ai/prompt/prompt_maker.py
+-rw-r--r--   0        0        0     7252 2024-04-26 18:58:22.578528 qai_ai-0.5.2/src/qai/ai/query.py
+-rw-r--r--   0        0        0      345 2024-02-11 05:30:15.870302 qai_ai-0.5.2/src/qai/ai/utils/config_utils.py
+-rw-r--r--   0        0        0     4619 2024-02-11 05:30:15.870618 qai_ai-0.5.2/src/qai/ai/utils/nltk_extras.py
+-rw-r--r--   0        0        0     4376 2024-02-13 23:31:25.728282 qai_ai-0.5.2/src/qai/ai/utils/nltk_utils.py
+-rw-r--r--   0        0        0     1641 2024-04-08 11:44:50.258208 qai_ai-0.5.2/src/qai/ai/utils/openai_utils.py
+-rw-r--r--   0        0        0      698 2024-02-13 04:36:21.672568 qai_ai-0.5.2/src/qai/ai/utils/token_utils.py
+-rw-r--r--   0        0        0      888 2024-02-11 05:30:15.871364 qai_ai-0.5.2/src/qai/ai/utils/validation_utils.py
+-rw-r--r--   0        0        0     1117 1970-01-01 00:00:00.000000 qai_ai-0.5.2/PKG-INFO
```

### Comparing `qai_ai-0.5.1/pyproject.toml` & `qai_ai-0.5.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.poetry]
 authors = ["parnell <152523161+leeparnell@users.noreply.github.com>"]
-description = ""
+description = "Qai AI API"
 name = "qai-ai"
 packages = [{from = "src", include = "qai"}]
 readme = "README.md"
-version = "0.5.1"
+version = "0.5.2"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 chromadb = "^0.4.22"
 dataclasses-json = "^0.6.4"
 langchain-community = "^0.0.34"
 llama-index = "^0.10.30"
 llama-index-embeddings-huggingface = "^0.2.0"
+llama-index-vector-stores-chroma = "^0.1.7"
 openai = "^1.23.2"
 pandas = "^2.2.1"
 pi-conf = "^0.7.7.5"
 pi-log = "^0.5.7.3"
+qai-storage = "^0.5.0"
 termcolor = "^2.4.0"
-
 torch = [
-    { version = "=2.3.0", source = "pypi", platform = "darwin" },
-    { version = "=2.3.0+cpu", source = "pytorch-cpu-src", platform = "linux" },
-    { version = "=2.3.0+cpu", source = "pytorch-cpu-src", platform = "win32" },
+    {platform = "darwin", source = "pypi", version = "=2.3.0"},
+    {platform = "linux", source = "pytorch-cpu-src", version = "=2.3.0+cpu"},
+    {platform = "win32", source = "pytorch-cpu-src", version = "=2.3.0+cpu"},
 ]
-llama-index-vector-stores-chroma = "^0.1.7"
-qai-storage = "^0.5.0"
 
 [tool.poetry.extras]
 test = ["pytest"]
 
 [[tool.poetry.source]]
 name = "pypi"
 priority = "primary"
 
-
 [[tool.poetry.source]]
 name = "pytorch-gpu-src"
-url = "https://download.pytorch.org/whl/cu118"
 priority = "explicit"
+url = "https://download.pytorch.org/whl/cu118"
 
 [[tool.poetry.source]]
 name = "pytorch-cpu-src"
-url = "https://download.pytorch.org/whl/cpu"
 priority = "explicit"
+url = "https://download.pytorch.org/whl/cpu"
 
 [tool.tomlsort]
 all = true
 in_place = true
 spaces_before_inline_comment = 2  # Match Python PEP 8
 spaces_indent_inline_array = 4  # Match Python PEP 8
 trailing_comma_inline_array = true
```

### Comparing `qai_ai-0.5.1/src/qai/ai/frameworks/llama/embeddings.py` & `qai_ai-0.5.2/src/qai/ai/frameworks/llama/embeddings.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5.1/src/qai/ai/frameworks/llama/llama_chroma.py` & `qai_ai-0.5.2/src/qai/ai/frameworks/llama/llama_chroma.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5.1/src/qai/ai/frameworks/openai/llm.py` & `qai_ai-0.5.2/src/qai/ai/frameworks/openai/llm.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5.1/src/qai/ai/llm.py` & `qai_ai-0.5.2/src/qai/ai/llm.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5.1/src/qai/ai/mock/mock.py` & `qai_ai-0.5.2/src/qai/ai/mock/mock.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5.1/src/qai/ai/prompt/config.py` & `qai_ai-0.5.2/src/qai/ai/prompt/config.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5.1/src/qai/ai/prompt/prompt_maker.py` & `qai_ai-0.5.2/src/qai/ai/prompt/prompt_maker.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5.1/src/qai/ai/query.py` & `qai_ai-0.5.2/src/qai/ai/query.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5.1/src/qai/ai/utils/nltk_extras.py` & `qai_ai-0.5.2/src/qai/ai/utils/nltk_extras.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5.1/src/qai/ai/utils/nltk_utils.py` & `qai_ai-0.5.2/src/qai/ai/utils/nltk_utils.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5.1/src/qai/ai/utils/openai_utils.py` & `qai_ai-0.5.2/src/qai/ai/utils/openai_utils.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5.1/src/qai/ai/utils/token_utils.py` & `qai_ai-0.5.2/src/qai/ai/utils/token_utils.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5.1/src/qai/ai/utils/validation_utils.py` & `qai_ai-0.5.2/src/qai/ai/utils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5.1/PKG-INFO` & `qai_ai-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: qai-ai
-Version: 0.5.1
-Summary: 
+Version: 0.5.2
+Summary: Qai AI API
 Author: parnell
 Author-email: 152523161+leeparnell@users.noreply.github.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: test
 Requires-Dist: chromadb (>=0.4.22,<0.5.0)
```

