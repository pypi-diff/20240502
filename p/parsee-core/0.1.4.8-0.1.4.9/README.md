# Comparing `tmp/parsee_core-0.1.4.8.tar.gz` & `tmp/parsee_core-0.1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsee_core-0.1.4.8.tar", max compression
+gzip compressed data, was "parsee_core-0.1.4.9.tar", max compression
```

## Comparing `parsee_core-0.1.4.8.tar` & `parsee_core-0.1.4.9.tar`

### file list

```diff
@@ -1,75 +1,76 @@
--rw-r--r--   0        0        0     1066 2024-03-21 12:33:53.103983 parsee_core-0.1.4.8/LICENSE
--rw-r--r--   0        0        0      529 2024-03-27 13:19:30.023928 parsee_core-0.1.4.8/parsee/__init__.py
--rw-r--r--   0        0        0     5174 2024-04-12 10:32:38.964069 parsee_core-0.1.4.8/parsee/cloud/api.py
--rw-r--r--   0        0        0     1093 2024-04-12 10:39:58.510402 parsee_core-0.1.4.8/parsee/cloud/cloud_image_fetcher.py
--rw-r--r--   0        0        0        0 2023-07-26 14:50:21.298000 parsee_core-0.1.4.8/parsee/converters/__init__.py
--rw-r--r--   0        0        0     6063 2024-03-29 10:54:00.293459 parsee_core-0.1.4.8/parsee/converters/html_extraction.py
--rw-r--r--   0        0        0     3752 2024-04-12 10:39:58.514327 parsee_core-0.1.4.8/parsee/converters/image_creation.py
--rw-r--r--   0        0        0      399 2024-03-27 13:22:36.894150 parsee_core-0.1.4.8/parsee/converters/interfaces.py
--rw-r--r--   0        0        0     1806 2024-04-10 14:57:20.432097 parsee_core-0.1.4.8/parsee/converters/json_to_raw.py
--rw-r--r--   0        0        0     1069 2024-04-10 14:57:20.432511 parsee_core-0.1.4.8/parsee/converters/langchain.py
--rw-r--r--   0        0        0     3015 2024-04-10 14:57:20.432769 parsee_core-0.1.4.8/parsee/converters/main.py
--rw-r--r--   0        0        0     4324 2024-03-27 13:19:30.029388 parsee_core-0.1.4.8/parsee/converters/pdf_extraction.py
--rw-r--r--   0        0        0      491 2024-03-27 13:22:36.895882 parsee_core-0.1.4.8/parsee/converters/simple_text.py
--rw-r--r--   0        0        0     6680 2024-03-25 10:47:46.831244 parsee_core-0.1.4.8/parsee/datasets/dataset_dataclasses.py
--rw-r--r--   0        0        0     7820 2024-03-20 10:51:40.783264 parsee_core-0.1.4.8/parsee/datasets/evaluation/main.py
--rw-r--r--   0        0        0     2645 2024-03-01 12:41:34.973375 parsee_core-0.1.4.8/parsee/datasets/main.py
--rw-r--r--   0        0        0     3538 2024-02-15 11:15:28.539480 parsee_core-0.1.4.8/parsee/datasets/readers/disk_reader.py
--rw-r--r--   0        0        0     1422 2024-02-14 09:53:17.733410 parsee_core-0.1.4.8/parsee/datasets/readers/interfaces.py
--rw-r--r--   0        0        0     1883 2024-02-14 10:08:53.958308 parsee_core-0.1.4.8/parsee/datasets/writers/disk_writer.py
--rw-r--r--   0        0        0     1084 2024-02-14 09:53:17.701394 parsee_core-0.1.4.8/parsee/datasets/writers/interfaces.py
--rw-r--r--   0        0        0        0 2022-08-08 15:31:09.039000 parsee_core-0.1.4.8/parsee/extraction/__init__.py
--rw-r--r--   0        0        0     4138 2024-04-11 14:09:13.370382 parsee_core-0.1.4.8/parsee/extraction/extractor_dataclasses.py
--rw-r--r--   0        0        0    30049 2024-04-13 09:32:29.198541 parsee_core-0.1.4.8/parsee/extraction/extractor_elements.py
--rw-r--r--   0        0        0     9472 2024-04-05 15:38:22.487342 parsee_core-0.1.4.8/parsee/extraction/final_structuring.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.686000 parsee_core-0.1.4.8/parsee/extraction/models/__init__.py
--rw-r--r--   0        0        0     2062 2024-04-10 14:57:20.433864 parsee_core-0.1.4.8/parsee/extraction/models/helpers.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.686000 parsee_core-0.1.4.8/parsee/extraction/models/llm_models/__init__.py
--rw-r--r--   0        0        0     2882 2024-04-10 14:57:20.434116 parsee_core-0.1.4.8/parsee/extraction/models/llm_models/anthropic_model.py
--rw-r--r--   0        0        0     2866 2024-04-10 14:57:20.434321 parsee_core-0.1.4.8/parsee/extraction/models/llm_models/chatgpt_model.py
--rw-r--r--   0        0        0      888 2024-04-10 14:57:20.434563 parsee_core-0.1.4.8/parsee/extraction/models/llm_models/llm_base_model.py
--rw-r--r--   0        0        0     1694 2024-04-10 14:57:20.434940 parsee_core-0.1.4.8/parsee/extraction/models/llm_models/ollama_model.py
--rw-r--r--   0        0        0      875 2024-04-10 14:57:20.435213 parsee_core-0.1.4.8/parsee/extraction/models/llm_models/prompts.py
--rw-r--r--   0        0        0     1971 2024-04-10 14:57:20.435485 parsee_core-0.1.4.8/parsee/extraction/models/llm_models/replicate_model.py
--rw-r--r--   0        0        0     7890 2024-04-13 12:45:28.238384 parsee_core-0.1.4.8/parsee/extraction/models/llm_models/structuring_schema.py
--rw-r--r--   0        0        0      985 2024-04-10 14:57:20.435851 parsee_core-0.1.4.8/parsee/extraction/models/model_dataclasses.py
--rw-r--r--   0        0        0     8163 2024-03-20 12:24:18.192932 parsee_core-0.1.4.8/parsee/extraction/models/model_loader.py
--rw-r--r--   0        0        0     4651 2024-04-12 11:29:47.420418 parsee_core-0.1.4.8/parsee/extraction/run.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.8/parsee/extraction/tasks/__init__.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.8/parsee/extraction/tasks/element_classification/__init__.py
--rw-r--r--   0        0        0     1756 2024-02-22 09:52:47.322977 parsee_core-0.1.4.8/parsee/extraction/tasks/element_classification/element_model.py
--rw-r--r--   0        0        0     2207 2024-04-15 21:34:41.015208 parsee_core-0.1.4.8/parsee/extraction/tasks/element_classification/element_model_llm.py
--rw-r--r--   0        0        0     8051 2024-04-10 14:57:20.436667 parsee_core-0.1.4.8/parsee/extraction/tasks/element_classification/features.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.8/parsee/extraction/tasks/mappings/__init__.py
--rw-r--r--   0        0        0     6108 2024-04-04 15:01:44.484913 parsee_core-0.1.4.8/parsee/extraction/tasks/mappings/features.py
--rw-r--r--   0        0        0     1493 2024-02-22 09:52:47.319414 parsee_core-0.1.4.8/parsee/extraction/tasks/mappings/mapping_model.py
--rw-r--r--   0        0        0     2527 2024-04-15 21:34:41.012205 parsee_core-0.1.4.8/parsee/extraction/tasks/mappings/mapping_model_llm.py
--rw-r--r--   0        0        0      894 2024-03-28 20:25:58.634238 parsee_core-0.1.4.8/parsee/extraction/tasks/mappings/utils.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.688000 parsee_core-0.1.4.8/parsee/extraction/tasks/meta_info_structuring/__init__.py
--rw-r--r--   0        0        0    13073 2024-04-10 14:57:20.437207 parsee_core-0.1.4.8/parsee/extraction/tasks/meta_info_structuring/features.py
--rw-r--r--   0        0        0      729 2024-02-22 09:52:47.324193 parsee_core-0.1.4.8/parsee/extraction/tasks/meta_info_structuring/meta_info.py
--rw-r--r--   0        0        0     2649 2024-04-15 21:34:41.003866 parsee_core-0.1.4.8/parsee/extraction/tasks/meta_info_structuring/meta_info_llm.py
--rw-r--r--   0        0        0        0 2023-11-24 15:51:09.688000 parsee_core-0.1.4.8/parsee/extraction/tasks/questions/__init__.py
--rw-r--r--   0        0        0     6371 2024-04-13 09:30:58.743777 parsee_core-0.1.4.8/parsee/extraction/tasks/questions/features.py
--rw-r--r--   0        0        0     1430 2024-03-01 12:41:34.971601 parsee_core-0.1.4.8/parsee/extraction/tasks/questions/question_model.py
--rw-r--r--   0        0        0     4031 2024-04-10 14:57:20.438067 parsee_core-0.1.4.8/parsee/extraction/tasks/questions/question_model_llm.py
--rw-r--r--   0        0        0     2678 2024-03-12 17:16:10.730178 parsee_core-0.1.4.8/parsee/extraction/tasks/questions/utils.py
--rw-r--r--   0        0        0        0 2023-08-08 14:40:07.901000 parsee_core-0.1.4.8/parsee/storage/__init__.py
--rw-r--r--   0        0        0     2491 2024-04-12 10:17:23.380409 parsee_core-0.1.4.8/parsee/storage/in_memory_storage.py
--rw-r--r--   0        0        0     1212 2024-04-10 14:57:20.438565 parsee_core-0.1.4.8/parsee/storage/interfaces.py
--rw-r--r--   0        0        0      317 2024-02-21 09:46:14.327121 parsee_core-0.1.4.8/parsee/storage/vector_stores/interfaces.py
--rw-r--r--   0        0        0     3204 2024-03-22 17:12:35.963569 parsee_core-0.1.4.8/parsee/storage/vector_stores/simple_faiss.py
--rw-r--r--   0        0        0        0 2023-08-03 13:44:22.929000 parsee_core-0.1.4.8/parsee/templates/__init__.py
--rw-r--r--   0        0        0     1360 2024-04-05 15:38:22.487748 parsee_core-0.1.4.8/parsee/templates/element_schema.py
--rw-r--r--   0        0        0     1959 2024-02-22 09:42:26.246323 parsee_core-0.1.4.8/parsee/templates/general_structuring_schema.py
--rw-r--r--   0        0        0     4019 2024-04-05 15:38:22.488067 parsee_core-0.1.4.8/parsee/templates/helpers.py
--rw-r--r--   0        0        0     1288 2024-02-22 09:33:07.394404 parsee_core-0.1.4.8/parsee/templates/job_template.py
--rw-r--r--   0        0        0     1011 2024-02-14 09:53:17.727343 parsee_core-0.1.4.8/parsee/templates/mappings.py
--rw-r--r--   0        0        0      384 2024-02-14 09:50:55.308500 parsee_core-0.1.4.8/parsee/templates/template_from_json.py
--rw-r--r--   0        0        0        0 2023-07-26 14:15:43.630000 parsee_core-0.1.4.8/parsee/utils/__init__.py
--rw-r--r--   0        0        0      405 2024-02-15 14:56:20.018887 parsee_core-0.1.4.8/parsee/utils/constants.py
--rw-r--r--   0        0        0      781 2024-03-27 13:19:30.038637 parsee_core-0.1.4.8/parsee/utils/enums.py
--rw-r--r--   0        0        0     6632 2024-04-08 08:51:44.149915 parsee_core-0.1.4.8/parsee/utils/helper.py
--rw-r--r--   0        0        0     2030 2024-03-26 12:40:38.547700 parsee_core-0.1.4.8/parsee/utils/sample_items.py
--rw-r--r--   0        0        0      827 2024-04-15 21:34:41.009401 parsee_core-0.1.4.8/pyproject.toml
--rw-r--r--   0        0        0     1064 1970-01-01 00:00:00.000000 parsee_core-0.1.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-21 12:33:53.103983 parsee_core-0.1.4.9/LICENSE
+-rw-r--r--   0        0        0      469 2024-04-16 15:57:05.188010 parsee_core-0.1.4.9/parsee/__init__.py
+-rw-r--r--   0        0        0     5174 2024-04-12 10:32:38.964069 parsee_core-0.1.4.9/parsee/cloud/api.py
+-rw-r--r--   0        0        0     1093 2024-04-12 10:39:58.510402 parsee_core-0.1.4.9/parsee/cloud/cloud_image_fetcher.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:50:21.298000 parsee_core-0.1.4.9/parsee/converters/__init__.py
+-rw-r--r--   0        0        0     6063 2024-03-29 10:54:00.293459 parsee_core-0.1.4.9/parsee/converters/html_extraction.py
+-rw-r--r--   0        0        0     3752 2024-04-12 10:39:58.514327 parsee_core-0.1.4.9/parsee/converters/image_creation.py
+-rw-r--r--   0        0        0      399 2024-03-27 13:22:36.894150 parsee_core-0.1.4.9/parsee/converters/interfaces.py
+-rw-r--r--   0        0        0     1806 2024-04-10 14:57:20.432097 parsee_core-0.1.4.9/parsee/converters/json_to_raw.py
+-rw-r--r--   0        0        0     1069 2024-04-10 14:57:20.432511 parsee_core-0.1.4.9/parsee/converters/langchain.py
+-rw-r--r--   0        0        0     3015 2024-04-10 14:57:20.432769 parsee_core-0.1.4.9/parsee/converters/main.py
+-rw-r--r--   0        0        0     4324 2024-03-27 13:19:30.029388 parsee_core-0.1.4.9/parsee/converters/pdf_extraction.py
+-rw-r--r--   0        0        0      491 2024-03-27 13:22:36.895882 parsee_core-0.1.4.9/parsee/converters/simple_text.py
+-rw-r--r--   0        0        0     6681 2024-04-16 15:57:07.458639 parsee_core-0.1.4.9/parsee/datasets/dataset_dataclasses.py
+-rw-r--r--   0        0        0     8710 2024-04-16 15:57:07.458964 parsee_core-0.1.4.9/parsee/datasets/evaluation/main.py
+-rw-r--r--   0        0        0     2765 2024-04-16 15:57:07.459219 parsee_core-0.1.4.9/parsee/datasets/main.py
+-rw-r--r--   0        0        0     3538 2024-04-16 15:24:41.145825 parsee_core-0.1.4.9/parsee/datasets/readers/disk_reader.py
+-rw-r--r--   0        0        0     1422 2024-02-14 09:53:17.733410 parsee_core-0.1.4.9/parsee/datasets/readers/interfaces.py
+-rw-r--r--   0        0        0     1883 2024-02-14 10:08:53.958308 parsee_core-0.1.4.9/parsee/datasets/writers/disk_writer.py
+-rw-r--r--   0        0        0     1084 2024-02-14 09:53:17.701394 parsee_core-0.1.4.9/parsee/datasets/writers/interfaces.py
+-rw-r--r--   0        0        0        0 2022-08-08 15:31:09.039000 parsee_core-0.1.4.9/parsee/extraction/__init__.py
+-rw-r--r--   0        0        0     4138 2024-04-11 14:09:13.370382 parsee_core-0.1.4.9/parsee/extraction/extractor_dataclasses.py
+-rw-r--r--   0        0        0    30049 2024-04-13 09:32:29.198541 parsee_core-0.1.4.9/parsee/extraction/extractor_elements.py
+-rw-r--r--   0        0        0     9472 2024-04-05 15:38:22.487342 parsee_core-0.1.4.9/parsee/extraction/final_structuring.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.686000 parsee_core-0.1.4.9/parsee/extraction/models/__init__.py
+-rw-r--r--   0        0        0     2458 2024-04-16 15:57:05.188295 parsee_core-0.1.4.9/parsee/extraction/models/helpers.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.686000 parsee_core-0.1.4.9/parsee/extraction/models/llm_models/__init__.py
+-rw-r--r--   0        0        0     2882 2024-04-10 14:57:20.434116 parsee_core-0.1.4.9/parsee/extraction/models/llm_models/anthropic_model.py
+-rw-r--r--   0        0        0     2866 2024-04-16 08:36:24.430947 parsee_core-0.1.4.9/parsee/extraction/models/llm_models/chatgpt_model.py
+-rw-r--r--   0        0        0      888 2024-04-10 14:57:20.434563 parsee_core-0.1.4.9/parsee/extraction/models/llm_models/llm_base_model.py
+-rw-r--r--   0        0        0     1694 2024-04-10 14:57:20.434940 parsee_core-0.1.4.9/parsee/extraction/models/llm_models/ollama_model.py
+-rw-r--r--   0        0        0      875 2024-04-10 14:57:20.435213 parsee_core-0.1.4.9/parsee/extraction/models/llm_models/prompts.py
+-rw-r--r--   0        0        0     1971 2024-04-10 14:57:20.435485 parsee_core-0.1.4.9/parsee/extraction/models/llm_models/replicate_model.py
+-rw-r--r--   0        0        0     7890 2024-04-13 12:45:28.238384 parsee_core-0.1.4.9/parsee/extraction/models/llm_models/structuring_schema.py
+-rw-r--r--   0        0        0     1646 2024-04-16 15:57:07.459506 parsee_core-0.1.4.9/parsee/extraction/models/llm_models/together_model.py
+-rw-r--r--   0        0        0      985 2024-04-10 14:57:20.435851 parsee_core-0.1.4.9/parsee/extraction/models/model_dataclasses.py
+-rw-r--r--   0        0        0     8323 2024-04-16 15:57:05.188730 parsee_core-0.1.4.9/parsee/extraction/models/model_loader.py
+-rw-r--r--   0        0        0     4651 2024-04-12 11:29:47.420418 parsee_core-0.1.4.9/parsee/extraction/run.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.9/parsee/extraction/tasks/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.9/parsee/extraction/tasks/element_classification/__init__.py
+-rw-r--r--   0        0        0     1756 2024-02-22 09:52:47.322977 parsee_core-0.1.4.9/parsee/extraction/tasks/element_classification/element_model.py
+-rw-r--r--   0        0        0     2207 2024-04-15 21:34:41.015208 parsee_core-0.1.4.9/parsee/extraction/tasks/element_classification/element_model_llm.py
+-rw-r--r--   0        0        0     8051 2024-04-10 14:57:20.436667 parsee_core-0.1.4.9/parsee/extraction/tasks/element_classification/features.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.687000 parsee_core-0.1.4.9/parsee/extraction/tasks/mappings/__init__.py
+-rw-r--r--   0        0        0     6108 2024-04-04 15:01:44.484913 parsee_core-0.1.4.9/parsee/extraction/tasks/mappings/features.py
+-rw-r--r--   0        0        0     1493 2024-02-22 09:52:47.319414 parsee_core-0.1.4.9/parsee/extraction/tasks/mappings/mapping_model.py
+-rw-r--r--   0        0        0     2527 2024-04-15 21:34:41.012205 parsee_core-0.1.4.9/parsee/extraction/tasks/mappings/mapping_model_llm.py
+-rw-r--r--   0        0        0      894 2024-03-28 20:25:58.634238 parsee_core-0.1.4.9/parsee/extraction/tasks/mappings/utils.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.688000 parsee_core-0.1.4.9/parsee/extraction/tasks/meta_info_structuring/__init__.py
+-rw-r--r--   0        0        0    13073 2024-04-10 14:57:20.437207 parsee_core-0.1.4.9/parsee/extraction/tasks/meta_info_structuring/features.py
+-rw-r--r--   0        0        0      729 2024-02-22 09:52:47.324193 parsee_core-0.1.4.9/parsee/extraction/tasks/meta_info_structuring/meta_info.py
+-rw-r--r--   0        0        0     2649 2024-04-15 21:34:41.003866 parsee_core-0.1.4.9/parsee/extraction/tasks/meta_info_structuring/meta_info_llm.py
+-rw-r--r--   0        0        0        0 2023-11-24 15:51:09.688000 parsee_core-0.1.4.9/parsee/extraction/tasks/questions/__init__.py
+-rw-r--r--   0        0        0     6224 2024-04-16 15:57:07.459782 parsee_core-0.1.4.9/parsee/extraction/tasks/questions/features.py
+-rw-r--r--   0        0        0     1430 2024-03-01 12:41:34.971601 parsee_core-0.1.4.9/parsee/extraction/tasks/questions/question_model.py
+-rw-r--r--   0        0        0     4141 2024-04-16 15:57:07.460031 parsee_core-0.1.4.9/parsee/extraction/tasks/questions/question_model_llm.py
+-rw-r--r--   0        0        0     2678 2024-03-12 17:16:10.730178 parsee_core-0.1.4.9/parsee/extraction/tasks/questions/utils.py
+-rw-r--r--   0        0        0        0 2023-08-08 14:40:07.901000 parsee_core-0.1.4.9/parsee/storage/__init__.py
+-rw-r--r--   0        0        0     2491 2024-04-12 10:17:23.380409 parsee_core-0.1.4.9/parsee/storage/in_memory_storage.py
+-rw-r--r--   0        0        0     1212 2024-04-10 14:57:20.438565 parsee_core-0.1.4.9/parsee/storage/interfaces.py
+-rw-r--r--   0        0        0      317 2024-02-21 09:46:14.327121 parsee_core-0.1.4.9/parsee/storage/vector_stores/interfaces.py
+-rw-r--r--   0        0        0     3204 2024-03-22 17:12:35.963569 parsee_core-0.1.4.9/parsee/storage/vector_stores/simple_faiss.py
+-rw-r--r--   0        0        0        0 2023-08-03 13:44:22.929000 parsee_core-0.1.4.9/parsee/templates/__init__.py
+-rw-r--r--   0        0        0     1360 2024-04-05 15:38:22.487748 parsee_core-0.1.4.9/parsee/templates/element_schema.py
+-rw-r--r--   0        0        0     1959 2024-02-22 09:42:26.246323 parsee_core-0.1.4.9/parsee/templates/general_structuring_schema.py
+-rw-r--r--   0        0        0     4019 2024-04-05 15:38:22.488067 parsee_core-0.1.4.9/parsee/templates/helpers.py
+-rw-r--r--   0        0        0     1288 2024-02-22 09:33:07.394404 parsee_core-0.1.4.9/parsee/templates/job_template.py
+-rw-r--r--   0        0        0     1011 2024-02-14 09:53:17.727343 parsee_core-0.1.4.9/parsee/templates/mappings.py
+-rw-r--r--   0        0        0      384 2024-02-14 09:50:55.308500 parsee_core-0.1.4.9/parsee/templates/template_from_json.py
+-rw-r--r--   0        0        0        0 2023-07-26 14:15:43.630000 parsee_core-0.1.4.9/parsee/utils/__init__.py
+-rw-r--r--   0        0        0      405 2024-02-15 14:56:20.018887 parsee_core-0.1.4.9/parsee/utils/constants.py
+-rw-r--r--   0        0        0      807 2024-04-16 15:57:05.188954 parsee_core-0.1.4.9/parsee/utils/enums.py
+-rw-r--r--   0        0        0     6632 2024-04-08 08:51:44.149915 parsee_core-0.1.4.9/parsee/utils/helper.py
+-rw-r--r--   0        0        0     2030 2024-03-26 12:40:38.547700 parsee_core-0.1.4.9/parsee/utils/sample_items.py
+-rw-r--r--   0        0        0      847 2024-04-16 15:57:07.460289 parsee_core-0.1.4.9/pyproject.toml
+-rw-r--r--   0        0        0     1105 1970-01-01 00:00:00.000000 parsee_core-0.1.4.9/PKG-INFO
```

### Comparing `parsee_core-0.1.4.8/LICENSE` & `parsee_core-0.1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/__init__.py` & `parsee_core-0.1.4.9/parsee/extraction/tasks/meta_info_structuring/meta_info.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,19 @@
-# This is also defined in setup.py and must be updated in both places.
-__version__ = "0.1.0"
+from typing import List, Dict, Optional
 
