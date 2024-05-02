# Comparing `tmp/langfuse_haystack-0.0.3.tar.gz` & `tmp/langfuse_haystack-0.0.4.tar.gz`

## Comparing `langfuse_haystack-0.0.3.tar` & `langfuse_haystack-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.3/example/basic_rag.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.3/example/chat.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.3/example/requirements.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.3/src/haystack_integrations/components/others/langfuse/__about__.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.3/src/haystack_integrations/components/others/langfuse/__init__.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.3/src/haystack_integrations/components/others/langfuse/component.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.3/src/haystack_integrations/tracing/langfuse/__init__.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.3/src/haystack_integrations/tracing/langfuse/tracer.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.3/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.3/README.md
--rw-r--r--   0        0        0     4010 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.4/example/basic_rag.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.4/example/chat.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.4/example/requirements.txt
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.4/pydoc/config.yml
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.4/src/haystack_integrations/components/connectors/langfuse/__init__.py
+-rw-r--r--   0        0        0     3450 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.4/src/haystack_integrations/components/connectors/langfuse/langfuse_connector.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.4/src/haystack_integrations/tracing/langfuse/__init__.py
+-rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.4/src/haystack_integrations/tracing/langfuse/tracer.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.4/tests/test_tracing.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.4/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.4/README.md
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4684 2020-02-02 00:00:00.000000 langfuse_haystack-0.0.4/PKG-INFO
```

### Comparing `langfuse_haystack-0.0.3/example/basic_rag.py` & `langfuse_haystack-0.0.4/example/basic_rag.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 import os
 
-os.environ["LANGFUSE_HOST"] = "https://cloud.langfuse.com"
 os.environ["TOKENIZERS_PARALLELISM"] = "false"
 os.environ["HAYSTACK_CONTENT_TRACING_ENABLED"] = "true"
 
 from datasets import load_dataset
-
-from haystack.document_stores.in_memory import InMemoryDocumentStore
 from haystack import Document, Pipeline
+from haystack.components.builders import PromptBuilder
 from haystack.components.embedders import SentenceTransformersDocumentEmbedder, SentenceTransformersTextEmbedder
-from haystack.components.retrievers import InMemoryEmbeddingRetriever
 from haystack.components.generators import OpenAIGenerator
-from haystack.components.builders import PromptBuilder
-
-from haystack_integrations.components.others.langfuse import LangfuseComponent
+from haystack.components.retrievers import InMemoryEmbeddingRetriever
+from haystack.document_stores.in_memory import InMemoryDocumentStore
+from haystack_integrations.components.connectors.langfuse import LangfuseConnector
 
 
 def get_pipeline(document_store: InMemoryDocumentStore):
     retriever = InMemoryEmbeddingRetriever(document_store=document_store, top_k=2)
 
     template = """
     Given the following information, answer the question.
@@ -31,15 +28,15 @@
     Answer:
     """
 
     prompt_builder = PromptBuilder(template=template)
 
     basic_rag_pipeline = Pipeline()
     # Add components to your pipeline
-    basic_rag_pipeline.add_component("tracer", LangfuseComponent("Basic RAG Pipeline"))
+    basic_rag_pipeline.add_component("tracer", LangfuseConnector("Basic RAG Pipeline"))
     basic_rag_pipeline.add_component(
         "text_embedder", SentenceTransformersTextEmbedder(model="sentence-transformers/all-MiniLM-L6-v2")
     )
     basic_rag_pipeline.add_component("retriever", retriever)
     basic_rag_pipeline.add_component("prompt_builder", prompt_builder)
     basic_rag_pipeline.add_component("llm", OpenAIGenerator(model="gpt-3.5-turbo", generation_kwargs={"n": 2}))
 
@@ -61,7 +58,8 @@
     document_store.write_documents(docs_with_embeddings)
 
     pipeline = get_pipeline(document_store)
     question = "What does Rhodes Statue look like?"
     response = pipeline.run({"text_embedder": {"text": question}, "prompt_builder": {"question": question}})
 
     print(response["llm"]["replies"][0])
+    print(response["tracer"]["trace_url"])
```

### Comparing `langfuse_haystack-0.0.3/example/chat.py` & `langfuse_haystack-0.0.4/example/chat.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 import os
 
-os.environ["LANGFUSE_HOST"] = "https://cloud.langfuse.com"
-os.environ["TOKENIZERS_PARALLELISM"] = "false"
 os.environ["HAYSTACK_CONTENT_TRACING_ENABLED"] = "true"
 
+from haystack import Pipeline
 from haystack.components.builders import DynamicChatPromptBuilder
 from haystack.components.generators.chat import OpenAIChatGenerator
 from haystack.dataclasses import ChatMessage
-from haystack import Pipeline
-from haystack.utils import Secret
-
-from haystack_integrations.components.others.langfuse import LangfuseComponent
-
+from haystack_integrations.components.connectors.langfuse import LangfuseConnector
 
 if __name__ == "__main__":
 
     pipe = Pipeline()
-    pipe.add_component("tracer", LangfuseComponent("Chat example"))
+    pipe.add_component("tracer", LangfuseConnector("Chat example"))
     pipe.add_component("prompt_builder", DynamicChatPromptBuilder())
     pipe.add_component("llm", OpenAIChatGenerator(model="gpt-3.5-turbo"))
 
     pipe.connect("prompt_builder.prompt", "llm.messages")
 
     messages = [
         ChatMessage.from_system("Always respond in German even if some input data is in other languages."),
         ChatMessage.from_user("Tell me about {{location}}"),
     ]
 
     response = pipe.run(
         data={"prompt_builder": {"template_variables": {"location": "Berlin"}, "prompt_source": messages}}
     )
     print(response["llm"]["replies"][0])
