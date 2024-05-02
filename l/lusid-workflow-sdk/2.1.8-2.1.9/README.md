# Comparing `tmp/lusid_workflow_sdk-2.1.8.tar.gz` & `tmp/lusid_workflow_sdk-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_workflow_sdk-2.1.8.tar", max compression
+gzip compressed data, was "lusid_workflow_sdk-2.1.9.tar", max compression
```

## Comparing `lusid_workflow_sdk-2.1.8.tar` & `lusid_workflow_sdk-2.1.9.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0    12899 2024-05-01 17:34:02.568454 lusid_workflow_sdk-2.1.8/README.md
--rw-r--r--   0        0        0     8569 2024-05-01 17:34:02.563454 lusid_workflow_sdk-2.1.8/lusid_workflow/__init__.py
--rw-r--r--   0        0        0      406 2024-05-01 17:34:02.563454 lusid_workflow_sdk-2.1.8/lusid_workflow/api/__init__.py
--rw-r--r--   0        0        0     7534 2024-05-01 17:34:02.563454 lusid_workflow_sdk-2.1.8/lusid_workflow/api/application_metadata_api.py
--rw-r--r--   0        0        0    57597 2024-05-01 17:34:02.563454 lusid_workflow_sdk-2.1.8/lusid_workflow/api/task_definitions_api.py
--rw-r--r--   0        0        0    44655 2024-05-01 17:34:02.563454 lusid_workflow_sdk-2.1.8/lusid_workflow/api/tasks_api.py
--rw-r--r--   0        0        0    61860 2024-05-01 17:34:02.563454 lusid_workflow_sdk-2.1.8/lusid_workflow/api/workers_api.py
--rw-r--r--   0        0        0    30785 2024-05-01 17:34:02.564454 lusid_workflow_sdk-2.1.8/lusid_workflow/api_client.py
--rw-r--r--   0        0        0      852 2024-05-01 17:34:02.564454 lusid_workflow_sdk-2.1.8/lusid_workflow/api_response.py
--rw-r--r--   0        0        0    14451 2024-05-01 17:34:02.563454 lusid_workflow_sdk-2.1.8/lusid_workflow/configuration.py
--rw-r--r--   0        0        0     5339 2024-05-01 17:34:02.563454 lusid_workflow_sdk-2.1.8/lusid_workflow/exceptions.py
--rw-r--r--   0        0        0      587 2024-05-01 17:34:02.564454 lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/__init__.py
--rw-r--r--   0        0        0    30652 2024-05-01 17:34:02.564454 lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/api_client.py
--rw-r--r--   0        0        0     9862 2024-05-01 17:34:02.564454 lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8097 2024-05-01 17:34:02.564454 lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/api_configuration.py
--rw-r--r--   0        0        0     6796 2024-05-01 17:34:02.564454 lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-05-01 17:34:02.564454 lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-05-01 17:34:02.564454 lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12707 2024-05-01 17:34:02.564454 lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/rest.py
--rw-r--r--   0        0        0    11573 2024-05-01 17:34:02.564454 lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-05-01 17:34:02.564454 lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3886 2024-05-01 17:34:02.564454 lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     7134 2024-05-01 17:34:02.563454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/__init__.py
--rw-r--r--   0        0        0     3903 2024-05-01 17:34:02.559455 lusid_workflow_sdk-2.1.8/lusid_workflow/models/access_controlled_action.py
--rw-r--r--   0        0        0     4846 2024-05-01 17:34:02.560454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/access_controlled_resource.py
--rw-r--r--   0        0        0     3649 2024-05-01 17:34:02.560454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/action_definition.py
--rw-r--r--   0        0        0     3233 2024-05-01 17:34:02.560454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/action_definition_response.py
--rw-r--r--   0        0        0     6172 2024-05-01 17:34:02.560454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/action_details.py
--rw-r--r--   0        0        0     6643 2024-05-01 17:34:02.560454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/action_details_response.py
--rw-r--r--   0        0        0     2070 2024-05-01 17:34:02.560454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/action_id.py
--rw-r--r--   0        0        0     5406 2024-05-01 17:34:02.560454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/create_child_task_configuration.py
--rw-r--r--   0        0        0     3165 2024-05-01 17:34:02.560454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/create_child_tasks_action.py
--rw-r--r--   0        0        0     3766 2024-05-01 17:34:02.560454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/create_child_tasks_action_response.py
--rw-r--r--   0        0        0     7468 2024-05-01 17:34:02.560454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/create_task_definition_request.py
--rw-r--r--   0        0        0     4145 2024-05-01 17:34:02.560454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/create_task_request.py
--rw-r--r--   0        0        0     3972 2024-05-01 17:34:02.560454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/create_worker_request.py
--rw-r--r--   0        0        0     3459 2024-05-01 17:34:02.560454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/deleted_entity_response.py
--rw-r--r--   0        0        0     2193 2024-05-01 17:34:02.560454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/fail.py
--rw-r--r--   0        0        0     2505 2024-05-01 17:34:02.560454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/fail_response.py
--rw-r--r--   0        0        0     2878 2024-05-01 17:34:02.560454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/field_mapping.py
--rw-r--r--   0        0        0     2607 2024-05-01 17:34:02.560454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/get_worker_result_response.py
--rw-r--r--   0        0        0     2341 2024-05-01 17:34:02.560454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/health_check.py
--rw-r--r--   0        0        0     2814 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/health_check_response.py
--rw-r--r--   0        0        0     3180 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/id_selector_definition.py
--rw-r--r--   0        0        0     3105 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/identifier_part_schema.py
--rw-r--r--   0        0        0     2723 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/initial_state.py
--rw-r--r--   0        0        0     2262 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/link.py
--rw-r--r--   0        0        0     2607 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/luminesce_view.py
--rw-r--r--   0        0        0     2811 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/luminesce_view_response.py
--rw-r--r--   0        0        0     3857 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4693 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     4053 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/paged_resource_list_of_task.py
--rw-r--r--   0        0        0     4174 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/paged_resource_list_of_task_definition.py
--rw-r--r--   0        0        0     4077 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/paged_resource_list_of_worker.py
--rw-r--r--   0        0        0     3317 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/parameter.py
--rw-r--r--   0        0        0     2583 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/parameter_value.py
--rw-r--r--   0        0        0     1869 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/resource_id.py
--rw-r--r--   0        0        0     4255 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     4013 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/resource_list_of_task.py
--rw-r--r--   0        0        0     2793 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/result_field.py
--rw-r--r--   0        0        0     2293 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/result_matching_pattern.py
--rw-r--r--   0        0        0     5713 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/resultant_child_task_configuration.py
--rw-r--r--   0        0        0     5913 2024-05-01 17:34:02.561454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/run_worker_action.py
--rw-r--r--   0        0        0     6227 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/run_worker_action_response.py
--rw-r--r--   0        0        0     2428 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/run_worker_request.py
--rw-r--r--   0        0        0     2360 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/run_worker_response.py
--rw-r--r--   0        0        0     2541 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/scheduler_job.py
--rw-r--r--   0        0        0     2864 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/scheduler_job_response.py
--rw-r--r--   0        0        0     2116 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/sleep.py
--rw-r--r--   0        0        0     2172 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/sleep_response.py
--rw-r--r--   0        0        0     4397 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/stack.py
--rw-r--r--   0        0        0     8353 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/task.py
--rw-r--r--   0        0        0     7864 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/task_definition.py
--rw-r--r--   0        0        0     2090 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/task_definition_version.py
--rw-r--r--   0        0        0     2483 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/task_field_definition.py
--rw-r--r--   0        0        0     2546 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/task_instance_field.py
--rw-r--r--   0        0        0     2279 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/task_state_definition.py
--rw-r--r--   0        0        0     3415 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/task_summary.py
--rw-r--r--   0        0        0     4806 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/task_transition_definition.py
--rw-r--r--   0        0        0     2728 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/transition_trigger_definition.py
--rw-r--r--   0        0        0     2716 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/trigger_parent_task_action.py
--rw-r--r--   0        0        0     2910 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/trigger_parent_task_action_response.py
--rw-r--r--   0        0        0     1951 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/trigger_schema.py
--rw-r--r--   0        0        0     7130 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/update_task_definition_request.py
--rw-r--r--   0        0        0     3588 2024-05-01 17:34:02.562454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/update_task_request.py
--rw-r--r--   0        0        0     3579 2024-05-01 17:34:02.563454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/update_worker_request.py
--rw-r--r--   0        0        0     5124 2024-05-01 17:34:02.563454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/version_info.py
--rw-r--r--   0        0        0     6137 2024-05-01 17:34:02.563454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/worker.py
--rw-r--r--   0        0        0     7051 2024-05-01 17:34:02.563454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/worker_configuration.py
--rw-r--r--   0        0        0     7753 2024-05-01 17:34:02.563454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/worker_configuration_response.py
--rw-r--r--   0        0        0     4204 2024-05-01 17:34:02.563454 lusid_workflow_sdk-2.1.8/lusid_workflow/models/worker_status_triggers.py
--rw-r--r--   0        0        0        0 2024-05-01 17:34:02.563454 lusid_workflow_sdk-2.1.8/lusid_workflow/py.typed
--rw-r--r--   0        0        0    10160 2024-05-01 17:34:02.564454 lusid_workflow_sdk-2.1.8/lusid_workflow/rest.py
--rw-r--r--   0        0        0      855 2024-05-01 17:34:02.568454 lusid_workflow_sdk-2.1.8/pyproject.toml
--rw-r--r--   0        0        0    13944 1970-01-01 00:00:00.000000 lusid_workflow_sdk-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0    12899 2024-05-02 21:26:46.242256 lusid_workflow_sdk-2.1.9/README.md
+-rw-r--r--   0        0        0     8569 2024-05-02 21:26:46.238256 lusid_workflow_sdk-2.1.9/lusid_workflow/__init__.py
+-rw-r--r--   0        0        0      406 2024-05-02 21:26:46.238256 lusid_workflow_sdk-2.1.9/lusid_workflow/api/__init__.py
+-rw-r--r--   0        0        0     7534 2024-05-02 21:26:46.237256 lusid_workflow_sdk-2.1.9/lusid_workflow/api/application_metadata_api.py
+-rw-r--r--   0        0        0    57597 2024-05-02 21:26:46.237256 lusid_workflow_sdk-2.1.9/lusid_workflow/api/task_definitions_api.py
+-rw-r--r--   0        0        0    44655 2024-05-02 21:26:46.237256 lusid_workflow_sdk-2.1.9/lusid_workflow/api/tasks_api.py
+-rw-r--r--   0        0        0    61860 2024-05-02 21:26:46.237256 lusid_workflow_sdk-2.1.9/lusid_workflow/api/workers_api.py
+-rw-r--r--   0        0        0    30785 2024-05-02 21:26:46.238256 lusid_workflow_sdk-2.1.9/lusid_workflow/api_client.py
+-rw-r--r--   0        0        0      855 2024-05-02 21:26:46.238256 lusid_workflow_sdk-2.1.9/lusid_workflow/api_response.py
+-rw-r--r--   0        0        0    14451 2024-05-02 21:26:46.238256 lusid_workflow_sdk-2.1.9/lusid_workflow/configuration.py
+-rw-r--r--   0        0        0     5339 2024-05-02 21:26:46.238256 lusid_workflow_sdk-2.1.9/lusid_workflow/exceptions.py
+-rw-r--r--   0        0        0      587 2024-05-02 21:26:46.238256 lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/__init__.py
+-rw-r--r--   0        0        0    30652 2024-05-02 21:26:46.238256 lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/api_client.py
+-rw-r--r--   0        0        0     9862 2024-05-02 21:26:46.238256 lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8097 2024-05-02 21:26:46.238256 lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6796 2024-05-02 21:26:46.238256 lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-05-02 21:26:46.238256 lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-05-02 21:26:46.238256 lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12707 2024-05-02 21:26:46.238256 lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/rest.py
+-rw-r--r--   0        0        0    11573 2024-05-02 21:26:46.238256 lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-05-02 21:26:46.238256 lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3886 2024-05-02 21:26:46.238256 lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     7134 2024-05-02 21:26:46.237256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/__init__.py
+-rw-r--r--   0        0        0     3903 2024-05-02 21:26:46.234256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4846 2024-05-02 21:26:46.234256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     3649 2024-05-02 21:26:46.234256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/action_definition.py
+-rw-r--r--   0        0        0     3233 2024-05-02 21:26:46.234256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/action_definition_response.py
+-rw-r--r--   0        0        0     6178 2024-05-02 21:26:46.234256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/action_details.py
+-rw-r--r--   0        0        0     6649 2024-05-02 21:26:46.234256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/action_details_response.py
+-rw-r--r--   0        0        0     2070 2024-05-02 21:26:46.234256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/action_id.py
+-rw-r--r--   0        0        0     5406 2024-05-02 21:26:46.234256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/create_child_task_configuration.py
+-rw-r--r--   0        0        0     3165 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/create_child_tasks_action.py
+-rw-r--r--   0        0        0     3766 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/create_child_tasks_action_response.py
+-rw-r--r--   0        0        0     7468 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/create_task_definition_request.py
+-rw-r--r--   0        0        0     4145 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/create_task_request.py
+-rw-r--r--   0        0        0     3972 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/create_worker_request.py
+-rw-r--r--   0        0        0     3459 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/deleted_entity_response.py
+-rw-r--r--   0        0        0     2193 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/fail.py
+-rw-r--r--   0        0        0     2505 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/fail_response.py
+-rw-r--r--   0        0        0     2878 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/field_mapping.py
+-rw-r--r--   0        0        0     2607 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/get_worker_result_response.py
+-rw-r--r--   0        0        0     2341 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/health_check.py
+-rw-r--r--   0        0        0     2814 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/health_check_response.py
+-rw-r--r--   0        0        0     3180 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3105 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     2723 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/initial_state.py
+-rw-r--r--   0        0        0     2262 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/link.py
+-rw-r--r--   0        0        0     2607 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/luminesce_view.py
+-rw-r--r--   0        0        0     2811 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/luminesce_view_response.py
+-rw-r--r--   0        0        0     3857 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4693 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     4053 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/paged_resource_list_of_task.py
+-rw-r--r--   0        0        0     4174 2024-05-02 21:26:46.235256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/paged_resource_list_of_task_definition.py
+-rw-r--r--   0        0        0     4077 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/paged_resource_list_of_worker.py
+-rw-r--r--   0        0        0     3317 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/parameter.py
+-rw-r--r--   0        0        0     2583 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/parameter_value.py
+-rw-r--r--   0        0        0     1869 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/resource_id.py
+-rw-r--r--   0        0        0     4255 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     4013 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/resource_list_of_task.py
+-rw-r--r--   0        0        0     2793 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/result_field.py
+-rw-r--r--   0        0        0     2293 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/result_matching_pattern.py
+-rw-r--r--   0        0        0     5713 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/resultant_child_task_configuration.py
+-rw-r--r--   0        0        0     5913 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/run_worker_action.py
+-rw-r--r--   0        0        0     6227 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/run_worker_action_response.py
+-rw-r--r--   0        0        0     2428 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/run_worker_request.py
+-rw-r--r--   0        0        0     2360 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/run_worker_response.py
+-rw-r--r--   0        0        0     2541 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/scheduler_job.py
+-rw-r--r--   0        0        0     2864 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/scheduler_job_response.py
+-rw-r--r--   0        0        0     2116 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/sleep.py
+-rw-r--r--   0        0        0     2172 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/sleep_response.py
+-rw-r--r--   0        0        0     4397 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/stack.py
+-rw-r--r--   0        0        0     8353 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/task.py
+-rw-r--r--   0        0        0     7864 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/task_definition.py
+-rw-r--r--   0        0        0     2090 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/task_definition_version.py
+-rw-r--r--   0        0        0     2483 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/task_field_definition.py
+-rw-r--r--   0        0        0     2546 2024-05-02 21:26:46.236256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/task_instance_field.py
+-rw-r--r--   0        0        0     2279 2024-05-02 21:26:46.237256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/task_state_definition.py
+-rw-r--r--   0        0        0     3415 2024-05-02 21:26:46.237256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/task_summary.py
+-rw-r--r--   0        0        0     4806 2024-05-02 21:26:46.237256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/task_transition_definition.py
+-rw-r--r--   0        0        0     2728 2024-05-02 21:26:46.237256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/transition_trigger_definition.py
+-rw-r--r--   0        0        0     2716 2024-05-02 21:26:46.237256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/trigger_parent_task_action.py
+-rw-r--r--   0        0        0     2910 2024-05-02 21:26:46.237256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/trigger_parent_task_action_response.py
+-rw-r--r--   0        0        0     1951 2024-05-02 21:26:46.237256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/trigger_schema.py
+-rw-r--r--   0        0        0     7130 2024-05-02 21:26:46.237256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/update_task_definition_request.py
+-rw-r--r--   0        0        0     3588 2024-05-02 21:26:46.237256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/update_task_request.py
+-rw-r--r--   0        0        0     3579 2024-05-02 21:26:46.237256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/update_worker_request.py
+-rw-r--r--   0        0        0     5124 2024-05-02 21:26:46.237256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/version_info.py
+-rw-r--r--   0        0        0     6137 2024-05-02 21:26:46.237256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/worker.py
+-rw-r--r--   0        0        0     7057 2024-05-02 21:26:46.237256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/worker_configuration.py
+-rw-r--r--   0        0        0     7759 2024-05-02 21:26:46.237256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/worker_configuration_response.py
+-rw-r--r--   0        0        0     4204 2024-05-02 21:26:46.237256 lusid_workflow_sdk-2.1.9/lusid_workflow/models/worker_status_triggers.py
+-rw-r--r--   0        0        0        0 2024-05-02 21:26:46.238256 lusid_workflow_sdk-2.1.9/lusid_workflow/py.typed
+-rw-r--r--   0        0        0    10160 2024-05-02 21:26:46.238256 lusid_workflow_sdk-2.1.9/lusid_workflow/rest.py
+-rw-r--r--   0        0        0      855 2024-05-02 21:26:46.242256 lusid_workflow_sdk-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0    13944 1970-01-01 00:00:00.000000 lusid_workflow_sdk-2.1.9/PKG-INFO
```

### Comparing `lusid_workflow_sdk-2.1.8/README.md` & `lusid_workflow_sdk-2.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-workflow-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.966
-- Package version: 2.1.8
+- API version: 0.1.973
+- Package version: 2.1.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/__init__.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/api/application_metadata_api.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/api/application_metadata_api.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/api/task_definitions_api.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/api/task_definitions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/api/tasks_api.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/api/tasks_api.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/api/workers_api.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/api/workers_api.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/api_client.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/api_response.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/api_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """API response object."""
 
 from __future__ import annotations
 from typing import Any, Dict, Optional
