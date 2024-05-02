# Comparing `tmp/scorecard_ai-0.2.1.tar.gz` & `tmp/scorecard_ai-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scorecard_ai-0.2.1.tar", max compression
+gzip compressed data, was "scorecard_ai-1.0.0b0.tar", max compression
```

## Comparing `scorecard_ai-0.2.1.tar` & `scorecard_ai-1.0.0b0.tar`

### file list

```diff
@@ -1,82 +1,88 @@
--rw-r--r--   0        0        0    11355 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/LICENSE
--rw-r--r--   0        0        0     3605 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/README.md
--rw-r--r--   0        0        0      430 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3159 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/__init__.py
--rw-r--r--   0        0        0     8199 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/client.py
--rw-r--r--   0        0        0      519 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/core/api_error.py
--rw-r--r--   0        0        0     1081 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      162 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/environment.py
--rw-r--r--   0        0        0      363 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/errors/__init__.py
--rw-r--r--   0        0        0      309 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/errors/forbidden_error.py
--rw-r--r--   0        0        0      297 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/errors/not_found_error.py
--rw-r--r--   0        0        0      308 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/errors/unauthorized_error.py
--rw-r--r--   0        0        0      313 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/py.typed
--rw-r--r--   0        0        0      890 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/resources/__init__.py
--rw-r--r--   0        0        0       65 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/resources/run/__init__.py
--rw-r--r--   0        0        0    14688 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/resources/run/client.py
--rw-r--r--   0        0        0       65 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/resources/score/__init__.py
--rw-r--r--   0        0        0    11534 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/resources/score/client.py
--rw-r--r--   0        0        0      255 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/resources/testcase/__init__.py
--rw-r--r--   0        0        0    14479 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/resources/testcase/client.py
--rw-r--r--   0        0        0      347 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/resources/testcase/types/__init__.py
--rw-r--r--   0        0        0      244 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/resources/testcase/types/testcase_create_params_custom_inputs_value.py
--rw-r--r--   0        0        0      244 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/resources/testcase/types/testcase_create_params_custom_labels_value.py
--rw-r--r--   0        0        0      567 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/resources/testrecord/__init__.py
--rw-r--r--   0        0        0    14995 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/resources/testrecord/client.py
--rw-r--r--   0        0        0      812 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/resources/testrecord/types/__init__.py
--rw-r--r--   0        0        0      246 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/resources/testrecord/types/testrecord_create_params_custom_inputs_value.py
--rw-r--r--   0        0        0      246 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/resources/testrecord/types/testrecord_create_params_custom_labels_value.py
--rw-r--r--   0        0        0      247 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/resources/testrecord/types/testrecord_create_params_custom_outputs_value.py
--rw-r--r--   0        0        0      154 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/resources/testrecord/types/testrecord_create_params_model_debug_info_value.py
--rw-r--r--   0        0        0      151 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/resources/testrecord/types/testrecord_create_params_model_params_value.py
--rw-r--r--   0        0        0       65 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/resources/testset/__init__.py
--rw-r--r--   0        0        0    20257 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/resources/testset/client.py
--rw-r--r--   0        0        0     3222 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/__init__.py
--rw-r--r--   0        0        0      112 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/app_create_run_params.py
--rw-r--r--   0        0        0      113 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/app_test_record_create.py
--rw-r--r--   0        0        0      110 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/app_test_set_create.py
--rw-r--r--   0        0        0      120 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/create_github_workflow_params.py
--rw-r--r--   0        0        0      109 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/create_run_params.py
--rw-r--r--   0        0        0     1121 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/custom_schema.py
--rw-r--r--   0        0        0     1116 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/custom_variable.py
--rw-r--r--   0        0        0      695 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/data_type_enum.py
--rw-r--r--   0        0        0      109 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/execution_params.py
--rw-r--r--   0        0        0      945 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/file_url.py
--rw-r--r--   0        0        0     1327 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/grade.py
--rw-r--r--   0        0        0      966 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/http_validation_error.py
--rw-r--r--   0        0        0     1200 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/json_object.py
--rw-r--r--   0        0        0      231 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/json_object_input_value.py
--rw-r--r--   0        0        0      232 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/json_object_output_value.py
--rw-r--r--   0        0        0      105 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/model_params.py
--rw-r--r--   0        0        0      974 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/not_found_error_body.py
--rw-r--r--   0        0        0     1016 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/paginated_testcase_response.py
--rw-r--r--   0        0        0      787 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/role_enum.py
--rw-r--r--   0        0        0     1504 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/run.py
--rw-r--r--   0        0        0     1462 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/run_status.py
--rw-r--r--   0        0        0      114 2024-04-01 19:06:09.832632 scorecard_ai-0.2.1/src/scorecard/types/score_execution_params.py
--rw-r--r--   0        0        0      639 2024-04-01 19:06:09.836632 scorecard_ai-0.2.1/src/scorecard/types/score_status.py
--rw-r--r--   0        0        0      107 2024-04-01 19:06:09.836632 scorecard_ai-0.2.1/src/scorecard/types/scoring_params.py
--rw-r--r--   0        0        0     1363 2024-04-01 19:06:09.836632 scorecard_ai-0.2.1/src/scorecard/types/test_case.py
--rw-r--r--   0        0        0      998 2024-04-01 19:06:09.836632 scorecard_ai-0.2.1/src/scorecard/types/test_case_create.py
--rw-r--r--   0        0        0      113 2024-04-01 19:06:09.836632 scorecard_ai-0.2.1/src/scorecard/types/test_case_create_input.py
--rw-r--r--   0        0        0      214 2024-04-01 19:06:09.836632 scorecard_ai-0.2.1/src/scorecard/types/test_case_custom_inputs_value.py
--rw-r--r--   0        0        0      214 2024-04-01 19:06:09.836632 scorecard_ai-0.2.1/src/scorecard/types/test_case_custom_labels_value.py
--rw-r--r--   0        0        0      110 2024-04-01 19:06:09.836632 scorecard_ai-0.2.1/src/scorecard/types/test_record_create.py
--rw-r--r--   0        0        0      107 2024-04-01 19:06:09.836632 scorecard_ai-0.2.1/src/scorecard/types/test_set_create.py
--rw-r--r--   0        0        0     2148 2024-04-01 19:06:09.836632 scorecard_ai-0.2.1/src/scorecard/types/testrecord.py
--rw-r--r--   0        0        0      216 2024-04-01 19:06:09.836632 scorecard_ai-0.2.1/src/scorecard/types/testrecord_custom_inputs_value.py
--rw-r--r--   0        0        0      216 2024-04-01 19:06:09.836632 scorecard_ai-0.2.1/src/scorecard/types/testrecord_custom_labels_value.py
--rw-r--r--   0        0        0      217 2024-04-01 19:06:09.836632 scorecard_ai-0.2.1/src/scorecard/types/testrecord_custom_outputs_value.py
--rw-r--r--   0        0        0      142 2024-04-01 19:06:09.836632 scorecard_ai-0.2.1/src/scorecard/types/testrecord_model_debug_info_value.py
--rw-r--r--   0        0        0      139 2024-04-01 19:06:09.836632 scorecard_ai-0.2.1/src/scorecard/types/testrecord_model_params_value.py
--rw-r--r--   0        0        0     1366 2024-04-01 19:06:09.836632 scorecard_ai-0.2.1/src/scorecard/types/testset.py
--rw-r--r--   0        0        0      977 2024-04-01 19:06:09.836632 scorecard_ai-0.2.1/src/scorecard/types/unauthenticated_error.py
--rw-r--r--   0        0        0      978 2024-04-01 19:06:09.836632 scorecard_ai-0.2.1/src/scorecard/types/unauthorized_error_body.py
--rw-r--r--   0        0        0      992 2024-04-01 19:06:09.836632 scorecard_ai-0.2.1/src/scorecard/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-01 19:06:09.836632 scorecard_ai-0.2.1/src/scorecard/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     4067 1970-01-01 00:00:00.000000 scorecard_ai-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/LICENSE
+-rw-r--r--   0        0        0     3605 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/README.md
+-rw-r--r--   0        0        0      657 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/pyproject.toml
+-rw-r--r--   0        0        0     3218 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/__init__.py
+-rw-r--r--   0        0        0     6675 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/base_client.py
+-rw-r--r--   0        0        0     4257 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/client.py
+-rw-r--r--   0        0        0     1006 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/api_error.py
+-rw-r--r--   0        0        0     1494 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/request_options.py
+-rw-r--r--   0        0        0     7123 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/core/unchecked_base_model.py
+-rw-r--r--   0        0        0      162 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/environment.py
+-rw-r--r--   0        0        0      363 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/errors/__init__.py
+-rw-r--r--   0        0        0      309 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/errors/forbidden_error.py
+-rw-r--r--   0        0        0      297 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/errors/not_found_error.py
+-rw-r--r--   0        0        0      308 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      313 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/py.typed
+-rw-r--r--   0        0        0       65 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/run/__init__.py
+-rw-r--r--   0        0        0    24116 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/run/client.py
+-rw-r--r--   0        0        0       65 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/score/__init__.py
+-rw-r--r--   0        0        0    18323 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/score/client.py
+-rw-r--r--   0        0        0      255 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testcase/__init__.py
+-rw-r--r--   0        0        0    23624 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testcase/client.py
+-rw-r--r--   0        0        0      347 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testcase/types/__init__.py
+-rw-r--r--   0        0        0      242 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testcase/types/testcase_create_params_custom_inputs_value.py
+-rw-r--r--   0        0        0      242 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testcase/types/testcase_create_params_custom_labels_value.py
+-rw-r--r--   0        0        0      567 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testrecord/__init__.py
+-rw-r--r--   0        0        0    21204 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testrecord/client.py
+-rw-r--r--   0        0        0      812 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testrecord/types/__init__.py
+-rw-r--r--   0        0        0      244 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testrecord/types/testrecord_create_params_custom_inputs_value.py
+-rw-r--r--   0        0        0      244 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testrecord/types/testrecord_create_params_custom_labels_value.py
+-rw-r--r--   0        0        0      245 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testrecord/types/testrecord_create_params_custom_outputs_value.py
+-rw-r--r--   0        0        0      154 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testrecord/types/testrecord_create_params_model_debug_info_value.py
+-rw-r--r--   0        0        0      151 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testrecord/types/testrecord_create_params_model_params_value.py
+-rw-r--r--   0        0        0       65 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testset/__init__.py
+-rw-r--r--   0        0        0    35470 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/testset/client.py
+-rw-r--r--   0        0        0     3222 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/types/__init__.py
+-rw-r--r--   0        0        0      112 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/types/app_create_run_params.py
+-rw-r--r--   0        0        0      113 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/types/app_test_record_create.py
+-rw-r--r--   0        0        0      110 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/types/app_test_set_create.py
+-rw-r--r--   0        0        0      120 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/types/create_github_workflow_params.py
+-rw-r--r--   0        0        0      109 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/types/create_run_params.py
+-rw-r--r--   0        0        0     1165 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/types/custom_schema.py
+-rw-r--r--   0        0        0     1159 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/types/custom_variable.py
+-rw-r--r--   0        0        0      171 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/types/data_type_enum.py
+-rw-r--r--   0        0        0      109 2024-05-02 01:57:29.255855 scorecard_ai-1.0.0b0/src/scorecard/types/execution_params.py
+-rw-r--r--   0        0        0      988 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/file_url.py
+-rw-r--r--   0        0        0     1447 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/grade.py
+-rw-r--r--   0        0        0     1009 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/http_validation_error.py
+-rw-r--r--   0        0        0     1244 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/json_object.py
+-rw-r--r--   0        0        0      231 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/json_object_input_value.py
+-rw-r--r--   0        0        0      232 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/json_object_output_value.py
+-rw-r--r--   0        0        0      105 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/model_params.py
+-rw-r--r--   0        0        0     1031 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/not_found_error_body.py
+-rw-r--r--   0        0        0     1066 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/paginated_testcase_response.py
+-rw-r--r--   0        0        0      172 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/role_enum.py
+-rw-r--r--   0        0        0     1645 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/run.py
+-rw-r--r--   0        0        0      339 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/run_status.py
+-rw-r--r--   0        0        0      114 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/score_execution_params.py
+-rw-r--r--   0        0        0      168 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/score_status.py
+-rw-r--r--   0        0        0      107 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/scoring_params.py
+-rw-r--r--   0        0        0     1441 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/test_case.py
+-rw-r--r--   0        0        0     1055 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/test_case_create.py
+-rw-r--r--   0        0        0      113 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/test_case_create_input.py
+-rw-r--r--   0        0        0      214 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/test_case_custom_inputs_value.py
+-rw-r--r--   0        0        0      214 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/test_case_custom_labels_value.py
+-rw-r--r--   0        0        0      110 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/test_record_create.py
+-rw-r--r--   0        0        0      107 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/test_set_create.py
+-rw-r--r--   0        0        0     2303 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/testrecord.py
+-rw-r--r--   0        0        0      216 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/testrecord_custom_inputs_value.py
+-rw-r--r--   0        0        0      216 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/testrecord_custom_labels_value.py
+-rw-r--r--   0        0        0      217 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/testrecord_custom_outputs_value.py
+-rw-r--r--   0        0        0      142 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/testrecord_model_debug_info_value.py
+-rw-r--r--   0        0        0      139 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/testrecord_model_params_value.py
+-rw-r--r--   0        0        0     1486 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/testset.py
+-rw-r--r--   0        0        0     1034 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/unauthenticated_error.py
+-rw-r--r--   0        0        0     1035 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/unauthorized_error_body.py
+-rw-r--r--   0        0        0     1028 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0       80 2024-05-02 01:57:29.259855 scorecard_ai-1.0.0b0/src/scorecard/version.py
+-rw-r--r--   0        0        0     4105 1970-01-01 00:00:00.000000 scorecard_ai-1.0.0b0/PKG-INFO
```

### Comparing `scorecard_ai-0.2.1/LICENSE` & `scorecard_ai-1.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `scorecard_ai-0.2.1/README.md` & `scorecard_ai-1.0.0b0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 scorecard_client = Scorecard(
   api_key="YOUR_API_KEY",
   timeout=15,
 )
 ```
 
 ## Handling Exceptions
