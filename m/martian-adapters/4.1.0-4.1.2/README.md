# Comparing `tmp/martian_adapters-4.1.0.tar.gz` & `tmp/martian_adapters-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martian_adapters-4.1.0.tar", max compression
+gzip compressed data, was "martian_adapters-4.1.2.tar", max compression
```

## Comparing `martian_adapters-4.1.0.tar` & `martian_adapters-4.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    35149 2024-04-30 00:30:40.565520 martian_adapters-4.1.0/LICENSE
--rw-r--r--   0        0        0     3452 2024-05-01 00:14:43.669585 martian_adapters-4.1.0/README.md
--rw-r--r--   0        0        0      725 2024-04-24 23:08:19.279531 martian_adapters-4.1.0/adapters/__init__.py
--rw-r--r--   0        0        0      305 2024-03-12 21:13:48.732102 martian_adapters-4.1.0/adapters/abstract_adapters/__init__.py
--rw-r--r--   0        0        0     2117 2024-02-06 20:08:59.742583 martian_adapters-4.1.0/adapters/abstract_adapters/api_key_adapter_mixin.py
--rw-r--r--   0        0        0     3347 2024-04-25 03:58:20.005866 martian_adapters-4.1.0/adapters/abstract_adapters/base_adapter.py
--rw-r--r--   0        0        0     1226 2024-03-15 23:53:07.585309 martian_adapters-4.1.0/adapters/abstract_adapters/chat_http_api_adapter.py
--rw-r--r--   0        0        0     7525 2024-04-01 03:49:11.566774 martian_adapters-4.1.0/adapters/abstract_adapters/http_api_adapter_mixin.py
--rw-r--r--   0        0        0     2386 2024-04-24 23:08:19.280106 martian_adapters-4.1.0/adapters/abstract_adapters/openai_sdk_chat_adapter.py
--rw-r--r--   0        0        0     3419 2024-04-25 03:58:20.006328 martian_adapters-4.1.0/adapters/abstract_adapters/provider_adapter_mixin.py
--rw-r--r--   0        0        0     5816 2024-04-25 03:58:20.007161 martian_adapters-4.1.0/adapters/abstract_adapters/sdk_chat_adapter.py
--rw-r--r--   0        0        0     5812 2024-04-25 03:58:20.007536 martian_adapters-4.1.0/adapters/adapter_factory.py
--rw-r--r--   0        0        0       59 2024-03-12 21:13:48.733334 martian_adapters-4.1.0/adapters/concrete_adapters/__init__.py
--rw-r--r--   0        0        0     3429 2024-04-24 23:08:19.282029 martian_adapters-4.1.0/adapters/concrete_adapters/you_com_rag_chat_adapter.py
--rw-r--r--   0        0        0      942 2024-04-25 21:01:54.033018 martian_adapters-4.1.0/adapters/provider_adapters/__init__.py
--rw-r--r--   0        0        0     9225 2024-04-25 03:58:20.008865 martian_adapters-4.1.0/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     4102 2024-05-01 00:33:38.184553 martian_adapters-4.1.0/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2053 2024-04-25 03:58:20.009535 martian_adapters-4.1.0/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1203 2024-04-26 19:57:14.024569 martian_adapters-4.1.0/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     7317 2024-04-29 21:51:04.769723 martian_adapters-4.1.0/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1663 2024-04-24 23:08:19.283717 martian_adapters-4.1.0/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1757 2024-04-25 03:58:20.009986 martian_adapters-4.1.0/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1331 2024-04-25 21:01:54.034177 martian_adapters-4.1.0/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     4444 2024-05-01 00:14:43.670186 martian_adapters-4.1.0/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     1425 2024-04-25 21:01:54.034673 martian_adapters-4.1.0/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0     2307 2024-03-15 23:53:07.590557 martian_adapters-4.1.0/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0    10017 2024-04-25 21:01:54.035420 martian_adapters-4.1.0/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
--rw-r--r--   0        0        0        0 2023-11-30 19:57:07.662865 martian_adapters-4.1.0/adapters/py.typed
--rw-r--r--   0        0        0      558 2024-02-06 20:08:59.751016 martian_adapters-4.1.0/adapters/rate_limiter.py
--rw-r--r--   0        0        0      334 2024-02-06 20:08:59.751444 martian_adapters-4.1.0/adapters/requirements.txt
--rw-r--r--   0        0        0     6903 2024-04-25 03:58:20.012283 martian_adapters-4.1.0/adapters/types.py
--rw-r--r--   0        0        0        0 2023-11-09 21:00:33.698900 martian_adapters-4.1.0/adapters/utils/__init__.py
--rw-r--r--   0        0        0      263 2024-04-24 23:08:19.285444 martian_adapters-4.1.0/adapters/utils/adapter_stream_response.py
--rw-r--r--   0        0        0     1064 2024-03-12 21:13:48.734260 martian_adapters-4.1.0/adapters/utils/general_utils.py
--rw-r--r--   0        0        0     2492 2024-03-08 00:01:49.626651 martian_adapters-4.1.0/adapters/utils/network_utils.py
--rw-r--r--   0        0        0     8173 2024-04-24 23:08:19.285987 martian_adapters-4.1.0/adapters/utils/openai_client_factory.py
--rw-r--r--   0        0        0     1170 2024-05-01 00:33:24.871044 martian_adapters-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     4851 1970-01-01 00:00:00.000000 martian_adapters-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/LICENSE
+-rw-r--r--   0        0        0     3452 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/README.md
+-rw-r--r--   0        0        0      725 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/__init__.py
+-rw-r--r--   0        0        0      305 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/abstract_adapters/__init__.py
+-rw-r--r--   0        0        0     2117 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/abstract_adapters/api_key_adapter_mixin.py
+-rw-r--r--   0        0        0     3347 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/abstract_adapters/base_adapter.py
+-rw-r--r--   0        0        0     1226 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/abstract_adapters/chat_http_api_adapter.py
+-rw-r--r--   0        0        0     7525 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/abstract_adapters/http_api_adapter_mixin.py
+-rw-r--r--   0        0        0     2386 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/abstract_adapters/openai_sdk_chat_adapter.py
+-rw-r--r--   0        0        0     3419 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/abstract_adapters/provider_adapter_mixin.py
+-rw-r--r--   0        0        0     5816 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/abstract_adapters/sdk_chat_adapter.py
+-rw-r--r--   0        0        0     5812 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/adapter_factory.py
+-rw-r--r--   0        0        0       59 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/concrete_adapters/__init__.py
+-rw-r--r--   0        0        0     3429 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/concrete_adapters/you_com_rag_chat_adapter.py
+-rw-r--r--   0        0        0      942 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/__init__.py
+-rw-r--r--   0        0        0     9225 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     4102 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2053 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1203 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     7317 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1663 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1757 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1331 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     4444 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     1425 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0     2307 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0    10017 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/provider_adapters/together_sdk_chat_provider_adapter.py
+-rw-r--r--   0        0        0        0 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/py.typed
+-rw-r--r--   0        0        0      558 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/rate_limiter.py
+-rw-r--r--   0        0        0      335 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/requirements.txt
+-rw-r--r--   0        0        0     6903 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/types.py
+-rw-r--r--   0        0        0        0 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/utils/__init__.py
+-rw-r--r--   0        0        0      263 2024-05-01 23:43:58.597538 martian_adapters-4.1.2/adapters/utils/adapter_stream_response.py
+-rw-r--r--   0        0        0     1064 2024-05-01 23:43:58.601538 martian_adapters-4.1.2/adapters/utils/general_utils.py
+-rw-r--r--   0        0        0     2492 2024-05-01 23:43:58.601538 martian_adapters-4.1.2/adapters/utils/network_utils.py
+-rw-r--r--   0        0        0     8173 2024-05-01 23:43:58.601538 martian_adapters-4.1.2/adapters/utils/openai_client_factory.py
+-rw-r--r--   0        0        0     1170 2024-05-01 23:43:58.601538 martian_adapters-4.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4800 1970-01-01 00:00:00.000000 martian_adapters-4.1.2/PKG-INFO
```

### Comparing `martian_adapters-4.1.0/LICENSE` & `martian_adapters-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/README.md` & `martian_adapters-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/__init__.py` & `martian_adapters-4.1.2/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/abstract_adapters/api_key_adapter_mixin.py` & `martian_adapters-4.1.2/adapters/abstract_adapters/api_key_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/abstract_adapters/base_adapter.py` & `martian_adapters-4.1.2/adapters/abstract_adapters/base_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/abstract_adapters/chat_http_api_adapter.py` & `martian_adapters-4.1.2/adapters/abstract_adapters/chat_http_api_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/abstract_adapters/http_api_adapter_mixin.py` & `martian_adapters-4.1.2/adapters/abstract_adapters/http_api_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/abstract_adapters/openai_sdk_chat_adapter.py` & `martian_adapters-4.1.2/adapters/abstract_adapters/openai_sdk_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/abstract_adapters/provider_adapter_mixin.py` & `martian_adapters-4.1.2/adapters/abstract_adapters/provider_adapter_mixin.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/abstract_adapters/sdk_chat_adapter.py` & `martian_adapters-4.1.2/adapters/abstract_adapters/sdk_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/adapter_factory.py` & `martian_adapters-4.1.2/adapters/adapter_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/concrete_adapters/you_com_rag_chat_adapter.py` & `martian_adapters-4.1.2/adapters/concrete_adapters/you_com_rag_chat_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/provider_adapters/__init__.py` & `martian_adapters-4.1.2/adapters/provider_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py` & `martian_adapters-4.1.2/adapters/provider_adapters/anthropic_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py` & `martian_adapters-4.1.2/adapters/provider_adapters/anyscale_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py` & `martian_adapters-4.1.2/adapters/provider_adapters/deepinfra_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py` & `martian_adapters-4.1.2/adapters/provider_adapters/fireworks_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py` & `martian_adapters-4.1.2/adapters/provider_adapters/gemini_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py` & `martian_adapters-4.1.2/adapters/provider_adapters/groq_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py` & `martian_adapters-4.1.2/adapters/provider_adapters/moonshot_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py` & `martian_adapters-4.1.2/adapters/provider_adapters/octoai_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py` & `martian_adapters-4.1.2/adapters/provider_adapters/openai_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py` & `martian_adapters-4.1.2/adapters/provider_adapters/openrouter_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py` & `martian_adapters-4.1.2/adapters/provider_adapters/perplexity_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/provider_adapters/together_sdk_chat_provider_adapter.py` & `martian_adapters-4.1.2/adapters/provider_adapters/together_sdk_chat_provider_adapter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/rate_limiter.py` & `martian_adapters-4.1.2/adapters/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/types.py` & `martian_adapters-4.1.2/adapters/types.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/utils/general_utils.py` & `martian_adapters-4.1.2/adapters/utils/general_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/utils/network_utils.py` & `martian_adapters-4.1.2/adapters/utils/network_utils.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/adapters/utils/openai_client_factory.py` & `martian_adapters-4.1.2/adapters/utils/openai_client_factory.py`

 * *Files identical despite different names*

### Comparing `martian_adapters-4.1.0/pyproject.toml` & `martian_adapters-4.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "martian-adapters"
-version = "4.1.0"
+version = "4.1.2"
 description = "Adapters as API gateways to Different LLM Models"
 authors = ["Martian team <team@withmartian.com>"]
 readme = "README.md"
 packages = [{include = "adapters", from = "."}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `martian_adapters-4.1.0/PKG-INFO` & `martian_adapters-4.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: martian-adapters
-Version: 4.1.0
+Version: 4.1.2
 Summary: Adapters as API gateways to Different LLM Models
 Author: Martian team
 Author-email: team@withmartian.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
 Requires-Dist: aiolimiter (>=1.1.0,<2.0.0)
 Requires-Dist: aiosignal (>=1.3.1,<2.0.0)
 Requires-Dist: anthropic (==0.16.0)
 Requires-Dist: async-timeout (>=4.0.3,<5.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: attrs (>=23.1.0,<24.0.0)
```