-from pydantic import Field, StrictInt, StrictStr
+from pydantic.v1 import Field, StrictInt, StrictStr
 
 class ApiResponse:
     """
     API response object
     """
 
     status_code: Optional[StrictInt] = Field(None, description="HTTP status code")
```

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/configuration.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("lusid_workflow-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.966\n"\
+               "Version of the API: 0.1.973\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/exceptions.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/__init__.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/api_client.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/api_client_factory.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/api_configuration.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/configuration_loaders.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/proxy_config.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/refreshing_token.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/rest.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/retry.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/socket_keep_alive.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/extensions/tcp_keep_alive_connector.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/__init__.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/access_controlled_action.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/access_controlled_action.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/access_controlled_resource.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/action_definition.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/action_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/action_definition_response.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/action_definition_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/action_details.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/action_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 
 from typing import Any, List, Optional
-from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
+from pydantic.v1 import BaseModel, Field, StrictStr, ValidationError, validator
 from lusid_workflow.models.create_child_tasks_action import CreateChildTasksAction
 from lusid_workflow.models.run_worker_action import RunWorkerAction
 from lusid_workflow.models.trigger_parent_task_action import TriggerParentTaskAction
 from typing import Union, Any, List, TYPE_CHECKING
-from pydantic import StrictStr, Field
+from pydantic.v1 import StrictStr, Field
 
 ACTIONDETAILS_ONE_OF_SCHEMAS = ["CreateChildTasksAction", "RunWorkerAction", "TriggerParentTaskAction"]
 
 class ActionDetails(BaseModel):
     """
     Abstracts the kinds of Actions available
     """
```

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/action_details_response.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/action_details_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 
 from typing import Any, List, Optional