-# top level imports
-from parsee.cloud.api import ParseeCloud
-from parsee.templates.helpers import MetaItem, StructuringItem, TableItem, create_template
-from parsee.extraction.models.helpers import gpt_config, replicate_config, anthropic_config, ollama_config
-from parsee.converters.main import load_document, from_text
-from parsee.extraction.run import run_job_with_single_model
-from parsee.utils.enums import OutputType, DocumentType
+from parsee.extraction.extractor_elements import ExtractedEl, FinalOutputTableColumn
+from parsee.templates.general_structuring_schema import StructuringItemSchema
+from parsee.extraction.extractor_dataclasses import ParseeMeta, ExtractedSource
+from parsee.extraction.tasks.meta_info_structuring.features import MetaFeatureBuilder
+
+
+class MetaInfoModel:
+
+    model_name = ""
+    feature_builder: MetaFeatureBuilder
+
+    def __init__(self, items: List[StructuringItemSchema]):
+        self.items = items
+
+    def predict_meta(self, columns: List[FinalOutputTableColumn], elements: List[ExtractedEl]) -> List[List[ParseeMeta]]:
+        # returns meta information
+        raise NotImplemented
```

### Comparing `parsee_core-0.1.4.8/parsee/cloud/api.py` & `parsee_core-0.1.4.9/parsee/cloud/api.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/cloud/cloud_image_fetcher.py` & `parsee_core-0.1.4.9/parsee/cloud/cloud_image_fetcher.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/converters/html_extraction.py` & `parsee_core-0.1.4.9/parsee/converters/html_extraction.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/converters/image_creation.py` & `parsee_core-0.1.4.9/parsee/converters/image_creation.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/converters/json_to_raw.py` & `parsee_core-0.1.4.9/parsee/converters/json_to_raw.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/converters/langchain.py` & `parsee_core-0.1.4.9/parsee/converters/langchain.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/converters/main.py` & `parsee_core-0.1.4.9/parsee/converters/main.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/converters/pdf_extraction.py` & `parsee_core-0.1.4.9/parsee/converters/pdf_extraction.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/datasets/dataset_dataclasses.py` & `parsee_core-0.1.4.9/parsee/datasets/dataset_dataclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import *
 from dataclasses import dataclass
 from enum import Enum
 
 from parsee.utils.constants import ID_NOT_CONFIGURED
 
 
