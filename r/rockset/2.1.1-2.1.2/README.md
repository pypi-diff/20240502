# Comparing `tmp/rockset-2.1.1.tar.gz` & `tmp/rockset-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockset-2.1.1.tar", max compression
+gzip compressed data, was "rockset-2.1.2.tar", max compression
```

## Comparing `rockset-2.1.1.tar` & `rockset-2.1.2.tar`

### file list

```diff
@@ -1,267 +1,273 @@
--rw-r--r--   0        0        0      357 2023-07-10 18:55:10.858843 rockset-2.1.1/LONG_DESCRIPTION.rst
--rw-r--r--   0        0        0     1616 2024-02-22 19:14:01.701867 rockset-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     1338 2023-12-19 06:10:46.211687 rockset-2.1.1/rockset/__init__.py
--rw-r--r--   0        0        0      208 2023-12-19 06:10:46.211687 rockset-2.1.1/rockset/api/__init__.py
--rw-r--r--   0        0        0    34696 2023-12-19 06:10:46.287687 rockset-2.1.1/rockset/api/aliases_api.py
--rw-r--r--   0        0        0    30366 2023-12-19 06:10:46.279687 rockset-2.1.1/rockset/api/api_keys_api.py
--rw-r--r--   0        0        0   121161 2023-12-19 06:10:46.279687 rockset-2.1.1/rockset/api/collections_api.py
--rw-r--r--   0        0        0    28165 2023-12-19 06:10:46.279687 rockset-2.1.1/rockset/api/custom_roles_api.py
--rw-r--r--   0        0        0    21187 2023-12-19 06:10:46.283687 rockset-2.1.1/rockset/api/documents_api.py
--rw-r--r--   0        0        0    85470 2023-12-19 06:10:46.283687 rockset-2.1.1/rockset/api/integrations_api.py
--rw-r--r--   0        0        0     6168 2023-12-19 06:10:46.287687 rockset-2.1.1/rockset/api/organizations_api.py
--rw-r--r--   0        0        0    38385 2023-12-19 06:10:46.283687 rockset-2.1.1/rockset/api/queries_api.py
--rw-r--r--   0        0        0    87753 2023-12-19 06:10:46.283687 rockset-2.1.1/rockset/api/query_lambdas_api.py
--rw-r--r--   0        0        0    22493 2023-12-19 06:10:46.279687 rockset-2.1.1/rockset/api/scheduled_lambdas_api.py
--rw-r--r--   0        0        0     7687 2023-12-19 06:10:46.279687 rockset-2.1.1/rockset/api/shared_lambdas_api.py
--rw-r--r--   0        0        0   110948 2023-12-19 06:10:46.283687 rockset-2.1.1/rockset/api/sources_api.py
--rw-r--r--   0        0        0    43268 2023-12-19 06:10:46.283687 rockset-2.1.1/rockset/api/users_api.py
--rw-r--r--   0        0        0    34441 2023-12-19 06:10:46.287687 rockset-2.1.1/rockset/api/views_api.py
--rw-r--r--   0        0        0    86893 2023-12-19 06:10:46.283687 rockset-2.1.1/rockset/api/virtual_instances_api.py
--rw-r--r--   0        0        0    22087 2023-12-19 06:10:46.283687 rockset-2.1.1/rockset/api/workspaces_api.py
--rw-r--r--   0        0        0    36393 2023-12-19 06:10:46.215687 rockset-2.1.1/rockset/api_client.py
--rw-r--r--   0        0        0     1219 2023-12-19 06:10:46.223687 rockset-2.1.1/rockset/apis/__init__.py
--rw-r--r--   0        0        0    15516 2023-12-19 06:10:46.211687 rockset-2.1.1/rockset/configuration.py
--rw-r--r--   0        0        0     3831 2023-07-10 18:55:10.862843 rockset-2.1.1/rockset/document.py
--rw-r--r--   0        0        0     6072 2023-12-19 06:10:46.215687 rockset-2.1.1/rockset/exceptions.py
--rw-r--r--   0        0        0      348 2023-12-19 06:10:46.223687 rockset-2.1.1/rockset/model/__init__.py
--rw-r--r--   0        0        0    11950 2023-12-19 06:10:44.935685 rockset-2.1.1/rockset/model/add_documents_request.py
--rw-r--r--   0        0        0    12291 2023-12-19 06:10:44.951686 rockset-2.1.1/rockset/model/add_documents_response.py
--rw-r--r--   0        0        0    14049 2023-12-19 06:10:44.967686 rockset-2.1.1/rockset/model/alias.py
--rw-r--r--   0        0        0    14557 2023-12-19 06:10:44.979686 rockset-2.1.1/rockset/model/api_key.py
--rw-r--r--   0        0        0    14462 2023-12-19 06:10:44.987686 rockset-2.1.1/rockset/model/async_query_options.py
--rw-r--r--   0        0        0    13796 2023-12-19 06:10:44.995686 rockset-2.1.1/rockset/model/auto_scaling_policy.py
--rw-r--r--   0        0        0    12229 2023-12-19 06:10:45.003686 rockset-2.1.1/rockset/model/aws_access_key.py
--rw-r--r--   0        0        0    12101 2023-12-19 06:10:45.015686 rockset-2.1.1/rockset/model/aws_role.py
--rw-r--r--   0        0        0    15709 2023-12-19 06:10:45.019686 rockset-2.1.1/rockset/model/azure_blob_storage_collection_creation_request.py
--rw-r--r--   0        0        0    11893 2023-12-19 06:10:45.027685 rockset-2.1.1/rockset/model/azure_blob_storage_integration.py
--rw-r--r--   0        0        0    12616 2023-12-19 06:10:45.031686 rockset-2.1.1/rockset/model/azure_blob_storage_integration_creation_request.py
--rw-r--r--   0        0        0    14536 2023-12-19 06:10:45.039686 rockset-2.1.1/rockset/model/azure_blob_storage_source_wrapper.py
--rw-r--r--   0        0        0    15689 2023-12-19 06:10:45.051686 rockset-2.1.1/rockset/model/azure_event_hubs_collection_creation_request.py
--rw-r--r--   0        0        0    11787 2023-12-19 06:10:45.059686 rockset-2.1.1/rockset/model/azure_event_hubs_integration.py
--rw-r--r--   0        0        0    12586 2023-12-19 06:10:45.067686 rockset-2.1.1/rockset/model/azure_event_hubs_integration_creation_request.py
--rw-r--r--   0        0        0    13452 2023-12-19 06:10:45.075686 rockset-2.1.1/rockset/model/azure_event_hubs_source_wrapper.py
--rw-r--r--   0        0        0    15062 2023-07-10 21:58:00.859999 rockset-2.1.1/rockset/model/azure_service_bus_collection_creation_request.py
--rw-r--r--   0        0        0    11888 2023-12-19 06:10:45.083686 rockset-2.1.1/rockset/model/azure_service_bus_integration.py
--rw-r--r--   0        0        0    13333 2023-07-10 21:58:00.871999 rockset-2.1.1/rockset/model/azure_service_bus_source_wrapper.py
--rw-r--r--   0        0        0    18743 2023-12-19 06:10:45.087686 rockset-2.1.1/rockset/model/bulk_stats.py
--rw-r--r--   0        0        0    11798 2023-12-19 06:10:45.095686 rockset-2.1.1/rockset/model/cancel_query_response.py
--rw-r--r--   0        0        0    13225 2023-12-19 06:10:45.099686 rockset-2.1.1/rockset/model/cluster.py
--rw-r--r--   0        0        0    18893 2023-12-19 06:10:45.107686 rockset-2.1.1/rockset/model/collection.py
--rw-r--r--   0        0        0    14847 2023-12-19 06:10:45.115686 rockset-2.1.1/rockset/model/collection_mount.py
--rw-r--r--   0        0        0    11852 2023-12-19 06:10:45.123686 rockset-2.1.1/rockset/model/collection_mount_response.py
--rw-r--r--   0        0        0    11772 2023-12-19 06:10:45.131686 rockset-2.1.1/rockset/model/collection_mount_stats.py
--rw-r--r--   0        0        0    16965 2023-12-19 06:10:45.135686 rockset-2.1.1/rockset/model/collection_stats.py
--rw-r--r--   0        0        0    12333 2023-12-19 06:10:45.147686 rockset-2.1.1/rockset/model/create_alias_request.py
--rw-r--r--   0        0        0    11769 2023-12-19 06:10:45.151686 rockset-2.1.1/rockset/model/create_alias_response.py
--rw-r--r--   0        0        0    12525 2023-12-19 06:10:45.159686 rockset-2.1.1/rockset/model/create_api_key_request.py
--rw-r--r--   0        0        0    11780 2023-12-19 06:10:45.163686 rockset-2.1.1/rockset/model/create_api_key_response.py
--rw-r--r--   0        0        0    11765 2023-12-19 06:10:45.167686 rockset-2.1.1/rockset/model/create_collection_mount_request.py
--rw-r--r--   0        0        0    11913 2023-12-19 06:10:45.171686 rockset-2.1.1/rockset/model/create_collection_mounts_response.py
--rw-r--r--   0        0        0    15091 2023-12-19 06:10:45.179686 rockset-2.1.1/rockset/model/create_collection_request.py
--rw-r--r--   0        0        0    11819 2023-12-19 06:10:45.183686 rockset-2.1.1/rockset/model/create_collection_response.py
--rw-r--r--   0        0        0    16037 2023-12-19 06:10:45.191686 rockset-2.1.1/rockset/model/create_integration_request.py
--rw-r--r--   0        0        0    11829 2023-12-19 06:10:45.195686 rockset-2.1.1/rockset/model/create_integration_response.py
--rw-r--r--   0        0        0    12571 2023-12-19 06:10:45.199686 rockset-2.1.1/rockset/model/create_query_lambda_request.py
--rw-r--r--   0        0        0    12063 2023-12-19 06:10:45.203686 rockset-2.1.1/rockset/model/create_query_lambda_tag_request.py
--rw-r--r--   0        0        0    12501 2023-12-19 06:10:45.207686 rockset-2.1.1/rockset/model/create_role_request.py
--rw-r--r--   0        0        0    14922 2023-12-19 06:10:45.211686 rockset-2.1.1/rockset/model/create_scheduled_lambda_request.py
--rw-r--r--   0        0        0    12479 2023-12-19 06:10:45.215686 rockset-2.1.1/rockset/model/create_user_request.py
--rw-r--r--   0        0        0    11759 2023-12-19 06:10:45.219686 rockset-2.1.1/rockset/model/create_user_response.py
--rw-r--r--   0        0        0    12170 2023-12-19 06:10:45.223686 rockset-2.1.1/rockset/model/create_view_request.py
--rw-r--r--   0        0        0    11759 2023-12-19 06:10:45.227686 rockset-2.1.1/rockset/model/create_view_response.py
--rw-r--r--   0        0        0    15539 2023-12-19 06:10:45.231686 rockset-2.1.1/rockset/model/create_virtual_instance_request.py
--rw-r--r--   0        0        0    11870 2023-12-19 06:10:45.235686 rockset-2.1.1/rockset/model/create_virtual_instance_response.py
--rw-r--r--   0        0        0    12038 2023-12-19 06:10:45.239686 rockset-2.1.1/rockset/model/create_workspace_request.py
--rw-r--r--   0        0        0    11809 2023-12-19 06:10:45.243686 rockset-2.1.1/rockset/model/create_workspace_response.py
--rw-r--r--   0        0        0    14179 2023-12-19 06:10:45.247686 rockset-2.1.1/rockset/model/csv_params.py
--rw-r--r--   0        0        0    11769 2023-12-19 06:10:45.251686 rockset-2.1.1/rockset/model/delete_alias_response.py
--rw-r--r--   0        0        0    11780 2023-12-19 06:10:45.255686 rockset-2.1.1/rockset/model/delete_api_key_response.py
--rw-r--r--   0        0        0    11819 2023-12-19 06:10:45.259686 rockset-2.1.1/rockset/model/delete_collection_response.py
--rw-r--r--   0        0        0    12036 2023-12-19 06:10:45.263686 rockset-2.1.1/rockset/model/delete_documents_request.py
--rw-r--r--   0        0        0    11686 2023-12-19 06:10:45.263686 rockset-2.1.1/rockset/model/delete_documents_request_data.py
--rw-r--r--   0        0        0    12300 2023-12-19 06:10:45.267686 rockset-2.1.1/rockset/model/delete_documents_response.py
--rw-r--r--   0        0        0    11829 2023-12-19 06:10:45.271686 rockset-2.1.1/rockset/model/delete_integration_response.py
--rw-r--r--   0        0        0    11830 2023-12-19 06:10:45.275686 rockset-2.1.1/rockset/model/delete_query_lambda_response.py
--rw-r--r--   0        0        0    11779 2023-12-19 06:10:45.279686 rockset-2.1.1/rockset/model/delete_source_response.py
--rw-r--r--   0        0        0    11759 2023-12-19 06:10:45.283686 rockset-2.1.1/rockset/model/delete_user_response.py
--rw-r--r--   0        0        0    11759 2023-12-19 06:10:45.287686 rockset-2.1.1/rockset/model/delete_view_response.py
--rw-r--r--   0        0        0    11870 2023-12-19 06:10:45.287686 rockset-2.1.1/rockset/model/delete_virtual_instance_response.py
--rw-r--r--   0        0        0    11809 2023-12-19 06:10:45.291686 rockset-2.1.1/rockset/model/delete_workspace_response.py
--rw-r--r--   0        0        0    13023 2023-12-19 06:10:45.295686 rockset-2.1.1/rockset/model/document_status.py
--rw-r--r--   0        0        0    15627 2023-12-19 06:10:45.303686 rockset-2.1.1/rockset/model/dynamodb_collection_creation_request.py
--rw-r--r--   0        0        0    12563 2023-12-19 06:10:45.307686 rockset-2.1.1/rockset/model/dynamodb_integration.py
--rw-r--r--   0        0        0    12484 2023-12-19 06:10:45.311686 rockset-2.1.1/rockset/model/dynamodb_integration_creation_request.py
--rw-r--r--   0        0        0    14861 2023-12-19 06:10:45.315686 rockset-2.1.1/rockset/model/dynamodb_source_wrapper.py
--rw-r--r--   0        0        0    14548 2023-12-19 06:10:45.319686 rockset-2.1.1/rockset/model/error_model.py
--rw-r--r--   0        0        0    12392 2023-12-19 06:10:45.323686 rockset-2.1.1/rockset/model/event_time_info.py
--rw-r--r--   0        0        0    12338 2023-12-19 06:10:45.327686 rockset-2.1.1/rockset/model/execute_public_query_lambda_request.py
--rw-r--r--   0        0        0    17858 2023-12-19 06:10:45.331686 rockset-2.1.1/rockset/model/execute_query_lambda_request.py
--rw-r--r--   0        0        0    12093 2023-12-19 06:10:45.331686 rockset-2.1.1/rockset/model/execution_status.py
--rw-r--r--   0        0        0    11743 2023-12-19 06:10:45.335686 rockset-2.1.1/rockset/model/field_mapping_query.py
--rw-r--r--   0        0        0    13075 2023-12-19 06:10:45.339686 rockset-2.1.1/rockset/model/field_mapping_v2.py
--rw-r--r--   0        0        0    12543 2023-12-19 06:10:45.343686 rockset-2.1.1/rockset/model/field_partition.py
--rw-r--r--   0        0        0    15063 2023-07-10 18:55:10.866843 rockset-2.1.1/rockset/model/file_upload_collection_creation_request.py
--rw-r--r--   0        0        0    13611 2023-07-10 18:55:10.866843 rockset-2.1.1/rockset/model/file_upload_source_wrapper.py
--rw-r--r--   0        0        0    13393 2023-12-19 06:10:45.347686 rockset-2.1.1/rockset/model/format_params.py
--rw-r--r--   0        0        0    12001 2023-12-19 06:10:45.347686 rockset-2.1.1/rockset/model/gcp_service_account.py
--rw-r--r--   0        0        0    15577 2023-12-19 06:10:45.355686 rockset-2.1.1/rockset/model/gcs_collection_creation_request.py
--rw-r--r--   0        0        0    11915 2023-12-19 06:10:45.355686 rockset-2.1.1/rockset/model/gcs_integration.py
--rw-r--r--   0        0        0    12409 2023-12-19 06:10:45.359686 rockset-2.1.1/rockset/model/gcs_integration_creation_request.py
--rw-r--r--   0        0        0    14681 2023-12-19 06:10:45.363686 rockset-2.1.1/rockset/model/gcs_source_wrapper.py
--rw-r--r--   0        0        0    11760 2023-12-19 06:10:45.367686 rockset-2.1.1/rockset/model/get_alias_response.py
--rw-r--r--   0        0        0    11771 2023-12-19 06:10:45.371686 rockset-2.1.1/rockset/model/get_api_key_response.py
--rw-r--r--   0        0        0    12194 2023-12-19 06:10:45.375686 rockset-2.1.1/rockset/model/get_collection_commit.py
--rw-r--r--   0        0        0    12318 2023-12-19 06:10:45.375686 rockset-2.1.1/rockset/model/get_collection_commit_data.py
--rw-r--r--   0        0        0    11751 2023-12-19 06:10:45.379686 rockset-2.1.1/rockset/model/get_collection_commit_request.py
--rw-r--r--   0        0        0    11810 2023-12-19 06:10:45.383686 rockset-2.1.1/rockset/model/get_collection_response.py
--rw-r--r--   0        0        0    11820 2023-12-19 06:10:45.387686 rockset-2.1.1/rockset/model/get_integration_response.py
--rw-r--r--   0        0        0    11789 2023-12-19 06:10:45.387686 rockset-2.1.1/rockset/model/get_query_response.py
--rw-r--r--   0        0        0    11770 2023-12-19 06:10:45.391686 rockset-2.1.1/rockset/model/get_source_response.py
--rw-r--r--   0        0        0    11750 2023-12-19 06:10:45.395686 rockset-2.1.1/rockset/model/get_view_response.py
--rw-r--r--   0        0        0    11861 2023-12-19 06:10:45.399686 rockset-2.1.1/rockset/model/get_virtual_instance_response.py
--rw-r--r--   0        0        0    11800 2023-12-19 06:10:45.403686 rockset-2.1.1/rockset/model/get_workspace_response.py
--rw-r--r--   0        0        0    12704 2023-12-19 06:10:45.403686 rockset-2.1.1/rockset/model/input_field.py
--rw-r--r--   0        0        0    17788 2023-12-19 06:10:45.407686 rockset-2.1.1/rockset/model/integration.py
--rw-r--r--   0        0        0    15597 2023-12-19 06:10:45.411686 rockset-2.1.1/rockset/model/kafka_collection_creation_request.py
--rw-r--r--   0        0        0    14826 2023-12-19 06:10:45.415686 rockset-2.1.1/rockset/model/kafka_integration.py
--rw-r--r--   0        0        0    12439 2023-12-19 06:10:45.419686 rockset-2.1.1/rockset/model/kafka_integration_creation_request.py
--rw-r--r--   0        0        0    14319 2023-12-19 06:10:45.423686 rockset-2.1.1/rockset/model/kafka_source_wrapper.py
--rw-r--r--   0        0        0    11845 2023-12-19 06:10:45.423686 rockset-2.1.1/rockset/model/kafka_v3_security_config.py
--rw-r--r--   0        0        0    15617 2023-12-19 06:10:45.427686 rockset-2.1.1/rockset/model/kinesis_collection_creation_request.py
--rw-r--r--   0        0        0    12169 2023-12-19 06:10:45.431686 rockset-2.1.1/rockset/model/kinesis_integration.py
--rw-r--r--   0        0        0    12469 2023-12-19 06:10:45.435686 rockset-2.1.1/rockset/model/kinesis_integration_creation_request.py
--rw-r--r--   0        0        0    13895 2023-12-19 06:10:45.439686 rockset-2.1.1/rockset/model/kinesis_source_wrapper.py
--rw-r--r--   0        0        0    11819 2023-12-19 06:10:45.443686 rockset-2.1.1/rockset/model/list_aliases_response.py
--rw-r--r--   0        0        0    11835 2023-12-19 06:10:45.443686 rockset-2.1.1/rockset/model/list_api_keys_response.py
--rw-r--r--   0        0        0    11937 2023-12-19 06:10:45.447686 rockset-2.1.1/rockset/model/list_collection_mounts_response.py
--rw-r--r--   0        0        0    11874 2023-12-19 06:10:45.451686 rockset-2.1.1/rockset/model/list_collections_response.py
--rw-r--r--   0        0        0    11892 2023-12-19 06:10:45.455686 rockset-2.1.1/rockset/model/list_integrations_response.py
--rw-r--r--   0        0        0    11804 2023-12-19 06:10:45.455686 rockset-2.1.1/rockset/model/list_queries_response.py
--rw-r--r--   0        0        0    11964 2023-12-19 06:10:45.459686 rockset-2.1.1/rockset/model/list_query_lambda_tags_response.py
--rw-r--r--   0        0        0    12010 2023-12-19 06:10:45.463686 rockset-2.1.1/rockset/model/list_query_lambda_versions_response.py
--rw-r--r--   0        0        0    11889 2023-12-19 06:10:45.467686 rockset-2.1.1/rockset/model/list_query_lambdas_response.py
--rw-r--r--   0        0        0    11802 2023-12-19 06:10:45.467686 rockset-2.1.1/rockset/model/list_roles_response.py
--rw-r--r--   0        0        0    11856 2023-12-19 06:10:45.471686 rockset-2.1.1/rockset/model/list_sources_response.py
--rw-r--r--   0        0        0    12003 2023-12-19 06:10:45.475686 rockset-2.1.1/rockset/model/list_unsubscribe_preferences_response.py
--rw-r--r--   0        0        0    11794 2023-12-19 06:10:45.479686 rockset-2.1.1/rockset/model/list_users_response.py
--rw-r--r--   0        0        0    11802 2023-12-19 06:10:45.479686 rockset-2.1.1/rockset/model/list_views_response.py
--rw-r--r--   0        0        0    11937 2023-12-19 06:10:45.483686 rockset-2.1.1/rockset/model/list_virtual_instances_response.py
--rw-r--r--   0        0        0    11854 2023-12-19 06:10:45.487686 rockset-2.1.1/rockset/model/list_workspaces_response.py
--rw-r--r--   0        0        0    12170 2023-12-19 06:10:45.491686 rockset-2.1.1/rockset/model/mongo_db_integration.py
--rw-r--r--   0        0        0    15617 2023-12-19 06:10:45.495686 rockset-2.1.1/rockset/model/mongodb_collection_creation_request.py
--rw-r--r--   0        0        0    12470 2023-12-19 06:10:45.495686 rockset-2.1.1/rockset/model/mongodb_integration_creation_request.py
--rw-r--r--   0        0        0    14123 2023-12-19 06:10:45.499686 rockset-2.1.1/rockset/model/mongodb_source_wrapper.py
--rw-r--r--   0        0        0    11918 2023-12-19 06:10:45.503686 rockset-2.1.1/rockset/model/offsets.py
--rw-r--r--   0        0        0    13910 2023-12-19 06:10:45.507686 rockset-2.1.1/rockset/model/organization.py
--rw-r--r--   0        0        0    11821 2023-12-19 06:10:45.507686 rockset-2.1.1/rockset/model/organization_response.py
--rw-r--r--   0        0        0    12527 2023-12-19 06:10:45.511686 rockset-2.1.1/rockset/model/output_field.py
--rw-r--r--   0        0        0    11775 2023-12-19 06:10:45.515686 rockset-2.1.1/rockset/model/pagination.py
--rw-r--r--   0        0        0    13055 2023-12-19 06:10:45.519686 rockset-2.1.1/rockset/model/pagination_info.py
--rw-r--r--   0        0        0    12155 2023-12-19 06:10:45.519686 rockset-2.1.1/rockset/model/patch_document.py
--rw-r--r--   0        0        0    11920 2023-12-19 06:10:45.523686 rockset-2.1.1/rockset/model/patch_documents_request.py
--rw-r--r--   0        0        0    12237 2023-12-19 06:10:45.527686 rockset-2.1.1/rockset/model/patch_documents_response.py
--rw-r--r--   0        0        0    13672 2023-12-19 06:10:45.531686 rockset-2.1.1/rockset/model/patch_operation.py
--rw-r--r--   0        0        0    16196 2023-12-19 06:10:45.531686 rockset-2.1.1/rockset/model/privilege.py
--rw-r--r--   0        0        0    12407 2023-12-19 06:10:45.535686 rockset-2.1.1/rockset/model/query_error.py
--rw-r--r--   0        0        0    11907 2023-12-19 06:10:45.539686 rockset-2.1.1/rockset/model/query_field_type.py
--rw-r--r--   0        0        0    14972 2023-12-19 06:10:45.539686 rockset-2.1.1/rockset/model/query_info.py
--rw-r--r--   0        0        0    13688 2023-12-19 06:10:45.543686 rockset-2.1.1/rockset/model/query_lambda.py
--rw-r--r--   0        0        0    12219 2023-12-19 06:10:45.547686 rockset-2.1.1/rockset/model/query_lambda_sql.py
--rw-r--r--   0        0        0    12786 2023-12-19 06:10:45.547686 rockset-2.1.1/rockset/model/query_lambda_stats.py
--rw-r--r--   0        0        0    12124 2023-12-19 06:10:45.551686 rockset-2.1.1/rockset/model/query_lambda_tag.py
--rw-r--r--   0        0        0    11843 2023-12-19 06:10:45.555686 rockset-2.1.1/rockset/model/query_lambda_tag_response.py
--rw-r--r--   0        0        0    15267 2023-12-19 06:10:45.555686 rockset-2.1.1/rockset/model/query_lambda_version.py
--rw-r--r--   0        0        0    11883 2023-12-19 06:10:45.559686 rockset-2.1.1/rockset/model/query_lambda_version_response.py
--rw-r--r--   0        0        0    13051 2023-07-10 18:55:10.866843 rockset-2.1.1/rockset/model/query_pagination_response.py
--rw-r--r--   0        0        0    12188 2023-12-19 06:10:45.563686 rockset-2.1.1/rockset/model/query_parameter.py
--rw-r--r--   0        0        0    15940 2023-12-19 06:10:45.567686 rockset-2.1.1/rockset/model/query_request.py
--rw-r--r--   0        0        0    13270 2023-12-19 06:10:45.567686 rockset-2.1.1/rockset/model/query_request_sql.py
--rw-r--r--   0        0        0    16189 2023-07-10 18:55:10.866843 rockset-2.1.1/rockset/model/query_response.py
--rw-r--r--   0        0        0    12105 2023-12-19 06:10:45.571686 rockset-2.1.1/rockset/model/query_response_stats.py
--rw-r--r--   0        0        0    11870 2023-12-19 06:10:45.575686 rockset-2.1.1/rockset/model/resume_virtual_instance_response.py
--rw-r--r--   0        0        0    13363 2023-12-19 06:10:45.579686 rockset-2.1.1/rockset/model/role.py
--rw-r--r--   0        0        0    11741 2023-12-19 06:10:45.579686 rockset-2.1.1/rockset/model/role_response.py
--rw-r--r--   0        0        0    15567 2023-12-19 06:10:45.583686 rockset-2.1.1/rockset/model/s3_collection_creation_request.py
--rw-r--r--   0        0        0    12154 2023-12-19 06:10:45.587686 rockset-2.1.1/rockset/model/s3_integration.py
--rw-r--r--   0        0        0    12394 2023-12-19 06:10:45.591686 rockset-2.1.1/rockset/model/s3_integration_creation_request.py
--rw-r--r--   0        0        0    15273 2023-12-19 06:10:45.591686 rockset-2.1.1/rockset/model/s3_source_wrapper.py
--rw-r--r--   0        0        0    17506 2023-12-19 06:10:45.595686 rockset-2.1.1/rockset/model/scheduled_lambda.py
--rw-r--r--   0        0        0    11852 2023-12-19 06:10:45.599686 rockset-2.1.1/rockset/model/scheduled_lambda_response.py
--rw-r--r--   0        0        0    12201 2023-12-19 06:10:45.599686 rockset-2.1.1/rockset/model/schema_registry_config.py
--rw-r--r--   0        0        0    11696 2023-07-10 18:55:10.866843 rockset-2.1.1/rockset/model/segment_integration.py
--rw-r--r--   0        0        0    12465 2023-07-10 18:55:10.866843 rockset-2.1.1/rockset/model/segment_integration_creation_request.py
--rw-r--r--   0        0        0    15637 2023-12-19 06:10:45.603686 rockset-2.1.1/rockset/model/snowflake_collection_creation_request.py
--rw-r--r--   0        0        0    14450 2023-12-19 06:10:45.607686 rockset-2.1.1/rockset/model/snowflake_integration.py
--rw-r--r--   0        0        0    12499 2023-12-19 06:10:45.611686 rockset-2.1.1/rockset/model/snowflake_integration_creation_request.py
--rw-r--r--   0        0        0    13907 2023-12-19 06:10:45.615686 rockset-2.1.1/rockset/model/snowflake_source_wrapper.py
--rw-r--r--   0        0        0    18381 2023-12-19 06:10:45.615686 rockset-2.1.1/rockset/model/source.py
--rw-r--r--   0        0        0    11959 2023-12-19 06:10:45.619686 rockset-2.1.1/rockset/model/source_az_blob_storage_base.py
--rw-r--r--   0        0        0    12723 2023-12-19 06:10:45.623686 rockset-2.1.1/rockset/model/source_az_blob_storage_settings.py
--rw-r--r--   0        0        0    13678 2023-12-19 06:10:45.627686 rockset-2.1.1/rockset/model/source_azure_blob_storage.py
--rw-r--r--   0        0        0    12664 2023-12-19 06:10:45.631686 rockset-2.1.1/rockset/model/source_azure_event_hubs.py
--rw-r--r--   0        0        0    12552 2023-12-19 06:10:45.631686 rockset-2.1.1/rockset/model/source_azure_service_bus.py
--rw-r--r--   0        0        0    12951 2023-12-19 06:10:45.635686 rockset-2.1.1/rockset/model/source_base.py
--rw-r--r--   0        0        0    14033 2023-12-19 06:10:45.639686 rockset-2.1.1/rockset/model/source_dynamo_db.py
--rw-r--r--   0        0        0    11908 2023-12-19 06:10:45.643686 rockset-2.1.1/rockset/model/source_dynamo_db_base.py
--rw-r--r--   0        0        0    12989 2023-12-19 06:10:45.647686 rockset-2.1.1/rockset/model/source_dynamo_db_settings.py
--rw-r--r--   0        0        0    12391 2023-12-19 06:10:45.651687 rockset-2.1.1/rockset/model/source_file_upload.py
--rw-r--r--   0        0        0    13808 2023-12-19 06:10:45.651687 rockset-2.1.1/rockset/model/source_gcs.py
--rw-r--r--   0        0        0    11857 2023-12-19 06:10:45.655686 rockset-2.1.1/rockset/model/source_gcs_base.py
--rw-r--r--   0        0        0    12640 2023-12-19 06:10:45.659686 rockset-2.1.1/rockset/model/source_gcs_settings.py
--rw-r--r--   0        0        0    13488 2023-12-19 06:10:45.663686 rockset-2.1.1/rockset/model/source_kafka.py
--rw-r--r--   0        0        0    13024 2023-12-19 06:10:45.663686 rockset-2.1.1/rockset/model/source_kinesis.py
--rw-r--r--   0        0        0    13315 2023-12-19 06:10:45.667686 rockset-2.1.1/rockset/model/source_mongo_db.py
--rw-r--r--   0        0        0    14379 2023-12-19 06:10:45.671687 rockset-2.1.1/rockset/model/source_s3.py
--rw-r--r--   0        0        0    11847 2023-12-19 06:10:45.671687 rockset-2.1.1/rockset/model/source_s3_base.py
--rw-r--r--   0        0        0    12632 2023-12-19 06:10:45.675686 rockset-2.1.1/rockset/model/source_s3_settings.py
--rw-r--r--   0        0        0    12274 2023-12-19 06:10:45.679686 rockset-2.1.1/rockset/model/source_snapshot.py
--rw-r--r--   0        0        0    13110 2023-12-19 06:10:45.683686 rockset-2.1.1/rockset/model/source_snowflake.py
--rw-r--r--   0        0        0    12384 2023-12-19 06:10:45.683686 rockset-2.1.1/rockset/model/source_system.py
--rw-r--r--   0        0        0    11661 2023-12-19 06:10:45.687687 rockset-2.1.1/rockset/model/sql_expression.py
--rw-r--r--   0        0        0    13116 2023-12-19 06:10:45.691686 rockset-2.1.1/rockset/model/stats.py
--rw-r--r--   0        0        0    13696 2023-12-19 06:10:45.691686 rockset-2.1.1/rockset/model/status.py
--rw-r--r--   0        0        0    13111 2023-12-19 06:10:45.695686 rockset-2.1.1/rockset/model/status_azure_event_hubs.py
--rw-r--r--   0        0        0    12364 2023-12-19 06:10:45.699686 rockset-2.1.1/rockset/model/status_azure_event_hubs_partition.py
--rw-r--r--   0        0        0    12727 2023-12-19 06:10:45.699686 rockset-2.1.1/rockset/model/status_azure_service_bus.py
--rw-r--r--   0        0        0    12210 2023-12-19 06:10:45.703687 rockset-2.1.1/rockset/model/status_azure_service_bus_session.py
--rw-r--r--   0        0        0    13563 2023-12-19 06:10:45.707687 rockset-2.1.1/rockset/model/status_dynamo_db.py
--rw-r--r--   0        0        0    12705 2023-12-19 06:10:45.707687 rockset-2.1.1/rockset/model/status_dynamo_db_v2.py
--rw-r--r--   0        0        0    13123 2023-12-19 06:10:45.711686 rockset-2.1.1/rockset/model/status_kafka.py
--rw-r--r--   0        0        0    12337 2023-12-19 06:10:45.715686 rockset-2.1.1/rockset/model/status_kafka_partition.py
--rw-r--r--   0        0        0    15614 2023-12-19 06:10:45.715686 rockset-2.1.1/rockset/model/status_mongo_db.py
--rw-r--r--   0        0        0    11924 2023-12-19 06:10:45.719687 rockset-2.1.1/rockset/model/status_snowflake.py
--rw-r--r--   0        0        0    11808 2023-12-19 06:10:45.723687 rockset-2.1.1/rockset/model/suspend_source_request.py
--rw-r--r--   0        0        0    11873 2023-12-19 06:10:45.723687 rockset-2.1.1/rockset/model/suspend_virtual_instance_response.py
--rw-r--r--   0        0        0    13338 2023-12-19 06:10:45.727687 rockset-2.1.1/rockset/model/tls_config.py
--rw-r--r--   0        0        0    11894 2023-12-19 06:10:45.731686 rockset-2.1.1/rockset/model/unsubscribe_preference.py
--rw-r--r--   0        0        0    12119 2023-12-19 06:10:45.731686 rockset-2.1.1/rockset/model/update_alias_request.py
--rw-r--r--   0        0        0    12635 2023-12-19 06:10:45.735687 rockset-2.1.1/rockset/model/update_api_key_request.py
--rw-r--r--   0        0        0    11780 2023-12-19 06:10:45.739687 rockset-2.1.1/rockset/model/update_api_key_response.py
--rw-r--r--   0        0        0    12247 2023-12-19 06:10:45.743687 rockset-2.1.1/rockset/model/update_collection_request.py
--rw-r--r--   0        0        0    15791 2023-12-19 06:10:45.743687 rockset-2.1.1/rockset/model/update_integration_request.py
--rw-r--r--   0        0        0    11829 2023-12-19 06:10:45.747686 rockset-2.1.1/rockset/model/update_integration_response.py
--rw-r--r--   0        0        0    12329 2023-12-19 06:10:45.751686 rockset-2.1.1/rockset/model/update_query_lambda_request.py
--rw-r--r--   0        0        0    12222 2023-12-19 06:10:45.751686 rockset-2.1.1/rockset/model/update_role_request.py
--rw-r--r--   0        0        0    14031 2023-12-19 06:10:45.755687 rockset-2.1.1/rockset/model/update_scheduled_lambda_request.py
--rw-r--r--   0        0        0    12006 2023-12-19 06:10:45.759687 rockset-2.1.1/rockset/model/update_unsubscribe_preferences_request.py
--rw-r--r--   0        0        0    12009 2023-12-19 06:10:45.759687 rockset-2.1.1/rockset/model/update_unsubscribe_preferences_response.py
--rw-r--r--   0        0        0    12206 2023-12-19 06:10:45.763687 rockset-2.1.1/rockset/model/update_user_request.py
--rw-r--r--   0        0        0    11958 2023-12-19 06:10:45.767686 rockset-2.1.1/rockset/model/update_view_request.py
--rw-r--r--   0        0        0    11759 2023-12-19 06:10:45.767686 rockset-2.1.1/rockset/model/update_view_response.py
--rw-r--r--   0        0        0    16338 2023-12-19 06:10:45.771687 rockset-2.1.1/rockset/model/update_virtual_instance_request.py
--rw-r--r--   0        0        0    11870 2023-12-19 06:10:45.775687 rockset-2.1.1/rockset/model/update_virtual_instance_response.py
--rw-r--r--   0        0        0    12907 2023-12-19 06:10:45.775687 rockset-2.1.1/rockset/model/user.py
--rw-r--r--   0        0        0    12155 2023-12-19 06:10:45.779687 rockset-2.1.1/rockset/model/validate_query_response.py
--rw-r--r--   0        0        0    14899 2023-12-19 06:10:45.783686 rockset-2.1.1/rockset/model/view.py
--rw-r--r--   0        0        0    19791 2023-12-19 06:10:45.783686 rockset-2.1.1/rockset/model/virtual_instance.py
--rw-r--r--   0        0        0    14087 2023-12-19 06:10:45.787687 rockset-2.1.1/rockset/model/virtual_instance_rrn.py
--rw-r--r--   0        0        0    11772 2023-12-19 06:10:45.791687 rockset-2.1.1/rockset/model/virtual_instance_stats.py
--rw-r--r--   0        0        0    12971 2023-12-19 06:10:45.791687 rockset-2.1.1/rockset/model/workspace.py
--rw-r--r--   0        0        0    12998 2023-12-19 06:10:45.795687 rockset-2.1.1/rockset/model/xml_params.py
--rw-r--r--   0        0        0    84037 2023-12-19 06:10:46.219687 rockset-2.1.1/rockset/model_utils.py
--rw-r--r--   0        0        0    16147 2023-12-19 06:10:46.223687 rockset-2.1.1/rockset/models/__init__.py
--rw-r--r--   0        0        0     1819 2023-07-10 18:55:10.870843 rockset-2.1.1/rockset/query_paginator.py
--rw-r--r--   0        0        0    14645 2023-12-19 06:10:46.215687 rockset-2.1.1/rockset/rest.py
--rw-r--r--   0        0        0     9281 2023-12-19 06:10:46.223687 rockset-2.1.1/rockset/rockset_client.py
--rw-r--r--   0        0        0     3644 2023-07-10 18:55:10.870843 rockset-2.1.1/rockset/value.py
--rw-r--r--   0        0        0     2169 1970-01-01 00:00:00.000000 rockset-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0      357 2023-07-10 18:55:10.858843 rockset-2.1.2/LONG_DESCRIPTION.rst
+-rw-r--r--   0        0        0     1616 2024-05-02 17:18:58.170182 rockset-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1338 2024-05-02 16:38:13.559561 rockset-2.1.2/rockset/__init__.py
+-rw-r--r--   0        0        0      208 2024-05-02 16:38:13.559561 rockset-2.1.2/rockset/api/__init__.py
+-rw-r--r--   0        0        0    34696 2024-05-02 16:38:13.679561 rockset-2.1.2/rockset/api/aliases_api.py
+-rw-r--r--   0        0        0    30366 2024-05-02 16:38:13.671560 rockset-2.1.2/rockset/api/api_keys_api.py
+-rw-r--r--   0        0        0   121161 2024-05-02 16:38:13.671560 rockset-2.1.2/rockset/api/collections_api.py
+-rw-r--r--   0        0        0    28165 2024-05-02 16:38:13.671560 rockset-2.1.2/rockset/api/custom_roles_api.py
+-rw-r--r--   0        0        0    12078 2024-05-02 16:38:13.671560 rockset-2.1.2/rockset/api/deployment_settings_api.py
+-rw-r--r--   0        0        0    21187 2024-05-02 16:38:13.675560 rockset-2.1.2/rockset/api/documents_api.py
+-rw-r--r--   0        0        0    85639 2024-05-02 16:38:13.675560 rockset-2.1.2/rockset/api/integrations_api.py
+-rw-r--r--   0        0        0     6168 2024-05-02 16:38:13.679561 rockset-2.1.2/rockset/api/organizations_api.py
+-rw-r--r--   0        0        0    38385 2024-05-02 16:38:13.675560 rockset-2.1.2/rockset/api/queries_api.py
+-rw-r--r--   0        0        0    87753 2024-05-02 16:38:13.675560 rockset-2.1.2/rockset/api/query_lambdas_api.py
+-rw-r--r--   0        0        0    33184 2024-05-02 16:38:13.675560 rockset-2.1.2/rockset/api/scheduled_lambdas_api.py
+-rw-r--r--   0        0        0     7687 2024-05-02 16:38:13.671560 rockset-2.1.2/rockset/api/shared_lambdas_api.py
+-rw-r--r--   0        0        0   110948 2024-05-02 16:38:13.675560 rockset-2.1.2/rockset/api/sources_api.py
+-rw-r--r--   0        0        0    43268 2024-05-02 16:38:13.675560 rockset-2.1.2/rockset/api/users_api.py
+-rw-r--r--   0        0        0    34441 2024-05-02 16:38:13.679561 rockset-2.1.2/rockset/api/views_api.py
+-rw-r--r--   0        0        0    87620 2024-05-02 16:38:13.679561 rockset-2.1.2/rockset/api/virtual_instances_api.py
+-rw-r--r--   0        0        0    22087 2024-05-02 16:38:13.679561 rockset-2.1.2/rockset/api/workspaces_api.py
+-rw-r--r--   0        0        0    36393 2024-05-02 16:38:13.563562 rockset-2.1.2/rockset/api_client.py
+-rw-r--r--   0        0        0     1286 2024-05-02 16:38:13.575561 rockset-2.1.2/rockset/apis/__init__.py
+-rw-r--r--   0        0        0    15516 2024-05-02 16:38:13.555561 rockset-2.1.2/rockset/configuration.py
+-rw-r--r--   0        0        0     3831 2023-07-10 18:55:10.862843 rockset-2.1.2/rockset/document.py
+-rw-r--r--   0        0        0     6072 2024-05-02 16:38:13.559561 rockset-2.1.2/rockset/exceptions.py
+-rw-r--r--   0        0        0      348 2024-05-02 16:38:13.575561 rockset-2.1.2/rockset/model/__init__.py
+-rw-r--r--   0        0        0    11950 2024-05-02 16:38:11.667578 rockset-2.1.2/rockset/model/add_documents_request.py
+-rw-r--r--   0        0        0    12291 2024-05-02 16:38:11.687578 rockset-2.1.2/rockset/model/add_documents_response.py
+-rw-r--r--   0        0        0    14049 2024-05-02 16:38:11.703578 rockset-2.1.2/rockset/model/alias.py
+-rw-r--r--   0        0        0    14557 2024-05-02 16:38:11.715578 rockset-2.1.2/rockset/model/api_key.py
+-rw-r--r--   0        0        0    14462 2024-05-02 16:38:11.727578 rockset-2.1.2/rockset/model/async_query_options.py
+-rw-r--r--   0        0        0    13796 2024-05-02 16:38:11.743578 rockset-2.1.2/rockset/model/auto_scaling_policy.py
+-rw-r--r--   0        0        0    12229 2024-05-02 16:38:11.751577 rockset-2.1.2/rockset/model/aws_access_key.py
+-rw-r--r--   0        0        0    12101 2024-05-02 16:38:11.763577 rockset-2.1.2/rockset/model/aws_role.py
+-rw-r--r--   0        0        0    15709 2024-05-02 16:38:11.775577 rockset-2.1.2/rockset/model/azure_blob_storage_collection_creation_request.py
+-rw-r--r--   0        0        0    11893 2024-05-02 16:38:11.783577 rockset-2.1.2/rockset/model/azure_blob_storage_integration.py
+-rw-r--r--   0        0        0    12616 2024-05-02 16:38:11.791577 rockset-2.1.2/rockset/model/azure_blob_storage_integration_creation_request.py
+-rw-r--r--   0        0        0    14536 2024-05-02 16:38:11.799577 rockset-2.1.2/rockset/model/azure_blob_storage_source_wrapper.py
+-rw-r--r--   0        0        0    15689 2024-05-02 16:38:11.815577 rockset-2.1.2/rockset/model/azure_event_hubs_collection_creation_request.py
+-rw-r--r--   0        0        0    11787 2024-05-02 16:38:11.839577 rockset-2.1.2/rockset/model/azure_event_hubs_integration.py
+-rw-r--r--   0        0        0    12586 2024-05-02 16:38:11.847577 rockset-2.1.2/rockset/model/azure_event_hubs_integration_creation_request.py
+-rw-r--r--   0        0        0    13452 2024-05-02 16:38:11.855577 rockset-2.1.2/rockset/model/azure_event_hubs_source_wrapper.py
+-rw-r--r--   0        0        0    15062 2023-07-10 21:58:00.859999 rockset-2.1.2/rockset/model/azure_service_bus_collection_creation_request.py
+-rw-r--r--   0        0        0    11888 2024-05-02 16:38:11.863577 rockset-2.1.2/rockset/model/azure_service_bus_integration.py
+-rw-r--r--   0        0        0    13333 2023-07-10 21:58:00.871999 rockset-2.1.2/rockset/model/azure_service_bus_source_wrapper.py
+-rw-r--r--   0        0        0    18743 2024-05-02 16:38:11.875576 rockset-2.1.2/rockset/model/bulk_stats.py
+-rw-r--r--   0        0        0    11798 2024-05-02 16:38:11.879576 rockset-2.1.2/rockset/model/cancel_query_response.py
+-rw-r--r--   0        0        0    13225 2024-05-02 16:38:11.887576 rockset-2.1.2/rockset/model/cluster.py
+-rw-r--r--   0        0        0    18893 2024-05-02 16:38:11.895576 rockset-2.1.2/rockset/model/collection.py
+-rw-r--r--   0        0        0    14847 2024-05-02 16:38:11.911576 rockset-2.1.2/rockset/model/collection_mount.py
+-rw-r--r--   0        0        0    11852 2024-05-02 16:38:11.915576 rockset-2.1.2/rockset/model/collection_mount_response.py
+-rw-r--r--   0        0        0    11772 2024-05-02 16:38:11.923576 rockset-2.1.2/rockset/model/collection_mount_stats.py
+-rw-r--r--   0        0        0    17061 2024-05-02 16:38:11.927576 rockset-2.1.2/rockset/model/collection_stats.py
+-rw-r--r--   0        0        0    12333 2024-05-02 16:38:11.931576 rockset-2.1.2/rockset/model/create_alias_request.py
+-rw-r--r--   0        0        0    11769 2024-05-02 16:38:11.939576 rockset-2.1.2/rockset/model/create_alias_response.py
+-rw-r--r--   0        0        0    12525 2024-05-02 16:38:11.947576 rockset-2.1.2/rockset/model/create_api_key_request.py
+-rw-r--r--   0        0        0    11780 2024-05-02 16:38:11.955576 rockset-2.1.2/rockset/model/create_api_key_response.py
+-rw-r--r--   0        0        0    11765 2024-05-02 16:38:11.963575 rockset-2.1.2/rockset/model/create_collection_mount_request.py
+-rw-r--r--   0        0        0    11913 2024-05-02 16:38:11.967576 rockset-2.1.2/rockset/model/create_collection_mounts_response.py
+-rw-r--r--   0        0        0    15091 2024-05-02 16:38:11.975576 rockset-2.1.2/rockset/model/create_collection_request.py
+-rw-r--r--   0        0        0    11819 2024-05-02 16:38:11.983575 rockset-2.1.2/rockset/model/create_collection_response.py
+-rw-r--r--   0        0        0    16382 2024-05-02 16:38:11.991575 rockset-2.1.2/rockset/model/create_integration_request.py
+-rw-r--r--   0        0        0    11829 2024-05-02 16:38:11.999575 rockset-2.1.2/rockset/model/create_integration_response.py
+-rw-r--r--   0        0        0    12571 2024-05-02 16:38:12.003575 rockset-2.1.2/rockset/model/create_query_lambda_request.py
+-rw-r--r--   0        0        0    12063 2024-05-02 16:38:12.007575 rockset-2.1.2/rockset/model/create_query_lambda_tag_request.py
+-rw-r--r--   0        0        0    12501 2024-05-02 16:38:12.015575 rockset-2.1.2/rockset/model/create_role_request.py
+-rw-r--r--   0        0        0    15152 2024-05-02 16:38:12.023575 rockset-2.1.2/rockset/model/create_scheduled_lambda_request.py
+-rw-r--r--   0        0        0    12479 2024-05-02 16:38:12.027575 rockset-2.1.2/rockset/model/create_user_request.py
+-rw-r--r--   0        0        0    11759 2024-05-02 16:38:12.035575 rockset-2.1.2/rockset/model/create_user_response.py
+-rw-r--r--   0        0        0    12170 2024-05-02 16:38:12.039575 rockset-2.1.2/rockset/model/create_view_request.py
+-rw-r--r--   0        0        0    11759 2024-05-02 16:38:12.047575 rockset-2.1.2/rockset/model/create_view_response.py
+-rw-r--r--   0        0        0    16139 2024-05-02 16:38:12.051575 rockset-2.1.2/rockset/model/create_virtual_instance_request.py
+-rw-r--r--   0        0        0    11870 2024-05-02 16:38:12.059575 rockset-2.1.2/rockset/model/create_virtual_instance_response.py
+-rw-r--r--   0        0        0    12038 2024-05-02 16:38:12.067575 rockset-2.1.2/rockset/model/create_workspace_request.py
+-rw-r--r--   0        0        0    11809 2024-05-02 16:38:12.071575 rockset-2.1.2/rockset/model/create_workspace_response.py
+-rw-r--r--   0        0        0    14179 2024-05-02 16:38:12.075574 rockset-2.1.2/rockset/model/csv_params.py
+-rw-r--r--   0        0        0    11769 2024-05-02 16:38:12.079574 rockset-2.1.2/rockset/model/delete_alias_response.py
+-rw-r--r--   0        0        0    11780 2024-05-02 16:38:12.083574 rockset-2.1.2/rockset/model/delete_api_key_response.py
+-rw-r--r--   0        0        0    11819 2024-05-02 16:38:12.087575 rockset-2.1.2/rockset/model/delete_collection_response.py
+-rw-r--r--   0        0        0    12036 2024-05-02 16:38:12.091575 rockset-2.1.2/rockset/model/delete_documents_request.py
+-rw-r--r--   0        0        0    11686 2024-05-02 16:38:12.099574 rockset-2.1.2/rockset/model/delete_documents_request_data.py
+-rw-r--r--   0        0        0    12300 2024-05-02 16:38:12.103574 rockset-2.1.2/rockset/model/delete_documents_response.py
+-rw-r--r--   0        0        0    11829 2024-05-02 16:38:12.107574 rockset-2.1.2/rockset/model/delete_integration_response.py
+-rw-r--r--   0        0        0    11830 2024-05-02 16:38:12.115574 rockset-2.1.2/rockset/model/delete_query_lambda_response.py
+-rw-r--r--   0        0        0    11779 2024-05-02 16:38:12.119574 rockset-2.1.2/rockset/model/delete_source_response.py
+-rw-r--r--   0        0        0    11759 2024-05-02 16:38:12.127574 rockset-2.1.2/rockset/model/delete_user_response.py
+-rw-r--r--   0        0        0    11759 2024-05-02 16:38:12.131574 rockset-2.1.2/rockset/model/delete_view_response.py
+-rw-r--r--   0        0        0    11870 2024-05-02 16:38:12.139574 rockset-2.1.2/rockset/model/delete_virtual_instance_response.py
+-rw-r--r--   0        0        0    11809 2024-05-02 16:38:12.143574 rockset-2.1.2/rockset/model/delete_workspace_response.py
+-rw-r--r--   0        0        0    11833 2024-05-02 16:38:12.151574 rockset-2.1.2/rockset/model/deployment_settings.py
+-rw-r--r--   0        0        0    11882 2024-05-02 16:38:12.155574 rockset-2.1.2/rockset/model/deployment_settings_response.py
+-rw-r--r--   0        0        0    13023 2024-05-02 16:38:12.163574 rockset-2.1.2/rockset/model/document_status.py
+-rw-r--r--   0        0        0    15627 2024-05-02 16:38:12.171574 rockset-2.1.2/rockset/model/dynamodb_collection_creation_request.py
+-rw-r--r--   0        0        0    12563 2024-05-02 16:38:12.175574 rockset-2.1.2/rockset/model/dynamodb_integration.py
+-rw-r--r--   0        0        0    12484 2024-05-02 16:38:12.183574 rockset-2.1.2/rockset/model/dynamodb_integration_creation_request.py
+-rw-r--r--   0        0        0    14861 2024-05-02 16:38:12.187574 rockset-2.1.2/rockset/model/dynamodb_source_wrapper.py
+-rw-r--r--   0        0        0    14996 2024-05-02 16:38:12.195573 rockset-2.1.2/rockset/model/error_model.py
+-rw-r--r--   0        0        0    12392 2024-05-02 16:38:12.199573 rockset-2.1.2/rockset/model/event_time_info.py
+-rw-r--r--   0        0        0    12338 2024-05-02 16:38:12.207574 rockset-2.1.2/rockset/model/execute_public_query_lambda_request.py
+-rw-r--r--   0        0        0    17858 2024-05-02 16:38:12.211573 rockset-2.1.2/rockset/model/execute_query_lambda_request.py
+-rw-r--r--   0        0        0    12093 2024-05-02 16:38:12.215573 rockset-2.1.2/rockset/model/execution_status.py
+-rw-r--r--   0        0        0    11743 2024-05-02 16:38:12.219573 rockset-2.1.2/rockset/model/field_mapping_query.py
+-rw-r--r--   0        0        0    13075 2024-05-02 16:38:12.227573 rockset-2.1.2/rockset/model/field_mapping_v2.py
+-rw-r--r--   0        0        0    12543 2024-05-02 16:38:12.231573 rockset-2.1.2/rockset/model/field_partition.py
+-rw-r--r--   0        0        0    15063 2023-07-10 18:55:10.866843 rockset-2.1.2/rockset/model/file_upload_collection_creation_request.py
+-rw-r--r--   0        0        0    13611 2023-07-10 18:55:10.866843 rockset-2.1.2/rockset/model/file_upload_source_wrapper.py
+-rw-r--r--   0        0        0    13393 2024-05-02 16:38:12.239573 rockset-2.1.2/rockset/model/format_params.py
+-rw-r--r--   0        0        0    12001 2024-05-02 16:38:12.243573 rockset-2.1.2/rockset/model/gcp_service_account.py
+-rw-r--r--   0        0        0    15577 2024-05-02 16:38:12.255573 rockset-2.1.2/rockset/model/gcs_collection_creation_request.py
+-rw-r--r--   0        0        0    11915 2024-05-02 16:38:12.259573 rockset-2.1.2/rockset/model/gcs_integration.py
+-rw-r--r--   0        0        0    12409 2024-05-02 16:38:12.267573 rockset-2.1.2/rockset/model/gcs_integration_creation_request.py
+-rw-r--r--   0        0        0    14681 2024-05-02 16:38:12.271573 rockset-2.1.2/rockset/model/gcs_source_wrapper.py
+-rw-r--r--   0        0        0    11760 2024-05-02 16:38:12.279573 rockset-2.1.2/rockset/model/get_alias_response.py
+-rw-r--r--   0        0        0    11771 2024-05-02 16:38:12.283573 rockset-2.1.2/rockset/model/get_api_key_response.py
+-rw-r--r--   0        0        0    12194 2024-05-02 16:38:12.287573 rockset-2.1.2/rockset/model/get_collection_commit.py
+-rw-r--r--   0        0        0    12318 2024-05-02 16:38:12.291573 rockset-2.1.2/rockset/model/get_collection_commit_data.py
+-rw-r--r--   0        0        0    11751 2024-05-02 16:38:12.303573 rockset-2.1.2/rockset/model/get_collection_commit_request.py
+-rw-r--r--   0        0        0    11810 2024-05-02 16:38:12.311572 rockset-2.1.2/rockset/model/get_collection_response.py
+-rw-r--r--   0        0        0    11820 2024-05-02 16:38:12.315572 rockset-2.1.2/rockset/model/get_integration_response.py
+-rw-r--r--   0        0        0    11789 2024-05-02 16:38:12.319572 rockset-2.1.2/rockset/model/get_query_response.py
+-rw-r--r--   0        0        0    11770 2024-05-02 16:38:12.323572 rockset-2.1.2/rockset/model/get_source_response.py
+-rw-r--r--   0        0        0    11750 2024-05-02 16:38:12.327572 rockset-2.1.2/rockset/model/get_view_response.py
+-rw-r--r--   0        0        0    11861 2024-05-02 16:38:12.335572 rockset-2.1.2/rockset/model/get_virtual_instance_response.py
+-rw-r--r--   0        0        0    11800 2024-05-02 16:38:12.339572 rockset-2.1.2/rockset/model/get_workspace_response.py
+-rw-r--r--   0        0        0    12704 2024-05-02 16:38:12.343572 rockset-2.1.2/rockset/model/input_field.py
+-rw-r--r--   0        0        0    18131 2024-05-02 16:38:12.351572 rockset-2.1.2/rockset/model/integration.py
+-rw-r--r--   0        0        0    15597 2024-05-02 16:38:12.359572 rockset-2.1.2/rockset/model/kafka_collection_creation_request.py
+-rw-r--r--   0        0        0    14826 2024-05-02 16:38:12.363572 rockset-2.1.2/rockset/model/kafka_integration.py
+-rw-r--r--   0        0        0    12439 2024-05-02 16:38:12.371572 rockset-2.1.2/rockset/model/kafka_integration_creation_request.py
+-rw-r--r--   0        0        0    14319 2024-05-02 16:38:12.375572 rockset-2.1.2/rockset/model/kafka_source_wrapper.py
+-rw-r--r--   0        0        0    11845 2024-05-02 16:38:12.379572 rockset-2.1.2/rockset/model/kafka_v3_security_config.py
+-rw-r--r--   0        0        0    15617 2024-05-02 16:38:12.387572 rockset-2.1.2/rockset/model/kinesis_collection_creation_request.py
+-rw-r--r--   0        0        0    12169 2024-05-02 16:38:12.391572 rockset-2.1.2/rockset/model/kinesis_integration.py
+-rw-r--r--   0        0        0    12469 2024-05-02 16:38:12.395572 rockset-2.1.2/rockset/model/kinesis_integration_creation_request.py
+-rw-r--r--   0        0        0    13895 2024-05-02 16:38:12.399572 rockset-2.1.2/rockset/model/kinesis_source_wrapper.py
+-rw-r--r--   0        0        0    11819 2024-05-02 16:38:12.403572 rockset-2.1.2/rockset/model/list_aliases_response.py
+-rw-r--r--   0        0        0    11835 2024-05-02 16:38:12.411572 rockset-2.1.2/rockset/model/list_api_keys_response.py
+-rw-r--r--   0        0        0    11937 2024-05-02 16:38:12.415572 rockset-2.1.2/rockset/model/list_collection_mounts_response.py
+-rw-r--r--   0        0        0    11874 2024-05-02 16:38:12.419571 rockset-2.1.2/rockset/model/list_collections_response.py
+-rw-r--r--   0        0        0    11892 2024-05-02 16:38:12.423571 rockset-2.1.2/rockset/model/list_integrations_response.py
+-rw-r--r--   0        0        0    11804 2024-05-02 16:38:12.431571 rockset-2.1.2/rockset/model/list_queries_response.py
+-rw-r--r--   0        0        0    11964 2024-05-02 16:38:12.435571 rockset-2.1.2/rockset/model/list_query_lambda_tags_response.py
+-rw-r--r--   0        0        0    12010 2024-05-02 16:38:12.439571 rockset-2.1.2/rockset/model/list_query_lambda_versions_response.py
+-rw-r--r--   0        0        0    11889 2024-05-02 16:38:12.447571 rockset-2.1.2/rockset/model/list_query_lambdas_response.py
+-rw-r--r--   0        0        0    11802 2024-05-02 16:38:12.451571 rockset-2.1.2/rockset/model/list_roles_response.py
+-rw-r--r--   0        0        0    11935 2024-05-02 16:38:12.455571 rockset-2.1.2/rockset/model/list_scheduled_lambdas_response.py
+-rw-r--r--   0        0        0    11856 2024-05-02 16:38:12.459571 rockset-2.1.2/rockset/model/list_sources_response.py
+-rw-r--r--   0        0        0    12003 2024-05-02 16:38:12.467571 rockset-2.1.2/rockset/model/list_unsubscribe_preferences_response.py
+-rw-r--r--   0        0        0    11794 2024-05-02 16:38:12.471571 rockset-2.1.2/rockset/model/list_users_response.py
+-rw-r--r--   0        0        0    11802 2024-05-02 16:38:12.475571 rockset-2.1.2/rockset/model/list_views_response.py
+-rw-r--r--   0        0        0    11937 2024-05-02 16:38:12.483571 rockset-2.1.2/rockset/model/list_virtual_instances_response.py
+-rw-r--r--   0        0        0    11854 2024-05-02 16:38:12.487571 rockset-2.1.2/rockset/model/list_workspaces_response.py
+-rw-r--r--   0        0        0    12454 2024-05-02 16:38:12.491571 rockset-2.1.2/rockset/model/microbatch_policy.py
+-rw-r--r--   0        0        0    12170 2024-05-02 16:38:12.495571 rockset-2.1.2/rockset/model/mongo_db_integration.py
+-rw-r--r--   0        0        0    15617 2024-05-02 16:38:12.503571 rockset-2.1.2/rockset/model/mongodb_collection_creation_request.py
+-rw-r--r--   0        0        0    12470 2024-05-02 16:38:12.507571 rockset-2.1.2/rockset/model/mongodb_integration_creation_request.py
+-rw-r--r--   0        0        0    14123 2024-05-02 16:38:12.515571 rockset-2.1.2/rockset/model/mongodb_source_wrapper.py
+-rw-r--r--   0        0        0    11918 2024-05-02 16:38:12.519571 rockset-2.1.2/rockset/model/offsets.py
+-rw-r--r--   0        0        0    13910 2024-05-02 16:38:12.531571 rockset-2.1.2/rockset/model/organization.py
+-rw-r--r--   0        0        0    11821 2024-05-02 16:38:12.535570 rockset-2.1.2/rockset/model/organization_response.py
+-rw-r--r--   0        0        0    12527 2024-05-02 16:38:12.539570 rockset-2.1.2/rockset/model/output_field.py
+-rw-r--r--   0        0        0    11775 2024-05-02 16:38:12.547570 rockset-2.1.2/rockset/model/pagination.py
+-rw-r--r--   0        0        0    13055 2024-05-02 16:38:12.551570 rockset-2.1.2/rockset/model/pagination_info.py
+-rw-r--r--   0        0        0    12155 2024-05-02 16:38:12.555570 rockset-2.1.2/rockset/model/patch_document.py
+-rw-r--r--   0        0        0    11920 2024-05-02 16:38:12.559570 rockset-2.1.2/rockset/model/patch_documents_request.py
+-rw-r--r--   0        0        0    12237 2024-05-02 16:38:12.567570 rockset-2.1.2/rockset/model/patch_documents_response.py
+-rw-r--r--   0        0        0    13672 2024-05-02 16:38:12.571570 rockset-2.1.2/rockset/model/patch_operation.py
+-rw-r--r--   0        0        0    16216 2024-05-02 16:38:12.575570 rockset-2.1.2/rockset/model/privilege.py
+-rw-r--r--   0        0        0    12407 2024-05-02 16:38:12.579570 rockset-2.1.2/rockset/model/query_error.py
+-rw-r--r--   0        0        0    11907 2024-05-02 16:38:12.587570 rockset-2.1.2/rockset/model/query_field_type.py
+-rw-r--r--   0        0        0    15365 2024-05-02 16:38:12.591570 rockset-2.1.2/rockset/model/query_info.py
+-rw-r--r--   0        0        0    13688 2024-05-02 16:38:12.595570 rockset-2.1.2/rockset/model/query_lambda.py
+-rw-r--r--   0        0        0    12219 2024-05-02 16:38:12.599570 rockset-2.1.2/rockset/model/query_lambda_sql.py
+-rw-r--r--   0        0        0    12786 2024-05-02 16:38:12.603570 rockset-2.1.2/rockset/model/query_lambda_stats.py
+-rw-r--r--   0        0        0    12124 2024-05-02 16:38:12.607570 rockset-2.1.2/rockset/model/query_lambda_tag.py
+-rw-r--r--   0        0        0    11843 2024-05-02 16:38:12.615570 rockset-2.1.2/rockset/model/query_lambda_tag_response.py
+-rw-r--r--   0        0        0    15267 2024-05-02 16:38:12.619570 rockset-2.1.2/rockset/model/query_lambda_version.py
+-rw-r--r--   0        0        0    11883 2024-05-02 16:38:12.623570 rockset-2.1.2/rockset/model/query_lambda_version_response.py
+-rw-r--r--   0        0        0    13051 2023-07-10 18:55:10.866843 rockset-2.1.2/rockset/model/query_pagination_response.py
+-rw-r--r--   0        0        0    12188 2024-05-02 16:38:12.631570 rockset-2.1.2/rockset/model/query_parameter.py
+-rw-r--r--   0        0        0    15940 2024-05-02 16:38:12.635570 rockset-2.1.2/rockset/model/query_request.py
+-rw-r--r--   0        0        0    13270 2024-05-02 16:38:12.639570 rockset-2.1.2/rockset/model/query_request_sql.py
+-rw-r--r--   0        0        0    16189 2023-07-10 18:55:10.866843 rockset-2.1.2/rockset/model/query_response.py
+-rw-r--r--   0        0        0    12105 2024-05-02 16:38:12.647570 rockset-2.1.2/rockset/model/query_response_stats.py
+-rw-r--r--   0        0        0    11870 2024-05-02 16:38:12.651569 rockset-2.1.2/rockset/model/resume_virtual_instance_response.py
+-rw-r--r--   0        0        0    13363 2024-05-02 16:38:12.655569 rockset-2.1.2/rockset/model/role.py
+-rw-r--r--   0        0        0    11741 2024-05-02 16:38:12.659569 rockset-2.1.2/rockset/model/role_response.py
+-rw-r--r--   0        0        0    15567 2024-05-02 16:38:12.667569 rockset-2.1.2/rockset/model/s3_collection_creation_request.py
+-rw-r--r--   0        0        0    12154 2024-05-02 16:38:12.671569 rockset-2.1.2/rockset/model/s3_integration.py
+-rw-r--r--   0        0        0    12394 2024-05-02 16:38:12.679569 rockset-2.1.2/rockset/model/s3_integration_creation_request.py
+-rw-r--r--   0        0        0    15273 2024-05-02 16:38:12.683569 rockset-2.1.2/rockset/model/s3_source_wrapper.py
+-rw-r--r--   0        0        0    17460 2024-05-02 16:38:12.687569 rockset-2.1.2/rockset/model/scheduled_lambda.py
+-rw-r--r--   0        0        0    11852 2024-05-02 16:38:12.695569 rockset-2.1.2/rockset/model/scheduled_lambda_response.py
+-rw-r--r--   0        0        0    12201 2024-05-02 16:38:12.695569 rockset-2.1.2/rockset/model/schema_registry_config.py
+-rw-r--r--   0        0        0    11696 2023-07-10 18:55:10.866843 rockset-2.1.2/rockset/model/segment_integration.py
+-rw-r--r--   0        0        0    12465 2023-07-10 18:55:10.866843 rockset-2.1.2/rockset/model/segment_integration_creation_request.py
+-rw-r--r--   0        0        0    15637 2024-05-02 16:38:12.699569 rockset-2.1.2/rockset/model/snowflake_collection_creation_request.py
+-rw-r--r--   0        0        0    14450 2024-05-02 16:38:12.707569 rockset-2.1.2/rockset/model/snowflake_integration.py
+-rw-r--r--   0        0        0    12499 2024-05-02 16:38:12.711569 rockset-2.1.2/rockset/model/snowflake_integration_creation_request.py
+-rw-r--r--   0        0        0    13907 2024-05-02 16:38:12.719569 rockset-2.1.2/rockset/model/snowflake_source_wrapper.py
+-rw-r--r--   0        0        0    18792 2024-05-02 16:38:12.723569 rockset-2.1.2/rockset/model/source.py
+-rw-r--r--   0        0        0    11959 2024-05-02 16:38:12.727569 rockset-2.1.2/rockset/model/source_az_blob_storage_base.py
+-rw-r--r--   0        0        0    12723 2024-05-02 16:38:12.735569 rockset-2.1.2/rockset/model/source_az_blob_storage_settings.py
+-rw-r--r--   0        0        0    13678 2024-05-02 16:38:12.743569 rockset-2.1.2/rockset/model/source_azure_blob_storage.py
+-rw-r--r--   0        0        0    12664 2024-05-02 16:38:12.747569 rockset-2.1.2/rockset/model/source_azure_event_hubs.py
+-rw-r--r--   0        0        0    12552 2024-05-02 16:38:12.751569 rockset-2.1.2/rockset/model/source_azure_service_bus.py
+-rw-r--r--   0        0        0    12951 2024-05-02 16:38:12.759569 rockset-2.1.2/rockset/model/source_base.py
+-rw-r--r--   0        0        0    14033 2024-05-02 16:38:12.763568 rockset-2.1.2/rockset/model/source_dynamo_db.py
+-rw-r--r--   0        0        0    11908 2024-05-02 16:38:12.767568 rockset-2.1.2/rockset/model/source_dynamo_db_base.py
+-rw-r--r--   0        0        0    12989 2024-05-02 16:38:12.771568 rockset-2.1.2/rockset/model/source_dynamo_db_settings.py
+-rw-r--r--   0        0        0    12391 2024-05-02 16:38:12.779568 rockset-2.1.2/rockset/model/source_file_upload.py
+-rw-r--r--   0        0        0    13808 2024-05-02 16:38:12.783568 rockset-2.1.2/rockset/model/source_gcs.py
+-rw-r--r--   0        0        0    11857 2024-05-02 16:38:12.787568 rockset-2.1.2/rockset/model/source_gcs_base.py
+-rw-r--r--   0        0        0    12640 2024-05-02 16:38:12.795568 rockset-2.1.2/rockset/model/source_gcs_settings.py
+-rw-r--r--   0        0        0    13488 2024-05-02 16:38:12.799568 rockset-2.1.2/rockset/model/source_kafka.py
+-rw-r--r--   0        0        0    13024 2024-05-02 16:38:12.803568 rockset-2.1.2/rockset/model/source_kinesis.py
+-rw-r--r--   0        0        0    13315 2024-05-02 16:38:12.811568 rockset-2.1.2/rockset/model/source_mongo_db.py
+-rw-r--r--   0        0        0    14379 2024-05-02 16:38:12.815568 rockset-2.1.2/rockset/model/source_s3.py
+-rw-r--r--   0        0        0    11847 2024-05-02 16:38:12.819568 rockset-2.1.2/rockset/model/source_s3_base.py
+-rw-r--r--   0        0        0    12632 2024-05-02 16:38:12.823568 rockset-2.1.2/rockset/model/source_s3_settings.py
+-rw-r--r--   0        0        0    12274 2024-05-02 16:38:12.831568 rockset-2.1.2/rockset/model/source_snapshot.py
+-rw-r--r--   0        0        0    13110 2024-05-02 16:38:12.835568 rockset-2.1.2/rockset/model/source_snowflake.py
+-rw-r--r--   0        0        0    12384 2024-05-02 16:38:12.839568 rockset-2.1.2/rockset/model/source_system.py
+-rw-r--r--   0        0        0    11661 2024-05-02 16:38:12.843568 rockset-2.1.2/rockset/model/sql_expression.py
+-rw-r--r--   0        0        0    13623 2024-05-02 16:38:12.847568 rockset-2.1.2/rockset/model/stats.py
+-rw-r--r--   0        0        0    13696 2024-05-02 16:38:12.855568 rockset-2.1.2/rockset/model/status.py
+-rw-r--r--   0        0        0    13111 2024-05-02 16:38:12.859568 rockset-2.1.2/rockset/model/status_azure_event_hubs.py
+-rw-r--r--   0        0        0    12364 2024-05-02 16:38:12.863568 rockset-2.1.2/rockset/model/status_azure_event_hubs_partition.py
+-rw-r--r--   0        0        0    12727 2024-05-02 16:38:12.867568 rockset-2.1.2/rockset/model/status_azure_service_bus.py
+-rw-r--r--   0        0        0    12210 2024-05-02 16:38:12.875568 rockset-2.1.2/rockset/model/status_azure_service_bus_session.py
+-rw-r--r--   0        0        0    13563 2024-05-02 16:38:12.879567 rockset-2.1.2/rockset/model/status_dynamo_db.py
+-rw-r--r--   0        0        0    12705 2024-05-02 16:38:12.883567 rockset-2.1.2/rockset/model/status_dynamo_db_v2.py
+-rw-r--r--   0        0        0    13123 2024-05-02 16:38:12.891567 rockset-2.1.2/rockset/model/status_kafka.py
+-rw-r--r--   0        0        0    12337 2024-05-02 16:38:12.895567 rockset-2.1.2/rockset/model/status_kafka_partition.py
+-rw-r--r--   0        0        0    15614 2024-05-02 16:38:12.899567 rockset-2.1.2/rockset/model/status_mongo_db.py
+-rw-r--r--   0        0        0    11924 2024-05-02 16:38:12.903567 rockset-2.1.2/rockset/model/status_snowflake.py
+-rw-r--r--   0        0        0    11808 2024-05-02 16:38:12.911567 rockset-2.1.2/rockset/model/suspend_source_request.py
+-rw-r--r--   0        0        0    11873 2024-05-02 16:38:12.915567 rockset-2.1.2/rockset/model/suspend_virtual_instance_response.py
+-rw-r--r--   0        0        0    13338 2024-05-02 16:38:12.919567 rockset-2.1.2/rockset/model/tls_config.py
+-rw-r--r--   0        0        0    11894 2024-05-02 16:38:12.923567 rockset-2.1.2/rockset/model/unsubscribe_preference.py
+-rw-r--r--   0        0        0    12119 2024-05-02 16:38:12.931567 rockset-2.1.2/rockset/model/update_alias_request.py
+-rw-r--r--   0        0        0    12635 2024-05-02 16:38:12.935567 rockset-2.1.2/rockset/model/update_api_key_request.py
+-rw-r--r--   0        0        0    11780 2024-05-02 16:38:12.939567 rockset-2.1.2/rockset/model/update_api_key_response.py
+-rw-r--r--   0        0        0    12247 2024-05-02 16:38:12.947567 rockset-2.1.2/rockset/model/update_collection_request.py
+-rw-r--r--   0        0        0    11872 2024-05-02 16:38:12.951567 rockset-2.1.2/rockset/model/update_deployment_settings_request.py
+-rw-r--r--   0        0        0    16136 2024-05-02 16:38:12.955567 rockset-2.1.2/rockset/model/update_integration_request.py
+-rw-r--r--   0        0        0    11829 2024-05-02 16:38:12.959567 rockset-2.1.2/rockset/model/update_integration_response.py
+-rw-r--r--   0        0        0    12329 2024-05-02 16:38:12.967567 rockset-2.1.2/rockset/model/update_query_lambda_request.py
+-rw-r--r--   0        0        0    12222 2024-05-02 16:38:12.971567 rockset-2.1.2/rockset/model/update_role_request.py
+-rw-r--r--   0        0        0    14031 2024-05-02 16:38:12.975567 rockset-2.1.2/rockset/model/update_scheduled_lambda_request.py
+-rw-r--r--   0        0        0    12006 2024-05-02 16:38:12.975567 rockset-2.1.2/rockset/model/update_unsubscribe_preferences_request.py
+-rw-r--r--   0        0        0    12009 2024-05-02 16:38:12.979567 rockset-2.1.2/rockset/model/update_unsubscribe_preferences_response.py
+-rw-r--r--   0        0        0    12206 2024-05-02 16:38:12.983567 rockset-2.1.2/rockset/model/update_user_request.py
+-rw-r--r--   0        0        0    11958 2024-05-02 16:38:12.987567 rockset-2.1.2/rockset/model/update_view_request.py
+-rw-r--r--   0        0        0    11759 2024-05-02 16:38:12.991567 rockset-2.1.2/rockset/model/update_view_response.py
+-rw-r--r--   0        0        0    17312 2024-05-02 16:38:12.995566 rockset-2.1.2/rockset/model/update_virtual_instance_request.py
+-rw-r--r--   0        0        0    11870 2024-05-02 16:38:12.999566 rockset-2.1.2/rockset/model/update_virtual_instance_response.py
+-rw-r--r--   0        0        0    12907 2024-05-02 16:38:13.003566 rockset-2.1.2/rockset/model/user.py
+-rw-r--r--   0        0        0    12155 2024-05-02 16:38:13.007566 rockset-2.1.2/rockset/model/validate_query_response.py
+-rw-r--r--   0        0        0    14899 2024-05-02 16:38:13.011566 rockset-2.1.2/rockset/model/view.py
+-rw-r--r--   0        0        0    20420 2024-05-02 16:38:13.015566 rockset-2.1.2/rockset/model/virtual_instance.py
+-rw-r--r--   0        0        0    14087 2024-05-02 16:37:13.744137 rockset-2.1.2/rockset/model/virtual_instance_rrn.py
+-rw-r--r--   0        0        0    11772 2024-05-02 16:38:13.019566 rockset-2.1.2/rockset/model/virtual_instance_stats.py
+-rw-r--r--   0        0        0    12971 2024-05-02 16:38:13.023566 rockset-2.1.2/rockset/model/workspace.py
+-rw-r--r--   0        0        0    12998 2024-05-02 16:38:13.027566 rockset-2.1.2/rockset/model/xml_params.py
+-rw-r--r--   0        0        0    84037 2024-05-02 16:38:13.571561 rockset-2.1.2/rockset/model_utils.py
+-rw-r--r--   0        0        0    16469 2024-05-02 16:38:13.575561 rockset-2.1.2/rockset/models/__init__.py
+-rw-r--r--   0        0        0     1819 2023-07-10 18:55:10.870843 rockset-2.1.2/rockset/query_paginator.py
+-rw-r--r--   0        0        0    14645 2024-05-02 16:38:13.567561 rockset-2.1.2/rockset/rest.py
+-rw-r--r--   0        0        0     9457 2024-05-02 16:38:13.575561 rockset-2.1.2/rockset/rockset_client.py
+-rw-r--r--   0        0        0     3644 2023-07-10 18:55:10.870843 rockset-2.1.2/rockset/value.py
+-rw-r--r--   0        0        0     2169 1970-01-01 00:00:00.000000 rockset-2.1.2/PKG-INFO
```

### Comparing `rockset-2.1.1/pyproject.toml` & `rockset-2.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rockset"
-version = "2.1.1"
+version = "2.1.2"
 description = "The python client for the Rockset API."
 authors = ["Rockset <support@rockset.com>"]
 packages = [
     {include = "rockset"}
 ]
 documentation = "https://github.com/rockset/rockset-python-client"
 repository = "https://github.com/rockset/rockset-python-client"
