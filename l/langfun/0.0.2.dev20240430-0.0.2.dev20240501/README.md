# Comparing `tmp/langfun-0.0.2.dev20240430.tar.gz` & `tmp/langfun-0.0.2.dev20240501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfun-0.0.2.dev20240430.tar", last modified: Tue Apr 30 08:03:45 2024, max compression
+gzip compressed data, was "langfun-0.0.2.dev20240501.tar", last modified: Wed May  1 08:04:56 2024, max compression
```

## Comparing `langfun-0.0.2.dev20240430.tar` & `langfun-0.0.2.dev20240501.tar`

### file list

```diff
@@ -1,126 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.668526 langfun-0.0.2.dev20240430/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-30 08:03:45.668526 langfun-0.0.2.dev20240430/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.648526 langfun-0.0.2.dev20240430/langfun/
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.656526 langfun-0.0.2.dev20240430/langfun/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.656526 langfun-0.0.2.dev20240430/langfun/core/coding/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.656526 langfun-0.0.2.dev20240430/langfun/core/coding/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/correction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/coding/python/permissions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/component_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.656526 langfun-0.0.2.dev20240430/langfun/core/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    68405 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/eval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    24081 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/eval/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/eval/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/eval/matching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/eval/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/eval/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11646 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/langfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/langfunc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20052 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    19548 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/language_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.660526 langfun-0.0.2.dev20240430/langfun/core/llms/
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/anthropic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.660526 langfun-0.0.2.dev20240430/langfun/core/llms/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/cache/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/cache/in_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/google_genai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/google_genai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/groq_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/llama_cpp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/llms/openai_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.660526 langfun-0.0.2.dev20240430/langfun/core/memories/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/memories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/memories/conversation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/memories/conversation_history_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/message_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.660526 langfun-0.0.2.dev20240430/langfun/core/modalities/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/modalities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/modalities/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/modalities/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/modalities/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/modalities/mime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/modalities/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/modalities/video_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/modality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/modality_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/natural_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/natural_language_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/sampling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.664526 langfun-0.0.2.dev20240430/langfun/core/structured/
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/function_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/function_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/mapping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)    20813 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/prompting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    25057 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/schema_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22360 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/structured/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/subscription_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.664526 langfun-0.0.2.dev20240430/langfun/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/templates/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/templates/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/templates/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/templates/conversation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/templates/demonstration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/templates/demonstration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/templates/selfplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/templates/selfplay_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/text_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/langfun/core/text_formatting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 08:03:45.668526 langfun-0.0.2.dev20240430/langfun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-30 08:03:45.000000 langfun-0.0.2.dev20240430/langfun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-30 08:03:45.000000 langfun-0.0.2.dev20240430/langfun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 08:03:45.000000 langfun-0.0.2.dev20240430/langfun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-30 08:03:45.000000 langfun-0.0.2.dev20240430/langfun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 08:03:45.000000 langfun-0.0.2.dev20240430/langfun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 08:03:45.668526 langfun-0.0.2.dev20240430/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-30 08:03:19.000000 langfun-0.0.2.dev20240430/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:04:56.667814 langfun-0.0.2.dev20240501/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-01 08:04:56.667814 langfun-0.0.2.dev20240501/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:04:56.647814 langfun-0.0.2.dev20240501/langfun/
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:04:56.651814 langfun-0.0.2.dev20240501/langfun/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:04:56.655814 langfun-0.0.2.dev20240501/langfun/core/coding/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:04:56.655814 langfun-0.0.2.dev20240501/langfun/core/coding/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/coding/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/coding/python/correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/coding/python/correction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/coding/python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/coding/python/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/coding/python/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/coding/python/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/coding/python/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/coding/python/generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/coding/python/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/coding/python/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/coding/python/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/coding/python/permissions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:04:56.659814 langfun-0.0.2.dev20240501/langfun/core/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73967 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/eval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/eval/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/eval/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/eval/matching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/eval/patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/eval/patching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/eval/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/eval/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11646 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/langfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/langfunc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20052 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19548 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/language_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:04:56.659814 langfun-0.0.2.dev20240501/langfun/core/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/llms/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/llms/anthropic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:04:56.659814 langfun-0.0.2.dev20240501/langfun/core/llms/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/llms/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/llms/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/llms/cache/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/llms/cache/in_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/llms/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/llms/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/llms/google_genai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/llms/google_genai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/llms/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/llms/groq_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/llms/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/llms/llama_cpp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/llms/openai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:04:56.663814 langfun-0.0.2.dev20240501/langfun/core/memories/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/memories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/memories/conversation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/memories/conversation_history_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/message_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:04:56.663814 langfun-0.0.2.dev20240501/langfun/core/modalities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/modalities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/modalities/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/modalities/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/modalities/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/modalities/mime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/modalities/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/modalities/video_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/modality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/modality_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/natural_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/natural_language_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/sampling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:04:56.667814 langfun-0.0.2.dev20240501/langfun/core/structured/
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/structured/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/structured/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/structured/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/structured/description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/structured/function_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/structured/function_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12112 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/structured/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/structured/mapping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/structured/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/structured/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/structured/prompting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20813 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/structured/prompting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25057 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/structured/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/structured/schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/structured/schema_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22360 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/structured/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/structured/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/structured/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/subscription_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:04:56.667814 langfun-0.0.2.dev20240501/langfun/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/templates/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/templates/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/templates/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/templates/conversation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/templates/demonstration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/templates/demonstration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/templates/selfplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/templates/selfplay_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/text_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/langfun/core/text_formatting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:04:56.667814 langfun-0.0.2.dev20240501/langfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-01 08:04:56.000000 langfun-0.0.2.dev20240501/langfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-01 08:04:56.000000 langfun-0.0.2.dev20240501/langfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 08:04:56.000000 langfun-0.0.2.dev20240501/langfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-01 08:04:56.000000 langfun-0.0.2.dev20240501/langfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 08:04:56.000000 langfun-0.0.2.dev20240501/langfun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 08:04:56.667814 langfun-0.0.2.dev20240501/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-01 08:04:32.000000 langfun-0.0.2.dev20240501/setup.py
```

### Comparing `langfun-0.0.2.dev20240430/LICENSE` & `langfun-0.0.2.dev20240501/LICENSE`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/PKG-INFO` & `langfun-0.0.2.dev20240501/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240430
+Version: 0.0.2.dev20240501
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
@@ -17,15 +17,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: absl-py>=1.0.0
 Requires-Dist: google-generativeai>=0.3.2
 Requires-Dist: jinja2>=3.1.2
 Requires-Dist: openai==0.27.2
 Requires-Dist: pyglove>=0.4.5.dev20240423
 Requires-Dist: python-magic>=0.4.27
 Requires-Dist: requests>=2.31.0
 Requires-Dist: termcolor==1.1.0
```