-TRUTH_PREFIX = "TRUTH"
+TRUTH_PREFIX = "ANSWER"
 FEATURE_PREFIX = "FEATURE"
 
 
 @dataclass(frozen=True)
 class DatasetColumn:
     col_idx: int
     col_name: str
```

### Comparing `parsee_core-0.1.4.8/parsee/datasets/evaluation/main.py` & `parsee_core-0.1.4.9/parsee/datasets/evaluation/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import os.path
 from typing import *
 
 from parsee.extraction.extractor_dataclasses import ParseeAnswer
 from parsee.datasets.readers.interfaces import DatasetReader
+from parsee.datasets.writers.interfaces import DatasetWriter
 from parsee.extraction.models.model_dataclasses import MlModelSpecification
 from parsee.templates.job_template import JobTemplate
 from parsee.extraction.models.model_loader import ModelLoader, LLMQuestionModel
 from parsee.storage.interfaces import StorageManager
 from parsee.storage.in_memory_storage import InMemoryStorageManager
 
 
@@ -97,34 +99,47 @@
             # scores EXCLUDING missing answers
             scores_dict_final["total_correct_percent_ex_missing"] = scores_dict_final["total_correct"] / (reference_scores["total_correct"]-scores_dict_final["missing_answers"])
             scores_dict_final["total_correct_meta_found_percent_ex_missing"] = scores_dict_final["total_correct_meta_found"] / (reference_scores["total_correct_meta_found"]-scores_dict_final["missing_answers"])
             total_scores[model] = scores_dict_final
         return total_scores
 
 
