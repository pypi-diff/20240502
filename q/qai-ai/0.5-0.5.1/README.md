# Comparing `tmp/qai_ai-0.5.tar.gz` & `tmp/qai_ai-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qai_ai-0.5.tar", max compression
+gzip compressed data, was "qai_ai-0.5.1.tar", max compression
```

## Comparing `qai_ai-0.5.tar` & `qai_ai-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       23 2024-05-01 22:37:27.943154 qai_ai-0.5/README.md
--rw-r--r--   0        0        0     1431 2024-05-01 22:38:16.585501 qai_ai-0.5/pyproject.toml
--rw-r--r--   0        0        0      220 2024-04-08 11:26:06.938861 qai_ai-0.5/src/qai/ai/__init__.py
--rw-r--r--   0        0        0      396 2024-03-06 15:37:18.122377 qai_ai-0.5/src/qai/ai/config.py
--rw-r--r--   0        0        0        0 2024-02-17 11:28:19.525049 qai_ai-0.5/src/qai/ai/frameworks/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 05:30:00.670000 qai_ai-0.5/src/qai/ai/frameworks/llama/__init__.py
--rw-r--r--   0        0        0        0 2024-02-17 12:22:07.629593 qai_ai-0.5/src/qai/ai/frameworks/llama/assistant.py
--rw-r--r--   0        0        0        0 2024-03-04 02:52:48.502113 qai_ai-0.5/src/qai/ai/frameworks/llama/chat.py
--rw-r--r--   0        0        0     1384 2024-03-09 04:42:31.137575 qai_ai-0.5/src/qai/ai/frameworks/llama/embeddings.py
--rw-r--r--   0        0        0     7750 2024-03-10 12:45:42.466531 qai_ai-0.5/src/qai/ai/frameworks/llama/llama_chroma.py
--rw-r--r--   0        0        0     5099 2024-04-09 04:09:38.373991 qai_ai-0.5/src/qai/ai/frameworks/openai/llm.py
--rw-r--r--   0        0        0     1795 2024-02-22 01:07:43.523199 qai_ai-0.5/src/qai/ai/llm.py
--rw-r--r--   0        0        0     1355 2024-02-13 05:29:49.384696 qai_ai-0.5/src/qai/ai/mock/mock.py
--rw-r--r--   0        0        0        0 2024-02-12 15:43:49.153677 qai_ai-0.5/src/qai/ai/prompt/__init__.py
--rw-r--r--   0        0        0     1725 2024-02-12 17:17:06.028769 qai_ai-0.5/src/qai/ai/prompt/config.py
--rw-r--r--   0        0        0     8535 2024-02-13 04:07:53.572075 qai_ai-0.5/src/qai/ai/prompt/prompt_maker.py
--rw-r--r--   0        0        0     7252 2024-04-26 18:58:22.578528 qai_ai-0.5/src/qai/ai/query.py
--rw-r--r--   0        0        0      345 2024-02-11 05:30:15.870302 qai_ai-0.5/src/qai/ai/utils/config_utils.py
--rw-r--r--   0        0        0     4619 2024-02-11 05:30:15.870618 qai_ai-0.5/src/qai/ai/utils/nltk_extras.py
--rw-r--r--   0        0        0     4376 2024-02-13 23:31:25.728282 qai_ai-0.5/src/qai/ai/utils/nltk_utils.py
--rw-r--r--   0        0        0     1641 2024-04-08 11:44:50.258208 qai_ai-0.5/src/qai/ai/utils/openai_utils.py
--rw-r--r--   0        0        0      698 2024-02-13 04:36:21.672568 qai_ai-0.5/src/qai/ai/utils/token_utils.py
--rw-r--r--   0        0        0      888 2024-02-11 05:30:15.871364 qai_ai-0.5/src/qai/ai/utils/validation_utils.py
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 qai_ai-0.5/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-05-01 22:37:27.943154 qai_ai-0.5.1/README.md
+-rw-r--r--   0        0        0     1472 2024-05-02 01:45:25.724783 qai_ai-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      220 2024-04-08 11:26:06.938861 qai_ai-0.5.1/src/qai/ai/__init__.py
+-rw-r--r--   0        0        0      396 2024-03-06 15:37:18.122377 qai_ai-0.5.1/src/qai/ai/config.py
+-rw-r--r--   0        0        0        0 2024-02-17 11:28:19.525049 qai_ai-0.5.1/src/qai/ai/frameworks/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 05:30:00.670000 qai_ai-0.5.1/src/qai/ai/frameworks/llama/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-17 12:22:07.629593 qai_ai-0.5.1/src/qai/ai/frameworks/llama/assistant.py
+-rw-r--r--   0        0        0        0 2024-03-04 02:52:48.502113 qai_ai-0.5.1/src/qai/ai/frameworks/llama/chat.py
+-rw-r--r--   0        0        0     1384 2024-03-09 04:42:31.137575 qai_ai-0.5.1/src/qai/ai/frameworks/llama/embeddings.py
+-rw-r--r--   0        0        0     7750 2024-05-02 01:23:37.859164 qai_ai-0.5.1/src/qai/ai/frameworks/llama/llama_chroma.py
+-rw-r--r--   0        0        0     5099 2024-04-09 04:09:38.373991 qai_ai-0.5.1/src/qai/ai/frameworks/openai/llm.py
+-rw-r--r--   0        0        0     1795 2024-02-22 01:07:43.523199 qai_ai-0.5.1/src/qai/ai/llm.py
+-rw-r--r--   0        0        0     1355 2024-02-13 05:29:49.384696 qai_ai-0.5.1/src/qai/ai/mock/mock.py
+-rw-r--r--   0        0        0        0 2024-02-12 15:43:49.153677 qai_ai-0.5.1/src/qai/ai/prompt/__init__.py
+-rw-r--r--   0        0        0     1725 2024-02-12 17:17:06.028769 qai_ai-0.5.1/src/qai/ai/prompt/config.py
+-rw-r--r--   0        0        0     8535 2024-02-13 04:07:53.572075 qai_ai-0.5.1/src/qai/ai/prompt/prompt_maker.py
+-rw-r--r--   0        0        0     7252 2024-04-26 18:58:22.578528 qai_ai-0.5.1/src/qai/ai/query.py
+-rw-r--r--   0        0        0      345 2024-02-11 05:30:15.870302 qai_ai-0.5.1/src/qai/ai/utils/config_utils.py
+-rw-r--r--   0        0        0     4619 2024-02-11 05:30:15.870618 qai_ai-0.5.1/src/qai/ai/utils/nltk_extras.py
+-rw-r--r--   0        0        0     4376 2024-02-13 23:31:25.728282 qai_ai-0.5.1/src/qai/ai/utils/nltk_utils.py
+-rw-r--r--   0        0        0     1641 2024-04-08 11:44:50.258208 qai_ai-0.5.1/src/qai/ai/utils/openai_utils.py
+-rw-r--r--   0        0        0      698 2024-02-13 04:36:21.672568 qai_ai-0.5.1/src/qai/ai/utils/token_utils.py
+-rw-r--r--   0        0        0      888 2024-02-11 05:30:15.871364 qai_ai-0.5.1/src/qai/ai/utils/validation_utils.py
+-rw-r--r--   0        0        0     1107 1970-01-01 00:00:00.000000 qai_ai-0.5.1/PKG-INFO
```

### Comparing `qai_ai-0.5/src/qai/ai/frameworks/llama/embeddings.py` & `qai_ai-0.5.1/src/qai/ai/frameworks/llama/embeddings.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5/src/qai/ai/frameworks/llama/llama_chroma.py` & `qai_ai-0.5.1/src/qai/ai/frameworks/llama/llama_chroma.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5/src/qai/ai/frameworks/openai/llm.py` & `qai_ai-0.5.1/src/qai/ai/frameworks/openai/llm.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5/src/qai/ai/llm.py` & `qai_ai-0.5.1/src/qai/ai/llm.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5/src/qai/ai/mock/mock.py` & `qai_ai-0.5.1/src/qai/ai/mock/mock.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5/src/qai/ai/prompt/config.py` & `qai_ai-0.5.1/src/qai/ai/prompt/config.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5/src/qai/ai/prompt/prompt_maker.py` & `qai_ai-0.5.1/src/qai/ai/prompt/prompt_maker.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5/src/qai/ai/query.py` & `qai_ai-0.5.1/src/qai/ai/query.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5/src/qai/ai/utils/nltk_extras.py` & `qai_ai-0.5.1/src/qai/ai/utils/nltk_extras.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5/src/qai/ai/utils/nltk_utils.py` & `qai_ai-0.5.1/src/qai/ai/utils/nltk_utils.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5/src/qai/ai/utils/openai_utils.py` & `qai_ai-0.5.1/src/qai/ai/utils/openai_utils.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5/src/qai/ai/utils/token_utils.py` & `qai_ai-0.5.1/src/qai/ai/utils/token_utils.py`

 * *Files identical despite different names*

### Comparing `qai_ai-0.5/src/qai/ai/utils/validation_utils.py` & `qai_ai-0.5.1/src/qai/ai/utils/validation_utils.py`

 * *Files identical despite different names*

