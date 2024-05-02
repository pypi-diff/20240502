# Comparing `tmp/langfuse-2.9.1a0.tar.gz` & `tmp/langfuse-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfuse-2.9.1a0.tar", max compression
+gzip compressed data, was "langfuse-2.9.2.tar", max compression
```

## Comparing `langfuse-2.9.1a0.tar` & `langfuse-2.9.2.tar`

### file list

```diff
@@ -1,133 +1,133 @@
--rw-r--r--   0        0        0     1074 2023-09-27 01:02:13.139768 langfuse-2.9.1a0/LICENSE
--rw-r--r--   0        0        0     2777 2024-01-05 14:15:29.325786 langfuse-2.9.1a0/README.md
--rw-r--r--   0        0        0       78 2023-12-22 08:31:50.691414 langfuse-2.9.1a0/langfuse/__init__.py
--rw-r--r--   0        0        0     3955 2024-02-01 14:56:53.080402 langfuse-2.9.1a0/langfuse/api/__init__.py
--rw-r--r--   0        0        0     4866 2024-02-01 13:48:02.971422 langfuse-2.9.1a0/langfuse/api/client.py
--rw-r--r--   0        0        0      519 2024-02-01 13:29:23.975403 langfuse-2.9.1a0/langfuse/api/core/__init__.py
--rw-r--r--   0        0        0      440 2024-02-01 13:48:02.972372 langfuse-2.9.1a0/langfuse/api/core/api_error.py
--rw-r--r--   0        0        0     3759 2024-02-01 13:48:02.972404 langfuse-2.9.1a0/langfuse/api/core/client_wrapper.py
--rw-r--r--   0        0        0     1069 2024-02-01 13:48:02.972372 langfuse-2.9.1a0/langfuse/api/core/datetime_utils.py
--rw-r--r--   0        0        0     3826 2024-02-01 13:48:02.972561 langfuse-2.9.1a0/langfuse/api/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-02-01 13:29:23.977336 langfuse-2.9.1a0/langfuse/api/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     4136 2024-02-01 14:56:53.080673 langfuse-2.9.1a0/langfuse/api/resources/__init__.py
--rw-r--r--   0        0        0      971 2024-02-01 14:56:53.080924 langfuse-2.9.1a0/langfuse/api/resources/commons/__init__.py
--rw-r--r--   0        0        0      422 2024-02-01 13:48:02.965474 langfuse-2.9.1a0/langfuse/api/resources/commons/errors/__init__.py
--rw-r--r--   0        0        0      252 2024-02-01 13:29:23.980058 langfuse-2.9.1a0/langfuse/api/resources/commons/errors/access_denied_error.py
--rw-r--r--   0        0        0      240 2024-02-01 13:29:23.980394 langfuse-2.9.1a0/langfuse/api/resources/commons/errors/error.py
--rw-r--r--   0        0        0      256 2024-02-01 13:29:23.980631 langfuse-2.9.1a0/langfuse/api/resources/commons/errors/method_not_allowed_error.py
--rw-r--r--   0        0        0      248 2024-02-01 13:29:23.981493 langfuse-2.9.1a0/langfuse/api/resources/commons/errors/not_found_error.py
--rw-r--r--   0        0        0      252 2024-02-01 13:29:23.981871 langfuse-2.9.1a0/langfuse/api/resources/commons/errors/unauthorized_error.py
--rw-r--r--   0        0        0     1073 2024-02-01 14:56:53.081567 langfuse-2.9.1a0/langfuse/api/resources/commons/types/__init__.py
--rw-r--r--   0        0        0     1303 2024-02-01 13:48:02.971053 langfuse-2.9.1a0/langfuse/api/resources/commons/types/dataset.py
--rw-r--r--   0        0        0     1522 2024-02-01 13:48:02.970510 langfuse-2.9.1a0/langfuse/api/resources/commons/types/dataset_item.py
--rw-r--r--   0        0        0     1357 2024-02-01 13:48:02.965232 langfuse-2.9.1a0/langfuse/api/resources/commons/types/dataset_run.py
--rw-r--r--   0        0        0     1331 2024-02-01 13:48:02.971747 langfuse-2.9.1a0/langfuse/api/resources/commons/types/dataset_run_item.py
--rw-r--r--   0        0        0      504 2024-02-01 13:48:02.969486 langfuse-2.9.1a0/langfuse/api/resources/commons/types/dataset_status.py
--rw-r--r--   0        0        0      225 2024-02-01 13:48:02.968142 langfuse-2.9.1a0/langfuse/api/resources/commons/types/map_value.py
--rw-r--r--   0        0        0      517 2024-02-01 13:48:02.971306 langfuse-2.9.1a0/langfuse/api/resources/commons/types/model_usage_unit.py
--rw-r--r--   0        0        0     2290 2024-02-01 13:48:02.969886 langfuse-2.9.1a0/langfuse/api/resources/commons/types/observation.py
--rw-r--r--   0        0        0      785 2024-02-01 13:29:23.985167 langfuse-2.9.1a0/langfuse/api/resources/commons/types/observation_level.py
--rw-r--r--   0        0        0     1805 2024-02-01 14:56:53.081791 langfuse-2.9.1a0/langfuse/api/resources/commons/types/observations_view.py
--rw-r--r--   0        0        0     1262 2024-02-01 13:48:02.968582 langfuse-2.9.1a0/langfuse/api/resources/commons/types/score.py
--rw-r--r--   0        0        0     1124 2024-02-01 13:48:02.965911 langfuse-2.9.1a0/langfuse/api/resources/commons/types/session.py
--rw-r--r--   0        0        0      963 2024-02-01 13:48:02.966804 langfuse-2.9.1a0/langfuse/api/resources/commons/types/session_with_traces.py
--rw-r--r--   0        0        0     1720 2024-02-01 13:48:02.968253 langfuse-2.9.1a0/langfuse/api/resources/commons/types/trace.py
--rw-r--r--   0        0        0     1197 2024-02-01 13:48:02.970476 langfuse-2.9.1a0/langfuse/api/resources/commons/types/trace_with_details.py
--rw-r--r--   0        0        0     1056 2024-02-01 14:56:53.082003 langfuse-2.9.1a0/langfuse/api/resources/commons/types/trace_with_full_details.py
--rw-r--r--   0        0        0     1485 2024-02-01 13:48:02.969253 langfuse-2.9.1a0/langfuse/api/resources/commons/types/usage.py
--rw-r--r--   0        0        0      149 2024-02-01 13:29:23.987969 langfuse-2.9.1a0/langfuse/api/resources/dataset_items/__init__.py
--rw-r--r--   0        0        0     7887 2024-02-01 13:48:02.965083 langfuse-2.9.1a0/langfuse/api/resources/dataset_items/client.py
--rw-r--r--   0        0        0      171 2024-02-01 13:29:23.988977 langfuse-2.9.1a0/langfuse/api/resources/dataset_items/types/__init__.py
--rw-r--r--   0        0        0     1245 2024-02-01 13:48:02.965800 langfuse-2.9.1a0/langfuse/api/resources/dataset_items/types/create_dataset_item_request.py
--rw-r--r--   0        0        0      155 2024-02-01 13:29:23.989673 langfuse-2.9.1a0/langfuse/api/resources/dataset_run_items/__init__.py
--rw-r--r--   0        0        0     4711 2024-02-01 13:48:02.967093 langfuse-2.9.1a0/langfuse/api/resources/dataset_run_items/client.py
--rw-r--r--   0        0        0      181 2024-02-01 13:29:23.990550 langfuse-2.9.1a0/langfuse/api/resources/dataset_run_items/types/__init__.py
--rw-r--r--   0        0        0     1193 2024-02-01 13:48:02.969024 langfuse-2.9.1a0/langfuse/api/resources/dataset_run_items/types/create_dataset_run_item_request.py
--rw-r--r--   0        0        0      141 2024-02-01 13:29:23.991182 langfuse-2.9.1a0/langfuse/api/resources/datasets/__init__.py
--rw-r--r--   0        0        0    11290 2024-02-01 13:48:02.967240 langfuse-2.9.1a0/langfuse/api/resources/datasets/client.py
--rw-r--r--   0        0        0      158 2024-02-01 13:29:23.992046 langfuse-2.9.1a0/langfuse/api/resources/datasets/types/__init__.py
--rw-r--r--   0        0        0      973 2024-02-01 13:48:02.967975 langfuse-2.9.1a0/langfuse/api/resources/datasets/types/create_dataset_request.py
--rw-r--r--   0        0        0      200 2024-02-01 13:29:23.992806 langfuse-2.9.1a0/langfuse/api/resources/health/__init__.py
--rw-r--r--   0        0        0     4333 2024-02-01 13:48:02.965577 langfuse-2.9.1a0/langfuse/api/resources/health/client.py
--rw-r--r--   0        0        0      167 2024-02-01 13:29:23.993608 langfuse-2.9.1a0/langfuse/api/resources/health/errors/__init__.py
--rw-r--r--   0        0        0      222 2024-02-01 13:29:23.993861 langfuse-2.9.1a0/langfuse/api/resources/health/errors/service_unavailable_error.py
--rw-r--r--   0        0        0      139 2024-02-01 13:29:23.994343 langfuse-2.9.1a0/langfuse/api/resources/health/types/__init__.py
--rw-r--r--   0        0        0     1170 2024-02-01 13:48:02.966343 langfuse-2.9.1a0/langfuse/api/resources/health/types/health_response.py
--rw-r--r--   0        0        0     2073 2024-02-01 13:29:23.994967 langfuse-2.9.1a0/langfuse/api/resources/ingestion/__init__.py
--rw-r--r--   0        0        0     4654 2024-02-01 13:48:02.965080 langfuse-2.9.1a0/langfuse/api/resources/ingestion/client.py
--rw-r--r--   0        0        0     2803 2024-02-01 13:29:23.996014 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/__init__.py
--rw-r--r--   0        0        0     1004 2024-02-01 13:48:02.968908 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/base_event.py
--rw-r--r--   0        0        0      991 2024-02-01 13:48:02.968669 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/create_event_body.py
--rw-r--r--   0        0        0      986 2024-02-01 13:48:02.967970 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/create_event_event.py
--rw-r--r--   0        0        0     1691 2024-02-01 13:48:02.969685 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/create_generation_body.py
--rw-r--r--   0        0        0     1006 2024-02-01 13:48:02.970619 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/create_generation_event.py
--rw-r--r--   0        0        0      991 2024-02-01 13:48:02.968463 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/create_observation_event.py
--rw-r--r--   0        0        0     1148 2024-02-01 13:48:02.969063 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/create_span_body.py
--rw-r--r--   0        0        0      982 2024-02-01 13:48:02.965415 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/create_span_event.py
--rw-r--r--   0        0        0     1068 2024-02-01 13:48:02.966333 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/ingestion_error.py
--rw-r--r--   0        0        0     3239 2024-02-01 13:29:23.998724 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/ingestion_event.py
--rw-r--r--   0        0        0     1133 2024-02-01 13:48:02.970247 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/ingestion_response.py
--rw-r--r--   0        0        0      983 2024-02-01 13:48:02.969019 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/ingestion_success.py
--rw-r--r--   0        0        0      211 2024-02-01 13:29:23.999522 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/ingestion_usage.py
--rw-r--r--   0        0        0     2408 2024-02-01 13:48:02.966173 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/observation_body.py
--rw-r--r--   0        0        0      645 2024-02-01 13:29:24.000199 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/observation_type.py
--rw-r--r--   0        0        0     1323 2024-02-01 13:48:02.966787 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/open_ai_usage.py
--rw-r--r--   0        0        0     1768 2024-02-01 13:48:02.971165 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/optional_observation_body.py
--rw-r--r--   0        0        0     1263 2024-02-01 13:48:02.967181 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/score_body.py
--rw-r--r--   0        0        0      961 2024-02-01 13:48:02.967103 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/score_event.py
--rw-r--r--   0        0        0      969 2024-02-01 13:48:02.968764 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/sdk_log_body.py
--rw-r--r--   0        0        0      966 2024-02-01 13:48:02.970818 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/sdk_log_event.py
--rw-r--r--   0        0        0     1644 2024-02-01 13:48:02.968112 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/trace_body.py
--rw-r--r--   0        0        0      961 2024-02-01 13:48:02.967895 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/trace_event.py
--rw-r--r--   0        0        0      967 2024-02-01 13:48:02.969971 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/update_event_body.py
--rw-r--r--   0        0        0     1691 2024-02-01 13:48:02.966844 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/update_generation_body.py
--rw-r--r--   0        0        0     1006 2024-02-01 13:48:02.969958 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/update_generation_event.py
--rw-r--r--   0        0        0      991 2024-02-01 13:48:02.965213 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/update_observation_event.py
--rw-r--r--   0        0        0     1148 2024-02-01 13:48:02.969098 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/update_span_body.py
--rw-r--r--   0        0        0      982 2024-02-01 13:48:02.969380 langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/update_span_event.py
--rw-r--r--   0        0        0      165 2024-02-01 14:56:53.082269 langfuse-2.9.1a0/langfuse/api/resources/observations/__init__.py
--rw-r--r--   0        0        0     9904 2024-02-01 14:56:53.082468 langfuse-2.9.1a0/langfuse/api/resources/observations/client.py
--rw-r--r--   0        0        0      203 2024-02-01 14:56:53.082757 langfuse-2.9.1a0/langfuse/api/resources/observations/types/__init__.py
--rw-r--r--   0        0        0     1137 2024-02-01 13:48:02.966090 langfuse-2.9.1a0/langfuse/api/resources/observations/types/observations.py
--rw-r--r--   0        0        0     1158 2024-02-01 14:56:53.083123 langfuse-2.9.1a0/langfuse/api/resources/observations/types/observations_views.py
--rw-r--r--   0        0        0      137 2024-02-01 13:29:24.008884 langfuse-2.9.1a0/langfuse/api/resources/projects/__init__.py
--rw-r--r--   0        0        0     3928 2024-02-01 13:48:02.968233 langfuse-2.9.1a0/langfuse/api/resources/projects/client.py
--rw-r--r--   0        0        0      160 2024-02-01 13:29:24.010008 langfuse-2.9.1a0/langfuse/api/resources/projects/types/__init__.py
--rw-r--r--   0        0        0      972 2024-02-01 13:48:02.965701 langfuse-2.9.1a0/langfuse/api/resources/projects/types/project.py
--rw-r--r--   0        0        0     1007 2024-02-01 13:48:02.966230 langfuse-2.9.1a0/langfuse/api/resources/projects/types/projects.py
--rw-r--r--   0        0        0      157 2024-02-01 13:29:24.010817 langfuse-2.9.1a0/langfuse/api/resources/prompts/__init__.py
--rw-r--r--   0        0        0     8082 2024-02-01 13:48:02.967260 langfuse-2.9.1a0/langfuse/api/resources/prompts/client.py
--rw-r--r--   0        0        0      192 2024-02-01 13:29:24.011626 langfuse-2.9.1a0/langfuse/api/resources/prompts/types/__init__.py
--rw-r--r--   0        0        0     1089 2024-02-01 13:48:02.968794 langfuse-2.9.1a0/langfuse/api/resources/prompts/types/create_prompt_request.py
--rw-r--r--   0        0        0      992 2024-02-01 13:48:02.968324 langfuse-2.9.1a0/langfuse/api/resources/prompts/types/prompt.py
--rw-r--r--   0        0        0      155 2024-02-01 13:29:24.012391 langfuse-2.9.1a0/langfuse/api/resources/score/__init__.py
--rw-r--r--   0        0        0     8744 2024-02-01 13:48:02.970689 langfuse-2.9.1a0/langfuse/api/resources/score/client.py
--rw-r--r--   0        0        0      189 2024-02-01 13:29:24.013091 langfuse-2.9.1a0/langfuse/api/resources/score/types/__init__.py
--rw-r--r--   0        0        0     1272 2024-02-01 13:48:02.971529 langfuse-2.9.1a0/langfuse/api/resources/score/types/create_score_request.py
--rw-r--r--   0        0        0     1113 2024-02-01 13:48:02.970982 langfuse-2.9.1a0/langfuse/api/resources/score/types/scores.py
--rw-r--r--   0        0        0       65 2024-02-01 14:56:53.083284 langfuse-2.9.1a0/langfuse/api/resources/sessions/__init__.py
--rw-r--r--   0        0        0     4339 2024-02-01 13:48:02.969522 langfuse-2.9.1a0/langfuse/api/resources/sessions/client.py
--rw-r--r--   0        0        0      127 2024-02-01 13:29:24.014516 langfuse-2.9.1a0/langfuse/api/resources/trace/__init__.py
--rw-r--r--   0        0        0     9705 2024-02-01 13:48:02.967598 langfuse-2.9.1a0/langfuse/api/resources/trace/client.py
--rw-r--r--   0        0        0      145 2024-02-01 13:29:24.015450 langfuse-2.9.1a0/langfuse/api/resources/trace/types/__init__.py
--rw-r--r--   0        0        0      955 2024-02-01 13:48:02.966876 langfuse-2.9.1a0/langfuse/api/resources/trace/types/sort.py
--rw-r--r--   0        0        0     1148 2024-02-01 13:48:02.966326 langfuse-2.9.1a0/langfuse/api/resources/trace/types/traces.py
--rw-r--r--   0        0        0      155 2024-02-01 13:29:24.016863 langfuse-2.9.1a0/langfuse/api/resources/utils/__init__.py
--rw-r--r--   0        0        0      169 2024-02-01 13:29:24.017190 langfuse-2.9.1a0/langfuse/api/resources/utils/resources/__init__.py
--rw-r--r--   0        0        0      125 2024-02-01 13:29:24.017570 langfuse-2.9.1a0/langfuse/api/resources/utils/resources/pagination/__init__.py
--rw-r--r--   0        0        0      133 2024-02-01 13:29:24.018041 langfuse-2.9.1a0/langfuse/api/resources/utils/resources/pagination/types/__init__.py
--rw-r--r--   0        0        0     1433 2024-02-01 13:48:02.965429 langfuse-2.9.1a0/langfuse/api/resources/utils/resources/pagination/types/meta_response.py
--rw-r--r--   0        0        0    28504 2024-02-05 10:04:37.211646 langfuse-2.9.1a0/langfuse/callback.py
--rw-r--r--   0        0        0    48855 2024-02-05 17:42:04.661738 langfuse-2.9.1a0/langfuse/client.py
--rw-r--r--   0        0        0      643 2023-12-17 15:50:22.264382 langfuse-2.9.1a0/langfuse/environment.py
--rw-r--r--   0        0        0      418 2023-12-17 15:50:26.950945 langfuse-2.9.1a0/langfuse/logging.py
--rw-r--r--   0        0        0     2102 2024-02-05 14:24:56.650580 langfuse-2.9.1a0/langfuse/model.py
--rw-r--r--   0        0        0    15417 2024-02-06 20:21:01.856869 langfuse-2.9.1a0/langfuse/openai.py
--rw-r--r--   0        0        0     1097 2024-02-05 14:24:56.650868 langfuse-2.9.1a0/langfuse/prompt_cache.py
--rw-r--r--   0        0        0     3902 2024-02-05 16:30:19.659307 langfuse-2.9.1a0/langfuse/request.py
--rw-r--r--   0        0        0     1069 2024-01-05 13:33:05.301169 langfuse-2.9.1a0/langfuse/serializer.py
--rw-r--r--   0        0        0     8497 2024-01-29 09:58:04.034481 langfuse-2.9.1a0/langfuse/task_manager.py
--rw-r--r--   0        0        0     2873 2024-02-01 15:05:11.921238 langfuse-2.9.1a0/langfuse/utils.py
--rw-r--r--   0        0        0       24 2024-02-06 20:21:42.760923 langfuse-2.9.1a0/langfuse/version.py
--rw-r--r--   0        0        0     1202 2024-02-06 20:21:42.757196 langfuse-2.9.1a0/pyproject.toml
--rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 langfuse-2.9.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-09-27 01:02:13.139768 langfuse-2.9.2/LICENSE
+-rw-r--r--   0        0        0     2777 2024-01-05 14:15:29.325786 langfuse-2.9.2/README.md
+-rw-r--r--   0        0        0       78 2023-12-22 08:31:50.691414 langfuse-2.9.2/langfuse/__init__.py
+-rw-r--r--   0        0        0     3955 2024-02-01 14:56:53.080402 langfuse-2.9.2/langfuse/api/__init__.py
+-rw-r--r--   0        0        0     4866 2024-02-01 13:48:02.971422 langfuse-2.9.2/langfuse/api/client.py
+-rw-r--r--   0        0        0      519 2024-02-01 13:29:23.975403 langfuse-2.9.2/langfuse/api/core/__init__.py
+-rw-r--r--   0        0        0      440 2024-02-01 13:48:02.972372 langfuse-2.9.2/langfuse/api/core/api_error.py
+-rw-r--r--   0        0        0     3759 2024-02-01 13:48:02.972404 langfuse-2.9.2/langfuse/api/core/client_wrapper.py
+-rw-r--r--   0        0        0     1069 2024-02-01 13:48:02.972372 langfuse-2.9.2/langfuse/api/core/datetime_utils.py
+-rw-r--r--   0        0        0     3826 2024-02-01 13:48:02.972561 langfuse-2.9.2/langfuse/api/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-02-01 13:29:23.977336 langfuse-2.9.2/langfuse/api/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     4136 2024-02-01 14:56:53.080673 langfuse-2.9.2/langfuse/api/resources/__init__.py
+-rw-r--r--   0        0        0      971 2024-02-01 14:56:53.080924 langfuse-2.9.2/langfuse/api/resources/commons/__init__.py
+-rw-r--r--   0        0        0      422 2024-02-01 13:48:02.965474 langfuse-2.9.2/langfuse/api/resources/commons/errors/__init__.py
+-rw-r--r--   0        0        0      252 2024-02-01 13:29:23.980058 langfuse-2.9.2/langfuse/api/resources/commons/errors/access_denied_error.py
+-rw-r--r--   0        0        0      240 2024-02-01 13:29:23.980394 langfuse-2.9.2/langfuse/api/resources/commons/errors/error.py
+-rw-r--r--   0        0        0      256 2024-02-01 13:29:23.980631 langfuse-2.9.2/langfuse/api/resources/commons/errors/method_not_allowed_error.py
+-rw-r--r--   0        0        0      248 2024-02-01 13:29:23.981493 langfuse-2.9.2/langfuse/api/resources/commons/errors/not_found_error.py
+-rw-r--r--   0        0        0      252 2024-02-01 13:29:23.981871 langfuse-2.9.2/langfuse/api/resources/commons/errors/unauthorized_error.py
+-rw-r--r--   0        0        0     1073 2024-02-01 14:56:53.081567 langfuse-2.9.2/langfuse/api/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0     1303 2024-02-01 13:48:02.971053 langfuse-2.9.2/langfuse/api/resources/commons/types/dataset.py
+-rw-r--r--   0        0        0     1522 2024-02-01 13:48:02.970510 langfuse-2.9.2/langfuse/api/resources/commons/types/dataset_item.py
+-rw-r--r--   0        0        0     1357 2024-02-01 13:48:02.965232 langfuse-2.9.2/langfuse/api/resources/commons/types/dataset_run.py
+-rw-r--r--   0        0        0     1331 2024-02-01 13:48:02.971747 langfuse-2.9.2/langfuse/api/resources/commons/types/dataset_run_item.py
+-rw-r--r--   0        0        0      504 2024-02-01 13:48:02.969486 langfuse-2.9.2/langfuse/api/resources/commons/types/dataset_status.py
+-rw-r--r--   0        0        0      225 2024-02-01 13:48:02.968142 langfuse-2.9.2/langfuse/api/resources/commons/types/map_value.py
+-rw-r--r--   0        0        0      969 2024-02-07 10:10:34.053244 langfuse-2.9.2/langfuse/api/resources/commons/types/model_usage_unit.py
+-rw-r--r--   0        0        0     2290 2024-02-01 13:48:02.969886 langfuse-2.9.2/langfuse/api/resources/commons/types/observation.py
+-rw-r--r--   0        0        0      785 2024-02-01 13:29:23.985167 langfuse-2.9.2/langfuse/api/resources/commons/types/observation_level.py
+-rw-r--r--   0        0        0     1805 2024-02-01 14:56:53.081791 langfuse-2.9.2/langfuse/api/resources/commons/types/observations_view.py
+-rw-r--r--   0        0        0     1262 2024-02-01 13:48:02.968582 langfuse-2.9.2/langfuse/api/resources/commons/types/score.py
+-rw-r--r--   0        0        0     1124 2024-02-01 13:48:02.965911 langfuse-2.9.2/langfuse/api/resources/commons/types/session.py
+-rw-r--r--   0        0        0      963 2024-02-01 13:48:02.966804 langfuse-2.9.2/langfuse/api/resources/commons/types/session_with_traces.py
+-rw-r--r--   0        0        0     1720 2024-02-01 13:48:02.968253 langfuse-2.9.2/langfuse/api/resources/commons/types/trace.py
+-rw-r--r--   0        0        0     1197 2024-02-01 13:48:02.970476 langfuse-2.9.2/langfuse/api/resources/commons/types/trace_with_details.py
+-rw-r--r--   0        0        0     1056 2024-02-01 14:56:53.082003 langfuse-2.9.2/langfuse/api/resources/commons/types/trace_with_full_details.py
+-rw-r--r--   0        0        0     1485 2024-02-01 13:48:02.969253 langfuse-2.9.2/langfuse/api/resources/commons/types/usage.py
+-rw-r--r--   0        0        0      149 2024-02-01 13:29:23.987969 langfuse-2.9.2/langfuse/api/resources/dataset_items/__init__.py
+-rw-r--r--   0        0        0     7887 2024-02-01 13:48:02.965083 langfuse-2.9.2/langfuse/api/resources/dataset_items/client.py
+-rw-r--r--   0        0        0      171 2024-02-01 13:29:23.988977 langfuse-2.9.2/langfuse/api/resources/dataset_items/types/__init__.py
+-rw-r--r--   0        0        0     1245 2024-02-01 13:48:02.965800 langfuse-2.9.2/langfuse/api/resources/dataset_items/types/create_dataset_item_request.py
+-rw-r--r--   0        0        0      155 2024-02-01 13:29:23.989673 langfuse-2.9.2/langfuse/api/resources/dataset_run_items/__init__.py
+-rw-r--r--   0        0        0     4711 2024-02-01 13:48:02.967093 langfuse-2.9.2/langfuse/api/resources/dataset_run_items/client.py
+-rw-r--r--   0        0        0      181 2024-02-01 13:29:23.990550 langfuse-2.9.2/langfuse/api/resources/dataset_run_items/types/__init__.py
+-rw-r--r--   0        0        0     1193 2024-02-01 13:48:02.969024 langfuse-2.9.2/langfuse/api/resources/dataset_run_items/types/create_dataset_run_item_request.py
+-rw-r--r--   0        0        0      141 2024-02-01 13:29:23.991182 langfuse-2.9.2/langfuse/api/resources/datasets/__init__.py
+-rw-r--r--   0        0        0    11290 2024-02-01 13:48:02.967240 langfuse-2.9.2/langfuse/api/resources/datasets/client.py
+-rw-r--r--   0        0        0      158 2024-02-01 13:29:23.992046 langfuse-2.9.2/langfuse/api/resources/datasets/types/__init__.py
+-rw-r--r--   0        0        0      973 2024-02-01 13:48:02.967975 langfuse-2.9.2/langfuse/api/resources/datasets/types/create_dataset_request.py
+-rw-r--r--   0        0        0      200 2024-02-01 13:29:23.992806 langfuse-2.9.2/langfuse/api/resources/health/__init__.py
+-rw-r--r--   0        0        0     4333 2024-02-01 13:48:02.965577 langfuse-2.9.2/langfuse/api/resources/health/client.py
+-rw-r--r--   0        0        0      167 2024-02-01 13:29:23.993608 langfuse-2.9.2/langfuse/api/resources/health/errors/__init__.py
+-rw-r--r--   0        0        0      222 2024-02-01 13:29:23.993861 langfuse-2.9.2/langfuse/api/resources/health/errors/service_unavailable_error.py
+-rw-r--r--   0        0        0      139 2024-02-01 13:29:23.994343 langfuse-2.9.2/langfuse/api/resources/health/types/__init__.py
+-rw-r--r--   0        0        0     1170 2024-02-01 13:48:02.966343 langfuse-2.9.2/langfuse/api/resources/health/types/health_response.py
+-rw-r--r--   0        0        0     2073 2024-02-01 13:29:23.994967 langfuse-2.9.2/langfuse/api/resources/ingestion/__init__.py
+-rw-r--r--   0        0        0     4654 2024-02-01 13:48:02.965080 langfuse-2.9.2/langfuse/api/resources/ingestion/client.py
+-rw-r--r--   0        0        0     2803 2024-02-01 13:29:23.996014 langfuse-2.9.2/langfuse/api/resources/ingestion/types/__init__.py
+-rw-r--r--   0        0        0     1004 2024-02-01 13:48:02.968908 langfuse-2.9.2/langfuse/api/resources/ingestion/types/base_event.py
+-rw-r--r--   0        0        0      991 2024-02-01 13:48:02.968669 langfuse-2.9.2/langfuse/api/resources/ingestion/types/create_event_body.py
+-rw-r--r--   0        0        0      986 2024-02-01 13:48:02.967970 langfuse-2.9.2/langfuse/api/resources/ingestion/types/create_event_event.py
+-rw-r--r--   0        0        0     1691 2024-02-01 13:48:02.969685 langfuse-2.9.2/langfuse/api/resources/ingestion/types/create_generation_body.py
+-rw-r--r--   0        0        0     1006 2024-02-01 13:48:02.970619 langfuse-2.9.2/langfuse/api/resources/ingestion/types/create_generation_event.py
+-rw-r--r--   0        0        0      991 2024-02-01 13:48:02.968463 langfuse-2.9.2/langfuse/api/resources/ingestion/types/create_observation_event.py
+-rw-r--r--   0        0        0     1148 2024-02-01 13:48:02.969063 langfuse-2.9.2/langfuse/api/resources/ingestion/types/create_span_body.py
+-rw-r--r--   0        0        0      982 2024-02-01 13:48:02.965415 langfuse-2.9.2/langfuse/api/resources/ingestion/types/create_span_event.py
+-rw-r--r--   0        0        0     1068 2024-02-01 13:48:02.966333 langfuse-2.9.2/langfuse/api/resources/ingestion/types/ingestion_error.py
+-rw-r--r--   0        0        0     3239 2024-02-01 13:29:23.998724 langfuse-2.9.2/langfuse/api/resources/ingestion/types/ingestion_event.py
+-rw-r--r--   0        0        0     1133 2024-02-01 13:48:02.970247 langfuse-2.9.2/langfuse/api/resources/ingestion/types/ingestion_response.py
+-rw-r--r--   0        0        0      983 2024-02-01 13:48:02.969019 langfuse-2.9.2/langfuse/api/resources/ingestion/types/ingestion_success.py
+-rw-r--r--   0        0        0      211 2024-02-01 13:29:23.999522 langfuse-2.9.2/langfuse/api/resources/ingestion/types/ingestion_usage.py
+-rw-r--r--   0        0        0     2408 2024-02-01 13:48:02.966173 langfuse-2.9.2/langfuse/api/resources/ingestion/types/observation_body.py
+-rw-r--r--   0        0        0      645 2024-02-01 13:29:24.000199 langfuse-2.9.2/langfuse/api/resources/ingestion/types/observation_type.py
+-rw-r--r--   0        0        0     1323 2024-02-01 13:48:02.966787 langfuse-2.9.2/langfuse/api/resources/ingestion/types/open_ai_usage.py
+-rw-r--r--   0        0        0     1768 2024-02-01 13:48:02.971165 langfuse-2.9.2/langfuse/api/resources/ingestion/types/optional_observation_body.py
+-rw-r--r--   0        0        0     1263 2024-02-01 13:48:02.967181 langfuse-2.9.2/langfuse/api/resources/ingestion/types/score_body.py
+-rw-r--r--   0        0        0      961 2024-02-01 13:48:02.967103 langfuse-2.9.2/langfuse/api/resources/ingestion/types/score_event.py
+-rw-r--r--   0        0        0      969 2024-02-01 13:48:02.968764 langfuse-2.9.2/langfuse/api/resources/ingestion/types/sdk_log_body.py
+-rw-r--r--   0        0        0      966 2024-02-01 13:48:02.970818 langfuse-2.9.2/langfuse/api/resources/ingestion/types/sdk_log_event.py
+-rw-r--r--   0        0        0     1644 2024-02-01 13:48:02.968112 langfuse-2.9.2/langfuse/api/resources/ingestion/types/trace_body.py
+-rw-r--r--   0        0        0      961 2024-02-01 13:48:02.967895 langfuse-2.9.2/langfuse/api/resources/ingestion/types/trace_event.py
+-rw-r--r--   0        0        0      967 2024-02-01 13:48:02.969971 langfuse-2.9.2/langfuse/api/resources/ingestion/types/update_event_body.py
+-rw-r--r--   0        0        0     1691 2024-02-01 13:48:02.966844 langfuse-2.9.2/langfuse/api/resources/ingestion/types/update_generation_body.py
+-rw-r--r--   0        0        0     1006 2024-02-01 13:48:02.969958 langfuse-2.9.2/langfuse/api/resources/ingestion/types/update_generation_event.py
+-rw-r--r--   0        0        0      991 2024-02-01 13:48:02.965213 langfuse-2.9.2/langfuse/api/resources/ingestion/types/update_observation_event.py
+-rw-r--r--   0        0        0     1148 2024-02-01 13:48:02.969098 langfuse-2.9.2/langfuse/api/resources/ingestion/types/update_span_body.py
+-rw-r--r--   0        0        0      982 2024-02-01 13:48:02.969380 langfuse-2.9.2/langfuse/api/resources/ingestion/types/update_span_event.py
+-rw-r--r--   0        0        0      165 2024-02-01 14:56:53.082269 langfuse-2.9.2/langfuse/api/resources/observations/__init__.py
+-rw-r--r--   0        0        0     9904 2024-02-01 14:56:53.082468 langfuse-2.9.2/langfuse/api/resources/observations/client.py
+-rw-r--r--   0        0        0      203 2024-02-01 14:56:53.082757 langfuse-2.9.2/langfuse/api/resources/observations/types/__init__.py
+-rw-r--r--   0        0        0     1137 2024-02-01 13:48:02.966090 langfuse-2.9.2/langfuse/api/resources/observations/types/observations.py
+-rw-r--r--   0        0        0     1158 2024-02-01 14:56:53.083123 langfuse-2.9.2/langfuse/api/resources/observations/types/observations_views.py
+-rw-r--r--   0        0        0      137 2024-02-01 13:29:24.008884 langfuse-2.9.2/langfuse/api/resources/projects/__init__.py
+-rw-r--r--   0        0        0     3928 2024-02-01 13:48:02.968233 langfuse-2.9.2/langfuse/api/resources/projects/client.py
+-rw-r--r--   0        0        0      160 2024-02-01 13:29:24.010008 langfuse-2.9.2/langfuse/api/resources/projects/types/__init__.py
+-rw-r--r--   0        0        0      972 2024-02-01 13:48:02.965701 langfuse-2.9.2/langfuse/api/resources/projects/types/project.py
+-rw-r--r--   0        0        0     1007 2024-02-01 13:48:02.966230 langfuse-2.9.2/langfuse/api/resources/projects/types/projects.py
+-rw-r--r--   0        0        0      157 2024-02-01 13:29:24.010817 langfuse-2.9.2/langfuse/api/resources/prompts/__init__.py
+-rw-r--r--   0        0        0     8082 2024-02-01 13:48:02.967260 langfuse-2.9.2/langfuse/api/resources/prompts/client.py
+-rw-r--r--   0        0        0      192 2024-02-01 13:29:24.011626 langfuse-2.9.2/langfuse/api/resources/prompts/types/__init__.py
+-rw-r--r--   0        0        0     1089 2024-02-01 13:48:02.968794 langfuse-2.9.2/langfuse/api/resources/prompts/types/create_prompt_request.py
+-rw-r--r--   0        0        0      992 2024-02-01 13:48:02.968324 langfuse-2.9.2/langfuse/api/resources/prompts/types/prompt.py
+-rw-r--r--   0        0        0      155 2024-02-01 13:29:24.012391 langfuse-2.9.2/langfuse/api/resources/score/__init__.py
+-rw-r--r--   0        0        0     8744 2024-02-01 13:48:02.970689 langfuse-2.9.2/langfuse/api/resources/score/client.py
+-rw-r--r--   0        0        0      189 2024-02-01 13:29:24.013091 langfuse-2.9.2/langfuse/api/resources/score/types/__init__.py
+-rw-r--r--   0        0        0     1272 2024-02-01 13:48:02.971529 langfuse-2.9.2/langfuse/api/resources/score/types/create_score_request.py
+-rw-r--r--   0        0        0     1113 2024-02-01 13:48:02.970982 langfuse-2.9.2/langfuse/api/resources/score/types/scores.py
+-rw-r--r--   0        0        0       65 2024-02-01 14:56:53.083284 langfuse-2.9.2/langfuse/api/resources/sessions/__init__.py
+-rw-r--r--   0        0        0     4339 2024-02-01 13:48:02.969522 langfuse-2.9.2/langfuse/api/resources/sessions/client.py
+-rw-r--r--   0        0        0      127 2024-02-01 13:29:24.014516 langfuse-2.9.2/langfuse/api/resources/trace/__init__.py
+-rw-r--r--   0        0        0     9705 2024-02-01 13:48:02.967598 langfuse-2.9.2/langfuse/api/resources/trace/client.py
+-rw-r--r--   0        0        0      145 2024-02-01 13:29:24.015450 langfuse-2.9.2/langfuse/api/resources/trace/types/__init__.py
+-rw-r--r--   0        0        0      955 2024-02-01 13:48:02.966876 langfuse-2.9.2/langfuse/api/resources/trace/types/sort.py
+-rw-r--r--   0        0        0     1148 2024-02-01 13:48:02.966326 langfuse-2.9.2/langfuse/api/resources/trace/types/traces.py
+-rw-r--r--   0        0        0      155 2024-02-01 13:29:24.016863 langfuse-2.9.2/langfuse/api/resources/utils/__init__.py
+-rw-r--r--   0        0        0      169 2024-02-01 13:29:24.017190 langfuse-2.9.2/langfuse/api/resources/utils/resources/__init__.py
+-rw-r--r--   0        0        0      125 2024-02-01 13:29:24.017570 langfuse-2.9.2/langfuse/api/resources/utils/resources/pagination/__init__.py
+-rw-r--r--   0        0        0      133 2024-02-01 13:29:24.018041 langfuse-2.9.2/langfuse/api/resources/utils/resources/pagination/types/__init__.py
+-rw-r--r--   0        0        0     1433 2024-02-01 13:48:02.965429 langfuse-2.9.2/langfuse/api/resources/utils/resources/pagination/types/meta_response.py
+-rw-r--r--   0        0        0    28504 2024-02-05 10:04:37.211646 langfuse-2.9.2/langfuse/callback.py
+-rw-r--r--   0        0        0    48855 2024-02-05 17:42:04.661738 langfuse-2.9.2/langfuse/client.py
+-rw-r--r--   0        0        0      643 2023-12-17 15:50:22.264382 langfuse-2.9.2/langfuse/environment.py
+-rw-r--r--   0        0        0      418 2023-12-17 15:50:26.950945 langfuse-2.9.2/langfuse/logging.py
+-rw-r--r--   0        0        0     2102 2024-02-05 14:24:56.650580 langfuse-2.9.2/langfuse/model.py
+-rw-r--r--   0        0        0    15417 2024-02-06 21:08:32.290030 langfuse-2.9.2/langfuse/openai.py
+-rw-r--r--   0        0        0     1097 2024-02-05 14:24:56.650868 langfuse-2.9.2/langfuse/prompt_cache.py
+-rw-r--r--   0        0        0     3902 2024-02-05 16:30:19.659307 langfuse-2.9.2/langfuse/request.py
+-rw-r--r--   0        0        0     1069 2024-01-05 13:33:05.301169 langfuse-2.9.2/langfuse/serializer.py
+-rw-r--r--   0        0        0     8497 2024-01-29 09:58:04.034481 langfuse-2.9.2/langfuse/task_manager.py
+-rw-r--r--   0        0        0     2873 2024-02-01 15:05:11.921238 langfuse-2.9.2/langfuse/utils.py
+-rw-r--r--   0        0        0       22 2024-02-07 10:10:59.798487 langfuse-2.9.2/langfuse/version.py
+-rw-r--r--   0        0        0     1200 2024-02-07 10:10:59.795599 langfuse-2.9.2/pyproject.toml
+-rw-r--r--   0        0        0     3631 1970-01-01 00:00:00.000000 langfuse-2.9.2/PKG-INFO
```

### Comparing `langfuse-2.9.1a0/LICENSE` & `langfuse-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/README.md` & `langfuse-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/__init__.py` & `langfuse-2.9.2/langfuse/api/__init__.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/client.py` & `langfuse-2.9.2/langfuse/api/client.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/core/__init__.py` & `langfuse-2.9.2/langfuse/api/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/core/client_wrapper.py` & `langfuse-2.9.2/langfuse/api/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/core/datetime_utils.py` & `langfuse-2.9.2/langfuse/api/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/core/jsonable_encoder.py` & `langfuse-2.9.2/langfuse/api/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/__init__.py` & `langfuse-2.9.2/langfuse/api/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/commons/__init__.py` & `langfuse-2.9.2/langfuse/api/resources/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/commons/types/__init__.py` & `langfuse-2.9.2/langfuse/api/resources/commons/types/__init__.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/commons/types/dataset.py` & `langfuse-2.9.2/langfuse/api/resources/commons/types/dataset.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/commons/types/dataset_item.py` & `langfuse-2.9.2/langfuse/api/resources/commons/types/dataset_item.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/commons/types/dataset_run.py` & `langfuse-2.9.2/langfuse/api/resources/commons/types/dataset_run.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/commons/types/dataset_run_item.py` & `langfuse-2.9.2/langfuse/api/resources/commons/types/dataset_run_item.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/commons/types/observation.py` & `langfuse-2.9.2/langfuse/api/resources/commons/types/observation.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/commons/types/observation_level.py` & `langfuse-2.9.2/langfuse/api/resources/commons/types/observation_level.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/commons/types/observations_view.py` & `langfuse-2.9.2/langfuse/api/resources/commons/types/observations_view.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/commons/types/score.py` & `langfuse-2.9.2/langfuse/api/resources/commons/types/score.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/commons/types/session.py` & `langfuse-2.9.2/langfuse/api/resources/commons/types/session.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/commons/types/session_with_traces.py` & `langfuse-2.9.2/langfuse/api/resources/commons/types/session_with_traces.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/commons/types/trace.py` & `langfuse-2.9.2/langfuse/api/resources/commons/types/trace.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/commons/types/trace_with_details.py` & `langfuse-2.9.2/langfuse/api/resources/commons/types/trace_with_details.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/commons/types/trace_with_full_details.py` & `langfuse-2.9.2/langfuse/api/resources/commons/types/trace_with_full_details.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/commons/types/usage.py` & `langfuse-2.9.2/langfuse/api/resources/commons/types/usage.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/dataset_items/client.py` & `langfuse-2.9.2/langfuse/api/resources/dataset_items/client.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/dataset_items/types/create_dataset_item_request.py` & `langfuse-2.9.2/langfuse/api/resources/dataset_items/types/create_dataset_item_request.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/dataset_run_items/client.py` & `langfuse-2.9.2/langfuse/api/resources/dataset_run_items/client.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/dataset_run_items/types/create_dataset_run_item_request.py` & `langfuse-2.9.2/langfuse/api/resources/dataset_run_items/types/create_dataset_run_item_request.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/datasets/client.py` & `langfuse-2.9.2/langfuse/api/resources/datasets/client.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/datasets/types/create_dataset_request.py` & `langfuse-2.9.2/langfuse/api/resources/datasets/types/create_dataset_request.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/health/client.py` & `langfuse-2.9.2/langfuse/api/resources/health/client.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/health/types/health_response.py` & `langfuse-2.9.2/langfuse/api/resources/health/types/health_response.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/__init__.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/__init__.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/client.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/client.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/__init__.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/__init__.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/base_event.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/base_event.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/create_event_body.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/create_event_body.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/create_event_event.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/create_event_event.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/create_generation_body.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/create_generation_body.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/create_generation_event.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/create_generation_event.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/create_observation_event.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/create_observation_event.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/create_span_body.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/create_span_body.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/create_span_event.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/create_span_event.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/ingestion_error.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/ingestion_error.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/ingestion_event.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/ingestion_event.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/ingestion_response.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/ingestion_response.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/ingestion_success.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/ingestion_success.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/observation_body.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/observation_body.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/observation_type.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/observation_type.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/open_ai_usage.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/open_ai_usage.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/optional_observation_body.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/optional_observation_body.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/score_body.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/score_body.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/score_event.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/score_event.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/sdk_log_body.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/sdk_log_body.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/sdk_log_event.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/sdk_log_event.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/trace_body.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/trace_body.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/trace_event.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/trace_event.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/update_event_body.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/update_event_body.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/update_generation_body.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/update_generation_body.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/update_generation_event.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/update_generation_event.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/update_observation_event.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/update_observation_event.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/update_span_body.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/update_span_body.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/ingestion/types/update_span_event.py` & `langfuse-2.9.2/langfuse/api/resources/ingestion/types/update_span_event.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/observations/client.py` & `langfuse-2.9.2/langfuse/api/resources/observations/client.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/observations/types/observations.py` & `langfuse-2.9.2/langfuse/api/resources/observations/types/observations.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/observations/types/observations_views.py` & `langfuse-2.9.2/langfuse/api/resources/observations/types/observations_views.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/projects/client.py` & `langfuse-2.9.2/langfuse/api/resources/projects/client.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/projects/types/project.py` & `langfuse-2.9.2/langfuse/api/resources/projects/types/project.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/projects/types/projects.py` & `langfuse-2.9.2/langfuse/api/resources/projects/types/projects.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/prompts/client.py` & `langfuse-2.9.2/langfuse/api/resources/prompts/client.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/prompts/types/create_prompt_request.py` & `langfuse-2.9.2/langfuse/api/resources/prompts/types/create_prompt_request.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/prompts/types/prompt.py` & `langfuse-2.9.2/langfuse/api/resources/prompts/types/prompt.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/score/client.py` & `langfuse-2.9.2/langfuse/api/resources/score/client.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/score/types/create_score_request.py` & `langfuse-2.9.2/langfuse/api/resources/score/types/create_score_request.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/score/types/scores.py` & `langfuse-2.9.2/langfuse/api/resources/score/types/scores.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/sessions/client.py` & `langfuse-2.9.2/langfuse/api/resources/sessions/client.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/trace/client.py` & `langfuse-2.9.2/langfuse/api/resources/trace/client.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/trace/types/sort.py` & `langfuse-2.9.2/langfuse/api/resources/trace/types/sort.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/trace/types/traces.py` & `langfuse-2.9.2/langfuse/api/resources/trace/types/traces.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/api/resources/utils/resources/pagination/types/meta_response.py` & `langfuse-2.9.2/langfuse/api/resources/utils/resources/pagination/types/meta_response.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/callback.py` & `langfuse-2.9.2/langfuse/callback.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/client.py` & `langfuse-2.9.2/langfuse/client.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/environment.py` & `langfuse-2.9.2/langfuse/environment.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/model.py` & `langfuse-2.9.2/langfuse/model.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/openai.py` & `langfuse-2.9.2/langfuse/openai.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/prompt_cache.py` & `langfuse-2.9.2/langfuse/prompt_cache.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/request.py` & `langfuse-2.9.2/langfuse/request.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/serializer.py` & `langfuse-2.9.2/langfuse/serializer.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/task_manager.py` & `langfuse-2.9.2/langfuse/task_manager.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/langfuse/utils.py` & `langfuse-2.9.2/langfuse/utils.py`

 * *Files identical despite different names*

### Comparing `langfuse-2.9.1a0/pyproject.toml` & `langfuse-2.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langfuse"
-version = "2.9.1a0"
+version = "2.9.2"
 description = "A client library for accessing langfuse"
 authors = ["langfuse <developers@langfuse.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
```

### Comparing `langfuse-2.9.1a0/PKG-INFO` & `langfuse-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfuse
-Version: 2.9.1a0
+Version: 2.9.2
 Summary: A client library for accessing langfuse
 License: MIT
 Author: langfuse
 Author-email: developers@langfuse.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

