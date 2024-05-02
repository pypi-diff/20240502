# Comparing `tmp/datadreamer_dev-0.8.0.tar.gz` & `tmp/datadreamer_dev-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadreamer_dev-0.8.0.tar", max compression
+gzip compressed data, was "datadreamer_dev-0.9.0.tar", max compression
```

## Comparing `datadreamer_dev-0.8.0.tar` & `datadreamer_dev-0.9.0.tar`

### file list

```diff
@@ -1,179 +1,179 @@
--rw-r--r--   0        0        0     1078 2024-02-02 01:20:57.161082 datadreamer_dev-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     7457 2024-02-02 01:20:57.161082 datadreamer_dev-0.8.0/README.md
--rw-r--r--   0        0        0      953 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/.env
--rw-r--r--   0        0        0     2042 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/.gitignore
--rw-r--r--   0        0        0      768 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/.secrets.template.env
--rw-r--r--   0        0        0      171 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/__cli__.py
--rw-r--r--   0        0        0     2675 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/__init__.py
--rw-r--r--   0        0        0      308 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/__main__.py
--rw-r--r--   0        0        0      207 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/_cachable/__init__.py
--rw-r--r--   0        0        0    37066 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/_cachable/_cachable.py
--rw-r--r--   0        0        0     7517 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/_cachable/_parallel_cachable.py
--rw-r--r--   0        0        0        0 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/_stubs/.gitkeep
--rw-r--r--   0        0        0     6649 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/_stubs/datasets/__init__.pyi
--rw-r--r--   0        0        0    22987 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/datadreamer.py
--rw-r--r--   0        0        0     1256 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/datasets/__init__.py
--rw-r--r--   0        0        0    11866 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/datasets/datasets.py
--rw-r--r--   0        0        0     2621 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/datasets/utils.py
--rw-r--r--   0        0        0     1135 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/embedders/__init__.py
--rw-r--r--   0        0        0     3127 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/embedders/embedder.py
--rw-r--r--   0        0        0     7267 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/embedders/openai_embedder.py
--rw-r--r--   0        0        0      537 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/embedders/parallel_embedder.py
--rw-r--r--   0        0        0    12082 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/embedders/sentence_transformers_embedder.py
--rw-r--r--   0        0        0     6652 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/embedders/together_embedder.py
--rw-r--r--   0        0        0      387 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/errors/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/errors/steps/__init__.py
--rw-r--r--   0        0        0      610 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/errors/steps/step.py
--rw-r--r--   0        0        0     3849 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/llms/__init__.py
--rw-r--r--   0        0        0    23617 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/llms/_chat_prompt_templates.py
--rw-r--r--   0        0        0     7593 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/llms/_litellm.py
--rw-r--r--   0        0        0    10956 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/llms/_llm_api.py
--rw-r--r--   0        0        0     2675 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/llms/_tokenizers.py
--rw-r--r--   0        0        0      792 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/llms/ai21.py
--rw-r--r--   0        0        0     2035 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/llms/anthropic.py
--rw-r--r--   0        0        0     2236 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/llms/bedrock.py
--rw-r--r--   0        0        0      791 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/llms/cohere.py
--rw-r--r--   0        0        0     7145 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/llms/ctransformers.py
--rw-r--r--   0        0        0     8531 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/llms/hf_api_endpoint.py
--rw-r--r--   0        0        0    23295 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/llms/hf_transformers.py
--rw-r--r--   0        0        0    11265 2024-02-02 01:20:57.169082 datadreamer_dev-0.8.0/datadreamer/llms/llm.py
--rw-r--r--   0        0        0     6864 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/llms/mistral_ai.py
--rw-r--r--   0        0        0    17021 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/llms/openai.py
--rw-r--r--   0        0        0     8161 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/llms/openai_assistant.py
--rw-r--r--   0        0        0     4633 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/llms/palm.py
--rw-r--r--   0        0        0     1868 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/llms/parallel_llm.py
--rw-r--r--   0        0        0     7978 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/llms/petals.py
--rw-r--r--   0        0        0     7599 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/llms/together.py
--rw-r--r--   0        0        0     4886 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/llms/vertex_ai.py
--rw-r--r--   0        0        0    11205 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/llms/vllm.py
--rw-r--r--   0        0        0      141 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/logging/__init__.py
--rw-r--r--   0        0        0      885 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/logging/logger.py
--rw-r--r--   0        0        0       95 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/pickling/__init__.py
--rw-r--r--   0        0        0     1501 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/pickling/pickle.py
--rw-r--r--   0        0        0     3056 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/project/__init__.py
--rw-r--r--   0        0        0     1698 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/project/builtin_tasks.py
--rw-r--r--   0        0        0     2790 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/project/debug.py
--rw-r--r--   0        0        0     4767 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/project/devices.py
--rw-r--r--   0        0        0      159 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/project/environment.py
--rw-r--r--   0        0        0     1946 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/project/pennnlp.py
--rw-r--r--   0        0        0     1226 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/project/persistent_storage.py
--rw-r--r--   0        0        0     9175 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/project/report.py
--rw-r--r--   0        0        0     6105 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/project/serve.py
--rw-r--r--   0        0        0        0 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/py.typed
--rw-r--r--   0        0        0       19 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/requirements-accelerator-device.txt
--rw-r--r--   0        0        0       19 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/requirements-cpu.txt
--rw-r--r--   0        0        0      268 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/requirements-dev.txt
--rw-r--r--   0        0        0      118 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/requirements-test.txt
--rw-r--r--   0        0        0      680 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/requirements.txt
--rw-r--r--   0        0        0     1068 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/retrievers/__init__.py
--rw-r--r--   0        0        0    11292 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/retrievers/embedding_retriever.py
--rw-r--r--   0        0        0     1030 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/retrievers/parallel_retriever.py
--rw-r--r--   0        0        0     5575 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/retrievers/retriever.py
--rw-r--r--   0        0        0    11503 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/__init__.py
--rw-r--r--   0        0        0      826 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/data_card.py
--rw-r--r--   0        0        0     3011 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/data_sources/csv_data_source.py
--rw-r--r--   0        0        0     3016 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/data_sources/data_source.py
--rw-r--r--   0        0        0     2133 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/data_sources/hf_dataset_data_source.py
--rw-r--r--   0        0        0     5171 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/data_sources/hf_hub_data_source.py
--rw-r--r--   0        0        0     2943 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/data_sources/json_data_source.py
--rw-r--r--   0        0        0     2943 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/data_sources/text_data_source.py
--rw-r--r--   0        0        0     4739 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/prompt/_prompt_base.py
--rw-r--r--   0        0        0     7327 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/prompt/data_from_attributed_prompt.py
--rw-r--r--   0        0        0     1729 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/prompt/data_from_prompt.py
--rw-r--r--   0        0        0     5860 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/prompt/few_shot_prompt.py
--rw-r--r--   0        0        0     5465 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/prompt/few_shot_prompt_with_retrieval.py
--rw-r--r--   0        0        0     4432 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/prompt/filter_with_prompt.py
--rw-r--r--   0        0        0     8274 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/prompt/judge_generation_pairs_with_prompt.py
--rw-r--r--   0        0        0     7228 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/prompt/judge_pairs_with_prompt.py
--rw-r--r--   0        0        0     2624 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/prompt/process_with_prompt.py
--rw-r--r--   0        0        0      416 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/prompt/prompt.py
--rw-r--r--   0        0        0     5513 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/prompt/rag_prompt.py
--rw-r--r--   0        0        0     5572 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/prompt/rank_with_prompt.py
--rw-r--r--   0        0        0    99921 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/step.py
--rw-r--r--   0        0        0     1989 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/step_background.py
--rw-r--r--   0        0        0     1485 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/step_export.py
--rw-r--r--   0        0        0    32412 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/step_operations.py
--rw-r--r--   0        0        0    33686 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/step_output.py
--rw-r--r--   0        0        0     9180 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/tasks/cosine_similarity.py
--rw-r--r--   0        0        0     2756 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/tasks/embed.py
--rw-r--r--   0        0        0     3266 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/tasks/retrieve.py
--rw-r--r--   0        0        0     2585 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/steps/tasks/run_task_model.py
--rw-r--r--   0        0        0      817 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/task_models/__init__.py
--rw-r--r--   0        0        0    11129 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/task_models/hf_classification_task_model.py
--rw-r--r--   0        0        0     1195 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/task_models/parallel_task_model.py
--rw-r--r--   0        0        0     2641 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/task_models/task_model.py
--rw-r--r--   0        0        0        0 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/tests/__init__.py
--rw-r--r--   0        0        0      545 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/tests/datasets/__init__.py
--rw-r--r--   0        0        0    10385 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/tests/datasets/test_datasets.py
--rw-r--r--   0        0        0     3367 2024-02-02 01:20:57.173082 datadreamer_dev-0.8.0/datadreamer/tests/datasets/test_utils.py
--rw-r--r--   0        0        0        0 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/embedders/__init__.py
--rw-r--r--   0        0        0    10983 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/embedders/test_embedders.py
--rw-r--r--   0        0        0        0 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/llms/__init__.py
--rw-r--r--   0        0        0   115857 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/llms/test_llms.py
--rw-r--r--   0        0        0        0 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/retrievers/__init__.py
--rw-r--r--   0        0        0    13132 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/retrievers/test_retrievers.py
--rw-r--r--   0        0        0        0 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/steps/__init__.py
--rw-r--r--   0        0        0        0 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/steps/prompt/__init__.py
--rw-r--r--   0        0        0    29214 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/steps/prompt/test_prompt.py
--rw-r--r--   0        0        0        0 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/steps/tasks/__init__.py
--rw-r--r--   0        0        0     8716 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/steps/tasks/test_tasks.py
--rw-r--r--   0        0        0     9157 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/steps/test_data_sources.py
--rw-r--r--   0        0        0    16938 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/steps/test_step.py
--rw-r--r--   0        0        0     8551 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/steps/test_step_background.py
--rw-r--r--   0        0        0    15976 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/steps/test_step_export.py
--rw-r--r--   0        0        0    59342 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/steps/test_step_operations.py
--rw-r--r--   0        0        0   104583 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/steps/test_step_output.py
--rw-r--r--   0        0        0        0 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/task_models/__init__.py
--rw-r--r--   0        0        0     3524 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/task_models/test_task_models.py
--rw-r--r--   0        0        0      207 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/test_cli.py
--rw-r--r--   0        0        0    22149 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/test_datadreamer.py
--rw-r--r--   0        0        0      975 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/test_package.py
--rw-r--r--   0        0        0        0 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/test_utils/__init__.py
--rw-r--r--   0        0        0       27 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/test_utils/config.py
--rw-r--r--   0        0        0        0 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/test_utils/fixtures/__init__.py
--rw-r--r--   0        0        0      942 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/test_utils/fixtures/bitsandbytes_fixture.py
--rw-r--r--   0        0        0      406 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/test_utils/fixtures/clear_space.py
--rw-r--r--   0        0        0      109 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/test_utils/fixtures/cli_runner.py
--rw-r--r--   0        0        0      540 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/test_utils/fixtures/create_datadreamer.py
--rw-r--r--   0        0        0      953 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/test_utils/fixtures/create_test_step.py
--rw-r--r--   0        0        0      415 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/test_utils/fixtures/mock_llm.py
--rw-r--r--   0        0        0      189 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/test_utils/fixtures/restore_os_environ.py
--rw-r--r--   0        0        0        0 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/trainers/__init__.py
--rw-r--r--   0        0        0    37240 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/trainers/test_distributed.py
--rw-r--r--   0        0        0   162367 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/trainers/test_trainers.py
--rw-r--r--   0        0        0        0 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/utils/__init__.py
--rw-r--r--   0        0        0     3975 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/tests/utils/test_device_utils.py
--rw-r--r--   0        0        0     3381 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/trainers/__init__.py
--rw-r--r--   0        0        0    66382 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/trainers/_train_hf_base.py
--rw-r--r--   0        0        0        0 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/trainers/_vendored/__init__.py
--rw-r--r--   0        0        0    12262 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/trainers/_vendored/_dpo_helper.py
--rw-r--r--   0        0        0     4045 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/trainers/_vendored/_sentence_transformer_helper.py
--rw-r--r--   0        0        0     4485 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/trainers/_vendored/_setfit_helper.py
--rw-r--r--   0        0        0    59972 2024-02-02 01:20:57.177082 datadreamer_dev-0.8.0/datadreamer/trainers/_vendored/dpo_trainer.py
--rw-r--r--   0        0        0    18284 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/trainers/train_hf_classifier.py
--rw-r--r--   0        0        0    21196 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/trainers/train_hf_dpo.py
--rw-r--r--   0        0        0    17133 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/trainers/train_hf_finetune.py
--rw-r--r--   0        0        0    34820 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/trainers/train_hf_ppo.py
--rw-r--r--   0        0        0    30364 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/trainers/train_hf_reward_model.py
--rw-r--r--   0        0        0    17230 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/trainers/train_openai_finetune.py
--rw-r--r--   0        0        0    39637 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/trainers/train_sentence_transformer.py
--rw-r--r--   0        0        0    25126 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/trainers/train_setfit_classifier.py
--rw-r--r--   0        0        0    14024 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/trainers/trainer.py
--rw-r--r--   0        0        0        0 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/utils/__init__.py
--rw-r--r--   0        0        0      392 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/utils/arg_utils.py
--rw-r--r--   0        0        0    11311 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/utils/background_utils.py
--rw-r--r--   0        0        0      676 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/utils/collection_utils.py
--rw-r--r--   0        0        0     7702 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/utils/device_utils.py
--rw-r--r--   0        0        0    11608 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/utils/distributed_utils.py
--rw-r--r--   0        0        0     3557 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/utils/fingerprint_utils.py
--rw-r--r--   0        0        0     1383 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/utils/fs_utils.py
--rw-r--r--   0        0        0    10540 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/utils/hf_chat_prompt_templates.py
--rw-r--r--   0        0        0     7784 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/utils/hf_hub_utils.py
--rw-r--r--   0        0        0     7335 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/utils/hf_model_utils.py
--rw-r--r--   0        0        0     4320 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/utils/import_utils.py
--rw-r--r--   0        0        0      249 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/utils/ring_utils.py
--rw-r--r--   0        0        0      780 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/utils/str_utils.py
--rw-r--r--   0        0        0      814 2024-02-02 01:20:57.181082 datadreamer_dev-0.8.0/datadreamer/utils/time_utils.py
--rw-r--r--   0        0        0     4946 2024-02-02 01:26:38.684302 datadreamer_dev-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     9982 1970-01-01 00:00:00.000000 datadreamer_dev-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-02-02 17:11:20.837065 datadreamer_dev-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     7457 2024-02-02 17:11:20.837065 datadreamer_dev-0.9.0/README.md
+-rw-r--r--   0        0        0      953 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/.env
+-rw-r--r--   0        0        0     2042 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/.gitignore
+-rw-r--r--   0        0        0      768 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/.secrets.template.env
+-rw-r--r--   0        0        0      171 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/__cli__.py
+-rw-r--r--   0        0        0     2675 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/__init__.py
+-rw-r--r--   0        0        0      308 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/__main__.py
+-rw-r--r--   0        0        0      207 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/_cachable/__init__.py
+-rw-r--r--   0        0        0    37066 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/_cachable/_cachable.py
+-rw-r--r--   0        0        0     7517 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/_cachable/_parallel_cachable.py
+-rw-r--r--   0        0        0        0 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/_stubs/.gitkeep
+-rw-r--r--   0        0        0     6649 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/_stubs/datasets/__init__.pyi
+-rw-r--r--   0        0        0    23163 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/datadreamer.py
+-rw-r--r--   0        0        0     1256 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/datasets/__init__.py
+-rw-r--r--   0        0        0    12466 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/datasets/datasets.py
+-rw-r--r--   0        0        0     2621 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/datasets/utils.py
+-rw-r--r--   0        0        0     1135 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/embedders/__init__.py
+-rw-r--r--   0        0        0     3323 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/embedders/embedder.py
+-rw-r--r--   0        0        0     7476 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/embedders/openai_embedder.py
+-rw-r--r--   0        0        0      537 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/embedders/parallel_embedder.py
+-rw-r--r--   0        0        0    12291 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/embedders/sentence_transformers_embedder.py
+-rw-r--r--   0        0        0     6861 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/embedders/together_embedder.py
+-rw-r--r--   0        0        0      186 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/errors/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/errors/steps/__init__.py
+-rw-r--r--   0        0        0      910 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/errors/steps/step.py
+-rw-r--r--   0        0        0     3849 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/llms/__init__.py
+-rw-r--r--   0        0        0    23617 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/llms/_chat_prompt_templates.py
+-rw-r--r--   0        0        0     8166 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/llms/_litellm.py
+-rw-r--r--   0        0        0    11529 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/llms/_llm_api.py
+-rw-r--r--   0        0        0     2675 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/llms/_tokenizers.py
+-rw-r--r--   0        0        0      792 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/llms/ai21.py
+-rw-r--r--   0        0        0     2035 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/llms/anthropic.py
+-rw-r--r--   0        0        0     2236 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/llms/bedrock.py
+-rw-r--r--   0        0        0      791 2024-02-02 17:11:20.845064 datadreamer_dev-0.9.0/datadreamer/llms/cohere.py
+-rw-r--r--   0        0        0     7509 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/llms/ctransformers.py
+-rw-r--r--   0        0        0     8531 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/llms/hf_api_endpoint.py
+-rw-r--r--   0        0        0    23868 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/llms/hf_transformers.py
+-rw-r--r--   0        0        0    13632 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/llms/llm.py
+-rw-r--r--   0        0        0     6864 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/llms/mistral_ai.py
+-rw-r--r--   0        0        0    17614 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/llms/openai.py
+-rw-r--r--   0        0        0     8161 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/llms/openai_assistant.py
+-rw-r--r--   0        0        0     4633 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/llms/palm.py
+-rw-r--r--   0        0        0     2441 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/llms/parallel_llm.py
+-rw-r--r--   0        0        0     7978 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/llms/petals.py
+-rw-r--r--   0        0        0     7599 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/llms/together.py
+-rw-r--r--   0        0        0     4886 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/llms/vertex_ai.py
+-rw-r--r--   0        0        0    11205 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/llms/vllm.py
+-rw-r--r--   0        0        0      141 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/logging/__init__.py
+-rw-r--r--   0        0        0      885 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/logging/logger.py
+-rw-r--r--   0        0        0       95 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/pickling/__init__.py
+-rw-r--r--   0        0        0     1501 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/pickling/pickle.py
+-rw-r--r--   0        0        0     3056 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/project/__init__.py
+-rw-r--r--   0        0        0     1698 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/project/builtin_tasks.py
+-rw-r--r--   0        0        0     2790 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/project/debug.py
+-rw-r--r--   0        0        0     4767 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/project/devices.py
+-rw-r--r--   0        0        0      159 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/project/environment.py
+-rw-r--r--   0        0        0     1946 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/project/pennnlp.py
+-rw-r--r--   0        0        0     1226 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/project/persistent_storage.py
+-rw-r--r--   0        0        0     9175 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/project/report.py
+-rw-r--r--   0        0        0     6105 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/project/serve.py
+-rw-r--r--   0        0        0        0 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/py.typed
+-rw-r--r--   0        0        0       19 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/requirements-accelerator-device.txt
+-rw-r--r--   0        0        0       19 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/requirements-cpu.txt
+-rw-r--r--   0        0        0      268 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/requirements-dev.txt
+-rw-r--r--   0        0        0      118 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/requirements-test.txt
+-rw-r--r--   0        0        0      680 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/requirements.txt
+-rw-r--r--   0        0        0     1068 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/retrievers/__init__.py
+-rw-r--r--   0        0        0    11292 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/retrievers/embedding_retriever.py
+-rw-r--r--   0        0        0     1030 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/retrievers/parallel_retriever.py
+-rw-r--r--   0        0        0     5575 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/retrievers/retriever.py
+-rw-r--r--   0        0        0    11503 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/__init__.py
+-rw-r--r--   0        0        0      826 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/data_card.py
+-rw-r--r--   0        0        0     3011 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/data_sources/csv_data_source.py
+-rw-r--r--   0        0        0     3016 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/data_sources/data_source.py
+-rw-r--r--   0        0        0     2133 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/data_sources/hf_dataset_data_source.py
+-rw-r--r--   0        0        0     5171 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/data_sources/hf_hub_data_source.py
+-rw-r--r--   0        0        0     2943 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/data_sources/json_data_source.py
+-rw-r--r--   0        0        0     2943 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/data_sources/text_data_source.py
+-rw-r--r--   0        0        0     4739 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/prompt/_prompt_base.py
+-rw-r--r--   0        0        0     7327 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/prompt/data_from_attributed_prompt.py
+-rw-r--r--   0        0        0     1729 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/prompt/data_from_prompt.py
+-rw-r--r--   0        0        0     5860 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/prompt/few_shot_prompt.py
+-rw-r--r--   0        0        0     5465 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/prompt/few_shot_prompt_with_retrieval.py
+-rw-r--r--   0        0        0     4432 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/prompt/filter_with_prompt.py
+-rw-r--r--   0        0        0     8274 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/prompt/judge_generation_pairs_with_prompt.py
+-rw-r--r--   0        0        0     7228 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/prompt/judge_pairs_with_prompt.py
+-rw-r--r--   0        0        0     2624 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/prompt/process_with_prompt.py
+-rw-r--r--   0        0        0      416 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/prompt/prompt.py
+-rw-r--r--   0        0        0     5513 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/prompt/rag_prompt.py
+-rw-r--r--   0        0        0     5572 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/prompt/rank_with_prompt.py
+-rw-r--r--   0        0        0    99923 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/step.py
+-rw-r--r--   0        0        0     1989 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/step_background.py
+-rw-r--r--   0        0        0     1485 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/step_export.py
+-rw-r--r--   0        0        0    32412 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/step_operations.py
+-rw-r--r--   0        0        0    33686 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/step_output.py
+-rw-r--r--   0        0        0     9180 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/tasks/cosine_similarity.py
+-rw-r--r--   0        0        0     2756 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/tasks/embed.py
+-rw-r--r--   0        0        0     3266 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/tasks/retrieve.py
+-rw-r--r--   0        0        0     2585 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/steps/tasks/run_task_model.py
+-rw-r--r--   0        0        0      817 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/task_models/__init__.py
+-rw-r--r--   0        0        0    11338 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/task_models/hf_classification_task_model.py
+-rw-r--r--   0        0        0     1404 2024-02-02 17:11:20.849064 datadreamer_dev-0.9.0/datadreamer/task_models/parallel_task_model.py
+-rw-r--r--   0        0        0     2837 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/task_models/task_model.py
+-rw-r--r--   0        0        0        0 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/__init__.py
+-rw-r--r--   0        0        0      545 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/datasets/__init__.py
+-rw-r--r--   0        0        0    10385 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/datasets/test_datasets.py
+-rw-r--r--   0        0        0     3367 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/datasets/test_utils.py
+-rw-r--r--   0        0        0        0 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/embedders/__init__.py
+-rw-r--r--   0        0        0    10983 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/embedders/test_embedders.py
+-rw-r--r--   0        0        0        0 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/llms/__init__.py
+-rw-r--r--   0        0        0   115857 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/llms/test_llms.py
+-rw-r--r--   0        0        0        0 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/retrievers/__init__.py
+-rw-r--r--   0        0        0    13132 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/retrievers/test_retrievers.py
+-rw-r--r--   0        0        0        0 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/steps/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/steps/prompt/__init__.py
+-rw-r--r--   0        0        0    29214 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/steps/prompt/test_prompt.py
+-rw-r--r--   0        0        0        0 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/steps/tasks/__init__.py
+-rw-r--r--   0        0        0     8716 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/steps/tasks/test_tasks.py
+-rw-r--r--   0        0        0     9157 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/steps/test_data_sources.py
+-rw-r--r--   0        0        0    16938 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/steps/test_step.py
+-rw-r--r--   0        0        0     8551 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/steps/test_step_background.py
+-rw-r--r--   0        0        0    15976 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/steps/test_step_export.py
+-rw-r--r--   0        0        0    59342 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/steps/test_step_operations.py
+-rw-r--r--   0        0        0   104583 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/steps/test_step_output.py
+-rw-r--r--   0        0        0        0 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/task_models/__init__.py
+-rw-r--r--   0        0        0     3524 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/task_models/test_task_models.py
+-rw-r--r--   0        0        0      207 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/test_cli.py
+-rw-r--r--   0        0        0    22149 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/test_datadreamer.py
+-rw-r--r--   0        0        0      975 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/test_package.py
+-rw-r--r--   0        0        0        0 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0       27 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/test_utils/config.py
+-rw-r--r--   0        0        0        0 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/test_utils/fixtures/__init__.py
+-rw-r--r--   0        0        0      942 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/test_utils/fixtures/bitsandbytes_fixture.py
+-rw-r--r--   0        0        0      406 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/test_utils/fixtures/clear_space.py
+-rw-r--r--   0        0        0      109 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/test_utils/fixtures/cli_runner.py
+-rw-r--r--   0        0        0      540 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/test_utils/fixtures/create_datadreamer.py
+-rw-r--r--   0        0        0      953 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/test_utils/fixtures/create_test_step.py
+-rw-r--r--   0        0        0      415 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/test_utils/fixtures/mock_llm.py
+-rw-r--r--   0        0        0      189 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/test_utils/fixtures/restore_os_environ.py
+-rw-r--r--   0        0        0        0 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/trainers/__init__.py
+-rw-r--r--   0        0        0    37240 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/trainers/test_distributed.py
+-rw-r--r--   0        0        0   162367 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/trainers/test_trainers.py
+-rw-r--r--   0        0        0        0 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/utils/__init__.py
+-rw-r--r--   0        0        0     3975 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/tests/utils/test_device_utils.py
+-rw-r--r--   0        0        0     4206 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/trainers/__init__.py
+-rw-r--r--   0        0        0    67320 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/trainers/_train_hf_base.py
+-rw-r--r--   0        0        0        0 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/trainers/_vendored/__init__.py
+-rw-r--r--   0        0        0    12262 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/trainers/_vendored/_dpo_helper.py
+-rw-r--r--   0        0        0     4045 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/trainers/_vendored/_sentence_transformer_helper.py
+-rw-r--r--   0        0        0     4485 2024-02-02 17:11:20.853064 datadreamer_dev-0.9.0/datadreamer/trainers/_vendored/_setfit_helper.py
+-rw-r--r--   0        0        0    59972 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/trainers/_vendored/dpo_trainer.py
+-rw-r--r--   0        0        0    18284 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/trainers/train_hf_classifier.py
+-rw-r--r--   0        0        0    21196 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/trainers/train_hf_dpo.py
+-rw-r--r--   0        0        0    17133 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/trainers/train_hf_finetune.py
+-rw-r--r--   0        0        0    34820 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/trainers/train_hf_ppo.py
+-rw-r--r--   0        0        0    30364 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/trainers/train_hf_reward_model.py
+-rw-r--r--   0        0        0    17803 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/trainers/train_openai_finetune.py
+-rw-r--r--   0        0        0    39637 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/trainers/train_sentence_transformer.py
+-rw-r--r--   0        0        0    25126 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/trainers/train_setfit_classifier.py
+-rw-r--r--   0        0        0    14517 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/trainers/trainer.py
+-rw-r--r--   0        0        0        0 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/utils/__init__.py
+-rw-r--r--   0        0        0      392 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/utils/arg_utils.py
+-rw-r--r--   0        0        0    11311 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/utils/background_utils.py
+-rw-r--r--   0        0        0      676 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/utils/collection_utils.py
+-rw-r--r--   0        0        0     7702 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/utils/device_utils.py
+-rw-r--r--   0        0        0    11608 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/utils/distributed_utils.py
+-rw-r--r--   0        0        0     3557 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/utils/fingerprint_utils.py
+-rw-r--r--   0        0        0     1383 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/utils/fs_utils.py
+-rw-r--r--   0        0        0    10540 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/utils/hf_chat_prompt_templates.py
+-rw-r--r--   0        0        0     7784 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/utils/hf_hub_utils.py
+-rw-r--r--   0        0        0     7335 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/utils/hf_model_utils.py
+-rw-r--r--   0        0        0     4320 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/utils/import_utils.py
+-rw-r--r--   0        0        0      249 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/utils/ring_utils.py
+-rw-r--r--   0        0        0      780 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/utils/str_utils.py
+-rw-r--r--   0        0        0      814 2024-02-02 17:11:20.857065 datadreamer_dev-0.9.0/datadreamer/utils/time_utils.py
+-rw-r--r--   0        0        0     4946 2024-02-02 17:16:32.109419 datadreamer_dev-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     9982 1970-01-01 00:00:00.000000 datadreamer_dev-0.9.0/PKG-INFO
```

### Comparing `datadreamer_dev-0.8.0/LICENSE.txt` & `datadreamer_dev-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/README.md` & `datadreamer_dev-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/.env` & `datadreamer_dev-0.9.0/datadreamer/.env`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/.gitignore` & `datadreamer_dev-0.9.0/datadreamer/.gitignore`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/.secrets.template.env` & `datadreamer_dev-0.9.0/datadreamer/.secrets.template.env`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/__init__.py` & `datadreamer_dev-0.9.0/datadreamer/__init__.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/_cachable/_cachable.py` & `datadreamer_dev-0.9.0/datadreamer/_cachable/_cachable.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/_cachable/_parallel_cachable.py` & `datadreamer_dev-0.9.0/datadreamer/_cachable/_parallel_cachable.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/_stubs/datasets/__init__.pyi` & `datadreamer_dev-0.9.0/datadreamer/_stubs/datasets/__init__.pyi`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/datadreamer.py` & `datadreamer_dev-0.9.0/datadreamer/datadreamer.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,19 @@
         return (
             not DataDreamer.initialized()
             or get_thread_id() in DataDreamer.ctx.thread_ids
         )
 
     @staticmethod
     def get_output_folder_path() -> str:
+        """Gets the output folder path of the current DataDreamer session.
+
+        Returns:
+            The output folder path of the current DataDreamer session.
+        """
         if hasattr(DataDreamer.ctx, "output_folder_path"):
             return DataDreamer.ctx.output_folder_path
         else:
             raise RuntimeError("DataDreamer is running in-memory.")
 
     @staticmethod
     def _has_step_name(name: str) -> bool:
```

### Comparing `datadreamer_dev-0.8.0/datadreamer/datasets/__init__.py` & `datadreamer_dev-0.9.0/datadreamer/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/datasets/datasets.py` & `datadreamer_dev-0.9.0/datadreamer/datasets/datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,22 +13,25 @@
 if TYPE_CHECKING:  # pragma: no cover
     from ..steps import Step
 
 
 class OutputDatasetMixin:
     @property
     def step(self) -> "Step":
+        """The step that produced the dataset."""
         return self._step  # type:ignore[attr-defined]
 
     @property
     def column_names(self) -> list[str]:
+        """The column names in the dataset."""
         return get_column_names(self.dataset)  # type:ignore[attr-defined]
 
     @property
     def num_columns(self) -> int:
+        """The number of columns in the dataset."""
         return len(self.column_names)
 
     @property
     def info(self) -> Any:
         return self.dataset.info  # type:ignore[attr-defined]
 
     @property
