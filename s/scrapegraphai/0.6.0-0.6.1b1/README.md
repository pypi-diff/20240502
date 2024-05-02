# Comparing `tmp/scrapegraphai-0.6.0.tar.gz` & `tmp/scrapegraphai-0.6.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.6.0.tar", max compression
+gzip compressed data, was "scrapegraphai-0.6.1b1.tar", max compression
```

## Comparing `scrapegraphai-0.6.0.tar` & `scrapegraphai-0.6.1b1.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0     1065 2024-05-02 15:56:25.845046 scrapegraphai-0.6.0/LICENSE
--rw-r--r--   0        0        0     8876 2024-05-02 15:56:25.845046 scrapegraphai-0.6.0/README.md
--rw-r--r--   0        0        0     1711 2024-05-02 15:56:45.513022 scrapegraphai-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       54 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6653 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      402 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0     6578 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     5385 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2672 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/graphs/csv_scraper_graph.py
--rw-r--r--   0        0        0     3594 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/graphs/json_scraper_graph.py
--rw-r--r--   0        0        0     3880 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     3650 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     3749 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     4575 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0     3738 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/graphs/xml_scraper_graph.py
--rw-r--r--   0        0        0      202 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0     1171 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      313 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      441 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      463 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      426 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      459 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      427 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      412 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1367 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1221 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      644 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7932 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3716 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     6987 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/generate_answer_csv_node.py
--rw-r--r--   0        0        0     6431 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     6987 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/generate_answer_node_csv.py
--rw-r--r--   0        0        0     6639 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     3527 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1955 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     2684 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     5598 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     5605 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     3707 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     6261 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     2317 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      286 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     2141 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1974 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     4638 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      764 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0      800 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     1442 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     1605 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      836 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0     1320 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0    10672 1970-01-01 00:00:00.000000 scrapegraphai-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-02 15:58:17.712082 scrapegraphai-0.6.1b1/LICENSE
+-rw-r--r--   0        0        0     8876 2024-05-02 15:58:17.712082 scrapegraphai-0.6.1b1/README.md
+-rw-r--r--   0        0        0     1739 2024-05-02 15:58:37.872124 scrapegraphai-0.6.1b1/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6653 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      402 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0     7126 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     5385 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2672 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/graphs/csv_scraper_graph.py
+-rw-r--r--   0        0        0     3594 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/graphs/json_scraper_graph.py
+-rw-r--r--   0        0        0     3880 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     3650 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     3749 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     4575 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0     3738 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/graphs/xml_scraper_graph.py
+-rw-r--r--   0        0        0      202 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0     1909 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      342 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      441 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      579 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/models/bedrock.py
+-rw-r--r--   0        0        0      463 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      426 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      459 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      427 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      412 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1367 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1221 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      644 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7932 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3716 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     6987 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/generate_answer_csv_node.py
+-rw-r--r--   0        0        0     6431 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     6987 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/generate_answer_node_csv.py
+-rw-r--r--   0        0        0     6639 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     3527 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1955 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     2684 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     5835 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     5605 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     3707 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     6261 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     2317 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      286 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     2141 2024-05-02 15:58:17.740082 scrapegraphai-0.6.1b1/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1974 2024-05-02 15:58:17.744082 scrapegraphai-0.6.1b1/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     4638 2024-05-02 15:58:17.744082 scrapegraphai-0.6.1b1/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      764 2024-05-02 15:58:17.744082 scrapegraphai-0.6.1b1/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0      800 2024-05-02 15:58:17.744082 scrapegraphai-0.6.1b1/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     1442 2024-05-02 15:58:17.744082 scrapegraphai-0.6.1b1/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1605 2024-05-02 15:58:17.744082 scrapegraphai-0.6.1b1/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      836 2024-05-02 15:58:17.744082 scrapegraphai-0.6.1b1/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0     1320 2024-05-02 15:58:17.744082 scrapegraphai-0.6.1b1/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0    10720 1970-01-01 00:00:00.000000 scrapegraphai-0.6.1b1/PKG-INFO
```

### Comparing `scrapegraphai-0.6.0/LICENSE` & `scrapegraphai-0.6.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/README.md` & `scrapegraphai-0.6.1b1/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/pyproject.toml` & `scrapegraphai-0.6.1b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "scrapegraphai"
 