-from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
+from pydantic.v1 import BaseModel, Field, StrictStr, ValidationError, validator
 from lusid_workflow.models.create_child_tasks_action_response import CreateChildTasksActionResponse
 from lusid_workflow.models.run_worker_action_response import RunWorkerActionResponse
 from lusid_workflow.models.trigger_parent_task_action_response import TriggerParentTaskActionResponse
 from typing import Union, Any, List, TYPE_CHECKING
-from pydantic import StrictStr, Field
+from pydantic.v1 import StrictStr, Field
 
 ACTIONDETAILSRESPONSE_ONE_OF_SCHEMAS = ["CreateChildTasksActionResponse", "RunWorkerActionResponse", "TriggerParentTaskActionResponse"]
 
 class ActionDetailsResponse(BaseModel):
     """
     Abstracts the kinds of Actions available in a read-only form
     """
```

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/action_id.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/action_id.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/create_child_task_configuration.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/create_child_task_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/create_child_tasks_action.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/create_child_tasks_action.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/create_child_tasks_action_response.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/create_child_tasks_action_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/create_task_definition_request.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/create_task_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/create_task_request.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/create_task_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/create_worker_request.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/create_worker_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/deleted_entity_response.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/deleted_entity_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/fail.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/fail.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/fail_response.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/fail_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/field_mapping.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/field_mapping.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/get_worker_result_response.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/get_worker_result_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/health_check.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/health_check.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/health_check_response.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/health_check_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/id_selector_definition.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/id_selector_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/identifier_part_schema.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/identifier_part_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/initial_state.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/initial_state.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/link.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/link.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/luminesce_view.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/luminesce_view.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/luminesce_view_response.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/luminesce_view_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/lusid_problem_details.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/lusid_validation_problem_details.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/paged_resource_list_of_task.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/paged_resource_list_of_task.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/paged_resource_list_of_task_definition.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/paged_resource_list_of_task_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/paged_resource_list_of_worker.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/paged_resource_list_of_worker.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/parameter.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/parameter_value.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/parameter_value.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/resource_id.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/resource_id.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/resource_list_of_access_controlled_resource.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/resource_list_of_access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/resource_list_of_task.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/resource_list_of_task.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/result_field.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/result_field.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/result_matching_pattern.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/result_matching_pattern.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/resultant_child_task_configuration.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/resultant_child_task_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/run_worker_action.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/run_worker_action.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/run_worker_action_response.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/run_worker_action_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/run_worker_request.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/run_worker_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/run_worker_response.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/run_worker_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/scheduler_job.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/scheduler_job.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/scheduler_job_response.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/scheduler_job_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/sleep.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/sleep.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/sleep_response.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/sleep_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/stack.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/stack.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/task.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/task.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/task_definition.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/task_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/task_definition_version.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/task_definition_version.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/task_field_definition.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/task_field_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/task_instance_field.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/task_instance_field.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/task_state_definition.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/task_state_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/task_summary.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/task_summary.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/task_transition_definition.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/task_transition_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/transition_trigger_definition.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/transition_trigger_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/trigger_parent_task_action.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/trigger_parent_task_action.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/trigger_parent_task_action_response.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/trigger_parent_task_action_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/trigger_schema.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/trigger_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/update_task_definition_request.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/update_task_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/update_task_request.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/update_task_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/update_worker_request.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/update_worker_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/version_info.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/version_info.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/worker.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/worker.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/worker_configuration.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/worker_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 
 from typing import Any, List, Optional
-from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
+from pydantic.v1 import BaseModel, Field, StrictStr, ValidationError, validator
 from lusid_workflow.models.fail import Fail
 from lusid_workflow.models.health_check import HealthCheck
 from lusid_workflow.models.luminesce_view import LuminesceView
 from lusid_workflow.models.scheduler_job import SchedulerJob
 from lusid_workflow.models.sleep import Sleep
 from typing import Union, Any, List, TYPE_CHECKING
-from pydantic import StrictStr, Field
+from pydantic.v1 import StrictStr, Field
 
 WORKERCONFIGURATION_ONE_OF_SCHEMAS = ["Fail", "HealthCheck", "LuminesceView", "SchedulerJob", "Sleep"]
 
 class WorkerConfiguration(BaseModel):
     """
     Information about how the worker should be executed
     """
```

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/worker_configuration_response.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/worker_configuration_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import json
 import pprint
 import re  # noqa: F401
 
 from typing import Any, List, Optional
