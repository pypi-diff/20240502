# Comparing `tmp/openai-1.8.0.tar.gz` & `tmp/openai-1.9.0.tar.gz`

## Comparing `openai-1.8.0.tar` & `openai-1.9.0.tar`

### file list

```diff
@@ -1,194 +1,194 @@
--rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/__main__.py
--rw-r--r--   0        0        0    60768 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_base_client.py
--rw-r--r--   0        0        0    20141 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_client.py
--rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_compat.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_constants.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_exceptions.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_files.py
--rw-r--r--   0        0        0    13979 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_legacy_response.py
--rw-r--r--   0        0        0    16410 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_models.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_module_client.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_qs.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_resource.py
--rw-r--r--   0        0        0    26474 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_response.py
--rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_streaming.py
--rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_types.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_version.py
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/pagination.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/py.typed
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/version.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_extras/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_extras/_common.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_extras/numpy_proxy.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_extras/pandas_proxy.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_utils/__init__.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_utils/_logs.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_utils/_streams.py
--rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_utils/_transform.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_utils/_typing.py
--rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/_utils/_utils.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/cli/__init__.py
--rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/cli/_cli.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/cli/_errors.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/cli/_models.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/cli/_progress.py
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/cli/_utils.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/cli/_api/__init__.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/cli/_api/_main.py
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/cli/_api/audio.py
--rw-r--r--   0        0        0     6412 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/cli/_api/completions.py
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/cli/_api/files.py
--rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/cli/_api/image.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/cli/_api/models.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/cli/_api/chat/__init__.py
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/cli/_api/chat/completions.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/cli/_tools/__init__.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/cli/_tools/_main.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/cli/_tools/fine_tunes.py
--rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/cli/_tools/migrate.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/lib/.keep
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/lib/_old_api.py
--rw-r--r--   0        0        0    35189 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/lib/_validators.py
--rw-r--r--   0        0        0    20924 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/lib/azure.py
--rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/__init__.py
--rw-r--r--   0        0        0    56316 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/completions.py
--rw-r--r--   0        0        0     9887 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/embeddings.py
--rw-r--r--   0        0        0    25880 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/files.py
--rw-r--r--   0        0        0    24035 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/images.py
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/models.py
--rw-r--r--   0        0        0     6412 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/moderations.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/audio/__init__.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/audio/audio.py
--rw-r--r--   0        0        0     7411 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/audio/speech.py
--rw-r--r--   0        0        0     9509 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/audio/transcriptions.py
--rw-r--r--   0        0        0     8633 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/audio/translations.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/beta/__init__.py
--rw-r--r--   0        0        0     2628 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/beta/beta.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/beta/assistants/__init__.py
--rw-r--r--   0        0        0    30159 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/beta/assistants/assistants.py
--rw-r--r--   0        0        0    19316 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/beta/assistants/files.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/beta/threads/__init__.py
--rw-r--r--   0        0        0    24537 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/beta/threads/threads.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/beta/threads/messages/__init__.py
--rw-r--r--   0        0        0    12151 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/beta/threads/messages/files.py
--rw-r--r--   0        0        0    22405 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/beta/threads/messages/messages.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/beta/threads/runs/__init__.py
--rw-r--r--   0        0        0    31864 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/beta/threads/runs/runs.py
--rw-r--r--   0        0        0    12025 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/beta/threads/runs/steps.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/chat/__init__.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/chat/chat.py
--rw-r--r--   0        0        0    70284 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/chat/completions.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/fine_tuning/__init__.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/fine_tuning/fine_tuning.py
--rw-r--r--   0        0        0    24347 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/resources/fine_tuning/jobs.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/__init__.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/completion.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/completion_choice.py
--rw-r--r--   0        0        0     7201 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/completion_create_params.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/completion_usage.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/create_embedding_response.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/embedding.py
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/embedding_create_params.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/file_content.py
--rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/file_create_params.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/file_deleted.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/file_list_params.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/file_object.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/image.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/image_create_variation_params.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/image_edit_params.py
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/image_generate_params.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/images_response.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/model.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/model_deleted.py
--rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/moderation.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/moderation_create_params.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/moderation_create_response.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/audio/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/audio/speech_create_params.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/audio/transcription.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/audio/transcription_create_params.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/audio/translation.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/audio/translation_create_params.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/__init__.py
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/assistant.py
--rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/assistant_create_params.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/assistant_deleted.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/assistant_list_params.py
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/assistant_update_params.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/thread.py
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/thread_create_and_run_params.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/thread_create_params.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/thread_deleted.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/thread_update_params.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/assistants/__init__.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/assistants/assistant_file.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/assistants/file_create_params.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/assistants/file_delete_response.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/assistants/file_list_params.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/chat/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/__init__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/message_content_image_file.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/message_content_text.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/message_create_params.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/message_list_params.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/message_update_params.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/required_action_function_tool_call.py
--rw-r--r--   0        0        0     4500 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/run.py
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/run_create_params.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/run_list_params.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/run_submit_tool_outputs_params.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/run_update_params.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/thread_message.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/messages/__init__.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/messages/file_list_params.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/messages/message_file.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/runs/__init__.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/runs/code_tool_call.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/runs/function_tool_call.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/runs/message_creation_step_details.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/runs/retrieval_tool_call.py
--rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/runs/run_step.py
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/runs/step_list_params.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/beta/threads/runs/tool_calls_step_details.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/chat_completion.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/chat_completion_assistant_message_param.py
--rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/chat_completion_chunk.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/chat_completion_content_part_image_param.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/chat_completion_content_part_param.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/chat_completion_content_part_text_param.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/chat_completion_function_call_option_param.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/chat_completion_function_message_param.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/chat_completion_message.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/chat_completion_message_param.py
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/chat_completion_message_tool_call.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/chat_completion_message_tool_call_param.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/chat_completion_named_tool_choice_param.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/chat_completion_role.py
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/chat_completion_system_message_param.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/chat_completion_token_logprob.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/chat_completion_tool_choice_option_param.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/chat_completion_tool_message_param.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/chat_completion_tool_param.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/chat_completion_user_message_param.py
--rw-r--r--   0        0        0    10362 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/chat/completion_create_params.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/fine_tuning/__init__.py
--rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/fine_tuning/fine_tuning_job.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/fine_tuning/fine_tuning_job_event.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/fine_tuning/job_create_params.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/fine_tuning/job_list_events_params.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/fine_tuning/job_list_params.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/shared/__init__.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/shared/function_definition.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/shared/function_parameters.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/shared_params/__init__.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/shared_params/function_definition.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 openai-1.8.0/src/openai/types/shared_params/function_parameters.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 openai-1.8.0/.gitignore
--rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 openai-1.8.0/LICENSE
--rw-r--r--   0        0        0    17310 2020-02-02 00:00:00.000000 openai-1.8.0/README.md
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 openai-1.8.0/pyproject.toml
--rw-r--r--   0        0        0    18884 2020-02-02 00:00:00.000000 openai-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     9092 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/__main__.py
+-rw-r--r--   0        0        0    61285 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_base_client.py
+-rw-r--r--   0        0        0    20141 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_client.py
+-rw-r--r--   0        0        0     5113 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_compat.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_constants.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_exceptions.py
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_files.py
+-rw-r--r--   0        0        0    13979 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_legacy_response.py
+-rw-r--r--   0        0        0    16410 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_models.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_module_client.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_qs.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_resource.py
+-rw-r--r--   0        0        0    26474 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_response.py
+-rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_streaming.py
+-rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_types.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_version.py
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/pagination.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/py.typed
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/version.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_extras/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_extras/_common.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_extras/numpy_proxy.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_extras/pandas_proxy.py
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_utils/__init__.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_utils/_logs.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_utils/_streams.py
+-rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_utils/_transform.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_utils/_typing.py
+-rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/_utils/_utils.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/cli/__init__.py
+-rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/cli/_cli.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/cli/_errors.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/cli/_models.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/cli/_progress.py
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/cli/_utils.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/cli/_api/__init__.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/cli/_api/_main.py
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/cli/_api/audio.py
+-rw-r--r--   0        0        0     6412 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/cli/_api/completions.py
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/cli/_api/files.py
+-rw-r--r--   0        0        0     4711 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/cli/_api/image.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/cli/_api/models.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/cli/_api/chat/__init__.py
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/cli/_api/chat/completions.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/cli/_tools/__init__.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/cli/_tools/_main.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/cli/_tools/fine_tunes.py
+-rw-r--r--   0        0        0     4895 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/cli/_tools/migrate.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/lib/.keep
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/lib/_old_api.py
+-rw-r--r--   0        0        0    35189 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/lib/_validators.py
+-rw-r--r--   0        0        0    20924 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/lib/azure.py
+-rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/__init__.py
+-rw-r--r--   0        0        0    56480 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/completions.py
+-rw-r--r--   0        0        0    10043 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/embeddings.py
+-rw-r--r--   0        0        0    25996 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/files.py
+-rw-r--r--   0        0        0    24159 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/images.py
+-rw-r--r--   0        0        0    10150 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/models.py
+-rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/moderations.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/audio/__init__.py
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/audio/audio.py
+-rw-r--r--   0        0        0     7535 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/audio/speech.py
+-rw-r--r--   0        0        0     9697 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/audio/transcriptions.py
+-rw-r--r--   0        0        0     8805 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/audio/translations.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/beta/__init__.py
+-rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/beta/beta.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/beta/assistants/__init__.py
+-rw-r--r--   0        0        0    30601 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/beta/assistants/assistants.py
+-rw-r--r--   0        0        0    19432 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/beta/assistants/files.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/beta/threads/__init__.py
+-rw-r--r--   0        0        0    25253 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/beta/threads/threads.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/beta/threads/messages/__init__.py
+-rw-r--r--   0        0        0    12267 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/beta/threads/messages/files.py
+-rw-r--r--   0        0        0    22831 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/beta/threads/messages/messages.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/beta/threads/runs/__init__.py
+-rw-r--r--   0        0        0    32258 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/beta/threads/runs/runs.py
+-rw-r--r--   0        0        0    12141 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/beta/threads/runs/steps.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/chat/__init__.py
+-rw-r--r--   0        0        0     2309 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/chat/chat.py
+-rw-r--r--   0        0        0    70448 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/chat/completions.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/fine_tuning/__init__.py
+-rw-r--r--   0        0        0     2338 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/fine_tuning/fine_tuning.py
+-rw-r--r--   0        0        0    24455 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/resources/fine_tuning/jobs.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/__init__.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/completion.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/completion_choice.py
+-rw-r--r--   0        0        0     7201 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/completion_create_params.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/completion_usage.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/create_embedding_response.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/embedding.py
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/embedding_create_params.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/file_content.py
+-rw-r--r--   0        0        0      840 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/file_create_params.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/file_deleted.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/file_list_params.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/file_object.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/image.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/image_create_variation_params.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/image_edit_params.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/image_generate_params.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/images_response.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/model.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/model_deleted.py
+-rw-r--r--   0        0        0     3946 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/moderation.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/moderation_create_params.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/moderation_create_response.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/audio/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/audio/speech_create_params.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/audio/transcription.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/audio/transcription_create_params.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/audio/translation.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/audio/translation_create_params.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/__init__.py
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/assistant.py
+-rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/assistant_create_params.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/assistant_deleted.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/assistant_list_params.py
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/assistant_update_params.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/thread.py
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/thread_create_and_run_params.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/thread_create_params.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/thread_deleted.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/thread_update_params.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/assistants/__init__.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/assistants/assistant_file.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/assistants/file_create_params.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/assistants/file_delete_response.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/assistants/file_list_params.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/chat/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/__init__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/message_content_image_file.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/message_content_text.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/message_create_params.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/message_list_params.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/message_update_params.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/required_action_function_tool_call.py
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/run.py
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/run_create_params.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/run_list_params.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/run_submit_tool_outputs_params.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/run_update_params.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/thread_message.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/messages/__init__.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/messages/file_list_params.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/messages/message_file.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/runs/__init__.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/runs/code_tool_call.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/runs/function_tool_call.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/runs/message_creation_step_details.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/runs/retrieval_tool_call.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/runs/run_step.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/runs/step_list_params.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/beta/threads/runs/tool_calls_step_details.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/chat_completion.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/chat_completion_assistant_message_param.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/chat_completion_chunk.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/chat_completion_content_part_image_param.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/chat_completion_content_part_param.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/chat_completion_content_part_text_param.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/chat_completion_function_call_option_param.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/chat_completion_function_message_param.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/chat_completion_message.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/chat_completion_message_param.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/chat_completion_message_tool_call.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/chat_completion_message_tool_call_param.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/chat_completion_named_tool_choice_param.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/chat_completion_role.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/chat_completion_system_message_param.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/chat_completion_token_logprob.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/chat_completion_tool_choice_option_param.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/chat_completion_tool_message_param.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/chat_completion_tool_param.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/chat_completion_user_message_param.py
+-rw-r--r--   0        0        0    10362 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/chat/completion_create_params.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/fine_tuning/__init__.py
+-rw-r--r--   0        0        0     3312 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/fine_tuning/fine_tuning_job.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/fine_tuning/fine_tuning_job_event.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/fine_tuning/job_create_params.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/fine_tuning/job_list_events_params.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/fine_tuning/job_list_params.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/shared/__init__.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/shared/function_definition.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/shared/function_parameters.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/shared_params/__init__.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/shared_params/function_definition.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 openai-1.9.0/src/openai/types/shared_params/function_parameters.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 openai-1.9.0/.gitignore
+-rw-r--r--   0        0        0    11336 2020-02-02 00:00:00.000000 openai-1.9.0/LICENSE
+-rw-r--r--   0        0        0    17310 2020-02-02 00:00:00.000000 openai-1.9.0/README.md
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 openai-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0    18884 2020-02-02 00:00:00.000000 openai-1.9.0/PKG-INFO
```