-version = "0.6.0"
+version = "0.6.1b1"
 
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
@@ -37,14 +37,16 @@
 tqdm = "4.66.1"
 graphviz = "0.20.1"
 google = "3.0.0"
 minify-html = "0.15.0"
 free-proxy = "1.1.1"
 langchain-groq = "0.1.3"
 playwright = "^1.43.0"
+langchain-aws = "^0.1.2"
+
 
 [tool.poetry.dev-dependencies]
 pytest = "8.0.0"
 
 [tool.poetry.group.docs]
 optional = true
```

### Comparing `scrapegraphai-0.6.0/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.6.1b1/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.6.1b1/scrapegraphai/graphs/abstract_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 AbstractGraph Module
 """
 
 from abc import ABC, abstractmethod
 from typing import Optional
-from ..models import OpenAI, Gemini, Ollama, AzureOpenAI, HuggingFace, Groq
+
+from ..models import OpenAI, Gemini, Ollama, AzureOpenAI, HuggingFace, Groq, Bedrock
 from ..helpers import models_tokens
 
 
 class AbstractGraph(ABC):
     """
     Scaffolding class for creating a graph representation and executing it.
 
@@ -43,15 +44,16 @@
         self.config = config
         self.llm_model = self._create_llm(config["llm"], chat=True)
         self.embedder_model = self.llm_model if "embeddings" not in config else self._create_llm(
             config["embeddings"])
 
         # Set common configuration parameters
         self.verbose = True if config is None else config.get("verbose", False)
-        self.headless = True if config is None else config.get("headless", True)
+        self.headless = True if config is None else config.get(
+            "headless", True)
 
         # Create the graph
         self.graph = self._create_graph()
         self.final_state = None
         self.execution_info = None
 
 
@@ -136,20 +138,34 @@
             try:
                 self.model_token = models_tokens["hugging_face"][llm_params["model"]]
             except KeyError:
                 raise KeyError("Model not supported")
             return HuggingFace(llm_params)
         elif "groq" in llm_params["model"]:
             llm_params["model"] = llm_params["model"].split("/")[-1]
-            
+
             try:
                 self.model_token = models_tokens["groq"][llm_params["model"]]
             except KeyError:
                 raise KeyError("Model not supported")
             return Groq(llm_params)
+        elif "bedrock" in llm_params["model"]:
+            llm_params["model"] = llm_params["model"].split("/")[-1]
+            model_id = llm_params["model"]
+
+            try:
+                self.model_token = models_tokens["bedrock"][llm_params["model"]]
+            except KeyError:
+                raise KeyError("Model not supported")
+            return Bedrock({
+                "model_id": model_id,
+                "model_kwargs": {
+                    "temperature": llm_params["temperature"],
+                }
+            })
         else:
             raise ValueError(
                 "Model provided by the configuration not supported")
 
     def get_state(self, key=None) -> dict:
         """""
         Get the final state of the graph.
```

### Comparing `scrapegraphai-0.6.0/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.6.1b1/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/graphs/csv_scraper_graph.py` & `scrapegraphai-0.6.1b1/scrapegraphai/graphs/csv_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/graphs/json_scraper_graph.py` & `scrapegraphai-0.6.1b1/scrapegraphai/graphs/json_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.6.1b1/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.6.1b1/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.6.1b1/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.6.1b1/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/graphs/xml_scraper_graph.py` & `scrapegraphai-0.6.1b1/scrapegraphai/graphs/xml_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.6.1b1/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.6.1b1/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.6.1b1/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.6.1b1/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/nodes/__init__.py` & `scrapegraphai-0.6.1b1/scrapegraphai/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.6.1b1/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.6.1b1/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.6.1b1/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/nodes/generate_answer_csv_node.py` & `scrapegraphai-0.6.1b1/scrapegraphai/nodes/generate_answer_csv_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.6.1b1/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/nodes/generate_answer_node_csv.py` & `scrapegraphai-0.6.1b1/scrapegraphai/nodes/generate_answer_node_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.6.1b1/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.6.1b1/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.6.1b1/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.6.1b1/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.6.1b1/scrapegraphai/nodes/rag_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 RAGNode Module
 """
 
 from typing import List
 from langchain.docstore.document import Document
 from langchain.retrievers import ContextualCompressionRetriever
 from langchain.retrievers.document_compressors import EmbeddingsFilter, DocumentCompressorPipeline