### Comparing `langfun-0.0.2.dev20240430/README.md` & `langfun-0.0.2.dev20240501/README.md`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/__init__.py` & `langfun-0.0.2.dev20240501/langfun/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/__init__.py` & `langfun-0.0.2.dev20240501/langfun/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/coding/__init__.py` & `langfun-0.0.2.dev20240501/langfun/core/coding/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/coding/python/__init__.py` & `langfun-0.0.2.dev20240501/langfun/core/coding/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/coding/python/correction.py` & `langfun-0.0.2.dev20240501/langfun/core/coding/python/correction.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/coding/python/correction_test.py` & `langfun-0.0.2.dev20240501/langfun/core/coding/python/correction_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/coding/python/errors.py` & `langfun-0.0.2.dev20240501/langfun/core/coding/python/errors.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/coding/python/errors_test.py` & `langfun-0.0.2.dev20240501/langfun/core/coding/python/errors_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/coding/python/execution.py` & `langfun-0.0.2.dev20240501/langfun/core/coding/python/execution.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/coding/python/execution_test.py` & `langfun-0.0.2.dev20240501/langfun/core/coding/python/execution_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/coding/python/generation.py` & `langfun-0.0.2.dev20240501/langfun/core/coding/python/generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/coding/python/generation_test.py` & `langfun-0.0.2.dev20240501/langfun/core/coding/python/generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/coding/python/parsing.py` & `langfun-0.0.2.dev20240501/langfun/core/coding/python/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/coding/python/parsing_test.py` & `langfun-0.0.2.dev20240501/langfun/core/coding/python/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/coding/python/permissions.py` & `langfun-0.0.2.dev20240501/langfun/core/coding/python/permissions.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/coding/python/permissions_test.py` & `langfun-0.0.2.dev20240501/langfun/core/coding/python/permissions_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/component.py` & `langfun-0.0.2.dev20240501/langfun/core/component.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/component_test.py` & `langfun-0.0.2.dev20240501/langfun/core/component_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/concurrent.py` & `langfun-0.0.2.dev20240501/langfun/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/concurrent_test.py` & `langfun-0.0.2.dev20240501/langfun/core/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/console.py` & `langfun-0.0.2.dev20240501/langfun/core/console.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/console_test.py` & `langfun-0.0.2.dev20240501/langfun/core/console_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/eval/__init__.py` & `langfun-0.0.2.dev20240501/langfun/core/eval/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,15 +12,19 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """langfun eval framework."""
 
 # pylint: disable=g-importing-member
 # pylint: disable=g-bad-import-order
 