-def evaluate_llm_performance(template: JobTemplate, reader: DatasetReader, models: List[MlModelSpecification], storage: Optional[StorageManager] = None) -> Dict:
+def evaluate_llm_performance(template: JobTemplate, reader: DatasetReader, models: List[MlModelSpecification], storage: Optional[StorageManager] = None, writer_for_model_answers: Optional[DatasetWriter] = None, use_saved_model_answers: bool = False) -> Dict:
 
     storage = InMemoryStorageManager(models) if storage is None else storage
     loader = ModelLoader(storage)
     ev = EvaluationResult()
 
     for spec in models:
         if spec.model_type == "custom":
             raise Exception("custom models not allowed here")
 
+    new_rows = []
     for row, _ in reader.row_generator():
 
         for k, model_spec in enumerate(models):
             model: LLMQuestionModel = loader.get_question_model(model_spec.internal_name, template.questions.items, template.meta, {})
             if model is None:
                 raise Exception("model not found")
             schema_items = [x for x in template.questions.items if x.id == row.element_identifier]
             if len(schema_items) == 0:
                 raise Exception("item not found in schema")
             schema_item = schema_items[0]
-            answers_model = model.predict_for_prompt(row.get_feature("full_prompt"), schema_item, None, None)
+            if use_saved_model_answers and row.get_value(model_spec.internal_name, False) is not None:
+                prompt_answer = row.get_value(model_spec.internal_name, False)
+                answers_model = model.parse_prompt_answer(schema_item, prompt_answer, None, None)
+            else:
+                answers_model = model.predict_for_prompt(row.get_feature("full_prompt"), schema_item, None, None)
+                raw_answer = "\n\n".join([x.raw_value for x in answers_model])
+                row.assign_truth_values({model_spec.internal_name: raw_answer})
             ev.add_answers(row.source_identifier, answers_model, False)
             if k == 0:
-                answers_assigned = model.parse_prompt_answer(schema_item, row.get_value("answer", False), None, None)
+                answers_assigned = model.parse_prompt_answer(schema_item, row.get_value("assigned", False), None, None)
                 ev.add_answers(row.source_identifier, answers_assigned, True)
+        if writer_for_model_answers is not None:
+            new_rows.append(row)
+
+    if writer_for_model_answers is not None:
+        # write modified rows
+        writer_for_model_answers.write_rows(new_rows, "dataset_with_answers")
 
     return ev.evaluate()
```

### Comparing `parsee_core-0.1.4.8/parsee/datasets/main.py` & `parsee_core-0.1.4.9/parsee/datasets/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,17 +25,18 @@
     question_rows = []
     if len(question_models) > 0:
         question_model = question_models[0]
         answers = question_model.predict_answers(document)
         if len(answers) > 0:
             for item in question_model.items:
                 meta_items_filtered = [x for x in template.meta if x.id in item.metaInfoIds]
-                prompt = question_feature_builder.build_prompt(item, meta_items_filtered, document)
+                relevant_elements = question_feature_builder.get_relevant_elements(item, document)
+                prompt = question_feature_builder.build_prompt(item, meta_items_filtered, document, relevant_elements)
                 real_prompt, _ = truncate_prompt(str(prompt), encoding, max_tokens_prompt)
                 answers_filtered = [x for x in answers if x.class_id == item.id]
                 if len(answers_filtered) > 0:
                     # join together in case the answer has multiple blocks
                     full_answer = "\n\n".join([question_feature_builder.build_raw_value(answer.class_value, answer.meta, answer.sources, item, meta_items_filtered) for answer in answers_filtered])
                     row = DatasetRow(document.source_identifier, template.id, item.id, {"full_prompt": real_prompt})