@@ -42,14 +45,22 @@
         if self._pickled or self._pickled_inferred:  # type:ignore[attr-defined]
             for row in iter(self.dataset):  # type:ignore[attr-defined]
                 yield unpickle_transform(row, features=self._features, batched=False)
         else:
             yield from iter(self.dataset)  # type:ignore[attr-defined]
 
     def __getitem__(self, key: int | slice | str | Iterable[int]) -> Any:
+        """Get a row or column from the dataset.
+
+        Args:
+            key: The index or name of the column to get.
+
+        Returns:
+            The row or column from the dataset.
+        """
         if isinstance(key, str):
             feature = self._features.get(key, None)
             feature_is_pickle_type = False
             if isinstance(feature, Value) and feature.dtype == "binary":
                 feature_is_pickle_type = True
             if isinstance(self.dataset, Dataset):  # type:ignore[attr-defined]
                 return OutputDatasetColumn(
@@ -194,18 +205,20 @@
         for f in self._features.values():
             if isinstance(f, Value) and f.dtype == "binary":
                 self._pickled_inferred = True
                 break
 
     @property
     def dataset(self) -> IterableDataset:
+        """The underlying Hugging Face :py:class:`~datasets.IterableDataset`."""
         return self._dataset
 
     @property
     def num_rows(self) -> None | int:
+        """The number of rows in the dataset."""
         return self.total_num_rows
 
 
 class OutputDataset(OutputDatasetMixin):
     def __init__(self, step: "Step", dataset: Dataset, pickled: bool = False):
         from ..steps import Step
 
@@ -216,28 +229,30 @@
         self._step: "Step" = step
         self._dataset: Dataset = dataset
         self._pickled: bool = pickled
         self._pickled_inferred: bool = False
 
     @property
     def dataset(self) -> Dataset:
+        """The underlying Hugging Face :py:class:`~datasets.Dataset`."""
         return self._dataset
 
     def save_to_disk(
         self, path: str, num_proc: None | int, num_shards: None | int
     ) -> None:
         self._dataset.save_to_disk(
             path,
             num_proc=min(num_proc if num_proc is not None else 1, len(self._dataset)),
             num_shards=num_shards,
         )
         self._dataset = Dataset.load_from_disk(path)
 
     @property
     def num_rows(self) -> int:
+        """The number of rows in the dataset."""
         return len(self)
 
     def __len__(self):
         return len(self.dataset)
 
 
 class OutputIterableDatasetColumn(OutputDatasetColumnMixin, OutputIterableDataset):
```

### Comparing `datadreamer_dev-0.8.0/datadreamer/datasets/utils.py` & `datadreamer_dev-0.9.0/datadreamer/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/embedders/__init__.py` & `datadreamer_dev-0.9.0/datadreamer/embedders/__init__.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/embedders/embedder.py` & `datadreamer_dev-0.9.0/datadreamer/embedders/embedder.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 class Embedder(TaskModel):
     def __init__(self, model_name: str, cache_folder_path: None | str = None):
         super().__init__(cache_folder_path=cache_folder_path)
         self.model_name = model_name
 
     @abstractmethod
     def count_tokens(self, value: str) -> int:
+        """Counts the number of tokens in a string.
+
+        Args:
+            value: The string to count tokens for.
+
+        Returns:
+            The number of tokens in the string.
+        """
         pass
 
     @property
     @abstractmethod
     def model_max_length(self) -> int:
         pass
```

### Comparing `datadreamer_dev-0.8.0/datadreamer/embedders/openai_embedder.py` & `datadreamer_dev-0.9.0/datadreamer/embedders/openai_embedder.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,23 @@
 
     @cached_property
     def tokenizer(self) -> Encoding:
         return OpenAI.tokenizer.func(self)  # type: ignore[attr-defined]
 
     @ring.lru(maxsize=5000)
     def count_tokens(self, value: str) -> int:
+        """Counts the number of tokens in a string.
+
+        Args:
+            value: The string to count tokens for.
+
+        Returns:
+            The number of tokens in the string.
+        """
+        pass
         return OpenAI.count_tokens._callable.wrapped_callable(self, value)
 
     @cached_property
     def model_max_length(self) -> int:
         return 8191
 
     @cached_property
```

### Comparing `datadreamer_dev-0.8.0/datadreamer/embedders/parallel_embedder.py` & `datadreamer_dev-0.9.0/datadreamer/embedders/parallel_embedder.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/embedders/sentence_transformers_embedder.py` & `datadreamer_dev-0.9.0/datadreamer/embedders/sentence_transformers_embedder.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,23 @@
         return model
 
     @cached_property
     def tokenizer(self) -> Any:
         return self.model.tokenizer
 
     def count_tokens(self, value: str) -> int:
+        """Counts the number of tokens in a string.
+
+        Args:
+            value: The string to count tokens for.
+
+        Returns:
+            The number of tokens in the string.
+        """
+        pass
         return len(self.tokenizer.encode(value))
 
     @cached_property
     def model_max_length(self) -> int:
         return self.model.max_seq_length
 
     @cached_property
```

### Comparing `datadreamer_dev-0.8.0/datadreamer/embedders/together_embedder.py` & `datadreamer_dev-0.9.0/datadreamer/embedders/together_embedder.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,23 @@
 
     @cached_property
     def tokenizer(self) -> Encoding:
         return Together.tokenizer.func(self)  # type: ignore[attr-defined]
 
     @ring.lru(maxsize=5000)
     def count_tokens(self, value: str) -> int:
+        """Counts the number of tokens in a string.
+
+        Args:
+            value: The string to count tokens for.
+
+        Returns:
+            The number of tokens in the string.
+        """
+        pass
         return Together.count_tokens._callable.wrapped_callable(self, value)
 
     @cached_property
     def model_max_length(self) -> int:
         return Together.get_max_context_length._callable.wrapped_callable(
             self, max_new_tokens=0
         )
```

### Comparing `datadreamer_dev-0.8.0/datadreamer/llms/__init__.py` & `datadreamer_dev-0.9.0/datadreamer/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/llms/_chat_prompt_templates.py` & `datadreamer_dev-0.9.0/datadreamer/llms/_chat_prompt_templates.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/llms/_litellm.py` & `datadreamer_dev-0.9.0/datadreamer/llms/_litellm.py`

 * *Files 7% similar despite different names*

```diff
@@ -108,22 +108,41 @@
     def client(self) -> Any:
         with ignore_litellm_warnings():
             from litellm import completion
 
         return completion
 
     @ring.lru(maxsize=128)
-    def get_max_context_length(self, max_new_tokens: int) -> int:  # pragma: no cover
+    def get_max_context_length(self, max_new_tokens: int) -> int:
+        """Gets the maximum context length for the model. When ``max_new_tokens`` is
+        greater than 0, the maximum number of tokens that can be used for the prompt
+        context is returned.
+
+        Args:
+            max_new_tokens: The maximum number of tokens that can be generated.
+
+        Returns:
+            The maximum context length.
+        """  # pragma: no cover
         with ignore_litellm_warnings():
             from litellm import get_max_tokens
 
         return get_max_tokens(model=self._model_name_prefix + self.model_name)
 
     @ring.lru(maxsize=5000)
     def count_tokens(self, value: str) -> int:
+        """Counts the number of tokens in a string.
+
+        Args:
+            value: The string to count tokens for.
+
+        Returns:
+            The number of tokens in the string.
+        """
+        pass
         with ignore_litellm_warnings():
             from litellm import token_counter
 
         with ignore_litellm_warnings():
             return token_counter(
                 self._model_name_prefix + self.model_name,
                 messages=[{"user": "role", "content": value}],
```

### Comparing `datadreamer_dev-0.8.0/datadreamer/llms/_llm_api.py` & `datadreamer_dev-0.9.0/datadreamer/llms/_llm_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,15 +142,25 @@
             model_name=self.tokenizer_model_name,
             revision=self.tokenizer_revision,
             trust_remote_code=self.tokenizer_trust_remote_code,
             **self.kwargs,
         )
 
     @ring.lru(maxsize=128)
-    def get_max_context_length(self, max_new_tokens: int) -> int:  # pragma: no cover
+    def get_max_context_length(self, max_new_tokens: int) -> int:
+        """Gets the maximum context length for the model. When ``max_new_tokens`` is
+        greater than 0, the maximum number of tokens that can be used for the prompt
+        context is returned.
+
+        Args:
+            max_new_tokens: The maximum number of tokens that can be generated.
+
+        Returns:
+            The maximum context length.
+        """  # pragma: no cover
         model_name_lower = self.model_name.lower()
         if self.max_context_length is not None:
             return self.max_context_length
         if self.config is not None:
             estimate = get_model_max_context_length(
                 model_name=self.model_name, config=self.config
             )
@@ -174,14 +184,23 @@
                 " to remove this warning.",
                 stacklevel=2,
             )
         return estimate - max_new_tokens
 
     @ring.lru(maxsize=5000)
     def count_tokens(self, value: str) -> int:
+        """Counts the number of tokens in a string.
+
+        Args:
+            value: The string to count tokens for.
+
+        Returns:
+            The number of tokens in the string.
+        """
+        pass
         return len(self.tokenizer.encode(value))
 
     def _is_batch_size_exception(self, e: BaseException) -> bool:  # pragma: no cover
         return False
 
     @abstractmethod
     def _run_batch(
```

### Comparing `datadreamer_dev-0.8.0/datadreamer/llms/_tokenizers.py` & `datadreamer_dev-0.9.0/datadreamer/llms/_tokenizers.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/llms/ai21.py` & `datadreamer_dev-0.9.0/datadreamer/llms/ai21.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/llms/anthropic.py` & `datadreamer_dev-0.9.0/datadreamer/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/llms/bedrock.py` & `datadreamer_dev-0.9.0/datadreamer/llms/bedrock.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/llms/cohere.py` & `datadreamer_dev-0.9.0/datadreamer/llms/cohere.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/llms/ctransformers.py` & `datadreamer_dev-0.9.0/datadreamer/llms/ctransformers.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,14 +110,24 @@
 
     @cached_property
     def tokenizer(self) -> PreTrainedTokenizer:
         return AutoTokenizer.from_pretrained(self.model)
 
     @ring.lru(maxsize=128)
     def get_max_context_length(self, max_new_tokens: int) -> int:
+        """Gets the maximum context length for the model. When ``max_new_tokens`` is
+        greater than 0, the maximum number of tokens that can be used for the prompt
+        context is returned.
+
+        Args:
+            max_new_tokens: The maximum number of tokens that can be generated.
+
+        Returns:
+            The maximum context length.
+        """
         if self.max_context_length is None:
             return self.model._llm.context_length - max_new_tokens
         else:
             return self.max_context_length - max_new_tokens
 
     def _is_batch_size_exception(self, e: BaseException) -> bool:  # pragma: no cover
         return False
```

### Comparing `datadreamer_dev-0.8.0/datadreamer/llms/hf_api_endpoint.py` & `datadreamer_dev-0.9.0/datadreamer/llms/hf_api_endpoint.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/llms/hf_transformers.py` & `datadreamer_dev-0.9.0/datadreamer/llms/hf_transformers.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,23 +282,42 @@
             revision=self.revision,
             trust_remote_code=self.trust_remote_code,
             **self.kwargs,
         )
 
     @ring.lru(maxsize=128)
     def get_max_context_length(self, max_new_tokens: int) -> int:
+        """Gets the maximum context length for the model. When ``max_new_tokens`` is
+        greater than 0, the maximum number of tokens that can be used for the prompt
+        context is returned.
+
+        Args:
+            max_new_tokens: The maximum number of tokens that can be generated.
+
+        Returns:
+            The maximum context length.
+        """
         max_context_length = get_model_max_context_length(
             model_name=self.model_name, config=self.config
         )
         if self._is_encoder_decoder:
             return max_context_length
         else:
             return max_context_length - max_new_tokens
 
     def count_tokens(self, value: str) -> int:
+        """Counts the number of tokens in a string.
+
+        Args:
+            value: The string to count tokens for.
+
+        Returns:
+            The number of tokens in the string.
+        """
+        pass
         """_summary_
 
         Args:
             value (_type_): _description_
 
         Returns:
             _type_: _description_
```

### Comparing `datadreamer_dev-0.8.0/datadreamer/llms/mistral_ai.py` & `datadreamer_dev-0.9.0/datadreamer/llms/mistral_ai.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/llms/openai.py` & `datadreamer_dev-0.9.0/datadreamer/llms/openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,14 +181,24 @@
         try:
             return tiktoken.encoding_for_model(self.model_name)
         except KeyError:
             return tiktoken.get_encoding("cl100k_base")
 
     @ring.lru(maxsize=128)
     def get_max_context_length(self, max_new_tokens: int) -> int:  # pragma: no cover
+        """Gets the maximum context length for the model. When ``max_new_tokens`` is
+        greater than 0, the maximum number of tokens that can be used for the prompt
+        context is returned.
+
+        Args:
+            max_new_tokens: The maximum number of tokens that can be generated.
+
+        Returns:
+            The maximum context length.
+        """  # pragma: no cover
         model_name = _normalize_model_name(self.model_name)
         format_tokens = 0
         if _is_chat_model(model_name):
             # Each message is up to 4 tokens and there are 3 messages
             # (system prompt, user prompt, assistant response)
             # and then we have to account for the system prompt
             format_tokens = 4 * 3 + self.count_tokens(cast(str, self.system_prompt))
@@ -214,14 +224,23 @@
             max_context_length = 2049
         else:
             max_context_length = 8192
         return max_context_length - max_new_tokens - format_tokens
 
     @ring.lru(maxsize=5000)
     def count_tokens(self, value: str) -> int:
+        """Counts the number of tokens in a string.
+
+        Args:
+            value: The string to count tokens for.
+
+        Returns:
+            The number of tokens in the string.
+        """
+        pass
         return len(self.tokenizer.encode(value))
 
     def _run_batch(
         self,
         max_length_func: Callable[[list[str]], int],
         inputs: list[str],
         max_new_tokens: None | int = None,
```

### Comparing `datadreamer_dev-0.8.0/datadreamer/llms/openai_assistant.py` & `datadreamer_dev-0.9.0/datadreamer/llms/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/llms/palm.py` & `datadreamer_dev-0.9.0/datadreamer/llms/palm.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/llms/petals.py` & `datadreamer_dev-0.9.0/datadreamer/llms/petals.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/llms/together.py` & `datadreamer_dev-0.9.0/datadreamer/llms/together.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/llms/vertex_ai.py` & `datadreamer_dev-0.9.0/datadreamer/llms/vertex_ai.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/llms/vllm.py` & `datadreamer_dev-0.9.0/datadreamer/llms/vllm.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/logging/logger.py` & `datadreamer_dev-0.9.0/datadreamer/logging/logger.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/pickling/pickle.py` & `datadreamer_dev-0.9.0/datadreamer/pickling/pickle.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/project/__init__.py` & `datadreamer_dev-0.9.0/datadreamer/project/__init__.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/project/builtin_tasks.py` & `datadreamer_dev-0.9.0/datadreamer/project/builtin_tasks.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/project/debug.py` & `datadreamer_dev-0.9.0/datadreamer/project/debug.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/project/devices.py` & `datadreamer_dev-0.9.0/datadreamer/project/devices.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/project/pennnlp.py` & `datadreamer_dev-0.9.0/datadreamer/project/pennnlp.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/project/persistent_storage.py` & `datadreamer_dev-0.9.0/datadreamer/project/persistent_storage.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/project/report.py` & `datadreamer_dev-0.9.0/datadreamer/project/report.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/project/serve.py` & `datadreamer_dev-0.9.0/datadreamer/project/serve.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/requirements.txt` & `datadreamer_dev-0.9.0/datadreamer/requirements.txt`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/retrievers/__init__.py` & `datadreamer_dev-0.9.0/datadreamer/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/retrievers/embedding_retriever.py` & `datadreamer_dev-0.9.0/datadreamer/retrievers/embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/retrievers/parallel_retriever.py` & `datadreamer_dev-0.9.0/datadreamer/retrievers/parallel_retriever.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/retrievers/retriever.py` & `datadreamer_dev-0.9.0/datadreamer/retrievers/retriever.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/__init__.py` & `datadreamer_dev-0.9.0/datadreamer/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/data_card.py` & `datadreamer_dev-0.9.0/datadreamer/steps/data_card.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/data_sources/csv_data_source.py` & `datadreamer_dev-0.9.0/datadreamer/steps/data_sources/csv_data_source.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/data_sources/data_source.py` & `datadreamer_dev-0.9.0/datadreamer/steps/data_sources/data_source.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/data_sources/hf_dataset_data_source.py` & `datadreamer_dev-0.9.0/datadreamer/steps/data_sources/hf_dataset_data_source.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/data_sources/hf_hub_data_source.py` & `datadreamer_dev-0.9.0/datadreamer/steps/data_sources/hf_hub_data_source.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/data_sources/json_data_source.py` & `datadreamer_dev-0.9.0/datadreamer/steps/data_sources/json_data_source.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/data_sources/text_data_source.py` & `datadreamer_dev-0.9.0/datadreamer/steps/data_sources/text_data_source.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/prompt/_prompt_base.py` & `datadreamer_dev-0.9.0/datadreamer/steps/prompt/_prompt_base.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/prompt/data_from_attributed_prompt.py` & `datadreamer_dev-0.9.0/datadreamer/steps/prompt/data_from_attributed_prompt.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/prompt/data_from_prompt.py` & `datadreamer_dev-0.9.0/datadreamer/steps/prompt/data_from_prompt.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/prompt/few_shot_prompt.py` & `datadreamer_dev-0.9.0/datadreamer/steps/prompt/few_shot_prompt.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/prompt/few_shot_prompt_with_retrieval.py` & `datadreamer_dev-0.9.0/datadreamer/steps/prompt/few_shot_prompt_with_retrieval.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/prompt/filter_with_prompt.py` & `datadreamer_dev-0.9.0/datadreamer/steps/prompt/filter_with_prompt.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/prompt/judge_generation_pairs_with_prompt.py` & `datadreamer_dev-0.9.0/datadreamer/steps/prompt/judge_generation_pairs_with_prompt.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/prompt/judge_pairs_with_prompt.py` & `datadreamer_dev-0.9.0/datadreamer/steps/prompt/judge_pairs_with_prompt.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/prompt/process_with_prompt.py` & `datadreamer_dev-0.9.0/datadreamer/steps/prompt/process_with_prompt.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/prompt/rag_prompt.py` & `datadreamer_dev-0.9.0/datadreamer/steps/prompt/rag_prompt.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/prompt/rank_with_prompt.py` & `datadreamer_dev-0.9.0/datadreamer/steps/prompt/rank_with_prompt.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/step.py` & `datadreamer_dev-0.9.0/datadreamer/steps/step.py`

 * *Files 0% similar despite different names*

```diff
@@ -1958,15 +1958,15 @@
             stratify_by_column: The name of the column to use to stratify equally
                 between splits.
             writer_batch_size: The batch size to use if saving to disk.
             save_num_proc: The number of processes to use if saving to disk.
             save_num_shards: The number of shards on disk to save the dataset into.
             is_synthetic: Whether the dataset is synthetic (applies certain metadata
                 when publishing).
-            kwargs: Additional keyword arguments to pass to
+            **kwargs: Additional keyword arguments to pass to
                 :py:meth:`~datasets.Dataset.push_to_hub`.
 
         Returns:
             The URL to the published dataset.
         """
         # Login
         api = hf_hub_login(token=token)
