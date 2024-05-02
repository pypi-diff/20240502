# Comparing `tmp/haystack_ai-2.0.1rc2.tar.gz` & `tmp/haystack_ai-2.1.0rc1.tar.gz`

## Comparing `haystack_ai-2.0.1rc2.tar` & `haystack_ai-2.1.0rc1.tar`

### file list

```diff
@@ -1,169 +1,188 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/VERSION.txt
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/__init__.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/errors.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/lazy_imports.py
--rw-r--r--   0        0        0    13009 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/logging.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/__init__.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/audio/__init__.py
--rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/audio/whisper_local.py
--rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/audio/whisper_remote.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/builders/__init__.py
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/builders/answer_builder.py
--rw-r--r--   0        0        0    10149 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/builders/dynamic_chat_prompt_builder.py
--rw-r--r--   0        0        0     7114 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/builders/dynamic_prompt_builder.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/builders/prompt_builder.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/caching/__init__.py
--rw-r--r--   0        0        0     4340 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/caching/cache_checker.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/classifiers/__init__.py
--rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/classifiers/document_language_classifier.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/connectors/__init__.py
--rw-r--r--   0        0        0    13706 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/connectors/openapi_service.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/converters/__init__.py
--rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/converters/azure.py
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/converters/html.py
--rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/converters/markdown.py
--rw-r--r--   0        0        0    11212 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/converters/openapi_functions.py
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/converters/output_adapter.py
--rw-r--r--   0        0        0     4779 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/converters/pypdf.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/converters/tika.py
--rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/converters/txt.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/converters/utils.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/__init__.py
--rw-r--r--   0        0        0     8738 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/azure_document_embedder.py
--rw-r--r--   0        0        0     6392 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/azure_text_embedder.py
--rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/hugging_face_tei_document_embedder.py
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/hugging_face_tei_text_embedder.py
--rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/openai_document_embedder.py
--rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/openai_text_embedder.py
--rw-r--r--   0        0        0     6554 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/sentence_transformers_document_embedder.py
--rw-r--r--   0        0        0     5213 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/sentence_transformers_text_embedder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/backends/__init__.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/embedders/backends/sentence_transformers_backend.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/extractors/__init__.py
--rw-r--r--   0        0        0    16195 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/extractors/named_entity_extractor.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/fetchers/__init__.py
--rw-r--r--   0        0        0     9328 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/fetchers/link_content.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/__init__.py
--rw-r--r--   0        0        0     9010 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/azure.py
--rw-r--r--   0        0        0    12132 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/hugging_face_local.py
--rw-r--r--   0        0        0    12720 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/hugging_face_tgi.py
--rw-r--r--   0        0        0    14157 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/openai.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/utils.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/chat/__init__.py
--rw-r--r--   0        0        0     9647 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/chat/azure.py
--rw-r--r--   0        0        0    17612 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/chat/hugging_face_local.py
--rw-r--r--   0        0        0    14988 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/chat/hugging_face_tgi.py
--rw-r--r--   0        0        0    17574 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/generators/chat/openai.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/joiners/__init__.py
--rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/joiners/document_joiner.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/others/__init__.py
--rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/others/multiplexer.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/preprocessors/__init__.py
--rw-r--r--   0        0        0    10129 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/preprocessors/document_cleaner.py
--rw-r--r--   0        0        0     4477 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/preprocessors/document_splitter.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/preprocessors/text_cleaner.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/rankers/__init__.py
--rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/rankers/lost_in_the_middle.py
--rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/rankers/meta_field.py
--rw-r--r--   0        0        0    11598 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/rankers/transformers_similarity.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/readers/__init__.py
--rw-r--r--   0        0        0    27493 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/readers/extractive.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/retrievers/__init__.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/retrievers/filter_retriever.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/retrievers/in_memory/__init__.py
--rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/retrievers/in_memory/bm25_retriever.py
--rw-r--r--   0        0        0     6106 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/retrievers/in_memory/embedding_retriever.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/routers/__init__.py
--rw-r--r--   0        0        0    10114 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/routers/conditional_router.py
--rw-r--r--   0        0        0     4415 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/routers/file_type_router.py
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/routers/metadata_router.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/routers/text_language_router.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/samplers/__init__.py
--rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/samplers/top_p.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/validators/__init__.py
--rw-r--r--   0        0        0    10340 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/validators/json_schema.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/websearch/__init__.py
--rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/websearch/searchapi.py
--rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/websearch/serper_dev.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/writers/__init__.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/components/writers/document_writer.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/errors.py
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/serialization.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/type_utils.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/component/__init__.py
--rw-r--r--   0        0        0    16335 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/component/component.py
--rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/component/sockets.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/component/types.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/pipeline/__init__.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/pipeline/descriptions.py
--rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/pipeline/draw.py
--rw-r--r--   0        0        0    53414 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/pipeline/pipeline.py
--rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/pipeline/template.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/pipeline/predefined/indexing.yaml.jinja2
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/core/pipeline/predefined/rag.yaml.jinja2
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/dataclasses/__init__.py
--rw-r--r--   0        0        0     4874 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/dataclasses/answer.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/dataclasses/byte_stream.py
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/dataclasses/chat_message.py
--rw-r--r--   0        0        0     8530 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/dataclasses/document.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/dataclasses/sparse_embedding.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/dataclasses/streaming_chunk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/document_stores/__init__.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/document_stores/errors/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/document_stores/errors/errors.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/document_stores/in_memory/__init__.py
--rw-r--r--   0        0        0    15576 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/document_stores/in_memory/document_store.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/document_stores/types/__init__.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/document_stores/types/policy.py
--rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/document_stores/types/protocol.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/marshal/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/marshal/protocol.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/marshal/yaml.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/telemetry/__init__.py
--rw-r--r--   0        0        0     3567 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/telemetry/_environment.py
--rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/telemetry/_telemetry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/__init__.py
--rw-r--r--   0        0        0    57626 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/document_store.py
--rw-r--r--   0        0        0     8049 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/factory.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/test_utils.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/__init__.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/accumulate.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/add_value.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/concatenate.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/double.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/fstring.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/greet.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/hello.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/joiner.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/parity.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/remainder.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/repeat.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/self_loop.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/subtract.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/sum.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/text_splitter.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/testing/sample_components/threshold.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/tracing/__init__.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/tracing/datadog.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/tracing/opentelemetry.py
--rw-r--r--   0        0        0     7289 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/tracing/tracer.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/tracing/utils.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/utils/__init__.py
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/utils/auth.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/utils/callable_serialization.py
--rw-r--r--   0        0        0    15291 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/utils/device.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/utils/expit.py
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/utils/filters.py
--rw-r--r--   0        0        0    10666 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/utils/hf.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/utils/jupyter.py
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/utils/requests_utils.py
--rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/haystack/utils/type_serialization.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/.gitignore
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/LICENSE
--rw-r--r--   0        0        0    10480 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/README.md
--rw-r--r--   0        0        0     9627 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/pyproject.toml
--rw-r--r--   0        0        0    12378 2020-02-02 00:00:00.000000 haystack_ai-2.0.1rc2/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/VERSION.txt
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/__init__.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/errors.py
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/lazy_imports.py
+-rw-r--r--   0        0        0    13429 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/logging.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/__init__.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/audio/__init__.py
+-rw-r--r--   0        0        0     7398 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/audio/whisper_local.py
+-rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/audio/whisper_remote.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/builders/__init__.py
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/builders/answer_builder.py
+-rw-r--r--   0        0        0     9405 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/builders/dynamic_chat_prompt_builder.py
+-rw-r--r--   0        0        0     7130 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/builders/dynamic_prompt_builder.py
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/builders/prompt_builder.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/caching/__init__.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/caching/cache_checker.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/classifiers/__init__.py
+-rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/classifiers/document_language_classifier.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/connectors/__init__.py
+-rw-r--r--   0        0        0    13841 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/connectors/openapi_service.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/converters/__init__.py
+-rw-r--r--   0        0        0    24642 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/converters/azure.py
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/converters/html.py
+-rw-r--r--   0        0        0     3851 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/converters/markdown.py
+-rw-r--r--   0        0        0    11313 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/converters/openapi_functions.py
+-rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/converters/output_adapter.py
+-rw-r--r--   0        0        0     6591 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/converters/pdfminer.py
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/converters/pypdf.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/converters/tika.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/converters/txt.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/converters/utils.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/embedders/__init__.py
+-rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/embedders/azure_document_embedder.py
+-rw-r--r--   0        0        0     6894 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/embedders/azure_text_embedder.py
+-rw-r--r--   0        0        0    10897 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/embedders/hugging_face_api_document_embedder.py
+-rw-r--r--   0        0        0     8000 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/embedders/hugging_face_api_text_embedder.py
+-rw-r--r--   0        0        0     8671 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/embedders/hugging_face_tei_document_embedder.py
+-rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/embedders/hugging_face_tei_text_embedder.py
+-rw-r--r--   0        0        0     7559 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/embedders/openai_document_embedder.py
+-rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/embedders/openai_text_embedder.py
+-rw-r--r--   0        0        0     6971 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/embedders/sentence_transformers_document_embedder.py
+-rw-r--r--   0        0        0     5630 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/embedders/sentence_transformers_text_embedder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/embedders/backends/__init__.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/embedders/backends/sentence_transformers_backend.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/evaluators/__init__.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/evaluators/answer_exact_match.py
+-rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/evaluators/context_relevance.py
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/evaluators/document_map.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/evaluators/document_mrr.py
+-rw-r--r--   0        0        0     4561 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/evaluators/document_recall.py
+-rw-r--r--   0        0        0     7468 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/evaluators/faithfulness.py
+-rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/evaluators/llm_evaluator.py
+-rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/evaluators/sas_evaluator.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/extractors/__init__.py
+-rw-r--r--   0        0        0    16245 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/extractors/named_entity_extractor.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/fetchers/__init__.py
+-rw-r--r--   0        0        0     9385 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/fetchers/link_content.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/generators/__init__.py
+-rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/generators/azure.py
+-rw-r--r--   0        0        0     9860 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/generators/hugging_face_api.py
+-rw-r--r--   0        0        0    11239 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/generators/hugging_face_local.py
+-rw-r--r--   0        0        0    12949 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/generators/hugging_face_tgi.py
+-rw-r--r--   0        0        0    13449 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/generators/openai.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/generators/utils.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/generators/chat/__init__.py
+-rw-r--r--   0        0        0     9791 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/generators/chat/azure.py
+-rw-r--r--   0        0        0    11186 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/generators/chat/hugging_face_api.py
+-rw-r--r--   0        0        0    17793 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/generators/chat/hugging_face_local.py
+-rw-r--r--   0        0        0    15485 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/generators/chat/hugging_face_tgi.py
+-rw-r--r--   0        0        0    16934 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/generators/chat/openai.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/joiners/__init__.py
+-rw-r--r--   0        0        0     6614 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/joiners/document_joiner.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/others/__init__.py
+-rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/others/multiplexer.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/preprocessors/__init__.py
+-rw-r--r--   0        0        0    10218 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/preprocessors/document_cleaner.py
+-rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/preprocessors/document_splitter.py
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/preprocessors/text_cleaner.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/rankers/__init__.py
+-rw-r--r--   0        0        0     6102 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/rankers/lost_in_the_middle.py
+-rw-r--r--   0        0        0    17048 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/rankers/meta_field.py
+-rw-r--r--   0        0        0    10877 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/rankers/sentence_transformers_diversity.py
+-rw-r--r--   0        0        0    11598 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/rankers/transformers_similarity.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/readers/__init__.py
+-rw-r--r--   0        0        0    27548 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/readers/extractive.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/retrievers/__init__.py
+-rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/retrievers/filter_retriever.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/retrievers/in_memory/__init__.py
+-rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/retrievers/in_memory/bm25_retriever.py
+-rw-r--r--   0        0        0     6106 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/retrievers/in_memory/embedding_retriever.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/routers/__init__.py
+-rw-r--r--   0        0        0    10151 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/routers/conditional_router.py
+-rw-r--r--   0        0        0     5841 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/routers/file_type_router.py
+-rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/routers/metadata_router.py
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/routers/text_language_router.py
+-rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/routers/zero_shot_text_router.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/samplers/__init__.py
+-rw-r--r--   0        0        0     6053 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/samplers/top_p.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/validators/__init__.py
+-rw-r--r--   0        0        0    10328 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/validators/json_schema.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/websearch/__init__.py
+-rw-r--r--   0        0        0     6782 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/websearch/searchapi.py
+-rw-r--r--   0        0        0     6746 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/websearch/serper_dev.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/writers/__init__.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/components/writers/document_writer.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/core/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/core/errors.py
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/core/serialization.py
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/core/type_utils.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/core/component/__init__.py
+-rw-r--r--   0        0        0    18608 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/core/component/component.py
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/core/component/sockets.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/core/component/types.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/core/pipeline/__init__.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/core/pipeline/descriptions.py
+-rw-r--r--   0        0        0     5952 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/core/pipeline/draw.py
+-rw-r--r--   0        0        0    56764 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/core/pipeline/pipeline.py
+-rw-r--r--   0        0        0     5518 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/core/pipeline/template.py
+-rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/core/pipeline/predefined/indexing.yaml.jinja2
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/core/pipeline/predefined/rag.yaml.jinja2
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/dataclasses/__init__.py
+-rw-r--r--   0        0        0     5963 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/dataclasses/answer.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/dataclasses/byte_stream.py
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/dataclasses/chat_message.py
+-rw-r--r--   0        0        0     8531 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/dataclasses/document.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/dataclasses/sparse_embedding.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/dataclasses/streaming_chunk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/document_stores/__init__.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/document_stores/errors/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/document_stores/errors/errors.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/document_stores/in_memory/__init__.py
+-rw-r--r--   0        0        0    15577 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/document_stores/in_memory/document_store.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/document_stores/types/__init__.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/document_stores/types/policy.py
+-rw-r--r--   0        0        0     4777 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/document_stores/types/protocol.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/evaluation/__init__.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/evaluation/eval_run_result.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/marshal/__init__.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/marshal/protocol.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/marshal/yaml.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/telemetry/__init__.py
+-rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/telemetry/_environment.py
+-rw-r--r--   0        0        0     7384 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/telemetry/_telemetry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/__init__.py
+-rw-r--r--   0        0        0    63152 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/document_store.py
+-rw-r--r--   0        0        0     8049 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/factory.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/test_utils.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/sample_components/__init__.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/sample_components/accumulate.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/sample_components/add_value.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/sample_components/concatenate.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/sample_components/double.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/sample_components/fstring.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/sample_components/greet.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/sample_components/hello.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/sample_components/joiner.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/sample_components/parity.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/sample_components/remainder.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/sample_components/repeat.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/sample_components/self_loop.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/sample_components/subtract.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/sample_components/sum.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/sample_components/text_splitter.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/testing/sample_components/threshold.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/tracing/__init__.py
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/tracing/datadog.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/tracing/opentelemetry.py
+-rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/tracing/tracer.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/tracing/utils.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/utils/__init__.py
+-rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/utils/auth.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/utils/callable_serialization.py
+-rw-r--r--   0        0        0    15428 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/utils/device.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/utils/expit.py
+-rw-r--r--   0        0        0    11735 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/utils/filters.py
+-rw-r--r--   0        0        0    15510 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/utils/hf.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/utils/jupyter.py
+-rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/utils/requests_utils.py
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/utils/type_serialization.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/haystack/utils/url_validation.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/.gitignore
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/LICENSE
+-rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/README.md
+-rw-r--r--   0        0        0    10033 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    13263 2020-02-02 00:00:00.000000 haystack_ai-2.1.0rc1/PKG-INFO
```

### Comparing `haystack_ai-2.0.1rc2/haystack/__init__.py` & `haystack_ai-2.1.0rc1/haystack/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/lazy_imports.py` & `haystack_ai-2.1.0rc1/haystack/lazy_imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,28 @@
 from lazy_imports.try_import import _DeferredImportExceptionContextManager
 
 DEFAULT_IMPORT_ERROR_MSG = "Try 'pip install {}'"
 
 
 class LazyImport(_DeferredImportExceptionContextManager):
     """
-    Wrapper on top of lazy_import's _DeferredImportExceptionContextManager that adds the possibility to customize the
-    error messages.
+    Wrapper on top of lazy_import's _DeferredImportExceptionContextManager.
+
+    It adds the possibility to customize the error messages.
     """
 
     def __init__(self, message: str = DEFAULT_IMPORT_ERROR_MSG) -> None:
         super().__init__()
         self.import_error_msg = message
 
     def __exit__(
         self, exc_type: Optional[Type[Exception]], exc_value: Optional[Exception], traceback: Optional[TracebackType]
     ) -> Optional[bool]:
-        """Exit the context manager.
+        """
+        Exit the context manager.
 
         Args:
             exc_type:
                 Raised exception type. :obj:`None` if nothing is raised.
             exc_value:
                 Raised exception object. :obj:`None` if nothing is raised.
             traceback:
```

### Comparing `haystack_ai-2.0.1rc2/haystack/logging.py` & `haystack_ai-2.1.0rc1/haystack/logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,143 +22,143 @@
         *,
         _: Any = None,
         exc_info: Any = None,
         stack_info: Any = False,
         stacklevel: int = 1,
         **kwargs: Any,
     ) -> None:
-        ...
+        """Log a debug message."""
 
     def info(
         self,
         msg: str,
         *,
         _: Any = None,
         exc_info: Any = None,
         stack_info: Any = False,
         stacklevel: int = 1,
         **kwargs: Any,
     ) -> None:
-        ...
+        """Log an info message."""
 
     def warn(
         self,
         msg: str,
         *,
         _: Any = None,
         exc_info: Any = None,
         stack_info: Any = False,
         stacklevel: int = 1,
         **kwargs: Any,
     ) -> None:
-        ...
+        """Log a warning message."""
 
     def warning(
         self,
         msg: str,
         *,
         _: Any = None,
         exc_info: Any = None,
         stack_info: Any = False,
         stacklevel: int = 1,
         **kwargs: Any,
     ) -> None:
-        ...
+        """Log a warning message."""
 
     def error(
         self,
         msg: str,
         *,
         _: Any = None,
         exc_info: Any = None,
         stack_info: Any = False,
         stacklevel: int = 1,
         **kwargs: Any,
     ) -> None:
-        ...
+        """Log an error message."""
 
     def critical(
         self,
         msg: str,
         *,
         _: Any = None,
         exc_info: Any = None,
         stack_info: Any = False,
         stacklevel: int = 1,
         **kwargs: Any,
     ) -> None:
-        ...
+        """Log a critical message."""
 
     def exception(
         self,
         msg: str,
         *,
         _: Any = None,
         exc_info: Any = None,
         stack_info: Any = False,
         stacklevel: int = 1,
         **kwargs: Any,
     ) -> None:
-        ...
+        """Log an exception message."""
 
     def fatal(
         self,
         msg: str,
         *,
         _: Any = None,
         exc_info: Any = None,
         stack_info: Any = False,
         stacklevel: int = 1,
         **kwargs: Any,
     ) -> None:
-        ...
+        """Log a fatal message."""
 
     def log(
         self,
         level: int,
         msg: str,
         *,
         _: Any = None,
         exc_info: Any = None,
         stack_info: Any = False,
         stacklevel: int = 1,
         **kwargs: Any,
     ) -> None:
-        ...
+        """Log a message."""
 
     def setLevel(self, level: int) -> None:
-        ...
+        """Set the logging level."""
 
 
 def patch_log_method_to_kwargs_only(func: typing.Callable) -> typing.Callable:
     """A decorator to make sure that a function is only called with keyword arguments."""
 
     @functools.wraps(func)
-    def log_only_with_kwargs(
+    def _log_only_with_kwargs(
         msg, *, _: Any = None, exc_info: Any = None, stack_info: Any = False, stacklevel: int = 1, **kwargs: Any
     ) -> Any:  # we need the `_` to avoid a syntax error
         existing_extra = kwargs.pop("extra", {})
         return func(
             # we need to increase the stacklevel by 1 to point to the correct caller
             # (otherwise it points to this function)
             msg,
             exc_info=exc_info,
             stack_info=stack_info,
             stacklevel=stacklevel + 1,
             extra={**existing_extra, **kwargs},
         )
 
-    return log_only_with_kwargs
+    return _log_only_with_kwargs
 
 
 def patch_log_with_level_method_to_kwargs_only(func: typing.Callable) -> typing.Callable:
     """A decorator to make sure that a function is only called with keyword arguments."""
 
     @functools.wraps(func)
-    def log_only_with_kwargs(
+    def _log_only_with_kwargs(
         level,
         msg,
         *,
         _: Any = None,
         exc_info: Any = None,
         stack_info: Any = False,
         stacklevel: int = 1,
@@ -173,25 +173,27 @@
             stack_info=stack_info,
             # we need to increase the stacklevel by 1 to point to the correct caller
             # (otherwise it points to this function)
             stacklevel=stacklevel + 1,
             extra={**existing_extra, **kwargs},
         )
 
-    return log_only_with_kwargs
+    return _log_only_with_kwargs
 
 
 def patch_make_records_to_use_kwarg_string_interpolation(original_make_records: typing.Callable) -> typing.Callable:
+    """A decorator to ensure string interpolation is used."""
+
     @functools.wraps(original_make_records)
-    def wrapper(name, level, fn, lno, msg, args, exc_info, func=None, extra=None, sinfo=None) -> Any:
+    def _wrapper(name, level, fn, lno, msg, args, exc_info, func=None, extra=None, sinfo=None) -> Any:
         safe_extra = extra or {}
         interpolated_msg = msg.format(**safe_extra)
         return original_make_records(name, level, fn, lno, interpolated_msg, (), exc_info, func, extra, sinfo)
 
-    return wrapper
+    return _wrapper
 
 
 def _patch_structlog_call_information(logger: logging.Logger) -> None:
     # structlog patches the findCaller to hide itself from the traceback.
     # We need to patch their patch to hide `haystack.logging` from the traceback.
     try:
         from structlog._frames import _find_first_app_frame_and_name, _format_stack
@@ -215,19 +217,23 @@
 
         logger.findCaller = findCaller  # type: ignore
     except ImportError:
         pass
 
 
 def getLogger(name: str) -> PatchedLogger:
+    """
+    Get the Haystack logger, a patched version of the one from the standard library.
+
+    We patch the default logger methods to make sure that they are only called with keyword arguments.
+    We enforce keyword-arguments because
+        - it brings in consistency
+        - it makes structure logging effective, not just an available feature
+    """
     logger = logging.getLogger(name)
-    # We patch the default logger methods to make sure that they are only called with keyword arguments.
-    # We enforce keyword-arguments because
-    # - it brings in consistency
-    # - it makes structure logging effective, not just an available feature
     logger.debug = patch_log_method_to_kwargs_only(logger.debug)  # type: ignore
     logger.info = patch_log_method_to_kwargs_only(logger.info)  # type: ignore
     logger.warn = patch_log_method_to_kwargs_only(logger.warn)  # type: ignore
     logger.warning = patch_log_method_to_kwargs_only(logger.warning)  # type: ignore
     logger.error = patch_log_method_to_kwargs_only(logger.error)  # type: ignore
     logger.critical = patch_log_method_to_kwargs_only(logger.critical)  # type: ignore
     logger.exception = patch_log_method_to_kwargs_only(logger.exception)  # type: ignore
@@ -251,15 +257,16 @@
     event_dict["lineno"] = stdlib_record.lineno
     event_dict["module"] = stdlib_record.name
 
     return event_dict
 
 
 def correlate_logs_with_traces(_: "WrappedLogger", __: str, event_dict: "EventDict") -> "EventDict":
-    """Add correlation data for logs.
+    """
+    Add correlation data for logs.
 
     This is useful if you want to correlate logs with traces.
     """
     import haystack.tracing.tracer  # to avoid circular imports
 
     if not haystack.tracing.is_tracing_enabled():
         return event_dict
@@ -268,15 +275,16 @@
     if current_span:
         event_dict.update(current_span.get_correlation_data_for_logs())
 
     return event_dict
 
 
 def configure_logging(use_json: Optional[bool] = None) -> None:
-    """Configure logging for Haystack.
+    """
+    Configure logging for Haystack.
 
     - If `structlog` is not installed, we keep everything as it is. The user is responsible for configuring logging
       themselves.
     - If `structlog` is installed, we configure it to format log entries including its key-value data. To disable this
       behavior set the environment variable `HAYSTACK_LOGGING_IGNORE_STRUCTLOG` to `true`.
     - If `structlog` is installed, you can JSON format all logs. Enable this by
         - setting the `use_json` parameter to `True` when calling this function
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/audio/whisper_local.py` & `haystack_ai-2.1.0rc1/haystack/components/audio/whisper_local.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/components/audio/whisper_remote.py` & `haystack_ai-2.1.0rc1/haystack/components/audio/whisper_remote.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/components/builders/answer_builder.py` & `haystack_ai-2.1.0rc1/haystack/components/builders/answer_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 logger = logging.getLogger(__name__)
 
 
 @component
 class AnswerBuilder:
     """
     Takes a query and the replies a Generator returns as input and parses them into GeneratedAnswer objects.
+
     Optionally, it also takes Documents and metadata from the Generator as inputs to enrich the GeneratedAnswer objects.
 
     Usage example:
     ```python
     from haystack.components.builders import AnswerBuilder
 
     builder = AnswerBuilder(pattern="Answer: (.*)")
@@ -122,17 +123,18 @@
 
         return {"answers": all_answers}
 
     @staticmethod
     def _extract_answer_string(reply: str, pattern: Optional[str] = None) -> str:
         """
         Extract the answer string from the generator output using the specified pattern.
+
         If no pattern is specified, the whole string is used as the answer.
 
-        :param replies:
+        :param reply:
             The output of the Generator. A string.
         :param pattern:
             The regular expression pattern to use to extract the answer text from the generator output.
         """
         if pattern is None:
             return reply
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/builders/dynamic_chat_prompt_builder.py` & `haystack_ai-2.1.0rc1/haystack/components/builders/dynamic_chat_prompt_builder.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 
 logger = logging.getLogger(__name__)
 
 
 @component
 class DynamicChatPromptBuilder:
     """
-    DynamicChatPromptBuilder is designed to construct dynamic prompts from a list of `ChatMessage` instances. It
-    integrates with Jinja2 templating for dynamic prompt generation. It assumes that the last user message in the list
-    contains a template and renders it with variables provided to the constructor. Additional template variables
-    can be feed into the pipeline `run` method and will be merged before rendering the template.
+    DynamicChatPromptBuilder is designed to construct dynamic prompts from a list of `ChatMessage` instances.
+
+    It integrates with Jinja2 templating for dynamic prompt generation. It considers any user or system message in the
+    list potentially containing a template and renders it with variables provided to the constructor. Additional
+    template variables can be feed into the component/pipeline `run` method and will be merged before rendering the
+    template.
 
     Usage example:
     ```python
     from haystack.components.builders import DynamicChatPromptBuilder
     from haystack.components.generators.chat import OpenAIChatGenerator
     from haystack.dataclasses import ChatMessage
     from haystack import Pipeline
@@ -30,19 +32,20 @@
 
     pipe = Pipeline()
     pipe.add_component("prompt_builder", prompt_builder)
     pipe.add_component("llm", llm)
     pipe.connect("prompt_builder.prompt", "llm.messages")
 
     location = "Berlin"
-    system_message = ChatMessage.from_system("You are a helpful assistant giving out valuable information to tourists.")
+    language = "English"
+    system_message = ChatMessage.from_system("You are an assistant giving information to tourists in {{language}}")
     messages = [system_message, ChatMessage.from_user("Tell me about {{location}}")]
 
-
-    res = pipe.run(data={"prompt_builder": {"template_variables": {"location": location}, "prompt_source": messages}})
+    res = pipe.run(data={"prompt_builder": {"template_variables": {"location": location, "language": language},
+                                        "prompt_source": messages}})
     print(res)
 
     >> {'llm': {'replies': [ChatMessage(content="Berlin is the capital city of Germany and one of the most vibrant
     and diverse cities in Europe. Here are some key things to know...Enjoy your time exploring the vibrant and dynamic
     capital of Germany!", role=<ChatRole.ASSISTANT: 'assistant'>, name=None, meta={'model': 'gpt-3.5-turbo-0613',
     'index': 0, 'finish_reason': 'stop', 'usage': {'prompt_tokens': 27, 'completion_tokens': 681, 'total_tokens':
     708}})]}}
@@ -87,56 +90,31 @@
         # setup outputs
         component.set_output_types(self, prompt=List[ChatMessage])
         self.runtime_variables = runtime_variables
 
     def run(self, prompt_source: List[ChatMessage], template_variables: Optional[Dict[str, Any]] = None, **kwargs):
         """
         Executes the dynamic prompt building process by processing a list of `ChatMessage` instances.
-        The last user message is treated as a template and rendered with the variables provided to the constructor.
-        You can provide additional template variables directly to this method, which are then merged with the variables
-        provided to the constructor.
+
+        Any user message or system message is inspected for templates and rendered with the variables provided to the
+        constructor. You can provide additional template variables directly to this method, which are then merged with
+        the variables provided to the constructor.
 
         :param prompt_source:
-            A list of `ChatMessage` instances. We make an assumption that the last user message has
-            the template for the chat prompt
+            A list of `ChatMessage` instances. All user and system messages are treated as potentially having templates
+            and are rendered with the provided template variables - if templates are found.
         :param template_variables:
             A dictionary of template variables. Template variables provided at initialization are required
             to resolve pipeline variables, and these are additional variables users can provide directly to this method.
         :param kwargs:
-            Additional keyword arguments, typically resolved from a pipeline, which are merged with the provided template variables.
+            Additional keyword arguments, typically resolved from a pipeline, which are merged with the provided
+            template variables.
 
         :returns: A dictionary with the following keys:
-            - `prompt`: The updated list of `ChatMessage` instances after rendering the string template.
-        """
-        kwargs = kwargs or {}
-        template_variables = template_variables or {}
-        template_variables_combined = {**kwargs, **template_variables}
-        if not template_variables_combined:
-            logger.warning(
-                "The DynamicChatPromptBuilder run method requires template variables, but none were provided. "
-                "Please provide an appropriate template variable to enable correct prompt generation."
-            )
-        result: List[ChatMessage] = self._process_chat_messages(prompt_source, template_variables_combined)
-        return {"prompt": result}
-
-    def _process_chat_messages(self, prompt_source: List[ChatMessage], template_variables: Dict[str, Any]):
-        """
-        Processes a list of :class:`ChatMessage` instances to generate a chat prompt.
-
-        It takes the last user message in the list, treats it as a template, and renders it with the provided
-        template variables. The resulting message replaces the last user message in the list, forming a complete,
-        templated chat prompt.
-
-        :param prompt_source:
-            A list of `ChatMessage` instances to be processed. The last message is expected
-            to be from a user and is treated as a template.
-        :param template_variables:
-            A dictionary of template variables used for rendering the last user message.
-        :returns:
-            A list of `ChatMessage` instances, where the last user message has been replaced with its
+            - `prompt`: The updated list of `ChatMessage` instances after rendering the found templates.
         :raises ValueError:
             If `chat_messages` is empty or contains elements that are not instances of `ChatMessage`.
         :raises ValueError:
             If the last message in `chat_messages` is not from a user.
         """
         if not prompt_source:
             raise ValueError(
@@ -146,29 +124,41 @@
         if not all(isinstance(message, ChatMessage) for message in prompt_source):
             raise ValueError(
                 f"The {self.__class__.__name__} expects a list containing only ChatMessage instances. "
                 f"The provided list contains other types. Please ensure that all elements in the list "
                 f"are ChatMessage instances."
             )
 
-        last_message: ChatMessage = prompt_source[-1]
-        if last_message.is_from(ChatRole.USER):
-            template = self._validate_template(last_message.content, set(template_variables.keys()))
-            templated_user_message = ChatMessage.from_user(template.render(template_variables))
-            return prompt_source[:-1] + [templated_user_message]
-        else:
+        kwargs = kwargs or {}
+        template_variables = template_variables or {}
+        template_variables = {**kwargs, **template_variables}
+        if not template_variables:
             logger.warning(
-                "DynamicChatPromptBuilder was not provided with a user message as the last message in "
-                "chat conversation, no templating will be applied."
+                "The DynamicChatPromptBuilder run method requires template variables, but none were provided. "
+                "Please provide an appropriate template variable to enable correct prompt generation."
             )
-            return prompt_source
+        processed_messages = []
+        for message in prompt_source:
+            if message.is_from(ChatRole.USER) or message.is_from(ChatRole.SYSTEM):
+                template = self._validate_template(message.content, set(template_variables.keys()))
+                rendered_content = template.render(template_variables)
+                rendered_message = (
+                    ChatMessage.from_user(rendered_content)
+                    if message.is_from(ChatRole.USER)
+                    else ChatMessage.from_system(rendered_content)
+                )
+                processed_messages.append(rendered_message)
+            else:
+                processed_messages.append(message)
+        return {"prompt": processed_messages}
 
     def _validate_template(self, template_text: str, provided_variables: Set[str]):
         """
         Checks if all the required template variables are provided to the pipeline `run` method.
+
         If all the required template variables are provided, returns a Jinja2 template object.
         Otherwise, raises a ValueError.
 
         :param template_text:
             A Jinja2 template as a string.
         :param provided_variables:
             A set of provided template variables.
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/builders/dynamic_prompt_builder.py` & `haystack_ai-2.1.0rc1/haystack/components/builders/dynamic_prompt_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 
 logger = logging.getLogger(__name__)
 
 
 @component
 class DynamicPromptBuilder:
     """
-    DynamicPromptBuilder is designed to construct dynamic prompts for the pipeline. Users can change the prompt
-    template at runtime by providing a new template for each pipeline run invocation if needed.
+    DynamicPromptBuilder is designed to construct dynamic prompts for the pipeline.
+
+    Users can change the prompt template at runtime by providing a new template for each pipeline run invocation
+    if needed.
 
     Usage example:
     ```python
     from typing import List
     from haystack.components.builders import DynamicPromptBuilder
     from haystack.components.generators import OpenAIGenerator
     from haystack import Pipeline, component, Document
@@ -88,20 +90,23 @@
         # setup outputs
         component.set_output_types(self, prompt=str)
 
         self.runtime_variables = runtime_variables
 
     def run(self, prompt_source: str, template_variables: Optional[Dict[str, Any]] = None, **kwargs):
         """
-        Executes the dynamic prompt building process. Depending on the provided type of `prompt_source`, this method
-        either processes a list of `ChatMessage` instances or a string template. In the case of `ChatMessage` instances,
-        the last user message is treated as a template and rendered with the resolved pipeline variables and any
-        additional template variables provided. For a string template, it directly applies the template variables to
-        render the final prompt. You can provide additional template variables directly to this method, that are then
-        merged with the variables resolved from the pipeline runtime.
+        Executes the dynamic prompt building process.
+
+        Depending on the provided type of `prompt_source`, this method either processes a list of `ChatMessage`
+        instances or a string template. In the case of `ChatMessage` instances, the last user message is treated as a
+        template and rendered with the resolved pipeline variables and any additional template variables provided.
+
+        For a string template, it directly applies the template variables to render the final prompt. You can provide
+        additional template variables directly to this method, that are then merged with the variables resolved from
+        the pipeline runtime.
 
         :param prompt_source:
             A string template.
         :param template_variables:
             An optional dictionary of template variables. Template variables provided at initialization are required
             to resolve pipeline variables, and these are additional variables users can provide directly to this method.
         :param kwargs:
@@ -123,14 +128,15 @@
         template = self._validate_template(prompt_source, set(template_variables_combined.keys()))
         result = template.render(template_variables_combined)
         return {"prompt": result}
 
     def _validate_template(self, template_text: str, provided_variables: Set[str]):
         """
         Checks if all the required template variables are provided to the pipeline `run` method.
+
         If all the required template variables are provided, returns a Jinja2 template object.
         Otherwise, raises a ValueError.
 
         :param template_text:
             A Jinja2 template as a string.
         :param provided_variables:
             A set of provided template variables.
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/caching/cache_checker.py` & `haystack_ai-2.1.0rc1/haystack/components/caching/cache_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 @component
 class CacheChecker:
     """
-    Checks for the presence of documents in a Document Store based on a specified
-    field in each document's metadata.
+    Checks for the presence of documents in a Document Store based on a specified field in each document's metadata.
 
     If matching documents are found, they are returned as hits. If not, the items
     are returned as misses, indicating they are not in the cache.
 
     Usage example:
     ```python
     from haystack import Document
@@ -72,15 +71,15 @@
         if "document_store" not in init_params:
             raise DeserializationError("Missing 'document_store' in serialization data")
         if "type" not in init_params["document_store"]:
             raise DeserializationError("Missing 'type' in document store's serialization data")
 
         try:
             module_name, type_ = init_params["document_store"]["type"].rsplit(".", 1)
-            logger.debug("Trying to import module '{module}'", module=module_name)
+            logger.debug("Trying to import module '{module_name}'", module_name=module_name)
             module = importlib.import_module(module_name)
         except (ImportError, DeserializationError) as e:
             raise DeserializationError(
                 f"DocumentStore of type '{init_params['document_store']['type']}' not correctly imported"
             ) from e
 
         docstore_class = getattr(module, type_)
@@ -88,16 +87,15 @@
 
         data["init_parameters"]["document_store"] = docstore
         return default_from_dict(cls, data)
 
     @component.output_types(hits=List[Document], misses=List)
     def run(self, items: List[Any]):
         """
-        Checks if any document associated with the specified cache field
-        is already present in the store.
+        Checks if any document associated with the specified cache field is already present in the store.
 
         :param items:
             Values to be checked against the cache field.
         :return:
             A dictionary with two keys:
             - `hits` - Documents that matched with any of the items.
             - `misses` - Items that were not present in any documents.
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/classifiers/document_language_classifier.py` & `haystack_ai-2.1.0rc1/haystack/components/classifiers/document_language_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,27 +46,30 @@
     assert len(written_docs) == 1
     assert written_docs[0] == Document(id="1", content="This is an English document", meta={"language": "en"})
     ```
     """
 
     def __init__(self, languages: Optional[List[str]] = None):
         """
+        Initialize the DocumentLanguageClassifier.
+
         :param languages: A list of languages in ISO code, each corresponding to a different output connection.
             For supported languages, see the [`langdetect` documentation](https://github.com/Mimino666/langdetect#languages).
             If not specified, the default is ["en"].
         """
         langdetect_import.check()
         if not languages:
             languages = ["en"]
         self.languages = languages
 
     @component.output_types(documents=List[Document])
     def run(self, documents: List[Document]):
         """
         This method classifies the documents' language and adds it to their metadata.
+
         If a Document's text does not match any of the languages specified at initialization,
         the metadata value "unmatched" will be stored.
 
         :param documents: A list of documents to classify their language.
 
         :returns: A dictionary with the following key:
             - `documents`: List of Documents with an added metadata field called `language`.
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/connectors/openapi_service.py` & `haystack_ai-2.1.0rc1/haystack/components/connectors/openapi_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 with LazyImport("Run 'pip install openapi3'") as openapi_imports:
     from openapi3 import OpenAPI
 
 
 @component
 class OpenAPIServiceConnector:
     """
+    A component which connects the Haystack framework to OpenAPI services.
+
     The `OpenAPIServiceConnector` component connects the Haystack framework to OpenAPI services, enabling it to call
     operations as defined in the OpenAPI specification of the service.
 
     It integrates with `ChatMessage` dataclass, where the payload in messages is used to determine the method to be
     called and the parameters to be passed. The message payload should be an OpenAI JSON formatted function calling
     string consisting of the method name and the parameters to be passed to the method. The method name and parameters
     are then used to invoke the method on the OpenAPI service. The response from the service is returned as a
@@ -73,16 +75,18 @@
     def run(
         self,
         messages: List[ChatMessage],
         service_openapi_spec: Dict[str, Any],
         service_credentials: Optional[Union[dict, str]] = None,
     ) -> Dict[str, List[ChatMessage]]:
         """
-        Processes a list of chat messages to invoke a method on an OpenAPI service. It parses the last message in the
-        list, expecting it to contain an OpenAI function calling descriptor (name & parameters) in JSON format.
+        Processes a list of chat messages to invoke a method on an OpenAPI service.
+
+        It parses the last message in the list, expecting it to contain an OpenAI function calling descriptor
+        (name & parameters) in JSON format.
 
         :param messages: A list of `ChatMessage` objects containing the messages to be processed. The last message
         should contain the function invocation payload in OpenAI function calling format. See the example in the class
         docstring for the expected format.
         :param service_openapi_spec: The OpenAPI JSON specification object of the service to be invoked. All the refs
         should already be resolved.
         :param service_credentials: The credentials to be used for authentication with the service.
@@ -144,14 +148,16 @@
                 function_payloads.append(
                     {"arguments": json.loads(function_call["arguments"]), "name": function_call["name"]}
                 )
         return function_payloads
 
     def _authenticate_service(self, openapi_service: OpenAPI, credentials: Optional[Union[dict, str]] = None):
         """
+        Authentication with an OpenAPI service.
+
         Authenticates with the OpenAPI service if required, supporting both single (str) and multiple
         authentication methods (dict).
 
         OpenAPI spec v3 supports the following security schemes:
         http – for Basic, Bearer and other HTTP authentications schemes
         apiKey – for API keys and cookie authentication
         oauth2 – for OAuth 2
@@ -197,16 +203,17 @@
                 raise ValueError(
                     f"Service {service_name} requires authentication but no credentials were provided "
                     f"for it. Check the service configuration and credentials."
                 )
 
     def _invoke_method(self, openapi_service: OpenAPI, method_invocation_descriptor: Dict[str, Any]) -> Any:
         """
-        Invokes the specified method on the OpenAPI service. The method name and arguments are passed in the
-        method_invocation_descriptor.
+        Invokes the specified method on the OpenAPI service.
+
+        The method name and arguments are passed in the method_invocation_descriptor.
 
         :param openapi_service: The OpenAPI service instance.
         :param method_invocation_descriptor: The method name and arguments to be passed to the method. The payload
         should contain the method name (key: "name") and the arguments (key: "arguments"). The name is a string, and
         the arguments are a dictionary of key-value pairs.
         :return: A service JSON response.
         :raises RuntimeError: If the method is not found or invocation fails.
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/converters/__init__.py` & `haystack_ai-2.1.0rc1/haystack/components/converters/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from haystack.components.converters.azure import AzureOCRDocumentConverter
 from haystack.components.converters.html import HTMLToDocument
 from haystack.components.converters.markdown import MarkdownToDocument
 from haystack.components.converters.openapi_functions import OpenAPIServiceToFunctions
 from haystack.components.converters.output_adapter import OutputAdapter
+from haystack.components.converters.pdfminer import PDFMinerToDocument
 from haystack.components.converters.pypdf import PyPDFToDocument
 from haystack.components.converters.tika import TikaDocumentConverter
 from haystack.components.converters.txt import TextFileToDocument
 
 __all__ = [
     "TextFileToDocument",
     "TikaDocumentConverter",
     "AzureOCRDocumentConverter",
     "PyPDFToDocument",
+    "PDFMinerToDocument",
     "HTMLToDocument",
     "MarkdownToDocument",
     "OpenAPIServiceToFunctions",
     "OutputAdapter",
 ]
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/converters/azure.py` & `haystack_ai-2.1.0rc1/haystack/components/websearch/serper_dev.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,149 +1,172 @@
-from pathlib import Path
+import json
 from typing import Any, Dict, List, Optional, Union
 
-from haystack import Document, component, default_from_dict, default_to_dict, logging
-from haystack.components.converters.utils import get_bytestream_from_source, normalize_metadata
-from haystack.dataclasses import ByteStream
-from haystack.lazy_imports import LazyImport
+import requests
+
+from haystack import ComponentError, Document, component, default_from_dict, default_to_dict, logging
 from haystack.utils import Secret, deserialize_secrets_inplace
 
 logger = logging.getLogger(__name__)
 
-with LazyImport(message="Run 'pip install \"azure-ai-formrecognizer>=3.2.0b2\"'") as azure_import:
-    from azure.ai.formrecognizer import AnalyzeResult, DocumentAnalysisClient
-    from azure.core.credentials import AzureKeyCredential
+
+SERPERDEV_BASE_URL = "https://google.serper.dev/search"
+
+
+class SerperDevError(ComponentError):
+    ...
 
 
 @component
-class AzureOCRDocumentConverter:
+class SerperDevWebSearch:
     """
-    A component for converting files to Documents using Azure's Document Intelligence service.
-    Supported file formats are: PDF, JPEG, PNG, BMP, TIFF, DOCX, XLSX, PPTX, and HTML.
+    Uses [Serper](https://serper.dev/) to search the web for relevant documents.
 
-    In order to be able to use this component, you need an active Azure account
-    and a Document Intelligence or Cognitive Services resource. Follow the steps described in the
-    [Azure documentation](https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/quickstarts/get-started-sdks-rest-api)
-    to set up your resource.
+    See the [Serper Dev website](https://serper.dev/) for more details.
 
     Usage example:
     ```python
-    from haystack.components.converters import AzureOCRDocumentConverter
+    from haystack.components.websearch import SerperDevWebSearch
     from haystack.utils import Secret
 
-    converter = AzureOCRDocumentConverter(endpoint="<url>", api_key=Secret.from_token("<your-api-key>"))
-    results = converter.run(sources=["path/to/document_with_images.pdf"], meta={"date_added": datetime.now().isoformat()})
-    documents = results["documents"]
-    print(documents[0].content)
-    # 'This is a text from the PDF file.'
+    websearch = SerperDevWebSearch(top_k=10, api_key=Secret.from_token("test-api-key"))
+    results = websearch.run(query="Who is the boyfriend of Olivia Wilde?")
+
+    assert results["documents"]
+    assert results["links"]
     ```
     """
 
     def __init__(
-        self, endpoint: str, api_key: Secret = Secret.from_env_var("AZURE_AI_API_KEY"), model_id: str = "prebuilt-read"
+        self,
+        api_key: Secret = Secret.from_env_var("SERPERDEV_API_KEY"),
+        top_k: Optional[int] = 10,
+        allowed_domains: Optional[List[str]] = None,
+        search_params: Optional[Dict[str, Any]] = None,
     ):
         """
-        Create an AzureOCRDocumentConverter component.
-
-        :param endpoint:
-            The endpoint of your Azure resource.
-        :param api_key:
-            The key of your Azure resource.
-        :param model_id:
-            The model ID of the model you want to use. Please refer to [Azure documentation](https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/choose-model-feature)
-            for a list of available models. Default: `"prebuilt-read"`.
-        """
-        azure_import.check()
-
-        self.document_analysis_client = DocumentAnalysisClient(endpoint=endpoint, credential=AzureKeyCredential(api_key.resolve_value()))  # type: ignore
-        self.endpoint = endpoint
-        self.model_id = model_id
-        self.api_key = api_key
+        Initialize the SerperDevWebSearch component.
 
-    @component.output_types(documents=List[Document], raw_azure_response=List[Dict])
-    def run(self, sources: List[Union[str, Path, ByteStream]], meta: Optional[List[Dict[str, Any]]] = None):
+        :param api_key: API key for the Serper API.
+        :param top_k: Number of documents to return.
+        :param allowed_domains: List of domains to limit the search to.
+        :param search_params: Additional parameters passed to the Serper API.
+            For example, you can set 'num' to 20 to increase the number of search results.
+            See the [Serper website](https://serper.dev/) for more details.
         """
-        Convert a list of files to Documents using Azure's Document Intelligence service.
-
-        :param sources:
-            List of file paths or ByteStream objects.
-        :param meta:
-            Optional metadata to attach to the Documents.
-            This value can be either a list of dictionaries or a single dictionary.
-            If it's a single dictionary, its content is added to the metadata of all produced Documents.
-            If it's a list, the length of the list must match the number of sources, because the two lists will be zipped.
-            If `sources` contains ByteStream objects, their `meta` will be added to the output Documents.
-
-        :returns:
-            A dictionary with the following keys:
-            - `documents`: List of created Documents
-            - `raw_azure_response`: List of raw Azure responses used to create the Documents
-        """
-        documents = []
-        azure_output = []
-        meta_list = normalize_metadata(meta=meta, sources_count=len(sources))
-
-        for source, metadata in zip(sources, meta_list):
-            try:
-                bytestream = get_bytestream_from_source(source=source)
-            except Exception as e:
-                logger.warning("Could not read {source}. Skipping it. Error: {error}", source=source, error=e)
-                continue
-
-            poller = self.document_analysis_client.begin_analyze_document(
-                model_id=self.model_id, document=bytestream.data
-            )
-            result = poller.result()
-            azure_output.append(result.to_dict())
-
-            file_suffix = None
-            if "file_path" in bytestream.meta:
-                file_suffix = Path(bytestream.meta["file_path"]).suffix
-
-            document = AzureOCRDocumentConverter._convert_azure_result_to_document(result, file_suffix)
-            merged_metadata = {**bytestream.meta, **metadata}
-            document.meta = merged_metadata
-            documents.append(document)
+        self.api_key = api_key
+        self.top_k = top_k
+        self.allowed_domains = allowed_domains
+        self.search_params = search_params or {}
 
-        return {"documents": documents, "raw_azure_response": azure_output}
+        # Ensure that the API key is resolved.
+        _ = self.api_key.resolve_value()
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
         :returns:
-            Dictionary with serialized data.
+                Dictionary with serialized data.
         """
-        return default_to_dict(self, api_key=self.api_key.to_dict(), endpoint=self.endpoint, model_id=self.model_id)
+        return default_to_dict(
+            self,
+            top_k=self.top_k,
+            allowed_domains=self.allowed_domains,
+            search_params=self.search_params,
+            api_key=self.api_key.to_dict(),
+        )
 
     @classmethod
-    def from_dict(cls, data: Dict[str, Any]) -> "AzureOCRDocumentConverter":
+    def from_dict(cls, data: Dict[str, Any]) -> "SerperDevWebSearch":
         """
-        Deserializes the component from a dictionary.
+        Serializes the component to a dictionary.
 
-        :param data:
-            The dictionary to deserialize from.
         :returns:
-            The deserialized component.
+                Dictionary with serialized data.
         """
         deserialize_secrets_inplace(data["init_parameters"], keys=["api_key"])
         return default_from_dict(cls, data)
 
-    @staticmethod
-    def _convert_azure_result_to_document(result: "AnalyzeResult", file_suffix: Optional[str] = None) -> Document:
+    @component.output_types(documents=List[Document], links=List[str])
+    def run(self, query: str) -> Dict[str, Union[List[Document], List[str]]]:
         """
-        Convert the result of Azure OCR to a Haystack text Document.
-        """
-        if file_suffix == ".pdf":
-            text = ""
-            for page in result.pages:
-                lines = page.lines if page.lines else []
-                for line in lines:
-                    text += f"{line.content}\n"
-
-                text += "\f"
-        else:
-            text = result.content
-
-        document = Document(content=text)
+        Use [Serper](https://serper.dev/) to search the web.
 
-        return document
+        :param query: Search query.
+        :returns: A dictionary with the following keys:
+            - "documents": List of documents returned by the search engine.
+            - "links": List of links returned by the search engine.
+        :raises SerperDevError: If an error occurs while querying the SerperDev API.
+        :raises TimeoutError: If the request to the SerperDev API times out.
+        """
+        query_prepend = "OR ".join(f"site:{domain} " for domain in self.allowed_domains) if self.allowed_domains else ""
+
+        payload = json.dumps(
+            {"q": query_prepend + query, "gl": "us", "hl": "en", "autocorrect": True, **self.search_params}
+        )
+        headers = {"X-API-KEY": self.api_key.resolve_value(), "Content-Type": "application/json"}
+
+        try:
+            response = requests.post(SERPERDEV_BASE_URL, headers=headers, data=payload, timeout=30)  # type: ignore
+            response.raise_for_status()  # Will raise an HTTPError for bad responses
+        except requests.Timeout as error:
+            raise TimeoutError(f"Request to {self.__class__.__name__} timed out.") from error
+
+        except requests.RequestException as e:
+            raise SerperDevError(f"An error occurred while querying {self.__class__.__name__}. Error: {e}") from e
+
+        # If we reached this point, it means the request was successful and we can proceed
+        json_result = response.json()
+
+        # we get the snippet from the json result and put it in the content field of the document
+        organic = [
+            Document(meta={k: v for k, v in d.items() if k != "snippet"}, content=d["snippet"])
+            for d in json_result["organic"]
+        ]
+
+        # answer box is what search engine shows as a direct answer to the query
+        answer_box = []
+        if "answerBox" in json_result:
+            answer_dict = json_result["answerBox"]
+            highlighted_answers = answer_dict.get("snippetHighlighted")
+            answer_box_content = None
+            # Check if highlighted_answers is a list and has at least one element
+            if isinstance(highlighted_answers, list) and len(highlighted_answers) > 0:
+                answer_box_content = highlighted_answers[0]
+            elif isinstance(highlighted_answers, str):
+                answer_box_content = highlighted_answers
+            if not answer_box_content:
+                for key in ["snippet", "answer", "title"]:
+                    if key in answer_dict:
+                        answer_box_content = answer_dict[key]
+                        break
+            if answer_box_content:
+                answer_box = [
+                    Document(
+                        content=answer_box_content,
+                        meta={"title": answer_dict.get("title", ""), "link": answer_dict.get("link", "")},
+                    )
+                ]
+
+        # these are related questions that search engine shows
+        people_also_ask = []
+        if "peopleAlsoAsk" in json_result:
+            for result in json_result["peopleAlsoAsk"]:
+                title = result.get("title", "")
+                people_also_ask.append(
+                    Document(
+                        content=result["snippet"] if result.get("snippet") else title,
+                        meta={"title": title, "link": result.get("link", None)},
+                    )
+                )
+
+        documents = answer_box + organic + people_also_ask
+
+        links = [result["link"] for result in json_result["organic"]]
+
+        logger.debug(
+            "Serper Dev returned {number_documents} documents for the query '{query}'",
+            number_documents=len(documents),
+            query=query,
+        )
+        return {"documents": documents[: self.top_k], "links": links[: self.top_k]}
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/converters/html.py` & `haystack_ai-2.1.0rc1/haystack/components/converters/html.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Any, Dict, List, Literal, Optional, Union
+from typing import Any, ClassVar, Dict, List, Literal, Optional, Union
 
 from boilerpy3 import extractors
 
 from haystack import Document, component, default_from_dict, default_to_dict, logging
 from haystack.components.converters.utils import get_bytestream_from_source, normalize_metadata
 from haystack.dataclasses import ByteStream
 
@@ -23,44 +23,57 @@
     results = converter.run(sources=["path/to/sample.html"])
     documents = results["documents"]
     print(documents[0].content)
     # 'This is a text from the HTML file.'
     ```
     """
 
+    known_extractors: ClassVar[List[str]] = [
+        "DefaultExtractor",
+        "ArticleExtractor",
+        "ArticleSentencesExtractor",
+        "LargestContentExtractor",
+        "CanolaExtractor",
+        "KeepEverythingExtractor",
+        "NumWordsRulesExtractor",
+    ]
+
     def __init__(
         self,
         extractor_type: Literal[
             "DefaultExtractor",
             "ArticleExtractor",
             "ArticleSentencesExtractor",
             "LargestContentExtractor",
             "CanolaExtractor",
             "KeepEverythingExtractor",
             "NumWordsRulesExtractor",
         ] = "DefaultExtractor",
+        try_others: bool = True,
     ):
         """
         Create an HTMLToDocument component.
 
         :param
             extractor_type: Name of the extractor class to use. Defaults to `DefaultExtractor`.
             For more information on the different types of extractors,
             see [boilerpy3 documentation](https://github.com/jmriebold/BoilerPy3?tab=readme-ov-file#extractors).
+        :param try_others: If `True`, the component will try other extractors if the user chosen extractor fails.
         """
         self.extractor_type = extractor_type
+        self.try_others = try_others
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
         :returns:
             Dictionary with serialized data.
         """
-        return default_to_dict(self, extractor_type=self.extractor_type)
+        return default_to_dict(self, extractor_type=self.extractor_type, try_others=self.try_others)
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "HTMLToDocument":
         """
         Deserializes the component from a dictionary.
 
         :param data:
@@ -92,32 +105,53 @@
             A dictionary with the following keys:
             - `documents`: Created Documents
         """
 
         documents = []
         meta_list = normalize_metadata(meta=meta, sources_count=len(sources))
 
-        extractor_class = getattr(extractors, self.extractor_type)
-        extractor = extractor_class(raise_on_failure=False)
+        # Use all extractor types, ensuring user chosen extractor is first, preserve order, avoid duplicates
+        extractors_list = (
+            list(
+                dict.fromkeys(
+                    [self.extractor_type, *self.known_extractors]  # User chosen extractor is always tried first
+                )
+            )
+            if self.try_others
+            else [self.extractor_type]
+        )
 
         for source, metadata in zip(sources, meta_list):
             try:
                 bytestream = get_bytestream_from_source(source=source)
             except Exception as e:
                 logger.warning("Could not read {source}. Skipping it. Error: {error}", source=source, error=e)
                 continue
-            try:
-                file_content = bytestream.data.decode("utf-8")
-                text = extractor.get_content(file_content)
-            except Exception as conversion_e:
+
+            text = None
+            for extractor_name in extractors_list:
+                extractor_class = getattr(extractors, extractor_name)
+                extractor = extractor_class(raise_on_failure=False)
+                try:
+                    text = extractor.get_content(bytestream.data.decode("utf-8"))
+                    if text:
+                        break
+                except Exception as conversion_e:
+                    if self.try_others:
+                        logger.warning(
+                            "Failed to extract text using {extractor} from {source}. Trying next extractor. Error: {error}",
+                            extractor=extractor_name,
+                            source=source,
+                            error=conversion_e,
+                        )
+            if not text:
                 logger.warning(
-                    "Failed to extract text from {source}. Skipping it. Error: {error}",
+                    f"Failed to extract text from {source} using extractors: {extractors_list}. Skipping it.",
                     source=source,
-                    error=conversion_e,
+                    extractors_list=extractors_list,
                 )
                 continue
 
-            merged_metadata = {**bytestream.meta, **metadata}
-            document = Document(content=text, meta=merged_metadata)
+            document = Document(content=text, meta={**bytestream.meta, **metadata})
             documents.append(document)
 
         return {"documents": documents}
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/converters/markdown.py` & `haystack_ai-2.1.0rc1/haystack/components/converters/markdown.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/components/converters/openapi_functions.py` & `haystack_ai-2.1.0rc1/haystack/components/converters/openapi_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,14 +108,16 @@
         if not all_extracted_fc_definitions:
             logger.warning("No OpenAI function definitions extracted from the provided OpenAPI specification sources.")
 
         return {"functions": all_extracted_fc_definitions, "openapi_specs": all_openapi_specs}
 
     def _openapi_to_functions(self, service_openapi_spec: Dict[str, Any]) -> List[Dict[str, Any]]:
         """
+        OpenAPI to OpenAI function conversion.
+
         Extracts functions from the OpenAPI specification of the service and converts them into a format
         suitable for OpenAI function calling.
 
         :param service_openapi_spec: The OpenAPI specification from which functions are to be extracted.
         :type service_openapi_spec: Dict[str, Any]
         :return: A list of dictionaries, each representing a function. Each dictionary includes the function's
                  name, description, and a schema of its parameters.
@@ -184,14 +186,16 @@
             )
             return {}
 
     def _parse_property_attributes(
         self, property_schema: Dict[str, Any], include_attributes: Optional[List[str]] = None
     ) -> Dict[str, Any]:
         """
+        Parses the attributes of a property schema.
+
         Recursively parses the attributes of a property schema, including nested objects and arrays,
         and includes specified attributes like description, pattern, etc.
 
         :param property_schema: The schema of the property to parse.
         :param include_attributes: The list of attributes to include in the parsed schema.
         :return: The parsed schema of the property including the specified attributes.
         """
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/converters/output_adapter.py` & `haystack_ai-2.1.0rc1/haystack/components/converters/output_adapter.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/components/converters/pypdf.py` & `haystack_ai-2.1.0rc1/haystack/components/converters/pypdf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,64 @@
 import io
+import warnings
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Protocol, Union
 
-from haystack import Document, component, default_to_dict, logging
+from haystack import Document, component, default_from_dict, default_to_dict, logging
 from haystack.components.converters.utils import get_bytestream_from_source, normalize_metadata
 from haystack.dataclasses import ByteStream
 from haystack.lazy_imports import LazyImport
+from haystack.utils.type_serialization import deserialize_type
 
 with LazyImport("Run 'pip install pypdf'") as pypdf_import:
     from pypdf import PdfReader
 
 
 logger = logging.getLogger(__name__)
 
 
 class PyPDFConverter(Protocol):
     """
     A protocol that defines a converter which takes a PdfReader object and converts it into a Document object.
     """
 
-    def convert(self, reader: "PdfReader") -> Document:
+    def convert(self, reader: "PdfReader") -> Document:  # noqa: D102
+        ...
+
+    def to_dict(self):  # noqa: D102
+        ...
+
+    @classmethod
+    def from_dict(cls, data):  # noqa: D102
         ...
 
 
 class DefaultConverter:
     """
     The default converter class that extracts text from a PdfReader object's pages and returns a Document.
     """
 
     def convert(self, reader: "PdfReader") -> Document:
         """Extract text from the PDF and return a Document object with the text content."""
         text = "\f".join(page.extract_text() for page in reader.pages)
         return Document(content=text)
 
+    def to_dict(self):
+        """Serialize the converter to a dictionary."""
+        return default_to_dict(self)
+
+    @classmethod
+    def from_dict(cls, data):
+        """Deserialize the converter from a dictionary."""
+        return default_from_dict(cls, data)
+
 
 # This registry is used to store converters names and instances.
 # It can be used to register custom converters.
+# It is now deprecated and will be removed in Haystack 2.3.0.
 CONVERTERS_REGISTRY: Dict[str, PyPDFConverter] = {"default": DefaultConverter()}
 
 
 @component
 class PyPDFToDocument:
     """
     Converts PDF files to Documents.
@@ -55,42 +74,74 @@
     results = converter.run(sources=["sample.pdf"], meta={"date_added": datetime.now().isoformat()})
     documents = results["documents"]
     print(documents[0].content)
     # 'This is a text from the PDF file.'
     ```
     """
 
-    def __init__(self, converter_name: str = "default"):
+    def __init__(self, converter_name: Optional[str] = None, converter: Optional[PyPDFConverter] = None):
         """
         Create an PyPDFToDocument component.
 
         :param converter_name:
-            Name of the registered converter to use.
+            The name of a PyPDFConverter instance stored in the CONVERTERS_REGISTRY. Deprecated.
+        :param converter:
+            An instance of a PyPDFConverter compatible class.
         """
         pypdf_import.check()
 
-        try:
-            converter = CONVERTERS_REGISTRY[converter_name]
-        except KeyError:
-            msg = (
-                f"Invalid converter_name: {converter_name}.\n Available converters: {list(CONVERTERS_REGISTRY.keys())}"
-            )
-            raise ValueError(msg) from KeyError
         self.converter_name = converter_name
-        self._converter: PyPDFConverter = converter
+        if converter_name:
+            warnings.warn(
+                "The `converter_name` parameter is deprecated and will be removed in Haystack 2.3.0. "
+                "Please use the `converter` parameter instead.",
+                DeprecationWarning,
+            )
+            try:
+                converter = CONVERTERS_REGISTRY[converter_name]
+            except KeyError:
+                msg = (
+                    f"Invalid converter_name: {converter_name}.\n Available converters: {list(CONVERTERS_REGISTRY.keys())}"
+                    f"To specify a custom converter, it is recommended to use the `converter` parameter."
+                )
+                raise ValueError(msg) from KeyError
+
+            self.converter = converter
+
+        elif converter:
+            self.converter = converter
+        else:
+            self.converter = DefaultConverter()
 
     def to_dict(self):
         """
         Serializes the component to a dictionary.
 
         :returns:
             Dictionary with serialized data.
         """
-        # do not serialize the _converter instance
-        return default_to_dict(self, converter_name=self.converter_name)
+        return default_to_dict(self, converter_name=self.converter_name, converter=self.converter.to_dict())
+
+    @classmethod
+    def from_dict(cls, data):
+        """
+        Deserializes the component from a dictionary.
+
+        :param data:
+            Dictionary with serialized data.
+
+        :returns:
+            Deserialized component.
+        """
+        if data["init_parameters"].get("converter_name"):
+            return default_from_dict(cls, data)
+
+        converter_class = deserialize_type(data["init_parameters"]["converter"]["type"])
+        data["init_parameters"]["converter"] = converter_class.from_dict(data["init_parameters"]["converter"])
+        return default_from_dict(cls, data)
 
     @component.output_types(documents=List[Document])
     def run(
         self,
         sources: List[Union[str, Path, ByteStream]],
         meta: Optional[Union[Dict[str, Any], List[Dict[str, Any]]]] = None,
     ):
@@ -117,15 +168,15 @@
             try:
                 bytestream = get_bytestream_from_source(source)
             except Exception as e:
                 logger.warning("Could not read {source}. Skipping it. Error: {error}", source=source, error=e)
                 continue
             try:
                 pdf_reader = PdfReader(io.BytesIO(bytestream.data))
-                document = self._converter.convert(pdf_reader)
+                document = self.converter.convert(pdf_reader)
             except Exception as e:
                 logger.warning(
                     "Could not read {source} and convert it to Document, skipping. {error}", source=source, error=e
                 )
                 continue
 
             merged_metadata = {**bytestream.meta, **metadata}
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/converters/tika.py` & `haystack_ai-2.1.0rc1/haystack/components/converters/tika.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/components/converters/txt.py` & `haystack_ai-2.1.0rc1/haystack/components/converters/txt.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/components/converters/utils.py` & `haystack_ai-2.1.0rc1/haystack/components/converters/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from haystack.dataclasses import ByteStream
 
 
 def get_bytestream_from_source(source: Union[str, Path, ByteStream]) -> ByteStream:
     """
     Creates a ByteStream object from a source.
+
     :param source: A source to convert to a ByteStream. Can be a string (path to a file), a Path object, or a ByteStream.
     :return: A ByteStream object.
     """
 
     if isinstance(source, ByteStream):
         return source
     if isinstance(source, (str, Path)):
@@ -20,14 +21,16 @@
     raise ValueError(f"Unsupported source type {type(source)}")
 
 
 def normalize_metadata(
     meta: Optional[Union[Dict[str, Any], List[Dict[str, Any]]]], sources_count: int
 ) -> List[Dict[str, Any]]:
     """
+    Normalize the metadata input for a converter.
+
     Given all the possible value of the meta input for a converter (None, dictionary or list of dicts),
     makes sure to return a list of dictionaries of the correct length for the converter to use.
 
     :param meta: the meta input of the converter, as-is
     :param sources_count: the number of sources the converter received
     :returns: a list of dictionaries of the make length as the sources list
     """
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/embedders/azure_document_embedder.py` & `haystack_ai-2.1.0rc1/haystack/components/embedders/azure_document_embedder.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     """
 
     def __init__(
         self,
         azure_endpoint: Optional[str] = None,
         api_version: Optional[str] = "2023-05-15",
         azure_deployment: str = "text-embedding-ada-002",
+        dimensions: Optional[int] = None,
         api_key: Optional[Secret] = Secret.from_env_var("AZURE_OPENAI_API_KEY", strict=False),
         azure_ad_token: Optional[Secret] = Secret.from_env_var("AZURE_OPENAI_AD_TOKEN", strict=False),
         organization: Optional[str] = None,
         prefix: str = "",
         suffix: str = "",
         batch_size: int = 32,
         progress_bar: bool = True,
@@ -49,14 +50,16 @@
 
         :param azure_endpoint:
             The endpoint of the deployed model.
         :param api_version:
             The version of the API to use.
         :param azure_deployment:
             The deployment of the model, usually matches the model name.
+        :param dimensions:
+            The number of dimensions the resulting output embeddings should have. Only supported in text-embedding-3 and later models.
         :param api_key:
             The API key used for authentication.
         :param azure_ad_token:
             Microsoft Entra ID token, see Microsoft's official
             [Entra ID](https://www.microsoft.com/en-us/security/business/identity-access/microsoft-entra-id)
             documentation for more information.
             Used to be called Azure Active Directory.
@@ -86,14 +89,15 @@
             raise ValueError("Please provide an API key or an Azure Active Directory token.")
 
         self.api_key = api_key
         self.azure_ad_token = azure_ad_token
         self.api_version = api_version
         self.azure_endpoint = azure_endpoint
         self.azure_deployment = azure_deployment
+        self.dimensions = dimensions
         self.organization = organization
         self.prefix = prefix
         self.suffix = suffix
         self.batch_size = batch_size
         self.progress_bar = progress_bar
         self.meta_fields_to_embed = meta_fields_to_embed or []
         self.embedding_separator = embedding_separator
@@ -120,14 +124,15 @@
         :returns:
             Dictionary with serialized data.
         """
         return default_to_dict(
             self,
             azure_endpoint=self.azure_endpoint,
             azure_deployment=self.azure_deployment,
+            dimensions=self.dimensions,
             organization=self.organization,
             api_version=self.api_version,
             prefix=self.prefix,
             suffix=self.suffix,
             batch_size=self.batch_size,
             progress_bar=self.progress_bar,
             meta_fields_to_embed=self.meta_fields_to_embed,
@@ -171,15 +176,20 @@
         Embed a list of texts in batches.
         """
 
         all_embeddings: List[List[float]] = []
         meta: Dict[str, Any] = {"model": "", "usage": {"prompt_tokens": 0, "total_tokens": 0}}
         for i in tqdm(range(0, len(texts_to_embed), batch_size), desc="Embedding Texts"):
             batch = texts_to_embed[i : i + batch_size]
-            response = self._client.embeddings.create(model=self.azure_deployment, input=batch)
+            if self.dimensions is not None:
+                response = self._client.embeddings.create(
+                    model=self.azure_deployment, dimensions=self.dimensions, input=batch
+                )
+            else:
+                response = self._client.embeddings.create(model=self.azure_deployment, input=batch)
 
             # Append embeddings to the list
             all_embeddings.extend(el.embedding for el in response.data)
 
             # Update the meta information only once if it's empty
             if not meta["model"]:
                 meta["model"] = response.model
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/embedders/azure_text_embedder.py` & `haystack_ai-2.1.0rc1/haystack/components/embedders/azure_text_embedder.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     """
 
     def __init__(
         self,
         azure_endpoint: Optional[str] = None,
         api_version: Optional[str] = "2023-05-15",
         azure_deployment: str = "text-embedding-ada-002",
+        dimensions: Optional[int] = None,
         api_key: Optional[Secret] = Secret.from_env_var("AZURE_OPENAI_API_KEY", strict=False),
         azure_ad_token: Optional[Secret] = Secret.from_env_var("AZURE_OPENAI_AD_TOKEN", strict=False),
         organization: Optional[str] = None,
         prefix: str = "",
         suffix: str = "",
     ):
         """
@@ -44,14 +45,16 @@
 
         :param azure_endpoint:
             The endpoint of the deployed model.
         :param api_version:
             The version of the API to use.
         :param azure_deployment:
             The deployment of the model, usually matches the model name.
+        :param dimensions:
+            The number of dimensions the resulting output embeddings should have. Only supported in text-embedding-3 and later models.
         :param api_key:
             The API key used for authentication.
         :param azure_ad_token:
             Microsoft Entra ID token, see Microsoft's official
             [Entra ID](https://www.microsoft.com/en-us/security/business/identity-access/microsoft-entra-id)
             documentation for more information.
             Used to be called Azure Active Directory.
@@ -76,14 +79,15 @@
             raise ValueError("Please provide an API key or an Azure Active Directory token.")
 
         self.api_key = api_key
         self.azure_ad_token = azure_ad_token
         self.api_version = api_version
         self.azure_endpoint = azure_endpoint
         self.azure_deployment = azure_deployment
+        self.dimensions = dimensions
         self.organization = organization
         self.prefix = prefix
         self.suffix = suffix
 
         self._client = AzureOpenAI(
             api_version=api_version,
             azure_endpoint=azure_endpoint,
@@ -106,14 +110,15 @@
         :returns:
             Dictionary with serialized data.
         """
         return default_to_dict(
             self,
             azure_endpoint=self.azure_endpoint,
             azure_deployment=self.azure_deployment,
+            dimensions=self.dimensions,
             organization=self.organization,
             api_version=self.api_version,
             prefix=self.prefix,
             suffix=self.suffix,
             api_key=self.api_key.to_dict() if self.api_key is not None else None,
             azure_ad_token=self.azure_ad_token.to_dict() if self.azure_ad_token is not None else None,
         )
@@ -152,13 +157,18 @@
                 error_message = "Input must be a string."
             raise TypeError(error_message)
 
         # Preprocess the text by adding prefixes/suffixes
         # finally, replace newlines as recommended by OpenAI docs
         processed_text = f"{self.prefix}{text}{self.suffix}".replace("\n", " ")
 
-        response = self._client.embeddings.create(model=self.azure_deployment, input=processed_text)
+        if self.dimensions is not None:
+            response = self._client.embeddings.create(
+                model=self.azure_deployment, dimensions=self.dimensions, input=processed_text
+            )
+        else:
+            response = self._client.embeddings.create(model=self.azure_deployment, input=processed_text)
 
         return {
             "embedding": response.data[0].embedding,
             "meta": {"model": response.model, "usage": dict(response.usage)},
         }
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/embedders/hugging_face_tei_document_embedder.py` & `haystack_ai-2.1.0rc1/haystack/components/embedders/hugging_face_tei_document_embedder.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import json
+import warnings
 from typing import Any, Dict, List, Optional
 from urllib.parse import urlparse
 
 from tqdm import tqdm
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.dataclasses import Document
@@ -46,14 +48,16 @@
     def __init__(
         self,
         model: str = "BAAI/bge-small-en-v1.5",
         url: Optional[str] = None,
         token: Optional[Secret] = Secret.from_env_var("HF_API_TOKEN", strict=False),
         prefix: str = "",
         suffix: str = "",
+        truncate: bool = True,
+        normalize: bool = False,
         batch_size: int = 32,
         progress_bar: bool = True,
         meta_fields_to_embed: Optional[List[str]] = None,
         embedding_separator: str = "\n",
     ):
         """
         Create a HuggingFaceTEIDocumentEmbedder component.
@@ -66,23 +70,38 @@
         :param token:
             The HuggingFace Hub token. This is needed if you are using a paid HF Inference Endpoint or serving
             a private or gated model.
         :param prefix:
             A string to add at the beginning of each text.
         :param suffix:
             A string to add at the end of each text.
+        :param truncate:
+            Truncate input text from the end to the maximum length supported by the model. This option is only available
+            for self-deployed Text Embedding Inference (TEI) endpoints and paid HF Inference Endpoints deployed with
+            TEI. It will be ignored when used with free HF Inference endpoints or paid HF Inference endpoints deployed
+            without TEI.
+        :param normalize:
+            Normalize the embeddings to unit length. This option is only available for self-deployed Text Embedding
+            Inference (TEI) endpoints and paid HF Inference Endpoints deployed with TEI. It will be ignored when used
+            with free HF Inference endpoints or paid HF Inference endpoints deployed without TEI.
         :param batch_size:
             Number of Documents to encode at once.
         :param progress_bar:
             If True shows a progress bar when running.
         :param meta_fields_to_embed:
             List of meta fields that will be embedded along with the Document text.
         :param embedding_separator:
             Separator used to concatenate the meta fields to the Document text.
         """
+        warnings.warn(
+            "`HuggingFaceTEIDocumentEmbedder` is deprecated and will be removed in Haystack 2.3.0."
+            "Use `HuggingFaceAPIDocumentEmbedder` instead.",
+            DeprecationWarning,
+        )
+
         huggingface_hub_import.check()
 
         if url:
             r = urlparse(url)
             is_valid_url = all([r.scheme in ["http", "https"], r.netloc])
             if not is_valid_url:
                 raise ValueError(f"Invalid TEI endpoint URL provided: {url}")
@@ -91,14 +110,16 @@
 
         self.model = model
         self.url = url
         self.token = token
         self.client = InferenceClient(url or model, token=token.resolve_value() if token else None)
         self.prefix = prefix
         self.suffix = suffix
+        self.truncate = truncate
+        self.normalize = normalize
         self.batch_size = batch_size
         self.progress_bar = progress_bar
         self.meta_fields_to_embed = meta_fields_to_embed or []
         self.embedding_separator = embedding_separator
 
     def to_dict(self) -> Dict[str, Any]:
         """
@@ -109,14 +130,16 @@
         """
         return default_to_dict(
             self,
             model=self.model,
             url=self.url,
             prefix=self.prefix,
             suffix=self.suffix,
+            truncate=self.truncate,
+            normalize=self.normalize,
             batch_size=self.batch_size,
             progress_bar=self.progress_bar,
             meta_fields_to_embed=self.meta_fields_to_embed,
             embedding_separator=self.embedding_separator,
             token=self.token.to_dict() if self.token else None,
         )
 
@@ -163,16 +186,20 @@
         """
 
         all_embeddings = []
         for i in tqdm(
             range(0, len(texts_to_embed), batch_size), disable=not self.progress_bar, desc="Calculating embeddings"
         ):
             batch = texts_to_embed[i : i + batch_size]
-            embeddings = self.client.feature_extraction(text=batch)
-            all_embeddings.extend(embeddings.tolist())
+            response = self.client.post(
+                json={"inputs": batch, "truncate": self.truncate, "normalize": self.normalize},
+                task="feature-extraction",
+            )
+            embeddings = json.loads(response.decode())
+            all_embeddings.extend(embeddings)
 
         return all_embeddings
 
     @component.output_types(documents=List[Document])
     def run(self, documents: List[Document]):
         """
         Embed a list of Documents.
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/embedders/hugging_face_tei_text_embedder.py` & `haystack_ai-2.1.0rc1/haystack/components/embedders/openai_text_embedder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,142 +1,139 @@
 from typing import Any, Dict, List, Optional
-from urllib.parse import urlparse
 
-from haystack import component, default_from_dict, default_to_dict, logging
-from haystack.lazy_imports import LazyImport
-from haystack.utils import Secret, deserialize_secrets_inplace
-from haystack.utils.hf import HFModelType, check_valid_model
-
-with LazyImport(message="Run 'pip install \"huggingface_hub>=0.22.0\"'") as huggingface_hub_import:
-    from huggingface_hub import InferenceClient
+from openai import OpenAI
 
-logger = logging.getLogger(__name__)
+from haystack import component, default_from_dict, default_to_dict
+from haystack.utils import Secret, deserialize_secrets_inplace
 
 
 @component
-class HuggingFaceTEITextEmbedder:
+class OpenAITextEmbedder:
     """
-    A component for embedding strings using HuggingFace Text-Embeddings-Inference endpoints.
-
-    This component can be used with embedding models hosted on Hugging Face Inference endpoints, the rate-limited
-    Inference API tier, for embedding models hosted on [the paid inference endpoint](https://huggingface.co/inference-endpoints)
-    and/or your own custom TEI endpoint.
+    A component for embedding strings using OpenAI models.
 
     Usage example:
     ```python
-    from haystack.components.embedders import HuggingFaceTEITextEmbedder
-    from haystack.utils import Secret
+    from haystack.components.embedders import OpenAITextEmbedder
 
     text_to_embed = "I love pizza!"
 
-    text_embedder = HuggingFaceTEITextEmbedder(
-        model="BAAI/bge-small-en-v1.5", token=Secret.from_token("<your-api-key>")
-    )
+    text_embedder = OpenAITextEmbedder()
 
     print(text_embedder.run(text_to_embed))
 
     # {'embedding': [0.017020374536514282, -0.023255806416273117, ...],
+    # 'meta': {'model': 'text-embedding-ada-002-v2',
+    #          'usage': {'prompt_tokens': 4, 'total_tokens': 4}}}
     ```
     """
 
     def __init__(
         self,
-        model: str = "BAAI/bge-small-en-v1.5",
-        url: Optional[str] = None,
-        token: Optional[Secret] = Secret.from_env_var("HF_API_TOKEN", strict=False),
+        api_key: Secret = Secret.from_env_var("OPENAI_API_KEY"),
+        model: str = "text-embedding-ada-002",
+        dimensions: Optional[int] = None,
+        api_base_url: Optional[str] = None,
+        organization: Optional[str] = None,
         prefix: str = "",
         suffix: str = "",
     ):
         """
-        Create an HuggingFaceTEITextEmbedder component.
+        Create an OpenAITextEmbedder component.
 
+        :param api_key:
+            The OpenAI API key.
         :param model:
-            ID of the model on HuggingFace Hub.
-        :param url:
-            The URL of your self-deployed Text-Embeddings-Inference service or the URL of your paid HF Inference
-            Endpoint.
-        :param token:
-            The HuggingFace Hub token. This is needed if you are using a paid HF Inference Endpoint or serving
-            a private or gated model.
+            The name of the model to use.
+        :param dimensions:
+            The number of dimensions the resulting output embeddings should have. Only supported in `text-embedding-3` and later models.
+        :param api_base_url:
+            Overrides default base url for all HTTP requests.
+        :param organization:
+            The Organization ID. See OpenAI's
+            [production best practices](https://platform.openai.com/docs/guides/production-best-practices/setting-up-your-organization)
+            for more information.
         :param prefix:
             A string to add at the beginning of each text.
         :param suffix:
             A string to add at the end of each text.
         """
-        huggingface_hub_import.check()
-
-        if url:
-            r = urlparse(url)
-            is_valid_url = all([r.scheme in ["http", "https"], r.netloc])
-            if not is_valid_url:
-                raise ValueError(f"Invalid TEI endpoint URL provided: {url}")
-
-        check_valid_model(model, HFModelType.EMBEDDING, token)
-
         self.model = model
-        self.url = url
-        self.token = token
-        self.client = InferenceClient(url or model, token=token.resolve_value() if token else None)
+        self.dimensions = dimensions
+        self.api_base_url = api_base_url
+        self.organization = organization
         self.prefix = prefix
         self.suffix = suffix
+        self.api_key = api_key
+
+        self.client = OpenAI(api_key=api_key.resolve_value(), organization=organization, base_url=api_base_url)
+
+    def _get_telemetry_data(self) -> Dict[str, Any]:
+        """
+        Data that is sent to Posthog for usage analytics.
+        """
+        return {"model": self.model}
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
         :returns:
             Dictionary with serialized data.
         """
         return default_to_dict(
             self,
             model=self.model,
-            url=self.url,
+            api_base_url=self.api_base_url,
+            organization=self.organization,
             prefix=self.prefix,
             suffix=self.suffix,
-            token=self.token.to_dict() if self.token else None,
+            dimensions=self.dimensions,
+            api_key=self.api_key.to_dict(),
         )
 
     @classmethod
-    def from_dict(cls, data: Dict[str, Any]) -> "HuggingFaceTEITextEmbedder":
+    def from_dict(cls, data: Dict[str, Any]) -> "OpenAITextEmbedder":
         """
         Deserializes the component from a dictionary.
 
         :param data:
             Dictionary to deserialize from.
         :returns:
             Deserialized component.
         """
-        deserialize_secrets_inplace(data["init_parameters"], keys=["token"])
+        deserialize_secrets_inplace(data["init_parameters"], keys=["api_key"])
         return default_from_dict(cls, data)
 
-    def _get_telemetry_data(self) -> Dict[str, Any]:
-        """
-        Data that is sent to Posthog for usage analytics.
-        """
-        # Don't send URL as it is sensitive information
-        return {"model": self.model}
-
-    @component.output_types(embedding=List[float])
+    @component.output_types(embedding=List[float], meta=Dict[str, Any])
     def run(self, text: str):
         """
         Embed a single string.
 
         :param text:
             Text to embed.
 
         :returns:
             A dictionary with the following keys:
             - `embedding`: The embedding of the input text.
+            - `meta`: Information about the usage of the model.
         """
         if not isinstance(text, str):
             raise TypeError(
-                "HuggingFaceTEITextEmbedder expects a string as an input."
-                "In case you want to embed a list of Documents, please use the HuggingFaceTEIDocumentEmbedder."
+                "OpenAITextEmbedder expects a string as an input."
+                "In case you want to embed a list of Documents, please use the OpenAIDocumentEmbedder."
             )
 
         text_to_embed = self.prefix + text + self.suffix
 
-        embeddings = self.client.feature_extraction(text=[text_to_embed])
-        # The client returns a numpy array
-        embedding = embeddings.tolist()[0]
+        # copied from OpenAI embedding_utils (https://github.com/openai/openai-python/blob/main/openai/embeddings_utils.py)
+        # replace newlines, which can negatively affect performance.
+        text_to_embed = text_to_embed.replace("\n", " ")
+
+        if self.dimensions is not None:
+            response = self.client.embeddings.create(model=self.model, dimensions=self.dimensions, input=text_to_embed)
+        else:
+            response = self.client.embeddings.create(model=self.model, input=text_to_embed)
+
+        meta = {"model": response.model, "usage": dict(response.usage)}
 
-        return {"embedding": embedding}
+        return {"embedding": response.data[0].embedding, "meta": meta}
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/embedders/openai_document_embedder.py` & `haystack_ai-2.1.0rc1/haystack/components/embedders/openai_document_embedder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/components/embedders/openai_text_embedder.py` & `haystack_ai-2.1.0rc1/haystack/components/embedders/sentence_transformers_text_embedder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,83 @@
 from typing import Any, Dict, List, Optional
 
-from openai import OpenAI
-
 from haystack import component, default_from_dict, default_to_dict
-from haystack.utils import Secret, deserialize_secrets_inplace
+from haystack.components.embedders.backends.sentence_transformers_backend import (
+    _SentenceTransformersEmbeddingBackendFactory,
+)
+from haystack.utils import ComponentDevice, Secret, deserialize_secrets_inplace
 
 
 @component
-class OpenAITextEmbedder:
+class SentenceTransformersTextEmbedder:
     """
-    A component for embedding strings using OpenAI models.
+    A component for embedding strings using Sentence Transformers models.
 
     Usage example:
     ```python
-    from haystack.components.embedders import OpenAITextEmbedder
+    from haystack.components.embedders import SentenceTransformersTextEmbedder
 
     text_to_embed = "I love pizza!"
 
-    text_embedder = OpenAITextEmbedder()
+    text_embedder = SentenceTransformersTextEmbedder()
+    text_embedder.warm_up()
 
     print(text_embedder.run(text_to_embed))
 
-    # {'embedding': [0.017020374536514282, -0.023255806416273117, ...],
-    # 'meta': {'model': 'text-embedding-ada-002-v2',
-    #          'usage': {'prompt_tokens': 4, 'total_tokens': 4}}}
+    # {'embedding': [-0.07804739475250244, 0.1498992145061493,, ...]}
     ```
     """
 
     def __init__(
         self,
-        api_key: Secret = Secret.from_env_var("OPENAI_API_KEY"),
-        model: str = "text-embedding-ada-002",
-        dimensions: Optional[int] = None,
-        api_base_url: Optional[str] = None,
-        organization: Optional[str] = None,
+        model: str = "sentence-transformers/all-mpnet-base-v2",
+        device: Optional[ComponentDevice] = None,
+        token: Optional[Secret] = Secret.from_env_var("HF_API_TOKEN", strict=False),
         prefix: str = "",
         suffix: str = "",
+        batch_size: int = 32,
+        progress_bar: bool = True,
+        normalize_embeddings: bool = False,
+        trust_remote_code: bool = False,
     ):
         """
-        Create an OpenAITextEmbedder component.
+        Create a SentenceTransformersTextEmbedder component.
 
-        :param api_key:
-            The OpenAI API key.
         :param model:
-            The name of the model to use.
-        :param dimensions:
-            The number of dimensions the resulting output embeddings should have. Only supported in `text-embedding-3` and later models.
-        :param api_base_url:
-            Overrides default base url for all HTTP requests.
-        :param organization:
-            The Organization ID. See OpenAI's
-            [production best practices](https://platform.openai.com/docs/guides/production-best-practices/setting-up-your-organization)
-            for more information.
+            Local path or ID of the model on HuggingFace Hub.
+        :param device:
+            Overrides the default device used to load the model.
+        :param token:
+            The API token used to download private models from Hugging Face.
         :param prefix:
             A string to add at the beginning of each text.
+            Can be used to prepend the text with an instruction, as required by some embedding models,
+            such as E5 and bge.
         :param suffix:
             A string to add at the end of each text.
+        :param batch_size:
+            Number of Documents to encode at once.
+        :param progress_bar:
+            If True shows a progress bar when running.
+        :param normalize_embeddings:
+            If True returned vectors will have length 1.
+        :param trust_remote_code:
+            If `False`, only Hugging Face verified model architectures are allowed.
+            If `True`, custom models and scripts are allowed.
         """
+
         self.model = model
-        self.dimensions = dimensions
-        self.api_base_url = api_base_url
-        self.organization = organization
+        self.device = ComponentDevice.resolve_device(device)
+        self.token = token
         self.prefix = prefix
         self.suffix = suffix
-        self.api_key = api_key
-
-        self.client = OpenAI(api_key=api_key.resolve_value(), organization=organization, base_url=api_base_url)
+        self.batch_size = batch_size
+        self.progress_bar = progress_bar
+        self.normalize_embeddings = normalize_embeddings
+        self.trust_remote_code = trust_remote_code
 
     def _get_telemetry_data(self) -> Dict[str, Any]:
         """
         Data that is sent to Posthog for usage analytics.
         """
         return {"model": self.model}
 
@@ -79,61 +87,73 @@
 
         :returns:
             Dictionary with serialized data.
         """
         return default_to_dict(
             self,
             model=self.model,
-            api_base_url=self.api_base_url,
-            organization=self.organization,
+            device=self.device.to_dict(),
+            token=self.token.to_dict() if self.token else None,
             prefix=self.prefix,
             suffix=self.suffix,
-            dimensions=self.dimensions,
-            api_key=self.api_key.to_dict(),
+            batch_size=self.batch_size,
+            progress_bar=self.progress_bar,
+            normalize_embeddings=self.normalize_embeddings,
+            trust_remote_code=self.trust_remote_code,
         )
 
     @classmethod
-    def from_dict(cls, data: Dict[str, Any]) -> "OpenAITextEmbedder":
+    def from_dict(cls, data: Dict[str, Any]) -> "SentenceTransformersTextEmbedder":
         """
         Deserializes the component from a dictionary.
 
         :param data:
             Dictionary to deserialize from.
         :returns:
             Deserialized component.
         """
-        deserialize_secrets_inplace(data["init_parameters"], keys=["api_key"])
+        serialized_device = data["init_parameters"]["device"]
+        data["init_parameters"]["device"] = ComponentDevice.from_dict(serialized_device)
+
+        deserialize_secrets_inplace(data["init_parameters"], keys=["token"])
         return default_from_dict(cls, data)
 
-    @component.output_types(embedding=List[float], meta=Dict[str, Any])
+    def warm_up(self):
+        """
+        Initializes the component.
+        """
+        if not hasattr(self, "embedding_backend"):
+            self.embedding_backend = _SentenceTransformersEmbeddingBackendFactory.get_embedding_backend(
+                model=self.model,
+                device=self.device.to_torch_str(),
+                auth_token=self.token,
+                trust_remote_code=self.trust_remote_code,
+            )
+
+    @component.output_types(embedding=List[float])
     def run(self, text: str):
         """
         Embed a single string.
 
         :param text:
             Text to embed.
 
         :returns:
             A dictionary with the following keys:
             - `embedding`: The embedding of the input text.
-            - `meta`: Information about the usage of the model.
         """
         if not isinstance(text, str):
             raise TypeError(
-                "OpenAITextEmbedder expects a string as an input."
-                "In case you want to embed a list of Documents, please use the OpenAIDocumentEmbedder."
+                "SentenceTransformersTextEmbedder expects a string as input."
+                "In case you want to embed a list of Documents, please use the SentenceTransformersDocumentEmbedder."
             )
+        if not hasattr(self, "embedding_backend"):
+            raise RuntimeError("The embedding model has not been loaded. Please call warm_up() before running.")
 
         text_to_embed = self.prefix + text + self.suffix
-
-        # copied from OpenAI embedding_utils (https://github.com/openai/openai-python/blob/main/openai/embeddings_utils.py)
-        # replace newlines, which can negatively affect performance.
-        text_to_embed = text_to_embed.replace("\n", " ")
-
-        if self.dimensions is not None:
-            response = self.client.embeddings.create(model=self.model, dimensions=self.dimensions, input=text_to_embed)
-        else:
-            response = self.client.embeddings.create(model=self.model, input=text_to_embed)
-
-        meta = {"model": response.model, "usage": dict(response.usage)}
-
-        return {"embedding": response.data[0].embedding, "meta": meta}
+        embedding = self.embedding_backend.embed(
+            [text_to_embed],
+            batch_size=self.batch_size,
+            show_progress_bar=self.progress_bar,
+            normalize_embeddings=self.normalize_embeddings,
+        )[0]
+        return {"embedding": embedding}
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/embedders/sentence_transformers_document_embedder.py` & `haystack_ai-2.1.0rc1/haystack/components/embedders/sentence_transformers_document_embedder.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         prefix: str = "",
         suffix: str = "",
         batch_size: int = 32,
         progress_bar: bool = True,
         normalize_embeddings: bool = False,
         meta_fields_to_embed: Optional[List[str]] = None,
         embedding_separator: str = "\n",
+        trust_remote_code: bool = False,
     ):
         """
         Create a SentenceTransformersDocumentEmbedder component.
 
         :param model:
             Local path or ID of the model on HuggingFace Hub.
         :param device:
@@ -61,26 +62,30 @@
             If True shows a progress bar when running.
         :param normalize_embeddings:
             If True returned vectors will have length 1.
         :param meta_fields_to_embed:
             List of meta fields that will be embedded along with the Document text.
         :param embedding_separator:
             Separator used to concatenate the meta fields to the Document text.
+        :param trust_remote_code:
+            If `False`, only Hugging Face verified model architectures are allowed.
+            If `True`, custom models and scripts are allowed.
         """
 
         self.model = model
         self.device = ComponentDevice.resolve_device(device)
         self.token = token
         self.prefix = prefix
         self.suffix = suffix
         self.batch_size = batch_size
         self.progress_bar = progress_bar
         self.normalize_embeddings = normalize_embeddings
         self.meta_fields_to_embed = meta_fields_to_embed or []
         self.embedding_separator = embedding_separator
+        self.trust_remote_code = trust_remote_code
 
     def _get_telemetry_data(self) -> Dict[str, Any]:
         """
         Data that is sent to Posthog for usage analytics.
         """
         return {"model": self.model}
 
@@ -99,14 +104,15 @@
             prefix=self.prefix,
             suffix=self.suffix,
             batch_size=self.batch_size,
             progress_bar=self.progress_bar,
             normalize_embeddings=self.normalize_embeddings,
             meta_fields_to_embed=self.meta_fields_to_embed,
             embedding_separator=self.embedding_separator,
+            trust_remote_code=self.trust_remote_code,
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "SentenceTransformersDocumentEmbedder":
         """
         Deserializes the component from a dictionary.
 
@@ -123,15 +129,18 @@
 
     def warm_up(self):
         """
         Initializes the component.
         """
         if not hasattr(self, "embedding_backend"):
             self.embedding_backend = _SentenceTransformersEmbeddingBackendFactory.get_embedding_backend(
-                model=self.model, device=self.device.to_torch_str(), auth_token=self.token
+                model=self.model,
+                device=self.device.to_torch_str(),
+                auth_token=self.token,
+                trust_remote_code=self.trust_remote_code,
             )
 
     @component.output_types(documents=List[Document])
     def run(self, documents: List[Document]):
         """
         Embed a list of Documents.
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/embedders/sentence_transformers_text_embedder.py` & `haystack_ai-2.1.0rc1/haystack/components/retrievers/in_memory/embedding_retriever.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,150 +1,169 @@
 from typing import Any, Dict, List, Optional
 
-from haystack import component, default_from_dict, default_to_dict
-from haystack.components.embedders.backends.sentence_transformers_backend import (
-    _SentenceTransformersEmbeddingBackendFactory,
-)
-from haystack.utils import ComponentDevice, Secret, deserialize_secrets_inplace
+from haystack import DeserializationError, Document, component, default_from_dict, default_to_dict
+from haystack.document_stores.in_memory import InMemoryDocumentStore
 
 
 @component
-class SentenceTransformersTextEmbedder:
+class InMemoryEmbeddingRetriever:
     """
-    A component for embedding strings using Sentence Transformers models.
+    Retrieves documents using vector similarity.
 
     Usage example:
     ```python
-    from haystack.components.embedders import SentenceTransformersTextEmbedder
-
-    text_to_embed = "I love pizza!"
+    from haystack import Document
+    from haystack.components.embedders import SentenceTransformersDocumentEmbedder, SentenceTransformersTextEmbedder
+    from haystack.components.retrievers.in_memory import InMemoryEmbeddingRetriever
+    from haystack.document_stores.in_memory import InMemoryDocumentStore
+
+    docs = [
+        Document(content="Python is a popular programming language"),
+        Document(content="python ist eine beliebte Programmiersprache"),
+    ]
+    doc_embedder = SentenceTransformersDocumentEmbedder()
+    doc_embedder.warm_up()
+    docs_with_embeddings = doc_embedder.run(docs)["documents"]
+
+    doc_store = InMemoryDocumentStore()
+    doc_store.write_documents(docs_with_embeddings)
+    retriever = InMemoryEmbeddingRetriever(doc_store)
 
+    query="Programmiersprache"
     text_embedder = SentenceTransformersTextEmbedder()
     text_embedder.warm_up()
+    query_embedding = text_embedder.run(query)["embedding"]
 
-    print(text_embedder.run(text_to_embed))
+    result = retriever.run(query_embedding=query_embedding)
 
-    # {'embedding': [-0.07804739475250244, 0.1498992145061493,, ...]}
+    print(result["documents"])
     ```
     """
 
     def __init__(
         self,
-        model: str = "sentence-transformers/all-mpnet-base-v2",
-        device: Optional[ComponentDevice] = None,
-        token: Optional[Secret] = Secret.from_env_var("HF_API_TOKEN", strict=False),
-        prefix: str = "",
-        suffix: str = "",
-        batch_size: int = 32,
-        progress_bar: bool = True,
-        normalize_embeddings: bool = False,
+        document_store: InMemoryDocumentStore,
+        filters: Optional[Dict[str, Any]] = None,
+        top_k: int = 10,
+        scale_score: bool = False,
+        return_embedding: bool = False,
     ):
         """
-        Create a SentenceTransformersTextEmbedder component.
+        Create the InMemoryEmbeddingRetriever component.
 
-        :param model:
-            Local path or ID of the model on HuggingFace Hub.
-        :param device:
-            Overrides the default device used to load the model.
-        :param token:
-            The API token used to download private models from Hugging Face.
-        :param prefix:
-            A string to add at the beginning of each text.
-            Can be used to prepend the text with an instruction, as required by some embedding models,
-            such as E5 and bge.
-        :param suffix:
-            A string to add at the end of each text.
-        :param batch_size:
-            Number of Documents to encode at once.
-        :param progress_bar:
-            If True shows a progress bar when running.
-        :param normalize_embeddings:
-            If True returned vectors will have length 1.
-        """
-
-        self.model = model
-        self.device = ComponentDevice.resolve_device(device)
-        self.token = token
-        self.prefix = prefix
-        self.suffix = suffix
-        self.batch_size = batch_size
-        self.progress_bar = progress_bar
-        self.normalize_embeddings = normalize_embeddings
+        :param document_store:
+            An instance of InMemoryDocumentStore.
+        :param filters:
+            A dictionary with filters to narrow down the search space.
+        :param top_k:
+            The maximum number of documents to retrieve.
+        :param scale_score:
+            Scales the BM25 score to a unit interval in the range of 0 to 1, where 1 means extremely relevant. If set to `False`, uses raw similarity scores.
+        :param return_embedding:
+            Whether to return the embedding of the retrieved Documents.
+
+        :raises ValueError:
+            If the specified top_k is not > 0.
+        """
+        if not isinstance(document_store, InMemoryDocumentStore):
+            raise ValueError("document_store must be an instance of InMemoryDocumentStore")
+
+        self.document_store = document_store
+
+        if top_k <= 0:
+            raise ValueError(f"top_k must be greater than 0. Currently, top_k is {top_k}")
+
+        self.filters = filters
+        self.top_k = top_k
+        self.scale_score = scale_score
+        self.return_embedding = return_embedding
 
     def _get_telemetry_data(self) -> Dict[str, Any]:
         """
         Data that is sent to Posthog for usage analytics.
         """
-        return {"model": self.model}
+        return {"document_store": type(self.document_store).__name__}
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
         :returns:
             Dictionary with serialized data.
         """
+        docstore = self.document_store.to_dict()
         return default_to_dict(
             self,
-            model=self.model,
-            device=self.device.to_dict(),
-            token=self.token.to_dict() if self.token else None,
-            prefix=self.prefix,
-            suffix=self.suffix,
-            batch_size=self.batch_size,
-            progress_bar=self.progress_bar,
-            normalize_embeddings=self.normalize_embeddings,
+            document_store=docstore,
+            filters=self.filters,
+            top_k=self.top_k,
+            scale_score=self.scale_score,
+            return_embedding=self.return_embedding,
         )
 
     @classmethod
-    def from_dict(cls, data: Dict[str, Any]) -> "SentenceTransformersTextEmbedder":
+    def from_dict(cls, data: Dict[str, Any]) -> "InMemoryEmbeddingRetriever":
         """
         Deserializes the component from a dictionary.
 
         :param data:
-            Dictionary to deserialize from.
+            The dictionary to deserialize from.
         :returns:
-            Deserialized component.
+            The deserialized component.
         """
-        serialized_device = data["init_parameters"]["device"]
-        data["init_parameters"]["device"] = ComponentDevice.from_dict(serialized_device)
-
-        deserialize_secrets_inplace(data["init_parameters"], keys=["token"])
+        init_params = data.get("init_parameters", {})
+        if "document_store" not in init_params:
+            raise DeserializationError("Missing 'document_store' in serialization data")
+        if "type" not in init_params["document_store"]:
+            raise DeserializationError("Missing 'type' in document store's serialization data")
+        data["init_parameters"]["document_store"] = InMemoryDocumentStore.from_dict(
+            data["init_parameters"]["document_store"]
+        )
         return default_from_dict(cls, data)
 
-    def warm_up(self):
-        """
-        Initializes the component.
-        """
-        if not hasattr(self, "embedding_backend"):
-            self.embedding_backend = _SentenceTransformersEmbeddingBackendFactory.get_embedding_backend(
-                model=self.model, device=self.device.to_torch_str(), auth_token=self.token
-            )
-
-    @component.output_types(embedding=List[float])
-    def run(self, text: str):
+    @component.output_types(documents=List[Document])
+    def run(
+        self,
+        query_embedding: List[float],
+        filters: Optional[Dict[str, Any]] = None,
+        top_k: Optional[int] = None,
+        scale_score: Optional[bool] = None,
+        return_embedding: Optional[bool] = None,
+    ):
         """
-        Embed a single string.
-
-        :param text:
-            Text to embed.
+        Run the InMemoryEmbeddingRetriever on the given input data.
 
+        :param query_embedding:
+            Embedding of the query.
+        :param filters:
+            A dictionary with filters to narrow down the search space.
+        :param top_k:
+            The maximum number of documents to return.
+        :param scale_score:
+            Scales the similarity score to a unit interval in the range of 0 to 1, where 1 means extremely relevant. If set to `False`, uses raw similarity scores.
+            If not specified, the value provided at initialization is used.
+        :param return_embedding:
+            Whether to return the embedding of the retrieved Documents.
         :returns:
-            A dictionary with the following keys:
-            - `embedding`: The embedding of the input text.
+            The retrieved documents.
+
+        :raises ValueError:
+            If the specified DocumentStore is not found or is not an InMemoryDocumentStore instance.
         """
-        if not isinstance(text, str):
-            raise TypeError(
-                "SentenceTransformersTextEmbedder expects a string as input."
-                "In case you want to embed a list of Documents, please use the SentenceTransformersDocumentEmbedder."
-            )
-        if not hasattr(self, "embedding_backend"):
-            raise RuntimeError("The embedding model has not been loaded. Please call warm_up() before running.")
-
-        text_to_embed = self.prefix + text + self.suffix
-        embedding = self.embedding_backend.embed(
-            [text_to_embed],
-            batch_size=self.batch_size,
-            show_progress_bar=self.progress_bar,
-            normalize_embeddings=self.normalize_embeddings,
-        )[0]
-        return {"embedding": embedding}
+        if filters is None:
+            filters = self.filters
+        if top_k is None:
+            top_k = self.top_k
+        if scale_score is None:
+            scale_score = self.scale_score
+        if return_embedding is None:
+            return_embedding = self.return_embedding
+
+        docs = self.document_store.embedding_retrieval(
+            query_embedding=query_embedding,
+            filters=filters,
+            top_k=top_k,
+            scale_score=scale_score,
+            return_embedding=return_embedding,
+        )
+
+        return {"documents": docs}
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/embedders/backends/sentence_transformers_backend.py` & `haystack_ai-2.1.0rc1/haystack/components/embedders/backends/sentence_transformers_backend.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,31 +11,44 @@
     """
     Factory class to create instances of Sentence Transformers embedding backends.
     """
 
     _instances: Dict[str, "_SentenceTransformersEmbeddingBackend"] = {}
 
     @staticmethod
-    def get_embedding_backend(model: str, device: Optional[str] = None, auth_token: Optional[Secret] = None):
+    def get_embedding_backend(
+        model: str, device: Optional[str] = None, auth_token: Optional[Secret] = None, trust_remote_code: bool = False
+    ):
         embedding_backend_id = f"{model}{device}{auth_token}"
 
         if embedding_backend_id in _SentenceTransformersEmbeddingBackendFactory._instances:
             return _SentenceTransformersEmbeddingBackendFactory._instances[embedding_backend_id]
-        embedding_backend = _SentenceTransformersEmbeddingBackend(model=model, device=device, auth_token=auth_token)
+        embedding_backend = _SentenceTransformersEmbeddingBackend(
+            model=model, device=device, auth_token=auth_token, trust_remote_code=trust_remote_code
+        )
         _SentenceTransformersEmbeddingBackendFactory._instances[embedding_backend_id] = embedding_backend
         return embedding_backend
 
 
 class _SentenceTransformersEmbeddingBackend:
     """
     Class to manage Sentence Transformers embeddings.
     """
 
-    def __init__(self, model: str, device: Optional[str] = None, auth_token: Optional[Secret] = None):
+    def __init__(
+        self,
+        model: str,
+        device: Optional[str] = None,
+        auth_token: Optional[Secret] = None,
+        trust_remote_code: bool = False,
+    ):
         sentence_transformers_import.check()
         self.model = SentenceTransformer(
-            model_name_or_path=model, device=device, use_auth_token=auth_token.resolve_value() if auth_token else None
+            model_name_or_path=model,
+            device=device,
+            use_auth_token=auth_token.resolve_value() if auth_token else None,
+            trust_remote_code=trust_remote_code,
         )
 
     def embed(self, data: List[str], **kwargs) -> List[List[float]]:
         embeddings = self.model.encode(data, **kwargs).tolist()
         return embeddings
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/extractors/named_entity_extractor.py` & `haystack_ai-2.1.0rc1/haystack/components/extractors/named_entity_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 
 class _BackendEnumMeta(EnumMeta):
     """
     Metaclass for fine-grained error handling of backend enums.
     """
 
-    def __call__(cls, value, names=None, *, module=None, qualname=None, type=None, start=1):
+    def __call__(cls, value, names=None, *, module=None, qualname=None, type=None, start=1):  # noqa: A002
         if names is None:
             try:
                 return EnumMeta.__call__(cls, value, names, module=module, qualname=qualname, type=type, start=start)
             except ValueError:
                 supported_backends = ", ".join(sorted(v.value for v in cls))  # pylint: disable=not-an-iterable
                 raise ComponentError(
                     f"Invalid backend `{value}` for named entity extractor. "
@@ -155,16 +155,15 @@
             raise ComponentError(
                 f"Named entity extractor with backend '{self._backend.type} failed to initialize."
             ) from e
 
     @component.output_types(documents=List[Document])
     def run(self, documents: List[Document], batch_size: int = 1) -> Dict[str, Any]:
         """
-        Annotate named entities in each document and store
-        the annotations in the document's metadata.
+        Annotate named entities in each document and store the annotations in the document's metadata.
 
         :param documents:
             Documents to process.
         :param batch_size:
             Batch size used for processing the documents.
         :returns:
             Processed documents.
@@ -223,16 +222,15 @@
         Returns if the extractor is ready to annotate text.
         """
         return self._backend.initialized
 
     @classmethod
     def get_stored_annotations(cls, document: Document) -> Optional[List[NamedEntityAnnotation]]:
         """
-        Returns the document's named entity annotations stored
-        in its metadata, if any.
+        Returns the document's named entity annotations stored in its metadata, if any.
 
         :param document:
             Document whose annotations are to be fetched.
         :returns:
             The stored annotations.
         """
 
@@ -242,37 +240,35 @@
 class _NerBackend(ABC):
     """
     Base class for NER backends.
     """
 
     def __init__(
         self,
-        type: NamedEntityExtractorBackend,
+        _type: NamedEntityExtractorBackend,
         device: ComponentDevice,
         pipeline_kwargs: Optional[Dict[str, Any]] = None,
     ) -> None:
         super().__init__()
 
-        self._type = type
+        self._type = _type
         self._device = device
         self._pipeline_kwargs = pipeline_kwargs if pipeline_kwargs is not None else {}
 
     @abstractmethod
     def initialize(self):
         """
-        Initializes the backend. This would usually
-        entail loading models, pipelines, etc.
+        Initializes the backend. This would usually entail loading models, pipelines, and so on.
         """
 
     @property
     @abstractmethod
     def initialized(self) -> bool:
         """
-        Returns if the backend has been initialized, i.e,
-        ready to annotate text.
+        Returns if the backend has been initialized, for example, ready to annotate text.
         """
 
     @abstractmethod
     def annotate(self, texts: List[str], *, batch_size: int = 1) -> List[List[NamedEntityAnnotation]]:
         """
         Predict annotations for a collection of documents.
 
@@ -291,14 +287,16 @@
         """
         Returns the model name or path on the local disk.
         """
 
     @property
     def device(self) -> ComponentDevice:
         """
+        The device on which the backend's model is loaded.
+
         :returns:
             The device on which the backend's model is loaded.
         """
         return self._device
 
     @property
     def type(self) -> NamedEntityExtractorBackend:
@@ -453,16 +451,15 @@
     @property
     def model_name(self) -> str:
         return self._model_name_or_path
 
     @contextmanager
     def _select_device(self):
         """
-        Context manager used to run spaCy models on a specific
-        GPU in a scoped manner.
+        Context manager used to run spaCy models on a specific GPU in a scoped manner.
         """
 
         # TODO: This won't restore the active device.
         # Since there are no opaque API functions to determine
         # the active device in spaCy/Thinc, we can't do much
         # about it as a consumer unless we start poking into their
         # internals.
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/fetchers/link_content.py` & `haystack_ai-2.1.0rc1/haystack/components/fetchers/link_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,22 +22,26 @@
     "Accept-Language": "en-US,en;q=0.9,it;q=0.8,es;q=0.7",
     "referer": "https://www.google.com/",
 }
 
 
 def _text_content_handler(response: Response) -> ByteStream:
     """
+    Handles text content.
+
     :param response: Response object from the request.
     :return: The extracted text.
     """
     return ByteStream.from_string(response.text)
 
 
 def _binary_content_handler(response: Response) -> ByteStream:
     """
+    Handles binary content.
+
     :param response: Response object from the request.
     :return: The extracted binary file-like object.
     """
     return ByteStream(data=response.content)
 
 
 @component
@@ -207,13 +211,14 @@
         """
         content_type = response.headers.get("Content-Type", "")
         return content_type.split(";")[0]
 
     def _switch_user_agent(self, retry_state: RetryCallState) -> None:
         """
         Switches the User-Agent for this LinkContentRetriever to the next one in the list of user agents.
+
         Used by tenacity to retry the requests with a different user agent.
 
         :param retry_state: The retry state (unused, required by tenacity).
         """
         self.current_user_agent_idx = (self.current_user_agent_idx + 1) % len(self.user_agents)
         logger.debug("Switched user agent to {user_agent}", user_agent=self.user_agents[self.current_user_agent_idx])
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/generators/azure.py` & `haystack_ai-2.1.0rc1/haystack/components/generators/azure.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 from haystack.utils import Secret, deserialize_callable, deserialize_secrets_inplace, serialize_callable
 
 logger = logging.getLogger(__name__)
 
 
 class AzureOpenAIGenerator(OpenAIGenerator):
     """
-    Enables text generation using OpenAI's large language models (LLMs) on Azure. It supports gpt-4 and gpt-3.5-turbo
-    family of models.
+    A Generator component that uses OpenAI's large language models (LLMs) on Azure to generate text.
+
+    It supports gpt-4 and gpt-3.5-turbo family of models.
 
     Users can pass any text generation parameters valid for the `openai.ChatCompletion.create` method
     directly to this component via the `**generation_kwargs` parameter in __init__ or the `**generation_kwargs`
     parameter in `run` method.
 
     For more details on OpenAI models deployed on Azure, refer to the Microsoft
     [documentation](https://learn.microsoft.com/en-us/azure/ai-services/openai/).
@@ -55,14 +56,16 @@
         azure_ad_token: Optional[Secret] = Secret.from_env_var("AZURE_OPENAI_AD_TOKEN", strict=False),
         organization: Optional[str] = None,
         streaming_callback: Optional[Callable[[StreamingChunk], None]] = None,
         system_prompt: Optional[str] = None,
         generation_kwargs: Optional[Dict[str, Any]] = None,
     ):
         """
+        Initialize the Azure OpenAI Generator.
+
         :param azure_endpoint: The endpoint of the deployed model, e.g. `https://example-resource.azure.openai.com/`
         :param api_version: The version of the API to use. Defaults to 2023-05-15
         :param azure_deployment: The deployment of the model, usually the model name.
         :param api_key: The API key to use for authentication.
         :param azure_ad_token: [Azure Active Directory token](https://www.microsoft.com/en-us/security/business/identity-access/microsoft-entra-id)
         :param organization: The Organization ID, defaults to `None`. See
         [production best practices](https://platform.openai.com/docs/guides/production-best-practices/setting-up-your-organization).
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/generators/hugging_face_local.py` & `haystack_ai-2.1.0rc1/haystack/components/generators/hugging_face_local.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,21 @@
 from haystack.utils.hf import deserialize_hf_model_kwargs, serialize_hf_model_kwargs
 
 logger = logging.getLogger(__name__)
 
 SUPPORTED_TASKS = ["text-generation", "text2text-generation"]
 
 with LazyImport(message="Run 'pip install transformers[torch]'") as transformers_import:
-    from huggingface_hub import model_info
     from transformers import StoppingCriteriaList, pipeline
 
-    from haystack.utils.hf import HFTokenStreamingHandler, StopWordsCriteria  # pylint: disable=ungrouped-imports
+    from haystack.utils.hf import (  # pylint: disable=ungrouped-imports
+        HFTokenStreamingHandler,
+        StopWordsCriteria,
+        resolve_hf_pipeline_kwargs,
+    )
 
 
 @component
 class HuggingFaceLocalGenerator:
     """
     Generator based on a Hugging Face model.
 
@@ -89,45 +92,29 @@
             If you provide this parameter, you should not specify the `stopping_criteria` in `generation_kwargs`.
             For some chat models, the output includes both the new text and the original prompt.
             In these cases, it's important to make sure your prompt has no stop words.
         :param streaming_callback: An optional callable for handling streaming responses.
         """
         transformers_import.check()
 
-        huggingface_pipeline_kwargs = huggingface_pipeline_kwargs or {}
-        generation_kwargs = generation_kwargs or {}
-
         self.token = token
-        token = token.resolve_value() if token else None
-
-        # check if the huggingface_pipeline_kwargs contain the essential parameters
-        # otherwise, populate them with values from other init parameters
-        huggingface_pipeline_kwargs.setdefault("model", model)
-        huggingface_pipeline_kwargs.setdefault("token", token)
-
-        device = ComponentDevice.resolve_device(device)
-        device.update_hf_kwargs(huggingface_pipeline_kwargs, overwrite=False)
-
-        # task identification and validation
-        if task is None:
-            if "task" in huggingface_pipeline_kwargs:
-                task = huggingface_pipeline_kwargs["task"]
-            elif isinstance(huggingface_pipeline_kwargs["model"], str):
-                task = model_info(
-                    huggingface_pipeline_kwargs["model"], token=huggingface_pipeline_kwargs["token"]
-                ).pipeline_tag
+        generation_kwargs = generation_kwargs or {}
 
-        if task not in SUPPORTED_TASKS:
-            raise ValueError(
-                f"Task '{task}' is not supported. " f"The supported tasks are: {', '.join(SUPPORTED_TASKS)}."
-            )
-        huggingface_pipeline_kwargs["task"] = task
+        huggingface_pipeline_kwargs = resolve_hf_pipeline_kwargs(
+            huggingface_pipeline_kwargs=huggingface_pipeline_kwargs or {},
+            model=model,
+            task=task,
+            supported_tasks=SUPPORTED_TASKS,
+            device=device,
+            token=token,
+        )
 
         # if not specified, set return_full_text to False for text-generation
         # only generated text is returned (excluding prompt)
+        task = huggingface_pipeline_kwargs["task"]
         if task == "text-generation":
             generation_kwargs.setdefault("return_full_text", False)
 
         if stop_words and "stopping_criteria" in generation_kwargs:
             raise ValueError(
                 "Found both the `stop_words` init parameter and the `stopping_criteria` key in `generation_kwargs`. "
                 "Please specify only one of them."
@@ -152,15 +139,15 @@
     def warm_up(self):
         """
         Initializes the component.
         """
         if self.pipeline is None:
             self.pipeline = pipeline(**self.huggingface_pipeline_kwargs)
 
-        if self.stop_words and self.stopping_criteria_list is None:
+        if self.stop_words:
             stop_words_criteria = StopWordsCriteria(
                 tokenizer=self.pipeline.tokenizer, stop_words=self.stop_words, device=self.pipeline.device
             )
             self.stopping_criteria_list = StoppingCriteriaList([stop_words_criteria])
 
     def to_dict(self) -> Dict[str, Any]:
         """
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/generators/hugging_face_tgi.py` & `haystack_ai-2.1.0rc1/haystack/components/generators/hugging_face_tgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from dataclasses import asdict
 from typing import Any, Callable, Dict, Iterable, List, Optional
 from urllib.parse import urlparse
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.dataclasses import StreamingChunk
 from haystack.lazy_imports import LazyImport
@@ -96,14 +97,20 @@
         :param generation_kwargs:
             A dictionary containing keyword arguments to customize text generation.
                 Some examples: `max_new_tokens`, `temperature`, `top_k`, `top_p`,...
                 See Hugging Face's documentation for more information at: [TextGenerationParameters](https://huggingface.co/docs/huggingface_hub/v0.18.0.rc0/en/package_reference/inference_client#huggingface_hub.inference._text_generation.TextGenerationParameters
         :param stop_words: An optional list of strings representing the stop words.
         :param streaming_callback: An optional callable for handling streaming responses.
         """
+        warnings.warn(
+            "`HuggingFaceTGIGenerator` is deprecated and will be removed in Haystack 2.3.0."
+            "Use `HuggingFaceAPIGenerator` instead.",
+            DeprecationWarning,
+        )
+
         transformers_import.check()
 
         if url:
             r = urlparse(url)
             is_valid_url = all([r.scheme in ["http", "https"], r.netloc])
             if not is_valid_url:
                 raise ValueError(f"Invalid TGI endpoint URL provided: {url}")
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/generators/openai.py` & `haystack_ai-2.1.0rc1/haystack/components/generators/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import dataclasses
 from typing import Any, Callable, Dict, List, Optional, Union
 
 from openai import OpenAI, Stream
 from openai.types.chat import ChatCompletion, ChatCompletionChunk
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.dataclasses import ChatMessage, StreamingChunk
@@ -10,14 +9,16 @@
 
 logger = logging.getLogger(__name__)
 
 
 @component
 class OpenAIGenerator:
     """
+    Text generation component using OpenAI's large language models (LLMs).
+
     Enables text generation using OpenAI's large language models (LLMs). It supports gpt-4 and gpt-3.5-turbo
     family of models.
 
     Users can pass any text generation parameters valid for the `openai.ChatCompletion.create` method
     directly to this component via the `**generation_kwargs` parameter in __init__ or the `**generation_kwargs`
     parameter in `run` method.
 
@@ -160,15 +161,15 @@
         else:
             messages = [message]
 
         # update generation kwargs by merging with the generation kwargs passed to the run method
         generation_kwargs = {**self.generation_kwargs, **(generation_kwargs or {})}
 
         # adapt ChatMessage(s) to the format expected by the OpenAI API
-        openai_formatted_messages = self._convert_to_openai_format(messages)
+        openai_formatted_messages = [message.to_openai_format() for message in messages]
 
         completion: Union[Stream[ChatCompletionChunk], ChatCompletion] = self.client.chat.completions.create(
             model=self.model,
             messages=openai_formatted_messages,  # type: ignore
             stream=self.streaming_callback is not None,
             **generation_kwargs,
         )
@@ -196,31 +197,14 @@
             self._check_finish_reason(response)
 
         return {
             "replies": [message.content for message in completions],
             "meta": [message.meta for message in completions],
         }
 
-    def _convert_to_openai_format(self, messages: List[ChatMessage]) -> List[Dict[str, Any]]:
-        """
-        Converts the list of ChatMessage to the list of messages in the format expected by the OpenAI API.
-
-        :param messages:
-            The list of ChatMessage.
-        :returns:
-            The list of messages in the format expected by the OpenAI API.
-        """
-        openai_chat_message_format = {"role", "content", "name"}
-        openai_formatted_messages = []
-        for m in messages:
-            message_dict = dataclasses.asdict(m)
-            filtered_message = {k: v for k, v in message_dict.items() if k in openai_chat_message_format and v}
-            openai_formatted_messages.append(filtered_message)
-        return openai_formatted_messages
-
     def _connect_chunks(self, chunk: Any, chunks: List[StreamingChunk]) -> ChatMessage:
         """
         Connects the streaming chunks into a single ChatMessage.
         """
         complete_response = ChatMessage.from_assistant("".join([chunk.content for chunk in chunks]))
         complete_response.meta.update(
             {
@@ -272,14 +256,15 @@
         chunk_message = StreamingChunk(content)
         chunk_message.meta.update({"model": chunk.model, "index": choice.index, "finish_reason": choice.finish_reason})
         return chunk_message
 
     def _check_finish_reason(self, message: ChatMessage) -> None:
         """
         Check the `finish_reason` returned with the OpenAI completions.
+
         If the `finish_reason` is `length`, log a warning to the user.
 
         :param message:
             The message returned by the LLM.
         """
         if message.meta["finish_reason"] == "length":
             logger.warning(
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/generators/utils.py` & `haystack_ai-2.1.0rc1/haystack/components/generators/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,33 +3,36 @@
 from haystack.dataclasses import StreamingChunk
 from haystack.utils import deserialize_callable, serialize_callable
 
 
 def print_streaming_chunk(chunk: StreamingChunk) -> None:
     """
     Default callback function for streaming responses.
+
     Prints the tokens of the first completion to stdout as soon as they are received
     """
     print(chunk.content, flush=True, end="")
 
 
 def serialize_callback_handler(streaming_callback: Callable[[StreamingChunk], None]) -> str:
     """
     Serializes the streaming callback handler.
+
     :param streaming_callback:
         The streaming callback handler function
     :returns:
         The full path of the streaming callback handler function
     """
     return serialize_callable(streaming_callback)
 
 
 def deserialize_callback_handler(callback_name: str) -> Optional[Callable[[StreamingChunk], None]]:
     """
     Deserializes the streaming callback handler.
+
     :param callback_name:
         The full path of the streaming callback handler function
     :returns:
         The streaming callback handler function
     :raises DeserializationError:
         If the streaming callback handler function cannot be found
     """
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/generators/chat/__init__.py` & `haystack_ai-2.1.0rc1/haystack/components/generators/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from haystack.components.generators.chat.openai import (  # noqa: I001 (otherwise we end up with partial imports)
-    OpenAIChatGenerator,
+from haystack.components.generators.openai import (  # noqa: I001 (otherwise we end up with partial imports)
+    OpenAIGenerator,
 )
-from haystack.components.generators.chat.azure import AzureOpenAIChatGenerator
-from haystack.components.generators.chat.hugging_face_local import HuggingFaceLocalChatGenerator
-from haystack.components.generators.chat.hugging_face_tgi import HuggingFaceTGIChatGenerator
+from haystack.components.generators.azure import AzureOpenAIGenerator
+from haystack.components.generators.hugging_face_local import HuggingFaceLocalGenerator
+from haystack.components.generators.hugging_face_tgi import HuggingFaceTGIGenerator
+from haystack.components.generators.hugging_face_api import HuggingFaceAPIGenerator
 
 __all__ = [
-    "HuggingFaceLocalChatGenerator",
-    "HuggingFaceTGIChatGenerator",
-    "OpenAIChatGenerator",
-    "AzureOpenAIChatGenerator",
+    "HuggingFaceLocalGenerator",
+    "HuggingFaceTGIGenerator",
+    "HuggingFaceAPIGenerator",
+    "OpenAIGenerator",
+    "AzureOpenAIGenerator",
 ]
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/generators/chat/azure.py` & `haystack_ai-2.1.0rc1/haystack/components/generators/chat/azure.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from haystack.utils import Secret, deserialize_callable, deserialize_secrets_inplace, serialize_callable
 
 logger = logging.getLogger(__name__)
 
 
 class AzureOpenAIChatGenerator(OpenAIChatGenerator):
     """
+    A Chat Generator component that uses the Azure OpenAI API to generate text.
+
     Enables text generation using OpenAI's large language models (LLMs) on Azure. It supports `gpt-4` and `gpt-3.5-turbo`
     family of models accessed through the chat completions API endpoint.
 
     Users can pass any text generation parameters valid for the `openai.ChatCompletion.create` method
     directly to this component via the `generation_kwargs` parameter in `__init__` or the `generation_kwargs`
     parameter in `run` method.
 
@@ -72,14 +74,16 @@
         api_key: Optional[Secret] = Secret.from_env_var("AZURE_OPENAI_API_KEY", strict=False),
         azure_ad_token: Optional[Secret] = Secret.from_env_var("AZURE_OPENAI_AD_TOKEN", strict=False),
         organization: Optional[str] = None,
         streaming_callback: Optional[Callable[[StreamingChunk], None]] = None,
         generation_kwargs: Optional[Dict[str, Any]] = None,
     ):
         """
+        Initialize the Azure OpenAI Chat Generator component.
+
         :param azure_endpoint: The endpoint of the deployed model, e.g. `"https://example-resource.azure.openai.com/"`
         :param api_version: The version of the API to use. Defaults to 2023-05-15
         :param azure_deployment: The deployment of the model, usually the model name.
         :param api_key: The API key to use for authentication.
         :param azure_ad_token: [Azure Active Directory token](https://www.microsoft.com/en-us/security/business/identity-access/microsoft-entra-id)
         :param organization: The Organization ID, defaults to `None`. See
         [production best practices](https://platform.openai.com/docs/guides/production-best-practices/setting-up-your-organization).
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/generators/chat/hugging_face_local.py` & `haystack_ai-2.1.0rc1/haystack/components/generators/chat/hugging_face_local.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 
 PIPELINE_SUPPORTED_TASKS = ["text-generation", "text2text-generation"]
 
 
 @component
 class HuggingFaceLocalChatGenerator:
     """
+    A Chat Generator component that uses models available on Hugging Face Hub to generate chat responses locally.
+
     The `HuggingFaceLocalChatGenerator` class is a component designed for generating chat responses using models from
     Hugging Face's model hub. It is tailored for local runtime text generation tasks and provides a convenient interface
     for working with chat-based models, such as `HuggingFaceH4/zephyr-7b-beta` or `meta-llama/Llama-2-7b-chat-hf`
     etc.
 
     Usage example:
     ```python
@@ -74,14 +76,16 @@
         chat_template: Optional[str] = None,
         generation_kwargs: Optional[Dict[str, Any]] = None,
         huggingface_pipeline_kwargs: Optional[Dict[str, Any]] = None,
         stop_words: Optional[List[str]] = None,
         streaming_callback: Optional[Callable[[StreamingChunk], None]] = None,
     ):
         """
+        Initializes the HuggingFaceLocalChatGenerator component.
+
         :param model: The name or path of a Hugging Face model for text generation,
             for example, `mistralai/Mistral-7B-Instruct-v0.2`, `TheBloke/OpenHermes-2.5-Mistral-7B-16k-AWQ`, etc.
             The important aspect of the model is that it should be a chat model and that it supports ChatML messaging
             format.
             If the model is also specified in the `huggingface_pipeline_kwargs`, this parameter will be ignored.
         :param task: The task for the Hugging Face pipeline.
             Possible values are "text-generation" and "text2text-generation".
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/generators/chat/hugging_face_tgi.py` & `haystack_ai-2.1.0rc1/haystack/components/generators/chat/hugging_face_tgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from dataclasses import asdict
 from typing import Any, Callable, Dict, Iterable, List, Optional
 from urllib.parse import urlparse
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.dataclasses import ChatMessage, StreamingChunk
 from haystack.lazy_imports import LazyImport
@@ -19,14 +20,16 @@
 
 logger = logging.getLogger(__name__)
 
 
 @component
 class HuggingFaceTGIChatGenerator:
     """
+    A Chat-based text generation component using Hugging Face's Text Generation Inference (TGI) framework.
+
     Enables text generation using HuggingFace Hub hosted chat-based LLMs. This component is designed to seamlessly
     inference chat-based models deployed on the Text Generation Inference (TGI) backend.
 
     You can use this component for chat LLMs hosted on Hugging Face inference endpoints, the rate-limited
     Inference API tier.
 
     Key Features and Compatibility:
@@ -109,14 +112,19 @@
         :param generation_kwargs: A dictionary containing keyword arguments to customize text generation.
             Some examples: `max_new_tokens`, `temperature`, `top_k`, `top_p`,...
             See Hugging Face's [documentation](https://huggingface.co/docs/huggingface_hub/v0.18.0.rc0/en/package_reference/inference_client#huggingface_hub.inference._text_generation.TextGenerationParameters)
             for more information.
         :param stop_words: An optional list of strings representing the stop words.
         :param streaming_callback: An optional callable for handling streaming responses.
         """
+        warnings.warn(
+            "`HuggingFaceTGIChatGenerator` is deprecated and will be removed in Haystack 2.3.0."
+            "Use `HuggingFaceAPIChatGenerator` instead.",
+            DeprecationWarning,
+        )
         transformers_import.check()
 
         if url:
             r = urlparse(url)
             is_valid_url = all([r.scheme in ["http", "https"], r.netloc])
             if not is_valid_url:
                 raise ValueError(f"Invalid TGI endpoint URL provided: {url}")
@@ -137,14 +145,16 @@
         self.generation_kwargs = generation_kwargs
         self.client = InferenceClient(url or model, token=token.resolve_value() if token else None)
         self.streaming_callback = streaming_callback
         self.tokenizer = None
 
     def warm_up(self) -> None:
         """
+        Warm up the tokenizer by loading it from the model.
+
         If the url is not provided, check if the model is deployed on the free tier of the HF inference API.
         Load the tokenizer
         """
 
         # is this user using HF free tier inference API?
         if self.model and not self.url:
             deployed_models = list_inference_deployed_models()
@@ -228,16 +238,17 @@
         generation_kwargs["stop_sequences"] = generation_kwargs.get("stop_sequences", [])
         generation_kwargs["stop_sequences"].extend(generation_kwargs.pop("stop_words", []))
 
         if self.tokenizer is None:
             raise RuntimeError("Please call warm_up() before running LLM inference.")
 
         # apply either model's chat template or the user-provided one
+        formatted_messages = [message.to_openai_format() for message in messages]
         prepared_prompt: str = self.tokenizer.apply_chat_template(
-            conversation=messages, chat_template=self.chat_template, tokenize=False
+            conversation=formatted_messages, chat_template=self.chat_template, tokenize=False
         )
         prompt_token_count: int = len(self.tokenizer.encode(prepared_prompt, add_special_tokens=False))
 
         if self.streaming_callback:
             if num_responses > 1:
                 raise ValueError("Cannot stream multiple responses, please set n=1.")
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/generators/chat/openai.py` & `haystack_ai-2.1.0rc1/haystack/components/generators/chat/openai.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import copy
-import dataclasses
 import json
 from typing import Any, Callable, Dict, List, Optional, Union
 
-from openai import OpenAI, Stream  # type: ignore
+from openai import OpenAI, Stream
 from openai.types.chat import ChatCompletion, ChatCompletionChunk, ChatCompletionMessage
 from openai.types.chat.chat_completion import Choice
 from openai.types.chat.chat_completion_chunk import Choice as ChunkChoice
 
 from haystack import component, default_from_dict, default_to_dict, logging
 from haystack.dataclasses import ChatMessage, StreamingChunk
 from haystack.utils import Secret, deserialize_callable, deserialize_secrets_inplace, serialize_callable
 
 logger = logging.getLogger(__name__)
 
 
 @component
 class OpenAIChatGenerator:
     """
+    A Chat Generator component that uses the OpenAI API to generate text.
+
     Enables text generation using OpenAI's large language models (LLMs). It supports `gpt-4` and `gpt-3.5-turbo`
     family of models accessed through the chat completions API endpoint.
 
     Users can pass any text generation parameters valid for the `openai.ChatCompletion.create` method
     directly to this component via the `generation_kwargs` parameter in `__init__` or the `generation_kwargs`
     parameter in `run` method.
 
@@ -68,14 +69,16 @@
         model: str = "gpt-3.5-turbo",
         streaming_callback: Optional[Callable[[StreamingChunk], None]] = None,
         api_base_url: Optional[str] = None,
         organization: Optional[str] = None,
         generation_kwargs: Optional[Dict[str, Any]] = None,
     ):
         """
+        Initializes the OpenAIChatGenerator component.
+
         Creates an instance of OpenAIChatGenerator. Unless specified otherwise in the `model`, this is for OpenAI's
         GPT-3.5 model.
 
         :param api_key: The OpenAI API key.
         :param model: The name of the model to use.
         :param streaming_callback: A callback function that is called when a new token is received from the stream.
             The callback function accepts StreamingChunk as an argument.
@@ -165,15 +168,15 @@
             A list containing the generated responses as ChatMessage instances.
         """
 
         # update generation kwargs by merging with the generation kwargs passed to the run method
         generation_kwargs = {**self.generation_kwargs, **(generation_kwargs or {})}
 
         # adapt ChatMessage(s) to the format expected by the OpenAI API
-        openai_formatted_messages = self._convert_to_openai_format(messages)
+        openai_formatted_messages = [message.to_openai_format() for message in messages]
 
         chat_completion: Union[Stream[ChatCompletionChunk], ChatCompletion] = self.client.chat.completions.create(
             model=self.model,
             messages=openai_formatted_messages,  # type: ignore # openai expects list of specific message types
             stream=self.streaming_callback is not None,
             **generation_kwargs,
         )
@@ -200,31 +203,18 @@
 
         # before returning, do post-processing of the completions
         for message in completions:
             self._check_finish_reason(message)
 
         return {"replies": completions}
 
-    def _convert_to_openai_format(self, messages: List[ChatMessage]) -> List[Dict[str, Any]]:
-        """
-        Converts the list of ChatMessage to the list of messages in the format expected by the OpenAI API.
-        :param messages: The list of ChatMessage.
-        :return: The list of messages in the format expected by the OpenAI API.
-        """
-        openai_chat_message_format = {"role", "content", "name"}
-        openai_formatted_messages = []
-        for m in messages:
-            message_dict = dataclasses.asdict(m)
-            filtered_message = {k: v for k, v in message_dict.items() if k in openai_chat_message_format and v}
-            openai_formatted_messages.append(filtered_message)
-        return openai_formatted_messages
-
     def _connect_chunks(self, chunk: Any, chunks: List[StreamingChunk]) -> ChatMessage:
         """
         Connects the streaming chunks into a single ChatMessage.
+
         :param chunk: The last chunk returned by the OpenAI API.
         :param chunks: The list of all chunks returned by the OpenAI API.
         """
         is_tools_call = bool(chunks[0].meta.get("tool_calls"))
         is_function_call = bool(chunks[0].meta.get("function_call"))
         # if it's a tool call or function call, we need to build the payload dict from all the chunks
         if is_tools_call or is_function_call:
@@ -267,14 +257,15 @@
             }
         )
         return complete_response
 
     def _build_message(self, completion: ChatCompletion, choice: Choice) -> ChatMessage:
         """
         Converts the non-streaming response from the OpenAI API to a ChatMessage.
+
         :param completion: The completion returned by the OpenAI API.
         :param choice: The choice returned by the OpenAI API.
         :return: The ChatMessage.
         """
         message: ChatCompletionMessage = choice.message
         content = message.content or ""
         if message.function_call:
@@ -298,14 +289,15 @@
             }
         )
         return chat_message
 
     def _build_chunk(self, chunk: ChatCompletionChunk) -> StreamingChunk:
         """
         Converts the streaming response chunk from the OpenAI API to a StreamingChunk.
+
         :param chunk: The chunk returned by the OpenAI API.
         :param choice: The choice returned by the OpenAI API.
         :return: The StreamingChunk.
         """
         # we stream the content of the chunk if it's not a tool or function call
         choice: ChunkChoice = chunk.choices[0]
         content = choice.delta.content or ""
@@ -322,14 +314,15 @@
             }
         )
         return chunk_message
 
     def _check_finish_reason(self, message: ChatMessage) -> None:
         """
         Check the `finish_reason` returned with the OpenAI completions.
+
         If the `finish_reason` is `length` or `content_filter`, log a warning.
         :param message: The message returned by the LLM.
         """
         if message.meta["finish_reason"] == "length":
             logger.warning(
                 "The completion for index {index} has been truncated before reaching a natural stopping point. "
                 "Increase the max_tokens parameter to allow for longer completions.",
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/joiners/document_joiner.py` & `haystack_ai-2.1.0rc1/haystack/components/joiners/document_joiner.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,14 +133,15 @@
             doc.score = scores_map[doc.id]
 
         return documents_map.values()
 
     def _reciprocal_rank_fusion(self, document_lists):
         """
         Merge multiple lists of Documents and assign scores based on reciprocal rank fusion.
+
         The constant k is set to 61 (60 was suggested by the original paper,
         plus 1 as python lists are 0-based and the paper used 1-based ranking).
         """
         k = 61
 
         scores_map = defaultdict(int)
         documents_map = {}
@@ -150,14 +151,14 @@
         for documents, weight in zip(document_lists, weights):
             for rank, doc in enumerate(documents):
                 scores_map[doc.id] += (weight * len(document_lists)) / (k + rank)
                 documents_map[doc.id] = doc
 
         # Normalize scores. Note: len(results) / k is the maximum possible score,
         # achieved by being ranked first in all doc lists with non-zero weight.
-        for id in scores_map:
-            scores_map[id] /= len(document_lists) / k
+        for _id in scores_map:
+            scores_map[_id] /= len(document_lists) / k
 
         for doc in documents_map.values():
             doc.score = scores_map[doc.id]
 
         return documents_map.values()
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/others/multiplexer.py` & `haystack_ai-2.1.0rc1/haystack/components/others/multiplexer.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 logger = logging.getLogger(__name__)
 
 
 @component(is_greedy=True)
 class Multiplexer:
     """
+    A component which receives data connections from multiple components and distributes them to multiple components.
+
     `Multiplexer` offers the ability to both receive data connections from multiple other
     components and to distribute it to various other components, enhancing the functionality of complex data
     processing pipelines.
 
     `Multiplexer` is important for spreading outputs from a single source like a Large Language Model (LLM) across
     different branches of a pipeline. It is especially valuable in error correction loops by rerouting data for
     reevaluation if errors are detected. For instance, in an example pipeline below, `Multiplexer` helps create
@@ -121,14 +123,16 @@
               Deserialized component.
         """
         data["init_parameters"]["type_"] = deserialize_type(data["init_parameters"]["type_"])
         return default_from_dict(cls, data)
 
     def run(self, **kwargs):
         """
+        The run method of the `Multiplexer` component.
+
         Multiplexes the input data from the upstream connected components and distributes it to the downstream connected
         components.
 
         :param **kwargs: The input data. Must be of the type declared in `__init__`.
         :return: A dictionary with the following keys:
             - `value`: The input data.
         """
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/preprocessors/document_cleaner.py` & `haystack_ai-2.1.0rc1/haystack/components/preprocessors/document_cleaner.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 logger = logging.getLogger(__name__)
 
 
 @component
 class DocumentCleaner:
     """
+    Cleans the text in the documents.
+
     Cleans up text documents by removing extra whitespaces, empty lines, specified substrings, regexes,
     page headers and footers (in this order).
 
     Usage example:
     ```python
     from haystack import Document
     from haystack.components.preprocessors import DocumentCleaner
@@ -34,14 +36,16 @@
         remove_empty_lines: bool = True,
         remove_extra_whitespaces: bool = True,
         remove_repeated_substrings: bool = False,
         remove_substrings: Optional[List[str]] = None,
         remove_regex: Optional[str] = None,
     ):
         """
+        Initialize the DocumentCleaner.
+
         :param remove_empty_lines: Whether to remove empty lines.
         :param remove_extra_whitespaces: Whether to remove extra whitespaces.
         :param remove_repeated_substrings: Whether to remove repeated substrings (headers/footers) from pages.
             Pages in the text need to be separated by form feed character "\\f",
             which is supported by `TextFileToDocument` and `AzureOCRDocumentConverter`.
         :param remove_substrings: List of substrings to remove from the text.
         :param remove_regex: Regex to match and replace substrings by "".
@@ -93,65 +97,71 @@
             cleaned_docs.append(Document(content=text, meta=deepcopy(doc.meta)))
 
         return {"documents": cleaned_docs}
 
     def _remove_empty_lines(self, text: str) -> str:
         """
         Remove empty lines and lines that contain nothing but whitespaces from text.
+
         :param text: Text to clean.
         :returns: The text without empty lines.
         """
         lines = text.split("\n")
         non_empty_lines = filter(lambda line: line.strip() != "", lines)
         return "\n".join(non_empty_lines)
 
     def _remove_extra_whitespaces(self, text: str) -> str:
         """
         Remove extra whitespaces from text.
+
         :param text: Text to clean.
         :returns: The text without extra whitespaces.
         """
         return re.sub(r"\s\s+", " ", text).strip()
 
     def _remove_regex(self, text: str, regex: str) -> str:
         """
         Remove substrings that match the specified regex from the text.
+
         :param text: Text to clean.
         :param regex: Regex to match and replace substrings by "".
         :returns: The text without the substrings that match the regex.
         """
         return re.sub(regex, "", text).strip()
 
     def _remove_substrings(self, text: str, substrings: List[str]) -> str:
         """
         Remove all specified substrings from the text.
+
         :param text: Text to clean.
         :param substrings: Substrings to remove.
         :returns: The text without the specified substrings.
         """
         for substring in substrings:
             text = text.replace(substring, "")
         return text
 
     def _remove_repeated_substrings(self, text: str) -> str:
         """
         Remove any substrings from the text that occur repeatedly on every page. For example headers or footers.
+
         Pages in the text need to be separated by form feed character "\f".
         :param text: Text to clean.
         :returns: The text without the repeated substrings.
         """
         return self._find_and_remove_header_footer(
             text, n_chars=300, n_first_pages_to_ignore=1, n_last_pages_to_ignore=1
         )
 
     def _find_and_remove_header_footer(
         self, text: str, n_chars: int, n_first_pages_to_ignore: int, n_last_pages_to_ignore: int
     ) -> str:
         """
         Heuristic to find footers and headers across different pages by searching for the longest common string.
+
         Pages in the text need to be separated by form feed character "\f".
         For headers, we only search in the first n_chars characters (for footer: last n_chars).
         Note: This heuristic uses exact matches and therefore works well for footers like "Copyright 2019 by XXX",
          but won't detect "Page 3 of 4" or similar.
 
         :param n_chars: The number of first/last characters where the header/footer shall be searched in.
         :param n_first_pages_to_ignore: The number of first pages to ignore (e.g. TOCs often don't contain footer/header).
@@ -178,14 +188,15 @@
         )
         text = "\f".join(pages)
         return text
 
     def _ngram(self, seq: str, n: int) -> Generator[str, None, None]:
         """
         Return all ngrams of length n from a text sequence. Each ngram consists of n words split by whitespace.
+
         :param seq: The sequence to generate ngrams from.
         :param n: The length of the ngrams to generate.
         :returns: A Generator generating all ngrams of length n from the given sequence.
         """
 
         # In order to maintain the original whitespace, but still consider \n and \t for n-gram tokenization,
         # we add a space here and remove it after creation of the ngrams again (see below)
@@ -198,14 +209,15 @@
         )
 
         return ngrams
 
     def _allngram(self, seq: str, min_ngram: int, max_ngram: int) -> Set[str]:
         """
         Generates all possible ngrams from a given sequence of text.
+
         Considering all ngram lengths between the minimum and maximum length.
 
         :param seq: The sequence to generate ngrams from.
         :param min_ngram: The minimum length of ngram to consider.
         :param max_ngram: The maximum length of ngram to consider.
         :returns: A set of all ngrams from the given sequence.
         """
@@ -213,14 +225,15 @@
         ngrams = map(partial(self._ngram, seq), lengths)
         res = set(chain.from_iterable(ngrams))
         return res
 
     def _find_longest_common_ngram(self, sequences: List[str], min_ngram: int = 3, max_ngram: int = 30) -> str:
         """
         Find the longest common ngram across a list of text sequences (e.g. start of pages).
+
         Considering all ngram lengths between the minimum and maximum length. Helpful for finding footers, headers etc.
         Empty sequences are ignored.
 
         :param sequences: The list of strings that shall be searched for common n_grams.
         :param max_ngram: The maximum length of ngram to consider.
         :param min_ngram: The minimum length of ngram to consider.
         :returns: The longest ngram that all sequences have in common.
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/preprocessors/document_splitter.py` & `haystack_ai-2.1.0rc1/haystack/components/preprocessors/document_splitter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from copy import deepcopy
-from typing import List, Literal
+from typing import Dict, List, Literal, Tuple
 
 from more_itertools import windowed
 
 from haystack import Document, component
 
 
 @component
@@ -19,14 +19,16 @@
     def __init__(
         self,
         split_by: Literal["word", "sentence", "page", "passage"] = "word",
         split_length: int = 200,
         split_overlap: int = 0,
     ):
         """
+        Initialize the DocumentSplitter.
+
         :param split_by: The unit by which the document should be split. Choose from "word" for splitting by " ",
             "sentence" for splitting by ".", "page" for splitting by "\\f" or "passage" for splitting by "\\n\\n".
         :param split_length: The maximum number of units in each split.
         :param split_overlap: The number of units that each split should overlap.
         """
 
         self.split_by = split_by
@@ -38,22 +40,24 @@
         if split_overlap < 0:
             raise ValueError("split_overlap must be greater than or equal to 0.")
         self.split_overlap = split_overlap
 
     @component.output_types(documents=List[Document])
     def run(self, documents: List[Document]):
         """
+        Split documents into smaller parts.
+
         Splits documents by the unit expressed in `split_by`, with a length of `split_length`
         and an overlap of `split_overlap`.
 
         :param documents: The documents to split.
 
         :returns: A dictionary with the following key:
             - `documents`: List of documents with the split texts. A metadata field "source_id" is added to each
-            document to keep track of the original document that was split. Other metadata are copied from the original
+            document to keep track of the original document that was split. Another metadata field "page_number" is added to each number to keep track of the page it belonged to in the original document. Other metadata are copied from the original
             document.
 
         :raises TypeError: if the input is not a list of Documents.
         :raises ValueError: if the content of a document is None.
         """
 
         if not isinstance(documents, list) or (documents and not isinstance(documents[0], Document)):
@@ -62,18 +66,20 @@
         split_docs = []
         for doc in documents:
             if doc.content is None:
                 raise ValueError(
                     f"DocumentSplitter only works with text documents but document.content for document ID {doc.id} is None."
                 )
             units = self._split_into_units(doc.content, self.split_by)
-            text_splits = self._concatenate_units(units, self.split_length, self.split_overlap)
+            text_splits, splits_pages = self._concatenate_units(units, self.split_length, self.split_overlap)
             metadata = deepcopy(doc.meta)
             metadata["source_id"] = doc.id
-            split_docs += [Document(content=txt, meta=metadata) for txt in text_splits]
+            split_docs += self._create_docs_from_splits(
+                text_splits=text_splits, splits_pages=splits_pages, meta=metadata
+            )
         return {"documents": split_docs}
 
     def _split_into_units(self, text: str, split_by: Literal["word", "sentence", "passage", "page"]) -> List[str]:
         if split_by == "page":
             split_at = "\f"
         elif split_by == "passage":
             split_at = "\n\n"
@@ -87,19 +93,44 @@
             )
         units = text.split(split_at)
         # Add the delimiter back to all units except the last one
         for i in range(len(units) - 1):
             units[i] += split_at
         return units
 
-    def _concatenate_units(self, elements: List[str], split_length: int, split_overlap: int) -> List[str]:
+    def _concatenate_units(
+        self, elements: List[str], split_length: int, split_overlap: int
+    ) -> Tuple[List[str], List[int]]:
         """
-        Concatenates the elements into parts of split_length units.
+        Concatenates the elements into parts of split_length units keeping track of the original page number that each element belongs.
         """
         text_splits = []
+        splits_pages = []
+        cur_page = 1
         segments = windowed(elements, n=split_length, step=split_length - split_overlap)
         for seg in segments:
             current_units = [unit for unit in seg if unit is not None]
             txt = "".join(current_units)
             if len(txt) > 0:
                 text_splits.append(txt)
-        return text_splits
+                splits_pages.append(cur_page)
+                processed_units = current_units[: split_length - split_overlap]
+                if self.split_by == "page":
+                    num_page_breaks = len(processed_units)
+                else:
+                    num_page_breaks = sum(processed_unit.count("\f") for processed_unit in processed_units)
+                cur_page += num_page_breaks
+        return text_splits, splits_pages
+
+    @staticmethod
+    def _create_docs_from_splits(text_splits: List[str], splits_pages: List[int], meta: Dict) -> List[Document]:
+        """
+        Creates Document objects from text splits enriching them with page number and the metadata of the original document.
+        """
+        documents: List[Document] = []
+
+        for i, txt in enumerate(text_splits):
+            meta = deepcopy(meta)
+            doc = Document(content=txt, meta=meta)
+            doc.meta["page_number"] = splits_pages[i]
+            documents.append(doc)
+        return documents
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/preprocessors/text_cleaner.py` & `haystack_ai-2.1.0rc1/haystack/components/preprocessors/text_cleaner.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,28 +4,32 @@
 
 from haystack import component
 
 
 @component
 class TextCleaner:
     """
-    A preprocessor component to clean text data. It can remove substrings matching a list of regular expressions,
-    convert text to lowercase, remove punctuation, and remove numbers.
+    A PreProcessor component to clean text data.
 
-    This is useful to cleanup text data before evaluation.
+    It can remove substrings matching a list of regular expressions, convert text to lowercase, remove punctuation,
+    and remove numbers.
+
+    This is useful to clean up text data before evaluation.
     """
 
     def __init__(
         self,
         remove_regexps: Optional[List[str]] = None,
         convert_to_lowercase: bool = False,
         remove_punctuation: bool = False,
         remove_numbers: bool = False,
     ):
         """
+        Initialize the TextCleaner component.
+
         :param remove_regexps: A list of regular expressions. If provided, it removes substrings
             matching these regular expressions from the text.
         :param convert_to_lowercase: If True, converts all characters to lowercase.
         :param remove_punctuation: If True, removes punctuation from the text.
         :param remove_numbers: If True, removes numerical digits from the text.
         """
         self._remove_regexps = remove_regexps
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/rankers/lost_in_the_middle.py` & `haystack_ai-2.1.0rc1/haystack/components/rankers/lost_in_the_middle.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from haystack import Document, component
 
 
 @component
 class LostInTheMiddleRanker:
     """
+    A LostInTheMiddle Ranker.
+
     Ranks documents based on the 'lost in the middle' order so that the most relevant documents are either at the
     beginning or end, while the least relevant are in the middle.
 
     LostInTheMiddleRanker assumes that some prior component in the pipeline has already ranked documents by relevance
     and requires no query as input but only documents. It is typically used as the last component before building a
     prompt for an LLM to prepare the input context for the LLM.
 
@@ -29,14 +31,16 @@
     for doc in result["documents"]:
         print(doc.content)
     ```
     """
 
     def __init__(self, word_count_threshold: Optional[int] = None, top_k: Optional[int] = None):
         """
+        Initialize the LostInTheMiddleRanker.
+
         If 'word_count_threshold' is specified, this ranker includes all documents up until the point where adding
         another document would exceed the 'word_count_threshold'. The last document that causes the threshold to
         be breached will be included in the resulting list of documents, but all subsequent documents will be
         discarded.
 
         :param word_count_threshold: The maximum total number of words across all documents selected by the ranker.
         :param top_k: The maximum number of documents to return.
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/rankers/meta_field.py` & `haystack_ai-2.1.0rc1/haystack/components/rankers/meta_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,15 @@
         weight: Optional[float] = None,
         ranking_mode: Optional[Literal["reciprocal_rank_fusion", "linear_score"]] = None,
         sort_order: Optional[Literal["ascending", "descending"]] = None,
         meta_value_type: Optional[Literal["float", "int", "date"]] = None,
     ):
         """
         Ranks a list of Documents based on the selected meta field by:
+
         1. Sorting the Documents by the meta field in descending or ascending order.
         2. Merging the rankings from the previous component and based on the meta field according to ranking mode and
         weight.
         3. Returning the top-k documents.
 
         :param documents:
             Documents to be ranked.
@@ -187,15 +188,15 @@
             If `sort_order` is not 'ascending' or 'descending'.
             If `meta_value_type` is not 'float', 'int', 'date' or `None`.
         """
         if not documents:
             return {"documents": []}
 
         top_k = top_k or self.top_k
-        weight = weight or self.weight
+        weight = weight if weight is not None else self.weight
         ranking_mode = ranking_mode or self.ranking_mode
         sort_order = sort_order or self.sort_order
         meta_value_type = meta_value_type or self.meta_value_type
         self._validate_params(
             weight=weight,
             top_k=top_k,
             ranking_mode=ranking_mode,
@@ -246,15 +247,15 @@
                 error=error,
             )
             return {"documents": documents[:top_k]}
 
         # Add the docs missing the meta_field back on the end
         sorted_by_meta = [doc for meta, doc in tuple_sorted_by_meta]
         sorted_documents = sorted_by_meta + docs_missing_meta_field
-        sorted_documents = self._merge_rankings(documents, sorted_documents, weight)
+        sorted_documents = self._merge_rankings(documents, sorted_documents, weight, ranking_mode)
         return {"documents": sorted_documents[:top_k]}
 
     def _parse_meta(
         self, docs_with_meta_field: List[Document], meta_value_type: Optional[Literal["float", "int", "date"]]
     ) -> List[Any]:
         """
         Parse the meta values stored under `self.meta_field` for the Documents provided in `docs_with_meta_field`.
@@ -292,26 +293,30 @@
                 error=error,
             )
             meta_values = [d.meta[self.meta_field] for d in docs_with_meta_field]
 
         return meta_values
 
     def _merge_rankings(
-        self, documents: List[Document], sorted_documents: List[Document], weight: float
+        self,
+        documents: List[Document],
+        sorted_documents: List[Document],
+        weight: float,
+        ranking_mode: Literal["reciprocal_rank_fusion", "linear_score"],
     ) -> List[Document]:
         """
         Merge the two different rankings for Documents sorted both by their content and by their meta field.
         """
         scores_map: Dict = defaultdict(int)
 
-        if self.ranking_mode == "reciprocal_rank_fusion":
+        if ranking_mode == "reciprocal_rank_fusion":
             for i, (document, sorted_doc) in enumerate(zip(documents, sorted_documents)):
                 scores_map[document.id] += self._calculate_rrf(rank=i) * (1 - weight)
                 scores_map[sorted_doc.id] += self._calculate_rrf(rank=i) * weight
-        elif self.ranking_mode == "linear_score":
+        elif ranking_mode == "linear_score":
             for i, (document, sorted_doc) in enumerate(zip(documents, sorted_documents)):
                 score = float(0)
                 if document.score is None:
                     logger.warning("The score wasn't provided; defaulting to 0.")
                 elif document.score < 0 or document.score > 1:
                     logger.warning(
                         "The score {score} for Document {document_id} is outside the [0,1] range; defaulting to 0",
@@ -329,22 +334,25 @@
 
         new_sorted_documents = sorted(documents, key=lambda doc: doc.score if doc.score else -1, reverse=True)
         return new_sorted_documents
 
     @staticmethod
     def _calculate_rrf(rank: int, k: int = 61) -> float:
         """
-        Calculates the reciprocal rank fusion. The constant K is set to 61 (60 was suggested by the original paper,
-        plus 1 as python lists are 0-based and the [paper](https://plg.uwaterloo.ca/~gvcormac/cormacksigir09-rrf.pdf) used 1-based ranking).
+        Calculates the reciprocal rank fusion.
+
+        The constant K is set to 61 (60 was suggested by the original paper, plus 1 as python lists are 0-based and
+        the [paper](https://plg.uwaterloo.ca/~gvcormac/cormacksigir09-rrf.pdf) used 1-based ranking).
         """
         return 1 / (k + rank)
 
     @staticmethod
     def _calc_linear_score(rank: int, amount: int) -> float:
         """
         Calculate the meta field score as a linear score between the greatest and the lowest score in the list.
+
         This linear scaling is useful for:
         - Reducing the effect of outliers
         - Creating scores that are meaningfully distributed in the range [0,1],
         similar to scores coming from a Retriever or Ranker.
         """
         return (amount - rank) / amount
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/rankers/transformers_similarity.py` & `haystack_ai-2.1.0rc1/haystack/components/rankers/transformers_similarity.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/components/readers/extractive.py` & `haystack_ai-2.1.0rc1/haystack/components/readers/extractive.py`

 * *Files 1% similar despite different names*

```diff
@@ -451,14 +451,16 @@
 
         return keep
 
     def deduplicate_by_overlap(
         self, answers: List[ExtractedAnswer], overlap_threshold: Optional[float]
     ) -> List[ExtractedAnswer]:
         """
+        De-duplicates overlapping Extractive Answers.
+
         De-duplicates overlapping Extractive Answers from the same document based on how much the spans of the
         answers overlap.
 
         :param answers:
             List of answers to be deduplicated.
         :param overlap_threshold:
             If set this will remove duplicate answers if they have an overlap larger than the
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/retrievers/filter_retriever.py` & `haystack_ai-2.1.0rc1/haystack/components/retrievers/filter_retriever.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         init_params = data.get("init_parameters", {})
         if "document_store" not in init_params:
             raise DeserializationError("Missing 'document_store' in serialization data")
         if "type" not in init_params["document_store"]:
             raise DeserializationError("Missing 'type' in document store's serialization data")
         try:
             module_name, type_ = init_params["document_store"]["type"].rsplit(".", 1)
-            logger.debug("Trying to import module '{module}'", module=module_name)
+            logger.debug("Trying to import module '{module_name}'", module_name=module_name)
             module = importlib.import_module(module_name)
         except (ImportError, DeserializationError) as e:
             raise DeserializationError(
                 f"DocumentStore of type '{init_params['document_store']['type']}' not correctly imported"
             ) from e
 
         docstore_class = getattr(module, type_)
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/retrievers/in_memory/bm25_retriever.py` & `haystack_ai-2.1.0rc1/haystack/components/retrievers/in_memory/bm25_retriever.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/components/routers/conditional_router.py` & `haystack_ai-2.1.0rc1/haystack/components/routers/conditional_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,14 +159,16 @@
         for route in routes:
             # output_type needs to be deserialized from a string to a type
             route["output_type"] = deserialize_type(route["output_type"])
         return default_from_dict(cls, data)
 
     def run(self, **kwargs):
         """
+        Executes the routing logic.
+
         Executes the routing logic by evaluating the specified boolean condition expressions for each route in the order they are listed.
         The method directs the flow of data to the output specified in the first route whose `condition` is True.
 
         :param kwargs: All variables used in the `condition` expressed in the routes. When the component is used in a
             pipeline, these variables are passed from the previous component's output.
 
         :returns: A dictionary where the key is the `output_name` of the selected route and the value is the `output`
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/routers/file_type_router.py` & `haystack_ai-2.1.0rc1/haystack/components/routers/file_type_router.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,75 @@
 import mimetypes
+import re
 from collections import defaultdict
 from pathlib import Path
 from typing import Dict, List, Optional, Union
 
 from haystack import component, logging
 from haystack.dataclasses import ByteStream
 
 logger = logging.getLogger(__name__)
 
 
 @component
 class FileTypeRouter:
     """
-    FileTypeRouter takes a list of data sources (file paths or byte streams) and groups them by their corresponding
-    MIME types.
+    Groups a list of data sources by their MIME types.
 
-    For file paths, MIME types are inferred from their extensions, while for byte streams, MIME types
-    are determined from the provided metadata.
-
-    The set of MIME types to consider is specified during the initialization of the component.
-
-    This component is useful when you need to classify a large collection of files or data streams according to their
-    MIME types and route them to different components for further processing.
+    FileTypeRouter groups a list of data sources (file paths or byte streams) by their MIME types, allowing
+    for flexible routing of files to different components based on their content type. It supports both exact MIME type
+    matching and pattern matching using regular expressions.
+
+    For file paths, MIME types are inferred from their extensions, while for byte streams, MIME types are determined from
+    the provided metadata. This enables the router to classify a diverse collection of files and data streams for
+    specialized processing.
+
+    The router's flexibility is enhanced by the support for regex patterns in the `mime_types` parameter, allowing users
+    to specify broad categories (e.g., 'audio/*' or 'text/*') or more specific types with regex patterns. This feature
+    is designed to be backward compatible, treating MIME types without regex patterns as exact matches.
 
     Usage example:
     ```python
     from haystack.components.routers import FileTypeRouter
+    from pathlib import Path
+
+    # For exact MIME type matching
+    router = FileTypeRouter(mime_types=["text/plain", "application/pdf"])
 
-    router = FileTypeRouter(mime_types=["text/plain"])
+    # For flexible matching using regex, to handle all audio types
+    router_with_regex = FileTypeRouter(mime_types=[r"audio/.*", r"text/plain"])
 
-    print(router.run(sources=["text_file.txt", "pdf_file.pdf"]))
+    sources = [Path("file.txt"), Path("document.pdf"), Path("song.mp3")]
+    print(router.run(sources=sources))
+    print(router_with_regex.run(sources=sources))
 
-    # defaultdict(<class 'list'>, {'text/plain': [PosixPath('text_file.txt')],
-    #                              'unclassified': [PosixPath('pdf_file.pdf')]})
+    # Expected output:
+    # {'text/plain': [PosixPath('file.txt')], 'application/pdf': [PosixPath('document.pdf')], 'unclassified': [PosixPath('song.mp3')]}
+    # {'audio/.*': [PosixPath('song.mp3')], 'text/plain': [PosixPath('file.txt')], 'unclassified': [PosixPath('document.pdf')]}
     ```
+
+    :param mime_types: A list of MIME types or regex patterns to classify the incoming files or data streams.
     """
 
     def __init__(self, mime_types: List[str]):
         """
+        Initialize the FileTypeRouter component.
+
         :param mime_types: A list of file mime types to consider when routing files
             (e.g. `["text/plain", "audio/x-wav", "image/jpeg"]`).
         """
         if not mime_types:
             raise ValueError("The list of mime types cannot be empty.")
 
+        self.mime_type_patterns = []
         for mime_type in mime_types:
             if not self._is_valid_mime_type_format(mime_type):
-                raise ValueError(
-                    f"Unknown mime type: '{mime_type}'. Ensure you passed a list of strings in the 'mime_types' parameter"
-                )
+                raise ValueError(f"Invalid mime type or regex pattern: '{mime_type}'.")
+            pattern = re.compile(mime_type)
+            self.mime_type_patterns.append(pattern)
 
         component.set_output_types(self, unclassified=List[Path], **{mime_type: List[Path] for mime_type in mime_types})
         self.mime_types = mime_types
 
     def run(self, sources: List[Union[str, Path, ByteStream]]) -> Dict[str, List[Union[ByteStream, Path]]]:
         """
         Categorizes the provided data sources by their MIME types.
@@ -62,28 +79,32 @@
         :returns: A dictionary where the keys are MIME types (or `"unclassified"`) and the values are lists of data sources.
         """
 
         mime_types = defaultdict(list)
         for source in sources:
             if isinstance(source, str):
                 source = Path(source)
-
             if isinstance(source, Path):
                 mime_type = self._get_mime_type(source)
             elif isinstance(source, ByteStream):
-                mime_type = source.meta.get("content_type")
+                mime_type = source.meta.get("content_type", None)
             else:
-                raise ValueError(f"Unsupported data source type: {type(source)}")
+                raise ValueError(f"Unsupported data source type: {type(source).__name__}")
 
-            if mime_type in self.mime_types:
-                mime_types[mime_type].append(source)
-            else:
+            matched = False
+            if mime_type:
+                for pattern in self.mime_type_patterns:
+                    if pattern.fullmatch(mime_type):
+                        mime_types[pattern.pattern].append(source)
+                        matched = True
+                        break
+            if not matched:
                 mime_types["unclassified"].append(source)
 
-        return mime_types
+        return dict(mime_types)
 
     def _get_mime_type(self, path: Path) -> Optional[str]:
         """
         Get the MIME type of the provided file path.
 
         :param path: The file path to get the MIME type for.
 
@@ -92,21 +113,25 @@
         extension = path.suffix.lower()
         mime_type = mimetypes.guess_type(path.as_posix())[0]
         # lookup custom mappings if the mime type is not found
         return self._get_custom_mime_mappings().get(extension, mime_type)
 
     def _is_valid_mime_type_format(self, mime_type: str) -> bool:
         """
-        Check if the provided MIME type is in valid format
+        Checks if the provided MIME type string is a valid regex pattern.
 
-        :param mime_type: The MIME type to check.
-
-        :returns: `True` if the provided MIME type is a valid MIME type format, `False` otherwise.
-        """
-        return mime_type in mimetypes.types_map.values() or mime_type in self._get_custom_mime_mappings().values()
+        :param mime_type: The MIME type or regex pattern to validate.
+        :raises ValueError: If the mime_type is not a valid regex pattern.
+        :returns: Always True because a ValueError is raised for invalid patterns.
+        """
+        try:
+            re.compile(mime_type)
+            return True
+        except re.error:
+            raise ValueError(f"Invalid regex pattern '{mime_type}'.")
 
     @staticmethod
     def _get_custom_mime_mappings() -> Dict[str, str]:
         """
         Returns a dictionary of custom file extension to MIME type mappings.
         """
         # we add markdown because it is not added by the mimetypes module
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/routers/metadata_router.py` & `haystack_ai-2.1.0rc1/haystack/components/routers/metadata_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,16 @@
             ```
         """
         self.rules = rules
         component.set_output_types(self, unmatched=List[Document], **{edge: List[Document] for edge in rules})
 
     def run(self, documents: List[Document]):
         """
+        Route the documents.
+
         Route the documents to different edges based on their fields content and the rules specified during initialization.
         If a document does not match any of the rules, it is routed to a connection named "unmatched".
 
         :param documents: A list of documents to route to different edges.
 
         :returns: A dictionary where the keys are the names of the output connections (including `"unmatched"`)
             and the values are lists of routed documents.
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/routers/text_language_router.py` & `haystack_ai-2.1.0rc1/haystack/components/routers/text_language_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,27 +40,30 @@
     result = p.run({"text_language_router": {"text": "ένα ελληνικό κείμενο"}})
     assert result["text_language_router"]["unmatched"] == "ένα ελληνικό κείμενο"
     ```
     """
 
     def __init__(self, languages: Optional[List[str]] = None):
         """
+        Initialize the TextLanguageRouter component.
+
         :param languages: A list of languages in ISO code, each corresponding to a different output connection.
             For supported languages, see the [`langdetect` documentation](https://github.com/Mimino666/langdetect#languages).
             If not specified, the default is `["en"]`.
         """
         langdetect_import.check()
         if not languages:
             languages = ["en"]
         self.languages = languages
         component.set_output_types(self, unmatched=str, **{language: str for language in languages})
 
     def run(self, text: str) -> Dict[str, str]:
         """
         Route the text to one of different output connections based on its language.
+
         If the text does not match any of the languages specified at initialization, it is routed to
         a connection named "unmatched".
 
         :param text: A string to route to different edges based on its language.
 
         :returns: A dictionary of length one in which the key is the language (or `"unmatched"`)
             and the value is the text.
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/samplers/top_p.py` & `haystack_ai-2.1.0rc1/haystack/components/samplers/top_p.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         self.top_p = top_p
         self.score_field = score_field
 
     @component.output_types(documents=List[Document])
     def run(self, documents: List[Document], top_p: Optional[float] = None):
         """
         Filters documents using top-p sampling based on their scores.
+
         If the specified top_p results in no documents being selected (especially in cases of a low top_p value), the
         method returns the document with the highest similarity score.
 
         :param documents: List of Document objects to be filtered.
         :param top_p: Optional. A float to override the cumulative probability threshold set during initialization.
 
         :returns: A dictionary with the following key:
@@ -109,14 +110,15 @@
             selected_docs = [documents[int(highest_prob_indices[0].item())]]
 
         return {"documents": selected_docs}
 
     def _collect_scores(self, documents: List[Document]) -> List[float]:
         """
         Collect the scores from the documents' metadata.
+
         :param documents: List of Documents.
         :return: List of scores.
         """
         if self.score_field:
             missing_scores_docs = [d for d in documents if self.score_field not in d.meta]
             if missing_scores_docs:
                 missing_scores_docs_ids = [d.id for d in missing_scores_docs if d.id]
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/validators/json_schema.py` & `haystack_ai-2.1.0rc1/haystack/components/validators/json_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,16 @@
         "Please match the following schema:\n"
         "{json_schema}\n"
         "and provide the corrected JSON content ONLY."
     )
 
     def __init__(self, json_schema: Optional[Dict[str, Any]] = None, error_template: Optional[str] = None):
         """
+        Initialize the JsonSchemaValidator component.
+
         :param json_schema: A dictionary representing the [JSON schema](https://json-schema.org/) against which
             the messages' content is validated.
         :param error_template: A custom template string for formatting the error message in case of validation failure.
         """
         jsonschema_import.check()
         self.json_schema = json_schema
         self.error_template = error_template
@@ -182,16 +184,17 @@
         :param json_schema: The JSON schema to check
         :return: `True` if the schema is a valid OpenAI function calling schema; otherwise, `False`.
         """
         return all(key in json_schema for key in ["name", "description", "parameters"])
 
     def _recursive_json_to_object(self, data: Any) -> Any:
         """
-        Recursively traverses a data structure (dictionary or list), converting any string values
-        that are valid JSON objects into dictionary objects, and returns a new data structure.
+        Convert any string values that are valid JSON objects into dictionary objects.
+
+        Returns a new data structure.
 
         :param data: The data structure to be traversed.
         :return: A new data structure with JSON strings converted to dictionary objects.
         """
         if isinstance(data, list):
             return [self._recursive_json_to_object(item) for item in data]
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/websearch/searchapi.py` & `haystack_ai-2.1.0rc1/haystack/components/websearch/searchapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 from typing import Any, Dict, List, Optional, Union
 
 import requests
 
 from haystack import ComponentError, Document, component, default_from_dict, default_to_dict, logging
 from haystack.utils import Secret, deserialize_secrets_inplace
 
@@ -17,16 +16,14 @@
 
 
 @component
 class SearchApiWebSearch:
     """
     Uses [SearchApi](https://www.searchapi.io/) to search the web for relevant documents.
 
-    See the [SearchApi website](https://www.searchapi.io/) for more details.
-
     Usage example:
     ```python
     from haystack.components.websearch import SearchApiWebSearch
     from haystack.utils import Secret
 
     websearch = SearchApiWebSearch(top_k=10, api_key=Secret.from_token("test-api-key"))
     results = websearch.run(query="Who is the boyfriend of Olivia Wilde?")
@@ -40,26 +37,33 @@
         self,
         api_key: Secret = Secret.from_env_var("SEARCHAPI_API_KEY"),
         top_k: Optional[int] = 10,
         allowed_domains: Optional[List[str]] = None,
         search_params: Optional[Dict[str, Any]] = None,
     ):
         """
+        Initialize the SearchApiWebSearch component.
+
         :param api_key: API key for the SearchApi API
         :param top_k: Number of documents to return.
         :param allowed_domains: List of domains to limit the search to.
         :param search_params: Additional parameters passed to the SearchApi API.
             For example, you can set 'num' to 100 to increase the number of search results.
             See the [SearchApi website](https://www.searchapi.io/) for more details.
+
+            The default search engine is Google, however, users can change it by setting the `engine`
+            parameter in the `search_params`.
         """
 
         self.api_key = api_key
         self.top_k = top_k
         self.allowed_domains = allowed_domains
         self.search_params = search_params or {}
+        if "engine" not in self.search_params:
+            self.search_params["engine"] = "google"
 
         # Ensure that the API key is resolved.
         _ = self.api_key.resolve_value()
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
@@ -97,18 +101,16 @@
         :returns: A dictionary with the following keys:
             - "documents": List of documents returned by the search engine.
             - "links": List of links returned by the search engine.
         :raises TimeoutError: If the request to the SearchApi API times out.
         :raises SearchApiError: If an error occurs while querying the SearchApi API.
         """
         query_prepend = "OR ".join(f"site:{domain} " for domain in self.allowed_domains) if self.allowed_domains else ""
-
-        payload = json.dumps({"q": query_prepend + " " + query, **self.search_params})
+        payload = {"q": query_prepend + " " + query, **self.search_params}
         headers = {"Authorization": f"Bearer {self.api_key.resolve_value()}", "X-SearchApi-Source": "Haystack"}
-
         try:
             response = requests.get(SEARCHAPI_BASE_URL, headers=headers, params=payload, timeout=90)
             response.raise_for_status()  # Will raise an HTTPError for bad responses
         except requests.Timeout as error:
             raise TimeoutError(f"Request to {self.__class__.__name__} timed out.") from error
 
         except requests.RequestException as e:
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/websearch/serper_dev.py` & `haystack_ai-2.1.0rc1/haystack/core/serialization.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,170 +1,190 @@
-import json
-from typing import Any, Dict, List, Optional, Union
+# SPDX-FileCopyrightText: 2022-present deepset GmbH <info@deepset.ai>
+#
+# SPDX-License-Identifier: Apache-2.0
+import inspect
+from collections.abc import Callable
+from dataclasses import dataclass
+from typing import Any, Dict, Optional, Type
 
-import requests
+from haystack.core.component.component import _hook_component_init
+from haystack.core.errors import DeserializationError, SerializationError
 
-from haystack import ComponentError, Document, component, default_from_dict, default_to_dict, logging
-from haystack.utils import Secret, deserialize_secrets_inplace
 
-logger = logging.getLogger(__name__)
+@dataclass(frozen=True)
+class DeserializationCallbacks:
+    """
+    Callback functions that are invoked in specific stages of the pipeline deserialization process.
 
+    :param component_pre_init:
+        Invoked just before a component instance is
+        initialized. Receives the following inputs:
+        `component_name` (`str`), `component_class` (`Type`), `init_params` (`Dict[str, Any]`).
+
+        The callback is allowed to modify the `init_params`
+        dictionary, which contains all the parameters that
+        are passed to the component's constructor.
+    """
 
-SERPERDEV_BASE_URL = "https://google.serper.dev/search"
+    component_pre_init: Optional[Callable] = None
 
 
-class SerperDevError(ComponentError):
-    ...
+def component_to_dict(obj: Any) -> Dict[str, Any]:
+    """
+    Converts a component instance into a dictionary.
 
+    If a `to_dict` method is present in the component instance, that will be used instead of the default method.
 
-@component
-class SerperDevWebSearch:
+    :param obj:
+        The component to be serialized.
+    :returns:
+        A dictionary representation of the component.
+
+    :raises SerializationError:
+        If the component doesn't have a `to_dict` method and the values of the init parameters can't be determined.
     """
-    Uses [Serper](https://serper.dev/) to search the web for relevant documents.
+    if hasattr(obj, "to_dict"):
+        return obj.to_dict()
 
-    See the [Serper Dev website](https://serper.dev/) for more details.
+    init_parameters = {}
+    for name, param in inspect.signature(obj.__init__).parameters.items():
+        # Ignore `args` and `kwargs`, used by the default constructor
+        if name in ("args", "kwargs"):
+            continue
+        try:
+            # This only works if the Component constructor assigns the init
+            # parameter to an instance variable or property with the same name
+            param_value = getattr(obj, name)
+        except AttributeError as e:
+            # If the parameter doesn't have a default value, raise an error
+            if param.default is param.empty:
+                raise SerializationError(
+                    f"Cannot determine the value of the init parameter '{name}' for the class {obj.__class__.__name__}."
+                    f"You can fix this error by assigning 'self.{name} = {name}' or adding a "
+                    f"custom serialization method 'to_dict' to the class."
+                ) from e
+            # In case the init parameter was not assigned, we use the default value
+            param_value = param.default
+        init_parameters[name] = param_value
 
-    Usage example:
-    ```python
-    from haystack.components.websearch import SerperDevWebSearch
-    from haystack.utils import Secret
+    return default_to_dict(obj, **init_parameters)
 
-    websearch = SerperDevWebSearch(top_k=10, api_key=Secret.from_token("test-api-key"))
-    results = websearch.run(query="Who is the boyfriend of Olivia Wilde?")
 
-    assert results["documents"]
-    assert results["links"]
-    ```
+def generate_qualified_class_name(cls: Type[object]) -> str:
+    """
+    Generates a qualified class name for a class.
+
+    :param cls:
+        The class whose qualified name is to be generated.
+    :returns:
+        The qualified name of the class.
     """
+    return f"{cls.__module__}.{cls.__name__}"
+
+
+def component_from_dict(
+    cls: Type[object], data: Dict[str, Any], name: str, callbacks: Optional[DeserializationCallbacks] = None
+) -> Any:
+    """
+    Creates a component instance from a dictionary.
+
+    If a `from_dict` method is present in the component class, that will be used instead of the default method.
+
+    :param cls:
+        The class to be used for deserialization.
+    :param data:
+        The serialized data.
+    :param name:
+        The name of the component.
+    :param callbacks:
+        Callbacks to invoke during deserialization.
+    :returns:
+        The deserialized component.
+    """
+
+    def component_pre_init_callback(component_cls, init_params):
+        assert callbacks is not None
+        assert callbacks.component_pre_init is not None
+        callbacks.component_pre_init(name, component_cls, init_params)
+
+    def do_from_dict():
+        if hasattr(cls, "from_dict"):
+            return cls.from_dict(data)
 
-    def __init__(
-        self,
-        api_key: Secret = Secret.from_env_var("SERPERDEV_API_KEY"),
-        top_k: Optional[int] = 10,
-        allowed_domains: Optional[List[str]] = None,
-        search_params: Optional[Dict[str, Any]] = None,
-    ):
-        """
-        :param api_key: API key for the Serper API.
-        :param top_k: Number of documents to return.
-        :param allowed_domains: List of domains to limit the search to.
-        :param search_params: Additional parameters passed to the Serper API.
-            For example, you can set 'num' to 20 to increase the number of search results.
-            See the [Serper website](https://serper.dev/) for more details.
-        """
-        self.api_key = api_key
-        self.top_k = top_k
-        self.allowed_domains = allowed_domains
-        self.search_params = search_params or {}
-
-        # Ensure that the API key is resolved.
-        _ = self.api_key.resolve_value()
-
-    def to_dict(self) -> Dict[str, Any]:
-        """
-        Serializes the component to a dictionary.
-
-        :returns:
-                Dictionary with serialized data.
-        """
-        return default_to_dict(
-            self,
-            top_k=self.top_k,
-            allowed_domains=self.allowed_domains,
-            search_params=self.search_params,
-            api_key=self.api_key.to_dict(),
-        )
-
-    @classmethod
-    def from_dict(cls, data: Dict[str, Any]) -> "SerperDevWebSearch":
-        """
-        Serializes the component to a dictionary.
-
-        :returns:
-                Dictionary with serialized data.
-        """
-        deserialize_secrets_inplace(data["init_parameters"], keys=["api_key"])
         return default_from_dict(cls, data)
 
-    @component.output_types(documents=List[Document], links=List[str])
-    def run(self, query: str) -> Dict[str, Union[List[Document], List[str]]]:
-        """
-        Use [Serper](https://serper.dev/) to search the web.
-
-        :param query: Search query.
-        :returns: A dictionary with the following keys:
-            - "documents": List of documents returned by the search engine.
-            - "links": List of links returned by the search engine.
-        :raises SerperDevError: If an error occurs while querying the SerperDev API.
-        :raises TimeoutError: If the request to the SerperDev API times out.
-        """
-        query_prepend = "OR ".join(f"site:{domain} " for domain in self.allowed_domains) if self.allowed_domains else ""
-
-        payload = json.dumps(
-            {"q": query_prepend + query, "gl": "us", "hl": "en", "autocorrect": True, **self.search_params}
-        )
-        headers = {"X-API-KEY": self.api_key.resolve_value(), "Content-Type": "application/json"}
+    if callbacks is None or callbacks.component_pre_init is None:
+        return do_from_dict()
 
-        try:
-            response = requests.post(SERPERDEV_BASE_URL, headers=headers, data=payload, timeout=30)  # type: ignore
-            response.raise_for_status()  # Will raise an HTTPError for bad responses
-        except requests.Timeout as error:
-            raise TimeoutError(f"Request to {self.__class__.__name__} timed out.") from error
-
-        except requests.RequestException as e:
-            raise SerperDevError(f"An error occurred while querying {self.__class__.__name__}. Error: {e}") from e
-
-        # If we reached this point, it means the request was successful and we can proceed
-        json_result = response.json()
-
-        # we get the snippet from the json result and put it in the content field of the document
-        organic = [
-            Document(meta={k: v for k, v in d.items() if k != "snippet"}, content=d["snippet"])
-            for d in json_result["organic"]
-        ]
-
-        # answer box is what search engine shows as a direct answer to the query
-        answer_box = []
-        if "answerBox" in json_result:
-            answer_dict = json_result["answerBox"]
-            highlighted_answers = answer_dict.get("snippetHighlighted")
-            answer_box_content = None
-            # Check if highlighted_answers is a list and has at least one element
-            if isinstance(highlighted_answers, list) and len(highlighted_answers) > 0:
-                answer_box_content = highlighted_answers[0]
-            elif isinstance(highlighted_answers, str):
-                answer_box_content = highlighted_answers
-            if not answer_box_content:
-                for key in ["snippet", "answer", "title"]:
-                    if key in answer_dict:
-                        answer_box_content = answer_dict[key]
-                        break
-            if answer_box_content:
-                answer_box = [
-                    Document(
-                        content=answer_box_content,
-                        meta={"title": answer_dict.get("title", ""), "link": answer_dict.get("link", "")},
-                    )
-                ]
-
-        # these are related questions that search engine shows
-        people_also_ask = []
-        if "peopleAlsoAsk" in json_result:
-            for result in json_result["peopleAlsoAsk"]:
-                title = result.get("title", "")
-                people_also_ask.append(
-                    Document(
-                        content=result["snippet"] if result.get("snippet") else title,
-                        meta={"title": title, "link": result.get("link", None)},
-                    )
-                )
-
-        documents = answer_box + organic + people_also_ask
-
-        links = [result["link"] for result in json_result["organic"]]
-
-        logger.debug(
-            "Serper Dev returned {number_documents} documents for the query '{query}'",
-            number_documents=len(documents),
-            query=query,
-        )
-        return {"documents": documents[: self.top_k], "links": links[: self.top_k]}
+    with _hook_component_init(component_pre_init_callback):
+        return do_from_dict()
+
+
+def default_to_dict(obj: Any, **init_parameters) -> Dict[str, Any]:
+    """
+    Utility function to serialize an object to a dictionary.
+
+    This is mostly necessary for components but can be used by any object.
+    `init_parameters` are parameters passed to the object class `__init__`.
+    They must be defined explicitly as they'll be used when creating a new
+    instance of `obj` with `from_dict`. Omitting them might cause deserialisation
+    errors or unexpected behaviours later, when calling `from_dict`.
+
+    An example usage:
+
+    ```python
+    class MyClass:
+        def __init__(self, my_param: int = 10):
+            self.my_param = my_param
+
+        def to_dict(self):
+            return default_to_dict(self, my_param=self.my_param)
+
+
+    obj = MyClass(my_param=1000)
+    data = obj.to_dict()
+    assert data == {
+        "type": "MyClass",
+        "init_parameters": {
+            "my_param": 1000,
+        },
+    }
+    ```
+
+    :param obj:
+        The object to be serialized.
+    :param init_parameters:
+        The parameters used to create a new instance of the class.
+    :returns:
+        A dictionary representation of the instance.
+    """
+    return {"type": generate_qualified_class_name(type(obj)), "init_parameters": init_parameters}
+
+
+def default_from_dict(cls: Type[object], data: Dict[str, Any]) -> Any:
+    """
+    Utility function to deserialize a dictionary to an object.
+
+    This is mostly necessary for components but can be used by any object.
+
+    The function will raise a `DeserializationError` if the `type` field in `data` is
+    missing or it doesn't match the type of `cls`.
+
+    If `data` contains an `init_parameters` field it will be used as parameters to create
+    a new instance of `cls`.
+
+    :param cls:
+        The class to be used for deserialization.
+    :param data:
+        The serialized data.
+    :returns:
+        The deserialized object.
+
+    :raises DeserializationError:
+        If the `type` field in `data` is missing or it doesn't match the type of `cls`.
+    """
+    init_params = data.get("init_parameters", {})
+    if "type" not in data:
+        raise DeserializationError("Missing 'type' in serialization data")
+    if data["type"] != generate_qualified_class_name(cls):
+        raise DeserializationError(f"Class '{data['type']}' can't be deserialized as '{cls.__name__}'")
+    return cls(**init_params)
```

### Comparing `haystack_ai-2.0.1rc2/haystack/components/writers/document_writer.py` & `haystack_ai-2.1.0rc1/haystack/components/writers/document_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         Data that is sent to Posthog for usage analytics.
         """
         return {"document_store": type(self.document_store).__name__}
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
+
         :returns:
             Dictionary with serialized data.
         """
         return default_to_dict(self, document_store=self.document_store.to_dict(), policy=self.policy.name)
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "DocumentWriter":
@@ -72,15 +73,15 @@
         if "document_store" not in init_params:
             raise DeserializationError("Missing 'document_store' in serialization data")
         if "type" not in init_params["document_store"]:
             raise DeserializationError("Missing 'type' in document store's serialization data")
 
         try:
             module_name, type_ = init_params["document_store"]["type"].rsplit(".", 1)
-            logger.debug("Trying to import module '{module}'", module=module_name)
+            logger.debug("Trying to import module '{module_name}'", module_name=module_name)
             module = importlib.import_module(module_name)
         except (ImportError, DeserializationError) as e:
             raise DeserializationError(
                 f"DocumentStore of type '{init_params['document_store']['type']}' not correctly imported"
             ) from e
 
         docstore_class = getattr(module, type_)
```

### Comparing `haystack_ai-2.0.1rc2/haystack/core/errors.py` & `haystack_ai-2.1.0rc1/haystack/core/errors.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/core/type_utils.py` & `haystack_ai-2.1.0rc1/haystack/core/type_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
     return all(_types_are_compatible(*args) for args in zip(sender_args, receiver_args))
 
 
 def _type_name(type_):
     """
     Util methods to get a nice readable representation of a type.
+
     Handles Optional and Literal in a special way to make it more readable.
     """
     # Literal args are strings, so we wrap them in quotes to make it clear
     if isinstance(type_, str):
         return f"'{type_}'"
 
     name = getattr(type_, "__name__", str(type_))
```

### Comparing `haystack_ai-2.0.1rc2/haystack/core/component/component.py` & `haystack_ai-2.1.0rc1/haystack/core/component/component.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,27 +67,51 @@
     `@component.output`.
 
 """
 
 import inspect
 import sys
 from collections.abc import Callable
+from contextlib import contextmanager
+from contextvars import ContextVar
 from copy import deepcopy
 from types import new_class
 from typing import Any, Dict, Optional, Protocol, runtime_checkable
 
 from haystack import logging
 from haystack.core.errors import ComponentError
 
 from .sockets import Sockets
 from .types import InputSocket, OutputSocket, _empty
 
 logger = logging.getLogger(__name__)
 
 
+# Callback inputs: component class (Type) and init parameters (as keyword arguments) (Dict[str, Any]).
+_COMPONENT_PRE_INIT_CALLBACK: ContextVar[Optional[Callable]] = ContextVar("component_pre_init_callback", default=None)
+
+
+@contextmanager
+def _hook_component_init(callback: Callable):
+    """
+    Context manager to set a callback that will be invoked before a component's constructor is called.
+
+    The callback receives the component class and the init parameters (as keyword arguments) and can modify the init
+    parameters in place.
+
+    :param callback:
+        Callback function to invoke.
+    """
+    token = _COMPONENT_PRE_INIT_CALLBACK.set(callback)
+    try:
+        yield
+    finally:
+        _COMPONENT_PRE_INIT_CALLBACK.reset(token)
+
+
 @runtime_checkable
 class Component(Protocol):
     """
     Note this is only used by type checking tools.
 
     In order to implement the `Component` protocol, custom components need to
     have a `run` method. The signature of the method and its return value
@@ -119,21 +143,49 @@
     if sys.version_info >= (3, 9):
         run: Callable[..., Dict[str, Any]]
     else:
         run: Callable
 
 
 class ComponentMeta(type):
+    @staticmethod
+    def positional_to_kwargs(cls_type, args) -> Dict[str, Any]:
+        """
+        Convert positional arguments to keyword arguments based on the signature of the `__init__` method.
+        """
+        init_signature = inspect.signature(cls_type.__init__)
+        init_params = {name: info for name, info in init_signature.parameters.items() if name != "self"}
+
+        out = {}
+        for arg, (name, info) in zip(args, init_params.items()):
+            if info.kind == inspect.Parameter.VAR_POSITIONAL:
+                raise ComponentError(
+                    "Pre-init hooks do not support components with variadic positional args in their init method"
+                )
+
+            assert info.kind in (inspect.Parameter.POSITIONAL_OR_KEYWORD, inspect.Parameter.POSITIONAL_ONLY)
+            out[name] = arg
+        return out
+
     def __call__(cls, *args, **kwargs):
         """
-        This method is called when clients instantiate a Component and
-        runs before __new__ and __init__.
+        This method is called when clients instantiate a Component and runs before __new__ and __init__.
         """
         # This will call __new__ then __init__, giving us back the Component instance
-        instance = super().__call__(*args, **kwargs)
+        pre_init_hook = _COMPONENT_PRE_INIT_CALLBACK.get()
+        if pre_init_hook is None:
+            instance = super().__call__(*args, **kwargs)
+        else:
+            named_positional_args = ComponentMeta.positional_to_kwargs(cls, args)
+            assert (
+                set(named_positional_args.keys()).intersection(kwargs.keys()) == set()
+            ), "positional and keyword arguments overlap"
+            kwargs.update(named_positional_args)
+            pre_init_hook(cls, kwargs)
+            instance = super().__call__(**kwargs)
 
         # Before returning, we have the chance to modify the newly created
         # Component instance, so we take the chance and set up the I/O sockets
 
         # If `component.set_output_types()` was called in the component constructor,
         # `__haystack_output__` is already populated, no need to do anything.
         if not hasattr(instance, "__haystack_output__"):
@@ -180,14 +232,15 @@
 
         return instance
 
 
 def _component_repr(component: Component) -> str:
     """
     All Components override their __repr__ method with this one.
+
     It prints the component name and the input/output sockets.
     """
     result = object.__repr__(component)
     if pipeline := getattr(component, "__haystack_added_to_pipeline__"):
         # This Component has been added in a Pipeline, let's get the name from there.
         result += f"\n{pipeline.get_component_name(component)}"
 
@@ -211,15 +264,15 @@
     Raises:
         ComponentError: if the class provided has no `run()` method or otherwise doesn't respect the component contract.
     """
 
     def __init__(self):
         self.registry = {}
 
-    def set_input_type(self, instance, name: str, type: Any, default: Any = _empty):
+    def set_input_type(self, instance, name: str, type: Any, default: Any = _empty):  # noqa: A002
         """
         Add a single input socket to the component instance.
 
         :param instance: Component instance where the input type will be added.
         :param name: name of the input socket.
         :param type: type of the input socket.
         :param default: default value of the input socket, defaults to _empty
@@ -235,15 +288,15 @@
         Use as:
 
         ```python
         @component
         class MyComponent:
 
             def __init__(self, value: int):
-                component.set_input_types(value_1=str, value_2=str)
+                component.set_input_types(self, value_1=str, value_2=str)
                 ...
 
             @component.output_types(output_1=int, output_2=str)
             def run(self, **kwargs):
                 return {"output_1": kwargs["value_1"], "output_2": ""}
         ```
 
@@ -252,15 +305,15 @@
         For example:
 
         ```python
         @component
         class MyComponent:
 
             def __init__(self, value: int):
-                component.set_input_types(value_1=str, value_2=str)
+                component.set_input_types(self, value_1=str, value_2=str)
                 ...
 
             @component.output_types(output_1=int, output_2=str)
             def run(self, value_0: str, value_1: Optional[str] = None, **kwargs):
                 return {"output_1": kwargs["value_1"], "output_2": ""}
         ```
 
@@ -271,25 +324,24 @@
         """
         instance.__haystack_input__ = Sockets(
             instance, {name: InputSocket(name=name, type=type_) for name, type_ in types.items()}, InputSocket
         )
 
     def set_output_types(self, instance, **types):
         """
-        Method that specifies the output types when the 'run' method is not decorated
-        with 'component.output_types'.
+        Method that specifies the output types when the 'run' method is not decorated with 'component.output_types'.
 
         Use as:
 
         ```python
         @component
         class MyComponent:
 
             def __init__(self, value: int):
-                component.set_output_types(output_1=int, output_2=str)
+                component.set_output_types(self, output_1=int, output_2=str)
                 ...
 
             # no decorators here
             def run(self, value: int):
                 return {"output_1": 1, "output_2": "2"}
         ```
         """
@@ -310,14 +362,16 @@
             def run(self, value: int):
                 return {"output_1": 1, "output_2": "2"}
         ```
         """
 
         def output_types_decorator(run_method):
             """
+            Decorator that sets the output types of the decorated method.
+
             This happens at class creation time, and since we don't have the decorated
             class available here, we temporarily store the output types as an attribute of
             the decorated method. The ComponentMeta metaclass will use this data to create
             sockets at instance creation time.
             """
             setattr(
                 run_method,
@@ -336,17 +390,17 @@
 
         # Check for required methods and fail as soon as possible
         if not hasattr(cls, "run"):
             raise ComponentError(f"{cls.__name__} must have a 'run()' method. See the docs for more information.")
 
         def copy_class_namespace(namespace):
             """
-            This is the callback that `typing.new_class` will use
-            to populate the newly created class. We just copy
-            the whole namespace from the decorated class.
+            This is the callback that `typing.new_class` will use to populate the newly created class.
+
+            Simply copy the whole namespace from the decorated class.
             """
             for key, val in dict(cls.__dict__).items():
                 # __dict__ and __weakref__ are class-bound, we should let Python recreate them.
                 if key in ("__dict__", "__weakref__"):
                     continue
                 namespace[key] = val
 
@@ -357,18 +411,18 @@
         cls: cls.__name__ = new_class(cls.__name__, cls.__bases__, {"metaclass": ComponentMeta}, copy_class_namespace)  # type: ignore[no-redef]
 
         # Save the component in the class registry (for deserialization)
         class_path = f"{cls.__module__}.{cls.__name__}"
         if class_path in self.registry:
             # Corner case, but it may occur easily in notebooks when re-running cells.
             logger.debug(
-                "Component {component} is already registered. Previous imported from '{module}', new imported from '{new_module}'",
+                "Component {component} is already registered. Previous imported from '{module_name}', new imported from '{new_module_name}'",
                 component=class_path,
-                module=self.registry[class_path],
-                new_module=cls,
+                module_name=self.registry[class_path],
+                new_module_name=cls,
             )
         self.registry[class_path] = cls
         logger.debug("Registered Component {component}", component=cls)
 
         # Override the __repr__ method with a default one
         cls.__repr__ = _component_repr
```

### Comparing `haystack_ai-2.0.1rc2/haystack/core/component/sockets.py` & `haystack_ai-2.1.0rc1/haystack/core/component/sockets.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         self._component = component
         self._sockets_dict = sockets_dict
         self.__dict__.update(sockets_dict)
 
     def __setitem__(self, key: str, socket: Union[InputSocket, OutputSocket]):
         """
         Adds a new socket to this Sockets object.
+
         This eases a bit updating the list of sockets after Sockets has been created.
         That should happen only in the `component` decorator.
         """
         self._sockets_dict[key] = socket
         self.__dict__[key] = socket
 
     def _component_name(self) -> str:
```

### Comparing `haystack_ai-2.0.1rc2/haystack/core/component/types.py` & `haystack_ai-2.1.0rc1/haystack/core/component/types.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     type: Type
     default_value: Any = _empty
     is_variadic: bool = field(init=False)
     senders: List[str] = field(default_factory=list)
 
     @property
     def is_mandatory(self):
+        """Check if the input is mandatory."""
         return self.default_value == _empty
 
     def __post_init__(self):
         try:
             # __metadata__ is a tuple
             self.is_variadic = self.type.__metadata__[0] == HAYSTACK_VARIADIC_ANNOTATION
         except AttributeError:
```

### Comparing `haystack_ai-2.0.1rc2/haystack/core/pipeline/descriptions.py` & `haystack_ai-2.1.0rc1/haystack/core/pipeline/descriptions.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,31 +8,43 @@
 from haystack import logging
 from haystack.core.component.types import InputSocket, OutputSocket
 from haystack.core.type_utils import _type_name
 
 logger = logging.getLogger(__name__)
 
 
-def find_pipeline_inputs(graph: networkx.MultiDiGraph) -> Dict[str, List[InputSocket]]:
+def find_pipeline_inputs(
+    graph: networkx.MultiDiGraph, include_connected_sockets: bool = False
+) -> Dict[str, List[InputSocket]]:
     """
-    Collect components that have disconnected input sockets. Note that this method returns *ALL* disconnected
-    input sockets, including all such sockets with default values.
+    Collect components that have disconnected/connected input sockets. Note that this method returns *ALL*
+    disconnected input sockets, including all such sockets with default values.
     """
     return {
-        name: [socket for socket in data.get("input_sockets", {}).values() if not socket.senders or socket.is_variadic]
+        name: [
+            socket
+            for socket in data.get("input_sockets", {}).values()
+            if socket.is_variadic or (include_connected_sockets or not socket.senders)
+        ]
         for name, data in graph.nodes(data=True)
     }
 
 
-def find_pipeline_outputs(graph: networkx.MultiDiGraph) -> Dict[str, List[OutputSocket]]:
+def find_pipeline_outputs(
+    graph: networkx.MultiDiGraph, include_connected_sockets: bool = False
+) -> Dict[str, List[OutputSocket]]:
     """
-    Collect components that have disconnected output sockets. They define the pipeline output.
+    Collect components that have disconnected/connected output sockets. They define the pipeline output.
     """
     return {
-        name: [socket for socket in data.get("output_sockets", {}).values() if not socket.receivers]
+        name: [
+            socket
+            for socket in data.get("output_sockets", {}).values()
+            if (include_connected_sockets or not socket.receivers)
+        ]
         for name, data in graph.nodes(data=True)
     }
 
 
 def describe_pipeline_inputs(graph: networkx.MultiDiGraph):
     """
     Returns a dictionary with the input names and types that this pipeline accepts.
```

### Comparing `haystack_ai-2.0.1rc2/haystack/core/pipeline/draw.py` & `haystack_ai-2.1.0rc1/haystack/core/pipeline/draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 logger = logging.getLogger(__name__)
 
 
 def _prepare_for_drawing(graph: networkx.MultiDiGraph) -> networkx.MultiDiGraph:
     """
     Add some extra nodes to show the inputs and outputs of the pipeline.
+
     Also adds labels to edges.
     """
     # Label the edges
     for inp, outp, key, data in graph.edges(keys=True, data=True):
         data[
             "label"
         ] = f"{data['from_socket'].name} -> {data['to_socket'].name}{' (opt.)' if not data['mandatory'] else ''}"
@@ -95,16 +96,18 @@
         ) from exc
 
     return resp.content
 
 
 def _to_mermaid_text(graph: networkx.MultiDiGraph) -> str:
     """
-    Converts a Networkx graph into Mermaid syntax. The output of this function can be used in the documentation
-    with `mermaid` codeblocks and it will be automatically rendered.
+    Converts a Networkx graph into Mermaid syntax.
+
+    The output of this function can be used in the documentation with `mermaid` codeblocks and will be
+    automatically rendered.
     """
     # Copy the graph to avoid modifying the original
     graph = _prepare_for_drawing(graph.copy())
     sockets = {
         comp: "".join(
             [
                 f"<li>{name} ({_type_name(socket.type)})</li>"
```

### Comparing `haystack_ai-2.0.1rc2/haystack/core/pipeline/pipeline.py` & `haystack_ai-2.1.0rc1/haystack/core/pipeline/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     PipelineDrawingError,
     PipelineError,
     PipelineMaxLoops,
     PipelineRuntimeError,
     PipelineUnmarshalError,
     PipelineValidationError,
 )
-from haystack.core.serialization import component_from_dict, component_to_dict
+from haystack.core.serialization import DeserializationCallbacks, component_from_dict, component_to_dict
 from haystack.core.type_utils import _type_name, _types_are_compatible
 from haystack.marshal import Marshaller, YamlMarshaller
 from haystack.telemetry import pipeline_running
 from haystack.utils import is_in_jupyter
 
 from .descriptions import find_pipeline_inputs, find_pipeline_outputs
 from .draw import _to_mermaid_image
@@ -72,14 +72,16 @@
         self.max_loops_allowed = max_loops_allowed
         self.graph = networkx.MultiDiGraph()
         self._debug: Dict[int, Dict[str, Any]] = {}
         self._debug_path = Path(debug_path)
 
     def __eq__(self, other) -> bool:
         """
+        Pipeline equality is defined by the equality of their serialized form.
+
         Equal pipelines share every metadata, node and edge, but they're not required to use
         the same node instances: this allows pipeline saved and then loaded back to be equal to themselves.
         """
         if not isinstance(other, Pipeline):
             return False
         return self.to_dict() == other.to_dict()
 
@@ -104,14 +106,15 @@
             res += f"  - {sender}.{sender_socket} -> {receiver}.{receiver_socket} ({edge_data['conn_type']})\n"
 
         return res
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the pipeline to a dictionary.
+
         This is meant to be an intermediate representation but it can be also used to save a pipeline to file.
 
         :returns:
             Dictionary with serialized data.
         """
         components = {}
         for name, instance in self.graph.nodes(data="instance"):  # type:ignore
@@ -126,20 +129,24 @@
             "metadata": self.metadata,
             "max_loops_allowed": self.max_loops_allowed,
             "components": components,
             "connections": connections,
         }
 
     @classmethod
-    def from_dict(cls: Type[T], data: Dict[str, Any], **kwargs) -> T:
+    def from_dict(
+        cls: Type[T], data: Dict[str, Any], callbacks: Optional[DeserializationCallbacks] = None, **kwargs
+    ) -> T:
         """
         Deserializes the pipeline from a dictionary.
 
         :param data:
             Dictionary to deserialize from.
+        :param callbacks:
+            Callbacks to invoke during deserialization.
         :param kwargs:
             `components`: a dictionary of {name: instance} to reuse instances of components instead of creating new ones.
         :returns:
             Deserialized component.
         """
         metadata = data.get("metadata", {})
         max_loops_allowed = data.get("max_loops_allowed", 100)
@@ -154,93 +161,105 @@
                 if "type" not in component_data:
                     raise PipelineError(f"Missing 'type' in component '{name}'")
 
                 if component_data["type"] not in component.registry:
                     try:
                         # Import the module first...
                         module, _ = component_data["type"].rsplit(".", 1)
-                        logger.debug("Trying to import {module}", module=module)
+                        logger.debug("Trying to import module {module_name}", module_name=module)
                         importlib.import_module(module)
                         # ...then try again
                         if component_data["type"] not in component.registry:
                             raise PipelineError(
                                 f"Successfully imported module {module} but can't find it in the component registry."
                                 "This is unexpected and most likely a bug."
                             )
                     except (ImportError, PipelineError) as e:
                         raise PipelineError(f"Component '{component_data['type']}' not imported.") from e
 
                 # Create a new one
                 component_class = component.registry[component_data["type"]]
-                instance = component_from_dict(component_class, component_data)
+                instance = component_from_dict(component_class, component_data, name, callbacks)
             pipe.add_component(name=name, instance=instance)
 
         for connection in data.get("connections", []):
             if "sender" not in connection:
                 raise PipelineError(f"Missing sender in connection: {connection}")
             if "receiver" not in connection:
                 raise PipelineError(f"Missing receiver in connection: {connection}")
             pipe.connect(sender=connection["sender"], receiver=connection["receiver"])
 
         return pipe
 
     def dumps(self, marshaller: Marshaller = DEFAULT_MARSHALLER) -> str:
         """
-        Returns the string representation of this pipeline according to the
-        format dictated by the `Marshaller` in use.
+        Returns the string representation of this pipeline according to the format dictated by the `Marshaller` in use.
 
         :param marshaller:
             The Marshaller used to create the string representation. Defaults to `YamlMarshaller`.
         :returns:
             A string representing the pipeline.
         """
         return marshaller.marshal(self.to_dict())
 
     def dump(self, fp: TextIO, marshaller: Marshaller = DEFAULT_MARSHALLER):
         """
-        Writes the string representation of this pipeline to the file-like object
-        passed in the `fp` argument.
+        Writes the string representation of this pipeline to the file-like object passed in the `fp` argument.
 
         :param fp:
             A file-like object ready to be written to.
         :param marshaller:
             The Marshaller used to create the string representation. Defaults to `YamlMarshaller`.
         """
         fp.write(marshaller.marshal(self.to_dict()))
 
     @classmethod
-    def loads(cls, data: Union[str, bytes, bytearray], marshaller: Marshaller = DEFAULT_MARSHALLER) -> "Pipeline":
+    def loads(
+        cls,
+        data: Union[str, bytes, bytearray],
+        marshaller: Marshaller = DEFAULT_MARSHALLER,
+        callbacks: Optional[DeserializationCallbacks] = None,
+    ) -> "Pipeline":
         """
         Creates a `Pipeline` object from the string representation passed in the `data` argument.
 
         :param data:
             The string representation of the pipeline, can be `str`, `bytes` or `bytearray`.
         :param marshaller:
             The Marshaller used to create the string representation. Defaults to `YamlMarshaller`.
+        :param callbacks:
+            Callbacks to invoke during deserialization.
         :returns:
             A `Pipeline` object.
         """
-        return cls.from_dict(marshaller.unmarshal(data))
+        return cls.from_dict(marshaller.unmarshal(data), callbacks)
 
     @classmethod
-    def load(cls, fp: TextIO, marshaller: Marshaller = DEFAULT_MARSHALLER) -> "Pipeline":
+    def load(
+        cls,
+        fp: TextIO,
+        marshaller: Marshaller = DEFAULT_MARSHALLER,
+        callbacks: Optional[DeserializationCallbacks] = None,
+    ) -> "Pipeline":
         """
-        Creates a `Pipeline` object from the string representation read from the file-like
-        object passed in the `fp` argument.
+        Creates a `Pipeline` object a string representation.
+
+        The string representation is read from the file-like object passed in the `fp` argument.
+
 
-        :param data:
-            The string representation of the pipeline, can be `str`, `bytes` or `bytearray`.
         :param fp:
             A file-like object ready to be read from.
         :param marshaller:
             The Marshaller used to create the string representation. Defaults to `YamlMarshaller`.
+        :param callbacks:
+            Callbacks to invoke during deserialization.
         :returns:
             A `Pipeline` object.
         """
-        return cls.from_dict(marshaller.unmarshal(fp.read()))
+        return cls.from_dict(marshaller.unmarshal(fp.read()), callbacks)
 
     def add_component(self, name: str, instance: Component) -> None:
         """
         Add the given component to the pipeline.
 
         Components are not connected to anything by default: use `Pipeline.connect()` to connect components together.
         Component names must be unique, but component instances can be reused if needed.
@@ -290,15 +309,15 @@
         )
 
     def connect(self, sender: str, receiver: str) -> "Pipeline":
         """
         Connects two components together.
 
         All components to connect must exist in the pipeline.
-        If connecting to an component that has several output connections, specify the inputs and output names as
+        If connecting to a component that has several output connections, specify the inputs and output names as
         'component_name.connections_name'.
 
         :param sender:
             The component that delivers the value. This can be either just a component name or can be
             in the format `component_name.connection_name` if the component has multiple outputs.
         :param receiver:
             The component that receives the value. This can be either just a component name or can be
@@ -482,49 +501,57 @@
             The name of the Component instance.
         """
         for name, inst in self.graph.nodes(data="instance"):
             if inst == instance:
                 return name
         return ""
 
-    def inputs(self) -> Dict[str, Dict[str, Any]]:
+    def inputs(self, include_components_with_connected_inputs: bool = False) -> Dict[str, Dict[str, Any]]:
         """
-        Returns a dictionary containing the inputs of a pipeline. Each key in the dictionary
-        corresponds to a component name, and its value is another dictionary that describes the
-        input sockets of that component, including their types and whether they are optional.
+        Returns a dictionary containing the inputs of a pipeline.
 
+        Each key in the dictionary corresponds to a component name, and its value is another dictionary that describes
+        the input sockets of that component, including their types and whether they are optional.
+
+        :param include_components_with_connected_inputs:
+            If `False`, only components that have disconnected input edges are
+            included in the output.
         :returns:
             A dictionary where each key is a pipeline component name and each value is a dictionary of
             inputs sockets of that component.
         """
         inputs: Dict[str, Dict[str, Any]] = {}
-        for component_name, data in find_pipeline_inputs(self.graph).items():
+        for component_name, data in find_pipeline_inputs(self.graph, include_components_with_connected_inputs).items():
             sockets_description = {}
             for socket in data:
                 sockets_description[socket.name] = {"type": socket.type, "is_mandatory": socket.is_mandatory}
                 if not socket.is_mandatory:
                     sockets_description[socket.name]["default_value"] = socket.default_value
 
             if sockets_description:
                 inputs[component_name] = sockets_description
         return inputs
 
-    def outputs(self) -> Dict[str, Dict[str, Any]]:
+    def outputs(self, include_components_with_connected_outputs: bool = False) -> Dict[str, Dict[str, Any]]:
         """
-        Returns a dictionary containing the outputs of a pipeline. Each key in the dictionary
-        corresponds to a component name, and its value is another dictionary that describes the
-        output sockets of that component.
+        Returns a dictionary containing the outputs of a pipeline.
+
+        Each key in the dictionary corresponds to a component name, and its value is another dictionary that describes
+        the output sockets of that component.
 
+        :param include_components_with_connected_outputs:
+            If `False`, only components that have disconnected output edges are
+            included in the output.
         :returns:
             A dictionary where each key is a pipeline component name and each value is a dictionary of
             output sockets of that component.
         """
         outputs = {
             comp: {socket.name: {"type": socket.type} for socket in data}
-            for comp, data in find_pipeline_outputs(self.graph).items()
+            for comp, data in find_pipeline_outputs(self.graph, include_components_with_connected_outputs).items()
             if data
         }
         return outputs
 
     def show(self) -> None:
         """
         If running in a Jupyter notebook, display an image representing this `Pipeline`.
@@ -551,14 +578,15 @@
         # used for running the pipeline we copy it.
         image_data = _to_mermaid_image(self.graph)
         Path(path).write_bytes(image_data)
 
     def walk(self) -> Iterator[Tuple[str, Component]]:
         """
         Visits each component in the pipeline exactly once and yields its name and instance.
+
         No guarantees are provided on the visiting order.
 
         :returns:
             An iterator of tuples of component name and component instance.
         """
         for component_name, instance in self.graph.nodes(data="instance"):
             yield component_name, instance
@@ -573,14 +601,16 @@
         for node in self.graph.nodes:
             if hasattr(self.graph.nodes[node]["instance"], "warm_up"):
                 logger.info("Warming up component {node}...", node=node)
                 self.graph.nodes[node]["instance"].warm_up()
 
     def _validate_input(self, data: Dict[str, Any]):
         """
+        Validates pipeline input data.
+
         Validates that data:
         * Each Component name actually exists in the Pipeline
         * Each Component is not missing any input
         * Each Component has only one input per input socket, if not variadic
         * Each Component doesn't receive inputs that are already sent by another Component
 
         :param data:
@@ -609,26 +639,34 @@
                 if socket.senders and socket_name in component_inputs and not socket.is_variadic:
                     raise ValueError(
                         f"Input {socket_name} for component {component_name} is already sent by {socket.senders}."
                     )
 
     # TODO: We're ignoring these linting rules for the time being, after we properly optimize this function we'll remove the noqa
     def run(  # noqa: C901, PLR0912, PLR0915 pylint: disable=too-many-branches
-        self, data: Dict[str, Any], debug: bool = False
+        self, data: Dict[str, Any], debug: bool = False, include_outputs_from: Optional[Set[str]] = None
     ) -> Dict[str, Any]:
         """
         Runs the pipeline with given input data.
 
         :param data:
             A dictionary of inputs for the pipeline's components. Each key is a component name
             and its value is a dictionary of that component's input parameters.
         :param debug:
             Set to True to collect and return debug information.
+        :param include_outputs_from:
+            Set of component names whose individual outputs are to be
+            included in the pipeline's output. For components that are
+            invoked multiple times (in a loop), only the last-produced
+            output is included.
         :returns:
-            A dictionary containing the pipeline's output.
+            A dictionary where each entry corresponds to a component name
+            and its output. If `include_outputs_from` is `None`, this dictionary
+            will only contain the outputs of leaf components, i.e., components
+            without outgoing connections.
 
         :raises PipelineRuntimeError:
             If a component fails or returns unexpected output.
 
         Example a - Using named components:
         Consider a 'Hello' component that takes a 'word' input and outputs a greeting.
 
@@ -752,24 +790,32 @@
         # we know we're stuck in a loop and we can't make any progress.
         before_last_waiting_for_input: Optional[Set[str]] = None
         last_waiting_for_input: Optional[Set[str]] = None
 
         # The waiting_for_input list is used to keep track of components that are waiting for input.
         waiting_for_input: List[Tuple[str, Component]] = []
 
+        include_outputs_from = set() if include_outputs_from is None else include_outputs_from
+
+        # This is what we'll return at the end
+        final_outputs: Dict[Any, Any] = {}
+
         with tracing.tracer.trace(
             "haystack.pipeline.run",
             tags={
+                "haystack.pipeline.input_data": data,
+                "haystack.pipeline.output_data": final_outputs,
                 "haystack.pipeline.debug": debug,
                 "haystack.pipeline.metadata": self.metadata,
                 "haystack.pipeline.max_loops_allowed": self.max_loops_allowed,
             },
         ):
-            # This is what we'll return at the end
-            final_outputs = {}
+            # Cache for extra outputs, if enabled.
+            extra_outputs: Dict[Any, Any] = {}
+
             while len(to_run) > 0:
                 name, comp = to_run.pop(0)
 
                 if any(socket.is_variadic for socket in comp.__haystack_input__._sockets_dict.values()) and not getattr(  # type: ignore
                     comp, "is_greedy", False
                 ):
                     there_are_non_variadics = False
@@ -809,27 +855,33 @@
                                     "senders": value.receivers,
                                 }
                                 for key, value in comp.__haystack_output__._sockets_dict.items()  # type: ignore
                             },
                         },
                     ) as span:
                         span.set_content_tag("haystack.component.input", last_inputs[name])
-
+                        logger.info("Running component {name}", name=name)
+                        logger.info("Running component {component_name}", component_name=name)
                         res = comp.run(**last_inputs[name])
                         self.graph.nodes[name]["visits"] += 1
 
                         if not isinstance(res, Mapping):
                             raise PipelineRuntimeError(
                                 f"Component '{name}' didn't return a dictionary. "
                                 "Components must always return dictionaries: check the the documentation."
                             )
 
                         span.set_tags(tags={"haystack.component.visits": self.graph.nodes[name]["visits"]})
                         span.set_content_tag("haystack.component.output", res)
 
+                        if name in include_outputs_from:
+                            # Deepcopy the outputs to prevent downstream nodes from modifying them
+                            # We don't care about loops - Always store the last output.
+                            extra_outputs[name] = deepcopy(res)
+
                     # Reset the waiting for input previous states, we managed to run a component
                     before_last_waiting_for_input = None
                     last_waiting_for_input = None
 
                     if (name, comp) in waiting_for_input:
                         # We manage to run this component that was in the waiting list, we can remove it.
                         # This happens when a component was put in the waiting list but we reached it from another edge.
@@ -918,14 +970,23 @@
                             # This will never run.
                             # BAIL!
                             break
 
                         # There was a lazy variadic or a component with only default waiting for input, we can run it
                         waiting_for_input.remove((name, comp))
                         to_run.append((name, comp))
+
+                        # Let's use the default value for the inputs that are still missing, or the component
+                        # won't run and will be put back in the waiting list, causing an infinite loop.
+                        for input_socket in comp.__haystack_input__._sockets_dict.values():  # type: ignore
+                            if input_socket.is_mandatory:
+                                continue
+                            if input_socket.name not in last_inputs[name]:
+                                last_inputs[name][input_socket.name] = input_socket.default_value
+
                         continue
 
                     before_last_waiting_for_input = (
                         last_waiting_for_input.copy() if last_waiting_for_input is not None else None
                     )
                     last_waiting_for_input = {item[0] for item in waiting_for_input}
 
@@ -984,18 +1045,25 @@
                                 last_inputs[name][input_socket.name] = input_socket.default_value
                         if has_enough_inputs:
                             break
 
                     waiting_for_input.remove((name, comp))
                     to_run.append((name, comp))
 
+            if len(include_outputs_from) > 0:
+                for name, output in extra_outputs.items():
+                    if name not in final_outputs:
+                        final_outputs[name] = output
+
             return final_outputs
 
     def _prepare_component_input_data(self, data: Dict[str, Any]) -> Tuple[Dict[str, Dict[str, Any]], Dict[str, Any]]:
         """
+        Prepares input data for pipeline components.
+
         Organizes input data for pipeline components and identifies any inputs that are not matched to any
         component's input slots.
 
         This method processes a flat dictionary of input data, where each key-value pair represents an input name
         and its corresponding value. It distributes these inputs to the appropriate pipeline components based on
         their input requirements. Inputs that don't match any component's input slots are classified as unresolved.
```

### Comparing `haystack_ai-2.0.1rc2/haystack/core/pipeline/template.py` & `haystack_ai-2.1.0rc1/haystack/core/pipeline/template.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     RAG = "rag"
     INDEXING = "indexing"
     CHAT_WITH_WEBSITE = "chat_with_website"
 
 
 class PipelineTemplate:
     """
+    The PipelineTemplate enables the creation of flexible and configurable pipelines.
+
     The PipelineTemplate class enables the straightforward creation of flexible and configurable pipelines using
     Jinja2 templated YAML files. Specifically designed to simplify the setup of complex data processing pipelines for
     a range of NLP tasks—including question answering, retriever augmented generation (RAG), document indexing, among
     others - PipelineTemplate empowers users to dynamically generate pipeline configurations from templates and
     customize components as necessary. Its design philosophy centers on providing an accessible, yet powerful, tool
     for constructing pipelines that accommodate both common use cases and specialized requirements with ease.
 
@@ -56,17 +58,19 @@
 
     The `PipelineTemplate` is designed to offer both ease of use for common pipeline configurations and the
     flexibility to customize and extend pipelines as required by advanced users and specific use cases.
     """
 
     def __init__(self, template_content: str):
         """
-        Initialize a PipelineTemplate. Besides calling the constructor directly, a set of utility methods is provided
-        for conveniently create an instance of `PipelineTemplate` from different sources. See `from_string`,
-        `from_file`, `from_predefined` and `from_url`.
+        Initialize a PipelineTemplate.
+
+        Besides calling the constructor directly, a set of utility methods is provided to conveniently create an
+        instance of `PipelineTemplate` from different sources. See `from_string`, `from_file`, `from_predefined`
+        and `from_url`.
 
         :param template_content: The raw template source to use in the template.
         """
         env = Environment(
             loader=PackageLoader("haystack.core.pipeline", "predefined"), trim_blocks=True, lstrip_blocks=True
         )
         try:
@@ -89,24 +93,28 @@
         template_params = template_params or {}
         return self._template.render(**template_params)
 
     @classmethod
     def from_file(cls, file_path: Union[Path, str]) -> "PipelineTemplate":
         """
         Create a PipelineTemplate from a file.
+
         :param file_path: The path to the file containing the template. Must contain valid Jinja2 syntax.
         :returns: An instance of `PipelineTemplate`.
         """
         with open(file_path, "r") as file:
             return cls(file.read())
 
     @classmethod
     def from_predefined(cls, predefined_pipeline: PredefinedPipeline) -> "PipelineTemplate":
         """
-        Create a PipelineTemplate from a predefined template. See `PredefinedPipeline` for available options.
+        Create a PipelineTemplate from a predefined template.
+
+        See `PredefinedPipeline` for available options.
+
         :param predefined_pipeline: The predefined pipeline to use.
         :returns: An instance of `PipelineTemplate `.
         """
         template_path = f"{TEMPLATE_HOME_DIR}/{predefined_pipeline.value}{TEMPLATE_FILE_EXTENSION}"
         return cls.from_file(template_path)
 
     @property
```

### Comparing `haystack_ai-2.0.1rc2/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2` & `haystack_ai-2.1.0rc1/haystack/core/pipeline/predefined/chat_with_website.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2` & `haystack_ai-2.1.0rc1/haystack/core/pipeline/predefined/generative_qa.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/core/pipeline/predefined/indexing.yaml.jinja2` & `haystack_ai-2.1.0rc1/haystack/core/pipeline/predefined/indexing.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/core/pipeline/predefined/rag.yaml.jinja2` & `haystack_ai-2.1.0rc1/haystack/core/pipeline/predefined/rag.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/dataclasses/__init__.py` & `haystack_ai-2.1.0rc1/haystack/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/dataclasses/byte_stream.py` & `haystack_ai-2.1.0rc1/haystack/dataclasses/byte_stream.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/dataclasses/document.py` & `haystack_ai-2.1.0rc1/haystack/dataclasses/document.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     """
     Metaclass that handles Document backward compatibility.
     """
 
     def __call__(cls, *args, **kwargs):
         """
         Called before Document.__init__, will remap legacy fields to new ones.
+
         Also handles building a Document from a flattened dictionary.
         """
         # Move `content` to new fields depending on the type
         content = kwargs.get("content")
         if isinstance(content, DataFrame):
             kwargs["dataframe"] = content
             del kwargs["content"]
```

### Comparing `haystack_ai-2.0.1rc2/haystack/dataclasses/sparse_embedding.py` & `haystack_ai-2.1.0rc1/haystack/dataclasses/sparse_embedding.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,23 +4,42 @@
 class SparseEmbedding:
     """
     Class representing a sparse embedding.
     """
 
     def __init__(self, indices: List[int], values: List[float]):
         """
+        Initialize a SparseEmbedding object.
+
         :param indices: List of indices of non-zero elements in the embedding.
         :param values: List of values of non-zero elements in the embedding.
 
         :raises ValueError: If the indices and values lists are not of the same length.
         """
         if len(indices) != len(values):
             raise ValueError("Length of indices and values must be the same.")
         self.indices = indices
         self.values = values
 
+    def __eq__(self, other):
+        return self.indices == other.indices and self.values == other.values
+
     def to_dict(self):
+        """
+        Convert the SparseEmbedding object to a dictionary.
+
+        :returns:
+            Serialized sparse embedding.
+        """
         return {"indices": self.indices, "values": self.values}
 
     @classmethod
     def from_dict(cls, sparse_embedding_dict):
+        """
+        Deserializes the sparse embedding from a dictionary.
+
+        :param sparse_embedding_dict:
+            Dictionary to deserialize from.
+        :returns:
+            Deserialized sparse embedding.
+        """
         return cls(indices=sparse_embedding_dict["indices"], values=sparse_embedding_dict["values"])
```

### Comparing `haystack_ai-2.0.1rc2/haystack/dataclasses/streaming_chunk.py` & `haystack_ai-2.1.0rc1/haystack/dataclasses/streaming_chunk.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/document_stores/in_memory/document_store.py` & `haystack_ai-2.1.0rc1/haystack/document_stores/in_memory/document_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,14 +134,15 @@
                     continue
             self.storage[document.id] = document
         return written_documents
 
     def delete_documents(self, document_ids: List[str]) -> None:
         """
         Deletes all documents with matching document_ids from the DocumentStore.
+
         :param document_ids: The object_ids to delete.
         """
         for doc_id in document_ids:
             if doc_id not in self.storage.keys():
                 continue
             del self.storage[doc_id]
```

### Comparing `haystack_ai-2.0.1rc2/haystack/document_stores/types/protocol.py` & `haystack_ai-2.1.0rc1/haystack/document_stores/types/protocol.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/telemetry/_environment.py` & `haystack_ai-2.1.0rc1/haystack/telemetry/_environment.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,40 +12,45 @@
 
 # This value cannot change during the lifetime of the process
 _IS_DOCKER_CACHE = None
 
 
 def _in_podman() -> bool:
     """
+    Check if the code is running in a Podman container.
+
     Podman run would create the file /run/.containernv, see:
     https://github.com/containers/podman/blob/main/docs/source/markdown/podman-run.1.md.in#L31
     """
     return os.path.exists("/run/.containerenv")
 
 
 def _has_dockerenv() -> bool:
     """
+    Check if the code is running in a Docker container.
+
     This might not work anymore at some point (even if it's been a while now), see:
     https://github.com/moby/moby/issues/18355#issuecomment-220484748
     """
     return os.path.exists("/.dockerenv")
 
 
 def _has_docker_cgroup_v1() -> bool:
     """
-    This only works with cgroups v1
+    This only works with cgroups v1.
     """
     path = "/proc/self/cgroup"  # 'self' should be always symlinked to the actual PID
     return os.path.isfile(path) and any("docker" in line for line in open(path))
 
 
 def _has_docker_cgroup_v2() -> bool:
     """
-    cgroups v2 version, inspired from
-    https://github.com/jenkinsci/docker-workflow-plugin/blob/master/src/main/java/org/jenkinsci/plugins/docker/workflow/client/DockerClient.java
+    Check if the code is running in a Docker container using the cgroups v2 version.
+
+    inspired from: https://github.com/jenkinsci/docker-workflow-plugin/blob/master/src/main/java/org/jenkinsci/plugins/docker/workflow/client/DockerClient.java
     """
     path = "/proc/self/mountinfo"  # 'self' should be always symlinked to the actual PID
     return os.path.isfile(path) and any("/docker/containers/" in line for line in open(path))
 
 
 def _is_containerized() -> Optional[bool]:
     """
@@ -57,16 +62,17 @@
         _IS_DOCKER_CACHE = _in_podman() or _has_dockerenv() or _has_docker_cgroup_v1() or _has_docker_cgroup_v2()
 
     return _IS_DOCKER_CACHE
 
 
 def collect_system_specs() -> Dict[str, Any]:
     """
-    Collects meta data about the setup that is used with Haystack, such as:
-    operating system, python version, Haystack version, transformers version,
+    Collects meta-data about the setup that is used with Haystack.
+
+    Data collected includes: operating system, python version, Haystack version, transformers version,
     pytorch version, number of GPUs, execution environment.
 
     These values are highly unlikely to change during the runtime of the pipeline,
     so they're collected only once.
     """
     specs = {
         "libraries.haystack": __version__,
```

### Comparing `haystack_ai-2.0.1rc2/haystack/telemetry/_telemetry.py` & `haystack_ai-2.1.0rc1/haystack/telemetry/_telemetry.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,17 @@
     [documentation page](https://docs.haystack.deepset.ai/docs/telemetry#how-can-i-opt-out).
 
     Check out the documentation for more details: [Telemetry](https://docs.haystack.deepset.ai/docs/telemetry).
     """
 
     def __init__(self):
         """
-        Initializes the telemetry. Loads the user_id from the config file,
-        or creates a new id and saves it if the file is not found.
+        Initializes the telemetry.
+
+        Loads the user_id from the config file, or creates a new id and saves it if the file is not found.
 
         It also collects system information which cannot change across the lifecycle
         of the process (for example `is_containerized()`).
         """
         posthog.api_key = "phc_C44vUK9R1J6HYVdfJarTEPqVAoRPJzMXzFcj8PIrJgP"
         posthog.host = "https://eu.posthog.com"
 
@@ -106,14 +107,15 @@
         except Exception as e:
             logger.debug("Telemetry couldn't make a POST request to PostHog.", exc_info=e)
 
 
 def send_telemetry(func):
     """
     Decorator that sends the output of the wrapped function to PostHog.
+
     The wrapped function is actually called only if telemetry is enabled.
     """
 
     # FIXME? Somehow, functools.wraps makes `telemetry` out of scope. Let's take care of it later.
     def send_telemetry_wrapper(*args, **kwargs):
         try:
             if telemetry:
@@ -126,14 +128,16 @@
 
     return send_telemetry_wrapper
 
 
 @send_telemetry
 def pipeline_running(pipeline: "Pipeline") -> Optional[Tuple[str, Dict[str, Any]]]:
     """
+    Collects telemetry data for a pipeline run and sends it to Posthog.
+
     Collects name, type and the content of the _telemetry_data attribute, if present, for each component in the
     pipeline and sends such data to Posthog.
 
     :param pipeline: the pipeline that is running.
     """
     pipeline._telemetry_runs += 1
     if (
@@ -166,14 +170,15 @@
     }
 
 
 @send_telemetry
 def tutorial_running(tutorial_id: str) -> Tuple[str, Dict[str, Any]]:
     """
     Send a telemetry event for a tutorial, if telemetry is enabled.
+
     :param tutorial_id: identifier of the tutorial
     """
     return "Tutorial", {"tutorial.id": tutorial_id}
 
 
 telemetry = None
 if os.getenv("HAYSTACK_TELEMETRY_ENABLED", "true").lower() in ("true", "1"):
```

### Comparing `haystack_ai-2.0.1rc2/haystack/testing/document_store.py` & `haystack_ai-2.1.0rc1/haystack/testing/document_store.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 TEST_EMBEDDING_2 = _random_embeddings(768)
 
 
 class AssertDocumentsEqualMixin:
     def assert_documents_are_equal(self, received: List[Document], expected: List[Document]):
         """
         Assert that two lists of Documents are equal.
-        This is used in every test, if a Document Store implementation has a different behaviour
-        it should override this method.
 
-        This can happen for example when the Document Store sets a score to returned Documents.
-        Since we can't know what the score will be, we can't compare the Documents reliably.
+        This is used in every test, if a Document Store implementation has a different behaviour
+        it should override this method. This can happen for example when the Document Store sets
+        a score to returned Documents. Since we can't know what the score will be, we can't compare
+        the Documents reliably.
         """
         assert received == expected
 
 
 class CountDocumentsTest:
     """
     Utility class to test a Document Store `count_documents` method.
@@ -51,17 +51,19 @@
         @pytest.fixture
         def document_store(self):
             return MyDocumentStore()
     ```
     """
 
     def test_count_empty(self, document_store: DocumentStore):
+        """Test count is zero for an empty document store"""
         assert document_store.count_documents() == 0
 
     def test_count_not_empty(self, document_store: DocumentStore):
+        """Test count is greater than zero if the document store contains documents"""
         document_store.write_documents(
             [Document(content="test doc 1"), Document(content="test doc 2"), Document(content="test doc 3")]
         )
         assert document_store.count_documents() == 3
 
 
 class WriteDocumentsTest(AssertDocumentsEqualMixin):
@@ -89,50 +91,39 @@
             "Default write_documents() behaviour depends on the Document Store implementation, "
             "as we don't enforce a default behaviour when no policy is set. "
             "Override this test in your custom test class."
         )
         raise NotImplementedError(msg)
 
     def test_write_documents_duplicate_fail(self, document_store: DocumentStore):
-        """
-        Test write_documents() fails when trying to write Document with same id
-        using DuplicatePolicy.FAIL.
-        """
+        """Test write_documents() fails when writing documents with same id and `DuplicatePolicy.FAIL`."""
         doc = Document(content="test doc")
         assert document_store.write_documents([doc], policy=DuplicatePolicy.FAIL) == 1
         with pytest.raises(DuplicateDocumentError):
             document_store.write_documents(documents=[doc], policy=DuplicatePolicy.FAIL)
         self.assert_documents_are_equal(document_store.filter_documents(), [doc])
 
     def test_write_documents_duplicate_skip(self, document_store: DocumentStore):
-        """
-        Test write_documents() skips Document when trying to write one with same id
-        using DuplicatePolicy.SKIP.
-        """
+        """Test write_documents() skips writing when using DuplicatePolicy.SKIP."""
         doc = Document(content="test doc")
         assert document_store.write_documents([doc], policy=DuplicatePolicy.SKIP) == 1
         assert document_store.write_documents(documents=[doc], policy=DuplicatePolicy.SKIP) == 0
 
     def test_write_documents_duplicate_overwrite(self, document_store: DocumentStore):
-        """
-        Test write_documents() overwrites stored Document when trying to write one with same id
-        using DuplicatePolicy.OVERWRITE.
-        """
+        """Test write_documents() overwrites when using DuplicatePolicy.OVERWRITE."""
         doc1 = Document(id="1", content="test doc 1")
         doc2 = Document(id="1", content="test doc 2")
 
         assert document_store.write_documents([doc2], policy=DuplicatePolicy.OVERWRITE) == 1
         self.assert_documents_are_equal(document_store.filter_documents(), [doc2])
         assert document_store.write_documents(documents=[doc1], policy=DuplicatePolicy.OVERWRITE) == 1
         self.assert_documents_are_equal(document_store.filter_documents(), [doc1])
 
     def test_write_documents_invalid_input(self, document_store: DocumentStore):
-        """
-        Test write_documents() fails when providing unexpected input.
-        """
+        """Test write_documents() fails when providing unexpected input."""
         with pytest.raises(ValueError):
             document_store.write_documents(["not a document for sure"])  # type: ignore
         with pytest.raises(ValueError):
             document_store.write_documents("not a list actually")  # type: ignore
 
 
 class DeleteDocumentsTest:
@@ -148,34 +139,28 @@
         @pytest.fixture
         def document_store(self):
             return MyDocumentStore()
     ```
     """
 
     def test_delete_documents(self, document_store: DocumentStore):
-        """
-        Test delete_documents() normal behaviour.
-        """
+        """Test delete_documents() normal behaviour."""
         doc = Document(content="test doc")
         document_store.write_documents([doc])
         assert document_store.count_documents() == 1
 
         document_store.delete_documents([doc.id])
         assert document_store.count_documents() == 0
 
     def test_delete_documents_empty_document_store(self, document_store: DocumentStore):
-        """
-        Test delete_documents() doesn't fail when called using an empty Document Store.
-        """
+        """Test delete_documents() doesn't fail when called using an empty Document Store."""
         document_store.delete_documents(["non_existing_id"])
 
     def test_delete_documents_non_existing_document(self, document_store: DocumentStore):
-        """
-        Test delete_documents() doesn't delete any Document when called with non existing id.
-        """
+        """Test delete_documents() doesn't delete any Document when called with non existing id."""
         doc = Document(content="test doc")
         document_store.write_documents([doc])
         assert document_store.count_documents() == 1
 
         document_store.delete_documents(["non_existing_id"])
 
         # No Document has been deleted
@@ -185,14 +170,15 @@
 class FilterableDocsFixtureMixin:
     """
     Mixin class that adds a filterable_docs() fixture to a test class.
     """
 
     @pytest.fixture
     def filterable_docs(self) -> List[Document]:
+        """Fixture that returns a list of Documents that can be used to test filtering."""
         documents = []
         for i in range(3):
             documents.append(
                 Document(
                     content=f"A Foo Document {i}",
                     meta={
                         "name": f"name_{i}",
@@ -258,24 +244,27 @@
         @pytest.fixture
         def document_store(self):
             return MyDocumentStore()
     ```
     """
 
     def test_incorrect_filter_type(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         with pytest.raises(ValueError):
             document_store.filter_documents(filters="something odd")  # type: ignore
 
     def test_incorrect_filter_nesting(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"number": {"page": "100"}})
 
     def test_deeper_incorrect_filter_nesting(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"number": {"page": {"chapter": "intro"}}})
 
 
 class LegacyFilterDocumentsEqualTest(AssertDocumentsEqualMixin, FilterableDocsFixtureMixin):
     """
@@ -289,54 +278,61 @@
         @pytest.fixture
         def document_store(self):
             return MyDocumentStore()
     ```
     """
 
     def test_filter_document_content(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"content": "A Foo Document 1"})
         self.assert_documents_are_equal(result, [doc for doc in filterable_docs if doc.content == "A Foo Document 1"])
 
     def test_filter_simple_metadata_value(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"page": "100"})
         self.assert_documents_are_equal(result, [doc for doc in filterable_docs if doc.meta.get("page") == "100"])
 
     def test_filter_document_dataframe(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"dataframe": pd.DataFrame([1])})
         self.assert_documents_are_equal(
             result,
             [doc for doc in filterable_docs if doc.dataframe is not None and doc.dataframe.equals(pd.DataFrame([1]))],
         )
 
     def test_eq_filter_explicit(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"page": {"$eq": "100"}})
         self.assert_documents_are_equal(result, [doc for doc in filterable_docs if doc.meta.get("page") == "100"])
 
     def test_eq_filter_implicit(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"page": "100"})
         self.assert_documents_are_equal(result, [doc for doc in filterable_docs if doc.meta.get("page") == "100"])
 
     def test_eq_filter_table(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"dataframe": pd.DataFrame([1])})
         self.assert_documents_are_equal(
             result,
             [
                 doc
                 for doc in filterable_docs
                 if isinstance(doc.dataframe, pd.DataFrame) and doc.dataframe.equals(pd.DataFrame([1]))
             ],
         )
 
     def test_eq_filter_embedding(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         embedding = [0.0] * 768
         result = document_store.filter_documents(filters={"embedding": embedding})
         self.assert_documents_are_equal(result, [doc for doc in filterable_docs if embedding == doc.embedding])
 
 
 class LegacyFilterDocumentsNotEqualTest(AssertDocumentsEqualMixin, FilterableDocsFixtureMixin):
@@ -351,31 +347,34 @@
         @pytest.fixture
         def document_store(self):
             return MyDocumentStore()
     ```
     """
 
     def test_ne_filter(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"page": {"$ne": "100"}})
         self.assert_documents_are_equal(result, [doc for doc in filterable_docs if doc.meta.get("page") != "100"])
 
     def test_ne_filter_table(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"dataframe": {"$ne": pd.DataFrame([1])}})
         self.assert_documents_are_equal(
             result,
             [
                 doc
                 for doc in filterable_docs
                 if not isinstance(doc.dataframe, pd.DataFrame) or not doc.dataframe.equals(pd.DataFrame([1]))
             ],
         )
 
     def test_ne_filter_embedding(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"embedding": {"$ne": TEST_EMBEDDING_1}})
         self.assert_documents_are_equal(result, [doc for doc in filterable_docs if doc.embedding != TEST_EMBEDDING_1])
 
 
 class LegacyFilterDocumentsInTest(AssertDocumentsEqualMixin, FilterableDocsFixtureMixin):
     """
@@ -389,68 +388,77 @@
         @pytest.fixture
         def document_store(self):
             return MyDocumentStore()
     ```
     """
 
     def test_filter_simple_list_single_element(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"page": ["100"]})
         self.assert_documents_are_equal(result, [doc for doc in filterable_docs if doc.meta.get("page") == "100"])
 
     def test_filter_simple_list_one_value(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"page": ["100"]})
         self.assert_documents_are_equal(result, [doc for doc in filterable_docs if doc.meta.get("page") in ["100"]])
 
     def test_filter_simple_list(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"page": ["100", "123"]})
         self.assert_documents_are_equal(
             result, [doc for doc in filterable_docs if doc.meta.get("page") in ["100", "123"]]
         )
 
     def test_incorrect_filter_name(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"non_existing_meta_field": ["whatever"]})
         self.assert_documents_are_equal(result, [])
 
     def test_incorrect_filter_value(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"page": ["nope"]})
         self.assert_documents_are_equal(result, [])
 
     def test_in_filter_explicit(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"page": {"$in": ["100", "123", "n.a."]}})
         self.assert_documents_are_equal(
             result, [doc for doc in filterable_docs if doc.meta.get("page") in ["100", "123"]]
         )
 
     def test_in_filter_implicit(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"page": ["100", "123", "n.a."]})
         self.assert_documents_are_equal(
             result, [doc for doc in filterable_docs if doc.meta.get("page") in ["100", "123"]]
         )
 
     def test_in_filter_table(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"dataframe": {"$in": [pd.DataFrame([1]), pd.DataFrame([2])]}})
         self.assert_documents_are_equal(
             result,
             [
                 doc
                 for doc in filterable_docs
                 if isinstance(doc.dataframe, pd.DataFrame)
                 and (doc.dataframe.equals(pd.DataFrame([1])) or doc.dataframe.equals(pd.DataFrame([2])))
             ],
         )
 
     def test_in_filter_embedding(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         embedding_zero = [0.0] * 768
         embedding_one = [1.0] * 768
         result = document_store.filter_documents(filters={"embedding": {"$in": [embedding_zero, embedding_one]}})
         self.assert_documents_are_equal(
             result,
             [doc for doc in filterable_docs if (embedding_zero == doc.embedding or embedding_one == doc.embedding)],
@@ -469,14 +477,15 @@
         @pytest.fixture
         def document_store(self):
             return MyDocumentStore()
     ```
     """
 
     def test_nin_filter_table(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(
             filters={"dataframe": {"$nin": [pd.DataFrame([1]), pd.DataFrame([0])]}}
         )
         self.assert_documents_are_equal(
             result,
             [
@@ -484,21 +493,23 @@
                 for doc in filterable_docs
                 if not isinstance(doc.dataframe, pd.DataFrame)
                 or (not doc.dataframe.equals(pd.DataFrame([1])) and not doc.dataframe.equals(pd.DataFrame([0])))
             ],
         )
 
     def test_nin_filter_embedding(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"embedding": {"$nin": [TEST_EMBEDDING_1, TEST_EMBEDDING_2]}})
         self.assert_documents_are_equal(
             result, [doc for doc in filterable_docs if doc.embedding not in [TEST_EMBEDDING_1, TEST_EMBEDDING_2]]
         )
 
     def test_nin_filter(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"page": {"$nin": ["100", "123", "n.a."]}})
         self.assert_documents_are_equal(
             result, [doc for doc in filterable_docs if doc.meta.get("page") not in ["100", "123"]]
         )
 
 
@@ -514,31 +525,35 @@
         @pytest.fixture
         def document_store(self):
             return MyDocumentStore()
     ```
     """
 
     def test_gt_filter(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"number": {"$gt": 0.0}})
         self.assert_documents_are_equal(
             result, [doc for doc in filterable_docs if "number" in doc.meta and doc.meta["number"] > 0]
         )
 
     def test_gt_filter_non_numeric(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"page": {"$gt": "100"}})
 
     def test_gt_filter_table(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"dataframe": {"$gt": pd.DataFrame([[1, 2, 3], [-1, -2, -3]])}})
 
     def test_gt_filter_embedding(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"embedding": {"$gt": TEST_EMBEDDING_1}})
 
 
 class LegacyFilterDocumentsGreaterThanEqualTest(AssertDocumentsEqualMixin, FilterableDocsFixtureMixin):
     """
@@ -552,31 +567,35 @@
         @pytest.fixture
         def document_store(self):
             return MyDocumentStore()
     ```
     """
 
     def test_gte_filter(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"number": {"$gte": -2}})
         self.assert_documents_are_equal(
             result, [doc for doc in filterable_docs if "number" in doc.meta and doc.meta["number"] >= -2]
         )
 
     def test_gte_filter_non_numeric(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"page": {"$gte": "100"}})
 
     def test_gte_filter_table(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"dataframe": {"$gte": pd.DataFrame([[1, 2, 3], [-1, -2, -3]])}})
 
     def test_gte_filter_embedding(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"embedding": {"$gte": TEST_EMBEDDING_1}})
 
 
 class LegacyFilterDocumentsLessThanTest(AssertDocumentsEqualMixin, FilterableDocsFixtureMixin):
     """
@@ -590,31 +609,35 @@
         @pytest.fixture
         def document_store(self):
             return MyDocumentStore()
     ```
     """
 
     def test_lt_filter(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"number": {"$lt": 0.0}})
         self.assert_documents_are_equal(
             result, [doc for doc in filterable_docs if doc.meta.get("number") is not None and doc.meta["number"] < 0]
         )
 
     def test_lt_filter_non_numeric(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"page": {"$lt": "100"}})
 
     def test_lt_filter_table(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"dataframe": {"$lt": pd.DataFrame([[1, 2, 3], [-1, -2, -3]])}})
 
     def test_lt_filter_embedding(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"embedding": {"$lt": TEST_EMBEDDING_2}})
 
 
 class LegacyFilterDocumentsLessThanEqualTest(AssertDocumentsEqualMixin, FilterableDocsFixtureMixin):
     """
@@ -628,31 +651,35 @@
         @pytest.fixture
         def document_store(self):
             return MyDocumentStore()
     ```
     """
 
     def test_lte_filter(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"number": {"$lte": 2.0}})
         self.assert_documents_are_equal(
             result, [doc for doc in filterable_docs if doc.meta.get("number") is not None and doc.meta["number"] <= 2.0]
         )
 
     def test_lte_filter_non_numeric(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"page": {"$lte": "100"}})
 
     def test_lte_filter_table(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"dataframe": {"$lte": pd.DataFrame([[1, 2, 3], [-1, -2, -3]])}})
 
     def test_lte_filter_embedding(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"embedding": {"$lte": TEST_EMBEDDING_1}})
 
 
 class LegacyFilterDocumentsSimpleLogicalTest(AssertDocumentsEqualMixin, FilterableDocsFixtureMixin):
     """
@@ -666,14 +693,15 @@
         @pytest.fixture
         def document_store(self):
             return MyDocumentStore()
     ```
     """
 
     def test_filter_simple_or(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         filters = {"$or": {"name": {"$in": ["name_0", "name_1"]}, "number": {"$lt": 1.0}}}
         result = document_store.filter_documents(filters=filters)
         self.assert_documents_are_equal(
             result,
             [
                 doc
@@ -682,38 +710,41 @@
                 or doc.meta.get("name") in ["name_0", "name_1"]
             ],
         )
 
     def test_filter_simple_implicit_and_with_multi_key_dict(
         self, document_store: DocumentStore, filterable_docs: List[Document]
     ):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"number": {"$lte": 2.0, "$gte": 0.0}})
         self.assert_documents_are_equal(
             result,
             [
                 doc
                 for doc in filterable_docs
                 if "number" in doc.meta and doc.meta["number"] >= 0.0 and doc.meta["number"] <= 2.0
             ],
         )
 
     def test_filter_simple_explicit_and_with_list(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"number": {"$and": [{"$lte": 2}, {"$gte": 0}]}})
         self.assert_documents_are_equal(
             result,
             [
                 doc
                 for doc in filterable_docs
                 if "number" in doc.meta and doc.meta["number"] <= 2.0 and doc.meta["number"] >= 0.0
             ],
         )
 
     def test_filter_simple_implicit_and(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"number": {"$lte": 2.0, "$gte": 0}})
         self.assert_documents_are_equal(
             result,
             [
                 doc
                 for doc in filterable_docs
@@ -734,14 +765,15 @@
         @pytest.fixture
         def document_store(self):
             return MyDocumentStore()
     ```
     """
 
     def test_filter_nested_implicit_and(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         filters_simplified = {"number": {"$lte": 2, "$gte": 0}, "name": ["name_0", "name_1"]}
         result = document_store.filter_documents(filters=filters_simplified)
         self.assert_documents_are_equal(
             result,
             [
                 doc
@@ -752,14 +784,15 @@
                     and doc.meta["number"] >= 0
                     and doc.meta.get("name") in ["name_0", "name_1"]
                 )
             ],
         )
 
     def test_filter_nested_or(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         filters = {"$or": {"name": {"$or": [{"$eq": "name_0"}, {"$eq": "name_1"}]}, "number": {"$lt": 1.0}}}
         result = document_store.filter_documents(filters=filters)
         self.assert_documents_are_equal(
             result,
             [
                 doc
@@ -768,14 +801,15 @@
                     doc.meta.get("name") in ["name_0", "name_1"]
                     or (doc.meta.get("number") is not None and doc.meta["number"] < 1)
                 )
             ],
         )
 
     def test_filter_nested_and_or_explicit(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         filters_simplified = {
             "$and": {"page": {"$eq": "123"}, "$or": {"name": {"$in": ["name_0", "name_1"]}, "number": {"$lt": 1.0}}}
         }
         result = document_store.filter_documents(filters=filters_simplified)
         self.assert_documents_are_equal(
             result,
@@ -789,14 +823,15 @@
                         or ("number" in doc.meta and doc.meta["number"] < 1)
                     )
                 )
             ],
         )
 
     def test_filter_nested_and_or_implicit(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         filters_simplified = {
             "page": {"$eq": "123"},
             "$or": {"name": {"$in": ["name_0", "name_1"]}, "number": {"$lt": 1.0}},
         }
         result = document_store.filter_documents(filters=filters_simplified)
         self.assert_documents_are_equal(
@@ -811,14 +846,15 @@
                         or ("number" in doc.meta and doc.meta["number"] < 1)
                     )
                 )
             ],
         )
 
     def test_filter_nested_or_and(self, document_store: DocumentStore, filterable_docs: List[Document]):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         filters_simplified = {
             "$or": {
                 "number": {"$lt": 1},
                 "$and": {"name": {"$in": ["name_0", "name_1"]}, "$not": {"chapter": {"$eq": "intro"}}},
             }
         }
@@ -834,14 +870,15 @@
                 )
             ],
         )
 
     def test_filter_nested_multiple_identical_operators_same_level(
         self, document_store: DocumentStore, filterable_docs: List[Document]
     ):
+        """"""  # noqa # pylint: disable=C0112
         document_store.write_documents(filterable_docs)
         filters = {
             "$or": [
                 {"$and": {"name": {"$in": ["name_0", "name_1"]}, "page": "100"}},
                 {"$and": {"chapter": {"$in": ["intro", "abstract"]}, "page": "123"}},
             ]
         }
@@ -883,18 +920,20 @@
         @pytest.fixture
         def document_store(self):
             return MyDocumentStore()
     ```
     """
 
     def test_no_filter_empty(self, document_store: DocumentStore):
+        """"""  # noqa # pylint: disable=C0112
         assert document_store.filter_documents() == []
         assert document_store.filter_documents(filters={}) == []
 
     def test_no_filter_not_empty(self, document_store: DocumentStore):
+        """"""  # noqa # pylint: disable=C0112
         docs = [Document(content="test doc")]
         document_store.write_documents(docs)
         assert document_store.filter_documents() == docs
         assert document_store.filter_documents(filters={}) == docs
 
 
 class FilterDocumentsTest(AssertDocumentsEqualMixin, FilterableDocsFixtureMixin):
@@ -909,70 +948,79 @@
         @pytest.fixture
         def document_store(self):
             return MyDocumentStore()
     ```
     """
 
     def test_no_filters(self, document_store):
+        """Test filter_documents() with empty filters"""
         self.assert_documents_are_equal(document_store.filter_documents(), [])
         self.assert_documents_are_equal(document_store.filter_documents(filters={}), [])
         docs = [Document(content="test doc")]
         document_store.write_documents(docs)
         self.assert_documents_are_equal(document_store.filter_documents(), docs)
         self.assert_documents_are_equal(document_store.filter_documents(filters={}), docs)
 
     # == comparator
     def test_comparison_equal(self, document_store, filterable_docs):
+        """Test filter_documents() with == comparator"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"field": "meta.number", "operator": "==", "value": 100})
         self.assert_documents_are_equal(result, [d for d in filterable_docs if d.meta.get("number") == 100])
 
     def test_comparison_equal_with_dataframe(self, document_store, filterable_docs):
+        """Test filter_documents() with == comparator and dataframe"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(
             filters={"field": "dataframe", "operator": "==", "value": pd.DataFrame([1])}
         )
         self.assert_documents_are_equal(
             result, [d for d in filterable_docs if d.dataframe is not None and d.dataframe.equals(pd.DataFrame([1]))]
         )
 
     def test_comparison_equal_with_none(self, document_store, filterable_docs):
+        """Test filter_documents() with == comparator and None"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"field": "meta.number", "operator": "==", "value": None})
         self.assert_documents_are_equal(result, [d for d in filterable_docs if d.meta.get("number") is None])
 
     # != comparator
     def test_comparison_not_equal(self, document_store, filterable_docs):
+        """Test filter_documents() with != comparator"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents({"field": "meta.number", "operator": "!=", "value": 100})
         self.assert_documents_are_equal(result, [d for d in filterable_docs if d.meta.get("number") != 100])
 
     def test_comparison_not_equal_with_dataframe(self, document_store, filterable_docs):
+        """Test filter_documents() with != comparator and dataframe"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(
             filters={"field": "dataframe", "operator": "!=", "value": pd.DataFrame([1])}
         )
         self.assert_documents_are_equal(
             result, [d for d in filterable_docs if d.dataframe is None or not d.dataframe.equals(pd.DataFrame([1]))]
         )
 
     def test_comparison_not_equal_with_none(self, document_store, filterable_docs):
+        """Test filter_documents() with != comparator and None"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"field": "meta.number", "operator": "!=", "value": None})
         self.assert_documents_are_equal(result, [d for d in filterable_docs if d.meta.get("number") is not None])
 
     # > comparator
     def test_comparison_greater_than(self, document_store, filterable_docs):
+        """Test filter_documents() with > comparator"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents({"field": "meta.number", "operator": ">", "value": 0})
         self.assert_documents_are_equal(
             result, [d for d in filterable_docs if d.meta.get("number") is not None and d.meta["number"] > 0]
         )
 
     def test_comparison_greater_than_with_iso_date(self, document_store, filterable_docs):
+        """Test filter_documents() with > comparator and datetime"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(
             {"field": "meta.date", "operator": ">", "value": "1972-12-11T19:54:58"}
         )
         self.assert_documents_are_equal(
             result,
             [
@@ -980,42 +1028,48 @@
                 for d in filterable_docs
                 if d.meta.get("date") is not None
                 and datetime.fromisoformat(d.meta["date"]) > datetime.fromisoformat("1972-12-11T19:54:58")
             ],
         )
 
     def test_comparison_greater_than_with_string(self, document_store, filterable_docs):
+        """Test filter_documents() with > comparator and string"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"field": "meta.number", "operator": ">", "value": "1"})
 
     def test_comparison_greater_than_with_dataframe(self, document_store, filterable_docs):
+        """Test filter_documents() with > comparator and dataframe"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"field": "dataframe", "operator": ">", "value": pd.DataFrame([1])})
 
     def test_comparison_greater_than_with_list(self, document_store, filterable_docs):
+        """Test filter_documents() with > comparator and list"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"field": "meta.number", "operator": ">", "value": [1]})
 
     def test_comparison_greater_than_with_none(self, document_store, filterable_docs):
+        """Test filter_documents() with > comparator and None"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"field": "meta.number", "operator": ">", "value": None})
         self.assert_documents_are_equal(result, [])
 
     # >= comparator
     def test_comparison_greater_than_equal(self, document_store, filterable_docs):
+        """Test filter_documents() with >= comparator"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents({"field": "meta.number", "operator": ">=", "value": 0})
         self.assert_documents_are_equal(
             result, [d for d in filterable_docs if d.meta.get("number") is not None and d.meta["number"] >= 0]
         )
 
     def test_comparison_greater_than_equal_with_iso_date(self, document_store, filterable_docs):
+        """Test filter_documents() with >= comparator and datetime"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(
             {"field": "meta.date", "operator": ">=", "value": "1969-07-21T20:17:40"}
         )
         self.assert_documents_are_equal(
             result,
             [
@@ -1023,44 +1077,50 @@
                 for d in filterable_docs
                 if d.meta.get("date") is not None
                 and datetime.fromisoformat(d.meta["date"]) >= datetime.fromisoformat("1969-07-21T20:17:40")
             ],
         )
 
     def test_comparison_greater_than_equal_with_string(self, document_store, filterable_docs):
+        """Test filter_documents() with >= comparator and string"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"field": "meta.number", "operator": ">=", "value": "1"})
 
     def test_comparison_greater_than_equal_with_dataframe(self, document_store, filterable_docs):
+        """Test filter_documents() with >= comparator and dataframe"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(
                 filters={"field": "dataframe", "operator": ">=", "value": pd.DataFrame([1])}
             )
 
     def test_comparison_greater_than_equal_with_list(self, document_store, filterable_docs):
+        """Test filter_documents() with >= comparator and list"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"field": "meta.number", "operator": ">=", "value": [1]})
 
     def test_comparison_greater_than_equal_with_none(self, document_store, filterable_docs):
+        """Test filter_documents() with >= comparator and None"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"field": "meta.number", "operator": ">=", "value": None})
         self.assert_documents_are_equal(result, [])
 
     # < comparator
     def test_comparison_less_than(self, document_store, filterable_docs):
+        """Test filter_documents() with < comparator"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents({"field": "meta.number", "operator": "<", "value": 0})
         self.assert_documents_are_equal(
             result, [d for d in filterable_docs if d.meta.get("number") is not None and d.meta["number"] < 0]
         )
 
     def test_comparison_less_than_with_iso_date(self, document_store, filterable_docs):
+        """Test filter_documents() with < comparator and datetime"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(
             {"field": "meta.date", "operator": "<", "value": "1969-07-21T20:17:40"}
         )
         self.assert_documents_are_equal(
             result,
             [
@@ -1068,42 +1128,48 @@
                 for d in filterable_docs
                 if d.meta.get("date") is not None
                 and datetime.fromisoformat(d.meta["date"]) < datetime.fromisoformat("1969-07-21T20:17:40")
             ],
         )
 
     def test_comparison_less_than_with_string(self, document_store, filterable_docs):
+        """Test filter_documents() with < comparator and string"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"field": "meta.number", "operator": "<", "value": "1"})
 
     def test_comparison_less_than_with_dataframe(self, document_store, filterable_docs):
+        """Test filter_documents() with < comparator and dataframe"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"field": "dataframe", "operator": "<", "value": pd.DataFrame([1])})
 
     def test_comparison_less_than_with_list(self, document_store, filterable_docs):
+        """Test filter_documents() with < comparator and list"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"field": "meta.number", "operator": "<", "value": [1]})
 
     def test_comparison_less_than_with_none(self, document_store, filterable_docs):
+        """Test filter_documents() with < comparator and None"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"field": "meta.number", "operator": "<", "value": None})
         self.assert_documents_are_equal(result, [])
 
     # <= comparator
     def test_comparison_less_than_equal(self, document_store, filterable_docs):
+        """Test filter_documents() with <="""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents({"field": "meta.number", "operator": "<=", "value": 0})
         self.assert_documents_are_equal(
             result, [d for d in filterable_docs if d.meta.get("number") is not None and d.meta["number"] <= 0]
         )
 
     def test_comparison_less_than_equal_with_iso_date(self, document_store, filterable_docs):
+        """Test filter_documents() with <= comparator and datetime"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(
             {"field": "meta.date", "operator": "<=", "value": "1969-07-21T20:17:40"}
         )
         self.assert_documents_are_equal(
             result,
             [
@@ -1111,71 +1177,82 @@
                 for d in filterable_docs
                 if d.meta.get("date") is not None
                 and datetime.fromisoformat(d.meta["date"]) <= datetime.fromisoformat("1969-07-21T20:17:40")
             ],
         )
 
     def test_comparison_less_than_equal_with_string(self, document_store, filterable_docs):
+        """Test filter_documents() with <= comparator and string"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"field": "meta.number", "operator": "<=", "value": "1"})
 
     def test_comparison_less_than_equal_with_dataframe(self, document_store, filterable_docs):
+        """Test filter_documents() with <= comparator and dataframe"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(
                 filters={"field": "dataframe", "operator": "<=", "value": pd.DataFrame([1])}
             )
 
     def test_comparison_less_than_equal_with_list(self, document_store, filterable_docs):
+        """Test filter_documents() with <= comparator and list"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"field": "meta.number", "operator": "<=", "value": [1]})
 
     def test_comparison_less_than_equal_with_none(self, document_store, filterable_docs):
+        """Test filter_documents() with <= comparator and None"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(filters={"field": "meta.number", "operator": "<=", "value": None})
         self.assert_documents_are_equal(result, [])
 
     # in comparator
     def test_comparison_in(self, document_store, filterable_docs):
+        """Test filter_documents() with 'in' comparator"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents({"field": "meta.number", "operator": "in", "value": [10, -10]})
         assert len(result)
         expected = [d for d in filterable_docs if d.meta.get("number") is not None and d.meta["number"] in [10, -10]]
         self.assert_documents_are_equal(result, expected)
 
     def test_comparison_in_with_with_non_list(self, document_store, filterable_docs):
+        """Test filter_documents() with 'in' comparator and non-iterable"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents({"field": "meta.number", "operator": "in", "value": 9})
 
     def test_comparison_in_with_with_non_list_iterable(self, document_store, filterable_docs):
+        """Test filter_documents() with 'in' comparator and iterable"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents({"field": "meta.number", "operator": "in", "value": (10, 11)})
 
     # not in comparator
     def test_comparison_not_in(self, document_store, filterable_docs):
+        """Test filter_documents() with 'not in' comparator"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents({"field": "meta.number", "operator": "not in", "value": [9, 10]})
         self.assert_documents_are_equal(result, [d for d in filterable_docs if d.meta.get("number") not in [9, 10]])
 
     def test_comparison_not_in_with_with_non_list(self, document_store, filterable_docs):
+        """Test filter_documents() with 'not in' comparator and non-iterable"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents({"field": "meta.number", "operator": "not in", "value": 9})
 
     def test_comparison_not_in_with_with_non_list_iterable(self, document_store, filterable_docs):
+        """Test filter_documents() with 'not in' comparator and iterable"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents({"field": "meta.number", "operator": "not in", "value": (10, 11)})
 
     # Logical operator
     def test_and_operator(self, document_store, filterable_docs):
+        """Test filter_documents() with 'AND' operator"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(
             filters={
                 "operator": "AND",
                 "conditions": [
                     {"field": "meta.number", "operator": "==", "value": 100},
                     {"field": "meta.name", "operator": "==", "value": "name_0"},
@@ -1183,14 +1260,15 @@
             }
         )
         self.assert_documents_are_equal(
             result, [d for d in filterable_docs if d.meta.get("number") == 100 and d.meta.get("name") == "name_0"]
         )
 
     def test_or_operator(self, document_store, filterable_docs):
+        """Test filter_documents() with 'OR' operator"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(
             filters={
                 "operator": "OR",
                 "conditions": [
                     {"field": "meta.number", "operator": "==", "value": 100},
                     {"field": "meta.name", "operator": "==", "value": "name_0"},
@@ -1198,14 +1276,15 @@
             }
         )
         self.assert_documents_are_equal(
             result, [d for d in filterable_docs if d.meta.get("number") == 100 or d.meta.get("name") == "name_0"]
         )
 
     def test_not_operator(self, document_store, filterable_docs):
+        """Test filter_documents() with 'NOT' operator"""
         document_store.write_documents(filterable_docs)
         result = document_store.filter_documents(
             filters={
                 "operator": "NOT",
                 "conditions": [
                     {"field": "meta.number", "operator": "==", "value": 100},
                     {"field": "meta.name", "operator": "==", "value": "name_0"},
@@ -1214,44 +1293,50 @@
         )
         self.assert_documents_are_equal(
             result, [d for d in filterable_docs if not (d.meta.get("number") == 100 and d.meta.get("name") == "name_0")]
         )
 
     # Malformed filters
     def test_missing_top_level_operator_key(self, document_store, filterable_docs):
+        """Test filter_documents() with top-level operator"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(
                 filters={"conditions": [{"field": "meta.name", "operator": "==", "value": "test"}]}
             )
 
     def test_missing_top_level_conditions_key(self, document_store, filterable_docs):
+        """Test filter_documents() with missing top-level condition key"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(filters={"operator": "AND"})
 
     def test_missing_condition_field_key(self, document_store, filterable_docs):
+        """Test filter_documents() with missing condition key"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(
                 filters={"operator": "AND", "conditions": [{"operator": "==", "value": "test"}]}
             )
 
     def test_missing_condition_operator_key(self, document_store, filterable_docs):
+        """Test filter_documents() with missing operator key"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(
                 filters={"operator": "AND", "conditions": [{"field": "meta.name", "value": "test"}]}
             )
 
     def test_missing_condition_value_key(self, document_store, filterable_docs):
+        """Test filter_documents() with missing condition value"""
         document_store.write_documents(filterable_docs)
         with pytest.raises(FilterError):
             document_store.filter_documents(
                 filters={"operator": "AND", "conditions": [{"field": "meta.name", "operator": "=="}]}
             )
 
 
 class DocumentStoreBaseTests(CountDocumentsTest, WriteDocumentsTest, DeleteDocumentsTest, FilterDocumentsTest):
     @pytest.fixture
     def document_store(self) -> DocumentStore:
+        """Base fixture, to be reimplemented when deriving from DocumentStoreBaseTests"""
         raise NotImplementedError()
```

### Comparing `haystack_ai-2.0.1rc2/haystack/testing/factory.py` & `haystack_ai-2.1.0rc1/haystack/testing/factory.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/testing/test_utils.py` & `haystack_ai-2.1.0rc1/haystack/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/testing/sample_components/__init__.py` & `haystack_ai-2.1.0rc1/haystack/testing/sample_components/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/testing/sample_components/accumulate.py` & `haystack_ai-2.1.0rc1/haystack/testing/sample_components/accumulate.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,44 +15,48 @@
     return first + second
 
 
 @component
 class Accumulate:
     """
     Accumulates the value flowing through the connection into an internal attribute.
-    The sum function can be customized.
 
-    Example of how to deal with serialization when some of the parameters
+    The sum function can be customized. Example of how to deal with serialization when some of the parameters
     are not directly serializable.
     """
 
     def __init__(self, function: Optional[Callable] = None):
         """
-        :param function: the function to use to accumulate the values.
+        Class constructor
+
+        :param function:
+            the function to use to accumulate the values.
             The function must take exactly two values.
             If it's a callable, it's used as it is.
             If it's a string, the component will look for it in sys.modules and
             import it at need. This is also a parameter.
         """
         self.state = 0
         self.function: Callable = _default_function if function is None else function  # type: ignore
 
-    def to_dict(self) -> Dict[str, Any]:  # pylint: disable=missing-function-docstring
+    def to_dict(self) -> Dict[str, Any]:
+        """Converts the component to a dictionary"""
         module = sys.modules.get(self.function.__module__)
         if not module:
             raise ValueError("Could not locate the import module.")
         if module == builtins:
             function_name = self.function.__name__
         else:
             function_name = f"{module.__name__}.{self.function.__name__}"
 
         return default_to_dict(self, function=function_name)
 
     @classmethod
-    def from_dict(cls, data: Dict[str, Any]) -> "Accumulate":  # pylint: disable=missing-function-docstring
+    def from_dict(cls, data: Dict[str, Any]) -> "Accumulate":
+        """Loads the component from a dictionary"""
         if "type" not in data:
             raise ComponentDeserializationError("Missing 'type' in component serialization data")
         if data["type"] != f"{cls.__module__}.{cls.__name__}":
             raise ComponentDeserializationError(f"Class '{data['type']}' can't be deserialized as '{cls.__name__}'")
 
         init_params = data.get("init_parameters", {})
 
@@ -66,11 +70,12 @@
 
         return cls(function=accumulator_function)
 
     @component.output_types(value=int)
     def run(self, value: int):
         """
         Accumulates the value flowing through the connection into an internal attribute.
+
         The sum function can be customized.
         """
         self.state = self.function(self.state, value)
         return {"value": self.state}
```

### Comparing `haystack_ai-2.0.1rc2/haystack/testing/sample_components/add_value.py` & `haystack_ai-2.1.0rc1/haystack/testing/sample_components/add_value.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/testing/sample_components/concatenate.py` & `haystack_ai-2.1.0rc1/haystack/testing/sample_components/concatenate.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/testing/sample_components/fstring.py` & `haystack_ai-2.1.0rc1/haystack/testing/sample_components/fstring.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/testing/sample_components/greet.py` & `haystack_ai-2.1.0rc1/haystack/testing/sample_components/greet.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 class Greet:
     """
     Logs a greeting message without affecting the value passing on the connection.
     """
 
     def __init__(self, message: str = "\nGreeting component says: Hi! The value is {value}\n", log_level: str = "INFO"):
         """
+        Class constructor
+
         :param message: the message to log. Can use `{value}` to embed the value.
         :param log_level: the level to log at.
         """
         if log_level and not getattr(logging, log_level):
             raise ValueError(f"This log level does not exist: {log_level}")
         self.message = message
         self.log_level = log_level
```

### Comparing `haystack_ai-2.0.1rc2/haystack/testing/sample_components/joiner.py` & `haystack_ai-2.1.0rc1/haystack/testing/sample_components/joiner.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 
 
 @component
 class StringJoiner:
     @component.output_types(output=str)
     def run(self, input_str: Variadic[str]):
         """
-        Take strings from multiple input nodes and join them
-        into a single one returned in output. Since `input_str`
-        is Variadic, we know we'll receive a List[str].
+        Take strings from multiple input nodes and join them into a single one returned in output.
+
+        Since `input_str` is Variadic, we know we'll receive a List[str].
         """
         return {"output": " ".join(input_str)}
 
 
 @component
 class StringListJoiner:
     @component.output_types(output=str)
     def run(self, inputs: Variadic[List[str]]):
         """
-        Take list of strings from multiple input nodes and join them
-        into a single one returned in output. Since `input_str`
-        is Variadic, we know we'll receive a List[List[str]].
+        Take list of strings from multiple input nodes and join them into a single one returned in output.
+
+        Since `input_str` is Variadic, we know we'll receive a List[List[str]].
         """
         retval: List[str] = []
         for list_of_strings in inputs:
             retval += list_of_strings
 
         return {"output": retval}
```

### Comparing `haystack_ai-2.0.1rc2/haystack/testing/sample_components/parity.py` & `haystack_ai-2.1.0rc1/haystack/testing/sample_components/parity.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/testing/sample_components/remainder.py` & `haystack_ai-2.1.0rc1/haystack/testing/sample_components/remainder.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/testing/sample_components/subtract.py` & `haystack_ai-2.1.0rc1/haystack/testing/sample_components/subtract.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,11 +9,13 @@
     """
     Compute the difference between two values.
     """
 
     @component.output_types(difference=int)
     def run(self, first_value: int, second_value: int):
         """
+        Run the component.
+
         :param first_value: name of the connection carrying the value to subtract from.
         :param second_value: name of the connection carrying the value to subtract.
         """
         return {"difference": first_value - second_value}
```

### Comparing `haystack_ai-2.0.1rc2/haystack/testing/sample_components/threshold.py` & `haystack_ai-2.1.0rc1/haystack/testing/sample_components/threshold.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,31 +5,29 @@
 
 from haystack.core.component import component
 
 
 @component
 class Threshold:  # pylint: disable=too-few-public-methods
     """
-    Redirects the value, unchanged, along a different connection whether the value is above
-    or below the given threshold.
+    Redirects the value, along a different connection whether the value is above or below the given threshold.
 
     :param threshold: the number to compare the input value against. This is also a parameter.
     """
 
     def __init__(self, threshold: int = 10):
         """
         :param threshold: the number to compare the input value against.
         """
         self.threshold = threshold
 
     @component.output_types(above=int, below=int)
     def run(self, value: int, threshold: Optional[int] = None):
         """
-        Redirects the value, unchanged, along a different connection whether the value is above
-        or below the given threshold.
+        Redirects the value, along a different connection whether the value is above or below the given threshold.
 
         :param threshold: the number to compare the input value against. This is also a parameter.
         """
         if threshold is None:
             threshold = self.threshold
 
         if value < threshold:
```

### Comparing `haystack_ai-2.0.1rc2/haystack/tracing/datadog.py` & `haystack_ai-2.1.0rc1/haystack/tracing/datadog.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,21 +10,33 @@
 
 
 class DatadogSpan(Span):
     def __init__(self, span: "ddtrace.Span") -> None:
         self._span = span
 
     def set_tag(self, key: str, value: Any) -> None:
+        """
+        Set a single tag on the span.
+
+        :param key: the name of the tag.
+        :param value: the value of the tag.
+        """
         coerced_value = tracing_utils.coerce_tag_value(value)
         self._span.set_tag(key, coerced_value)
 
     def raw_span(self) -> Any:
+        """
+        Provides access to the underlying span object of the tracer.
+
+        :return: The underlying span object.
+        """
         return self._span
 
     def get_correlation_data_for_logs(self) -> Dict[str, Any]:
+        """Return a dictionary with correlation data for logs."""
         raw_span = self.raw_span()
         if not raw_span:
             return {}
 
         # https://docs.datadoghq.com/tracing/other_telemetry/connect_logs_and_traces/python/#no-standard-library-logging
         trace_id, span_id = (str((1 << 64) - 1 & raw_span.trace_id), raw_span.span_id)
 
@@ -40,20 +52,22 @@
 class DatadogTracer(Tracer):
     def __init__(self, tracer: "ddtrace.Tracer") -> None:
         ddtrace_import.check()
         self._tracer = tracer
 
     @contextlib.contextmanager
     def trace(self, operation_name: str, tags: Optional[Dict[str, Any]] = None) -> Iterator[Span]:
+        """Activate and return a new span that inherits from the current active span."""
         with self._tracer.trace(operation_name) as span:
             span = DatadogSpan(span)
             if tags:
                 span.set_tags(tags)
 
             yield span
 
     def current_span(self) -> Optional[Span]:
+        """Return the current active span"""
         current_span = self._tracer.current_span()
         if current_span is None:
             return None
 
         return DatadogSpan(current_span)
```

### Comparing `haystack_ai-2.0.1rc2/haystack/tracing/opentelemetry.py` & `haystack_ai-2.1.0rc1/haystack/tracing/opentelemetry.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,38 +11,52 @@
 
 
 class OpenTelemetrySpan(Span):
     def __init__(self, span: "opentelemetry.trace.Span") -> None:
         self._span = span
 
     def set_tag(self, key: str, value: Any) -> None:
+        """
+        Set a single tag on the span.
+
+        :param key: the name of the tag.
+        :param value: the value of the tag.
+        """
         coerced_value = tracing_utils.coerce_tag_value(value)
         self._span.set_attribute(key, coerced_value)
 
     def raw_span(self) -> Any:
+        """
+        Provides access to the underlying span object of the tracer.
+
+        :return: The underlying span object.
+        """
         return self._span
 
     def get_correlation_data_for_logs(self) -> Dict[str, Any]:
+        """Return a dictionary with correlation data for logs."""
         span_context = self._span.get_span_context()
         return {"trace_id": span_context.trace_id, "span_id": span_context.span_id}
 
 
 class OpenTelemetryTracer(Tracer):
     def __init__(self, tracer: "opentelemetry.trace.Tracer") -> None:
         opentelemetry_import.check()
         self._tracer = tracer
 
     @contextlib.contextmanager
     def trace(self, operation_name: str, tags: Optional[Dict[str, Any]] = None) -> Iterator[Span]:
+        """Activate and return a new span that inherits from the current active span."""
         with self._tracer.start_as_current_span(operation_name) as raw_span:
             span = OpenTelemetrySpan(raw_span)
             if tags:
                 span.set_tags(tags)
 
             yield span
 
     def current_span(self) -> Optional[Span]:
+        """Return the current active span"""
         current_span = opentelemetry.trace.get_current_span()
         if isinstance(current_span, opentelemetry.trace.NonRecordingSpan):
             return None
 
         return OpenTelemetrySpan(current_span)
```

### Comparing `haystack_ai-2.0.1rc2/haystack/tracing/tracer.py` & `haystack_ai-2.1.0rc1/haystack/tracing/tracer.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,43 +12,47 @@
 
 
 class Span(abc.ABC):
     """Interface for an instrumented operation."""
 
     @abc.abstractmethod
     def set_tag(self, key: str, value: Any) -> None:
-        """Set a single tag on the span.
+        """
+        Set a single tag on the span.
 
         Note that the value will be serialized to a string, so it's best to use simple types like strings, numbers, or
         booleans.
 
         :param key: the name of the tag.
         :param value: the value of the tag.
         """
         pass
 
     def set_tags(self, tags: Dict[str, Any]) -> None:
-        """Set multiple tags on the span.
+        """
+        Set multiple tags on the span.
 
         :param tags: a mapping of tag names to tag values.
         """
         for key, value in tags.items():
             self.set_tag(key, value)
 
     def raw_span(self) -> Any:
-        """Provides access to the underlying span object of the tracer.
+        """
+        Provides access to the underlying span object of the tracer.
 
         Use this if you need full access to the underlying span object.
 
         :return: The underlying span object.
         """
         return self
 
     def set_content_tag(self, key: str, value: Any) -> None:
-        """Set a single tag containing content information.
+        """
+        Set a single tag containing content information.
 
         Content is sensitive information such as
         - the content of a query
         - the content of a document
         - the content of an answer
 
         By default, this behavior is disabled. To enable it
@@ -58,79 +62,89 @@
         :param key: the name of the tag.
         :param value: the value of the tag.
         """
         if tracer.is_content_tracing_enabled:
             self.set_tag(key, value)
 
     def get_correlation_data_for_logs(self) -> Dict[str, Any]:
-        """Return a dictionary with correlation data for logs.
+        """
+        Return a dictionary with correlation data for logs.
 
-        This is useful if you want to correlate logs with traces."""
+        This is useful if you want to correlate logs with traces.
+        """
         return {}
 
 
 class Tracer(abc.ABC):
     """Interface for instrumenting code by creating and submitting spans."""
 
     @abc.abstractmethod
     @contextlib.contextmanager
     def trace(self, operation_name: str, tags: Optional[Dict[str, Any]] = None) -> Iterator[Span]:
-        """Trace the execution of a block of code.
+        """
+        Trace the execution of a block of code.
 
         :param operation_name: the name of the operation being traced.
         :param tags: tags to apply to the newly created span.
         :return: the newly created span.
         """
         pass
 
     @abc.abstractmethod
     def current_span(self) -> Optional[Span]:
-        """Returns the currently active span. If no span is active, returns `None`.
+        """
+        Returns the currently active span. If no span is active, returns `None`.
 
         :return: Currently active span or `None` if no span is active.
         """
         pass
 
 
 class ProxyTracer(Tracer):
-    """Container for the actual tracer instance.
+    """
+    Container for the actual tracer instance.
 
     This eases
     - replacing the actual tracer instance without having to change the global tracer instance
     - implementing default behavior for the tracer
     """
 
     def __init__(self, provided_tracer: Tracer) -> None:
         self.actual_tracer: Tracer = provided_tracer
         self.is_content_tracing_enabled = os.getenv(HAYSTACK_CONTENT_TRACING_ENABLED_ENV_VAR, "false").lower() == "true"
 
     @contextlib.contextmanager
     def trace(self, operation_name: str, tags: Optional[Dict[str, Any]] = None) -> Iterator[Span]:
+        """Activate and return a new span that inherits from the current active span."""
         with self.actual_tracer.trace(operation_name, tags=tags) as span:
             yield span
 
     def current_span(self) -> Optional[Span]:
+        """Return the current active span"""
         return self.actual_tracer.current_span()
 
 
 class NullSpan(Span):
     """A no-op implementation of the `Span` interface. This is used when tracing is disabled."""
 
     def set_tag(self, key: str, value: Any) -> None:
+        """Set a single tag on the span."""
         pass
 
 
 class NullTracer(Tracer):
     """A no-op implementation of the `Tracer` interface. This is used when tracing is disabled."""
 
     @contextlib.contextmanager
     def trace(self, operation_name: str, tags: Optional[Dict[str, Any]] = None) -> Iterator[Span]:
+        """Activate and return a new span that inherits from the current active span."""
         yield NullSpan()
 
     def current_span(self) -> Optional[Span]:
+        """Return the current active span"""
         return NullSpan()
 
 
 # We use the proxy pattern to allow for easy enabling and disabling of tracing without having to change the global
 # tracer instance. That's especially convenient if users import the object directly
 # (in that case we'd have to monkey-patch it in all of these modules).
 tracer: ProxyTracer = ProxyTracer(provided_tracer=NullTracer())
@@ -148,15 +162,16 @@
 
 def is_tracing_enabled() -> bool:
     """Return whether tracing is enabled."""
     return not isinstance(tracer.actual_tracer, NullTracer)
 
 
 def auto_enable_tracing() -> None:
-    """Auto-enable the right tracing backend.
+    """
+    Auto-enable the right tracing backend.
 
     This behavior can be disabled by setting the environment variable `HAYSTACK_AUTO_TRACE_ENABLED` to `false`.
     Note that it will only work correctly if tracing was configured _before_ Haystack is imported.
     """
     if os.getenv(HAYSTACK_AUTO_TRACE_ENABLED_ENV_VAR, "true").lower() == "false":
         logger.info(
             "Tracing disabled via environment variable '{env_key}'", env_key=HAYSTACK_AUTO_TRACE_ENABLED_ENV_VAR
```

### Comparing `haystack_ai-2.0.1rc2/haystack/tracing/utils.py` & `haystack_ai-2.1.0rc1/haystack/tracing/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 logger = logging.getLogger(__name__)
 
 PRIMITIVE_TYPES = (bool, str, int, float)
 
 
 def coerce_tag_value(value: Any) -> Union[bool, str, int, float]:
-    """Coerces span tag values to compatible types for the tracing backend.
+    """
+    Coerces span tag values to compatible types for the tracing backend.
 
     Most tracing libraries don't support sending complex types to the backend. Hence, we need to convert them to
     compatible types.
 
     :param value: an arbitrary value which should be coerced to a compatible type
     :return: the value coerced to a compatible type
     """
```

### Comparing `haystack_ai-2.0.1rc2/haystack/utils/__init__.py` & `haystack_ai-2.1.0rc1/haystack/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/utils/auth.py` & `haystack_ai-2.1.0rc1/haystack/utils/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,24 @@
     ENV_VAR = "env_var"
 
     def __str__(self):
         return self.value
 
     @staticmethod
     def from_str(string: str) -> "SecretType":
-        map = {e.value: e for e in SecretType}
-        type = map.get(string)
-        if type is None:
+        """
+        Convert a string to a SecretType.
+
+        :param string: The string to convert.
+        """
+        mapping = {e.value: e for e in SecretType}
+        _type = mapping.get(string)
+        if _type is None:
             raise ValueError(f"Unknown secret type '{string}'")
-        return type
+        return _type
 
 
 class Secret(ABC):
     """
     Encapsulates a secret used for authentication.
 
     Usage example:
@@ -43,18 +48,17 @@
             The token to use for authentication.
         """
         return TokenSecret(_token=token)
 
     @staticmethod
     def from_env_var(env_vars: Union[str, List[str]], *, strict: bool = True) -> "Secret":
         """
-        Create an environment variable-based secret. Accepts
-        one or more environment variables. Upon resolution, it
-        returns a string token from the first environment variable
-        that is set.
+        Create an environment variable-based secret. Accepts one or more environment variables.
+
+        Upon resolution, it returns a string token from the first environment variable that is set.
 
         :param env_vars:
             A single environment variable or an ordered list of
             candidate environment variables.
         :param strict:
             Whether to raise an exception if none of the environment
             variables are set.
@@ -62,27 +66,28 @@
         if isinstance(env_vars, str):
             env_vars = [env_vars]
         return EnvVarSecret(_env_vars=tuple(env_vars), _strict=strict)
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Convert the secret to a JSON-serializable dictionary.
+
         Some secrets may not be serializable.
 
         :returns:
             The serialized policy.
         """
         out = {"type": self.type.value}
         inner = self._to_dict()
         assert all(k not in inner for k in out.keys())
         out.update(inner)
         return out
 
     @staticmethod
-    def from_dict(dict: Dict[str, Any]) -> "Secret":
+    def from_dict(dict: Dict[str, Any]) -> "Secret":  # noqa:A002
         """
         Create a secret from a JSON-serializable dictionary.
 
         :param dict:
             The dictionary with the serialized data.
         :returns:
             The deserialized secret.
@@ -90,16 +95,15 @@
         secret_map = {SecretType.TOKEN: TokenSecret, SecretType.ENV_VAR: EnvVarSecret}
         secret_type = SecretType.from_str(dict["type"])
         return secret_map[secret_type]._from_dict(dict)  # type: ignore
 
     @abstractmethod
     def resolve_value(self) -> Optional[Any]:
         """
-        Resolve the secret to an atomic value. The semantics
-        of the value is secret-dependent.
+        Resolve the secret to an atomic value. The semantics of the value is secret-dependent.
 
         :returns:
             The value of the secret, if any.
         """
         pass
 
     @property
@@ -112,22 +116,23 @@
 
     @abstractmethod
     def _to_dict(self) -> Dict[str, Any]:
         pass
 
     @staticmethod
     @abstractmethod
-    def _from_dict(dict: Dict[str, Any]) -> "Secret":
+    def _from_dict(_: Dict[str, Any]) -> "Secret":
         pass
 
 
 @dataclass(frozen=True)
 class TokenSecret(Secret):
     """
     A secret that uses a string token/API key.
+
     Cannot be serialized.
     """
 
     _token: str
     _type: SecretType = SecretType.TOKEN
 
     def __post_init__(self):
@@ -139,33 +144,35 @@
 
     def _to_dict(self) -> Dict[str, Any]:
         raise ValueError(
             "Cannot serialize token-based secret. Use an alternative secret type like environment variables."
         )
 
     @staticmethod
-    def _from_dict(dict: Dict[str, Any]) -> "Secret":
+    def _from_dict(_: Dict[str, Any]) -> "Secret":
         raise ValueError(
             "Cannot deserialize token-based secret. Use an alternative secret type like environment variables."
         )
 
     def resolve_value(self) -> Optional[Any]:
+        """Return the token."""
         return self._token
 
     @property
     def type(self) -> SecretType:
+        """The type of the secret."""
         return self._type
 
 
 @dataclass(frozen=True)
 class EnvVarSecret(Secret):
     """
     A secret that accepts one or more environment variables.
-    Upon resolution, it returns a string token from the first
-    environment variable that is set. Can be serialized.
+
+    Upon resolution, it returns a string token from the first environment variable that is set. Can be serialized.
     """
 
     _env_vars: Tuple[str, ...]
     _strict: bool = True
     _type: SecretType = SecretType.ENV_VAR
 
     def __post_init__(self):
@@ -175,30 +182,32 @@
         if len(self._env_vars) == 0:
             raise ValueError("One or more environment variables must be provided for the secret.")
 
     def _to_dict(self) -> Dict[str, Any]:
         return {"env_vars": list(self._env_vars), "strict": self._strict}
 
     @staticmethod
-    def _from_dict(dict: Dict[str, Any]) -> "Secret":
-        return EnvVarSecret(tuple(dict["env_vars"]), _strict=dict["strict"])
+    def _from_dict(dictionary: Dict[str, Any]) -> "Secret":
+        return EnvVarSecret(tuple(dictionary["env_vars"]), _strict=dictionary["strict"])
 
     def resolve_value(self) -> Optional[Any]:
+        """Resolve the secret to an atomic value. The semantics of the value is secret-dependent."""
         out = None
         for env_var in self._env_vars:
             value = os.getenv(env_var)
             if value is not None:
                 out = value
                 break
         if out is None and self._strict:
             raise ValueError(f"None of the following authentication environment variables are set: {self._env_vars}")
         return out
 
     @property
     def type(self) -> SecretType:
+        """The type of the secret."""
         return self._type
 
 
 def deserialize_secrets_inplace(data: Dict[str, Any], keys: Iterable[str], *, recursive: bool = False):
     """
     Deserialize secrets in a dictionary inplace.
```

### Comparing `haystack_ai-2.0.1rc2/haystack/utils/callable_serialization.py` & `haystack_ai-2.1.0rc1/haystack/utils/callable_serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from haystack import DeserializationError
 
 
 def serialize_callable(callable_handle: Callable) -> str:
     """
     Serializes a callable to its full path.
+
     :param callable_handle: The callable to serialize
     :return: The full path of the callable
     """
     module = inspect.getmodule(callable_handle)
 
     # Get the full package path of the function
     if module is not None:
@@ -20,14 +21,15 @@
         full_path = callable_handle.__name__
     return full_path
 
 
 def deserialize_callable(callable_handle: str) -> Optional[Callable]:
     """
     Deserializes a callable given its full import path as a string.
+
     :param callable_handle: The full path of the callable_handle
     :return: The callable
     :raises DeserializationError: If the callable cannot be found
     """
     parts = callable_handle.split(".")
     module_name = ".".join(parts[:-1])
     function_name = parts[-1]
```

### Comparing `haystack_ai-2.0.1rc2/haystack/utils/device.py` & `haystack_ai-2.1.0rc1/haystack/utils/device.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,18 +12,18 @@
     message="PyTorch must be installed to use torch.device or use GPU support in HuggingFace transformers. Run 'pip install transformers[torch]'"
 ) as torch_import:
     import torch
 
 
 class DeviceType(Enum):
     """
-    Represents device types supported by Haystack. This also includes
-    devices that are not directly used by models - for example, the disk
-    device is exclusively used in device maps for frameworks that support
-    offloading model weights to disk.
+    Represents device types supported by Haystack.
+
+    This also includes devices that are not directly used by models - for example, the disk device is exclusively used
+    in device maps for frameworks that support offloading model weights to disk.
     """
 
     CPU = "cpu"
     GPU = "cuda"
     DISK = "disk"
     MPS = "mps"
 
@@ -36,19 +36,19 @@
         Create a device type from a string.
 
         :param string:
             The string to convert.
         :returns:
             The device type.
         """
-        map = {e.value: e for e in DeviceType}
-        type = map.get(string)
-        if type is None:
+        mapping = {e.value: e for e in DeviceType}
+        _type = mapping.get(string)
+        if _type is None:
             raise ValueError(f"Unknown device type string '{string}'")
-        return type
+        return _type
 
 
 @dataclass
 class Device:
     """
     A generic representation of a device.
 
@@ -57,15 +57,15 @@
     :param id:
         The optional device id.
     """
 
     type: DeviceType
     id: Optional[int] = field(default=None)
 
-    def __init__(self, type: DeviceType, id: Optional[int] = None):
+    def __init__(self, type: DeviceType, id: Optional[int] = None):  # noqa:A002
         """
         Create a generic device.
 
         :param type:
             The device type.
         :param id:
             The device id.
@@ -89,15 +89,15 @@
 
         :returns:
             The CPU device.
         """
         return Device(DeviceType.CPU)
 
     @staticmethod
-    def gpu(id: int = 0) -> "Device":
+    def gpu(id: int = 0) -> "Device":  # noqa:A002
         """
         Create a generic GPU device.
 
         :param id:
             The GPU id.
         :returns:
             The GPU device.
@@ -122,24 +122,32 @@
         :returns:
             The MPS device.
         """
         return Device(DeviceType.MPS)
 
     @staticmethod
     def from_str(string: str) -> "Device":
+        """
+        Create a generic device from a string.
+
+        :returns:
+            The device.
+
+        """
         device_type_str, device_id = _split_device_string(string)
         return Device(DeviceType.from_str(device_type_str), device_id)
 
 
 @dataclass
 class DeviceMap:
     """
-    A generic mapping from strings to devices. The semantics of the
-    strings are dependent on target framework. Primarily used to deploy
-    HuggingFace models to multiple devices.
+    A generic mapping from strings to devices.
+
+    The semantics of the strings are dependent on target framework. Primarily used to deploy HuggingFace models to
+    multiple devices.
 
     :param mapping:
         Dictionary mapping strings to devices.
     """
 
     mapping: Dict[str, Device] = field(default_factory=dict, hash=False)
 
@@ -177,15 +185,15 @@
         """
         if not self.mapping:
             return None
         else:
             return next(iter(self.mapping.values()))
 
     @staticmethod
-    def from_dict(dict: Dict[str, str]) -> "DeviceMap":
+    def from_dict(dict: Dict[str, str]) -> "DeviceMap":  # noqa:A002
         """
         Create a generic device map from a JSON-serialized dictionary.
 
         :param dict:
             The serialized mapping.
         :returns:
             The generic device map.
@@ -222,39 +230,42 @@
                 )
         return DeviceMap(mapping)
 
 
 @dataclass(frozen=True)
 class ComponentDevice:
     """
-    A representation of a device for a component. This can be either
-    a single device or a device map.
+    A representation of a device for a component.
+
+    This can be either a single device or a device map.
     """
 
     _single_device: Optional[Device] = field(default=None)
     _multiple_devices: Optional[DeviceMap] = field(default=None)
 
     @classmethod
     def from_str(cls, device_str: str) -> "ComponentDevice":
         """
         Create a component device representation from a device string.
+
         The device string can only represent a single device.
 
         :param device_str:
             The device string.
         :returns:
             The component device representation.
         """
         device = Device.from_str(device_str)
         return cls.from_single(device)
 
     @classmethod
     def from_single(cls, device: Device) -> "ComponentDevice":
         """
         Create a component device representation from a single device.
+
         Disks cannot be used as single devices.
 
         :param device:
             The device.
         :returns:
             The component device representation.
         """
@@ -283,14 +294,15 @@
             raise ValueError(
                 "The component device can neither be empty nor contain both a single device and a device map"
             )
 
     def to_torch(self) -> "torch.device":
         """
         Convert the component device representation to PyTorch format.
+
         Device maps are not supported.
 
         :returns:
             The PyTorch device representation.
         """
         self._validate()
 
@@ -300,14 +312,15 @@
         torch_import.check()
         assert self._single_device is not None
         return torch.device(str(self._single_device))
 
     def to_torch_str(self) -> str:
         """
         Convert the component device representation to PyTorch string format.
+
         Device maps are not supported.
 
         :returns:
             The PyTorch device string representation.
         """
         self._validate()
 
@@ -316,14 +329,15 @@
 
         assert self._single_device is not None
         return str(self._single_device)
 
     def to_spacy(self) -> int:
         """
         Convert the component device representation to spaCy format.
+
         Device maps are not supported.
 
         :returns:
             The spaCy device representation.
         """
         self._validate()
 
@@ -357,17 +371,17 @@
             return convert_device(self._single_device)
 
         assert self._multiple_devices is not None
         return {key: convert_device(device, gpu_id_only=True) for key, device in self._multiple_devices.mapping.items()}
 
     def update_hf_kwargs(self, hf_kwargs: Dict[str, Any], *, overwrite: bool) -> Dict[str, Any]:
         """
-        Convert the component device representation to HuggingFace format
-        and add them as canonical keyword arguments to the keyword arguments
-        dictionary.
+        Convert the component device representation to HuggingFace format.
+
+        Add them as canonical keyword arguments to the keyword arguments dictionary.
 
         :param hf_kwargs:
             The HuggingFace keyword arguments dictionary.
         :param overwrite:
             Whether to overwrite existing device arguments.
         :returns:
             The HuggingFace keyword arguments dictionary.
@@ -381,26 +395,24 @@
         key = "device_map" if self.has_multiple_devices else "device"
         hf_kwargs[key] = converted
         return hf_kwargs
 
     @property
     def has_multiple_devices(self) -> bool:
         """
-        Whether this component device representation contains multiple
-        devices.
+        Whether this component device representation contains multiple devices.
         """
         self._validate()
 
         return self._multiple_devices is not None
 
     @property
     def first_device(self) -> Optional["ComponentDevice"]:
         """
-        Return either the single device or the first device in the
-        device map, if any.
+        Return either the single device or the first device in the device map, if any.
 
         :returns:
             The first device.
         """
         self._validate()
 
         if self._single_device is not None:
@@ -409,16 +421,15 @@
         assert self._multiple_devices is not None
         assert self._multiple_devices.first_device is not None
         return self.from_single(self._multiple_devices.first_device)
 
     @staticmethod
     def resolve_device(device: Optional["ComponentDevice"] = None) -> "ComponentDevice":
         """
-        Select a device for a component. If a device is specified,
-        it's used. Otherwise, the default device is used.
+        Select a device for a component. If a device is specified, it's used. Otherwise, the default device is used.
 
         :param device:
             The provided device, if any.
         :returns:
             The resolved device.
         """
         if not isinstance(device, ComponentDevice) and device is not None:
@@ -429,33 +440,31 @@
         if device is None:
             device = ComponentDevice.from_single(_get_default_device())
 
         return device
 
     def to_dict(self) -> Dict[str, Any]:
         """
-        Convert the component device representation to a JSON-serializable
-        dictionary.
+        Convert the component device representation to a JSON-serializable dictionary.
 
         :returns:
             The dictionary representation.
         """
         if self._single_device is not None:
             return {"type": "single", "device": str(self._single_device)}
         elif self._multiple_devices is not None:
             return {"type": "multiple", "device_map": self._multiple_devices.to_dict()}
         else:
             # Unreachable
             assert False
 
     @classmethod
-    def from_dict(cls, dict: Dict[str, Any]) -> "ComponentDevice":
+    def from_dict(cls, dict: Dict[str, Any]) -> "ComponentDevice":  # noqa:A002
         """
-        Create a component device representation from a JSON-serialized
-        dictionary.
+        Create a component device representation from a JSON-serialized dictionary.
 
         :param dict:
             The serialized representation.
         :returns:
             The deserialized component device.
         """
         if dict["type"] == "single":
@@ -464,17 +473,18 @@
             return cls.from_multiple(DeviceMap.from_dict(dict["device_map"]))
         else:
             raise ValueError(f"Unknown component device type '{dict['type']}' in serialized data")
 
 
 def _get_default_device() -> Device:
     """
-    Return the default device for Haystack. Precedence:
-    GPU > MPS > CPU. If PyTorch is not installed, only CPU
-    is available.
+    Return the default device for Haystack.
+
+    Precedence:
+        GPU > MPS > CPU. If PyTorch is not installed, only CPU is available.
 
     :returns:
         The default device.
     """
     try:
         torch_import.check()
```

### Comparing `haystack_ai-2.0.1rc2/haystack/utils/filters.py` & `haystack_ai-2.1.0rc1/haystack/utils/filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,14 +172,15 @@
     filter_value: Any = condition["value"]
     return COMPARISON_OPERATORS[operator](filter_value=filter_value, document_value=document_value)
 
 
 def convert(filters: Dict[str, Any]) -> Dict[str, Any]:
     """
     Convert a filter declared using the legacy style into the new style.
+
     This is mostly meant to ease migration from Haystack 1.x to 2.x for developers
     of Document Stores and Components that use filters.
 
     This function doesn't verify if `filters` are declared using the legacy style.
 
     Example usage:
     ```python
```

### Comparing `haystack_ai-2.0.1rc2/haystack/utils/hf.py` & `haystack_ai-2.1.0rc1/haystack/utils/hf.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,23 +17,89 @@
 with LazyImport(message="Run 'pip install \"huggingface_hub>=0.22.0\"'") as huggingface_hub_import:
     from huggingface_hub import HfApi, InferenceClient, model_info
     from huggingface_hub.utils import RepositoryNotFoundError
 
 logger = logging.getLogger(__name__)
 
 
+class HFGenerationAPIType(Enum):
+    """
+    API type to use for Hugging Face API Generators.
+    """
+
+    # HF [Text Generation Inference (TGI)](https://github.com/huggingface/text-generation-inference).
+    TEXT_GENERATION_INFERENCE = "text_generation_inference"
+
+    # HF [Inference Endpoints](https://huggingface.co/inference-endpoints).
+    INFERENCE_ENDPOINTS = "inference_endpoints"
+
+    # HF [Serverless Inference API](https://huggingface.co/inference-api).
+    SERVERLESS_INFERENCE_API = "serverless_inference_api"
+
+    def __str__(self):
+        return self.value
+
+    @staticmethod
+    def from_str(string: str) -> "HFGenerationAPIType":
+        """
+        Convert a string to a HFGenerationAPIType enum.
+
+        :param string: The string to convert.
+        :return: The corresponding HFGenerationAPIType enum.
+
+        """
+        enum_map = {e.value: e for e in HFGenerationAPIType}
+        mode = enum_map.get(string)
+        if mode is None:
+            msg = f"Unknown Hugging Face API type '{string}'. Supported types are: {list(enum_map.keys())}"
+            raise ValueError(msg)
+        return mode
+
+
+class HFEmbeddingAPIType(Enum):
+    """
+    API type to use for Hugging Face API Embedders.
+    """
+
+    # HF [Text Embeddings Inference (TEI)](https://github.com/huggingface/text-embeddings-inference).
+    TEXT_EMBEDDINGS_INFERENCE = "text_embeddings_inference"
+
+    # HF [Inference Endpoints](https://huggingface.co/inference-endpoints).
+    INFERENCE_ENDPOINTS = "inference_endpoints"
+
+    # HF [Serverless Inference API](https://huggingface.co/inference-api).
+    SERVERLESS_INFERENCE_API = "serverless_inference_api"
+
+    def __str__(self):
+        return self.value
+
+    @staticmethod
+    def from_str(string: str) -> "HFEmbeddingAPIType":
+        """
+        Convert a string to a HFEmbeddingAPIType enum.
+
+        :param string:
+        :return: The corresponding HFEmbeddingAPIType enum.
+        """
+        enum_map = {e.value: e for e in HFEmbeddingAPIType}
+        mode = enum_map.get(string)
+        if mode is None:
+            msg = f"Unknown Hugging Face API type '{string}'. Supported types are: {list(enum_map.keys())}"
+            raise ValueError(msg)
+        return mode
+
+
 class HFModelType(Enum):
     EMBEDDING = 1
     GENERATION = 2
 
 
 def serialize_hf_model_kwargs(kwargs: Dict[str, Any]):
     """
-    Recursively serialize HuggingFace specific model keyword arguments
-    in-place to make them JSON serializable.
+    Recursively serialize HuggingFace specific model keyword arguments in-place to make them JSON serializable.
 
     :param kwargs: The keyword arguments to serialize
     """
     torch_import.check()
 
     for k, v in kwargs.items():
         # torch.dtype
@@ -42,16 +108,15 @@
 
         if isinstance(v, dict):
             serialize_hf_model_kwargs(v)
 
 
 def deserialize_hf_model_kwargs(kwargs: Dict[str, Any]):
     """
-    Recursively deserialize HuggingFace specific model keyword arguments
-    in-place to make them JSON serializable.
+    Recursively deserialize HuggingFace specific model keyword arguments in-place to make them JSON serializable.
 
     :param kwargs: The keyword arguments to deserialize
     """
     torch_import.check()
 
     for k, v in kwargs.items():
         # torch.dtype
@@ -63,17 +128,18 @@
 
         if isinstance(v, dict):
             deserialize_hf_model_kwargs(v)
 
 
 def resolve_hf_device_map(device: Optional[ComponentDevice], model_kwargs: Optional[Dict[str, Any]]) -> Dict[str, Any]:
     """
-    Update `model_kwargs` to include the keyword argument `device_map` based on `device` if `device_map` is not
-    already present in `model_kwargs`. This method is useful you want to force loading a transformers model when using
-    `AutoModel.from_pretrained` to use `device_map`.
+    Update `model_kwargs` to include the keyword argument `device_map` based on `device` if `device_map` is not already present in `model_kwargs`.
+
+    This method is useful you want to force loading a transformers model when using `AutoModel.from_pretrained` to
+    use `device_map`.
 
     We handle the edge case where `device` and `device_map` is specified by ignoring the `device` parameter and printing
     a warning.
 
     :param device: The device on which the model is loaded. If `None`, the default device is automatically
         selected.
     :param model_kwargs: Additional HF keyword arguments passed to `AutoModel.from_pretrained`.
@@ -94,14 +160,58 @@
     # Set up device_map which allows quantized loading and multi device inference
     # requires accelerate which is always installed when using `pip install transformers[torch]`
     model_kwargs["device_map"] = device_map
 
     return model_kwargs
 
 
+def resolve_hf_pipeline_kwargs(
+    huggingface_pipeline_kwargs: Dict[str, Any],
+    model: str,
+    task: Optional[str],
+    supported_tasks: List[str],
+    device: Optional[ComponentDevice],
+    token: Optional[Secret],
+) -> Dict[str, Any]:
+    """
+    Resolve the HuggingFace pipeline keyword arguments based on explicit user inputs.
+
+    :param huggingface_pipeline_kwargs: Dictionary containing keyword arguments used to initialize a
+        Hugging Face pipeline.
+    :param model: The name or path of a Hugging Face model for on the HuggingFace Hub.
+    :param task: The task for the Hugging Face pipeline.
+    :param supported_tasks: The list of supported tasks to check the task of the model against. If the task of the model
+        is not present within this list then a ValueError is thrown.
+    :param device: The device on which the model is loaded. If `None`, the default device is automatically
+        selected. If a device/device map is specified in `huggingface_pipeline_kwargs`, it overrides this parameter.
+    :param token: The token to use as HTTP bearer authorization for remote files.
+        If the token is also specified in the `huggingface_pipeline_kwargs`, this parameter will be ignored.
+    """
+    huggingface_hub_import.check()
+
+    token = token.resolve_value() if token else None
+    # check if the huggingface_pipeline_kwargs contain the essential parameters
+    # otherwise, populate them with values from other init parameters
+    huggingface_pipeline_kwargs.setdefault("model", model)
+    huggingface_pipeline_kwargs.setdefault("token", token)
+
+    device = ComponentDevice.resolve_device(device)
+    device.update_hf_kwargs(huggingface_pipeline_kwargs, overwrite=False)
+
+    # task identification and validation
+    task = task or huggingface_pipeline_kwargs.get("task")
+    if task is None and isinstance(huggingface_pipeline_kwargs["model"], str):
+        task = model_info(huggingface_pipeline_kwargs["model"], token=huggingface_pipeline_kwargs["token"]).pipeline_tag
+
+    if task not in supported_tasks:
+        raise ValueError(f"Task '{task}' is not supported. " f"The supported tasks are: {', '.join(supported_tasks)}.")
+    huggingface_pipeline_kwargs["task"] = task
+    return huggingface_pipeline_kwargs
+
+
 def list_inference_deployed_models(headers: Optional[Dict] = None) -> List[str]:
     """
     List all currently deployed models on HF TGI free tier
 
     :param headers: Optional dictionary of headers to include in the request
     :return: list of all currently deployed models
     :raises Exception: If the request to the TGI API fails
@@ -118,14 +228,15 @@
         raise Exception(f"Failed to fetch TGI deployed models: {message}. Error type: {error_type}")
     return [model["model_id"] for model in payload]
 
 
 def check_valid_model(model_id: str, model_type: HFModelType, token: Optional[Secret]) -> None:
     """
     Check if the provided model ID corresponds to a valid model on HuggingFace Hub.
+
     Also check if the model is an embedding or generation model.
 
     :param model_id: A string representing the HuggingFace model ID.
     :param model_type: the model type, HFModelType.EMBEDDING or HFModelType.GENERATION
     :param token: The optional authentication token.
     :raises ValueError: If the model is not found or is not a embedding model.
     """
@@ -174,16 +285,16 @@
                 f"Unknown text generation parameters: {unknown_params}. The valid parameters are: {accepted_params}."
             )
 
 
 with LazyImport(message="Run 'pip install transformers[torch]'") as transformers_import:
     from transformers import PreTrainedTokenizer, PreTrainedTokenizerFast, StoppingCriteria, TextStreamer
 
-    transformers_import.check()
     torch_import.check()
+    transformers_import.check()
 
     class StopWordsCriteria(StoppingCriteria):
         """
         Stops text generation in HuggingFace generators if any one of the stop words is generated.
 
         Note: When a stop word is encountered, the generation of new text is stopped.
         However, if the stop word is in the prompt itself, it can stop generating new text
@@ -211,21 +322,28 @@
                     tokenizer.pad_token = tokenizer.eos_token
                 else:
                     tokenizer.add_special_tokens({"pad_token": "[PAD]"})
             encoded_stop_words = tokenizer(stop_words, add_special_tokens=False, padding=True, return_tensors="pt")
             self.stop_ids = encoded_stop_words.input_ids.to(device)
 
         def __call__(self, input_ids: torch.LongTensor, scores: torch.FloatTensor, **kwargs) -> bool:
+            """Check if any of the stop words are generated in the current text generation step."""
             for stop_id in self.stop_ids:
                 found_stop_word = self.is_stop_word_found(input_ids, stop_id)
                 if found_stop_word:
                     return True
             return False
 
-        def is_stop_word_found(self, generated_text_ids: torch.Tensor, stop_id: torch.Tensor) -> bool:
+        @staticmethod
+        def is_stop_word_found(generated_text_ids: torch.Tensor, stop_id: torch.Tensor) -> bool:
+            """
+            Performs phrase matching.
+
+            Checks if a sequence of stop tokens appears in a continuous or sequential order within the generated text.
+            """
             generated_text_ids = generated_text_ids[-1]
             len_generated_text_ids = generated_text_ids.size(0)
             len_stop_id = stop_id.size(0)
             result = all(generated_text_ids[len_generated_text_ids - len_stop_id :].eq(stop_id))
             return result
 
     class HFTokenStreamingHandler(TextStreamer):
@@ -245,10 +363,11 @@
             stop_words: Optional[List[str]] = None,
         ):
             super().__init__(tokenizer=tokenizer, skip_prompt=True)  # type: ignore
             self.token_handler = stream_handler
             self.stop_words = stop_words or []
 
         def on_finalized_text(self, word: str, stream_end: bool = False):
+            """Callback function for handling the generated text."""
             word_to_send = word + "\n" if stream_end else word
             if word_to_send.strip() not in self.stop_words:
                 self.token_handler(StreamingChunk(content=word_to_send))
```

### Comparing `haystack_ai-2.0.1rc2/haystack/utils/jupyter.py` & `haystack_ai-2.1.0rc1/haystack/utils/jupyter.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/utils/requests_utils.py` & `haystack_ai-2.1.0rc1/haystack/utils/requests_utils.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/haystack/utils/type_serialization.py` & `haystack_ai-2.1.0rc1/haystack/utils/type_serialization.py`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/.gitignore` & `haystack_ai-2.1.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/LICENSE` & `haystack_ai-2.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `haystack_ai-2.0.1rc2/README.md` & `haystack_ai-2.1.0rc1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <div align="center">
-  <a href="https://www.deepset.ai/haystack/"><img src="https://github.com/deepset-ai/haystack/blob/main/docs/img/banner_20.png" alt="Haystack"></a>
+  <a href="https://haystack.deepset.ai/"><img src="https://github.com/deepset-ai/haystack/blob/main/docs/img/banner_20.png" alt="Green logo of a stylized white 'H' with the text 'Haystack, by deepset. Haystack 2.0 is live 🎉' Abstract green and yellow diagrams in the background."></a>
 
-|         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
-| ------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| CI/CD   | [![Tests](https://github.com/deepset-ai/haystack/actions/workflows/tests.yml/badge.svg)](https://github.com/deepset-ai/haystack/actions/workflows/tests.yml) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![Coverage Status](https://coveralls.io/repos/github/deepset-ai/haystack/badge.svg?branch=main)](https://coveralls.io/github/deepset-ai/haystack?branch=main)                                                        |
-| Docs    | [![Website](https://img.shields.io/website?label=documentation&up_message=online&url=https%3A%2F%2Fdocs.haystack.deepset.ai)](https://docs.haystack.deepset.ai)                                                                                                                                                                                                                                                                                                                                                                                                                                          |
-| Package | [![PyPI](https://img.shields.io/pypi/v/haystack-ai)](https://pypi.org/project/haystack-ai/) ![PyPI - Downloads](https://img.shields.io/pypi/dm/haystack-ai?color=blue&logo=pypi&logoColor=gold) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/farm-haystack?logo=python&logoColor=gold) [![GitHub](https://img.shields.io/github/license/deepset-ai/haystack?color=blue)](LICENSE) [![License Compliance](https://github.com/deepset-ai/haystack/actions/workflows/license_compliance.yml/badge.svg)](https://github.com/deepset-ai/haystack/actions/workflows/license_compliance.yml) |
-| Meta    | [![Discord](https://img.shields.io/discord/993534733298450452?logo=discord)](https://discord.gg/haystack) [![Twitter Follow](https://img.shields.io/twitter/follow/haystack_ai)](https://twitter.com/haystack_ai)                                                                                                                                                                                                                                                                                                                                                                                        |
+|         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
+| ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
+| CI/CD   | [![Tests](https://github.com/deepset-ai/haystack/actions/workflows/tests.yml/badge.svg)](https://github.com/deepset-ai/haystack/actions/workflows/tests.yml) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![Coverage Status](https://coveralls.io/repos/github/deepset-ai/haystack/badge.svg?branch=main)](https://coveralls.io/github/deepset-ai/haystack?branch=main)                                                                                                                                                                                    |
+| Docs    | [![Website](https://img.shields.io/website?label=documentation&up_message=online&url=https%3A%2F%2Fdocs.haystack.deepset.ai)](https://docs.haystack.deepset.ai)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
+| Package | [![PyPI](https://img.shields.io/pypi/v/haystack-ai)](https://pypi.org/project/haystack-ai/) ![PyPI - Downloads](https://img.shields.io/pypi/dm/haystack-ai?color=blue&logo=pypi&logoColor=gold) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/haystack-ai?logo=python&logoColor=gold) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/haystack-ai.svg)](https://anaconda.org/conda-forge/haystack-ai) [![GitHub](https://img.shields.io/github/license/deepset-ai/haystack?color=blue)](LICENSE) [![License Compliance](https://github.com/deepset-ai/haystack/actions/workflows/license_compliance.yml/badge.svg)](https://github.com/deepset-ai/haystack/actions/workflows/license_compliance.yml) |
+| Meta    | [![Discord](https://img.shields.io/discord/993534733298450452?logo=discord)](https://discord.gg/haystack) [![Twitter Follow](https://img.shields.io/twitter/follow/haystack_ai)](https://twitter.com/haystack_ai)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
 </div>
 
 [Haystack](https://haystack.deepset.ai/) is an end-to-end LLM framework that allows you to build applications powered by
 LLMs, Transformer models, vector search and more. Whether you want to perform retrieval-augmented generation (RAG),
 document search, question answering or answer generation, Haystack can orchestrate state-of-the-art embedding models
 and LLMs into pipelines to build end-to-end NLP applications and solve your use case.
```

#### html2text {}

```diff
@@ -1,36 +1,42 @@
-_[_H_a_y_s_t_a_c_k_]| | | | ------- | ---------------------------------------------------
+   _[_G_r_e_e_n_ _l_o_g_o_ _o_f_ _a_ _s_t_y_l_i_z_e_d_ _w_h_i_t_e_ _'_H_'_ _w_i_t_h_ _t_h_e_ _t_e_x_t_ _'_H_a_y_s_t_a_c_k_,_ _b_y_ _d_e_e_p_s_e_t_.
+     _H_a_y_s_t_a_c_k_ _2_._0_ _i_s_ _l_i_v_e_ _ð____'_Â_ _A_b_s_t_r_a_c_t_ _g_r_e_e_n_ _a_n_d_ _y_e_l_l_o_w_ _d_i_a_g_r_a_m_s_ _i_n_ _t_h_e
+_b_a_c_k_g_r_o_u_n_d_._]| | | | ------- | -------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-  ----------------------------------------------------------- | | CI/CD | [!
-  [Tests](https://github.com/deepset-ai/haystack/actions/workflows/tests.yml/
-badge.svg)](https://github.com/deepset-ai/haystack/actions/workflows/tests.yml)
-    [![code style - Black](https://img.shields.io/badge/code%20style-black-
-     000000.svg)](https://github.com/psf/black) [![types - Mypy](https://
- img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [!
-   [Coverage Status](https://coveralls.io/repos/github/deepset-ai/haystack/
-        badge.svg?branch=main)](https://coveralls.io/github/deepset-ai/
-     haystack?branch=main) | | Docs | [![Website](https://img.shields.io/
+-------------------------------------------------------------------------------
+-------------------------------------------------------------------------------
+ --------------------------- | | CI/CD | [![Tests](https://github.com/deepset-
+ai/haystack/actions/workflows/tests.yml/badge.svg)](https://github.com/deepset-
+   ai/haystack/actions/workflows/tests.yml) [![code style - Black](https://
+ img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
+  black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)]
+  (https://github.com/python/mypy) [![Coverage Status](https://coveralls.io/
+repos/github/deepset-ai/haystack/badge.svg?branch=main)](https://coveralls.io/
+    github/deepset-ai/haystack?branch=main) | | Docs | [![Website](https://
+                                img.shields.io/
 website?label=documentation&up_message=online&url=https%3A%2F%2Fdocs.haystack.deepset.ai)]
       (https://docs.haystack.deepset.ai) | | Package | [![PyPI](https://
  img.shields.io/pypi/v/haystack-ai)](https://pypi.org/project/haystack-ai/) !
           [PyPI - Downloads](https://img.shields.io/pypi/dm/haystack-
    ai?color=blue&logo=pypi&logoColor=gold) ![PyPI - Python Version](https://
-  img.shields.io/pypi/pyversions/farm-haystack?logo=python&logoColor=gold) [!
-[GitHub](https://img.shields.io/github/license/deepset-ai/haystack?color=blue)]
-   (LICENSE) [![License Compliance](https://github.com/deepset-ai/haystack/
-   actions/workflows/license_compliance.yml/badge.svg)](https://github.com/
-  deepset-ai/haystack/actions/workflows/license_compliance.yml) | | Meta | [!
-  [Discord](https://img.shields.io/discord/993534733298450452?logo=discord)]
-   (https://discord.gg/haystack) [![Twitter Follow](https://img.shields.io/
-        twitter/follow/haystack_ai)](https://twitter.com/haystack_ai) |
+img.shields.io/pypi/pyversions/haystack-ai?logo=python&logoColor=gold) [![Conda
+Version](https://img.shields.io/conda/vn/conda-forge/haystack-ai.svg)](https://
+anaconda.org/conda-forge/haystack-ai) [![GitHub](https://img.shields.io/github/
+license/deepset-ai/haystack?color=blue)](LICENSE) [![License Compliance](https:
+  //github.com/deepset-ai/haystack/actions/workflows/license_compliance.yml/
+     badge.svg)](https://github.com/deepset-ai/haystack/actions/workflows/
+license_compliance.yml) | | Meta | [![Discord](https://img.shields.io/discord/
+   993534733298450452?logo=discord)](https://discord.gg/haystack) [![Twitter
+     Follow](https://img.shields.io/twitter/follow/haystack_ai)](https://
+                          twitter.com/haystack_ai) |
 [Haystack](https://haystack.deepset.ai/) is an end-to-end LLM framework that
 allows you to build applications powered by LLMs, Transformer models, vector
 search and more. Whether you want to perform retrieval-augmented generation
 (RAG), document search, question answering or answer generation, Haystack can
 orchestrate state-of-the-art embedding models and LLMs into pipelines to build
 end-to-end NLP applications and solve your use case. ## Installation The
 simplest way to get Haystack is via pip: ```sh pip install haystack-ai ```
```

### Comparing `haystack_ai-2.0.1rc2/pyproject.toml` & `haystack_ai-2.1.0rc1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -105,14 +105,15 @@
   "huggingface_hub>=0.22.0", # TGI Generators and TEI Embedders
   "spacy>=3.7,<3.8",  # NamedEntityExtractor
   "spacy-curated-transformers>=0.2,<=0.3",  # NamedEntityExtractor
   "en-core-web-trf @ https://github.com/explosion/spacy-models/releases/download/en_core_web_trf-3.7.3/en_core_web_trf-3.7.3-py3-none-any.whl",  # NamedEntityExtractor
 
   # Converters
   "pypdf",  # PyPDFConverter
+  "pdfminer.six", # PDFMinerToDocument
   "markdown-it-py",  # MarkdownToDocument
   "mdit_plain",  # MarkdownToDocument
   "tika",  # TikaDocumentConverter
   "azure-ai-formrecognizer>=3.2.0b2",  # AzureOCRDocumentConverter
   "langdetect",  # TextLanguageRouter and DocumentLanguageClassifier
   "sentence-transformers>=2.2.0",  # SentenceTransformersTextEmbedder and SentenceTransformersDocumentEmbedder
   "openai-whisper>=20231106",  # LocalWhisperTranscriber
@@ -135,26 +136,26 @@
   # Looking for missing imports
   "isort",
   "pyproject-parser",
 ]
 
 [tool.hatch.envs.test.scripts]
 e2e = "pytest e2e"
-unit = 'pytest --cov-report xml:coverage.xml --cov="haystack" -m "not integration" test'
-integration = 'pytest --maxfail=5 -m "integration" test'
-integration-mac = 'pytest --maxfail=5 -m "integration" test -k "not tika"'
-integration-windows = 'pytest --maxfail=5 -m "integration" test -k "not tika"'
+unit = 'pytest --cov-report xml:coverage.xml --cov="haystack" -m "not integration" {args:test}'
+integration = 'pytest --maxfail=5 -m "integration" {args:test}'
+integration-mac = 'pytest --maxfail=5 -m "integration" -k "not tika" {args:test}'
+integration-windows = 'pytest --maxfail=5 -m "integration" -k "not tika" {args:test}'
 types = "mypy --install-types --non-interactive --cache-dir=.mypy_cache/ {args:haystack}"
 lint = [
-  "ruff {args:haystack}",
+  "ruff check {args:haystack}",
   "pylint -ry -j 0 {args:haystack}"
 ]
 lint-fix = [
   "black .",
-  "ruff {args:haystack} --fix",
+  "ruff check {args:haystack} --fix",
 ]
 
 [tool.hatch.envs.readme]
 detached = true  # To avoid installing the dependencies from the default environment
 dependencies = [
   "haystack-pydoc-tools",
 ]
@@ -197,15 +198,15 @@
 [tool.black]
 line-length = 120
 skip_magic_trailing_comma = true  # For compatibility with pydoc>=4.6, check if still needed.
 
 [tool.codespell]
 ignore-words-list = "ans,astroid,nd,ned,nin,ue,rouge,ist"
 quiet-level = 3
-skip = "test/nodes/*,test/others/*,test/samples/*"
+skip = "test/nodes/*,test/others/*,test/samples/*,e2e/*"
 
 [tool.pylint.'MESSAGES CONTROL']
 max-line-length=120
 disable = [
 
   # To keep
   "fixme",
@@ -290,44 +291,49 @@
 
 [tool.mypy]
 warn_return_any = false
 warn_unused_configs = true
 ignore_missing_imports = true
 
 [tool.ruff]
-line-length = 1486
+line-length = 301
 target-version = "py38"
+exclude= ["test"]
+
 
 [tool.ruff.lint]
 select = [
-  "AIR",    # Airflow
   "ASYNC",  # flake8-async
   "C4",     # flake8-comprehensions
   "C90",    # McCabe cyclomatic complexity
-  "CPY",    # flake8-copyright
-  "DJ",     # flake8-django
   "E501",   # Long lines
   "EXE",    # flake8-executable
   "F",      # Pyflakes
-  "FURB",   # refurb
   "INT",    # flake8-gettext
   "PERF",   # Perflint
   "PL",     # Pylint
   "Q",      # flake8-quotes
   "SIM",    # flake8-simplify
   "SLOT",   # flake8-slots
   "T10",    # flake8-debugger
   "W",      # pycodestyle
   "YTT",    # flake8-2020
-  "I"       # isort
-  # "E",    # pycodestyle
-  # "NPY",  # NumPy-specific rules
-  # "PD",   # pandas-vet
-  # "PT",   # flake8-pytest-style
-  # "UP",   # pyupgrade
+  "I",       # isort
+  # built-in shadowing
+  "A001",	# builtin-variable-shadowing
+  "A002",	# builtin-argument-shadowing
+  "A003",	# builtin-attribute-shadowing
+  # docstring rules
+  "D102",   # Missing docstring in public method
+  "D103",   # Missing docstring in public function
+  "D209",   # Closing triple quotes go to new line
+  "D205",   # 1 blank line required between summary line and description
+  "D213",   # summary lines must be positioned on the second physical line of the docstring
+  "D417",   # undocumented-parameter
+  "D419",   # undocumented-returns
 ]
 
 ignore = [
   "F401",     # unused-import
   "PERF203",	# `try`-`except` within a loop incurs performance overhead
   "PERF401",	# Use a list comprehension to create a transformed list
   "PLR1714",  # repeated-equality-comparison
@@ -346,17 +352,17 @@
 [tool.ruff.lint.per-file-ignores]
 "examples/basic_qa_pipeline.py" = ["C416"]
 "haystack/preview/testing/document_store.py" = ["C416", "F821"]
 "haystack/telemetry.py" = ["F821"]
 
 [tool.ruff.lint.pylint]
 allow-magic-value-types = ["float", "int", "str"]
-max-args = 38  # Default is 5
-max-branches = 32  # Default is 12
-max-public-methods = 90  # Default is 20
-max-returns = 9  # Default is 6
-max-statements = 105  # Default is 50
+max-args = 14  # Default is 5
+max-branches = 21  # Default is 12
+max-public-methods = 20  # Default is 20
+max-returns = 7  # Default is 6
+max-statements = 60  # Default is 50
 
 [tool.coverage.run]
 omit = [
     "haystack/testing/*",
 ]
```

### Comparing `haystack_ai-2.0.1rc2/PKG-INFO` & `haystack_ai-2.1.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: haystack-ai
-Version: 2.0.1rc2
+Version: 2.1.0rc1
 Summary: LLM framework to build customizable, production-ready LLM applications. Connect components (models, vector DBs, file converters) to pipelines or agents that can interact with your data.
 Project-URL: CI: GitHub, https://github.com/deepset-ai/haystack/actions
 Project-URL: Docs: RTD, https://haystack.deepset.ai/overview/intro
 Project-URL: GitHub: issues, https://github.com/deepset-ai/haystack/issues
 Project-URL: GitHub: repo, https://github.com/deepset-ai/haystack
 Project-URL: Homepage, https://github.com/deepset-ai/haystack
 Author-email: "deepset.ai" <malte.pietsch@deepset.ai>
@@ -38,22 +38,22 @@
 Requires-Dist: requests
 Requires-Dist: tenacity
 Requires-Dist: tqdm
 Requires-Dist: typing-extensions>=4.7
 Description-Content-Type: text/markdown
 
 <div align="center">
-  <a href="https://www.deepset.ai/haystack/"><img src="https://github.com/deepset-ai/haystack/blob/main/docs/img/banner_20.png" alt="Haystack"></a>
+  <a href="https://haystack.deepset.ai/"><img src="https://github.com/deepset-ai/haystack/blob/main/docs/img/banner_20.png" alt="Green logo of a stylized white 'H' with the text 'Haystack, by deepset. Haystack 2.0 is live 🎉' Abstract green and yellow diagrams in the background."></a>
 
-|         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
-| ------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| CI/CD   | [![Tests](https://github.com/deepset-ai/haystack/actions/workflows/tests.yml/badge.svg)](https://github.com/deepset-ai/haystack/actions/workflows/tests.yml) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![Coverage Status](https://coveralls.io/repos/github/deepset-ai/haystack/badge.svg?branch=main)](https://coveralls.io/github/deepset-ai/haystack?branch=main)                                                        |
-| Docs    | [![Website](https://img.shields.io/website?label=documentation&up_message=online&url=https%3A%2F%2Fdocs.haystack.deepset.ai)](https://docs.haystack.deepset.ai)                                                                                                                                                                                                                                                                                                                                                                                                                                          |
-| Package | [![PyPI](https://img.shields.io/pypi/v/haystack-ai)](https://pypi.org/project/haystack-ai/) ![PyPI - Downloads](https://img.shields.io/pypi/dm/haystack-ai?color=blue&logo=pypi&logoColor=gold) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/farm-haystack?logo=python&logoColor=gold) [![GitHub](https://img.shields.io/github/license/deepset-ai/haystack?color=blue)](LICENSE) [![License Compliance](https://github.com/deepset-ai/haystack/actions/workflows/license_compliance.yml/badge.svg)](https://github.com/deepset-ai/haystack/actions/workflows/license_compliance.yml) |
-| Meta    | [![Discord](https://img.shields.io/discord/993534733298450452?logo=discord)](https://discord.gg/haystack) [![Twitter Follow](https://img.shields.io/twitter/follow/haystack_ai)](https://twitter.com/haystack_ai)                                                                                                                                                                                                                                                                                                                                                                                        |
+|         |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
+| ------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
+| CI/CD   | [![Tests](https://github.com/deepset-ai/haystack/actions/workflows/tests.yml/badge.svg)](https://github.com/deepset-ai/haystack/actions/workflows/tests.yml) [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![Coverage Status](https://coveralls.io/repos/github/deepset-ai/haystack/badge.svg?branch=main)](https://coveralls.io/github/deepset-ai/haystack?branch=main)                                                                                                                                                                                    |
+| Docs    | [![Website](https://img.shields.io/website?label=documentation&up_message=online&url=https%3A%2F%2Fdocs.haystack.deepset.ai)](https://docs.haystack.deepset.ai)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
+| Package | [![PyPI](https://img.shields.io/pypi/v/haystack-ai)](https://pypi.org/project/haystack-ai/) ![PyPI - Downloads](https://img.shields.io/pypi/dm/haystack-ai?color=blue&logo=pypi&logoColor=gold) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/haystack-ai?logo=python&logoColor=gold) [![Conda Version](https://img.shields.io/conda/vn/conda-forge/haystack-ai.svg)](https://anaconda.org/conda-forge/haystack-ai) [![GitHub](https://img.shields.io/github/license/deepset-ai/haystack?color=blue)](LICENSE) [![License Compliance](https://github.com/deepset-ai/haystack/actions/workflows/license_compliance.yml/badge.svg)](https://github.com/deepset-ai/haystack/actions/workflows/license_compliance.yml) |
+| Meta    | [![Discord](https://img.shields.io/discord/993534733298450452?logo=discord)](https://discord.gg/haystack) [![Twitter Follow](https://img.shields.io/twitter/follow/haystack_ai)](https://twitter.com/haystack_ai)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
 </div>
 
 [Haystack](https://haystack.deepset.ai/) is an end-to-end LLM framework that allows you to build applications powered by
 LLMs, Transformer models, vector search and more. Whether you want to perform retrieval-augmented generation (RAG),
 document search, question answering or answer generation, Haystack can orchestrate state-of-the-art embedding models
 and LLMs into pipelines to build end-to-end NLP applications and solve your use case.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: haystack-ai Version: 2.0.1rc2 Summary: LLM
+Metadata-Version: 2.3 Name: haystack-ai Version: 2.1.0rc1 Summary: LLM
 framework to build customizable, production-ready LLM applications. Connect
 components (models, vector DBs, file converters) to pipelines or agents that
 can interact with your data. Project-URL: CI: GitHub, https://github.com/
 deepset-ai/haystack/actions Project-URL: Docs: RTD, https://
 haystack.deepset.ai/overview/intro Project-URL: GitHub: issues, https://
 github.com/deepset-ai/haystack/issues Project-URL: GitHub: repo, https://
 github.com/deepset-ai/haystack Project-URL: Homepage, https://github.com/
@@ -20,43 +20,49 @@
 Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8
 Requires-Dist: boilerpy3 Requires-Dist: haystack-bm25 Requires-Dist: jinja2
 Requires-Dist: lazy-imports Requires-Dist: more-itertools Requires-Dist:
 networkx Requires-Dist: numpy Requires-Dist: openai>=1.1.0 Requires-Dist:
 pandas Requires-Dist: posthog Requires-Dist: python-dateutil Requires-Dist:
 pyyaml Requires-Dist: requests Requires-Dist: tenacity Requires-Dist: tqdm
 Requires-Dist: typing-extensions>=4.7 Description-Content-Type: text/markdown
-_[_H_a_y_s_t_a_c_k_]| | | | ------- | ---------------------------------------------------
+   _[_G_r_e_e_n_ _l_o_g_o_ _o_f_ _a_ _s_t_y_l_i_z_e_d_ _w_h_i_t_e_ _'_H_'_ _w_i_t_h_ _t_h_e_ _t_e_x_t_ _'_H_a_y_s_t_a_c_k_,_ _b_y_ _d_e_e_p_s_e_t_.
+     _H_a_y_s_t_a_c_k_ _2_._0_ _i_s_ _l_i_v_e_ _ð____'_Â_ _A_b_s_t_r_a_c_t_ _g_r_e_e_n_ _a_n_d_ _y_e_l_l_o_w_ _d_i_a_g_r_a_m_s_ _i_n_ _t_h_e
+_b_a_c_k_g_r_o_u_n_d_._]| | | | ------- | -------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
 -------------------------------------------------------------------------------
-  ----------------------------------------------------------- | | CI/CD | [!
-  [Tests](https://github.com/deepset-ai/haystack/actions/workflows/tests.yml/
-badge.svg)](https://github.com/deepset-ai/haystack/actions/workflows/tests.yml)
-    [![code style - Black](https://img.shields.io/badge/code%20style-black-
-     000000.svg)](https://github.com/psf/black) [![types - Mypy](https://
- img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [!
-   [Coverage Status](https://coveralls.io/repos/github/deepset-ai/haystack/
-        badge.svg?branch=main)](https://coveralls.io/github/deepset-ai/
-     haystack?branch=main) | | Docs | [![Website](https://img.shields.io/
+-------------------------------------------------------------------------------
+-------------------------------------------------------------------------------
+ --------------------------- | | CI/CD | [![Tests](https://github.com/deepset-
+ai/haystack/actions/workflows/tests.yml/badge.svg)](https://github.com/deepset-
+   ai/haystack/actions/workflows/tests.yml) [![code style - Black](https://
+ img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/
+  black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)]
+  (https://github.com/python/mypy) [![Coverage Status](https://coveralls.io/
+repos/github/deepset-ai/haystack/badge.svg?branch=main)](https://coveralls.io/
+    github/deepset-ai/haystack?branch=main) | | Docs | [![Website](https://
+                                img.shields.io/
 website?label=documentation&up_message=online&url=https%3A%2F%2Fdocs.haystack.deepset.ai)]
       (https://docs.haystack.deepset.ai) | | Package | [![PyPI](https://
  img.shields.io/pypi/v/haystack-ai)](https://pypi.org/project/haystack-ai/) !
           [PyPI - Downloads](https://img.shields.io/pypi/dm/haystack-
    ai?color=blue&logo=pypi&logoColor=gold) ![PyPI - Python Version](https://
-  img.shields.io/pypi/pyversions/farm-haystack?logo=python&logoColor=gold) [!
-[GitHub](https://img.shields.io/github/license/deepset-ai/haystack?color=blue)]
-   (LICENSE) [![License Compliance](https://github.com/deepset-ai/haystack/
-   actions/workflows/license_compliance.yml/badge.svg)](https://github.com/
-  deepset-ai/haystack/actions/workflows/license_compliance.yml) | | Meta | [!
-  [Discord](https://img.shields.io/discord/993534733298450452?logo=discord)]
-   (https://discord.gg/haystack) [![Twitter Follow](https://img.shields.io/
-        twitter/follow/haystack_ai)](https://twitter.com/haystack_ai) |
+img.shields.io/pypi/pyversions/haystack-ai?logo=python&logoColor=gold) [![Conda
+Version](https://img.shields.io/conda/vn/conda-forge/haystack-ai.svg)](https://
+anaconda.org/conda-forge/haystack-ai) [![GitHub](https://img.shields.io/github/
+license/deepset-ai/haystack?color=blue)](LICENSE) [![License Compliance](https:
+  //github.com/deepset-ai/haystack/actions/workflows/license_compliance.yml/
+     badge.svg)](https://github.com/deepset-ai/haystack/actions/workflows/
+license_compliance.yml) | | Meta | [![Discord](https://img.shields.io/discord/
+   993534733298450452?logo=discord)](https://discord.gg/haystack) [![Twitter
+     Follow](https://img.shields.io/twitter/follow/haystack_ai)](https://
+                          twitter.com/haystack_ai) |
 [Haystack](https://haystack.deepset.ai/) is an end-to-end LLM framework that
 allows you to build applications powered by LLMs, Transformer models, vector
 search and more. Whether you want to perform retrieval-augmented generation
 (RAG), document search, question answering or answer generation, Haystack can
 orchestrate state-of-the-art embedding models and LLMs into pipelines to build
 end-to-end NLP applications and solve your use case. ## Installation The
 simplest way to get Haystack is via pip: ```sh pip install haystack-ai ```
```

