# Comparing `tmp/octoai-0.0.4.tar.gz` & `tmp/octoai-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octoai-0.0.4.tar", max compression
+gzip compressed data, was "octoai-0.6.0.tar", max compression
```

## Comparing `octoai-0.0.4.tar` & `octoai-0.6.0.tar`

### file list

```diff
@@ -1,124 +1,125 @@
--rw-r--r--   0        0        0     4922 2024-04-29 18:41:27.434935 octoai-0.0.4/README.md
--rw-r--r--   0        0        0      649 2024-04-29 18:41:27.434935 octoai-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      308 2024-04-29 18:41:27.434935 octoai-0.0.4/src/octoai/__init__.py
--rw-r--r--   0        0        0     2266 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/__init__.py
--rw-r--r--   0        0        0    34872 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/client.py
--rw-r--r--   0        0        0      170 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/errors/__init__.py
--rw-r--r--   0        0        0      314 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     2925 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/__init__.py
--rw-r--r--   0        0        0     2134 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/asset.py
--rw-r--r--   0        0        0      201 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/asset_type.py
--rw-r--r--   0        0        0      646 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/base_engine.py
--rw-r--r--   0        0        0      164 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/base_engine_type.py
--rw-r--r--   0        0        0     1241 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/checkpoint_data.py
--rw-r--r--   0        0        0      891 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/complete_asset_upload_response.py
--rw-r--r--   0        0        0     1257 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/create_asset_response.py
--rw-r--r--   0        0        0     1218 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/create_asset_response_transfer_api.py
--rw-r--r--   0        0        0     1870 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/data.py
--rw-r--r--   0        0        0      164 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/data_type.py
--rw-r--r--   0        0        0      986 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/delete_asset_response.py
--rw-r--r--   0        0        0     1133 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/file_data.py
--rw-r--r--   0        0        0      191 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/file_extension.py
--rw-r--r--   0        0        0      155 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/file_format.py
--rw-r--r--   0        0        0      181 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/file_structure.py
--rw-r--r--   0        0        0      955 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/http_validation_error.py
--rw-r--r--   0        0        0     1098 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/latent_data.py
--rw-r--r--   0        0        0     1137 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/list_assets_response.py
--rw-r--r--   0        0        0     1296 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/lora_data.py
--rw-r--r--   0        0        0     1096 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/no_transfer_api.py
--rw-r--r--   0        0        0     1003 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/presigned_url_transfer_api.py
--rw-r--r--   0        0        0     1128 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/retrieve_asset_response.py
--rw-r--r--   0        0        0     1241 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/retrieve_asset_response_transfer_api.py
--rw-r--r--   0        0        0      221 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/status.py
--rw-r--r--   0        0        0     1505 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/sts_transfer_api.py
--rw-r--r--   0        0        0     1370 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/textual_inversion_data.py
--rw-r--r--   0        0        0      163 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/transfer_api_type.py
--rw-r--r--   0        0        0     1234 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/vae_data.py
--rw-r--r--   0        0        0      974 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/asset_library/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     5541 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/base_client.py
--rw-r--r--   0        0        0     3834 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/client.py
--rw-r--r--   0        0        0      853 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/core/api_error.py
--rw-r--r--   0        0        0     2224 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/core/request_options.py
--rw-r--r--   0        0        0      500 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/environment.py
--rw-r--r--   0        0        0     1032 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/fine_tuning/__init__.py
--rw-r--r--   0        0        0    29562 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/fine_tuning/client.py
--rw-r--r--   0        0        0      170 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/fine_tuning/errors/__init__.py
--rw-r--r--   0        0        0      314 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/fine_tuning/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     1266 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/fine_tuning/types/__init__.py
--rw-r--r--   0        0        0      671 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/fine_tuning/types/base_engine.py
--rw-r--r--   0        0        0      826 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/fine_tuning/types/details.py
--rw-r--r--   0        0        0      955 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/fine_tuning/types/http_validation_error.py
--rw-r--r--   0        0        0     1189 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/fine_tuning/types/list_tunes_response.py
--rw-r--r--   0        0        0     1592 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/fine_tuning/types/lora_tune.py
--rw-r--r--   0        0        0     1111 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/fine_tuning/types/lora_tune_checkpoint.py
--rw-r--r--   0        0        0     1039 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/fine_tuning/types/lora_tune_file.py
--rw-r--r--   0        0        0     1062 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/fine_tuning/types/text_to_speech_latent_tune.py
--rw-r--r--   0        0        0     2273 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/fine_tuning/types/tune.py
--rw-r--r--   0        0        0      846 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/fine_tuning/types/tune_details.py
--rw-r--r--   0        0        0     1122 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/fine_tuning/types/tune_result.py
--rw-r--r--   0        0        0      192 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/fine_tuning/types/tune_status.py
--rw-r--r--   0        0        0      259 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/fine_tuning/types/tune_type.py
--rw-r--r--   0        0        0      974 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/fine_tuning/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/fine_tuning/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      838 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/image_gen/__init__.py
--rw-r--r--   0        0        0    41620 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/image_gen/client.py
--rw-r--r--   0        0        0      170 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/image_gen/errors/__init__.py
--rw-r--r--   0        0        0      314 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/image_gen/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     1115 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/image_gen/types/__init__.py
--rw-r--r--   0        0        0      955 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/image_gen/types/http_validation_error.py
--rw-r--r--   0        0        0      152 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/image_gen/types/image_encoding.py
--rw-r--r--   0        0        0     1245 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/image_gen/types/image_generation.py
--rw-r--r--   0        0        0     5332 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/image_gen/types/image_generation_request.py
--rw-r--r--   0        0        0      162 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/image_gen/types/image_generation_request_seed.py
--rw-r--r--   0        0        0     1205 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/image_gen/types/image_generation_response.py
--rw-r--r--   0        0        0      514 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/image_gen/types/scheduler.py
--rw-r--r--   0        0        0     1880 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/image_gen/types/sdxl_styles.py
--rw-r--r--   0        0        0      974 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/image_gen/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/image_gen/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     1271 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/image_gen/types/video_generation.py
--rw-r--r--   0        0        0      162 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/image_gen/types/video_generation_request_seed.py
--rw-r--r--   0        0        0     1208 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/image_gen/types/video_generation_response.py
--rw-r--r--   0        0        0        0 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/py.typed
--rw-r--r--   0        0        0     1528 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/__init__.py
--rw-r--r--   0        0        0    53893 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/client.py
--rw-r--r--   0        0        0      248 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/errors/__init__.py
--rw-r--r--   0        0        0      290 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/errors/internal_server_error.py
--rw-r--r--   0        0        0      314 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     2131 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/__init__.py
--rw-r--r--   0        0        0     1089 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/chat_completion_choice.py
--rw-r--r--   0        0        0     1815 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/chat_completion_chunk.py
--rw-r--r--   0        0        0     1133 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/chat_completion_chunk_choice.py
--rw-r--r--   0        0        0     1100 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/chat_completion_delta.py
--rw-r--r--   0        0        0     1118 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/chat_completion_request_ext.py
--rw-r--r--   0        0        0     1143 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/chat_completion_request_ext_vllm.py
--rw-r--r--   0        0        0     1185 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/chat_completion_response.py
--rw-r--r--   0        0        0     1054 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/chat_completion_response_format.py
--rw-r--r--   0        0        0      947 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/chat_fn_call.py
--rw-r--r--   0        0        0     1061 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/chat_message.py
--rw-r--r--   0        0        0      996 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/completion_choice.py
--rw-r--r--   0        0        0     1311 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/completion_response.py
--rw-r--r--   0        0        0      163 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/create_chat_completion_request_function_call.py
--rw-r--r--   0        0        0      169 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/create_chat_completion_stream_request_function_call.py
--rw-r--r--   0        0        0     1265 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/error_response.py
--rw-r--r--   0        0        0      153 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/error_response_validation_errors_value.py
--rw-r--r--   0        0        0      197 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/finish_reason.py
--rw-r--r--   0        0        0      982 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/function.py
--rw-r--r--   0        0        0      955 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/http_validation_error.py
--rw-r--r--   0        0        0     1178 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/log_probs.py
--rw-r--r--   0        0        0      174 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/prompt.py
--rw-r--r--   0        0        0      123 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/stop.py
--rw-r--r--   0        0        0      964 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/usage_stats.py
--rw-r--r--   0        0        0      974 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-29 18:41:27.438935 octoai-0.0.4/src/octoai/text_gen/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     7630 2024-04-29 18:41:27.442935 octoai-0.0.4/src/octoai/uploading_asset_library.py
--rw-r--r--   0        0        0       74 2024-04-29 18:41:27.442935 octoai-0.0.4/src/octoai/version.py
--rw-r--r--   0        0        0     5526 1970-01-01 00:00:00.000000 octoai-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     4922 2024-05-01 20:10:13.103144 octoai-0.6.0/README.md
+-rw-r--r--   0        0        0      649 2024-05-01 20:10:13.103144 octoai-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      308 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/__init__.py
+-rw-r--r--   0        0        0     2266 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/__init__.py
+-rw-r--r--   0        0        0    36620 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/client.py
+-rw-r--r--   0        0        0      170 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/errors/__init__.py
+-rw-r--r--   0        0        0      314 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0     2925 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/__init__.py
+-rw-r--r--   0        0        0     2172 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/asset.py
+-rw-r--r--   0        0        0      201 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/asset_type.py
+-rw-r--r--   0        0        0      646 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/base_engine.py
+-rw-r--r--   0        0        0      164 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/base_engine_type.py
+-rw-r--r--   0        0        0     1241 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/checkpoint_data.py
+-rw-r--r--   0        0        0      891 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/complete_asset_upload_response.py
+-rw-r--r--   0        0        0     1257 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/create_asset_response.py
+-rw-r--r--   0        0        0     1218 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/create_asset_response_transfer_api.py
+-rw-r--r--   0        0        0     1870 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/data.py
+-rw-r--r--   0        0        0      164 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/data_type.py
+-rw-r--r--   0        0        0      986 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/delete_asset_response.py
+-rw-r--r--   0        0        0     1133 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/file_data.py
+-rw-r--r--   0        0        0      191 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/file_extension.py
+-rw-r--r--   0        0        0      155 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/file_format.py
+-rw-r--r--   0        0        0      181 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/file_structure.py
+-rw-r--r--   0        0        0      955 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/http_validation_error.py
+-rw-r--r--   0        0        0     1098 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/latent_data.py
+-rw-r--r--   0        0        0     1137 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/list_assets_response.py
+-rw-r--r--   0        0        0     1340 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/lora_data.py
+-rw-r--r--   0        0        0     1096 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/no_transfer_api.py
+-rw-r--r--   0        0        0     1003 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/presigned_url_transfer_api.py
+-rw-r--r--   0        0        0     1128 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/retrieve_asset_response.py
+-rw-r--r--   0        0        0     1241 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/retrieve_asset_response_transfer_api.py
+-rw-r--r--   0        0        0      221 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/status.py
+-rw-r--r--   0        0        0     1505 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/sts_transfer_api.py
+-rw-r--r--   0        0        0     1370 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/textual_inversion_data.py
+-rw-r--r--   0        0        0      163 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/transfer_api_type.py
+-rw-r--r--   0        0        0     1234 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/vae_data.py
+-rw-r--r--   0        0        0      974 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/asset_library/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     5549 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/base_client.py
+-rw-r--r--   0        0        0    13262 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/client.py
+-rw-r--r--   0        0        0      853 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/core/api_error.py
+-rw-r--r--   0        0        0     2224 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/core/request_options.py
+-rw-r--r--   0        0        0      732 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/environment.py
+-rw-r--r--   0        0        0     1032 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/__init__.py
+-rw-r--r--   0        0        0    31006 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/client.py
+-rw-r--r--   0        0        0      170 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/errors/__init__.py
+-rw-r--r--   0        0        0      314 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0     1266 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/types/__init__.py
+-rw-r--r--   0        0        0      646 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/types/base_engine.py
+-rw-r--r--   0        0        0      826 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/types/details.py
+-rw-r--r--   0        0        0      955 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/types/http_validation_error.py
+-rw-r--r--   0        0        0     1189 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/types/list_tunes_response.py
+-rw-r--r--   0        0        0     1592 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/types/lora_tune.py
+-rw-r--r--   0        0        0     1111 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/types/lora_tune_checkpoint.py
+-rw-r--r--   0        0        0     1039 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/types/lora_tune_file.py
+-rw-r--r--   0        0        0     1062 2024-05-01 20:10:13.103144 octoai-0.6.0/src/octoai/fine_tuning/types/text_to_speech_latent_tune.py
+-rw-r--r--   0        0        0     2273 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/fine_tuning/types/tune.py
+-rw-r--r--   0        0        0      846 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/fine_tuning/types/tune_details.py
+-rw-r--r--   0        0        0     1122 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/fine_tuning/types/tune_result.py
+-rw-r--r--   0        0        0      192 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/fine_tuning/types/tune_status.py
+-rw-r--r--   0        0        0      259 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/fine_tuning/types/tune_type.py
+-rw-r--r--   0        0        0      974 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/fine_tuning/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/fine_tuning/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      838 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/__init__.py
+-rw-r--r--   0        0        0   123904 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/client.py
+-rw-r--r--   0        0        0      170 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/errors/__init__.py
+-rw-r--r--   0        0        0      314 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0     1115 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/__init__.py
+-rw-r--r--   0        0        0      955 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/http_validation_error.py
+-rw-r--r--   0        0        0      152 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/image_encoding.py
+-rw-r--r--   0        0        0     1245 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/image_generation.py
+-rw-r--r--   0        0        0     5332 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/image_generation_request.py
+-rw-r--r--   0        0        0      162 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/image_generation_request_seed.py
+-rw-r--r--   0        0        0     1205 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/image_generation_response.py
+-rw-r--r--   0        0        0      514 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/scheduler.py
+-rw-r--r--   0        0        0     1880 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/sdxl_styles.py
+-rw-r--r--   0        0        0      974 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     1271 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/video_generation.py
+-rw-r--r--   0        0        0      162 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/video_generation_request_seed.py
+-rw-r--r--   0        0        0     1208 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/image_gen/types/video_generation_response.py
+-rw-r--r--   0        0        0        0 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/py.typed
+-rw-r--r--   0        0        0     1528 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/__init__.py
+-rw-r--r--   0        0        0    54677 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/client.py
+-rw-r--r--   0        0        0      248 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/errors/__init__.py
+-rw-r--r--   0        0        0      290 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/errors/internal_server_error.py
+-rw-r--r--   0        0        0      314 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0     2131 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/__init__.py
+-rw-r--r--   0        0        0     1358 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/chat_completion_choice.py
+-rw-r--r--   0        0        0     1684 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/chat_completion_chunk.py
+-rw-r--r--   0        0        0     1133 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/chat_completion_chunk_choice.py
+-rw-r--r--   0        0        0     1100 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/chat_completion_delta.py
+-rw-r--r--   0        0        0     1066 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/chat_completion_request_ext.py
+-rw-r--r--   0        0        0     1143 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/chat_completion_request_ext_vllm.py
+-rw-r--r--   0        0        0     1688 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/chat_completion_response.py
+-rw-r--r--   0        0        0     1054 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/chat_completion_response_format.py
+-rw-r--r--   0        0        0      947 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/chat_fn_call.py
+-rw-r--r--   0        0        0     1061 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/chat_message.py
+-rw-r--r--   0        0        0     1045 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/completion_choice.py
+-rw-r--r--   0        0        0     1429 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/completion_response.py
+-rw-r--r--   0        0        0      163 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/create_chat_completion_request_function_call.py
+-rw-r--r--   0        0        0      169 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/create_chat_completion_stream_request_function_call.py
+-rw-r--r--   0        0        0     1265 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/error_response.py
+-rw-r--r--   0        0        0      153 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/error_response_validation_errors_value.py
+-rw-r--r--   0        0        0      189 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/finish_reason.py
+-rw-r--r--   0        0        0      982 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/function.py
+-rw-r--r--   0        0        0      955 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/http_validation_error.py
+-rw-r--r--   0        0        0     1247 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/log_probs.py
+-rw-r--r--   0        0        0      174 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/prompt.py
+-rw-r--r--   0        0        0      123 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/stop.py
+-rw-r--r--   0        0        0     1228 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/usage_stats.py
+-rw-r--r--   0        0        0      974 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/text_gen/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     7630 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/uploading_asset_library.py
+-rw-r--r--   0        0        0     2799 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/util.py
+-rw-r--r--   0        0        0       74 2024-05-01 20:10:13.107144 octoai-0.6.0/src/octoai/version.py
+-rw-r--r--   0        0        0     5526 1970-01-01 00:00:00.000000 octoai-0.6.0/PKG-INFO
```

### Comparing `octoai-0.0.4/README.md` & `octoai-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/pyproject.toml` & `octoai-0.6.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "octoai"
-version = "0.0.4"
+version = "0.6.0"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "octoai", from = "src"}
 ]
