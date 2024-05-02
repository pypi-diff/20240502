# Comparing `tmp/okahu_observability-0.0.1.tar.gz` & `tmp/okahu_observability-0.0.2.tar.gz`

## Comparing `okahu_observability-0.0.1.tar` & `okahu_observability-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 okahu_observability-0.0.1/src/okahu_apptrace/__init__.py
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 okahu_observability-0.0.1/src/okahu_apptrace/exporter.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 okahu_observability-0.0.1/src/okahu_apptrace/instrumentor.py
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 okahu_observability-0.0.1/src/okahu_apptrace/utils.py
--rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 okahu_observability-0.0.1/src/okahu_apptrace/wrapped_methods.py
--rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 okahu_observability-0.0.1/.gitignore
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 okahu_observability-0.0.1/LICENSE
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 okahu_observability-0.0.1/README.md
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 okahu_observability-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 okahu_observability-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 okahu_observability-0.0.2/src/okahu_apptrace/__init__.py
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 okahu_observability-0.0.2/src/okahu_apptrace/exporter.py
+-rw-r--r--   0        0        0     3878 2020-02-02 00:00:00.000000 okahu_observability-0.0.2/src/okahu_apptrace/instrumentor.py
+-rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 okahu_observability-0.0.2/src/okahu_apptrace/utils.py
+-rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 okahu_observability-0.0.2/src/okahu_apptrace/wrapper.py
+-rw-r--r--   0        0        0     1590 2020-02-02 00:00:00.000000 okahu_observability-0.0.2/.gitignore
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 okahu_observability-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 okahu_observability-0.0.2/README.md
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 okahu_observability-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 okahu_observability-0.0.2/PKG-INFO
```

### Comparing `okahu_observability-0.0.1/src/okahu_apptrace/exporter.py` & `okahu_observability-0.0.2/src/okahu_apptrace/exporter.py`

 * *Files identical despite different names*

### Comparing `okahu_observability-0.0.1/src/okahu_apptrace/instrumentor.py` & `okahu_observability-0.0.2/src/okahu_apptrace/instrumentor.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from opentelemetry.trace import get_tracer
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor
 from opentelemetry.instrumentation.utils import unwrap
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor, SpanProcessor
 from opentelemetry.sdk.resources import SERVICE_NAME, Resource
 from opentelemetry import trace
-from okahu_apptrace.wrapped_methods import METHODS_LIST, WrapperMethod
+from okahu_apptrace.wrapper import METHODS_LIST, WrapperMethod
 from okahu_apptrace.exporter import OkahuSpanExporter 
 
 logger = logging.getLogger(__name__)
 
 _instruments = ("langchain >= 0.0.346",)
 
 class OkahuInstrumentor(BaseInstrumentor):
```

### Comparing `okahu_observability-0.0.1/src/okahu_apptrace/utils.py` & `okahu_observability-0.0.2/src/okahu_apptrace/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -91,17 +91,17 @@
     elif to_wrap.get("span_name"):
         name = to_wrap.get("span_name")
     else:
         name = f"langchain.task.{instance.__class__.__name__}"
     kind = to_wrap.get("kind")
     with tracer.start_as_current_span(name) as span:
         update_llm_endpoint(curr_span= span, instance=instance)
-        
 
         return_value = wrapped(*args, **kwargs)
+        update_span_from_llm_response(response = return_value, span = span)       
 
     return return_value
 
 def update_llm_endpoint(curr_span: Span, instance):
     triton_llm_endpoint = os.environ.get("TRITON_LLM_ENDPOINT")
     if triton_llm_endpoint is not None and len(triton_llm_endpoint) > 0:
         curr_span.set_attribute("server_url", triton_llm_endpoint)
@@ -113,7 +113,29 @@
 def is_root_span(curr_span: Span) -> bool:
     return curr_span.parent == None
 
 def get_input_from_args(chain_args):
     if len(chain_args) > 0 and type(chain_args[0]) == str:
         return chain_args[0]
     return ""