-from langfun.core.eval.base import app_run
+from langfun.core.eval.base import register
+from langfun.core.eval.base import registered_names
+from langfun.core.eval.base import get_evaluation
+from langfun.core.eval.base import get
+from langfun.core.eval.base import run
 
 from langfun.core.eval.base import Evaluable
 from langfun.core.eval.base import Evaluation
 from langfun.core.eval.base import Suite
 from langfun.core.eval.base import Summary
 
 from langfun.core.eval.base import load
@@ -30,10 +34,19 @@
 # Functors for loading inputs.
 from langfun.core.eval.base import inputs_from
 from langfun.core.eval.base import as_inputs
 
 from langfun.core.eval.matching import Matching
 from langfun.core.eval.scoring import Scoring
 
+# Experiment patching.
+from langfun.core.eval.patching import patch_member
 
+from langfun.core.eval.patching import patch_lm
+from langfun.core.eval.patching import patch_parsing_lm
+from langfun.core.eval.patching import patch_inputs
+from langfun.core.eval.patching import patch_prompt
+from langfun.core.eval.patching import patch_schema_fn
+
+# Placeholder for Google-internal imports.
 # pylint: enable=g-bad-import-order
 # pylint: enable=g-importing-member
```

### Comparing `langfun-0.0.2.dev20240430/langfun/core/eval/base.py` & `langfun-0.0.2.dev20240501/langfun/core/eval/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,18 +21,17 @@
 import html
 import inspect
 import io
 import os
 import re
 import threading
 import time
+import types
 from typing import Annotated, Any, Callable, Iterator, Literal, Optional, Sequence, Type, Union
 
-from absl import app
-from absl import flags
 import langfun.core as lf
 import langfun.core.coding as lf_coding
 from langfun.core.llms.cache import in_memory
 import langfun.core.structured as lf_structured
 import pyglove as pg
 
 
@@ -596,15 +595,14 @@
   enabled: bool = True
   progress_bar: int | None = None
 
 
 @pg.use_init_args(['children'])
 class Suite(Evaluable):
   """Evaluation suite."""
-
   children: Annotated[list[Evaluable], 'Child evaluation sets or suites.']
 
   # Use empty ID as suite is just a container of child evaluations.
   id: str = ''
 
   __kwargs__: Annotated[
       Any,
@@ -2142,45 +2140,195 @@
       pivot_field=pivot_field,
       expect_new_dirs=expect_new_dirs,
       scan_interval=scan_interval,
       refresh_when_stop=refresh_when_stop,
   )
 
 
-def app_run(target: Evaluable):
-  """Runs the target evaluation as an absl app.
+#
+# Named evaluations and experiments support.
+#
 
-  Args:
-    target: An Langfun evaluable object.
-  """
-  flags.DEFINE_string(
-      'root_dir', None, 'Root directory for running the evaluation.'
-  )
 
-  flags.DEFINE_bool(
-      'dryrun', False, 'If True, dryrun the experiment instead of running it.'
-  )
+class _NamedEvaluationRegistry:
+  """Named evaluation registry."""
 