-                    row.assign_truth_values({"answer": full_answer})
+                    row.assign_truth_values({"assigned": full_answer})
                     question_rows.append(row)
     return question_rows
```

### Comparing `parsee_core-0.1.4.8/parsee/datasets/readers/disk_reader.py` & `parsee_core-0.1.4.9/parsee/datasets/readers/disk_reader.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/datasets/readers/interfaces.py` & `parsee_core-0.1.4.9/parsee/datasets/readers/interfaces.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/datasets/writers/disk_writer.py` & `parsee_core-0.1.4.9/parsee/datasets/writers/disk_writer.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/datasets/writers/interfaces.py` & `parsee_core-0.1.4.9/parsee/datasets/writers/interfaces.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/extractor_dataclasses.py` & `parsee_core-0.1.4.9/parsee/extraction/extractor_dataclasses.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/extractor_elements.py` & `parsee_core-0.1.4.9/parsee/extraction/extractor_elements.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/final_structuring.py` & `parsee_core-0.1.4.9/parsee/extraction/final_structuring.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/models/helpers.py` & `parsee_core-0.1.4.9/parsee/extraction/models/helpers.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,8 +20,13 @@
 def anthropic_config(anthropic_api_key: str, model_name: str, token_limit: Optional[int] = None, multimodal: bool = False, max_images: int = 5, max_image_size: int = 2000) -> MlModelSpecification:
     token_limit = NUM_TOKENS_DEFAULT_LLM if token_limit is None else token_limit
     return MlModelSpecification(f"Anthropic model: {model_name}", model_name, ModelType.ANTHROPIC, None, None, token_limit, anthropic_api_key, None, None, None, None, None, multimodal, max_images, max_image_size)
 
 
 def ollama_config(model_name: str, custom_host: Optional[str] = None, token_limit: Optional[int] = None) -> MlModelSpecification:
     token_limit = NUM_TOKENS_DEFAULT_LLM if token_limit is None else token_limit