```

### Comparing `rockset-2.1.1/rockset/__init__.py` & `rockset-2.1.2/rockset/__init__.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/api/aliases_api.py` & `rockset-2.1.2/rockset/api/aliases_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/api/api_keys_api.py` & `rockset-2.1.2/rockset/api/api_keys_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/api/collections_api.py` & `rockset-2.1.2/rockset/api/collections_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/api/custom_roles_api.py` & `rockset-2.1.2/rockset/api/custom_roles_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/api/documents_api.py` & `rockset-2.1.2/rockset/api/documents_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/api/integrations_api.py` & `rockset-2.1.2/rockset/api/integrations_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1877,14 +1877,15 @@
         integration: str,
         azure_blob_storage: AzureBlobStorageIntegration = None,
         azure_event_hubs: AzureEventHubsIntegration = None,
         azure_service_bus: AzureServiceBusIntegration = None,
         description: str = None,
         dynamodb: DynamodbIntegration = None,
         gcs: GcsIntegration = None,
+        is_write_enabled: bool = None,
         kafka: KafkaIntegration = None,
         kinesis: KinesisIntegration = None,
         mongodb: MongoDbIntegration = None,
         s3: S3Integration = None,
         snowflake: SnowflakeIntegration = None,
         **kwargs
     ) -> typing.Union[UpdateIntegrationResponse, asyncio.Future]:
@@ -1921,14 +1922,15 @@
                 s3_export_bucket_name="s3_export_bucket_name_example",
             ),
             gcs=GcsIntegration(
                 gcp_service_account=GcpServiceAccount(
                     service_account_key_file_json="service_account_key_file_json_example",
                 ),
             ),
+            is_write_enabled=True,
             kafka=KafkaIntegration(
                 aws_role=AwsRole(
                     aws_external_id="external id of aws",
                     aws_role_arn="arn:aws:iam::2378964092:role/rockset-role",
                 ),
                 bootstrap_servers="localhost:9092",
                 connection_string="connection_string_example",
@@ -2006,14 +2008,15 @@
             integration (str): [required]
             azure_blob_storage (AzureBlobStorageIntegration): [optional]
             azure_event_hubs (AzureEventHubsIntegration): [optional]
             azure_service_bus (AzureServiceBusIntegration): [optional]
             description (str): Longer explanation for the integration.. [optional]
             dynamodb (DynamodbIntegration): [optional]
             gcs (GcsIntegration): [optional]
+            is_write_enabled (bool): is write access enabled for this integration.. [optional]
             kafka (KafkaIntegration): [optional]
             kinesis (KinesisIntegration): [optional]
             mongodb (MongoDbIntegration): [optional]
             s3 (S3Integration): [optional]
             snowflake (SnowflakeIntegration): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
```

### Comparing `rockset-2.1.1/rockset/api/organizations_api.py` & `rockset-2.1.2/rockset/api/organizations_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/api/queries_api.py` & `rockset-2.1.2/rockset/api/queries_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/api/query_lambdas_api.py` & `rockset-2.1.2/rockset/api/query_lambdas_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/api/scheduled_lambdas_api.py` & `rockset-2.1.2/rockset/api/scheduled_lambdas_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from rockset.model.create_scheduled_lambda_request import CreateScheduledLambdaRequest
 from rockset.model.error_model import ErrorModel
+from rockset.model.list_scheduled_lambdas_response import ListScheduledLambdasResponse
 from rockset.model.scheduled_lambda_response import ScheduledLambdaResponse
 from rockset.model.update_scheduled_lambda_request import UpdateScheduledLambdaRequest
 from rockset.models import *
 
 
 class ScheduledLambdas(object):
     """NOTE: This class is auto generated by OpenAPI Generator
@@ -152,14 +153,115 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.get_endpoint = _Endpoint(
+            settings={
+                'response_type': (ScheduledLambdaResponse,),
+                'auth': [
+                    'apikey'
+                ],
+                'endpoint_path': '/v1/orgs/self/ws/{workspace}/scheduled_lambdas/{scheduledLambdaId}',
+                'operation_id': 'get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'workspace',
+                    'scheduled_lambda_id',
+                ],
+                'required': [
+                    'workspace',
+                    'scheduled_lambda_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'workspace':
+                        (str,),
+                    'scheduled_lambda_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'workspace': 'workspace',
+                    'scheduled_lambda_id': 'scheduledLambdaId',
+                },
+                'location_map': {
+                    'workspace': 'path',
+                    'scheduled_lambda_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.list_org_scheduled_lambdas_endpoint = _Endpoint(
+            settings={
+                'response_type': (ListScheduledLambdasResponse,),
+                'auth': [
+                    'apikey'
+                ],
+                'endpoint_path': '/v1/orgs/self/lambdas/scheduled_lambdas',
+                'operation_id': 'list_org_scheduled_lambdas',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.update_endpoint = _Endpoint(
             settings={
                 'response_type': (ScheduledLambdaResponse,),
                 'auth': [
                     'apikey'
                 ],
                 'endpoint_path': '/v1/orgs/self/ws/{workspace}/scheduled_lambdas/{scheduledLambdaId}',
@@ -259,17 +361,17 @@
         ```
 
         Keyword Args:
             workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
             apikey (str): The apikey to use when triggering execution of the associated query lambda.. [optional]
             cron_string (str): The UNIX-formatted cron string for this scheduled query lambda.. [required]
             ql_name (str): The name of the QL to use for scheduled execution.. [required]
-            tag (str): The QL tag to use for scheduled execution.. [optional]
+            tag (str): The QL tag to use for scheduled execution. One of either the QL tag or version must be specified. [optional]
             total_times_to_execute (int): The number of times to execute this scheduled query lambda. Once this scheduled query lambda has been executed this many times, it will no longer be executed.. [optional]
-            version (str): The version of the QL to use for scheduled execution.. [optional]
+            version (str): The version of the QL to use for scheduled execution. One of either the QL version or tag must be specified.. [optional]
             webhook_auth_header (str): The value to use as the authorization header when hitting the webhook.. [optional]
             webhook_payload (str): The payload that should be sent to the webhook. JSON format.. [optional]
             webhook_url (str): The URL of the webhook that should be triggered after this scheduled query lambda completes.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -418,14 +520,182 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['workspace'] = \
             workspace
         kwargs['scheduled_lambda_id'] = \
             scheduled_lambda_id
         return self.delete_endpoint.call_with_http_info(**kwargs)
 
+    def get(
+        self,
+        *,
+        scheduled_lambda_id: str,
+        workspace = "commons",
+        **kwargs
+    ) -> typing.Union[ScheduledLambdaResponse, asyncio.Future]:
+        """Retrieve a Scheduled Lambda mapping  # noqa: E501
+
+        Retrieve a scheduled lambda mapping for your organization.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        ```python
+        rs = RocksetClient(api_key=APIKEY)
+        future = rs.ScheduledLambdas.get(
+            scheduled_lambda_id="scheduledLambdaId_example",
+            async_req=True,
+        )
+        result = await future
+        ```
+
+        Keyword Args:
+            workspace (str): name of the workspace. [required] if omitted the server will use the default value of "commons"
+            scheduled_lambda_id (str): Scheduled Lambda RRN. [required]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done on the data received from the server.
+                If False, the client will also not convert nested inner objects
+                into the respective model types (the outermost object
+                is still converted to the model).
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ScheduledLambdaResponse
+                If the method is called asynchronously, returns an asyncio.Future which resolves to the response.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['workspace'] = \
+            workspace
+        kwargs['scheduled_lambda_id'] = \
+            scheduled_lambda_id
+        return self.get_endpoint.call_with_http_info(**kwargs)
+
+    def list_org_scheduled_lambdas(
+        self,
+        **kwargs
+    ) -> typing.Union[ListScheduledLambdasResponse, asyncio.Future]:
+        """List Scheduled Lambdas  # noqa: E501
+
+        List all Scheduled Lambdas in an organization.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        ```python
+        rs = RocksetClient(api_key=APIKEY)
+        future = rs.ScheduledLambdas.list_org_scheduled_lambdas(
+            async_req=True,
+        )
+        result = await future
+        ```
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done on the data received from the server.
+                If False, the client will also not convert nested inner objects
+                into the respective model types (the outermost object
+                is still converted to the model).
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ListScheduledLambdasResponse
+                If the method is called asynchronously, returns an asyncio.Future which resolves to the response.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        return self.list_org_scheduled_lambdas_endpoint.call_with_http_info(**kwargs)
+
     def update(
         self,
         *,
         scheduled_lambda_id: str,
         apikey: str = None,
         resume_permanent_error: bool = None,
         total_times_to_execute: int = None,
```

### Comparing `rockset-2.1.1/rockset/api/shared_lambdas_api.py` & `rockset-2.1.2/rockset/api/shared_lambdas_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/api/sources_api.py` & `rockset-2.1.2/rockset/api/sources_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/api/users_api.py` & `rockset-2.1.2/rockset/api/users_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/api/views_api.py` & `rockset-2.1.2/rockset/api/views_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/api/virtual_instances_api.py` & `rockset-2.1.2/rockset/api/virtual_instances_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -810,14 +810,15 @@
     def create(
         self,
         *,
         name: str,
         auto_suspend_seconds: int = None,
         description: str = None,
         enable_remount_on_resume: bool = None,
+        instance_class: str = None,
         mount_refresh_interval_seconds: int = None,
         mount_type: str = None,
         type: str = None,
         **kwargs
     ) -> typing.Union[CreateVirtualInstanceResponse, asyncio.Future]:
         """Create Virtual Instance  # noqa: E501
 
@@ -827,29 +828,31 @@
 
         ```python
         rs = RocksetClient(api_key=APIKEY)
         future = rs.VirtualInstances.create(
             auto_suspend_seconds=3600,
             description="VI serving prod traffic",
             enable_remount_on_resume=True,
+            instance_class="MO_IL",
             mount_refresh_interval_seconds=0,
             mount_type="LIVE",
             name="prod_vi",
             type="LARGE",
             async_req=True,
         )
         result = await future
         ```
 
         Keyword Args:
             auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]
             description (str): Description of requested virtual instance.. [optional]
