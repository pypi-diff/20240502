# Comparing `tmp/eidolon_ai_sdk-0.1.42.tar.gz` & `tmp/eidolon_ai_sdk-0.1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon_ai_sdk-0.1.42.tar", max compression
+gzip compressed data, was "eidolon_ai_sdk-0.1.43.tar", max compression
```

## Comparing `eidolon_ai_sdk-0.1.42.tar` & `eidolon_ai_sdk-0.1.43.tar`

### file list

```diff
@@ -1,144 +1,144 @@
--rw-r--r--   0        0        0     2569 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/README.md
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/__init__.py
--rw-r--r--   0        0        0     2400 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/agent.py
--rw-r--r--   0        0        0     1311 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/audio_agent.py
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/__init__.py
--rw-r--r--   0        0        0     3025 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/document_manager.py
--rw-r--r--   0        0        0     2710 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/document_processor.py
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
--rw-r--r--   0        0        0      971 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
--rw-r--r--   0        0        0     3405 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
--rw-r--r--   0        0        0     4173 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
--rw-r--r--   0        0        0     2817 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
--rw-r--r--   0        0        0     4519 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
--rw-r--r--   0        0        0      448 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
--rw-r--r--   0        0        0     3699 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
--rw-r--r--   0        0        0     2053 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
--rw-r--r--   0        0        0     3212 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
--rw-r--r--   0        0        0     1647 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
--rw-r--r--   0        0        0     1328 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
--rw-r--r--   0        0        0     3356 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
--rw-r--r--   0        0        0     1400 2024-05-01 13:52:02.990563 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
--rw-r--r--   0        0        0     1398 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
--rw-r--r--   0        0        0     4786 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
--rw-r--r--   0        0        0    43465 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
--rw-r--r--   0        0        0     4825 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/generic_agent.py
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/retriever_agent/__init__.py
--rw-r--r--   0        0        0     2078 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
--rw-r--r--   0        0        0     1434 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
--rw-r--r--   0        0        0     2329 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
--rw-r--r--   0        0        0      559 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
--rw-r--r--   0        0        0     2864 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/retriever_agent/retriever.py
--rw-r--r--   0        0        0     3717 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
--rw-r--r--   0        0        0    12776 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/simple_agent.py
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/tot_agent/__init__.py
--rw-r--r--   0        0        0     1815 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/tot_agent/checker.py
--rw-r--r--   0        0        0     2468 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/tot_agent/controller.py
--rw-r--r--   0        0        0     1503 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/tot_agent/memory.py
--rw-r--r--   0        0        0     1423 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/tot_agent/prompts.py
--rw-r--r--   0        0        0      364 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/tot_agent/thought.py
--rw-r--r--   0        0        0     4951 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
--rw-r--r--   0        0        0     7614 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
--rw-r--r--   0        0        0     4572 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent_os.py
--rw-r--r--   0        0        0    12735 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent_os_interfaces.py
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/bin/__init__.py
--rwxr-xr-x   0        0        0     9444 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/bin/agent_creator.py
--rw-r--r--   0        0        0     8381 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/bin/agent_http_server.py
--rwxr-xr-x   0        0        0     3789 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/bin/replay.py
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/__init__.py
--rw-r--r--   0        0        0     9079 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/code_builtins.py
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/components/__init__.py
--rw-r--r--   0        0        0     2223 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/components/opentelemetry.py
--rw-r--r--   0        0        0     4256 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/components/usage.py
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/logic_units/__init__.py
--rw-r--r--   0        0        0     1823 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py
--rw-r--r--   0        0        0     6355 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/logic_units/web_search.py
--rw-r--r--   0        0        0      550 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
--rw-r--r--   0        0        0      601 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
--rw-r--r--   0        0        0      614 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
--rw-r--r--   0        0        0      181 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/resources/machine.yaml
--rw-r--r--   0        0        0      597 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
--rw-r--r--   0        0        0      547 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
--rw-r--r--   0        0        0      540 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
--rw-r--r--   0        0        0      595 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/resources/openai_35.yaml
--rw-r--r--   0        0        0      586 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/resources/openai_4.yaml
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/__init__.py
--rw-r--r--   0        0        0     1843 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/agent_call_history.py
--rw-r--r--   0        0        0     4638 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/agent_cpu.py
--rw-r--r--   0        0        0     2562 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/agent_io.py
--rw-r--r--   0        0        0     7916 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/agents_logic_unit.py
--rw-r--r--   0        0        0     3718 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/audio_unit.py
--rw-r--r--   0        0        0      292 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/call_context.py
--rw-r--r--   0        0        0     2833 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/conversation_memory_unit.py
--rw-r--r--   0        0        0    14295 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/conversational_apu.py
--rw-r--r--   0        0        0     4680 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/image_unit.py
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/llm/__init__.py
--rw-r--r--   0        0        0     9936 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
--rw-r--r--   0        0        0    11967 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
--rw-r--r--   0        0        0     4518 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
--rw-r--r--   0        0        0     5753 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
--rw-r--r--   0        0        0     9422 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
--rw-r--r--   0        0        0     3567 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
--rw-r--r--   0        0        0     3962 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/llm_message.py
--rw-r--r--   0        0        0     2421 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/llm_unit.py
--rw-r--r--   0        0        0     4199 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/logic_unit.py
--rw-r--r--   0        0        0     3541 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/memory_unit.py
--rw-r--r--   0        0        0      825 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/processing_unit.py
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/io/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/__init__.py
--rw-r--r--   0        0        0     1193 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/agent_memory.py
--rw-r--r--   0        0        0     5309 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/chroma_vector_store.py
--rw-r--r--   0        0        0      641 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/document.py
--rw-r--r--   0        0        0     2766 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/embeddings.py
--rw-r--r--   0        0        0      907 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/file_memory.py
--rw-r--r--   0        0        0     4203 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/file_system_vector_store.py
--rw-r--r--   0        0        0     3974 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/in_memory_file_memory.py
--rw-r--r--   0        0        0     5788 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/local_file_memory.py
--rw-r--r--   0        0        0     4845 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/local_symbolic_memory.py
--rw-r--r--   0        0        0     3793 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
--rw-r--r--   0        0        0      996 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/noop_memory.py
--rw-r--r--   0        0        0     1984 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/s3_file_memory.py
--rw-r--r--   0        0        0      974 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/semantic_memory.py
--rw-r--r--   0        0        0     2809 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/similarity_memory.py
--rw-r--r--   0        0        0     1516 2024-05-01 13:52:02.994564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/vector_store.py
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/__init__.py
--rw-r--r--   0        0        0      771 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/authentication_processor.py
--rw-r--r--   0        0        0     2159 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/azure_authorizer.py
--rw-r--r--   0        0        0     1277 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/functional_authorizer.py
--rw-r--r--   0        0        0     2001 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/google_auth.py
--rw-r--r--   0        0        0     1867 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/jwt_processor.py
--rw-r--r--   0        0        0      484 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/okta_authorizor.py
--rw-r--r--   0        0        0     1017 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/permissions.py
--rw-r--r--   0        0        0     2508 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/process_authorizer.py
--rw-r--r--   0        0        0     2977 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/security_manager.py
--rw-r--r--   0        0        0     1035 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/security_middleware.py
--rw-r--r--   0        0        0      428 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/user.py
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/__init__.py
--rw-r--r--   0        0        0     1473 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/agent_contract.py
--rw-r--r--   0        0        0    22653 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/agent_controller.py
--rw-r--r--   0        0        0    14196 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/agent_machine.py
--rw-r--r--   0        0        0     1149 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/dynamic_middleware.py
--rw-r--r--   0        0        0     3432 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/fn_handler.py
--rw-r--r--   0        0        0     4902 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/process_file_system.py
--rw-r--r--   0        0        0     4275 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/processes.py
--rw-r--r--   0        0        0     6895 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/reference_model.py
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/resources/__init__.py
--rw-r--r--   0        0        0      314 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/resources/agent_resource.py
--rw-r--r--   0        0        0      414 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/resources/machine_resource.py
--rw-r--r--   0        0        0      684 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/resources/reference_resource.py
--rw-r--r--   0        0        0     1663 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/resources/resources_base.py
--rw-r--r--   0        0        0        0 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/util/__init__.py
--rw-r--r--   0        0        0      509 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/util/async_wrapper.py
--rw-r--r--   0        0        0     2806 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/util/class_utils.py
--rw-r--r--   0        0        0     1604 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/util/image_utils.py
--rw-r--r--   0        0        0     3808 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/util/replay.py
--rw-r--r--   0        0        0     6917 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/util/schema_to_model.py
--rw-r--r--   0        0        0      898 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/util/str_utils.py
--rw-r--r--   0        0        0     3445 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/util/stream_collector.py
--rw-r--r--   0        0        0      565 2024-05-01 13:52:02.998564 eidolon_ai_sdk-0.1.42/logging.conf
--rw-r--r--   0        0        0     2204 2024-05-01 13:52:03.002564 eidolon_ai_sdk-0.1.42/pyproject.toml
--rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.42/PKG-INFO
+-rw-r--r--   0        0        0     2569 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/__init__.py
+-rw-r--r--   0        0        0     2400 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/agent.py
+-rw-r--r--   0        0        0     1311 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/audio_agent.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/__init__.py
+-rw-r--r--   0        0        0     3025 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/document_manager.py
+-rw-r--r--   0        0        0     2710 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/document_processor.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/loaders/__init__.py
+-rw-r--r--   0        0        0      971 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py
+-rw-r--r--   0        0        0     3405 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py
+-rw-r--r--   0        0        0     4173 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/__init__.py
+-rw-r--r--   0        0        0     2817 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py
+-rw-r--r--   0        0        0     4519 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/__init__.py
+-rw-r--r--   0        0        0      448 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/base_ast_generator.py
+-rw-r--r--   0        0        0     3699 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py
+-rw-r--r--   0        0        0     2053 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py
+-rw-r--r--   0        0        0     3212 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py
+-rw-r--r--   0        0        0     1647 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py
+-rw-r--r--   0        0        0     1328 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py
+-rw-r--r--   0        0        0     3356 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py
+-rw-r--r--   0        0        0     1400 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/transformer/__init__.py
+-rw-r--r--   0        0        0     1398 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py
+-rw-r--r--   0        0        0     4786 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py
+-rw-r--r--   0        0        0    43465 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py
+-rw-r--r--   0        0        0     4825 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/generic_agent.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/retriever_agent/__init__.py
+-rw-r--r--   0        0        0     2078 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py
+-rw-r--r--   0        0        0     1434 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py
+-rw-r--r--   0        0        0     2329 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py
+-rw-r--r--   0        0        0      559 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py
+-rw-r--r--   0        0        0     2864 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/retriever_agent/retriever.py
+-rw-r--r--   0        0        0     3717 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py
+-rw-r--r--   0        0        0    12776 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/simple_agent.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/tot_agent/__init__.py
+-rw-r--r--   0        0        0     1815 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/tot_agent/checker.py
+-rw-r--r--   0        0        0     2468 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/tot_agent/controller.py
+-rw-r--r--   0        0        0     1503 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/tot_agent/memory.py
+-rw-r--r--   0        0        0     1423 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/tot_agent/prompts.py
+-rw-r--r--   0        0        0      364 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/tot_agent/thought.py
+-rw-r--r--   0        0        0     4951 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/tot_agent/thought_generators.py
+-rw-r--r--   0        0        0     7614 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/tot_agent/tot_agent.py
+-rw-r--r--   0        0        0     4572 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent_os.py
+-rw-r--r--   0        0        0    12735 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent_os_interfaces.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/bin/__init__.py
+-rwxr-xr-x   0        0        0     9444 2024-05-02 00:37:33.086040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/bin/agent_creator.py
+-rw-r--r--   0        0        0     8381 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/bin/agent_http_server.py
+-rwxr-xr-x   0        0        0     3789 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/bin/replay.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/__init__.py
+-rw-r--r--   0        0        0     9079 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/code_builtins.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/components/__init__.py
+-rw-r--r--   0        0        0     2223 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/components/opentelemetry.py
+-rw-r--r--   0        0        0     4256 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/components/usage.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/logic_units/__init__.py
+-rw-r--r--   0        0        0     1823 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py
+-rw-r--r--   0        0        0     6355 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/logic_units/web_search.py
+-rw-r--r--   0        0        0      550 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml
+-rw-r--r--   0        0        0      601 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/resources/claude_opus.yaml
+-rw-r--r--   0        0        0      614 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml
+-rw-r--r--   0        0        0      181 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/resources/machine.yaml
+-rw-r--r--   0        0        0      597 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/resources/mistral_large.yaml
+-rw-r--r--   0        0        0      547 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml
+-rw-r--r--   0        0        0      540 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/resources/mistral_small.yaml
+-rw-r--r--   0        0        0      595 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/resources/openai_35.yaml
+-rw-r--r--   0        0        0      586 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/resources/openai_4.yaml
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/__init__.py
+-rw-r--r--   0        0        0     1843 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/agent_call_history.py
+-rw-r--r--   0        0        0     4638 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/agent_cpu.py
+-rw-r--r--   0        0        0     2562 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/agent_io.py
+-rw-r--r--   0        0        0     9033 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/agents_logic_unit.py
+-rw-r--r--   0        0        0     3718 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/audio_unit.py
+-rw-r--r--   0        0        0      292 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/call_context.py
+-rw-r--r--   0        0        0     2833 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/conversation_memory_unit.py
+-rw-r--r--   0        0        0    14295 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/conversational_apu.py
+-rw-r--r--   0        0        0     4680 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/image_unit.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/llm/__init__.py
+-rw-r--r--   0        0        0     9936 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py
+-rw-r--r--   0        0        0    11967 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py
+-rw-r--r--   0        0        0     4518 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py
+-rw-r--r--   0        0        0     5753 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py
+-rw-r--r--   0        0        0     9422 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py
+-rw-r--r--   0        0        0     3567 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/llm/open_ai_speech.py
+-rw-r--r--   0        0        0     3962 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/llm_message.py
+-rw-r--r--   0        0        0     2421 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/llm_unit.py
+-rw-r--r--   0        0        0     4199 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/logic_unit.py
+-rw-r--r--   0        0        0     3541 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/memory_unit.py
+-rw-r--r--   0        0        0      825 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/processing_unit.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/io/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/__init__.py
+-rw-r--r--   0        0        0     1193 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/agent_memory.py
+-rw-r--r--   0        0        0     5309 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/chroma_vector_store.py
+-rw-r--r--   0        0        0      641 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/document.py
+-rw-r--r--   0        0        0     2766 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/embeddings.py
+-rw-r--r--   0        0        0      907 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/file_memory.py
+-rw-r--r--   0        0        0     4203 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/file_system_vector_store.py
+-rw-r--r--   0        0        0     3974 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/in_memory_file_memory.py
+-rw-r--r--   0        0        0     5788 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/local_file_memory.py
+-rw-r--r--   0        0        0     4845 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/local_symbolic_memory.py
+-rw-r--r--   0        0        0     3793 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/mongo_symbolic_memory.py
+-rw-r--r--   0        0        0      996 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/noop_memory.py
+-rw-r--r--   0        0        0     1984 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/s3_file_memory.py
+-rw-r--r--   0        0        0      974 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/semantic_memory.py
+-rw-r--r--   0        0        0     2809 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/similarity_memory.py
+-rw-r--r--   0        0        0     1516 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/vector_store.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/__init__.py
+-rw-r--r--   0        0        0      771 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/authentication_processor.py
+-rw-r--r--   0        0        0     2159 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/azure_authorizer.py
+-rw-r--r--   0        0        0     1277 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/functional_authorizer.py
+-rw-r--r--   0        0        0     2001 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/google_auth.py
+-rw-r--r--   0        0        0     1867 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/jwt_processor.py
+-rw-r--r--   0        0        0      484 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/okta_authorizor.py
+-rw-r--r--   0        0        0     1017 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/permissions.py
+-rw-r--r--   0        0        0     2508 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/process_authorizer.py
+-rw-r--r--   0        0        0     2977 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/security_manager.py
+-rw-r--r--   0        0        0     1035 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/security_middleware.py
+-rw-r--r--   0        0        0      428 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/user.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/__init__.py
+-rw-r--r--   0        0        0     1473 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/agent_contract.py
+-rw-r--r--   0        0        0    22700 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/agent_controller.py
+-rw-r--r--   0        0        0    14196 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/agent_machine.py
+-rw-r--r--   0        0        0     1149 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/dynamic_middleware.py
+-rw-r--r--   0        0        0     3432 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/fn_handler.py
+-rw-r--r--   0        0        0     4911 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/process_file_system.py
+-rw-r--r--   0        0        0     4275 2024-05-02 00:37:33.090040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/processes.py
+-rw-r--r--   0        0        0     6895 2024-05-02 00:37:33.094040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/reference_model.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.094040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/resources/__init__.py
+-rw-r--r--   0        0        0      314 2024-05-02 00:37:33.094040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/resources/agent_resource.py
+-rw-r--r--   0        0        0      414 2024-05-02 00:37:33.094040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/resources/machine_resource.py
+-rw-r--r--   0        0        0      684 2024-05-02 00:37:33.094040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/resources/reference_resource.py
+-rw-r--r--   0        0        0     1663 2024-05-02 00:37:33.094040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/resources/resources_base.py
+-rw-r--r--   0        0        0        0 2024-05-02 00:37:33.094040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/util/__init__.py
+-rw-r--r--   0        0        0      509 2024-05-02 00:37:33.094040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/util/async_wrapper.py
+-rw-r--r--   0        0        0     2806 2024-05-02 00:37:33.094040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/util/class_utils.py
+-rw-r--r--   0        0        0     1604 2024-05-02 00:37:33.094040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/util/image_utils.py
+-rw-r--r--   0        0        0     3808 2024-05-02 00:37:33.094040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/util/replay.py
+-rw-r--r--   0        0        0     6917 2024-05-02 00:37:33.094040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/util/schema_to_model.py
+-rw-r--r--   0        0        0      898 2024-05-02 00:37:33.094040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/util/str_utils.py
+-rw-r--r--   0        0        0     3445 2024-05-02 00:37:33.094040 eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/util/stream_collector.py
+-rw-r--r--   0        0        0      565 2024-05-02 00:37:33.094040 eidolon_ai_sdk-0.1.43/logging.conf
+-rw-r--r--   0        0        0     2204 2024-05-02 00:37:33.094040 eidolon_ai_sdk-0.1.43/pyproject.toml
+-rw-r--r--   0        0        0     4852 1970-01-01 00:00:00.000000 eidolon_ai_sdk-0.1.43/PKG-INFO
```

### Comparing `eidolon_ai_sdk-0.1.42/README.md` & `eidolon_ai_sdk-0.1.43/README.md`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/agent.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/audio_agent.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/audio_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/document_manager.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/document_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/document_processor.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/document_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/loaders/base_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/loaders/filesystem_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/loaders/github_loader.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/auto_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/base_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/cobol.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/javascript.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/programing_language_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/code_ast_parsers/python.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/ms_word_parser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/pdf_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/parsers/text_parsers.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/transformer/auto_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/transformer/document_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/doc_manager/transformer/text_splitters.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/generic_agent.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/generic_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/retriever_agent/document_reranker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/retriever_agent/hyde_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/retriever_agent/multi_question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/retriever_agent/question_transformer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/retriever_agent/retriever.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/retriever_agent/retriever.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/retriever_agent/retriever_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/simple_agent.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/simple_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/tot_agent/checker.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/tot_agent/checker.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/tot_agent/controller.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/tot_agent/controller.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/tot_agent/memory.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/tot_agent/memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/tot_agent/prompts.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/tot_agent/prompts.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/tot_agent/thought_generators.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/tot_agent/thought_generators.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent/tot_agent/tot_agent.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent/tot_agent/tot_agent.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent_os.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent_os.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/agent_os_interfaces.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/agent_os_interfaces.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/bin/agent_creator.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/bin/agent_creator.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/bin/agent_http_server.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/bin/agent_http_server.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/bin/replay.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/bin/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/code_builtins.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/code_builtins.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/components/opentelemetry.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/components/opentelemetry.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/components/usage.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/components/usage.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/logic_units/playwrite_browser.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/logic_units/web_search.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/logic_units/web_search.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/resources/claude_haiku.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/resources/claude_opus.yaml` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/resources/claude_opus.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/resources/claude_sonnet.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/resources/mistral_large.yaml` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/resources/mistral_large.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/resources/mistral_medium.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/resources/mistral_small.yaml` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/resources/mistral_small.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/resources/openai_35.yaml` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/resources/openai_35.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/builtins/resources/openai_4.yaml` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/builtins/resources/openai_4.yaml`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/agent_call_history.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/agent_call_history.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/agent_cpu.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/agent_cpu.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/agent_io.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/agent_io.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/agents_logic_unit.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/agents_logic_unit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import copy
+from collections import defaultdict
+
 from pydantic import BaseModel
-from typing import List, Any, Dict, AsyncIterator
+from typing import List, Any, Dict, AsyncIterator, Set
 
 from eidolon_ai_client.client import Machine, Agent, AgentResponseIterator
 from eidolon_ai_sdk.cpu.agent_call_history import AgentCallHistory
 from eidolon_ai_sdk.cpu.call_context import CallContext
 from eidolon_ai_sdk.cpu.logic_unit import LogicUnit
-from eidolon_ai_client.events import StreamEvent
+from eidolon_ai_client.events import StreamEvent, ObjectOutputEvent
 from eidolon_ai_sdk.system.fn_handler import FnHandler
 from eidolon_ai_sdk.system.reference_model import Specable
 from eidolon_ai_client.util.logger import logger
 from eidolon_ai_sdk.util.schema_to_model import schema_to_model
 
 
 class AgentsLogicUnitSpec(BaseModel):
@@ -21,23 +24,27 @@
     _machine_schemas: Dict[str, dict]
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._machine_schemas = {}
 
     async def build_tools(self, call_context: CallContext) -> List[FnHandler]:
+        agent_actions = defaultdict(set)
         tools = await self.build_program_tools(call_context)
         call_history = await AgentCallHistory.get_agent_state(call_context.process_id, call_context.thread_id)
         for call in call_history:
             for action in call.available_actions:
-                context_ = await self.build_action_tool(
-                    call.machine, call.agent, action, call.remote_process_id, call_context
-                )
-                if context_:
-                    tools.append(context_)
+                agent_actions[(call.machine, call.agent, action)].add(call.remote_process_id)
+        for key, allowed_pids in agent_actions.items():
+            machine, agent, action = key
+            context_ = await self.build_action_tool(
+                machine, agent, action, allowed_pids, call_context
+            )
+            if context_:
+                tools.append(context_)
 
         return tools
 
     async def clone_thread(self, old_context: CallContext, new_context: CallContext):
         call_history = await AgentCallHistory.get_agent_state(old_context.process_id, old_context.thread_id)
         for call in call_history:
             await AgentCallHistory(
@@ -49,84 +56,94 @@
                 state=call.state,
                 available_actions=call.available_actions,
             ).upsert()
 
     async def _get_schema(self, machine: str) -> dict:
         if machine not in self._machine_schemas:
             self._machine_schemas[machine] = await Machine(machine=machine).get_schema()
-        return self._machine_schemas[machine]
+        return copy.deepcopy(self._machine_schemas[machine])
 
     async def build_action_tool(
-        self, machine: str, agent: str, action: str, remote_process_id: str, call_context: CallContext
+        self, machine: str, agent: str, action: str, allowed_pids: Set[str], call_context: CallContext
     ):
         agent_client = Agent.get(agent)
         path = f"/processes/{{process_id}}/agent/{agent}/actions/{action}"
         machine_schema = await self._get_schema(machine)
         endpoint_schema = machine_schema["paths"][path]["post"]
         try:
             name = self._name(agent, action=action)
+            description = self._description(endpoint_schema, name)
+            body_schema: dict = self._body_schema(endpoint_schema, name)
+            body_schema['properties']['conversation_id'] = {'type': 'string'}
+            if 'required' in body_schema:
+                body_schema['required'].append('conversation_id')
+            else:
+                body_schema['required'] = ['conversation_id']
             tool = self._build_tool_def(
                 agent,
                 action,
                 name,
-                endpoint_schema,
-                self._process_tool(agent_client, action, remote_process_id, call_context),
+                body_schema,
+                description,
+                self._process_tool(agent_client, action, allowed_pids, call_context),
             )
             return tool
         except ValueError:
             logger.warning(f"unable to build tool {path}", exc_info=True)
 
     async def build_program_tools(self, call_context: CallContext):
         tools = []
         for agent in self.spec.agents:
             agent_client = Agent.get(agent)
             machine_schema = await self._get_schema(agent_client.machine)
             for action in await agent_client.programs():
                 path = f"/processes/{{process_id}}/agent/{agent}/actions/{action}"
                 try:
                     name = self._name(agent, action=action)
+                    schema = machine_schema["paths"][path]["post"]
+                    description = self._description(schema, name)
                     tool = self._build_tool_def(
                         agent,
                         action,
                         name,
-                        machine_schema["paths"][path]["post"],
+                        self._body_schema(schema, name),
+                        description,
                         self._program_tool(agent_client, action, call_context),
                     )
                     tools.append(tool)
                 except ValueError:
                     logger.warning(f"unable to build tool {path}", exc_info=True)
         return tools
 
-    def _build_tool_def(self, agent, operation, name, endpoint_schema, tool_call):
-        description = self._description(endpoint_schema, name)
-        model = self._body_model(endpoint_schema, name)
+    def _build_tool_def(self, agent, operation, name, schema, description, tool_call):
+        model = schema_to_model(schema, "InputModel")
         return FnHandler(
             name=name,
             description=lambda a, b: description,
             input_model_fn=lambda a, b: model,
             output_model_fn=lambda a, b: Any,
             fn=tool_call,
             extra={
                 "title": agent,
                 "sub_title": operation,
                 "agent_call": True,
             },
         )
 
     @staticmethod
-    def _body_model(endpoint_schema, name):
+    def _body_schema(endpoint_schema, name):
         body = endpoint_schema.get("requestBody")
         if not body:
             json_schema = dict(type="object", properties={})
-            return schema_to_model(dict(type="object", properties=dict(body=json_schema)), "Input")
+            return dict(type="object", properties=dict(body=json_schema))
         elif "application/json" in body["content"]:
             json_schema = body["content"]["application/json"]["schema"]
-            return schema_to_model(dict(type="object", properties=dict(body=json_schema)), "Input")
+            return dict(type="object", properties=dict(body=json_schema))
         elif "text/plain" in body["content"]:
-            return schema_to_model(dict(type="object", properties=dict(body=dict(type="string"))), "Input")
+            return dict(type="object", properties=dict(body=dict(type="string")))
         else:
             raise ValueError(f"Agent action at {name} does not support text/plain or application/json")
 
     @staticmethod
     def _description(endpoint_schema, name):
         description = endpoint_schema.get("description", "")
         if not description:
@@ -141,28 +158,35 @@
         action = action[:15]
         action = "_" + action if action else ""
         return self.spec.tool_prefix + "_" + agent + process_id + action
 
     # todo, this needs to create history record before iterating
     def _program_tool(self, agent: Agent, program: str, call_context: CallContext):
         async def fn(_self, body):
+            process = await agent.create_process()
+            yield ObjectOutputEvent(content=dict(
+                action="created new conversation",
+                conversation_id=process.process_id,
+            ))
             async for event in RecordAgentResponseIterator(
-                (await agent.create_process()).stream_action(program, body),
+                process.stream_action(program, body),
                 call_context.process_id,
                 call_context.thread_id,
             ):
                 yield event
 
         return fn
 
     # todo, this needs to create history record before iterating
-    def _process_tool(self, agent: Agent, action: str, process_id: str, call_context: CallContext):
-        def fn(_self, body):
+    def _process_tool(self, agent: Agent, action: str, allowed_pids: Set[str], call_context: CallContext):
+        def fn(_self, conversation_id: str, body):
+            if conversation_id not in allowed_pids:
+                raise ValueError(f"Conversation id {conversation_id} not allowed for action {action}")
             return RecordAgentResponseIterator(
-                agent.process(process_id).stream_action(action, body), call_context.process_id, call_context.thread_id
+                agent.process(conversation_id).stream_action(action, body), call_context.process_id, call_context.thread_id
             )
 
         return fn
 
 
 # todo, it would be nice to work this into the client automatically
 class RecordAgentResponseIterator(AgentResponseIterator):
```

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/audio_unit.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/audio_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/conversation_memory_unit.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/conversation_memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/conversational_apu.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/conversational_apu.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/image_unit.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/image_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/llm/anthropic_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/llm/mistral_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/llm/open_ai_connection_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/llm/open_ai_image_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/llm/open_ai_llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/llm/open_ai_speech.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/llm/open_ai_speech.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/llm_message.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/llm_message.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/llm_unit.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/llm_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/logic_unit.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/logic_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/memory_unit.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/memory_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/cpu/processing_unit.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/cpu/processing_unit.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/agent_memory.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/agent_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/chroma_vector_store.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/chroma_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/document.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/document.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/embeddings.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/file_memory.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/file_system_vector_store.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/file_system_vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/in_memory_file_memory.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/in_memory_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/local_file_memory.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/local_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/local_symbolic_memory.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/local_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/mongo_symbolic_memory.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/mongo_symbolic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/noop_memory.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/noop_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/s3_file_memory.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/s3_file_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/semantic_memory.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/semantic_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/similarity_memory.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/similarity_memory.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/memory/vector_store.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/memory/vector_store.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/authentication_processor.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/authentication_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/azure_authorizer.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/azure_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/functional_authorizer.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/functional_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/google_auth.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/google_auth.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/jwt_processor.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/jwt_processor.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/permissions.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/permissions.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/process_authorizer.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/process_authorizer.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/security_manager.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/security_manager.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/security/security_middleware.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/security/security_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/agent_contract.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/agent_contract.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/agent_controller.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/agent_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import inspect
 import logging
 import typing
 import uuid
 from collections.abc import AsyncIterator
 from inspect import Parameter
 