-  flags.DEFINE_bool(
-      'debug', False, 'If True, output prompt and response to the console.'
-  )
+  def __init__(self):
+    self._registry = {}
+
+  def names(self) -> list[str]:
+    """Returns all registered names."""
+    return sorted(self._registry.keys())
+
+  def get(self, name: str) -> Type[Evaluable]:
+    """Gets an evaluation by name."""
+    if name not in self._registry:
+      raise ValueError(
+          f'Evaluation {name!r} not found. '
+          'Did you forget to import the module that registers it?'
+      )
+    return self._registry[name]
+
+  def register(
+      self,
+      name: str,
+      experiment_cls: Type[Evaluable],
+  ):
+    """Register an experiment class."""
+    self._registry[name] = experiment_cls
+
+
+_eval_registry = _NamedEvaluationRegistry()
+
+
+def registered_names() -> list[str]:
+  """Returns all registered names."""
+  return _eval_registry.names()
+
+
+def get_evaluation(evaluation: str | Evaluable) -> Evaluable:
+  """Gets an evaluation experiment by name."""
+  if isinstance(evaluation, str):
+    return _eval_registry.get(evaluation)()
+  return evaluation
 
-  flags.DEFINE_bool(
-      'rerun',
-      False,
-      'If True, rerun the experiment even a cached result is found.',
-  )
 
-  FLAGS = flags.FLAGS  # pylint: disable=invalid-name
+def register(name: str):
+  """Decorator to create a named evaluation class."""
 
-  def _main(argv):
-    if len(argv) > 1:
-      raise app.UsageError('Too many command-line arguments.')
-
-    if FLAGS.root_dir:
-      target.rebind(root_dir=FLAGS.root_dir, raise_on_no_change=False)
-    if FLAGS.dryrun:
-      target.dryrun(debug=FLAGS.debug)
+  def _register(func_or_cls: Type[Evaluation] | types.FunctionType):
+    if inspect.isfunction(func_or_cls):
+      e = func_or_cls()
+      if not isinstance(e, Evaluable):
+        raise TypeError(
+            f'The return value of `{func_or_cls}` should be an instance of '
+            '`lf.eval.Evaluable` subclass.'
+        )
+
+      class GeneratedSuite(Suite):
+        # NOTE(daiyip): Delay serialization key registration for generated
+        # class.
+        auto_register = False
+        children = e.children if isinstance(e, Suite) else [e]
+
+      cls = GeneratedSuite
+      cls.__name__ = func_or_cls.__name__
+      cls.__doc__ = func_or_cls.__doc__
+      cls.__qualname__ = func_or_cls.__qualname__
+      cls.__module__ = getattr(func_or_cls, '__module__', 'wrapper')
+      cls.register_for_deserialization(cls.__type_name__)
+
+    elif issubclass(func_or_cls, Evaluable):
+      cls = func_or_cls
     else:
-      target.run(debug=FLAGS.debug, rerun=FLAGS.rerun)
+      raise ValueError(f'Unsupported type: {type(func_or_cls)}')
+
+    _eval_registry.register(name, cls)
+    return cls
+
+  return _register
+
+
+def get(
+    root_dir: str,
+    evaluations: list[str | Evaluable],
+    filter: Union[                    # pylint: disable=redefined-builtin
+        str,                          # Regex to filter evaluation based on ID.
+        Callable[[Evaluable], bool],  # Custom filter function.
+        None                          # No filtering (Default).
+    ] = None,                         # pylint: disable=bad-whitespace
+    patches: list[Union[
+        str,                                    # String-based PyGlove patcher.
+        pg.patching.Patcher,                    # PyGlove patcher object.
+        Callable[[pg.KeyPath, Any, Any], Any],  # PyGlove rebind function.
+    ]] | None = None,                           # pylint: disable=bad-whitespace
+) -> Suite:
+  """Gets a suite from a list of patched evaluations.
+
+  Args:
+    root_dir: The root directory of the experiment.
+    evaluations: A list of evaluations to be included in the suite.
+    filter: A regular expression (str) for selecting sub-experiments of matched
+      IDs, or a filter function to filter the evaluations.
+    patches: A list of patches to be applied to the suite. Each element can be
+      a string (for string-based patcher), a `pg.patching.Patcher` object, or
+      a rebind function (e.g. `pg.rebind`). See `lf.eval.patch_*` for more
+      details.
+
+  Returns:
+    A suite of selected `lf.eval.Evaluation` objects.
+  """
+  evaluations = [get_evaluation(e) for e in evaluations]
+  suite = Suite(evaluations, root_dir=root_dir)
+  if patches:
+    suite = pg.patch(suite, patches)
+
+  if isinstance(filter, str):
+    regex = re.compile(filter)
+    filter = lambda x: bool(regex.match(x.id))
+
+  if filter:
+    suite = Suite(
+        [leaf for leaf in suite.leaf_nodes if filter(leaf)], root_dir=root_dir)
+  return suite
+
+
+def run(
+    root_dir: str,
+    evaluations: list[str | Evaluable],
+    filter: Union[                    # pylint: disable=redefined-builtin
+        str,                          # Regex to filter evaluation based on ID.
+        Callable[[Evaluable], bool],  # Custom filter function.
+        None                          # No filtering (Default).
+    ] = None,                         # pylint: disable=bad-whitespace
+    patches: list[Union[
+        str,                                    # String-based PyGlove patcher.
+        pg.patching.Patcher,                    # PyGlove patcher object.
+        Callable[[pg.KeyPath, Any, Any], Any],  # PyGlove rebind function.
+    ]] | None = None,                           # pylint: disable=bad-whitespace
+    mode: Literal['run', 'rerun', 'dryrun', 'noop'] = 'run',
+    debug: bool = False,
+    print_definition: bool = False,
+    **kwargs,
+) -> Suite:
+  """Run selected evaluations with patching.
+
+  Args:
+    root_dir: The root directory of the experiment.
+    evaluations: A list of evaluations to be included in the suite.
+    filter: A regular expression (str) for selecting sub-experiments of matched
+      IDs, or a filter function to filter the evaluations.
+    patches: A list of patches to be applied to the suite. Each element can be
+      a string (for string-based patcher), a `pg.patching.Patcher` object, or
+      a rebind function (e.g. `pg.rebind`). See `lf.eval.patch_*` for more
+      details.
+    mode: The mode to run the suite. "run" to run the suite, with reusing
+      existing results if available; "rerun" to rerun all evaluations even if
+      there are existing results; "dryrun" to dryrun the suite; and "noop"
+      to do nothing.
+    debug: Whether to run in debug mode.
+    print_definition: Whether to print the experiment definition.
+    **kwargs: Additional arguments to be passed to dryrun/run the suite.
+
+  Returns:
+    A suite of selected `lf.eval.Evaluation` objects.
+  """
+  suite = get(root_dir, evaluations, patches=patches, filter=filter)
+  if print_definition:
+    lf.console.write(
+        pg.format(
+            suite,
+            compact=False,
+            verbose=False,
+            hide_default_values=True,
+            python_format=True,
+        ),
+        title='[EXPERIMENT DEFINITION]',
+        color='blue',
+    )
 
-  app.run(_main)
+  if mode == 'run':
+    rerun = mode == 'rerun'
+    suite.run(debug=debug, rerun=rerun, **kwargs)
+  elif mode == 'dryrun':
+    suite.dryrun(debug=debug, **kwargs)
+  return suite
```

### Comparing `langfun-0.0.2.dev20240430/langfun/core/eval/base_test.py` & `langfun-0.0.2.dev20240501/langfun/core/eval/base_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -745,21 +745,102 @@
     r = base.monitor_async(root_dir, summary_file, expect_new_dirs=True)
     self._eval_set(root_dir).run(summary=False)
     summary = r.stop()
     self.assertTrue(all(e.result for e in summary.evaluations))
     self.assertTrue(pg.io.path_exists(summary_file))
 
 
-class AppRunTest(unittest.TestCase):
+class NamedEvaluationTest(unittest.TestCase):
 
