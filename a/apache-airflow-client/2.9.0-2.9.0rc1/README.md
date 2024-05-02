# Comparing `tmp/apache_airflow_client-2.9.0.tar.gz` & `tmp/apache_airflow_client-2.9.0rc1.tar.gz`

## Comparing `apache_airflow_client-2.9.0.tar` & `apache_airflow_client-2.9.0rc1.tar`

### file list

```diff
@@ -1,423 +1,423 @@
--rw-r--r--   0        0        0     1070 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/INSTALL
--rw-r--r--   0        0        0   169267 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/v1.yaml
--rw-r--r--   0        0        0        6 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/version.txt
--rw-r--r--   0        0        0        0 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/__init__.py
--rw-r--r--   0        0        0     8762 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/__init__.py
--rw-r--r--   0        0        0    45598 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/api_client.py
--rw-r--r--   0        0        0    24844 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/configuration.py
--rw-r--r--   0        0        0    13016 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/exceptions.py
--rw-r--r--   0        0        0    90037 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model_utils.py
--rw-r--r--   0        0        0    22147 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/rest.py
--rw-r--r--   0        0        0      224 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/api/__init__.py
--rw-r--r--   0        0        0    18392 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/api/config_api.py
--rw-r--r--   0        0        0    39418 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/api/connection_api.py
--rw-r--r--   0        0        0    69109 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/api/dag_api.py
--rw-r--r--   0        0        0    61107 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/api/dag_run_api.py
--rw-r--r--   0        0        0    14859 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/api/dag_warning_api.py
--rw-r--r--   0        0        0    67803 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/api/dataset_api.py
--rw-r--r--   0        0        0    21612 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/api/event_log_api.py
--rw-r--r--   0        0        0    19120 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/api/import_error_api.py
--rw-r--r--   0        0        0    17605 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/api/monitoring_api.py
--rw-r--r--   0        0        0    14086 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/api/permission_api.py
--rw-r--r--   0        0        0    13994 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/api/plugin_api.py
--rw-r--r--   0        0        0    33352 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/api/pool_api.py
--rw-r--r--   0        0        0    13444 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/api/provider_api.py
--rw-r--r--   0        0        0    34061 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/api/role_api.py
--rw-r--r--   0        0        0    86359 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/api/task_instance_api.py
--rw-r--r--   0        0        0    34364 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/api/user_api.py
--rw-r--r--   0        0        0    33950 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/api/variable_api.py
--rw-r--r--   0        0        0    22559 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/api/x_com_api.py
--rw-r--r--   0        0        0     1525 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/apis/__init__.py
--rw-r--r--   0        0        0      348 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/__init__.py
--rw-r--r--   0        0        0    19035 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/action.py
--rw-r--r--   0        0        0    21919 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/action_collection.py
--rw-r--r--   0        0        0    19187 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/action_collection_all_of.py
--rw-r--r--   0        0        0    19467 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/action_resource.py
--rw-r--r--   0        0        0    22061 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/basic_dag_run.py
--rw-r--r--   0        0        0    19297 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/class_reference.py
--rw-r--r--   0        0        0    19400 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/clear_dag_run.py
--rw-r--r--   0        0        0    24350 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/clear_task_instances.py
--rw-r--r--   0        0        0    19244 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/collection_info.py
--rw-r--r--   0        0        0    19464 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/color.py
--rw-r--r--   0        0        0    19197 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/config.py
--rw-r--r--   0        0        0    19213 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/config_option.py
--rw-r--r--   0        0        0    19414 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/config_section.py
--rw-r--r--   0        0        0    23682 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/connection.py
--rw-r--r--   0        0        0    19414 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/connection_all_of.py
--rw-r--r--   0        0        0    22099 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/connection_collection.py
--rw-r--r--   0        0        0    19347 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/connection_collection_all_of.py
--rw-r--r--   0        0        0    20726 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/connection_collection_item.py
--rw-r--r--   0        0        0    19339 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/connection_test.py
--rw-r--r--   0        0        0    19622 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/create_dataset_event.py
--rw-r--r--   0        0        0    19225 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/cron_expression.py
--rw-r--r--   0        0        0    30855 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/dag.py
--rw-r--r--   0        0        0    21859 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/dag_collection.py
--rw-r--r--   0        0        0    19142 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/dag_collection_all_of.py
--rw-r--r--   0        0        0    38352 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/dag_detail.py
--rw-r--r--   0        0        0    24562 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/dag_detail_all_of.py
--rw-r--r--   0        0        0    19707 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/dag_processor_status.py
--rw-r--r--   0        0        0    26254 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/dag_run.py
--rw-r--r--   0        0        0    21926 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/dag_run_collection.py
--rw-r--r--   0        0        0    19193 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/dag_run_collection_all_of.py
--rw-r--r--   0        0        0    19705 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/dag_schedule_dataset_reference.py
--rw-r--r--   0        0        0    19977 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/dag_state.py
--rw-r--r--   0        0        0    19983 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/dag_warning.py
--rw-r--r--   0        0        0    22011 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/dag_warning_collection.py
--rw-r--r--   0        0        0    19258 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/dag_warning_collection_all_of.py
--rw-r--r--   0        0        0    21191 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/dataset.py
--rw-r--r--   0        0        0    21939 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/dataset_collection.py
--rw-r--r--   0        0        0    19202 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/dataset_collection_all_of.py
--rw-r--r--   0        0        0    21845 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/dataset_event.py
--rw-r--r--   0        0        0    22046 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/dataset_event_collection.py
--rw-r--r--   0        0        0    19283 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/dataset_event_collection_all_of.py
--rw-r--r--   0        0        0    20851 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/error.py
--rw-r--r--   0        0        0    21760 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/event_log.py
--rw-r--r--   0        0        0    21966 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/event_log_collection.py
--rw-r--r--   0        0        0    19223 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/event_log_collection_all_of.py
--rw-r--r--   0        0        0    19628 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/extra_link.py
--rw-r--r--   0        0        0    19223 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/extra_link_collection.py
--rw-r--r--   0        0        0    20401 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/health_info.py
--rw-r--r--   0        0        0    19602 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/health_status.py
--rw-r--r--   0        0        0    19986 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/import_error.py
--rw-r--r--   0        0        0    22026 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/import_error_collection.py
--rw-r--r--   0        0        0    19268 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/import_error_collection_all_of.py
--rw-r--r--   0        0        0    19005 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/inline_response200.py
--rw-r--r--   0        0        0    19256 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/inline_response2001.py
--rw-r--r--   0        0        0    21071 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/job.py
--rw-r--r--   0        0        0    24213 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/list_dag_runs_form.py
--rw-r--r--   0        0        0    25771 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/list_task_instance_form.py
--rw-r--r--   0        0        0    19210 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/metadatabase_status.py
--rw-r--r--   0        0        0    22019 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/plugin_collection.py
--rw-r--r--   0        0        0    19287 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/plugin_collection_all_of.py
--rw-r--r--   0        0        0    23048 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/plugin_collection_item.py
--rw-r--r--   0        0        0    22705 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/pool.py
--rw-r--r--   0        0        0    21879 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/pool_collection.py
--rw-r--r--   0        0        0    19157 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/pool_collection_all_of.py
--rw-r--r--   0        0        0    19607 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/provider.py
--rw-r--r--   0        0        0    19202 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/provider_collection.py
--rw-r--r--   0        0        0    19506 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/queued_event.py
--rw-r--r--   0        0        0    22001 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/queued_event_collection.py
--rw-r--r--   0        0        0    19243 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/queued_event_collection_all_of.py
--rw-r--r--   0        0        0    22235 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/relative_delta.py
--rw-r--r--   0        0        0    19015 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/resource.py
--rw-r--r--   0        0        0    19670 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/role.py
--rw-r--r--   0        0        0    21879 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/role_collection.py
--rw-r--r--   0        0        0    19157 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/role_collection_all_of.py
--rw-r--r--   0        0        0    24639 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/schedule_interval.py
--rw-r--r--   0        0        0    19666 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/scheduler_status.py
--rw-r--r--   0        0        0    19070 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/set_dag_run_note.py
--rw-r--r--   0        0        0    19132 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/set_task_instance_note.py
--rw-r--r--   0        0        0    20383 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/sla_miss.py
--rw-r--r--   0        0        0    18948 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/tag.py
--rw-r--r--   0        0        0    25902 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/task.py
--rw-r--r--   0        0        0    19142 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/task_collection.py
--rw-r--r--   0        0        0    19227 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/task_extra_links.py
--rw-r--r--   0        0        0    26592 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/task_instance.py
--rw-r--r--   0        0        0    22046 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/task_instance_collection.py
--rw-r--r--   0        0        0    19283 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/task_instance_collection_all_of.py
--rw-r--r--   0        0        0    19870 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/task_instance_reference.py
--rw-r--r--   0        0        0    19359 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/task_instance_reference_collection.py
--rw-r--r--   0        0        0    19960 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/task_outlet_dataset_reference.py
--rw-r--r--   0        0        0    22519 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/task_state.py
--rw-r--r--   0        0        0    19700 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/time_delta.py
--rw-r--r--   0        0        0    19809 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/trigger.py
--rw-r--r--   0        0        0    22530 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/trigger_rule.py
--rw-r--r--   0        0        0    19666 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/triggerer_status.py
--rw-r--r--   0        0        0    19186 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/update_dag_run_state.py
--rw-r--r--   0        0        0    19851 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/update_task_instance.py
--rw-r--r--   0        0        0    22282 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/update_task_instances_state.py
--rw-r--r--   0        0        0    20322 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/update_task_state.py
--rw-r--r--   0        0        0    25698 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/user.py
--rw-r--r--   0        0        0    18986 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/user_all_of.py
--rw-r--r--   0        0        0    21979 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/user_collection.py
--rw-r--r--   0        0        0    19257 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/user_collection_all_of.py
--rw-r--r--   0        0        0    23276 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/user_collection_item.py
--rw-r--r--   0        0        0    19007 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/user_collection_item_roles.py
--rw-r--r--   0        0        0    21875 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/variable.py
--rw-r--r--   0        0        0    18983 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/variable_all_of.py
--rw-r--r--   0        0        0    22059 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/variable_collection.py
--rw-r--r--   0        0        0    19317 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/variable_collection_all_of.py
--rw-r--r--   0        0        0    19364 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/variable_collection_item.py
--rw-r--r--   0        0        0    19371 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/version_info.py
--rw-r--r--   0        0        0    19663 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/weight_rule.py
--rw-r--r--   0        0        0    22498 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/x_com.py
--rw-r--r--   0        0        0    18993 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/x_com_all_of.py
--rw-r--r--   0        0        0    22016 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/x_com_collection.py
--rw-r--r--   0        0        0    19293 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/x_com_collection_all_of.py
--rw-r--r--   0        0        0    20003 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/model/x_com_collection_item.py
--rw-r--r--   0        0        0     8907 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/airflow_client/client/models/__init__.py
--rw-r--r--   0        0        0      578 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/Action.md
--rw-r--r--   0        0        0      723 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ActionCollection.md
--rw-r--r--   0        0        0      526 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ActionCollectionAllOf.md
--rw-r--r--   0        0        0      599 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ActionResource.md
--rw-r--r--   0        0        0     1446 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/BasicDAGRun.md
--rw-r--r--   0        0        0      585 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ClassReference.md
--rw-r--r--   0        0        0      706 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ClearDagRun.md
--rw-r--r--   0        0        0     2250 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ClearTaskInstances.md
--rw-r--r--   0        0        0      641 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/CollectionInfo.md
--rw-r--r--   0        0        0      371 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/Color.md
--rw-r--r--   0        0        0      545 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/Config.md
--rw-r--r--   0        0        0     5517 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ConfigApi.md
--rw-r--r--   0        0        0      583 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ConfigOption.md
--rw-r--r--   0        0        0      607 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ConfigSection.md
--rw-r--r--   0        0        0     1176 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/Connection.md
--rw-r--r--   0        0        0      644 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ConnectionAllOf.md
--rw-r--r--   0        0        0    18687 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ConnectionApi.md
--rw-r--r--   0        0        0      810 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ConnectionCollection.md
--rw-r--r--   0        0        0      570 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ConnectionCollectionAllOf.md
--rw-r--r--   0        0        0     1117 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ConnectionCollectionItem.md
--rw-r--r--   0        0        0      662 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ConnectionTest.md
--rw-r--r--   0        0        0      657 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/CreateDatasetEvent.md
--rw-r--r--   0        0        0      529 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/CronExpression.md
--rw-r--r--   0        0        0     4174 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DAG.md
--rw-r--r--   0        0        0    38591 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DAGApi.md
--rw-r--r--   0        0        0      747 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DAGCollection.md
--rw-r--r--   0        0        0      514 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DAGCollectionAllOf.md
--rw-r--r--   0        0        0     5786 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DAGDetail.md
--rw-r--r--   0        0        0     2037 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DAGDetailAllOf.md
--rw-r--r--   0        0        0     2986 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DAGRun.md
--rw-r--r--   0        0        0    33346 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DAGRunApi.md
--rw-r--r--   0        0        0      764 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DAGRunCollection.md
--rw-r--r--   0        0        0      527 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DAGRunCollectionAllOf.md
--rw-r--r--   0        0        0      740 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DagProcessorStatus.md
--rw-r--r--   0        0        0      782 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DagScheduleDatasetReference.md
--rw-r--r--   0        0        0      552 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DagState.md
--rw-r--r--   0        0        0      782 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DagWarning.md
--rw-r--r--   0        0        0     3987 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DagWarningApi.md
--rw-r--r--   0        0        0      720 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DagWarningCollection.md
--rw-r--r--   0        0        0      544 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DagWarningCollectionAllOf.md
--rw-r--r--   0        0        0     1068 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/Dataset.md
--rw-r--r--   0        0        0    37997 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DatasetApi.md
--rw-r--r--   0        0        0      728 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DatasetCollection.md
--rw-r--r--   0        0        0      530 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DatasetCollectionAllOf.md
--rw-r--r--   0        0        0     1292 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DatasetEvent.md
--rw-r--r--   0        0        0      755 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DatasetEventCollection.md
--rw-r--r--   0        0        0      551 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/DatasetEventCollectionAllOf.md
--rw-r--r--   0        0        0     1197 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/Error.md
--rw-r--r--   0        0        0     1366 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/EventLog.md
--rw-r--r--   0        0        0     8308 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/EventLogApi.md
--rw-r--r--   0        0        0      774 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/EventLogCollection.md
--rw-r--r--   0        0        0      535 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/EventLogCollectionAllOf.md
--rw-r--r--   0        0        0      691 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ExtraLink.md
--rw-r--r--   0        0        0      565 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ExtraLinkCollection.md
--rw-r--r--   0        0        0      806 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/HealthInfo.md
--rw-r--r--   0        0        0      386 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/HealthStatus.md
--rw-r--r--   0        0        0      765 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ImportError.md
--rw-r--r--   0        0        0     6265 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ImportErrorApi.md
--rw-r--r--   0        0        0      789 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ImportErrorCollection.md
--rw-r--r--   0        0        0      547 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ImportErrorCollectionAllOf.md
--rw-r--r--   0        0        0      504 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/InlineResponse200.md
--rw-r--r--   0        0        0      555 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/InlineResponse2001.md
--rw-r--r--   0        0        0      955 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/Job.md
--rw-r--r--   0        0        0     2351 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ListDagRunsForm.md
--rw-r--r--   0        0        0     2935 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ListTaskInstanceForm.md
--rw-r--r--   0        0        0      564 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/MetadatabaseStatus.md
--rw-r--r--   0        0        0     4655 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/MonitoringApi.md
--rw-r--r--   0        0        0     3281 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/PermissionApi.md
--rw-r--r--   0        0        0     3241 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/PluginApi.md
--rw-r--r--   0        0        0      750 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/PluginCollection.md
--rw-r--r--   0        0        0      554 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/PluginCollectionAllOf.md
--rw-r--r--   0        0        0     1624 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/PluginCollectionItem.md
--rw-r--r--   0        0        0     1725 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/Pool.md
--rw-r--r--   0        0        0    14692 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/PoolApi.md
--rw-r--r--   0        0        0      752 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/PoolCollection.md
--rw-r--r--   0        0        0      518 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/PoolCollectionAllOf.md
--rw-r--r--   0        0        0      713 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/Provider.md
--rw-r--r--   0        0        0     2748 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ProviderApi.md
--rw-r--r--   0        0        0      579 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ProviderCollection.md
--rw-r--r--   0        0        0      637 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/QueuedEvent.md
--rw-r--r--   0        0        0      754 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/QueuedEventCollection.md
--rw-r--r--   0        0        0      542 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/QueuedEventCollectionAllOf.md
--rw-r--r--   0        0        0      909 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/RelativeDelta.md
--rw-r--r--   0        0        0      586 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/Resource.md
--rw-r--r--   0        0        0      728 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/Role.md
--rw-r--r--   0        0        0    15554 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/RoleApi.md
--rw-r--r--   0        0        0      713 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/RoleCollection.md
--rw-r--r--   0        0        0      518 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/RoleCollectionAllOf.md
--rw-r--r--   0        0        0      800 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/SLAMiss.md
--rw-r--r--   0        0        0     1249 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/ScheduleInterval.md
--rw-r--r--   0        0        0      700 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/SchedulerStatus.md
--rw-r--r--   0        0        0      541 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/SetDagRunNote.md
--rw-r--r--   0        0        0      538 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/SetTaskInstanceNote.md
--rw-r--r--   0        0        0      491 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/Tag.md
--rw-r--r--   0        0        0     2170 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/Task.md
--rw-r--r--   0        0        0      534 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/TaskCollection.md
--rw-r--r--   0        0        0      535 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/TaskExtraLinks.md
--rw-r--r--   0        0        0     2373 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/TaskInstance.md
--rw-r--r--   0        0        0    52613 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/TaskInstanceApi.md
--rw-r--r--   0        0        0      794 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/TaskInstanceCollection.md
--rw-r--r--   0        0        0      551 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/TaskInstanceCollectionAllOf.md
--rw-r--r--   0        0        0      716 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/TaskInstanceReference.md
--rw-r--r--   0        0        0      573 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/TaskInstanceReferenceCollection.md
--rw-r--r--   0        0        0      845 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/TaskOutletDatasetReference.md
--rw-r--r--   0        0        0     1536 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/TaskState.md
--rw-r--r--   0        0        0      579 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/TimeDelta.md
--rw-r--r--   0        0        0      667 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/Trigger.md
--rw-r--r--   0        0        0     1443 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/TriggerRule.md
--rw-r--r--   0        0        0      725 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/TriggererStatus.md
--rw-r--r--   0        0        0      586 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/UpdateDagRunState.md
--rw-r--r--   0        0        0      791 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/UpdateTaskInstance.md
--rw-r--r--   0        0        0     1526 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/UpdateTaskInstancesState.md
--rw-r--r--   0        0        0      735 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/UpdateTaskState.md
--rw-r--r--   0        0        0     1903 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/User.md
--rw-r--r--   0        0        0      497 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/UserAllOf.md
--rw-r--r--   0        0        0    15526 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/UserApi.md
--rw-r--r--   0        0        0      739 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/UserCollection.md
--rw-r--r--   0        0        0      546 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/UserCollectionAllOf.md
--rw-r--r--   0        0        0     1857 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/UserCollectionItem.md
--rw-r--r--   0        0        0      507 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/UserCollectionItemRoles.md
--rw-r--r--   0        0        0      671 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/Variable.md
--rw-r--r--   0        0        0      498 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/VariableAllOf.md
--rw-r--r--   0        0        0    15059 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/VariableApi.md
--rw-r--r--   0        0        0      800 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/VariableCollection.md
--rw-r--r--   0        0        0      562 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/VariableCollectionAllOf.md
--rw-r--r--   0        0        0      748 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/VariableCollectionItem.md
--rw-r--r--   0        0        0      638 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/VersionInfo.md
--rw-r--r--   0        0        0      396 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/WeightRule.md
--rw-r--r--   0        0        0      774 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/XCom.md
--rw-r--r--   0        0        0      503 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/XComAllOf.md
--rw-r--r--   0        0        0     9154 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/XComApi.md
--rw-r--r--   0        0        0      794 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/XComCollection.md
--rw-r--r--   0        0        0      553 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/XComCollectionAllOf.md
--rw-r--r--   0        0        0      829 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/docs/XComCollectionItem.md
--rw-r--r--   0        0        0        0 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/__init__.py
--rw-r--r--   0        0        0     8665 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_action.py
--rw-r--r--   0        0        0     9081 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_action_collection.py
--rw-r--r--   0        0        0     8856 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_action_collection_all_of.py
--rw-r--r--   0        0        0     8896 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_action_resource.py
--rw-r--r--   0        0        0     8794 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_basic_dag_run.py
--rw-r--r--   0        0        0     8722 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_class_reference.py
--rw-r--r--   0        0        0     8702 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_clear_dag_run.py
--rw-r--r--   0        0        0     8751 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_clear_task_instances.py
--rw-r--r--   0        0        0     8722 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_collection_info.py
--rw-r--r--   0        0        0     8658 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_color.py
--rw-r--r--   0        0        0     8777 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_config.py
--rw-r--r--   0        0        0     8812 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_config_api.py
--rw-r--r--   0        0        0     8708 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_config_option.py
--rw-r--r--   0        0        0     8823 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_config_section.py
--rw-r--r--   0        0        0     8971 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_connection.py
--rw-r--r--   0        0        0     8730 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_connection_all_of.py
--rw-r--r--   0        0        0     9416 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_connection_api.py
--rw-r--r--   0        0        0     9199 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_connection_collection.py
--rw-r--r--   0        0        0     8958 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_connection_collection_all_of.py
--rw-r--r--   0        0        0     8793 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_connection_collection_item.py
--rw-r--r--   0        0        0     8722 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_connection_test.py
--rw-r--r--   0        0        0     8751 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_create_dataset_event.py
--rw-r--r--   0        0        0     8722 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_cron_expression.py
--rw-r--r--   0        0        0     8839 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dag.py
--rw-r--r--   0        0        0    10110 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dag_api.py
--rw-r--r--   0        0        0     9036 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dag_collection.py
--rw-r--r--   0        0        0     8823 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dag_collection_all_of.py
--rw-r--r--   0        0        0     9167 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dag_detail.py
--rw-r--r--   0        0        0     8820 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dag_detail_all_of.py
--rw-r--r--   0        0        0     8859 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dag_processor_status.py
--rw-r--r--   0        0        0     8758 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dag_run.py
--rw-r--r--   0        0        0     9855 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dag_run_api.py
--rw-r--r--   0        0        0     9084 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dag_run_collection.py
--rw-r--r--   0        0        0     8858 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dag_run_collection_all_of.py
--rw-r--r--   0        0        0     8815 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dag_schedule_dataset_reference.py
--rw-r--r--   0        0        0     8680 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dag_state.py
--rw-r--r--   0        0        0     8694 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dag_warning.py
--rw-r--r--   0        0        0     8691 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dag_warning_api.py
--rw-r--r--   0        0        0     9144 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dag_warning_collection.py
--rw-r--r--   0        0        0     8902 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dag_warning_collection_all_of.py
--rw-r--r--   0        0        0     9008 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dataset.py
--rw-r--r--   0        0        0    10448 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dataset_api.py
--rw-r--r--   0        0        0     9096 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dataset_collection.py
--rw-r--r--   0        0        0     8867 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dataset_collection_all_of.py
--rw-r--r--   0        0        0     8813 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dataset_event.py
--rw-r--r--   0        0        0     9174 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dataset_event_collection.py
--rw-r--r--   0        0        0     8924 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_dataset_event_collection_all_of.py
--rw-r--r--   0        0        0     8658 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_error.py
--rw-r--r--   0        0        0     8680 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_event_log.py
--rw-r--r--   0        0        0     8814 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_event_log_api.py
--rw-r--r--   0        0        0     9114 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_event_log_collection.py
--rw-r--r--   0        0        0     8880 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_event_log_collection_all_of.py
--rw-r--r--   0        0        0     8803 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_extra_link.py
--rw-r--r--   0        0        0     8854 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_extra_link_collection.py
--rw-r--r--   0        0        0     9199 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_health_info.py
--rw-r--r--   0        0        0     8708 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_health_status.py
--rw-r--r--   0        0        0     8701 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_import_error.py
--rw-r--r--   0        0        0     8847 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_import_error_api.py
--rw-r--r--   0        0        0     9159 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_import_error_collection.py
--rw-r--r--   0        0        0     8913 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_import_error_collection_all_of.py
--rw-r--r--   0        0        0     8743 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_inline_response200.py
--rw-r--r--   0        0        0     8750 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_inline_response2001.py
--rw-r--r--   0        0        0     8644 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_job.py
--rw-r--r--   0        0        0     8731 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_list_dag_runs_form.py
--rw-r--r--   0        0        0     8862 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_list_task_instance_form.py
--rw-r--r--   0        0        0     8858 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_metadatabase_status.py
--rw-r--r--   0        0        0     8822 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_monitoring_api.py
--rw-r--r--   0        0        0     8687 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_permission_api.py
--rw-r--r--   0        0        0     8671 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_plugin_api.py
--rw-r--r--   0        0        0     9139 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_plugin_collection.py
--rw-r--r--   0        0        0     8914 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_plugin_collection_all_of.py
--rw-r--r--   0        0        0     8765 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_plugin_collection_item.py
--rw-r--r--   0        0        0     8651 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_pool.py
--rw-r--r--   0        0        0     9152 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_pool_api.py
--rw-r--r--   0        0        0     9051 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_pool_collection.py
--rw-r--r--   0        0        0     8834 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_pool_collection_all_of.py
--rw-r--r--   0        0        0     8679 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_provider.py
--rw-r--r--   0        0        0     8671 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_provider_api.py
--rw-r--r--   0        0        0     8841 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_provider_collection.py
--rw-r--r--   0        0        0     8701 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_queued_event.py
--rw-r--r--   0        0        0     9159 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_queued_event_collection.py
--rw-r--r--   0        0        0     8913 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_queued_event_collection_all_of.py
--rw-r--r--   0        0        0     8715 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_relative_delta.py
--rw-r--r--   0        0        0     8679 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_resource.py
--rw-r--r--   0        0        0     8767 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_role.py
--rw-r--r--   0        0        0     9152 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_role_api.py
--rw-r--r--   0        0        0     9051 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_role_collection.py
--rw-r--r--   0        0        0     8834 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_role_collection_all_of.py
--rw-r--r--   0        0        0     9060 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_schedule_interval.py
--rw-r--r--   0        0        0     8837 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_scheduler_status.py
--rw-r--r--   0        0        0     8717 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_set_dag_run_note.py
--rw-r--r--   0        0        0     8759 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_set_task_instance_note.py
--rw-r--r--   0        0        0     8673 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_sla_miss.py
--rw-r--r--   0        0        0     8644 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_tag.py
--rw-r--r--   0        0        0     9334 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_task.py
--rw-r--r--   0        0        0     8797 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_task_collection.py
--rw-r--r--   0        0        0     8839 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_task_extra_links.py
--rw-r--r--   0        0        0     9050 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_task_instance.py
--rw-r--r--   0        0        0    10352 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_task_instance_api.py
--rw-r--r--   0        0        0     9174 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_task_instance_collection.py
--rw-r--r--   0        0        0     8924 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_task_instance_collection_all_of.py
--rw-r--r--   0        0        0     8772 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_task_instance_reference.py
--rw-r--r--   0        0        0     8988 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_task_instance_reference_collection.py
--rw-r--r--   0        0        0     8808 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_task_outlet_dataset_reference.py
--rw-r--r--   0        0        0     8687 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_task_state.py
--rw-r--r--   0        0        0     8687 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_time_delta.py
--rw-r--r--   0        0        0     8672 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_trigger.py
--rw-r--r--   0        0        0     8701 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_trigger_rule.py
--rw-r--r--   0        0        0     8837 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_triggerer_status.py
--rw-r--r--   0        0        0     8745 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_update_dag_run_state.py
--rw-r--r--   0        0        0     8872 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_update_task_instance.py
--rw-r--r--   0        0        0     8915 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_update_task_instances_state.py
--rw-r--r--   0        0        0     8730 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_update_task_state.py
--rw-r--r--   0        0        0     9035 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_user.py
--rw-r--r--   0        0        0     8688 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_user_all_of.py
--rw-r--r--   0        0        0     9152 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_user_api.py
--rw-r--r--   0        0        0     9109 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_user_collection.py
--rw-r--r--   0        0        0     8892 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_user_collection_all_of.py
--rw-r--r--   0        0        0     8905 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_user_collection_item.py
--rw-r--r--   0        0        0     8787 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_user_collection_item_roles.py
--rw-r--r--   0        0        0     8941 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_variable.py
--rw-r--r--   0        0        0     8716 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_variable_all_of.py
--rw-r--r--   0        0        0     9234 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_variable_api.py
--rw-r--r--   0        0        0     9169 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_variable_collection.py
--rw-r--r--   0        0        0     8936 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_variable_collection_all_of.py
--rw-r--r--   0        0        0     8779 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_variable_collection_item.py
--rw-r--r--   0        0        0     8701 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_version_info.py
--rw-r--r--   0        0        0     8694 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_weight_rule.py
--rw-r--r--   0        0        0     8884 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_x_com.py
--rw-r--r--   0        0        0     8689 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_x_com_all_of.py
--rw-r--r--   0        0        0     8803 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_x_com_api.py
--rw-r--r--   0        0        0     9112 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_x_com_collection.py
--rw-r--r--   0        0        0     8894 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_x_com_collection_all_of.py
--rw-r--r--   0        0        0     8752 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/test/test_x_com_collection_item.py
--rw-r--r--   0        0        0       99 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/.gitignore
--rw-r--r--   0        0        0    13569 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/LICENSE
--rw-r--r--   0        0        0        0 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/NOTICE
--rw-r--r--   0        0        0    29440 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/README.md
--rw-r--r--   0        0        0     3273 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/pyproject.toml
--rw-r--r--   0        0        0    30909 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/INSTALL
+-rw-r--r--   0        0        0   169267 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/v1.yaml
+-rw-r--r--   0        0        0        8 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/version.txt
+-rw-r--r--   0        0        0        0 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/__init__.py
+-rw-r--r--   0        0        0     8765 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/__init__.py
+-rw-r--r--   0        0        0    45601 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/api_client.py
+-rw-r--r--   0        0        0    24847 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/configuration.py
+-rw-r--r--   0        0        0    13016 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/exceptions.py
+-rw-r--r--   0        0        0    90037 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model_utils.py
+-rw-r--r--   0        0        0    22147 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/rest.py
+-rw-r--r--   0        0        0      224 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/api/__init__.py
+-rw-r--r--   0        0        0    18392 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/api/config_api.py
+-rw-r--r--   0        0        0    39418 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/api/connection_api.py
+-rw-r--r--   0        0        0    69109 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/api/dag_api.py
+-rw-r--r--   0        0        0    61107 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/api/dag_run_api.py
+-rw-r--r--   0        0        0    14859 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/api/dag_warning_api.py
+-rw-r--r--   0        0        0    67803 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/api/dataset_api.py
+-rw-r--r--   0        0        0    21612 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/api/event_log_api.py
+-rw-r--r--   0        0        0    19120 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/api/import_error_api.py
+-rw-r--r--   0        0        0    17605 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/api/monitoring_api.py
+-rw-r--r--   0        0        0    14086 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/api/permission_api.py
+-rw-r--r--   0        0        0    13994 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/api/plugin_api.py
+-rw-r--r--   0        0        0    33352 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/api/pool_api.py
+-rw-r--r--   0        0        0    13444 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/api/provider_api.py
+-rw-r--r--   0        0        0    34061 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/api/role_api.py
+-rw-r--r--   0        0        0    86359 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/api/task_instance_api.py
+-rw-r--r--   0        0        0    34364 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/api/user_api.py
+-rw-r--r--   0        0        0    33950 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/api/variable_api.py
+-rw-r--r--   0        0        0    22559 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/api/x_com_api.py
+-rw-r--r--   0        0        0     1525 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/apis/__init__.py
+-rw-r--r--   0        0        0      348 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/__init__.py
+-rw-r--r--   0        0        0    19035 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/action.py
+-rw-r--r--   0        0        0    21919 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/action_collection.py
+-rw-r--r--   0        0        0    19187 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/action_collection_all_of.py
+-rw-r--r--   0        0        0    19467 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/action_resource.py
+-rw-r--r--   0        0        0    22061 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/basic_dag_run.py
+-rw-r--r--   0        0        0    19297 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/class_reference.py
+-rw-r--r--   0        0        0    19400 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/clear_dag_run.py
+-rw-r--r--   0        0        0    24350 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/clear_task_instances.py
+-rw-r--r--   0        0        0    19244 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/collection_info.py
+-rw-r--r--   0        0        0    19464 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/color.py
+-rw-r--r--   0        0        0    19197 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/config.py
+-rw-r--r--   0        0        0    19213 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/config_option.py
+-rw-r--r--   0        0        0    19414 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/config_section.py
+-rw-r--r--   0        0        0    23682 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/connection.py
+-rw-r--r--   0        0        0    19414 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/connection_all_of.py
+-rw-r--r--   0        0        0    22099 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/connection_collection.py
+-rw-r--r--   0        0        0    19347 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/connection_collection_all_of.py
+-rw-r--r--   0        0        0    20726 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/connection_collection_item.py
+-rw-r--r--   0        0        0    19339 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/connection_test.py
+-rw-r--r--   0        0        0    19622 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/create_dataset_event.py
+-rw-r--r--   0        0        0    19225 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/cron_expression.py
+-rw-r--r--   0        0        0    30855 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag.py
+-rw-r--r--   0        0        0    21859 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_collection.py
+-rw-r--r--   0        0        0    19142 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_collection_all_of.py
+-rw-r--r--   0        0        0    38352 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_detail.py
+-rw-r--r--   0        0        0    24562 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_detail_all_of.py
+-rw-r--r--   0        0        0    19707 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_processor_status.py
+-rw-r--r--   0        0        0    26254 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_run.py
+-rw-r--r--   0        0        0    21926 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_run_collection.py
+-rw-r--r--   0        0        0    19193 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_run_collection_all_of.py
+-rw-r--r--   0        0        0    19705 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_schedule_dataset_reference.py
+-rw-r--r--   0        0        0    19977 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_state.py
+-rw-r--r--   0        0        0    19983 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_warning.py
+-rw-r--r--   0        0        0    22011 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_warning_collection.py
+-rw-r--r--   0        0        0    19258 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_warning_collection_all_of.py
+-rw-r--r--   0        0        0    21191 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/dataset.py
+-rw-r--r--   0        0        0    21939 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/dataset_collection.py
+-rw-r--r--   0        0        0    19202 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/dataset_collection_all_of.py
+-rw-r--r--   0        0        0    21845 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/dataset_event.py
+-rw-r--r--   0        0        0    22046 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/dataset_event_collection.py
+-rw-r--r--   0        0        0    19283 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/dataset_event_collection_all_of.py
+-rw-r--r--   0        0        0    20851 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/error.py
+-rw-r--r--   0        0        0    21760 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/event_log.py
+-rw-r--r--   0        0        0    21966 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/event_log_collection.py
+-rw-r--r--   0        0        0    19223 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/event_log_collection_all_of.py
+-rw-r--r--   0        0        0    19628 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/extra_link.py
+-rw-r--r--   0        0        0    19223 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/extra_link_collection.py
+-rw-r--r--   0        0        0    20401 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/health_info.py
+-rw-r--r--   0        0        0    19602 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/health_status.py
+-rw-r--r--   0        0        0    19986 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/import_error.py
+-rw-r--r--   0        0        0    22026 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/import_error_collection.py
+-rw-r--r--   0        0        0    19268 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/import_error_collection_all_of.py
+-rw-r--r--   0        0        0    19005 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/inline_response200.py
+-rw-r--r--   0        0        0    19256 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/inline_response2001.py
+-rw-r--r--   0        0        0    21071 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/job.py
+-rw-r--r--   0        0        0    24213 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/list_dag_runs_form.py
+-rw-r--r--   0        0        0    25771 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/list_task_instance_form.py
+-rw-r--r--   0        0        0    19210 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/metadatabase_status.py
+-rw-r--r--   0        0        0    22019 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/plugin_collection.py
+-rw-r--r--   0        0        0    19287 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/plugin_collection_all_of.py
+-rw-r--r--   0        0        0    23048 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/plugin_collection_item.py
+-rw-r--r--   0        0        0    22705 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/pool.py
+-rw-r--r--   0        0        0    21879 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/pool_collection.py
+-rw-r--r--   0        0        0    19157 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/pool_collection_all_of.py
+-rw-r--r--   0        0        0    19607 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/provider.py
+-rw-r--r--   0        0        0    19202 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/provider_collection.py
+-rw-r--r--   0        0        0    19506 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/queued_event.py
+-rw-r--r--   0        0        0    22001 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/queued_event_collection.py
+-rw-r--r--   0        0        0    19243 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/queued_event_collection_all_of.py
+-rw-r--r--   0        0        0    22235 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/relative_delta.py
+-rw-r--r--   0        0        0    19015 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/resource.py
+-rw-r--r--   0        0        0    19670 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/role.py
+-rw-r--r--   0        0        0    21879 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/role_collection.py
+-rw-r--r--   0        0        0    19157 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/role_collection_all_of.py
+-rw-r--r--   0        0        0    24639 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/schedule_interval.py
+-rw-r--r--   0        0        0    19666 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/scheduler_status.py
+-rw-r--r--   0        0        0    19070 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/set_dag_run_note.py
+-rw-r--r--   0        0        0    19132 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/set_task_instance_note.py
+-rw-r--r--   0        0        0    20383 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/sla_miss.py
+-rw-r--r--   0        0        0    18948 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/tag.py
+-rw-r--r--   0        0        0    25902 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/task.py
+-rw-r--r--   0        0        0    19142 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/task_collection.py
+-rw-r--r--   0        0        0    19227 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/task_extra_links.py
+-rw-r--r--   0        0        0    26592 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/task_instance.py
+-rw-r--r--   0        0        0    22046 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/task_instance_collection.py
+-rw-r--r--   0        0        0    19283 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/task_instance_collection_all_of.py
+-rw-r--r--   0        0        0    19870 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/task_instance_reference.py
+-rw-r--r--   0        0        0    19359 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/task_instance_reference_collection.py
+-rw-r--r--   0        0        0    19960 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/task_outlet_dataset_reference.py
+-rw-r--r--   0        0        0    22519 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/task_state.py
+-rw-r--r--   0        0        0    19700 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/time_delta.py
+-rw-r--r--   0        0        0    19809 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/trigger.py
+-rw-r--r--   0        0        0    22530 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/trigger_rule.py
+-rw-r--r--   0        0        0    19666 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/triggerer_status.py
+-rw-r--r--   0        0        0    19186 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/update_dag_run_state.py
+-rw-r--r--   0        0        0    19851 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/update_task_instance.py
+-rw-r--r--   0        0        0    22282 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/update_task_instances_state.py
+-rw-r--r--   0        0        0    20322 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/update_task_state.py
+-rw-r--r--   0        0        0    25698 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/user.py
+-rw-r--r--   0        0        0    18986 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/user_all_of.py
+-rw-r--r--   0        0        0    21979 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/user_collection.py
+-rw-r--r--   0        0        0    19257 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/user_collection_all_of.py
+-rw-r--r--   0        0        0    23276 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/user_collection_item.py
+-rw-r--r--   0        0        0    19007 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/user_collection_item_roles.py
+-rw-r--r--   0        0        0    21875 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/variable.py
+-rw-r--r--   0        0        0    18983 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/variable_all_of.py
+-rw-r--r--   0        0        0    22059 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/variable_collection.py
+-rw-r--r--   0        0        0    19317 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/variable_collection_all_of.py
+-rw-r--r--   0        0        0    19364 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/variable_collection_item.py
+-rw-r--r--   0        0        0    19371 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/version_info.py
+-rw-r--r--   0        0        0    19663 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/weight_rule.py
+-rw-r--r--   0        0        0    22498 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/x_com.py
+-rw-r--r--   0        0        0    18993 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/x_com_all_of.py
+-rw-r--r--   0        0        0    22016 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/x_com_collection.py
+-rw-r--r--   0        0        0    19293 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/x_com_collection_all_of.py
+-rw-r--r--   0        0        0    20003 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/model/x_com_collection_item.py
+-rw-r--r--   0        0        0     8907 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/airflow_client/client/models/__init__.py
+-rw-r--r--   0        0        0      578 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/Action.md
+-rw-r--r--   0        0        0      723 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ActionCollection.md
+-rw-r--r--   0        0        0      526 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ActionCollectionAllOf.md
+-rw-r--r--   0        0        0      599 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ActionResource.md
+-rw-r--r--   0        0        0     1446 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/BasicDAGRun.md
+-rw-r--r--   0        0        0      585 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ClassReference.md
+-rw-r--r--   0        0        0      706 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ClearDagRun.md
+-rw-r--r--   0        0        0     2250 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ClearTaskInstances.md
+-rw-r--r--   0        0        0      641 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/CollectionInfo.md
+-rw-r--r--   0        0        0      371 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/Color.md
+-rw-r--r--   0        0        0      545 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/Config.md
+-rw-r--r--   0        0        0     5517 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ConfigApi.md
+-rw-r--r--   0        0        0      583 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ConfigOption.md
+-rw-r--r--   0        0        0      607 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ConfigSection.md
+-rw-r--r--   0        0        0     1176 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/Connection.md
+-rw-r--r--   0        0        0      644 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ConnectionAllOf.md
+-rw-r--r--   0        0        0    18687 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ConnectionApi.md
+-rw-r--r--   0        0        0      810 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ConnectionCollection.md
+-rw-r--r--   0        0        0      570 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ConnectionCollectionAllOf.md
+-rw-r--r--   0        0        0     1117 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ConnectionCollectionItem.md
+-rw-r--r--   0        0        0      662 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ConnectionTest.md
+-rw-r--r--   0        0        0      657 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/CreateDatasetEvent.md
+-rw-r--r--   0        0        0      529 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/CronExpression.md
+-rw-r--r--   0        0        0     4174 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DAG.md
+-rw-r--r--   0        0        0    38591 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DAGApi.md
+-rw-r--r--   0        0        0      747 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DAGCollection.md
+-rw-r--r--   0        0        0      514 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DAGCollectionAllOf.md
+-rw-r--r--   0        0        0     5786 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DAGDetail.md
+-rw-r--r--   0        0        0     2037 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DAGDetailAllOf.md
+-rw-r--r--   0        0        0     2986 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DAGRun.md
+-rw-r--r--   0        0        0    33346 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DAGRunApi.md
+-rw-r--r--   0        0        0      764 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DAGRunCollection.md
+-rw-r--r--   0        0        0      527 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DAGRunCollectionAllOf.md
+-rw-r--r--   0        0        0      740 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DagProcessorStatus.md
+-rw-r--r--   0        0        0      782 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DagScheduleDatasetReference.md
+-rw-r--r--   0        0        0      552 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DagState.md
+-rw-r--r--   0        0        0      782 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DagWarning.md
+-rw-r--r--   0        0        0     3987 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DagWarningApi.md
+-rw-r--r--   0        0        0      720 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DagWarningCollection.md
+-rw-r--r--   0        0        0      544 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DagWarningCollectionAllOf.md
+-rw-r--r--   0        0        0     1068 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/Dataset.md
+-rw-r--r--   0        0        0    37997 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DatasetApi.md
+-rw-r--r--   0        0        0      728 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DatasetCollection.md
+-rw-r--r--   0        0        0      530 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DatasetCollectionAllOf.md
+-rw-r--r--   0        0        0     1292 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DatasetEvent.md
+-rw-r--r--   0        0        0      755 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DatasetEventCollection.md
+-rw-r--r--   0        0        0      551 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/DatasetEventCollectionAllOf.md
+-rw-r--r--   0        0        0     1197 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/Error.md
+-rw-r--r--   0        0        0     1366 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/EventLog.md
+-rw-r--r--   0        0        0     8308 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/EventLogApi.md
+-rw-r--r--   0        0        0      774 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/EventLogCollection.md
+-rw-r--r--   0        0        0      535 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/EventLogCollectionAllOf.md
+-rw-r--r--   0        0        0      691 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ExtraLink.md
+-rw-r--r--   0        0        0      565 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ExtraLinkCollection.md
+-rw-r--r--   0        0        0      806 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/HealthInfo.md
+-rw-r--r--   0        0        0      386 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/HealthStatus.md
+-rw-r--r--   0        0        0      765 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ImportError.md
+-rw-r--r--   0        0        0     6265 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ImportErrorApi.md
+-rw-r--r--   0        0        0      789 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ImportErrorCollection.md
+-rw-r--r--   0        0        0      547 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ImportErrorCollectionAllOf.md
+-rw-r--r--   0        0        0      504 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/InlineResponse200.md
+-rw-r--r--   0        0        0      555 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/InlineResponse2001.md
+-rw-r--r--   0        0        0      955 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/Job.md
+-rw-r--r--   0        0        0     2351 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ListDagRunsForm.md
+-rw-r--r--   0        0        0     2935 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ListTaskInstanceForm.md
+-rw-r--r--   0        0        0      564 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/MetadatabaseStatus.md
+-rw-r--r--   0        0        0     4655 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/MonitoringApi.md
+-rw-r--r--   0        0        0     3281 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/PermissionApi.md
+-rw-r--r--   0        0        0     3241 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/PluginApi.md
+-rw-r--r--   0        0        0      750 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/PluginCollection.md
+-rw-r--r--   0        0        0      554 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/PluginCollectionAllOf.md
+-rw-r--r--   0        0        0     1624 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/PluginCollectionItem.md
+-rw-r--r--   0        0        0     1725 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/Pool.md
+-rw-r--r--   0        0        0    14692 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/PoolApi.md
+-rw-r--r--   0        0        0      752 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/PoolCollection.md
+-rw-r--r--   0        0        0      518 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/PoolCollectionAllOf.md
+-rw-r--r--   0        0        0      713 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/Provider.md
+-rw-r--r--   0        0        0     2748 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ProviderApi.md
+-rw-r--r--   0        0        0      579 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ProviderCollection.md
+-rw-r--r--   0        0        0      637 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/QueuedEvent.md
+-rw-r--r--   0        0        0      754 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/QueuedEventCollection.md
+-rw-r--r--   0        0        0      542 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/QueuedEventCollectionAllOf.md
+-rw-r--r--   0        0        0      909 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/RelativeDelta.md
+-rw-r--r--   0        0        0      586 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/Resource.md
+-rw-r--r--   0        0        0      728 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/Role.md
+-rw-r--r--   0        0        0    15554 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/RoleApi.md
+-rw-r--r--   0        0        0      713 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/RoleCollection.md
+-rw-r--r--   0        0        0      518 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/RoleCollectionAllOf.md
+-rw-r--r--   0        0        0      800 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/SLAMiss.md
+-rw-r--r--   0        0        0     1249 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/ScheduleInterval.md
+-rw-r--r--   0        0        0      700 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/SchedulerStatus.md
+-rw-r--r--   0        0        0      541 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/SetDagRunNote.md
+-rw-r--r--   0        0        0      538 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/SetTaskInstanceNote.md
+-rw-r--r--   0        0        0      491 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/Tag.md
+-rw-r--r--   0        0        0     2170 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/Task.md
+-rw-r--r--   0        0        0      534 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/TaskCollection.md
+-rw-r--r--   0        0        0      535 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/TaskExtraLinks.md
+-rw-r--r--   0        0        0     2373 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/TaskInstance.md
+-rw-r--r--   0        0        0    52613 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/TaskInstanceApi.md
+-rw-r--r--   0        0        0      794 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/TaskInstanceCollection.md
+-rw-r--r--   0        0        0      551 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/TaskInstanceCollectionAllOf.md
+-rw-r--r--   0        0        0      716 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/TaskInstanceReference.md
+-rw-r--r--   0        0        0      573 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/TaskInstanceReferenceCollection.md
+-rw-r--r--   0        0        0      845 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/TaskOutletDatasetReference.md
+-rw-r--r--   0        0        0     1536 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/TaskState.md
+-rw-r--r--   0        0        0      579 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/TimeDelta.md
+-rw-r--r--   0        0        0      667 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/Trigger.md
+-rw-r--r--   0        0        0     1443 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/TriggerRule.md
+-rw-r--r--   0        0        0      725 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/TriggererStatus.md
+-rw-r--r--   0        0        0      586 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/UpdateDagRunState.md
+-rw-r--r--   0        0        0      791 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/UpdateTaskInstance.md
+-rw-r--r--   0        0        0     1526 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/UpdateTaskInstancesState.md
+-rw-r--r--   0        0        0      735 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/UpdateTaskState.md
+-rw-r--r--   0        0        0     1903 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/User.md
+-rw-r--r--   0        0        0      497 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/UserAllOf.md
+-rw-r--r--   0        0        0    15526 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/UserApi.md
+-rw-r--r--   0        0        0      739 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/UserCollection.md
+-rw-r--r--   0        0        0      546 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/UserCollectionAllOf.md
+-rw-r--r--   0        0        0     1857 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/UserCollectionItem.md
+-rw-r--r--   0        0        0      507 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/UserCollectionItemRoles.md
+-rw-r--r--   0        0        0      671 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/Variable.md
+-rw-r--r--   0        0        0      498 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/VariableAllOf.md
+-rw-r--r--   0        0        0    15059 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/VariableApi.md
+-rw-r--r--   0        0        0      800 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/VariableCollection.md
+-rw-r--r--   0        0        0      562 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/VariableCollectionAllOf.md
+-rw-r--r--   0        0        0      748 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/VariableCollectionItem.md
+-rw-r--r--   0        0        0      638 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/VersionInfo.md
+-rw-r--r--   0        0        0      396 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/WeightRule.md
+-rw-r--r--   0        0        0      774 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/XCom.md
+-rw-r--r--   0        0        0      503 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/XComAllOf.md
+-rw-r--r--   0        0        0     9154 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/XComApi.md
+-rw-r--r--   0        0        0      794 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/XComCollection.md
+-rw-r--r--   0        0        0      553 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/XComCollectionAllOf.md
+-rw-r--r--   0        0        0      829 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/docs/XComCollectionItem.md
+-rw-r--r--   0        0        0        0 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/__init__.py
+-rw-r--r--   0        0        0     8665 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_action.py
+-rw-r--r--   0        0        0     9081 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_action_collection.py
+-rw-r--r--   0        0        0     8856 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_action_collection_all_of.py
+-rw-r--r--   0        0        0     8896 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_action_resource.py
+-rw-r--r--   0        0        0     8794 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_basic_dag_run.py
+-rw-r--r--   0        0        0     8722 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_class_reference.py
+-rw-r--r--   0        0        0     8702 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_clear_dag_run.py
+-rw-r--r--   0        0        0     8751 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_clear_task_instances.py
+-rw-r--r--   0        0        0     8722 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_collection_info.py
+-rw-r--r--   0        0        0     8658 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_color.py
+-rw-r--r--   0        0        0     8777 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_config.py
+-rw-r--r--   0        0        0     8812 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_config_api.py
+-rw-r--r--   0        0        0     8708 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_config_option.py
+-rw-r--r--   0        0        0     8823 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_config_section.py
+-rw-r--r--   0        0        0     8971 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_connection.py
+-rw-r--r--   0        0        0     8730 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_connection_all_of.py
+-rw-r--r--   0        0        0     9416 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_connection_api.py
+-rw-r--r--   0        0        0     9199 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_connection_collection.py
+-rw-r--r--   0        0        0     8958 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_connection_collection_all_of.py
+-rw-r--r--   0        0        0     8793 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_connection_collection_item.py
+-rw-r--r--   0        0        0     8722 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_connection_test.py
+-rw-r--r--   0        0        0     8751 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_create_dataset_event.py
+-rw-r--r--   0        0        0     8722 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_cron_expression.py
+-rw-r--r--   0        0        0     8839 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dag.py
+-rw-r--r--   0        0        0    10110 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dag_api.py
+-rw-r--r--   0        0        0     9036 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dag_collection.py
+-rw-r--r--   0        0        0     8823 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dag_collection_all_of.py
+-rw-r--r--   0        0        0     9167 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dag_detail.py
+-rw-r--r--   0        0        0     8820 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dag_detail_all_of.py
+-rw-r--r--   0        0        0     8859 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dag_processor_status.py
+-rw-r--r--   0        0        0     8758 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dag_run.py
+-rw-r--r--   0        0        0     9855 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dag_run_api.py
+-rw-r--r--   0        0        0     9084 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dag_run_collection.py
+-rw-r--r--   0        0        0     8858 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dag_run_collection_all_of.py
+-rw-r--r--   0        0        0     8815 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dag_schedule_dataset_reference.py
+-rw-r--r--   0        0        0     8680 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dag_state.py
+-rw-r--r--   0        0        0     8694 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dag_warning.py
+-rw-r--r--   0        0        0     8691 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dag_warning_api.py
+-rw-r--r--   0        0        0     9144 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dag_warning_collection.py
+-rw-r--r--   0        0        0     8902 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dag_warning_collection_all_of.py
+-rw-r--r--   0        0        0     9008 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dataset.py
+-rw-r--r--   0        0        0    10448 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dataset_api.py
+-rw-r--r--   0        0        0     9096 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dataset_collection.py
+-rw-r--r--   0        0        0     8867 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dataset_collection_all_of.py
+-rw-r--r--   0        0        0     8813 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dataset_event.py
+-rw-r--r--   0        0        0     9174 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dataset_event_collection.py
+-rw-r--r--   0        0        0     8924 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_dataset_event_collection_all_of.py
+-rw-r--r--   0        0        0     8658 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_error.py
+-rw-r--r--   0        0        0     8680 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_event_log.py
+-rw-r--r--   0        0        0     8814 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_event_log_api.py
+-rw-r--r--   0        0        0     9114 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_event_log_collection.py
+-rw-r--r--   0        0        0     8880 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_event_log_collection_all_of.py
+-rw-r--r--   0        0        0     8803 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_extra_link.py
+-rw-r--r--   0        0        0     8854 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_extra_link_collection.py
+-rw-r--r--   0        0        0     9199 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_health_info.py
+-rw-r--r--   0        0        0     8708 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_health_status.py
+-rw-r--r--   0        0        0     8701 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_import_error.py
+-rw-r--r--   0        0        0     8847 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_import_error_api.py
+-rw-r--r--   0        0        0     9159 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_import_error_collection.py
+-rw-r--r--   0        0        0     8913 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_import_error_collection_all_of.py
+-rw-r--r--   0        0        0     8743 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_inline_response200.py
+-rw-r--r--   0        0        0     8750 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_inline_response2001.py
+-rw-r--r--   0        0        0     8644 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_job.py
+-rw-r--r--   0        0        0     8731 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_list_dag_runs_form.py
+-rw-r--r--   0        0        0     8862 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_list_task_instance_form.py
+-rw-r--r--   0        0        0     8858 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_metadatabase_status.py
+-rw-r--r--   0        0        0     8822 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_monitoring_api.py
+-rw-r--r--   0        0        0     8687 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_permission_api.py
+-rw-r--r--   0        0        0     8671 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_plugin_api.py
+-rw-r--r--   0        0        0     9139 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_plugin_collection.py
+-rw-r--r--   0        0        0     8914 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_plugin_collection_all_of.py
+-rw-r--r--   0        0        0     8765 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_plugin_collection_item.py
+-rw-r--r--   0        0        0     8651 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_pool.py
+-rw-r--r--   0        0        0     9152 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_pool_api.py
+-rw-r--r--   0        0        0     9051 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_pool_collection.py
+-rw-r--r--   0        0        0     8834 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_pool_collection_all_of.py
+-rw-r--r--   0        0        0     8679 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_provider.py
+-rw-r--r--   0        0        0     8671 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_provider_api.py
+-rw-r--r--   0        0        0     8841 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_provider_collection.py
+-rw-r--r--   0        0        0     8701 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_queued_event.py
+-rw-r--r--   0        0        0     9159 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_queued_event_collection.py
+-rw-r--r--   0        0        0     8913 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_queued_event_collection_all_of.py
+-rw-r--r--   0        0        0     8715 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_relative_delta.py
+-rw-r--r--   0        0        0     8679 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_resource.py
+-rw-r--r--   0        0        0     8767 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_role.py
+-rw-r--r--   0        0        0     9152 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_role_api.py
+-rw-r--r--   0        0        0     9051 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_role_collection.py
+-rw-r--r--   0        0        0     8834 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_role_collection_all_of.py
+-rw-r--r--   0        0        0     9060 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_schedule_interval.py
+-rw-r--r--   0        0        0     8837 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_scheduler_status.py
+-rw-r--r--   0        0        0     8717 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_set_dag_run_note.py
+-rw-r--r--   0        0        0     8759 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_set_task_instance_note.py
+-rw-r--r--   0        0        0     8673 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_sla_miss.py
+-rw-r--r--   0        0        0     8644 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_tag.py
+-rw-r--r--   0        0        0     9334 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_task.py
+-rw-r--r--   0        0        0     8797 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_task_collection.py
+-rw-r--r--   0        0        0     8839 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_task_extra_links.py
+-rw-r--r--   0        0        0     9050 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_task_instance.py
+-rw-r--r--   0        0        0    10352 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_task_instance_api.py
+-rw-r--r--   0        0        0     9174 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_task_instance_collection.py
+-rw-r--r--   0        0        0     8924 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_task_instance_collection_all_of.py
+-rw-r--r--   0        0        0     8772 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_task_instance_reference.py
+-rw-r--r--   0        0        0     8988 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_task_instance_reference_collection.py
+-rw-r--r--   0        0        0     8808 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_task_outlet_dataset_reference.py
+-rw-r--r--   0        0        0     8687 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_task_state.py
+-rw-r--r--   0        0        0     8687 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_time_delta.py
+-rw-r--r--   0        0        0     8672 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_trigger.py
+-rw-r--r--   0        0        0     8701 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_trigger_rule.py
+-rw-r--r--   0        0        0     8837 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_triggerer_status.py
+-rw-r--r--   0        0        0     8745 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_update_dag_run_state.py
+-rw-r--r--   0        0        0     8872 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_update_task_instance.py
+-rw-r--r--   0        0        0     8915 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_update_task_instances_state.py
+-rw-r--r--   0        0        0     8730 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_update_task_state.py
+-rw-r--r--   0        0        0     9035 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_user.py
+-rw-r--r--   0        0        0     8688 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_user_all_of.py
+-rw-r--r--   0        0        0     9152 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_user_api.py
+-rw-r--r--   0        0        0     9109 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_user_collection.py
+-rw-r--r--   0        0        0     8892 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_user_collection_all_of.py
+-rw-r--r--   0        0        0     8905 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_user_collection_item.py
+-rw-r--r--   0        0        0     8787 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_user_collection_item_roles.py
+-rw-r--r--   0        0        0     8941 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_variable.py
+-rw-r--r--   0        0        0     8716 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_variable_all_of.py
+-rw-r--r--   0        0        0     9234 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_variable_api.py
+-rw-r--r--   0        0        0     9169 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_variable_collection.py
+-rw-r--r--   0        0        0     8936 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_variable_collection_all_of.py
+-rw-r--r--   0        0        0     8779 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_variable_collection_item.py
+-rw-r--r--   0        0        0     8701 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_version_info.py
+-rw-r--r--   0        0        0     8694 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_weight_rule.py
+-rw-r--r--   0        0        0     8884 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_x_com.py
+-rw-r--r--   0        0        0     8689 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_x_com_all_of.py
+-rw-r--r--   0        0        0     8803 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_x_com_api.py
+-rw-r--r--   0        0        0     9112 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_x_com_collection.py
+-rw-r--r--   0        0        0     8894 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_x_com_collection_all_of.py
+-rw-r--r--   0        0        0     8752 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/test/test_x_com_collection_item.py
+-rw-r--r--   0        0        0       99 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/.gitignore
+-rw-r--r--   0        0        0    13569 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/NOTICE
+-rw-r--r--   0        0        0    29440 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/README.md
+-rw-r--r--   0        0        0     3273 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    30912 2024-04-06 20:41:24.000000 apache_airflow_client-2.9.0rc1/PKG-INFO
```