-            enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended.. [optional]
+            enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended. Defaults to true.. [optional]
+            instance_class (str): Virtual Instance Class. Use `MO_IL` for Memory Optimized and `GP_IL` for General Purpose instance class.. [optional]
             mount_refresh_interval_seconds (int): DEPRECATED. Use `mount_type` instead. Number of seconds between data refreshes for mounts on this Virtual Instance. The only valid values are 0 and null. 0 means the data will be refreshed continuously and null means the data will never refresh.. [optional]
-            mount_type (str): The mount type of collections that this Virtual Instance will query. Live mounted collections stay up-to-date with the underlying collection in real-time. Static mounted collections do not stay up-to-date. See https://docs.rockset.com/documentation/docs/virtual-instances#virtual-instance-configuration. [optional]
+            mount_type (str): The mount type of collections that this Virtual Instance will query. Live mounted collections stay up-to-date with the underlying collection in real-time. Static mounted collections do not stay up-to-date. See https://docs.rockset.com/documentation/docs/using-virtual-instances#virtual-instance-configuration. [optional]
             name (str): Unique identifier for virtual instance, can contain alphanumeric or dash characters.. [required]
             type (str): Requested virtual instance type.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -1989,14 +1992,16 @@
         *,
         virtual_instance_id: str,
         auto_scaling_policy: AutoScalingPolicy = None,
         auto_suspend_enabled: bool = None,
         auto_suspend_seconds: int = None,
         description: str = None,
         enable_remount_on_resume: bool = None,
