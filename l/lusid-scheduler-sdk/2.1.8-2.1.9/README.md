# Comparing `tmp/lusid_scheduler_sdk-2.1.8.tar.gz` & `tmp/lusid_scheduler_sdk-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_scheduler_sdk-2.1.8.tar", max compression
+gzip compressed data, was "lusid_scheduler_sdk-2.1.9.tar", max compression
```

## Comparing `lusid_scheduler_sdk-2.1.8.tar` & `lusid_scheduler_sdk-2.1.9.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0    11892 2024-04-18 11:44:40.028659 lusid_scheduler_sdk-2.1.8/README.md
--rw-r--r--   0        0        0     5616 2024-04-18 11:44:40.025659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/__init__.py
--rw-r--r--   0        0        0      385 2024-04-18 11:44:40.025659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/api/__init__.py
--rw-r--r--   0        0        0     7539 2024-04-18 11:44:40.025659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/api/application_metadata_api.py
--rw-r--r--   0        0        0    56274 2024-04-18 11:44:40.025659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/api/images_api.py
--rw-r--r--   0        0        0    78669 2024-04-18 11:44:40.025659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/api/jobs_api.py
--rw-r--r--   0        0        0    59919 2024-04-18 11:44:40.025659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/api/schedules_api.py
--rw-r--r--   0        0        0    30793 2024-04-18 11:44:40.025659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/api_client.py
--rw-r--r--   0        0        0      852 2024-04-18 11:44:40.025659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/api_response.py
--rw-r--r--   0        0        0    14458 2024-04-18 11:44:40.025659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/configuration.py
--rw-r--r--   0        0        0     5340 2024-04-18 11:44:40.025659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/exceptions.py
--rw-r--r--   0        0        0      590 2024-04-18 11:44:40.026659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/__init__.py
--rw-r--r--   0        0        0    30661 2024-04-18 11:44:40.026659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/api_client.py
--rw-r--r--   0        0        0     9872 2024-04-18 11:44:40.026659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8102 2024-04-18 11:44:40.026659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/api_configuration.py
--rw-r--r--   0        0        0     6800 2024-04-18 11:44:40.026659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-04-18 11:44:40.026659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-04-18 11:44:40.026659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12708 2024-04-18 11:44:40.026659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/rest.py
--rw-r--r--   0        0        0    11574 2024-04-18 11:44:40.026659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-04-18 11:44:40.026659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3887 2024-04-18 11:44:40.026659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     4194 2024-04-18 11:44:40.025659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/__init__.py
--rw-r--r--   0        0        0     3907 2024-04-18 11:44:40.023659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/access_controlled_action.py
--rw-r--r--   0        0        0     4850 2024-04-18 11:44:40.023659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/access_controlled_resource.py
--rw-r--r--   0        0        0     2071 2024-04-18 11:44:40.023659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/action_id.py
--rw-r--r--   0        0        0     3659 2024-04-18 11:44:40.023659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/argument_definition.py
--rw-r--r--   0        0        0     8580 2024-04-18 11:44:40.023659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/create_job_request.py
--rw-r--r--   0        0        0     7843 2024-04-18 11:44:40.023659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/create_schedule_request.py
--rw-r--r--   0        0        0     3182 2024-04-18 11:44:40.023659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/id_selector_definition.py
--rw-r--r--   0        0        0     3107 2024-04-18 11:44:40.023659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/identifier_part_schema.py
--rw-r--r--   0        0        0     4714 2024-04-18 11:44:40.023659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/image.py
--rw-r--r--   0        0        0     5517 2024-04-18 11:44:40.023659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/image_summary.py
--rw-r--r--   0        0        0     8238 2024-04-18 11:44:40.023659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/job_definition.py
--rw-r--r--   0        0        0     7923 2024-04-18 11:44:40.023659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/job_history.py
--rw-r--r--   0        0        0     8429 2024-04-18 11:44:40.023659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/job_run_result.py
--rw-r--r--   0        0        0     2263 2024-04-18 11:44:40.023659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/link.py
--rw-r--r--   0        0        0     3858 2024-04-18 11:44:40.023659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4694 2024-04-18 11:44:40.023659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     2946 2024-04-18 11:44:40.023659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/notification.py
--rw-r--r--   0        0        0     4310 2024-04-18 11:44:40.023659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/repository.py
--rw-r--r--   0        0        0     3194 2024-04-18 11:44:40.023659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/required_resources.py
--rw-r--r--   0        0        0     2626 2024-04-18 11:44:40.024659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/resource_id.py
--rw-r--r--   0        0        0     4258 2024-04-18 11:44:40.024659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     4113 2024-04-18 11:44:40.024659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/resource_list_of_image_summary.py
--rw-r--r--   0        0        0     4125 2024-04-18 11:44:40.024659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/resource_list_of_job_definition.py
--rw-r--r--   0        0        0     4089 2024-04-18 11:44:40.024659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/resource_list_of_job_history.py
--rw-r--r--   0        0        0     4088 2024-04-18 11:44:40.024659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/resource_list_of_repository.py
--rw-r--r--   0        0        0     4185 2024-04-18 11:44:40.024659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/resource_list_of_schedule_definition.py
--rw-r--r--   0        0        0     5115 2024-04-18 11:44:40.024659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/scan_report.py
--rw-r--r--   0        0        0     4633 2024-04-18 11:44:40.024659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/scan_summary.py
--rw-r--r--   0        0        0     6367 2024-04-18 11:44:40.024659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/schedule_definition.py
--rw-r--r--   0        0        0     3676 2024-04-18 11:44:40.024659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/start_job_request.py
--rw-r--r--   0        0        0     3267 2024-04-18 11:44:40.024659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/start_job_response.py
--rw-r--r--   0        0        0     3693 2024-04-18 11:44:40.024659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/start_schedule_response.py
--rw-r--r--   0        0        0     2707 2024-04-18 11:44:40.024659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/tag.py
--rw-r--r--   0        0        0     2610 2024-04-18 11:44:40.024659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/time_trigger.py
--rw-r--r--   0        0        0     2228 2024-04-18 11:44:40.024659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/trigger.py
--rw-r--r--   0        0        0     7977 2024-04-18 11:44:40.024659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/update_job_request.py
--rw-r--r--   0        0        0     7518 2024-04-18 11:44:40.025659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/update_schedule_request.py
--rw-r--r--   0        0        0     4012 2024-04-18 11:44:40.025659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/upload_image_instructions.py
--rw-r--r--   0        0        0     2480 2024-04-18 11:44:40.025659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/upload_image_request.py
--rw-r--r--   0        0        0     4396 2024-04-18 11:44:40.025659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/vulnerability.py
--rw-r--r--   0        0        0        0 2024-04-18 11:44:40.025659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/py.typed
--rw-r--r--   0        0        0    10162 2024-04-18 11:44:40.025659 lusid_scheduler_sdk-2.1.8/lusid_scheduler/rest.py
--rw-r--r--   0        0        0      862 2024-04-18 11:44:40.028659 lusid_scheduler_sdk-2.1.8/pyproject.toml
--rw-r--r--   0        0        0    12943 1970-01-01 00:00:00.000000 lusid_scheduler_sdk-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11892 2024-04-19 11:25:46.467164 lusid_scheduler_sdk-2.1.9/README.md
+-rw-r--r--   0        0        0     5616 2024-04-19 11:25:46.464164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/__init__.py
+-rw-r--r--   0        0        0      385 2024-04-19 11:25:46.462164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/api/__init__.py
+-rw-r--r--   0        0        0     7539 2024-04-19 11:25:46.461164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/api/application_metadata_api.py
+-rw-r--r--   0        0        0    56274 2024-04-19 11:25:46.461164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/api/images_api.py
+-rw-r--r--   0        0        0    78669 2024-04-19 11:25:46.461164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/api/jobs_api.py
+-rw-r--r--   0        0        0    59919 2024-04-19 11:25:46.462164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/api/schedules_api.py
+-rw-r--r--   0        0        0    30793 2024-04-19 11:25:46.464164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-19 11:25:46.464164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/api_response.py
+-rw-r--r--   0        0        0    14458 2024-04-19 11:25:46.464164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/configuration.py
+-rw-r--r--   0        0        0     5340 2024-04-19 11:25:46.464164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/exceptions.py
+-rw-r--r--   0        0        0      590 2024-04-19 11:25:46.465164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/__init__.py
+-rw-r--r--   0        0        0    30661 2024-04-19 11:25:46.465164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/api_client.py
+-rw-r--r--   0        0        0     9872 2024-04-19 11:25:46.465164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8102 2024-04-19 11:25:46.465164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6800 2024-04-19 11:25:46.465164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-04-19 11:25:46.465164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-04-19 11:25:46.465164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12708 2024-04-19 11:25:46.465164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/rest.py
+-rw-r--r--   0        0        0    11574 2024-04-19 11:25:46.465164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-04-19 11:25:46.465164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3887 2024-04-19 11:25:46.465164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     4194 2024-04-19 11:25:46.464164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/__init__.py
+-rw-r--r--   0        0        0     3907 2024-04-19 11:25:46.462164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4850 2024-04-19 11:25:46.462164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     2071 2024-04-19 11:25:46.462164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/action_id.py
+-rw-r--r--   0        0        0     3659 2024-04-19 11:25:46.462164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/argument_definition.py
+-rw-r--r--   0        0        0     8580 2024-04-19 11:25:46.462164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/create_job_request.py
+-rw-r--r--   0        0        0     7843 2024-04-19 11:25:46.462164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/create_schedule_request.py
+-rw-r--r--   0        0        0     3182 2024-04-19 11:25:46.462164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3107 2024-04-19 11:25:46.463164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     4714 2024-04-19 11:25:46.463164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/image.py
+-rw-r--r--   0        0        0     5517 2024-04-19 11:25:46.463164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/image_summary.py
+-rw-r--r--   0        0        0     8238 2024-04-19 11:25:46.463164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/job_definition.py
+-rw-r--r--   0        0        0     7923 2024-04-19 11:25:46.463164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/job_history.py
+-rw-r--r--   0        0        0     8429 2024-04-19 11:25:46.463164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/job_run_result.py
+-rw-r--r--   0        0        0     2263 2024-04-19 11:25:46.463164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/link.py
+-rw-r--r--   0        0        0     3858 2024-04-19 11:25:46.462164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4694 2024-04-19 11:25:46.463164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     2946 2024-04-19 11:25:46.463164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/notification.py
+-rw-r--r--   0        0        0     4310 2024-04-19 11:25:46.463164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/repository.py
+-rw-r--r--   0        0        0     3194 2024-04-19 11:25:46.463164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/required_resources.py
+-rw-r--r--   0        0        0     2626 2024-04-19 11:25:46.463164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/resource_id.py
+-rw-r--r--   0        0        0     4258 2024-04-19 11:25:46.463164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     4113 2024-04-19 11:25:46.463164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/resource_list_of_image_summary.py
+-rw-r--r--   0        0        0     4125 2024-04-19 11:25:46.463164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/resource_list_of_job_definition.py
+-rw-r--r--   0        0        0     4089 2024-04-19 11:25:46.463164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/resource_list_of_job_history.py
+-rw-r--r--   0        0        0     4088 2024-04-19 11:25:46.463164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/resource_list_of_repository.py
+-rw-r--r--   0        0        0     4185 2024-04-19 11:25:46.463164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/resource_list_of_schedule_definition.py
+-rw-r--r--   0        0        0     5115 2024-04-19 11:25:46.463164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/scan_report.py
+-rw-r--r--   0        0        0     4633 2024-04-19 11:25:46.464164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/scan_summary.py
+-rw-r--r--   0        0        0     6367 2024-04-19 11:25:46.464164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/schedule_definition.py
+-rw-r--r--   0        0        0     3676 2024-04-19 11:25:46.464164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/start_job_request.py
+-rw-r--r--   0        0        0     3267 2024-04-19 11:25:46.464164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/start_job_response.py
+-rw-r--r--   0        0        0     3693 2024-04-19 11:25:46.464164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/start_schedule_response.py
+-rw-r--r--   0        0        0     2707 2024-04-19 11:25:46.464164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/tag.py
+-rw-r--r--   0        0        0     2610 2024-04-19 11:25:46.464164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/time_trigger.py
+-rw-r--r--   0        0        0     2228 2024-04-19 11:25:46.464164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/trigger.py
+-rw-r--r--   0        0        0     7977 2024-04-19 11:25:46.464164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/update_job_request.py
+-rw-r--r--   0        0        0     7518 2024-04-19 11:25:46.464164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/update_schedule_request.py
+-rw-r--r--   0        0        0     4012 2024-04-19 11:25:46.464164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/upload_image_instructions.py
+-rw-r--r--   0        0        0     2480 2024-04-19 11:25:46.464164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/upload_image_request.py
+-rw-r--r--   0        0        0     4396 2024-04-19 11:25:46.464164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/vulnerability.py
+-rw-r--r--   0        0        0        0 2024-04-19 11:25:46.464164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/py.typed
+-rw-r--r--   0        0        0    10162 2024-04-19 11:25:46.465164 lusid_scheduler_sdk-2.1.9/lusid_scheduler/rest.py
+-rw-r--r--   0        0        0      862 2024-04-19 11:25:46.467164 lusid_scheduler_sdk-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0    12943 1970-01-01 00:00:00.000000 lusid_scheduler_sdk-2.1.9/PKG-INFO
```

### Comparing `lusid_scheduler_sdk-2.1.8/README.md` & `lusid_scheduler_sdk-2.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-scheduler-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.892
-- Package version: 2.1.8
+- API version: 0.0.893
+- Package version: 2.1.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/__init__.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/api/application_metadata_api.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/api/application_metadata_api.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/api/images_api.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/api/images_api.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/api/jobs_api.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/api/schedules_api.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/api/schedules_api.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/api_client.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/api_response.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/api_response.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/configuration.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("lusid_scheduler-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.0.892\n"\
+               "Version of the API: 0.0.893\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/exceptions.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/exceptions.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/__init__.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/api_client.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/api_client_factory.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/api_configuration.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/configuration_loaders.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/proxy_config.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/refreshing_token.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/rest.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/retry.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/socket_keep_alive.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/extensions/tcp_keep_alive_connector.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/__init__.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/access_controlled_action.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/access_controlled_action.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/access_controlled_resource.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/action_id.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/action_id.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/argument_definition.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/argument_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/create_job_request.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/create_job_request.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/create_schedule_request.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/create_schedule_request.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/id_selector_definition.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/id_selector_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/identifier_part_schema.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/identifier_part_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/image.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/image.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/image_summary.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/image_summary.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/job_definition.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/job_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/job_history.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/job_history.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/job_run_result.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/job_run_result.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/link.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/link.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/lusid_problem_details.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/lusid_validation_problem_details.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/notification.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/notification.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/repository.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/repository.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/required_resources.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/required_resources.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/resource_id.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/resource_id.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/resource_list_of_access_controlled_resource.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/resource_list_of_access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/resource_list_of_image_summary.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/resource_list_of_image_summary.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/resource_list_of_job_definition.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/resource_list_of_job_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/resource_list_of_job_history.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/resource_list_of_job_history.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/resource_list_of_repository.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/resource_list_of_repository.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/resource_list_of_schedule_definition.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/resource_list_of_schedule_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/scan_report.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/scan_report.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/scan_summary.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/scan_summary.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/schedule_definition.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/start_job_request.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/start_job_request.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/start_job_response.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/start_job_response.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/start_schedule_response.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/start_schedule_response.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/tag.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/tag.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/time_trigger.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/time_trigger.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/trigger.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/trigger.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/update_job_request.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/update_job_request.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/update_schedule_request.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/update_schedule_request.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/upload_image_instructions.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/upload_image_instructions.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/upload_image_request.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/upload_image_request.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/models/vulnerability.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/models/vulnerability.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/lusid_scheduler/rest.py` & `lusid_scheduler_sdk-2.1.9/lusid_scheduler/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_scheduler_sdk-2.1.8/pyproject.toml` & `lusid_scheduler_sdk-2.1.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lusid-scheduler-sdk"
-version = "2.1.8"
+version = "2.1.9"
 description = "FINBOURNE Scheduler API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/scheduler-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Scheduler API", "lusid-scheduler-sdk"]
 packages = [
```

### Comparing `lusid_scheduler_sdk-2.1.8/PKG-INFO` & `lusid_scheduler_sdk-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-scheduler-sdk
-Version: 2.1.8
+Version: 2.1.9
 Summary: FINBOURNE Scheduler API
 Home-page: https://github.com/finbourne/scheduler-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Scheduler API,lusid-scheduler-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # lusid-scheduler-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.892
-- Package version: 2.1.8
+- API version: 0.0.893
+- Package version: 2.1.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