```

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/step_background.py` & `datadreamer_dev-0.9.0/datadreamer/steps/step_background.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/step_export.py` & `datadreamer_dev-0.9.0/datadreamer/steps/step_export.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/step_operations.py` & `datadreamer_dev-0.9.0/datadreamer/steps/step_operations.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/step_output.py` & `datadreamer_dev-0.9.0/datadreamer/steps/step_output.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/tasks/cosine_similarity.py` & `datadreamer_dev-0.9.0/datadreamer/steps/tasks/cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/tasks/embed.py` & `datadreamer_dev-0.9.0/datadreamer/steps/tasks/embed.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/tasks/retrieve.py` & `datadreamer_dev-0.9.0/datadreamer/steps/tasks/retrieve.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/steps/tasks/run_task_model.py` & `datadreamer_dev-0.9.0/datadreamer/steps/tasks/run_task_model.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/task_models/__init__.py` & `datadreamer_dev-0.9.0/datadreamer/task_models/__init__.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/task_models/hf_classification_task_model.py` & `datadreamer_dev-0.9.0/datadreamer/task_models/hf_classification_task_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,14 +145,23 @@
     @property
     def model_max_length(self) -> int:  # pragma: no cover
         return get_model_max_context_length(
             model_name=self.model_name, config=self.config
         )
 
     def count_tokens(self, value: str) -> int:
+        """Counts the number of tokens in a string.
+
+        Args:
+            value: The string to count tokens for.
+
+        Returns:
+            The number of tokens in the string.
+        """
+        pass
         return len(self.tokenizer.encode(value))
 
     @torch.no_grad()
     def _run_batch(  # noqa: C901
         self,
         max_length_func: Callable[[list[str]], int],
         inputs: list[str],
```