+        instance_class: str = None,
+        microbatch_policy: MicrobatchPolicy = None,
         mount_refresh_interval_seconds: int = None,
         mount_type: str = None,
         name: str = None,
         new_size: str = None,
         **kwargs
     ) -> typing.Union[UpdateVirtualInstanceResponse, asyncio.Future]:
         """Update Virtual Instance  # noqa: E501
@@ -2014,14 +2019,19 @@
                 max_size="XLARGE2",
                 min_size="LARGE",
             ),
             auto_suspend_enabled=True,
             auto_suspend_seconds=3600,
             description="VI for prod traffic",
             enable_remount_on_resume=True,
+            instance_class="MO_IL",
+            microbatch_policy=MicrobatchPolicy(
+                enabled=True,
+                resume_interval="PT2H30M5S",
+            ),
             mount_refresh_interval_seconds=0,
             mount_type="LIVE",
             name="prod_vi",
             new_size="LARGE",
             async_req=True,
         )
         result = await future
@@ -2030,16 +2040,18 @@
         Keyword Args:
             virtual_instance_id (str): Virtual Instance RRN. [required]
             auto_scaling_policy (AutoScalingPolicy): [optional]
             auto_suspend_enabled (bool): Whether Query VI auto-suspend should be enabled for this Virtual Instance.. [optional]
             auto_suspend_seconds (int): Number of seconds without queries after which the Query VI is suspended. [optional]
             description (str): New virtual instance description.. [optional]
             enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended.. [optional]
+            instance_class (str): Virtual Instance Class. Use `MO_IL` for Memory Optimized and `GP_IL` for General Purpose instance class.. [optional]
+            microbatch_policy (MicrobatchPolicy): [optional]
             mount_refresh_interval_seconds (int): DEPRECATED. Use `mount_type` instead. Number of seconds between data refreshes for mounts on this Virtual Instance. The only valid values are 0 and null. 0 means the data will be refreshed continuously and null means the data will never refresh.. [optional]
-            mount_type (str): The mount type of collections that this Virtual Instance will query. Live mounted collections stay up-to-date with the underlying collection in real-time. Static mounted collections do not stay up-to-date. See https://docs.rockset.com/documentation/docs/virtual-instances#virtual-instance-configuration. [optional]
+            mount_type (str): The mount type of collections that this Virtual Instance will query. Live mounted collections stay up-to-date with the underlying collection in real-time. Static mounted collections do not stay up-to-date. See https://docs.rockset.com/documentation/docs/using-virtual-instances#virtual-instance-configuration. [optional]
             name (str): New virtual instance name.. [optional]
             new_size (str): Requested virtual instance size.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
```

### Comparing `rockset-2.1.1/rockset/api/workspaces_api.py` & `rockset-2.1.2/rockset/api/workspaces_api.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/api_client.py` & `rockset-2.1.2/rockset/api_client.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/apis/__init__.py` & `rockset-2.1.2/rockset/apis/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #   sys.setrecursionlimit(n)
 
 # Import APIs into API package:
 from rockset.api.api_keys_api import APIKeys
 from rockset.api.aliases_api import Aliases
 from rockset.api.collections_api import Collections
 from rockset.api.custom_roles_api import CustomRoles
+from rockset.api.deployment_settings_api import DeploymentSettings
 from rockset.api.documents_api import Documents
 from rockset.api.integrations_api import Integrations
 from rockset.api.organizations_api import Organizations
 from rockset.api.queries_api import Queries
 from rockset.api.query_lambdas_api import QueryLambdas
 from rockset.api.scheduled_lambdas_api import ScheduledLambdas
 from rockset.api.shared_lambdas_api import SharedLambdas
```

### Comparing `rockset-2.1.1/rockset/configuration.py` & `rockset-2.1.2/rockset/configuration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/document.py` & `rockset-2.1.2/rockset/document.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/exceptions.py` & `rockset-2.1.2/rockset/exceptions.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/add_documents_request.py` & `rockset-2.1.2/rockset/model/add_documents_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/add_documents_response.py` & `rockset-2.1.2/rockset/model/add_documents_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/alias.py` & `rockset-2.1.2/rockset/model/alias.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/api_key.py` & `rockset-2.1.2/rockset/model/api_key.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/async_query_options.py` & `rockset-2.1.2/rockset/model/async_query_options.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/auto_scaling_policy.py` & `rockset-2.1.2/rockset/model/auto_scaling_policy.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/aws_access_key.py` & `rockset-2.1.2/rockset/model/aws_access_key.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/aws_role.py` & `rockset-2.1.2/rockset/model/aws_role.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/azure_blob_storage_collection_creation_request.py` & `rockset-2.1.2/rockset/model/azure_blob_storage_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/azure_blob_storage_integration.py` & `rockset-2.1.2/rockset/model/azure_blob_storage_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/azure_blob_storage_integration_creation_request.py` & `rockset-2.1.2/rockset/model/azure_blob_storage_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/azure_blob_storage_source_wrapper.py` & `rockset-2.1.2/rockset/model/azure_blob_storage_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/azure_event_hubs_collection_creation_request.py` & `rockset-2.1.2/rockset/model/azure_event_hubs_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/azure_event_hubs_integration.py` & `rockset-2.1.2/rockset/model/azure_event_hubs_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/azure_event_hubs_integration_creation_request.py` & `rockset-2.1.2/rockset/model/azure_event_hubs_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/azure_event_hubs_source_wrapper.py` & `rockset-2.1.2/rockset/model/azure_event_hubs_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/azure_service_bus_collection_creation_request.py` & `rockset-2.1.2/rockset/model/azure_service_bus_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/azure_service_bus_integration.py` & `rockset-2.1.2/rockset/model/azure_service_bus_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/azure_service_bus_source_wrapper.py` & `rockset-2.1.2/rockset/model/azure_service_bus_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/bulk_stats.py` & `rockset-2.1.2/rockset/model/bulk_stats.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/cancel_query_response.py` & `rockset-2.1.2/rockset/model/cancel_query_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/cluster.py` & `rockset-2.1.2/rockset/model/cluster.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/collection.py` & `rockset-2.1.2/rockset/model/collection.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/collection_mount.py` & `rockset-2.1.2/rockset/model/collection_mount.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/collection_mount_response.py` & `rockset-2.1.2/rockset/model/collection_mount_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/collection_mount_stats.py` & `rockset-2.1.2/rockset/model/collection_mount_stats.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/collection_stats.py` & `rockset-2.1.2/rockset/model/collection_stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,24 +164,24 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             bulk_bytes_inserted (int): Total number of bytes inserted into the collection during bulk.. [optional]  # noqa: E501
             bulk_bytes_overwritten (int): Total number of bytes overwritten in writing into the collection during bulk.. [optional]  # noqa: E501
             bytes_inserted (int): Total number of bytes inserted into the collection.. [optional]  # noqa: E501
             bytes_overwritten (int): Total number of bytes overwritten in writing into the collection.. [optional]  # noqa: E501
-            column_index_size (int): Total collection column index size in bytes.. [optional]  # noqa: E501
+            column_index_size (int): DEPRECATED: Total collection column index size in bytes.. [optional]  # noqa: E501
             doc_count (int): Number of documents in the collection.. [optional]  # noqa: E501
             fill_progress (float): Number between 0 and 1 that indicates progress of collection creation.. [optional]  # noqa: E501
-            inverted_index_size (int): Total collection inverted index size in bytes.. [optional]  # noqa: E501
+            inverted_index_size (int): DEPRECATED: Total collection inverted index size in bytes.. [optional]  # noqa: E501
             last_queried_ms (int): Milliseconds since Unix epoch Jan 1, 1970.. [optional]  # noqa: E501
             last_updated_ms (int): Milliseconds since Unix epoch Jan 1, 1970.. [optional]  # noqa: E501
             purged_doc_count (int): Number of documents purged from the collection.. [optional]  # noqa: E501
             purged_doc_size (int): Total size of bytes purged in bytes.. [optional]  # noqa: E501
-            range_index_size (int): Total collection range index size in bytes.. [optional]  # noqa: E501
-            row_index_size (int): Total collection row index size in bytes.. [optional]  # noqa: E501
+            range_index_size (int): DEPRECATED: Total collection range index size in bytes.. [optional]  # noqa: E501
+            row_index_size (int): DEPRECATED: Total collection row index size in bytes.. [optional]  # noqa: E501
             total_index_size (int): Total collection index size in bytes.. [optional]  # noqa: E501
             total_size (int): Total collection size in bytes.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -231,24 +231,24 @@
         """CollectionStats - a model defined in OpenAPI
 
         Keyword Args:
             bulk_bytes_inserted (int): Total number of bytes inserted into the collection during bulk.. [optional]  # noqa: E501
             bulk_bytes_overwritten (int): Total number of bytes overwritten in writing into the collection during bulk.. [optional]  # noqa: E501
             bytes_inserted (int): Total number of bytes inserted into the collection.. [optional]  # noqa: E501
             bytes_overwritten (int): Total number of bytes overwritten in writing into the collection.. [optional]  # noqa: E501
-            column_index_size (int): Total collection column index size in bytes.. [optional]  # noqa: E501
+            column_index_size (int): DEPRECATED: Total collection column index size in bytes.. [optional]  # noqa: E501
             doc_count (int): Number of documents in the collection.. [optional]  # noqa: E501
             fill_progress (float): Number between 0 and 1 that indicates progress of collection creation.. [optional]  # noqa: E501
-            inverted_index_size (int): Total collection inverted index size in bytes.. [optional]  # noqa: E501
+            inverted_index_size (int): DEPRECATED: Total collection inverted index size in bytes.. [optional]  # noqa: E501
             last_queried_ms (int): Milliseconds since Unix epoch Jan 1, 1970.. [optional]  # noqa: E501
             last_updated_ms (int): Milliseconds since Unix epoch Jan 1, 1970.. [optional]  # noqa: E501
             purged_doc_count (int): Number of documents purged from the collection.. [optional]  # noqa: E501
             purged_doc_size (int): Total size of bytes purged in bytes.. [optional]  # noqa: E501
-            range_index_size (int): Total collection range index size in bytes.. [optional]  # noqa: E501
-            row_index_size (int): Total collection row index size in bytes.. [optional]  # noqa: E501
+            range_index_size (int): DEPRECATED: Total collection range index size in bytes.. [optional]  # noqa: E501
+            row_index_size (int): DEPRECATED: Total collection row index size in bytes.. [optional]  # noqa: E501
             total_index_size (int): Total collection index size in bytes.. [optional]  # noqa: E501
             total_size (int): Total collection size in bytes.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `rockset-2.1.1/rockset/model/create_alias_request.py` & `rockset-2.1.2/rockset/model/create_alias_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/create_alias_response.py` & `rockset-2.1.2/rockset/model/create_alias_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/create_api_key_request.py` & `rockset-2.1.2/rockset/model/create_api_key_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/create_api_key_response.py` & `rockset-2.1.2/rockset/model/create_api_key_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/create_collection_mount_request.py` & `rockset-2.1.2/rockset/model/create_collection_mount_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/create_collection_mounts_response.py` & `rockset-2.1.2/rockset/model/create_collection_mounts_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/create_collection_request.py` & `rockset-2.1.2/rockset/model/create_collection_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/create_collection_response.py` & `rockset-2.1.2/rockset/model/create_collection_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/create_integration_request.py` & `rockset-2.1.2/rockset/model/create_integration_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
             'name': (str,),  # noqa: E501
             'azure_blob_storage': (AzureBlobStorageIntegration, none_type),  # noqa: E501
             'azure_event_hubs': (AzureEventHubsIntegration, none_type),  # noqa: E501
             'azure_service_bus': (AzureServiceBusIntegration, none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'dynamodb': (DynamodbIntegration, none_type),  # noqa: E501
             'gcs': (GcsIntegration, none_type),  # noqa: E501
+            'is_write_enabled': (bool, none_type),  # noqa: E501
             'kafka': (KafkaIntegration, none_type),  # noqa: E501
             'kinesis': (KinesisIntegration, none_type),  # noqa: E501
             'mongodb': (MongoDbIntegration, none_type),  # noqa: E501
             's3': (S3Integration, none_type),  # noqa: E501
             'snowflake': (SnowflakeIntegration, none_type),  # noqa: E501
         }
 
@@ -128,14 +129,15 @@
         'name': 'name',  # noqa: E501
         'azure_blob_storage': 'azure_blob_storage',  # noqa: E501
         'azure_event_hubs': 'azure_event_hubs',  # noqa: E501
         'azure_service_bus': 'azure_service_bus',  # noqa: E501
         'description': 'description',  # noqa: E501
         'dynamodb': 'dynamodb',  # noqa: E501
         'gcs': 'gcs',  # noqa: E501
+        'is_write_enabled': 'is_write_enabled',  # noqa: E501
         'kafka': 'kafka',  # noqa: E501
         'kinesis': 'kinesis',  # noqa: E501
         'mongodb': 'mongodb',  # noqa: E501
         's3': 's3',  # noqa: E501
         'snowflake': 'snowflake',  # noqa: E501
     }
 
@@ -185,14 +187,15 @@
                                 _visited_composed_classes = (Animal,)
             azure_blob_storage (AzureBlobStorageIntegration): [optional]  # noqa: E501
             azure_event_hubs (AzureEventHubsIntegration): [optional]  # noqa: E501
             azure_service_bus (AzureServiceBusIntegration): [optional]  # noqa: E501
             description (str): Longer explanation for the integration.. [optional]  # noqa: E501
             dynamodb (DynamodbIntegration): [optional]  # noqa: E501
             gcs (GcsIntegration): [optional]  # noqa: E501
+            is_write_enabled (bool): is write access enabled for this integration.. [optional]  # noqa: E501
             kafka (KafkaIntegration): [optional]  # noqa: E501
             kinesis (KinesisIntegration): [optional]  # noqa: E501
             mongodb (MongoDbIntegration): [optional]  # noqa: E501
             s3 (S3Integration): [optional]  # noqa: E501
             snowflake (SnowflakeIntegration): [optional]  # noqa: E501
         """
 
@@ -249,14 +252,15 @@
             name (str): Descriptive label.
             azure_blob_storage (AzureBlobStorageIntegration): [optional]  # noqa: E501
             azure_event_hubs (AzureEventHubsIntegration): [optional]  # noqa: E501
             azure_service_bus (AzureServiceBusIntegration): [optional]  # noqa: E501
             description (str): Longer explanation for the integration.. [optional]  # noqa: E501
             dynamodb (DynamodbIntegration): [optional]  # noqa: E501
             gcs (GcsIntegration): [optional]  # noqa: E501
+            is_write_enabled (bool): is write access enabled for this integration.. [optional]  # noqa: E501
             kafka (KafkaIntegration): [optional]  # noqa: E501
             kinesis (KinesisIntegration): [optional]  # noqa: E501
             mongodb (MongoDbIntegration): [optional]  # noqa: E501
             s3 (S3Integration): [optional]  # noqa: E501
             snowflake (SnowflakeIntegration): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
```

### Comparing `rockset-2.1.1/rockset/model/create_integration_response.py` & `rockset-2.1.2/rockset/model/create_integration_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/create_query_lambda_request.py` & `rockset-2.1.2/rockset/model/create_query_lambda_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/create_query_lambda_tag_request.py` & `rockset-2.1.2/rockset/model/create_query_lambda_tag_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/create_role_request.py` & `rockset-2.1.2/rockset/model/create_role_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/create_scheduled_lambda_request.py` & `rockset-2.1.2/rockset/model/update_scheduled_lambda_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 
-class CreateScheduledLambdaRequest(ModelNormal):
+class UpdateScheduledLambdaRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,55 +77,45 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'cron_string': (str,),  # noqa: E501
-            'ql_name': (str,),  # noqa: E501
             'apikey': (str, none_type),  # noqa: E501
-            'tag': (str, none_type),  # noqa: E501
+            'resume_permanent_error': (bool, none_type),  # noqa: E501
             'total_times_to_execute': (int, none_type),  # noqa: E501
-            'version': (str, none_type),  # noqa: E501
             'webhook_auth_header': (str, none_type),  # noqa: E501
             'webhook_payload': (str, none_type),  # noqa: E501
             'webhook_url': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'cron_string': 'cron_string',  # noqa: E501
-        'ql_name': 'ql_name',  # noqa: E501
         'apikey': 'apikey',  # noqa: E501
-        'tag': 'tag',  # noqa: E501
+        'resume_permanent_error': 'resume_permanent_error',  # noqa: E501
         'total_times_to_execute': 'total_times_to_execute',  # noqa: E501
-        'version': 'version',  # noqa: E501
         'webhook_auth_header': 'webhook_auth_header',  # noqa: E501
         'webhook_payload': 'webhook_payload',  # noqa: E501
         'webhook_url': 'webhook_url',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, cron_string, ql_name, *args, **kwargs):  # noqa: E501
-        """CreateScheduledLambdaRequest - a model defined in OpenAPI
-
-        Args:
-            cron_string (str): The UNIX-formatted cron string for this scheduled query lambda.
-            ql_name (str): The name of the QL to use for scheduled execution.
+    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
+        """UpdateScheduledLambdaRequest - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -151,17 +141,16 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             apikey (str): The apikey to use when triggering execution of the associated query lambda.. [optional]  # noqa: E501
-            tag (str): The QL tag to use for scheduled execution.. [optional]  # noqa: E501
-            total_times_to_execute (int): The number of times to execute this scheduled query lambda. Once this scheduled query lambda has been executed this many times, it will no longer be executed.. [optional]  # noqa: E501
-            version (str): The version of the QL to use for scheduled execution.. [optional]  # noqa: E501
+            resume_permanent_error (bool): Boolean flag to allow a scheduled query lambda to resume execution after being suspended due to execution failure. This flag will be unset after scheduled lambda execution.. [optional]  # noqa: E501
+            total_times_to_execute (int): The number of times to execute this scheduled query lambda.. [optional]  # noqa: E501
             webhook_auth_header (str): The value to use as the authorization header when hitting the webhook.. [optional]  # noqa: E501
             webhook_payload (str): The payload that should be sent to the webhook. JSON format.. [optional]  # noqa: E501
             webhook_url (str): The URL of the webhook that should be triggered after this scheduled query lambda completes.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -184,16 +173,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.cron_string = cron_string
-        self.ql_name = ql_name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -206,24 +193,21 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, *, cron_string, ql_name, **kwargs):  # noqa: E501
-        """CreateScheduledLambdaRequest - a model defined in OpenAPI
+    def __init__(self, **kwargs):  # noqa: E501
+        """UpdateScheduledLambdaRequest - a model defined in OpenAPI
 
         Keyword Args:
-            cron_string (str): The UNIX-formatted cron string for this scheduled query lambda.
-            ql_name (str): The name of the QL to use for scheduled execution.
             apikey (str): The apikey to use when triggering execution of the associated query lambda.. [optional]  # noqa: E501
-            tag (str): The QL tag to use for scheduled execution.. [optional]  # noqa: E501
-            total_times_to_execute (int): The number of times to execute this scheduled query lambda. Once this scheduled query lambda has been executed this many times, it will no longer be executed.. [optional]  # noqa: E501
-            version (str): The version of the QL to use for scheduled execution.. [optional]  # noqa: E501
+            resume_permanent_error (bool): Boolean flag to allow a scheduled query lambda to resume execution after being suspended due to execution failure. This flag will be unset after scheduled lambda execution.. [optional]  # noqa: E501
+            total_times_to_execute (int): The number of times to execute this scheduled query lambda.. [optional]  # noqa: E501
             webhook_auth_header (str): The value to use as the authorization header when hitting the webhook.. [optional]  # noqa: E501
             webhook_payload (str): The payload that should be sent to the webhook. JSON format.. [optional]  # noqa: E501
             webhook_url (str): The URL of the webhook that should be triggered after this scheduled query lambda completes.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -275,16 +259,14 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
-        self.cron_string = cron_string
-        self.ql_name = ql_name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rockset-2.1.1/rockset/model/create_user_request.py` & `rockset-2.1.2/rockset/model/create_user_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/create_user_response.py` & `rockset-2.1.2/rockset/model/create_user_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/create_view_request.py` & `rockset-2.1.2/rockset/model/create_view_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/create_view_response.py` & `rockset-2.1.2/rockset/model/create_view_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/create_virtual_instance_request.py` & `rockset-2.1.2/rockset/model/create_virtual_instance_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('instance_class',): {
+            'MO_IL': "MO_IL",
+            'GP_IL': "GP_IL",
+        },
         ('mount_type',): {
             'LIVE': "LIVE",
             'STATIC': "STATIC",
         },
         ('type',): {
             'FREE': "FREE",
             'NANO': "NANO",
@@ -100,14 +104,15 @@
                 and the value is attribute type.
         """
         return {
             'name': (str,),  # noqa: E501
             'auto_suspend_seconds': (int, none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'enable_remount_on_resume': (bool, none_type),  # noqa: E501
+            'instance_class': (str, none_type),  # noqa: E501
             'mount_refresh_interval_seconds': (int, none_type),  # noqa: E501
             'mount_type': (str, none_type),  # noqa: E501
             'type': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -115,14 +120,15 @@
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'auto_suspend_seconds': 'auto_suspend_seconds',  # noqa: E501
         'description': 'description',  # noqa: E501
         'enable_remount_on_resume': 'enable_remount_on_resume',  # noqa: E501
+        'instance_class': 'instance_class',  # noqa: E501
         'mount_refresh_interval_seconds': 'mount_refresh_interval_seconds',  # noqa: E501
         'mount_type': 'mount_type',  # noqa: E501
         'type': 'type',  # noqa: E501
     }
 
     read_only_vars = {
     }
@@ -166,17 +172,18 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]  # noqa: E501
             description (str): Description of requested virtual instance.. [optional]  # noqa: E501
-            enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended.. [optional]  # noqa: E501
+            enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended. Defaults to true.. [optional]  # noqa: E501
+            instance_class (str): Virtual Instance Class. Use `MO_IL` for Memory Optimized and `GP_IL` for General Purpose instance class.. [optional]  # noqa: E501
             mount_refresh_interval_seconds (int): DEPRECATED. Use `mount_type` instead. Number of seconds between data refreshes for mounts on this Virtual Instance. The only valid values are 0 and null. 0 means the data will be refreshed continuously and null means the data will never refresh.. [optional]  # noqa: E501
-            mount_type (str): The mount type of collections that this Virtual Instance will query. Live mounted collections stay up-to-date with the underlying collection in real-time. Static mounted collections do not stay up-to-date. See https://docs.rockset.com/documentation/docs/virtual-instances#virtual-instance-configuration. [optional]  # noqa: E501
+            mount_type (str): The mount type of collections that this Virtual Instance will query. Live mounted collections stay up-to-date with the underlying collection in real-time. Static mounted collections do not stay up-to-date. See https://docs.rockset.com/documentation/docs/using-virtual-instances#virtual-instance-configuration. [optional]  # noqa: E501
             type (str): Requested virtual instance type.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -225,17 +232,18 @@
     def __init__(self, *, name, **kwargs):  # noqa: E501
         """CreateVirtualInstanceRequest - a model defined in OpenAPI
 
         Keyword Args:
             name (str): Unique identifier for virtual instance, can contain alphanumeric or dash characters.
             auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]  # noqa: E501
             description (str): Description of requested virtual instance.. [optional]  # noqa: E501