```

### Comparing `octoai-0.0.4/src/octoai/asset_library/__init__.py` & `octoai-0.6.0/src/octoai/asset_library/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/asset_library/client.py` & `octoai-0.6.0/src/octoai/asset_library/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -45,39 +45,48 @@
         offset: typing.Optional[int] = None,
         get_preview_urls: typing.Optional[bool] = None,
         asset_ids: typing.Optional[str] = None,
         owner: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListAssetsResponse:
         """
-        Parameters:
-            - name: typing.Optional[str].
+        Parameters
+        ----------
+        name : typing.Optional[str]
 
-            - is_public: typing.Optional[bool].
+        is_public : typing.Optional[bool]
 
-            - data_type: typing.Optional[DataType].
+        data_type : typing.Optional[DataType]
 
-            - asset_type: typing.Optional[typing.Union[AssetType, typing.Sequence[AssetType]]].
+        asset_type : typing.Optional[typing.Union[AssetType, typing.Sequence[AssetType]]]
 
-            - engine: typing.Optional[typing.Union[BaseEngine, typing.Sequence[BaseEngine]]].
+        engine : typing.Optional[typing.Union[BaseEngine, typing.Sequence[BaseEngine]]]
 
-            - engine_type: typing.Optional[BaseEngineType].
+        engine_type : typing.Optional[BaseEngineType]
 
-            - limit: typing.Optional[int].
+        limit : typing.Optional[int]
 
-            - offset: typing.Optional[int].
+        offset : typing.Optional[int]
 
-            - get_preview_urls: typing.Optional[bool].
+        get_preview_urls : typing.Optional[bool]
 
-            - asset_ids: typing.Optional[str].
+        asset_ids : typing.Optional[str]
 
-            - owner: typing.Optional[str].
+        owner : typing.Optional[str]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListAssetsResponse
+            Successful Response
+
+        Examples
+        --------
         from octoai.client import OctoAI
 
         client = OctoAI(
             api_key="YOUR_API_KEY",
         )
         client.asset_library.list()
         """
@@ -133,48 +142,63 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
         self,
         *,
         asset_type: AssetType,
         data: Data,
+        name: str,
         description: typing.Optional[str] = OMIT,
         hf_repo: typing.Optional[str] = OMIT,
         hf_token_secret: typing.Optional[str] = OMIT,
         is_public: typing.Optional[bool] = OMIT,
-        name: str,
         skip_validation: typing.Optional[bool] = OMIT,
         transfer_api_type: typing.Optional[TransferApiType] = OMIT,
         url: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> CreateAssetResponse:
         """
-        Parameters:
-            - asset_type: AssetType. Asset type.
+        Parameters
+        ----------
+        asset_type : AssetType
+            Asset type.
+
+        data : Data
+            Asset data.
+
+        name : str
+            Asset name.
 
-            - data: Data. Asset data.
+        description : typing.Optional[str]
 
-            - description: typing.Optional[str].
+        hf_repo : typing.Optional[str]
 
-            - hf_repo: typing.Optional[str].
+        hf_token_secret : typing.Optional[str]
 
-            - hf_token_secret: typing.Optional[str].
+        is_public : typing.Optional[bool]
+            True if asset is public.
 
-            - is_public: typing.Optional[bool]. True if asset is public.
+        skip_validation : typing.Optional[bool]
+            Skip asset validation.
 
-            - name: str. Asset name.
+        transfer_api_type : typing.Optional[TransferApiType]
+            Transfer API type.
 
-            - skip_validation: typing.Optional[bool]. Skip asset validation.
+        url : typing.Optional[str]
 
-            - transfer_api_type: typing.Optional[TransferApiType]. Transfer API type.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - url: typing.Optional[str].
+        Returns
+        -------
+        CreateAssetResponse
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from octoai.asset_library import Data_Checkpoint
         from octoai.client import OctoAI
 
         client = OctoAI(
             api_key="YOUR_API_KEY",
         )
         client.asset_library.create(
@@ -245,19 +269,28 @@
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, asset_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> DeleteAssetResponse:
         """
