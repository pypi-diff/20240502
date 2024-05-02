# Comparing `tmp/openlit-1.1.1.tar.gz` & `tmp/openlit-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlit-1.1.1.tar", max compression
+gzip compressed data, was "openlit-1.1.2.tar", max compression
```

## Comparing `openlit-1.1.1.tar` & `openlit-1.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    11357 2024-05-02 06:30:25.575605 openlit-1.1.1/LICENSE
--rw-r--r--   0        0        0     9235 2024-05-02 06:30:25.575605 openlit-1.1.1/README.md
--rw-r--r--   0        0        0      966 2024-05-02 06:30:25.575605 openlit-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     4651 2024-05-02 06:30:25.575605 openlit-1.1.1/src/openlit/__helpers.py
--rw-r--r--   0        0        0     8931 2024-05-02 06:30:25.575605 openlit-1.1.1/src/openlit/__init__.py
--rw-r--r--   0        0        0     1955 2024-05-02 06:30:25.575605 openlit-1.1.1/src/openlit/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0    15993 2024-05-02 06:30:25.575605 openlit-1.1.1/src/openlit/instrumentation/anthropic/anthropic.py
--rw-r--r--   0        0        0    16035 2024-05-02 06:30:25.575605 openlit-1.1.1/src/openlit/instrumentation/anthropic/async_anthropic.py
--rw-r--r--   0        0        0     1540 2024-05-02 06:30:25.575605 openlit-1.1.1/src/openlit/instrumentation/bedrock/__init__.py
--rw-r--r--   0        0        0    22278 2024-05-02 06:30:25.575605 openlit-1.1.1/src/openlit/instrumentation/bedrock/bedrock.py
--rw-r--r--   0        0        0     3253 2024-05-02 06:30:25.575605 openlit-1.1.1/src/openlit/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0    10374 2024-05-02 06:30:25.575605 openlit-1.1.1/src/openlit/instrumentation/chroma/chroma.py
--rw-r--r--   0        0        0     1920 2024-05-02 06:30:25.575605 openlit-1.1.1/src/openlit/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0    20348 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/cohere/cohere.py
--rw-r--r--   0        0        0     2531 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     7609 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/langchain/langchain.py
--rw-r--r--   0        0        0     3156 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/mistral/__init__.py
--rw-r--r--   0        0        0    21328 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/mistral/async_mistral.py
--rw-r--r--   0        0        0    21179 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/mistral/mistral.py
--rw-r--r--   0        0        0    16265 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0    46297 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/openai/async_azure_openai.py
--rw-r--r--   0        0        0    45841 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/openai/async_openai.py
--rw-r--r--   0        0        0    46091 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/openai/azure_openai.py
--rw-r--r--   0        0        0    46522 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/openai/openai.py
--rw-r--r--   0        0        0     2526 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     8732 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/pinecone/pinecone.py
--rw-r--r--   0        0        0     1478 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/transformers/__init__.py
--rw-r--r--   0        0        0     7592 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/transformers/transformers.py
--rw-r--r--   0        0        0     4291 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/otel/metrics.py
--rw-r--r--   0        0        0     3612 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/otel/tracing.py
--rw-r--r--   0        0        0     5724 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/semcov/__init__.py
--rw-r--r--   0        0        0    10535 1970-01-01 00:00:00.000000 openlit-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-02 08:09:23.440619 openlit-1.1.2/LICENSE
+-rw-r--r--   0        0        0     9235 2024-05-02 08:09:23.440619 openlit-1.1.2/README.md
+-rw-r--r--   0        0        0      966 2024-05-02 08:09:23.440619 openlit-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4651 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/__helpers.py
+-rw-r--r--   0        0        0     8939 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/__init__.py
+-rw-r--r--   0        0        0     1955 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0    15993 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/anthropic/anthropic.py
+-rw-r--r--   0        0        0    16035 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/anthropic/async_anthropic.py
+-rw-r--r--   0        0        0     1540 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/bedrock/__init__.py
+-rw-r--r--   0        0        0    22278 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/bedrock/bedrock.py
+-rw-r--r--   0        0        0     3253 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0    10374 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/chroma/chroma.py
+-rw-r--r--   0        0        0     1920 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0    20348 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/cohere/cohere.py
+-rw-r--r--   0        0        0     2531 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     7609 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/langchain/langchain.py
+-rw-r--r--   0        0        0     3156 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/mistral/__init__.py
+-rw-r--r--   0        0        0    21328 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/mistral/async_mistral.py
+-rw-r--r--   0        0        0    21179 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/mistral/mistral.py
+-rw-r--r--   0        0        0    16265 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0    46297 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/openai/async_azure_openai.py
+-rw-r--r--   0        0        0    45841 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/openai/async_openai.py
+-rw-r--r--   0        0        0    46091 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/openai/azure_openai.py
+-rw-r--r--   0        0        0    46522 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/openai/openai.py
+-rw-r--r--   0        0        0     2526 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     8732 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/pinecone/pinecone.py
+-rw-r--r--   0        0        0     1478 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/transformers/__init__.py
+-rw-r--r--   0        0        0     7592 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/instrumentation/transformers/transformers.py
+-rw-r--r--   0        0        0     4291 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/otel/metrics.py
+-rw-r--r--   0        0        0     3612 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/otel/tracing.py
+-rw-r--r--   0        0        0     5724 2024-05-02 08:09:23.440619 openlit-1.1.2/src/openlit/semcov/__init__.py
+-rw-r--r--   0        0        0    10535 1970-01-01 00:00:00.000000 openlit-1.1.2/PKG-INFO
```

### Comparing `openlit-1.1.1/LICENSE` & `openlit-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/README.md` & `openlit-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/pyproject.toml` & `openlit-1.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openlit"
-version = "1.1.1"
+version = "1.1.2"
 description = "OpenTelemetry-native Auto instrumentation library for monitoring LLM Applications, facilitating the integration of observability into your GenAI-driven projects"
 authors = ["OpenLIT"]
 repository = "https://github.com/openlit/openlit/tree/main/openlit/python"
 readme = "README.md"
 homepage = "https://github.com/openlit/openlit/tree/main/openlit/python"
 keywords = ["OpenTelemetry", "otel", "otlp","llm", "tracing", "openai", "anthropic", "claude", "cohere", "llm monitoring", "observability", "monitoring", "gpt", "Generative AI", "chatGPT"]
