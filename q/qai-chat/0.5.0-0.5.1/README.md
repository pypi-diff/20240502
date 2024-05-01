# Comparing `tmp/qai_chat-0.5.0.tar.gz` & `tmp/qai_chat-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qai_chat-0.5.0.tar", max compression
+gzip compressed data, was "qai_chat-0.5.1.tar", max compression
```

## Comparing `qai_chat-0.5.0.tar` & `qai_chat-0.5.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      770 2024-02-11 05:47:17.579886 qai_chat-0.5.0/README.md
--rw-r--r--   0        0        0     1462 2024-05-01 22:46:44.726018 qai_chat-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      119 2024-04-19 22:20:22.144347 qai_chat-0.5.0/src/qai/chat/__init__.py
--rw-r--r--   0        0        0        0 2024-02-11 05:30:15.847105 qai_chat-0.5.0/src/qai/chat/aws/__init__.py
--rw-r--r--   0        0        0     3806 2024-05-01 22:34:43.059574 qai_chat-0.5.0/src/qai/chat/chat.py
--rw-r--r--   0        0        0       58 2024-05-01 22:35:47.322687 qai_chat-0.5.0/src/qai/chat/config.py
--rw-r--r--   0        0        0      130 2024-02-11 22:06:12.219783 qai_chat-0.5.0/src/qai/chat/db/__init__.py
--rw-r--r--   0        0        0     4275 2024-04-19 22:20:28.377648 qai_chat-0.5.0/src/qai/chat/db/chroma/chroma.py
--rw-r--r--   0        0        0     2131 2024-02-28 17:58:43.228750 qai_chat-0.5.0/src/qai/chat/db/chroma/chroma_loader.py
--rw-r--r--   0        0        0      323 2024-02-11 05:30:15.853308 qai_chat-0.5.0/src/qai/chat/db/retriever.py
--rw-r--r--   0        0        0      316 2024-02-28 19:01:14.113345 qai_chat-0.5.0/src/qai/chat/db/retriever_factory.py
--rw-r--r--   0        0        0        0 2024-02-26 04:45:15.519842 qai_chat-0.5.0/src/qai/chat/facts/__init__.py
--rw-r--r--   0        0        0        0 2024-02-11 05:30:15.853779 qai_chat-0.5.0/src/qai/chat/layers/__init__.py
--rw-r--r--   0        0        0     1346 2024-02-13 23:30:27.419212 qai_chat-0.5.0/src/qai/chat/layers/chatbot.py
--rw-r--r--   0        0        0      205 2024-02-11 05:30:15.856223 qai_chat-0.5.0/src/qai/chat/layers/fact_table/__init__.py
--rw-r--r--   0        0        0      499 2024-02-11 21:52:50.873809 qai_chat-0.5.0/src/qai/chat/layers/fact_table/fact.py
--rw-r--r--   0        0        0     2964 2024-05-01 22:35:17.803029 qai_chat-0.5.0/src/qai/chat/layers/fact_table/factory.py
--rw-r--r--   0        0        0      781 2024-02-12 05:43:51.403892 qai_chat-0.5.0/src/qai/chat/layers/fact_table/table.py
--rw-r--r--   0        0        0     1887 2024-02-13 23:30:41.328422 qai_chat-0.5.0/src/qai/chat/layers/factory.py
--rw-r--r--   0        0        0     1587 2024-02-11 22:05:46.765875 qai_chat-0.5.0/src/qai/chat/layers/layer.py
--rw-r--r--   0        0        0        0 2024-02-11 05:30:15.859258 qai_chat-0.5.0/src/qai/chat/layers/llm/__init__.py
--rw-r--r--   0        0        0    14278 2024-04-02 15:08:04.409859 qai_chat-0.5.0/src/qai/chat/layers/llm/assistant/assistant.py
--rw-r--r--   0        0        0     2079 2024-02-11 05:30:15.862778 qai_chat-0.5.0/src/qai/chat/layers/llm/assistant/assistant_schema.py
--rw-r--r--   0        0        0     3869 2024-02-11 05:30:15.863025 qai_chat-0.5.0/src/qai/chat/layers/llm/assistant/assistant_tools.py
--rw-r--r--   0        0        0     8637 2024-05-01 22:44:59.208784 qai_chat-0.5.0/src/qai/chat/layers/llm/chatbot.py
--rw-r--r--   0        0        0      674 2024-02-13 23:32:19.460110 qai_chat-0.5.0/src/qai/chat/layers/llm/factory.py
--rw-r--r--   0        0        0     5211 2024-02-12 17:16:41.539512 qai_chat-0.5.0/src/qai/chat/layers/query.py
--rw-r--r--   0        0        0      226 2024-05-01 02:29:19.270926 qai_chat-0.5.0/src/qai/chat/models.py
--rw-r--r--   0        0        0        0 2024-02-11 05:30:15.864611 qai_chat-0.5.0/src/qai/chat/prompt/__init__.py
--rw-r--r--   0        0        0     1725 2024-02-11 05:30:15.866700 qai_chat-0.5.0/src/qai/chat/prompt/config.py
--rw-r--r--   0        0        0     8647 2024-05-01 22:43:50.812909 qai_chat-0.5.0/src/qai/chat/prompt/prompt_maker.py
--rw-r--r--   0        0        0      642 2024-02-11 05:30:15.867537 qai_chat-0.5.0/src/qai/chat/prompts.py
--rw-r--r--   0        0        0     1577 1970-01-01 00:00:00.000000 qai_chat-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2024-05-01 22:47:30.841205 qai_chat-0.5.1/README.md
+-rw-r--r--   0        0        0     1462 2024-05-01 22:47:38.316118 qai_chat-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      119 2024-04-19 22:20:22.144347 qai_chat-0.5.1/src/qai/chat/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-11 05:30:15.847105 qai_chat-0.5.1/src/qai/chat/aws/__init__.py
+-rw-r--r--   0        0        0     3806 2024-05-01 22:34:43.059574 qai_chat-0.5.1/src/qai/chat/chat.py
+-rw-r--r--   0        0        0       58 2024-05-01 22:35:47.322687 qai_chat-0.5.1/src/qai/chat/config.py
+-rw-r--r--   0        0        0      130 2024-02-11 22:06:12.219783 qai_chat-0.5.1/src/qai/chat/db/__init__.py
+-rw-r--r--   0        0        0     4275 2024-04-19 22:20:28.377648 qai_chat-0.5.1/src/qai/chat/db/chroma/chroma.py
+-rw-r--r--   0        0        0     2131 2024-02-28 17:58:43.228750 qai_chat-0.5.1/src/qai/chat/db/chroma/chroma_loader.py
+-rw-r--r--   0        0        0      323 2024-02-11 05:30:15.853308 qai_chat-0.5.1/src/qai/chat/db/retriever.py
+-rw-r--r--   0        0        0      316 2024-02-28 19:01:14.113345 qai_chat-0.5.1/src/qai/chat/db/retriever_factory.py
+-rw-r--r--   0        0        0        0 2024-02-26 04:45:15.519842 qai_chat-0.5.1/src/qai/chat/facts/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-11 05:30:15.853779 qai_chat-0.5.1/src/qai/chat/layers/__init__.py
+-rw-r--r--   0        0        0     1346 2024-02-13 23:30:27.419212 qai_chat-0.5.1/src/qai/chat/layers/chatbot.py
+-rw-r--r--   0        0        0      205 2024-02-11 05:30:15.856223 qai_chat-0.5.1/src/qai/chat/layers/fact_table/__init__.py
+-rw-r--r--   0        0        0      499 2024-02-11 21:52:50.873809 qai_chat-0.5.1/src/qai/chat/layers/fact_table/fact.py
+-rw-r--r--   0        0        0     2964 2024-05-01 22:35:17.803029 qai_chat-0.5.1/src/qai/chat/layers/fact_table/factory.py
+-rw-r--r--   0        0        0      781 2024-02-12 05:43:51.403892 qai_chat-0.5.1/src/qai/chat/layers/fact_table/table.py
+-rw-r--r--   0        0        0     1887 2024-02-13 23:30:41.328422 qai_chat-0.5.1/src/qai/chat/layers/factory.py
+-rw-r--r--   0        0        0     1587 2024-02-11 22:05:46.765875 qai_chat-0.5.1/src/qai/chat/layers/layer.py
+-rw-r--r--   0        0        0        0 2024-02-11 05:30:15.859258 qai_chat-0.5.1/src/qai/chat/layers/llm/__init__.py
+-rw-r--r--   0        0        0    14278 2024-04-02 15:08:04.409859 qai_chat-0.5.1/src/qai/chat/layers/llm/assistant/assistant.py
+-rw-r--r--   0        0        0     2079 2024-02-11 05:30:15.862778 qai_chat-0.5.1/src/qai/chat/layers/llm/assistant/assistant_schema.py
+-rw-r--r--   0        0        0     3869 2024-02-11 05:30:15.863025 qai_chat-0.5.1/src/qai/chat/layers/llm/assistant/assistant_tools.py
+-rw-r--r--   0        0        0     8637 2024-05-01 22:44:59.208784 qai_chat-0.5.1/src/qai/chat/layers/llm/chatbot.py
+-rw-r--r--   0        0        0      674 2024-02-13 23:32:19.460110 qai_chat-0.5.1/src/qai/chat/layers/llm/factory.py
+-rw-r--r--   0        0        0     5211 2024-02-12 17:16:41.539512 qai_chat-0.5.1/src/qai/chat/layers/query.py
+-rw-r--r--   0        0        0      226 2024-05-01 02:29:19.270926 qai_chat-0.5.1/src/qai/chat/models.py
+-rw-r--r--   0        0        0        0 2024-02-11 05:30:15.864611 qai_chat-0.5.1/src/qai/chat/prompt/__init__.py
+-rw-r--r--   0        0        0     1725 2024-02-11 05:30:15.866700 qai_chat-0.5.1/src/qai/chat/prompt/config.py
+-rw-r--r--   0        0        0     8647 2024-05-01 22:43:50.812909 qai_chat-0.5.1/src/qai/chat/prompt/prompt_maker.py
+-rw-r--r--   0        0        0      642 2024-02-11 05:30:15.867537 qai_chat-0.5.1/src/qai/chat/prompts.py
+-rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 qai_chat-0.5.1/PKG-INFO
```

### Comparing `qai_chat-0.5.0/pyproject.toml` & `qai_chat-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.poetry]
 authors = ["parnell <152523161+leeparnell@users.noreply.github.com>"]
 description = ""
 name = "qai-chat"
 packages = [{from = "src", include = "qai"}]
 readme = "README.md"