+
+def update_span_from_llm_response(response, span: Span):
+    # extract token uasge from langchain openai
+    if (response is not None and hasattr(response, "response_metadata")):
+        response_metadata = response.response_metadata
+        token_usage = response_metadata.get("token_usage")
+        if token_usage is not None:
+            span.set_attribute("completion_tokens", token_usage.get("completion_tokens"))
+            span.set_attribute("prompt_tokens", token_usage.get("prompt_tokens"))
+            span.set_attribute("total_tokens", token_usage.get("total_tokens"))
+    
+    # extract token usage from llamaindex openai
+    if (response is not None and hasattr(response, "raw")):
+        token_usage = response.raw.get("usage")
+        if token_usage is not None:
+            if(hasattr(token_usage, "completion_tokens")):
+                span.set_attribute("completion_tokens", token_usage.completion_tokens)
+            if(hasattr(token_usage, "prompt_tokens")):
+                span.set_attribute("prompt_tokens", token_usage.prompt_tokens)
+            if(hasattr(token_usage, "total_tokens")):
+                span.set_attribute("total_tokens", token_usage.total_tokens)
+
```

### Comparing `okahu_observability-0.0.1/src/okahu_apptrace/wrapped_methods.py` & `okahu_observability-0.0.2/src/okahu_apptrace/wrapper.py`

 * *Files identical despite different names*

### Comparing `okahu_observability-0.0.1/.gitignore` & `okahu_observability-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `okahu_observability-0.0.1/LICENSE` & `okahu_observability-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `okahu_observability-0.0.1/README.md` & `okahu_observability-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 chain.invoke({"number":2}, {"callbacks":[handler]})
     
 ```
 
 ### Monitoring custom methods with Okahu
 
 ```python
-from okahu_apptrace.wrapped_methods import WrapperMethod,task_wrapper,atask_wrapper
+from okahu_apptrace.wrapper import WrapperMethod,task_wrapper,atask_wrapper
 from opentelemetry.sdk.trace.export import BatchSpanProcessor, ConsoleSpanExporter
 
 # extend the default wrapped methods list as follows
 app_name = "simple_math_app"
 setup_okahu_telemetry(
         workflow_name=app_name,
         span_processors=[BatchSpanProcessor(ConsoleSpanExporter())],
```

### Comparing `okahu_observability-0.0.1/pyproject.toml` & `okahu_observability-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "okahu-observability"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Okahu Inc.", email="okahu-pypi@okahu.ai" },
 ]
 description = "package with okahu opentelemetry"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -31,17 +31,19 @@
 
 [project.optional-dependencies]
 dev = [
   'langchain-openai==0.0.5',
   'numpy==1.26.4',
   'types-requests==2.31.0.20240106',
   'InstructorEmbedding==1.0.1',
-  'sentence-transformers==2.2.2',
+  'sentence-transformers==2.6.1',
   'faiss-cpu==1.7.4',
-  'pytest==8.0.0'
+  'pytest==8.0.0',
+  'llama-index==0.10.30',
+  'llama-index-embeddings-huggingface==0.2.0'
 ]
 
 [project.urls]
 Homepage = "https://github.com/okahu/demo-repository"
 Issues = "https://github.com/okahu/demo-repository/issues"
 
 [tool.hatch.build.targets.wheel]
```

### Comparing `okahu_observability-0.0.1/PKG-INFO` & `okahu_observability-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: okahu-observability
-Version: 0.0.1
+Version: 0.0.2
 Summary: package with okahu opentelemetry
 Project-URL: Homepage, https://github.com/okahu/demo-repository
 Project-URL: Issues, https://github.com/okahu/demo-repository/issues
 Author-email: "Okahu Inc." <okahu-pypi@okahu.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,17 +15,19 @@
 Requires-Dist: opentelemetry-sdk>=1.21.0
 Requires-Dist: requests
 Requires-Dist: wrapt>=1.14.0
 Provides-Extra: dev
 Requires-Dist: faiss-cpu==1.7.4; extra == 'dev'
 Requires-Dist: instructorembedding==1.0.1; extra == 'dev'
 Requires-Dist: langchain-openai==0.0.5; extra == 'dev'
+Requires-Dist: llama-index-embeddings-huggingface==0.2.0; extra == 'dev'
+Requires-Dist: llama-index==0.10.30; extra == 'dev'
 Requires-Dist: numpy==1.26.4; extra == 'dev'
 Requires-Dist: pytest==8.0.0; extra == 'dev'
-Requires-Dist: sentence-transformers==2.2.2; extra == 'dev'
+Requires-Dist: sentence-transformers==2.6.1; extra == 'dev'
 Requires-Dist: types-requests==2.31.0.20240106; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Okahu callback handler
 
 This package provides okahu telemetry setup.
 
@@ -65,15 +67,15 @@
 chain.invoke({"number":2}, {"callbacks":[handler]})
     
 ```
 
 ### Monitoring custom methods with Okahu
 
 ```python
-from okahu_apptrace.wrapped_methods import WrapperMethod,task_wrapper,atask_wrapper
+from okahu_apptrace.wrapper import WrapperMethod,task_wrapper,atask_wrapper
 from opentelemetry.sdk.trace.export import BatchSpanProcessor, ConsoleSpanExporter
 
 # extend the default wrapped methods list as follows
 app_name = "simple_math_app"
 setup_okahu_telemetry(
         workflow_name=app_name,
         span_processors=[BatchSpanProcessor(ConsoleSpanExporter())],
```