+from langchain_aws.embeddings.bedrock import BedrockEmbeddings
 from langchain_community.document_transformers import EmbeddingsRedundantFilter
 from langchain_community.embeddings import HuggingFaceHubEmbeddings
 from langchain_community.vectorstores import FAISS
 from langchain_community.embeddings import OllamaEmbeddings
 from langchain_openai import OpenAIEmbeddings, AzureOpenAIEmbeddings
-from ..models import OpenAI, Ollama, AzureOpenAI, HuggingFace
+
+from ..models import OpenAI, Ollama, AzureOpenAI, HuggingFace, Bedrock
 from .base_node import BaseNode
 
 
 class RAGNode(BaseNode):
     """
     A node responsible for compressing the input tokens and storing the document
     in a vector database for retrieval. Relevant chunks are stored in the state.
@@ -35,15 +37,16 @@
     """
 
     def __init__(self, input: str, output: List[str], node_config: dict, node_name: str = "RAG"):
         super().__init__(node_name, "node", input, output, 2, node_config)
 
         self.llm_model = node_config["llm"]
         self.embedder_model = node_config.get("embedder_model", None)
-        self.verbose = True if node_config is None else node_config.get("verbose", False)
+        self.verbose = True if node_config is None else node_config.get(
+            "verbose", False)
 
     def execute(self, state: dict) -> dict:
         """
         Executes the node's logic to implement RAG (Retrieval-Augmented Generation).
         The method updates the state with relevant chunks of the document.
 
         Args:
@@ -76,15 +79,15 @@
             doc = Document(
                 page_content=chunk,
                 metadata={
                     "chunk": i + 1,
                 },
             )
             chunked_docs.append(doc)
-        
+
         if self.verbose:
             print("--- (updated chunks metadata) ---")
 
         # check if embedder_model is provided, if not use llm_model
         embedding_model = self.embedder_model if self.embedder_model else self.llm_model
 
         if isinstance(embedding_model, OpenAI):
@@ -100,14 +103,17 @@
             # remove streaming and temperature
             params.pop("streaming", None)
             params.pop("temperature", None)
 
             embeddings = OllamaEmbeddings(**params)
         elif isinstance(embedding_model, HuggingFace):
             embeddings = HuggingFaceHubEmbeddings(model=embedding_model.model)
+        elif isinstance(embedding_model, Bedrock):
+            embeddings = BedrockEmbeddings(
+                client=None, model_id=embedding_model.model_id)
         else:
             raise ValueError("Embedding Model missing or not supported")
 
         retriever = FAISS.from_documents(
             chunked_docs, embeddings).as_retriever()
 
         redundant_filter = EmbeddingsRedundantFilter(embeddings=embeddings)
```

### Comparing `scrapegraphai-0.6.0/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-0.6.1b1/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.6.1b1/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-0.6.1b1/scrapegraphai/nodes/search_link_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.6.1b1/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.6.1b1/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.6.1b1/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.6.1b1/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.6.1b1/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-0.6.1b1/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/utils/remover.py` & `scrapegraphai-0.6.1b1/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.6.1b1/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.6.1b1/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.6.1b1/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.6.0/PKG-INFO` & `scrapegraphai-0.6.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.6.0
+Version: 0.6.1b1
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -20,14 +20,15 @@
 Requires-Dist: beautifulsoup4 (==4.12.3)
 Requires-Dist: faiss-cpu (==1.8.0)
 Requires-Dist: free-proxy (==1.1.1)
 Requires-Dist: google (==3.0.0)
 Requires-Dist: graphviz (==0.20.1)
 Requires-Dist: html2text (==2020.1.16)
 Requires-Dist: langchain (==0.1.14)
+Requires-Dist: langchain-aws (>=0.1.2,<0.2.0)
 Requires-Dist: langchain-google-genai (==1.0.1)
 Requires-Dist: langchain-groq (==0.1.3)
 Requires-Dist: langchain-openai (==0.1.1)
 Requires-Dist: minify-html (==0.15.0)
 Requires-Dist: pandas (==2.0.3)
 Requires-Dist: playwright (>=1.43.0,<2.0.0)
 Requires-Dist: python-dotenv (==1.0.1)
```