-version = "0.5.0"
+version = "0.5.1"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
 flask = "^3.0.3"
 llama-index = "^0.10.30"
 llama-index-llms-openai = "^0.1.16"
 llama-index-vector-stores-chroma = "^0.1.6"
```

### Comparing `qai_chat-0.5.0/src/qai/chat/chat.py` & `qai_chat-0.5.1/src/qai/chat/chat.py`

 * *Files identical despite different names*

### Comparing `qai_chat-0.5.0/src/qai/chat/db/chroma/chroma.py` & `qai_chat-0.5.1/src/qai/chat/db/chroma/chroma.py`

 * *Files identical despite different names*

### Comparing `qai_chat-0.5.0/src/qai/chat/db/chroma/chroma_loader.py` & `qai_chat-0.5.1/src/qai/chat/db/chroma/chroma_loader.py`

 * *Files identical despite different names*

### Comparing `qai_chat-0.5.0/src/qai/chat/layers/chatbot.py` & `qai_chat-0.5.1/src/qai/chat/layers/chatbot.py`

 * *Files identical despite different names*

### Comparing `qai_chat-0.5.0/src/qai/chat/layers/fact_table/factory.py` & `qai_chat-0.5.1/src/qai/chat/layers/fact_table/factory.py`

 * *Files identical despite different names*

### Comparing `qai_chat-0.5.0/src/qai/chat/layers/fact_table/table.py` & `qai_chat-0.5.1/src/qai/chat/layers/fact_table/table.py`

 * *Files identical despite different names*

### Comparing `qai_chat-0.5.0/src/qai/chat/layers/factory.py` & `qai_chat-0.5.1/src/qai/chat/layers/factory.py`

 * *Files identical despite different names*

### Comparing `qai_chat-0.5.0/src/qai/chat/layers/layer.py` & `qai_chat-0.5.1/src/qai/chat/layers/layer.py`

 * *Files identical despite different names*

### Comparing `qai_chat-0.5.0/src/qai/chat/layers/llm/assistant/assistant.py` & `qai_chat-0.5.1/src/qai/chat/layers/llm/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `qai_chat-0.5.0/src/qai/chat/layers/llm/assistant/assistant_schema.py` & `qai_chat-0.5.1/src/qai/chat/layers/llm/assistant/assistant_schema.py`

 * *Files identical despite different names*

