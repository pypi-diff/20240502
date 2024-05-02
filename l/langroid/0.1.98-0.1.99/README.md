# Comparing `tmp/langroid-0.1.98.tar.gz` & `tmp/langroid-0.1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langroid-0.1.98.tar", max compression
+gzip compressed data, was "langroid-0.1.99.tar", max compression
```

## Comparing `langroid-0.1.98.tar` & `langroid-0.1.99.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0     1065 2023-05-11 20:36:27.491909 langroid-0.1.98/LICENSE
--rw-r--r--   0        0        0    34655 2023-10-15 01:02:13.422544 langroid-0.1.98/README.md
--rw-r--r--   0        0        0       30 2023-07-16 18:07:11.916919 langroid-0.1.98/langroid/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 20:36:27.496878 langroid-0.1.98/langroid/agent/__init__.py
--rw-r--r--   0        0        0    29977 2023-10-18 00:44:12.144930 langroid-0.1.98/langroid/agent/base.py
--rw-r--r--   0        0        0     5358 2023-10-18 14:35:25.455897 langroid-0.1.98/langroid/agent/batch.py
--rw-r--r--   0        0        0    33358 2023-10-18 00:43:06.690528 langroid-0.1.98/langroid/agent/chat_agent.py
--rw-r--r--   0        0        0     6252 2023-09-16 15:25:46.865817 langroid-0.1.98/langroid/agent/chat_document.py
--rw-r--r--   0        0        0        0 2023-06-28 17:38:40.294031 langroid-0.1.98/langroid/agent/helpers.py
--rw-r--r--   0        0        0      339 2023-06-09 22:22:24.291666 langroid-0.1.98/langroid/agent/junk
--rw-r--r--   0        0        0        0 2023-06-28 22:15:49.364295 langroid-0.1.98/langroid/agent/special/__init__.py
--rw-r--r--   0        0        0    29521 2023-10-14 22:17:36.885008 langroid-0.1.98/langroid/agent/special/doc_chat_agent.py
--rw-r--r--   0        0        0     6035 2023-08-30 20:42:08.584707 langroid-0.1.98/langroid/agent/special/recipient_validator_agent.py
--rw-r--r--   0        0        0     3901 2023-10-16 16:20:29.105750 langroid-0.1.98/langroid/agent/special/relevance_extractor_agent.py
--rw-r--r--   0        0        0     6579 2023-10-10 23:20:35.944149 langroid-0.1.98/langroid/agent/special/retriever_agent.py
--rw-r--r--   0        0        0        0 2023-08-30 20:42:08.584750 langroid-0.1.98/langroid/agent/special/sql/__init__.py
--rw-r--r--   0        0        0    12867 2023-09-18 17:40:44.521953 langroid-0.1.98/langroid/agent/special/sql/sql_chat_agent.py
--rw-r--r--   0        0        0        0 2023-08-30 20:42:08.584826 langroid-0.1.98/langroid/agent/special/sql/utils/__init__.py
--rw-r--r--   0        0        0     4494 2023-09-01 14:39:38.564597 langroid-0.1.98/langroid/agent/special/sql/utils/description_extractors.py
--rw-r--r--   0        0        0     2712 2023-09-01 14:39:38.565007 langroid-0.1.98/langroid/agent/special/sql/utils/populate_metadata.py
--rw-r--r--   0        0        0     1885 2023-09-01 14:39:38.565566 langroid-0.1.98/langroid/agent/special/sql/utils/system_message.py
--rw-r--r--   0        0        0     1332 2023-09-01 14:39:38.565879 langroid-0.1.98/langroid/agent/special/sql/utils/tools.py
--rw-r--r--   0        0        0     7691 2023-09-29 16:59:58.812736 langroid-0.1.98/langroid/agent/special/table_chat_agent.py
--rw-r--r--   0        0        0    35391 2023-10-18 14:28:50.626037 langroid-0.1.98/langroid/agent/task.py
--rw-r--r--   0        0        0     6085 2023-09-29 17:44:34.310994 langroid-0.1.98/langroid/agent/tool_message.py
--rw-r--r--   0        0        0        0 2023-08-30 20:42:08.585633 langroid-0.1.98/langroid/agent/tools/__init__.py
--rw-r--r--   0        0        0     3789 2023-10-15 13:53:13.381604 langroid-0.1.98/langroid/agent/tools/extract_tool.py
--rw-r--r--   0        0        0      663 2023-09-24 22:29:05.401815 langroid-0.1.98/langroid/agent/tools/generator_tool.py
--rw-r--r--   0        0        0     1160 2023-08-30 20:42:08.585788 langroid-0.1.98/langroid/agent/tools/google_search_tool.py
--rw-r--r--   0        0        0    10217 2023-09-08 00:19:32.456348 langroid-0.1.98/langroid/agent/tools/recipient_tool.py
--rw-r--r--   0        0        0     1307 2023-10-16 01:11:08.304432 langroid-0.1.98/langroid/agent/tools/sentence_extract_tool.py
--rw-r--r--   0        0        0        0 2023-04-27 15:53:22.184840 langroid-0.1.98/langroid/agent_config.py
--rw-r--r--   0        0        0        0 2023-07-10 01:25:43.422507 langroid-0.1.98/langroid/cachedb/__init__.py
--rw-r--r--   0        0        0      790 2023-06-06 13:08:26.511045 langroid-0.1.98/langroid/cachedb/base.py
--rw-r--r--   0        0        0     2342 2023-09-07 21:20:53.512839 langroid-0.1.98/langroid/cachedb/momento_cachedb.py
--rw-r--r--   0        0        0     2369 2023-09-07 21:20:53.512506 langroid-0.1.98/langroid/cachedb/redis_cachedb.py
--rw-r--r--   0        0        0        0 2023-05-11 20:36:27.497415 langroid-0.1.98/langroid/embedding_models/__init__.py
--rw-r--r--   0        0        0     1179 2023-09-23 19:08:12.787472 langroid-0.1.98/langroid/embedding_models/base.py
--rw-r--r--   0        0        0     6684 2023-07-09 22:56:35.472443 langroid-0.1.98/langroid/embedding_models/clustering.py
--rw-r--r--   0        0        0     3295 2023-09-28 22:39:03.321466 langroid-0.1.98/langroid/embedding_models/models.py
--rw-r--r--   0        0        0        0 2023-05-11 20:36:27.497787 langroid-0.1.98/langroid/language_models/__init__.py
--rw-r--r--   0        0        0     3458 2023-09-01 19:21:46.555551 langroid-0.1.98/langroid/language_models/azure_openai.py
--rw-r--r--   0        0        0    17803 2023-10-17 18:41:24.408684 langroid-0.1.98/langroid/language_models/base.py
--rw-r--r--   0        0        0      269 2023-09-13 23:54:39.993414 langroid-0.1.98/langroid/language_models/config.py
--rw-r--r--   0        0        0    36949 2023-10-14 22:17:36.885976 langroid-0.1.98/langroid/language_models/openai_gpt.py
--rw-r--r--   0        0        0        0 2023-09-13 23:54:39.993870 langroid-0.1.98/langroid/language_models/prompt_formatter/__init__.py
--rw-r--r--   0        0        0     1247 2023-09-13 23:54:39.994174 langroid-0.1.98/langroid/language_models/prompt_formatter/base.py
--rw-r--r--   0        0        0     2899 2023-09-14 16:00:04.713532 langroid-0.1.98/langroid/language_models/prompt_formatter/llama2_formatter.py
--rw-r--r--   0        0        0     4668 2023-09-09 00:35:49.206618 langroid-0.1.98/langroid/language_models/utils.py
--rw-r--r--   0        0        0     2110 2023-09-19 11:29:03.185625 langroid-0.1.98/langroid/mytypes.py
--rw-r--r--   0        0        0        0 2023-07-09 14:18:20.695283 langroid-0.1.98/langroid/parsing/__init__.py
--rw-r--r--   0        0        0     1068 2023-06-19 02:13:48.643592 langroid-0.1.98/langroid/parsing/agent_chats.py
--rw-r--r--   0        0        0     3294 2023-05-01 22:42:52.628110 langroid-0.1.98/langroid/parsing/code-parsing.md
--rw-r--r--   0        0        0     3727 2023-09-08 00:19:32.457614 langroid-0.1.98/langroid/parsing/code_parser.py
--rw-r--r--   0        0        0        0 2023-09-21 01:16:16.841716 langroid-0.1.98/langroid/parsing/config.py
--rw-r--r--   0        0        0    14581 2023-10-04 16:47:10.818699 langroid-0.1.98/langroid/parsing/document_parser.py
--rw-r--r--   0        0        0     1650 2023-08-30 20:42:08.587194 langroid-0.1.98/langroid/parsing/json.py
--rw-r--r--   0        0        0     2000 2023-08-30 20:42:08.587449 langroid-0.1.98/langroid/parsing/para_sentence_split.py
--rw-r--r--   0        0        0     8070 2023-10-04 16:47:10.818751 langroid-0.1.98/langroid/parsing/parser.py
--rw-r--r--   0        0        0    27695 2023-10-06 19:59:47.715633 langroid-0.1.98/langroid/parsing/repo_loader.py
--rw-r--r--   0        0        0     8375 2023-10-04 16:47:10.818808 langroid-0.1.98/langroid/parsing/search.py
--rw-r--r--   0        0        0     3008 2023-10-09 01:26:36.188537 langroid-0.1.98/langroid/parsing/spider.py
--rw-r--r--   0        0        0     1767 2023-08-12 21:22:01.264293 langroid-0.1.98/langroid/parsing/table_loader.py
--rw-r--r--   0        0        0     2153 2023-10-08 18:43:05.662299 langroid-0.1.98/langroid/parsing/url_loader.py
--rw-r--r--   0        0        0     2327 2023-07-09 22:56:36.375054 langroid-0.1.98/langroid/parsing/url_loader_cookies.py
--rw-r--r--   0        0        0     7520 2023-10-09 17:07:52.830078 langroid-0.1.98/langroid/parsing/urls.py
--rw-r--r--   0        0        0     6162 2023-10-16 16:18:21.151418 langroid-0.1.98/langroid/parsing/utils.py
--rw-r--r--   0        0        0     2496 2023-08-12 21:22:01.264590 langroid-0.1.98/langroid/parsing/web_search.py
--rw-r--r--   0        0        0        0 2023-07-10 01:26:13.103739 langroid-0.1.98/langroid/prompts/__init__.py
--rw-r--r--   0        0        0      331 2023-06-06 13:08:26.513984 langroid-0.1.98/langroid/prompts/dialog.py
--rw-r--r--   0        0        0       98 2023-09-08 00:19:32.458744 langroid-0.1.98/langroid/prompts/prompts_config.py
--rw-r--r--   0        0        0     6369 2023-09-25 14:08:42.326287 langroid-0.1.98/langroid/prompts/templates.py
--rw-r--r--   0        0        0     2706 2023-07-22 20:54:23.661690 langroid-0.1.98/langroid/prompts/transforms.py
--rw-r--r--   0        0        0        0 2023-07-10 01:26:53.055820 langroid-0.1.98/langroid/scripts/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 20:36:27.499726 langroid-0.1.98/langroid/utils/__init__.py
--rw-r--r--   0        0        0     2258 2023-10-09 01:33:58.765524 langroid-0.1.98/langroid/utils/configuration.py
--rw-r--r--   0        0        0      484 2023-09-07 21:20:53.508915 langroid-0.1.98/langroid/utils/constants.py
--rw-r--r--   0        0        0     1105 2023-06-06 13:08:26.514914 langroid-0.1.98/langroid/utils/docker.py
--rw-r--r--   0        0        0     1337 2023-09-07 21:20:53.508581 langroid-0.1.98/langroid/utils/globals.py
--rw-r--r--   0        0        0        0 2023-05-11 20:36:27.500241 langroid-0.1.98/langroid/utils/llms/__init__.py
--rw-r--r--   0        0        0      263 2023-05-11 20:36:27.500371 langroid-0.1.98/langroid/utils/llms/strings.py
--rw-r--r--   0        0        0     3951 2023-07-28 17:28:03.882922 langroid-0.1.98/langroid/utils/logging.py
--rw-r--r--   0        0        0        0 2023-05-11 20:36:27.500552 langroid-0.1.98/langroid/utils/output/__init__.py
--rw-r--r--   0        0        0     1311 2023-07-09 22:56:35.554851 langroid-0.1.98/langroid/utils/output/printing.py
--rw-r--r--   0        0        0     6226 2023-10-15 01:02:13.422937 langroid-0.1.98/langroid/utils/pydantic_utils.py
--rw-r--r--   0        0        0     1518 2023-10-14 22:17:36.886516 langroid-0.1.98/langroid/utils/system.py
--rw-r--r--   0        0        0        0 2023-04-26 13:22:53.627926 langroid-0.1.98/langroid/utils/web/__init__.py
--rw-r--r--   0        0        0     2528 2023-04-30 02:01:56.075462 langroid-0.1.98/langroid/utils/web/login.py
--rw-r--r--   0        0        0     1156 2023-07-10 02:24:36.986647 langroid-0.1.98/langroid/utils/web/selenium_login.py
--rw-r--r--   0        0        0        0 2023-05-11 20:36:27.500862 langroid-0.1.98/langroid/vector_store/__init__.py
--rw-r--r--   0        0        0     5492 2023-10-15 01:02:13.423235 langroid-0.1.98/langroid/vector_store/base.py
--rw-r--r--   0        0        0     6744 2023-10-04 16:47:10.818999 langroid-0.1.98/langroid/vector_store/chromadb.py
--rw-r--r--   0        0        0    11262 2023-10-14 22:17:36.886834 langroid-0.1.98/langroid/vector_store/lancedb.py
--rw-r--r--   0        0        0    11168 2023-10-04 16:47:10.819043 langroid-0.1.98/langroid/vector_store/meilisearch.py
--rw-r--r--   0        0        0     9891 2023-10-15 01:02:13.423437 langroid-0.1.98/langroid/vector_store/momento.py
--rw-r--r--   0        0        0      188 2023-05-25 14:59:22.453121 langroid-0.1.98/langroid/vector_store/qdrant_cloud.py
--rw-r--r--   0        0        0    10865 2023-10-04 16:47:10.819091 langroid-0.1.98/langroid/vector_store/qdrantdb.py
--rw-r--r--   0        0        0     3804 2023-10-18 14:45:02.401219 langroid-0.1.98/pyproject.toml
--rw-r--r--   0        0        0    38664 1970-01-01 00:00:00.000000 langroid-0.1.98/setup.py
--rw-r--r--   0        0        0    38372 1970-01-01 00:00:00.000000 langroid-0.1.98/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-11 20:36:27.491909 langroid-0.1.99/LICENSE
+-rw-r--r--   0        0        0    34655 2023-10-15 01:02:13.422544 langroid-0.1.99/README.md
+-rw-r--r--   0        0        0       30 2023-07-16 18:07:11.916919 langroid-0.1.99/langroid/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 20:36:27.496878 langroid-0.1.99/langroid/agent/__init__.py
+-rw-r--r--   0        0        0    29977 2023-10-18 00:44:12.144930 langroid-0.1.99/langroid/agent/base.py
+-rw-r--r--   0        0        0     5329 2023-10-18 15:16:44.856567 langroid-0.1.99/langroid/agent/batch.py
+-rw-r--r--   0        0        0    33358 2023-10-18 00:43:06.690528 langroid-0.1.99/langroid/agent/chat_agent.py
+-rw-r--r--   0        0        0     6252 2023-09-16 15:25:46.865817 langroid-0.1.99/langroid/agent/chat_document.py
+-rw-r--r--   0        0        0        0 2023-06-28 17:38:40.294031 langroid-0.1.99/langroid/agent/helpers.py
+-rw-r--r--   0        0        0      339 2023-06-09 22:22:24.291666 langroid-0.1.99/langroid/agent/junk
+-rw-r--r--   0        0        0        0 2023-06-28 22:15:49.364295 langroid-0.1.99/langroid/agent/special/__init__.py
+-rw-r--r--   0        0        0    29521 2023-10-14 22:17:36.885008 langroid-0.1.99/langroid/agent/special/doc_chat_agent.py
+-rw-r--r--   0        0        0     6035 2023-08-30 20:42:08.584707 langroid-0.1.99/langroid/agent/special/recipient_validator_agent.py
+-rw-r--r--   0        0        0     3901 2023-10-16 16:20:29.105750 langroid-0.1.99/langroid/agent/special/relevance_extractor_agent.py
+-rw-r--r--   0        0        0     6579 2023-10-10 23:20:35.944149 langroid-0.1.99/langroid/agent/special/retriever_agent.py
+-rw-r--r--   0        0        0        0 2023-08-30 20:42:08.584750 langroid-0.1.99/langroid/agent/special/sql/__init__.py
+-rw-r--r--   0        0        0    12867 2023-09-18 17:40:44.521953 langroid-0.1.99/langroid/agent/special/sql/sql_chat_agent.py
+-rw-r--r--   0        0        0        0 2023-08-30 20:42:08.584826 langroid-0.1.99/langroid/agent/special/sql/utils/__init__.py
+-rw-r--r--   0        0        0     4494 2023-09-01 14:39:38.564597 langroid-0.1.99/langroid/agent/special/sql/utils/description_extractors.py
+-rw-r--r--   0        0        0     2712 2023-09-01 14:39:38.565007 langroid-0.1.99/langroid/agent/special/sql/utils/populate_metadata.py
+-rw-r--r--   0        0        0     1885 2023-09-01 14:39:38.565566 langroid-0.1.99/langroid/agent/special/sql/utils/system_message.py
+-rw-r--r--   0        0        0     1332 2023-09-01 14:39:38.565879 langroid-0.1.99/langroid/agent/special/sql/utils/tools.py
+-rw-r--r--   0        0        0     7691 2023-09-29 16:59:58.812736 langroid-0.1.99/langroid/agent/special/table_chat_agent.py
+-rw-r--r--   0        0        0    35396 2023-10-18 15:18:14.094779 langroid-0.1.99/langroid/agent/task.py
+-rw-r--r--   0        0        0     6085 2023-09-29 17:44:34.310994 langroid-0.1.99/langroid/agent/tool_message.py
+-rw-r--r--   0        0        0        0 2023-08-30 20:42:08.585633 langroid-0.1.99/langroid/agent/tools/__init__.py
+-rw-r--r--   0        0        0     3789 2023-10-15 13:53:13.381604 langroid-0.1.99/langroid/agent/tools/extract_tool.py
+-rw-r--r--   0        0        0      663 2023-09-24 22:29:05.401815 langroid-0.1.99/langroid/agent/tools/generator_tool.py
+-rw-r--r--   0        0        0     1160 2023-08-30 20:42:08.585788 langroid-0.1.99/langroid/agent/tools/google_search_tool.py
+-rw-r--r--   0        0        0    10217 2023-09-08 00:19:32.456348 langroid-0.1.99/langroid/agent/tools/recipient_tool.py
+-rw-r--r--   0        0        0     1307 2023-10-16 01:11:08.304432 langroid-0.1.99/langroid/agent/tools/sentence_extract_tool.py
+-rw-r--r--   0        0        0        0 2023-04-27 15:53:22.184840 langroid-0.1.99/langroid/agent_config.py
+-rw-r--r--   0        0        0        0 2023-07-10 01:25:43.422507 langroid-0.1.99/langroid/cachedb/__init__.py
+-rw-r--r--   0        0        0      790 2023-06-06 13:08:26.511045 langroid-0.1.99/langroid/cachedb/base.py
+-rw-r--r--   0        0        0     2342 2023-09-07 21:20:53.512839 langroid-0.1.99/langroid/cachedb/momento_cachedb.py
+-rw-r--r--   0        0        0     2369 2023-09-07 21:20:53.512506 langroid-0.1.99/langroid/cachedb/redis_cachedb.py
+-rw-r--r--   0        0        0        0 2023-05-11 20:36:27.497415 langroid-0.1.99/langroid/embedding_models/__init__.py
+-rw-r--r--   0        0        0     1179 2023-09-23 19:08:12.787472 langroid-0.1.99/langroid/embedding_models/base.py
+-rw-r--r--   0        0        0     6684 2023-07-09 22:56:35.472443 langroid-0.1.99/langroid/embedding_models/clustering.py
+-rw-r--r--   0        0        0     3295 2023-09-28 22:39:03.321466 langroid-0.1.99/langroid/embedding_models/models.py
+-rw-r--r--   0        0        0        0 2023-05-11 20:36:27.497787 langroid-0.1.99/langroid/language_models/__init__.py
+-rw-r--r--   0        0        0     3458 2023-09-01 19:21:46.555551 langroid-0.1.99/langroid/language_models/azure_openai.py
+-rw-r--r--   0        0        0    17803 2023-10-17 18:41:24.408684 langroid-0.1.99/langroid/language_models/base.py
+-rw-r--r--   0        0        0      269 2023-09-13 23:54:39.993414 langroid-0.1.99/langroid/language_models/config.py
+-rw-r--r--   0        0        0    36949 2023-10-14 22:17:36.885976 langroid-0.1.99/langroid/language_models/openai_gpt.py
+-rw-r--r--   0        0        0        0 2023-09-13 23:54:39.993870 langroid-0.1.99/langroid/language_models/prompt_formatter/__init__.py
+-rw-r--r--   0        0        0     1247 2023-09-13 23:54:39.994174 langroid-0.1.99/langroid/language_models/prompt_formatter/base.py
+-rw-r--r--   0        0        0     2899 2023-09-14 16:00:04.713532 langroid-0.1.99/langroid/language_models/prompt_formatter/llama2_formatter.py
+-rw-r--r--   0        0        0     4668 2023-09-09 00:35:49.206618 langroid-0.1.99/langroid/language_models/utils.py
+-rw-r--r--   0        0        0     2110 2023-09-19 11:29:03.185625 langroid-0.1.99/langroid/mytypes.py
+-rw-r--r--   0        0        0        0 2023-07-09 14:18:20.695283 langroid-0.1.99/langroid/parsing/__init__.py
+-rw-r--r--   0        0        0     1068 2023-06-19 02:13:48.643592 langroid-0.1.99/langroid/parsing/agent_chats.py
+-rw-r--r--   0        0        0     3294 2023-05-01 22:42:52.628110 langroid-0.1.99/langroid/parsing/code-parsing.md
+-rw-r--r--   0        0        0     3727 2023-09-08 00:19:32.457614 langroid-0.1.99/langroid/parsing/code_parser.py
+-rw-r--r--   0        0        0        0 2023-09-21 01:16:16.841716 langroid-0.1.99/langroid/parsing/config.py
+-rw-r--r--   0        0        0    14581 2023-10-04 16:47:10.818699 langroid-0.1.99/langroid/parsing/document_parser.py
+-rw-r--r--   0        0        0     1650 2023-08-30 20:42:08.587194 langroid-0.1.99/langroid/parsing/json.py
+-rw-r--r--   0        0        0     2000 2023-08-30 20:42:08.587449 langroid-0.1.99/langroid/parsing/para_sentence_split.py
+-rw-r--r--   0        0        0     8070 2023-10-04 16:47:10.818751 langroid-0.1.99/langroid/parsing/parser.py
+-rw-r--r--   0        0        0    27695 2023-10-06 19:59:47.715633 langroid-0.1.99/langroid/parsing/repo_loader.py
+-rw-r--r--   0        0        0     8375 2023-10-04 16:47:10.818808 langroid-0.1.99/langroid/parsing/search.py
+-rw-r--r--   0        0        0     3008 2023-10-09 01:26:36.188537 langroid-0.1.99/langroid/parsing/spider.py
+-rw-r--r--   0        0        0     1767 2023-08-12 21:22:01.264293 langroid-0.1.99/langroid/parsing/table_loader.py
+-rw-r--r--   0        0        0     2153 2023-10-08 18:43:05.662299 langroid-0.1.99/langroid/parsing/url_loader.py
+-rw-r--r--   0        0        0     2327 2023-07-09 22:56:36.375054 langroid-0.1.99/langroid/parsing/url_loader_cookies.py
+-rw-r--r--   0        0        0     7520 2023-10-09 17:07:52.830078 langroid-0.1.99/langroid/parsing/urls.py
+-rw-r--r--   0        0        0     6162 2023-10-16 16:18:21.151418 langroid-0.1.99/langroid/parsing/utils.py
+-rw-r--r--   0        0        0     2496 2023-08-12 21:22:01.264590 langroid-0.1.99/langroid/parsing/web_search.py
+-rw-r--r--   0        0        0        0 2023-07-10 01:26:13.103739 langroid-0.1.99/langroid/prompts/__init__.py
+-rw-r--r--   0        0        0      331 2023-06-06 13:08:26.513984 langroid-0.1.99/langroid/prompts/dialog.py
+-rw-r--r--   0        0        0       98 2023-09-08 00:19:32.458744 langroid-0.1.99/langroid/prompts/prompts_config.py
+-rw-r--r--   0        0        0     6369 2023-09-25 14:08:42.326287 langroid-0.1.99/langroid/prompts/templates.py
+-rw-r--r--   0        0        0     2706 2023-07-22 20:54:23.661690 langroid-0.1.99/langroid/prompts/transforms.py
+-rw-r--r--   0        0        0        0 2023-07-10 01:26:53.055820 langroid-0.1.99/langroid/scripts/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 20:36:27.499726 langroid-0.1.99/langroid/utils/__init__.py
+-rw-r--r--   0        0        0     2258 2023-10-09 01:33:58.765524 langroid-0.1.99/langroid/utils/configuration.py
+-rw-r--r--   0        0        0      484 2023-09-07 21:20:53.508915 langroid-0.1.99/langroid/utils/constants.py
+-rw-r--r--   0        0        0     1105 2023-06-06 13:08:26.514914 langroid-0.1.99/langroid/utils/docker.py
+-rw-r--r--   0        0        0     1337 2023-09-07 21:20:53.508581 langroid-0.1.99/langroid/utils/globals.py
+-rw-r--r--   0        0        0        0 2023-05-11 20:36:27.500241 langroid-0.1.99/langroid/utils/llms/__init__.py
+-rw-r--r--   0        0        0      263 2023-05-11 20:36:27.500371 langroid-0.1.99/langroid/utils/llms/strings.py
+-rw-r--r--   0        0        0     3951 2023-07-28 17:28:03.882922 langroid-0.1.99/langroid/utils/logging.py
+-rw-r--r--   0        0        0        0 2023-05-11 20:36:27.500552 langroid-0.1.99/langroid/utils/output/__init__.py
+-rw-r--r--   0        0        0     1311 2023-07-09 22:56:35.554851 langroid-0.1.99/langroid/utils/output/printing.py
+-rw-r--r--   0        0        0     6226 2023-10-15 01:02:13.422937 langroid-0.1.99/langroid/utils/pydantic_utils.py
+-rw-r--r--   0        0        0     1518 2023-10-14 22:17:36.886516 langroid-0.1.99/langroid/utils/system.py
+-rw-r--r--   0        0        0        0 2023-04-26 13:22:53.627926 langroid-0.1.99/langroid/utils/web/__init__.py
+-rw-r--r--   0        0        0     2528 2023-04-30 02:01:56.075462 langroid-0.1.99/langroid/utils/web/login.py
+-rw-r--r--   0        0        0     1156 2023-07-10 02:24:36.986647 langroid-0.1.99/langroid/utils/web/selenium_login.py
+-rw-r--r--   0        0        0        0 2023-05-11 20:36:27.500862 langroid-0.1.99/langroid/vector_store/__init__.py
+-rw-r--r--   0        0        0     5492 2023-10-15 01:02:13.423235 langroid-0.1.99/langroid/vector_store/base.py
+-rw-r--r--   0        0        0     6744 2023-10-04 16:47:10.818999 langroid-0.1.99/langroid/vector_store/chromadb.py
+-rw-r--r--   0        0        0    11262 2023-10-14 22:17:36.886834 langroid-0.1.99/langroid/vector_store/lancedb.py
+-rw-r--r--   0        0        0    11168 2023-10-04 16:47:10.819043 langroid-0.1.99/langroid/vector_store/meilisearch.py
+-rw-r--r--   0        0        0     9891 2023-10-15 01:02:13.423437 langroid-0.1.99/langroid/vector_store/momento.py
+-rw-r--r--   0        0        0      188 2023-05-25 14:59:22.453121 langroid-0.1.99/langroid/vector_store/qdrant_cloud.py
+-rw-r--r--   0        0        0    10865 2023-10-04 16:47:10.819091 langroid-0.1.99/langroid/vector_store/qdrantdb.py
+-rw-r--r--   0        0        0     3804 2023-10-18 15:18:40.938652 langroid-0.1.99/pyproject.toml
+-rw-r--r--   0        0        0    38664 1970-01-01 00:00:00.000000 langroid-0.1.99/setup.py
+-rw-r--r--   0        0        0    38372 1970-01-01 00:00:00.000000 langroid-0.1.99/PKG-INFO
```

### Comparing `langroid-0.1.98/LICENSE` & `langroid-0.1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/README.md` & `langroid-0.1.99/README.md`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/agent/base.py` & `langroid-0.1.99/langroid/agent/base.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/agent/batch.py` & `langroid-0.1.99/langroid/agent/batch.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,17 +40,18 @@
         List[Any]: list of final results
     """
 
     inputs = [input_map(item) for item in items]
 
     async def _do_task(input: str | ChatDocument, i: int) -> Any:
         task_i = task.clone(i)
-        assert task_i.agent.config.llm is not None, "task agent must have llm config"
-        task_i.agent.config.show_stats = False
-        task_i.agent.config.llm.stream = False
+        if task_i.agent.config.llm is not None:
+            task_i.agent.config.llm.stream = False
+            task_i.agent.config.show_stats = False
+
         result = await task_i.run_async(input)
         return output_map(result)
 
     async def _do_all() -> List[Any]:
         return await asyncio.gather(  # type: ignore
             *(_do_task(input, i) for i, input in enumerate(inputs))
         )
```

