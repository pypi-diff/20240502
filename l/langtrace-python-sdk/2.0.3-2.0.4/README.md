# Comparing `tmp/langtrace_python_sdk-2.0.3.tar.gz` & `tmp/langtrace_python_sdk-2.0.4.tar.gz`

## Comparing `langtrace_python_sdk-2.0.3.tar` & `langtrace_python_sdk-2.0.4.tar`

### file list

```diff
@@ -1,130 +1,130 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/__init__.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/run_example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/anthropic_example/__init__.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/anthropic_example/completion.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/chroma_example/__init__.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/chroma_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/cohere_example/__init__.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/cohere_example/chat.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/cohere_example/chat_stream.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/cohere_example/embed.py
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/cohere_example/rerank.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/cohere_example/tools.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/fastapi_example/basic_route.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/hiveagent_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/langchain_example/__init__.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/langchain_example/basic.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/langchain_example/groq_example.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/langchain_example/langgraph_example.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/langchain_example/tool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/llamaindex_example/__init__.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/llamaindex_example/agent.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/llamaindex_example/basic.py
--rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/llamaindex_example/data/abramov.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/openai_example/__init__.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/openai_example/async_tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/openai_example/async_tool_calling_streaming.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/openai_example/chat_completion.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/openai_example/embeddings_create.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/openai_example/function_calling.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/openai_example/images_generate.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/openai_example/tool_calling.py
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/openai_example/tool_calling_nonstreaming.py
--rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/openai_example/tool_calling_streaming.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/perplexity_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/pinecone_example/__init__.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/pinecone_example/basic.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/qdrant_example/__init__.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/examples/qdrant_example/basic.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/__init__.py
--rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/langtrace.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/constants/__init__.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/constants/instrumentation/__init__.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/constants/instrumentation/chroma.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/constants/instrumentation/cohere.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/constants/instrumentation/common.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/constants/instrumentation/groq.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/constants/instrumentation/openai.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/constants/instrumentation/qdrant.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/extensions/__init__.py
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/extensions/langtrace_exporter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
--rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/chroma/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
--rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/cohere/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/groq/__init__.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py
--rw-r--r--   0        0        0    25572 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/groq/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
--rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/langchain/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
--rw-r--r--   0        0        0     5198 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
--rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
--rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/langgraph/__init__.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py
--rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/langgraph/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
--rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
--rw-r--r--   0        0        0    36773 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/openai/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/qdrant/__init__.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/qdrant/patch.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/utils/__init__.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/utils/llm.py
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/utils/with_root_span.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/__init__.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/conftest.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/utils.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/anthropic/conftest.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/anthropic/test_anthropic.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/anthropic/cassettes/test_anthropic.yaml
--rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/chroma/test_chroma.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/cohere/conftest.py
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/cohere/test_cohere_chat.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/cohere/test_cohere_embed.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/cohere/test_cohere_rerank.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/cohere/cassettes/test_cohere_chat.yaml
--rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml
--rw-r--r--   0        0        0    27312 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/cohere/cassettes/test_cohere_embed.yaml
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/cohere/cassettes/test_cohere_rerank.yaml
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/langchain/test_langchain.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/langchain/test_langchain_community.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/langchain/test_langchain_core.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/openai/conftest.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/openai/test_chat_completion.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/openai/test_embeddings.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/openai/test_image_generation.py
--rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/openai/cassettes/test_async_image_generation.yaml
--rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/openai/cassettes/test_chat_completion.yaml
--rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/openai/cassettes/test_image_generation.yaml
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/src/tests/pinecone/test_pinecone.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/LICENSE
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/README.md
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/__init__.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/run_example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/anthropic_example/__init__.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/anthropic_example/completion.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/chroma_example/__init__.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/chroma_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/cohere_example/__init__.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/cohere_example/chat.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/cohere_example/chat_stream.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/cohere_example/embed.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/cohere_example/rerank.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/cohere_example/tools.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/fastapi_example/basic_route.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/hiveagent_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/langchain_example/__init__.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/langchain_example/basic.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/langchain_example/groq_example.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/langchain_example/langgraph_example.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/langchain_example/tool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/llamaindex_example/__init__.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/llamaindex_example/agent.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/llamaindex_example/basic.py
+-rw-r--r--   0        0        0    32667 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/llamaindex_example/data/abramov.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/openai_example/__init__.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/openai_example/async_tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/openai_example/async_tool_calling_streaming.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/openai_example/chat_completion.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/openai_example/embeddings_create.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/openai_example/function_calling.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/openai_example/images_generate.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/openai_example/tool_calling.py
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/openai_example/tool_calling_nonstreaming.py
+-rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/openai_example/tool_calling_streaming.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/perplexity_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/pinecone_example/__init__.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/pinecone_example/basic.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/qdrant_example/__init__.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/examples/qdrant_example/basic.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/__init__.py
+-rw-r--r--   0        0        0     4762 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/langtrace.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/__init__.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/exporter/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/__init__.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/anthropic.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/chroma.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/cohere.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/common.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/groq.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/openai.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/pinecone.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/qdrant.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/extensions/__init__.py
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/extensions/langtrace_exporter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/anthropic/__init__.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py
+-rw-r--r--   0        0        0     8249 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/anthropic/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/chroma/__init__.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/chroma/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/cohere/__init__.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py
+-rw-r--r--   0        0        0    26563 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/cohere/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/groq/__init__.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py
+-rw-r--r--   0        0        0    25572 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/groq/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py
+-rw-r--r--   0        0        0     3789 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain_community/__init__.py
+-rw-r--r--   0        0        0     5198 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain_core/__init__.py
+-rw-r--r--   0        0        0     5931 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py
+-rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langgraph/__init__.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py
+-rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langgraph/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/llamaindex/__init__.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py
+-rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py
+-rw-r--r--   0        0        0    36645 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/openai/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/pinecone/__init__.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/pinecone/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/qdrant/__init__.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/qdrant/patch.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/utils/llm.py
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/utils/with_root_span.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/__init__.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/conftest.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/utils.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/anthropic/conftest.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/anthropic/test_anthropic.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/anthropic/cassettes/test_anthropic.yaml
+-rw-r--r--   0        0        0    11675 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/chroma/test_chroma.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/cohere/conftest.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/cohere/test_cohere_chat.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/cohere/test_cohere_embed.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/cohere/test_cohere_rerank.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/cohere/cassettes/test_cohere_chat.yaml
+-rw-r--r--   0        0        0    10610 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml
+-rw-r--r--   0        0        0    27312 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/cohere/cassettes/test_cohere_embed.yaml
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/cohere/cassettes/test_cohere_rerank.yaml
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/langchain/test_langchain.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/langchain/test_langchain_community.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/langchain/test_langchain_core.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/openai/conftest.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/openai/test_chat_completion.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/openai/test_embeddings.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/openai/test_image_generation.py
+-rw-r--r--   0        0        0     6844 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/openai/cassettes/test_async_image_generation.yaml
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/openai/cassettes/test_chat_completion.yaml
+-rw-r--r--   0        0        0  2592394 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/openai/cassettes/test_chat_completion_streaming.yaml
+-rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/openai/cassettes/test_image_generation.yaml
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/src/tests/pinecone/test_pinecone.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/LICENSE
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/README.md
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 langtrace_python_sdk-2.0.4/PKG-INFO
```