```

### Comparing `openlit-1.1.1/src/openlit/__helpers.py` & `openlit-1.1.2/src/openlit/__helpers.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/__init__.py` & `openlit-1.1.2/src/openlit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         "openai": "openai",
         "anthropic": "anthropic",  
         "cohere": "cohere",  
         "mistral": "mistralai",
         "bedrock": "boto3",
         "langchain": "langchain",
         "chroma": "chromadb",
-        "pinecone": "pincone",
+        "pinecone": "pinecone-client",
         "transformers": "transformers"
     }
 
     invalid_instrumentors = [name for name in disabled_instrumentors if name not in module_name_map]
     for invalid_name in invalid_instrumentors:
         logger.warning("Invalid instrumentor name detected and ignored: '%s'", invalid_name)
```

### Comparing `openlit-1.1.1/src/openlit/instrumentation/anthropic/__init__.py` & `openlit-1.1.2/src/openlit/instrumentation/anthropic/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/anthropic/anthropic.py` & `openlit-1.1.2/src/openlit/instrumentation/anthropic/anthropic.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/anthropic/async_anthropic.py` & `openlit-1.1.2/src/openlit/instrumentation/anthropic/async_anthropic.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/bedrock/__init__.py` & `openlit-1.1.2/src/openlit/instrumentation/bedrock/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/bedrock/bedrock.py` & `openlit-1.1.2/src/openlit/instrumentation/bedrock/bedrock.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/chroma/__init__.py` & `openlit-1.1.2/src/openlit/instrumentation/chroma/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/chroma/chroma.py` & `openlit-1.1.2/src/openlit/instrumentation/chroma/chroma.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/cohere/__init__.py` & `openlit-1.1.2/src/openlit/instrumentation/cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/cohere/cohere.py` & `openlit-1.1.2/src/openlit/instrumentation/cohere/cohere.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/langchain/__init__.py` & `openlit-1.1.2/src/openlit/instrumentation/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/langchain/langchain.py` & `openlit-1.1.2/src/openlit/instrumentation/langchain/langchain.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/mistral/__init__.py` & `openlit-1.1.2/src/openlit/instrumentation/mistral/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/mistral/async_mistral.py` & `openlit-1.1.2/src/openlit/instrumentation/mistral/async_mistral.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/mistral/mistral.py` & `openlit-1.1.2/src/openlit/instrumentation/mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/openai/__init__.py` & `openlit-1.1.2/src/openlit/instrumentation/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/openai/async_azure_openai.py` & `openlit-1.1.2/src/openlit/instrumentation/openai/async_azure_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/openai/async_openai.py` & `openlit-1.1.2/src/openlit/instrumentation/openai/async_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/openai/azure_openai.py` & `openlit-1.1.2/src/openlit/instrumentation/openai/azure_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/openai/openai.py` & `openlit-1.1.2/src/openlit/instrumentation/openai/openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/pinecone/__init__.py` & `openlit-1.1.2/src/openlit/instrumentation/pinecone/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/pinecone/pinecone.py` & `openlit-1.1.2/src/openlit/instrumentation/pinecone/pinecone.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/transformers/__init__.py` & `openlit-1.1.2/src/openlit/instrumentation/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/instrumentation/transformers/transformers.py` & `openlit-1.1.2/src/openlit/instrumentation/transformers/transformers.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/otel/metrics.py` & `openlit-1.1.2/src/openlit/otel/metrics.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/otel/tracing.py` & `openlit-1.1.2/src/openlit/otel/tracing.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/src/openlit/semcov/__init__.py` & `openlit-1.1.2/src/openlit/semcov/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.1/PKG-INFO` & `openlit-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlit
-Version: 1.1.1
+Version: 1.1.2
 Summary: OpenTelemetry-native Auto instrumentation library for monitoring LLM Applications, facilitating the integration of observability into your GenAI-driven projects
 Home-page: https://github.com/openlit/openlit/tree/main/openlit/python
 Keywords: OpenTelemetry,otel,otlp,llm,tracing,openai,anthropic,claude,cohere,llm monitoring,observability,monitoring,gpt,Generative AI,chatGPT
 Author: OpenLIT
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