### Comparing `langroid-0.1.98/langroid/agent/chat_agent.py` & `langroid-0.1.99/langroid/agent/chat_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/agent/chat_document.py` & `langroid-0.1.99/langroid/agent/chat_document.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/agent/special/doc_chat_agent.py` & `langroid-0.1.99/langroid/agent/special/doc_chat_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/agent/special/recipient_validator_agent.py` & `langroid-0.1.99/langroid/agent/special/recipient_validator_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/agent/special/relevance_extractor_agent.py` & `langroid-0.1.99/langroid/agent/special/relevance_extractor_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/agent/special/retriever_agent.py` & `langroid-0.1.99/langroid/agent/special/retriever_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/agent/special/sql/sql_chat_agent.py` & `langroid-0.1.99/langroid/agent/special/sql/sql_chat_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/agent/special/sql/utils/description_extractors.py` & `langroid-0.1.99/langroid/agent/special/sql/utils/description_extractors.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/agent/special/sql/utils/populate_metadata.py` & `langroid-0.1.99/langroid/agent/special/sql/utils/populate_metadata.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/agent/special/sql/utils/system_message.py` & `langroid-0.1.99/langroid/agent/special/sql/utils/system_message.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/agent/special/sql/utils/tools.py` & `langroid-0.1.99/langroid/agent/special/sql/utils/tools.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/agent/special/table_chat_agent.py` & `langroid-0.1.99/langroid/agent/special/table_chat_agent.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/agent/task.py` & `langroid-0.1.99/langroid/agent/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,16 @@
         self.parent_task: Set[Task] = set()
         self.caller: Task | None = None  # which task called this task's `run` method
 
     def clone(self, i: int) -> "Task":
         """
         Returns a copy of this task, with a new agent.
         """