-            enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended.. [optional]  # noqa: E501
+            enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended. Defaults to true.. [optional]  # noqa: E501
+            instance_class (str): Virtual Instance Class. Use `MO_IL` for Memory Optimized and `GP_IL` for General Purpose instance class.. [optional]  # noqa: E501
             mount_refresh_interval_seconds (int): DEPRECATED. Use `mount_type` instead. Number of seconds between data refreshes for mounts on this Virtual Instance. The only valid values are 0 and null. 0 means the data will be refreshed continuously and null means the data will never refresh.. [optional]  # noqa: E501
-            mount_type (str): The mount type of collections that this Virtual Instance will query. Live mounted collections stay up-to-date with the underlying collection in real-time. Static mounted collections do not stay up-to-date. See https://docs.rockset.com/documentation/docs/virtual-instances#virtual-instance-configuration. [optional]  # noqa: E501
+            mount_type (str): The mount type of collections that this Virtual Instance will query. Live mounted collections stay up-to-date with the underlying collection in real-time. Static mounted collections do not stay up-to-date. See https://docs.rockset.com/documentation/docs/using-virtual-instances#virtual-instance-configuration. [optional]  # noqa: E501
             type (str): Requested virtual instance type.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
```

### Comparing `rockset-2.1.1/rockset/model/create_virtual_instance_response.py` & `rockset-2.1.2/rockset/model/create_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/create_workspace_request.py` & `rockset-2.1.2/rockset/model/create_workspace_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/create_workspace_response.py` & `rockset-2.1.2/rockset/model/create_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/csv_params.py` & `rockset-2.1.2/rockset/model/csv_params.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/delete_alias_response.py` & `rockset-2.1.2/rockset/model/delete_alias_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/delete_api_key_response.py` & `rockset-2.1.2/rockset/model/delete_api_key_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/delete_collection_response.py` & `rockset-2.1.2/rockset/model/delete_collection_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/delete_documents_request.py` & `rockset-2.1.2/rockset/model/delete_documents_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/delete_documents_request_data.py` & `rockset-2.1.2/rockset/model/delete_documents_request_data.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/delete_documents_response.py` & `rockset-2.1.2/rockset/model/delete_documents_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/delete_integration_response.py` & `rockset-2.1.2/rockset/model/delete_integration_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/delete_query_lambda_response.py` & `rockset-2.1.2/rockset/model/delete_query_lambda_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/delete_source_response.py` & `rockset-2.1.2/rockset/model/delete_source_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/delete_user_response.py` & `rockset-2.1.2/rockset/model/delete_user_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/delete_view_response.py` & `rockset-2.1.2/rockset/model/delete_view_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/delete_virtual_instance_response.py` & `rockset-2.1.2/rockset/model/delete_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/delete_workspace_response.py` & `rockset-2.1.2/rockset/model/delete_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/document_status.py` & `rockset-2.1.2/rockset/model/document_status.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/dynamodb_collection_creation_request.py` & `rockset-2.1.2/rockset/model/dynamodb_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/dynamodb_integration.py` & `rockset-2.1.2/rockset/model/dynamodb_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/dynamodb_integration_creation_request.py` & `rockset-2.1.2/rockset/model/dynamodb_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/dynamodb_source_wrapper.py` & `rockset-2.1.2/rockset/model/dynamodb_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/error_model.py` & `rockset-2.1.2/rockset/model/error_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,14 +111,15 @@
             'column': (int, none_type),  # noqa: E501
             'error_id': (str, none_type),  # noqa: E501
             'line': (int, none_type),  # noqa: E501
             'message': (str, none_type),  # noqa: E501
             'query_id': (str, none_type),  # noqa: E501
             'trace_id': (str, none_type),  # noqa: E501
             'type': (str, none_type),  # noqa: E501
+            'virtual_instance_rrn': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -126,14 +127,15 @@
         'column': 'column',  # noqa: E501
         'error_id': 'error_id',  # noqa: E501
         'line': 'line',  # noqa: E501
         'message': 'message',  # noqa: E501
         'query_id': 'query_id',  # noqa: E501
         'trace_id': 'trace_id',  # noqa: E501
         'type': 'type',  # noqa: E501
+        'virtual_instance_rrn': 'virtual_instance_rrn',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -176,14 +178,15 @@
             column (int): Column where the error happened (if applicable).. [optional]  # noqa: E501
             error_id (str): ID of the error.. [optional]  # noqa: E501
             line (int): Line where the error happened (if applicable).. [optional]  # noqa: E501
             message (str): Descriptive message about the error.. [optional]  # noqa: E501
             query_id (str): ID of the query (if applicable).. [optional]  # noqa: E501
             trace_id (str): Internal trace ID to help with debugging.. [optional]  # noqa: E501
             type (str): Category of the error.. [optional]  # noqa: E501
+            virtual_instance_rrn (str): Virtual Instance RRN for the Virtual Instance that the query was run on (if applicable).. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -234,14 +237,15 @@
             column (int): Column where the error happened (if applicable).. [optional]  # noqa: E501
             error_id (str): ID of the error.. [optional]  # noqa: E501
             line (int): Line where the error happened (if applicable).. [optional]  # noqa: E501
             message (str): Descriptive message about the error.. [optional]  # noqa: E501
             query_id (str): ID of the query (if applicable).. [optional]  # noqa: E501
             trace_id (str): Internal trace ID to help with debugging.. [optional]  # noqa: E501
             type (str): Category of the error.. [optional]  # noqa: E501
+            virtual_instance_rrn (str): Virtual Instance RRN for the Virtual Instance that the query was run on (if applicable).. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.1.1/rockset/model/event_time_info.py` & `rockset-2.1.2/rockset/model/event_time_info.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/execute_public_query_lambda_request.py` & `rockset-2.1.2/rockset/model/execute_public_query_lambda_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/execute_query_lambda_request.py` & `rockset-2.1.2/rockset/model/execute_query_lambda_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/execution_status.py` & `rockset-2.1.2/rockset/model/execution_status.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/field_mapping_query.py` & `rockset-2.1.2/rockset/model/field_mapping_query.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/field_mapping_v2.py` & `rockset-2.1.2/rockset/model/field_mapping_v2.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/field_partition.py` & `rockset-2.1.2/rockset/model/field_partition.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/file_upload_collection_creation_request.py` & `rockset-2.1.2/rockset/model/file_upload_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/file_upload_source_wrapper.py` & `rockset-2.1.2/rockset/model/file_upload_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/format_params.py` & `rockset-2.1.2/rockset/model/format_params.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/gcp_service_account.py` & `rockset-2.1.2/rockset/model/gcp_service_account.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/gcs_collection_creation_request.py` & `rockset-2.1.2/rockset/model/gcs_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/gcs_integration.py` & `rockset-2.1.2/rockset/model/gcs_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/gcs_integration_creation_request.py` & `rockset-2.1.2/rockset/model/gcs_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/gcs_source_wrapper.py` & `rockset-2.1.2/rockset/model/gcs_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/get_alias_response.py` & `rockset-2.1.2/rockset/model/get_alias_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/get_api_key_response.py` & `rockset-2.1.2/rockset/model/get_api_key_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/get_collection_commit.py` & `rockset-2.1.2/rockset/model/get_collection_commit.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/get_collection_commit_data.py` & `rockset-2.1.2/rockset/model/get_collection_commit_data.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/get_collection_commit_request.py` & `rockset-2.1.2/rockset/model/get_collection_commit_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/get_collection_response.py` & `rockset-2.1.2/rockset/model/get_collection_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/get_integration_response.py` & `rockset-2.1.2/rockset/model/get_integration_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/get_query_response.py` & `rockset-2.1.2/rockset/model/get_query_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/get_source_response.py` & `rockset-2.1.2/rockset/model/get_source_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/get_view_response.py` & `rockset-2.1.2/rockset/model/get_view_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/get_virtual_instance_response.py` & `rockset-2.1.2/rockset/model/get_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/get_workspace_response.py` & `rockset-2.1.2/rockset/model/get_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/input_field.py` & `rockset-2.1.2/rockset/model/input_field.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/integration.py` & `rockset-2.1.2/rockset/model/integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,15 @@
             'azure_service_bus': (AzureServiceBusIntegration, none_type),  # noqa: E501
             'collections': ([Collection], none_type),  # noqa: E501
             'created_at': (str, none_type),  # noqa: E501
             'created_by_apikey_name': (str, none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'dynamodb': (DynamodbIntegration, none_type),  # noqa: E501
             'gcs': (GcsIntegration, none_type),  # noqa: E501
+            'is_write_enabled': (bool, none_type),  # noqa: E501
             'kafka': (KafkaIntegration, none_type),  # noqa: E501
             'kinesis': (KinesisIntegration, none_type),  # noqa: E501
             'mongodb': (MongoDbIntegration, none_type),  # noqa: E501
             'owner_email': (str, none_type),  # noqa: E501
             's3': (S3Integration, none_type),  # noqa: E501
             'snowflake': (SnowflakeIntegration, none_type),  # noqa: E501
         }
@@ -139,14 +140,15 @@
         'azure_service_bus': 'azure_service_bus',  # noqa: E501
         'collections': 'collections',  # noqa: E501
         'created_at': 'created_at',  # noqa: E501
         'created_by_apikey_name': 'created_by_apikey_name',  # noqa: E501
         'description': 'description',  # noqa: E501
         'dynamodb': 'dynamodb',  # noqa: E501
         'gcs': 'gcs',  # noqa: E501
+        'is_write_enabled': 'is_write_enabled',  # noqa: E501
         'kafka': 'kafka',  # noqa: E501
         'kinesis': 'kinesis',  # noqa: E501
         'mongodb': 'mongodb',  # noqa: E501
         'owner_email': 'owner_email',  # noqa: E501
         's3': 's3',  # noqa: E501
         'snowflake': 'snowflake',  # noqa: E501
     }
@@ -201,14 +203,15 @@
             azure_service_bus (AzureServiceBusIntegration): [optional]  # noqa: E501
             collections ([Collection]): List of collections that use the integration.. [optional]  # noqa: E501
             created_at (str): ISO-8601 date.. [optional]  # noqa: E501
             created_by_apikey_name (str): Name of the API key that was used to create this object if one was used.. [optional]  # noqa: E501
             description (str): Longer explanation for the integration.. [optional]  # noqa: E501
             dynamodb (DynamodbIntegration): [optional]  # noqa: E501
             gcs (GcsIntegration): [optional]  # noqa: E501
+            is_write_enabled (bool): is write access enabled for this integration. [optional]  # noqa: E501
             kafka (KafkaIntegration): [optional]  # noqa: E501
             kinesis (KinesisIntegration): [optional]  # noqa: E501
             mongodb (MongoDbIntegration): [optional]  # noqa: E501
             owner_email (str): User that owns this integration.. [optional]  # noqa: E501
             s3 (S3Integration): [optional]  # noqa: E501
             snowflake (SnowflakeIntegration): [optional]  # noqa: E501
         """
@@ -271,14 +274,15 @@
             azure_service_bus (AzureServiceBusIntegration): [optional]  # noqa: E501
             collections ([Collection]): List of collections that use the integration.. [optional]  # noqa: E501
             created_at (str): ISO-8601 date.. [optional]  # noqa: E501
             created_by_apikey_name (str): Name of the API key that was used to create this object if one was used.. [optional]  # noqa: E501
             description (str): Longer explanation for the integration.. [optional]  # noqa: E501
             dynamodb (DynamodbIntegration): [optional]  # noqa: E501
             gcs (GcsIntegration): [optional]  # noqa: E501
+            is_write_enabled (bool): is write access enabled for this integration. [optional]  # noqa: E501
             kafka (KafkaIntegration): [optional]  # noqa: E501
             kinesis (KinesisIntegration): [optional]  # noqa: E501
             mongodb (MongoDbIntegration): [optional]  # noqa: E501
             owner_email (str): User that owns this integration.. [optional]  # noqa: E501
             s3 (S3Integration): [optional]  # noqa: E501
             snowflake (SnowflakeIntegration): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
```

### Comparing `rockset-2.1.1/rockset/model/kafka_collection_creation_request.py` & `rockset-2.1.2/rockset/model/kafka_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/kafka_integration.py` & `rockset-2.1.2/rockset/model/kafka_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/kafka_integration_creation_request.py` & `rockset-2.1.2/rockset/model/kafka_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/kafka_source_wrapper.py` & `rockset-2.1.2/rockset/model/kafka_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/kafka_v3_security_config.py` & `rockset-2.1.2/rockset/model/kafka_v3_security_config.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/kinesis_collection_creation_request.py` & `rockset-2.1.2/rockset/model/kinesis_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/kinesis_integration.py` & `rockset-2.1.2/rockset/model/kinesis_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/kinesis_integration_creation_request.py` & `rockset-2.1.2/rockset/model/kinesis_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/kinesis_source_wrapper.py` & `rockset-2.1.2/rockset/model/kinesis_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/list_aliases_response.py` & `rockset-2.1.2/rockset/model/list_aliases_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/list_api_keys_response.py` & `rockset-2.1.2/rockset/model/list_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/list_collection_mounts_response.py` & `rockset-2.1.2/rockset/model/list_collection_mounts_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/list_collections_response.py` & `rockset-2.1.2/rockset/model/list_collections_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/list_integrations_response.py` & `rockset-2.1.2/rockset/model/list_integrations_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/list_queries_response.py` & `rockset-2.1.2/rockset/model/list_queries_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/list_query_lambda_tags_response.py` & `rockset-2.1.2/rockset/model/list_query_lambda_tags_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/list_query_lambda_versions_response.py` & `rockset-2.1.2/rockset/model/list_query_lambda_versions_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/list_query_lambdas_response.py` & `rockset-2.1.2/rockset/model/list_query_lambdas_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/list_roles_response.py` & `rockset-2.1.2/rockset/model/list_roles_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/list_sources_response.py` & `rockset-2.1.2/rockset/model/list_sources_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/list_unsubscribe_preferences_response.py` & `rockset-2.1.2/rockset/model/list_unsubscribe_preferences_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/list_users_response.py` & `rockset-2.1.2/rockset/model/list_users_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/list_views_response.py` & `rockset-2.1.2/rockset/model/list_views_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/list_virtual_instances_response.py` & `rockset-2.1.2/rockset/model/list_virtual_instances_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/list_workspaces_response.py` & `rockset-2.1.2/rockset/model/list_workspaces_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/mongo_db_integration.py` & `rockset-2.1.2/rockset/model/mongo_db_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/mongodb_collection_creation_request.py` & `rockset-2.1.2/rockset/model/mongodb_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/mongodb_integration_creation_request.py` & `rockset-2.1.2/rockset/model/mongodb_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/mongodb_source_wrapper.py` & `rockset-2.1.2/rockset/model/mongodb_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/offsets.py` & `rockset-2.1.2/rockset/model/offsets.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/organization.py` & `rockset-2.1.2/rockset/model/organization.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/organization_response.py` & `rockset-2.1.2/rockset/model/organization_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/output_field.py` & `rockset-2.1.2/rockset/model/output_field.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/pagination.py` & `rockset-2.1.2/rockset/model/pagination.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/pagination_info.py` & `rockset-2.1.2/rockset/model/pagination_info.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/patch_document.py` & `rockset-2.1.2/rockset/model/patch_document.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/patch_documents_request.py` & `rockset-2.1.2/rockset/model/patch_documents_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/patch_documents_response.py` & `rockset-2.1.2/rockset/model/patch_documents_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/patch_operation.py` & `rockset-2.1.2/rockset/model/patch_operation.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/privilege.py` & `rockset-2.1.2/rockset/model/privilege.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             'SUSPEND_RESUME_VI': "SUSPEND_RESUME_VI",
             'DELETE_VI': "DELETE_VI",
             'CREATE_SIMILARITY_INDEX_WS': "CREATE_SIMILARITY_INDEX_WS",
             'DELETE_SIMILARITY_INDEX_WS': "DELETE_SIMILARITY_INDEX_WS",
             'CREATE_NETWORK_CONFIGURATION_GLOBAL': "CREATE_NETWORK_CONFIGURATION_GLOBAL",
             'DELETE_NETWORK_CONFIGURATION_GLOBAL': "DELETE_NETWORK_CONFIGURATION_GLOBAL",
             'LIST_NETWORK_CONFIGURATIONS_GLOBAL': "LIST_NETWORK_CONFIGURATIONS_GLOBAL",
-            'UPDATE_ORG_QUERY_ROUTING': "UPDATE_ORG_QUERY_ROUTING",
+            'UPDATE_DEPLOYMENT_DEFAULT_QUERY_VI': "UPDATE_DEPLOYMENT_DEFAULT_QUERY_VI",
         },
     }
 
     validations = {
     }
 
     @cached_property
```

### Comparing `rockset-2.1.1/rockset/model/query_error.py` & `rockset-2.1.2/rockset/model/query_error.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/query_field_type.py` & `rockset-2.1.2/rockset/model/query_field_type.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/query_info.py` & `rockset-2.1.2/rockset/model/query_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
+            'destination_uri': (str, none_type),  # noqa: E501
             'executed_by': (str, none_type),  # noqa: E501
             'expires_at': (str, none_type),  # noqa: E501
             'last_offset': (str, none_type),  # noqa: E501
             'pagination': (Pagination, none_type),  # noqa: E501
             'query_errors': ([QueryError], none_type),  # noqa: E501
             'query_id': (str, none_type),  # noqa: E501
             'sql': (str, none_type),  # noqa: E501
@@ -112,14 +113,15 @@
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'destination_uri': 'destination_uri',  # noqa: E501
         'executed_by': 'executed_by',  # noqa: E501
         'expires_at': 'expires_at',  # noqa: E501
         'last_offset': 'last_offset',  # noqa: E501
         'pagination': 'pagination',  # noqa: E501
         'query_errors': 'query_errors',  # noqa: E501
         'query_id': 'query_id',  # noqa: E501
         'sql': 'sql',  # noqa: E501
@@ -165,14 +167,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
+            destination_uri (str): destination for query results. Only populated for Insert INTO s3 queries.. [optional]  # noqa: E501
             executed_by (str): User ID who executed the query.. [optional]  # noqa: E501
             expires_at (str): Time (UTC) that query results expire. Only populated if `status` is `COMPLETE`.. [optional]  # noqa: E501
             last_offset (str): The log offset that query results were written to in the destination collection. Only populated for INSERT INTO queries.. [optional]  # noqa: E501
             pagination (Pagination): [optional]  # noqa: E501
             query_errors ([QueryError]): Errors encountered while executing the query.. [optional]  # noqa: E501
             query_id (str): Unique Query ID.. [optional]  # noqa: E501
             sql (str): The SQL query for this request. [optional]  # noqa: E501
@@ -226,14 +229,15 @@
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, **kwargs):  # noqa: E501
         """QueryInfo - a model defined in OpenAPI
 
         Keyword Args:
+            destination_uri (str): destination for query results. Only populated for Insert INTO s3 queries.. [optional]  # noqa: E501
             executed_by (str): User ID who executed the query.. [optional]  # noqa: E501
             expires_at (str): Time (UTC) that query results expire. Only populated if `status` is `COMPLETE`.. [optional]  # noqa: E501
             last_offset (str): The log offset that query results were written to in the destination collection. Only populated for INSERT INTO queries.. [optional]  # noqa: E501
             pagination (Pagination): [optional]  # noqa: E501
             query_errors ([QueryError]): Errors encountered while executing the query.. [optional]  # noqa: E501
             query_id (str): Unique Query ID.. [optional]  # noqa: E501
             sql (str): The SQL query for this request. [optional]  # noqa: E501
```

### Comparing `rockset-2.1.1/rockset/model/query_lambda.py` & `rockset-2.1.2/rockset/model/query_lambda.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/query_lambda_sql.py` & `rockset-2.1.2/rockset/model/query_lambda_sql.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/query_lambda_stats.py` & `rockset-2.1.2/rockset/model/query_lambda_stats.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/query_lambda_tag.py` & `rockset-2.1.2/rockset/model/query_lambda_tag.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/query_lambda_tag_response.py` & `rockset-2.1.2/rockset/model/query_lambda_tag_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/query_lambda_version.py` & `rockset-2.1.2/rockset/model/query_lambda_version.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/query_lambda_version_response.py` & `rockset-2.1.2/rockset/model/query_lambda_version_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/query_pagination_response.py` & `rockset-2.1.2/rockset/model/query_pagination_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/query_parameter.py` & `rockset-2.1.2/rockset/model/query_parameter.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/query_request.py` & `rockset-2.1.2/rockset/model/query_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/query_request_sql.py` & `rockset-2.1.2/rockset/model/query_request_sql.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/query_response.py` & `rockset-2.1.2/rockset/model/query_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/query_response_stats.py` & `rockset-2.1.2/rockset/model/query_response_stats.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/resume_virtual_instance_response.py` & `rockset-2.1.2/rockset/model/resume_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/role.py` & `rockset-2.1.2/rockset/model/role.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/role_response.py` & `rockset-2.1.2/rockset/model/role_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/s3_collection_creation_request.py` & `rockset-2.1.2/rockset/model/s3_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/s3_integration.py` & `rockset-2.1.2/rockset/model/s3_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/s3_integration_creation_request.py` & `rockset-2.1.2/rockset/model/s3_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/s3_source_wrapper.py` & `rockset-2.1.2/rockset/model/s3_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/scheduled_lambda.py` & `rockset-2.1.2/rockset/model/scheduled_lambda.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,15 @@
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from rockset.model.execution_status import ExecutionStatus
-    from rockset.model.virtual_instance_rrn import VirtualInstanceRrn
     globals()['ExecutionStatus'] = ExecutionStatus