### Comparing `langtrace_python_sdk-2.0.3/src/run_example.py` & `langtrace_python_sdk-2.0.4/src/run_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/anthropic_example/completion.py` & `langtrace_python_sdk-2.0.4/src/examples/anthropic_example/completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/chroma_example/basic.py` & `langtrace_python_sdk-2.0.4/src/examples/chroma_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/cohere_example/chat.py` & `langtrace_python_sdk-2.0.4/src/examples/cohere_example/chat.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/cohere_example/chat_stream.py` & `langtrace_python_sdk-2.0.4/src/examples/cohere_example/chat_stream.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/cohere_example/embed.py` & `langtrace_python_sdk-2.0.4/src/examples/cohere_example/embed.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/cohere_example/rerank.py` & `langtrace_python_sdk-2.0.4/src/examples/cohere_example/rerank.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/cohere_example/tools.py` & `langtrace_python_sdk-2.0.4/src/examples/cohere_example/tools.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/fastapi_example/basic_route.py` & `langtrace_python_sdk-2.0.4/src/examples/fastapi_example/basic_route.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/langchain_example/basic.py` & `langtrace_python_sdk-2.0.4/src/examples/langchain_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/langchain_example/groq_example.py` & `langtrace_python_sdk-2.0.4/src/examples/langchain_example/groq_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/langchain_example/langgraph_example.py` & `langtrace_python_sdk-2.0.4/src/examples/langchain_example/langgraph_example.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/langchain_example/tool.py` & `langtrace_python_sdk-2.0.4/src/examples/langchain_example/tool.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/llamaindex_example/agent.py` & `langtrace_python_sdk-2.0.4/src/examples/llamaindex_example/agent.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/llamaindex_example/basic.py` & `langtrace_python_sdk-2.0.4/src/examples/llamaindex_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/llamaindex_example/data/abramov.txt` & `langtrace_python_sdk-2.0.4/src/examples/llamaindex_example/data/abramov.txt`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/openai_example/async_tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.0.4/src/examples/openai_example/async_tool_calling_nonstreaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/openai_example/async_tool_calling_streaming.py` & `langtrace_python_sdk-2.0.4/src/examples/openai_example/async_tool_calling_streaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/openai_example/chat_completion.py` & `langtrace_python_sdk-2.0.4/src/examples/openai_example/chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/openai_example/function_calling.py` & `langtrace_python_sdk-2.0.4/src/examples/openai_example/function_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/openai_example/tool_calling.py` & `langtrace_python_sdk-2.0.4/src/examples/openai_example/tool_calling.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/openai_example/tool_calling_nonstreaming.py` & `langtrace_python_sdk-2.0.4/src/examples/openai_example/tool_calling_nonstreaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/openai_example/tool_calling_streaming.py` & `langtrace_python_sdk-2.0.4/src/examples/openai_example/tool_calling_streaming.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/perplexity_example/basic.py` & `langtrace_python_sdk-2.0.4/src/examples/perplexity_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/pinecone_example/basic.py` & `langtrace_python_sdk-2.0.4/src/examples/pinecone_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/examples/qdrant_example/basic.py` & `langtrace_python_sdk-2.0.4/src/examples/qdrant_example/basic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/__init__.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/langtrace.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/langtrace.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/constants/instrumentation/chroma.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/constants/instrumentation/cohere.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/cohere.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/constants/instrumentation/common.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/common.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/constants/instrumentation/openai.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/constants/instrumentation/qdrant.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/constants/instrumentation/qdrant.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/extensions/langtrace_exporter.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/extensions/langtrace_exporter.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/anthropic/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/anthropic/patch.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/anthropic/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/chroma/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/chroma/patch.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/chroma/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/cohere/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/cohere/patch.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/cohere/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/groq/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/groq/patch.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/groq/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/langchain/patch.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain_community/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain_community/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain_core/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langchain_core/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langgraph/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/langgraph/patch.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/langgraph/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/llamaindex/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/llamaindex/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/openai/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/openai/patch.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/openai/patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -711,21 +711,19 @@
             "llm.model": kwargs.get("model"),
             "llm.prompts": "",
             "llm.embedding_inputs": json.dumps([kwargs.get("input", "")]),
             **(extra_attributes if extra_attributes is not None else {}),
         }
 
         if kwargs.get("encoding_format") is not None:
-            span_attributes["llm.encoding_format"] = json.dumps([kwargs.get("encoding_format")])
+            span_attributes["llm.encoding.formats"] = json.dumps([kwargs.get("encoding_format")])
 
         attributes = LLMSpanAttributes(**span_attributes)
         kwargs.get("encoding_format")
 
-        if kwargs.get("encoding_format") is not None:
-            attributes.llm_encoding_format = kwargs.get("encoding_format")
         if kwargs.get("dimensions") is not None:
             attributes["llm.dimensions"] = kwargs.get("dimensions")
         if kwargs.get("user") is not None:
             attributes["llm.user"] = kwargs.get("user")
 
         with tracer.start_as_current_span(
             APIS["EMBEDDINGS_CREATE"]["METHOD"], kind=SpanKind.CLIENT
```

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/pinecone/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/pinecone/patch.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/pinecone/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/qdrant/instrumentation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/instrumentation/qdrant/patch.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/instrumentation/qdrant/patch.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/utils/llm.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/utils/llm.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/langtrace_python_sdk/utils/with_root_span.py` & `langtrace_python_sdk-2.0.4/src/langtrace_python_sdk/utils/with_root_span.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/conftest.py` & `langtrace_python_sdk-2.0.4/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/utils.py` & `langtrace_python_sdk-2.0.4/src/tests/utils.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/anthropic/conftest.py` & `langtrace_python_sdk-2.0.4/src/tests/anthropic/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/anthropic/test_anthropic.py` & `langtrace_python_sdk-2.0.4/src/tests/anthropic/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/anthropic/cassettes/test_anthropic.yaml` & `langtrace_python_sdk-2.0.4/src/tests/anthropic/cassettes/test_anthropic.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml` & `langtrace_python_sdk-2.0.4/src/tests/anthropic/cassettes/test_anthropic_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml` & `langtrace_python_sdk-2.0.4/src/tests/anthropic/cassettes/test_async_anthropic_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/chroma/test_chroma.py` & `langtrace_python_sdk-2.0.4/src/tests/chroma/test_chroma.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/cohere/conftest.py` & `langtrace_python_sdk-2.0.4/src/tests/cohere/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/cohere/test_cohere_chat.py` & `langtrace_python_sdk-2.0.4/src/tests/cohere/test_cohere_chat.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/cohere/test_cohere_embed.py` & `langtrace_python_sdk-2.0.4/src/tests/cohere/test_cohere_embed.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/cohere/test_cohere_rerank.py` & `langtrace_python_sdk-2.0.4/src/tests/cohere/test_cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/cohere/cassettes/test_cohere_chat.yaml` & `langtrace_python_sdk-2.0.4/src/tests/cohere/cassettes/test_cohere_chat.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml` & `langtrace_python_sdk-2.0.4/src/tests/cohere/cassettes/test_cohere_chat_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/cohere/cassettes/test_cohere_embed.yaml` & `langtrace_python_sdk-2.0.4/src/tests/cohere/cassettes/test_cohere_embed.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/cohere/cassettes/test_cohere_rerank.yaml` & `langtrace_python_sdk-2.0.4/src/tests/cohere/cassettes/test_cohere_rerank.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/langchain/test_langchain.py` & `langtrace_python_sdk-2.0.4/src/tests/langchain/test_langchain.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/langchain/test_langchain_community.py` & `langtrace_python_sdk-2.0.4/src/tests/langchain/test_langchain_community.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/langchain/test_langchain_core.py` & `langtrace_python_sdk-2.0.4/src/tests/langchain/test_langchain_core.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/openai/conftest.py` & `langtrace_python_sdk-2.0.4/src/tests/openai/conftest.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/openai/test_chat_completion.py` & `langtrace_python_sdk-2.0.4/src/tests/openai/test_chat_completion.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/openai/test_image_generation.py` & `langtrace_python_sdk-2.0.4/src/tests/openai/test_image_generation.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.0.4/src/tests/openai/cassettes/test_async_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/openai/cassettes/test_async_image_generation.yaml` & `langtrace_python_sdk-2.0.4/src/tests/openai/cassettes/test_async_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/openai/cassettes/test_chat_completion.yaml` & `langtrace_python_sdk-2.0.4/src/tests/openai/cassettes/test_chat_completion.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/openai/cassettes/test_chat_completion_streaming.yaml` & `langtrace_python_sdk-2.0.4/src/tests/openai/cassettes/test_chat_completion_streaming.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/openai/cassettes/test_image_generation.yaml` & `langtrace_python_sdk-2.0.4/src/tests/openai/cassettes/test_image_generation.yaml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/src/tests/pinecone/test_pinecone.py` & `langtrace_python_sdk-2.0.4/src/tests/pinecone/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/.gitignore` & `langtrace_python_sdk-2.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/LICENSE` & `langtrace_python_sdk-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/README.md` & `langtrace_python_sdk-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/pyproject.toml` & `langtrace_python_sdk-2.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `langtrace_python_sdk-2.0.3/PKG-INFO` & `langtrace_python_sdk-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: langtrace-python-sdk
-Version: 2.0.3
+Version: 2.0.4
 Summary: Python SDK for LangTrace
 Project-URL: Homepage, https://github.com/Scale3-Labs/langtrace-python-sdk
 Author-email: Scale3 Labs <engineering@scale3labs.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

