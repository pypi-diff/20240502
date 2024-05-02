# Comparing `tmp/scrapegraphai-0.5.0b6.tar.gz` & `tmp/scrapegraphai-0.5.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapegraphai-0.5.0b6.tar", max compression
+gzip compressed data, was "scrapegraphai-0.5.0b7.tar", max compression
```

## Comparing `scrapegraphai-0.5.0b6.tar` & `scrapegraphai-0.5.0b7.tar`

### file list

```diff
@@ -1,54 +1,57 @@
--rw-r--r--   0        0        0     1065 2024-04-30 13:45:13.367901 scrapegraphai-0.5.0b6/LICENSE
--rw-r--r--   0        0        0     8753 2024-04-30 13:45:13.367901 scrapegraphai-0.5.0b6/README.md
--rw-r--r--   0        0        0     1712 2024-04-30 13:45:40.143950 scrapegraphai-0.5.0b6/pyproject.toml
--rw-r--r--   0        0        0       54 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/__init__.py
--rw-r--r--   0        0        0       90 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/builders/__init__.py
--rw-r--r--   0        0        0     6670 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/builders/graph_builder.py
--rw-r--r--   0        0        0      354 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/graphs/__init__.py
--rw-r--r--   0        0        0     4595 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/graphs/abstract_graph.py
--rw-r--r--   0        0        0     5157 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/graphs/base_graph.py
--rw-r--r--   0        0        0     2672 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/graphs/json_scraper_graph.py
--rw-r--r--   0        0        0     2615 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/graphs/script_creator_graph.py
--rw-r--r--   0        0        0     2568 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/graphs/search_graph.py
--rw-r--r--   0        0        0     2692 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/graphs/smart_scraper_graph.py
--rw-r--r--   0        0        0     3478 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/graphs/speech_graph.py
--rw-r--r--   0        0        0     2666 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/graphs/xml_scraper_graph.py
--rw-r--r--   0        0        0      202 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/helpers/__init__.py
--rw-r--r--   0        0        0     1118 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/helpers/models_tokens.py
--rw-r--r--   0        0        0     3807 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/helpers/nodes_metadata.py
--rw-r--r--   0        0        0      310 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/helpers/robots.py
--rw-r--r--   0        0        0     2363 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/helpers/schemas.py
--rw-r--r--   0        0        0      313 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/models/__init__.py
--rw-r--r--   0        0        0      601 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/models/azure_openai.py
--rw-r--r--   0        0        0      651 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/models/gemini.py
--rw-r--r--   0        0        0      611 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/models/groq.py
--rw-r--r--   0        0        0      839 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/models/hugging_face.py
--rw-r--r--   0        0        0      590 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/models/ollama.py
--rw-r--r--   0        0        0      575 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/models/openai.py
--rw-r--r--   0        0        0     1721 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/models/openai_itt.py
--rw-r--r--   0        0        0     1657 2024-04-30 13:45:13.395901 scrapegraphai-0.5.0b6/scrapegraphai/models/openai_tts.py
--rw-r--r--   0        0        0      584 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/nodes/__init__.py
--rw-r--r--   0        0        0     7544 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/nodes/base_node.py
--rw-r--r--   0        0        0     2914 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/nodes/conditional_node.py
--rw-r--r--   0        0        0     4306 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/nodes/fetch_node.py
--rw-r--r--   0        0        0     7005 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/nodes/generate_answer_node.py
--rw-r--r--   0        0        0     7236 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/nodes/generate_scraper_node.py
--rw-r--r--   0        0        0     4097 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/nodes/get_probable_tags_node.py
--rw-r--r--   0        0        0     1724 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/nodes/image_to_text_node.py
--rw-r--r--   0        0        0     3457 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/nodes/parse_node.py
--rw-r--r--   0        0        0     5321 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/nodes/rag_node.py
--rw-r--r--   0        0        0     6627 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/nodes/robots_node.py
--rw-r--r--   0        0        0     4668 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/nodes/search_internet_node.py
--rw-r--r--   0        0        0     6898 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/nodes/search_link_node.py
--rw-r--r--   0        0        0     1754 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/nodes/text_to_speech_node.py
--rw-r--r--   0        0        0      286 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/utils/__init__.py
--rw-r--r--   0        0        0     1742 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/utils/convert_to_csv.py
--rw-r--r--   0        0        0     1443 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/utils/convert_to_json.py
--rw-r--r--   0        0        0     3630 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/utils/parse_state_keys.py
--rw-r--r--   0        0        0      513 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/utils/prettify_exec_info.py
--rw-r--r--   0        0        0      731 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/utils/proxy_rotation.py
--rw-r--r--   0        0        0     1070 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/utils/remover.py
--rw-r--r--   0        0        0     1118 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/utils/research_web.py
--rw-r--r--   0        0        0      631 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/utils/save_audio_from_bytes.py
--rw-r--r--   0        0        0      990 2024-04-30 13:45:13.399901 scrapegraphai-0.5.0b6/scrapegraphai/utils/token_calculator.py
--rw-r--r--   0        0        0    10551 1970-01-01 00:00:00.000000 scrapegraphai-0.5.0b6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-01 19:36:12.932726 scrapegraphai-0.5.0b7/LICENSE
+-rw-r--r--   0        0        0     8753 2024-05-01 19:36:12.932726 scrapegraphai-0.5.0b7/README.md
+-rw-r--r--   0        0        0     1712 2024-05-01 19:36:32.480991 scrapegraphai-0.5.0b7/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-05-01 19:36:12.960726 scrapegraphai-0.5.0b7/scrapegraphai/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-01 19:36:12.960726 scrapegraphai-0.5.0b7/scrapegraphai/builders/__init__.py
+-rw-r--r--   0        0        0     6670 2024-05-01 19:36:12.960726 scrapegraphai-0.5.0b7/scrapegraphai/builders/graph_builder.py
+-rw-r--r--   0        0        0      401 2024-05-01 19:36:12.960726 scrapegraphai-0.5.0b7/scrapegraphai/graphs/__init__.py
+-rw-r--r--   0        0        0     4595 2024-05-01 19:36:12.960726 scrapegraphai-0.5.0b7/scrapegraphai/graphs/abstract_graph.py
+-rw-r--r--   0        0        0     5157 2024-05-01 19:36:12.960726 scrapegraphai-0.5.0b7/scrapegraphai/graphs/base_graph.py
+-rw-r--r--   0        0        0     2672 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/graphs/csv_scraper_graph.py
+-rw-r--r--   0        0        0     2672 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/graphs/json_scraper_graph.py
+-rw-r--r--   0        0        0     2615 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/graphs/script_creator_graph.py
+-rw-r--r--   0        0        0     2568 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/graphs/search_graph.py
+-rw-r--r--   0        0        0     2692 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/graphs/smart_scraper_graph.py
+-rw-r--r--   0        0        0     3478 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/graphs/speech_graph.py
+-rw-r--r--   0        0        0     2666 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/graphs/xml_scraper_graph.py
+-rw-r--r--   0        0        0      202 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/helpers/__init__.py
+-rw-r--r--   0        0        0     1118 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/helpers/models_tokens.py
+-rw-r--r--   0        0        0     3807 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/helpers/nodes_metadata.py
+-rw-r--r--   0        0        0      310 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/helpers/robots.py
+-rw-r--r--   0        0        0     2363 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/helpers/schemas.py
+-rw-r--r--   0        0        0      313 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/models/__init__.py
+-rw-r--r--   0        0        0      601 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/models/azure_openai.py
+-rw-r--r--   0        0        0      651 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/models/gemini.py
+-rw-r--r--   0        0        0      611 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/models/groq.py
+-rw-r--r--   0        0        0      839 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/models/hugging_face.py
+-rw-r--r--   0        0        0      590 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/models/ollama.py
+-rw-r--r--   0        0        0      575 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/models/openai.py
+-rw-r--r--   0        0        0     1721 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/models/openai_itt.py
+-rw-r--r--   0        0        0     1657 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/models/openai_tts.py
+-rw-r--r--   0        0        0      644 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/nodes/__init__.py
+-rw-r--r--   0        0        0     7544 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/nodes/base_node.py
+-rw-r--r--   0        0        0     2914 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/nodes/conditional_node.py
+-rw-r--r--   0        0        0     4306 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/nodes/fetch_node.py
+-rw-r--r--   0        0        0     6987 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/nodes/generate_answer_csv_node.py
+-rw-r--r--   0        0        0     7005 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/nodes/generate_answer_node.py
+-rw-r--r--   0        0        0     6987 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/nodes/generate_answer_node_csv.py
+-rw-r--r--   0        0        0     7236 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/nodes/generate_scraper_node.py
+-rw-r--r--   0        0        0     4097 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/nodes/get_probable_tags_node.py
+-rw-r--r--   0        0        0     1724 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/nodes/image_to_text_node.py
+-rw-r--r--   0        0        0     3457 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/nodes/parse_node.py
+-rw-r--r--   0        0        0     5321 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/nodes/rag_node.py
+-rw-r--r--   0        0        0     6627 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/nodes/robots_node.py
+-rw-r--r--   0        0        0     4668 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/nodes/search_internet_node.py
+-rw-r--r--   0        0        0     6898 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/nodes/search_link_node.py
+-rw-r--r--   0        0        0     1754 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/nodes/text_to_speech_node.py
+-rw-r--r--   0        0        0      286 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/utils/__init__.py
+-rw-r--r--   0        0        0     1742 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/utils/convert_to_csv.py
+-rw-r--r--   0        0        0     1443 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/utils/convert_to_json.py
+-rw-r--r--   0        0        0     3630 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/utils/parse_state_keys.py
+-rw-r--r--   0        0        0      513 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/utils/prettify_exec_info.py
+-rw-r--r--   0        0        0      731 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/utils/proxy_rotation.py
+-rw-r--r--   0        0        0     1070 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/utils/remover.py
+-rw-r--r--   0        0        0     1118 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/utils/research_web.py
+-rw-r--r--   0        0        0      631 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/utils/save_audio_from_bytes.py
+-rw-r--r--   0        0        0      990 2024-05-01 19:36:12.964727 scrapegraphai-0.5.0b7/scrapegraphai/utils/token_calculator.py
+-rw-r--r--   0        0        0    10551 1970-01-01 00:00:00.000000 scrapegraphai-0.5.0b7/PKG-INFO
```

### Comparing `scrapegraphai-0.5.0b6/LICENSE` & `scrapegraphai-0.5.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/README.md` & `scrapegraphai-0.5.0b7/README.md`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/pyproject.toml` & `scrapegraphai-0.5.0b7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "scrapegraphai"
 
-version = "0.5.0b6"
+version = "0.5.0b7"
 
 description = "A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines."
 authors = [
     "Marco Vinciguerra <mvincig11@gmail.com>",
     "Marco Perini <perinim.98@gmail.com>",
     "Lorenzo Padoan <lorenzo.padoan977@gmail.com>"
 ]
```

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/builders/graph_builder.py` & `scrapegraphai-0.5.0b7/scrapegraphai/builders/graph_builder.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/graphs/abstract_graph.py` & `scrapegraphai-0.5.0b7/scrapegraphai/graphs/abstract_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/graphs/base_graph.py` & `scrapegraphai-0.5.0b7/scrapegraphai/graphs/base_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/graphs/json_scraper_graph.py` & `scrapegraphai-0.5.0b7/scrapegraphai/graphs/json_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/graphs/script_creator_graph.py` & `scrapegraphai-0.5.0b7/scrapegraphai/graphs/script_creator_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/graphs/search_graph.py` & `scrapegraphai-0.5.0b7/scrapegraphai/graphs/search_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/graphs/smart_scraper_graph.py` & `scrapegraphai-0.5.0b7/scrapegraphai/graphs/smart_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/graphs/speech_graph.py` & `scrapegraphai-0.5.0b7/scrapegraphai/graphs/speech_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/graphs/xml_scraper_graph.py` & `scrapegraphai-0.5.0b7/scrapegraphai/graphs/xml_scraper_graph.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/helpers/models_tokens.py` & `scrapegraphai-0.5.0b7/scrapegraphai/helpers/models_tokens.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/helpers/nodes_metadata.py` & `scrapegraphai-0.5.0b7/scrapegraphai/helpers/nodes_metadata.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/helpers/schemas.py` & `scrapegraphai-0.5.0b7/scrapegraphai/helpers/schemas.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/models/azure_openai.py` & `scrapegraphai-0.5.0b7/scrapegraphai/models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/models/gemini.py` & `scrapegraphai-0.5.0b7/scrapegraphai/models/gemini.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/models/groq.py` & `scrapegraphai-0.5.0b7/scrapegraphai/models/groq.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/models/hugging_face.py` & `scrapegraphai-0.5.0b7/scrapegraphai/models/hugging_face.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/models/ollama.py` & `scrapegraphai-0.5.0b7/scrapegraphai/models/ollama.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/models/openai.py` & `scrapegraphai-0.5.0b7/scrapegraphai/models/openai.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/models/openai_itt.py` & `scrapegraphai-0.5.0b7/scrapegraphai/models/openai_itt.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/models/openai_tts.py` & `scrapegraphai-0.5.0b7/scrapegraphai/models/openai_tts.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/nodes/__init__.py` & `scrapegraphai-0.5.0b7/scrapegraphai/nodes/__init__.py`

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

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/nodes/base_node.py` & `scrapegraphai-0.5.0b7/scrapegraphai/nodes/base_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/nodes/conditional_node.py` & `scrapegraphai-0.5.0b7/scrapegraphai/nodes/conditional_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/nodes/fetch_node.py` & `scrapegraphai-0.5.0b7/scrapegraphai/nodes/fetch_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/nodes/generate_answer_node.py` & `scrapegraphai-0.5.0b7/scrapegraphai/nodes/generate_answer_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/nodes/generate_scraper_node.py` & `scrapegraphai-0.5.0b7/scrapegraphai/nodes/generate_scraper_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/nodes/get_probable_tags_node.py` & `scrapegraphai-0.5.0b7/scrapegraphai/nodes/get_probable_tags_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/nodes/image_to_text_node.py` & `scrapegraphai-0.5.0b7/scrapegraphai/nodes/image_to_text_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/nodes/parse_node.py` & `scrapegraphai-0.5.0b7/scrapegraphai/nodes/parse_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/nodes/rag_node.py` & `scrapegraphai-0.5.0b7/scrapegraphai/nodes/rag_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/nodes/robots_node.py` & `scrapegraphai-0.5.0b7/scrapegraphai/nodes/robots_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/nodes/search_internet_node.py` & `scrapegraphai-0.5.0b7/scrapegraphai/nodes/search_internet_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/nodes/search_link_node.py` & `scrapegraphai-0.5.0b7/scrapegraphai/nodes/search_link_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/nodes/text_to_speech_node.py` & `scrapegraphai-0.5.0b7/scrapegraphai/nodes/text_to_speech_node.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/utils/convert_to_csv.py` & `scrapegraphai-0.5.0b7/scrapegraphai/utils/convert_to_csv.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/utils/convert_to_json.py` & `scrapegraphai-0.5.0b7/scrapegraphai/utils/convert_to_json.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/utils/parse_state_keys.py` & `scrapegraphai-0.5.0b7/scrapegraphai/utils/parse_state_keys.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/utils/prettify_exec_info.py` & `scrapegraphai-0.5.0b7/scrapegraphai/utils/prettify_exec_info.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/utils/proxy_rotation.py` & `scrapegraphai-0.5.0b7/scrapegraphai/utils/proxy_rotation.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/utils/remover.py` & `scrapegraphai-0.5.0b7/scrapegraphai/utils/remover.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/utils/research_web.py` & `scrapegraphai-0.5.0b7/scrapegraphai/utils/research_web.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/utils/save_audio_from_bytes.py` & `scrapegraphai-0.5.0b7/scrapegraphai/utils/save_audio_from_bytes.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/scrapegraphai/utils/token_calculator.py` & `scrapegraphai-0.5.0b7/scrapegraphai/utils/token_calculator.py`

 * *Files identical despite different names*

### Comparing `scrapegraphai-0.5.0b6/PKG-INFO` & `scrapegraphai-0.5.0b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapegraphai
-Version: 0.5.0b6
+Version: 0.5.0b7
 Summary: A web scraping library based on LangChain which uses LLM and direct graph logic to create scraping pipelines.
 Home-page: https://scrapegraph-ai.readthedocs.io/
 License: MIT
 Keywords: scrapegraph,scrapegraphai,langchain,ai,artificial intelligence,gpt,machine learning,rag,nlp,natural language processing,openai,scraping,web scraping,web scraping library,web scraping tool,webscraping,graph
 Author: Marco Vinciguerra
 Author-email: mvincig11@gmail.com
 Requires-Python: >=3.9,<4.0
```