-All exceptions thrown by the SDK will sublcass [scorecard.ApiError](./src/scorecard/core/api_error.py). 
+All exceptions thrown by the SDK will subclass [scorecard.ApiError](./src/scorecard/core/api_error.py). 
 
 ```python
 from scorecard.core import ApiError
 from scorecard import UnprocessableEntityError
 
 try:
   client.testset.get("testset-id")
```

### Comparing `scorecard_ai-0.2.1/src/scorecard/__init__.py` & `scorecard_ai-1.0.0b0/src/scorecard/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,29 +41,25 @@
     Testset,
     UnauthenticatedError,
     UnauthorizedErrorBody,
     ValidationError,
     ValidationErrorLocItem,
 )
 from .errors import ForbiddenError, NotFoundError, UnauthorizedError, UnprocessableEntityError
-from .resources import (
-    TestcaseCreateParamsCustomInputsValue,
-    TestcaseCreateParamsCustomLabelsValue,
+from . import run, score, testcase, testrecord, testset
+from .environment import ScorecardEnvironment
+from .testcase import TestcaseCreateParamsCustomInputsValue, TestcaseCreateParamsCustomLabelsValue
+from .testrecord import (
     TestrecordCreateParamsCustomInputsValue,
     TestrecordCreateParamsCustomLabelsValue,
     TestrecordCreateParamsCustomOutputsValue,
     TestrecordCreateParamsModelDebugInfoValue,
     TestrecordCreateParamsModelParamsValue,
-    run,
-    score,
-    testcase,
-    testrecord,
-    testset,
 )
-from .environment import ScorecardEnvironment
+from .version import __version__
 
 __all__ = [
     "AppCreateRunParams",
     "AppTestRecordCreate",
     "AppTestSetCreate",
     "CreateGithubWorkflowParams",
     "CreateRunParams",
@@ -112,13 +108,14 @@
     "Testset",
     "UnauthenticatedError",
     "UnauthorizedError",
     "UnauthorizedErrorBody",
     "UnprocessableEntityError",
     "ValidationError",
     "ValidationErrorLocItem",
+    "__version__",
     "run",
     "score",
     "testcase",
     "testrecord",
     "testset",
 ]
```

### Comparing `scorecard_ai-0.2.1/src/scorecard/core/client_wrapper.py` & `scorecard_ai-1.0.0b0/src/scorecard/core/client_wrapper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 
 import httpx
 
+from .http_client import AsyncHttpClient, HttpClient
+
 
 class BaseClientWrapper:
-    def __init__(self, *, api_key: str, base_url: str):
+    def __init__(self, *, api_key: str, base_url: str, timeout: typing.Optional[float] = None):
         self.api_key = api_key
         self._base_url = base_url
+        self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "scorecard-ai",
-            "X-Fern-SDK-Version": "0.2.1",
+            "X-Fern-SDK-Version": "v1.0.0-beta0",
         }
         headers["X-API-Key"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
 
+    def get_timeout(self) -> typing.Optional[float]:
+        return self._timeout
+
 
 class SyncClientWrapper(BaseClientWrapper):
-    def __init__(self, *, api_key: str, base_url: str, httpx_client: httpx.Client):
-        super().__init__(api_key=api_key, base_url=base_url)
-        self.httpx_client = httpx_client
+    def __init__(
+        self, *, api_key: str, base_url: str, timeout: typing.Optional[float] = None, httpx_client: httpx.Client
+    ):
+        super().__init__(api_key=api_key, base_url=base_url, timeout=timeout)
+        self.httpx_client = HttpClient(httpx_client=httpx_client)
 
 
 class AsyncClientWrapper(BaseClientWrapper):
-    def __init__(self, *, api_key: str, base_url: str, httpx_client: httpx.AsyncClient):
-        super().__init__(api_key=api_key, base_url=base_url)
-        self.httpx_client = httpx_client
+    def __init__(
+        self, *, api_key: str, base_url: str, timeout: typing.Optional[float] = None, httpx_client: httpx.AsyncClient
+    ):
+        super().__init__(api_key=api_key, base_url=base_url, timeout=timeout)
+        self.httpx_client = AsyncHttpClient(httpx_client=httpx_client)
```

### Comparing `scorecard_ai-0.2.1/src/scorecard/core/datetime_utils.py` & `scorecard_ai-1.0.0b0/src/scorecard/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-0.2.1/src/scorecard/core/jsonable_encoder.py` & `scorecard_ai-1.0.0b0/src/scorecard/core/jsonable_encoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,47 +12,43 @@
 import datetime as dt
 from collections import defaultdict
 from enum import Enum
 from pathlib import PurePath
 from types import GeneratorType
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 from .datetime_utils import serialize_datetime
+from .pydantic_utilities import pydantic_v1
 
 SetIntStr = Set[Union[int, str]]
 DictIntStrAny = Dict[Union[int, str], Any]
 
 
 def generate_encoders_by_class_tuples(
     type_encoder_map: Dict[Any, Callable[[Any], Any]]
 ) -> Dict[Callable[[Any], Any], Tuple[Any, ...]]:
     encoders_by_class_tuples: Dict[Callable[[Any], Any], Tuple[Any, ...]] = defaultdict(tuple)
     for type_, encoder in type_encoder_map.items():
         encoders_by_class_tuples[encoder] += (type_,)
     return encoders_by_class_tuples
 
 
-encoders_by_class_tuples = generate_encoders_by_class_tuples(pydantic.json.ENCODERS_BY_TYPE)
+encoders_by_class_tuples = generate_encoders_by_class_tuples(pydantic_v1.json.ENCODERS_BY_TYPE)
 
 
 def jsonable_encoder(obj: Any, custom_encoder: Optional[Dict[Any, Callable[[Any], Any]]] = None) -> Any:
     custom_encoder = custom_encoder or {}
     if custom_encoder:
         if type(obj) in custom_encoder:
             return custom_encoder[type(obj)](obj)
         else:
             for encoder_type, encoder_instance in custom_encoder.items():
                 if isinstance(obj, encoder_type):
                     return encoder_instance(obj)
-    if isinstance(obj, pydantic.BaseModel):
+    if isinstance(obj, pydantic_v1.BaseModel):
         encoder = getattr(obj.__config__, "json_encoders", {})
         if custom_encoder:
             encoder.update(custom_encoder)
         obj_dict = obj.dict(by_alias=True)
         if "__root__" in obj_dict:
             obj_dict = obj_dict["__root__"]
         return jsonable_encoder(obj_dict, custom_encoder=encoder)
@@ -61,18 +57,18 @@
         return jsonable_encoder(obj_dict, custom_encoder=custom_encoder)
     if isinstance(obj, Enum):
         return obj.value
     if isinstance(obj, PurePath):
         return str(obj)
     if isinstance(obj, (str, int, float, type(None))):
         return obj
-    if isinstance(obj, dt.date):
-        return str(obj)
     if isinstance(obj, dt.datetime):
         return serialize_datetime(obj)
+    if isinstance(obj, dt.date):
+        return str(obj)
     if isinstance(obj, dict):
         encoded_dict = {}
         allowed_keys = set(obj.keys())
         for key, value in obj.items():
             if key in allowed_keys:
                 encoded_key = jsonable_encoder(key, custom_encoder=custom_encoder)
                 encoded_value = jsonable_encoder(value, custom_encoder=custom_encoder)
@@ -80,16 +76,16 @@
         return encoded_dict
     if isinstance(obj, (list, set, frozenset, GeneratorType, tuple)):
         encoded_list = []
         for item in obj:
             encoded_list.append(jsonable_encoder(item, custom_encoder=custom_encoder))
         return encoded_list
 
-    if type(obj) in pydantic.json.ENCODERS_BY_TYPE:
-        return pydantic.json.ENCODERS_BY_TYPE[type(obj)](obj)
+    if type(obj) in pydantic_v1.json.ENCODERS_BY_TYPE:
+        return pydantic_v1.json.ENCODERS_BY_TYPE[type(obj)](obj)
     for encoder, classes_tuple in encoders_by_class_tuples.items():
         if isinstance(obj, classes_tuple):
             return encoder(obj)
 
     try:
         data = dict(obj)
     except Exception as e:
```

### Comparing `scorecard_ai-0.2.1/src/scorecard/resources/__init__.py` & `scorecard_ai-1.0.0b0/src/scorecard/testrecord/types/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from . import run, score, testcase, testrecord, testset
-from .testcase import TestcaseCreateParamsCustomInputsValue, TestcaseCreateParamsCustomLabelsValue
-from .testrecord import (
-    TestrecordCreateParamsCustomInputsValue,
-    TestrecordCreateParamsCustomLabelsValue,
-    TestrecordCreateParamsCustomOutputsValue,
-    TestrecordCreateParamsModelDebugInfoValue,
-    TestrecordCreateParamsModelParamsValue,
-)
+from .testrecord_create_params_custom_inputs_value import TestrecordCreateParamsCustomInputsValue
+from .testrecord_create_params_custom_labels_value import TestrecordCreateParamsCustomLabelsValue
+from .testrecord_create_params_custom_outputs_value import TestrecordCreateParamsCustomOutputsValue
+from .testrecord_create_params_model_debug_info_value import TestrecordCreateParamsModelDebugInfoValue
+from .testrecord_create_params_model_params_value import TestrecordCreateParamsModelParamsValue
 
 __all__ = [
-    "TestcaseCreateParamsCustomInputsValue",
-    "TestcaseCreateParamsCustomLabelsValue",
     "TestrecordCreateParamsCustomInputsValue",
     "TestrecordCreateParamsCustomLabelsValue",
     "TestrecordCreateParamsCustomOutputsValue",
     "TestrecordCreateParamsModelDebugInfoValue",
     "TestrecordCreateParamsModelParamsValue",
-    "run",
-    "score",
-    "testcase",
-    "testrecord",
-    "testset",
 ]
```

### Comparing `scorecard_ai-0.2.1/src/scorecard/resources/testrecord/__init__.py` & `scorecard_ai-1.0.0b0/src/scorecard/testrecord/__init__.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-0.2.1/src/scorecard/resources/testrecord/client.py` & `scorecard_ai-1.0.0b0/src/scorecard/testrecord/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,115 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
-from ...core.api_error import ApiError
-from ...core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
-from ...core.jsonable_encoder import jsonable_encoder
-from ...errors.forbidden_error import ForbiddenError
-from ...errors.not_found_error import NotFoundError
-from ...errors.unauthorized_error import UnauthorizedError
-from ...errors.unprocessable_entity_error import UnprocessableEntityError
-from ...types.http_validation_error import HttpValidationError
-from ...types.not_found_error_body import NotFoundErrorBody
-from ...types.testrecord import Testrecord
-from ...types.unauthenticated_error import UnauthenticatedError
-from ...types.unauthorized_error_body import UnauthorizedErrorBody
+from ..core.api_error import ApiError
+from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
+from ..core.jsonable_encoder import jsonable_encoder
+from ..core.remove_none_from_dict import remove_none_from_dict
+from ..core.request_options import RequestOptions
+from ..core.unchecked_base_model import construct_type
+from ..errors.forbidden_error import ForbiddenError
+from ..errors.not_found_error import NotFoundError
+from ..errors.unauthorized_error import UnauthorizedError
+from ..errors.unprocessable_entity_error import UnprocessableEntityError
+from ..types.http_validation_error import HttpValidationError
+from ..types.not_found_error_body import NotFoundErrorBody
+from ..types.testrecord import Testrecord
+from ..types.unauthenticated_error import UnauthenticatedError
+from ..types.unauthorized_error_body import UnauthorizedErrorBody
 from .types.testrecord_create_params_custom_inputs_value import TestrecordCreateParamsCustomInputsValue
 from .types.testrecord_create_params_custom_labels_value import TestrecordCreateParamsCustomLabelsValue
 from .types.testrecord_create_params_custom_outputs_value import TestrecordCreateParamsCustomOutputsValue
 from .types.testrecord_create_params_model_debug_info_value import TestrecordCreateParamsModelDebugInfoValue
 from .types.testrecord_create_params_model_params_value import TestrecordCreateParamsModelParamsValue
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
 # this is used as the default value for optional parameters
 OMIT = typing.cast(typing.Any, ...)
 
 
 class TestrecordClient:
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    def get(self, testrecord_id: int, run_id: int) -> Testrecord:
+    def get(
+        self, testrecord_id: int, run_id: int, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> Testrecord:
         """
         Retrieve Testrecord metadata
 
-        Parameters:
-            - testrecord_id: int.
+        Parameters
+        ----------
+        testrecord_id : int
+
+        run_id : int
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Testrecord
+            Successful Response
 
-            - run_id: int.
-        ---
+        Examples
+        --------
         from scorecard.client import Scorecard
 
         client = Scorecard(
             api_key="YOUR_API_KEY",
         )
         client.testrecord.get(
             testrecord_id=1,
             run_id=1,
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/run/{run_id}/testrecord/{testrecord_id}"
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"v1/run/{jsonable_encoder(run_id)}/testrecord/{jsonable_encoder(testrecord_id)}",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
             ),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Testrecord, _response.json())  # type: ignore
+            return typing.cast(Testrecord, construct_type(type_=Testrecord, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(UnauthenticatedError, _response.json()))  # type: ignore
+            raise UnauthorizedError(
+                typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 403:
-            raise ForbiddenError(pydantic.parse_obj_as(UnauthorizedErrorBody, _response.json()))  # type: ignore
+            raise ForbiddenError(
+                typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(NotFoundErrorBody, _response.json()))  # type: ignore
+            raise NotFoundError(
+                typing.cast(NotFoundErrorBody, construct_type(type_=NotFoundErrorBody, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
@@ -98,45 +132,57 @@
             typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomLabelsValue]]
         ] = OMIT,
         prompt: typing.Optional[str] = OMIT,
         model_params: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsModelParamsValue]]] = OMIT,
         model_debug_info: typing.Optional[
             typing.Dict[str, typing.Optional[TestrecordCreateParamsModelDebugInfoValue]]
         ] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
     ) -> Testrecord:
         """
         Create a new Testrecord
 
-        Parameters:
-            - run_id: int.
+        Parameters
+        ----------
+        run_id : int
+
+        testset_id : typing.Optional[int]
 
-            - testset_id: typing.Optional[int].
+        testcase_id : typing.Optional[int]
 
-            - testcase_id: typing.Optional[int].
+        user_query : typing.Optional[str]
 
-            - user_query: typing.Optional[str].
+        context : typing.Optional[str]
 
-            - context: typing.Optional[str].
+        response : typing.Optional[str]
 
-            - response: typing.Optional[str].
+        ideal : typing.Optional[str]
 
-            - ideal: typing.Optional[str].
+        custom_inputs : typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomInputsValue]]]
 