### Comparing `datadreamer_dev-0.8.0/datadreamer/task_models/parallel_task_model.py` & `datadreamer_dev-0.9.0/datadreamer/task_models/parallel_task_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,23 @@
 
 class ParallelTaskModel(_ParallelCachable, TaskModel):
     def __init__(self, *task_models: TaskModel):
         super().__init__(*task_models, cls=TaskModel)
         self.task_models = cast(list[TaskModel], self.cachables)
 
     def count_tokens(self, value: str) -> int:
+        """Counts the number of tokens in a string.
+
+        Args:
+            value: The string to count tokens for.
+
+        Returns:
+            The number of tokens in the string.
+        """
+        pass
         return self.task_models[0].count_tokens(value=value)
 
     @property
     def model_max_length(self) -> int:  # pragma: no cover
         return self.task_models[0].model_max_length
 
     def run(  # type:ignore[override]
```

### Comparing `datadreamer_dev-0.8.0/datadreamer/task_models/task_model.py` & `datadreamer_dev-0.9.0/datadreamer/task_models/task_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,22 @@
 
 class TaskModel(_Cachable):
     def __init__(self, cache_folder_path: None | str = None):
         super().__init__(cache_folder_path=cache_folder_path)
 
     @abstractmethod
     def count_tokens(self, value: str) -> int:
+        """Counts the number of tokens in a string.
+
+        Args:
+            value: The string to count tokens for.
+
+        Returns:
+            The number of tokens in the string.
+        """
         pass
 
     @property
     @abstractmethod
     def model_max_length(self) -> int:
         pass
```

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/conftest.py` & `datadreamer_dev-0.9.0/datadreamer/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/datasets/test_datasets.py` & `datadreamer_dev-0.9.0/datadreamer/tests/datasets/test_datasets.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/datasets/test_utils.py` & `datadreamer_dev-0.9.0/datadreamer/tests/datasets/test_utils.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/embedders/test_embedders.py` & `datadreamer_dev-0.9.0/datadreamer/tests/embedders/test_embedders.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/llms/test_llms.py` & `datadreamer_dev-0.9.0/datadreamer/tests/llms/test_llms.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/retrievers/test_retrievers.py` & `datadreamer_dev-0.9.0/datadreamer/tests/retrievers/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/steps/prompt/test_prompt.py` & `datadreamer_dev-0.9.0/datadreamer/tests/steps/prompt/test_prompt.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/steps/tasks/test_tasks.py` & `datadreamer_dev-0.9.0/datadreamer/tests/steps/tasks/test_tasks.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/steps/test_data_sources.py` & `datadreamer_dev-0.9.0/datadreamer/tests/steps/test_data_sources.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/steps/test_step.py` & `datadreamer_dev-0.9.0/datadreamer/tests/steps/test_step.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/steps/test_step_background.py` & `datadreamer_dev-0.9.0/datadreamer/tests/steps/test_step_background.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/steps/test_step_export.py` & `datadreamer_dev-0.9.0/datadreamer/tests/steps/test_step_export.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,15 +324,15 @@
 
 class TestPublishToHFHub:
     def test_code_implementation(
         self, create_datadreamer, create_test_step: Callable[..., Step]
     ):
         with create_datadreamer():
             step = create_test_step(name="my-step", inputs=None, output_names=["out1"])
-            assert Hasher.hash(getsource(step.publish_to_hf_hub)) == "f6c09158265ff094"
+            assert Hasher.hash(getsource(step.publish_to_hf_hub)) == "9640479091d9bc18"
 
     @pytest.mark.skip(reason="skipping because requires interactive")
     def test_publish_dataset_to_hf_hub_single_train_split(
         self, create_datadreamer, create_test_step: Callable[..., Step]
     ):
         def setup(self):
             self.register_data_card(DataCardType.DATASET_NAME, "truthful_qa")
```

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/steps/test_step_operations.py` & `datadreamer_dev-0.9.0/datadreamer/tests/steps/test_step_operations.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/steps/test_step_output.py` & `datadreamer_dev-0.9.0/datadreamer/tests/steps/test_step_output.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/task_models/test_task_models.py` & `datadreamer_dev-0.9.0/datadreamer/tests/task_models/test_task_models.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/test_datadreamer.py` & `datadreamer_dev-0.9.0/datadreamer/tests/test_datadreamer.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/test_package.py` & `datadreamer_dev-0.9.0/datadreamer/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/test_utils/fixtures/bitsandbytes_fixture.py` & `datadreamer_dev-0.9.0/datadreamer/tests/test_utils/fixtures/bitsandbytes_fixture.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/test_utils/fixtures/create_datadreamer.py` & `datadreamer_dev-0.9.0/datadreamer/tests/test_utils/fixtures/create_datadreamer.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/test_utils/fixtures/create_test_step.py` & `datadreamer_dev-0.9.0/datadreamer/tests/test_utils/fixtures/create_test_step.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/trainers/test_distributed.py` & `datadreamer_dev-0.9.0/datadreamer/tests/trainers/test_distributed.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/trainers/test_trainers.py` & `datadreamer_dev-0.9.0/datadreamer/tests/trainers/test_trainers.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/tests/utils/test_device_utils.py` & `datadreamer_dev-0.9.0/datadreamer/tests/utils/test_device_utils.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/trainers/__init__.py` & `datadreamer_dev-0.9.0/datadreamer/trainers/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -32,14 +32,35 @@
 
 Parameter-Efficient Training 
 ----------------------------
 See the
 `Parameter-Efficient Training <pages/advanced_usage/parameter_efficient_training.html>`_
 page.
 
+Configuring Training
+====================
+
+You can make use of ``**kwargs`` to pass in additional keyword arguments to the
+underlying model's training method.
+
+.. dropdown:: Configuring Early Stopping
+
+    To override the default early stopping, pass in the ``early_stopping_patience``
+    parameter and the ``early_stopping_threshold`` parameter. To disable early stopping,
+    set ``early_stopping_patience`` to ``None``.
+
+    See :py:class:`~transformers.EarlyStoppingCallback` for more details.
+
+.. dropdown:: Advanced Configuration
+
+    Most configuration you need can be done by passing ``**kwargs``. However, if you need
+    more advanced configuration, you can subclass the trainer class and override as
+    needed or :doc:`create your own trainer
+    <pages/advanced_usage/creating_a_new_datadreamer_.../trainer>`.
+
 Model Card Generation
 =====================
 An automatically generated model card can be viewed by calling
 :py:meth:`~Trainer.model_card`. The model card can be helpful for reproducibility and
 for sharing your work with others when published alongside your code. When
 `publishing models <#exporting-and-publishing-models>`_, the model card will be
 published alongside the model.
```

### Comparing `datadreamer_dev-0.8.0/datadreamer/trainers/_train_hf_base.py` & `datadreamer_dev-0.9.0/datadreamer/trainers/_train_hf_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1306,14 +1306,23 @@
     @property
     def model_path(self) -> str:  # type:ignore[return]
         """The path to the trained model after training."""
         if self.model:
             return os.path.join(self._output_folder_path, "_model")
 
     def export_to_disk(self, path: str, adapter_only: bool = False) -> PreTrainedModel:
+        """Export the trained model to disk.
+
+        Args:
+            path: The path to export the model to.
+            adapter_only: Whether to export only the adapter.
+
+        Returns:
+            The exported model.
+        """
         from .train_hf_finetune import TrainHFFineTune
         from .train_setfit_classifier import TrainSetFitClassifier
 
         assert (
             not adapter_only or self.peft_config
         ), "`adapter_only` can only be used if a `peft_config` was provided."
 
@@ -1425,14 +1434,30 @@
         branch: None | str = None,
         private: bool = False,
         token: None | str = None,
         adapter_only: bool = False,
         is_synthetic: bool = True,
         **kwargs,
     ) -> str:  # pragma: no cover
+        """Publish the model to the Hugging Face Hub.
+
+        Args:
+            repo_id: The repository ID to publish the model to.
+            branch: The branch to push the model to.
+            private: Whether to make the model private.
+            token: The Hugging Face API token to use for authentication.
+            adapter_only: Whether to publish only the adapter.
+            is_synthetic: Whether the dataset is synthetic (applies certain metadata
+                when publishing).
+            **kwargs: Additional keyword arguments to pass to
+                :py:meth:`~transformers.PreTrainedModel.push_to_hub`.
+
+        Returns:
+            The URL to the published model.
+        """
         from .train_hf_finetune import TrainHFFineTune
         from .train_setfit_classifier import TrainSetFitClassifier
 
         assert (
             not adapter_only or self.peft_config
         ), "`adapter_only` can only be used if a `peft_config` was provided."