### Comparing `qai_chat-0.5.0/src/qai/chat/layers/llm/assistant/assistant_tools.py` & `qai_chat-0.5.1/src/qai/chat/layers/llm/assistant/assistant_tools.py`

 * *Files identical despite different names*

### Comparing `qai_chat-0.5.0/src/qai/chat/layers/llm/chatbot.py` & `qai_chat-0.5.1/src/qai/chat/layers/llm/chatbot.py`

 * *Files identical despite different names*

### Comparing `qai_chat-0.5.0/src/qai/chat/layers/llm/factory.py` & `qai_chat-0.5.1/src/qai/chat/layers/llm/factory.py`

 * *Files identical despite different names*

### Comparing `qai_chat-0.5.0/src/qai/chat/layers/query.py` & `qai_chat-0.5.1/src/qai/chat/layers/query.py`

 * *Files identical despite different names*

### Comparing `qai_chat-0.5.0/src/qai/chat/prompt/config.py` & `qai_chat-0.5.1/src/qai/chat/prompt/config.py`

 * *Files identical despite different names*

### Comparing `qai_chat-0.5.0/src/qai/chat/prompt/prompt_maker.py` & `qai_chat-0.5.1/src/qai/chat/prompt/prompt_maker.py`

 * *Files identical despite different names*

### Comparing `qai_chat-0.5.0/src/qai/chat/prompts.py` & `qai_chat-0.5.1/src/qai/chat/prompts.py`

 * *Files identical despite different names*

