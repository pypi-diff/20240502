# Comparing `tmp/openlit-1.1.0.tar.gz` & `tmp/openlit-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlit-1.1.0.tar", max compression
+gzip compressed data, was "openlit-1.1.1.tar", max compression
```

## Comparing `openlit-1.1.0.tar` & `openlit-1.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    11357 2024-05-01 09:49:17.276286 openlit-1.1.0/LICENSE
--rw-r--r--   0        0        0     9235 2024-05-01 09:49:17.276286 openlit-1.1.0/README.md
--rw-r--r--   0        0        0      966 2024-05-01 09:49:17.276286 openlit-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4651 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/__helpers.py
--rw-r--r--   0        0        0     8931 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/__init__.py
--rw-r--r--   0        0        0     1955 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0    15993 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/anthropic/anthropic.py
--rw-r--r--   0        0        0    16035 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/anthropic/async_anthropic.py
--rw-r--r--   0        0        0     1540 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/bedrock/__init__.py
--rw-r--r--   0        0        0    22278 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/bedrock/bedrock.py
--rw-r--r--   0        0        0     3253 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0    10374 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/chroma/chroma.py
--rw-r--r--   0        0        0     1920 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0    20348 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/cohere/cohere.py
--rw-r--r--   0        0        0     2531 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     7609 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/langchain/langchain.py
--rw-r--r--   0        0        0     3156 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/mistral/__init__.py
--rw-r--r--   0        0        0    21328 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/mistral/async_mistral.py
--rw-r--r--   0        0        0    21179 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/mistral/mistral.py
--rw-r--r--   0        0        0    16265 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0    46297 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/openai/async_azure_openai.py
--rw-r--r--   0        0        0    45841 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/openai/async_openai.py
--rw-r--r--   0        0        0    46091 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/openai/azure_openai.py
--rw-r--r--   0        0        0    46522 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/openai/openai.py
--rw-r--r--   0        0        0     2526 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     8732 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/pinecone/pinecone.py
--rw-r--r--   0        0        0     1478 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/transformers/__init__.py
--rw-r--r--   0        0        0     7592 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/instrumentation/transformers/transformers.py
--rw-r--r--   0        0        0     4291 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/otel/metrics.py
--rw-r--r--   0        0        0     3612 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/otel/tracing.py
--rw-r--r--   0        0        0     5724 2024-05-01 09:49:17.276286 openlit-1.1.0/src/openlit/semcov/__init__.py
--rw-r--r--   0        0        0    10535 1970-01-01 00:00:00.000000 openlit-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-02 06:30:25.575605 openlit-1.1.1/LICENSE
+-rw-r--r--   0        0        0     9235 2024-05-02 06:30:25.575605 openlit-1.1.1/README.md
+-rw-r--r--   0        0        0      966 2024-05-02 06:30:25.575605 openlit-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4651 2024-05-02 06:30:25.575605 openlit-1.1.1/src/openlit/__helpers.py
+-rw-r--r--   0        0        0     8931 2024-05-02 06:30:25.575605 openlit-1.1.1/src/openlit/__init__.py
+-rw-r--r--   0        0        0     1955 2024-05-02 06:30:25.575605 openlit-1.1.1/src/openlit/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0    15993 2024-05-02 06:30:25.575605 openlit-1.1.1/src/openlit/instrumentation/anthropic/anthropic.py
+-rw-r--r--   0        0        0    16035 2024-05-02 06:30:25.575605 openlit-1.1.1/src/openlit/instrumentation/anthropic/async_anthropic.py
+-rw-r--r--   0        0        0     1540 2024-05-02 06:30:25.575605 openlit-1.1.1/src/openlit/instrumentation/bedrock/__init__.py
+-rw-r--r--   0        0        0    22278 2024-05-02 06:30:25.575605 openlit-1.1.1/src/openlit/instrumentation/bedrock/bedrock.py
+-rw-r--r--   0        0        0     3253 2024-05-02 06:30:25.575605 openlit-1.1.1/src/openlit/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0    10374 2024-05-02 06:30:25.575605 openlit-1.1.1/src/openlit/instrumentation/chroma/chroma.py
+-rw-r--r--   0        0        0     1920 2024-05-02 06:30:25.575605 openlit-1.1.1/src/openlit/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0    20348 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/cohere/cohere.py
+-rw-r--r--   0        0        0     2531 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     7609 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/langchain/langchain.py
+-rw-r--r--   0        0        0     3156 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/mistral/__init__.py
+-rw-r--r--   0        0        0    21328 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/mistral/async_mistral.py
+-rw-r--r--   0        0        0    21179 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/mistral/mistral.py
+-rw-r--r--   0        0        0    16265 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0    46297 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/openai/async_azure_openai.py
+-rw-r--r--   0        0        0    45841 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/openai/async_openai.py
+-rw-r--r--   0        0        0    46091 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/openai/azure_openai.py
+-rw-r--r--   0        0        0    46522 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/openai/openai.py
+-rw-r--r--   0        0        0     2526 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     8732 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/pinecone/pinecone.py
+-rw-r--r--   0        0        0     1478 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/transformers/__init__.py
+-rw-r--r--   0        0        0     7592 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/instrumentation/transformers/transformers.py
+-rw-r--r--   0        0        0     4291 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/otel/metrics.py
+-rw-r--r--   0        0        0     3612 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/otel/tracing.py
+-rw-r--r--   0        0        0     5724 2024-05-02 06:30:25.579604 openlit-1.1.1/src/openlit/semcov/__init__.py
+-rw-r--r--   0        0        0    10535 1970-01-01 00:00:00.000000 openlit-1.1.1/PKG-INFO
```

### Comparing `openlit-1.1.0/LICENSE` & `openlit-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/README.md` & `openlit-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/pyproject.toml` & `openlit-1.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "openlit"
-version = "1.1.0"
+version = "1.1.1"
 description = "OpenTelemetry-native Auto instrumentation library for monitoring LLM Applications, facilitating the integration of observability into your GenAI-driven projects"
 authors = ["OpenLIT"]
 repository = "https://github.com/openlit/openlit/tree/main/openlit/python"
 readme = "README.md"
 homepage = "https://github.com/openlit/openlit/tree/main/openlit/python"
 keywords = ["OpenTelemetry", "otel", "otlp","llm", "tracing", "openai", "anthropic", "claude", "cohere", "llm monitoring", "observability", "monitoring", "gpt", "Generative AI", "chatGPT"]
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
 requests = "^2.26.0"