```

### Comparing `datadreamer_dev-0.8.0/datadreamer/trainers/_vendored/_dpo_helper.py` & `datadreamer_dev-0.9.0/datadreamer/trainers/_vendored/_dpo_helper.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/trainers/_vendored/_sentence_transformer_helper.py` & `datadreamer_dev-0.9.0/datadreamer/trainers/_vendored/_sentence_transformer_helper.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/trainers/_vendored/_setfit_helper.py` & `datadreamer_dev-0.9.0/datadreamer/trainers/_vendored/_setfit_helper.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/trainers/_vendored/dpo_trainer.py` & `datadreamer_dev-0.9.0/datadreamer/trainers/_vendored/dpo_trainer.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/trainers/train_hf_classifier.py` & `datadreamer_dev-0.9.0/datadreamer/trainers/train_hf_classifier.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/trainers/train_hf_dpo.py` & `datadreamer_dev-0.9.0/datadreamer/trainers/train_hf_dpo.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/trainers/train_hf_finetune.py` & `datadreamer_dev-0.9.0/datadreamer/trainers/train_hf_finetune.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/trainers/train_hf_ppo.py` & `datadreamer_dev-0.9.0/datadreamer/trainers/train_hf_ppo.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/trainers/train_hf_reward_model.py` & `datadreamer_dev-0.9.0/datadreamer/trainers/train_hf_reward_model.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/trainers/train_openai_finetune.py` & `datadreamer_dev-0.9.0/datadreamer/trainers/train_openai_finetune.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,21 +73,40 @@
         return OpenAI.client.func(self)  # type: ignore[attr-defined]
 
     @cached_property
     def tokenizer(self) -> Encoding:
         return OpenAI.tokenizer.func(self)  # type: ignore[attr-defined]
 
     @ring.lru(maxsize=128)
-    def get_max_context_length(self, max_new_tokens: int) -> int:  # pragma: no cover
+    def get_max_context_length(self, max_new_tokens: int) -> int:
+        """Gets the maximum context length for the model. When ``max_new_tokens`` is
+        greater than 0, the maximum number of tokens that can be used for the prompt
+        context is returned.
+
+        Args:
+            max_new_tokens: The maximum number of tokens that can be generated.
+
+        Returns:
+            The maximum context length.
+        """  # pragma: no cover
         return OpenAI.get_max_context_length._callable.wrapped_callable(
             self, max_new_tokens
         )
 
     @ring.lru(maxsize=5000)
     def count_tokens(self, value: str) -> int:
+        """Counts the number of tokens in a string.
+
+        Args:
+            value: The string to count tokens for.
+
+        Returns:
+            The number of tokens in the string.
+        """
+        pass
         return OpenAI.count_tokens._callable.wrapped_callable(self, value)
 
     def _train(  # type:ignore[override] # noqa: C901
         self,
         train_input: OutputDatasetColumn | OutputIterableDatasetColumn,
         train_output: OutputDatasetColumn | OutputIterableDatasetColumn,
         validation_input: OutputDatasetColumn | OutputIterableDatasetColumn,
```

### Comparing `datadreamer_dev-0.8.0/datadreamer/trainers/train_sentence_transformer.py` & `datadreamer_dev-0.9.0/datadreamer/trainers/train_sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/trainers/train_setfit_classifier.py` & `datadreamer_dev-0.9.0/datadreamer/trainers/train_setfit_classifier.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/trainers/trainer.py` & `datadreamer_dev-0.9.0/datadreamer/trainers/trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,14 +79,22 @@
     def __init__(  # noqa: C901
         self,
         name: str,
         force: bool = False,
         verbose: None | bool = None,
         log_level: None | int = None,
     ):
+        """Base class for all trainers.
+
+        Args:
+            name: The name of the trainer.
+            force: Whether to force run the trainer (ignore saved results).
+            verbose: Whether or not to print verbose logs.
+            log_level: The logging level to use (:py:data:`~logging.DEBUG`, :py:data:`~logging.INFO`, etc.).
+        """
         if not DataDreamer.initialized() or DataDreamer.is_running_in_memory():
             raise RuntimeError("Trainers only be run within DataDreamer() context.")
 
         # Check pid
         if DataDreamer.is_background_process():  # pragma: no cover
             raise RuntimeError(
                 f"Trainers must be initialized in the same process"
@@ -301,14 +309,15 @@
 
     @abstractmethod
     def _train(self):
         pass
 
     @abstractmethod
     def train(self) -> "Trainer":
+        """Train the model."""
         pass
 
     @abstractmethod
     def _load(self, with_optimizations: bool = True):
         pass
 
     @property
@@ -320,14 +329,15 @@
         if self._model is None:  # pragma: no cover
             self._model = self._load()
         return self._model
 
     @property
     @abstractmethod
     def model_path(self) -> str:
+        """The path to the trained model after training."""
         pass
 
     @property
     @abstractmethod
     def base_model_card(self) -> None | str:
         return None
 
@@ -366,14 +376,15 @@
         return {
             "model_card": sort_data_card(model_card),
             "data_card": data_card,
             **orig_step_metadata,
         }
 
     def model_card(self):
+        """Print the data card for the step."""
         print(json.dumps(self._model_card, indent=4))
 
     @property
     def version(self) -> float:  # pragma: no cover
         return 1.0
 
     @cached_property
```

### Comparing `datadreamer_dev-0.8.0/datadreamer/utils/background_utils.py` & `datadreamer_dev-0.9.0/datadreamer/utils/background_utils.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/utils/collection_utils.py` & `datadreamer_dev-0.9.0/datadreamer/utils/collection_utils.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/utils/device_utils.py` & `datadreamer_dev-0.9.0/datadreamer/utils/device_utils.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/utils/distributed_utils.py` & `datadreamer_dev-0.9.0/datadreamer/utils/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/utils/fingerprint_utils.py` & `datadreamer_dev-0.9.0/datadreamer/utils/fingerprint_utils.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/utils/fs_utils.py` & `datadreamer_dev-0.9.0/datadreamer/utils/fs_utils.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/utils/hf_chat_prompt_templates.py` & `datadreamer_dev-0.9.0/datadreamer/utils/hf_chat_prompt_templates.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/utils/hf_hub_utils.py` & `datadreamer_dev-0.9.0/datadreamer/utils/hf_hub_utils.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/utils/hf_model_utils.py` & `datadreamer_dev-0.9.0/datadreamer/utils/hf_model_utils.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/utils/import_utils.py` & `datadreamer_dev-0.9.0/datadreamer/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/utils/str_utils.py` & `datadreamer_dev-0.9.0/datadreamer/utils/str_utils.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/datadreamer/utils/time_utils.py` & `datadreamer_dev-0.9.0/datadreamer/utils/time_utils.py`

 * *Files identical despite different names*

### Comparing `datadreamer_dev-0.8.0/pyproject.toml` & `datadreamer_dev-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datadreamer.dev"
-version = "0.8.0"
+version = "0.9.0"
 description = "Prompt. Generate Synthetic Data. Train & Align Models."
 license = "MIT"
 authors= [
     "Ajay Patel <me@ajayp.app>"
 ]
 maintainers = [
     "Ajay Patel <me@ajayp.app>"
```

### Comparing `datadreamer_dev-0.8.0/PKG-INFO` & `datadreamer_dev-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadreamer.dev
-Version: 0.8.0
+Version: 0.9.0
 Summary: Prompt. Generate Synthetic Data. Train & Align Models.
 Home-page: https://datadreamer.dev/
 License: MIT
 Keywords: python,nlp,machine learning,natural language processing,deep learning,transformers,pytorch,openai,alignment,gpt,nlp library,synthetic data,fine-tuning,synthetic dataset generation,llm,llms,llmops,instruction-tuning
 Author: Ajay Patel
 Author-email: me@ajayp.app
 Maintainer: Ajay Patel
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datadreamer.dev Version: 0.8.0 Summary: Prompt.
+Metadata-Version: 2.1 Name: datadreamer.dev Version: 0.9.0 Summary: Prompt.
 Generate Synthetic Data. Train & Align Models. Home-page: https://
 datadreamer.dev/ License: MIT Keywords: python,nlp,machine learning,natural
 language processing,deep learning,transformers,pytorch,openai,alignment,gpt,nlp
 library,synthetic data,fine-tuning,synthetic dataset
 generation,llm,llms,llmops,instruction-tuning Author: Ajay Patel Author-email:
 me@ajayp.app Maintainer: Ajay Patel Maintainer-email: me@ajayp.app Requires-
 Python: >=3.10,<3.14 Classifier: Development Status :: 5 - Production/Stable
```