-    return MlModelSpecification(f"Ollama model: {model_name}", model_name, ModelType.OLLAMA, custom_host, Decimal(0), token_limit, None, None, None, None, None, None, False, None, None)
+    return MlModelSpecification(f"Ollama model: {model_name}", model_name, ModelType.OLLAMA, custom_host, Decimal(0), token_limit, None, None, None, None, None, None, False, None, None)
+
+
+def together_config(together_api_key: str, model_name: str, token_limit: Optional[int] = None) -> MlModelSpecification:
+    token_limit = NUM_TOKENS_DEFAULT_LLM if token_limit is None else token_limit
+    return MlModelSpecification(f"Together AI model: {model_name}", model_name, ModelType.TOGETHER, None, None, token_limit, together_api_key, None, None, None, None, None, False, None, None)
```

### Comparing `parsee_core-0.1.4.8/parsee/extraction/models/llm_models/anthropic_model.py` & `parsee_core-0.1.4.9/parsee/extraction/models/llm_models/anthropic_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/models/llm_models/chatgpt_model.py` & `parsee_core-0.1.4.9/parsee/extraction/models/llm_models/chatgpt_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/models/llm_models/llm_base_model.py` & `parsee_core-0.1.4.9/parsee/extraction/models/llm_models/llm_base_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/models/llm_models/ollama_model.py` & `parsee_core-0.1.4.9/parsee/extraction/models/llm_models/ollama_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/models/llm_models/prompts.py` & `parsee_core-0.1.4.9/parsee/extraction/models/llm_models/prompts.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/models/llm_models/replicate_model.py` & `parsee_core-0.1.4.9/parsee/extraction/models/llm_models/replicate_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/models/llm_models/structuring_schema.py` & `parsee_core-0.1.4.9/parsee/extraction/models/llm_models/structuring_schema.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/models/model_dataclasses.py` & `parsee_core-0.1.4.9/parsee/extraction/models/model_dataclasses.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/models/model_loader.py` & `parsee_core-0.1.4.9/parsee/extraction/models/model_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from parsee.templates.general_structuring_schema import StructuringItemSchema, GeneralQuerySchema, GeneralQueryItemSchema
 from parsee.extraction.tasks.element_classification.element_model import ElementModel, AssignedElementModel
 from parsee.extraction.tasks.questions.question_model import QuestionModel, AssignedQuestionModel
 from parsee.extraction.models.llm_models.chatgpt_model import ChatGPTModel
 from parsee.extraction.models.llm_models.replicate_model import ReplicateModel
 from parsee.extraction.models.llm_models.anthropic_model import AnthropicModel
 from parsee.extraction.models.llm_models.ollama_model import OllamaModel
+from parsee.extraction.models.llm_models.together_model import TogetherModel
 from parsee.extraction.tasks.questions.question_model_llm import LLMQuestionModel
 from parsee.extraction.tasks.meta_info_structuring.meta_info import MetaInfoModel
 from parsee.extraction.tasks.meta_info_structuring.meta_info_llm import MetaLLMModel
 from parsee.extraction.tasks.element_classification.element_model_llm import ElementModelLLM
 from parsee.extraction.tasks.mappings.mapping_model import MappingModel
 from parsee.extraction.tasks.mappings.mapping_model_llm import MappingModelLLM
 from parsee.storage.interfaces import StorageManager
@@ -25,14 +26,16 @@
         return ChatGPTModel(spec)
     elif spec.model_type == ModelType.REPLICATE:
         return ReplicateModel(spec)
     elif spec.model_type == ModelType.ANTHROPIC:
         return AnthropicModel(spec)
     elif spec.model_type == ModelType.OLLAMA:
         return OllamaModel(spec)
+    elif spec.model_type == ModelType.TOGETHER:
+        return TogetherModel(spec)
     else:
         raise Exception("llm base model not found")
 
 
 class ModelLoader:
 
     def __init__(self, storage: StorageManager):
```

### Comparing `parsee_core-0.1.4.8/parsee/extraction/run.py` & `parsee_core-0.1.4.9/parsee/extraction/run.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/tasks/element_classification/element_model.py` & `parsee_core-0.1.4.9/parsee/extraction/tasks/element_classification/element_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/tasks/element_classification/element_model_llm.py` & `parsee_core-0.1.4.9/parsee/extraction/tasks/element_classification/element_model_llm.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/tasks/element_classification/features.py` & `parsee_core-0.1.4.9/parsee/extraction/tasks/element_classification/features.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/tasks/mappings/features.py` & `parsee_core-0.1.4.9/parsee/extraction/tasks/mappings/features.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/tasks/mappings/mapping_model.py` & `parsee_core-0.1.4.9/parsee/extraction/tasks/mappings/mapping_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/tasks/mappings/mapping_model_llm.py` & `parsee_core-0.1.4.9/parsee/extraction/tasks/mappings/mapping_model_llm.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/tasks/mappings/utils.py` & `parsee_core-0.1.4.9/parsee/extraction/tasks/mappings/utils.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/tasks/meta_info_structuring/features.py` & `parsee_core-0.1.4.9/parsee/extraction/tasks/meta_info_structuring/features.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/tasks/meta_info_structuring/meta_info_llm.py` & `parsee_core-0.1.4.9/parsee/extraction/tasks/meta_info_structuring/meta_info_llm.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/tasks/questions/features.py` & `parsee_core-0.1.4.9/parsee/extraction/tasks/questions/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,15 @@
 
     def get_elements_text(self, elements: List[ExtractedEl], document: StandardDocumentFormat):
         llm_text = "This is the available data to answer the question (in the following, if tables have empty cells, they are omitted, if a cell spans several columns, values might be repeated for each cell):\n"
         for el in elements:
             llm_text += f"[{el.source.element_index}]: {el.get_text_and_surrounding_elements_text(document.elements) if isinstance(el, StructuredTable) else el.get_text_llm(True)}\n"
         return llm_text
 
-    def build_prompt(self, structuring_item: GeneralQueryItemSchema, meta_items: List[StructuringItemSchema], document: StandardDocumentFormat, relevant_elements_custom: Optional[List[ExtractedEl]] = None, multimodal: bool = False, max_images: Optional[int] = None, max_image_size: Optional[int] = None) -> Prompt:
-
-        elements = self.get_relevant_elements(structuring_item, document) if relevant_elements_custom is None else relevant_elements_custom
+    def build_prompt(self, structuring_item: GeneralQueryItemSchema, meta_items: List[StructuringItemSchema], document: StandardDocumentFormat, relevant_elements: List[ExtractedEl], multimodal: bool = False, max_images: Optional[int] = None, max_image_size: Optional[int] = None) -> Prompt:
 
         if not multimodal:
             general_info = "You are supposed to answer a question based on text fragments that are provided. " \
                            "The fragments start with a number and then the actual text. The lower the number of the fragment, " \
                            "the earlier the fragment appeared in the document (reading from left to right, top to bottom). " \
                            "Please respond as concise as possible."
         else:
@@ -80,9 +78,9 @@
             for meta_item in relevant_meta_items:
                 meta_prompt_item = get_prompt_schema_item(meta_item)
                 main_question += f"\n({meta_item.id}): {meta_item.title} {meta_item.additionalInfo} {meta_prompt_item.get_possible_values_str()}"
 
         prompt = Prompt(general_info, main_question,
                         'Please at the end of each answer also provide the numbers of the text fragments you used to answer in square brackets.' if not multimodal else "",
                         full_example,
-                        self.get_elements_text(elements, document) if not multimodal else self.storage.image_creator.get_images(document, elements, max_images, max_image_size))
+                        self.get_elements_text(relevant_elements, document) if not multimodal else self.storage.image_creator.get_images(document, relevant_elements, max_images, max_image_size))
         return prompt
```

### Comparing `parsee_core-0.1.4.8/parsee/extraction/tasks/questions/question_model.py` & `parsee_core-0.1.4.9/parsee/extraction/tasks/questions/question_model.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/extraction/tasks/questions/question_model_llm.py` & `parsee_core-0.1.4.9/parsee/extraction/tasks/questions/question_model_llm.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,11 +66,12 @@
         self.storage.log_expense(self.llm.spec.internal_name, amount, schema_item.id)
         return self.parse_prompt_answer(schema_item, prompt_answer, max_element_index, document)
 
     def predict_answers(self, document: StandardDocumentFormat) -> List[ParseeAnswer]:
 
         answers: List[ParseeAnswer] = []
         for schema_item in self.items:
-            prompt = self.prompt_builder.build_prompt(schema_item, self.meta, document, None, self.llm.spec.multimodal, self.llm.spec.max_images, self.llm.spec.max_image_pixels)
+            relevant_elements = self.prompt_builder.get_relevant_elements(schema_item, document)
+            prompt = self.prompt_builder.build_prompt(schema_item, self.meta, document, relevant_elements, self.llm.spec.multimodal, self.llm.spec.max_images, self.llm.spec.max_image_pixels)
             answers += self.predict_for_prompt(prompt, schema_item, len(document.elements), document)
 
         return answers
```

### Comparing `parsee_core-0.1.4.8/parsee/extraction/tasks/questions/utils.py` & `parsee_core-0.1.4.9/parsee/extraction/tasks/questions/utils.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/storage/in_memory_storage.py` & `parsee_core-0.1.4.9/parsee/storage/in_memory_storage.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/storage/interfaces.py` & `parsee_core-0.1.4.9/parsee/storage/interfaces.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/storage/vector_stores/simple_faiss.py` & `parsee_core-0.1.4.9/parsee/storage/vector_stores/simple_faiss.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/templates/element_schema.py` & `parsee_core-0.1.4.9/parsee/templates/element_schema.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/templates/general_structuring_schema.py` & `parsee_core-0.1.4.9/parsee/templates/general_structuring_schema.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/templates/helpers.py` & `parsee_core-0.1.4.9/parsee/templates/helpers.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/templates/job_template.py` & `parsee_core-0.1.4.9/parsee/templates/job_template.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/templates/mappings.py` & `parsee_core-0.1.4.9/parsee/templates/mappings.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/utils/enums.py` & `parsee_core-0.1.4.9/parsee/utils/enums.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,7 +45,8 @@
 
 class ModelType(Enum):
     GPT = "gpt"
     CUSTOM = "custom"
     REPLICATE = "replicate"
     ANTHROPIC = "anthropic"
     OLLAMA = "ollama"
+    TOGETHER = "together"
```

### Comparing `parsee_core-0.1.4.8/parsee/utils/helper.py` & `parsee_core-0.1.4.9/parsee/utils/helper.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/parsee/utils/sample_items.py` & `parsee_core-0.1.4.9/parsee/utils/sample_items.py`

 * *Files identical despite different names*

### Comparing `parsee_core-0.1.4.8/pyproject.toml` & `parsee_core-0.1.4.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 [tool.poetry]
 name = "parsee-core"
-version = "0.1.4.8"
+version = "0.1.4.9"
 description = ""
 authors = ["Parsee.ai <info@parsee.ai>"]
 homepage = "https://parsee.ai"
 packages = [{include = "parsee"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 requests = "^2.28.1"
 pandas = "^1.4.3"
 numpy = "^1.23.1"
 tiktoken = "^0.4.0"
 openai = "^0.27.8"
-pydantic = "^1.6.2"
+pydantic = "^2.7.0"
 faiss-cpu = [{version = "<1.7.1", platform = "darwin"}, {version = "^1.7.1", platform = "linux"}]
 replicate = "^0.23.1"
 beautifulsoup4 = "^4.11.1"
 parsee-pdf-reader = "^0.1.5.8"
 sentence-transformers = "^2.2.2"
 lxml = "^4.9.1"
 anthropic = "^0.20.0"
 ollama = "^0.1.7"
 opencv-python = "^4.9.0.80"
+together = "^1.1.1"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.extras.dependencies]
 langchain = "^0.1.11"
 
 [build-system]
```

### Comparing `parsee_core-0.1.4.8/PKG-INFO` & `parsee_core-0.1.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsee-core
-Version: 0.1.4.8
+Version: 0.1.4.9
 Summary: 
 Home-page: https://parsee.ai
 Author: Parsee.ai
 Author-email: info@parsee.ai
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -16,12 +16,13 @@
 Requires-Dist: lxml (>=4.9.1,<5.0.0)
 Requires-Dist: numpy (>=1.23.1,<2.0.0)
 Requires-Dist: ollama (>=0.1.7,<0.2.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: parsee-pdf-reader (>=0.1.5.8,<0.2.0.0)
-Requires-Dist: pydantic (>=1.6.2,<2.0.0)
+Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: replicate (>=0.23.1,<0.24.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
 Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
+Requires-Dist: together (>=1.1.1,<2.0.0)
```