-    globals()['VirtualInstanceRrn'] = VirtualInstanceRrn
 
 
 class ScheduledLambda(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -97,15 +95,15 @@
             'ql_name': (str, none_type),  # noqa: E501
             'query_execution_status': (ExecutionStatus, none_type),  # noqa: E501
             'resume_permanent_error': (bool, none_type),  # noqa: E501
             'rrn': (str, none_type),  # noqa: E501
             'tag': (str, none_type),  # noqa: E501
             'total_times_to_execute': (int, none_type),  # noqa: E501
             'version': (str, none_type),  # noqa: E501
-            'vi_rrn': (VirtualInstanceRrn, none_type),  # noqa: E501
+            'webhook_execution_status': (ExecutionStatus, none_type),  # noqa: E501
             'webhook_payload': (str, none_type),  # noqa: E501
             'webhook_url': (str, none_type),  # noqa: E501
             'workspace': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -121,15 +119,15 @@
         'ql_name': 'ql_name',  # noqa: E501
         'query_execution_status': 'query_execution_status',  # noqa: E501
         'resume_permanent_error': 'resume_permanent_error',  # noqa: E501
         'rrn': 'rrn',  # noqa: E501
         'tag': 'tag',  # noqa: E501
         'total_times_to_execute': 'total_times_to_execute',  # noqa: E501
         'version': 'version',  # noqa: E501
-        'vi_rrn': 'vi_rrn',  # noqa: E501
+        'webhook_execution_status': 'webhook_execution_status',  # noqa: E501
         'webhook_payload': 'webhook_payload',  # noqa: E501
         'webhook_url': 'webhook_url',  # noqa: E501
         'workspace': 'workspace',  # noqa: E501
     }
 
     read_only_vars = {
     }
@@ -180,15 +178,15 @@
             ql_name (str): The name of the associated query lambda.. [optional]  # noqa: E501
             query_execution_status (ExecutionStatus): [optional]  # noqa: E501
             resume_permanent_error (bool): Boolean flag to allow a scheduled query lambda to resume execution after being suspended due to execution failure. This flag will be unset after scheduled lambda execution.. [optional]  # noqa: E501
             rrn (str): Scheduled Lambda mapping RRN.. [optional]  # noqa: E501
             tag (str): The query lambda tag.. [optional]  # noqa: E501
             total_times_to_execute (int): The number of times to execute this scheduled query lambda. Once this scheduled query lambda has been executed this many times, it will no longer be executed.. [optional]  # noqa: E501
             version (str): The version of the associated query lambda.. [optional]  # noqa: E501
-            vi_rrn (VirtualInstanceRrn): [optional]  # noqa: E501
+            webhook_execution_status (ExecutionStatus): [optional]  # noqa: E501
             webhook_payload (str): The payload that should be sent to the webhook.. [optional]  # noqa: E501
             webhook_url (str): The URL of the webhook that should be triggered after this scheduled query lambda completes.. [optional]  # noqa: E501
             workspace (str): Workspace of the associated query lambda.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -247,15 +245,15 @@
             ql_name (str): The name of the associated query lambda.. [optional]  # noqa: E501
             query_execution_status (ExecutionStatus): [optional]  # noqa: E501
             resume_permanent_error (bool): Boolean flag to allow a scheduled query lambda to resume execution after being suspended due to execution failure. This flag will be unset after scheduled lambda execution.. [optional]  # noqa: E501
             rrn (str): Scheduled Lambda mapping RRN.. [optional]  # noqa: E501
             tag (str): The query lambda tag.. [optional]  # noqa: E501
             total_times_to_execute (int): The number of times to execute this scheduled query lambda. Once this scheduled query lambda has been executed this many times, it will no longer be executed.. [optional]  # noqa: E501
             version (str): The version of the associated query lambda.. [optional]  # noqa: E501
-            vi_rrn (VirtualInstanceRrn): [optional]  # noqa: E501
+            webhook_execution_status (ExecutionStatus): [optional]  # noqa: E501
             webhook_payload (str): The payload that should be sent to the webhook.. [optional]  # noqa: E501
             webhook_url (str): The URL of the webhook that should be triggered after this scheduled query lambda completes.. [optional]  # noqa: E501
             workspace (str): Workspace of the associated query lambda.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
```

### Comparing `rockset-2.1.1/rockset/model/scheduled_lambda_response.py` & `rockset-2.1.2/rockset/model/scheduled_lambda_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/schema_registry_config.py` & `rockset-2.1.2/rockset/model/schema_registry_config.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/segment_integration.py` & `rockset-2.1.2/rockset/model/segment_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/segment_integration_creation_request.py` & `rockset-2.1.2/rockset/model/segment_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/snowflake_collection_creation_request.py` & `rockset-2.1.2/rockset/model/snowflake_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/snowflake_integration.py` & `rockset-2.1.2/rockset/model/snowflake_integration.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/snowflake_integration_creation_request.py` & `rockset-2.1.2/rockset/model/snowflake_integration_creation_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/snowflake_source_wrapper.py` & `rockset-2.1.2/rockset/model/snowflake_source_wrapper.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source.py` & `rockset-2.1.2/rockset/model/source.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
             'resume_at': (str, none_type),  # noqa: E501
             's3': (SourceS3, none_type),  # noqa: E501
             'snapshot': (SourceSnapshot, none_type),  # noqa: E501
             'snowflake': (SourceSnowflake, none_type),  # noqa: E501
             'status': (bool, date, datetime, dict, float, int, list, str, none_type, none_type),  # noqa: E501
             'suspended_at': (str, none_type),  # noqa: E501
             'system': (SourceSystem, none_type),  # noqa: E501
+            'write_api': ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -161,14 +162,15 @@
         'resume_at': 'resume_at',  # noqa: E501
         's3': 's3',  # noqa: E501
         'snapshot': 'snapshot',  # noqa: E501
         'snowflake': 'snowflake',  # noqa: E501
         'status': 'status',  # noqa: E501
         'suspended_at': 'suspended_at',  # noqa: E501
         'system': 'system',  # noqa: E501