-            - custom_inputs: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomInputsValue]]].
+        custom_outputs : typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomOutputsValue]]]
 
-            - custom_outputs: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomOutputsValue]]].
+        custom_labels : typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomLabelsValue]]]
 
-            - custom_labels: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomLabelsValue]]].
+        prompt : typing.Optional[str]
 
-            - prompt: typing.Optional[str].
+        model_params : typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsModelParamsValue]]]
 
-            - model_params: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsModelParamsValue]]].
+        model_debug_info : typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsModelDebugInfoValue]]]
 
-            - model_debug_info: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsModelDebugInfoValue]]].
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Testrecord
+            Successful Response
+
+        Examples
+        --------
         from scorecard.client import Scorecard
 
         client = Scorecard(
             api_key="YOUR_API_KEY",
         )
         client.testrecord.create(
             run_id=1,
@@ -164,78 +210,143 @@
         if prompt is not OMIT:
             _request["prompt"] = prompt
         if model_params is not OMIT:
             _request["model_params"] = model_params
         if model_debug_info is not OMIT:
             _request["model_debug_info"] = model_debug_info
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/run/{run_id}/testrecord"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            method="POST",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/run/{jsonable_encoder(run_id)}/testrecord"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Testrecord, _response.json())  # type: ignore
+            return typing.cast(Testrecord, construct_type(type_=Testrecord, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(UnauthenticatedError, _response.json()))  # type: ignore
+            raise UnauthorizedError(
+                typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 403:
-            raise ForbiddenError(pydantic.parse_obj_as(UnauthorizedErrorBody, _response.json()))  # type: ignore
+            raise ForbiddenError(
+                typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(NotFoundErrorBody, _response.json()))  # type: ignore
+            raise NotFoundError(
+                typing.cast(NotFoundErrorBody, construct_type(type_=NotFoundErrorBody, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncTestrecordClient:
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
-    async def get(self, testrecord_id: int, run_id: int) -> Testrecord:
+    async def get(
+        self, testrecord_id: int, run_id: int, *, request_options: typing.Optional[RequestOptions] = None
+    ) -> Testrecord:
         """
         Retrieve Testrecord metadata
 
-        Parameters:
-            - testrecord_id: int.
+        Parameters
+        ----------
+        testrecord_id : int
+
+        run_id : int
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Testrecord
+            Successful Response
 
-            - run_id: int.
-        ---
+        Examples
+        --------
         from scorecard.client import AsyncScorecard
 
         client = AsyncScorecard(
             api_key="YOUR_API_KEY",
         )
         await client.testrecord.get(
             testrecord_id=1,
             run_id=1,
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
-                f"{self._client_wrapper.get_base_url()}/", f"v1/run/{run_id}/testrecord/{testrecord_id}"
+            method="GET",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/",
+                f"v1/run/{jsonable_encoder(run_id)}/testrecord/{jsonable_encoder(testrecord_id)}",
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
             ),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Testrecord, _response.json())  # type: ignore
+            return typing.cast(Testrecord, construct_type(type_=Testrecord, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(UnauthenticatedError, _response.json()))  # type: ignore
+            raise UnauthorizedError(
+                typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 403:
-            raise ForbiddenError(pydantic.parse_obj_as(UnauthorizedErrorBody, _response.json()))  # type: ignore
+            raise ForbiddenError(
+                typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(NotFoundErrorBody, _response.json()))  # type: ignore
+            raise NotFoundError(
+                typing.cast(NotFoundErrorBody, construct_type(type_=NotFoundErrorBody, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
@@ -258,45 +369,57 @@
             typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomLabelsValue]]
         ] = OMIT,
         prompt: typing.Optional[str] = OMIT,
         model_params: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsModelParamsValue]]] = OMIT,
         model_debug_info: typing.Optional[
             typing.Dict[str, typing.Optional[TestrecordCreateParamsModelDebugInfoValue]]
         ] = OMIT,
+        request_options: typing.Optional[RequestOptions] = None,
     ) -> Testrecord:
         """
         Create a new Testrecord
 
-        Parameters:
-            - run_id: int.
+        Parameters
+        ----------
+        run_id : int
+
+        testset_id : typing.Optional[int]
+
+        testcase_id : typing.Optional[int]
 
-            - testset_id: typing.Optional[int].
+        user_query : typing.Optional[str]
 
-            - testcase_id: typing.Optional[int].
+        context : typing.Optional[str]
 
-            - user_query: typing.Optional[str].
+        response : typing.Optional[str]
 
-            - context: typing.Optional[str].
+        ideal : typing.Optional[str]
 
-            - response: typing.Optional[str].
+        custom_inputs : typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomInputsValue]]]
 
-            - ideal: typing.Optional[str].
+        custom_outputs : typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomOutputsValue]]]
 