-from pydantic import BaseModel, Field, StrictStr, ValidationError, validator
+from pydantic.v1 import BaseModel, Field, StrictStr, ValidationError, validator
 from lusid_workflow.models.fail_response import FailResponse
 from lusid_workflow.models.health_check_response import HealthCheckResponse
 from lusid_workflow.models.luminesce_view_response import LuminesceViewResponse
 from lusid_workflow.models.scheduler_job_response import SchedulerJobResponse
 from lusid_workflow.models.sleep_response import SleepResponse
 from typing import Union, Any, List, TYPE_CHECKING
-from pydantic import StrictStr, Field
+from pydantic.v1 import StrictStr, Field
 
 WORKERCONFIGURATIONRESPONSE_ONE_OF_SCHEMAS = ["FailResponse", "HealthCheckResponse", "LuminesceViewResponse", "SchedulerJobResponse", "SleepResponse"]
 
 class WorkerConfigurationResponse(BaseModel):
     """
     Readonly information about how the worker should be executed
     """
```

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/models/worker_status_triggers.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/models/worker_status_triggers.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/lusid_workflow/rest.py` & `lusid_workflow_sdk-2.1.9/lusid_workflow/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.1.8/pyproject.toml` & `lusid_workflow_sdk-2.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lusid-workflow-sdk"
-version = "2.1.8"
+version = "2.1.9"
 description = "FINBOURNE Workflow API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/workflow-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Workflow API", "lusid-workflow-sdk"]
 packages = [
```

### Comparing `lusid_workflow_sdk-2.1.8/PKG-INFO` & `lusid_workflow_sdk-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-workflow-sdk
-Version: 2.1.8
+Version: 2.1.9
 Summary: FINBOURNE Workflow API
 Home-page: https://github.com/finbourne/workflow-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Workflow API,lusid-workflow-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # lusid-workflow-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.966
-- Package version: 2.1.8
+- API version: 0.1.973
+- Package version: 2.1.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

