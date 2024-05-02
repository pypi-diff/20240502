# Comparing `tmp/scrapegraphai-0.5.2.tar.gz` & `tmp/scrapegraphai-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.5.2.tar", max compression
+gzip compressed data, was "scrapegraphai-0.6.0.tar", max compression
```

## Comparing `scrapegraphai-0.5.2.tar` & `scrapegraphai-0.6.0.tar`

### file list

```diff
@@ -1,54 +1,57 @@
--rw-r--r--   0        0        0     1065 2024-05-02 07:24:45.753296 scrapegraphai-0.5.2/LICENSE
--rw-r--r--   0        0        0     8876 2024-05-02 07:24:45.753296 scrapegraphai-0.5.2/README.md
--rw-r--r--   0        0        0     1710 2024-05-02 07:25:04.433255 scrapegraphai-0.5.2/pyproject.toml
--rw-r--r--   0        0        0       54 2024-05-02 07:24:45.781296 scrapegraphai-0.5.2/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6653 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      355 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0     6036 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     5385 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     3594 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/graphs/json_scraper_graph.py
--rw-r--r--   0        0        0     3880 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     3650 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     3749 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     4575 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0     3738 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/graphs/xml_scraper_graph.py
--rw-r--r--   0        0        0      202 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0     1119 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      313 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      441 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      463 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      426 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      459 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      427 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      412 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1367 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1221 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      584 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7932 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     3716 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     6431 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     6639 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     3527 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1955 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     2684 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     5491 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     5605 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     3707 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     6261 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     2317 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      286 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     2141 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1974 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     4638 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      764 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0      800 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     1442 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     1605 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      836 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0     1320 2024-05-02 07:24:45.785296 scrapegraphai-0.5.2/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0    10672 1970-01-01 00:00:00.000000 scrapegraphai-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-02 15:56:25.845046 scrapegraphai-0.6.0/LICENSE
+-rw-r--r--   0        0        0     8876 2024-05-02 15:56:25.845046 scrapegraphai-0.6.0/README.md
+-rw-r--r--   0        0        0     1711 2024-05-02 15:56:45.513022 scrapegraphai-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6653 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      402 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0     6578 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     5385 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2672 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/graphs/csv_scraper_graph.py
+-rw-r--r--   0        0        0     3594 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/graphs/json_scraper_graph.py
+-rw-r--r--   0        0        0     3880 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     3650 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     3749 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     4575 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0     3738 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/graphs/xml_scraper_graph.py
+-rw-r--r--   0        0        0      202 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0     1171 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      313 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      441 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      463 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      426 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      459 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      427 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      412 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1367 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1221 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      644 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7932 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     3716 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     6987 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/generate_answer_csv_node.py
+-rw-r--r--   0        0        0     6431 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     6987 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/generate_answer_node_csv.py
+-rw-r--r--   0        0        0     6639 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     3527 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1955 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     2684 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     5598 2024-05-02 15:56:25.873046 scrapegraphai-0.6.0/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     5605 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     3707 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     6261 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     2317 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      286 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     2141 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1974 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     4638 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      764 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0      800 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     1442 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1605 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      836 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0     1320 2024-05-02 15:56:25.877046 scrapegraphai-0.6.0/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0    10672 1970-01-01 00:00:00.000000 scrapegraphai-0.6.0/PKG-INFO
```

### Comparing `scrapegraphai-0.5.2/LICENSE` & `scrapegraphai-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/README.md` & `scrapegraphai-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/pyproject.toml` & `scrapegraphai-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [tool.poetry]
 name = "scrapegraphai"
 
-version = "0.5.2"
+version = "0.6.0"
+
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
```

### Comparing `scrapegraphai-0.5.2/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.6.0/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.6.0/scrapegraphai/graphs/abstract_graph.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,28 +37,38 @@
     """
 
     def __init__(self, prompt: str, config: dict, source: Optional[str] = None):
 
         self.prompt = prompt
         self.source = source
         self.config = config
-        self.llm_model = self._create_llm(config["llm"])
+        self.llm_model = self._create_llm(config["llm"], chat=True)
         self.embedder_model = self.llm_model if "embeddings" not in config else self._create_llm(
             config["embeddings"])
 
         # Set common configuration parameters
         self.verbose = True if config is None else config.get("verbose", False)
         self.headless = True if config is None else config.get("headless", True)
 
         # Create the graph
         self.graph = self._create_graph()
         self.final_state = None
         self.execution_info = None
 
-    def _create_llm(self, llm_config: dict) -> object:
+
+    def _set_model_token(self, llm):
+
+        if 'Azure' in str(type(llm)):
+            try:
+                self.model_token = models_tokens["azure"][llm.model_name]
+            except KeyError:
+                raise KeyError("Model not supported")
+
+
+    def _create_llm(self, llm_config: dict, chat=False) -> object:
         """
         Create a large language model instance based on the configuration provided.
 
         Args:
             llm_config (dict): Configuration parameters for the language model.
 
         Returns:
@@ -70,14 +80,20 @@
 
         llm_defaults = {
             "temperature": 0,
             "streaming": False
         }
         llm_params = {**llm_defaults, **llm_config}
 
+        # If model instance is passed directly instead of the model details
+        if 'model_instance' in llm_params:
+            if chat:
+                self._set_model_token(llm_params['model_instance'])
+            return llm_params['model_instance']
+        
         # Instantiate the language model based on the model name
         if "gpt-" in llm_params["model"]:
             try:
                 self.model_token = models_tokens["openai"][llm_params["model"]]
             except KeyError:
                 raise KeyError("Model not supported")
             return OpenAI(llm_params)
@@ -168,7 +184,8 @@
 
     @abstractmethod
     def run(self) -> str:
         """
         Abstract method to execute the graph and return the result.
         """
         pass
+
```

### Comparing `scrapegraphai-0.5.2/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.6.0/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/graphs/json_scraper_graph.py` & `scrapegraphai-0.6.0/scrapegraphai/graphs/json_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.6.0/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.6.0/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.6.0/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.6.0/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/graphs/xml_scraper_graph.py` & `scrapegraphai-0.6.0/scrapegraphai/graphs/xml_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.6.0/scrapegraphai/helpers/models_tokens.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,17 @@
         "gpt-4-1106-preview": 128000,
         "gpt-4-vision-preview": 128000,
         "gpt-4": 8192,
         "gpt-4-0613": 8192,
         "gpt-4-32k": 32768,
         "gpt-4-32k-0613": 32768,
     },
-
+    "azure": {
+        "gpt-3.5-turbo": 4096
+    },
     "gemini": {
         "gemini-pro": 128000,
     },
 
     "ollama": {
         "llama2": 4096,
         "llama3": 8192,
@@ -42,7 +44,8 @@
     "claude": {
         "claude_instant": 100000,
         "claude2": 9000,
         "claude2.1": 200000,
         "claude3": 200000
     }
 }
+
```

### Comparing `scrapegraphai-0.5.2/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.6.0/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.6.0/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.6.0/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.6.0/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/nodes/__init__.py` & `scrapegraphai-0.6.0/scrapegraphai/nodes/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,7 +10,8 @@
 from .rag_node import RAGNode
 from .text_to_speech_node import TextToSpeechNode
 from .image_to_text_node import ImageToTextNode
 from .search_internet_node import SearchInternetNode
 from .generate_scraper_node import GenerateScraperNode
 from .search_link_node import SearchLinkNode
 from .robots_node import RobotsNode
+from .generate_answer_csv_node import GenerateAnswerCSVNode
```

### Comparing `scrapegraphai-0.5.2/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.6.0/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.6.0/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.6.0/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.6.0/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.6.0/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.6.0/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.6.0/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.6.0/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.6.0/scrapegraphai/nodes/rag_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,16 @@
 
         # check if embedder_model is provided, if not use llm_model
         embedding_model = self.embedder_model if self.embedder_model else self.llm_model
 
         if isinstance(embedding_model, OpenAI):
             embeddings = OpenAIEmbeddings(
                 api_key=embedding_model.openai_api_key)
+        elif isinstance(embedding_model, AzureOpenAIEmbeddings):
+            embeddings = embedding_model
         elif isinstance(embedding_model, AzureOpenAI):
             embeddings = AzureOpenAIEmbeddings()
         elif isinstance(embedding_model, Ollama):
             # unwrap the kwargs from the model whihc is a dict
             params = embedding_model._lc_kwargs
             # remove streaming and temperature
             params.pop("streaming", None)
@@ -127,7 +129,8 @@
         compressed_docs = compression_retriever.invoke(user_prompt)
 
         if self.verbose:
             print("--- (tokens compressed and vector stored) ---")
 
         state.update({self.output[0]: compressed_docs})
         return state
+
```

### Comparing `scrapegraphai-0.5.2/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-0.6.0/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.6.0/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-0.6.0/scrapegraphai/nodes/search_link_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.6.0/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.6.0/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.6.0/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.6.0/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.6.0/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-0.6.0/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/utils/remover.py` & `scrapegraphai-0.6.0/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.6.0/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.6.0/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.6.0/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.2/PKG-INFO` & `scrapegraphai-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.5.2
+Version: 0.6.0
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >=3.9,<4.0
```