### Comparing `openai-1.8.0/src/openai/__init__.py` & `openai-1.9.0/src/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/_base_client.py` & `openai-1.9.0/src/openai/_base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,17 @@
     BaseAPIResponse,
     AsyncAPIResponse,
     extract_response_type,
 )
 from ._constants import (
     DEFAULT_LIMITS,
     DEFAULT_TIMEOUT,
+    MAX_RETRY_DELAY,
     DEFAULT_MAX_RETRIES,
+    INITIAL_RETRY_DELAY,
     RAW_RESPONSE_HEADER,
     OVERRIDE_CAST_TO_HEADER,
 )
 from ._streaming import Stream, AsyncStream
 from ._exceptions import (
     APIStatusError,
     APITimeoutError,
@@ -586,55 +588,65 @@
     @base_url.setter
     def base_url(self, url: URL | str) -> None:
         self._base_url = self._enforce_trailing_slash(url if isinstance(url, URL) else URL(url))
 
     def platform_headers(self) -> Dict[str, str]:
         return platform_headers(self._version)
 
+    def _parse_retry_after_header(self, response_headers: Optional[httpx.Headers] = None) -> float | None:
+        """Returns a float of the number of seconds (not milliseconds) to wait after retrying, or None if unspecified.
+
+        About the Retry-After header: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Retry-After
+        See also  https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Retry-After#syntax
+        """
+        if response_headers is None:
+            return None
+
+        # First, try the non-standard `retry-after-ms` header for milliseconds,
+        # which is more precise than integer-seconds `retry-after`
+        try:
+            retry_ms_header = response_headers.get("retry-after-ms", None)
+            return float(retry_ms_header) / 1000
+        except (TypeError, ValueError):
+            pass
+
+        # Next, try parsing `retry-after` header as seconds (allowing nonstandard floats).
+        retry_header = response_headers.get("retry-after")
+        try:
+            # note: the spec indicates that this should only ever be an integer
+            # but if someone sends a float there's no reason for us to not respect it
+            return float(retry_header)
+        except (TypeError, ValueError):
+            pass
+
+        # Last, try parsing `retry-after` as a date.
+        retry_date_tuple = email.utils.parsedate_tz(retry_header)
+        if retry_date_tuple is None:
+            return None
+
+        retry_date = email.utils.mktime_tz(retry_date_tuple)
+        return float(retry_date - time.time())
+
     def _calculate_retry_timeout(
         self,
         remaining_retries: int,
         options: FinalRequestOptions,
         response_headers: Optional[httpx.Headers] = None,
     ) -> float:
         max_retries = options.get_max_retries(self.max_retries)
-        try:
-            # About the Retry-After header: https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Retry-After
-            #
-            # <http-date>". See https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Retry-After#syntax for
-            # details.
-            if response_headers is not None:
-                retry_header = response_headers.get("retry-after")
-                try:
-                    # note: the spec indicates that this should only ever be an integer
-                    # but if someone sends a float there's no reason for us to not respect it
-                    retry_after = float(retry_header)
-                except Exception:
-                    retry_date_tuple = email.utils.parsedate_tz(retry_header)
-                    if retry_date_tuple is None:
-                        retry_after = -1
-                    else:
-                        retry_date = email.utils.mktime_tz(retry_date_tuple)
-                        retry_after = int(retry_date - time.time())
-            else:
-                retry_after = -1
-
-        except Exception:
-            retry_after = -1
 
         # If the API asks us to wait a certain amount of time (and it's a reasonable amount), just do what it says.
-        if 0 < retry_after <= 60:
+        retry_after = self._parse_retry_after_header(response_headers)
+        if retry_after is not None and 0 < retry_after <= 60:
             return retry_after
 
-        initial_retry_delay = 0.5
-        max_retry_delay = 8.0
         nb_retries = max_retries - remaining_retries
 
         # Apply exponential backoff, but not more than the max.
-        sleep_seconds = min(initial_retry_delay * pow(2.0, nb_retries), max_retry_delay)
+        sleep_seconds = min(INITIAL_RETRY_DELAY * pow(2.0, nb_retries), MAX_RETRY_DELAY)
 
         # Apply some jitter, plus-or-minus half a second.
         jitter = 1 - 0.25 * random()
         timeout = sleep_seconds * jitter
         return timeout if timeout >= 0 else 0
 
     def _should_retry(self, response: httpx.Response) -> bool:
```

### Comparing `openai-1.8.0/src/openai/_client.py` & `openai-1.9.0/src/openai/_client.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/_compat.py` & `openai-1.9.0/src/openai/_compat.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/_exceptions.py` & `openai-1.9.0/src/openai/_exceptions.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/_files.py` & `openai-1.9.0/src/openai/_files.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/_legacy_response.py` & `openai-1.9.0/src/openai/_legacy_response.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/_models.py` & `openai-1.9.0/src/openai/_models.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/_module_client.py` & `openai-1.9.0/src/openai/_module_client.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/_qs.py` & `openai-1.9.0/src/openai/_qs.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/_resource.py` & `openai-1.9.0/src/openai/_resource.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/_response.py` & `openai-1.9.0/src/openai/_response.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/_streaming.py` & `openai-1.9.0/src/openai/_streaming.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/_types.py` & `openai-1.9.0/src/openai/_types.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/pagination.py` & `openai-1.9.0/src/openai/pagination.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/_extras/numpy_proxy.py` & `openai-1.9.0/src/openai/_extras/numpy_proxy.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/_extras/pandas_proxy.py` & `openai-1.9.0/src/openai/_extras/pandas_proxy.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/_utils/__init__.py` & `openai-1.9.0/src/openai/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/_utils/_logs.py` & `openai-1.9.0/src/openai/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/_utils/_proxy.py` & `openai-1.9.0/src/openai/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/_utils/_transform.py` & `openai-1.9.0/src/openai/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/_utils/_typing.py` & `openai-1.9.0/src/openai/_utils/_typing.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any, cast
+from typing import Any, TypeVar, cast
 from typing_extensions import Required, Annotated, get_args, get_origin
 
 from .._types import InheritsGeneric
 from .._compat import is_union as _is_union
 
 
 def is_annotated_type(typ: type) -> bool:
@@ -19,14 +19,20 @@
     return _is_union(get_origin(typ))
 
 
 def is_required_type(typ: type) -> bool:
     return get_origin(typ) == Required
 
 
+def is_typevar(typ: type) -> bool:
+    # type ignore is required because type checkers
+    # think this expression will always return False
+    return type(typ) == TypeVar  # type: ignore
+
+
 # Extracts T from Annotated[T, ...] or from Required[Annotated[T, ...]]
 def strip_annotated_type(typ: type) -> type:
     if is_required_type(typ) or is_annotated_type(typ):
         return strip_annotated_type(cast(type, get_args(typ)[0]))
 
     return typ
 
@@ -45,14 +51,23 @@
     This also handles the case where a concrete subclass is given, e.g.
     ```py
     class MyResponse(Foo[bytes]):
         ...
 
     extract_type_var(MyResponse, bases=(Foo,), index=0) -> bytes
     ```
+
+    And where a generic subclass is given:
+    ```py
+    _T = TypeVar('_T')
+    class MyResponse(Foo[_T]):
+        ...
+
+    extract_type_var(MyResponse[bytes], bases=(Foo,), index=0) -> bytes
+    ```
     """
     cls = cast(object, get_origin(typ) or typ)
     if cls in generic_bases:
         # we're given the class directly
         return extract_type_arg(typ, index)
 
     # if a subclass is given
@@ -71,10 +86,22 @@
         if target_base_class is None:
             raise RuntimeError(
                 "Could not find the generic base class;\n"
                 "This should never happen;\n"
                 f"Does {cls} inherit from one of {generic_bases} ?"
             )
 
-        return extract_type_arg(target_base_class, index)
+        extracted = extract_type_arg(target_base_class, index)
+        if is_typevar(extracted):
+            # If the extracted type argument is itself a type variable
+            # then that means the subclass itself is generic, so we have
+            # to resolve the type argument from the class itself, not
+            # the base class.
+            #
+            # Note: if there is more than 1 type argument, the subclass could
+            # change the ordering of the type arguments, this is not currently
+            # supported.
+            return extract_type_arg(typ, index)
+
+        return extracted
 
     raise RuntimeError(f"Could not resolve inner type variable at index {index} for {typ}")
```

### Comparing `openai-1.8.0/src/openai/_utils/_utils.py` & `openai-1.9.0/src/openai/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/cli/_cli.py` & `openai-1.9.0/src/openai/cli/_cli.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/cli/_progress.py` & `openai-1.9.0/src/openai/cli/_progress.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/cli/_utils.py` & `openai-1.9.0/src/openai/cli/_utils.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/cli/_api/audio.py` & `openai-1.9.0/src/openai/cli/_api/audio.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/cli/_api/completions.py` & `openai-1.9.0/src/openai/cli/_api/completions.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/cli/_api/files.py` & `openai-1.9.0/src/openai/cli/_api/files.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/cli/_api/image.py` & `openai-1.9.0/src/openai/cli/_api/image.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/cli/_api/models.py` & `openai-1.9.0/src/openai/cli/_api/models.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/cli/_api/chat/completions.py` & `openai-1.9.0/src/openai/cli/_api/chat/completions.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/cli/_tools/fine_tunes.py` & `openai-1.9.0/src/openai/cli/_tools/fine_tunes.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/cli/_tools/migrate.py` & `openai-1.9.0/src/openai/cli/_tools/migrate.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/lib/_old_api.py` & `openai-1.9.0/src/openai/lib/_old_api.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/lib/_validators.py` & `openai-1.9.0/src/openai/lib/_validators.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/lib/azure.py` & `openai-1.9.0/src/openai/lib/azure.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/resources/__init__.py` & `openai-1.9.0/src/openai/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/resources/completions.py` & `openai-1.9.0/src/openai/resources/completions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1048,31 +1048,39 @@
             stream=stream or False,
             stream_cls=AsyncStream[Completion],
         )
 
 
 class CompletionsWithRawResponse:
     def __init__(self, completions: Completions) -> None:
+        self._completions = completions
+
         self.create = _legacy_response.to_raw_response_wrapper(
             completions.create,
         )
 
 
 class AsyncCompletionsWithRawResponse:
     def __init__(self, completions: AsyncCompletions) -> None:
+        self._completions = completions
+
         self.create = _legacy_response.async_to_raw_response_wrapper(
             completions.create,
         )
 
 
 class CompletionsWithStreamingResponse:
     def __init__(self, completions: Completions) -> None:
+        self._completions = completions
+
         self.create = to_streamed_response_wrapper(
             completions.create,
         )
 
 
 class AsyncCompletionsWithStreamingResponse:
     def __init__(self, completions: AsyncCompletions) -> None:
+        self._completions = completions
+
         self.create = async_to_streamed_response_wrapper(
             completions.create,
         )
```

### Comparing `openai-1.8.0/src/openai/resources/embeddings.py` & `openai-1.9.0/src/openai/resources/embeddings.py`

 * *Files 6% similar despite different names*

```diff
@@ -213,31 +213,39 @@
             ),
             cast_to=CreateEmbeddingResponse,
         )
 
 
 class EmbeddingsWithRawResponse:
     def __init__(self, embeddings: Embeddings) -> None:
+        self._embeddings = embeddings
+
         self.create = _legacy_response.to_raw_response_wrapper(
             embeddings.create,
         )
 
 
 class AsyncEmbeddingsWithRawResponse:
     def __init__(self, embeddings: AsyncEmbeddings) -> None:
+        self._embeddings = embeddings
+
         self.create = _legacy_response.async_to_raw_response_wrapper(
             embeddings.create,
         )
 
 
 class EmbeddingsWithStreamingResponse:
     def __init__(self, embeddings: Embeddings) -> None:
+        self._embeddings = embeddings
+
         self.create = to_streamed_response_wrapper(
             embeddings.create,
         )
 
 
 class AsyncEmbeddingsWithStreamingResponse:
     def __init__(self, embeddings: AsyncEmbeddings) -> None:
+        self._embeddings = embeddings
+
         self.create = async_to_streamed_response_wrapper(
             embeddings.create,
         )
```

### Comparing `openai-1.8.0/src/openai/resources/files.py` & `openai-1.9.0/src/openai/resources/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -576,14 +576,16 @@
                 )
 
         return file
 
 
 class FilesWithRawResponse:
     def __init__(self, files: Files) -> None:
+        self._files = files
+
         self.create = _legacy_response.to_raw_response_wrapper(
             files.create,
         )
         self.retrieve = _legacy_response.to_raw_response_wrapper(
             files.retrieve,
         )
         self.list = _legacy_response.to_raw_response_wrapper(
@@ -600,14 +602,16 @@
                 files.retrieve_content  # pyright: ignore[reportDeprecated],
             )
         )
 
 
 class AsyncFilesWithRawResponse:
     def __init__(self, files: AsyncFiles) -> None:
+        self._files = files
+
         self.create = _legacy_response.async_to_raw_response_wrapper(
             files.create,
         )
         self.retrieve = _legacy_response.async_to_raw_response_wrapper(
             files.retrieve,
         )
         self.list = _legacy_response.async_to_raw_response_wrapper(
@@ -624,14 +628,16 @@
                 files.retrieve_content  # pyright: ignore[reportDeprecated],
             )
         )
 
 
 class FilesWithStreamingResponse:
     def __init__(self, files: Files) -> None:
+        self._files = files
+
         self.create = to_streamed_response_wrapper(
             files.create,
         )
         self.retrieve = to_streamed_response_wrapper(
             files.retrieve,
         )
         self.list = to_streamed_response_wrapper(
@@ -649,14 +655,16 @@
                 files.retrieve_content  # pyright: ignore[reportDeprecated],
             )
         )
 
 
 class AsyncFilesWithStreamingResponse:
     def __init__(self, files: AsyncFiles) -> None:
+        self._files = files
+
         self.create = async_to_streamed_response_wrapper(
             files.create,
         )
         self.retrieve = async_to_streamed_response_wrapper(
             files.retrieve,
         )
         self.list = async_to_streamed_response_wrapper(
```

### Comparing `openai-1.8.0/src/openai/resources/images.py` & `openai-1.9.0/src/openai/resources/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -514,53 +514,61 @@
             ),
             cast_to=ImagesResponse,
         )
 
 
 class ImagesWithRawResponse:
     def __init__(self, images: Images) -> None:
+        self._images = images
+
         self.create_variation = _legacy_response.to_raw_response_wrapper(
             images.create_variation,
         )
         self.edit = _legacy_response.to_raw_response_wrapper(
             images.edit,
         )
         self.generate = _legacy_response.to_raw_response_wrapper(
             images.generate,
         )
 
 
 class AsyncImagesWithRawResponse:
     def __init__(self, images: AsyncImages) -> None:
+        self._images = images
+
         self.create_variation = _legacy_response.async_to_raw_response_wrapper(
             images.create_variation,
         )
         self.edit = _legacy_response.async_to_raw_response_wrapper(
             images.edit,
         )
         self.generate = _legacy_response.async_to_raw_response_wrapper(
             images.generate,
         )
 
 
 class ImagesWithStreamingResponse:
     def __init__(self, images: Images) -> None:
+        self._images = images
+
         self.create_variation = to_streamed_response_wrapper(
             images.create_variation,
         )
         self.edit = to_streamed_response_wrapper(
             images.edit,
         )
         self.generate = to_streamed_response_wrapper(
             images.generate,
         )
 
 
 class AsyncImagesWithStreamingResponse:
     def __init__(self, images: AsyncImages) -> None:
+        self._images = images
+
         self.create_variation = async_to_streamed_response_wrapper(
             images.create_variation,
         )
         self.edit = async_to_streamed_response_wrapper(
             images.edit,
         )
         self.generate = async_to_streamed_response_wrapper(
```

### Comparing `openai-1.8.0/src/openai/resources/models.py` & `openai-1.9.0/src/openai/resources/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,53 +221,61 @@
             ),
             cast_to=ModelDeleted,
         )
 
 
 class ModelsWithRawResponse:
     def __init__(self, models: Models) -> None:
+        self._models = models
+
         self.retrieve = _legacy_response.to_raw_response_wrapper(
             models.retrieve,
         )
         self.list = _legacy_response.to_raw_response_wrapper(
             models.list,
         )
         self.delete = _legacy_response.to_raw_response_wrapper(
             models.delete,
         )
 
 
 class AsyncModelsWithRawResponse:
     def __init__(self, models: AsyncModels) -> None:
+        self._models = models
+
         self.retrieve = _legacy_response.async_to_raw_response_wrapper(
             models.retrieve,
         )
         self.list = _legacy_response.async_to_raw_response_wrapper(
             models.list,
         )
         self.delete = _legacy_response.async_to_raw_response_wrapper(
             models.delete,
         )
 
 
 class ModelsWithStreamingResponse:
     def __init__(self, models: Models) -> None:
+        self._models = models
+
         self.retrieve = to_streamed_response_wrapper(
             models.retrieve,
         )
         self.list = to_streamed_response_wrapper(
             models.list,
         )
         self.delete = to_streamed_response_wrapper(
             models.delete,
         )
 
 
 class AsyncModelsWithStreamingResponse:
     def __init__(self, models: AsyncModels) -> None:
+        self._models = models
+
         self.retrieve = async_to_streamed_response_wrapper(
             models.retrieve,
         )
         self.list = async_to_streamed_response_wrapper(
             models.list,
         )
         self.delete = async_to_streamed_response_wrapper(
```

### Comparing `openai-1.8.0/src/openai/resources/moderations.py` & `openai-1.9.0/src/openai/resources/moderations.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,31 +139,39 @@
             ),
             cast_to=ModerationCreateResponse,
         )
 
 
 class ModerationsWithRawResponse:
     def __init__(self, moderations: Moderations) -> None:
+        self._moderations = moderations
+
         self.create = _legacy_response.to_raw_response_wrapper(
             moderations.create,
         )
 
 
 class AsyncModerationsWithRawResponse:
     def __init__(self, moderations: AsyncModerations) -> None:
+        self._moderations = moderations
+
         self.create = _legacy_response.async_to_raw_response_wrapper(
             moderations.create,
         )
 
 
 class ModerationsWithStreamingResponse:
     def __init__(self, moderations: Moderations) -> None:
+        self._moderations = moderations
+
         self.create = to_streamed_response_wrapper(
             moderations.create,
         )
 
 
 class AsyncModerationsWithStreamingResponse:
     def __init__(self, moderations: AsyncModerations) -> None:
+        self._moderations = moderations
+
         self.create = async_to_streamed_response_wrapper(
             moderations.create,
         )
```

### Comparing `openai-1.8.0/src/openai/resources/audio/__init__.py` & `openai-1.9.0/src/openai/resources/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/resources/audio/audio.py` & `openai-1.9.0/src/openai/resources/audio/audio.py`

 * *Files 24% similar despite different names*

```diff
@@ -74,31 +74,71 @@
     @cached_property
     def with_streaming_response(self) -> AsyncAudioWithStreamingResponse:
         return AsyncAudioWithStreamingResponse(self)
 
 
 class AudioWithRawResponse:
     def __init__(self, audio: Audio) -> None:
-        self.transcriptions = TranscriptionsWithRawResponse(audio.transcriptions)
-        self.translations = TranslationsWithRawResponse(audio.translations)
-        self.speech = SpeechWithRawResponse(audio.speech)
+        self._audio = audio
+
+    @cached_property
+    def transcriptions(self) -> TranscriptionsWithRawResponse:
+        return TranscriptionsWithRawResponse(self._audio.transcriptions)
+
+    @cached_property
+    def translations(self) -> TranslationsWithRawResponse:
+        return TranslationsWithRawResponse(self._audio.translations)
+
+    @cached_property
+    def speech(self) -> SpeechWithRawResponse:
+        return SpeechWithRawResponse(self._audio.speech)
 
 
 class AsyncAudioWithRawResponse:
     def __init__(self, audio: AsyncAudio) -> None:
-        self.transcriptions = AsyncTranscriptionsWithRawResponse(audio.transcriptions)
-        self.translations = AsyncTranslationsWithRawResponse(audio.translations)
-        self.speech = AsyncSpeechWithRawResponse(audio.speech)
+        self._audio = audio
+
+    @cached_property
+    def transcriptions(self) -> AsyncTranscriptionsWithRawResponse:
+        return AsyncTranscriptionsWithRawResponse(self._audio.transcriptions)
+
+    @cached_property
+    def translations(self) -> AsyncTranslationsWithRawResponse:
+        return AsyncTranslationsWithRawResponse(self._audio.translations)
+
+    @cached_property
+    def speech(self) -> AsyncSpeechWithRawResponse:
+        return AsyncSpeechWithRawResponse(self._audio.speech)
 
 
 class AudioWithStreamingResponse:
     def __init__(self, audio: Audio) -> None:
-        self.transcriptions = TranscriptionsWithStreamingResponse(audio.transcriptions)
-        self.translations = TranslationsWithStreamingResponse(audio.translations)
-        self.speech = SpeechWithStreamingResponse(audio.speech)
+        self._audio = audio
+
+    @cached_property
+    def transcriptions(self) -> TranscriptionsWithStreamingResponse:
+        return TranscriptionsWithStreamingResponse(self._audio.transcriptions)
+
+    @cached_property
+    def translations(self) -> TranslationsWithStreamingResponse:
+        return TranslationsWithStreamingResponse(self._audio.translations)
+
+    @cached_property
+    def speech(self) -> SpeechWithStreamingResponse:
+        return SpeechWithStreamingResponse(self._audio.speech)
 
 
 class AsyncAudioWithStreamingResponse:
     def __init__(self, audio: AsyncAudio) -> None:
-        self.transcriptions = AsyncTranscriptionsWithStreamingResponse(audio.transcriptions)
-        self.translations = AsyncTranslationsWithStreamingResponse(audio.translations)
-        self.speech = AsyncSpeechWithStreamingResponse(audio.speech)
+        self._audio = audio
+
+    @cached_property
+    def transcriptions(self) -> AsyncTranscriptionsWithStreamingResponse:
+        return AsyncTranscriptionsWithStreamingResponse(self._audio.transcriptions)
+
+    @cached_property
+    def translations(self) -> AsyncTranslationsWithStreamingResponse:
+        return AsyncTranslationsWithStreamingResponse(self._audio.translations)
+
+    @cached_property
+    def speech(self) -> AsyncSpeechWithStreamingResponse:
+        return AsyncSpeechWithStreamingResponse(self._audio.speech)
```

### Comparing `openai-1.8.0/src/openai/resources/audio/speech.py` & `openai-1.9.0/src/openai/resources/audio/speech.py`

 * *Files 4% similar despite different names*

```diff
@@ -166,33 +166,41 @@
             ),
             cast_to=_legacy_response.HttpxBinaryResponseContent,
         )
 
 
 class SpeechWithRawResponse:
     def __init__(self, speech: Speech) -> None:
+        self._speech = speech
+
         self.create = _legacy_response.to_raw_response_wrapper(
             speech.create,
         )
 
 
 class AsyncSpeechWithRawResponse:
     def __init__(self, speech: AsyncSpeech) -> None:
+        self._speech = speech
+
         self.create = _legacy_response.async_to_raw_response_wrapper(
             speech.create,
         )
 
 
 class SpeechWithStreamingResponse:
     def __init__(self, speech: Speech) -> None:
+        self._speech = speech
+
         self.create = to_custom_streamed_response_wrapper(
             speech.create,
             StreamedBinaryAPIResponse,
         )
 
 
 class AsyncSpeechWithStreamingResponse:
     def __init__(self, speech: AsyncSpeech) -> None:
+        self._speech = speech
+
         self.create = async_to_custom_streamed_response_wrapper(
             speech.create,
             AsyncStreamedBinaryAPIResponse,
         )
```

### Comparing `openai-1.8.0/src/openai/resources/audio/transcriptions.py` & `openai-1.9.0/src/openai/resources/audio/transcriptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -195,31 +195,39 @@
             ),
             cast_to=Transcription,
         )
 
 
 class TranscriptionsWithRawResponse:
     def __init__(self, transcriptions: Transcriptions) -> None:
+        self._transcriptions = transcriptions
+
         self.create = _legacy_response.to_raw_response_wrapper(
             transcriptions.create,
         )
 
 
 class AsyncTranscriptionsWithRawResponse:
     def __init__(self, transcriptions: AsyncTranscriptions) -> None:
+        self._transcriptions = transcriptions
+
         self.create = _legacy_response.async_to_raw_response_wrapper(
             transcriptions.create,
         )
 
 
 class TranscriptionsWithStreamingResponse:
     def __init__(self, transcriptions: Transcriptions) -> None:
+        self._transcriptions = transcriptions
+
         self.create = to_streamed_response_wrapper(
             transcriptions.create,
         )
 
 
 class AsyncTranscriptionsWithStreamingResponse:
     def __init__(self, transcriptions: AsyncTranscriptions) -> None:
+        self._transcriptions = transcriptions
+
         self.create = async_to_streamed_response_wrapper(
             transcriptions.create,
         )
```

### Comparing `openai-1.8.0/src/openai/resources/audio/translations.py` & `openai-1.9.0/src/openai/resources/audio/translations.py`

 * *Files 4% similar despite different names*

```diff
@@ -181,31 +181,39 @@
             ),
             cast_to=Translation,
         )
 
 
 class TranslationsWithRawResponse:
     def __init__(self, translations: Translations) -> None:
+        self._translations = translations
+
         self.create = _legacy_response.to_raw_response_wrapper(
             translations.create,
         )
 
 
 class AsyncTranslationsWithRawResponse:
     def __init__(self, translations: AsyncTranslations) -> None:
+        self._translations = translations
+
         self.create = _legacy_response.async_to_raw_response_wrapper(
             translations.create,
         )
 
 
 class TranslationsWithStreamingResponse:
     def __init__(self, translations: Translations) -> None:
+        self._translations = translations
+
         self.create = to_streamed_response_wrapper(
             translations.create,
         )
 
 
 class AsyncTranslationsWithStreamingResponse:
     def __init__(self, translations: AsyncTranslations) -> None:
+        self._translations = translations
+
         self.create = async_to_streamed_response_wrapper(
             translations.create,
         )
```

### Comparing `openai-1.8.0/src/openai/resources/beta/__init__.py` & `openai-1.9.0/src/openai/resources/beta/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/resources/beta/beta.py` & `openai-1.9.0/src/openai/resources/beta/beta.py`

 * *Files 27% similar despite different names*

```diff
@@ -60,27 +60,55 @@
     @cached_property
     def with_streaming_response(self) -> AsyncBetaWithStreamingResponse:
         return AsyncBetaWithStreamingResponse(self)
 
 
 class BetaWithRawResponse:
     def __init__(self, beta: Beta) -> None:
-        self.assistants = AssistantsWithRawResponse(beta.assistants)
-        self.threads = ThreadsWithRawResponse(beta.threads)
+        self._beta = beta
+
+    @cached_property
+    def assistants(self) -> AssistantsWithRawResponse:
+        return AssistantsWithRawResponse(self._beta.assistants)
+
+    @cached_property
+    def threads(self) -> ThreadsWithRawResponse:
+        return ThreadsWithRawResponse(self._beta.threads)
 
 
 class AsyncBetaWithRawResponse:
     def __init__(self, beta: AsyncBeta) -> None:
-        self.assistants = AsyncAssistantsWithRawResponse(beta.assistants)
-        self.threads = AsyncThreadsWithRawResponse(beta.threads)
+        self._beta = beta
+
+    @cached_property
+    def assistants(self) -> AsyncAssistantsWithRawResponse:
+        return AsyncAssistantsWithRawResponse(self._beta.assistants)
+
+    @cached_property
+    def threads(self) -> AsyncThreadsWithRawResponse:
+        return AsyncThreadsWithRawResponse(self._beta.threads)
 
 
 class BetaWithStreamingResponse:
     def __init__(self, beta: Beta) -> None:
-        self.assistants = AssistantsWithStreamingResponse(beta.assistants)
-        self.threads = ThreadsWithStreamingResponse(beta.threads)
+        self._beta = beta
+
+    @cached_property
+    def assistants(self) -> AssistantsWithStreamingResponse:
+        return AssistantsWithStreamingResponse(self._beta.assistants)
+
+    @cached_property
+    def threads(self) -> ThreadsWithStreamingResponse:
+        return ThreadsWithStreamingResponse(self._beta.threads)
 
 
 class AsyncBetaWithStreamingResponse:
     def __init__(self, beta: AsyncBeta) -> None:
-        self.assistants = AsyncAssistantsWithStreamingResponse(beta.assistants)
-        self.threads = AsyncThreadsWithStreamingResponse(beta.threads)
+        self._beta = beta
+
+    @cached_property
+    def assistants(self) -> AsyncAssistantsWithStreamingResponse:
+        return AsyncAssistantsWithStreamingResponse(self._beta.assistants)
+
+    @cached_property
+    def threads(self) -> AsyncThreadsWithStreamingResponse:
+        return AsyncThreadsWithStreamingResponse(self._beta.threads)
```

### Comparing `openai-1.8.0/src/openai/resources/beta/assistants/__init__.py` & `openai-1.9.0/src/openai/resources/beta/assistants/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/resources/beta/assistants/assistants.py` & `openai-1.9.0/src/openai/resources/beta/assistants/assistants.py`

 * *Files 3% similar despite different names*

```diff
@@ -641,15 +641,15 @@
             ),
             cast_to=AssistantDeleted,
         )
 
 
 class AssistantsWithRawResponse:
     def __init__(self, assistants: Assistants) -> None:
-        self.files = FilesWithRawResponse(assistants.files)
+        self._assistants = assistants
 
         self.create = _legacy_response.to_raw_response_wrapper(
             assistants.create,
         )
         self.retrieve = _legacy_response.to_raw_response_wrapper(
             assistants.retrieve,
         )
@@ -659,18 +659,22 @@
         self.list = _legacy_response.to_raw_response_wrapper(
             assistants.list,
         )
         self.delete = _legacy_response.to_raw_response_wrapper(
             assistants.delete,
         )
 
+    @cached_property
+    def files(self) -> FilesWithRawResponse:
+        return FilesWithRawResponse(self._assistants.files)
+
 
 class AsyncAssistantsWithRawResponse:
     def __init__(self, assistants: AsyncAssistants) -> None:
-        self.files = AsyncFilesWithRawResponse(assistants.files)
+        self._assistants = assistants
 
         self.create = _legacy_response.async_to_raw_response_wrapper(
             assistants.create,
         )
         self.retrieve = _legacy_response.async_to_raw_response_wrapper(
             assistants.retrieve,
         )
@@ -680,18 +684,22 @@
         self.list = _legacy_response.async_to_raw_response_wrapper(
             assistants.list,
         )
         self.delete = _legacy_response.async_to_raw_response_wrapper(
             assistants.delete,
         )
 
+    @cached_property
+    def files(self) -> AsyncFilesWithRawResponse:
+        return AsyncFilesWithRawResponse(self._assistants.files)
+
 
 class AssistantsWithStreamingResponse:
     def __init__(self, assistants: Assistants) -> None:
-        self.files = FilesWithStreamingResponse(assistants.files)
+        self._assistants = assistants
 
         self.create = to_streamed_response_wrapper(
             assistants.create,
         )
         self.retrieve = to_streamed_response_wrapper(
             assistants.retrieve,
         )
@@ -701,18 +709,22 @@
         self.list = to_streamed_response_wrapper(
             assistants.list,
         )
         self.delete = to_streamed_response_wrapper(
             assistants.delete,
         )
 
+    @cached_property
+    def files(self) -> FilesWithStreamingResponse:
+        return FilesWithStreamingResponse(self._assistants.files)
+
 
 class AsyncAssistantsWithStreamingResponse:
     def __init__(self, assistants: AsyncAssistants) -> None:
-        self.files = AsyncFilesWithStreamingResponse(assistants.files)
+        self._assistants = assistants
 
         self.create = async_to_streamed_response_wrapper(
             assistants.create,
         )
         self.retrieve = async_to_streamed_response_wrapper(
             assistants.retrieve,
         )
@@ -721,7 +733,11 @@
         )
         self.list = async_to_streamed_response_wrapper(
             assistants.list,
         )
         self.delete = async_to_streamed_response_wrapper(
             assistants.delete,
         )
+
+    @cached_property
+    def files(self) -> AsyncFilesWithStreamingResponse:
+        return AsyncFilesWithStreamingResponse(self._assistants.files)
```

### Comparing `openai-1.8.0/src/openai/resources/beta/assistants/files.py` & `openai-1.9.0/src/openai/resources/beta/assistants/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,14 +406,16 @@
             ),
             cast_to=FileDeleteResponse,
         )
 
 
 class FilesWithRawResponse:
     def __init__(self, files: Files) -> None:
+        self._files = files
+
         self.create = _legacy_response.to_raw_response_wrapper(
             files.create,
         )
         self.retrieve = _legacy_response.to_raw_response_wrapper(
             files.retrieve,
         )
         self.list = _legacy_response.to_raw_response_wrapper(
@@ -422,14 +424,16 @@
         self.delete = _legacy_response.to_raw_response_wrapper(
             files.delete,
         )
 
 
 class AsyncFilesWithRawResponse:
     def __init__(self, files: AsyncFiles) -> None:
+        self._files = files
+
         self.create = _legacy_response.async_to_raw_response_wrapper(
             files.create,
         )
         self.retrieve = _legacy_response.async_to_raw_response_wrapper(
             files.retrieve,
         )
         self.list = _legacy_response.async_to_raw_response_wrapper(
@@ -438,14 +442,16 @@
         self.delete = _legacy_response.async_to_raw_response_wrapper(
             files.delete,
         )
 
 
 class FilesWithStreamingResponse:
     def __init__(self, files: Files) -> None:
+        self._files = files
+
         self.create = to_streamed_response_wrapper(
             files.create,
         )
         self.retrieve = to_streamed_response_wrapper(
             files.retrieve,
         )
         self.list = to_streamed_response_wrapper(
@@ -454,14 +460,16 @@
         self.delete = to_streamed_response_wrapper(
             files.delete,
         )
 
 
 class AsyncFilesWithStreamingResponse:
     def __init__(self, files: AsyncFiles) -> None:
+        self._files = files
+
         self.create = async_to_streamed_response_wrapper(
             files.create,
         )
         self.retrieve = async_to_streamed_response_wrapper(
             files.retrieve,
         )
         self.list = async_to_streamed_response_wrapper(
```

### Comparing `openai-1.8.0/src/openai/resources/beta/threads/__init__.py` & `openai-1.9.0/src/openai/resources/beta/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/resources/beta/threads/threads.py` & `openai-1.9.0/src/openai/resources/beta/threads/threads.py`

 * *Files 4% similar despite different names*

```diff
@@ -533,16 +533,15 @@
             ),
             cast_to=Run,
         )
 
 
 class ThreadsWithRawResponse:
     def __init__(self, threads: Threads) -> None:
-        self.runs = RunsWithRawResponse(threads.runs)
-        self.messages = MessagesWithRawResponse(threads.messages)
+        self._threads = threads
 
         self.create = _legacy_response.to_raw_response_wrapper(
             threads.create,
         )
         self.retrieve = _legacy_response.to_raw_response_wrapper(
             threads.retrieve,
         )
@@ -552,19 +551,26 @@
         self.delete = _legacy_response.to_raw_response_wrapper(
             threads.delete,
         )
         self.create_and_run = _legacy_response.to_raw_response_wrapper(
             threads.create_and_run,
         )
 
+    @cached_property
+    def runs(self) -> RunsWithRawResponse:
+        return RunsWithRawResponse(self._threads.runs)
+
+    @cached_property
+    def messages(self) -> MessagesWithRawResponse:
+        return MessagesWithRawResponse(self._threads.messages)
+
 
 class AsyncThreadsWithRawResponse:
     def __init__(self, threads: AsyncThreads) -> None:
-        self.runs = AsyncRunsWithRawResponse(threads.runs)
-        self.messages = AsyncMessagesWithRawResponse(threads.messages)
+        self._threads = threads
 
         self.create = _legacy_response.async_to_raw_response_wrapper(
             threads.create,
         )
         self.retrieve = _legacy_response.async_to_raw_response_wrapper(
             threads.retrieve,
         )
@@ -574,19 +580,26 @@
         self.delete = _legacy_response.async_to_raw_response_wrapper(
             threads.delete,
         )
         self.create_and_run = _legacy_response.async_to_raw_response_wrapper(
             threads.create_and_run,
         )
 
+    @cached_property
+    def runs(self) -> AsyncRunsWithRawResponse:
+        return AsyncRunsWithRawResponse(self._threads.runs)
+
+    @cached_property
+    def messages(self) -> AsyncMessagesWithRawResponse:
+        return AsyncMessagesWithRawResponse(self._threads.messages)
+
 
 class ThreadsWithStreamingResponse:
     def __init__(self, threads: Threads) -> None:
-        self.runs = RunsWithStreamingResponse(threads.runs)
-        self.messages = MessagesWithStreamingResponse(threads.messages)
+        self._threads = threads
 
         self.create = to_streamed_response_wrapper(
             threads.create,
         )
         self.retrieve = to_streamed_response_wrapper(
             threads.retrieve,
         )
@@ -596,19 +609,26 @@
         self.delete = to_streamed_response_wrapper(
             threads.delete,
         )
         self.create_and_run = to_streamed_response_wrapper(
             threads.create_and_run,
         )
 
+    @cached_property
+    def runs(self) -> RunsWithStreamingResponse:
+        return RunsWithStreamingResponse(self._threads.runs)
+
+    @cached_property
+    def messages(self) -> MessagesWithStreamingResponse:
+        return MessagesWithStreamingResponse(self._threads.messages)
+
 
 class AsyncThreadsWithStreamingResponse:
     def __init__(self, threads: AsyncThreads) -> None:
-        self.runs = AsyncRunsWithStreamingResponse(threads.runs)
-        self.messages = AsyncMessagesWithStreamingResponse(threads.messages)
+        self._threads = threads
 
         self.create = async_to_streamed_response_wrapper(
             threads.create,
         )
         self.retrieve = async_to_streamed_response_wrapper(
             threads.retrieve,
         )
@@ -617,7 +637,15 @@
         )
         self.delete = async_to_streamed_response_wrapper(
             threads.delete,
         )
         self.create_and_run = async_to_streamed_response_wrapper(
             threads.create_and_run,
         )
+
+    @cached_property
+    def runs(self) -> AsyncRunsWithStreamingResponse:
+        return AsyncRunsWithStreamingResponse(self._threads.runs)
+
+    @cached_property
+    def messages(self) -> AsyncMessagesWithStreamingResponse:
+        return AsyncMessagesWithStreamingResponse(self._threads.messages)
```

### Comparing `openai-1.8.0/src/openai/resources/beta/threads/messages/__init__.py` & `openai-1.9.0/src/openai/resources/beta/threads/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/resources/beta/threads/messages/files.py` & `openai-1.9.0/src/openai/resources/beta/threads/messages/files.py`

 * *Files 3% similar despite different names*

```diff
@@ -262,43 +262,51 @@
             ),
             model=MessageFile,
         )
 
 
 class FilesWithRawResponse:
     def __init__(self, files: Files) -> None:
+        self._files = files
+
         self.retrieve = _legacy_response.to_raw_response_wrapper(
             files.retrieve,
         )
         self.list = _legacy_response.to_raw_response_wrapper(
             files.list,
         )
 
 
 class AsyncFilesWithRawResponse:
     def __init__(self, files: AsyncFiles) -> None:
+        self._files = files
+
         self.retrieve = _legacy_response.async_to_raw_response_wrapper(
             files.retrieve,
         )
         self.list = _legacy_response.async_to_raw_response_wrapper(
             files.list,
         )
 
 
 class FilesWithStreamingResponse:
     def __init__(self, files: Files) -> None:
+        self._files = files
+
         self.retrieve = to_streamed_response_wrapper(
             files.retrieve,
         )
         self.list = to_streamed_response_wrapper(
             files.list,
         )
 
 
 class AsyncFilesWithStreamingResponse:
     def __init__(self, files: AsyncFiles) -> None:
+        self._files = files
+
         self.retrieve = async_to_streamed_response_wrapper(
             files.retrieve,
         )
         self.list = async_to_streamed_response_wrapper(
             files.list,
         )
```

### Comparing `openai-1.8.0/src/openai/resources/beta/threads/messages/messages.py` & `openai-1.9.0/src/openai/resources/beta/threads/messages/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -477,75 +477,91 @@
             ),
             model=ThreadMessage,
         )
 
 
 class MessagesWithRawResponse:
     def __init__(self, messages: Messages) -> None:
-        self.files = FilesWithRawResponse(messages.files)
+        self._messages = messages
 
         self.create = _legacy_response.to_raw_response_wrapper(
             messages.create,
         )
         self.retrieve = _legacy_response.to_raw_response_wrapper(
             messages.retrieve,
         )
         self.update = _legacy_response.to_raw_response_wrapper(
             messages.update,
         )
         self.list = _legacy_response.to_raw_response_wrapper(
             messages.list,
         )
 
+    @cached_property
+    def files(self) -> FilesWithRawResponse:
+        return FilesWithRawResponse(self._messages.files)
+
 
 class AsyncMessagesWithRawResponse:
     def __init__(self, messages: AsyncMessages) -> None:
-        self.files = AsyncFilesWithRawResponse(messages.files)
+        self._messages = messages
 
         self.create = _legacy_response.async_to_raw_response_wrapper(
             messages.create,
         )
         self.retrieve = _legacy_response.async_to_raw_response_wrapper(
             messages.retrieve,
         )
         self.update = _legacy_response.async_to_raw_response_wrapper(
             messages.update,
         )
         self.list = _legacy_response.async_to_raw_response_wrapper(
             messages.list,
         )
 
+    @cached_property
+    def files(self) -> AsyncFilesWithRawResponse:
+        return AsyncFilesWithRawResponse(self._messages.files)
+
 
 class MessagesWithStreamingResponse:
     def __init__(self, messages: Messages) -> None:
-        self.files = FilesWithStreamingResponse(messages.files)
+        self._messages = messages
 
         self.create = to_streamed_response_wrapper(
             messages.create,
         )
         self.retrieve = to_streamed_response_wrapper(
             messages.retrieve,
         )
         self.update = to_streamed_response_wrapper(
             messages.update,
         )
         self.list = to_streamed_response_wrapper(
             messages.list,
         )
 
+    @cached_property
+    def files(self) -> FilesWithStreamingResponse:
+        return FilesWithStreamingResponse(self._messages.files)
+
 
 class AsyncMessagesWithStreamingResponse:
     def __init__(self, messages: AsyncMessages) -> None:
-        self.files = AsyncFilesWithStreamingResponse(messages.files)
+        self._messages = messages
 
         self.create = async_to_streamed_response_wrapper(
             messages.create,
         )
         self.retrieve = async_to_streamed_response_wrapper(
             messages.retrieve,
         )
         self.update = async_to_streamed_response_wrapper(
             messages.update,
         )
         self.list = async_to_streamed_response_wrapper(
             messages.list,
         )
+
+    @cached_property
+    def files(self) -> AsyncFilesWithStreamingResponse:
+        return AsyncFilesWithStreamingResponse(self._messages.files)
```

### Comparing `openai-1.8.0/src/openai/resources/beta/threads/runs/__init__.py` & `openai-1.9.0/src/openai/resources/beta/threads/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/resources/beta/threads/runs/runs.py` & `openai-1.9.0/src/openai/resources/beta/threads/runs/runs.py`

 * *Files 1% similar despite different names*

```diff
@@ -677,15 +677,15 @@
             ),
             cast_to=Run,
         )
 
 
 class RunsWithRawResponse:
     def __init__(self, runs: Runs) -> None:
-        self.steps = StepsWithRawResponse(runs.steps)
+        self._runs = runs
 
         self.create = _legacy_response.to_raw_response_wrapper(
             runs.create,
         )
         self.retrieve = _legacy_response.to_raw_response_wrapper(
             runs.retrieve,
         )
@@ -698,18 +698,22 @@
         self.cancel = _legacy_response.to_raw_response_wrapper(
             runs.cancel,
         )
         self.submit_tool_outputs = _legacy_response.to_raw_response_wrapper(
             runs.submit_tool_outputs,
         )
 
+    @cached_property
+    def steps(self) -> StepsWithRawResponse:
+        return StepsWithRawResponse(self._runs.steps)
+
 
 class AsyncRunsWithRawResponse:
     def __init__(self, runs: AsyncRuns) -> None:
-        self.steps = AsyncStepsWithRawResponse(runs.steps)
+        self._runs = runs
 
         self.create = _legacy_response.async_to_raw_response_wrapper(
             runs.create,
         )
         self.retrieve = _legacy_response.async_to_raw_response_wrapper(
             runs.retrieve,
         )
@@ -722,18 +726,22 @@
         self.cancel = _legacy_response.async_to_raw_response_wrapper(
             runs.cancel,
         )
         self.submit_tool_outputs = _legacy_response.async_to_raw_response_wrapper(
             runs.submit_tool_outputs,
         )
 
+    @cached_property
+    def steps(self) -> AsyncStepsWithRawResponse:
+        return AsyncStepsWithRawResponse(self._runs.steps)
+
 
 class RunsWithStreamingResponse:
     def __init__(self, runs: Runs) -> None:
-        self.steps = StepsWithStreamingResponse(runs.steps)
+        self._runs = runs
 
         self.create = to_streamed_response_wrapper(
             runs.create,
         )
         self.retrieve = to_streamed_response_wrapper(
             runs.retrieve,
         )
@@ -746,18 +754,22 @@
         self.cancel = to_streamed_response_wrapper(
             runs.cancel,
         )
         self.submit_tool_outputs = to_streamed_response_wrapper(
             runs.submit_tool_outputs,
         )
 
+    @cached_property
+    def steps(self) -> StepsWithStreamingResponse:
+        return StepsWithStreamingResponse(self._runs.steps)
+
 
 class AsyncRunsWithStreamingResponse:
     def __init__(self, runs: AsyncRuns) -> None:
-        self.steps = AsyncStepsWithStreamingResponse(runs.steps)
+        self._runs = runs
 
         self.create = async_to_streamed_response_wrapper(
             runs.create,
         )
         self.retrieve = async_to_streamed_response_wrapper(
             runs.retrieve,
         )
@@ -769,7 +781,11 @@
         )
         self.cancel = async_to_streamed_response_wrapper(
             runs.cancel,
         )
         self.submit_tool_outputs = async_to_streamed_response_wrapper(
             runs.submit_tool_outputs,
         )
+
+    @cached_property
+    def steps(self) -> AsyncStepsWithStreamingResponse:
+        return AsyncStepsWithStreamingResponse(self._runs.steps)
```

### Comparing `openai-1.8.0/src/openai/resources/beta/threads/runs/steps.py` & `openai-1.9.0/src/openai/resources/beta/threads/runs/steps.py`

 * *Files 2% similar despite different names*

```diff
@@ -260,43 +260,51 @@
             ),
             model=RunStep,
         )
 
 
 class StepsWithRawResponse:
     def __init__(self, steps: Steps) -> None:
+        self._steps = steps
+
         self.retrieve = _legacy_response.to_raw_response_wrapper(
             steps.retrieve,
         )
         self.list = _legacy_response.to_raw_response_wrapper(
             steps.list,
         )
 
 
 class AsyncStepsWithRawResponse:
     def __init__(self, steps: AsyncSteps) -> None:
+        self._steps = steps
+
         self.retrieve = _legacy_response.async_to_raw_response_wrapper(
             steps.retrieve,
         )
         self.list = _legacy_response.async_to_raw_response_wrapper(
             steps.list,
         )
 
 
 class StepsWithStreamingResponse:
     def __init__(self, steps: Steps) -> None:
+        self._steps = steps
+
         self.retrieve = to_streamed_response_wrapper(
             steps.retrieve,
         )
         self.list = to_streamed_response_wrapper(
             steps.list,
         )
 
 
 class AsyncStepsWithStreamingResponse:
     def __init__(self, steps: AsyncSteps) -> None:
+        self._steps = steps
+
         self.retrieve = async_to_streamed_response_wrapper(
             steps.retrieve,
         )
         self.list = async_to_streamed_response_wrapper(
             steps.list,
         )
```

### Comparing `openai-1.8.0/src/openai/resources/chat/__init__.py` & `openai-1.9.0/src/openai/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/resources/chat/chat.py` & `openai-1.9.0/src/openai/resources/chat/chat.py`

 * *Files 18% similar despite different names*

```diff
@@ -42,23 +42,39 @@
     @cached_property
     def with_streaming_response(self) -> AsyncChatWithStreamingResponse:
         return AsyncChatWithStreamingResponse(self)
 
 
 class ChatWithRawResponse:
     def __init__(self, chat: Chat) -> None:
-        self.completions = CompletionsWithRawResponse(chat.completions)
+        self._chat = chat
+
+    @cached_property
+    def completions(self) -> CompletionsWithRawResponse:
+        return CompletionsWithRawResponse(self._chat.completions)
 
 
 class AsyncChatWithRawResponse:
     def __init__(self, chat: AsyncChat) -> None:
-        self.completions = AsyncCompletionsWithRawResponse(chat.completions)
+        self._chat = chat
+
+    @cached_property
+    def completions(self) -> AsyncCompletionsWithRawResponse:
+        return AsyncCompletionsWithRawResponse(self._chat.completions)
 
 
 class ChatWithStreamingResponse:
     def __init__(self, chat: Chat) -> None:
-        self.completions = CompletionsWithStreamingResponse(chat.completions)
+        self._chat = chat
+
+    @cached_property
+    def completions(self) -> CompletionsWithStreamingResponse:
+        return CompletionsWithStreamingResponse(self._chat.completions)
 
 
 class AsyncChatWithStreamingResponse:
     def __init__(self, chat: AsyncChat) -> None:
-        self.completions = AsyncCompletionsWithStreamingResponse(chat.completions)
+        self._chat = chat
+
+    @cached_property
+    def completions(self) -> AsyncCompletionsWithStreamingResponse:
+        return AsyncCompletionsWithStreamingResponse(self._chat.completions)
```

### Comparing `openai-1.8.0/src/openai/resources/chat/completions.py` & `openai-1.9.0/src/openai/resources/chat/completions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1331,31 +1331,39 @@
             stream=stream or False,
             stream_cls=AsyncStream[ChatCompletionChunk],
         )
 
 
 class CompletionsWithRawResponse:
     def __init__(self, completions: Completions) -> None:
+        self._completions = completions
+
         self.create = _legacy_response.to_raw_response_wrapper(
             completions.create,
         )
 
 
 class AsyncCompletionsWithRawResponse:
     def __init__(self, completions: AsyncCompletions) -> None:
+        self._completions = completions
+
         self.create = _legacy_response.async_to_raw_response_wrapper(
             completions.create,
         )
 
 
 class CompletionsWithStreamingResponse:
     def __init__(self, completions: Completions) -> None:
+        self._completions = completions
+
         self.create = to_streamed_response_wrapper(
             completions.create,
         )
 
 
 class AsyncCompletionsWithStreamingResponse:
     def __init__(self, completions: AsyncCompletions) -> None:
+        self._completions = completions
+
         self.create = async_to_streamed_response_wrapper(
             completions.create,
         )
```

### Comparing `openai-1.8.0/src/openai/resources/fine_tuning/__init__.py` & `openai-1.9.0/src/openai/resources/fine_tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/resources/fine_tuning/fine_tuning.py` & `openai-1.9.0/src/openai/resources/fine_tuning/fine_tuning.py`

 * *Files 19% similar despite different names*

```diff
@@ -42,23 +42,39 @@
     @cached_property
     def with_streaming_response(self) -> AsyncFineTuningWithStreamingResponse:
         return AsyncFineTuningWithStreamingResponse(self)
 
 
 class FineTuningWithRawResponse:
     def __init__(self, fine_tuning: FineTuning) -> None:
-        self.jobs = JobsWithRawResponse(fine_tuning.jobs)
+        self._fine_tuning = fine_tuning
+
+    @cached_property
+    def jobs(self) -> JobsWithRawResponse:
+        return JobsWithRawResponse(self._fine_tuning.jobs)
 
 
 class AsyncFineTuningWithRawResponse:
     def __init__(self, fine_tuning: AsyncFineTuning) -> None:
-        self.jobs = AsyncJobsWithRawResponse(fine_tuning.jobs)
+        self._fine_tuning = fine_tuning
+
+    @cached_property
+    def jobs(self) -> AsyncJobsWithRawResponse:
+        return AsyncJobsWithRawResponse(self._fine_tuning.jobs)
 
 
 class FineTuningWithStreamingResponse:
     def __init__(self, fine_tuning: FineTuning) -> None:
-        self.jobs = JobsWithStreamingResponse(fine_tuning.jobs)
+        self._fine_tuning = fine_tuning
+
+    @cached_property
+    def jobs(self) -> JobsWithStreamingResponse:
+        return JobsWithStreamingResponse(self._fine_tuning.jobs)
 
 
 class AsyncFineTuningWithStreamingResponse:
     def __init__(self, fine_tuning: AsyncFineTuning) -> None:
-        self.jobs = AsyncJobsWithStreamingResponse(fine_tuning.jobs)
+        self._fine_tuning = fine_tuning
+
+    @cached_property
+    def jobs(self) -> AsyncJobsWithStreamingResponse:
+        return AsyncJobsWithStreamingResponse(self._fine_tuning.jobs)
```

### Comparing `openai-1.8.0/src/openai/resources/fine_tuning/jobs.py` & `openai-1.9.0/src/openai/resources/fine_tuning/jobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -549,14 +549,16 @@
             ),
             model=FineTuningJobEvent,
         )
 
 
 class JobsWithRawResponse:
     def __init__(self, jobs: Jobs) -> None:
+        self._jobs = jobs
+
         self.create = _legacy_response.to_raw_response_wrapper(
             jobs.create,
         )
         self.retrieve = _legacy_response.to_raw_response_wrapper(
             jobs.retrieve,
         )
         self.list = _legacy_response.to_raw_response_wrapper(
@@ -568,14 +570,16 @@
         self.list_events = _legacy_response.to_raw_response_wrapper(
             jobs.list_events,
         )
 
 
 class AsyncJobsWithRawResponse:
     def __init__(self, jobs: AsyncJobs) -> None:
+        self._jobs = jobs
+
         self.create = _legacy_response.async_to_raw_response_wrapper(
             jobs.create,
         )
         self.retrieve = _legacy_response.async_to_raw_response_wrapper(
             jobs.retrieve,
         )
         self.list = _legacy_response.async_to_raw_response_wrapper(
@@ -587,14 +591,16 @@
         self.list_events = _legacy_response.async_to_raw_response_wrapper(
             jobs.list_events,
         )
 
 
 class JobsWithStreamingResponse:
     def __init__(self, jobs: Jobs) -> None:
+        self._jobs = jobs
+
         self.create = to_streamed_response_wrapper(
             jobs.create,
         )
         self.retrieve = to_streamed_response_wrapper(
             jobs.retrieve,
         )
         self.list = to_streamed_response_wrapper(
@@ -606,14 +612,16 @@
         self.list_events = to_streamed_response_wrapper(
             jobs.list_events,
         )
 
 
 class AsyncJobsWithStreamingResponse:
     def __init__(self, jobs: AsyncJobs) -> None:
+        self._jobs = jobs
+
         self.create = async_to_streamed_response_wrapper(
             jobs.create,
         )
         self.retrieve = async_to_streamed_response_wrapper(
             jobs.retrieve,
         )
         self.list = async_to_streamed_response_wrapper(
```

### Comparing `openai-1.8.0/src/openai/types/__init__.py` & `openai-1.9.0/src/openai/types/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/completion.py` & `openai-1.9.0/src/openai/types/completion.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/completion_choice.py` & `openai-1.9.0/src/openai/types/completion_choice.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/completion_create_params.py` & `openai-1.9.0/src/openai/types/completion_create_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/create_embedding_response.py` & `openai-1.9.0/src/openai/types/create_embedding_response.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/embedding.py` & `openai-1.9.0/src/openai/types/embedding.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/embedding_create_params.py` & `openai-1.9.0/src/openai/types/embedding_create_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/file_create_params.py` & `openai-1.9.0/src/openai/types/file_create_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/file_object.py` & `openai-1.9.0/src/openai/types/file_object.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/image.py` & `openai-1.9.0/src/openai/types/image.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/image_create_variation_params.py` & `openai-1.9.0/src/openai/types/image_create_variation_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/image_edit_params.py` & `openai-1.9.0/src/openai/types/image_edit_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/image_generate_params.py` & `openai-1.9.0/src/openai/types/image_generate_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/moderation.py` & `openai-1.9.0/src/openai/types/moderation.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/moderation_create_params.py` & `openai-1.9.0/src/openai/types/moderation_create_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/audio/speech_create_params.py` & `openai-1.9.0/src/openai/types/audio/speech_create_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/audio/transcription_create_params.py` & `openai-1.9.0/src/openai/types/audio/transcription_create_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/audio/translation_create_params.py` & `openai-1.9.0/src/openai/types/audio/translation_create_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/__init__.py` & `openai-1.9.0/src/openai/types/beta/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/assistant.py` & `openai-1.9.0/src/openai/types/beta/assistant.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/assistant_create_params.py` & `openai-1.9.0/src/openai/types/beta/assistant_create_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/assistant_list_params.py` & `openai-1.9.0/src/openai/types/beta/assistant_list_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/assistant_update_params.py` & `openai-1.9.0/src/openai/types/beta/assistant_update_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/thread.py` & `openai-1.9.0/src/openai/types/beta/thread.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/thread_create_and_run_params.py` & `openai-1.9.0/src/openai/types/beta/thread_create_and_run_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/thread_create_params.py` & `openai-1.9.0/src/openai/types/beta/thread_create_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/thread_update_params.py` & `openai-1.9.0/src/openai/types/beta/thread_update_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/assistants/assistant_file.py` & `openai-1.9.0/src/openai/types/beta/assistants/assistant_file.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/assistants/file_list_params.py` & `openai-1.9.0/src/openai/types/beta/assistants/file_list_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/threads/__init__.py` & `openai-1.9.0/src/openai/types/beta/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/threads/message_content_text.py` & `openai-1.9.0/src/openai/types/beta/threads/message_content_text.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/threads/message_create_params.py` & `openai-1.9.0/src/openai/types/beta/threads/message_create_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/threads/message_list_params.py` & `openai-1.9.0/src/openai/types/beta/threads/message_list_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/threads/message_update_params.py` & `openai-1.9.0/src/openai/types/beta/threads/message_update_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/threads/required_action_function_tool_call.py` & `openai-1.9.0/src/openai/types/beta/threads/required_action_function_tool_call.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/threads/run.py` & `openai-1.9.0/src/openai/types/beta/threads/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     "LastError",
     "RequiredAction",
     "RequiredActionSubmitToolOutputs",
     "Tool",
     "ToolAssistantToolsCode",
     "ToolAssistantToolsRetrieval",
     "ToolAssistantToolsFunction",
+    "Usage",
 ]
 
 
 class LastError(BaseModel):
     code: Literal["server_error", "rate_limit_exceeded"]
     """One of `server_error` or `rate_limit_exceeded`."""
 
@@ -57,14 +58,25 @@
     type: Literal["function"]
     """The type of tool being defined: `function`"""
 
 
 Tool = Union[ToolAssistantToolsCode, ToolAssistantToolsRetrieval, ToolAssistantToolsFunction]
 
 
+class Usage(BaseModel):
+    completion_tokens: int
+    """Number of completion tokens used over the course of the run."""
+
+    prompt_tokens: int
+    """Number of prompt tokens used over the course of the run."""
+
+    total_tokens: int
+    """Total number of tokens used (prompt + completion)."""
+
+
 class Run(BaseModel):
     id: str
     """The identifier, which can be referenced in API endpoints."""
 
     assistant_id: str
     """
     The ID of the
@@ -148,7 +160,14 @@
 
     tools: List[Tool]
     """
     The list of tools that the
     [assistant](https://platform.openai.com/docs/api-reference/assistants) used for
     this run.
     """
+
+    usage: Optional[Usage] = None
+    """Usage statistics related to the run.
+
+    This value will be `null` if the run is not in a terminal state (i.e.
+    `in_progress`, `queued`, etc.).
+    """
```

### Comparing `openai-1.8.0/src/openai/types/beta/threads/run_create_params.py` & `openai-1.9.0/src/openai/types/beta/threads/run_create_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/threads/run_list_params.py` & `openai-1.9.0/src/openai/types/beta/threads/run_list_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/threads/run_submit_tool_outputs_params.py` & `openai-1.9.0/src/openai/types/beta/threads/run_submit_tool_outputs_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/threads/run_update_params.py` & `openai-1.9.0/src/openai/types/beta/threads/run_update_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/threads/thread_message.py` & `openai-1.9.0/src/openai/types/beta/threads/thread_message.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/threads/messages/file_list_params.py` & `openai-1.9.0/src/openai/types/beta/threads/messages/file_list_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/threads/messages/message_file.py` & `openai-1.9.0/src/openai/types/beta/threads/messages/message_file.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/threads/runs/__init__.py` & `openai-1.9.0/src/openai/types/beta/threads/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/threads/runs/code_tool_call.py` & `openai-1.9.0/src/openai/types/beta/threads/runs/code_tool_call.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/threads/runs/function_tool_call.py` & `openai-1.9.0/src/openai/types/beta/threads/runs/function_tool_call.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/threads/runs/run_step.py` & `openai-1.9.0/src/openai/types/beta/threads/runs/run_step.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,28 +4,39 @@
 from typing import Union, Optional
 from typing_extensions import Literal
 
 from ....._models import BaseModel
 from .tool_calls_step_details import ToolCallsStepDetails
 from .message_creation_step_details import MessageCreationStepDetails
 
-__all__ = ["RunStep", "LastError", "StepDetails"]
+__all__ = ["RunStep", "LastError", "StepDetails", "Usage"]
 
 
 class LastError(BaseModel):
     code: Literal["server_error", "rate_limit_exceeded"]
     """One of `server_error` or `rate_limit_exceeded`."""
 
     message: str
     """A human-readable description of the error."""
 
 
 StepDetails = Union[MessageCreationStepDetails, ToolCallsStepDetails]
 
 
+class Usage(BaseModel):
+    completion_tokens: int
+    """Number of completion tokens used over the course of the run step."""
+
+    prompt_tokens: int
+    """Number of prompt tokens used over the course of the run step."""
+
+    total_tokens: int
+    """Total number of tokens used (prompt + completion)."""
+
+
 class RunStep(BaseModel):
     id: str
     """The identifier of the run step, which can be referenced in API endpoints."""
 
     assistant_id: str
     """
     The ID of the
@@ -87,7 +98,13 @@
     """
     The ID of the [thread](https://platform.openai.com/docs/api-reference/threads)
     that was run.
     """
 
     type: Literal["message_creation", "tool_calls"]
     """The type of run step, which can be either `message_creation` or `tool_calls`."""
+
+    usage: Optional[Usage] = None
+    """Usage statistics related to the run step.
+
+    This value will be `null` while the run step's status is `in_progress`.
+    """
```

### Comparing `openai-1.8.0/src/openai/types/beta/threads/runs/step_list_params.py` & `openai-1.9.0/src/openai/types/beta/threads/runs/step_list_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/beta/threads/runs/tool_calls_step_details.py` & `openai-1.9.0/src/openai/types/beta/threads/runs/tool_calls_step_details.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/chat/__init__.py` & `openai-1.9.0/src/openai/types/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/chat/chat_completion.py` & `openai-1.9.0/src/openai/types/chat/chat_completion.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/chat/chat_completion_assistant_message_param.py` & `openai-1.9.0/src/openai/types/chat/chat_completion_assistant_message_param.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/chat/chat_completion_chunk.py` & `openai-1.9.0/src/openai/types/chat/chat_completion_chunk.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/chat/chat_completion_content_part_image_param.py` & `openai-1.9.0/src/openai/types/chat/chat_completion_content_part_image_param.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/chat/chat_completion_function_message_param.py` & `openai-1.9.0/src/openai/types/chat/chat_completion_function_message_param.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/chat/chat_completion_message.py` & `openai-1.9.0/src/openai/types/chat/chat_completion_message.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/chat/chat_completion_message_param.py` & `openai-1.9.0/src/openai/types/chat/chat_completion_message_param.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/chat/chat_completion_message_tool_call.py` & `openai-1.9.0/src/openai/types/chat/chat_completion_message_tool_call.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/chat/chat_completion_message_tool_call_param.py` & `openai-1.9.0/src/openai/types/chat/chat_completion_message_tool_call_param.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/chat/chat_completion_named_tool_choice_param.py` & `openai-1.9.0/src/openai/types/chat/chat_completion_named_tool_choice_param.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/chat/chat_completion_system_message_param.py` & `openai-1.9.0/src/openai/types/chat/chat_completion_system_message_param.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/chat/chat_completion_token_logprob.py` & `openai-1.9.0/src/openai/types/chat/chat_completion_token_logprob.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/chat/chat_completion_tool_message_param.py` & `openai-1.9.0/src/openai/types/chat/chat_completion_tool_message_param.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/chat/chat_completion_user_message_param.py` & `openai-1.9.0/src/openai/types/chat/chat_completion_user_message_param.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/chat/completion_create_params.py` & `openai-1.9.0/src/openai/types/chat/completion_create_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/fine_tuning/fine_tuning_job.py` & `openai-1.9.0/src/openai/types/fine_tuning/fine_tuning_job.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/fine_tuning/job_create_params.py` & `openai-1.9.0/src/openai/types/fine_tuning/job_create_params.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/shared/function_definition.py` & `openai-1.9.0/src/openai/types/shared/function_definition.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/src/openai/types/shared_params/function_definition.py` & `openai-1.9.0/src/openai/types/shared_params/function_definition.py`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/LICENSE` & `openai-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/README.md` & `openai-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `openai-1.8.0/pyproject.toml` & `openai-1.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "openai"
-version = "1.8.0"
+version = "1.9.0"
 description = "The official Python library for the openai API"
 readme = "README.md"
 license = "Apache-2.0"
 authors = [
 { name = "OpenAI", email = "support@openai.com" },
 ]
 dependencies = [
```

### Comparing `openai-1.8.0/PKG-INFO` & `openai-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai
-Version: 1.8.0
+Version: 1.9.0
 Summary: The official Python library for the openai API
 Project-URL: Homepage, https://github.com/openai/openai-python
 Project-URL: Repository, https://github.com/openai/openai-python
 Author-email: OpenAI <support@openai.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
```