-        Parameters:
-            - asset_id: str.
+        Parameters
+        ----------
+        asset_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        DeleteAssetResponse
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from octoai.client import OctoAI
 
         client = OctoAI(
             api_key="YOUR_API_KEY",
         )
         client.asset_library.delete(
             asset_id="asset_id",
@@ -297,35 +330,51 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def complete_upload(
         self,
         asset_id: str,
         *,
+        skip_validation: typing.Optional[bool] = OMIT,
         token: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> CompleteAssetUploadResponse:
         """
-        Parameters:
-            - asset_id: str.
-
-            - token: typing.Optional[str]. Unused
+        Parameters
+        ----------
+        asset_id : str
+
+        skip_validation : typing.Optional[bool]
+            Skip asset validation.
+
+        token : typing.Optional[str]
+            Unused
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        CompleteAssetUploadResponse
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from octoai.client import OctoAI
 
         client = OctoAI(
             api_key="YOUR_API_KEY",
         )
         client.asset_library.complete_upload(
             asset_id="asset_id",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
+        if skip_validation is not OMIT:
+            _request["skip_validation"] = skip_validation
         if token is not OMIT:
             _request["token"] = token
         _response = self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_environment().default}/",
                 f"v1/assets/{jsonable_encoder(asset_id)}/complete-upload",
@@ -369,21 +418,30 @@
         self,
         asset_owner_and_name_or_id: str,
         *,
         transfer_api_type: typing.Optional[TransferApiType] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> RetrieveAssetResponse:
         """
-        Parameters:
-            - asset_owner_and_name_or_id: str.
-
-            - transfer_api_type: typing.Optional[TransferApiType].
+        Parameters
+        ----------
+        asset_owner_and_name_or_id : str
+
+        transfer_api_type : typing.Optional[TransferApiType]
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        RetrieveAssetResponse
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from octoai.client import OctoAI
 
         client = OctoAI(
             api_key="YOUR_API_KEY",
         )
         client.asset_library.get(
             asset_owner_and_name_or_id="string",
@@ -452,39 +510,48 @@
         offset: typing.Optional[int] = None,
         get_preview_urls: typing.Optional[bool] = None,
         asset_ids: typing.Optional[str] = None,
         owner: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListAssetsResponse:
         """
-        Parameters:
-            - name: typing.Optional[str].
+        Parameters
+        ----------
+        name : typing.Optional[str]
 
-            - is_public: typing.Optional[bool].
+        is_public : typing.Optional[bool]
 
-            - data_type: typing.Optional[DataType].
+        data_type : typing.Optional[DataType]
 
-            - asset_type: typing.Optional[typing.Union[AssetType, typing.Sequence[AssetType]]].
+        asset_type : typing.Optional[typing.Union[AssetType, typing.Sequence[AssetType]]]
 
-            - engine: typing.Optional[typing.Union[BaseEngine, typing.Sequence[BaseEngine]]].
+        engine : typing.Optional[typing.Union[BaseEngine, typing.Sequence[BaseEngine]]]
 
-            - engine_type: typing.Optional[BaseEngineType].
+        engine_type : typing.Optional[BaseEngineType]
 
-            - limit: typing.Optional[int].
+        limit : typing.Optional[int]
 
-            - offset: typing.Optional[int].
+        offset : typing.Optional[int]
 
-            - get_preview_urls: typing.Optional[bool].
+        get_preview_urls : typing.Optional[bool]
 
-            - asset_ids: typing.Optional[str].
+        asset_ids : typing.Optional[str]
 
-            - owner: typing.Optional[str].
+        owner : typing.Optional[str]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListAssetsResponse
+            Successful Response
+
+        Examples
+        --------
         from octoai.client import AsyncOctoAI
 
         client = AsyncOctoAI(
             api_key="YOUR_API_KEY",
         )
         await client.asset_library.list()
         """
@@ -540,48 +607,63 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
         self,
         *,
         asset_type: AssetType,
         data: Data,
+        name: str,
         description: typing.Optional[str] = OMIT,
         hf_repo: typing.Optional[str] = OMIT,
         hf_token_secret: typing.Optional[str] = OMIT,
         is_public: typing.Optional[bool] = OMIT,
-        name: str,
         skip_validation: typing.Optional[bool] = OMIT,
         transfer_api_type: typing.Optional[TransferApiType] = OMIT,
         url: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> CreateAssetResponse:
         """
-        Parameters:
-            - asset_type: AssetType. Asset type.
+        Parameters
+        ----------
+        asset_type : AssetType
+            Asset type.
+
+        data : Data
+            Asset data.
+
+        name : str
+            Asset name.
 
-            - data: Data. Asset data.
+        description : typing.Optional[str]
 
-            - description: typing.Optional[str].
+        hf_repo : typing.Optional[str]
 
-            - hf_repo: typing.Optional[str].
+        hf_token_secret : typing.Optional[str]
 
-            - hf_token_secret: typing.Optional[str].
+        is_public : typing.Optional[bool]
+            True if asset is public.
 
-            - is_public: typing.Optional[bool]. True if asset is public.
+        skip_validation : typing.Optional[bool]
+            Skip asset validation.
 
-            - name: str. Asset name.
+        transfer_api_type : typing.Optional[TransferApiType]
+            Transfer API type.
 
-            - skip_validation: typing.Optional[bool]. Skip asset validation.
+        url : typing.Optional[str]
 
-            - transfer_api_type: typing.Optional[TransferApiType]. Transfer API type.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - url: typing.Optional[str].
+        Returns
+        -------
+        CreateAssetResponse
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from octoai.asset_library import Data_Checkpoint
         from octoai.client import AsyncOctoAI
 
         client = AsyncOctoAI(
             api_key="YOUR_API_KEY",
         )
         await client.asset_library.create(
@@ -654,19 +736,28 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(
         self, asset_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> DeleteAssetResponse:
         """
-        Parameters:
-            - asset_id: str.
+        Parameters
+        ----------
+        asset_id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        DeleteAssetResponse
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from octoai.client import AsyncOctoAI
 
         client = AsyncOctoAI(
             api_key="YOUR_API_KEY",
         )
         await client.asset_library.delete(
             asset_id="asset_id",
@@ -706,35 +797,51 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def complete_upload(
         self,
         asset_id: str,
         *,
+        skip_validation: typing.Optional[bool] = OMIT,
         token: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> CompleteAssetUploadResponse:
         """
-        Parameters:
-            - asset_id: str.
-
-            - token: typing.Optional[str]. Unused
+        Parameters
+        ----------
+        asset_id : str
+
+        skip_validation : typing.Optional[bool]
+            Skip asset validation.
+
+        token : typing.Optional[str]
+            Unused
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        CompleteAssetUploadResponse
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from octoai.client import AsyncOctoAI
 
         client = AsyncOctoAI(
             api_key="YOUR_API_KEY",
         )
         await client.asset_library.complete_upload(
             asset_id="asset_id",
         )
         """
         _request: typing.Dict[str, typing.Any] = {}
+        if skip_validation is not OMIT:
+            _request["skip_validation"] = skip_validation
         if token is not OMIT:
             _request["token"] = token
         _response = await self._client_wrapper.httpx_client.request(
             method="POST",
             url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_environment().default}/",
                 f"v1/assets/{jsonable_encoder(asset_id)}/complete-upload",
@@ -778,21 +885,30 @@
         self,
         asset_owner_and_name_or_id: str,
         *,
         transfer_api_type: typing.Optional[TransferApiType] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> RetrieveAssetResponse:
         """
-        Parameters:
-            - asset_owner_and_name_or_id: str.
-
-            - transfer_api_type: typing.Optional[TransferApiType].
+        Parameters
+        ----------
+        asset_owner_and_name_or_id : str
+
+        transfer_api_type : typing.Optional[TransferApiType]
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        RetrieveAssetResponse
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from octoai.client import AsyncOctoAI
 
         client = AsyncOctoAI(
             api_key="YOUR_API_KEY",
         )
         await client.asset_library.get(
             asset_owner_and_name_or_id="string",
```

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/__init__.py` & `octoai-0.6.0/src/octoai/asset_library/types/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/asset.py` & `octoai-0.6.0/src/octoai/asset_library/types/asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,16 @@
     """
 
     tenant_uuid: str = pydantic_v1.Field()
     """
     Asset tenant ID.
     """
 
+    url: typing.Optional[str] = None
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/base_engine.py` & `octoai-0.6.0/src/octoai/asset_library/types/base_engine.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/checkpoint_data.py` & `octoai-0.6.0/src/octoai/asset_library/types/checkpoint_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/complete_asset_upload_response.py` & `octoai-0.6.0/src/octoai/asset_library/types/complete_asset_upload_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/create_asset_response.py` & `octoai-0.6.0/src/octoai/asset_library/types/create_asset_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/create_asset_response_transfer_api.py` & `octoai-0.6.0/src/octoai/asset_library/types/create_asset_response_transfer_api.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/data.py` & `octoai-0.6.0/src/octoai/asset_library/types/data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/delete_asset_response.py` & `octoai-0.6.0/src/octoai/asset_library/types/delete_asset_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/file_data.py` & `octoai-0.6.0/src/octoai/asset_library/types/file_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/http_validation_error.py` & `octoai-0.6.0/src/octoai/asset_library/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/latent_data.py` & `octoai-0.6.0/src/octoai/asset_library/types/latent_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/list_assets_response.py` & `octoai-0.6.0/src/octoai/asset_library/types/list_assets_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/lora_data.py` & `octoai-0.6.0/src/octoai/fine_tuning/types/lora_tune_checkpoint.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,35 +2,28 @@
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import pydantic_v1
 from .base_engine import BaseEngine
-from .data_type import DataType
-from .file_format import FileFormat
 
 
-class LoraData(pydantic_v1.BaseModel):
-    data_type: typing.Optional[DataType] = pydantic_v1.Field(default=None)
+class LoraTuneCheckpoint(pydantic_v1.BaseModel):
     """
-    Data type.
+    A checkpoint used for a LoRA Tune.
     """
 
-    engine: BaseEngine = pydantic_v1.Field()
+    checkpoint_id: str = pydantic_v1.Field()
     """
-    Engine type.
+    The checkpoint asset ID.
     """
 
-    file_format: typing.Optional[FileFormat] = pydantic_v1.Field(default=None)
-    """
-    File format.
-    """
-
-    trigger_words: typing.Optional[typing.List[str]] = None
+    engine: typing.Optional[BaseEngine] = None
+    name: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/no_transfer_api.py` & `octoai-0.6.0/src/octoai/asset_library/types/no_transfer_api.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/presigned_url_transfer_api.py` & `octoai-0.6.0/src/octoai/asset_library/types/presigned_url_transfer_api.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/retrieve_asset_response.py` & `octoai-0.6.0/src/octoai/asset_library/types/retrieve_asset_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/retrieve_asset_response_transfer_api.py` & `octoai-0.6.0/src/octoai/asset_library/types/retrieve_asset_response_transfer_api.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/sts_transfer_api.py` & `octoai-0.6.0/src/octoai/asset_library/types/sts_transfer_api.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/textual_inversion_data.py` & `octoai-0.6.0/src/octoai/asset_library/types/textual_inversion_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/vae_data.py` & `octoai-0.6.0/src/octoai/asset_library/types/vae_data.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/asset_library/types/validation_error.py` & `octoai-0.6.0/src/octoai/asset_library/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/base_client.py` & `octoai-0.6.0/src/octoai/base_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,27 +13,37 @@
 from .text_gen.client import AsyncTextGenClient, TextGenClient
 
 
 class BaseOctoAI:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
-    Parameters:
-        - environment: OctoAIEnvironment. The environment to use for requests from the client. from .environment import OctoAIEnvironment
+    Parameters
+    ----------
+    environment : OctoAIEnvironment
+        The environment to use for requests from the client. from .environment import OctoAIEnvironment
 
-                                          Defaults to OctoAIEnvironment.PRODUCTION
 
-        - api_key: typing.Optional[typing.Union[str, typing.Callable[[], str]]].
 
-        - timeout: typing.Optional[float]. The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
+        Defaults to OctoAIEnvironment.PRODUCTION
 
-        - follow_redirects: typing.Optional[bool]. Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
 
-        - httpx_client: typing.Optional[httpx.Client]. The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
-    ---
+
+    api_key : typing.Optional[typing.Union[str, typing.Callable[[], str]]]
+    timeout : typing.Optional[float]
+        The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
+
+    follow_redirects : typing.Optional[bool]
+        Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
+
+    httpx_client : typing.Optional[httpx.Client]
+        The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
+
+    Examples
+    --------
     from octoai.client import OctoAI
 
     client = OctoAI(
         api_key="YOUR_API_KEY",
     )
     """
 
@@ -54,36 +64,46 @@
             if httpx_client is not None
             else httpx.Client(timeout=_defaulted_timeout, follow_redirects=follow_redirects)
             if follow_redirects is not None
             else httpx.Client(timeout=_defaulted_timeout),
             timeout=_defaulted_timeout,
         )
         self.asset_library = AssetLibraryClient(client_wrapper=self._client_wrapper)
-        self.image_gen = ImageGenClient(client_wrapper=self._client_wrapper)
         self.fine_tuning = FineTuningClient(client_wrapper=self._client_wrapper)
+        self.image_gen = ImageGenClient(client_wrapper=self._client_wrapper)
         self.text_gen = TextGenClient(client_wrapper=self._client_wrapper)
 
 
 class AsyncBaseOctoAI:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
-    Parameters:
-        - environment: OctoAIEnvironment. The environment to use for requests from the client. from .environment import OctoAIEnvironment
+    Parameters
+    ----------
+    environment : OctoAIEnvironment
+        The environment to use for requests from the client. from .environment import OctoAIEnvironment
 
-                                          Defaults to OctoAIEnvironment.PRODUCTION
 
-        - api_key: typing.Optional[typing.Union[str, typing.Callable[[], str]]].
 
-        - timeout: typing.Optional[float]. The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
+        Defaults to OctoAIEnvironment.PRODUCTION
 
-        - follow_redirects: typing.Optional[bool]. Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
 
-        - httpx_client: typing.Optional[httpx.AsyncClient]. The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
-    ---
+
+    api_key : typing.Optional[typing.Union[str, typing.Callable[[], str]]]
+    timeout : typing.Optional[float]
+        The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
+
+    follow_redirects : typing.Optional[bool]
+        Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
+
+    httpx_client : typing.Optional[httpx.AsyncClient]
+        The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
+
+    Examples
+    --------
     from octoai.client import AsyncOctoAI
 
     client = AsyncOctoAI(
         api_key="YOUR_API_KEY",
     )
     """
 
@@ -104,10 +124,10 @@
             if httpx_client is not None
             else httpx.AsyncClient(timeout=_defaulted_timeout, follow_redirects=follow_redirects)
             if follow_redirects is not None
             else httpx.AsyncClient(timeout=_defaulted_timeout),
             timeout=_defaulted_timeout,
         )
         self.asset_library = AsyncAssetLibraryClient(client_wrapper=self._client_wrapper)
-        self.image_gen = AsyncImageGenClient(client_wrapper=self._client_wrapper)
         self.fine_tuning = AsyncFineTuningClient(client_wrapper=self._client_wrapper)
+        self.image_gen = AsyncImageGenClient(client_wrapper=self._client_wrapper)
         self.text_gen = AsyncTextGenClient(client_wrapper=self._client_wrapper)
```

### Comparing `octoai-0.0.4/src/octoai/core/__init__.py` & `octoai-0.6.0/src/octoai/core/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/core/client_wrapper.py` & `octoai-0.6.0/src/octoai/core/client_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self._environment = environment
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "octoai",
-            "X-Fern-SDK-Version": "0.0.4",
+            "X-Fern-SDK-Version": "0.6.0",
         }
         api_key = self._get_api_key()
         if api_key is not None:
             headers["Authorization"] = f"Bearer {api_key}"
         return headers
 
     def _get_api_key(self) -> typing.Optional[str]:
```

### Comparing `octoai-0.0.4/src/octoai/core/datetime_utils.py` & `octoai-0.6.0/src/octoai/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/core/file.py` & `octoai-0.6.0/src/octoai/core/file.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/core/http_client.py` & `octoai-0.6.0/src/octoai/core/http_client.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/core/jsonable_encoder.py` & `octoai-0.6.0/src/octoai/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/core/request_options.py` & `octoai-0.6.0/src/octoai/core/request_options.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/fine_tuning/__init__.py` & `octoai-0.6.0/src/octoai/fine_tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/fine_tuning/client.py` & `octoai-0.6.0/src/octoai/fine_tuning/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,34 +24,45 @@
 class FineTuningClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def create(
         self,
         *,
-        continue_on_rejection: typing.Optional[bool] = OMIT,
-        description: typing.Optional[str] = OMIT,
         details: Details,
         name: str,
+        continue_on_rejection: typing.Optional[bool] = OMIT,
+        description: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> Tune:
         """
         Spawn a tune.
 
-        Parameters:
-            - continue_on_rejection: typing.Optional[bool].
+        Parameters
+        ----------
+        details : Details
+            Details of the tune.
 
-            - description: typing.Optional[str].
+        name : str
+            The name of the tune.
 
-            - details: Details. Details of the tune.
+        continue_on_rejection : typing.Optional[bool]
 
-            - name: str. The name of the tune.
+        description : typing.Optional[str]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Tune
+            Successful Response
+
+        Examples
+        --------
         from octoai.client import OctoAI
         from octoai.fine_tuning import (
             Details_LoraTune,
             LoraTuneCheckpoint,
             LoraTuneFile,
         )
 
@@ -115,19 +126,29 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, tune_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Tune:
         """
         Get the specific tune.
 
-        Parameters:
-            - tune_id: str. The ID of the tune.
+        Parameters
+        ----------
+        tune_id : str
+            The ID of the tune.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Tune
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from octoai.client import OctoAI
 
         client = OctoAI(
             api_key="YOUR_API_KEY",
         )
         client.fine_tuning.get(
             tune_id="string",
@@ -169,19 +190,29 @@
 
     def delete(
         self, tune_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Dict[str, typing.Any]:
         """
         Delete the specified tune.
 
-        Parameters:
-            - tune_id: str. The ID of the tune.
+        Parameters
+        ----------
+        tune_id : str
+            The ID of the tune.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Dict[str, typing.Any]
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from octoai.client import OctoAI
 
         client = OctoAI(
             api_key="YOUR_API_KEY",
         )
         client.fine_tuning.delete(
             tune_id="tune_id",
@@ -221,19 +252,29 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def cancel(self, tune_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Tune:
         """
         Cancel the specified tune.
 
-        Parameters:
-            - tune_id: str. The ID of the tune to cancel.
+        Parameters
+        ----------
+        tune_id : str
+            The ID of the tune to cancel.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Tune
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from octoai.client import OctoAI
 
         client = OctoAI(
             api_key="YOUR_API_KEY",
         )
         client.fine_tuning.cancel(
             tune_id="string",
@@ -287,31 +328,47 @@
         trigger_words: typing.Optional[typing.Union[str, typing.Sequence[str]]] = None,
         engine: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListTunesResponse:
         """
         List all tunes owned by the current user.
 
-        Parameters:
-            - offset: typing.Optional[int]. Offset into the results.
+        Parameters
+        ----------
+        offset : typing.Optional[int]
+            Offset into the results.
+
+        limit : typing.Optional[int]
+            The max number of results to be shown (limit 100).
+
+        name : typing.Optional[str]
+            The name of the tune to filter on.
 
-            - limit: typing.Optional[int]. The max number of results to be shown (limit 100).
+        tune_type : typing.Optional[TuneType]
+            The type of the tune to filter on.
 
-            - name: typing.Optional[str]. The name of the tune to filter on.
+        base_checkpoint_id : typing.Optional[str]
+            The base checkpoint ID for the LoRA tune.
 
-            - tune_type: typing.Optional[TuneType]. The type of the tune to filter on.
+        trigger_words : typing.Optional[typing.Union[str, typing.Sequence[str]]]
+            The trigger words to filter on.
 
-            - base_checkpoint_id: typing.Optional[str]. The base checkpoint ID for the LoRA tune.
+        engine : typing.Optional[str]
+            The engine type.
 
-            - trigger_words: typing.Optional[typing.Union[str, typing.Sequence[str]]]. The trigger words to filter on.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - engine: typing.Optional[str]. The engine type.
+        Returns
+        -------
+        ListTunesResponse
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from octoai.client import OctoAI
 
         client = OctoAI(
             api_key="YOUR_API_KEY",
         )
         client.fine_tuning.list()
         """
@@ -366,34 +423,45 @@
 class AsyncFineTuningClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def create(
         self,
         *,
-        continue_on_rejection: typing.Optional[bool] = OMIT,
-        description: typing.Optional[str] = OMIT,
         details: Details,
         name: str,
+        continue_on_rejection: typing.Optional[bool] = OMIT,
+        description: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> Tune:
         """
         Spawn a tune.
 
-        Parameters:
-            - continue_on_rejection: typing.Optional[bool].
+        Parameters
+        ----------
+        details : Details
+            Details of the tune.
 
-            - description: typing.Optional[str].
+        name : str
+            The name of the tune.
 
-            - details: Details. Details of the tune.
+        continue_on_rejection : typing.Optional[bool]
 
-            - name: str. The name of the tune.
+        description : typing.Optional[str]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Tune
+            Successful Response
+
+        Examples
+        --------
         from octoai.client import AsyncOctoAI
         from octoai.fine_tuning import (
             Details_LoraTune,
             LoraTuneCheckpoint,
             LoraTuneFile,
         )
 
@@ -457,19 +525,29 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, tune_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Tune:
         """
         Get the specific tune.
 
-        Parameters:
-            - tune_id: str. The ID of the tune.
+        Parameters
+        ----------
+        tune_id : str
+            The ID of the tune.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Tune
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from octoai.client import AsyncOctoAI
 
         client = AsyncOctoAI(
             api_key="YOUR_API_KEY",
         )
         await client.fine_tuning.get(
             tune_id="string",
@@ -511,19 +589,29 @@
 
     async def delete(
         self, tune_id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Dict[str, typing.Any]:
         """
         Delete the specified tune.
 
-        Parameters:
-            - tune_id: str. The ID of the tune.
+        Parameters
+        ----------
+        tune_id : str
+            The ID of the tune.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Dict[str, typing.Any]
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from octoai.client import AsyncOctoAI
 
         client = AsyncOctoAI(
             api_key="YOUR_API_KEY",
         )
         await client.fine_tuning.delete(
             tune_id="tune_id",
@@ -563,19 +651,29 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def cancel(self, tune_id: str, *, request_options: typing.Optional[RequestOptions] = None) -> Tune:
         """
         Cancel the specified tune.
 
-        Parameters:
-            - tune_id: str. The ID of the tune to cancel.
+        Parameters
+        ----------
+        tune_id : str
+            The ID of the tune to cancel.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Tune
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from octoai.client import AsyncOctoAI
 
         client = AsyncOctoAI(
             api_key="YOUR_API_KEY",
         )
         await client.fine_tuning.cancel(
             tune_id="string",
@@ -629,31 +727,47 @@
         trigger_words: typing.Optional[typing.Union[str, typing.Sequence[str]]] = None,
         engine: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListTunesResponse:
         """
         List all tunes owned by the current user.
 
-        Parameters:
-            - offset: typing.Optional[int]. Offset into the results.
+        Parameters
+        ----------
+        offset : typing.Optional[int]
+            Offset into the results.
+
+        limit : typing.Optional[int]
+            The max number of results to be shown (limit 100).
+
+        name : typing.Optional[str]
+            The name of the tune to filter on.
 
-            - limit: typing.Optional[int]. The max number of results to be shown (limit 100).
+        tune_type : typing.Optional[TuneType]
+            The type of the tune to filter on.
 
-            - name: typing.Optional[str]. The name of the tune to filter on.
+        base_checkpoint_id : typing.Optional[str]
+            The base checkpoint ID for the LoRA tune.
 
-            - tune_type: typing.Optional[TuneType]. The type of the tune to filter on.
+        trigger_words : typing.Optional[typing.Union[str, typing.Sequence[str]]]
+            The trigger words to filter on.
 
-            - base_checkpoint_id: typing.Optional[str]. The base checkpoint ID for the LoRA tune.
+        engine : typing.Optional[str]
+            The engine type.
 
-            - trigger_words: typing.Optional[typing.Union[str, typing.Sequence[str]]]. The trigger words to filter on.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - engine: typing.Optional[str]. The engine type.
+        Returns
+        -------
+        ListTunesResponse
+            Successful Response
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from octoai.client import AsyncOctoAI
 
         client = AsyncOctoAI(
             api_key="YOUR_API_KEY",
         )
         await client.fine_tuning.list()
         """
```

### Comparing `octoai-0.0.4/src/octoai/fine_tuning/types/__init__.py` & `octoai-0.6.0/src/octoai/fine_tuning/types/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/fine_tuning/types/details.py` & `octoai-0.6.0/src/octoai/fine_tuning/types/details.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/fine_tuning/types/http_validation_error.py` & `octoai-0.6.0/src/octoai/fine_tuning/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/fine_tuning/types/list_tunes_response.py` & `octoai-0.6.0/src/octoai/fine_tuning/types/list_tunes_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/fine_tuning/types/lora_tune.py` & `octoai-0.6.0/src/octoai/fine_tuning/types/lora_tune.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/fine_tuning/types/lora_tune_checkpoint.py` & `octoai-0.6.0/src/octoai/text_gen/types/chat_fn_call.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import pydantic_v1
-from .base_engine import BaseEngine
 
 
-class LoraTuneCheckpoint(pydantic_v1.BaseModel):
+class ChatFnCall(pydantic_v1.BaseModel):
     """
-    A checkpoint used for a LoRA Tune.
+    An OpenAI API compatible schema for a chat function call.
     """
 
-    checkpoint_id: str = pydantic_v1.Field()
-    """
-    The checkpoint asset ID.
-    """
-
-    engine: typing.Optional[BaseEngine] = None
-    name: typing.Optional[str] = None
+    arguments: str
+    name: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `octoai-0.0.4/src/octoai/fine_tuning/types/lora_tune_file.py` & `octoai-0.6.0/src/octoai/fine_tuning/types/lora_tune_file.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/fine_tuning/types/text_to_speech_latent_tune.py` & `octoai-0.6.0/src/octoai/fine_tuning/types/text_to_speech_latent_tune.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/fine_tuning/types/tune.py` & `octoai-0.6.0/src/octoai/fine_tuning/types/tune.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/fine_tuning/types/tune_details.py` & `octoai-0.6.0/src/octoai/fine_tuning/types/tune_details.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/fine_tuning/types/tune_result.py` & `octoai-0.6.0/src/octoai/fine_tuning/types/tune_result.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/fine_tuning/types/validation_error.py` & `octoai-0.6.0/src/octoai/fine_tuning/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/image_gen/__init__.py` & `octoai-0.6.0/src/octoai/image_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/image_gen/types/__init__.py` & `octoai-0.6.0/src/octoai/image_gen/types/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/image_gen/types/http_validation_error.py` & `octoai-0.6.0/src/octoai/image_gen/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/image_gen/types/image_generation.py` & `octoai-0.6.0/src/octoai/image_gen/types/image_generation.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/image_gen/types/image_generation_request.py` & `octoai-0.6.0/src/octoai/image_gen/types/image_generation_request.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/image_gen/types/image_generation_response.py` & `octoai-0.6.0/src/octoai/image_gen/types/image_generation_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/image_gen/types/scheduler.py` & `octoai-0.6.0/src/octoai/image_gen/types/scheduler.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/image_gen/types/sdxl_styles.py` & `octoai-0.6.0/src/octoai/image_gen/types/sdxl_styles.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/image_gen/types/validation_error.py` & `octoai-0.6.0/src/octoai/image_gen/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/image_gen/types/video_generation.py` & `octoai-0.6.0/src/octoai/image_gen/types/video_generation.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/image_gen/types/video_generation_response.py` & `octoai-0.6.0/src/octoai/image_gen/types/video_generation_response.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/text_gen/__init__.py` & `octoai-0.6.0/src/octoai/text_gen/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/text_gen/client.py` & `octoai-0.6.0/src/octoai/text_gen/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,73 +36,84 @@
 class TextGenClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def create_chat_completion_stream(
         self,
         *,
+        messages: typing.Sequence[ChatMessage],
+        model: str,
         frequency_penalty: typing.Optional[float] = OMIT,
         function_call: typing.Optional[CreateChatCompletionStreamRequestFunctionCall] = OMIT,
         functions: typing.Optional[typing.Sequence[Function]] = OMIT,
         ignore_eos: typing.Optional[bool] = OMIT,
         logit_bias: typing.Optional[typing.Dict[str, typing.Optional[float]]] = OMIT,
-        max_tokens: typing.Optional[float] = OMIT,
-        messages: typing.Sequence[ChatMessage],
-        model: str,
+        max_tokens: typing.Optional[int] = OMIT,
         n: typing.Optional[int] = OMIT,
         octoai: typing.Optional[ChatCompletionRequestExt] = OMIT,
         presence_penalty: typing.Optional[float] = OMIT,
         repetition_penalty: typing.Optional[float] = OMIT,
         response_format: typing.Optional[ChatCompletionResponseFormat] = OMIT,
         stop: typing.Optional[Stop] = OMIT,
         temperature: typing.Optional[float] = OMIT,
         top_p: typing.Optional[float] = OMIT,
         user: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Iterator[ChatCompletionChunk]:
         """
-        An OpenAI compatible Chat Completion API.
+        Create a Chat Completion.
 
-        Parameters:
-            - frequency_penalty: typing.Optional[float].
+        Parameters
+        ----------
+        messages : typing.Sequence[ChatMessage]
+            A list of messages comprising the conversation so far.
 
-            - function_call: typing.Optional[CreateChatCompletionStreamRequestFunctionCall].
+        model : str
+            The identifier of the model to use.Can be a shared tenancy or custom model identifier.
 
-            - functions: typing.Optional[typing.Sequence[Function]].
+        frequency_penalty : typing.Optional[float]
 
-            - ignore_eos: typing.Optional[bool].
+        function_call : typing.Optional[CreateChatCompletionStreamRequestFunctionCall]
 
-            - logit_bias: typing.Optional[typing.Dict[str, typing.Optional[float]]].
+        functions : typing.Optional[typing.Sequence[Function]]
 
-            - max_tokens: typing.Optional[float].
+        ignore_eos : typing.Optional[bool]
 
-            - messages: typing.Sequence[ChatMessage]. A list of messages comprising the conversation so far.
+        logit_bias : typing.Optional[typing.Dict[str, typing.Optional[float]]]
 
-            - model: str. The identifier of the model to use.Can be a shared tenancy or custom model identifier.
+        max_tokens : typing.Optional[int]
 
-            - n: typing.Optional[int].
+        n : typing.Optional[int]
 
-            - octoai: typing.Optional[ChatCompletionRequestExt].
+        octoai : typing.Optional[ChatCompletionRequestExt]
 
-            - presence_penalty: typing.Optional[float].
+        presence_penalty : typing.Optional[float]
 
-            - repetition_penalty: typing.Optional[float].
+        repetition_penalty : typing.Optional[float]
 
-            - response_format: typing.Optional[ChatCompletionResponseFormat].
+        response_format : typing.Optional[ChatCompletionResponseFormat]
 
-            - stop: typing.Optional[Stop].
+        stop : typing.Optional[Stop]
 
-            - temperature: typing.Optional[float].
+        temperature : typing.Optional[float]
 
-            - top_p: typing.Optional[float].
+        top_p : typing.Optional[float]
 
-            - user: typing.Optional[str].
+        user : typing.Optional[str]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Yields
+        ------
+        typing.Iterator[ChatCompletionChunk]
+
+
+        Examples
+        --------
         from octoai.client import OctoAI
         from octoai.text_gen import (
             ChatCompletionRequestExt,
             ChatCompletionRequestExtVllm,
             ChatCompletionResponseFormat,
             ChatFnCall,
             ChatMessage,
@@ -120,29 +131,28 @@
                     description="string",
                     name="string",
                     parameters={"key": "value"},
                 )
             ],
             ignore_eos=True,
             logit_bias={"string": {"key": "value"}},
-            max_tokens=1.1,
+            max_tokens=1,
             messages=[
                 ChatMessage(
                     content="string",
                     function_call=ChatFnCall(
                         arguments="string",
                         name="string",
                     ),
                     role="string",
                 )
             ],
             model="string",
             n=1,
             octoai=ChatCompletionRequestExt(
-                loras=["string"],
                 vllm=ChatCompletionRequestExtVllm(),
             ),
             presence_penalty=1.1,
             repetition_penalty=1.1,
             response_format=ChatCompletionResponseFormat(
                 schema={"string": {"key": "value"}},
                 type="string",
@@ -227,73 +237,84 @@
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_chat_completion(
         self,
         *,
+        messages: typing.Sequence[ChatMessage],
+        model: str,
         frequency_penalty: typing.Optional[float] = OMIT,
         function_call: typing.Optional[CreateChatCompletionRequestFunctionCall] = OMIT,
         functions: typing.Optional[typing.Sequence[Function]] = OMIT,
         ignore_eos: typing.Optional[bool] = OMIT,
         logit_bias: typing.Optional[typing.Dict[str, typing.Optional[float]]] = OMIT,
-        max_tokens: typing.Optional[float] = OMIT,
-        messages: typing.Sequence[ChatMessage],
-        model: str,
+        max_tokens: typing.Optional[int] = OMIT,
         n: typing.Optional[int] = OMIT,
         octoai: typing.Optional[ChatCompletionRequestExt] = OMIT,
         presence_penalty: typing.Optional[float] = OMIT,
         repetition_penalty: typing.Optional[float] = OMIT,
         response_format: typing.Optional[ChatCompletionResponseFormat] = OMIT,
         stop: typing.Optional[Stop] = OMIT,
         temperature: typing.Optional[float] = OMIT,
         top_p: typing.Optional[float] = OMIT,
         user: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ChatCompletionResponse:
         """
-        An OpenAI compatible Chat Completion API.
+        Create a Chat Completion.
 
-        Parameters:
-            - frequency_penalty: typing.Optional[float].
+        Parameters
+        ----------
+        messages : typing.Sequence[ChatMessage]
+            A list of messages comprising the conversation so far.
 
-            - function_call: typing.Optional[CreateChatCompletionRequestFunctionCall].
+        model : str
+            The identifier of the model to use.Can be a shared tenancy or custom model identifier.
 
-            - functions: typing.Optional[typing.Sequence[Function]].
+        frequency_penalty : typing.Optional[float]
 
-            - ignore_eos: typing.Optional[bool].
+        function_call : typing.Optional[CreateChatCompletionRequestFunctionCall]
 
-            - logit_bias: typing.Optional[typing.Dict[str, typing.Optional[float]]].
+        functions : typing.Optional[typing.Sequence[Function]]
 
-            - max_tokens: typing.Optional[float].
+        ignore_eos : typing.Optional[bool]
 
-            - messages: typing.Sequence[ChatMessage]. A list of messages comprising the conversation so far.
+        logit_bias : typing.Optional[typing.Dict[str, typing.Optional[float]]]
 
-            - model: str. The identifier of the model to use.Can be a shared tenancy or custom model identifier.
+        max_tokens : typing.Optional[int]
 
-            - n: typing.Optional[int].
+        n : typing.Optional[int]
 
-            - octoai: typing.Optional[ChatCompletionRequestExt].
+        octoai : typing.Optional[ChatCompletionRequestExt]
 
-            - presence_penalty: typing.Optional[float].
+        presence_penalty : typing.Optional[float]
 
-            - repetition_penalty: typing.Optional[float].
+        repetition_penalty : typing.Optional[float]
 
-            - response_format: typing.Optional[ChatCompletionResponseFormat].
+        response_format : typing.Optional[ChatCompletionResponseFormat]
 
-            - stop: typing.Optional[Stop].
+        stop : typing.Optional[Stop]
 
-            - temperature: typing.Optional[float].
+        temperature : typing.Optional[float]
 
-            - top_p: typing.Optional[float].
+        top_p : typing.Optional[float]
 
-            - user: typing.Optional[str].
+        user : typing.Optional[str]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ChatCompletionResponse
+
+
+        Examples
+        --------
         from octoai.client import OctoAI
         from octoai.text_gen import ChatMessage
 
         client = OctoAI(
             api_key="YOUR_API_KEY",
         )
         client.text_gen.create_chat_completion(
@@ -375,73 +396,85 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_completion_stream(
         self,
         *,
+        model: str,
+        prompt: Prompt,
         best_of: typing.Optional[int] = OMIT,
         echo: typing.Optional[bool] = OMIT,
         frequency_penalty: typing.Optional[float] = OMIT,
         logit_bias: typing.Optional[typing.Dict[str, typing.Optional[float]]] = OMIT,
         logprobs: typing.Optional[int] = OMIT,
         max_tokens: typing.Optional[int] = OMIT,
-        model: str,
         n: typing.Optional[int] = OMIT,
         presence_penalty: typing.Optional[float] = OMIT,
-        prompt: Prompt,
         repetition_penalty: typing.Optional[float] = OMIT,
         seed: typing.Optional[int] = OMIT,
         stop: typing.Optional[Stop] = OMIT,
         suffix: typing.Optional[str] = OMIT,
         temperature: typing.Optional[float] = OMIT,
         top_p: typing.Optional[float] = OMIT,
         user: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Iterator[CompletionResponse]:
         """
-        An OpenAI compatible Completion API.
+        Create a Completion.
+
+        Parameters
+        ----------
+        model : str
+            Model name to use for completion.
+
+        prompt : Prompt
+            The prompt to generate completions from.
 
-        Parameters:
-            - best_of: typing.Optional[int].
+        best_of : typing.Optional[int]
 
-            - echo: typing.Optional[bool].
+        echo : typing.Optional[bool]
 
-            - frequency_penalty: typing.Optional[float].
+        frequency_penalty : typing.Optional[float]
 
-            - logit_bias: typing.Optional[typing.Dict[str, typing.Optional[float]]].
+        logit_bias : typing.Optional[typing.Dict[str, typing.Optional[float]]]
 
-            - logprobs: typing.Optional[int].
+        logprobs : typing.Optional[int]
 
-            - max_tokens: typing.Optional[int].
+        max_tokens : typing.Optional[int]
 
-            - model: str. Model name to use for completion.
+        n : typing.Optional[int]
 
-            - n: typing.Optional[int].
+        presence_penalty : typing.Optional[float]
 
-            - presence_penalty: typing.Optional[float].
+        repetition_penalty : typing.Optional[float]
 
-            - prompt: Prompt. The prompt to generate completions from.
+        seed : typing.Optional[int]
 
-            - repetition_penalty: typing.Optional[float].
+        stop : typing.Optional[Stop]
+            Strings that stop the generation when they are generated.
 
-            - seed: typing.Optional[int].
+        suffix : typing.Optional[str]
 
-            - stop: typing.Optional[Stop]. Strings that stop the generation when they are generated.
+        temperature : typing.Optional[float]
 
-            - suffix: typing.Optional[str].
+        top_p : typing.Optional[float]
 
-            - temperature: typing.Optional[float].
+        user : typing.Optional[str]
 
-            - top_p: typing.Optional[float].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - user: typing.Optional[str].
+        Yields
+        ------
+        typing.Iterator[CompletionResponse]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+
+        Examples
+        --------
         from octoai.client import OctoAI
 
         client = OctoAI(
             api_key="YOUR_API_KEY",
         )
         client.text_gen.create_completion_stream(
             best_of=1,
@@ -526,82 +559,96 @@
                     yield pydantic_v1.parse_obj_as(CompletionResponse, json.loads(_sse.data))  # type: ignore
                 return
             _response.read()
             if _response.status_code == 422:
                 raise UnprocessableEntityError(
                     pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
                 )
+            if _response.status_code == 500:
+                raise InternalServerError(pydantic_v1.parse_obj_as(ErrorResponse, _response.json()))  # type: ignore
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_completion(
         self,
         *,
+        model: str,
+        prompt: Prompt,
         best_of: typing.Optional[int] = OMIT,
         echo: typing.Optional[bool] = OMIT,
         frequency_penalty: typing.Optional[float] = OMIT,
         logit_bias: typing.Optional[typing.Dict[str, typing.Optional[float]]] = OMIT,
         logprobs: typing.Optional[int] = OMIT,
         max_tokens: typing.Optional[int] = OMIT,
-        model: str,
         n: typing.Optional[int] = OMIT,
         presence_penalty: typing.Optional[float] = OMIT,
-        prompt: Prompt,
         repetition_penalty: typing.Optional[float] = OMIT,
         seed: typing.Optional[int] = OMIT,
         stop: typing.Optional[Stop] = OMIT,
         suffix: typing.Optional[str] = OMIT,
         temperature: typing.Optional[float] = OMIT,
         top_p: typing.Optional[float] = OMIT,
         user: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> CompletionResponse:
         """
-        An OpenAI compatible Completion API.
+        Create a Completion.
+
+        Parameters
+        ----------
+        model : str
+            Model name to use for completion.
 
-        Parameters:
-            - best_of: typing.Optional[int].
+        prompt : Prompt
+            The prompt to generate completions from.
 
-            - echo: typing.Optional[bool].
+        best_of : typing.Optional[int]
 
-            - frequency_penalty: typing.Optional[float].
+        echo : typing.Optional[bool]
 
-            - logit_bias: typing.Optional[typing.Dict[str, typing.Optional[float]]].
+        frequency_penalty : typing.Optional[float]
 
-            - logprobs: typing.Optional[int].
+        logit_bias : typing.Optional[typing.Dict[str, typing.Optional[float]]]
 
-            - max_tokens: typing.Optional[int].
+        logprobs : typing.Optional[int]
 
-            - model: str. Model name to use for completion.
+        max_tokens : typing.Optional[int]
 
-            - n: typing.Optional[int].
+        n : typing.Optional[int]
 
-            - presence_penalty: typing.Optional[float].
+        presence_penalty : typing.Optional[float]
 
-            - prompt: Prompt. The prompt to generate completions from.
+        repetition_penalty : typing.Optional[float]
 
-            - repetition_penalty: typing.Optional[float].
+        seed : typing.Optional[int]
 
-            - seed: typing.Optional[int].
+        stop : typing.Optional[Stop]
+            Strings that stop the generation when they are generated.
 
-            - stop: typing.Optional[Stop]. Strings that stop the generation when they are generated.
+        suffix : typing.Optional[str]
 
-            - suffix: typing.Optional[str].
+        temperature : typing.Optional[float]
 
-            - temperature: typing.Optional[float].
+        top_p : typing.Optional[float]
 
-            - top_p: typing.Optional[float].
+        user : typing.Optional[str]
 
-            - user: typing.Optional[str].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        CompletionResponse
+
+
+        Examples
+        --------
         from octoai.client import OctoAI
 
         client = OctoAI(
             api_key="YOUR_API_KEY",
         )
         client.text_gen.create_completion(
             model="model",
@@ -667,87 +714,100 @@
         )
         if 200 <= _response.status_code < 300:
             return pydantic_v1.parse_obj_as(CompletionResponse, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(
                 pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
             )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic_v1.parse_obj_as(ErrorResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncTextGenClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def create_chat_completion_stream(
         self,
         *,
+        messages: typing.Sequence[ChatMessage],
+        model: str,
         frequency_penalty: typing.Optional[float] = OMIT,
         function_call: typing.Optional[CreateChatCompletionStreamRequestFunctionCall] = OMIT,
         functions: typing.Optional[typing.Sequence[Function]] = OMIT,
         ignore_eos: typing.Optional[bool] = OMIT,
         logit_bias: typing.Optional[typing.Dict[str, typing.Optional[float]]] = OMIT,
-        max_tokens: typing.Optional[float] = OMIT,
-        messages: typing.Sequence[ChatMessage],
-        model: str,
+        max_tokens: typing.Optional[int] = OMIT,
         n: typing.Optional[int] = OMIT,
         octoai: typing.Optional[ChatCompletionRequestExt] = OMIT,
         presence_penalty: typing.Optional[float] = OMIT,
         repetition_penalty: typing.Optional[float] = OMIT,
         response_format: typing.Optional[ChatCompletionResponseFormat] = OMIT,
         stop: typing.Optional[Stop] = OMIT,
         temperature: typing.Optional[float] = OMIT,
         top_p: typing.Optional[float] = OMIT,
         user: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.AsyncIterator[ChatCompletionChunk]:
         """
-        An OpenAI compatible Chat Completion API.
+        Create a Chat Completion.
 
-        Parameters:
-            - frequency_penalty: typing.Optional[float].
+        Parameters
+        ----------
+        messages : typing.Sequence[ChatMessage]
+            A list of messages comprising the conversation so far.
 
-            - function_call: typing.Optional[CreateChatCompletionStreamRequestFunctionCall].
+        model : str
+            The identifier of the model to use.Can be a shared tenancy or custom model identifier.
 
-            - functions: typing.Optional[typing.Sequence[Function]].
+        frequency_penalty : typing.Optional[float]
 
-            - ignore_eos: typing.Optional[bool].
+        function_call : typing.Optional[CreateChatCompletionStreamRequestFunctionCall]
 
-            - logit_bias: typing.Optional[typing.Dict[str, typing.Optional[float]]].
+        functions : typing.Optional[typing.Sequence[Function]]
 
-            - max_tokens: typing.Optional[float].
+        ignore_eos : typing.Optional[bool]
 
-            - messages: typing.Sequence[ChatMessage]. A list of messages comprising the conversation so far.
+        logit_bias : typing.Optional[typing.Dict[str, typing.Optional[float]]]
 
-            - model: str. The identifier of the model to use.Can be a shared tenancy or custom model identifier.
+        max_tokens : typing.Optional[int]
 
-            - n: typing.Optional[int].
+        n : typing.Optional[int]
 
-            - octoai: typing.Optional[ChatCompletionRequestExt].
+        octoai : typing.Optional[ChatCompletionRequestExt]
 
-            - presence_penalty: typing.Optional[float].
+        presence_penalty : typing.Optional[float]
 
-            - repetition_penalty: typing.Optional[float].
+        repetition_penalty : typing.Optional[float]
 
-            - response_format: typing.Optional[ChatCompletionResponseFormat].
+        response_format : typing.Optional[ChatCompletionResponseFormat]
 
-            - stop: typing.Optional[Stop].
+        stop : typing.Optional[Stop]
 
-            - temperature: typing.Optional[float].
+        temperature : typing.Optional[float]
 
-            - top_p: typing.Optional[float].
+        top_p : typing.Optional[float]
 
-            - user: typing.Optional[str].
+        user : typing.Optional[str]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Yields
+        ------
+        typing.AsyncIterator[ChatCompletionChunk]
+
+
+        Examples
+        --------
         from octoai.client import AsyncOctoAI
         from octoai.text_gen import (
             ChatCompletionRequestExt,
             ChatCompletionRequestExtVllm,
             ChatCompletionResponseFormat,
             ChatFnCall,
             ChatMessage,
@@ -765,29 +825,28 @@
                     description="string",
                     name="string",
                     parameters={"key": "value"},
                 )
             ],
             ignore_eos=True,
             logit_bias={"string": {"key": "value"}},
-            max_tokens=1.1,
+            max_tokens=1,
             messages=[
                 ChatMessage(
                     content="string",
                     function_call=ChatFnCall(
                         arguments="string",
                         name="string",
                     ),
                     role="string",
                 )
             ],
             model="string",
             n=1,
             octoai=ChatCompletionRequestExt(
-                loras=["string"],
                 vllm=ChatCompletionRequestExtVllm(),
             ),
             presence_penalty=1.1,
             repetition_penalty=1.1,
             response_format=ChatCompletionResponseFormat(
                 schema={"string": {"key": "value"}},
                 type="string",
@@ -872,73 +931,84 @@
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_chat_completion(
         self,
         *,
+        messages: typing.Sequence[ChatMessage],
+        model: str,
         frequency_penalty: typing.Optional[float] = OMIT,
         function_call: typing.Optional[CreateChatCompletionRequestFunctionCall] = OMIT,
         functions: typing.Optional[typing.Sequence[Function]] = OMIT,
         ignore_eos: typing.Optional[bool] = OMIT,
         logit_bias: typing.Optional[typing.Dict[str, typing.Optional[float]]] = OMIT,
-        max_tokens: typing.Optional[float] = OMIT,
-        messages: typing.Sequence[ChatMessage],
-        model: str,
+        max_tokens: typing.Optional[int] = OMIT,
         n: typing.Optional[int] = OMIT,
         octoai: typing.Optional[ChatCompletionRequestExt] = OMIT,
         presence_penalty: typing.Optional[float] = OMIT,
         repetition_penalty: typing.Optional[float] = OMIT,
         response_format: typing.Optional[ChatCompletionResponseFormat] = OMIT,
         stop: typing.Optional[Stop] = OMIT,
         temperature: typing.Optional[float] = OMIT,
         top_p: typing.Optional[float] = OMIT,
         user: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ChatCompletionResponse:
         """
-        An OpenAI compatible Chat Completion API.
+        Create a Chat Completion.
 
-        Parameters:
-            - frequency_penalty: typing.Optional[float].
+        Parameters
+        ----------
+        messages : typing.Sequence[ChatMessage]
+            A list of messages comprising the conversation so far.
 
-            - function_call: typing.Optional[CreateChatCompletionRequestFunctionCall].
+        model : str
+            The identifier of the model to use.Can be a shared tenancy or custom model identifier.
 
-            - functions: typing.Optional[typing.Sequence[Function]].
+        frequency_penalty : typing.Optional[float]
 
-            - ignore_eos: typing.Optional[bool].
+        function_call : typing.Optional[CreateChatCompletionRequestFunctionCall]
 
-            - logit_bias: typing.Optional[typing.Dict[str, typing.Optional[float]]].
+        functions : typing.Optional[typing.Sequence[Function]]
 
-            - max_tokens: typing.Optional[float].
+        ignore_eos : typing.Optional[bool]
 
-            - messages: typing.Sequence[ChatMessage]. A list of messages comprising the conversation so far.
+        logit_bias : typing.Optional[typing.Dict[str, typing.Optional[float]]]
 
-            - model: str. The identifier of the model to use.Can be a shared tenancy or custom model identifier.
+        max_tokens : typing.Optional[int]
 
-            - n: typing.Optional[int].
+        n : typing.Optional[int]
 
-            - octoai: typing.Optional[ChatCompletionRequestExt].
+        octoai : typing.Optional[ChatCompletionRequestExt]
 
-            - presence_penalty: typing.Optional[float].
+        presence_penalty : typing.Optional[float]
 
-            - repetition_penalty: typing.Optional[float].
+        repetition_penalty : typing.Optional[float]
 
-            - response_format: typing.Optional[ChatCompletionResponseFormat].
+        response_format : typing.Optional[ChatCompletionResponseFormat]
 
-            - stop: typing.Optional[Stop].
+        stop : typing.Optional[Stop]
 
-            - temperature: typing.Optional[float].
+        temperature : typing.Optional[float]
 
-            - top_p: typing.Optional[float].
+        top_p : typing.Optional[float]
 
-            - user: typing.Optional[str].
+        user : typing.Optional[str]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ChatCompletionResponse
+
+
+        Examples
+        --------
         from octoai.client import AsyncOctoAI
         from octoai.text_gen import ChatMessage
 
         client = AsyncOctoAI(
             api_key="YOUR_API_KEY",
         )
         await client.text_gen.create_chat_completion(
@@ -1020,73 +1090,85 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_completion_stream(
         self,
         *,
+        model: str,
+        prompt: Prompt,
         best_of: typing.Optional[int] = OMIT,
         echo: typing.Optional[bool] = OMIT,
         frequency_penalty: typing.Optional[float] = OMIT,
         logit_bias: typing.Optional[typing.Dict[str, typing.Optional[float]]] = OMIT,
         logprobs: typing.Optional[int] = OMIT,
         max_tokens: typing.Optional[int] = OMIT,
-        model: str,
         n: typing.Optional[int] = OMIT,
         presence_penalty: typing.Optional[float] = OMIT,
-        prompt: Prompt,
         repetition_penalty: typing.Optional[float] = OMIT,
         seed: typing.Optional[int] = OMIT,
         stop: typing.Optional[Stop] = OMIT,
         suffix: typing.Optional[str] = OMIT,
         temperature: typing.Optional[float] = OMIT,
         top_p: typing.Optional[float] = OMIT,
         user: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.AsyncIterator[CompletionResponse]:
         """
-        An OpenAI compatible Completion API.
+        Create a Completion.
+
+        Parameters
+        ----------
+        model : str
+            Model name to use for completion.
+
+        prompt : Prompt
+            The prompt to generate completions from.
 
-        Parameters:
-            - best_of: typing.Optional[int].
+        best_of : typing.Optional[int]
 
-            - echo: typing.Optional[bool].
+        echo : typing.Optional[bool]
 
-            - frequency_penalty: typing.Optional[float].
+        frequency_penalty : typing.Optional[float]
 
-            - logit_bias: typing.Optional[typing.Dict[str, typing.Optional[float]]].
+        logit_bias : typing.Optional[typing.Dict[str, typing.Optional[float]]]
 
-            - logprobs: typing.Optional[int].
+        logprobs : typing.Optional[int]
 
-            - max_tokens: typing.Optional[int].
+        max_tokens : typing.Optional[int]
 
-            - model: str. Model name to use for completion.
+        n : typing.Optional[int]
 
-            - n: typing.Optional[int].
+        presence_penalty : typing.Optional[float]
 
-            - presence_penalty: typing.Optional[float].
+        repetition_penalty : typing.Optional[float]
 
-            - prompt: Prompt. The prompt to generate completions from.
+        seed : typing.Optional[int]
 
-            - repetition_penalty: typing.Optional[float].
+        stop : typing.Optional[Stop]
+            Strings that stop the generation when they are generated.
 
-            - seed: typing.Optional[int].
+        suffix : typing.Optional[str]
 
-            - stop: typing.Optional[Stop]. Strings that stop the generation when they are generated.
+        temperature : typing.Optional[float]
 
-            - suffix: typing.Optional[str].
+        top_p : typing.Optional[float]
 
-            - temperature: typing.Optional[float].
+        user : typing.Optional[str]
 
-            - top_p: typing.Optional[float].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - user: typing.Optional[str].
+        Yields
+        ------
+        typing.AsyncIterator[CompletionResponse]
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+
+        Examples
+        --------
         from octoai.client import AsyncOctoAI
 
         client = AsyncOctoAI(
             api_key="YOUR_API_KEY",
         )
         await client.text_gen.create_completion_stream(
             best_of=1,
@@ -1171,82 +1253,96 @@
                     yield pydantic_v1.parse_obj_as(CompletionResponse, json.loads(_sse.data))  # type: ignore
                 return
             await _response.aread()
             if _response.status_code == 422:
                 raise UnprocessableEntityError(
                     pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
                 )
+            if _response.status_code == 500:
+                raise InternalServerError(pydantic_v1.parse_obj_as(ErrorResponse, _response.json()))  # type: ignore
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_completion(
         self,
         *,
+        model: str,
+        prompt: Prompt,
         best_of: typing.Optional[int] = OMIT,
         echo: typing.Optional[bool] = OMIT,
         frequency_penalty: typing.Optional[float] = OMIT,
         logit_bias: typing.Optional[typing.Dict[str, typing.Optional[float]]] = OMIT,
         logprobs: typing.Optional[int] = OMIT,
         max_tokens: typing.Optional[int] = OMIT,
-        model: str,
         n: typing.Optional[int] = OMIT,
         presence_penalty: typing.Optional[float] = OMIT,
-        prompt: Prompt,
         repetition_penalty: typing.Optional[float] = OMIT,
         seed: typing.Optional[int] = OMIT,
         stop: typing.Optional[Stop] = OMIT,
         suffix: typing.Optional[str] = OMIT,
         temperature: typing.Optional[float] = OMIT,
         top_p: typing.Optional[float] = OMIT,
         user: typing.Optional[str] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> CompletionResponse:
         """
-        An OpenAI compatible Completion API.
+        Create a Completion.
+
+        Parameters
+        ----------
+        model : str
+            Model name to use for completion.
 
-        Parameters:
-            - best_of: typing.Optional[int].
+        prompt : Prompt
+            The prompt to generate completions from.
 
-            - echo: typing.Optional[bool].
+        best_of : typing.Optional[int]
 
-            - frequency_penalty: typing.Optional[float].
+        echo : typing.Optional[bool]
 
-            - logit_bias: typing.Optional[typing.Dict[str, typing.Optional[float]]].
+        frequency_penalty : typing.Optional[float]
 
-            - logprobs: typing.Optional[int].
+        logit_bias : typing.Optional[typing.Dict[str, typing.Optional[float]]]
 
-            - max_tokens: typing.Optional[int].
+        logprobs : typing.Optional[int]
 
-            - model: str. Model name to use for completion.
+        max_tokens : typing.Optional[int]
 
-            - n: typing.Optional[int].
+        n : typing.Optional[int]
 
-            - presence_penalty: typing.Optional[float].
+        presence_penalty : typing.Optional[float]
 
-            - prompt: Prompt. The prompt to generate completions from.
+        repetition_penalty : typing.Optional[float]
 
-            - repetition_penalty: typing.Optional[float].
+        seed : typing.Optional[int]
 
-            - seed: typing.Optional[int].
+        stop : typing.Optional[Stop]
+            Strings that stop the generation when they are generated.
 
-            - stop: typing.Optional[Stop]. Strings that stop the generation when they are generated.
+        suffix : typing.Optional[str]
 
-            - suffix: typing.Optional[str].
+        temperature : typing.Optional[float]
 
-            - temperature: typing.Optional[float].
+        top_p : typing.Optional[float]
 
-            - top_p: typing.Optional[float].
+        user : typing.Optional[str]
 
-            - user: typing.Optional[str].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        CompletionResponse
+
+
+        Examples
+        --------
         from octoai.client import AsyncOctoAI
 
         client = AsyncOctoAI(
             api_key="YOUR_API_KEY",
         )
         await client.text_gen.create_completion(
             model="model",
@@ -1312,12 +1408,14 @@
         )
         if 200 <= _response.status_code < 300:
             return pydantic_v1.parse_obj_as(CompletionResponse, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(
                 pydantic_v1.parse_obj_as(HttpValidationError, _response.json())  # type: ignore
             )
+        if _response.status_code == 500:
+            raise InternalServerError(pydantic_v1.parse_obj_as(ErrorResponse, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `octoai-0.0.4/src/octoai/text_gen/types/__init__.py` & `octoai-0.6.0/src/octoai/text_gen/types/__init__.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/text_gen/types/chat_completion_choice.py` & `octoai-0.6.0/src/octoai/text_gen/types/completion_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import pydantic_v1
-from .chat_message import ChatMessage
-from .finish_reason import FinishReason
+from .completion_choice import CompletionChoice
+from .usage_stats import UsageStats
 
 
-class ChatCompletionChoice(pydantic_v1.BaseModel):
+class CompletionResponse(pydantic_v1.BaseModel):
     """
-    An OpenAI API compatible chat completion choice.
+    Represents a completion response from the API.
+    Note: both the streamed and non-streamed response objects
+    share the same shape (unlike the chat endpoint).
     """
 
-    finish_reason: typing.Optional[FinishReason] = None
-    index: int
-    message: ChatMessage
+    choices: typing.List[CompletionChoice]
+    created: int = pydantic_v1.Field()
+    """
+    The Unix timestamp (in seconds) of when the completion was created.
+    """
+
+    id: str
+    model: str
+    object: typing.Optional[typing.Any] = None
+    system_fingerprint: str
+    usage: typing.Optional[UsageStats] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `octoai-0.0.4/src/octoai/text_gen/types/chat_completion_chunk.py` & `octoai-0.6.0/src/octoai/text_gen/types/chat_completion_chunk.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,31 +18,28 @@
     choices: typing.List[ChatCompletionChunkChoice] = pydantic_v1.Field()
     """
     A list of chat completion choices.Can be more than one if n is greater than 1.
     """
 
     created: int = pydantic_v1.Field()
     """
-    The Unix timestamp (in seconds) of whenthe chat completion was created. Each chunk has the same timestamp.
+    The Unix timestamp (in seconds) of when the chat completion was created.
     """
 
     id: str = pydantic_v1.Field()
     """
-    A unique identifier for the entire chat completion request.Each chunk in the stream has the same ID.
+    A unique identifier for the entire chat completion request. Each chunk in the stream has the same ID.
     """
 
     model: str = pydantic_v1.Field()
     """
     The model used for the chat completion.
     """
 
-    object: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    The object type, which is always `chat.completion.chunk`.
-    """
+    object: typing.Optional[typing.Any] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `octoai-0.0.4/src/octoai/text_gen/types/chat_completion_chunk_choice.py` & `octoai-0.6.0/src/octoai/text_gen/types/chat_completion_chunk_choice.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/text_gen/types/chat_completion_delta.py` & `octoai-0.6.0/src/octoai/text_gen/types/chat_completion_delta.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/text_gen/types/chat_completion_request_ext.py` & `octoai-0.6.0/src/octoai/text_gen/types/chat_completion_request_ext.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 
 class ChatCompletionRequestExt(pydantic_v1.BaseModel):
     """
     OctoAI specific extensions for a chat completion request.
     """
 
-    loras: typing.Optional[typing.List[str]] = None
     vllm: typing.Optional[ChatCompletionRequestExtVllm] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `octoai-0.0.4/src/octoai/text_gen/types/chat_completion_request_ext_vllm.py` & `octoai-0.6.0/src/octoai/text_gen/types/chat_completion_request_ext_vllm.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/text_gen/types/chat_completion_response.py` & `octoai-0.6.0/src/octoai/text_gen/types/error_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import pydantic_v1
-from .chat_completion_choice import ChatCompletionChoice
-from .usage_stats import UsageStats
+from .error_response_validation_errors_value import ErrorResponseValidationErrorsValue
 
 
-class ChatCompletionResponse(pydantic_v1.BaseModel):
+class ErrorResponse(pydantic_v1.BaseModel):
     """
-    An OpenAI API compatible schema for a chat completion response object.
+    An OpenAI API compatible schema for a error response.
     """
 
-    choices: typing.List[ChatCompletionChoice]
-    created: int
-    id: str
-    model: str
+    code: typing.Optional[str] = None
+    message: str
     object: typing.Optional[str] = None
-    usage: UsageStats
+    param: typing.Optional[str] = None
+    type: str
+    validation_errors: typing.Optional[typing.Dict[str, typing.Optional[ErrorResponseValidationErrorsValue]]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `octoai-0.0.4/src/octoai/text_gen/types/chat_completion_response_format.py` & `octoai-0.6.0/src/octoai/text_gen/types/chat_completion_response_format.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/text_gen/types/chat_fn_call.py` & `octoai-0.6.0/src/octoai/text_gen/types/http_validation_error.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import pydantic_v1
+from .validation_error import ValidationError
 
 
-class ChatFnCall(pydantic_v1.BaseModel):
-    """
-    An OpenAI API compatible schema for a chat function call.
-    """
-
-    arguments: str
-    name: str
+class HttpValidationError(pydantic_v1.BaseModel):
+    detail: typing.Optional[typing.List[ValidationError]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `octoai-0.0.4/src/octoai/text_gen/types/chat_message.py` & `octoai-0.6.0/src/octoai/text_gen/types/chat_message.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/text_gen/types/completion_choice.py` & `octoai-0.6.0/src/octoai/text_gen/types/completion_choice.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import pydantic_v1
+from .finish_reason import FinishReason
 from .log_probs import LogProbs
 
 
 class CompletionChoice(pydantic_v1.BaseModel):
-    finish_reason: typing.Optional[str] = None
+    finish_reason: typing.Optional[FinishReason] = None
     index: int
     logprobs: typing.Optional[LogProbs] = None
     text: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `octoai-0.0.4/src/octoai/text_gen/types/function.py` & `octoai-0.6.0/src/octoai/text_gen/types/function.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/src/octoai/text_gen/types/http_validation_error.py` & `octoai-0.6.0/src/octoai/text_gen/types/validation_error.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import pydantic_v1
-from .validation_error import ValidationError
+from .validation_error_loc_item import ValidationErrorLocItem
 
 
-class HttpValidationError(pydantic_v1.BaseModel):
-    detail: typing.Optional[typing.List[ValidationError]] = None
+class ValidationError(pydantic_v1.BaseModel):
+    loc: typing.List[ValidationErrorLocItem]
+    msg: str
+    type: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `octoai-0.0.4/src/octoai/text_gen/types/log_probs.py` & `octoai-0.6.0/src/octoai/text_gen/types/log_probs.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import pydantic_v1
 
 
 class LogProbs(pydantic_v1.BaseModel):
     """
-    TOOD: write comment
+    The tokens and their [log probabilities](https://en.wikipedia.org/wiki/Log_probability).
     """
 
     text_offset: typing.Optional[typing.List[int]] = None
     token_logprobs: typing.Optional[typing.List[typing.Optional[float]]] = None
     tokens: typing.Optional[typing.List[str]] = None
     top_logprobs: typing.Optional[typing.List[typing.Optional[typing.Dict[str, typing.Optional[float]]]]] = None
```

### Comparing `octoai-0.0.4/src/octoai/text_gen/types/validation_error.py` & `octoai-0.6.0/src/octoai/text_gen/types/chat_completion_choice.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
 from ...core.pydantic_utilities import pydantic_v1
-from .validation_error_loc_item import ValidationErrorLocItem
+from .chat_message import ChatMessage
+from .finish_reason import FinishReason
 
 
-class ValidationError(pydantic_v1.BaseModel):
-    loc: typing.List[ValidationErrorLocItem]
-    msg: str
-    type: str
+class ChatCompletionChoice(pydantic_v1.BaseModel):
+    """
+    A single chat completion choice. A response will contain one or
+    more of these based on the setting of `n`.
+    """
+
+    finish_reason: typing.Optional[FinishReason] = None
+    index: int = pydantic_v1.Field()
+    """
+    A unique identifier for the chat completion.Each chunk has the same ID.
+    """
+
+    message: ChatMessage = pydantic_v1.Field()
+    """
+    A chat completion message generated by the model.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `octoai-0.0.4/src/octoai/uploading_asset_library.py` & `octoai-0.6.0/src/octoai/uploading_asset_library.py`

 * *Files identical despite different names*

### Comparing `octoai-0.0.4/PKG-INFO` & `octoai-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoai
-Version: 0.0.4
+Version: 0.6.0
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

