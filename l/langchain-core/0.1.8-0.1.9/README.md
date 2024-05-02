# Comparing `tmp/langchain_core-0.1.8.tar.gz` & `tmp/langchain_core-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_core-0.1.8.tar", max compression
+gzip compressed data, was "langchain_core-0.1.9.tar", max compression
```

## Comparing `langchain_core-0.1.8.tar` & `langchain_core-0.1.9.tar`

### file list

```diff
@@ -1,119 +1,120 @@
--rw-r--r--   0        0        0     3046 2024-01-08 05:05:42.570001 langchain_core-0.1.8/README.md
--rw-r--r--   0        0        0      390 2024-01-08 05:05:42.570001 langchain_core-0.1.8/langchain_core/__init__.py
--rw-r--r--   0        0        0     1025 2024-01-08 05:05:42.570001 langchain_core-0.1.8/langchain_core/_api/__init__.py
--rw-r--r--   0        0        0     8977 2024-01-08 05:05:42.570001 langchain_core-0.1.8/langchain_core/_api/beta_decorator.py
--rw-r--r--   0        0        0    12552 2024-01-08 05:05:42.570001 langchain_core-0.1.8/langchain_core/_api/deprecation.py
--rw-r--r--   0        0        0      662 2024-01-08 05:05:42.570001 langchain_core-0.1.8/langchain_core/_api/internal.py
--rw-r--r--   0        0        0      984 2024-01-08 05:05:42.570001 langchain_core-0.1.8/langchain_core/_api/path.py
--rw-r--r--   0        0        0     6197 2024-01-08 05:05:42.570001 langchain_core-0.1.8/langchain_core/agents.py
--rw-r--r--   0        0        0        0 2024-01-08 05:05:42.570001 langchain_core-0.1.8/langchain_core/beta/__init__.py
--rw-r--r--   0        0        0        0 2024-01-08 05:05:42.570001 langchain_core-0.1.8/langchain_core/beta/runnables/__init__.py
--rw-r--r--   0        0        0    10617 2024-01-08 05:05:42.570001 langchain_core-0.1.8/langchain_core/beta/runnables/context.py
--rw-r--r--   0        0        0      722 2024-01-08 05:05:42.570001 langchain_core-0.1.8/langchain_core/caches.py
--rw-r--r--   0        0        0     1852 2024-01-08 05:05:42.570001 langchain_core-0.1.8/langchain_core/callbacks/__init__.py
--rw-r--r--   0        0        0    16850 2024-01-08 05:05:42.570001 langchain_core-0.1.8/langchain_core/callbacks/base.py
--rw-r--r--   0        0        0    62827 2024-01-08 05:05:42.570001 langchain_core-0.1.8/langchain_core/callbacks/manager.py
--rw-r--r--   0        0        0     2256 2024-01-08 05:05:42.570001 langchain_core-0.1.8/langchain_core/callbacks/stdout.py
--rw-r--r--   0        0        0     2433 2024-01-08 05:05:42.570001 langchain_core-0.1.8/langchain_core/callbacks/streaming_stdout.py
--rw-r--r--   0        0        0     2493 2024-01-08 05:05:42.570001 langchain_core-0.1.8/langchain_core/chat_history.py
--rw-r--r--   0        0        0      415 2024-01-08 05:05:42.570001 langchain_core-0.1.8/langchain_core/chat_sessions.py
--rw-r--r--   0        0        0      176 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/documents/__init__.py
--rw-r--r--   0        0        0      839 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/documents/base.py
--rw-r--r--   0        0        0     2494 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/documents/transformers.py
--rw-r--r--   0        0        0      787 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/embeddings.py
--rw-r--r--   0        0        0      486 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/env.py
--rw-r--r--   0        0        0      571 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/example_selectors/__init__.py
--rw-r--r--   0        0        0      516 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/example_selectors/base.py
--rw-r--r--   0        0        0     2453 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/example_selectors/length_based.py
--rw-r--r--   0        0        0     7143 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/example_selectors/semantic_similarity.py
--rw-r--r--   0        0        0     1869 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/exceptions.py
--rw-r--r--   0        0        0     8376 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/globals/__init__.py
--rw-r--r--   0        0        0      522 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/language_models/__init__.py
--rw-r--r--   0        0        0    10688 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/language_models/base.py
--rw-r--r--   0        0        0    29147 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/language_models/chat_models.py
--rw-r--r--   0        0        0    41173 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/language_models/llms.py
--rw-r--r--   0        0        0      261 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/load/__init__.py
--rw-r--r--   0        0        0     1174 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/load/dump.py
--rw-r--r--   0        0        0     5333 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/load/load.py
--rw-r--r--   0        0        0    16194 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/load/mapping.py
--rw-r--r--   0        0        0     6237 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/load/serializable.py
--rw-r--r--   0        0        0     2019 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/memory.py
--rw-r--r--   0        0        0     4642 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/messages/__init__.py
--rw-r--r--   0        0        0     1754 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/messages/ai.py
--rw-r--r--   0        0        0     6254 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/messages/base.py
--rw-r--r--   0        0        0     2047 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/messages/chat.py
--rw-r--r--   0        0        0     1759 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/messages/function.py
--rw-r--r--   0        0        0     1093 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/messages/human.py
--rw-r--r--   0        0        0     1046 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/messages/system.py
--rw-r--r--   0        0        0     1753 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/messages/tool.py
--rw-r--r--   0        0        0     1044 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/output_parsers/__init__.py
--rw-r--r--   0        0        0     9740 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/output_parsers/base.py
--rw-r--r--   0        0        0      527 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/output_parsers/format_instructions.py
--rw-r--r--   0        0        0     7839 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/output_parsers/json.py
--rw-r--r--   0        0        0     5507 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/output_parsers/list.py
--rw-r--r--   0        0        0      789 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/output_parsers/string.py
--rw-r--r--   0        0        0     4466 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/output_parsers/transform.py
--rw-r--r--   0        0        0     6056 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/output_parsers/xml.py
--rw-r--r--   0        0        0      482 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/outputs/__init__.py
--rw-r--r--   0        0        0     2633 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/outputs/chat_generation.py
--rw-r--r--   0        0        0      511 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/outputs/chat_result.py
--rw-r--r--   0        0        0     1848 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/outputs/generation.py
--rw-r--r--   0        0        0     2448 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/outputs/llm_result.py
--rw-r--r--   0        0        0      295 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/outputs/run_info.py
--rw-r--r--   0        0        0     2662 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/prompt_values.py
--rw-r--r--   0        0        0     2581 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/prompts/__init__.py
--rw-r--r--   0        0        0     8813 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/prompts/base.py
--rw-r--r--   0        0        0    25391 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/prompts/chat.py
--rw-r--r--   0        0        0    11888 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/prompts/few_shot.py
--rw-r--r--   0        0        0     5817 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/prompts/few_shot_with_templates.py
--rw-r--r--   0        0        0     6357 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/prompts/loading.py
--rw-r--r--   0        0        0     2498 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/prompts/pipeline.py
--rw-r--r--   0        0        0     9833 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/prompts/prompt.py
--rw-r--r--   0        0        0     5684 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/prompts/string.py
--rw-r--r--   0        0        0        0 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/py.typed
--rw-r--r--   0        0        0      927 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/pydantic_v1/__init__.py
--rw-r--r--   0        0        0      134 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/pydantic_v1/dataclasses.py
--rw-r--r--   0        0        0      120 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/pydantic_v1/main.py
--rw-r--r--   0        0        0    10835 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/retrievers.py
--rw-r--r--   0        0        0     2184 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/runnables/__init__.py
--rw-r--r--   0        0        0   143823 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/runnables/base.py
--rw-r--r--   0        0        0    14400 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/runnables/branch.py
--rw-r--r--   0        0        0    16801 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/runnables/config.py
--rw-r--r--   0        0        0    16031 2024-01-08 05:05:42.574001 langchain_core-0.1.8/langchain_core/runnables/configurable.py
--rw-r--r--   0        0        0    11862 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/runnables/fallbacks.py
--rw-r--r--   0        0        0     5044 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/runnables/graph.py
--rw-r--r--   0        0        0     8703 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/runnables/graph_draw.py
--rw-r--r--   0        0        0    15977 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/runnables/history.py
--rw-r--r--   0        0        0    21912 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/runnables/passthrough.py
--rw-r--r--   0        0        0    11952 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/runnables/retry.py
--rw-r--r--   0        0        0     6274 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/runnables/router.py
--rw-r--r--   0        0        0    12554 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/runnables/utils.py
--rw-r--r--   0        0        0     1647 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/stores.py
--rw-r--r--   0        0        0    30198 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/tools.py
--rw-r--r--   0        0        0      598 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/tracers/__init__.py
--rw-r--r--   0        0        0    18584 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/tracers/base.py
--rw-r--r--   0        0        0     7626 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/tracers/context.py
--rw-r--r--   0        0        0     8220 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/tracers/evaluation.py
--rw-r--r--   0        0        0     9208 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/tracers/langchain.py
--rw-r--r--   0        0        0     7467 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/tracers/langchain_v1.py
--rw-r--r--   0        0        0    11231 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/tracers/log_stream.py
--rw-r--r--   0        0        0     1706 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/tracers/root_listeners.py
--rw-r--r--   0        0        0     1532 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/tracers/run_collector.py
--rw-r--r--   0        0        0     4265 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/tracers/schemas.py
--rw-r--r--   0        0        0     6186 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/tracers/stdout.py
--rw-r--r--   0        0        0     1232 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/utils/__init__.py
--rw-r--r--   0        0        0     7198 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/utils/aiter.py
--rw-r--r--   0        0        0     1297 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/utils/env.py
--rw-r--r--   0        0        0      907 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/utils/formatting.py
--rw-r--r--   0        0        0     6666 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/utils/function_calling.py
--rw-r--r--   0        0        0     3090 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/utils/html.py
--rw-r--r--   0        0        0     1289 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/utils/input.py
--rw-r--r--   0        0        0     5822 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/utils/iter.py
--rw-r--r--   0        0        0     2318 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/utils/json_schema.py
--rw-r--r--   0        0        0     2011 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/utils/loading.py
--rw-r--r--   0        0        0      301 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/utils/pydantic.py
--rw-r--r--   0        0        0      908 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/utils/strings.py
--rw-r--r--   0        0        0     6160 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/utils/utils.py
--rw-r--r--   0        0        0    25692 2024-01-08 05:05:42.578001 langchain_core-0.1.8/langchain_core/vectorstores.py
--rw-r--r--   0        0        0     2725 2024-01-08 05:05:42.578001 langchain_core-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4006 1970-01-01 00:00:00.000000 langchain_core-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     3046 2024-01-10 03:28:32.000835 langchain_core-0.1.9/README.md
+-rw-r--r--   0        0        0      390 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/__init__.py
+-rw-r--r--   0        0        0     1025 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/_api/__init__.py
+-rw-r--r--   0        0        0     8977 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/_api/beta_decorator.py
+-rw-r--r--   0        0        0    13829 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/_api/deprecation.py
+-rw-r--r--   0        0        0      662 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/_api/internal.py
+-rw-r--r--   0        0        0      984 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/_api/path.py
+-rw-r--r--   0        0        0     6197 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/agents.py
+-rw-r--r--   0        0        0        0 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/beta/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/beta/runnables/__init__.py
+-rw-r--r--   0        0        0    10617 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/beta/runnables/context.py
+-rw-r--r--   0        0        0      722 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/caches.py
+-rw-r--r--   0        0        0     1852 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/callbacks/__init__.py
+-rw-r--r--   0        0        0    16850 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/callbacks/base.py
+-rw-r--r--   0        0        0    62827 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/callbacks/manager.py
+-rw-r--r--   0        0        0     2256 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/callbacks/stdout.py
+-rw-r--r--   0        0        0     2433 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/callbacks/streaming_stdout.py
+-rw-r--r--   0        0        0     2493 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/chat_history.py
+-rw-r--r--   0        0        0      415 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/chat_sessions.py
+-rw-r--r--   0        0        0      176 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/documents/__init__.py
+-rw-r--r--   0        0        0      839 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/documents/base.py
+-rw-r--r--   0        0        0     2494 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/documents/transformers.py
+-rw-r--r--   0        0        0      787 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/embeddings.py
+-rw-r--r--   0        0        0      486 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/env.py
+-rw-r--r--   0        0        0      571 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/example_selectors/__init__.py
+-rw-r--r--   0        0        0      516 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/example_selectors/base.py
+-rw-r--r--   0        0        0     2453 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/example_selectors/length_based.py
+-rw-r--r--   0        0        0     7143 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/example_selectors/semantic_similarity.py
+-rw-r--r--   0        0        0     1869 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/exceptions.py
+-rw-r--r--   0        0        0     8376 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/globals/__init__.py
+-rw-r--r--   0        0        0      522 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/language_models/__init__.py
+-rw-r--r--   0        0        0    10688 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/language_models/base.py
+-rw-r--r--   0        0        0    29147 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/language_models/chat_models.py
+-rw-r--r--   0        0        0    41173 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/language_models/llms.py
+-rw-r--r--   0        0        0      261 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/load/__init__.py
+-rw-r--r--   0        0        0     1174 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/load/dump.py
+-rw-r--r--   0        0        0     5333 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/load/load.py
+-rw-r--r--   0        0        0    16194 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/load/mapping.py
+-rw-r--r--   0        0        0     6237 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/load/serializable.py
+-rw-r--r--   0        0        0     2019 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/memory.py
+-rw-r--r--   0        0        0     4642 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/messages/__init__.py
+-rw-r--r--   0        0        0     1754 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/messages/ai.py
+-rw-r--r--   0        0        0     6254 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/messages/base.py
+-rw-r--r--   0        0        0     2047 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/messages/chat.py
+-rw-r--r--   0        0        0     1759 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/messages/function.py
+-rw-r--r--   0        0        0     1093 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/messages/human.py
+-rw-r--r--   0        0        0     1046 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/messages/system.py
+-rw-r--r--   0        0        0     1753 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/messages/tool.py
+-rw-r--r--   0        0        0     1044 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/output_parsers/__init__.py
+-rw-r--r--   0        0        0     9740 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/output_parsers/base.py
+-rw-r--r--   0        0        0      527 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/output_parsers/format_instructions.py
+-rw-r--r--   0        0        0     7839 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/output_parsers/json.py
+-rw-r--r--   0        0        0     5507 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/output_parsers/list.py
+-rw-r--r--   0        0        0      789 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/output_parsers/string.py
+-rw-r--r--   0        0        0     4466 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/output_parsers/transform.py
+-rw-r--r--   0        0        0     6056 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/output_parsers/xml.py
+-rw-r--r--   0        0        0      482 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/outputs/__init__.py
+-rw-r--r--   0        0        0     2633 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/outputs/chat_generation.py
+-rw-r--r--   0        0        0      511 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/outputs/chat_result.py
+-rw-r--r--   0        0        0     1848 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/outputs/generation.py
+-rw-r--r--   0        0        0     2448 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/outputs/llm_result.py
+-rw-r--r--   0        0        0      295 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/outputs/run_info.py
+-rw-r--r--   0        0        0     2662 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/prompt_values.py
+-rw-r--r--   0        0        0     2581 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/prompts/__init__.py
+-rw-r--r--   0        0        0     8813 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/prompts/base.py
+-rw-r--r--   0        0        0    25391 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/prompts/chat.py
+-rw-r--r--   0        0        0    11888 2024-01-10 03:28:32.000835 langchain_core-0.1.9/langchain_core/prompts/few_shot.py
+-rw-r--r--   0        0        0     5817 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/prompts/few_shot_with_templates.py
+-rw-r--r--   0        0        0     6357 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/prompts/loading.py
+-rw-r--r--   0        0        0     2498 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/prompts/pipeline.py
+-rw-r--r--   0        0        0     9833 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/prompts/prompt.py
+-rw-r--r--   0        0        0     5684 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/prompts/string.py
+-rw-r--r--   0        0        0        0 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/py.typed
+-rw-r--r--   0        0        0      927 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/pydantic_v1/__init__.py
+-rw-r--r--   0        0        0      134 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/pydantic_v1/dataclasses.py
+-rw-r--r--   0        0        0      120 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/pydantic_v1/main.py
+-rw-r--r--   0        0        0    10835 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/retrievers.py
+-rw-r--r--   0        0        0     2184 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/runnables/__init__.py
+-rw-r--r--   0        0        0   143823 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/runnables/base.py
+-rw-r--r--   0        0        0    14400 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/runnables/branch.py
+-rw-r--r--   0        0        0    16801 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/runnables/config.py
+-rw-r--r--   0        0        0    16031 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/runnables/configurable.py
+-rw-r--r--   0        0        0    11862 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/runnables/fallbacks.py
+-rw-r--r--   0        0        0     5044 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/runnables/graph.py
+-rw-r--r--   0        0        0     8703 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/runnables/graph_draw.py
+-rw-r--r--   0        0        0    15977 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/runnables/history.py
+-rw-r--r--   0        0        0    21912 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/runnables/passthrough.py
+-rw-r--r--   0        0        0    11952 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/runnables/retry.py
+-rw-r--r--   0        0        0     6274 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/runnables/router.py
+-rw-r--r--   0        0        0    12554 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/runnables/utils.py
+-rw-r--r--   0        0        0     1647 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/stores.py
+-rw-r--r--   0        0        0     1604 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/sys_info.py
+-rw-r--r--   0        0        0    30198 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/tools.py
+-rw-r--r--   0        0        0      598 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/tracers/__init__.py
+-rw-r--r--   0        0        0    18584 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/tracers/base.py
+-rw-r--r--   0        0        0     7626 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/tracers/context.py
+-rw-r--r--   0        0        0     8220 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/tracers/evaluation.py
+-rw-r--r--   0        0        0     9208 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/tracers/langchain.py
+-rw-r--r--   0        0        0     7467 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/tracers/langchain_v1.py
+-rw-r--r--   0        0        0    11231 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/tracers/log_stream.py
+-rw-r--r--   0        0        0     1706 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/tracers/root_listeners.py
+-rw-r--r--   0        0        0     1532 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/tracers/run_collector.py
+-rw-r--r--   0        0        0     4265 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/tracers/schemas.py
+-rw-r--r--   0        0        0     6186 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/tracers/stdout.py
+-rw-r--r--   0        0        0     1232 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/utils/__init__.py
+-rw-r--r--   0        0        0     7198 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/utils/aiter.py
+-rw-r--r--   0        0        0     1297 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/utils/env.py
+-rw-r--r--   0        0        0      907 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/utils/formatting.py
+-rw-r--r--   0        0        0     6666 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/utils/function_calling.py
+-rw-r--r--   0        0        0     3090 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/utils/html.py
+-rw-r--r--   0        0        0     1289 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/utils/input.py
+-rw-r--r--   0        0        0     5822 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/utils/iter.py
+-rw-r--r--   0        0        0     2318 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/utils/json_schema.py
+-rw-r--r--   0        0        0     2011 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/utils/loading.py
+-rw-r--r--   0        0        0      301 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/utils/pydantic.py
+-rw-r--r--   0        0        0      908 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/utils/strings.py
+-rw-r--r--   0        0        0     6160 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/utils/utils.py
+-rw-r--r--   0        0        0    25692 2024-01-10 03:28:32.004835 langchain_core-0.1.9/langchain_core/vectorstores.py
+-rw-r--r--   0        0        0     2725 2024-01-10 03:28:32.004835 langchain_core-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4006 1970-01-01 00:00:00.000000 langchain_core-0.1.9/PKG-INFO
```

### Comparing `langchain_core-0.1.8/README.md` & `langchain_core-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/_api/__init__.py` & `langchain_core-0.1.9/langchain_core/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/_api/beta_decorator.py` & `langchain_core-0.1.9/langchain_core/_api/beta_decorator.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/_api/deprecation.py` & `langchain_core-0.1.9/langchain_core/_api/deprecation.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 def deprecated(
     since: str,
     *,
     message: str = "",
     name: str = "",
     alternative: str = "",
+    alternative_import: str = "",
     pending: bool = False,
     obj_type: str = "",
     addendum: str = "",
     removal: str = "",
 ) -> Callable[[T], T]:
     """Decorator to mark a function, a class, or a property as deprecated.
 
@@ -101,26 +102,28 @@
     def deprecate(
         obj: T,
         *,
         _obj_type: str = obj_type,
         _name: str = name,
         _message: str = message,
         _alternative: str = alternative,
+        _alternative_import: str = alternative_import,
         _pending: bool = pending,
         _addendum: str = addendum,
     ) -> T:
         """Implementation of the decorator returned by `deprecated`."""
 
         def emit_warning() -> None:
             """Emit the warning."""
             warn_deprecated(
                 since,
                 message=_message,
                 name=_name,
                 alternative=_alternative,
+                alternative_import=_alternative_import,
                 pending=_pending,
                 obj_type=_obj_type,
                 addendum=_addendum,
                 removal=removal,
             )
 
         warned = False
@@ -141,15 +144,17 @@
                 emit_warning()
             return wrapped(*args, **kwargs)
 
         if isinstance(obj, type):
             if not _obj_type:
                 _obj_type = "class"
             wrapped = obj.__init__  # type: ignore
-            _name = _name or obj.__name__
+            _name = _name or (
+                f"{obj.__module__}.{obj.__name__}" if obj.__module__ else obj.__name__
+            )
             old_doc = obj.__doc__
 
             def finalize(_: Any, new_doc: str) -> T:
                 """Finalize the deprecation of a class."""
                 try:
                     obj.__doc__ = new_doc
                 except AttributeError:  # Can't set on some extension objects.
@@ -267,14 +272,15 @@
 
 def warn_deprecated(
     since: str,
     *,
     message: str = "",
     name: str = "",
     alternative: str = "",
+    alternative_import: str = "",
     pending: bool = False,
     obj_type: str = "",
     addendum: str = "",
     removal: str = "",
 ) -> None:
     """Display a standardized deprecation.
 