### Comparing `apache_airflow_client-2.9.0/INSTALL` & `apache_airflow_client-2.9.0rc1/INSTALL`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/v1.yaml` & `apache_airflow_client-2.9.0rc1/v1.yaml`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/__init__.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: 2.9.0
     Contact: dev@airflow.apache.org
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "&quot;2.9.0&quot;"
+__version__ = "&quot;2.9.0rc1&quot;"
 
 # import ApiClient
 from airflow_client.client.api_client import ApiClient
 
 # import Configuration
 from airflow_client.client.configuration import Configuration
```

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/api_client.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/"2.9.0"/python'
+        self.user_agent = 'OpenAPI-Generator/"2.9.0rc1"/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/configuration.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -401,15 +401,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 2.9.0\n"\
-               "SDK Package Version: &quot;2.9.0&quot;".\
+               "SDK Package Version: &quot;2.9.0rc1&quot;".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/exceptions.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model_utils.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model_utils.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/rest.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/rest.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/api/config_api.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/api/config_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/api/connection_api.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/api/connection_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/api/dag_api.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/api/dag_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/api/dag_run_api.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/api/dag_run_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/api/dag_warning_api.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/api/dag_warning_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/api/dataset_api.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/api/dataset_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/api/event_log_api.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/api/event_log_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/api/import_error_api.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/api/import_error_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/api/monitoring_api.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/api/monitoring_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/api/permission_api.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/api/permission_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/api/plugin_api.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/api/plugin_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/api/pool_api.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/api/pool_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/api/provider_api.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/api/provider_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/api/role_api.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/api/role_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/api/task_instance_api.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/api/task_instance_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/api/user_api.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/api/variable_api.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/api/variable_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/api/x_com_api.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/api/x_com_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/apis/__init__.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/action.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/action.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/action_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/action_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/action_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/action_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/action_resource.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/action_resource.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/basic_dag_run.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/basic_dag_run.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/class_reference.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/class_reference.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/clear_dag_run.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/clear_dag_run.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/clear_task_instances.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/clear_task_instances.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/collection_info.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/collection_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/color.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/color.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/config.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/config.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/config_option.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/config_option.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/config_section.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/config_section.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/connection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/connection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/connection_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/connection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/connection_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/connection_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/connection_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/connection_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/connection_collection_item.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/connection_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/connection_test.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/connection_test.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/create_dataset_event.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/create_dataset_event.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/cron_expression.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/cron_expression.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/dag.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/dag_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/dag_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/dag_detail.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_detail.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/dag_detail_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_detail_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/dag_processor_status.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_processor_status.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/dag_run.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_run.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/dag_run_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_run_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/dag_run_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_run_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/dag_schedule_dataset_reference.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_schedule_dataset_reference.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/dag_state.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_state.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/dag_warning.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_warning.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/dag_warning_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_warning_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/dag_warning_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/dag_warning_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/dataset.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/dataset.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/dataset_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/dataset_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/dataset_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/dataset_event.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/dataset_event.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/dataset_event_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/dataset_event_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/dataset_event_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/dataset_event_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/error.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/error.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/event_log.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/event_log.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/event_log_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/event_log_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/event_log_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/event_log_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/extra_link.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/extra_link.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/extra_link_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/extra_link_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/health_info.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/health_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/health_status.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/health_status.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/import_error.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/import_error.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/import_error_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/import_error_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/import_error_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/import_error_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/inline_response200.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/inline_response200.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/inline_response2001.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/job.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/job.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/list_dag_runs_form.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/list_dag_runs_form.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/list_task_instance_form.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/list_task_instance_form.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/metadatabase_status.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/metadatabase_status.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/plugin_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/plugin_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/plugin_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/plugin_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/plugin_collection_item.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/plugin_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/pool.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/pool.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/pool_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/pool_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/pool_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/pool_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/provider.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/provider.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/provider_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/provider_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/queued_event.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/queued_event.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/queued_event_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/queued_event_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/queued_event_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/queued_event_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/relative_delta.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/relative_delta.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/resource.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/resource.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/role.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/role.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/role_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/role_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/role_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/role_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/schedule_interval.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/schedule_interval.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/scheduler_status.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/scheduler_status.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/set_dag_run_note.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/set_dag_run_note.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/set_task_instance_note.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/set_task_instance_note.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/sla_miss.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/sla_miss.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/tag.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/tag.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/task.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/task.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/task_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/task_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/task_extra_links.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/task_extra_links.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/task_instance.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/task_instance.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/task_instance_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/task_instance_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/task_instance_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/task_instance_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/task_instance_reference.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/task_instance_reference.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/task_instance_reference_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/task_instance_reference_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/task_outlet_dataset_reference.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/task_outlet_dataset_reference.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/task_state.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/task_state.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/time_delta.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/time_delta.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/trigger.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/trigger.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/trigger_rule.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/trigger_rule.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/triggerer_status.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/triggerer_status.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/update_dag_run_state.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/update_dag_run_state.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/update_task_instance.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/update_task_instance.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/update_task_instances_state.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/update_task_instances_state.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/update_task_state.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/update_task_state.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/user.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/user.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/user_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/user_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/user_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/user_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/user_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/user_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/user_collection_item.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/user_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/user_collection_item_roles.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/user_collection_item_roles.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/variable.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/variable.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/variable_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/variable_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/variable_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/variable_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/variable_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/variable_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/variable_collection_item.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/variable_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/version_info.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/version_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/weight_rule.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/weight_rule.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/x_com.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/x_com.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/x_com_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/x_com_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/x_com_collection.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/x_com_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/x_com_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/x_com_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/model/x_com_collection_item.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/model/x_com_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/airflow_client/client/models/__init__.py` & `apache_airflow_client-2.9.0rc1/airflow_client/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/Action.md` & `apache_airflow_client-2.9.0rc1/docs/Action.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ActionCollection.md` & `apache_airflow_client-2.9.0rc1/docs/ActionCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ActionCollectionAllOf.md` & `apache_airflow_client-2.9.0rc1/docs/ActionCollectionAllOf.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ActionResource.md` & `apache_airflow_client-2.9.0rc1/docs/ActionResource.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/BasicDAGRun.md` & `apache_airflow_client-2.9.0rc1/docs/BasicDAGRun.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ClassReference.md` & `apache_airflow_client-2.9.0rc1/docs/ClassReference.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ClearDagRun.md` & `apache_airflow_client-2.9.0rc1/docs/ClearDagRun.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ClearTaskInstances.md` & `apache_airflow_client-2.9.0rc1/docs/ClearTaskInstances.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/CollectionInfo.md` & `apache_airflow_client-2.9.0rc1/docs/CollectionInfo.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/Config.md` & `apache_airflow_client-2.9.0rc1/docs/Config.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ConfigApi.md` & `apache_airflow_client-2.9.0rc1/docs/ConfigApi.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ConfigOption.md` & `apache_airflow_client-2.9.0rc1/docs/ConfigOption.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ConfigSection.md` & `apache_airflow_client-2.9.0rc1/docs/ConfigSection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/Connection.md` & `apache_airflow_client-2.9.0rc1/docs/Connection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ConnectionAllOf.md` & `apache_airflow_client-2.9.0rc1/docs/ConnectionAllOf.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ConnectionApi.md` & `apache_airflow_client-2.9.0rc1/docs/ConnectionApi.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ConnectionCollection.md` & `apache_airflow_client-2.9.0rc1/docs/ConnectionCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ConnectionCollectionAllOf.md` & `apache_airflow_client-2.9.0rc1/docs/ConnectionCollectionAllOf.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ConnectionCollectionItem.md` & `apache_airflow_client-2.9.0rc1/docs/ConnectionCollectionItem.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ConnectionTest.md` & `apache_airflow_client-2.9.0rc1/docs/ConnectionTest.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/CreateDatasetEvent.md` & `apache_airflow_client-2.9.0rc1/docs/CreateDatasetEvent.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/CronExpression.md` & `apache_airflow_client-2.9.0rc1/docs/CronExpression.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DAG.md` & `apache_airflow_client-2.9.0rc1/docs/DAG.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DAGApi.md` & `apache_airflow_client-2.9.0rc1/docs/DAGApi.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DAGCollection.md` & `apache_airflow_client-2.9.0rc1/docs/DAGCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DAGCollectionAllOf.md` & `apache_airflow_client-2.9.0rc1/docs/DAGCollectionAllOf.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DAGDetail.md` & `apache_airflow_client-2.9.0rc1/docs/DAGDetail.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DAGDetailAllOf.md` & `apache_airflow_client-2.9.0rc1/docs/DAGDetailAllOf.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DAGRun.md` & `apache_airflow_client-2.9.0rc1/docs/DAGRun.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DAGRunApi.md` & `apache_airflow_client-2.9.0rc1/docs/DAGRunApi.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DAGRunCollection.md` & `apache_airflow_client-2.9.0rc1/docs/DAGRunCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DAGRunCollectionAllOf.md` & `apache_airflow_client-2.9.0rc1/docs/DAGRunCollectionAllOf.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DagProcessorStatus.md` & `apache_airflow_client-2.9.0rc1/docs/DagProcessorStatus.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DagScheduleDatasetReference.md` & `apache_airflow_client-2.9.0rc1/docs/DagScheduleDatasetReference.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DagState.md` & `apache_airflow_client-2.9.0rc1/docs/DagState.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DagWarning.md` & `apache_airflow_client-2.9.0rc1/docs/DagWarning.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DagWarningApi.md` & `apache_airflow_client-2.9.0rc1/docs/DagWarningApi.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DagWarningCollection.md` & `apache_airflow_client-2.9.0rc1/docs/DagWarningCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DagWarningCollectionAllOf.md` & `apache_airflow_client-2.9.0rc1/docs/DagWarningCollectionAllOf.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/Dataset.md` & `apache_airflow_client-2.9.0rc1/docs/Dataset.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DatasetApi.md` & `apache_airflow_client-2.9.0rc1/docs/DatasetApi.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DatasetCollection.md` & `apache_airflow_client-2.9.0rc1/docs/DatasetCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DatasetCollectionAllOf.md` & `apache_airflow_client-2.9.0rc1/docs/DatasetCollectionAllOf.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DatasetEvent.md` & `apache_airflow_client-2.9.0rc1/docs/DatasetEvent.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DatasetEventCollection.md` & `apache_airflow_client-2.9.0rc1/docs/DatasetEventCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/DatasetEventCollectionAllOf.md` & `apache_airflow_client-2.9.0rc1/docs/DatasetEventCollectionAllOf.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/Error.md` & `apache_airflow_client-2.9.0rc1/docs/Error.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/EventLog.md` & `apache_airflow_client-2.9.0rc1/docs/EventLog.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/EventLogApi.md` & `apache_airflow_client-2.9.0rc1/docs/EventLogApi.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/EventLogCollection.md` & `apache_airflow_client-2.9.0rc1/docs/EventLogCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/EventLogCollectionAllOf.md` & `apache_airflow_client-2.9.0rc1/docs/EventLogCollectionAllOf.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ExtraLink.md` & `apache_airflow_client-2.9.0rc1/docs/ExtraLink.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ExtraLinkCollection.md` & `apache_airflow_client-2.9.0rc1/docs/ExtraLinkCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/HealthInfo.md` & `apache_airflow_client-2.9.0rc1/docs/HealthInfo.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ImportError.md` & `apache_airflow_client-2.9.0rc1/docs/ImportError.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ImportErrorApi.md` & `apache_airflow_client-2.9.0rc1/docs/ImportErrorApi.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ImportErrorCollection.md` & `apache_airflow_client-2.9.0rc1/docs/ImportErrorCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ImportErrorCollectionAllOf.md` & `apache_airflow_client-2.9.0rc1/docs/ImportErrorCollectionAllOf.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/InlineResponse2001.md` & `apache_airflow_client-2.9.0rc1/docs/InlineResponse2001.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/Job.md` & `apache_airflow_client-2.9.0rc1/docs/Job.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ListDagRunsForm.md` & `apache_airflow_client-2.9.0rc1/docs/ListDagRunsForm.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ListTaskInstanceForm.md` & `apache_airflow_client-2.9.0rc1/docs/ListTaskInstanceForm.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/MetadatabaseStatus.md` & `apache_airflow_client-2.9.0rc1/docs/MetadatabaseStatus.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/MonitoringApi.md` & `apache_airflow_client-2.9.0rc1/docs/MonitoringApi.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/PermissionApi.md` & `apache_airflow_client-2.9.0rc1/docs/PermissionApi.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/PluginApi.md` & `apache_airflow_client-2.9.0rc1/docs/PluginApi.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/PluginCollection.md` & `apache_airflow_client-2.9.0rc1/docs/PluginCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/PluginCollectionAllOf.md` & `apache_airflow_client-2.9.0rc1/docs/PluginCollectionAllOf.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/PluginCollectionItem.md` & `apache_airflow_client-2.9.0rc1/docs/PluginCollectionItem.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/Pool.md` & `apache_airflow_client-2.9.0rc1/docs/Pool.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/PoolApi.md` & `apache_airflow_client-2.9.0rc1/docs/PoolApi.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/PoolCollection.md` & `apache_airflow_client-2.9.0rc1/docs/PoolCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/PoolCollectionAllOf.md` & `apache_airflow_client-2.9.0rc1/docs/PoolCollectionAllOf.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/Provider.md` & `apache_airflow_client-2.9.0rc1/docs/Provider.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ProviderApi.md` & `apache_airflow_client-2.9.0rc1/docs/ProviderApi.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ProviderCollection.md` & `apache_airflow_client-2.9.0rc1/docs/ProviderCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/QueuedEvent.md` & `apache_airflow_client-2.9.0rc1/docs/QueuedEvent.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/QueuedEventCollection.md` & `apache_airflow_client-2.9.0rc1/docs/QueuedEventCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/QueuedEventCollectionAllOf.md` & `apache_airflow_client-2.9.0rc1/docs/QueuedEventCollectionAllOf.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/RelativeDelta.md` & `apache_airflow_client-2.9.0rc1/docs/RelativeDelta.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/Resource.md` & `apache_airflow_client-2.9.0rc1/docs/Resource.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/Role.md` & `apache_airflow_client-2.9.0rc1/docs/Role.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/RoleApi.md` & `apache_airflow_client-2.9.0rc1/docs/RoleApi.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/RoleCollection.md` & `apache_airflow_client-2.9.0rc1/docs/RoleCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/RoleCollectionAllOf.md` & `apache_airflow_client-2.9.0rc1/docs/RoleCollectionAllOf.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/SLAMiss.md` & `apache_airflow_client-2.9.0rc1/docs/SLAMiss.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/ScheduleInterval.md` & `apache_airflow_client-2.9.0rc1/docs/ScheduleInterval.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/SchedulerStatus.md` & `apache_airflow_client-2.9.0rc1/docs/SchedulerStatus.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/SetDagRunNote.md` & `apache_airflow_client-2.9.0rc1/docs/SetDagRunNote.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/SetTaskInstanceNote.md` & `apache_airflow_client-2.9.0rc1/docs/SetTaskInstanceNote.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/Task.md` & `apache_airflow_client-2.9.0rc1/docs/Task.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/TaskCollection.md` & `apache_airflow_client-2.9.0rc1/docs/TaskCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/TaskExtraLinks.md` & `apache_airflow_client-2.9.0rc1/docs/TaskExtraLinks.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/TaskInstance.md` & `apache_airflow_client-2.9.0rc1/docs/TaskInstance.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/TaskInstanceApi.md` & `apache_airflow_client-2.9.0rc1/docs/TaskInstanceApi.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/TaskInstanceCollection.md` & `apache_airflow_client-2.9.0rc1/docs/TaskInstanceCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/TaskInstanceCollectionAllOf.md` & `apache_airflow_client-2.9.0rc1/docs/TaskInstanceCollectionAllOf.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/TaskInstanceReference.md` & `apache_airflow_client-2.9.0rc1/docs/TaskInstanceReference.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/TaskInstanceReferenceCollection.md` & `apache_airflow_client-2.9.0rc1/docs/TaskInstanceReferenceCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/TaskOutletDatasetReference.md` & `apache_airflow_client-2.9.0rc1/docs/TaskOutletDatasetReference.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/TaskState.md` & `apache_airflow_client-2.9.0rc1/docs/TaskState.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/TimeDelta.md` & `apache_airflow_client-2.9.0rc1/docs/TimeDelta.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/Trigger.md` & `apache_airflow_client-2.9.0rc1/docs/Trigger.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/TriggerRule.md` & `apache_airflow_client-2.9.0rc1/docs/TriggerRule.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/TriggererStatus.md` & `apache_airflow_client-2.9.0rc1/docs/TriggererStatus.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/UpdateDagRunState.md` & `apache_airflow_client-2.9.0rc1/docs/UpdateDagRunState.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/UpdateTaskInstance.md` & `apache_airflow_client-2.9.0rc1/docs/UpdateTaskInstance.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/UpdateTaskInstancesState.md` & `apache_airflow_client-2.9.0rc1/docs/UpdateTaskInstancesState.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/UpdateTaskState.md` & `apache_airflow_client-2.9.0rc1/docs/UpdateTaskState.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/User.md` & `apache_airflow_client-2.9.0rc1/docs/User.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/UserApi.md` & `apache_airflow_client-2.9.0rc1/docs/UserApi.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/UserCollection.md` & `apache_airflow_client-2.9.0rc1/docs/UserCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/UserCollectionAllOf.md` & `apache_airflow_client-2.9.0rc1/docs/UserCollectionAllOf.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/UserCollectionItem.md` & `apache_airflow_client-2.9.0rc1/docs/UserCollectionItem.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/Variable.md` & `apache_airflow_client-2.9.0rc1/docs/Variable.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/VariableApi.md` & `apache_airflow_client-2.9.0rc1/docs/VariableApi.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/VariableCollection.md` & `apache_airflow_client-2.9.0rc1/docs/VariableCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/VariableCollectionAllOf.md` & `apache_airflow_client-2.9.0rc1/docs/VariableCollectionAllOf.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/VariableCollectionItem.md` & `apache_airflow_client-2.9.0rc1/docs/VariableCollectionItem.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/VersionInfo.md` & `apache_airflow_client-2.9.0rc1/docs/VersionInfo.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/XCom.md` & `apache_airflow_client-2.9.0rc1/docs/XCom.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/XComApi.md` & `apache_airflow_client-2.9.0rc1/docs/XComApi.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/XComCollection.md` & `apache_airflow_client-2.9.0rc1/docs/XComCollection.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/XComCollectionAllOf.md` & `apache_airflow_client-2.9.0rc1/docs/XComCollectionAllOf.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/docs/XComCollectionItem.md` & `apache_airflow_client-2.9.0rc1/docs/XComCollectionItem.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_action.py` & `apache_airflow_client-2.9.0rc1/test/test_action.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_action_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_action_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_action_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_action_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_action_resource.py` & `apache_airflow_client-2.9.0rc1/test/test_action_resource.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_basic_dag_run.py` & `apache_airflow_client-2.9.0rc1/test/test_basic_dag_run.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_class_reference.py` & `apache_airflow_client-2.9.0rc1/test/test_class_reference.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_clear_dag_run.py` & `apache_airflow_client-2.9.0rc1/test/test_clear_dag_run.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_clear_task_instances.py` & `apache_airflow_client-2.9.0rc1/test/test_clear_task_instances.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_collection_info.py` & `apache_airflow_client-2.9.0rc1/test/test_collection_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_color.py` & `apache_airflow_client-2.9.0rc1/test/test_color.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_config.py` & `apache_airflow_client-2.9.0rc1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_config_api.py` & `apache_airflow_client-2.9.0rc1/test/test_config_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_config_option.py` & `apache_airflow_client-2.9.0rc1/test/test_config_option.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_config_section.py` & `apache_airflow_client-2.9.0rc1/test/test_config_section.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_connection.py` & `apache_airflow_client-2.9.0rc1/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_connection_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_connection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_connection_api.py` & `apache_airflow_client-2.9.0rc1/test/test_connection_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_connection_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_connection_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_connection_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_connection_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_connection_collection_item.py` & `apache_airflow_client-2.9.0rc1/test/test_connection_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_connection_test.py` & `apache_airflow_client-2.9.0rc1/test/test_connection_test.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_create_dataset_event.py` & `apache_airflow_client-2.9.0rc1/test/test_create_dataset_event.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_cron_expression.py` & `apache_airflow_client-2.9.0rc1/test/test_cron_expression.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dag.py` & `apache_airflow_client-2.9.0rc1/test/test_dag.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dag_api.py` & `apache_airflow_client-2.9.0rc1/test/test_dag_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dag_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_dag_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dag_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_dag_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dag_detail.py` & `apache_airflow_client-2.9.0rc1/test/test_dag_detail.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dag_detail_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_dag_detail_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dag_processor_status.py` & `apache_airflow_client-2.9.0rc1/test/test_dag_processor_status.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dag_run.py` & `apache_airflow_client-2.9.0rc1/test/test_dag_run.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dag_run_api.py` & `apache_airflow_client-2.9.0rc1/test/test_dag_run_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dag_run_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_dag_run_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dag_run_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_dag_run_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dag_schedule_dataset_reference.py` & `apache_airflow_client-2.9.0rc1/test/test_dag_schedule_dataset_reference.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dag_state.py` & `apache_airflow_client-2.9.0rc1/test/test_dag_state.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dag_warning.py` & `apache_airflow_client-2.9.0rc1/test/test_dag_warning.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dag_warning_api.py` & `apache_airflow_client-2.9.0rc1/test/test_dag_warning_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dag_warning_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_dag_warning_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dag_warning_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_dag_warning_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dataset.py` & `apache_airflow_client-2.9.0rc1/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dataset_api.py` & `apache_airflow_client-2.9.0rc1/test/test_dataset_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dataset_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dataset_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_dataset_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dataset_event.py` & `apache_airflow_client-2.9.0rc1/test/test_dataset_event.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dataset_event_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_dataset_event_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_dataset_event_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_dataset_event_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_error.py` & `apache_airflow_client-2.9.0rc1/test/test_error.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_event_log.py` & `apache_airflow_client-2.9.0rc1/test/test_event_log.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_event_log_api.py` & `apache_airflow_client-2.9.0rc1/test/test_event_log_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_event_log_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_event_log_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_event_log_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_event_log_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_extra_link.py` & `apache_airflow_client-2.9.0rc1/test/test_extra_link.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_extra_link_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_extra_link_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_health_info.py` & `apache_airflow_client-2.9.0rc1/test/test_health_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_health_status.py` & `apache_airflow_client-2.9.0rc1/test/test_health_status.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_import_error.py` & `apache_airflow_client-2.9.0rc1/test/test_import_error.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_import_error_api.py` & `apache_airflow_client-2.9.0rc1/test/test_import_error_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_import_error_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_import_error_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_import_error_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_import_error_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_inline_response200.py` & `apache_airflow_client-2.9.0rc1/test/test_inline_response200.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_inline_response2001.py` & `apache_airflow_client-2.9.0rc1/test/test_inline_response2001.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_job.py` & `apache_airflow_client-2.9.0rc1/test/test_job.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_list_dag_runs_form.py` & `apache_airflow_client-2.9.0rc1/test/test_list_dag_runs_form.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_list_task_instance_form.py` & `apache_airflow_client-2.9.0rc1/test/test_list_task_instance_form.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_metadatabase_status.py` & `apache_airflow_client-2.9.0rc1/test/test_metadatabase_status.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_monitoring_api.py` & `apache_airflow_client-2.9.0rc1/test/test_monitoring_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_permission_api.py` & `apache_airflow_client-2.9.0rc1/test/test_permission_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_plugin_api.py` & `apache_airflow_client-2.9.0rc1/test/test_plugin_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_plugin_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_plugin_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_plugin_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_plugin_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_plugin_collection_item.py` & `apache_airflow_client-2.9.0rc1/test/test_plugin_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_pool.py` & `apache_airflow_client-2.9.0rc1/test/test_pool.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_pool_api.py` & `apache_airflow_client-2.9.0rc1/test/test_pool_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_pool_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_pool_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_pool_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_pool_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_provider.py` & `apache_airflow_client-2.9.0rc1/test/test_provider.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_provider_api.py` & `apache_airflow_client-2.9.0rc1/test/test_provider_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_provider_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_provider_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_queued_event.py` & `apache_airflow_client-2.9.0rc1/test/test_queued_event.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_queued_event_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_queued_event_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_queued_event_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_queued_event_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_relative_delta.py` & `apache_airflow_client-2.9.0rc1/test/test_relative_delta.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_resource.py` & `apache_airflow_client-2.9.0rc1/test/test_resource.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_role.py` & `apache_airflow_client-2.9.0rc1/test/test_role.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_role_api.py` & `apache_airflow_client-2.9.0rc1/test/test_role_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_role_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_role_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_role_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_role_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_schedule_interval.py` & `apache_airflow_client-2.9.0rc1/test/test_schedule_interval.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_scheduler_status.py` & `apache_airflow_client-2.9.0rc1/test/test_scheduler_status.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_set_dag_run_note.py` & `apache_airflow_client-2.9.0rc1/test/test_set_dag_run_note.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_set_task_instance_note.py` & `apache_airflow_client-2.9.0rc1/test/test_set_task_instance_note.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_sla_miss.py` & `apache_airflow_client-2.9.0rc1/test/test_sla_miss.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_tag.py` & `apache_airflow_client-2.9.0rc1/test/test_tag.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_task.py` & `apache_airflow_client-2.9.0rc1/test/test_task.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_task_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_task_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_task_extra_links.py` & `apache_airflow_client-2.9.0rc1/test/test_task_extra_links.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_task_instance.py` & `apache_airflow_client-2.9.0rc1/test/test_task_instance.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_task_instance_api.py` & `apache_airflow_client-2.9.0rc1/test/test_task_instance_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_task_instance_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_task_instance_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_task_instance_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_task_instance_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_task_instance_reference.py` & `apache_airflow_client-2.9.0rc1/test/test_task_instance_reference.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_task_instance_reference_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_task_instance_reference_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_task_outlet_dataset_reference.py` & `apache_airflow_client-2.9.0rc1/test/test_task_outlet_dataset_reference.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_task_state.py` & `apache_airflow_client-2.9.0rc1/test/test_task_state.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_time_delta.py` & `apache_airflow_client-2.9.0rc1/test/test_time_delta.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_trigger.py` & `apache_airflow_client-2.9.0rc1/test/test_trigger.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_trigger_rule.py` & `apache_airflow_client-2.9.0rc1/test/test_trigger_rule.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_triggerer_status.py` & `apache_airflow_client-2.9.0rc1/test/test_triggerer_status.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_update_dag_run_state.py` & `apache_airflow_client-2.9.0rc1/test/test_update_dag_run_state.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_update_task_instance.py` & `apache_airflow_client-2.9.0rc1/test/test_update_task_instance.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_update_task_instances_state.py` & `apache_airflow_client-2.9.0rc1/test/test_update_task_instances_state.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_update_task_state.py` & `apache_airflow_client-2.9.0rc1/test/test_update_task_state.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_user.py` & `apache_airflow_client-2.9.0rc1/test/test_user.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_user_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_user_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_user_api.py` & `apache_airflow_client-2.9.0rc1/test/test_user_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_user_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_user_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_user_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_user_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_user_collection_item.py` & `apache_airflow_client-2.9.0rc1/test/test_user_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_user_collection_item_roles.py` & `apache_airflow_client-2.9.0rc1/test/test_user_collection_item_roles.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_variable.py` & `apache_airflow_client-2.9.0rc1/test/test_variable.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_variable_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_variable_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_variable_api.py` & `apache_airflow_client-2.9.0rc1/test/test_variable_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_variable_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_variable_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_variable_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_variable_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_variable_collection_item.py` & `apache_airflow_client-2.9.0rc1/test/test_variable_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_version_info.py` & `apache_airflow_client-2.9.0rc1/test/test_version_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_weight_rule.py` & `apache_airflow_client-2.9.0rc1/test/test_weight_rule.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_x_com.py` & `apache_airflow_client-2.9.0rc1/test/test_x_com.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_x_com_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_x_com_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_x_com_api.py` & `apache_airflow_client-2.9.0rc1/test/test_x_com_api.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_x_com_collection.py` & `apache_airflow_client-2.9.0rc1/test/test_x_com_collection.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_x_com_collection_all_of.py` & `apache_airflow_client-2.9.0rc1/test/test_x_com_collection_all_of.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/test/test_x_com_collection_item.py` & `apache_airflow_client-2.9.0rc1/test/test_x_com_collection_item.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/LICENSE` & `apache_airflow_client-2.9.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/README.md` & `apache_airflow_client-2.9.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/pyproject.toml` & `apache_airflow_client-2.9.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache_airflow_client-2.9.0/PKG-INFO` & `apache_airflow_client-2.9.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: apache-airflow-client
-Version: 2.9.0
+Version: 2.9.0rc1
 Summary: Apache Airflow API (Stable)
 Project-URL: Bug Tracker, https://github.com/apache/airflow-client-python/issues
 Project-URL: Changelog, https://github.com/apache/airflow-client-python/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow/stable/stable-rest-api-ref.html
 Project-URL: Download, https://archive.apache.org/dist/airflow/clients/python/
 Project-URL: Homepage, https://airflow.apache.org/
 Project-URL: Source Code, https://github.com/apache/airflow/clients/python
```