+from bson import ObjectId
 from fastapi import FastAPI, Request, HTTPException
 from fastapi.params import Body, Param
 from pydantic import BaseModel, Field, create_model
 from pydantic_core import PydanticUndefined, to_jsonable_python
 from sse_starlette import EventSourceResponse, ServerSentEvent
 from starlette.responses import JSONResponse
 
@@ -188,15 +189,15 @@
             )
         else:
             # run the program synchronously
 
             return await self.send_response(handler, process, last_state, **kwargs)
 
     async def _create_process(self, **kwargs):
-        process = await ProcessDoc.create(agent=self.name, **kwargs)
+        process = await ProcessDoc.create(agent=self.name, **kwargs, _id=str(ObjectId()))
         if hasattr(self.agent, "create_process"):
             await self.agent.create_process(process.record_id)
         return process
 
     async def send_response(self, handler: FnHandler, process: ProcessDoc, last_state: str, **kwargs) -> JSONResponse:
         state_change_event = None
         final_event = None
```

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/agent_machine.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/agent_machine.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/dynamic_middleware.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/dynamic_middleware.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/fn_handler.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/fn_handler.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/process_file_system.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/process_file_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import asyncio
 import json
 from pathlib import Path
 from typing import Optional, Dict, Tuple
 
-import bson
+from bson import ObjectId
 from pydantic import BaseModel
 
 from eidolon_ai_client.events import FileHandle
 from eidolon_ai_sdk.agent_os import AgentOS
 from eidolon_ai_sdk.agent_os_interfaces import ProcessFileSystem
 from eidolon_ai_sdk.system.reference_model import Specable
 
@@ -57,15 +57,15 @@
         """
         Writes the given `file_contents` to a new file within the context of the process_id.
         :param file_md:
         :param process_id:
         :param file_contents:
         :return:
         """
-        file_id = str(bson.ObjectId())
+        file_id = str(ObjectId())
         await AgentOS.file_memory.mkdir(str(Path(self.root, process_id)), exist_ok=True)
         await AgentOS.file_memory.write_file(str(Path(self.root, process_id, file_id)), file_contents)
         md_to_write = {"process_id": process_id, "file_id": file_id}
         if file_md:
             md_to_write.update(file_md)
         path = str(Path(self.root, process_id, file_id + ".md"))
         await AgentOS.file_memory.write_file(path, json.dumps(md_to_write).encode())
```

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/processes.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/processes.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/reference_model.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/reference_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/resources/reference_resource.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/resources/reference_resource.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/system/resources/resources_base.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/system/resources/resources_base.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/util/class_utils.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/util/class_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/util/image_utils.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/util/image_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/util/replay.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/util/replay.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/util/schema_to_model.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/util/schema_to_model.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/util/str_utils.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/util/str_utils.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/eidolon_ai_sdk/util/stream_collector.py` & `eidolon_ai_sdk-0.1.43/eidolon_ai_sdk/util/stream_collector.py`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/logging.conf` & `eidolon_ai_sdk-0.1.43/logging.conf`

 * *Files identical despite different names*