+        'write_api': 'write_api',  # noqa: E501
     }
 
     read_only_vars = {
         'file_upload',  # noqa: E501
         'id',  # noqa: E501
         'resume_at',  # noqa: E501
         'status',  # noqa: E501
@@ -229,14 +231,15 @@
             resume_at (str): ISO-8601 date when source would be auto resumed, if suspended. [optional]  # noqa: E501
             s3 (SourceS3): [optional]  # noqa: E501
             snapshot (SourceSnapshot): [optional]  # noqa: E501
             snowflake (SourceSnowflake): [optional]  # noqa: E501
             status (bool, date, datetime, dict, float, int, list, str, none_type): [optional]  # noqa: E501
             suspended_at (str): ISO-8601 date when source was suspended, if suspended. [optional]  # noqa: E501
             system (SourceSystem): [optional]  # noqa: E501
+            write_api ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -295,14 +298,15 @@
             kafka (SourceKafka): [optional]  # noqa: E501
             kinesis (SourceKinesis): [optional]  # noqa: E501
             mongodb (SourceMongoDb): [optional]  # noqa: E501
             s3 (SourceS3): [optional]  # noqa: E501
             snapshot (SourceSnapshot): [optional]  # noqa: E501
             snowflake (SourceSnowflake): [optional]  # noqa: E501
             system (SourceSystem): [optional]  # noqa: E501
+            write_api ({str: (bool, date, datetime, dict, float, int, list, str, none_type)}): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `rockset-2.1.1/rockset/model/source_az_blob_storage_base.py` & `rockset-2.1.2/rockset/model/source_az_blob_storage_base.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_az_blob_storage_settings.py` & `rockset-2.1.2/rockset/model/source_az_blob_storage_settings.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_azure_blob_storage.py` & `rockset-2.1.2/rockset/model/source_azure_blob_storage.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_azure_event_hubs.py` & `rockset-2.1.2/rockset/model/source_azure_event_hubs.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_azure_service_bus.py` & `rockset-2.1.2/rockset/model/source_azure_service_bus.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_base.py` & `rockset-2.1.2/rockset/model/source_base.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_dynamo_db.py` & `rockset-2.1.2/rockset/model/source_dynamo_db.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_dynamo_db_base.py` & `rockset-2.1.2/rockset/model/source_dynamo_db_base.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_dynamo_db_settings.py` & `rockset-2.1.2/rockset/model/source_dynamo_db_settings.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_file_upload.py` & `rockset-2.1.2/rockset/model/source_file_upload.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_gcs.py` & `rockset-2.1.2/rockset/model/source_gcs.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_gcs_base.py` & `rockset-2.1.2/rockset/model/source_gcs_base.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_gcs_settings.py` & `rockset-2.1.2/rockset/model/source_gcs_settings.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_kafka.py` & `rockset-2.1.2/rockset/model/source_kafka.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_kinesis.py` & `rockset-2.1.2/rockset/model/source_kinesis.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_mongo_db.py` & `rockset-2.1.2/rockset/model/source_mongo_db.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_s3.py` & `rockset-2.1.2/rockset/model/source_s3.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_s3_base.py` & `rockset-2.1.2/rockset/model/source_s3_base.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_s3_settings.py` & `rockset-2.1.2/rockset/model/source_s3_settings.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_snapshot.py` & `rockset-2.1.2/rockset/model/source_snapshot.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_snowflake.py` & `rockset-2.1.2/rockset/model/source_snowflake.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/source_system.py` & `rockset-2.1.2/rockset/model/source_system.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/sql_expression.py` & `rockset-2.1.2/rockset/model/sql_expression.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/stats.py` & `rockset-2.1.2/rockset/model/stats.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,26 +80,28 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'elapsed_time_ms': (int, none_type),  # noqa: E501
             'result_set_bytes_size': (int, none_type),  # noqa: E501
             'result_set_document_count': (int, none_type),  # noqa: E501
+            'result_set_file_count': (int, none_type),  # noqa: E501
             'throttled_time_ms': (int, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'elapsed_time_ms': 'elapsed_time_ms',  # noqa: E501
         'result_set_bytes_size': 'result_set_bytes_size',  # noqa: E501
         'result_set_document_count': 'result_set_document_count',  # noqa: E501
+        'result_set_file_count': 'result_set_file_count',  # noqa: E501
         'throttled_time_ms': 'throttled_time_ms',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
@@ -139,14 +141,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             elapsed_time_ms (int): Total execution time (including time queued) of the query, in milliseconds.. [optional]  # noqa: E501
             result_set_bytes_size (int): Number of bytes in the query result set. Only populated if `status` is `COMPLETE`. Not populated for INSERT INTO queries.. [optional]  # noqa: E501
             result_set_document_count (int): Number of documents returned by the query. Only populated if `status` is `COMPLETE`.. [optional]  # noqa: E501
+            result_set_file_count (int): Number of files written by by the query. Only populated if `status` is `COMPLETE` and the query is an export query.. [optional]  # noqa: E501
             throttled_time_ms (int): Time query spent queued, in milliseconds.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -194,14 +197,15 @@
     def __init__(self, **kwargs):  # noqa: E501
         """Stats - a model defined in OpenAPI
 
         Keyword Args:
             elapsed_time_ms (int): Total execution time (including time queued) of the query, in milliseconds.. [optional]  # noqa: E501
             result_set_bytes_size (int): Number of bytes in the query result set. Only populated if `status` is `COMPLETE`. Not populated for INSERT INTO queries.. [optional]  # noqa: E501
             result_set_document_count (int): Number of documents returned by the query. Only populated if `status` is `COMPLETE`.. [optional]  # noqa: E501
+            result_set_file_count (int): Number of files written by by the query. Only populated if `status` is `COMPLETE` and the query is an export query.. [optional]  # noqa: E501
             throttled_time_ms (int): Time query spent queued, in milliseconds.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
```

### Comparing `rockset-2.1.1/rockset/model/status.py` & `rockset-2.1.2/rockset/model/status.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/status_azure_event_hubs.py` & `rockset-2.1.2/rockset/model/status_azure_event_hubs.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/status_azure_event_hubs_partition.py` & `rockset-2.1.2/rockset/model/status_azure_event_hubs_partition.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/status_azure_service_bus.py` & `rockset-2.1.2/rockset/model/status_azure_service_bus.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/status_azure_service_bus_session.py` & `rockset-2.1.2/rockset/model/status_azure_service_bus_session.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/status_dynamo_db.py` & `rockset-2.1.2/rockset/model/status_dynamo_db.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/status_dynamo_db_v2.py` & `rockset-2.1.2/rockset/model/status_dynamo_db_v2.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/status_kafka.py` & `rockset-2.1.2/rockset/model/status_kafka.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/status_kafka_partition.py` & `rockset-2.1.2/rockset/model/status_kafka_partition.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/status_mongo_db.py` & `rockset-2.1.2/rockset/model/status_mongo_db.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/status_snowflake.py` & `rockset-2.1.2/rockset/model/status_snowflake.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/suspend_source_request.py` & `rockset-2.1.2/rockset/model/suspend_source_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/suspend_virtual_instance_response.py` & `rockset-2.1.2/rockset/model/suspend_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/tls_config.py` & `rockset-2.1.2/rockset/model/tls_config.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/unsubscribe_preference.py` & `rockset-2.1.2/rockset/model/unsubscribe_preference.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/update_alias_request.py` & `rockset-2.1.2/rockset/model/update_alias_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/update_api_key_request.py` & `rockset-2.1.2/rockset/model/update_api_key_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/update_api_key_response.py` & `rockset-2.1.2/rockset/model/update_api_key_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/update_collection_request.py` & `rockset-2.1.2/rockset/model/update_collection_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/update_integration_request.py` & `rockset-2.1.2/rockset/model/update_integration_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,14 +107,15 @@
         return {
             'azure_blob_storage': (AzureBlobStorageIntegration, none_type),  # noqa: E501
             'azure_event_hubs': (AzureEventHubsIntegration, none_type),  # noqa: E501
             'azure_service_bus': (AzureServiceBusIntegration, none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'dynamodb': (DynamodbIntegration, none_type),  # noqa: E501
             'gcs': (GcsIntegration, none_type),  # noqa: E501
+            'is_write_enabled': (bool, none_type),  # noqa: E501
             'kafka': (KafkaIntegration, none_type),  # noqa: E501
             'kinesis': (KinesisIntegration, none_type),  # noqa: E501
             'mongodb': (MongoDbIntegration, none_type),  # noqa: E501
             's3': (S3Integration, none_type),  # noqa: E501
             'snowflake': (SnowflakeIntegration, none_type),  # noqa: E501
         }
 
@@ -126,14 +127,15 @@
     attribute_map = {
         'azure_blob_storage': 'azure_blob_storage',  # noqa: E501
         'azure_event_hubs': 'azure_event_hubs',  # noqa: E501
         'azure_service_bus': 'azure_service_bus',  # noqa: E501
         'description': 'description',  # noqa: E501
         'dynamodb': 'dynamodb',  # noqa: E501
         'gcs': 'gcs',  # noqa: E501
+        'is_write_enabled': 'is_write_enabled',  # noqa: E501
         'kafka': 'kafka',  # noqa: E501
         'kinesis': 'kinesis',  # noqa: E501
         'mongodb': 'mongodb',  # noqa: E501
         's3': 's3',  # noqa: E501
         'snowflake': 'snowflake',  # noqa: E501
     }
 
@@ -180,14 +182,15 @@
                                 _visited_composed_classes = (Animal,)
             azure_blob_storage (AzureBlobStorageIntegration): [optional]  # noqa: E501
             azure_event_hubs (AzureEventHubsIntegration): [optional]  # noqa: E501
             azure_service_bus (AzureServiceBusIntegration): [optional]  # noqa: E501
             description (str): Longer explanation for the integration.. [optional]  # noqa: E501
             dynamodb (DynamodbIntegration): [optional]  # noqa: E501
             gcs (GcsIntegration): [optional]  # noqa: E501
+            is_write_enabled (bool): is write access enabled for this integration.. [optional]  # noqa: E501
             kafka (KafkaIntegration): [optional]  # noqa: E501
             kinesis (KinesisIntegration): [optional]  # noqa: E501
             mongodb (MongoDbIntegration): [optional]  # noqa: E501
             s3 (S3Integration): [optional]  # noqa: E501
             snowflake (SnowflakeIntegration): [optional]  # noqa: E501
         """
 
@@ -242,14 +245,15 @@
         Keyword Args:
             azure_blob_storage (AzureBlobStorageIntegration): [optional]  # noqa: E501
             azure_event_hubs (AzureEventHubsIntegration): [optional]  # noqa: E501
             azure_service_bus (AzureServiceBusIntegration): [optional]  # noqa: E501
             description (str): Longer explanation for the integration.. [optional]  # noqa: E501
             dynamodb (DynamodbIntegration): [optional]  # noqa: E501
             gcs (GcsIntegration): [optional]  # noqa: E501
+            is_write_enabled (bool): is write access enabled for this integration.. [optional]  # noqa: E501
             kafka (KafkaIntegration): [optional]  # noqa: E501
             kinesis (KinesisIntegration): [optional]  # noqa: E501
             mongodb (MongoDbIntegration): [optional]  # noqa: E501
             s3 (S3Integration): [optional]  # noqa: E501
             snowflake (SnowflakeIntegration): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
```

### Comparing `rockset-2.1.1/rockset/model/update_integration_response.py` & `rockset-2.1.2/rockset/model/update_integration_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/update_query_lambda_request.py` & `rockset-2.1.2/rockset/model/update_query_lambda_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/update_role_request.py` & `rockset-2.1.2/rockset/model/update_role_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/update_scheduled_lambda_request.py` & `rockset-2.1.2/rockset/model/create_scheduled_lambda_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 
-class UpdateScheduledLambdaRequest(ModelNormal):
+class CreateScheduledLambdaRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -77,45 +77,56 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'apikey': (str, none_type),  # noqa: E501
-            'resume_permanent_error': (bool, none_type),  # noqa: E501
+            'apikey': (str,),  # noqa: E501
+            'cron_string': (str,),  # noqa: E501
+            'ql_name': (str,),  # noqa: E501
+            'tag': (str, none_type),  # noqa: E501
             'total_times_to_execute': (int, none_type),  # noqa: E501
+            'version': (str, none_type),  # noqa: E501
             'webhook_auth_header': (str, none_type),  # noqa: E501
             'webhook_payload': (str, none_type),  # noqa: E501
             'webhook_url': (str, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'apikey': 'apikey',  # noqa: E501
-        'resume_permanent_error': 'resume_permanent_error',  # noqa: E501
+        'cron_string': 'cron_string',  # noqa: E501
+        'ql_name': 'ql_name',  # noqa: E501
+        'tag': 'tag',  # noqa: E501
         'total_times_to_execute': 'total_times_to_execute',  # noqa: E501
+        'version': 'version',  # noqa: E501
         'webhook_auth_header': 'webhook_auth_header',  # noqa: E501
         'webhook_payload': 'webhook_payload',  # noqa: E501
         'webhook_url': 'webhook_url',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
-    def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """UpdateScheduledLambdaRequest - a model defined in OpenAPI
+    def _from_openapi_data(cls, apikey, cron_string, ql_name, *args, **kwargs):  # noqa: E501
+        """CreateScheduledLambdaRequest - a model defined in OpenAPI
+
+        Args:
+            apikey (str): The apikey to use when triggering execution of the associated query lambda.
+            cron_string (str): The UNIX-formatted cron string for this scheduled query lambda.
+            ql_name (str): The name of the QL to use for scheduled execution.
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -140,17 +151,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            apikey (str): The apikey to use when triggering execution of the associated query lambda.. [optional]  # noqa: E501
-            resume_permanent_error (bool): Boolean flag to allow a scheduled query lambda to resume execution after being suspended due to execution failure. This flag will be unset after scheduled lambda execution.. [optional]  # noqa: E501
-            total_times_to_execute (int): The number of times to execute this scheduled query lambda.. [optional]  # noqa: E501
+            tag (str): The QL tag to use for scheduled execution. One of either the QL tag or version must be specified. [optional]  # noqa: E501
+            total_times_to_execute (int): The number of times to execute this scheduled query lambda. Once this scheduled query lambda has been executed this many times, it will no longer be executed.. [optional]  # noqa: E501
+            version (str): The version of the QL to use for scheduled execution. One of either the QL version or tag must be specified.. [optional]  # noqa: E501
             webhook_auth_header (str): The value to use as the authorization header when hitting the webhook.. [optional]  # noqa: E501
             webhook_payload (str): The payload that should be sent to the webhook. JSON format.. [optional]  # noqa: E501
             webhook_url (str): The URL of the webhook that should be triggered after this scheduled query lambda completes.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
@@ -173,14 +184,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.apikey = apikey
+        self.cron_string = cron_string
+        self.ql_name = ql_name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
@@ -193,21 +207,24 @@
         '_spec_property_naming',
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
-    def __init__(self, **kwargs):  # noqa: E501
-        """UpdateScheduledLambdaRequest - a model defined in OpenAPI
+    def __init__(self, *, apikey, cron_string, ql_name, **kwargs):  # noqa: E501
+        """CreateScheduledLambdaRequest - a model defined in OpenAPI
 
         Keyword Args:
-            apikey (str): The apikey to use when triggering execution of the associated query lambda.. [optional]  # noqa: E501
-            resume_permanent_error (bool): Boolean flag to allow a scheduled query lambda to resume execution after being suspended due to execution failure. This flag will be unset after scheduled lambda execution.. [optional]  # noqa: E501
-            total_times_to_execute (int): The number of times to execute this scheduled query lambda.. [optional]  # noqa: E501
+            apikey (str): The apikey to use when triggering execution of the associated query lambda.
+            cron_string (str): The UNIX-formatted cron string for this scheduled query lambda.
+            ql_name (str): The name of the QL to use for scheduled execution.
+            tag (str): The QL tag to use for scheduled execution. One of either the QL tag or version must be specified. [optional]  # noqa: E501
+            total_times_to_execute (int): The number of times to execute this scheduled query lambda. Once this scheduled query lambda has been executed this many times, it will no longer be executed.. [optional]  # noqa: E501
+            version (str): The version of the QL to use for scheduled execution. One of either the QL version or tag must be specified.. [optional]  # noqa: E501
             webhook_auth_header (str): The value to use as the authorization header when hitting the webhook.. [optional]  # noqa: E501
             webhook_payload (str): The payload that should be sent to the webhook. JSON format.. [optional]  # noqa: E501
             webhook_url (str): The URL of the webhook that should be triggered after this scheduled query lambda completes.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
@@ -259,14 +276,17 @@
         self._data_store = {}
         self._check_type = _check_type
         self._spec_property_naming = _spec_property_naming
         self._path_to_item = _path_to_item
         self._configuration = _configuration
         self._visited_composed_classes = _visited_composed_classes + (self.__class__,)
 
+        self.apikey = apikey
+        self.cron_string = cron_string
+        self.ql_name = ql_name
         for var_name, var_value in kwargs.items():
             if var_name not in self.attribute_map and \
                         self._configuration is not None and \
                         self._configuration.discard_unknown_keys and \
                         self.additional_properties_type is None:
                 # discard variable.
                 continue
```

### Comparing `rockset-2.1.1/rockset/model/update_unsubscribe_preferences_request.py` & `rockset-2.1.2/rockset/model/update_unsubscribe_preferences_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/update_unsubscribe_preferences_response.py` & `rockset-2.1.2/rockset/model/update_unsubscribe_preferences_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/update_user_request.py` & `rockset-2.1.2/rockset/model/update_user_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/update_view_request.py` & `rockset-2.1.2/rockset/model/update_view_request.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/update_view_response.py` & `rockset-2.1.2/rockset/model/update_view_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/update_virtual_instance_request.py` & `rockset-2.1.2/rockset/model/update_virtual_instance_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,17 @@
     OpenApiModel
 )
 from rockset.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from rockset.model.auto_scaling_policy import AutoScalingPolicy
+    from rockset.model.microbatch_policy import MicrobatchPolicy
     globals()['AutoScalingPolicy'] = AutoScalingPolicy
+    globals()['MicrobatchPolicy'] = MicrobatchPolicy
 
 
 class UpdateVirtualInstanceRequest(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -55,14 +57,18 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('instance_class',): {
+            'MO_IL': "MO_IL",
+            'GP_IL': "GP_IL",
+        },
         ('mount_type',): {
             'LIVE': "LIVE",
             'STATIC': "STATIC",
         },
         ('new_size',): {
             'FREE': "FREE",
             'NANO': "NANO",
@@ -107,14 +113,16 @@
         lazy_import()
         return {
             'auto_scaling_policy': (AutoScalingPolicy, none_type),  # noqa: E501
             'auto_suspend_enabled': (bool, none_type),  # noqa: E501
             'auto_suspend_seconds': (int, none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
             'enable_remount_on_resume': (bool, none_type),  # noqa: E501
+            'instance_class': (str, none_type),  # noqa: E501
+            'microbatch_policy': (MicrobatchPolicy, none_type),  # noqa: E501
             'mount_refresh_interval_seconds': (int, none_type),  # noqa: E501
             'mount_type': (str, none_type),  # noqa: E501
             'name': (str, none_type),  # noqa: E501
             'new_size': (str, none_type),  # noqa: E501
         }
 
     @cached_property
@@ -124,14 +132,16 @@
 
     attribute_map = {
         'auto_scaling_policy': 'auto_scaling_policy',  # noqa: E501
         'auto_suspend_enabled': 'auto_suspend_enabled',  # noqa: E501
         'auto_suspend_seconds': 'auto_suspend_seconds',  # noqa: E501
         'description': 'description',  # noqa: E501
         'enable_remount_on_resume': 'enable_remount_on_resume',  # noqa: E501
+        'instance_class': 'instance_class',  # noqa: E501
+        'microbatch_policy': 'microbatch_policy',  # noqa: E501
         'mount_refresh_interval_seconds': 'mount_refresh_interval_seconds',  # noqa: E501
         'mount_type': 'mount_type',  # noqa: E501
         'name': 'name',  # noqa: E501
         'new_size': 'new_size',  # noqa: E501
     }
 
     read_only_vars = {
@@ -176,16 +186,18 @@
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             auto_scaling_policy (AutoScalingPolicy): [optional]  # noqa: E501
             auto_suspend_enabled (bool): Whether Query VI auto-suspend should be enabled for this Virtual Instance.. [optional]  # noqa: E501
             auto_suspend_seconds (int): Number of seconds without queries after which the Query VI is suspended. [optional]  # noqa: E501
             description (str): New virtual instance description.. [optional]  # noqa: E501
             enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended.. [optional]  # noqa: E501
+            instance_class (str): Virtual Instance Class. Use `MO_IL` for Memory Optimized and `GP_IL` for General Purpose instance class.. [optional]  # noqa: E501
+            microbatch_policy (MicrobatchPolicy): [optional]  # noqa: E501
             mount_refresh_interval_seconds (int): DEPRECATED. Use `mount_type` instead. Number of seconds between data refreshes for mounts on this Virtual Instance. The only valid values are 0 and null. 0 means the data will be refreshed continuously and null means the data will never refresh.. [optional]  # noqa: E501
-            mount_type (str): The mount type of collections that this Virtual Instance will query. Live mounted collections stay up-to-date with the underlying collection in real-time. Static mounted collections do not stay up-to-date. See https://docs.rockset.com/documentation/docs/virtual-instances#virtual-instance-configuration. [optional]  # noqa: E501
+            mount_type (str): The mount type of collections that this Virtual Instance will query. Live mounted collections stay up-to-date with the underlying collection in real-time. Static mounted collections do not stay up-to-date. See https://docs.rockset.com/documentation/docs/using-virtual-instances#virtual-instance-configuration. [optional]  # noqa: E501
             name (str): New virtual instance name.. [optional]  # noqa: E501
             new_size (str): Requested virtual instance size.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -236,16 +248,18 @@
 
         Keyword Args:
             auto_scaling_policy (AutoScalingPolicy): [optional]  # noqa: E501
             auto_suspend_enabled (bool): Whether Query VI auto-suspend should be enabled for this Virtual Instance.. [optional]  # noqa: E501
             auto_suspend_seconds (int): Number of seconds without queries after which the Query VI is suspended. [optional]  # noqa: E501
             description (str): New virtual instance description.. [optional]  # noqa: E501
             enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended.. [optional]  # noqa: E501
+            instance_class (str): Virtual Instance Class. Use `MO_IL` for Memory Optimized and `GP_IL` for General Purpose instance class.. [optional]  # noqa: E501
+            microbatch_policy (MicrobatchPolicy): [optional]  # noqa: E501
             mount_refresh_interval_seconds (int): DEPRECATED. Use `mount_type` instead. Number of seconds between data refreshes for mounts on this Virtual Instance. The only valid values are 0 and null. 0 means the data will be refreshed continuously and null means the data will never refresh.. [optional]  # noqa: E501
-            mount_type (str): The mount type of collections that this Virtual Instance will query. Live mounted collections stay up-to-date with the underlying collection in real-time. Static mounted collections do not stay up-to-date. See https://docs.rockset.com/documentation/docs/virtual-instances#virtual-instance-configuration. [optional]  # noqa: E501
+            mount_type (str): The mount type of collections that this Virtual Instance will query. Live mounted collections stay up-to-date with the underlying collection in real-time. Static mounted collections do not stay up-to-date. See https://docs.rockset.com/documentation/docs/using-virtual-instances#virtual-instance-configuration. [optional]  # noqa: E501
             name (str): New virtual instance name.. [optional]  # noqa: E501
             new_size (str): Requested virtual instance size.. [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `rockset-2.1.1/rockset/model/update_virtual_instance_response.py` & `rockset-2.1.2/rockset/model/update_virtual_instance_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/user.py` & `rockset-2.1.2/rockset/model/user.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/validate_query_response.py` & `rockset-2.1.2/rockset/model/validate_query_response.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/view.py` & `rockset-2.1.2/rockset/model/view.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/virtual_instance.py` & `rockset-2.1.2/rockset/model/virtual_instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,19 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
     
     allowed_values = {
+        ('current_instance_class',): {
+            'MO_BR': "MO_BR",
+            'MO_IL': "MO_IL",
+            'GP_IL': "GP_IL",
+        },
         ('current_size',): {
             'FREE': "FREE",
             'NANO': "NANO",
             'SHARED': "SHARED",
             'MILLI': "MILLI",
             'XSMALL': "XSMALL",
             'SMALL': "SMALL",
@@ -72,14 +77,19 @@
             'LARGE': "LARGE",
             'XLARGE': "XLARGE",
             'XLARGE2': "XLARGE2",
             'XLARGE4': "XLARGE4",
             'XLARGE8': "XLARGE8",
             'XLARGE16': "XLARGE16",
         },
+        ('desired_instance_class',): {
+            'MO_BR': "MO_BR",
+            'MO_IL': "MO_IL",
+            'GP_IL': "GP_IL",
+        },
         ('desired_size',): {
             'FREE': "FREE",
             'NANO': "NANO",
             'SHARED': "SHARED",
             'MILLI': "MILLI",
             'XSMALL': "XSMALL",
             'SMALL': "SMALL",
@@ -136,27 +146,27 @@
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
             'auto_scaling_policy': (AutoScalingPolicy, none_type),  # noqa: E501
             'auto_suspend_seconds': (int, none_type),  # noqa: E501
             'created_at': (str, none_type),  # noqa: E501
             'created_by': (str, none_type),  # noqa: E501
+            'current_instance_class': (str, none_type),  # noqa: E501
             'current_size': (str, none_type),  # noqa: E501
-            'default_pod_count': (int, none_type),  # noqa: E501
             'default_vi': (bool, none_type),  # noqa: E501
             'description': (str, none_type),  # noqa: E501
+            'desired_instance_class': (str, none_type),  # noqa: E501
             'desired_size': (str, none_type),  # noqa: E501
             'enable_remount_on_resume': (bool, none_type),  # noqa: E501
             'id': (str, none_type),  # noqa: E501
             'monitoring_enabled': (bool, none_type),  # noqa: E501
             'mount_refresh_interval_seconds': (int, none_type),  # noqa: E501
             'mount_type': (str, none_type),  # noqa: E501
             'resumed_at': (str, none_type),  # noqa: E501
             'rrn': (str, none_type),  # noqa: E501
-            'scaled_pod_count': (int, none_type),  # noqa: E501
             'state': (str, none_type),  # noqa: E501
             'stats': (VirtualInstanceStats, none_type),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -164,27 +174,27 @@
 
     attribute_map = {
         'name': 'name',  # noqa: E501
         'auto_scaling_policy': 'auto_scaling_policy',  # noqa: E501
         'auto_suspend_seconds': 'auto_suspend_seconds',  # noqa: E501
         'created_at': 'created_at',  # noqa: E501
         'created_by': 'created_by',  # noqa: E501
+        'current_instance_class': 'current_instance_class',  # noqa: E501
         'current_size': 'current_size',  # noqa: E501
-        'default_pod_count': 'default_pod_count',  # noqa: E501
         'default_vi': 'default_vi',  # noqa: E501
         'description': 'description',  # noqa: E501
+        'desired_instance_class': 'desired_instance_class',  # noqa: E501
         'desired_size': 'desired_size',  # noqa: E501
         'enable_remount_on_resume': 'enable_remount_on_resume',  # noqa: E501
         'id': 'id',  # noqa: E501
         'monitoring_enabled': 'monitoring_enabled',  # noqa: E501
         'mount_refresh_interval_seconds': 'mount_refresh_interval_seconds',  # noqa: E501
         'mount_type': 'mount_type',  # noqa: E501
         'resumed_at': 'resumed_at',  # noqa: E501
         'rrn': 'rrn',  # noqa: E501
-        'scaled_pod_count': 'scaled_pod_count',  # noqa: E501
         'state': 'state',  # noqa: E501
         'stats': 'stats',  # noqa: E501
     }
 
     read_only_vars = {
         'current_size',  # noqa: E501
         'desired_size',  # noqa: E501
@@ -231,27 +241,27 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             auto_scaling_policy (AutoScalingPolicy): [optional]  # noqa: E501
             auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]  # noqa: E501
             created_at (str): ISO-8601 date of when virtual instance was created.. [optional]  # noqa: E501
             created_by (str): Creator of requested virtual instance.. [optional]  # noqa: E501
+            current_instance_class (str): Virtual Instance Class. `MO_IL` represents Memory Optimized and `GP_IL` represents General Purpose instance class.. [optional]  # noqa: E501
             current_size (str): Virtual instance current size.. [optional]  # noqa: E501
-            default_pod_count (int): [optional]  # noqa: E501
             default_vi (bool): [optional]  # noqa: E501
             description (str): Virtual instance description.. [optional]  # noqa: E501
+            desired_instance_class (str): Virtual Instance Class.. [optional]  # noqa: E501
             desired_size (str): Virtual instance desired size.. [optional]  # noqa: E501
             enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended.. [optional]  # noqa: E501
             id (str): Unique identifier for virtual instance.. [optional]  # noqa: E501
             monitoring_enabled (bool): [optional]  # noqa: E501
             mount_refresh_interval_seconds (int): DEPRECATED. Number of seconds between data refreshes for mounts on this Virtual Instance. [optional]  # noqa: E501
-            mount_type (str): The mount type of collections that this Virtual Instance will query. Live mounted collections stay up-to-date with the underlying collection in real-time. Static mounted collections do not stay up-to-date. See https://docs.rockset.com/documentation/docs/virtual-instances#virtual-instance-configuration. [optional]  # noqa: E501
+            mount_type (str): The mount type of collections that this Virtual Instance will query. Live mounted collections stay up-to-date with the underlying collection in real-time. Static mounted collections do not stay up-to-date. See https://docs.rockset.com/documentation/docs/using-virtual-instances#virtual-instance-configuration. [optional]  # noqa: E501
             resumed_at (str): ISO-8601 date of when virtual instance was created.. [optional]  # noqa: E501
             rrn (str): Virtual Instance RRN.. [optional]  # noqa: E501
-            scaled_pod_count (int): [optional]  # noqa: E501
             state (str): Virtual instance state.. [optional]  # noqa: E501
             stats (VirtualInstanceStats): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -303,25 +313,25 @@
 
         Keyword Args:
             name (str): Virtual instance name.
             auto_scaling_policy (AutoScalingPolicy): [optional]  # noqa: E501
             auto_suspend_seconds (int): Number of seconds without queries after which the VI is suspended. [optional]  # noqa: E501
             created_at (str): ISO-8601 date of when virtual instance was created.. [optional]  # noqa: E501
             created_by (str): Creator of requested virtual instance.. [optional]  # noqa: E501
-            default_pod_count (int): [optional]  # noqa: E501
+            current_instance_class (str): Virtual Instance Class. `MO_IL` represents Memory Optimized and `GP_IL` represents General Purpose instance class.. [optional]  # noqa: E501
             default_vi (bool): [optional]  # noqa: E501
             description (str): Virtual instance description.. [optional]  # noqa: E501
+            desired_instance_class (str): Virtual Instance Class.. [optional]  # noqa: E501
             enable_remount_on_resume (bool): When a Virtual Instance is resumed, it will remount all collections that were mounted when the Virtual Instance was suspended.. [optional]  # noqa: E501
             id (str): Unique identifier for virtual instance.. [optional]  # noqa: E501
             monitoring_enabled (bool): [optional]  # noqa: E501
             mount_refresh_interval_seconds (int): DEPRECATED. Number of seconds between data refreshes for mounts on this Virtual Instance. [optional]  # noqa: E501
-            mount_type (str): The mount type of collections that this Virtual Instance will query. Live mounted collections stay up-to-date with the underlying collection in real-time. Static mounted collections do not stay up-to-date. See https://docs.rockset.com/documentation/docs/virtual-instances#virtual-instance-configuration. [optional]  # noqa: E501
+            mount_type (str): The mount type of collections that this Virtual Instance will query. Live mounted collections stay up-to-date with the underlying collection in real-time. Static mounted collections do not stay up-to-date. See https://docs.rockset.com/documentation/docs/using-virtual-instances#virtual-instance-configuration. [optional]  # noqa: E501
             resumed_at (str): ISO-8601 date of when virtual instance was created.. [optional]  # noqa: E501
             rrn (str): Virtual Instance RRN.. [optional]  # noqa: E501
-            scaled_pod_count (int): [optional]  # noqa: E501
             state (str): Virtual instance state.. [optional]  # noqa: E501
             stats (VirtualInstanceStats): [optional]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `rockset-2.1.1/rockset/model/virtual_instance_rrn.py` & `rockset-2.1.2/rockset/model/virtual_instance_rrn.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/virtual_instance_stats.py` & `rockset-2.1.2/rockset/model/virtual_instance_stats.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/workspace.py` & `rockset-2.1.2/rockset/model/workspace.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model/xml_params.py` & `rockset-2.1.2/rockset/model/xml_params.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/model_utils.py` & `rockset-2.1.2/rockset/model_utils.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/models/__init__.py` & `rockset-2.1.2/rockset/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,14 +66,16 @@
 from rockset.model.delete_integration_response import DeleteIntegrationResponse
 from rockset.model.delete_query_lambda_response import DeleteQueryLambdaResponse
 from rockset.model.delete_source_response import DeleteSourceResponse
 from rockset.model.delete_user_response import DeleteUserResponse
 from rockset.model.delete_view_response import DeleteViewResponse
 from rockset.model.delete_virtual_instance_response import DeleteVirtualInstanceResponse
 from rockset.model.delete_workspace_response import DeleteWorkspaceResponse
+from rockset.model.deployment_settings import DeploymentSettings
+from rockset.model.deployment_settings_response import DeploymentSettingsResponse
 from rockset.model.document_status import DocumentStatus
 from rockset.model.dynamodb_collection_creation_request import DynamodbCollectionCreationRequest
 from rockset.model.dynamodb_integration import DynamodbIntegration
 from rockset.model.dynamodb_integration_creation_request import DynamodbIntegrationCreationRequest
 from rockset.model.dynamodb_source_wrapper import DynamodbSourceWrapper
 from rockset.model.error_model import ErrorModel
 from rockset.model.event_time_info import EventTimeInfo
@@ -118,20 +120,22 @@
 from rockset.model.list_collections_response import ListCollectionsResponse
 from rockset.model.list_integrations_response import ListIntegrationsResponse
 from rockset.model.list_queries_response import ListQueriesResponse
 from rockset.model.list_query_lambda_tags_response import ListQueryLambdaTagsResponse
 from rockset.model.list_query_lambda_versions_response import ListQueryLambdaVersionsResponse
 from rockset.model.list_query_lambdas_response import ListQueryLambdasResponse
 from rockset.model.list_roles_response import ListRolesResponse
+from rockset.model.list_scheduled_lambdas_response import ListScheduledLambdasResponse
 from rockset.model.list_sources_response import ListSourcesResponse
 from rockset.model.list_unsubscribe_preferences_response import ListUnsubscribePreferencesResponse
 from rockset.model.list_users_response import ListUsersResponse
 from rockset.model.list_views_response import ListViewsResponse
 from rockset.model.list_virtual_instances_response import ListVirtualInstancesResponse
 from rockset.model.list_workspaces_response import ListWorkspacesResponse
+from rockset.model.microbatch_policy import MicrobatchPolicy
 from rockset.model.mongo_db_integration import MongoDbIntegration
 from rockset.model.mongodb_collection_creation_request import MongodbCollectionCreationRequest
 from rockset.model.mongodb_integration_creation_request import MongodbIntegrationCreationRequest
 from rockset.model.mongodb_source_wrapper import MongodbSourceWrapper
 from rockset.model.offsets import Offsets
 from rockset.model.organization import Organization
 from rockset.model.organization_response import OrganizationResponse
@@ -213,14 +217,15 @@
 from rockset.model.suspend_virtual_instance_response import SuspendVirtualInstanceResponse
 from rockset.model.tls_config import TLSConfig
 from rockset.model.unsubscribe_preference import UnsubscribePreference
 from rockset.model.update_alias_request import UpdateAliasRequest
 from rockset.model.update_api_key_request import UpdateApiKeyRequest
 from rockset.model.update_api_key_response import UpdateApiKeyResponse
 from rockset.model.update_collection_request import UpdateCollectionRequest
+from rockset.model.update_deployment_settings_request import UpdateDeploymentSettingsRequest
 from rockset.model.update_integration_request import UpdateIntegrationRequest
 from rockset.model.update_integration_response import UpdateIntegrationResponse
 from rockset.model.update_query_lambda_request import UpdateQueryLambdaRequest
 from rockset.model.update_role_request import UpdateRoleRequest
 from rockset.model.update_scheduled_lambda_request import UpdateScheduledLambdaRequest
 from rockset.model.update_unsubscribe_preferences_request import UpdateUnsubscribePreferencesRequest
 from rockset.model.update_unsubscribe_preferences_response import UpdateUnsubscribePreferencesResponse
@@ -229,11 +234,10 @@
 from rockset.model.update_view_response import UpdateViewResponse
 from rockset.model.update_virtual_instance_request import UpdateVirtualInstanceRequest
 from rockset.model.update_virtual_instance_response import UpdateVirtualInstanceResponse
 from rockset.model.user import User
 from rockset.model.validate_query_response import ValidateQueryResponse
 from rockset.model.view import View
 from rockset.model.virtual_instance import VirtualInstance
-from rockset.model.virtual_instance_rrn import VirtualInstanceRrn
 from rockset.model.virtual_instance_stats import VirtualInstanceStats
 from rockset.model.workspace import Workspace
 from rockset.model.xml_params import XmlParams
```

### Comparing `rockset-2.1.1/rockset/query_paginator.py` & `rockset-2.1.2/rockset/query_paginator.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/rest.py` & `rockset-2.1.2/rockset/rest.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/rockset/rockset_client.py` & `rockset-2.1.2/rockset/rockset_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,18 @@
     pass
 
 
 class CustomRolesApiWrapper(apis.CustomRoles, metaclass=ApiMetaclass):
     pass
 
 
+class DeploymentSettingsApiWrapper(apis.DeploymentSettings, metaclass=ApiMetaclass):
+    pass
+
+
 class DocumentsApiWrapper(apis.Documents, metaclass=ApiMetaclass):
     pass
 
 
 class IntegrationsApiWrapper(apis.Integrations, metaclass=ApiMetaclass):
     pass
 
@@ -247,14 +251,15 @@
 
         self.api_client = ApiClient(config, max_workers=max_workers)
 
         self.APIKeys = APIKeysApiWrapper(self.api_client)
         self.Aliases = AliasesApiWrapper(self.api_client)
         self.Collections = CollectionsApiWrapper(self.api_client)
         self.CustomRoles = CustomRolesApiWrapper(self.api_client)
+        self.DeploymentSettings = DeploymentSettingsApiWrapper(self.api_client)
         self.Documents = DocumentsApiWrapper(self.api_client)
         self.Integrations = IntegrationsApiWrapper(self.api_client)
         self.Organizations = OrganizationsApiWrapper(self.api_client)
         self.Queries = QueriesApiWrapper(self.api_client)
         self.QueryLambdas = QueryLambdasApiWrapper(self.api_client)
         self.ScheduledLambdas = ScheduledLambdasApiWrapper(self.api_client)
         self.SharedLambdas = SharedLambdasApiWrapper(self.api_client)
```

### Comparing `rockset-2.1.1/rockset/value.py` & `rockset-2.1.2/rockset/value.py`

 * *Files identical despite different names*

### Comparing `rockset-2.1.1/PKG-INFO` & `rockset-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockset
-Version: 2.1.1
+Version: 2.1.2
 Summary: The python client for the Rockset API.
 Home-page: https://github.com/rockset/rockset-python-client
 License: Apache-2.0
 Author: Rockset
 Author-email: support@rockset.com
 Requires-Python: >=3.6,<4.0
 Classifier: Environment :: Console
```