@@ -303,42 +309,59 @@
             The expected removal version. With the default (an empty
             string), a removal version is automatically computed from
             since. Set to other Falsy values to not schedule a removal
             date. Cannot be used together with pending.
     """
     if pending and removal:
         raise ValueError("A pending deprecation cannot have a scheduled removal")
+    if alternative and alternative_import:
+        raise ValueError("Cannot specify both alternative and alternative_import")
+    if alternative_import and "." not in alternative_import:
+        raise ValueError("alternative_import must be a fully qualified module path")
 
     if not pending:
         if not removal:
             removal = f"in {removal}" if removal else "within ?? minor releases"
             raise NotImplementedError(
                 f"Need to determine which default deprecation schedule to use. "
                 f"{removal}"
             )
         else:
             removal = f"in {removal}"
 
     if not message:
         message = ""
+        package = name.split(".")[0].replace("_", "-") if "." in name else "LangChain"
 
         if obj_type:
             message += f"The {obj_type} `{name}`"
         else:
             message += f"`{name}`"
 
         if pending:
             message += " will be deprecated in a future version"
         else:
-            message += f" was deprecated in LangChain {since}"
+            message += f" was deprecated in {package} {since}"
 
             if removal:
                 message += f" and will be removed {removal}"
 
-        if alternative:
+        if alternative_import:
+            alt_package = alternative_import.split(".")[0].replace("_", "-")
+            if alt_package == package:
+                message += f". Use {alternative_import} instead."
+            else:
+                alt_module, alt_name = alternative_import.rsplit(".", 1)
+                message += (
+                    f". An updated version of the {obj_type} exists in the "
+                    f"{alt_package} package and should be used instead. To use it run "
+                    f"`pip install -U {alt_package}` and import as "
+                    f"`from {alt_module} import {alt_name}`."
+                )
+        elif alternative:
             message += f". Use {alternative} instead."
 
         if addendum:
             message += f" {addendum}"
 
     warning_cls = (
         LangChainPendingDeprecationWarning if pending else LangChainDeprecationWarning
```

### Comparing `langchain_core-0.1.8/langchain_core/_api/internal.py` & `langchain_core-0.1.9/langchain_core/_api/internal.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/_api/path.py` & `langchain_core-0.1.9/langchain_core/_api/path.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/agents.py` & `langchain_core-0.1.9/langchain_core/agents.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/beta/runnables/context.py` & `langchain_core-0.1.9/langchain_core/beta/runnables/context.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/caches.py` & `langchain_core-0.1.9/langchain_core/caches.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/callbacks/__init__.py` & `langchain_core-0.1.9/langchain_core/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/callbacks/base.py` & `langchain_core-0.1.9/langchain_core/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/callbacks/manager.py` & `langchain_core-0.1.9/langchain_core/callbacks/manager.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/callbacks/stdout.py` & `langchain_core-0.1.9/langchain_core/callbacks/stdout.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/callbacks/streaming_stdout.py` & `langchain_core-0.1.9/langchain_core/callbacks/streaming_stdout.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/chat_history.py` & `langchain_core-0.1.9/langchain_core/chat_history.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/documents/base.py` & `langchain_core-0.1.9/langchain_core/documents/base.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/documents/transformers.py` & `langchain_core-0.1.9/langchain_core/documents/transformers.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/embeddings.py` & `langchain_core-0.1.9/langchain_core/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/example_selectors/__init__.py` & `langchain_core-0.1.9/langchain_core/example_selectors/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/example_selectors/base.py` & `langchain_core-0.1.9/langchain_core/example_selectors/base.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/example_selectors/length_based.py` & `langchain_core-0.1.9/langchain_core/example_selectors/length_based.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/example_selectors/semantic_similarity.py` & `langchain_core-0.1.9/langchain_core/example_selectors/semantic_similarity.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/exceptions.py` & `langchain_core-0.1.9/langchain_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/globals/__init__.py` & `langchain_core-0.1.9/langchain_core/globals/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/language_models/__init__.py` & `langchain_core-0.1.9/langchain_core/language_models/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/language_models/base.py` & `langchain_core-0.1.9/langchain_core/language_models/base.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/language_models/chat_models.py` & `langchain_core-0.1.9/langchain_core/language_models/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/language_models/llms.py` & `langchain_core-0.1.9/langchain_core/language_models/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/load/dump.py` & `langchain_core-0.1.9/langchain_core/load/dump.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/load/load.py` & `langchain_core-0.1.9/langchain_core/load/load.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/load/mapping.py` & `langchain_core-0.1.9/langchain_core/load/mapping.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/load/serializable.py` & `langchain_core-0.1.9/langchain_core/load/serializable.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/memory.py` & `langchain_core-0.1.9/langchain_core/memory.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/messages/__init__.py` & `langchain_core-0.1.9/langchain_core/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/messages/ai.py` & `langchain_core-0.1.9/langchain_core/messages/ai.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/messages/base.py` & `langchain_core-0.1.9/langchain_core/messages/base.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/messages/chat.py` & `langchain_core-0.1.9/langchain_core/messages/chat.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/messages/function.py` & `langchain_core-0.1.9/langchain_core/messages/function.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/messages/human.py` & `langchain_core-0.1.9/langchain_core/messages/human.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/messages/system.py` & `langchain_core-0.1.9/langchain_core/messages/system.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/messages/tool.py` & `langchain_core-0.1.9/langchain_core/messages/tool.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/output_parsers/__init__.py` & `langchain_core-0.1.9/langchain_core/output_parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/output_parsers/base.py` & `langchain_core-0.1.9/langchain_core/output_parsers/base.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/output_parsers/format_instructions.py` & `langchain_core-0.1.9/langchain_core/output_parsers/format_instructions.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/output_parsers/json.py` & `langchain_core-0.1.9/langchain_core/output_parsers/json.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/output_parsers/list.py` & `langchain_core-0.1.9/langchain_core/output_parsers/list.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/output_parsers/string.py` & `langchain_core-0.1.9/langchain_core/output_parsers/string.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/output_parsers/transform.py` & `langchain_core-0.1.9/langchain_core/output_parsers/transform.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/output_parsers/xml.py` & `langchain_core-0.1.9/langchain_core/output_parsers/xml.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/outputs/chat_generation.py` & `langchain_core-0.1.9/langchain_core/outputs/chat_generation.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/outputs/generation.py` & `langchain_core-0.1.9/langchain_core/outputs/generation.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/outputs/llm_result.py` & `langchain_core-0.1.9/langchain_core/outputs/llm_result.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/prompt_values.py` & `langchain_core-0.1.9/langchain_core/prompt_values.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/prompts/__init__.py` & `langchain_core-0.1.9/langchain_core/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/prompts/base.py` & `langchain_core-0.1.9/langchain_core/prompts/base.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/prompts/chat.py` & `langchain_core-0.1.9/langchain_core/prompts/chat.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/prompts/few_shot.py` & `langchain_core-0.1.9/langchain_core/prompts/few_shot.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/prompts/few_shot_with_templates.py` & `langchain_core-0.1.9/langchain_core/prompts/few_shot_with_templates.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/prompts/loading.py` & `langchain_core-0.1.9/langchain_core/prompts/loading.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/prompts/pipeline.py` & `langchain_core-0.1.9/langchain_core/prompts/pipeline.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/prompts/prompt.py` & `langchain_core-0.1.9/langchain_core/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/prompts/string.py` & `langchain_core-0.1.9/langchain_core/prompts/string.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/pydantic_v1/__init__.py` & `langchain_core-0.1.9/langchain_core/pydantic_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/retrievers.py` & `langchain_core-0.1.9/langchain_core/retrievers.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/runnables/__init__.py` & `langchain_core-0.1.9/langchain_core/runnables/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/runnables/base.py` & `langchain_core-0.1.9/langchain_core/runnables/base.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/runnables/branch.py` & `langchain_core-0.1.9/langchain_core/runnables/branch.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/runnables/config.py` & `langchain_core-0.1.9/langchain_core/runnables/config.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/runnables/configurable.py` & `langchain_core-0.1.9/langchain_core/runnables/configurable.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/runnables/fallbacks.py` & `langchain_core-0.1.9/langchain_core/runnables/fallbacks.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/runnables/graph.py` & `langchain_core-0.1.9/langchain_core/runnables/graph.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/runnables/graph_draw.py` & `langchain_core-0.1.9/langchain_core/runnables/graph_draw.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/runnables/history.py` & `langchain_core-0.1.9/langchain_core/runnables/history.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/runnables/passthrough.py` & `langchain_core-0.1.9/langchain_core/runnables/passthrough.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/runnables/retry.py` & `langchain_core-0.1.9/langchain_core/runnables/retry.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/runnables/router.py` & `langchain_core-0.1.9/langchain_core/runnables/router.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/runnables/utils.py` & `langchain_core-0.1.9/langchain_core/runnables/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/stores.py` & `langchain_core-0.1.9/langchain_core/stores.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/tools.py` & `langchain_core-0.1.9/langchain_core/tools.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/tracers/__init__.py` & `langchain_core-0.1.9/langchain_core/tracers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/tracers/base.py` & `langchain_core-0.1.9/langchain_core/tracers/base.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/tracers/context.py` & `langchain_core-0.1.9/langchain_core/tracers/context.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/tracers/evaluation.py` & `langchain_core-0.1.9/langchain_core/tracers/evaluation.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/tracers/langchain.py` & `langchain_core-0.1.9/langchain_core/tracers/langchain.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/tracers/langchain_v1.py` & `langchain_core-0.1.9/langchain_core/tracers/langchain_v1.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/tracers/log_stream.py` & `langchain_core-0.1.9/langchain_core/tracers/log_stream.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/tracers/root_listeners.py` & `langchain_core-0.1.9/langchain_core/tracers/root_listeners.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/tracers/run_collector.py` & `langchain_core-0.1.9/langchain_core/tracers/run_collector.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/tracers/schemas.py` & `langchain_core-0.1.9/langchain_core/tracers/schemas.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/tracers/stdout.py` & `langchain_core-0.1.9/langchain_core/tracers/stdout.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/utils/__init__.py` & `langchain_core-0.1.9/langchain_core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/utils/aiter.py` & `langchain_core-0.1.9/langchain_core/utils/aiter.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/utils/env.py` & `langchain_core-0.1.9/langchain_core/utils/env.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/utils/formatting.py` & `langchain_core-0.1.9/langchain_core/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/utils/function_calling.py` & `langchain_core-0.1.9/langchain_core/utils/function_calling.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/utils/html.py` & `langchain_core-0.1.9/langchain_core/utils/html.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/utils/input.py` & `langchain_core-0.1.9/langchain_core/utils/input.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/utils/iter.py` & `langchain_core-0.1.9/langchain_core/utils/iter.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/utils/json_schema.py` & `langchain_core-0.1.9/langchain_core/utils/json_schema.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/utils/loading.py` & `langchain_core-0.1.9/langchain_core/utils/loading.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/utils/strings.py` & `langchain_core-0.1.9/langchain_core/utils/strings.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/utils/utils.py` & `langchain_core-0.1.9/langchain_core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/langchain_core/vectorstores.py` & `langchain_core-0.1.9/langchain_core/vectorstores.py`

 * *Files identical despite different names*

### Comparing `langchain_core-0.1.8/pyproject.toml` & `langchain_core-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-core"
-version = "0.1.8"
+version = "0.1.9"
 description = "Building applications with LLMs through composability"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
```

### Comparing `langchain_core-0.1.8/PKG-INFO` & `langchain_core-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-core
-Version: 0.1.8
+Version: 0.1.9
 Summary: Building applications with LLMs through composability
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