-        assert type(self.agent) is ChatAgent, "Task clone only works for ChatAgent"
+        assert isinstance(self.agent, ChatAgent), "Task clone only works for ChatAgent"
+
         agent_cls = type(self.agent)
         config_copy = copy.deepcopy(self.agent.config)
         agent: ChatAgent = agent_cls(config_copy)
         return Task(
             agent,
             name=self.name + f"-{i}",
             llm_delegate=self.llm_delegate,
```

### Comparing `langroid-0.1.98/langroid/agent/tool_message.py` & `langroid-0.1.99/langroid/agent/tool_message.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/agent/tools/extract_tool.py` & `langroid-0.1.99/langroid/agent/tools/extract_tool.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/agent/tools/generator_tool.py` & `langroid-0.1.99/langroid/agent/tools/generator_tool.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/agent/tools/google_search_tool.py` & `langroid-0.1.99/langroid/agent/tools/google_search_tool.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/agent/tools/recipient_tool.py` & `langroid-0.1.99/langroid/agent/tools/recipient_tool.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/agent/tools/sentence_extract_tool.py` & `langroid-0.1.99/langroid/agent/tools/sentence_extract_tool.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/cachedb/base.py` & `langroid-0.1.99/langroid/cachedb/base.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/cachedb/momento_cachedb.py` & `langroid-0.1.99/langroid/cachedb/momento_cachedb.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/cachedb/redis_cachedb.py` & `langroid-0.1.99/langroid/cachedb/redis_cachedb.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/embedding_models/base.py` & `langroid-0.1.99/langroid/embedding_models/base.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/embedding_models/clustering.py` & `langroid-0.1.99/langroid/embedding_models/clustering.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/embedding_models/models.py` & `langroid-0.1.99/langroid/embedding_models/models.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/language_models/azure_openai.py` & `langroid-0.1.99/langroid/language_models/azure_openai.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/language_models/base.py` & `langroid-0.1.99/langroid/language_models/base.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/language_models/openai_gpt.py` & `langroid-0.1.99/langroid/language_models/openai_gpt.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/language_models/prompt_formatter/base.py` & `langroid-0.1.99/langroid/language_models/prompt_formatter/base.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/language_models/prompt_formatter/llama2_formatter.py` & `langroid-0.1.99/langroid/language_models/prompt_formatter/llama2_formatter.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/language_models/utils.py` & `langroid-0.1.99/langroid/language_models/utils.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/mytypes.py` & `langroid-0.1.99/langroid/mytypes.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/parsing/agent_chats.py` & `langroid-0.1.99/langroid/parsing/agent_chats.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/parsing/code-parsing.md` & `langroid-0.1.99/langroid/parsing/code-parsing.md`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/parsing/code_parser.py` & `langroid-0.1.99/langroid/parsing/code_parser.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/parsing/document_parser.py` & `langroid-0.1.99/langroid/parsing/document_parser.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/parsing/json.py` & `langroid-0.1.99/langroid/parsing/json.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/parsing/para_sentence_split.py` & `langroid-0.1.99/langroid/parsing/para_sentence_split.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/parsing/parser.py` & `langroid-0.1.99/langroid/parsing/parser.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/parsing/repo_loader.py` & `langroid-0.1.99/langroid/parsing/repo_loader.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/parsing/search.py` & `langroid-0.1.99/langroid/parsing/search.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/parsing/spider.py` & `langroid-0.1.99/langroid/parsing/spider.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/parsing/table_loader.py` & `langroid-0.1.99/langroid/parsing/table_loader.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/parsing/url_loader.py` & `langroid-0.1.99/langroid/parsing/url_loader.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/parsing/url_loader_cookies.py` & `langroid-0.1.99/langroid/parsing/url_loader_cookies.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/parsing/urls.py` & `langroid-0.1.99/langroid/parsing/urls.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/parsing/utils.py` & `langroid-0.1.99/langroid/parsing/utils.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/parsing/web_search.py` & `langroid-0.1.99/langroid/parsing/web_search.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/prompts/templates.py` & `langroid-0.1.99/langroid/prompts/templates.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/prompts/transforms.py` & `langroid-0.1.99/langroid/prompts/transforms.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/utils/configuration.py` & `langroid-0.1.99/langroid/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/utils/docker.py` & `langroid-0.1.99/langroid/utils/docker.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/utils/globals.py` & `langroid-0.1.99/langroid/utils/globals.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/utils/logging.py` & `langroid-0.1.99/langroid/utils/logging.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/utils/output/printing.py` & `langroid-0.1.99/langroid/utils/output/printing.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/utils/pydantic_utils.py` & `langroid-0.1.99/langroid/utils/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/utils/system.py` & `langroid-0.1.99/langroid/utils/system.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/utils/web/login.py` & `langroid-0.1.99/langroid/utils/web/login.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/utils/web/selenium_login.py` & `langroid-0.1.99/langroid/utils/web/selenium_login.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/vector_store/base.py` & `langroid-0.1.99/langroid/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/vector_store/chromadb.py` & `langroid-0.1.99/langroid/vector_store/chromadb.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/vector_store/lancedb.py` & `langroid-0.1.99/langroid/vector_store/lancedb.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/vector_store/meilisearch.py` & `langroid-0.1.99/langroid/vector_store/meilisearch.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/vector_store/momento.py` & `langroid-0.1.99/langroid/vector_store/momento.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/langroid/vector_store/qdrantdb.py` & `langroid-0.1.99/langroid/vector_store/qdrantdb.py`

 * *Files identical despite different names*

### Comparing `langroid-0.1.98/pyproject.toml` & `langroid-0.1.99/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langroid"
-version = "0.1.98"
+version = "0.1.99"
 description = "Harness LLMs with Multi-Agent Programming"
 authors = ["Prasad Chalasani <pchalasani@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9.1,<3.12"
```

### Comparing `langroid-0.1.98/setup.py` & `langroid-0.1.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 extras_require = \
 {'hf-embeddings': ['sentence-transformers==2.2.2', 'torch==2.0.0'],
  'mysql': ['pymysql>=1.1.0,<2.0.0', 'pytest-mysql>=2.4.2,<3.0.0'],
  'postgres': ['psycopg2>=2.9.7,<3.0.0', 'pytest-postgresql>=5.0.0,<6.0.0']}
 
 setup_kwargs = {
     'name': 'langroid',
-    'version': '0.1.98',
+    'version': '0.1.99',
     'description': 'Harness LLMs with Multi-Agent Programming',
     'long_description': '<div align="center">\n  <img src="docs/assets/langroid-card-lambda-ossem-rust-1200-630.png" alt="Logo" \n        width="400" align="center">\n</div>\n\n<div align="center">\n\n[![PyPI - Version](https://img.shields.io/pypi/v/langroid)](https://pypi.org/project/langroid/)\n[![Pytest](https://github.com/langroid/langroid/actions/workflows/pytest.yml/badge.svg)](https://github.com/langroid/langroid/actions/workflows/pytest.yml)\n[![codecov](https://codecov.io/gh/langroid/langroid/branch/main/graph/badge.svg?token=H94BX5F0TE)](https://codecov.io/gh/langroid/langroid)\n[![Lint](https://github.com/langroid/langroid/actions/workflows/validate.yml/badge.svg)](https://github.com/langroid/langroid/actions/workflows/validate.yml)\n[![Docs](https://github.com/langroid/langroid/actions/workflows/mkdocs-deploy.yml/badge.svg)](https://github.com/langroid/langroid/actions/workflows/mkdocs-deploy.yml)\n\n[![Static Badge](https://img.shields.io/badge/Documentation-blue?link=https%3A%2F%2Flangroid.github.io%2Flangroid%2F&link=https%3A%2F%2Flangroid.github.io%2Flangroid%2F)](https://langroid.github.io/langroid)\n[![Discord](https://img.shields.io/badge/Discord-%235865F2.svg?style=for-the-badge&logo=discord&logoColor=white)](https://discord.gg/ZU36McDgDs)\n[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/langroid/langroid/blob/main/examples/langroid_quick_examples.ipynb)\n\n[![Docker Pulls](https://img.shields.io/docker/pulls/langroid/langroid.svg)](https://hub.docker.com/r/langroid/langroid)\n![Docker Image Size (tag)](https://img.shields.io/docker/image-size/langroid/langroid/latest)\n[![Multi-Architecture DockerHub](https://github.com/langroid/langroid/actions/workflows/docker-publish.yml/badge.svg)](https://github.com/langroid/langroid/actions/workflows/docker-publish.yml)\n\n[![Substack](https://img.shields.io/badge/Substack-%23006f5c.svg?style=for-the-badge&logo=substack&logoColor=FF6719)](https://langroid.substack.com/p/langroid-harness-llms-with-multi-agent-programming)\n\n[![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Flangroid%2Flangroid&t=Harness%20LLMs%20with%20Multi-Agent%20Programming)\n[![Share on Reddit](https://img.shields.io/badge/Reddit-FF4500?style=for-the-badge&logo=reddit&logoColor=white)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Flangroid%2Flangroid&title=Harness%20LLMs%20with%20Multi-Agent%20Programming)\n[![Share on Twitter](https://img.shields.io/twitter/url?style=social&url=https://github.com/langroid/langroid)](https://twitter.com/intent/tweet?text=Langroid%20is%20a%20powerful,%20elegant%20new%20framework%20to%20easily%20build%20%23LLM%20applications.%20You%20set%20up%20LLM-powered%20Agents%20with%20vector-stores,%20assign%20tasks,%20and%20have%20them%20collaboratively%20solve%20problems%20via%20message-transformations.%20https://github.com/langroid/langroid)\n[![LinkedIn](https://img.shields.io/badge/linkedin-%230077B5.svg?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/shareArticle?mini=true&url=https://github.com/langroid/langroid&title=Langroid:%20A%20Powerful,%20Elegant%20Framework&summary=Langroid%20is%20a%20powerful,%20elegant%20new%20framework%20to%20easily%20build%20%23LLM%20applications.%20You%20set%20up%20LLM-powered%20Agents%20with%20vector-stores,%20assign%20tasks,%20and%20have%20them%20collaboratively%20solve%20problems%20via%20message-transformations.)\n\n\n</div>\n\n<h3 align="center">\n  <a target="_blank" \n    href="https://langroid.github.io/langroid/" rel="dofollow">\n      <strong>Documentation</strong></a>\n  &middot;\n  <a target="_blank" href="https://github.com/langroid/langroid-examples" rel="dofollow">\n      <strong>Examples Repo</strong></a>\n  &middot;\n  <a target="_blank" href="https://discord.gg/ZU36McDgDs" rel="dofollow">\n      <strong>Discord</strong></a>\n  &middot;\n  <a target="_blank" href="./CONTRIBUTING.md" rel="dofollow">\n      <strong>Contributing</strong></a>\n\n  <br />\n</h3>\n\n`Langroid` is an intuitive, lightweight, extensible and principled\nPython framework to easily build LLM-powered applications. \nYou set up Agents, equip them with optional components (LLM, \nvector-store and methods), assign them tasks, and have them \ncollaboratively solve a problem by exchanging messages. \nThis Multi-Agent paradigm is inspired by the\n[Actor Framework](https://en.wikipedia.org/wiki/Actor_model)\n(but you do not need to know anything about this!). \n\n`Langroid` is a fresh take on LLM app-development, where considerable thought has gone \ninto simplifying the developer experience; it does not use `Langchain`.\n\nWe welcome contributions -- See the [contributions](./CONTRIBUTING.md) document\nfor ideas on what to contribute.\n\n**Questions, Feedback, Ideas? Join us on [Discord](https://discord.gg/ZU36McDgDs)!**\n\n<details>\n<summary> <b>:fire: Updates/Releases</b></summary>\n\n- **Oct 2023:**\n  - **0.1.95:** Added support for [Momento Serverless Vector Index](https://docs.momentohq.com/vector-index)\n  - **0.1.94:** Added support for [LanceDB](https://lancedb.github.io/lancedb/) vector-store -- allows vector, Full-text, SQL search.\n  - **0.1.84:** Added [LiteLLM](https://docs.litellm.ai/docs/providers), so now Langroid can be used with over 100 LLM providers (remote or local)! \n     See guide [here](https://langroid.github.io/langroid/tutorials/non-openai-llms/).\n- **Sep 2023:**\n  - **0.1.78:** Async versions of several Task, Agent and LLM methods; \n      Nested Pydantic classes are now supported for LLM Function-calling, Tools, Structured Output.    \n  - **0.1.76:** DocChatAgent: support for loading `docx` files (preliminary).\n  - **0.1.72:** Many improvements to DocChatAgent: better embedding model, \n          hybrid search to improve retrieval, better pdf parsing, re-ranking retrieved results with cross-encoders. \n  - **Use with local LLama Models:** see tutorial [here](https://langroid.github.io/langroid/blog/2023/09/14/using-langroid-with-local-llms/)\n  - **Langroid Blog/Newsletter Launched!**: First post is [here](https://substack.com/notes/post/p-136704592) -- Please subscribe to stay updated. \n  - **0.1.56:** Support Azure OpenAI. \n  - **0.1.55:** Improved [`SQLChatAgent`](https://github.com/langroid/langroid/blob/main/langroid/agent/special/sql/sql_chat_agent.py) that efficiently retrieves relevant schema info when translating natural language to SQL.  \n- **Aug 2023:**\n  - **[Hierarchical computation](https://langroid.github.io/langroid/examples/agent-tree/)** example using Langroid agents and task orchestration.\n  - **0.1.51:** Support for global state, see [test_global_state.py](tests/main/test_global_state.py).\n  - **:whale: Langroid Docker image**, available, see instructions below.\n  - [**RecipientTool**](langroid/agent/tools/recipient_tool.py) enables (+ enforces) LLM to \nspecify an intended recipient when talking to 2 or more agents. \nSee [this test](tests/main/test_recipient_tool.py) for example usage.\n  - **Example:** [Answer questions](examples/docqa/chat-search.py) using Google Search + vecdb-retrieval from URL contents. \n  - **0.1.39:** [`GoogleSearchTool`](langroid/agent/tools/google_search_tool.py) to enable Agents (their LLM) to do Google searches via function-calling/tools.\n    See [this chat example](examples/basic/chat-search.py) for how easy it is to add this tool to an agent.\n  - **Colab notebook** to try the quick-start examples: [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/langroid/langroid/blob/main/examples/langroid_quick_examples.ipynb) \n  - **0.1.37:** Added [`SQLChatAgent`](langroid/agent/special/sql_chat_agent.py) -- thanks to our latest contributor [Rithwik Babu](https://github.com/rithwikbabu)!\n  - Multi-agent Example: [Autocorrect chat](examples/basic/autocorrect.py)\n- **July 2023:** \n  - **0.1.30:** Added [`TableChatAgent`](langroid/agent/special/table_chat_agent.py) to \n    [chat](examples/data-qa/table_chat.py) with tabular datasets (dataframes, files, URLs): LLM generates Pandas code,\n    and code is executed using Langroid\'s tool/function-call mechanism. \n  - **Demo:** 3-agent system for Audience [Targeting](https://langroid.github.io/langroid/demos/targeting/audience-targeting/).\n  - **0.1.27**: Added [support](langroid/cachedb/momento_cachedb.py) \n    for [Momento Serverless Cache](https://www.gomomento.com/) as an alternative to Redis.\n  - **0.1.24**: [`DocChatAgent`](langroid/agent/special/doc_chat_agent.py) \n    now [accepts](langroid/parsing/document_parser.py) PDF files or URLs.\n\n</details>\n\n# :rocket: Demo\nSuppose you want to extract structured information about the key terms \nof a commercial lease document. You can easily do this with Langroid using a two-agent system,\nas we show in the [langroid-examples](https://github.com/langroid/langroid-examples/blob/main/examples/docqa/chat_multi_extract.py) repo.\nThe demo showcases just a few of the many features of Langroid, such as:\n- Multi-agent collaboration: `LeaseExtractor` is in charge of the task, and its LLM (GPT4) generates questions \nto be answered by the `DocAgent`.\n- Retrieval augmented question-answering, with **source-citation**: `DocAgent` LLM (GPT4) uses retrieval from a vector-store to \nanswer the `LeaseExtractor`\'s questions, cites the specific excerpt supporting the answer. \n- Function-calling (also known as tool/plugin): When it has all the information it \nneeds, the `LeaseExtractor` LLM presents the information in a structured \nformat using a Function-call. \n\nHere is what it looks like in action \n(a pausable mp4 video is [here](https://vimeo.com/871429249)).\n\n![Demo](docs/assets/demos/lease-extractor-demo.gif)\n\n\n# :zap: Highlights\n\n- **Agents as first-class citizens:** The [Agent](https://langroid.github.io/langroid/reference/agent/base/#langroid.agent.base.Agent) class encapsulates LLM conversation state,\n  and optionally a vector-store and tools. Agents are a core abstraction in Langroid;\n  Agents act as _message transformers_, and by default provide 3 _responder_ methods, one corresponding to each entity: LLM, Agent, User.\n- **Tasks:** A [Task](https://langroid.github.io/langroid/reference/agent/task/) class wraps an Agent, and gives the agent instructions (or roles, or goals), \n  manages iteration over an Agent\'s responder methods, \n  and orchestrates multi-agent interactions via hierarchical, recursive\n  task-delegation. The `Task.run()` method has the same \n  type-signature as an Agent\'s responder\'s methods, and this is key to how \n  a task of an agent can delegate to other sub-tasks: from the point of view of a Task,\n  sub-tasks are simply additional responders, to be used in a round-robin fashion \n  after the agent\'s own responders.\n- **Modularity, Reusabilily, Loose coupling:** The `Agent` and `Task` abstractions allow users to design\n  Agents with specific skills, wrap them in Tasks, and combine tasks in a flexible way.\n- **LLM Support**: Langroid supports OpenAI LLMs as well as LLMs from hundreds of \nproviders (local/open or remote/commercial) via proxy libraries and local model servers\nsuch as [LiteLLM](https://docs.litellm.ai/docs/providers) that in effect mimic the OpenAI API. \n- **Caching of LLM responses:** Langroid supports [Redis](https://redis.com/try-free/) and \n  [Momento](https://www.gomomento.com/) to cache LLM responses.\n- **Vector-stores**: [Qdrant](https://qdrant.tech/) and [Chroma](https://www.trychroma.com/) are currently supported.\n  Vector stores allow for Retrieval-Augmented-Generation (RAG).\n- **Grounding and source-citation:** Access to external documents via vector-stores \n   allows for grounding and source-citation.\n- **Observability, Logging, Lineage:** Langroid generates detailed logs of multi-agent interactions and\n  maintains provenance/lineage of messages, so that you can trace back\n  the origin of a message.\n- **Tools/Plugins/Function-calling**: Langroid supports OpenAI\'s recently\n  released [function calling](https://platform.openai.com/docs/guides/gpt/function-calling)\n  feature. In addition, Langroid has its own native equivalent, which we\n  call **tools** (also known as "plugins" in other contexts). Function\n  calling and tools have the same developer-facing interface, implemented\n  using [Pydantic](https://docs.pydantic.dev/latest/),\n  which makes it very easy to define tools/functions and enable agents\n  to use them. Benefits of using Pydantic are that you never have to write\n  complex JSON specs for function calling, and when the LLM\n  hallucinates malformed JSON, the Pydantic error message is sent back to\n  the LLM so it can fix it!\n\n--- \n\n# :gear: Installation and Setup\n\n### Install `langroid`\nLangroid requires Python 3.11+. We recommend using a virtual environment.\nUse `pip` to install `langroid` (from PyPi) to your virtual environment:\n```bash\npip install langroid\n```\nThe core Langroid package lets you use OpenAI Embeddings models via their API. \nIf you instead want to use the `sentence-transformers` embedding models from HuggingFace, \ninstall Langroid like this: \n```bash\npip install langroid[hf-embeddings]\n```\n\n<details>\n<summary><b>Optional Installs for using SQL Chat with a PostgreSQL DB </b></summary>\n\nIf you are using `SQLChatAgent` \n(e.g. the script [`examples/data-qa/sql-chat/sql_chat.py`](examples/data-qa/sql-chat/sql_chat.py)),\nwith a postgres db, you will need to:\n\n- Install PostgreSQL dev libraries for your platform, e.g.\n  - `sudo apt-get install libpq-dev` on Ubuntu,\n  - `brew install postgresql` on Mac, etc.\n- Install langroid with the postgres extra, e.g. `pip install langroid[postgres]`\n  or `poetry add langroid[postgres]` or `poetry install -E postgres`.\n  If this gives you an error, try `pip install psycopg2-binary` in your virtualenv.\n</details>\n\n### Set up environment variables (API keys, etc)\n\nTo get started, all you need is an OpenAI API Key.\nIf you don\'t have one, see [this OpenAI Page](https://help.openai.com/en/collections/3675940-getting-started-with-openai-api).\nCurrently only OpenAI models are supported. Others will be added later\n(Pull Requests welcome!).\n\nIn the root of the repo, copy the `.env-template` file to a new file `.env`: \n```bash\ncp .env-template .env\n```\nThen insert your OpenAI API Key. \nYour `.env` file should look like this:\n```bash\nOPENAI_API_KEY=your-key-here-without-quotes\n````\n\nAlternatively, you can set this as an environment variable in your shell\n(you will need to do this every time you open a new shell):\n```bash\nexport OPENAI_API_KEY=your-key-here-without-quotes\n```\n\n\n<details>\n<summary><b>Optional Setup Instructions (click to expand) </b></summary>\n\nAll of the following environment variable settings are optional, and some are only needed \nto use specific features (as noted below).\n\n- **Qdrant** Vector Store API Key, URL. This is only required if you want to use Qdrant cloud.\n  You can sign up for a free 1GB account at [Qdrant cloud](https://cloud.qdrant.io).\n  If you skip setting up these, Langroid will use Qdrant in local-storage mode.\n  Alternatively [Chroma](https://docs.trychroma.com/) is also currently supported. \n  We use the local-storage version of Chroma, so there is no need for an API key.\n  Langroid uses Qdrant by default.\n- **Redis** Password, host, port: This is optional, and only needed to cache LLM API responses\n  using Redis Cloud. Redis [offers](https://redis.com/try-free/) a free 30MB Redis account\n  which is more than sufficient to try out Langroid and even beyond.\n  If you don\'t set up these, Langroid will use a pure-python \n  Redis in-memory cache via the [Fakeredis](https://fakeredis.readthedocs.io/en/latest/) library.\n- **Momento** Serverless Caching of LLM API responses (as an alternative to Redis). \n   To use Momento instead of Redis:\n  - enter your Momento Token in the `.env` file, as the value of `MOMENTO_AUTH_TOKEN` (see example file below),\n  - in the `.env` file set `CACHE_TYPE=momento` (instead of `CACHE_TYPE=redis` which is the default).\n- **GitHub** Personal Access Token (required for apps that need to analyze git\n  repos; token-based API calls are less rate-limited). See this\n  [GitHub page](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens).\n- **Google Custom Search API Credentials:** Only needed to enable an Agent to use the `GoogleSearchTool`.\n  To use Google Search as an LLM Tool/Plugin/function-call, \n  you\'ll need to set up \n  [a Google API key](https://developers.google.com/custom-search/v1/introduction#identify_your_application_to_google_with_api_key),\n  then [setup a Google Custom Search Engine (CSE) and get the CSE ID](https://developers.google.com/custom-search/docs/tutorial/creatingcse).\n  (Documentation for these can be challenging, we suggest asking GPT4 for a step-by-step guide.)\n  After obtaining these credentials, store them as values of \n  `GOOGLE_API_KEY` and `GOOGLE_CSE_ID` in your `.env` file. \n  Full documentation on using this (and other such "stateless" tools) is coming soon, but \n  in the meantime take a peek at this [chat example](examples/basic/chat-search.py), which \n  shows how you can easily equip an Agent with a `GoogleSearchtool`.\n  \n\n\nIf you add all of these optional variables, your `.env` file should look like this:\n```bash\nOPENAI_API_KEY=your-key-here-without-quotes\nGITHUB_ACCESS_TOKEN=your-personal-access-token-no-quotes\nCACHE_TYPE=redis # or momento\nREDIS_PASSWORD=your-redis-password-no-quotes\nREDIS_HOST=your-redis-hostname-no-quotes\nREDIS_PORT=your-redis-port-no-quotes\nMOMENTO_AUTH_TOKEN=your-momento-token-no-quotes # instead of REDIS* variables\nQDRANT_API_KEY=your-key\nQDRANT_API_URL=https://your.url.here:6333 # note port number must be included\nGOOGLE_API_KEY=your-key\nGOOGLE_CSE_ID=your-cse-id\n```\n</details>\n\n<details>\n<summary><b>Optional setup instructions for Microsoft Azure OpenAI(click to expand)</b></summary> \n\nWhen using Azure OpenAI, additional environment variables are required in the \n`.env` file.\nThis page [Microsoft Azure OpenAI](https://learn.microsoft.com/en-us/azure/ai-services/openai/chatgpt-quickstart?tabs=command-line&pivots=programming-language-python#environment-variables)\nprovides more information, and you can set each environment variable as follows:\n\n- `AZURE_API_KEY`, from the value of `API_KEY`\n- `AZURE_OPENAI_API_BASE` from the value of `ENDPOINT`, typically looks like `https://your.domain.azure.com`.\n- For `AZURE_OPENAI_API_VERSION`, you can use the default value in `.env-template`, and latest version can be found [here](https://learn.microsoft.com/en-us/azure/ai-services/openai/whats-new#azure-openai-chat-completion-general-availability-ga)\n- `AZURE_OPENAI_DEPLOYMENT_NAME` is the name of the deployed model, which is defined by the user during the model setup \n- `AZURE_GPT_MODEL_NAME` GPT-3.5-Turbo or GPT-4 model names that you chose when you setup your Azure OpenAI account.\n\n</details>\n\n---\n\n# :whale: Docker Instructions\n\nWe provide a containerized version of the [`langroid-examples`](https://github.com/langroid/langroid-examples) \nrepository via this [Docker Image](https://hub.docker.com/r/langroid/langroid).\nAll you need to do is set up environment variables in the `.env` file.\nPlease follow these steps to setup the container:\n\n```bash\n# get the .env file template from `langroid` repo\nwget https://github.com/langroid/langroid/blob/main/.env-template .env\n\n# Edit the .env file with your favorite editor (here nano), \n# and add API keys as explained above\nnano .env\n\n# launch the container\ndocker run -it  -v ./.env:/.env langroid/langroid\n\n# Use this command to run any of the scripts in the `examples` directory\npython examples/<Path/To/Example.py> \n``` \n\n\n\n# :tada: Usage Examples\n\nThese are quick teasers to give a glimpse of what you can do with Langroid\nand how your code would look. \n\n:warning: The code snippets below are intended to give a flavor of the code\nand they are **not** complete runnable examples! For that we encourage you to \nconsult the [`langroid-examples`](https://github.com/langroid/langroid-examples) \nrepository.\n\n:information_source: The various LLM prompts and instructions in Langroid\nhave been tested to work well with GPT4.\nSwitching to GPT3.5-Turbo is easy via a config flag\n(e.g., `cfg = OpenAIGPTConfig(chat_model=OpenAIChatModel.GPT3_5_TURBO)`),\nand may suffice for some applications, but in general you may see inferior results.\n\n\n:book: Also see the\n[`Getting Started Guide`](https://langroid.github.io/langroid/quick-start/)\nfor a detailed tutorial.\n\n\n\nClick to expand any of the code examples below.\nAll of these can be run in a Colab notebook:\n[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/langroid/langroid/blob/main/examples/langroid_quick_examples.ipynb)\n\n<details>\n<summary> <b> Direct interaction with OpenAI LLM </b> </summary>\n\n```python\nfrom langroid.language_models.openai_gpt import ( \n        OpenAIGPTConfig, OpenAIChatModel, OpenAIGPT,\n)\nfrom langroid.language_models.base import LLMMessage, Role\n\ncfg = OpenAIGPTConfig(chat_model=OpenAIChatModel.GPT4)\n\nmdl = OpenAIGPT(cfg)\n\nmessages = [\n  LLMMessage(content="You are a helpful assistant",  role=Role.SYSTEM), \n  LLMMessage(content="What is the capital of Ontario?",  role=Role.USER),\n]\nresponse = mdl.chat(messages, max_tokens=200)\nprint(response.message)\n```\n</details>\n\n<details>\n<summary> <b> Interaction with non-OpenAI LLM (local or remote) </b> </summary>\nLocal model: if model is served at `http://localhost:8000`:\n\n```python\ncfg = OpenAIGPTConfig(\n  chat_model="local/localhost:8000", \n  chat_context_length=4096\n)\nmdl = OpenAIGPT(cfg)\n# now interact with it as above, or create an Agent + Task as shown below.\n```\n\nIf the model is [supported by `liteLLM`](https://docs.litellm.ai/docs/providers), \nthen no need to launch the proxy server.\nJust set the `chat_model` param above to `litellm/[provider]/[model]`, e.g. \n`litellm/anthropic/claude-instant-1` and use the config object as above.\nFor remote models, you will typically need to set API Keys etc as environment variables.\nYou can set those based on the LiteLLM docs. \nIf any required environment variables are missing, Langroid gives a helpful error\nmessage indicating which ones are needed.\n</details>\n\n<details>\n<summary> <b> Define an agent, set up a task, and run it </b> </summary>\n\n```python\nfrom langroid.agent.chat_agent import ChatAgent, ChatAgentConfig\nfrom langroid.agent.task import Task\nfrom langroid.language_models.openai_gpt import OpenAIChatModel, OpenAIGPTConfig\n\nconfig = ChatAgentConfig(\n    llm = OpenAIGPTConfig(\n        chat_model=OpenAIChatModel.GPT4,\n    ),\n    vecdb=None, # no vector store\n)\nagent = ChatAgent(config)\n# get response from agent\'s LLM, and put this in an interactive loop...\n# answer = agent.llm_response("What is the capital of Ontario?")\n  # ... OR instead, set up a task (which has a built-in loop) and run it\ntask = Task(agent, name="Bot") \ntask.run() # ... a loop seeking response from LLM or User at each turn\n```\n</details>\n\n<details>\n<summary><b> Three communicating agents </b></summary>\n\nA toy numbers game, where when given a number `n`:\n- `repeater_agent`\'s LLM simply returns `n`,\n- `even_agent`\'s LLM returns `n/2` if `n` is even, else says "DO-NOT-KNOW"\n- `odd_agent`\'s LLM returns `3*n+1` if `n` is odd, else says "DO-NOT-KNOW"\n\nFirst define the 3 agents, and set up their tasks with instructions:\n\n```python\nfrom langroid.utils.constants import NO_ANSWER\nfrom langroid.agent.chat_agent import ChatAgent, ChatAgentConfig\nfrom langroid.agent.task import Task\nfrom langroid.language_models.openai_gpt import OpenAIChatModel, OpenAIGPTConfig\nconfig = ChatAgentConfig(\n    llm = OpenAIGPTConfig(\n        chat_model=OpenAIChatModel.GPT4,\n    ),\n    vecdb = None,\n)\nrepeater_agent = ChatAgent(config)\nrepeater_task = Task(\n    repeater_agent,\n    name = "Repeater",\n    system_message="""\n    Your job is to repeat whatever number you receive.\n    """,\n    llm_delegate=True, # LLM takes charge of task\n    single_round=False, \n)\neven_agent = ChatAgent(config)\neven_task = Task(\n    even_agent,\n    name = "EvenHandler",\n    system_message=f"""\n    You will be given a number. \n    If it is even, divide by 2 and say the result, nothing else.\n    If it is odd, say {NO_ANSWER}\n    """,\n    single_round=True,  # task done after 1 step() with valid response\n)\n\nodd_agent = ChatAgent(config)\nodd_task = Task(\n    odd_agent,\n    name = "OddHandler",\n    system_message=f"""\n    You will be given a number n. \n    If it is odd, return (n*3+1), say nothing else. \n    If it is even, say {NO_ANSWER}\n    """,\n    single_round=True,  # task done after 1 step() with valid response\n)\n```\nThen add the `even_task` and `odd_task` as sub-tasks of `repeater_task`, \nand run the `repeater_task`, kicking it off with a number as input:\n```python\nrepeater_task.add_sub_task([even_task, odd_task])\nrepeater_task.run("3")\n```\n\n</details>\n\n<details>\n<summary><b> Simple Tool/Function-calling example </b></summary>\n\nLangroid leverages Pydantic to support OpenAI\'s\n[Function-calling API](https://platform.openai.com/docs/guides/gpt/function-calling)\nas well as its own native tools. The benefits are that you don\'t have to write\nany JSON to specify the schema, and also if the LLM hallucinates a malformed\ntool syntax, Langroid sends the Pydantic validation error (suitiably sanitized) \nto the LLM so it can fix it!\n\nSimple example: Say the agent has a secret list of numbers, \nand we want the LLM to find the smallest number in the list. \nWe want to give the LLM a `probe` tool/function which takes a\nsingle number `n` as argument. The tool handler method in the agent\nreturns how many numbers in its list are at most `n`.\n\nFirst define the tool using Langroid\'s `ToolMessage` class:\n\n\n```python\nfrom langroid.agent.tool_message import ToolMessage\nclass ProbeTool(ToolMessage):\n  request: str = "probe" # specifies which agent method handles this tool\n  purpose: str = """\n        To find how many numbers in my list are less than or equal to  \n        the <number> you specify.\n        """ # description used to instruct the LLM on when/how to use the tool\n  number: int  # required argument to the tool\n```\n\nThen define a `SpyGameAgent` as a subclass of `ChatAgent`, \nwith a method `probe` that handles this tool:\n\n```python\nfrom langroid.agent.chat_agent import ChatAgent, ChatAgentConfig\nclass SpyGameAgent(ChatAgent):\n  def __init__(self, config: ChatAgentConfig):\n    super().__init__(config)\n    self.numbers = [3, 4, 8, 11, 15, 25, 40, 80, 90]\n\n  def probe(self, msg: ProbeTool) -> str:\n    # return how many numbers in self.numbers are less or equal to msg.number\n    return str(len([n for n in self.numbers if n <= msg.number]))\n```\n\nWe then instantiate the agent and enable it to use and respond to the tool:\n\n```python\nfrom langroid.language_models.openai_gpt import OpenAIChatModel, OpenAIGPTConfig\nspy_game_agent = SpyGameAgent(\n    ChatAgentConfig(\n        name="Spy",\n        llm = OpenAIGPTConfig(\n            chat_model=OpenAIChatModel.GPT4,\n        ),\n        vecdb=None,\n        use_tools=False, #  don\'t use Langroid native tool\n        use_functions_api=True, # use OpenAI function-call API\n    )\n)\nspy_game_agent.enable_message(ProbeTool)\n```\n\nFor a full working example see the\n[chat-agent-tool.py](https://github.com/langroid/langroid-examples/blob/main/examples/quick-start/chat-agent-tool.py)\nscript in the `langroid-examples` repo.\n</details>\n\n<details>\n<summary> <b>Tool/Function-calling to extract structured information from text </b> </summary>\n\nSuppose you want an agent to extract \nthe key terms of a lease, from a lease document, as a nested JSON structure.\nFirst define the desired structure via Pydantic models:\n\n```python\nfrom pydantic import BaseModel\nclass LeasePeriod(BaseModel):\n    start_date: str\n    end_date: str\n\n\nclass LeaseFinancials(BaseModel):\n    monthly_rent: str\n    deposit: str\n\nclass Lease(BaseModel):\n    period: LeasePeriod\n    financials: LeaseFinancials\n    address: str\n```\n\nThen define the `LeaseMessage` tool as a subclass of Langroid\'s `ToolMessage`.\nNote the tool has a required argument `terms` of type `Lease`:\n\n```python\nclass LeaseMessage(ToolMessage):\n    request: str = "lease_info"\n    purpose: str = """\n        Collect information about a Commercial Lease.\n        """\n    terms: Lease\n```\n\nThen define a `LeaseExtractorAgent` with a method `lease_info` that handles this tool,\ninstantiate the agent, and enable it to use and respond to this tool:\n\n```python\nclass LeaseExtractorAgent(ChatAgent):\n    def lease_info(self, message: LeaseMessage) -> str:\n        print(\n            f"""\n        DONE! Successfully extracted Lease Info:\n        {message.terms}\n        """\n        )\n        return json.dumps(message.terms.dict())\n    \nlease_extractor_agent = LeaseExtractorAgent(\n  ChatAgentConfig(\n    llm=OpenAIGPTConfig(),\n    use_functions_api=False,\n    use_tools=True,\n  )\n)\nlease_extractor_agent.enable_message(LeaseMessage)\n```\n\nSee the [`chat_multi_extract.py`](https://github.com/langroid/langroid-examples/blob/main/examples/docqa/chat_multi_extract.py)\nscript in the `langroid-examples` repo for a full working example.\n</details>\n\n<details>\n<summary><b> Chat with documents (file paths, URLs, etc) </b></summary>\n\nLangroid provides a specialized agent class `DocChatAgent` for this purpose.\nIt incorporates document sharding, embedding, storage in a vector-DB, \nand retrieval-augmented query-answer generation.\nUsing this class to chat with a collection of documents is easy.\nFirst create a `DocChatAgentConfig` instance, with a \n`doc_paths` field that specifies the documents to chat with.\n\n```python\nfrom langroid.agent.doc_chat_agent import DocChatAgentConfig\nfrom langroid.vector_store.qdrantdb import QdrantDBConfig\nconfig = DocChatAgentConfig(\n  doc_paths = [\n    "https://en.wikipedia.org/wiki/Language_model",\n    "https://en.wikipedia.org/wiki/N-gram_language_model",\n    "/path/to/my/notes-on-language-models.txt",\n  ]\n  llm = OpenAIGPTConfig(\n    chat_model=OpenAIChatModel.GPT4,\n  ),\n  vecdb=QdrantDBConfig()\n)\n```\n\nThen instantiate the `DocChatAgent` (this ingests the docs into the vector-store):\n\n```python\nagent = DocChatAgent(config)\n```\nThen we can either ask the agent one-off questions,\n```python\nagent.chat("What is a language model?")\n```\nor wrap it in a `Task` and run an interactive loop with the user:\n```python\nfrom langroid.task import Task\ntask = Task(agent)\ntask.run()\n```\n\nSee full working scripts in the \n[`docqa`](https://github.com/langroid/langroid-examples/tree/main/examples/docqa)\nfolder of the `langroid-examples` repo.\n</details>\n\n<details>\n<summary><b> :fire: Chat with tabular data (file paths, URLs, dataframes) </b></summary>\n\nUsing Langroid you can set up a `TableChatAgent` with a dataset (file path, URL or dataframe),\nand query it. The Agent\'s LLM generates Pandas code to answer the query, \nvia function-calling (or tool/plugin), and the Agent\'s function-handling method\nexecutes the code and returns the answer.\n\nHere is how you can do this:\n\n```python\nfrom langroid.agent.special.table_chat_agent import TableChatAgent, TableChatAgentConfig\nfrom langroid.agent.task import Task\nfrom langroid.language_models.openai_gpt import OpenAIChatModel, OpenAIGPTConfig\n```\n\nSet up a `TableChatAgent` for a data file, URL or dataframe\n(Ensure the data table has a header row; the delimiter/separator is auto-detected):\n```python\ndataset =  "https://archive.ics.uci.edu/ml/machine-learning-databases/wine-quality/winequality-red.csv"\n# or dataset = "/path/to/my/data.csv"\n# or dataset = pd.read_csv("/path/to/my/data.csv")\nagent = TableChatAgent(\n    config=TableChatAgentConfig(\n        data=dataset,  \n        llm=OpenAIGPTConfig(\n            chat_model=OpenAIChatModel.GPT4,\n        ),\n    )\n)\n```\nSet up a task, and ask one-off questions like this: \n\n```python\ntask = Task(\n  agent, \n  name = "DataAssistant",\n  default_human_response="", # to avoid waiting for user input\n)\nresult = task.run(\n  "What is the average alcohol content of wines with a quality rating above 7?",\n  turns=2 # return after user question, LLM fun-call/tool response, Agent code-exec result\n) \nprint(result.content)\n```\nOr alternatively, set up a task and run it in an interactive loop with the user:\n\n```python\ntask = Task(agent, name="DataAssistant")\ntask.run()\n``` \n\nFor a full working example see the \n[`table_chat.py`](https://github.com/langroid/langroid-examples/tree/main/examples/data-qa/table_chat.py)\nscript in the `langroid-examples` repo.\n\n\n</details>\n\n---\n\n# :heart: Thank you to our [supporters](https://github.com/langroid/langroid/stargazers)\n\nIf you like this project, please give it a star ⭐ and 📢 spread the word in your network or social media:\n\n[![Share on Twitter](https://img.shields.io/twitter/url?style=social&url=https://github.com/langroid/langroid)](https://twitter.com/intent/tweet?text=Langroid%20is%20a%20powerful,%20elegant%20new%20framework%20to%20easily%20build%20%23LLM%20applications.%20You%20set%20up%20LLM-powered%20Agents%20with%20vector-stores,%20assign%20tasks,%20and%20have%20them%20collaboratively%20solve%20problems%20via%20message-transformations.%20https://github.com/langroid/langroid)\n[![Share on LinkedIn](https://img.shields.io/badge/Share%20on-LinkedIn-blue)](https://www.linkedin.com/shareArticle?mini=true&url=https://github.com/langroid/langroid&title=Langroid:%20A%20Powerful,%20Elegant%20Framework&summary=Langroid%20is%20a%20powerful,%20elegant%20new%20framework%20to%20easily%20build%20%23LLM%20applications.%20You%20set%20up%20LLM-powered%20Agents%20with%20vector-stores,%20assign%20tasks,%20and%20have%20them%20collaboratively%20solve%20problems%20via%20message-transformations.)\n[![Share on Hacker News](https://img.shields.io/badge/-Share%20on%20Hacker%20News-orange)](https://news.ycombinator.com/submitlink?u=https%3A%2F%2Fgithub.com%2Flangroid%2Flangroid&t=Harness%20LLMs%20with%20Multi-Agent%20Programming)\n[![Share on Reddit](https://img.shields.io/badge/-Share%20on%20Reddit-blue)](https://www.reddit.com/submit?url=https%3A%2F%2Fgithub.com%2Flangroid%2Flangroid&title=Harness%20LLMs%20with%20Multi-Agent%20Programming)\n\n\n\n\nYour support will help build Langroid\'s momentum and community.\n\n\n\n\n# Langroid Co-Founders\n\n- [Prasad Chalasani](https://www.linkedin.com/in/pchalasani/) (IIT BTech/CS, CMU PhD/ML; Independent ML Consultant)\n- [Somesh Jha](https://www.linkedin.com/in/somesh-jha-80208015/) (IIT BTech/CS, CMU PhD/CS; Professor of CS, U Wisc at Madison)\n\n\n\n',
     'author': 'Prasad Chalasani',
     'author_email': 'pchalasani@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `langroid-0.1.98/PKG-INFO` & `langroid-0.1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langroid
-Version: 0.1.98
+Version: 0.1.99
 Summary: Harness LLMs with Multi-Agent Programming
 License: MIT
 Author: Prasad Chalasani
 Author-email: pchalasani@gmail.com
 Requires-Python: >=3.9.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

