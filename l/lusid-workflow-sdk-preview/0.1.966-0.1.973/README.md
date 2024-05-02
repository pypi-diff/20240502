# Comparing `tmp/lusid-workflow-sdk-preview-0.1.966.tar.gz` & `tmp/lusid-workflow-sdk-preview-0.1.973.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lusid-workflow-sdk-preview-0.1.966.tar", last modified: Wed May  1 17:31:44 2024, max compression
+gzip compressed data, was "dist/lusid-workflow-sdk-preview-0.1.973.tar", last modified: Thu May  2 21:24:12 2024, max compression
```

## Comparing `lusid-workflow-sdk-preview-0.1.966.tar` & `lusid-workflow-sdk-preview-0.1.973.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 17:31:44.000000 lusid-workflow-sdk-preview-0.1.966/
--rw-r--r--   0 root         (0) root         (0)       49 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      353 2024-05-01 17:31:44.000000 lusid-workflow-sdk-preview-0.1.966/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9995 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 17:31:44.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/
--rw-r--r--   0 root         (0) root         (0)     6528 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)       24 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 17:31:44.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/api/
--rw-r--r--   0 root         (0) root         (0)      341 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6826 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/api/application_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    57864 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/api/task_definitions_api.py
--rw-r--r--   0 root         (0) root         (0)    42809 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/api/tasks_api.py
--rw-r--r--   0 root         (0) root         (0)    62480 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/api/workers_api.py
--rw-r--r--   0 root         (0) root         (0)    27758 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16610 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5094 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 17:31:44.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/
--rw-r--r--   0 root         (0) root         (0)     5369 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7209 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/access_controlled_action.py
--rw-r--r--   0 root         (0) root         (0)     8972 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     8262 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/action_definition.py
--rw-r--r--   0 root         (0) root         (0)     6409 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/action_definition_response.py
--rw-r--r--   0 root         (0) root         (0)    12100 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/action_details.py
--rw-r--r--   0 root         (0) root         (0)    10733 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/action_details_response.py
--rw-r--r--   0 root         (0) root         (0)     7222 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/action_id.py
--rw-r--r--   0 root         (0) root         (0)    10122 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/create_child_task_configuration.py
--rw-r--r--   0 root         (0) root         (0)     6232 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/create_child_tasks_action.py
--rw-r--r--   0 root         (0) root         (0)     5895 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/create_child_tasks_action_response.py
--rw-r--r--   0 root         (0) root         (0)    13450 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/create_task_definition_request.py
--rw-r--r--   0 root         (0) root         (0)     7821 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/create_task_request.py
--rw-r--r--   0 root         (0) root         (0)     9176 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/create_worker_request.py
--rw-r--r--   0 root         (0) root         (0)     6852 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/deleted_entity_response.py
--rw-r--r--   0 root         (0) root         (0)     4368 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/fail.py
--rw-r--r--   0 root         (0) root         (0)     4239 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/fail_response.py
--rw-r--r--   0 root         (0) root         (0)     5622 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/field_mapping.py
--rw-r--r--   0 root         (0) root         (0)     6800 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/get_worker_result_response.py
--rw-r--r--   0 root         (0) root         (0)     5878 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/health_check.py
--rw-r--r--   0 root         (0) root         (0)     5112 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/health_check_response.py
--rw-r--r--   0 root         (0) root         (0)     8000 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/id_selector_definition.py
--rw-r--r--   0 root         (0) root         (0)     9489 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/identifier_part_schema.py
--rw-r--r--   0 root         (0) root         (0)     5984 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/initial_state.py
--rw-r--r--   0 root         (0) root         (0)     6416 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/link.py
--rw-r--r--   0 root         (0) root         (0)     6165 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/luminesce_view.py
--rw-r--r--   0 root         (0) root         (0)     5113 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/luminesce_view_response.py
--rw-r--r--   0 root         (0) root         (0)     9530 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/lusid_problem_details.py
--rw-r--r--   0 root         (0) root         (0)    10695 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/lusid_validation_problem_details.py
--rw-r--r--   0 root         (0) root         (0)     7295 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/paged_resource_list_of_task.py
--rw-r--r--   0 root         (0) root         (0)     7575 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/paged_resource_list_of_task_definition.py
--rw-r--r--   0 root         (0) root         (0)     7351 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/paged_resource_list_of_worker.py
--rw-r--r--   0 root         (0) root         (0)     9076 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/parameter.py
--rw-r--r--   0 root         (0) root         (0)     5767 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/parameter_value.py
--rw-r--r--   0 root         (0) root         (0)     4822 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/resource_id.py
--rw-r--r--   0 root         (0) root         (0)     7735 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0 root         (0) root         (0)     7175 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/resource_list_of_task.py
--rw-r--r--   0 root         (0) root         (0)     7211 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/result_field.py
--rw-r--r--   0 root         (0) root         (0)     4985 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/result_matching_pattern.py
--rw-r--r--   0 root         (0) root         (0)    11562 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/resultant_child_task_configuration.py
--rw-r--r--   0 root         (0) root         (0)    10386 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/run_worker_action.py
--rw-r--r--   0 root         (0) root         (0)    10247 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/run_worker_action_response.py
--rw-r--r--   0 root         (0) root         (0)     4435 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/run_worker_request.py
--rw-r--r--   0 root         (0) root         (0)     5179 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/run_worker_response.py
--rw-r--r--   0 root         (0) root         (0)     5383 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/scheduler_job.py
--rw-r--r--   0 root         (0) root         (0)     5119 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/scheduler_job_response.py
--rw-r--r--   0 root         (0) root         (0)     4377 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/sleep.py
--rw-r--r--   0 root         (0) root         (0)     4441 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/sleep_response.py
--rw-r--r--   0 root         (0) root         (0)    11504 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/stack.py
--rw-r--r--   0 root         (0) root         (0)    19688 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/task.py
--rw-r--r--   0 root         (0) root         (0)    14093 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/task_definition.py
--rw-r--r--   0 root         (0) root         (0)     4386 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/task_definition_version.py
--rw-r--r--   0 root         (0) root         (0)     6387 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/task_field_definition.py
--rw-r--r--   0 root         (0) root         (0)     5243 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/task_instance_field.py
--rw-r--r--   0 root         (0) root         (0)     4944 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/task_state_definition.py
--rw-r--r--   0 root         (0) root         (0)     9826 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/task_summary.py
--rw-r--r--   0 root         (0) root         (0)    12376 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/task_transition_definition.py
--rw-r--r--   0 root         (0) root         (0)     6067 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/transition_trigger_definition.py
--rw-r--r--   0 root         (0) root         (0)     6451 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/trigger_parent_task_action.py
--rw-r--r--   0 root         (0) root         (0)     5348 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/trigger_parent_task_action_response.py
--rw-r--r--   0 root         (0) root         (0)     4440 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/trigger_schema.py
--rw-r--r--   0 root         (0) root         (0)    12546 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/update_task_definition_request.py
--rw-r--r--   0 root         (0) root         (0)     6427 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/update_task_request.py
--rw-r--r--   0 root         (0) root         (0)     8188 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/update_worker_request.py
--rw-r--r--   0 root         (0) root         (0)    11105 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/version_info.py
--rw-r--r--   0 root         (0) root         (0)    11171 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/worker.py
--rw-r--r--   0 root         (0) root         (0)     8585 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/worker_configuration.py
--rw-r--r--   0 root         (0) root         (0)     7048 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/worker_configuration_response.py
--rw-r--r--   0 root         (0) root         (0)     8967 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/worker_status_triggers.py
--rw-r--r--   0 root         (0) root         (0)    13551 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 17:31:44.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/utilities/
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/utilities/config_keys.json
--rw-r--r--   0 root         (0) root         (0)      295 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow/utilities/config_keys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-01 17:31:44.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow_sdk_preview.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2024-05-01 17:31:44.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow_sdk_preview.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3924 2024-05-01 17:31:44.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow_sdk_preview.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-01 17:31:44.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow_sdk_preview.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      116 2024-05-01 17:31:44.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow_sdk_preview.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-01 17:31:44.000000 lusid-workflow-sdk-preview-0.1.966/lusid_workflow_sdk_preview.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-01 17:31:44.000000 lusid-workflow-sdk-preview-0.1.966/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2237 2024-05-01 17:30:46.000000 lusid-workflow-sdk-preview-0.1.966/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/
+-rw-r--r--   0 root         (0) root         (0)       49 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      353 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9995 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/
+-rw-r--r--   0 root         (0) root         (0)     6528 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       24 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api/
+-rw-r--r--   0 root         (0) root         (0)      341 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6826 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api/application_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    57864 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api/task_definitions_api.py
+-rw-r--r--   0 root         (0) root         (0)    42809 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api/tasks_api.py
+-rw-r--r--   0 root         (0) root         (0)    62480 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api/workers_api.py
+-rw-r--r--   0 root         (0) root         (0)    27758 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    16610 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5094 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/
+-rw-r--r--   0 root         (0) root         (0)     5369 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7209 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/access_controlled_action.py
+-rw-r--r--   0 root         (0) root         (0)     8972 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     8262 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/action_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6409 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/action_definition_response.py
+-rw-r--r--   0 root         (0) root         (0)    12100 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/action_details.py
+-rw-r--r--   0 root         (0) root         (0)    10733 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/action_details_response.py
+-rw-r--r--   0 root         (0) root         (0)     7222 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/action_id.py
+-rw-r--r--   0 root         (0) root         (0)    10122 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_child_task_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     6232 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_child_tasks_action.py
+-rw-r--r--   0 root         (0) root         (0)     5895 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_child_tasks_action_response.py
+-rw-r--r--   0 root         (0) root         (0)    13450 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_task_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     7821 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_task_request.py
+-rw-r--r--   0 root         (0) root         (0)     9176 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_worker_request.py
+-rw-r--r--   0 root         (0) root         (0)     6852 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/deleted_entity_response.py
+-rw-r--r--   0 root         (0) root         (0)     4368 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/fail.py
+-rw-r--r--   0 root         (0) root         (0)     4239 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/fail_response.py
+-rw-r--r--   0 root         (0) root         (0)     5622 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/field_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     6800 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/get_worker_result_response.py
+-rw-r--r--   0 root         (0) root         (0)     5878 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/health_check.py
+-rw-r--r--   0 root         (0) root         (0)     5112 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/health_check_response.py
+-rw-r--r--   0 root         (0) root         (0)     8000 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/id_selector_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9489 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/identifier_part_schema.py
+-rw-r--r--   0 root         (0) root         (0)     5984 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/initial_state.py
+-rw-r--r--   0 root         (0) root         (0)     6416 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/link.py
+-rw-r--r--   0 root         (0) root         (0)     6165 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/luminesce_view.py
+-rw-r--r--   0 root         (0) root         (0)     5113 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/luminesce_view_response.py
+-rw-r--r--   0 root         (0) root         (0)     9530 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/lusid_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)    10695 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/lusid_validation_problem_details.py
+-rw-r--r--   0 root         (0) root         (0)     7295 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/paged_resource_list_of_task.py
+-rw-r--r--   0 root         (0) root         (0)     7575 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/paged_resource_list_of_task_definition.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/paged_resource_list_of_worker.py
+-rw-r--r--   0 root         (0) root         (0)     9076 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/parameter.py
+-rw-r--r--   0 root         (0) root         (0)     5767 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/parameter_value.py
+-rw-r--r--   0 root         (0) root         (0)     4822 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/resource_id.py
+-rw-r--r--   0 root         (0) root         (0)     7735 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0 root         (0) root         (0)     7175 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/resource_list_of_task.py
+-rw-r--r--   0 root         (0) root         (0)     7211 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/result_field.py
+-rw-r--r--   0 root         (0) root         (0)     4985 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/result_matching_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    11562 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/resultant_child_task_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    10386 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/run_worker_action.py
+-rw-r--r--   0 root         (0) root         (0)    10247 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/run_worker_action_response.py
+-rw-r--r--   0 root         (0) root         (0)     4435 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/run_worker_request.py
+-rw-r--r--   0 root         (0) root         (0)     5179 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/run_worker_response.py
+-rw-r--r--   0 root         (0) root         (0)     5383 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/scheduler_job.py
+-rw-r--r--   0 root         (0) root         (0)     5119 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/scheduler_job_response.py
+-rw-r--r--   0 root         (0) root         (0)     4377 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/sleep.py
+-rw-r--r--   0 root         (0) root         (0)     4441 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/sleep_response.py
+-rw-r--r--   0 root         (0) root         (0)    11504 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/stack.py
+-rw-r--r--   0 root         (0) root         (0)    19688 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task.py
+-rw-r--r--   0 root         (0) root         (0)    14093 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_definition.py
+-rw-r--r--   0 root         (0) root         (0)     4386 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_definition_version.py
+-rw-r--r--   0 root         (0) root         (0)     6387 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_field_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5243 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_instance_field.py
+-rw-r--r--   0 root         (0) root         (0)     4944 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_state_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9826 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_summary.py
+-rw-r--r--   0 root         (0) root         (0)    12376 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_transition_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6067 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/transition_trigger_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6451 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/trigger_parent_task_action.py
+-rw-r--r--   0 root         (0) root         (0)     5348 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/trigger_parent_task_action_response.py
+-rw-r--r--   0 root         (0) root         (0)     4440 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/trigger_schema.py
+-rw-r--r--   0 root         (0) root         (0)    12546 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/update_task_definition_request.py
+-rw-r--r--   0 root         (0) root         (0)     6427 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/update_task_request.py
+-rw-r--r--   0 root         (0) root         (0)     8188 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/update_worker_request.py
+-rw-r--r--   0 root         (0) root         (0)    11105 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/version_info.py
+-rw-r--r--   0 root         (0) root         (0)    11171 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/worker.py
+-rw-r--r--   0 root         (0) root         (0)     8585 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/worker_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     7048 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/worker_configuration_response.py
+-rw-r--r--   0 root         (0) root         (0)     8967 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/worker_status_triggers.py
+-rw-r--r--   0 root         (0) root         (0)    13551 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/utilities/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/utilities/config_keys.json
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow/utilities/config_keys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow_sdk_preview.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow_sdk_preview.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3924 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow_sdk_preview.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow_sdk_preview.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      116 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow_sdk_preview.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/lusid_workflow_sdk_preview.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 21:24:12.000000 lusid-workflow-sdk-preview-0.1.973/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2237 2024-05-02 21:23:37.000000 lusid-workflow-sdk-preview-0.1.973/setup.py
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/README.md` & `lusid-workflow-sdk-preview-0.1.973/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-workflow-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.966
-- Package version: 0.1.966
+- API version: 0.1.973
+- Package version: 0.1.973
 - Build package: org.openapitools.codegen.languages.PythonLegacyClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/__init__.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.966"