-            - custom_inputs: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomInputsValue]]].
+        custom_labels : typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomLabelsValue]]]
 
-            - custom_outputs: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomOutputsValue]]].
+        prompt : typing.Optional[str]
 
-            - custom_labels: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsCustomLabelsValue]]].
+        model_params : typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsModelParamsValue]]]
 
-            - prompt: typing.Optional[str].
+        model_debug_info : typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsModelDebugInfoValue]]]
 
-            - model_params: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsModelParamsValue]]].
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - model_debug_info: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCreateParamsModelDebugInfoValue]]].
-        ---
+        Returns
+        -------
+        Testrecord
+            Successful Response
+
+        Examples
+        --------
         from scorecard.client import AsyncScorecard
 
         client = AsyncScorecard(
             api_key="YOUR_API_KEY",
         )
         await client.testrecord.create(
             run_id=1,
@@ -324,28 +447,57 @@
         if prompt is not OMIT:
             _request["prompt"] = prompt
         if model_params is not OMIT:
             _request["model_params"] = model_params
         if model_debug_info is not OMIT:
             _request["model_debug_info"] = model_debug_info
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"v1/run/{run_id}/testrecord"),
-            json=jsonable_encoder(_request),
-            headers=self._client_wrapper.get_headers(),
-            timeout=60,
+            method="POST",
+            url=urllib.parse.urljoin(
+                f"{self._client_wrapper.get_base_url()}/", f"v1/run/{jsonable_encoder(run_id)}/testrecord"
+            ),
+            params=jsonable_encoder(
+                request_options.get("additional_query_parameters") if request_options is not None else None
+            ),
+            json=jsonable_encoder(_request)
+            if request_options is None or request_options.get("additional_body_parameters") is None
+            else {
+                **jsonable_encoder(_request),
+                **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
+            },
+            headers=jsonable_encoder(
+                remove_none_from_dict(
+                    {
+                        **self._client_wrapper.get_headers(),
+                        **(request_options.get("additional_headers", {}) if request_options is not None else {}),
+                    }
+                )
+            ),
+            timeout=request_options.get("timeout_in_seconds")
+            if request_options is not None and request_options.get("timeout_in_seconds") is not None
+            else self._client_wrapper.get_timeout(),
+            retries=0,
+            max_retries=request_options.get("max_retries") if request_options is not None else 0,  # type: ignore
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(Testrecord, _response.json())  # type: ignore
+            return typing.cast(Testrecord, construct_type(type_=Testrecord, object_=_response.json()))  # type: ignore
         if _response.status_code == 401:
-            raise UnauthorizedError(pydantic.parse_obj_as(UnauthenticatedError, _response.json()))  # type: ignore
+            raise UnauthorizedError(
+                typing.cast(UnauthenticatedError, construct_type(type_=UnauthenticatedError, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 403:
-            raise ForbiddenError(pydantic.parse_obj_as(UnauthorizedErrorBody, _response.json()))  # type: ignore
+            raise ForbiddenError(
+                typing.cast(UnauthorizedErrorBody, construct_type(type_=UnauthorizedErrorBody, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 404:
-            raise NotFoundError(pydantic.parse_obj_as(NotFoundErrorBody, _response.json()))  # type: ignore
+            raise NotFoundError(
+                typing.cast(NotFoundErrorBody, construct_type(type_=NotFoundErrorBody, object_=_response.json()))  # type: ignore
+            )
         if _response.status_code == 422:
-            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+            raise UnprocessableEntityError(
+                typing.cast(HttpValidationError, construct_type(type_=HttpValidationError, object_=_response.json()))  # type: ignore
+            )
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `scorecard_ai-0.2.1/src/scorecard/types/__init__.py` & `scorecard_ai-1.0.0b0/src/scorecard/types/__init__.py`

 * *Files identical despite different names*

### Comparing `scorecard_ai-0.2.1/src/scorecard/types/custom_schema.py` & `scorecard_ai-1.0.0b0/src/scorecard/types/custom_schema.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .custom_variable import CustomVariable
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class CustomSchema(pydantic.BaseModel):
+class CustomSchema(UncheckedBaseModel):
     """
     Custom schema model with an ordered list of custom variables.
     """
 
-    variables: typing.Optional[typing.List[CustomVariable]] = pydantic.Field(
-        description="Ordered list of custom variables"
-    )
+    variables: typing.Optional[typing.List[CustomVariable]] = pydantic_v1.Field(default=None)
+    """
+    Ordered list of custom variables
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-0.2.1/src/scorecard/types/custom_variable.py` & `scorecard_ai-1.0.0b0/src/scorecard/types/custom_variable.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .data_type_enum import DataTypeEnum
 from .role_enum import RoleEnum
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class CustomVariable(pydantic.BaseModel):
+class CustomVariable(UncheckedBaseModel):
     """
     Custom variable model with name, description, role and data type.
     """
 
     name: str
-    description: typing.Optional[str]
+    description: typing.Optional[str] = None
     role: RoleEnum
     data_type: DataTypeEnum
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-0.2.1/src/scorecard/types/file_url.py` & `scorecard_ai-1.0.0b0/src/scorecard/types/json_object.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
+from __future__ import annotations
+
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class FileUrl(pydantic.BaseModel):
+class JsonObject(UncheckedBaseModel):
+    value: typing.Optional[JsonObjectOutputValue] = pydantic_v1.Field(default=None)
     """
-    File model with url and name.
+    The value of the JSON object, which can be a dictionary, list, string, integer, float, boolean, or None.
     """
 
-    url: str
-    name: typing.Optional[str]
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
+
+
+from .json_object_output_value import JsonObjectOutputValue  # noqa: E402
+
+JsonObject.update_forward_refs()
```

### Comparing `scorecard_ai-0.2.1/src/scorecard/types/grade.py` & `scorecard_ai-1.0.0b0/src/scorecard/types/run.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .score_status import ScoreStatus
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class Grade(pydantic.BaseModel):
-    id: typing.Optional[int]
-    run_id: typing.Optional[int]
-    testcase_id: typing.Optional[int]
-    testrecord_id: typing.Optional[int]
-    metric_id: typing.Optional[int]
-    user_id: typing.Optional[str]
-    binary_score: typing.Optional[bool]
-    int_score: typing.Optional[int]
-    reasoning: typing.Optional[str]
-    human_eval: typing.Optional[bool]
-    status: typing.Optional[ScoreStatus]
-    error_message: typing.Optional[str]
+
+class Run(UncheckedBaseModel):
+    id: typing.Optional[int] = None
+    created_at: typing.Optional[dt.datetime] = None
+    updated_at: typing.Optional[dt.datetime] = None
+    execution_start_time: typing.Optional[dt.datetime] = None
+    execution_end_time: typing.Optional[dt.datetime] = None
+    testset_id: typing.Optional[int] = None
+    status: typing.Optional[str] = None
+    limit_testcases: typing.Optional[int] = None
+    source: typing.Optional[str] = None
+    model_params: typing.Optional[typing.Dict[str, typing.Any]] = None
+    notes: typing.Optional[str] = None
+    scoring_config_id: typing.Optional[int] = None
+    prompt_template: typing.Optional[str] = None
+    scoring_start_time: typing.Optional[dt.datetime] = None
+    scoring_end_time: typing.Optional[dt.datetime] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-0.2.1/src/scorecard/types/http_validation_error.py` & `scorecard_ai-1.0.0b0/src/scorecard/types/test_case_create.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .validation_error import ValidationError
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class HttpValidationError(pydantic.BaseModel):
-    detail: typing.Optional[typing.List[ValidationError]]
+class TestCaseCreate(UncheckedBaseModel):
+    testset_id: int
+    user_query: str
+    context: typing.Optional[str] = None
+    response: typing.Optional[str] = None
+    ideal: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-0.2.1/src/scorecard/types/json_object.py` & `scorecard_ai-1.0.0b0/src/scorecard/types/not_found_error_body.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from __future__ import annotations
-
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class JsonObject(pydantic.BaseModel):
-    value: typing.Optional[JsonObjectOutputValue] = pydantic.Field(
-        description="The value of the JSON object, which can be a dictionary, list, string, integer, float, boolean, or None."
-    )
+class NotFoundErrorBody(UncheckedBaseModel):
+    error: typing.Optional[str] = None
+    error_description: typing.Optional[str] = None
+    status_code: typing.Optional[int] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
-
-
-from .json_object_output_value import JsonObjectOutputValue  # noqa: E402
-
-JsonObject.update_forward_refs()
```

### Comparing `scorecard_ai-0.2.1/src/scorecard/types/not_found_error_body.py` & `scorecard_ai-1.0.0b0/src/scorecard/types/validation_error.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .validation_error_loc_item import ValidationErrorLocItem
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class NotFoundErrorBody(pydantic.BaseModel):
-    error: typing.Optional[str]
-    error_description: typing.Optional[str]
-    status_code: typing.Optional[int]
+class ValidationError(UncheckedBaseModel):
+    loc: typing.List[ValidationErrorLocItem]
+    msg: str
+    type: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-0.2.1/src/scorecard/types/paginated_testcase_response.py` & `scorecard_ai-1.0.0b0/src/scorecard/types/paginated_testcase_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .test_case import TestCase
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class PaginatedTestcaseResponse(pydantic.BaseModel):
+class PaginatedTestcaseResponse(UncheckedBaseModel):
     count: int
-    next: typing.Optional[str]
-    previous: typing.Optional[str]
+    next: typing.Optional[str] = None
+    previous: typing.Optional[str] = None
     results: typing.List[TestCase]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-0.2.1/src/scorecard/types/test_case.py` & `scorecard_ai-1.0.0b0/src/scorecard/types/file_url.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .test_case_custom_inputs_value import TestCaseCustomInputsValue
-from .test_case_custom_labels_value import TestCaseCustomLabelsValue
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class TestCase(pydantic.BaseModel):
-    id: typing.Optional[int]
-    created_at: typing.Optional[dt.datetime]
-    testset_id: int
-    user_query: str
-    context: typing.Optional[str]
-    ideal: typing.Optional[str]
-    custom_inputs: typing.Optional[typing.Dict[str, typing.Optional[TestCaseCustomInputsValue]]]
-    custom_labels: typing.Optional[typing.Dict[str, typing.Optional[TestCaseCustomLabelsValue]]]
+
+class FileUrl(UncheckedBaseModel):
+    """
+    File model with url and name.
+    """
+
+    url: str
+    name: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-0.2.1/src/scorecard/types/test_case_create.py` & `scorecard_ai-1.0.0b0/src/scorecard/types/unauthorized_error_body.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class TestCaseCreate(pydantic.BaseModel):
-    testset_id: int
-    user_query: str
-    context: typing.Optional[str]
-    response: typing.Optional[str]
-    ideal: typing.Optional[str]
+class UnauthorizedErrorBody(UncheckedBaseModel):
+    error: typing.Optional[str] = None
+    error_description: typing.Optional[str] = None
+    status_code: typing.Optional[int] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-0.2.1/src/scorecard/types/testrecord.py` & `scorecard_ai-1.0.0b0/src/scorecard/types/testrecord.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 from .testrecord_custom_inputs_value import TestrecordCustomInputsValue
 from .testrecord_custom_labels_value import TestrecordCustomLabelsValue
 from .testrecord_custom_outputs_value import TestrecordCustomOutputsValue
 from .testrecord_model_debug_info_value import TestrecordModelDebugInfoValue
 from .testrecord_model_params_value import TestrecordModelParamsValue
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class Testrecord(pydantic.BaseModel):
-    id: typing.Optional[int]
-    created_at: typing.Optional[dt.datetime]
-    run_id: typing.Optional[int]
-    testset_id: typing.Optional[int]
-    testcase_id: typing.Optional[int]
-    user_query: typing.Optional[str]
-    context: typing.Optional[str]
-    model_response: typing.Optional[str]
-    ideal: typing.Optional[str]
-    full_prompt: typing.Optional[str]
-    custom_inputs: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCustomInputsValue]]]
-    custom_labels: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCustomLabelsValue]]]
-    custom_outputs: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCustomOutputsValue]]]
-    status: typing.Optional[str]
-    prompt: typing.Optional[str]
-    model_params: typing.Optional[typing.Dict[str, typing.Optional[TestrecordModelParamsValue]]]
-    model_debug_info: typing.Optional[typing.Dict[str, typing.Optional[TestrecordModelDebugInfoValue]]]
+
+class Testrecord(UncheckedBaseModel):
+    id: typing.Optional[int] = None
+    created_at: typing.Optional[dt.datetime] = None
+    run_id: typing.Optional[int] = None
+    testset_id: typing.Optional[int] = None
+    testcase_id: typing.Optional[int] = None
+    user_query: typing.Optional[str] = None
+    context: typing.Optional[str] = None
+    model_response: typing.Optional[str] = None
+    ideal: typing.Optional[str] = None
+    full_prompt: typing.Optional[str] = None
+    custom_inputs: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCustomInputsValue]]] = None
+    custom_labels: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCustomLabelsValue]]] = None
+    custom_outputs: typing.Optional[typing.Dict[str, typing.Optional[TestrecordCustomOutputsValue]]] = None
+    status: typing.Optional[str] = None
+    prompt: typing.Optional[str] = None
+    model_params: typing.Optional[typing.Dict[str, typing.Optional[TestrecordModelParamsValue]]] = None
+    model_debug_info: typing.Optional[typing.Dict[str, typing.Optional[TestrecordModelDebugInfoValue]]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-0.2.1/src/scorecard/types/testset.py` & `scorecard_ai-1.0.0b0/src/scorecard/types/grade.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .custom_schema import CustomSchema
-
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
-
-
-class Testset(pydantic.BaseModel):
-    id: typing.Optional[int]
-    created_at: typing.Optional[dt.datetime]
-    name: typing.Optional[str]
-    description: typing.Optional[str]
-    using_retrieval: typing.Optional[bool]
-    ingestion_method: typing.Optional[str]
-    num_testcases: typing.Optional[int]
-    published: typing.Optional[bool]
-    updated_at: typing.Optional[dt.datetime]
-    is_archived: typing.Optional[bool]
-    project_id: typing.Optional[int]
-    custom_schema: typing.Optional[CustomSchema]
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .score_status import ScoreStatus
+
+
+class Grade(UncheckedBaseModel):
+    id: typing.Optional[int] = None
+    run_id: typing.Optional[int] = None
+    testcase_id: typing.Optional[int] = None
+    testrecord_id: typing.Optional[int] = None
+    metric_id: typing.Optional[int] = None
+    user_id: typing.Optional[str] = None
+    binary_score: typing.Optional[bool] = None
+    int_score: typing.Optional[int] = None
+    reasoning: typing.Optional[str] = None
+    human_eval: typing.Optional[bool] = None
+    status: typing.Optional[ScoreStatus] = None
+    error_message: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-0.2.1/src/scorecard/types/unauthenticated_error.py` & `scorecard_ai-1.0.0b0/src/scorecard/types/unauthenticated_error.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class UnauthenticatedError(pydantic.BaseModel):
-    error: typing.Optional[str]
-    error_description: typing.Optional[str]
-    status_code: typing.Optional[int]
+class UnauthenticatedError(UncheckedBaseModel):
+    error: typing.Optional[str] = None
+    error_description: typing.Optional[str] = None
+    status_code: typing.Optional[int] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-0.2.1/src/scorecard/types/unauthorized_error_body.py` & `scorecard_ai-1.0.0b0/src/scorecard/types/http_validation_error.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .validation_error import ValidationError
 
-try:
-    import pydantic.v1 as pydantic  # type: ignore
-except ImportError:
-    import pydantic  # type: ignore
 
-
-class UnauthorizedErrorBody(pydantic.BaseModel):
-    error: typing.Optional[str]
-    error_description: typing.Optional[str]
-    status_code: typing.Optional[int]
+class HttpValidationError(UncheckedBaseModel):
+    detail: typing.Optional[typing.List[ValidationError]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
         smart_union = True
+        extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `scorecard_ai-0.2.1/PKG-INFO` & `scorecard_ai-1.0.0b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: scorecard-ai
-Version: 0.2.1
+Version: 1.0.0b0
 Summary: 
 License: Apache-2.0
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.21.2)
-Requires-Dist: pydantic (>=1.9.2,<2.5.0)
+Requires-Dist: pydantic (>=1.9.2)
+Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
+Requires-Dist: typing_extensions (>=4.0.0)
 Description-Content-Type: text/markdown
 
 # Scorecard AI Python Library
 
 [![pypi](https://img.shields.io/pypi/v/scorecard-ai.svg)](https://pypi.python.org/pypi/scorecard-ai)
 [![fern shield](https://img.shields.io/badge/%F0%9F%8C%BF-SDK%20generated%20by%20Fern-brightgreen)](https://github.com/fern-api/fern)
 
@@ -112,15 +113,15 @@
 scorecard_client = Scorecard(
   api_key="YOUR_API_KEY",
   timeout=15,
 )
 ```
 
 ## Handling Exceptions
-All exceptions thrown by the SDK will sublcass [scorecard.ApiError](./src/scorecard/core/api_error.py). 
+All exceptions thrown by the SDK will subclass [scorecard.ApiError](./src/scorecard/core/api_error.py). 
 
 ```python
 from scorecard.core import ApiError
 from scorecard import UnprocessableEntityError
 
 try:
   client.testset.get("testset-id")
```