### Comparing `eidolon_ai_sdk-0.1.42/pyproject.toml` & `eidolon_ai_sdk-0.1.43/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "eidolon-ai-sdk"
-version = "0.1.42"
+version = "0.1.43"
 description = "An Open Source Agent Services Framework"
 authors = [ "Luke Lalor <lukehlalor@gmail.com>",]
 readme = "README.md"
 include = [ "logging.conf",]
 
 [tool.ruff]
 line-length = 121
 
 [tool.eidolon]
 update-tag = "sdk"
-last-update-hash = "37df0a310654a5b99416ab24e85d37bf61e3bd28"
+last-update-hash = "401ef0add52397484c85247c2a0fd801bb1c7b85"
 
 [tool.poetry.urls]
 Github = "https://github.com/eidolon-ai/eidolon"
 Website = "https://www.eidolonai.com/"
 
 [tool.poetry.scripts]
 eidolon-server = "eidolon_ai_sdk.bin.agent_http_server:main"
```

### Comparing `eidolon_ai_sdk-0.1.42/PKG-INFO` & `eidolon_ai_sdk-0.1.43/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eidolon-ai-sdk
-Version: 0.1.42
+Version: 0.1.43
 Summary: An Open Source Agent Services Framework
 Author: Luke Lalor
 Author-email: lukehlalor@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anthropic (>=0.21.3,<0.22.0)
```