+    print(response["tracer"]["trace_url"])
```

### Comparing `langfuse_haystack-0.0.3/src/haystack_integrations/tracing/langfuse/tracer.py` & `langfuse_haystack-0.0.4/src/haystack_integrations/tracing/langfuse/tracer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,72 @@
 import contextlib
 from typing import Any, Dict, Iterator, Optional, Union
 
+from haystack.dataclasses import ChatMessage
 from haystack.tracing import Span, Tracer, tracer
 from haystack.tracing import utils as tracing_utils
 
 import langfuse
 
 
 class LangfuseSpan(Span):
     def __init__(self, span: "Union[langfuse.client.StatefulSpanClient, langfuse.client.StatefulTraceClient]") -> None:
         self._span = span
         # locally cache tags
-        self._data = {}
+        self._data: Dict[str, Any] = {}
 
     def set_tag(self, key: str, value: Any) -> None:
         coerced_value = tracing_utils.coerce_tag_value(value)
         self._span.update(metadata={key: coerced_value})
         self._data[key] = value
 
     def set_content_tag(self, key: str, value: Any) -> None:
         if not tracer.is_content_tracing_enabled:
             return
-
         if key.endswith(".input"):
             if "messages" in value:
-                messages = [m.to_openai_format() for m in value["messages"]]
+                messages = [self.to_openai_format(m) for m in value["messages"]]
                 self._span.update(input=messages)
             else:
                 self._span.update(input=value)
         elif key.endswith(".output"):
             if "replies" in value:
-                replies = [m.to_openai_format() for m in value["replies"]]
+                if all(isinstance(r, ChatMessage) for r in value["replies"]):
+                    replies = [self.to_openai_format(m) for m in value["replies"]]
+                else:
+                    replies = value["replies"]
                 self._span.update(output=replies)
             else:
                 self._span.update(output=value)
 
         self._data[key] = value
 
     def raw_span(self) -> Any:
         return self._span
 
     def get_correlation_data_for_logs(self) -> Dict[str, Any]:
         return {}
 
+    def to_openai_format(self, m: ChatMessage) -> Dict[str, Any]:
+        """
+        Remove after haystack 2.0.1 has been released and use the `to_openai_format` method from the ChatMessage class
+        """
+        msg = {"role": m.role.value, "content": m.content}
+        if m.name:
+            msg["name"] = m.name
+
+        return msg
+
 
 class LangfuseTracer(Tracer):
-    def __init__(self, tracer: "langfuse.Langfuse", name: str = "Haystack") -> None:
+    def __init__(self, tracer: "langfuse.Langfuse", name: str = "Haystack", public: bool = False) -> None:
         self._tracer = tracer
         self._context: list[LangfuseSpan] = []
         self._name = name
+        self._public = public
 
     @contextlib.contextmanager
     def trace(self, operation_name: str, tags: Optional[Dict[str, Any]] = None) -> Iterator[Span]:
         tags = tags or {}
         span_name = tags.get("haystack.component.name", operation_name)
 
         if tags.get("haystack.component.type") in ["OpenAIGenerator", "OpenAIChatGenerator"]:
@@ -74,16 +88,26 @@
                 span._span.update(usage=m.get("usage"), model=m.get("model"))
         elif tags.get("haystack.component.type") == "OpenAIChatGenerator":
             replies = span._data.get("haystack.component.output", {}).get("replies")
             if replies:
                 meta = replies[0].meta
                 span._span.update(usage=meta.get("usage"), model=meta.get("model"))
 
+        pipeline_input = tags.get("haystack.pipeline.input_data", None)
+        if pipeline_input:
+            span._span.update(input=tags["haystack.pipeline.input_data"])
+        pipeline_output = tags.get("haystack.pipeline.output_data", None)
+        if pipeline_output:
+            span._span.update(output=tags["haystack.pipeline.output_data"])
+
         span.raw_span().end()
         self._context.pop()
         self._tracer.flush()
 
     def current_span(self) -> Span:
         if not self._context:
             # The root span has to be a trace
-            self._context.append(LangfuseSpan(self._tracer.trace(name=self._name)))
+            self._context.append(LangfuseSpan(self._tracer.trace(name=self._name, public=self._public)))
         return self._context[-1]
+
+    def get_trace_url(self) -> str:
+        return self._tracer.get_trace_url()
```

### Comparing `langfuse_haystack-0.0.3/.gitignore` & `langfuse_haystack-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `langfuse_haystack-0.0.3/LICENSE.txt` & `langfuse_haystack-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langfuse_haystack-0.0.3/pyproject.toml` & `langfuse_haystack-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "hatch-vcs"]
 build-backend = "hatchling.build"
 
 [project]
 name = "langfuse-haystack"
 dynamic = ["version"]
 description = ''
 readme = "README.md"
@@ -34,28 +34,27 @@
 Issues = "https://github.com/deepset-ai/haystack-core-integrations/issues"
 Source = "https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/langfuse"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/haystack_integrations"]
 
 [tool.hatch.version]
-# Remove the following line and uncomment the others to enable git versioning
-path = "src/haystack_integrations/components/others/langfuse/__about__.py"
-# source = "vcs"
-# tag-pattern = 'integrations\/langfuse-v(?P<version>.*)'
+source = "vcs"
+tag-pattern = 'integrations\/langfuse-v(?P<version>.*)'
 
 
 [tool.hatch.version.raw-options]
 root = "../.."
 git_describe_command = 'git describe --tags --match="integrations/langfuse-v[0-9]*"'
 
 [tool.hatch.envs.default]
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
+  "haystack-pydoc-tools",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
   "- coverage combine",
   "coverage report",
```