-  def test_app_run(self):
-    lm = fake.StaticSequence(['two', 'Solution(final_answer=2)'])
-    try:
-      base.app_run(
-          eval_set('app_run_test', 'query', schema_fn=answer_schema(), lm=lm)
+  def test_named_eval_class(self):
+
+    @base.register('named_eval/class_test')
+    class MyEval(base.Evaluation):
+      inputs = base.as_inputs([
+          pg.Dict(question='Compute 1 + 1'),
+      ])
+      method = 'query'
+      prompt = pg.oneof([
+          lf.Template('{{example.question}}'),
+          lf.Template('Hello {{example.question}}'),
+      ])
+      schema_fn = answer_schema()
+
+    evaluation = base.get_evaluation('named_eval/class_test')
+    self.assertIsInstance(evaluation, MyEval)
+    self.assertIsNone(evaluation.dir)
+    self.assertIsNone(evaluation.root_dir)
+    self.assertIn('named_eval/class_test', base.registered_names())
+
+    with self.assertRaisesRegex(ValueError, 'Unsupported type.*'):
+      @base.register('named_eval/bad_class')
+      class Foo:  # pylint: disable=unused-variable
+        pass
+
+  def test_named_eval_functor(self):
+
+    @base.register('named_eval/functor_test')
+    def my_eval():
+      return base.Evaluation(
+          inputs=base.as_inputs([
+              pg.Dict(question='Compute 1 + 1'),
+          ]),
+          method='query',
+          prompt=pg.oneof([
+              lf.Template('{{example.question}}'),
+              lf.Template('Hello {{example.question}}'),
+          ]),
+          schema_fn=answer_schema(),
       )
-    except SystemExit:
-      pass
+
+    self.assertTrue(issubclass(my_eval, base.Evaluable))
+    evaluation = base.get_evaluation('named_eval/functor_test')
+    self.assertIn('named_eval/functor_test', base.registered_names())
+    self.assertIsInstance(evaluation, my_eval)
+    self.assertIsNone(evaluation.root_dir, None)
+
+    with self.assertRaisesRegex(ValueError, 'Evaluation .* not found'):
+      base.get_evaluation('named_eval/non_existent')
+
+    with self.assertRaisesRegex(TypeError, 'The return value .*'):
+      @base.register('named_eval/bad_return_type')
+      def bad_eval():   # pylint: disable=unused-variable
+        return 1
+
+  def test_run(self):
+    @base.register('test/run')
+    def test_run():  # pylint: disable=unused-variable
+      lm = fake.StaticResponse('Solution(final_answer=2)')
+      return eval_set('run_test', 'query', schema_fn=answer_schema(), lm=lm)
+
+    e = base.run(
+        tempfile.gettempdir(),
+        ['test/run'],
+        id_regex='run_test.*',
+        mode='dryrun',
+        print_definition=True,
+    )
+    self.assertEqual(
+        e.leaf_nodes[0].dir,
+        os.path.join(tempfile.gettempdir(), e.leaf_nodes[0].id),
+    )
+    self.assertTrue(
+        pg.eq(
+            e.leaf_nodes[0].lm, fake.StaticResponse('Solution(final_answer=2)')
+        )
+    )
+
+    @pg.patcher()
+    def bad_lm(unused_eval):  # pylint: disable=unused-variable
+      return dict(lm=fake.StaticResponse('efg'))
+
+    e = base.run(
+        tempfile.gettempdir(),
+        [test_run()],
+        filter='Evaluation.*',
+        patches=['bad_lm']
+    )
+    self.assertTrue(pg.eq(e.leaf_nodes[0].lm, fake.StaticResponse('efg')))
 
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `langfun-0.0.2.dev20240430/langfun/core/eval/matching.py` & `langfun-0.0.2.dev20240501/langfun/core/eval/matching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/eval/matching_test.py` & `langfun-0.0.2.dev20240501/langfun/core/eval/matching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/eval/scoring.py` & `langfun-0.0.2.dev20240501/langfun/core/eval/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/eval/scoring_test.py` & `langfun-0.0.2.dev20240501/langfun/core/eval/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/langfunc.py` & `langfun-0.0.2.dev20240501/langfun/core/langfunc.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/langfunc_test.py` & `langfun-0.0.2.dev20240501/langfun/core/langfunc_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/language_model.py` & `langfun-0.0.2.dev20240501/langfun/core/language_model.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/language_model_test.py` & `langfun-0.0.2.dev20240501/langfun/core/language_model_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/llms/__init__.py` & `langfun-0.0.2.dev20240501/langfun/core/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/llms/anthropic.py` & `langfun-0.0.2.dev20240501/langfun/core/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/llms/anthropic_test.py` & `langfun-0.0.2.dev20240501/langfun/core/llms/anthropic_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/llms/cache/__init__.py` & `langfun-0.0.2.dev20240501/langfun/core/llms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/llms/cache/base.py` & `langfun-0.0.2.dev20240501/langfun/core/llms/cache/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/llms/cache/in_memory.py` & `langfun-0.0.2.dev20240501/langfun/core/llms/cache/in_memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/llms/cache/in_memory_test.py` & `langfun-0.0.2.dev20240501/langfun/core/llms/cache/in_memory_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/llms/fake.py` & `langfun-0.0.2.dev20240501/langfun/core/llms/fake.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/llms/fake_test.py` & `langfun-0.0.2.dev20240501/langfun/core/llms/fake_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/llms/google_genai.py` & `langfun-0.0.2.dev20240501/langfun/core/llms/google_genai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/llms/google_genai_test.py` & `langfun-0.0.2.dev20240501/langfun/core/llms/google_genai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/llms/groq.py` & `langfun-0.0.2.dev20240501/langfun/core/llms/groq.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/llms/groq_test.py` & `langfun-0.0.2.dev20240501/langfun/core/llms/groq_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/llms/llama_cpp.py` & `langfun-0.0.2.dev20240501/langfun/core/llms/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/llms/llama_cpp_test.py` & `langfun-0.0.2.dev20240501/langfun/core/llms/llama_cpp_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/llms/openai.py` & `langfun-0.0.2.dev20240501/langfun/core/llms/openai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/llms/openai_test.py` & `langfun-0.0.2.dev20240501/langfun/core/llms/openai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/memories/__init__.py` & `langfun-0.0.2.dev20240501/langfun/core/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/memories/conversation_history.py` & `langfun-0.0.2.dev20240501/langfun/core/memories/conversation_history.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/memories/conversation_history_test.py` & `langfun-0.0.2.dev20240501/langfun/core/memories/conversation_history_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/memory.py` & `langfun-0.0.2.dev20240501/langfun/core/memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/message.py` & `langfun-0.0.2.dev20240501/langfun/core/message.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/message_test.py` & `langfun-0.0.2.dev20240501/langfun/core/message_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/modalities/__init__.py` & `langfun-0.0.2.dev20240501/langfun/core/modalities/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/modalities/image.py` & `langfun-0.0.2.dev20240501/langfun/core/modalities/image.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/modalities/image_test.py` & `langfun-0.0.2.dev20240501/langfun/core/modalities/image_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/modalities/mime.py` & `langfun-0.0.2.dev20240501/langfun/core/modalities/mime.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/modalities/mime_test.py` & `langfun-0.0.2.dev20240501/langfun/core/modalities/mime_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/modalities/video.py` & `langfun-0.0.2.dev20240501/langfun/core/modalities/video.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/modalities/video_test.py` & `langfun-0.0.2.dev20240501/langfun/core/modalities/video_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/modality.py` & `langfun-0.0.2.dev20240501/langfun/core/modality.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/modality_test.py` & `langfun-0.0.2.dev20240501/langfun/core/modality_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/natural_language.py` & `langfun-0.0.2.dev20240501/langfun/core/natural_language.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/natural_language_test.py` & `langfun-0.0.2.dev20240501/langfun/core/natural_language_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/sampling.py` & `langfun-0.0.2.dev20240501/langfun/core/sampling.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/sampling_test.py` & `langfun-0.0.2.dev20240501/langfun/core/sampling_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/structured/__init__.py` & `langfun-0.0.2.dev20240501/langfun/core/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/structured/completion.py` & `langfun-0.0.2.dev20240501/langfun/core/structured/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/structured/completion_test.py` & `langfun-0.0.2.dev20240501/langfun/core/structured/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/structured/description.py` & `langfun-0.0.2.dev20240501/langfun/core/structured/description.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/structured/description_test.py` & `langfun-0.0.2.dev20240501/langfun/core/structured/description_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/structured/function_generation.py` & `langfun-0.0.2.dev20240501/langfun/core/structured/function_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/structured/function_generation_test.py` & `langfun-0.0.2.dev20240501/langfun/core/structured/function_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/structured/mapping.py` & `langfun-0.0.2.dev20240501/langfun/core/structured/mapping.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/structured/mapping_test.py` & `langfun-0.0.2.dev20240501/langfun/core/structured/mapping_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/structured/parsing.py` & `langfun-0.0.2.dev20240501/langfun/core/structured/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/structured/parsing_test.py` & `langfun-0.0.2.dev20240501/langfun/core/structured/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/structured/prompting.py` & `langfun-0.0.2.dev20240501/langfun/core/structured/prompting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/structured/prompting_test.py` & `langfun-0.0.2.dev20240501/langfun/core/structured/prompting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/structured/schema.py` & `langfun-0.0.2.dev20240501/langfun/core/structured/schema.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/structured/schema_generation.py` & `langfun-0.0.2.dev20240501/langfun/core/structured/schema_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/structured/schema_generation_test.py` & `langfun-0.0.2.dev20240501/langfun/core/structured/schema_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/structured/schema_test.py` & `langfun-0.0.2.dev20240501/langfun/core/structured/schema_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/structured/scoring.py` & `langfun-0.0.2.dev20240501/langfun/core/structured/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/structured/scoring_test.py` & `langfun-0.0.2.dev20240501/langfun/core/structured/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/subscription.py` & `langfun-0.0.2.dev20240501/langfun/core/subscription.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/subscription_test.py` & `langfun-0.0.2.dev20240501/langfun/core/subscription_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/template.py` & `langfun-0.0.2.dev20240501/langfun/core/template.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/template_test.py` & `langfun-0.0.2.dev20240501/langfun/core/template_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/templates/__init__.py` & `langfun-0.0.2.dev20240501/langfun/core/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/templates/completion.py` & `langfun-0.0.2.dev20240501/langfun/core/templates/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/templates/completion_test.py` & `langfun-0.0.2.dev20240501/langfun/core/templates/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/templates/conversation.py` & `langfun-0.0.2.dev20240501/langfun/core/templates/conversation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/templates/conversation_test.py` & `langfun-0.0.2.dev20240501/langfun/core/templates/conversation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/templates/demonstration.py` & `langfun-0.0.2.dev20240501/langfun/core/templates/demonstration.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/templates/demonstration_test.py` & `langfun-0.0.2.dev20240501/langfun/core/templates/demonstration_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/templates/selfplay.py` & `langfun-0.0.2.dev20240501/langfun/core/templates/selfplay.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/templates/selfplay_test.py` & `langfun-0.0.2.dev20240501/langfun/core/templates/selfplay_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/text_formatting.py` & `langfun-0.0.2.dev20240501/langfun/core/text_formatting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun/core/text_formatting_test.py` & `langfun-0.0.2.dev20240501/langfun/core/text_formatting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240430/langfun.egg-info/PKG-INFO` & `langfun-0.0.2.dev20240501/langfun.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240430
+Version: 0.0.2.dev20240501
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
@@ -17,15 +17,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: absl-py>=1.0.0
 Requires-Dist: google-generativeai>=0.3.2
 Requires-Dist: jinja2>=3.1.2
 Requires-Dist: openai==0.27.2
 Requires-Dist: pyglove>=0.4.5.dev20240423
 Requires-Dist: python-magic>=0.4.27
 Requires-Dist: requests>=2.31.0
 Requires-Dist: termcolor==1.1.0
```

### Comparing `langfun-0.0.2.dev20240430/langfun.egg-info/SOURCES.txt` & `langfun-0.0.2.dev20240501/langfun.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
 langfun/core/coding/python/permissions.py
 langfun/core/coding/python/permissions_test.py
 langfun/core/eval/__init__.py
 langfun/core/eval/base.py
 langfun/core/eval/base_test.py
 langfun/core/eval/matching.py
 langfun/core/eval/matching_test.py
+langfun/core/eval/patching.py
+langfun/core/eval/patching_test.py
 langfun/core/eval/scoring.py
 langfun/core/eval/scoring_test.py
 langfun/core/llms/__init__.py
 langfun/core/llms/anthropic.py
 langfun/core/llms/anthropic_test.py
 langfun/core/llms/fake.py
 langfun/core/llms/fake_test.py
```

### Comparing `langfun-0.0.2.dev20240430/setup.py` & `langfun-0.0.2.dev20240501/setup.py`

 * *Files identical despite different names*