+__version__ = "0.1.973"
 
 # import apis into sdk package
 from lusid_workflow.api.application_metadata_api import ApplicationMetadataApi
 from lusid_workflow.api.task_definitions_api import TaskDefinitionsApi
 from lusid_workflow.api.tasks_api import TasksApi
 from lusid_workflow.api.workers_api import WorkersApi
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/api/application_metadata_api.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api/application_metadata_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -141,15 +141,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.966'
+        header_params['X-LUSID-SDK-Version'] = '0.1.973'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfAccessControlledResource",
         }
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/api/task_definitions_api.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api/task_definitions_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -159,15 +159,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.966'
+        header_params['X-LUSID-SDK-Version'] = '0.1.973'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "TaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -328,15 +328,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.966'
+        header_params['X-LUSID-SDK-Version'] = '0.1.973'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -505,15 +505,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.966'
+        header_params['X-LUSID-SDK-Version'] = '0.1.973'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "TaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -681,15 +681,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.966'
+        header_params['X-LUSID-SDK-Version'] = '0.1.973'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfTaskDefinition",
             400: "LusidValidationProblemDetails",
@@ -858,15 +858,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.966'
+        header_params['X-LUSID-SDK-Version'] = '0.1.973'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "ResourceListOfTask",
             400: "LusidValidationProblemDetails",