-tiktoken = "^0.1.1"
+tiktoken = "^0.6.0"
 boto3 = "^1.34.0"
 botocore = "^1.34.0"
 opentelemetry-api = "^1.24.0"
 opentelemetry-sdk = "^1.24.0"
 opentelemetry-exporter-otlp = "^1.24.0"
 opentelemetry-instrumentation = "^0.45b0"
```

### Comparing `openlit-1.1.0/src/openlit/__helpers.py` & `openlit-1.1.1/src/openlit/__helpers.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/__init__.py` & `openlit-1.1.1/src/openlit/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/anthropic/__init__.py` & `openlit-1.1.1/src/openlit/instrumentation/anthropic/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/anthropic/anthropic.py` & `openlit-1.1.1/src/openlit/instrumentation/anthropic/anthropic.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/anthropic/async_anthropic.py` & `openlit-1.1.1/src/openlit/instrumentation/anthropic/async_anthropic.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/bedrock/__init__.py` & `openlit-1.1.1/src/openlit/instrumentation/bedrock/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/bedrock/bedrock.py` & `openlit-1.1.1/src/openlit/instrumentation/bedrock/bedrock.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/chroma/__init__.py` & `openlit-1.1.1/src/openlit/instrumentation/chroma/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/chroma/chroma.py` & `openlit-1.1.1/src/openlit/instrumentation/chroma/chroma.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/cohere/__init__.py` & `openlit-1.1.1/src/openlit/instrumentation/cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/cohere/cohere.py` & `openlit-1.1.1/src/openlit/instrumentation/cohere/cohere.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/langchain/__init__.py` & `openlit-1.1.1/src/openlit/instrumentation/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/langchain/langchain.py` & `openlit-1.1.1/src/openlit/instrumentation/langchain/langchain.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/mistral/__init__.py` & `openlit-1.1.1/src/openlit/instrumentation/mistral/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/mistral/async_mistral.py` & `openlit-1.1.1/src/openlit/instrumentation/mistral/async_mistral.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/mistral/mistral.py` & `openlit-1.1.1/src/openlit/instrumentation/mistral/mistral.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/openai/__init__.py` & `openlit-1.1.1/src/openlit/instrumentation/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/openai/async_azure_openai.py` & `openlit-1.1.1/src/openlit/instrumentation/openai/async_azure_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/openai/async_openai.py` & `openlit-1.1.1/src/openlit/instrumentation/openai/async_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/openai/azure_openai.py` & `openlit-1.1.1/src/openlit/instrumentation/openai/azure_openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/openai/openai.py` & `openlit-1.1.1/src/openlit/instrumentation/openai/openai.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/pinecone/__init__.py` & `openlit-1.1.1/src/openlit/instrumentation/pinecone/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/pinecone/pinecone.py` & `openlit-1.1.1/src/openlit/instrumentation/pinecone/pinecone.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/transformers/__init__.py` & `openlit-1.1.1/src/openlit/instrumentation/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/instrumentation/transformers/transformers.py` & `openlit-1.1.1/src/openlit/instrumentation/transformers/transformers.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/otel/metrics.py` & `openlit-1.1.1/src/openlit/otel/metrics.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/otel/tracing.py` & `openlit-1.1.1/src/openlit/otel/tracing.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/src/openlit/semcov/__init__.py` & `openlit-1.1.1/src/openlit/semcov/__init__.py`

 * *Files identical despite different names*

### Comparing `openlit-1.1.0/PKG-INFO` & `openlit-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlit
-Version: 1.1.0
+Version: 1.1.1
 Summary: OpenTelemetry-native Auto instrumentation library for monitoring LLM Applications, facilitating the integration of observability into your GenAI-driven projects
 Home-page: https://github.com/openlit/openlit/tree/main/openlit/python
 Keywords: OpenTelemetry,otel,otlp,llm,tracing,openai,anthropic,claude,cohere,llm monitoring,observability,monitoring,gpt,Generative AI,chatGPT
 Author: OpenLIT
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -15,15 +15,15 @@
 Requires-Dist: boto3 (>=1.34.0,<2.0.0)
 Requires-Dist: botocore (>=1.34.0,<2.0.0)
 Requires-Dist: opentelemetry-api (>=1.24.0,<2.0.0)
 Requires-Dist: opentelemetry-exporter-otlp (>=1.24.0,<2.0.0)
 Requires-Dist: opentelemetry-instrumentation (>=0.45b0,<0.46)
 Requires-Dist: opentelemetry-sdk (>=1.24.0,<2.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
-Requires-Dist: tiktoken (>=0.1.1,<0.2.0)
+Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
 Project-URL: Repository, https://github.com/openlit/openlit/tree/main/openlit/python
 Description-Content-Type: text/markdown
 
 <div align="center">
 <img src="https://github.com/openlit/.github/blob/main/profile/assets/wide-logo-no-bg.png?raw=true" alt="OpenLIT Logo" width="30%"><h1>
 OpenTelemetry Auto-Instrumentation for GenAI & LLM Applications</h1>
```

