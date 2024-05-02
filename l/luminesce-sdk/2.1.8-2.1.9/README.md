# Comparing `tmp/luminesce_sdk-2.1.8.tar.gz` & `tmp/luminesce_sdk-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luminesce_sdk-2.1.8.tar", max compression
+gzip compressed data, was "luminesce_sdk-2.1.9.tar", max compression
```

## Comparing `luminesce_sdk-2.1.8.tar` & `luminesce_sdk-2.1.9.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0    21798 2024-04-13 04:24:02.192720 luminesce_sdk-2.1.8/README.md
--rw-r--r--   0        0        0     8148 2024-04-13 04:24:02.187720 luminesce_sdk-2.1.8/luminesce/__init__.py
--rw-r--r--   0        0        0     1000 2024-04-13 04:24:02.187720 luminesce_sdk-2.1.8/luminesce/api/__init__.py
--rw-r--r--   0        0        0     8544 2024-04-13 04:24:02.186720 luminesce_sdk-2.1.8/luminesce/api/application_metadata_api.py
--rw-r--r--   0        0        0    12078 2024-04-13 04:24:02.186720 luminesce_sdk-2.1.8/luminesce/api/binary_downloading_api.py
--rw-r--r--   0        0        0    31272 2024-04-13 04:24:02.186720 luminesce_sdk-2.1.8/luminesce/api/certificate_management_api.py
--rw-r--r--   0        0        0    11804 2024-04-13 04:24:02.186720 luminesce_sdk-2.1.8/luminesce/api/current_table_field_catalog_api.py
--rw-r--r--   0        0        0    66234 2024-04-13 04:24:02.186720 luminesce_sdk-2.1.8/luminesce/api/historically_executed_queries_api.py
--rw-r--r--   0        0        0    38562 2024-04-13 04:24:02.186720 luminesce_sdk-2.1.8/luminesce/api/multi_query_execution_api.py
--rw-r--r--   0        0        0   238147 2024-04-13 04:24:02.187720 luminesce_sdk-2.1.8/luminesce/api/sql_background_execution_api.py
--rw-r--r--   0        0        0   104257 2024-04-13 04:24:02.187720 luminesce_sdk-2.1.8/luminesce/api/sql_design_api.py
--rw-r--r--   0        0        0   148001 2024-04-13 04:24:02.187720 luminesce_sdk-2.1.8/luminesce/api/sql_execution_api.py
--rw-r--r--   0        0        0    30755 2024-04-13 04:24:02.187720 luminesce_sdk-2.1.8/luminesce/api_client.py
--rw-r--r--   0        0        0      852 2024-04-13 04:24:02.187720 luminesce_sdk-2.1.8/luminesce/api_response.py
--rw-r--r--   0        0        0    14448 2024-04-13 04:24:02.187720 luminesce_sdk-2.1.8/luminesce/configuration.py
--rw-r--r--   0        0        0     5344 2024-04-13 04:24:02.187720 luminesce_sdk-2.1.8/luminesce/exceptions.py
--rw-r--r--   0        0        0      572 2024-04-13 04:24:02.188720 luminesce_sdk-2.1.8/luminesce/extensions/__init__.py
--rw-r--r--   0        0        0    30617 2024-04-13 04:24:02.188720 luminesce_sdk-2.1.8/luminesce/extensions/api_client.py
--rw-r--r--   0        0        0     9812 2024-04-13 04:24:02.188720 luminesce_sdk-2.1.8/luminesce/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8072 2024-04-13 04:24:02.188720 luminesce_sdk-2.1.8/luminesce/extensions/api_configuration.py
--rw-r--r--   0        0        0     6776 2024-04-13 04:24:02.188720 luminesce_sdk-2.1.8/luminesce/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-04-13 04:24:02.188720 luminesce_sdk-2.1.8/luminesce/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-04-13 04:24:02.188720 luminesce_sdk-2.1.8/luminesce/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12702 2024-04-13 04:24:02.188720 luminesce_sdk-2.1.8/luminesce/extensions/rest.py
--rw-r--r--   0        0        0    11568 2024-04-13 04:24:02.188720 luminesce_sdk-2.1.8/luminesce/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-04-13 04:24:02.188720 luminesce_sdk-2.1.8/luminesce/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3881 2024-04-13 04:24:02.188720 luminesce_sdk-2.1.8/luminesce/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     6159 2024-04-13 04:24:02.186720 luminesce_sdk-2.1.8/luminesce/models/__init__.py
--rw-r--r--   0        0        0     3399 2024-04-13 04:24:02.182721 luminesce_sdk-2.1.8/luminesce/models/access_controlled_action.py
--rw-r--r--   0        0        0     4674 2024-04-13 04:24:02.182721 luminesce_sdk-2.1.8/luminesce/models/access_controlled_resource.py
--rw-r--r--   0        0        0     3963 2024-04-13 04:24:02.182721 luminesce_sdk-2.1.8/luminesce/models/access_controlled_resource_identifier_part_schema_attribute.py
--rw-r--r--   0        0        0     2075 2024-04-13 04:24:02.182721 luminesce_sdk-2.1.8/luminesce/models/action_id.py
--rw-r--r--   0        0        0      828 2024-04-13 04:24:02.182721 luminesce_sdk-2.1.8/luminesce/models/aggregate_function.py
--rw-r--r--   0        0        0     2318 2024-04-13 04:24:02.182721 luminesce_sdk-2.1.8/luminesce/models/aggregation.py
--rw-r--r--   0        0        0      802 2024-04-13 04:24:02.182721 luminesce_sdk-2.1.8/luminesce/models/auto_detect_type.py
--rw-r--r--   0        0        0     3207 2024-04-13 04:24:02.182721 luminesce_sdk-2.1.8/luminesce/models/available_field.py
--rw-r--r--   0        0        0     2939 2024-04-13 04:24:02.182721 luminesce_sdk-2.1.8/luminesce/models/available_parameter.py
--rw-r--r--   0        0        0     4237 2024-04-13 04:24:02.182721 luminesce_sdk-2.1.8/luminesce/models/background_multi_query_progress_response.py
--rw-r--r--   0        0        0    10653 2024-04-13 04:24:02.182721 luminesce_sdk-2.1.8/luminesce/models/background_multi_query_response.py
--rw-r--r--   0        0        0     2760 2024-04-13 04:24:02.182721 luminesce_sdk-2.1.8/luminesce/models/background_query_cancel_response.py
--rw-r--r--   0        0        0     5677 2024-04-13 04:24:02.183720 luminesce_sdk-2.1.8/luminesce/models/background_query_progress_response.py
--rw-r--r--   0        0        0     6285 2024-04-13 04:24:02.183720 luminesce_sdk-2.1.8/luminesce/models/background_query_response.py
--rw-r--r--   0        0        0     1055 2024-04-13 04:24:02.183720 luminesce_sdk-2.1.8/luminesce/models/background_query_state.py
--rw-r--r--   0        0        0      808 2024-04-13 04:24:02.183720 luminesce_sdk-2.1.8/luminesce/models/certificate_action.py
--rw-r--r--   0        0        0      778 2024-04-13 04:24:02.183720 luminesce_sdk-2.1.8/luminesce/models/certificate_file_type.py
--rw-r--r--   0        0        0     7171 2024-04-13 04:24:02.183720 luminesce_sdk-2.1.8/luminesce/models/certificate_state.py
--rw-r--r--   0        0        0      847 2024-04-13 04:24:02.183720 luminesce_sdk-2.1.8/luminesce/models/certificate_status.py
--rw-r--r--   0        0        0      716 2024-04-13 04:24:02.183720 luminesce_sdk-2.1.8/luminesce/models/certificate_type.py
--rw-r--r--   0        0        0     5108 2024-04-13 04:24:02.183720 luminesce_sdk-2.1.8/luminesce/models/column.py
--rw-r--r--   0        0        0     2859 2024-04-13 04:24:02.183720 luminesce_sdk-2.1.8/luminesce/models/column_info.py
--rw-r--r--   0        0        0      738 2024-04-13 04:24:02.184720 luminesce_sdk-2.1.8/luminesce/models/condition_attributes.py
--rw-r--r--   0        0        0     5193 2024-04-13 04:24:02.184720 luminesce_sdk-2.1.8/luminesce/models/convert_to_view_data.py
--rw-r--r--   0        0        0     2055 2024-04-13 04:24:02.184720 luminesce_sdk-2.1.8/luminesce/models/cursor_position.py
--rw-r--r--   0        0        0      789 2024-04-13 04:24:02.184720 luminesce_sdk-2.1.8/luminesce/models/data_type.py
--rw-r--r--   0        0        0     3345 2024-04-13 04:24:02.184720 luminesce_sdk-2.1.8/luminesce/models/error_highlight_item.py
--rw-r--r--   0        0        0     2386 2024-04-13 04:24:02.184720 luminesce_sdk-2.1.8/luminesce/models/error_highlight_request.py
--rw-r--r--   0        0        0     2702 2024-04-13 04:24:02.184720 luminesce_sdk-2.1.8/luminesce/models/error_highlight_response.py
--rw-r--r--   0        0        0     2589 2024-04-13 04:24:02.184720 luminesce_sdk-2.1.8/luminesce/models/expression_with_alias.py
--rw-r--r--   0        0        0     4095 2024-04-13 04:24:02.184720 luminesce_sdk-2.1.8/luminesce/models/feedback_event_args.py
--rw-r--r--   0        0        0      994 2024-04-13 04:24:02.184720 luminesce_sdk-2.1.8/luminesce/models/feedback_level.py
--rw-r--r--   0        0        0     4548 2024-04-13 04:24:02.184720 luminesce_sdk-2.1.8/luminesce/models/field_design.py
--rw-r--r--   0        0        0      654 2024-04-13 04:24:02.184720 luminesce_sdk-2.1.8/luminesce/models/field_type.py
--rw-r--r--   0        0        0     8355 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/file_reader_builder_def.py
--rw-r--r--   0        0        0     3731 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/file_reader_builder_response.py
--rw-r--r--   0        0        0     2210 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/filter_term_design.py
--rw-r--r--   0        0        0     3180 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/id_selector_definition.py
--rw-r--r--   0        0        0     3236 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/intellisense_item.py
--rw-r--r--   0        0        0     2405 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/intellisense_request.py
--rw-r--r--   0        0        0     3144 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/intellisense_response.py
--rw-r--r--   0        0        0      807 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/intellisense_type.py
--rw-r--r--   0        0        0     2267 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/link.py
--rw-r--r--   0        0        0     1656 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/luminesce_binary_type.py
--rw-r--r--   0        0        0     3862 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/lusid_problem_details.py
--rw-r--r--   0        0        0     5204 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/mappable_field.py
--rw-r--r--   0        0        0      711 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/mapping_flags.py
--rw-r--r--   0        0        0     1099 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/multi_query_definition_type.py
--rw-r--r--   0        0        0     6322 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/options_csv.py
--rw-r--r--   0        0        0     5383 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/options_excel.py
--rw-r--r--   0        0        0     2313 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/options_parquet.py
--rw-r--r--   0        0        0     2219 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/options_sq_lite.py
--rw-r--r--   0        0        0     4491 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/options_xml.py
--rw-r--r--   0        0        0      707 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/order_by_direction.py
--rw-r--r--   0        0        0     2149 2024-04-13 04:24:02.185721 luminesce_sdk-2.1.8/luminesce/models/order_by_term_design.py
--rw-r--r--   0        0        0     5696 2024-04-13 04:24:02.186720 luminesce_sdk-2.1.8/luminesce/models/query_design.py
--rw-r--r--   0        0        0      884 2024-04-13 04:24:02.186720 luminesce_sdk-2.1.8/luminesce/models/query_designer_binary_operator.py
--rw-r--r--   0        0        0     4250 2024-04-13 04:24:02.186720 luminesce_sdk-2.1.8/luminesce/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     2328 2024-04-13 04:24:02.186720 luminesce_sdk-2.1.8/luminesce/models/source.py
--rw-r--r--   0        0        0      770 2024-04-13 04:24:02.186720 luminesce_sdk-2.1.8/luminesce/models/source_type.py
--rw-r--r--   0        0        0      897 2024-04-13 04:24:02.186720 luminesce_sdk-2.1.8/luminesce/models/task_status.py
--rw-r--r--   0        0        0     2991 2024-04-13 04:24:02.186720 luminesce_sdk-2.1.8/luminesce/models/view_parameter.py
--rw-r--r--   0        0        0     4494 2024-04-13 04:24:02.186720 luminesce_sdk-2.1.8/luminesce/models/writer_design.py
--rw-r--r--   0        0        0        0 2024-04-13 04:24:02.187720 luminesce_sdk-2.1.8/luminesce/py.typed
--rw-r--r--   0        0        0    10160 2024-04-13 04:24:02.188720 luminesce_sdk-2.1.8/luminesce/rest.py
--rw-r--r--   0        0        0      846 2024-04-13 04:24:02.193720 luminesce_sdk-2.1.8/pyproject.toml
--rw-r--r--   0        0        0    22845 1970-01-01 00:00:00.000000 luminesce_sdk-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0    21798 2024-04-17 13:57:51.570968 luminesce_sdk-2.1.9/README.md
+-rw-r--r--   0        0        0     8148 2024-04-17 13:57:51.565968 luminesce_sdk-2.1.9/luminesce/__init__.py
+-rw-r--r--   0        0        0     1000 2024-04-17 13:57:51.565968 luminesce_sdk-2.1.9/luminesce/api/__init__.py
+-rw-r--r--   0        0        0     8544 2024-04-17 13:57:51.564968 luminesce_sdk-2.1.9/luminesce/api/application_metadata_api.py
+-rw-r--r--   0        0        0    12078 2024-04-17 13:57:51.564968 luminesce_sdk-2.1.9/luminesce/api/binary_downloading_api.py
+-rw-r--r--   0        0        0    31272 2024-04-17 13:57:51.564968 luminesce_sdk-2.1.9/luminesce/api/certificate_management_api.py
+-rw-r--r--   0        0        0    11804 2024-04-17 13:57:51.564968 luminesce_sdk-2.1.9/luminesce/api/current_table_field_catalog_api.py
+-rw-r--r--   0        0        0    66234 2024-04-17 13:57:51.565968 luminesce_sdk-2.1.9/luminesce/api/historically_executed_queries_api.py
+-rw-r--r--   0        0        0    38562 2024-04-17 13:57:51.565968 luminesce_sdk-2.1.9/luminesce/api/multi_query_execution_api.py
+-rw-r--r--   0        0        0   238147 2024-04-17 13:57:51.565968 luminesce_sdk-2.1.9/luminesce/api/sql_background_execution_api.py
+-rw-r--r--   0        0        0   104257 2024-04-17 13:57:51.565968 luminesce_sdk-2.1.9/luminesce/api/sql_design_api.py
+-rw-r--r--   0        0        0   148001 2024-04-17 13:57:51.565968 luminesce_sdk-2.1.9/luminesce/api/sql_execution_api.py
+-rw-r--r--   0        0        0    30755 2024-04-17 13:57:51.563968 luminesce_sdk-2.1.9/luminesce/api_client.py
+-rw-r--r--   0        0        0      852 2024-04-17 13:57:51.563968 luminesce_sdk-2.1.9/luminesce/api_response.py
+-rw-r--r--   0        0        0    14448 2024-04-17 13:57:51.565968 luminesce_sdk-2.1.9/luminesce/configuration.py
+-rw-r--r--   0        0        0     5344 2024-04-17 13:57:51.565968 luminesce_sdk-2.1.9/luminesce/exceptions.py
+-rw-r--r--   0        0        0      572 2024-04-17 13:57:51.564968 luminesce_sdk-2.1.9/luminesce/extensions/__init__.py
+-rw-r--r--   0        0        0    30617 2024-04-17 13:57:51.564968 luminesce_sdk-2.1.9/luminesce/extensions/api_client.py
+-rw-r--r--   0        0        0     9812 2024-04-17 13:57:51.564968 luminesce_sdk-2.1.9/luminesce/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8072 2024-04-17 13:57:51.564968 luminesce_sdk-2.1.9/luminesce/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6776 2024-04-17 13:57:51.564968 luminesce_sdk-2.1.9/luminesce/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-04-17 13:57:51.564968 luminesce_sdk-2.1.9/luminesce/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-04-17 13:57:51.564968 luminesce_sdk-2.1.9/luminesce/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12702 2024-04-17 13:57:51.564968 luminesce_sdk-2.1.9/luminesce/extensions/rest.py
+-rw-r--r--   0        0        0    11568 2024-04-17 13:57:51.564968 luminesce_sdk-2.1.9/luminesce/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-04-17 13:57:51.564968 luminesce_sdk-2.1.9/luminesce/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3881 2024-04-17 13:57:51.564968 luminesce_sdk-2.1.9/luminesce/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     6159 2024-04-17 13:57:51.563968 luminesce_sdk-2.1.9/luminesce/models/__init__.py
+-rw-r--r--   0        0        0     3399 2024-04-17 13:57:51.559968 luminesce_sdk-2.1.9/luminesce/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4674 2024-04-17 13:57:51.560968 luminesce_sdk-2.1.9/luminesce/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     3963 2024-04-17 13:57:51.560968 luminesce_sdk-2.1.9/luminesce/models/access_controlled_resource_identifier_part_schema_attribute.py
+-rw-r--r--   0        0        0     2075 2024-04-17 13:57:51.560968 luminesce_sdk-2.1.9/luminesce/models/action_id.py
+-rw-r--r--   0        0        0      828 2024-04-17 13:57:51.560968 luminesce_sdk-2.1.9/luminesce/models/aggregate_function.py
+-rw-r--r--   0        0        0     2318 2024-04-17 13:57:51.560968 luminesce_sdk-2.1.9/luminesce/models/aggregation.py
+-rw-r--r--   0        0        0      802 2024-04-17 13:57:51.560968 luminesce_sdk-2.1.9/luminesce/models/auto_detect_type.py
+-rw-r--r--   0        0        0     3207 2024-04-17 13:57:51.560968 luminesce_sdk-2.1.9/luminesce/models/available_field.py
+-rw-r--r--   0        0        0     2939 2024-04-17 13:57:51.560968 luminesce_sdk-2.1.9/luminesce/models/available_parameter.py
+-rw-r--r--   0        0        0     4237 2024-04-17 13:57:51.560968 luminesce_sdk-2.1.9/luminesce/models/background_multi_query_progress_response.py
+-rw-r--r--   0        0        0    10653 2024-04-17 13:57:51.560968 luminesce_sdk-2.1.9/luminesce/models/background_multi_query_response.py
+-rw-r--r--   0        0        0     2760 2024-04-17 13:57:51.560968 luminesce_sdk-2.1.9/luminesce/models/background_query_cancel_response.py
+-rw-r--r--   0        0        0     5677 2024-04-17 13:57:51.560968 luminesce_sdk-2.1.9/luminesce/models/background_query_progress_response.py
+-rw-r--r--   0        0        0     6285 2024-04-17 13:57:51.560968 luminesce_sdk-2.1.9/luminesce/models/background_query_response.py
+-rw-r--r--   0        0        0     1055 2024-04-17 13:57:51.560968 luminesce_sdk-2.1.9/luminesce/models/background_query_state.py
+-rw-r--r--   0        0        0      808 2024-04-17 13:57:51.560968 luminesce_sdk-2.1.9/luminesce/models/certificate_action.py
+-rw-r--r--   0        0        0      778 2024-04-17 13:57:51.560968 luminesce_sdk-2.1.9/luminesce/models/certificate_file_type.py
+-rw-r--r--   0        0        0     7171 2024-04-17 13:57:51.560968 luminesce_sdk-2.1.9/luminesce/models/certificate_state.py
+-rw-r--r--   0        0        0      847 2024-04-17 13:57:51.561968 luminesce_sdk-2.1.9/luminesce/models/certificate_status.py
+-rw-r--r--   0        0        0      716 2024-04-17 13:57:51.561968 luminesce_sdk-2.1.9/luminesce/models/certificate_type.py
+-rw-r--r--   0        0        0     5108 2024-04-17 13:57:51.561968 luminesce_sdk-2.1.9/luminesce/models/column.py
+-rw-r--r--   0        0        0     2859 2024-04-17 13:57:51.561968 luminesce_sdk-2.1.9/luminesce/models/column_info.py
+-rw-r--r--   0        0        0      738 2024-04-17 13:57:51.561968 luminesce_sdk-2.1.9/luminesce/models/condition_attributes.py
+-rw-r--r--   0        0        0     5193 2024-04-17 13:57:51.561968 luminesce_sdk-2.1.9/luminesce/models/convert_to_view_data.py
+-rw-r--r--   0        0        0     2055 2024-04-17 13:57:51.561968 luminesce_sdk-2.1.9/luminesce/models/cursor_position.py
+-rw-r--r--   0        0        0      789 2024-04-17 13:57:51.561968 luminesce_sdk-2.1.9/luminesce/models/data_type.py
+-rw-r--r--   0        0        0     3345 2024-04-17 13:57:51.561968 luminesce_sdk-2.1.9/luminesce/models/error_highlight_item.py
+-rw-r--r--   0        0        0     2386 2024-04-17 13:57:51.561968 luminesce_sdk-2.1.9/luminesce/models/error_highlight_request.py
+-rw-r--r--   0        0        0     2702 2024-04-17 13:57:51.561968 luminesce_sdk-2.1.9/luminesce/models/error_highlight_response.py
+-rw-r--r--   0        0        0     2589 2024-04-17 13:57:51.562968 luminesce_sdk-2.1.9/luminesce/models/expression_with_alias.py
+-rw-r--r--   0        0        0     4095 2024-04-17 13:57:51.562968 luminesce_sdk-2.1.9/luminesce/models/feedback_event_args.py
+-rw-r--r--   0        0        0      994 2024-04-17 13:57:51.562968 luminesce_sdk-2.1.9/luminesce/models/feedback_level.py
+-rw-r--r--   0        0        0     4548 2024-04-17 13:57:51.562968 luminesce_sdk-2.1.9/luminesce/models/field_design.py
+-rw-r--r--   0        0        0      654 2024-04-17 13:57:51.562968 luminesce_sdk-2.1.9/luminesce/models/field_type.py
+-rw-r--r--   0        0        0     8355 2024-04-17 13:57:51.562968 luminesce_sdk-2.1.9/luminesce/models/file_reader_builder_def.py
+-rw-r--r--   0        0        0     3731 2024-04-17 13:57:51.562968 luminesce_sdk-2.1.9/luminesce/models/file_reader_builder_response.py
+-rw-r--r--   0        0        0     2210 2024-04-17 13:57:51.562968 luminesce_sdk-2.1.9/luminesce/models/filter_term_design.py
+-rw-r--r--   0        0        0     3180 2024-04-17 13:57:51.562968 luminesce_sdk-2.1.9/luminesce/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3236 2024-04-17 13:57:51.562968 luminesce_sdk-2.1.9/luminesce/models/intellisense_item.py
+-rw-r--r--   0        0        0     2405 2024-04-17 13:57:51.562968 luminesce_sdk-2.1.9/luminesce/models/intellisense_request.py
+-rw-r--r--   0        0        0     3144 2024-04-17 13:57:51.562968 luminesce_sdk-2.1.9/luminesce/models/intellisense_response.py
+-rw-r--r--   0        0        0      807 2024-04-17 13:57:51.562968 luminesce_sdk-2.1.9/luminesce/models/intellisense_type.py
+-rw-r--r--   0        0        0     2267 2024-04-17 13:57:51.562968 luminesce_sdk-2.1.9/luminesce/models/link.py
+-rw-r--r--   0        0        0     1656 2024-04-17 13:57:51.562968 luminesce_sdk-2.1.9/luminesce/models/luminesce_binary_type.py
+-rw-r--r--   0        0        0     3862 2024-04-17 13:57:51.562968 luminesce_sdk-2.1.9/luminesce/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     5204 2024-04-17 13:57:51.562968 luminesce_sdk-2.1.9/luminesce/models/mappable_field.py
+-rw-r--r--   0        0        0      711 2024-04-17 13:57:51.562968 luminesce_sdk-2.1.9/luminesce/models/mapping_flags.py
+-rw-r--r--   0        0        0     1099 2024-04-17 13:57:51.562968 luminesce_sdk-2.1.9/luminesce/models/multi_query_definition_type.py
+-rw-r--r--   0        0        0     6322 2024-04-17 13:57:51.563968 luminesce_sdk-2.1.9/luminesce/models/options_csv.py
+-rw-r--r--   0        0        0     5383 2024-04-17 13:57:51.563968 luminesce_sdk-2.1.9/luminesce/models/options_excel.py
+-rw-r--r--   0        0        0     2313 2024-04-17 13:57:51.563968 luminesce_sdk-2.1.9/luminesce/models/options_parquet.py
+-rw-r--r--   0        0        0     2219 2024-04-17 13:57:51.563968 luminesce_sdk-2.1.9/luminesce/models/options_sq_lite.py
+-rw-r--r--   0        0        0     4491 2024-04-17 13:57:51.563968 luminesce_sdk-2.1.9/luminesce/models/options_xml.py
+-rw-r--r--   0        0        0      707 2024-04-17 13:57:51.563968 luminesce_sdk-2.1.9/luminesce/models/order_by_direction.py
+-rw-r--r--   0        0        0     2149 2024-04-17 13:57:51.563968 luminesce_sdk-2.1.9/luminesce/models/order_by_term_design.py
+-rw-r--r--   0        0        0     5696 2024-04-17 13:57:51.563968 luminesce_sdk-2.1.9/luminesce/models/query_design.py
+-rw-r--r--   0        0        0      884 2024-04-17 13:57:51.563968 luminesce_sdk-2.1.9/luminesce/models/query_designer_binary_operator.py
+-rw-r--r--   0        0        0     4250 2024-04-17 13:57:51.563968 luminesce_sdk-2.1.9/luminesce/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     2328 2024-04-17 13:57:51.563968 luminesce_sdk-2.1.9/luminesce/models/source.py
+-rw-r--r--   0        0        0      770 2024-04-17 13:57:51.563968 luminesce_sdk-2.1.9/luminesce/models/source_type.py
+-rw-r--r--   0        0        0      897 2024-04-17 13:57:51.563968 luminesce_sdk-2.1.9/luminesce/models/task_status.py
+-rw-r--r--   0        0        0     2991 2024-04-17 13:57:51.563968 luminesce_sdk-2.1.9/luminesce/models/view_parameter.py
+-rw-r--r--   0        0        0     4494 2024-04-17 13:57:51.563968 luminesce_sdk-2.1.9/luminesce/models/writer_design.py
+-rw-r--r--   0        0        0        0 2024-04-17 13:57:51.565968 luminesce_sdk-2.1.9/luminesce/py.typed
+-rw-r--r--   0        0        0    10160 2024-04-17 13:57:51.564968 luminesce_sdk-2.1.9/luminesce/rest.py
+-rw-r--r--   0        0        0      846 2024-04-17 13:57:51.573968 luminesce_sdk-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0    22845 1970-01-01 00:00:00.000000 luminesce_sdk-2.1.9/PKG-INFO
```

### Comparing `luminesce_sdk-2.1.8/README.md` & `luminesce_sdk-2.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # luminesce-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.15.14
-- Package version: 2.1.8
+- API version: 1.15.32
+- Package version: 2.1.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `luminesce_sdk-2.1.8/luminesce/__init__.py` & `luminesce_sdk-2.1.9/luminesce/__init__.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/api/__init__.py` & `luminesce_sdk-2.1.9/luminesce/api/__init__.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/api/application_metadata_api.py` & `luminesce_sdk-2.1.9/luminesce/api/application_metadata_api.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/api/binary_downloading_api.py` & `luminesce_sdk-2.1.9/luminesce/api/binary_downloading_api.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/api/certificate_management_api.py` & `luminesce_sdk-2.1.9/luminesce/api/certificate_management_api.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/api/current_table_field_catalog_api.py` & `luminesce_sdk-2.1.9/luminesce/api/current_table_field_catalog_api.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/api/historically_executed_queries_api.py` & `luminesce_sdk-2.1.9/luminesce/api/historically_executed_queries_api.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/api/multi_query_execution_api.py` & `luminesce_sdk-2.1.9/luminesce/api/multi_query_execution_api.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/api/sql_background_execution_api.py` & `luminesce_sdk-2.1.9/luminesce/api/sql_background_execution_api.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/api/sql_design_api.py` & `luminesce_sdk-2.1.9/luminesce/api/sql_design_api.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/api/sql_execution_api.py` & `luminesce_sdk-2.1.9/luminesce/api/sql_execution_api.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/api_client.py` & `luminesce_sdk-2.1.9/luminesce/api_client.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/api_response.py` & `luminesce_sdk-2.1.9/luminesce/api_response.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/configuration.py` & `luminesce_sdk-2.1.9/luminesce/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("luminesce-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.15.14\n"\
+               "Version of the API: 1.15.32\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `luminesce_sdk-2.1.8/luminesce/exceptions.py` & `luminesce_sdk-2.1.9/luminesce/exceptions.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/extensions/__init__.py` & `luminesce_sdk-2.1.9/luminesce/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/extensions/api_client.py` & `luminesce_sdk-2.1.9/luminesce/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/extensions/api_client_factory.py` & `luminesce_sdk-2.1.9/luminesce/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/extensions/api_configuration.py` & `luminesce_sdk-2.1.9/luminesce/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/extensions/configuration_loaders.py` & `luminesce_sdk-2.1.9/luminesce/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/extensions/proxy_config.py` & `luminesce_sdk-2.1.9/luminesce/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/extensions/refreshing_token.py` & `luminesce_sdk-2.1.9/luminesce/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/extensions/rest.py` & `luminesce_sdk-2.1.9/luminesce/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/extensions/retry.py` & `luminesce_sdk-2.1.9/luminesce/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/extensions/socket_keep_alive.py` & `luminesce_sdk-2.1.9/luminesce/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/extensions/tcp_keep_alive_connector.py` & `luminesce_sdk-2.1.9/luminesce/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/__init__.py` & `luminesce_sdk-2.1.9/luminesce/models/__init__.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/access_controlled_action.py` & `luminesce_sdk-2.1.9/luminesce/models/access_controlled_action.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/access_controlled_resource.py` & `luminesce_sdk-2.1.9/luminesce/models/access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/access_controlled_resource_identifier_part_schema_attribute.py` & `luminesce_sdk-2.1.9/luminesce/models/access_controlled_resource_identifier_part_schema_attribute.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/action_id.py` & `luminesce_sdk-2.1.9/luminesce/models/action_id.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/aggregate_function.py` & `luminesce_sdk-2.1.9/luminesce/models/aggregate_function.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/aggregation.py` & `luminesce_sdk-2.1.9/luminesce/models/aggregation.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/auto_detect_type.py` & `luminesce_sdk-2.1.9/luminesce/models/auto_detect_type.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/available_field.py` & `luminesce_sdk-2.1.9/luminesce/models/available_field.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/available_parameter.py` & `luminesce_sdk-2.1.9/luminesce/models/available_parameter.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/background_multi_query_progress_response.py` & `luminesce_sdk-2.1.9/luminesce/models/background_multi_query_progress_response.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/background_multi_query_response.py` & `luminesce_sdk-2.1.9/luminesce/models/background_multi_query_response.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/background_query_cancel_response.py` & `luminesce_sdk-2.1.9/luminesce/models/background_query_cancel_response.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/background_query_progress_response.py` & `luminesce_sdk-2.1.9/luminesce/models/background_query_progress_response.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/background_query_response.py` & `luminesce_sdk-2.1.9/luminesce/models/background_query_response.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/background_query_state.py` & `luminesce_sdk-2.1.9/luminesce/models/background_query_state.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/certificate_action.py` & `luminesce_sdk-2.1.9/luminesce/models/certificate_action.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/certificate_file_type.py` & `luminesce_sdk-2.1.9/luminesce/models/certificate_file_type.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/certificate_state.py` & `luminesce_sdk-2.1.9/luminesce/models/certificate_state.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/certificate_status.py` & `luminesce_sdk-2.1.9/luminesce/models/certificate_status.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/certificate_type.py` & `luminesce_sdk-2.1.9/luminesce/models/certificate_type.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/column.py` & `luminesce_sdk-2.1.9/luminesce/models/column.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/column_info.py` & `luminesce_sdk-2.1.9/luminesce/models/column_info.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/condition_attributes.py` & `luminesce_sdk-2.1.9/luminesce/models/condition_attributes.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/convert_to_view_data.py` & `luminesce_sdk-2.1.9/luminesce/models/convert_to_view_data.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/cursor_position.py` & `luminesce_sdk-2.1.9/luminesce/models/cursor_position.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/data_type.py` & `luminesce_sdk-2.1.9/luminesce/models/data_type.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/error_highlight_item.py` & `luminesce_sdk-2.1.9/luminesce/models/error_highlight_item.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/error_highlight_request.py` & `luminesce_sdk-2.1.9/luminesce/models/error_highlight_request.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/error_highlight_response.py` & `luminesce_sdk-2.1.9/luminesce/models/error_highlight_response.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/expression_with_alias.py` & `luminesce_sdk-2.1.9/luminesce/models/expression_with_alias.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/feedback_event_args.py` & `luminesce_sdk-2.1.9/luminesce/models/feedback_event_args.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/feedback_level.py` & `luminesce_sdk-2.1.9/luminesce/models/feedback_level.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/field_design.py` & `luminesce_sdk-2.1.9/luminesce/models/field_design.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/field_type.py` & `luminesce_sdk-2.1.9/luminesce/models/field_type.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/file_reader_builder_def.py` & `luminesce_sdk-2.1.9/luminesce/models/file_reader_builder_def.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/file_reader_builder_response.py` & `luminesce_sdk-2.1.9/luminesce/models/file_reader_builder_response.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/filter_term_design.py` & `luminesce_sdk-2.1.9/luminesce/models/filter_term_design.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/id_selector_definition.py` & `luminesce_sdk-2.1.9/luminesce/models/id_selector_definition.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/intellisense_item.py` & `luminesce_sdk-2.1.9/luminesce/models/intellisense_item.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/intellisense_request.py` & `luminesce_sdk-2.1.9/luminesce/models/intellisense_request.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/intellisense_response.py` & `luminesce_sdk-2.1.9/luminesce/models/intellisense_response.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/intellisense_type.py` & `luminesce_sdk-2.1.9/luminesce/models/intellisense_type.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/link.py` & `luminesce_sdk-2.1.9/luminesce/models/link.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/luminesce_binary_type.py` & `luminesce_sdk-2.1.9/luminesce/models/luminesce_binary_type.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/lusid_problem_details.py` & `luminesce_sdk-2.1.9/luminesce/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/mappable_field.py` & `luminesce_sdk-2.1.9/luminesce/models/mappable_field.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/mapping_flags.py` & `luminesce_sdk-2.1.9/luminesce/models/mapping_flags.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/multi_query_definition_type.py` & `luminesce_sdk-2.1.9/luminesce/models/multi_query_definition_type.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/options_csv.py` & `luminesce_sdk-2.1.9/luminesce/models/options_csv.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/options_excel.py` & `luminesce_sdk-2.1.9/luminesce/models/options_excel.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/options_parquet.py` & `luminesce_sdk-2.1.9/luminesce/models/options_parquet.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/options_sq_lite.py` & `luminesce_sdk-2.1.9/luminesce/models/options_sq_lite.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/options_xml.py` & `luminesce_sdk-2.1.9/luminesce/models/options_xml.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/order_by_direction.py` & `luminesce_sdk-2.1.9/luminesce/models/order_by_direction.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/order_by_term_design.py` & `luminesce_sdk-2.1.9/luminesce/models/order_by_term_design.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/query_design.py` & `luminesce_sdk-2.1.9/luminesce/models/query_design.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/query_designer_binary_operator.py` & `luminesce_sdk-2.1.9/luminesce/models/query_designer_binary_operator.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/resource_list_of_access_controlled_resource.py` & `luminesce_sdk-2.1.9/luminesce/models/resource_list_of_access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/source.py` & `luminesce_sdk-2.1.9/luminesce/models/source.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/source_type.py` & `luminesce_sdk-2.1.9/luminesce/models/source_type.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/task_status.py` & `luminesce_sdk-2.1.9/luminesce/models/task_status.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/view_parameter.py` & `luminesce_sdk-2.1.9/luminesce/models/view_parameter.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/models/writer_design.py` & `luminesce_sdk-2.1.9/luminesce/models/writer_design.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/luminesce/rest.py` & `luminesce_sdk-2.1.9/luminesce/rest.py`

 * *Files identical despite different names*

### Comparing `luminesce_sdk-2.1.8/pyproject.toml` & `luminesce_sdk-2.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "luminesce-sdk"
-version = "2.1.8"
+version = "2.1.9"
 description = "FINBOURNE Luminesce Web API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/luminesce-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Luminesce Web API", "luminesce-sdk"]
 packages = [
```

### Comparing `luminesce_sdk-2.1.8/PKG-INFO` & `luminesce_sdk-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luminesce-sdk
-Version: 2.1.8
+Version: 2.1.9
 Summary: FINBOURNE Luminesce Web API
 Home-page: https://github.com/finbourne/luminesce-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Luminesce Web API,luminesce-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # luminesce-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 1.15.14
-- Package version: 2.1.8
+- API version: 1.15.32
+- Package version: 2.1.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