@@ -1042,15 +1042,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.966'
+        header_params['X-LUSID-SDK-Version'] = '0.1.973'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "TaskDefinition",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/api/tasks_api.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api/tasks_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -173,15 +173,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.966'
+        header_params['X-LUSID-SDK-Version'] = '0.1.973'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Task",
             400: "LusidValidationProblemDetails",
@@ -323,15 +323,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.966'
+        header_params['X-LUSID-SDK-Version'] = '0.1.973'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -481,15 +481,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.966'
+        header_params['X-LUSID-SDK-Version'] = '0.1.973'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Task",
             400: "LusidValidationProblemDetails",
@@ -657,15 +657,15 @@
             ['application/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.966'
+        header_params['X-LUSID-SDK-Version'] = '0.1.973'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfTask",
             400: "LusidValidationProblemDetails",
@@ -833,15 +833,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.966'
+        header_params['X-LUSID-SDK-Version'] = '0.1.973'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Task",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/api/workers_api.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api/workers_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -163,15 +163,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.966'
+        header_params['X-LUSID-SDK-Version'] = '0.1.973'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Worker",
             400: "LusidValidationProblemDetails",
@@ -334,15 +334,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.966'
+        header_params['X-LUSID-SDK-Version'] = '0.1.973'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "DeletedEntityResponse",
             400: "LusidValidationProblemDetails",
@@ -513,15 +513,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.966'
+        header_params['X-LUSID-SDK-Version'] = '0.1.973'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             201: "Worker",
             400: "LusidValidationProblemDetails",
@@ -655,15 +655,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.966'
+        header_params['X-LUSID-SDK-Version'] = '0.1.973'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "GetWorkerResultResponse",
             400: "LusidValidationProblemDetails",
@@ -815,15 +815,15 @@
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         header_params['Accept-Encoding'] = "gzip, deflate, br"
 
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.966'
+        header_params['X-LUSID-SDK-Version'] = '0.1.973'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "PagedResourceListOfWorker",
             400: "LusidValidationProblemDetails",
@@ -1005,15 +1005,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.966'
+        header_params['X-LUSID-SDK-Version'] = '0.1.973'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "RunWorkerResponse",
             400: "LusidValidationProblemDetails",
@@ -1190,15 +1190,15 @@
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json-patch+json', 'application/json', 'text/json', 'application/*+json'])  # noqa: E501
 
         # set the LUSID header
         header_params['X-LUSID-SDK-Language'] = 'Python'
-        header_params['X-LUSID-SDK-Version'] = '0.1.966'
+        header_params['X-LUSID-SDK-Version'] = '0.1.973'
 
         # Authentication setting
         auth_settings = ['oauth2']  # noqa: E501
 
         response_types_map = {
             200: "Worker",
             400: "LusidValidationProblemDetails",
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/api_client.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 from __future__ import absolute_import
 
 import atexit
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.966/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.973/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/configuration.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
@@ -392,16 +392,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.966\n"\
-               "SDK Package Version: 0.1.966".\
+               "Version of the API: 0.1.973\n"\
+               "SDK Package Version: 0.1.973".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/exceptions.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 import six
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/__init__.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/access_controlled_action.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/access_controlled_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/access_controlled_resource.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/action_definition.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/action_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/action_definition_response.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/action_definition_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/action_details.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/action_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/action_details_response.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/action_details_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/action_id.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/action_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/create_child_task_configuration.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_child_task_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/create_child_tasks_action.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_child_tasks_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/create_child_tasks_action_response.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_child_tasks_action_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/create_task_definition_request.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_task_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/create_task_request.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_task_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/create_worker_request.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/create_worker_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/deleted_entity_response.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/deleted_entity_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/fail.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/fail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/fail_response.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/fail_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/field_mapping.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/field_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/get_worker_result_response.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/get_worker_result_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/health_check.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/health_check.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/health_check_response.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/health_check_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/id_selector_definition.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/id_selector_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/identifier_part_schema.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/identifier_part_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/initial_state.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/initial_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/link.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/link.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/luminesce_view.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/luminesce_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/luminesce_view_response.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/luminesce_view_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/lusid_problem_details.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/lusid_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/lusid_validation_problem_details.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/lusid_validation_problem_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/paged_resource_list_of_task.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/paged_resource_list_of_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/paged_resource_list_of_task_definition.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/paged_resource_list_of_task_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/paged_resource_list_of_worker.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/paged_resource_list_of_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/parameter.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/parameter_value.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/parameter_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/resource_id.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/resource_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/resource_list_of_access_controlled_resource.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/resource_list_of_access_controlled_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/resource_list_of_task.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/resource_list_of_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/result_field.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/result_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/result_matching_pattern.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/result_matching_pattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/resultant_child_task_configuration.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/resultant_child_task_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/run_worker_action.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/run_worker_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/run_worker_action_response.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/run_worker_action_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/run_worker_request.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/run_worker_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/run_worker_response.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/run_worker_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/scheduler_job.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/scheduler_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/scheduler_job_response.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/scheduler_job_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/sleep.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/sleep.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/sleep_response.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/sleep_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/stack.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/task.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/task_definition.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/task_definition_version.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_definition_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/task_field_definition.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_field_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/task_instance_field.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_instance_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/task_state_definition.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_state_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/task_summary.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/task_transition_definition.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/task_transition_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/transition_trigger_definition.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/transition_trigger_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/trigger_parent_task_action.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/trigger_parent_task_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/trigger_parent_task_action_response.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/trigger_parent_task_action_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/trigger_schema.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/trigger_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/update_task_definition_request.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/update_task_definition_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/update_task_request.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/update_task_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/update_worker_request.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/update_worker_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/version_info.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/version_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/worker.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/worker_configuration.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/worker_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/worker_configuration_response.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/worker_configuration_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/models/worker_status_triggers.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/models/worker_status_triggers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 try:
     from inspect import getfullargspec
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/rest.py` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     FINBOURNE Workflow API
 
     FINBOURNE Technology  # noqa: E501
 
-    The version of the OpenAPI document: 0.1.966
+    The version of the OpenAPI document: 0.1.973
     Contact: info@finbourne.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
```

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow/utilities/config_keys.json` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow/utilities/config_keys.json`

 * *Files identical despite different names*

### Comparing `lusid-workflow-sdk-preview-0.1.966/lusid_workflow_sdk_preview.egg-info/SOURCES.txt` & `lusid-workflow-sdk-preview-0.1.973/lusid_workflow_sdk_preview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lusid-workflow-sdk-preview-0.1.966/setup.py` & `lusid-workflow-sdk-preview-0.1.973/setup.py`

 * *Files identical despite different names*

